# Comparing `tmp/dig_ass_text_protos-0.0.5.tar.gz` & `tmp/dig_ass_text_protos-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dig_ass_text_protos-0.0.5.tar", last modified: Mon Apr 15 13:10:10 2024, max compression
+gzip compressed data, was "dig_ass_text_protos-0.0.6.tar", last modified: Wed Apr 17 17:57:30 2024, max compression
```

## Comparing `dig_ass_text_protos-0.0.5.tar` & `dig_ass_text_protos-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-15 13:10:10.006558 dig_ass_text_protos-0.0.5/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_text_protos-0.0.5/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-15 13:10:10.006558 dig_ass_text_protos-0.0.5/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:59:00.000000 dig_ass_text_protos-0.0.5/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-15 13:10:10.006558 dig_ass_text_protos-0.0.5/dig_ass_text_protos/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2725 2024-04-15 13:10:08.000000 dig_ass_text_protos-0.0.5/dig_ass_text_protos/DigitalAssistantText_pb2.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2366 2024-04-15 13:10:08.000000 dig_ass_text_protos-0.0.5/dig_ass_text_protos/DigitalAssistantText_pb2.pyi
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2946 2024-04-15 13:10:08.000000 dig_ass_text_protos-0.0.5/dig_ass_text_protos/DigitalAssistantText_pb2_grpc.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-15 13:01:41.000000 dig_ass_text_protos-0.0.5/dig_ass_text_protos/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      389 2024-04-12 20:28:21.000000 dig_ass_text_protos-0.0.5/dig_ass_text_protos/abstract_client.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1492 2024-04-15 11:32:31.000000 dig_ass_text_protos-0.0.5/dig_ass_text_protos/client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-15 13:10:10.006558 dig_ass_text_protos-0.0.5/dig_ass_text_protos.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-15 13:10:09.000000 dig_ass_text_protos-0.0.5/dig_ass_text_protos.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      512 2024-04-15 13:10:10.000000 dig_ass_text_protos-0.0.5/dig_ass_text_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-15 13:10:09.000000 dig_ass_text_protos-0.0.5/dig_ass_text_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-15 13:10:09.000000 dig_ass_text_protos-0.0.5/dig_ass_text_protos.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       20 2024-04-15 13:10:09.000000 dig_ass_text_protos-0.0.5/dig_ass_text_protos.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_text_protos-0.0.5/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-15 13:10:10.006558 dig_ass_text_protos-0.0.5/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      803 2024-04-11 10:26:57.000000 dig_ass_text_protos-0.0.5/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-17 17:57:30.496836 dig_ass_text_protos-0.0.6/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_text_protos-0.0.6/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-17 17:57:30.496836 dig_ass_text_protos-0.0.6/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:59:00.000000 dig_ass_text_protos-0.0.6/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-17 17:57:30.492836 dig_ass_text_protos-0.0.6/dig_ass_text_protos/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2725 2024-04-17 17:57:29.000000 dig_ass_text_protos-0.0.6/dig_ass_text_protos/DigitalAssistantText_pb2.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2366 2024-04-17 17:57:29.000000 dig_ass_text_protos-0.0.6/dig_ass_text_protos/DigitalAssistantText_pb2.pyi
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2946 2024-04-17 17:57:29.000000 dig_ass_text_protos-0.0.6/dig_ass_text_protos/DigitalAssistantText_pb2_grpc.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-17 17:56:53.000000 dig_ass_text_protos-0.0.6/dig_ass_text_protos/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      389 2024-04-12 20:28:21.000000 dig_ass_text_protos-0.0.6/dig_ass_text_protos/abstract_client.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1307 2024-04-17 17:55:45.000000 dig_ass_text_protos-0.0.6/dig_ass_text_protos/client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-17 17:57:30.492836 dig_ass_text_protos-0.0.6/dig_ass_text_protos.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-17 17:57:30.000000 dig_ass_text_protos-0.0.6/dig_ass_text_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      512 2024-04-17 17:57:30.000000 dig_ass_text_protos-0.0.6/dig_ass_text_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-17 17:57:30.000000 dig_ass_text_protos-0.0.6/dig_ass_text_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-17 17:57:30.000000 dig_ass_text_protos-0.0.6/dig_ass_text_protos.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       20 2024-04-17 17:57:30.000000 dig_ass_text_protos-0.0.6/dig_ass_text_protos.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_text_protos-0.0.6/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-17 17:57:30.496836 dig_ass_text_protos-0.0.6/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      803 2024-04-11 10:26:57.000000 dig_ass_text_protos-0.0.6/setup.py
```

### Comparing `dig_ass_text_protos-0.0.5/dig_ass_text_protos/DigitalAssistantText_pb2.py` & `dig_ass_text_protos-0.0.6/dig_ass_text_protos/DigitalAssistantText_pb2.py`

 * *Files identical despite different names*

### Comparing `dig_ass_text_protos-0.0.5/dig_ass_text_protos/DigitalAssistantText_pb2.pyi` & `dig_ass_text_protos-0.0.6/dig_ass_text_protos/DigitalAssistantText_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dig_ass_text_protos-0.0.5/dig_ass_text_protos/DigitalAssistantText_pb2_grpc.py` & `dig_ass_text_protos-0.0.6/dig_ass_text_protos/DigitalAssistantText_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dig_ass_text_protos-0.0.5/dig_ass_text_protos.egg-info/SOURCES.txt` & `dig_ass_text_protos-0.0.6/dig_ass_text_protos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dig_ass_text_protos-0.0.5/setup.py` & `dig_ass_text_protos-0.0.6/setup.py`

 * *Files identical despite different names*

