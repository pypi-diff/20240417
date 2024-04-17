# Comparing `tmp/bigdata_client-0.0.6.tar.gz` & `tmp/bigdata_client-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigdata_client-0.0.6.tar", max compression
+gzip compressed data, was "bigdata_client-0.0.7.tar", max compression
```

## Comparing `bigdata_client-0.0.6.tar` & `bigdata_client-0.0.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0      358 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/README.md
--rw-r--r--   0        0        0      155 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/__init__.py
--rw-r--r--   0        0        0     6526 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/advanced_search_query.py
--rw-r--r--   0        0        0        0 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/api/__init__.py
--rw-r--r--   0        0        0     1045 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/api/autosuggest.py
--rw-r--r--   0        0        0     8160 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/api/search.py
--rw-r--r--   0        0        0     6324 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/auth.py
--rw-r--r--   0        0        0        0 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/clerk/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/clerk/authenticators/__init__.py
--rw-r--r--   0        0        0     2256 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/clerk/authenticators/base_instance.py
--rw-r--r--   0        0        0     4166 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/clerk/authenticators/dev_instance.py
--rw-r--r--   0        0        0     3650 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/clerk/authenticators/production_instance.py
--rw-r--r--   0        0        0      853 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/clerk/exceptions.py
--rw-r--r--   0        0        0      245 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/clerk/models.py
--rw-r--r--   0        0        0        0 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/clerk/sign_in_strategies/__init__.py
--rw-r--r--   0        0        0      243 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/clerk/sign_in_strategies/base.py
--rw-r--r--   0        0        0     1008 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/clerk/sign_in_strategies/password.py
--rw-r--r--   0        0        0     2510 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/clerk/token_manager.py
--rw-r--r--   0        0        0     2040 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/clerk/token_manager_factory.py
--rw-r--r--   0        0        0     6778 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/connection.py
--rw-r--r--   0        0        0      154 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/constants.py
--rw-r--r--   0        0        0     3626 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/daterange.py
--rw-r--r--   0        0        0     1234 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/entity_types.py
--rw-r--r--   0        0        0      664 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/enum_utils.py
--rw-r--r--   0        0        0       82 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/errors.py
--rw-r--r--   0        0        0      513 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/jwt.py
--rw-r--r--   0        0        0        0 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/models/__init__.py
--rw-r--r--   0        0        0    21160 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/models/advanced_search_query.py
--rw-r--r--   0        0        0     1181 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/models/comentions.py
--rw-r--r--   0        0        0     5988 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/models/entities.py
--rw-r--r--   0        0        0     1094 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/models/languages.py
--rw-r--r--   0        0        0     3443 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/models/parse.py
--rw-r--r--   0        0        0     1710 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/models/search.py
--rw-r--r--   0        0        0     2280 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/models/sources.py
--rw-r--r--   0        0        0      855 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/models/story.py
--rw-r--r--   0        0        0     2180 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/models/topics.py
--rw-r--r--   0        0        0     1390 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/models/uploads.py
--rw-r--r--   0        0        0     1084 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/models/watchlists.py
--rw-r--r--   0        0        0     4633 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/old_auth.py
--rw-r--r--   0        0        0      970 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/query.py
--rw-r--r--   0        0        0      251 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/query_type.py
--rw-r--r--   0        0        0     7873 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/search.py
--rw-r--r--   0        0        0     9021 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/services.py
--rw-r--r--   0        0        0     1020 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/settings.py
--rw-r--r--   0        0        0    12157 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/simple_search_query.py
--rw-r--r--   0        0        0     2022 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/story.py
--rw-r--r--   0        0        0      465 2024-04-12 07:39:36.074213 bigdata_client-0.0.6/bigdata/user_agent.py
--rw-r--r--   0        0        0     1453 2024-04-12 07:39:36.078214 bigdata_client-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1056 1970-01-01 00:00:00.000000 bigdata_client-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      358 2024-04-17 14:53:51.264716 bigdata_client-0.0.7/README.md
+-rw-r--r--   0        0        0      155 2024-04-17 14:53:51.264716 bigdata_client-0.0.7/bigdata/__init__.py
+-rw-r--r--   0        0        0     6526 2024-04-17 14:53:51.264716 bigdata_client-0.0.7/bigdata/advanced_search_query.py
+-rw-r--r--   0        0        0        0 2024-04-17 14:53:51.264716 bigdata_client-0.0.7/bigdata/api/__init__.py
+-rw-r--r--   0        0        0     1045 2024-04-17 14:53:51.264716 bigdata_client-0.0.7/bigdata/api/autosuggest.py
+-rw-r--r--   0        0        0     8160 2024-04-17 14:53:51.264716 bigdata_client-0.0.7/bigdata/api/search.py
+-rw-r--r--   0        0        0     6324 2024-04-17 14:53:51.264716 bigdata_client-0.0.7/bigdata/auth.py
+-rw-r--r--   0        0        0        0 2024-04-17 14:53:51.264716 bigdata_client-0.0.7/bigdata/clerk/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 14:53:51.264716 bigdata_client-0.0.7/bigdata/clerk/authenticators/__init__.py
+-rw-r--r--   0        0        0     2256 2024-04-17 14:53:51.264716 bigdata_client-0.0.7/bigdata/clerk/authenticators/base_instance.py
+-rw-r--r--   0        0        0     4166 2024-04-17 14:53:51.264716 bigdata_client-0.0.7/bigdata/clerk/authenticators/dev_instance.py
+-rw-r--r--   0        0        0     3650 2024-04-17 14:53:51.264716 bigdata_client-0.0.7/bigdata/clerk/authenticators/production_instance.py
+-rw-r--r--   0        0        0      853 2024-04-17 14:53:51.264716 bigdata_client-0.0.7/bigdata/clerk/exceptions.py
+-rw-r--r--   0        0        0      245 2024-04-17 14:53:51.264716 bigdata_client-0.0.7/bigdata/clerk/models.py
+-rw-r--r--   0        0        0        0 2024-04-17 14:53:51.264716 bigdata_client-0.0.7/bigdata/clerk/sign_in_strategies/__init__.py
+-rw-r--r--   0        0        0      243 2024-04-17 14:53:51.264716 bigdata_client-0.0.7/bigdata/clerk/sign_in_strategies/base.py
+-rw-r--r--   0        0        0     1008 2024-04-17 14:53:51.264716 bigdata_client-0.0.7/bigdata/clerk/sign_in_strategies/password.py
+-rw-r--r--   0        0        0     2510 2024-04-17 14:53:51.264716 bigdata_client-0.0.7/bigdata/clerk/token_manager.py
+-rw-r--r--   0        0        0     2040 2024-04-17 14:53:51.268716 bigdata_client-0.0.7/bigdata/clerk/token_manager_factory.py
+-rw-r--r--   0        0        0     6854 2024-04-17 14:53:51.268716 bigdata_client-0.0.7/bigdata/connection.py
+-rw-r--r--   0        0        0      154 2024-04-17 14:53:51.268716 bigdata_client-0.0.7/bigdata/constants.py
+-rw-r--r--   0        0        0     3626 2024-04-17 14:53:51.268716 bigdata_client-0.0.7/bigdata/daterange.py
+-rw-r--r--   0        0        0     1234 2024-04-17 14:53:51.268716 bigdata_client-0.0.7/bigdata/entity_types.py
+-rw-r--r--   0        0        0      664 2024-04-17 14:53:51.268716 bigdata_client-0.0.7/bigdata/enum_utils.py
+-rw-r--r--   0        0        0       82 2024-04-17 14:53:51.268716 bigdata_client-0.0.7/bigdata/errors.py
+-rw-r--r--   0        0        0      513 2024-04-17 14:53:51.268716 bigdata_client-0.0.7/bigdata/jwt.py
+-rw-r--r--   0        0        0        0 2024-04-17 14:53:51.268716 bigdata_client-0.0.7/bigdata/models/__init__.py
+-rw-r--r--   0        0        0    21160 2024-04-17 14:53:51.268716 bigdata_client-0.0.7/bigdata/models/advanced_search_query.py
+-rw-r--r--   0        0        0     1181 2024-04-17 14:53:51.268716 bigdata_client-0.0.7/bigdata/models/comentions.py
+-rw-r--r--   0        0        0     6012 2024-04-17 14:53:51.268716 bigdata_client-0.0.7/bigdata/models/entities.py
+-rw-r--r--   0        0        0     1094 2024-04-17 14:53:51.268716 bigdata_client-0.0.7/bigdata/models/languages.py
+-rw-r--r--   0        0        0     3443 2024-04-17 14:53:51.268716 bigdata_client-0.0.7/bigdata/models/parse.py
+-rw-r--r--   0        0        0     1710 2024-04-17 14:53:51.268716 bigdata_client-0.0.7/bigdata/models/search.py
+-rw-r--r--   0        0        0     2280 2024-04-17 14:53:51.268716 bigdata_client-0.0.7/bigdata/models/sources.py
+-rw-r--r--   0        0        0      855 2024-04-17 14:53:51.268716 bigdata_client-0.0.7/bigdata/models/story.py
+-rw-r--r--   0        0        0     2180 2024-04-17 14:53:51.268716 bigdata_client-0.0.7/bigdata/models/topics.py
+-rw-r--r--   0        0        0     1390 2024-04-17 14:53:51.268716 bigdata_client-0.0.7/bigdata/models/uploads.py
+-rw-r--r--   0        0        0     1084 2024-04-17 14:53:51.268716 bigdata_client-0.0.7/bigdata/models/watchlists.py
+-rw-r--r--   0        0        0     4633 2024-04-17 14:53:51.268716 bigdata_client-0.0.7/bigdata/old_auth.py
+-rw-r--r--   0        0        0      970 2024-04-17 14:53:51.268716 bigdata_client-0.0.7/bigdata/query.py
+-rw-r--r--   0        0        0      251 2024-04-17 14:53:51.268716 bigdata_client-0.0.7/bigdata/query_type.py
+-rw-r--r--   0        0        0     7873 2024-04-17 14:53:51.268716 bigdata_client-0.0.7/bigdata/search.py
+-rw-r--r--   0        0        0     9021 2024-04-17 14:53:51.268716 bigdata_client-0.0.7/bigdata/services.py
+-rw-r--r--   0        0        0     1020 2024-04-17 14:53:51.268716 bigdata_client-0.0.7/bigdata/settings.py
+-rw-r--r--   0        0        0    12157 2024-04-17 14:53:51.268716 bigdata_client-0.0.7/bigdata/simple_search_query.py
+-rw-r--r--   0        0        0     2022 2024-04-17 14:53:51.268716 bigdata_client-0.0.7/bigdata/story.py
+-rw-r--r--   0        0        0      465 2024-04-17 14:53:51.268716 bigdata_client-0.0.7/bigdata/user_agent.py
+-rw-r--r--   0        0        0     1359 2024-04-17 14:53:51.268716 bigdata_client-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1058 1970-01-01 00:00:00.000000 bigdata_client-0.0.7/PKG-INFO
```

### Comparing `bigdata_client-0.0.6/bigdata/advanced_search_query.py` & `bigdata_client-0.0.7/bigdata/advanced_search_query.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/bigdata/api/autosuggest.py` & `bigdata_client-0.0.7/bigdata/api/autosuggest.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/bigdata/api/search.py` & `bigdata_client-0.0.7/bigdata/api/search.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/bigdata/auth.py` & `bigdata_client-0.0.7/bigdata/auth.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/bigdata/clerk/authenticators/base_instance.py` & `bigdata_client-0.0.7/bigdata/clerk/authenticators/base_instance.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/bigdata/clerk/authenticators/dev_instance.py` & `bigdata_client-0.0.7/bigdata/clerk/authenticators/dev_instance.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/bigdata/clerk/authenticators/production_instance.py` & `bigdata_client-0.0.7/bigdata/clerk/authenticators/production_instance.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/bigdata/clerk/exceptions.py` & `bigdata_client-0.0.7/bigdata/clerk/exceptions.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/bigdata/clerk/sign_in_strategies/password.py` & `bigdata_client-0.0.7/bigdata/clerk/sign_in_strategies/password.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/bigdata/clerk/token_manager.py` & `bigdata_client-0.0.7/bigdata/clerk/token_manager.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/bigdata/clerk/token_manager_factory.py` & `bigdata_client-0.0.7/bigdata/clerk/token_manager_factory.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/bigdata/connection.py` & `bigdata_client-0.0.7/bigdata/connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,22 +12,19 @@
 )
 from bigdata.api.search import (
     DiscoveryPanelRequest,
     DiscoveryPanelResponse,
     ListSavedSearchesResponse,
     QueryChunksRequest,
     QueryChunksResponse,
-    QueryClustersRequest,
-    QueryClustersResponse,
     SavedSearchResponse,
     SaveSearchRequest,
     UpdateSearchRequest,
 )
 from bigdata.auth import AsyncRequestContext, AsyncResponseContext, Auth
