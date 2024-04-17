# Comparing `tmp/sciveo-0.1.0.tar.gz` & `tmp/sciveo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciveo-0.1.0.tar", last modified: Wed Apr 17 12:57:01 2024, max compression
+gzip compressed data, was "sciveo-0.1.1.tar", last modified: Wed Apr 17 13:34:53 2024, max compression
```

## Comparing `sciveo-0.1.0.tar` & `sciveo-0.1.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:57:01.411182 sciveo-0.1.0/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     6513 2024-04-17 12:57:01.411042 sciveo-0.1.0/PKG-INFO
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     6361 2024-04-17 12:56:26.000000 sciveo-0.1.0/README.md
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:57:01.390706 sciveo-0.1.0/sciveo/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1428 2024-04-17 12:51:40.000000 sciveo-0.1.0/sciveo/__init__.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:57:01.397506 sciveo-0.1.0/sciveo/api/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:04:12.000000 sciveo-0.1.0/sciveo/api/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1788 2024-04-16 17:39:04.000000 sciveo-0.1.0/sciveo/api/base.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1815 2024-04-05 16:37:24.000000 sciveo-0.1.0/sciveo/api/upload.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:57:01.400021 sciveo-0.1.0/sciveo/common/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:03:59.000000 sciveo-0.1.0/sciveo/common/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2043 2024-03-14 17:02:24.000000 sciveo-0.1.0/sciveo/common/configuration.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1583 2024-03-14 17:02:24.000000 sciveo-0.1.0/sciveo/common/model.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3842 2024-04-07 18:52:23.000000 sciveo-0.1.0/sciveo/common/optimizers.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)    10567 2024-03-19 14:47:24.000000 sciveo-0.1.0/sciveo/common/sampling.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:57:01.403406 sciveo-0.1.0/sciveo/common/tools/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:07:07.000000 sciveo-0.1.0/sciveo/common/tools/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1647 2024-04-17 12:51:40.000000 sciveo-0.1.0/sciveo/common/tools/daemon.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1053 2023-11-17 12:42:35.000000 sciveo-0.1.0/sciveo/common/tools/formating.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1654 2024-04-14 08:49:26.000000 sciveo-0.1.0/sciveo/common/tools/hardware.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1071 2023-11-15 15:21:05.000000 sciveo-0.1.0/sciveo/common/tools/logger.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1333 2024-04-17 12:51:40.000000 sciveo-0.1.0/sciveo/common/tools/synchronized.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1087 2024-04-17 12:51:40.000000 sciveo-0.1.0/sciveo/common/tools/timers.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:57:01.405758 sciveo-0.1.0/sciveo/content/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:14:23.000000 sciveo-0.1.0/sciveo/content/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      827 2024-03-14 17:02:24.000000 sciveo-0.1.0/sciveo/content/dataset.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     5859 2024-04-07 18:52:23.000000 sciveo-0.1.0/sciveo/content/experiment.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3129 2024-04-07 18:52:23.000000 sciveo-0.1.0/sciveo/content/project.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2015 2024-03-19 14:47:07.000000 sciveo-0.1.0/sciveo/content/runner.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:57:01.408563 sciveo-0.1.0/sciveo/monitoring/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2024-04-07 18:52:23.000000 sciveo-0.1.0/sciveo/monitoring/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     5898 2024-04-17 12:51:40.000000 sciveo-0.1.0/sciveo/monitoring/monitor.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2564 2024-04-17 12:51:40.000000 sciveo-0.1.0/sciveo/monitoring/network.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1671 2024-04-17 12:51:40.000000 sciveo-0.1.0/sciveo/monitoring/start.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       23 2024-04-17 12:51:59.000000 sciveo-0.1.0/sciveo/version.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:57:01.396153 sciveo-0.1.0/sciveo.egg-info/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     6513 2024-04-17 12:57:01.000000 sciveo-0.1.0/sciveo.egg-info/PKG-INFO
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      965 2024-04-17 12:57:01.000000 sciveo-0.1.0/sciveo.egg-info/SOURCES.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        1 2024-04-17 12:57:01.000000 sciveo-0.1.0/sciveo.egg-info/dependency_links.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      112 2024-04-17 12:57:01.000000 sciveo-0.1.0/sciveo.egg-info/requires.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        7 2024-04-17 12:57:01.000000 sciveo-0.1.0/sciveo.egg-info/top_level.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       38 2024-04-17 12:57:01.411237 sciveo-0.1.0/setup.cfg
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      778 2024-04-17 12:51:40.000000 sciveo-0.1.0/setup.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:57:01.410555 sciveo-0.1.0/test/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      521 2024-03-14 17:02:24.000000 sciveo-0.1.0/test/test_configuration.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3256 2024-04-10 18:44:45.000000 sciveo-0.1.0/test/test_monitoring.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1554 2024-03-19 14:47:07.000000 sciveo-0.1.0/test/test_runner.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     9045 2024-03-19 14:47:24.000000 sciveo-0.1.0/test/test_sampling.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 13:34:53.699225 sciveo-0.1.1/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6513 2024-04-17 13:34:53.699078 sciveo-0.1.1/PKG-INFO
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6361 2024-04-17 12:58:32.000000 sciveo-0.1.1/README.md
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 13:34:53.675412 sciveo-0.1.1/sciveo/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1428 2024-04-17 12:51:40.000000 sciveo-0.1.1/sciveo/__init__.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 13:34:53.686145 sciveo-0.1.1/sciveo/api/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:04:12.000000 sciveo-0.1.1/sciveo/api/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1788 2024-04-16 17:39:04.000000 sciveo-0.1.1/sciveo/api/base.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1815 2024-04-05 16:37:24.000000 sciveo-0.1.1/sciveo/api/upload.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 13:34:53.688021 sciveo-0.1.1/sciveo/common/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:03:59.000000 sciveo-0.1.1/sciveo/common/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2043 2024-03-14 17:02:24.000000 sciveo-0.1.1/sciveo/common/configuration.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1583 2024-03-14 17:02:24.000000 sciveo-0.1.1/sciveo/common/model.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3842 2024-04-07 18:52:23.000000 sciveo-0.1.1/sciveo/common/optimizers.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)    10567 2024-03-19 14:47:24.000000 sciveo-0.1.1/sciveo/common/sampling.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 13:34:53.692409 sciveo-0.1.1/sciveo/common/tools/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:07:07.000000 sciveo-0.1.1/sciveo/common/tools/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1647 2024-04-17 12:51:40.000000 sciveo-0.1.1/sciveo/common/tools/daemon.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1053 2023-11-17 12:42:35.000000 sciveo-0.1.1/sciveo/common/tools/formating.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1654 2024-04-17 13:30:32.000000 sciveo-0.1.1/sciveo/common/tools/hardware.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1071 2023-11-15 15:21:05.000000 sciveo-0.1.1/sciveo/common/tools/logger.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1333 2024-04-17 12:51:40.000000 sciveo-0.1.1/sciveo/common/tools/synchronized.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1087 2024-04-17 12:51:40.000000 sciveo-0.1.1/sciveo/common/tools/timers.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 13:34:53.696836 sciveo-0.1.1/sciveo/content/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:14:23.000000 sciveo-0.1.1/sciveo/content/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      827 2024-03-14 17:02:24.000000 sciveo-0.1.1/sciveo/content/dataset.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     5859 2024-04-07 18:52:23.000000 sciveo-0.1.1/sciveo/content/experiment.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3129 2024-04-07 18:52:23.000000 sciveo-0.1.1/sciveo/content/project.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2015 2024-03-19 14:47:07.000000 sciveo-0.1.1/sciveo/content/runner.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 13:34:53.697788 sciveo-0.1.1/sciveo/monitoring/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2024-04-07 18:52:23.000000 sciveo-0.1.1/sciveo/monitoring/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     5858 2024-04-17 13:32:18.000000 sciveo-0.1.1/sciveo/monitoring/monitor.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2564 2024-04-17 12:51:40.000000 sciveo-0.1.1/sciveo/monitoring/network.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1671 2024-04-17 12:51:40.000000 sciveo-0.1.1/sciveo/monitoring/start.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       23 2024-04-17 13:33:03.000000 sciveo-0.1.1/sciveo/version.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 13:34:53.684823 sciveo-0.1.1/sciveo.egg-info/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6513 2024-04-17 13:34:53.000000 sciveo-0.1.1/sciveo.egg-info/PKG-INFO
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      965 2024-04-17 13:34:53.000000 sciveo-0.1.1/sciveo.egg-info/SOURCES.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        1 2024-04-17 13:34:53.000000 sciveo-0.1.1/sciveo.egg-info/dependency_links.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      112 2024-04-17 13:34:53.000000 sciveo-0.1.1/sciveo.egg-info/requires.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        7 2024-04-17 13:34:53.000000 sciveo-0.1.1/sciveo.egg-info/top_level.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       38 2024-04-17 13:34:53.699282 sciveo-0.1.1/setup.cfg
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      778 2024-04-17 12:51:40.000000 sciveo-0.1.1/setup.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 13:34:53.698707 sciveo-0.1.1/test/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      521 2024-03-14 17:02:24.000000 sciveo-0.1.1/test/test_configuration.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3256 2024-04-10 18:44:45.000000 sciveo-0.1.1/test/test_monitoring.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1554 2024-03-19 14:47:07.000000 sciveo-0.1.1/test/test_runner.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     9045 2024-03-19 14:47:24.000000 sciveo-0.1.1/test/test_sampling.py
```

### Comparing `sciveo-0.1.0/PKG-INFO` & `sciveo-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciveo
-Version: 0.1.0
+Version: 0.1.1
 Description-Content-Type: text/markdown
 Provides-Extra: mon
 Provides-Extra: net
 Provides-Extra: all
 
 # SCIVEO - ML/AI and Scientific tools
