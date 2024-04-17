# Comparing `tmp/pysanet-0.0.8.tar.gz` & `tmp/pysanet-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysanet-0.0.8.tar", max compression
+gzip compressed data, was "pysanet-0.0.9.tar", max compression
```

## Comparing `pysanet-0.0.8.tar` & `pysanet-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1477 2023-11-22 11:27:36.695073 pysanet-0.0.8/LICENSE
--rw-r--r--   0        0        0        0 2023-10-21 16:49:57.478474 pysanet-0.0.8/README.md
--rw-r--r--   0        0        0     3361 2023-11-22 11:26:13.469578 pysanet-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       22 2023-11-22 11:26:13.470023 pysanet-0.0.8/src/pysanet/__init__.py
--rw-r--r--   0        0        0      317 2023-10-27 11:13:48.077074 pysanet-0.0.8/src/pysanet/__main__.py
--rw-r--r--   0        0        0     4801 2023-11-03 11:18:37.796121 pysanet-0.0.8/src/pysanet/api.py
--rw-r--r--   0        0        0        0 2023-10-27 11:11:34.613115 pysanet-0.0.8/src/pysanet/cli/__init__.py
--rw-r--r--   0        0        0     1667 2023-10-28 15:30:37.350979 pysanet-0.0.8/src/pysanet/cli/commands.py
--rw-r--r--   0        0        0     1556 2023-10-28 15:37:49.375806 pysanet-0.0.8/src/pysanet/cli/utils.py
--rw-r--r--   0        0        0     1115 2023-11-22 11:25:55.130326 pysanet-0.0.8/src/pysanet/core.py
--rw-r--r--   0        0        0      238 2023-10-27 15:48:28.923755 pysanet-0.0.8/src/pysanet/enums.py
--rw-r--r--   0        0        0      271 2023-10-27 11:49:35.967288 pysanet-0.0.8/src/pysanet/exceptions.py
--rw-r--r--   0        0        0        0 2023-10-28 15:41:30.867248 pysanet-0.0.8/src/pysanet/schemas/__init__.py
--rw-r--r--   0        0        0     5740 2023-11-06 10:59:38.366207 pysanet-0.0.8/src/pysanet/schemas/models.py
--rw-r--r--   0        0        0     1737 2023-10-28 15:42:28.214882 pysanet-0.0.8/src/pysanet/schemas/outs.py
--rw-r--r--   0        0        0      751 2023-10-27 16:53:20.753745 pysanet-0.0.8/src/pysanet/settings.py
--rw-r--r--   0        0        0     1368 1970-01-01 00:00:00.000000 pysanet-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1477 2023-11-22 11:27:36.695073 pysanet-0.0.9/LICENSE
+-rw-r--r--   0        0        0        0 2023-10-21 16:49:57.478474 pysanet-0.0.9/README.md
+-rw-r--r--   0        0        0     3361 2023-11-22 11:28:58.996731 pysanet-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-11-22 11:28:58.997035 pysanet-0.0.9/src/pysanet/__init__.py
+-rw-r--r--   0        0        0      317 2023-10-27 11:13:48.077074 pysanet-0.0.9/src/pysanet/__main__.py
+-rw-r--r--   0        0        0     4801 2023-11-03 11:18:37.796121 pysanet-0.0.9/src/pysanet/api.py
+-rw-r--r--   0        0        0        0 2023-10-27 11:11:34.613115 pysanet-0.0.9/src/pysanet/cli/__init__.py
+-rw-r--r--   0        0        0     1667 2023-10-28 15:30:37.350979 pysanet-0.0.9/src/pysanet/cli/commands.py
+-rw-r--r--   0        0        0     1556 2023-10-28 15:37:49.375806 pysanet-0.0.9/src/pysanet/cli/utils.py
+-rw-r--r--   0        0        0     1115 2023-11-22 11:25:55.130326 pysanet-0.0.9/src/pysanet/core.py
+-rw-r--r--   0        0        0      238 2023-10-27 15:48:28.923755 pysanet-0.0.9/src/pysanet/enums.py
+-rw-r--r--   0        0        0      271 2023-10-27 11:49:35.967288 pysanet-0.0.9/src/pysanet/exceptions.py
+-rw-r--r--   0        0        0        0 2023-10-28 15:41:30.867248 pysanet-0.0.9/src/pysanet/schemas/__init__.py
+-rw-r--r--   0        0        0     5740 2023-11-06 10:59:38.366207 pysanet-0.0.9/src/pysanet/schemas/models.py
+-rw-r--r--   0        0        0     1737 2023-10-28 15:42:28.214882 pysanet-0.0.9/src/pysanet/schemas/outs.py
+-rw-r--r--   0        0        0      751 2023-10-27 16:53:20.753745 pysanet-0.0.9/src/pysanet/settings.py
+-rw-r--r--   0        0        0     1368 1970-01-01 00:00:00.000000 pysanet-0.0.9/PKG-INFO
```

### Comparing `pysanet-0.0.8/LICENSE` & `pysanet-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pysanet-0.0.8/pyproject.toml` & `pysanet-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysanet"
-version = "0.0.8"
+version = "0.0.9"
 description = ""
 authors = ["Simone Dalla <simodalla@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "pysanet", from = "src" }]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Programming Language :: Python",
@@ -56,15 +56,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.bumpver]
-current_version = "0.0.8"
+current_version = "0.0.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version v{old_version} -> v{new_version}"
 tag_message = "v{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = false
```

### Comparing `pysanet-0.0.8/src/pysanet/api.py` & `pysanet-0.0.9/src/pysanet/api.py`

 * *Files identical despite different names*

### Comparing `pysanet-0.0.8/src/pysanet/cli/commands.py` & `pysanet-0.0.9/src/pysanet/cli/commands.py`

 * *Files identical despite different names*

### Comparing `pysanet-0.0.8/src/pysanet/cli/utils.py` & `pysanet-0.0.9/src/pysanet/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pysanet-0.0.8/src/pysanet/core.py` & `pysanet-0.0.9/src/pysanet/core.py`

 * *Files identical despite different names*

### Comparing `pysanet-0.0.8/src/pysanet/schemas/models.py` & `pysanet-0.0.9/src/pysanet/schemas/models.py`

 * *Files identical despite different names*

### Comparing `pysanet-0.0.8/src/pysanet/schemas/outs.py` & `pysanet-0.0.9/src/pysanet/schemas/outs.py`

 * *Files identical despite different names*

### Comparing `pysanet-0.0.8/src/pysanet/settings.py` & `pysanet-0.0.9/src/pysanet/settings.py`

 * *Files identical despite different names*

### Comparing `pysanet-0.0.8/PKG-INFO` & `pysanet-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysanet
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Author: Simone Dalla
 Author-email: simodalla@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
```

