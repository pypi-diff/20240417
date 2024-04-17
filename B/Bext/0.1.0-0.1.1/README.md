# Comparing `tmp/Bext-0.1.0.tar.gz` & `tmp/Bext-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Bext-0.1.0.tar", last modified: Thu Nov  9 21:45:42 2023, max compression
+gzip compressed data, was "Bext-0.1.1.tar", last modified: Wed Apr 17 13:50:21 2024, max compression
```

## Comparing `Bext-0.1.0.tar` & `Bext-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-11-09 21:45:42.627593 Bext-0.1.0/
--rw-rw-rw-   0        0        0     3051 2019-01-08 18:35:16.000000 Bext-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0       19 2019-01-08 18:32:41.000000 Bext-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3590 2023-11-09 21:45:42.626592 Bext-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3124 2023-11-09 21:44:57.000000 Bext-0.1.0/README.md
--rw-rw-rw-   0        0        0        0 2019-01-19 04:22:53.000000 Bext-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-11-09 21:45:42.627593 Bext-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1149 2023-02-16 20:51:08.000000 Bext-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-09 21:45:42.565454 Bext-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-11-09 21:45:42.613346 Bext-0.1.0/src/Bext.egg-info/
--rw-rw-rw-   0        0        0     3590 2023-11-09 21:45:42.000000 Bext-0.1.0/src/Bext.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-11-09 21:45:42.000000 Bext-0.1.0/src/Bext.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-09 21:45:42.000000 Bext-0.1.0/src/Bext.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-11-09 21:45:42.000000 Bext-0.1.0/src/Bext.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-11-09 21:45:42.000000 Bext-0.1.0/src/Bext.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-11-09 21:45:42.614345 Bext-0.1.0/src/bext/
--rw-rw-rw-   0        0        0    23049 2023-02-18 15:23:39.000000 Bext-0.1.0/src/bext/__init__.py
-drwxrwxrwx   0        0        0        0 2023-11-09 21:45:42.624593 Bext-0.1.0/tests/
--rw-rw-rw-   0        0        0      183 2019-01-08 18:32:41.000000 Bext-0.1.0/tests/test_bext.py
+drwxrwxrwx   0        0        0        0 2024-04-17 13:50:21.480094 Bext-0.1.1/
+-rw-rw-rw-   0        0        0     3051 2019-01-08 18:35:16.000000 Bext-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       19 2019-01-08 18:32:41.000000 Bext-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4405 2024-04-17 13:50:21.480094 Bext-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3124 2023-11-09 21:44:57.000000 Bext-0.1.1/README.md
+-rw-rw-rw-   0        0        0        0 2019-01-19 04:22:53.000000 Bext-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-17 13:50:21.480094 Bext-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1149 2023-02-16 20:51:08.000000 Bext-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 13:50:21.436276 Bext-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-17 13:50:21.480094 Bext-0.1.1/src/Bext.egg-info/
+-rw-rw-rw-   0        0        0     4405 2024-04-17 13:50:21.000000 Bext-0.1.1/src/Bext.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2024-04-17 13:50:21.000000 Bext-0.1.1/src/Bext.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 13:50:21.000000 Bext-0.1.1/src/Bext.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-17 13:50:21.000000 Bext-0.1.1/src/Bext.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-17 13:50:21.000000 Bext-0.1.1/src/Bext.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 13:50:21.480094 Bext-0.1.1/src/bext/
+-rw-rw-rw-   0        0        0    23067 2024-04-17 13:41:13.000000 Bext-0.1.1/src/bext/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 13:50:21.480094 Bext-0.1.1/tests/
+-rw-rw-rw-   0        0        0      183 2019-01-08 18:32:41.000000 Bext-0.1.1/tests/test_bext.py
```

### Comparing `Bext-0.1.0/LICENSE.txt` & `Bext-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Bext-0.1.0/PKG-INFO` & `Bext-0.1.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: Bext
-Version: 0.1.0
-Summary: A cross-platform Python 2/3 module for colorful, boring, text-based terminal programs.
-Home-page: https://github.com/asweigart/bext
-Author: Al Sweigart
-Author-email: al@inventwithpython.com
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 Bext
 ======
 
 A cross-platform Python 2/3 module for colorful, boring, text-based terminal programs.
 
 Basically, use Bext if you want to move the cursor around the terminal window and have colorful text, like some kind of limited curses module (but it works on Windows also.)
```

### Comparing `Bext-0.1.0/setup.py` & `Bext-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `Bext-0.1.0/src/bext/__init__.py` & `Bext-0.1.1/src/bext/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Bext
 # By Al Sweigart al@inventwithpython.com
 # Copyright 2019, BSD 3-Clause license, see LICENSE file.
 # Built on top of Colorama by Jonathan Hartley
 
 # TODO - read https://learn.microsoft.com/en-us/windows/console/console-virtual-terminal-sequences
 
-__version__ = '0.1.0'
+__version__ = '0.1.1'
 
 import colorama, sys, os, random, shutil
 from contextlib import contextmanager
 
 ALL_COLORS = ('black', 'red', 'green', 'yellow', 'blue', 'purple', 'cyan', 'white')
 
 class BextException(Exception):
@@ -393,15 +393,15 @@
         try:
             yield
         finally:
             termios.tcsetattr(
                 fd, termios.TCSADRAIN, old_settings
             )
 
-    def getchars(self, blocking=True):
+    def getcharsUnix(self, blocking=True):
         """Get characters on Unix."""
         with self.context():
             if blocking:
                 yield self.__decoded_stream.read(1)
             while select.select([self.fileno()], [], [], 0)[0]:
                 yield self.__decoded_stream.read(1)
 
@@ -423,26 +423,26 @@
             buffer += self.__decoder.decode(os.read(sys.stdin.fileno(), 1))
         return buffer
 
 
 class GetKeyWindows(object):
     def get_key(self, blocking=True):
         buffer = ''
-        for c in self.getchars(blocking):
+        for c in self.getcharsWindows(blocking):
             buffer += c.decode(encoding=locale.getpreferredencoding())
             if buffer not in windowsPrefixes:
                 break
 
         if buffer == '\x03':
             raise KeyboardInterrupt
         if buffer == '':
             return ''  # In non-blocking mode, return '' if nothing was pressed.
         return windowsCodeToNameMapping.get(buffer, buffer)
 
-    def getchars(self, blocking=True):
+    def getcharsWindows(self, blocking=True):
         """Get characters on Windows."""
 
         if blocking:
             yield msvcrt.getch()
         while msvcrt.kbhit():
             yield msvcrt.getch()
```

