# Comparing `tmp/sentenai-1.7.0.2.tar.gz` & `tmp/sentenai-1.7.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentenai-1.7.0.2.tar", last modified: Thu Feb  8 03:11:03 2024, max compression
+gzip compressed data, was "sentenai-1.7.1.1.tar", last modified: Wed Apr 17 20:29:47 2024, max compression
```

## Comparing `sentenai-1.7.0.2.tar` & `sentenai-1.7.1.1.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2024-02-08 03:11:03.223480 sentenai-1.7.0.2/
--rw-r--r--   0 xnomagichash   (501) staff       (20)      598 2021-12-01 20:18:24.000000 sentenai-1.7.0.2/.coveragerc
--rw-r--r--   0 xnomagichash   (501) staff       (20)       57 2021-12-01 20:18:24.000000 sentenai-1.7.0.2/.editorconfig
--rw-r--r--   0 xnomagichash   (501) staff       (20)     1115 2022-10-20 02:44:17.000000 sentenai-1.7.0.2/.gitignore
--rw-r--r--   0 xnomagichash   (501) staff       (20)      190 2021-12-01 20:18:24.000000 sentenai-1.7.0.2/.travis.yml
--rw-r--r--   0 xnomagichash   (501) staff       (20)     1514 2021-12-01 20:18:24.000000 sentenai-1.7.0.2/LICENSE
--rw-r--r--   0 xnomagichash   (501) staff       (20)      193 2021-12-01 20:18:24.000000 sentenai-1.7.0.2/Makefile
--rw-r--r--   0 xnomagichash   (501) staff       (20)      721 2024-02-08 03:11:03.223537 sentenai-1.7.0.2/PKG-INFO
--rw-r--r--   0 xnomagichash   (501) staff       (20)      781 2021-12-01 20:18:24.000000 sentenai-1.7.0.2/README.md
--rw-r--r--   0 xnomagichash   (501) staff       (20)      141 2021-12-01 20:18:24.000000 sentenai-1.7.0.2/requirements.txt
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2024-02-08 03:11:03.218728 sentenai-1.7.0.2/sentenai/
--rw-r--r--   0 xnomagichash   (501) staff       (20)    12003 2024-02-01 22:05:19.000000 sentenai-1.7.0.2/sentenai/__init__.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)    10113 2024-02-08 03:10:02.000000 sentenai-1.7.0.2/sentenai/api.py
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2024-02-08 03:11:03.220581 sentenai-1.7.0.2/sentenai/stream/
--rw-r--r--   0 xnomagichash   (501) staff       (20)       59 2023-05-04 20:20:46.000000 sentenai-1.7.0.2/sentenai/stream/__init__.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     5141 2022-03-25 18:39:40.000000 sentenai-1.7.0.2/sentenai/stream/events.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     2284 2023-06-20 01:41:51.000000 sentenai-1.7.0.2/sentenai/stream/metadata.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)    24864 2024-02-08 03:08:48.000000 sentenai-1.7.0.2/sentenai/stream/streams.py
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2024-02-08 03:11:03.221932 sentenai-1.7.0.2/sentenai/tests/
--rw-r--r--   0 xnomagichash   (501) staff       (20)        0 2021-12-01 20:18:24.000000 sentenai-1.7.0.2/sentenai/tests/__init__.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)      468 2021-12-01 20:18:24.000000 sentenai-1.7.0.2/sentenai/tests/conftest.py
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2024-02-08 03:11:03.222305 sentenai-1.7.0.2/sentenai/tests/streams/
--rw-r--r--   0 xnomagichash   (501) staff       (20)        0 2021-12-01 20:18:24.000000 sentenai-1.7.0.2/sentenai/tests/streams/__init__.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)        0 2021-12-01 20:18:24.000000 sentenai-1.7.0.2/sentenai/tests/streams/__init__.py-e
--rw-r--r--   0 xnomagichash   (501) staff       (20)      924 2021-12-01 20:18:24.000000 sentenai-1.7.0.2/sentenai/tests/streams/test_stream.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)      924 2021-12-01 20:18:24.000000 sentenai-1.7.0.2/sentenai/tests/streams/test_stream.py-e
--rw-r--r--   0 xnomagichash   (501) staff       (20)      231 2021-12-01 20:18:24.000000 sentenai-1.7.0.2/sentenai/tests/test_client.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     4032 2021-12-01 20:18:24.000000 sentenai-1.7.0.2/sentenai/tests/test_events.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     1289 2021-12-01 20:18:24.000000 sentenai-1.7.0.2/sentenai/tests/test_fields.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)      543 2021-12-01 20:18:24.000000 sentenai-1.7.0.2/sentenai/tests/test_streams.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     1357 2021-12-01 20:18:24.000000 sentenai-1.7.0.2/sentenai/tests/test_views.py
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2024-02-08 03:11:03.219489 sentenai-1.7.0.2/sentenai.egg-info/
--rw-r--r--   0 xnomagichash   (501) staff       (20)      721 2024-02-08 03:11:02.000000 sentenai-1.7.0.2/sentenai.egg-info/PKG-INFO
--rw-r--r--   0 xnomagichash   (501) staff       (20)      926 2024-02-08 03:11:03.000000 sentenai-1.7.0.2/sentenai.egg-info/SOURCES.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)        1 2024-02-08 03:11:02.000000 sentenai-1.7.0.2/sentenai.egg-info/dependency_links.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)       68 2024-02-08 03:11:03.000000 sentenai-1.7.0.2/sentenai.egg-info/requires.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)        9 2024-02-08 03:11:03.000000 sentenai-1.7.0.2/sentenai.egg-info/top_level.txt
--rw-r--r--   0 xnomagichash   (501) staff       (20)       79 2024-02-08 03:11:03.223734 sentenai-1.7.0.2/setup.cfg
--rw-r--r--   0 xnomagichash   (501) staff       (20)     1030 2024-02-08 03:10:57.000000 sentenai-1.7.0.2/setup.py
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2024-02-08 03:11:03.222740 sentenai-1.7.0.2/tests/
-drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2024-02-08 03:11:03.223354 sentenai-1.7.0.2/tests/flare/
--rw-r--r--   0 xnomagichash   (501) staff       (20)    16087 2021-12-01 20:18:24.000000 sentenai-1.7.0.2/tests/flare/test_ast.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)      448 2021-12-01 20:18:24.000000 sentenai-1.7.0.2/tests/flare/test_merge.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     6372 2021-12-01 20:18:24.000000 sentenai-1.7.0.2/tests/flare/test_queries.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     1954 2021-12-01 20:18:24.000000 sentenai-1.7.0.2/tests/flare/test_stream_construction.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)     5702 2021-12-01 20:18:24.000000 sentenai-1.7.0.2/tests/test_api.py
--rw-r--r--   0 xnomagichash   (501) staff       (20)      386 2021-12-01 20:18:24.000000 sentenai-1.7.0.2/tests/test_utils.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2024-04-17 20:29:47.151491 sentenai-1.7.1.1/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      598 2021-12-01 20:18:24.000000 sentenai-1.7.1.1/.coveragerc
+-rw-r--r--   0 xnomagichash   (501) staff       (20)       57 2021-12-01 20:18:24.000000 sentenai-1.7.1.1/.editorconfig
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     1115 2022-10-20 02:44:17.000000 sentenai-1.7.1.1/.gitignore
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      190 2021-12-01 20:18:24.000000 sentenai-1.7.1.1/.travis.yml
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     1514 2021-12-01 20:18:24.000000 sentenai-1.7.1.1/LICENSE
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      193 2021-12-01 20:18:24.000000 sentenai-1.7.1.1/Makefile
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      721 2024-04-17 20:29:47.151554 sentenai-1.7.1.1/PKG-INFO
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      781 2021-12-01 20:18:24.000000 sentenai-1.7.1.1/README.md
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      141 2021-12-01 20:18:24.000000 sentenai-1.7.1.1/requirements.txt
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2024-04-17 20:29:47.147347 sentenai-1.7.1.1/sentenai/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)    12003 2024-02-01 22:05:19.000000 sentenai-1.7.1.1/sentenai/__init__.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)    10113 2024-02-08 03:10:02.000000 sentenai-1.7.1.1/sentenai/api.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     7574 2024-04-14 12:44:20.000000 sentenai-1.7.1.1/sentenai/new.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2024-04-17 20:29:47.148800 sentenai-1.7.1.1/sentenai/stream/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)       59 2023-05-04 20:20:46.000000 sentenai-1.7.1.1/sentenai/stream/__init__.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     5141 2022-03-25 18:39:40.000000 sentenai-1.7.1.1/sentenai/stream/events.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     2284 2023-06-20 01:41:51.000000 sentenai-1.7.1.1/sentenai/stream/metadata.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)    24864 2024-03-21 18:42:21.000000 sentenai-1.7.1.1/sentenai/stream/streams.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2024-04-17 20:29:47.150150 sentenai-1.7.1.1/sentenai/tests/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)        0 2021-12-01 20:18:24.000000 sentenai-1.7.1.1/sentenai/tests/__init__.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      468 2021-12-01 20:18:24.000000 sentenai-1.7.1.1/sentenai/tests/conftest.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2024-04-17 20:29:47.150525 sentenai-1.7.1.1/sentenai/tests/streams/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)        0 2021-12-01 20:18:24.000000 sentenai-1.7.1.1/sentenai/tests/streams/__init__.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)        0 2021-12-01 20:18:24.000000 sentenai-1.7.1.1/sentenai/tests/streams/__init__.py-e
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      924 2021-12-01 20:18:24.000000 sentenai-1.7.1.1/sentenai/tests/streams/test_stream.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      924 2021-12-01 20:18:24.000000 sentenai-1.7.1.1/sentenai/tests/streams/test_stream.py-e
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      231 2021-12-01 20:18:24.000000 sentenai-1.7.1.1/sentenai/tests/test_client.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     4032 2021-12-01 20:18:24.000000 sentenai-1.7.1.1/sentenai/tests/test_events.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     1289 2021-12-01 20:18:24.000000 sentenai-1.7.1.1/sentenai/tests/test_fields.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      543 2021-12-01 20:18:24.000000 sentenai-1.7.1.1/sentenai/tests/test_streams.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     1357 2021-12-01 20:18:24.000000 sentenai-1.7.1.1/sentenai/tests/test_views.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2024-04-17 20:29:47.147991 sentenai-1.7.1.1/sentenai.egg-info/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      721 2024-04-17 20:29:46.000000 sentenai-1.7.1.1/sentenai.egg-info/PKG-INFO
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      942 2024-04-17 20:29:47.000000 sentenai-1.7.1.1/sentenai.egg-info/SOURCES.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)        1 2024-04-17 20:29:46.000000 sentenai-1.7.1.1/sentenai.egg-info/dependency_links.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)       68 2024-04-17 20:29:47.000000 sentenai-1.7.1.1/sentenai.egg-info/requires.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)        9 2024-04-17 20:29:47.000000 sentenai-1.7.1.1/sentenai.egg-info/top_level.txt
+-rw-r--r--   0 xnomagichash   (501) staff       (20)       79 2024-04-17 20:29:47.151759 sentenai-1.7.1.1/setup.cfg
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     1030 2024-04-17 20:28:42.000000 sentenai-1.7.1.1/setup.py
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2024-04-17 20:29:47.150848 sentenai-1.7.1.1/tests/
+drwxr-xr-x   0 xnomagichash   (501) staff       (20)        0 2024-04-17 20:29:47.151383 sentenai-1.7.1.1/tests/flare/
+-rw-r--r--   0 xnomagichash   (501) staff       (20)    16087 2021-12-01 20:18:24.000000 sentenai-1.7.1.1/tests/flare/test_ast.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      448 2021-12-01 20:18:24.000000 sentenai-1.7.1.1/tests/flare/test_merge.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     6372 2021-12-01 20:18:24.000000 sentenai-1.7.1.1/tests/flare/test_queries.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     1954 2021-12-01 20:18:24.000000 sentenai-1.7.1.1/tests/flare/test_stream_construction.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)     5702 2021-12-01 20:18:24.000000 sentenai-1.7.1.1/tests/test_api.py
+-rw-r--r--   0 xnomagichash   (501) staff       (20)      386 2021-12-01 20:18:24.000000 sentenai-1.7.1.1/tests/test_utils.py
```

### Comparing `sentenai-1.7.0.2/.coveragerc` & `sentenai-1.7.1.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `sentenai-1.7.0.2/.gitignore` & `sentenai-1.7.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `sentenai-1.7.0.2/LICENSE` & `sentenai-1.7.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sentenai-1.7.0.2/PKG-INFO` & `sentenai-1.7.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentenai
-Version: 1.7.0.2
+Version: 1.7.1.1
 Summary: Client library for Sentenai
 Home-page: https://github.com/sentenai/py-sentenai
 Author: Sentenai, Inc.
 Author-email: info@sentenai.com
 License: BSD
 Keywords: sentenai cloud sensor database
 Platform: UNKNOWN
