# Comparing `tmp/moesif_aiohttp-1.0.1.tar.gz` & `tmp/moesif_aiohttp-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moesif_aiohttp-1.0.1.tar", last modified: Mon Apr  8 23:46:35 2024, max compression
+gzip compressed data, was "moesif_aiohttp-1.1.0.tar", last modified: Wed Apr 17 04:27:01 2024, max compression
```

## Comparing `moesif_aiohttp-1.0.1.tar` & `moesif_aiohttp-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-04-08 23:46:35.889846 moesif_aiohttp-1.0.1/
--rw-r--r--   0 keyur      (501) staff       (20)    11908 2024-04-05 20:04:31.000000 moesif_aiohttp-1.0.1/LICENSE
--rw-r--r--   0 keyur      (501) staff       (20)       61 2024-04-05 20:05:42.000000 moesif_aiohttp-1.0.1/MANIFEST.in
--rw-r--r--   0 keyur      (501) staff       (20)    12975 2024-04-08 23:46:35.889975 moesif_aiohttp-1.0.1/PKG-INFO
--rw-r--r--   0 keyur      (501) staff       (20)    11910 2024-04-05 23:45:16.000000 moesif_aiohttp-1.0.1/README.md
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-04-08 23:46:35.887184 moesif_aiohttp-1.0.1/moesif_aiohttp/
--rw-r--r--   0 keyur      (501) staff       (20)       26 2024-04-06 01:32:25.000000 moesif_aiohttp-1.0.1/moesif_aiohttp/__init__.py
--rw-r--r--   0 keyur      (501) staff       (20)     2887 2024-04-05 18:44:49.000000 moesif_aiohttp-1.0.1/moesif_aiohttp/event_mapper.py
--rw-r--r--   0 keyur      (501) staff       (20)     7723 2024-04-06 01:33:17.000000 moesif_aiohttp-1.0.1/moesif_aiohttp/logger_helper.py
--rw-r--r--   0 keyur      (501) staff       (20)     8299 2024-04-08 21:31:37.000000 moesif_aiohttp-1.0.1/moesif_aiohttp/middleware.py
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-04-08 23:46:35.889571 moesif_aiohttp-1.0.1/moesif_aiohttp.egg-info/
--rw-r--r--   0 keyur      (501) staff       (20)    12975 2024-04-08 23:46:35.000000 moesif_aiohttp-1.0.1/moesif_aiohttp.egg-info/PKG-INFO
--rw-r--r--   0 keyur      (501) staff       (20)      356 2024-04-08 23:46:35.000000 moesif_aiohttp-1.0.1/moesif_aiohttp.egg-info/SOURCES.txt
--rw-r--r--   0 keyur      (501) staff       (20)        1 2024-04-08 23:46:35.000000 moesif_aiohttp-1.0.1/moesif_aiohttp.egg-info/dependency_links.txt
--rw-r--r--   0 keyur      (501) staff       (20)      154 2024-04-08 23:46:35.000000 moesif_aiohttp-1.0.1/moesif_aiohttp.egg-info/requires.txt
--rw-r--r--   0 keyur      (501) staff       (20)       15 2024-04-08 23:46:35.000000 moesif_aiohttp-1.0.1/moesif_aiohttp.egg-info/top_level.txt
--rw-r--r--   0 keyur      (501) staff       (20)       67 2024-04-08 23:46:35.890778 moesif_aiohttp-1.0.1/setup.cfg
--rw-r--r--   0 keyur      (501) staff       (20)     3273 2024-04-08 23:44:28.000000 moesif_aiohttp-1.0.1/setup.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-04-17 04:27:01.480150 moesif_aiohttp-1.1.0/
+-rw-r--r--   0 keyur      (501) staff       (20)    11908 2024-04-05 20:04:31.000000 moesif_aiohttp-1.1.0/LICENSE
+-rw-r--r--   0 keyur      (501) staff       (20)       61 2024-04-05 20:05:42.000000 moesif_aiohttp-1.1.0/MANIFEST.in
+-rw-r--r--   0 keyur      (501) staff       (20)    12975 2024-04-17 04:27:01.480376 moesif_aiohttp-1.1.0/PKG-INFO
+-rw-r--r--   0 keyur      (501) staff       (20)    11910 2024-04-05 23:45:16.000000 moesif_aiohttp-1.1.0/README.md
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-04-17 04:27:01.477132 moesif_aiohttp-1.1.0/moesif_aiohttp/
+-rw-r--r--   0 keyur      (501) staff       (20)       26 2024-04-06 01:32:25.000000 moesif_aiohttp-1.1.0/moesif_aiohttp/__init__.py
+-rw-r--r--   0 keyur      (501) staff       (20)     3282 2024-04-17 04:25:54.000000 moesif_aiohttp-1.1.0/moesif_aiohttp/event_mapper.py
+-rw-r--r--   0 keyur      (501) staff       (20)     7723 2024-04-06 01:33:17.000000 moesif_aiohttp-1.1.0/moesif_aiohttp/logger_helper.py
+-rw-r--r--   0 keyur      (501) staff       (20)    10291 2024-04-17 04:25:54.000000 moesif_aiohttp-1.1.0/moesif_aiohttp/middleware.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-04-17 04:27:01.479735 moesif_aiohttp-1.1.0/moesif_aiohttp.egg-info/
+-rw-r--r--   0 keyur      (501) staff       (20)    12975 2024-04-17 04:27:01.000000 moesif_aiohttp-1.1.0/moesif_aiohttp.egg-info/PKG-INFO
+-rw-r--r--   0 keyur      (501) staff       (20)      356 2024-04-17 04:27:01.000000 moesif_aiohttp-1.1.0/moesif_aiohttp.egg-info/SOURCES.txt
+-rw-r--r--   0 keyur      (501) staff       (20)        1 2024-04-17 04:27:01.000000 moesif_aiohttp-1.1.0/moesif_aiohttp.egg-info/dependency_links.txt
+-rw-r--r--   0 keyur      (501) staff       (20)      154 2024-04-17 04:27:01.000000 moesif_aiohttp-1.1.0/moesif_aiohttp.egg-info/requires.txt
+-rw-r--r--   0 keyur      (501) staff       (20)       15 2024-04-17 04:27:01.000000 moesif_aiohttp-1.1.0/moesif_aiohttp.egg-info/top_level.txt
+-rw-r--r--   0 keyur      (501) staff       (20)       67 2024-04-17 04:27:01.480951 moesif_aiohttp-1.1.0/setup.cfg
+-rw-r--r--   0 keyur      (501) staff       (20)     3273 2024-04-17 04:25:54.000000 moesif_aiohttp-1.1.0/setup.py
```

### Comparing `moesif_aiohttp-1.0.1/LICENSE` & `moesif_aiohttp-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moesif_aiohttp-1.0.1/PKG-INFO` & `moesif_aiohttp-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moesif_aiohttp
-Version: 1.0.1
+Version: 1.1.0
 Summary: Moesif Middleware for AIOHTTP
 Home-page: https://www.moesif.com/docs/server-integration/python-aiohttp/
 Author: Moesif, Inc
 License: Apache Software License
 Keywords: log analysis restful api development debug wsgi flask bottle http middleware
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `moesif_aiohttp-1.0.1/README.md` & `moesif_aiohttp-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `moesif_aiohttp-1.0.1/moesif_aiohttp/event_mapper.py` & `moesif_aiohttp-1.1.0/moesif_aiohttp/event_mapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from moesifapi.models import *
 from datetime import datetime
 from moesifapi.parse_body import ParseBody
 import logging
 import os
