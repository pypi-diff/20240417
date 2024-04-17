# Comparing `tmp/langchain_cohere-0.1.3rc0.tar.gz` & `tmp/langchain_cohere-0.1.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_cohere-0.1.3rc0.tar", max compression
+gzip compressed data, was "langchain_cohere-0.1.3rc1.tar", max compression
```

## Comparing `langchain_cohere-0.1.3rc0.tar` & `langchain_cohere-0.1.3rc1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1072 2024-04-12 18:56:41.673409 langchain_cohere-0.1.3rc0/LICENSE
--rw-r--r--   0        0        0     3796 2024-04-12 18:56:41.677409 langchain_cohere-0.1.3rc0/README.md
--rw-r--r--   0        0        0      608 2024-04-12 18:56:41.677409 langchain_cohere-0.1.3rc0/langchain_cohere/__init__.py
--rw-r--r--   0        0        0    15941 2024-04-12 18:56:41.677409 langchain_cohere-0.1.3rc0/langchain_cohere/chat_models.py
--rw-r--r--   0        0        0     8173 2024-04-12 18:56:41.677409 langchain_cohere-0.1.3rc0/langchain_cohere/cohere_agent.py
--rw-r--r--   0        0        0     1215 2024-04-12 18:56:41.677409 langchain_cohere-0.1.3rc0/langchain_cohere/common.py
--rw-r--r--   0        0        0     5366 2024-04-12 18:56:41.677409 langchain_cohere-0.1.3rc0/langchain_cohere/embeddings.py
--rw-r--r--   0        0        0     8050 2024-04-12 18:56:41.677409 langchain_cohere-0.1.3rc0/langchain_cohere/llms.py
--rw-r--r--   0        0        0        0 2024-04-12 18:56:41.677409 langchain_cohere-0.1.3rc0/langchain_cohere/py.typed
--rw-r--r--   0        0        0     3349 2024-04-12 18:56:41.677409 langchain_cohere-0.1.3rc0/langchain_cohere/rag_retrievers.py
--rw-r--r--   0        0        0        0 2024-04-12 18:56:41.677409 langchain_cohere-0.1.3rc0/langchain_cohere/react_multi_hop/__init__.py
--rw-r--r--   0        0        0     4899 2024-04-12 18:56:41.677409 langchain_cohere-0.1.3rc0/langchain_cohere/react_multi_hop/agent.py
--rw-r--r--   0        0        0     4059 2024-04-12 18:56:41.677409 langchain_cohere-0.1.3rc0/langchain_cohere/react_multi_hop/default_prompt_constants.py
--rw-r--r--   0        0        0    10974 2024-04-12 18:56:41.677409 langchain_cohere-0.1.3rc0/langchain_cohere/react_multi_hop/parsing.py
--rw-r--r--   0        0        0     9635 2024-04-12 18:56:41.677409 langchain_cohere-0.1.3rc0/langchain_cohere/react_multi_hop/prompt.py
--rw-r--r--   0        0        0     3995 2024-04-12 18:56:41.677409 langchain_cohere-0.1.3rc0/langchain_cohere/rerank.py
--rw-r--r--   0        0        0     1655 2024-04-12 18:56:41.677409 langchain_cohere-0.1.3rc0/langchain_cohere/utils.py
--rw-r--r--   0        0        0     2640 2024-04-12 18:56:41.677409 langchain_cohere-0.1.3rc0/pyproject.toml
--rw-r--r--   0        0        0     4626 1970-01-01 00:00:00.000000 langchain_cohere-0.1.3rc0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-17 09:47:47.788452 langchain_cohere-0.1.3rc1/LICENSE
+-rw-r--r--   0        0        0     5585 2024-04-17 09:47:47.788452 langchain_cohere-0.1.3rc1/README.md
+-rw-r--r--   0        0        0      608 2024-04-17 09:47:47.788452 langchain_cohere-0.1.3rc1/langchain_cohere/__init__.py
+-rw-r--r--   0        0        0    17262 2024-04-17 09:47:47.788452 langchain_cohere-0.1.3rc1/langchain_cohere/chat_models.py
+-rw-r--r--   0        0        0     8173 2024-04-17 09:47:47.788452 langchain_cohere-0.1.3rc1/langchain_cohere/cohere_agent.py
+-rw-r--r--   0        0        0     1215 2024-04-17 09:47:47.792452 langchain_cohere-0.1.3rc1/langchain_cohere/common.py
+-rw-r--r--   0        0        0     5813 2024-04-17 09:47:47.792452 langchain_cohere-0.1.3rc1/langchain_cohere/embeddings.py
+-rw-r--r--   0        0        0     8058 2024-04-17 09:47:47.792452 langchain_cohere-0.1.3rc1/langchain_cohere/llms.py
+-rw-r--r--   0        0        0        0 2024-04-17 09:47:47.792452 langchain_cohere-0.1.3rc1/langchain_cohere/py.typed
+-rw-r--r--   0        0        0     3349 2024-04-17 09:47:47.792452 langchain_cohere-0.1.3rc1/langchain_cohere/rag_retrievers.py
+-rw-r--r--   0        0        0        0 2024-04-17 09:47:47.792452 langchain_cohere-0.1.3rc1/langchain_cohere/react_multi_hop/__init__.py
+-rw-r--r--   0        0        0     4899 2024-04-17 09:47:47.792452 langchain_cohere-0.1.3rc1/langchain_cohere/react_multi_hop/agent.py
+-rw-r--r--   0        0        0     4060 2024-04-17 09:47:47.792452 langchain_cohere-0.1.3rc1/langchain_cohere/react_multi_hop/default_prompt_constants.py
+-rw-r--r--   0        0        0    10981 2024-04-17 09:47:47.792452 langchain_cohere-0.1.3rc1/langchain_cohere/react_multi_hop/parsing.py
+-rw-r--r--   0        0        0     9694 2024-04-17 09:47:47.792452 langchain_cohere-0.1.3rc1/langchain_cohere/react_multi_hop/prompt.py
+-rw-r--r--   0        0        0     4134 2024-04-17 09:47:47.792452 langchain_cohere-0.1.3rc1/langchain_cohere/rerank.py
+-rw-r--r--   0        0        0     1655 2024-04-17 09:47:47.792452 langchain_cohere-0.1.3rc1/langchain_cohere/utils.py
+-rw-r--r--   0        0        0     2682 2024-04-17 09:47:47.792452 langchain_cohere-0.1.3rc1/pyproject.toml
+-rw-r--r--   0        0        0     6413 1970-01-01 00:00:00.000000 langchain_cohere-0.1.3rc1/PKG-INFO
```

### Comparing `langchain_cohere-0.1.3rc0/LICENSE` & `langchain_cohere-0.1.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.3rc0/langchain_cohere/__init__.py` & `langchain_cohere-0.1.3rc1/langchain_cohere/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.3rc0/langchain_cohere/chat_models.py` & `langchain_cohere-0.1.3rc1/langchain_cohere/chat_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 from typing import (
+    TYPE_CHECKING,
     Any,
     AsyncIterator,
     Callable,
     Dict,
     Iterator,
     List,
     Optional,
@@ -38,24 +39,27 @@
 )
 from langchain_core.output_parsers.base import OutputParserLike
 from langchain_core.output_parsers.openai_tools import (
     JsonOutputKeyToolsParser,
     PydanticToolsParser,
 )
 from langchain_core.outputs import ChatGeneration, ChatGenerationChunk, ChatResult
