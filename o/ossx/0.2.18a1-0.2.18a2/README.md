# Comparing `tmp/ossx-0.2.18a1.tar.gz` & `tmp/ossx-0.2.18a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ossx-0.2.18a1.tar", max compression
+gzip compressed data, was "ossx-0.2.18a2.tar", max compression
```

## Comparing `ossx-0.2.18a1.tar` & `ossx-0.2.18a2.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0      245 2024-04-14 08:24:39.302328 ossx-0.2.18a1/README.md
--rw-r--r--   0        0        0      113 2024-04-14 08:32:03.266569 ossx-0.2.18a1/ossx/__init__.py
--rw-r--r--   0        0        0     6722 2024-04-14 08:09:27.832781 ossx-0.2.18a1/ossx/_http.py
--rw-r--r--   0        0        0     8908 2024-04-14 08:12:24.336508 ossx-0.2.18a1/ossx/bucket.py
--rw-r--r--   0        0        0      193 2024-04-14 07:13:38.904632 ossx-0.2.18a1/ossx/patch.py
--rw-r--r--   0        0        0     5048 2024-04-14 07:57:45.765087 ossx-0.2.18a1/ossx/utils.py
--rw-r--r--   0        0        0      495 2024-04-14 08:32:03.264943 ossx-0.2.18a1/pyproject.toml
--rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 ossx-0.2.18a1/PKG-INFO
+-rw-r--r--   0        0        0     1991 2024-04-16 12:23:46.786185 ossx-0.2.18a2/README.md
+-rw-r--r--   0        0        0      143 2024-04-16 12:24:08.359535 ossx-0.2.18a2/ossx/__init__.py
+-rw-r--r--   0        0        0     7034 2024-04-17 06:05:55.724656 ossx-0.2.18a2/ossx/_http.py
+-rw-r--r--   0        0        0    33002 2024-04-17 06:05:55.724889 ossx-0.2.18a2/ossx/bucket.py
+-rw-r--r--   0        0        0     1439 2024-04-17 06:05:55.725027 ossx-0.2.18a2/ossx/models.py
+-rw-r--r--   0        0        0      315 2024-04-17 06:05:55.725168 ossx-0.2.18a2/ossx/patch.py
+-rw-r--r--   0        0        0     9835 2024-04-17 06:05:55.725340 ossx-0.2.18a2/ossx/select_response.py
+-rw-r--r--   0        0        0     5962 2024-04-17 06:05:55.725783 ossx-0.2.18a2/ossx/utils.py
+-rw-r--r--   0        0        0      495 2024-04-16 12:23:21.749178 ossx-0.2.18a2/pyproject.toml
+-rw-r--r--   0        0        0     2524 1970-01-01 00:00:00.000000 ossx-0.2.18a2/PKG-INFO
```

### Comparing `ossx-0.2.18a1/ossx/_http.py` & `ossx-0.2.18a2/ossx/_http.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,25 +17,26 @@
 
 class Session:
     def __init__(
         self,
         pool_size: Optional[int] = None,
         adapter: Optional[AsyncBaseTransport] = None,
         timeout: float = defaults.connect_timeout,
+        proxies: Optional[dict] = None,
     ):
         psize = pool_size or defaults.connection_pool_size
         limits = httpx.Limits(max_connections=psize, max_keepalive_connections=psize)
         if adapter is None:
             adapter = httpx.AsyncHTTPTransport(limits=limits)
         mounts = {"http://": adapter, "https://": adapter}
-        self.session = httpx.AsyncClient(mounts=mounts, timeout=timeout)
+        self.session = httpx.AsyncClient(mounts=mounts, timeout=timeout, proxies=proxies)
 
     def do_request(self, req: "Request", timeout: float):
         try:
-            # TODO fix proxy
+
             logger.debug(
                 "Send request, method: {0}, url: {1}, params: {2}, headers: {3}, timeout: {4}".format(
                     req.method, req.url, req.params, req.headers, timeout
                 )
             )
             request = self.session.build_request(
                 method=req.method,
@@ -78,14 +79,18 @@
         self.cloudbox_id = cloudbox_id
 
         if not isinstance(headers, httpx.Headers):
             self.headers = httpx.Headers(headers)
         else:
             self.headers = headers
 
+        # not to add 'Accept-Encoding: gzip, deflate' by default
+        if "Accept-Encoding" not in self.headers:
+            self.headers["Accept-Encoding"] = "identity"
+
         if "User-Agent" not in self.headers:
             if app_name:
                 self.headers["User-Agent"] = USER_AGENT + "/" + app_name
             else:
                 self.headers["User-Agent"] = USER_AGENT
 
         logger.debug(
@@ -106,14 +111,17 @@
         self.headers = {}
         self.request_id = ""
 
         self.__all_read = False
         self.__iter = None
         self.chunker = io.BytesIO()
 
+    def __iter__(self):
+        return self
+
     def __await__(self):
         return self._await().__await__()
 
     async def _await(self):
         if self.response is not None:
             return self
 
@@ -161,14 +169,17 @@
 
             chunk = self.chunker.getvalue()[:amt]
             self.chunker = io.BytesIO(self.chunker.getvalue()[amt:])
             if len(self.chunker.getbuffer()) == 0:
                 self.__all_read = True
             return chunk
 
+    async def close(self):
+        await self.response.aclose()
+
     @property
     def _iter(self):
         if self.__iter is None:
             self.__iter = self.__aiter__()
         return self.__iter
 
     def __aiter__(self) -> AsyncIterator[bytes]:
```

### Comparing `ossx-0.2.18a1/ossx/utils.py` & `ossx-0.2.18a2/ossx/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from inspect import iscoroutinefunction
+from inspect import isawaitable, iscoroutinefunction
+from io import BytesIO
+from typing import IO, AsyncIterable, Union
 
 from oss2.utils import (
     _CHUNK_SIZE,
     ClientError,
     Crc64,
     _BytesAndFileAdapter,
     _FileLikeAdapter,
     _get_data_size,
     _has_data_size_attr,
     _invoke_cipher_callback,
     _invoke_crc_callback,
-    _invoke_progress_callback,
     _IterableAdapter,
     to_bytes,
 )
 
 
 def make_crc_adapter(data, init_crc=0, discard=0):
     """返回一个适配器，从而在读取 `data` ，即调用read或者对其进行迭代的时候，能够计算CRC。
@@ -22,23 +23,28 @@
     :param discard:
     :return:
     :param data: 可以是bytes、file object或iterable
     :param init_crc: 初始CRC值，可选
 
     :return: 能够调用计算CRC函数的适配器
     """
+    if isinstance(data, AwaitReadAdapter):
+        data.crc_callback = Crc64(init_crc)
+        data.discard = discard
+        return data
+
     data = to_bytes(data)
 
     # bytes or file object
     if _has_data_size_attr(data):
         if discard:
             raise ClientError("Bytes of file object adapter does not support discard bytes")
         return _BytesAndFileAdapter(data, size=_get_data_size(data), crc_callback=Crc64(init_crc))
     elif hasattr(data, "read") and iscoroutinefunction(data.read):
-        return _AwaitReadAdapter(data, crc_callback=Crc64(init_crc), discard=discard)
+        return AwaitReadAdapter(data, crc_callback=Crc64(init_crc), discard=discard)
     # file-like object
     elif hasattr(data, "read"):
         return _FileLikeAdapter(data, crc_callback=Crc64(init_crc), discard=discard)
     # iterator
     elif hasattr(data, "__iter__"):
         if discard:
             raise ClientError("Iterator adapter does not support discard bytes")
@@ -55,50 +61,70 @@
 
     :param data: 可以是bytes、file object或iterable
     :param progress_callback: 进度回调函数，参见 :ref:`progress_callback`
     :param size: 指定 `data` 的大小，可选
 
     :return: 能够调用进度回调函数的适配器
     """
+    if isinstance(data, AwaitReadAdapter):
+        data.progress_callback = progress_callback
+        return data
+
     data = to_bytes(data)
 
     if size is None:
         size = _get_data_size(data)
 
     if size is None:
         if hasattr(data, "read") and iscoroutinefunction(data.read):
-            return _AwaitReadAdapter(data, progress_callback)
+            return AwaitReadAdapter(data, progress_callback)
         if hasattr(data, "read"):
             return _FileLikeAdapter(data, progress_callback)
         elif hasattr(data, "__iter__"):
             return _IterableAdapter(data, progress_callback)
         else:
             raise ClientError(
                 "{0} is not a file object, nor an iterator".format(data.__class__.__name__)
             )
     else:
         return _BytesAndFileAdapter(data, progress_callback, size)
 
 
-class _AwaitReadAdapter(object):
+def warp_async_data(data: Union[str, bytes, IO, AsyncIterable]):
+    if isinstance(data, bytes):
+        data = BytesIO(data)
+    elif isinstance(data, str):
+        data = BytesIO(data.encode("utf-8"))
+    return AwaitReadAdapter(data)
+
+
+async def _invoke_progress_callback(progress_callback, consumed_bytes, total_bytes):
+    if progress_callback:
+        if iscoroutinefunction(progress_callback):
+            await progress_callback(consumed_bytes, total_bytes)
+        else:
+            progress_callback(consumed_bytes, total_bytes)
+
+
+class AwaitReadAdapter(object):
     """通过这个适配器，可以给AwaitResponse加上进度监控。
 
-    :param resp: file-like object，只要支持async read即可
+    :param f: file-like object，只要支持async read / read即可
     :param progress_callback: 进度回调函数
     """
 
     def __init__(
         self,
-        resp,
+        f,
         progress_callback=None,
         crc_callback=None,
         cipher_callback=None,
         discard=0,
     ):
-        self.fileobj = resp
+        self.fileobj = f
         self.progress_callback = progress_callback
         self.offset = 0
 
         self.crc_callback = crc_callback
         self.cipher_callback = cipher_callback
         self.discard = discard
         self.read_all = False
@@ -121,20 +147,22 @@
             raise StopAsyncIteration
 
     async def read(self, amt=None):
         offset_start = self.offset
         if offset_start < self.discard and amt and self.cipher_callback:
             amt += self.discard
 
-        content = await self.fileobj.read(amt)
+        content = self.fileobj.read(amt)
+        if isawaitable(content):
+            content = await content
         if not content:
             self.read_all = True
-            _invoke_progress_callback(self.progress_callback, self.offset, None)
+            await _invoke_progress_callback(self.progress_callback, self.offset, None)
         else:
-            _invoke_progress_callback(self.progress_callback, self.offset, None)
+            await _invoke_progress_callback(self.progress_callback, self.offset, None)
 
             self.offset += len(content)
 
             real_discard = 0
             if offset_start < self.discard:
                 if len(content) <= self.discard:
                     real_discard = len(content)
```

