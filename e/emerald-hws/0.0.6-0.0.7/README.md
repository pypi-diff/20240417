# Comparing `tmp/emerald_hws-0.0.6.tar.gz` & `tmp/emerald_hws-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emerald_hws-0.0.6.tar", last modified: Mon Apr 15 10:10:58 2024, max compression
+gzip compressed data, was "emerald_hws-0.0.7.tar", last modified: Wed Apr 17 11:01:16 2024, max compression
```

## Comparing `emerald_hws-0.0.6.tar` & `emerald_hws-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-15 10:10:58.355442 emerald_hws-0.0.6/
--rw-r--r--   0 ross       (501) staff       (20)     1072 2024-01-24 10:16:13.000000 emerald_hws-0.0.6/LICENSE
--rw-r--r--   0 ross       (501) staff       (20)      694 2024-04-15 10:10:58.354632 emerald_hws-0.0.6/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)       84 2024-01-24 10:15:13.000000 emerald_hws-0.0.6/README.md
--rw-r--r--   0 ross       (501) staff       (20)      824 2024-04-15 10:10:04.000000 emerald_hws-0.0.6/pyproject.toml
--rw-r--r--   0 ross       (501) staff       (20)       38 2024-04-15 10:10:58.355666 emerald_hws-0.0.6/setup.cfg
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-15 10:10:58.344481 emerald_hws-0.0.6/src/
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-15 10:10:58.347910 emerald_hws-0.0.6/src/emerald_hws/
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-15 10:10:58.352689 emerald_hws-0.0.6/src/emerald_hws/__assets__/
--rw-r--r--   0 ross       (501) staff       (20)     1424 2024-01-23 10:06:20.000000 emerald_hws-0.0.6/src/emerald_hws/__assets__/SFSRootCAG2.pem
--rw-r--r--   0 ross       (501) staff       (20)        1 2024-01-24 10:24:29.000000 emerald_hws-0.0.6/src/emerald_hws/__init__.py
--rw-r--r--   0 ross       (501) staff       (20)    12051 2024-04-15 10:07:58.000000 emerald_hws-0.0.6/src/emerald_hws/emeraldhws.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-15 10:10:58.353568 emerald_hws-0.0.6/src/emerald_hws.egg-info/
--rw-r--r--   0 ross       (501) staff       (20)      694 2024-04-15 10:10:58.000000 emerald_hws-0.0.6/src/emerald_hws.egg-info/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)      327 2024-04-15 10:10:58.000000 emerald_hws-0.0.6/src/emerald_hws.egg-info/SOURCES.txt
--rw-r--r--   0 ross       (501) staff       (20)        1 2024-04-15 10:10:58.000000 emerald_hws-0.0.6/src/emerald_hws.egg-info/dependency_links.txt
--rw-r--r--   0 ross       (501) staff       (20)       22 2024-04-15 10:10:58.000000 emerald_hws-0.0.6/src/emerald_hws.egg-info/requires.txt
--rw-r--r--   0 ross       (501) staff       (20)       12 2024-04-15 10:10:58.000000 emerald_hws-0.0.6/src/emerald_hws.egg-info/top_level.txt
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-17 11:01:16.951022 emerald_hws-0.0.7/
+-rw-r--r--   0 ross       (501) staff       (20)     1072 2024-01-24 10:16:13.000000 emerald_hws-0.0.7/LICENSE
+-rw-r--r--   0 ross       (501) staff       (20)      688 2024-04-17 11:01:16.950647 emerald_hws-0.0.7/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)       84 2024-01-24 10:15:13.000000 emerald_hws-0.0.7/README.md
+-rw-r--r--   0 ross       (501) staff       (20)      818 2024-04-17 10:59:24.000000 emerald_hws-0.0.7/pyproject.toml
+-rw-r--r--   0 ross       (501) staff       (20)       38 2024-04-17 11:01:16.951151 emerald_hws-0.0.7/setup.cfg
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-17 11:01:16.944107 emerald_hws-0.0.7/src/
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-17 11:01:16.947821 emerald_hws-0.0.7/src/emerald_hws/
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-17 11:01:16.949567 emerald_hws-0.0.7/src/emerald_hws/__assets__/
+-rw-r--r--   0 ross       (501) staff       (20)     1424 2024-01-23 10:06:20.000000 emerald_hws-0.0.7/src/emerald_hws/__assets__/SFSRootCAG2.pem
+-rw-r--r--   0 ross       (501) staff       (20)        1 2024-01-24 10:24:29.000000 emerald_hws-0.0.7/src/emerald_hws/__init__.py
+-rw-r--r--   0 ross       (501) staff       (20)    13251 2024-04-17 10:56:27.000000 emerald_hws-0.0.7/src/emerald_hws/emeraldhws.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-17 11:01:16.950243 emerald_hws-0.0.7/src/emerald_hws.egg-info/
+-rw-r--r--   0 ross       (501) staff       (20)      688 2024-04-17 11:01:16.000000 emerald_hws-0.0.7/src/emerald_hws.egg-info/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)      327 2024-04-17 11:01:16.000000 emerald_hws-0.0.7/src/emerald_hws.egg-info/SOURCES.txt
+-rw-r--r--   0 ross       (501) staff       (20)        1 2024-04-17 11:01:16.000000 emerald_hws-0.0.7/src/emerald_hws.egg-info/dependency_links.txt
+-rw-r--r--   0 ross       (501) staff       (20)       16 2024-04-17 11:01:16.000000 emerald_hws-0.0.7/src/emerald_hws.egg-info/requires.txt
+-rw-r--r--   0 ross       (501) staff       (20)       12 2024-04-17 11:01:16.000000 emerald_hws-0.0.7/src/emerald_hws.egg-info/top_level.txt
```

### Comparing `emerald_hws-0.0.6/LICENSE` & `emerald_hws-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `emerald_hws-0.0.6/PKG-INFO` & `emerald_hws-0.0.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: emerald_hws
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package to manipulate and monitor Emerald Heat Pump Hot Water Systems
 Author-email: Ross Williamson <ross@inertia.net.nz>
 Project-URL: Homepage, https://github.com/ross-w/emerald_hws_py
 Project-URL: Bug Tracker, https://github.com/ross-w/emerald_hws_py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: boto3
-Requires-Dist: AWSIoTPythonSDK
+Requires-Dist: awsiotsdk
 
 # emerald_hws_py
 Python package for controlling Emerald Heat Pump Hot Water Systems
```

