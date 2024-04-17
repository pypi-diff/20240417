# Comparing `tmp/tehzor-0.0.2.tar.gz` & `tmp/tehzor-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tehzor-0.0.2.tar", last modified: Fri Apr 12 13:26:34 2024, max compression
+gzip compressed data, was "tehzor-0.0.3.tar", last modified: Wed Apr 17 07:10:42 2024, max compression
```

## Comparing `tehzor-0.0.2.tar` & `tehzor-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 13:26:34.000163 tehzor-0.0.2/
--rw-rw-rw-   0        0        0     1082 2024-04-12 09:32:26.000000 tehzor-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1959 2024-04-12 13:26:34.000163 tehzor-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1184 2024-04-12 10:21:21.000000 tehzor-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-12 13:26:34.000163 tehzor-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1028 2024-04-12 13:26:04.000000 tehzor-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:26:33.994866 tehzor-0.0.2/tehzor/
--rw-rw-rw-   0        0        0       83 2024-04-12 08:09:01.000000 tehzor-0.0.2/tehzor/__init__.py
--rw-rw-rw-   0        0        0     5976 2024-04-12 13:06:38.000000 tehzor-0.0.2/tehzor/api.py
--rw-rw-rw-   0        0        0      748 2024-04-11 13:41:40.000000 tehzor-0.0.2/tehzor/constants_thz.py
--rw-rw-rw-   0        0        0     2907 2024-04-12 07:01:24.000000 tehzor-0.0.2/tehzor/models_thz.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:26:33.999053 tehzor-0.0.2/tehzor.egg-info/
--rw-rw-rw-   0        0        0     1959 2024-04-12 13:26:33.000000 tehzor-0.0.2/tehzor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2024-04-12 13:26:33.000000 tehzor-0.0.2/tehzor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 13:26:33.000000 tehzor-0.0.2/tehzor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-04-12 13:26:33.000000 tehzor-0.0.2/tehzor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-12 13:26:33.000000 tehzor-0.0.2/tehzor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 07:10:42.394502 tehzor-0.0.3/
+-rw-rw-rw-   0        0        0     1082 2024-04-12 09:32:26.000000 tehzor-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1955 2024-04-17 07:10:42.393502 tehzor-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1180 2024-04-17 06:48:00.000000 tehzor-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-17 07:10:42.394502 tehzor-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1028 2024-04-17 06:48:48.000000 tehzor-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 07:10:42.383501 tehzor-0.0.3/tehzor/
+-rw-rw-rw-   0        0        0       77 2024-04-17 06:33:50.000000 tehzor-0.0.3/tehzor/__init__.py
+-rw-rw-rw-   0        0        0     6700 2024-04-17 06:33:50.000000 tehzor-0.0.3/tehzor/api.py
+-rw-rw-rw-   0        0        0      748 2024-04-17 06:33:50.000000 tehzor-0.0.3/tehzor/constants.py
+-rw-rw-rw-   0        0        0     4170 2024-04-17 06:33:50.000000 tehzor-0.0.3/tehzor/models.py
+drwxrwxrwx   0        0        0        0 2024-04-17 07:10:42.392502 tehzor-0.0.3/tehzor.egg-info/
+-rw-rw-rw-   0        0        0     1955 2024-04-17 07:10:42.000000 tehzor-0.0.3/tehzor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2024-04-17 07:10:42.000000 tehzor-0.0.3/tehzor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 07:10:42.000000 tehzor-0.0.3/tehzor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-17 07:10:42.000000 tehzor-0.0.3/tehzor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-17 07:10:42.000000 tehzor-0.0.3/tehzor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 07:10:42.391502 tehzor-0.0.3/tests/
+-rw-rw-rw-   0        0        0      531 2024-04-17 06:33:50.000000 tehzor-0.0.3/tests/test_api_create.py
+-rw-rw-rw-   0        0        0      927 2024-04-17 06:33:50.000000 tehzor-0.0.3/tests/test_get_problem_id.py
+-rw-rw-rw-   0        0        0      975 2024-04-17 06:33:50.000000 tehzor-0.0.3/tests/test_get_work_acceptance.py
```

### Comparing `tehzor-0.0.2/LICENSE.txt` & `tehzor-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tehzor-0.0.2/PKG-INFO` & `tehzor-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tehzor
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python API wrapper for Tehzor API
 Home-page: https://github.com/gritsyuk/tehzor
 Download-URL: https://github.com/gritsyuk/tehzor/archive/refs/heads/develop.zip
 Author: Igor Gritsyuk
 Author-email: gritsyuk.igor@gmail.com
 Project-URL: GitHub, https://github.com/gritsyuk/tehzor
 Keywords: tehzor api tehzorapi construction supervision operation inspections constarctionsite building management
