# Comparing `tmp/asynctaskpool-0.1.0.post1.tar.gz` & `tmp/asynctaskpool-0.1.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asynctaskpool-0.1.0.post1.tar", max compression
+gzip compressed data, was "asynctaskpool-0.1.0.post2.tar", max compression
```

## Comparing `asynctaskpool-0.1.0.post1.tar` & `asynctaskpool-0.1.0.post2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      269 2024-04-17 01:27:05.871060 asynctaskpool-0.1.0.post1/README.md
--rw-r--r--   0        0        0       36 2024-04-17 01:22:02.972148 asynctaskpool-0.1.0.post1/asynctaskpool/__init__.py
--rw-r--r--   0        0        0     1151 2024-04-17 01:22:31.908809 asynctaskpool-0.1.0.post1/asynctaskpool/in_progress_task.py
--rw-r--r--   0        0        0     3963 2024-04-17 01:21:53.207925 asynctaskpool-0.1.0.post1/asynctaskpool/task_pool.py
--rw-r--r--   0        0        0      594 2024-04-17 02:13:02.382552 asynctaskpool-0.1.0.post1/pyproject.toml
--rw-r--r--   0        0        0      871 1970-01-01 00:00:00.000000 asynctaskpool-0.1.0.post1/PKG-INFO
+-rw-r--r--   0        0        0      269 2024-04-17 01:27:05.871060 asynctaskpool-0.1.0.post2/README.md
+-rw-r--r--   0        0        0       36 2024-04-17 01:22:02.972148 asynctaskpool-0.1.0.post2/asynctaskpool/__init__.py
+-rw-r--r--   0        0        0     1151 2024-04-17 01:22:31.908809 asynctaskpool-0.1.0.post2/asynctaskpool/in_progress_task.py
+-rw-r--r--   0        0        0     3963 2024-04-17 01:21:53.207925 asynctaskpool-0.1.0.post2/asynctaskpool/task_pool.py
+-rw-r--r--   0        0        0      595 2024-04-17 02:37:00.985922 asynctaskpool-0.1.0.post2/pyproject.toml
+-rw-r--r--   0        0        0      917 1970-01-01 00:00:00.000000 asynctaskpool-0.1.0.post2/PKG-INFO
```

### Comparing `asynctaskpool-0.1.0.post1/asynctaskpool/in_progress_task.py` & `asynctaskpool-0.1.0.post2/asynctaskpool/in_progress_task.py`

 * *Files identical despite different names*

### Comparing `asynctaskpool-0.1.0.post1/asynctaskpool/task_pool.py` & `asynctaskpool-0.1.0.post2/asynctaskpool/task_pool.py`

 * *Files identical despite different names*

### Comparing `asynctaskpool-0.1.0.post1/PKG-INFO` & `asynctaskpool-0.1.0.post2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: asynctaskpool
-Version: 0.1.0.post1
+Version: 0.1.0.post2
 Summary: Provides a task pool for asynchronous tasks to be executed only once.
 Home-page: https://codeberg.org/QCanvas/AsyncTaskPool
 Keywords: async,taskpool
 Author: QCanvas
 Author-email: qcanvas@noreply.codeberg.org
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10
 Classifier: Framework :: AsyncIO
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Repository, https://codeberg.org/QCanvas/AsyncTaskPool
 Description-Content-Type: text/markdown
 
 # AsyncTaskPool
```

