# Comparing `tmp/database-common-tools-1.1.0.tar.gz` & `tmp/database-common-tools-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database-common-tools-1.1.0.tar", last modified: Wed Apr 17 03:14:53 2024, max compression
+gzip compressed data, was "database-common-tools-1.1.1.tar", last modified: Wed Apr 17 03:44:34 2024, max compression
```

## Comparing `database-common-tools-1.1.0.tar` & `database-common-tools-1.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-17 03:14:53.438090 database-common-tools-1.1.0/
--rw-r--r--   0 yangming   (501) staff       (20)     1066 2024-01-24 08:52:12.000000 database-common-tools-1.1.0/LICENSE
--rw-r--r--   0 yangming   (501) staff       (20)      701 2024-04-17 03:14:53.437644 database-common-tools-1.1.0/PKG-INFO
--rw-r--r--   0 yangming   (501) staff       (20)       23 2024-01-24 08:52:12.000000 database-common-tools-1.1.0/README.md
-drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-17 03:14:53.424377 database-common-tools-1.1.0/database_common_tools.egg-info/
--rw-r--r--   0 yangming   (501) staff       (20)      701 2024-04-17 03:14:53.000000 database-common-tools-1.1.0/database_common_tools.egg-info/PKG-INFO
--rw-r--r--   0 yangming   (501) staff       (20)      682 2024-04-17 03:14:53.000000 database-common-tools-1.1.0/database_common_tools.egg-info/SOURCES.txt
--rw-r--r--   0 yangming   (501) staff       (20)        1 2024-04-17 03:14:53.000000 database-common-tools-1.1.0/database_common_tools.egg-info/dependency_links.txt
--rw-r--r--   0 yangming   (501) staff       (20)       85 2024-04-17 03:14:53.000000 database-common-tools-1.1.0/database_common_tools.egg-info/requires.txt
--rw-r--r--   0 yangming   (501) staff       (20)       19 2024-04-17 03:14:53.000000 database-common-tools-1.1.0/database_common_tools.egg-info/top_level.txt
-drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-17 03:14:53.435905 database-common-tools-1.1.0/databasetools/
--rw-r--r--   0 yangming   (501) staff       (20)     1636 2024-01-25 08:25:09.000000 database-common-tools-1.1.0/databasetools/__init__.py
--rw-r--r--   0 yangming   (501) staff       (20)     1990 2024-01-24 09:06:09.000000 database-common-tools-1.1.0/databasetools/analysis_json.py
--rw-r--r--   0 yangming   (501) staff       (20)     2090 2024-04-16 11:58:05.000000 database-common-tools-1.1.0/databasetools/analysis_json_v2.py
--rw-r--r--   0 yangming   (501) staff       (20)     2508 2024-04-16 08:05:52.000000 database-common-tools-1.1.0/databasetools/analysis_json_v3.py
--rw-r--r--   0 yangming   (501) staff       (20)     3191 2024-01-24 09:06:09.000000 database-common-tools-1.1.0/databasetools/data_analysis.py
--rw-r--r--   0 yangming   (501) staff       (20)     3562 2024-04-16 12:39:11.000000 database-common-tools-1.1.0/databasetools/data_analysis_v2.py
--rw-r--r--   0 yangming   (501) staff       (20)     4515 2024-04-16 12:38:53.000000 database-common-tools-1.1.0/databasetools/data_analysis_v3.py
--rw-r--r--   0 yangming   (501) staff       (20)      331 2024-01-26 03:25:22.000000 database-common-tools-1.1.0/databasetools/kafka_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)     2180 2024-03-14 06:55:26.000000 database-common-tools-1.1.0/databasetools/mongo_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)      721 2024-01-26 07:55:44.000000 database-common-tools-1.1.0/databasetools/mt_wx_message.py
--rw-r--r--   0 yangming   (501) staff       (20)      279 2024-04-15 02:52:56.000000 database-common-tools-1.1.0/databasetools/mysql_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)     1047 2024-04-16 08:35:37.000000 database-common-tools-1.1.0/databasetools/opensearch_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)     5458 2024-01-26 08:31:58.000000 database-common-tools-1.1.0/databasetools/redis_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)       38 2024-04-17 03:14:53.438230 database-common-tools-1.1.0/setup.cfg
--rw-r--r--   0 yangming   (501) staff       (20)     3932 2024-04-16 12:00:01.000000 database-common-tools-1.1.0/setup.py
-drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-17 03:14:53.437163 database-common-tools-1.1.0/test/
--rw-r--r--   0 yangming   (501) staff       (20)        0 2024-01-26 07:51:53.000000 database-common-tools-1.1.0/test/__init__.py
+drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-17 03:44:34.867218 database-common-tools-1.1.1/
+-rw-r--r--   0 yangming   (501) staff       (20)     1066 2024-01-24 08:52:12.000000 database-common-tools-1.1.1/LICENSE
+-rw-r--r--   0 yangming   (501) staff       (20)      701 2024-04-17 03:44:34.866724 database-common-tools-1.1.1/PKG-INFO
+-rw-r--r--   0 yangming   (501) staff       (20)       23 2024-01-24 08:52:12.000000 database-common-tools-1.1.1/README.md
+drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-17 03:44:34.854309 database-common-tools-1.1.1/database_common_tools.egg-info/
+-rw-r--r--   0 yangming   (501) staff       (20)      701 2024-04-17 03:44:34.000000 database-common-tools-1.1.1/database_common_tools.egg-info/PKG-INFO
+-rw-r--r--   0 yangming   (501) staff       (20)      682 2024-04-17 03:44:34.000000 database-common-tools-1.1.1/database_common_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 yangming   (501) staff       (20)        1 2024-04-17 03:44:34.000000 database-common-tools-1.1.1/database_common_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 yangming   (501) staff       (20)       85 2024-04-17 03:44:34.000000 database-common-tools-1.1.1/database_common_tools.egg-info/requires.txt
+-rw-r--r--   0 yangming   (501) staff       (20)       19 2024-04-17 03:44:34.000000 database-common-tools-1.1.1/database_common_tools.egg-info/top_level.txt
+drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-17 03:44:34.865244 database-common-tools-1.1.1/databasetools/
+-rw-r--r--   0 yangming   (501) staff       (20)     1636 2024-01-25 08:25:09.000000 database-common-tools-1.1.1/databasetools/__init__.py
+-rw-r--r--   0 yangming   (501) staff       (20)     1990 2024-01-24 09:06:09.000000 database-common-tools-1.1.1/databasetools/analysis_json.py
+-rw-r--r--   0 yangming   (501) staff       (20)     2090 2024-04-16 11:58:05.000000 database-common-tools-1.1.1/databasetools/analysis_json_v2.py
+-rw-r--r--   0 yangming   (501) staff       (20)     2508 2024-04-16 08:05:52.000000 database-common-tools-1.1.1/databasetools/analysis_json_v3.py
+-rw-r--r--   0 yangming   (501) staff       (20)     3191 2024-01-24 09:06:09.000000 database-common-tools-1.1.1/databasetools/data_analysis.py
+-rw-r--r--   0 yangming   (501) staff       (20)     3562 2024-04-16 12:39:11.000000 database-common-tools-1.1.1/databasetools/data_analysis_v2.py
+-rw-r--r--   0 yangming   (501) staff       (20)     4515 2024-04-17 03:43:55.000000 database-common-tools-1.1.1/databasetools/data_analysis_v3.py
+-rw-r--r--   0 yangming   (501) staff       (20)      331 2024-01-26 03:25:22.000000 database-common-tools-1.1.1/databasetools/kafka_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)     2180 2024-03-14 06:55:26.000000 database-common-tools-1.1.1/databasetools/mongo_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)      721 2024-01-26 07:55:44.000000 database-common-tools-1.1.1/databasetools/mt_wx_message.py
+-rw-r--r--   0 yangming   (501) staff       (20)      279 2024-04-15 02:52:56.000000 database-common-tools-1.1.1/databasetools/mysql_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)     1047 2024-04-16 08:35:37.000000 database-common-tools-1.1.1/databasetools/opensearch_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)     5458 2024-01-26 08:31:58.000000 database-common-tools-1.1.1/databasetools/redis_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)       38 2024-04-17 03:44:34.867351 database-common-tools-1.1.1/setup.cfg
+-rw-r--r--   0 yangming   (501) staff       (20)     3932 2024-04-17 03:44:06.000000 database-common-tools-1.1.1/setup.py
+drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-17 03:44:34.866226 database-common-tools-1.1.1/test/
+-rw-r--r--   0 yangming   (501) staff       (20)        0 2024-01-26 07:51:53.000000 database-common-tools-1.1.1/test/__init__.py
```

### Comparing `database-common-tools-1.1.0/LICENSE` & `database-common-tools-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.0/PKG-INFO` & `database-common-tools-1.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-common-tools
-Version: 1.1.0
+Version: 1.1.1
 Summary: let message middleware and use database more easy
 Home-page: https://github.com/yangming9/database-common-tools.git
 Author: Coder Yang
 Author-email: yma91412@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `database-common-tools-1.1.0/database_common_tools.egg-info/PKG-INFO` & `database-common-tools-1.1.1/database_common_tools.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-common-tools
-Version: 1.1.0
+Version: 1.1.1
 Summary: let message middleware and use database more easy
 Home-page: https://github.com/yangming9/database-common-tools.git
 Author: Coder Yang
 Author-email: yma91412@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `database-common-tools-1.1.0/database_common_tools.egg-info/SOURCES.txt` & `database-common-tools-1.1.1/database_common_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.0/databasetools/__init__.py` & `database-common-tools-1.1.1/databasetools/__init__.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.0/databasetools/analysis_json.py` & `database-common-tools-1.1.1/databasetools/analysis_json.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.0/databasetools/analysis_json_v2.py` & `database-common-tools-1.1.1/databasetools/analysis_json_v2.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.0/databasetools/analysis_json_v3.py` & `database-common-tools-1.1.1/databasetools/analysis_json_v3.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.0/databasetools/data_analysis.py` & `database-common-tools-1.1.1/databasetools/data_analysis.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.0/databasetools/data_analysis_v2.py` & `database-common-tools-1.1.1/databasetools/data_analysis_v2.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.0/databasetools/data_analysis_v3.py` & `database-common-tools-1.1.1/databasetools/data_analysis_v3.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
                 elif FLD['types'][3] == _type:
                     # init field type2array
                     default_value = _map.get(FLD['names'][3], FLD['value'][1])
                     status, fieldValue = analysis_json_v2.dump_doc_field_type2array(srcDoc, path, default_value, _toType)
                     destDoc[_field] = fieldValue
                     if not status:
                         keyError = True
-                elif FLD['types'][3] == _type:
+                elif FLD['types'][4] == _type:
                     # init field toType
                     default_value = _map.get(FLD['names'][3], FLD['value'][0])
                     status, fieldValue = analysis_json_v2.dump_doc_field_type(srcDoc, path, default_value, _toType)
                     destDoc[_field] = fieldValue
                     if not status:
                         keyError = True
             else:
```

### Comparing `database-common-tools-1.1.0/databasetools/mongo_connect.py` & `database-common-tools-1.1.1/databasetools/mongo_connect.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.0/databasetools/mt_wx_message.py` & `database-common-tools-1.1.1/databasetools/mt_wx_message.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.0/databasetools/opensearch_connect.py` & `database-common-tools-1.1.1/databasetools/opensearch_connect.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.0/databasetools/redis_connect.py` & `database-common-tools-1.1.1/databasetools/redis_connect.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.1.0/setup.py` & `database-common-tools-1.1.1/setup.py`

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
-VERSION = '1.1.0'
+VERSION = '1.1.1'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests',
     'jsonpath',
     'pymongo',
     'redis',
```
