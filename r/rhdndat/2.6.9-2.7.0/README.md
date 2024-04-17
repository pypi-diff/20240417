# Comparing `tmp/rhdndat-2.6.9.tar.gz` & `tmp/rhdndat-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rhdndat-2.6.9.tar", max compression
+gzip compressed data, was "rhdndat-2.7.0.tar", max compression
```

## Comparing `rhdndat-2.6.9.tar` & `rhdndat-2.7.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35150 2023-06-19 23:15:10.262670 rhdndat-2.6.9/LICENSE.txt
--rw-r--r--   0        0        0     7909 2023-06-19 23:15:10.262670 rhdndat-2.6.9/README.rst
--rw-r--r--   0        0        0      906 2023-06-19 23:15:10.262670 rhdndat-2.6.9/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-19 23:15:10.262670 rhdndat-2.6.9/rhdndat/__init__.py
--rw-r--r--   0        0        0    39110 2023-06-19 23:15:10.262670 rhdndat-2.6.9/rhdndat/__main__.py
--rw-r--r--   0        0        0     9055 2023-06-19 23:15:19.701110 rhdndat-2.6.9/setup.py
--rw-r--r--   0        0        0     8976 2023-06-19 23:15:19.702194 rhdndat-2.6.9/PKG-INFO
+-rw-r--r--   0        0        0    35150 2024-04-17 07:01:41.785178 rhdndat-2.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     7909 2024-04-17 07:01:41.785178 rhdndat-2.7.0/README.rst
+-rw-r--r--   0        0        0      927 2024-04-17 07:01:41.785178 rhdndat-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-17 07:01:41.785178 rhdndat-2.7.0/rhdndat/__init__.py
+-rw-r--r--   0        0        0    39185 2024-04-17 07:01:41.785178 rhdndat-2.7.0/rhdndat/__main__.py
+-rw-r--r--   0        0        0     9083 2024-04-17 07:01:53.256140 rhdndat-2.7.0/setup.py
+-rw-r--r--   0        0        0     9018 2024-04-17 07:01:53.256981 rhdndat-2.7.0/PKG-INFO
```

### Comparing `rhdndat-2.6.9/LICENSE.txt` & `rhdndat-2.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rhdndat-2.6.9/README.rst` & `rhdndat-2.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `rhdndat-2.6.9/pyproject.toml` & `rhdndat-2.7.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "rhdndat"
-version = "2.6.9"
+version = "2.7.0"
 description = "www.romhacking.net update checker"
 authors = ["i30817 <i30817@gmail.com>"]
 license = "GNU General Public License v3.0"
 readme = "README.rst"
 repository = "https://github.com/i30817/rhdndat"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 beautifulsoup4 = "^4.10.0"
 questionary = "^1.10.0"
 typer = "^0.9.0"
 colorama = "^0.4.4"
 lxml = "^4.9.1"
+requests = "^2.31.0"
 xattr = [
     { version = "^0.9.9", markers = "sys_platform != 'win32'" },
 ]
 
 [tool.poetry.scripts]
 rhdndat = 'rhdndat.__main__:main'
 rhdndat-rn = 'rhdndat.__main__:rename'
```

### Comparing `rhdndat-2.6.9/rhdndat/__main__.py` & `rhdndat-2.7.0/rhdndat/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 import sys
 import os
 import subprocess
 import urllib
 import shutil
 import tempfile
 import mimetypes
-from urllib.parse import urlparse
-from urllib.request import urlopen
-from urllib.error import URLError
+import requests
 from pathlib import Path
 from hashlib import sha1
 import re
 import signal
 import typer
 from io import DEFAULT_BUFFER_SIZE
 from itertools import chain
@@ -86,22 +84,21 @@
 
     while len(buf) > 0:
         hash_sha1.update(buf)
         buf = yield
 
     yield hash_sha1.hexdigest()
 
-def link(uri, label=None, parameters=None):
+def link(uri, label=None, parameters=''):
     '''
     Found in github, windows console and many unix consoles trick to embeed hyperlinks/uri with text
+    https://gist.github.com/egmontkob/eb114294efbcd5adb1944c9f3cb5feda
     '''
     if label is None:
         label = uri
