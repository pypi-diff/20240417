# Comparing `tmp/athena_intelligence-0.1.37.tar.gz` & `tmp/athena_intelligence-0.1.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athena_intelligence-0.1.37.tar", max compression
+gzip compressed data, was "athena_intelligence-0.1.38.tar", max compression
```

## Comparing `athena_intelligence-0.1.37.tar` & `athena_intelligence-0.1.38.tar`

### file list

```diff
@@ -1,48 +1,49 @@
--rw-r--r--   0        0        0     4235 2024-04-16 21:57:28.661732 athena_intelligence-0.1.37/README.md
--rw-r--r--   0        0        0      435 2024-04-16 21:57:28.661732 athena_intelligence-0.1.37/pyproject.toml
--rw-r--r--   0        0        0      959 2024-04-16 21:57:28.661732 athena_intelligence-0.1.37/src/athena/__init__.py
--rw-r--r--   0        0        0     5014 2024-04-16 21:57:28.661732 athena_intelligence-0.1.37/src/athena/base_client.py
--rw-r--r--   0        0        0     3576 2024-04-16 21:57:28.661732 athena_intelligence-0.1.37/src/athena/client.py
--rw-r--r--   0        0        0      790 2024-04-16 21:57:28.661732 athena_intelligence-0.1.37/src/athena/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-16 21:57:28.661732 athena_intelligence-0.1.37/src/athena/core/api_error.py
--rw-r--r--   0        0        0     1198 2024-04-16 21:57:28.661732 athena_intelligence-0.1.37/src/athena/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-16 21:57:28.661732 athena_intelligence-0.1.37/src/athena/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-16 21:57:28.661732 athena_intelligence-0.1.37/src/athena/core/file.py
--rw-r--r--   0        0        0     4882 2024-04-16 21:57:28.661732 athena_intelligence-0.1.37/src/athena/core/http_client.py
--rw-r--r--   0        0        0     3799 2024-04-16 21:57:28.661732 athena_intelligence-0.1.37/src/athena/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-04-16 21:57:28.661732 athena_intelligence-0.1.37/src/athena/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-16 21:57:28.661732 athena_intelligence-0.1.37/src/athena/core/request_options.py
--rw-r--r--   0        0        0       65 2024-04-16 21:57:28.661732 athena_intelligence-0.1.37/src/athena/dataset/__init__.py
--rw-r--r--   0        0        0     6087 2024-04-16 21:57:28.661732 athena_intelligence-0.1.37/src/athena/dataset/client.py
--rw-r--r--   0        0        0      165 2024-04-16 21:57:28.661732 athena_intelligence-0.1.37/src/athena/environment.py
--rw-r--r--   0        0        0      170 2024-04-16 21:57:28.661732 athena_intelligence-0.1.37/src/athena/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-04-16 21:57:28.661732 athena_intelligence-0.1.37/src/athena/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0       65 2024-04-16 21:57:28.661732 athena_intelligence-0.1.37/src/athena/message/__init__.py
--rw-r--r--   0        0        0    12185 2024-04-16 21:57:28.661732 athena_intelligence-0.1.37/src/athena/message/client.py
--rw-r--r--   0        0        0     3998 2024-04-16 21:57:28.661732 athena_intelligence-0.1.37/src/athena/polling_message_client.py
--rw-r--r--   0        0        0        0 2024-04-16 21:57:28.661732 athena_intelligence-0.1.37/src/athena/py.typed
--rw-r--r--   0        0        0       65 2024-04-16 21:57:28.661732 athena_intelligence-0.1.37/src/athena/query/__init__.py
--rw-r--r--   0        0        0     6243 2024-04-16 21:57:28.661732 athena_intelligence-0.1.37/src/athena/query/client.py
--rw-r--r--   0        0        0       65 2024-04-16 21:57:28.661732 athena_intelligence-0.1.37/src/athena/report/__init__.py
--rw-r--r--   0        0        0     6528 2024-04-16 21:57:28.661732 athena_intelligence-0.1.37/src/athena/report/client.py
--rw-r--r--   0        0        0       65 2024-04-16 21:57:28.661732 athena_intelligence-0.1.37/src/athena/search/__init__.py
--rw-r--r--   0        0        0    12255 2024-04-16 21:57:28.661732 athena_intelligence-0.1.37/src/athena/search/client.py
--rw-r--r--   0        0        0       65 2024-04-16 21:57:28.661732 athena_intelligence-0.1.37/src/athena/snippet/__init__.py
--rw-r--r--   0        0        0     6087 2024-04-16 21:57:28.661732 athena_intelligence-0.1.37/src/athena/snippet/client.py
--rw-r--r--   0        0        0      969 2024-04-16 21:57:28.665732 athena_intelligence-0.1.37/src/athena/types/__init__.py
--rw-r--r--   0        0        0     1014 2024-04-16 21:57:28.665732 athena_intelligence-0.1.37/src/athena/types/dataset.py
--rw-r--r--   0        0        0      989 2024-04-16 21:57:28.665732 athena_intelligence-0.1.37/src/athena/types/get_datasets_response.py
--rw-r--r--   0        0        0      989 2024-04-16 21:57:28.665732 athena_intelligence-0.1.37/src/athena/types/get_snippets_response.py
--rw-r--r--   0        0        0      973 2024-04-16 21:57:28.665732 athena_intelligence-0.1.37/src/athena/types/http_validation_error.py
--rw-r--r--   0        0        0      865 2024-04-16 21:57:28.665732 athena_intelligence-0.1.37/src/athena/types/message_out.py
--rw-r--r--   0        0        0     1051 2024-04-16 21:57:28.665732 athena_intelligence-0.1.37/src/athena/types/message_out_dto.py
--rw-r--r--   0        0        0     2545 2024-04-16 21:57:28.665732 athena_intelligence-0.1.37/src/athena/types/model.py
--rw-r--r--   0        0        0      946 2024-04-16 21:57:28.665732 athena_intelligence-0.1.37/src/athena/types/report.py
--rw-r--r--   0        0        0     1126 2024-04-16 21:57:28.665732 athena_intelligence-0.1.37/src/athena/types/snippet.py
--rw-r--r--   0        0        0      900 2024-04-16 21:57:28.665732 athena_intelligence-0.1.37/src/athena/types/sql_results.py
--rw-r--r--   0        0        0      672 2024-04-16 21:57:28.665732 athena_intelligence-0.1.37/src/athena/types/status_enum.py
--rw-r--r--   0        0        0     1422 2024-04-16 21:57:28.665732 athena_intelligence-0.1.37/src/athena/types/tools.py
--rw-r--r--   0        0        0      893 2024-04-16 21:57:28.665732 athena_intelligence-0.1.37/src/athena/types/url_result.py
--rw-r--r--   0        0        0      992 2024-04-16 21:57:28.665732 athena_intelligence-0.1.37/src/athena/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-16 21:57:28.665732 athena_intelligence-0.1.37/src/athena/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 athena_intelligence-0.1.37/PKG-INFO
+-rw-r--r--   0        0        0     4235 2024-04-16 22:21:28.959996 athena_intelligence-0.1.38/README.md
+-rw-r--r--   0        0        0      435 2024-04-16 22:21:28.959996 athena_intelligence-0.1.38/pyproject.toml
+-rw-r--r--   0        0        0     1013 2024-04-16 22:21:28.959996 athena_intelligence-0.1.38/src/athena/__init__.py
+-rw-r--r--   0        0        0     5014 2024-04-16 22:21:28.959996 athena_intelligence-0.1.38/src/athena/base_client.py
+-rw-r--r--   0        0        0     3576 2024-04-16 22:21:28.959996 athena_intelligence-0.1.38/src/athena/client.py
+-rw-r--r--   0        0        0      790 2024-04-16 22:21:28.959996 athena_intelligence-0.1.38/src/athena/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-16 22:21:28.959996 athena_intelligence-0.1.38/src/athena/core/api_error.py
+-rw-r--r--   0        0        0     1198 2024-04-16 22:21:28.959996 athena_intelligence-0.1.38/src/athena/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-16 22:21:28.959996 athena_intelligence-0.1.38/src/athena/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-16 22:21:28.959996 athena_intelligence-0.1.38/src/athena/core/file.py
+-rw-r--r--   0        0        0     4882 2024-04-16 22:21:28.959996 athena_intelligence-0.1.38/src/athena/core/http_client.py
+-rw-r--r--   0        0        0     3799 2024-04-16 22:21:28.959996 athena_intelligence-0.1.38/src/athena/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-16 22:21:28.959996 athena_intelligence-0.1.38/src/athena/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-16 22:21:28.959996 athena_intelligence-0.1.38/src/athena/core/request_options.py
+-rw-r--r--   0        0        0       65 2024-04-16 22:21:28.959996 athena_intelligence-0.1.38/src/athena/dataset/__init__.py
+-rw-r--r--   0        0        0     6087 2024-04-16 22:21:28.959996 athena_intelligence-0.1.38/src/athena/dataset/client.py
+-rw-r--r--   0        0        0      165 2024-04-16 22:21:28.959996 athena_intelligence-0.1.38/src/athena/environment.py
+-rw-r--r--   0        0        0      170 2024-04-16 22:21:28.959996 athena_intelligence-0.1.38/src/athena/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-04-16 22:21:28.959996 athena_intelligence-0.1.38/src/athena/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0       65 2024-04-16 22:21:28.959996 athena_intelligence-0.1.38/src/athena/message/__init__.py
+-rw-r--r--   0        0        0    12185 2024-04-16 22:21:28.959996 athena_intelligence-0.1.38/src/athena/message/client.py
+-rw-r--r--   0        0        0     3998 2024-04-16 22:21:28.963996 athena_intelligence-0.1.38/src/athena/polling_message_client.py
+-rw-r--r--   0        0        0        0 2024-04-16 22:21:28.963996 athena_intelligence-0.1.38/src/athena/py.typed
+-rw-r--r--   0        0        0       65 2024-04-16 22:21:28.963996 athena_intelligence-0.1.38/src/athena/query/__init__.py
+-rw-r--r--   0        0        0     6243 2024-04-16 22:21:28.963996 athena_intelligence-0.1.38/src/athena/query/client.py
+-rw-r--r--   0        0        0       65 2024-04-16 22:21:28.963996 athena_intelligence-0.1.38/src/athena/report/__init__.py
+-rw-r--r--   0        0        0     6528 2024-04-16 22:21:28.963996 athena_intelligence-0.1.38/src/athena/report/client.py
+-rw-r--r--   0        0        0       65 2024-04-16 22:21:28.963996 athena_intelligence-0.1.38/src/athena/search/__init__.py
+-rw-r--r--   0        0        0    12391 2024-04-16 22:21:28.963996 athena_intelligence-0.1.38/src/athena/search/client.py
+-rw-r--r--   0        0        0       65 2024-04-16 22:21:28.963996 athena_intelligence-0.1.38/src/athena/snippet/__init__.py
+-rw-r--r--   0        0        0     6087 2024-04-16 22:21:28.963996 athena_intelligence-0.1.38/src/athena/snippet/client.py
+-rw-r--r--   0        0        0     1054 2024-04-16 22:21:28.963996 athena_intelligence-0.1.38/src/athena/types/__init__.py
+-rw-r--r--   0        0        0     1014 2024-04-16 22:21:28.963996 athena_intelligence-0.1.38/src/athena/types/dataset.py
+-rw-r--r--   0        0        0      989 2024-04-16 22:21:28.963996 athena_intelligence-0.1.38/src/athena/types/get_datasets_response.py
+-rw-r--r--   0        0        0      989 2024-04-16 22:21:28.963996 athena_intelligence-0.1.38/src/athena/types/get_snippets_response.py
+-rw-r--r--   0        0        0      973 2024-04-16 22:21:28.963996 athena_intelligence-0.1.38/src/athena/types/http_validation_error.py
+-rw-r--r--   0        0        0      865 2024-04-16 22:21:28.963996 athena_intelligence-0.1.38/src/athena/types/message_out.py
+-rw-r--r--   0        0        0     1051 2024-04-16 22:21:28.963996 athena_intelligence-0.1.38/src/athena/types/message_out_dto.py
+-rw-r--r--   0        0        0     2545 2024-04-16 22:21:28.963996 athena_intelligence-0.1.38/src/athena/types/model.py
+-rw-r--r--   0        0        0      946 2024-04-16 22:21:28.963996 athena_intelligence-0.1.38/src/athena/types/report.py
+-rw-r--r--   0        0        0      881 2024-04-16 22:21:28.963996 athena_intelligence-0.1.38/src/athena/types/scrape_markdown_result.py
+-rw-r--r--   0        0        0     1126 2024-04-16 22:21:28.963996 athena_intelligence-0.1.38/src/athena/types/snippet.py
+-rw-r--r--   0        0        0      900 2024-04-16 22:21:28.963996 athena_intelligence-0.1.38/src/athena/types/sql_results.py
+-rw-r--r--   0        0        0      672 2024-04-16 22:21:28.963996 athena_intelligence-0.1.38/src/athena/types/status_enum.py
+-rw-r--r--   0        0        0     1422 2024-04-16 22:21:28.963996 athena_intelligence-0.1.38/src/athena/types/tools.py
+-rw-r--r--   0        0        0      893 2024-04-16 22:21:28.963996 athena_intelligence-0.1.38/src/athena/types/url_result.py
+-rw-r--r--   0        0        0      992 2024-04-16 22:21:28.963996 athena_intelligence-0.1.38/src/athena/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-16 22:21:28.963996 athena_intelligence-0.1.38/src/athena/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 athena_intelligence-0.1.38/PKG-INFO
```

### Comparing `athena_intelligence-0.1.37/README.md` & `athena_intelligence-0.1.38/README.md`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.37/src/athena/__init__.py` & `athena_intelligence-0.1.38/src/athena/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     GetDatasetsResponse,
     GetSnippetsResponse,
     HttpValidationError,
     MessageOut,
     MessageOutDto,
     Model,
     Report,
+    ScrapeMarkdownResult,
     Snippet,
     SqlResults,
     StatusEnum,
     Tools,
     UrlResult,
     ValidationError,
     ValidationErrorLocItem,
@@ -27,14 +28,15 @@
     "GetDatasetsResponse",
     "GetSnippetsResponse",
     "HttpValidationError",
     "MessageOut",
     "MessageOutDto",
     "Model",
     "Report",
+    "ScrapeMarkdownResult",
     "Snippet",
     "SqlResults",
     "StatusEnum",
     "Tools",
     "UnprocessableEntityError",
     "UrlResult",
     "ValidationError",
```

