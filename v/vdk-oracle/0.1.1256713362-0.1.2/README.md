# Comparing `tmp/vdk_oracle-0.1.1256713362.tar.gz` & `tmp/vdk-oracle-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk_oracle-0.1.1256713362.tar", last modified: Wed Apr 17 09:54:37 2024, max compression
+gzip compressed data, was "vdk-oracle-0.1.2.tar", last modified: Tue Jan 16 23:54:31 2024, max compression
```

## Comparing `vdk_oracle-0.1.1256713362.tar` & `vdk-oracle-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:54:37.577650 vdk_oracle-0.1.1256713362/
--rw-r--r--   0 root         (0) root         (0)     9651 2024-04-17 09:54:37.577650 vdk_oracle-0.1.1256713362/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     8642 2024-04-17 09:54:14.000000 vdk_oracle-0.1.1256713362/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 09:54:37.577650 vdk_oracle-0.1.1256713362/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1701 2024-04-17 09:54:20.000000 vdk_oracle-0.1.1256713362/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:54:37.573650 vdk_oracle-0.1.1256713362/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:54:37.573650 vdk_oracle-0.1.1256713362/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:54:37.573650 vdk_oracle-0.1.1256713362/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:54:37.573650 vdk_oracle-0.1.1256713362/src/vdk/plugin/oracle/
--rw-rw-rw-   0 root         (0) root         (0)    10702 2024-04-17 09:54:14.000000 vdk_oracle-0.1.1256713362/src/vdk/plugin/oracle/ingest_to_oracle.py
--rw-rw-rw-   0 root         (0) root         (0)     5120 2024-04-17 09:54:14.000000 vdk_oracle-0.1.1256713362/src/vdk/plugin/oracle/oracle_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     3296 2024-04-17 09:54:14.000000 vdk_oracle-0.1.1256713362/src/vdk/plugin/oracle/oracle_connection.py
--rw-rw-rw-   0 root         (0) root         (0)     4017 2024-04-17 09:54:14.000000 vdk_oracle-0.1.1256713362/src/vdk/plugin/oracle/oracle_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:54:37.577650 vdk_oracle-0.1.1256713362/src/vdk_oracle.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9651 2024-04-17 09:54:37.000000 vdk_oracle-0.1.1256713362/src/vdk_oracle.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2024-04-17 09:54:37.000000 vdk_oracle-0.1.1256713362/src/vdk_oracle.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 09:54:37.000000 vdk_oracle-0.1.1256713362/src/vdk_oracle.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2024-04-17 09:54:37.000000 vdk_oracle-0.1.1256713362/src/vdk_oracle.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       27 2024-04-17 09:54:37.000000 vdk_oracle-0.1.1256713362/src/vdk_oracle.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2024-04-17 09:54:37.000000 vdk_oracle-0.1.1256713362/src/vdk_oracle.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:54:37.577650 vdk_oracle-0.1.1256713362/tests/
--rw-rw-rw-   0 root         (0) root         (0)    16601 2024-04-17 09:54:14.000000 vdk_oracle-0.1.1256713362/tests/test_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     5228 2024-04-17 09:54:14.000000 vdk_oracle-0.1.1256713362/tests/test_secrets_config.py
+drwxr-xr-x   0 aivanov    (502) staff       (20)        0 2024-01-16 23:54:31.982146 vdk-oracle-0.1.2/
+-rw-r--r--   0 aivanov    (502) staff       (20)     7363 2024-01-16 23:54:31.979875 vdk-oracle-0.1.2/PKG-INFO
+-rw-r--r--   0 aivanov    (502) staff       (20)     6414 2024-01-16 16:15:12.000000 vdk-oracle-0.1.2/README.md
+-rw-r--r--   0 aivanov    (502) staff       (20)       38 2024-01-16 23:54:31.982451 vdk-oracle-0.1.2/setup.cfg
+-rw-r--r--   0 aivanov    (502) staff       (20)     1646 2024-01-16 23:54:23.000000 vdk-oracle-0.1.2/setup.py
+drwxr-xr-x   0 aivanov    (502) staff       (20)        0 2024-01-16 23:54:31.957032 vdk-oracle-0.1.2/src/
+drwxr-xr-x   0 aivanov    (502) staff       (20)        0 2024-01-16 23:54:31.955869 vdk-oracle-0.1.2/src/vdk/
+drwxr-xr-x   0 aivanov    (502) staff       (20)        0 2024-01-16 23:54:31.956330 vdk-oracle-0.1.2/src/vdk/plugin/
+drwxr-xr-x   0 aivanov    (502) staff       (20)        0 2024-01-16 23:54:31.965605 vdk-oracle-0.1.2/src/vdk/plugin/oracle/
+-rw-r--r--   0 aivanov    (502) staff       (20)     7702 2024-01-09 13:57:58.000000 vdk-oracle-0.1.2/src/vdk/plugin/oracle/ingest_to_oracle.py
+-rw-r--r--   0 aivanov    (502) staff       (20)     4340 2024-01-16 17:02:09.000000 vdk-oracle-0.1.2/src/vdk/plugin/oracle/oracle_configuration.py
+-rw-r--r--   0 aivanov    (502) staff       (20)     3168 2024-01-16 17:02:10.000000 vdk-oracle-0.1.2/src/vdk/plugin/oracle/oracle_connection.py
+-rw-r--r--   0 aivanov    (502) staff       (20)     4029 2024-01-16 17:02:09.000000 vdk-oracle-0.1.2/src/vdk/plugin/oracle/oracle_plugin.py
+drwxr-xr-x   0 aivanov    (502) staff       (20)        0 2024-01-16 23:54:31.976413 vdk-oracle-0.1.2/src/vdk_oracle.egg-info/
+-rw-r--r--   0 aivanov    (502) staff       (20)     7363 2024-01-16 23:54:31.000000 vdk-oracle-0.1.2/src/vdk_oracle.egg-info/PKG-INFO
+-rw-r--r--   0 aivanov    (502) staff       (20)      468 2024-01-16 23:54:31.000000 vdk-oracle-0.1.2/src/vdk_oracle.egg-info/SOURCES.txt
+-rw-r--r--   0 aivanov    (502) staff       (20)        1 2024-01-16 23:54:31.000000 vdk-oracle-0.1.2/src/vdk_oracle.egg-info/dependency_links.txt
+-rw-r--r--   0 aivanov    (502) staff       (20)       62 2024-01-16 23:54:31.000000 vdk-oracle-0.1.2/src/vdk_oracle.egg-info/entry_points.txt
+-rw-r--r--   0 aivanov    (502) staff       (20)       27 2024-01-16 23:54:31.000000 vdk-oracle-0.1.2/src/vdk_oracle.egg-info/requires.txt
+-rw-r--r--   0 aivanov    (502) staff       (20)        4 2024-01-16 23:54:31.000000 vdk-oracle-0.1.2/src/vdk_oracle.egg-info/top_level.txt
+drwxr-xr-x   0 aivanov    (502) staff       (20)        0 2024-01-16 23:54:31.974616 vdk-oracle-0.1.2/tests/
+-rw-r--r--   0 aivanov    (502) staff       (20)     8319 2024-01-16 17:02:09.000000 vdk-oracle-0.1.2/tests/test_plugin.py
+-rw-r--r--   0 aivanov    (502) staff       (20)     5232 2024-01-09 13:57:58.000000 vdk-oracle-0.1.2/tests/test_secrets_config.py
```

### Comparing `vdk_oracle-0.1.1256713362/PKG-INFO` & `vdk-oracle-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 Metadata-Version: 2.1
 Name: vdk-oracle