-from langchain_core.pydantic_v1 import BaseModel
+from langchain_core.pydantic_v1 import BaseModel, PrivateAttr
 from langchain_core.runnables import Runnable
 from langchain_core.tools import BaseTool
 
 from langchain_cohere.cohere_agent import (
     _convert_to_cohere_tool,
     _format_to_cohere_tools,
 )
 from langchain_cohere.llms import BaseCohere
 
+if TYPE_CHECKING:
+    from cohere.types import ListModelsResponse  # noqa: F401
+
 
 def get_role(message: BaseMessage) -> str:
     """Get the role of the message.
 
     Args:
         message: The message.
 
@@ -143,55 +147,53 @@
         **kwargs,
     }
 
     return {k: v for k, v in req.items() if v is not None}
 
 
 class ChatCohere(BaseChatModel, BaseCohere):
-    """`Cohere` chat large language models.
+    """
+    Implements the BaseChatModel (and BaseLanguageModel) interface with Cohere's large
+    language models.
+
+    Find out more about us at https://cohere.com and https://huggingface.co/CohereForAI
+
+    This implementation uses the Chat API - see https://docs.cohere.com/reference/chat
+
+    To use this you'll need to a Cohere API key - either pass it to cohere_api_key
+    parameter or set the COHERE_API_KEY environment variable.
 
-    To use, you should have the ``cohere`` python package installed, and the
-    environment variable ``COHERE_API_KEY`` set with your API key, or pass
-    it as a named parameter to the constructor.
+    API keys are available on https://cohere.com - it's free to sign up and trial API
+    keys work with this implementation.
 
-    Example:
+    Basic Example:
         .. code-block:: python
 
             from langchain_cohere import ChatCohere
             from langchain_core.messages import HumanMessage
 
-            chat = ChatCohere(cohere_api_key="my-api-key")
+            llm = ChatCohere(cohere_api_key="{API KEY}")
 
-            messages = [HumanMessage(content="knock knock")]
-            chat.invoke(messages)
+            message = [HumanMessage(content="Hello, can you introduce yourself?")]
+
+            print(llm.invoke(message).content)
     """
 
     preamble: Optional[str] = None
 
