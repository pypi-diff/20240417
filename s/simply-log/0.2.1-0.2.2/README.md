# Comparing `tmp/simply-log-0.2.1.tar.gz` & `tmp/simply-log-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simply-log-0.2.1.tar", last modified: Wed Apr 17 10:02:25 2024, max compression
+gzip compressed data, was "simply-log-0.2.2.tar", last modified: Wed Apr 17 10:08:18 2024, max compression
```

## Comparing `simply-log-0.2.1.tar` & `simply-log-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-04-17 10:02:25.248692 simply-log-0.2.1/
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     1006 2024-04-17 10:02:25.248571 simply-log-0.2.1/PKG-INFO
--rw-r--r--   0 corneliusvincent   (501) staff       (20)      911 2024-04-17 10:02:09.000000 simply-log-0.2.1/README.md
-drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-04-17 10:02:25.247703 simply-log-0.2.1/log/
--rw-r--r--   0 corneliusvincent   (501) staff       (20)       45 2024-04-17 09:35:52.000000 simply-log-0.2.1/log/__init__.py
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     1067 2024-04-17 08:42:59.000000 simply-log-0.2.1/log/main.py
--rw-r--r--   0 corneliusvincent   (501) staff       (20)       38 2024-04-17 10:02:25.248748 simply-log-0.2.1/setup.cfg
--rw-r--r--   0 corneliusvincent   (501) staff       (20)      310 2024-04-17 10:01:10.000000 simply-log-0.2.1/setup.py
-drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-04-17 10:02:25.248396 simply-log-0.2.1/simply_log.egg-info/
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     1006 2024-04-17 10:02:25.000000 simply-log-0.2.1/simply_log.egg-info/PKG-INFO
--rw-r--r--   0 corneliusvincent   (501) staff       (20)      182 2024-04-17 10:02:25.000000 simply-log-0.2.1/simply_log.egg-info/SOURCES.txt
--rw-r--r--   0 corneliusvincent   (501) staff       (20)        1 2024-04-17 10:02:25.000000 simply-log-0.2.1/simply_log.egg-info/dependency_links.txt
--rw-r--r--   0 corneliusvincent   (501) staff       (20)        4 2024-04-17 10:02:25.000000 simply-log-0.2.1/simply_log.egg-info/top_level.txt
+drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-04-17 10:08:18.781011 simply-log-0.2.2/
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     1045 2024-04-17 10:08:18.780876 simply-log-0.2.2/PKG-INFO
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)      911 2024-04-17 10:02:09.000000 simply-log-0.2.2/README.md
+drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-04-17 10:08:18.779974 simply-log-0.2.2/log/
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)       45 2024-04-17 09:35:52.000000 simply-log-0.2.2/log/__init__.py
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     1067 2024-04-17 08:42:59.000000 simply-log-0.2.2/log/main.py
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)       38 2024-04-17 10:08:18.781054 simply-log-0.2.2/setup.cfg
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)      359 2024-04-17 10:08:13.000000 simply-log-0.2.2/setup.py
+drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-04-17 10:08:18.780682 simply-log-0.2.2/simply_log.egg-info/
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     1045 2024-04-17 10:08:18.000000 simply-log-0.2.2/simply_log.egg-info/PKG-INFO
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)      182 2024-04-17 10:08:18.000000 simply-log-0.2.2/simply_log.egg-info/SOURCES.txt
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)        1 2024-04-17 10:08:18.000000 simply-log-0.2.2/simply_log.egg-info/dependency_links.txt
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)        4 2024-04-17 10:08:18.000000 simply-log-0.2.2/simply_log.egg-info/top_level.txt
```

### Comparing `simply-log-0.2.1/PKG-INFO` & `simply-log-0.2.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-Metadata-Version: 2.1
-Name: simply-log
-Version: 0.2.1
-Description-Content-Type: text/markdown
-
 # Text File Generation Module
 
 This Python module provides a simple logging functionality, allowing users to generate text log files.
 
 ## Usage
 
 Once installed, you can import the module into your Python script like this:
```

### Comparing `simply-log-0.2.1/README.md` & `simply-log-0.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Metadata-Version: 2.1
+Name: simply-log
+Version: 0.2.2
+Summary: A simple logging.txt library 
+Description-Content-Type: text/markdown
+
 # Text File Generation Module
 
 This Python module provides a simple logging functionality, allowing users to generate text log files.
 
 ## Usage
 
 Once installed, you can import the module into your Python script like this:
```

### Comparing `simply-log-0.2.1/log/main.py` & `simply-log-0.2.2/log/main.py`

 * *Files identical despite different names*

### Comparing `simply-log-0.2.1/simply_log.egg-info/PKG-INFO` & `simply-log-0.2.2/simply_log.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: simply-log
-Version: 0.2.1
+Version: 0.2.2
+Summary: A simple logging.txt library 
 Description-Content-Type: text/markdown
 
 # Text File Generation Module
 
 This Python module provides a simple logging functionality, allowing users to generate text log files.
 
 ## Usage
```

