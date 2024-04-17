# Comparing `tmp/ataskq-0.4.1.tar.gz` & `tmp/ataskq-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ataskq-0.4.1.tar", last modified: Sun Oct 22 20:03:15 2023, max compression
+gzip compressed data, was "ataskq-5.0.0.tar", last modified: Wed Apr 17 20:31:31 2024, max compression
```

## Comparing `ataskq-0.4.1.tar` & `ataskq-5.0.0.tar`

### file list

```diff
@@ -1,24 +1,49 @@
-drwxr-xr-x   0 markk     (1000) markk     (1000)        0 2023-10-22 20:03:15.713050 ataskq-0.4.1/
--rw-r--r--   0 markk     (1000) markk     (1000)     1068 2023-10-22 19:44:43.000000 ataskq-0.4.1/LICENSE
--rw-r--r--   0 markk     (1000) markk     (1000)      442 2023-10-22 20:03:15.713050 ataskq-0.4.1/PKG-INFO
--rw-r--r--   0 markk     (1000) markk     (1000)       75 2023-10-22 19:44:43.000000 ataskq-0.4.1/README.md
-drwxr-xr-x   0 markk     (1000) markk     (1000)        0 2023-10-22 20:03:15.713050 ataskq-0.4.1/ataskq/
--rw-r--r--   0 markk     (1000) markk     (1000)      198 2023-10-22 19:44:43.000000 ataskq-0.4.1/ataskq/__init__.py
--rw-r--r--   0 markk     (1000) markk     (1000)     8278 2023-10-22 19:44:43.000000 ataskq-0.4.1/ataskq/ataskq.py
--rw-r--r--   0 markk     (1000) markk     (1000)    11511 2023-10-22 19:44:43.000000 ataskq-0.4.1/ataskq/db_handler.py
--rw-r--r--   0 markk     (1000) markk     (1000)      664 2023-10-22 19:44:43.000000 ataskq-0.4.1/ataskq/logger.py
--rw-r--r--   0 markk     (1000) markk     (1000)      824 2023-10-22 19:44:43.000000 ataskq-0.4.1/ataskq/monitor.py
--rw-r--r--   0 markk     (1000) markk     (1000)     2980 2023-10-22 19:44:43.000000 ataskq-0.4.1/ataskq/server.py
--rw-r--r--   0 markk     (1000) markk     (1000)      925 2023-10-22 19:44:43.000000 ataskq-0.4.1/ataskq/task.py
-drwxr-xr-x   0 markk     (1000) markk     (1000)        0 2023-10-22 20:03:15.713050 ataskq-0.4.1/ataskq/templates/
--rw-r--r--   0 markk     (1000) markk     (1000)     6752 2023-10-22 19:44:43.000000 ataskq-0.4.1/ataskq/templates/base.html
--rw-r--r--   0 markk     (1000) markk     (1000)     3253 2023-10-22 19:44:43.000000 ataskq-0.4.1/ataskq/test_db_handler.py
--rw-r--r--   0 markk     (1000) markk     (1000)     5392 2023-10-22 19:44:43.000000 ataskq-0.4.1/ataskq/test_run.py
--rw-r--r--   0 markk     (1000) markk     (1000)       44 2023-10-22 20:03:13.000000 ataskq-0.4.1/ataskq/version.py
-drwxr-xr-x   0 markk     (1000) markk     (1000)        0 2023-10-22 20:03:15.713050 ataskq-0.4.1/ataskq.egg-info/
--rw-r--r--   0 markk     (1000) markk     (1000)      442 2023-10-22 20:03:15.000000 ataskq-0.4.1/ataskq.egg-info/PKG-INFO
--rw-r--r--   0 markk     (1000) markk     (1000)      360 2023-10-22 20:03:15.000000 ataskq-0.4.1/ataskq.egg-info/SOURCES.txt
--rw-r--r--   0 markk     (1000) markk     (1000)        1 2023-10-22 20:03:15.000000 ataskq-0.4.1/ataskq.egg-info/dependency_links.txt
--rw-r--r--   0 markk     (1000) markk     (1000)        7 2023-10-22 20:03:15.000000 ataskq-0.4.1/ataskq.egg-info/top_level.txt
--rw-r--r--   0 markk     (1000) markk     (1000)       38 2023-10-22 20:03:15.713050 ataskq-0.4.1/setup.cfg
--rw-r--r--   0 markk     (1000) markk     (1000)      822 2023-10-22 19:44:43.000000 ataskq-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:31:31.907540 ataskq-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-17 20:31:11.000000 ataskq-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-17 20:31:31.907540 ataskq-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-17 20:31:11.000000 ataskq-5.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:31:31.903540 ataskq-5.0.0/ataskq/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12687 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/ataskq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:31:31.903540 ataskq-5.0.0/ataskq/handler/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17044 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/handler/db_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/handler/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/handler/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/handler/rest_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/handler/sqlite3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/imodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15812 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:31:31.903540 ataskq-5.0.0/ataskq/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/server/form_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6085 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:31:31.907540 ataskq-5.0.0/ataskq/server/www/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:31:31.907540 ataskq-5.0.0/ataskq/server/www/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    24285 2024-04-17 20:31:20.000000 ataskq-5.0.0/ataskq/server/www/assets/index-MiCEdQXI.js
+-rw-r--r--   0 runner    (1001) docker     (127)    70928 2024-04-17 20:31:20.000000 ataskq-5.0.0/ataskq/server/www/assets/index-MiCEdQXI.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-17 20:31:20.000000 ataskq-5.0.0/ataskq/server/www/assets/index-_NWmBfbC.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-17 20:31:20.000000 ataskq-5.0.0/ataskq/server/www/ataskq-32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-17 20:31:20.000000 ataskq-5.0.0/ataskq/server/www/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-17 20:31:20.000000 ataskq-5.0.0/ataskq/server/www/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 20:31:20.000000 ataskq-5.0.0/ataskq/server/www/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:31:31.907540 ataskq-5.0.0/ataskq/tasks_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/tasks_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/tasks_utils/counter_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/tasks_utils/write_to_file_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/test_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16313 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/test_ataskq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/test_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-17 20:31:11.000000 ataskq-5.0.0/ataskq/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 20:31:20.000000 ataskq-5.0.0/ataskq/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:31:31.907540 ataskq-5.0.0/ataskq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-17 20:31:31.000000 ataskq-5.0.0/ataskq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-17 20:31:31.000000 ataskq-5.0.0/ataskq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 20:31:31.000000 ataskq-5.0.0/ataskq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 20:31:31.000000 ataskq-5.0.0/ataskq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-17 20:31:20.000000 ataskq-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 20:31:31.907540 ataskq-5.0.0/setup.cfg
```

### Comparing `ataskq-0.4.1/LICENSE` & `ataskq-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ataskq-0.4.1/ataskq/logger.py` & `ataskq-5.0.0/ataskq/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 
+
 class Logger:
     def __init__(self, logger: logging.Logger or None):
