# Comparing `tmp/nimbusagent-0.5.0.tar.gz` & `tmp/nimbusagent-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nimbusagent-0.5.0.tar", last modified: Fri Apr  5 21:28:58 2024, max compression
+gzip compressed data, was "nimbusagent-0.5.1.tar", last modified: Tue Apr 16 22:50:43 2024, max compression
```

## Comparing `nimbusagent-0.5.0.tar` & `nimbusagent-0.5.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-05 21:28:58.600841 nimbusagent-0.5.0/
--rw-r--r--   0 Lee        (501) staff       (20)     3101 2023-12-04 18:36:26.000000 nimbusagent-0.5.0/.gitignore
--rw-r--r--   0 Lee        (501) staff       (20)     1073 2023-12-06 18:57:23.000000 nimbusagent-0.5.0/LICENSE.txt
--rw-r--r--   0 Lee        (501) staff       (20)       48 2023-11-18 23:57:46.000000 nimbusagent-0.5.0/MANIFEST.in
--rw-r--r--   0 Lee        (501) staff       (20)    10524 2024-04-05 21:28:58.600142 nimbusagent-0.5.0/PKG-INFO
--rw-r--r--   0 Lee        (501) staff       (20)     7989 2024-04-05 21:23:21.000000 nimbusagent-0.5.0/README.md
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-05 21:28:58.518938 nimbusagent-0.5.0/bin/
--rwxr-xr-x   0 Lee        (501) staff       (20)      384 2023-12-26 20:55:01.000000 nimbusagent-0.5.0/bin/build.sh
--rwxr-xr-x   0 Lee        (501) staff       (20)      209 2023-12-22 17:10:13.000000 nimbusagent-0.5.0/bin/publish-pypi.sh
--rwxr-xr-x   0 Lee        (501) staff       (20)      240 2023-12-22 17:34:16.000000 nimbusagent-0.5.0/bin/run_tests.sh
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-05 21:28:58.529665 nimbusagent-0.5.0/examples/
--rw-r--r--   0 Lee        (501) staff       (20)      277 2023-12-04 21:15:51.000000 nimbusagent-0.5.0/examples/completion_agent_basic_example.py
--rw-r--r--   0 Lee        (501) staff       (20)     1532 2023-12-26 21:17:23.000000 nimbusagent-0.5.0/examples/completion_agent_function_example.py
--rw-r--r--   0 Lee        (501) staff       (20)      427 2023-12-04 21:15:51.000000 nimbusagent-0.5.0/examples/completion_agent_history_example.py
--rw-r--r--   0 Lee        (501) staff       (20)      362 2023-12-04 21:15:51.000000 nimbusagent-0.5.0/examples/streaming_agent_basic_example.py
--rw-r--r--   0 Lee        (501) staff       (20)     1620 2023-12-26 21:17:23.000000 nimbusagent-0.5.0/examples/streaming_agent_function_example.py
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-05 21:28:58.535663 nimbusagent-0.5.0/examples/streaming_cli_chatbot/
--rw-r--r--   0 Lee        (501) staff       (20)     2376 2023-12-04 18:36:26.000000 nimbusagent-0.5.0/examples/streaming_cli_chatbot/simple_spinner.py
--rw-r--r--   0 Lee        (501) staff       (20)     2999 2023-12-04 21:15:51.000000 nimbusagent-0.5.0/examples/streaming_cli_chatbot/streaming_cli_chatbot.py
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-05 21:28:58.536218 nimbusagent-0.5.0/nimbusagent/
--rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.5.0/nimbusagent/__init__.py
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-05 21:28:58.549908 nimbusagent-0.5.0/nimbusagent/agent/
--rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.5.0/nimbusagent/agent/__init__.py
--rw-r--r--   0 Lee        (501) staff       (20)    13678 2024-04-05 21:20:08.000000 nimbusagent-0.5.0/nimbusagent/agent/base.py
--rw-r--r--   0 Lee        (501) staff       (20)     5140 2024-04-05 21:23:21.000000 nimbusagent-0.5.0/nimbusagent/agent/completion.py
--rw-r--r--   0 Lee        (501) staff       (20)    12843 2024-04-05 21:20:08.000000 nimbusagent-0.5.0/nimbusagent/agent/streaming.py
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-05 21:28:58.562969 nimbusagent-0.5.0/nimbusagent/functions/
--rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.5.0/nimbusagent/functions/__init__.py
--rw-r--r--   0 Lee        (501) staff       (20)    17923 2024-01-26 20:49:40.000000 nimbusagent-0.5.0/nimbusagent/functions/handler.py
--rw-r--r--   0 Lee        (501) staff       (20)     9997 2023-12-04 21:15:51.000000 nimbusagent-0.5.0/nimbusagent/functions/parser.py
--rw-r--r--   0 Lee        (501) staff       (20)     2293 2023-12-26 21:17:23.000000 nimbusagent-0.5.0/nimbusagent/functions/responses.py
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-05 21:28:58.567805 nimbusagent-0.5.0/nimbusagent/memory/
--rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.5.0/nimbusagent/memory/__init__.py
--rw-r--r--   0 Lee        (501) staff       (20)     5417 2023-12-04 21:15:51.000000 nimbusagent-0.5.0/nimbusagent/memory/base.py
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-05 21:28:58.573906 nimbusagent-0.5.0/nimbusagent/utils/
--rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.5.0/nimbusagent/utils/__init__.py
--rw-r--r--   0 Lee        (501) staff       (20)     4246 2024-01-26 21:46:54.000000 nimbusagent-0.5.0/nimbusagent/utils/helper.py
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-05 21:28:58.599536 nimbusagent-0.5.0/nimbusagent.egg-info/
--rw-r--r--   0 Lee        (501) staff       (20)    10524 2024-04-05 21:28:58.000000 nimbusagent-0.5.0/nimbusagent.egg-info/PKG-INFO
--rw-r--r--   0 Lee        (501) staff       (20)     1259 2024-04-05 21:28:58.000000 nimbusagent-0.5.0/nimbusagent.egg-info/SOURCES.txt
--rw-r--r--   0 Lee        (501) staff       (20)        1 2024-04-05 21:28:58.000000 nimbusagent-0.5.0/nimbusagent.egg-info/dependency_links.txt
--rw-r--r--   0 Lee        (501) staff       (20)       60 2024-04-05 21:28:58.000000 nimbusagent-0.5.0/nimbusagent.egg-info/requires.txt
--rw-r--r--   0 Lee        (501) staff       (20)       12 2024-04-05 21:28:58.000000 nimbusagent-0.5.0/nimbusagent.egg-info/top_level.txt
--rw-r--r--   0 Lee        (501) staff       (20)     1365 2024-04-05 21:23:21.000000 nimbusagent-0.5.0/pyproject.toml
--rw-r--r--   0 Lee        (501) staff       (20)       38 2024-04-05 21:28:58.600921 nimbusagent-0.5.0/setup.cfg
-drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-05 21:28:58.598557 nimbusagent-0.5.0/tests/
--rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 18:36:26.000000 nimbusagent-0.5.0/tests/__init__.py
--rw-r--r--   0 Lee        (501) staff       (20)     1961 2023-12-04 21:15:51.000000 nimbusagent-0.5.0/tests/test_nimbusagent_agent_base.py
--rw-r--r--   0 Lee        (501) staff       (20)     1012 2023-12-26 21:17:23.000000 nimbusagent-0.5.0/tests/test_nimbusagent_functions_handler.py
--rw-r--r--   0 Lee        (501) staff       (20)     1874 2023-12-04 21:15:51.000000 nimbusagent-0.5.0/tests/test_nimbusagent_functions_parser.py
--rw-r--r--   0 Lee        (501) staff       (20)      607 2023-12-26 21:17:23.000000 nimbusagent-0.5.0/tests/test_nimbusagent_functions_response.py
--rw-r--r--   0 Lee        (501) staff       (20)     4619 2023-12-04 21:15:51.000000 nimbusagent-0.5.0/tests/test_nimbusagent_memory_base.py
--rw-r--r--   0 Lee        (501) staff       (20)     6772 2024-01-05 19:48:38.000000 nimbusagent-0.5.0/tests/test_nimbusagent_utils.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-16 22:50:43.309659 nimbusagent-0.5.1/
+-rw-r--r--   0 Lee        (501) staff       (20)     3101 2023-12-04 18:36:26.000000 nimbusagent-0.5.1/.gitignore
+-rw-r--r--   0 Lee        (501) staff       (20)     1073 2023-12-06 18:57:23.000000 nimbusagent-0.5.1/LICENSE.txt
+-rw-r--r--   0 Lee        (501) staff       (20)       48 2023-11-18 23:57:46.000000 nimbusagent-0.5.1/MANIFEST.in
+-rw-r--r--   0 Lee        (501) staff       (20)    10524 2024-04-16 22:50:43.309136 nimbusagent-0.5.1/PKG-INFO
+-rw-r--r--   0 Lee        (501) staff       (20)     7989 2024-04-05 21:23:21.000000 nimbusagent-0.5.1/README.md
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-16 22:50:43.232431 nimbusagent-0.5.1/bin/
+-rwxr-xr-x   0 Lee        (501) staff       (20)      384 2023-12-26 20:55:01.000000 nimbusagent-0.5.1/bin/build.sh
+-rwxr-xr-x   0 Lee        (501) staff       (20)      209 2023-12-22 17:10:13.000000 nimbusagent-0.5.1/bin/publish-pypi.sh
+-rwxr-xr-x   0 Lee        (501) staff       (20)      240 2023-12-22 17:34:16.000000 nimbusagent-0.5.1/bin/run_tests.sh
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-16 22:50:43.247201 nimbusagent-0.5.1/examples/
+-rw-r--r--   0 Lee        (501) staff       (20)      277 2023-12-04 21:15:51.000000 nimbusagent-0.5.1/examples/completion_agent_basic_example.py
+-rw-r--r--   0 Lee        (501) staff       (20)     1532 2023-12-26 21:17:23.000000 nimbusagent-0.5.1/examples/completion_agent_function_example.py
+-rw-r--r--   0 Lee        (501) staff       (20)      427 2023-12-04 21:15:51.000000 nimbusagent-0.5.1/examples/completion_agent_history_example.py
+-rw-r--r--   0 Lee        (501) staff       (20)      362 2023-12-04 21:15:51.000000 nimbusagent-0.5.1/examples/streaming_agent_basic_example.py
+-rw-r--r--   0 Lee        (501) staff       (20)     1620 2023-12-26 21:17:23.000000 nimbusagent-0.5.1/examples/streaming_agent_function_example.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-16 22:50:43.252955 nimbusagent-0.5.1/examples/streaming_cli_chatbot/
+-rw-r--r--   0 Lee        (501) staff       (20)     2376 2023-12-04 18:36:26.000000 nimbusagent-0.5.1/examples/streaming_cli_chatbot/simple_spinner.py
+-rw-r--r--   0 Lee        (501) staff       (20)     2999 2023-12-04 21:15:51.000000 nimbusagent-0.5.1/examples/streaming_cli_chatbot/streaming_cli_chatbot.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-16 22:50:43.253443 nimbusagent-0.5.1/nimbusagent/
+-rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.5.1/nimbusagent/__init__.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-16 22:50:43.268663 nimbusagent-0.5.1/nimbusagent/agent/
+-rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.5.1/nimbusagent/agent/__init__.py
+-rw-r--r--   0 Lee        (501) staff       (20)    13678 2024-04-05 21:20:08.000000 nimbusagent-0.5.1/nimbusagent/agent/base.py
+-rw-r--r--   0 Lee        (501) staff       (20)     5140 2024-04-05 21:23:21.000000 nimbusagent-0.5.1/nimbusagent/agent/completion.py
+-rw-r--r--   0 Lee        (501) staff       (20)    12853 2024-04-16 22:49:59.000000 nimbusagent-0.5.1/nimbusagent/agent/streaming.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-16 22:50:43.282665 nimbusagent-0.5.1/nimbusagent/functions/
+-rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.5.1/nimbusagent/functions/__init__.py
+-rw-r--r--   0 Lee        (501) staff       (20)    17923 2024-01-26 20:49:40.000000 nimbusagent-0.5.1/nimbusagent/functions/handler.py
+-rw-r--r--   0 Lee        (501) staff       (20)     9997 2023-12-04 21:15:51.000000 nimbusagent-0.5.1/nimbusagent/functions/parser.py
+-rw-r--r--   0 Lee        (501) staff       (20)     2293 2023-12-26 21:17:23.000000 nimbusagent-0.5.1/nimbusagent/functions/responses.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-16 22:50:43.286062 nimbusagent-0.5.1/nimbusagent/memory/
+-rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.5.1/nimbusagent/memory/__init__.py
+-rw-r--r--   0 Lee        (501) staff       (20)     5417 2023-12-04 21:15:51.000000 nimbusagent-0.5.1/nimbusagent/memory/base.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-16 22:50:43.290023 nimbusagent-0.5.1/nimbusagent/utils/
+-rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 21:15:51.000000 nimbusagent-0.5.1/nimbusagent/utils/__init__.py
+-rw-r--r--   0 Lee        (501) staff       (20)     4246 2024-01-26 21:46:54.000000 nimbusagent-0.5.1/nimbusagent/utils/helper.py
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-16 22:50:43.308502 nimbusagent-0.5.1/nimbusagent.egg-info/
+-rw-r--r--   0 Lee        (501) staff       (20)    10524 2024-04-16 22:50:43.000000 nimbusagent-0.5.1/nimbusagent.egg-info/PKG-INFO
+-rw-r--r--   0 Lee        (501) staff       (20)     1259 2024-04-16 22:50:43.000000 nimbusagent-0.5.1/nimbusagent.egg-info/SOURCES.txt
+-rw-r--r--   0 Lee        (501) staff       (20)        1 2024-04-16 22:50:43.000000 nimbusagent-0.5.1/nimbusagent.egg-info/dependency_links.txt
+-rw-r--r--   0 Lee        (501) staff       (20)       60 2024-04-16 22:50:43.000000 nimbusagent-0.5.1/nimbusagent.egg-info/requires.txt
+-rw-r--r--   0 Lee        (501) staff       (20)       12 2024-04-16 22:50:43.000000 nimbusagent-0.5.1/nimbusagent.egg-info/top_level.txt
+-rw-r--r--   0 Lee        (501) staff       (20)     1365 2024-04-16 22:49:45.000000 nimbusagent-0.5.1/pyproject.toml
+-rw-r--r--   0 Lee        (501) staff       (20)       38 2024-04-16 22:50:43.309783 nimbusagent-0.5.1/setup.cfg
+drwxr-xr-x   0 Lee        (501) staff       (20)        0 2024-04-16 22:50:43.307901 nimbusagent-0.5.1/tests/
+-rw-r--r--   0 Lee        (501) staff       (20)        0 2023-12-04 18:36:26.000000 nimbusagent-0.5.1/tests/__init__.py
+-rw-r--r--   0 Lee        (501) staff       (20)     1961 2023-12-04 21:15:51.000000 nimbusagent-0.5.1/tests/test_nimbusagent_agent_base.py
+-rw-r--r--   0 Lee        (501) staff       (20)     1012 2023-12-26 21:17:23.000000 nimbusagent-0.5.1/tests/test_nimbusagent_functions_handler.py
+-rw-r--r--   0 Lee        (501) staff       (20)     1874 2023-12-04 21:15:51.000000 nimbusagent-0.5.1/tests/test_nimbusagent_functions_parser.py
+-rw-r--r--   0 Lee        (501) staff       (20)      607 2023-12-26 21:17:23.000000 nimbusagent-0.5.1/tests/test_nimbusagent_functions_response.py
+-rw-r--r--   0 Lee        (501) staff       (20)     4619 2023-12-04 21:15:51.000000 nimbusagent-0.5.1/tests/test_nimbusagent_memory_base.py
+-rw-r--r--   0 Lee        (501) staff       (20)     6772 2024-01-05 19:48:38.000000 nimbusagent-0.5.1/tests/test_nimbusagent_utils.py
```

### Comparing `nimbusagent-0.5.0/.gitignore` & `nimbusagent-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.0/LICENSE.txt` & `nimbusagent-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.0/PKG-INFO` & `nimbusagent-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nimbusagent
-Version: 0.5.0
+Version: 0.5.1
 Summary: An OpenAI agent with basic memory, functions, and moderation support
 Author: Lee Huffman
 License: MIT License
         
         Copyright (c) 2023 Vaisala Xweather
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nimbusagent-0.5.0/README.md` & `nimbusagent-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.0/examples/completion_agent_function_example.py` & `nimbusagent-0.5.1/examples/completion_agent_function_example.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.0/examples/streaming_agent_function_example.py` & `nimbusagent-0.5.1/examples/streaming_agent_function_example.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.0/examples/streaming_cli_chatbot/simple_spinner.py` & `nimbusagent-0.5.1/examples/streaming_cli_chatbot/simple_spinner.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.0/examples/streaming_cli_chatbot/streaming_cli_chatbot.py` & `nimbusagent-0.5.1/examples/streaming_cli_chatbot/streaming_cli_chatbot.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.0/nimbusagent/agent/base.py` & `nimbusagent-0.5.1/nimbusagent/agent/base.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.0/nimbusagent/agent/completion.py` & `nimbusagent-0.5.1/nimbusagent/agent/completion.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.0/nimbusagent/agent/streaming.py` & `nimbusagent-0.5.1/nimbusagent/agent/streaming.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,29 +21,33 @@
         """
         Ask the agent a question and return a generator that yields the response.
         :param query:  The query to ask the agent.
         :param max_retries:  The maximum number of times to retry the query if the AI fails to respond.
         :return:  A generator that yields the response.
         """
         if self._needs_moderation(query):
