# Comparing `tmp/drumpler_mammoth-2.1.1.tar.gz` & `tmp/drumpler_mammoth-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drumpler_mammoth-2.1.1.tar", last modified: Wed Apr 17 17:53:18 2024, max compression
+gzip compressed data, was "drumpler_mammoth-2.1.2.tar", last modified: Wed Apr 17 19:46:39 2024, max compression
```

## Comparing `drumpler_mammoth-2.1.1.tar` & `drumpler_mammoth-2.1.2.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 17:53:18.873572 drumpler_mammoth-2.1.1/
--rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler_mammoth-2.1.1/LICENSE
--rw-r--r--   0 Karel      (503) staff       (20)     4083 2024-04-17 17:53:18.872629 drumpler_mammoth-2.1.1/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler_mammoth-2.1.1/README.md
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 17:53:18.868033 drumpler_mammoth-2.1.1/drumpler_mammoth/
--rw-r--r--   0 Karel      (503) staff       (20)       30 2024-04-16 20:58:49.000000 drumpler_mammoth-2.1.1/drumpler_mammoth/__init__.py
--rw-r--r--   0 Karel      (503) staff       (20)      301 2024-04-16 21:10:49.000000 drumpler_mammoth-2.1.1/drumpler_mammoth/config.py
--rw-r--r--   0 Karel      (503) staff       (20)     3132 2024-04-16 23:32:45.000000 drumpler_mammoth-2.1.1/drumpler_mammoth/http_request.py
--rw-r--r--   0 Karel      (503) staff       (20)     6039 2024-04-17 17:49:15.000000 drumpler_mammoth-2.1.1/drumpler_mammoth/mammoth.py
--rw-r--r--   0 Karel      (503) staff       (20)      938 2024-04-17 16:38:09.000000 drumpler_mammoth-2.1.1/drumpler_mammoth/mylogger.py
-drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 17:53:18.871715 drumpler_mammoth-2.1.1/drumpler_mammoth.egg-info/
--rw-r--r--   0 Karel      (503) staff       (20)     4083 2024-04-17 17:53:18.000000 drumpler_mammoth-2.1.1/drumpler_mammoth.egg-info/PKG-INFO
--rw-r--r--   0 Karel      (503) staff       (20)      371 2024-04-17 17:53:18.000000 drumpler_mammoth-2.1.1/drumpler_mammoth.egg-info/SOURCES.txt
--rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-17 17:53:18.000000 drumpler_mammoth-2.1.1/drumpler_mammoth.egg-info/dependency_links.txt
--rw-r--r--   0 Karel      (503) staff       (20)       23 2024-04-17 17:53:18.000000 drumpler_mammoth-2.1.1/drumpler_mammoth.egg-info/requires.txt
--rw-r--r--   0 Karel      (503) staff       (20)       17 2024-04-17 17:53:18.000000 drumpler_mammoth-2.1.1/drumpler_mammoth.egg-info/top_level.txt
--rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-17 17:53:18.873768 drumpler_mammoth-2.1.1/setup.cfg
--rw-r--r--   0 Karel      (503) staff       (20)      725 2024-04-17 17:53:06.000000 drumpler_mammoth-2.1.1/setup.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 19:46:39.490521 drumpler_mammoth-2.1.2/
+-rw-r--r--   0 Karel      (503) staff       (20)     1068 2024-04-01 14:29:50.000000 drumpler_mammoth-2.1.2/LICENSE
+-rw-r--r--   0 Karel      (503) staff       (20)     4083 2024-04-17 19:46:39.489819 drumpler_mammoth-2.1.2/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)     3538 2024-04-09 21:15:49.000000 drumpler_mammoth-2.1.2/README.md
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 19:46:39.485137 drumpler_mammoth-2.1.2/drumpler_mammoth/
+-rw-r--r--   0 Karel      (503) staff       (20)       30 2024-04-16 20:58:49.000000 drumpler_mammoth-2.1.2/drumpler_mammoth/__init__.py
+-rw-r--r--   0 Karel      (503) staff       (20)     3132 2024-04-16 23:32:45.000000 drumpler_mammoth-2.1.2/drumpler_mammoth/http_request.py
+-rw-r--r--   0 Karel      (503) staff       (20)     5973 2024-04-17 19:46:23.000000 drumpler_mammoth-2.1.2/drumpler_mammoth/mammoth.py
+-rw-r--r--   0 Karel      (503) staff       (20)      938 2024-04-17 16:38:09.000000 drumpler_mammoth-2.1.2/drumpler_mammoth/mylogger.py
+drwxr-xr-x   0 Karel      (503) staff       (20)        0 2024-04-17 19:46:39.488878 drumpler_mammoth-2.1.2/drumpler_mammoth.egg-info/
+-rw-r--r--   0 Karel      (503) staff       (20)     4083 2024-04-17 19:46:39.000000 drumpler_mammoth-2.1.2/drumpler_mammoth.egg-info/PKG-INFO
+-rw-r--r--   0 Karel      (503) staff       (20)      344 2024-04-17 19:46:39.000000 drumpler_mammoth-2.1.2/drumpler_mammoth.egg-info/SOURCES.txt
+-rw-r--r--   0 Karel      (503) staff       (20)        1 2024-04-17 19:46:39.000000 drumpler_mammoth-2.1.2/drumpler_mammoth.egg-info/dependency_links.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       23 2024-04-17 19:46:39.000000 drumpler_mammoth-2.1.2/drumpler_mammoth.egg-info/requires.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       17 2024-04-17 19:46:39.000000 drumpler_mammoth-2.1.2/drumpler_mammoth.egg-info/top_level.txt
+-rw-r--r--   0 Karel      (503) staff       (20)       38 2024-04-17 19:46:39.490647 drumpler_mammoth-2.1.2/setup.cfg
+-rw-r--r--   0 Karel      (503) staff       (20)      725 2024-04-17 19:46:29.000000 drumpler_mammoth-2.1.2/setup.py
```

### Comparing `drumpler_mammoth-2.1.1/LICENSE` & `drumpler_mammoth-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `drumpler_mammoth-2.1.1/PKG-INFO` & `drumpler_mammoth-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drumpler_mammoth
-Version: 2.1.1
+Version: 2.1.2
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler-Mammoth
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `drumpler_mammoth-2.1.1/README.md` & `drumpler_mammoth-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `drumpler_mammoth-2.1.1/drumpler_mammoth/http_request.py` & `drumpler_mammoth-2.1.2/drumpler_mammoth/http_request.py`

 * *Files identical despite different names*

