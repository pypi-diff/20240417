# Comparing `tmp/stellards-0.0.0.7.tar.gz` & `tmp/stellards-0.0.0.8.tar.gz`

## Comparing `stellards-0.0.0.7.tar` & `stellards-0.0.0.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    25900 2020-02-02 00:00:00.000000 stellards-0.0.0.7/StellarDS/StellarDS.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stellards-0.0.0.7/StellarDS/__init__.py
--rw-r--r--   0        0        0     5907 2020-02-02 00:00:00.000000 stellards-0.0.0.7/tests/StellarAndBMP180.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 stellards-0.0.0.7/LICENSE
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 stellards-0.0.0.7/README.md
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 stellards-0.0.0.7/pyproject.toml
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 stellards-0.0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    25900 2020-02-02 00:00:00.000000 stellards-0.0.0.8/StellarDS.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stellards-0.0.0.8/__init__.py
+-rw-r--r--   0        0        0     5907 2020-02-02 00:00:00.000000 stellards-0.0.0.8/tests/StellarAndBMP180.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 stellards-0.0.0.8/LICENSE
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 stellards-0.0.0.8/README.md
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 stellards-0.0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 stellards-0.0.0.8/PKG-INFO
```

### Comparing `stellards-0.0.0.7/StellarDS/StellarDS.py` & `stellards-0.0.0.8/StellarDS.py`

 * *Files identical despite different names*

### Comparing `stellards-0.0.0.7/tests/StellarAndBMP180.py` & `stellards-0.0.0.8/tests/StellarAndBMP180.py`

 * *Files identical despite different names*

### Comparing `stellards-0.0.0.7/LICENSE` & `stellards-0.0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `stellards-0.0.0.7/pyproject.toml` & `stellards-0.0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "StellarDS"
-version = "0.0.0.7"
+version = "0.0.0.8"
 authors = [
   { name="StellarDS", email="info@stellards.io" },
 ]
 description = "StellarDS.io SDK for Python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `stellards-0.0.0.7/PKG-INFO` & `stellards-0.0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: StellarDS
-Version: 0.0.0.7
+Version: 0.0.0.8
 Summary: StellarDS.io SDK for Python
 Project-URL: Homepage, https://github.com/StellarDS-SDK/StellarDS-SDK
 Project-URL: Issues, https://github.com/StellarDS-SDK/StellarDS-SDK/issues
 Author-email: StellarDS <info@stellards.io>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

