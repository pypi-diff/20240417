# Comparing `tmp/ubitlogger-0.1.0.tar.gz` & `tmp/ubitlogger-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubitlogger-0.1.0.tar", last modified: Mon Apr 15 23:33:51 2024, max compression
+gzip compressed data, was "ubitlogger-0.2.0.tar", last modified: Wed Apr 17 14:49:36 2024, max compression
```

## Comparing `ubitlogger-0.1.0.tar` & `ubitlogger-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-15 23:33:51.053019 ubitlogger-0.1.0/
--rw-r--r--   0 pairin    (1000) pairin    (1000)     1062 2024-04-15 23:12:06.000000 ubitlogger-0.1.0/LICENSE
--rw-r--r--   0 pairin    (1000) pairin    (1000)     2102 2024-04-15 23:33:51.053019 ubitlogger-0.1.0/PKG-INFO
--rw-r--r--   0 pairin    (1000) pairin    (1000)      667 2024-04-15 23:09:25.000000 ubitlogger-0.1.0/README.md
--rw-r--r--   0 pairin    (1000) pairin    (1000)     1940 2024-04-15 22:36:23.000000 ubitlogger-0.1.0/pyproject.toml
--rw-r--r--   0 pairin    (1000) pairin    (1000)       38 2024-04-15 23:33:51.053019 ubitlogger-0.1.0/setup.cfg
--rw-r--r--   0 pairin    (1000) pairin    (1000)      529 2024-04-15 21:47:43.000000 ubitlogger-0.1.0/setup.py
-drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-15 23:33:51.053019 ubitlogger-0.1.0/src/
-drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-15 23:33:51.053019 ubitlogger-0.1.0/src/ubitlogger/
--rw-r--r--   0 pairin    (1000) pairin    (1000)     2750 2024-04-15 14:58:27.000000 ubitlogger-0.1.0/src/ubitlogger/__init__.py
-drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-15 23:33:51.053019 ubitlogger-0.1.0/src/ubitlogger.egg-info/
--rw-r--r--   0 pairin    (1000) pairin    (1000)     2102 2024-04-15 23:33:51.000000 ubitlogger-0.1.0/src/ubitlogger.egg-info/PKG-INFO
--rw-r--r--   0 pairin    (1000) pairin    (1000)      257 2024-04-15 23:33:51.000000 ubitlogger-0.1.0/src/ubitlogger.egg-info/SOURCES.txt
--rw-r--r--   0 pairin    (1000) pairin    (1000)        1 2024-04-15 23:33:51.000000 ubitlogger-0.1.0/src/ubitlogger.egg-info/dependency_links.txt
--rw-r--r--   0 pairin    (1000) pairin    (1000)      204 2024-04-15 23:33:51.000000 ubitlogger-0.1.0/src/ubitlogger.egg-info/requires.txt
--rw-r--r--   0 pairin    (1000) pairin    (1000)       11 2024-04-15 23:33:51.000000 ubitlogger-0.1.0/src/ubitlogger.egg-info/top_level.txt
+drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-17 14:49:36.340581 ubitlogger-0.2.0/
+-rw-r--r--   0 pairin    (1000) pairin    (1000)     1062 2024-04-15 23:12:06.000000 ubitlogger-0.2.0/LICENSE
+-rw-r--r--   0 pairin    (1000) pairin    (1000)     2102 2024-04-17 14:49:36.340581 ubitlogger-0.2.0/PKG-INFO
+-rw-r--r--   0 pairin    (1000) pairin    (1000)      667 2024-04-15 23:09:25.000000 ubitlogger-0.2.0/README.md
+-rw-r--r--   0 pairin    (1000) pairin    (1000)     1880 2024-04-17 14:47:44.000000 ubitlogger-0.2.0/pyproject.toml
+-rw-r--r--   0 pairin    (1000) pairin    (1000)       38 2024-04-17 14:49:36.340581 ubitlogger-0.2.0/setup.cfg
+-rw-r--r--   0 pairin    (1000) pairin    (1000)      529 2024-04-15 21:47:43.000000 ubitlogger-0.2.0/setup.py
+drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-17 14:49:36.330581 ubitlogger-0.2.0/src/
+drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-17 14:49:36.340581 ubitlogger-0.2.0/src/ubitlogger/
+-rw-r--r--   0 pairin    (1000) pairin    (1000)     2846 2024-04-17 14:47:44.000000 ubitlogger-0.2.0/src/ubitlogger/__init__.py
+-rw-r--r--   0 pairin    (1000) pairin    (1000)     1392 2024-04-17 14:27:21.000000 ubitlogger-0.2.0/src/ubitlogger/cli.py
+drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-17 14:49:36.340581 ubitlogger-0.2.0/src/ubitlogger.egg-info/
+-rw-r--r--   0 pairin    (1000) pairin    (1000)     2102 2024-04-17 14:49:36.000000 ubitlogger-0.2.0/src/ubitlogger.egg-info/PKG-INFO
+-rw-r--r--   0 pairin    (1000) pairin    (1000)      335 2024-04-17 14:49:36.000000 ubitlogger-0.2.0/src/ubitlogger.egg-info/SOURCES.txt
+-rw-r--r--   0 pairin    (1000) pairin    (1000)        1 2024-04-17 14:49:36.000000 ubitlogger-0.2.0/src/ubitlogger.egg-info/dependency_links.txt
+-rw-r--r--   0 pairin    (1000) pairin    (1000)       50 2024-04-17 14:49:36.000000 ubitlogger-0.2.0/src/ubitlogger.egg-info/entry_points.txt
+-rw-r--r--   0 pairin    (1000) pairin    (1000)      204 2024-04-17 14:49:36.000000 ubitlogger-0.2.0/src/ubitlogger.egg-info/requires.txt
+-rw-r--r--   0 pairin    (1000) pairin    (1000)       11 2024-04-17 14:49:36.000000 ubitlogger-0.2.0/src/ubitlogger.egg-info/top_level.txt
+drwxr-xr-x   0 pairin    (1000) pairin    (1000)        0 2024-04-17 14:49:36.340581 ubitlogger-0.2.0/tests/
+-rw-r--r--   0 pairin    (1000) pairin    (1000)        0 2024-04-17 14:44:36.000000 ubitlogger-0.2.0/tests/tests.py
```

### Comparing `ubitlogger-0.1.0/LICENSE` & `ubitlogger-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ubitlogger-0.1.0/PKG-INFO` & `ubitlogger-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubitlogger
-Version: 0.1.0
+Version: 0.2.0
 Summary: A micro:bit serial port logger
 Author-email: p4irin <p4irin.github.io@gmail.com>
 Project-URL: Homepage, https://github.com/p4irin/ubitlogger
 Project-URL: Bug Tracker, https://github.com/p4irin/ubitlogger/issues
 Keywords: microbit,microbit-v1,data-logger,serial-port-listener
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ubitlogger-0.1.0/README.md` & `ubitlogger-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ubitlogger-0.1.0/pyproject.toml` & `ubitlogger-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ubitlogger"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="p4irin", email="p4irin.github.io@gmail.com" },
 ]
 description = "A micro:bit serial port logger"
 readme = "README.md"
 requires-python = ">=3.8.10"
 keywords = [
@@ -45,28 +45,29 @@
   "bumpver >= 2023.1126",
   "ubitlogger[lint]",
   "ubitlogger[test]",
   "ubitlogger[package]",
 ]
 
 [project.scripts]
