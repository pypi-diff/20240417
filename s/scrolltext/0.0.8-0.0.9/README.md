# Comparing `tmp/scrolltext-0.0.8.tar.gz` & `tmp/scrolltext-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrolltext-0.0.8.tar", last modified: Tue Mar 12 10:18:07 2024, max compression
+gzip compressed data, was "scrolltext-0.0.9.tar", last modified: Sat Mar 30 10:41:21 2024, max compression
```

## Comparing `scrolltext-0.0.8.tar` & `scrolltext-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2024-03-12 10:18:07.006421 scrolltext-0.0.8/
--rw-r--r--   0 jim       (1000) jim       (1000)    35149 2024-01-27 12:14:09.000000 scrolltext-0.0.8/LICENSE
--rw-r--r--   0 jim       (1000) jim       (1000)     3098 2024-03-12 10:18:07.006421 scrolltext-0.0.8/PKG-INFO
--rw-r--r--   0 jim       (1000) jim       (1000)     2167 2024-03-12 09:50:20.000000 scrolltext-0.0.8/README.md
--rw-r--r--   0 jim       (1000) jim       (1000)       81 2024-02-06 19:34:27.000000 scrolltext-0.0.8/pyproject.toml
-drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2024-03-12 10:18:07.006421 scrolltext-0.0.8/scrolltext/
--rw-r--r--   0 jim       (1000) jim       (1000)      155 2024-03-11 23:14:27.000000 scrolltext-0.0.8/scrolltext/__init__.py
--rw-r--r--   0 jim       (1000) jim       (1000)     1667 2024-03-12 09:56:26.000000 scrolltext-0.0.8/scrolltext/cli.py
--rw-r--r--   0 jim       (1000) jim       (1000)     3764 2024-03-12 08:58:33.000000 scrolltext-0.0.8/scrolltext/config.py
--rw-r--r--   0 jim       (1000) jim       (1000)     2757 2024-03-11 23:14:27.000000 scrolltext-0.0.8/scrolltext/cursestext.py
--rw-r--r--   0 jim       (1000) jim       (1000)     1237 2024-03-11 00:27:20.000000 scrolltext-0.0.8/scrolltext/getchtimeout.py
--rw-r--r--   0 jim       (1000) jim       (1000)     1997 2024-03-11 23:14:27.000000 scrolltext-0.0.8/scrolltext/linescroller.py
--rw-r--r--   0 jim       (1000) jim       (1000)     7568 2024-03-12 09:23:36.000000 scrolltext-0.0.8/scrolltext/utils.py
-drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2024-03-12 10:18:07.006421 scrolltext-0.0.8/scrolltext.egg-info/
--rw-r--r--   0 jim       (1000) jim       (1000)     3098 2024-03-12 10:18:07.000000 scrolltext-0.0.8/scrolltext.egg-info/PKG-INFO
--rw-r--r--   0 jim       (1000) jim       (1000)      376 2024-03-12 10:18:07.000000 scrolltext-0.0.8/scrolltext.egg-info/SOURCES.txt
--rw-r--r--   0 jim       (1000) jim       (1000)        1 2024-03-12 10:18:07.000000 scrolltext-0.0.8/scrolltext.egg-info/dependency_links.txt
--rw-r--r--   0 jim       (1000) jim       (1000)       51 2024-03-12 10:18:07.000000 scrolltext-0.0.8/scrolltext.egg-info/entry_points.txt
--rw-r--r--   0 jim       (1000) jim       (1000)       11 2024-03-12 10:18:07.000000 scrolltext-0.0.8/scrolltext.egg-info/top_level.txt
--rw-r--r--   0 jim       (1000) jim       (1000)     1080 2024-03-12 10:18:07.006421 scrolltext-0.0.8/setup.cfg
+drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2024-03-30 10:41:21.767710 scrolltext-0.0.9/
+-rw-r--r--   0 jim       (1000) jim       (1000)    35149 2024-01-27 12:14:09.000000 scrolltext-0.0.9/LICENSE
+-rw-r--r--   0 jim       (1000) jim       (1000)     3323 2024-03-30 10:41:21.767710 scrolltext-0.0.9/PKG-INFO
+-rw-r--r--   0 jim       (1000) jim       (1000)     2392 2024-03-30 10:38:03.000000 scrolltext-0.0.9/README.md
+-rw-r--r--   0 jim       (1000) jim       (1000)       81 2024-02-06 19:34:27.000000 scrolltext-0.0.9/pyproject.toml
+drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2024-03-30 10:41:21.767710 scrolltext-0.0.9/scrolltext/
+-rw-r--r--   0 jim       (1000) jim       (1000)      155 2024-03-11 23:14:27.000000 scrolltext-0.0.9/scrolltext/__init__.py
+-rw-r--r--   0 jim       (1000) jim       (1000)     1718 2024-03-30 00:00:40.000000 scrolltext-0.0.9/scrolltext/cli.py
+-rw-r--r--   0 jim       (1000) jim       (1000)     3277 2024-03-30 10:38:03.000000 scrolltext-0.0.9/scrolltext/config.py
+-rw-r--r--   0 jim       (1000) jim       (1000)     3873 2024-03-30 10:38:03.000000 scrolltext-0.0.9/scrolltext/cursestext.py
+-rw-r--r--   0 jim       (1000) jim       (1000)     1237 2024-03-11 00:27:20.000000 scrolltext-0.0.9/scrolltext/getchtimeout.py
+-rw-r--r--   0 jim       (1000) jim       (1000)     2707 2024-03-30 10:38:03.000000 scrolltext-0.0.9/scrolltext/linescroller.py
+-rw-r--r--   0 jim       (1000) jim       (1000)     9003 2024-03-30 10:38:03.000000 scrolltext-0.0.9/scrolltext/utils.py
+drwxr-xr-x   0 jim       (1000) jim       (1000)        0 2024-03-30 10:41:21.767710 scrolltext-0.0.9/scrolltext.egg-info/
+-rw-r--r--   0 jim       (1000) jim       (1000)     3323 2024-03-30 10:41:21.000000 scrolltext-0.0.9/scrolltext.egg-info/PKG-INFO
+-rw-r--r--   0 jim       (1000) jim       (1000)      376 2024-03-30 10:41:21.000000 scrolltext-0.0.9/scrolltext.egg-info/SOURCES.txt
+-rw-r--r--   0 jim       (1000) jim       (1000)        1 2024-03-30 10:41:21.000000 scrolltext-0.0.9/scrolltext.egg-info/dependency_links.txt
+-rw-r--r--   0 jim       (1000) jim       (1000)       51 2024-03-30 10:41:21.000000 scrolltext-0.0.9/scrolltext.egg-info/entry_points.txt
+-rw-r--r--   0 jim       (1000) jim       (1000)       11 2024-03-30 10:41:21.000000 scrolltext-0.0.9/scrolltext.egg-info/top_level.txt
+-rw-r--r--   0 jim       (1000) jim       (1000)     1080 2024-03-30 10:41:21.767710 scrolltext-0.0.9/setup.cfg
```

### Comparing `scrolltext-0.0.8/LICENSE` & `scrolltext-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scrolltext-0.0.8/PKG-INFO` & `scrolltext-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrolltext
-Version: 0.0.8
+Version: 0.0.9
 Summary: A little toy for scrolling text.
 Home-page: https://github.com/jimdeekepler/python-scrolltext
 Author: Jim Dee Kepler
 Author-email: jimdee@gmail.com
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -86,19 +86,25 @@
 Fastest scrolling speed.
 
     SCROLL_SPEED=10 scrolltext
 
 
 ## Bugs and quirks
 
