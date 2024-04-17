# Comparing `tmp/hectiq_console-1.2.0.tar.gz` & `tmp/hectiq_console-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/console/console/python-collector/dist/.tmp-ir0cukys/hectiq_console-1.2.0.tar", last modified: Fri Mar 22 17:37:35 2024, max compression
+gzip compressed data, was "/home/runner/work/console/console/python-collector/dist/.tmp-9_9n33pn/hectiq_console-1.2.1.tar", last modified: Wed Apr 17 13:24:41 2024, max compression
```

## Comparing `hectiq_console-1.2.0.tar` & `hectiq_console-1.2.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:37:35.000000 hectiq_console-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-03-22 17:37:24.000000 hectiq_console-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-22 17:37:24.000000 hectiq_console-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8677 2024-03-22 17:37:35.000000 hectiq_console-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8047 2024-03-22 17:37:24.000000 hectiq_console-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:37:35.000000 hectiq_console-1.2.0/hectiq_console/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-22 17:37:24.000000 hectiq_console-1.2.0/hectiq_console/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:37:35.000000 hectiq_console-1.2.0/hectiq_console/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-22 17:37:24.000000 hectiq_console-1.2.0/hectiq_console/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-22 17:37:24.000000 hectiq_console-1.2.0/hectiq_console/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-03-22 17:37:24.000000 hectiq_console-1.2.0/hectiq_console/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    36483 2024-03-22 17:37:24.000000 hectiq_console-1.2.0/hectiq_console/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:37:35.000000 hectiq_console-1.2.0/hectiq_console/starlette/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-22 17:37:24.000000 hectiq_console-1.2.0/hectiq_console/starlette/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9763 2024-03-22 17:37:24.000000 hectiq_console-1.2.0/hectiq_console/starlette/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-03-22 17:37:24.000000 hectiq_console-1.2.0/hectiq_console/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:37:35.000000 hectiq_console-1.2.0/hectiq_console/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:37:24.000000 hectiq_console-1.2.0/hectiq_console/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-03-22 17:37:24.000000 hectiq_console-1.2.0/hectiq_console/utils/batch_fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-22 17:37:24.000000 hectiq_console-1.2.0/hectiq_console/utils/docstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-03-22 17:37:24.000000 hectiq_console-1.2.0/hectiq_console/utils/log_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:37:35.000000 hectiq_console-1.2.0/hectiq_console.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8677 2024-03-22 17:37:35.000000 hectiq_console-1.2.0/hectiq_console.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-22 17:37:35.000000 hectiq_console-1.2.0/hectiq_console.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 17:37:35.000000 hectiq_console-1.2.0/hectiq_console.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-22 17:37:35.000000 hectiq_console-1.2.0/hectiq_console.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 17:37:27.000000 hectiq_console-1.2.0/hectiq_console.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-22 17:37:35.000000 hectiq_console-1.2.0/hectiq_console.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-22 17:37:35.000000 hectiq_console-1.2.0/hectiq_console.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-22 17:37:24.000000 hectiq_console-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 17:37:35.000000 hectiq_console-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-22 17:37:24.000000 hectiq_console-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:24:41.000000 hectiq_console-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8677 2024-04-17 13:24:41.000000 hectiq_console-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8047 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:24:41.000000 hectiq_console-1.2.1/hectiq_console/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/hectiq_console/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:24:41.000000 hectiq_console-1.2.1/hectiq_console/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/hectiq_console/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/hectiq_console/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/hectiq_console/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37370 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/hectiq_console/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:24:41.000000 hectiq_console-1.2.1/hectiq_console/starlette/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/hectiq_console/starlette/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9763 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/hectiq_console/starlette/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/hectiq_console/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:24:41.000000 hectiq_console-1.2.1/hectiq_console/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/hectiq_console/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/hectiq_console/utils/batch_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/hectiq_console/utils/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/hectiq_console/utils/log_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:24:41.000000 hectiq_console-1.2.1/hectiq_console.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8677 2024-04-17 13:24:41.000000 hectiq_console-1.2.1/hectiq_console.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-17 13:24:41.000000 hectiq_console-1.2.1/hectiq_console.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 13:24:41.000000 hectiq_console-1.2.1/hectiq_console.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-17 13:24:41.000000 hectiq_console-1.2.1/hectiq_console.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 13:24:33.000000 hectiq_console-1.2.1/hectiq_console.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-17 13:24:41.000000 hectiq_console-1.2.1/hectiq_console.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 13:24:41.000000 hectiq_console-1.2.1/hectiq_console.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 13:24:41.000000 hectiq_console-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-17 13:24:28.000000 hectiq_console-1.2.1/setup.py
```

### Comparing `hectiq_console-1.2.0/LICENSE` & `hectiq_console-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hectiq_console-1.2.0/PKG-INFO` & `hectiq_console-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hectiq_console
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python client to use the Hectiq Console
 Home-page: https://console.hectiq.ai
 Author: Edward Laurence
 Author-email: edwardl@hectiq.ai
 Keywords: pip requirements imports
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `hectiq_console-1.2.0/README.md` & `hectiq_console-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `hectiq_console-1.2.0/hectiq_console/cli/auth.py` & `hectiq_console-1.2.1/hectiq_console/cli/auth.py`

 * *Files identical despite different names*

### Comparing `hectiq_console-1.2.0/hectiq_console/functional.py` & `hectiq_console-1.2.1/hectiq_console/functional.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,62 +1,77 @@
 from hectiq_console import CONSOLE_APP_URL
 
 import os
-import contextvars 
+import contextvars
 import requests
 import time
 import datetime as dt
 import traceback
 from typing import Optional, Union, List, Dict, Literal
 from contextlib import contextmanager
 from hectiq_console.utils.batch_fetch import BatchFetch
 from hectiq_console.utils.log_handler import MemoryHandler, get_handler
 from hectiq_console.utils.docstring import inherit_docstring_from
 
+try:
+    import tqdm
+except ImportError:
+    tqdm = None
+
 import logging
+
 logger = logging.getLogger()
 
-resource_cvar = contextvars.ContextVar("resource_id", default=None) 
-api_key_cvar = contextvars.ContextVar("api_key", default=None) 
-author_cvar = contextvars.ContextVar("author", default=os.environ.get("HECTIQ_CONSOLE_EMAIL")) 
+resource_cvar = contextvars.ContextVar("resource_id", default=None)
+api_key_cvar = contextvars.ContextVar("api_key", default=None)
+author_cvar = contextvars.ContextVar("author", default=os.environ.get("HECTIQ_CONSOLE_EMAIL"))
 organization_cvar = contextvars.ContextVar("organization", default=None)
 current_job_cvar = contextvars.ContextVar("current_job", default=None)
 current_job_step_cvar = contextvars.ContextVar("current_job_step", default=None)
 batch_annotations_cvar = contextvars.ContextVar("batch_annotations", default=None)
 
