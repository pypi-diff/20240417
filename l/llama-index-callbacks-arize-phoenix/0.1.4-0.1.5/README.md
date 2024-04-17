# Comparing `tmp/llama_index_callbacks_arize_phoenix-0.1.4.tar.gz` & `tmp/llama_index_callbacks_arize_phoenix-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_callbacks_arize_phoenix-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_callbacks_arize_phoenix-0.1.5.tar", max compression
```

## Comparing `llama_index_callbacks_arize_phoenix-0.1.4.tar` & `llama_index_callbacks_arize_phoenix-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       50 2024-02-13 13:53:01.587178 llama_index_callbacks_arize_phoenix-0.1.4/README.md
--rw-r--r--   0        0        0      130 2024-02-13 13:53:01.587639 llama_index_callbacks_arize_phoenix-0.1.4/llama_index/callbacks/arize_phoenix/__init__.py
--rw-r--r--   0        0        0      456 2024-02-13 13:53:01.587706 llama_index_callbacks_arize_phoenix-0.1.4/llama_index/callbacks/arize_phoenix/base.py
--rw-r--r--   0        0        0     1643 2024-02-21 16:11:41.670410 llama_index_callbacks_arize_phoenix-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      741 1970-01-01 00:00:00.000000 llama_index_callbacks_arize_phoenix-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       50 2024-04-17 21:36:44.087050 llama_index_callbacks_arize_phoenix-0.1.5/README.md
+-rw-r--r--   0        0        0      130 2024-04-17 21:36:44.087050 llama_index_callbacks_arize_phoenix-0.1.5/llama_index/callbacks/arize_phoenix/__init__.py
+-rw-r--r--   0        0        0      456 2024-04-17 21:36:44.087050 llama_index_callbacks_arize_phoenix-0.1.5/llama_index/callbacks/arize_phoenix/base.py
+-rw-r--r--   0        0        0     1643 2024-04-17 21:36:44.087050 llama_index_callbacks_arize_phoenix-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      741 1970-01-01 00:00:00.000000 llama_index_callbacks_arize_phoenix-0.1.5/PKG-INFO
```

### Comparing `llama_index_callbacks_arize_phoenix-0.1.4/pyproject.toml` & `llama_index_callbacks_arize_phoenix-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 [tool.poetry]
 authors = ["Arize AI <phoenix-devs@arize.com>", "OpenInference Authors <oss@arize.com>"]
 description = "llama-index callbacks arize-phoenix integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-callbacks-arize-phoenix"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<3.12"
+python = ">=3.8.1,<3.13"
 arize-phoenix = ">=3.0.3"
 openinference-instrumentation-llama-index = ">=1.0.0"
 llama-index-core = "^0.10.11.post1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
```

### Comparing `llama_index_callbacks_arize_phoenix-0.1.4/PKG-INFO` & `llama_index_callbacks_arize_phoenix-0.1.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: llama-index-callbacks-arize-phoenix
-Version: 0.1.4
+Version: 0.1.5
 Summary: llama-index callbacks arize-phoenix integration
 License: MIT
 Author: Arize AI
 Author-email: phoenix-devs@arize.com
-Requires-Python: >=3.8.1,<3.12
+Requires-Python: >=3.8.1,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arize-phoenix (>=3.0.3)
 Requires-Dist: llama-index-core (>=0.10.11.post1,<0.11.0)
```

