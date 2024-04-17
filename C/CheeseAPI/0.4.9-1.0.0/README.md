# Comparing `tmp/cheeseapi-0.4.9.tar.gz` & `tmp/cheeseapi-1.0.0.tar.gz`

## Comparing `cheeseapi-0.4.9.tar` & `cheeseapi-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/CheeseAPI/__init__.py
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/CheeseAPI/app.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/CheeseAPI/cors.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/CheeseAPI/exception.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/CheeseAPI/file.py
--rw-r--r--   0        0        0    30687 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/CheeseAPI/handle.py
--rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/CheeseAPI/protocol.py
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/CheeseAPI/request.py
--rw-r--r--   0        0        0    14572 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/CheeseAPI/response.py
--rw-r--r--   0        0        0     6814 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/CheeseAPI/route.py
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/CheeseAPI/server.py
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/CheeseAPI/signal.py
--rw-r--r--   0        0        0     7664 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/CheeseAPI/text.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/CheeseAPI/websocket.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/CheeseAPI/workspace.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/LICENSE
--rw-r--r--   0        0        0     4566 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/README.md
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/pyproject.toml
--rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 cheeseapi-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/CheeseAPI/__init__.py
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/CheeseAPI/app.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/CheeseAPI/cors.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/CheeseAPI/exception.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/CheeseAPI/file.py
+-rw-r--r--   0        0        0    30863 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/CheeseAPI/handle.py
+-rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/CheeseAPI/protocol.py
+-rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/CheeseAPI/request.py
+-rw-r--r--   0        0        0    15979 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/CheeseAPI/response.py
+-rw-r--r--   0        0        0     6814 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/CheeseAPI/route.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/CheeseAPI/server.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/CheeseAPI/signal.py
+-rw-r--r--   0        0        0     7664 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/CheeseAPI/text.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/CheeseAPI/websocket.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/CheeseAPI/workspace.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/LICENSE
+-rw-r--r--   0        0        0     4311 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 cheeseapi-1.0.0/PKG-INFO
```

### Comparing `cheeseapi-0.4.9/CheeseAPI/app.py` & `cheeseapi-1.0.0/CheeseAPI/app.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.9/CheeseAPI/file.py` & `cheeseapi-1.0.0/CheeseAPI/file.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.9/CheeseAPI/handle.py` & `cheeseapi-1.0.0/CheeseAPI/handle.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,15 +271,17 @@
                             'response': protocol.response,
                             **protocol.kwargs
                         })
                     await self.http_response(protocol)
                     return
 
                 if e.args[0] == 1:
-                    if isinstance(protocol.response, BaseResponse):
+                    if protocol.request.method == http.HTTPMethod.OPTIONS:
+                        protocol.response = Response(status = 200)
+
                         if self._app.signal.http_options.receivers:
                             await self._app.signal.http_options.send_async(**{
                                 'request': protocol.request,
                                 'response': protocol.response,
                                 **protocol.kwargs
                             })
                         await self.http_response(protocol)
@@ -342,14 +344,17 @@
                     await self._app.signal.http_static.send_async(**{
                         'request': protocol.request,
                         **protocol.kwargs
                     })
             except (FileNotFoundError, IsADirectoryError):
                 ...
 
+    async def http_options(self, protocol: 'HttpProtocol'):
+        protocol.response = Response(status = http.HTTPStatus.OK)
+
     async def http_404(self, protocol: 'HttpProtocol'):
         protocol.response = Response(status = http.HTTPStatus.NOT_FOUND)
 
     async def http_405(self, protocol: 'HttpProtocol'):
         protocol.response = Response(status = http.HTTPStatus.METHOD_NOT_ALLOWED)
 
     async def http_500(self, protocol: 'HttpProtocol', e: BaseException, recycled: bool = False):
@@ -384,16 +389,14 @@
             )
             and (
                 self._app.cors.methods == '*'
                 or
                 protocol.request.method in self._app.cors.methods
             )
         ):
-            protocol.response = Response(status = http.HTTPStatus.OK)
-
             protocol.response.headers['Access-Control-Allow-Origin'] = protocol.request.origin
 
             if self._app.cors.methods:
                 protocol.response.headers['Access-Control-Allow-Methods'] = ', '.join(self._app.cors.methods - self._app.cors.exclude_methods)
 
             if self._app.cors.headers == '*':
                 protocol.response.headers['Access-Control-Allow-Headers'] = self._app.cors.headers
