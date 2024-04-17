# Comparing `tmp/llama_index_embeddings_cohere-0.1.7.tar.gz` & `tmp/llama_index_embeddings_cohere-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_embeddings_cohere-0.1.7.tar", max compression
+gzip compressed data, was "llama_index_embeddings_cohere-0.1.8.tar", max compression
```

## Comparing `llama_index_embeddings_cohere-0.1.7.tar` & `llama_index_embeddings_cohere-0.1.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       44 2024-04-11 16:35:44.894788 llama_index_embeddings_cohere-0.1.7/README.md
--rw-r--r--   0        0        0       94 2024-04-11 16:35:44.894788 llama_index_embeddings_cohere-0.1.7/llama_index/embeddings/cohere/__init__.py
--rw-r--r--   0        0        0     9394 2024-04-11 16:35:44.894788 llama_index_embeddings_cohere-0.1.7/llama_index/embeddings/cohere/base.py
--rw-r--r--   0        0        0     1466 2024-04-11 16:35:44.894788 llama_index_embeddings_cohere-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 llama_index_embeddings_cohere-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       44 2024-04-17 19:23:24.482014 llama_index_embeddings_cohere-0.1.8/README.md
+-rw-r--r--   0        0        0       94 2024-04-17 19:23:24.482014 llama_index_embeddings_cohere-0.1.8/llama_index/embeddings/cohere/__init__.py
+-rw-r--r--   0        0        0     9459 2024-04-17 19:23:24.482014 llama_index_embeddings_cohere-0.1.8/llama_index/embeddings/cohere/base.py
+-rw-r--r--   0        0        0     1493 2024-04-17 19:23:24.482014 llama_index_embeddings_cohere-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 llama_index_embeddings_cohere-0.1.8/PKG-INFO
```

### Comparing `llama_index_embeddings_cohere-0.1.7/llama_index/embeddings/cohere/base.py` & `llama_index_embeddings_cohere-0.1.8/llama_index/embeddings/cohere/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,16 @@
         truncate: str = "END",
         input_type: Optional[str] = None,
         embedding_type: str = "float",
         embed_batch_size: int = DEFAULT_EMBED_BATCH_SIZE,
         callback_manager: Optional[CallbackManager] = None,
         base_url: Optional[str] = None,
         timeout: Optional[float] = None,
-        httpx_client: Optional[httpx.AsyncClient] = None,
+        httpx_client: Optional[httpx.Client] = None,
+        httpx_async_client: Optional[httpx.AsyncClient] = None,
     ):
         """
         A class representation for generating embeddings using the Cohere API.
 
         Args:
             cohere_client (Any): An instance of the Cohere client, which is used to communicate with the Cohere API.
             truncate (str): A string indicating the truncation strategy to be applied to input text. Possible values
@@ -166,15 +167,15 @@
                 httpx_client=httpx_client,
             ),
             cohere_async_client=cohere.AsyncClient(
                 cohere_api_key,
                 client_name="llama_index",
                 base_url=base_url,
                 timeout=timeout,
-                httpx_client=httpx_client,
+                httpx_client=httpx_async_client,
             ),
             cohere_api_key=cohere_api_key,
             model_name=model_name,
             input_type=input_type,
             embedding_type=embedding_type,
             truncate=truncate,
             embed_batch_size=embed_batch_size,
```

### Comparing `llama_index_embeddings_cohere-0.1.7/pyproject.toml` & `llama_index_embeddings_cohere-0.1.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -23,28 +23,29 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index embeddings cohere integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-embeddings-cohere"
 readme = "README.md"
-version = "0.1.7"
+version = "0.1.8"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 cohere = "^5.2.5"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
 pytest = "7.2.1"
+pytest-asyncio = "^0.23.6"
 pytest-mock = "3.11.1"
 ruff = "0.0.292"
 tree-sitter-languages = "^1.8.0"
 types-Deprecated = ">=0.1.0"
 types-PyYAML = "^6.0.12.12"
 types-protobuf = "^4.24.0.4"
 types-redis = "4.5.5.0"
```

### Comparing `llama_index_embeddings_cohere-0.1.7/PKG-INFO` & `llama_index_embeddings_cohere-0.1.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-embeddings-cohere
-Version: 0.1.7
+Version: 0.1.8
 Summary: llama-index embeddings cohere integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

