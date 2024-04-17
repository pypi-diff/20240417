# Comparing `tmp/up42-py-0.9.3.tar.gz` & `tmp/up42_py-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/up42-py-0.9.3.tar", last modified: Wed Jul 15 08:44:17 2020, max compression
+gzip compressed data, was "up42_py-1.0.0.tar", max compression
```

## Comparing `up42-py-0.9.3.tar` & `up42_py-1.0.0.tar`

### file list

```diff
@@ -1,39 +1,27 @@
-drwxr-xr-x   0 christoph.rieke   (501) staff       (20)        0 2020-07-15 08:44:17.985724 up42-py-0.9.3/
--rw-r--r--   0 christoph.rieke   (501) staff       (20)     4941 2020-07-15 08:44:17.985319 up42-py-0.9.3/PKG-INFO
--rw-r--r--   0 christoph.rieke   (501) staff       (20)     3712 2020-07-06 16:29:30.000000 up42-py-0.9.3/README.md
--rw-r--r--   0 christoph.rieke   (501) staff       (20)       38 2020-07-15 08:44:17.985871 up42-py-0.9.3/setup.cfg
--rw-r--r--   0 christoph.rieke   (501) staff       (20)     1156 2020-05-05 12:09:18.000000 up42-py-0.9.3/setup.py
-drwxr-xr-x   0 christoph.rieke   (501) staff       (20)        0 2020-07-15 08:44:17.922757 up42-py-0.9.3/tests/
--rw-r--r--   0 christoph.rieke   (501) staff       (20)        0 2020-04-16 13:11:05.000000 up42-py-0.9.3/tests/__init__.py
--rw-r--r--   0 christoph.rieke   (501) staff       (20)      799 2020-07-04 12:26:42.000000 up42-py-0.9.3/tests/context.py
--rw-r--r--   0 christoph.rieke   (501) staff       (20)      962 2020-04-27 14:02:14.000000 up42-py-0.9.3/tests/e2e.py
--rw-r--r--   0 christoph.rieke   (501) staff       (20)     4113 2020-05-07 09:50:38.000000 up42-py-0.9.3/tests/fixtures.py
--rw-r--r--   0 christoph.rieke   (501) staff       (20)     3858 2020-04-27 13:22:11.000000 up42-py-0.9.3/tests/test_auth.py
--rw-r--r--   0 christoph.rieke   (501) staff       (20)     4124 2020-06-29 19:07:02.000000 up42-py-0.9.3/tests/test_catalog.py
--rw-r--r--   0 christoph.rieke   (501) staff       (20)     9930 2020-04-27 14:02:14.000000 up42-py-0.9.3/tests/test_cli.py
--rw-r--r--   0 christoph.rieke   (501) staff       (20)     1446 2020-04-16 13:11:05.000000 up42-py-0.9.3/tests/test_initialization.py
--rw-r--r--   0 christoph.rieke   (501) staff       (20)    10068 2020-07-15 08:37:10.000000 up42-py-0.9.3/tests/test_job.py
--rw-r--r--   0 christoph.rieke   (501) staff       (20)     4312 2020-05-07 08:37:27.000000 up42-py-0.9.3/tests/test_jobtask.py
--rw-r--r--   0 christoph.rieke   (501) staff       (20)     5377 2020-05-06 16:00:14.000000 up42-py-0.9.3/tests/test_project.py
--rw-r--r--   0 christoph.rieke   (501) staff       (20)     6367 2020-04-27 13:22:11.000000 up42-py-0.9.3/tests/test_tools.py
--rw-r--r--   0 christoph.rieke   (501) staff       (20)     8785 2020-07-04 12:26:42.000000 up42-py-0.9.3/tests/test_utils.py
--rw-r--r--   0 christoph.rieke   (501) staff       (20)    17082 2020-05-07 09:50:38.000000 up42-py-0.9.3/tests/test_workflow.py
-drwxr-xr-x   0 christoph.rieke   (501) staff       (20)        0 2020-07-15 08:44:17.949414 up42-py-0.9.3/up42/
--rw-r--r--   0 christoph.rieke   (501) staff       (20)     4435 2020-05-05 12:09:23.000000 up42-py-0.9.3/up42/__init__.py
--rw-r--r--   0 christoph.rieke   (501) staff       (20)     9360 2020-04-27 13:22:11.000000 up42-py-0.9.3/up42/auth.py
--rw-r--r--   0 christoph.rieke   (501) staff       (20)    10113 2020-07-06 16:29:30.000000 up42-py-0.9.3/up42/catalog.py
--rw-r--r--   0 christoph.rieke   (501) staff       (20)    20181 2020-05-05 10:54:11.000000 up42-py-0.9.3/up42/cli.py
--rw-r--r--   0 christoph.rieke   (501) staff       (20)    15379 2020-07-15 08:37:10.000000 up42-py-0.9.3/up42/job.py
--rw-r--r--   0 christoph.rieke   (501) staff       (20)     5662 2020-07-06 16:29:30.000000 up42-py-0.9.3/up42/jobtask.py
--rw-r--r--   0 christoph.rieke   (501) staff       (20)     6525 2020-07-06 16:29:30.000000 up42-py-0.9.3/up42/project.py
--rw-r--r--   0 christoph.rieke   (501) staff       (20)    14311 2020-07-06 16:29:30.000000 up42-py-0.9.3/up42/tools.py
--rw-r--r--   0 christoph.rieke   (501) staff       (20)    15178 2020-07-15 08:37:10.000000 up42-py-0.9.3/up42/utils.py
--rw-r--r--   0 christoph.rieke   (501) staff       (20)    20079 2020-07-06 16:29:30.000000 up42-py-0.9.3/up42/workflow.py
-drwxr-xr-x   0 christoph.rieke   (501) staff       (20)        0 2020-07-15 08:44:17.984468 up42-py-0.9.3/up42_py.egg-info/
--rw-r--r--   0 christoph.rieke   (501) staff       (20)     4941 2020-07-15 08:44:17.000000 up42-py-0.9.3/up42_py.egg-info/PKG-INFO
--rw-r--r--   0 christoph.rieke   (501) staff       (20)      662 2020-07-15 08:44:17.000000 up42-py-0.9.3/up42_py.egg-info/SOURCES.txt
--rw-r--r--   0 christoph.rieke   (501) staff       (20)        1 2020-07-15 08:44:17.000000 up42-py-0.9.3/up42_py.egg-info/dependency_links.txt
--rw-r--r--   0 christoph.rieke   (501) staff       (20)       58 2020-07-15 08:44:17.000000 up42-py-0.9.3/up42_py.egg-info/entry_points.txt
--rw-r--r--   0 christoph.rieke   (501) staff       (20)        1 2020-03-24 12:32:50.000000 up42-py-0.9.3/up42_py.egg-info/not-zip-safe
--rw-r--r--   0 christoph.rieke   (501) staff       (20)       98 2020-07-15 08:44:17.000000 up42-py-0.9.3/up42_py.egg-info/requires.txt
--rw-r--r--   0 christoph.rieke   (501) staff       (20)        5 2020-07-15 08:44:17.000000 up42-py-0.9.3/up42_py.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1061 2024-04-17 09:59:47.743636 up42_py-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2990 2024-04-17 09:59:47.743636 up42_py-1.0.0/README.md
+-rw-r--r--   0        0        0     1786 2024-04-17 09:59:47.763636 up42_py-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1731 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/__init__.py
+-rw-r--r--   0        0        0     7991 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/asset.py
+-rw-r--r--   0        0        0     3754 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/asset_searcher.py
+-rw-r--r--   0        0        0     5068 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/auth.py
+-rw-r--r--   0        0        0    20308 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/catalog.py
+-rw-r--r--   0        0        0      706 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/data/aoi_berlin.geojson
+-rw-r--r--   0        0        0      703 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/data/aoi_washington.geojson
+-rw-r--r--   0        0        0      135 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/host.py
+-rw-r--r--   0        0        0        0 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/http/__init__.py
+-rw-r--r--   0        0        0     1782 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/http/client.py
+-rw-r--r--   0        0        0      484 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/http/config.py
+-rw-r--r--   0        0        0      673 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/http/http_adapter.py
+-rw-r--r--   0        0        0     3290 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/http/oauth.py
+-rw-r--r--   0        0        0     1113 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/http/session.py
+-rw-r--r--   0        0        0     1885 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/initialization.py
+-rw-r--r--   0        0        0     3424 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/main.py
+-rw-r--r--   0        0        0     8372 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/order.py
+-rw-r--r--   0        0        0      910 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/stac_client.py
+-rw-r--r--   0        0        0     8485 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/storage.py
+-rw-r--r--   0        0        0    10622 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/tasking.py
+-rw-r--r--   0        0        0     3287 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/tools.py
+-rw-r--r--   0        0        0    14820 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/utils.py
+-rw-r--r--   0        0        0     6749 2024-04-17 09:59:47.771636 up42_py-1.0.0/up42/webhooks.py
+-rw-r--r--   0        0        0     4034 1970-01-01 00:00:00.000000 up42_py-1.0.0/PKG-INFO
```

### Comparing `up42-py-0.9.3/up42/auth.py` & `up42_py-1.0.0/up42/order.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,262 +1,238 @@
-import json
-from pathlib import Path
-from typing import Dict, List, Union
-
-import requests
-import requests.exceptions
-from tenacity import (
-    Retrying,
-    wait_fixed,
-    stop_after_attempt,
-    retry_if_exception_type,
-)
+import copy
+import time
+from typing import Any, Dict, List, Optional, TypedDict
+
+from up42 import asset, asset_searcher
+from up42 import auth as up42_auth
+from up42 import host, utils
+
+logger = utils.get_logger(__name__)
+
+MAX_ITEM = 200
+LIMIT = 200
+
+
+def _translate_construct_parameters(order_parameters):
+    order_parameters_v2 = copy.deepcopy(order_parameters)
+    params = order_parameters_v2["params"]
+    data_product_id = order_parameters_v2["dataProduct"]
+    default_name = f"{data_product_id} order"
+    order_parameters_v2["displayName"] = params.get("displayName", default_name)
+    aoi = params.pop("aoi", None) or params.pop("geometry", None)
+    feature_collection = {
+        "type": "FeatureCollection",
+        "features": [
+            {
+                "type": "Feature",
+                "geometry": aoi,
+            }
+        ],
+    }
+    order_parameters_v2["featureCollection"] = feature_collection
+    return order_parameters_v2
+
+
+class OrderParams(TypedDict):
+    """
+    Represents the stucture data format for the order parameters.
+    dataProduct: The dataProduct id for the specific product configuration.
+    params: Order parameters for each product. \
+        They are different from product to product depending on product schema.
+    tags: User tags to helping to identify the order.
+    """
+
+    dataProduct: str  # pylint: disable=invalid-name
+    params: Dict[str, Any]
+    tags: List[str]
+
+
+class Order:
+    """
+    The Order class enables you to place, inspect and get information on orders.
+
+    Use an existing order:
+    ```python
+    order = up42.initialize_order(order_id="ea36dee9-fed6-457e-8400-2c20ebd30f44")
+    ```
+    """
 