### Comparing `athena_intelligence-0.1.37/src/athena/base_client.py` & `athena_intelligence-0.1.38/src/athena/base_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.37/src/athena/client.py` & `athena_intelligence-0.1.38/src/athena/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.37/src/athena/core/__init__.py` & `athena_intelligence-0.1.38/src/athena/core/__init__.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.37/src/athena/core/client_wrapper.py` & `athena_intelligence-0.1.38/src/athena/core/client_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         self.api_key = api_key
         self._base_url = base_url
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "athena-intelligence",
-            "X-Fern-SDK-Version": "0.1.37",
+            "X-Fern-SDK-Version": "0.1.38",
         }
         headers["X-API-KEY"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `athena_intelligence-0.1.37/src/athena/core/datetime_utils.py` & `athena_intelligence-0.1.38/src/athena/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.37/src/athena/core/file.py` & `athena_intelligence-0.1.38/src/athena/core/file.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.37/src/athena/core/http_client.py` & `athena_intelligence-0.1.38/src/athena/core/http_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.37/src/athena/core/jsonable_encoder.py` & `athena_intelligence-0.1.38/src/athena/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.37/src/athena/core/request_options.py` & `athena_intelligence-0.1.38/src/athena/core/request_options.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.37/src/athena/dataset/client.py` & `athena_intelligence-0.1.38/src/athena/dataset/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.37/src/athena/message/client.py` & `athena_intelligence-0.1.38/src/athena/message/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.37/src/athena/polling_message_client.py` & `athena_intelligence-0.1.38/src/athena/polling_message_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.37/src/athena/query/client.py` & `athena_intelligence-0.1.38/src/athena/query/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.37/src/athena/report/client.py` & `athena_intelligence-0.1.38/src/athena/report/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.37/src/athena/search/client.py` & `athena_intelligence-0.1.38/src/athena/search/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..errors.unprocessable_entity_error import UnprocessableEntityError
 from ..types.http_validation_error import HttpValidationError
+from ..types.scrape_markdown_result import ScrapeMarkdownResult
 from ..types.url_result import UrlResult
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
@@ -103,15 +104,17 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_markdown(self, *, url: str, request_options: typing.Optional[RequestOptions] = None) -> UrlResult:
+    def get_markdown(
+        self, *, url: str, request_options: typing.Optional[RequestOptions] = None
+    ) -> ScrapeMarkdownResult:
         """
         Parameters:
             - url: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from athena.client import Athena
@@ -146,15 +149,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else 60,
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(UrlResult, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ScrapeMarkdownResult, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
@@ -241,15 +244,17 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_markdown(self, *, url: str, request_options: typing.Optional[RequestOptions] = None) -> UrlResult:
+    async def get_markdown(
+        self, *, url: str, request_options: typing.Optional[RequestOptions] = None
+    ) -> ScrapeMarkdownResult:
         """
         Parameters:
             - url: str.
 
             - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
         ---
         from athena.client import AsyncAthena
@@ -284,15 +289,15 @@
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
             else 60,
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(UrlResult, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(ScrapeMarkdownResult, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `athena_intelligence-0.1.37/src/athena/snippet/client.py` & `athena_intelligence-0.1.38/src/athena/snippet/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.37/src/athena/types/__init__.py` & `athena_intelligence-0.1.38/src/athena/types/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .get_datasets_response import GetDatasetsResponse
 from .get_snippets_response import GetSnippetsResponse
 from .http_validation_error import HttpValidationError
 from .message_out import MessageOut
 from .message_out_dto import MessageOutDto
 from .model import Model
 from .report import Report
+from .scrape_markdown_result import ScrapeMarkdownResult
 from .snippet import Snippet
 from .sql_results import SqlResults
 from .status_enum import StatusEnum
 from .tools import Tools
 from .url_result import UrlResult
 from .validation_error import ValidationError
 from .validation_error_loc_item import ValidationErrorLocItem
@@ -21,14 +22,15 @@
     "GetDatasetsResponse",
     "GetSnippetsResponse",
     "HttpValidationError",
     "MessageOut",
     "MessageOutDto",
     "Model",
     "Report",
+    "ScrapeMarkdownResult",
     "Snippet",
     "SqlResults",
     "StatusEnum",
     "Tools",
     "UrlResult",
     "ValidationError",
     "ValidationErrorLocItem",
```

### Comparing `athena_intelligence-0.1.37/src/athena/types/dataset.py` & `athena_intelligence-0.1.38/src/athena/types/dataset.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.37/src/athena/types/get_datasets_response.py` & `athena_intelligence-0.1.38/src/athena/types/get_datasets_response.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.37/src/athena/types/get_snippets_response.py` & `athena_intelligence-0.1.38/src/athena/types/get_snippets_response.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.37/src/athena/types/http_validation_error.py` & `athena_intelligence-0.1.38/src/athena/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.37/src/athena/types/message_out.py` & `athena_intelligence-0.1.38/src/athena/types/message_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.37/src/athena/types/message_out_dto.py` & `athena_intelligence-0.1.38/src/athena/types/message_out_dto.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.37/src/athena/types/model.py` & `athena_intelligence-0.1.38/src/athena/types/model.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.37/src/athena/types/report.py` & `athena_intelligence-0.1.38/src/athena/types/report.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.37/src/athena/types/snippet.py` & `athena_intelligence-0.1.38/src/athena/types/snippet.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.37/src/athena/types/sql_results.py` & `athena_intelligence-0.1.38/src/athena/types/sql_results.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.37/src/athena/types/status_enum.py` & `athena_intelligence-0.1.38/src/athena/types/status_enum.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.37/src/athena/types/tools.py` & `athena_intelligence-0.1.38/src/athena/types/tools.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.37/src/athena/types/url_result.py` & `athena_intelligence-0.1.38/src/athena/types/url_result.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.37/src/athena/types/validation_error.py` & `athena_intelligence-0.1.38/src/athena/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.37/PKG-INFO` & `athena_intelligence-0.1.38/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athena-intelligence
-Version: 0.1.37
+Version: 0.1.38
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