+import json
 
 logger = logging.getLogger(__name__)
 
 class EventMapper:
 
     def __init__(self):
         self.parse_body = ParseBody()
@@ -27,56 +28,59 @@
                         user_id=user_id,
                         company_id=company_id,
                         session_token=session_token,
                         metadata=metadata,
                         direction="Incoming",
                         blocked_by=blocked_by)
 
-    async def to_request(self, request, log_body):
+    async def to_request(self, request, log_body, debug):
         request_time = self.get_utc_now()
 
         # convert headers (multiDictProxy class) into dict
         req_headers = self.get_headers(request.headers.items())
 
         req_body = None
         req_transfer_encoding = None
         if log_body:
             try:
                 if request.body_exists:
-                    request_text = await request.text()
-                    req_body, req_transfer_encoding = self.parse_body.parse_string_body(request_text, None, req_headers)
+                    request_text = await request.read()
+                    req_body, req_transfer_encoding = self.parse_body.parse_bytes_body(request_text, None, req_headers)
             except Exception as e:
-                pass
+                if debug:
+                    logger.error(f"Error while parsing the request body: {str(e)}")
 
         # Prepare Event Request Model
         return EventRequestModel(time=request_time,
                                 uri=str(request.url),
                                 verb=request.method,
                                 api_version=None,
                                 ip_address=request.remote,
                                 headers=req_headers,
                                 body=req_body,
                                 transfer_encoding=req_transfer_encoding)
 
