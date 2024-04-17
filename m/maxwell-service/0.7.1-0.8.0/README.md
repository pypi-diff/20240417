# Comparing `tmp/maxwell_service-0.7.1.tar.gz` & `tmp/maxwell_service-0.8.0.tar.gz`

## Comparing `maxwell_service-0.7.1.tar` & `maxwell_service-0.8.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 maxwell_service-0.7.1/.git
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 maxwell_service-0.7.1/Makefile
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 maxwell_service-0.7.1/requirements.txt
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 maxwell_service-0.7.1/setup.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 maxwell_service-0.7.1/.vscode/settings.json
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 maxwell_service-0.7.1/config/logging.json
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 maxwell_service-0.7.1/config/service.template.toml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 maxwell_service-0.7.1/examples/__init__.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 maxwell_service-0.7.1/examples/hello.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 maxwell_service-0.7.1/maxwell/__init__.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 maxwell_service-0.7.1/maxwell/service/__init__.py
--rw-r--r--   0        0        0     5714 2020-02-02 00:00:00.000000 maxwell_service-0.7.1/maxwell/service/config.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 maxwell_service-0.7.1/maxwell/service/hooks.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 maxwell_service-0.7.1/maxwell/service/master_client.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 maxwell_service-0.7.1/maxwell/service/publisher.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 maxwell_service-0.7.1/maxwell/service/registrar.py
--rw-r--r--   0        0        0     3258 2020-02-02 00:00:00.000000 maxwell_service-0.7.1/maxwell/service/server.py
--rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 maxwell_service-0.7.1/maxwell/service/service.py
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 maxwell_service-0.7.1/maxwell/service/topic_locatlizer.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 maxwell_service-0.7.1/maxwell/service/worker.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 maxwell_service-0.7.1/test/__init__.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 maxwell_service-0.7.1/test/test_config.py
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 maxwell_service-0.7.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 maxwell_service-0.7.1/LICENSE
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 maxwell_service-0.7.1/README.md
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 maxwell_service-0.7.1/pyproject.toml
--rw-r--r--   0        0        0    14000 2020-02-02 00:00:00.000000 maxwell_service-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 maxwell_service-0.8.0/.git
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 maxwell_service-0.8.0/Makefile
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 maxwell_service-0.8.0/requirements.txt
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 maxwell_service-0.8.0/setup.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 maxwell_service-0.8.0/.vscode/settings.json
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 maxwell_service-0.8.0/config/logging.json
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 maxwell_service-0.8.0/config/service.template.toml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 maxwell_service-0.8.0/examples/__init__.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 maxwell_service-0.8.0/examples/hello.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 maxwell_service-0.8.0/maxwell/__init__.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 maxwell_service-0.8.0/maxwell/service/__init__.py
+-rw-r--r--   0        0        0     5714 2020-02-02 00:00:00.000000 maxwell_service-0.8.0/maxwell/service/config.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 maxwell_service-0.8.0/maxwell/service/hooks.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 maxwell_service-0.8.0/maxwell/service/master_client.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 maxwell_service-0.8.0/maxwell/service/publisher.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 maxwell_service-0.8.0/maxwell/service/registrar.py
+-rw-r--r--   0        0        0     3258 2020-02-02 00:00:00.000000 maxwell_service-0.8.0/maxwell/service/server.py
+-rw-r--r--   0        0        0     5550 2020-02-02 00:00:00.000000 maxwell_service-0.8.0/maxwell/service/service.py
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 maxwell_service-0.8.0/maxwell/service/topic_locatlizer.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 maxwell_service-0.8.0/maxwell/service/worker.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 maxwell_service-0.8.0/test/__init__.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 maxwell_service-0.8.0/test/test_config.py
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 maxwell_service-0.8.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 maxwell_service-0.8.0/LICENSE
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 maxwell_service-0.8.0/README.md
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 maxwell_service-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    14000 2020-02-02 00:00:00.000000 maxwell_service-0.8.0/PKG-INFO
```

### Comparing `maxwell_service-0.7.1/Makefile` & `maxwell_service-0.8.0/Makefile`

 * *Files identical despite different names*

### Comparing `maxwell_service-0.7.1/requirements.txt` & `maxwell_service-0.8.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `maxwell_service-0.7.1/config/logging.json` & `maxwell_service-0.8.0/config/logging.json`

 * *Files identical despite different names*

