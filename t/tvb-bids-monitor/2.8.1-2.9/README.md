# Comparing `tmp/tvb-bids-monitor-2.8.1.tar.gz` & `tmp/tvb-bids-monitor-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvb-bids-monitor-2.8.1.tar", last modified: Tue May 23 12:09:36 2023, max compression
+gzip compressed data, was "tvb-bids-monitor-2.9.tar", last modified: Fri Apr 12 19:21:45 2024, max compression
```

## Comparing `tvb-bids-monitor-2.8.1.tar` & `tvb-bids-monitor-2.9.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:36.683415 tvb-bids-monitor-2.8.1/
--rw-r--r--   0 root         (0) root         (0)     1759 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/AUTHORS
--rw-r--r--   0 root         (0) root         (0)    36777 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      403 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/MANIFEST_bids_monitor.in
--rw-r--r--   0 root         (0) root         (0)     4158 2023-05-23 12:09:36.683415 tvb-bids-monitor-2.8.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4235 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/README.rst
--rw-r--r--   0 root         (0) root         (0)     3656 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/README_bids_monitor.rst
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 12:09:36.683415 tvb-bids-monitor-2.8.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2989 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:36.671414 tvb-bids-monitor-2.8.1/tvb/
--rw-r--r--   0 root         (0) root         (0)     1537 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:36.672414 tvb-bids-monitor-2.8.1/tvb/config/
--rw-r--r--   0 root         (0) root         (0)     2391 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2566 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/algorithm_categories.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:36.674414 tvb-bids-monitor-2.8.1/tvb/config/init/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/init/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:36.674414 tvb-bids-monitor-2.8.1/tvb/config/init/alembic/
--rw-r--r--   0 root         (0) root         (0)     2238 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/init/alembic/env.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:36.676414 tvb-bids-monitor-2.8.1/tvb/config/init/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     2466 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/init/alembic/versions/32d4bf9f8cab_update_db_002.py
--rw-r--r--   0 root         (0) root         (0)     2262 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/init/alembic/versions/32d4bf9f8def_update_db_003.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/init/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12427 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/init/alembic/versions/ec2859bb9114_update_db_001.py
--rw-r--r--   0 root         (0) root         (0)     9934 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/init/datatypes_registry.py
--rw-r--r--   0 root         (0) root         (0)     9460 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/init/initializer.py
--rw-r--r--   0 root         (0) root         (0)     6604 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/init/introspector_registry.py
--rw-r--r--   0 root         (0) root         (0)     5505 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/init/model_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:36.677414 tvb-bids-monitor-2.8.1/tvb/config/logger/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/logger/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3176 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/logger/cluster_handler.py
--rw-r--r--   0 root         (0) root         (0)     3465 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/logger/dev_logger_config.conf
--rw-r--r--   0 root         (0) root         (0)     5445 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/logger/elasticsearch_handler.py
--rw-r--r--   0 root         (0) root         (0)     3130 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/logger/logger_config.conf
--rw-r--r--   0 root         (0) root         (0)     5820 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/config/profile_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:36.678414 tvb-bids-monitor-2.8.1/tvb/interfaces/
--rw-r--r--   0 root         (0) root         (0)     1374 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/interfaces/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:36.678414 tvb-bids-monitor-2.8.1/tvb/interfaces/rest/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/interfaces/rest/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:36.679414 tvb-bids-monitor-2.8.1/tvb/interfaces/rest/bids_monitor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/interfaces/rest/bids_monitor/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10489 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/interfaces/rest/bids_monitor/bids_data_builder.py
--rw-r--r--   0 root         (0) root         (0)     8764 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/interfaces/rest/bids_monitor/bids_dir_monitor.py
--rw-r--r--   0 root         (0) root         (0)     2335 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/interfaces/rest/bids_monitor/launch_bids_monitor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:36.680414 tvb-bids-monitor-2.8.1/tvb/interfaces/rest/bids_monitor/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/interfaces/rest/bids_monitor/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10056 2023-05-23 11:37:04.000000 tvb-bids-monitor-2.8.1/tvb/interfaces/rest/bids_monitor/tests/bids_monitor_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 12:09:36.682414 tvb-bids-monitor-2.8.1/tvb_bids_monitor.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4158 2023-05-23 12:09:36.000000 tvb-bids-monitor-2.8.1/tvb_bids_monitor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1390 2023-05-23 12:09:36.000000 tvb-bids-monitor-2.8.1/tvb_bids_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 12:09:36.000000 tvb-bids-monitor-2.8.1/tvb_bids_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-05-23 12:09:36.000000 tvb-bids-monitor-2.8.1/tvb_bids_monitor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-23 12:09:36.000000 tvb-bids-monitor-2.8.1/tvb_bids_monitor.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:45.297407 tvb-bids-monitor-2.9/
+-rw-r--r--   0 root         (0) root         (0)     1759 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)    36777 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      403 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/MANIFEST_bids_monitor.in
+-rw-r--r--   0 root         (0) root         (0)     4337 2024-04-12 19:21:45.297407 tvb-bids-monitor-2.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4206 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/README.rst
+-rw-r--r--   0 root         (0) root         (0)     3656 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/README_bids_monitor.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 19:21:45.297407 tvb-bids-monitor-2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3050 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:45.287407 tvb-bids-monitor-2.9/tvb/
+-rw-r--r--   0 root         (0) root         (0)     1537 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/tvb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:45.288407 tvb-bids-monitor-2.9/tvb/config/
+-rw-r--r--   0 root         (0) root         (0)     2391 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/tvb/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/tvb/config/algorithm_categories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:45.289407 tvb-bids-monitor-2.9/tvb/config/init/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/tvb/config/init/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:45.289407 tvb-bids-monitor-2.9/tvb/config/init/alembic/
+-rw-r--r--   0 root         (0) root         (0)     2238 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/tvb/config/init/alembic/env.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:45.291407 tvb-bids-monitor-2.9/tvb/config/init/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     2466 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/tvb/config/init/alembic/versions/32d4bf9f8cab_update_db_002.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/tvb/config/init/alembic/versions/32d4bf9f8def_update_db_003.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/tvb/config/init/alembic/versions/32d4bf9f8ghj_update_db_004.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/tvb/config/init/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12427 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/tvb/config/init/alembic/versions/ec2859bb9114_update_db_001.py
+-rw-r--r--   0 root         (0) root         (0)     9934 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/tvb/config/init/datatypes_registry.py
+-rw-r--r--   0 root         (0) root         (0)     9460 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/tvb/config/init/initializer.py
+-rw-r--r--   0 root         (0) root         (0)     6604 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/tvb/config/init/introspector_registry.py
+-rw-r--r--   0 root         (0) root         (0)     5505 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/tvb/config/init/model_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:45.293407 tvb-bids-monitor-2.9/tvb/config/logger/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/tvb/config/logger/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3176 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/tvb/config/logger/cluster_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3465 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/tvb/config/logger/dev_logger_config.conf
+-rw-r--r--   0 root         (0) root         (0)     5445 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/tvb/config/logger/elasticsearch_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3130 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/tvb/config/logger/logger_config.conf
+-rw-r--r--   0 root         (0) root         (0)     5820 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/tvb/config/profile_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:45.293407 tvb-bids-monitor-2.9/tvb/interfaces/
+-rw-r--r--   0 root         (0) root         (0)     1374 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/tvb/interfaces/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:45.293407 tvb-bids-monitor-2.9/tvb/interfaces/rest/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/tvb/interfaces/rest/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:45.294407 tvb-bids-monitor-2.9/tvb/interfaces/rest/bids_monitor/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/tvb/interfaces/rest/bids_monitor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10489 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/tvb/interfaces/rest/bids_monitor/bids_data_builder.py
+-rw-r--r--   0 root         (0) root         (0)     8764 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/tvb/interfaces/rest/bids_monitor/bids_dir_monitor.py
+-rw-r--r--   0 root         (0) root         (0)     2335 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/tvb/interfaces/rest/bids_monitor/launch_bids_monitor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:45.295407 tvb-bids-monitor-2.9/tvb/interfaces/rest/bids_monitor/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/tvb/interfaces/rest/bids_monitor/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10056 2024-04-12 19:06:40.000000 tvb-bids-monitor-2.9/tvb/interfaces/rest/bids_monitor/tests/bids_monitor_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 19:21:45.296408 tvb-bids-monitor-2.9/tvb_bids_monitor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4337 2024-04-12 19:21:44.000000 tvb-bids-monitor-2.9/tvb_bids_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1453 2024-04-12 19:21:45.000000 tvb-bids-monitor-2.9/tvb_bids_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 19:21:44.000000 tvb-bids-monitor-2.9/tvb_bids_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2024-04-12 19:21:44.000000 tvb-bids-monitor-2.9/tvb_bids_monitor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2024-04-12 19:21:44.000000 tvb-bids-monitor-2.9/tvb_bids_monitor.egg-info/top_level.txt
```

### Comparing `tvb-bids-monitor-2.8.1/AUTHORS` & `tvb-bids-monitor-2.9/AUTHORS`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.8.1/LICENSE` & `tvb-bids-monitor-2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.8.1/PKG-INFO` & `tvb-bids-monitor-2.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: tvb-bids-monitor
-Version: 2.8.1
+Version: 2.9
 Summary: A helper package containing BIDS directory monitor module
-Home-page: http://www.thevirtualbrain.org
+Home-page: https://www.thevirtualbrain.org
 Download-URL: https://github.com/the-virtual-brain/tvb-root
 Author: Akash Upadhyay, Paula Prodan
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: tvb rest client brain simulator neuroscience human animal neuronal dynamics models delay
-Provides-Extra: test
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
+Requires-Dist: tvb-rest-client
+Requires-Dist: watchdog
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-benchmark; extra == "test"
 
 BIDS data builder and directory monitor
 =======================================
 
 This module contains helper classes which can build BIDS datasets and import them into TVB projects. Along with this, the module also provides a way to monitor a BIDS directory and build datasets accordingly when new files are added.
 
 BIDSDataBuilder
```