- - does not detect term-resize
+ - attempts to detect term-resize, and clumsily adjusts some things
  - no colors
 
 
 ## Changes
 
+### v0.0.9
+
+ - attempt to handle term resizes
+ - added config-option: endless  (see newly generated config-file)
+ - removed logging from main branch (you may find it on the devel branch)
+
 ### v0.0.8
 
  - doc-comments have never been generated, nor are those validated. (TODO)
  - renamed log-file to "scrolltext.log"
  - uses config file "scrolltextrc"
    \*NIX uses "~/.config/scrolltextrc", windows uses "scrolltextrc" in current directory
```

### Comparing `scrolltext-0.0.8/README.md` & `scrolltext-0.0.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -61,19 +61,25 @@
 Fastest scrolling speed.
 
     SCROLL_SPEED=10 scrolltext
 
 
 ## Bugs and quirks
 
- - does not detect term-resize
+ - attempts to detect term-resize, and clumsily adjusts some things
  - no colors
 
 
 ## Changes
 
+### v0.0.9
+
+ - attempt to handle term resizes
+ - added config-option: endless  (see newly generated config-file)
+ - removed logging from main branch (you may find it on the devel branch)
+
 ### v0.0.8
 
  - doc-comments have never been generated, nor are those validated. (TODO)
  - renamed log-file to "scrolltext.log"
  - uses config file "scrolltextrc"
    \*NIX uses "~/.config/scrolltextrc", windows uses "scrolltextrc" in current directory
```

### Comparing `scrolltext-0.0.8/scrolltext/cli.py` & `scrolltext-0.0.9/scrolltext/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,18 +22,19 @@
     """
     Main method.
     """
     write_config, action = _parse_args()
     try:
         cfg = init_utils(write_config)
         action = action or _str_to_action_type(cfg["main"]["action"])
-        action(write_config)
+        action(cfg)
+    except KeyError as e:
+        print("KeyError occured: " + str(e) + "\nProbalby check config?")
     except NameError as e:
         print("NameError occured: " + str(e))
-        print("Probalby check config?")
 
 
 def _parse_args():  # pylint: disable=inconsistent-return-statements  (R1710)
     write_config = False
     action = None
     for arg in sys.argv[1:]:
         if _check_help_or_version(arg):
```

### Comparing `scrolltext-0.0.8/scrolltext/config.py` & `scrolltext-0.0.9/scrolltext/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 """
 Config module for scrolltext
 """
 from pathlib import Path
 import configparser
-import logging
 import sys
 
 
 IS_WINDOWS = sys.platform in ["msys", "win32", "nt"]
 DEF_SCROLL_TEXT = """\
 Hello, this is a  classic side scrolling text. You can override it by setting the \
 environment variable 'SCROLL_TEXT'. It is supposed to be a simple example."""
 SCROLL_SPEEDS = [.25, .20, .18, .15, .125, .1, .09, .08, .075, .07, .0675]
 
 
