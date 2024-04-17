# Comparing `tmp/testontoplibrary-0.0.1.tar.gz` & `tmp/testontoplibrary-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testontoplibrary-0.0.1.tar", last modified: Wed Apr 17 19:56:09 2024, max compression
+gzip compressed data, was "testontoplibrary-0.0.2.tar", last modified: Wed Apr 17 21:12:20 2024, max compression
```

## Comparing `testontoplibrary-0.0.1.tar` & `testontoplibrary-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 19:56:09.627897 testontoplibrary-0.0.1/
-drwxrwxrwx   0        0        0        0 2024-04-17 19:56:09.592898 testontoplibrary-0.0.1/Calculations/
-drwxrwxrwx   0        0        0        0 2024-04-17 19:56:09.620900 testontoplibrary-0.0.1/Calculations/testontoplibrary.egg-info/
--rw-rw-rw-   0        0        0     1671 2024-04-17 19:56:09.000000 testontoplibrary-0.0.1/Calculations/testontoplibrary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2024-04-17 19:56:09.000000 testontoplibrary-0.0.1/Calculations/testontoplibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 19:56:09.000000 testontoplibrary-0.0.1/Calculations/testontoplibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 19:56:09.000000 testontoplibrary-0.0.1/Calculations/testontoplibrary.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1077 2024-04-17 19:55:34.000000 testontoplibrary-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1671 2024-04-17 19:56:09.624900 testontoplibrary-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      257 2024-04-16 21:28:30.000000 testontoplibrary-0.0.1/README.txt
--rw-rw-rw-   0        0        0       86 2024-04-16 21:25:53.000000 testontoplibrary-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      747 2024-04-17 19:56:09.628898 testontoplibrary-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 21:12:20.502382 testontoplibrary-0.0.2/
+-rw-rw-rw-   0        0        0     1077 2024-04-17 19:55:34.000000 testontoplibrary-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1671 2024-04-17 21:12:20.499381 testontoplibrary-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2024-04-16 21:28:30.000000 testontoplibrary-0.0.2/README.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 21:12:20.462375 testontoplibrary-0.0.2/calculator/
+drwxrwxrwx   0        0        0        0 2024-04-17 21:12:20.496381 testontoplibrary-0.0.2/calculator/testontoplibrary.egg-info/
+-rw-rw-rw-   0        0        0     1671 2024-04-17 21:12:20.000000 testontoplibrary-0.0.2/calculator/testontoplibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2024-04-17 21:12:20.000000 testontoplibrary-0.0.2/calculator/testontoplibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 21:12:20.000000 testontoplibrary-0.0.2/calculator/testontoplibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 21:12:20.000000 testontoplibrary-0.0.2/calculator/testontoplibrary.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-16 21:25:53.000000 testontoplibrary-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      743 2024-04-17 21:12:20.503382 testontoplibrary-0.0.2/setup.cfg
```

### Comparing `testontoplibrary-0.0.1/Calculations/testontoplibrary.egg-info/PKG-INFO` & `testontoplibrary-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testontoplibrary
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple Python package
 Home-page: https://github.com/erezklr/TestOnTopLibrary
 Author: erez keller
 Author-email: erezk@cyber.org.il
 Project-URL: Bug Tracker, https://github.com/erezklr/TestOnTopLibrary
 Project-URL: repository, https://github.com/erezklr/TestOnTopLibrary
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testontoplibrary-0.0.1/LICENSE.txt` & `testontoplibrary-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `testontoplibrary-0.0.1/PKG-INFO` & `testontoplibrary-0.0.2/calculator/testontoplibrary.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testontoplibrary
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple Python package
 Home-page: https://github.com/erezklr/TestOnTopLibrary
 Author: erez keller
 Author-email: erezk@cyber.org.il
 Project-URL: Bug Tracker, https://github.com/erezklr/TestOnTopLibrary
 Project-URL: repository, https://github.com/erezklr/TestOnTopLibrary
 Classifier: Programming Language :: Python :: 3
```

