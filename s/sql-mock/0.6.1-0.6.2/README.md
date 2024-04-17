# Comparing `tmp/sql_mock-0.6.1.tar.gz` & `tmp/sql_mock-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql_mock-0.6.1.tar", max compression
+gzip compressed data, was "sql_mock-0.6.2.tar", max compression
```

## Comparing `sql_mock-0.6.1.tar` & `sql_mock-0.6.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    10302 2024-04-08 07:45:26.242525 sql_mock-0.6.1/README.md
--rw-r--r--   0        0        0     2617 2024-04-08 07:45:26.246525 sql_mock-0.6.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/bigquery/__init__.py
--rw-r--r--   0        0        0      981 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/bigquery/column_mocks.py
--rw-r--r--   0        0        0      123 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/bigquery/settings.py
--rw-r--r--   0        0        0      681 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/bigquery/table_mocks.py
--rw-r--r--   0        0        0        0 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/clickhouse/__init__.py
--rw-r--r--   0        0        0     1230 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/clickhouse/column_mocks.py
--rw-r--r--   0        0        0      278 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/clickhouse/settings.py
--rw-r--r--   0        0        0      836 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/clickhouse/table_mocks.py
--rw-r--r--   0        0        0     1818 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/column_mocks.py
--rw-r--r--   0        0        0      387 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/config.py
--rw-r--r--   0        0        0       47 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/constants.py
--rw-r--r--   0        0        0     6300 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/dbt.py
--rw-r--r--   0        0        0       43 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/exceptions.py
--rw-r--r--   0        0        0     9185 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/helpers.py
--rw-r--r--   0        0        0        0 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/redshift/__init__.py
--rw-r--r--   0        0        0     1384 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/redshift/column_mocks.py
--rw-r--r--   0        0        0      266 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/redshift/settings.py
--rw-r--r--   0        0        0      839 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/redshift/table_mocks.py
--rw-r--r--   0        0        0        0 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/snowflake/__init__.py
--rw-r--r--   0        0        0     1319 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/snowflake/column_mocks.py
--rw-r--r--   0        0        0      225 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/snowflake/settings.py
--rw-r--r--   0        0        0      734 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/snowflake/table_mocks.py
--rw-r--r--   0        0        0    15214 2024-04-08 07:45:26.246525 sql_mock-0.6.1/src/sql_mock/table_mocks.py
--rw-r--r--   0        0        0    12482 1970-01-01 00:00:00.000000 sql_mock-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    10302 2024-04-17 10:06:38.556729 sql_mock-0.6.2/README.md
+-rw-r--r--   0        0        0     2705 2024-04-17 10:06:38.560729 sql_mock-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-17 10:06:38.560729 sql_mock-0.6.2/src/sql_mock/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 10:06:38.560729 sql_mock-0.6.2/src/sql_mock/bigquery/__init__.py
+-rw-r--r--   0        0        0      984 2024-04-17 10:06:38.560729 sql_mock-0.6.2/src/sql_mock/bigquery/column_mocks.py
+-rw-r--r--   0        0        0      123 2024-04-17 10:06:38.560729 sql_mock-0.6.2/src/sql_mock/bigquery/settings.py
+-rw-r--r--   0        0        0      681 2024-04-17 10:06:38.560729 sql_mock-0.6.2/src/sql_mock/bigquery/table_mocks.py
+-rw-r--r--   0        0        0        0 2024-04-17 10:06:38.560729 sql_mock-0.6.2/src/sql_mock/clickhouse/__init__.py
+-rw-r--r--   0        0        0     1233 2024-04-17 10:06:38.560729 sql_mock-0.6.2/src/sql_mock/clickhouse/column_mocks.py
+-rw-r--r--   0        0        0      278 2024-04-17 10:06:38.560729 sql_mock-0.6.2/src/sql_mock/clickhouse/settings.py
+-rw-r--r--   0        0        0      836 2024-04-17 10:06:38.560729 sql_mock-0.6.2/src/sql_mock/clickhouse/table_mocks.py
+-rw-r--r--   0        0        0     1818 2024-04-17 10:06:38.560729 sql_mock-0.6.2/src/sql_mock/column_mocks.py
+-rw-r--r--   0        0        0      387 2024-04-17 10:06:38.560729 sql_mock-0.6.2/src/sql_mock/config.py
+-rw-r--r--   0        0        0       47 2024-04-17 10:06:38.560729 sql_mock-0.6.2/src/sql_mock/constants.py
+-rw-r--r--   0        0        0     6300 2024-04-17 10:06:38.560729 sql_mock-0.6.2/src/sql_mock/dbt.py
+-rw-r--r--   0        0        0       43 2024-04-17 10:06:38.560729 sql_mock-0.6.2/src/sql_mock/exceptions.py
+-rw-r--r--   0        0        0     9147 2024-04-17 10:06:38.560729 sql_mock-0.6.2/src/sql_mock/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-17 10:06:38.560729 sql_mock-0.6.2/src/sql_mock/redshift/__init__.py
+-rw-r--r--   0        0        0     1384 2024-04-17 10:06:38.560729 sql_mock-0.6.2/src/sql_mock/redshift/column_mocks.py
+-rw-r--r--   0        0        0      266 2024-04-17 10:06:38.560729 sql_mock-0.6.2/src/sql_mock/redshift/settings.py
+-rw-r--r--   0        0        0      839 2024-04-17 10:06:38.560729 sql_mock-0.6.2/src/sql_mock/redshift/table_mocks.py
+-rw-r--r--   0        0        0        0 2024-04-17 10:06:38.560729 sql_mock-0.6.2/src/sql_mock/snowflake/__init__.py
+-rw-r--r--   0        0        0     1319 2024-04-17 10:06:38.560729 sql_mock-0.6.2/src/sql_mock/snowflake/column_mocks.py
+-rw-r--r--   0        0        0      225 2024-04-17 10:06:38.560729 sql_mock-0.6.2/src/sql_mock/snowflake/settings.py
+-rw-r--r--   0        0        0      734 2024-04-17 10:06:38.560729 sql_mock-0.6.2/src/sql_mock/snowflake/table_mocks.py
+-rw-r--r--   0        0        0    15214 2024-04-17 10:06:38.560729 sql_mock-0.6.2/src/sql_mock/table_mocks.py
+-rw-r--r--   0        0        0    12482 1970-01-01 00:00:00.000000 sql_mock-0.6.2/PKG-INFO
```

### Comparing `sql_mock-0.6.1/README.md` & `sql_mock-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `sql_mock-0.6.1/pyproject.toml` & `sql_mock-0.6.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "sql-mock"
-version = "0.6.1"
+version = "0.6.2"
 description = "Simplify the testing of SQL data models and queries by allowing users to mock input data and create tests for various scenarios. It provides a consistent and convenient way to test the execution of your query without the need to process a massive amount of data."
 repository = "https://github.com/DeepLcom/sql-mock"
 readme = "README.md"
 authors = ["DeepL SE", "Thomas Schmidt <thomas.heinz.schmidt@gmail.com>"]
 license = "MIT"
 
 classifiers = [
@@ -71,13 +71,16 @@
 isort = "^5.12.0"
 flake8 = "^6.1.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
-# Ignore Google Bigquery namespace deprecation warnings
 [tool.pytest.ini_options]
+# Ignore Google Bigquery namespace deprecation warnings
 filterwarnings = [
     "ignore:Deprecated call to `pkg_resources\\.declare_namespace\\('.*'\\):DeprecationWarning",
     "ignore::DeprecationWarning:google.rpc",
 ]
