# Comparing `tmp/sciveo-0.0.49.tar.gz` & `tmp/sciveo-0.0.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciveo-0.0.49.tar", last modified: Tue Apr 16 17:56:09 2024, max compression
+gzip compressed data, was "sciveo-0.0.50.tar", last modified: Wed Apr 17 12:00:18 2024, max compression
```

## Comparing `sciveo-0.0.49.tar` & `sciveo-0.0.50.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-16 17:56:09.946414 sciveo-0.0.49/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     6208 2024-04-16 17:56:09.946226 sciveo-0.0.49/PKG-INFO
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     6055 2024-04-10 20:04:28.000000 sciveo-0.0.49/README.md
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-16 17:56:09.930226 sciveo-0.0.49/sciveo/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1428 2024-04-16 17:53:18.000000 sciveo-0.0.49/sciveo/__init__.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-16 17:56:09.934712 sciveo-0.0.49/sciveo/api/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:04:12.000000 sciveo-0.0.49/sciveo/api/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1788 2024-04-16 17:39:04.000000 sciveo-0.0.49/sciveo/api/base.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1815 2024-04-05 16:37:24.000000 sciveo-0.0.49/sciveo/api/upload.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-16 17:56:09.936430 sciveo-0.0.49/sciveo/common/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:03:59.000000 sciveo-0.0.49/sciveo/common/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2043 2024-03-14 17:02:24.000000 sciveo-0.0.49/sciveo/common/configuration.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1583 2024-03-14 17:02:24.000000 sciveo-0.0.49/sciveo/common/model.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3842 2024-04-07 18:52:23.000000 sciveo-0.0.49/sciveo/common/optimizers.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)    10567 2024-03-19 14:47:24.000000 sciveo-0.0.49/sciveo/common/sampling.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-16 17:56:09.939264 sciveo-0.0.49/sciveo/common/tools/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:07:07.000000 sciveo-0.0.49/sciveo/common/tools/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1647 2024-04-16 17:39:58.000000 sciveo-0.0.49/sciveo/common/tools/daemon.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1053 2023-11-17 12:42:35.000000 sciveo-0.0.49/sciveo/common/tools/formating.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1654 2024-04-14 08:49:26.000000 sciveo-0.0.49/sciveo/common/tools/hardware.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1071 2023-11-15 15:21:05.000000 sciveo-0.0.49/sciveo/common/tools/logger.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1333 2024-04-16 17:40:12.000000 sciveo-0.0.49/sciveo/common/tools/synchronized.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1087 2024-04-16 17:42:03.000000 sciveo-0.0.49/sciveo/common/tools/timers.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-16 17:56:09.940768 sciveo-0.0.49/sciveo/content/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:14:23.000000 sciveo-0.0.49/sciveo/content/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      827 2024-03-14 17:02:24.000000 sciveo-0.0.49/sciveo/content/dataset.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     5859 2024-04-07 18:52:23.000000 sciveo-0.0.49/sciveo/content/experiment.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3129 2024-04-07 18:52:23.000000 sciveo-0.0.49/sciveo/content/project.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2015 2024-03-19 14:47:07.000000 sciveo-0.0.49/sciveo/content/runner.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-16 17:56:09.941964 sciveo-0.0.49/sciveo/monitoring/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2024-04-07 18:52:23.000000 sciveo-0.0.49/sciveo/monitoring/__init__.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     5380 2024-04-14 11:46:31.000000 sciveo-0.0.49/sciveo/monitoring/monitor.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     2564 2024-04-16 17:50:56.000000 sciveo-0.0.49/sciveo/monitoring/network.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1671 2024-04-16 17:41:11.000000 sciveo-0.0.49/sciveo/monitoring/start.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       24 2024-04-16 17:56:04.000000 sciveo-0.0.49/sciveo/version.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-16 17:56:09.933777 sciveo-0.0.49/sciveo.egg-info/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     6208 2024-04-16 17:56:09.000000 sciveo-0.0.49/sciveo.egg-info/PKG-INFO
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      965 2024-04-16 17:56:09.000000 sciveo-0.0.49/sciveo.egg-info/SOURCES.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        1 2024-04-16 17:56:09.000000 sciveo-0.0.49/sciveo.egg-info/dependency_links.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      112 2024-04-16 17:56:09.000000 sciveo-0.0.49/sciveo.egg-info/requires.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)        7 2024-04-16 17:56:09.000000 sciveo-0.0.49/sciveo.egg-info/top_level.txt
--rw-r--r--   0 sgeorgiev   (501) staff       (20)       38 2024-04-16 17:56:09.946472 sciveo-0.0.49/setup.cfg
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      778 2024-04-16 17:42:22.000000 sciveo-0.0.49/setup.py
-drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-16 17:56:09.945889 sciveo-0.0.49/test/
--rw-r--r--   0 sgeorgiev   (501) staff       (20)      521 2024-03-14 17:02:24.000000 sciveo-0.0.49/test/test_configuration.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     3256 2024-04-10 18:44:45.000000 sciveo-0.0.49/test/test_monitoring.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     1554 2024-03-19 14:47:07.000000 sciveo-0.0.49/test/test_runner.py
--rw-r--r--   0 sgeorgiev   (501) staff       (20)     9045 2024-03-19 14:47:24.000000 sciveo-0.0.49/test/test_sampling.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:00:18.606768 sciveo-0.0.50/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6208 2024-04-17 12:00:18.606605 sciveo-0.0.50/PKG-INFO
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6055 2024-04-10 20:04:28.000000 sciveo-0.0.50/README.md
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:00:18.560520 sciveo-0.0.50/sciveo/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1428 2024-04-16 17:53:18.000000 sciveo-0.0.50/sciveo/__init__.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:00:18.570516 sciveo-0.0.50/sciveo/api/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:04:12.000000 sciveo-0.0.50/sciveo/api/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1788 2024-04-16 17:39:04.000000 sciveo-0.0.50/sciveo/api/base.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1815 2024-04-05 16:37:24.000000 sciveo-0.0.50/sciveo/api/upload.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:00:18.573936 sciveo-0.0.50/sciveo/common/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:03:59.000000 sciveo-0.0.50/sciveo/common/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2043 2024-03-14 17:02:24.000000 sciveo-0.0.50/sciveo/common/configuration.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1583 2024-03-14 17:02:24.000000 sciveo-0.0.50/sciveo/common/model.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3842 2024-04-07 18:52:23.000000 sciveo-0.0.50/sciveo/common/optimizers.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)    10567 2024-03-19 14:47:24.000000 sciveo-0.0.50/sciveo/common/sampling.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:00:18.588035 sciveo-0.0.50/sciveo/common/tools/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:07:07.000000 sciveo-0.0.50/sciveo/common/tools/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1647 2024-04-16 17:39:58.000000 sciveo-0.0.50/sciveo/common/tools/daemon.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1053 2023-11-17 12:42:35.000000 sciveo-0.0.50/sciveo/common/tools/formating.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1654 2024-04-14 08:49:26.000000 sciveo-0.0.50/sciveo/common/tools/hardware.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1071 2023-11-15 15:21:05.000000 sciveo-0.0.50/sciveo/common/tools/logger.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1333 2024-04-16 17:40:12.000000 sciveo-0.0.50/sciveo/common/tools/synchronized.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1087 2024-04-16 17:42:03.000000 sciveo-0.0.50/sciveo/common/tools/timers.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:00:18.592724 sciveo-0.0.50/sciveo/content/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2023-11-15 15:14:23.000000 sciveo-0.0.50/sciveo/content/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      827 2024-03-14 17:02:24.000000 sciveo-0.0.50/sciveo/content/dataset.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     5859 2024-04-07 18:52:23.000000 sciveo-0.0.50/sciveo/content/experiment.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3129 2024-04-07 18:52:23.000000 sciveo-0.0.50/sciveo/content/project.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2015 2024-03-19 14:47:07.000000 sciveo-0.0.50/sciveo/content/runner.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:00:18.602281 sciveo-0.0.50/sciveo/monitoring/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        0 2024-04-07 18:52:23.000000 sciveo-0.0.50/sciveo/monitoring/__init__.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     5663 2024-04-17 11:58:08.000000 sciveo-0.0.50/sciveo/monitoring/monitor.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     2564 2024-04-16 17:50:56.000000 sciveo-0.0.50/sciveo/monitoring/network.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1671 2024-04-16 17:41:11.000000 sciveo-0.0.50/sciveo/monitoring/start.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       24 2024-04-17 11:59:53.000000 sciveo-0.0.50/sciveo/version.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:00:18.569688 sciveo-0.0.50/sciveo.egg-info/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     6208 2024-04-17 12:00:18.000000 sciveo-0.0.50/sciveo.egg-info/PKG-INFO
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      965 2024-04-17 12:00:18.000000 sciveo-0.0.50/sciveo.egg-info/SOURCES.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        1 2024-04-17 12:00:18.000000 sciveo-0.0.50/sciveo.egg-info/dependency_links.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      112 2024-04-17 12:00:18.000000 sciveo-0.0.50/sciveo.egg-info/requires.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)        7 2024-04-17 12:00:18.000000 sciveo-0.0.50/sciveo.egg-info/top_level.txt
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)       38 2024-04-17 12:00:18.606824 sciveo-0.0.50/setup.cfg
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      778 2024-04-16 17:42:22.000000 sciveo-0.0.50/setup.py
+drwxr-xr-x   0 sgeorgiev   (501) staff       (20)        0 2024-04-17 12:00:18.606147 sciveo-0.0.50/test/
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)      521 2024-03-14 17:02:24.000000 sciveo-0.0.50/test/test_configuration.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     3256 2024-04-10 18:44:45.000000 sciveo-0.0.50/test/test_monitoring.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     1554 2024-03-19 14:47:07.000000 sciveo-0.0.50/test/test_runner.py
+-rw-r--r--   0 sgeorgiev   (501) staff       (20)     9045 2024-03-19 14:47:24.000000 sciveo-0.0.50/test/test_sampling.py
```

### Comparing `sciveo-0.0.49/PKG-INFO` & `sciveo-0.0.50/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciveo
-Version: 0.0.49
+Version: 0.0.50
 Description-Content-Type: text/markdown
 Provides-Extra: mon
 Provides-Extra: net
 Provides-Extra: all
 
 # SCIVEO - ML/Scientific Experiments Management Client
