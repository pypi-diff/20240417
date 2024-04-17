# Comparing `tmp/wzl-udi-9.3.7.tar.gz` & `tmp/wzl-udi-9.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wzl-udi-9.3.7.tar", last modified: Mon Mar 18 20:14:30 2024, max compression
+gzip compressed data, was "wzl-udi-9.3.8.tar", last modified: Tue Mar 19 06:59:38 2024, max compression
```

## Comparing `wzl-udi-9.3.7.tar` & `wzl-udi-9.3.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 20:14:29.981778 wzl-udi-9.3.7/
--rw-rw-rw-   0 root         (0) root         (0)     1135 2023-02-24 13:15:09.000000 wzl-udi-9.3.7/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       17 2023-03-25 10:32:29.000000 wzl-udi-9.3.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    12619 2024-03-18 20:14:29.980778 wzl-udi-9.3.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    11964 2024-03-18 20:14:25.000000 wzl-udi-9.3.7/README.md
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-03-25 10:32:29.000000 wzl-udi-9.3.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-18 20:14:29.981778 wzl-udi-9.3.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1308 2024-03-18 20:14:25.000000 wzl-udi-9.3.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 20:14:29.977778 wzl-udi-9.3.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 20:14:29.978778 wzl-udi-9.3.7/src/http/
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-02-24 13:15:09.000000 wzl-udi-9.3.7/src/http/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      304 2023-03-25 10:32:29.000000 wzl-udi-9.3.7/src/http/error.py
--rw-rw-rw-   0 root         (0) root         (0)    19678 2024-03-18 20:14:25.000000 wzl-udi-9.3.7/src/http/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 20:14:29.979778 wzl-udi-9.3.7/src/soil/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-18 20:14:25.000000 wzl-udi-9.3.7/src/soil/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22541 2024-03-14 12:30:23.000000 wzl-udi-9.3.7/src/soil/component.py
--rw-rw-rw-   0 root         (0) root         (0)     1171 2024-03-18 19:25:57.000000 wzl-udi-9.3.7/src/soil/datatype.py
--rw-rw-rw-   0 root         (0) root         (0)     5348 2024-03-14 12:30:23.000000 wzl-udi-9.3.7/src/soil/element.py
--rw-rw-rw-   0 root         (0) root         (0)     1980 2023-02-24 13:15:09.000000 wzl-udi-9.3.7/src/soil/error.py
--rw-rw-rw-   0 root         (0) root         (0)     4964 2024-01-10 08:08:44.000000 wzl-udi-9.3.7/src/soil/event.py
--rw-rw-rw-   0 root         (0) root         (0)    13376 2024-03-15 07:02:27.000000 wzl-udi-9.3.7/src/soil/function.py
--rw-rw-rw-   0 root         (0) root         (0)    11351 2024-03-18 19:25:57.000000 wzl-udi-9.3.7/src/soil/measurement.py
--rw-rw-rw-   0 root         (0) root         (0)     8876 2024-03-18 19:25:57.000000 wzl-udi-9.3.7/src/soil/parameter.py
--rw-rw-rw-   0 root         (0) root         (0)     2284 2024-01-17 07:10:29.000000 wzl-udi-9.3.7/src/soil/semantics.py
--rw-rw-rw-   0 root         (0) root         (0)    11033 2024-03-18 19:25:57.000000 wzl-udi-9.3.7/src/soil/stream.py
--rw-rw-rw-   0 root         (0) root         (0)    15769 2024-03-18 19:25:57.000000 wzl-udi-9.3.7/src/soil/variable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 20:14:29.980778 wzl-udi-9.3.7/src/utils/
--rw-rw-rw-   0 root         (0) root         (0)      366 2023-03-25 10:32:29.000000 wzl-udi-9.3.7/src/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      422 2024-01-17 07:10:29.000000 wzl-udi-9.3.7/src/utils/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1198 2024-03-14 12:30:23.000000 wzl-udi-9.3.7/src/utils/error.py
--rw-rw-rw-   0 root         (0) root         (0)     1802 2023-03-25 10:32:29.000000 wzl-udi-9.3.7/src/utils/logger.py
--rw-rw-rw-   0 root         (0) root         (0)      588 2024-03-14 12:30:23.000000 wzl-udi-9.3.7/src/utils/resources.py
--rw-rw-rw-   0 root         (0) root         (0)     1026 2023-02-24 13:15:09.000000 wzl-udi-9.3.7/src/utils/serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 20:14:29.980778 wzl-udi-9.3.7/wzl_udi.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12619 2024-03-18 20:14:29.000000 wzl-udi-9.3.7/wzl_udi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      674 2024-03-18 20:14:29.000000 wzl-udi-9.3.7/wzl_udi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-18 20:14:29.000000 wzl-udi-9.3.7/wzl_udi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-18 20:14:29.000000 wzl-udi-9.3.7/wzl_udi.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      104 2024-03-18 20:14:29.000000 wzl-udi-9.3.7/wzl_udi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2024-03-18 20:14:29.000000 wzl-udi-9.3.7/wzl_udi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 06:59:38.553998 wzl-udi-9.3.8/
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2023-02-24 13:15:09.000000 wzl-udi-9.3.8/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-03-25 10:32:29.000000 wzl-udi-9.3.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    12697 2024-03-19 06:59:38.553998 wzl-udi-9.3.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    12042 2024-03-19 06:59:33.000000 wzl-udi-9.3.8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-03-25 10:32:29.000000 wzl-udi-9.3.8/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-19 06:59:38.553998 wzl-udi-9.3.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1308 2024-03-19 06:59:33.000000 wzl-udi-9.3.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 06:59:38.549998 wzl-udi-9.3.8/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 06:59:38.550998 wzl-udi-9.3.8/src/http/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-02-24 13:15:09.000000 wzl-udi-9.3.8/src/http/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      304 2023-03-25 10:32:29.000000 wzl-udi-9.3.8/src/http/error.py
+-rw-rw-rw-   0 root         (0) root         (0)    19678 2024-03-18 20:14:25.000000 wzl-udi-9.3.8/src/http/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 06:59:38.551998 wzl-udi-9.3.8/src/soil/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-19 06:59:33.000000 wzl-udi-9.3.8/src/soil/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22541 2024-03-14 12:30:23.000000 wzl-udi-9.3.8/src/soil/component.py
+-rw-rw-rw-   0 root         (0) root         (0)     1175 2024-03-19 06:59:33.000000 wzl-udi-9.3.8/src/soil/datatype.py
+-rw-rw-rw-   0 root         (0) root         (0)     5348 2024-03-14 12:30:23.000000 wzl-udi-9.3.8/src/soil/element.py
+-rw-rw-rw-   0 root         (0) root         (0)     1980 2023-02-24 13:15:09.000000 wzl-udi-9.3.8/src/soil/error.py
+-rw-rw-rw-   0 root         (0) root         (0)     4964 2024-01-10 08:08:44.000000 wzl-udi-9.3.8/src/soil/event.py
+-rw-rw-rw-   0 root         (0) root         (0)    13376 2024-03-15 07:02:27.000000 wzl-udi-9.3.8/src/soil/function.py
+-rw-rw-rw-   0 root         (0) root         (0)    11351 2024-03-18 19:25:57.000000 wzl-udi-9.3.8/src/soil/measurement.py
+-rw-rw-rw-   0 root         (0) root         (0)     8876 2024-03-18 19:25:57.000000 wzl-udi-9.3.8/src/soil/parameter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2284 2024-01-17 07:10:29.000000 wzl-udi-9.3.8/src/soil/semantics.py
+-rw-rw-rw-   0 root         (0) root         (0)    11033 2024-03-18 19:25:57.000000 wzl-udi-9.3.8/src/soil/stream.py
+-rw-rw-rw-   0 root         (0) root         (0)    15769 2024-03-18 19:25:57.000000 wzl-udi-9.3.8/src/soil/variable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 06:59:38.552998 wzl-udi-9.3.8/src/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      366 2023-03-25 10:32:29.000000 wzl-udi-9.3.8/src/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      422 2024-01-17 07:10:29.000000 wzl-udi-9.3.8/src/utils/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1198 2024-03-14 12:30:23.000000 wzl-udi-9.3.8/src/utils/error.py
+-rw-rw-rw-   0 root         (0) root         (0)     1802 2023-03-25 10:32:29.000000 wzl-udi-9.3.8/src/utils/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      588 2024-03-14 12:30:23.000000 wzl-udi-9.3.8/src/utils/resources.py
+-rw-rw-rw-   0 root         (0) root         (0)     1026 2023-02-24 13:15:09.000000 wzl-udi-9.3.8/src/utils/serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 06:59:38.553998 wzl-udi-9.3.8/wzl_udi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12697 2024-03-19 06:59:38.000000 wzl-udi-9.3.8/wzl_udi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      674 2024-03-19 06:59:38.000000 wzl-udi-9.3.8/wzl_udi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-19 06:59:38.000000 wzl-udi-9.3.8/wzl_udi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-19 06:59:38.000000 wzl-udi-9.3.8/wzl_udi.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      104 2024-03-19 06:59:38.000000 wzl-udi-9.3.8/wzl_udi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2024-03-19 06:59:38.000000 wzl-udi-9.3.8/wzl_udi.egg-info/top_level.txt
```

### Comparing `wzl-udi-9.3.7/LICENSE` & `wzl-udi-9.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `wzl-udi-9.3.7/PKG-INFO` & `wzl-udi-9.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: wzl-udi
-Version: 9.3.7
+Version: 9.3.8
 Summary: Provides REST-server, publisher-interface and serializer for the Unified Device Interface in Python based on the SensOr Interfacing Language (SOIL).
 Home-page: https://git-ce.rwth-aachen.de/wzl-mq-public/soil/python
 Author: Matthias Bodenbenner
 Author-email: m.bodenbenner@wzl-mq.rwth-aachen.de
 Project-URL: Bug Tracker, https://git-ce.rwth-aachen.de/wzl-mq-public/soil/python/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Build](https://git-ce.rwth-aachen.de/wzl-mq-ms/forschung-lehre/lava/unified-device-interface/python/badges/master/pipeline.svg)](https://git-ce.rwth-aachen.de/wzl-mq-ms/forschung-lehre/lava/unified-device-interface/python/commits/master)
 
 # Python Unified Device Interface
-Current stable version: 9.3.7
+Current stable version: 9.3.8
 
 ## Installation
 1. Install the WZL-UDI package via pip
 ```
 pip install wzl-udi
 ```
 
@@ -68,14 +68,17 @@
 
 Funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) under Germany's Excellence Strategy – EXC-2023 Internet of Production – 390621612.
 
 Funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) under Project-ID 432233186 -- AIMS. 
 
 ## Recent changes
 
+**9.3.8** - 2024-03-19
+  - fixed semantic serialization of integer variables
+
 **9.3.7** - 2024-03-18
   - fixed serialization of semantics
 
 **9.3.6** - 2024-03-18
   - fixed serialization of semantic values
 
 **9.3.5** - 2024-03-18
```