```

### Comparing `sciveo-0.1.0/README.md` & `sciveo-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.0/sciveo/__init__.py` & `sciveo-0.1.1/sciveo/__init__.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.0/sciveo/api/base.py` & `sciveo-0.1.1/sciveo/api/base.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.0/sciveo/api/upload.py` & `sciveo-0.1.1/sciveo/api/upload.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.0/sciveo/common/configuration.py` & `sciveo-0.1.1/sciveo/common/configuration.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.0/sciveo/common/model.py` & `sciveo-0.1.1/sciveo/common/model.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.0/sciveo/common/optimizers.py` & `sciveo-0.1.1/sciveo/common/optimizers.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.0/sciveo/common/sampling.py` & `sciveo-0.1.1/sciveo/common/sampling.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.0/sciveo/common/tools/daemon.py` & `sciveo-0.1.1/sciveo/common/tools/daemon.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.0/sciveo/common/tools/formating.py` & `sciveo-0.1.1/sciveo/common/tools/formating.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.0/sciveo/common/tools/hardware.py` & `sciveo-0.1.1/sciveo/common/tools/hardware.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.0/sciveo/common/tools/logger.py` & `sciveo-0.1.1/sciveo/common/tools/logger.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.0/sciveo/common/tools/synchronized.py` & `sciveo-0.1.1/sciveo/common/tools/synchronized.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.0/sciveo/common/tools/timers.py` & `sciveo-0.1.1/sciveo/common/tools/timers.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.0/sciveo/content/dataset.py` & `sciveo-0.1.1/sciveo/content/dataset.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.0/sciveo/content/experiment.py` & `sciveo-0.1.1/sciveo/content/experiment.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.0/sciveo/content/project.py` & `sciveo-0.1.1/sciveo/content/project.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.0/sciveo/content/runner.py` & `sciveo-0.1.1/sciveo/content/runner.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.0/sciveo/monitoring/monitor.py` & `sciveo-0.1.1/sciveo/monitoring/monitor.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,24 +11,40 @@
 
 import os
 import subprocess
 import time
 import datetime
 import socket
 import psutil
