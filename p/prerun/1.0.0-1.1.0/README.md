# Comparing `tmp/prerun-1.0.0.tar.gz` & `tmp/prerun-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prerun-1.0.0.tar", last modified: Tue Apr 16 07:48:41 2024, max compression
+gzip compressed data, was "prerun-1.1.0.tar", last modified: Tue Apr 16 09:04:06 2024, max compression
```

## Comparing `prerun-1.0.0.tar` & `prerun-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:48:41.524508 prerun-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-16 07:48:36.000000 prerun-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-16 07:48:41.524508 prerun-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 07:48:36.000000 prerun-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-16 07:48:36.000000 prerun-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 07:48:41.524508 prerun-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:48:41.524508 prerun-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:48:41.524508 prerun-1.0.0/src/prerun/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-16 07:48:36.000000 prerun-1.0.0/src/prerun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 07:48:36.000000 prerun-1.0.0/src/prerun/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-16 07:48:36.000000 prerun-1.0.0/src/prerun/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-16 07:48:36.000000 prerun-1.0.0/src/prerun/recv_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-16 07:48:36.000000 prerun-1.0.0/src/prerun/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-16 07:48:36.000000 prerun-1.0.0/src/prerun/sigint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:48:41.524508 prerun-1.0.0/src/prerun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-16 07:48:41.000000 prerun-1.0.0/src/prerun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-16 07:48:41.000000 prerun-1.0.0/src/prerun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 07:48:41.000000 prerun-1.0.0/src/prerun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-16 07:48:41.000000 prerun-1.0.0/src/prerun.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 07:48:41.000000 prerun-1.0.0/src/prerun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 07:48:41.000000 prerun-1.0.0/src/prerun.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:04:06.846144 prerun-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-16 09:04:01.000000 prerun-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-16 09:04:06.846144 prerun-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 09:04:01.000000 prerun-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-16 09:04:01.000000 prerun-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 09:04:06.846144 prerun-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:04:06.842143 prerun-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:04:06.842143 prerun-1.1.0/src/prerun/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-16 09:04:01.000000 prerun-1.1.0/src/prerun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-16 09:04:01.000000 prerun-1.1.0/src/prerun/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-16 09:04:01.000000 prerun-1.1.0/src/prerun/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-16 09:04:01.000000 prerun-1.1.0/src/prerun/recv_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-16 09:04:01.000000 prerun-1.1.0/src/prerun/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-16 09:04:01.000000 prerun-1.1.0/src/prerun/sigint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:04:06.846144 prerun-1.1.0/src/prerun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-16 09:04:06.000000 prerun-1.1.0/src/prerun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-16 09:04:06.000000 prerun-1.1.0/src/prerun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 09:04:06.000000 prerun-1.1.0/src/prerun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-16 09:04:06.000000 prerun-1.1.0/src/prerun.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 09:04:06.000000 prerun-1.1.0/src/prerun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 09:04:06.000000 prerun-1.1.0/src/prerun.egg-info/top_level.txt
```

### Comparing `prerun-1.0.0/LICENSE` & `prerun-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prerun-1.0.0/PKG-INFO` & `prerun-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prerun
-Version: 1.0.0
+Version: 1.1.0
 Summary: Prerun
 License: Copyright (c) <year> <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
         use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `prerun-1.0.0/pyproject.toml` & `prerun-1.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "prerun"
-version = "1.0.0"
+version = "1.1.0"
 description = "Prerun"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 keywords = ["development"]
 classifiers = [
   "Development Status :: 3 - Alpha",
```

### Comparing `prerun-1.0.0/src/prerun/__init__.py` & `prerun-1.1.0/src/prerun/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 import sys
 
 from .client import client
 from .server import server
 
+SAVED = {}
+
 
 def main():
     if len(sys.argv) >= 2 and sys.argv[1] == "--help":
         print("Start server:\n\t-s <PRELOADER> [NUM_PROCESSES]\n\nRun Python program:\n\t[FILE [ARG...]]\n")
         return 0
 
     if len(sys.argv) < 2 or sys.argv[1] != "-s":
```

### Comparing `prerun-1.0.0/src/prerun/client.py` & `prerun-1.1.0/src/prerun/client.py`

 * *Files identical despite different names*

### Comparing `prerun-1.0.0/src/prerun/server.py` & `prerun-1.1.0/src/prerun/server.py`

 * *Files identical despite different names*

### Comparing `prerun-1.0.0/src/prerun/sigint.py` & `prerun-1.1.0/src/prerun/sigint.py`

 * *Files identical despite different names*

### Comparing `prerun-1.0.0/src/prerun.egg-info/PKG-INFO` & `prerun-1.1.0/src/prerun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prerun
-Version: 1.0.0
+Version: 1.1.0
 Summary: Prerun
 License: Copyright (c) <year> <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
         use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

