# Comparing `tmp/suql-1.1.4a0.tar.gz` & `tmp/suql-1.1.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suql-1.1.4a0.tar", last modified: Tue Apr 16 20:55:51 2024, max compression
+gzip compressed data, was "suql-1.1.4a1.tar", last modified: Wed Apr 17 07:37:32 2024, max compression
```

## Comparing `suql-1.1.4a0.tar` & `suql-1.1.4a1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwx------   0 oval      (1000) users      (100)        0 2024-04-16 20:55:51.281867 suql-1.1.4a0/
--rw-------   0 oval      (1000) users      (100)    11356 2024-04-03 06:02:28.000000 suql-1.1.4a0/LICENSE
--rw-------   0 oval      (1000) users      (100)     4884 2024-04-16 20:55:51.281867 suql-1.1.4a0/PKG-INFO
--rw-------   0 oval      (1000) users      (100)     4278 2024-04-15 19:06:57.000000 suql-1.1.4a0/README.md
--rw-------   0 oval      (1000) users      (100)       38 2024-04-16 20:55:51.281867 suql-1.1.4a0/setup.cfg
--rw-------   0 oval      (1000) users      (100)     1514 2024-04-16 20:10:07.000000 suql-1.1.4a0/setup.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-16 20:55:51.277867 suql-1.1.4a0/src/
-drwx------   0 oval      (1000) users      (100)        0 2024-04-16 20:55:51.277867 suql-1.1.4a0/src/suql/
--rw-------   0 oval      (1000) users      (100)       73 2024-04-03 06:02:28.000000 suql-1.1.4a0/src/suql/__init__.py
--rw-------   0 oval      (1000) users      (100)    17354 2024-04-07 06:37:06.000000 suql-1.1.4a0/src/suql/agent.py
--rw-------   0 oval      (1000) users      (100)    17524 2024-04-16 03:55:43.000000 suql-1.1.4a0/src/suql/faiss_embedding.py
--rw-------   0 oval      (1000) users      (100)     8591 2024-04-12 01:46:05.000000 suql-1.1.4a0/src/suql/free_text_fcns_server.py
--rw-------   0 oval      (1000) users      (100)     3591 2024-04-12 01:45:49.000000 suql-1.1.4a0/src/suql/postgresql_connection.py
--rw-------   0 oval      (1000) users      (100)     9642 2024-04-12 01:46:33.000000 suql-1.1.4a0/src/suql/prompt_continuation.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-16 20:55:51.281867 suql-1.1.4a0/src/suql/prompts/
--rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:18.000000 suql-1.1.4a0/src/suql/prompts/__init__.py
--rw-------   0 oval      (1000) users      (100)      169 2024-04-03 06:02:28.000000 suql-1.1.4a0/src/suql/prompts/answer_qa.prompt
--rw-------   0 oval      (1000) users      (100)      451 2024-04-03 06:02:28.000000 suql-1.1.4a0/src/suql/prompts/field_classification.prompt
--rw-------   0 oval      (1000) users      (100)     2945 2024-04-03 06:02:28.000000 suql-1.1.4a0/src/suql/prompts/if_db_classification.prompt
--rw-------   0 oval      (1000) users      (100)     1305 2024-04-03 06:02:28.000000 suql-1.1.4a0/src/suql/prompts/opening_hours.prompt
--rw-------   0 oval      (1000) users      (100)     5574 2024-04-03 06:02:28.000000 suql-1.1.4a0/src/suql/prompts/parser_suql.prompt
--rw-------   0 oval      (1000) users      (100)      227 2024-04-03 06:02:28.000000 suql-1.1.4a0/src/suql/prompts/verification.prompt
--rw-------   0 oval      (1000) users      (100)     2983 2024-04-03 06:02:28.000000 suql-1.1.4a0/src/suql/prompts/yelp_response_SQL.prompt
--rw-------   0 oval      (1000) users      (100)     1454 2024-04-03 06:02:28.000000 suql-1.1.4a0/src/suql/prompts/yelp_response_no_results.prompt
-drwx------   0 oval      (1000) users      (100)        0 2024-04-16 20:55:51.281867 suql-1.1.4a0/src/suql/sql_free_text_support/
--rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:11.000000 suql-1.1.4a0/src/suql/sql_free_text_support/__init__.py
--rw-------   0 oval      (1000) users      (100)    63679 2024-04-16 20:09:35.000000 suql-1.1.4a0/src/suql/sql_free_text_support/execute_free_text_sql.py
--rw-------   0 oval      (1000) users      (100)     6455 2024-04-03 06:02:28.000000 suql-1.1.4a0/src/suql/utils.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-16 20:55:51.277867 suql-1.1.4a0/src/suql.egg-info/
--rw-r--r--   0 oval      (1000) users      (100)     4884 2024-04-16 20:55:51.000000 suql-1.1.4a0/src/suql.egg-info/PKG-INFO
--rw-------   0 oval      (1000) users      (100)      824 2024-04-16 20:55:51.000000 suql-1.1.4a0/src/suql.egg-info/SOURCES.txt
--rw-------   0 oval      (1000) users      (100)        1 2024-04-16 20:55:51.000000 suql-1.1.4a0/src/suql.egg-info/dependency_links.txt
--rw-------   0 oval      (1000) users      (100)      186 2024-04-16 20:55:51.000000 suql-1.1.4a0/src/suql.egg-info/requires.txt
--rw-------   0 oval      (1000) users      (100)        5 2024-04-16 20:55:51.000000 suql-1.1.4a0/src/suql.egg-info/top_level.txt
+drwx------   0 oval      (1000) users      (100)        0 2024-04-17 07:37:32.890176 suql-1.1.4a1/
+-rw-------   0 oval      (1000) users      (100)    11356 2024-04-03 06:02:28.000000 suql-1.1.4a1/LICENSE
+-rw-------   0 oval      (1000) users      (100)     4884 2024-04-17 07:37:32.890176 suql-1.1.4a1/PKG-INFO
+-rw-------   0 oval      (1000) users      (100)     4278 2024-04-15 19:06:57.000000 suql-1.1.4a1/README.md
+-rw-------   0 oval      (1000) users      (100)       38 2024-04-17 07:37:32.890176 suql-1.1.4a1/setup.cfg
+-rw-------   0 oval      (1000) users      (100)     1514 2024-04-17 07:36:37.000000 suql-1.1.4a1/setup.py
+drwx------   0 oval      (1000) users      (100)        0 2024-04-17 07:37:32.886176 suql-1.1.4a1/src/
+drwx------   0 oval      (1000) users      (100)        0 2024-04-17 07:37:32.886176 suql-1.1.4a1/src/suql/
+-rw-------   0 oval      (1000) users      (100)       73 2024-04-03 06:02:28.000000 suql-1.1.4a1/src/suql/__init__.py
+-rw-------   0 oval      (1000) users      (100)    17354 2024-04-07 06:37:06.000000 suql-1.1.4a1/src/suql/agent.py
+-rw-------   0 oval      (1000) users      (100)    16980 2024-04-17 07:37:16.000000 suql-1.1.4a1/src/suql/faiss_embedding.py
+-rw-------   0 oval      (1000) users      (100)     8792 2024-04-17 07:27:02.000000 suql-1.1.4a1/src/suql/free_text_fcns_server.py
+-rw-------   0 oval      (1000) users      (100)     3591 2024-04-12 01:45:49.000000 suql-1.1.4a1/src/suql/postgresql_connection.py
+-rw-------   0 oval      (1000) users      (100)     9642 2024-04-12 01:46:33.000000 suql-1.1.4a1/src/suql/prompt_continuation.py
+drwx------   0 oval      (1000) users      (100)        0 2024-04-17 07:37:32.890176 suql-1.1.4a1/src/suql/prompts/
+-rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:18.000000 suql-1.1.4a1/src/suql/prompts/__init__.py
+-rw-------   0 oval      (1000) users      (100)      169 2024-04-03 06:02:28.000000 suql-1.1.4a1/src/suql/prompts/answer_qa.prompt
+-rw-------   0 oval      (1000) users      (100)      451 2024-04-03 06:02:28.000000 suql-1.1.4a1/src/suql/prompts/field_classification.prompt
+-rw-------   0 oval      (1000) users      (100)     2945 2024-04-03 06:02:28.000000 suql-1.1.4a1/src/suql/prompts/if_db_classification.prompt
+-rw-------   0 oval      (1000) users      (100)     1305 2024-04-03 06:02:28.000000 suql-1.1.4a1/src/suql/prompts/opening_hours.prompt
+-rw-------   0 oval      (1000) users      (100)     5574 2024-04-03 06:02:28.000000 suql-1.1.4a1/src/suql/prompts/parser_suql.prompt
+-rw-------   0 oval      (1000) users      (100)      227 2024-04-03 06:02:28.000000 suql-1.1.4a1/src/suql/prompts/verification.prompt
+-rw-------   0 oval      (1000) users      (100)     2983 2024-04-03 06:02:28.000000 suql-1.1.4a1/src/suql/prompts/yelp_response_SQL.prompt
+-rw-------   0 oval      (1000) users      (100)     1454 2024-04-03 06:02:28.000000 suql-1.1.4a1/src/suql/prompts/yelp_response_no_results.prompt
+drwx------   0 oval      (1000) users      (100)        0 2024-04-17 07:37:32.890176 suql-1.1.4a1/src/suql/sql_free_text_support/
+-rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:11.000000 suql-1.1.4a1/src/suql/sql_free_text_support/__init__.py
+-rw-------   0 oval      (1000) users      (100)    64753 2024-04-17 07:35:47.000000 suql-1.1.4a1/src/suql/sql_free_text_support/execute_free_text_sql.py
+-rw-------   0 oval      (1000) users      (100)     6455 2024-04-03 06:02:28.000000 suql-1.1.4a1/src/suql/utils.py
+drwx------   0 oval      (1000) users      (100)        0 2024-04-17 07:37:32.886176 suql-1.1.4a1/src/suql.egg-info/
+-rw-r--r--   0 oval      (1000) users      (100)     4884 2024-04-17 07:37:32.000000 suql-1.1.4a1/src/suql.egg-info/PKG-INFO
+-rw-------   0 oval      (1000) users      (100)      824 2024-04-17 07:37:32.000000 suql-1.1.4a1/src/suql.egg-info/SOURCES.txt
+-rw-------   0 oval      (1000) users      (100)        1 2024-04-17 07:37:32.000000 suql-1.1.4a1/src/suql.egg-info/dependency_links.txt
+-rw-------   0 oval      (1000) users      (100)      186 2024-04-17 07:37:32.000000 suql-1.1.4a1/src/suql.egg-info/requires.txt
+-rw-------   0 oval      (1000) users      (100)        5 2024-04-17 07:37:32.000000 suql-1.1.4a1/src/suql.egg-info/top_level.txt
```

### Comparing `suql-1.1.4a0/LICENSE` & `suql-1.1.4a1/LICENSE`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a0/PKG-INFO` & `suql-1.1.4a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suql
-Version: 1.1.4a0
+Version: 1.1.4a1
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
-Metadata-Version: 2.1 Name: suql Version: 1.1.4a0 Summary: Structured and
+Metadata-Version: 2.1 Name: suql Version: 1.1.4a1 Summary: Structured and
 Unstructured Query Language (SUQL) Python API Home-page: https://github.com/
 stanford-oval/suql Author: Shicheng Liu Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `suql-1.1.4a0/README.md` & `suql-1.1.4a1/README.md`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a0/setup.py` & `suql-1.1.4a1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 # Package metadata
 name = "suql"
-version = "1.1.4a0"
+version = "1.1.4a1"
 description = "Structured and Unstructured Query Language (SUQL) Python API"
 author = "Shicheng Liu"
 author_email = "shicheng@cs.stanford.edu"
 url = "https://github.com/stanford-oval/suql"
 
 # Specify the packages to include. You can use `find_packages` to automatically discover them.
 packages = find_packages(where="src")
```

