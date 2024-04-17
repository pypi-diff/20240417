# Comparing `tmp/connpy-4.0.0b1.tar.gz` & `tmp/connpy-4.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connpy-4.0.0b1.tar", last modified: Wed Apr 17 19:29:52 2024, max compression
+gzip compressed data, was "connpy-4.0.0b2.tar", last modified: Wed Apr 17 20:09:34 2024, max compression
```

## Comparing `connpy-4.0.0b1.tar` & `connpy-4.0.0b2.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:29:52.115888 connpy-4.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-17 19:29:47.000000 connpy-4.0.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12164 2024-04-17 19:29:52.115888 connpy-4.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11054 2024-04-17 19:29:47.000000 connpy-4.0.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:29:52.115888 connpy-4.0.0b1/connpy/
--rw-r--r--   0 runner    (1001) docker     (127)    10798 2024-04-17 19:29:47.000000 connpy-4.0.0b1/connpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-17 19:29:47.000000 connpy-4.0.0b1/connpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-17 19:29:47.000000 connpy-4.0.0b1/connpy/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24698 2024-04-17 19:29:47.000000 connpy-4.0.0b1/connpy/ai.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5102 2024-04-17 19:29:47.000000 connpy-4.0.0b1/connpy/api.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7896 2024-04-17 19:29:47.000000 connpy-4.0.0b1/connpy/completion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16208 2024-04-17 19:29:47.000000 connpy-4.0.0b1/connpy/configfile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    74522 2024-04-17 19:29:47.000000 connpy-4.0.0b1/connpy/connapp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    32826 2024-04-17 19:29:47.000000 connpy-4.0.0b1/connpy/core.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1572 2024-04-17 19:29:47.000000 connpy-4.0.0b1/connpy/hooks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7133 2024-04-17 19:29:47.000000 connpy-4.0.0b1/connpy/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:29:52.115888 connpy-4.0.0b1/connpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12164 2024-04-17 19:29:52.000000 connpy-4.0.0b1/connpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-17 19:29:52.000000 connpy-4.0.0b1/connpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 19:29:52.000000 connpy-4.0.0b1/connpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-17 19:29:52.000000 connpy-4.0.0b1/connpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-17 19:29:52.000000 connpy-4.0.0b1/connpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 19:29:52.000000 connpy-4.0.0b1/connpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-17 19:29:52.115888 connpy-4.0.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-17 19:29:47.000000 connpy-4.0.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:09:34.909044 connpy-4.0.0b2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-17 20:09:29.000000 connpy-4.0.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12164 2024-04-17 20:09:34.909044 connpy-4.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11054 2024-04-17 20:09:29.000000 connpy-4.0.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:09:34.905044 connpy-4.0.0b2/connpy/
+-rw-r--r--   0 runner    (1001) docker     (127)    10798 2024-04-17 20:09:29.000000 connpy-4.0.0b2/connpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-17 20:09:29.000000 connpy-4.0.0b2/connpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-17 20:09:29.000000 connpy-4.0.0b2/connpy/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24698 2024-04-17 20:09:29.000000 connpy-4.0.0b2/connpy/ai.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5102 2024-04-17 20:09:29.000000 connpy-4.0.0b2/connpy/api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7896 2024-04-17 20:09:29.000000 connpy-4.0.0b2/connpy/completion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16208 2024-04-17 20:09:29.000000 connpy-4.0.0b2/connpy/configfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    74522 2024-04-17 20:09:29.000000 connpy-4.0.0b2/connpy/connapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    32826 2024-04-17 20:09:29.000000 connpy-4.0.0b2/connpy/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:09:34.905044 connpy-4.0.0b2/connpy/core_plugins/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16380 2024-04-17 20:09:29.000000 connpy-4.0.0b2/connpy/core_plugins/sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1572 2024-04-17 20:09:29.000000 connpy-4.0.0b2/connpy/hooks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7133 2024-04-17 20:09:29.000000 connpy-4.0.0b2/connpy/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:09:34.905044 connpy-4.0.0b2/connpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12164 2024-04-17 20:09:34.000000 connpy-4.0.0b2/connpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-17 20:09:34.000000 connpy-4.0.0b2/connpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 20:09:34.000000 connpy-4.0.0b2/connpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-17 20:09:34.000000 connpy-4.0.0b2/connpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-17 20:09:34.000000 connpy-4.0.0b2/connpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 20:09:34.000000 connpy-4.0.0b2/connpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-17 20:09:34.909044 connpy-4.0.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-17 20:09:29.000000 connpy-4.0.0b2/setup.py
```

### Comparing `connpy-4.0.0b1/LICENSE` & `connpy-4.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `connpy-4.0.0b1/PKG-INFO` & `connpy-4.0.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 4.0.0b1
+Version: 4.0.0b2
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
```

### Comparing `connpy-4.0.0b1/README.md` & `connpy-4.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `connpy-4.0.0b1/connpy/__init__.py` & `connpy-4.0.0b2/connpy/__init__.py`

 * *Files identical despite different names*

### Comparing `connpy-4.0.0b1/connpy/ai.py` & `connpy-4.0.0b2/connpy/ai.py`

 * *Files identical despite different names*

### Comparing `connpy-4.0.0b1/connpy/api.py` & `connpy-4.0.0b2/connpy/api.py`

 * *Files identical despite different names*

### Comparing `connpy-4.0.0b1/connpy/completion.py` & `connpy-4.0.0b2/connpy/completion.py`

 * *Files identical despite different names*

### Comparing `connpy-4.0.0b1/connpy/configfile.py` & `connpy-4.0.0b2/connpy/configfile.py`

 * *Files identical despite different names*

### Comparing `connpy-4.0.0b1/connpy/connapp.py` & `connpy-4.0.0b2/connpy/connapp.py`

 * *Files identical despite different names*

### Comparing `connpy-4.0.0b1/connpy/core.py` & `connpy-4.0.0b2/connpy/core.py`

 * *Files identical despite different names*

### Comparing `connpy-4.0.0b1/connpy/hooks.py` & `connpy-4.0.0b2/connpy/hooks.py`

 * *Files identical despite different names*

### Comparing `connpy-4.0.0b1/connpy/plugins.py` & `connpy-4.0.0b2/connpy/plugins.py`

 * *Files identical despite different names*

### Comparing `connpy-4.0.0b1/connpy.egg-info/PKG-INFO` & `connpy-4.0.0b2/connpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 4.0.0b1
+Version: 4.0.0b2
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
```

### Comparing `connpy-4.0.0b1/setup.cfg` & `connpy-4.0.0b2/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -40,11 +40,14 @@
 
 [options.entry_points]
 console_scripts = 
 	conn = connpy.__main__:main
 	connpy = connpy.__main__:main
 	connpy-completion-helper = connpy.completion:main
 
+[options.package_data]
+connpy = core_plugins/*
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