-    if parameters is None:
-        parameters = ''
     # OSC 8 ; params ; URI ST <name> OSC 8 ;; ST
     escape_mask = '\033]8;{};{}\033\\{}\033]8;;\033\\'
     return escape_mask.format(parameters, uri, label)
 
 def file_producer(source_filename, generator_function):
     next(generator_function)
     with open(source_filename, 'rb') as f:
@@ -606,26 +603,27 @@
                 hacks_list += [(version, url)]
     except Exception as e:
         raise VersionFileSyntaxError(possible_metadata)
     if not hacks_list:
         raise VersionFileSyntaxError(possible_metadata)
     return hacks_list
 
-def get_romhacking_data(possible_metadata):
+def get_romhacking_data(possible_metadata, session):
     ''' returns the tuple (metadata, language)
         metadata is a list of (title, authors_string, version, url) 1 for each hack
         language is the last language of the hacks
     '''
     metadata = []
     language = None
     version_hacks = read_version_file(possible_metadata)
 
     for (version, url) in version_hacks:
         try:
-            page = urlopen(url).read()
+            response = session.get(url, headers={'User-Agent': 'Mozilla/5.0'})
+            page = response.text
             soup = BeautifulSoup(page, 'lxml')
 
             #removed hacks from romhacking.net can be bad news, broken or malicious hacks
             #warn the user to verify if he might have to remove the hack from the merge file
             check_removed = soup.find('div', id='main')
             if check_removed:
                 check_removed = check_removed.find('div', class_='topbar', string='Error Encountered!')
@@ -648,27 +646,27 @@
                 authors = authors.findAll('a')
                 authors_str = authors[0].string
                 for author in authors[1:-1]:
                     authors_str += ', {}'.format(author.string)
                 authors_str += ' and {}'.format(authors[-1].string)
 
             metadata += [(
-                info.find('div').find('div').string, #main title
+                info.find('div').string, #main title
                 authors_str,
                 version, #the version we actually have
                 url
             )]
 
             remote_version = info.find('th', string='Patch Version').nextSibling.string.strip()
             if not remote_version:
                 raise VersionFileURLError(possible_metadata, url)
 
             if remote_version != version:
                 warn(f'warn: local \'{version}\' {link(possible_metadata.parent.as_uri(),"(open dir)")} != remote \'{remote_version}\' {link(url, "(open url)")} versions')
-        except (URLError, AttributeError) as e:
+        except (requests.exceptions.RequestException, AttributeError) as e:
             raise VersionFileURLError(possible_metadata, url)
     return (metadata, language)
 
 
 def versioncheck(romdir: Path = typer.Argument(..., exists=True, file_okay=False, dir_okay=True, readable=True, resolve_path=True, help='Directory to search for versions to check.'),
     show: bool = typer.Option(False, '--show', help='Show link to each checked directory.')
     ):