### Comparing `suql-1.1.4a0/src/suql/agent.py` & `suql-1.1.4a1/src/suql/agent.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a0/src/suql/faiss_embedding.py` & `suql-1.1.4a1/src/suql/faiss_embedding.py`

 * *Files 6% similar despite different names*

```diff
@@ -480,31 +480,13 @@
         table_name="restaurants",
         primary_key_field_name="_id",
         free_text_field_name="popular_dishes",
         db_name="restaurants",
         user="select_user",
         password="select_user",
     )
-    embedding_store.add(
-        table_name="courses",
-        primary_key_field_name="course_id",
-        free_text_field_name="description",
-        db_name="course_assistant"
-    )
-    embedding_store.add(
-        table_name="ratings",
-        primary_key_field_name="rating_id",
-        free_text_field_name="reviews",
-        db_name="course_assistant"
-    )
-    embedding_store.add(
-        table_name="programs",
-        primary_key_field_name="program_id",
-        free_text_field_name="sheet",
-        db_name="course_assistant"
-    )
 
     # Set the server address, if running through command line
     host = "127.0.0.1"
-    port = 8509
+    port = 8501
 
     embedding_store.start_embedding_server(host=host, port=port)
```

### Comparing `suql-1.1.4a0/src/suql/free_text_fcns_server.py` & `suql-1.1.4a1/src/suql/free_text_fcns_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,54 @@
 # # Max number of input tokens for the `summary` function
 # max_input_token = 3800
 
 # # Default LLM engine for `answer` and `summary` functions
 # engine = "gpt-3.5-turbo-0613"
 
 
