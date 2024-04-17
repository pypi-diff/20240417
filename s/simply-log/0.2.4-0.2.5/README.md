# Comparing `tmp/simply-log-0.2.4.tar.gz` & `tmp/simply-log-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simply-log-0.2.4.tar", last modified: Wed Apr 17 10:17:44 2024, max compression
+gzip compressed data, was "simply-log-0.2.5.tar", last modified: Wed Apr 17 10:22:46 2024, max compression
```

## Comparing `simply-log-0.2.4.tar` & `simply-log-0.2.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-04-17 10:17:44.583183 simply-log-0.2.4/
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     1387 2024-04-17 10:17:44.583047 simply-log-0.2.4/PKG-INFO
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     1253 2024-04-17 10:14:48.000000 simply-log-0.2.4/README.md
-drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-04-17 10:17:44.582286 simply-log-0.2.4/log/
--rw-r--r--   0 corneliusvincent   (501) staff       (20)       45 2024-04-17 09:35:52.000000 simply-log-0.2.4/log/__init__.py
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     1342 2024-04-17 10:17:31.000000 simply-log-0.2.4/log/main.py
--rw-r--r--   0 corneliusvincent   (501) staff       (20)       38 2024-04-17 10:17:44.583228 simply-log-0.2.4/setup.cfg
--rw-r--r--   0 corneliusvincent   (501) staff       (20)      359 2024-04-17 10:17:40.000000 simply-log-0.2.4/setup.py
-drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-04-17 10:17:44.582859 simply-log-0.2.4/simply_log.egg-info/
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     1387 2024-04-17 10:17:44.000000 simply-log-0.2.4/simply_log.egg-info/PKG-INFO
--rw-r--r--   0 corneliusvincent   (501) staff       (20)      182 2024-04-17 10:17:44.000000 simply-log-0.2.4/simply_log.egg-info/SOURCES.txt
--rw-r--r--   0 corneliusvincent   (501) staff       (20)        1 2024-04-17 10:17:44.000000 simply-log-0.2.4/simply_log.egg-info/dependency_links.txt
--rw-r--r--   0 corneliusvincent   (501) staff       (20)        4 2024-04-17 10:17:44.000000 simply-log-0.2.4/simply_log.egg-info/top_level.txt
+drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-04-17 10:22:46.980228 simply-log-0.2.5/
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     1516 2024-04-17 10:22:46.980064 simply-log-0.2.5/PKG-INFO
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     1382 2024-04-17 10:22:29.000000 simply-log-0.2.5/README.md
+drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-04-17 10:22:46.979122 simply-log-0.2.5/log/
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)       45 2024-04-17 09:35:52.000000 simply-log-0.2.5/log/__init__.py
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     1195 2024-04-17 10:21:06.000000 simply-log-0.2.5/log/main.py
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)       38 2024-04-17 10:22:46.980273 simply-log-0.2.5/setup.cfg
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)      359 2024-04-17 10:22:37.000000 simply-log-0.2.5/setup.py
+drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-04-17 10:22:46.979871 simply-log-0.2.5/simply_log.egg-info/
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     1516 2024-04-17 10:22:46.000000 simply-log-0.2.5/simply_log.egg-info/PKG-INFO
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)      182 2024-04-17 10:22:46.000000 simply-log-0.2.5/simply_log.egg-info/SOURCES.txt
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)        1 2024-04-17 10:22:46.000000 simply-log-0.2.5/simply_log.egg-info/dependency_links.txt
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)        4 2024-04-17 10:22:46.000000 simply-log-0.2.5/simply_log.egg-info/top_level.txt
```

### Comparing `simply-log-0.2.4/PKG-INFO` & `simply-log-0.2.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simply-log
-Version: 0.2.4
+Version: 0.2.5
 Summary: A simple logging.txt library 
 Description-Content-Type: text/markdown
 
 # Text File Generation Module
 
 This Python module provides a simple logging functionality, allowing users to generate text log files.
 
@@ -57,8 +57,15 @@
 
 4. Logging a critical message:
 
    ```python
    log_message("logFile", "critical", "this is a critical message")
    ```
 
+5. Auto Log:
+
+   ```python
+   log_message("auto", "debug", "this is a debug message")
+   # name file = %d%m%Y_%H%M%S.txt
+   ```
+
 [Cornelius Vincent @MIT @author ](https://www.linkedin.com/in/corneliusvincent)
```

### Comparing `simply-log-0.2.4/README.md` & `simply-log-0.2.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -51,8 +51,15 @@
 
 4. Logging a critical message:
 
    ```python
    log_message("logFile", "critical", "this is a critical message")
    ```
 
+5. Auto Log:
+
+   ```python
+   log_message("auto", "debug", "this is a debug message")
+   # name file = %d%m%Y_%H%M%S.txt
+   ```
+
 [Cornelius Vincent @MIT @author ](https://www.linkedin.com/in/corneliusvincent)
```

### Comparing `simply-log-0.2.4/log/main.py` & `simply-log-0.2.5/log/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,29 @@
 import os
 import datetime
 
 
-def log_message(filename, log_type, message):
+def log_message(filename: str, log_type: str, message: str):
     """
     Function for logging messages to a text file.
-    :param filename: Name of log file
+    :param filename: Name of log file or auto
     :param log_type: Type of log (info, error, warning, etc.)
     :param message: Message to be logged
     :return: None
 
     Example of use:
     log_message("logfile", "info", "This is an information message.")
     log_message("logfile", "error", "This is an error message.")
 
     If the file does not exist, it will be created. Otherwise, the message will be added to the end of the file.
     """
     timestamp = datetime.datetime.now().strftime("%d/%m/%Y %H:%M:%S")
+    if filename == "auto":
+        filename = f"log_{datetime.datetime.now().strftime('%d%m%Y_%H%M%S')}"
     try:
-        # Séparation du nom de fichier et du chemin du dossier
-        folder_path, file_name = os.path.split(filename)
-
-        # Création des dossiers si ils n'existent pas
-        if folder_path and not os.path.exists(folder_path):
-            os.makedirs(folder_path)
-
         if not os.path.exists(filename + ".txt"):
             with open(filename + ".txt", "w") as file:
                 file.write(f"[{timestamp}] [{log_type.upper()}] {message}\n")
         else:
             with open(filename + ".txt", "a") as file:
                 file.write(f"\n[{timestamp}] [{log_type.upper()}] {message}")
     except Exception as e:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `simply-log-0.2.4/simply_log.egg-info/PKG-INFO` & `simply-log-0.2.5/simply_log.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simply-log
-Version: 0.2.4
+Version: 0.2.5
 Summary: A simple logging.txt library 
 Description-Content-Type: text/markdown
 
 # Text File Generation Module
 
 This Python module provides a simple logging functionality, allowing users to generate text log files.
 
@@ -57,8 +57,15 @@
 
 4. Logging a critical message:
 
    ```python
    log_message("logFile", "critical", "this is a critical message")
    ```
 
+5. Auto Log:
+
+   ```python
+   log_message("auto", "debug", "this is a debug message")
+   # name file = %d%m%Y_%H%M%S.txt
+   ```
+
 [Cornelius Vincent @MIT @author ](https://www.linkedin.com/in/corneliusvincent)
```

