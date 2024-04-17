# Comparing `tmp/sqlalchemy_schema_factory-0.1.2.tar.gz` & `tmp/sqlalchemy_schema_factory-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_schema_factory-0.1.2.tar", max compression
+gzip compressed data, was "sqlalchemy_schema_factory-0.1.3.tar", max compression
```

## Comparing `sqlalchemy_schema_factory-0.1.2.tar` & `sqlalchemy_schema_factory-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       79 2024-04-15 12:07:12.792817 sqlalchemy_schema_factory-0.1.2/README.md
--rw-r--r--   0        0        0      511 2024-04-15 12:11:24.192670 sqlalchemy_schema_factory-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       80 2024-01-11 09:14:13.699175 sqlalchemy_schema_factory-0.1.2/sqlalchemy_schema_factory/__init__.py
--rw-r--r--   0        0        0      807 2022-07-27 17:35:59.300000 sqlalchemy_schema_factory-0.1.2/sqlalchemy_schema_factory/auxiliary.py
--rw-r--r--   0        0        0      699 2022-07-27 17:35:59.303000 sqlalchemy_schema_factory-0.1.2/sqlalchemy_schema_factory/conventions.py
--rw-r--r--   0        0        0     7236 2023-10-22 17:21:00.808619 sqlalchemy_schema_factory-0.1.2/sqlalchemy_schema_factory/factory.py
--rw-r--r--   0        0        0       58 2024-01-11 09:14:13.699423 sqlalchemy_schema_factory-0.1.2/sqlalchemy_schema_factory/jsonb/__init__.py
--rw-r--r--   0        0        0      538 2024-01-11 09:14:13.699814 sqlalchemy_schema_factory-0.1.2/sqlalchemy_schema_factory/jsonb/decoding.py
--rw-r--r--   0        0        0      669 2024-01-11 09:14:13.699968 sqlalchemy_schema_factory-0.1.2/sqlalchemy_schema_factory/jsonb/encoding.py
--rw-r--r--   0        0        0      712 1970-01-01 00:00:00.000000 sqlalchemy_schema_factory-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       79 2024-04-15 12:07:12.792817 sqlalchemy_schema_factory-0.1.3/README.md
+-rw-r--r--   0        0        0      510 2024-04-17 08:14:57.989699 sqlalchemy_schema_factory-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       80 2024-01-11 09:14:13.699175 sqlalchemy_schema_factory-0.1.3/sqlalchemy_schema_factory/__init__.py
+-rw-r--r--   0        0        0      807 2022-07-27 17:35:59.300000 sqlalchemy_schema_factory-0.1.3/sqlalchemy_schema_factory/auxiliary.py
+-rw-r--r--   0        0        0      699 2022-07-27 17:35:59.303000 sqlalchemy_schema_factory-0.1.3/sqlalchemy_schema_factory/conventions.py
+-rw-r--r--   0        0        0     7236 2023-10-22 17:21:00.808619 sqlalchemy_schema_factory-0.1.3/sqlalchemy_schema_factory/factory.py
+-rw-r--r--   0        0        0       58 2024-01-11 09:14:13.699423 sqlalchemy_schema_factory-0.1.3/sqlalchemy_schema_factory/jsonb/__init__.py
+-rw-r--r--   0        0        0      538 2024-01-11 09:14:13.699814 sqlalchemy_schema_factory-0.1.3/sqlalchemy_schema_factory/jsonb/decoding.py
+-rw-r--r--   0        0        0      669 2024-01-11 09:14:13.699968 sqlalchemy_schema_factory-0.1.3/sqlalchemy_schema_factory/jsonb/encoding.py
+-rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 sqlalchemy_schema_factory-0.1.3/PKG-INFO
```

### Comparing `sqlalchemy_schema_factory-0.1.2/sqlalchemy_schema_factory/auxiliary.py` & `sqlalchemy_schema_factory-0.1.3/sqlalchemy_schema_factory/auxiliary.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_schema_factory-0.1.2/sqlalchemy_schema_factory/conventions.py` & `sqlalchemy_schema_factory-0.1.3/sqlalchemy_schema_factory/conventions.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_schema_factory-0.1.2/sqlalchemy_schema_factory/factory.py` & `sqlalchemy_schema_factory-0.1.3/sqlalchemy_schema_factory/factory.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_schema_factory-0.1.2/sqlalchemy_schema_factory/jsonb/decoding.py` & `sqlalchemy_schema_factory-0.1.3/sqlalchemy_schema_factory/jsonb/decoding.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_schema_factory-0.1.2/sqlalchemy_schema_factory/jsonb/encoding.py` & `sqlalchemy_schema_factory-0.1.3/sqlalchemy_schema_factory/jsonb/encoding.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_schema_factory-0.1.2/PKG-INFO` & `sqlalchemy_schema_factory-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-schema-factory
-Version: 0.1.2
+Version: 0.1.3
 Summary: Collection of tools for building sqlalchemy schemas
 Home-page: https://github.com/smairon/sqlalchemy-schema-factory
 Author: Smairon
 Author-email: man@smairon.ru
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: sqlalchemy (>=1.4.39,<2.0.0)
+Requires-Dist: sqlalchemy (>=2.0.0,<3.0.0)
 Project-URL: Repository, https://github.com/smairon/sqlalchemy-schema-factory
 Description-Content-Type: text/markdown
 
 # Sqlalchemy schema factory
 Collection of tools for building sqlalchemy schemas
```

