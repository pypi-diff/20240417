# Comparing `tmp/schematic_db-0.0.dev33.tar.gz` & `tmp/schematic_db-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schematic_db-0.0.dev33.tar", max compression
+gzip compressed data, was "schematic_db-0.1.0.tar", max compression
```

## Comparing `schematic_db-0.0.dev33.tar` & `schematic_db-0.1.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     1060 2023-11-01 17:20:47.185265 schematic_db-0.0.dev33/pyproject.toml
--rw-r--r--   0        0        0     1131 2023-11-01 17:20:47.185265 schematic_db-0.0.dev33/schematic_db/__init__.py
--rw-r--r--   0        0        0        0 2023-11-01 17:20:47.185265 schematic_db-0.0.dev33/schematic_db/api_utils/__init__.py
--rw-r--r--   0        0        0     9152 2023-11-01 17:20:47.185265 schematic_db-0.0.dev33/schematic_db/api_utils/api_utils.py
--rw-r--r--   0        0        0        0 2023-11-01 17:20:47.185265 schematic_db-0.0.dev33/schematic_db/db_schema/__init__.py
--rw-r--r--   0        0        0    14416 2023-11-01 17:20:47.185265 schematic_db-0.0.dev33/schematic_db/db_schema/db_schema.py
--rw-r--r--   0        0        0        0 2023-11-01 17:20:47.189265 schematic_db-0.0.dev33/schematic_db/manifest_store/__init__.py
--rw-r--r--   0        0        0     4060 2023-11-01 17:20:47.189265 schematic_db-0.0.dev33/schematic_db/manifest_store/api_manifest_store.py
--rw-r--r--   0        0        0     3907 2023-11-01 17:20:47.189265 schematic_db-0.0.dev33/schematic_db/manifest_store/manifest_metadata_list.py
--rw-r--r--   0        0        0     3340 2023-11-01 17:20:47.189265 schematic_db-0.0.dev33/schematic_db/manifest_store/manifest_store.py
--rw-r--r--   0        0        0     3078 2023-11-01 17:20:47.189265 schematic_db-0.0.dev33/schematic_db/manifest_store/synapse_manifest_store.py
--rw-r--r--   0        0        0        0 2023-11-01 17:20:47.189265 schematic_db-0.0.dev33/schematic_db/query_store/__init__.py
--rw-r--r--   0        0        0      914 2023-11-01 17:20:47.189265 schematic_db-0.0.dev33/schematic_db/query_store/query_store.py
--rw-r--r--   0        0        0     1042 2023-11-01 17:20:47.189265 schematic_db-0.0.dev33/schematic_db/query_store/synapse_query_store.py
--rw-r--r--   0        0        0        0 2023-11-01 17:20:47.189265 schematic_db-0.0.dev33/schematic_db/rdb/__init__.py
--rw-r--r--   0        0        0     4198 2023-11-01 17:20:47.189265 schematic_db-0.0.dev33/schematic_db/rdb/mysql.py
--rw-r--r--   0        0        0     3800 2023-11-01 17:20:47.189265 schematic_db-0.0.dev33/schematic_db/rdb/postgres.py
--rw-r--r--   0        0        0     3931 2023-11-01 17:20:47.189265 schematic_db-0.0.dev33/schematic_db/rdb/rdb.py
--rw-r--r--   0        0        0    14270 2023-11-01 17:20:47.189265 schematic_db-0.0.dev33/schematic_db/rdb/sql_alchemy_database.py
--rw-r--r--   0        0        0    20274 2023-11-01 17:20:47.189265 schematic_db-0.0.dev33/schematic_db/rdb/synapse_database.py
--rw-r--r--   0        0        0        0 2023-11-01 17:20:47.189265 schematic_db-0.0.dev33/schematic_db/rdb_builder/__init__.py
--rw-r--r--   0        0        0     2028 2023-11-01 17:20:47.189265 schematic_db-0.0.dev33/schematic_db/rdb_builder/rdb_builder.py
--rw-r--r--   0        0        0        0 2023-11-01 17:20:47.189265 schematic_db-0.0.dev33/schematic_db/rdb_queryer/__init__.py
--rw-r--r--   0        0        0     2234 2023-11-01 17:20:47.189265 schematic_db-0.0.dev33/schematic_db/rdb_queryer/rdb_queryer.py
--rw-r--r--   0        0        0        0 2023-11-01 17:20:47.189265 schematic_db-0.0.dev33/schematic_db/rdb_updater/__init__.py
--rw-r--r--   0        0        0     9133 2023-11-01 17:20:47.189265 schematic_db-0.0.dev33/schematic_db/rdb_updater/rdb_updater.py
--rw-r--r--   0        0        0        0 2023-11-01 17:20:47.189265 schematic_db-0.0.dev33/schematic_db/schema/__init__.py
--rw-r--r--   0        0        0     6490 2023-11-01 17:20:47.189265 schematic_db-0.0.dev33/schematic_db/schema/database_config.py
--rw-r--r--   0        0        0    13366 2023-11-01 17:20:47.189265 schematic_db-0.0.dev33/schematic_db/schema/schema.py
--rw-r--r--   0        0        0        0 2023-11-01 17:20:47.189265 schematic_db-0.0.dev33/schematic_db/schema_graph/__init__.py
--rw-r--r--   0        0        0     1674 2023-11-01 17:20:47.189265 schematic_db-0.0.dev33/schematic_db/schema_graph/schema_graph.py
--rw-r--r--   0        0        0        0 2023-11-01 17:20:47.189265 schematic_db-0.0.dev33/schematic_db/synapse/__init__.py
--rw-r--r--   0        0        0    13033 2023-11-01 17:20:47.189265 schematic_db-0.0.dev33/schematic_db/synapse/synapse.py
--rw-r--r--   0        0        0     1086 1970-01-01 00:00:00.000000 schematic_db-0.0.dev33/PKG-INFO
+-rw-r--r--   0        0        0     1399 2024-04-17 01:48:01.464447 schematic_db-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1131 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/api_utils/__init__.py
+-rw-r--r--   0        0        0     9702 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/api_utils/api_utils.py
+-rw-r--r--   0        0        0        0 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/db_schema/__init__.py
+-rw-r--r--   0        0        0    14390 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/db_schema/db_schema.py
+-rw-r--r--   0        0        0        0 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/manifest_store/__init__.py
+-rw-r--r--   0        0        0     4278 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/manifest_store/api_manifest_store.py
+-rw-r--r--   0        0        0     3908 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/manifest_store/manifest_metadata_list.py
+-rw-r--r--   0        0        0     3395 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/manifest_store/manifest_store.py
+-rw-r--r--   0        0        0     3118 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/manifest_store/synapse_manifest_store.py
+-rw-r--r--   0        0        0        0 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/query_store/__init__.py
+-rw-r--r--   0        0        0      915 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/query_store/query_store.py
+-rw-r--r--   0        0        0     1043 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/query_store/synapse_query_store.py
+-rw-r--r--   0        0        0        0 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/rdb/__init__.py
+-rw-r--r--   0        0        0     4326 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/rdb/mysql.py
+-rw-r--r--   0        0        0     3801 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/rdb/postgres.py
+-rw-r--r--   0        0        0     3855 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/rdb/rdb.py
+-rw-r--r--   0        0        0    14447 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/rdb/sql_alchemy_database.py
+-rw-r--r--   0        0        0    21765 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/rdb/synapse_database.py
+-rw-r--r--   0        0        0        0 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/rdb_builder/__init__.py
+-rw-r--r--   0        0        0     2010 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/rdb_builder/rdb_builder.py
+-rw-r--r--   0        0        0        0 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/rdb_queryer/__init__.py
+-rw-r--r--   0        0        0     2235 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/rdb_queryer/rdb_queryer.py
+-rw-r--r--   0        0        0        0 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/rdb_updater/__init__.py
+-rw-r--r--   0        0        0     9134 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/rdb_updater/rdb_updater.py
+-rw-r--r--   0        0        0        0 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/schema/__init__.py
+-rw-r--r--   0        0        0     6526 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/schema/database_config.py
+-rw-r--r--   0        0        0    13393 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/schema/schema.py
+-rw-r--r--   0        0        0        0 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/schema_graph/__init__.py
+-rw-r--r--   0        0        0     1974 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/schema_graph/schema_graph.py
+-rw-r--r--   0        0        0        0 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/synapse/__init__.py
+-rw-r--r--   0        0        0    13270 2024-04-17 01:48:01.464447 schematic_db-0.1.0/schematic_db/synapse/synapse.py
+-rw-r--r--   0        0        0      241 2024-04-17 01:48:01.468447 schematic_db-0.1.0/schematic_db/utils.py
+-rw-r--r--   0        0        0     1583 1970-01-01 00:00:00.000000 schematic_db-0.1.0/PKG-INFO
```

### Comparing `schematic_db-0.0.dev33/schematic_db/__init__.py` & `schematic_db-0.1.0/schematic_db/__init__.py`

 * *Files identical despite different names*

### Comparing `schematic_db-0.0.dev33/schematic_db/api_utils/api_utils.py` & `schematic_db-0.1.0/schematic_db/api_utils/api_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Functions that interact with the schematic API"""
+
 # pylint: disable=duplicate-code
 
 from typing import Any
 from os import getenv
 from datetime import datetime
 import pytz
 import requests
 import pandas
 from schematic_db.manifest_store.manifest_metadata_list import ManifestMetadataList
+from schematic_db.utils import DisplayLabelType
 
 
 class SchematicAPIError(Exception):
     """When schematic API response status code is anything other than 200"""
 
     def __init__(  # pylint:disable=too-many-arguments
         self,
@@ -86,118 +88,122 @@
         )
 
 
 def create_schematic_api_response(
     endpoint_path: str,
     params: dict[str, Any],
     timeout: float = 30,
+    access_token: str | None = None,
 ) -> requests.Response:
     """Performs a GET request on the schematic API
 
     Args:
         endpoint_path (str): The path for the endpoint in the schematic API
         params (dict): The parameters in dict form for the requested endpoint
         timeout (float): The amount of seconds the API call has to run