+import platform
 import uuid
 import numpy as np
 
 from sciveo.common.tools.logger import *
 from sciveo.common.tools.daemon import DaemonBase
 from sciveo.common.tools.hardware import *
 from sciveo.common.tools.formating import format_memory_size
 from sciveo.api.base import APIRemoteClient
 
 
+class MonitorTools:
+  @staticmethod
+  def serial():
+    machine_serial = ""
+    s = "-"
+    list_uid_calls = [socket.gethostname, psutil.cpu_count, platform.processor]
+    for uid_call in list_uid_calls:
+      try:
+        machine_serial += f"{uid_call()}{s}"
+        s = ""
+      except Exception:
+        pass
+    return machine_serial
+
+
 class BaseMonitor(DaemonBase):
   def __init__(self, period=5):
     super().__init__(period=period)
 
     self.data = HardwareInfo()()
     self.data.setdefault("CPU", {})
     self.data.setdefault("DISK", {})
@@ -46,15 +62,15 @@
     self.previous_io_counters = {
       "DISK": psutil.disk_io_counters(perdisk=False),
       "NET": psutil.net_io_counters(pernic=False)
     }
     self.previous_time = {"DISK": time.time(), "NET": time.time()}
     time.sleep(1)
 
-    machine_serial = self.getserial()
+    machine_serial = MonitorTools.serial()
 
     debug(type(self).__name__, f"init monitor with period={period}", machine_serial, "initial_cpu_usage", initial_cpu_usage)
 
   def __call__(self):
     return self.data
 
   def loop(self):
