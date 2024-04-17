# Comparing `tmp/ALASutils-0.0.1.tar.gz` & `tmp/alasutils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ALASutils-0.0.1.tar", last modified: Sun Mar  3 02:43:54 2024, max compression
+gzip compressed data, was "alasutils-0.0.2.tar", last modified: Wed Apr 17 15:03:03 2024, max compression
```

## Comparing `ALASutils-0.0.1.tar` & `alasutils-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 jpcalderon  (1005) jpcalderon  (1005)        0 2024-03-03 02:43:54.108215 ALASutils-0.0.1/
-drwxr-xr-x   0 jpcalderon  (1005) jpcalderon  (1005)        0 2024-03-03 02:43:54.108215 ALASutils-0.0.1/ALASutils.egg-info/
--rw-r--r--   0 jpcalderon  (1005) jpcalderon  (1005)      314 2024-03-03 02:43:54.000000 ALASutils-0.0.1/ALASutils.egg-info/PKG-INFO
--rw-r--r--   0 jpcalderon  (1005) jpcalderon  (1005)      140 2024-03-03 02:43:54.000000 ALASutils-0.0.1/ALASutils.egg-info/SOURCES.txt
--rw-r--r--   0 jpcalderon  (1005) jpcalderon  (1005)        1 2024-03-03 02:43:54.000000 ALASutils-0.0.1/ALASutils.egg-info/dependency_links.txt
--rw-r--r--   0 jpcalderon  (1005) jpcalderon  (1005)        1 2024-03-03 02:43:54.000000 ALASutils-0.0.1/ALASutils.egg-info/top_level.txt
--rw-r--r--   0 jpcalderon  (1005) jpcalderon  (1005)      314 2024-03-03 02:43:54.108215 ALASutils-0.0.1/PKG-INFO
--rw-r--r--   0 jpcalderon  (1005) jpcalderon  (1005)       38 2024-03-03 02:43:54.108215 ALASutils-0.0.1/setup.cfg
--rw-r--r--   0 jpcalderon  (1005) jpcalderon  (1005)      376 2024-03-03 02:43:16.000000 ALASutils-0.0.1/setup.py
+drwxr-xr-x   0 jpcalderon  (1036) users      (100)        0 2024-04-17 15:03:03.733784 alasutils-0.0.2/
+drwxr-xr-x   0 jpcalderon  (1036) users      (100)        0 2024-04-17 15:03:03.733784 alasutils-0.0.2/ALASutils.egg-info/
+-rw-r--r--   0 jpcalderon  (1036) users      (100)      314 2024-04-17 15:03:03.000000 alasutils-0.0.2/ALASutils.egg-info/PKG-INFO
+-rw-r--r--   0 jpcalderon  (1036) users      (100)      140 2024-04-17 15:03:03.000000 alasutils-0.0.2/ALASutils.egg-info/SOURCES.txt
+-rw-r--r--   0 jpcalderon  (1036) users      (100)        1 2024-04-17 15:03:03.000000 alasutils-0.0.2/ALASutils.egg-info/dependency_links.txt
+-rw-r--r--   0 jpcalderon  (1036) users      (100)        1 2024-04-17 15:03:03.000000 alasutils-0.0.2/ALASutils.egg-info/top_level.txt
+-rw-r--r--   0 jpcalderon  (1036) users      (100)      314 2024-04-17 15:03:03.733784 alasutils-0.0.2/PKG-INFO
+-rw-r--r--   0 jpcalderon  (1036) users      (100)       38 2024-04-17 15:03:03.733784 alasutils-0.0.2/setup.cfg
+-rw-r--r--   0 jpcalderon  (1036) users      (100)      377 2024-04-17 15:02:58.000000 alasutils-0.0.2/setup.py
```