+    _default_model_name: Optional[str] = PrivateAttr(
+        default=None
+    )  # Used internally to cache API calls to list models.
+
     class Config:
         """Configuration for this pydantic object."""
 
         allow_population_by_field_name = True
         arbitrary_types_allowed = True
 
-    @property
-    def _llm_type(self) -> str:
-        """Return type of chat model."""
-        return "cohere-chat"
-
-    @property
-    def _default_params(self) -> Dict[str, Any]:
-        """Get the default parameters for calling Cohere API."""
-        base_params = {
-            "model": self.model,
-            "temperature": self.temperature,
-            "preamble": self.preamble,
-        }
-        return {k: v for k, v in base_params.items() if v is not None}
-
     def bind_tools(
         self,
         tools: Sequence[Union[Dict[str, Any], Type[BaseModel], Callable, BaseTool]],
         **kwargs: Any,
     ) -> Runnable[LanguageModelInput, BaseMessage]:
         formatted_tools = _format_to_cohere_tools(tools)
         return super().bind(tools=formatted_tools, **kwargs)
@@ -224,14 +226,28 @@
             output_parser = JsonOutputKeyToolsParser(
                 key_name=key_name, first_tool_only=True
             )
 
         return llm | output_parser
 
     @property
+    def _llm_type(self) -> str:
+        """Return type of chat model."""
+        return "cohere-chat"
+
+    @property
+    def _default_params(self) -> Dict[str, Any]:
+        """Get the default parameters for calling Cohere API."""
+        base_params = {
+            "model": self.model,
+            "temperature": self.temperature,
+        }
+        return {k: v for k, v in base_params.items() if v is not None}
+
+    @property
     def _identifying_params(self) -> Dict[str, Any]:
         """Get the identifying parameters."""
         return self._default_params
 
     def _stream(
         self,
         messages: List[BaseMessage],
@@ -420,17 +436,35 @@
         )
         return ChatResult(
             generations=[
                 ChatGeneration(message=message, generation_info=generation_info)
             ]
         )
 
