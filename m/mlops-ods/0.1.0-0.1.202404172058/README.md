# Comparing `tmp/mlops_ods-0.1.0.tar.gz` & `tmp/mlops_ods-0.1.202404172058.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlops_ods-0.1.0.tar", max compression
+gzip compressed data, was "mlops_ods-0.1.202404172058.tar", max compression
```

## Comparing `mlops_ods-0.1.0.tar` & `mlops_ods-0.1.202404172058.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      613 2024-04-17 20:35:07.132622 mlops_ods-0.1.0/README.md
--rw-r--r--   0        0        0      692 2024-04-17 20:35:07.136622 mlops_ods-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-17 20:35:07.136622 mlops_ods-0.1.0/src/mlops_ods/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 20:35:07.136622 mlops_ods-0.1.0/src/mlops_ods/app/__init__.py
--rw-r--r--   0        0        0       50 2024-04-17 20:35:07.136622 mlops_ods-0.1.0/src/mlops_ods/app/example.py
--rw-r--r--   0        0        0  9730652 2024-04-17 20:35:07.164622 mlops_ods-0.1.0/src/mlops_ods/notebooks/eda.ipynb
--rw-r--r--   0        0        0     1276 1970-01-01 00:00:00.000000 mlops_ods-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      613 2024-04-17 20:58:11.638004 mlops_ods-0.1.202404172058/README.md
+-rw-r--r--   0        0        0      703 2024-04-17 20:58:26.082066 mlops_ods-0.1.202404172058/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-17 20:58:11.642004 mlops_ods-0.1.202404172058/src/mlops_ods/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 20:58:11.642004 mlops_ods-0.1.202404172058/src/mlops_ods/app/__init__.py
+-rw-r--r--   0        0        0       50 2024-04-17 20:58:11.642004 mlops_ods-0.1.202404172058/src/mlops_ods/app/example.py
+-rw-r--r--   0        0        0  9730652 2024-04-17 20:58:11.670004 mlops_ods-0.1.202404172058/src/mlops_ods/notebooks/eda.ipynb
+-rw-r--r--   0        0        0     1287 1970-01-01 00:00:00.000000 mlops_ods-0.1.202404172058/PKG-INFO
```

### Comparing `mlops_ods-0.1.0/README.md` & `mlops_ods-0.1.202404172058/README.md`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.0/pyproject.toml` & `mlops_ods-0.1.202404172058/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlops_ods"
-version = "0.1.0"
+version = "0.1.202404172058"
 description = ""
 authors = ["Iuliia Fokina"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pandas = "^2.2.2"
```

### Comparing `mlops_ods-0.1.0/src/mlops_ods/notebooks/eda.ipynb` & `mlops_ods-0.1.202404172058/src/mlops_ods/notebooks/eda.ipynb`

 * *Files identical despite different names*

### Comparing `mlops_ods-0.1.0/PKG-INFO` & `mlops_ods-0.1.202404172058/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlops_ods
-Version: 0.1.0
+Version: 0.1.202404172058
 Summary: 
 Author: Iuliia Fokina
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

