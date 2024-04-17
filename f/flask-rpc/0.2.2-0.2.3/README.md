# Comparing `tmp/flask_rpc-0.2.2.tar.gz` & `tmp/flask_rpc-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_rpc-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "flask_rpc-0.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `flask_rpc-0.2.2.tar` & `flask_rpc-0.2.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     3222 2024-04-12 19:58:26.539229 flask_rpc-0.2.2/.gitignore
--rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 flask_rpc-0.2.2/LICENSE
--rw-r--r--   0        0        0     3159 2024-04-13 10:47:58.119119 flask_rpc-0.2.2/README.md
--rw-r--r--   0        0        0      763 2024-04-12 16:22:33.729380 flask_rpc-0.2.2/app/__init__.py
--rw-r--r--   0        0        0       59 2024-04-12 10:26:26.537975 flask_rpc-0.2.2/app/extensions/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 20:04:31.966024 flask_rpc-0.2.2/app/models/__init__.py
--rw-r--r--   0        0        0     1637 2024-04-12 20:03:10.485400 flask_rpc-0.2.2/app/models/clients.py
--rw-r--r--   0        0        0     1707 2024-04-12 07:34:15.967950 flask_rpc-0.2.2/app/models/users.py
--rw-r--r--   0        0        0      344 2024-04-13 09:21:50.042415 flask_rpc-0.2.2/app/rpc/__init__.py
--rw-r--r--   0        0        0      302 2024-04-12 11:18:08.444428 flask_rpc-0.2.2/app/rpc/auth/__init__.py
--rw-r--r--   0        0        0        1 2024-04-11 20:44:17.134954 flask_rpc-0.2.2/app/rpc/auth/funcs/__init__.py
--rw-r--r--   0        0        0      274 2024-04-13 09:42:00.786616 flask_rpc-0.2.2/app/rpc/auth/funcs/login.py
--rw-r--r--   0        0        0      217 2024-04-13 09:42:00.798497 flask_rpc-0.2.2/app/rpc/auth/funcs/logout.py
--rw-r--r--   0        0        0      209 2024-04-13 09:42:00.791406 flask_rpc-0.2.2/app/rpc/auth/funcs/session.py
--rw-r--r--   0        0        0      341 2024-04-12 11:18:17.395564 flask_rpc-0.2.2/app/rpc/clients/__init__.py
--rw-r--r--   0        0        0     1454 2024-04-13 09:42:00.793180 flask_rpc-0.2.2/app/rpc/clients/funcs/__init__.py
--rw-r--r--   0        0        0      263 2024-04-13 11:01:57.572442 flask_rpc-0.2.2/app/rpc/tester/__init__.py
--rw-r--r--   0        0        0      293 2024-04-13 10:27:56.719801 flask_rpc-0.2.2/app/rpc/tester/funcs/__init__.py
--rw-r--r--   0        0        0     1289 2024-04-12 19:44:05.326618 flask_rpc-0.2.2/app/templates/index.html
--rw-r--r--   0        0        0       22 2024-04-13 11:11:19.434388 flask_rpc-0.2.2/flask_rpc/__init__.py
--rw-r--r--   0        0        0      124 2024-04-12 16:20:34.358527 flask_rpc-0.2.2/flask_rpc/latest.py
--rw-r--r--   0        0        0     4838 2024-04-13 11:10:41.736132 flask_rpc-0.2.2/flask_rpc/version_1_0.py
--rw-r--r--   0        0        0      741 2024-04-12 20:35:46.646934 flask_rpc-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       59 2024-04-10 22:19:07.350737 flask_rpc-0.2.2/requirements.txt
--rw-r--r--   0        0        0       16 2024-04-12 19:48:22.616554 flask_rpc-0.2.2/requirements_dev.txt
--rw-r--r--   0        0        0     3049 2024-04-13 09:57:53.420335 flask_rpc-0.2.2/test.py
--rw-r--r--   0        0        0     3798 1970-01-01 00:00:00.000000 flask_rpc-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     3222 2024-04-12 19:58:26.539229 flask_rpc-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 flask_rpc-0.2.3/LICENSE
+-rw-r--r--   0        0        0     3159 2024-04-13 10:47:58.119119 flask_rpc-0.2.3/README.md
+-rw-r--r--   0        0        0      763 2024-04-12 16:22:33.729380 flask_rpc-0.2.3/app/__init__.py
+-rw-r--r--   0        0        0       59 2024-04-12 10:26:26.537975 flask_rpc-0.2.3/app/extensions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 20:04:31.966024 flask_rpc-0.2.3/app/models/__init__.py
+-rw-r--r--   0        0        0     1637 2024-04-12 20:03:10.485400 flask_rpc-0.2.3/app/models/clients.py
+-rw-r--r--   0        0        0     1707 2024-04-12 07:34:15.967950 flask_rpc-0.2.3/app/models/users.py
+-rw-r--r--   0        0        0      344 2024-04-13 09:21:50.042415 flask_rpc-0.2.3/app/rpc/__init__.py
+-rw-r--r--   0        0        0      302 2024-04-12 11:18:08.444428 flask_rpc-0.2.3/app/rpc/auth/__init__.py
+-rw-r--r--   0        0        0        1 2024-04-11 20:44:17.134954 flask_rpc-0.2.3/app/rpc/auth/funcs/__init__.py
+-rw-r--r--   0        0        0      274 2024-04-13 09:42:00.786616 flask_rpc-0.2.3/app/rpc/auth/funcs/login.py
+-rw-r--r--   0        0        0      217 2024-04-13 09:42:00.798497 flask_rpc-0.2.3/app/rpc/auth/funcs/logout.py
+-rw-r--r--   0        0        0      209 2024-04-13 09:42:00.791406 flask_rpc-0.2.3/app/rpc/auth/funcs/session.py
+-rw-r--r--   0        0        0      341 2024-04-12 11:18:17.395564 flask_rpc-0.2.3/app/rpc/clients/__init__.py
+-rw-r--r--   0        0        0     1454 2024-04-13 09:42:00.793180 flask_rpc-0.2.3/app/rpc/clients/funcs/__init__.py
+-rw-r--r--   0        0        0      263 2024-04-13 11:01:57.572442 flask_rpc-0.2.3/app/rpc/tester/__init__.py
+-rw-r--r--   0        0        0      293 2024-04-13 10:27:56.719801 flask_rpc-0.2.3/app/rpc/tester/funcs/__init__.py
+-rw-r--r--   0        0        0     1289 2024-04-12 19:44:05.326618 flask_rpc-0.2.3/app/templates/index.html
+-rw-r--r--   0        0        0       22 2024-04-17 11:59:29.370829 flask_rpc-0.2.3/flask_rpc/__init__.py
+-rw-r--r--   0        0        0      124 2024-04-12 16:20:34.358527 flask_rpc-0.2.3/flask_rpc/latest.py
+-rw-r--r--   0        0        0     4964 2024-04-17 11:54:48.950561 flask_rpc-0.2.3/flask_rpc/version_1_0.py
+-rw-r--r--   0        0        0      741 2024-04-12 20:35:46.646934 flask_rpc-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       59 2024-04-10 22:19:07.350737 flask_rpc-0.2.3/requirements.txt
+-rw-r--r--   0        0        0       16 2024-04-12 19:48:22.616554 flask_rpc-0.2.3/requirements_dev.txt
+-rw-r--r--   0        0        0     3049 2024-04-13 09:57:53.420335 flask_rpc-0.2.3/test.py
+-rw-r--r--   0        0        0     3798 1970-01-01 00:00:00.000000 flask_rpc-0.2.3/PKG-INFO
```

### Comparing `flask_rpc-0.2.2/.gitignore` & `flask_rpc-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.2/LICENSE` & `flask_rpc-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.2/README.md` & `flask_rpc-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.2/app/__init__.py` & `flask_rpc-0.2.3/app/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.2/app/models/clients.py` & `flask_rpc-0.2.3/app/models/clients.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.2/app/models/users.py` & `flask_rpc-0.2.3/app/models/users.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.2/app/rpc/clients/funcs/__init__.py` & `flask_rpc-0.2.3/app/rpc/clients/funcs/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.2/app/templates/index.html` & `flask_rpc-0.2.3/app/templates/index.html`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.2/flask_rpc/version_1_0.py` & `flask_rpc-0.2.3/flask_rpc/version_1_0.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,15 +85,18 @@
         return r
 
 
 class RPC:
     LOOKUP: t.Dict[str, t.Callable]
 
     def __init__(
-        self, app_or_blueprint: t.Union[Flask, Blueprint], url_prefix: str = "/"
+        self,
+        app_or_blueprint: t.Union[Flask, Blueprint],
+        url_prefix: str = "/",
+        functions: t.Dict[str, t.Callable] = None,
     ):
         """
         Register the RPC route.
 
         :param app_or_blueprint: Flask / Blueprint
         :param url_prefix: Str
         """
@@ -104,14 +107,17 @@
                 f"Looks like {app_or_blueprint}, type({type(app_or_blueprint)}) might "
                 f"not be an instance of Flask, Flask Blueprint or be compatible with "
                 "setting Flask routes."
             )
 
         self._register_route(app_or_blueprint, url_prefix)
 
+        if functions:
+            self.functions(**functions)
+
     def functions(self, **kwargs: t.Callable):
         """
         Register RPC functions.
 
         remote_name=local_name
 
         :param kwargs:
@@ -166,15 +172,15 @@
         if not request.is_json:
             return RPCResponse.fail("Request must be JSON.")
 
         if not request.json:
             return RPCResponse.fail("Request must not be empty.")
 
         if not request.json.get("frpc") == 1.0:
-            return RPCResponse.fail("Invalid Flask-RPC version.")
+            return RPCResponse.fail("Invalid frpc version.")
 
         try:
             rpcm = RPCModel(**request.json)
         except ValidationError:
             return RPCResponse.fail("Invalid request.")
 
         try:
```

### Comparing `flask_rpc-0.2.2/pyproject.toml` & `flask_rpc-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.2/test.py` & `flask_rpc-0.2.3/test.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.2.2/PKG-INFO` & `flask_rpc-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-rpc
-Version: 0.2.2
+Version: 0.2.3
 Summary: Turn Flask into a simple RPC server
 Author-email: David Carmichael <david@uilix.com>
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

