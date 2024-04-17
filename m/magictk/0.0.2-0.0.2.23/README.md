# Comparing `tmp/magictk-0.0.2.tar.gz` & `tmp/magictk-0.0.2.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magictk-0.0.2.tar", last modified: Tue Apr 16 22:46:18 2024, max compression
+gzip compressed data, was "magictk-0.0.2.23.tar", last modified: Wed Apr 17 14:11:12 2024, max compression
```

## Comparing `magictk-0.0.2.tar` & `magictk-0.0.2.23.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 22:46:18.841700 magictk-0.0.2/
--rw-r--r--   0 root         (0) root         (0)      272 2024-04-16 22:46:18.841700 magictk-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1376 2024-04-16 22:46:18.000000 magictk-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 22:46:18.841700 magictk-0.0.2/magictk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      272 2024-04-16 22:46:18.000000 magictk-0.0.2/magictk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      142 2024-04-16 22:46:18.000000 magictk-0.0.2/magictk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 22:46:18.000000 magictk-0.0.2/magictk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 22:46:18.000000 magictk-0.0.2/magictk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 22:46:18.841700 magictk-0.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      564 2024-04-16 22:46:18.000000 magictk-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:11:12.440415 magictk-0.0.2.23/
+-rw-r--r--   0 root         (0) root         (0)      275 2024-04-17 14:11:12.436415 magictk-0.0.2.23/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1376 2024-04-17 14:11:12.000000 magictk-0.0.2.23/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 14:11:12.436415 magictk-0.0.2.23/magictk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      275 2024-04-17 14:11:12.000000 magictk-0.0.2.23/magictk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-17 14:11:12.000000 magictk-0.0.2.23/magictk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 14:11:12.000000 magictk-0.0.2.23/magictk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-17 14:11:12.000000 magictk-0.0.2.23/magictk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 14:11:12.000000 magictk-0.0.2.23/magictk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 14:11:12.440415 magictk-0.0.2.23/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      760 2024-04-17 14:11:12.000000 magictk-0.0.2.23/setup.py
```

### Comparing `magictk-0.0.2/README.md` & `magictk-0.0.2.23/README.md`

 * *Files identical despite different names*

