# Comparing `tmp/types-python-crontab-3.0.0.20240106.tar.gz` & `tmp/types-python-crontab-3.0.0.20240417.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-python-crontab-3.0.0.20240106.tar", last modified: Sat Jan  6 02:21:57 2024, max compression
+gzip compressed data, was "types-python-crontab-3.0.0.20240417.tar", last modified: Wed Apr 17 02:16:58 2024, max compression
```

## Comparing `types-python-crontab-3.0.0.20240106.tar` & `types-python-crontab-3.0.0.20240417.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 02:21:57.591850 types-python-crontab-3.0.0.20240106/
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-01-06 02:21:57.000000 types-python-crontab-3.0.0.20240106/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-06 02:21:57.000000 types-python-crontab-3.0.0.20240106/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-01-06 02:21:57.591850 types-python-crontab-3.0.0.20240106/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 02:21:57.591850 types-python-crontab-3.0.0.20240106/cronlog-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-01-06 02:21:57.000000 types-python-crontab-3.0.0.20240106/cronlog-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-01-06 02:21:57.000000 types-python-crontab-3.0.0.20240106/cronlog-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 02:21:57.591850 types-python-crontab-3.0.0.20240106/crontab-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-01-06 02:21:57.000000 types-python-crontab-3.0.0.20240106/crontab-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)    11501 2024-01-06 02:21:57.000000 types-python-crontab-3.0.0.20240106/crontab-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 02:21:57.591850 types-python-crontab-3.0.0.20240106/crontabs-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-01-06 02:21:57.000000 types-python-crontab-3.0.0.20240106/crontabs-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-01-06 02:21:57.000000 types-python-crontab-3.0.0.20240106/crontabs-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-06 02:21:57.591850 types-python-crontab-3.0.0.20240106/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-01-06 02:21:57.000000 types-python-crontab-3.0.0.20240106/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 02:21:57.591850 types-python-crontab-3.0.0.20240106/types_python_crontab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-01-06 02:21:57.000000 types-python-crontab-3.0.0.20240106/types_python_crontab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-01-06 02:21:57.000000 types-python-crontab-3.0.0.20240106/types_python_crontab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-06 02:21:57.000000 types-python-crontab-3.0.0.20240106/types_python_crontab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-06 02:21:57.000000 types-python-crontab-3.0.0.20240106/types_python_crontab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:58.733122 types-python-crontab-3.0.0.20240417/
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-17 02:16:58.729122 types-python-crontab-3.0.0.20240417/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:58.729122 types-python-crontab-3.0.0.20240417/cronlog-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/cronlog-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/cronlog-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/cronlog-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:58.729122 types-python-crontab-3.0.0.20240417/crontab-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/crontab-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/crontab-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/crontab-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:58.729122 types-python-crontab-3.0.0.20240417/crontabs-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/crontabs-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/crontabs-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/crontabs-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 02:16:58.733122 types-python-crontab-3.0.0.20240417/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:58.729122 types-python-crontab-3.0.0.20240417/types_python_crontab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/types_python_crontab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/types_python_crontab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/types_python_crontab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-17 02:16:58.000000 types-python-crontab-3.0.0.20240417/types_python_crontab.egg-info/top_level.txt
```

### Comparing `types-python-crontab-3.0.0.20240106/CHANGELOG.md` & `types-python-crontab-3.0.0.20240417/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 3.0.0.20240417 (2024-04-17)
+
+Remove remaining bare `Incomplete`s (#11768)
+
+Enable Y065
+
 ## 3.0.0.20240106 (2024-01-06)
 
 Update typing_extensions imports in third-party stubs (#11245)
 
 ## 3.0.0.1 (2023-07-20)
 
 Add a few more upstream_repository URLs (#10489)
```

### Comparing `types-python-crontab-3.0.0.20240106/PKG-INFO` & `types-python-crontab-3.0.0.20240417/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-python-crontab
-Version: 3.0.0.20240106
+Version: 3.0.0.20240417
 Summary: Typing stubs for python-crontab
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/python-crontab.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-python-crontab` aims to provide accurate annotations
 for `python-crontab==3.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/python-crontab. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `1de5830a2703936a96a126248227d5c7db883674` and was tested
-with mypy 1.8.0, pyright 1.1.342, and
-pytype 2023.12.18.
+This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

### Comparing `types-python-crontab-3.0.0.20240106/cronlog-stubs/__init__.pyi` & `types-python-crontab-3.0.0.20240417/cronlog-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-python-crontab-3.0.0.20240106/crontab-stubs/__init__.pyi` & `types-python-crontab-3.0.0.20240417/crontab-stubs/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -154,17 +154,17 @@
     @overload
     def frequency_at_hour(self, year: int, month: int, day: int, hour: int) -> int: ...
     @overload
     def frequency_at_hour(self, year: None = None, month: None = None, day: None = None, hour: None = None) -> int: ...
     def run_pending(self, now: datetime | None = ...) -> int | str: ...
     def run(self) -> str: ...
     # TODO: use types from `croniter` module here:
-    def schedule(self, date_from: datetime | None = ...) -> Incomplete: ...
+    def schedule(self, date_from: datetime | None = ...): ...
     # TODO: use types from `cron_descriptor` here:
-    def description(self, **kw: Incomplete) -> Incomplete: ...
+    def description(self, **kw): ...
     @property
     def log(self) -> CronLog: ...
     @property
     def minute(self) -> int | str: ...
     @property
     def minutes(self) -> int | str: ...
     @property
@@ -288,10 +288,10 @@
     def __int__(self) -> int: ...
 
 # TODO: make generic
 class OrderedVariableList(OrderedDict[Incomplete, Incomplete]):
     job: Incomplete
     def __init__(self, *args: Any, **kw: Any) -> None: ...
     @property
-    def previous(self) -> Incomplete: ...
+    def previous(self): ...
     def all(self) -> Self: ...
-    def __getitem__(self, key: Incomplete) -> Incomplete: ...
+    def __getitem__(self, key): ...
```

### Comparing `types-python-crontab-3.0.0.20240106/crontabs-stubs/__init__.pyi` & `types-python-crontab-3.0.0.20240417/crontabs-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-python-crontab-3.0.0.20240106/setup.py` & `types-python-crontab-3.0.0.20240417/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,34 +17,34 @@
 This version of `types-python-crontab` aims to provide accurate annotations
 for `python-crontab==3.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/python-crontab. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `1de5830a2703936a96a126248227d5c7db883674` and was tested
-with mypy 1.8.0, pyright 1.1.342, and
-pytype 2023.12.18.
+This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="3.0.0.20240106",
+      version="3.0.0.20240417",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/python-crontab.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
-      packages=['crontabs-stubs', 'cronlog-stubs', 'crontab-stubs'],
-      package_data={'crontabs-stubs': ['__init__.pyi', 'METADATA.toml'], 'cronlog-stubs': ['__init__.pyi', 'METADATA.toml'], 'crontab-stubs': ['__init__.pyi', 'METADATA.toml']},
+      packages=['crontab-stubs', 'crontabs-stubs', 'cronlog-stubs'],
+      package_data={'crontab-stubs': ['__init__.pyi', 'METADATA.toml', 'py.typed'], 'crontabs-stubs': ['__init__.pyi', 'METADATA.toml', 'py.typed'], 'cronlog-stubs': ['__init__.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
```

### Comparing `types-python-crontab-3.0.0.20240106/types_python_crontab.egg-info/PKG-INFO` & `types-python-crontab-3.0.0.20240417/types_python_crontab.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-python-crontab
-Version: 3.0.0.20240106
+Version: 3.0.0.20240417
 Summary: Typing stubs for python-crontab
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/python-crontab.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-python-crontab` aims to provide accurate annotations
 for `python-crontab==3.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/python-crontab. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `1de5830a2703936a96a126248227d5c7db883674` and was tested
-with mypy 1.8.0, pyright 1.1.342, and
-pytype 2023.12.18.
+This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

