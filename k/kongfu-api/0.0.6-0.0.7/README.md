# Comparing `tmp/kongfu-api-0.0.6.tar.gz` & `tmp/kongfu-api-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kongfu-api-0.0.6.tar", last modified: Mon Apr  8 08:24:40 2024, max compression
+gzip compressed data, was "kongfu-api-0.0.7.tar", last modified: Wed Apr 17 04:09:52 2024, max compression
```

## Comparing `kongfu-api-0.0.6.tar` & `kongfu-api-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 zhudelong   (501) staff       (20)        0 2024-04-08 08:24:40.617045 kongfu-api-0.0.6/
--rw-r--r--   0 zhudelong   (501) staff       (20)      620 2024-04-08 08:24:40.612774 kongfu-api-0.0.6/PKG-INFO
--rw-r--r--   0 zhudelong   (501) staff       (20)      103 2024-02-20 01:47:07.000000 kongfu-api-0.0.6/README.md
-drwxr-xr-x   0 zhudelong   (501) staff       (20)        0 2024-04-08 08:24:40.600655 kongfu-api-0.0.6/kongfu_api/
--rw-r--r--   0 zhudelong   (501) staff       (20)       21 2024-03-15 02:22:53.000000 kongfu-api-0.0.6/kongfu_api/__init__.py
--rw-r--r--   0 zhudelong   (501) staff       (20)     1643 2024-04-08 08:24:15.000000 kongfu-api-0.0.6/kongfu_api/db.py
--rw-r--r--   0 zhudelong   (501) staff       (20)    45684 2024-03-25 05:12:32.000000 kongfu-api-0.0.6/kongfu_api/kongfu.py
--rw-r--r--   0 zhudelong   (501) staff       (20)     7419 2024-03-15 02:22:53.000000 kongfu-api-0.0.6/kongfu_api/tool.py
-drwxr-xr-x   0 zhudelong   (501) staff       (20)        0 2024-04-08 08:24:40.611083 kongfu-api-0.0.6/kongfu_api.egg-info/
--rw-r--r--   0 zhudelong   (501) staff       (20)      620 2024-04-08 08:24:40.000000 kongfu-api-0.0.6/kongfu_api.egg-info/PKG-INFO
--rw-r--r--   0 zhudelong   (501) staff       (20)      304 2024-04-08 08:24:40.000000 kongfu-api-0.0.6/kongfu_api.egg-info/SOURCES.txt
--rw-r--r--   0 zhudelong   (501) staff       (20)        1 2024-04-08 08:24:40.000000 kongfu-api-0.0.6/kongfu_api.egg-info/dependency_links.txt
--rw-r--r--   0 zhudelong   (501) staff       (20)       48 2024-04-08 08:24:40.000000 kongfu-api-0.0.6/kongfu_api.egg-info/entry_points.txt
--rw-r--r--   0 zhudelong   (501) staff       (20)       67 2024-04-08 08:24:40.000000 kongfu-api-0.0.6/kongfu_api.egg-info/requires.txt
--rw-r--r--   0 zhudelong   (501) staff       (20)       11 2024-04-08 08:24:40.000000 kongfu-api-0.0.6/kongfu_api.egg-info/top_level.txt
--rw-r--r--   0 zhudelong   (501) staff       (20)       38 2024-04-08 08:24:40.617351 kongfu-api-0.0.6/setup.cfg
--rw-r--r--   0 zhudelong   (501) staff       (20)     1500 2024-04-08 08:24:36.000000 kongfu-api-0.0.6/setup.py
+drwxr-xr-x   0 zhudelong   (501) staff       (20)        0 2024-04-17 04:09:52.897064 kongfu-api-0.0.7/
+-rw-r--r--   0 zhudelong   (501) staff       (20)      620 2024-04-17 04:09:52.894499 kongfu-api-0.0.7/PKG-INFO
+-rw-r--r--   0 zhudelong   (501) staff       (20)      103 2024-02-20 01:47:07.000000 kongfu-api-0.0.7/README.md
+drwxr-xr-x   0 zhudelong   (501) staff       (20)        0 2024-04-17 04:09:52.878657 kongfu-api-0.0.7/kongfu_api/
+-rw-r--r--   0 zhudelong   (501) staff       (20)       21 2024-03-15 02:22:53.000000 kongfu-api-0.0.7/kongfu_api/__init__.py
+-rw-r--r--   0 zhudelong   (501) staff       (20)     1643 2024-04-08 08:24:15.000000 kongfu-api-0.0.7/kongfu_api/db.py
+-rw-r--r--   0 zhudelong   (501) staff       (20)    45945 2024-04-17 03:53:29.000000 kongfu-api-0.0.7/kongfu_api/kongfu.py
+-rw-r--r--   0 zhudelong   (501) staff       (20)     7419 2024-03-15 02:22:53.000000 kongfu-api-0.0.7/kongfu_api/tool.py
+drwxr-xr-x   0 zhudelong   (501) staff       (20)        0 2024-04-17 04:09:52.892980 kongfu-api-0.0.7/kongfu_api.egg-info/
+-rw-r--r--   0 zhudelong   (501) staff       (20)      620 2024-04-17 04:09:52.000000 kongfu-api-0.0.7/kongfu_api.egg-info/PKG-INFO
+-rw-r--r--   0 zhudelong   (501) staff       (20)      304 2024-04-17 04:09:52.000000 kongfu-api-0.0.7/kongfu_api.egg-info/SOURCES.txt
+-rw-r--r--   0 zhudelong   (501) staff       (20)        1 2024-04-17 04:09:52.000000 kongfu-api-0.0.7/kongfu_api.egg-info/dependency_links.txt
+-rw-r--r--   0 zhudelong   (501) staff       (20)       48 2024-04-17 04:09:52.000000 kongfu-api-0.0.7/kongfu_api.egg-info/entry_points.txt
+-rw-r--r--   0 zhudelong   (501) staff       (20)       67 2024-04-17 04:09:52.000000 kongfu-api-0.0.7/kongfu_api.egg-info/requires.txt
+-rw-r--r--   0 zhudelong   (501) staff       (20)       11 2024-04-17 04:09:52.000000 kongfu-api-0.0.7/kongfu_api.egg-info/top_level.txt
+-rw-r--r--   0 zhudelong   (501) staff       (20)       38 2024-04-17 04:09:52.897276 kongfu-api-0.0.7/setup.cfg
+-rw-r--r--   0 zhudelong   (501) staff       (20)     1500 2024-04-17 04:09:41.000000 kongfu-api-0.0.7/setup.py
```

### Comparing `kongfu-api-0.0.6/PKG-INFO` & `kongfu-api-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kongfu-api
-Version: 0.0.6
+Version: 0.0.7
 Summary: sample wsgi server
 Author: smart_long
 Author-email: smart_long@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `kongfu-api-0.0.6/kongfu_api/db.py` & `kongfu-api-0.0.7/kongfu_api/db.py`

 * *Files identical despite different names*

