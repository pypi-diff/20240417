# Comparing `tmp/dnsdist_console-1.4.4.tar.gz` & `tmp/dnsdist_console-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnsdist_console-1.4.4.tar", last modified: Sun Dec 10 08:11:20 2023, max compression
+gzip compressed data, was "dnsdist_console-1.4.5.tar", last modified: Wed Apr 17 09:30:32 2024, max compression
```

## Comparing `dnsdist_console-1.4.4.tar` & `dnsdist_console-1.4.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 08:11:20.488334 dnsdist_console-1.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2023-12-10 08:11:13.000000 dnsdist_console-1.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2023-12-10 08:11:20.484334 dnsdist_console-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4523 2023-12-10 08:11:13.000000 dnsdist_console-1.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 08:11:20.484334 dnsdist_console-1.4.4/dnsdist_console/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2023-12-10 08:11:13.000000 dnsdist_console-1.4.4/dnsdist_console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2023-12-10 08:11:13.000000 dnsdist_console-1.4.4/dnsdist_console/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2023-12-10 08:11:13.000000 dnsdist_console-1.4.4/dnsdist_console/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2023-12-10 08:11:13.000000 dnsdist_console-1.4.4/dnsdist_console/hashpwd.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2023-12-10 08:11:13.000000 dnsdist_console-1.4.4/dnsdist_console/key.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2023-12-10 08:11:13.000000 dnsdist_console-1.4.4/dnsdist_console/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 08:11:20.484334 dnsdist_console-1.4.4/dnsdist_console.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2023-12-10 08:11:20.000000 dnsdist_console-1.4.4/dnsdist_console.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      489 2023-12-10 08:11:20.000000 dnsdist_console-1.4.4/dnsdist_console.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-10 08:11:20.000000 dnsdist_console-1.4.4/dnsdist_console.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-10 08:11:20.000000 dnsdist_console-1.4.4/dnsdist_console.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-10 08:11:20.000000 dnsdist_console-1.4.4/dnsdist_console.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-10 08:11:20.488334 dnsdist_console-1.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      890 2023-12-10 08:11:20.000000 dnsdist_console-1.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 08:11:20.484334 dnsdist_console-1.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-10 08:11:13.000000 dnsdist_console-1.4.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2023-12-10 08:11:13.000000 dnsdist_console-1.4.4/tests/test_console.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2023-12-10 08:11:13.000000 dnsdist_console-1.4.4/tests/test_hashpwd.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2023-12-10 08:11:13.000000 dnsdist_console-1.4.4/tests/test_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2023-12-10 08:11:13.000000 dnsdist_console-1.4.4/tests/test_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:30:32.976262 dnsdist_console-1.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-17 09:30:20.000000 dnsdist_console-1.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-17 09:30:32.976262 dnsdist_console-1.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-04-17 09:30:20.000000 dnsdist_console-1.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:30:32.972262 dnsdist_console-1.4.5/dnsdist_console/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-17 09:30:20.000000 dnsdist_console-1.4.5/dnsdist_console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-17 09:30:20.000000 dnsdist_console-1.4.5/dnsdist_console/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-17 09:30:20.000000 dnsdist_console-1.4.5/dnsdist_console/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-17 09:30:20.000000 dnsdist_console-1.4.5/dnsdist_console/hashpwd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-17 09:30:20.000000 dnsdist_console-1.4.5/dnsdist_console/key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-17 09:30:20.000000 dnsdist_console-1.4.5/dnsdist_console/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:30:32.976262 dnsdist_console-1.4.5/dnsdist_console.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-17 09:30:32.000000 dnsdist_console-1.4.5/dnsdist_console.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-17 09:30:32.000000 dnsdist_console-1.4.5/dnsdist_console.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:30:32.000000 dnsdist_console-1.4.5/dnsdist_console.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 09:30:32.000000 dnsdist_console-1.4.5/dnsdist_console.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-17 09:30:32.000000 dnsdist_console-1.4.5/dnsdist_console.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 09:30:32.976262 dnsdist_console-1.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-17 09:30:32.000000 dnsdist_console-1.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:30:32.976262 dnsdist_console-1.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:30:20.000000 dnsdist_console-1.4.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-17 09:30:20.000000 dnsdist_console-1.4.5/tests/test_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-17 09:30:20.000000 dnsdist_console-1.4.5/tests/test_hashpwd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-17 09:30:20.000000 dnsdist_console-1.4.5/tests/test_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-17 09:30:20.000000 dnsdist_console-1.4.5/tests/test_statistics.py
```

### Comparing `dnsdist_console-1.4.4/LICENSE` & `dnsdist_console-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dnsdist_console-1.4.4/PKG-INFO` & `dnsdist_console-1.4.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnsdist_console
-Version: 1.4.4
+Version: 1.4.5
 Summary: Python client for dnsdist console
 Home-page: https://github.com/dmachard/dnsdist_console
 Author: Denis MACHARD
 Author-email: d.machard@gmail.com
 Keywords: dnsdist console client
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 Requires-Dist: libnacl
 Requires-Dist: scrypt
 
 # Python client for dnsdist console
 
 Tool to interact with your dnsdist console from Python.
 