+def _answer(source, query, type_prompt = None, k=5, max_input_token=3800, engine="gpt-3.5-turbo-0613"):
+    from suql.prompt_continuation import llm_generate
+    if not source:
+        return {"result": "no information"}
+
+    text_res = []
+    if isinstance(source, list):
+        documents = compute_top_similarity_documents(
+            source, query, top=k
+        )
+        for i in documents:
+            if num_tokens_from_string("\n".join(text_res + [i])) < max_input_token:
+                text_res.append(i)
+            else:
+                break
+    else:
+        text_res = [source]
+
+    type_prompt = ""
+    if type_prompt:
+        if type_prompt == "date":
+            type_prompt = f" Output in date format, for instance 2001-09-28."
+        if type_prompt == "int4":
+            type_prompt = f" Output an integer."
+
+    continuation, _ = llm_generate(
+        "prompts/answer_qa.prompt",
+        {
+            "reviews": text_res,
+            "question": query,
+            "type_prompt": type_prompt,
+        },
+        engine=engine,
+        max_tokens=200,
+        temperature=0.0,
+        stop_tokens=["\n"],
+        postprocess=False,
+    )
+    return {"result": continuation}
+
 def start_free_text_fncs_server(
     host="127.0.0.1", port=8500, k=5, max_input_token=3800, engine="gpt-3.5-turbo-0613"
 ):
     """
     Set up a free text functions server for the free text
     `answer` and `summary` functions.
 
@@ -60,53 +100,23 @@
         from suql.prompt_continuation import llm_generate
 
         data = request.get_json()
 
         if "text" not in data or "question" not in data:
             return None
 
-        if not data["text"]:
-            return {"result": "no information"}
-
-        text_res = []
-        if isinstance(data["text"], list):
-            documents = compute_top_similarity_documents(
-                data["text"], data["question"], top=k
-            )
-            for i in documents:
-                if num_tokens_from_string("\n".join(text_res + [i])) < max_input_token:
-                    text_res.append(i)
-                else:
-                    break
-        else:
-            text_res = [data["text"]]
-
-        type_prompt = ""
-        if "type_prompt" in data:
-            if data["type_prompt"] == "date":
-                type_prompt = f" Output in date format, for instance 2001-09-28."
-            if data["type_prompt"] == "int4":
-                type_prompt = f" Output an integer."
-
-        continuation, _ = llm_generate(
-            "prompts/answer_qa.prompt",
-            {
-                "reviews": text_res,
-                "question": data["question"],
-                "type_prompt": type_prompt,
-            },
-            engine=engine,
-            max_tokens=200,
-            temperature=0.0,
-            stop_tokens=["\n"],
-            postprocess=False,
+        return _answer(
+            data["text"],
+            data["question"],
+            type_prompt=data["type_prompt"] if "type_prompt" in data else None,
+            k = k,
+            max_input_token = max_input_token,
+            engine = engine
         )
-
-        res = {"result": continuation}
-        return res
+    
 
     @app.route("/summary", methods=["POST"])
     def summary():
         """
         LLM-based summary function, set up as a server for PSQL to call.
         `summary(text)` is a syntactic sugar for `answer(text, 'what is the summary of this document?')`
         By default, append as many documents as possible until `max_input_token` is reached
