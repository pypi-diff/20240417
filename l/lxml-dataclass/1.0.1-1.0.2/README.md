# Comparing `tmp/lxml-dataclass-1.0.1.tar.gz` & `tmp/lxml_dataclass-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lxml-dataclass-1.0.1.tar", last modified: Wed Mar 13 01:15:10 2024, max compression
+gzip compressed data, was "lxml_dataclass-1.0.2.tar", last modified: Wed Apr 17 12:43:32 2024, max compression
```

## Comparing `lxml-dataclass-1.0.1.tar` & `lxml_dataclass-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 thonder5  (1000) thonder5  (1000)        0 2024-03-13 01:15:10.060186 lxml-dataclass-1.0.1/
--rw-r--r--   0 thonder5  (1000) thonder5  (1000)     1081 2024-01-15 02:57:21.000000 lxml-dataclass-1.0.1/LICENSE
--rw-r--r--   0 thonder5  (1000) thonder5  (1000)     7792 2024-03-13 01:15:10.060186 lxml-dataclass-1.0.1/PKG-INFO
--rw-r--r--   0 thonder5  (1000) thonder5  (1000)     5868 2024-01-15 04:40:53.000000 lxml-dataclass-1.0.1/README.md
--rw-r--r--   0 thonder5  (1000) thonder5  (1000)     1084 2024-03-13 01:12:11.000000 lxml-dataclass-1.0.1/pyproject.toml
--rw-r--r--   0 thonder5  (1000) thonder5  (1000)       38 2024-03-13 01:15:10.060186 lxml-dataclass-1.0.1/setup.cfg
--rw-r--r--   0 thonder5  (1000) thonder5  (1000)       51 2024-03-13 01:07:44.000000 lxml-dataclass-1.0.1/setup.py
-drwxr-xr-x   0 thonder5  (1000) thonder5  (1000)        0 2024-03-13 01:15:10.040186 lxml-dataclass-1.0.1/src/
-drwxr-xr-x   0 thonder5  (1000) thonder5  (1000)        0 2024-03-13 01:15:10.050186 lxml-dataclass-1.0.1/src/lxml_dataclass/
--rw-r--r--   0 thonder5  (1000) thonder5  (1000)      123 2024-01-15 05:01:43.000000 lxml-dataclass-1.0.1/src/lxml_dataclass/__init__.py
--rw-r--r--   0 thonder5  (1000) thonder5  (1000)    21313 2024-03-13 01:07:11.000000 lxml-dataclass-1.0.1/src/lxml_dataclass/element.py
-drwxr-xr-x   0 thonder5  (1000) thonder5  (1000)        0 2024-03-13 01:15:10.050186 lxml-dataclass-1.0.1/src/lxml_dataclass.egg-info/
--rw-r--r--   0 thonder5  (1000) thonder5  (1000)     7792 2024-03-13 01:15:10.000000 lxml-dataclass-1.0.1/src/lxml_dataclass.egg-info/PKG-INFO
--rw-r--r--   0 thonder5  (1000) thonder5  (1000)      311 2024-03-13 01:15:10.000000 lxml-dataclass-1.0.1/src/lxml_dataclass.egg-info/SOURCES.txt
--rw-r--r--   0 thonder5  (1000) thonder5  (1000)        1 2024-03-13 01:15:10.000000 lxml-dataclass-1.0.1/src/lxml_dataclass.egg-info/dependency_links.txt
--rw-r--r--   0 thonder5  (1000) thonder5  (1000)       41 2024-03-13 01:15:10.000000 lxml-dataclass-1.0.1/src/lxml_dataclass.egg-info/requires.txt
--rw-r--r--   0 thonder5  (1000) thonder5  (1000)       15 2024-03-13 01:15:10.000000 lxml-dataclass-1.0.1/src/lxml_dataclass.egg-info/top_level.txt
+drwxr-xr-x   0 thonder   (1000) thonder   (1000)        0 2024-04-17 12:43:32.721923 lxml_dataclass-1.0.2/
+-rw-r--r--   0 thonder   (1000) thonder   (1000)     1081 2024-04-16 01:38:06.000000 lxml_dataclass-1.0.2/LICENSE
+-rw-r--r--   0 thonder   (1000) thonder   (1000)     7795 2024-04-17 12:43:32.711923 lxml_dataclass-1.0.2/PKG-INFO
+-rw-r--r--   0 thonder   (1000) thonder   (1000)     5868 2024-04-16 01:38:06.000000 lxml_dataclass-1.0.2/README.md
+-rw-r--r--   0 thonder   (1000) thonder   (1000)      758 2024-04-17 12:41:46.000000 lxml_dataclass-1.0.2/pyproject.toml
+-rw-r--r--   0 thonder   (1000) thonder   (1000)       38 2024-04-17 12:43:32.721923 lxml_dataclass-1.0.2/setup.cfg
+-rw-r--r--   0 thonder   (1000) thonder   (1000)       51 2024-04-17 12:16:31.000000 lxml_dataclass-1.0.2/setup.py
+drwxr-xr-x   0 thonder   (1000) thonder   (1000)        0 2024-04-17 12:43:32.661923 lxml_dataclass-1.0.2/src/
+drwxr-xr-x   0 thonder   (1000) thonder   (1000)        0 2024-04-17 12:43:32.681923 lxml_dataclass-1.0.2/src/lxml_dataclass/
+-rw-r--r--   0 thonder   (1000) thonder   (1000)      123 2024-04-16 01:38:06.000000 lxml_dataclass-1.0.2/src/lxml_dataclass/__init__.py
+-rw-r--r--   0 thonder   (1000) thonder   (1000)    21313 2024-04-17 12:19:07.000000 lxml_dataclass-1.0.2/src/lxml_dataclass/element.py
+drwxr-xr-x   0 thonder   (1000) thonder   (1000)        0 2024-04-17 12:43:32.711923 lxml_dataclass-1.0.2/src/lxml_dataclass.egg-info/
+-rw-r--r--   0 thonder   (1000) thonder   (1000)     7795 2024-04-17 12:43:32.000000 lxml_dataclass-1.0.2/src/lxml_dataclass.egg-info/PKG-INFO
+-rw-r--r--   0 thonder   (1000) thonder   (1000)      311 2024-04-17 12:43:32.000000 lxml_dataclass-1.0.2/src/lxml_dataclass.egg-info/SOURCES.txt
+-rw-r--r--   0 thonder   (1000) thonder   (1000)        1 2024-04-17 12:43:32.000000 lxml_dataclass-1.0.2/src/lxml_dataclass.egg-info/dependency_links.txt
+-rw-r--r--   0 thonder   (1000) thonder   (1000)       44 2024-04-17 12:43:32.000000 lxml_dataclass-1.0.2/src/lxml_dataclass.egg-info/requires.txt
+-rw-r--r--   0 thonder   (1000) thonder   (1000)       15 2024-04-17 12:43:32.000000 lxml_dataclass-1.0.2/src/lxml_dataclass.egg-info/top_level.txt
```

### Comparing `lxml-dataclass-1.0.1/LICENSE` & `lxml_dataclass-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lxml-dataclass-1.0.1/PKG-INFO` & `lxml_dataclass-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lxml-dataclass
-Version: 1.0.1
+Version: 1.0.2
 Summary: Create LXML Elements as dataclasses representations
 Author-email: Sebastian Salinas <seba.salinas.delrio@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Sebastian Salinas Del Rio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,15 +28,15 @@
 Keywords: lxml,dataclass,xml
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: lxml==4.9.4
+Requires-Dist: lxml<6,>=5.2.1
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
 # LXML-DATACLASS
```

### Comparing `lxml-dataclass-1.0.1/README.md` & `lxml_dataclass-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `lxml-dataclass-1.0.1/src/lxml_dataclass/element.py` & `lxml_dataclass-1.0.2/src/lxml_dataclass/element.py`

 * *Files identical despite different names*

### Comparing `lxml-dataclass-1.0.1/src/lxml_dataclass.egg-info/PKG-INFO` & `lxml_dataclass-1.0.2/src/lxml_dataclass.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lxml-dataclass
-Version: 1.0.1
+Version: 1.0.2
 Summary: Create LXML Elements as dataclasses representations
 Author-email: Sebastian Salinas <seba.salinas.delrio@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Sebastian Salinas Del Rio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,15 +28,15 @@
 Keywords: lxml,dataclass,xml
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: lxml==4.9.4
+Requires-Dist: lxml<6,>=5.2.1
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
 # LXML-DATACLASS
```