### Comparing `drumpler_mammoth-2.1.1/drumpler_mammoth/mammoth.py` & `drumpler_mammoth-2.1.2/drumpler_mammoth/mammoth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import requests
 import json
 import signal
 import threading
 import multiprocessing
 from .http_request import HttpRequest  # Make sure to import your HttpRequest class
-from .config import Config
 from .mylogger import MyLogger
 
-
 class Mammoth:
-    def __init__(self, process_request_data, drumpler_url=Config.DRUMPLER_URL, num_workers=1, custom_value=None):
+    def __init__(self, drumpler_url, authorization_key, custom_value, process_request_data, num_workers=None):
         self.drumpler_url = drumpler_url
-        self.user_process_request_data = process_request_data
-        self.auth_key = Config.AUTHORIZATION_KEY  # Default value if not set
+        self.auth_key = authorization_key
         self.custom_value = custom_value
+        self.user_process_request_data = process_request_data
         
         # Initialize custom logger
         self.logger = MyLogger.get_logger()
         
         self.num_workers = num_workers if num_workers is not None else multiprocessing.cpu_count()
         
         # Signal handling to gracefully shutdown on SIGINT (CTRL+C)
```

### Comparing `drumpler_mammoth-2.1.1/drumpler_mammoth/mylogger.py` & `drumpler_mammoth-2.1.2/drumpler_mammoth/mylogger.py`

 * *Files identical despite different names*

### Comparing `drumpler_mammoth-2.1.1/drumpler_mammoth.egg-info/PKG-INFO` & `drumpler_mammoth-2.1.2/drumpler_mammoth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drumpler_mammoth
-Version: 2.1.1
+Version: 2.1.2
 Summary: Framework for rapidly developing a restful API that requires post processing
 Home-page: https://github.com/KarelOmab/Drumpler-Mammoth
 Author: Karel Tutsu
 Author-email: karel.tutsu@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `drumpler_mammoth-2.1.1/setup.py` & `drumpler_mammoth-2.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='drumpler_mammoth',
-    version='2.1.1',
+    version='2.1.2',
     author='Karel Tutsu',
     author_email='karel.tutsu@gmail.com',
     description='Framework for rapidly developing a restful API that requires post processing',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/KarelOmab/Drumpler-Mammoth',
     packages=find_packages(),
```