-Version: 0.1.1256713362
+Version: 0.1.2
 Summary: Support for VDK Managed Oracle connection
 Home-page: https://github.com/vmware/versatile-data-kit
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/tree/main/projects/vdk-plugins/vdk-oracle
 Project-URL: Source Code, https://github.com/vmware/versatile-data-kit/tree/main/projects/vdk-plugins/vdk-oracle
 Project-URL: Bug Tracker, https://github.com/vmware/versatile-data-kit/issues/new/choose
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: vdk-core
 Requires-Dist: oracledb
 Requires-Dist: tabulate
 
 # oracle
 
-<a href="https://pypistats.org/packages/vdk-oracle" alt="Monthly Downloads">
-        <img src="https://img.shields.io/pypi/dm/vdk-oracle.svg" alt="monthly download count for vdk-oracle"></a>
-
 Support for VDK Managed Oracle connection
 
 TODO: what the project is about, what is its purpose
 
 
 ## Usage
 
@@ -44,17 +40,15 @@
 | oracle_user              | Username used when connecting to Oracle database                                                                                                                                                                                      | my_user             |
 | oracle_password          | Password used when connecting to Oracle database                                                                                                                                                                                      | super_secret_shhhh  |
 | oracle_use_secrets       | Set to True to use secrets to connect to Oracle                                                                                                                                                                                       | True                |
 | oracle_connection_string | The Oracle connection string                                                                                                                                                                                                          | localhost:1521/free |
 | oracle_host              | The host of the Oracle database. Note: This gets overridden if oracle_connection_string is set.                                                                                                                                       | localhost           |
 | oracle_port              | The port of the Oracle database. Note: This gets overridden if oracle_connection_string is set.                                                                                                                                       | 1521                |
 | oracle_sid               | The SID of the Oracle database. Note: This gets overridden if oracle_connection_string is set.                                                                                                                                        | free                |
