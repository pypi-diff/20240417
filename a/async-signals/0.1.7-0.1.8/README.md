# Comparing `tmp/async_signals-0.1.7.tar.gz` & `tmp/async_signals-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_signals-0.1.7.tar", max compression
+gzip compressed data, was "async_signals-0.1.8.tar", max compression
```

## Comparing `async_signals-0.1.7.tar` & `async_signals-0.1.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1665 2024-01-04 21:04:00.096240 async_signals-0.1.7/LICENSE
--rw-r--r--   0        0        0     4416 2024-01-04 21:04:00.096240 async_signals-0.1.7/README.md
--rw-r--r--   0        0        0      302 2024-01-04 21:04:00.096240 async_signals-0.1.7/async_signals/__init__.py
--rw-r--r--   0        0        0    13159 2024-01-04 21:04:00.096240 async_signals-0.1.7/async_signals/dispatcher.py
--rw-r--r--   0        0        0     3427 2024-01-04 21:04:00.096240 async_signals-0.1.7/async_signals/license.txt
--rw-r--r--   0        0        0        0 2024-01-04 21:04:00.096240 async_signals-0.1.7/async_signals/py.typed
--rw-r--r--   0        0        0      959 2024-01-04 21:04:00.096240 async_signals-0.1.7/async_signals/utils.py
--rw-r--r--   0        0        0     1096 2024-01-04 21:04:00.096240 async_signals-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     5169 1970-01-01 00:00:00.000000 async_signals-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1665 2024-04-17 07:25:01.430515 async_signals-0.1.8/LICENSE
+-rw-r--r--   0        0        0     4416 2024-04-17 07:25:01.430515 async_signals-0.1.8/README.md
+-rw-r--r--   0        0        0      347 2024-04-17 07:25:01.430515 async_signals-0.1.8/async_signals/__init__.py
+-rw-r--r--   0        0        0    13159 2024-04-17 07:25:01.430515 async_signals-0.1.8/async_signals/dispatcher.py
+-rw-r--r--   0        0        0     3427 2024-04-17 07:25:01.430515 async_signals-0.1.8/async_signals/license.txt
+-rw-r--r--   0        0        0        0 2024-04-17 07:25:01.430515 async_signals-0.1.8/async_signals/py.typed
+-rw-r--r--   0        0        0      959 2024-04-17 07:25:01.430515 async_signals-0.1.8/async_signals/utils.py
+-rw-r--r--   0        0        0     1130 2024-04-17 07:25:01.430515 async_signals-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     5169 1970-01-01 00:00:00.000000 async_signals-0.1.8/PKG-INFO
```

### Comparing `async_signals-0.1.7/LICENSE` & `async_signals-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `async_signals-0.1.7/README.md` & `async_signals-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `async_signals-0.1.7/async_signals/dispatcher.py` & `async_signals-0.1.8/async_signals/dispatcher.py`

 * *Files identical despite different names*

### Comparing `async_signals-0.1.7/async_signals/license.txt` & `async_signals-0.1.8/async_signals/license.txt`

 * *Files identical despite different names*

### Comparing `async_signals-0.1.7/async_signals/utils.py` & `async_signals-0.1.8/async_signals/utils.py`

 * *Files identical despite different names*

### Comparing `async_signals-0.1.7/pyproject.toml` & `async_signals-0.1.8/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 [tool.poetry]
 name = "async-signals"
-version = "0.1.7"
+version = "0.1.8"
 description = "Async version of the Django signals class - for usage in for example FastAPI."
 authors = ["TEAM23 GmbH <info@team23.de>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/team23/async-signals"
 readme = "README.md"
 packages = [{include = "async_signals"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.1.3"
-pytest-cov = ">=3,<5"
+pytest = ">=7.1.3,<9.0.0"
+pytest-cov = ">=3,<6"
 pytest-mock = "^3.8.2"
-mypy = ">=0.971,<2.0"
 anyio = {extras = ["trio"], version = ">=3.6.1,<5.0.0"}
 tox = ">=3.26,<5.0"
-ruff = ">=0.0.284,<0.2.0"
+ruff = ">=0.2.0,<0.4.0"
+pyright = ">=1.1.350,<1.2"
 
 [tool.ruff]
-select = ["F","E","W","C","I","N","UP","ANN","S","B","A","COM","C4","T20","PT","ARG","TD","RUF"]
 line-length = 115
 target-version = "py38"
-ignore = ["A001","A002","A003","ANN101","ANN102","ANN401","C901","N8","B008","F405","F821"]
 output-format = "grouped"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint]
+select = ["F","E","W","C","I","N","UP","ANN","S","B","A","COM","C4","T20","PT","ARG","TD","RUF"]
+ignore = ["A001","A002","A003","ANN101","ANN102","ANN401","C901","N8","B008","F405","F821"]
+
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
 "conftest.py" = ["S101","ANN","F401"]
 "test_*.py" = ["S101","ANN","F401","ARG001"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `async_signals-0.1.7/PKG-INFO` & `async_signals-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-signals
-Version: 0.1.7
+Version: 0.1.8
 Summary: Async version of the Django signals class - for usage in for example FastAPI.
 Home-page: https://github.com/team23/async-signals
 License: BSD-3-Clause
 Author: TEAM23 GmbH
 Author-email: info@team23.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

