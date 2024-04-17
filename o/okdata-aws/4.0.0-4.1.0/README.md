# Comparing `tmp/okdata-aws-4.0.0.tar.gz` & `tmp/okdata_aws-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okdata-aws-4.0.0.tar", last modified: Thu Mar 21 12:42:43 2024, max compression
+gzip compressed data, was "okdata_aws-4.1.0.tar", last modified: Wed Apr 17 10:21:45 2024, max compression
```

## Comparing `okdata-aws-4.0.0.tar` & `okdata_aws-4.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-03-21 12:42:43.431416 okdata-aws-4.0.0/
--rw-r--r--   0 simen     (1000) simen     (1000)     4707 2024-03-21 12:42:43.431416 okdata-aws-4.0.0/PKG-INFO
--rw-r--r--   0 simen     (1000) simen     (1000)     3989 2024-03-21 12:40:24.000000 okdata-aws-4.0.0/README.md
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-03-21 12:42:43.431416 okdata-aws-4.0.0/okdata/
--rw-r--r--   0 simen     (1000) simen     (1000)       56 2024-03-15 09:08:49.000000 okdata-aws-4.0.0/okdata/__init__.py
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-03-21 12:42:43.431416 okdata-aws-4.0.0/okdata/aws/
--rw-r--r--   0 simen     (1000) simen     (1000)        0 2024-03-15 09:08:49.000000 okdata-aws-4.0.0/okdata/aws/__init__.py
--rw-r--r--   0 simen     (1000) simen     (1000)     7389 2024-03-15 09:08:49.000000 okdata-aws-4.0.0/okdata/aws/logging.py
--rw-r--r--   0 simen     (1000) simen     (1000)      551 2024-03-15 09:08:49.000000 okdata-aws-4.0.0/okdata/aws/ssm.py
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-03-21 12:42:43.431416 okdata-aws-4.0.0/okdata/aws/status/
--rw-r--r--   0 simen     (1000) simen     (1000)      176 2024-03-15 09:08:49.000000 okdata-aws-4.0.0/okdata/aws/status/__init__.py
--rw-r--r--   0 simen     (1000) simen     (1000)     3363 2024-03-21 10:50:36.000000 okdata-aws-4.0.0/okdata/aws/status/model.py
--rw-r--r--   0 simen     (1000) simen     (1000)     1936 2024-03-18 12:33:04.000000 okdata-aws-4.0.0/okdata/aws/status/sdk.py
--rw-r--r--   0 simen     (1000) simen     (1000)     2381 2024-03-21 12:40:24.000000 okdata-aws-4.0.0/okdata/aws/status/wrapper.py
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-03-21 12:42:43.431416 okdata-aws-4.0.0/okdata_aws.egg-info/
--rw-r--r--   0 simen     (1000) simen     (1000)     4707 2024-03-21 12:42:43.000000 okdata-aws-4.0.0/okdata_aws.egg-info/PKG-INFO
--rw-r--r--   0 simen     (1000) simen     (1000)      501 2024-03-21 12:42:43.000000 okdata-aws-4.0.0/okdata_aws.egg-info/SOURCES.txt
--rw-r--r--   0 simen     (1000) simen     (1000)        1 2024-03-21 12:42:43.000000 okdata-aws-4.0.0/okdata_aws.egg-info/dependency_links.txt
--rw-r--r--   0 simen     (1000) simen     (1000)        7 2024-03-21 12:42:43.000000 okdata-aws-4.0.0/okdata_aws.egg-info/namespace_packages.txt
--rw-r--r--   0 simen     (1000) simen     (1000)       67 2024-03-21 12:42:43.000000 okdata-aws-4.0.0/okdata_aws.egg-info/requires.txt
--rw-r--r--   0 simen     (1000) simen     (1000)        7 2024-03-21 12:42:43.000000 okdata-aws-4.0.0/okdata_aws.egg-info/top_level.txt
--rw-r--r--   0 simen     (1000) simen     (1000)      241 2024-03-15 09:08:49.000000 okdata-aws-4.0.0/pyproject.toml
--rw-r--r--   0 simen     (1000) simen     (1000)       38 2024-03-21 12:42:43.431416 okdata-aws-4.0.0/setup.cfg
--rw-r--r--   0 simen     (1000) simen     (1000)     1196 2024-03-21 12:40:56.000000 okdata-aws-4.0.0/setup.py
-drwxr-xr-x   0 simen     (1000) simen     (1000)        0 2024-03-21 12:42:43.431416 okdata-aws-4.0.0/tests/
--rw-r--r--   0 simen     (1000) simen     (1000)     8593 2024-03-15 09:08:49.000000 okdata-aws-4.0.0/tests/test_logging.py
--rw-r--r--   0 simen     (1000) simen     (1000)     1087 2024-03-21 10:50:36.000000 okdata-aws-4.0.0/tests/test_model.py
--rw-r--r--   0 simen     (1000) simen     (1000)     5174 2024-03-21 10:50:36.000000 okdata-aws-4.0.0/tests/test_status.py
+drwxr-xr-x   0 petterhj   (501) staff       (20)        0 2024-04-17 10:21:45.134966 okdata_aws-4.1.0/
+-rw-r--r--   0 petterhj   (501) staff       (20)     4853 2024-04-17 10:21:45.134619 okdata_aws-4.1.0/PKG-INFO
+-rw-r--r--   0 petterhj   (501) staff       (20)     3989 2024-03-22 12:29:23.000000 okdata_aws-4.1.0/README.md
+drwxr-xr-x   0 petterhj   (501) staff       (20)        0 2024-04-17 10:21:45.130759 okdata_aws-4.1.0/okdata/
+-rw-r--r--   0 petterhj   (501) staff       (20)       56 2024-02-15 11:04:36.000000 okdata_aws-4.1.0/okdata/__init__.py
+drwxr-xr-x   0 petterhj   (501) staff       (20)        0 2024-04-17 10:21:45.131196 okdata_aws-4.1.0/okdata/aws/
+-rw-r--r--   0 petterhj   (501) staff       (20)        0 2024-02-15 11:04:36.000000 okdata_aws-4.1.0/okdata/aws/__init__.py
+-rw-r--r--   0 petterhj   (501) staff       (20)     7830 2024-04-17 10:14:24.000000 okdata_aws-4.1.0/okdata/aws/logging.py
+-rw-r--r--   0 petterhj   (501) staff       (20)      551 2024-03-15 12:36:35.000000 okdata_aws-4.1.0/okdata/aws/ssm.py
+drwxr-xr-x   0 petterhj   (501) staff       (20)        0 2024-04-17 10:21:45.132230 okdata_aws-4.1.0/okdata/aws/status/
+-rw-r--r--   0 petterhj   (501) staff       (20)      176 2024-02-15 11:04:36.000000 okdata_aws-4.1.0/okdata/aws/status/__init__.py
+-rw-r--r--   0 petterhj   (501) staff       (20)     3363 2024-03-21 08:53:37.000000 okdata_aws-4.1.0/okdata/aws/status/model.py
+-rw-r--r--   0 petterhj   (501) staff       (20)     1936 2024-03-18 14:49:37.000000 okdata_aws-4.1.0/okdata/aws/status/sdk.py
+-rw-r--r--   0 petterhj   (501) staff       (20)     2381 2024-03-22 12:29:23.000000 okdata_aws-4.1.0/okdata/aws/status/wrapper.py
+drwxr-xr-x   0 petterhj   (501) staff       (20)        0 2024-04-17 10:21:45.134222 okdata_aws-4.1.0/okdata_aws.egg-info/
+-rw-r--r--   0 petterhj   (501) staff       (20)     4853 2024-04-17 10:21:45.000000 okdata_aws-4.1.0/okdata_aws.egg-info/PKG-INFO
+-rw-r--r--   0 petterhj   (501) staff       (20)      501 2024-04-17 10:21:45.000000 okdata_aws-4.1.0/okdata_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 petterhj   (501) staff       (20)        1 2024-04-17 10:21:45.000000 okdata_aws-4.1.0/okdata_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 petterhj   (501) staff       (20)        7 2024-04-17 10:21:45.000000 okdata_aws-4.1.0/okdata_aws.egg-info/namespace_packages.txt
+-rw-r--r--   0 petterhj   (501) staff       (20)       71 2024-04-17 10:21:45.000000 okdata_aws-4.1.0/okdata_aws.egg-info/requires.txt
+-rw-r--r--   0 petterhj   (501) staff       (20)        7 2024-04-17 10:21:45.000000 okdata_aws-4.1.0/okdata_aws.egg-info/top_level.txt
+-rw-r--r--   0 petterhj   (501) staff       (20)      241 2024-02-15 11:04:36.000000 okdata_aws-4.1.0/pyproject.toml
+-rw-r--r--   0 petterhj   (501) staff       (20)       38 2024-04-17 10:21:45.135030 okdata_aws-4.1.0/setup.cfg
+-rw-r--r--   0 petterhj   (501) staff       (20)     1200 2024-04-17 10:19:24.000000 okdata_aws-4.1.0/setup.py
+drwxr-xr-x   0 petterhj   (501) staff       (20)        0 2024-04-17 10:21:45.133860 okdata_aws-4.1.0/tests/
+-rw-r--r--   0 petterhj   (501) staff       (20)     9125 2024-04-17 10:14:24.000000 okdata_aws-4.1.0/tests/test_logging.py
+-rw-r--r--   0 petterhj   (501) staff       (20)     1087 2024-03-21 08:53:37.000000 okdata_aws-4.1.0/tests/test_model.py
+-rw-r--r--   0 petterhj   (501) staff       (20)     5174 2024-03-21 08:53:37.000000 okdata_aws-4.1.0/tests/test_status.py
```

### Comparing `okdata-aws-4.0.0/PKG-INFO` & `okdata_aws-4.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: okdata-aws
-Version: 4.0.0
+Version: 4.1.0
 Summary: Collection of helpers for working with AWS
 Home-page: https://github.com/oslokommune/okdata-aws
 Author: Oslo Origo
 Author-email: dataplattform@oslo.kommune.no
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
+Requires-Dist: boto3
+Requires-Dist: okdata-sdk<4,>=3.1.1
+Requires-Dist: requests
+Requires-Dist: starlette<1.0.0,>=0.36.3
+Requires-Dist: structlog
 
 # okdata-aws
 
 Collection of helpers for working with AWS.
 
 ## Logging for Lambda
