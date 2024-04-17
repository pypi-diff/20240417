# Comparing `tmp/sirtuin-1.0.0.tar.gz` & `tmp/sirtuin-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirtuin-1.0.0.tar", max compression
+gzip compressed data, was "sirtuin-1.0.1.tar", max compression
```

## Comparing `sirtuin-1.0.0.tar` & `sirtuin-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    10935 2024-03-04 00:27:45.021909 sirtuin-1.0.0/LICENSE
--rw-r--r--   0        0        0     7463 2024-03-04 00:07:28.373405 sirtuin-1.0.0/README.md
--rw-r--r--   0        0        0     2003 2024-03-04 00:20:57.306988 sirtuin-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2495 2024-03-04 00:31:29.331580 sirtuin-1.0.0/src/sirtuin/controllers/aws_cloudfront.py
--rw-r--r--   0        0        0     2515 2024-03-04 00:29:35.807810 sirtuin-1.0.0/src/sirtuin/controllers/aws_container.py
--rw-r--r--   0        0        0     1591 2024-03-04 00:29:44.080814 sirtuin-1.0.0/src/sirtuin/controllers/http_headers.py
--rw-r--r--   0        0        0     2000 2024-03-04 00:32:52.788762 sirtuin-1.0.0/src/sirtuin/main.py
--rw-r--r--   0        0        0      620 2024-03-04 00:27:19.578572 sirtuin-1.0.0/src/sirtuin/models/aws_cloudfront.py
--rw-r--r--   0        0        0      734 2024-03-04 00:27:19.578571 sirtuin-1.0.0/src/sirtuin/models/aws_container.py
--rw-r--r--   0        0        0      134 2024-03-04 00:04:14.580148 sirtuin-1.0.0/src/sirtuin/models/aws_instances.py
--rw-r--r--   0        0        0      282 2024-03-04 00:04:14.580192 sirtuin-1.0.0/src/sirtuin/models/aws_regions.py
--rw-r--r--   0        0        0      832 2024-03-04 00:23:13.185138 sirtuin-1.0.0/src/sirtuin/models/base_models.py
--rw-r--r--   0        0        0      867 2024-03-04 00:42:52.964401 sirtuin-1.0.0/src/sirtuin/models/http_headers.py
--rw-r--r--   0        0        0      244 2024-03-04 00:04:14.581883 sirtuin-1.0.0/src/sirtuin/utils/cleaners.py
--rw-r--r--   0        0        0      132 2024-03-04 00:04:14.581930 sirtuin-1.0.0/src/sirtuin/utils/constants.py
--rw-r--r--   0        0        0     2470 2024-03-04 00:27:19.578616 sirtuin-1.0.0/src/sirtuin/utils/decorators.py
--rw-r--r--   0        0        0     1363 2024-03-04 00:04:14.582081 sirtuin-1.0.0/src/sirtuin/utils/dumpers.py
--rw-r--r--   0        0        0      406 2024-03-04 00:34:27.565385 sirtuin-1.0.0/src/sirtuin/utils/filepaths.py
--rw-r--r--   0        0        0     1309 2024-03-04 00:34:29.971524 sirtuin-1.0.0/src/sirtuin/utils/loaders.py
--rw-r--r--   0        0        0     8035 1970-01-01 00:00:00.000000 sirtuin-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    10935 2024-03-04 00:27:45.021909 sirtuin-1.0.1/LICENSE
+-rw-r--r--   0        0        0     7463 2024-03-04 00:07:28.373405 sirtuin-1.0.1/README.md
+-rw-r--r--   0        0        0     2033 2024-04-17 03:00:44.037390 sirtuin-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2495 2024-03-04 00:31:29.331580 sirtuin-1.0.1/src/sirtuin/controllers/aws_cloudfront.py
+-rw-r--r--   0        0        0     2515 2024-03-04 00:29:35.807810 sirtuin-1.0.1/src/sirtuin/controllers/aws_container.py
+-rw-r--r--   0        0        0     1591 2024-03-04 00:29:44.080814 sirtuin-1.0.1/src/sirtuin/controllers/http_headers.py
+-rw-r--r--   0        0        0     2000 2024-03-04 00:32:52.788762 sirtuin-1.0.1/src/sirtuin/main.py
+-rw-r--r--   0        0        0      620 2024-03-04 00:27:19.578572 sirtuin-1.0.1/src/sirtuin/models/aws_cloudfront.py
+-rw-r--r--   0        0        0      734 2024-03-04 00:27:19.578571 sirtuin-1.0.1/src/sirtuin/models/aws_container.py
+-rw-r--r--   0        0        0      134 2024-03-04 00:04:14.580148 sirtuin-1.0.1/src/sirtuin/models/aws_instances.py
+-rw-r--r--   0        0        0      282 2024-03-04 00:04:14.580192 sirtuin-1.0.1/src/sirtuin/models/aws_regions.py
+-rw-r--r--   0        0        0      832 2024-03-04 00:23:13.185138 sirtuin-1.0.1/src/sirtuin/models/base_models.py
+-rw-r--r--   0        0        0      867 2024-03-04 00:42:52.964401 sirtuin-1.0.1/src/sirtuin/models/http_headers.py
+-rw-r--r--   0        0        0      244 2024-03-04 00:04:14.581883 sirtuin-1.0.1/src/sirtuin/utils/cleaners.py
+-rw-r--r--   0        0        0      132 2024-03-04 00:04:14.581930 sirtuin-1.0.1/src/sirtuin/utils/constants.py
+-rw-r--r--   0        0        0     2470 2024-03-04 00:27:19.578616 sirtuin-1.0.1/src/sirtuin/utils/decorators.py
+-rw-r--r--   0        0        0     1363 2024-03-04 00:04:14.582081 sirtuin-1.0.1/src/sirtuin/utils/dumpers.py
+-rw-r--r--   0        0        0      406 2024-03-04 00:34:27.565385 sirtuin-1.0.1/src/sirtuin/utils/filepaths.py
+-rw-r--r--   0        0        0     1309 2024-03-04 00:34:29.971524 sirtuin-1.0.1/src/sirtuin/utils/loaders.py
+-rw-r--r--   0        0        0     8040 1970-01-01 00:00:00.000000 sirtuin-1.0.1/PKG-INFO
```

### Comparing `sirtuin-1.0.0/LICENSE` & `sirtuin-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sirtuin-1.0.0/README.md` & `sirtuin-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `sirtuin-1.0.0/pyproject.toml` & `sirtuin-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -34,31 +34,31 @@
 warn_unused_ignores = true
 
 [tool.poetry]
 authors = ["Meryll Dindin <merylldin@gmail.com>"]
 description = "AWS routines for Python projects"
 name = "sirtuin"
 readme = "README.md"
-version = "1.0.0"
+version = "1.0.1"
 
 [tool.poetry.dependencies]
 pydantic = "^2.6.3"
 python = ">=3.10,<3.13"
 pyyaml = "^6.0"
 tomli = "^2.0"
-typer = {extras = ["all"], version = "^0.9"}
+typer = { extras = ["all"], version = "^0.12.0" }
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.0.0"
 mypy = "^1.0"
 pytest = "^8.1.0"
-pytest-cov = "^4.0"
+pytest-cov = "^5.0.0"
 ruff = "^0.3.0"
 toml-sort = "^0.23"
 
 [tool.poetry.group.types]
 optional = true
 
 [tool.poetry.group.types.dependencies]
@@ -80,8 +80,14 @@
 [tool.ruff.lint]
 dummy-variable-rgx = "_+$|(_[a-zA-Z0-9_]*[a-zA-Z0-9]+?$)|dummy|^ignored_|^unused_"
 ignore = ["D100", "D101", "E501"]
 ignore-init-module-imports = true
 select = ["E", "F", "I001", "W"]
 
 [tool.ruff.lint.isort]
-section-order = ["first-party", "future", "local-folder", "standard-library", "third-party"]
+section-order = [
+    "first-party",
+    "future",
+    "local-folder",
+    "standard-library",
+    "third-party",
+]
```

