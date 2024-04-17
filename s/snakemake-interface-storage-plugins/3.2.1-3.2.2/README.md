# Comparing `tmp/snakemake_interface_storage_plugins-3.2.1.tar.gz` & `tmp/snakemake_interface_storage_plugins-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakemake_interface_storage_plugins-3.2.1.tar", max compression
+gzip compressed data, was "snakemake_interface_storage_plugins-3.2.2.tar", max compression
```

## Comparing `snakemake_interface_storage_plugins-3.2.1.tar` & `snakemake_interface_storage_plugins-3.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1076 2024-04-16 07:39:00.854762 snakemake_interface_storage_plugins-3.2.1/LICENSE
--rw-r--r--   0        0        0     8633 2024-04-16 07:39:00.854762 snakemake_interface_storage_plugins-3.2.1/README.md
--rw-r--r--   0        0        0      911 2024-04-16 07:39:00.854762 snakemake_interface_storage_plugins-3.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 07:39:00.854762 snakemake_interface_storage_plugins-3.2.1/snakemake_interface_storage_plugins/__init__.py
--rw-r--r--   0        0        0      525 2024-04-16 07:39:00.854762 snakemake_interface_storage_plugins-3.2.1/snakemake_interface_storage_plugins/common.py
--rw-r--r--   0        0        0     2858 2024-04-16 07:39:00.854762 snakemake_interface_storage_plugins-3.2.1/snakemake_interface_storage_plugins/io.py
--rw-r--r--   0        0        0     2041 2024-04-16 07:39:00.854762 snakemake_interface_storage_plugins-3.2.1/snakemake_interface_storage_plugins/registry/__init__.py
--rw-r--r--   0        0        0     1315 2024-04-16 07:39:00.854762 snakemake_interface_storage_plugins-3.2.1/snakemake_interface_storage_plugins/registry/plugin.py
--rw-r--r--   0        0        0      898 2024-04-16 07:39:00.854762 snakemake_interface_storage_plugins-3.2.1/snakemake_interface_storage_plugins/settings.py
--rw-r--r--   0        0        0     7389 2024-04-16 07:39:00.854762 snakemake_interface_storage_plugins-3.2.1/snakemake_interface_storage_plugins/storage_object.py
--rw-r--r--   0        0        0     5155 2024-04-16 07:39:00.854762 snakemake_interface_storage_plugins-3.2.1/snakemake_interface_storage_plugins/storage_provider.py
--rw-r--r--   0        0        0     4191 2024-04-16 07:39:00.854762 snakemake_interface_storage_plugins-3.2.1/snakemake_interface_storage_plugins/tests.py
--rw-r--r--   0        0        0     9369 1970-01-01 00:00:00.000000 snakemake_interface_storage_plugins-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-17 10:36:42.234379 snakemake_interface_storage_plugins-3.2.2/LICENSE
+-rw-r--r--   0        0        0     8633 2024-04-17 10:36:42.234379 snakemake_interface_storage_plugins-3.2.2/README.md
+-rw-r--r--   0        0        0      911 2024-04-17 10:36:42.234379 snakemake_interface_storage_plugins-3.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-17 10:36:42.234379 snakemake_interface_storage_plugins-3.2.2/snakemake_interface_storage_plugins/__init__.py
+-rw-r--r--   0        0        0      525 2024-04-17 10:36:42.234379 snakemake_interface_storage_plugins-3.2.2/snakemake_interface_storage_plugins/common.py
+-rw-r--r--   0        0        0     2858 2024-04-17 10:36:42.234379 snakemake_interface_storage_plugins-3.2.2/snakemake_interface_storage_plugins/io.py
+-rw-r--r--   0        0        0     2041 2024-04-17 10:36:42.234379 snakemake_interface_storage_plugins-3.2.2/snakemake_interface_storage_plugins/registry/__init__.py
+-rw-r--r--   0        0        0     1315 2024-04-17 10:36:42.234379 snakemake_interface_storage_plugins-3.2.2/snakemake_interface_storage_plugins/registry/plugin.py
+-rw-r--r--   0        0        0      898 2024-04-17 10:36:42.234379 snakemake_interface_storage_plugins-3.2.2/snakemake_interface_storage_plugins/settings.py
+-rw-r--r--   0        0        0     7389 2024-04-17 10:36:42.238379 snakemake_interface_storage_plugins-3.2.2/snakemake_interface_storage_plugins/storage_object.py
+-rw-r--r--   0        0        0     5155 2024-04-17 10:36:42.238379 snakemake_interface_storage_plugins-3.2.2/snakemake_interface_storage_plugins/storage_provider.py
+-rw-r--r--   0        0        0     4353 2024-04-17 10:36:42.238379 snakemake_interface_storage_plugins-3.2.2/snakemake_interface_storage_plugins/tests.py
+-rw-r--r--   0        0        0     9369 1970-01-01 00:00:00.000000 snakemake_interface_storage_plugins-3.2.2/PKG-INFO
```

### Comparing `snakemake_interface_storage_plugins-3.2.1/LICENSE` & `snakemake_interface_storage_plugins-3.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `snakemake_interface_storage_plugins-3.2.1/README.md` & `snakemake_interface_storage_plugins-3.2.2/README.md`

 * *Files identical despite different names*

