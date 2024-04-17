# Comparing `tmp/simple-mockforce-0.8.0.tar.gz` & `tmp/simple-mockforce-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-mockforce-0.8.0.tar", max compression
+gzip compressed data, was "simple-mockforce-0.8.1.tar", max compression
```

## Comparing `simple-mockforce-0.8.0.tar` & `simple-mockforce-0.8.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1064 2023-02-22 18:59:06.909618 simple-mockforce-0.8.0/LICENSE
--rw-r--r--   0        0        0     3824 2023-02-22 18:59:06.909618 simple-mockforce-0.8.0/README.md
--rw-r--r--   0        0        0      807 2023-02-22 18:59:06.909618 simple-mockforce-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     3029 2023-02-22 18:59:06.909618 simple-mockforce-0.8.0/simple_mockforce/__init__.py
--rw-r--r--   0        0        0     6847 2023-02-22 18:59:06.909618 simple-mockforce-0.8.0/simple_mockforce/callbacks.py
--rw-r--r--   0        0        0     1626 2023-02-22 18:59:06.909618 simple-mockforce-0.8.0/simple_mockforce/constants.py
--rw-r--r--   0        0        0       24 2023-02-22 18:59:06.909618 simple-mockforce-0.8.0/simple_mockforce/error_codes.py
--rw-r--r--   0        0        0      241 2023-02-22 18:59:06.909618 simple-mockforce-0.8.0/simple_mockforce/query_algorithms/__init__.py
--rw-r--r--   0        0        0      543 2023-02-22 18:59:06.909618 simple-mockforce-0.8.0/simple_mockforce/query_algorithms/date_token.py
--rw-r--r--   0        0        0     1305 2023-02-22 18:59:06.909618 simple-mockforce-0.8.0/simple_mockforce/query_algorithms/order_by.py
--rw-r--r--   0        0        0     1334 2023-02-22 18:59:06.909618 simple-mockforce-0.8.0/simple_mockforce/query_algorithms/parent_attrs.py
--rw-r--r--   0        0        0     5635 2023-02-22 18:59:06.909618 simple-mockforce-0.8.0/simple_mockforce/query_algorithms/where.py
--rw-r--r--   0        0        0     1471 2023-02-22 18:59:06.909618 simple-mockforce-0.8.0/simple_mockforce/utils.py
--rw-r--r--   0        0        0    12668 2023-02-22 18:59:06.909618 simple-mockforce-0.8.0/simple_mockforce/virtual.py
--rw-r--r--   0        0        0     4845 1970-01-01 00:00:00.000000 simple-mockforce-0.8.0/setup.py
--rw-r--r--   0        0        0     4784 1970-01-01 00:00:00.000000 simple-mockforce-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-17 20:15:22.133746 simple-mockforce-0.8.1/LICENSE
+-rw-r--r--   0        0        0     3824 2024-04-17 20:15:22.133746 simple-mockforce-0.8.1/README.md
+-rw-r--r--   0        0        0      807 2024-04-17 20:15:22.133746 simple-mockforce-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     3277 2024-04-17 20:15:22.133746 simple-mockforce-0.8.1/simple_mockforce/__init__.py
+-rw-r--r--   0        0        0     7540 2024-04-17 20:15:22.133746 simple-mockforce-0.8.1/simple_mockforce/callbacks.py
+-rw-r--r--   0        0        0     1683 2024-04-17 20:15:22.137745 simple-mockforce-0.8.1/simple_mockforce/constants.py
+-rw-r--r--   0        0        0       24 2024-04-17 20:15:22.137745 simple-mockforce-0.8.1/simple_mockforce/error_codes.py
+-rw-r--r--   0        0        0      241 2024-04-17 20:15:22.137745 simple-mockforce-0.8.1/simple_mockforce/query_algorithms/__init__.py
+-rw-r--r--   0        0        0      543 2024-04-17 20:15:22.137745 simple-mockforce-0.8.1/simple_mockforce/query_algorithms/date_token.py
+-rw-r--r--   0        0        0     1305 2024-04-17 20:15:22.137745 simple-mockforce-0.8.1/simple_mockforce/query_algorithms/order_by.py
+-rw-r--r--   0        0        0     1334 2024-04-17 20:15:22.137745 simple-mockforce-0.8.1/simple_mockforce/query_algorithms/parent_attrs.py
+-rw-r--r--   0        0        0     5635 2024-04-17 20:15:22.137745 simple-mockforce-0.8.1/simple_mockforce/query_algorithms/where.py
+-rw-r--r--   0        0        0     1676 2024-04-17 20:15:22.137745 simple-mockforce-0.8.1/simple_mockforce/utils.py
+-rw-r--r--   0        0        0    12668 2024-04-17 20:15:22.137745 simple-mockforce-0.8.1/simple_mockforce/virtual.py
+-rw-r--r--   0        0        0     4845 1970-01-01 00:00:00.000000 simple-mockforce-0.8.1/setup.py
+-rw-r--r--   0        0        0     4784 1970-01-01 00:00:00.000000 simple-mockforce-0.8.1/PKG-INFO
```

### Comparing `simple-mockforce-0.8.0/LICENSE` & `simple-mockforce-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-mockforce-0.8.0/README.md` & `simple-mockforce-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `simple-mockforce-0.8.0/pyproject.toml` & `simple-mockforce-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simple-mockforce"
-version = "0.8.0"
+version = "0.8.1"
 description = "A companion package for simple-salesforce that enables the testing of code that interacts with Salesforce's API"
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Kicksaw-Consulting/simple-mockforce"
 authors = ["Alex Drozd <drozdster@gmail.com>"]
 keywords = ["python", "simple-salesforce", "salesforce", "testing", "mocking"]
 packages = [
```