-from bigdata.models.parse import KnowledgeGraphAnnotated, KnowledgeGraphTypes
 
 CONCURRENT_AUTOSUGGEST_REQUESTS_LIMIT = 10
 
 
 class AsyncRequestPartialContext(BaseModel):
     """
     Context used to pass information to connection module for making async requests.
@@ -51,16 +48,15 @@
 
     Contains the Auth object with the JWT and abstracts all the calls to the API,
     receiving and returning objects to/from the caller.
     For internal use only.
     """
 
     def __init__(self, auth: Auth, api_url: str):
-        self.auth = auth
-        self.api_url = api_url
+        self.http = HTTPWrapper(auth, api_url)
 
     # Autosuggest
 
     def autosuggest(
         self, items: AutosuggestRequests, limit: int
     ) -> AutosuggestResponse:
         """Calls GET /autosuggest"""
@@ -75,15 +71,15 @@
             for item in items.root
         ]
 
         responses = []
         for batch in self._get_batches(
             all_requests_input, CONCURRENT_AUTOSUGGEST_REQUESTS_LIMIT
         ):
-            responses.extend(self._async_get(batch))
+            responses.extend(self.http.async_get(batch))
 
         return AutosuggestResponse(
             root={
                 item.id: AutosuggestResponseItem(root=item.response["results"])
                 for item in responses
             }
         )