+markers = [
+    "integration: Integration tests requiring running database instances"
+]
```

### Comparing `sql_mock-0.6.1/src/sql_mock/bigquery/column_mocks.py` & `sql_mock-0.6.2/src/sql_mock/bigquery/column_mocks.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from typing import Any
+
 from sql_mock.column_mocks import BaseColumnMock
 
 
 class BigQueryColumnMock(BaseColumnMock):
     pass
 
 
 class Boolean(BigQueryColumnMock):
-    dtype = 'Boolean'
+    dtype = "Boolean"
 
 
 class Int(BigQueryColumnMock):
     dtype = "Integer"
 
 
 class Date(BigQueryColumnMock):
@@ -29,21 +30,21 @@
 class Decimal(BigQueryColumnMock):
     def __init__(self, default, precision, scale, nullable=False) -> None:
         self.dtype = f"Decimal({precision}, {scale})"
         super().__init__(default, nullable)
 
 
 class Timestamp(BigQueryColumnMock):
-    dtype = 'Timestamp'
+    dtype = "Timestamp"
 
 
 class Array(BigQueryColumnMock):
     use_quotes_for_casting = False
 
     def __init__(
         self,
         inner_type: BigQueryColumnMock,
         default: Any,
-        nullable: bool=False,
+        nullable: bool = False,
     ) -> None:
         self.dtype = f"Array<{inner_type.dtype}>"
         super().__init__(default, nullable)
