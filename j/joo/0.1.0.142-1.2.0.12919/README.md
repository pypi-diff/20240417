# Comparing `tmp/joo-0.1.0.142.tar.gz` & `tmp/joo-1.2.0.12919.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joo-0.1.0.142.tar", last modified: Fri Apr 12 09:02:01 2024, max compression
+gzip compressed data, was "joo-1.2.0.12919.tar", last modified: Wed Apr 17 06:27:56 2024, max compression
```

## Comparing `joo-0.1.0.142.tar` & `joo-1.2.0.12919.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 09:02:01.632316 joo-0.1.0.142/
--rw-rw-rw-   0        0        0      625 2024-04-12 09:02:01.628326 joo-0.1.0.142/PKG-INFO
--rw-rw-rw-   0        0        0       78 2024-04-12 09:01:55.000000 joo-0.1.0.142/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 09:02:01.460486 joo-0.1.0.142/lib/
-drwxrwxrwx   0        0        0        0 2024-04-12 09:02:01.551127 joo-0.1.0.142/lib/joo/
--rw-rw-rw-   0        0        0     1102 2024-03-27 11:42:14.000000 joo-0.1.0.142/lib/joo/LICENSE
--rw-rw-rw-   0        0        0     6197 2024-04-12 05:15:52.000000 joo-0.1.0.142/lib/joo/__init__.py
--rw-rw-rw-   0        0        0      759 2024-04-12 09:01:55.000000 joo-0.1.0.142/lib/joo/__version__.py
--rw-rw-rw-   0        0        0     2780 2024-04-12 03:38:16.000000 joo-0.1.0.142/lib/joo/cli.py
--rw-rw-rw-   0        0        0    12334 2024-04-12 09:01:46.000000 joo-0.1.0.142/lib/joo/datetimeutil.py
-drwxrwxrwx   0        0        0        0 2024-04-12 09:02:01.622814 joo-0.1.0.142/lib/joo/dc/
--rw-rw-rw-   0        0        0     8141 2024-04-11 09:21:46.000000 joo-0.1.0.142/lib/joo/dc/__init__.py
--rw-rw-rw-   0        0        0     4921 2024-04-09 06:59:29.000000 joo-0.1.0.142/lib/joo/dc/http.py
--rw-rw-rw-   0        0        0     9678 2024-04-09 05:54:46.000000 joo-0.1.0.142/lib/joo/dc/selenium.py
--rw-rw-rw-   0        0        0     5117 2024-04-12 09:01:46.000000 joo-0.1.0.142/lib/joo/httpapi.py
--rw-rw-rw-   0        0        0    11862 2024-04-12 09:01:46.000000 joo-0.1.0.142/lib/joo/logging.py
--rw-rw-rw-   0        0        0    15709 2024-04-12 08:55:08.000000 joo-0.1.0.142/lib/joo/sysutil.py
-drwxrwxrwx   0        0        0        0 2024-04-12 09:02:01.604997 joo-0.1.0.142/lib/joo.egg-info/
--rw-rw-rw-   0        0        0      625 2024-04-12 09:01:58.000000 joo-0.1.0.142/lib/joo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2024-04-12 09:01:59.000000 joo-0.1.0.142/lib/joo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 09:01:58.000000 joo-0.1.0.142/lib/joo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-04-12 09:01:58.000000 joo-0.1.0.142/lib/joo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 09:02:01.633313 joo-0.1.0.142/setup.cfg
--rw-rw-rw-   0        0        0     1424 2024-04-12 09:01:55.000000 joo-0.1.0.142/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:27:56.015875 joo-1.2.0.12919/
+-rw-rw-rw-   0        0        0      627 2024-04-17 06:27:56.014877 joo-1.2.0.12919/PKG-INFO
+-rw-rw-rw-   0        0        0       78 2024-04-17 06:27:52.000000 joo-1.2.0.12919/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 06:27:55.925117 joo-1.2.0.12919/lib/
+drwxrwxrwx   0        0        0        0 2024-04-17 06:27:55.959027 joo-1.2.0.12919/lib/joo/
+-rw-rw-rw-   0        0        0     1102 2024-03-27 11:42:14.000000 joo-1.2.0.12919/lib/joo/LICENSE
+-rw-rw-rw-   0        0        0     6203 2024-04-13 10:22:43.000000 joo-1.2.0.12919/lib/joo/__init__.py
+-rw-rw-rw-   0        0        0      761 2024-04-17 06:27:52.000000 joo-1.2.0.12919/lib/joo/__version__.py
+-rw-rw-rw-   0        0        0     2780 2024-04-12 03:38:16.000000 joo-1.2.0.12919/lib/joo/cli.py
+-rw-rw-rw-   0        0        0    12334 2024-04-12 09:01:46.000000 joo-1.2.0.12919/lib/joo/datetimeutil.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:27:56.001911 joo-1.2.0.12919/lib/joo/db/
+-rw-rw-rw-   0        0        0     6395 2024-04-17 06:27:52.000000 joo-1.2.0.12919/lib/joo/db/__init__.py
+-rw-rw-rw-   0        0        0    11031 2024-04-17 06:27:52.000000 joo-1.2.0.12919/lib/joo/db/mysql.py
+-rw-rw-rw-   0        0        0     1602 2024-04-17 06:27:52.000000 joo-1.2.0.12919/lib/joo/db/sqlbuilder.py
+-rw-rw-rw-   0        0        0     5117 2024-04-12 09:01:46.000000 joo-1.2.0.12919/lib/joo/httpapi.py
+-rw-rw-rw-   0        0        0    11862 2024-04-12 09:01:46.000000 joo-1.2.0.12919/lib/joo/logging.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:27:56.011885 joo-1.2.0.12919/lib/joo/scraping/
+-rw-rw-rw-   0        0        0     6077 2024-04-13 00:44:37.000000 joo-1.2.0.12919/lib/joo/scraping/__init__.py
+-rw-rw-rw-   0        0        0     4951 2024-04-13 00:57:32.000000 joo-1.2.0.12919/lib/joo/scraping/http.py
+-rw-rw-rw-   0        0        0     9707 2024-04-13 00:58:15.000000 joo-1.2.0.12919/lib/joo/scraping/selenium.py
+-rw-rw-rw-   0        0        0    17938 2024-04-13 09:27:24.000000 joo-1.2.0.12919/lib/joo/sysutil.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:27:55.990945 joo-1.2.0.12919/lib/joo.egg-info/
+-rw-rw-rw-   0        0        0      627 2024-04-17 06:27:54.000000 joo-1.2.0.12919/lib/joo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2024-04-17 06:27:54.000000 joo-1.2.0.12919/lib/joo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 06:27:54.000000 joo-1.2.0.12919/lib/joo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2024-04-17 06:27:54.000000 joo-1.2.0.12919/lib/joo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 06:27:56.015875 joo-1.2.0.12919/setup.cfg
+-rw-rw-rw-   0        0        0     1424 2024-04-17 06:27:52.000000 joo-1.2.0.12919/setup.py
```

### Comparing `joo-0.1.0.142/PKG-INFO` & `joo-1.2.0.12919/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joo
-Version: 0.1.0.142
+Version: 1.2.0.12919
 Summary: joo library
 Home-page: https://github.com/metatutu/joo
 Author: Wooloo Studio
 Author-email: max.wu@wooloostudio.com
 License: MIT License
 Project-URL: Documentation, https://github.com/metatutu/joo
 Project-URL: Source Code, https://github.com/metatutu/joo
