# Comparing `tmp/pr_pilot-1.0.3.tar.gz` & `tmp/pr_pilot-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pr_pilot-1.0.3.tar", last modified: Sat Apr 13 04:49:24 2024, max compression
+gzip compressed data, was "pr_pilot-1.0.4.tar", last modified: Wed Apr 17 00:16:37 2024, max compression
```

## Comparing `pr_pilot-1.0.3.tar` & `pr_pilot-1.0.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:49:24.222672 pr_pilot-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-13 04:49:20.000000 pr_pilot-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-13 04:49:20.000000 pr_pilot-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-13 04:49:24.222672 pr_pilot-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-13 04:49:20.000000 pr_pilot-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:49:24.222672 pr_pilot-1.0.3/pr_pilot/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-13 04:49:20.000000 pr_pilot-1.0.3/pr_pilot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:49:24.222672 pr_pilot-1.0.3/pr_pilot/api/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-13 04:49:20.000000 pr_pilot-1.0.3/pr_pilot/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11037 2024-04-13 04:49:20.000000 pr_pilot-1.0.3/pr_pilot/api/task_creation_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-04-13 04:49:20.000000 pr_pilot-1.0.3/pr_pilot/api/task_retrieval_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26236 2024-04-13 04:49:20.000000 pr_pilot-1.0.3/pr_pilot/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-13 04:49:20.000000 pr_pilot-1.0.3/pr_pilot/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    15420 2024-04-13 04:49:20.000000 pr_pilot-1.0.3/pr_pilot/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-04-13 04:49:20.000000 pr_pilot-1.0.3/pr_pilot/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:49:24.222672 pr_pilot-1.0.3/pr_pilot/models/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-13 04:49:20.000000 pr_pilot-1.0.3/pr_pilot/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-13 04:49:20.000000 pr_pilot-1.0.3/pr_pilot/models/bad_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-13 04:49:20.000000 pr_pilot-1.0.3/pr_pilot/models/not_found.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-13 04:49:20.000000 pr_pilot-1.0.3/pr_pilot/models/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-13 04:49:20.000000 pr_pilot-1.0.3/pr_pilot/models/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     9332 2024-04-13 04:49:20.000000 pr_pilot-1.0.3/pr_pilot/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:49:24.222672 pr_pilot-1.0.3/pr_pilot/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 04:49:20.000000 pr_pilot-1.0.3/pr_pilot/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-13 04:49:20.000000 pr_pilot-1.0.3/pr_pilot/test/test_bad_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-13 04:49:20.000000 pr_pilot-1.0.3/pr_pilot/test/test_not_found.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-13 04:49:20.000000 pr_pilot-1.0.3/pr_pilot/test/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-13 04:49:20.000000 pr_pilot-1.0.3/pr_pilot/test/test_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-13 04:49:20.000000 pr_pilot-1.0.3/pr_pilot/test/test_task_creation_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-13 04:49:20.000000 pr_pilot-1.0.3/pr_pilot/test/test_task_retrieval_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-13 04:49:20.000000 pr_pilot-1.0.3/pr_pilot/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 04:49:24.222672 pr_pilot-1.0.3/pr_pilot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-13 04:49:24.000000 pr_pilot-1.0.3/pr_pilot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-13 04:49:24.000000 pr_pilot-1.0.3/pr_pilot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 04:49:24.000000 pr_pilot-1.0.3/pr_pilot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-13 04:49:24.000000 pr_pilot-1.0.3/pr_pilot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 04:49:24.000000 pr_pilot-1.0.3/pr_pilot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-13 04:49:20.000000 pr_pilot-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 04:49:24.222672 pr_pilot-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-13 04:49:20.000000 pr_pilot-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:16:37.125172 pr_pilot-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-17 00:16:30.000000 pr_pilot-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 00:16:30.000000 pr_pilot-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-17 00:16:37.125172 pr_pilot-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-17 00:16:30.000000 pr_pilot-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:16:37.121172 pr_pilot-1.0.4/pr_pilot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-17 00:16:30.000000 pr_pilot-1.0.4/pr_pilot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:16:37.121172 pr_pilot-1.0.4/pr_pilot/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-17 00:16:30.000000 pr_pilot-1.0.4/pr_pilot/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11037 2024-04-17 00:16:30.000000 pr_pilot-1.0.4/pr_pilot/api/task_creation_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-04-17 00:16:30.000000 pr_pilot-1.0.4/pr_pilot/api/task_retrieval_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26236 2024-04-17 00:16:30.000000 pr_pilot-1.0.4/pr_pilot/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-17 00:16:30.000000 pr_pilot-1.0.4/pr_pilot/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15420 2024-04-17 00:16:30.000000 pr_pilot-1.0.4/pr_pilot/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-04-17 00:16:30.000000 pr_pilot-1.0.4/pr_pilot/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:16:37.121172 pr_pilot-1.0.4/pr_pilot/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-17 00:16:30.000000 pr_pilot-1.0.4/pr_pilot/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-17 00:16:30.000000 pr_pilot-1.0.4/pr_pilot/models/bad_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-17 00:16:30.000000 pr_pilot-1.0.4/pr_pilot/models/not_found.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-17 00:16:30.000000 pr_pilot-1.0.4/pr_pilot/models/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-17 00:16:30.000000 pr_pilot-1.0.4/pr_pilot/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9332 2024-04-17 00:16:30.000000 pr_pilot-1.0.4/pr_pilot/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:16:37.125172 pr_pilot-1.0.4/pr_pilot/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 00:16:30.000000 pr_pilot-1.0.4/pr_pilot/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-17 00:16:30.000000 pr_pilot-1.0.4/pr_pilot/test/test_bad_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-17 00:16:30.000000 pr_pilot-1.0.4/pr_pilot/test/test_not_found.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-17 00:16:30.000000 pr_pilot-1.0.4/pr_pilot/test/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-17 00:16:30.000000 pr_pilot-1.0.4/pr_pilot/test/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-17 00:16:30.000000 pr_pilot-1.0.4/pr_pilot/test/test_task_creation_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-17 00:16:30.000000 pr_pilot-1.0.4/pr_pilot/test/test_task_retrieval_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-17 00:16:30.000000 pr_pilot-1.0.4/pr_pilot/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:16:37.125172 pr_pilot-1.0.4/pr_pilot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-17 00:16:37.000000 pr_pilot-1.0.4/pr_pilot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-17 00:16:37.000000 pr_pilot-1.0.4/pr_pilot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 00:16:37.000000 pr_pilot-1.0.4/pr_pilot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-17 00:16:37.000000 pr_pilot-1.0.4/pr_pilot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 00:16:37.000000 pr_pilot-1.0.4/pr_pilot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-17 00:16:30.000000 pr_pilot-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 00:16:37.125172 pr_pilot-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-17 00:16:30.000000 pr_pilot-1.0.4/setup.py
```

### Comparing `pr_pilot-1.0.3/LICENSE` & `pr_pilot-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.0.3/PKG-INFO` & `pr_pilot-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr_pilot
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python SDK for PR Pilot, a text-to-task automation platform for Github.
 Home-page: https://github.com/PR-Pilot-AI/pr-pilot-python
 Author: Marco Lamina
 Author-email: marco@pr-pilot.ai
 License: GPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pr_pilot Version: 1.0.3 Summary: Python SDK for PR