```

### Comparing `sentenai-1.7.0.2/README.md` & `sentenai-1.7.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sentenai-1.7.0.2/sentenai/__init__.py` & `sentenai-1.7.1.1/sentenai/__init__.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.7.0.2/sentenai/api.py` & `sentenai-1.7.1.1/sentenai/api.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.7.0.2/sentenai/stream/events.py` & `sentenai-1.7.1.1/sentenai/stream/events.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.7.0.2/sentenai/stream/metadata.py` & `sentenai-1.7.1.1/sentenai/stream/metadata.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.7.0.2/sentenai/stream/streams.py` & `sentenai-1.7.1.1/sentenai/stream/streams.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.7.0.2/sentenai/tests/streams/test_stream.py` & `sentenai-1.7.1.1/sentenai/tests/streams/test_stream.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.7.0.2/sentenai/tests/streams/test_stream.py-e` & `sentenai-1.7.1.1/sentenai/tests/streams/test_stream.py-e`

 * *Files identical despite different names*

### Comparing `sentenai-1.7.0.2/sentenai/tests/test_events.py` & `sentenai-1.7.1.1/sentenai/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.7.0.2/sentenai/tests/test_fields.py` & `sentenai-1.7.1.1/sentenai/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.7.0.2/sentenai/tests/test_streams.py` & `sentenai-1.7.1.1/sentenai/tests/test_streams.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.7.0.2/sentenai/tests/test_views.py` & `sentenai-1.7.1.1/sentenai/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.7.0.2/sentenai.egg-info/PKG-INFO` & `sentenai-1.7.1.1/sentenai.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentenai
-Version: 1.7.0.2
+Version: 1.7.1.1
 Summary: Client library for Sentenai
 Home-page: https://github.com/sentenai/py-sentenai
 Author: Sentenai, Inc.
 Author-email: info@sentenai.com
 License: BSD
 Keywords: sentenai cloud sensor database
 Platform: UNKNOWN
