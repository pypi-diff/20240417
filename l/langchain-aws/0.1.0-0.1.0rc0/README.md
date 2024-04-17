# Comparing `tmp/langchain_aws-0.1.0.tar.gz` & `tmp/langchain_aws-0.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_aws-0.1.0.tar", max compression
+gzip compressed data, was "langchain_aws-0.1.0rc0.tar", max compression
```

## Comparing `langchain_aws-0.1.0.tar` & `langchain_aws-0.1.0rc0.tar`

### file list

```diff
@@ -1,18 +1,16 @@
--rw-r--r--   0        0        0     1072 2024-04-17 20:35:58.349413 langchain_aws-0.1.0/LICENSE
--rw-r--r--   0        0        0     1534 2024-04-17 20:35:58.349413 langchain_aws-0.1.0/README.md
--rw-r--r--   0        0        0      531 2024-04-17 20:35:58.349413 langchain_aws-0.1.0/langchain_aws/__init__.py
--rw-r--r--   0        0        0      113 2024-04-17 20:35:58.349413 langchain_aws-0.1.0/langchain_aws/chat_models/__init__.py
--rw-r--r--   0        0        0    13294 2024-04-17 20:35:58.349413 langchain_aws-0.1.0/langchain_aws/chat_models/bedrock.py
--rw-r--r--   0        0        0      191 2024-04-17 20:35:58.349413 langchain_aws-0.1.0/langchain_aws/graphs/__init__.py
--rw-r--r--   0        0        0    14347 2024-04-17 20:35:58.349413 langchain_aws-0.1.0/langchain_aws/graphs/neptune_graph.py
--rw-r--r--   0        0        0    10331 2024-04-17 20:35:58.349413 langchain_aws-0.1.0/langchain_aws/graphs/neptune_rdf_graph.py
--rw-r--r--   0        0        0      297 2024-04-17 20:35:58.349413 langchain_aws-0.1.0/langchain_aws/llms/__init__.py
--rw-r--r--   0        0        0    31691 2024-04-17 20:35:58.353412 langchain_aws-0.1.0/langchain_aws/llms/bedrock.py
--rw-r--r--   0        0        0    13595 2024-04-17 20:35:58.353412 langchain_aws-0.1.0/langchain_aws/llms/sagemaker_endpoint.py
--rw-r--r--   0        0        0        0 2024-04-17 20:35:58.353412 langchain_aws-0.1.0/langchain_aws/py.typed
--rw-r--r--   0        0        0      251 2024-04-17 20:35:58.353412 langchain_aws-0.1.0/langchain_aws/retrievers/__init__.py
--rw-r--r--   0        0        0     4654 2024-04-17 20:35:58.353412 langchain_aws-0.1.0/langchain_aws/retrievers/bedrock.py
--rw-r--r--   0        0        0    15189 2024-04-17 20:35:58.353412 langchain_aws-0.1.0/langchain_aws/retrievers/kendra.py
--rw-r--r--   0        0        0     1033 2024-04-17 20:35:58.353412 langchain_aws-0.1.0/langchain_aws/utils.py
--rw-r--r--   0        0        0     2706 2024-04-17 20:35:58.353412 langchain_aws-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2341 1970-01-01 00:00:00.000000 langchain_aws-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-05 16:50:44.671510 langchain_aws-0.1.0rc0/LICENSE
+-rw-r--r--   0        0        0      820 2024-04-05 16:50:44.671510 langchain_aws-0.1.0rc0/README.md
+-rw-r--r--   0        0        0      413 2024-04-05 16:50:44.671510 langchain_aws-0.1.0rc0/langchain_aws/__init__.py
+-rw-r--r--   0        0        0      113 2024-04-05 16:50:44.671510 langchain_aws-0.1.0rc0/langchain_aws/chat_models/__init__.py
+-rw-r--r--   0        0        0    13294 2024-04-05 16:50:44.671510 langchain_aws-0.1.0rc0/langchain_aws/chat_models/bedrock.py
+-rw-r--r--   0        0        0        0 2024-04-05 16:50:44.671510 langchain_aws-0.1.0rc0/langchain_aws/graphs/__init__.py
+-rw-r--r--   0        0        0      297 2024-04-05 16:50:44.675510 langchain_aws-0.1.0rc0/langchain_aws/llms/__init__.py
+-rw-r--r--   0        0        0    31517 2024-04-05 16:50:44.675510 langchain_aws-0.1.0rc0/langchain_aws/llms/bedrock.py
+-rw-r--r--   0        0        0    13595 2024-04-05 16:50:44.675510 langchain_aws-0.1.0rc0/langchain_aws/llms/sagemaker_endpoint.py
+-rw-r--r--   0        0        0        0 2024-04-05 16:50:44.675510 langchain_aws-0.1.0rc0/langchain_aws/py.typed
+-rw-r--r--   0        0        0      251 2024-04-05 16:50:44.675510 langchain_aws-0.1.0rc0/langchain_aws/retrievers/__init__.py
+-rw-r--r--   0        0        0     4654 2024-04-05 16:50:44.675510 langchain_aws-0.1.0rc0/langchain_aws/retrievers/bedrock.py
+-rw-r--r--   0        0        0    15189 2024-04-05 16:50:44.675510 langchain_aws-0.1.0rc0/langchain_aws/retrievers/kendra.py
+-rw-r--r--   0        0        0     1033 2024-04-05 16:50:44.675510 langchain_aws-0.1.0rc0/langchain_aws/utils.py
+-rw-r--r--   0        0        0     2376 2024-04-05 16:50:44.675510 langchain_aws-0.1.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     1630 1970-01-01 00:00:00.000000 langchain_aws-0.1.0rc0/PKG-INFO
```

### Comparing `langchain_aws-0.1.0/LICENSE` & `langchain_aws-0.1.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.0/langchain_aws/chat_models/bedrock.py` & `langchain_aws-0.1.0rc0/langchain_aws/chat_models/bedrock.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.0/langchain_aws/llms/bedrock.py` & `langchain_aws-0.1.0rc0/langchain_aws/llms/bedrock.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 )
 
 from langchain_core._api.deprecation import deprecated
 from langchain_core.callbacks import (
     AsyncCallbackManagerForLLMRun,
     CallbackManagerForLLMRun,
 )
