# Comparing `tmp/stellards-0.0.0.1.tar.gz` & `tmp/stellards-0.0.0.2.tar.gz`

## Comparing `stellards-0.0.0.1.tar` & `stellards-0.0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    25900 2020-02-02 00:00:00.000000 stellards-0.0.0.1/src/StellarDS/StellarDS.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stellards-0.0.0.1/src/StellarDS/__init__.py
--rw-r--r--   0        0        0     5911 2020-02-02 00:00:00.000000 stellards-0.0.0.1/tests/StellarAndBMP180.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 stellards-0.0.0.1/LICENSE
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 stellards-0.0.0.1/README.md
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 stellards-0.0.0.1/pyproject.toml
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 stellards-0.0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    25900 2020-02-02 00:00:00.000000 stellards-0.0.0.2/src/StellarDS.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stellards-0.0.0.2/src/__init__.py
+-rw-r--r--   0        0        0     5898 2020-02-02 00:00:00.000000 stellards-0.0.0.2/tests/StellarAndBMP180.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 stellards-0.0.0.2/LICENSE
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 stellards-0.0.0.2/README.md
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 stellards-0.0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 stellards-0.0.0.2/PKG-INFO
```

### Comparing `stellards-0.0.0.1/src/StellarDS/StellarDS.py` & `stellards-0.0.0.2/src/StellarDS.py`

 * *Files identical despite different names*

### Comparing `stellards-0.0.0.1/tests/StellarAndBMP180.py` & `stellards-0.0.0.2/tests/StellarAndBMP180.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from SDK.StellarDS_io_PythonLibrary import *
+from .StellarDS import StellarDS
 from datetime import datetime
 from ctypes import c_short
 import smbus2
 import time
 
 DEVICE = 0x77
  
@@ -83,15 +83,15 @@
     return (temperature/10.0,pressure/100.0)
 
 PROJECT_ID = 'your_project_id'
 CLIENT_ID = 'your_client_id'
 CLIENT_SECRET = 'your_client_secret'
 CALLBACK_URL = 'http://localhost:8080'
 #Change to false if you want to use an access token instead of OAuth
-oauth = False
+oauth = True
 #Change to false if you want to authenticate every time you run the script
 persistent = True
 ACCESS_TOKEN = 'your_access_token'
 
 class SensorData:
     def __init__(self, chip_id, chip_version, temperature, pressure, measure_date):
         self.chip_id = chip_id
```

### Comparing `stellards-0.0.0.1/LICENSE` & `stellards-0.0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stellards-0.0.0.1/pyproject.toml` & `stellards-0.0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "StellarDS"
-version = "0.0.0.1"
+version = "0.0.0.2"
 authors = [
   { name="StellarDS", email="info@stellards.io" },
 ]
 description = "StellarDS.io SDK for Python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `stellards-0.0.0.1/PKG-INFO` & `stellards-0.0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: StellarDS
-Version: 0.0.0.1
+Version: 0.0.0.2
 Summary: StellarDS.io SDK for Python
 Project-URL: Homepage, https://github.com/StellarDS-SDK/StellarDS-SDK
 Project-URL: Issues, https://github.com/StellarDS-SDK/StellarDS-SDK/issues
 Author-email: StellarDS <info@stellards.io>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

