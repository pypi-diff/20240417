# Comparing `tmp/charmcraftcache-0.3.0.tar.gz` & `tmp/charmcraftcache-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "charmcraftcache-0.3.0.tar", max compression
+gzip compressed data, was "charmcraftcache-0.3.1.tar", max compression
```

## Comparing `charmcraftcache-0.3.0.tar` & `charmcraftcache-0.3.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2024-03-04 12:21:27.396240 charmcraftcache-0.3.0/LICENSE
--rw-r--r--   0        0        0     1931 2024-03-04 12:21:27.396240 charmcraftcache-0.3.0/README.md
--rw-r--r--   0        0        0        0 2024-03-04 12:21:27.396240 charmcraftcache-0.3.0/charmcraftcache/__init__.py
--rw-r--r--   0        0        0    18299 2024-03-04 12:21:27.396240 charmcraftcache-0.3.0/charmcraftcache/main.py
--rw-r--r--   0        0        0      619 2024-03-04 12:21:27.400240 charmcraftcache-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2574 1970-01-01 00:00:00.000000 charmcraftcache-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-17 13:33:50.649416 charmcraftcache-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1931 2024-04-17 13:33:50.649416 charmcraftcache-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 13:33:50.649416 charmcraftcache-0.3.1/charmcraftcache/__init__.py
+-rw-r--r--   0        0        0    18299 2024-04-17 13:33:50.649416 charmcraftcache-0.3.1/charmcraftcache/main.py
+-rw-r--r--   0        0        0      619 2024-04-17 13:33:50.649416 charmcraftcache-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2574 1970-01-01 00:00:00.000000 charmcraftcache-0.3.1/PKG-INFO
```

### Comparing `charmcraftcache-0.3.0/LICENSE` & `charmcraftcache-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `charmcraftcache-0.3.0/README.md` & `charmcraftcache-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `charmcraftcache-0.3.0/charmcraftcache/main.py` & `charmcraftcache-0.3.1/charmcraftcache/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -298,15 +298,15 @@
     # Example: v1
     hub_version = release_name.split("-")[-1]
     clean_cache_if_version_changed(VersionType.CHARMCRAFTCACHE_HUB, hub_version)
     missing_wheels = 0
     assets = {}
     # TODO: remove hardcoded path
     build_base_subdirectory = (
-        charmcraft_cache_subdirectory / "charmcraft-buildd-base-v5.0"
+        charmcraft_cache_subdirectory / "charmcraft-buildd-base-v8.0"
     )
     build_base_subdirectory.mkdir(parents=True, exist_ok=True)
     logger.debug(
         f'Selecting wheels for Ubuntu versions ({architecture}): {", ".join(bases)}'
     )
     for dependency in dependencies:
         for asset in response_data["assets"]:
```

### Comparing `charmcraftcache-0.3.0/pyproject.toml` & `charmcraftcache-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "charmcraftcache"
-version = "0.3.0"
+version = "0.3.1"
 description = "Fast first-time builds for charmcraft"
 authors = ["Carl Csaposs <carl.csaposs@canonical.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 ccc = "charmcraftcache.main:app"
 charmcraftcache = "charmcraftcache.main:app"
```

### Comparing `charmcraftcache-0.3.0/PKG-INFO` & `charmcraftcache-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: charmcraftcache
-Version: 0.3.0
+Version: 0.3.1
 Summary: Fast first-time builds for charmcraft
 Author: Carl Csaposs
 Author-email: carl.csaposs@canonical.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

