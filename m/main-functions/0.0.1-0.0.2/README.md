# Comparing `tmp/main_functions-0.0.1.tar.gz` & `tmp/main_functions-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "main_functions-0.0.1.tar", last modified: Wed Apr 17 18:15:04 2024, max compression
+gzip compressed data, was "main_functions-0.0.2.tar", last modified: Wed Apr 17 18:17:08 2024, max compression
```

## Comparing `main_functions-0.0.1.tar` & `main_functions-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 bibishanpandey  (1000) bibishanpandey  (1000)        0 2024-04-17 18:15:04.419725 main_functions-0.0.1/
--rw-r--r--   0 bibishanpandey  (1000) bibishanpandey  (1000)      320 2024-04-17 18:15:04.419725 main_functions-0.0.1/PKG-INFO
-drwxr-xr-x   0 bibishanpandey  (1000) bibishanpandey  (1000)        0 2024-04-17 18:15:04.419725 main_functions-0.0.1/main_functions/
--rw-r--r--   0 bibishanpandey  (1000) bibishanpandey  (1000)        0 2024-04-17 18:04:19.000000 main_functions-0.0.1/main_functions/__init__.py
--rw-r--r--   0 bibishanpandey  (1000) bibishanpandey  (1000)      115 2024-04-17 17:55:00.000000 main_functions-0.0.1/main_functions/main_functions.py
-drwxr-xr-x   0 bibishanpandey  (1000) bibishanpandey  (1000)        0 2024-04-17 18:15:04.419725 main_functions-0.0.1/main_functions.egg-info/
--rw-r--r--   0 bibishanpandey  (1000) bibishanpandey  (1000)      320 2024-04-17 18:15:04.000000 main_functions-0.0.1/main_functions.egg-info/PKG-INFO
--rw-r--r--   0 bibishanpandey  (1000) bibishanpandey  (1000)      220 2024-04-17 18:15:04.000000 main_functions-0.0.1/main_functions.egg-info/SOURCES.txt
--rw-r--r--   0 bibishanpandey  (1000) bibishanpandey  (1000)        1 2024-04-17 18:15:04.000000 main_functions-0.0.1/main_functions.egg-info/dependency_links.txt
--rw-r--r--   0 bibishanpandey  (1000) bibishanpandey  (1000)       15 2024-04-17 18:15:04.000000 main_functions-0.0.1/main_functions.egg-info/top_level.txt
--rw-r--r--   0 bibishanpandey  (1000) bibishanpandey  (1000)       38 2024-04-17 18:15:04.419725 main_functions-0.0.1/setup.cfg
--rw-r--r--   0 bibishanpandey  (1000) bibishanpandey  (1000)      444 2024-04-17 18:14:46.000000 main_functions-0.0.1/setup.py
+drwxr-xr-x   0 bibishanpandey  (1000) bibishanpandey  (1000)        0 2024-04-17 18:17:08.065491 main_functions-0.0.2/
+-rw-r--r--   0 bibishanpandey  (1000) bibishanpandey  (1000)      320 2024-04-17 18:17:08.065491 main_functions-0.0.2/PKG-INFO
+drwxr-xr-x   0 bibishanpandey  (1000) bibishanpandey  (1000)        0 2024-04-17 18:17:08.065491 main_functions-0.0.2/main_functions/
+-rw-r--r--   0 bibishanpandey  (1000) bibishanpandey  (1000)       34 2024-04-17 18:16:55.000000 main_functions-0.0.2/main_functions/__init__.py
+-rw-r--r--   0 bibishanpandey  (1000) bibishanpandey  (1000)      115 2024-04-17 17:55:00.000000 main_functions-0.0.2/main_functions/main_functions.py
+drwxr-xr-x   0 bibishanpandey  (1000) bibishanpandey  (1000)        0 2024-04-17 18:17:08.065491 main_functions-0.0.2/main_functions.egg-info/
+-rw-r--r--   0 bibishanpandey  (1000) bibishanpandey  (1000)      320 2024-04-17 18:17:08.000000 main_functions-0.0.2/main_functions.egg-info/PKG-INFO
+-rw-r--r--   0 bibishanpandey  (1000) bibishanpandey  (1000)      220 2024-04-17 18:17:08.000000 main_functions-0.0.2/main_functions.egg-info/SOURCES.txt
+-rw-r--r--   0 bibishanpandey  (1000) bibishanpandey  (1000)        1 2024-04-17 18:17:08.000000 main_functions-0.0.2/main_functions.egg-info/dependency_links.txt
+-rw-r--r--   0 bibishanpandey  (1000) bibishanpandey  (1000)       15 2024-04-17 18:17:08.000000 main_functions-0.0.2/main_functions.egg-info/top_level.txt
+-rw-r--r--   0 bibishanpandey  (1000) bibishanpandey  (1000)       38 2024-04-17 18:17:08.065491 main_functions-0.0.2/setup.cfg
+-rw-r--r--   0 bibishanpandey  (1000) bibishanpandey  (1000)      444 2024-04-17 18:17:05.000000 main_functions-0.0.2/setup.py
```

