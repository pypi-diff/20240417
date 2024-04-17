# Comparing `tmp/sciveo-0.0.50.tar.gz` & `tmp/sciveo-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciveo-0.0.50.tar", last modified: Wed Apr 17 12:00:18 2024, max compression
+gzip compressed data, was "sciveo-0.1.0.tar", last modified: Wed Apr 17 12:57:01 2024, max compression
```

## Comparing `sciveo-0.0.50.tar` & `sciveo-0.1.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:00:18.606768 sciveo-0.0.50/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     6208 2024-04-17 12:00:18.606605 sciveo-0.0.50/PKG-INFO
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     6055 2024-04-10 20:04:28.000000 sciveo-0.0.50/README.md
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:00:18.560520 sciveo-0.0.50/sciveo/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1428 2024-04-16 17:53:18.000000 sciveo-0.0.50/sciveo/__init__.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:00:18.570516 sciveo-0.0.50/sciveo/api/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:04:12.000000 sciveo-0.0.50/sciveo/api/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1788 2024-04-16 17:39:04.000000 sciveo-0.0.50/sciveo/api/base.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1815 2024-04-05 16:37:24.000000 sciveo-0.0.50/sciveo/api/upload.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:00:18.573936 sciveo-0.0.50/sciveo/common/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:03:59.000000 sciveo-0.0.50/sciveo/common/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2043 2024-03-14 17:02:24.000000 sciveo-0.0.50/sciveo/common/configuration.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1583 2024-03-14 17:02:24.000000 sciveo-0.0.50/sciveo/common/model.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3842 2024-04-07 18:52:23.000000 sciveo-0.0.50/sciveo/common/optimizers.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)    10567 2024-03-19 14:47:24.000000 sciveo-0.0.50/sciveo/common/sampling.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:00:18.588035 sciveo-0.0.50/sciveo/common/tools/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:07:07.000000 sciveo-0.0.50/sciveo/common/tools/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1647 2024-04-16 17:39:58.000000 sciveo-0.0.50/sciveo/common/tools/daemon.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1053 2023-11-17 12:42:35.000000 sciveo-0.0.50/sciveo/common/tools/formating.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1654 2024-04-14 08:49:26.000000 sciveo-0.0.50/sciveo/common/tools/hardware.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1071 2023-11-15 15:21:05.000000 sciveo-0.0.50/sciveo/common/tools/logger.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1333 2024-04-16 17:40:12.000000 sciveo-0.0.50/sciveo/common/tools/synchronized.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1087 2024-04-16 17:42:03.000000 sciveo-0.0.50/sciveo/common/tools/timers.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:00:18.592724 sciveo-0.0.50/sciveo/content/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:14:23.000000 sciveo-0.0.50/sciveo/content/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      827 2024-03-14 17:02:24.000000 sciveo-0.0.50/sciveo/content/dataset.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     5859 2024-04-07 18:52:23.000000 sciveo-0.0.50/sciveo/content/experiment.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3129 2024-04-07 18:52:23.000000 sciveo-0.0.50/sciveo/content/project.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2015 2024-03-19 14:47:07.000000 sciveo-0.0.50/sciveo/content/runner.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:00:18.602281 sciveo-0.0.50/sciveo/monitoring/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2024-04-07 18:52:23.000000 sciveo-0.0.50/sciveo/monitoring/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     5663 2024-04-17 11:58:08.000000 sciveo-0.0.50/sciveo/monitoring/monitor.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2564 2024-04-16 17:50:56.000000 sciveo-0.0.50/sciveo/monitoring/network.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1671 2024-04-16 17:41:11.000000 sciveo-0.0.50/sciveo/monitoring/start.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       24 2024-04-17 11:59:53.000000 sciveo-0.0.50/sciveo/version.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:00:18.569688 sciveo-0.0.50/sciveo.egg-info/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     6208 2024-04-17 12:00:18.000000 sciveo-0.0.50/sciveo.egg-info/PKG-INFO
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      965 2024-04-17 12:00:18.000000 sciveo-0.0.50/sciveo.egg-info/SOURCES.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        1 2024-04-17 12:00:18.000000 sciveo-0.0.50/sciveo.egg-info/dependency_links.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      112 2024-04-17 12:00:18.000000 sciveo-0.0.50/sciveo.egg-info/requires.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        7 2024-04-17 12:00:18.000000 sciveo-0.0.50/sciveo.egg-info/top_level.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       38 2024-04-17 12:00:18.606824 sciveo-0.0.50/setup.cfg
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      778 2024-04-16 17:42:22.000000 sciveo-0.0.50/setup.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:00:18.606147 sciveo-0.0.50/test/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      521 2024-03-14 17:02:24.000000 sciveo-0.0.50/test/test_configuration.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3256 2024-04-10 18:44:45.000000 sciveo-0.0.50/test/test_monitoring.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1554 2024-03-19 14:47:07.000000 sciveo-0.0.50/test/test_runner.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     9045 2024-03-19 14:47:24.000000 sciveo-0.0.50/test/test_sampling.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:57:01.411182 sciveo-0.1.0/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6513 2024-04-17 12:57:01.411042 sciveo-0.1.0/PKG-INFO
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6361 2024-04-17 12:56:26.000000 sciveo-0.1.0/README.md
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:57:01.390706 sciveo-0.1.0/sciveo/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1428 2024-04-17 12:51:40.000000 sciveo-0.1.0/sciveo/__init__.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:57:01.397506 sciveo-0.1.0/sciveo/api/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:04:12.000000 sciveo-0.1.0/sciveo/api/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1788 2024-04-16 17:39:04.000000 sciveo-0.1.0/sciveo/api/base.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1815 2024-04-05 16:37:24.000000 sciveo-0.1.0/sciveo/api/upload.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:57:01.400021 sciveo-0.1.0/sciveo/common/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:03:59.000000 sciveo-0.1.0/sciveo/common/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2043 2024-03-14 17:02:24.000000 sciveo-0.1.0/sciveo/common/configuration.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1583 2024-03-14 17:02:24.000000 sciveo-0.1.0/sciveo/common/model.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3842 2024-04-07 18:52:23.000000 sciveo-0.1.0/sciveo/common/optimizers.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)    10567 2024-03-19 14:47:24.000000 sciveo-0.1.0/sciveo/common/sampling.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:57:01.403406 sciveo-0.1.0/sciveo/common/tools/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:07:07.000000 sciveo-0.1.0/sciveo/common/tools/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1647 2024-04-17 12:51:40.000000 sciveo-0.1.0/sciveo/common/tools/daemon.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1053 2023-11-17 12:42:35.000000 sciveo-0.1.0/sciveo/common/tools/formating.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1654 2024-04-14 08:49:26.000000 sciveo-0.1.0/sciveo/common/tools/hardware.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1071 2023-11-15 15:21:05.000000 sciveo-0.1.0/sciveo/common/tools/logger.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1333 2024-04-17 12:51:40.000000 sciveo-0.1.0/sciveo/common/tools/synchronized.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1087 2024-04-17 12:51:40.000000 sciveo-0.1.0/sciveo/common/tools/timers.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:57:01.405758 sciveo-0.1.0/sciveo/content/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:14:23.000000 sciveo-0.1.0/sciveo/content/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      827 2024-03-14 17:02:24.000000 sciveo-0.1.0/sciveo/content/dataset.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     5859 2024-04-07 18:52:23.000000 sciveo-0.1.0/sciveo/content/experiment.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3129 2024-04-07 18:52:23.000000 sciveo-0.1.0/sciveo/content/project.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2015 2024-03-19 14:47:07.000000 sciveo-0.1.0/sciveo/content/runner.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:57:01.408563 sciveo-0.1.0/sciveo/monitoring/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2024-04-07 18:52:23.000000 sciveo-0.1.0/sciveo/monitoring/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     5898 2024-04-17 12:51:40.000000 sciveo-0.1.0/sciveo/monitoring/monitor.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2564 2024-04-17 12:51:40.000000 sciveo-0.1.0/sciveo/monitoring/network.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1671 2024-04-17 12:51:40.000000 sciveo-0.1.0/sciveo/monitoring/start.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       23 2024-04-17 12:51:59.000000 sciveo-0.1.0/sciveo/version.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:57:01.396153 sciveo-0.1.0/sciveo.egg-info/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6513 2024-04-17 12:57:01.000000 sciveo-0.1.0/sciveo.egg-info/PKG-INFO
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      965 2024-04-17 12:57:01.000000 sciveo-0.1.0/sciveo.egg-info/SOURCES.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        1 2024-04-17 12:57:01.000000 sciveo-0.1.0/sciveo.egg-info/dependency_links.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      112 2024-04-17 12:57:01.000000 sciveo-0.1.0/sciveo.egg-info/requires.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        7 2024-04-17 12:57:01.000000 sciveo-0.1.0/sciveo.egg-info/top_level.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       38 2024-04-17 12:57:01.411237 sciveo-0.1.0/setup.cfg
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      778 2024-04-17 12:51:40.000000 sciveo-0.1.0/setup.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:57:01.410555 sciveo-0.1.0/test/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      521 2024-03-14 17:02:24.000000 sciveo-0.1.0/test/test_configuration.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3256 2024-04-10 18:44:45.000000 sciveo-0.1.0/test/test_monitoring.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1554 2024-03-19 14:47:07.000000 sciveo-0.1.0/test/test_runner.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     9045 2024-03-19 14:47:24.000000 sciveo-0.1.0/test/test_sampling.py
```

### Comparing `sciveo-0.0.50/PKG-INFO` & `sciveo-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 Metadata-Version: 2.1
 Name: sciveo