+        access_token (str): Access token for storage related endpoints
 
     Raises:
         SchematicAPIError: When response code is anything other than 200
         SchematicAPITimeoutError: When API call times out
 
     Returns:
         requests.Response: The response from the API
     """
     api_url = getenv("API_URL", "https://schematic.api.sagebionetworks.org/v1/")
     endpoint_url = f"{api_url}/{endpoint_path}"
     start_time = datetime.now(pytz.timezone("US/Pacific"))
+    headers = {"Authorization": f"Bearer {access_token}"}
     try:
-        response = requests.get(endpoint_url, params=params, timeout=timeout)
+        response = requests.get(
+            endpoint_url, params=params, headers=headers, timeout=timeout
+        )
     except requests.exceptions.Timeout as exc:
-        raise SchematicAPITimeoutError(
-            endpoint_url, start_time, filter_params(params)
-        ) from exc
+        raise SchematicAPITimeoutError(endpoint_url, start_time, params) from exc
     if response.status_code != 200:
         raise SchematicAPIError(
             endpoint_url,
             response.status_code,
             response.reason,
             start_time,
-            filter_params(params),
+            params,
         )
     return response
 
 
-def filter_params(params: dict[str, Any]) -> dict[str, Any]:
-    """Removes any parameters from the input dictionary that should not be seen.
-
-    Args:
-        params (dict[str, Any]): A dictionary of parameters
-
-    Returns:
-        dict[str, Any]: A dictionary of parameters with any secrets removed
-    """
-    secret_params = ["access_token"]
-    for param in secret_params:
-        params.pop(param, None)
-    return params
-
-
-def find_class_specific_properties(schema_url: str, schema_class: str) -> list[str]:
+def find_class_specific_properties(
+    schema_url: str,
+    schema_class: str,
+    data_model_labels: DisplayLabelType = "class_label",
+) -> list[str]:
     """Find properties specifically associated with a given class
 
     Args:
         schema_url (str): Data Model URL
         schema_class (str): The class/name fo the component
+        data_model_labels (DisplayLabelType): The type of label to use as display
 
     Returns:
         list[str]: A list of properties of a given class/component.
     """
-    params = {"schema_url": schema_url, "schema_class": schema_class}
+    params = {
+        "schema_url": schema_url,
+        "schema_class": schema_class,
+        "data_model_labels": data_model_labels,
+    }
     response = create_schematic_api_response(
-        "explorer/find_class_specific_properties", params
+        "/schemas/find_class_specific_properties", params
     )
     return response.json()
 
 
 def get_property_label_from_display_name(
-    schema_url: str, display_name: str, strict_camel_case: bool = True
+    display_name: str, strict_camel_case: bool = True
 ) -> str:
     """Converts a given display name string into a proper property label string
 
     Args:
-        schema_url (str): Data Model URL
         display_name (str): The display name to be converted
         strict_camel_case (bool, optional): If true the more strict way of converting
             to camel case is used. Defaults to True.
 
     Returns:
         str: the property label name
     """
     params = {
-        "schema_url": schema_url,
         "display_name": display_name,
         "strict_camel_case": strict_camel_case,
     }
     response = create_schematic_api_response(
-        "explorer/get_property_label_from_display_name", params
+        "/utils/get_property_label_from_display_name", params
     )
     return response.json()
 
 
-def get_graph_by_edge_type(schema_url: str, relationship: str) -> list[tuple[str, str]]:
+def get_graph_by_edge_type(
+    schema_url: str,
+    relationship: str,
+    data_model_labels: DisplayLabelType = "class_label",
+) -> list[tuple[str, str]]:
     """Get a subgraph containing all edges of a given type (aka relationship)
 
     Args:
         schema_url (str): Data Model URL
         relationship (str): Relationship (i.e. parentOf, requiresDependency,
             rangeValue, domainValue)