@@ -91,28 +87,28 @@
     @staticmethod
     def _get_batches(items: list[T], batch_size: int) -> Generator[list[T], None, None]:
         for idx in range(0, len(items), batch_size):
             yield items[idx : idx + batch_size]
 
     def by_ids(self, request: ByIdsRequest) -> ByIdsResponse:
         json_request = request.model_dump(exclude_none=True, by_alias=True)
-        json_response = self._post("cqs/by-ids", json=json_request)
+        json_response = self.http.post("cqs/by-ids", json=json_request)
         return ByIdsResponse(root=json_response)
 
     # Search
 
     def query_chunks(self, request: QueryChunksRequest) -> QueryChunksResponse:
         """Calls POST /cqs/query-chunks"""
         json_request = request.model_dump(exclude_none=True, by_alias=True)
-        json_response = self._post("cqs/query-chunks", json=json_request)
+        json_response = self.http.post("cqs/query-chunks", json=json_request)
         return QueryChunksResponse(**json_response)
 
     def get_search(self, id: str) -> SavedSearchResponse:
         """Calls GET /user-data/queries/{id}"""
-        json_response = self._get(f"user-data/queries/{id}")
+        json_response = self.http.get(f"user-data/queries/{id}")
         try:
             return SavedSearchResponse(**json_response)
         except ValidationError as e:
             raise NotImplementedError(
                 "Query expression may have unsupported expression types"
             ) from e
 
