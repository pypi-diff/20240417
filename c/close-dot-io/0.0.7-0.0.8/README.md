# Comparing `tmp/close_dot_io-0.0.7.tar.gz` & `tmp/close_dot_io-0.0.8.tar.gz`

## Comparing `close_dot_io-0.0.7.tar` & `close_dot_io-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 close_dot_io-0.0.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 close_dot_io-0.0.7/requirements-dev.txt
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 close_dot_io-0.0.7/src/close_dot_io/__about__.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 close_dot_io-0.0.7/src/close_dot_io/__init__.py
--rw-r--r--   0        0        0    10782 2020-02-02 00:00:00.000000 close_dot_io-0.0.7/src/close_dot_io/client.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 close_dot_io-0.0.7/src/close_dot_io/dict_util.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 close_dot_io-0.0.7/src/close_dot_io/enums.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 close_dot_io-0.0.7/src/close_dot_io/resources/__init__.py
--rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 close_dot_io-0.0.7/src/close_dot_io/resources/activity.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 close_dot_io-0.0.7/src/close_dot_io/resources/base.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 close_dot_io-0.0.7/src/close_dot_io/resources/connected_account.py
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 close_dot_io-0.0.7/src/close_dot_io/resources/contact.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 close_dot_io-0.0.7/src/close_dot_io/resources/lead.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 close_dot_io-0.0.7/src/close_dot_io/resources/sequence.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 close_dot_io-0.0.7/src/close_dot_io/resources/smart_view.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 close_dot_io-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 close_dot_io-0.0.7/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 close_dot_io-0.0.7/LICENSE.txt
--rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 close_dot_io-0.0.7/README.md
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 close_dot_io-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     8480 2020-02-02 00:00:00.000000 close_dot_io-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/requirements-dev.txt
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/src/close_dot_io/__about__.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/src/close_dot_io/__init__.py
+-rw-r--r--   0        0        0    11989 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/src/close_dot_io/client.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/src/close_dot_io/dict_util.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/src/close_dot_io/enums.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/src/close_dot_io/resources/__init__.py
+-rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/src/close_dot_io/resources/activity.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/src/close_dot_io/resources/base.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/src/close_dot_io/resources/connected_account.py
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/src/close_dot_io/resources/contact.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/src/close_dot_io/resources/lead.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/src/close_dot_io/resources/sequence.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/src/close_dot_io/resources/smart_view.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/LICENSE.txt
+-rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/README.md
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 close_dot_io-0.0.8/PKG-INFO
```

### Comparing `close_dot_io-0.0.7/.pre-commit-config.yaml` & `close_dot_io-0.0.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.7/src/close_dot_io/client.py` & `close_dot_io-0.0.8/src/close_dot_io/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,67 +1,79 @@
 import re
 import time
-from typing import Literal
+from typing import Type, TypeVar
 from urllib.parse import urlencode
 
 import requests
 from pydantic import ValidationError, create_model
 
-from . import SmartView
-from .resources import BaseResourceModel, Contact, Lead
+from .resources import BaseResourceModel, Contact, Lead, SmartView
 from .resources.activity import BaseActivity
 
 MAX_RETRY = 5
 
 CAMEL_CASE_PATTERN = re.compile(r"(?<!^)(?=[A-Z])")
 
 
+R = TypeVar("R", bound=BaseResourceModel)
+
+
 class CloseClient:
     def __init__(
         self,
         api_key: str,
-        contact_model: type[Contact] = Contact,
-        lead_model: type[Lead] = Lead,
-        model_depth: int = 5,
+        model_depth: int = 10,
     ):
         self.base_url = "https://api.close.com/api/v1/"
         if not api_key:
             raise ValueError("No API key provided!")
         self.api_key = api_key
-        self.contact_model = contact_model
-        self.lead_model = lead_model
         self.model_depth = model_depth
 
         self.lead_statuses: dict = {}
 
     @staticmethod
+    def get_model_fields_for_query(
+        lead_resource: Type[R] = None, contact_resource: Type[R] = None
+    ) -> dict:
+        q = {"_fields": {}}
+        if lead_resource:
+            lead_fields = lead_resource.model_fields
+            q["_fields"]["lead"] = list(lead_fields.keys()) + ["custom"]
+
+        if contact_resource:
+            contact_fields = contact_resource.model_fields
+            q["_fields"]["contact"] = list(contact_fields.keys()) + ["custom"]
+        return q
+
+    @staticmethod
     def _get_rate_limit_sleep_time(response):
         """Get rate limit window expiration time from response if the response
         status code is 429.
         """
         try:
             if "error" in response.json():
                 return int(float(response.json()["error"]["rate_reset"]))
         except (AttributeError, KeyError, ValueError, Exception):
             return 60
 
