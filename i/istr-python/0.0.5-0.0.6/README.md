# Comparing `tmp/istr_python-0.0.5.tar.gz` & `tmp/istr_python-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "istr_python-0.0.5.tar", last modified: Wed Apr 17 09:26:23 2024, max compression
+gzip compressed data, was "istr_python-0.0.6.tar", last modified: Wed Apr 17 15:02:27 2024, max compression
```

## Comparing `istr_python-0.0.5.tar` & `istr_python-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 09:26:23.304048 istr_python-0.0.5/
--rw-rw-rw-   0        0        0     4153 2024-04-17 09:26:23.302907 istr_python-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3724 2024-04-17 07:17:19.000000 istr_python-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 09:26:23.290836 istr_python-0.0.5/istr/
--rw-rw-rw-   0        0        0       19 2024-04-13 09:15:49.000000 istr_python-0.0.5/istr/__init__.py
--rw-rw-rw-   0        0        0     7734 2024-04-14 16:04:53.000000 istr_python-0.0.5/istr/install istr.py
--rw-rw-rw-   0        0        0    12604 2024-04-17 07:46:55.000000 istr_python-0.0.5/istr/istr.py
-drwxrwxrwx   0        0        0        0 2024-04-17 09:26:23.301906 istr_python-0.0.5/istr_python.egg-info/
--rw-rw-rw-   0        0        0     4153 2024-04-17 09:26:23.000000 istr_python-0.0.5/istr_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2024-04-17 09:26:23.000000 istr_python-0.0.5/istr_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 09:26:23.000000 istr_python-0.0.5/istr_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-17 09:26:23.000000 istr_python-0.0.5/istr_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      353 2024-04-17 09:26:05.000000 istr_python-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-17 09:26:23.304048 istr_python-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-17 09:26:23.299903 istr_python-0.0.5/tests/
--rw-rw-rw-   0        0        0     9682 2024-04-17 07:00:43.000000 istr_python-0.0.5/tests/test_istr.py
+drwxrwxrwx   0        0        0        0 2024-04-17 15:02:27.510317 istr_python-0.0.6/
+-rw-rw-rw-   0        0        0     4153 2024-04-17 15:02:27.510317 istr_python-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3724 2024-04-17 07:17:19.000000 istr_python-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 15:02:27.476216 istr_python-0.0.6/istr/
+-rw-rw-rw-   0        0        0       50 2024-04-17 12:23:20.000000 istr_python-0.0.6/istr/__init__.py
+-rw-rw-rw-   0        0        0     7734 2024-04-14 16:04:53.000000 istr_python-0.0.6/istr/install istr.py
+-rw-rw-rw-   0        0        0    12753 2024-04-17 12:29:37.000000 istr_python-0.0.6/istr/istr.py
+drwxrwxrwx   0        0        0        0 2024-04-17 15:02:27.510317 istr_python-0.0.6/istr_python.egg-info/
+-rw-rw-rw-   0        0        0     4153 2024-04-17 15:02:27.000000 istr_python-0.0.6/istr_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2024-04-17 15:02:27.000000 istr_python-0.0.6/istr_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 15:02:27.000000 istr_python-0.0.6/istr_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-17 15:02:27.000000 istr_python-0.0.6/istr_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      368 2024-04-17 15:02:20.000000 istr_python-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-17 15:02:27.515329 istr_python-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 15:02:27.508235 istr_python-0.0.6/tests/
+-rw-rw-rw-   0        0        0     9682 2024-04-17 07:00:43.000000 istr_python-0.0.6/tests/test_istr.py
```

### Comparing `istr_python-0.0.5/PKG-INFO` & `istr_python-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: istr-python
-Version: 0.0.5
+Version: 0.0.6
 Summary: istr is a module to use strings as if they were integers.
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Introduction
```

### Comparing `istr_python-0.0.5/README.md` & `istr_python-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `istr_python-0.0.5/istr/install istr.py` & `istr_python-0.0.6/istr/install istr.py`

 * *Files identical despite different names*

### Comparing `istr_python-0.0.5/istr/istr.py` & `istr_python-0.0.6/istr/istr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 from functools import partial
 import math
 import contextlib
 
+#   _       _
+#  (_) ___ | |_  _ __
+#  | |/ __|| __|| '__|
+#  | |\__ \| |_ | |
+#  |_||___/ \__||_|    use strings as integers
+
+__version__ = "0.0.6"
 
 class istr(str):
     """
     istr object
 
     Parameters
     ----------
```

### Comparing `istr_python-0.0.5/istr_python.egg-info/PKG-INFO` & `istr_python-0.0.6/istr_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: istr-python
-Version: 0.0.5
+Version: 0.0.6
 Summary: istr is a module to use strings as if they were integers.
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Introduction
```

### Comparing `istr_python-0.0.5/tests/test_istr.py` & `istr_python-0.0.6/tests/test_istr.py`

 * *Files identical despite different names*

