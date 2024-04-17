# Comparing `tmp/autocron-1.0.tar.gz` & `tmp/autocron-1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autocron-1.0.tar", last modified: Wed Apr 17 11:54:58 2024, max compression
+gzip compressed data, was "autocron-1.0rc1.tar", last modified: Mon Apr 15 15:14:44 2024, max compression
```

## Comparing `autocron-1.0.tar` & `autocron-1.0rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 klaus      (501) staff       (20)        0 2024-04-17 11:54:58.147005 autocron-1.0/
--rw-r--r--   0 klaus      (501) staff       (20)     1085 2024-04-03 12:57:14.000000 autocron-1.0/LICENSE.txt
--rw-r--r--   0 klaus      (501) staff       (20)       61 2024-04-03 13:00:18.000000 autocron-1.0/MANIFEST.in
--rw-r--r--   0 klaus      (501) staff       (20)     3391 2024-04-17 11:54:58.146943 autocron-1.0/PKG-INFO
--rw-r--r--   0 klaus      (501) staff       (20)     2194 2024-04-17 11:53:24.000000 autocron-1.0/README.md
-drwxr-xr-x   0 klaus      (501) staff       (20)        0 2024-04-17 11:54:58.145220 autocron-1.0/autocron/
--rw-r--r--   0 klaus      (501) staff       (20)     1306 2024-04-17 11:53:24.000000 autocron-1.0/autocron/__init__.py
--rw-r--r--   0 klaus      (501) staff       (20)     6929 2024-04-03 09:47:15.000000 autocron-1.0/autocron/admin.py
--rw-r--r--   0 klaus      (501) staff       (20)     6916 2024-04-15 13:28:09.000000 autocron-1.0/autocron/decorators.py
--rw-r--r--   0 klaus      (501) staff       (20)     7594 2024-04-09 10:05:02.000000 autocron-1.0/autocron/engine.py
--rw-r--r--   0 klaus      (501) staff       (20)    10767 2024-02-14 08:16:16.000000 autocron-1.0/autocron/schedule.py
--rw-r--r--   0 klaus      (501) staff       (20)    33910 2024-04-15 13:28:09.000000 autocron-1.0/autocron/sqlite_interface.py
--rw-r--r--   0 klaus      (501) staff       (20)     6101 2024-04-03 09:33:49.000000 autocron-1.0/autocron/worker.py
-drwxr-xr-x   0 klaus      (501) staff       (20)        0 2024-04-17 11:54:58.146760 autocron-1.0/autocron.egg-info/
--rw-r--r--   0 klaus      (501) staff       (20)     3391 2024-04-17 11:54:58.000000 autocron-1.0/autocron.egg-info/PKG-INFO
--rw-r--r--   0 klaus      (501) staff       (20)      501 2024-04-17 11:54:58.000000 autocron-1.0/autocron.egg-info/SOURCES.txt
--rw-r--r--   0 klaus      (501) staff       (20)        1 2024-04-17 11:54:58.000000 autocron-1.0/autocron.egg-info/dependency_links.txt
--rw-r--r--   0 klaus      (501) staff       (20)       49 2024-04-17 11:54:58.000000 autocron-1.0/autocron.egg-info/entry_points.txt
--rw-r--r--   0 klaus      (501) staff       (20)        9 2024-04-17 11:54:58.000000 autocron-1.0/autocron.egg-info/top_level.txt
--rw-r--r--   0 klaus      (501) staff       (20)       81 2023-04-22 13:30:54.000000 autocron-1.0/pyproject.toml
--rw-r--r--   0 klaus      (501) staff       (20)     1269 2024-04-17 11:54:58.147261 autocron-1.0/setup.cfg
--rw-r--r--   0 klaus      (501) staff       (20)      135 2023-03-23 08:40:38.000000 autocron-1.0/setup.py
-drwxr-xr-x   0 klaus      (501) staff       (20)        0 2024-04-17 11:54:58.146599 autocron-1.0/tests/
--rw-r--r--   0 klaus      (501) staff       (20)     3349 2024-04-15 13:28:09.000000 autocron-1.0/tests/test_decorators.py
--rw-r--r--   0 klaus      (501) staff       (20)     2412 2024-04-03 09:07:51.000000 autocron-1.0/tests/test_engine.py
--rw-r--r--   0 klaus      (501) staff       (20)     7652 2024-02-14 08:16:16.000000 autocron-1.0/tests/test_schedule.py
--rw-r--r--   0 klaus      (501) staff       (20)    13980 2024-04-08 14:37:26.000000 autocron-1.0/tests/test_sqlite_interface.py
--rw-r--r--   0 klaus      (501) staff       (20)     1918 2024-04-08 14:37:26.000000 autocron-1.0/tests/test_worker.py
+drwxr-xr-x   0 klaus      (501) staff       (20)        0 2024-04-15 15:14:44.839508 autocron-1.0rc1/
+-rw-r--r--   0 klaus      (501) staff       (20)     1085 2024-04-03 12:57:14.000000 autocron-1.0rc1/LICENSE.txt
+-rw-r--r--   0 klaus      (501) staff       (20)       61 2024-04-03 13:00:18.000000 autocron-1.0rc1/MANIFEST.in
+-rw-r--r--   0 klaus      (501) staff       (20)     3393 2024-04-15 15:14:44.839449 autocron-1.0rc1/PKG-INFO
+-rw-r--r--   0 klaus      (501) staff       (20)     2193 2024-01-13 16:36:00.000000 autocron-1.0rc1/README.md
+drwxr-xr-x   0 klaus      (501) staff       (20)        0 2024-04-15 15:14:44.837252 autocron-1.0rc1/autocron/
+-rw-r--r--   0 klaus      (501) staff       (20)     1309 2024-04-15 15:00:07.000000 autocron-1.0rc1/autocron/__init__.py
+-rw-r--r--   0 klaus      (501) staff       (20)     6929 2024-04-03 09:47:15.000000 autocron-1.0rc1/autocron/admin.py
+-rw-r--r--   0 klaus      (501) staff       (20)     6916 2024-04-15 13:28:09.000000 autocron-1.0rc1/autocron/decorators.py
+-rw-r--r--   0 klaus      (501) staff       (20)     7594 2024-04-09 10:05:02.000000 autocron-1.0rc1/autocron/engine.py
+-rw-r--r--   0 klaus      (501) staff       (20)    10767 2024-02-14 08:16:16.000000 autocron-1.0rc1/autocron/schedule.py
+-rw-r--r--   0 klaus      (501) staff       (20)    33910 2024-04-15 13:28:09.000000 autocron-1.0rc1/autocron/sqlite_interface.py
+-rw-r--r--   0 klaus      (501) staff       (20)     6101 2024-04-03 09:33:49.000000 autocron-1.0rc1/autocron/worker.py
+drwxr-xr-x   0 klaus      (501) staff       (20)        0 2024-04-15 15:14:44.839259 autocron-1.0rc1/autocron.egg-info/
+-rw-r--r--   0 klaus      (501) staff       (20)     3393 2024-04-15 15:14:44.000000 autocron-1.0rc1/autocron.egg-info/PKG-INFO
+-rw-r--r--   0 klaus      (501) staff       (20)      501 2024-04-15 15:14:44.000000 autocron-1.0rc1/autocron.egg-info/SOURCES.txt
+-rw-r--r--   0 klaus      (501) staff       (20)        1 2024-04-15 15:14:44.000000 autocron-1.0rc1/autocron.egg-info/dependency_links.txt
+-rw-r--r--   0 klaus      (501) staff       (20)       49 2024-04-15 15:14:44.000000 autocron-1.0rc1/autocron.egg-info/entry_points.txt
+-rw-r--r--   0 klaus      (501) staff       (20)        9 2024-04-15 15:14:44.000000 autocron-1.0rc1/autocron.egg-info/top_level.txt
+-rw-r--r--   0 klaus      (501) staff       (20)       81 2023-04-22 13:30:54.000000 autocron-1.0rc1/pyproject.toml
+-rw-r--r--   0 klaus      (501) staff       (20)     1269 2024-04-15 15:14:44.839748 autocron-1.0rc1/setup.cfg
+-rw-r--r--   0 klaus      (501) staff       (20)      135 2023-03-23 08:40:38.000000 autocron-1.0rc1/setup.py
+drwxr-xr-x   0 klaus      (501) staff       (20)        0 2024-04-15 15:14:44.838993 autocron-1.0rc1/tests/
+-rw-r--r--   0 klaus      (501) staff       (20)     3349 2024-04-15 13:28:09.000000 autocron-1.0rc1/tests/test_decorators.py
+-rw-r--r--   0 klaus      (501) staff       (20)     2412 2024-04-03 09:07:51.000000 autocron-1.0rc1/tests/test_engine.py
+-rw-r--r--   0 klaus      (501) staff       (20)     7652 2024-02-14 08:16:16.000000 autocron-1.0rc1/tests/test_schedule.py
+-rw-r--r--   0 klaus      (501) staff       (20)    13980 2024-04-08 14:37:26.000000 autocron-1.0rc1/tests/test_sqlite_interface.py
+-rw-r--r--   0 klaus      (501) staff       (20)     1918 2024-04-08 14:37:26.000000 autocron-1.0rc1/tests/test_worker.py
```

### Comparing `autocron-1.0/LICENSE.txt` & `autocron-1.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autocron-1.0/PKG-INFO` & `autocron-1.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autocron
-Version: 1.0
+Version: 1.0rc1
 Summary: Asynchronous background tasks for Python web-frameworks with no dependencies
 Home-page: https://github.com/kbr/autocron
 Author: Klaus Bremer
 Author-email: bremer@bremer-media.com
 License: MIT
 Project-URL: Homepage, https://github.com/kbr/autocron
 Project-URL: Code, https://github.com/kbr/autocron
