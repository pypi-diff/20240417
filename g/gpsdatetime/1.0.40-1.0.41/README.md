# Comparing `tmp/gpsdatetime-1.0.40.tar.gz` & `tmp/gpsdatetime-1.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpsdatetime-1.0.40.tar", last modified: Fri Sep  1 12:45:11 2023, max compression
+gzip compressed data, was "gpsdatetime-1.0.41.tar", last modified: Wed Apr 17 16:52:13 2024, max compression
```

## Comparing `gpsdatetime-1.0.40.tar` & `gpsdatetime-1.0.41.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 beilin    (1000) beilin    (1000)        0 2023-09-01 12:45:11.351794 gpsdatetime-1.0.40/
--rw-r--r--   0 beilin    (1000) beilin    (1000)    22118 2018-11-27 11:41:19.000000 gpsdatetime-1.0.40/LICENCE.txt
--rw-r--r--   0 beilin    (1000) beilin    (1000)       73 2021-02-27 15:24:38.000000 gpsdatetime-1.0.40/MANIFEST.in
--rw-rw-r--   0 beilin    (1000) beilin    (1000)     5334 2023-09-01 12:45:11.351794 gpsdatetime-1.0.40/PKG-INFO
--rw-r--r--   0 beilin    (1000) beilin    (1000)     4915 2023-09-01 12:44:29.000000 gpsdatetime-1.0.40/README.md
--rw-r--r--   0 beilin    (1000) beilin    (1000)       90 2023-08-22 14:34:04.000000 gpsdatetime-1.0.40/__init__.py
-drwxrwxr-x   0 beilin    (1000) beilin    (1000)        0 2023-09-01 12:45:11.347794 gpsdatetime-1.0.40/gpsdatetime/
--rw-r--r--   0 beilin    (1000) beilin    (1000)       68 2023-08-22 14:34:07.000000 gpsdatetime-1.0.40/gpsdatetime/__init__.py
--rw-r--r--   0 beilin    (1000) beilin    (1000)    22896 2023-08-30 08:22:53.000000 gpsdatetime-1.0.40/gpsdatetime/gpsdatetime.py
--rw-rw-r--   0 beilin    (1000) beilin    (1000)      450 2022-12-09 15:29:36.000000 gpsdatetime-1.0.40/gpsdatetime/gpstime.py
-drwxrwxr-x   0 beilin    (1000) beilin    (1000)        0 2023-09-01 12:45:11.351794 gpsdatetime-1.0.40/gpsdatetime.egg-info/
--rw-rw-r--   0 beilin    (1000) beilin    (1000)     5334 2023-09-01 12:45:11.000000 gpsdatetime-1.0.40/gpsdatetime.egg-info/PKG-INFO
--rw-rw-r--   0 beilin    (1000) beilin    (1000)      278 2023-09-01 12:45:11.000000 gpsdatetime-1.0.40/gpsdatetime.egg-info/SOURCES.txt
--rw-rw-r--   0 beilin    (1000) beilin    (1000)        1 2023-09-01 12:45:11.000000 gpsdatetime-1.0.40/gpsdatetime.egg-info/dependency_links.txt
--rw-rw-r--   0 beilin    (1000) beilin    (1000)       12 2023-09-01 12:45:11.000000 gpsdatetime-1.0.40/gpsdatetime.egg-info/top_level.txt
--rw-rw-r--   0 beilin    (1000) beilin    (1000)       79 2023-09-01 12:45:11.351794 gpsdatetime-1.0.40/setup.cfg
--rw-rw-r--   0 beilin    (1000) beilin    (1000)     1707 2023-09-01 12:41:30.000000 gpsdatetime-1.0.40/setup.py
+drwxrwxr-x   0 beilin    (1000) beilin    (1000)        0 2024-04-17 16:52:13.348986 gpsdatetime-1.0.41/
+-rw-r--r--   0 beilin    (1000) beilin    (1000)    22118 2018-11-27 11:41:19.000000 gpsdatetime-1.0.41/LICENCE.txt
+-rw-r--r--   0 beilin    (1000) beilin    (1000)       73 2021-02-27 15:24:38.000000 gpsdatetime-1.0.41/MANIFEST.in
+-rw-r--r--   0 beilin    (1000) beilin    (1000)     5296 2024-04-17 16:52:13.348986 gpsdatetime-1.0.41/PKG-INFO
+-rw-r--r--   0 beilin    (1000) beilin    (1000)     4914 2024-04-17 16:45:46.000000 gpsdatetime-1.0.41/README.md
+-rw-r--r--   0 beilin    (1000) beilin    (1000)       90 2023-08-22 14:34:04.000000 gpsdatetime-1.0.41/__init__.py
+drwxrwxr-x   0 beilin    (1000) beilin    (1000)        0 2024-04-17 16:52:13.348986 gpsdatetime-1.0.41/gpsdatetime/
+-rw-r--r--   0 beilin    (1000) beilin    (1000)       68 2023-08-22 14:34:07.000000 gpsdatetime-1.0.41/gpsdatetime/__init__.py
+-rw-r--r--   0 beilin    (1000) beilin    (1000)    22896 2023-08-30 08:22:53.000000 gpsdatetime-1.0.41/gpsdatetime/gpsdatetime.py
+-rw-rw-r--   0 beilin    (1000) beilin    (1000)      450 2022-12-09 15:29:36.000000 gpsdatetime-1.0.41/gpsdatetime/gpstime.py
+drwxrwxr-x   0 beilin    (1000) beilin    (1000)        0 2024-04-17 16:52:13.348986 gpsdatetime-1.0.41/gpsdatetime.egg-info/
+-rw-r--r--   0 beilin    (1000) beilin    (1000)     5296 2024-04-17 16:52:13.000000 gpsdatetime-1.0.41/gpsdatetime.egg-info/PKG-INFO
+-rw-rw-r--   0 beilin    (1000) beilin    (1000)      278 2024-04-17 16:52:13.000000 gpsdatetime-1.0.41/gpsdatetime.egg-info/SOURCES.txt
+-rw-rw-r--   0 beilin    (1000) beilin    (1000)        1 2024-04-17 16:52:13.000000 gpsdatetime-1.0.41/gpsdatetime.egg-info/dependency_links.txt
+-rw-rw-r--   0 beilin    (1000) beilin    (1000)       12 2024-04-17 16:52:13.000000 gpsdatetime-1.0.41/gpsdatetime.egg-info/top_level.txt
+-rw-rw-r--   0 beilin    (1000) beilin    (1000)       79 2024-04-17 16:52:13.352985 gpsdatetime-1.0.41/setup.cfg
+-rw-rw-r--   0 beilin    (1000) beilin    (1000)     1707 2024-04-17 16:51:09.000000 gpsdatetime-1.0.41/setup.py
```

### Comparing `gpsdatetime-1.0.40/LICENCE.txt` & `gpsdatetime-1.0.41/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `gpsdatetime-1.0.40/PKG-INFO` & `gpsdatetime-1.0.41/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: gpsdatetime
-Version: 1.0.40
+Version: 1.0.41
 Summary: Python GPS date/time management package
 Home-page: https://gitlab.com/jbeilin/gpsdatetime
+Download-URL: https://gitlab.com/jbeilin/gpsdatetime/-/archive/v1.0.41/gpsdatetime-v1.0.41.tar.gz
 Author: Jacques Beilin
 Author-email: jacques.beilin@gmail.com
-License: UNKNOWN
-Download-URL: https://gitlab.com/jbeilin/gpsdatetime/-/archive/v1.0.40/gpsdatetime-v1.0.40.tar.gz
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 # gpsdatetime - Python GPS date/time management package
 
 This is a python library for GNSS date/time transformations
 
@@ -36,15 +34,15 @@
 * init from GPS week and second of week
 ```python
 t=gpst.gpsdatetime(wk=1400, wsec=600700)
 ```
 
 * init from usual time elements
 ```python