+            self.last_response = self.moderation_fail_message
             yield self.moderation_fail_message
-            return
 
-        self._clear_internal_thoughts()
-        self._clear_last_response()
-        self.function_handler.get_functions_from_query_and_history(query, self.get_chat_history())
-        self._append_to_chat_history('user', query)
-
-        ai_response = self._generate_streaming_response(max_retries=max_retries)
-        content_accumulated = []
-        for content in ai_response:
-            content_accumulated.append(content)
-            yield content
+        else:
+            self._clear_internal_thoughts()
+            self._clear_last_response()
+            self.function_handler.get_functions_from_query_and_history(query, self.get_chat_history())
+            self._append_to_chat_history('user', query)
+
+            ai_response = self._generate_streaming_response(max_retries=max_retries)
+            content_accumulated = []
+            for content in ai_response:
+                content_accumulated.append(content)
+                yield content
 
-        self._append_to_chat_history('assistant', "".join(content_accumulated))
+            self.last_response = "".join(content_accumulated)
+            self._append_to_chat_history('assistant', self.last_response)
+
+        self.handle_on_complete()
 
     def _generate_streaming_response(self, max_retries: int = 1) -> Generator[str, None, None]:
         """
         Generate a response from the AI and return a generator that yields the response.
         :param max_retries:  The maximum number of times to retry the query if the AI fails to respond.
         :return:  A generator that yields the response.
         """
