# Comparing `tmp/suql-1.1.4a1.tar.gz` & `tmp/suql-1.1.4a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suql-1.1.4a1.tar", last modified: Wed Apr 17 07:37:32 2024, max compression
+gzip compressed data, was "suql-1.1.4a2.tar", last modified: Wed Apr 17 07:42:03 2024, max compression
```

## Comparing `suql-1.1.4a1.tar` & `suql-1.1.4a2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwx------   0 oval      (1000) users      (100)        0 2024-04-17 07:37:32.890176 suql-1.1.4a1/
--rw-------   0 oval      (1000) users      (100)    11356 2024-04-03 06:02:28.000000 suql-1.1.4a1/LICENSE
--rw-------   0 oval      (1000) users      (100)     4884 2024-04-17 07:37:32.890176 suql-1.1.4a1/PKG-INFO
--rw-------   0 oval      (1000) users      (100)     4278 2024-04-15 19:06:57.000000 suql-1.1.4a1/README.md
--rw-------   0 oval      (1000) users      (100)       38 2024-04-17 07:37:32.890176 suql-1.1.4a1/setup.cfg
--rw-------   0 oval      (1000) users      (100)     1514 2024-04-17 07:36:37.000000 suql-1.1.4a1/setup.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-17 07:37:32.886176 suql-1.1.4a1/src/
-drwx------   0 oval      (1000) users      (100)        0 2024-04-17 07:37:32.886176 suql-1.1.4a1/src/suql/
--rw-------   0 oval      (1000) users      (100)       73 2024-04-03 06:02:28.000000 suql-1.1.4a1/src/suql/__init__.py
--rw-------   0 oval      (1000) users      (100)    17354 2024-04-07 06:37:06.000000 suql-1.1.4a1/src/suql/agent.py
--rw-------   0 oval      (1000) users      (100)    16980 2024-04-17 07:37:16.000000 suql-1.1.4a1/src/suql/faiss_embedding.py
--rw-------   0 oval      (1000) users      (100)     8792 2024-04-17 07:27:02.000000 suql-1.1.4a1/src/suql/free_text_fcns_server.py
--rw-------   0 oval      (1000) users      (100)     3591 2024-04-12 01:45:49.000000 suql-1.1.4a1/src/suql/postgresql_connection.py
--rw-------   0 oval      (1000) users      (100)     9642 2024-04-12 01:46:33.000000 suql-1.1.4a1/src/suql/prompt_continuation.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-17 07:37:32.890176 suql-1.1.4a1/src/suql/prompts/
--rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:18.000000 suql-1.1.4a1/src/suql/prompts/__init__.py
--rw-------   0 oval      (1000) users      (100)      169 2024-04-03 06:02:28.000000 suql-1.1.4a1/src/suql/prompts/answer_qa.prompt
--rw-------   0 oval      (1000) users      (100)      451 2024-04-03 06:02:28.000000 suql-1.1.4a1/src/suql/prompts/field_classification.prompt
--rw-------   0 oval      (1000) users      (100)     2945 2024-04-03 06:02:28.000000 suql-1.1.4a1/src/suql/prompts/if_db_classification.prompt
--rw-------   0 oval      (1000) users      (100)     1305 2024-04-03 06:02:28.000000 suql-1.1.4a1/src/suql/prompts/opening_hours.prompt
--rw-------   0 oval      (1000) users      (100)     5574 2024-04-03 06:02:28.000000 suql-1.1.4a1/src/suql/prompts/parser_suql.prompt
--rw-------   0 oval      (1000) users      (100)      227 2024-04-03 06:02:28.000000 suql-1.1.4a1/src/suql/prompts/verification.prompt
--rw-------   0 oval      (1000) users      (100)     2983 2024-04-03 06:02:28.000000 suql-1.1.4a1/src/suql/prompts/yelp_response_SQL.prompt
--rw-------   0 oval      (1000) users      (100)     1454 2024-04-03 06:02:28.000000 suql-1.1.4a1/src/suql/prompts/yelp_response_no_results.prompt
-drwx------   0 oval      (1000) users      (100)        0 2024-04-17 07:37:32.890176 suql-1.1.4a1/src/suql/sql_free_text_support/
--rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:11.000000 suql-1.1.4a1/src/suql/sql_free_text_support/__init__.py
--rw-------   0 oval      (1000) users      (100)    64753 2024-04-17 07:35:47.000000 suql-1.1.4a1/src/suql/sql_free_text_support/execute_free_text_sql.py
--rw-------   0 oval      (1000) users      (100)     6455 2024-04-03 06:02:28.000000 suql-1.1.4a1/src/suql/utils.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-17 07:37:32.886176 suql-1.1.4a1/src/suql.egg-info/
--rw-r--r--   0 oval      (1000) users      (100)     4884 2024-04-17 07:37:32.000000 suql-1.1.4a1/src/suql.egg-info/PKG-INFO
--rw-------   0 oval      (1000) users      (100)      824 2024-04-17 07:37:32.000000 suql-1.1.4a1/src/suql.egg-info/SOURCES.txt
--rw-------   0 oval      (1000) users      (100)        1 2024-04-17 07:37:32.000000 suql-1.1.4a1/src/suql.egg-info/dependency_links.txt
--rw-------   0 oval      (1000) users      (100)      186 2024-04-17 07:37:32.000000 suql-1.1.4a1/src/suql.egg-info/requires.txt
--rw-------   0 oval      (1000) users      (100)        5 2024-04-17 07:37:32.000000 suql-1.1.4a1/src/suql.egg-info/top_level.txt
+drwx------   0 oval      (1000) users      (100)        0 2024-04-17 07:42:03.965490 suql-1.1.4a2/
+-rw-------   0 oval      (1000) users      (100)    11356 2024-04-03 06:02:28.000000 suql-1.1.4a2/LICENSE
+-rw-------   0 oval      (1000) users      (100)     4884 2024-04-17 07:42:03.965490 suql-1.1.4a2/PKG-INFO
+-rw-------   0 oval      (1000) users      (100)     4278 2024-04-15 19:06:57.000000 suql-1.1.4a2/README.md
+-rw-------   0 oval      (1000) users      (100)       38 2024-04-17 07:42:03.965490 suql-1.1.4a2/setup.cfg
+-rw-------   0 oval      (1000) users      (100)     1514 2024-04-17 07:40:52.000000 suql-1.1.4a2/setup.py
+drwx------   0 oval      (1000) users      (100)        0 2024-04-17 07:42:03.961490 suql-1.1.4a2/src/
+drwx------   0 oval      (1000) users      (100)        0 2024-04-17 07:42:03.961490 suql-1.1.4a2/src/suql/
+-rw-------   0 oval      (1000) users      (100)       73 2024-04-03 06:02:28.000000 suql-1.1.4a2/src/suql/__init__.py
+-rw-------   0 oval      (1000) users      (100)    17354 2024-04-07 06:37:06.000000 suql-1.1.4a2/src/suql/agent.py
+-rw-------   0 oval      (1000) users      (100)    16980 2024-04-17 07:37:16.000000 suql-1.1.4a2/src/suql/faiss_embedding.py
+-rw-------   0 oval      (1000) users      (100)     8792 2024-04-17 07:27:02.000000 suql-1.1.4a2/src/suql/free_text_fcns_server.py
+-rw-------   0 oval      (1000) users      (100)     3591 2024-04-12 01:45:49.000000 suql-1.1.4a2/src/suql/postgresql_connection.py
+-rw-------   0 oval      (1000) users      (100)     9642 2024-04-12 01:46:33.000000 suql-1.1.4a2/src/suql/prompt_continuation.py
+drwx------   0 oval      (1000) users      (100)        0 2024-04-17 07:42:03.961490 suql-1.1.4a2/src/suql/prompts/
+-rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:18.000000 suql-1.1.4a2/src/suql/prompts/__init__.py
+-rw-------   0 oval      (1000) users      (100)      169 2024-04-03 06:02:28.000000 suql-1.1.4a2/src/suql/prompts/answer_qa.prompt
+-rw-------   0 oval      (1000) users      (100)      451 2024-04-03 06:02:28.000000 suql-1.1.4a2/src/suql/prompts/field_classification.prompt
+-rw-------   0 oval      (1000) users      (100)     2945 2024-04-03 06:02:28.000000 suql-1.1.4a2/src/suql/prompts/if_db_classification.prompt
+-rw-------   0 oval      (1000) users      (100)     1305 2024-04-03 06:02:28.000000 suql-1.1.4a2/src/suql/prompts/opening_hours.prompt
+-rw-------   0 oval      (1000) users      (100)     5574 2024-04-03 06:02:28.000000 suql-1.1.4a2/src/suql/prompts/parser_suql.prompt
+-rw-------   0 oval      (1000) users      (100)      227 2024-04-03 06:02:28.000000 suql-1.1.4a2/src/suql/prompts/verification.prompt
+-rw-------   0 oval      (1000) users      (100)     2983 2024-04-03 06:02:28.000000 suql-1.1.4a2/src/suql/prompts/yelp_response_SQL.prompt
+-rw-------   0 oval      (1000) users      (100)     1454 2024-04-03 06:02:28.000000 suql-1.1.4a2/src/suql/prompts/yelp_response_no_results.prompt
+drwx------   0 oval      (1000) users      (100)        0 2024-04-17 07:42:03.965490 suql-1.1.4a2/src/suql/sql_free_text_support/
+-rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:11.000000 suql-1.1.4a2/src/suql/sql_free_text_support/__init__.py
+-rw-------   0 oval      (1000) users      (100)    64761 2024-04-17 07:40:44.000000 suql-1.1.4a2/src/suql/sql_free_text_support/execute_free_text_sql.py
+-rw-------   0 oval      (1000) users      (100)     6455 2024-04-03 06:02:28.000000 suql-1.1.4a2/src/suql/utils.py
+drwx------   0 oval      (1000) users      (100)        0 2024-04-17 07:42:03.961490 suql-1.1.4a2/src/suql.egg-info/
+-rw-r--r--   0 oval      (1000) users      (100)     4884 2024-04-17 07:42:03.000000 suql-1.1.4a2/src/suql.egg-info/PKG-INFO
+-rw-------   0 oval      (1000) users      (100)      824 2024-04-17 07:42:03.000000 suql-1.1.4a2/src/suql.egg-info/SOURCES.txt
+-rw-------   0 oval      (1000) users      (100)        1 2024-04-17 07:42:03.000000 suql-1.1.4a2/src/suql.egg-info/dependency_links.txt
+-rw-------   0 oval      (1000) users      (100)      186 2024-04-17 07:42:03.000000 suql-1.1.4a2/src/suql.egg-info/requires.txt
+-rw-------   0 oval      (1000) users      (100)        5 2024-04-17 07:42:03.000000 suql-1.1.4a2/src/suql.egg-info/top_level.txt
```

### Comparing `suql-1.1.4a1/LICENSE` & `suql-1.1.4a2/LICENSE`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a1/PKG-INFO` & `suql-1.1.4a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suql
-Version: 1.1.4a1
+Version: 1.1.4a2
 Summary: Structured and Unstructured Query Language (SUQL) Python API
 Home-page: https://github.com/stanford-oval/suql
 Author: Shicheng Liu
 Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: suql Version: 1.1.4a1 Summary: Structured and
+Metadata-Version: 2.1 Name: suql Version: 1.1.4a2 Summary: Structured and
 Unstructured Query Language (SUQL) Python API Home-page: https://github.com/
 stanford-oval/suql Author: Shicheng Liu Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `suql-1.1.4a1/README.md` & `suql-1.1.4a2/README.md`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a1/setup.py` & `suql-1.1.4a2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 # Package metadata
 name = "suql"
-version = "1.1.4a1"
+version = "1.1.4a2"
 description = "Structured and Unstructured Query Language (SUQL) Python API"
 author = "Shicheng Liu"
 author_email = "shicheng@cs.stanford.edu"
 url = "https://github.com/stanford-oval/suql"
 
 # Specify the packages to include. You can use `find_packages` to automatically discover them.
 packages = find_packages(where="src")
```

