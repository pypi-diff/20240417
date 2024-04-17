# Comparing `tmp/ebs-linuxnode-modapi-3.4.1.tar.gz` & `tmp/ebs-linuxnode-modapi-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebs-linuxnode-modapi-3.4.1.tar", last modified: Sat Mar 30 12:18:41 2024, max compression
+gzip compressed data, was "ebs-linuxnode-modapi-3.5.0.tar", last modified: Wed Apr 17 21:39:48 2024, max compression
```

## Comparing `ebs-linuxnode-modapi-3.4.1.tar` & `ebs-linuxnode-modapi-3.5.0.tar`

### file list

```diff
@@ -1,32 +1,43 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-30 12:18:41.535919 ebs-linuxnode-modapi-3.4.1/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2233 2023-03-15 16:55:09.000000 ebs-linuxnode-modapi-3.4.1/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      121 2023-03-15 16:55:09.000000 ebs-linuxnode-modapi-3.4.1/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      653 2024-03-30 12:18:41.535919 ebs-linuxnode-modapi-3.4.1/PKG-INFO
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-30 12:18:41.535919 ebs-linuxnode-modapi-3.4.1/ebs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:55:09.000000 ebs-linuxnode-modapi-3.4.1/ebs/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-30 12:18:41.535919 ebs-linuxnode-modapi-3.4.1/ebs/linuxnode/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:55:09.000000 ebs-linuxnode-modapi-3.4.1/ebs/linuxnode/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-30 12:18:41.535919 ebs-linuxnode-modapi-3.4.1/ebs/linuxnode/gui/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:55:09.000000 ebs-linuxnode-modapi-3.4.1/ebs/linuxnode/gui/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-30 12:18:41.535919 ebs-linuxnode-modapi-3.4.1/ebs/linuxnode/gui/kivy/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:55:09.000000 ebs-linuxnode-modapi-3.4.1/ebs/linuxnode/gui/kivy/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-30 12:18:41.535919 ebs-linuxnode-modapi-3.4.1/ebs/linuxnode/gui/kivy/modapi/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       53 2023-03-15 16:55:09.000000 ebs-linuxnode-modapi-3.4.1/ebs/linuxnode/gui/kivy/modapi/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-30 12:18:41.535919 ebs-linuxnode-modapi-3.4.1/ebs/linuxnode/gui/kivy/modapi/images/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1584 2023-03-15 16:55:09.000000 ebs-linuxnode-modapi-3.4.1/ebs/linuxnode/gui/kivy/modapi/images/no-internet.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    16453 2023-03-15 16:55:09.000000 ebs-linuxnode-modapi-3.4.1/ebs/linuxnode/gui/kivy/modapi/images/no-server.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5601 2024-03-30 12:00:21.000000 ebs-linuxnode-modapi-3.4.1/ebs/linuxnode/gui/kivy/modapi/mixin.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-30 12:18:41.535919 ebs-linuxnode-modapi-3.4.1/ebs/linuxnode/modapi/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 16:55:09.000000 ebs-linuxnode-modapi-3.4.1/ebs/linuxnode/modapi/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    12325 2024-03-24 03:41:08.000000 ebs-linuxnode-modapi-3.4.1/ebs/linuxnode/modapi/engine.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1306 2023-03-15 16:55:09.000000 ebs-linuxnode-modapi-3.4.1/ebs/linuxnode/modapi/manager.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     6681 2023-09-04 07:33:49.000000 ebs-linuxnode-modapi-3.4.1/ebs/linuxnode/modapi/primitives.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      439 2023-03-15 16:55:09.000000 ebs-linuxnode-modapi-3.4.1/ebs/linuxnode/modapi/standalone.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-03-30 12:18:41.535919 ebs-linuxnode-modapi-3.4.1/ebs_linuxnode_modapi.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      653 2024-03-30 12:18:41.000000 ebs-linuxnode-modapi-3.4.1/ebs_linuxnode_modapi.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      708 2024-03-30 12:18:41.000000 ebs-linuxnode-modapi-3.4.1/ebs_linuxnode_modapi.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-03-30 12:18:41.000000 ebs-linuxnode-modapi-3.4.1/ebs_linuxnode_modapi.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       95 2024-03-30 12:18:41.000000 ebs-linuxnode-modapi-3.4.1/ebs_linuxnode_modapi.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        4 2024-03-30 12:18:41.000000 ebs-linuxnode-modapi-3.4.1/ebs_linuxnode_modapi.egg-info/top_level.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       38 2024-03-30 12:18:41.535919 ebs-linuxnode-modapi-3.4.1/setup.cfg
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1406 2023-09-04 09:32:30.000000 ebs-linuxnode-modapi-3.4.1/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-17 21:39:48.188987 ebs-linuxnode-modapi-3.5.0/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2233 2023-03-15 16:55:09.000000 ebs-linuxnode-modapi-3.5.0/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      121 2023-03-15 16:55:09.000000 ebs-linuxnode-modapi-3.5.0/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      653 2024-04-17 21:39:48.188987 ebs-linuxnode-modapi-3.5.0/PKG-INFO
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-17 21:39:48.184987 ebs-linuxnode-modapi-3.5.0/ebs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:55:09.000000 ebs-linuxnode-modapi-3.5.0/ebs/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-17 21:39:48.184987 ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:55:09.000000 ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-17 21:39:48.184987 ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/gui/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:55:09.000000 ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/gui/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-17 21:39:48.184987 ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/gui/kivy/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:55:09.000000 ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/gui/kivy/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-17 21:39:48.184987 ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/gui/kivy/modapi/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       53 2023-03-15 16:55:09.000000 ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/gui/kivy/modapi/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-17 21:39:48.184987 ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/gui/kivy/modapi/images/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1584 2023-03-15 16:55:09.000000 ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/gui/kivy/modapi/images/no-internet.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    16453 2023-03-15 16:55:09.000000 ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/gui/kivy/modapi/images/no-server.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5601 2024-04-16 22:12:50.000000 ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/gui/kivy/modapi/mixin.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-17 21:39:48.184987 ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/modapi/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-03-15 16:55:09.000000 ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/modapi/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-17 21:39:48.184987 ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/modapi/engines/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2024-04-16 21:26:51.000000 ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/modapi/engines/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-17 21:39:48.188987 ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/modapi/engines/amqp/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2024-04-16 21:45:28.000000 ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/modapi/engines/amqp/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1207 2024-04-17 21:29:46.000000 ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/modapi/engines/amqp/commands.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2555 2024-04-17 15:09:53.000000 ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/modapi/engines/amqp/core.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     6004 2024-04-17 14:28:47.000000 ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/modapi/engines/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      450 2024-04-17 02:56:57.000000 ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/modapi/engines/exceptions.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     6513 2024-04-16 21:32:01.000000 ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/modapi/engines/http.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1306 2023-03-15 16:55:09.000000 ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/modapi/manager.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     6681 2023-09-04 07:33:49.000000 ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/modapi/primitives.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      439 2023-03-15 16:55:09.000000 ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/modapi/standalone.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-17 21:39:48.188987 ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/mq/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2024-04-17 00:45:43.000000 ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/mq/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9651 2024-04-17 21:30:56.000000 ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/mq/amqp.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-17 21:39:48.188987 ebs-linuxnode-modapi-3.5.0/ebs_linuxnode_modapi.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      653 2024-04-17 21:39:48.000000 ebs-linuxnode-modapi-3.5.0/ebs_linuxnode_modapi.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1023 2024-04-17 21:39:48.000000 ebs-linuxnode-modapi-3.5.0/ebs_linuxnode_modapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-17 21:39:48.000000 ebs-linuxnode-modapi-3.5.0/ebs_linuxnode_modapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       95 2024-04-17 21:39:48.000000 ebs-linuxnode-modapi-3.5.0/ebs_linuxnode_modapi.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        4 2024-04-17 21:39:48.000000 ebs-linuxnode-modapi-3.5.0/ebs_linuxnode_modapi.egg-info/top_level.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       38 2024-04-17 21:39:48.188987 ebs-linuxnode-modapi-3.5.0/setup.cfg
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1406 2023-09-04 09:32:30.000000 ebs-linuxnode-modapi-3.5.0/setup.py
```

### Comparing `ebs-linuxnode-modapi-3.4.1/.gitignore` & `ebs-linuxnode-modapi-3.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ebs-linuxnode-modapi-3.4.1/PKG-INFO` & `ebs-linuxnode-modapi-3.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebs-linuxnode-modapi
-Version: 3.4.1
+Version: 3.5.0
 Summary: Modular API Client Infrastructure for EBS linuxnode applications
 Home-page: https://github.com/ebs-universe/ebs-linuxnode-modapi
 Author: Chintalagiri Shashank
 Author-email: shashank.chintalagiri@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `ebs-linuxnode-modapi-3.4.1/ebs/linuxnode/gui/kivy/modapi/images/no-internet.png` & `ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/gui/kivy/modapi/images/no-internet.png`

 * *Files identical despite different names*