### Comparing `snakemake_interface_storage_plugins-3.2.1/pyproject.toml` & `snakemake_interface_storage_plugins-3.2.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snakemake-interface-storage-plugins"
-version = "3.2.1"
+version = "3.2.2"
 description = "This package provides a stable interface for interactions between Snakemake and its storage plugins."
 authors = ["Johannes Koester <johannes.koester@uni-due.de>"]
 readme = "README.md"
 homepage = "https://github.com/snakemake/snakemake-interface-storage-plugins"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `snakemake_interface_storage_plugins-3.2.1/snakemake_interface_storage_plugins/common.py` & `snakemake_interface_storage_plugins-3.2.2/snakemake_interface_storage_plugins/common.py`

 * *Files identical despite different names*

### Comparing `snakemake_interface_storage_plugins-3.2.1/snakemake_interface_storage_plugins/io.py` & `snakemake_interface_storage_plugins-3.2.2/snakemake_interface_storage_plugins/io.py`

 * *Files identical despite different names*

### Comparing `snakemake_interface_storage_plugins-3.2.1/snakemake_interface_storage_plugins/registry/__init__.py` & `snakemake_interface_storage_plugins-3.2.2/snakemake_interface_storage_plugins/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `snakemake_interface_storage_plugins-3.2.1/snakemake_interface_storage_plugins/registry/plugin.py` & `snakemake_interface_storage_plugins-3.2.2/snakemake_interface_storage_plugins/registry/plugin.py`

 * *Files identical despite different names*

### Comparing `snakemake_interface_storage_plugins-3.2.1/snakemake_interface_storage_plugins/settings.py` & `snakemake_interface_storage_plugins-3.2.2/snakemake_interface_storage_plugins/settings.py`

 * *Files identical despite different names*

### Comparing `snakemake_interface_storage_plugins-3.2.1/snakemake_interface_storage_plugins/storage_object.py` & `snakemake_interface_storage_plugins-3.2.2/snakemake_interface_storage_plugins/storage_object.py`

 * *Files identical despite different names*

### Comparing `snakemake_interface_storage_plugins-3.2.1/snakemake_interface_storage_plugins/storage_provider.py` & `snakemake_interface_storage_plugins-3.2.2/snakemake_interface_storage_plugins/storage_provider.py`

 * *Files identical despite different names*

### Comparing `snakemake_interface_storage_plugins-3.2.1/snakemake_interface_storage_plugins/tests.py` & `snakemake_interface_storage_plugins-3.2.2/snakemake_interface_storage_plugins/tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,42 +62,51 @@
         assert not (
             self.store_only and self.retrieve_only
         ), "store_only and retrieve_only may not be True at the same time"
 
         obj = self._get_obj(tmp_path, self.get_query(tmp_path))
 
         stored = False
+
+        if directory:
+            dirpath = obj.local_path()
+            filepath = dirpath / "test.txt"
+        else:
+            dirpath = obj.local_path().parent
+            filepath = obj.local_path()
+
         try:
             if not self.retrieve_only:
-                if directory:
-                    dirpath = obj.local_path()
-                    filepath = dirpath / "test.txt"
-                else:
-                    dirpath = obj.local_path().parent
-                    filepath = obj.local_path()
-                shutil.rmtree(dirpath, ignore_errors=True)
+                if dirpath.exists():
+                    if dirpath.is_dir():
+                        shutil.rmtree(dirpath)
+                    else:
+                        dirpath.unlink()
                 dirpath.mkdir(parents=True, exist_ok=True)
                 with open(filepath, "w") as f:
                     f.write("test")
                     f.flush()
                 obj.store_object()
                 stored = True
-                obj.local_path().unlink()
+                if directory:
+                    shutil.rmtree(dirpath)
+                else:
+                    filepath.unlink()
 
             assert obj.exists()
 
             assert isinstance(obj.mtime(), (float, int))
 
             self._test_inventory(obj)
 
             if self.touch:
                 obj.touch()
 
             if not self.store_only:
-                obj.local_path().parent.mkdir(parents=True, exist_ok=True)
+                dirpath.mkdir(parents=True, exist_ok=True)
                 obj.retrieve_object()
 
         finally:
             if not self.retrieve_only and stored and self.delete:
                 obj.remove()
 
     def test_storage_not_existing(self, tmp_path):
```

### Comparing `snakemake_interface_storage_plugins-3.2.1/PKG-INFO` & `snakemake_interface_storage_plugins-3.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakemake-interface-storage-plugins
-Version: 3.2.1
+Version: 3.2.2
 Summary: This package provides a stable interface for interactions between Snakemake and its storage plugins.
 Home-page: https://github.com/snakemake/snakemake-interface-storage-plugins
 Author: Johannes Koester
 Author-email: johannes.koester@uni-due.de
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