-Version: 0.0.50
+Version: 0.1.0
 Description-Content-Type: text/markdown
 Provides-Extra: mon
 Provides-Extra: net
 Provides-Extra: all
 
-# SCIVEO - ML/Scientific Experiments Management Client
+# SCIVEO - ML/AI and Scientific tools
 
+## Experiments Management Client
 `sciveo` is a Python library that serves as a client for managing machine learning and scientific experiments on the sciveo.com platform. This library provides a convenient interface to interact with the sciveo.com API, enabling users to organize, track, and analyze their experiments efficiently.
 There are few configuration params samplers, which allows easy parameter tuning. The "auto" sampler perhaps is the easiest to use, but also
 "random" and "grid" ones are available.
 
-There is also the sciveo.monitor() which will start monitoring machine CPU/RAM/GPU etc.
+## Monitoring client
+There is also the sciveo.monitor() which will start monitoring machine CPU/RAM/GPU/NET/DISK/TEMP etc.
+It is very easy to start and use.
 
 
 ## Features
 
 - **Experiment Tracking:** Easily log and track your machine learning experiments.
 - **Experiment Comparison:** Compare different experiments and their results.
 - **Data Visualization:** Visualize experiment metrics and results.
 - **Integration with sciveo.com:** Seamlessly connect and synchronize with the sciveo.com platform.