+Metadata-Version: 2.1 Name: pr_pilot Version: 1.0.4 Summary: Python SDK for PR
 Pilot, a text-to-task automation platform for Github. Home-page: https://
 github.com/PR-Pilot-AI/pr-pilot-python Author: Marco Lamina Author-email:
 marco@pr-pilot.ai License: GPL-3.0 Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: pydantic==2.7.0 Requires-Dist:
 urllib3==2.2.1 Requires-Dist: python-dateutil==2.9.0 Requires-Dist:
```

### Comparing `pr_pilot-1.0.3/README.md` & `pr_pilot-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.0.3/pr_pilot/__init__.py` & `pr_pilot-1.0.4/pr_pilot/__init__.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.0.3/pr_pilot/api/task_creation_api.py` & `pr_pilot-1.0.4/pr_pilot/api/task_creation_api.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.0.3/pr_pilot/api/task_retrieval_api.py` & `pr_pilot-1.0.4/pr_pilot/api/task_retrieval_api.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.0.3/pr_pilot/api_client.py` & `pr_pilot-1.0.4/pr_pilot/api_client.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.0.3/pr_pilot/api_response.py` & `pr_pilot-1.0.4/pr_pilot/api_response.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.0.3/pr_pilot/configuration.py` & `pr_pilot-1.0.4/pr_pilot/configuration.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.0.3/pr_pilot/exceptions.py` & `pr_pilot-1.0.4/pr_pilot/exceptions.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.0.3/pr_pilot/models/bad_request.py` & `pr_pilot-1.0.4/pr_pilot/models/bad_request.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.0.3/pr_pilot/models/not_found.py` & `pr_pilot-1.0.4/pr_pilot/models/not_found.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.0.3/pr_pilot/models/prompt.py` & `pr_pilot-1.0.4/pr_pilot/models/prompt.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.0.3/pr_pilot/models/task.py` & `pr_pilot-1.0.4/pr_pilot/models/task.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.0.3/pr_pilot/rest.py` & `pr_pilot-1.0.4/pr_pilot/rest.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.0.3/pr_pilot/test/test_bad_request.py` & `pr_pilot-1.0.4/pr_pilot/test/test_bad_request.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.0.3/pr_pilot/test/test_not_found.py` & `pr_pilot-1.0.4/pr_pilot/test/test_not_found.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.0.3/pr_pilot/test/test_prompt.py` & `pr_pilot-1.0.4/pr_pilot/test/test_prompt.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.0.3/pr_pilot/test/test_task.py` & `pr_pilot-1.0.4/pr_pilot/test/test_task.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.0.3/pr_pilot/test/test_task_creation_api.py` & `pr_pilot-1.0.4/pr_pilot/test/test_task_creation_api.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.0.3/pr_pilot/test/test_task_retrieval_api.py` & `pr_pilot-1.0.4/pr_pilot/test/test_task_retrieval_api.py`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.0.3/pr_pilot/util.py` & `pr_pilot-1.0.4/pr_pilot/util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,50 @@
+import logging
 import os
-import time
 
 import pr_pilot
 from pr_pilot import Task, Prompt
 
+logger = logging.getLogger(__name__)
+
 
 def _get_config_from_env():
     configuration = pr_pilot.Configuration(
         host="https://app.pr-pilot.ai",
     )
     if not os.environ.get("PR_PILOT_API_KEY"):
         raise ValueError("Please set the PR_PILOT_API_KEY environment variable.")
     configuration.api_key['apiKeyAuth'] = os.environ["PR_PILOT_API_KEY"]
     return configuration
 
 
-def create_task(repo: str, prompt: str) -> Task:
+def set_github_action_output(key: str, value: str):
+    """Set an output parameter for GitHub Actions."""
+    # Get the path to the environment file for outputs
+    output_file = os.getenv('GITHUB_OUTPUT')
+
+    # Ensure the output file path is available
+    if output_file is not None:
+        with open(output_file, "a") as file:
+            file.write(f"{key}={value}\n")
+    else:
+        logger.debug("GITHUB_OUTPUT environment variable is not set.")
+
+
+def create_task(repo: str, prompt: str, log=True) -> Task:
     """Create a task for the specified repository with the given prompt."""
     with pr_pilot.ApiClient(_get_config_from_env()) as api_client:
         api_instance = pr_pilot.TaskCreationApi(api_client)
-        return api_instance.tasks_create(Prompt(prompt=prompt, github_repo=repo))
+        task = api_instance.tasks_create(Prompt(prompt=prompt, github_repo=repo))
+        dashboard_url = f"https://app.pr-pilot.ai/dashboard/tasks/{str(task.id)}/"
+        set_github_action_output("task-id", str(task.id))
+        set_github_action_output("task-url", dashboard_url)
+        if log:
+            logger.info(f"PR Pilot task created: {dashboard_url}")
+        return task
 
 
 def get_task(task_id: str) -> Task:
     """Get the task with the specified ID."""
     with pr_pilot.ApiClient(_get_config_from_env()) as api_client:
         api_instance = pr_pilot.TaskRetrievalApi(api_client)
         return api_instance.tasks_retrieve(task_id)
```

