# Comparing `tmp/composio_core-0.2.5.tar.gz` & `tmp/composio_core-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.2.5.tar", last modified: Tue Apr 16 12:59:39 2024, max compression
+gzip compressed data, was "composio_core-0.2.6.tar", last modified: Tue Apr 16 13:03:22 2024, max compression
```

## Comparing `composio_core-0.2.5.tar` & `composio_core-0.2.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-16 12:59:39.290352 composio_core-0.2.5/
--rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.2.5/MANIFEST.in
--rw-r--r--   0 utkarsh    (501) staff       (20)      796 2024-04-16 12:59:39.290114 composio_core-0.2.5/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.2.5/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-16 12:59:39.287570 composio_core-0.2.5/composio/
--rw-r--r--   0 utkarsh    (501) staff       (20)      159 2024-04-12 09:34:06.000000 composio_core-0.2.5/composio/__init__.py
--rwxr-xr-x   0 utkarsh    (501) staff       (20)    22056 2024-04-15 14:10:00.000000 composio_core-0.2.5/composio/composio_cli.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-16 12:59:39.288816 composio_core-0.2.5/composio/sdk/
--rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.2.5/composio/sdk/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     6837 2024-04-15 14:05:59.000000 composio_core-0.2.5/composio/sdk/core.py
--rw-r--r--   0 utkarsh    (501) staff       (20)    10226 2024-04-12 13:08:03.000000 composio_core-0.2.5/composio/sdk/enums.py
--rw-r--r--   0 utkarsh    (501) staff       (20)    19301 2024-04-16 12:53:07.000000 composio_core-0.2.5/composio/sdk/sdk.py
--rw-r--r--   0 utkarsh    (501) staff       (20)        0 2024-04-12 13:36:37.000000 composio_core-0.2.5/composio/sdk/shared.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     1358 2024-04-15 14:06:14.000000 composio_core-0.2.5/composio/sdk/storage.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     3328 2024-04-12 09:33:50.000000 composio_core-0.2.5/composio/sdk/utils.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-16 12:59:39.289863 composio_core-0.2.5/composio_core.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)      796 2024-04-16 12:59:39.000000 composio_core-0.2.5/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      489 2024-04-16 12:59:39.000000 composio_core-0.2.5/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-16 12:59:39.000000 composio_core-0.2.5/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-16 12:59:39.000000 composio_core-0.2.5/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      103 2024-04-16 12:59:39.000000 composio_core-0.2.5/composio_core.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-16 12:59:39.000000 composio_core-0.2.5/composio_core.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      528 2024-04-12 15:10:44.000000 composio_core-0.2.5/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)      130 2024-04-12 15:11:16.000000 composio_core-0.2.5/requirements.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-16 12:59:39.290395 composio_core-0.2.5/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)     1127 2024-04-16 12:59:30.000000 composio_core-0.2.5/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-16 13:03:22.043270 composio_core-0.2.6/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.2.6/MANIFEST.in
+-rw-r--r--   0 utkarsh    (501) staff       (20)      796 2024-04-16 13:03:22.043032 composio_core-0.2.6/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.2.6/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-16 13:03:22.040225 composio_core-0.2.6/composio/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      159 2024-04-12 09:34:06.000000 composio_core-0.2.6/composio/__init__.py
+-rwxr-xr-x   0 utkarsh    (501) staff       (20)    22056 2024-04-15 14:10:00.000000 composio_core-0.2.6/composio/composio_cli.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-16 13:03:22.041748 composio_core-0.2.6/composio/sdk/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.2.6/composio/sdk/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     6837 2024-04-15 14:05:59.000000 composio_core-0.2.6/composio/sdk/core.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)    10226 2024-04-12 13:08:03.000000 composio_core-0.2.6/composio/sdk/enums.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)    19329 2024-04-16 13:03:06.000000 composio_core-0.2.6/composio/sdk/sdk.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)        0 2024-04-12 13:36:37.000000 composio_core-0.2.6/composio/sdk/shared.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     1358 2024-04-15 14:06:14.000000 composio_core-0.2.6/composio/sdk/storage.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3328 2024-04-12 09:33:50.000000 composio_core-0.2.6/composio/sdk/utils.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-16 13:03:22.042800 composio_core-0.2.6/composio_core.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      796 2024-04-16 13:03:22.000000 composio_core-0.2.6/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      489 2024-04-16 13:03:22.000000 composio_core-0.2.6/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-16 13:03:22.000000 composio_core-0.2.6/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-16 13:03:22.000000 composio_core-0.2.6/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      103 2024-04-16 13:03:22.000000 composio_core-0.2.6/composio_core.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-16 13:03:22.000000 composio_core-0.2.6/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      528 2024-04-12 15:10:44.000000 composio_core-0.2.6/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)      130 2024-04-12 15:11:16.000000 composio_core-0.2.6/requirements.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-16 13:03:22.043312 composio_core-0.2.6/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)     1127 2024-04-16 13:03:15.000000 composio_core-0.2.6/setup.py
```

### Comparing `composio_core-0.2.5/PKG-INFO` & `composio_core-0.2.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.2.5
+Version: 0.2.6
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.2.5/composio/composio_cli.py` & `composio_core-0.2.6/composio/composio_cli.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.2.5/composio/sdk/core.py` & `composio_core-0.2.6/composio/sdk/core.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.2.5/composio/sdk/enums.py` & `composio_core-0.2.6/composio/sdk/enums.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.2.5/composio/sdk/sdk.py` & `composio_core-0.2.6/composio/sdk/sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,15 +356,15 @@
     def get_connected_accounts(
         self, entity_id: Union[list[str], str] = None, showActiveOnly: bool = None
     ) -> list[ConnectedAccount]:
         query_params = {}
         if entity_id is not None:
             query_params['user_uuid'] = entity_id if isinstance(entity_id, str) else ",".join(entity_id)
         if showActiveOnly:
-            query_params['showActiveOnly'] = showActiveOnly
+            query_params['showActiveOnly'] = str("true" if showActiveOnly else "false")
 
         query_string = "&".join([f"{key}={value}" for key, value in query_params.items()])
         url = f"{self.base_url}/v1/connectedAccounts"
         if query_string:
             url += f"?{query_string}"
 
         resp = self.http_client.get(url)
```

### Comparing `composio_core-0.2.5/composio/sdk/storage.py` & `composio_core-0.2.6/composio/sdk/storage.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.2.5/composio/sdk/utils.py` & `composio_core-0.2.6/composio/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.2.5/composio_core.egg-info/PKG-INFO` & `composio_core-0.2.6/composio_core.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.2.5
+Version: 0.2.6
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.2.5/pyproject.toml` & `composio_core-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `composio_core-0.2.5/setup.py` & `composio_core-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     """Customized setuptools install command."""
 
     def run(self):
         install.run(self)
 
 setup(
     name="composio_core",
-    version="0.2.5",
+    version="0.2.6",
     author="Utkarsh",
     author_email="utkarsh@composio.dev",
     description="Core package to act as a bridge between composio platform and other services.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

