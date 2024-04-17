# Comparing `tmp/kafka_schema_registry_admin-0.5.1.tar.gz` & `tmp/kafka_schema_registry_admin-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafka_schema_registry_admin-0.5.1.tar", max compression
+gzip compressed data, was "kafka_schema_registry_admin-0.5.2.tar", max compression
```

## Comparing `kafka_schema_registry_admin-0.5.1.tar` & `kafka_schema_registry_admin-0.5.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11358 2024-03-09 18:55:10.060282 kafka_schema_registry_admin-0.5.1/LICENSE
--rw-r--r--   0        0        0     1240 2024-03-10 20:28:07.462628 kafka_schema_registry_admin-0.5.1/README.rst
--rw-r--r--   0        0        0      831 2024-04-06 18:35:44.578590 kafka_schema_registry_admin-0.5.1/kafka_schema_registry_admin/__init__.py
--rw-r--r--   0        0        0    18174 2024-04-06 18:35:34.451788 kafka_schema_registry_admin-0.5.1/kafka_schema_registry_admin/async_schema_registry.py
--rw-r--r--   0        0        0     2868 2024-04-06 17:18:24.239586 kafka_schema_registry_admin-0.5.1/kafka_schema_registry_admin/client_wrapper/__init__.py
--rw-r--r--   0        0        0     3731 2024-04-06 17:18:24.239586 kafka_schema_registry_admin-0.5.1/kafka_schema_registry_admin/client_wrapper/async_client.py
--rw-r--r--   0        0        0     4086 2024-04-06 17:18:24.239586 kafka_schema_registry_admin-0.5.1/kafka_schema_registry_admin/client_wrapper/errors.py
--rw-r--r--   0        0        0    14622 2024-04-06 18:35:34.451788 kafka_schema_registry_admin-0.5.1/kafka_schema_registry_admin/kafka_schema_registry_admin.py
--rw-r--r--   0        0        0     1707 2024-04-06 18:35:44.578590 kafka_schema_registry_admin-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1994 1970-01-01 00:00:00.000000 kafka_schema_registry_admin-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-03-09 18:55:10.060282 kafka_schema_registry_admin-0.5.2/LICENSE
+-rw-r--r--   0        0        0     1240 2024-03-10 20:28:07.462628 kafka_schema_registry_admin-0.5.2/README.rst
+-rw-r--r--   0        0        0      830 2024-04-17 07:55:21.764237 kafka_schema_registry_admin-0.5.2/kafka_schema_registry_admin/__init__.py
+-rw-r--r--   0        0        0    18174 2024-04-06 18:35:34.451788 kafka_schema_registry_admin-0.5.2/kafka_schema_registry_admin/async_schema_registry.py
+-rw-r--r--   0        0        0     2868 2024-04-06 17:18:24.239586 kafka_schema_registry_admin-0.5.2/kafka_schema_registry_admin/client_wrapper/__init__.py
+-rw-r--r--   0        0        0     3731 2024-04-06 17:18:24.239586 kafka_schema_registry_admin-0.5.2/kafka_schema_registry_admin/client_wrapper/async_client.py
+-rw-r--r--   0        0        0     4086 2024-04-06 17:18:24.239586 kafka_schema_registry_admin-0.5.2/kafka_schema_registry_admin/client_wrapper/errors.py
+-rw-r--r--   0        0        0    14622 2024-04-06 18:35:34.451788 kafka_schema_registry_admin-0.5.2/kafka_schema_registry_admin/kafka_schema_registry_admin.py
+-rw-r--r--   0        0        0     1707 2024-04-17 07:55:21.764237 kafka_schema_registry_admin-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1994 1970-01-01 00:00:00.000000 kafka_schema_registry_admin-0.5.2/PKG-INFO
```

### Comparing `kafka_schema_registry_admin-0.5.1/LICENSE` & `kafka_schema_registry_admin-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kafka_schema_registry_admin-0.5.1/README.rst` & `kafka_schema_registry_admin-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `kafka_schema_registry_admin-0.5.1/kafka_schema_registry_admin/__init__.py` & `kafka_schema_registry_admin-0.5.2/kafka_schema_registry_admin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 """Top-level package for Kafka schema registry admin."""
 
 from __future__ import annotations
 
 __author__ = """JohnPreston"""
 __email__ = "john@ews-network.net"
-__version__ = "0.5.1"
+__version__ = "0.5.2"
 
 from enum import Enum
 
 
 class RegistryMode(Enum):
     IMPORT = "IMPORT"
     READONLY = "READONLY"
@@ -27,13 +27,13 @@
     FULL_TRANSITIVE = "FULL_TRANSITIVE"
     NONE = "NONE"
 
 
 class Type(Enum):
     AVRO = "AVRO"
     JSON = "JSON"
-    PROTOBUFF = "PROTOBUF"
+    PROTOBUF = "PROTOBUF"
 
 
 from .kafka_schema_registry_admin import SchemaRegistry
 
 __all__ = ["SchemaRegistry"]
```

### Comparing `kafka_schema_registry_admin-0.5.1/kafka_schema_registry_admin/async_schema_registry.py` & `kafka_schema_registry_admin-0.5.2/kafka_schema_registry_admin/async_schema_registry.py`

 * *Files identical despite different names*

### Comparing `kafka_schema_registry_admin-0.5.1/kafka_schema_registry_admin/client_wrapper/__init__.py` & `kafka_schema_registry_admin-0.5.2/kafka_schema_registry_admin/client_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka_schema_registry_admin-0.5.1/kafka_schema_registry_admin/client_wrapper/async_client.py` & `kafka_schema_registry_admin-0.5.2/kafka_schema_registry_admin/client_wrapper/async_client.py`

 * *Files identical despite different names*

### Comparing `kafka_schema_registry_admin-0.5.1/kafka_schema_registry_admin/client_wrapper/errors.py` & `kafka_schema_registry_admin-0.5.2/kafka_schema_registry_admin/client_wrapper/errors.py`

 * *Files identical despite different names*

### Comparing `kafka_schema_registry_admin-0.5.1/kafka_schema_registry_admin/kafka_schema_registry_admin.py` & `kafka_schema_registry_admin-0.5.2/kafka_schema_registry_admin/kafka_schema_registry_admin.py`

 * *Files identical despite different names*

### Comparing `kafka_schema_registry_admin-0.5.1/pyproject.toml` & `kafka_schema_registry_admin-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "kafka-schema-registry-admin"
-version = "0.5.1"
+version = "0.5.2"
 description = "Pure HTTP client to manage schemas in Schema Registry"
 authors = ["John Preston <john@ews-network.net>"]
 license = "Apache License 2.0"
 classifiers = [
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "Natural Language :: English",
@@ -37,15 +37,15 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.tbump]
 github_url = "https://github.com/compose-x/kafka_schema_registry_admin"
 
 [tool.tbump.version]
-current = "0.5.1"
+current = "0.5.2"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
```

### Comparing `kafka_schema_registry_admin-0.5.1/PKG-INFO` & `kafka_schema_registry_admin-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-schema-registry-admin
-Version: 0.5.1
+Version: 0.5.2
 Summary: Pure HTTP client to manage schemas in Schema Registry
 License: Apache-2.0
 Author: John Preston
 Author-email: john@ews-network.net
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

