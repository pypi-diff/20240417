# Comparing `tmp/simply-log-0.2.3.tar.gz` & `tmp/simply-log-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simply-log-0.2.3.tar", last modified: Wed Apr 17 10:14:57 2024, max compression
+gzip compressed data, was "simply-log-0.2.4.tar", last modified: Wed Apr 17 10:17:44 2024, max compression
```

## Comparing `simply-log-0.2.3.tar` & `simply-log-0.2.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-04-17 10:14:57.411185 simply-log-0.2.3/
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     1387 2024-04-17 10:14:57.411049 simply-log-0.2.3/PKG-INFO
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     1253 2024-04-17 10:14:48.000000 simply-log-0.2.3/README.md
-drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-04-17 10:14:57.410084 simply-log-0.2.3/log/
--rw-r--r--   0 corneliusvincent   (501) staff       (20)       45 2024-04-17 09:35:52.000000 simply-log-0.2.3/log/__init__.py
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     1067 2024-04-17 08:42:59.000000 simply-log-0.2.3/log/main.py
--rw-r--r--   0 corneliusvincent   (501) staff       (20)       38 2024-04-17 10:14:57.411230 simply-log-0.2.3/setup.cfg
--rw-r--r--   0 corneliusvincent   (501) staff       (20)      359 2024-04-17 10:10:21.000000 simply-log-0.2.3/setup.py
-drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-04-17 10:14:57.410858 simply-log-0.2.3/simply_log.egg-info/
--rw-r--r--   0 corneliusvincent   (501) staff       (20)     1387 2024-04-17 10:14:57.000000 simply-log-0.2.3/simply_log.egg-info/PKG-INFO
--rw-r--r--   0 corneliusvincent   (501) staff       (20)      182 2024-04-17 10:14:57.000000 simply-log-0.2.3/simply_log.egg-info/SOURCES.txt
--rw-r--r--   0 corneliusvincent   (501) staff       (20)        1 2024-04-17 10:14:57.000000 simply-log-0.2.3/simply_log.egg-info/dependency_links.txt
--rw-r--r--   0 corneliusvincent   (501) staff       (20)        4 2024-04-17 10:14:57.000000 simply-log-0.2.3/simply_log.egg-info/top_level.txt
+drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-04-17 10:17:44.583183 simply-log-0.2.4/
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     1387 2024-04-17 10:17:44.583047 simply-log-0.2.4/PKG-INFO
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     1253 2024-04-17 10:14:48.000000 simply-log-0.2.4/README.md
+drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-04-17 10:17:44.582286 simply-log-0.2.4/log/
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)       45 2024-04-17 09:35:52.000000 simply-log-0.2.4/log/__init__.py
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     1342 2024-04-17 10:17:31.000000 simply-log-0.2.4/log/main.py
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)       38 2024-04-17 10:17:44.583228 simply-log-0.2.4/setup.cfg
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)      359 2024-04-17 10:17:40.000000 simply-log-0.2.4/setup.py
+drwxr-xr-x   0 corneliusvincent   (501) staff       (20)        0 2024-04-17 10:17:44.582859 simply-log-0.2.4/simply_log.egg-info/
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)     1387 2024-04-17 10:17:44.000000 simply-log-0.2.4/simply_log.egg-info/PKG-INFO
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)      182 2024-04-17 10:17:44.000000 simply-log-0.2.4/simply_log.egg-info/SOURCES.txt
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)        1 2024-04-17 10:17:44.000000 simply-log-0.2.4/simply_log.egg-info/dependency_links.txt
+-rw-r--r--   0 corneliusvincent   (501) staff       (20)        4 2024-04-17 10:17:44.000000 simply-log-0.2.4/simply_log.egg-info/top_level.txt
```

### Comparing `simply-log-0.2.3/PKG-INFO` & `simply-log-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simply-log
-Version: 0.2.3
+Version: 0.2.4
 Summary: A simple logging.txt library 
 Description-Content-Type: text/markdown
 
 # Text File Generation Module
 
 This Python module provides a simple logging functionality, allowing users to generate text log files.
```

### Comparing `simply-log-0.2.3/README.md` & `simply-log-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `simply-log-0.2.3/log/main.py` & `simply-log-0.2.4/log/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,21 @@
     log_message("logfile", "info", "This is an information message.")
     log_message("logfile", "error", "This is an error message.")
 
     If the file does not exist, it will be created. Otherwise, the message will be added to the end of the file.
     """
     timestamp = datetime.datetime.now().strftime("%d/%m/%Y %H:%M:%S")
     try:
+        # Séparation du nom de fichier et du chemin du dossier
+        folder_path, file_name = os.path.split(filename)
+
+        # Création des dossiers si ils n'existent pas
+        if folder_path and not os.path.exists(folder_path):
+            os.makedirs(folder_path)
+
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
-us-ascii
+utf-8
```

### Comparing `simply-log-0.2.3/simply_log.egg-info/PKG-INFO` & `simply-log-0.2.4/simply_log.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simply-log
-Version: 0.2.3
+Version: 0.2.4
 Summary: A simple logging.txt library 
 Description-Content-Type: text/markdown
 
 # Text File Generation Module
 
 This Python module provides a simple logging functionality, allowing users to generate text log files.
```