-t=gpst.gpsdatetime(yyyy=2016, mon=1, dd=7, hh=3, min=5, sec=5)
+t=gpst.gpsdatetime(yyyy=2016, mon=1, dd=7, h=3, min=5, sec=5)
 ```
 
 * init from SINEX time string
 ```python
 t=gpst.gpsdatetime('16:004:46888')
 ```
 
@@ -243,9 +241,7 @@
 ```
 
 ## licence
 
 Copyright (C) 2014-2023, Jacques Beilin / ENSG-Geomatique
 
 Distributed under terms of the CECILL-C licence.
-
-
```

### Comparing `gpsdatetime-1.0.40/README.md` & `gpsdatetime-1.0.41/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 * init from GPS week and second of week
 ```python
 t=gpst.gpsdatetime(wk=1400, wsec=600700)
 ```
 
 * init from usual time elements
 ```python
-t=gpst.gpsdatetime(yyyy=2016, mon=1, dd=7, hh=3, min=5, sec=5)
+t=gpst.gpsdatetime(yyyy=2016, mon=1, dd=7, h=3, min=5, sec=5)
 ```
 
 * init from SINEX time string
 ```python
 t=gpst.gpsdatetime('16:004:46888')
 ```
```

### Comparing `gpsdatetime-1.0.40/gpsdatetime/gpsdatetime.py` & `gpsdatetime-1.0.41/gpsdatetime/gpsdatetime.py`

 * *Files identical despite different names*

### Comparing `gpsdatetime-1.0.40/gpsdatetime.egg-info/PKG-INFO` & `gpsdatetime-1.0.41/gpsdatetime.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: gpsdatetime
-Version: 1.0.40
+Version: 1.0.41
 Summary: Python GPS date/time management package
 Home-page: https://gitlab.com/jbeilin/gpsdatetime
+Download-URL: https://gitlab.com/jbeilin/gpsdatetime/-/archive/v1.0.41/gpsdatetime-v1.0.41.tar.gz
 Author: Jacques Beilin
 Author-email: jacques.beilin@gmail.com
-License: UNKNOWN
-Download-URL: https://gitlab.com/jbeilin/gpsdatetime/-/archive/v1.0.40/gpsdatetime-v1.0.40.tar.gz
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 # gpsdatetime - Python GPS date/time management package
 
 This is a python library for GNSS date/time transformations
 
@@ -36,15 +34,15 @@
 * init from GPS week and second of week
 ```python
 t=gpst.gpsdatetime(wk=1400, wsec=600700)
 ```
 
 * init from usual time elements
 ```python
-t=gpst.gpsdatetime(yyyy=2016, mon=1, dd=7, hh=3, min=5, sec=5)
+t=gpst.gpsdatetime(yyyy=2016, mon=1, dd=7, h=3, min=5, sec=5)
 ```
 
 * init from SINEX time string
 ```python
 t=gpst.gpsdatetime('16:004:46888')
 ```
 
@@ -243,9 +241,7 @@
 ```
 
 ## licence
 
 Copyright (C) 2014-2023, Jacques Beilin / ENSG-Geomatique
 
 Distributed under terms of the CECILL-C licence.
-
-
```

### Comparing `gpsdatetime-1.0.40/setup.py` & `gpsdatetime-1.0.41/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from setuptools import setup
 import os.path as path
 import sys
 
 install_reqs = []
 
-VERSION="1.0.40"
+VERSION="1.0.41"
 
 if sys.platform.startswith('win'):
     install_reqs.append('pywin32')
     
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
```

