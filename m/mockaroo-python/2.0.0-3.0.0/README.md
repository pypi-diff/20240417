# Comparing `tmp/mockaroo_python-2.0.0.tar.gz` & `tmp/mockaroo_python-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mockaroo_python-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mockaroo_python-3.0.0.tar", max compression
```

## Comparing `mockaroo_python-2.0.0.tar` & `mockaroo_python-3.0.0.tar`

### file list

```diff
@@ -1,23 +1,10 @@
--rw-r--r--   0        0        0      825 2023-10-12 02:10:20.056208 mockaroo_python-2.0.0/.github/workflows/continuous_integration.yml
--rw-r--r--   0        0        0     3134 2023-10-17 05:39:30.780177 mockaroo_python-2.0.0/.gitignore
--rw-r--r--   0        0        0     1533 2023-10-18 02:15:09.972372 mockaroo_python-2.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1081 2023-10-06 20:41:45.952985 mockaroo_python-2.0.0/LICENSE
--rw-r--r--   0        0        0      232 2023-10-17 05:38:28.753929 mockaroo_python-2.0.0/Makefile
--rw-r--r--   0        0        0     7625 2023-10-18 02:15:53.242549 mockaroo_python-2.0.0/README.md
--rw-r--r--   0        0        0      273 2023-10-18 02:25:11.352616 mockaroo_python-2.0.0/mockaroo/__init__.py
--rw-r--r--   0        0        0      714 2023-10-18 00:10:25.609828 mockaroo_python-2.0.0/mockaroo/__main__.py
--rw-r--r--   0        0        0       12 2023-10-17 04:22:43.352680 mockaroo_python-2.0.0/mockaroo/api/__init__.py
--rw-r--r--   0        0        0     9986 2023-10-18 01:20:12.809642 mockaroo_python-2.0.0/mockaroo/api/client.py
--rw-r--r--   0        0        0      217 2023-10-16 23:49:13.179742 mockaroo_python-2.0.0/mockaroo/api/constants.py
--rw-r--r--   0        0        0      342 2023-10-16 23:49:13.179948 mockaroo_python-2.0.0/mockaroo/api/exceptions.py
--rw-r--r--   0        0        0       12 2023-10-17 05:15:41.612573 mockaroo_python-2.0.0/mockaroo/cli/__init__.py
--rw-r--r--   0        0        0     1068 2023-10-17 23:39:07.462241 mockaroo_python-2.0.0/mockaroo/cli/commands.py
--rw-r--r--   0        0        0     1858 2023-10-18 01:21:30.828682 mockaroo_python-2.0.0/mockaroo/cli/layout.py
--rw-r--r--   0        0        0     1277 2023-10-18 02:12:15.819554 mockaroo_python-2.0.0/pyproject.toml
--rw-r--r--   0        0        0       33 2023-10-16 23:49:13.165184 mockaroo_python-2.0.0/requirements.txt
--rw-r--r--   0        0        0       12 2023-10-17 04:22:20.253399 mockaroo_python-2.0.0/tests/__init__.py
--rw-r--r--   0        0        0     2808 2023-10-18 01:51:27.692139 mockaroo_python-2.0.0/tests/test_cli.py
--rw-r--r--   0        0        0     7768 2023-10-18 00:51:24.376650 mockaroo_python-2.0.0/tests/test_client.py
--rw-r--r--   0        0        0      294 2023-10-18 00:00:40.045415 mockaroo_python-2.0.0/tests/test_layout.py
--rw-r--r--   0        0        0      479 2023-10-18 01:41:34.960965 mockaroo_python-2.0.0/tox.ini
--rw-r--r--   0        0        0     8606 1970-01-01 00:00:00.000000 mockaroo_python-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-10-06 20:41:45.952985 mockaroo_python-3.0.0/LICENSE
+-rw-r--r--   0        0        0     3631 2024-04-17 04:22:52.815266 mockaroo_python-3.0.0/README.md
+-rw-r--r--   0        0        0       49 2024-04-17 03:03:54.891616 mockaroo_python-3.0.0/mockaroo/__init__.py
+-rw-r--r--   0        0        0       59 2024-04-17 02:49:37.974098 mockaroo_python-3.0.0/mockaroo/__main__.py
+-rw-r--r--   0        0        0     1791 2024-04-17 04:51:23.404855 mockaroo_python-3.0.0/mockaroo/cli.py
+-rw-r--r--   0        0        0    10899 2024-04-17 03:28:41.620681 mockaroo_python-3.0.0/mockaroo/client.py
+-rw-r--r--   0        0        0      342 2023-10-19 23:22:35.350250 mockaroo_python-3.0.0/mockaroo/exceptions.py
+-rw-r--r--   0        0        0     1873 2023-10-19 23:22:28.485833 mockaroo_python-3.0.0/mockaroo/layout.py
+-rw-r--r--   0        0        0      603 2024-04-17 04:53:15.012083 mockaroo_python-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4443 1970-01-01 00:00:00.000000 mockaroo_python-3.0.0/PKG-INFO
```

### Comparing `mockaroo_python-2.0.0/LICENSE` & `mockaroo_python-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mockaroo_python-2.0.0/mockaroo/api/client.py` & `mockaroo_python-3.0.0/mockaroo/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 """Provides code to interact with the Mockaroo API."""
-import warnings
+
 import os