+        data_model_labels (DisplayLabelType): The type of label to use as display
 
     Returns:
         list[tuple[str, str]]: A subgraph in the form of a list of tuples.
     """
-    params = {"schema_url": schema_url, "relationship": relationship}
+    params = {
+        "schema_url": schema_url,
+        "relationship": relationship,
+        "data_model_labels": data_model_labels,
+    }
     response = create_schematic_api_response("schemas/get/graph_by_edge_type", params)
     return response.json()
 
 
 def get_project_manifests(
     access_token: str, project_id: str, asset_view: str
 ) -> ManifestMetadataList:
@@ -210,20 +216,19 @@
             for Synapse this would be the Synapse ID of the fileview listing all
             data assets for a given project.(i.e. master_fileview in config.yml)
 
     Returns:
         ManifestMetadataList: A list of manifests in Synapse
     """
     params = {
-        "access_token": access_token,
         "project_id": project_id,
         "asset_view": asset_view,
     }
     response = create_schematic_api_response(
-        "storage/project/manifests", params, timeout=1000
+        "storage/project/manifests", params, timeout=1000, access_token=access_token
     )
     metadata_list = []
     for item in response.json():
         metadata_list.append(
             {
                 "dataset_id": item[0][0],
                 "dataset_name": item[0][1],
@@ -242,50 +247,66 @@
         access_token (str): Access token
         manifest_id (str): The synapse id of the manifest
 
     Returns:
         pd.DataFrame: The manifest in dataframe form
     """
     params = {
-        "access_token": access_token,
         "manifest_id": manifest_id,
         "as_json": True,
     }
-    response = create_schematic_api_response("manifest/download", params, timeout=1000)
+    response = create_schematic_api_response(
+        "manifest/download", params, timeout=1000, access_token=access_token
+    )
     manifest = pandas.DataFrame(response.json())
     return manifest
 
 
-def is_node_required(schema_url: str, node_label: str) -> bool:
+def is_node_required(
+    schema_url: str,
+    node_display_name: str,
+    data_model_labels: DisplayLabelType = "class_label",
+) -> bool:
     """Checks if node is required
 
     Args:
         schema_url (str): Data Model URL
-        node_label (str): Label/display name for the node to check
+        node_display_name (str): Label/display name for the node to check
+        data_model_labels (DisplayLabelType): The type of label to use as display
 
     Returns:
         bool: Wether or not the node is required
     """
 
-    params = {"schema_url": schema_url, "node_display_name": node_label}
+    params = {
+        "schema_url": schema_url,
+        "node_display_name": node_display_name,
+        "data_model_labels": data_model_labels,
+    }
     response = create_schematic_api_response("schemas/is_node_required", params)
     return response.json()
 
 
-def get_node_validation_rules(schema_url: str, node_display_name: str) -> list[str]:
+def get_node_validation_rules(
+    schema_url: str,
+    node_display_name: str,
+    data_model_labels: DisplayLabelType = "class_label",
+) -> list[str]:
     """Gets the validation rules for the node
 
     Args:
         schema_url (str): Data Model URL
         node_display_name (str): Label/display name for the node to check
+        data_model_labels (DisplayLabelType): The type of label to use as display
 
     Returns:
         list[str]: A list of validation rules
     """
     params = {
         "schema_url": schema_url,
         "node_display_name": node_display_name,
+        "data_model_labels": data_model_labels,
     }
     response = create_schematic_api_response(
         "schemas/get_node_validation_rules", params
     )
     return response.json()
```

### Comparing `schematic_db-0.0.dev33/schematic_db/db_schema/db_schema.py` & `schematic_db-0.1.0/schematic_db/db_schema/db_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """DB schema
 These are a set of classes for defining a database table in a dialect agnostic way.
 """
+
 from enum import Enum
-from typing import Any, Optional, TypeVar
+from typing import Any, TypeVar
 from pydantic.dataclasses import dataclass
 from pydantic import validator
 
 
 class ColumnDatatype(Enum):
     """A generic datatype that should be supported by all database types."""
 
@@ -108,17 +109,15 @@
         """String representation"""
         return f"{self.message}: {self.table_name}"
 
 
 class TableKeyError(Exception):
     """TableKeyError"""
 
-    def __init__(
-        self, message: str, table_name: str, key: Optional[str] = None
-    ) -> None:
+    def __init__(self, message: str, table_name: str, key: str | None = None) -> None:
         """
         Args:
             message (str): A message describing the error
             table_name (str): The name of the table involved in the error
             key (Optional[str], optional): The name of the key involved in the error.
              Defaults to None.
         """
```

### Comparing `schematic_db-0.0.dev33/schematic_db/manifest_store/api_manifest_store.py` & `schematic_db-0.1.0/schematic_db/manifest_store/api_manifest_store.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """The APIManifestStore class interacts with the Schematic API download manifests."""
+
 # pylint: disable=duplicate-code
 
-from typing import Optional
 import pandas
 from schematic_db.api_utils.api_utils import (
     get_project_manifests,
     download_manifest,
     ManifestMetadataList,
 )
 from schematic_db.schema_graph.schema_graph import SchemaGraph
+from schematic_db.utils import DisplayLabelType
 from .manifest_store import ManifestStore, ManifestStoreConfig
 
 
 class ManifestMissingPrimaryKeyError(Exception):
     """Raised when a manifest is missing its primary key"""
 
     def __init__(
@@ -46,27 +47,32 @@
 
 
 class APIManifestStore(ManifestStore):
     """
     The APIManifestStore class interacts with the Schematic API download manifests.
     """
 
-    def __init__(self, config: ManifestStoreConfig) -> None:
+    def __init__(
+        self,
+        config: ManifestStoreConfig,
+        display_label_type: DisplayLabelType = "class_label",
+    ) -> None:
         """
         The Schema class handles interactions with the schematic API.
         The main responsibilities are creating the database schema, and retrieving manifests.
 
         Args:
             config (SchemaConfig): A config describing the basic inputs for the schema object
+            display_model_type (DisplayLabelType): The type of label used for display purposes
         """
         self.synapse_project_id = config.synapse_project_id
         self.synapse_asset_view_id = config.synapse_asset_view_id
         self.synapse_auth_token = config.synapse_auth_token
-        self.schema_graph = SchemaGraph(config.schema_url)
-        self.manifest_metadata: Optional[ManifestMetadataList] = None
+        self.schema_graph = SchemaGraph(config.schema_url, display_label_type)
+        self.manifest_metadata: ManifestMetadataList | None = None
 
     def create_sorted_table_name_list(self) -> list[str]:
         """
         Uses the schema graph to create a table name list such tables always come after ones they
          depend on.
         This order is how tables in a database should be built and/or updated.
```

### Comparing `schematic_db-0.0.dev33/schematic_db/manifest_store/manifest_metadata_list.py` & `schematic_db-0.1.0/schematic_db/manifest_store/manifest_metadata_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Metadata for a manifest in Synapse."""
+
 # pylint: disable=duplicate-code
 from typing import Any
 import json
 import re
 from pydantic.dataclasses import dataclass
 from pydantic import validator
```

### Comparing `schematic_db-0.0.dev33/schematic_db/manifest_store/manifest_store.py` & `schematic_db-0.1.0/schematic_db/manifest_store/manifest_store.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 ManifestStore is an abstract base class that implements an interface.
 The interface is used to interact with manifests
 """
+
 # pylint: disable=duplicate-code
 from abc import ABC, abstractmethod
 import re
 import pandas
 from pydantic.dataclasses import dataclass
 from pydantic import validator
 import validators
@@ -36,19 +37,19 @@
         valid_url = validators.url(value)
         if not valid_url:
             raise ValueError(f"{value} is a valid url")
         return value
 
     @validator("schema_url")
     @classmethod
-    def validate_is_jsonld(cls, value: str) -> str:
-        """Validates that the value is a jsonld file"""
-        is_jsonld = value.endswith(".jsonld")
-        if not is_jsonld:
-            raise ValueError(f"{value} does end with '.jsonld'")
+    def validate_is_valid_type(cls, value: str) -> str:
+        """Validates that the value is a jsonld or csv file"""
+        is_valid_type = value.endswith(".jsonld") | value.endswith(".csv")
+        if not is_valid_type:
+            raise ValueError(f"{value} does end with '.jsonld', or '.csv")
         return value
 
     @validator("synapse_project_id", "synapse_asset_view_id")
     @classmethod
     def validate_synapse_id(cls, value: str) -> str:
         """Check if string is a valid synapse id"""
         if not re.search("^syn[0-9]+", value):
```

### Comparing `schematic_db-0.0.dev33/schematic_db/manifest_store/synapse_manifest_store.py` & `schematic_db-0.1.0/schematic_db/manifest_store/synapse_manifest_store.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 """
 SynapseManifestStore implements the ManifestStore interface.
 It interacts with Synapse through the Python client.
 This is used to interact with manifests
 """
-from typing import Optional
+
 import pandas
-from deprecation import deprecated
 from schematic_db.schema_graph.schema_graph import SchemaGraph
 from schematic_db.api_utils.api_utils import ManifestMetadataList
 from schematic_db.synapse.synapse import Synapse
+from schematic_db.utils import DisplayLabelType
 from .manifest_store import ManifestStore, ManifestStoreConfig
 
 
-@deprecated(
-    deprecated_in="0.0.29",
-    details="This is both an experimental and temporary class that will be removed in the future.",
-)
 class SynapseManifestStore(ManifestStore):
     """An interface for interacting with manifests"""
 
-    def __init__(self, config: ManifestStoreConfig) -> None:
+    def __init__(
+        self,
+        config: ManifestStoreConfig,
+        display_label_type: DisplayLabelType = "class_label",
+    ) -> None:
         """
         Args:
             config (ManifestStoreConfig): A config with setup values
+            display_model_type (DisplayLabelType): The type of label used for display purposes
         """
         self.synapse_asset_view_id = config.synapse_asset_view_id
         self.synapse = Synapse(config.synapse_auth_token, config.synapse_project_id)
-        self.schema_graph = SchemaGraph(config.schema_url)
-        self.manifest_metadata: Optional[ManifestMetadataList] = None
+        self.schema_graph = SchemaGraph(config.schema_url, display_label_type)
+        self.manifest_metadata: ManifestMetadataList | None = None
 
     def create_sorted_table_name_list(self) -> list[str]:
         """
         Creates a table name list such tables always come after ones they
          depend on.
         This order is how tables in a database should be built and/or updated.
```

### Comparing `schematic_db-0.0.dev33/schematic_db/query_store/query_store.py` & `schematic_db-0.1.0/schematic_db/query_store/query_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """QueryStore"""
+
 from abc import ABC, abstractmethod
 import pandas as pd
 
 
 class QueryStore(ABC):  # pylint: disable=too-few-public-methods
     """An interface for Query Store objects"""
```

### Comparing `schematic_db-0.0.dev33/schematic_db/query_store/synapse_query_store.py` & `schematic_db-0.1.0/schematic_db/query_store/synapse_query_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Synapse Query Store
 """
+
 import pandas as pd
 from schematic_db.synapse.synapse import Synapse
 from .query_store import QueryStore
 
 
 class SynapseQueryStore(QueryStore):  # pylint: disable=too-few-public-methods
     """SynapseQueryStore
```

### Comparing `schematic_db-0.0.dev33/schematic_db/rdb/mysql.py` & `schematic_db-0.1.0/schematic_db/rdb/mysql.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """MySQLDatabase"""
+
 from typing import Any
 import pandas
 import numpy
 import sqlalchemy
 import sqlalchemy.dialects.mysql
 from sqlalchemy import exc
 from schematic_db.db_schema.db_schema import (
@@ -80,32 +81,32 @@
         statement = sqlalchemy.dialects.mysql.insert(table).values(row)
         statement = statement.on_duplicate_key_update(**row)
         with self.engine.begin() as conn:
             conn.execute(statement)
 
     def _get_datatype(
         self, column_schema: ColumnSchema, primary_key: str, foreign_keys: list[str]
-    ) -> Any:
+    ) -> sqlalchemy.types.TypeEngine:
         """
         Gets the datatype of the column based on its schema
 
         Args:
             column_schema (ColumnSchema): The schema of the column
             primary_key (str): The primary key fo the column (unused)
             foreign_keys (list[str]): A list of foreign keys for the the column
 
         Returns:
-            Any: The SQLAlchemy datatype
+            sqlalchemy.types.TypeEngine: The SQLAlchemy datatype of the input column
         """
-        datatypes = {
+        datatypes: dict[ColumnDatatype, sqlalchemy.types.TypeEngine] = {
             ColumnDatatype.TEXT: sqlalchemy.VARCHAR(5000),
-            ColumnDatatype.DATE: sqlalchemy.Date,
-            ColumnDatatype.INT: sqlalchemy.Integer,
-            ColumnDatatype.FLOAT: sqlalchemy.Float,
-            ColumnDatatype.BOOLEAN: sqlalchemy.Boolean,
+            ColumnDatatype.DATE: sqlalchemy.Date(),
+            ColumnDatatype.INT: sqlalchemy.Integer(),
+            ColumnDatatype.FLOAT: sqlalchemy.Float(),
+            ColumnDatatype.BOOLEAN: sqlalchemy.Boolean(),
         }
         # Keys need to be max 100 chars
         if column_schema.datatype == ColumnDatatype.TEXT and (
             column_schema.name == primary_key or column_schema.name in foreign_keys
         ):
             return sqlalchemy.VARCHAR(100)
         # Strings that need to be indexed need to be max 1000 chars
```

### Comparing `schematic_db-0.0.dev33/schematic_db/rdb/postgres.py` & `schematic_db-0.1.0/schematic_db/rdb/postgres.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Represents a Postgres database."""
+
 from typing import Any
 import numpy
 import pandas
 import sqlalchemy
 import sqlalchemy.dialects.postgresql
 from sqlalchemy.inspection import inspect
 from sqlalchemy import exc
```

### Comparing `schematic_db-0.0.dev33/schematic_db/rdb/rdb.py` & `schematic_db-0.1.0/schematic_db/rdb/rdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """RelationalDatabase"""
+
 from abc import ABC, abstractmethod
 import pandas as pd
 from schematic_db.db_schema.db_schema import TableSchema
 
 
 class UpsertDatabaseError(Exception):
     """Raised when a database class catches an error doing an upsert"""
@@ -13,15 +14,15 @@
             table_name (str): The name of the table being upserted into
         """
         self.message = "Error upserting table"
         self.table_name = table_name
         super().__init__(self.message)
 
     def __str__(self) -> str:
-        return f"{self.message}; " f"Table Name: {self.table_name}"
+        return f"{self.message}; Table Name: {self.table_name}"
 
 
 class InsertDatabaseError(Exception):
     """Raised when a database class catches an error doing an insert"""
 
     def __init__(self, table_name: str) -> None:
         """
@@ -29,15 +30,15 @@
             table_name (str): The name of the table being inserted into
         """
         self.message = "Error inserting table"
         self.table_name = table_name
         super().__init__(self.message)
 
     def __str__(self) -> str:
-        return f"{self.message}; " f"Table Name: {self.table_name}"
+        return f"{self.message}; Table Name: {self.table_name}"
 
 
 class RelationalDatabase(ABC):
     """An interface for relational database types"""
 
     @abstractmethod
     def get_table_names(self) -> list[str]:
@@ -79,19 +80,18 @@
             table_name (str): The name of the table
 
         Returns:
             pd.DataFrame: The table
         """
 
     @abstractmethod
-    def add_table(self, table_name: str, table_schema: TableSchema) -> None:
+    def add_table(self, table_schema: TableSchema) -> None:
         """Adds a table to the schema
 
         Args:
-            table_name (str): The name of the table
             table_schema (TableSchema): The schema for the table being added
         """
 
     @abstractmethod
     def drop_table(self, table_name: str) -> None:
         """Drops a table from the schema
         Args:
```

### Comparing `schematic_db-0.0.dev33/schematic_db/rdb/sql_alchemy_database.py` & `schematic_db-0.1.0/schematic_db/rdb/sql_alchemy_database.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """SQLAlchemy"""
-from typing import Any
+
 from dataclasses import dataclass
 import pandas
 import numpy
 import sqlalchemy
 import sqlalchemy_utils
 from sqlalchemy import exc
 from sqlalchemy.inspection import inspect
+from sqlalchemy.sql.schema import Table as SQLAlchemyTable
 from schematic_db.db_schema.db_schema import (
     TableSchema,
     ColumnDatatype,
     ColumnSchema,
     ForeignKeySchema,
 )
 from .rdb import RelationalDatabase, InsertDatabaseError
@@ -26,23 +27,23 @@
 
     def __str__(self) -> str:
         return f"{self.message}:{self.key}"
 
 
 def create_foreign_key_column(
     name: str,
-    datatype: Any,
+    datatype: sqlalchemy.types.TypeEngine,
     foreign_table_name: str,
     foreign_table_column: str,
 ) -> sqlalchemy.Column:
     """Creates a sqlalchemy.column that is a foreign key
 
     Args:
         name (str): The name of the column
-        datatype (Any): The SQL datatype of the column
+        datatype (sqlalchemy.types.TypeEngine): The SQLAlchemy datatype of the column to be created
         foreign_table_name (str): The name of the table the foreign key is referencing
         foreign_table_column (str): The name of the column the foreign key is referencing
 
     Returns:
         sqlalchemy.Column: A sqlalchemy.column
     """
     col: sqlalchemy.Column = sqlalchemy.Column(
@@ -54,20 +55,20 @@
         ),
         nullable=True,
     )
     return col
 
 
 def create_foreign_key_configs(
-    table_schema: sqlalchemy.sql.schema.Table,
+    table_schema: SQLAlchemyTable,
 ) -> list[ForeignKeySchema]:
     """Creates a list of foreign key configs from a sqlalchemy table schema
 
     Args:
-        table_schema (sqlalchemy.sql.schema.Table): A sqlalchemy table schema
+        table_schema (SQLAlchemyTable): A sqlalchemy table schema
 
     Returns:
         list[ForeignKeySchema]: A list of foreign key configs
     """
     foreign_keys = inspect(table_schema).foreign_keys
     return [
         ForeignKeySchema(
@@ -76,25 +77,25 @@
             foreign_column_name=key.column.name,
         )
         for key in foreign_keys
     ]
 
 
 def create_column_schemas(
-    table_schema: sqlalchemy.sql.schema.Table,
+    table_schema: SQLAlchemyTable,
     indexed_columns: list[str],
-    column_datatypes: dict[Any, ColumnDatatype],
+    column_datatypes: dict[type, ColumnDatatype],
 ) -> list[ColumnSchema]:
     """Creates a list of column schemas from a sqlalchemy table schema
 
     Args:
-        table_schema (sqlalchemy.sql.schema.Table): A sqlalchemy table schema
+        table_schema (SQLAlchemyTable): A sqlalchemy table schema
         indexed_columns (list[str]): A list of columns in the schema to be indexed
-        column_datatypes(dict[Any, ColumnDatatype]): A dictionary whose keys
-          are a sql column datatype, and values are a ColumnDatatype
+        column_datatypes(dict[type, ColumnDatatype]): A dictionary whose keys
+          are a SQLAlchemy column data type, and values are a ColumnDatatype
 
     Returns:
         list[ColumnSchema]: A list of column schemas
     """
     columns = table_schema.c
     return [
         ColumnSchema(
@@ -125,15 +126,15 @@
     - Implements the RelationalDatabase interface.
     - Handles generic SQL specific functionality.
     - Not intended to be used, only inherited from
     """
 
     def __init__(
         self, config: SQLConfig, verbose: bool = False, db_type_string: str = "sql"
-    ):
+    ) -> None:
         """Init
 
         Args:
             config (MySQLConfig): A MySQL config
             verbose (bool): Sends much more to logging.info
             db_type_string (str): They type of database in string form
         """
@@ -206,16 +207,14 @@
             primary_key=primary_key,
             foreign_keys=create_foreign_key_configs(table_schema),
             columns=create_column_schemas(
                 table_schema, indexed_columns, self.column_datatypes
             ),
         )
 
