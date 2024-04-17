# Comparing `tmp/mediawiki_dump-1.2.0.tar.gz` & `tmp/mediawiki_dump-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mediawiki_dump-1.2.0.tar", last modified: Tue Sep 26 12:29:02 2023, max compression
+gzip compressed data, was "mediawiki_dump-1.2.1.tar", last modified: Wed Apr 17 09:22:02 2024, max compression
```

## Comparing `mediawiki_dump-1.2.0.tar` & `mediawiki_dump-1.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:29:02.408038 mediawiki_dump-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-09-26 12:28:50.000000 mediawiki_dump-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-09-26 12:28:50.000000 mediawiki_dump-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8315 2023-09-26 12:29:02.408038 mediawiki_dump-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7698 2023-09-26 12:28:50.000000 mediawiki_dump-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:29:02.408038 mediawiki_dump-1.2.0/mediawiki_dump/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-26 12:28:50.000000 mediawiki_dump-1.2.0/mediawiki_dump/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7881 2023-09-26 12:28:50.000000 mediawiki_dump-1.2.0/mediawiki_dump/dumps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2023-09-26 12:28:50.000000 mediawiki_dump-1.2.0/mediawiki_dump/entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9147 2023-09-26 12:28:50.000000 mediawiki_dump-1.2.0/mediawiki_dump/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2023-09-26 12:28:50.000000 mediawiki_dump-1.2.0/mediawiki_dump/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-09-26 12:28:50.000000 mediawiki_dump-1.2.0/mediawiki_dump/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:29:02.408038 mediawiki_dump-1.2.0/mediawiki_dump.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8315 2023-09-26 12:29:02.000000 mediawiki_dump-1.2.0/mediawiki_dump.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      379 2023-09-26 12:29:02.000000 mediawiki_dump-1.2.0/mediawiki_dump.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-26 12:29:02.000000 mediawiki_dump-1.2.0/mediawiki_dump.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-09-26 12:29:02.000000 mediawiki_dump-1.2.0/mediawiki_dump.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-09-26 12:29:02.000000 mediawiki_dump-1.2.0/mediawiki_dump.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-26 12:29:02.408038 mediawiki_dump-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2023-09-26 12:28:50.000000 mediawiki_dump-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:02.112660 mediawiki_dump-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-17 09:21:54.000000 mediawiki_dump-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-17 09:21:54.000000 mediawiki_dump-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8693 2024-04-17 09:22:02.112660 mediawiki_dump-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-04-17 09:21:54.000000 mediawiki_dump-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:02.108660 mediawiki_dump-1.2.1/mediawiki_dump/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:21:54.000000 mediawiki_dump-1.2.1/mediawiki_dump/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-04-17 09:21:54.000000 mediawiki_dump-1.2.1/mediawiki_dump/dumps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-17 09:21:54.000000 mediawiki_dump-1.2.1/mediawiki_dump/entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-04-17 09:21:54.000000 mediawiki_dump-1.2.1/mediawiki_dump/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-17 09:21:54.000000 mediawiki_dump-1.2.1/mediawiki_dump/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-17 09:21:54.000000 mediawiki_dump-1.2.1/mediawiki_dump/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:22:02.112660 mediawiki_dump-1.2.1/mediawiki_dump.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8693 2024-04-17 09:22:02.000000 mediawiki_dump-1.2.1/mediawiki_dump.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-17 09:22:02.000000 mediawiki_dump-1.2.1/mediawiki_dump.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:22:02.000000 mediawiki_dump-1.2.1/mediawiki_dump.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-17 09:22:02.000000 mediawiki_dump-1.2.1/mediawiki_dump.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-17 09:22:02.000000 mediawiki_dump-1.2.1/mediawiki_dump.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 09:22:02.112660 mediawiki_dump-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-17 09:21:54.000000 mediawiki_dump-1.2.1/setup.py
```

### Comparing `mediawiki_dump-1.2.0/LICENSE` & `mediawiki_dump-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mediawiki_dump-1.2.0/PKG-INFO` & `mediawiki_dump-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 Metadata-Version: 2.1
 Name: mediawiki_dump
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python package for working with MediaWiki XML content dumps
 Home-page: https://github.com/macbre/mediawiki-dump
 Author: Maciej Brencz
 Author-email: maciej.brencz@gmail.com
 License: MIT
 Keywords: dump fandom mediawiki wikipedia wikia
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Text Processing :: Markup :: XML
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: libarchive-c==5.1
+Requires-Dist: requests>=2.26.0
+Requires-Dist: mwclient>=0.10.1
+Provides-Extra: dev
+Requires-Dist: black==24.4.0; extra == "dev"
+Requires-Dist: coveralls==3.3.1; extra == "dev"
+Requires-Dist: pylint==3.1.0; extra == "dev"
+Requires-Dist: pytest==8.1.1; extra == "dev"
+Requires-Dist: pytest-cov==5.0.0; extra == "dev"
+Requires-Dist: responses==0.25.0; extra == "dev"
 
 # mediawiki-dump
 [![PyPI](https://img.shields.io/pypi/v/mediawiki_dump.svg)](https://pypi.python.org/pypi/mediawiki_dump)
 [![Downloads](https://pepy.tech/badge/mediawiki_dump)](https://pepy.tech/project/mediawiki_dump)
 [![CI](https://github.com/macbre/mediawiki-dump/actions/workflows/tests.yml/badge.svg)](https://github.com/macbre/mediawiki-dump/actions/workflows/tests.yml)
 [![Coverage Status](https://coveralls.io/repos/github/macbre/mediawiki-dump/badge.svg?branch=master)](https://coveralls.io/github/macbre/mediawiki-dump?branch=master)
```

### Comparing `mediawiki_dump-1.2.0/README.md` & `mediawiki_dump-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mediawiki_dump-1.2.0/mediawiki_dump/dumps.py` & `mediawiki_dump-1.2.1/mediawiki_dump/dumps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 CLasses that support fetching dumps
 """
+
 import bz2
 import logging
 
 from typing import Generator, Iterator
 
 from hashlib import md5
 from os.path import isfile
@@ -35,17 +36,17 @@
         :type wiki str
         :type full_history bool
         """
         self.wiki = wiki
         self.logger = logging.getLogger(self.__class__.__name__)
 
         self.http = requests.session()
-        self.http.headers[
-            "User-Agent"
-        ] = "python-mediawiki-dump (+https://github.com/macbre/mediawiki-dump)"
+        self.http.headers["User-Agent"] = (
+            "python-mediawiki-dump (+https://github.com/macbre/mediawiki-dump)"
+        )
 
         # do we want a full history or just the latest revisions?
         self.full_history = full_history
 
     def get_cache_filename(self, url):
         """
         Return a hashed filename of cache entry for a given URL
@@ -170,16 +171,15 @@
         except AttributeError as ex:
             # AttributeError: undefined symbol: archive_errno
             raise DumpError("Failed to import libarchive with 7zip support") from ex
 
         with self.fetch() as handler:
             with libarchive.file_reader(handler.name) as archive:
                 for entry in archive:
-                    for block in entry.get_blocks():
-                        yield block
+                    yield from entry.get_blocks()
 
 
 class LocalFileDump(BaseDump):
     """
     This class can be used to load locally stored XML dump file
     """
```

### Comparing `mediawiki_dump-1.2.0/mediawiki_dump/entry.py` & `mediawiki_dump-1.2.1/mediawiki_dump/entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 A class representing dump entry
 """
+
 from .utils import parse_date_string
 
 
 # pylint: disable=too-many-instance-attributes
 class DumpEntry:
     """
     An entry in XML dump
```

### Comparing `mediawiki_dump-1.2.0/mediawiki_dump/reader.py` & `mediawiki_dump-1.2.1/mediawiki_dump/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Class used to parse provided XML dump and emit a stream of articles content
 
 https://gist.github.com/macbre/1543d945f5244c5c68681966f07e2d6c
 """
+
 import logging
 from typing import Generator
 
 from xml import sax
 from xml.sax.xmlreader import AttributesImpl
 
 from .dumps import BaseDump
@@ -177,16 +178,15 @@
 
         self.tag_content += content
 
     def get_entries(self) -> Generator[tuple, None, None]:
         """
         Used by DumpReader to yield pages as we parse the XML dump
         """
-        for entry in self.entries_batch:
-            yield entry
+        yield from self.entries_batch
 
         self.entries_batch = []
 
     def get_entries_count(self) -> int:
         """
         :rtype: int
         """
```

### Comparing `mediawiki_dump-1.2.0/mediawiki_dump/tokenizer.py` & `mediawiki_dump-1.2.1/mediawiki_dump/tokenizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Cleans and tokenizes given text
 """
+
 import re
 from typing import Callable, List
 
 
 def clean(text: str) -> str:
     """Cleans up the provided wikitext.
     Removes templates, tables, parser hooks, magic words, HTML tags and file embeds.
```

### Comparing `mediawiki_dump-1.2.0/mediawiki_dump.egg-info/PKG-INFO` & `mediawiki_dump-1.2.1/mediawiki_dump.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 Metadata-Version: 2.1
-Name: mediawiki-dump
-Version: 1.2.0
+Name: mediawiki_dump
+Version: 1.2.1
 Summary: Python package for working with MediaWiki XML content dumps
 Home-page: https://github.com/macbre/mediawiki-dump
 Author: Maciej Brencz
 Author-email: maciej.brencz@gmail.com
 License: MIT
 Keywords: dump fandom mediawiki wikipedia wikia
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Text Processing :: Markup :: XML
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: libarchive-c==5.1
+Requires-Dist: requests>=2.26.0
+Requires-Dist: mwclient>=0.10.1
+Provides-Extra: dev
+Requires-Dist: black==24.4.0; extra == "dev"
+Requires-Dist: coveralls==3.3.1; extra == "dev"
+Requires-Dist: pylint==3.1.0; extra == "dev"
+Requires-Dist: pytest==8.1.1; extra == "dev"
+Requires-Dist: pytest-cov==5.0.0; extra == "dev"
+Requires-Dist: responses==0.25.0; extra == "dev"
 
 # mediawiki-dump
 [![PyPI](https://img.shields.io/pypi/v/mediawiki_dump.svg)](https://pypi.python.org/pypi/mediawiki_dump)
 [![Downloads](https://pepy.tech/badge/mediawiki_dump)](https://pepy.tech/project/mediawiki_dump)
 [![CI](https://github.com/macbre/mediawiki-dump/actions/workflows/tests.yml/badge.svg)](https://github.com/macbre/mediawiki-dump/actions/workflows/tests.yml)
 [![Coverage Status](https://coveralls.io/repos/github/macbre/mediawiki-dump/badge.svg?branch=master)](https://coveralls.io/github/macbre/mediawiki-dump?branch=master)
```

### Comparing `mediawiki_dump-1.2.0/setup.py` & `mediawiki_dump-1.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "1.2.0"
+VERSION = "1.2.1"
 
 # @see https://packaging.python.org/tutorials/packaging-projects/#creating-setup-py
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # @see https://github.com/pypa/sampleproject/blob/master/setup.py
 setup(
@@ -31,21 +31,21 @@
         # Pick your license as you wish
         "License :: OSI Approved :: MIT License",
     ],
     python_requires=">=3.8",
     packages=find_packages(),
     extras_require={
         "dev": [
-            "black==23.9.1",
+            "black==24.4.0",
             "coveralls==3.3.1",
-            "pylint==2.17.6",
-            "pytest==7.4.2",
-            "pytest-cov==4.1.0",
-            "responses==0.23.3",
+            "pylint==3.1.0",
+            "pytest==8.1.1",
+            "pytest-cov==5.0.0",
+            "responses==0.25.0",
         ]
     },
     install_requires=[
-        "libarchive-c==5.0",
+        "libarchive-c==5.1",
         "requests>=2.26.0",
         "mwclient>=0.10.1",
     ],
 )
```