### Comparing `simple-mockforce-0.8.0/simple_mockforce/__init__.py` & `simple-mockforce-0.8.1/simple_mockforce/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 
 from decorator import decorator
 
 from simple_mockforce.callbacks import (
     bulk_callback,
     bulk_detail_callback,
     bulk_result_callback,
+    bulk_query_result_callback,
     create_callback,
     delete_callback,
     get_callback,
     job_callback,
     job_detail_callback,
     query_callback,
     query_all_callback,
     update_callback,
 )
 from simple_mockforce.constants import (
     BATCH_DETAIL_URL,
     BATCH_RESULT_URL,
+    BATCH_QUERY_RESULT_URL,
     CREATE_URL,
     JOB_DETAIL_URL,
     LOGIN_URL,
     OAUTH_RESPONSE,
     OAUTH_URL,
     SOAP_API_LOGIN_RESPONSE,
     DETAIL_URL,
@@ -92,14 +94,20 @@
         responses.GET,
         terminate_regex(BATCH_RESULT_URL),
         callback=bulk_result_callback,
         content_type="content/json",
     )
     responses.add_callback(
         responses.GET,
+        terminate_regex(BATCH_QUERY_RESULT_URL),
+        callback=bulk_query_result_callback,
+        content_type="content/json",
+    )
+    responses.add_callback(
+        responses.GET,
         terminate_regex(BATCH_DETAIL_URL),
         callback=bulk_detail_callback,
         content_type="content/json",
     )
     responses.add_callback(
         responses.POST,
         terminate_regex(BATCH_URL),
```

### Comparing `simple-mockforce-0.8.0/simple_mockforce/callbacks.py` & `simple-mockforce-0.8.1/simple_mockforce/callbacks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 
 from urllib.parse import urlparse
 
 from simple_mockforce.error_codes import NOT_FOUND
 from simple_mockforce.utils import (
     parse_batch_detail_url,
+    parse_batch_query_result_url,
     parse_batch_result_url,
     parse_detail_url,
     parse_create_url,
     parse_job_batch_url,
 )
 from simple_mockforce.virtual import virtual_salesforce
 
@@ -146,21 +147,26 @@
         json.dumps(job),
     )
 
 
 def bulk_callback(request):
     url = request.url
     path = urlparse(url).path
-    body = json.loads(request.body)
 
     job_id = parse_job_batch_url(path)
     job = virtual_salesforce.jobs[job_id]
     operation = job["operation"]
 
-    batch = virtual_salesforce.create_batch(job_id, body, operation)
+    if operation == "query":
+        # For testing purposes we only return one results set.
+        data = {"752x00000004CJE": virtual_salesforce.query(request.body)}
+    else:
+        data = json.loads(request.body)
+
+    batch = virtual_salesforce.create_batch(job_id, data, operation)
 
     return (
         201,
         {},
         json.dumps(batch),
     )
 
@@ -189,16 +195,26 @@
     path = urlparse(url).path
 
     job_id, batch_id = parse_batch_result_url(path)
 
     job = virtual_salesforce.jobs[job_id]
     sobject_name = job["object"]
     operation = job["operation"]