-| oracle_service_name      | The Service name of the Oracle database. Note: This gets overridden if oracle_connection_string is set.                                                                                                                               | free                |
 | oracle_thick_mode        | Python-oracledb is said to be in Thick mode when Oracle Client libraries are used. True by default. Set to False to disable Oracle Thick mode. More info: https://python-oracledb.readthedocs.io/en/latest/user_guide/appendix_b.html | True                |
-| oracle_ingest_batch_size | vdk-oracle splits ingestion payloads into batches. Change this config to control the batch size. Default is set to 100.                                                                                                               | 100                 |
 
 ### Example
 
 #### CLI Queries
 
 ```sh
 export VDK_ORACLE_USER=my_username
@@ -159,71 +153,14 @@
         "bool_data": "False",
         "timestamp_data": "2023-11-21T08:12:53",
         "decimal_data": "0.1",
     }
 
     job_input.send_object_for_ingestion(payload=payload, destination_table="test_table")
 ```
-
-#### Case Sensitivity
-
-**vdk-oracle supports only lower-case and upper-case payload keys.** Oracle is case-insensitive by default. This is a
-challenge when ingesting payloads and doing type and schema inference, so we've opted for the simplest solution to
-avoid confusion on the user side.
-
-**Valid Ingestion**
-
-```python
-def run(job_input):
-    payload = {
-        "id": "5",
-        "str_data": "string",
-        "int_data": "12",
-        "float_data": "1.2",
-        "bool_data": "False",
-        "timestamp_data": "2023-11-21T08:12:53",
-        "decimal_data": "0.1",
-    }
-
-    job_input.send_object_for_ingestion(payload=payload, destination_table="test_table")
-```
-
-```python
-def run(job_input):
-    payload = {
-        "ID": "5",
-        "STR_DATA": "string",
-        "INT_DATA": "12",
-        "FLOAT_DATA": "1.2",
-        "BOOL_DATA": "False",
-        "TIMESTAMP_DATA": "2023-11-21T08:12:53",
-        "DECIMAL_DATA": "0.1",
-    }
-
-    job_input.send_object_for_ingestion(payload=payload, destination_table="TEST_TABLE")
-```
-
-**Invalid ingestion**
-
-Will infer the schema, but won't insert correctly.
-
-```python
-def run(job_input):
-    payload = {
-        "Id": "5",
-        "Str_Data": "string",
-        "Int_Data": "12",
-        "Float_Data": "1.2",
-        "Bool_Data": "False",
-        "Timestamp_Data": "2023-11-21T08:12:53",
-        "Decimal_Data": "0.1",
-    }
-    job_input.send_object_for_ingestion(payload=payload, destination_table="test_table")
-```
-
 ### Build and testing
 
 ```
 pip install -r requirements.txt
 pip install -e .
 pytest
 ```
