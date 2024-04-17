# Comparing `tmp/trubrics_beta-0.1.0.tar.gz` & `tmp/trubrics_beta-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trubrics_beta-0.1.0.tar", last modified: Tue Apr 16 13:05:19 2024, max compression
+gzip compressed data, was "trubrics_beta-0.1.1.tar", last modified: Wed Apr 17 16:42:45 2024, max compression
```

## Comparing `trubrics_beta-0.1.0.tar` & `trubrics_beta-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2024-04-16 13:05:19.122871 trubrics_beta-0.1.0/
--rw-r--r--   0 jeffkayne   (501) staff       (20)      627 2024-04-16 13:05:19.122631 trubrics_beta-0.1.0/PKG-INFO
--rw-r--r--   0 jeffkayne   (501) staff       (20)      311 2024-04-16 12:55:47.000000 trubrics_beta-0.1.0/README.md
--rw-r--r--   0 jeffkayne   (501) staff       (20)      417 2024-04-16 13:04:20.000000 trubrics_beta-0.1.0/pyproject.toml
--rw-r--r--   0 jeffkayne   (501) staff       (20)       38 2024-04-16 13:05:19.122922 trubrics_beta-0.1.0/setup.cfg
-drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2024-04-16 13:05:19.121003 trubrics_beta-0.1.0/trubrics_beta/
--rw-r--r--   0 jeffkayne   (501) staff       (20)      142 2024-04-16 13:00:41.000000 trubrics_beta-0.1.0/trubrics_beta/__init__.py
--rw-r--r--   0 jeffkayne   (501) staff       (20)     2433 2024-04-16 12:46:24.000000 trubrics_beta-0.1.0/trubrics_beta/sdk.py
-drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2024-04-16 13:05:19.122386 trubrics_beta-0.1.0/trubrics_beta.egg-info/
--rw-r--r--   0 jeffkayne   (501) staff       (20)      627 2024-04-16 13:05:19.000000 trubrics_beta-0.1.0/trubrics_beta.egg-info/PKG-INFO
--rw-r--r--   0 jeffkayne   (501) staff       (20)      219 2024-04-16 13:05:19.000000 trubrics_beta-0.1.0/trubrics_beta.egg-info/SOURCES.txt
--rw-r--r--   0 jeffkayne   (501) staff       (20)        1 2024-04-16 13:05:19.000000 trubrics_beta-0.1.0/trubrics_beta.egg-info/dependency_links.txt
--rw-r--r--   0 jeffkayne   (501) staff       (20)       14 2024-04-16 13:05:19.000000 trubrics_beta-0.1.0/trubrics_beta.egg-info/top_level.txt
+drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2024-04-17 16:42:45.072568 trubrics_beta-0.1.1/
+-rw-r--r--   0 jeffkayne   (501) staff       (20)      627 2024-04-17 16:42:45.072322 trubrics_beta-0.1.1/PKG-INFO
+-rw-r--r--   0 jeffkayne   (501) staff       (20)      311 2024-04-17 14:52:00.000000 trubrics_beta-0.1.1/README.md
+-rw-r--r--   0 jeffkayne   (501) staff       (20)      417 2024-04-17 16:41:39.000000 trubrics_beta-0.1.1/pyproject.toml
+-rw-r--r--   0 jeffkayne   (501) staff       (20)       38 2024-04-17 16:42:45.072613 trubrics_beta-0.1.1/setup.cfg
+drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2024-04-17 16:42:45.071049 trubrics_beta-0.1.1/trubrics_beta/
+-rw-r--r--   0 jeffkayne   (501) staff       (20)      143 2024-04-17 16:37:25.000000 trubrics_beta-0.1.1/trubrics_beta/__init__.py
+-rw-r--r--   0 jeffkayne   (501) staff       (20)     2455 2024-04-17 16:26:59.000000 trubrics_beta-0.1.1/trubrics_beta/main.py
+drwxr-xr-x   0 jeffkayne   (501) staff       (20)        0 2024-04-17 16:42:45.072117 trubrics_beta-0.1.1/trubrics_beta.egg-info/
+-rw-r--r--   0 jeffkayne   (501) staff       (20)      627 2024-04-17 16:42:45.000000 trubrics_beta-0.1.1/trubrics_beta.egg-info/PKG-INFO
+-rw-r--r--   0 jeffkayne   (501) staff       (20)      220 2024-04-17 16:42:45.000000 trubrics_beta-0.1.1/trubrics_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffkayne   (501) staff       (20)        1 2024-04-17 16:42:45.000000 trubrics_beta-0.1.1/trubrics_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffkayne   (501) staff       (20)       14 2024-04-17 16:42:45.000000 trubrics_beta-0.1.1/trubrics_beta.egg-info/top_level.txt
```

### Comparing `trubrics_beta-0.1.0/PKG-INFO` & `trubrics_beta-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trubrics-beta
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python SDK to track events in Trubrics.
 Author-email: Jeff Kayne <jeff.kayne@trubrics.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `trubrics_beta-0.1.0/trubrics_beta/sdk.py` & `trubrics_beta-0.1.1/trubrics_beta/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 import json
 import threading
-from datetime import datetime
+from datetime import datetime, timezone
 
 import aiohttp
 import requests
 
 
 class Trubrics:
     def __init__(self, api_key: str, host: str = "https://api.trubrics.com"):
@@ -41,15 +41,15 @@
     def _post_body(
         self, event: str, user_id: str, properties: dict[str, str] | None = None
     ):
         return {
             "event": event,
             "user_id": user_id,
             "properties": properties,
-            "timestamp": datetime.now().isoformat(),
+            "timestamp": datetime.now(timezone.utc).isoformat(),
         }
 
     async def _post_event(
         self, session, user_id: str, event: str, properties: dict | None
     ):
         try:
             post_request = session.post(
```

### Comparing `trubrics_beta-0.1.0/trubrics_beta.egg-info/PKG-INFO` & `trubrics_beta-0.1.1/trubrics_beta.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trubrics-beta
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python SDK to track events in Trubrics.
 Author-email: Jeff Kayne <jeff.kayne@trubrics.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