-from langchain_core.language_models import LLM, BaseLanguageModel
+from langchain_core.language_models.llms import LLM
 from langchain_core.outputs import GenerationChunk
-from langchain_core.pydantic_v1 import Extra, Field, root_validator
+from langchain_core.pydantic_v1 import BaseModel, Extra, Field, root_validator
 from langchain_core.utils import get_from_dict_or_env
 
 from langchain_aws.utils import (
     enforce_stop_tokens,
     get_num_tokens_anthropic,
     get_token_ids_anthropic,
 )
@@ -288,15 +288,15 @@
                     chunk_obj[output_key]
                     if provider != "mistral"
                     else chunk_obj[output_key][0]["text"]
                 )
             )
 
 
-class BedrockBase(BaseLanguageModel, ABC):
+class BedrockBase(BaseModel, ABC):
     """Base class for Bedrock models."""
 
     client: Any = Field(exclude=True)  #: :meta private:
 
     region_name: Optional[str] = None
     """The aws region e.g., `us-west-2`. Fallsback to AWS_DEFAULT_REGION env variable
     or region specified in ~/.aws/config in case it is not provided here.
@@ -321,15 +321,15 @@
     associated with them."""
 
     model_id: str
     """Id of the model to call, e.g., amazon.titan-text-express-v1, this is
     equivalent to the modelId property in the list-foundation-models api. For custom and
     provisioned models, an ARN value is expected."""
 
-    model_kwargs: Optional[Dict[str, Any]] = None
+    model_kwargs: Optional[Dict] = None
     """Keyword arguments to pass to the model."""
 
     endpoint_url: Optional[str] = None
     """Needed if you don't want to default to us-east-1 endpoint"""
 
     streaming: bool = False
     """Whether to stream the results."""
@@ -436,22 +436,19 @@
                 "Please check that credentials in the specified "
                 f"profile name are valid. Bedrock error: {e}"
             ) from e
 
         return values
 
     @property
