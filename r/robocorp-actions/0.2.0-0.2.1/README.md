# Comparing `tmp/robocorp_actions-0.2.0.tar.gz` & `tmp/robocorp_actions-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_actions-0.2.0.tar", max compression
+gzip compressed data, was "robocorp_actions-0.2.1.tar", max compression
```

## Comparing `robocorp_actions-0.2.0.tar` & `robocorp_actions-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     2958 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/README.md
--rw-r--r--   0        0        0      991 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3638 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/src/robocorp/actions/__init__.py
--rw-r--r--   0        0        0       81 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/src/robocorp/actions/__main__.py
--rw-r--r--   0        0        0     6717 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/src/robocorp/actions/_action_context.py
--rw-r--r--   0        0        0      140 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/src/robocorp/actions/_action_options.py
--rw-r--r--   0        0        0     5199 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/src/robocorp/actions/_args_dispatcher.py
--rw-r--r--   0        0        0     4243 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/src/robocorp/actions/_fixtures.py
--rw-r--r--   0        0        0    11984 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/src/robocorp/actions/_lint_action.py
--rw-r--r--   0        0        0     4359 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/src/robocorp/actions/_managed_parameters.py
--rw-r--r--   0        0        0      561 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/src/robocorp/actions/_protocols.py
--rw-r--r--   0        0        0     2907 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/src/robocorp/actions/_request.py
--rw-r--r--   0        0        0     1023 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/src/robocorp/actions/_request_impl.py
--rw-r--r--   0        0        0     4480 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/src/robocorp/actions/_secret.py
--rw-r--r--   0        0        0     2123 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/src/robocorp/actions/cli.py
--rw-r--r--   0        0        0        0 2024-04-10 19:50:43.170851 robocorp_actions-0.2.0/src/robocorp/actions/py.typed
--rw-r--r--   0        0        0     3697 1970-01-01 00:00:00.000000 robocorp_actions-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2958 2024-04-17 18:12:23.825776 robocorp_actions-0.2.1/README.md
+-rw-r--r--   0        0        0      991 2024-04-17 18:12:23.825776 robocorp_actions-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3638 2024-04-17 18:12:23.825776 robocorp_actions-0.2.1/src/robocorp/actions/__init__.py
+-rw-r--r--   0        0        0       81 2024-04-17 18:12:23.825776 robocorp_actions-0.2.1/src/robocorp/actions/__main__.py
+-rw-r--r--   0        0        0     7521 2024-04-17 18:12:23.825776 robocorp_actions-0.2.1/src/robocorp/actions/_action_context.py
+-rw-r--r--   0        0        0      140 2024-04-17 18:12:23.825776 robocorp_actions-0.2.1/src/robocorp/actions/_action_options.py
+-rw-r--r--   0        0        0     5199 2024-04-17 18:12:23.825776 robocorp_actions-0.2.1/src/robocorp/actions/_args_dispatcher.py
+-rw-r--r--   0        0        0     4243 2024-04-17 18:12:23.825776 robocorp_actions-0.2.1/src/robocorp/actions/_fixtures.py
+-rw-r--r--   0        0        0    11984 2024-04-17 18:12:23.825776 robocorp_actions-0.2.1/src/robocorp/actions/_lint_action.py
+-rw-r--r--   0        0        0     4359 2024-04-17 18:12:23.825776 robocorp_actions-0.2.1/src/robocorp/actions/_managed_parameters.py
+-rw-r--r--   0        0        0      561 2024-04-17 18:12:23.825776 robocorp_actions-0.2.1/src/robocorp/actions/_protocols.py
+-rw-r--r--   0        0        0     2907 2024-04-17 18:12:23.825776 robocorp_actions-0.2.1/src/robocorp/actions/_request.py
+-rw-r--r--   0        0        0     1023 2024-04-17 18:12:23.825776 robocorp_actions-0.2.1/src/robocorp/actions/_request_impl.py
+-rw-r--r--   0        0        0     4480 2024-04-17 18:12:23.825776 robocorp_actions-0.2.1/src/robocorp/actions/_secret.py
+-rw-r--r--   0        0        0     2123 2024-04-17 18:12:23.825776 robocorp_actions-0.2.1/src/robocorp/actions/cli.py
+-rw-r--r--   0        0        0        0 2024-04-17 18:12:23.825776 robocorp_actions-0.2.1/src/robocorp/actions/py.typed
+-rw-r--r--   0        0        0     3697 1970-01-01 00:00:00.000000 robocorp_actions-0.2.1/PKG-INFO
```

### Comparing `robocorp_actions-0.2.0/README.md` & `robocorp_actions-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `robocorp_actions-0.2.0/pyproject.toml` & `robocorp_actions-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-actions"
-version = "0.2.0"
+version = "0.2.1"
 description = "Robocorp Actions"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robocorp/"
 license = "Apache-2.0"
```

### Comparing `robocorp_actions-0.2.0/src/robocorp/actions/__init__.py` & `robocorp_actions-0.2.1/src/robocorp/actions/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ._action_options import ActionOptions
 from ._fixtures import setup, teardown
 from ._protocols import IAction, Status
 from ._request import Request
 from ._secret import Secret
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 @overload
 def action(func: Callable) -> Callable:
     ...
