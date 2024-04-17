# Comparing `tmp/rocc-3.0.1.tar.gz` & `tmp/rocc-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocc-3.0.1.tar", last modified: Wed Dec 20 11:26:58 2023, max compression
+gzip compressed data, was "rocc-3.0.2.tar", last modified: Wed Apr 17 10:49:10 2024, max compression
```

## Comparing `rocc-3.0.1.tar` & `rocc-3.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-12-20 11:26:58.102133 rocc-3.0.1/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      526 2023-12-20 11:23:33.000000 rocc-3.0.1/HISTORY.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)     1014 2022-12-01 11:33:46.000000 rocc-3.0.1/LICENSE
--rw-r--r--   0 anthony   (1000) anthony   (1000)      217 2022-11-28 21:00:01.000000 rocc-3.0.1/MANIFEST.in
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4620 2023-12-20 11:26:58.102133 rocc-3.0.1/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)     3286 2022-11-28 21:00:01.000000 rocc-3.0.1/README.rst
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-12-20 11:26:58.102133 rocc-3.0.1/rocc/
--rw-r--r--   0 anthony   (1000) anthony   (1000)       51 2023-12-20 11:24:05.000000 rocc-3.0.1/rocc/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)   505076 2022-12-01 11:34:50.000000 rocc-3.0.1/rocc/calculation.c
--rw-r--r--   0 anthony   (1000) anthony   (1000)      272 2022-11-30 15:20:35.000000 rocc-3.0.1/rocc/rocc.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-12-20 11:26:58.102133 rocc-3.0.1/rocc.egg-info/
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4620 2023-12-20 11:26:58.000000 rocc-3.0.1/rocc.egg-info/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)      313 2023-12-20 11:26:58.000000 rocc-3.0.1/rocc.egg-info/SOURCES.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2023-12-20 11:26:58.000000 rocc-3.0.1/rocc.egg-info/dependency_links.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2022-11-28 21:03:40.000000 rocc-3.0.1/rocc.egg-info/not-zip-safe
--rw-r--r--   0 anthony   (1000) anthony   (1000)       18 2023-12-20 11:26:58.000000 rocc-3.0.1/rocc.egg-info/requires.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        5 2023-12-20 11:26:58.000000 rocc-3.0.1/rocc.egg-info/top_level.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       92 2023-12-20 11:26:58.102133 rocc-3.0.1/setup.cfg
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)     3019 2023-12-20 11:23:33.000000 rocc-3.0.1/setup.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-12-20 11:26:58.102133 rocc-3.0.1/tests/
--rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2022-11-28 21:00:01.000000 rocc-3.0.1/tests/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     5838 2022-12-01 11:33:46.000000 rocc-3.0.1/tests/test_rocc.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-17 10:49:10.763347 rocc-3.0.2/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      599 2024-04-17 10:48:05.000000 rocc-3.0.2/HISTORY.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     1014 2022-12-01 11:33:46.000000 rocc-3.0.2/LICENSE
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      217 2022-11-28 21:00:01.000000 rocc-3.0.2/MANIFEST.in
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4644 2024-04-17 10:49:10.763347 rocc-3.0.2/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     3286 2022-11-28 21:00:01.000000 rocc-3.0.2/README.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-17 10:49:10.763347 rocc-3.0.2/rocc/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       51 2024-04-17 10:48:47.000000 rocc-3.0.2/rocc/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)   505076 2022-12-01 11:34:50.000000 rocc-3.0.2/rocc/calculation.c
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      272 2022-11-30 15:20:35.000000 rocc-3.0.2/rocc/rocc.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-17 10:49:10.763347 rocc-3.0.2/rocc.egg-info/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4644 2024-04-17 10:49:10.000000 rocc-3.0.2/rocc.egg-info/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      313 2024-04-17 10:49:10.000000 rocc-3.0.2/rocc.egg-info/SOURCES.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2024-04-17 10:49:10.000000 rocc-3.0.2/rocc.egg-info/dependency_links.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2022-11-28 21:03:40.000000 rocc-3.0.2/rocc.egg-info/not-zip-safe
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       18 2024-04-17 10:49:10.000000 rocc-3.0.2/rocc.egg-info/requires.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        5 2024-04-17 10:49:10.000000 rocc-3.0.2/rocc.egg-info/top_level.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       92 2024-04-17 10:49:10.763347 rocc-3.0.2/setup.cfg
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)     2971 2024-04-17 10:48:05.000000 rocc-3.0.2/setup.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2024-04-17 10:49:10.763347 rocc-3.0.2/tests/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2022-11-28 21:00:01.000000 rocc-3.0.2/tests/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     5838 2022-12-01 11:33:46.000000 rocc-3.0.2/tests/test_rocc.py
```

### Comparing `rocc-3.0.1/HISTORY.rst` & `rocc-3.0.2/HISTORY.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =======
 History
 =======
 