-        self._logger = logger or logging.getLogger('ataskq')
-    
+        self._logger = logger or logging.getLogger("ataskq")
+
     def exception(self, *args, **kwargs):
         self._logger.exception(*args, **kwargs)
 
     def critical(self, *args, **kwargs):
         self._logger.critical(*args, **kwargs)
 
     def error(self, *args, **kwargs):
@@ -16,8 +17,8 @@
     def warning(self, *args, **kwargs):
         self._logger.warning(*args, **kwargs)
 
     def info(self, *args, **kwargs):
         self._logger.info(*args, **kwargs)
 
     def debug(self, *args, **kwargs):
-        self._logger.debug(*args, **kwargs)
+        self._logger.debug(*args, **kwargs)
```

### Comparing `ataskq-0.4.1/ataskq/monitor.py` & `ataskq-5.0.0/ataskq/monitor.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import socket
 from threading import Thread, Event
 import time
 
-from .task import Task, EStatus
+from .models import Task, EStatus
 
 
 class MonitorThread(Thread):
     # task runner is .task_runner TaskRunner, avoiding circular import
-    def __init__(self, task: Task, task_runner, pulse_interval: float = 60) -> None:
+    def __init__(self, task: Task, ataskq, pulse_interval: float = 60) -> None:
         super().__init__(daemon=True)
         self._stop_event = Event()
         self._task = task
-        self._task_runner = task_runner
+        self._ataskq = ataskq
         self._pulse_interval = pulse_interval
 
     def run(self) -> None:
-        self._task_runner.info(f"Running monitor thread for task id '{self._task.tid}'")
+        self._ataskq.info(f"Running monitor thread for task id '{self._task.task_id}'")
         while not self._stop_event.is_set():
-            self._task_runner.update_task_status(self._task, EStatus.RUNNING)
+            self._ataskq.update_task_status(self._task, EStatus.RUNNING)
             self._stop_event.wait(self._pulse_interval)
 
     def stop(self):
         self._stop_event.set()
-
```