-
-    def to_response(self, response, log_body):
-        
+    def to_response(self, response, log_body, sent_data, debug):
         response_time = self.get_utc_now()
 
         # convert headers (multiDictProxy class) into dict
         rsp_headers = self.get_headers(response.headers.items())
 
         rsp_body = None
         rsp_transfer_encoding = None
 
         if log_body:
             try:
-                rsp_text = response.text
-                rsp_body, rsp_transfer_encoding = self.parse_body.parse_string_body(rsp_text, None, rsp_headers)
+                if sent_data:
+                    rsp_body, rsp_transfer_encoding = self.parse_body.parse_string_body(json.dumps(sent_data), None, rsp_headers)
+                else:
+                    rsp_text = response.text
+                    rsp_body, rsp_transfer_encoding = self.parse_body.parse_string_body(rsp_text, None, rsp_headers)
             except Exception as e:
-                pass
+                if debug:
+                    logger.error(f"Error while parsing the response body: {str(e)}")
 
         return EventResponseModel(time=response_time,
                                 status=response.status,
                                 headers=rsp_headers,
                                 body=rsp_body,
                                 transfer_encoding=rsp_transfer_encoding)
```

### Comparing `moesif_aiohttp-1.0.1/moesif_aiohttp/logger_helper.py` & `moesif_aiohttp-1.1.0/moesif_aiohttp/logger_helper.py`

 * *Files identical despite different names*

### Comparing `moesif_aiohttp-1.0.1/moesif_aiohttp/middleware.py` & `moesif_aiohttp-1.1.0/moesif_aiohttp/middleware.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,19 +8,64 @@
 from moesifapi.app_config import AppConfig
 from moesifapi.api_helper import APIHelper
 from moesifapi.update_companies import Company
 from moesifapi.update_users import User
 from .logger_helper import LoggerHelper
 from .event_mapper import EventMapper
 from aiohttp import web
+from aiohttp_sse import EventSourceResponse
+from aiohttp.web_response import Response, StreamResponse
 import logging
 import atexit
 import random
 import math
 import aiohttp_sse