+    def _get_default_model(self) -> str:
+        """Fetches the current default model name."""
+        response = self.client.models.list(default_only=True, endpoint="chat")  # type: "ListModelsResponse"
+        if not response.models:
+            raise Exception("invalid cohere list models response")
+        if not response.models[0].name:
+            raise Exception("invalid cohere list models response")
+        return response.models[0].name
+
     def get_num_tokens(self, text: str) -> int:
         """Calculate number of tokens."""
-        return len(self.client.tokenize(text=text).tokens)
+        model: str
+        if self.model is not None:
+            model = self.model
+        elif self._default_model_name is not None:
+            model = self._default_model_name
+        else:
+            model = self._get_default_model()
+            self._default_model_name = model
+
+        return len(self.client.tokenize(text=text, model=model).tokens)
 
 
 def _format_cohere_tool_calls(
     generation_id: str, tool_calls: Optional[List[ToolCall]] = None
 ) -> List[Dict]:
     """
     Formats a Cohere API response into the tool call format used elsewhere in Langchain.
```

### Comparing `langchain_cohere-0.1.3rc0/langchain_cohere/cohere_agent.py` & `langchain_cohere-0.1.3rc1/langchain_cohere/cohere_agent.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.3rc0/langchain_cohere/common.py` & `langchain_cohere-0.1.3rc1/langchain_cohere/common.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.3rc0/langchain_cohere/embeddings.py` & `langchain_cohere-0.1.3rc1/langchain_cohere/embeddings.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,28 +6,39 @@
 from langchain_core.pydantic_v1 import BaseModel, Extra, root_validator
 from langchain_core.utils import get_from_dict_or_env
 
 from .utils import _create_retry_decorator
 
 
 class CohereEmbeddings(BaseModel, Embeddings):
-    """Cohere embedding models.
+    """
+    Implements the Embeddings interface with Cohere's text representation language
+    models.
+
+    Find out more about us at https://cohere.com and https://huggingface.co/CohereForAI
+
+    This implementation uses the Embed API - see https://docs.cohere.com/reference/embed
 
-    To use, you should have the ``cohere`` python package installed, and the
-    environment variable ``COHERE_API_KEY`` set with your API key or pass it
-    as a named parameter to the constructor.
+    To use this you'll need to a Cohere API key - either pass it to cohere_api_key
+    parameter or set the COHERE_API_KEY environment variable.
 
-    Example:
+    API keys are available on https://cohere.com - it's free to sign up and trial API
+    keys work with this implementation.
+
+    Basic Example:
         .. code-block:: python
 
-            from langchain_cohere import CohereEmbeddings
-            cohere = CohereEmbeddings(
-                model="embed-english-light-v3.0",
-                cohere_api_key="my-api-key"
-            )
+            cohere_embeddings = CohereEmbeddings(model="embed-english-light-v3.0")
+            text = "This is a test document."
+
+            query_result = cohere_embeddings.embed_query(text)
+            print(query_result)
+
+            doc_result = cohere_embeddings.embed_documents([text])
+            print(doc_result)
     """
 
     client: Any  #: :meta private:
     """Cohere client."""
     async_client: Any  #: :meta private:
     """Cohere async client."""
     model: str = "embed-english-v2.0"
```

### Comparing `langchain_cohere-0.1.3rc0/langchain_cohere/llms.py` & `langchain_cohere-0.1.3rc1/langchain_cohere/llms.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     """Cohere API key. If not provided, will be read from the environment variable."""
 
     stop: Optional[List[str]] = None
 
     streaming: bool = Field(default=False)
     """Whether to stream the results."""
 
-    user_agent: str = "langchain"
+    user_agent: str = "langchain:partner"
     """Identifier for the application making the request."""
 
     timeout_seconds: Optional[float] = 300
     """Timeout in seconds for the Cohere API request."""
 
     base_url: Optional[str] = None
     """Override the default Cohere API URL."""