```

### Comparing `sentenai-1.7.0.2/sentenai.egg-info/SOURCES.txt` & `sentenai-1.7.1.1/sentenai.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 Makefile
 README.md
 requirements.txt
 setup.cfg
 setup.py
 sentenai/__init__.py
 sentenai/api.py
+sentenai/new.py
 sentenai.egg-info/PKG-INFO
 sentenai.egg-info/SOURCES.txt
 sentenai.egg-info/dependency_links.txt
 sentenai.egg-info/requires.txt
 sentenai.egg-info/top_level.txt
 sentenai/stream/__init__.py
 sentenai/stream/events.py
```

### Comparing `sentenai-1.7.0.2/setup.py` & `sentenai-1.7.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='sentenai',
-    version='1.7.0.2',
+    version='1.7.1.1',
     description='Client library for Sentenai',
     long_description="",
     url='https://github.com/sentenai/py-sentenai',
 
     author='Sentenai, Inc.',
     author_email='info@sentenai.com',
```

### Comparing `sentenai-1.7.0.2/tests/flare/test_ast.py` & `sentenai-1.7.1.1/tests/flare/test_ast.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.7.0.2/tests/flare/test_queries.py` & `sentenai-1.7.1.1/tests/flare/test_queries.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.7.0.2/tests/flare/test_stream_construction.py` & `sentenai-1.7.1.1/tests/flare/test_stream_construction.py`

 * *Files identical despite different names*

### Comparing `sentenai-1.7.0.2/tests/test_api.py` & `sentenai-1.7.1.1/tests/test_api.py`

 * *Files identical despite different names*

