# Comparing `tmp/zephyr-python-api-0.0.4.tar.gz` & `tmp/zephyr_python_api-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zephyr-python-api-0.0.4.tar", last modified: Fri Jan  5 21:00:57 2024, max compression
+gzip compressed data, was "zephyr_python_api-0.0.5.tar", last modified: Wed Apr 17 11:29:36 2024, max compression
```

## Comparing `zephyr-python-api-0.0.4.tar` & `zephyr_python_api-0.0.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 21:00:57.578097 zephyr-python-api-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11345 2024-01-05 21:00:32.000000 zephyr-python-api-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-01-05 21:00:57.578097 zephyr-python-api-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-01-05 21:00:32.000000 zephyr-python-api-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-05 21:00:32.000000 zephyr-python-api-0.0.4/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-01-05 21:00:32.000000 zephyr-python-api-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-01-05 21:00:57.578097 zephyr-python-api-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 21:00:57.570097 zephyr-python-api-0.0.4/zephyr/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-01-05 21:00:32.000000 zephyr-python-api-0.0.4/zephyr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 21:00:57.574097 zephyr-python-api-0.0.4/zephyr/scale/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-05 21:00:32.000000 zephyr-python-api-0.0.4/zephyr/scale/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 21:00:57.574097 zephyr-python-api-0.0.4/zephyr/scale/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 21:00:32.000000 zephyr-python-api-0.0.4/zephyr/scale/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-01-05 21:00:32.000000 zephyr-python-api-0.0.4/zephyr/scale/cloud/cloud_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 21:00:57.574097 zephyr-python-api-0.0.4/zephyr/scale/cloud/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-01-05 21:00:32.000000 zephyr-python-api-0.0.4/zephyr/scale/cloud/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-01-05 21:00:32.000000 zephyr-python-api-0.0.4/zephyr/scale/cloud/endpoints/automations.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-01-05 21:00:32.000000 zephyr-python-api-0.0.4/zephyr/scale/cloud/endpoints/environments.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-01-05 21:00:32.000000 zephyr-python-api-0.0.4/zephyr/scale/cloud/endpoints/folders.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-01-05 21:00:32.000000 zephyr-python-api-0.0.4/zephyr/scale/cloud/endpoints/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-01-05 21:00:32.000000 zephyr-python-api-0.0.4/zephyr/scale/cloud/endpoints/links.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-01-05 21:00:32.000000 zephyr-python-api-0.0.4/zephyr/scale/cloud/endpoints/priorities.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-01-05 21:00:32.000000 zephyr-python-api-0.0.4/zephyr/scale/cloud/endpoints/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-01-05 21:00:32.000000 zephyr-python-api-0.0.4/zephyr/scale/cloud/endpoints/statuses.py
--rw-r--r--   0 runner    (1001) docker     (127)     6182 2024-01-05 21:00:32.000000 zephyr-python-api-0.0.4/zephyr/scale/cloud/endpoints/test_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-01-05 21:00:32.000000 zephyr-python-api-0.0.4/zephyr/scale/cloud/endpoints/test_cycles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-01-05 21:00:32.000000 zephyr-python-api-0.0.4/zephyr/scale/cloud/endpoints/test_executions.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-01-05 21:00:32.000000 zephyr-python-api-0.0.4/zephyr/scale/cloud/endpoints/test_plans.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-01-05 21:00:32.000000 zephyr-python-api-0.0.4/zephyr/scale/scale.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 21:00:57.574097 zephyr-python-api-0.0.4/zephyr/scale/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 21:00:32.000000 zephyr-python-api-0.0.4/zephyr/scale/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 21:00:57.574097 zephyr-python-api-0.0.4/zephyr/scale/server/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-01-05 21:00:32.000000 zephyr-python-api-0.0.4/zephyr/scale/server/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15428 2024-01-05 21:00:32.000000 zephyr-python-api-0.0.4/zephyr/scale/server/endpoints/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-01-05 21:00:32.000000 zephyr-python-api-0.0.4/zephyr/scale/server/endpoints/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-01-05 21:00:32.000000 zephyr-python-api-0.0.4/zephyr/scale/server/server_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-01-05 21:00:32.000000 zephyr-python-api-0.0.4/zephyr/scale/server/server_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-01-05 21:00:32.000000 zephyr-python-api-0.0.4/zephyr/scale/zephyr_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 21:00:57.578097 zephyr-python-api-0.0.4/zephyr/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 21:00:32.000000 zephyr-python-api-0.0.4/zephyr/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-01-05 21:00:32.000000 zephyr-python-api-0.0.4/zephyr/utils/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 21:00:57.578097 zephyr-python-api-0.0.4/zephyr_python_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-01-05 21:00:57.000000 zephyr-python-api-0.0.4/zephyr_python_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-01-05 21:00:57.000000 zephyr-python-api-0.0.4/zephyr_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-05 21:00:57.000000 zephyr-python-api-0.0.4/zephyr_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-05 21:00:57.000000 zephyr-python-api-0.0.4/zephyr_python_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-05 21:00:57.000000 zephyr-python-api-0.0.4/zephyr_python_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:29:36.475239 zephyr_python_api-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11345 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-17 11:29:36.475239 zephyr_python_api-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-17 11:29:36.475239 zephyr_python_api-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:29:36.467239 zephyr_python_api-0.0.5/zephyr/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:29:36.471239 zephyr_python_api-0.0.5/zephyr/scale/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:29:36.471239 zephyr_python_api-0.0.5/zephyr/scale/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/cloud/cloud_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:29:36.471239 zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/automations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/folders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/priorities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/statuses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6182 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/test_cycles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/test_executions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/test_plans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/scale.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:29:36.471239 zephyr_python_api-0.0.5/zephyr/scale/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:29:36.471239 zephyr_python_api-0.0.5/zephyr/scale/server/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/server/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15427 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/server/endpoints/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/server/endpoints/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/server/server_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/server/server_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/scale/zephyr_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:29:36.475239 zephyr_python_api-0.0.5/zephyr/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-17 11:29:05.000000 zephyr_python_api-0.0.5/zephyr/utils/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 11:29:36.475239 zephyr_python_api-0.0.5/zephyr_python_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-17 11:29:36.000000 zephyr_python_api-0.0.5/zephyr_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-17 11:29:36.000000 zephyr_python_api-0.0.5/zephyr_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 11:29:36.000000 zephyr_python_api-0.0.5/zephyr_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 11:29:36.000000 zephyr_python_api-0.0.5/zephyr_python_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 11:29:36.000000 zephyr_python_api-0.0.5/zephyr_python_api.egg-info/top_level.txt
```

### Comparing `zephyr-python-api-0.0.4/LICENSE` & `zephyr_python_api-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zephyr-python-api-0.0.4/PKG-INFO` & `zephyr_python_api-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zephyr-python-api
-Version: 0.0.4
+Version: 0.0.5
 Summary: Zephyr (TM4J) Python REST API wrapper
 Home-page: https://github.com/nassauwinter/zephyr-python-api
 Author: Petr Sharapenko
 Author-email: nassauwinter@gmail.com
 Project-URL: Bug Tracker, https://github.com/nassauwinter/zephyr-python-api/issues
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `zephyr-python-api-0.0.4/README.md` & `zephyr_python_api-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `zephyr-python-api-0.0.4/setup.cfg` & `zephyr_python_api-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `zephyr-python-api-0.0.4/zephyr/scale/cloud/cloud_api.py` & `zephyr_python_api-0.0.5/zephyr/scale/cloud/cloud_api.py`

 * *Files identical despite different names*

