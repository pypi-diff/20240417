# Comparing `tmp/open_fleet-0.0.1.tar.gz` & `tmp/open_fleet-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_fleet-0.0.1.tar", last modified: Wed Apr 17 12:55:19 2024, max compression
+gzip compressed data, was "open_fleet-0.0.2.tar", last modified: Wed Apr 17 12:56:32 2024, max compression
```

## Comparing `open_fleet-0.0.1.tar` & `open_fleet-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-04-17 12:55:19.903403 open_fleet-0.0.1/
--rw-r--r--   0 huangshiyu   (501) staff       (20)    11357 2024-04-17 07:28:40.000000 open_fleet-0.0.1/LICENSE
--rw-r--r--   0 huangshiyu   (501) staff       (20)     1826 2024-04-17 12:55:19.903181 open_fleet-0.0.1/PKG-INFO
--rw-r--r--   0 huangshiyu   (501) staff       (20)      504 2024-04-17 12:54:08.000000 open_fleet-0.0.1/README.md
-drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-04-17 12:55:19.899963 open_fleet-0.0.1/fleet/
--rw-r--r--   0 huangshiyu   (501) staff       (20)      457 2024-04-17 07:36:34.000000 open_fleet-0.0.1/fleet/__init__.py
-drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-04-17 12:55:19.900431 open_fleet-0.0.1/fleet/config/
--rw-r--r--   0 huangshiyu   (501) staff       (20)        0 2024-04-17 08:43:11.000000 open_fleet-0.0.1/fleet/config/__init__.py
--rw-r--r--   0 huangshiyu   (501) staff       (20)      653 2024-04-16 11:50:22.000000 open_fleet-0.0.1/fleet/config/config.py
--rw-r--r--   0 huangshiyu   (501) staff       (20)     9602 2024-04-17 10:49:17.000000 open_fleet-0.0.1/fleet/manager.py
-drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-04-17 12:55:19.901450 open_fleet-0.0.1/fleet/utils/
--rw-r--r--   0 huangshiyu   (501) staff       (20)        0 2024-04-17 08:43:03.000000 open_fleet-0.0.1/fleet/utils/__init__.py
--rw-r--r--   0 huangshiyu   (501) staff       (20)      496 2024-04-17 07:18:40.000000 open_fleet-0.0.1/fleet/utils/file_utils.py
--rw-r--r--   0 huangshiyu   (501) staff       (20)      573 2024-04-16 07:33:32.000000 open_fleet-0.0.1/fleet/utils/host_utils.py
--rw-r--r--   0 huangshiyu   (501) staff       (20)     2143 2024-04-17 10:43:53.000000 open_fleet-0.0.1/fleet/utils/time_tracker.py
--rw-r--r--   0 huangshiyu   (501) staff       (20)     5543 2024-04-17 09:52:18.000000 open_fleet-0.0.1/fleet/worker.py
-drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-04-17 12:55:19.902532 open_fleet-0.0.1/open_fleet.egg-info/
--rw-r--r--   0 huangshiyu   (501) staff       (20)     1826 2024-04-17 12:55:19.000000 open_fleet-0.0.1/open_fleet.egg-info/PKG-INFO
--rw-r--r--   0 huangshiyu   (501) staff       (20)      398 2024-04-17 12:55:19.000000 open_fleet-0.0.1/open_fleet.egg-info/SOURCES.txt
--rw-r--r--   0 huangshiyu   (501) staff       (20)        1 2024-04-17 12:55:19.000000 open_fleet-0.0.1/open_fleet.egg-info/dependency_links.txt
--rw-r--r--   0 huangshiyu   (501) staff       (20)       94 2024-04-17 12:55:19.000000 open_fleet-0.0.1/open_fleet.egg-info/requires.txt
--rw-r--r--   0 huangshiyu   (501) staff       (20)        6 2024-04-17 12:55:19.000000 open_fleet-0.0.1/open_fleet.egg-info/top_level.txt
--rw-r--r--   0 huangshiyu   (501) staff       (20)       38 2024-04-17 12:55:19.903455 open_fleet-0.0.1/setup.cfg
--rw-r--r--   0 huangshiyu   (501) staff       (20)     2456 2024-04-17 12:55:11.000000 open_fleet-0.0.1/setup.py
+drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-04-17 12:56:32.484314 open_fleet-0.0.2/
+-rw-r--r--   0 huangshiyu   (501) staff       (20)    11357 2024-04-17 07:28:40.000000 open_fleet-0.0.2/LICENSE
+-rw-r--r--   0 huangshiyu   (501) staff       (20)     1828 2024-04-17 12:56:32.484110 open_fleet-0.0.2/PKG-INFO
+-rw-r--r--   0 huangshiyu   (501) staff       (20)      506 2024-04-17 12:56:16.000000 open_fleet-0.0.2/README.md
+drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-04-17 12:56:32.480780 open_fleet-0.0.2/fleet/
+-rw-r--r--   0 huangshiyu   (501) staff       (20)      457 2024-04-17 12:56:27.000000 open_fleet-0.0.2/fleet/__init__.py
+drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-04-17 12:56:32.481358 open_fleet-0.0.2/fleet/config/
+-rw-r--r--   0 huangshiyu   (501) staff       (20)        0 2024-04-17 08:43:11.000000 open_fleet-0.0.2/fleet/config/__init__.py
+-rw-r--r--   0 huangshiyu   (501) staff       (20)      653 2024-04-16 11:50:22.000000 open_fleet-0.0.2/fleet/config/config.py
+-rw-r--r--   0 huangshiyu   (501) staff       (20)     9602 2024-04-17 10:49:17.000000 open_fleet-0.0.2/fleet/manager.py
+drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-04-17 12:56:32.482459 open_fleet-0.0.2/fleet/utils/
+-rw-r--r--   0 huangshiyu   (501) staff       (20)        0 2024-04-17 08:43:03.000000 open_fleet-0.0.2/fleet/utils/__init__.py
+-rw-r--r--   0 huangshiyu   (501) staff       (20)      496 2024-04-17 07:18:40.000000 open_fleet-0.0.2/fleet/utils/file_utils.py
+-rw-r--r--   0 huangshiyu   (501) staff       (20)      573 2024-04-16 07:33:32.000000 open_fleet-0.0.2/fleet/utils/host_utils.py
+-rw-r--r--   0 huangshiyu   (501) staff       (20)     2143 2024-04-17 10:43:53.000000 open_fleet-0.0.2/fleet/utils/time_tracker.py
+-rw-r--r--   0 huangshiyu   (501) staff       (20)     5543 2024-04-17 09:52:18.000000 open_fleet-0.0.2/fleet/worker.py
+drwxr-xr-x   0 huangshiyu   (501) staff       (20)        0 2024-04-17 12:56:32.483519 open_fleet-0.0.2/open_fleet.egg-info/
+-rw-r--r--   0 huangshiyu   (501) staff       (20)     1828 2024-04-17 12:56:32.000000 open_fleet-0.0.2/open_fleet.egg-info/PKG-INFO
+-rw-r--r--   0 huangshiyu   (501) staff       (20)      398 2024-04-17 12:56:32.000000 open_fleet-0.0.2/open_fleet.egg-info/SOURCES.txt
+-rw-r--r--   0 huangshiyu   (501) staff       (20)        1 2024-04-17 12:56:32.000000 open_fleet-0.0.2/open_fleet.egg-info/dependency_links.txt
+-rw-r--r--   0 huangshiyu   (501) staff       (20)       94 2024-04-17 12:56:32.000000 open_fleet-0.0.2/open_fleet.egg-info/requires.txt
+-rw-r--r--   0 huangshiyu   (501) staff       (20)        6 2024-04-17 12:56:32.000000 open_fleet-0.0.2/open_fleet.egg-info/top_level.txt
+-rw-r--r--   0 huangshiyu   (501) staff       (20)       38 2024-04-17 12:56:32.484357 open_fleet-0.0.2/setup.cfg
+-rw-r--r--   0 huangshiyu   (501) staff       (20)     2456 2024-04-17 12:55:11.000000 open_fleet-0.0.2/setup.py
```

### Comparing `open_fleet-0.0.1/LICENSE` & `open_fleet-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `open_fleet-0.0.1/PKG-INFO` & `open_fleet-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-fleet
-Version: 0.0.1
+Version: 0.0.2
 Summary: distributed task distribution framework
 Author: Shiyu Huang
 Author-email: huangsy1314@163.com
 Project-URL: Documentation, https://github.com/huangshiyu13/Fleet
 Keywords: distributed framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -36,9 +36,9 @@
 # Fleet
 
 Fleet is a generic distributed task distribution framework based on a distributed file system. Task distribution frameworks like Ray and Celery require network connections for communication, which makes them difficult to use in clusters with poor network conditions. Fleet is a distributed framework based on a shared file system, independent of any network communication, allowing for task distribution among nodes without any network connections.
 
 ## Install
 
 ```bash
