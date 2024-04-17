# Comparing `tmp/database-common-tools-1.0.9.tar.gz` & `tmp/database-common-tools-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database-common-tools-1.0.9.tar", last modified: Tue Apr 16 08:43:01 2024, max compression
+gzip compressed data, was "database-common-tools-1.1.0.tar", last modified: Wed Apr 17 03:14:53 2024, max compression
```

## Comparing `database-common-tools-1.0.9.tar` & `database-common-tools-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-16 08:43:01.265065 database-common-tools-1.0.9/
--rw-r--r--   0 yangming   (501) staff       (20)     1066 2024-01-24 08:52:12.000000 database-common-tools-1.0.9/LICENSE
--rw-r--r--   0 yangming   (501) staff       (20)      701 2024-04-16 08:43:01.264558 database-common-tools-1.0.9/PKG-INFO
--rw-r--r--   0 yangming   (501) staff       (20)       23 2024-01-24 08:52:12.000000 database-common-tools-1.0.9/README.md
-drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-16 08:43:01.247029 database-common-tools-1.0.9/database_common_tools.egg-info/
--rw-r--r--   0 yangming   (501) staff       (20)      701 2024-04-16 08:43:01.000000 database-common-tools-1.0.9/database_common_tools.egg-info/PKG-INFO
--rw-r--r--   0 yangming   (501) staff       (20)      682 2024-04-16 08:43:01.000000 database-common-tools-1.0.9/database_common_tools.egg-info/SOURCES.txt
--rw-r--r--   0 yangming   (501) staff       (20)        1 2024-04-16 08:43:01.000000 database-common-tools-1.0.9/database_common_tools.egg-info/dependency_links.txt
--rw-r--r--   0 yangming   (501) staff       (20)       85 2024-04-16 08:43:01.000000 database-common-tools-1.0.9/database_common_tools.egg-info/requires.txt
--rw-r--r--   0 yangming   (501) staff       (20)       19 2024-04-16 08:43:01.000000 database-common-tools-1.0.9/database_common_tools.egg-info/top_level.txt
-drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-16 08:43:01.263017 database-common-tools-1.0.9/databasetools/
--rw-r--r--   0 yangming   (501) staff       (20)     1636 2024-01-25 08:25:09.000000 database-common-tools-1.0.9/databasetools/__init__.py
--rw-r--r--   0 yangming   (501) staff       (20)     1990 2024-01-24 09:06:09.000000 database-common-tools-1.0.9/databasetools/analysis_json.py
--rw-r--r--   0 yangming   (501) staff       (20)     2090 2024-04-16 07:53:00.000000 database-common-tools-1.0.9/databasetools/analysis_json_v2.py
--rw-r--r--   0 yangming   (501) staff       (20)     2508 2024-04-16 08:05:52.000000 database-common-tools-1.0.9/databasetools/analysis_json_v3.py
--rw-r--r--   0 yangming   (501) staff       (20)     3191 2024-01-24 09:06:09.000000 database-common-tools-1.0.9/databasetools/data_analysis.py
--rw-r--r--   0 yangming   (501) staff       (20)     3564 2024-04-16 06:59:31.000000 database-common-tools-1.0.9/databasetools/data_analysis_v2.py
--rw-r--r--   0 yangming   (501) staff       (20)     4139 2024-04-16 08:04:03.000000 database-common-tools-1.0.9/databasetools/data_analysis_v3.py
--rw-r--r--   0 yangming   (501) staff       (20)      331 2024-01-26 03:25:22.000000 database-common-tools-1.0.9/databasetools/kafka_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)     2180 2024-03-14 06:55:26.000000 database-common-tools-1.0.9/databasetools/mongo_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)      721 2024-01-26 07:55:44.000000 database-common-tools-1.0.9/databasetools/mt_wx_message.py
--rw-r--r--   0 yangming   (501) staff       (20)      279 2024-04-15 02:52:56.000000 database-common-tools-1.0.9/databasetools/mysql_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)     1047 2024-04-16 08:35:37.000000 database-common-tools-1.0.9/databasetools/opensearch_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)     5458 2024-01-26 08:31:58.000000 database-common-tools-1.0.9/databasetools/redis_connect.py
--rw-r--r--   0 yangming   (501) staff       (20)       38 2024-04-16 08:43:01.265252 database-common-tools-1.0.9/setup.cfg
--rw-r--r--   0 yangming   (501) staff       (20)     3932 2024-04-16 08:42:52.000000 database-common-tools-1.0.9/setup.py
-drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-16 08:43:01.263973 database-common-tools-1.0.9/test/
--rw-r--r--   0 yangming   (501) staff       (20)        0 2024-01-26 07:51:53.000000 database-common-tools-1.0.9/test/__init__.py
+drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-17 03:14:53.438090 database-common-tools-1.1.0/
+-rw-r--r--   0 yangming   (501) staff       (20)     1066 2024-01-24 08:52:12.000000 database-common-tools-1.1.0/LICENSE
+-rw-r--r--   0 yangming   (501) staff       (20)      701 2024-04-17 03:14:53.437644 database-common-tools-1.1.0/PKG-INFO
+-rw-r--r--   0 yangming   (501) staff       (20)       23 2024-01-24 08:52:12.000000 database-common-tools-1.1.0/README.md
+drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-17 03:14:53.424377 database-common-tools-1.1.0/database_common_tools.egg-info/
+-rw-r--r--   0 yangming   (501) staff       (20)      701 2024-04-17 03:14:53.000000 database-common-tools-1.1.0/database_common_tools.egg-info/PKG-INFO
+-rw-r--r--   0 yangming   (501) staff       (20)      682 2024-04-17 03:14:53.000000 database-common-tools-1.1.0/database_common_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 yangming   (501) staff       (20)        1 2024-04-17 03:14:53.000000 database-common-tools-1.1.0/database_common_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 yangming   (501) staff       (20)       85 2024-04-17 03:14:53.000000 database-common-tools-1.1.0/database_common_tools.egg-info/requires.txt
+-rw-r--r--   0 yangming   (501) staff       (20)       19 2024-04-17 03:14:53.000000 database-common-tools-1.1.0/database_common_tools.egg-info/top_level.txt
+drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-17 03:14:53.435905 database-common-tools-1.1.0/databasetools/
+-rw-r--r--   0 yangming   (501) staff       (20)     1636 2024-01-25 08:25:09.000000 database-common-tools-1.1.0/databasetools/__init__.py
+-rw-r--r--   0 yangming   (501) staff       (20)     1990 2024-01-24 09:06:09.000000 database-common-tools-1.1.0/databasetools/analysis_json.py
+-rw-r--r--   0 yangming   (501) staff       (20)     2090 2024-04-16 11:58:05.000000 database-common-tools-1.1.0/databasetools/analysis_json_v2.py
+-rw-r--r--   0 yangming   (501) staff       (20)     2508 2024-04-16 08:05:52.000000 database-common-tools-1.1.0/databasetools/analysis_json_v3.py
+-rw-r--r--   0 yangming   (501) staff       (20)     3191 2024-01-24 09:06:09.000000 database-common-tools-1.1.0/databasetools/data_analysis.py
+-rw-r--r--   0 yangming   (501) staff       (20)     3562 2024-04-16 12:39:11.000000 database-common-tools-1.1.0/databasetools/data_analysis_v2.py
+-rw-r--r--   0 yangming   (501) staff       (20)     4515 2024-04-16 12:38:53.000000 database-common-tools-1.1.0/databasetools/data_analysis_v3.py
+-rw-r--r--   0 yangming   (501) staff       (20)      331 2024-01-26 03:25:22.000000 database-common-tools-1.1.0/databasetools/kafka_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)     2180 2024-03-14 06:55:26.000000 database-common-tools-1.1.0/databasetools/mongo_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)      721 2024-01-26 07:55:44.000000 database-common-tools-1.1.0/databasetools/mt_wx_message.py
+-rw-r--r--   0 yangming   (501) staff       (20)      279 2024-04-15 02:52:56.000000 database-common-tools-1.1.0/databasetools/mysql_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)     1047 2024-04-16 08:35:37.000000 database-common-tools-1.1.0/databasetools/opensearch_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)     5458 2024-01-26 08:31:58.000000 database-common-tools-1.1.0/databasetools/redis_connect.py
+-rw-r--r--   0 yangming   (501) staff       (20)       38 2024-04-17 03:14:53.438230 database-common-tools-1.1.0/setup.cfg
+-rw-r--r--   0 yangming   (501) staff       (20)     3932 2024-04-16 12:00:01.000000 database-common-tools-1.1.0/setup.py
+drwxr-xr-x   0 yangming   (501) staff       (20)        0 2024-04-17 03:14:53.437163 database-common-tools-1.1.0/test/
+-rw-r--r--   0 yangming   (501) staff       (20)        0 2024-01-26 07:51:53.000000 database-common-tools-1.1.0/test/__init__.py
```

### Comparing `database-common-tools-1.0.9/LICENSE` & `database-common-tools-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.9/PKG-INFO` & `database-common-tools-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-common-tools
-Version: 1.0.9
+Version: 1.1.0
 Summary: let message middleware and use database more easy
 Home-page: https://github.com/yangming9/database-common-tools.git
 Author: Coder Yang
 Author-email: yma91412@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `database-common-tools-1.0.9/database_common_tools.egg-info/PKG-INFO` & `database-common-tools-1.1.0/database_common_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-common-tools
-Version: 1.0.9
+Version: 1.1.0
 Summary: let message middleware and use database more easy
 Home-page: https://github.com/yangming9/database-common-tools.git
 Author: Coder Yang
 Author-email: yma91412@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `database-common-tools-1.0.9/database_common_tools.egg-info/SOURCES.txt` & `database-common-tools-1.1.0/database_common_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.9/databasetools/__init__.py` & `database-common-tools-1.1.0/databasetools/__init__.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.9/databasetools/analysis_json.py` & `database-common-tools-1.1.0/databasetools/analysis_json.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.9/databasetools/analysis_json_v2.py` & `database-common-tools-1.1.0/databasetools/analysis_json_v2.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.9/databasetools/analysis_json_v3.py` & `database-common-tools-1.1.0/databasetools/analysis_json_v3.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.9/databasetools/data_analysis.py` & `database-common-tools-1.1.0/databasetools/data_analysis.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.9/databasetools/data_analysis_v2.py` & `database-common-tools-1.1.0/databasetools/data_analysis_v2.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,16 +67,16 @@
                     # init field object
                     default_value = _map.get(FLD['names'][3], FLD['value'][2])
                     status, fieldValue = analysis_json_v2.dump_doc_field_object(srcDoc, path, default_value)
                     destDoc[_field] = fieldValue
                     if not status:
                         keyError = True
                 elif FLD['types'][3] == _type:
-                    # init field string2array
-                    default_value = _map.get(FLD['names'][3], FLD['value'][3])
+                    # init field type2array
+                    default_value = _map.get(FLD['names'][3], FLD['value'][1])
                     status, fieldValue = analysis_json_v2.dump_doc_field_type2array(srcDoc, path, default_value, _toType)
                     destDoc[_field] = fieldValue
                     if not status:
                         keyError = True
             else:
                 mapConfigFlag = False
         if not necessity and keyError:
```

### Comparing `database-common-tools-1.0.9/databasetools/data_analysis_v3.py` & `database-common-tools-1.1.0/databasetools/data_analysis_v3.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 ##################################################
 FLD = dict()
 FLD['names'] = list()
 FLD['names'].append('necessity')    # 0
 FLD['names'].append('path')         # 1
 FLD['names'].append('type')         # 2
 FLD['names'].append('default')      # 3
-FLD['names'].append('toArrayType')  # 4
-FLD['names'].append('toType')       # 5
+FLD['names'].append('toType')       # 4
 
 FLD['types'] = list()
 FLD['types'].append('string')         # 0
 FLD['types'].append('array')          # 1
 FLD['types'].append('object')         # 2
 FLD['types'].append('type2array')     # 3
 FLD['types'].append('toType')         # 4
