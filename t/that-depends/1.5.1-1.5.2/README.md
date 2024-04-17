# Comparing `tmp/that_depends-1.5.1.tar.gz` & `tmp/that_depends-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "that_depends-1.5.1.tar", max compression
+gzip compressed data, was "that_depends-1.5.2.tar", max compression
```

## Comparing `that_depends-1.5.1.tar` & `that_depends-1.5.2.tar`

### file list

```diff
@@ -1,8 +1,13 @@
--rw-r--r--   0        0        0     6086 2024-04-15 19:22:41.395455 that_depends-1.5.1/README.md
--rw-r--r--   0        0        0     1482 2024-04-15 19:33:05.746075 that_depends-1.5.1/pyproject.toml
--rw-r--r--   0        0        0      164 2024-03-18 09:15:04.223171 that_depends-1.5.1/that_depends/__init__.py
--rw-r--r--   0        0        0      747 2024-04-11 11:51:20.009107 that_depends-1.5.1/that_depends/container.py
--rw-r--r--   0        0        0     1013 2024-04-15 19:32:21.955087 that_depends-1.5.1/that_depends/injection.py
--rw-r--r--   0        0        0     5545 2024-04-15 18:25:35.357555 that_depends-1.5.1/that_depends/providers.py
--rw-r--r--   0        0        0        0 2023-08-28 10:48:35.000000 that_depends-1.5.1/that_depends/py.typed
--rw-r--r--   0        0        0     6566 1970-01-01 00:00:00.000000 that_depends-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     6711 2024-04-16 18:31:17.949107 that_depends-1.5.2/README.md
+-rw-r--r--   0        0        0     1482 2024-04-17 05:36:28.992323 that_depends-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0      164 2024-03-18 09:15:04.223171 that_depends-1.5.2/that_depends/__init__.py
+-rw-r--r--   0        0        0      747 2024-04-11 11:51:20.009107 that_depends-1.5.2/that_depends/container.py
+-rw-r--r--   0        0        0     1013 2024-04-15 19:32:21.955087 that_depends-1.5.2/that_depends/injection.py
+-rw-r--r--   0        0        0      484 2024-04-16 06:00:55.731335 that_depends-1.5.2/that_depends/providers/__init__.py
+-rw-r--r--   0        0        0      642 2024-04-16 06:00:18.298948 that_depends-1.5.2/that_depends/providers/base.py
+-rw-r--r--   0        0        0      465 2024-04-16 06:00:22.046508 that_depends-1.5.2/that_depends/providers/collections.py
+-rw-r--r--   0        0        0     1365 2024-04-16 06:00:22.046739 that_depends-1.5.2/that_depends/providers/factories.py
+-rw-r--r--   0        0        0     2552 2024-04-16 06:00:22.049297 that_depends-1.5.2/that_depends/providers/resources.py
+-rw-r--r--   0        0        0      993 2024-04-17 05:36:03.299156 that_depends-1.5.2/that_depends/providers/singleton.py
+-rw-r--r--   0        0        0        0 2023-08-28 10:48:35.000000 that_depends-1.5.2/that_depends/py.typed
+-rw-r--r--   0        0        0     7191 1970-01-01 00:00:00.000000 that_depends-1.5.2/PKG-INFO
```

### Comparing `that_depends-1.5.1/README.md` & `that_depends-1.5.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,40 @@
 "That Depends"
 ==
 This package is dependency injection framework for Python, mostly inspired by `python-dependency-injector`.
 
+It is production-ready and gives you the following:
+- Fully-async simple DI framework with IOC-container.
+- Python 3.10-3.12 support.
+- Full coverage by types annotations (mypy in strict mode).
+- FastAPI and Litestar compatibility.
+- Zero dependencies.
+- Overriding dependencies for tests.
+
+# Main characteristics:
+1. Fully async -> means every dependency resolving is async, so you should construct with `await` keyword:
+```python
+from tests.container import DIContainer
+
+async def main():
+    some_dependency = await DIContainer.independent_factory()
+```
+2. No wiring for injections in function arguments -> achieved by decision that only one instance of container is supported
+```python
+from tests import container
+from that_depends import Provide, inject
+
+
+@inject
+async def some_function(
+    independent_factory: container.IndependentFactory = Provide[container.DIContainer.independent_factory],
+) -> None:
+    assert independent_factory.dep1
+```
+
 # Quickstart
 ## Install
 
 ```bash
 pip install that-depends
 ```
 
@@ -165,15 +194,15 @@
     # resource teardown
 
 class DIContainer(BaseContainer):
     sync_resource = providers.Resource(create_sync_resource)
 ```
 
 ### AsyncResource
-- Same as but async generator function is required.
+- Same as `Resource` but async generator function is required.
 ```python
 import typing
 
 from that_depends import BaseContainer, providers
 
 
 async def create_async_resource() -> typing.AsyncIterator[str]:
@@ -217,15 +246,15 @@
     dep2: int
 
 
 class DIContainer(BaseContainer):
     independent_factory = providers.Factory(IndependentFactory, dep1="text", dep2=123)
 ```
 ### AsyncFactory
-- Initialized on every call, as Factory.
+- Initialized on every call, as `Factory`.
 - Async function is required.
 ```python
 import datetime
 
 from that_depends import BaseContainer, providers
 
 
@@ -245,17 +274,7 @@
 from that_depends import BaseContainer, providers
 
 
 class DIContainer(BaseContainer):
     random_number = providers.Factory(random.random)
     numbers_sequence = providers.List(random_number, random_number)
 ```
-
-# Main decisions:
-1. Every dependency resolving is async, so you should construct with `await` keyword:
-```python
-from tests.container import DIContainer
-
-async def main():
-    some_dependency = await DIContainer.independent_factory()
-```
-2. No containers initialization to avoid wiring -> only one global instance of container is supported
```

### Comparing `that_depends-1.5.1/pyproject.toml` & `that_depends-1.5.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "that-depends"
-version = "1.5.1"
+version = "1.5.2"
 description = "Simple Dependency Injection framework"
 authors = ["Artur Shiriev <me@shiriev.ru>"]
 readme = "README.md"
 homepage = "https://github.com/modern-python/that-depends"
 packages = [
     { include = "that_depends" },
 ]
```

### Comparing `that_depends-1.5.1/that_depends/container.py` & `that_depends-1.5.2/that_depends/container.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.5.1/that_depends/injection.py` & `that_depends-1.5.2/that_depends/injection.py`

 * *Files identical despite different names*

### Comparing `that_depends-1.5.1/PKG-INFO` & `that_depends-1.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: that-depends
-Version: 1.5.1
+Version: 1.5.2
 Summary: Simple Dependency Injection framework
 Home-page: https://github.com/modern-python/that-depends
 Author: Artur Shiriev
 Author-email: me@shiriev.ru
 Requires-Python: >=3.10,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -12,14 +12,43 @@
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 "That Depends"
 ==
 This package is dependency injection framework for Python, mostly inspired by `python-dependency-injector`.
 
+It is production-ready and gives you the following:
+- Fully-async simple DI framework with IOC-container.
+- Python 3.10-3.12 support.
+- Full coverage by types annotations (mypy in strict mode).
+- FastAPI and Litestar compatibility.
+- Zero dependencies.
+- Overriding dependencies for tests.
+
+# Main characteristics:
+1. Fully async -> means every dependency resolving is async, so you should construct with `await` keyword:
+```python
+from tests.container import DIContainer
+
+async def main():
+    some_dependency = await DIContainer.independent_factory()
+```
+2. No wiring for injections in function arguments -> achieved by decision that only one instance of container is supported
+```python
+from tests import container
+from that_depends import Provide, inject
+
+
+@inject
+async def some_function(
+    independent_factory: container.IndependentFactory = Provide[container.DIContainer.independent_factory],
+) -> None:
+    assert independent_factory.dep1
+```
+
 # Quickstart
 ## Install
 
 ```bash
 pip install that-depends
 ```
 
@@ -179,15 +208,15 @@
     # resource teardown
 
 class DIContainer(BaseContainer):
     sync_resource = providers.Resource(create_sync_resource)
 ```
 
 ### AsyncResource
-- Same as but async generator function is required.
+- Same as `Resource` but async generator function is required.
 ```python
 import typing
 
 from that_depends import BaseContainer, providers
 
 
 async def create_async_resource() -> typing.AsyncIterator[str]:
@@ -231,15 +260,15 @@
     dep2: int
 
 
 class DIContainer(BaseContainer):
     independent_factory = providers.Factory(IndependentFactory, dep1="text", dep2=123)
 ```
 ### AsyncFactory
-- Initialized on every call, as Factory.
+- Initialized on every call, as `Factory`.
 - Async function is required.
 ```python
 import datetime
 
 from that_depends import BaseContainer, providers
 
 
@@ -260,17 +289,7 @@
 
 
 class DIContainer(BaseContainer):
     random_number = providers.Factory(random.random)
     numbers_sequence = providers.List(random_number, random_number)
 ```
 
-# Main decisions:
-1. Every dependency resolving is async, so you should construct with `await` keyword:
-```python
-from tests.container import DIContainer
-
-async def main():
-    some_dependency = await DIContainer.independent_factory()
-```
-2. No containers initialization to avoid wiring -> only one global instance of container is supported
-
```