```

### Comparing `sciveo-0.0.49/README.md` & `sciveo-0.0.50/README.md`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.49/sciveo/__init__.py` & `sciveo-0.0.50/sciveo/__init__.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.49/sciveo/api/base.py` & `sciveo-0.0.50/sciveo/api/base.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.49/sciveo/api/upload.py` & `sciveo-0.0.50/sciveo/api/upload.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.49/sciveo/common/configuration.py` & `sciveo-0.0.50/sciveo/common/configuration.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.49/sciveo/common/model.py` & `sciveo-0.0.50/sciveo/common/model.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.49/sciveo/common/optimizers.py` & `sciveo-0.0.50/sciveo/common/optimizers.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.49/sciveo/common/sampling.py` & `sciveo-0.0.50/sciveo/common/sampling.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.49/sciveo/common/tools/daemon.py` & `sciveo-0.0.50/sciveo/common/tools/daemon.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.49/sciveo/common/tools/formating.py` & `sciveo-0.0.50/sciveo/common/tools/formating.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.49/sciveo/common/tools/hardware.py` & `sciveo-0.0.50/sciveo/common/tools/hardware.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.49/sciveo/common/tools/logger.py` & `sciveo-0.0.50/sciveo/common/tools/logger.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.49/sciveo/common/tools/synchronized.py` & `sciveo-0.0.50/sciveo/common/tools/synchronized.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.49/sciveo/common/tools/timers.py` & `sciveo-0.0.50/sciveo/common/tools/timers.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.49/sciveo/content/dataset.py` & `sciveo-0.0.50/sciveo/content/dataset.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.49/sciveo/content/experiment.py` & `sciveo-0.0.50/sciveo/content/experiment.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.49/sciveo/content/project.py` & `sciveo-0.0.50/sciveo/content/project.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.49/sciveo/content/runner.py` & `sciveo-0.0.50/sciveo/content/runner.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.49/sciveo/monitoring/monitor.py` & `sciveo-0.0.50/sciveo/monitoring/monitor.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
   def __init__(self, period=5):
     super().__init__(period=period)
 
     self.data = HardwareInfo()()
     self.data.setdefault("CPU", {})
     self.data.setdefault("DISK", {})
     self.data.setdefault("NET", {})
+    self.data.setdefault("TEMP", {})
     self.data["RAM"] = {}
     self.data["LOG"] = {}
     self.list_logs = []
 
     self.api = APIRemoteClient()
 
     # Warmup the psutil
@@ -54,14 +55,15 @@
     debug(type(self).__name__, f"init monitor with period={period}", machine_serial, "initial_cpu_usage", initial_cpu_usage)
 
   def __call__(self):
     return self.data
 
   def loop(self):
     self.get_cpu_usage()
+    self.get_temperatures()
     self.get_memory()
     self.get_gpu()
     self.get_disk()
     self.get_network()
 
     self.tail_logs()
     self.data["local_time"] = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
@@ -78,14 +80,22 @@
     try:
       usage_per_core = psutil.cpu_percent(interval=None, percpu=True)
       self.data["CPU"]["usage per core"] = usage_per_core
       self.data["CPU"]["usage"] = np.array(usage_per_core).mean()
     except Exception:
       pass
 
+  def get_temperatures(self):
+    try:
+      temperatures = psutil.sensors_temperatures()
+      for k, v in temperatures.items():
+        self.data["TEMP"][k] = [t.current for t in v]
+    except Exception:
+      pass
+
   def get_memory(self):
     try:
       memory = psutil.virtual_memory()
       self.data["RAM"]["used"] = memory.used
       self.data["RAM"]["total"] = memory.total
       self.data["RAM"]["free"] = memory.free
       # self.data["RAM"]["installed"] = format_memory_size(memory.total)
```

### Comparing `sciveo-0.0.49/sciveo/monitoring/network.py` & `sciveo-0.0.50/sciveo/monitoring/network.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.49/sciveo/monitoring/start.py` & `sciveo-0.0.50/sciveo/monitoring/start.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.49/sciveo.egg-info/PKG-INFO` & `sciveo-0.0.50/sciveo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciveo
-Version: 0.0.49
+Version: 0.0.50
 Description-Content-Type: text/markdown
 Provides-Extra: mon
 Provides-Extra: net
 Provides-Extra: all
 
 # SCIVEO - ML/Scientific Experiments Management Client
```

### Comparing `sciveo-0.0.49/sciveo.egg-info/SOURCES.txt` & `sciveo-0.0.50/sciveo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.49/setup.py` & `sciveo-0.0.50/setup.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.49/test/test_configuration.py` & `sciveo-0.0.50/test/test_configuration.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.49/test/test_monitoring.py` & `sciveo-0.0.50/test/test_monitoring.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.49/test/test_runner.py` & `sciveo-0.0.50/test/test_runner.py`

 * *Files identical despite different names*

### Comparing `sciveo-0.0.49/test/test_sampling.py` & `sciveo-0.0.50/test/test_sampling.py`

 * *Files identical despite different names*