+
 def set_ressource(resource: str):
     """Will be removed in the future. Use `set_resource` instead."""
     resource_cvar.set(resource)
 
+
 def set_resource(resource: str):
     resource_cvar.set(resource)
 
+
 def set_organization(organization: str):
     organization_cvar.set(organization)
 
+
 def set_job(job: str):
     current_job_cvar.set(job)
 
+
 def get_job() -> Optional[str]:
     return current_job_cvar.get()
 
+
 def set_job_step(job_step: str):
     current_job_step_cvar.set(job_step)
 
+
 def get_job_step() -> Optional[str]:
     return current_job_step_cvar.get()
 
+
 def get_organization() -> Optional[str]:
     """Get the organization in the context.
 
     Returns:
         str: Organization
     """
     return organization_cvar.get()
 
+
 def get_resource(resource: Optional[str] = None) -> Optional[str]:
     """Get a resource in the context.
 
     Args:
         resource (Optional[str], optional): Ressource ID of the resource to get. Defaults to None.
 
     Returns:
@@ -64,17 +79,18 @@
     """
     if resource is None:
         resource = resource_cvar.get()
     if resource is None:
         raise ValueError("You must provide a resource ID to the get_resource method or use `set_resource`.")
     return resource
 
-def authenticate(api_key: Optional[str] = None,
-                 email: Optional[str] = None,
-                 organization: Optional[str] = None) -> bool:
+
+def authenticate(
+    api_key: Optional[str] = None, email: Optional[str] = None, organization: Optional[str] = None
+) -> bool:
     """Authenticate to the Hectiq Console.
     If api_key is None, the api_key is taken from:
      - the environment variable `HECTIQ_CONSOLE_API_KEY`.
      - the api_key located in the file `~/.hectiq-console/credentials.toml` (or the HECTIQ_CONSOLE_CREDENTIALS_FILE).
 
     Args:
         api_key (Optional[str], optional): API key. Defaults to None.
@@ -83,129 +99,135 @@
 
     Returns:
         bool: True if the authentication is successful, False otherwise.
     """
     if api_key_cvar.get() is not None:
         # Already authenticated
         return True
-    
+
     organization = organization or organization_cvar.get()
     email = email or author_cvar.get()
-    
+
     if api_key is None:
         # Try to get the api_key from the environment variable
         api_key = os.environ.get("HECTIQ_CONSOLE_API_KEY")
         email = os.environ.get("HECTIQ_CONSOLE_EMAIL", email)
 
     if api_key is None:
         # Try to get the api_key from the credentials file
         import toml
         from pathlib import Path
-        path = os.getenv("HECTIQ_CONSOLE_CREDENTIALS_FILE", 
-                         os.path.join(Path.home(),".hectiq-console", "credentials.toml"))
+
+        path = os.getenv(
+            "HECTIQ_CONSOLE_CREDENTIALS_FILE", os.path.join(Path.home(), ".hectiq-console", "credentials.toml")
+        )
         if not os.path.exists(path):
             return False
         with open(path, "r") as path:
             data = toml.load(path)
 
         if organization is not None:
             data = data.get(organization, {})
         else:
             # Multiple organizations
-            if len(data)==0:
+            if len(data) == 0:
                 return False
-            
+
             organization = list(data.keys())[0]
-            set_organization(organization) # Set the organization in the context
+            set_organization(organization)  # Set the organization in the context
             data = list(data.values())[0]
-      
+
         api_key = data.get("value")
         email = data.get("email", email)
 
         if api_key is None:
             return False
 
     api_key_cvar.set(api_key)
     author_cvar.set(email)
     return True
 
+
 def get_authentification_headers() -> dict:
-    """Get the authentification headers for the Hectiq Console. 
+    """Get the authentification headers for the Hectiq Console.
     Do not use this method directly. Instead, use the `authenticate` method.
 
     Returns:
         dict: Headers
     """
     is_logged = authenticate()
     if not is_logged:
-        raise ValueError(f"You must authenticate to the Hectiq Console using the `hectiq_console.functional.authenticate` method or the command line `hectiq-console authenticate`. This error may occur if the organization ({get_organization()}) is not set or incorrect.")
+        raise ValueError(
+            f"You must authenticate to the Hectiq Console using the `hectiq_console.functional.authenticate` method or the command line `hectiq-console authenticate`. This error may occur if the organization ({get_organization()}) is not set or incorrect."
+        )
     api_key = api_key_cvar.get()
     if api_key is None:
         raise ValueError("You must authenticate to the Hectiq Console using the `authenticate` method.")
     return {"X-API-Key": f"{api_key}"}
 
+
 def set_email(email: str):
     author_cvar.set(email)
 
 
 def get_email(email: Optional[str] = None) -> Optional[str]:
     """Get the email in the context.
 
     Returns:
         str: Email
     """
     return email or author_cvar.get()
 
-def create_incident(title: str, 
-                    description: Optional[str] = None,
-                    filenames: Optional[List] = None, 
-                    resource: Optional[str] = None):
+
+def create_incident(
+    title: str, description: Optional[str] = None, filenames: Optional[List] = None, resource: Optional[str] = None
+):
     """Create an incident in the Hectiq Console.
 
     Args:
         title (str): Title of the incident
         description (Optional[str], optional): Description of the incident. Defaults to None.
         filenames (Optional[List], optional): List of filenames to attach to the incident. Defaults to None.
-        resource (Optional[str], optional): Ressource ID of the resource to which the incident is related. 
+        resource (Optional[str], optional): Ressource ID of the resource to which the incident is related.
             Defaults to None.
     """
     resource = get_resource(resource)
     body = {"name": title, "description": description}
     if filenames is not None:
         body["files"] = []
         for filename in filenames:
             assert os.path.exists(filename), f"File {filename} does not exist."
             name = os.path.basename(filename)
             num_bytes = os.path.getsize(filename)
             extension = os.path.splitext(filename)[1].replace(".", "")
             body["files"].append({"name": name, "num_bytes": num_bytes, "extension": extension})
-    res = requests.post(f"{CONSOLE_APP_URL}/app/sender-client/{resource}/incidents", 
-                 json=body)
+    res = requests.post(f"{CONSOLE_APP_URL}/app/sender-client/{resource}/incidents", json=body)
     if res.status_code != 200:
         logger.error(f"⚠️ Error while creating the incident with hectiq_console.create_incident: {res.text}")
         return
-    
+
     # Upload the files
     if filenames is not None:
         from hectiq_console.upload import upload_file
+
         for filename, policy in zip(filenames, res.json()["policies"]):
             upload_file(filepath=filename, policy=policy)
 
-def add_file(filename: str,
-             job: Optional[str] = None,
-             resource: Optional[str] = None):
+
+def add_file(filename: str, job: Optional[str] = None, resource: Optional[str] = None):
     """Add a file to a resource in the Hectiq Console.
 
     Args:
         filename (str): Name of the file
         job (Optional[str], optional): Job ID of the job to which the file is related. Defaults to None.