@@ -121,68 +117,76 @@
     ) -> ListSavedSearchesResponse:
         """Calls GET /user-data/queries"""
         params = {}
         if saved:
             params["save_status"] = "saved"
         if owned:
             params["owned"] = "true"
-        json_response = self._get("user-data/queries", params=params)
+        json_response = self.http.get("user-data/queries", params=params)
         return ListSavedSearchesResponse(**json_response)
 
     def save_search(self, request: SaveSearchRequest) -> dict:
         """Calls POST /user-data/queries"""
         json_request = request.model_dump(exclude_none=True, by_alias=True)
-        return self._post("user-data/queries", json=json_request)
+        return self.http.post("user-data/queries", json=json_request)
 
     def update_search(self, request: UpdateSearchRequest, search_id: str) -> dict:
         """Calls PATCH /user-data/queries/{id}"""
         json_request = request.model_dump(exclude_none=True, by_alias=True)
-        return self._patch(f"user-data/queries/{search_id}", json=json_request)
+        return self.http.patch(f"user-data/queries/{search_id}", json=json_request)
 
     def delete_search(self, id: str) -> dict:
         """Calls DELETE /user-data/queries/{id}"""
-        return self._delete(f"user-data/queries/{id}")
+        return self.http.delete(f"user-data/queries/{id}")
 
     def query_discovery_panel(
         self, request: DiscoveryPanelRequest
     ) -> DiscoveryPanelResponse:
         """Calls POST /cqs/discovery-panel"""
         json_request = request.model_dump(exclude_none=True, by_alias=True)
