# Comparing `tmp/digitalhub-data-0.3.1.tar.gz` & `tmp/digitalhub_data-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub-data-0.3.1.tar", last modified: Wed Apr 10 08:28:35 2024, max compression
+gzip compressed data, was "digitalhub_data-0.3.2.tar", last modified: Wed Apr 17 12:31:38 2024, max compression
```

## Comparing `digitalhub-data-0.3.1.tar` & `digitalhub_data-0.3.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:35.151824 digitalhub-data-0.3.1/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)      557 2024-04-10 08:28:35.151824 digitalhub-data-0.3.1/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       81 2023-11-20 10:01:24.000000 digitalhub-data-0.3.1/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:35.147824 digitalhub-data-0.3.1/digitalhub_data/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      329 2024-04-10 08:00:27.000000 digitalhub-data-0.3.1/digitalhub_data/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:35.147824 digitalhub-data-0.3.1/digitalhub_data/entities/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:56.000000 digitalhub-data-0.3.1/digitalhub_data/entities/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:35.147824 digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:45.000000 digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3446 2024-04-10 08:00:27.000000 digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/builder.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6406 2024-04-10 08:00:27.000000 digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/crud.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:35.151824 digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/entity/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-03-04 14:42:21.000000 digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/entity/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6512 2024-04-10 08:26:04.000000 digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/entity/_base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      180 2024-03-15 13:13:54.000000 digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/entity/dataitem.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      142 2024-03-04 15:16:25.000000 digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/entity/iceberg.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3134 2024-03-06 16:32:11.000000 digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/entity/table.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1464 2024-03-15 12:04:30.000000 digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1093 2024-04-08 13:12:06.000000 digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1418 2024-04-08 13:12:04.000000 digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      863 2024-03-15 12:04:24.000000 digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:35.151824 digitalhub-data-0.3.1/digitalhub_data/entities/projects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-31 10:03:33.000000 digitalhub-data-0.3.1/digitalhub_data/entities/projects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6053 2024-04-10 08:00:27.000000 digitalhub-data-0.3.1/digitalhub_data/entities/projects/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6167 2024-04-10 08:26:04.000000 digitalhub-data-0.3.1/digitalhub_data/entities/projects/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      950 2024-02-15 10:15:41.000000 digitalhub-data-0.3.1/digitalhub_data/entities/projects/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      816 2024-03-07 13:44:22.000000 digitalhub-data-0.3.1/digitalhub_data/entities/registries.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:35.151824 digitalhub-data-0.3.1/digitalhub_data/entities/runs/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-22 14:51:32.000000 digitalhub-data-0.3.1/digitalhub_data/entities/runs/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub-data-0.3.1/digitalhub_data/entities/runs/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      407 2024-03-08 13:54:39.000000 digitalhub-data-0.3.1/digitalhub_data/entities/runs/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      351 2024-03-14 13:46:16.000000 digitalhub-data-0.3.1/digitalhub_data/entities/runs/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:35.151824 digitalhub-data-0.3.1/digitalhub_data/utils/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-29 10:07:05.000000 digitalhub-data-0.3.1/digitalhub_data/utils/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2440 2024-02-05 09:25:21.000000 digitalhub-data-0.3.1/digitalhub_data/utils/data_utils.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-10 08:28:35.151824 digitalhub-data-0.3.1/digitalhub_data.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)      557 2024-04-10 08:28:35.000000 digitalhub-data-0.3.1/digitalhub_data.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1305 2024-04-10 08:28:35.000000 digitalhub-data-0.3.1/digitalhub_data.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-04-10 08:28:35.000000 digitalhub-data-0.3.1/digitalhub_data.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-04-10 08:28:35.000000 digitalhub-data-0.3.1/digitalhub_data.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-04-10 08:28:35.000000 digitalhub-data-0.3.1/digitalhub_data.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1052 2024-04-09 13:57:43.000000 digitalhub-data-0.3.1/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-04-10 08:28:35.151824 digitalhub-data-0.3.1/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:31:38.837430 digitalhub_data-0.3.2/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)      557 2024-04-17 12:31:38.837430 digitalhub_data-0.3.2/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       81 2023-11-20 10:01:24.000000 digitalhub_data-0.3.2/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:31:38.833430 digitalhub_data-0.3.2/digitalhub_data/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      329 2024-04-16 14:28:24.000000 digitalhub_data-0.3.2/digitalhub_data/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:31:38.833430 digitalhub_data-0.3.2/digitalhub_data/entities/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:56.000000 digitalhub_data-0.3.2/digitalhub_data/entities/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:31:38.833430 digitalhub_data-0.3.2/digitalhub_data/entities/dataitems/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:45.000000 digitalhub_data-0.3.2/digitalhub_data/entities/dataitems/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3446 2024-04-17 12:30:02.000000 digitalhub_data-0.3.2/digitalhub_data/entities/dataitems/builder.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6406 2024-04-16 14:28:25.000000 digitalhub_data-0.3.2/digitalhub_data/entities/dataitems/crud.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:31:38.833430 digitalhub_data-0.3.2/digitalhub_data/entities/dataitems/entity/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-03-04 14:42:21.000000 digitalhub_data-0.3.2/digitalhub_data/entities/dataitems/entity/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6512 2024-04-17 12:30:02.000000 digitalhub_data-0.3.2/digitalhub_data/entities/dataitems/entity/_base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      180 2024-03-15 13:13:54.000000 digitalhub_data-0.3.2/digitalhub_data/entities/dataitems/entity/dataitem.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      142 2024-03-04 15:16:25.000000 digitalhub_data-0.3.2/digitalhub_data/entities/dataitems/entity/iceberg.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3134 2024-03-06 16:32:11.000000 digitalhub_data-0.3.2/digitalhub_data/entities/dataitems/entity/table.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1464 2024-04-17 12:30:02.000000 digitalhub_data-0.3.2/digitalhub_data/entities/dataitems/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1093 2024-04-08 13:12:06.000000 digitalhub_data-0.3.2/digitalhub_data/entities/dataitems/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1418 2024-04-08 13:12:04.000000 digitalhub_data-0.3.2/digitalhub_data/entities/dataitems/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      863 2024-03-15 12:04:24.000000 digitalhub_data-0.3.2/digitalhub_data/entities/dataitems/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:31:38.837430 digitalhub_data-0.3.2/digitalhub_data/entities/projects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-31 10:03:33.000000 digitalhub_data-0.3.2/digitalhub_data/entities/projects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6053 2024-04-16 14:28:24.000000 digitalhub_data-0.3.2/digitalhub_data/entities/projects/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6167 2024-04-17 12:30:02.000000 digitalhub_data-0.3.2/digitalhub_data/entities/projects/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      950 2024-02-15 10:15:41.000000 digitalhub_data-0.3.2/digitalhub_data/entities/projects/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      816 2024-04-17 12:30:02.000000 digitalhub_data-0.3.2/digitalhub_data/entities/registries.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:31:38.837430 digitalhub_data-0.3.2/digitalhub_data/entities/runs/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-22 14:51:32.000000 digitalhub_data-0.3.2/digitalhub_data/entities/runs/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub_data-0.3.2/digitalhub_data/entities/runs/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      407 2024-03-08 13:54:39.000000 digitalhub_data-0.3.2/digitalhub_data/entities/runs/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      351 2024-03-14 13:46:16.000000 digitalhub_data-0.3.2/digitalhub_data/entities/runs/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:31:38.837430 digitalhub_data-0.3.2/digitalhub_data/utils/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-29 10:07:05.000000 digitalhub_data-0.3.2/digitalhub_data/utils/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2440 2024-02-05 09:25:21.000000 digitalhub_data-0.3.2/digitalhub_data/utils/data_utils.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-17 12:31:38.837430 digitalhub_data-0.3.2/digitalhub_data.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)      557 2024-04-17 12:31:38.000000 digitalhub_data-0.3.2/digitalhub_data.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1305 2024-04-17 12:31:38.000000 digitalhub_data-0.3.2/digitalhub_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-04-17 12:31:38.000000 digitalhub_data-0.3.2/digitalhub_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-04-17 12:31:38.000000 digitalhub_data-0.3.2/digitalhub_data.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-04-17 12:31:38.000000 digitalhub_data-0.3.2/digitalhub_data.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1052 2024-04-17 12:30:02.000000 digitalhub_data-0.3.2/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-04-17 12:31:38.837430 digitalhub_data-0.3.2/setup.cfg
```

### Comparing `digitalhub-data-0.3.1/PKG-INFO` & `digitalhub_data-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-data
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 Keywords: data,dataops,kubernetes
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
```

### Comparing `digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/builder.py` & `digitalhub_data-0.3.2/digitalhub_data/entities/dataitems/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/crud.py` & `digitalhub_data-0.3.2/digitalhub_data/entities/dataitems/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/entity/_base.py` & `digitalhub_data-0.3.2/digitalhub_data/entities/dataitems/entity/_base.py`

 * *Files identical despite different names*

### Comparing `digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/entity/table.py` & `digitalhub_data-0.3.2/digitalhub_data/entities/dataitems/entity/table.py`

 * *Files identical despite different names*

### Comparing `digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/metadata.py` & `digitalhub_data-0.3.2/digitalhub_data/entities/dataitems/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/models.py` & `digitalhub_data-0.3.2/digitalhub_data/entities/dataitems/models.py`

 * *Files identical despite different names*

### Comparing `digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/spec.py` & `digitalhub_data-0.3.2/digitalhub_data/entities/dataitems/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub-data-0.3.1/digitalhub_data/entities/dataitems/status.py` & `digitalhub_data-0.3.2/digitalhub_data/entities/dataitems/status.py`

 * *Files identical despite different names*

### Comparing `digitalhub-data-0.3.1/digitalhub_data/entities/projects/crud.py` & `digitalhub_data-0.3.2/digitalhub_data/entities/projects/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub-data-0.3.1/digitalhub_data/entities/projects/entity.py` & `digitalhub_data-0.3.2/digitalhub_data/entities/projects/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub-data-0.3.1/digitalhub_data/entities/projects/spec.py` & `digitalhub_data-0.3.2/digitalhub_data/entities/projects/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub-data-0.3.1/digitalhub_data/entities/registries.py` & `digitalhub_data-0.3.2/digitalhub_data/entities/registries.py`

 * *Files identical despite different names*

### Comparing `digitalhub-data-0.3.1/digitalhub_data/utils/data_utils.py` & `digitalhub_data-0.3.2/digitalhub_data/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub-data-0.3.1/digitalhub_data.egg-info/PKG-INFO` & `digitalhub_data-0.3.2/digitalhub_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-data
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 Keywords: data,dataops,kubernetes
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
```

### Comparing `digitalhub-data-0.3.1/digitalhub_data.egg-info/SOURCES.txt` & `digitalhub_data-0.3.2/digitalhub_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digitalhub-data-0.3.1/pyproject.toml` & `digitalhub_data-0.3.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digitalhub-data"
-version = "0.3.1"
+version = "0.3.2"
 description = "Python SDK for DHCore"
 readme = "README.md"
 authors = [
     { name = "Fondazione Bruno Kessler", email = "dslab@fbk.eu" },
     { name = "Matteo Martini", email = "mmartini@fbk.eu" }
 ]
 license = { file = "LICENSE.txt" }
@@ -23,15 +23,15 @@
     "digitalhub-core~=0.3",
 ]
 
 [tool.setuptools.packages.find]
 exclude = ["modules*"]
 
 [tool.bumpver]
-current_version = "0.3.1"
+current_version = "0.3.2"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = false
 tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
```