-![powerdns dnsdist 1.6.x](https://img.shields.io/badge/dnsdist%201.6.x-tested-green) ![powerdns dnsdist 1.7.x](https://img.shields.io/badge/dnsdist%201.7.x-tested-green) ![powerdns dnsdist 1.8.x](https://img.shields.io/badge/dnsdist%201.8.x-tested-green) 
+![powerdns dnsdist 1.9.x](https://img.shields.io/badge/dnsdist%201.9.x-tested-green) ![powerdns dnsdist 1.8.x](https://img.shields.io/badge/dnsdist%201.8.x-tested-green) ![powerdns dnsdist 1.7.x](https://img.shields.io/badge/dnsdist%201.7.x-tested-green) ![powerdns dnsdist 1.6.x](https://img.shields.io/badge/dnsdist%201.6.x-tested-green) 
 
 ## Table of contents
 * [Installation](#installation)
 * [Generate console key](#generate-console-key)
 * [Generate hash password](#generate-hash-password)
 * [Run command](#run-command)
 * [Get statistics](#get-statistics)
```

### Comparing `dnsdist_console-1.4.4/README.md` & `dnsdist_console-1.4.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Python client for dnsdist console
 
 Tool to interact with your dnsdist console from Python.
 
-![powerdns dnsdist 1.6.x](https://img.shields.io/badge/dnsdist%201.6.x-tested-green) ![powerdns dnsdist 1.7.x](https://img.shields.io/badge/dnsdist%201.7.x-tested-green) ![powerdns dnsdist 1.8.x](https://img.shields.io/badge/dnsdist%201.8.x-tested-green) 
+![powerdns dnsdist 1.9.x](https://img.shields.io/badge/dnsdist%201.9.x-tested-green) ![powerdns dnsdist 1.8.x](https://img.shields.io/badge/dnsdist%201.8.x-tested-green) ![powerdns dnsdist 1.7.x](https://img.shields.io/badge/dnsdist%201.7.x-tested-green) ![powerdns dnsdist 1.6.x](https://img.shields.io/badge/dnsdist%201.6.x-tested-green) 
 
 ## Table of contents
 * [Installation](#installation)
 * [Generate console key](#generate-console-key)
 * [Generate hash password](#generate-hash-password)
 * [Run command](#run-command)
 * [Get statistics](#get-statistics)
```

### Comparing `dnsdist_console-1.4.4/dnsdist_console/console.py` & `dnsdist_console-1.4.5/dnsdist_console/console.py`

 * *Files identical despite different names*

### Comparing `dnsdist_console-1.4.4/dnsdist_console/dashboard.py` & `dnsdist_console-1.4.5/dnsdist_console/dashboard.py`

 * *Files identical despite different names*

### Comparing `dnsdist_console-1.4.4/dnsdist_console/hashpwd.py` & `dnsdist_console-1.4.5/dnsdist_console/hashpwd.py`

 * *Files identical despite different names*

### Comparing `dnsdist_console-1.4.4/dnsdist_console/statistics.py` & `dnsdist_console-1.4.5/dnsdist_console/statistics.py`

 * *Files identical despite different names*

### Comparing `dnsdist_console-1.4.4/dnsdist_console.egg-info/PKG-INFO` & `dnsdist_console-1.4.5/dnsdist_console.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dnsdist-console
-Version: 1.4.4
+Name: dnsdist_console
+Version: 1.4.5
 Summary: Python client for dnsdist console
 Home-page: https://github.com/dmachard/dnsdist_console
 Author: Denis MACHARD
 Author-email: d.machard@gmail.com
 Keywords: dnsdist console client
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 Requires-Dist: libnacl
 Requires-Dist: scrypt
 
 # Python client for dnsdist console
 
 Tool to interact with your dnsdist console from Python.
 
-![powerdns dnsdist 1.6.x](https://img.shields.io/badge/dnsdist%201.6.x-tested-green) ![powerdns dnsdist 1.7.x](https://img.shields.io/badge/dnsdist%201.7.x-tested-green) ![powerdns dnsdist 1.8.x](https://img.shields.io/badge/dnsdist%201.8.x-tested-green) 
+![powerdns dnsdist 1.9.x](https://img.shields.io/badge/dnsdist%201.9.x-tested-green) ![powerdns dnsdist 1.8.x](https://img.shields.io/badge/dnsdist%201.8.x-tested-green) ![powerdns dnsdist 1.7.x](https://img.shields.io/badge/dnsdist%201.7.x-tested-green) ![powerdns dnsdist 1.6.x](https://img.shields.io/badge/dnsdist%201.6.x-tested-green) 
 
 ## Table of contents
 * [Installation](#installation)
 * [Generate console key](#generate-console-key)
 * [Generate hash password](#generate-hash-password)
 * [Run command](#run-command)
 * [Get statistics](#get-statistics)
```

### Comparing `dnsdist_console-1.4.4/setup.py` & `dnsdist_console-1.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open("README.md", "r") as fh:
     LONG_DESCRIPTION = fh.read()
     
 KEYWORDS = ('dnsdist console client')
 
 setuptools.setup(
     name="dnsdist_console",
-    version="1.4.4",
+    version="1.4.5",
     author="Denis MACHARD",
     author_email="d.machard@gmail.com",
     description="Python client for dnsdist console",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/dmachard/dnsdist_console",
     packages=['dnsdist_console', 'tests'],
```

### Comparing `dnsdist_console-1.4.4/tests/test_console.py` & `dnsdist_console-1.4.5/tests/test_console.py`

 * *Files identical despite different names*

### Comparing `dnsdist_console-1.4.4/tests/test_statistics.py` & `dnsdist_console-1.4.5/tests/test_statistics.py`

 * *Files identical despite different names*