@@ -48,15 +48,15 @@
     $ pip install autocron
 ```
 
 ## Quickstart
 
 autocron provides two decorators: ``cron`` that takes a string in [cron](https://en.wikipedia.org/wiki/Cron#CRON_expression)-format as argument, but accepts also keyword-arguments like *minutes* and *hours*. And ``delay`` to delegate a long running task to a background process.
 
-Here is a simple example how to use autocron with the flask web-framework that can be run with ``$ flask --app application run``:
+Here is a simple example how to use autocron with the flask web-framework that can be run with ``$ flak --app application run``:
 
 ```
     # application.py
 
     import autocron
     from flask import Flask
```

### Comparing `autocron-1.0/README.md` & `autocron-1.0rc1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     $ pip install autocron
 ```
 
 ## Quickstart
 
 autocron provides two decorators: ``cron`` that takes a string in [cron](https://en.wikipedia.org/wiki/Cron#CRON_expression)-format as argument, but accepts also keyword-arguments like *minutes* and *hours*. And ``delay`` to delegate a long running task to a background process.
 
-Here is a simple example how to use autocron with the flask web-framework that can be run with ``$ flask --app application run``:
+Here is a simple example how to use autocron with the flask web-framework that can be run with ``$ flak --app application run``:
 
 ```
     # application.py
 
     import autocron
     from flask import Flask