### Comparing `ebs-linuxnode-modapi-3.4.1/ebs/linuxnode/gui/kivy/modapi/images/no-server.png` & `ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/gui/kivy/modapi/images/no-server.png`

 * *Files identical despite different names*

### Comparing `ebs-linuxnode-modapi-3.4.1/ebs/linuxnode/gui/kivy/modapi/mixin.py` & `ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/gui/kivy/modapi/mixin.py`

 * *Files identical despite different names*

### Comparing `ebs-linuxnode-modapi-3.4.1/ebs/linuxnode/modapi/manager.py` & `ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/modapi/manager.py`

 * *Files identical despite different names*

### Comparing `ebs-linuxnode-modapi-3.4.1/ebs/linuxnode/modapi/primitives.py` & `ebs-linuxnode-modapi-3.5.0/ebs/linuxnode/modapi/primitives.py`

 * *Files identical despite different names*

### Comparing `ebs-linuxnode-modapi-3.4.1/ebs_linuxnode_modapi.egg-info/PKG-INFO` & `ebs-linuxnode-modapi-3.5.0/ebs_linuxnode_modapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebs-linuxnode-modapi
-Version: 3.4.1
+Version: 3.5.0
 Summary: Modular API Client Infrastructure for EBS linuxnode applications
 Home-page: https://github.com/ebs-universe/ebs-linuxnode-modapi
 Author: Chintalagiri Shashank
 Author-email: shashank.chintalagiri@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `ebs-linuxnode-modapi-3.4.1/ebs_linuxnode_modapi.egg-info/SOURCES.txt` & `ebs-linuxnode-modapi-3.5.0/ebs_linuxnode_modapi.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -6,16 +6,24 @@
 ebs/linuxnode/gui/__init__.py
 ebs/linuxnode/gui/kivy/__init__.py
 ebs/linuxnode/gui/kivy/modapi/__init__.py
 ebs/linuxnode/gui/kivy/modapi/mixin.py
 ebs/linuxnode/gui/kivy/modapi/images/no-internet.png
 ebs/linuxnode/gui/kivy/modapi/images/no-server.png
 ebs/linuxnode/modapi/__init__.py
-ebs/linuxnode/modapi/engine.py
 ebs/linuxnode/modapi/manager.py
 ebs/linuxnode/modapi/primitives.py
 ebs/linuxnode/modapi/standalone.py
+ebs/linuxnode/modapi/engines/__init__.py
+ebs/linuxnode/modapi/engines/base.py
+ebs/linuxnode/modapi/engines/exceptions.py
+ebs/linuxnode/modapi/engines/http.py
+ebs/linuxnode/modapi/engines/amqp/__init__.py
+ebs/linuxnode/modapi/engines/amqp/commands.py
+ebs/linuxnode/modapi/engines/amqp/core.py
+ebs/linuxnode/mq/__init__.py
+ebs/linuxnode/mq/amqp.py
 ebs_linuxnode_modapi.egg-info/PKG-INFO
 ebs_linuxnode_modapi.egg-info/SOURCES.txt
 ebs_linuxnode_modapi.egg-info/dependency_links.txt
 ebs_linuxnode_modapi.egg-info/requires.txt
 ebs_linuxnode_modapi.egg-info/top_level.txt
```

### Comparing `ebs-linuxnode-modapi-3.4.1/setup.py` & `ebs-linuxnode-modapi-3.5.0/setup.py`

 * *Files identical despite different names*