@@ -30,14 +29,29 @@
 FLD['data_type'].append(int)         # 0
 FLD['data_type'].append(float)       # 1
 FLD['data_type'].append(str)         # 2
 FLD['data_type'].append(list)        # 3
 
 
 ##################################################
+# common function
+##################################################
+def getDataType(_type):
+    if isinstance(_type, str):
+        if _type == 'int':
+            return FLD['data_type'][0]
+        if _type == 'float':
+            return FLD['data_type'][1]
+        if _type == 'str':
+            return FLD['data_type'][2]
+        if _type == 'list':
+            return FLD['data_type'][3]
+        
+
+##################################################
 # src to dest doc analysis
 ##################################################
 # mapConfigFlag mapping配置标志 false 错误
 # fieldError 数据传输错误，缺少必要字段  true 错误
 def doc_fields_analysis(srcDoc, destDoc, _mapping):
     mapConfigFlag = False
     errorKeys = list()
@@ -45,16 +59,16 @@
     for _field, _map in _mapping.items():
         mapConfigFlag = True
         keyError = False
         necessity = _map.get(FLD['names'][0], False)
         if isinstance(_map, dict):
             path = _map.get(FLD['names'][1], None)
             _type = _map.get(FLD['names'][2], FLD['types'][0])
-            _toArrayType = _map.get(FLD['names'][4], FLD['data_type'][2])
-            _toType = _map.get(FLD['names'][5], FLD['data_type'][2])
+            _toType = _map.get(FLD['names'][4], FLD['data_type'][2])
+            _toType = getDataType(_toType)
             if path:
                 if FLD['types'][0] == _type:
                     # init string
                     default_value = _map.get(FLD['names'][3], FLD['value'][0])
                     status, fieldValue = analysis_json_v2.dump_doc_field_str(srcDoc, path, default_value)
                     destDoc[_field] = fieldValue
                     if not status:
@@ -71,22 +85,22 @@
                     default_value = _map.get(FLD['names'][3], FLD['value'][2])
                     status, fieldValue = analysis_json_v2.dump_doc_field_object(srcDoc, path, default_value)
                     destDoc[_field] = fieldValue
                     if not status:
                         keyError = True
                 elif FLD['types'][3] == _type:
                     # init field type2array
-                    default_value = _map.get(FLD['names'][3], FLD['value'][3])
-                    status, fieldValue = analysis_json_v2.dump_doc_field_type2array(srcDoc, path, default_value, _toArrayType)
+                    default_value = _map.get(FLD['names'][3], FLD['value'][1])
+                    status, fieldValue = analysis_json_v2.dump_doc_field_type2array(srcDoc, path, default_value, _toType)
                     destDoc[_field] = fieldValue
                     if not status:
                         keyError = True
                 elif FLD['types'][3] == _type:
                     # init field toType
-                    default_value = _map.get(FLD['names'][3], FLD['value'][4])
+                    default_value = _map.get(FLD['names'][3], FLD['value'][0])
                     status, fieldValue = analysis_json_v2.dump_doc_field_type(srcDoc, path, default_value, _toType)
                     destDoc[_field] = fieldValue
                     if not status:
                         keyError = True
             else:
                 mapConfigFlag = False
         if not necessity and keyError:
```

### Comparing `database-common-tools-1.0.9/databasetools/mongo_connect.py` & `database-common-tools-1.1.0/databasetools/mongo_connect.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.9/databasetools/mt_wx_message.py` & `database-common-tools-1.1.0/databasetools/mt_wx_message.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.9/databasetools/opensearch_connect.py` & `database-common-tools-1.1.0/databasetools/opensearch_connect.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.9/databasetools/redis_connect.py` & `database-common-tools-1.1.0/databasetools/redis_connect.py`

 * *Files identical despite different names*

### Comparing `database-common-tools-1.0.9/setup.py` & `database-common-tools-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'database-common-tools'
 DESCRIPTION = 'let message middleware and use database more easy'
 URL = 'https://github.com/yangming9/database-common-tools.git'
 EMAIL = 'yma91412@gmail.com'
 AUTHOR = 'Coder Yang'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '1.0.9'
+VERSION = '1.1.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests',
     'jsonpath',
     'pymongo',
     'redis',
```

