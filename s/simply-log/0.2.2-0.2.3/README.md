# Comparing `tmp/simply-log-0.2.2.tar.gz` & `tmp/simply-log-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simply-log-0.2.2.tar", last modified: Wed Apr 17 10:08:18 2024, max compression
+gzip compressed data, was "simply-log-0.2.3.tar", last modified: Wed Apr 17 10:14:57 2024, max compression
```

## Comparing `simply-log-0.2.2.tar` & `simply-log-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-04-17 10:08:18.781011 simply-log-0.2.2/
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     1045 2024-04-17 10:08:18.780876 simply-log-0.2.2/PKG-INFO
--rw-r--r--   0 corneliusvincent   (501) staff       (20)      911 2024-04-17 10:02:09.000000 simply-log-0.2.2/README.md
-drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-04-17 10:08:18.779974 simply-log-0.2.2/log/
--rw-r--r--   0 corneliusvincent   (501) staff       (20)       45 2024-04-17 09:35:52.000000 simply-log-0.2.2/log/__init__.py
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     1067 2024-04-17 08:42:59.000000 simply-log-0.2.2/log/main.py
--rw-r--r--   0 corneliusvincent   (501) staff       (20)       38 2024-04-17 10:08:18.781054 simply-log-0.2.2/setup.cfg
--rw-r--r--   0 corneliusvincent   (501) staff       (20)      359 2024-04-17 10:08:13.000000 simply-log-0.2.2/setup.py
-drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-04-17 10:08:18.780682 simply-log-0.2.2/simply_log.egg-info/
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     1045 2024-04-17 10:08:18.000000 simply-log-0.2.2/simply_log.egg-info/PKG-INFO
--rw-r--r--   0 corneliusvincent   (501) staff       (20)      182 2024-04-17 10:08:18.000000 simply-log-0.2.2/simply_log.egg-info/SOURCES.txt
--rw-r--r--   0 corneliusvincent   (501) staff       (20)        1 2024-04-17 10:08:18.000000 simply-log-0.2.2/simply_log.egg-info/dependency_links.txt
--rw-r--r--   0 corneliusvincent   (501) staff       (20)        4 2024-04-17 10:08:18.000000 simply-log-0.2.2/simply_log.egg-info/top_level.txt
+drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-04-17 10:14:57.411185 simply-log-0.2.3/
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     1387 2024-04-17 10:14:57.411049 simply-log-0.2.3/PKG-INFO
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     1253 2024-04-17 10:14:48.000000 simply-log-0.2.3/README.md
+drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-04-17 10:14:57.410084 simply-log-0.2.3/log/
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)       45 2024-04-17 09:35:52.000000 simply-log-0.2.3/log/__init__.py
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     1067 2024-04-17 08:42:59.000000 simply-log-0.2.3/log/main.py
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)       38 2024-04-17 10:14:57.411230 simply-log-0.2.3/setup.cfg
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)      359 2024-04-17 10:10:21.000000 simply-log-0.2.3/setup.py
+drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-04-17 10:14:57.410858 simply-log-0.2.3/simply_log.egg-info/
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     1387 2024-04-17 10:14:57.000000 simply-log-0.2.3/simply_log.egg-info/PKG-INFO
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)      182 2024-04-17 10:14:57.000000 simply-log-0.2.3/simply_log.egg-info/SOURCES.txt
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)        1 2024-04-17 10:14:57.000000 simply-log-0.2.3/simply_log.egg-info/dependency_links.txt
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)        4 2024-04-17 10:14:57.000000 simply-log-0.2.3/simply_log.egg-info/top_level.txt
```

### Comparing `simply-log-0.2.2/PKG-INFO` & `simply-log-0.2.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,34 @@
 Metadata-Version: 2.1
 Name: simply-log
-Version: 0.2.2
+Version: 0.2.3
 Summary: A simple logging.txt library 
 Description-Content-Type: text/markdown
 
 # Text File Generation Module
 
 This Python module provides a simple logging functionality, allowing users to generate text log files.
 
+if not exist => create file.txt
+
+```
+- dir/
+___ logFile.txt
+___ logFile-1.txt
+___ logFile-2.txt
+```
+
+coontent file :
+
+```
+[17/04/2024 09:56:05] [ERROR] this is a test message error dag
+[17/04/2024 09:56:05] [INFO] this is a test info message index null
+[17/04/2024 09:56:05] [WARNING] this is a test warning message scripte.py break
+```
+
 ## Usage
 
 Once installed, you can import the module into your Python script like this:
 
 ```python
 from log import log_message
 
@@ -25,21 +42,21 @@
    ```python
    log_message("logFile", "info", "this is an informational message")
    ```
 
 2. Logging a warning message:
 
    ```python
-   log_message("logFile", "warning", "this is a warning message")
+   log_message("logFile-1", "warning", "this is a warning message")
    ```
 
 3. Logging a debug message:
 
    ```python
-   log_message("logFile", "debug", "this is a debug message")
+   log_message("logFile-2", "debug", "this is a debug message")
    ```
 
 4. Logging a critical message:
 
    ```python
    log_message("logFile", "critical", "this is a critical message")
    ```
```

### Comparing `simply-log-0.2.2/README.md` & `simply-log-0.2.3/simply_log.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,34 @@
+Metadata-Version: 2.1
+Name: simply-log
+Version: 0.2.3
+Summary: A simple logging.txt library 
+Description-Content-Type: text/markdown
+
 # Text File Generation Module
 
 This Python module provides a simple logging functionality, allowing users to generate text log files.
 
+if not exist => create file.txt
+
+```
+- dir/
+___ logFile.txt
+___ logFile-1.txt
+___ logFile-2.txt
+```
+
+coontent file :
+
+```
+[17/04/2024 09:56:05] [ERROR] this is a test message error dag
+[17/04/2024 09:56:05] [INFO] this is a test info message index null
+[17/04/2024 09:56:05] [WARNING] this is a test warning message scripte.py break
+```
+
 ## Usage
 
 Once installed, you can import the module into your Python script like this:
 
 ```python
 from log import log_message
 
@@ -19,21 +42,21 @@
    ```python
    log_message("logFile", "info", "this is an informational message")
    ```
 
 2. Logging a warning message:
 
    ```python
-   log_message("logFile", "warning", "this is a warning message")
+   log_message("logFile-1", "warning", "this is a warning message")
    ```
 
 3. Logging a debug message:
 
    ```python
-   log_message("logFile", "debug", "this is a debug message")
+   log_message("logFile-2", "debug", "this is a debug message")
    ```
 
 4. Logging a critical message:
 
    ```python
    log_message("logFile", "critical", "this is a critical message")
    ```
```

### Comparing `simply-log-0.2.2/log/main.py` & `simply-log-0.2.3/log/main.py`

 * *Files identical despite different names*