@@ -682,19 +680,20 @@
     To update this program to the latest release with pip installed, type:
     
     pip install --force-reinstall rhdndat
     """
     
     versions = romdir.glob("**/rhdndat.ver")
     try:
+        session = requests.Session()
         for possible_metadata in versions:
             if show:
                 log(f'check: {link(possible_metadata.parent.as_uri(),possible_metadata.parent.name + " (open dir)")}') 
             try:
-                get_romhacking_data(possible_metadata)
+                get_romhacking_data(possible_metadata, session)
             except RHDNTRomRemovedError as e:
                 error(f'error: romhacking.net deleted the patch {link(e.url, "(open url)")} check reason and consider deletion {link(e.versionfile.parent.as_uri(),"(open dir)")}')
     #fatal errors
     except VersionFileURLError as e:
         error(f'error: rhdndat.ver file {link(e.versionfile.as_uri(), "(open file)")} had a connection failure {link(e.url, "(open url)")}')
         raise typer.Abort()
     except VersionFileSyntaxError as e:
```

### Comparing `rhdndat-2.6.9/setup.py` & `rhdndat-2.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,26 +8,27 @@
 {'': ['*']}
 
 install_requires = \
 ['beautifulsoup4>=4.10.0,<5.0.0',
  'colorama>=0.4.4,<0.5.0',
  'lxml>=4.9.1,<5.0.0',
  'questionary>=1.10.0,<2.0.0',
+ 'requests>=2.31.0,<3.0.0',
  'typer>=0.9.0,<0.10.0']
 
 extras_require = \
 {':sys_platform != "win32"': ['xattr>=0.9.9,<0.10.0']}
 
 entry_points = \
 {'console_scripts': ['rhdndat = rhdndat.__main__:main',
                      'rhdndat-rn = rhdndat.__main__:rename']}
 
 setup_kwargs = {
     'name': 'rhdndat',
-    'version': '2.6.9',
+    'version': '2.7.0',
     'description': 'www.romhacking.net update checker',
     'long_description': "romhacking.net_ update checker and rom renamer\n==============================================\n\n.. _romhacking.net: http://www.romhacking.net\n\n\n**rhdndat** finds ``rhdndat.ver`` files to check for romhacking.net updates\n\nA version file is named ``rhdndat.ver`` and has a version number line followed by a romhacking.net url line, repeated. These correspond to each hack or translation. To check for needed updates to version file, if any patch version in the file does not match the version on the romhacking.net patch page, it presents a warning.\n\n**rhdndat-rn** renames files and patches to new .DAT [1]_ [2]_ rom names if it can find the rom checksum in those .DAT files and memorizes the checksum of the 'original rom' as a extended attribute ``user.rhdndat.rom_sha1`` to speed up renaming in subsequent executions (in unix, not windows).\n\nTo find the checksum of the original file for hardpatched roms, rhdndat-rn can support a custom convention for 'revert patches'. Revert patches are a patch that you apply to a hardpatched file to get the original. These have the same name as the file and extension '.rxdelta' and are done with xdelta3. I keep them for patch updates for cd images (since delta chd support is rare).\n\nrhdndat-rn will read a xml dat file or every dat file from a directory given, and ask for renaming for every match where the rom filename is not equal to the dat name proposed. It will skip the question if all the names proposed already exist in the rom directory, and not allow a rename to a existing file in the rom directory.\n\nBesides bare rom files, files affected by renames are compressed wii/gamecube .rvz files, .cue/.toc/.gdi (treated especially to not ask for every track), the softpatch types .ips, .bps, .ups, including the new retroarch multiple softpatch convention (a number after the softpatch extension), .rxdelta, .pal NES color palettes, and sbi subchannel data files.\n\n``nes fds lnx a78`` roms require headers and are hardcoded to ignore headers when calculating ``user.rhdndat.rom_sha1`` to match the no-intro dat checksums that checksum everything except the header. This is problematic for hacks, where you can 'verify' a file is the right rom, but the hack was created for a rom with another header. A solution that keeps the softpatch is tracking down the right rom, hardpatching it, and creating a softpatch from the current no-intro rom to the older patched rom. For sfc and pce ips hacks that target a headered rom I recommend ipsbehead to change the patch to target the no-header rom.\n\nRequires xdelta3 (to process rxdelta) and dolphin-tool (to operate on rvz files) on path or the same directory.\n\nTo check for updates if you have the version files:\n\n``rhdndat romdir``\n                        check if there are any updates\n\nTo rename files if you have the dat files:\n\n``rhdndat-rn [--force] [--ext a78 --ext nes ...] romdir xmlpath``\n                        the rom extensions should be all file extensions on the files you want to rename (see below for default)\n\nrhdndat [OPTIONS] ROMDIR\n  :ROMDIR:  Directory to search for versions to check.  [required]\n\n  --show                Show link to each checked directory.\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or\n                        customize the installation.\n  --help                Show this message and exit.\n\n\nrhdndat-rn [OPTIONS] ROMDIR XMLPATH\n  :ROMDIR:  Directory to search for roms to rename.  [required]\n  \n  :XMLPATH: Xml dat file or directory to search for xml dat files to use as source of new names.  [required]\n\n  --skip DIRECTORY      Directory to skip, can be repeated.\n  --ext TEXT            ROM extensions to find names of, can be\n                        repeated. Note that you can ommit this\n                        argument to get the predefined list.\n                        [default: a78, hdi, fdi, ngc, ws, wsc, pce,\n                        gb, gba, gbc, n64, v64, z64, 3ds, nds, nes,\n                        lnx, fds, sfc, smc, bs, nsp, 32x, gg, sms,\n                        md, iso, dim, adf, ipf, dsi, wad, cue, gdi,\n                        toc, rvz]\n  --force               Force a recalculation and store of checksum\n                        (on windows the calculation always happens).\n  --no-rename           Check and store checksums only.\n  --verbose             Print more information about skipped roms.\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or\n                        customize the installation.\n  --help                Show this message and exit.\n\n\n.. [1] `scroll down and click 'prepare' to get a collection of cartidge rom .DAT files <https://datomatic.no-intro.org/index.php?page=download&s=64&op=daily>`_.\n.. [2] `download cd/dvd roms .DAT files here <http://redump.org/downloads/>`_.\n\nInstall\n-------\n\nrhdndat requires python 3.8 or later.\n\nrhdndat may fail to execute in linux if the dir ``~/.local/bin`` to is not in the ``$PATH``.\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python. \n\nThe project can be installed with pip but you'll have to provide your own xdelta3 and dolphin-tool executables in the path (or current dir) for supporting rvz and rxdelta.\n\nIn linux just installing xdelta3 from the repositories is enough, in windows, placing a executable for xdelta3 named ``xdelta3.exe`` in the python install ``Scripts`` directory if you installed with the path option selected is enough.\n\nIn linux you'll have to build dolphin-tool (it's not built by dolphin-emu packages) and place it in ``~/.local/bin``, and in windows you can copy it from the dolphin install directory, rename it to ``dolphin-tool.exe`` and place it in the python install ``Scripts`` directory.\n\n\n+----------------+----------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall rhdndat``                                              |\n+----------------+----------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/rhdndat/archive/master.zip`` |\n+----------------+----------------------------------------------------------------------------------------+\n\nLinks\n-----\n\n.. class:: tablacreditos\n\n+-------------------------------------------------------+----------------------------------------------+\n| Alcaro for helpful comments and for flips             | https://github.com/Alcaro/Flips              |\n+-------------------------------------------------------+----------------------------------------------+\n| romhacking.net for being awesome                      | http://www.romhacking.net/                   |\n+-------------------------------------------------------+----------------------------------------------+\n| Turn sfc and pce ips header patches to no-header      | https://github.com/heuripedes/ipsbehead      |\n| patches                                               |                                              |\n+-------------------------------------------------------+----------------------------------------------+\n| Remember to rename to xdelta3 and place in path       | https://github.com/jmacd/xdelta-gpl/releases |\n+-------------------------------------------------------+----------------------------------------------+\n| Remember to rename to dolphin-tool and place in path, | https://dolphin-emu.org/download/            |\n| linux requires build                                  |                                              |\n+-------------------------------------------------------+----------------------------------------------+\n\n`The source for this project is available here\n<https://github.com/i30817/rhdndat>`_.\n",
     'author': 'i30817',
     'author_email': 'i30817@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/i30817/rhdndat',
```

### Comparing `rhdndat-2.6.9/PKG-INFO` & `rhdndat-2.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rhdndat
-Version: 2.6.9
+Version: 2.7.0
 Summary: www.romhacking.net update checker
 Home-page: https://github.com/i30817/rhdndat
 License: GNU General Public License v3.0
 Author: i30817
 Author-email: i30817@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: beautifulsoup4 (>=4.10.0,<5.0.0)
 Requires-Dist: colorama (>=0.4.4,<0.5.0)
 Requires-Dist: lxml (>=4.9.1,<5.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: xattr (>=0.9.9,<0.10.0); sys_platform != "win32"
 Project-URL: Bug Tracker, https://github.com/i30817/rhdndat/issues
 Project-URL: Repository, https://github.com/i30817/rhdndat
 Project-URL: documentation, https://github.com/i30817/rhdndat#readme
 Project-URL: homepage, https://github.com/i30817/rhdndat
 Description-Content-Type: text/x-rst
```

