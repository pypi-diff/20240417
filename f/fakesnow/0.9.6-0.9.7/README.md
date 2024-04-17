# Comparing `tmp/fakesnow-0.9.6.tar.gz` & `tmp/fakesnow-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fakesnow-0.9.6.tar", last modified: Sun Mar 24 02:04:47 2024, max compression
+gzip compressed data, was "fakesnow-0.9.7.tar", last modified: Wed Apr 17 21:12:47 2024, max compression
```

## Comparing `fakesnow-0.9.6.tar` & `fakesnow-0.9.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 02:04:47.892158 fakesnow-0.9.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-03-24 02:04:40.000000 fakesnow-0.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17816 2024-03-24 02:04:47.892158 fakesnow-0.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-03-24 02:04:40.000000 fakesnow-0.9.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 02:04:47.884158 fakesnow-0.9.6/fakesnow/
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-03-24 02:04:40.000000 fakesnow-0.9.6/fakesnow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-24 02:04:40.000000 fakesnow-0.9.6/fakesnow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-03-24 02:04:40.000000 fakesnow-0.9.6/fakesnow/checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-03-24 02:04:40.000000 fakesnow-0.9.6/fakesnow/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-03-24 02:04:40.000000 fakesnow-0.9.6/fakesnow/expr.py
--rw-r--r--   0 runner    (1001) docker     (127)    28463 2024-03-24 02:04:40.000000 fakesnow-0.9.6/fakesnow/fakes.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-24 02:04:40.000000 fakesnow-0.9.6/fakesnow/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-03-24 02:04:40.000000 fakesnow-0.9.6/fakesnow/global_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-03-24 02:04:40.000000 fakesnow-0.9.6/fakesnow/info_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-24 02:04:40.000000 fakesnow-0.9.6/fakesnow/macros.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-24 02:04:40.000000 fakesnow-0.9.6/fakesnow/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    40109 2024-03-24 02:04:40.000000 fakesnow-0.9.6/fakesnow/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 02:04:47.888158 fakesnow-0.9.6/fakesnow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17816 2024-03-24 02:04:47.000000 fakesnow-0.9.6/fakesnow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-24 02:04:47.000000 fakesnow-0.9.6/fakesnow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 02:04:47.000000 fakesnow-0.9.6/fakesnow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-24 02:04:47.000000 fakesnow-0.9.6/fakesnow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-24 02:04:47.000000 fakesnow-0.9.6/fakesnow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-24 02:04:47.000000 fakesnow-0.9.6/fakesnow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-03-24 02:04:40.000000 fakesnow-0.9.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 02:04:47.892158 fakesnow-0.9.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 02:04:47.888158 fakesnow-0.9.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-03-24 02:04:40.000000 fakesnow-0.9.6/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-03-24 02:04:40.000000 fakesnow-0.9.6/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-03-24 02:04:40.000000 fakesnow-0.9.6/tests/test_expr.py
--rw-r--r--   0 runner    (1001) docker     (127)    58023 2024-03-24 02:04:40.000000 fakesnow-0.9.6/tests/test_fakes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-03-24 02:04:40.000000 fakesnow-0.9.6/tests/test_info_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-03-24 02:04:40.000000 fakesnow-0.9.6/tests/test_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-03-24 02:04:40.000000 fakesnow-0.9.6/tests/test_sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)    16020 2024-03-24 02:04:40.000000 fakesnow-0.9.6/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-24 02:04:40.000000 fakesnow-0.9.6/tests/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:12:47.081417 fakesnow-0.9.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-17 21:12:41.000000 fakesnow-0.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17845 2024-04-17 21:12:47.081417 fakesnow-0.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-17 21:12:41.000000 fakesnow-0.9.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:12:47.073417 fakesnow-0.9.7/fakesnow/
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-17 21:12:41.000000 fakesnow-0.9.7/fakesnow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-17 21:12:41.000000 fakesnow-0.9.7/fakesnow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-17 21:12:41.000000 fakesnow-0.9.7/fakesnow/checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-17 21:12:41.000000 fakesnow-0.9.7/fakesnow/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-17 21:12:41.000000 fakesnow-0.9.7/fakesnow/expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28929 2024-04-17 21:12:41.000000 fakesnow-0.9.7/fakesnow/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-17 21:12:41.000000 fakesnow-0.9.7/fakesnow/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-17 21:12:41.000000 fakesnow-0.9.7/fakesnow/global_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-04-17 21:12:41.000000 fakesnow-0.9.7/fakesnow/info_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-17 21:12:41.000000 fakesnow-0.9.7/fakesnow/macros.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-17 21:12:41.000000 fakesnow-0.9.7/fakesnow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    48818 2024-04-17 21:12:41.000000 fakesnow-0.9.7/fakesnow/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:12:47.077417 fakesnow-0.9.7/fakesnow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17845 2024-04-17 21:12:47.000000 fakesnow-0.9.7/fakesnow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-17 21:12:47.000000 fakesnow-0.9.7/fakesnow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 21:12:47.000000 fakesnow-0.9.7/fakesnow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-17 21:12:47.000000 fakesnow-0.9.7/fakesnow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-17 21:12:47.000000 fakesnow-0.9.7/fakesnow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 21:12:47.000000 fakesnow-0.9.7/fakesnow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-17 21:12:41.000000 fakesnow-0.9.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 21:12:47.081417 fakesnow-0.9.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:12:47.077417 fakesnow-0.9.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-17 21:12:41.000000 fakesnow-0.9.7/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-17 21:12:41.000000 fakesnow-0.9.7/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-17 21:12:41.000000 fakesnow-0.9.7/tests/test_expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66139 2024-04-17 21:12:41.000000 fakesnow-0.9.7/tests/test_fakes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-04-17 21:12:41.000000 fakesnow-0.9.7/tests/test_info_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-17 21:12:41.000000 fakesnow-0.9.7/tests/test_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-17 21:12:41.000000 fakesnow-0.9.7/tests/test_sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32132 2024-04-17 21:12:41.000000 fakesnow-0.9.7/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-17 21:12:41.000000 fakesnow-0.9.7/tests/test_users.py
```

### Comparing `fakesnow-0.9.6/LICENSE` & `fakesnow-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.6/PKG-INFO` & `fakesnow-0.9.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakesnow
-Version: 0.9.6
+Version: 0.9.7
 Summary: Fake Snowflake Connector for Python. Run, mock and test Snowflake DB locally.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -209,15 +209,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: duckdb~=0.10.0
 Requires-Dist: pyarrow
 Requires-Dist: snowflake-connector-python
