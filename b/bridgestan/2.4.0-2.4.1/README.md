# Comparing `tmp/bridgestan-2.4.0.tar.gz` & `tmp/bridgestan-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bridgestan-2.4.0.tar", last modified: Mon Mar 25 18:00:57 2024, max compression
+gzip compressed data, was "bridgestan-2.4.1.tar", last modified: Wed Apr 17 13:47:05 2024, max compression
```

## Comparing `bridgestan-2.4.0.tar` & `bridgestan-2.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:00:57.587292 bridgestan-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-25 18:00:57.587292 bridgestan-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-25 17:59:18.000000 bridgestan-2.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:00:57.587292 bridgestan-2.4.0/bridgestan/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-25 17:59:18.000000 bridgestan-2.4.0/bridgestan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-25 18:00:34.000000 bridgestan-2.4.0/bridgestan/__version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6313 2024-03-25 17:59:18.000000 bridgestan-2.4.0/bridgestan/compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-03-25 17:59:18.000000 bridgestan-2.4.0/bridgestan/download.py
--rw-r--r--   0 runner    (1001) docker     (127)    30962 2024-03-25 17:59:18.000000 bridgestan-2.4.0/bridgestan/model.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 17:59:18.000000 bridgestan-2.4.0/bridgestan/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-25 17:59:18.000000 bridgestan-2.4.0/bridgestan/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:00:57.587292 bridgestan-2.4.0/bridgestan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-25 18:00:57.000000 bridgestan-2.4.0/bridgestan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-25 18:00:57.000000 bridgestan-2.4.0/bridgestan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 18:00:57.000000 bridgestan-2.4.0/bridgestan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-25 18:00:57.000000 bridgestan-2.4.0/bridgestan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-25 18:00:57.000000 bridgestan-2.4.0/bridgestan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-25 17:59:18.000000 bridgestan-2.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 18:00:57.587292 bridgestan-2.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 18:00:57.587292 bridgestan-2.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-03-25 17:59:18.000000 bridgestan-2.4.0/test/test_compile.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-25 17:59:18.000000 bridgestan-2.4.0/test/test_download.py
--rw-r--r--   0 runner    (1001) docker     (127)    26317 2024-03-25 17:59:18.000000 bridgestan-2.4.0/test/test_stanmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:47:05.839395 bridgestan-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-17 13:47:05.839395 bridgestan-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-17 13:45:29.000000 bridgestan-2.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:47:05.839395 bridgestan-2.4.1/bridgestan/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-17 13:45:29.000000 bridgestan-2.4.1/bridgestan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-17 13:46:50.000000 bridgestan-2.4.1/bridgestan/__version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6313 2024-04-17 13:45:29.000000 bridgestan-2.4.1/bridgestan/compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-17 13:45:29.000000 bridgestan-2.4.1/bridgestan/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30962 2024-04-17 13:45:29.000000 bridgestan-2.4.1/bridgestan/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 13:45:29.000000 bridgestan-2.4.1/bridgestan/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-17 13:45:29.000000 bridgestan-2.4.1/bridgestan/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:47:05.839395 bridgestan-2.4.1/bridgestan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-17 13:47:05.000000 bridgestan-2.4.1/bridgestan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-17 13:47:05.000000 bridgestan-2.4.1/bridgestan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 13:47:05.000000 bridgestan-2.4.1/bridgestan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-17 13:47:05.000000 bridgestan-2.4.1/bridgestan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-17 13:47:05.000000 bridgestan-2.4.1/bridgestan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-17 13:45:29.000000 bridgestan-2.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 13:47:05.839395 bridgestan-2.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:47:05.839395 bridgestan-2.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-17 13:45:29.000000 bridgestan-2.4.1/test/test_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-17 13:45:29.000000 bridgestan-2.4.1/test/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26317 2024-04-17 13:45:29.000000 bridgestan-2.4.1/test/test_stanmodel.py
```

### Comparing `bridgestan-2.4.0/PKG-INFO` & `bridgestan-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bridgestan
-Version: 2.4.0
+Version: 2.4.1
 Summary: Access the methods of a Stan model in Python.
 Author-email: Brian Ward <bward@flatironinstitute.org>, Bob Carpenter <bcarpenter@flatironinstitute.org>, Edward Roualdes <eroualdes@csuchico.edu>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/roualdes/bridgestan
 Project-URL: Bug Tracker, https://github.com/roualdes/bridgestan/issues
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `bridgestan-2.4.0/bridgestan/compile.py` & `bridgestan-2.4.1/bridgestan/compile.py`

 * *Files identical despite different names*

### Comparing `bridgestan-2.4.0/bridgestan/download.py` & `bridgestan-2.4.1/bridgestan/download.py`

 * *Files identical despite different names*

### Comparing `bridgestan-2.4.0/bridgestan/model.py` & `bridgestan-2.4.1/bridgestan/model.py`

 * *Files identical despite different names*

### Comparing `bridgestan-2.4.0/bridgestan.egg-info/PKG-INFO` & `bridgestan-2.4.1/bridgestan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bridgestan
-Version: 2.4.0
+Version: 2.4.1
 Summary: Access the methods of a Stan model in Python.
 Author-email: Brian Ward <bward@flatironinstitute.org>, Bob Carpenter <bcarpenter@flatironinstitute.org>, Edward Roualdes <eroualdes@csuchico.edu>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/roualdes/bridgestan
 Project-URL: Bug Tracker, https://github.com/roualdes/bridgestan/issues
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `bridgestan-2.4.0/pyproject.toml` & `bridgestan-2.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bridgestan-2.4.0/test/test_compile.py` & `bridgestan-2.4.1/test/test_compile.py`

 * *Files identical despite different names*

### Comparing `bridgestan-2.4.0/test/test_stanmodel.py` & `bridgestan-2.4.1/test/test_stanmodel.py`

 * *Files identical despite different names*