-from .tools import Tools
-from .utils import get_logger
-
-logger = get_logger(__name__)
-
-
-class Auth(Tools):
     def __init__(
         self,
-        cfg_file: Union[str, Path] = None,
-        project_id: str = None,
-        project_api_key: str = None,
-        **kwargs,
+        auth: up42_auth.Auth,
+        order_id: str,
+        order_parameters: Optional[dict] = None,
+        order_info: Optional[dict] = None,
     ):
+        self.auth = auth
+        self.order_id = order_id
+        self.order_parameters = order_parameters
+        if order_info is not None:
+            self._info = order_info
+        else:
+            self._info = self.info
+
+    def __repr__(self):
+        return (
+            f"""Order(order_id: {self.order_id}, status: {self._info["status"]},"""
+            f"""createdAt: {self._info["createdAt"]}, updatedAt: {self._info["updatedAt"]})"""
+        )
+
+    def __eq__(self, other: Optional[object]):
+        return other and hasattr(other, "_info") and other._info == self._info
+
+    @property
+    def info(self) -> dict:
+        """
+        Gets and updates the order information.
         """
-        The Auth class handles the authentication with UP42.
+        url = host.endpoint(f"/v2/orders/{self.order_id}")
+        response_json = self.auth.request(request_type="GET", url=url)
+        self._info = response_json
+        return self._info
 
-        Info:
-            Authentication is possible via the credentials of a specific project (project_id &
-            project_api_key). To get your **project id** and **project api key**, follow
-            the instructions in the docs installation chapter.
+    @property
+    def status(self) -> str:
+        """
+        Gets the Order status. One of `PLACED`, `FAILED`, `FULFILLED`, `BEING_FULFILLED`, `FAILED_PERMANENTLY`.
+        """
+        status = self.info["status"]
+        logger.info("Order is %s", status)
+        return status
 
