# Comparing `tmp/wptserve-4.0.1.tar.gz` & `tmp/wptserve-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wptserve-4.0.1.tar", last modified: Mon Nov  6 11:58:36 2023, max compression
+gzip compressed data, was "wptserve-4.0.2.tar", last modified: Wed Apr 17 14:53:22 2024, max compression
```

## Comparing `wptserve-4.0.1.tar` & `wptserve-4.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2023-11-06 11:58:36.835196 wptserve-4.0.1/
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)       17 2021-11-08 15:23:28.000000 wptserve-4.0.1/MANIFEST.in
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      574 2023-11-06 11:58:36.835196 wptserve-4.0.1/PKG-INFO
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      178 2021-11-08 15:23:28.000000 wptserve-4.0.1/README.md
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)       38 2023-11-06 11:58:36.835196 wptserve-4.0.1/setup.cfg
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1047 2023-11-06 11:58:22.000000 wptserve-4.0.1/setup.py
-drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2023-11-06 11:58:36.831196 wptserve-4.0.1/tests/
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)    11884 2023-07-24 09:32:19.000000 wptserve-4.0.1/tests/test_config.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1192 2023-05-04 08:42:57.000000 wptserve-4.0.1/tests/test_replacement_tokenizer.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     3194 2023-05-04 08:42:57.000000 wptserve-4.0.1/tests/test_request.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1016 2023-05-04 08:42:57.000000 wptserve-4.0.1/tests/test_response.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     4876 2023-05-04 08:42:57.000000 wptserve-4.0.1/tests/test_stash.py
-drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2023-11-06 11:58:36.831196 wptserve-4.0.1/wptserve/
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      158 2023-05-04 08:42:59.000000 wptserve-4.0.1/wptserve/__init__.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)    11340 2023-07-24 09:32:19.000000 wptserve-4.0.1/wptserve/config.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     4055 2023-05-04 08:42:58.000000 wptserve-4.0.1/wptserve/constants.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)    18729 2023-09-25 13:45:11.000000 wptserve-4.0.1/wptserve/handlers.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      109 2023-05-04 08:42:58.000000 wptserve-4.0.1/wptserve/logger.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)    18908 2023-07-24 09:32:19.000000 wptserve-4.0.1/wptserve/pipes.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     3166 2023-05-04 08:42:58.000000 wptserve-4.0.1/wptserve/ranges.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)    20731 2023-07-24 09:32:19.000000 wptserve-4.0.1/wptserve/request.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)    31447 2023-07-24 09:32:19.000000 wptserve-4.0.1/wptserve/response.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     6370 2023-05-04 08:42:58.000000 wptserve-4.0.1/wptserve/router.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      230 2023-05-04 08:42:58.000000 wptserve-4.0.1/wptserve/routes.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)    36045 2023-07-24 09:32:19.000000 wptserve-4.0.1/wptserve/server.py
-drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2023-11-06 11:58:36.835196 wptserve-4.0.1/wptserve/sslutils/
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      454 2023-05-04 08:42:58.000000 wptserve-4.0.1/wptserve/sslutils/__init__.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      352 2023-05-04 08:42:58.000000 wptserve-4.0.1/wptserve/sslutils/base.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)    14085 2023-05-04 08:42:58.000000 wptserve-4.0.1/wptserve/sslutils/openssl.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      904 2023-05-04 08:42:58.000000 wptserve-4.0.1/wptserve/sslutils/pregenerated.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     8176 2023-09-20 13:39:46.000000 wptserve-4.0.1/wptserve/stash.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     5884 2023-07-24 09:32:19.000000 wptserve-4.0.1/wptserve/utils.py
--rwxrwxr-x   0 jgraham   (1000) jgraham   (1000)     1160 2023-05-04 08:42:59.000000 wptserve-4.0.1/wptserve/wptserve.py
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     2458 2023-05-04 08:42:59.000000 wptserve-4.0.1/wptserve/ws_h2_handshake.py
-drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2023-11-06 11:58:36.835196 wptserve-4.0.1/wptserve.egg-info/
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      574 2023-11-06 11:58:36.000000 wptserve-4.0.1/wptserve.egg-info/PKG-INFO
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      783 2023-11-06 11:58:36.000000 wptserve-4.0.1/wptserve.egg-info/SOURCES.txt
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)        1 2023-11-06 11:58:36.000000 wptserve-4.0.1/wptserve.egg-info/dependency_links.txt
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)        1 2023-11-03 09:43:02.000000 wptserve-4.0.1/wptserve.egg-info/not-zip-safe
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      201 2023-11-06 11:58:36.000000 wptserve-4.0.1/wptserve.egg-info/requires.txt
--rw-rw-r--   0 jgraham   (1000) jgraham   (1000)        9 2023-11-06 11:58:36.000000 wptserve-4.0.1/wptserve.egg-info/top_level.txt
+drwxr-xr-x   0 henrik     (501) staff       (20)        0 2024-04-17 14:53:22.138470 wptserve-4.0.2/
+-rw-r--r--   0 henrik     (501) staff       (20)       17 2023-08-22 18:34:29.000000 wptserve-4.0.2/MANIFEST.in
+-rw-r--r--   0 henrik     (501) staff       (20)      634 2024-04-17 14:53:22.138170 wptserve-4.0.2/PKG-INFO
+-rw-r--r--   0 henrik     (501) staff       (20)      178 2023-08-22 18:34:29.000000 wptserve-4.0.2/README.md
+-rw-r--r--   0 henrik     (501) staff       (20)       38 2024-04-17 14:53:22.138529 wptserve-4.0.2/setup.cfg
+-rw-r--r--   0 henrik     (501) staff       (20)      867 2024-04-17 14:45:14.000000 wptserve-4.0.2/setup.py
+drwxr-xr-x   0 henrik     (501) staff       (20)        0 2024-04-17 14:53:22.131250 wptserve-4.0.2/tests/
+-rw-r--r--   0 henrik     (501) staff       (20)    11884 2023-08-31 08:41:42.000000 wptserve-4.0.2/tests/test_config.py
+-rw-r--r--   0 henrik     (501) staff       (20)     1192 2023-08-22 18:34:29.000000 wptserve-4.0.2/tests/test_replacement_tokenizer.py
+-rw-r--r--   0 henrik     (501) staff       (20)     3194 2023-08-22 18:34:56.000000 wptserve-4.0.2/tests/test_request.py
+-rw-r--r--   0 henrik     (501) staff       (20)     1016 2023-08-22 18:34:56.000000 wptserve-4.0.2/tests/test_response.py
+-rw-r--r--   0 henrik     (501) staff       (20)     4876 2023-08-22 18:34:29.000000 wptserve-4.0.2/tests/test_stash.py
+drwxr-xr-x   0 henrik     (501) staff       (20)        0 2024-04-17 14:53:22.133961 wptserve-4.0.2/wptserve/
+-rw-r--r--   0 henrik     (501) staff       (20)      158 2023-08-22 18:34:29.000000 wptserve-4.0.2/wptserve/__init__.py
+-rw-r--r--   0 henrik     (501) staff       (20)    11340 2023-08-31 08:41:42.000000 wptserve-4.0.2/wptserve/config.py
+-rw-r--r--   0 henrik     (501) staff       (20)     4022 2024-04-16 11:51:30.000000 wptserve-4.0.2/wptserve/constants.py
+-rw-r--r--   0 henrik     (501) staff       (20)    19390 2024-03-26 06:53:25.000000 wptserve-4.0.2/wptserve/handlers.py
+-rw-r--r--   0 henrik     (501) staff       (20)      109 2023-08-22 18:34:56.000000 wptserve-4.0.2/wptserve/logger.py
+-rw-r--r--   0 henrik     (501) staff       (20)    18908 2023-08-31 08:41:42.000000 wptserve-4.0.2/wptserve/pipes.py
+-rw-r--r--   0 henrik     (501) staff       (20)     3166 2023-08-22 18:34:56.000000 wptserve-4.0.2/wptserve/ranges.py
+-rw-r--r--   0 henrik     (501) staff       (20)    20731 2023-08-31 08:41:42.000000 wptserve-4.0.2/wptserve/request.py
+-rw-r--r--   0 henrik     (501) staff       (20)    31447 2023-08-31 08:41:42.000000 wptserve-4.0.2/wptserve/response.py
+-rw-r--r--   0 henrik     (501) staff       (20)     6370 2023-08-22 18:34:56.000000 wptserve-4.0.2/wptserve/router.py
+-rw-r--r--   0 henrik     (501) staff       (20)      230 2023-08-22 18:34:29.000000 wptserve-4.0.2/wptserve/routes.py
+-rw-r--r--   0 henrik     (501) staff       (20)    36896 2024-04-16 14:31:02.000000 wptserve-4.0.2/wptserve/server.py
+drwxr-xr-x   0 henrik     (501) staff       (20)        0 2024-04-17 14:53:22.137632 wptserve-4.0.2/wptserve/sslutils/
+-rw-r--r--   0 henrik     (501) staff       (20)      454 2023-08-22 18:34:56.000000 wptserve-4.0.2/wptserve/sslutils/__init__.py
+-rw-r--r--   0 henrik     (501) staff       (20)      352 2023-08-22 18:34:56.000000 wptserve-4.0.2/wptserve/sslutils/base.py
+-rw-r--r--   0 henrik     (501) staff       (20)    14085 2023-08-22 18:34:56.000000 wptserve-4.0.2/wptserve/sslutils/openssl.py
+-rw-r--r--   0 henrik     (501) staff       (20)      904 2023-08-22 18:34:56.000000 wptserve-4.0.2/wptserve/sslutils/pregenerated.py
+-rw-r--r--   0 henrik     (501) staff       (20)     8176 2023-08-31 08:41:42.000000 wptserve-4.0.2/wptserve/stash.py
+-rw-r--r--   0 henrik     (501) staff       (20)     5930 2024-04-03 10:57:32.000000 wptserve-4.0.2/wptserve/utils.py
+-rwxr-xr-x   0 henrik     (501) staff       (20)     1160 2023-08-22 18:34:56.000000 wptserve-4.0.2/wptserve/wptserve.py
+-rw-r--r--   0 henrik     (501) staff       (20)     2443 2024-04-16 14:31:02.000000 wptserve-4.0.2/wptserve/ws_h2_handshake.py
+drwxr-xr-x   0 henrik     (501) staff       (20)        0 2024-04-17 14:53:22.137879 wptserve-4.0.2/wptserve.egg-info/
+-rw-r--r--   0 henrik     (501) staff       (20)      634 2024-04-17 14:53:22.000000 wptserve-4.0.2/wptserve.egg-info/PKG-INFO
+-rw-r--r--   0 henrik     (501) staff       (20)      783 2024-04-17 14:53:22.000000 wptserve-4.0.2/wptserve.egg-info/SOURCES.txt
+-rw-r--r--   0 henrik     (501) staff       (20)        1 2024-04-17 14:53:22.000000 wptserve-4.0.2/wptserve.egg-info/dependency_links.txt
+-rw-r--r--   0 henrik     (501) staff       (20)        1 2023-11-01 14:11:54.000000 wptserve-4.0.2/wptserve.egg-info/not-zip-safe
+-rw-r--r--   0 henrik     (501) staff       (20)       30 2024-04-17 14:53:22.000000 wptserve-4.0.2/wptserve.egg-info/requires.txt
+-rw-r--r--   0 henrik     (501) staff       (20)        9 2024-04-17 14:53:22.000000 wptserve-4.0.2/wptserve.egg-info/top_level.txt
```

### Comparing `wptserve-4.0.1/setup.py` & `wptserve-4.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
-PACKAGE_VERSION = '4.0.1'
+PACKAGE_VERSION = '4.0.2'
 deps = [
     "h2>=4.1.0",
-    "mod_pywebsocket @ https://github.com/GoogleChromeLabs/pywebsocket3/archive/50602a14f1b6da17e0b619833a13addc6ea78bc2.zip#sha256=4dadd116e67af5625606f883e1973178d4121e8a1dc87b096ba2bb43c692f958",  # noqa
+    "pywebsocket3>=4.0.2",
 ]
 
 setup(name='wptserve',
       version=PACKAGE_VERSION,
       description="Python web server intended for in web browser testing",
       long_description=open("README.md").read(),
       # Get strings from http://pypi.python.org/pypi?%3Aaction=list_classifiers
```

### Comparing `wptserve-4.0.1/tests/test_config.py` & `wptserve-4.0.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `wptserve-4.0.1/tests/test_replacement_tokenizer.py` & `wptserve-4.0.2/tests/test_replacement_tokenizer.py`

 * *Files identical despite different names*

### Comparing `wptserve-4.0.1/tests/test_request.py` & `wptserve-4.0.2/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `wptserve-4.0.1/tests/test_response.py` & `wptserve-4.0.2/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `wptserve-4.0.1/tests/test_stash.py` & `wptserve-4.0.2/tests/test_stash.py`

 * *Files identical despite different names*

### Comparing `wptserve-4.0.1/wptserve/config.py` & `wptserve-4.0.2/wptserve/config.py`

 * *Files identical despite different names*

### Comparing `wptserve-4.0.1/wptserve/constants.py` & `wptserve-4.0.2/wptserve/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     "text/css": ["css"],
     "text/event-stream": ["event_stream"],
     "text/html": ["htm", "html"],
     "text/javascript": ["js", "mjs"],
     "text/plain": ["txt", "md"],
     "text/vtt": ["vtt"],
     "video/mp4": ["mp4", "m4v"],
-    "video/ogg": ["ogg", "ogv"],
     "video/webm": ["webm"],
 })
 
 response_codes = {
     100: ('Continue', 'Request received, please continue'),
     101: ('Switching Protocols',
           'Switching to new protocol; obey Upgrade header'),
```

### Comparing `wptserve-4.0.1/wptserve/handlers.py` & `wptserve-4.0.2/wptserve/handlers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # mypy: allow-untyped-defs
 
 import json
 import os
+import pathlib
 from collections import defaultdict
 
 from urllib.parse import quote, unquote, urljoin
 
 from .constants import content_types
 from .pipes import Pipeline, template
 from .ranges import RangeParser
@@ -285,23 +286,35 @@
     def __repr__(self):
         return "<%s base_path:%s url_base:%s>" % (self.__class__.__name__, self.base_path, self.url_base)
 
     def _load_file(self, request, response, func):
         """
         This loads the requested python file as an environ variable.
 
+        If the requested file is a directory, this instead loads the first
+        lexicographically sorted file found in that directory that matches
+        "default*.py".
+
         Once the environ is loaded, the passed `func` is run with this loaded environ.
 
         :param request: The request object
         :param response: The response object
         :param func: The function to be run with the loaded environ with the modified filepath. Signature: (request, response, environ, path)
         :return: The return of func
         """
         path = filesystem_path(self.base_path, request, self.url_base)
 
+        # Find a default Python file if the specified path is a directory
+        if os.path.isdir(path):
+            default_py_files = sorted(list(filter(
+                pathlib.Path.is_file,
+                pathlib.Path(path).glob("default*.py"))))
+            if default_py_files:
+                path = str(default_py_files[0])
+
         try:
             environ = {"__file__": path}
             with open(path, 'rb') as f:
                 exec(compile(f.read(), path, 'exec'), environ, environ)
 
             if func is not None:
                 return func(request, response, environ, path)
@@ -412,14 +425,17 @@
 class AsIsHandler:
     def __init__(self, base_path=None, url_base="/"):
         self.base_path = base_path
         self.url_base = url_base
 
     def __call__(self, request, response):
         path = filesystem_path(self.base_path, request, self.url_base)
+        if os.path.isdir(path):
+            raise HTTPException(
+                500, "AsIsHandler cannot process directory, %s" % path)
 
         try:
             with open(path, 'rb') as f:
                 response.writer.write_raw_content(f.read())
             wrap_pipeline(path, request, response)
             response.close_connection = True
         except OSError:
```

### Comparing `wptserve-4.0.1/wptserve/pipes.py` & `wptserve-4.0.2/wptserve/pipes.py`

 * *Files identical despite different names*

### Comparing `wptserve-4.0.1/wptserve/ranges.py` & `wptserve-4.0.2/wptserve/ranges.py`

 * *Files identical despite different names*

### Comparing `wptserve-4.0.1/wptserve/request.py` & `wptserve-4.0.2/wptserve/request.py`

 * *Files identical despite different names*

### Comparing `wptserve-4.0.1/wptserve/response.py` & `wptserve-4.0.2/wptserve/response.py`

 * *Files identical despite different names*

### Comparing `wptserve-4.0.1/wptserve/router.py` & `wptserve-4.0.2/wptserve/router.py`

 * *Files identical despite different names*

### Comparing `wptserve-4.0.1/wptserve/server.py` & `wptserve-4.0.2/wptserve/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 from h2.events import RequestReceived, ConnectionTerminated, DataReceived, StreamReset, StreamEnded
 from h2.exceptions import StreamClosedError, ProtocolError
 from h2.settings import SettingCodes
 from h2.utilities import extract_method_header
 
 from urllib.parse import urlsplit, urlunsplit
 
-from mod_pywebsocket import dispatch
-from mod_pywebsocket.handshake import HandshakeException, AbortedByUserException
+from pywebsocket3 import dispatch
+from pywebsocket3.handshake import HandshakeException, AbortedByUserException
 
 from . import routes as default_routes
 from .config import ConfigBuilder
 from .logger import get_logger
 from .request import Server, Request, H2Request
 from .response import Response, H2Response
 from .router import Router
@@ -126,15 +126,17 @@
                 new_url[2] = destination
                 new_url = urlunsplit(new_url)
                 request_handler.path = new_url
 
 
 class WebTestServer(http.server.ThreadingHTTPServer):
     allow_reuse_address = True
-    acceptable_errors = (errno.EPIPE, errno.ECONNABORTED)
+    # Older versions of Python might throw `OSError: [Errno 0] Error`
+    # instead of `SSLEOFError`.
+    acceptable_errors = (errno.EPIPE, errno.ECONNABORTED, 0)
     request_queue_size = 2000
 
     # Ensure that we don't hang on shutdown waiting for requests
     daemon_threads = True
 
     def __init__(self, server_address, request_handler_cls,
                  router, rewriter, bind_address, ws_doc_root=None,
@@ -210,30 +212,41 @@
 
         if use_ssl and not encrypt_after_connect:
             if http2:
                 ssl_context = ssl.create_default_context(purpose=ssl.Purpose.CLIENT_AUTH)
                 ssl_context.load_cert_chain(keyfile=self.key_file, certfile=self.certificate)
                 ssl_context.set_alpn_protocols(['h2'])
                 self.socket = ssl_context.wrap_socket(self.socket,
+                                                      do_handshake_on_connect=False,
                                                       server_side=True)
 
             else:
-                self.socket = ssl.wrap_socket(self.socket,
-                                              keyfile=self.key_file,
-                                              certfile=self.certificate,
-                                              server_side=True)
+                ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
+                ssl_context.load_cert_chain(keyfile=self.key_file, certfile=self.certificate)
+                self.socket = ssl_context.wrap_socket(self.socket,
+                                                      do_handshake_on_connect=False,
+                                                      server_side=True)
+
+    def finish_request(self, request, client_address):
+        if isinstance(self.socket, ssl.SSLSocket):
+            request.do_handshake()
+        super().finish_request(request, client_address)
 
     def handle_error(self, request, client_address):
         error = sys.exc_info()[1]
 
         if ((isinstance(error, OSError) and
              isinstance(error.args, tuple) and
              error.args[0] in self.acceptable_errors) or
             (isinstance(error, IOError) and
-             error.errno in self.acceptable_errors)):
+             error.errno in self.acceptable_errors) or
+            # `SSLEOFError` and `SSLError` may occur when a client
+            # (e.g., wptrunner's `TestEnvironment`) tests for connectivity
+            # but doesn't perform the handshake.
+            isinstance(error, ssl.SSLEOFError) or isinstance(error, ssl.SSLError)):
             pass  # remote hang up before the result is sent
         else:
             msg = traceback.format_exc()
             self.logger.error(f"{type(error)} {error}")
             self.logger.info(msg)
 
 