+- **Monitoring machines (from HPC to jetson nano):** Visualisation and metrics collection in sciveo platform.
 
 ## Installation
 
  - main sciveo
 pip install sciveo
 
  - optional for sciveo monitoring
 pip install sciveo[mon]
+ - optional for sciveo network tools
+pip install sciveo[net]
+
+ - for full installation
+pip install sciveo[all]
 
 ## Example usage
 
 There are few public examples in sciveo.com.
 
 The library has local and remote mode. The local one is ready to use, but for the remote one you will need a sciveo.com account.
```

### Comparing `sciveo-0.0.50/README.md` & `sciveo-0.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,39 @@
-# SCIVEO - ML/Scientific Experiments Management Client
+# SCIVEO - ML/AI and Scientific tools
 
+## Experiments Management Client
 `sciveo` is a Python library that serves as a client for managing machine learning and scientific experiments on the sciveo.com platform. This library provides a convenient interface to interact with the sciveo.com API, enabling users to organize, track, and analyze their experiments efficiently.
 There are few configuration params samplers, which allows easy parameter tuning. The "auto" sampler perhaps is the easiest to use, but also
 "random" and "grid" ones are available.
 
-There is also the sciveo.monitor() which will start monitoring machine CPU/RAM/GPU etc.
+## Monitoring client
+There is also the sciveo.monitor() which will start monitoring machine CPU/RAM/GPU/NET/DISK/TEMP etc.
+It is very easy to start and use.
 
 
 ## Features
 
 - **Experiment Tracking:** Easily log and track your machine learning experiments.
 - **Experiment Comparison:** Compare different experiments and their results.
 - **Data Visualization:** Visualize experiment metrics and results.
 - **Integration with sciveo.com:** Seamlessly connect and synchronize with the sciveo.com platform.
+- **Monitoring machines (from HPC to jetson nano):** Visualisation and metrics collection in sciveo platform.
 
 ## Installation
 
  - main sciveo
 pip install sciveo
 
  - optional for sciveo monitoring
 pip install sciveo[mon]
+ - optional for sciveo network tools
+pip install sciveo[net]
+
+ - for full installation
+pip install sciveo[all]
 
 ## Example usage
 
 There are few public examples in sciveo.com.
 
 The library has local and remote mode. The local one is ready to use, but for the remote one you will need a sciveo.com account.
