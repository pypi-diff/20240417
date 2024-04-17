# Comparing `tmp/lvm_read_comma-1.30.tar.gz` & `tmp/lvm_read_comma-1.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lvm_read_comma-1.30.tar", last modified: Wed Apr 17 12:15:55 2024, max compression
+gzip compressed data, was "lvm_read_comma-1.31.tar", last modified: Wed Apr 17 12:25:31 2024, max compression
```

## Comparing `lvm_read_comma-1.30.tar` & `lvm_read_comma-1.31.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 professor  (1000) users      (984)        0 2024-04-17 12:15:55.740619 lvm_read_comma-1.30/
--rw-r--r--   0 professor  (1000) users      (984)     1070 2024-04-17 04:21:15.000000 lvm_read_comma-1.30/LICENSE
--rw-r--r--   0 professor  (1000) users      (984)      478 2024-04-17 12:15:55.740619 lvm_read_comma-1.30/PKG-INFO
-drwxr-xr-x   0 professor  (1000) users      (984)        0 2024-04-17 12:15:55.740619 lvm_read_comma-1.30/lvm_read_comma.egg-info/
--rw-r--r--   0 professor  (1000) users      (984)      478 2024-04-17 12:15:55.000000 lvm_read_comma-1.30/lvm_read_comma.egg-info/PKG-INFO
--rw-r--r--   0 professor  (1000) users      (984)      223 2024-04-17 12:15:55.000000 lvm_read_comma-1.30/lvm_read_comma.egg-info/SOURCES.txt
--rw-r--r--   0 professor  (1000) users      (984)        1 2024-04-17 12:15:55.000000 lvm_read_comma-1.30/lvm_read_comma.egg-info/dependency_links.txt
--rw-r--r--   0 professor  (1000) users      (984)        6 2024-04-17 12:15:55.000000 lvm_read_comma-1.30/lvm_read_comma.egg-info/requires.txt
--rw-r--r--   0 professor  (1000) users      (984)       15 2024-04-17 12:15:55.000000 lvm_read_comma-1.30/lvm_read_comma.egg-info/top_level.txt
--rw-r--r--   0 professor  (1000) users      (984)       38 2024-04-17 12:15:55.740619 lvm_read_comma-1.30/setup.cfg
--rw-r--r--   0 professor  (1000) users      (984)      719 2024-04-17 12:03:52.000000 lvm_read_comma-1.30/setup.py
-drwxr-xr-x   0 professor  (1000) users      (984)        0 2024-04-17 12:15:55.740619 lvm_read_comma-1.30/tests/
--rw-r--r--   0 professor  (1000) users      (984)     2013 2024-04-17 07:37:39.000000 lvm_read_comma-1.30/tests/test_all.py
+drwxr-xr-x   0 professor  (1000) users      (984)        0 2024-04-17 12:25:31.005226 lvm_read_comma-1.31/
+-rw-r--r--   0 professor  (1000) users      (984)     1070 2024-04-17 04:21:15.000000 lvm_read_comma-1.31/LICENSE
+-rw-r--r--   0 professor  (1000) users      (984)     1073 2024-04-17 12:25:31.005226 lvm_read_comma-1.31/PKG-INFO
+drwxr-xr-x   0 professor  (1000) users      (984)        0 2024-04-17 12:25:31.005226 lvm_read_comma-1.31/lvm_read_comma.egg-info/
+-rw-r--r--   0 professor  (1000) users      (984)     1073 2024-04-17 12:25:31.000000 lvm_read_comma-1.31/lvm_read_comma.egg-info/PKG-INFO
+-rw-r--r--   0 professor  (1000) users      (984)      212 2024-04-17 12:25:31.000000 lvm_read_comma-1.31/lvm_read_comma.egg-info/SOURCES.txt
+-rw-r--r--   0 professor  (1000) users      (984)        1 2024-04-17 12:25:31.000000 lvm_read_comma-1.31/lvm_read_comma.egg-info/dependency_links.txt
+-rw-r--r--   0 professor  (1000) users      (984)       15 2024-04-17 12:25:31.000000 lvm_read_comma-1.31/lvm_read_comma.egg-info/top_level.txt
+-rw-r--r--   0 professor  (1000) users      (984)      503 2024-04-17 12:25:10.000000 lvm_read_comma-1.31/pyproject.toml
+-rw-r--r--   0 professor  (1000) users      (984)      475 2024-04-17 04:21:15.000000 lvm_read_comma-1.31/readme.rst
+-rw-r--r--   0 professor  (1000) users      (984)       38 2024-04-17 12:25:31.005226 lvm_read_comma-1.31/setup.cfg
+-rw-r--r--   0 professor  (1000) users      (984)      719 2024-04-17 12:03:52.000000 lvm_read_comma-1.31/setup.py
+drwxr-xr-x   0 professor  (1000) users      (984)        0 2024-04-17 12:25:31.005226 lvm_read_comma-1.31/tests/
+-rw-r--r--   0 professor  (1000) users      (984)     2013 2024-04-17 07:37:39.000000 lvm_read_comma-1.31/tests/test_all.py
```

### Comparing `lvm_read_comma-1.30/LICENSE` & `lvm_read_comma-1.31/LICENSE`

 * *Files identical despite different names*

### Comparing `lvm_read_comma-1.30/setup.py` & `lvm_read_comma-1.31/setup.py`

 * *Files identical despite different names*

### Comparing `lvm_read_comma-1.30/tests/test_all.py` & `lvm_read_comma-1.31/tests/test_all.py`

 * *Files identical despite different names*

