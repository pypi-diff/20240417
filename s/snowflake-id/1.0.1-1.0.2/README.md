# Comparing `tmp/snowflake_id-1.0.1.tar.gz` & `tmp/snowflake_id-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowflake_id-1.0.1.tar", last modified: Mon Feb 26 22:43:03 2024, max compression
+gzip compressed data, was "snowflake_id-1.0.2.tar", last modified: Wed Apr 17 13:36:03 2024, max compression
```

## Comparing `snowflake_id-1.0.1.tar` & `snowflake_id-1.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2024-02-26 22:42:50.365422 snowflake_id-1.0.1/LICENSE
--rw-r--r--   0        0        0     1536 2024-02-26 22:42:50.365422 snowflake_id-1.0.1/README.md
--rw-r--r--   0        0        0     1658 2024-02-26 22:43:03.357414 snowflake_id-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      322 2024-02-26 22:42:50.365422 snowflake_id-1.0.1/src/snowflake/__init__.py
--rw-r--r--   0        0        0     4147 2024-02-26 22:42:50.365422 snowflake_id-1.0.1/src/snowflake/snowflake.py
--rw-r--r--   0        0        0     2715 2024-02-26 22:42:50.365422 snowflake_id-1.0.1/tests/test_generator.py
--rw-r--r--   0        0        0     2511 2024-02-26 22:42:50.365422 snowflake_id-1.0.1/tests/test_snowflake.py
--rw-r--r--   0        0        0     4055 1970-01-01 00:00:00.000000 snowflake_id-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-17 13:35:45.753204 snowflake_id-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1536 2024-04-17 13:35:45.753204 snowflake_id-1.0.2/README.md
+-rw-r--r--   0        0        0     1610 2024-04-17 13:36:03.449295 snowflake_id-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      322 2024-04-17 13:35:45.753204 snowflake_id-1.0.2/src/snowflake/__init__.py
+-rw-r--r--   0        0        0     4147 2024-04-17 13:35:45.753204 snowflake_id-1.0.2/src/snowflake/snowflake.py
+-rw-r--r--   0        0        0     2715 2024-04-17 13:35:45.753204 snowflake_id-1.0.2/tests/test_generator.py
+-rw-r--r--   0        0        0     2511 2024-04-17 13:35:45.753204 snowflake_id-1.0.2/tests/test_snowflake.py
+-rw-r--r--   0        0        0     4054 1970-01-01 00:00:00.000000 snowflake_id-1.0.2/PKG-INFO
```

### Comparing `snowflake_id-1.0.1/LICENSE` & `snowflake_id-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `snowflake_id-1.0.1/README.md` & `snowflake_id-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `snowflake_id-1.0.1/pyproject.toml` & `snowflake_id-1.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "snowflake-id"
-version = "1.0.1"
+version = "1.0.2"
 description = "The Snowflake generator done right"
 keywords = [
     "snowflake",
     "snowflake-id",
     "id",
     "ids",
     "generator",
@@ -26,15 +26,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 authors = [
     { name = "vd", email = "snowflake@vd2.org" },
 ]
 dependencies = []
-requires-python = ">=3.8,<3.13"
+requires-python = ">=3.8,<4.0"
 readme = "README.md"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 homepage = "https://github.com/vd2org/snowflake"
@@ -49,15 +49,14 @@
 
 [tool.pdm]
 distribution = true
 
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest~=8.0.2",
-    "ubump~=0.1.10; python_version >= '3.11'",
     "requests>=2.31.0",
 ]
 
 [tool.ubump]
 template = "v${major}.${minor}.${patch}"
 message = "Bump to ${version}"
 tag = true
```

### Comparing `snowflake_id-1.0.1/src/snowflake/snowflake.py` & `snowflake_id-1.0.2/src/snowflake/snowflake.py`

 * *Files identical despite different names*

### Comparing `snowflake_id-1.0.1/tests/test_generator.py` & `snowflake_id-1.0.2/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `snowflake_id-1.0.1/tests/test_snowflake.py` & `snowflake_id-1.0.2/tests/test_snowflake.py`

 * *Files identical despite different names*

### Comparing `snowflake_id-1.0.1/PKG-INFO` & `snowflake_id-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: snowflake-id
-Version: 1.0.1
+Version: 1.0.2
 Summary: The Snowflake generator done right
-Keywords: snowflake snowflake-id id ids generator
+Keywords: snowflake,snowflake-id,id,ids,generator
 Home-page: https://github.com/vd2org/snowflake
 Author-Email: vd <snowflake@vd2.org>
 License: MIT License
         
         Copyright (c) 2021-2024 Vd
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,15 +40,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Homepage, https://github.com/vd2org/snowflake
 Project-URL: Repository, https://github.com/vd2org/snowflake.git
 Project-URL: Issues, https://github.com/vd2org/snowflake/issues
-Requires-Python: <3.13,>=3.8
+Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
 
 # Snowflake
 
 The Snowflake generator done right.
 
 See [here](https://en.wikipedia.org/wiki/Snowflake_ID) for additional information.
```