+
     data = virtual_salesforce.batch_data[batch_id]
 
+    if operation == "query":
+        return (
+            201,
+            {},
+            # Keys of the query data are result set ids
+            json.dumps(list(data.keys()))
+        )
+
+
     id_to_created = dict()
 
     duplicate_ids = set()
     sfdc_ids = list()
     for sobject in data:
         if operation == "upsert":
             external_field_id = job["externalIdFieldName"]
@@ -260,14 +276,27 @@
     return (
         201,
         {},
         json.dumps(fake_response),
     )
 
 
+def bulk_query_result_callback(request):
+    path = urlparse(request.url).path
+
+    _, batch_id, result_set_id = parse_batch_query_result_url(path)
+    data = virtual_salesforce.batch_data[batch_id][result_set_id]
+
+    return (
+        201,
+        {},
+        json.dumps(data),
+    )
+
+
 def job_detail_callback(request):
     """
     This is a no-op as far as we're concerned
     """
     return (
         201,
         {},
```

### Comparing `simple-mockforce-0.8.0/simple_mockforce/constants.py` & `simple-mockforce-0.8.1/simple_mockforce/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 BATCH_URL = f"{BASE_URL}/services/async/{SF_VERSION}/job/{SFDC_ID}/batch"
 BATCH_DETAIL_URL = (
     f"{BASE_URL}/services/async/{SF_VERSION}/job/{SFDC_ID}/batch/{SFDC_ID}"
 )
 BATCH_RESULT_URL = (
     f"{BASE_URL}/services/async/{SF_VERSION}/job/{SFDC_ID}/batch/{SFDC_ID}/result"
 )
+BATCH_QUERY_RESULT_URL = f"{BATCH_RESULT_URL}/{SFDC_ID}"
 
 
 # login stuff
 LOGIN_URL = f"{BASE_URL}/services/Soap/u/{SF_VERSION}"
 # bare minimum needed to make simple salesforce happy
 SOAP_API_LOGIN_RESPONSE = f"""<?xml version="1.0"?>
 <soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/">
```

### Comparing `simple-mockforce-0.8.0/simple_mockforce/query_algorithms/date_token.py` & `simple-mockforce-0.8.1/simple_mockforce/query_algorithms/date_token.py`

 * *Files identical despite different names*

### Comparing `simple-mockforce-0.8.0/simple_mockforce/query_algorithms/order_by.py` & `simple-mockforce-0.8.1/simple_mockforce/query_algorithms/order_by.py`

 * *Files identical despite different names*

### Comparing `simple-mockforce-0.8.0/simple_mockforce/query_algorithms/parent_attrs.py` & `simple-mockforce-0.8.1/simple_mockforce/query_algorithms/parent_attrs.py`

 * *Files identical despite different names*

### Comparing `simple-mockforce-0.8.0/simple_mockforce/query_algorithms/where.py` & `simple-mockforce-0.8.1/simple_mockforce/query_algorithms/where.py`

 * *Files identical despite different names*

### Comparing `simple-mockforce-0.8.0/simple_mockforce/utils.py` & `simple-mockforce-0.8.1/simple_mockforce/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,21 @@
 
 def parse_batch_result_url(url: str):
     split_up = url.split("/")
     job_id = split_up[-4]
     batch_id = split_up[-2]
     return job_id, batch_id
 
+def parse_batch_query_result_url(url: str):
+    split_up = url.split("/")
+    job_id = split_up[-5]
+    batch_id = split_up[-3]
+    result_set_id = split_up[-1]
+    return job_id, batch_id, result_set_id
+
 
 def find_object_and_index(objects: list, pk_name: str, pk: str):
     index = None
     original = None
     for idx, object_ in enumerate(objects):
         if object_.get(pk_name) == pk:
             index = idx
```

### Comparing `simple-mockforce-0.8.0/simple_mockforce/virtual.py` & `simple-mockforce-0.8.1/simple_mockforce/virtual.py`

 * *Files identical despite different names*

### Comparing `simple-mockforce-0.8.0/setup.py` & `simple-mockforce-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['decorator>=5.1.1,<6.0.0',
  'python-dateutil>=2.8.2,<3.0.0',
  'python-soql-parser>=0.2.0,<0.3.0',
  'responses>=0.20.0,<0.21.0']
 
 setup_kwargs = {
     'name': 'simple-mockforce',
-    'version': '0.8.0',
+    'version': '0.8.1',
     'description': "A companion package for simple-salesforce that enables the testing of code that interacts with Salesforce's API",
     'long_description': '# Introduction\n\nThis library was inspired by [moto](https://github.com/spulec/moto) and mimics some of its design. Mainly,\nno `simple-salesforce` code is patched; instead, the HTTP calls it makes are intercepted, and state is\nstored in an in-memory, virtual Salesforce organization, which is just a globally instantiated class that\nis created at the run-time of a test-suite.\n\n# Installation\n\n`pip install simple-mockforce`\n\nor, with poetry\n\n`poetry add simple-mockforce`\n\n# Usage\n\nTo patch calls to the Salesforce API and instead interact with the "virtual"\nSalesforce organization provided by this library, add the following:\n\n```python\nimport os\n\nfrom simple_mockforce import mock_salesforce\n\nfrom simple_salesforce import Salesforce\n\n\n@mock_salesforce\ndef test_api():\n    # The username, password, and security token are ignored - any value will work.\n    salesforce = Salesforce(\n        username=os.getenv("SFDC_USERNAME"),\n        password=os.getenv("SFDC_PASSWORD"),\n        security_token=os.getenv("SFDC_SECURITY_TOKEN")\n    )\n\n    response = salesforce.Account.create({"Name": "Test Account"})\n\n    account_id = response["id"]\n\n    account = salesforce.Account.get(account_id)\n\n    assert account["Name"] == "Test Account"\n```\n\nAnd that\'s about it!\n\n# Caveats\n\n## Case sensitivity\n\nUnlike a real Salesforce organization, the virtual organization will not handle case-insensitive\ndependent code for you. You must remain consistent with your casing of object and field\nnames in all aspects of the code.\n\n## Missing endpoints\n\nThe following features are currently not supported:\n\n- the describe API\n- bulk queries\n- SOSL searches\n\n## Queries\n\nSOQL is only partially supported as of now. Please refer to the README\nfor [python-soql-parser](https://github.com/Kicksaw-Consulting/python-soql-parser#notable-unsupported-features)\nto see what\'s not yet implemented.\n\nYou should only expect this library to be able to mock the most basic of queries.\nWhile there are plans to, mocking query calls which traverse object relationships\nor that use SOQL-specific where-clause tokens are not yet supported.\n\nNotable mentions:\n\n- be explicit with direction in `ORDER BY` clauses, i.e., always supply `DESC` or `ASC`\n- attributes of parent objects can be specified in the `select` clause (but not in the `where` clause)\n\n## Error handling\n\nError handling is only mocked to a degree, and for some calls it isn\'t at all.\nThis is because the virtual Salesforce organization does not yet enforce any of\nthe server-side validation you might encounter when working with the real API.\n\nThis means that the virtual organization is much more permissive and loose than a\nreal Salesforce organization would be.\n\nThere are plans to read the XML consumed by the meta API in order to enforce\nmore rigidity inside the virtual organization, but this is not yet implemented.\n\n## All HTTP traffic is blocked\n\nWhen using `@mock_salesforce`, do note that the `requests` library is being\npatched with `responses`, so any calls you make to any other APIs will fail\nunless you patch them yourself, or patch the code which invokes said calls.\n\n## Relations\n\nRelations are the weakest part of this library, and some features are just\nplain not supported yet.\n\nIf you have a relational field that points to an object whose name cannot be\ninferred from the field name (e.g., from `Account__r` it can be inferred\nthat this is pointing to an `Account` object), you can create a file called\n`relations.json` that translates a relational field name to your intended\nSalesforce object\'s name. See `relations.json` in the test folder for an\nexample.\n\nTo specify the location of `relations.json`, set an environment variable\ncalled `MOCKFORCE_RELATIONS_ROOT` which points to the parent folder of\n`relations.json`. Note, this defaults to the current directory `.`.\n',
     'author': 'Alex Drozd',
     'author_email': 'drozdster@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Kicksaw-Consulting/simple-mockforce',
```

### Comparing `simple-mockforce-0.8.0/PKG-INFO` & `simple-mockforce-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-mockforce
-Version: 0.8.0
+Version: 0.8.1
 Summary: A companion package for simple-salesforce that enables the testing of code that interacts with Salesforce's API
 Home-page: https://github.com/Kicksaw-Consulting/simple-mockforce
 License: MIT
 Keywords: python,simple-salesforce,salesforce,testing,mocking
 Author: Alex Drozd
 Author-email: drozdster@gmail.com
 Requires-Python: >=3.8,<4.0
```

