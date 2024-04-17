# Comparing `tmp/stellards-0.0.0.3.tar.gz` & `tmp/stellards-0.0.0.4.tar.gz`

## Comparing `stellards-0.0.0.3.tar` & `stellards-0.0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    25900 2020-02-02 00:00:00.000000 stellards-0.0.0.3/src/StellarDS.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stellards-0.0.0.3/src/__init__.py
--rw-r--r--   0        0        0     5898 2020-02-02 00:00:00.000000 stellards-0.0.0.3/tests/StellarAndBMP180.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 stellards-0.0.0.3/LICENSE
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 stellards-0.0.0.3/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 stellards-0.0.0.3/pyproject.toml
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 stellards-0.0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    25900 2020-02-02 00:00:00.000000 stellards-0.0.0.4/src/StellarDS.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stellards-0.0.0.4/src/__init__.py
+-rw-r--r--   0        0        0     5898 2020-02-02 00:00:00.000000 stellards-0.0.0.4/tests/StellarAndBMP180.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 stellards-0.0.0.4/LICENSE
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 stellards-0.0.0.4/README.md
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 stellards-0.0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 stellards-0.0.0.4/PKG-INFO
```

### Comparing `stellards-0.0.0.3/src/StellarDS.py` & `stellards-0.0.0.4/src/StellarDS.py`

 * *Files identical despite different names*

### Comparing `stellards-0.0.0.3/tests/StellarAndBMP180.py` & `stellards-0.0.0.4/tests/StellarAndBMP180.py`

 * *Files identical despite different names*

### Comparing `stellards-0.0.0.3/LICENSE` & `stellards-0.0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `stellards-0.0.0.3/pyproject.toml` & `stellards-0.0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "StellarDS"
-version = "0.0.0.3"
+version = "0.0.0.4"
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
-packages = ["stellarDS"]
+packages = ["src"]
```

### Comparing `stellards-0.0.0.3/PKG-INFO` & `stellards-0.0.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: StellarDS
-Version: 0.0.0.3
+Version: 0.0.0.4
 Summary: StellarDS.io SDK for Python
 Project-URL: Homepage, https://github.com/StellarDS-SDK/StellarDS-SDK
 Project-URL: Issues, https://github.com/StellarDS-SDK/StellarDS-SDK/issues
 Author-email: StellarDS <info@stellards.io>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