-        resource (Optional[str], optional): Ressource ID of the resource to which the file is related. 
+        resource (Optional[str], optional): Ressource ID of the resource to which the file is related.
             Defaults to None.
     """
     from hectiq_console.upload import upload_file
+
     resource = get_resource(resource)
     job = get_job() if job is None else job
 
     assert os.path.exists(filename), f"File {filename} does not exist."
     name = os.path.basename(filename)
     num_bytes = os.path.getsize(filename)
     extension = os.path.splitext(filename)[1].replace(".", "")
@@ -219,38 +241,37 @@
     try:
         policy = res.json()
     except:
         logger.error(f"⚠️ Error while creating the file with hectiq_console.add_file: {res.text}")
         return
     upload_file(filepath=filename, policy=policy)
 
-def add_metrics(name: str, 
-                value: Union[float, int], 
-                resource: Optional[str] = None):
+
+def add_metrics(name: str, value: Union[float, int], resource: Optional[str] = None):
     """Add metrics to the Hectiq Console.
 
     Args:
         key (str): Key of the metrics
         value (Union[float, int]): Value of the metrics
-        resource (Optional[str], optional): Ressource ID of the resource to which the metrics are related. 
+        resource (Optional[str], optional): Ressource ID of the resource to which the metrics are related.
             Defaults to None.
     """
     resource = get_resource(resource)
-    body = {
-        "metrics" : [{"name": name, "value": value}]
-    }
-    requests.post(f"{CONSOLE_APP_URL}/app/sender-client/{resource}/metrics", 
-                 json=body)
-    
-def add_annotation(id: Optional[str] = None, 
-                    inputs: Optional[Dict] = None,
-                    outputs: Optional[Dict] = None,
-                    metadata: Optional[Dict] = None,
-                    resource: Optional[str] = None):
-    """Add an annotation to the Hectiq Console. 
+    body = {"metrics": [{"name": name, "value": value}]}
+    requests.post(f"{CONSOLE_APP_URL}/app/sender-client/{resource}/metrics", json=body)
+
+
+def add_annotation(
+    id: Optional[str] = None,
+    inputs: Optional[Dict] = None,
+    outputs: Optional[Dict] = None,
+    metadata: Optional[Dict] = None,
+    resource: Optional[str] = None,
+):
+    """Add an annotation to the Hectiq Console.
     For multiple annotations, you can use
 
     ```
     with hectiq_console.batch_annotations():
         hectiq_console.add_annotation(...)
         hectiq_console.add_annotation(...)
     ```
@@ -267,68 +288,69 @@
         data["id"] = id
 
     if batch_annotations_cvar.get() is not None:
         val = batch_annotations_cvar.get()
         val.append(data)
         batch_annotations_cvar.set(val)
         return
-    
-    res = requests.post(f"{CONSOLE_APP_URL}/app/sender-client/{resource}/annotations", 
-                        json=data)
+
+    res = requests.post(f"{CONSOLE_APP_URL}/app/sender-client/{resource}/annotations", json=data)
     if res.status_code != 200:
         logger.error(f"⚠️ Error while creating the annotation with hectiq_console.add_annotation: {res.text}")
 
-def add_annotations(annotations: List[Dict],
-                    resource: Optional[str] = None):
+
+def add_annotations(annotations: List[Dict], resource: Optional[str] = None):
     """Add multiple annotations to the Hectiq Console.
 
     Args:
-        annotations (List[Dict]): Annotations with optional keys `id`, `inputs`, `outputs` and `metadata`. 
-        resource (Optional[str], optional): Ressource ID of the resource to which the annotations are related. 
+        annotations (List[Dict]): Annotations with optional keys `id`, `inputs`, `outputs` and `metadata`.
+        resource (Optional[str], optional): Ressource ID of the resource to which the annotations are related.
             Defaults to None.
     """
     resource = get_resource(resource)
     data = {"annotations": annotations}
-    res = requests.post(f"{CONSOLE_APP_URL}/app/sender-client/{resource}/batch-annotations",
-                        json=data)
+    res = requests.post(f"{CONSOLE_APP_URL}/app/sender-client/{resource}/batch-annotations", json=data)
     if res.status_code != 200:
         logger.error(f"⚠️ Error while creating the annotations with hectiq_console.add_annotations: {res.text}")
 
-def download_annotation(id: str,
-                        resource: Optional[str] = None) -> dict:
+
+def download_annotation(id: str, resource: Optional[str] = None) -> dict:
     """Download an annotation from the Hectiq Console.
 
     Args:
         id (str): ID of the annotation
-        resource (Optional[str], optional): Ressource ID of the resource to which the annotation is related. 
+        resource (Optional[str], optional): Ressource ID of the resource to which the annotation is related.
             Defaults to None.
     """
     resource = get_resource(resource)
     headers = get_authentification_headers()
     res = requests.get(f"{CONSOLE_APP_URL}/app/sender-client/{resource}/annotations/{id}", headers=headers)
     if res.status_code != 200:
         logger.error(f"⚠️ Error while downloading the annotation with hectiq_console.download_annotation: {res.text}")
         return
     return res.json()
 
-def download_annotations(from_date: Optional[dt.datetime] = None,
-                        to_date: Optional[dt.datetime] = None,
-                        labels: Optional[List[str]] = None,
-                        label_set: Literal["any", "all", "none", "empty"] = "any",
-                        annotated_by: Optional[List[str]] = None,
-                        annotated_by_set: Literal["any", "all", "none"] = "any",
-                        fields: Optional[List[str]] = ["private_id", "inputs", "outputs", "metadata"],
-                        page: Optional[int] = 1,
-                        limit: Optional[int] = 100,
-                        order_by: Optional[str] = None,
-                        order_direction: Literal["asc", "desc"] = "asc",
-                         resource: Optional[str] = None):
+
+def download_annotations(
+    from_date: Optional[dt.datetime] = None,
+    to_date: Optional[dt.datetime] = None,
+    labels: Optional[List[str]] = None,
+    label_set: Literal["any", "all", "none", "empty"] = "any",
+    annotated_by: Optional[List[str]] = None,
+    annotated_by_set: Literal["any", "all", "none"] = "any",
+    fields: Optional[List[str]] = ["private_id", "inputs", "outputs", "metadata"],
+    page: Optional[int] = 1,
+    limit: Optional[int] = 100,
+    order_by: Optional[str] = None,
+    order_direction: Literal["asc", "desc"] = "asc",
+    resource: Optional[str] = None,
+):
     """Download all annotations from the Hectiq Console.
 