-        json_response = self._post("cqs/discovery-panel", json=json_request)
+        json_response = self.http.post("cqs/discovery-panel", json=json_request)
         return DiscoveryPanelResponse(**json_response)
 
-    # Wrappers for HTTP methods
 
-    def _get(self, endpoint: str, params: dict = None) -> dict:
+class HTTPWrapper:
+    """
+    A basic connection to perform HTTP GET, POST, PATCH, DELETE requests.
+    """
+
+    def __init__(self, auth: Auth, api_url: str):
+        self.auth = auth
+        self.api_url = api_url
+
+    def get(self, endpoint: str, params: dict = None) -> dict:
         params = params or {}
         url = self._get_url(endpoint)
         response = self.auth.request("GET", url, params=params)
         response.raise_for_status()
         return response.json()
 
-    def _post(self, endpoint: str, json: json_types) -> json_types:
+    def post(self, endpoint: str, json: json_types) -> json_types:
         url = self._get_url(endpoint)
         response = self.auth.request("POST", url, json=json)
         response.raise_for_status()
         return response.json()
 
-    def _patch(self, endpoint: str, json: json_types) -> json_types:
+    def patch(self, endpoint: str, json: json_types) -> json_types:
         url = self._get_url(endpoint)
         response = self.auth.request("PATCH", url, json=json)
         response.raise_for_status()
         return response.json()
 
-    def _delete(self, endpoint: str) -> json_types:
+    def delete(self, endpoint: str) -> json_types:
         url = self._get_url(endpoint)
         response = self.auth.request("DELETE", url)
         response.raise_for_status()
         return response.json()
 
     # Async wrappers for HTTP methods