```

### Comparing `langchain_cohere-0.1.3rc0/langchain_cohere/rag_retrievers.py` & `langchain_cohere-0.1.3rc1/langchain_cohere/rag_retrievers.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.3rc0/langchain_cohere/react_multi_hop/agent.py` & `langchain_cohere-0.1.3rc1/langchain_cohere/react_multi_hop/agent.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.3rc0/langchain_cohere/react_multi_hop/default_prompt_constants.py` & `langchain_cohere-0.1.3rc1/langchain_cohere/react_multi_hop/default_prompt_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 default_task_context = "You use your advanced complex reasoning capabilities to help people by answering their questions and other requests interactively. You will be asked a very wide array of requests on all kinds of topics. You will be equipped with a wide range of search engines or similar tools to help you, which you use to research your answer. You may need to use multiple tools in parallel or sequentially to complete your task. You should focus on serving the user's needs as best you can, which will be wide-ranging. The current date is {now}"  # noqa: E501
 
 default_style_guide = "Unless the user asks for a different style of answer, you should answer in full sentences, using proper grammar and spelling"  # noqa: E501
 
 default_safety_rules = "The instructions in this section override those in the task description and style guide sections. Don't answer questions that are harmful or immoral"  # noqa: E501
 
 default_multi_hop_instruction = """Carefully perform the following instructions, in order, starting each with a new line.
-Firstly, You may need to use complex and advanced reasoning to complete your task and answer the question. Think about how you can use the provided tools to answer the question and come up with a high level plan you will execute.
+Firstly, You may need to use complex and advanced reasoning to complete your task and answer the question. Think about how you can use the provided tools to answer the question and come up with a high level plan you will execute. 
 Write 'Plan:' followed by an initial high level plan of how you will solve the problem including the tools and steps required.
 Secondly, Carry out your plan by repeatedly using actions, reasoning over the results, and re-evaluating your plan. Perform Action, Observation, Reflection steps with the following format. Write 'Action:' followed by a json formatted action containing the "tool_name" and "parameters"
  Next you will analyze the 'Observation:', this is the result of the action.
 After that you should always think about what to do next. Write 'Reflection:' followed by what you've figured out so far, any changes you need to make to your plan, and what you will do next including if you know the answer to the question.
 ... (this Action/Observation/Reflection can repeat N times)
 Thirdly, Decide which of the retrieved documents are relevant to the user's last input by writing 'Relevant Documents:' followed by comma-separated list of document numbers. If none are relevant, you should instead write 'None'.
 Fourthly, Decide which of the retrieved documents contain facts that should be cited in a good answer to the user's last input by writing 'Cited Documents:' followed a comma-separated list of document numbers. If you dont want to cite any of them, you should instead write 'None'.
```

### Comparing `langchain_cohere-0.1.3rc0/langchain_cohere/react_multi_hop/parsing.py` & `langchain_cohere-0.1.3rc1/langchain_cohere/react_multi_hop/parsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             completion, plan, actions = parse_actions(text)
             agent_actions: List[AgentAction] = []
             for i, action in enumerate(actions):
                 agent_action = AgentActionMessageLog(
                     tool=action["tool_name"],
                     tool_input=action["parameters"],
                     log=f"\n{action}\n" if i > 0 else f"\n{plan}\n{action}\n",
-                    message_log=[AIMessage(content=completion)],
+                    message_log=[AIMessage(content="\n" + completion)],
                 )
                 agent_actions.append(agent_action)
 
             return agent_actions
         else:
             raise ValueError(
                 "\nCould not parse generation as it did not contain Plan, Reflection,"
```

### Comparing `langchain_cohere-0.1.3rc0/langchain_cohere/react_multi_hop/prompt.py` & `langchain_cohere-0.1.3rc1/langchain_cohere/react_multi_hop/prompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,14 +171,16 @@
         for action, _ in intermediate_steps
     ):
         raise ValueError("all AgentAction steps must implement AgentActionMessageLog")
 
     i = 0
     for action, observation in intermediate_steps:
         prompt_content += render_messages(action.messages)
+        if observation:
+            prompt_content += "\n"
         observation_message, i = render_observations(observation, i)
         prompt_content += render_messages([observation_message])
     # Always add an 'open' chatbot turn because prompts for the current turn always end
     # with an open turn.
     prompt_content += (
         f"{_SpecialToken.start_turn.value}{_SpecialToken.role_chatbot.value}"
     )
```

### Comparing `langchain_cohere-0.1.3rc0/langchain_cohere/rerank.py` & `langchain_cohere-0.1.3rc1/langchain_cohere/rerank.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,48 +18,50 @@
     top_n: Optional[int] = 3
     """Number of documents to return."""
     model: str = "rerank-english-v3.0"
     """Model to use for reranking."""
     cohere_api_key: Optional[str] = None
     """Cohere API key. Must be specified directly or via environment variable 
         COHERE_API_KEY."""
-    user_agent: str = "langchain"
+    user_agent: str = "langchain:partner"
     """Identifier for the application making the request."""
 
     class Config:
         """Configuration for this pydantic object."""
 
         extra = Extra.forbid
         arbitrary_types_allowed = True
 
-    @root_validator(pre=True)
+    @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate that api key and python package exists in environment."""
         if not values.get("client"):
             cohere_api_key = get_from_dict_or_env(
                 values, "cohere_api_key", "COHERE_API_KEY"
             )