-    Args:   
+    Args:
         from_date (Optional[dt.datetime]): Start date of creation of the annotations. Defaults to None.
         to_date (Optional[dt.datetime]): End date of creation of the annotations. Defaults to None.
         labels (Optional[List[str]]): Labels of the annotations. Defaults to None.
         label_set (Literal["any", "all", "none", "empty"]): Set of labels. Defaults to "any".
             - "any": At least one label must be present
             - "all": All labels must be present
             - "none": No label from the label list must be present
@@ -339,15 +361,15 @@
             - "all": All users must have annotated the annotations
             - "none": No user from the user list must have annotated the annotations
         fields (Optional[List[str]]): Fields to return. Defaults to ["private_id", "inputs", "outputs", "metadata"].
         page (Optional[int]): Page number. Defaults to 1.
         limit (Optional[int]): Number of annotations per page. Defaults to 100.
         order_by (Optional[str]): Field to order by. Defaults to None.
         order_direction (Literal["asc", "desc"]): Order direction. Defaults to "asc".
-        resource (Optional[str]): Ressource ID of the resource to which the annotations are related. 
+        resource (Optional[str]): Ressource ID of the resource to which the annotations are related.
             Defaults to None.
     """
     resource = get_resource(resource)
     headers = get_authentification_headers()
 
     params = {
         "fields": fields,
@@ -356,65 +378,75 @@
         "labels": labels,
         "label_set": label_set,
         "annotated_by": annotated_by,
         "annotated_by_set": annotated_by_set,
         "page": page,
         "limit": limit,
         "order_by": order_by,
-        "order_direction": order_direction
+        "order_direction": order_direction,
     }
     res = requests.get(f"{CONSOLE_APP_URL}/app/sender-client/{resource}/annotations", params=params, headers=headers)
     if res.status_code != 200:
         logger.error(f"⚠️ Error while downloading the annotations with hectiq_console.download_annotations: {res.text}")
         return
     return res.json()
 
-def search_annotation_labels(search: Optional[str] = None,
-                             fields: Optional[List[str]] = ["id", "label"],
-                                page: Optional[int] = 1,
-                                limit: Optional[int] = 100,
-                                order_by: Optional[str] = None,
-                                order_direction: Literal["asc", "desc"] = "asc",
-                                resource: Optional[str] = None):
+
+def search_annotation_labels(
+    search: Optional[str] = None,
+    fields: Optional[List[str]] = ["id", "label"],
+    page: Optional[int] = 1,
+    limit: Optional[int] = 100,
+    order_by: Optional[str] = None,
+    order_direction: Literal["asc", "desc"] = "asc",
+    resource: Optional[str] = None,
+):
     """Search annotation labels from the Hectiq Console.
 
     Args:
         search (Optional[str]): Search string. Defaults to None.
         fields (Optional[List[str]]): Fields to return. Defaults to ["id", "label"].
         page (Optional[int]): Page number. Defaults to 1.
         limit (Optional[int]): Number of annotations per page. Defaults to 100.
         order_by (Optional[str]): Field to order by. Defaults to None.
         order_direction (Literal["asc", "desc"]): Order direction. Defaults to "asc".
-        resource (Optional[str]): Ressource ID of the resource to which the annotations are related. 
+        resource (Optional[str]): Ressource ID of the resource to which the annotations are related.
             Defaults to None.
     """
     resource = get_resource(resource)
     headers = get_authentification_headers()
 
     params = {
         "fields": fields,
         "search": search,
         "page": page,
         "limit": limit,
         "order_by": order_by,
-        "order_direction": order_direction
+        "order_direction": order_direction,
     }
-    res = requests.get(f"{CONSOLE_APP_URL}/app/sender-client/{resource}/annotation-labels", params=params, headers=headers)
-    if res.status_code != 200:
-        logger.error(f"⚠️ Error while fetching the annotation labels with hectiq_console.search_annotation_labels: {res.text}")
+    res = requests.get(
+        f"{CONSOLE_APP_URL}/app/sender-client/{resource}/annotation-labels", params=params, headers=headers
+    )
+    if res.status_code != 200:
+        logger.error(
+            f"⚠️ Error while fetching the annotation labels with hectiq_console.search_annotation_labels: {res.text}"
+        )
         return
     return res.json()
 
-def count_annotations(from_date: Optional[dt.datetime] = None,
-                        to_date: Optional[dt.datetime] = None,
-                        labels: Optional[List[str]] = None,
-                        label_set: Literal["any", "all", "none", "empty"] = "any",
-                        annotated_by: Optional[List[str]] = None,
-                        annotated_by_set: Literal["any", "all", "none"] = "any",
-                        resource: Optional[str] = None):
+
+def count_annotations(
+    from_date: Optional[dt.datetime] = None,
+    to_date: Optional[dt.datetime] = None,
+    labels: Optional[List[str]] = None,
+    label_set: Literal["any", "all", "none", "empty"] = "any",
+    annotated_by: Optional[List[str]] = None,
+    annotated_by_set: Literal["any", "all", "none"] = "any",
+    resource: Optional[str] = None,
+):
     """Count annotations from the Hectiq Console.
 
     Args:
         from_date (Optional[dt.datetime]): Start date of creation of the annotations. Defaults to None.
         to_date (Optional[dt.datetime]): End date of creation of the annotations. Defaults to None.
         labels (Optional[List[str]]): Labels of the annotations. Defaults to None.
         label_set (Literal["any", "all", "none", "empty"]): Set of labels. Defaults to "any".
@@ -423,409 +455,426 @@
             - "none": No label from the label list must be present
             - "empty": No label must be present (label list must be empty)
         annotated_by (Optional[List[str]]): Email of the user who annotated the annotations. Defaults to None.
         annotated_by_set (Literal["any", "all", "none"]): Set of annotated_by. Defaults to "any".
             - "any": At least one user must have annotated the annotations
             - "all": All users must have annotated the annotations
             - "none": No user from the user list must have annotated the annotations