### Comparing `emerald_hws-0.0.6/pyproject.toml` & `emerald_hws-0.0.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "emerald_hws"
-version = "0.0.6"
+version = "0.0.7"
 dependencies = [
   "boto3",
-  "AWSIoTPythonSDK"
+  "awsiotsdk"
 ]
 authors = [
   { name="Ross Williamson", email="ross@inertia.net.nz" },
 ]
 description = "A package to manipulate and monitor Emerald Heat Pump Hot Water Systems"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `emerald_hws-0.0.6/src/emerald_hws/__assets__/SFSRootCAG2.pem` & `emerald_hws-0.0.7/src/emerald_hws/__assets__/SFSRootCAG2.pem`

 * *Files identical despite different names*

### Comparing `emerald_hws-0.0.6/src/emerald_hws.egg-info/PKG-INFO` & `emerald_hws-0.0.7/src/emerald_hws.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: emerald_hws
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package to manipulate and monitor Emerald Heat Pump Hot Water Systems
 Author-email: Ross Williamson <ross@inertia.net.nz>
 Project-URL: Homepage, https://github.com/ross-w/emerald_hws_py
 Project-URL: Bug Tracker, https://github.com/ross-w/emerald_hws_py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: boto3
-Requires-Dist: AWSIoTPythonSDK
+Requires-Dist: awsiotsdk
 
 # emerald_hws_py
 Python package for controlling Emerald Heat Pump Hot Water Systems
```