@@ -650,14 +653,15 @@
                 await self._app.signal.websocket_beforeMessage.send_async(**{
                     'request': protocol.request,
                     'message': message,
                     **protocol.kwargs
                 })
 
             await protocol.server.message(**{
+                'request': protocol.request,
                 'message': message,
                 **protocol.kwargs
             })
 
             await self.websocket_afterMessage(protocol, message)
             if self._app.signal.websocket_afterMessage.receivers:
                 await self._app.signal.websocket_afterMessage.send_async({
```

### Comparing `cheeseapi-0.4.9/CheeseAPI/protocol.py` & `cheeseapi-1.0.0/CheeseAPI/protocol.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,19 @@
         self.request.headers['-'.join([t.capitalize() for t in key.decode().split('-')])] = value.decode()
 
     def on_headers_complete(self):
         self.request.client = self.request.headers.get('X-Real-Ip', self.transport.get_extra_info('socket').getpeername()[0])
         self.request.origin = self.request.headers.get('Origin', f'{self.transport.get_extra_info("socket").getsockname()[0]}:{self.transport.get_extra_info("socket").getsockname()[1]}')
         self.request.scheme = self.request.headers.get('X-Forwarded-Proto', 'https' if self.transport.get_extra_info('sslcontext') else 'http')
 
+        if 'Cookie' in self.request.headers:
+            self.request.cookie = {
+                t.split('=')[0]: t.split('=')[1] for t in self.request.headers['Cookie'].split('; ')
+            }
+
         if not self.parser.should_upgrade() and not int(self.request.headers.get('Content-Length', 0)):
             asyncio.get_event_loop().create_task(app._handle.http(self))
 
     def on_body(self, body: bytes):
         if self.request.body is None:
             self.request.body = b''
         self.request.body += body
```

### Comparing `cheeseapi-0.4.9/CheeseAPI/request.py` & `cheeseapi-1.0.0/CheeseAPI/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         self.method: http.HTTPMethod | Literal['WEBSOCKET'] = method
         self.origin: str | None = None
         self.client: str | None = None
 
         # Http
         self.body: list | dict | str | bytes | None = None
         self.form: Dict[str, str | File] | None = None
+        self.cookie: Dict[str, str] | None = None
 
         # Websocket
         self.subprotocols: List[str] | None = None
         self.subprotocol: str | None = None
 
         try:
             for pair in self.fullPath.split('?')[1].split('&'):
```

### Comparing `cheeseapi-0.4.9/CheeseAPI/response.py` & `cheeseapi-1.0.0/CheeseAPI/response.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import http, json, time
-from typing import Callable, Dict, AsyncIterator, Tuple, overload
+import http, json, time, datetime
+from typing import Callable, Dict, AsyncIterator, Tuple, overload, Literal
 from email.utils import formatdate
 
 from CheeseAPI.file import File
 
 contentTypes = {
     'tif': 'image/tiff',
     '001': 'application/x-001',
@@ -366,29 +366,60 @@
             if isinstance(self.body, AsyncIterator):
                 self._transfering = True
 
             self.headers['Data'] = formatdate(time.time(), usegmt = True)
 
             value = b'HTTP/1.1 ' + str(self.status).encode() + b' ' + http.HTTPStatus(self.status).phrase.encode() + b'\r\n'
             for key, _value in self.headers.items():
-                value += key.encode() + b': ' + str(_value).encode() + b'\r\n'
+                if key == 'Set-Cookies':
+                    for _, __value in _value.items():
+                        value += 'Set-Cookie: ' + __value
+                else:
+                    value += key.encode() + b': ' + str(_value).encode() + b'\r\n'
             value += b'\r\n'
 
             _value = None
             if isinstance(self.body, Callable):
                 _value = self.body().encode()
             elif isinstance(self.body, str):
                 _value = self.body.encode()
             elif isinstance(self.body, bytes):
                 _value += self.body
             if _value:
                 value += b'%x\r\n' % len(_value) + _value + b'\r\n0\r\n\r\n'
 
             return value, self._transfering
 
+    def setCookie(self, key: str, value: str, *, path: str = '/', secure: bool = False, httpOnly: bool = False, domain: str = '', sameSite: Literal['Strict', 'Lax', 'None'] = 'Lax', expires: datetime.datetime | str | None = None, maxAge: datetime.timedelta | int | None = None):
+        if 'Set-Cookies' not in self.headers:
+            self.headers['Set-Cookies'] = {}
+
+        s = f'{key}={value};'
+        if path:
+            s += f' Path={path};'
+        if sameSite == 'None' or secure:
+            s += ' Secure;'
+        if httpOnly:
+            s += ' HttpOnly;'
+        if domain:
+            s += f' Domain={domain};'
+        if sameSite != 'Lax':
+            s += f' SameSite={sameSite};'
+        if expires:
+            if isinstance(expires, str):
+                s += f' Expires={expires};'
+            elif isinstance(expires, datetime.datetime):
+                s += f' Expires={expires.strftime("%a, %d-%b-%Y %H:%M:%S GMT")};'
+        if maxAge:
+            if isinstance(maxAge, int):
+                s += f' Max-Age={maxAge};'
+            elif isinstance(maxAge, datetime.timedelta):
+                s += f' Max-Age={maxAge.total_seconds()};'
+        self.headers['Set-Cookies'][key] = s
+
 class Response(BaseResponse):
     def __init__(self, body: str | bytes | Callable | AsyncIterator | None = None, status: http.HTTPStatus | int = http.HTTPStatus.OK, headers: Dict[str, str] = {}):
         super().__init__(body, status, {
             'Content-Type': 'text/plain',
             **headers
         })
```

### Comparing `cheeseapi-0.4.9/CheeseAPI/route.py` & `cheeseapi-1.0.0/CheeseAPI/route.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.9/CheeseAPI/server.py` & `cheeseapi-1.0.0/CheeseAPI/server.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.9/CheeseAPI/signal.py` & `cheeseapi-1.0.0/CheeseAPI/signal.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.9/CheeseAPI/text.py` & `cheeseapi-1.0.0/CheeseAPI/text.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.9/CheeseAPI/websocket.py` & `cheeseapi-1.0.0/CheeseAPI/websocket.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.9/CheeseAPI/workspace.py` & `cheeseapi-1.0.0/CheeseAPI/workspace.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.9/LICENSE` & `cheeseapi-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.9/README.md` & `cheeseapi-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,36 @@
+Metadata-Version: 2.3
+Name: CheeseAPI
+Version: 1.0.0
+Summary: 一款web协程框架。
+Project-URL: Source, https://github.com/CheeseUnknown/CheeseAPI
+Author-email: Cheese Unknown <cheese@cheese.ren>
+License-File: LICENSE
+Keywords: API,BackEnd
+Requires-Dist: blinker
+Requires-Dist: cheeselog==1.0.*
+Requires-Dist: httptools
+Requires-Dist: ordered-set
+Requires-Dist: uvloop
+Requires-Dist: websockets
+Requires-Dist: xmltodict
+Description-Content-Type: text/markdown
+
 # **CheeseAPI**
 
 ## **介绍**
 
 一款协程友好的web框架，它具有以下功能：
 
 1. 插件支持，更可塑的事件处理以及个性化设置。
 
 2. 以模块为主的项目结构，以及灵活的模块导入方式。
 
 3. Websocket支持。
 
-暂时未添加的功能：
-
-1. ssl证书。
-
-2. http2协议支持。
-
-3. 部分不常用请求的处理方式可能有误。
-
-目前项目仍处于开发状态，有大部分功能尚不稳定或未提供，对于一些功能未来不能确保支持。
-
 ## **安装**
 
 系统要求：Linux。
 
 Python要求：目前仅保证支持3.11及以上版本的Python，新版本会优先支持Python的最新稳定版本。
 
 ```
```

### Comparing `cheeseapi-0.4.9/pyproject.toml` & `cheeseapi-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = [ "hatchling" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "CheeseAPI"
-version = "0.4.9"
+version = "1.0.0"
 description = "一款web协程框架。"
 readme = "README.md"
 license-files = { paths = [ "LICENSE" ] }
 authors = [
     { name = "Cheese Unknown", email = "cheese@cheese.ren" }
 ]
 keywords = [ 'API', 'BackEnd' ]
 
 dependencies = [
-    "CheeseLog",
+    "CheeseLog==1.0.*",
     "xmltodict",
     "blinker",
     "websockets",
     "uvloop",
     "httptools",
     "ordered_set"
 ]
```

### Comparing `cheeseapi-0.4.9/PKG-INFO` & `cheeseapi-1.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,19 @@
-Metadata-Version: 2.3
-Name: CheeseAPI
-Version: 0.4.9
-Summary: 一款web协程框架。
-Project-URL: Source, https://github.com/CheeseUnknown/CheeseAPI
-Author-email: Cheese Unknown <cheese@cheese.ren>
-License-File: LICENSE
-Keywords: API,BackEnd
-Requires-Dist: blinker
-Requires-Dist: cheeselog
-Requires-Dist: httptools
-Requires-Dist: ordered-set
-Requires-Dist: uvloop
-Requires-Dist: websockets
-Requires-Dist: xmltodict
-Description-Content-Type: text/markdown
-
 # **CheeseAPI**
 
 ## **介绍**
 
 一款协程友好的web框架，它具有以下功能：
 
 1. 插件支持，更可塑的事件处理以及个性化设置。
 
 2. 以模块为主的项目结构，以及灵活的模块导入方式。
 
 3. Websocket支持。
 
-暂时未添加的功能：
-
-1. ssl证书。
-
-2. http2协议支持。
-
-3. 部分不常用请求的处理方式可能有误。
-
-目前项目仍处于开发状态，有大部分功能尚不稳定或未提供，对于一些功能未来不能确保支持。
-
 ## **安装**
 
 系统要求：Linux。
 
 Python要求：目前仅保证支持3.11及以上版本的Python，新版本会优先支持Python的最新稳定版本。
 
 ```
```