+ubitlogger = "ubitlogger.cli:cli"
 
 [project.urls]
 "Homepage" = "https://github.com/p4irin/ubitlogger"
 "Bug Tracker" = "https://github.com/p4irin/ubitlogger/issues"
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 
 [tool.bumpver]
-current_version = "0.1.0"
+current_version = "0.2.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 commit = true
 tag = true
 push = false
 
@@ -74,20 +75,14 @@
 "pyproject.toml" = [
   'current_version = "{version}"',
   'version = "{version}"',
 ]
 "src/ubitlogger/__init__.py" = [
   "^__version__ = '{version}'$",
 ]
-"tests/tests.py" = [
-  "^__version__ = '{version}'$",
-]
-"README.md" = [
-  " - v{version}$",
-]
 
 
 [tool.mypy]
 
 [[tool.mypy.overrides]]
 module = "serial.*"
 ignore_missing_imports = true
```

### Comparing `ubitlogger-0.1.0/setup.py` & `ubitlogger-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `ubitlogger-0.1.0/src/ubitlogger/__init__.py` & `ubitlogger-0.2.0/src/ubitlogger/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+"""
+"""
+
+__author__ = 'p4irin'
+__email__ = 'p4irin.github.io@gmail.com'
+__version__ = '0.2.0'
+
+
 from threading import Thread, Event
 from signal import signal, SIGINT, SIGTERM
 from time import sleep
 from serial import Serial
 from serial.tools.list_ports import comports
```

### Comparing `ubitlogger-0.1.0/src/ubitlogger.egg-info/PKG-INFO` & `ubitlogger-0.2.0/src/ubitlogger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ubitlogger
-Version: 0.1.0
+Version: 0.2.0
 Summary: A micro:bit serial port logger
 Author-email: p4irin <p4irin.github.io@gmail.com>
 Project-URL: Homepage, https://github.com/p4irin/ubitlogger
 Project-URL: Bug Tracker, https://github.com/p4irin/ubitlogger/issues
 Keywords: microbit,microbit-v1,data-logger,serial-port-listener
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

