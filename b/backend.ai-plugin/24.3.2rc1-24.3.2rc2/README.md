# Comparing `tmp/backend.ai-plugin-24.3.2rc1.tar.gz` & `tmp/backend.ai-plugin-24.3.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-plugin-24.3.2rc1.tar", last modified: Wed Apr 17 01:17:26 2024, max compression
+gzip compressed data, was "backend.ai-plugin-24.3.2rc2.tar", last modified: Wed Apr 17 05:19:32 2024, max compression
```

## Comparing `backend.ai-plugin-24.3.2rc1.tar` & `backend.ai-plugin-24.3.2rc2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:17:26.976308 backend.ai-plugin-24.3.2rc1/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 01:17:26.000000 backend.ai-plugin-24.3.2rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-17 01:17:26.976308 backend.ai-plugin-24.3.2rc1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:17:26.972308 backend.ai-plugin-24.3.2rc1/ai/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:17:26.972308 backend.ai-plugin-24.3.2rc1/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:17:26.976308 backend.ai-plugin-24.3.2rc1/ai/backend/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-17 01:17:26.000000 backend.ai-plugin-24.3.2rc1/ai/backend/plugin/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-17 01:17:26.000000 backend.ai-plugin-24.3.2rc1/ai/backend/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-17 01:17:26.000000 backend.ai-plugin-24.3.2rc1/ai/backend/plugin/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 01:17:26.000000 backend.ai-plugin-24.3.2rc1/ai/backend/plugin/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:17:26.976308 backend.ai-plugin-24.3.2rc1/backend.ai_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-17 01:17:26.000000 backend.ai-plugin-24.3.2rc1/backend.ai_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-17 01:17:26.000000 backend.ai-plugin-24.3.2rc1/backend.ai_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 01:17:26.000000 backend.ai-plugin-24.3.2rc1/backend.ai_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 01:17:26.000000 backend.ai-plugin-24.3.2rc1/backend.ai_plugin.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 01:17:26.000000 backend.ai-plugin-24.3.2rc1/backend.ai_plugin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-17 01:17:26.000000 backend.ai-plugin-24.3.2rc1/backend.ai_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-17 01:17:26.000000 backend.ai-plugin-24.3.2rc1/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 01:17:26.976308 backend.ai-plugin-24.3.2rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-17 01:17:26.000000 backend.ai-plugin-24.3.2rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:19:32.584391 backend.ai-plugin-24.3.2rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 05:19:32.000000 backend.ai-plugin-24.3.2rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-17 05:19:32.584391 backend.ai-plugin-24.3.2rc2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:19:32.576391 backend.ai-plugin-24.3.2rc2/ai/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:19:32.576391 backend.ai-plugin-24.3.2rc2/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:19:32.580391 backend.ai-plugin-24.3.2rc2/ai/backend/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-17 05:19:32.000000 backend.ai-plugin-24.3.2rc2/ai/backend/plugin/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-17 05:19:32.000000 backend.ai-plugin-24.3.2rc2/ai/backend/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-17 05:19:32.000000 backend.ai-plugin-24.3.2rc2/ai/backend/plugin/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 05:19:32.000000 backend.ai-plugin-24.3.2rc2/ai/backend/plugin/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:19:32.584391 backend.ai-plugin-24.3.2rc2/backend.ai_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-17 05:19:32.000000 backend.ai-plugin-24.3.2rc2/backend.ai_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-17 05:19:32.000000 backend.ai-plugin-24.3.2rc2/backend.ai_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 05:19:32.000000 backend.ai-plugin-24.3.2rc2/backend.ai_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 05:19:32.000000 backend.ai-plugin-24.3.2rc2/backend.ai_plugin.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 05:19:32.000000 backend.ai-plugin-24.3.2rc2/backend.ai_plugin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-17 05:19:32.000000 backend.ai-plugin-24.3.2rc2/backend.ai_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-17 05:19:32.000000 backend.ai-plugin-24.3.2rc2/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 05:19:32.584391 backend.ai-plugin-24.3.2rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-17 05:19:32.000000 backend.ai-plugin-24.3.2rc2/setup.py
```

### Comparing `backend.ai-plugin-24.3.2rc1/PKG-INFO` & `backend.ai-plugin-24.3.2rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-plugin
-Version: 24.3.2rc1
+Version: 24.3.2rc2
 Summary: Backend.AI Plugin Subsystem
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-plugin-24.3.2rc1/ai/backend/plugin/entrypoint.py` & `backend.ai-plugin-24.3.2rc2/ai/backend/plugin/entrypoint.py`

 * *Files identical despite different names*

### Comparing `backend.ai-plugin-24.3.2rc1/backend.ai_plugin.egg-info/PKG-INFO` & `backend.ai-plugin-24.3.2rc2/backend.ai_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-plugin
-Version: 24.3.2rc1
+Version: 24.3.2rc2
 Summary: Backend.AI Plugin Subsystem
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-plugin-24.3.2rc1/backend_shim.py` & `backend.ai-plugin-24.3.2rc2/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-plugin-24.3.2rc1/setup.py` & `backend.ai-plugin-24.3.2rc2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,11 +46,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.12,<3.13',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """24.03.2rc1
+    'version': """24.03.2rc2
 """,
     'zip_safe': False,
 })
```