### Comparing `zephyr-python-api-0.0.4/zephyr/scale/cloud/endpoints/automations.py` & `zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/automations.py`

 * *Files identical despite different names*

### Comparing `zephyr-python-api-0.0.4/zephyr/scale/cloud/endpoints/environments.py` & `zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/environments.py`

 * *Files identical despite different names*

### Comparing `zephyr-python-api-0.0.4/zephyr/scale/cloud/endpoints/folders.py` & `zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/folders.py`

 * *Files identical despite different names*

### Comparing `zephyr-python-api-0.0.4/zephyr/scale/cloud/endpoints/test_cases.py` & `zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/test_cases.py`

 * *Files identical despite different names*

### Comparing `zephyr-python-api-0.0.4/zephyr/scale/cloud/endpoints/test_cycles.py` & `zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/test_cycles.py`

 * *Files identical despite different names*

### Comparing `zephyr-python-api-0.0.4/zephyr/scale/cloud/endpoints/test_executions.py` & `zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/test_executions.py`

 * *Files identical despite different names*

### Comparing `zephyr-python-api-0.0.4/zephyr/scale/cloud/endpoints/test_plans.py` & `zephyr_python_api-0.0.5/zephyr/scale/cloud/endpoints/test_plans.py`

 * *Files identical despite different names*

