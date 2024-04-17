# Comparing `tmp/pypomes_core-0.8.5.tar.gz` & `tmp/pypomes_core-0.8.6.tar.gz`

## Comparing `pypomes_core-0.8.5.tar` & `pypomes_core-0.8.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     6763 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/src/pypomes_core/.ruff.toml
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    27941 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6218 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/src/pypomes_core/validation_msgs.py
--rw-r--r--   0        0        0    23119 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0     6824 2020-02-02 00:00:00.000000 pypomes_core-0.8.6/src/pypomes_core/.ruff.toml
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 pypomes_core-0.8.6/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 pypomes_core-0.8.6/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    27940 2020-02-02 00:00:00.000000 pypomes_core-0.8.6/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 pypomes_core-0.8.6/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-0.8.6/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 pypomes_core-0.8.6/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.8.6/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 pypomes_core-0.8.6/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.8.6/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6218 2020-02-02 00:00:00.000000 pypomes_core-0.8.6/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 pypomes_core-0.8.6/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 pypomes_core-0.8.6/src/pypomes_core/validation_msgs.py
+-rw-r--r--   0        0        0    23119 2020-02-02 00:00:00.000000 pypomes_core-0.8.6/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 pypomes_core-0.8.6/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.8.6/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.8.6/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.8.6/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.8.6/PKG-INFO
```

### Comparing `pypomes_core-0.8.5/src/pypomes_core/.ruff.toml` & `pypomes_core-0.8.6/src/pypomes_core/.ruff.toml`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 #   "T10",   # flake8-debugger - check for 'pdb;idbp' imports and set traces
 #   "T20",   # flake8-print - check for 'print' and 'pprint' statements in python files
 ]
 ignore = [
     "ANN002",   # missing type annotation for *kargs
     "ANN101",   # missing type annotation for 'self' in method
     "ANN401",   # dynamically typed expressions (typing.Any) are disallowed
+    "COM812",   # checks for the absence of trailing commas
     "COM819",   # prohibited trailing commas
     "D200",     # one-line docstring should fit on one line
     "D204",     # 1 blank line required after class docstring
     "D210",     # whitespaces surrounding docstring text
     "D212",     # multi-line docstring summary to start at the second line
     "DTZ005",   # the use of datetime.datetime.now() without tz argument is not allowed
     "G004",     # logging statement uses 'f-string'
```

### Comparing `pypomes_core-0.8.5/src/pypomes_core/__init__.py` & `pypomes_core-0.8.6/src/pypomes_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.5/src/pypomes_core/datetime_pomes.py` & `pypomes_core-0.8.6/src/pypomes_core/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.5/src/pypomes_core/dict_pomes.py` & `pypomes_core-0.8.6/src/pypomes_core/dict_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -610,15 +610,15 @@
 
 def dict_clone(source: dict, from_to_keys: list) -> dict:
     """
     Build a new *dict*, according to the rules presented herein.
 
     This dictionary is constructed by creating a new element for each element in the list
     *from_to_keys*. When the element of this list is a tuple, the name indicated by its
-    second term is used, and the value of the *source* element indicated by the tuple´s
+    second term is used, and the value of the *source* element indicated by the tuple's
     first term is assigned. This first term can be represented by a chain of  nested keys.
     The name of the element to be created can be omitted, in which case the name of the term
     indicative of the value to be assigned is used. If the corresponding value is not found
     in *source*, *None* is assigned.
 
     :param source: the source dict
     :param from_to_keys: list of elements indicative of the source and target keys
```

### Comparing `pypomes_core-0.8.5/src/pypomes_core/email_pomes.py` & `pypomes_core-0.8.6/src/pypomes_core/email_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.5/src/pypomes_core/encoding_pomes.py` & `pypomes_core-0.8.6/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.5/src/pypomes_core/env_pomes.py` & `pypomes_core-0.8.6/src/pypomes_core/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.5/src/pypomes_core/exception_pomes.py` & `pypomes_core-0.8.6/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.5/src/pypomes_core/file_pomes.py` & `pypomes_core-0.8.6/src/pypomes_core/file_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from flask import Request
 from pathlib import Path
 from tempfile import gettempdir
 from typing import Final
 from werkzeug.datastructures import FileStorage
+
 from .env_pomes import APP_PREFIX, env_get_path
 
 TEMP_DIR: Final[Path] = env_get_path(f"{APP_PREFIX}_TEMP_DIR", Path(gettempdir()))
 
 
 def file_from_request(request: Request, file_name: str = None, file_seq: int = 0) -> bytes:
     """
```

### Comparing `pypomes_core-0.8.5/src/pypomes_core/json_pomes.py` & `pypomes_core-0.8.6/src/pypomes_core/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.5/src/pypomes_core/list_pomes.py` & `pypomes_core-0.8.6/src/pypomes_core/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.5/src/pypomes_core/str_pomes.py` & `pypomes_core-0.8.6/src/pypomes_core/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.5/src/pypomes_core/validation_msgs.py` & `pypomes_core-0.8.6/src/pypomes_core/validation_msgs.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.5/src/pypomes_core/validation_pomes.py` & `pypomes_core-0.8.6/src/pypomes_core/validation_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.5/LICENSE` & `pypomes_core-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.8.5/pyproject.toml` & `pypomes_core-0.8.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "0.8.5"
+version = "0.8.6"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-0.8.5/PKG-INFO` & `pypomes_core-0.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_core
-Version: 0.8.5
+Version: 0.8.6
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

