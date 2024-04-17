# Comparing `tmp/snakemake_storage_plugin_fs-1.0.2.tar.gz` & `tmp/snakemake_storage_plugin_fs-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakemake_storage_plugin_fs-1.0.2.tar", max compression
+gzip compressed data, was "snakemake_storage_plugin_fs-1.0.3.tar", max compression
```

## Comparing `snakemake_storage_plugin_fs-1.0.2.tar` & `snakemake_storage_plugin_fs-1.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1066 2024-04-16 15:09:39.707158 snakemake_storage_plugin_fs-1.0.2/LICENSE
--rw-r--r--   0        0        0      139 2024-04-16 15:09:39.707158 snakemake_storage_plugin_fs-1.0.2/README.md
--rw-r--r--   0        0        0      948 2024-04-16 15:09:39.707158 snakemake_storage_plugin_fs-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     9268 2024-04-16 15:09:39.707158 snakemake_storage_plugin_fs-1.0.2/snakemake_storage_plugin_fs/__init__.py
--rw-r--r--   0        0        0     1185 1970-01-01 00:00:00.000000 snakemake_storage_plugin_fs-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-17 11:42:38.955679 snakemake_storage_plugin_fs-1.0.3/LICENSE
+-rw-r--r--   0        0        0      139 2024-04-17 11:42:38.955679 snakemake_storage_plugin_fs-1.0.3/README.md
+-rw-r--r--   0        0        0      948 2024-04-17 11:42:38.955679 snakemake_storage_plugin_fs-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     9266 2024-04-17 11:42:38.955679 snakemake_storage_plugin_fs-1.0.3/snakemake_storage_plugin_fs/__init__.py
+-rw-r--r--   0        0        0     1185 1970-01-01 00:00:00.000000 snakemake_storage_plugin_fs-1.0.3/PKG-INFO
```

### Comparing `snakemake_storage_plugin_fs-1.0.2/LICENSE` & `snakemake_storage_plugin_fs-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `snakemake_storage_plugin_fs-1.0.2/pyproject.toml` & `snakemake_storage_plugin_fs-1.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "snakemake-storage-plugin-fs"
-version = "1.0.2"
+version = "1.0.3"
 description = " A Snakemake storage plugin that reads and writes from a locally mounted filesystem using rsync"
 authors = ["Johannes Koester <johannes.koester@uni-due.de>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/snakemake/snakemake-storage-plugin-fs"
 documentation = "https://snakemake.github.io/snakemake-plugin-catalog/plugins/storage/fs.html"
 keywords = ["snakemake", "plugin", "storage", "filesystem", "rsync"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 snakemake-interface-common = "^1.17.0"
-snakemake-interface-storage-plugins = "^3.1.0"
+snakemake-interface-storage-plugins = "^3.2.2"
 sysrsync = "^1.1.1"
 reretry = "^0.11.8"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.11.0"
 flake8 = "^6.1.0"
```

### Comparing `snakemake_storage_plugin_fs-1.0.2/snakemake_storage_plugin_fs/__init__.py` & `snakemake_storage_plugin_fs-1.0.3/snakemake_storage_plugin_fs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,24 +83,24 @@
 
         # disallow queries that are URL like
         parsed = urlparse(query)
         if parsed.scheme:
             return StorageQueryValidationResult(
                 query=query,
                 valid=False,
-                message="Query is URL-like, but should be a system path instead.",
+                reason="Query is URL-like, but should be a system path instead.",
             )
 
         try:
             Path(query)
         except Exception:
             return StorageQueryValidationResult(
                 query=query,
                 valid=False,
-                message="Query is not a valid path.",
+                reason="Query is not a valid path.",
             )
         return StorageQueryValidationResult(
             query=query,
             valid=True,
         )
 
     def list_objects(self, query: Any) -> Iterable[str]:
```

### Comparing `snakemake_storage_plugin_fs-1.0.2/PKG-INFO` & `snakemake_storage_plugin_fs-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: snakemake-storage-plugin-fs
-Version: 1.0.2
+Version: 1.0.3
 Summary:  A Snakemake storage plugin that reads and writes from a locally mounted filesystem using rsync
 Home-page: https://github.com/snakemake/snakemake-storage-plugin-fs
 License: MIT
 Keywords: snakemake,plugin,storage,filesystem,rsync
 Author: Johannes Koester
 Author-email: johannes.koester@uni-due.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: reretry (>=0.11.8,<0.12.0)
 Requires-Dist: snakemake-interface-common (>=1.17.0,<2.0.0)
-Requires-Dist: snakemake-interface-storage-plugins (>=3.1.0,<4.0.0)
+Requires-Dist: snakemake-interface-storage-plugins (>=3.2.2,<4.0.0)
 Requires-Dist: sysrsync (>=1.1.1,<2.0.0)
 Project-URL: Documentation, https://snakemake.github.io/snakemake-plugin-catalog/plugins/storage/fs.html
 Project-URL: Repository, https://github.com/snakemake/snakemake-storage-plugin-fs
 Description-Content-Type: text/markdown
 
 # Snakemake storage plugin: fs
```