@@ -99,30 +115,14 @@
       self.data["RAM"]["total"] = memory.total
       self.data["RAM"]["free"] = memory.free
       # self.data["RAM"]["installed"] = format_memory_size(memory.total)
       self.data["RAM"]["print"] = f"total: {format_memory_size(memory.total)} used: {format_memory_size(memory.used)}"
     except Exception:
       pass
 
-  def getserial(self):
-    machine_serial = None
-    try:
-      machine_serial = f"{socket.gethostname()}-{uuid.getnode()}"
-    except Exception:
-      pass
-    if machine_serial is None:
-      try:
-        machine_serial = f"UUID-{uuid.getnode()}"
-      except Exception:
-        pass
-    if machine_serial is None:
-      machine_serial = f"RND-{random_token(8)}"
-    self.data["serial"] = machine_serial
-    return machine_serial
-
   def tail_file(self, file_path, block_size=1024):
     result = ["EMPTY"]
     try:
       with open(file_path,'rb') as fp:
         fp.seek(-block_size, os.SEEK_END)
         result = str(fp.read(block_size).rstrip()).split("\\n")
     except Exception as e:
@@ -178,12 +178,14 @@
       if "bytes" in metric_name:
         speed_metric = metric_name.replace("bytes", "speed")
         self.data[name][speed_metric] = self.data[name][metric_name] / time_diff
     self.previous_time[name] = time.time()
     self.previous_io_counters[name] = io_counters
 
 if __name__ == "__main__":
+  print(MonitorTools.serial())
+
   mon = BaseMonitor(period=10)
   mon.start()
 
   while(True):
     time.sleep(30)
```

### Comparing `sciveo-0.1.0/sciveo/monitoring/network.py` & `sciveo-0.1.1/sciveo/monitoring/network.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.0/sciveo/monitoring/start.py` & `sciveo-0.1.1/sciveo/monitoring/start.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.0/sciveo.egg-info/PKG-INFO` & `sciveo-0.1.1/sciveo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciveo
-Version: 0.1.0
+Version: 0.1.1
 Description-Content-Type: text/markdown
 Provides-Extra: mon
 Provides-Extra: net
 Provides-Extra: all
 
 # SCIVEO - ML/AI and Scientific tools
```

### Comparing `sciveo-0.1.0/sciveo.egg-info/SOURCES.txt` & `sciveo-0.1.1/sciveo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.0/setup.py` & `sciveo-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.0/test/test_configuration.py` & `sciveo-0.1.1/test/test_configuration.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.0/test/test_monitoring.py` & `sciveo-0.1.1/test/test_monitoring.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.0/test/test_runner.py` & `sciveo-0.1.1/test/test_runner.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.1.0/test/test_sampling.py` & `sciveo-0.1.1/test/test_sampling.py`

 * *Files identical despite different names*

