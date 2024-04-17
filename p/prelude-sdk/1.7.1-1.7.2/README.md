# Comparing `tmp/prelude-sdk-1.7.1.tar.gz` & `tmp/prelude_sdk-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-sdk-1.7.1.tar", last modified: Tue Apr  9 20:52:02 2024, max compression
+gzip compressed data, was "prelude_sdk-1.7.2.tar", last modified: Wed Apr 17 18:50:02 2024, max compression
```

## Comparing `prelude-sdk-1.7.1.tar` & `prelude_sdk-1.7.2.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-09 20:52:02.601940 prelude-sdk-1.7.1/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-sdk-1.7.1/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)     1163 2024-04-09 20:52:02.601780 prelude-sdk-1.7.1/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      697 2023-04-11 22:16:02.000000 prelude-sdk-1.7.1/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-09 20:52:02.592973 prelude-sdk-1.7.1/prelude_sdk/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.7.1/prelude_sdk/__init__.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-09 20:52:02.596385 prelude-sdk-1.7.1/prelude_sdk/controllers/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.7.1/prelude_sdk/controllers/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     5859 2024-04-09 20:41:12.000000 prelude-sdk-1.7.1/prelude_sdk/controllers/build_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     6376 2024-04-09 20:41:12.000000 prelude-sdk-1.7.1/prelude_sdk/controllers/detect_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      958 2024-04-09 20:41:12.000000 prelude-sdk-1.7.1/prelude_sdk/controllers/generate_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     7692 2024-04-09 20:41:12.000000 prelude-sdk-1.7.1/prelude_sdk/controllers/iam_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     3581 2024-04-09 20:41:12.000000 prelude-sdk-1.7.1/prelude_sdk/controllers/partner_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      443 2024-04-09 20:41:12.000000 prelude-sdk-1.7.1/prelude_sdk/controllers/probe_controller.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-09 20:52:02.597579 prelude-sdk-1.7.1/prelude_sdk/models/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.7.1/prelude_sdk/models/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2816 2023-07-11 13:50:29.000000 prelude-sdk-1.7.1/prelude_sdk/models/account.py
--rw-r--r--   0 pack       (501) staff       (20)     4642 2024-04-09 20:41:14.000000 prelude-sdk-1.7.1/prelude_sdk/models/codes.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-09 20:52:02.601459 prelude-sdk-1.7.1/prelude_sdk.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)     1163 2024-04-09 20:52:02.000000 prelude-sdk-1.7.1/prelude_sdk.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      799 2024-04-09 20:52:02.000000 prelude-sdk-1.7.1/prelude_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2024-04-09 20:52:02.000000 prelude-sdk-1.7.1/prelude_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)        9 2024-04-09 20:52:02.000000 prelude-sdk-1.7.1/prelude_sdk.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       12 2024-04-09 20:52:02.000000 prelude-sdk-1.7.1/prelude_sdk.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-sdk-1.7.1/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      532 2024-04-09 20:52:02.602232 prelude-sdk-1.7.1/setup.cfg
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-09 20:52:02.600237 prelude-sdk-1.7.1/tests/
--rw-r--r--   0 pack       (501) staff       (20)     1258 2024-03-01 18:30:16.000000 prelude-sdk-1.7.1/tests/conftest.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-09 20:52:02.601175 prelude-sdk-1.7.1/tests/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.7.1/tests/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     8164 2024-04-03 22:19:39.000000 prelude-sdk-1.7.1/tests/test_build.py
--rw-r--r--   0 pack       (501) staff       (20)     5018 2024-03-12 19:51:09.000000 prelude-sdk-1.7.1/tests/test_detect.py
--rw-r--r--   0 pack       (501) staff       (20)     7801 2024-04-03 22:19:39.000000 prelude-sdk-1.7.1/tests/test_iam.py
--rw-r--r--   0 pack       (501) staff       (20)    12179 2024-03-01 18:30:16.000000 prelude-sdk-1.7.1/tests/test_partner.py
--rw-r--r--   0 pack       (501) staff       (20)     3857 2024-03-12 19:51:09.000000 prelude-sdk-1.7.1/tests/test_probe.py
--rw-r--r--   0 pack       (501) staff       (20)      971 2024-03-01 18:30:16.000000 prelude-sdk-1.7.1/tests/testutils.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-17 18:50:02.366851 prelude_sdk-1.7.2/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude_sdk-1.7.2/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)     1163 2024-04-17 18:50:02.366769 prelude_sdk-1.7.2/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      697 2023-04-11 22:16:02.000000 prelude_sdk-1.7.2/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-17 18:50:02.359145 prelude_sdk-1.7.2/prelude_sdk/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude_sdk-1.7.2/prelude_sdk/__init__.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-17 18:50:02.362801 prelude_sdk-1.7.2/prelude_sdk/controllers/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude_sdk-1.7.2/prelude_sdk/controllers/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     6020 2024-04-17 18:29:22.000000 prelude_sdk-1.7.2/prelude_sdk/controllers/build_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     6626 2024-04-17 18:29:22.000000 prelude_sdk-1.7.2/prelude_sdk/controllers/detect_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     1080 2024-04-17 18:29:22.000000 prelude_sdk-1.7.2/prelude_sdk/controllers/generate_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      580 2024-04-17 18:29:22.000000 prelude_sdk-1.7.2/prelude_sdk/controllers/http_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     8288 2024-04-17 18:29:22.000000 prelude_sdk-1.7.2/prelude_sdk/controllers/iam_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     3727 2024-04-17 18:29:22.000000 prelude_sdk-1.7.2/prelude_sdk/controllers/partner_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      559 2024-04-17 18:29:22.000000 prelude_sdk-1.7.2/prelude_sdk/controllers/probe_controller.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-17 18:50:02.363653 prelude_sdk-1.7.2/prelude_sdk/models/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude_sdk-1.7.2/prelude_sdk/models/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2816 2023-07-11 13:50:29.000000 prelude_sdk-1.7.2/prelude_sdk/models/account.py
+-rw-r--r--   0 pack       (501) staff       (20)     4642 2024-04-11 16:14:14.000000 prelude_sdk-1.7.2/prelude_sdk/models/codes.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-17 18:50:02.366496 prelude_sdk-1.7.2/prelude_sdk.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)     1163 2024-04-17 18:50:02.000000 prelude_sdk-1.7.2/prelude_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      865 2024-04-17 18:50:02.000000 prelude_sdk-1.7.2/prelude_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2024-04-17 18:50:02.000000 prelude_sdk-1.7.2/prelude_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)        9 2024-04-17 18:50:02.000000 prelude_sdk-1.7.2/prelude_sdk.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       12 2024-04-17 18:50:02.000000 prelude_sdk-1.7.2/prelude_sdk.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude_sdk-1.7.2/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      532 2024-04-17 18:50:02.367107 prelude_sdk-1.7.2/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-17 18:50:02.365904 prelude_sdk-1.7.2/tests/
+-rw-r--r--   0 pack       (501) staff       (20)     5494 2024-04-17 18:29:22.000000 prelude_sdk-1.7.2/tests/conftest.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-04-17 18:50:02.366074 prelude_sdk-1.7.2/tests/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude_sdk-1.7.2/tests/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)    10423 2024-04-17 18:29:22.000000 prelude_sdk-1.7.2/tests/test_build.py
+-rw-r--r--   0 pack       (501) staff       (20)     5991 2024-04-17 18:29:22.000000 prelude_sdk-1.7.2/tests/test_detect.py
+-rw-r--r--   0 pack       (501) staff       (20)     1936 2024-04-17 18:29:22.000000 prelude_sdk-1.7.2/tests/test_generate.py
+-rw-r--r--   0 pack       (501) staff       (20)     8372 2024-04-17 18:29:22.000000 prelude_sdk-1.7.2/tests/test_iam.py
+-rw-r--r--   0 pack       (501) staff       (20)    12997 2024-04-17 18:29:22.000000 prelude_sdk-1.7.2/tests/test_partner.py
+-rw-r--r--   0 pack       (501) staff       (20)     4587 2024-04-17 18:29:22.000000 prelude_sdk-1.7.2/tests/test_probe.py
+-rw-r--r--   0 pack       (501) staff       (20)     2073 2024-04-17 18:29:22.000000 prelude_sdk-1.7.2/tests/testutils.py
```

### Comparing `prelude-sdk-1.7.1/LICENSE` & `prelude_sdk-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.7.1/PKG-INFO` & `prelude_sdk-1.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 1.7.1
+Version: 1.7.2
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-sdk-1.7.1/README.md` & `prelude_sdk-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.7.1/prelude_sdk/controllers/build_controller.py` & `prelude_sdk-1.7.2/prelude_sdk/controllers/build_controller.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import requests
 
+from prelude_sdk.controllers.http_controller import HttpController
+
 from prelude_sdk.models.account import verify_credentials
 from prelude_sdk.models.codes import Control
 
 
-class BuildController:
+class BuildController(HttpController):
 
     def __init__(self, account):
+        super().__init__()
         self.account = account
 
     @verify_credentials
     def create_test(self, name, unit, technique=None, test_id=None):
         """ Create or update a test """
         body = dict(name=name, unit=unit)
         if technique:
             body['technique'] = technique
         if test_id:
             body['id'] = test_id
 
