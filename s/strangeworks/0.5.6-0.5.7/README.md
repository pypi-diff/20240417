# Comparing `tmp/strangeworks-0.5.6.tar.gz` & `tmp/strangeworks-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks-0.5.6.tar", max compression
+gzip compressed data, was "strangeworks-0.5.7.tar", max compression
```

## Comparing `strangeworks-0.5.6.tar` & `strangeworks-0.5.7.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0      222 2024-04-09 13:07:27.042629 strangeworks-0.5.6/DESCRIPTION.md
--rw-r--r--   0        0        0    11357 2024-04-09 13:07:27.042629 strangeworks-0.5.6/LICENSE
--rw-r--r--   0        0        0      818 2024-04-09 13:07:41.162781 strangeworks-0.5.6/pyproject.toml
--rw-r--r--   0        0        0      981 2024-04-09 13:07:27.042629 strangeworks-0.5.6/strangeworks/__init__.py
--rw-r--r--   0        0        0       19 2024-04-09 13:07:27.042629 strangeworks-0.5.6/strangeworks/core/client/__init__.py
--rw-r--r--   0        0        0      558 2024-04-09 13:07:27.042629 strangeworks-0.5.6/strangeworks/core/client/auth.py
--rw-r--r--   0        0        0     2883 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/client/backends.py
--rw-r--r--   0        0        0    16008 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/client/experiments.py
--rw-r--r--   0        0        0     5494 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/client/file.py
--rw-r--r--   0        0        0     6411 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/client/jobs.py
--rw-r--r--   0        0        0     1571 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/client/resource.py
--rw-r--r--   0        0        0    11287 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/client/rest_client.py
--rw-r--r--   0        0        0     3275 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/client/transport.py
--rw-r--r--   0        0        0     1056 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/client/workspace.py
--rw-r--r--   0        0        0        0 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/config/__init__.py
--rw-r--r--   0        0        0     1640 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/config/base.py
--rw-r--r--   0        0        0     5604 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/config/config.py
--rw-r--r--   0        0        0      876 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/config/defaults.py
--rw-r--r--   0        0        0     1611 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/config/env.py
--rw-r--r--   0        0        0     6719 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/config/file.py
--rw-r--r--   0        0        0       17 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/errors/__init__.py
--rw-r--r--   0        0        0     2614 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/errors/error.py
--rw-r--r--   0        0        0      714 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/core/utils.py
--rw-r--r--   0        0        0      475 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/platform/gql.py
--rw-r--r--   0        0        0    31966 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/sw_client.py
--rw-r--r--   0        0        0      323 2024-04-09 13:07:27.046629 strangeworks-0.5.6/strangeworks/utils.py
--rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 strangeworks-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0      222 2024-04-17 20:38:28.790147 strangeworks-0.5.7/DESCRIPTION.md
+-rw-r--r--   0        0        0    11357 2024-04-17 20:38:28.790147 strangeworks-0.5.7/LICENSE
+-rw-r--r--   0        0        0      818 2024-04-17 20:38:42.298190 strangeworks-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0      981 2024-04-17 20:38:28.790147 strangeworks-0.5.7/strangeworks/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 20:38:28.790147 strangeworks-0.5.7/strangeworks/core/__init__.py
+-rw-r--r--   0        0        0       19 2024-04-17 20:38:28.790147 strangeworks-0.5.7/strangeworks/core/client/__init__.py
+-rw-r--r--   0        0        0      558 2024-04-17 20:38:28.790147 strangeworks-0.5.7/strangeworks/core/client/auth.py
+-rw-r--r--   0        0        0     2883 2024-04-17 20:38:28.790147 strangeworks-0.5.7/strangeworks/core/client/backends.py
+-rw-r--r--   0        0        0    16008 2024-04-17 20:38:28.790147 strangeworks-0.5.7/strangeworks/core/client/experiments.py
+-rw-r--r--   0        0        0     5494 2024-04-17 20:38:28.790147 strangeworks-0.5.7/strangeworks/core/client/file.py
+-rw-r--r--   0        0        0     6411 2024-04-17 20:38:28.790147 strangeworks-0.5.7/strangeworks/core/client/jobs.py
+-rw-r--r--   0        0        0     1571 2024-04-17 20:38:28.790147 strangeworks-0.5.7/strangeworks/core/client/resource.py
+-rw-r--r--   0        0        0    11287 2024-04-17 20:38:28.790147 strangeworks-0.5.7/strangeworks/core/client/rest_client.py
+-rw-r--r--   0        0        0     3275 2024-04-17 20:38:28.790147 strangeworks-0.5.7/strangeworks/core/client/transport.py
+-rw-r--r--   0        0        0     1056 2024-04-17 20:38:28.790147 strangeworks-0.5.7/strangeworks/core/client/workspace.py
+-rw-r--r--   0        0        0        0 2024-04-17 20:38:28.790147 strangeworks-0.5.7/strangeworks/core/config/__init__.py
+-rw-r--r--   0        0        0     1640 2024-04-17 20:38:28.790147 strangeworks-0.5.7/strangeworks/core/config/base.py
+-rw-r--r--   0        0        0     5604 2024-04-17 20:38:28.790147 strangeworks-0.5.7/strangeworks/core/config/config.py
+-rw-r--r--   0        0        0      876 2024-04-17 20:38:28.790147 strangeworks-0.5.7/strangeworks/core/config/defaults.py
+-rw-r--r--   0        0        0     1611 2024-04-17 20:38:28.790147 strangeworks-0.5.7/strangeworks/core/config/env.py
+-rw-r--r--   0        0        0     6719 2024-04-17 20:38:28.790147 strangeworks-0.5.7/strangeworks/core/config/file.py
+-rw-r--r--   0        0        0       17 2024-04-17 20:38:28.790147 strangeworks-0.5.7/strangeworks/core/errors/__init__.py
+-rw-r--r--   0        0        0     2614 2024-04-17 20:38:28.794147 strangeworks-0.5.7/strangeworks/core/errors/error.py
+-rw-r--r--   0        0        0      714 2024-04-17 20:38:28.794147 strangeworks-0.5.7/strangeworks/core/utils.py
+-rw-r--r--   0        0        0      475 2024-04-17 20:38:28.794147 strangeworks-0.5.7/strangeworks/platform/gql.py
+-rw-r--r--   0        0        0    31966 2024-04-17 20:38:28.794147 strangeworks-0.5.7/strangeworks/sw_client.py
+-rw-r--r--   0        0        0      323 2024-04-17 20:38:28.794147 strangeworks-0.5.7/strangeworks/utils.py
+-rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 strangeworks-0.5.7/PKG-INFO
```

### Comparing `strangeworks-0.5.6/LICENSE` & `strangeworks-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.6/pyproject.toml` & `strangeworks-0.5.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strangeworks"
-version = "0.5.6"
+version = "0.5.7"
 description = "Strangeworks Python SDK"
 readme = "DESCRIPTION.md"
 authors = ["Strange Devs <hello@strangeworks.com>"]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `strangeworks-0.5.6/strangeworks/__init__.py` & `strangeworks-0.5.7/strangeworks/__init__.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.6/strangeworks/core/client/auth.py` & `strangeworks-0.5.7/strangeworks/core/client/auth.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.6/strangeworks/core/client/backends.py` & `strangeworks-0.5.7/strangeworks/core/client/backends.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.6/strangeworks/core/client/experiments.py` & `strangeworks-0.5.7/strangeworks/core/client/experiments.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.6/strangeworks/core/client/file.py` & `strangeworks-0.5.7/strangeworks/core/client/file.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.6/strangeworks/core/client/jobs.py` & `strangeworks-0.5.7/strangeworks/core/client/jobs.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.6/strangeworks/core/client/resource.py` & `strangeworks-0.5.7/strangeworks/core/client/resource.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.6/strangeworks/core/client/rest_client.py` & `strangeworks-0.5.7/strangeworks/core/client/rest_client.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.6/strangeworks/core/client/transport.py` & `strangeworks-0.5.7/strangeworks/core/client/transport.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.6/strangeworks/core/client/workspace.py` & `strangeworks-0.5.7/strangeworks/core/client/workspace.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.6/strangeworks/core/config/base.py` & `strangeworks-0.5.7/strangeworks/core/config/base.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.6/strangeworks/core/config/config.py` & `strangeworks-0.5.7/strangeworks/core/config/config.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.6/strangeworks/core/config/defaults.py` & `strangeworks-0.5.7/strangeworks/core/config/defaults.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.6/strangeworks/core/config/env.py` & `strangeworks-0.5.7/strangeworks/core/config/env.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.6/strangeworks/core/config/file.py` & `strangeworks-0.5.7/strangeworks/core/config/file.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.6/strangeworks/core/errors/error.py` & `strangeworks-0.5.7/strangeworks/core/errors/error.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.6/strangeworks/core/utils.py` & `strangeworks-0.5.7/strangeworks/core/utils.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.6/strangeworks/sw_client.py` & `strangeworks-0.5.7/strangeworks/sw_client.py`

 * *Files identical despite different names*

### Comparing `strangeworks-0.5.6/PKG-INFO` & `strangeworks-0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strangeworks
-Version: 0.5.6
+Version: 0.5.7
 Summary: Strangeworks Python SDK
 License: Apache-2.0
 Author: Strange Devs
 Author-email: hello@strangeworks.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