```

### Comparing `vdk_oracle-0.1.1256713362/README.md` & `vdk-oracle-0.1.2/src/vdk_oracle.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,28 @@
-# oracle
+Metadata-Version: 2.1
+Name: vdk-oracle
+Version: 0.1.2
+Summary: Support for VDK Managed Oracle connection
+Home-page: https://github.com/vmware/versatile-data-kit
+Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/tree/main/projects/vdk-plugins/vdk-oracle
+Project-URL: Source Code, https://github.com/vmware/versatile-data-kit/tree/main/projects/vdk-plugins/vdk-oracle
+Project-URL: Bug Tracker, https://github.com/vmware/versatile-data-kit/issues/new/choose
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+Requires-Dist: vdk-core
+Requires-Dist: oracledb
+Requires-Dist: tabulate
 
-<a href="https://pypistats.org/packages/vdk-oracle" alt="Monthly Downloads">
-        <img src="https://img.shields.io/pypi/dm/vdk-oracle.svg" alt="monthly download count for vdk-oracle"></a>
+# oracle
 
 Support for VDK Managed Oracle connection
 
 TODO: what the project is about, what is its purpose
 
 
 ## Usage
@@ -23,17 +40,15 @@
 | oracle_user              | Username used when connecting to Oracle database                                                                                                                                                                                      | my_user             |
 | oracle_password          | Password used when connecting to Oracle database                                                                                                                                                                                      | super_secret_shhhh  |
 | oracle_use_secrets       | Set to True to use secrets to connect to Oracle                                                                                                                                                                                       | True                |
 | oracle_connection_string | The Oracle connection string                                                                                                                                                                                                          | localhost:1521/free |
 | oracle_host              | The host of the Oracle database. Note: This gets overridden if oracle_connection_string is set.                                                                                                                                       | localhost           |
 | oracle_port              | The port of the Oracle database. Note: This gets overridden if oracle_connection_string is set.                                                                                                                                       | 1521                |
 | oracle_sid               | The SID of the Oracle database. Note: This gets overridden if oracle_connection_string is set.                                                                                                                                        | free                |
-| oracle_service_name      | The Service name of the Oracle database. Note: This gets overridden if oracle_connection_string is set.                                                                                                                               | free                |
 | oracle_thick_mode        | Python-oracledb is said to be in Thick mode when Oracle Client libraries are used. True by default. Set to False to disable Oracle Thick mode. More info: https://python-oracledb.readthedocs.io/en/latest/user_guide/appendix_b.html | True                |
-| oracle_ingest_batch_size | vdk-oracle splits ingestion payloads into batches. Change this config to control the batch size. Default is set to 100.                                                                                                               | 100                 |
 
 ### Example
 
 #### CLI Queries
 
 ```sh
 export VDK_ORACLE_USER=my_username
@@ -138,71 +153,14 @@
         "bool_data": "False",
         "timestamp_data": "2023-11-21T08:12:53",
         "decimal_data": "0.1",
     }
 
     job_input.send_object_for_ingestion(payload=payload, destination_table="test_table")
 ```
