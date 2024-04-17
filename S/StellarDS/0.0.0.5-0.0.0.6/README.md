# Comparing `tmp/stellards-0.0.0.5.tar.gz` & `tmp/stellards-0.0.0.6.tar.gz`

## Comparing `stellards-0.0.0.5.tar` & `stellards-0.0.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    25900 2020-02-02 00:00:00.000000 stellards-0.0.0.5/src/StellarDS/StellarDS.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stellards-0.0.0.5/src/StellarDS/__init__.py
--rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 stellards-0.0.0.5/tests/StellarAndBMP180.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 stellards-0.0.0.5/LICENSE
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 stellards-0.0.0.5/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 stellards-0.0.0.5/pyproject.toml
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 stellards-0.0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    25900 2020-02-02 00:00:00.000000 stellards-0.0.0.6/StellarDS/StellarDS.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stellards-0.0.0.6/StellarDS/__init__.py
+-rw-r--r--   0        0        0     5907 2020-02-02 00:00:00.000000 stellards-0.0.0.6/tests/StellarAndBMP180.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 stellards-0.0.0.6/LICENSE
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 stellards-0.0.0.6/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 stellards-0.0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 stellards-0.0.0.6/PKG-INFO
```

### Comparing `stellards-0.0.0.5/src/StellarDS/StellarDS.py` & `stellards-0.0.0.6/StellarDS/StellarDS.py`

 * *Files identical despite different names*

### Comparing `stellards-0.0.0.5/tests/StellarAndBMP180.py` & `stellards-0.0.0.6/tests/StellarAndBMP180.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from src.StellarDS import StellarDS
+from StellarDS.StellarDS import StellarDS
 from datetime import datetime
 from ctypes import c_short
 import smbus2
 import time
 
 DEVICE = 0x77
```

### Comparing `stellards-0.0.0.5/LICENSE` & `stellards-0.0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `stellards-0.0.0.5/pyproject.toml` & `stellards-0.0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "StellarDS"
-version = "0.0.0.5"
+version = "0.0.0.6"
 authors = [
   { name="StellarDS", email="info@stellards.io" },
 ]
 description = "StellarDS.io SDK for Python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `stellards-0.0.0.5/PKG-INFO` & `stellards-0.0.0.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: StellarDS
-Version: 0.0.0.5
+Version: 0.0.0.6
 Summary: StellarDS.io SDK for Python
 Project-URL: Homepage, https://github.com/StellarDS-SDK/StellarDS-SDK
 Project-URL: Issues, https://github.com/StellarDS-SDK/StellarDS-SDK/issues
 Author-email: StellarDS <info@stellards.io>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