```

### Comparing `joo-0.1.0.142/lib/joo/LICENSE` & `joo-1.2.0.12919/lib/joo/LICENSE`

 * *Files identical despite different names*

### Comparing `joo-0.1.0.142/lib/joo/__init__.py` & `joo-1.2.0.12919/lib/joo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             ManagedObject.__del__(self)
     """
     def __init__(self):
         self._state = None
 
     def __del__(self):
         if self._state != None:
-            raise Exception("Object must be released explicitly.")
+            raise Exception("Object must be released explicitly.", self)
         
     @property
     def state(self): return self._state
 
 class ManagedObjects(list):
     """List of objects to be managed.
```

### Comparing `joo-0.1.0.142/lib/joo/__version__.py` & `joo-1.2.0.12919/lib/joo/__version__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,16 @@
     This file is part of joo library.
     :copyright: Copyright 1993-2024 Wooloo Studio.  All rights reserved.
     :license: MIT, check LICENSE for details.
 """
 __VERSION__ = {
     "name": "joo",
     "description": "joo library",
-    "version": "0.1.0",
-    "build": 142,
+    "version": "1.2.0",
+    "build": 12919,
     "license": "MIT License",
     "author": "Wooloo Studio",
     "author_email": "max.wu@wooloostudio.com",
     "url": "https://github.com/metatutu/joo",
     "project_urls": {
         "Documentation": "https://github.com/metatutu/joo",
         "Source Code": "https://github.com/metatutu/joo",
```

### Comparing `joo-0.1.0.142/lib/joo/cli.py` & `joo-1.2.0.12919/lib/joo/cli.py`

 * *Files identical despite different names*

### Comparing `joo-0.1.0.142/lib/joo/datetimeutil.py` & `joo-1.2.0.12919/lib/joo/datetimeutil.py`

 * *Files identical despite different names*

### Comparing `joo-0.1.0.142/lib/joo/dc/http.py` & `joo-1.2.0.12919/lib/joo/scraping/http.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
     This file is part of joo library.
     :copyright: Copyright 1993-2024 Wooloo Studio.  All rights reserved.
     :license: MIT, check LICENSE for details.
 """
 import requests
 import joo.sysutil as sysutil