```

### Comparing `sql_mock-0.6.1/src/sql_mock/bigquery/table_mocks.py` & `sql_mock-0.6.2/src/sql_mock/bigquery/table_mocks.py`

 * *Files identical despite different names*

### Comparing `sql_mock-0.6.1/src/sql_mock/clickhouse/column_mocks.py` & `sql_mock-0.6.2/src/sql_mock/clickhouse/column_mocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Any
+
 from sql_mock.column_mocks import BaseColumnMock
 
 
 class ClickhouseColumnMock(BaseColumnMock):
     def __init__(self, default, nullable=False) -> None:
         super().__init__(default, nullable)
         if nullable:
@@ -46,11 +47,11 @@
 class Array(ClickhouseColumnMock):
     use_quotes_for_casting = False
 
     def __init__(
         self,
         inner_type: ClickhouseColumnMock,
         default: Any,
-        nullable: bool=False,
+        nullable: bool = False,
     ) -> None:
         self.dtype = f"Array({inner_type.dtype})"
         super().__init__(default, nullable)
```

### Comparing `sql_mock-0.6.1/src/sql_mock/clickhouse/table_mocks.py` & `sql_mock-0.6.2/src/sql_mock/clickhouse/table_mocks.py`

 * *Files identical despite different names*

### Comparing `sql_mock-0.6.1/src/sql_mock/column_mocks.py` & `sql_mock-0.6.2/src/sql_mock/column_mocks.py`

 * *Files identical despite different names*

### Comparing `sql_mock-0.6.1/src/sql_mock/dbt.py` & `sql_mock-0.6.2/src/sql_mock/dbt.py`

 * *Files identical despite different names*

### Comparing `sql_mock-0.6.1/src/sql_mock/helpers.py` & `sql_mock-0.6.2/src/sql_mock/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,14 @@
         table_ref (str): Table ref to be replaced
         sql_mock_cte_name (str): Name of the CTE that will contain the mocked data
         dialect (str): The SQL dialect to use for parsing the query
     """
     query_ast = _replace_table_ref_in_columns(
         query_ast=query_ast, table_ref=table_ref, new_ref=sql_mock_cte_name, dialect=dialect
     )
-    print(query_ast.sql(pretty=True))
     return replace_tables(expression=query_ast, mapping={table_ref: sql_mock_cte_name}, dialect=dialect)
 
 
 def select_from_cte(query: str, cte_name: str, sql_dialect: str):
     """
     If selecting from a CTE, we need to replace the the final SELECT statement
     with a SELECT * FROM select_cte
```

### Comparing `sql_mock-0.6.1/src/sql_mock/redshift/column_mocks.py` & `sql_mock-0.6.2/src/sql_mock/redshift/column_mocks.py`

 * *Files identical despite different names*

### Comparing `sql_mock-0.6.1/src/sql_mock/redshift/table_mocks.py` & `sql_mock-0.6.2/src/sql_mock/redshift/table_mocks.py`

 * *Files identical despite different names*

### Comparing `sql_mock-0.6.1/src/sql_mock/snowflake/column_mocks.py` & `sql_mock-0.6.2/src/sql_mock/snowflake/column_mocks.py`

 * *Files identical despite different names*

### Comparing `sql_mock-0.6.1/src/sql_mock/snowflake/table_mocks.py` & `sql_mock-0.6.2/src/sql_mock/snowflake/table_mocks.py`

 * *Files identical despite different names*

### Comparing `sql_mock-0.6.1/src/sql_mock/table_mocks.py` & `sql_mock-0.6.2/src/sql_mock/table_mocks.py`

 * *Files identical despite different names*

### Comparing `sql_mock-0.6.1/PKG-INFO` & `sql_mock-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-mock
-Version: 0.6.1
+Version: 0.6.2
 Summary: Simplify the testing of SQL data models and queries by allowing users to mock input data and create tests for various scenarios. It provides a consistent and convenient way to test the execution of your query without the need to process a massive amount of data.
 Home-page: https://github.com/DeepLcom/sql-mock
 License: MIT
 Author: DeepL SE
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