-from typing import Any, Dict, List, Optional, Union, ByteString
-from urllib.parse import urlencode, quote
+import warnings
+from typing import Any, ByteString, Dict, List, Optional, Union
+from urllib.parse import quote, urlencode
 
 import requests
 from dotenv import load_dotenv
+from requests.exceptions import RequestException
 
-from .constants import (
-    TYPE_ENDPOINT,
-    UPLOAD_ENDPOINT,
-    GENERATE_ENDPOINT,
-    HTTP_GET,
-    HTTP_POST,
-    HTTP_DELETE,
-)
 from .exceptions import (
-    MockarooError,
     InvalidApiKeyError,
+    MockarooError,
     UsageLimitExceededError,
 )
 
 load_dotenv()
 
 
 class Client:
     """Client for interacting with the Mockaroo API.
 
     Attributes:
-        api_key (Optional[str]): API key for Mockaroo API.
+        api_key (Optional[str]): API key for the Mockaroo API.
         host (str): Hostname of the API. Default: api.mockaroo.com
         secure (bool): Whether to use HTTPS. Default: True
         port (Optional[int]): Port number to connect to. Default: None.
 
     """
+
+    TYPE_ENDPOINT = "/api/types/"
+    UPLOAD_ENDPOINT = "/api/datasets/"
+    GENERATE_ENDPOINT = "/api/generate"
+
+    HTTP_GET = "GET"
+    HTTP_POST = "POST"
+    HTTP_DELETE = "DELETE"
+
     def __init__(
         self,
         api_key: Optional[str] = None,
         host: str = "api.mockaroo.com",
         secure: bool = True,
         port: Optional[int] = None,
     ) -> None:
@@ -56,19 +59,19 @@
 
         self.last_request: Optional[Dict[str, Any]] = None
 
     @property
     def api_key(self):
         """Set API key."""
         if not self._api_key:
-            self._api_key = os.environ.get("API_KEY")
+            self._api_key = os.environ.get("MOCKAROO_API_KEY")
             if not self._api_key:
                 warnings.warn(
-                    "API key is not provided. " \
-                    "Set API_KEY `export API_KEY=your_api_key`."
+                    "API key is not provided. "
+                    "Set MOCKAROO_API_KEY `export MOCKAROO_API_KEY=your_api_key`."
                 )
         return self._api_key
 
     def _convert_error(self, response_data: Dict[str, Any]) -> None:
         """Convert API errors into appropriate exceptions.
 
         Args:
@@ -85,24 +88,25 @@
         exception_cls = exception_mapping.get(error, MockarooError)
         raise exception_cls(error)
 
     def _validate_fields(self, fields: List[Dict[str, Any]]) -> None:
         """Validate that each field has 'name' and 'type' keys.
 
         Args:
-            fields (List[Dict[str, Any]]): 
-            A list of dictionaries representing the fields for data generation.
+            fields (List[Dict[str, Any]]): A list of dictionaries
+            representing the fields for data generation.
 
         Raises:
             ValueError: If any dictionary lacks a 'name' or 'type' key.
         """
-        if not all("name" in field and "type" in field for field in fields):
-            raise ValueError("Each field must have a 'name' and 'type'")
+        for idx, field in enumerate(fields):
+            if not all(k in field for k in ["name", "type"]):
+                raise ValueError(f"Field at index {idx} must have a 'name' and 'type'")
 
-    def _get_url( # noqa: D417
+    def _get_url(  # noqa: D417
         self,
         endpoint: str,
         **params,
     ) -> str:
         """Construct the API URL.
 
         Args:
@@ -139,72 +143,88 @@
             endpoint = (
                 f"{endpoint}{quote(name)}"  # Example: api/upload/name%20of%20dataset?
             )
 
         return f"{base_url}{endpoint}?{urlencode(params)}"
 
     def _http_request(self, method: str, url: str, **kwargs) -> requests.Response:
+        """Perform an HTTP request and return a requests.Response object.
+
+        Args:
+            method (str): The HTTP method to use (e.g., 'GET', 'POST').
+            url (str): The URL to which the request is sent.
+            **kwargs: Additional keyword arguments to pass to `requests.request`.
+
+        Returns:
+            requests.Response: The response object containing details of the HTTP response.
+
+        Raises:
+            Exception: If the HTTP request fails for any reason or if the status code is not 200.
+
+        Side Effects:
+            Updates the `last_request` instance variable with details about the request and its outcome.
+        """  # noqa: E501
         self.last_request = {
             "method": method,
             "url": url,
             "request": kwargs,
             "error": None,
         }
         try:
             resp = requests.request(method, url, **kwargs)
             self.last_request["response"] = resp.text
