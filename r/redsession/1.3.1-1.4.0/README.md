# Comparing `tmp/redsession-1.3.1.tar.gz` & `tmp/redsession-1.4.0.tar.gz`

## Comparing `redsession-1.3.1.tar` & `redsession-1.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 redsession-1.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 redsession-1.3.1/.readthedocs.yaml
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 redsession-1.3.1/requirements-docs.txt
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 redsession-1.3.1/requirements-tests.txt
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 redsession-1.3.1/requirements.txt
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 redsession-1.3.1/redsession/__init__.py
--rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 redsession-1.3.1/redsession/middleware.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 redsession-1.3.1/redsession/backend/__init__.py
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 redsession-1.3.1/redsession/backend/base.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 redsession-1.3.1/redsession/backend/redis.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redsession-1.3.1/tests/__init__.py
--rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 redsession-1.3.1/tests/test_session.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 redsession-1.3.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 redsession-1.3.1/LICENSE.md
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 redsession-1.3.1/README.rst
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 redsession-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 redsession-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 redsession-1.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 redsession-1.4.0/.readthedocs.yaml
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 redsession-1.4.0/requirements-docs.txt
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 redsession-1.4.0/requirements-tests.txt
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 redsession-1.4.0/requirements.txt
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 redsession-1.4.0/redsession/__init__.py
+-rw-r--r--   0        0        0     6679 2020-02-02 00:00:00.000000 redsession-1.4.0/redsession/middleware.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 redsession-1.4.0/redsession/backend/__init__.py
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 redsession-1.4.0/redsession/backend/base.py
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 redsession-1.4.0/redsession/backend/redis.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redsession-1.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 redsession-1.4.0/tests/test_session.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 redsession-1.4.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 redsession-1.4.0/LICENSE.md
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 redsession-1.4.0/README.rst
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 redsession-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 redsession-1.4.0/PKG-INFO
```

### Comparing `redsession-1.3.1/.pre-commit-config.yaml` & `redsession-1.4.0/.pre-commit-config.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 default_language_version:
   python: python3.11
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
-  - repo: https://github.com/psf/black
-    rev: 23.10.1
-    hooks:
-      - id: black
-
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.15.0
+    rev: v3.15.2
     hooks:
       - id: pyupgrade
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.1.4
+    rev: v0.3.7
     hooks:
+      # Run the linter.
       - id: ruff
-        args:
-          - --fix
+        args: [ --fix ]
+      # Run the formatter.
+      - id: ruff-format
```

### Comparing `redsession-1.3.1/.readthedocs.yaml` & `redsession-1.4.0/.readthedocs.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Required
 version: 2
 
 # Set the OS, Python version and other tools you might need
 build:
   os: ubuntu-22.04
   tools:
-    python: "3.11"
+    python: "3.12"
 
 # Build documentation in the "docs/" directory with Sphinx
 sphinx:
   configuration: docs/conf.py
 
 # Optional but recommended, declare the Python requirements required
 # to build your documentation
