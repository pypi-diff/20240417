# Comparing `tmp/ubump-0.1.8.tar.gz` & `tmp/ubump-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubump-0.1.8.tar", last modified: Fri Feb 23 23:25:15 2024, max compression
+gzip compressed data, was "ubump-0.1.9.tar", last modified: Mon Feb 26 11:26:18 2024, max compression
```

## Comparing `ubump-0.1.8.tar` & `ubump-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,7 @@
--rw-r--r--   0        0        0     1058 2024-02-23 16:09:08.919403 ubump-0.1.8/LICENSE
--rw-r--r--   0        0        0      987 2024-02-23 23:09:14.486895 ubump-0.1.8/README.md
--rw-r--r--   0        0        0     1384 2024-02-23 23:25:15.865221 ubump-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      139 2024-02-23 16:19:21.156909 ubump-0.1.8/src/ubump/__init__.py
--rw-r--r--   0        0        0    12773 2024-02-23 23:23:14.189835 ubump-0.1.8/src/ubump/main.py
--rw-r--r--   0        0        0       37 2024-02-23 12:22:55.918252 ubump-0.1.8/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2024-02-23 12:22:55.918344 ubump-0.1.8/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2024-02-23 12:22:55.918154 ubump-0.1.8/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0       41 2024-02-23 12:22:55.918557 ubump-0.1.8/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0       35 2024-02-23 12:24:17.249632 ubump-0.1.8/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2024-02-23 12:24:17.249838 ubump-0.1.8/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      241 2024-02-23 12:24:21.620772 ubump-0.1.8/tests/test_config.py
--rw-r--r--   0        0        0     3196 1970-01-01 00:00:00.000000 ubump-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-02-26 11:26:04.390501 ubump-0.1.9/LICENSE
+-rw-r--r--   0        0        0      987 2024-02-26 11:26:04.390501 ubump-0.1.9/README.md
+-rw-r--r--   0        0        0     1408 2024-02-26 11:26:18.770397 ubump-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      139 2024-02-26 11:26:04.390501 ubump-0.1.9/src/ubump/__init__.py
+-rw-r--r--   0        0        0    12774 2024-02-26 11:26:04.390501 ubump-0.1.9/src/ubump/main.py
+-rw-r--r--   0        0        0      221 2024-02-26 11:26:04.390501 ubump-0.1.9/tests/test_config.py
+-rw-r--r--   0        0        0     3196 1970-01-01 00:00:00.000000 ubump-0.1.9/PKG-INFO
```

### Comparing `ubump-0.1.8/LICENSE` & `ubump-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ubump-0.1.8/README.md` & `ubump-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ubump-0.1.8/pyproject.toml` & `ubump-0.1.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ubump"
-version = "0.1.8"
+version = "0.1.9"
 description = "Yet another bump tool"
 keywords = [
     "bump",
     "bumpversion",
     "bump2version",
     "bump-version",
     "bumper",
@@ -52,14 +52,15 @@
 
 [tool.pdm]
 distribution = true
 
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest~=8.0.1",
+    "requests>=2.31.0",
 ]
 
 [tool.ubump]
 template = "v${major}.${minor}.${patch}"
 message = "Bump to ${version}"
 tag = true
 files = [
```

### Comparing `ubump-0.1.8/src/ubump/main.py` & `ubump-0.1.9/src/ubump/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from typing import Optional, NamedTuple, Self
 
 import tomlkit
 from packaging.version import parse
 from tomlkit.exceptions import TOMLKitError
 
 NAME = "ubump"
-VERSION = "v0.1.8"
+VERSION = "v0.1.9"
 
 logging.basicConfig(level=logging.INFO, format="%(levelname)s - %(message)s")
 logger = logging.getLogger(NAME)
 logger.setLevel(logging.DEBUG if sys.flags.debug else logging.INFO)
 
 
 class ConfigError(ValueError):
@@ -75,15 +75,15 @@
             tag: Optional[bool] = None,
             files: Optional[list[str]] = None
     ):
         self._version = version
         self._template = template
         self._files = files or []
         self._tag = tag or True
-        self._message = message or "Bump to {version}"
+        self._message = message or "Bump to ${version}"
 
     @property
     def version(self) -> Version:
         return self._version
 
     @property
     def str_version(self) -> str:
```

### Comparing `ubump-0.1.8/PKG-INFO` & `ubump-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubump
-Version: 0.1.8
+Version: 0.1.9
 Summary: Yet another bump tool
 Keywords: bump bumpversion bump2version bump-version bumper bumping version versioning
 Home-page: https://github.com/vd2org/ubump
 Author-Email: vd <ubump@vd2.org>
 License: Copyright 2024 Vd <ubump@vd2.org>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```