-from joo.dc import Session, Cache
+from joo.scraping import Session as SessionBase
 
-class HttpSession(Session):
+class Session(SessionBase):
     def __init__(self):
-        Session.__init__(self)
+        SessionBase.__init__(self)
 
         # settings
         self.user_agent = None
         self.ok_status_codes = [200]
 
     def open(self, **kwargs):
         try:
@@ -104,35 +104,35 @@
         kwargs["retries"] = retries
         return self.request("POST", url, **kwargs)
 
     def _get_page(self, url, cache, format, **kwargs):
         if format == "html":
             # read from cache
             if cache:
-                key = Cache.make_key(url)
+                key = sysutil.Cache.make_key(url)
                 content = cache.get(key)
                 if content: return self.bytes_str(content)
 
             # read from online
             retries = kwargs.pop("retries", 0)
             response = self.get(url, retries, **kwargs)
             if response:
                 if response.status_code == 200:
                     if cache:
-                        key = Cache.make_key(url)
+                        key = sysutil.Cache.make_key(url)
                         cache.set(key, response.content)
                     return self.bytes_str(response.content, response.encoding)
 
         #
         return None
 
     @classmethod
     def download(cls, url, filepath, retries=0, create_parent=True, **kwargs):
         success = False
-        session = HttpSession()
+        session = Session()
         try:
             response = session.get(url, retries, **kwargs)
             if response:
                 if response.status_code == 200:
                     success = sysutil.save_file_bytes(filepath, response.content, create_parent)
         except:
             pass
```

### Comparing `joo-0.1.0.142/lib/joo/dc/selenium.py` & `joo-1.2.0.12919/lib/joo/scraping/selenium.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 """
 import os
 import time
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from bs4 import BeautifulSoup
 import joo.sysutil as sysutil
-from joo.dc import Session, Cache
+from joo.scraping import Session as SessionBase
 
-class WebDriverSession(Session):
+class Session(SessionBase):
     def __init__(self):
-        Session.__init__(self)
+        SessionBase.__init__(self)
 
         # settings
         self.webdriver = "chrome"
         self.desired_capabilities = None
         self.options = None
         self.default_timeout = 10.0
         self.default_wait = 0.5
@@ -80,26 +80,26 @@
             self.exception(ex)
             return None
 
     def _get_page(self, url, cache, format, **kwargs):
         if format == "html":
             # read from cache
             if cache:
-                key = Cache.make_key(url)
+                key = sysutil.Cache.make_key(url)
                 content = cache.get(key, text_format=True)
                 if content: return content
 
             # read from online
             wait = kwargs.pop("wait", 0)
             self.get(url)
             self.wait(wait)
             html = self.get_html()
             if html:
                 if cache:
-                    key = Cache.make_key(url)
+                    key = sysutil.Cache.make_key(url)
                     cache.set(key, html, text_format=True)
                 return html
 
         #
         return None
 
     def get_url(self, leading_wait=2.0, timeout=None, wait=None):
```

### Comparing `joo-0.1.0.142/lib/joo/httpapi.py` & `joo-1.2.0.12919/lib/joo/httpapi.py`

 * *Files identical despite different names*

### Comparing `joo-0.1.0.142/lib/joo/logging.py` & `joo-1.2.0.12919/lib/joo/logging.py`

 * *Files identical despite different names*

### Comparing `joo-0.1.0.142/lib/joo/sysutil.py` & `joo-1.2.0.12919/lib/joo/sysutil.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,19 +4,22 @@
     :license: MIT, check LICENSE for details.
 """
 import os
 import re
 import sys
 import json
 import uuid
