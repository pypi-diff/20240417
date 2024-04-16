# Comparing `tmp/magictk-0.0.1.tar.gz` & `tmp/magictk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magictk-0.0.1.tar", last modified: Tue Apr 16 14:14:56 2024, max compression
+gzip compressed data, was "magictk-0.0.2.tar", last modified: Tue Apr 16 22:46:18 2024, max compression
```

## Comparing `magictk-0.0.1.tar` & `magictk-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,10 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-16 14:14:56.014756 magictk-0.0.1/
--rwxrwxrwx   0 root         (0) root         (0)    17337 2024-03-24 10:22:26.000000 magictk-0.0.1/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      255 2024-04-16 14:14:56.012201 magictk-0.0.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1376 2024-04-15 13:11:06.000000 magictk-0.0.1/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-16 14:14:56.010777 magictk-0.0.1/magictk.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      255 2024-04-16 14:14:55.000000 magictk-0.0.1/magictk.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      150 2024-04-16 14:14:55.000000 magictk-0.0.1/magictk.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-16 14:14:55.000000 magictk-0.0.1/magictk.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-16 14:14:55.000000 magictk-0.0.1/magictk.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-16 14:14:56.014942 magictk-0.0.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      564 2024-04-15 13:40:45.000000 magictk-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 22:46:18.841700 magictk-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)      272 2024-04-16 22:46:18.841700 magictk-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1376 2024-04-16 22:46:18.000000 magictk-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 22:46:18.841700 magictk-0.0.2/magictk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      272 2024-04-16 22:46:18.000000 magictk-0.0.2/magictk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      142 2024-04-16 22:46:18.000000 magictk-0.0.2/magictk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 22:46:18.000000 magictk-0.0.2/magictk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 22:46:18.000000 magictk-0.0.2/magictk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 22:46:18.841700 magictk-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      564 2024-04-16 22:46:18.000000 magictk-0.0.2/setup.py
```

### Comparing `magictk-0.0.1/README.md` & `magictk-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `magictk-0.0.1/setup.py` & `magictk-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 from setuptools import setup, find_packages
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 pywin32_need = ([] if sys.platform.startswith("linux") else ["pywin32"])
 setup(
     name="magictk",
     version=VERSION,
     packages=(
         find_packages(where="./magictk")
     ),
```