-    # def _get_column_type_dict(self)
-
     def insert_table_rows(self, table_name: str, data: pandas.DataFrame) -> None:
         """Inserts the rows of the table into a target table in the database
 
         Args:
             table_name (str): The name of the table to be inserted into
             data (pandas.DataFrame): The rows to be inserted
 
@@ -262,25 +261,24 @@
 
         Returns:
             list[str]: A list of table names
         """
         inspector = sqlalchemy.inspect(self.engine)
         return sorted(inspector.get_table_names())
 
-    def add_table(self, table_name: str, table_schema: TableSchema) -> None:
+    def add_table(self, table_schema: TableSchema) -> None:
         """Adds a table to the schema
 
         Args:
-            table_name (str): The name of the table
             table_schema (TableSchema): The schema for the table to be added
         """
         metadata = self._get_current_metadata()
         columns = self._create_columns(table_schema)
         sqlalchemy.Table(
-            table_name,
+            table_schema.name,
             metadata,
             *columns,
             sqlalchemy.PrimaryKeyConstraint(table_schema.primary_key),
         )
         metadata.create_all(self.engine)
 
     def query_table(self, table_name: str) -> pandas.DataFrame:
@@ -291,36 +289,36 @@
 
         Returns:
             pandas.DataFrame: The table in pandas.Dataframe form
         """
         query = f"SELECT * FROM `{table_name}`"
         return self.execute_sql_query(query)
 
-    def _execute_sql_statement(self, statement: Any) -> Any:
+    def _execute_sql_statement(
+        self, statement: sqlalchemy.sql.expression.Executable
+    ) -> sqlalchemy.CursorResult:
         """Executes a sql statement
 
         Args:
-            statement (Any): A sql statement in sqlalchemy.text form
+            statement (sqlalchemy.sql.expression.Executable): The sql executable to run
 
         Returns:
-            Any: The result, if any, from the sql statement
+            sqlalchemy.CursorResult: The result from the sql statement
         """
         with self.engine.begin() as conn:
             return conn.execute(statement)
 
-    def _create_columns(
-        self, table_schema: TableSchema
-    ) -> list[sqlalchemy.Column[Any]]:
+    def _create_columns(self, table_schema: TableSchema) -> list[sqlalchemy.Column]:
         """Creates a list SQLAlchemy columns for a table
 
         Args:
             table_schema (TableSchema): The schema of the table to create columns for
 
         Returns:
-            list[sqlalchemy.Column[Any]]: A list SQLAlchemy columns
+            list[sqlalchemy.Column]: A list SQLAlchemy columns
         """
         columns = [
             self._create_column(att, table_schema) for att in table_schema.columns
         ]
         return columns
 
     def _create_column(
@@ -379,33 +377,33 @@
         return indexed_columns
 
     def _get_datatype(
         self,
         column_schema: ColumnSchema,
         primary_key: str,  # pylint: disable=unused-argument
         foreign_keys: list[str],  # pylint: disable=unused-argument
-    ) -> Any:
+    ) -> sqlalchemy.types.TypeEngine:
         """
         Gets the datatype of the column based on its schema
         Other _get_datatype methods depend on primary and foreign keys
 
         Args:
             column_schema (ColumnSchema): The schema of the column
             primary_key (str): The primary key fo the column (unused)
             foreign_keys (list[str]): A list of foreign keys for the the column (unused)
 
         Returns:
-            Any: The SQLAlchemy datatype
+            sqlalchemy.types.TypeEngine: The SQLAlchemy datatype of the column input
         """
-        datatypes = {
-            ColumnDatatype.TEXT: sqlalchemy.VARCHAR,
-            ColumnDatatype.DATE: sqlalchemy.Date,
-            ColumnDatatype.INT: sqlalchemy.Integer,
-            ColumnDatatype.FLOAT: sqlalchemy.Float,
-            ColumnDatatype.BOOLEAN: sqlalchemy.Boolean,
+        datatypes: dict[ColumnDatatype, sqlalchemy.types.TypeEngine] = {
+            ColumnDatatype.TEXT: sqlalchemy.VARCHAR(),
+            ColumnDatatype.DATE: sqlalchemy.Date(),
+            ColumnDatatype.INT: sqlalchemy.Integer(),
+            ColumnDatatype.FLOAT: sqlalchemy.Float(),
+            ColumnDatatype.BOOLEAN: sqlalchemy.Boolean(),
         }
         return datatypes[column_schema.datatype]
 
     def _get_table_object(self, table_name: str) -> sqlalchemy.Table:
         """Gets a sqlalchemy Table by its name
 
         Args:
```

### Comparing `schematic_db-0.0.dev33/schematic_db/rdb/synapse_database.py` & `schematic_db-0.1.0/schematic_db/rdb/synapse_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """SynapseDatabase"""
-from typing import Union
+
 from functools import partial
 import pandas as pd
 import synapseclient as sc  # type: ignore
 from schematic_db.db_schema.db_schema import (
     DatabaseSchema,
     TableSchema,
     ForeignKeySchema,
@@ -30,14 +30,33 @@
         self.table_name = table_name
         super().__init__(self.message)
 
     def __str__(self) -> str:
         return f"{self.message}; " f"name: {self.table_name};"
 
 
+class InputDataframeMissingColumn(Exception):
+    """Raised when an input dataframe is missing a needed column(s)"""
+
+    def __init__(
+        self, message: str, table_columns: list[str], missing_columns: list[str]
+    ) -> None:
+        self.message = message
+        self.table_columns = table_columns
+        self.missing_columns = missing_columns
+        super().__init__(self.message)
+
+    def __str__(self) -> str:
+        return (
+            f"{self.message}; "
+            f"table_columns: {self.table_columns}; "
+            f"missing_columns: {self.missing_columns}"
+        )
+
+
 class SynapseDatabaseDropTableError(Exception):
     """SynapseDatabaseDropTableError"""
 
     def __init__(
         self, message: str, table_name: str, reverse_dependencies: list[str]
     ) -> None:
         self.message = message
@@ -160,15 +179,15 @@
     func = datatypes[datatype]
     return func(name=name)
 
 
 class SynapseDatabase(RelationalDatabase):
     """Represents a database stored as Synapse tables"""
 
-    def __init__(self, auth_token: str, project_id: str):
+    def __init__(self, auth_token: str, project_id: str) -> None:
         """Init
 
         Args:
             auth_token (str): A Synapse auth_token
             project_id (str): A Synapse id for a project
         """
         self.synapse = Synapse(auth_token, project_id)
@@ -285,15 +304,15 @@
                 raise SynapseDatabaseUpdateTableError(
                     table_name=table_config.name,
                     foreign_key=key.name,
                     values=insert_keys,
                     dependency=key.foreign_table_name,
                 )
 
-    def add_table(self, table_name: str, table_schema: TableSchema) -> None:
+    def add_table(self, table_schema: TableSchema) -> None:
         table_names = self.synapse.get_table_names()
         table_name = table_schema.name
         columns = [
             create_synapse_column(att.name, att.datatype)
             for att in table_schema.columns
         ]
 
@@ -312,15 +331,15 @@
         """Annotates the table with it's primary key and foreign keys
 
         Args:
             table_name (str): The name of the table to be annotated
             table_schema (TableSchema): The config for the table
         """
         synapse_id = self.synapse.get_synapse_id_from_table_name(table_name)
-        annotations: dict[str, Union[str, list[str]]] = {
+        annotations: dict[str, str | list[str]] = {
             f"attribute{str(i)}": create_attribute_annotation_string(att)
             for i, att in enumerate(table_schema.columns)
         }
         annotations["primary_key"] = table_schema.primary_key
         if len(table_schema.foreign_keys) > 0:
             foreign_key_strings = [
                 create_foreign_key_annotation_string(key)
@@ -433,14 +452,15 @@
             # merge the reverse dependency data with the input data
             data = pd.merge(
                 rd_data,
                 data,
                 how="inner",
                 left_on=foreign_key.name,
                 right_on=foreign_key.foreign_column_name,
+                validate="many_to_one",
             )
 
             # if data has no rows continue to next reverse dependency
             if len(data.index) == 0:
                 continue
 
             data = data[[primary_key, "ROW_ID", "ROW_VERSION"]]
@@ -480,18 +500,32 @@
         self, table_id: str, data: pd.DataFrame, primary_key: str
     ) -> None:
         """Upserts rows into the given table
 
         Args:
             table_id (str): The Synapse id of the table to be upserted into.
             data (pd.DataFrame): The table the rows will come from
-            primary_key (str): The primary key of the table used to identify which rows to update
+            primary_key (str): The primary key of the table used to identify
+              which rows to update
+
+        Raises:
+            InputDataframeMissingColumn: Raised when the input dataframe has
+              no column that matches the primary key argument.
         """
+        if primary_key not in list(data.columns):
+            raise InputDataframeMissingColumn(
+                "Input dataframe missing primary key column.",
+                list(data.columns),
+                [primary_key],
+            )
+
         table = self._create_primary_key_table(table_id, primary_key)
-        merged_table = pd.merge(data, table, how="left", on=primary_key)
+        merged_table = pd.merge(
+            data, table, how="left", on=primary_key, validate="one_to_one"
+        )
         self.synapse.upsert_table_rows(table_id, merged_table)
 
     def _merge_dataframe_with_primary_key_table(
         self, table_id: str, data: pd.DataFrame, primary_key: str
     ) -> pd.DataFrame:
         """
         Merges the dataframe with a table that has just the primary key column.
@@ -505,26 +539,38 @@
 
         Returns:
             pd.DataFrame: A dataframe with only rows where the primary key currently exists
         """
         data = data[[primary_key]]
         table = self.synapse.query_table(table_id, include_row_data=True)
         table = table[["ROW_ID", "ROW_VERSION", primary_key]]
-        merged_table = pd.merge(data, table, how="inner", on=primary_key)
+        merged_table = pd.merge(
+            data, table, how="inner", on=primary_key, validate="one_to_one"
+        )
         return merged_table
 
     def _create_primary_key_table(
         self, table_id: str, primary_key: str
     ) -> pd.DataFrame:
         """Creates a dataframe with just the primary key of the table
 
         Args:
             table_id (str): The id of the table to query
             primary_key (str): The name of the primary key
 
         Returns:
             pd.DataFrame: The table in pandas.DataFrame form with the primary key, ROW_ID, and
              ROW_VERSION columns
+
+        Raises:
+            InputDataframeMissingColumn: Raised when the synapse table has no column that
+              matches the primary key argument.
         """
         table = self.synapse.query_table(table_id, include_row_data=True)
+        if primary_key not in list(table.columns):
+            raise InputDataframeMissingColumn(
+                "Synapse table missing primary key column",
+                list(table.columns),
+                [primary_key],
+            )
         table = table[["ROW_ID", "ROW_VERSION", primary_key]]
         return table
```

### Comparing `schematic_db-0.0.dev33/schematic_db/rdb_builder/rdb_builder.py` & `schematic_db-0.1.0/schematic_db/rdb_builder/rdb_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """RDBBuilder"""
+
 # pylint: disable=logging-fstring-interpolation
 import logging
 from schematic_db.rdb.rdb import RelationalDatabase
 from schematic_db.schema.schema import Schema, DatabaseSchema
 
 
 logging.getLogger(__name__)
@@ -49,9 +50,9 @@
 
         Args:
             database_schema (DatabaseSchema): A generic schema for the database
         """
         logging.info("Building database")
         for table_schema in database_schema.table_schemas:
             logging.info(f"Adding table to database schema: {table_schema.name}")
-            self.rdb.add_table(table_schema.name, table_schema)
+            self.rdb.add_table(table_schema)
         logging.info("Database built")
```

### Comparing `schematic_db-0.0.dev33/schematic_db/rdb_queryer/rdb_queryer.py` & `schematic_db-0.1.0/schematic_db/rdb_queryer/rdb_queryer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """RDB Queryer"""
+
 import pandas as pd
 from schematic_db.rdb.rdb import RelationalDatabase
 from schematic_db.query_store.synapse_query_store import QueryStore
 
 
 class DuplicateColumnError(Exception):
     """Occurs when a query results in a table with duplicate columns"""
```

### Comparing `schematic_db-0.0.dev33/schematic_db/rdb_updater/rdb_updater.py` & `schematic_db-0.1.0/schematic_db/rdb_updater/rdb_updater.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """RDBUpdater"""
+
 # pylint: disable=logging-fstring-interpolation
 import warnings
 import logging
 import pandas as pd
 from schematic_db.rdb.rdb import (
     RelationalDatabase,
     UpsertDatabaseError,
```

### Comparing `schematic_db-0.0.dev33/schematic_db/schema/database_config.py` & `schematic_db-0.1.0/schematic_db/schema/database_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 A config for database specific items
 """
-from typing import Optional, Any
+
+from typing import Any, Optional
 from deprecation import deprecated
 from schematic_db.db_schema.db_schema import (
     ForeignKeySchema,
     ColumnSchema,
     ColumnDatatype,
 )
 
@@ -16,25 +17,28 @@
     "int": ColumnDatatype.INT,
     "date": ColumnDatatype.DATE,
 }
 
 
 @deprecated(
     deprecated_in="0.0.27",
-    details="Functionality will be accomplished with future Schematic API calls.",
+    details=(
+        "Functionality will be accomplished with future Schematic API calls. "
+        "This will be sunsetted in ~0.1.1.",
+    ),
 )
 class DatabaseTableConfig:  # pylint: disable=too-few-public-methods
     """A config for database specific items for one table"""
 
     def __init__(
         self,
         name: str,
-        primary_key: Optional[str] = None,
-        foreign_keys: Optional[list[dict[str, str]]] = None,
-        columns: Optional[list[dict[str, Any]]] = None,
+        primary_key: str | None = None,
+        foreign_keys: list[dict[str, str]] | None = None,
+        columns: list[dict[str, Any]] | None = None,
     ) -> None:
         """
         Init
         """
         self.name = name
         self.primary_key = primary_key
         if foreign_keys is None:
@@ -68,15 +72,15 @@
             ValueError: Raised when there are duplicate column names
         """
         column_names = self._get_column_names()
         if column_names is not None:
             if len(column_names) != len(list(set(column_names))):
                 raise ValueError("There are duplicate column names")
 
-    def _get_column_names(self) -> Optional[list[str]]:
+    def _get_column_names(self) -> list[str] | None:
         """Gets the list of column names in the config
 
         Returns:
             list[str]: A list of column names
         """
         if self.columns is not None:
             return [column.name for column in self.columns]
@@ -89,15 +93,15 @@
             ValueError: Raised when there are duplicate foreign keys
         """
         foreign_keys_names = self._get_foreign_key_names()
         if foreign_keys_names is not None:
             if len(foreign_keys_names) != len(list(set(foreign_keys_names))):
                 raise ValueError("There are duplicate column names")
 
-    def _get_foreign_key_names(self) -> Optional[list[str]]:
+    def _get_foreign_key_names(self) -> list[str] | None:
         """Gets the list of foreign key names in the config
 
         Returns:
             list[str]: A list of foreign key names
         """
         if self.foreign_keys is not None:
             return [key.name for key in self.foreign_keys]
@@ -112,51 +116,51 @@
         Init
         """
         self.tables: list[DatabaseTableConfig] = [
             DatabaseTableConfig(**table) for table in tables
         ]
         self._check_table_names()
 
-    def get_primary_key(self, table_name: str) -> Optional[str]:
+    def get_primary_key(self, table_name: str) -> str | None:
         """Gets the primary key for an table
 
         Args:
             table_name (str): The name of the table
 
         Returns:
             Optional[str]: The primary key
         """
         table = self._get_table_by_name(table_name)
         return None if table is None else table.primary_key
 
-    def get_foreign_keys(self, table_name: str) -> Optional[list[ForeignKeySchema]]:
+    def get_foreign_keys(self, table_name: str) -> list[ForeignKeySchema] | None:
         """Gets the foreign keys for an table
 
         Args:
             table_name (str): The name of the table
 
         Returns:
             Optional[list[ForeignKeySchema]]: The foreign keys
         """
         table = self._get_table_by_name(table_name)
         return None if table is None else table.foreign_keys
 
-    def get_columns(self, table_name: str) -> Optional[list[ColumnSchema]]:
+    def get_columns(self, table_name: str) -> list[ColumnSchema] | None:
         """Gets the columns for an table
 
         Args:
             table_name (str): The name of the table
 
         Returns:
             Optional[list[ColumnSchema]]: The list of columns
         """
         table = self._get_table_by_name(table_name)
         return None if table is None else table.columns
 
-    def get_column(self, table_name: str, column_name: str) -> Optional[ColumnSchema]:
+    def get_column(self, table_name: str, column_name: str) -> ColumnSchema | None:
         """Gets a column for a table
 
         Args:
             table_name (str): The name of the table to get the column for
             column_name (str): The name of the column to get
 
         Returns:
```

### Comparing `schematic_db-0.0.dev33/schematic_db/schema/schema.py` & `schematic_db-0.1.0/schematic_db/schema/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Schema class"""
+
 # pylint: disable=duplicate-code
 
-from typing import Optional
 import warnings
 from pydantic.dataclasses import dataclass
 from pydantic import validator
 import validators
 from schematic_db.db_schema.db_schema import (
     DatabaseSchema,
     TableSchema,
@@ -18,14 +18,15 @@
     get_property_label_from_display_name,
     is_node_required,
     get_node_validation_rules,
     SchematicAPIError,
     SchematicAPITimeoutError,
 )
 from schematic_db.schema_graph.schema_graph import SchemaGraph
+from schematic_db.utils import DisplayLabelType
 from .database_config import DatabaseConfig
 
 
 class NoColumnsWarning(Warning):
     """
     Occurs when a database table has no columns returned from find_class_specific_properties().
     """
@@ -105,50 +106,49 @@
         valid_url = validators.url(value)
         if not valid_url:
             raise ValueError(f"{value} is a valid url")
         return value
 
     @validator("schema_url")
     @classmethod
-    def validate_is_jsonld(cls, value: str) -> str:
-        """Validates that the value is a jsonld file"""
-        is_jsonld = value.endswith(".jsonld")
-        if not is_jsonld:
-            raise ValueError(f"{value} does end with '.jsonld'")
+    def validate_is_valid_type(cls, value: str) -> str:
+        """Validates that the value is a jsonld or csv file"""
+        is_valid_type = value.endswith(".jsonld") | value.endswith(".csv")
+        if not is_valid_type:
+            raise ValueError(f"{value} does end with '.jsonld', or '.csv")
         return value
 
 
 class Schema:
     """
     The Schema class interacts with the Schematic API to create a DatabaseSchema
      table.
     """
 
     def __init__(
         self,
         config: SchemaConfig,
         database_config: DatabaseConfig = DatabaseConfig([]),
-        use_display_names_as_labels: bool = False,
+        display_label_type: DisplayLabelType = "class_label",
     ) -> None:
         """
         The Schema class handles interactions with the schematic API.
         The main responsibilities are creating the database schema, and retrieving manifests.
 
         Args:
             config (SchemaConfig): A config describing the basic inputs for the schema table
             database_config (DatabaseConfig): Experimental and will be deprecated in the near
              future. A config describing optional database specific columns.
-            use_display_names_as_labels(bool): Experimental and will be deprecated in the near
-             future. Use when display names and labels are the same in the schema.
+            display_label_type (DisplayLabelType): The type of label used for display purposes
         """
         self.database_config = database_config
         self.schema_url = config.schema_url
-        self.use_display_names_as_labels = use_display_names_as_labels
-        self.schema_graph = SchemaGraph(config.schema_url)
-        self.database_schema: Optional[DatabaseSchema] = None
+        self.display_label_type = display_label_type
+        self.schema_graph = SchemaGraph(config.schema_url, display_label_type)
+        self.database_schema: DatabaseSchema | None = None
 
     def get_database_schema(self) -> DatabaseSchema:
         """Gets the current database schema
 
         Returns:
             DatabaseSchema: the current database schema
         """
@@ -164,15 +164,15 @@
         table_schemas = [
             schema
             for schema in [self._create_table_schema(name) for name in table_names]
             if schema is not None
         ]
         self.database_schema = DatabaseSchema(table_schemas)
 
-    def _create_table_schema(self, table_name: str) -> Optional[TableSchema]:
+    def _create_table_schema(self, table_name: str) -> TableSchema | None:
         """Creates the the schema for one table in the database, if any column
          schemas can be created.
 
         Args:
             table_name (str): The name of the table the schema will be created for.
 
         Returns:
@@ -190,25 +190,27 @@
             primary_key=self._get_primary_key(table_name),
             foreign_keys=self._get_foreign_keys(table_name),
         )
 
     def _create_column_schemas(
         self,
         table_name: str,
-    ) -> Optional[list[ColumnSchema]]:
+    ) -> list[ColumnSchema] | None:
         """Create the column schemas for the table, if any can be created.
 
         Args:
             table_name (str): The name of the table to create the column schemas for
 
         Returns:
-            Optional[list[ColumnSchema]]: A list of columns in ColumnSchema form
+            list[ColumnSchema] | None: A list of columns in ColumnSchema form
         """
         # the names of the columns to be created, in label(not display) form