```

### Comparing `autocron-1.0/autocron/__init__.py` & `autocron-1.0rc1/autocron/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     delay,
 )
 from autocron.engine import Engine
 from autocron.sqlite_interface import SQLiteInterface
 
 
 __all__ = ["cron", "delay", "start", "stop"]
-__version__ = "1.0"
+__version__ = "1.0rc1"
 
 _engine = Engine()
 _interface = SQLiteInterface()
 
 
 def start(database_file, workers=None):
     """
```

### Comparing `autocron-1.0/autocron/admin.py` & `autocron-1.0rc1/autocron/admin.py`

 * *Files identical despite different names*

### Comparing `autocron-1.0/autocron/decorators.py` & `autocron-1.0rc1/autocron/decorators.py`

 * *Files identical despite different names*

### Comparing `autocron-1.0/autocron/engine.py` & `autocron-1.0rc1/autocron/engine.py`

 * *Files identical despite different names*

### Comparing `autocron-1.0/autocron/schedule.py` & `autocron-1.0rc1/autocron/schedule.py`

 * *Files identical despite different names*

### Comparing `autocron-1.0/autocron/sqlite_interface.py` & `autocron-1.0rc1/autocron/sqlite_interface.py`

 * *Files identical despite different names*

### Comparing `autocron-1.0/autocron/worker.py` & `autocron-1.0rc1/autocron/worker.py`

 * *Files identical despite different names*

### Comparing `autocron-1.0/autocron.egg-info/PKG-INFO` & `autocron-1.0rc1/autocron.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autocron
-Version: 1.0
+Version: 1.0rc1
 Summary: Asynchronous background tasks for Python web-frameworks with no dependencies
 Home-page: https://github.com/kbr/autocron
 Author: Klaus Bremer
 Author-email: bremer@bremer-media.com
 License: MIT
 Project-URL: Homepage, https://github.com/kbr/autocron
 Project-URL: Code, https://github.com/kbr/autocron
@@ -48,15 +48,15 @@
     $ pip install autocron
 ```
 
 ## Quickstart
 
 autocron provides two decorators: ``cron`` that takes a string in [cron](https://en.wikipedia.org/wiki/Cron#CRON_expression)-format as argument, but accepts also keyword-arguments like *minutes* and *hours*. And ``delay`` to delegate a long running task to a background process.
 
-Here is a simple example how to use autocron with the flask web-framework that can be run with ``$ flask --app application run``:
+Here is a simple example how to use autocron with the flask web-framework that can be run with ``$ flak --app application run``:
 
 ```
     # application.py
 
     import autocron
     from flask import Flask
```

### Comparing `autocron-1.0/setup.cfg` & `autocron-1.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `autocron-1.0/tests/test_decorators.py` & `autocron-1.0rc1/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `autocron-1.0/tests/test_engine.py` & `autocron-1.0rc1/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `autocron-1.0/tests/test_schedule.py` & `autocron-1.0rc1/tests/test_schedule.py`

 * *Files identical despite different names*

### Comparing `autocron-1.0/tests/test_sqlite_interface.py` & `autocron-1.0rc1/tests/test_sqlite_interface.py`

 * *Files identical despite different names*

### Comparing `autocron-1.0/tests/test_worker.py` & `autocron-1.0rc1/tests/test_worker.py`

 * *Files identical despite different names*