-
-#### Case Sensitivity
-
-**vdk-oracle supports only lower-case and upper-case payload keys.** Oracle is case-insensitive by default. This is a
-challenge when ingesting payloads and doing type and schema inference, so we've opted for the simplest solution to
-avoid confusion on the user side.
-
-**Valid Ingestion**
-
-```python
-def run(job_input):
-    payload = {
-        "id": "5",
-        "str_data": "string",
-        "int_data": "12",
-        "float_data": "1.2",
-        "bool_data": "False",
-        "timestamp_data": "2023-11-21T08:12:53",
-        "decimal_data": "0.1",
-    }
-
-    job_input.send_object_for_ingestion(payload=payload, destination_table="test_table")
-```
-
-```python
-def run(job_input):
-    payload = {
-        "ID": "5",
-        "STR_DATA": "string",
-        "INT_DATA": "12",
-        "FLOAT_DATA": "1.2",
-        "BOOL_DATA": "False",
-        "TIMESTAMP_DATA": "2023-11-21T08:12:53",
-        "DECIMAL_DATA": "0.1",
-    }
-
-    job_input.send_object_for_ingestion(payload=payload, destination_table="TEST_TABLE")
-```
-
-**Invalid ingestion**
-
-Will infer the schema, but won't insert correctly.
-
-```python
-def run(job_input):
-    payload = {
-        "Id": "5",
-        "Str_Data": "string",
-        "Int_Data": "12",
-        "Float_Data": "1.2",
-        "Bool_Data": "False",
-        "Timestamp_Data": "2023-11-21T08:12:53",
-        "Decimal_Data": "0.1",
-    }
-    job_input.send_object_for_ingestion(payload=payload, destination_table="test_table")
-```
-
 ### Build and testing
 
 ```
 pip install -r requirements.txt
 pip install -e .
 pytest
 ```