-        resource (Optional[str]): Ressource ID of the resource to which the annotations are related. 
+        resource (Optional[str]): Ressource ID of the resource to which the annotations are related.
             Defaults to None.
     """
     resource = get_resource(resource)
     headers = get_authentification_headers()
 
     params = {
         "created_from_date": from_date.toisoformat() if from_date is not None else None,
         "created_to_date": to_date.toisoformat() if to_date is not None else None,
         "labels": labels,
         "label_set": label_set,
         "annotated_by": annotated_by,
-        "annotated_by_set": annotated_by_set
+        "annotated_by_set": annotated_by_set,
     }
-    res = requests.get(f"{CONSOLE_APP_URL}/app/sender-client/{resource}/count-annotations", params=params, headers=headers)
+    res = requests.get(
+        f"{CONSOLE_APP_URL}/app/sender-client/{resource}/count-annotations", params=params, headers=headers
+    )
     if res.status_code != 200:
         logger.error(f"⚠️ Error while counting the annotations with hectiq_console.count_annotations: {res.text}")
         return
     return res.json()["count"]
 
-def attach_annotation_label(annotation_id: str, 
-                               label_id: str,
-                               email: Optional[str] = None,
-                               resource: Optional[str] = None):
+
+def attach_annotation_label(
+    annotation_id: str, label_id: str, email: Optional[str] = None, resource: Optional[str] = None
+):
     """Attach a label to an annotation in the Hectiq Console.
     If the label is already attached, nothing is done.
 
     Args:
         annotation_id (str): ID of the annotation
         label_id (str): ID of the label
         email (Optional[str], optional): Email of the user. Defaults to None.
-        resource (Optional[str], optional): Ressource ID of the resource to which the annotation is related. 
+        resource (Optional[str], optional): Ressource ID of the resource to which the annotation is related.
             Defaults to None.
     """
     resource = get_resource(resource)
     headers = get_authentification_headers()
     email = get_email(email)
     assert email is not None, "You must set the email with `set_email` or use `hectiq-console authenticate --replace`."
-    params = {
-        "email": email
-    }
-    res = requests.post(f"{CONSOLE_APP_URL}/app/sender-client/{resource}/annotations/{annotation_id}/add-label/{label_id}", 
-                 headers=headers, params=params)
-    if res.status_code != 200:
-        logger.error(f"⚠️ Error while attaching the label to the annotation with hectiq_console.attach_label_to_annotation: {res.text}")
+    params = {"email": email}
+    res = requests.post(
+        f"{CONSOLE_APP_URL}/app/sender-client/{resource}/annotations/{annotation_id}/add-label/{label_id}",
+        headers=headers,
+        params=params,
+    )
+    if res.status_code != 200:
+        logger.error(
+            f"⚠️ Error while attaching the label to the annotation with hectiq_console.attach_label_to_annotation: {res.text}"
+        )
         return
-    
+
     return True
 
-def detach_annotation_label(annotation_id: str, 
-                               label_id: str,
-                               email: Optional[str] = None,
-                               resource: Optional[str] = None):
+
+def detach_annotation_label(
+    annotation_id: str, label_id: str, email: Optional[str] = None, resource: Optional[str] = None
+):
     """Remove a label to an annotation in the Hectiq Console.
     If the label is not attached, nothing is done.
 
     Args:
         annotation_id (str): ID of the annotation
         label_id (str): ID of the label
         email (Optional[str], optional): Email. Defaults to None.
-        resource (Optional[str], optional): Ressource ID of the resource to which the annotation is related. 
+        resource (Optional[str], optional): Ressource ID of the resource to which the annotation is related.
             Defaults to None.
     """
     resource = get_resource(resource)
     headers = get_authentification_headers()
     email = get_email(email)
     assert email is not None, "You must set the email with `set_email` or use `hectiq-console authenticate --replace`."
-    params = {
-        "email": email
-    }
-    res = requests.post(f"{CONSOLE_APP_URL}/app/sender-client/{resource}/annotations/{annotation_id}/remove-label/{label_id}", 
-                 headers=headers, params=params)
-    if res.status_code != 200:
-        logger.error(f"⚠️ Error while attaching the label to the annotation with hectiq_console.remove_label_to_annotation: {res.text}")
+    params = {"email": email}
+    res = requests.post(
+        f"{CONSOLE_APP_URL}/app/sender-client/{resource}/annotations/{annotation_id}/remove-label/{label_id}",
+        headers=headers,
+        params=params,
+    )
+    if res.status_code != 200:
+        logger.error(
+            f"⚠️ Error while attaching the label to the annotation with hectiq_console.remove_label_to_annotation: {res.text}"
+        )
         return
-    
+
     return True
 
-def start_job(name: str, 
-              description: Optional[str] = None, 
-              metadata: Optional[Dict] = None,
-              status: Optional[str] = None,
-              log_level: int = logging.INFO,
-              logger_name: Optional[str] = None,
-              resource: Optional[str] = None):
-    """Start a job in the Hectiq Console.
-    """
+
+def start_job(
+    name: str,
+    description: Optional[str] = None,
+    metadata: Optional[Dict] = None,
+    status: Optional[str] = None,
+    log_level: int = logging.INFO,
+    logger_name: Optional[str] = None,
+    resource: Optional[str] = None,
+):
+    """Start a job in the Hectiq Console."""
 
     if get_job() is not None:
         # Current job already started
         return
-    
+
     resource = get_resource()
-    body = {"name": name, 
-            "description": description, 
-            "metadata": metadata,
-            "status": status or "running"}
+    body = {"name": name, "description": description, "metadata": metadata, "status": status or "running"}
     headers = get_authentification_headers()
-    res = requests.post(f"{CONSOLE_APP_URL}/app/sender-client/{resource}/jobs", 
-                 json=body, headers=headers)
+    res = requests.post(f"{CONSOLE_APP_URL}/app/sender-client/{resource}/jobs", json=body, headers=headers)
     if res.status_code != 200:
         logger.error(f"⚠️ Error while starting the job with hectiq_console.start_job: {res.text}")
         return
     job_id = res.json().get("id")
     set_job(job_id)
 
-    handler = MemoryHandler(name="hectiq-console-job-handler",
-                            capacity=100000, # Flush every 5000 lines
-                            target=append_current_job_logs)
-    formatter = logging.Formatter('%(asctime)s - %(levelname)s - %(message)s')
+    handler = MemoryHandler(
+        name="hectiq-console-job-handler", capacity=100000, target=append_current_job_logs  # Flush every 5000 lines
+    )
+    formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(message)s")
     handler.setFormatter(formatter)
     root = logging.getLogger(logger_name)
     root.addHandler(handler)
     root.setLevel(log_level)
     handler.setLevel(log_level)
 
     return True
 
+
 def end_job(status: Optional[str] = None):
-    """End the current job.
-    """
+    """End the current job."""
     job_id = get_job()
     if job_id is None:
         # No job started
         return
     resource = get_resource()
     headers = get_authentification_headers()
     body = {"status": status}
 
     root = logging.getLogger()
     handler = get_handler(logger=root, name="hectiq-console-job-handler")
     logs = handler.value() if handler is not None else None
-    if logs is not None and len(logs)>0:
+    if logs is not None and len(logs) > 0:
         if isinstance(logs, list):
             logs = "\n".join(logs)
         body["logs"] = logs
-    res = requests.post(f"{CONSOLE_APP_URL}/app/sender-client/{resource}/jobs/{job_id}/end", json=body, headers=headers)
+    res = requests.post(
+        f"{CONSOLE_APP_URL}/app/sender-client/{resource}/jobs/{job_id}/end", json=body, headers=headers
+    )
     if res.status_code != 200:
         logger.error(f"⚠️ Error while ending the job with hectiq_console.end_job: {res.text}")
         return
     set_job(None)
     if handler:
         handler.close(flush=False)
 
-def update_current_job(name: Optional[str] = None,
-                        description: Optional[str] = None, 
-                        metadata: Optional[Dict] = None,
-                        logs: Optional[str] = None,
-                        status: Optional[str] = None):
-    """Update the current job. 
+
+def update_current_job(
+    name: Optional[str] = None,
+    description: Optional[str] = None,
+    metadata: Optional[Dict] = None,
+    logs: Optional[str] = None,
+    status: Optional[str] = None,
+):
+    """Update the current job.
     Only the non-null values are updated.
     """
     job_id = get_job()
     if job_id is None:
         # No job started
         return
     resource = get_resource()