@@ -318,18 +331,18 @@
 
     def handle_connect(self, response):
         self.logger.debug("Got CONNECT")
         response.status = 200
         response.write()
         if self.server.encrypt_after_connect:
             self.logger.debug("Enabling SSL for connection")
-            self.request = ssl.wrap_socket(self.connection,
-                                           keyfile=self.server.key_file,
-                                           certfile=self.server.certificate,
-                                           server_side=True)
+            ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
+            ssl_context.load_cert_chain(keyfile=self.server.key_file, certfile=self.server.certificate)
+            self.request = ssl_context.wrap_socket(self.connection,
+                                                   server_side=True)
             self.setup()
         return
 
 
 class Http2WebTestRequestHandler(BaseWebTestRequestHandler):
     protocol_version = "HTTP/2.0"
 
@@ -530,27 +543,27 @@
 
         t.join()
 
     def _stream_ws_sub_thread(self, request, stream_handler, queue):
         dispatcher = request._dispatcher
         try:
             dispatcher.transfer_data(request)
-        except StreamClosedError:
+        except (StreamClosedError, ProtocolError):
             # work around https://github.com/web-platform-tests/wpt/issues/27786
             # The stream was already closed.
             queue.put(None)
             return
 
         stream_id = stream_handler.h2_stream_id
         with stream_handler.conn as connection:
             try:
                 connection.end_stream(stream_id)
                 data = connection.data_to_send()
                 stream_handler.request.sendall(data)