### Comparing `wzl-udi-9.3.7/README.md` & `wzl-udi-9.3.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [![Build](https://git-ce.rwth-aachen.de/wzl-mq-ms/forschung-lehre/lava/unified-device-interface/python/badges/master/pipeline.svg)](https://git-ce.rwth-aachen.de/wzl-mq-ms/forschung-lehre/lava/unified-device-interface/python/commits/master)
 
 # Python Unified Device Interface
-Current stable version: 9.3.7
+Current stable version: 9.3.8
 
 ## Installation
 1. Install the WZL-UDI package via pip
 ```
 pip install wzl-udi
 ```
 
@@ -54,14 +54,17 @@
 
 Funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) under Germany's Excellence Strategy – EXC-2023 Internet of Production – 390621612.
 
 Funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) under Project-ID 432233186 -- AIMS. 
 
 ## Recent changes
 
+**9.3.8** - 2024-03-19
+  - fixed semantic serialization of integer variables
+
 **9.3.7** - 2024-03-18
   - fixed serialization of semantics
 
 **9.3.6** - 2024-03-18
   - fixed serialization of semantic values
 
 **9.3.5** - 2024-03-18
```

### Comparing `wzl-udi-9.3.7/setup.py` & `wzl-udi-9.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(name='wzl-udi',
-      version='9.3.7',
+      version='9.3.8',
       url='https://git-ce.rwth-aachen.de/wzl-mq-public/soil/python',
       project_urls={
           "Bug Tracker": "https://git-ce.rwth-aachen.de/wzl-mq-public/soil/python/-/issues",
       },
       author='Matthias Bodenbenner',
       author_email='m.bodenbenner@wzl-mq.rwth-aachen.de',
       description='Provides REST-server, publisher-interface and serializer for the Unified Device Interface in Python based on the SensOr Interfacing Language (SOIL).',
```

### Comparing `wzl-udi-9.3.7/src/http/server.py` & `wzl-udi-9.3.8/src/http/server.py`

 * *Files identical despite different names*

### Comparing `wzl-udi-9.3.7/src/soil/component.py` & `wzl-udi-9.3.8/src/soil/component.py`

 * *Files identical despite different names*

### Comparing `wzl-udi-9.3.7/src/soil/datatype.py` & `wzl-udi-9.3.8/src/soil/datatype.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 
     def to_string(self, legacy_mode: bool = False) -> str:
         if legacy_mode:
             return ["bool", "int", "double", "string", "time", "enum"][self.value]
         return ["boolean", "int", "float", "string", "time", "enum"][self.value]
 
     def to_semantic(self):
-        return [rdflib.XSD.boolean, rdflib.XSD.int, rdflib.XSD.float, rdflib.XSD.string, rdflib.XSD.dateTime, rdflib.XSD.string][self.value]
+        return [rdflib.XSD.boolean, rdflib.XSD.integer, rdflib.XSD.float, rdflib.XSD.string, rdflib.XSD.dateTime, rdflib.XSD.string][self.value]
```

### Comparing `wzl-udi-9.3.7/src/soil/element.py` & `wzl-udi-9.3.8/src/soil/element.py`

 * *Files identical despite different names*

### Comparing `wzl-udi-9.3.7/src/soil/error.py` & `wzl-udi-9.3.8/src/soil/error.py`

 * *Files identical despite different names*

### Comparing `wzl-udi-9.3.7/src/soil/event.py` & `wzl-udi-9.3.8/src/soil/event.py`

 * *Files identical despite different names*

### Comparing `wzl-udi-9.3.7/src/soil/function.py` & `wzl-udi-9.3.8/src/soil/function.py`

 * *Files identical despite different names*

### Comparing `wzl-udi-9.3.7/src/soil/measurement.py` & `wzl-udi-9.3.8/src/soil/measurement.py`

 * *Files identical despite different names*

### Comparing `wzl-udi-9.3.7/src/soil/parameter.py` & `wzl-udi-9.3.8/src/soil/parameter.py`

 * *Files identical despite different names*

### Comparing `wzl-udi-9.3.7/src/soil/semantics.py` & `wzl-udi-9.3.8/src/soil/semantics.py`

 * *Files identical despite different names*

### Comparing `wzl-udi-9.3.7/src/soil/stream.py` & `wzl-udi-9.3.8/src/soil/stream.py`

 * *Files identical despite different names*

### Comparing `wzl-udi-9.3.7/src/soil/variable.py` & `wzl-udi-9.3.8/src/soil/variable.py`

 * *Files identical despite different names*

### Comparing `wzl-udi-9.3.7/src/utils/error.py` & `wzl-udi-9.3.8/src/utils/error.py`

 * *Files identical despite different names*

### Comparing `wzl-udi-9.3.7/src/utils/logger.py` & `wzl-udi-9.3.8/src/utils/logger.py`

 * *Files identical despite different names*

### Comparing `wzl-udi-9.3.7/src/utils/resources.py` & `wzl-udi-9.3.8/src/utils/resources.py`

 * *Files identical despite different names*

### Comparing `wzl-udi-9.3.7/src/utils/serialize.py` & `wzl-udi-9.3.8/src/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `wzl-udi-9.3.7/wzl_udi.egg-info/PKG-INFO` & `wzl-udi-9.3.8/wzl_udi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: wzl-udi
-Version: 9.3.7
+Version: 9.3.8
 Summary: Provides REST-server, publisher-interface and serializer for the Unified Device Interface in Python based on the SensOr Interfacing Language (SOIL).
 Home-page: https://git-ce.rwth-aachen.de/wzl-mq-public/soil/python
 Author: Matthias Bodenbenner
 Author-email: m.bodenbenner@wzl-mq.rwth-aachen.de
 Project-URL: Bug Tracker, https://git-ce.rwth-aachen.de/wzl-mq-public/soil/python/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Build](https://git-ce.rwth-aachen.de/wzl-mq-ms/forschung-lehre/lava/unified-device-interface/python/badges/master/pipeline.svg)](https://git-ce.rwth-aachen.de/wzl-mq-ms/forschung-lehre/lava/unified-device-interface/python/commits/master)
 
 # Python Unified Device Interface
-Current stable version: 9.3.7
+Current stable version: 9.3.8
 
 ## Installation
 1. Install the WZL-UDI package via pip
 ```
 pip install wzl-udi
 ```
 
@@ -68,14 +68,17 @@
 
 Funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) under Germany's Excellence Strategy – EXC-2023 Internet of Production – 390621612.
 
 Funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) under Project-ID 432233186 -- AIMS. 
 
 ## Recent changes
 
+**9.3.8** - 2024-03-19
+  - fixed semantic serialization of integer variables
+
 **9.3.7** - 2024-03-18
   - fixed serialization of semantics
 
 **9.3.6** - 2024-03-18
   - fixed serialization of semantic values
 
 **9.3.5** - 2024-03-18
```

### Comparing `wzl-udi-9.3.7/wzl_udi.egg-info/SOURCES.txt` & `wzl-udi-9.3.8/wzl_udi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