-log = logging.getLogger(__name__)
-
-
 initial_config = {
-    "main": {"action": "linescroller"},
+    "main": {"action": "linescroller", "endless": "0"},
     "cursestext": {"box": "1"},
     "scrolltext.text 1": {
         "direction": "0",
         "text": DEF_SCROLL_TEXT,
         "line": "0",
         "speed": "0",
     }
@@ -51,34 +47,29 @@
     if not IS_WINDOWS:
         config_path = Path("~/.config/scrolltextrc").expanduser()
     else:
         config_path = Path("scrolltextrc")
 
     cfg, really_write = _read_config(config_path)
     if write_config and really_write:
-        log.info("Writing a new config '%s' using defaults", config_path)
         _write_config(cfg, config_path)
     return cfg
 
 
 def _read_config(config_path):
     """
     Reads the config file and returns an object.
     """
     really_write = False
     cfg = configparser.ConfigParser(default_section="main")
-    log.debug("try read config path: '%s'", config_path)
     read_config_files = cfg.read(config_path)
 
     if not read_config_files:
         really_write = True
-        log.info("No config file found")
         cfg.update(initial_config)
-    else:
-        log.debug("config read: '%s'", read_config_files)
     _validate(cfg)
     return cfg, really_write
 
 
 def _write_config(cfg, config_path):
     with open(config_path, "w", encoding="utf-8") as newfile:
         cfg.write(newfile)
@@ -91,27 +82,23 @@
     for section, entries in initial_config.items():
         if "%d" in section:
             section = section.replace("%d", "1")
         if section not in cfg:
             raise NameError("Section '" + section + "' is missing in config")
         _validate_section_entries(cfg, section, entries)
 
-    log.debug(cfg["main"]["action"])
-
     # NOTE: allow for several "scrolltext.text %d" sections
     # for index in range(2, 9):
     #     scrolltext_section = "scrolltext.text " + str(index)
     #     if not scrolltext_section in cfg:
     #         cfg["main"]["max_index"] = str(index - 1)
-    #         log.debug("max scrolltext.text %d", cfg["main"]["max_index"])
     #         break
     _fix_scrolltext_section(cfg, "scrolltext.text 1")
     if "cursestext" not in cfg:
         cfg["cursestext"] = {"box": "1"}
-    log.debug("cursestext draw box: %s", cfg["cursestext"].getboolean("box"))
 
 
 def _validate_section_entries(cfg, section, entries):
     for entry in entries:
         if entry not in cfg[section]:
             raise NameError("Entry '" + entry + "' is missing in Section '"
                             + section + "'")
@@ -120,8 +107,7 @@
 def _fix_scrolltext_section(cfg, section_name):
     """
     Helper function for joining lines in text to one line.
     """
     text_lines = cfg[section_name]["text"]
     text = "".join(text_lines.split("\n"))
     cfg[section_name]["text"] = text
-    log.debug(text)
```

### Comparing `scrolltext-0.0.8/scrolltext/getchtimeout.py` & `scrolltext-0.0.9/scrolltext/getchtimeout.py`

 * *Files identical despite different names*

### Comparing `scrolltext-0.0.8/scrolltext/linescroller.py` & `scrolltext-0.0.9/scrolltext/linescroller.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,122 +4,167 @@
 00000030: 220a 696d 706f 7274 2073 6875 7469 6c0a  ".import shutil.
 00000040: 6672 6f6d 2074 696d 6520 696d 706f 7274  from time import
 00000050: 2073 6c65 6570 0a66 726f 6d20 2e75 7469   sleep.from .uti
 00000060: 6c73 2069 6d70 6f72 7420 434c 4541 522c  ls import CLEAR,
 00000070: 2048 4f4d 452c 2049 535f 5749 4e44 4f57   HOME, IS_WINDOW
 00000080: 532c 2055 505f 4f4e 455f 524f 572c 2043  S, UP_ONE_ROW, C
 00000090: 6861 7261 6374 6572 5363 726f 6c6c 6572  haracterScroller
-000000a0: 2c20 696e 6974 5f75 7469 6c73 0a0a 6966  , init_utils..if
-000000b0: 206e 6f74 2049 535f 5749 4e44 4f57 533a   not IS_WINDOWS:
-000000c0: 0a20 2020 2066 726f 6d20 7363 726f 6c6c  .    from scroll
-000000d0: 7465 7874 2e67 6574 6368 7469 6d65 6f75  text.getchtimeou
-000000e0: 7420 696d 706f 7274 2047 6574 6368 5769  t import GetchWi
-000000f0: 7468 5469 6d65 6f75 740a 0a0a 5649 5349  thTimeout...VISI
-00000100: 4249 4c45 5f54 4558 545f 4c45 4e47 5448  BILE_TEXT_LENGTH
-00000110: 203d 2073 6875 7469 6c2e 6765 745f 7465   = shutil.get_te
-00000120: 726d 696e 616c 5f73 697a 6528 295b 305d  rminal_size()[0]
-00000130: 0a0a 0a64 6566 206c 696e 6573 6372 6f6c  ...def linescrol
-00000140: 6c65 7228 7772 6974 655f 636f 6e66 6967  ler(write_config
-00000150: 293a 0a20 2020 2022 2222 0a20 2020 204d  ):.    """.    M
-00000160: 6169 6e20 656e 7472 7920 706f 696e 7420  ain entry point 
-00000170: 666f 7220 6c69 6e65 7363 726f 6c6c 6572  for linescroller
-00000180: 2e0a 2020 2020 3a70 6172 616d 2077 7269  ..    :param wri
-00000190: 7465 5f63 6f6e 6669 673a 2057 7269 7465  te_config: Write
-000001a0: 2069 6e69 7469 616c 2063 6f6e 6669 670a   initial config.
-000001b0: 2020 2020 3a74 7970 653a 2062 6f6f 6c0a      :type: bool.
-000001c0: 2020 2020 2222 220a 2020 2020 6765 7463      """.    getc
-000001d0: 6820 3d20 4e6f 6e65 0a20 2020 2069 6620  h = None.    if 
-000001e0: 6e6f 7420 4953 5f57 494e 444f 5753 3a0a  not IS_WINDOWS:.
-000001f0: 2020 2020 2020 2020 6765 7463 6820 3d20          getch = 
-00000200: 4765 7463 6857 6974 6854 696d 656f 7574  GetchWithTimeout
-00000210: 2829 0a20 2020 2074 7279 3a0a 2020 2020  ().    try:.    
-00000220: 2020 2020 5f6c 696e 6573 6372 6f6c 6c65      _linescrolle
-00000230: 7228 6765 7463 682c 2077 7269 7465 5f63  r(getch, write_c
-00000240: 6f6e 6669 6729 0a20 2020 2065 7863 6570  onfig).    excep
-00000250: 7420 5275 6e74 696d 6545 7272 6f72 3a0a  t RuntimeError:.
-00000260: 2020 2020 2020 2020 7061 7373 0a20 2020          pass.   
-00000270: 2066 696e 616c 6c79 3a0a 2020 2020 2020   finally:.      
-00000280: 2020 6966 206e 6f74 2049 535f 5749 4e44    if not IS_WIND
-00000290: 4f57 533a 0a20 2020 2020 2020 2020 2020  OWS:.           
-000002a0: 2067 6574 6368 2e63 6c65 616e 7570 2829   getch.cleanup()
-000002b0: 0a0a 0a64 6566 205f 6c69 6e65 7363 726f  ...def _linescro
-000002c0: 6c6c 6572 2867 6574 6368 2c20 7772 6974  ller(getch, writ
-000002d0: 655f 636f 6e66 6967 293a 0a20 2020 2022  e_config):.    "
-000002e0: 2222 0a20 2020 2050 7269 6e74 7320 6120  "".    Prints a 
-000002f0: 7465 7874 2069 6e20 6120 7369 6465 2d73  text in a side-s
-00000300: 6372 6f6c 6c69 6e67 206d 616e 6e65 722e  crolling manner.
-00000310: 0a20 2020 2022 2222 0a20 2020 2063 6667  .    """.    cfg
-00000320: 203d 2069 6e69 745f 7574 696c 7328 7772   = init_utils(wr
-00000330: 6974 655f 636f 6e66 6967 290a 2020 2020  ite_config).    
-00000340: 6172 6776 203d 207b 7d0a 2020 2020 6172  argv = {}.    ar
-00000350: 6776 5b22 7465 726d 5f72 6f77 7322 5d20  gv["term_rows"] 
-00000360: 3d20 7368 7574 696c 2e67 6574 5f74 6572  = shutil.get_ter
-00000370: 6d69 6e61 6c5f 7369 7a65 2829 5b31 5d0a  minal_size()[1].
-00000380: 2020 2020 6172 6776 5b22 7465 726d 5f63      argv["term_c
-00000390: 6f6c 756d 6e73 225d 203d 2073 6875 7469  olumns"] = shuti
-000003a0: 6c2e 6765 745f 7465 726d 696e 616c 5f73  l.get_terminal_s
-000003b0: 697a 6528 295b 305d 0a20 2020 2061 7267  ize()[0].    arg
-000003c0: 765b 226d 696e 5f73 6372 6f6c 6c5f 6c69  v["min_scroll_li
-000003d0: 6e65 225d 203d 2030 0a20 2020 2073 6372  ne"] = 0.    scr
-000003e0: 6f6c 6c65 7220 3d20 4368 6172 6163 7465  oller = Characte
-000003f0: 7253 6372 6f6c 6c65 7228 6366 672c 202a  rScroller(cfg, *
-00000400: 2a61 7267 7629 0a0a 2020 2020 7072 696e  *argv)..    prin
-00000410: 7428 6622 7b43 4c45 4152 7d7b 484f 4d45  t(f"{CLEAR}{HOME
-00000420: 7d22 2c20 656e 643d 2222 290a 2020 2020  }", end="").    
-00000430: 6966 2073 6372 6f6c 6c65 722e 6c69 6e65  if scroller.line
-00000440: 203e 2030 3a0a 2020 2020 2020 2020 5f6d   > 0:.        _m
-00000450: 6f76 655f 746f 5f6c 696e 6528 7363 726f  ove_to_line(scro
-00000460: 6c6c 6572 2e6c 696e 6529 0a20 2020 2066  ller.line).    f
-00000470: 6f72 2074 6578 7420 696e 2073 6372 6f6c  or text in scrol
-00000480: 6c65 723a 0a20 2020 2020 2020 2077 696e  ler:.        win
-00000490: 5f74 6578 7420 3d20 7465 7874 0a20 2020  _text = text.   
-000004a0: 2020 2020 2070 7269 6e74 2877 696e 5f74       print(win_t
-000004b0: 6578 742c 2065 6e64 3d22 5c72 2229 0a20  ext, end="\r"). 
-000004c0: 2020 2020 2020 2069 6620 4953 5f57 494e         if IS_WIN
-000004d0: 444f 5753 3a0a 2020 2020 2020 2020 2020  DOWS:.          
-000004e0: 2020 736c 6565 7028 2e31 3529 0a20 2020    sleep(.15).   
-000004f0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00000500: 2020 2020 2020 205f 6368 6563 6b5f 696e         _check_in
-00000510: 7075 7428 6765 7463 6829 0a20 2020 2069  put(getch).    i
-00000520: 6620 4953 5f57 494e 444f 5753 3a0a 2020  f IS_WINDOWS:.  
-00000530: 2020 2020 2020 7072 696e 7428 6622 7b55        print(f"{U
-00000540: 505f 4f4e 455f 524f 577d 222c 2065 6e64  P_ONE_ROW}", end
-00000550: 3d22 2229 0a0a 0a64 6566 205f 6368 6563  ="")...def _chec
-00000560: 6b5f 696e 7075 7428 6765 7463 6829 3a0a  k_input(getch):.
-00000570: 2020 2020 2222 220a 2020 2020 5573 6520      """.    Use 
-00000580: 6765 7463 6874 696d 656f 7574 2074 6f20  getchtimeout to 
-00000590: 6765 7420 6120 6368 6172 6163 7465 722e  get a character.
-000005a0: 2049 6620 2251 2220 6f72 2022 7122 2069   If "Q" or "q" i
-000005b0: 7320 6769 7665 6e2c 2074 6865 6e20 6974  s given, then it
-000005c0: 2072 6169 7365 7320 5379 7374 656d 4578   raises SystemEx
-000005d0: 6974 0a20 2020 2022 2222 0a20 2020 2063  it.    """.    c
-000005e0: 6861 7261 6374 6572 203d 2067 6574 6368  haracter = getch
-000005f0: 2e67 6574 6368 2874 696d 656f 7574 3d2e  .getch(timeout=.
-00000600: 3129 0a20 2020 2069 6620 6368 6172 6163  1).    if charac
-00000610: 7465 7220 6973 206e 6f74 204e 6f6e 6520  ter is not None 
-00000620: 616e 6420 6368 6172 6163 7465 7220 696e  and character in
-00000630: 205b 225c 3033 3322 2c20 225c 7831 6222   ["\033", "\x1b"
-00000640: 2c20 2203 222c 2022 5c72 222c 2022 1122  , ".", "\r", "."
-00000650: 2c20 2220 222c 2022 5122 2c20 2271 225d  , " ", "Q", "q"]
-00000660: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
-00000670: 5275 6e74 696d 6545 7272 6f72 2829 0a0a  RuntimeError()..
-00000680: 0a64 6566 205f 6d6f 7665 5f74 6f5f 6c69  .def _move_to_li
-00000690: 6e65 286c 696e 6529 3a0a 2020 2020 2222  ne(line):.    ""
-000006a0: 220a 2020 2020 4d6f 7665 2074 6865 2063  ".    Move the c
-000006b0: 7572 736f 7220 746f 2074 6865 2073 7065  ursor to the spe
-000006c0: 6369 6669 6564 206c 696e 652e 2054 6869  cified line. Thi
-000006d0: 7320 6973 2064 6f6e 6520 7573 696e 6720  s is done using 
-000006e0: 414e 5349 2045 7363 6170 6520 7365 7175  ANSI Escape sequ
-000006f0: 656e 6365 732e 0a20 2020 203a 7061 7261  ences..    :para
-00000700: 6d20 6c69 6e65 3a20 5468 6520 6c69 6e65  m line: The line
-00000710: 206e 756d 6265 7220 746f 2073 6372 6f6c   number to scrol
-00000720: 6c20 746f 2e0a 2020 2020 3a74 7970 6520  l to..    :type 
-00000730: 6c69 6e65 3a20 696e 740a 2020 2020 2222  line: int.    ""
-00000740: 220a 2020 2020 6966 206e 6f74 2049 535f  ".    if not IS_
-00000750: 5749 4e44 4f57 533a 0a20 2020 2020 2020  WINDOWS:.       
-00000760: 2070 7269 6e74 2866 225c 3033 335b 7b6c   print(f"\033[{l
-00000770: 696e 657d 4222 2c20 656e 643d 2222 290a  ine}B", end="").
-00000780: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00000790: 2020 666f 7220 5f20 696e 2072 616e 6765    for _ in range
-000007a0: 286c 696e 6529 3a0a 2020 2020 2020 2020  (line):.        
-000007b0: 2020 2020 7072 696e 7428 225c 3033 335b      print("\033[
-000007c0: 3142 222c 2065 6e64 3d22 2229 0a         1B", end="").
+000000a0: 2c20 5465 726d 5369 7a65 0a0a 6966 206e  , TermSize..if n
+000000b0: 6f74 2049 535f 5749 4e44 4f57 533a 0a20  ot IS_WINDOWS:. 
+000000c0: 2020 2066 726f 6d20 7363 726f 6c6c 7465     from scrollte
+000000d0: 7874 2e67 6574 6368 7469 6d65 6f75 7420  xt.getchtimeout 
+000000e0: 696d 706f 7274 2047 6574 6368 5769 7468  import GetchWith
+000000f0: 5469 6d65 6f75 740a 0a0a 6c61 7374 5f74  Timeout...last_t
+00000100: 6572 6d5f 726f 7773 203d 202d 3120 2023  erm_rows = -1  #
+00000110: 2070 796c 696e 743a 2064 6973 6162 6c65   pylint: disable
+00000120: 3d43 3031 3033 2028 696e 7661 6c69 642d  =C0103 (invalid-
+00000130: 6e61 6d65 290a 0a0a 6465 6620 6c69 6e65  name)...def line
+00000140: 7363 726f 6c6c 6572 2863 6667 293a 0a20  scroller(cfg):. 
+00000150: 2020 2022 2222 0a20 2020 204d 6169 6e20     """.    Main 
+00000160: 656e 7472 7920 706f 696e 7420 666f 7220  entry point for 
+00000170: 6c69 6e65 7363 726f 6c6c 6572 2e0a 2020  linescroller..  
+00000180: 2020 3a70 6172 616d 2063 6667 3a20 436f    :param cfg: Co
+00000190: 6e66 6967 206f 626a 6563 740a 2020 2020  nfig object.    
+000001a0: 3a74 7970 653a 2063 6f6e 6669 6770 6172  :type: configpar
+000001b0: 7365 722e 436f 6e66 6967 5061 7273 6572  ser.ConfigParser
+000001c0: 0a20 2020 2022 2222 0a20 2020 2067 6574  .    """.    get
+000001d0: 6368 203d 204e 6f6e 650a 2020 2020 6966  ch = None.    if
+000001e0: 206e 6f74 2049 535f 5749 4e44 4f57 533a   not IS_WINDOWS:
+000001f0: 0a20 2020 2020 2020 2067 6574 6368 203d  .        getch =
+00000200: 2047 6574 6368 5769 7468 5469 6d65 6f75   GetchWithTimeou
+00000210: 7428 290a 2020 2020 7472 793a 0a20 2020  t().    try:.   
+00000220: 2020 2020 205f 6c69 6e65 7363 726f 6c6c       _linescroll
+00000230: 6572 2867 6574 6368 2c20 6366 6729 0a20  er(getch, cfg). 
+00000240: 2020 2065 7863 6570 7420 5275 6e74 696d     except Runtim
+00000250: 6545 7272 6f72 3a0a 2020 2020 2020 2020  eError:.        
+00000260: 7061 7373 0a20 2020 2066 696e 616c 6c79  pass.    finally
+00000270: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
+00000280: 2049 535f 5749 4e44 4f57 533a 0a20 2020   IS_WINDOWS:.   
+00000290: 2020 2020 2020 2020 2067 6574 6368 2e63           getch.c
+000002a0: 6c65 616e 7570 2829 0a0a 0a64 6566 205f  leanup()...def _
+000002b0: 6c69 6e65 7363 726f 6c6c 6572 2867 6574  linescroller(get
+000002c0: 6368 2c20 6366 6729 3a0a 2020 2020 2222  ch, cfg):.    ""
+000002d0: 220a 2020 2020 5072 696e 7473 2061 2074  ".    Prints a t
+000002e0: 6578 7420 696e 2061 2073 6964 652d 7363  ext in a side-sc
+000002f0: 726f 6c6c 696e 6720 6d61 6e6e 6572 2e0a  rolling manner..
+00000300: 2020 2020 2222 220a 2020 2020 7465 726d      """.    term
+00000310: 5f73 697a 6520 3d20 5465 726d 5369 7a65  _size = TermSize
+00000320: 2830 2c20 3029 0a20 2020 205f 7570 6461  (0, 0).    _upda
+00000330: 7465 5f74 6572 6d5f 7369 7a65 2874 6572  te_term_size(ter
+00000340: 6d5f 7369 7a65 290a 2020 2020 6172 6776  m_size).    argv
+00000350: 203d 207b 7d0a 2020 2020 6172 6776 5b22   = {}.    argv["
+00000360: 6d69 6e5f 7363 726f 6c6c 5f6c 696e 6522  min_scroll_line"
+00000370: 5d20 3d20 300a 2020 2020 7363 726f 6c6c  ] = 0.    scroll
+00000380: 6572 203d 2043 6861 7261 6374 6572 5363  er = CharacterSc
+00000390: 726f 6c6c 6572 2863 6667 2c20 7465 726d  roller(cfg, term
+000003a0: 5f73 697a 652c 202a 2a61 7267 7629 0a0a  _size, **argv)..
+000003b0: 2020 2020 7072 696e 7428 6622 7b43 4c45      print(f"{CLE
+000003c0: 4152 7d7b 484f 4d45 7d22 2c20 656e 643d  AR}{HOME}", end=
+000003d0: 2222 290a 2020 2020 6966 2073 6372 6f6c  "").    if scrol
+000003e0: 6c65 722e 6c69 6e65 203e 2030 3a0a 2020  ler.line > 0:.  
+000003f0: 2020 2020 2020 5f6d 6f76 655f 746f 5f6c        _move_to_l
+00000400: 696e 6528 7363 726f 6c6c 6572 2e6c 696e  ine(scroller.lin
+00000410: 6529 0a20 2020 2063 6e74 203d 2030 0a20  e).    cnt = 0. 
+00000420: 2020 2066 6f72 2074 6578 7420 696e 2073     for text in s
+00000430: 6372 6f6c 6c65 723a 0a20 2020 2020 2020  croller:.       
+00000440: 2069 6620 7363 726f 6c6c 6572 2e6c 696e   if scroller.lin
+00000450: 6520 3c20 7465 726d 5f73 697a 652e 6765  e < term_size.ge
+00000460: 745f 726f 7773 2829 202d 2031 3a0a 2020  t_rows() - 1:.  
+00000470: 2020 2020 2020 2020 2020 7769 6e5f 7465            win_te
+00000480: 7874 203d 2074 6578 740a 2020 2020 2020  xt = text.      
+00000490: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000004a0: 2020 2020 7769 6e5f 7465 7874 203d 2074      win_text = t
+000004b0: 6578 745b 3a2d 315d 0a20 2020 2020 2020  ext[:-1].       
+000004c0: 2070 7269 6e74 2877 696e 5f74 6578 742c   print(win_text,
+000004d0: 2065 6e64 3d22 5c72 2229 0a20 2020 2020   end="\r").     
+000004e0: 2020 2069 6620 4953 5f57 494e 444f 5753     if IS_WINDOWS
+000004f0: 3a0a 2020 2020 2020 2020 2020 2020 736c  :.            sl
+00000500: 6565 7028 2e31 3529 0a20 2020 2020 2020  eep(.15).       
+00000510: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00000520: 2020 205f 6368 6563 6b5f 696e 7075 7428     _check_input(
+00000530: 6765 7463 6829 0a20 2020 2020 2020 2063  getch).        c
+00000540: 6e74 202b 3d20 310a 2020 2020 2020 2020  nt += 1.        
+00000550: 6966 205f 7570 6461 7465 5f74 6572 6d5f  if _update_term_
+00000560: 7369 7a65 2874 6572 6d5f 7369 7a65 293a  size(term_size):
+00000570: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00000580: 6e74 2866 227b 434c 4541 527d 7b48 4f4d  nt(f"{CLEAR}{HOM
+00000590: 457d 222c 2065 6e64 3d22 2229 0a20 2020  E}", end="").   
+000005a0: 2020 2020 2020 2020 2069 6620 7363 726f           if scro
+000005b0: 6c6c 6572 2e6c 696e 6520 3e20 303a 0a20  ller.line > 0:. 
+000005c0: 2020 2020 2020 2020 2020 2020 2020 205f                 _
+000005d0: 6d6f 7665 5f74 6f5f 6c69 6e65 2873 6372  move_to_line(scr
+000005e0: 6f6c 6c65 722e 6c69 6e65 290a 2020 2020  oller.line).    
+000005f0: 6966 2049 535f 5749 4e44 4f57 533a 0a20  if IS_WINDOWS:. 
+00000600: 2020 2020 2020 2070 7269 6e74 2866 227b         print(f"{
+00000610: 5550 5f4f 4e45 5f52 4f57 7d22 2c20 656e  UP_ONE_ROW}", en
+00000620: 643d 2222 290a 0a0a 6465 6620 5f63 6865  d="")...def _che
+00000630: 636b 5f69 6e70 7574 2867 6574 6368 293a  ck_input(getch):
+00000640: 0a20 2020 2022 2222 0a20 2020 2055 7365  .    """.    Use
+00000650: 2067 6574 6368 7469 6d65 6f75 7420 746f   getchtimeout to
+00000660: 2067 6574 2061 2063 6861 7261 6374 6572   get a character
+00000670: 2e20 4966 2022 5122 206f 7220 2271 2220  . If "Q" or "q" 
+00000680: 6973 2067 6976 656e 2c20 7468 656e 2069  is given, then i
+00000690: 7420 7261 6973 6573 2053 7973 7465 6d45  t raises SystemE
+000006a0: 7869 740a 2020 2020 2222 220a 2020 2020  xit.    """.    
+000006b0: 6368 6172 6163 7465 7220 3d20 6765 7463  character = getc
+000006c0: 682e 6765 7463 6828 7469 6d65 6f75 743d  h.getch(timeout=
+000006d0: 2e31 290a 2020 2020 6966 2063 6861 7261  .1).    if chara
+000006e0: 6374 6572 2069 7320 6e6f 7420 4e6f 6e65  cter is not None
+000006f0: 2061 6e64 2063 6861 7261 6374 6572 2069   and character i
+00000700: 6e20 5b22 5c30 3333 222c 2022 5c78 3162  n ["\033", "\x1b
+00000710: 222c 2022 0322 2c20 225c 7222 2c20 2211  ", ".", "\r", ".
+00000720: 222c 2022 2022 2c20 2251 222c 2022 7122  ", " ", "Q", "q"
+00000730: 5d3a 0a20 2020 2020 2020 2072 6169 7365  ]:.        raise
+00000740: 2052 756e 7469 6d65 4572 726f 7228 290a   RuntimeError().
+00000750: 0a0a 6465 6620 5f6d 6f76 655f 746f 5f6c  ..def _move_to_l
+00000760: 696e 6528 6c69 6e65 293a 0a20 2020 2022  ine(line):.    "
+00000770: 2222 0a20 2020 204d 6f76 6520 7468 6520  "".    Move the 
+00000780: 6375 7273 6f72 2074 6f20 7468 6520 7370  cursor to the sp
+00000790: 6563 6966 6965 6420 6c69 6e65 2e20 5468  ecified line. Th
+000007a0: 6973 2069 7320 646f 6e65 2075 7369 6e67  is is done using
+000007b0: 2041 4e53 4920 4573 6361 7065 2073 6571   ANSI Escape seq
+000007c0: 7565 6e63 6573 2e0a 2020 2020 3a70 6172  uences..    :par
+000007d0: 616d 206c 696e 653a 2054 6865 206c 696e  am line: The lin
+000007e0: 6520 6e75 6d62 6572 2074 6f20 7363 726f  e number to scro
+000007f0: 6c6c 2074 6f2e 0a20 2020 203a 7479 7065  ll to..    :type
+00000800: 206c 696e 653a 2069 6e74 0a20 2020 2022   line: int.    "
+00000810: 2222 0a20 2020 2069 6620 6e6f 7420 4953  "".    if not IS
+00000820: 5f57 494e 444f 5753 3a0a 2020 2020 2020  _WINDOWS:.      
+00000830: 2020 7072 696e 7428 6622 5c30 3333 5b7b    print(f"\033[{
+00000840: 6c69 6e65 7d42 222c 2065 6e64 3d22 2229  line}B", end="")
+00000850: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00000860: 2020 2066 6f72 205f 2069 6e20 7261 6e67     for _ in rang
+00000870: 6528 6c69 6e65 293a 0a20 2020 2020 2020  e(line):.       
+00000880: 2020 2020 2070 7269 6e74 2822 5c30 3333       print("\033
+00000890: 5b31 4222 2c20 656e 643d 2222 290a 0a0a  [1B", end="")...
+000008a0: 6465 6620 5f75 7064 6174 655f 7465 726d  def _update_term
+000008b0: 5f73 697a 6528 7465 726d 5f73 697a 6529  _size(term_size)
+000008c0: 3a0a 2020 2020 676c 6f62 616c 206c 6173  :.    global las
+000008d0: 745f 7465 726d 5f72 6f77 7320 2023 2070  t_term_rows  # p
+000008e0: 796c 696e 743a 2064 6973 6162 6c65 3d57  ylint: disable=W
+000008f0: 3036 3033 2028 676c 6f62 616c 2d73 7461  0603 (global-sta
+00000900: 7465 6d65 6e74 290a 2020 2020 6176 6169  tement).    avai
+00000910: 6c61 626c 655f 726f 7773 203d 2073 6875  lable_rows = shu
+00000920: 7469 6c2e 6765 745f 7465 726d 696e 616c  til.get_terminal
+00000930: 5f73 697a 6528 295b 315d 0a20 2020 2061  _size()[1].    a
+00000940: 7661 696c 6162 6c65 5f63 6f6c 756d 6e73  vailable_columns
+00000950: 203d 2073 6875 7469 6c2e 6765 745f 7465   = shutil.get_te
+00000960: 726d 696e 616c 5f73 697a 6528 295b 305d  rminal_size()[0]
+00000970: 202d 2028 3120 6966 2049 535f 5749 4e44   - (1 if IS_WIND
+00000980: 4f57 5320 656c 7365 2030 290a 2020 2020  OWS else 0).    
+00000990: 7465 726d 5f73 697a 652e 7365 745f 7369  term_size.set_si
+000009a0: 7a65 2861 7661 696c 6162 6c65 5f63 6f6c  ze(available_col
+000009b0: 756d 6e73 2c20 6176 6169 6c61 626c 655f  umns, available_
+000009c0: 726f 7773 290a 2020 2020 6966 206c 6173  rows).    if las
+000009d0: 745f 7465 726d 5f72 6f77 7320 3d3d 202d  t_term_rows == -
+000009e0: 313a 0a20 2020 2020 2020 206c 6173 745f  1:.        last_
+000009f0: 7465 726d 5f72 6f77 7320 3d20 7465 726d  term_rows = term
+00000a00: 5f73 697a 652e 6765 745f 726f 7773 2829  _size.get_rows()
+00000a10: 0a20 2020 2069 6620 7465 726d 5f73 697a  .    if term_siz
+00000a20: 652e 6765 745f 726f 7773 2829 2021 3d20  e.get_rows() != 
+00000a30: 6c61 7374 5f74 6572 6d5f 726f 7773 3a0a  last_term_rows:.
+00000a40: 2020 2020 2020 2020 6c61 7374 5f74 6572          last_ter
+00000a50: 6d5f 726f 7773 203d 2074 6572 6d5f 7369  m_rows = term_si
+00000a60: 7a65 2e67 6574 5f72 6f77 7328 290a 2020  ze.get_rows().  
+00000a70: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+00000a80: 650a 2020 2020 7265 7475 726e 2046 616c  e.    return Fal
+00000a90: 7365 0a                                  se.
```

### Comparing `scrolltext-0.0.8/scrolltext/utils.py` & `scrolltext-0.0.9/scrolltext/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 """
 Utilities for line-based text scrollers.
 """
-import logging
 from os import getenv
 from time import time
 from scrolltext.config import get_speedsec_float, init_config
 from scrolltext.config import IS_WINDOWS  # pylint: disable=no-name-in-module (W0611)
 
 
 CLEAR = "\033[2J"
 HOME = "\033[H"
 UP_ONE_ROW = "\033[1A"
 
 
-log = logging.getLogger(__name__)
-
-
 def parse_int(var):
     """
     Calls int on var, ignores TypeError and ValueError.
 
     :returns: Integer value given in var string, 0 if one of the forementioned errors occurs.
     :rtype: int
     """
@@ -36,15 +32,14 @@
     Initialises config object and updates some configs via environment varialbes, if
     set.
     :param write_config: Write initial config
     :type: bool
     """
     cfg = init_config(write_config)
     _override_from_env(cfg)
-    _init_logging(cfg)
     return cfg
 
 
 def get_linenum(scroll_line_str, min_row, max_row):
     """
     :param scroll_line_str: Terminal line number for one scrolling text
     :type scroll_line_str: str
@@ -62,140 +57,186 @@
     if line < 0:
         line = max_row + line + 1
     line = max(line, min_row)
     line = min(line, max_row)
     return line
 
 
-def _init_logging(cfg):
-    verbose = cfg["main"].getboolean("verbose")
-    if verbose:
-        # logging.basicConfig(filename="cursesscroller.log", filemode="w", level=logging.DEBUG)
-        logging.basicConfig(filename="scrolltext.log", filemode="w", level=logging.DEBUG)
-
-
 def _override_from_env(cfg):
     _override_verbose(cfg)  # x x x  todo: recap (all of those ...)
+    _override_scroll_box(cfg)
     _override_scroll_direction(cfg)
     _override_scroll_text(cfg)
     _override_scroll_line(cfg)
     _override_scroll_speed(cfg)
 
 
 def _override_verbose(cfg):
     verbose = getenv("VERBOSE") == "1"
     if verbose:
-        log.debug("Using env-var 'VERBOSE'")
         cfg["main"]["verbose"] = "1"
 
 
+def _override_scroll_box(cfg):
+    scroll_direction = getenv("SCROLL_BOX") == "1"
+    if scroll_direction:
+        cfg["cursestext"]["box"] = "1"
+
+
 def _override_scroll_direction(cfg):
     scroll_direction = getenv("SCROLL_DIRECTION") == "1"
     if scroll_direction:
-        log.debug("Using env-var 'SCROLL_DIRECTION'")
         cfg["scrolltext.text 1"]["direction"] = "1"
 
 
 def _override_scroll_text(cfg):
     scroll_text = getenv("SCROLL_TEXT")
     if scroll_text:
-        log.debug("Using env-var 'SCROLL_TEXT'")
         cfg["scrolltext.text 1"]["text"] = scroll_text
 
 
 def _override_scroll_line(cfg):
     scroll_line_str = getenv("SCROLL_LINE")
     if scroll_line_str:
-        log.debug("Using env-var 'SCROLL_LINE_STR'")
         cfg["scrolltext.text 1"]["line"] = scroll_line_str
 
 
 def _override_scroll_speed(cfg):
     scroll_speed = getenv("SCROLL_SPEED")
     if scroll_speed:
         scroll_speed_index = parse_int(getenv("SCROLL_SPEED"))
-        log.debug("Using env-var 'SCROLL_SPEED' with '%s'", scroll_speed)
         cfg["scrolltext.text 1"]["speed"] = str(scroll_speed_index)
 
 
+class TermSize:
+    """
+    Stores terminal columns and rows
+    """
+    def __init__(self, cols, rows):
+        """
+        Initializes current terminal size
+        :param cols: Current terminal columns
+        :ptype cols: int
+        :param rows: Current terminal rows
+        :ptype rows: int
+        """
+        self.term_columns = cols
+        self.term_rows = rows
+        self.resized = False
+
+    def set_size(self, cols, rows):
+        """
+        Checks if the terminal window size has changed, and sets the
+        new term columns and rows paramters. Also sets the resized flag.
+        """
+        if self.term_columns != cols:
+            self.term_columns = cols
+            self.resized = True
+        if self.term_rows != rows:
+            self.term_rows = rows
+            self.resized = True
+
+    def is_resized(self):
+        """
+        Returns true, when the terminal window changed its size.
+        """
+        resized = self.resized
+        self.resized = False
+        return resized
+
+    def get_cols(self):
+        """ Return terminal columns. """
+        return self.term_columns
+
+    def get_rows(self):
+        """ Return terminal rows. """
+        return self.term_rows
+
+
 class CharacterScroller:  # pylint: disable=R0902  # disable (too-many-instance-attributes)
     """
     Utility class  for all character based text-scrollers.
     """
 
-    def __init__(self, cfg, **argv):
+    def __init__(self, cfg, term_size, **argv):
         """Objects init method.
         :param cfg: Configuration dictionary
         :type: configparser.ConfigParser
+        :param term_size: Current terminal size, number of available columns and rows
+        :type: TermSize
         :param argv["section_index"]: Number of scrolltext.text section in use [1..3]
-        :param argv["term_rows"]: Terminal height in number of rows
-        :param argv["term_columns"]: Terminal width in number of columns
         :param argv["min_scroll_line"]: The minimum terminal row allowed
         :param argv["test"]: Only used in unittests
         """
-        self.visible_text_length = argv["term_columns"]
+        self.term_size = term_size
+        self.min_scroll_line = argv["min_scroll_line"] if "min_scroll_line" in argv else 0
+        self.endless = cfg["main"].getboolean("endless")
 
         section_index = str(argv["section_index"]) if "section_index" in argv else "1"
         str_section = "scrolltext.text " + section_index
-        scroll_text = cfg[str_section]["text"]
-        scroll_line_str = cfg[str_section]["line"]
+        self.scroll_text = cfg[str_section]["text"]
+        self.scroll_line_str = cfg[str_section]["line"]
         scroll_direction = cfg[str_section].getboolean("direction")
 
-        self.line = get_linenum(scroll_line_str, argv["min_scroll_line"], argv["term_rows"])
-        log.debug("screenline %d", self.line)
-        log.debug("scrolltext length: %d", len(scroll_text))
-        log.debug("scrolltext part: >> %s <<", scroll_text[20:100])
-
-        num_blanks = argv["blanks"] if "blanks" in argv else self.visible_text_length
-        self.blanks = num_blanks * " "
-        self.complete_text = self.blanks + scroll_text + self.blanks
+        self.visible_text_length = -1
+        self._resized(**argv)
+
+        self._update_complete_text()
         self.pos = 0
+        self._last_pos = 0
         self.terminal_pos = len(self.complete_text)
         self.right_to_left = scroll_direction
         if "test" in argv:
             self.scrollspeedsec = 0
         else:
             self.scrollspeedsec = get_speedsec_float(cfg[str_section].getint("speed"))
-        if not self.right_to_left:
-            self.pos = 0
-            self.terminal_pos = len(self.complete_text)
-            self._pos_real = 0.
-            self._last_pos = 0
-        else:
-            self.pos = len(self.complete_text)
-            self.terminal_pos = -1
-            self._pos_real = float(self.pos)
-            self._last_pos = self.pos
+        self._set_start_params()
         self.last_time = time()
         self._text = self.complete_text
 
     def __iter__(self):
         return iter(self.next, None)
 
+    def _resized(self, **argv):
+        self.line = get_linenum(self.scroll_line_str,
+                                self.min_scroll_line, self.term_size.get_rows())
+        if self.term_size.get_cols() != self.visible_text_length:
+            self.visible_text_length = self.term_size.get_cols()
+            self.num_blanks = argv["blanks"] if "blanks" in argv else self.visible_text_length
+            self._update_complete_text()
+
+    def _update_complete_text(self):
+        blanks = self.num_blanks * " "
+        self.complete_text = blanks + self.scroll_text + (blanks if not self.endless else "")
+
     def next(self):
         """
         Gives the next visible text to display by the client-program.
 
         :returns: A str object of visible text length
         :rtype: str
         """
+        if self.term_size.is_resized():
+            self._resized()
         if not self.right_to_left:
             return self._next_left_to_right()
         return self._next_right_to_left()
 
     def _next_left_to_right(self):
         """
         Gives the next visible text to display by the client-program.
         Left-to-right reading text
 
         :returns: A str object of visible text length
         :rtype: str
         """
         if self.pos >= self.terminal_pos:
-            return None
+            if not self.endless:
+                return None
+            self._set_start_params()
         end = self.pos + self.visible_text_length
         win_text = self.complete_text[self.pos:end]
         if self.scrollspeedsec == 0:  # Special case for tests
             self.pos += 1
             return win_text
         time_now = time()
         delta = time_now - self.last_time
@@ -213,15 +254,17 @@
         Gives the next visible text to display by the client-program.
         Right-to-left reading text
 
         :returns: A str object of visible text length
         :rtype: str
         """
         if self.pos <= self.terminal_pos:
-            return None
+            if not self.endless:
+                return None
+            self._set_start_params()
         start = self.pos - self.visible_text_length
         win_text = self.complete_text[start:self.pos]
         if self.scrollspeedsec == 0:  # Special case for tests
             self.pos -= 1
             return win_text
         time_now = time()
         delta = time_now - self.last_time
@@ -229,7 +272,19 @@
         offset = delta / self.scrollspeedsec
         self._pos_real -= offset
         if int(self._pos_real) != self._last_pos:
             self.pos = int(self._pos_real)
             self._last_pos = self.pos
         self._text = win_text
         return self._text
+
+    def _set_start_params(self):
+        if not self.right_to_left:
+            self.pos = 0
+            self.terminal_pos = len(self.complete_text)
+            self._pos_real = 0.
+            self._last_pos = 0
+        else:
+            self.pos = len(self.complete_text)
+            self.terminal_pos = -1
+            self._pos_real = float(self.pos)
+            self._last_pos = self.pos
```

### Comparing `scrolltext-0.0.8/scrolltext.egg-info/PKG-INFO` & `scrolltext-0.0.9/scrolltext.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrolltext
-Version: 0.0.8
+Version: 0.0.9
 Summary: A little toy for scrolling text.
 Home-page: https://github.com/jimdeekepler/python-scrolltext
 Author: Jim Dee Kepler
 Author-email: jimdee@gmail.com
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -86,19 +86,25 @@
 Fastest scrolling speed.
 
     SCROLL_SPEED=10 scrolltext
 
 
 ## Bugs and quirks
 
- - does not detect term-resize
+ - attempts to detect term-resize, and clumsily adjusts some things
  - no colors
 
 
 ## Changes
 
+### v0.0.9
+
+ - attempt to handle term resizes
+ - added config-option: endless  (see newly generated config-file)
+ - removed logging from main branch (you may find it on the devel branch)
+
 ### v0.0.8
 
  - doc-comments have never been generated, nor are those validated. (TODO)
  - renamed log-file to "scrolltext.log"
  - uses config file "scrolltextrc"
    \*NIX uses "~/.config/scrolltextrc", windows uses "scrolltextrc" in current directory
```

### Comparing `scrolltext-0.0.8/setup.cfg` & `scrolltext-0.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = scrolltext
-version = 0.0.8
+version = 0.0.9
 author = Jim Dee Kepler
 author_email = jimdee@gmail.com
 license = GPLv3
 description = A little toy for scrolling text.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license.file = "LICENSE"
```

