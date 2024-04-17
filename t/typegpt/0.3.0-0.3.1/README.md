# Comparing `tmp/typegpt-0.3.0.tar.gz` & `tmp/typegpt-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typegpt-0.3.0.tar", last modified: Thu Apr 11 17:01:10 2024, max compression
+gzip compressed data, was "typegpt-0.3.1.tar", last modified: Wed Apr 17 09:42:28 2024, max compression
```

## Comparing `typegpt-0.3.0.tar` & `typegpt-0.3.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:01:10.826071 typegpt-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-11 17:01:07.000000 typegpt-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11015 2024-04-11 17:01:10.826071 typegpt-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10460 2024-04-11 17:01:07.000000 typegpt-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 17:01:10.826071 typegpt-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-11 17:01:07.000000 typegpt-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:01:10.818071 typegpt-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-04-11 17:01:07.000000 typegpt-0.3.0/tests/test_fewshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-04-11 17:01:07.000000 typegpt-0.3.0/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     8699 2024-04-11 17:01:07.000000 typegpt-0.3.0/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    19118 2024-04-11 17:01:07.000000 typegpt-0.3.0/tests/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    14423 2024-04-11 17:01:07.000000 typegpt-0.3.0/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-11 17:01:07.000000 typegpt-0.3.0/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)    13431 2024-04-11 17:01:07.000000 typegpt-0.3.0/tests/test_response_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-11 17:01:07.000000 typegpt-0.3.0/tests/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:01:10.822071 typegpt-0.3.0/typegpt/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/example_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/example_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/message_collection_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:01:10.822071 typegpt-0.3.0/typegpt/openai/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/openai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:01:10.822071 typegpt-0.3.0/typegpt/openai/_async/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/openai/_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8864 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/openai/_async/chat_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/openai/_async/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:01:10.822071 typegpt-0.3.0/typegpt/openai/_sync/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/openai/_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8761 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/openai/_sync/chat_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/openai/_sync/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/openai/base_chat_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/openai/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/openai/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/prompt_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:01:10.822071 typegpt-0.3.0/typegpt/prompt_definition/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/prompt_definition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/prompt_definition/few_shot_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/prompt_definition/prompt_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/prompt_definition/prompt_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:01:10.826071 typegpt-0.3.0/typegpt/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/utils/internal_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/utils/type_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-11 17:01:07.000000 typegpt-0.3.0/typegpt/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:01:10.826071 typegpt-0.3.0/typegpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11015 2024-04-11 17:01:10.000000 typegpt-0.3.0/typegpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-11 17:01:10.000000 typegpt-0.3.0/typegpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 17:01:10.000000 typegpt-0.3.0/typegpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 17:01:10.000000 typegpt-0.3.0/typegpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 17:01:10.000000 typegpt-0.3.0/typegpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:42:28.132899 typegpt-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-17 09:42:22.000000 typegpt-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11015 2024-04-17 09:42:28.132899 typegpt-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10460 2024-04-17 09:42:22.000000 typegpt-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 09:42:28.136899 typegpt-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-17 09:42:22.000000 typegpt-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:42:28.128899 typegpt-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8985 2024-04-17 09:42:22.000000 typegpt-0.3.1/tests/test_fewshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-04-17 09:42:22.000000 typegpt-0.3.1/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8699 2024-04-17 09:42:22.000000 typegpt-0.3.1/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19118 2024-04-17 09:42:22.000000 typegpt-0.3.1/tests/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14423 2024-04-17 09:42:22.000000 typegpt-0.3.1/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-17 09:42:22.000000 typegpt-0.3.1/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13431 2024-04-17 09:42:22.000000 typegpt-0.3.1/tests/test_response_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-17 09:42:22.000000 typegpt-0.3.1/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:42:28.128899 typegpt-0.3.1/typegpt/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/example_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/example_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/message_collection_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8467 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:42:28.132899 typegpt-0.3.1/typegpt/openai/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/openai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:42:28.132899 typegpt-0.3.1/typegpt/openai/_async/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/openai/_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8864 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/openai/_async/chat_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/openai/_async/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:42:28.132899 typegpt-0.3.1/typegpt/openai/_sync/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/openai/_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8761 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/openai/_sync/chat_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/openai/_sync/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/openai/base_chat_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/openai/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/openai/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/prompt_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:42:28.132899 typegpt-0.3.1/typegpt/prompt_definition/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/prompt_definition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/prompt_definition/few_shot_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/prompt_definition/prompt_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/prompt_definition/prompt_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:42:28.132899 typegpt-0.3.1/typegpt/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/utils/internal_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/utils/type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-17 09:42:22.000000 typegpt-0.3.1/typegpt/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:42:28.132899 typegpt-0.3.1/typegpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11015 2024-04-17 09:42:28.000000 typegpt-0.3.1/typegpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-17 09:42:28.000000 typegpt-0.3.1/typegpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:42:28.000000 typegpt-0.3.1/typegpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-17 09:42:28.000000 typegpt-0.3.1/typegpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 09:42:28.000000 typegpt-0.3.1/typegpt.egg-info/top_level.txt
```

### Comparing `typegpt-0.3.0/LICENSE` & `typegpt-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.0/PKG-INFO` & `typegpt-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typegpt
-Version: 0.3.0
+Version: 0.3.1
 Summary: TypeGPT - Make GPT safe for production
 Home-page: https://github.com/alexeichhorn/typegpt
 Author: Alexander Eichhorn
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `typegpt-0.3.0/README.md` & `typegpt-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.0/setup.py` & `typegpt-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="typegpt",
-    version="0.3.0",
+    version="0.3.1",
     author="Alexander Eichhorn",
     author_email="",
     description="TypeGPT - Make GPT safe for production",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/alexeichhorn/typegpt",
     install_requires=[
```

