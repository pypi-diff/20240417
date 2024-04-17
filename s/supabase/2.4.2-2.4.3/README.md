# Comparing `tmp/supabase-2.4.2.tar.gz` & `tmp/supabase-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supabase-2.4.2.tar", max compression
+gzip compressed data, was "supabase-2.4.3.tar", max compression
```

## Comparing `supabase-2.4.2.tar` & `supabase-2.4.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1067 2024-04-14 00:32:56.096397 supabase-2.4.2/LICENSE
--rw-r--r--   0        0        0     8244 2024-04-14 00:32:56.096397 supabase-2.4.2/README.md
--rw-r--r--   0        0        0     1892 2024-04-14 00:33:01.912412 supabase-2.4.2/pyproject.toml
--rw-r--r--   0        0        0      751 2024-04-14 00:32:56.096397 supabase-2.4.2/supabase/__init__.py
--rw-r--r--   0        0        0       22 2024-04-14 00:33:01.912412 supabase-2.4.2/supabase/__version__.py
--rw-r--r--   0        0        0       35 2024-04-14 00:32:56.096397 supabase-2.4.2/supabase/_async/__init__.py
--rw-r--r--   0        0        0     1130 2024-04-14 00:32:56.096397 supabase-2.4.2/supabase/_async/auth_client.py
--rw-r--r--   0        0        0    10713 2024-04-14 00:32:56.096397 supabase-2.4.2/supabase/_async/client.py
--rw-r--r--   0        0        0       35 2024-04-14 00:32:56.096397 supabase-2.4.2/supabase/_sync/__init__.py
--rw-r--r--   0        0        0     1120 2024-04-14 00:32:56.096397 supabase-2.4.2/supabase/_sync/auth_client.py
--rw-r--r--   0        0        0    10656 2024-04-14 00:32:56.096397 supabase-2.4.2/supabase/_sync/client.py
--rw-r--r--   0        0        0      772 2024-04-14 00:32:56.096397 supabase-2.4.2/supabase/client.py
--rw-r--r--   0        0        0      127 2024-04-14 00:32:56.096397 supabase-2.4.2/supabase/lib/__init__.py
--rw-r--r--   0        0        0     3133 2024-04-14 00:32:56.096397 supabase-2.4.2/supabase/lib/client_options.py
--rw-r--r--   0        0        0     1892 2024-04-14 00:32:56.096397 supabase-2.4.2/supabase/lib/realtime_client.py
--rw-r--r--   0        0        0        0 2024-04-14 00:32:56.096397 supabase-2.4.2/supabase/py.typed
--rw-r--r--   0        0        0     9313 1970-01-01 00:00:00.000000 supabase-2.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-17 14:07:12.395553 supabase-2.4.3/LICENSE
+-rw-r--r--   0        0        0     8244 2024-04-17 14:07:12.395553 supabase-2.4.3/README.md
+-rw-r--r--   0        0        0     1892 2024-04-17 14:07:18.427550 supabase-2.4.3/pyproject.toml
+-rw-r--r--   0        0        0      751 2024-04-17 14:07:12.399553 supabase-2.4.3/supabase/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-17 14:07:18.427550 supabase-2.4.3/supabase/__version__.py
+-rw-r--r--   0        0        0       35 2024-04-17 14:07:12.399553 supabase-2.4.3/supabase/_async/__init__.py
+-rw-r--r--   0        0        0     1130 2024-04-17 14:07:12.399553 supabase-2.4.3/supabase/_async/auth_client.py
+-rw-r--r--   0        0        0    10127 2024-04-17 14:07:12.399553 supabase-2.4.3/supabase/_async/client.py
+-rw-r--r--   0        0        0       35 2024-04-17 14:07:12.399553 supabase-2.4.3/supabase/_sync/__init__.py
+-rw-r--r--   0        0        0     1120 2024-04-17 14:07:12.399553 supabase-2.4.3/supabase/_sync/auth_client.py
+-rw-r--r--   0        0        0    10088 2024-04-17 14:07:12.399553 supabase-2.4.3/supabase/_sync/client.py
+-rw-r--r--   0        0        0      772 2024-04-17 14:07:12.399553 supabase-2.4.3/supabase/client.py
+-rw-r--r--   0        0        0      127 2024-04-17 14:07:12.399553 supabase-2.4.3/supabase/lib/__init__.py
+-rw-r--r--   0        0        0     3133 2024-04-17 14:07:12.399553 supabase-2.4.3/supabase/lib/client_options.py
+-rw-r--r--   0        0        0     1892 2024-04-17 14:07:12.399553 supabase-2.4.3/supabase/lib/realtime_client.py
+-rw-r--r--   0        0        0        0 2024-04-17 14:07:12.399553 supabase-2.4.3/supabase/py.typed
+-rw-r--r--   0        0        0     9313 1970-01-01 00:00:00.000000 supabase-2.4.3/PKG-INFO
```

### Comparing `supabase-2.4.2/LICENSE` & `supabase-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `supabase-2.4.2/README.md` & `supabase-2.4.3/README.md`

 * *Files identical despite different names*