-Requires-Dist: sqlglot~=21.2.0
+Requires-Dist: sqlglot~=23.3.0
 Provides-Extra: dev
 Requires-Dist: build~=1.0; extra == "dev"
 Requires-Dist: pandas-stubs; extra == "dev"
 Requires-Dist: snowflake-connector-python[pandas,secure-local-storage]; extra == "dev"
 Requires-Dist: pre-commit~=3.4; extra == "dev"
 Requires-Dist: pytest~=8.0; extra == "dev"
 Requires-Dist: ruff~=0.3.2; extra == "dev"
@@ -229,16 +229,15 @@
 Requires-Dist: jupysql; extra == "notebook"
 
 # fakesnow ❄️
 
 [![ci](https://github.com/tekumara/fakesnow/actions/workflows/ci.yml/badge.svg)](https://github.com/tekumara/fakesnow/actions/workflows/ci.yml)
 [![release](https://github.com/tekumara/fakesnow/actions/workflows/release.yml/badge.svg)](https://github.com/tekumara/fakesnow/actions/workflows/release.yml)
 [![PyPI](https://img.shields.io/pypi/v/fakesnow?color=violet)](https://pypi.org/project/fakesnow/)
-
-[![ci](../../actions/workflows/ci.yml/badge.svg)](../../actions/workflows/ci.yml)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/fakesnow?color=violet)](https://pypi.org/project/fakesnow/)
 
 Fake [Snowflake Connector for Python](https://docs.snowflake.com/en/user-guide/python-connector). Run and mock Snowflake DB locally.
 
 ## Install
 
 ```
 pip install fakesnow
```

### Comparing `fakesnow-0.9.6/README.md` & `fakesnow-0.9.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # fakesnow ❄️
 
 [![ci](https://github.com/tekumara/fakesnow/actions/workflows/ci.yml/badge.svg)](https://github.com/tekumara/fakesnow/actions/workflows/ci.yml)
 [![release](https://github.com/tekumara/fakesnow/actions/workflows/release.yml/badge.svg)](https://github.com/tekumara/fakesnow/actions/workflows/release.yml)
 [![PyPI](https://img.shields.io/pypi/v/fakesnow?color=violet)](https://pypi.org/project/fakesnow/)
-
-[![ci](../../actions/workflows/ci.yml/badge.svg)](../../actions/workflows/ci.yml)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/fakesnow?color=violet)](https://pypi.org/project/fakesnow/)
 
 Fake [Snowflake Connector for Python](https://docs.snowflake.com/en/user-guide/python-connector). Run and mock Snowflake DB locally.
 
 ## Install
 
 ```
 pip install fakesnow
```

### Comparing `fakesnow-0.9.6/fakesnow/__init__.py` & `fakesnow-0.9.7/fakesnow/__init__.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.6/fakesnow/checks.py` & `fakesnow-0.9.7/fakesnow/checks.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.6/fakesnow/cli.py` & `fakesnow-0.9.7/fakesnow/cli.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.6/fakesnow/expr.py` & `fakesnow-0.9.7/fakesnow/expr.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.6/fakesnow/fakes.py` & `fakesnow-0.9.7/fakesnow/fakes.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,45 +169,52 @@
             .transform(transforms.extract_comment_on_table)
             .transform(transforms.extract_comment_on_columns)
             .transform(transforms.information_schema_fs_columns_snowflake)
             .transform(transforms.information_schema_fs_tables_ext)
             .transform(transforms.drop_schema_cascade)
             .transform(transforms.tag)
             .transform(transforms.semi_structured_types)
-            .transform(transforms.parse_json)
+            .transform(transforms.try_parse_json)
             # indices_to_json_extract must be before regex_substr
             .transform(transforms.indices_to_json_extract)
             .transform(transforms.json_extract_cast_as_varchar)
             .transform(transforms.json_extract_cased_as_varchar)
             .transform(transforms.json_extract_precedence)
             .transform(transforms.flatten)
             .transform(transforms.regex_replace)
             .transform(transforms.regex_substr)
             .transform(transforms.values_columns)
             .transform(transforms.to_date)
             .transform(transforms.to_decimal)
+            .transform(transforms.try_to_decimal)
             .transform(transforms.to_timestamp_ntz)
             .transform(transforms.to_timestamp)
             .transform(transforms.object_construct)
             .transform(transforms.timestamp_ntz_ns)
             .transform(transforms.float_to_double)
             .transform(transforms.integer_precision)
             .transform(transforms.extract_text_length)
             .transform(transforms.sample)
             .transform(transforms.array_size)
             .transform(transforms.random)
             .transform(transforms.identifier)
+            .transform(transforms.array_agg_within_group)
+            .transform(transforms.array_agg_to_json)
+            .transform(transforms.dateadd_date_cast)
+            .transform(transforms.dateadd_string_literal_timestamp_cast)
+            .transform(transforms.datediff_string_literal_timestamp_cast)
             .transform(lambda e: transforms.show_schemas(e, self._conn.database))
             .transform(lambda e: transforms.show_objects_tables(e, self._conn.database))
             # TODO collapse into a single show_keys function
             .transform(lambda e: transforms.show_keys(e, self._conn.database, kind="PRIMARY"))
             .transform(lambda e: transforms.show_keys(e, self._conn.database, kind="UNIQUE"))
             .transform(lambda e: transforms.show_keys(e, self._conn.database, kind="FOREIGN"))
             .transform(transforms.show_users)
             .transform(transforms.create_user)
+            .transform(transforms.sha256)
         )
         sql = transformed.sql(dialect="duckdb")
         result_sql = None
 
         if transformed.find(exp.Select) and (seed := transformed.args.get("seed")):
             sql = f"SELECT setseed({seed}); {sql}"
 
@@ -613,15 +620,17 @@
         object_cols = df.select_dtypes(include=["object"]).columns
 
         # Apply json.dumps to these columns
         for col in object_cols:
             # don't jsonify string
             df[col] = df[col].apply(lambda x: json.dumps(x) if isinstance(x, (dict, list)) else x)
 
-        self._duck_conn.execute(f"INSERT INTO {table_name}({','.join(df.columns.to_list())}) SELECT * FROM df")
+        escaped_cols = ",".join(f'"{col}"' for col in df.columns.to_list())
+        self._duck_conn.execute(f"INSERT INTO {table_name}({escaped_cols}) SELECT * FROM df")
+
         return self._duck_conn.fetchall()[0][0]
 
 
 class FakeResultBatch(ResultBatch):
     def __init__(self, use_dict_result: bool, batch: pyarrow.RecordBatch):
         self._use_dict_result = use_dict_result
         self._batch = batch
```

### Comparing `fakesnow-0.9.6/fakesnow/global_database.py` & `fakesnow-0.9.7/fakesnow/global_database.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.6/fakesnow/info_schema.py` & `fakesnow-0.9.7/fakesnow/info_schema.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.6/fakesnow/transforms.py` & `fakesnow-0.9.7/fakesnow/transforms.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from pathlib import Path
 from string import Template
-from typing import Literal, cast
+from typing import ClassVar, Literal, cast
 
 import sqlglot
 from sqlglot import exp
 
 from fakesnow.global_database import USERS_TABLE_FQ_NAME
 
 MISSING_DATABASE = "missing_database"
@@ -18,14 +18,47 @@
         # case is used to convert 0 to null, because null is returned by duckdb when no case matches
         jal = exp.Anonymous(this="json_array_length", expressions=[expression.this])
         return exp.Case(ifs=[exp.If(this=jal, true=jal)])
 
     return expression
 
 
+def array_agg_to_json(expression: exp.Expression) -> exp.Expression:
+    if isinstance(expression, exp.ArrayAgg):
+        return exp.Anonymous(this="TO_JSON", expressions=[expression])
+
+    return expression
+
+
+def array_agg_within_group(expression: exp.Expression) -> exp.Expression:
+    """Convert ARRAY_AGG(<expr>) WITHIN GROUP (<order-by-clause>) to ARRAY_AGG( <expr> <order-by-clause> )
+    Snowflake uses ARRAY_AGG(<expr>) WITHIN GROUP (ORDER BY <order-by-clause>)
+    to order the array, but DuckDB uses ARRAY_AGG( <expr> <order-by-clause> ).
+    See;
+        - https://docs.snowflake.com/en/sql-reference/functions/array_agg
+        - https://duckdb.org/docs/sql/aggregates.html#order-by-clause-in-aggregate-functions
+    Note; Snowflake has following restriction;
+            If you specify DISTINCT and WITHIN GROUP, both must refer to the same column.
+          Transformation does not handle this restriction.
+    """
+    if (
+        isinstance(expression, exp.WithinGroup)
+        and (agg := expression.find(exp.ArrayAgg))
+        and (order := expression.expression)
+    ):
+        return exp.ArrayAgg(
+            this=exp.Order(
+                this=agg.this,
+                expressions=order.expressions,
+            )
+        )
+
+    return expression
+
+
 # TODO: move this into a Dialect as a transpilation
 def create_database(expression: exp.Expression, db_path: Path | None = None) -> exp.Expression:
     """Transform create database to attach database.
 
     Example:
         >>> import sqlglot
         >>> sqlglot.parse_one("CREATE database foo").transform(create_database).sql()
@@ -132,14 +165,106 @@
         return expression
 
     new = expression.copy()
     new.args["cascade"] = True
     return new
 
 
+def dateadd_date_cast(expression: exp.Expression) -> exp.Expression:
+    """Cast result of DATEADD to DATE if the given expression is a cast to DATE
+       and unit is either DAY, WEEK, MONTH or YEAR to mimic Snowflake's DATEADD
+       behaviour.
+
+    Snowflake;
+        SELECT DATEADD(DAY, 3, '2023-03-03'::DATE) as D;
+            D: 2023-03-06 (DATE)
+    DuckDB;
+        SELECT CAST('2023-03-03' AS DATE) + INTERVAL 3 DAY AS D
+            D: 2023-03-06 00:00:00 (TIMESTAMP)
+    """
+
+    if not isinstance(expression, exp.DateAdd):
+        return expression
+
+    if expression.unit is None:
+        return expression
+
+    if not isinstance(expression.unit.this, str):
+        return expression
+
+    if (unit := expression.unit.this.upper()) and unit.upper() not in {"DAY", "WEEK", "MONTH", "YEAR"}:
+        return expression
+
+    if not isinstance(expression.this, exp.Cast):
+        return expression
+
+    if expression.this.to.this != exp.DataType.Type.DATE:
+        return expression
+
+    return exp.Cast(
+        this=expression,
+        to=exp.DataType(this=exp.DataType.Type.DATE, nested=False, prefix=False),
+    )
+
+
+def dateadd_string_literal_timestamp_cast(expression: exp.Expression) -> exp.Expression:
+    """Snowflake's DATEADD function implicitly casts string literals to
+    timestamps regardless of unit.
+    """
+    if not isinstance(expression, exp.DateAdd):
+        return expression
+
+    if not isinstance(expression.this, exp.Literal) or not expression.this.is_string:
+        return expression
+
+    new_dateadd = expression.copy()
+    new_dateadd.set(
+        "this",
+        exp.Cast(
+            this=expression.this,
+            # TODO: support TIMESTAMP_TYPE_MAPPING of TIMESTAMP_LTZ/TZ
+            to=exp.DataType(this=exp.DataType.Type.TIMESTAMP, nested=False, prefix=False),
+        ),
+    )
+
+    return new_dateadd
+
+
+def datediff_string_literal_timestamp_cast(expression: exp.Expression) -> exp.Expression:
+    """Snowflake's DATEDIFF function implicitly casts string literals to
+    timestamps regardless of unit.
+    """
+
+    if not isinstance(expression, exp.DateDiff):
+        return expression
+
+    op1 = expression.this.copy()
+    op2 = expression.expression.copy()
+
+    if isinstance(op1, exp.Literal) and op1.is_string:
+        op1 = exp.Cast(
+            this=op1,
+            # TODO: support TIMESTAMP_TYPE_MAPPING of TIMESTAMP_LTZ/TZ
+            to=exp.DataType(this=exp.DataType.Type.TIMESTAMP, nested=False, prefix=False),
+        )
+
+    if isinstance(op2, exp.Literal) and op2.is_string:
+        op2 = exp.Cast(
+            this=op2,
+            # TODO: support TIMESTAMP_TYPE_MAPPING of TIMESTAMP_LTZ/TZ
+            to=exp.DataType(this=exp.DataType.Type.TIMESTAMP, nested=False, prefix=False),
+        )
+
+    new_datediff = expression.copy()
+    new_datediff.set("this", op1)
+    new_datediff.set("expression", op2)
+
+    return new_datediff
+
+
 def extract_comment_on_columns(expression: exp.Expression) -> exp.Expression:
     """Extract column comments, removing it from the Expression.
 
     duckdb doesn't support comments. So we remove them from the expression and store them in the column_comment arg.
     We also replace the transform the expression to NOP if the statement can't be executed by duckdb.
 
     Args:
@@ -504,46 +629,34 @@
 
     Internally snowflake stores OBJECT types as a json string, so the Duckdb JSON type most closely matches.
 
     See https://docs.snowflake.com/en/sql-reference/functions/object_construct
     """
 
     if isinstance(expression, exp.Struct):
-        # remove expressions containing NULL
-        for enull in expression.find_all(exp.Null):
-            if enull.parent:
-                enull.parent.pop()
-
-        return exp.Anonymous(this="TO_JSON", expressions=[expression])
-
-    return expression
-
-
-def parse_json(expression: exp.Expression) -> exp.Expression:
-    """Convert parse_json() to json().
-
-    Example:
-        >>> import sqlglot
-        >>> sqlglot.parse_one("insert into table1 (name) select parse_json('{}')").transform(parse_json).sql()
-        "CREATE TABLE table1 (name JSON)"
-    Args:
-        expression (exp.Expression): the expression that will be transformed.
-
-    Returns:
-        exp.Expression: The transformed expression.
-    """
-
-    if (
-        isinstance(expression, exp.Anonymous)
-        and isinstance(expression.this, str)
-        and expression.this.upper() == "PARSE_JSON"
-    ):
-        new = expression.copy()
-        new.args["this"] = "JSON"
-        return new
+        non_null_expressions = []
+        for e in expression.expressions:
+            if not (isinstance(e, exp.PropertyEQ)):
+                non_null_expressions.append(e)
+                continue
+
+            left = e.left
+            right = e.right
+
+            left_is_null = isinstance(left, exp.Null)
+            right_is_null = isinstance(right, exp.Null)
+
+            if left_is_null or right_is_null:
+                continue
+
+            non_null_expressions.append(e)
+
+        new_struct = expression.copy()
+        new_struct.set("expressions", non_null_expressions)
+        return exp.Anonymous(this="TO_JSON", expressions=[new_struct])
 
     return expression
 
 
 def regex_replace(expression: exp.Expression) -> exp.Expression:
     """Transform regex_replace expressions from snowflake to duckdb."""
 
@@ -825,38 +938,115 @@
         return exp.Cast(
             this=expression.expressions[0],
             to=exp.DataType(this=exp.DataType.Type.DATE, nested=False, prefix=False),
         )
     return expression
 
 
+def _get_to_number_args(e: exp.ToNumber) -> tuple[exp.Expression | None, exp.Expression | None, exp.Expression | None]:
+    arg_format = e.args.get("format")
+    arg_precision = e.args.get("precision")
+    arg_scale = e.args.get("scale")
+
+    _format = None
+    _precision = None
+    _scale = None
+
+    # to_number(value, <format>, <precision>, <scale>)
+    if arg_format:
+        if arg_format.is_string:
+            # to_number('100', 'TM9' ...)
+            _format = arg_format
+
+            # to_number('100', 'TM9', 10 ...)
+            if arg_precision:
+                _precision = arg_precision
+
+                # to_number('100', 'TM9', 10, 2)
+                if arg_scale:
+                    _scale = arg_scale
+            else:
+                pass
+        else:
+            # to_number('100', 10, ...)
+            # arg_format is not a string, so it must be precision.
+            _precision = arg_format
+
+            # to_number('100', 10, 2)
+            # And arg_precision must be scale
+            if arg_precision:
+                _scale = arg_precision
+    else:
+        # If format is not provided, just check for precision and scale directly
+        if arg_precision:
+            _precision = arg_precision
+            if arg_scale:
+                _scale = arg_scale
+
+    return _format, _precision, _scale
+
+
+def _to_decimal(expression: exp.Expression, cast_node: type[exp.Cast]) -> exp.Expression:
+    expressions: list[exp.Expression] = expression.expressions
+
+    if len(expressions) > 1 and expressions[1].is_string:
+        # see https://docs.snowflake.com/en/sql-reference/functions/to_decimal#arguments
+        raise NotImplementedError(f"{expression.this} with format argument")
+
+    precision = expressions[1] if len(expressions) > 1 else exp.Literal(this="38", is_string=False)
+    scale = expressions[2] if len(expressions) > 2 else exp.Literal(this="0", is_string=False)
+
+    return cast_node(
+        this=expressions[0],
+        to=exp.DataType(this=exp.DataType.Type.DECIMAL, expressions=[precision, scale], nested=False, prefix=False),
+    )
+
+
 def to_decimal(expression: exp.Expression) -> exp.Expression:
     """Transform to_decimal, to_number, to_numeric expressions from snowflake to duckdb.
 
     See https://docs.snowflake.com/en/sql-reference/functions/to_decimal
     """
 
+    if isinstance(expression, exp.ToNumber):
+        format_, precision, scale = _get_to_number_args(expression)
+        if format_:
+            raise NotImplementedError(f"{expression.this} with format argument")
+
+        if not precision:
+            precision = exp.Literal(this="38", is_string=False)
+        if not scale:
+            scale = exp.Literal(this="0", is_string=False)
+
+        return exp.Cast(
+            this=expression.this,
+            to=exp.DataType(this=exp.DataType.Type.DECIMAL, expressions=[precision, scale], nested=False, prefix=False),
+        )
+
     if (
         isinstance(expression, exp.Anonymous)
         and isinstance(expression.this, str)
-        and expression.this.upper() in ["TO_DECIMAL", "TO_NUMBER", "TO_NUMERIC"]
+        and expression.this.upper() in ["TO_DECIMAL", "TO_NUMERIC"]
     ):
-        expressions: list[exp.Expression] = expression.expressions
+        return _to_decimal(expression, exp.Cast)
 
-        if len(expressions) > 1 and expressions[1].is_string:
-            # see https://docs.snowflake.com/en/sql-reference/functions/to_decimal#arguments
-            raise NotImplementedError(f"{expression.this} with format argument")
+    return expression
 
-        precision = expressions[1] if len(expressions) > 1 else exp.Literal(this="38", is_string=False)
-        scale = expressions[2] if len(expressions) > 2 else exp.Literal(this="0", is_string=False)
 
-        return exp.Cast(
-            this=expressions[0],
-            to=exp.DataType(this=exp.DataType.Type.DECIMAL, expressions=[precision, scale], nested=False, prefix=False),
-        )
+def try_to_decimal(expression: exp.Expression) -> exp.Expression:
+    """Transform try_to_decimal, try_to_number, try_to_numeric expressions from snowflake to duckdb.
+    See https://docs.snowflake.com/en/sql-reference/functions/try_to_decimal
+    """
+
+    if (
+        isinstance(expression, exp.Anonymous)
+        and isinstance(expression.this, str)
+        and expression.this.upper() in ["TRY_TO_DECIMAL", "TRY_TO_NUMBER", "TRY_TO_NUMERIC"]
+    ):
+        return _to_decimal(expression, exp.TryCast)
 
     return expression
 
 
 def to_timestamp(expression: exp.Expression) -> exp.Expression:
     """Convert to_timestamp(seconds) to timestamp without timezone (ie: TIMESTAMP_NTZ).
 
@@ -901,14 +1091,42 @@
         new = expression.copy()
         del new.args["expressions"]
         return new
 
     return expression
 
 
+def try_parse_json(expression: exp.Expression) -> exp.Expression:
+    """Convert TRY_PARSE_JSON() to TRY_CAST(... as JSON).
+
+    Example:
+        >>> import sqlglot
+        >>> sqlglot.parse_one("select try_parse_json('{}')").transform(parse_json).sql()
+        "SELECT TRY_CAST('{}' AS JSON)"
+    Args:
+        expression (exp.Expression): the expression that will be transformed.
+
+    Returns:
+        exp.Expression: The transformed expression.
+    """
+
+    if (
+        isinstance(expression, exp.Anonymous)
+        and isinstance(expression.this, str)
+        and expression.this.upper() == "TRY_PARSE_JSON"
+    ):
+        expressions = expression.expressions
+        return exp.TryCast(
+            this=expressions[0],
+            to=exp.DataType(this=exp.DataType.Type.JSON, nested=False),
+        )
+
+    return expression
+
+
 # sqlglot.parse_one("create table example(date TIMESTAMP_NTZ(9));", read="snowflake")
 def semi_structured_types(expression: exp.Expression) -> exp.Expression:
     """Convert OBJECT, ARRAY, and VARIANT types to duckdb compatible types.
 
     Example:
         >>> import sqlglot
         >>> sqlglot.parse_one("CREATE TABLE table1 (name object)").transform(semi_structured_types).sql()
@@ -1083,7 +1301,52 @@
 
                 if schema:
                     statement += f"AND schema_name = '{schema}' "
             else:
                 raise NotImplementedError(f"SHOW PRIMARY KEYS with {scope_kind} not yet supported")
         return sqlglot.parse_one(statement)
     return expression
+
+
+class SHA256(exp.Func):
+    _sql_names: ClassVar = ["SHA256"]
+    arg_types: ClassVar = {"this": True}
+
+
+def sha256(expression: exp.Expression) -> exp.Expression:
+    """Convert sha2() or sha2_hex() to sha256().
+
+    Convert sha2_binary() to unhex(sha256()).
+
+    Example:
+        >>> import sqlglot
+        >>> sqlglot.parse_one("insert into table1 (name) select sha2('foo')").transform(sha256).sql()
+        "INSERT INTO table1 (name) SELECT SHA256('foo')"
+    Args:
+        expression (exp.Expression): the expression that will be transformed.
+
+    Returns:
+        exp.Expression: The transformed expression.
+    """
+
+    if isinstance(expression, exp.SHA2) and expression.args.get("length", exp.Literal.number(256)).this == "256":
+        return SHA256(this=expression.this)
+    elif (
+        isinstance(expression, exp.Anonymous)
+        and expression.this.upper() == "SHA2_HEX"
+        and (
+            len(expression.expressions) == 1
+            or (len(expression.expressions) == 2 and expression.expressions[1].this == "256")
+        )
+    ):
+        return SHA256(this=expression.expressions[0])
+    elif (
+        isinstance(expression, exp.Anonymous)
+        and expression.this.upper() == "SHA2_BINARY"
+        and (
+            len(expression.expressions) == 1
+            or (len(expression.expressions) == 2 and expression.expressions[1].this == "256")
+        )
+    ):
+        return exp.Unhex(this=SHA256(this=expression.expressions[0]))
+
+    return expression
```

### Comparing `fakesnow-0.9.6/fakesnow.egg-info/PKG-INFO` & `fakesnow-0.9.7/fakesnow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakesnow
-Version: 0.9.6
+Version: 0.9.7
 Summary: Fake Snowflake Connector for Python. Run, mock and test Snowflake DB locally.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -209,15 +209,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: duckdb~=0.10.0
 Requires-Dist: pyarrow
 Requires-Dist: snowflake-connector-python
-Requires-Dist: sqlglot~=21.2.0
+Requires-Dist: sqlglot~=23.3.0
 Provides-Extra: dev
 Requires-Dist: build~=1.0; extra == "dev"
 Requires-Dist: pandas-stubs; extra == "dev"
 Requires-Dist: snowflake-connector-python[pandas,secure-local-storage]; extra == "dev"
 Requires-Dist: pre-commit~=3.4; extra == "dev"
 Requires-Dist: pytest~=8.0; extra == "dev"
 Requires-Dist: ruff~=0.3.2; extra == "dev"
@@ -229,16 +229,15 @@
 Requires-Dist: jupysql; extra == "notebook"
 
 # fakesnow ❄️
 
 [![ci](https://github.com/tekumara/fakesnow/actions/workflows/ci.yml/badge.svg)](https://github.com/tekumara/fakesnow/actions/workflows/ci.yml)
 [![release](https://github.com/tekumara/fakesnow/actions/workflows/release.yml/badge.svg)](https://github.com/tekumara/fakesnow/actions/workflows/release.yml)
 [![PyPI](https://img.shields.io/pypi/v/fakesnow?color=violet)](https://pypi.org/project/fakesnow/)
-
-[![ci](../../actions/workflows/ci.yml/badge.svg)](../../actions/workflows/ci.yml)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/fakesnow?color=violet)](https://pypi.org/project/fakesnow/)
 
 Fake [Snowflake Connector for Python](https://docs.snowflake.com/en/user-guide/python-connector). Run and mock Snowflake DB locally.
 
 ## Install
 
 ```
 pip install fakesnow
```

### Comparing `fakesnow-0.9.6/fakesnow.egg-info/SOURCES.txt` & `fakesnow-0.9.7/fakesnow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.6/pyproject.toml` & `fakesnow-0.9.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 name = "fakesnow"
 description = "Fake Snowflake Connector for Python. Run, mock and test Snowflake DB locally."
-version = "0.9.6"
+version = "0.9.7"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = ["License :: OSI Approved :: MIT License"]
 keywords = ["snowflake", "snowflakedb", "fake", "local", "mock", "testing"]
 requires-python = ">=3.9"
 dependencies = [
     "duckdb~=0.10.0",
     "pyarrow",
     "snowflake-connector-python",
-    "sqlglot~=21.2.0",
+    "sqlglot~=23.3.0",
 ]
 
 [project.urls]
 homepage = "https://github.com/tekumara/fakesnow"
 
 [project.scripts]
 fakesnow = "fakesnow.cli:main"
```

### Comparing `fakesnow-0.9.6/tests/test_checks.py` & `fakesnow-0.9.7/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.6/tests/test_cli.py` & `fakesnow-0.9.7/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.6/tests/test_expr.py` & `fakesnow-0.9.7/tests/test_expr.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.6/tests/test_fakes.py` & `fakesnow-0.9.7/tests/test_fakes.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # ruff: noqa: E501
 # pyright: reportOptionalMemberAccess=false
 import datetime
 import json
 import tempfile
 from collections.abc import Sequence
 from decimal import Decimal
+from typing import cast
 
 import pandas as pd
 import pytest
 import pytz
 import snowflake.connector
 import snowflake.connector.cursor
 import snowflake.connector.pandas_tools
@@ -31,14 +32,54 @@
     assert cur.fetchall() == [(2,)]
 
     # when json is not an array
     cur.execute("""select array_size(parse_json('{"a":"b"}'))""")
     assert cur.fetchall() == [(None,)]
 
 
+def test_array_agg_to_json(dcur: snowflake.connector.cursor.DictCursor):
+    dcur.execute("create table table1 (id number, name varchar)")
+    values = [(1, "foo"), (2, "bar"), (1, "baz"), (2, "qux")]
+
+    dcur.executemany("insert into table1 values (%s, %s)", values)
+
+    dcur.execute("select array_agg(name) as names from table1")
+    assert dindent(dcur.fetchall()) == [{"NAMES": '[\n  "foo",\n  "bar",\n  "baz",\n  "qux"\n]'}]
+
+
+def test_array_agg_within_group(dcur: snowflake.connector.cursor.DictCursor):
+    dcur.execute("CREATE TABLE table1 (ID INT, amount INT)")
+
+    # two unique ids, for id 1 there are 3 amounts, for id 2 there are 2 amounts
+    values = [
+        (2, 40),
+        (1, 10),
+        (1, 30),
+        (2, 50),
+        (1, 20),
+    ]
+    dcur.executemany("INSERT INTO TABLE1 VALUES (%s, %s)", values)
+
+    dcur.execute("SELECT id, ARRAY_AGG(amount) WITHIN GROUP (ORDER BY amount DESC) amounts FROM table1 GROUP BY id")
+    rows = dcur.fetchall()
+
+    assert dindent(rows) == [
+        {"ID": 1, "AMOUNTS": "[\n  30,\n  20,\n  10\n]"},
+        {"ID": 2, "AMOUNTS": "[\n  50,\n  40\n]"},
+    ]
+
+    dcur.execute("SELECT id, ARRAY_AGG(amount) WITHIN GROUP (ORDER BY amount ASC) amounts FROM table1 GROUP BY id")
+    rows = dcur.fetchall()
+
+    assert dindent(rows) == [
+        {"ID": 1, "AMOUNTS": "[\n  10,\n  20,\n  30\n]"},
+        {"ID": 2, "AMOUNTS": "[\n  40,\n  50\n]"},
+    ]
+
+
 def test_binding_default_paramstyle(conn: snowflake.connector.SnowflakeConnection):
     assert snowflake.connector.paramstyle == "pyformat"
     with conn.cursor() as cur:
         cur.execute("create table customers (ID int, FIRST_NAME varchar, ACTIVE boolean)")
         cur.execute("insert into customers values (%s, %s, %s)", (1, "Jenny", True))
         cur.execute("select * from customers")
         assert cur.fetchall() == [(1, "Jenny", True)]
@@ -245,14 +286,99 @@
             in str(excinfo.value)
         )
 
         # schema still present on connection
         assert conn.schema == "JAFFLES"
 
 
+def test_dateadd_date_cast(dcur: snowflake.connector.DictCursor):
+    q = """
+    SELECT
+        dateadd(hour, 1, '2023-04-02'::date) as d_noop,
+        dateadd(day, 1, '2023-04-02'::date) as d_day,
+        dateadd(week, 1, '2023-04-02'::date) as d_week,
+        dateadd(month, 1, '2023-04-02'::date) as d_month,
+        dateadd(year, 1, '2023-04-02'::date) as d_year
+    """
+
+    dcur.execute(q)
+    assert dcur.fetchall() == [
+        {
+            "D_NOOP": datetime.datetime(2023, 4, 2, 1, 0),
+            "D_DAY": datetime.date(2023, 4, 3),
+            "D_WEEK": datetime.date(2023, 4, 9),
+            "D_MONTH": datetime.date(2023, 5, 2),
+            "D_YEAR": datetime.date(2024, 4, 2),
+        }
+    ]
+
+
+def test_dateadd_string_literal_timestamp_cast(dcur: snowflake.connector.cursor.DictCursor):
+    q = """
+    SELECT
+        DATEADD('MINUTE', 3, '2023-04-02') AS D_MINUTE,
+        DATEADD('HOUR', 3, '2023-04-02') AS D_HOUR,
+        DATEADD('DAY', 3, '2023-04-02') AS D_DAY,
+        DATEADD('WEEK', 3, '2023-04-02') AS D_WEEK,
+        DATEADD('MONTH', 3, '2023-04-02') AS D_MONTH,
+        DATEADD('YEAR', 3, '2023-04-02') AS D_YEAR
+    ;
+    """
+    dcur.execute(q)
+
+    assert dcur.fetchall() == [
+        {
+            "D_MINUTE": datetime.datetime(2023, 4, 2, 0, 3),
+            "D_HOUR": datetime.datetime(2023, 4, 2, 3, 0),
+            "D_DAY": datetime.datetime(2023, 4, 5, 0, 0),
+            "D_WEEK": datetime.datetime(2023, 4, 23, 0, 0),
+            "D_MONTH": datetime.datetime(2023, 7, 2, 0, 0),
+            "D_YEAR": datetime.datetime(2026, 4, 2, 0, 0),
+        }
+    ]
+
+    q = """
+    SELECT
+        DATEADD('MINUTE', 3, '2023-04-02 01:15:00') AS DT_MINUTE,
+        DATEADD('HOUR', 3, '2023-04-02 01:15:00') AS DT_HOUR,
+        DATEADD('DAY', 3, '2023-04-02 01:15:00') AS DT_DAY,
+        DATEADD('WEEK', 3, '2023-04-02 01:15:00') AS DT_WEEK,
+        DATEADD('MONTH', 3, '2023-04-02 01:15:00') AS DT_MONTH,
+        DATEADD('YEAR', 3, '2023-04-02 01:15:00') AS DT_YEAR
+    ;
+    """
+    dcur.execute(q)
+
+    assert dcur.fetchall() == [
+        {
+            "DT_MINUTE": datetime.datetime(2023, 4, 2, 1, 18),
+            "DT_HOUR": datetime.datetime(2023, 4, 2, 4, 15),
+            "DT_DAY": datetime.datetime(2023, 4, 5, 1, 15),
+            "DT_WEEK": datetime.datetime(2023, 4, 23, 1, 15),
+            "DT_MONTH": datetime.datetime(2023, 7, 2, 1, 15),
+            "DT_YEAR": datetime.datetime(2026, 4, 2, 1, 15),
+        }
+    ]
+
+
+def test_datediff_string_literal_timestamp_cast(cur: snowflake.connector.cursor.SnowflakeCursor):
+    cur.execute("SELECT DATEDIFF(DAY, '2023-04-02', '2023-03-02') AS D")
+    assert cur.fetchall() == [(-31,)]
+
+    cur.execute("SELECT DATEDIFF(HOUR, '2023-04-02', '2023-03-02') AS D")
+    assert cur.fetchall() == [(-744,)]
+
+    cur.execute("SELECT DATEDIFF(week, '2023-04-02', '2023-03-02') AS D")
+    assert cur.fetchall() == [(-4,)]
+
+    # noop
+    cur.execute("select '2023-04-02'::timestamp as c1, '2023-03-02'::timestamp as c2, DATEDIFF(minute, c1, c2) AS D")
+    assert cur.fetchall() == [(datetime.datetime(2023, 4, 2, 0, 0), datetime.datetime(2023, 3, 2, 0, 0), -44640)]
+
+
 def test_current_database_schema(conn: snowflake.connector.SnowflakeConnection):
     with conn.cursor(snowflake.connector.cursor.DictCursor) as cur:
         cur.execute("select current_database(), current_schema()")
 
         assert cur.fetchall() == [
             {"current_database()": "DB1", "current_schema()": "SCHEMA1"},
         ]
@@ -720,24 +846,52 @@
 
 
 def test_non_existent_table_throws_snowflake_exception(cur: snowflake.connector.cursor.SnowflakeCursor):
     with pytest.raises(snowflake.connector.errors.ProgrammingError) as _:
         cur.execute("select * from this_table_does_not_exist")
 
 
-def test_object_construct(cur: snowflake.connector.cursor.SnowflakeCursor):
-    cur.execute("SELECT OBJECT_CONSTRUCT('a',1,'b','BBBB', 'c',null)")
+def test_object_construct(conn: snowflake.connector.SnowflakeConnection):
+    with conn.cursor() as cur:
+        cur.execute("SELECT OBJECT_CONSTRUCT('a',1,'b','BBBB', 'c',null)")
+
+        # TODO: strip null within duckdb via python UDF
+        def strip_none_values(d: dict) -> dict:
+            return {k: v for k, v in d.items() if v}
+
+        result = cur.fetchone()
+        assert isinstance(result, tuple)
+        assert strip_none_values(json.loads(result[0])) == json.loads('{\n  "a": 1,\n  "b": "BBBB"\n}')
+
+    with conn.cursor() as cur:
+        cur.execute("SELECT OBJECT_CONSTRUCT('a', 1, null, 'nulkeyed') as col")
+
+        result = cur.fetchone()
+        assert isinstance(result, tuple)
+        assert strip_none_values(json.loads(result[0])) == json.loads('{\n  "a": 1\n}')
+
+    with conn.cursor() as cur:
+        cur.execute(
+            "SELECT NULL as col, OBJECT_CONSTRUCT( 'k1', 'v1', 'k2', CASE WHEN ZEROIFNULL(col) + 1 >= 2 THEN 'v2' ELSE NULL END, 'k3', 'v3')"
+        )
+
+        result = cur.fetchone()
+        assert isinstance(result, tuple)
+        assert strip_none_values(json.loads(result[1])) == json.loads('{\n  "k1": "v1",\n  "k3": "v3"\n}')
 
-    # TODO: strip null within duckdb via python UDF
-    def strip_none_values(d: dict) -> dict:
-        return {k: v for k, v in d.items() if v}
-
-    result = cur.fetchone()
-    assert isinstance(result, tuple)
-    assert strip_none_values(json.loads(result[0])) == json.loads('{\n  "a": 1,\n  "b": "BBBB"\n}')
+    with conn.cursor() as cur:
+        cur.execute(
+            "SELECT 1 as col, OBJECT_CONSTRUCT( 'k1', 'v1', 'k2', CASE WHEN ZEROIFNULL(col) + 1 >= 2 THEN 'v2' ELSE NULL END, 'k3', 'v3')"
+        )
+
+        result = cur.fetchone()
+        assert isinstance(result, tuple)
+        assert strip_none_values(json.loads(result[1])) == json.loads(
+            '{\n  "k1": "v1",\n  "k2": "v2",\n  "k3": "v3"\n}'
+        )
 
 
 def test_percentile_cont(conn: snowflake.connector.SnowflakeConnection):
     *_, cur = conn.execute_string(
         """
         create or replace table aggr(k int, v decimal(10,2));
         insert into aggr (k, v) values
@@ -1162,14 +1316,47 @@
 
     assert cur.fetchall() == [
         ("12.3456", 12, Decimal("12.3"), Decimal("12.34560000")),
         ("98.76546", 99, Decimal("98.8"), Decimal("98.76546000")),
     ]
 
 
+def test_sha2(cur: snowflake.connector.cursor.SnowflakeCursor):
+    # see https://docs.snowflake.com/en/sql-reference/functions/sha2#examples
+    cur.execute(
+        "select sha2('Snowflake') as a, sha2_hex('Snowflake') as b, sha2('Snowflake', 256) as c, sha2_hex('Snowflake', 256) as d;"
+    )
+
+    assert cur.fetchall() == [
+        ("1dbd59f661d68b90724f21084396b865497173e4d2714f4d91cf05fa5fc5e18d",) * 4,
+    ]
+
+
+def test_try_parse_json(dcur: snowflake.connector.cursor.DictCursor):
+    dcur.execute("""SELECT TRY_PARSE_JSON('{"first":"foo", "last":"bar"}') AS j""")
+    assert dindent(dcur.fetchall()) == [{"J": '{\n  "first": "foo",\n  "last": "bar"\n}'}]
+
+    dcur.execute("""SELECT TRY_PARSE_JSON('{invalid: ,]') AS j""")
+    assert dcur.fetchall() == [{"J": None}]
+
+
+def test_try_to_decimal(cur: snowflake.connector.cursor.SnowflakeCursor):
+    cur.execute(
+        "SELECT column1 AS orig_string, TRY_TO_DECIMAL(column1) AS dec, TRY_TO_DECIMAL(column1, 10, 2) AS dec_with_scale, TRY_TO_DECIMAL(column1, 4, 2) AS dec_with_range_err FROM VALUES ('345.123');"
+    )
+    assert cur.fetchall() == [
+        (
+            "345.123",
+            Decimal("345"),
+            Decimal("345.12"),
+            None,
+        ),
+    ]
+
+
 def test_transactions(conn: snowflake.connector.SnowflakeConnection):
     # test behaviours required for sqlalchemy
 
     conn.execute_string(
         """CREATE OR REPLACE TABLE table1 (i int);
             BEGIN TRANSACTION;
             INSERT INTO table1 (i) VALUES (1);"""
@@ -1259,14 +1446,34 @@
 
         assert cur.fetchall() == [
             {"COLUMN2": 1, "COLUMN1": "Amsterdam", "PJ": "[]"},
             {"COLUMN2": 2, "COLUMN1": "London", "PJ": "{}"},
         ]
 
 
+def test_write_pandas_quoted_column_names(conn: snowflake.connector.SnowflakeConnection):
+    with conn.cursor(snowflake.connector.cursor.DictCursor) as dcur:
+        # colunmn names with spaces
+        dcur.execute('create table customers (id int, "first name" varchar)')
+        df = pd.DataFrame.from_records(
+            [
+                {"ID": 1, "first name": "Jenny"},
+                {"ID": 2, "first name": "Jasper"},
+            ]
+        )
+        snowflake.connector.pandas_tools.write_pandas(conn, df, "CUSTOMERS")
+
+        dcur.execute("select * from customers")
+
+        assert dcur.fetchall() == [
+            {"ID": 1, "first name": "Jenny"},
+            {"ID": 2, "first name": "Jasper"},
+        ]
+
+
 def test_write_pandas_array(conn: snowflake.connector.SnowflakeConnection):
     with conn.cursor() as cur:
         cur.execute("create table customers (ID int, FIRST_NAME varchar, LAST_NAME varchar, ORDERS array)")
 
         df = pd.DataFrame.from_records(
             [
                 {"ID": 1, "FIRST_NAME": "Jenny", "LAST_NAME": "P", "ORDERS": ["A", "B"]},
@@ -1349,20 +1556,33 @@
 
         cur.execute("select * from customers")
 
         assert indent(cur.fetchall()) == [('{\n  "k": "v1"\n}',), ('{\n  "k2": [\n    "v\'2",\n    "v\\"3"\n  ]\n}',)]
 
 
 def indent(rows: Sequence[tuple] | Sequence[dict]) -> list[tuple]:
-    # indent duckdb json strings to match snowflake json strings
+    # indent duckdb json strings tuple values to match snowflake json strings
+    assert isinstance(rows[0], tuple)
     return [
         (*[json.dumps(json.loads(c), indent=2) if (isinstance(c, str) and c.startswith(("[", "{"))) else c for c in r],)
         for r in rows
     ]
 
 
+def dindent(rows: Sequence[tuple] | Sequence[dict]) -> list[dict]:
+    # indent duckdb json strings dict values to match snowflake json strings
+    assert isinstance(rows[0], dict)
+    return [
+        {
+            k: json.dumps(json.loads(v), indent=2) if (isinstance(v, str) and v.startswith(("[", "{"))) else v
+            for k, v in cast(dict, r).items()
+        }
+        for r in rows
+    ]
+
+
 def sort_keys(sdict: str, indent: int | None = 2) -> str:
     return json.dumps(
         json.loads(sdict, object_pairs_hook=lambda x: dict(sorted(x))),
         indent=indent,
         separators=None if indent else (",", ":"),
     )
```

### Comparing `fakesnow-0.9.6/tests/test_info_schema.py` & `fakesnow-0.9.7/tests/test_info_schema.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.6/tests/test_patch.py` & `fakesnow-0.9.7/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.6/tests/test_sqlalchemy.py` & `fakesnow-0.9.7/tests/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.9.6/tests/test_users.py` & `fakesnow-0.9.7/tests/test_users.py`

 * *Files identical despite different names*

