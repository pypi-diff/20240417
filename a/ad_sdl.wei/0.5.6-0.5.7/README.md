# Comparing `tmp/ad_sdl.wei-0.5.6.tar.gz` & `tmp/ad_sdl_wei-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ad_sdl.wei-0.5.6.tar", last modified: Fri Mar 22 17:32:00 2024, max compression
+gzip compressed data, was "ad_sdl_wei-0.5.7.tar", last modified: Wed Apr 17 20:08:20 2024, max compression
```

## Comparing `ad_sdl.wei-0.5.6.tar` & `ad_sdl_wei-0.5.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:32:00.214098 ad_sdl.wei-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-03-22 17:32:00.214098 ad_sdl.wei-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:32:00.214098 ad_sdl.wei-0.5.6/ad_sdl.wei.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-03-22 17:32:00.000000 ad_sdl.wei-0.5.6/ad_sdl.wei.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-03-22 17:32:00.000000 ad_sdl.wei-0.5.6/ad_sdl.wei.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 17:32:00.000000 ad_sdl.wei-0.5.6/ad_sdl.wei.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-22 17:32:00.000000 ad_sdl.wei-0.5.6/ad_sdl.wei.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-22 17:32:00.000000 ad_sdl.wei-0.5.6/ad_sdl.wei.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 17:32:00.214098 ad_sdl.wei-0.5.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:32:00.210098 ad_sdl.wei-0.5.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/tests/test_wei_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/tests/test_workcell.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/tests/test_workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:32:00.210098 ad_sdl.wei-0.5.6/wei/
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:32:00.210098 ad_sdl.wei-0.5.6/wei/core/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/core/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    17278 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/core/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11112 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/core/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/core/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/core/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:32:00.210098 ad_sdl.wei-0.5.6/wei/core/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/core/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/core/interfaces/rest_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/core/interfaces/ros2_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/core/interfaces/simulate_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/core/interfaces/tcp_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/core/interfaces/zmq_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/core/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/core/loggers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/core/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/core/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8547 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/core/state_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/core/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/core/workcell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/core/workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    12557 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/experiment_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:32:00.214098 ad_sdl.wei-0.5.6/wei/routers/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/routers/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/routers/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/routers/experiments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/routers/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/routers/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/routers/workcells.py
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/routers/workflow_runs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-03-22 17:31:21.000000 ad_sdl.wei-0.5.6/wei/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:08:20.085303 ad_sdl_wei-0.5.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-17 20:08:20.085303 ad_sdl_wei-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:08:20.081303 ad_sdl_wei-0.5.7/ad_sdl.wei.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-04-17 20:08:20.000000 ad_sdl_wei-0.5.7/ad_sdl.wei.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-17 20:08:20.000000 ad_sdl_wei-0.5.7/ad_sdl.wei.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 20:08:20.000000 ad_sdl_wei-0.5.7/ad_sdl.wei.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-17 20:08:20.000000 ad_sdl_wei-0.5.7/ad_sdl.wei.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-17 20:08:20.000000 ad_sdl_wei-0.5.7/ad_sdl.wei.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 20:08:20.085303 ad_sdl_wei-0.5.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:08:20.073303 ad_sdl_wei-0.5.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/tests/test_wei_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/tests/test_workcell.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/tests/test_workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:08:20.077303 ad_sdl_wei-0.5.7/wei/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:08:20.077303 ad_sdl_wei-0.5.7/wei/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17284 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11112 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:08:20.081303 ad_sdl_wei-0.5.7/wei/core/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/interfaces/rest_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/interfaces/ros2_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/interfaces/simulate_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/interfaces/tcp_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/interfaces/zmq_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8547 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/state_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/workcell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/core/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12557 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/experiment_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:08:20.081303 ad_sdl_wei-0.5.7/wei/routers/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/routers/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/routers/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/routers/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/routers/locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/routers/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/routers/workcells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/routers/workflow_runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-17 20:07:39.000000 ad_sdl_wei-0.5.7/wei/server.py
```

### Comparing `ad_sdl.wei-0.5.6/LICENSE` & `ad_sdl_wei-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/PKG-INFO` & `ad_sdl_wei-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ad_sdl.wei
-Version: 0.5.6
+Version: 0.5.7
 Summary: The Rapid Prototyping Laboratory's Workflow Execution Interface.
 Author-email: Rafael Vescovi <ravescovi@anl.gov>, Tobias Ginsburg <tginsburg@anl.gov>, "Ryan D. Lewis" <ryan.lewis@anl.gov>, Casey Stone <cstone@anl.gov>, Doga Ozgulbas <dozgulbas@anl.gov>, Kyle Hippe <khippe@anl.gov>
 License: MIT
 Project-URL: Homepage, https://github.com/AD-SDL/wei
 Project-URL: Downloads, https://github.com/AD-SDL/wei/archive/refs/tags/0.5.1.tar.gz
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
```

### Comparing `ad_sdl.wei-0.5.6/README.md` & `ad_sdl_wei-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/ad_sdl.wei.egg-info/PKG-INFO` & `ad_sdl_wei-0.5.7/ad_sdl.wei.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ad_sdl.wei
-Version: 0.5.6
+Version: 0.5.7
 Summary: The Rapid Prototyping Laboratory's Workflow Execution Interface.
 Author-email: Rafael Vescovi <ravescovi@anl.gov>, Tobias Ginsburg <tginsburg@anl.gov>, "Ryan D. Lewis" <ryan.lewis@anl.gov>, Casey Stone <cstone@anl.gov>, Doga Ozgulbas <dozgulbas@anl.gov>, Kyle Hippe <khippe@anl.gov>
 License: MIT
 Project-URL: Homepage, https://github.com/AD-SDL/wei
 Project-URL: Downloads, https://github.com/AD-SDL/wei/archive/refs/tags/0.5.1.tar.gz
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
```

### Comparing `ad_sdl.wei-0.5.6/ad_sdl.wei.egg-info/SOURCES.txt` & `ad_sdl_wei-0.5.7/ad_sdl.wei.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/pyproject.toml` & `ad_sdl_wei-0.5.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ad_sdl.wei"
-version = "0.5.6"
+version = "0.5.7"
 description = "The Rapid Prototyping Laboratory's Workflow Execution Interface."
 authors = [
     {name = "Rafael Vescovi", email = "ravescovi@anl.gov"},
     {name = "Tobias Ginsburg", email = "tginsburg@anl.gov"},
     {name = "Ryan D. Lewis", email = "ryan.lewis@anl.gov"},
     {name = "Casey Stone", email = "cstone@anl.gov"},
     {name = "Doga Ozgulbas", email = "dozgulbas@anl.gov"},
```

### Comparing `ad_sdl.wei-0.5.6/tests/test_base.py` & `ad_sdl_wei-0.5.7/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/tests/test_wei_locations.py` & `ad_sdl_wei-0.5.7/tests/test_wei_locations.py`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/tests/test_workcell.py` & `ad_sdl_wei-0.5.7/tests/test_workcell.py`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/tests/test_workflows.py` & `ad_sdl_wei-0.5.7/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/wei/core/admin.py` & `ad_sdl_wei-0.5.7/wei/core/admin.py`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/wei/core/data_classes.py` & `ad_sdl_wei-0.5.7/wei/core/data_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -463,15 +463,15 @@
 
 
 class Workflow(BaseModel):
     """Grand container that pulls all info of a workflow together"""
 
     name: str
     """Name of the workflow"""
-    modules: List[str | SimpleModule]
+    modules: List[Union[str, SimpleModule]]
     """List of modules needed for the workflow"""
     flowdef: List[Step]
     """User Submitted Steps of the flow"""
     metadata: Metadata = Field(default_factory=Metadata)
     """Information about the flow"""
 
     @field_validator("modules", mode="after")
```

### Comparing `ad_sdl.wei-0.5.6/wei/core/events.py` & `ad_sdl_wei-0.5.7/wei/core/events.py`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/wei/core/experiment.py` & `ad_sdl_wei-0.5.7/wei/core/experiment.py`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/wei/core/interface.py` & `ad_sdl_wei-0.5.7/wei/core/interface.py`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/wei/core/interfaces/rest_interface.py` & `ad_sdl_wei-0.5.7/wei/core/interfaces/rest_interface.py`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/wei/core/interfaces/ros2_interface.py` & `ad_sdl_wei-0.5.7/wei/core/interfaces/ros2_interface.py`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/wei/core/interfaces/simulate_interface.py` & `ad_sdl_wei-0.5.7/wei/core/interfaces/simulate_interface.py`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/wei/core/interfaces/tcp_interface.py` & `ad_sdl_wei-0.5.7/wei/core/interfaces/tcp_interface.py`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/wei/core/interfaces/zmq_interface.py` & `ad_sdl_wei-0.5.7/wei/core/interfaces/zmq_interface.py`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/wei/core/location.py` & `ad_sdl_wei-0.5.7/wei/core/location.py`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/wei/core/loggers.py` & `ad_sdl_wei-0.5.7/wei/core/loggers.py`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/wei/core/module.py` & `ad_sdl_wei-0.5.7/wei/core/module.py`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/wei/core/scheduler.py` & `ad_sdl_wei-0.5.7/wei/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/wei/core/state_manager.py` & `ad_sdl_wei-0.5.7/wei/core/state_manager.py`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/wei/core/step.py` & `ad_sdl_wei-0.5.7/wei/core/step.py`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/wei/core/workcell.py` & `ad_sdl_wei-0.5.7/wei/core/workcell.py`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/wei/core/workflow.py` & `ad_sdl_wei-0.5.7/wei/core/workflow.py`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/wei/engine.py` & `ad_sdl_wei-0.5.7/wei/engine.py`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/wei/experiment_client.py` & `ad_sdl_wei-0.5.7/wei/experiment_client.py`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/wei/helpers.py` & `ad_sdl_wei-0.5.7/wei/helpers.py`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/wei/routers/admin.py` & `ad_sdl_wei-0.5.7/wei/routers/admin.py`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/wei/routers/experiments.py` & `ad_sdl_wei-0.5.7/wei/routers/experiments.py`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/wei/routers/locations.py` & `ad_sdl_wei-0.5.7/wei/routers/locations.py`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/wei/routers/modules.py` & `ad_sdl_wei-0.5.7/wei/routers/modules.py`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/wei/routers/workcells.py` & `ad_sdl_wei-0.5.7/wei/routers/workcells.py`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/wei/routers/workflow_runs.py` & `ad_sdl_wei-0.5.7/wei/routers/workflow_runs.py`

 * *Files identical despite different names*

### Comparing `ad_sdl.wei-0.5.6/wei/server.py` & `ad_sdl_wei-0.5.7/wei/server.py`

 * *Files identical despite different names*

