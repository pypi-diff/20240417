# Comparing `tmp/mistral_common-1.0.1.tar.gz` & `tmp/mistral_common-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mistral_common-1.0.1.tar", max compression
+gzip compressed data, was "mistral_common-1.0.2.tar", max compression
```

## Comparing `mistral_common-1.0.1.tar` & `mistral_common-1.0.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     2949 2024-04-17 14:18:35.356766 mistral_common-1.0.1/README.md
--rw-r--r--   0        0        0     1288 2024-04-17 14:21:42.528726 mistral_common-1.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-17 12:28:15.315166 mistral_common-1.0.1/src/mistral_common/__init__.py
--rw-r--r--   0        0        0      244 2024-04-17 12:28:15.512167 mistral_common-1.0.1/src/mistral_common/base.py
--rw-r--r--   0        0        0   587404 2024-04-17 12:28:15.524166 mistral_common-1.0.1/src/mistral_common/data/mistral_instruct_tokenizer_240216.model.v2
--rw-r--r--   0        0        0   587404 2024-04-17 12:28:15.529175 mistral_common-1.0.1/src/mistral_common/data/mistral_instruct_tokenizer_240216.model.v3
--rw-r--r--   0        0        0   493443 2024-04-17 12:28:15.536165 mistral_common-1.0.1/src/mistral_common/data/tokenizer.model.v1
--rw-r--r--   0        0        0     1807 2024-04-17 12:28:15.516164 mistral_common-1.0.1/src/mistral_common/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-17 12:28:15.328168 mistral_common-1.0.1/src/mistral_common/protocol/__init__.py
--rw-r--r--   0        0        0      199 2024-04-17 12:28:15.333167 mistral_common-1.0.1/src/mistral_common/protocol/base.py
--rw-r--r--   0        0        0      400 2024-04-17 12:28:15.339167 mistral_common-1.0.1/src/mistral_common/protocol/embedding/request.py
--rw-r--r--   0        0        0      873 2024-04-17 12:28:15.344167 mistral_common-1.0.1/src/mistral_common/protocol/embedding/response.py
--rw-r--r--   0        0        0        0 2024-04-17 12:28:15.375166 mistral_common-1.0.1/src/mistral_common/protocol/instruct/__init__.py
--rw-r--r--   0        0        0     1376 2024-04-17 12:28:15.380167 mistral_common-1.0.1/src/mistral_common/protocol/instruct/messages.py
--rw-r--r--   0        0        0      956 2024-04-17 12:28:15.397171 mistral_common-1.0.1/src/mistral_common/protocol/instruct/request.py
--rw-r--r--   0        0        0     1918 2024-04-17 12:28:15.384183 mistral_common-1.0.1/src/mistral_common/protocol/instruct/response.py
--rw-r--r--   0        0        0      658 2024-04-17 12:28:15.388166 mistral_common-1.0.1/src/mistral_common/protocol/instruct/tool_calls.py
--rw-r--r--   0        0        0    10534 2024-04-17 12:28:15.393166 mistral_common-1.0.1/src/mistral_common/protocol/instruct/validator.py
--rw-r--r--   0        0        0       73 2024-04-17 12:28:15.403166 mistral_common-1.0.1/src/mistral_common/protocol/utils.py
--rw-r--r--   0        0        0        0 2024-04-17 12:28:15.408165 mistral_common-1.0.1/src/mistral_common/py.typed
--rw-r--r--   0        0        0        0 2024-04-17 12:28:15.421165 mistral_common-1.0.1/src/mistral_common/tokens/__init__.py
--rw-r--r--   0        0        0     6119 2024-04-17 12:28:15.443166 mistral_common-1.0.1/src/mistral_common/tokens/instruct/normalize.py
--rw-r--r--   0        0        0      418 2024-04-17 12:28:15.448166 mistral_common-1.0.1/src/mistral_common/tokens/instruct/request.py
--rw-r--r--   0        0        0     1481 2024-04-17 12:28:15.481165 mistral_common-1.0.1/src/mistral_common/tokens/tokenizers/base.py
--rw-r--r--   0        0        0     4660 2024-04-17 14:19:11.465776 mistral_common-1.0.1/src/mistral_common/tokens/tokenizers/mistral.py
--rw-r--r--   0        0        0    12394 2024-04-17 12:28:15.490165 mistral_common-1.0.1/src/mistral_common/tokens/tokenizers/sentencepiece.py
--rw-r--r--   0        0        0      187 2024-04-17 12:28:15.476165 mistral_common-1.0.1/src/mistral_common/tokens/tokenizers/utils.py
--rw-r--r--   0        0        0     3550 1970-01-01 00:00:00.000000 mistral_common-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11339 2024-04-17 14:26:20.275663 mistral_common-1.0.2/LICENCE
+-rw-r--r--   0        0        0     2949 2024-04-17 14:18:35.356766 mistral_common-1.0.2/README.md
+-rw-r--r--   0        0        0     1288 2024-04-17 14:26:42.134667 mistral_common-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-17 12:28:15.315166 mistral_common-1.0.2/src/mistral_common/__init__.py
+-rw-r--r--   0        0        0      244 2024-04-17 12:28:15.512167 mistral_common-1.0.2/src/mistral_common/base.py
+-rw-r--r--   0        0        0   587404 2024-04-17 12:28:15.524166 mistral_common-1.0.2/src/mistral_common/data/mistral_instruct_tokenizer_240216.model.v2
+-rw-r--r--   0        0        0   587404 2024-04-17 12:28:15.529175 mistral_common-1.0.2/src/mistral_common/data/mistral_instruct_tokenizer_240216.model.v3
+-rw-r--r--   0        0        0   493443 2024-04-17 12:28:15.536165 mistral_common-1.0.2/src/mistral_common/data/tokenizer.model.v1
+-rw-r--r--   0        0        0     1807 2024-04-17 12:28:15.516164 mistral_common-1.0.2/src/mistral_common/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:28:15.328168 mistral_common-1.0.2/src/mistral_common/protocol/__init__.py
+-rw-r--r--   0        0        0      199 2024-04-17 12:28:15.333167 mistral_common-1.0.2/src/mistral_common/protocol/base.py
+-rw-r--r--   0        0        0      400 2024-04-17 12:28:15.339167 mistral_common-1.0.2/src/mistral_common/protocol/embedding/request.py
+-rw-r--r--   0        0        0      873 2024-04-17 12:28:15.344167 mistral_common-1.0.2/src/mistral_common/protocol/embedding/response.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:28:15.375166 mistral_common-1.0.2/src/mistral_common/protocol/instruct/__init__.py
+-rw-r--r--   0        0        0     1376 2024-04-17 12:28:15.380167 mistral_common-1.0.2/src/mistral_common/protocol/instruct/messages.py
+-rw-r--r--   0        0        0      956 2024-04-17 12:28:15.397171 mistral_common-1.0.2/src/mistral_common/protocol/instruct/request.py
+-rw-r--r--   0        0        0     1918 2024-04-17 12:28:15.384183 mistral_common-1.0.2/src/mistral_common/protocol/instruct/response.py
+-rw-r--r--   0        0        0      658 2024-04-17 12:28:15.388166 mistral_common-1.0.2/src/mistral_common/protocol/instruct/tool_calls.py
+-rw-r--r--   0        0        0    10534 2024-04-17 12:28:15.393166 mistral_common-1.0.2/src/mistral_common/protocol/instruct/validator.py
+-rw-r--r--   0        0        0       73 2024-04-17 12:28:15.403166 mistral_common-1.0.2/src/mistral_common/protocol/utils.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:28:15.408165 mistral_common-1.0.2/src/mistral_common/py.typed
+-rw-r--r--   0        0        0        0 2024-04-17 12:28:15.421165 mistral_common-1.0.2/src/mistral_common/tokens/__init__.py
+-rw-r--r--   0        0        0     6119 2024-04-17 12:28:15.443166 mistral_common-1.0.2/src/mistral_common/tokens/instruct/normalize.py
+-rw-r--r--   0        0        0      418 2024-04-17 12:28:15.448166 mistral_common-1.0.2/src/mistral_common/tokens/instruct/request.py
+-rw-r--r--   0        0        0     1481 2024-04-17 12:28:15.481165 mistral_common-1.0.2/src/mistral_common/tokens/tokenizers/base.py
+-rw-r--r--   0        0        0     4660 2024-04-17 14:19:11.465776 mistral_common-1.0.2/src/mistral_common/tokens/tokenizers/mistral.py
+-rw-r--r--   0        0        0    12394 2024-04-17 12:28:15.490165 mistral_common-1.0.2/src/mistral_common/tokens/tokenizers/sentencepiece.py
+-rw-r--r--   0        0        0      187 2024-04-17 12:28:15.476165 mistral_common-1.0.2/src/mistral_common/tokens/tokenizers/utils.py
+-rw-r--r--   0        0        0     3550 1970-01-01 00:00:00.000000 mistral_common-1.0.2/PKG-INFO
```

### Comparing `mistral_common-1.0.1/README.md` & `mistral_common-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mistral_common-1.0.1/pyproject.toml` & `mistral_common-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mistral_common"
-version = "v1.0.1"
+version = "v1.0.2"
 description = ""
 authors = ["bam4d <bam4d@mistral.ai>"]
 readme = "README.md"
 packages = [{ include = "mistral_common", from = "src" }]
 
 [tool.ruff]
 lint.select = ["E", "F", "W", "Q", "I"]