```

### Comparing `sciveo-0.0.50/sciveo/__init__.py` & `sciveo-0.1.0/sciveo/__init__.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.50/sciveo/api/base.py` & `sciveo-0.1.0/sciveo/api/base.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.50/sciveo/api/upload.py` & `sciveo-0.1.0/sciveo/api/upload.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.50/sciveo/common/configuration.py` & `sciveo-0.1.0/sciveo/common/configuration.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.50/sciveo/common/model.py` & `sciveo-0.1.0/sciveo/common/model.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.50/sciveo/common/optimizers.py` & `sciveo-0.1.0/sciveo/common/optimizers.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.50/sciveo/common/sampling.py` & `sciveo-0.1.0/sciveo/common/sampling.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.50/sciveo/common/tools/daemon.py` & `sciveo-0.1.0/sciveo/common/tools/daemon.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.50/sciveo/common/tools/formating.py` & `sciveo-0.1.0/sciveo/common/tools/formating.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.50/sciveo/common/tools/hardware.py` & `sciveo-0.1.0/sciveo/common/tools/hardware.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.50/sciveo/common/tools/logger.py` & `sciveo-0.1.0/sciveo/common/tools/logger.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.50/sciveo/common/tools/synchronized.py` & `sciveo-0.1.0/sciveo/common/tools/synchronized.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.50/sciveo/common/tools/timers.py` & `sciveo-0.1.0/sciveo/common/tools/timers.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.50/sciveo/content/dataset.py` & `sciveo-0.1.0/sciveo/content/dataset.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.50/sciveo/content/experiment.py` & `sciveo-0.1.0/sciveo/content/experiment.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.50/sciveo/content/project.py` & `sciveo-0.1.0/sciveo/content/project.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.50/sciveo/content/runner.py` & `sciveo-0.1.0/sciveo/content/runner.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.50/sciveo/monitoring/monitor.py` & `sciveo-0.1.0/sciveo/monitoring/monitor.py`

 * *Files 15% similar despite different names*

```diff
@@ -149,14 +149,17 @@
       pass
 
   def get_disk(self):
     try:
       list_metrics = ["read bytes", "write bytes", "read count", "write count", "read time", "write time"]
       disk_io_counters = psutil.disk_io_counters(perdisk=False)
       self.get_io_metrics("DISK", list_metrics, disk_io_counters)
+
+      disk_usage = psutil.disk_usage('/')._asdict()
+      self.data["DISK"]["print"] = f"{disk_usage['percent']}% ({round(disk_usage['used'] / (1024 * 1024 * 1024), 1)} GB / {round(disk_usage['total'] / (1024 * 1024 * 1024), 1)} GB)"
     except Exception as e:
       pass
 
   def get_network(self):
     try:
       list_metrics = ["bytes sent", "bytes recv", "packets sent", "packets recv"]
       net_io_counters = psutil.net_io_counters(pernic=False)
```

### Comparing `sciveo-0.0.50/sciveo/monitoring/network.py` & `sciveo-0.1.0/sciveo/monitoring/network.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.50/sciveo/monitoring/start.py` & `sciveo-0.1.0/sciveo/monitoring/start.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.50/sciveo.egg-info/PKG-INFO` & `sciveo-0.1.0/sciveo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 Metadata-Version: 2.1
 Name: sciveo
-Version: 0.0.50
+Version: 0.1.0
 Description-Content-Type: text/markdown
 Provides-Extra: mon
 Provides-Extra: net
 Provides-Extra: all
 
-# SCIVEO - ML/Scientific Experiments Management Client
+# SCIVEO - ML/AI and Scientific tools
 
+## Experiments Management Client
 `sciveo` is a Python library that serves as a client for managing machine learning and scientific experiments on the sciveo.com platform. This library provides a convenient interface to interact with the sciveo.com API, enabling users to organize, track, and analyze their experiments efficiently.
 There are few configuration params samplers, which allows easy parameter tuning. The "auto" sampler perhaps is the easiest to use, but also
 "random" and "grid" ones are available.
 
-There is also the sciveo.monitor() which will start monitoring machine CPU/RAM/GPU etc.
+## Monitoring client
+There is also the sciveo.monitor() which will start monitoring machine CPU/RAM/GPU/NET/DISK/TEMP etc.
+It is very easy to start and use.
 
 
 ## Features
 
 - **Experiment Tracking:** Easily log and track your machine learning experiments.
 - **Experiment Comparison:** Compare different experiments and their results.
 - **Data Visualization:** Visualize experiment metrics and results.
 - **Integration with sciveo.com:** Seamlessly connect and synchronize with the sciveo.com platform.
+- **Monitoring machines (from HPC to jetson nano):** Visualisation and metrics collection in sciveo platform.
 
 ## Installation
 
  - main sciveo
 pip install sciveo
 
  - optional for sciveo monitoring
 pip install sciveo[mon]
+ - optional for sciveo network tools
+pip install sciveo[net]
+
+ - for full installation
+pip install sciveo[all]
 
 ## Example usage
 
 There are few public examples in sciveo.com.
 
 The library has local and remote mode. The local one is ready to use, but for the remote one you will need a sciveo.com account.
```

### Comparing `sciveo-0.0.50/sciveo.egg-info/SOURCES.txt` & `sciveo-0.1.0/sciveo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.50/setup.py` & `sciveo-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.50/test/test_configuration.py` & `sciveo-0.1.0/test/test_configuration.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.50/test/test_monitoring.py` & `sciveo-0.1.0/test/test_monitoring.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.50/test/test_runner.py` & `sciveo-0.1.0/test/test_runner.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.50/test/test_sampling.py` & `sciveo-0.1.0/test/test_sampling.py`

 * *Files identical despite different names*