-pip install Fleet-py
+pip install open-fleet
 ```
```

### Comparing `open_fleet-0.0.1/fleet/config/config.py` & `open_fleet-0.0.2/fleet/config/config.py`

 * *Files identical despite different names*

### Comparing `open_fleet-0.0.1/fleet/manager.py` & `open_fleet-0.0.2/fleet/manager.py`

 * *Files identical despite different names*

### Comparing `open_fleet-0.0.1/fleet/utils/host_utils.py` & `open_fleet-0.0.2/fleet/utils/host_utils.py`

 * *Files identical despite different names*

### Comparing `open_fleet-0.0.1/fleet/utils/time_tracker.py` & `open_fleet-0.0.2/fleet/utils/time_tracker.py`

 * *Files identical despite different names*

### Comparing `open_fleet-0.0.1/fleet/worker.py` & `open_fleet-0.0.2/fleet/worker.py`

 * *Files identical despite different names*

### Comparing `open_fleet-0.0.1/open_fleet.egg-info/PKG-INFO` & `open_fleet-0.0.2/open_fleet.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-fleet
-Version: 0.0.1
+Version: 0.0.2
 Summary: distributed task distribution framework
 Author: Shiyu Huang
 Author-email: huangsy1314@163.com
 Project-URL: Documentation, https://github.com/huangshiyu13/Fleet
 Keywords: distributed framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -36,9 +36,9 @@
 # Fleet
 
 Fleet is a generic distributed task distribution framework based on a distributed file system. Task distribution frameworks like Ray and Celery require network connections for communication, which makes them difficult to use in clusters with poor network conditions. Fleet is a distributed framework based on a shared file system, independent of any network communication, allowing for task distribution among nodes without any network connections.
 
 ## Install
 
 ```bash
-pip install Fleet-py
+pip install open-fleet
 ```
```

### Comparing `open_fleet-0.0.1/setup.py` & `open_fleet-0.0.2/setup.py`

 * *Files identical despite different names*