### Comparing `kongfu-api-0.0.6/kongfu_api/kongfu.py` & `kongfu-api-0.0.7/kongfu_api/kongfu.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from urllib.parse import parse_qs
 import cgi
 import threading
 from io import BytesIO
 import xmldict
 import jwt
 import tempfile
+from decimal import Decimal
 from peewee import Field
 from .db import db, BaseModel
 
 
 sys.path.append(os.getcwd())
 
 # try:
@@ -91,14 +92,19 @@
             continue
 
         d[col[0]] = row[idx]
         if isinstance(row[idx], datetime.datetime):
             d[col[0]] = row[idx].strftime('%Y-%m-%d %H:%M:%S')
         elif isinstance(row[idx], datetime.date):
             d[col[0]] = row[idx].strftime('%Y-%m-%d')
+        elif isinstance(row[idx], Decimal):
+            if Decimal(str(row[idx])) == Decimal(str(row[idx])).to_integral_value():
+                d[col[0]] = int(row[idx])
+            else:
+                d[col[0]] = float(row[idx])
         else:
             d[col[0]] = row[idx]
     return d
 
 
 def get_permission(path_resource, path_operation):
     if path_resource in API_PERMISSION:
```

### Comparing `kongfu-api-0.0.6/kongfu_api/tool.py` & `kongfu-api-0.0.7/kongfu_api/tool.py`

 * *Files identical despite different names*

### Comparing `kongfu-api-0.0.6/kongfu_api.egg-info/PKG-INFO` & `kongfu-api-0.0.7/kongfu_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kongfu-api
-Version: 0.0.6
+Version: 0.0.7
 Summary: sample wsgi server
 Author: smart_long
 Author-email: smart_long@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `kongfu-api-0.0.6/setup.py` & `kongfu-api-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # these things are needed for the README.md show on pypi (if you dont need delete it)
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 # you need to change all these
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'sample wsgi server'
 
 setup(
     name="kongfu-api",
     version=VERSION,
     author="smart_long",
     author_email="smart_long@outlook.com",
```