+import json
+
+# Override the write method of StreamResponse for API logging
+async def custom_write(self, data, _mo_body=[]):
+    # The data is of type bytes, so converting it to string
+    decoded_data = data.decode("utf-8")
+    # When the response is of type StreamResponse, the data: stream is already processed by the send method,
+    # so avoid it to process data: stream multiple time
+    if "data:" not in decoded_data:
+        # Create the _mo_body if it doesn't exist and add the decoded_data to the list
+        # else keep appending decoded_data to an existing _mo_body list
+        try:
+            self._mo_body.append(decoded_data)
+        except Exception as e:
+            self._mo_body = [decoded_data]
+
+    # Call the original send method
+    await self.original_write(data)
+
+
+StreamResponse.original_write = StreamResponse.write
+StreamResponse.write = custom_write
+
+# Override the send method of EventSourceResponse for API logging
+async def custom_send(self, data, event=None, _mo_body=[]):
+    # Try to convert to json object and if couldn't use it as it is
+    json_data = None
+    try:
+        json_data = json.loads(data)
+    except Exception as e:
+        json_data = data
+
+    # Create the _mo_body if it doesn't exist and add the json_data to the list
+    # else keep appending json_data to an existing _mo_body list
+    try:
+        self._mo_body.append(json_data)
+    except Exception as e:
+        self._mo_body = [json_data]
+    # Call the original send method
+    await self._send(data, event=event)
+
+EventSourceResponse._send = EventSourceResponse.send
+EventSourceResponse.send = custom_send
 
 logger = logging.getLogger(__name__)
 
 @middleware
 class MoesifMiddleware:
 
     def __init__(self, settings):
@@ -101,15 +146,15 @@
             if self.DEBUG:
                 logger.debug(f"Error while preparing the response content: {str(ex)}")
         return response_content
 
     async def __call__(self, request, handler):
 
         # Prepare Event Request Model
-        event_request = await self.event_mapper.to_request(request, self.LOG_BODY)
+        event_request = await self.event_mapper.to_request(request, self.LOG_BODY, self.DEBUG)
 
         governed_response = {}
         if self.config.have_governance_rules():
             # we must fire these hooks early.
             user_id = self.logger_helper.get_user_id(self.settings, request, None, self.DEBUG)
             company_id = self.logger_helper.get_company_id(self.settings, request, None, self.DEBUG)
             governed_response = self.config.govern_request(event_request, user_id, company_id, event_request.body)
@@ -119,16 +164,22 @@
             # start response immediately, skip next step
             response_content = self.prepare_response_content(governed_response['body'])
             blocked_by = governed_response['blocked_by']
             response = web.Response(status=governed_response['status'], headers=governed_response['headers'], text=response_content)
         else:
             response = await handler(request)
 
-        # Prepare Event Response Model
-        event_response = self.event_mapper.to_response(response, self.LOG_BODY)
+        # Prepare the event response body
+        event_response = self.event_mapper.to_response(response, self.LOG_BODY, getattr(response, '_mo_body', None), self.DEBUG)
+        # Clear the response._mo_body list after the request
+        try:
+            if "_mo_body" in response:
+                response._mo_body.clear()
+        except Exception as e:
+            pass
 
         # Add user, company, session_token, and metadata
         user_id = self.logger_helper.get_user_id(self.settings, request, response, self.DEBUG)
         company_id = self.logger_helper.get_company_id(self.settings, request, response, self.DEBUG)
         session_token = self.logger_helper.get_session_token(self.settings, request, response, self.DEBUG)
         metadata = self.logger_helper.get_metadata(self.settings, request, response, self.DEBUG)
```

### Comparing `moesif_aiohttp-1.0.1/moesif_aiohttp.egg-info/PKG-INFO` & `moesif_aiohttp-1.1.0/moesif_aiohttp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moesif-aiohttp
-Version: 1.0.1
+Version: 1.1.0
 Summary: Moesif Middleware for AIOHTTP
 Home-page: https://www.moesif.com/docs/server-integration/python-aiohttp/
 Author: Moesif, Inc
 License: Apache Software License
 Keywords: log analysis restful api development debug wsgi flask bottle http middleware
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `moesif_aiohttp-1.0.1/setup.py` & `moesif_aiohttp-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 setup(
     name='moesif_aiohttp',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.1',
+    version='1.1.0',
 
     description='Moesif Middleware for AIOHTTP',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     # The project's main homepage.
     url='https://www.moesif.com/docs/server-integration/python-aiohttp/',
```