### Comparing `supabase-2.4.2/pyproject.toml` & `supabase-2.4.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "supabase"
-version = "2.4.2"
+version = "2.4.3"
 description = "Supabase client for Python."
 authors = ["Joel Lee <joel@joellee.org>", "Leon Fedden <leonfedden@gmail.com>", "Daniel Reinón García <danielreinon@outlook.com>", "Leynier Gutiérrez González <leynier41@gmail.com>", "Anand", "Andrew Smith <a.smith@silentworks.co.uk>"]
 homepage = "https://github.com/supabase-community/supabase-py"
 repository = "https://github.com/supabase-community/supabase-py"
 documentation = "https://github.com/supabase-community/supabase-py"
 readme = "README.md"
 license = "MIT"
```

### Comparing `supabase-2.4.2/supabase/__init__.py` & `supabase-2.4.3/supabase/__init__.py`

 * *Files identical despite different names*

### Comparing `supabase-2.4.2/supabase/_async/auth_client.py` & `supabase-2.4.3/supabase/_async/auth_client.py`

 * *Files identical despite different names*

### Comparing `supabase-2.4.2/supabase/_async/client.py` & `supabase-2.4.3/supabase/_async/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,19 +63,16 @@
             raise SupabaseException("Invalid API key")
 
         if options is None:
             options = ClientOptions(storage=AsyncMemoryStorage())
 
         self.supabase_url = supabase_url
         self.supabase_key = supabase_key
-        self._auth_token = {
-            "Authorization": f"Bearer {supabase_key}",
-        }
-        options.headers.update(self._get_auth_headers())
         self.options = options
+        options.headers.update(self._get_auth_headers())
         self.rest_url = f"{supabase_url}/rest/v1"
         self.realtime_url = f"{supabase_url}/realtime/v1".replace("http", "ws")
         self.auth_url = f"{supabase_url}/auth/v1"
         self.storage_url = f"{supabase_url}/storage/v1"
         self.functions_url = f"{supabase_url}/functions/v1"
         self.schema = options.schema
 
@@ -98,17 +95,15 @@
     @classmethod
     async def create(
         cls,
         supabase_url: str,
         supabase_key: str,
         options: Union[ClientOptions, None] = None,
     ):
