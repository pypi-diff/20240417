# Comparing `tmp/nose-launchable-0.5.0.tar.gz` & `tmp/nose_launchable-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nose-launchable-0.5.0.tar", last modified: Mon Mar 27 02:59:04 2023, max compression
+gzip compressed data, was "nose_launchable-0.6.0.tar", last modified: Wed Apr 17 03:05:58 2024, max compression
```

## Comparing `nose-launchable-0.5.0.tar` & `nose_launchable-0.6.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 02:59:04.164640 nose-launchable-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-03-27 02:58:47.000000 nose-launchable-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-03-27 02:58:47.000000 nose-launchable-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3273 2023-03-27 02:59:04.164640 nose-launchable-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2815 2023-03-27 02:58:47.000000 nose-launchable-0.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 02:59:04.160639 nose-launchable-0.5.0/nose_launchable/
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-03-27 02:58:47.000000 nose-launchable-0.5.0/nose_launchable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      873 2023-03-27 02:58:47.000000 nose-launchable-0.5.0/nose_launchable/case_event.py
--rw-r--r--   0 runner    (1001) docker     (122)     7309 2023-03-27 02:58:47.000000 nose-launchable-0.5.0/nose_launchable/client.py
--rw-r--r--   0 runner    (1001) docker     (122)      202 2023-03-27 02:58:47.000000 nose-launchable-0.5.0/nose_launchable/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     4282 2023-03-27 02:58:47.000000 nose-launchable-0.5.0/nose_launchable/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     8134 2023-03-27 02:58:47.000000 nose-launchable-0.5.0/nose_launchable/plugin.py
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-03-27 02:58:47.000000 nose-launchable-0.5.0/nose_launchable/protecter.py
--rw-r--r--   0 runner    (1001) docker     (122)      265 2023-03-27 02:58:47.000000 nose-launchable-0.5.0/nose_launchable/test_path_component.py
--rw-r--r--   0 runner    (1001) docker     (122)     2561 2023-03-27 02:58:47.000000 nose-launchable-0.5.0/nose_launchable/uploader.py
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-03-27 02:58:47.000000 nose-launchable-0.5.0/nose_launchable/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 02:59:04.164640 nose-launchable-0.5.0/nose_launchable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3273 2023-03-27 02:59:04.000000 nose-launchable-0.5.0/nose_launchable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      792 2023-03-27 02:59:04.000000 nose-launchable-0.5.0/nose_launchable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-27 02:59:04.000000 nose-launchable-0.5.0/nose_launchable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-03-27 02:59:04.000000 nose-launchable-0.5.0/nose_launchable.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-03-27 02:59:04.000000 nose-launchable-0.5.0/nose_launchable.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-03-27 02:59:04.000000 nose-launchable-0.5.0/nose_launchable.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-03-27 02:58:47.000000 nose-launchable-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-27 02:59:04.164640 nose-launchable-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1004 2023-03-27 02:58:47.000000 nose-launchable-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 02:59:04.164640 nose-launchable-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-27 02:58:47.000000 nose-launchable-0.5.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-27 02:59:04.164640 nose-launchable-0.5.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-27 02:58:47.000000 nose-launchable-0.5.0/tests/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-03-27 02:58:47.000000 nose-launchable-0.5.0/tests/resources/module0.py
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-03-27 02:58:47.000000 nose-launchable-0.5.0/tests/resources/module1.py
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-03-27 02:58:47.000000 nose-launchable-0.5.0/tests/resources/module2.py
--rw-r--r--   0 runner    (1001) docker     (122)    13730 2023-03-27 02:58:47.000000 nose-launchable-0.5.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     1748 2023-03-27 02:58:47.000000 nose-launchable-0.5.0/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)      687 2023-03-27 02:58:47.000000 nose-launchable-0.5.0/tests/test_protecter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3415 2023-03-27 02:58:47.000000 nose-launchable-0.5.0/tests/test_uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:05:58.910820 nose_launchable-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-17 03:05:45.000000 nose_launchable-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-17 03:05:45.000000 nose_launchable-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-17 03:05:58.910820 nose_launchable-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-17 03:05:45.000000 nose_launchable-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:05:58.906820 nose_launchable-0.6.0/nose_launchable/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-17 03:05:45.000000 nose_launchable-0.6.0/nose_launchable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-17 03:05:45.000000 nose_launchable-0.6.0/nose_launchable/case_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7309 2024-04-17 03:05:45.000000 nose_launchable-0.6.0/nose_launchable/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-17 03:05:45.000000 nose_launchable-0.6.0/nose_launchable/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-17 03:05:45.000000 nose_launchable-0.6.0/nose_launchable/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-04-17 03:05:45.000000 nose_launchable-0.6.0/nose_launchable/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-17 03:05:45.000000 nose_launchable-0.6.0/nose_launchable/protecter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-17 03:05:45.000000 nose_launchable-0.6.0/nose_launchable/test_path_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-17 03:05:45.000000 nose_launchable-0.6.0/nose_launchable/uploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-17 03:05:45.000000 nose_launchable-0.6.0/nose_launchable/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:05:58.910820 nose_launchable-0.6.0/nose_launchable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-17 03:05:58.000000 nose_launchable-0.6.0/nose_launchable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-17 03:05:58.000000 nose_launchable-0.6.0/nose_launchable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 03:05:58.000000 nose_launchable-0.6.0/nose_launchable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-17 03:05:58.000000 nose_launchable-0.6.0/nose_launchable.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-17 03:05:58.000000 nose_launchable-0.6.0/nose_launchable.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-17 03:05:58.000000 nose_launchable-0.6.0/nose_launchable.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-17 03:05:45.000000 nose_launchable-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 03:05:58.910820 nose_launchable-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-17 03:05:45.000000 nose_launchable-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:05:58.910820 nose_launchable-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:05:45.000000 nose_launchable-0.6.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:05:58.910820 nose_launchable-0.6.0/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:05:45.000000 nose_launchable-0.6.0/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-17 03:05:45.000000 nose_launchable-0.6.0/tests/resources/module0.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-17 03:05:45.000000 nose_launchable-0.6.0/tests/resources/module1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-17 03:05:45.000000 nose_launchable-0.6.0/tests/resources/module2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13730 2024-04-17 03:05:45.000000 nose_launchable-0.6.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-17 03:05:45.000000 nose_launchable-0.6.0/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-17 03:05:45.000000 nose_launchable-0.6.0/tests/test_protecter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-17 03:05:45.000000 nose_launchable-0.6.0/tests/test_uploader.py
```

### Comparing `nose-launchable-0.5.0/LICENSE` & `nose_launchable-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nose-launchable-0.5.0/PKG-INFO` & `nose_launchable-0.6.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: nose-launchable
-Version: 0.5.0
-Summary: A nose plugin to interact with Launchable API
-Home-page: https://github.com/launchableinc/nose-launchable
-Author: Launchable team
-Author-email:  info@launchableinc.com
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-License-File: LICENSE
-
 nose-launchable
 ===============
 
 A nose plugin to interact with
 `Launchable <https://www.launchableinc.com/>`__ API.
 
 Install