-        res = requests.post(
+        res = self._session.post(
             f'{self.account.hq}/build/tests',
             json=body,
             headers=self.account.headers,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
@@ -35,28 +38,28 @@
         if name:
             body['name'] = name
         if unit:
             body['unit'] = unit
         if technique is not None:
             body['technique'] = technique
 
-        res = requests.post(
+        res = self._session.post(
             f'{self.account.hq}/build/tests/{test_id}',
             json=body,
             headers=self.account.headers,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
     def delete_test(self, test_id, purge):
         """ Delete an existing test """
-        res = requests.delete(
+        res = self._session.delete(
             f'{self.account.hq}/build/tests/{test_id}',
             json=dict(purge=purge),
             headers=self.account.headers,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
@@ -65,15 +68,15 @@
     @verify_credentials
     def upload(self, test_id, filename, data):
         """ Upload a test or attachment """
         if len(data) > 1000000:
             raise ValueError(f'File size must be under 1MB ({filename})')
 
         h = self.account.headers | {'Content-Type': 'application/octet-stream'}
-        res = requests.post(
+        res = self._session.post(
             f'{self.account.hq}/build/tests/{test_id}/{filename}',
             data=data,
             headers=h,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
@@ -88,15 +91,15 @@
         if source_id:
             body['source_id'] = source_id
         if source:
             body['source'] = source
         if tests:
             body['tests'] = tests
 
-        res = requests.post(
+        res = self._session.post(
             f'{self.account.hq}/build/threats',
             json=body,
             headers=self.account.headers,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
@@ -113,28 +116,28 @@
         if source is not None:
             body['source'] = source
         if published is not None:
             body['published'] = published
         if tests is not None:
             body['tests'] = tests
 
-        res = requests.post(
+        res = self._session.post(
             f'{self.account.hq}/build/threats/{threat_id}',
             json=body,
             headers=self.account.headers,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
     def delete_threat(self, threat_id, purge):
         """ Delete an existing threat """
-        res = requests.delete(
+        res = self._session.delete(
             f'{self.account.hq}/build/threats/{threat_id}',
             json=dict(purge=purge),
             headers=self.account.headers,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
@@ -145,15 +148,15 @@
         """ Create a detection """
         body = dict(rule=rule, test_id=test_id)
         if detection_id:
             body['detection_id'] = detection_id
         if rule_id:
             body['rule_id'] = rule_id
 
-        res = requests.post(
+        res = self._session.post(
             f'{self.account.hq}/build/detections',
             json=body,
             headers=self.account.headers,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
@@ -164,28 +167,28 @@
         """ Update a detection """
         body = dict()
         if rule:
             body['rule'] = rule
         if test_id:
             body['test_id'] = test_id
 
-        res = requests.post(
+        res = self._session.post(
             f'{self.account.hq}/build/detections/{detection_id}',
             json=body,
             headers=self.account.headers,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
     def delete_detection(self, detection_id: str):
         """ Delete an existing detection """
-        res = requests.delete(
+        res = self._session.delete(
             f'{self.account.hq}/build/detections/{detection_id}',
             headers=self.account.headers,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
```

### Comparing `prelude-sdk-1.7.1/prelude_sdk/controllers/detect_controller.py` & `prelude_sdk-1.7.2/prelude_sdk/controllers/detect_controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import requests
 
+from prelude_sdk.controllers.http_controller import HttpController
+
 from prelude_sdk.models.account import verify_credentials
 from prelude_sdk.models.codes import RunCode
 
 
-class DetectController:
+class DetectController(HttpController):
 
     def __init__(self, account):
+        super().__init__()
         self.account = account
 
     @verify_credentials
     def register_endpoint(self, host, serial_num, tags=None):
         """ Register (or re-register) an endpoint to your account """
         body = dict(id=f'{host}:{serial_num}')
         if tags:
             body['tags'] = tags
 
-        res = requests.post(
+        res = self._session.post(
             f'{self.account.hq}/detect/endpoint',
             headers=self.account.headers,
             json=body,
             timeout=10
         )
         if res.status_code == 200:
             return res.text
@@ -29,144 +32,145 @@
     @verify_credentials
     def update_endpoint(self, endpoint_id, tags=None):
         """ Update an endpoint in your account """
         body = dict()
         if tags is not None:
             body['tags'] = tags
 
-        res = requests.post(
+        res = self._session.post(
             f'{self.account.hq}/detect/endpoint/{endpoint_id}',
             headers=self.account.headers,
             json=body,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
     def delete_endpoint(self, ident: str):
         """ Delete an endpoint from your account """
         params = dict(id=ident)
-        res = requests.delete(
+        res = self._session.delete(
             f'{self.account.hq}/detect/endpoint',
             headers=self.account.headers,
             json=params,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
     def list_endpoints(self, days: int = 90):
         """ List all endpoints on your account """
         params = dict(days=days)
-        res = requests.get(
+        res = self._session.get(
             f'{self.account.hq}/detect/endpoint',
             headers=self.account.headers,
             params=params,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
     def describe_activity(self, filters: dict, view: str = 'protected'):
         """ Get report for an Account """
         params = dict(view=view, **filters)
-        res = requests.get(
+        res = self._session.get(
             f'{self.account.hq}/detect/activity',
             headers=self.account.headers,
             params=params,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
-    def list_tests(self):
+    def list_tests(self, filters: dict = None):
         """ List all tests available to an account """
-        res = requests.get(
+        res = self._session.get(
             f'{self.account.hq}/detect/tests',
             headers=self.account.headers,
+            params=filters if filters else {},
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
     def get_test(self, test_id):
         """ Get properties of an existing test """
-        res = requests.get(
+        res = self._session.get(
             f'{self.account.hq}/detect/tests/{test_id}',
             headers=self.account.headers,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
     def list_threats(self):
         """ List threats """
-        res = requests.get(
+        res = self._session.get(
             f'{self.account.hq}/detect/threats',
             headers=self.account.headers,
             params={},
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
     def get_threat(self, threat_id):
         """ Get properties of an existing threat """
-        res = requests.get(
+        res = self._session.get(
             f'{self.account.hq}/detect/threats/{threat_id}',
             headers=self.account.headers,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
     def list_detections(self):
         """ List detections """
-        res = requests.get(
+        res = self._session.get(
             f'{self.account.hq}/detect/detections',
             headers=self.account.headers,
             params={},
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
     def get_detection(self, detection_id):
         """ Get properties of an existing detection """
-        res = requests.get(
+        res = self._session.get(
             f'{self.account.hq}/detect/detections/{detection_id}',
             headers=self.account.headers,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
     def download(self, test_id, filename):
         """ Clone a test file or attachment"""
-        res = requests.get(
+        res = self._session.get(
             f'{self.account.hq}/detect/tests/{test_id}/{filename}',
             headers=self.account.headers,
             timeout=10
         )
         if res.status_code == 200:
             return res.content
         raise Exception(res.text)
@@ -174,15 +178,15 @@
     @verify_credentials
     def schedule(self, items: list):
         """ Schedule tests and threats so endpoints will start running them
 
         Example: items=[dict(run_code='DAILY', tags='grp-1,grp2', test_id='123-123-123'),
                         dict(run_code='DAILY', tags='grp-1', threat_id='abc-def-ghi')]
         """
-        res = requests.post(
+        res = self._session.post(
             url=f'{self.account.hq}/detect/queue',
             headers=self.account.headers,
             json=dict(items=items),
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
@@ -191,15 +195,15 @@
     @verify_credentials
     def unschedule(self, items: list):
         """ Unschedule tests and threats so endpoints will stop running them
 
         Example: items=[dict(tags='grp-1,grp2', test_id='123-123-123'),
                         dict(tags='grp-1', threat_id='abc-def-ghi')]
         """
-        res = requests.delete(
+        res = self._session.delete(
             f'{self.account.hq}/detect/queue',
             headers=self.account.headers,
             json=dict(items=items),
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
```

### Comparing `prelude-sdk-1.7.1/prelude_sdk/controllers/generate_controller.py` & `prelude_sdk-1.7.2/prelude_sdk/controllers/generate_controller.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 import requests
+
+from prelude_sdk.controllers.http_controller import HttpController
+
 from prelude_sdk.models.account import verify_credentials
 
 
-class GenerateController:
+class GenerateController(HttpController):
     def __init__(self, account):
+        super().__init__()
         self.account = account
 
     @verify_credentials
     def upload_threat_intel(self, file: str):
         with open(file, 'rb') as f:
             body = f.read()
-        res = requests.post(
+        res = self._session.post(
             f'{self.account.hq}/generate/threat-intel',
             data=body,
             headers=self.account.headers | {'Content-Type': 'application/pdf'},
             timeout=30
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
     def get_threat_intel(self, job_id: str):
-        res = requests.get(
+        res = self._session.get(
             f'{self.account.hq}/generate/threat-intel/{job_id}',
             headers=self.account.headers,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
```

### Comparing `prelude-sdk-1.7.1/prelude_sdk/controllers/iam_controller.py` & `prelude_sdk-1.7.2/prelude_sdk/controllers/iam_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 import requests
 import datetime
 
+from prelude_sdk.controllers.http_controller import HttpController
+
 from prelude_sdk.models.codes import AuditEvent, Mode, Permission
 from prelude_sdk.models.account import verify_credentials
 
 
-class IAMController:
+class IAMController(HttpController):
 
     def __init__(self, account):
+        super().__init__()
         self.account = account
 
     @verify_credentials
     def new_account(self, user_email: str, user_name: str = None, company: str = None, slug: str = None):
         body = dict(handle=user_email)
         if user_name:
             body['user_name'] = user_name
         if company:
             body['company'] = company
         if slug:
             body['slug'] = slug
 
-        res = requests.post(
+        res = self._session.post(
             url=f'{self.account.hq}/iam/account',
             json=body,
             headers=self.account.headers,
             timeout=10
         )
         if res.status_code != 200:
             raise Exception(res.text)
@@ -35,15 +38,15 @@
         cfg[self.account.profile]['token'] = res_json['token']
         self.account.write_keychain_config(cfg)
         return res_json
 
     @verify_credentials
     def purge_account(self):
         """ Delete an account and all things in it """
-        res = requests.delete(
+        res = self._session.delete(
             f'{self.account.hq}/iam/account',
             headers=self.account.headers,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
@@ -55,15 +58,15 @@
         if mode is not None:
             body['mode'] = mode.name
         if company is not None:
             body['company'] = company
         if slug is not None:
             body['slug'] = slug
 
-        res = requests.put(
+        res = self._session.put(
             f'{self.account.hq}/iam/account',
             headers=self.account.headers,
             json=body,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
@@ -75,40 +78,40 @@
         body = dict(
             issuer=issuer,
             client_id=client_id,
             client_secret=client_secret,
             oidc_config_url=oidc_config_url
         )
 
-        res = requests.post(
+        res = self._session.post(
             f'{self.account.hq}/iam/account/oidc',
             headers=self.account.headers,
             json=body,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
     def detach_oidc(self):
         """ Detach OIDC to an account """
-        res = requests.delete(
+        res = self._session.delete(
             f'{self.account.hq}/iam/account/oidc',
             headers=self.account.headers,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
     def get_account(self):
         """ Get account properties """
-        res = requests.get(
+        res = self._session.get(
             f'{self.account.hq}/iam/account',
             headers=self.account.headers,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
@@ -118,15 +121,15 @@
         """ Create a new user inside an account """
         body = dict(permission=permission.name, handle=email, oidc=oidc)
         if name:
             body['name'] = name
         if expires:
             body['expires'] = expires.isoformat()
 
-        res = requests.post(
+        res = self._session.post(
             url=f'{self.account.hq}/iam/user',
             json=body,
             headers=self.account.headers,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
@@ -141,28 +144,28 @@
         if expires:
             body['expires'] = expires.isoformat()
         if name is not None:
             body['name'] = name
         if oidc is not None:
             body['oidc'] = oidc
 
-        res = requests.put(
+        res = self._session.put(
             f'{self.account.hq}/iam/user',
             json=body,
             headers=self.account.headers,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
     def delete_user(self, handle):
         """ Delete a user from an account """
-        res = requests.delete(
+        res = self._session.delete(
             f'{self.account.hq}/iam/user',
             json=dict(handle=handle),
             headers=self.account.headers,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
@@ -171,28 +174,28 @@
     @verify_credentials
     def reset_password(self, email: str, account_id: str = None):
         """ Reset a user's password """
         data = dict(
             account_id=account_id or self.account.headers['account'],
             handle=email
         )
-        res = requests.post(
+        res = self._session.post(
             f'{self.account.hq}/iam/user/reset',
             json=data,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
     def verify_user(self, token: str):
         """ Verify a user """
         params = dict(token=token, request_credentials='true')
-        res = requests.get(
+        res = self._session.get(
             f'{self.account.hq}/iam/user',
             params=params,
             timeout=10
         )
         if res.status_code == 200:
             cfg = self.account.read_keychain_config()
             res_json = res.json()
@@ -202,40 +205,53 @@
             return res_json
         raise Exception(res.text)
 
     @verify_credentials
     def audit_logs(self, days: int = 7, limit: int = 1000):
         """ Get audit logs from the last X days """
         params = dict(days=days, limit=limit)
-        res = requests.get(
+        res = self._session.get(
             f'{self.account.hq}/iam/audit',
             headers=self.account.headers,
             params=params,
             timeout=30
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
     def subscribe(self, event: AuditEvent):
         """ Subscribe to email notifications for an event """
-        res = requests.post(
+        res = self._session.post(
             f'{self.account.hq}/iam/subscribe/{event.name}',
             headers=self.account.headers,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
     def unsubscribe(self, event: AuditEvent):
         """ Unsubscribe to email notifications for an event """
-        res = requests.delete(
+        res = self._session.delete(
             f'{self.account.hq}/iam/subscribe/{event.name}',
             headers=self.account.headers,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
+
+    @verify_credentials
+    def accept_terms(self, name, version):
+        """ Accept terms and conditions """
+        res = self._session.post(
+            f'{self.account.hq}/iam/terms',
+            headers=self.account.headers,
+            json=dict(name=name, version=version),
+            timeout=10
+        )
+        if res.status_code == 200:
+            return res.json()
+        raise Exception(res.text)
```

### Comparing `prelude-sdk-1.7.1/prelude_sdk/controllers/partner_controller.py` & `prelude_sdk-1.7.2/prelude_sdk/controllers/partner_controller.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,103 +1,106 @@
 import requests
 
+from prelude_sdk.controllers.http_controller import HttpController
+
 from prelude_sdk.models.codes import Control
 from prelude_sdk.models.account import verify_credentials
 
 
-class PartnerController:
+class PartnerController(HttpController):
 
     def __init__(self, account):
+        super().__init__()
         self.account = account
 
     @verify_credentials
     def attach(self, partner: Control, api: str, user: str, secret: str):
         """ Attach a partner to your account """
         params = dict(api=api, user=user, secret=secret)
-        res = requests.post(
+        res = self._session.post(
             f'{self.account.hq}/partner/{partner.name}',
             headers=self.account.headers,
             json=params,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
     def detach(self, partner: Control):
         """ Detach a partner from your Detect account """
-        res = requests.delete(
+        res = self._session.delete(
             f'{self.account.hq}/partner/{partner.name}',
             headers=self.account.headers,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
     def block(self, partner: Control, test_id: str):
         """ Report to a partner to block a test """
         params = dict(test_id=test_id)
-        res = requests.post(
+        res = self._session.post(
             f'{self.account.hq}/partner/block/{partner.name}',
             headers=self.account.headers,
             json=params,
             timeout=30
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
         
     @verify_credentials
     def endpoints(self, partner: Control, platform: str, hostname: str = '', offset: int = 0, count: int = 100):
         """ Get a list of endpoints from a partner """
         params = dict(platform=platform, hostname=hostname, offset=offset, count=count)
-        res = requests.get(
+        res = self._session.get(
             f'{self.account.hq}/partner/endpoints/{partner.name}',
             headers=self.account.headers,
             params=params,
             timeout=30
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
     def generate_webhook(self, partner: Control):
         """ Generate webhook credentials for an EDR system to enable the forwarding of alerts to the Prelude API, facilitating automatic alert suppression """
-        res = requests.get(
+        res = self._session.get(
             f'{self.account.hq}/partner/suppress/{partner.name}',
             headers=self.account.headers,
             timeout=30
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
     def deploy(self, partner: Control, host_ids: list):
         """ Deploy probes on all specified partner endpoints """
         params = dict(host_ids=host_ids)
-        res = requests.post(
+        res = self._session.post(
             f'{self.account.hq}/partner/deploy/{partner.name}',
             headers=self.account.headers,
             json=params,
             timeout=30
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
     def list_reports(self, partner: Control, test_id: str):
         """ Get reports to a partner for a test """
         params = dict(test_id=test_id)
-        res = requests.get(
+        res = self._session.get(
             f'{self.account.hq}/partner/reports/{partner.name}',
             headers=self.account.headers,
             json=params,
             timeout=30
         )
         if res.status_code == 200:
             return res.json()
```

### Comparing `prelude-sdk-1.7.1/prelude_sdk/models/account.py` & `prelude_sdk-1.7.2/prelude_sdk/models/account.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.7.1/prelude_sdk/models/codes.py` & `prelude_sdk-1.7.2/prelude_sdk/models/codes.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.7.1/prelude_sdk.egg-info/PKG-INFO` & `prelude_sdk-1.7.2/prelude_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 1.7.1
+Version: 1.7.2
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-sdk-1.7.1/prelude_sdk.egg-info/SOURCES.txt` & `prelude_sdk-1.7.2/prelude_sdk.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -8,21 +8,23 @@
 prelude_sdk.egg-info/dependency_links.txt
 prelude_sdk.egg-info/requires.txt
 prelude_sdk.egg-info/top_level.txt
 prelude_sdk/controllers/__init__.py
 prelude_sdk/controllers/build_controller.py
 prelude_sdk/controllers/detect_controller.py
 prelude_sdk/controllers/generate_controller.py
+prelude_sdk/controllers/http_controller.py
 prelude_sdk/controllers/iam_controller.py
 prelude_sdk/controllers/partner_controller.py
 prelude_sdk/controllers/probe_controller.py
 prelude_sdk/models/__init__.py
 prelude_sdk/models/account.py
 prelude_sdk/models/codes.py
 tests/conftest.py
 tests/test_build.py
 tests/test_detect.py
+tests/test_generate.py
 tests/test_iam.py
 tests/test_partner.py
 tests/test_probe.py
 tests/testutils.py
 tests/templates/__init__.py
```

### Comparing `prelude-sdk-1.7.1/setup.cfg` & `prelude_sdk-1.7.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-sdk
-version = 1.7.1
+version = 1.7.2
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers =
```

### Comparing `prelude-sdk-1.7.1/tests/test_build.py` & `prelude_sdk-1.7.2/tests/test_build.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,187 +1,168 @@
 import json
 import os
 import pytest
 import time
-import uuid
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 from importlib.resources import files
 
 from dateutil.parser import parse
 
 from prelude_sdk.controllers.build_controller import BuildController
 from prelude_sdk.controllers.detect_controller import DetectController
 
 import templates
 from testutils import *
 
 
 @pytest.mark.order(2)
-class TestBuild:
+@pytest.mark.usefixtures('setup_account', 'setup_test')
+class TestVST:
 
     def setup_class(self):
         self.build = BuildController(pytest.account)
         self.detect = DetectController(pytest.account)
 
-        self.test_id = str(uuid.uuid4())
-        self.name = 'test'
-        self.unit = 'custom'
-        self.technique = 'T1234.001'
-
-    def test_create_test(self, unwrap, email):
-        res = unwrap(self.build.create_test)(self.build, test_id=self.test_id, name=self.name, unit=self.unit)
-
-        pytest.test_id = self.test_id
-        pytest.expected_test = dict(
+    def test_create_test(self):
+        expected = dict(
             account_id=pytest.account.headers['account'],
-            author=email,
-            id=self.test_id,
-            name=self.name,
-            unit=self.unit,
+            author=pytest.expected_account['whoami'],
+            id=pytest.test_id,
+            name='test_name',
+            unit='custom',
             technique=None,
             attachments=[],
             tombstoned=None
         )
 
-        diffs = check_dict_items(pytest.expected_test, res)
+        diffs = check_dict_items(expected, pytest.expected_test)
         assert not diffs, json.dumps(diffs, indent=2)
 
     def test_upload(self, unwrap):
         template = files(templates).joinpath('template.go').read_text()
-        res = unwrap(self.build.upload)(self.build, test_id=self.test_id, filename=f'{self.test_id}.go',
+        res = unwrap(self.build.upload)(self.build, test_id=pytest.test_id, filename=f'{pytest.test_id}.go',
                                         data=template.encode("utf-8"))
 
         expected = dict(
-            id=self.test_id,
-            filename=f'{self.test_id}.go'
+            id=pytest.test_id,
+            filename=f'{pytest.test_id}.go'
         )
         assert expected == res
 
         pytest.expected_test['attachments'].append(res['filename'])
 
     def test_get_test(self, unwrap):
         def wait_for_compile():
             timeout = time.time() + 60
             while time.time() < timeout:
                 time.sleep(6)
-                res = unwrap(self.detect.get_test)(self.detect, test_id=self.test_id)
+                res = unwrap(self.detect.get_test)(self.detect, test_id=pytest.test_id)
                 if len(res['attachments']) == 6:
                     break
                 # Hack to clear test from cache
-                unwrap(self.build.update_test)(self.build, test_id=self.test_id, name=self.name)
+                unwrap(self.build.update_test)(self.build, test_id=pytest.test_id, name=pytest.expected_test['name'])
             return
 
         wait_for_compile()
         for suffix in ['darwin-arm64', 'darwin-x86_64', 'linux-arm64', 'linux-x86_64', 'windows-x86_64']:
-            pytest.expected_test['attachments'].append(f'{self.test_id}_{suffix}')
-        res = unwrap(self.detect.get_test)(self.detect, test_id=self.test_id)
+            pytest.expected_test['attachments'].append(f'{pytest.test_id}_{suffix}')
+        res = unwrap(self.detect.get_test)(self.detect, test_id=pytest.test_id)
 
         diffs = check_dict_items(pytest.expected_test, res)
         assert not diffs, json.dumps(diffs, indent=2)
 
     def test_list_tests(self, unwrap):
         res = unwrap(self.detect.list_tests)(self.detect)
         owners = set([r['account_id'] for r in res])
-        assert owners == {'prelude', pytest.account.headers['account']}
+        assert {'prelude', pytest.account.headers['account']} >= owners
 
-        mine = [r for r in res if r['account_id'] == pytest.account.headers['account']]
+        mine = [r for r in res if r['id'] == pytest.expected_test['id']]
         assert 1 == len(mine)
         del pytest.expected_test['attachments']
         diffs = check_dict_items(pytest.expected_test, mine[0])
         assert not diffs, json.dumps(diffs, indent=2)
 
     def test_update_test(self, unwrap):
         updated_name = 'updated_test'
-        res = unwrap(self.build.update_test)(self.build, test_id=self.test_id, name=updated_name, technique=self.technique)
+        res = unwrap(self.build.update_test)(self.build, test_id=pytest.test_id, name=updated_name, technique='T1234.001')
 
         pytest.expected_test['name'] = updated_name
-        pytest.expected_test['technique'] = self.technique
+        pytest.expected_test['technique'] = 'T1234.001'
 
         diffs = check_dict_items(pytest.expected_test, res)
         assert not diffs, json.dumps(diffs, indent=2)
 
     def test_download(self, unwrap):
-        filename = f'{self.test_id}.go'
-        res = unwrap(self.detect.download)(self.detect, test_id=self.test_id, filename=filename)
+        filename = f'{pytest.test_id}.go'
+        res = unwrap(self.detect.download)(self.detect, test_id=pytest.test_id, filename=filename)
         assert res is not None
         with open(filename, 'wb') as f:
             f.write(res)
         assert os.path.isfile(filename)
         os.remove(filename)
 
     @pytest.mark.order(-2)
     def test_delete_test(self, unwrap):
         unwrap(self.build.delete_test)(self.build, test_id=pytest.test_id, purge=False)
         res = unwrap(self.detect.get_test)(self.detect, test_id=pytest.test_id)
         pytest.expected_test['tombstoned'] = res['tombstoned']
 
         diffs = check_dict_items(pytest.expected_test, res)
         assert not diffs, json.dumps(diffs, indent=2)
-        assert parse(res['tombstoned']) <= datetime.utcnow() + timedelta(minutes=1)
+        assert parse(res['tombstoned']).replace(tzinfo=timezone.utc) <= datetime.now(timezone.utc) + timedelta(minutes=1)
 
         unwrap(self.build.delete_test)(self.build, test_id=pytest.test_id, purge=True)
         with pytest.raises(Exception):
             unwrap(self.detect.get_test)(self.detect, test_id=pytest.test_id)
 
 
 @pytest.mark.order(3)
+@pytest.mark.usefixtures('setup_account', 'setup_test', 'setup_threat')
 class TestThreat:
 
     def setup_class(self):
         self.build = BuildController(pytest.account)
         self.detect = DetectController(pytest.account)
 
-        self.threat_id = str(uuid.uuid4())
-        self.name = 'threat'
-        self.published = '2023-11-13'
-        self.source_id = 'aa23-061a'
-        self.source = 'https://www.cisa.gov/news-events/cybersecurity-advisories/aa23-061a'
-        self.tests = ['881f9052-fb52-4daf-9ad2-0a7ad9615baf', 'b74ad239-2ddd-4b1e-b608-8397a43c7c54', pytest.test_id]
-
-    def test_create_threat(self, unwrap, email):
-        res = unwrap(self.build.create_threat)(self.build, name=self.name, published=self.published,
-                                               threat_id=self.threat_id, source_id=self.source_id, source=self.source,
-                                               tests=','.join(self.tests))
-
-        pytest.threat_id = self.threat_id
-        pytest.expected_threat = dict(
+    def test_create_threat(self):
+        expected = dict(
             account_id=pytest.account.headers['account'],
-            author=email,
-            id=self.threat_id,
-            source_id=self.source_id,
-            name=self.name,
-            source=self.source,
-            published=self.published,
-            tests=self.tests,
+            author=pytest.expected_account['whoami'],
+            id=pytest.threat_id,
+            source_id='aa23-061a',
+            name='threat_name',
+            source='https://www.cisa.gov/news-events/cybersecurity-advisories/aa23-061a',
+            published='2023-11-13',
+            tests=['881f9052-fb52-4daf-9ad2-0a7ad9615baf', 'b74ad239-2ddd-4b1e-b608-8397a43c7c54', pytest.test_id],
             tombstoned=None
         )
 
-        diffs = check_dict_items(pytest.expected_threat, res)
+        diffs = check_dict_items(expected, pytest.expected_threat)
         assert not diffs, json.dumps(diffs, indent=2)
 
     def test_get_threat(self, unwrap):
-        res = unwrap(self.detect.get_threat)(self.detect, threat_id=self.threat_id)
+        res = unwrap(self.detect.get_threat)(self.detect, threat_id=pytest.threat_id)
 
         diffs = check_dict_items(pytest.expected_threat, res)
         assert not diffs, json.dumps(diffs, indent=2)
 
     def test_list_threats(self, unwrap):
         res = unwrap(self.detect.list_threats)(self.detect)
         owners = set([r['account_id'] for r in res])
-        assert owners == {'prelude', pytest.account.headers['account']}
+        assert {'prelude', pytest.account.headers['account']} >= owners
 
-        mine = [r for r in res if r['account_id'] == pytest.account.headers['account']]
+        mine = [r for r in res if r['id'] == pytest.expected_threat['id']]
         assert 1 == len(mine)
         diffs = check_dict_items(pytest.expected_threat, mine[0])
         assert not diffs, json.dumps(diffs, indent=2)
 
     def test_update_threat(self, unwrap):
         updated_name = 'updated-threat'
-        updated_tests = ['881f9052-fb52-4daf-9ad2-0a7ad9615baf', 'b74ad239-2ddd-4b1e-b608-8397a43c7c54']
-        res = unwrap(self.build.update_threat)(self.build, threat_id=self.threat_id, name=updated_name, source='',
+        updated_tests = ['881f9052-fb52-4daf-9ad2-0a7ad9615baf', '74077d3b-6a2f-49fa-903e-99cad6f34cf6', 'b74ad239-2ddd-4b1e-b608-8397a43c7c54']
+        res = unwrap(self.build.update_threat)(self.build, threat_id=pytest.threat_id, name=updated_name, source='',
                                                tests=','.join(updated_tests))
 
         pytest.expected_threat['name'] = updated_name
         pytest.expected_threat['source'] = None
         pytest.expected_threat['tests'] = updated_tests
 
         diffs = check_dict_items(pytest.expected_threat, res)
@@ -191,12 +172,73 @@
     def test_delete_threat(self, unwrap):
         unwrap(self.build.delete_threat)(self.build, threat_id=pytest.threat_id, purge=False)
         res = unwrap(self.detect.get_threat)(self.detect, threat_id=pytest.threat_id)
         pytest.expected_threat['tombstoned'] = res['tombstoned']
 
         diffs = check_dict_items(pytest.expected_threat, res)
         assert not diffs, json.dumps(diffs, indent=2)
-        assert parse(res['tombstoned']) <= datetime.utcnow() + timedelta(minutes=1)
+        assert parse(res['tombstoned']).replace(tzinfo=timezone.utc) <= datetime.now(timezone.utc) + timedelta(minutes=1)
 
         unwrap(self.build.delete_threat)(self.build, threat_id=pytest.threat_id, purge=True)
         with pytest.raises(Exception):
             unwrap(self.detect.get_threat)(self.detect, threat_id=pytest.threat_id)
+
+
+@pytest.mark.order(4)
+@pytest.mark.usefixtures('setup_account', 'setup_test', 'setup_detection')
+class TestDetection:
+
+    def setup_class(self):
+        if not pytest.expected_account['features']['detections']:
+            pytest.skip("DETECTIONS feature not enabled")
+
+        self.build = BuildController(pytest.account)
+        self.detect = DetectController(pytest.account)
+
+    def test_create_detection(self, unwrap):
+        expected = dict(
+            account_id=pytest.account.headers['account'],
+            id=pytest.detection_id,
+            name='Suspicious Command Line Usage in Windows',
+            rule=dict(
+                title='Suspicious Command Line Usage in Windows',
+                description='Detects suspicious use of cmd.exe or powershell.exe with commands often used for reconnaissance like directory listing, tree viewing, or searching for sensitive files.',
+                logsource=dict(category='process_creation', product='windows'),
+                detection=dict(condition='selection', selection=dict(ParentImage='cmd.exe')),
+                level='medium'
+            ),
+            rule_id=pytest.expected_detection['rule_id'],
+            test=pytest.test_id
+        )
+
+        diffs = check_dict_items(expected, pytest.expected_detection)
+        assert not diffs, json.dumps(diffs, indent=2)
+
+    def test_get_detection(self, unwrap):
+        res = unwrap(self.detect.get_detection)(self.detect, detection_id=pytest.detection_id)
+
+        diffs = check_dict_items(pytest.expected_detection, res)
+        assert not diffs, json.dumps(diffs, indent=2)
+
+    def test_list_detections(self, unwrap):
+        res = unwrap(self.detect.list_detections)(self.detect)
+        owners = set([r['account_id'] for r in res])
+        assert {'prelude', pytest.account.headers['account']} >= owners
+
+        mine = [r for r in res if r['id'] == pytest.expected_detection['id']]
+        assert 1 == len(mine)
+        diffs = check_dict_items(pytest.expected_detection, mine[0])
+        assert not diffs, json.dumps(diffs, indent=2)
+
+    def test_update_detection(self, unwrap):
+        updated_rule = pytest.detection_rule.replace(pytest.expected_detection['rule']['title'], 'Suspicious no more')
+        res = unwrap(self.build.update_detection)(self.build, detection_id=pytest.detection_id, rule=updated_rule)
+        pytest.expected_detection['rule']['title'] = 'Suspicious no more'
+
+        diffs = check_dict_items(pytest.expected_detection, res)
+        assert not diffs, json.dumps(diffs, indent=2)
+
+    @pytest.mark.order(-4)
+    def test_delete_detection(self, unwrap):
+        unwrap(self.build.delete_detection)(self.build, detection_id=pytest.detection_id)
+        with pytest.raises(Exception):
+            unwrap(self.detect.get_detection)(self.detect, detection_id=pytest.detection_id)
```

### Comparing `prelude-sdk-1.7.1/tests/test_detect.py` & `prelude_sdk-1.7.2/tests/test_detect.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import json
 import pytest
 import requests
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 
 from dateutil.parser import parse
 from testutils import *
 
 from prelude_sdk.controllers.detect_controller import DetectController
 from prelude_sdk.controllers.iam_controller import IAMController
 from prelude_sdk.models.codes import RunCode
 
 
-@pytest.mark.order(4)
+@pytest.mark.order(5)
+@pytest.mark.usefixtures('setup_account', 'setup_test', 'setup_threat')
 class TestDetect:
 
     def setup_class(self):
         self.iam = IAMController(pytest.account)
         self.detect = DetectController(pytest.account)
 
         self.host = 'test_host'
@@ -39,16 +40,16 @@
             os=None,
             policy=None,
             policy_name=None
         )
 
     def test_list_endpoints(self, unwrap):
         res = unwrap(self.detect.list_endpoints)(self.detect)
-        assert len(res) == 1
-        ep = res[0]
+        assert 1 <= len(res)
+        ep = [r for r in res if r['serial_num'] == self.serial][0]
         pytest.expected_endpoint['endpoint_id'] = ep['endpoint_id']
         pytest.endpoint_id = ep['endpoint_id']
 
         diffs = check_dict_items(pytest.expected_endpoint, ep)
         assert not diffs, json.dumps(diffs, indent=2)
         assert parse(ep['last_seen']).date() == parse(ep['created']).date()
 
@@ -58,64 +59,77 @@
         pytest.expected_endpoint['tags'] = [self.updated_tags]
 
         res = unwrap(self.detect.list_endpoints)(self.detect)
         diffs = check_dict_items(pytest.expected_endpoint, res[0])
         assert not diffs, json.dumps(diffs, indent=2)
 
     def test_schedule_threat(self, unwrap):
+        queue_length = len(pytest.expected_account['queue'])
+
         res = unwrap(self.detect.schedule)(self.detect, [dict(threat_id=pytest.threat_id, run_code=RunCode.DAILY.name)])
+        pytest.expected_account['queue'].append(res[0])
         assert 1 == len(res), json.dumps(res, indent=2)
         diffs = check_dict_items(dict(threat=pytest.threat_id, run_code=RunCode.DAILY.value, tag=None), res[0])
         assert not diffs, json.dumps(diffs, indent=2)
 
-        queue = unwrap(self.iam.get_account)(self.iam)['queue']
-        assert 1 == len(queue), json.dumps(queue, indent=2)
+        queue = sorted(unwrap(self.iam.get_account)(self.iam)['queue'], key=lambda x: x['started'], reverse=True)
+        assert queue_length + 1 == len(queue), json.dumps(queue, indent=2)
         expected = dict(
             threat=pytest.threat_id,
             run_code=RunCode.DAILY.value
         )
         diffs = check_dict_items(expected, queue[0])
         assert not diffs, json.dumps(diffs, indent=2)
 
     def test_unschedule_threat(self, unwrap):
+        queue_length = len(pytest.expected_account['queue'])
+
         unwrap(self.detect.unschedule)(self.detect, [dict(threat_id=pytest.threat_id)])
+        pytest.expected_account['queue'] = [q for q in pytest.expected_account['queue'] if q['threat'] != pytest.threat_id]
         queue = unwrap(self.iam.get_account)(self.iam)['queue']
-        assert 0 == len(queue), json.dumps(queue, indent=2)
+        assert queue_length - 1 == len(queue), json.dumps(queue, indent=2)
 
     def test_schedule_test(self, unwrap):
+        queue_length = len(pytest.expected_account['queue'])
+
         res = unwrap(self.detect.schedule)(self.detect, [dict(test_id=pytest.test_id, run_code=RunCode.DEBUG.name, tags=self.updated_tags)])
+        pytest.expected_account['queue'].append(res[0])
         assert 1 == len(res), json.dumps(res, indent=2)
         diffs = check_dict_items(dict(test=pytest.test_id, run_code=RunCode.DEBUG.value, tag=self.updated_tags), res[0])
         assert not diffs, json.dumps(diffs, indent=2)
 
-        queue = unwrap(self.iam.get_account)(self.iam)['queue']
-        assert 1 == len(queue), json.dumps(queue, indent=2)
+        queue = sorted(unwrap(self.iam.get_account)(self.iam)['queue'], key=lambda x: x['started'], reverse=True)
+        assert queue_length + 1 == len(queue), json.dumps(queue, indent=2)
         expected = dict(
             test=pytest.test_id,
             run_code=RunCode.DEBUG.value,
             tag=self.updated_tags
         )
         diffs = check_dict_items(expected, queue[0])
         assert not diffs, json.dumps(diffs, indent=2)
 
     def test_unschedule_test(self, unwrap):
+        queue_length = len(pytest.expected_account['queue'])
+
         unwrap(self.detect.unschedule)(self.detect, [dict(test_id=pytest.test_id, tags=self.updated_tags)])
+        pytest.expected_account['queue'] = [q for q in pytest.expected_account['queue'] if q['test'] != pytest.test_id]
         queue = unwrap(self.iam.get_account)(self.iam)['queue']
-        assert 0 == len(queue), json.dumps(queue, indent=2)
+        assert queue_length - 1 == len(queue), json.dumps(queue, indent=2)
 
     def test_describe_activity(self, unwrap, api):
         res = requests.get(api, headers=dict(token=pytest.token, dos=f'darwin-x86_64', dat=f'{pytest.test_id}:100',
                                              version='2.1'))
         assert res.status_code in [200, 302]
         filters = dict(
-            start=datetime.utcnow() - timedelta(days=7),
-            finish=datetime.utcnow() + timedelta(days=1),
+            start=datetime.now(timezone.utc) - timedelta(days=1),
+            finish=datetime.now(timezone.utc) + timedelta(days=1),
             endpoints=pytest.endpoint_id
         )
         res = unwrap(self.detect.describe_activity)(self.detect, view='logs', filters=filters)
         assert 1 == len(res), json.dumps(res, indent=2)
 
     def test_delete_endpoint(self, unwrap):
         unwrap(self.detect.delete_endpoint)(self.detect, ident=pytest.endpoint_id)
         res = unwrap(self.detect.list_endpoints)(self.detect)
-        assert 0 == len(res), json.dumps(res, indent=2)
+        ep = [r for r in res if r['serial_num'] == self.serial]
+        assert 0 == len(ep), json.dumps(ep, indent=2)
```

### Comparing `prelude-sdk-1.7.1/tests/test_iam.py` & `prelude_sdk-1.7.2/tests/test_iam.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,187 +1,193 @@
 import json
-import time
 import pytest
 
+from datetime import datetime, timedelta, timezone
 from dateutil.parser import parse
-from datetime import datetime, timedelta
-from prelude_sdk.models.codes import AuditEvent, Mode, Permission, RunCode
 from prelude_sdk.controllers.iam_controller import IAMController
+from prelude_sdk.models.codes import AuditEvent, Mode, Permission, RunCode
 
 from testutils import *
 
 
-class Account:
-    def __init__(self, account_id='', token='', hq=''):
-        self.hq = hq
-        self.profile = 'test'
-        self.headers = dict(
-            account=account_id,
-            token=token,
-            _product='py-sdk'
-        )
-
-    def read_keychain_config(self):
-        return {self.profile: dict()}
-
-    def write_keychain_config(self, cfg):
-        pass
-
-
 @pytest.mark.order(1)
+@pytest.mark.usefixtures('setup_account')
 class TestIAM:
 
     def setup_class(self):
-        self.iam = IAMController(Account())
+        self.iam = IAMController(pytest.account)
 
         self.company = 'prelude'
         self.second_user = 'registration'
+        self.subscription_event = AuditEvent.CREATE_USER
 
-    def test_new_account(self, unwrap, manual, pause_for_manual_action, email, api):
-        pytest.account = Account(hq=api)
-        self.iam.account = pytest.account
-        res = unwrap(self.iam.new_account)(self.iam, user_email=email, user_name='Bob')
-        if manual:
-            with pause_for_manual_action:
-                input("Press ENTER to continue testing after verifying the account...\n")
-        else:
-            time.sleep(5)
-        assert 32 == len(res['account_id'])
-        assert email == res['handle']
-        assert check_if_string_is_uuid(res['token'])
+    def test_new_account(self, email, existing_account):
+        if existing_account:
+            pytest.skip("Pre-existing account")
 
-        pytest.account.headers['account'] = res['account_id']
-        pytest.account.headers['token'] = res['token']
-        print(f'[account_id: {res["account_id"]}]', end=' ')
+        created = pytest.expected_account
+
+        assert 32 == len(pytest.account.headers['account'])
+        assert check_if_string_is_uuid(pytest.account.headers['token'])
+        assert email == created['whoami']
 
         pytest.expected_account = dict(
-            account_id=res['account_id'],
+            account_id=created['account_id'],
             whoami=email,
-            slug=res['account_id'],
+            slug=created['account_id'],
             company='',
             mode=Mode.AUTOPILOT.value,
             controls=[],
             users=[
                 dict(
                     handle=email,
                     permission=Permission.ADMIN.value,
                     name='Bob',
                     subscriptions=[],
-                    oidc=False
-                )
-            ],
-            queue=[
-                dict(
-                    run_code=RunCode.SMART.value,
-                    tag='autopilot'
+                    oidc=False,
+                    terms={},
                 )
             ],
             probe_sleep='600s',
             oidc=dict(),
             features=dict(
                 oidc=False,
                 threat_intel=False,
                 detections=False
             )
         )
+        pytest.expected_account['users'][0]['expires'] = created['users'][0]['expires']
+        pytest.expected_account['queue'] = created['queue']
+        if created['queue']:
+            assert 'autopilot' == created['queue'][0]['tag']
+            assert RunCode.SMART.value == created['queue'][0]['run_code']
+
+    def test_account_subscribe(self, unwrap):
+        res = unwrap(self.iam.subscribe)(self.iam, event=self.subscription_event)
+
+        for user in pytest.expected_account['users']:
+            if user['handle'] == pytest.expected_account['whoami']:
+                user['subscriptions'].append(self.subscription_event.value)
+                self.expected_subs = user['subscriptions']
+                break
 
-    def test_account_subscribe(self, unwrap, manual, email):
-        if not manual:
-            pytest.skip("Not manual mode")
-
-        res = unwrap(self.iam.subscribe)(self.iam, event=AuditEvent.CREATE_USER)
         expected = dict(
-            email=email,
-            subscriptions=[AuditEvent.CREATE_USER.value]
+            email=pytest.expected_account['whoami'],
+            subscriptions=self.expected_subs
         )
         diffs = check_dict_items(expected, res)
         assert not diffs, json.dumps(diffs, indent=2)
 
-        pytest.expected_account['users'][0]['subscriptions'] = res['subscriptions']
-
-    def test_get_account(self, unwrap, manual):
+    def test_get_account(self, unwrap):
         res = unwrap(self.iam.get_account)(self.iam)
         diffs = check_dict_items(pytest.expected_account, res)
         assert not diffs, json.dumps(diffs, indent=2)
-        if manual:
-            assert parse(res['users'][0]['expires']) >= datetime.utcnow() + timedelta(days=364)
-        else:
-            assert parse(res['users'][0]['expires']) <= datetime.utcnow() + timedelta(days=1)
 
     def test_create_user(self, unwrap):
+        ex = datetime.now(timezone.utc) + timedelta(days=1)
         res = unwrap(self.iam.create_user)(self.iam, email=self.second_user, permission=Permission.SERVICE, name='Rob',
-                                      expires=(datetime.utcnow() + timedelta(days=1)))
+                                           expires=ex)
         assert self.second_user == res['handle']
         assert check_if_string_is_uuid(res['token'])
 
-
         res = unwrap(self.iam.get_account)(self.iam)
 
-        pytest.second_user_index = 0 if res['users'][0]['name'] == 'Rob' else 1
-        pytest.expected_account['users'].insert(pytest.second_user_index,
-                                                dict(
-                                                    handle=self.second_user,
-                                                    permission=Permission.SERVICE.value,
-                                                    name='Rob',
-                                                    subscriptions=[],
-                                                    oidc=False
-                                                )
+        pytest.expected_account['users'].append(
+            dict(
+                handle=self.second_user,
+                permission=Permission.SERVICE.value,
+                name='Rob',
+                subscriptions=[],
+                oidc=False,
+                terms={},
+                expires=ex.isoformat()
+            )
         )
 
         diffs = check_dict_items(pytest.expected_account, res)
         assert not diffs, json.dumps(diffs, indent=2)
-        assert parse(res['users'][1]['expires']) <= datetime.utcnow() + timedelta(days=1)
 
-    def test_account_unsubscribe(self, unwrap, manual, email):
-        if not manual:
-            pytest.skip("Not manual mode")
+    def test_account_unsubscribe(self, unwrap):
+        res = unwrap(self.iam.unsubscribe)(self.iam, event=self.subscription_event)
+
+        for user in pytest.expected_account['users']:
+            if user['handle'] == pytest.expected_account['whoami']:
+                user['subscriptions'].remove(self.subscription_event.value)
+                self.expected_subs = user['subscriptions']
+                break
 
-        res = unwrap(self.iam.unsubscribe)(self.iam, event=AuditEvent.CREATE_USER)
         expected = dict(
-            email=email,
-            subscriptions=[]
+            email=pytest.expected_account['whoami'],
+            subscriptions=self.expected_subs
         )
         diffs = check_dict_items(expected, res)
         assert not diffs, json.dumps(diffs, indent=2)
 
-        pytest.expected_account['users'][0]['subscriptions'] = res['subscriptions']
-
     def test_update_user(self, unwrap):
-        unwrap(self.iam.update_user)(self.iam, email=self.second_user, name='Robb',
-                                     expires=(datetime.utcnow() + timedelta(days=365)))
-        pytest.expected_account['users'][pytest.second_user_index]['name'] = 'Robb'
+        ex = datetime.now(timezone.utc) + timedelta(days=365)
+        unwrap(self.iam.update_user)(self.iam, email=self.second_user, name='Robb', expires=ex)
+
+        for i, user in enumerate(pytest.expected_account['users']):
+            if user['handle'] == self.second_user:
+                user['name'] = 'Robb'
+                user['expires'] = ex.isoformat()
+                break
 
         res = unwrap(self.iam.get_account)(self.iam)
         diffs = check_dict_items(pytest.expected_account, res)
         assert not diffs, json.dumps(diffs, indent=2)
-        assert parse(res['users'][pytest.second_user_index]['expires']) >= datetime.utcnow() + timedelta(days=360)
+
+    def test_accept_terms(self, unwrap):
+        for user in pytest.expected_account['users']:
+            if user['handle'] == pytest.expected_account['whoami']:
+                if user['terms'].get('threat_intel', {}).get('1.0.0'):
+                    with pytest.raises(Exception) as e:
+                        unwrap(self.iam.accept_terms)(self.iam, name='threat_intel', version='1.0.0')
+                    return
+
+        unwrap(self.iam.accept_terms)(self.iam, name='threat_intel', version='1.0.0')
+        res = unwrap(self.iam.get_account)(self.iam)
+
+        for user in res['users']:
+            if user['handle'] == pytest.expected_account['whoami']:
+                assert user['terms'].get('threat_intel', {}).get('1.0.0'), json.dumps(user, indent=2)
+                assert parse(user['terms']['threat_intel']['1.0.0']) <= datetime.now(timezone.utc)
+                break
+
+        pytest.expected_account['users'] = res['users']
 
     def test_delete_user(self, unwrap):
         unwrap(self.iam.delete_user)(self.iam, handle=self.second_user)
-        del pytest.expected_account['users'][pytest.second_user_index]
+
+        for i, user in enumerate(pytest.expected_account['users']):
+            if user['handle'] == self.second_user:
+                break
+        del pytest.expected_account['users'][i]
 
         res = unwrap(self.iam.get_account)(self.iam)
         diffs = check_dict_items(pytest.expected_account, res)
         assert not diffs, json.dumps(diffs, indent=2)
 
     def test_update_account(self, unwrap):
         unwrap(self.iam.update_account)(self.iam, mode=Mode.MANUAL, company=self.company)
         pytest.expected_account['mode'] = Mode.MANUAL.value
         pytest.expected_account['company'] = self.company
-        pytest.expected_account['queue'] = []
+        autopilot = [i for i, item in enumerate(pytest.expected_account['queue']) if item['tag'] == 'autopilot']
+        for i in sorted(autopilot, reverse=True):
+            del pytest.expected_account['queue'][i]
 
         res = unwrap(self.iam.get_account)(self.iam)
         diffs = check_dict_items(pytest.expected_account, res)
         assert not diffs, json.dumps(diffs, indent=2)
 
-    def test_audit_logs(self, unwrap, email):
+    def test_audit_logs(self, unwrap):
         res = unwrap(self.iam.audit_logs)(self.iam, limit=1)[0]
         expected = dict(
             event='update_account',
-            user_id=email,
+            user_id=pytest.expected_account['whoami'],
             status='200',
             values=dict(mode=Mode.MANUAL.name, company=self.company),
             account_id=pytest.expected_account['account_id']
         )
         diffs = check_dict_items(expected, res)
         assert not diffs, json.dumps(diffs, indent=2)
 
@@ -195,10 +201,13 @@
         res = unwrap(self.iam.verify_user)(self.iam, token=token)
         assert pytest.expected_account['account_id'] == res['account']
         assert check_if_string_is_uuid(res['token'])
 
         pytest.account.headers['token'] = res['token']
 
     @pytest.mark.order(-1)
-    def test_purge_account(self, unwrap):
+    def test_purge_account(self, unwrap, existing_account):
+        if existing_account:
+            pytest.skip("Pre-existing account")
+
         iam = IAMController(pytest.account)
         unwrap(iam.purge_account)(iam)
```

### Comparing `prelude-sdk-1.7.1/tests/test_partner.py` & `prelude_sdk-1.7.2/tests/test_partner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import json
 import pytest
 import requests
 
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 from prelude_sdk.models.codes import Control
 from prelude_sdk.controllers.iam_controller import IAMController
 from prelude_sdk.controllers.detect_controller import DetectController
 from prelude_sdk.controllers.partner_controller import PartnerController
 
 from testutils import *
 
@@ -69,15 +69,16 @@
             if not all([scenario[1][k] for k in ['partner_api', 'user', 'secret']]):
                 argvalues.append(pytest.param(*[x[1] for x in items], marks=pytest.mark.skip('Creds not supplied')))
             else:
                 argvalues.append([x[1] for x in items])
         metafunc.parametrize(argnames, argvalues, ids=idlist, scope="class")
 
 
-@pytest.mark.order(5)
+@pytest.mark.order(6)
+@pytest.mark.usefixtures('setup_account', 'setup_test', 'setup_detection')
 class TestPartner:
     scenarios = [crowdstrike, defender, sentinel_one]
 
     def setup_class(self):
         self.iam = IAMController(pytest.account)
         self.detect = DetectController(pytest.account)
         self.partner = PartnerController(pytest.account)
@@ -97,16 +98,16 @@
 
         # Create endpoint after attach
         unwrap(self.detect.register_endpoint)(self.detect, host=host, serial_num=host + '2')
         pytest.endpoint_2 = pytest.endpoint_1 | dict(serial_num=host + '2')
 
     def test_get_account(self, unwrap, host, edr_id, control, os, platform, policy, policy_name, partner_api, user, secret, webhook_keys):
         res = unwrap(self.iam.get_account)(self.iam)
-        expected = [dict(api=partner_api, id=control.value)]
-        assert expected == res['controls']
+        expected = dict(api=partner_api, id=control.value)
+        assert expected in res['controls']
 
     def test_list_endpoints(self, unwrap, host, edr_id, control, os, platform, policy, policy_name, partner_api, user, secret, webhook_keys):
         try:
             res = unwrap(self.detect.list_endpoints)(self.detect)
             assert len(res) >= 2
             sorted_res = {r['serial_num']: r for r in res}
             pytest.endpoint_1['endpoint_id'] = sorted_res[pytest.endpoint_1['serial_num']]['endpoint_id']
@@ -130,16 +131,16 @@
     def test_activity_logs(self, unwrap, api, host, edr_id, control, os, platform, policy, policy_name, partner_api, user, secret, webhook_keys):
         res = requests.get(api, headers=dict(token=pytest.token, dos=f'{platform}-x86_64', dat=f'{pytest.test_id}:100',
                                              version='2.1'))
         assert res.status_code in [200, 302]
         pytest.endpoint_1['dos'] = f'{platform}-x86_64'
 
         filters = dict(
-            start=datetime.utcnow() - timedelta(days=7),
-            finish=datetime.utcnow() + timedelta(days=1),
+            start=datetime.now(timezone.utc) - timedelta(days=7),
+            finish=datetime.now(timezone.utc) + timedelta(days=1),
             endpoints=pytest.endpoint_1['endpoint_id']
         )
         res = unwrap(self.detect.describe_activity)(self.detect, view='logs', filters=filters)
         assert len(res) == 1, json.dumps(res, indent=2)
         expected = dict(
             test=pytest.test_id,
             endpoint_id=pytest.endpoint_1['endpoint_id'],
@@ -154,29 +155,41 @@
 
     def test_generate_webhook(self, unwrap, api, host, edr_id, control, os, platform, policy, policy_name, partner_api, user, secret, webhook_keys):
         res = unwrap(self.partner.generate_webhook)(self.partner, partner=control)
         assert webhook_keys == res.keys()
         assert res['url'].startswith(f'{api}/partner/suppress/{control.name.lower()}')
 
     def test_block(self, unwrap, host, edr_id, control, os, platform, policy, policy_name, partner_api, user, secret, webhook_keys):
+        if control == Control.CROWDSTRIKE and not pytest.expected_account['features']['detections']:
+            pytest.skip("DETECTIONS feature not enabled")
+
         res = unwrap(self.partner.block)(self.partner, partner=control, test_id=pytest.test_id)
-        assert len(res) == 5
-        assert {'file', 'ioc_id'} == res[0].keys()
-        assert res[0]['file'].startswith(pytest.test_id)
+        if control == Control.CROWDSTRIKE:
+            assert 1 == len(res)
+            assert pytest.expected_detection['rule']['logsource']['product'] == res[0]['platform']
+            assert 1 == len(res[0]['rules'])
+            assert f'{pytest.expected_detection["rule"]["title"]} ({pytest.detection_id[:8]}) (0)' == res[0]['rules'][0]['name']
+            assert res[0]['rules'][0]['status'] in ['ALREADY_EXISTS', 'CREATED']
+        else:
+            assert len(res) == 5
+            assert {'file', 'ioc_id'} == res[0].keys()
+            assert res[0]['file'].startswith(pytest.test_id)
 
     def test_detach(self, unwrap, host, edr_id, control, os, platform, policy, policy_name, partner_api, user, secret, webhook_keys):
         try:
             unwrap(self.partner.detach)(self.partner, partner=control)
             res = unwrap(self.iam.get_account)(self.iam)
-            assert res['controls'] == []
+            for c in res['controls']:
+                assert c['id'] != control.value
         finally:
             unwrap(self.detect.delete_endpoint)(self.detect, ident=pytest.endpoint_1['endpoint_id'])
 
 
-@pytest.mark.order(6)
+@pytest.mark.order(7)
+@pytest.mark.usefixtures('setup_account')
 class TestSiems:
 
     def setup_class(self):
         self.iam = IAMController(pytest.account)
         self.detect = DetectController(pytest.account)
         self.partner = PartnerController(pytest.account)
 
@@ -230,43 +243,44 @@
         expected = dict(api=bucket, connected=True)
         assert expected == res
 
         pytest.expected_siems.append(dict(api=bucket, id=Control.S3.value))
 
     def test_get_account(self, unwrap):
         res = unwrap(self.iam.get_account)(self.iam)
-        assert pytest.expected_siems == res['controls']
+        for c in pytest.expected_siems:
+            assert c in res['controls']
 
     def test_save_result(self, unwrap, api):
         try:
-            res = requests.get(api, headers=dict(token=pytest.token, dos=f'linux-x86_64', dat=f'{pytest.test_id}:101',
+            res = requests.get(api, headers=dict(token=pytest.token, dos=f'linux-x86_64', dat='b74ad239-2ddd-4b1e-b608-8397a43c7c54:101',
                                                  version='2.1'))
             assert res.status_code in [200, 302]
         finally:
             unwrap(self.detect.delete_endpoint)(self.detect, ident=pytest.endpoint_id)
 
     def test_detach_splunk(self, unwrap):
         if not self.splunk:
             pytest.skip("Creds not supplied")
 
         unwrap(self.partner.detach)(self.partner, partner=Control.SPLUNK)
         res = unwrap(self.iam.get_account)(self.iam)
-        del pytest.expected_siems[0]
-        assert pytest.expected_siems == res['controls']
+        for c in res['controls']:
+            assert c['id'] != Control.SPLUNK.value
 
     def test_detach_vectr(self, unwrap):
         if not self.vectr:
             pytest.skip("Creds not supplied")
 
         unwrap(self.partner.detach)(self.partner, partner=Control.VECTR)
         res = unwrap(self.iam.get_account)(self.iam)
-        del pytest.expected_siems[0]
-        assert pytest.expected_siems == res['controls']
+        for c in res['controls']:
+            assert c['id'] != Control.VECTR.value
 
     def test_detach_s3(self, unwrap):
         if not self.s3:
             pytest.skip("Creds not supplied")
 
         unwrap(self.partner.detach)(self.partner, partner=Control.S3)
         res = unwrap(self.iam.get_account)(self.iam)
-        del pytest.expected_siems[0]
-        assert pytest.expected_siems == res['controls']
+        for c in res['controls']:
+            assert c['id'] != Control.S3.value
```

### Comparing `prelude-sdk-1.7.1/tests/test_probe.py` & `prelude_sdk-1.7.2/tests/test_probe.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import json
 import os
 import pytest
 import subprocess
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 
 from prelude_sdk.controllers.detect_controller import DetectController
 from prelude_sdk.controllers.iam_controller import IAMController
 from prelude_sdk.controllers.probe_controller import ProbeController
 from prelude_sdk.models.codes import RunCode
 
 
-@pytest.mark.order(7)
+@pytest.mark.order(8)
+@pytest.mark.usefixtures('setup_account', 'setup_test', 'setup_threat')
 class TestProbe:
 
     def setup_class(self):
         self.iam = IAMController(pytest.account)
         self.detect = DetectController(pytest.account)
         self.probe = ProbeController(pytest.account)
 
@@ -25,30 +26,32 @@
         pytest.token = unwrap(self.detect.register_endpoint)(self.detect, host=self.host, serial_num=self.serial)
 
         res = unwrap(self.detect.list_endpoints)(self.detect)
         ep = [r for r in res if r['serial_num'] == self.serial]
         pytest.endpoint_id = ep[0]['endpoint_id']
 
     def test_schedule(self, unwrap):
+        queue_len = len(pytest.expected_account['queue'])
         unwrap(self.detect.schedule)(
             self.detect,
             [
                 dict(test_id='9f410a6b-76b6-45d6-b80f-d7365add057e', run_code=RunCode.DEBUG.name, tags=''),
                 dict(test_id='b74ad239-2ddd-4b1e-b608-8397a43c7c54', run_code=RunCode.RUN_ONCE.name, tags=''),
-                # 2 tests in this threat (881.., b74...)
+                # 3 tests in this threat (881.., b74..., 740... or uuid)
                 dict(threat_id=pytest.threat_id, run_code=RunCode.DAILY.name, tags=''),
                 # windows only test
                 dict(test_id='f12d00db-571f-4c51-a536-12a3577b5a4b', run_code=RunCode.DEBUG.name, tags=''),
                 # should not run
                 dict(test_id='8f9558f3-d451-46e3-bdda-97378c1e8ce4', run_code=RunCode.DAILY.name, tags='diff-tag')
             ]
         )
 
         queue = unwrap(self.iam.get_account)(self.iam)['queue']
-        assert 5 == len(queue), json.dumps(queue, indent=2)
+        pytest.expected_account['queue'] = queue
+        assert queue_len + 5 == len(queue), json.dumps(queue, indent=2)
 
     def test_download_probe(self):
         probe_name = 'nocturnal'
         res = self.probe.download(name=probe_name, dos='darwin-arm64')
         assert res is not None
 
         with open(f'{probe_name}.sh', 'w') as f:
@@ -59,35 +62,41 @@
 
     def test_describe_activity(self, unwrap):
         try:
             with pytest.raises(subprocess.TimeoutExpired):
                 subprocess.run([pytest.probe_file], capture_output=True, env={'PRELUDE_TOKEN': pytest.token}, timeout=40)
 
             filters = dict(
-                start=datetime.utcnow() - timedelta(days=7),
-                finish=datetime.utcnow() + timedelta(days=1),
+                start=datetime.now(timezone.utc) - timedelta(days=1),
+                finish=datetime.now(timezone.utc) + timedelta(days=1),
                 endpoints=pytest.endpoint_id
             )
             res = unwrap(self.detect.describe_activity)(self.detect, view='logs', filters=filters)
-            assert 5 == len(res), json.dumps(res, indent=2)
+            assert 6 <= len(res), json.dumps(res, indent=2)
+            tests_run = {r['test'] for r in res}
+            queued_tests = ['9f410a6b-76b6-45d6-b80f-d7365add057e', 'b74ad239-2ddd-4b1e-b608-8397a43c7c54', 'f12d00db-571f-4c51-a536-12a3577b5a4b'] + pytest.expected_threat['tests']
+            assert set(queued_tests) <= tests_run, json.dumps(tests_run, indent=2)
         finally:
             os.remove(pytest.probe_file)
 
     def test_unschedule(self, unwrap):
+        queue_len = len(pytest.expected_account['queue'])
         unwrap(self.detect.unschedule)(
             self.detect,
             [
                 dict(test_id='9f410a6b-76b6-45d6-b80f-d7365add057e', tags=''),
                 dict(test_id='b74ad239-2ddd-4b1e-b608-8397a43c7c54', tags=''),
                 dict(threat_id=pytest.threat_id, tags=''),
                 dict(test_id='f12d00db-571f-4c51-a536-12a3577b5a4b', tags=''),
                 dict(test_id='8f9558f3-d451-46e3-bdda-97378c1e8ce4', tags='diff-tag')
             ]
         )
 
         queue = unwrap(self.iam.get_account)(self.iam)['queue']
-        assert 0 == len(queue), json.dumps(queue, indent=2)
+        pytest.expected_account['queue'] = queue
+        assert queue_len - 5 == len(queue), json.dumps(queue, indent=2)
 
     def test_delete_endpoint(self, unwrap):
         unwrap(self.detect.delete_endpoint)(self.detect, ident=pytest.endpoint_id)
         res = unwrap(self.detect.list_endpoints)(self.detect)
-        assert 0 == len(res), json.dumps(res, indent=2)
+        ep = [r for r in res if r['serial_num'] == self.serial]
+        assert 0 == len(ep), json.dumps(ep, indent=2)
```