-        except Exception as e:
+        except RequestException as e:
             self.last_request["error"] = str(e)
             raise
 
         if resp.status_code != 200:
             self._convert_error(resp.json())
         return resp
 
     def types(self) -> List[Dict[str, Any]]:
         """Retrieve the types supported by the Mockaroo API.
 
         Returns:
             dict: A list of dictionaries containing types supported by Mockaroo.
         """
-        url = self._get_url(TYPE_ENDPOINT)
-        json_resp = self._http_request(HTTP_GET, url=url).json()
+        url = self._get_url(self.TYPE_ENDPOINT)
+        json_resp = self._http_request(self.HTTP_GET, url=url).json()
         return json_resp["types"]
 
     def upload(self, name: str, path: str) -> Dict[str, Any]:
         """Upload a dataset to Mockaroo.
 
         Args:
             name (str): Name of the dataset to upload.
             path (str): File path of the dataset to upload.
 
         Returns:
             dict: Dictionary containing upload status and other metadata.
         """
-        url = self._get_url(UPLOAD_ENDPOINT, name=name)
+        url = self._get_url(self.UPLOAD_ENDPOINT, name=name)
         with open(path, "rb") as f:
-            files = {"file": f}
+            file_content = f.read()
             return self._http_request(
-                HTTP_POST,
+                self.HTTP_POST,
                 url=url,
-                files=files,
                 headers={"content-type": "text/csv"},
+                data=file_content,
             ).json()
 
     def delete(self, name: str) -> Dict[str, Any]:
         """Delete a dataset from Mockaroo.
 
         Args:
             name (str): Name of the dataset to delete.
 
         Returns:
             dict: Dictionary containing delete status and other metadata.
         """
-        url = self._get_url(UPLOAD_ENDPOINT, name=name)
-        return self._http_request(HTTP_DELETE, url=url).json()
+        url = self._get_url(self.UPLOAD_ENDPOINT, name=name)
+        return self._http_request(self.HTTP_DELETE, url=url).json()
 
     def generate(  # noqa: D417
         self,
         **kwargs,
     ) -> Union[Dict[str, Any], List[Dict[str, Any]], ByteString]:
         """Generate mock data using the Mockaroo API.
 
@@ -249,34 +269,34 @@
                             "type": "Custom List",
                             "values": ["credit","debit"]
                         }
                     ]
                 )
             >>> data
             [
-                {'id': 1, 'transactionType': 'credit'}, 
+                {'id': 1, 'transactionType': 'credit'},
                 {'id': 2, 'transactionType': 'debit'}
             ]
-        """ # noqa: E501
+        """  # noqa: E501
         schema = kwargs.get("schema")
         fields = kwargs.get("fields")
 
         if (schema is None and fields is None) or (
             schema is not None and fields is not None
         ):
             warnings.warn(
-                "You should specify either 'schema' or 'fields', "\
-                "but not both. `schema` will override any values passed"\
+                "You should specify either 'schema' or 'fields', "
+                "but not both. `schema` will override any values passed"
                 "to `fields`."
             )
 
         if fields:
             self._validate_fields(fields)
 
         fields = kwargs.pop("fields", None)  # Remove fields from keyword args
 
-        url = self._get_url(GENERATE_ENDPOINT, **kwargs)
-        response = self._http_request(HTTP_POST, url=url, json=fields)
+        url = self._get_url(self.GENERATE_ENDPOINT, **kwargs)
+        response = self._http_request(self.HTTP_POST, url=url, json=fields)
 
         return (
             response.json() if kwargs.get("fmt", "json") == "json" else response.content
         )
```

### Comparing `mockaroo_python-2.0.0/mockaroo/cli/layout.py` & `mockaroo_python-3.0.0/mockaroo/layout.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,19 +23,20 @@
     for d in data_types:
         name = Text(d["name"], style="bold #19857b")
         data_type = Text(d["type"], style="bold #52a552") if d["type"] else Text("")
         params = d.get("parameters", "")
         if params:
             result = []
             for count, param in enumerate(params, start=1):
-                formatted_str = \
-                    f"{count}.) [#90caf9]Name[/#90caf9]: {param['name']}"\
-                    "[#90caf9]Type[/#90caf9]: {param['type']} "\
-                    "[#90caf9]Description[/#90caf9]: '{param['description']}' "\
+                formatted_str = (
+                    f"{count}.) [#90caf9]Name[/#90caf9]: {param['name']}"
+                    "[#90caf9]Type[/#90caf9]: {param['type']} "
+                    "[#90caf9]Description[/#90caf9]: '{param['description']}' "
                     "[#90caf9]Default[/#90caf9]: {param['default']}\n"
+                )
                 result.append(formatted_str)
 
             result_str = "\n".join(result)
         else:
             result_str = "None"
 
         table.add_row(name, data_type, result_str)
```

