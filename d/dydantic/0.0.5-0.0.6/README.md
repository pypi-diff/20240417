# Comparing `tmp/dydantic-0.0.5.tar.gz` & `tmp/dydantic-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dydantic-0.0.5.tar", max compression
+gzip compressed data, was "dydantic-0.0.6.tar", max compression
```

## Comparing `dydantic-0.0.5.tar` & `dydantic-0.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2024-04-06 05:52:07.999927 dydantic-0.0.5/LICENSE
--rw-r--r--   0        0        0     2847 2024-04-12 23:11:08.576469 dydantic-0.0.5/README.md
--rw-r--r--   0        0        0     1979 2024-04-08 06:06:13.745492 dydantic-0.0.5/dydantic/__init__.py
--rw-r--r--   0        0        0    18628 2024-04-15 23:58:29.574296 dydantic-0.0.5/dydantic/_utils.py
--rw-r--r--   0        0        0        0 2024-04-06 06:24:35.972780 dydantic-0.0.5/dydantic/py.typed
--rw-r--r--   0        0        0     1312 2024-04-15 23:58:29.574807 dydantic-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3467 1970-01-01 00:00:00.000000 dydantic-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-06 05:52:07.999927 dydantic-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2847 2024-04-12 23:11:08.576469 dydantic-0.0.6/README.md
+-rw-r--r--   0        0        0     1979 2024-04-08 06:06:13.745492 dydantic-0.0.6/dydantic/__init__.py
+-rw-r--r--   0        0        0    18684 2024-04-17 06:31:12.794625 dydantic-0.0.6/dydantic/_utils.py
+-rw-r--r--   0        0        0        0 2024-04-06 06:24:35.972780 dydantic-0.0.6/dydantic/py.typed
+-rw-r--r--   0        0        0     1452 2024-04-17 06:31:12.795906 dydantic-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3552 1970-01-01 00:00:00.000000 dydantic-0.0.6/PKG-INFO
```

### Comparing `dydantic-0.0.5/LICENSE` & `dydantic-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dydantic-0.0.5/README.md` & `dydantic-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `dydantic-0.0.5/dydantic/__init__.py` & `dydantic-0.0.6/dydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `dydantic-0.0.5/dydantic/_utils.py` & `dydantic-0.0.6/dydantic/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -433,14 +433,16 @@
         type_ = pydantic_type
 
     if isinstance(type_, type) and issubclass(type_, str):
         if "minLength" in json_schema:
             field_kwargs["min_length"] = json_schema["minLength"]
         if "maxLength" in json_schema:
             field_kwargs["max_length"] = json_schema["maxLength"]
+    if not is_required:
+        type_ = Optional[type_]
     return (type_, Field(default, json_schema_extra=field_kwargs))
 
 
 def _json_schema_to_pydantic_type(
     json_schema: Dict[str, Any],
     root_schema: Dict[str, Any],
     *,
```

### Comparing `dydantic-0.0.5/pyproject.toml` & `dydantic-0.0.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 [tool.poetry]
 name = "dydantic"
-version = "0.0.5"
+version = "0.0.6"
 description = "Dynamically generate pydantic models from JSON schema."
 authors = ["William Fu-Hinthorn <13333726+hinthornw@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pydantic = "^2"
+email-validator = { version = "^2.1", optional = true }
+
+[tool.poetry.extras]
+email = ["email-validator"]
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.3.5"
 black = "^24.3.0"
 mypy = "^1.9.0"
 
 
 [tool.poetry.group.test.dependencies]
 poethepoet = "^0.25.0"
 pytest = "^8.1.1"
 
+[tool.poetry.group.email.dependencies]
+email-validator = "^2.1.0"
+
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.5.3"
 mkdocs-material = "^9.5.17"
 mkdocstrings = "^0.24.3"
 mkdocstrings-python = "^1.9.2"
 mkdocs-redirects = "^1.2.1"
@@ -39,28 +46,17 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poe.tasks]
 ruff = "ruff"
 black = "black"
 mypy = "mypy"
-format = [
-    "ruff check --fix .",
-    "black .",
-    "ruff format ."
-]
-lint = [
-    "ruff check .",
-    "mypy ."
-]
+format = ["ruff check --fix .", "black .", "ruff format ."]
+lint = ["ruff check .", "mypy ."]
 pytest = "poetry run pytest"
 test = "poetry run pytest tests"
 doctest = "pytest --doctest-modules dydantic"
 
 mkdocs = "poetry run mkdocs"
-build-docs ="mkdocs build --clean -f docs/mkdocs.yml"
-
-serve-docs = [
-   "build-docs",
-   "mkdocs serve -f docs/mkdocs.yml",
-]
+build-docs = "mkdocs build --clean -f docs/mkdocs.yml"
 
+serve-docs = ["build-docs", "mkdocs serve -f docs/mkdocs.yml"]
```

### Comparing `dydantic-0.0.5/PKG-INFO` & `dydantic-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: dydantic
-Version: 0.0.5
+Version: 0.0.6
 Summary: Dynamically generate pydantic models from JSON schema.
 License: MIT
 Author: William Fu-Hinthorn
 Author-email: 13333726+hinthornw@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: email
+Requires-Dist: email-validator (>=2.1,<3.0) ; extra == "email"
 Requires-Dist: pydantic (>=2,<3)
 Description-Content-Type: text/markdown
 
 # dydantic
 
 [![Documentation](https://img.shields.io/badge/docs-hinthornw.github.io%2Fdydantic-blue)](https://hinthornw.github.io/dydantic/) [![GitHub Repo](https://img.shields.io/badge/GitHub-Repo-black?logo=github)](https://github.com/hinthornw/dydantic)
```