### Comparing `sirtuin-1.0.0/src/sirtuin/controllers/aws_cloudfront.py` & `sirtuin-1.0.1/src/sirtuin/controllers/aws_cloudfront.py`

 * *Files identical despite different names*

### Comparing `sirtuin-1.0.0/src/sirtuin/controllers/aws_container.py` & `sirtuin-1.0.1/src/sirtuin/controllers/aws_container.py`

 * *Files identical despite different names*

### Comparing `sirtuin-1.0.0/src/sirtuin/controllers/http_headers.py` & `sirtuin-1.0.1/src/sirtuin/controllers/http_headers.py`

 * *Files identical despite different names*

### Comparing `sirtuin-1.0.0/src/sirtuin/main.py` & `sirtuin-1.0.1/src/sirtuin/main.py`

 * *Files identical despite different names*

### Comparing `sirtuin-1.0.0/src/sirtuin/models/aws_cloudfront.py` & `sirtuin-1.0.1/src/sirtuin/models/aws_cloudfront.py`

 * *Files identical despite different names*

### Comparing `sirtuin-1.0.0/src/sirtuin/models/aws_container.py` & `sirtuin-1.0.1/src/sirtuin/models/aws_container.py`

 * *Files identical despite different names*

### Comparing `sirtuin-1.0.0/src/sirtuin/models/base_models.py` & `sirtuin-1.0.1/src/sirtuin/models/base_models.py`

 * *Files identical despite different names*

### Comparing `sirtuin-1.0.0/src/sirtuin/models/http_headers.py` & `sirtuin-1.0.1/src/sirtuin/models/http_headers.py`

 * *Files identical despite different names*

### Comparing `sirtuin-1.0.0/src/sirtuin/utils/decorators.py` & `sirtuin-1.0.1/src/sirtuin/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `sirtuin-1.0.0/src/sirtuin/utils/dumpers.py` & `sirtuin-1.0.1/src/sirtuin/utils/dumpers.py`

 * *Files identical despite different names*

### Comparing `sirtuin-1.0.0/src/sirtuin/utils/loaders.py` & `sirtuin-1.0.1/src/sirtuin/utils/loaders.py`

 * *Files identical despite different names*

### Comparing `sirtuin-1.0.0/PKG-INFO` & `sirtuin-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: sirtuin
-Version: 1.0.0
+Version: 1.0.1
 Summary: AWS routines for Python projects
 Author: Meryll Dindin
 Author-email: merylldin@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pydantic (>=2.6.3,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: tomli (>=2.0,<3.0)
-Requires-Dist: typer[all] (>=0.9,<0.10)
+Requires-Dist: typer[all] (>=0.12.0,<0.13.0)
 Description-Content-Type: text/markdown
 
 <a href="https://merylldindin.com">
   <img src="https://cdn.merylldindin.com/github/sirtuin.webp" alt="sirtuin" width="100%">
 </a>
 
 <div align="center">
```