-    def _async_get(
+    def async_get(
         self, async_partial_contexts: list[AsyncRequestPartialContext]
     ) -> list[AsyncResponseContext]:
         all_requests_context = [
             AsyncRequestContext(
                 id=partial_context.id,
                 url=self._get_url(partial_context.endpoint),
                 params=partial_context.params,
```

### Comparing `bigdata_client-0.0.6/bigdata/daterange.py` & `bigdata_client-0.0.7/bigdata/daterange.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/bigdata/entity_types.py` & `bigdata_client-0.0.7/bigdata/entity_types.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/bigdata/enum_utils.py` & `bigdata_client-0.0.7/bigdata/enum_utils.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/bigdata/jwt.py` & `bigdata_client-0.0.7/bigdata/jwt.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/bigdata/models/advanced_search_query.py` & `bigdata_client-0.0.7/bigdata/models/advanced_search_query.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/bigdata/models/comentions.py` & `bigdata_client-0.0.7/bigdata/models/comentions.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/bigdata/models/entities.py` & `bigdata_client-0.0.7/bigdata/models/entities.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 class Product(_AbstractEntity):
     model_config = ConfigDict(populate_by_name=True)
     id: str = Field(validation_alias="key")
     name: str
     entity_type: Literal["PROD"] = Field(default="PROD", validation_alias="entityType")
     product_type: str = Field(validation_alias="group1")
-    product_owner: str = Field(validation_alias="group2")
+    product_owner: Optional[str] = Field(validation_alias="group2", default=None)
 
 
 # TODO rm queryType from models, create MacroModel
 class ProductType(_AbstractEntity):
     model_config = ConfigDict(populate_by_name=True)
     id: str = Field(validation_alias="key")
     name: str
```

### Comparing `bigdata_client-0.0.6/bigdata/models/languages.py` & `bigdata_client-0.0.7/bigdata/models/languages.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/bigdata/models/parse.py` & `bigdata_client-0.0.7/bigdata/models/parse.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/bigdata/models/search.py` & `bigdata_client-0.0.7/bigdata/models/search.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/bigdata/models/sources.py` & `bigdata_client-0.0.7/bigdata/models/sources.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/bigdata/models/story.py` & `bigdata_client-0.0.7/bigdata/models/story.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/bigdata/models/topics.py` & `bigdata_client-0.0.7/bigdata/models/topics.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/bigdata/models/uploads.py` & `bigdata_client-0.0.7/bigdata/models/uploads.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/bigdata/models/watchlists.py` & `bigdata_client-0.0.7/bigdata/models/watchlists.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/bigdata/old_auth.py` & `bigdata_client-0.0.7/bigdata/old_auth.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/bigdata/query.py` & `bigdata_client-0.0.7/bigdata/query.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/bigdata/search.py` & `bigdata_client-0.0.7/bigdata/search.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/bigdata/services.py` & `bigdata_client-0.0.7/bigdata/services.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/bigdata/settings.py` & `bigdata_client-0.0.7/bigdata/settings.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/bigdata/simple_search_query.py` & `bigdata_client-0.0.7/bigdata/simple_search_query.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/bigdata/story.py` & `bigdata_client-0.0.7/bigdata/story.py`

 * *Files identical despite different names*

### Comparing `bigdata_client-0.0.6/pyproject.toml` & `bigdata_client-0.0.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 [tool.poetry]
 name = "bigdata-client"
 packages = [
     { include = "bigdata" },
 ]
-version = "0.0.6"
+version = "0.0.7"
 description = ""
 authors = [
-    "Iago Veloso <iago@ravenpack.com>",
-    "Diego de Aguilar <ddeaguilar@ravenpack.com>",
-    "Jose Ramon Cano <jcano@ravenpack.com>"
+    "Bigdata Team <support@bigdata.com>"
 ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.31.0"
 pydantic = "^2.5.3"
```

### Comparing `bigdata_client-0.0.6/PKG-INFO` & `bigdata_client-0.0.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bigdata-client
-Version: 0.0.6
+Version: 0.0.7
 Summary: 
-Author: Iago Veloso
-Author-email: iago@ravenpack.com
+Author: Bigdata Team
+Author-email: support@bigdata.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
```