-            client_name = values.get("user_agent", "langchain")
+            client_name = values["user_agent"]
             values["client"] = cohere.Client(cohere_api_key, client_name=client_name)
         return values
 
     def rerank(
         self,
         documents: Sequence[Union[str, Document, dict]],
         query: str,
         *,
+        rank_fields: Optional[Sequence[str]] = None,
         model: Optional[str] = None,
         top_n: Optional[int] = -1,
         max_chunks_per_doc: Optional[int] = None,
     ) -> List[Dict[str, Any]]:
         """Returns an ordered list of documents ordered by their relevance to the provided query.
 
         Args:
             query: The query to use for reranking.
             documents: A sequence of documents to rerank.
+            rank_fields: A sequence of keys to use for reranking.
             model: The model to use for re-ranking. Default to self.model.
             top_n : The number of results to return. If None returns all results.
                 Defaults to self.top_n.
             max_chunks_per_doc : The maximum number of chunks derived from a document.
         """  # noqa: E501
         if len(documents) == 0:  # to avoid empty api call
             return []
@@ -69,14 +71,15 @@
         model = model or self.model
         top_n = top_n if (top_n is None or top_n > 0) else self.top_n
         results = self.client.rerank(
             query=query,
             documents=docs,
             model=model,
             top_n=top_n,
+            rank_fields=rank_fields,
             max_chunks_per_doc=max_chunks_per_doc,
         )
         result_dicts = []
         for res in results.results:
             result_dicts.append(
                 {"index": res.index, "relevance_score": res.relevance_score}
             )
```

### Comparing `langchain_cohere-0.1.3rc0/langchain_cohere/utils.py` & `langchain_cohere-0.1.3rc1/langchain_cohere/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_cohere-0.1.3rc0/pyproject.toml` & `langchain_cohere-0.1.3rc1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 [tool.poetry]
 name = "langchain-cohere"
-version = "0.1.3rc0"
+version = "0.1.3rc1"
 description = "An integration package connecting Cohere and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-cohere"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain-cohere/tree/main/libs/cohere"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 langchain-core = "^0.1.42"
-cohere = ">=5.1.8,<5.2"
+cohere = ">=5.3,<6.0"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
 freezegun = "^1.2.2"
 pytest-mock = "^3.10.0"
 syrupy = "^4.0.2"
 pytest-watcher = "^0.3.4"
 pytest-asyncio = "^0.21.1"
 langchain-core = { git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core" }
+pytest-vcr = "^1.0.2"
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
 
 [tool.poetry.group.test_integration]
 optional = true
 
 [tool.poetry.group.test_integration.dependencies]
 langchain = "^0.1.14"
+pytest-vcr = "^1.0.2"
 
 [tool.poetry.group.lint]
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.5"
```