```

### Comparing `okdata-aws-4.0.0/README.md` & `okdata_aws-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `okdata-aws-4.0.0/okdata/aws/logging.py` & `okdata_aws-4.1.0/okdata/aws/logging.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import time
+from contextlib import asynccontextmanager
 from copy import copy
 from functools import wraps
 
 import structlog
 from starlette.middleware.base import BaseHTTPMiddleware
 from starlette.responses import JSONResponse, Response as StarletteResponse
 
@@ -34,39 +35,50 @@
         return _handle_response(await call_next(request))
 
     return async_handler(
         request.scope.get("aws.event", {}), request.scope.get("aws.context")
     )
 
 
+def _fastapi_lifespan_context(app):
+    # https://fastapi.tiangolo.com/advanced/events/#lifespan
+
+    global SERVICE_NAME
+    SERVICE_NAME = os.getenv("SERVICE_NAME")
+
+    default_lifespan = app.router.lifespan_context
+
+    @asynccontextmanager
+    async def _lifespan(app):
+        # Wrap the existing lifespan generator in order to not override
+        # any additional lifespan events configured for the app using
+        # `FastAPI(lifespan=...)`.
+        async with default_lifespan(app) as state:
+            yield state
+
+        # Take advantage of the fact that shutdown is called after each
+        # Lambda function invocation to finalize the logging after any
+        # exceptions are logged.
+        _finalize(_start_time)
+
+    return _lifespan
+
+
 def add_fastapi_logging(app):
+    app.router.lifespan_context = _fastapi_lifespan_context(app)
     app.add_middleware(BaseHTTPMiddleware, dispatch=_logging_middleware)
 
-    @app.on_event("startup")
-    async def startup_event():
-        global SERVICE_NAME
-        SERVICE_NAME = os.getenv("SERVICE_NAME")
-
     @app.exception_handler(Exception)
     async def exception_handler(request, e):
         global _logger
         _logger = _logger.bind(exc_info=e, level="error")
         return JSONResponse(
             status_code=500, content={"detail": "Oops! Something went wrong!"}
         )
 
-    @app.on_event("shutdown")
-    async def shutdown_event():
-        """
-        Take advantage of the fact that shutdown is called after each
-        Lambda function invocation to finalize the logging after any
-        exceptions are logged.
-        """
-        _finalize(_start_time)
-
 
 def _init_logger(handler, event, context):
     global COLD_START
     global SERVICE_NAME
     global _logger
 
     headers = event.get("headers", {}) or {}
```