-    def get_resource_or_none(self, resource, data: dict):
+    def get_resource_or_none(self, resource: Type[R], data: dict) -> R | None:
         try:
             return resource(**data | {"lead_statuses": self.lead_statuses})
         except ValidationError:
             # todo log?
             return None
 
     def set_lead_statuses(self):
         if self.lead_statuses:
             return
         res = self.dispatch(endpoint="/status/lead/").get("data")
         self.lead_statuses = {status.get("label"): status.get("id") for status in res}
 
-    def get_base_model(self, model):
+    def get_base_model(self, model: Type[R] | R):
         """
         Keep checking model inheritance until we hit the model that is directly above
         'BaseResourceModel' or 'BaseActivity' as this is what we use
         to build the resource endpoint route.
 
         This allows for deep inheritance of Lead/Contact/Oppertunity models.
         :param model:
@@ -87,15 +99,15 @@
             else:
                 model = last_class
                 recur_count += 1
             if recur_count >= self.model_depth:
                 break
         return model
 
-    def resource_to_endpoint(self, resource, resource_id=None):
+    def resource_to_endpoint(self, resource: R, resource_id=None) -> str:
         base_model = self.get_base_model(model=resource)
         snake_case = CAMEL_CASE_PATTERN.sub("_", base_model.__name__).lower()
         if snake_case.endswith("_activity"):
             activity_object = snake_case[: snake_case.index("_activity")]
             snake_case = f"activity/{activity_object}"
         return f"{snake_case}/{resource_id}" if resource_id else snake_case
 
@@ -117,47 +129,38 @@
                     sleep_time = self._get_rate_limit_sleep_time(res)
                     time.sleep(sleep_time)
                     continue
             except Exception as e:
                 raise e
         return {}
 
-    def get_model_fields_for_query(self, include_lead=True, include_contact=True):
-        q = {"_fields": {}}
-        if include_lead:
-            lead_fields = self.lead_model.model_fields
-            q["_fields"]["lead"] = list(lead_fields.keys()) + ["custom"]
-
-        if include_contact:
-            contact_fields = self.contact_model.model_fields
-            q["_fields"]["contact"] = list(contact_fields.keys()) + ["custom"]
-        return q
-
-    def run_pagination(self, resource, max_results: int = 100, url_params: dict = None):
+    def run_pagination(
+        self, resource_endpoint: str, max_results: int = 100, url_params: dict = None
+    ) -> list:
         items = []
         url_params = url_params or {}
         limit = 100
 
         def fetch_data(new_url):
             res = self.dispatch(endpoint=new_url)
             items.extend(res.get("data", []))
             return res.get("has_more", False)
 
         while len(items) < max_results:
             encoded_params = urlencode(
                 url_params | {"_skip": len(items), "_limit": limit}
             )
-            url = f"{resource}/?{encoded_params}"
+            url = f"{resource_endpoint}/?{encoded_params}"
             has_more = fetch_data(url)
             if not has_more:
                 break
 
         return items[:max_results]
 
-    def run_query(self, query: dict, max_results: int):
+    def run_query(self, query: dict, max_results: int) -> list:
         max_results = min(max_results, 9500)
         items = []
         query["_limit"] = 100
         res = self.dispatch(method="POST", json_data=query, endpoint="data/search/")
         items += res.get("data", [])
         cursor = res.get("cursor", None)
         while cursor is not None:
@@ -166,91 +169,126 @@
             query["cursor"] = cursor
             res = self.dispatch(method="POST", json_data=query, endpoint="data/search/")
             items += res.get("data", [])
             cursor = res.get("cursor", None)
         return items[:max_results]
 
     def get_contacts(
-        self, query: dict, fields: dict = None, max_results: int = 100
-    ) -> list[type[Contact]]:
+        self,
+        resource: Type[R],
+        query: dict,
+        fields: dict = None,
+        max_results: int = 100,
+    ) -> list[R]:
+        if self.get_base_model(resource) != Contact:
+            raise ValueError(
+                "Resource must be a subclass of 'Contact' to fetch contacts."
+            )
+        if not query:
+            raise ValueError("No query provided. Maybe you meant to use '.list()'?")
         contacts = []
-        fields = fields or self.get_model_fields_for_query(include_lead=False)
+        fields = fields or self.get_model_fields_for_query(contact_resource=resource)
         query = query | fields
         for contact in self.run_query(query=query, max_results=max_results):
-            if contact := self.get_resource_or_none(
-                resource=self.contact_model, data=contact
-            ):
+            if contact := self.get_resource_or_none(resource=resource, data=contact):
                 contacts.append(contact)
         return contacts
 
     def get_leads(
-        self, query: dict, fields: dict = None, max_results: int = 100
-    ) -> list[type[Lead]]:
+        self,
+        resource: Type[R],
+        query: dict,
+        fields: dict = None,
+        max_results: int = 100,
+    ) -> list[R]:
         leads = []
-        fields = fields or self.get_model_fields_for_query()
+        if self.get_base_model(resource) != Lead:
+            raise ValueError("Resource must be a subclass of 'Lead' to fetch leads.")
+        if not query:
+            raise ValueError("No query provided. Maybe you meant to use '.list()'?")
+        fields = fields or self.get_model_fields_for_query(
+            lead_resource=resource, contact_resource=resource.get_contact_type()
+        )
         query = query | fields
         for lead in self.run_query(query=query, max_results=max_results):
-            if lead := self.get_resource_or_none(resource=self.lead_model, data=lead):
+            if lead := self.get_resource_or_none(resource=resource, data=lead):
                 leads.append(lead)
         return leads
 
     def get_from_smartview(
         self,
+        resource: Type[R],
         smartview_name: str = None,
         smartview_id: str = None,
         max_results: int = 100,
-        resource: Literal["contact", "lead"] = None,
     ):
         if not smartview_name and not smartview_id:
             raise ValueError("One of smartview name or ID is required.")
         q, q_type = {}, None
         if smartview_id:
-            sv: SmartView = self.get(resource=SmartView, resource_id=smartview_id)
+            sv = self.get(resource=SmartView, resource_id=smartview_id)
             if not sv:
                 raise ValueError(f"SmartView '{smartview_id}' was not found.")
             q, q_type = sv.s_query, sv.type
         if not q:
-            params = {"type": resource} if resource else {"type__in": "lead,contact"}
-            svs: list[SmartView] = self.list(resource=SmartView, url_params=params)
+            params = (
+                {"type": self.resource_to_endpoint(resource)}
+                if resource
+                else {"type__in": "lead,contact"}
+            )
+            svs = self.list(resource=SmartView, url_params=params)
             for smart_view in svs:
                 if smart_view.name == smartview_name:
                     q, q_type = smart_view.s_query, smart_view.type
                     break
         if not q:
             raise ValueError(f"SmartView '{smartview_name}' was not found.")
         query = q.model_dump(mode="json")
         if q_type == "lead":
-            return self.get_leads(query=query, max_results=max_results)
-        return self.get_contacts(query=query, max_results=max_results)
+            return self.get_leads(
+                resource=resource, query=query, max_results=max_results
+            )
+        # If Lead resource passed but target return is Contact we extract out the Contact field.
+        # means if you dont know if your smartview is Lead or Contact can just throw in Lead and
+        # it's handled.
+        if self.get_base_model(resource) == Lead:
+            resource = resource.get_contact_type()
+        return self.get_contacts(
+            resource=resource, query=query, max_results=max_results
+        )
 
-    def list(self, resource, max_results: int = 100, url_params: dict = None):
+    def list(
+        self, resource: Type[R], max_results: int = 100, url_params: dict = None
+    ) -> list[R]:
         items = []
         for item in self.run_pagination(
             self.resource_to_endpoint(resource),
             max_results=max_results,
             url_params=url_params,
         ):
             if item := self.get_resource_or_none(resource=resource, data=item):
                 items.append(item)
         return items
 
-    def get(self, resource, resource_id: str = None, resource_instance=None):
+    def get(
+        self, resource: Type[R], resource_id: str = None, resource_instance=None
+    ) -> R:
         if not resource_id and not resource_instance:
-            raise ValueError("model_id or model_instance must be declared.")
+            raise ValueError("resource_id or resource_instance must be declared.")
         if resource_instance and not resource_instance.id:
             raise ValueError("Your instance does not have an ID!")
         return resource(
             **self.dispatch(
                 endpoint=self.resource_to_endpoint(
                     resource, resource_id or resource_instance.id
                 )
             )
         )
 
-    def save(self, resource, lead_id: str = None):
+    def save(self, resource: R, lead_id: str = None) -> R:
         base_resource = self.get_base_model(resource)
         swapped_to_lead = False
         # check if trying to create direct Contact, if so make Lead.
         if base_resource == Contact and resource.id is None and lead_id is None:
             # gen Lead model using Contact field schema.
             dynamic_lead_model = create_model(
                 "Lead",
@@ -269,14 +307,14 @@
         res = self.dispatch(endpoint=endpoint, method=method, json_data=data)
         resource = resource.__class__(**res)
         # If target resource was a contact, grab it instead of lead.
         if base_resource == Contact and swapped_to_lead:
             resource = resource.contacts[0]
         return resource
 
-    def delete(self, resource_instance) -> None:
+    def delete(self, resource_instance: R) -> None:
         endpoint = self.resource_to_endpoint(
             resource=resource_instance, resource_id=resource_instance.id
         )
         if not resource_instance.id:
             raise ValueError("Can't delete without an ID.")
         self.dispatch(endpoint=endpoint, method="DELETE")
```

### Comparing `close_dot_io-0.0.7/src/close_dot_io/resources/__init__.py` & `close_dot_io-0.0.8/src/close_dot_io/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.7/src/close_dot_io/resources/activity.py` & `close_dot_io-0.0.8/src/close_dot_io/resources/activity.py`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.7/src/close_dot_io/resources/base.py` & `close_dot_io-0.0.8/src/close_dot_io/resources/base.py`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.7/src/close_dot_io/resources/contact.py` & `close_dot_io-0.0.8/src/close_dot_io/resources/contact.py`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.7/src/close_dot_io/resources/lead.py` & `close_dot_io-0.0.8/src/close_dot_io/resources/lead.py`

 * *Files 17% similar despite different names*

```diff
@@ -30,7 +30,13 @@
     @computed_field
     @property
     def status_id(self) -> str | None:
         if not self.status_label:
             return None
         if self.status_label in self.lead_statuses:
             return self.lead_statuses[self.status_label]
+
+    @classmethod
+    def get_contact_type(cls):
+        # Get the 'Contact' type from the Lead.
+        contact_resource = cls.__annotations__["contacts"]
+        return contact_resource.__args__[0]
```

### Comparing `close_dot_io-0.0.7/src/close_dot_io/resources/sequence.py` & `close_dot_io-0.0.8/src/close_dot_io/resources/sequence.py`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.7/src/close_dot_io/resources/smart_view.py` & `close_dot_io-0.0.8/src/close_dot_io/resources/smart_view.py`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.7/LICENSE.txt` & `close_dot_io-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.7/README.md` & `close_dot_io-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Close[.]io
 
-[![PyPI - Version](https://img.shields.io/pypi/v/close-dot-io.svg)](https://pypi.org/project/close-io-flows)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/close-dot-io.svg)](https://pypi.org/project/close-io-flows)
+[![PyPI - Version](https://img.shields.io/pypi/v/close-dot-io.svg)](https://pypi.org/project/close-dot-io)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/close-dot-io.svg)](https://pypi.org/project/close-dot-io)
 
 -----
 
 Simpler and saner interface for working with the [Close](https://close.com/) API
 
 Features:
```

### Comparing `close_dot_io-0.0.7/pyproject.toml` & `close_dot_io-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.7/PKG-INFO` & `close_dot_io-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: close-dot-io
-Version: 0.0.7
+Version: 0.0.8
 Summary: Easy interface to work with the Close.io API.
 Project-URL: Documentation, https://github.com/unknown/close_dot_io#readme
 Project-URL: Issues, https://github.com/unknown/close_dot_io/issues
 Project-URL: Source, https://github.com/unknown/close_dot_io
 Author-email: Copyfactory <dev@copyfactory.io>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -22,16 +22,16 @@
 Requires-Dist: pydantic-extra-types
 Requires-Dist: pydantic[email]>=2.5.2
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # Close[.]io
 
-[![PyPI - Version](https://img.shields.io/pypi/v/close-dot-io.svg)](https://pypi.org/project/close-io-flows)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/close-dot-io.svg)](https://pypi.org/project/close-io-flows)
+[![PyPI - Version](https://img.shields.io/pypi/v/close-dot-io.svg)](https://pypi.org/project/close-dot-io)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/close-dot-io.svg)](https://pypi.org/project/close-dot-io)
 
 -----
 
 Simpler and saner interface for working with the [Close](https://close.com/) API
 
 Features:
```