```

### Comparing `redsession-1.3.1/redsession/middleware.py` & `redsession-1.4.0/redsession/middleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,26 @@
             "lax", "strict", or "none". Default is "lax".
 
         https_only (:obj:`bool`, optional): If True, the "secure" flag will
             be added to the session cookie, making it accessible only over
             HTTPS. Default is False.
     """
 
+    __slots__ = (
+        "_app",
+        "_backend",
+        "_session_length",
+        "_name_cookie",
+        "_max_age",
+        "_path",
+        "_domain",
+        "_security_flags",
+        "signer",
+    )
+
     def __init__(
         self,
         app: ASGIApp,
         backend: BaseAsyncBackend,
         secret_key: Iterable[str] | str,
         session_length: int = 16,
         name_cookie: str = "s",
```

### Comparing `redsession-1.3.1/redsession/backend/base.py` & `redsession-1.4.0/redsession/backend/base.py`

 * *Files identical despite different names*

### Comparing `redsession-1.3.1/redsession/backend/redis.py` & `redsession-1.4.0/redsession/backend/redis.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
-import orjson
+try:
+    import orjson as json
+except ImportError:
+    import json  # type: ignore
 
 if TYPE_CHECKING:
     from redis.asyncio import Redis
 
 from .base import BaseAsyncBackend
 
 
@@ -20,20 +23,20 @@
 
     def __init__(self, redis: Redis[Any]) -> None:  # type: ignore
         self.redis = redis
 
     async def get(self, key: str) -> dict[str, Any] | None:
         data = await self.redis.get(key)
         if data:
-            return orjson.loads(data)  # type: ignore
+            return json.loads(data)  # type: ignore
         return None
 
     async def set(self, key: str, value: dict[str, Any], ex: int | None = None) -> Any:
-        data = orjson.dumps(value)
+        data = json.dumps(value)
         return await self.redis.set(key, data, ex)
 
     async def update(self, key: str, value: dict[str, Any]) -> Any:
-        data = orjson.dumps(value)
+        data = json.dumps(value)
         return await self.redis.set(key, data, keepttl=True)
 
     async def delete(self, key: str) -> Any:
         return await self.redis.delete(key)
```

### Comparing `redsession-1.3.1/tests/test_session.py` & `redsession-1.4.0/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `redsession-1.3.1/LICENSE.md` & `redsession-1.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `redsession-1.3.1/README.rst` & `redsession-1.4.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -40,11 +40,17 @@
 You can install or update starlette-middleware
 
 .. code:: shell
 
     $ pip install redsession --upgrade
 
 
+If you want to use `orjson` and `hiredis` to maximize performance, use the optional dependencies
+
+.. code:: shell
+
+    $ pip install redsession[opt] --upgrade
+
 Documentation
 =============
 
 You can find more information on usage `here <https://red-session.readthedocs.io/en/stable/>`_.
```

### Comparing `redsession-1.3.1/pyproject.toml` & `redsession-1.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -23,42 +23,40 @@
     "Framework :: FastAPI",
 ]
 dynamic = ["version"]
 
 dependencies = [
     "starlette>=0.36.3",
     "itsdangerous>=2.1.2",
-    "redis[hiredis]>=5.0.0,<6.0.0",
-    "orjson>=3.9.0",
+    "redis>=5.0.0,<6.0.0",
 ]
 
+[project.optional-dependencies]
+opt = ["redis[hiredis]>=5.0.0,<6.0.0", "orjson>=3.9.0"]
+
 [project.urls]
 Repository = "https://github.com/TheJecksMan/red-session"
 Issues = "https://github.com/TheJecksMan/red-session/issues"
 Docs = "https://red-session.readthedocs.io/en/stable/"
 
 [tool.hatch.version]
 path = "redsession/__init__.py"
 
 [tool.hatch.build.targets.sdist]
 exclude = ["/.github", "/docs", "/examples"]
 
 [tool.mypy]
 strict = true
 
-[tool.ruff.lint]
+[tool.ruff]
 select = [
     "E",  # pycodestyle errors
     "W",  # pycodestyle warnings
     "F",  # pyflakes
     "I",  # isort
     "B",  # flake8-bugbear
     "FA", # flake8-future-annotations
     "UP", # pyupgrade
 ]
 
-# [tool.ruff.lint.per-file-ignores]
-# "examples/fastapi.py" = ["I001"]
-# "examples/starlette.py" = ["I001"]
-
 [tool.ruff.format]
 quote-style = "double"
```

### Comparing `redsession-1.3.1/PKG-INFO` & `redsession-1.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: redsession
-Version: 1.3.1
+Version: 1.4.0
 Summary: Simple and fast server session middleware for FastAPI and Starlette
 Project-URL: Repository, https://github.com/TheJecksMan/red-session
 Project-URL: Issues, https://github.com/TheJecksMan/red-session/issues
 Project-URL: Docs, https://red-session.readthedocs.io/en/stable/
 Author: TheJecksMan
 License-Expression: MIT
 License-File: LICENSE.md
@@ -17,17 +17,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Requires-Dist: itsdangerous>=2.1.2
-Requires-Dist: orjson>=3.9.0
-Requires-Dist: redis[hiredis]<6.0.0,>=5.0.0
+Requires-Dist: redis<6.0.0,>=5.0.0
 Requires-Dist: starlette>=0.36.3
+Provides-Extra: opt
+Requires-Dist: orjson>=3.9.0; extra == 'opt'
+Requires-Dist: redis[hiredis]<6.0.0,>=5.0.0; extra == 'opt'
 Description-Content-Type: text/x-rst
 
 .. image:: https://raw.githubusercontent.com/TheJecksMan/red-session/main/docs/_static/logo_lib.png
    :align: center
    :alt: red-session logo
    :width: 200
 
@@ -68,11 +70,17 @@
 You can install or update starlette-middleware
 
 .. code:: shell
 
     $ pip install redsession --upgrade
 
 
+If you want to use `orjson` and `hiredis` to maximize performance, use the optional dependencies
+
+.. code:: shell
+
+    $ pip install redsession[opt] --upgrade
+
 Documentation
 =============
 
 You can find more information on usage `here <https://red-session.readthedocs.io/en/stable/>`_.
```