-        column_names = find_class_specific_properties(self.schema_url, table_name)
+        column_names = find_class_specific_properties(
+            self.schema_url, table_name, self.display_label_type
+        )
         columns = [
             self._create_column_schema(name, table_name) for name in column_names
         ]
         # Some Tables will not have any columns for various reasons
         if not columns:
             warnings.warn(
                 NoColumnsWarning(
@@ -251,15 +253,17 @@
             ColumnSchematicError: Raised when there is an issue with getting a result from the
              schematic API
 
         Returns:
             bool: Is the column required?
         """
         try:
-            is_column_required = is_node_required(self.schema_url, column_name)
+            is_column_required = is_node_required(
+                self.schema_url, column_name, self.display_label_type
+            )
         except (SchematicAPIError, SchematicAPITimeoutError) as exc:
             raise ColumnSchematicError(column_name, table_name) from exc
         return is_column_required
 
     def _get_column_datatype(self, column_name: str, table_name: str) -> ColumnDatatype:
         """Gets the datatype for the column
 
@@ -282,15 +286,15 @@
             "num": ColumnDatatype.FLOAT,
             "int": ColumnDatatype.INT,
             "date": ColumnDatatype.DATE,
         }
         # Try to get validation rules from Schematic API
         try:
             all_validation_rules = get_node_validation_rules(
-                self.schema_url, column_name
+                self.schema_url, column_name, self.display_label_type
             )
         except (SchematicAPIError, SchematicAPITimeoutError) as exc:
             raise ColumnSchematicError(column_name, table_name) from exc
         # Try to get type from validation rules
         type_validation_rules = [
             rule for rule in all_validation_rules if rule in datatypes
         ]
@@ -373,10 +377,8 @@
 
         Args:
             column_name (str): The name of the column
 
         Returns:
             str: The column name of the column
         """
-        if self.use_display_names_as_labels:
-            return column_name
-        return get_property_label_from_display_name(self.schema_url, column_name)
+        return get_property_label_from_display_name(column_name)
```

### Comparing `schematic_db-0.0.dev33/schematic_db/schema_graph/schema_graph.py` & `schematic_db-0.1.0/schematic_db/schema_graph/schema_graph.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 """Stores the graph structure of the database schema"""
 
 import networkx
 from schematic_db.api_utils.api_utils import get_graph_by_edge_type
+from schematic_db.utils import DisplayLabelType
 
 
 class SchemaGraph:
     """
     Stores the graph structure of the database schema
     """
 
-    def __init__(self, schema_url: str) -> None:
+    def __init__(
+        self, schema_url: str, display_label_type: DisplayLabelType = "display_label"
+    ) -> None:
         """
         Args:
             schema_url (str): The url of the schema in jsonld form.
+            display_label_type (DisplayLabelType): The type of display label used
         """
         self.schema_url = schema_url
+        self.display_label_type = display_label_type
         self.schema_graph = self.create_schema_graph()
 
     def create_schema_graph(self) -> networkx.DiGraph:
         """Retrieve the edges from schematic API and store in networkx.DiGraph()
 
         Returns:
             networkx.DiGraph: The edges of the graph
         """
-        subgraph = get_graph_by_edge_type(self.schema_url, "requiresComponent")
+        subgraph = get_graph_by_edge_type(
+            self.schema_url, "requiresComponent", self.display_label_type
+        )
         schema_graph = networkx.DiGraph()
         schema_graph.add_edges_from(subgraph)
         return schema_graph
 
     def create_sorted_table_name_list(self) -> list[str]:
         """
         Uses the schema graph to create a table name list where tables always come after ones they
```

### Comparing `schematic_db-0.0.dev33/schematic_db/synapse/synapse.py` & `schematic_db-0.1.0/schematic_db/synapse/synapse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Synapse"""
+
 from typing import Any
 from tenacity import retry, stop_after_attempt, wait_fixed, retry_if_exception_type
 import synapseclient  # type: ignore
 import pandas  # type: ignore
 
 
 class SynapseTableNameError(Exception):
@@ -64,15 +65,15 @@
         Args:
             synapse_id (str): The Synapse id of the file
 
         Returns:
             pandas.DataFrame: The file in dataframe form
         """
         entity = self.syn.get(synapse_id)
-        return pandas.read_csv(entity.path)
+        return pandas.read_csv(entity.path, keep_default_na=False, na_values="")
 
     def get_table_names(self) -> list[str]:
         """Gets the names of the tables in the schema
 
         Returns:
             list[str]: A list of table names
         """
@@ -166,27 +167,30 @@
         """
         result = self.execute_sql_statement(query, include_row_data)
         table = pandas.read_csv(result.filepath)
         return table
 
     def execute_sql_statement(
         self, statement: str, include_row_data: bool = False
-    ) -> Any:
+    ) -> synapseclient.table.CsvFileTable:
         """Execute a SQL statement
 
         Args:
             statement (str): A SQL statement that can be run by Synapse
             include_row_data (bool): Include row_id and row_etag. Defaults to False.
 
         Returns:
-            any: An object from
+            synapseclient.table.CsvFileTable: The synapse table result from
+              the provided statement
         """
-        return self.syn.tableQuery(
+        table = self.syn.tableQuery(
             statement, includeRowIdAndRowVersion=include_row_data
         )
+        assert isinstance(table, synapseclient.table.CsvFileTable)
+        return table
 
     def build_table(self, table_name: str, table: pandas.DataFrame) -> None:
         """Adds a table to the project based on the input table
 
         Args:
             table_name (str): The name fo the table
             table (pandas.DataFrame): A dataframe of the table
```