```

### Comparing `mistral_common-1.0.1/src/mistral_common/data/mistral_instruct_tokenizer_240216.model.v2` & `mistral_common-1.0.2/src/mistral_common/data/mistral_instruct_tokenizer_240216.model.v2`

 * *Files identical despite different names*

### Comparing `mistral_common-1.0.1/src/mistral_common/data/mistral_instruct_tokenizer_240216.model.v3` & `mistral_common-1.0.2/src/mistral_common/data/mistral_instruct_tokenizer_240216.model.v3`

 * *Files identical despite different names*

### Comparing `mistral_common-1.0.1/src/mistral_common/data/tokenizer.model.v1` & `mistral_common-1.0.2/src/mistral_common/data/tokenizer.model.v1`

 * *Files identical despite different names*

### Comparing `mistral_common-1.0.1/src/mistral_common/exceptions.py` & `mistral_common-1.0.2/src/mistral_common/exceptions.py`

 * *Files identical despite different names*

### Comparing `mistral_common-1.0.1/src/mistral_common/protocol/embedding/response.py` & `mistral_common-1.0.2/src/mistral_common/protocol/embedding/response.py`

 * *Files identical despite different names*

### Comparing `mistral_common-1.0.1/src/mistral_common/protocol/instruct/messages.py` & `mistral_common-1.0.2/src/mistral_common/protocol/instruct/messages.py`

 * *Files identical despite different names*

### Comparing `mistral_common-1.0.1/src/mistral_common/protocol/instruct/request.py` & `mistral_common-1.0.2/src/mistral_common/protocol/instruct/request.py`

 * *Files identical despite different names*

### Comparing `mistral_common-1.0.1/src/mistral_common/protocol/instruct/response.py` & `mistral_common-1.0.2/src/mistral_common/protocol/instruct/response.py`

 * *Files identical despite different names*

### Comparing `mistral_common-1.0.1/src/mistral_common/protocol/instruct/tool_calls.py` & `mistral_common-1.0.2/src/mistral_common/protocol/instruct/tool_calls.py`

 * *Files identical despite different names*

### Comparing `mistral_common-1.0.1/src/mistral_common/protocol/instruct/validator.py` & `mistral_common-1.0.2/src/mistral_common/protocol/instruct/validator.py`

 * *Files identical despite different names*

### Comparing `mistral_common-1.0.1/src/mistral_common/tokens/instruct/normalize.py` & `mistral_common-1.0.2/src/mistral_common/tokens/instruct/normalize.py`

 * *Files identical despite different names*

### Comparing `mistral_common-1.0.1/src/mistral_common/tokens/tokenizers/base.py` & `mistral_common-1.0.2/src/mistral_common/tokens/tokenizers/base.py`

 * *Files identical despite different names*

### Comparing `mistral_common-1.0.1/src/mistral_common/tokens/tokenizers/mistral.py` & `mistral_common-1.0.2/src/mistral_common/tokens/tokenizers/mistral.py`

 * *Files identical despite different names*

### Comparing `mistral_common-1.0.1/src/mistral_common/tokens/tokenizers/sentencepiece.py` & `mistral_common-1.0.2/src/mistral_common/tokens/tokenizers/sentencepiece.py`

 * *Files identical despite different names*

### Comparing `mistral_common-1.0.1/PKG-INFO` & `mistral_common-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistral_common
-Version: 1.0.1
+Version: 1.0.2
 Summary: 
 Author: bam4d
 Author-email: bam4d@mistral.ai
 Requires-Python: >=3.8.10,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