-        client = cls(supabase_url, supabase_key, options)
-        client._auth_token = await client._get_token_header()
-        return client
+        return cls(supabase_url, supabase_key, options)
 
     def table(self, table_name: str) -> AsyncRequestBuilder:
         """Perform a table operation.
 
         Note that the supabase client uses the `from` method, but in Python,
         this is a reserved keyword, so we have elected to use the name `table`.
         Alternatively you can use the `.from_()` method.
@@ -143,42 +138,39 @@
         if params is None:
             params = {}
         return self.postgrest.rpc(fn, params)
 
     @property
     def postgrest(self):
         if self._postgrest is None:
-            self.options.headers.update(self._auth_token)
             self._postgrest = self._init_postgrest_client(
                 rest_url=self.rest_url,
                 headers=self.options.headers,
                 schema=self.options.schema,
                 timeout=self.options.postgrest_client_timeout,
             )
 
         return self._postgrest
 
     @property
     def storage(self):
         if self._storage is None:
-            headers = self._get_auth_headers()
-            headers.update(self._auth_token)
             self._storage = self._init_storage_client(
                 storage_url=self.storage_url,
-                headers=headers,
+                headers=self.options.headers,
                 storage_client_timeout=self.options.storage_client_timeout,
             )
         return self._storage
 
     @property
     def functions(self):
         if self._functions is None:
-            headers = self._get_auth_headers()
-            headers.update(self._auth_token)
-            self._functions = AsyncFunctionsClient(self.functions_url, headers)
+            self._functions = AsyncFunctionsClient(
+                self.functions_url, self.options.headers
+            )
         return self._functions
 
     #     async def remove_subscription_helper(resolve):
     #         try:
     #             await self._close_subscription(subscription)
     #             open_subscriptions = len(self.get_subscriptions())
     #             if not open_subscriptions:
@@ -244,46 +236,37 @@
     ) -> AsyncPostgrestClient:
         """Private helper for creating an instance of the Postgrest client."""
         return AsyncPostgrestClient(
             rest_url, headers=headers, schema=schema, timeout=timeout
         )
 
     def _create_auth_header(self, token: str):
-        return {
-            "Authorization": f"Bearer {token}",
-        }
+        return f"Bearer {token}"
 
     def _get_auth_headers(self) -> Dict[str, str]:
         """Helper method to get auth headers."""
         return {
             "apiKey": self.supabase_key,
-            "Authorization": f"Bearer {self.supabase_key}",
+            "Authorization": self.options.headers.get(
+                "Authorization", self._create_auth_header(self.supabase_key)
+            ),
         }
 
-    async def _get_token_header(self):
-        try:
-            session = await self.auth.get_session()
-            access_token = session.access_token
-        except Exception as err:
-            access_token = self.supabase_key
-
-        return self._create_auth_header(access_token)
-
     def _listen_to_auth_events(
         self, event: AuthChangeEvent, session: Union[Session, None]
     ):
         access_token = self.supabase_key
         if event in ["SIGNED_IN", "TOKEN_REFRESHED", "SIGNED_OUT"]:
             # reset postgrest and storage instance on event change
             self._postgrest = None
             self._storage = None
             self._functions = None
             access_token = session.access_token if session else self.supabase_key
 
-        self._auth_token = self._create_auth_header(access_token)
+        self.options.headers["Authorization"] = self._create_auth_header(access_token)
 
 
 async def create_client(
     supabase_url: str,
     supabase_key: str,
     options: Union[ClientOptions, None] = None,
 ) -> AsyncClient:
```

### Comparing `supabase-2.4.2/supabase/_sync/auth_client.py` & `supabase-2.4.3/supabase/_sync/auth_client.py`

 * *Files identical despite different names*

### Comparing `supabase-2.4.2/supabase/_sync/client.py` & `supabase-2.4.3/supabase/_sync/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,19 +63,16 @@
             raise SupabaseException("Invalid API key")
 
         if options is None:
             options = ClientOptions(storage=SyncMemoryStorage())
 
         self.supabase_url = supabase_url
         self.supabase_key = supabase_key
-        self._auth_token = {
-            "Authorization": f"Bearer {supabase_key}",
-        }
-        options.headers.update(self._get_auth_headers())
         self.options = options
+        options.headers.update(self._get_auth_headers())
         self.rest_url = f"{supabase_url}/rest/v1"
         self.realtime_url = f"{supabase_url}/realtime/v1".replace("http", "ws")
         self.auth_url = f"{supabase_url}/auth/v1"
         self.storage_url = f"{supabase_url}/storage/v1"
         self.functions_url = f"{supabase_url}/functions/v1"
         self.schema = options.schema
 
@@ -98,17 +95,15 @@
     @classmethod
     def create(
         cls,
         supabase_url: str,
         supabase_key: str,
         options: Union[ClientOptions, None] = None,
     ):
-        client = cls(supabase_url, supabase_key, options)
-        client._auth_token = client._get_token_header()
-        return client
+        return cls(supabase_url, supabase_key, options)
 
     def table(self, table_name: str) -> SyncRequestBuilder:
         """Perform a table operation.
 
         Note that the supabase client uses the `from` method, but in Python,
         this is a reserved keyword, so we have elected to use the name `table`.
         Alternatively you can use the `.from_()` method.
