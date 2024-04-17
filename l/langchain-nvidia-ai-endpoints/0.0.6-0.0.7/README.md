# Comparing `tmp/langchain_nvidia_ai_endpoints-0.0.6.tar.gz` & `tmp/langchain_nvidia_ai_endpoints-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_nvidia_ai_endpoints-0.0.6.tar", max compression
+gzip compressed data, was "langchain_nvidia_ai_endpoints-0.0.7.tar", max compression
```

## Comparing `langchain_nvidia_ai_endpoints-0.0.6.tar` & `langchain_nvidia_ai_endpoints-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1072 2024-04-10 13:05:45.926275 langchain_nvidia_ai_endpoints-0.0.6/LICENSE
--rw-r--r--   0        0        0    10720 2024-04-10 13:05:45.926275 langchain_nvidia_ai_endpoints-0.0.6/README.md
--rw-r--r--   0        0        0     2070 2024-04-10 13:05:45.934275 langchain_nvidia_ai_endpoints-0.0.6/langchain_nvidia_ai_endpoints/__init__.py
--rw-r--r--   0        0        0    29740 2024-04-10 13:05:45.934275 langchain_nvidia_ai_endpoints-0.0.6/langchain_nvidia_ai_endpoints/_common.py
--rw-r--r--   0        0        0     5659 2024-04-10 13:05:45.934275 langchain_nvidia_ai_endpoints-0.0.6/langchain_nvidia_ai_endpoints/_statics.py
--rw-r--r--   0        0        0    10149 2024-04-10 13:05:45.934275 langchain_nvidia_ai_endpoints-0.0.6/langchain_nvidia_ai_endpoints/callbacks.py
--rw-r--r--   0        0        0    15758 2024-04-10 13:05:45.934275 langchain_nvidia_ai_endpoints-0.0.6/langchain_nvidia_ai_endpoints/chat_models.py
--rw-r--r--   0        0        0     4955 2024-04-10 13:05:45.934275 langchain_nvidia_ai_endpoints-0.0.6/langchain_nvidia_ai_endpoints/embeddings.py
--rw-r--r--   0        0        0     5735 2024-04-10 13:05:45.934275 langchain_nvidia_ai_endpoints-0.0.6/langchain_nvidia_ai_endpoints/image_gen.py
--rw-r--r--   0        0        0     7597 2024-04-10 13:05:45.934275 langchain_nvidia_ai_endpoints-0.0.6/langchain_nvidia_ai_endpoints/llm.py
--rw-r--r--   0        0        0        0 2024-04-10 13:05:45.934275 langchain_nvidia_ai_endpoints-0.0.6/langchain_nvidia_ai_endpoints/py.typed
--rw-r--r--   0        0        0    10047 2024-04-10 13:05:45.934275 langchain_nvidia_ai_endpoints-0.0.6/langchain_nvidia_ai_endpoints/tools.py
--rw-r--r--   0        0        0     2894 2024-04-10 13:05:45.934275 langchain_nvidia_ai_endpoints-0.0.6/pyproject.toml
--rw-r--r--   0        0        0    11619 1970-01-01 00:00:00.000000 langchain_nvidia_ai_endpoints-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-17 15:51:53.209527 langchain_nvidia_ai_endpoints-0.0.7/LICENSE
+-rw-r--r--   0        0        0    10720 2024-04-17 15:51:53.209527 langchain_nvidia_ai_endpoints-0.0.7/README.md
+-rw-r--r--   0        0        0     2070 2024-04-17 15:51:53.213528 langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/__init__.py
+-rw-r--r--   0        0        0    29740 2024-04-17 15:51:53.213528 langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/_common.py
+-rw-r--r--   0        0        0     6441 2024-04-17 15:51:53.213528 langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/_statics.py
+-rw-r--r--   0        0        0    10149 2024-04-17 15:51:53.213528 langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/callbacks.py
+-rw-r--r--   0        0        0    16465 2024-04-17 15:51:53.213528 langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/chat_models.py
+-rw-r--r--   0        0        0     5442 2024-04-17 15:51:53.213528 langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/embeddings.py
+-rw-r--r--   0        0        0     5735 2024-04-17 15:51:53.213528 langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/image_gen.py
+-rw-r--r--   0        0        0     7597 2024-04-17 15:51:53.213528 langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/llm.py
+-rw-r--r--   0        0        0        0 2024-04-17 15:51:53.213528 langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/py.typed
+-rw-r--r--   0        0        0    10047 2024-04-17 15:51:53.213528 langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/tools.py
+-rw-r--r--   0        0        0     2894 2024-04-17 15:51:53.213528 langchain_nvidia_ai_endpoints-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0    11619 1970-01-01 00:00:00.000000 langchain_nvidia_ai_endpoints-0.0.7/PKG-INFO
```

### Comparing `langchain_nvidia_ai_endpoints-0.0.6/LICENSE` & `langchain_nvidia_ai_endpoints-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.6/README.md` & `langchain_nvidia_ai_endpoints-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.6/langchain_nvidia_ai_endpoints/__init__.py` & `langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.6/langchain_nvidia_ai_endpoints/_common.py` & `langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/_common.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.6/langchain_nvidia_ai_endpoints/_statics.py` & `langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/_statics.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,40 +11,88 @@
     client: Optional[str] = None
     path: str
 
 
 MODEL_SPECS = {
     "playground_smaug_72b": {"model_type": "chat", "api_type": "aifm"},
     "playground_kosmos_2": {"model_type": "image_in", "api_type": "aifm"},
-    "playground_llama2_70b": {"model_type": "chat", "api_type": "aifm"},
+    "playground_llama2_70b": {
+        "model_type": "chat",
+        "api_type": "aifm",
+        "alternative": "ai-llama2-70b",
+    },
     "playground_nvolveqa_40k": {"model_type": "embedding", "api_type": "aifm"},
     "playground_nemotron_qa_8b": {"model_type": "qa", "api_type": "aifm"},
-    "playground_gemma_7b": {"model_type": "chat", "api_type": "aifm"},
-    "playground_mistral_7b": {"model_type": "chat", "api_type": "aifm"},
+    "playground_gemma_7b": {
+        "model_type": "chat",
+        "api_type": "aifm",
+        "alternative": "ai-gemma-7b",
+    },
+    "playground_mistral_7b": {
+        "model_type": "chat",
+        "api_type": "aifm",
+        "alternative": "ai-mistral-7b-instruct-v2",
+    },
     "playground_mamba_chat": {"model_type": "chat", "api_type": "aifm"},
     "playground_phi2": {"model_type": "chat", "api_type": "aifm"},
     "playground_sdxl": {"model_type": "image_out", "api_type": "aifm"},
     "playground_nv_llama2_rlhf_70b": {"model_type": "chat", "api_type": "aifm"},
-    "playground_neva_22b": {"model_type": "image_in", "api_type": "aifm"},
+    "playground_neva_22b": {
+        "model_type": "image_in",
+        "api_type": "aifm",
+        "alternative": "ai-neva-22b",
+    },
     "playground_yi_34b": {"model_type": "chat", "api_type": "aifm"},
     "playground_nemotron_steerlm_8b": {"model_type": "chat", "api_type": "aifm"},
     "playground_cuopt": {"model_type": "cuopt", "api_type": "aifm"},
     "playground_llama_guard": {"model_type": "classifier", "api_type": "aifm"},
     "playground_starcoder2_15b": {"model_type": "completion", "api_type": "aifm"},
-    "playground_deplot": {"model_type": "image_in", "api_type": "aifm"},
-    "playground_llama2_code_70b": {"model_type": "chat", "api_type": "aifm"},
-    "playground_gemma_2b": {"model_type": "chat", "api_type": "aifm"},
+    "playground_deplot": {
+        "model_type": "image_in",
+        "api_type": "aifm",
+        "alternative": "ai-google-deplot",
+    },
+    "playground_llama2_code_70b": {
+        "model_type": "chat",
+        "api_type": "aifm",
+        "alternative": "ai-codellama-70b",
+    },
+    "playground_gemma_2b": {
+        "model_type": "chat",
+        "api_type": "aifm",
+        "alternative": "ai-gemma-2b",
+    },
     "playground_seamless": {"model_type": "translation", "api_type": "aifm"},
-    "playground_mixtral_8x7b": {"model_type": "chat", "api_type": "aifm"},
-    "playground_fuyu_8b": {"model_type": "image_in", "api_type": "aifm"},
-    "playground_llama2_code_34b": {"model_type": "chat", "api_type": "aifm"},
-    "playground_llama2_code_13b": {"model_type": "chat", "api_type": "aifm"},
+    "playground_mixtral_8x7b": {
+        "model_type": "chat",
+        "api_type": "aifm",
+        "alternative": "ai-mixtral-8x7b-instruct",
+    },
+    "playground_fuyu_8b": {
+        "model_type": "image_in",
+        "api_type": "aifm",
+        "alternative": "ai-fuyu-8b",
+    },
+    "playground_llama2_code_34b": {
+        "model_type": "chat",
+        "api_type": "aifm",
+        "alternative": "ai-codellama-70b",
+    },
+    "playground_llama2_code_13b": {
+        "model_type": "chat",
+        "api_type": "aifm",
+        "alternative": "ai-codellama-70b",
+    },
     "playground_steerlm_llama_70b": {"model_type": "chat", "api_type": "aifm"},
     "playground_clip": {"model_type": "similarity", "api_type": "aifm"},
-    "playground_llama2_13b": {"model_type": "chat", "api_type": "aifm"},
+    "playground_llama2_13b": {
+        "model_type": "chat",
+        "api_type": "aifm",
+        "alternative": "ai-llama2-70b",
+    },
 }
 
 MODEL_SPECS.update(
     {
         "ai-codellama-70b": {"model_type": "chat", "model_name": "meta/codellama-70b"},
         "ai-embed-qa-4": {"model_type": "embedding", "model_name": "NV-Embed-QA"},
         "ai-fuyu-8b": {"model_type": "image_in"},
```

### Comparing `langchain_nvidia_ai_endpoints-0.0.6/langchain_nvidia_ai_endpoints/callbacks.py` & `langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/callbacks.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.6/langchain_nvidia_ai_endpoints/chat_models.py` & `langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/chat_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import base64
 import io
 import logging
 import os
 import sys
 import urllib.parse
+import warnings
 from typing import (
     Any,
     AsyncIterator,
     Callable,
     Dict,
     Iterator,
     List,
@@ -35,20 +36,21 @@
     ChatMessageChunk,
 )
 from langchain_core.outputs import (
     ChatGeneration,
     ChatGenerationChunk,
     ChatResult,
 )
-from langchain_core.pydantic_v1 import BaseModel, Field
+from langchain_core.pydantic_v1 import BaseModel, Field, validator
 from langchain_core.runnables import Runnable
 from langchain_core.runnables.config import run_in_executor
 from langchain_core.tools import BaseTool
 
 from langchain_nvidia_ai_endpoints import _common as nvidia_ai_endpoints
+from langchain_nvidia_ai_endpoints._statics import MODEL_SPECS
 
 _CallbackManager = Union[AsyncCallbackManagerForLLMRun, CallbackManagerForLLMRun]
 _DictOrPydanticClass = Union[Dict[str, Any], Type[BaseModel]]
 _DictOrPydantic = Union[Dict, BaseModel]
 
 try:
     import PIL.Image
@@ -136,14 +138,28 @@
     top_p: Optional[float] = Field(description="Top-p for distribution sampling")
     seed: Optional[int] = Field(description="The seed for deterministic results")
     bad: Optional[Sequence[str]] = Field(description="Bad words to avoid (cased)")
     stop: Optional[Sequence[str]] = Field(description="Stop words (cased)")
     labels: Optional[Dict[str, float]] = Field(description="Steering parameters")
     streaming: bool = Field(True)
 
+    @validator("model")
+    def aifm_deprecated(cls, value: str) -> str:
+        """All AI Foundataion Models are deprecate, use API Catalog models instead."""
+        for model in [value, f"playground_{value}"]:
+            if model in MODEL_SPECS and MODEL_SPECS[model].get("api_type") == "aifm":
+                alternative = MODEL_SPECS[model].get(
+                    "alternative", ChatNVIDIA._default_model
+                )
+                warnings.warn(
+                    f"{value} is deprecated. Try {alternative} instead.",
+                    DeprecationWarning,
+                )
+        return value
+
     @property
     def _llm_type(self) -> str:
         """Return type of NVIDIA AI Foundation Model Interface."""
         return "chat-nvidia-ai-playground"
 
     def _generate(
         self,
```

### Comparing `langchain_nvidia_ai_endpoints-0.0.6/langchain_nvidia_ai_endpoints/embeddings.py` & `langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/embeddings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Embeddings Components Derived from NVEModel/Embeddings"""
 
+import warnings
 from typing import List, Literal, Optional
 
 from langchain_core.embeddings import Embeddings
 from langchain_core.outputs.llm_result import LLMResult
-from langchain_core.pydantic_v1 import Field
+from langchain_core.pydantic_v1 import Field, validator
 
 from langchain_nvidia_ai_endpoints._common import _NVIDIAClient
 from langchain_nvidia_ai_endpoints.callbacks import usage_callback_var
 
 from ._statics import MODEL_SPECS
 
 
@@ -21,14 +22,25 @@
     model: str = Field(_default_model, description="Name of the model to invoke")
     max_length: int = Field(2048, ge=1, le=2048)
     max_batch_size: int = Field(default=_default_max_batch_size)
     model_type: Optional[Literal["passage", "query"]] = Field(
         None, description="The type of text to be embedded."
     )
 
+    # todo: fix _NVIDIAClient.validate_client and enable Config.validate_assignment
+    @validator("model")
+    def deprecated_nvolveqa_40k(cls, value: str) -> str:
+        """Deprecate the nvolveqa_40k model."""
+        if value == "nvolveqa_40k" or value == "playground_nvolveqa_40k":
+            warnings.warn(
+                "nvolveqa_40k is deprecated. Use ai-embed-qa-4 instead.",
+                DeprecationWarning,
+            )
+        return value
+
     def _embed(
         self, texts: List[str], model_type: Literal["passage", "query"]
     ) -> List[List[float]]:
         """Embed a single text entry to either passage or query type"""
         # AI Foundation Model API -
         #  input: str | list[str]              -- <= 2048 characters, <= 50 inputs
         #  model: "query" | "passage"          -- type of input text to be embedded
```

### Comparing `langchain_nvidia_ai_endpoints-0.0.6/langchain_nvidia_ai_endpoints/image_gen.py` & `langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/image_gen.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.6/langchain_nvidia_ai_endpoints/llm.py` & `langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/llm.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.6/langchain_nvidia_ai_endpoints/tools.py` & `langchain_nvidia_ai_endpoints-0.0.7/langchain_nvidia_ai_endpoints/tools.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.6/pyproject.toml` & `langchain_nvidia_ai_endpoints-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-nvidia-ai-endpoints"
-version = "0.0.6"
+version = "0.0.7"
 description = "An integration package connecting NVIDIA AI Endpoints and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
```

### Comparing `langchain_nvidia_ai_endpoints-0.0.6/PKG-INFO` & `langchain_nvidia_ai_endpoints-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-nvidia-ai-endpoints
-Version: 0.0.6
+Version: 0.0.7
 Summary: An integration package connecting NVIDIA AI Endpoints and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