### Comparing `zephyr-python-api-0.0.4/zephyr/scale/scale.py` & `zephyr_python_api-0.0.5/zephyr/scale/scale.py`

 * *Files identical despite different names*

### Comparing `zephyr-python-api-0.0.4/zephyr/scale/server/endpoints/__init__.py` & `zephyr_python_api-0.0.5/zephyr/scale/server/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `zephyr-python-api-0.0.4/zephyr/scale/server/endpoints/endpoints.py` & `zephyr_python_api-0.0.5/zephyr/scale/server/endpoints/endpoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
                                  json=json)
 
     def update_test_result(self, test_run_key, test_case_key, **json):
         """
         Updates the last Test Result on the specified Test Run, looking for an item that matches
         the testCaseKey and the query string filter parameters. Only defined fields will be updated.
         """
-        return self.session.post(Paths.RUN_TEST_RESULT.format(test_run_key, test_case_key),
+        return self.session.put(Paths.RUN_TEST_RESULT.format(test_run_key, test_case_key),
                                  json=json)
 
     def get_test_results(self, test_run_key):
         """Retrieve All Test Results linked to a Test Run"""
         return self.session.get(Paths.RUN_TEST_RESULTS.format(test_run_key))
 
     def create_test_results(self, test_run_key, results):
```

### Comparing `zephyr-python-api-0.0.4/zephyr/scale/server/endpoints/paths.py` & `zephyr_python_api-0.0.5/zephyr/scale/server/endpoints/paths.py`

 * *Files identical despite different names*

### Comparing `zephyr-python-api-0.0.4/zephyr/scale/server/server_api.py` & `zephyr_python_api-0.0.5/zephyr/scale/server/server_api.py`

 * *Files identical despite different names*

### Comparing `zephyr-python-api-0.0.4/zephyr/scale/server/server_defaults.py` & `zephyr_python_api-0.0.5/zephyr/scale/server/server_defaults.py`

 * *Files identical despite different names*

### Comparing `zephyr-python-api-0.0.4/zephyr/scale/zephyr_session.py` & `zephyr_python_api-0.0.5/zephyr/scale/zephyr_session.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,20 +89,23 @@
         if params is None:
             params = {}
 
         while True:
             response = self.get(endpoint, params=params)
             if "values" not in response:
                 return
-            for value in response.get("values", []):
-                yield value
+
+            yield from response.get("values", [])
+
             if response.get("isLast") is True:
                 break
+
             params_str = urlparse(response.get("next")).query
             params.update(parse_qs(params_str))
+
         return
 
     def post_file(self, endpoint: str, file_path: str, to_files=None, **kwargs):
         """
         Post wrapper to send a file. Handles single file opening,
         sending its content and closing
         """
```

### Comparing `zephyr-python-api-0.0.4/zephyr/utils/common.py` & `zephyr_python_api-0.0.5/zephyr/utils/common.py`

 * *Files identical despite different names*

### Comparing `zephyr-python-api-0.0.4/zephyr_python_api.egg-info/PKG-INFO` & `zephyr_python_api-0.0.5/zephyr_python_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zephyr-python-api
-Version: 0.0.4
+Version: 0.0.5
 Summary: Zephyr (TM4J) Python REST API wrapper
 Home-page: https://github.com/nassauwinter/zephyr-python-api
 Author: Petr Sharapenko
 Author-email: nassauwinter@gmail.com
 Project-URL: Bug Tracker, https://github.com/nassauwinter/zephyr-python-api/issues
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `zephyr-python-api-0.0.4/zephyr_python_api.egg-info/SOURCES.txt` & `zephyr_python_api-0.0.5/zephyr_python_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