### Comparing `typegpt-0.3.0/tests/test_fewshot.py` & `typegpt-0.3.1/tests/test_fewshot.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.0/tests/test_fields.py` & `typegpt-0.3.1/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.0/tests/test_helpers.py` & `typegpt-0.3.1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.0/tests/test_openai.py` & `typegpt-0.3.1/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.0/tests/test_parser.py` & `typegpt-0.3.1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.0/tests/test_prompt.py` & `typegpt-0.3.1/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.0/tests/test_response_object.py` & `typegpt-0.3.1/tests/test_response_object.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.0/tests/test_settings.py` & `typegpt-0.3.1/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.0/typegpt/base.py` & `typegpt-0.3.1/typegpt/base.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.0/typegpt/example_builder.py` & `typegpt-0.3.1/typegpt/example_builder.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.0/typegpt/example_formatter.py` & `typegpt-0.3.1/typegpt/example_formatter.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.0/typegpt/fields.py` & `typegpt-0.3.1/typegpt/fields.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.0/typegpt/helper.py` & `typegpt-0.3.1/typegpt/helper.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.0/typegpt/message_collection_builder.py` & `typegpt-0.3.1/typegpt/message_collection_builder.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.0/typegpt/meta.py` & `typegpt-0.3.1/typegpt/meta.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.0/typegpt/openai/_async/chat_completion.py` & `typegpt-0.3.1/typegpt/openai/_async/chat_completion.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.0/typegpt/openai/_async/client.py` & `typegpt-0.3.1/typegpt/openai/_async/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import inspect
 from typing import Mapping
 
 import httpx
 from openai import AsyncAzureOpenAI, AsyncOpenAI, resources
 from openai._constants import DEFAULT_MAX_RETRIES
 from openai._types import NOT_GIVEN, NotGiven
 from openai.lib.azure import AsyncAzureADTokenProvider
@@ -21,32 +22,46 @@
     chat: AsyncTypeChat
 
     def __init__(
         self,
         *,
         api_key: str | None = None,
         organization: str | None = None,
+        project: str | None = None,
         base_url: str | httpx.URL | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
         max_retries: int = DEFAULT_MAX_RETRIES,
         default_headers: Mapping[str, str] | None = None,
         default_query: Mapping[str, object] | None = None,
         # Configure a custom httpx client. See the [httpx documentation](https://www.python-httpx.org/api/#asyncclient) for more details.
         http_client: httpx.AsyncClient | None = None,
         # only needed to have same subclass capabilities (i.e. for Azure)
         _strict_response_validation: bool = False,
     ) -> None:
-        super().__init__(
-            api_key=api_key,
-            organization=organization,
-            base_url=base_url,
-            timeout=timeout,
-            max_retries=max_retries,
-            default_headers=default_headers,
-            default_query=default_query,
-            http_client=http_client,
-        )
+        init_signature = inspect.signature(super.__init__)
+        if "project" in init_signature.parameters:  # openai version >= 1.20.0
+            super().__init__(
+                api_key=api_key,
+                organization=organization,
+                project=project,
+                base_url=base_url,
+                timeout=timeout,
+                max_retries=max_retries,
+                default_headers=default_headers,
+                default_query=default_query,
+                http_client=http_client,
+            )
+        else:
+            super().__init__(
+                api_key=api_key,
+                organization=organization,
+                base_url=base_url,
+                timeout=timeout,
+                max_retries=max_retries,
+                default_headers=default_headers,
+                default_query=default_query,
+                http_client=http_client,
+            )
         self.chat = AsyncTypeChat(self)
 
 
-class AsyncTypeAzureOpenAI(AsyncAzureOpenAI, AsyncTypeOpenAI):
-    ...
+class AsyncTypeAzureOpenAI(AsyncAzureOpenAI, AsyncTypeOpenAI): ...
```

### Comparing `typegpt-0.3.0/typegpt/openai/_sync/chat_completion.py` & `typegpt-0.3.1/typegpt/openai/_sync/chat_completion.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.0/typegpt/openai/base_chat_completion.py` & `typegpt-0.3.1/typegpt/openai/base_chat_completion.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.0/typegpt/openai/views.py` & `typegpt-0.3.1/typegpt/openai/views.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.0/typegpt/parser.py` & `typegpt-0.3.1/typegpt/parser.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.0/typegpt/prompt_builder.py` & `typegpt-0.3.1/typegpt/prompt_builder.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.0/typegpt/prompt_definition/prompt_template.py` & `typegpt-0.3.1/typegpt/prompt_definition/prompt_template.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.0/typegpt/utils/type_checker.py` & `typegpt-0.3.1/typegpt/utils/type_checker.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.0/typegpt/utils/utils.py` & `typegpt-0.3.1/typegpt/utils/utils.py`

 * *Files identical despite different names*

### Comparing `typegpt-0.3.0/typegpt.egg-info/PKG-INFO` & `typegpt-0.3.1/typegpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typegpt
-Version: 0.3.0
+Version: 0.3.1
 Summary: TypeGPT - Make GPT safe for production
 Home-page: https://github.com/alexeichhorn/typegpt
 Author: Alexander Eichhorn
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `typegpt-0.3.0/typegpt.egg-info/SOURCES.txt` & `typegpt-0.3.1/typegpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

