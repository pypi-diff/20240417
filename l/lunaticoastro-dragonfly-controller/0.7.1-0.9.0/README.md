# Comparing `tmp/lunaticoastro_dragonfly_controller-0.7.1.tar.gz` & `tmp/lunaticoastro_dragonfly_controller-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lunaticoastro_dragonfly_controller-0.7.1.tar", max compression
+gzip compressed data, was "lunaticoastro_dragonfly_controller-0.9.0.tar", max compression
```

## Comparing `lunaticoastro_dragonfly_controller-0.7.1.tar` & `lunaticoastro_dragonfly_controller-0.9.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11357 2024-04-16 12:22:41.276066 lunaticoastro_dragonfly_controller-0.7.1/LICENSE
--rw-r--r--   0        0        0     2832 2024-04-16 12:22:41.276066 lunaticoastro_dragonfly_controller-0.7.1/README.md
--rw-r--r--   0        0        0     8644 2024-04-16 12:22:41.276066 lunaticoastro_dragonfly_controller-0.7.1/dragonfly_dome/controller.py
--rw-r--r--   0        0        0     1377 2024-04-16 12:22:41.276066 lunaticoastro_dragonfly_controller-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     3430 1970-01-01 00:00:00.000000 lunaticoastro_dragonfly_controller-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-16 15:22:11.077518 lunaticoastro_dragonfly_controller-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2832 2024-04-16 15:22:11.077518 lunaticoastro_dragonfly_controller-0.9.0/README.md
+-rw-r--r--   0        0        0     8644 2024-04-16 15:22:11.077518 lunaticoastro_dragonfly_controller-0.9.0/dragonfly_dome/controller.py
+-rw-r--r--   0        0        0     1377 2024-04-16 15:22:11.077518 lunaticoastro_dragonfly_controller-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3430 1970-01-01 00:00:00.000000 lunaticoastro_dragonfly_controller-0.9.0/PKG-INFO
```

### Comparing `lunaticoastro_dragonfly_controller-0.7.1/LICENSE` & `lunaticoastro_dragonfly_controller-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lunaticoastro_dragonfly_controller-0.7.1/README.md` & `lunaticoastro_dragonfly_controller-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `lunaticoastro_dragonfly_controller-0.7.1/dragonfly_dome/controller.py` & `lunaticoastro_dragonfly_controller-0.9.0/dragonfly_dome/controller.py`

 * *Files identical despite different names*

### Comparing `lunaticoastro_dragonfly_controller-0.7.1/pyproject.toml` & `lunaticoastro_dragonfly_controller-0.9.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lunaticoastro-dragonfly-controller"
-version = "0.7.1"
+version = "0.9.0"
 description = "Python Lib to control lunaticoastro dragonfly"
 readme = "README.md"
 authors = ["Robert Bradley <robbrad182@gmail.com>"]
 packages = [
     { include = "dragonfly_dome", from = "." },
 ]
```

### Comparing `lunaticoastro_dragonfly_controller-0.7.1/PKG-INFO` & `lunaticoastro_dragonfly_controller-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lunaticoastro-dragonfly-controller
-Version: 0.7.1
+Version: 0.9.0
 Summary: Python Lib to control lunaticoastro dragonfly
 Author: Robert Bradley
 Author-email: robbrad182@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

