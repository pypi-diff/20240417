# Comparing `tmp/ovld-0.3.4.tar.gz` & `tmp/ovld-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovld-0.3.4.tar", max compression
+gzip compressed data, was "ovld-0.3.5.tar", max compression
```

## Comparing `ovld-0.3.4.tar` & `ovld-0.3.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2021-03-11 20:11:21.537259 ovld-0.3.4/LICENSE
--rw-r--r--   0        0        0     8758 2021-06-21 18:33:09.067471 ovld-0.3.4/README.md
--rw-r--r--   0        0        0       85 2021-03-03 23:11:27.683713 ovld-0.3.4/ovld/__init__.py
--rw-r--r--   0        0        0    33078 2024-04-12 18:44:42.542358 ovld-0.3.4/ovld/core.py
--rw-r--r--   0        0        0     5006 2024-04-12 16:00:16.628660 ovld-0.3.4/ovld/mro.py
--rw-r--r--   0        0        0     3861 2024-04-12 16:08:27.619178 ovld-0.3.4/ovld/utils.py
--rw-r--r--   0        0        0       18 2024-04-12 18:59:54.328025 ovld-0.3.4/ovld/version.py
--rw-r--r--   0        0        0      906 2024-04-12 18:59:54.304605 ovld-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     9439 1970-01-01 00:00:00.000000 ovld-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2021-03-11 20:11:21.537259 ovld-0.3.5/LICENSE
+-rw-r--r--   0        0        0     8758 2021-06-21 18:33:09.067471 ovld-0.3.5/README.md
+-rw-r--r--   0        0        0       85 2021-03-03 23:11:27.683713 ovld-0.3.5/ovld/__init__.py
+-rw-r--r--   0        0        0    33146 2024-04-17 21:20:39.250013 ovld-0.3.5/ovld/core.py
+-rw-r--r--   0        0        0     5006 2024-04-17 21:20:05.582720 ovld-0.3.5/ovld/mro.py
+-rw-r--r--   0        0        0     3861 2024-04-13 23:23:42.261204 ovld-0.3.5/ovld/utils.py
+-rw-r--r--   0        0        0       18 2024-04-17 21:31:05.427244 ovld-0.3.5/ovld/version.py
+-rw-r--r--   0        0        0      715 2024-04-17 21:31:05.404446 ovld-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     9439 1970-01-01 00:00:00.000000 ovld-0.3.5/PKG-INFO
```

### Comparing `ovld-0.3.4/LICENSE` & `ovld-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ovld-0.3.4/README.md` & `ovld-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `ovld-0.3.4/ovld/core.py` & `ovld-0.3.5/ovld/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,18 +4,23 @@
 import itertools
 import math
 import textwrap
 import typing
 from types import FunctionType
 
 try:
-    from types import GenericAlias, UnionType
+    from types import UnionType
 except ImportError:  # pragma: no cover
     UnionType = None
 
+
+try:
+    from types import GenericAlias
+except ImportError:  # pragma: no cover
+
     class GenericAliasMC(type):
         def __instancecheck__(cls, obj):
             return hasattr(obj, "__origin__")
 
     class GenericAlias(metaclass=GenericAliasMC):
         pass
```

### Comparing `ovld-0.3.4/ovld/mro.py` & `ovld-0.3.5/ovld/mro.py`

 * *Files identical despite different names*

### Comparing `ovld-0.3.4/ovld/utils.py` & `ovld-0.3.5/ovld/utils.py`

 * *Files identical despite different names*

### Comparing `ovld-0.3.4/pyproject.toml` & `ovld-0.3.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,32 @@
 [tool.poetry]
 name = "ovld"
-version = "0.3.4"
+version = "0.3.5"
 description = "Overloading Python functions"
 authors = ["Olivier Breuleux <breuleux@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/breuleux/ovld"
 repository = "https://github.com/breuleux/ovld"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 [tool.poetry.dev-dependencies]
-black = "^24.3.0"
 ruff = "^0.3.5"
 codefind = "^0.1.0"
 pytest = "^6.0.1"
 pytest-cov = "^2.10.0"
 
-[tool.black]
-line-length = 80
-
-[tool.isort]
-known_first_party = "ovld"
-known_third_party = ""
-multi_line_output = 3
-include_trailing_comma = true
-combine_as_imports = true
-
 [build-system]
 requires = ["poetry-core>=1.0.8"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
-line-length = 99
+line-length = 80
 
 [tool.ruff.lint]
 extend-select = ["I"]
 ignore = ["E241", "F722", "E501", "E203", "F811", "F821"]
 
 [tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401", "F403"]
```

### Comparing `ovld-0.3.4/PKG-INFO` & `ovld-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovld
-Version: 0.3.4
+Version: 0.3.5
 Summary: Overloading Python functions
 Home-page: https://github.com/breuleux/ovld
 License: MIT
 Author: Olivier Breuleux
 Author-email: breuleux@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