+import time
 import shutil
 import base64
 import getopt
+import hashlib
 import datetime
 import tempfile
+from abc import ABC, abstractmethod
 from joo import ManagedObject, ManagedObjects
 if os.name == "posix":
     import fcntl
 
 def create_folder(folderpath):
     try:
         if not os.path.exists(folderpath): os.makedirs(folderpath)
@@ -245,23 +248,22 @@
         # detach
         fpath = self._fpath
         self._fpath = None
         self._state = None
         return fpath
 
     def delete(self):
-        # detach
-        fpath = self.detach()
-
         # delete
-        if fpath is None: return
-        if self._is_folder:
-            delete_folder(self._fpath)
-        else:
-            delete_file(self._fpath)
+        if self._fpath:
+            if self._is_folder:
+                delete_folder(self._fpath)
+            else:
+                delete_file(self._fpath)
+        self._fpath = None
+        self._state = None
 
 class TempFile(TempFileSystemObject):
     def __init__(self, temp_folderpath=None):
         TempFileSystemObject.__init__(self)
         self._is_folder = False
         self.create(temp_folderpath)
 
@@ -422,14 +424,77 @@
             else:
                 if os.path.realpath(fpath) == fpath_lockfile: continue
                 delete_file(fpath)
 
 FSL = FileSystemLock
 FSLock = FileSystemLock
 
+class Cache(ABC):
+    @abstractmethod
+    def set(self, key, value, text_format=False): pass
+
+    @abstractmethod
+    def remove(self, key): pass
+
+    @abstractmethod
+    def get(self, key, valid_period=0, text_format=False): pass
+
+    @abstractmethod
+    def clear(self, valid_period=0): pass
+
+    @classmethod
+    def make_key(cls, resource_id):
+        return hashlib.md5(resource_id.encode(encoding="utf-8")).hexdigest()
+    
+class FileSystemCache(Cache, FileSystemDataStore):
+    def __init__(self, root_folderpath=None):
+        FileSystemDataStore.__init__(self, root_folderpath)
+
+    def _get_filepath(self, key):
+        return self.get_path(key, True)
+
+    def set(self, key, value, text_format=False):
+        fpath = self._get_filepath(key)
+        if value is None:
+            delete_file(fpath)
+        else:
+            if text_format:
+                save_file_contents(fpath, value)
+            else:
+                save_file_bytes(fpath, value)
+
+    def remove(self, key):
+        fpath = self._get_filepath(key)
+        delete_file(fpath)
+
+    def get(self, key, valid_period=0, text_format=False):
+        fpath = self._get_filepath(key)
+        if not file_exists(fpath): return None
+        if valid_period > 0:
+            # NOTE: getctime() is with issue on some systems.
+            # For example, on Windows with some file system (aka. drives), when a file
+            # is deleted and recreated, the ctime could be as the file before it's deleted.
+            if (time.time() - os.path.getmtime(fpath)) > valid_period: return None
+        if text_format:
+            return load_file_contents(fpath)
+        else:
+            return load_file_bytes(fpath)
+
+    def clear(self, valid_period=0):
+        fpaths = list_files(self.root_folderpath)
+        t_now = time.time()
+        if fpaths is None: return
+        if valid_period > 0:
+            for fpath in fpaths:
+                if (t_now - os.path.getmtime(fpath)) > valid_period:
+                    delete_file(fpath)
+        else:
+            for fpath in fpaths:
+                delete_file(fpath)
+
 def parse_command_line(parts):
     """Parse command line.
 
     Syntax of command list is as:
     program <command 1> <command 2> ... [option 1] [option 2] ...
 
     Commands are required and options are optional, and commands are always
```

### Comparing `joo-0.1.0.142/lib/joo.egg-info/PKG-INFO` & `joo-1.2.0.12919/lib/joo.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joo
-Version: 0.1.0.142
+Version: 1.2.0.12919
 Summary: joo library
 Home-page: https://github.com/metatutu/joo
 Author: Wooloo Studio
 Author-email: max.wu@wooloostudio.com
 License: MIT License
 Project-URL: Documentation, https://github.com/metatutu/joo
 Project-URL: Source Code, https://github.com/metatutu/joo
```

### Comparing `joo-0.1.0.142/setup.py` & `joo-1.2.0.12919/setup.py`

 * *Files identical despite different names*