```

### Comparing `robocorp_actions-0.2.0/src/robocorp/actions/_action_context.py` & `robocorp_actions-0.2.1/src/robocorp/actions/_action_context.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         """
         Args:
             data: The data requested from that source.
                 If encrypted, must be something as:
 
                 base64(json.dumps({
                    cipher: blob_of_data
-                   algorithm: "aes256-cdc"
+                   algorithm: "aes256-gcm"
                    iv: nonce
                 }))
 
                 Otherwise the payload should be passed directly,
                 which should be something as:
                     base64(json.dumps({
                       'secrets': {'secret_name': 'secret_value'}
@@ -122,25 +122,28 @@
                 raise RuntimeError(
                     "The information in the X-Action-Server seems to be encrypted, but decryption keys are not available in ACTION_SERVER_DECRYPT_KEYS."
                 )
 
             cipher = self._encrypted_data["cipher"]
             algorithm = self._encrypted_data["algorithm"]
             iv = self._encrypted_data["iv"]
+            auth_tag = self._encrypted_data.get("auth-tag")
 
             if not isinstance(cipher, str):
-                raise RuntimeError(f"Expected the cipher to be a str. Found: {cipher}")
+                raise RuntimeError(
+                    f"Expected the cipher to be a str. Found: {cipher!r}"
+                )
 
             if not isinstance(algorithm, str):
                 raise RuntimeError(
-                    f"Expected the algorithm to be a str. Found: {algorithm}"
+                    f"Expected the algorithm to be a str. Found: {algorithm!r}"
                 )
 
             if not isinstance(iv, str):
-                raise RuntimeError(f"Expected the iv to be a str. Found: {iv}")
+                raise RuntimeError(f"Expected the iv to be a str. Found: {iv!r}")
 
             try:
                 cipher_decoded_base_64: bytes = base64.b64decode(cipher)
             except Exception:
                 raise RuntimeError(
                     "Unable to decode the 'cipher' field passed to X-Action-Context as base64."
                 )
@@ -148,25 +151,42 @@
             try:
                 iv_decoded_base_64: bytes = base64.b64decode(iv)
             except Exception:
                 raise RuntimeError(
                     "Unable to decode the 'iv' field passed to X-Action-Context as base64."
                 )
 
-            if algorithm != "aes256-cdc":
+            if not auth_tag:
+                auth_tag_decoded_base_64: bytes = b""
+            else:
+                if isinstance(auth_tag, str):
+                    try:
+                        auth_tag_decoded_base_64 = base64.b64decode(auth_tag)
+                    except Exception:
+                        raise RuntimeError(
+                            "Unable to decode the 'auth-tag' field passed to X-Action-Context as base64."
+                        )
+                else:
+                    raise RuntimeError(
+                        f"Expected the auth-tag to be a str. Found: {auth_tag!r}"
+                    )
+
+            if algorithm != "aes256-gcm":
                 raise RuntimeError(
                     f"Unable to recognize X-Action-Context encryption algorithm: {algorithm}"
                 )
 
             for key in keys:
                 k: bytes = base64.b64decode(key.encode("ascii"))
                 aesgcm = AESGCM(k)
                 try:
                     raw_data = aesgcm.decrypt(
-                        iv_decoded_base_64, cipher_decoded_base_64, None
+                        iv_decoded_base_64,
+                        cipher_decoded_base_64,
+                        auth_tag_decoded_base_64,
                     )
                     break
                 except Exception:
                     continue
             else:
                 raise RuntimeError(
                     "It was not possible to decode the X-Action-Context header with any of the available keys."
```

### Comparing `robocorp_actions-0.2.0/src/robocorp/actions/_args_dispatcher.py` & `robocorp_actions-0.2.1/src/robocorp/actions/_args_dispatcher.py`

 * *Files identical despite different names*

### Comparing `robocorp_actions-0.2.0/src/robocorp/actions/_fixtures.py` & `robocorp_actions-0.2.1/src/robocorp/actions/_fixtures.py`

 * *Files identical despite different names*

### Comparing `robocorp_actions-0.2.0/src/robocorp/actions/_lint_action.py` & `robocorp_actions-0.2.1/src/robocorp/actions/_lint_action.py`

 * *Files identical despite different names*

### Comparing `robocorp_actions-0.2.0/src/robocorp/actions/_managed_parameters.py` & `robocorp_actions-0.2.1/src/robocorp/actions/_managed_parameters.py`

 * *Files identical despite different names*

### Comparing `robocorp_actions-0.2.0/src/robocorp/actions/_protocols.py` & `robocorp_actions-0.2.1/src/robocorp/actions/_protocols.py`

 * *Files identical despite different names*

### Comparing `robocorp_actions-0.2.0/src/robocorp/actions/_request.py` & `robocorp_actions-0.2.1/src/robocorp/actions/_request.py`

 * *Files identical despite different names*

### Comparing `robocorp_actions-0.2.0/src/robocorp/actions/_request_impl.py` & `robocorp_actions-0.2.1/src/robocorp/actions/_request_impl.py`

 * *Files identical despite different names*

### Comparing `robocorp_actions-0.2.0/src/robocorp/actions/_secret.py` & `robocorp_actions-0.2.1/src/robocorp/actions/_secret.py`

 * *Files identical despite different names*

### Comparing `robocorp_actions-0.2.0/src/robocorp/actions/cli.py` & `robocorp_actions-0.2.1/src/robocorp/actions/cli.py`

 * *Files identical despite different names*

### Comparing `robocorp_actions-0.2.0/PKG-INFO` & `robocorp_actions-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocorp-actions
-Version: 0.2.0
+Version: 0.2.1
 Summary: Robocorp Actions
 Home-page: https://github.com/robocorp/robocorp/
 License: Apache-2.0
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

