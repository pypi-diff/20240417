# Comparing `tmp/lowatt_grdf-2.2.0.tar.gz` & `tmp/lowatt_grdf-2.2.1.tar.gz`

## Comparing `lowatt_grdf-2.2.0.tar` & `lowatt_grdf-2.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/.flake8
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/MANIFEST.in
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/dev-requirements.txt
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/mypy.ini
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/pytest.ini
--rw-r--r--   0        0        0     8730 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/staging-api-requests.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/tox.ini
--rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/.github/workflows/tox.yml
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/lowatt_grdf/__init__.py
--rw-r--r--   0        0        0     9717 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/lowatt_grdf/api.py
--rw-r--r--   0        0        0     6885 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/lowatt_grdf/main.py
--rw-r--r--   0        0        0     7735 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/lowatt_grdf/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/lowatt_grdf/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/tests/__init__.py
--rw-r--r--   0        0        0    16435 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/tests/test_api.py
--rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/tests/test_main.py
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/tests/test_models.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/LICENSE
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/README.md
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.1/.flake8
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.1/MANIFEST.in
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.1/dev-requirements.txt
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.1/mypy.ini
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.1/pytest.ini
+-rw-r--r--   0        0        0     8730 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.1/staging-api-requests.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.1/tox.ini
+-rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.1/.github/workflows/tox.yml
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.1/lowatt_grdf/__init__.py
+-rw-r--r--   0        0        0     9623 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.1/lowatt_grdf/api.py
+-rw-r--r--   0        0        0     6885 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.1/lowatt_grdf/main.py
+-rw-r--r--   0        0        0     7735 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.1/lowatt_grdf/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.1/lowatt_grdf/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.1/tests/__init__.py
+-rw-r--r--   0        0        0    16435 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.1/tests/test_api.py
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.1/tests/test_main.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.1/tests/test_models.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.1/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.1/LICENSE
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.1/README.md
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 lowatt_grdf-2.2.1/PKG-INFO
```

### Comparing `lowatt_grdf-2.2.0/.pre-commit-config.yaml` & `lowatt_grdf-2.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lowatt_grdf-2.2.0/staging-api-requests.md` & `lowatt_grdf-2.2.1/staging-api-requests.md`

 * *Files identical despite different names*

### Comparing `lowatt_grdf-2.2.0/.github/workflows/tox.yml` & `lowatt_grdf-2.2.1/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `lowatt_grdf-2.2.0/lowatt_grdf/__init__.py` & `lowatt_grdf-2.2.1/lowatt_grdf/__init__.py`

 * *Files identical despite different names*

### Comparing `lowatt_grdf-2.2.0/lowatt_grdf/api.py` & `lowatt_grdf-2.2.1/lowatt_grdf/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,19 @@
         raise NotImplementedError()
 
     @property
     @abc.abstractmethod
     def api(self) -> str:
         raise NotImplementedError()
 
+    @property
+    @abc.abstractmethod
+    def _auth_endpoint(self) -> str:
+        raise NotImplementedError()
+
     def __init__(self, client_id: str, client_secret: str):
         self.client_id = client_id
         self.client_secret = client_secret
         self._access_token: Optional[str] = None
         self._last_request: Optional[float] = None
         self._access_expires: Optional[float] = None
 
@@ -84,28 +89,20 @@
     put = functools.partialmethod(request, "PUT")
 
     @property
     def access_token(self) -> str:
         if self._access_token is None or (
             self._access_expires is not None and self._access_expires < time.time()
         ):
-            self._access_token, self._access_expires = (
-                self._authenticate_with_fallback()
-            )
+            self._access_token, self._access_expires = self._authenticate()
         return self._access_token
 
-    def _authenticate_with_fallback(self) -> tuple[str, float]:
-        try:
-            return self._authenticate(auth_endpoint=NEW_AUTH_ENDPOINT)
-        except requests.exceptions.HTTPError:
-            return self._authenticate(auth_endpoint=OLD_AUTH_ENDPOINT)
-
-    def _authenticate(self, auth_endpoint: str) -> tuple[str, float]:
+    def _authenticate(self) -> tuple[str, float]:
         resp = requests.post(
-            auth_endpoint,
+            self._auth_endpoint,
             data={
                 "grant_type": "client_credentials",
                 "client_id": self.client_id,
                 "client_secret": self.client_secret,
                 "scope": self.scope,
             },
         )
@@ -240,16 +237,17 @@
         return payload
 
 
 class StagingAPI(BaseAPI):
     scope = "/adict/bas/v6"
     api = "https://api.grdf.fr/adict/bas/v6"
 
-    def _authenticate_with_fallback(self) -> tuple[str, float]:
-        return self._authenticate(auth_endpoint=OLD_AUTH_ENDPOINT)
+    @property
+    def _auth_endpoint(self) -> str:
+        return OLD_AUTH_ENDPOINT
 
     def _parse_response(self, resp: requests.Response) -> Any:
         # XXX: Adjusts GRDF API responses to fit ndjson expected input because
         # GRDF Staging API v6 responses contain multiple-lines JSON objects
         # whereas ndjson expects one-line JSON objects
         return ndjson.loads(resp.text.replace("\n", "").replace("}{", "}\n{"))
 
@@ -265,7 +263,13 @@
             },
         )
 
 
 class API(BaseAPI):
     scope = "/adict/v2"
     api = "https://api.grdf.fr/adict/v2"
+
+    @property
+    def _auth_endpoint(self) -> str:
+        if self.client_id.endswith("_grdf"):
+            return OLD_AUTH_ENDPOINT
+        return NEW_AUTH_ENDPOINT
```

### Comparing `lowatt_grdf-2.2.0/lowatt_grdf/main.py` & `lowatt_grdf-2.2.1/lowatt_grdf/main.py`

 * *Files identical despite different names*

### Comparing `lowatt_grdf-2.2.0/lowatt_grdf/models.py` & `lowatt_grdf-2.2.1/lowatt_grdf/models.py`

 * *Files identical despite different names*

### Comparing `lowatt_grdf-2.2.0/tests/test_api.py` & `lowatt_grdf-2.2.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `lowatt_grdf-2.2.0/tests/test_main.py` & `lowatt_grdf-2.2.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `lowatt_grdf-2.2.0/tests/test_models.py` & `lowatt_grdf-2.2.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `lowatt_grdf-2.2.0/LICENSE` & `lowatt_grdf-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lowatt_grdf-2.2.0/README.md` & `lowatt_grdf-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lowatt_grdf-2.2.0/pyproject.toml` & `lowatt_grdf-2.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lowatt_grdf-2.2.0/PKG-INFO` & `lowatt_grdf-2.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: lowatt-grdf
-Version: 2.2.0
+Version: 2.2.1
 Summary: Python client for GRDF ADICT API
 Project-URL: Source, https://github.com/lowatt/lowatt-grdf
 Project-URL: Tracker, https://github.com/lowatt/lowatt-grdf/issues
 Author-email: Lowatt <info@lowatt.fr>
 License: GPLv3
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
```