@@ -143,42 +138,39 @@
         if params is None:
             params = {}
         return self.postgrest.rpc(fn, params)
 
     @property
     def postgrest(self):
         if self._postgrest is None:
-            self.options.headers.update(self._auth_token)
             self._postgrest = self._init_postgrest_client(
                 rest_url=self.rest_url,
                 headers=self.options.headers,
                 schema=self.options.schema,
                 timeout=self.options.postgrest_client_timeout,
             )
 
         return self._postgrest
 
     @property
     def storage(self):
         if self._storage is None:
-            headers = self._get_auth_headers()
-            headers.update(self._auth_token)
             self._storage = self._init_storage_client(
                 storage_url=self.storage_url,
-                headers=headers,
+                headers=self.options.headers,
                 storage_client_timeout=self.options.storage_client_timeout,
             )
         return self._storage
 
     @property
     def functions(self):
         if self._functions is None:
-            headers = self._get_auth_headers()
-            headers.update(self._auth_token)
-            self._functions = SyncFunctionsClient(self.functions_url, headers)
+            self._functions = SyncFunctionsClient(
+                self.functions_url, self.options.headers
+            )
         return self._functions
 
     #     async def remove_subscription_helper(resolve):
     #         try:
     #             await self._close_subscription(subscription)
     #             open_subscriptions = len(self.get_subscriptions())
     #             if not open_subscriptions:
@@ -244,46 +236,37 @@
     ) -> SyncPostgrestClient:
         """Private helper for creating an instance of the Postgrest client."""
         return SyncPostgrestClient(
             rest_url, headers=headers, schema=schema, timeout=timeout
         )
 
     def _create_auth_header(self, token: str):
-        return {
-            "Authorization": f"Bearer {token}",
-        }
+        return f"Bearer {token}"
 
     def _get_auth_headers(self) -> Dict[str, str]:
         """Helper method to get auth headers."""
         return {
             "apiKey": self.supabase_key,
-            "Authorization": f"Bearer {self.supabase_key}",
+            "Authorization": self.options.headers.get(
+                "Authorization", self._create_auth_header(self.supabase_key)
+            ),
         }
 
-    def _get_token_header(self):
-        try:
-            session = self.auth.get_session()
-            access_token = session.access_token
-        except Exception as err:
-            access_token = self.supabase_key
-
-        return self._create_auth_header(access_token)
-
     def _listen_to_auth_events(
         self, event: AuthChangeEvent, session: Union[Session, None]
     ):
         access_token = self.supabase_key
         if event in ["SIGNED_IN", "TOKEN_REFRESHED", "SIGNED_OUT"]:
             # reset postgrest and storage instance on event change
             self._postgrest = None
             self._storage = None
             self._functions = None
             access_token = session.access_token if session else self.supabase_key
 
-        self._auth_token = self._create_auth_header(access_token)
+        self.options.headers["Authorization"] = self._create_auth_header(access_token)
 
 
 def create_client(
     supabase_url: str,
     supabase_key: str,
     options: Union[ClientOptions, None] = None,
 ) -> SyncClient:
```

### Comparing `supabase-2.4.2/supabase/client.py` & `supabase-2.4.3/supabase/client.py`

 * *Files identical despite different names*

### Comparing `supabase-2.4.2/supabase/lib/client_options.py` & `supabase-2.4.3/supabase/lib/client_options.py`

 * *Files identical despite different names*

### Comparing `supabase-2.4.2/supabase/lib/realtime_client.py` & `supabase-2.4.3/supabase/lib/realtime_client.py`

 * *Files identical despite different names*

### Comparing `supabase-2.4.2/PKG-INFO` & `supabase-2.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supabase
-Version: 2.4.2
+Version: 2.4.3
 Summary: Supabase client for Python.
 Home-page: https://github.com/supabase-community/supabase-py
 License: MIT
 Author: Joel Lee
 Author-email: joel@joellee.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