```

### Comparing `suql-1.1.4a0/src/suql/postgresql_connection.py` & `suql-1.1.4a1/src/suql/postgresql_connection.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a0/src/suql/prompt_continuation.py` & `suql-1.1.4a1/src/suql/prompt_continuation.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a0/src/suql/prompts/if_db_classification.prompt` & `suql-1.1.4a1/src/suql/prompts/if_db_classification.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a0/src/suql/prompts/opening_hours.prompt` & `suql-1.1.4a1/src/suql/prompts/opening_hours.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a0/src/suql/prompts/parser_suql.prompt` & `suql-1.1.4a1/src/suql/prompts/parser_suql.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a0/src/suql/prompts/yelp_response_SQL.prompt` & `suql-1.1.4a1/src/suql/prompts/yelp_response_SQL.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a0/src/suql/prompts/yelp_response_no_results.prompt` & `suql-1.1.4a1/src/suql/prompts/yelp_response_no_results.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a0/src/suql/sql_free_text_support/execute_free_text_sql.py` & `suql-1.1.4a1/src/suql/sql_free_text_support/execute_free_text_sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import concurrent.futures
 import json
 import random
 import string
 import time
 import traceback
 import logging
+import re
 from collections import defaultdict
 from copy import deepcopy
 from typing import List, Union
 
 import pglast
 import requests
 from pglast import parse_sql