-    body = {"name": name, 
-        "description": description, 
-        "metadata": metadata,
-        "logs": logs,
-        "status": status}
+    body = {"name": name, "description": description, "metadata": metadata, "logs": logs, "status": status}
     # Remove null values
     body = {k: v for k, v in body.items() if v is not None}
-    if len(body)==0:
+    if len(body) == 0:
         return
     headers = get_authentification_headers()
-    res = requests.put(f"{CONSOLE_APP_URL}/app/sender-client/{resource}/jobs/{job_id}", 
-                json=body, headers=headers)
+    res = requests.put(f"{CONSOLE_APP_URL}/app/sender-client/{resource}/jobs/{job_id}", json=body, headers=headers)
     if res.status_code != 200:
         logger.error(f"⚠️ Error while updating the job with hectiq_console.update_current_job: {res.text}")
         return
     return True
 
+
 def append_current_job_logs(logs: Union[str, List[str]]):
     # Format the logs
-    if len(logs)==0:
+    if len(logs) == 0:
         return
     if isinstance(logs, list):
         logs = "\n".join(logs)
     update_current_job(logs=logs)
 
-def start_job_step(name: str, 
-              description: Optional[str] = None, 
-              metadata: Optional[Dict] = None,
-              status: Optional[str] = None,
-              log_level: int = logging.INFO,
-              logger_name: Optional[str] = None,
-              resource: Optional[str] = None):
-    """Start a job in the Hectiq Console.
-    """
+
+def start_job_step(
+    name: str,
+    description: Optional[str] = None,
+    metadata: Optional[Dict] = None,
+    status: Optional[str] = None,
+    log_level: int = logging.INFO,
+    logger_name: Optional[str] = None,
+    resource: Optional[str] = None,
+):
+    """Start a job in the Hectiq Console."""
     job = get_job()
     if job is None:
         # No job started
         return
-    
+
     if get_job_step() is not None:
         # Job step is started, close it
         end_job_step()
-    
+
     resource = get_resource()
-    body = {"name": name, 
-            "description": description, 
-            "metadata": metadata,
-            "status": status or "running"}
+    body = {"name": name, "description": description, "metadata": metadata, "status": status or "running"}
     headers = get_authentification_headers()
-    res = requests.post(f"{CONSOLE_APP_URL}/app/sender-client/{resource}/jobs/{job}/steps", 
-                 json=body, headers=headers)
+    res = requests.post(f"{CONSOLE_APP_URL}/app/sender-client/{resource}/jobs/{job}/steps", json=body, headers=headers)
     if res.status_code != 200:
         logger.error(f"⚠️ Error while starting the job step with hectiq_console.start_job_step: {res.text}")
         return
     step_id = res.json().get("id")
     set_job_step(step_id)
 
-    handler = MemoryHandler(name="hectiq-console-job-step-handler", 
-                            capacity=100000,
-                            target=append_current_job_step_logs)
-    formatter = logging.Formatter('%(asctime)s - %(levelname)s - %(message)s')
+    handler = MemoryHandler(
+        name="hectiq-console-job-step-handler", capacity=100000, target=append_current_job_step_logs
+    )
+    formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(message)s")
     handler.setFormatter(formatter)
     root = logging.getLogger(logger_name)
     root.addHandler(handler)
     root.setLevel(log_level)
 
     handler.setLevel(log_level)
 
     return True
 
+
 def end_job_step(status: Optional[str] = None):
-    """End the current job.
-    """
+    """End the current job."""
     job_id = get_job()
     if job_id is None:
         # No job started
         return
     step_id = get_job_step()
     if step_id is None:
         # No job step started
         return
     resource = get_resource()
     headers = get_authentification_headers()
     handler = get_handler(logger=logging.getLogger(), name="hectiq-console-job-step-handler")
     logs = handler.value() if handler is not None else None
     body = {"status": status}
-    if logs is not None and len(logs)>0:
+    if logs is not None and len(logs) > 0:
         if isinstance(logs, list):
             logs = "\n".join(logs)
         body["logs"] = logs
 
-    res = requests.post(f"{CONSOLE_APP_URL}/app/sender-client/{resource}/job-steps/{step_id}/end", json=body, headers=headers)
+    res = requests.post(
+        f"{CONSOLE_APP_URL}/app/sender-client/{resource}/job-steps/{step_id}/end", json=body, headers=headers
+    )
     if res.status_code != 200:
         logger.error(f"⚠️ Error while ending the job step with hectiq_console.end_job_step: {res.text}")
         return
     set_job_step(None)
     if handler:
         handler.close(flush=False)
 