-            except StreamClosedError:  # maybe the stream has already been closed
+            except (StreamClosedError, ProtocolError):  # maybe the stream has already been closed
                 pass
         queue.put(None)
 
     def _stream_thread(self, stream_id, queue):
         """
         This thread processes frames for a specific stream. It waits for frames to be placed
         in the queue, and processes them. When it receives a request frame, it will start processing
```

### Comparing `wptserve-4.0.1/wptserve/sslutils/openssl.py` & `wptserve-4.0.2/wptserve/sslutils/openssl.py`

 * *Files identical despite different names*

### Comparing `wptserve-4.0.1/wptserve/sslutils/pregenerated.py` & `wptserve-4.0.2/wptserve/sslutils/pregenerated.py`

 * *Files identical despite different names*

### Comparing `wptserve-4.0.1/wptserve/stash.py` & `wptserve-4.0.2/wptserve/stash.py`

 * *Files identical despite different names*

### Comparing `wptserve-4.0.1/wptserve/utils.py` & `wptserve-4.0.2/wptserve/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,23 +137,25 @@
         995,   # pop3+ssl
         1719,  # h323gatestat
         1720,  # h323hostcall
         1723,  # pptp
         2049,  # nfs
         3659,  # apple-sasl
         4045,  # lockd
+        4190,  # sieve
         5060,  # sip
         5061,  # sips
         6000,  # x11
         6566,  # sane-port
         6665,  # irc (alternate)
         6666,  # irc (alternate)
         6667,  # irc (default)
         6668,  # irc (alternate)
         6669,  # irc (alternate)
+        6679,  # osaut
         6697,  # irc+tls
         10080,  # amanda
     ]
 
 
 def get_port(host: str = '') -> int:
     host = host or '127.0.0.1'
```

### Comparing `wptserve-4.0.1/wptserve/wptserve.py` & `wptserve-4.0.2/wptserve/wptserve.py`

 * *Files identical despite different names*

### Comparing `wptserve-4.0.1/wptserve/ws_h2_handshake.py` & `wptserve-4.0.2/wptserve/ws_h2_handshake.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 """This file provides the opening handshake processor for the Bootstrapping
 WebSockets with HTTP/2 protocol (RFC 8441).
 
 Specification:
 https://tools.ietf.org/html/rfc8441
 """
 
-from mod_pywebsocket import common
+from pywebsocket3 import common
 
-from mod_pywebsocket.handshake.base import get_mandatory_header
-from mod_pywebsocket.handshake.base import HandshakeException
-from mod_pywebsocket.handshake.base import validate_mandatory_header
-from mod_pywebsocket.handshake.base import HandshakerBase
+from pywebsocket3.handshake.base import get_mandatory_header
+from pywebsocket3.handshake.base import HandshakeException
+from pywebsocket3.handshake.base import validate_mandatory_header
+from pywebsocket3.handshake.base import HandshakerBase
 
 
 def check_connect_method(request):
     if request.method != 'CONNECT':
         raise HandshakeException('Method is not CONNECT: %r' % request.method)
```

### Comparing `wptserve-4.0.1/wptserve.egg-info/SOURCES.txt` & `wptserve-4.0.2/wptserve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

