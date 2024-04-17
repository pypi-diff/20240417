# Comparing `tmp/types-pytz-2024.1.0.20240203.tar.gz` & `tmp/types-pytz-2024.1.0.20240417.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pytz-2024.1.0.20240203.tar", last modified: Sat Feb  3 02:10:33 2024, max compression
+gzip compressed data, was "types-pytz-2024.1.0.20240417.tar", last modified: Wed Apr 17 02:16:54 2024, max compression
```

## Comparing `types-pytz-2024.1.0.20240203.tar` & `types-pytz-2024.1.0.20240417.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 02:10:32.998349 types-pytz-2024.1.0.20240203/
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-02-03 02:10:31.000000 types-pytz-2024.1.0.20240203/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-03 02:10:31.000000 types-pytz-2024.1.0.20240203/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-02-03 02:10:32.998349 types-pytz-2024.1.0.20240203/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 02:10:32.994349 types-pytz-2024.1.0.20240203/pytz-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-03 02:10:31.000000 types-pytz-2024.1.0.20240203/pytz-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-02-03 02:10:21.000000 types-pytz-2024.1.0.20240203/pytz-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-03 02:10:21.000000 types-pytz-2024.1.0.20240203/pytz-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-02-03 02:10:21.000000 types-pytz-2024.1.0.20240203/pytz-stubs/lazy.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-02-03 02:10:21.000000 types-pytz-2024.1.0.20240203/pytz-stubs/reference.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-03 02:10:21.000000 types-pytz-2024.1.0.20240203/pytz-stubs/tzfile.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-02-03 02:10:21.000000 types-pytz-2024.1.0.20240203/pytz-stubs/tzinfo.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-03 02:10:32.998349 types-pytz-2024.1.0.20240203/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-02-03 02:10:31.000000 types-pytz-2024.1.0.20240203/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 02:10:32.998349 types-pytz-2024.1.0.20240203/types_pytz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-02-03 02:10:32.000000 types-pytz-2024.1.0.20240203/types_pytz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-02-03 02:10:32.000000 types-pytz-2024.1.0.20240203/types_pytz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-03 02:10:32.000000 types-pytz-2024.1.0.20240203/types_pytz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-03 02:10:32.000000 types-pytz-2024.1.0.20240203/types_pytz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:54.593075 types-pytz-2024.1.0.20240417/
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-04-17 02:16:52.000000 types-pytz-2024.1.0.20240417/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-17 02:16:52.000000 types-pytz-2024.1.0.20240417/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-17 02:16:54.589075 types-pytz-2024.1.0.20240417/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:54.589075 types-pytz-2024.1.0.20240417/pytz-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-17 02:16:52.000000 types-pytz-2024.1.0.20240417/pytz-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-17 02:16:41.000000 types-pytz-2024.1.0.20240417/pytz-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-17 02:16:41.000000 types-pytz-2024.1.0.20240417/pytz-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-17 02:16:41.000000 types-pytz-2024.1.0.20240417/pytz-stubs/lazy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:52.000000 types-pytz-2024.1.0.20240417/pytz-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-17 02:16:41.000000 types-pytz-2024.1.0.20240417/pytz-stubs/reference.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-17 02:16:41.000000 types-pytz-2024.1.0.20240417/pytz-stubs/tzfile.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-17 02:16:41.000000 types-pytz-2024.1.0.20240417/pytz-stubs/tzinfo.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 02:16:54.593075 types-pytz-2024.1.0.20240417/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-17 02:16:52.000000 types-pytz-2024.1.0.20240417/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:54.589075 types-pytz-2024.1.0.20240417/types_pytz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-17 02:16:54.000000 types-pytz-2024.1.0.20240417/types_pytz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-17 02:16:54.000000 types-pytz-2024.1.0.20240417/types_pytz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 02:16:54.000000 types-pytz-2024.1.0.20240417/types_pytz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-17 02:16:54.000000 types-pytz-2024.1.0.20240417/types_pytz.egg-info/top_level.txt
```

### Comparing `types-pytz-2024.1.0.20240203/CHANGELOG.md` & `types-pytz-2024.1.0.20240417/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 2024.1.0.20240417 (2024-04-17)
+
+Remove remaining bare `Incomplete`s (#11768)
+
+Enable Y065
+
 ## 2024.1.0.20240203 (2024-02-03)
 
 [stubsabot] Bump pytz to 2024.1 (#11355)
 
 ## 2023.4.0.20240130 (2024-01-30)
 
 [stubsabot] Bump pytz to 2023.4 (#11341)
```

### Comparing `types-pytz-2024.1.0.20240203/PKG-INFO` & `types-pytz-2024.1.0.20240417/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pytz
-Version: 2024.1.0.20240203
+Version: 2024.1.0.20240417
 Summary: Typing stubs for pytz
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pytz.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-pytz` aims to provide accurate annotations
 for `pytz==2024.1`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pytz. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `5ce34dc09606aa3fcd09254e6e51c9d68afefe49` and was tested
-with mypy 1.8.0, pyright 1.1.342, and
-pytype 2023.12.18.
+This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

### Comparing `types-pytz-2024.1.0.20240203/pytz-stubs/__init__.pyi` & `types-pytz-2024.1.0.20240417/pytz-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-pytz-2024.1.0.20240203/pytz-stubs/lazy.pyi` & `types-pytz-2024.1.0.20240417/pytz-stubs/lazy.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from _typeshed import Incomplete
 from collections.abc import Iterator, Mapping as DictMixin
+from typing import TypeVar
 
-class LazyDict(DictMixin[str, Incomplete]):
-    data: dict[str, Incomplete] | None
-    def __getitem__(self, key: str) -> Incomplete: ...
+_T = TypeVar("_T")
+_VT = TypeVar("_VT")
+
+class LazyDict(DictMixin[str, _VT]):
+    data: dict[str, _VT] | None
+    def __getitem__(self, key: str) -> _VT: ...
     def __contains__(self, key: object) -> bool: ...
     def __iter__(self) -> Iterator[str]: ...
     def __len__(self) -> int: ...
 
-class LazyList(list[Incomplete]):
+class LazyList(list[_T]):
     # does not return `Self` type:
-    def __new__(cls, fill_iter: Incomplete | None = None) -> LazyList: ...  # noqa: Y034
+    def __new__(cls, fill_iter: Incomplete | None = None) -> LazyList[_T]: ...
 
-class LazySet(set[Incomplete]):
+class LazySet(set[_T]):
     # does not return `Self` type:
-    def __new__(cls, fill_iter: Incomplete | None = None) -> LazySet: ...  # noqa: Y034
+    def __new__(cls, fill_iter: Incomplete | None = None) -> LazySet[_T]: ...
```

### Comparing `types-pytz-2024.1.0.20240203/pytz-stubs/reference.pyi` & `types-pytz-2024.1.0.20240417/pytz-stubs/reference.pyi`

 * *Files identical despite different names*

### Comparing `types-pytz-2024.1.0.20240203/pytz-stubs/tzinfo.pyi` & `types-pytz-2024.1.0.20240417/pytz-stubs/tzinfo.pyi`

 * *Files identical despite different names*

### Comparing `types-pytz-2024.1.0.20240203/setup.py` & `types-pytz-2024.1.0.20240417/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,34 +17,34 @@
 This version of `types-pytz` aims to provide accurate annotations
 for `pytz==2024.1`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pytz. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `5ce34dc09606aa3fcd09254e6e51c9d68afefe49` and was tested
-with mypy 1.8.0, pyright 1.1.342, and
-pytype 2023.12.18.
+This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="2024.1.0.20240203",
+      version="2024.1.0.20240417",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pytz.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['pytz-stubs'],
-      package_data={'pytz-stubs': ['__init__.pyi', 'exceptions.pyi', 'lazy.pyi', 'reference.pyi', 'tzfile.pyi', 'tzinfo.pyi', 'METADATA.toml']},
+      package_data={'pytz-stubs': ['__init__.pyi', 'exceptions.pyi', 'lazy.pyi', 'reference.pyi', 'tzfile.pyi', 'tzinfo.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
```

### Comparing `types-pytz-2024.1.0.20240203/types_pytz.egg-info/PKG-INFO` & `types-pytz-2024.1.0.20240417/types_pytz.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pytz
-Version: 2024.1.0.20240203
+Version: 2024.1.0.20240417
 Summary: Typing stubs for pytz
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pytz.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-pytz` aims to provide accurate annotations
 for `pytz==2024.1`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pytz. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `5ce34dc09606aa3fcd09254e6e51c9d68afefe49` and was tested
-with mypy 1.8.0, pyright 1.1.342, and
-pytype 2023.12.18.
+This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