@@ -20,14 +21,15 @@
 from psycopg2 import Error as psyconpg2Error
 from sympy import Symbol, symbols
 from sympy.logic.boolalg import And, Not, Or, to_dnf
 
 from suql.postgresql_connection import execute_sql, execute_sql_with_column_info
 from suql.prompt_continuation import llm_generate
 from suql.utils import num_tokens_from_string
+from suql.free_text_fcns_server import _answer
 
 # System parameters, do not modify
 _SET_FREE_TEXT_FCNS = ["answer"]
 _verified_res = {}
 
 def _generate_random_string(length=12):
     characters = string.ascii_lowercase + string.digits
@@ -1554,28 +1556,54 @@
         raise ValueError(
             "Expects sql to be in DNF, but is not: {}".format(
                 RawStream()(sql_dnf_predicates)
             )
         )
 
 
+def _parse_standalone_answer(suql):
+    # Define a regular expression pattern to match the required format
+    # \s* allows for any number of whitespaces around the parentheses
+    pattern = r"\s*answer\s*\(\s*([a-zA-Z_0-9]+)\s*,\s*['\"](.+?)['\"]\s*\)\s*"
+    
+    # Use the re.match function to check if the entire string matches the pattern
+    match = re.match(pattern, suql)
+    
+    # If a match is found, return the captured groups: source and query
+    if match:
+        return match.group(1), match.group(2)
+    else:
+        return None
+
+def _execute_standalone_answer(suql, source_file_mapping):
+    source, query = _parse_standalone_answer(suql)
+    if source not in source_file_mapping:
+        return None
+    
+    with open(source_file_mapping[source], "r") as fd:
+        source_content = fd.read()
+    
+    return _answer(source_content, query)
+    
+
 def suql_execute(
     suql,
     table_w_ids,
     fts_fields=[],
     llm_model_name="gpt-3.5-turbo-0125",
     max_verify=20,
     loggings="",
     log_filename=None,
     disable_try_catch=False,
     embedding_server_address="http://127.0.0.1:8501",
     select_username="select_user",
     select_userpswd="select_user",
     create_username="creator_role",
     create_userpswd="creator_role",
+    source_file_mapping={},
 ):
     """
     Main entry point to the SUQL Python-based compiler.
 
     # Parameters:
     `suql` (str): The to-be-executed suql query.
     
@@ -1641,14 +1669,17 @@
                                 logging.FileHandler(log_filename),
                                 logging.StreamHandler()
                             ])
 
     else:
         logging.basicConfig(level=logging.CRITICAL + 1)
 
+    if _parse_standalone_answer(suql) is not None:
+        return _execute_standalone_answer(suql, source_file_mapping)
+
     results, column_names, cache = _suql_execute_single(
         suql,
         table_w_ids,
         fts_fields,
         llm_model_name,
         max_verify,
         embedding_server_address,
```

### Comparing `suql-1.1.4a0/src/suql/utils.py` & `suql-1.1.4a1/src/suql/utils.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.4a0/src/suql.egg-info/PKG-INFO` & `suql-1.1.4a1/src/suql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suql
-Version: 1.1.4a0
+Version: 1.1.4a1
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
-Metadata-Version: 2.1 Name: suql Version: 1.1.4a0 Summary: Structured and
+Metadata-Version: 2.1 Name: suql Version: 1.1.4a1 Summary: Structured and
 Unstructured Query Language (SUQL) Python API Home-page: https://github.com/
 stanford-oval/suql Author: Shicheng Liu Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `suql-1.1.4a0/src/suql.egg-info/SOURCES.txt` & `suql-1.1.4a1/src/suql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