@@ -14,42 +14,41 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: aiohttp>=3.9.3
 Requires-Dist: pydantic[email]>=2.6.4
 
 # ![logo Tehzor](https://tehzor.com/images/components/Header/logo.svg)
-
+![PyPI - Version](https://img.shields.io/pypi/v/tehzor)
 ## Обертка над  API системы Техзор на python (async/await)
 Официальная документация [https://api.tehzor.ru/docs](https://api.tehzor.ru/docs)
 
 ## Установка
-
 ```bash
 pip install tehzor
 ```
 
 ## Примеры
-Обновления параметров квартир (площадь, плащадь БТИ, тип отделки). Предварительно необходимо знать id квартир и id типа отделки:
+Обновления параметров квартир (площадь, плащадь БТИ, тип отделки ...). Предварительно необходимо знать id квартир и id типа отделки:
 ```python
 from tehzor import TehzorAPI
 from excel_apartments import result_flats
 
 
 API_KEY = "00000000-0000-0000-0000-000000000000"
 USER_ID = "123d7cdfc7ea123d123456ab"
 
 
 async def main():     
-    thz = await TehzorAPI.create(api_key=API_KEY, 
-                                 user_id=USER_ID
-                                )
+    thz = await TehzorAPI.create(api_key=API_KEY, user_id=USER_ID)
+    
     async with asyncio.TaskGroup() as tg:
         for id, data in result_flats.items():
             tg.create_task(thz.update_spaces(id, data.model_dump_json()))
+
     await thz.session_close()
 
 
 if __name__ == "__main__":    
     asyncio.run(main())
 ```
```

### Comparing `tehzor-0.0.2/README.md` & `tehzor-0.0.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 # ![logo Tehzor](https://tehzor.com/images/components/Header/logo.svg)
-
+![PyPI - Version](https://img.shields.io/pypi/v/tehzor)
 ## Обертка над  API системы Техзор на python (async/await)
 Официальная документация [https://api.tehzor.ru/docs](https://api.tehzor.ru/docs)
 
 ## Установка
-
 ```bash
 pip install tehzor
 ```
 
 ## Примеры
-Обновления параметров квартир (площадь, плащадь БТИ, тип отделки). Предварительно необходимо знать id квартир и id типа отделки:
+Обновления параметров квартир (площадь, плащадь БТИ, тип отделки ...). Предварительно необходимо знать id квартир и id типа отделки:
 ```python
 from tehzor import TehzorAPI
 from excel_apartments import result_flats
 
 
 API_KEY = "00000000-0000-0000-0000-000000000000"
 USER_ID = "123d7cdfc7ea123d123456ab"
 
 
 async def main():     
-    thz = await TehzorAPI.create(api_key=API_KEY, 
-                                 user_id=USER_ID
-                                )
+    thz = await TehzorAPI.create(api_key=API_KEY, user_id=USER_ID)
+    
     async with asyncio.TaskGroup() as tg:
         for id, data in result_flats.items():
             tg.create_task(thz.update_spaces(id, data.model_dump_json()))
+
     await thz.session_close()
 
 
 if __name__ == "__main__":    
     asyncio.run(main())
 ```
```

### Comparing `tehzor-0.0.2/setup.py` & `tehzor-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
   
 
 setup(
   name='tehzor',
-  version='0.0.2',
+  version='0.0.3',
   author='Igor Gritsyuk',
   author_email='gritsyuk.igor@gmail.com',
   description='A Python API wrapper for Tehzor API',
   download_url='https://github.com/gritsyuk/tehzor/archive/refs/heads/develop.zip',
   long_description=long_description,
   long_description_content_type='text/markdown',
   url='https://github.com/gritsyuk/tehzor',
```

### Comparing `tehzor-0.0.2/tehzor/api.py` & `tehzor-0.0.3/tehzor/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 from aiohttp import ClientSession, ClientResponse
 from asyncio import Semaphore
 from typing import List, AsyncGenerator, Optional
-from .models_thz import ProblemFilter
+from .models import ProblemFilter, Problem, WorkAcceptances
+
 
 class TehzorAPIError(Exception):
     pass
 
 
 class TehzorAPI(object):
     def __init__(self) -> None:
         pass
-    
+
     @classmethod
-    async def create(cls, 
-                     api_key: str, 
-                     url_api: str = "https://api.tehzor.ru", 
-                     user_id: str = None, 
+    async def create(cls,
+                     api_key: str,
+                     url_api: str = "https://api.tehzor.ru",
+                     user_id: str = None,
                      proxy: str = None,
                      limit_threads: int = 25):
         self = cls()
         self.url_api = url_api
-        self.user_id = user_id 
-        self.headers =  {
-                        "Content-Type": "application/json",
-                        "api-key": api_key
-                        }
+        self.user_id = user_id
+        self.headers = {
+            "Content-Type": "application/json",
+            "api-key": api_key
+        }
         self.proxy = proxy
-        self.semaphore = Semaphore(limit_threads)  
+        self.semaphore = Semaphore(limit_threads)
         self.session = ClientSession(base_url=self.url_api, headers=self.headers)
-        
+
         return self
-    
 
     async def session_close(self):
-        await self.session.close() 
+        await self.session.close()
 
-    
     async def _handle_response(self, response: ClientResponse):
-        try:    
-            if response.status == 200:
+        try:
+            if response.status == 200 or response.status == 201:
                 return
             elif response.status == 400:
                 raise TehzorAPIError(f"ERROR {response.status}: Error while fetching the violation list")
             elif response.status == 401:
                 raise TehzorAPIError(f"ERROR {response.status}: Unauthorized (api-key not provided)")
             elif response.status == 403:
                 raise TehzorAPIError(f"ERROR {response.status}: Access forbidden")
@@ -54,101 +53,108 @@
                 raise TehzorAPIError(f"ERROR {response.status}: Server limit exceeded 0.5 Mb or other server error")
             else:
                 raise TehzorAPIError(f"Unhandled status code: {response.status}")
         except TehzorAPIError:
             await self.session.close()
             raise
 
+    async def get_problem(self, id: str) -> Problem:
+        url = f"/problems/{id}"
+        async with self.session.get(url,
+                                    proxy=self.proxy,
+                                    verify_ssl=False) as r:
+            await self._handle_response(r)
+            res_json = await r.json()
+
+            return Problem.model_validate(res_json)
 
-    async def _get_problems_chunk(self, limit: int, offset: int, filter: Optional[ProblemFilter]) -> List[dict]:
+    async def get_problems(self,
+                           user_id: str = None,  
+                           limit: int = 50000,
+                           offset: int = 0, 
+                           filter: Optional[ProblemFilter] = None) -> AsyncGenerator[Problem, None]:
         url = r"/problems"
-        params = dict(userId=self.user_id, limit=limit, offset=offset)
+        if not user_id and self.user_id:
+            user_id = self.user_id
+        params = dict(userId=user_id,
+                      limit=limit, 
+                      offset=offset)
         filter_json = filter.model_dump() if filter else None
-
         async with self.session.get(url, 
                                     params=params, 
                                     proxy=self.proxy, 
-                                    json=filter_json,
+                                    json=filter_json) as r:
+            await self._handle_response(r)
+            res_json = await r.json()
+            for data in res_json:
+                yield Problem.model_validate(data)
+    
+    async def get_work_acceptance(self, id: str) -> WorkAcceptances:
+        url = f"/work-acceptances/{id}"
+        async with self.session.get(url,
+                                    proxy=self.proxy,
                                     verify_ssl=False) as r:
             await self._handle_response(r)
-            return await r.json()
-        
+            res_json = await r.json()
+            return WorkAcceptances.model_validate(res_json)
 
-    async def get_problems(self, limit: int = 50000, 
-                           offset: int = 0, 
-                           filter: Optional[ProblemFilter] = None) -> AsyncGenerator[dict, None]:
-        total_problems = 0
-        total_loaded = 0
-        chunk_size = 50000
-
-        while True:
-            problems_chunk = await self._get_problems_chunk(limit, offset, filter)
-
-            if not problems_chunk:
-                break
-
-            total_problems += len(problems_chunk)
-            total_loaded += len(problems_chunk)
-
-            if total_loaded > total_problems:
-                break
-
-            for problem in problems_chunk:
-                yield problem
-
-            offset += chunk_size
-
-    # async def get_problems(self, limit: int = 100, offset: int = 0, filter: Optional[ProblemFilter] = None) -> List[dict]:
-    #     url = r"/problems"
-    #     params = dict(userId=self.user_id, limit=limit, offset=offset)
-    #     filter_json = filter.model_dump() if filter else None
-    #     async with self.session.get(url, params=params, proxy=self.proxy, json=filter_json) as r:
-    #         await self._handle_response(r)
-    #         return await r.json()        
-    
-
-    async def get_problem(self, id: str) -> dict:
-        url = fr"/problems/{id}"
-        async with self.session.get(url, 
+    async def get_work_acceptances(self,
+                                   object_id: str= "",
+                                   limit: int = 50000,
+                                   offset: int = 0,
+                                   ) -> AsyncGenerator[WorkAcceptances, None]:
+        url = "/work-acceptances"
+        params = dict(objectId=object_id,
+                      limit=limit, 
+                      offset=offset)
+        async with self.session.get(url,
+                                    params=params,
                                     proxy=self.proxy,
                                     verify_ssl=False) as r:
-            assert r.status == 200
-            return await r.json()
-        
+            await self._handle_response(r)
+            res_json = await r.json()
+            for data in res_json:
+                yield WorkAcceptances.model_validate(data)
 
     async def update_problem(self, id: str, data: dict):
         url = fr"/problems/{id}"
-        async with self.session.post(url, 
-                                     data = data, 
+        async with self.session.post(url,
+                                     data=data,
                                      proxy=self.proxy,
                                      verify_ssl=False) as r:
-            assert r.status == 201 
+            assert r.status == 201
             return await r.json()
-
+    
+    # async def create_problem(self, data: ProblemNew) -> Problem:
+    #     url = fr"/problems"
+    #     async with self.session.post(url,
+    #                                  data=data,
+    #                                  proxy=self.proxy,
+    #                                  verify_ssl=False) as r:
+            # assert r.status == 201
+            # return await r.json()
 
     async def get_contract_forms(self) -> dict:
         url = r"/contract-forms"
-        async with self.session.get(url, 
-                                    proxy=self.proxy, 
+        async with self.session.get(url,
+                                    proxy=self.proxy,
                                     verify_ssl=False) as r:
             assert r.status == 200
             return await r.json()
-    
 
     async def create_owners(self, data: dict):
         url = fr"/space-owners"
         async with self.semaphore:
-            async with self.session.post(url, 
-                                         data = data, 
-                                         proxy=self.proxy, 
+            async with self.session.post(url,
+                                         data=data,
+                                         proxy=self.proxy,
                                          verify_ssl=False) as r:
                 assert r.status == 201
-    
 
     async def update_spaces(self, id: str, data: dict):
         url = fr"/spaces/{id}"
         async with self.semaphore:
-            async with self.session.post(url, 
-                                         data = data, 
-                                         proxy=self.proxy, 
+            async with self.session.post(url,
+                                         data=data,
+                                         proxy=self.proxy,
                                          verify_ssl=False) as r:
-                assert r.status == 201
+                assert r.status == 201
```

### Comparing `tehzor-0.0.2/tehzor/constants_thz.py` & `tehzor-0.0.3/tehzor/constants.py`

 * *Files identical despite different names*

### Comparing `tehzor-0.0.2/tehzor.egg-info/PKG-INFO` & `tehzor-0.0.3/tehzor.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tehzor
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python API wrapper for Tehzor API
 Home-page: https://github.com/gritsyuk/tehzor
 Download-URL: https://github.com/gritsyuk/tehzor/archive/refs/heads/develop.zip
 Author: Igor Gritsyuk
 Author-email: gritsyuk.igor@gmail.com
 Project-URL: GitHub, https://github.com/gritsyuk/tehzor
 Keywords: tehzor api tehzorapi construction supervision operation inspections constarctionsite building management
@@ -14,42 +14,41 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: aiohttp>=3.9.3
 Requires-Dist: pydantic[email]>=2.6.4
 
 # ![logo Tehzor](https://tehzor.com/images/components/Header/logo.svg)
-
+![PyPI - Version](https://img.shields.io/pypi/v/tehzor)
 ## Обертка над  API системы Техзор на python (async/await)
 Официальная документация [https://api.tehzor.ru/docs](https://api.tehzor.ru/docs)
 
 ## Установка
-
 ```bash
 pip install tehzor
 ```
 
 ## Примеры
-Обновления параметров квартир (площадь, плащадь БТИ, тип отделки). Предварительно необходимо знать id квартир и id типа отделки:
+Обновления параметров квартир (площадь, плащадь БТИ, тип отделки ...). Предварительно необходимо знать id квартир и id типа отделки:
 ```python
 from tehzor import TehzorAPI
 from excel_apartments import result_flats
 
 
 API_KEY = "00000000-0000-0000-0000-000000000000"
 USER_ID = "123d7cdfc7ea123d123456ab"
 
 
 async def main():     
-    thz = await TehzorAPI.create(api_key=API_KEY, 
-                                 user_id=USER_ID
-                                )
+    thz = await TehzorAPI.create(api_key=API_KEY, user_id=USER_ID)
+    
     async with asyncio.TaskGroup() as tg:
         for id, data in result_flats.items():
             tg.create_task(thz.update_spaces(id, data.model_dump_json()))
+
     await thz.session_close()
 
 
 if __name__ == "__main__":    
     asyncio.run(main())
 ```
```

