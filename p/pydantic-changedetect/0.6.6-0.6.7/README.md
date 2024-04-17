# Comparing `tmp/pydantic_changedetect-0.6.6.tar.gz` & `tmp/pydantic_changedetect-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_changedetect-0.6.6.tar", max compression
+gzip compressed data, was "pydantic_changedetect-0.6.7.tar", max compression
```

## Comparing `pydantic_changedetect-0.6.6.tar` & `pydantic_changedetect-0.6.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2024-04-15 08:26:03.233980 pydantic_changedetect-0.6.6/LICENSE
--rw-r--r--   0        0        0     5576 2024-04-15 08:26:03.233980 pydantic_changedetect-0.6.6/README.md
--rw-r--r--   0        0        0       47 2024-04-15 08:26:03.233980 pydantic_changedetect-0.6.6/pydantic_changedetect/__init__.py
--rw-r--r--   0        0        0     1407 2024-04-15 08:26:03.233980 pydantic_changedetect-0.6.6/pydantic_changedetect/_compat.py
--rw-r--r--   0        0        0    31972 2024-04-15 08:26:03.237980 pydantic_changedetect-0.6.6/pydantic_changedetect/changedetect.py
--rw-r--r--   0        0        0        0 2024-04-15 08:26:03.237980 pydantic_changedetect-0.6.6/pydantic_changedetect/py.typed
--rw-r--r--   0        0        0     2654 2024-04-15 08:26:03.237980 pydantic_changedetect-0.6.6/pydantic_changedetect/utils.py
--rw-r--r--   0        0        0     1052 2024-04-15 08:26:03.237980 pydantic_changedetect-0.6.6/pyproject.toml
--rw-r--r--   0        0        0     6394 1970-01-01 00:00:00.000000 pydantic_changedetect-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-04-17 07:38:33.849676 pydantic_changedetect-0.6.7/LICENSE
+-rw-r--r--   0        0        0     5584 2024-04-17 07:38:33.849676 pydantic_changedetect-0.6.7/README.md
+-rw-r--r--   0        0        0       71 2024-04-17 07:38:33.849676 pydantic_changedetect-0.6.7/pydantic_changedetect/__init__.py
+-rw-r--r--   0        0        0     1407 2024-04-17 07:38:33.849676 pydantic_changedetect-0.6.7/pydantic_changedetect/_compat.py
+-rw-r--r--   0        0        0    31972 2024-04-17 07:38:33.849676 pydantic_changedetect-0.6.7/pydantic_changedetect/changedetect.py
+-rw-r--r--   0        0        0        0 2024-04-17 07:38:33.849676 pydantic_changedetect-0.6.7/pydantic_changedetect/py.typed
+-rw-r--r--   0        0        0     2654 2024-04-17 07:38:33.849676 pydantic_changedetect-0.6.7/pydantic_changedetect/utils.py
+-rw-r--r--   0        0        0     1052 2024-04-17 07:38:33.849676 pydantic_changedetect-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0     6402 1970-01-01 00:00:00.000000 pydantic_changedetect-0.6.7/PKG-INFO
```

### Comparing `pydantic_changedetect-0.6.6/LICENSE` & `pydantic_changedetect-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_changedetect-0.6.6/README.md` & `pydantic_changedetect-0.6.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Pydantic change detection
 
 ## Installation
 
 Just use `pip install pydantic-changedetect` to install the library.
 
 **Note:** `pydantic-changedetect` is compatible with `pydantic` versions `1.9`, `1.10` and even `2.x` (🥳) on
-Python `3.8`, `3.9`, `3.10` and `3.11`. This is also ensured running all tests on all those versions
+Python `3.8`, `3.9`, `3.10`, `3.11` and `3.12`. This is also ensured running all tests on all those versions
 using `tox`.
 
 ## About
 
 When working with database models it is pretty common to want to detect changes
 to the model attributes. The `ChangeDetectionMixin` just provides this mechanism
 to any pydantic models. Changes will be detected and stored after the model
```

### Comparing `pydantic_changedetect-0.6.6/pydantic_changedetect/_compat.py` & `pydantic_changedetect-0.6.7/pydantic_changedetect/_compat.py`

 * *Files identical despite different names*

### Comparing `pydantic_changedetect-0.6.6/pydantic_changedetect/changedetect.py` & `pydantic_changedetect-0.6.7/pydantic_changedetect/changedetect.py`

 * *Files identical despite different names*

### Comparing `pydantic_changedetect-0.6.6/pydantic_changedetect/utils.py` & `pydantic_changedetect-0.6.7/pydantic_changedetect/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_changedetect-0.6.6/pyproject.toml` & `pydantic_changedetect-0.6.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-changedetect"
-version = "0.6.6"
+version = "0.6.7"
 description = "Extend pydantic models to also detect and record changes made to the model attributes."
 authors = ["TEAM23 GmbH <info@team23.de>"]
 license = "MIT"
 repository = "https://github.com/team23/pydantic-changedetect"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `pydantic_changedetect-0.6.6/PKG-INFO` & `pydantic_changedetect-0.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-changedetect
-Version: 0.6.6
+Version: 0.6.7
 Summary: Extend pydantic models to also detect and record changes made to the model attributes.
 Home-page: https://github.com/team23/pydantic-changedetect
 License: MIT
 Author: TEAM23 GmbH
 Author-email: info@team23.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -21,15 +21,15 @@
 # Pydantic change detection
 
 ## Installation
 
 Just use `pip install pydantic-changedetect` to install the library.
 
 **Note:** `pydantic-changedetect` is compatible with `pydantic` versions `1.9`, `1.10` and even `2.x` (🥳) on
-Python `3.8`, `3.9`, `3.10` and `3.11`. This is also ensured running all tests on all those versions
+Python `3.8`, `3.9`, `3.10`, `3.11` and `3.12`. This is also ensured running all tests on all those versions
 using `tox`.
 
 ## About
 
 When working with database models it is pretty common to want to detect changes
 to the model attributes. The `ChangeDetectionMixin` just provides this mechanism
 to any pydantic models. Changes will be detected and stored after the model
```