### Comparing `okdata-aws-4.0.0/okdata/aws/ssm.py` & `okdata_aws-4.1.0/okdata/aws/ssm.py`

 * *Files identical despite different names*

### Comparing `okdata-aws-4.0.0/okdata/aws/status/model.py` & `okdata_aws-4.1.0/okdata/aws/status/model.py`

 * *Files identical despite different names*

### Comparing `okdata-aws-4.0.0/okdata/aws/status/sdk.py` & `okdata_aws-4.1.0/okdata/aws/status/sdk.py`

 * *Files identical despite different names*

### Comparing `okdata-aws-4.0.0/okdata/aws/status/wrapper.py` & `okdata_aws-4.1.0/okdata/aws/status/wrapper.py`

 * *Files identical despite different names*

### Comparing `okdata-aws-4.0.0/okdata_aws.egg-info/PKG-INFO` & `okdata_aws-4.1.0/okdata_aws.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 Metadata-Version: 2.1
 Name: okdata-aws
-Version: 4.0.0
+Version: 4.1.0
 Summary: Collection of helpers for working with AWS
 Home-page: https://github.com/oslokommune/okdata-aws
 Author: Oslo Origo
 Author-email: dataplattform@oslo.kommune.no
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
+Requires-Dist: boto3
+Requires-Dist: okdata-sdk<4,>=3.1.1
+Requires-Dist: requests
+Requires-Dist: starlette<1.0.0,>=0.36.3
+Requires-Dist: structlog
 
 # okdata-aws
 
 Collection of helpers for working with AWS.
 
 ## Logging for Lambda