@@ -54,18 +58,22 @@
             :return:  A generator that yields the response.
             """
             retries = max_retries
 
             def output_post_content(post_content: List[str]):
                 if post_content:
                     post_content_str = f"{' '.join(post_content)}\n"
-                    self.last_response += post_content_str
                     return post_content_str
                 return ""
 
+            def output_content(out_content: str):
+                if out_content:
+                    return out_content
+                return ""
+
             def output_event(event_type: str, name: str, data: any):
 
                 if not data:
                     return f"[[[{event_type}:{name}]]]"
 
                 if not isinstance(data, str):
                     data = json.dumps(data)
@@ -178,15 +186,15 @@
 
                                     if func_results.use_secondary_model:
                                         use_secondary_model = True
                                     if func_results.force_no_functions:
                                         force_no_functions = True
 
                             if content_send_directly_to_user:
-                                yield "\n".join(content_send_directly_to_user)
+                                yield output_content("\n".join(content_send_directly_to_user))
                                 yield output_post_content(post_content_items)
                                 return
 
                             tool_calls = []  # reset tool calls
 
                         elif finish_reason == "function_call":
                             if self.send_events:
@@ -229,44 +237,35 @@
                                     use_secondary_model = True
                                 if func_results.force_no_functions:
                                     force_no_functions = True
 
                         content = delta.content
                         if content is not None:
                             has_content = True
-                            if self.last_response is None:
-                                self.last_response = content
-                            else:
-                                self.last_response += content
-
-                            yield delta.content
+                            yield output_content(delta.content)
 
                         if message.choices[0].finish_reason == 'stop':
                             yield output_post_content(post_content_items)
-
-                            self.handle_on_complete()
                             return
                         if len(self.internal_thoughts) > self.internal_thoughts_max_entries:
                             if post_content_items:
                                 yield output_post_content(post_content_items)
                             else:
                                 num_thoughts = len(self.internal_thoughts)
                                 logging.error(f"Too many internal thoughts: {num_thoughts}.")
                                 yield "Too many internal thoughts."
-
-                            self.handle_on_complete()
                             return
 
                 except Exception as e:
                     logging.error("Exception encountered: %s (%s)", str(e), type(e).__name__, exc_info=True)
 
                     if retries > 0 and not has_content:
                         retries -= 1
                         time.sleep(1)
                         continue
-                    yield "AI temporarily unavailable."
+                    yield output_content("AI temporarily unavailable.")
                     break
 
             if loops >= self.loops_max:
-                yield HAVING_TROUBLE_MSG
+                yield output_content(HAVING_TROUBLE_MSG)
 
         return generate()
```

### Comparing `nimbusagent-0.5.0/nimbusagent/functions/handler.py` & `nimbusagent-0.5.1/nimbusagent/functions/handler.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.0/nimbusagent/functions/parser.py` & `nimbusagent-0.5.1/nimbusagent/functions/parser.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.0/nimbusagent/functions/responses.py` & `nimbusagent-0.5.1/nimbusagent/functions/responses.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.0/nimbusagent/memory/base.py` & `nimbusagent-0.5.1/nimbusagent/memory/base.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.0/nimbusagent/utils/helper.py` & `nimbusagent-0.5.1/nimbusagent/utils/helper.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.0/nimbusagent.egg-info/PKG-INFO` & `nimbusagent-0.5.1/nimbusagent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nimbusagent
-Version: 0.5.0
+Version: 0.5.1
 Summary: An OpenAI agent with basic memory, functions, and moderation support
 Author: Lee Huffman
 License: MIT License
         
         Copyright (c) 2023 Vaisala Xweather
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nimbusagent-0.5.0/nimbusagent.egg-info/SOURCES.txt` & `nimbusagent-0.5.1/nimbusagent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.0/pyproject.toml` & `nimbusagent-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nimbusagent"
-version = "0.5.0"
+version = "0.5.1"
 description = "An OpenAI agent with basic memory, functions, and moderation support"
 readme = "README.md"
 license = { file = "LICENSE.txt" }
 keywords = [
     "openai",
     "gpt3",
     "gpt3.5",
```

### Comparing `nimbusagent-0.5.0/tests/test_nimbusagent_agent_base.py` & `nimbusagent-0.5.1/tests/test_nimbusagent_agent_base.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.0/tests/test_nimbusagent_functions_handler.py` & `nimbusagent-0.5.1/tests/test_nimbusagent_functions_handler.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.0/tests/test_nimbusagent_functions_parser.py` & `nimbusagent-0.5.1/tests/test_nimbusagent_functions_parser.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.0/tests/test_nimbusagent_functions_response.py` & `nimbusagent-0.5.1/tests/test_nimbusagent_functions_response.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.0/tests/test_nimbusagent_memory_base.py` & `nimbusagent-0.5.1/tests/test_nimbusagent_memory_base.py`

 * *Files identical despite different names*

### Comparing `nimbusagent-0.5.0/tests/test_nimbusagent_utils.py` & `nimbusagent-0.5.1/tests/test_nimbusagent_utils.py`

 * *Files identical despite different names*

