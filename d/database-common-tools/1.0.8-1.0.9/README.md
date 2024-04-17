# Comparing `tmp/database-common-tools-1.0.8.tar.gz` & `tmp/database-common-tools-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database-common-tools-1.0.8.tar", last modified: Tue Apr 16 08:07:36 2024, max compression
+gzip compressed data, was "database-common-tools-1.0.9.tar", last modified: Tue Apr 16 08:43:01 2024, max compression
```

## Comparing `database-common-tools-1.0.8.tar` & `database-common-tools-1.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-16 08:07:36.454096 database-common-tools-1.0.8/
--rw-r--r--   0 yangming   (501) staff       (20)     1066 2024-01-24 08:52:12.000000 database-common-tools-1.0.8/LICENSE
--rw-r--r--   0 yangming   (501) staff       (20)      701 2024-04-16 08:07:36.453375 database-common-tools-1.0.8/PKG-INFO
--rw-r--r--   0 yangming   (501) staff       (20)       23 2024-01-24 08:52:12.000000 database-common-tools-1.0.8/README.md
-drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-16 08:07:36.440513 database-common-tools-1.0.8/database_common_tools.egg-info/
--rw-r--r--   0 yangming   (501) staff       (20)      701 2024-04-16 08:07:36.000000 database-common-tools-1.0.8/database_common_tools.egg-info/PKG-INFO
--rw-r--r--   0 yangming   (501) staff       (20)      682 2024-04-16 08:07:36.000000 database-common-tools-1.0.8/database_common_tools.egg-info/SOURCES.txt
--rw-r--r--   0 yangming   (501) staff       (20)        1 2024-04-16 08:07:36.000000 database-common-tools-1.0.8/database_common_tools.egg-info/dependency_links.txt
--rw-r--r--   0 yangming   (501) staff       (20)       85 2024-04-16 08:07:36.000000 database-common-tools-1.0.8/database_common_tools.egg-info/requires.txt
--rw-r--r--   0 yangming   (501) staff       (20)       19 2024-04-16 08:07:36.000000 database-common-tools-1.0.8/database_common_tools.egg-info/top_level.txt
-drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-16 08:07:36.451751 database-common-tools-1.0.8/databasetools/
--rw-r--r--   0 yangming   (501) staff       (20)     1636 2024-01-25 08:25:09.000000 database-common-tools-1.0.8/databasetools/__init__.py
--rw-r--r--   0 yangming   (501) staff       (20)     1990 2024-01-24 09:06:09.000000 database-common-tools-1.0.8/databasetools/analysis_json.py
--rw-r--r--   0 yangming   (501) staff       (20)     2090 2024-04-16 07:53:00.000000 database-common-tools-1.0.8/databasetools/analysis_json_v2.py
--rw-r--r--   0 yangming   (501) staff       (20)     2508 2024-04-16 08:05:52.000000 database-common-tools-1.0.8/databasetools/analysis_json_v3.py
--rw-r--r--   0 yangming   (501) staff       (20)     3191 2024-01-24 09:06:09.000000 database-common-tools-1.0.8/databasetools/data_analysis.py
--rw-r--r--   0 yangming   (501) staff       (20)     3564 2024-04-16 06:59:31.000000 database-common-tools-1.0.8/databasetools/data_analysis_v2.py
--rw-r--r--   0 yangming   (501) staff       (20)     4139 2024-04-16 08:04:03.000000 database-common-tools-1.0.8/databasetools/data_analysis_v3.py
--rw-r--r--   0 yangming   (501) staff       (20)      331 2024-01-26 03:25:22.000000 database-common-tools-1.0.8/databasetools/kafka_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)     2180 2024-03-14 06:55:26.000000 database-common-tools-1.0.8/databasetools/mongo_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)      721 2024-01-26 07:55:44.000000 database-common-tools-1.0.8/databasetools/mt_wx_message.py
--rw-r--r--   0 yangming   (501) staff       (20)      279 2024-04-15 02:52:56.000000 database-common-tools-1.0.8/databasetools/mysql_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)      939 2024-04-16 06:15:02.000000 database-common-tools-1.0.8/databasetools/opensearch_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)     5458 2024-01-26 08:31:58.000000 database-common-tools-1.0.8/databasetools/redis_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)       38 2024-04-16 08:07:36.454308 database-common-tools-1.0.8/setup.cfg
--rw-r--r--   0 yangming   (501) staff       (20)     3932 2024-04-16 04:01:08.000000 database-common-tools-1.0.8/setup.py
-drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-16 08:07:36.452775 database-common-tools-1.0.8/test/
--rw-r--r--   0 yangming   (501) staff       (20)        0 2024-01-26 07:51:53.000000 database-common-tools-1.0.8/test/__init__.py
+drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-16 08:43:01.265065 database-common-tools-1.0.9/
+-rw-r--r--   0 yangming   (501) staff       (20)     1066 2024-01-24 08:52:12.000000 database-common-tools-1.0.9/LICENSE
+-rw-r--r--   0 yangming   (501) staff       (20)      701 2024-04-16 08:43:01.264558 database-common-tools-1.0.9/PKG-INFO
+-rw-r--r--   0 yangming   (501) staff       (20)       23 2024-01-24 08:52:12.000000 database-common-tools-1.0.9/README.md
+drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-16 08:43:01.247029 database-common-tools-1.0.9/database_common_tools.egg-info/
+-rw-r--r--   0 yangming   (501) staff       (20)      701 2024-04-16 08:43:01.000000 database-common-tools-1.0.9/database_common_tools.egg-info/PKG-INFO
+-rw-r--r--   0 yangming   (501) staff       (20)      682 2024-04-16 08:43:01.000000 database-common-tools-1.0.9/database_common_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 yangming   (501) staff       (20)        1 2024-04-16 08:43:01.000000 database-common-tools-1.0.9/database_common_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 yangming   (501) staff       (20)       85 2024-04-16 08:43:01.000000 database-common-tools-1.0.9/database_common_tools.egg-info/requires.txt
+-rw-r--r--   0 yangming   (501) staff       (20)       19 2024-04-16 08:43:01.000000 database-common-tools-1.0.9/database_common_tools.egg-info/top_level.txt
+drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-16 08:43:01.263017 database-common-tools-1.0.9/databasetools/
+-rw-r--r--   0 yangming   (501) staff       (20)     1636 2024-01-25 08:25:09.000000 database-common-tools-1.0.9/databasetools/__init__.py
+-rw-r--r--   0 yangming   (501) staff       (20)     1990 2024-01-24 09:06:09.000000 database-common-tools-1.0.9/databasetools/analysis_json.py
+-rw-r--r--   0 yangming   (501) staff       (20)     2090 2024-04-16 07:53:00.000000 database-common-tools-1.0.9/databasetools/analysis_json_v2.py
+-rw-r--r--   0 yangming   (501) staff       (20)     2508 2024-04-16 08:05:52.000000 database-common-tools-1.0.9/databasetools/analysis_json_v3.py
+-rw-r--r--   0 yangming   (501) staff       (20)     3191 2024-01-24 09:06:09.000000 database-common-tools-1.0.9/databasetools/data_analysis.py
+-rw-r--r--   0 yangming   (501) staff       (20)     3564 2024-04-16 06:59:31.000000 database-common-tools-1.0.9/databasetools/data_analysis_v2.py
+-rw-r--r--   0 yangming   (501) staff       (20)     4139 2024-04-16 08:04:03.000000 database-common-tools-1.0.9/databasetools/data_analysis_v3.py
+-rw-r--r--   0 yangming   (501) staff       (20)      331 2024-01-26 03:25:22.000000 database-common-tools-1.0.9/databasetools/kafka_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)     2180 2024-03-14 06:55:26.000000 database-common-tools-1.0.9/databasetools/mongo_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)      721 2024-01-26 07:55:44.000000 database-common-tools-1.0.9/databasetools/mt_wx_message.py
+-rw-r--r--   0 yangming   (501) staff       (20)      279 2024-04-15 02:52:56.000000 database-common-tools-1.0.9/databasetools/mysql_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)     1047 2024-04-16 08:35:37.000000 database-common-tools-1.0.9/databasetools/opensearch_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)     5458 2024-01-26 08:31:58.000000 database-common-tools-1.0.9/databasetools/redis_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)       38 2024-04-16 08:43:01.265252 database-common-tools-1.0.9/setup.cfg
+-rw-r--r--   0 yangming   (501) staff       (20)     3932 2024-04-16 08:42:52.000000 database-common-tools-1.0.9/setup.py
+drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-16 08:43:01.263973 database-common-tools-1.0.9/test/
+-rw-r--r--   0 yangming   (501) staff       (20)        0 2024-01-26 07:51:53.000000 database-common-tools-1.0.9/test/__init__.py
```

### Comparing `database-common-tools-1.0.8/LICENSE` & `database-common-tools-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.8/PKG-INFO` & `database-common-tools-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-common-tools
-Version: 1.0.8
+Version: 1.0.9
 Summary: let message middleware and use database more easy
 Home-page: https://github.com/yangming9/database-common-tools.git
 Author: Coder Yang
 Author-email: yma91412@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `database-common-tools-1.0.8/database_common_tools.egg-info/PKG-INFO` & `database-common-tools-1.0.9/database_common_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-common-tools
-Version: 1.0.8
+Version: 1.0.9
 Summary: let message middleware and use database more easy
 Home-page: https://github.com/yangming9/database-common-tools.git
 Author: Coder Yang
 Author-email: yma91412@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `database-common-tools-1.0.8/database_common_tools.egg-info/SOURCES.txt` & `database-common-tools-1.0.9/database_common_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.8/databasetools/__init__.py` & `database-common-tools-1.0.9/databasetools/__init__.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.8/databasetools/analysis_json.py` & `database-common-tools-1.0.9/databasetools/analysis_json.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.8/databasetools/analysis_json_v2.py` & `database-common-tools-1.0.9/databasetools/analysis_json_v2.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.8/databasetools/analysis_json_v3.py` & `database-common-tools-1.0.9/databasetools/analysis_json_v3.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.8/databasetools/data_analysis.py` & `database-common-tools-1.0.9/databasetools/data_analysis.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.8/databasetools/data_analysis_v2.py` & `database-common-tools-1.0.9/databasetools/data_analysis_v2.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.8/databasetools/data_analysis_v3.py` & `database-common-tools-1.0.9/databasetools/data_analysis_v3.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.8/databasetools/mongo_connect.py` & `database-common-tools-1.0.9/databasetools/mongo_connect.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.8/databasetools/mt_wx_message.py` & `database-common-tools-1.0.9/databasetools/mt_wx_message.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.8/databasetools/opensearch_connect.py` & `database-common-tools-1.0.9/databasetools/opensearch_connect.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from concurrent.futures import ThreadPoolExecutor, wait
 from elasticsearch import Elasticsearch
 from elasticsearch import helpers
 
 # 构建es客户端对象
-def create_client(endpoint):
-    return Elasticsearch(endpoint)
+def create_client(hosts,port):
+    addrs = []
+    for host in hosts:
+        addr = {'host': host, 'port': port}
+        addrs.append(addr)
+    return Elasticsearch(addrs)
 
 # es索引是否存在
 def index_exists(es, index_name):
     return es.indices.exists(index=index_name)
 
 # 创建索引
 def create_index(es, index_name, mapping):
```

### Comparing `database-common-tools-1.0.8/databasetools/redis_connect.py` & `database-common-tools-1.0.9/databasetools/redis_connect.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.8/setup.py` & `database-common-tools-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'database-common-tools'
 DESCRIPTION = 'let message middleware and use database more easy'
 URL = 'https://github.com/yangming9/database-common-tools.git'
 EMAIL = 'yma91412@gmail.com'
 AUTHOR = 'Coder Yang'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '1.0.8'
+VERSION = '1.0.9'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests',
     'jsonpath',
     'pymongo',
     'redis',
```