### Comparing `maxwell_service-0.7.1/maxwell/service/config.py` & `maxwell_service-0.8.0/maxwell/service/config.py`

 * *Files identical despite different names*

### Comparing `maxwell_service-0.7.1/maxwell/service/hooks.py` & `maxwell_service-0.8.0/maxwell/service/hooks.py`

 * *Files identical despite different names*

### Comparing `maxwell_service-0.7.1/maxwell/service/master_client.py` & `maxwell_service-0.8.0/maxwell/service/master_client.py`

 * *Files identical despite different names*

### Comparing `maxwell_service-0.7.1/maxwell/service/publisher.py` & `maxwell_service-0.8.0/maxwell/service/publisher.py`

 * *Files identical despite different names*

### Comparing `maxwell_service-0.7.1/maxwell/service/registrar.py` & `maxwell_service-0.8.0/maxwell/service/registrar.py`

 * *Files identical despite different names*

### Comparing `maxwell_service-0.7.1/maxwell/service/server.py` & `maxwell_service-0.8.0/maxwell/service/server.py`

 * *Files identical despite different names*

### Comparing `maxwell_service-0.7.1/maxwell/service/service.py` & `maxwell_service-0.8.0/maxwell/service/service.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,40 @@
 import asyncio
 import functools
 import inspect
+import json
 import traceback
-from typing import Any
+from typing import Any, TypeAlias
 from fastapi import FastAPI, WebSocket, WebSocketDisconnect
 from maxwell.utils.logger import get_logger
 import maxwell.protocol.maxwell_protocol_pb2 as protocol_types
 import maxwell.protocol.maxwell_protocol as protocol
 
 logger = get_logger(__name__)
 
 
+Request: TypeAlias = protocol_types.req_req_t
+
+V0 = 0
+V1 = 1
+
+
+class Reply:
+    def __init__(self, code: int = 0, desc: str = "", payload: str = ""):
+        self.code = code
+        self.desc = desc
+        self.payload = payload
+
+
 class Service(FastAPI):
     def __init__(self, *args: Any, **kwargs: Any):
         super(Service, self).__init__(*args, **kwargs)
         self.__is_registered = False
         self.__ws_routes = {}
-        self.__init_ws()
+        self.__on_ws_msg()
 
     def register(self):
         if self.__is_registered is False:
             self.__is_registered = True
         return self
 
     def is_registered(self):
@@ -29,54 +43,100 @@
     def ws(self, path):
         def decorator(func):
             @functools.wraps(func)
             def func_wrapper(*args, **kwargs):
                 value = func(*args, **kwargs)
                 return value
 
-            self.__ws_routes[path] = [func_wrapper, inspect.iscoroutinefunction(func)]
+            self.__ws_routes[path] = [
+                func_wrapper,
+                inspect.iscoroutinefunction(func),
+                V0,
+            ]
+            return func_wrapper
+
+        return decorator
+
+    def add_ws_route(self, path):
+        def decorator(func):
+            @functools.wraps(func)
+            def func_wrapper(*args, **kwargs):
+                value = func(*args, **kwargs)
+                return value
+
+            self.__ws_routes[path] = [
+                func_wrapper,
+                inspect.iscoroutinefunction(func),
+                V1,
+            ]
             return func_wrapper
 
         return decorator
 
     def get_ws_routes(self):
         return self.__ws_routes
 
     def get_paths(self):
         return list(self.__ws_routes.keys())
 
     def get_handler(self, path):
         return self.__ws_routes.get(path)
 
-    def __init_ws(self):
+    def __on_ws_msg(self):
         @self.websocket("/$ws")
         async def websocket_endpoint(websocket: WebSocket):
             await websocket.accept()
             try:
                 while True:
                     data = await websocket.receive_bytes()
                     asyncio.ensure_future(self.__handle_msg(websocket, data))
             except WebSocketDisconnect as e:
                 logger.warning("Connection was closed: %s", e)