```

### Comparing `vdk_oracle-0.1.1256713362/setup.py` & `vdk-oracle-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# Copyright 2023-2024 Broadcom
+# Copyright 2021-2024 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 """
 Builds a package with the help of setuptools in order for this package to be imported in other projects
 """
 
-__version__ = "0.1.1256713362"
+__version__ = "0.1.2"
 
 setuptools.setup(
     name="vdk-oracle",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Support for VDK Managed Oracle connection",
     long_description=pathlib.Path("README.md").read_text(),
@@ -27,15 +27,14 @@
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3.12",
     ],
     project_urls={
         "Documentation": "https://github.com/vmware/versatile-data-kit/tree/main/projects/vdk-plugins/vdk-oracle",
         "Source Code": "https://github.com/vmware/versatile-data-kit/tree/main/projects/vdk-plugins/vdk-oracle",
         "Bug Tracker": "https://github.com/vmware/versatile-data-kit/issues/new/choose",
     },
 )
```

### Comparing `vdk_oracle-0.1.1256713362/src/vdk/plugin/oracle/oracle_configuration.py` & `vdk-oracle-0.1.2/src/vdk/plugin/oracle/oracle_configuration.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023-2024 Broadcom
+# Copyright 2021-2024 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import json
 import pathlib
 import tempfile
 from typing import Dict
 from typing import Optional
 
@@ -14,16 +14,14 @@
 ORACLE_USE_SECRETS = "ORACLE_USE_SECRETS"
 ORACLE_THICK_MODE = "ORACLE_THICK_MODE"
 ORACLE_THICK_MODE_LIB_DIR = "ORACLE_THICK_MODE_LIB_DIR"
 ORACLE_CONNECTION_STRING = "ORACLE_CONNECTION_STRING"
 ORACLE_HOST = "ORACLE_HOST"
 ORACLE_PORT = "ORACLE_PORT"
 ORACLE_SID = "ORACLE_SID"
-ORACLE_SERVICE_NAME = "ORACLE_SERVICE_NAME"
-ORACLE_INGEST_BATCH_SIZE = "ORACLE_INGEST_BATCH_SIZE"
 
 
 class OracleConfiguration:
     def __init__(self, configuration: Configuration):
         self.__config = configuration
 
     def get_oracle_user(self) -> str:
@@ -40,29 +38,23 @@
 
     def get_oracle_port(self) -> int:
         return int(self.__config.get_value(ORACLE_PORT))
 
     def get_oracle_sid(self) -> str:
         return self.__config.get_value(ORACLE_SID)
 
-    def get_oracle_service_name(self) -> str:
-        return self.__config.get_value(ORACLE_SERVICE_NAME)
-
     def oracle_use_secrets(self) -> bool:
         return self.__config.get_value(ORACLE_USE_SECRETS)
 
     def oracle_thick_mode(self) -> bool:
         return self.__config.get_value(ORACLE_THICK_MODE)
 
     def oracle_thick_mode_lib_dir(self) -> Optional[str]:
         return self.__config.get_value(ORACLE_THICK_MODE_LIB_DIR)
 
-    def oracle_ingest_batch_size(self) -> Optional[int]:
-        return int(self.__config.get_value(ORACLE_INGEST_BATCH_SIZE))
-
     @staticmethod
     def add_definitions(config_builder: ConfigurationBuilder):
         config_builder.add(
             key=ORACLE_USER,
             default_value=None,
             is_sensitive=True,
             description="The Oracle user for the database connection",
@@ -94,40 +86,29 @@
         config_builder.add(
             key=ORACLE_SID,
             default_value=None,
             is_sensitive=True,
             description="The schema id of the Oracle database. Note: This option is overridden by ORACLE_CONNECTION_STRING",
         )
         config_builder.add(
-            key=ORACLE_SERVICE_NAME,
-            default_value=None,
-            is_sensitive=True,
-            description="The service name of the Oracle database. Note: This option is overridden by ORACLE_CONNECTION_STRING",
-        )
-        config_builder.add(
             key=ORACLE_USE_SECRETS,
             default_value=True,
             description="Set this flag to use secrets to connect to Oracle. This is protype option. "
             "Leave default value unless there are issues.",
         )
         config_builder.add(
             key=ORACLE_THICK_MODE,
-            default_value=True,
+            default_value=False,
             description="Use oracle thick mode. Set to False to disable oracle thick mode."
             "If set to true you may need to manually install client library. "
             "Refer to "
             "https://python-oracledb.readthedocs.io/en/latest/user_guide/initialization.html#enablingthick "
             "More info: https://python-oracledb.readthedocs.io/en/latest/user_guide/appendix_b.html",
         )
         config_builder.add(
             key=ORACLE_THICK_MODE_LIB_DIR,
             default_value=None,
-            description="This is the location of the Oracle Client library used when thick mode is enabled. "
+            description="This is the location of the Oracle Client library used when tick mode is enabled. "
             "This option is ignored if ORACLE_THICK_MODE is false."
             "Before setting this follow instruction in "
             "https://python-oracledb.readthedocs.io/en/latest/user_guide/initialization.html#enablingthick ",
         )
-        config_builder.add(
-            key=ORACLE_INGEST_BATCH_SIZE,
-            default_value=100,
-            description="Batch size when ingesting records into Oracle.",
-        )
```

### Comparing `vdk_oracle-0.1.1256713362/src/vdk/plugin/oracle/oracle_connection.py` & `vdk-oracle-0.1.2/src/vdk/plugin/oracle/oracle_connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023-2024 Broadcom
+# Copyright 2021-2024 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 from typing import Any
 from typing import List
 from typing import Optional
 
 from oracledb import Connection
@@ -18,26 +18,24 @@
     def __init__(
         self,
         user: str,
         password: str,
         connection_string: str = None,
         host=None,
         port=1521,
-        sid: str = None,
-        service_name: str = None,
+        sid=None,
         thick_mode: bool = True,
         thick_mode_lib_dir: Optional[str] = None,
     ):
         super().__init__(log)
         self._oracle_user = user
         self._oracle_password = password
         self._host = host
         self._port = port
         self._sid = sid
-        self._service_name = service_name
         self._oracle_connection_string = connection_string
         self._thick_mode = thick_mode
         self._thick_mode_lib_dir = thick_mode_lib_dir
 
     def _connect(self) -> Connection:
         import oracledb
 
@@ -58,15 +56,14 @@
             log.debug("Connecting to Oracle using host,port,sid")
             params = oracledb.ConnectParams(
                 user=self._oracle_user,
                 password=self._oracle_password,
                 host=self._host,
                 port=self._port,
                 sid=self._sid,
-                service_name=self._service_name,
             )
             conn = oracledb.connect(params=params)
         return conn
 
     def _is_connected(self) -> bool:
         if None is self._is_db_con_open:
             return False
```

### Comparing `vdk_oracle-0.1.1256713362/src/vdk/plugin/oracle/oracle_plugin.py` & `vdk-oracle-0.1.2/src/vdk/plugin/oracle/oracle_plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023-2024 Broadcom
+# Copyright 2021-2024 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 from typing import List
 
 import click
 import oracledb
 from tabulate import tabulate
@@ -31,56 +31,50 @@
     def vdk_configure(self, config_builder: ConfigurationBuilder):
         OracleConfiguration.add_definitions(config_builder)
 
     @hookimpl(trylast=True)
     def initialize_job(self, context: JobContext):
         conf = OracleConfiguration(context.core_context.configuration)
         oracle_user, oracle_pass = conf.get_oracle_user(), conf.get_oracle_password()
+        if conf.oracle_use_secrets():
+            # TODO: this will be removed once support for reading configuration from secrets is added in core
+            job_secrets = context.job_input.get_all_secrets()
+            oracle_user = job_secrets.get(ORACLE_USER.lower(), oracle_user)
+            oracle_pass = job_secrets.get(ORACLE_PASSWORD.lower(), oracle_pass)
         context.connections.add_open_connection_factory_method(
             "ORACLE",
             lambda: OracleConnection(
                 oracle_user,
                 oracle_pass,
                 conf.get_oracle_connection_string(),
                 host=conf.get_oracle_host(),
                 port=conf.get_oracle_port(),
                 sid=conf.get_oracle_sid(),
-                service_name=conf.get_oracle_service_name(),
                 thick_mode=conf.oracle_thick_mode(),
                 thick_mode_lib_dir=conf.oracle_thick_mode_lib_dir(),
             ),
         )
         context.ingester.add_ingester_factory_method(
-            "oracle",
-            lambda: IngestToOracle(
-                context.connections, conf.oracle_ingest_batch_size()
-            ),
+            "oracle", (lambda: IngestToOracle(context.connections))
         )
 
 
 @hookimpl
 def vdk_start(plugin_registry: IPluginRegistry, command_line_args: List):
     plugin_registry.load_plugin_with_hooks_impl(OraclePlugin(), "OraclePlugin")
 
 
 # TODO: https://github.com/vmware/versatile-data-kit/issues/2940
 @click.command(
     name="oracle-query",
-    help="DEPRECATED: use sql-query, instead."
-    "Execute an Oracle query against an Oracle database (should be configured with env variables)",
+    help="Execute an Oracle query against an Oracle database (should be configured with env variables)",
 )
 @click.option("-q", "--query", type=click.STRING, required=True)
 @click.pass_context
 def oracle_query(ctx: click.Context, query):
-    """
-    Deprecated: "Use sql-query instead"
-
-    oracle-query: kept for compatibility
-    """
-    log.warning("oracle-query has been deprecated; please use sql-query instead.")
     conf = ctx.obj.configuration
     conn = oracledb.connect(
         user=conf.get_value(ORACLE_USER),
         password=conf.get_value(ORACLE_PASSWORD),
         dsn=conf.get_value(ORACLE_CONNECTION_STRING),
     )
```

### Comparing `vdk_oracle-0.1.1256713362/src/vdk_oracle.egg-info/PKG-INFO` & `vdk-oracle-0.1.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,9 @@
-Metadata-Version: 2.1
-Name: vdk-oracle
-Version: 0.1.1256713362
-Summary: Support for VDK Managed Oracle connection
-Home-page: https://github.com/vmware/versatile-data-kit
-Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/tree/main/projects/vdk-plugins/vdk-oracle
-Project-URL: Source Code, https://github.com/vmware/versatile-data-kit/tree/main/projects/vdk-plugins/vdk-oracle
-Project-URL: Bug Tracker, https://github.com/vmware/versatile-data-kit/issues/new/choose
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Description-Content-Type: text/markdown
-Requires-Dist: vdk-core
-Requires-Dist: oracledb
-Requires-Dist: tabulate
-
 # oracle
 
-<a href="https://pypistats.org/packages/vdk-oracle" alt="Monthly Downloads">
-        <img src="https://img.shields.io/pypi/dm/vdk-oracle.svg" alt="monthly download count for vdk-oracle"></a>
-
 Support for VDK Managed Oracle connection
 
 TODO: what the project is about, what is its purpose
 
 
 ## Usage
 
@@ -44,17 +20,15 @@
 | oracle_user              | Username used when connecting to Oracle database                                                                                                                                                                                      | my_user             |
 | oracle_password          | Password used when connecting to Oracle database                                                                                                                                                                                      | super_secret_shhhh  |
 | oracle_use_secrets       | Set to True to use secrets to connect to Oracle                                                                                                                                                                                       | True                |
 | oracle_connection_string | The Oracle connection string                                                                                                                                                                                                          | localhost:1521/free |
 | oracle_host              | The host of the Oracle database. Note: This gets overridden if oracle_connection_string is set.                                                                                                                                       | localhost           |
 | oracle_port              | The port of the Oracle database. Note: This gets overridden if oracle_connection_string is set.                                                                                                                                       | 1521                |
 | oracle_sid               | The SID of the Oracle database. Note: This gets overridden if oracle_connection_string is set.                                                                                                                                        | free                |
-| oracle_service_name      | The Service name of the Oracle database. Note: This gets overridden if oracle_connection_string is set.                                                                                                                               | free                |
 | oracle_thick_mode        | Python-oracledb is said to be in Thick mode when Oracle Client libraries are used. True by default. Set to False to disable Oracle Thick mode. More info: https://python-oracledb.readthedocs.io/en/latest/user_guide/appendix_b.html | True                |
-| oracle_ingest_batch_size | vdk-oracle splits ingestion payloads into batches. Change this config to control the batch size. Default is set to 100.                                                                                                               | 100                 |
 
 ### Example
 
 #### CLI Queries
 
 ```sh
 export VDK_ORACLE_USER=my_username
@@ -159,71 +133,14 @@
         "bool_data": "False",
         "timestamp_data": "2023-11-21T08:12:53",
         "decimal_data": "0.1",
     }
 
     job_input.send_object_for_ingestion(payload=payload, destination_table="test_table")
 ```
-
-#### Case Sensitivity
-
-**vdk-oracle supports only lower-case and upper-case payload keys.** Oracle is case-insensitive by default. This is a
-challenge when ingesting payloads and doing type and schema inference, so we've opted for the simplest solution to
-avoid confusion on the user side.
-
-**Valid Ingestion**
-
-```python
-def run(job_input):
-    payload = {
-        "id": "5",
-        "str_data": "string",
-        "int_data": "12",
-        "float_data": "1.2",
-        "bool_data": "False",
-        "timestamp_data": "2023-11-21T08:12:53",
-        "decimal_data": "0.1",
-    }
-
-    job_input.send_object_for_ingestion(payload=payload, destination_table="test_table")
-```
-
-```python
-def run(job_input):
-    payload = {
-        "ID": "5",
-        "STR_DATA": "string",
-        "INT_DATA": "12",
-        "FLOAT_DATA": "1.2",
-        "BOOL_DATA": "False",
-        "TIMESTAMP_DATA": "2023-11-21T08:12:53",
-        "DECIMAL_DATA": "0.1",
-    }
-
-    job_input.send_object_for_ingestion(payload=payload, destination_table="TEST_TABLE")
-```
-
-**Invalid ingestion**
-
-Will infer the schema, but won't insert correctly.
-
-```python
-def run(job_input):
-    payload = {
-        "Id": "5",
-        "Str_Data": "string",
-        "Int_Data": "12",
-        "Float_Data": "1.2",
-        "Bool_Data": "False",
-        "Timestamp_Data": "2023-11-21T08:12:53",
-        "Decimal_Data": "0.1",
-    }
-    job_input.send_object_for_ingestion(payload=payload, destination_table="test_table")
-```
-
 ### Build and testing
 
 ```
 pip install -r requirements.txt
 pip install -e .
 pytest
 ```
```

### Comparing `vdk_oracle-0.1.1256713362/tests/test_secrets_config.py` & `vdk-oracle-0.1.2/tests/test_secrets_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023-2024 Broadcom
+# Copyright 2021-2024 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import json
 import os
 from unittest import mock
 
 import pytest
 from click.testing import Result
```