### Comparing `pr_pilot-1.0.3/pr_pilot.egg-info/PKG-INFO` & `pr_pilot-1.0.4/pr_pilot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr_pilot
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python SDK for PR Pilot, a text-to-task automation platform for Github.
 Home-page: https://github.com/PR-Pilot-AI/pr-pilot-python
 Author: Marco Lamina
 Author-email: marco@pr-pilot.ai
 License: GPL-3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pr_pilot Version: 1.0.3 Summary: Python SDK for PR
+Metadata-Version: 2.1 Name: pr_pilot Version: 1.0.4 Summary: Python SDK for PR
 Pilot, a text-to-task automation platform for Github. Home-page: https://
 github.com/PR-Pilot-AI/pr-pilot-python Author: Marco Lamina Author-email:
 marco@pr-pilot.ai License: GPL-3.0 Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: pydantic==2.7.0 Requires-Dist:
 urllib3==2.2.1 Requires-Dist: python-dateutil==2.9.0 Requires-Dist:
```

### Comparing `pr_pilot-1.0.3/pr_pilot.egg-info/SOURCES.txt` & `pr_pilot-1.0.4/pr_pilot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pr_pilot-1.0.3/setup.py` & `pr_pilot-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 this_dir = path.abspath(path.dirname(__file__))
 requirements_path = path.join(this_dir, 'requirements.txt')
 with open(requirements_path) as f:
     required = f.read().splitlines()
 
 setup(
     name='pr_pilot',
-    version='1.0.3',
+    version='1.0.4',
     packages=find_packages(),
     install_requires=required,
     python_requires='>=3.6',
     author='Marco Lamina',
     author_email='marco@pr-pilot.ai',
     description='Python SDK for PR Pilot, a text-to-task automation platform for Github.',
     long_description=open('README.md').read(),
```