+            except Exception:
+                logger.error(
+                    "Failed to handle data: %s, error: %s", data, traceback.format_exc()
+                )
 
     async def __handle_msg(self, websocket, data):
         try:
             req = protocol.decode_msg(data)
             if req.__class__ == protocol_types.req_req_t:
+                logger.debug("Received msg: %s", req)
                 handler = self.get_handler(req.path)
                 if handler is not None:
-                    logger.debug("Received msg: %s", req)
-                    rep = protocol_types.req_rep_t()
-                    if handler[1] is True:
-                        rep.payload = await handler[0](req)
+                    handle, is_coroutine, version = handler
+                    if version == V1:
+                        if is_coroutine is True:
+                            userland_rep: Reply = await handle(req)
+                        else:
+                            userland_rep: Reply = handle(req)
+                        if userland_rep.code == protocol_types.error_code_t.OK:
+                            rep = protocol_types.req_rep_t()
+                            rep.payload = json.dumps(userland_rep.payload)
+                            rep.conn0_ref = req.conn0_ref
+                            rep.ref = req.ref
+                            await websocket.send_bytes(protocol.encode_msg(rep))
+                        else:
+                            rep = protocol_types.error2_rep_t()
+                            rep.code = userland_rep.code
+                            rep.desc = userland_rep.desc
+                            rep.conn0_ref = req.conn0_ref
+                            rep.ref = req.ref
+                            await websocket.send_bytes(protocol.encode_msg(rep))
+                    elif version == V0:
+                        rep = protocol_types.req_rep_t()
+                        if is_coroutine is True:
+                            rep.payload = await handle(req)
+                        else:
+                            rep.payload = handle(req)
+                        rep.conn0_ref = req.conn0_ref
+                        rep.ref = req.ref
+                        await websocket.send_bytes(protocol.encode_msg(rep))
                     else:
-                        rep.payload = handler[0](req)
-                    rep.conn0_ref = req.conn0_ref
-                    rep.ref = req.ref
-                    await websocket.send_bytes(protocol.encode_msg(rep))
+                        raise SystemExit("Unknown version: %s" % version)
                 else:
                     logger.error("Unknown path: %s", req.path)
                     rep = protocol_types.error2_rep_t()
                     rep.code = protocol_types.error_code_t.UNKNOWN_PATH
                     rep.desc = "Unknown path: %s" % req.path
                     rep.conn0_ref = req.conn0_ref
                     rep.ref = req.ref
```

### Comparing `maxwell_service-0.7.1/maxwell/service/topic_locatlizer.py` & `maxwell_service-0.8.0/maxwell/service/topic_locatlizer.py`

 * *Files identical despite different names*

### Comparing `maxwell_service-0.7.1/maxwell/service/worker.py` & `maxwell_service-0.8.0/maxwell/service/worker.py`

 * *Files identical despite different names*

### Comparing `maxwell_service-0.7.1/.gitignore` & `maxwell_service-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `maxwell_service-0.7.1/LICENSE` & `maxwell_service-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `maxwell_service-0.7.1/pyproject.toml` & `maxwell_service-0.8.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
   "maxwell-utils == 0.6.2",
 ]
 description = "The maxwell service implementation for python."
 license = {file = "LICENSE"}
 name = "maxwell-service"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "0.7.1"
+version = "0.8.0"
 
 [tool.pytest.ini_options]
 log_cli = true
 log_cli_date_format = "%Y-%m-%d %H:%M:%S"
 log_cli_format = "[%(levelname)8s] %(asctime)s (%(filename)s:%(lineno)s) %(message)s"
 log_cli_level = "DEBUG"
```

### Comparing `maxwell_service-0.7.1/PKG-INFO` & `maxwell_service-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxwell-service
-Version: 0.7.1
+Version: 0.8.0
 Summary: The maxwell service implementation for python.
 Project-URL: changelog, https://github.com/maxwell-dev/maxwell-service-python/CHANGELOG.md
 Project-URL: repository, https://github.com/maxwell-dev/maxwell-service-python
 Author-email: Xu Chaoqian <chaoranxu@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