-def update_current_job_step(name: Optional[str] = None,
-                          description: Optional[str] = None, 
-                          metadata: Optional[Dict] = None,
-                          status: Optional[str] = None,
-                          logs: Optional[str] = None):
-    """Update the current job. 
+
+def update_current_job_step(
+    name: Optional[str] = None,
+    description: Optional[str] = None,
+    metadata: Optional[Dict] = None,
+    status: Optional[str] = None,
+    logs: Optional[str] = None,
+):
+    """Update the current job.
     Only the non-null values are updated.
     """
     job_id = get_job()
     if job_id is None:
         # No job started
         return
     step_id = get_job_step()
     if step_id is None:
         # No job step started
         return
     resource = get_resource()
-    body = {"name": name, 
-        "description": description, 
-        "metadata": metadata,
-        "logs": logs,
-        "status": status}
+    body = {"name": name, "description": description, "metadata": metadata, "logs": logs, "status": status}
     # Remove null values
     body = {k: v for k, v in body.items() if v is not None}
-    if len(body)==0:
+    if len(body) == 0:
         return
     headers = get_authentification_headers()
-    res = requests.put(f"{CONSOLE_APP_URL}/app/sender-client/{resource}/job-steps/{step_id}", 
-                json=body, headers=headers)
+    res = requests.put(
+        f"{CONSOLE_APP_URL}/app/sender-client/{resource}/job-steps/{step_id}", json=body, headers=headers
+    )
     if res.status_code != 200:
         logger.error(f"⚠️ Error while updating the job step with hectiq_console.update_current_job_step: {res.text}")
         return
     return True
 
+
 def append_current_job_step_logs(logs: Union[str, List[str]]):
     # Format the logs
-    if len(logs)==0:
+    if len(logs) == 0:
         return
     if isinstance(logs, list):
         logs = "\n".join(logs)
     update_current_job_step(logs=logs)
 
+
 @inherit_docstring_from(BatchFetch, header="Below is the BatchFetch (parent) docstring")
 class BatchDownloadAnnotations(BatchFetch):
-    """A helper class to download annotations. 
+    """A helper class to download annotations.
 
     Example:
 
     ```python
     for annotations in BatchDownloadAnnotations(batch=100):
         print(f"✅ Downloaded {len(annotations)} annotations.")
     ```
     """
+
     @inherit_docstring_from(BatchFetch.__init__, header="BatchFetch.__init__ docstring.")
     def __init__(self, **kwargs):
         """The **kwargs are passed to the BatchFetch class.
         The method used is `hectiq_console.functional.download_annotations`.
         """
         super().__init__(method=download_annotations, **kwargs)
 
+
 @inherit_docstring_from(BatchFetch, header="Below is the BatchFetch (parent) docstring")
 class BatchSearchAnnotationLabels(BatchFetch):
-    """A helper class to search annotation labels. 
+    """A helper class to search annotation labels.
 
     Example:
 
     ```python
     for labels in BatchSearchAnnotationLabels(batch=100):
         print(f"✅ Downloaded {len(labels)} labels.")
     ```
     """
+
     @inherit_docstring_from(BatchFetch.__init__, header="BatchFetch.__init__ docstring.")
     def __init__(self, **kwargs):
         """The **kwargs are passed to the BatchFetch class.
         The method used is `hectiq_console.functional.search_annotation_labels`.
         """
         super().__init__(method=search_annotation_labels, **kwargs)
 
+
 @contextmanager
-def timer_context(name: str, 
-                  resource: Optional[str] = None):
+def timer_context(name: str, resource: Optional[str] = None):
     """Context manager to time a block of code.
 
     Args:
         key (str): Key of the timer
-        resource (Optional[str], optional): Ressource ID of the resource to which the timer is related. 
+        resource (Optional[str], optional): Ressource ID of the resource to which the timer is related.
             Defaults to None.
     """
     start = time.time()
     yield
     end = time.time()
     duration = end - start
     add_metrics(name=name, value=duration, resource=resource)
 
+
 @contextmanager
 def batch_annotations():
-    """Context manager to batch the creation of annotations.
-    """
+    """Context manager to batch the creation of annotations."""
 
     batch_annotations_cvar.set([])
     yield
-    if len(batch_annotations_cvar.get())>0:
+    if len(batch_annotations_cvar.get()) > 0:
         add_annotations(annotations=batch_annotations_cvar.get())
     batch_annotations_cvar.set(None)
 
+
 @contextmanager
-def job_context(name: str, 
-                description: Optional[str] = None, 
-                metadata: Optional[Dict] = None,
-                status: Optional[str] = None,
-                log_level: int = logging.INFO,
-                logger_name: Optional[str] = None,
-                timer_metrics: Optional[str] = None,
-                resource: Optional[str] = None):
+def job_context(
+    name: str,
+    description: Optional[str] = None,
+    metadata: Optional[Dict] = None,
+    status: Optional[str] = None,
+    log_level: int = logging.INFO,
+    logger_name: Optional[str] = None,
+    timer_metrics: Optional[str] = None,
+    resource: Optional[str] = None,
+):
     """Context manager to start a job.
 
     Args:
         name (str): Name of the job
         description (Optional[str], optional): Description of the job. Defaults to None.
         metadata (Optional[Dict], optional): Metadata of the job. Defaults to None.
         status (Optional[str], optional): Status of the job. Defaults to None.