### Comparing `tvb-bids-monitor-2.8.1/README.rst` & `tvb-bids-monitor-2.9/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                 |
                 |
             tvb.config.init
                 |
                 |
             tvb.interfaces
 
-**tvb-data** should be installed from **Zenodo**: https://zenodo.org/record/7574266/files/tvb_data.zip?download=1.
+**tvb-data** should be installed from **Zenodo**: https://zenodo.org/record/10128131.
 After download, unzip and execute `python setup.py develop` in the correct env.
 
 Usage
 -----
 
 To use TVB code, clone from GitHub (https://github.com/the-virtual-brain/tvb-root), or get from Pypi::
```

### Comparing `tvb-bids-monitor-2.8.1/README_bids_monitor.rst` & `tvb-bids-monitor-2.9/README_bids_monitor.rst`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.8.1/setup.py` & `tvb-bids-monitor-2.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,38 +32,39 @@
 import shutil
 
 import setuptools
 from setuptools.command.egg_info import manifest_maker
 
 manifest_maker.template = 'MANIFEST_bids_monitor.in'
 
-VERSION = "2.8.1"
+VERSION = "2.9"
 
 TVB_TEAM = "Akash Upadhyay, Paula Prodan"
 
 TVB_INSTALL_REQUIREMENTS = ["tvb-rest-client", "watchdog"]
 
 # Packaging bids-monitor
 with open(os.path.join(os.path.dirname(__file__), 'README_bids_monitor.rst')) as fd:
     DESCRIPTION = fd.read()
 
 setuptools.setup(name="tvb-bids-monitor",
                  version=VERSION,
                  packages=setuptools.find_packages(
                      exclude=['tvb.interfaces.web', 'tvb.interfaces.web.*', 'tvb.interfaces.command',
-                              'tvb.interfaces.command.*', 'tvb.tests', 'tvb.tests.*', 'tvb.interfaces.rest'
+                              'tvb.interfaces.command.*', 'tvb.tests', 'tvb.tests.*', 'tvb.interfaces.rest',
                               'tvb.interfaces.rest.*', 'tvb.adapters', 'tvb.adapters.*', 'tvb.core',
                               'tvb.core.*']),
                  include_package_data=True,
                  install_requires=TVB_INSTALL_REQUIREMENTS,
                  extras_require={'test': ["pytest", "pytest-benchmark"]},
                  description='A helper package containing BIDS directory monitor module',
                  long_description=DESCRIPTION,
+                 long_description_content_type="text/x-rst",
                  license="GPL-3.0-or-later",
                  author=TVB_TEAM,
                  author_email='tvb.admin@thevirtualbrain.org',
-                 url='http://www.thevirtualbrain.org',
+                 url='https://www.thevirtualbrain.org',
                  download_url='https://github.com/the-virtual-brain/tvb-root',
                  keywords='tvb rest client brain simulator neuroscience human animal neuronal dynamics models delay')
 
 # Clean after install
 shutil.rmtree('tvb_bids_monitor.egg-info', True)
```

### Comparing `tvb-bids-monitor-2.8.1/tvb/__init__.py` & `tvb-bids-monitor-2.9/tvb/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.8.1/tvb/config/__init__.py` & `tvb-bids-monitor-2.9/tvb/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.8.1/tvb/config/algorithm_categories.py` & `tvb-bids-monitor-2.9/tvb/config/algorithm_categories.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.8.1/tvb/config/init/alembic/env.py` & `tvb-bids-monitor-2.9/tvb/config/init/alembic/env.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.8.1/tvb/config/init/alembic/versions/32d4bf9f8cab_update_db_002.py` & `tvb-bids-monitor-2.9/tvb/config/init/alembic/versions/32d4bf9f8cab_update_db_002.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.8.1/tvb/config/init/alembic/versions/32d4bf9f8def_update_db_003.py` & `tvb-bids-monitor-2.9/tvb/config/init/alembic/versions/32d4bf9f8def_update_db_003.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.8.1/tvb/config/init/alembic/versions/ec2859bb9114_update_db_001.py` & `tvb-bids-monitor-2.9/tvb/config/init/alembic/versions/ec2859bb9114_update_db_001.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.8.1/tvb/config/init/datatypes_registry.py` & `tvb-bids-monitor-2.9/tvb/config/init/datatypes_registry.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.8.1/tvb/config/init/initializer.py` & `tvb-bids-monitor-2.9/tvb/config/init/initializer.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.8.1/tvb/config/init/introspector_registry.py` & `tvb-bids-monitor-2.9/tvb/config/init/introspector_registry.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.8.1/tvb/config/init/model_manager.py` & `tvb-bids-monitor-2.9/tvb/config/init/model_manager.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.8.1/tvb/config/logger/cluster_handler.py` & `tvb-bids-monitor-2.9/tvb/config/logger/cluster_handler.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.8.1/tvb/config/logger/dev_logger_config.conf` & `tvb-bids-monitor-2.9/tvb/config/logger/dev_logger_config.conf`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.8.1/tvb/config/logger/elasticsearch_handler.py` & `tvb-bids-monitor-2.9/tvb/config/logger/elasticsearch_handler.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.8.1/tvb/config/logger/logger_config.conf` & `tvb-bids-monitor-2.9/tvb/config/logger/logger_config.conf`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.8.1/tvb/config/profile_settings.py` & `tvb-bids-monitor-2.9/tvb/config/profile_settings.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.8.1/tvb/interfaces/__init__.py` & `tvb-bids-monitor-2.9/tvb/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.8.1/tvb/interfaces/rest/bids_monitor/bids_data_builder.py` & `tvb-bids-monitor-2.9/tvb/interfaces/rest/bids_monitor/bids_data_builder.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.8.1/tvb/interfaces/rest/bids_monitor/bids_dir_monitor.py` & `tvb-bids-monitor-2.9/tvb/interfaces/rest/bids_monitor/bids_dir_monitor.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.8.1/tvb/interfaces/rest/bids_monitor/launch_bids_monitor.py` & `tvb-bids-monitor-2.9/tvb/interfaces/rest/bids_monitor/launch_bids_monitor.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.8.1/tvb/interfaces/rest/bids_monitor/tests/bids_monitor_test.py` & `tvb-bids-monitor-2.9/tvb/interfaces/rest/bids_monitor/tests/bids_monitor_test.py`

 * *Files identical despite different names*

### Comparing `tvb-bids-monitor-2.8.1/tvb_bids_monitor.egg-info/PKG-INFO` & `tvb-bids-monitor-2.9/tvb_bids_monitor.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: tvb-bids-monitor
-Version: 2.8.1
+Version: 2.9
 Summary: A helper package containing BIDS directory monitor module
-Home-page: http://www.thevirtualbrain.org
+Home-page: https://www.thevirtualbrain.org
 Download-URL: https://github.com/the-virtual-brain/tvb-root
 Author: Akash Upadhyay, Paula Prodan
 Author-email: tvb.admin@thevirtualbrain.org
 License: GPL-3.0-or-later
 Keywords: tvb rest client brain simulator neuroscience human animal neuronal dynamics models delay
-Provides-Extra: test
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
+Requires-Dist: tvb-rest-client
+Requires-Dist: watchdog
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-benchmark; extra == "test"
 
 BIDS data builder and directory monitor
 =======================================
 
 This module contains helper classes which can build BIDS datasets and import them into TVB projects. Along with this, the module also provides a way to monitor a BIDS directory and build datasets accordingly when new files are added.
 
 BIDSDataBuilder
```

### Comparing `tvb-bids-monitor-2.8.1/tvb_bids_monitor.egg-info/SOURCES.txt` & `tvb-bids-monitor-2.9/tvb_bids_monitor.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 tvb/config/init/datatypes_registry.py
 tvb/config/init/initializer.py
 tvb/config/init/introspector_registry.py
 tvb/config/init/model_manager.py
 tvb/config/init/alembic/env.py
 tvb/config/init/alembic/versions/32d4bf9f8cab_update_db_002.py
 tvb/config/init/alembic/versions/32d4bf9f8def_update_db_003.py
+tvb/config/init/alembic/versions/32d4bf9f8ghj_update_db_004.py
 tvb/config/init/alembic/versions/__init__.py
 tvb/config/init/alembic/versions/ec2859bb9114_update_db_001.py
 tvb/config/logger/__init__.py
 tvb/config/logger/cluster_handler.py
 tvb/config/logger/dev_logger_config.conf
 tvb/config/logger/elasticsearch_handler.py
 tvb/config/logger/logger_config.conf
```

