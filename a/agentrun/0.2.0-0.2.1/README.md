# Comparing `tmp/agentrun-0.2.0.tar.gz` & `tmp/agentrun-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentrun-0.2.0.tar", last modified: Wed Apr 17 02:15:23 2024, max compression
+gzip compressed data, was "agentrun-0.2.1.tar", last modified: Wed Apr 17 02:27:32 2024, max compression
```

## Comparing `agentrun-0.2.0.tar` & `agentrun-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:15:23.533288 agentrun-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-04-17 02:15:17.000000 agentrun-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15754 2024-04-17 02:15:23.533288 agentrun-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14680 2024-04-17 02:15:17.000000 agentrun-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:15:23.529288 agentrun-0.2.0/agentrun/
--rw-r--r--   0 runner    (1001) docker     (127)    17208 2024-04-17 02:15:17.000000 agentrun-0.2.0/agentrun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:15:23.533288 agentrun-0.2.0/agentrun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15754 2024-04-17 02:15:23.000000 agentrun-0.2.0/agentrun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-17 02:15:23.000000 agentrun-0.2.0/agentrun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 02:15:23.000000 agentrun-0.2.0/agentrun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-17 02:15:23.000000 agentrun-0.2.0/agentrun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 02:15:23.000000 agentrun-0.2.0/agentrun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-17 02:15:17.000000 agentrun-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 02:15:23.533288 agentrun-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:15:23.533288 agentrun-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10382 2024-04-17 02:15:17.000000 agentrun-0.2.0/tests/test_agentrun.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:27:32.794897 agentrun-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-04-17 02:27:26.000000 agentrun-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15754 2024-04-17 02:27:32.794897 agentrun-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14680 2024-04-17 02:27:26.000000 agentrun-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:27:32.790897 agentrun-0.2.1/agentrun/
+-rw-r--r--   0 runner    (1001) docker     (127)    17208 2024-04-17 02:27:26.000000 agentrun-0.2.1/agentrun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:27:32.794897 agentrun-0.2.1/agentrun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15754 2024-04-17 02:27:32.000000 agentrun-0.2.1/agentrun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-17 02:27:32.000000 agentrun-0.2.1/agentrun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 02:27:32.000000 agentrun-0.2.1/agentrun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-17 02:27:32.000000 agentrun-0.2.1/agentrun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 02:27:32.000000 agentrun-0.2.1/agentrun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-17 02:27:26.000000 agentrun-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 02:27:32.794897 agentrun-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:27:32.794897 agentrun-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10382 2024-04-17 02:27:26.000000 agentrun-0.2.1/tests/test_agentrun.py
```

### Comparing `agentrun-0.2.0/LICENSE` & `agentrun-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `agentrun-0.2.0/PKG-INFO` & `agentrun-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentrun
-Version: 0.2.0
+Version: 0.2.1
 Summary: The easiest way to run AI or user generated python code safely in a docker container
 Author-email: Jonathan Adly <gadly0123@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/jonathan-adly/agentrun
 Project-URL: Changelog, https://github.com/jonathan-adly/agentrun/releases
 Project-URL: Issues, https://github.com/jonathan-adly/agentrun/issues
 Project-URL: CI, https://github.com/jonathan-adly/agentrun/actions
```

### Comparing `agentrun-0.2.0/README.md` & `agentrun-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `agentrun-0.2.0/agentrun/__init__.py` & `agentrun-0.2.1/agentrun/__init__.py`

 * *Files identical despite different names*

### Comparing `agentrun-0.2.0/agentrun.egg-info/PKG-INFO` & `agentrun-0.2.1/agentrun.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentrun
-Version: 0.2.0
+Version: 0.2.1
 Summary: The easiest way to run AI or user generated python code safely in a docker container
 Author-email: Jonathan Adly <gadly0123@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/jonathan-adly/agentrun
 Project-URL: Changelog, https://github.com/jonathan-adly/agentrun/releases
 Project-URL: Issues, https://github.com/jonathan-adly/agentrun/issues
 Project-URL: CI, https://github.com/jonathan-adly/agentrun/actions
```

### Comparing `agentrun-0.2.0/pyproject.toml` & `agentrun-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "agentrun"
-version = "v0.2.0"
+version = "v0.2.1"
 description = "The easiest way to run AI or user generated python code safely in a docker container"
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [{name = "Jonathan Adly", email = "gadly0123@gmail.com"}]
 license = {text = "Apache-2.0"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
```

### Comparing `agentrun-0.2.0/tests/test_agentrun.py` & `agentrun-0.2.1/tests/test_agentrun.py`

 * *Files identical despite different names*