-        Args:
-            cfg_file: File path to the cfg.json with {project_id: "...", project_api_key: "..."}.
-            project_id: The unique identifier of the project.
-            project_api_key: The project-specific API key.
-        """
-        self.cfg_file = cfg_file
-        self.project_id = project_id
-        self.project_api_key = project_api_key
-
-        try:
-            self.env: str = kwargs["env"]
-        except KeyError:
-            self.env = "com"
-        try:
-            self.authenticate: bool = kwargs["authenticate"]
-        except KeyError:
-            self.authenticate = True
-        try:
-            self.retry: bool = kwargs["retry"]
-        except KeyError:
-            self.retry = True
-        try:
-            self.get_info: bool = kwargs["get_info"]
-        except KeyError:
-            self.get_info = True
-
-        if self.authenticate:
-            self._find_credentials()
-            self._get_token()
-            logger.info("Authentication with UP42 successful!")
+    @property
+    def order_details(self) -> dict:
+        """
+        Gets the Order Details. Only for tasking type orders, archive types return empty.
+        """
+        if self.info["type"] == "TASKING":
+            order_details = self.info["orderDetails"]
+            return order_details
+        logger.info("Order is not TASKING type. Order details are not provided.")
+        return {}
 
-    def __repr__(self):
-        return f"UP42ProjectAuth(project_id={self.project_id}, env={self.env})"
+    @property
+    def is_fulfilled(self) -> bool:
+        """
+        Gets `True` if the order is fulfilled, `False` otherwise.
+        Also see [status attribute](order-reference.md#up42.order.Order.status).
+        """
+        return self.status == "FULFILLED"
 
-    def _find_credentials(self) -> None:
+    def get_assets(self) -> List[asset.Asset]:
         """
-        Sources the project credentials from a provided config file and error handling
-        if no credentials are provided in arguments or config file.
+        Gets the Order assets or results.
         """
-        if self.project_id is None or self.project_api_key is None:
-            if self.cfg_file is None:
-                raise ValueError(
-                    "Provide project_id and project_api_key via arguments or config file!"
-                )
-
-            # Source credentials from config file.
-            try:
-                with open(self.cfg_file) as src:
-                    config = json.load(src)
-                    try:
-                        self.project_id = config["project_id"]
-                        self.project_api_key = config["project_api_key"]
-                    except KeyError:
-                        raise ValueError(
-                            "Provided config file does not contain project_id and "
-                            "project_api_key!"
-                        )
-                logger.info("Got credentials from config file.")
-            except FileNotFoundError:
-                raise ValueError("Selected config file does not exist!")
-
-        elif all(
-            v is not None
-            for v in [self.cfg_file, self.project_id, self.project_api_key]
-        ):
-            logger.info(
-                "Credentials are provided via arguments and config file, "
-                "now using the argument credentials."
-            )
+        if self.is_fulfilled:
+            params: asset_searcher.AssetSearchParams = {"search": self.order_id}
+            assets_response = asset_searcher.search_assets(self.auth, params=params)
+            return [asset.Asset(self.auth, asset_info=asset_info) for asset_info in assets_response]
+        raise ValueError(f"Order {self.order_id} is not FULFILLED! Current status is {self.status}")
 
-    def _endpoint(self) -> str:
-        """Gets the endpoint."""
-        return f"https://api.up42.{self.env}"
-
-    # pylint: disable=assignment-from-no-return
-    def _get_token(self):
-        try:
-            self._get_token_project()
-        except requests.exceptions.HTTPError:
-            raise ValueError(
-                "Authentication was not successful, check the provided project keys."
-            )
+    @classmethod
+    def place(cls, auth: up42_auth.Auth, order_parameters: dict) -> "Order":
+        """
+        Places an order.
 
-    def _get_token_project(self) -> None:
-        """Project specific authentication via project id and project api key."""
-        url = (
-            f"https://{self.project_id}:{self.project_api_key}@api.up42.{self.env}"
-            f"/oauth/token"
+        Args:
+            auth: An authentication object.
+            order_parameters: A dictionary for the order configuration.
+
+        Returns:
+            Order: The placed order.
+        """
+        url = host.endpoint(f"/v2/orders?workspaceId={auth.workspace_id}")
+        response_json = auth.request(
+            request_type="POST",
+            url=url,
+            data=_translate_construct_parameters(order_parameters),
         )
-        payload = "grant_type=client_credentials"
-        headers = {
-            "Content-Type": "application/x-www-form-urlencoded",
-            "cache-control": "no-cache",
-        }
-        token_response = requests.request("POST", url, data=payload, headers=headers)
-        token_response.raise_for_status()
-        token = json.loads(token_response.text)
-        # pylint: disable=attribute-defined-outside-init
-        self.token = token["data"]["accessToken"]
+        if response_json["errors"]:
+            message = response_json["errors"][0]["message"]
+            raise ValueError(f"Order was not placed: {message}")
+        order_id = response_json["results"][0]["id"]
+        order = cls(auth=auth, order_id=order_id, order_parameters=order_parameters)
+        logger.info("Order %s is now %s.", order.order_id, order.status)
+        return order
 
     @staticmethod
-    def _generate_headers(token: str) -> Dict[str, str]:
-        version = (
-            Path(__file__)
-            .resolve()
-            .parent.joinpath("_version.txt")
-            .read_text(encoding="utf-8")
-        )
-        headers = {
-            "Content-Type": "application/json",
-            "Authorization": f"Bearer {token}",
-            "cache-control": "no-cache",
-            "X-UP42-info": f"python/{version}",
-        }
-        return headers
-
-    # pylint: disable=dangerous-default-value
-    def _request_helper(
-        self, request_type: str, url: str, data: Dict = {}, querystring: Dict = {}
-    ) -> requests.Response:
+    def estimate(auth: up42_auth.Auth, order_parameters: OrderParams) -> int:
         """
-        Helper function for the request, running the actual request with the correct headers.
+        Returns an estimation of the cost of an order.
 
         Args:
-            request_type: 'GET', 'POST', 'PUT', 'PATCH', 'DELETE'
-            url: The requests url.
-            data: The payload, e.g. dictionary with job parameters etc.
-            querystring: The querystring.
+            auth: An authentication object.
+            order_parameters: A dictionary for the order configuration.
 
         Returns:
-            The request response.
+            int: The estimated cost of the order
         """
-        headers = self._generate_headers(self.token)
-        if querystring == {}:
-            response = requests.request(
-                method=request_type, url=url, data=json.dumps(data), headers=headers
-            )
-        else:
-            response = requests.request(
-                method=request_type,
-                url=url,
-                data=json.dumps(data),
-                headers=headers,
-                params=querystring,
-            )
-        logger.debug(response)
-        logger.debug(data)
-        return response
 
-    def _request(
-        self,
-        request_type: str,
-        url: str,
-        data: Union[Dict, List] = {},
-        querystring: Dict = {},
-        return_text: bool = True,
-    ) -> Union[str, requests.Response]:
+        url = host.endpoint("/v2/orders/estimate")
+        response_json = auth.request(
+            request_type="POST",
+            url=url,
+            data=_translate_construct_parameters(order_parameters),
+        )
+        estimated_credits: int = response_json["summary"]["totalCredits"]
+        logger.info(
+            "Order is estimated to cost %s UP42 credits (order_parameters: %s)", estimated_credits, order_parameters
+        )
+        return estimated_credits
+
+    def track_status(self, report_time: int = 120) -> str:
         """
-        Handles retrying the request and automatically gets a new token if the old
-        is invalid.
+        Continuously gets the order status until order is fulfilled or failed.
+
+        Internally checks every `report_time` (s) for the status and prints the log.
 
-        Retry is enabled by default, can be set to False as kwargs in Api().
+        Warning:
+            When placing orders of items that are in archive or cold storage,
+            the order fulfillment can happen up to **24h after order placement**.
+            In such cases,
+            please make sure to set an appropriate `report_time`.
 
         Args:
-            request_type: 'GET', 'POST', 'PUT', 'PATCH', 'DELETE'
-            url: The url to request.
-            data: The payload, e.g. dictionary with job parameters etc.
-            querystring: The querystring.
-            return_text: If true returns response text/json, false returns response.
-            retry: If False, after 5 minutes and invalid token will return 401
-                errors.
+            report_time: The interval (in seconds) when to get the order status.
 
         Returns:
-            The API response.
+            str: The final order status.
         """
-        if self.retry:
-            retryer = Retrying(
-                stop=stop_after_attempt(1),  # TODO: Find optimal retry solution
-                wait=wait_fixed(0),
-                retry=(
-                    retry_if_exception_type(requests.exceptions.HTTPError)
-                    | retry_if_exception_type(requests.exceptions.ConnectionError)
-                ),
-                after=self._get_token(),
-            )
-            response = retryer(
-                self._request_helper, request_type, url, data, querystring
-            )
-        else:
-            response = self._request_helper(request_type, url, data, querystring)  # type: ignore
 
-        # TODO: Uniform error format on backend, too many different cases.
-        # TODO: Put error messages in the specific functions.
-        if response.status_code != 200:
-            if response.status_code == 403:  # pylint: disable=no-else-raise
-                raise ValueError(
-                    "Access not possible, check if the given ids are correct, "
-                    "you have sufficient credits, "
-                    "that the referenced workflow/job object exists, "
-                    "and if the aoi is too big (>1000 sqkm)."
-                )
-            elif response.status_code == 404:
-                raise ValueError("Product not found!")
-
-        # Handle response text.
-        if return_text:
-            try:
-                response_text = json.loads(response.text)
-            except json.JSONDecodeError:  # e.g. JobTask logs are str format.
-                response_text = response.text
-
-            # Handle api error messages here before handling it in every single function.
-            # pylint: disable=no-else-raise
-            try:
-                if response_text["error"] is not None and response_text["data"] is None:
-                    raise ValueError(response_text["error"])
-                else:
-                    return response_text
-            except (
-                KeyError,
-                TypeError,
-            ):  # Catalog search, JobTask logs etc. does not have the usual {"data":"",
-                # "error":""} format.
-                return response_text
+        def substatus_messages(substatus: str) -> str:
+            substatus_user_messages = {
+                "FEASIBILITY_WAITING_UPLOAD": "Wait for feasibility.",
+                "FEASIBILITY_WAITING_RESPONSE": "Feasibility is ready.",
+                "QUOTATION_WAITING_UPLOAD": "Wait for quotation.",
+                "QUOTATION_WAITING_RESPONSE": "Quotation is ready",
+                "QUOTATION_ACCEPTED": "In progress.",
+            }
+
+            if substatus in substatus_user_messages:
+                message = substatus_user_messages[substatus]
+                return f"{substatus}, {message}"
+            return f"{substatus}"
+
+        logger.info("Tracking order status, reporting every %s seconds...", report_time)
+        time_asleep = 0
+
+        # check order details and react for tasking orders.
+
+        while not self.is_fulfilled:
+            status = self.status
+            substatus_message = (
+                substatus_messages(self.order_details.get("subStatus", "")) if self.info["type"] == "TASKING" else ""
+            )
+            if status in ["PLACED", "BEING_FULFILLED"]:
+                if time_asleep != 0 and time_asleep % report_time == 0:
+                    logger.info("Order is %s! - %s", status, self.order_id)
+                    logger.info(substatus_message)
+
+            elif status in ["FAILED", "FAILED_PERMANENTLY"]:
+                logger.info("Order is %s! - %s", status, self.order_id)
+                raise ValueError("Order has failed!")
+
+            time.sleep(report_time)
+            time_asleep += report_time
 
-        else:  # E.g. for DELETE
-            return response
+        logger.info("Order is fulfilled successfully! - %s", self.order_id)
+        return self.status
```

### Comparing `up42-py-0.9.3/up42/utils.py` & `up42_py-1.0.0/up42/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,425 +1,403 @@
 import copy
+import datetime
+import functools
+import importlib.metadata
+import json
 import logging
-from typing import Dict, List, Union, Tuple
-from pathlib import Path
-import tempfile
+import pathlib
 import tarfile
-import math
+import tempfile
+import warnings
+import zipfile
+from typing import List, Optional, Union, cast
+from urllib import parse
 
-import folium
-from folium.plugins import Draw
-from geopandas import GeoDataFrame
-import shapely
-import rasterio
-from rasterio.plot import show
-from shapely.geometry import Point, Polygon
-from geojson import Feature, FeatureCollection
-from geojson import Polygon as geojson_Polygon
+import geojson  # type: ignore
+import geopandas  # type: ignore
 import requests
-from tqdm import tqdm
-import matplotlib.pyplot as plt
+import shapely  # type: ignore
+import tqdm
+from shapely import geometry  # type: ignore
 
+TIMEOUT = 120  # seconds
+CHUNK_SIZE = 1024
 
-LOG_FORMAT = "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
+
+def get_filename(signed_url: str, default_filename: str) -> str:
+    """
+    Returns the filename from the signed URL
+    """
+    parsed_url = parse.urlparse(signed_url)
+    extension = pathlib.Path(parsed_url.path).suffix
+    try:
+        file_name = parse.parse_qs(parsed_url.query)["response-content-disposition"][0].split("filename=")[1]
+        return f"{file_name}{extension}"
+    except (IndexError, KeyError):
+        warnings.warn(
+            f"Unable to extract filename from URL. Using default filename: {default_filename}",
+            UserWarning,
+        )
+        return f"{default_filename}{extension}"
 
 
-def get_logger(name, level=logging.INFO):
+def get_logger(
+    name: str,
+    level=logging.INFO,
+    verbose: bool = False,
+):
     """
     Use level=logging.CRITICAL to disable temporarily.
     """
-    logger = logging.getLogger(name)  # pylint: disable=redefined-outer-name
-    logger.setLevel(level)
+    inner_logger = logging.getLogger(name)
+    inner_logger.setLevel(level)
     # create console handler and set level to debug
     ch = logging.StreamHandler()
     ch.setLevel(level)
-    formatter = logging.Formatter(LOG_FORMAT)
+    if verbose:
+        log_format = "%(asctime)s - %(name)s - %(levelname)s - %(message)"
+    else:
+        # hide logger module & level, truncate log messages > 2000 characters (e.g. huge geometries)
+        log_format = "%(asctime)s - %(message).2000s"
+    formatter = logging.Formatter(log_format)
     ch.setFormatter(formatter)
-    logger.addHandler(ch)
-    logger.propagate = False
-    return logger
+    inner_logger.addHandler(ch)
+    inner_logger.propagate = False
+    return inner_logger
 
 
 logger = get_logger(__name__)
 
 
-def download_results_from_gcs(
-    download_url: str, output_directory: Union[str, Path]
+def deprecation(
+    replacement_name: str,
+    version: str,
+    extra_message: str = "",
+):
+    """
+    Decorator for custom deprecation warnings.
+
+    Args:
+        replacement_name: Name of the replacement function.
+        version: The package version in which the deprecation will happen.
+        extra_message: Optional message after default deprecation warning.
+    """
+
+    def actual_decorator(func):
+        @functools.wraps(func)
+        def wrapper(*args, **kwargs):
+            message = (
+                f"`{func.__name__}` will be deprecated in version {version}, "
+                f"use `{replacement_name}` instead! {extra_message}"
+            )
+            warnings.warn(message, DeprecationWarning, stacklevel=2)
+            return func(*args, **kwargs)
+
+        return wrapper
+
+    return actual_decorator
+
+
+def download_from_gcs_unpack(
+    download_url: str,
+    output_directory: Union[str, pathlib.Path],
 ) -> List[str]:
     """
-    General download function for results of job and jobtask from cloud storage
+    General download function for results of storage assets, job & jobtask from cloud storage
     provider.
 
     Args:
         download_url: The signed gcs url to download.
         output_directory: The file output directory, defaults to the current working
             directory.
     """
-    output_directory = Path(output_directory)
-
     # Download
-    tgz_file = tempfile.mktemp()
-    with open(tgz_file, "wb") as dst_tgz:
+    out_temp = tempfile.mkstemp()[1]
+    with open(out_temp, "wb") as dst:
         try:
-            r = requests.get(download_url)
+            r = requests.get(download_url, stream=True, timeout=TIMEOUT)
             r.raise_for_status()
-            for chunk in tqdm(r.iter_content(chunk_size=1024)):
+            for chunk in tqdm.tqdm(r.iter_content(chunk_size=CHUNK_SIZE)):
                 if chunk:  # filter out keep-alive new chunks
-                    dst_tgz.write(chunk)
+                    dst.write(chunk)
         except requests.exceptions.HTTPError as err:
-            logger.debug("Connection error, please try again! %s", err)
-            raise requests.exceptions.HTTPError(
-                f"Connection error, please try again! {err}"
-            )
-
-    # Unpack and exclude data.json
-    out_filepaths: List[str] = []
-    with tarfile.open(tgz_file) as tar:
-        members = tar.getmembers()
-        files = [f for f in members if f.isfile()]
-        for file in files:
-            f = tar.extractfile(file)
-            content = f.read()  # type: ignore
-            out_fp = output_directory / f"{Path(file.name).name}"
-            with open(out_fp, "wb") as dst:
-                dst.write(content)
-            out_filepaths.append(str(out_fp))
-
+            error_message = f"Connection error, please try again! {err}"
+            logger.debug(error_message)
+            raise requests.exceptions.HTTPError(error_message)
+
+    # Unpack
+    # Order results are zip, job results are tgz(tar.gzipped)
+    out_filepaths: List[pathlib.Path] = []
+    if tarfile.is_tarfile(out_temp):
+        with tarfile.open(out_temp) as tar_file:
+            for tar_member in tar_file.getmembers():
+                if tar_member.isfile():
+                    # Avoid up42 inherent output/ .. directory
+                    if "output/" in tar_member.name:
+                        tar_member.name = tar_member.name.split("output/")[1]
+                    tar_file.extract(tar_member, output_directory)
+                    out_filepaths.append(pathlib.Path(output_directory) / tar_member.name)
+    elif zipfile.is_zipfile(out_temp):
+        with zipfile.ZipFile(out_temp) as zip_file:
+            for zip_info in zip_file.infolist():
+                if not zip_info.filename.endswith("/"):
+                    # Avoid up42 inherent output/ .. directory
+                    if "output/" in zip_info.filename:
+                        zip_info.filename = zip_info.filename.split("output/")[1]
+                    zip_file.extract(zip_info, output_directory)
+                    out_filepaths.append(pathlib.Path(output_directory) / zip_info.filename)
+    else:
+        raise ValueError("Downloaded file is not a TGZ/TAR or ZIP archive.")
     logger.info(
         "Download successful of %s files to output_directory '%s': %s",
         len(out_filepaths),
         output_directory,
-        [Path(p).name for p in out_filepaths],
-    )
-    return out_filepaths
-
-
-def folium_base_map(
-    lat: float = 52.49190032214706,
-    lon: float = 13.39117252959244,
-    zoom_start: int = 14,
-    width_percent: str = "95%",
-    layer_control=False,
-) -> folium.Map:
-    """Provides a folium map with basic features and UP42 logo."""
-    mapfigure = folium.Figure(width=width_percent)
-    m = folium.Map(location=[lat, lon], zoom_start=zoom_start, crs="EPSG3857").add_to(
-        mapfigure
-    )
-
-    tiles = (
-        "https://server.arcgisonline.com/ArcGIS/rest/services/World_Imagery"
-        "/MapServer/tile/{z}/{y}/{x}.png"
+        [p.name for p in out_filepaths],
     )
-    attr = (
-        "Tiles &copy; Esri &mdash; Source: Esri, i-cubed, USDA, USGS, "
-        "AEX, GeoEye, Getmapping, Aerogrid, IGN, IGP, UPR-EGP, and the "
-        "GIS User Community"
-    )
-    folium.TileLayer(tiles=tiles, attr=attr, name="Satellite - ESRI").add_to(m)
-
-    formatter = "function(num) {return L.Util.formatNum(num, 4) + ' ';};"
-    folium.plugins.MousePosition(
-        position="bottomright",
-        separator=" | ",
-        empty_string="NaN",
-        lng_first=True,
-        num_digits=20,
-        prefix="lon/lat:",
-        lat_formatter=formatter,
-        lng_formatter=formatter,
-    ).add_to(m)
-
-    folium.plugins.MiniMap(
-        tile_layer="OpenStreetMap", position="bottomright", zoom_level_offset=-6
-    ).add_to(m)
-    folium.plugins.Fullscreen().add_to(m)
-    folium.plugins.FloatImage(
-        image="https://cdn-images-1.medium.com/max/140/1*XJ_B7ur_c8bYKniXpKVpWg@2x.png",
-        bottom=90,
-        left=88,
-    ).add_to(m)
-
-    if layer_control:
-        folium.LayerControl(position="bottomleft", collapsed=False, zindex=100).add_to(
-            m
-        )
-        # If adding additional layers outside of the folium base map function, don't
-        # use this one here. Causes an empty map.
-    return m
+    return [str(p) for p in out_filepaths]
 
 
-class DrawFoliumOverride(Draw):
-    def render(self, **kwargs):
-        # pylint: disable=import-outside-toplevel
-        from branca.element import CssLink, Element, Figure, JavascriptLink
+def download_gcs_not_unpack(download_url: str, output_directory: Union[str, pathlib.Path]) -> List[str]:
+    """
+    General download function for assets, job and jobtasks from cloud storage
+    provider.
 
-        super(DrawFoliumOverride, self).render(**kwargs)
+    Args:
+        download_url: The signed gcs url to download.
+        output_directory: The file output directory, defaults to the current working
+            directory.
+    """
+    file_name = get_filename(download_url, default_filename="output")
+    out_fp = pathlib.Path().joinpath(output_directory, file_name)
+    # Download
+    with open(out_fp, "wb") as dst:
+        try:
+            r = requests.get(download_url, stream=True, timeout=TIMEOUT)
+            r.raise_for_status()
+            for chunk in tqdm.tqdm(r.iter_content(chunk_size=CHUNK_SIZE)):
+                if chunk:  # filter out keep-alive new chunks
+                    dst.write(chunk)
+        except requests.exceptions.HTTPError as err:
+            logger.debug("Connection error, please try again! %s", err)
+            raise requests.exceptions.HTTPError(f"Connection error, please try again! {err}")
 
-        figure = self.get_root()
-        assert isinstance(figure, Figure), (
-            "You cannot render this Element " "if it is not in a Figure."
-        )
+        logger.info("Successfully downloaded the file at %s", out_fp)
+        return [str(out_fp)]
 
-        figure.header.add_child(
-            JavascriptLink(
-                "https://cdnjs.cloudflare.com/ajax/libs/leaflet.draw/1.0.2/"
-                "leaflet.draw.js"
-            )
-        )  # noqa
-        figure.header.add_child(
-            CssLink(
-                "https://cdnjs.cloudflare.com/ajax/libs/leaflet.draw/1.0.2/"
-                "leaflet.draw.css"
-            )
-        )  # noqa
 
-        export_style = """
-            <style>
-                #export {
-                    position: absolute;
-                    top: 270px;
-                    left: 11px;
-                    z-index: 999;
-                    padding: 6px;
-                    border-radius: 3px;
-                    box-sizing: border-box;
-                    color: #333;
-                    background-color: #fff;
-                    border: 2px solid rgba(0,0,0,0.5);
-                    box-shadow: None;
-                    font-family: 'Helvetica Neue';
-                    cursor: pointer;
-                    font-size: 17px;
-                    text-decoration: none;
-                    text-align: center;
-                    font-weight: bold;
-                }
-            </style>
-        """
-        # TODO: How to change hover color?
-        export_button = """<a href='#' id='export'>Export as<br/>GeoJson</a>"""
-        if self.export:
-            figure.header.add_child(Element(export_style), name="export")
-            figure.html.add_child(Element(export_button), name="export_button")
-
-
-def _plot_images(
-    plot_file_format: List[str],
-    figsize: Tuple[int, int] = (8, 8),
-    filepaths: List[Union[str, Path]] = None,
-    titles: List[str] = None,
-) -> None:
+def format_time(date: Optional[Union[str, datetime.datetime]], set_end_of_day=False):
     """
-    Plots image data (quicklooks or results)
+    Formats date isostring to datetime string format
 
     Args:
-        plot_file_format: List of accepted image file formats e.g. [".tif"]
-        figsize: matplotlib figure size.
-        filepaths: Paths to images to plot. Optional, by default picks up the last
-            downloaded results.
-        titles: Optional list of titles for the subplots.
-
+        date: datetime object or isodatetime string e.g. "YYYY-MM-DD" or "YYYY-MM-DDTHH:MM:SS".
+        set_end_of_day: Sets the date to end of day, as required for most image archive searches. Only applies for
+            type date string without time, e.g. "YYYY-MM-DD", not explicit datetime object or time of day.
     """
-    if not isinstance(filepaths, list):
-        filepaths = [filepaths]  # type: ignore
-    filepaths = [Path(path) for path in filepaths]
-
-    imagepaths = [
-        path for path in filepaths if str(path.suffix) in plot_file_format  # type: ignore
-    ]
-    if not imagepaths:
-        raise ValueError(
-            f"This function only plots files of format {plot_file_format}."
-        )
-
-    if not titles:
-        titles = [Path(fp).stem for fp in imagepaths]
-    if not isinstance(titles, list):
-        titles = [titles]  # type: ignore
-
-    if len(imagepaths) < 2:
-        nrows, ncols = 1, 1
+    if isinstance(date, str):
+        has_time_of_day = len(date) > 11
+        date = datetime.datetime.fromisoformat(date)
+        if not has_time_of_day and set_end_of_day:
+            date = datetime.datetime.combine(date.date(), datetime.time(23, 59, 59, 999999))
+    elif isinstance(date, datetime.datetime):
+        pass
     else:
-        ncols = 3
-        nrows = int(math.ceil(len(imagepaths) / float(ncols)))
+        raise ValueError("date needs to be of type datetime or isoformat date string!")
 
-    _, axs = plt.subplots(nrows=nrows, ncols=ncols, figsize=figsize)
-    if len(imagepaths) > 1:
-        axs = axs.ravel()
-    else:
-        axs = [axs]
-    for idx, (fp, title) in enumerate(zip(imagepaths, titles)):
-        with rasterio.open(fp) as src:
-            img_array = src.read()[:3, :, :]
-            # TODO: Handle more band configurations.
-            # TODO: add histogram equalization?
-            show(
-                img_array, transform=src.transform, title=title, ax=axs[idx],
-            )
-        axs[idx].set_axis_off()
-    plt.tight_layout()
-    plt.show()
+    return date.strftime("%Y-%m-%dT%H:%M:%SZ")
 
 
 def any_vector_to_fc(
     vector: Union[
-        Dict, Feature, FeatureCollection, List, GeoDataFrame, Polygon, Point,
+        geojson.FeatureCollection,
+        geojson.Feature,
+        dict,
+        list,
+        geopandas.GeoDataFrame,
+        geometry.Polygon,
+        geometry.Point,
     ],
     as_dataframe: bool = False,
-) -> Union[Dict, GeoDataFrame]:
+) -> Union[dict, geopandas.GeoDataFrame]:
     """
     Gets a uniform feature collection dictionary (with fc and f bboxes) from any input vector type.
 
     Args:
-        vector: One of Dict, FeatureCollection, Feature, List of bounds coordinates,
-            GeoDataFrame, shapely.geometry.Polygon, shapely.geometry.Point.
-            All assume EPSG 4326 and Polygons!
+        vector: One of FeatureCollection, Feature, dict (geojson geometry), list (bounds coordinates),
+            GeoDataFrame, shapely.Polygon, shapely.Point. All assume EPSG 4326!
         as_dataframe: GeoDataFrame output with as_dataframe=True.
     """
     if not isinstance(
         vector,
         (
+            geojson.FeatureCollection,
+            geojson.Feature,
             dict,
-            FeatureCollection,
-            Feature,
-            geojson_Polygon,
             list,
-            GeoDataFrame,
-            Polygon,
-            Point,
+            geopandas.GeoDataFrame,
+            geometry.Polygon,
+            geometry.Point,
+            geojson.Polygon,
         ),
     ):
         raise ValueError(
-            "The provided geometry muste be a FeatureCollection, Feature, Dict, geopandas "
-            "Dataframe, shapely Polygon, shapely Point or a list of 4 bounds coordinates."
+            "The provided geometry must be a FeatureCollection, Feature, dict (geojson geometry), geopandas "
+            "dataframe, shapely Polygon, Point or a list (bounds coordinates)."
         )
 
-    ## Transform all possible input geometries to a uniform feature collection.
-    vector = copy.deepcopy(vector)  # otherwise changes input geometry.
-    if isinstance(vector, (dict, FeatureCollection, Feature)):
+    vector = copy.deepcopy(vector)  # avoid altering input geometry
+    if isinstance(vector, (dict, geojson.FeatureCollection, geojson.Feature)):
         try:
             if vector["type"] == "FeatureCollection":
-                df = GeoDataFrame.from_features(vector, crs=4326)
+                df = geopandas.GeoDataFrame.from_features(vector, crs=4326)
             elif vector["type"] == "Feature":
-                df = GeoDataFrame.from_features(FeatureCollection([vector]), crs=4326)
-            elif vector["type"] == "Polygon":  # Geojson geometry
-                df = GeoDataFrame.from_features(
-                    FeatureCollection([Feature(geometry=vector)]), crs=4326
+                df = geopandas.GeoDataFrame.from_features(geojson.FeatureCollection([vector]), crs=4326)
+            else:  # Only geometry dict of Feature
+                df = geopandas.GeoDataFrame.from_features(
+                    geojson.FeatureCollection([geojson.Feature(geometry=vector)]),
+                    crs=4326,
                 )
-        except KeyError:
-            raise ValueError(
-                "Provided geometry dictionary has to include a featurecollection or feature."
-            )
+        except KeyError as e:
+            raise ValueError("Provided geometry dictionary has to include a FeatureCollection or Feature.") from e
     else:
         if isinstance(vector, list):
             if len(vector) == 4:
                 box_poly = shapely.geometry.box(*vector)
-                df = GeoDataFrame({"geometry": [box_poly]}, crs=4326)
+                df = geopandas.GeoDataFrame({"geometry": [box_poly]}, crs=4326)
             else:
                 raise ValueError("The list requires 4 bounds coordinates.")
-        elif isinstance(vector, Polygon):
-            df = GeoDataFrame({"geometry": [vector]}, crs=4326)
-        elif isinstance(vector, Point):
-            df = GeoDataFrame(
-                {"geometry": [vector.buffer(0.00001)]}, crs=4326
-            )  # Around 1m buffer # TODO: Find better solution than small buffer?
-        elif isinstance(vector, GeoDataFrame):
+        elif isinstance(vector, (geometry.Polygon, geometry.Point)):
+            df = geopandas.GeoDataFrame({"geometry": [vector]}, crs=4326)
+        elif isinstance(vector, geopandas.GeoDataFrame):
             df = vector
-            if df.crs.to_string() != "EPSG:4326":
-                df = df.to_crs(epsg=4326)
+            try:
+                if df.crs.to_string() != "EPSG:4326":
+                    df = df.to_crs(epsg=4326)
+            except AttributeError as e:
+                raise AttributeError("GeoDataFrame requires a CRS.") from e
 
-    df.geometry = df.geometry.buffer(0)
     if as_dataframe:
         return df
     else:
         fc = df.__geo_interface__
         return fc
 
 
-def fc_to_query_geometry(
-    fc: Union[Dict, FeatureCollection],
-    geometry_operation: str,
-    squash_multiple_features: str = "union",
-) -> Union[List, dict]:
-    """
-    From a feature collection (one or multiple polygons) & any geometry_operation,
-    gets a single query geometry for the workflow parameters.
-    Returns either a list of bounds or a geojson Polygon (as dict) depending on geometry_operation.
-    If an input fc with multiple features is provided, it gets squashed to a single
-    output geometry, either by taking the first geometry or the union (footprint) of all geometries,
-    depending on handle_multiple_features.
-
-    Examples (geometry & geometry_operation > always returns a single feature):
-        Single input geometries:
-            - feature & "intersects/contains" > same as input feature
-            - feature & "bbox" > rectangular feature that is the bbox of the input feature
-        Multiple input geometries:
-            - features & "intersects/contains" > feature of first object in fc or union
-                of fc (depending on "handle_multiple_features")
-            - features & "bbox" > rectangular feature of first object in fc or union of
-                fc (depending on "handle_multiple_features")
+def validate_fc_up42_requirements(fc: Union[dict, geojson.FeatureCollection]):
+    """
+    Validate the feature collection if it fits UP42 geometry requirements.
+    """
+    geometry_error = "UP42 only accepts single geometries, the provided geometry {}."
+    if len(fc["features"]) != 1:
+        raise ValueError(geometry_error.format("contains multiple geometries"))
+
+    fc_type = fc["features"][0]["geometry"]["type"]
+    if fc_type != "Polygon":
+        raise ValueError(geometry_error.format(f"is a {fc_type}"))
+
+
+def fc_to_query_geometry(fc: Union[dict, geojson.FeatureCollection], geometry_operation: str) -> Union[List, dict]:
+    """
+    From a feature collection with a single feature, depending on the geometry_operation,
+    returns the feature as a list of bounds coordinates or a GeoJSON Polygon (as dict).
 
     Args:
         fc: feature collection
         geometry_operation: One of "bbox", "intersects", "contains".
-        squash_multiple_features: One of "union" (default, footprint of all features)
-            or "first" (takes the first feature.
 
     Returns:
-
+        The feature as a list of bounds coordinates or a GeoJSON Polygon (as dict)
     """
-    if geometry_operation not in ["bbox", "intersects", "contains"]:
+    validate_fc_up42_requirements(fc)
+    feature = fc["features"][0]
+
+    if geometry_operation == "bbox":
+        try:
+            query_geometry = list(feature["bbox"])
+        except KeyError:
+            query_geometry = list(shapely.geometry.shape(feature["geometry"]).bounds)
+    elif geometry_operation in ["intersects", "contains"]:
+        query_geometry = feature["geometry"]
+    else:
         raise ValueError(
-            "geometry_operation needs to be one of bbox", "intersects", "contains",
+            "geometry_operation needs to be one of bbox, intersects or contains!",
         )
+
+    return query_geometry
+
+
+def autocomplete_order_parameters(order_parameters: dict, schema: dict):
+    """
+    Adds missing required catalog/tasking order parameters and logs parameter suggestions.
+
+    Args:
+        order_parameters: The initial order_parameters, in format
+            {"dataProduct": data_product_id, "params" : {...}}
+        schema: The data product parameter schema from .get_data_product_schema
+        The existing order parameter params
+
+    Returns:
+        The order parameters with complete params
+    """
+    additional_params = {param: None for param in schema["required"] if param not in order_parameters["params"]}
+    order_parameters["params"] = dict(order_parameters["params"], **additional_params)
+
+    # Log message help for parameter selection
     try:
-        if fc["type"] != "FeatureCollection":
-            raise ValueError("Geometry argument only supports Feature Collections!")
-    except (KeyError, TypeError):
-        raise ValueError("Geometry argument only supports Feature Collections!")
-
-    # TODO: Handle multipolygons
-
-    # With the now uniform feature collection, decide to return a feature or list of bounds (bbox).
-    if len(fc["features"]) == 1:
-        f = fc["features"][0]
-        if geometry_operation == "bbox":
-            try:
-                query_geometry = list(f["bbox"])
-            except KeyError:
-                query_geometry = list(shapely.geometry.shape(f["geometry"]).bounds)
-        elif geometry_operation in ["intersects", "contains"]:
-            query_geometry = f["geometry"]
-    # In case of multiple geometries transform the feature collection a single aoi
-    # geometry via handle_multiple_features method.
-    else:
-        logger.info(
-            "The provided geometry contains multiple geometries, the %s feature is "
-            "taken instead.",
-            squash_multiple_features,
+        for param in additional_params.keys():
+            if param in ["aoi", "geometry"]:
+                continue
+            elif "allOf" in schema["properties"][param]:  # has further definitions key
+                potential_values = [x["const"] for x in schema["definitions"][param]["anyOf"]]
+                logger.info("As `%s` select one of %s", param, potential_values)
+            else:
+                # Full information for simple parameters
+                del schema["properties"][param]["title"]
+                logger.info("As `%s` select `%s`", param, schema["properties"][param])
+    except KeyError as exc:
+        raise KeyError("Please reach out to UP42 Support (support@up42.com)") from exc
+    return order_parameters
+
+
+def replace_page_query(url: str, new_page: int) -> str:
+    """
+    Handle pagination replacement in an encoded url
+    Args:
+        url (str): a url with query parameters including page
+        new_page (int): the desired page starting at 0 to include in the url
+
+    Returns:
+        str: the url with the new page parameter.
+    """
+    parsed_url = parse.urlparse(url)
+    query_params = parse.parse_qs(parsed_url.query)
+    query_params["page"] = [str(new_page)]
+
+    # Update the query string with the modified parameters
+    encoded_query = parse.urlencode(query_params, doseq=True)
+
+    # Reconstruct the modified URL
+    return parse.urlunparse(
+        (
+            parsed_url.scheme,
+            parsed_url.netloc,
+            parsed_url.path,
+            parsed_url.params,
+            encoded_query,
+            parsed_url.fragment,
         )
-        if geometry_operation == "bbox":
-            if squash_multiple_features == "union":
-                try:
-                    query_geometry = list(fc["bbox"])
-                except KeyError:
-                    query_geometry = list(
-                        GeoDataFrame.from_features(fc, crs=4326).total_bounds
-                    )
-            elif squash_multiple_features == "first":
-                try:
-                    query_geometry = fc["features"][0]["bbox"]
-                except KeyError:
-                    query_geometry = list(
-                        shapely.geometry.shape(fc["features"][0]["geometry"]).bounds
-                    )
-        elif geometry_operation in [
-            "intersects",
-            "contains",
-        ]:  # pylint: disable=no-else-raise
-            if squash_multiple_features == "union":
-                union_poly = GeoDataFrame.from_features(fc, crs=4326).unary_union
-                query_geometry = shapely.geometry.mapping(union_poly)
-            elif squash_multiple_features == "first":
-                query_geometry = fc["features"][0]["geometry"]
-    return query_geometry
+    )
+
+
+def get_up42_py_version():
+    """Get the version of the up42-py package."""
+    return importlib.metadata.version("up42-py")
+
+
+def read_json(path_or_dict: Union[dict, str, pathlib.Path, None]) -> Optional[dict]:
+    if path_or_dict and isinstance(path_or_dict, (str, pathlib.Path)):
+        try:
+            with open(path_or_dict, encoding="utf-8") as file:
+                return json.load(file)
+        except FileNotFoundError as ex:
+            raise ValueError(f"File {path_or_dict} does not exist!") from ex
+    return cast(Optional[dict], path_or_dict)
```

### Comparing `up42-py-0.9.3/up42/workflow.py` & `up42_py-1.0.0/up42/catalog.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,509 +1,512 @@
-import json
-import logging
-from collections import Counter
-from pathlib import Path
-from typing import Dict, List, Union, Optional
-
-from geopandas import GeoDataFrame
-from shapely.geometry import Point, Polygon
-from geojson import Feature, FeatureCollection
-from geojson import Polygon as geojson_Polygon
-from tqdm import tqdm
-
-from .auth import Auth
-from .job import Job
-from .tools import Tools
-from .utils import get_logger, any_vector_to_fc, fc_to_query_geometry
-
-logger = get_logger(__name__)
-
-
-class Workflow(Tools):
-    def __init__(self, auth: Auth, project_id: str, workflow_id: str):
-        """
-        The Workflow class can query all available and spawn new jobs for
-        an UP42 Workflow and helps to find and set the the workflow tasks, parameters
-        and aoi.
-        """
-        self.auth = auth
-        self.project_id = project_id
-        self.workflow_id = workflow_id
-        if self.auth.get_info:
-            self.info = self._get_info()
-
-    def __repr__(self):
-        return (
-            f"Workflow(workflow_id={self.workflow_id}, project_id={self.project_id}, "
-            f"auth={self.auth}, info={self.info})"
-        )
-
-    def _get_info(self) -> Dict:
-        """Gets metadata info from an existing workflow"""
-        url = (
-            f"{self.auth._endpoint()}/projects/{self.project_id}/workflows/"
-            f"{self.workflow_id}"
-        )
-        response_json = self.auth._request(request_type="GET", url=url)
-        self.info = response_json["data"]
-        return self.info
-
-    def get_compatible_blocks(self) -> Dict:
-        """
-        Gets all compatible blocks for the current workflow. If the workflow is empty
-        it will provide all data blocks, if the workflow already has workflow tasks, it
-        will provide the compatible blocks for the last workflow task in the workflow.
-
-        Currently no data blocks can be attached to other data blocks.
-        """
-        last_task = list(self.get_workflow_tasks(basic=True).keys())[-1]  # type: ignore
-        url = (
-            f"{self.auth._endpoint()}/projects/{self.project_id}/workflows/{self.workflow_id}/"
-            f"compatible-blocks?parentTaskName={last_task}"
-        )
-        response_json = self.auth._request(request_type="GET", url=url)
-        compatible_blocks = response_json["data"]["blocks"]
-        # TODO: Plot diagram of current workflow in green, attachable blocks in red.
-        compatible_blocks = {
-            block["name"]: block["blockId"] for block in compatible_blocks
-        }
-        return compatible_blocks
+"""
+Catalog search functionality
+"""
 
-    def get_workflow_tasks(self, basic: bool = False) -> Union[List, Dict]:
-        """
-        Get the workflow-tasks of the workflow (Blocks in a workflow are called workflow_tasks)
+import pathlib
+import warnings
+from typing import Any, Dict, List, Optional, Union
 
-        Args:
-            basic: If selected returns a simplified task-name : task-id` version.
+import geojson  # type: ignore
+import geopandas  # type: ignore
+import tqdm
+from shapely import geometry as geom  # type: ignore
 
-        Returns:
-            The workflow task info.
-        """
-        url = (
-            f"{self.auth._endpoint()}/projects/{self.project_id}/workflows/"
-            f"{self.workflow_id}/tasks"
-        )
-        response_json = self.auth._request(request_type="GET", url=url)
-        tasks = response_json["data"]
-        logger.info("Got %s tasks/blocks in workflow %s.", len(tasks), self.workflow_id)
+from up42 import auth as up42_auth
+from up42 import host, order, utils
 
-        if basic:
-            return {task["name"]: task["id"] for task in tasks}
-        else:
-            return tasks
+logger = utils.get_logger(__name__)
 
-    def _construct_full_workflow_tasks_dict(
-        self, input_tasks: Union[List]
-    ) -> List[Dict]:
-        """
-        Constructs the full workflow task definition from a simplified version.
-        Accepts blocks ids, block names, block display names & combinations of them.
 
-        Args:
-            input_tasks: List of block names, block ids, or block display names.
+class CatalogBase:
+    """
+    The base for Catalog and Tasking class, shared functionality.
+    """
 
-        Returns:
-            The full workflow task definition.
-
-        Example:
-            ```python
-            input_tasks = ["sobloo-s2-l1c-aoiclipped",
-                           "tiling"]
-            ```
-
-            ```python
-            input_tasks = ["a2daaab4-196d-4226-a018-a810444dcad1",
-                           "4ed70368-d4e1-4462-bef6-14e768049471"]
-            ```
+    def __init__(self, auth: up42_auth.Auth):
+        self.auth = auth
+        self.type: Optional[str] = None
 
-            ```python
-            input_tasks = ["Sentinel-2 L1C MSI AOI clipped",
-                           "Raster Tiling"]
-            ```
+    def get_data_products(self, basic: bool = True) -> Union[Dict, List[Dict]]:
         """
-        full_input_tasks_definition = []
-
-        # Get public + custom blocks.
-        logging.getLogger("up42.tools").setLevel(logging.CRITICAL)
-        blocks: Dict = self.get_blocks(basic=False)  # type: ignore
-        logging.getLogger("up42.tools").setLevel(logging.INFO)
-
-        # Get ids of the input tasks, regardless of the specified format.
-        blocks_id_name = {block["id"]: block["name"] for block in blocks}
-        blocks_name_id = {block["name"]: block["id"] for block in blocks}
-        blocks_displaynames_id = {block["displayName"]: block["id"] for block in blocks}
-
-        input_tasks_ids = []
-        for task in input_tasks:
-            if task in list(blocks_id_name.keys()):
-                input_tasks_ids.append(task)
-            elif task in list(blocks_name_id.keys()):
-                input_tasks_ids.append(blocks_name_id[task])
-            elif task in list(blocks_displaynames_id.keys()):
-                input_tasks_ids.append(blocks_displaynames_id[task])
-            else:
-                raise ValueError(
-                    f"The specified input task {task} does not match any "
-                    f"available block."
-                )
-
-        # Add first task, the data block.
-        data_task = {
-            "name": f"{blocks_id_name[input_tasks_ids[0]]}:1",
-            "parentName": None,
-            "blockId": input_tasks_ids[0],
-        }
-        full_input_tasks_definition.append(data_task)
-        previous_task_name = data_task["name"]
+        Get the available data product information for each collection. A data
+        product is the available data configurations for each collection,
+        e.g. Pleiades Display product.
 
-        # All all following (processing) blocks.
-        for block_id in input_tasks_ids[1:]:
-            # Check if multiple of the same block are in the input tasks definition,
-            # so that is does not get skipped as it has the same id.
-            counts = Counter([x["blockId"] for x in full_input_tasks_definition])
+        Args:
+            basic: A dictionary containing only the collection title,
+                name, host and available data product configurations,
+                default True.
+        """
+        url = host.endpoint("/data-products")
+        json_response = self.auth.request("GET", url)
+        unfiltered_products: list = json_response["data"]
+
+        products = []
+        for product in unfiltered_products:
+            if product["collection"]["type"] != self.type:
+                continue
+            try:
+                if not product["collection"]["isIntegrated"]:
+                    continue
+            except KeyError:
+                # isIntegrated potentially removed from future public API
+                pass
             try:
-                count_block = int(counts[block_id]) + 1
+                if not product["productConfiguration"]["isIntegrated"]:
+                    continue
             except KeyError:
-                count_block = 1
+                pass
+            products.append(product)
 
-            next_task = {
-                "name": f"{blocks_id_name[block_id]}:{count_block}",
-                "parentName": previous_task_name,
-                "blockId": block_id,
-            }
-            full_input_tasks_definition.append(next_task)
-            previous_task_name = next_task["name"]
-        return full_input_tasks_definition
+        if not basic:
+            return products
+        else:
+            collection_overview = {}
+            for product in products:
+                collection_title = product["collection"]["title"]
+                collection_name = product["collectionName"]
+                product_host = product["collection"]["host"]["name"]
+                data_product = {product["productConfiguration"]["title"]: product["id"]}
+
+                if collection_title not in collection_overview:
+                    collection_overview[collection_title] = {
+                        "collection": collection_name,
+                        "host": product_host,
+                        "data_products": data_product,
+                    }
+                else:
+                    # Add additional products for same collection
+                    collection_overview[collection_title]["data_products"][
+                        product["productConfiguration"]["title"]
+                    ] = product["id"]
+
+            return collection_overview
+
+    def get_data_product_schema(self, data_product_id: str) -> dict:
+        """
+        Gets the parameters schema of a data product to help
+        with the construction of the catalog/tasking order
+        parameters.
 
-    def add_workflow_tasks(self, input_tasks: Union[List[str], List[Dict]]) -> None:
+        Args:
+            data_product_id: The id of a catalog/tasking data product.
         """
-        Adds or overwrites workflow tasks in a workflow on UP42.
+        url = host.endpoint(f"/orders/schema/{data_product_id}")
+        json_response = self.auth.request("GET", url)
+        return json_response  # Does not contain APIv1 "data" key
 
-        Args:
-            input_tasks: The input tasks, specifying the blocks. Can be a list of the
-                block ids, block names or block display names (The name shown on the
-                [marketplace](https://marketplace.up42.com).
-
-        !!! Info
-            Using block ids specifies a specific version of the block that will be added
-            to the workflow. With block names or block display names, the most recent
-            version of a block will always be added.
+    def get_collections(self) -> Union[Dict, List]:
+        """
+        Get the available data collections.
+        """
+        url = host.endpoint("/collections")
+        json_response = self.auth.request("GET", url)
+        collections = [c for c in json_response["data"] if c["type"] == self.type]
+        return collections
 
-        Example:
-            ```python
-            input_tasks_simple = ['a2daaab4-196d-4226-a018-a810444dcad1',
-                                  '4ed70368-d4e1-4462-bef6-14e768049471']
-            ```
+    def place_order(
+        self,
+        order_parameters: Optional[Dict],
+        track_status: bool = False,
+        report_time: int = 120,
+        **kwargs,
+    ) -> order.Order:
+        """
+        Place an order.
 
-            ```python
-            input_tasks = ["sobloo-s2-l1c-aoiclipped", "tiling"]
-            ```
+        Args:
+            order_parameters: A dictionary like
+                {dataProduct: ..., "params": {"id": ..., "aoi": ...}}
+            track_status (bool): If set to True, will only return
+                the Order once it is `FULFILLED` or `FAILED`.
+            report_time (int): The interval (in seconds) to query
+                the order status if `track_status` is True.
+
+        Warning "Deprecated order parameters"
+            The use of the 'scene' and 'geometry' parameters for
+            the data ordering is deprecated. Please use the new
+            order_parameters parameter as described above.
+
+         Warning:
+            When placing orders of items that are in
+            archive or cold storage,
+            the order fulfillment can happen up to
+            **24h after order placement**.
+            In such cases, please make sure to set
+            an appropriate `report_time`.
+            You can also use `Order.track_status` on the
+            returned object to track the status later.
 
-            ```python
-            input_tasks = ["Sentinel-2 L1C MSI AOI clipped",
-                           "Raster Tiling"]
+        Returns:
+            Order class object of the placed order.
+        """
+        if "scene" in kwargs or "geometry" in kwargs:
+            # Deprecated, to be removed, use order_parameters.
+            message = (
+                "The use of the 'scene' and 'geometry' parameters "
+                "for the data ordering is deprecated. "
+                "Please use the new 'order_parameters' parameter."
+            )
+            warnings.warn(message, DeprecationWarning, stacklevel=2)
+        elif order_parameters is None:
+            raise ValueError("Please provide the 'order_parameters' parameter!")
+        placed_order = order.Order.place(self.auth, order_parameters)  # type: ignore
+        if track_status:
+            placed_order.track_status(report_time)
+        return placed_order
 
 
-        Optional: The input_tasks can also be provided as the full, detailed workflow task
-        definition (dict of block id, block name and parent block name). Always use :1
-        to be able to identify the order when two times the same workflow task is used.
-        The name is arbitrary, but best use the block name.
+class Catalog(CatalogBase):
+    """
+    The Catalog class enables access to the UP42 catalog
+    functionality (data archive search & ordering).
 
-        Example:
-            ```python
-            input_tasks_full = [{'name': 'sobloo-s2-l1c-aoiclipped:1',
-                                 'parentName': None,
-                                 'blockId': 'a2daaab4-196d-4226-a018-a810444dcad1'},
-                                {'name': 'sharpening:1',
-                                 'parentName': 'sobloo-s2-l1c-aoiclipped',
-                                 'blockId': '4ed70368-d4e1-4462-bef6-14e768049471'}]
-            ```
-        """
-        # Construct proper task definition from simplified input.
-        if isinstance(input_tasks[0], str) and not isinstance(input_tasks[0], dict):
-            input_tasks = self._construct_full_workflow_tasks_dict(input_tasks)
-
-        url = (
-            f"{self.auth._endpoint()}/projects/{self.project_id}/workflows/"
-            f"{self.workflow_id}/tasks/"
-        )
-        self.auth._request(request_type="POST", url=url, data=input_tasks)
-        logger.info("Added tasks to workflow: %r", input_tasks)
+    Use catalog:
+    ```python
+    catalog = up42.initialize_catalog()
+    ```
 
-    def get_parameters_info(self) -> Dict:
-        """
-        Gets infos about the workflow parameters of each block in the workflow to
-        make it easy to construct the desired parameters.
+    This class also inherits functions from the
+    [CatalogBase](catalogbase-reference.md) class.
+    """
 
-        Returns:
-            Workflow parameters info json.
-        """
-        workflow_parameters_info = {}
-        workflow_tasks = self.get_workflow_tasks()
-        for task in workflow_tasks:
-            task_name = task["name"]
-            task_default_parameters = task["block"]["parameters"]
-            workflow_parameters_info[task_name] = task_default_parameters
-        return workflow_parameters_info
+    def __init__(self, auth: up42_auth.Auth):
+        super().__init__(auth)
+        self.quicklooks: Optional[List[str]] = None
+        self.type: str = "ARCHIVE"
+        self.data_products: Optional[Dict] = None
 
-    def _get_default_parameters(self) -> Dict:
+    def estimate_order(self, order_parameters: Optional[Dict], **kwargs) -> int:
         """
-        Gets the default parameters for the workflow that can be directly used to
-        run a job. Excludes geometry operation and geometry of the data block.
-        """
-        default_workflow_parameters = {}
-
-        logger.setLevel(logging.CRITICAL)
-        workflow_tasks = self.get_workflow_tasks()
-        logger.setLevel(logging.INFO)
-        for task in workflow_tasks:
-            task_name = task["name"]
-            task_parameters = task["block"]["parameters"]
+        Estimate the cost of an order.
 
-            default_task_parameters = {}
-
-            for param_name, param_values in task_parameters.items():
-                if "default" in param_values and param_values["default"] is not None:
-                    default_task_parameters[param_name] = param_values["default"]
+        Args:
+            order_parameters: A dictionary like
+            {dataProduct: ..., "params": {"id": ..., "aoi": ...}}
 
-            default_workflow_parameters[task_name] = default_task_parameters
-        return default_workflow_parameters
+        Returns:
+            int: An estimated cost for the order in UP42 credits.
 
-    def construct_parameters(
-        self,
-        geometry: Optional[
-            Union[
-                Dict,
-                Feature,
-                FeatureCollection,
-                geojson_Polygon,
-                List,
-                GeoDataFrame,
-                Polygon,
-                Point,
-            ]
-        ] = None,
-        geometry_operation: Optional[str] = None,
-        handle_multiple_features: str = "footprint",
-        start_date: str = None,  # TODO: Other format? More time options?
-        end_date: str = None,
-        limit: int = None,
-        scene_ids: List = None,
-        order_ids: List[str] = None,
-    ) -> Dict:
-        """
-        Constructs workflow input parameters with a specified aoi, the default input parameters, and
-        optionally limit and order-ids. Further parameter editing needs to be done manually
-        via dict.update({key:value}).
+        Warning "Deprecated order parameters"
+            The use of the 'scene' and 'geometry' parameters for
+            the data estimation is deprecated. Please use the new
+            order_parameters parameter as described above.
+        """
+        if "scene" in kwargs or "geometry" in kwargs:
+            # Deprecated, to be removed, use order_parameters.
+            message = (
+                "The use of the 'scene' and 'geometry' parameters "
+                "for the data estimation is deprecated. "
+                "Please use the new 'order_parameters' parameter."
+            )
+            warnings.warn(message, DeprecationWarning, stacklevel=2)
+        elif order_parameters is None:
+            raise ValueError("Please provide the 'order_parameters' parameter!")
+        return order.Order.estimate(self.auth, order_parameters)  # type: ignore
+
+    @utils.deprecation("construct_search_parameters", "0.25.0")
+    def construct_parameters(self, **kwargs):  # pragma: no cover
+        """Deprecated, see construct_search_parameters"""
+        return self.construct_search_parameters(**kwargs)
+
+    @staticmethod
+    def construct_search_parameters(
+        geometry: Union[
+            geojson.FeatureCollection,
+            geojson.Feature,
+            dict,
+            list,
+            geopandas.GeoDataFrame,
+            geom.Polygon,
+        ],
+        collections: List[str],
+        start_date: str = "2020-01-01",
+        end_date: str = "2020-01-30",
+        usage_type: Optional[List[str]] = None,
+        limit: int = 10,
+        max_cloudcover: Optional[int] = None,
+        sortby: Optional[str] = None,
+        ascending: Optional[bool] = None,
+    ) -> dict:
+        """
+        Helps constructing the parameters dictionary required for the search.
 
         Args:
-            geometry: One of Dict, FeatureCollection, Feature, List,
-                GeoDataFrame, shapely.geometry.Polygon, shapely.geometry.Point. All
-                assume EPSG 4326.
-            geometry_operation: Desired operation, One of "bbox", "intersects", "contains".
-            limit: Maximum number of expected results.
+            geometry: The search geometry, default a Polygon.
+                One of FeatureCollection, Feature, dict (geojson geometry),
+                list (bounds coordinates), GeoDataFrame,
+                shapely.Polygon, shapely.Point.
+                All assume EPSG 4326!
+            collections: The satellite sensor collections to search for,
+                e.g. ["phr"] or ["phr", "spot"].
+                Also see catalog.get_collections().
             start_date: Query period starting day, format "2020-01-01".
             end_date: Query period ending day, format "2020-01-01".
-            scene_ids: List of scene_ids, if given ignores all other parameters except geometry.
-            order_ids: Optional, can be used to incorporate existing bought imagery on UP42
-                into new workflows.
-
+            usage_type: Optional. Filter for imagery that can
+                be purchased & downloaded or also processed.
+                ["DATA"] (can only be downloaded),
+                ["ANALYTICS"] (can be downloaded
+                or used directly with a processing algorithm),
+                ["DATA", "ANALYTICS"] (can be any combination).
+                The filter is inclusive, using ["DATA"] can
+                also result in results with ["DATA", "ANALYTICS"].
+            limit: The maximum number of search results to return (1-max.500).
+            max_cloudcover: Optional. Maximum cloud coverage percent.
+                e.g. 100 will return all scenes,
+                8.4 will return all scenes with 8.4 or less cloud coverage.
+            sortby: (deprecated)
+            ascending: (deprecated)
         Returns:
-            Dictionary of constructed input parameters.
+            The constructed parameters dictionary.
         """
-        # TODO: Add ipy slide widget option? One for each block.
-        input_parameters = self._get_default_parameters()
-        data_block_name = list(input_parameters.keys())[0]
-
-        if order_ids is not None:
-            # Needs to be handled in this function(not run_job) as it is only
-            # relevant for the data block.
-            # TODO: Check for order-id correct schema, should be handled on backend?
-            input_parameters[data_block_name] = {"order_ids": order_ids}
-        else:
-            if limit is not None:
-                input_parameters[data_block_name]["limit"] = limit
-            if scene_ids is not None:
-                if not isinstance(scene_ids, list):
-                    scene_ids = [scene_ids]
-                input_parameters[data_block_name]["ids"] = scene_ids
-                input_parameters[data_block_name]["limit"] = len(scene_ids)
-                input_parameters[data_block_name].pop("time")
-                # TODO: In case of ids remove all non-relevant parameters. Cleaner.
-            elif start_date is not None and end_date is not None:
-                datetime = f"{start_date}T00:00:00Z/{end_date}T00:00:00Z"
-                input_parameters[data_block_name]["time"] = datetime
-            aoi_fc = any_vector_to_fc(vector=geometry,)
-            aoi_feature = fc_to_query_geometry(
-                fc=aoi_fc,
-                geometry_operation=geometry_operation,  # type: ignore
-                squash_multiple_features=handle_multiple_features,
-            )
 
-            input_parameters[data_block_name][geometry_operation] = aoi_feature
-        return input_parameters
+        if sortby is not None or ascending is not None:
+            logger.info("sortby is deprecated, currently only sorting output by creation date.")
+        start = utils.format_time(start_date)
+        end = utils.format_time(end_date, set_end_of_day=True)
+        time_period = f"{start}/{end}"
+
+        aoi_fc = utils.any_vector_to_fc(
+            vector=geometry,
+        )
+        aoi_geometry = utils.fc_to_query_geometry(fc=aoi_fc, geometry_operation="intersects")
+
+        query_filters: Dict[Any, Any] = {}
+        if max_cloudcover is not None:
+            query_filters["cloudCoverage"] = {"lte": max_cloudcover}  # type: ignore
+
+        if usage_type is not None:
+            if usage_type == ["DATA"]:
+                query_filters["up42:usageType"] = {"in": ["DATA"]}
+            elif usage_type == ["ANALYTICS"]:
+                query_filters["up42:usageType"] = {"in": ["ANALYTICS"]}
+            elif usage_type == ["DATA", "ANALYTICS"]:
+                query_filters["up42:usageType"] = {"in": ["DATA", "ANALYTICS"]}
+            else:
+                raise ValueError("Select correct `usage_type`")
 
-    def _helper_run_job(
-        self,
-        input_parameters: Union[Dict, str, Path] = None,
-        test_job=False,
-        track_status: bool = False,
-        name: str = None,
-    ) -> "Job":
+        search_parameters = {
+            "datetime": time_period,
+            "intersects": aoi_geometry,
+            "limit": limit,
+            "collections": collections,
+            "query": query_filters,
+        }
+
+        return search_parameters
+
+    def search(self, search_parameters: dict, as_dataframe: bool = True) -> Union[geopandas.GeoDataFrame, dict]:
         """
-        Helper function to create and run a new real or test job.
+        Searches the catalog for the the search parameters and
+        returns the metadata of the matching scenes.
 
         Args:
-            input_parameters: Either json string of workflow parameters or filepath to json.
-            test_job: If set, runs a test query (search for available imagery based on your data parameters).
-            track_status: Automatically attaches workflow.track_status which queries
-                the job status every 30 seconds.
-            name: The job name. Optional, by default the workflow name is assigned.
+            search_parameters: The catalog search parameters, see example.
+            as_dataframe: return type, geopandas.GeoDataFrame if True (default),
+                FeatureCollection if False.
 
         Returns:
-            The spawned real or test job object.
+            The search results as a geopandas.GeoDataFrame,
+            optionally as JSON dict.
+
+        Example:
+            ```python
+                search_parameters={
+                    "datetime": "2019-01-01T00:00:00Z/2019-01-15T23:59:59Z",
+                    "collections": ["phr"],
+                    "intersects": {
+                        "type": "Polygon",
+                        "coordinates": [[[13.32113746,52.73971768],
+                        [13.15981158,52.2092959],[13.62204483,52.15632025],
+                        [13.78859517,52.68655119],[13.32113746,
+                        52.73971768]]]},
+                    "limit": 10,
+                    "sortby": [{"field" : "properties.acquisitionDate",
+                        "direction" : "asc"}]
+                    }
+            ```
         """
-        if input_parameters is None:
+        logger.info("Searching catalog with search_parameters: %s", search_parameters)
+
+        # The API request would fail with a limit above 500,
+        # thus 500 is forced in the initial
+        # request but additional results are handled below via pagination.
+        try:
+            max_limit = search_parameters["limit"]
+        except KeyError:
+            logger.info("No `limit` parameter in search_parameters, using default 500.")
+            max_limit = 500
+
+        if max_limit > 500:
+            search_parameters["limit"] = 500
+
+        # UP42 API can query multiple collections of the same host at once.
+        if self.data_products is None:
+            self.data_products = self.get_data_products(basic=True)  # type: ignore
+        hosts = [
+            v["host"]
+            for v in self.data_products.values()  # type: ignore
+            if v["collection"] in search_parameters["collections"]
+        ]
+        if not hosts:
             raise ValueError(
-                "Select the job_parameters, use workflow.construct_parameters()!"
+                f"""Selected collections {search_parameters["collections"]} are """
+                "not valid. See catalog.get_collections."
             )
+        if len(set(hosts)) > 1:
+            raise ValueError(
+                "Only collections with the same host can be searched "
+                "at the same time. Please adjust the "
+                "collections in the search_parameters!"
+            )
+        product_host = hosts[0]
 
-        if isinstance(input_parameters, (str, Path)):
-            with open(input_parameters) as src:
-                input_parameters = json.load(src)
-            logger.info("Loading job parameters from json file.")
-
-        if test_job:
-            input_parameters = input_parameters.copy()  # type: ignore
-            input_parameters.update({"config": {"mode": "DRY_RUN"}})  # type: ignore
-            logger.info("+++++++++++++++++++++++++++++++++")
-            logger.info("Running this job as Test Query...")
-            logger.info("+++++++++++++++++++++++++++++++++")
-
-        logger.info("Selected input_parameters: %s.", input_parameters)
-
-        if name is None:
-            name = self.info["name"]
-        name = f"{name}_py"  # Temporary recognition of python API usage.
-        url = (
-            f"{self.auth._endpoint()}/projects/{self.project_id}/"
-            f"workflows/{self.workflow_id}/jobs?name={name}"
-        )
-        response_json = self.auth._request(
-            request_type="POST", url=url, data=input_parameters
-        )
-        job_json = response_json["data"]
-        logger.info("Created and running new job: %s.", job_json["id"])
-        job = Job(self.auth, job_id=job_json["id"], project_id=self.project_id,)
+        url = host.endpoint(f"/catalog/hosts/{product_host}/stac/search")
+        response_json: dict = self.auth.request("POST", url, search_parameters)
+        features = response_json["features"]
+
+        # Search results with more than 500 items
+        # are given as 50-per-page additional pages.
+        while len(features) < max_limit:
+            pagination_exhausted = len(response_json["links"]) == 1
+            if pagination_exhausted:
+                break
+            next_page_url = response_json["links"][1]["href"]
+            response_json = self.auth.request("POST", next_page_url, search_parameters)
+            features += response_json["features"]
+
+        features = features[:max_limit]
+        if not features:
+            df = geopandas.GeoDataFrame(columns=["geometry"], geometry="geometry")
+        else:
+            df = geopandas.GeoDataFrame.from_features(geojson.FeatureCollection(features=features), crs="EPSG:4326")
 
-        if track_status:
-            job.track_status()
-        return job
+        logger.info("%s results returned.", df.shape[0])
+        if as_dataframe:
+            return df
+        else:
+            return df.__geo_interface__
 
-    def test_job(
+    def construct_order_parameters(
         self,
-        input_parameters: Union[Dict, str, Path] = None,
-        track_status: bool = False,
-        name: str = None,
-    ) -> "Job":
+        data_product_id: str,
+        image_id: str,
+        aoi: Union[
+            dict,
+            geojson.Feature,
+            geojson.FeatureCollection,
+            list,
+            geopandas.GeoDataFrame,
+            geom.Polygon,
+        ] = None,
+        tags: Optional[List[str]] = None,
+    ):
         """
-        Create a run a new test job (Test Query). With this test query you will not be
-        charged with any data or processing credits, but have a preview of the job result.
+        Helps constructing the parameters dictionary required
+        for the catalog order. Some collections have
+        additional parameters that are added to the output
+        dictionary with value None. The potential values to
+        select from are given in the logs, for more detail on
+        the parameter use `catalog.get_data_product_schema()`.
 
         Args:
-            input_parameters: Either json string of workflow parameters or filepath to json.
-            track_status: Automatically attaches workflow.track_status which queries
-                the job status every 30 seconds.
-            name: The job name. Optional, by default the workflow name is assigned.
-
+            data_product_id: Id of the desired UP42 data product,
+                see `catalog.get_data_products`
+            image_id: The id of the desired image
+                (from search results)
+            aoi: The geometry of the order, one of dict, Feature,
+                FeatureCollection, list, geopandas.GeoDataFrame, Polygon.
+                Optional for "full-image products".
+            tags: A list of tags that categorize the order.
         Returns:
-            The spawned test job object.
-        """
-        return self._helper_run_job(
-            input_parameters=input_parameters,
-            test_job=True,
-            track_status=track_status,
-            name=name,
-        )
+            The order parameters dictionary.
 
-    def run_job(
-        self,
-        input_parameters: Union[Dict, str, Path] = None,
-        track_status: bool = False,
-        name: str = None,
-    ) -> "Job":
+        Example:
+            ```python
+            order_parameters = catalog.construct_order_parameters(
+                data_product_id='647780db-5a06-4b61-b525-577a8b68bb54',
+                image_id='6434e7af-2d41-4ded-a789-fb1b2447ac92',
+                aoi={'type': 'Polygon',
+                'coordinates': (((13.375966, 52.515068),
+                  (13.375966, 52.516639),
+                  (13.378314, 52.516639),
+                  (13.378314, 52.515068),
+                  (13.375966, 52.515068)),)})
+            ```
         """
-        Creates and runs a new job.
-
-        Args:
-            input_parameters: Either json string of workflow parameters or filepath to json.
-            track_status: Automatically attaches workflow.track_status which queries
-                the job status every 30 seconds.
-            name: The job name. Optional, by default the workflow name is assigned.
+        order_parameters = {
+            "dataProduct": data_product_id,
+            "params": {"id": image_id},
+        }
+        if tags is not None:
+            order_parameters["tags"] = tags
+        schema = self.get_data_product_schema(data_product_id)
+        order_parameters = utils.autocomplete_order_parameters(order_parameters, schema)
+
+        # Some catalog orders, e.g. Capella don't require AOI (full image order)
+        # Handled on API level, don't manipulate in SDK,
+        # providers might accept geometries in the future.
+        if aoi is not None:
+            aoi = utils.any_vector_to_fc(vector=aoi)
+            aoi = utils.fc_to_query_geometry(fc=aoi, geometry_operation="intersects")
+            order_parameters["params"]["aoi"] = aoi  # type: ignore
 
-        Returns:
-            The spawned job object.
-        """
-        return self._helper_run_job(
-            input_parameters=input_parameters, track_status=track_status, name=name
-        )
+        return order_parameters
 
-    def get_jobs(self, return_json: bool = False) -> Union[List["Job"], Dict]:
+    def download_quicklooks(
+        self,
+        image_ids: List[str],
+        collection: str,
+        output_directory: Union[str, pathlib.Path, None] = None,
+    ) -> List[str]:
         """
-        Get all jobs associated with the workflow as job objects or json.
+        Gets the quicklooks of scenes from a single sensor. After download, can
+        be plotted via catalog.map_quicklooks() or catalog.plot_quicklooks().
 
         Args:
-            return_json: If true, returns the job info jsons instead of job objects.
+            image_ids: List of provider image_ids
+                e.g. ["6dffb8be-c2ab-46e3-9c1c-6958a54e4527"].
+                Access the search results id column via
+                `list(search_results.id)`.
+            collection: The data collection corresponding to the image ids.
+            output_directory: The file output directory,
+                defaults to the current working directory.
 
         Returns:
-            All job objects as a list, or alternatively the jobs info as json.
+            List of quicklook image output file paths.
         """
-        url = f"{self.auth._endpoint()}/projects/{self.project_id}/jobs"
-        response_json = self.auth._request(request_type="GET", url=url)
-        jobs_json = response_json["data"]
-
-        jobs_workflow_json = [
-            j for j in jobs_json if j["workflowId"] == self.workflow_id
-        ]
+        if self.data_products is None:
+            self.data_products = self.get_data_products(basic=True)  # type: ignore
+        hosts = [v["host"] for v in self.data_products.values() if v["collection"] == collection]  # type: ignore
+        if not host:
+            raise ValueError(f"Selected collections {collection} is not valid. See catalog.get_collections.")
+        product_host = hosts[0]
+        logger.info("Downloading quicklooks from provider %s.", product_host)
 
-        logger.info(
-            "Got %s jobs for workflow %s in project %s.",
-            len(jobs_workflow_json),
-            self.workflow_id,
-            self.project_id,
-        )
-        if return_json:
-            return jobs_workflow_json
+        if output_directory is None:
+            output_directory = pathlib.Path.cwd() / "catalog"
         else:
-            jobs = [
-                Job(self.auth, job_id=job["id"], project_id=self.project_id)
-                for job in tqdm(jobs_workflow_json)
-            ]
-            return jobs
+            output_directory = pathlib.Path(output_directory)
+        output_directory.mkdir(parents=True, exist_ok=True)
+        logger.info("Download directory: %s", output_directory)
 
-    def update_name(self, name: str = None, description: str = None) -> None:
-        """
-        Updates the workflow name and description.
+        if isinstance(image_ids, str):
+            image_ids = [image_ids]
 
-        Args:
-            name: New name of the workflow.
-            description: New description of the workflow.
-        """
-        properties_to_update = {"name": name, "description": description}
-        url = (
-            f"{self.auth._endpoint()}/projects/{self.project_id}/workflows/"
-            f"{self.workflow_id}"
-        )
-        self.auth._request(request_type="PUT", url=url, data=properties_to_update)
-        logger.info("Updated workflow name: %r", properties_to_update)
-
-    def delete(self) -> None:
-        """
-        Deletes the workflow and sets the Python object to None.
-        """
-        url = (
-            f"{self.auth._endpoint()}/projects/{self.project_id}/workflows/"
-            f"{self.workflow_id}"
-        )
-        self.auth._request(request_type="DELETE", url=url, return_text=False)
-        logger.info("Successfully deleted workflow: %s", self.workflow_id)
-        del self
+        out_paths: List[str] = []
+        for image_id in tqdm.tqdm(image_ids):
+            try:
+                url = host.endpoint(f"/catalog/{product_host}/image/{image_id}/quicklook")
+                response = self.auth.request(request_type="GET", url=url, return_text=False)
+                out_path = output_directory / f"quicklook_{image_id}.jpg"
+                out_paths.append(str(out_path))
+                with open(out_path, "wb") as dst:
+                    for chunk in response:
+                        dst.write(chunk)
+            except IOError:
+                logger.warning(
+                    "Image with id %s does not have quicklook available. Skipping ...",
+                    image_id,
+                )
+        self.quicklooks = out_paths  # pylint: disable=attribute-defined-outside-init
+        return out_paths
```