-    def _identifying_params(self) -> Dict[str, Any]:
+    def _identifying_params(self) -> Mapping[str, Any]:
+        """Get the identifying parameters."""
         _model_kwargs = self.model_kwargs or {}
         return {
-            "model_id": self.model_id,
-            "provider": self._get_provider(),
-            "stream": self.streaming,
-            "guardrails": self.guardrails,
-            **_model_kwargs,
+            **{"model_kwargs": _model_kwargs},
         }
 
     def _get_provider(self) -> str:
         if self.provider:
             return self.provider
         if self.model_id.startswith("arn"):
             raise ValueError(
@@ -616,16 +613,15 @@
             if provider not in self.provider_stop_sequence_key_name_map:
                 raise ValueError(
                     f"Stop sequence key name for {provider} is not supported."
                 )
 
             # stop sequence from _generate() overrides
             # stop sequences in the class attribute
-            if k := self.provider_stop_sequence_key_name_map.get(provider):
-                _model_kwargs[k] = stop
+            _model_kwargs[self.provider_stop_sequence_key_name_map.get(provider)] = stop
 
         if provider == "cohere":
             _model_kwargs["stream"] = True
 
         params = {**_model_kwargs, **kwargs}
 
         if self._guardrails_enabled:
@@ -679,16 +675,15 @@
         provider = self._get_provider()
 
         if stop:
             if provider not in self.provider_stop_sequence_key_name_map:
                 raise ValueError(
                     f"Stop sequence key name for {provider} is not supported."
                 )
-            if k := self.provider_stop_sequence_key_name_map.get(provider):
-                _model_kwargs[k] = stop
+            _model_kwargs[self.provider_stop_sequence_key_name_map.get(provider)] = stop
 
         if provider == "cohere":
             _model_kwargs["stream"] = True
 
         params = {**_model_kwargs, **kwargs}
         input_body = LLMInputOutputAdapter.prepare_input(
             provider=provider, prompt=prompt, model_kwargs=params
```

### Comparing `langchain_aws-0.1.0/langchain_aws/llms/sagemaker_endpoint.py` & `langchain_aws-0.1.0rc0/langchain_aws/llms/sagemaker_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.0/langchain_aws/retrievers/bedrock.py` & `langchain_aws-0.1.0rc0/langchain_aws/retrievers/bedrock.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.0/langchain_aws/retrievers/kendra.py` & `langchain_aws-0.1.0rc0/langchain_aws/retrievers/kendra.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.0/langchain_aws/utils.py` & `langchain_aws-0.1.0rc0/langchain_aws/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.0/pyproject.toml` & `langchain_aws-0.1.0rc0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-aws"
-version = "0.1.0"
+version = "0.1.0rc0"
 description = "An integration package connecting AWS and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-aws"
 license = "MIT"
 
 [tool.poetry.urls]
@@ -19,15 +19,14 @@
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.3"
 pytest-cov = "^4.1.0"
 syrupy = "^4.0.2"
 pytest-asyncio = "^0.23.2"
-langchain-core = {git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core"}
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.6"
 
@@ -40,22 +39,19 @@
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.8"
 
 [tool.poetry.group.typing.dependencies]
 mypy = "^1.7.1"
-types-requests = "^2.28.11.5"
-langchain-core = {git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core"}
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-langchain-core = {git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core"}
 
 [tool.ruff.lint]
 select = [
   "E",    # pycodestyle
   "F",    # pyflakes
   "I",    # isort
   "T201", # print
```

### Comparing `langchain_aws-0.1.0/PKG-INFO` & `langchain_aws-0.1.0rc0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-aws
-Version: 0.1.0
+Version: 0.1.0rc0
 Summary: An integration package connecting AWS and LangChain
 Home-page: https://github.com/langchain-ai/langchain-aws
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -15,22 +15,25 @@
 Requires-Dist: langchain-core (>=0.1,<0.2)
 Project-URL: Repository, https://github.com/langchain-ai/langchain-aws
 Project-URL: Source Code, https://github.com/langchain-ai/langchain-aws/tree/main/libs/aws
 Description-Content-Type: text/markdown
 
 # langchain-aws
 
-This package contains the LangChain integrations with AWS.
+This package contains the LangChain integration with Bedrock
 
 ## Installation
 
 ```bash
 pip install -U langchain-aws
 ```
-All integrations in this package assume that you have the credentials setup to connect with AWS services.
+
+And you should configure credentials by setting the following environment variables:
+
+* TODO: fill this out
 
 ## Chat Models
 
 `ChatBedrock` class exposes chat models from Bedrock.
 
 ```python
 from langchain_aws import ChatBedrock
@@ -56,32 +59,7 @@
 ```python
 from langchain_aws import BedrockLLM
 
 llm = BedrockLLM()
 llm.invoke("The meaning of life is")
 ```
 
-## Retrievers
-`AmazonKendraRetriever` class provides a retriever to connect with Amazon Kendra.
-
-```python
-from langchain_aws import AmazonKendraRetriever
-
-retriever = AmazonKendraRetriever(
-    index_id="561be2b6d-9804c7e7-f6a0fbb8-5ccd350"
-)
-
-retriever.get_relevant_documents(query="What is the meaning of life?")
-```
-
-`AmazonKnowlegeBasesRetriever` class provides a retriever to connect with Amazon Knowlege Bases.
-
-```python
-from langchain_aws import AmazonKnowledgeBasesRetriever
-
-retriever = AmazonKnowledgeBasesRetriever(
-    knowledge_base_id="IAPJ4QPUEU",
-    retrieval_config={"vectorSearchConfiguration": {"numberOfResults": 4}},
-)
-
-retriever.get_relevant_documents(query="What is the meaning of life?")
-```
```

