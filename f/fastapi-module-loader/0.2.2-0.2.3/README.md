# Comparing `tmp/fastapi_module_loader-0.2.2.tar.gz` & `tmp/fastapi_module_loader-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_module_loader-0.2.2.tar", max compression
+gzip compressed data, was "fastapi_module_loader-0.2.3.tar", max compression
```

## Comparing `fastapi_module_loader-0.2.2.tar` & `fastapi_module_loader-0.2.3.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1078 2024-01-04 20:59:28.251911 fastapi_module_loader-0.2.2/LICENSE
--rw-r--r--   0        0        0     7547 2024-01-04 20:59:28.251911 fastapi_module_loader-0.2.2/README.md
--rw-r--r--   0        0        0      106 2024-01-04 20:59:28.251911 fastapi_module_loader-0.2.2/fastapi_module_loader/__init__.py
--rw-r--r--   0        0        0      158 2024-01-04 20:59:28.251911 fastapi_module_loader-0.2.2/fastapi_module_loader/exceptions.py
--rw-r--r--   0        0        0     2844 2024-01-04 20:59:28.251911 fastapi_module_loader-0.2.2/fastapi_module_loader/loader.py
--rw-r--r--   0        0        0     1268 2024-01-04 20:59:28.251911 fastapi_module_loader-0.2.2/fastapi_module_loader/module.py
--rw-r--r--   0        0        0     1061 2024-01-04 20:59:28.251911 fastapi_module_loader-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     8366 1970-01-01 00:00:00.000000 fastapi_module_loader-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-04-17 07:28:12.793977 fastapi_module_loader-0.2.3/LICENSE
+-rw-r--r--   0        0        0     7547 2024-04-17 07:28:12.793977 fastapi_module_loader-0.2.3/README.md
+-rw-r--r--   0        0        0      136 2024-04-17 07:28:12.793977 fastapi_module_loader-0.2.3/fastapi_module_loader/__init__.py
+-rw-r--r--   0        0        0      158 2024-04-17 07:28:12.793977 fastapi_module_loader-0.2.3/fastapi_module_loader/exceptions.py
+-rw-r--r--   0        0        0     2844 2024-04-17 07:28:12.793977 fastapi_module_loader-0.2.3/fastapi_module_loader/loader.py
+-rw-r--r--   0        0        0     1268 2024-04-17 07:28:12.793977 fastapi_module_loader-0.2.3/fastapi_module_loader/module.py
+-rw-r--r--   0        0        0        0 2024-04-17 07:28:12.793977 fastapi_module_loader-0.2.3/fastapi_module_loader/py.typed
+-rw-r--r--   0        0        0     1087 2024-04-17 07:28:12.793977 fastapi_module_loader-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     8366 1970-01-01 00:00:00.000000 fastapi_module_loader-0.2.3/PKG-INFO
```

### Comparing `fastapi_module_loader-0.2.2/LICENSE` & `fastapi_module_loader-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_module_loader-0.2.2/README.md` & `fastapi_module_loader-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_module_loader-0.2.2/fastapi_module_loader/loader.py` & `fastapi_module_loader-0.2.3/fastapi_module_loader/loader.py`

 * *Files identical despite different names*

### Comparing `fastapi_module_loader-0.2.2/fastapi_module_loader/module.py` & `fastapi_module_loader-0.2.3/fastapi_module_loader/module.py`

 * *Files identical despite different names*

### Comparing `fastapi_module_loader-0.2.2/pyproject.toml` & `fastapi_module_loader-0.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 [tool.poetry]
 name = "fastapi-module-loader"
-version = "0.2.2"
+version = "0.2.3"
 description = "FastAPI modules loading for better structure in your projects (like Django AppConfig)"
 authors = ["TEAM23 GmbH <info@team23.de>"]
 license = "MIT"
 repository = "https://github.com/team23/fastapi-module-loading"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 fastapi = ">=0.65.2,<1.0.0"
 
 [tool.poetry.group.dev.dependencies]
-pytest = ">=7.1.2,<8.0.0"
-pytest-cov = ">=3,<5"
-mypy = ">=0.971,<2.0"
+pytest = ">=7.1.2,<9.0.0"
+pytest-cov = ">=3,<6"
 tox = ">=3.26,<5.0"
 httpx = ">=0.24.1,<1.0.0"
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
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fastapi_module_loader-0.2.2/PKG-INFO` & `fastapi_module_loader-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-module-loader
-Version: 0.2.2
+Version: 0.2.3
 Summary: FastAPI modules loading for better structure in your projects (like Django AppConfig)
 Home-page: https://github.com/team23/fastapi-module-loading
 License: MIT
 Author: TEAM23 GmbH
 Author-email: info@team23.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

