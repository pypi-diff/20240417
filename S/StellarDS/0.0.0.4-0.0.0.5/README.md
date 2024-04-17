# Comparing `tmp/stellards-0.0.0.4.tar.gz` & `tmp/stellards-0.0.0.5.tar.gz`

## Comparing `stellards-0.0.0.4.tar` & `stellards-0.0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    25900 2020-02-02 00:00:00.000000 stellards-0.0.0.4/src/StellarDS.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stellards-0.0.0.4/src/__init__.py
--rw-r--r--   0        0        0     5898 2020-02-02 00:00:00.000000 stellards-0.0.0.4/tests/StellarAndBMP180.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 stellards-0.0.0.4/LICENSE
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 stellards-0.0.0.4/README.md
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 stellards-0.0.0.4/pyproject.toml
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 stellards-0.0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    25900 2020-02-02 00:00:00.000000 stellards-0.0.0.5/src/StellarDS/StellarDS.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stellards-0.0.0.5/src/StellarDS/__init__.py
+-rw-r--r--   0        0        0     5901 2020-02-02 00:00:00.000000 stellards-0.0.0.5/tests/StellarAndBMP180.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 stellards-0.0.0.5/LICENSE
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 stellards-0.0.0.5/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 stellards-0.0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 stellards-0.0.0.5/PKG-INFO
```

### Comparing `stellards-0.0.0.4/src/StellarDS.py` & `stellards-0.0.0.5/src/StellarDS/StellarDS.py`

 * *Files identical despite different names*

### Comparing `stellards-0.0.0.4/tests/StellarAndBMP180.py` & `stellards-0.0.0.5/tests/StellarAndBMP180.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .StellarDS import StellarDS
+from src.StellarDS import StellarDS
 from datetime import datetime
 from ctypes import c_short
 import smbus2
 import time
 
 DEVICE = 0x77
```

### Comparing `stellards-0.0.0.4/LICENSE` & `stellards-0.0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `stellards-0.0.0.4/pyproject.toml` & `stellards-0.0.0.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "StellarDS"
-version = "0.0.0.4"
+version = "0.0.0.5"
 authors = [
   { name="StellarDS", email="info@stellards.io" },
 ]
 description = "StellarDS.io SDK for Python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -18,8 +18,8 @@
 ]
 
 [project.urls]
 Homepage = "https://github.com/StellarDS-SDK/StellarDS-SDK"
 Issues = "https://github.com/StellarDS-SDK/StellarDS-SDK/issues"
 
 [tool.hatch.build.targets.wheel]
-packages = ["src"]
+packages = ["StellarDS"]
```

### Comparing `stellards-0.0.0.4/PKG-INFO` & `stellards-0.0.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: StellarDS
-Version: 0.0.0.4
+Version: 0.0.0.5
 Summary: StellarDS.io SDK for Python
 Project-URL: Homepage, https://github.com/StellarDS-SDK/StellarDS-SDK
 Project-URL: Issues, https://github.com/StellarDS-SDK/StellarDS-SDK/issues
 Author-email: StellarDS <info@stellards.io>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