```

### Comparing `nose-launchable-0.5.0/README.rst` & `nose_launchable-0.6.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: nose-launchable
+Version: 0.6.0
+Summary: A nose plugin to interact with Launchable API
+Home-page: https://github.com/launchableinc/nose-launchable
+Author: Launchable team
+Author-email:  info@launchableinc.com
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
+Requires-Dist: launchable>=1.26.0,~=1.0
+Requires-Dist: nose>=1.0.0; python_version < "3.10"
+Requires-Dist: pynose>=1.5.1; python_version >= "3.10"
+Requires-Dist: boto3>=1.0.0
+Requires-Dist: requests>=2.0.0
+Requires-Dist: urllib3<2
+
 nose-launchable
 ===============
 
 A nose plugin to interact with
 `Launchable <https://www.launchableinc.com/>`__ API.
 
 Install
```

### Comparing `nose-launchable-0.5.0/nose_launchable/case_event.py` & `nose_launchable-0.6.0/nose_launchable/case_event.py`

 * *Files identical despite different names*

### Comparing `nose-launchable-0.5.0/nose_launchable/client.py` & `nose_launchable-0.6.0/nose_launchable/client.py`

 * *Files identical despite different names*

### Comparing `nose-launchable-0.5.0/nose_launchable/manager.py` & `nose_launchable-0.6.0/nose_launchable/manager.py`

 * *Files identical despite different names*

### Comparing `nose-launchable-0.5.0/nose_launchable/plugin.py` & `nose_launchable-0.6.0/nose_launchable/plugin.py`

 * *Files identical despite different names*

### Comparing `nose-launchable-0.5.0/nose_launchable/protecter.py` & `nose_launchable-0.6.0/nose_launchable/protecter.py`

 * *Files identical despite different names*

### Comparing `nose-launchable-0.5.0/nose_launchable/uploader.py` & `nose_launchable-0.6.0/nose_launchable/uploader.py`

 * *Files identical despite different names*

### Comparing `nose-launchable-0.5.0/nose_launchable.egg-info/PKG-INFO` & `nose_launchable-0.6.0/nose_launchable.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 Metadata-Version: 2.1
 Name: nose-launchable
-Version: 0.5.0
+Version: 0.6.0
 Summary: A nose plugin to interact with Launchable API
 Home-page: https://github.com/launchableinc/nose-launchable
 Author: Launchable team
 Author-email:  info@launchableinc.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
+Requires-Dist: launchable>=1.26.0,~=1.0
+Requires-Dist: nose>=1.0.0; python_version < "3.10"
+Requires-Dist: pynose>=1.5.1; python_version >= "3.10"
+Requires-Dist: boto3>=1.0.0
+Requires-Dist: requests>=2.0.0
+Requires-Dist: urllib3<2
 
 nose-launchable
 ===============
 
 A nose plugin to interact with
 `Launchable <https://www.launchableinc.com/>`__ API.
```

### Comparing `nose-launchable-0.5.0/nose_launchable.egg-info/SOURCES.txt` & `nose_launchable-0.6.0/nose_launchable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nose-launchable-0.5.0/setup.py` & `nose_launchable-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `nose-launchable-0.5.0/tests/test_client.py` & `nose_launchable-0.6.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `nose-launchable-0.5.0/tests/test_manager.py` & `nose_launchable-0.6.0/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `nose-launchable-0.5.0/tests/test_protecter.py` & `nose_launchable-0.6.0/tests/test_protecter.py`

 * *Files identical despite different names*

### Comparing `nose-launchable-0.5.0/tests/test_uploader.py` & `nose_launchable-0.6.0/tests/test_uploader.py`

 * *Files identical despite different names*