-        resource (Optional[str], optional): Ressource ID of the resource to which the job is related. 
+        resource (Optional[str], optional): Ressource ID of the resource to which the job is related.
             Defaults to None.
         log_level (int, optional): Log level. Defaults to logging.INFO. Other possible values are:
             - logging.DEBUG = 10
             - logging.INFO = 20
             - logging.WARNING = 30
             - logging.ERROR = 40
             - logging.CRITICAL = 50
 
     """
-    start_job(name=name, 
-              description=description, 
-              metadata=metadata, 
-              status=status,
-              log_level=log_level,
-              logger_name=logger_name,
-              resource=resource)
-    
+    start_job(
+        name=name,
+        description=description,
+        metadata=metadata,
+        status=status,
+        log_level=log_level,
+        logger_name=logger_name,
+        resource=resource,
+    )
+
     exception_raised = False
     resource = get_resource(resource)
 
     try:
         if timer_metrics:
             with timer_context(name=timer_metrics, resource=resource):
                 yield
@@ -839,47 +888,52 @@
         if exception_raised:
             logger.error(traceback.format_exc())
             end_job_step(status="failed")
             end_job(status="failed")
         else:
             end_job_step()
             end_job()
-            
+
+
 @contextmanager
-def job_step_context(name: str, 
-                      description: Optional[str] = None, 
-                      metadata: Optional[Dict] = None,
-                      status: Optional[str] = None,
-                      log_level: int = logging.INFO,
-                      logger_name: Optional[str] = None,
-                      timer_metrics: Optional[str] = None,
-                      resource: Optional[str] = None):
+def job_step_context(
+    name: str,
+    description: Optional[str] = None,
+    metadata: Optional[Dict] = None,
+    status: Optional[str] = None,
+    log_level: int = logging.INFO,
+    logger_name: Optional[str] = None,
+    timer_metrics: Optional[str] = None,
+    resource: Optional[str] = None,
+):
     """Context manager to start a job step.
 
     Args:
         name (str): Name of the job step
         description (Optional[str], optional): Description of the job step. Defaults to None.
         metadata (Optional[Dict], optional): Metadata of the job step. Defaults to None.
         status (Optional[str], optional): Status of the job step. Defaults to None.
-        resource (Optional[str], optional): Ressource ID of the resource to which the job step is related. 
+        resource (Optional[str], optional): Ressource ID of the resource to which the job step is related.
             Defaults to None.
         log_level (int, optional): Log level. Defaults to logging.INFO. Other possible values are:
             - logging.DEBUG = 10
             - logging.INFO = 20
             - logging.WARNING = 30
             - logging.ERROR = 40
             - logging.CRITICAL = 50
     """
-    start_job_step(name=name, 
-              description=description, 
-              metadata=metadata, 
-              status=status,
-              log_level=log_level,
-              logger_name=logger_name,
-              resource=resource)
+    start_job_step(
+        name=name,
+        description=description,
+        metadata=metadata,
+        status=status,
+        log_level=log_level,
+        logger_name=logger_name,
+        resource=resource,
+    )
     exception_raised = False
     try:
         if timer_metrics:
             with timer_context(name=timer_metrics, resource=resource):
                 yield
         else:
             yield
@@ -888,8 +942,64 @@
         raise e
     finally:
         # Catch all exceptions to end the job step
         if exception_raised:
             logger.error(traceback.format_exc())
             end_job_step(status="failed")
         else:
-            end_job_step()
+            end_job_step()
+
+
+def download_model(name: str, version: str, savepath: str = "./") -> str:
+    """Download a model from the Hectiq Console. If savepath is a directory, 
+    the directory will be created and the model will be saved in a folder with the name and version.
+
+    Args:
+        model (str): ID of the model
+        version (str, optional): Version of the model. Default: None.
+        savepath (str, optional): Path to save the model. Default: "./"
+
+    Returns:
+        str: Path to the downloaded model
+    """
+    headers = get_authentification_headers()
+    params = {"name": name, "version": version}
+    res = requests.get(f"{CONSOLE_APP_URL}/app/sender-client/models/retrieve", headers=headers, params=params)
+    logger.info(f"Downloading the model {name} version {version}...")
+    if res.status_code != 200:
+        logger.error(f"⚠️ Error while downloading the model with hectiq_console.download_model: {res.text}")
+        return
+
+    model_id = res.json()["id"]
+    res = requests.get(
+        f"{CONSOLE_APP_URL}/app/sender-client/models/{model_id}/files",
+        headers=headers,
+        params={"limit": 2000, "fields": ["download_url"]},
+    )
+    if res.status_code != 200:
+        logger.error(f"⚠️ Error while downloading the model with hectiq_console.download_model: {res.text}")
+    savepath = os.path.join(savepath, name)
+    os.makedirs(savepath, exist_ok=True)
+    files = res.json()["results"]
+    urls = [file["download_url"] for file in files]
+    local_paths = [os.path.join(savepath, file["name"]) for file in files]
+    num_bytes = [file["num_bytes"] for file in files]
+    for url, path, byt in zip(urls, local_paths, num_bytes):
+        with open(path, "wb") as f:
+            if tqdm is None:
+                with requests.get(url, stream=True) as r:
+                    r.raise_for_status()
+                    logger.info("Downloading %s", path)
+                    for chunk in r.iter_content(chunk_size=8192):
+                        f.write(chunk)
+            else:
+                with tqdm.tqdm(
+                    total=byt, unit="iB", unit_scale=True, bar_format="{desc:<5.5}{percentage:3.0f}%|{bar:10}{r_bar}"
+                ) as pbar:
+                    with requests.get(url, stream=True) as r:
+                        r.raise_for_status()
+                        for chunk in r.iter_content(chunk_size=8192):
+                            f.write(chunk)
+                            pbar.update(len(chunk))
+                    
+    logger.info(f"Model {name} version {version} downloaded at {savepath}.")
+    return savepath
```

### Comparing `hectiq_console-1.2.0/hectiq_console/starlette/middleware.py` & `hectiq_console-1.2.1/hectiq_console/starlette/middleware.py`

 * *Files identical despite different names*

### Comparing `hectiq_console-1.2.0/hectiq_console/upload.py` & `hectiq_console-1.2.1/hectiq_console/upload.py`

 * *Files identical despite different names*

### Comparing `hectiq_console-1.2.0/hectiq_console/utils/batch_fetch.py` & `hectiq_console-1.2.1/hectiq_console/utils/batch_fetch.py`

 * *Files identical despite different names*

### Comparing `hectiq_console-1.2.0/hectiq_console/utils/log_handler.py` & `hectiq_console-1.2.1/hectiq_console/utils/log_handler.py`

 * *Files identical despite different names*

### Comparing `hectiq_console-1.2.0/hectiq_console.egg-info/PKG-INFO` & `hectiq_console-1.2.1/hectiq_console.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hectiq-console
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python client to use the Hectiq Console
 Home-page: https://console.hectiq.ai
 Author: Edward Laurence
 Author-email: edwardl@hectiq.ai
 Keywords: pip requirements imports
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
```

### Comparing `hectiq_console-1.2.0/hectiq_console.egg-info/SOURCES.txt` & `hectiq_console-1.2.1/hectiq_console.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hectiq_console-1.2.0/setup.py` & `hectiq_console-1.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
-__version__ = '1.2.0'
+__version__ = '1.2.1'
 
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 requirements = [
     "requests",
     "toml",
     "pydantic",
+    "tqdm",
     "click"]
 
 setup(
     name="hectiq_console",
     version=__version__,
     description="Python client to use the Hectiq Console",
     long_description=readme,
```