+3.0.2 (2024-04-17)
+==================
+
+- Compatible with htimeseries 7.
+
 3.0.1 (2023-12-20)
 ==================
 
 - Compatible with htimeseries 6.
 
 3.0.0 (2022-12-01)
 ==================
```

### Comparing `rocc-3.0.1/LICENSE` & `rocc-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rocc-3.0.1/PKG-INFO` & `rocc-3.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: rocc
-Version: 3.0.1
+Version: 3.0.2
 Summary: Rate-of-change check of time series
 Home-page: https://github.com/openmeteo/rocc
 Author: Antonis Christofides
 Author-email: antonis@antonischristofides.com
 License: GNU General Public License v3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: htimeseries<7,>=4
+Requires-Dist: htimeseries<8,>=4
 
 ===========================================
 rocc - Rate-of-change check for time series
 ===========================================
 
 
 .. image:: https://img.shields.io/pypi/v/rocc.svg
@@ -109,14 +108,19 @@
 .. _HTimeseries: https://github.com/openmeteo/htimeseries/
 
 
 =======
 History
 =======
 
+3.0.2 (2024-04-17)
+==================
+
+- Compatible with htimeseries 7.
+
 3.0.1 (2023-12-20)
 ==================
 
 - Compatible with htimeseries 6.
 
 3.0.0 (2022-12-01)
 ==================
```

### Comparing `rocc-3.0.1/README.rst` & `rocc-3.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `rocc-3.0.1/rocc/calculation.c` & `rocc-3.0.2/rocc/calculation.c`

 * *Files identical despite different names*

### Comparing `rocc-3.0.1/rocc.egg-info/PKG-INFO` & `rocc-3.0.2/rocc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: rocc
-Version: 3.0.1
+Version: 3.0.2
 Summary: Rate-of-change check of time series
 Home-page: https://github.com/openmeteo/rocc
 Author: Antonis Christofides
 Author-email: antonis@antonischristofides.com
 License: GNU General Public License v3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: htimeseries<7,>=4
+Requires-Dist: htimeseries<8,>=4
 
 ===========================================
 rocc - Rate-of-change check for time series
 ===========================================
 
 
 .. image:: https://img.shields.io/pypi/v/rocc.svg
@@ -109,14 +108,19 @@
 .. _HTimeseries: https://github.com/openmeteo/htimeseries/
 
 
 =======
 History
 =======
 
+3.0.2 (2024-04-17)
+==================
+
+- Compatible with htimeseries 7.
+
 3.0.1 (2023-12-20)
 ==================
 
 - Compatible with htimeseries 6.
 
 3.0.0 (2022-12-01)
 ==================
```

### Comparing `rocc-3.0.1/setup.py` & `rocc-3.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open("README.rst") as readme_file:
     readme = readme_file.read()
 
 with open("HISTORY.rst") as history_file:
     history = history_file.read()
 
-requirements = ["htimeseries>=4,<7"]
+requirements = ["htimeseries>=4,<8"]
 
 setup_requirements = ["cython>=0.29,<0.30"]
 
 test_requirements = []
 
 
 def use_cython():
@@ -73,19 +73,18 @@
     author="Antonis Christofides",
     author_email="antonis@antonischristofides.com",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Natural Language :: English",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
     description="Rate-of-change check of time series",
     install_requires=requirements,
     license="GNU General Public License v3",
     long_description=readme + "\n\n" + history,
     long_description_content_type="text/x-rst",
     include_package_data=True,
```

### Comparing `rocc-3.0.1/tests/test_rocc.py` & `rocc-3.0.2/tests/test_rocc.py`

 * *Files identical despite different names*