```

### Comparing `okdata-aws-4.0.0/setup.py` & `okdata_aws-4.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="okdata-aws",
-    version="4.0.0",
+    version="4.1.0",
     author="Oslo Origo",
     author_email="dataplattform@oslo.kommune.no",
     description="Collection of helpers for working with AWS",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/oslokommune/okdata-aws",
     packages=setuptools.find_namespace_packages(
@@ -25,13 +25,13 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
     ],
     install_requires=[
         "boto3",
-        "okdata-sdk>=3,<4",
+        "okdata-sdk>=3.1.1,<4",
         "requests",
-        "starlette>=0.25.0,<1.0.0",
+        "starlette>=0.36.3,<1.0.0",
         "structlog",
     ],
 )
```

### Comparing `okdata-aws-4.0.0/tests/test_logging.py` & `okdata_aws-4.1.0/tests/test_logging.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 import json
 import os
 from time import sleep
 
-from okdata.aws.logging import hide_suffix, log_duration, log_dynamodb, logging_wrapper
+from fastapi import FastAPI
+from fastapi.testclient import TestClient
+
+from okdata.aws.logging import (
+    add_fastapi_logging,
+    hide_suffix,
+    log_duration,
+    log_dynamodb,
+    logging_wrapper,
+)
 
 empty_event = {}
 empty_context = None
 
 
 def empty_handler(event, context):
     return {}
@@ -312,7 +321,24 @@
     event = {"Count": 123}
     wrapper = logging_wrapper(dynamodb_handler)
     wrapper(event, empty_context)
 
     log = json.loads(capsys.readouterr().out)
 
     assert log["dynamodb_item_count"] == 123
+
+
+def test_fastapi_logging(capsys):
+    app = FastAPI()
+    add_fastapi_logging(app)
+
+    @app.get("/hello")
+    async def hello():
+        return {"msg": "Hello World"}
+
+    with TestClient(app) as client:
+        response = client.get("/hello")
+        assert response.status_code == 200
+
+    log = json.loads(capsys.readouterr().out)
+    assert log["response_status_code"] == 200
+    assert "duration_ms" in log
```

### Comparing `okdata-aws-4.0.0/tests/test_model.py` & `okdata_aws-4.1.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `okdata-aws-4.0.0/tests/test_status.py` & `okdata_aws-4.1.0/tests/test_status.py`

 * *Files identical despite different names*

