# Comparing `tmp/maths_operations_package-0.1.tar.gz` & `tmp/maths_operations_package-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maths_operations_package-0.1.tar", last modified: Wed Apr 17 15:43:38 2024, max compression
+gzip compressed data, was "maths_operations_package-0.2.tar", last modified: Wed Apr 17 16:40:06 2024, max compression
```

## Comparing `maths_operations_package-0.1.tar` & `maths_operations_package-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 snigdha   (1000) snigdha   (1000)        0 2024-04-17 15:43:38.254536 maths_operations_package-0.1/
--rw-r--r--   0 snigdha   (1000) snigdha   (1000)      277 2024-04-17 15:43:38.254536 maths_operations_package-0.1/PKG-INFO
-drwxr-xr-x   0 snigdha   (1000) snigdha   (1000)        0 2024-04-17 15:43:38.254536 maths_operations_package-0.1/maths_operations/
--rw-r--r--   0 snigdha   (1000) snigdha   (1000)        0 2024-04-17 15:08:00.000000 maths_operations_package-0.1/maths_operations/__init__.py
--rw-r--r--   0 snigdha   (1000) snigdha   (1000)      423 2024-04-17 15:38:56.000000 maths_operations_package-0.1/maths_operations/maths_operations.py
-drwxr-xr-x   0 snigdha   (1000) snigdha   (1000)        0 2024-04-17 15:43:38.254536 maths_operations_package-0.1/maths_operations_package.egg-info/
--rw-r--r--   0 snigdha   (1000) snigdha   (1000)      277 2024-04-17 15:43:38.000000 maths_operations_package-0.1/maths_operations_package.egg-info/PKG-INFO
--rw-r--r--   0 snigdha   (1000) snigdha   (1000)      266 2024-04-17 15:43:38.000000 maths_operations_package-0.1/maths_operations_package.egg-info/SOURCES.txt
--rw-r--r--   0 snigdha   (1000) snigdha   (1000)        1 2024-04-17 15:43:38.000000 maths_operations_package-0.1/maths_operations_package.egg-info/dependency_links.txt
--rw-r--r--   0 snigdha   (1000) snigdha   (1000)       17 2024-04-17 15:43:38.000000 maths_operations_package-0.1/maths_operations_package.egg-info/top_level.txt
--rw-r--r--   0 snigdha   (1000) snigdha   (1000)       38 2024-04-17 15:43:38.254536 maths_operations_package-0.1/setup.cfg
--rw-r--r--   0 snigdha   (1000) snigdha   (1000)      367 2024-04-17 15:43:27.000000 maths_operations_package-0.1/setup.py
+drwxr-xr-x   0 snigdha   (1000) snigdha   (1000)        0 2024-04-17 16:40:06.335219 maths_operations_package-0.2/
+-rw-r--r--   0 snigdha   (1000) snigdha   (1000)      277 2024-04-17 16:40:06.335219 maths_operations_package-0.2/PKG-INFO
+drwxr-xr-x   0 snigdha   (1000) snigdha   (1000)        0 2024-04-17 16:40:06.335219 maths_operations_package-0.2/maths_operations/
+-rw-r--r--   0 snigdha   (1000) snigdha   (1000)        0 2024-04-17 15:08:00.000000 maths_operations_package-0.2/maths_operations/__init__.py
+-rw-r--r--   0 snigdha   (1000) snigdha   (1000)      395 2024-04-17 16:38:04.000000 maths_operations_package-0.2/maths_operations/maths_operations.py
+drwxr-xr-x   0 snigdha   (1000) snigdha   (1000)        0 2024-04-17 16:40:06.335219 maths_operations_package-0.2/maths_operations_package.egg-info/
+-rw-r--r--   0 snigdha   (1000) snigdha   (1000)      277 2024-04-17 16:40:06.000000 maths_operations_package-0.2/maths_operations_package.egg-info/PKG-INFO
+-rw-r--r--   0 snigdha   (1000) snigdha   (1000)      266 2024-04-17 16:40:06.000000 maths_operations_package-0.2/maths_operations_package.egg-info/SOURCES.txt
+-rw-r--r--   0 snigdha   (1000) snigdha   (1000)        1 2024-04-17 16:40:06.000000 maths_operations_package-0.2/maths_operations_package.egg-info/dependency_links.txt
+-rw-r--r--   0 snigdha   (1000) snigdha   (1000)       17 2024-04-17 16:40:06.000000 maths_operations_package-0.2/maths_operations_package.egg-info/top_level.txt
+-rw-r--r--   0 snigdha   (1000) snigdha   (1000)       38 2024-04-17 16:40:06.335219 maths_operations_package-0.2/setup.cfg
+-rw-r--r--   0 snigdha   (1000) snigdha   (1000)      367 2024-04-17 16:39:19.000000 maths_operations_package-0.2/setup.py
```