### Comparing `suql-1.1.4a1/src/suql/agent.py` & `suql-1.1.4a2/src/suql/agent.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a1/src/suql/faiss_embedding.py` & `suql-1.1.4a2/src/suql/faiss_embedding.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a1/src/suql/free_text_fcns_server.py` & `suql-1.1.4a2/src/suql/free_text_fcns_server.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a1/src/suql/postgresql_connection.py` & `suql-1.1.4a2/src/suql/postgresql_connection.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a1/src/suql/prompt_continuation.py` & `suql-1.1.4a2/src/suql/prompt_continuation.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a1/src/suql/prompts/if_db_classification.prompt` & `suql-1.1.4a2/src/suql/prompts/if_db_classification.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a1/src/suql/prompts/opening_hours.prompt` & `suql-1.1.4a2/src/suql/prompts/opening_hours.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a1/src/suql/prompts/parser_suql.prompt` & `suql-1.1.4a2/src/suql/prompts/parser_suql.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a1/src/suql/prompts/yelp_response_SQL.prompt` & `suql-1.1.4a2/src/suql/prompts/yelp_response_SQL.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a1/src/suql/prompts/yelp_response_no_results.prompt` & `suql-1.1.4a2/src/suql/prompts/yelp_response_no_results.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a1/src/suql/sql_free_text_support/execute_free_text_sql.py` & `suql-1.1.4a2/src/suql/sql_free_text_support/execute_free_text_sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -1670,15 +1670,15 @@
                                 logging.StreamHandler()
                             ])
 
     else:
         logging.basicConfig(level=logging.CRITICAL + 1)
 
     if _parse_standalone_answer(suql) is not None:
-        return _execute_standalone_answer(suql, source_file_mapping)
+        return _execute_standalone_answer(suql, source_file_mapping), [], {}
 
     results, column_names, cache = _suql_execute_single(
         suql,
         table_w_ids,
         fts_fields,
         llm_model_name,
         max_verify,
```

### Comparing `suql-1.1.4a1/src/suql/utils.py` & `suql-1.1.4a2/src/suql/utils.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a1/src/suql.egg-info/PKG-INFO` & `suql-1.1.4a2/src/suql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suql
-Version: 1.1.4a1
+Version: 1.1.4a2
 Summary: Structured and Unstructured Query Language (SUQL) Python API
 Home-page: https://github.com/stanford-oval/suql
 Author: Shicheng Liu
 Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: suql Version: 1.1.4a1 Summary: Structured and
+Metadata-Version: 2.1 Name: suql Version: 1.1.4a2 Summary: Structured and
 Unstructured Query Language (SUQL) Python API Home-page: https://github.com/
 stanford-oval/suql Author: Shicheng Liu Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `suql-1.1.4a1/src/suql.egg-info/SOURCES.txt` & `suql-1.1.4a2/src/suql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

