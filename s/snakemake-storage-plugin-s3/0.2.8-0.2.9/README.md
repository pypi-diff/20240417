# Comparing `tmp/snakemake_storage_plugin_s3-0.2.8.tar.gz` & `tmp/snakemake_storage_plugin_s3-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakemake_storage_plugin_s3-0.2.8.tar", max compression
+gzip compressed data, was "snakemake_storage_plugin_s3-0.2.9.tar", max compression
```

## Comparing `snakemake_storage_plugin_s3-0.2.8.tar` & `snakemake_storage_plugin_s3-0.2.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1066 2023-12-08 15:50:07.523553 snakemake_storage_plugin_s3-0.2.8/LICENSE
--rw-r--r--   0        0        0       98 2023-12-08 15:50:07.523553 snakemake_storage_plugin_s3-0.2.8/README.md
--rw-r--r--   0        0        0      904 2023-12-08 15:50:07.523553 snakemake_storage_plugin_s3-0.2.8/pyproject.toml
--rw-r--r--   0        0        0    13630 2023-12-08 15:50:07.523553 snakemake_storage_plugin_s3-0.2.8/snakemake_storage_plugin_s3/__init__.py
--rw-r--r--   0        0        0     1102 1970-01-01 00:00:00.000000 snakemake_storage_plugin_s3-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-02-15 20:42:43.198495 snakemake_storage_plugin_s3-0.2.9/LICENSE
+-rw-r--r--   0        0        0      256 2024-02-15 20:42:43.198495 snakemake_storage_plugin_s3-0.2.9/README.md
+-rw-r--r--   0        0        0      984 2024-02-15 20:42:43.198495 snakemake_storage_plugin_s3-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0    13630 2024-02-15 20:42:43.198495 snakemake_storage_plugin_s3-0.2.9/snakemake_storage_plugin_s3/__init__.py
+-rw-r--r--   0        0        0     1250 1970-01-01 00:00:00.000000 snakemake_storage_plugin_s3-0.2.9/PKG-INFO
```

### Comparing `snakemake_storage_plugin_s3-0.2.8/LICENSE` & `snakemake_storage_plugin_s3-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `snakemake_storage_plugin_s3-0.2.8/pyproject.toml` & `snakemake_storage_plugin_s3-0.2.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,26 @@
-[tool.poetry]
-name = "snakemake-storage-plugin-s3"
-version = "0.2.8"
-description = "A Snakemake storage plugin for S3 API storage (AWS S3, MinIO, etc.)"
-authors = ["Johannes Koester <johannes.koester@uni-due.de>"]
-readme = "README.md"
-repository = "https://github.com/snakemake/snakemake-storage-plugin-s3"
-documentation = "https://snakemake.github.io/snakemake-plugin-catalog/plugins/storage/s3.html"
-license = "MIT"
-keywords = ["snakemake", "plugin", "storage", "s3"]
+Metadata-Version: 2.1
+Name: snakemake-storage-plugin-s3
+Version: 0.2.9
+Summary: A Snakemake storage plugin for S3 API storage (AWS S3, MinIO, etc.)
+Home-page: https://github.com/snakemake/snakemake-storage-plugin-s3
+License: MIT
+Keywords: snakemake,plugin,storage,s3
+Author: Johannes Koester
+Author-email: johannes.koester@uni-due.de
+Requires-Python: >=3.11,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: boto3 (>=1.33,<2.0)
+Requires-Dist: botocore (>=1.33,<2.0)
+Requires-Dist: snakemake-interface-common (>=1.14.0,<2.0.0)
+Requires-Dist: snakemake-interface-storage-plugins (>=3.0.0,<4.0.0)
+Project-URL: Documentation, https://snakemake.github.io/snakemake-plugin-catalog/plugins/storage/s3.html
+Project-URL: Repository, https://github.com/snakemake/snakemake-storage-plugin-s3
+Description-Content-Type: text/markdown
 
+# Snakemake storage plugin: s3
 
-[tool.poetry.dependencies]
-python = "^3.11"
-snakemake-interface-common = "^1.14.0"
-snakemake-interface-storage-plugins = "^3.0.0"
-boto3 = "^1.28.55"
-botocore = "^1.31.55"
-
-
-[tool.poetry.group.dev.dependencies]
-black = "^23.9.1"
-flake8 = "^6.1.0"
-coverage = "^7.3.1"
-pytest = "^7.4.2"
-snakemake = {git="https://github.com/snakemake/snakemake.git"}
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+A Snakemake storage plugin for S3 API storage (AWS S3, MinIO, etc.).
+For documentation and usage instructions, see the [Snakemake plugin catalog](https://snakemake.github.io/snakemake-plugin-catalog/plugins/storage/s3.html).
```

### Comparing `snakemake_storage_plugin_s3-0.2.8/snakemake_storage_plugin_s3/__init__.py` & `snakemake_storage_plugin_s3-0.2.9/snakemake_storage_plugin_s3/__init__.py`

 * *Files identical despite different names*

