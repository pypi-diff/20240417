# Comparing `tmp/deltalake2db-0.3.0.tar.gz` & `tmp/deltalake2db-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltalake2db-0.3.0.tar", max compression
+gzip compressed data, was "deltalake2db-0.3.1.tar", max compression
```

## Comparing `deltalake2db-0.3.0.tar` & `deltalake2db-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2066 2024-04-16 08:56:26.257312 deltalake2db-0.3.0/README.md
--rw-r--r--   0        0        0      343 2024-04-16 08:56:26.257312 deltalake2db-0.3.0/deltalake2db/__init__.py
--rw-r--r--   0        0        0    14504 2024-04-16 08:56:26.257312 deltalake2db-0.3.0/deltalake2db/duckdb.py
--rw-r--r--   0        0        0      891 2024-04-16 08:56:26.257312 deltalake2db-0.3.0/deltalake2db/filter_by_meta.py
--rw-r--r--   0        0        0     5989 2024-04-16 08:56:26.257312 deltalake2db-0.3.0/deltalake2db/polars.py
--rw-r--r--   0        0        0      963 2024-04-16 08:56:26.257312 deltalake2db-0.3.0/deltalake2db/protocol_check.py
--rw-r--r--   0        0        0     2608 2024-04-16 08:56:26.257312 deltalake2db-0.3.0/deltalake2db/sql_utils.py
--rw-r--r--   0        0        0      697 2024-04-16 08:56:26.257312 deltalake2db-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2539 1970-01-01 00:00:00.000000 deltalake2db-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2066 2024-04-17 07:06:37.171103 deltalake2db-0.3.1/README.md
+-rw-r--r--   0        0        0      343 2024-04-17 07:06:37.171103 deltalake2db-0.3.1/deltalake2db/__init__.py
+-rw-r--r--   0        0        0    14504 2024-04-17 07:06:37.171103 deltalake2db-0.3.1/deltalake2db/duckdb.py
+-rw-r--r--   0        0        0      891 2024-04-17 07:06:37.171103 deltalake2db-0.3.1/deltalake2db/filter_by_meta.py
+-rw-r--r--   0        0        0     7383 2024-04-17 07:06:37.171103 deltalake2db-0.3.1/deltalake2db/polars.py
+-rw-r--r--   0        0        0      963 2024-04-17 07:06:37.175103 deltalake2db-0.3.1/deltalake2db/protocol_check.py
+-rw-r--r--   0        0        0     2608 2024-04-17 07:06:37.175103 deltalake2db-0.3.1/deltalake2db/sql_utils.py
+-rw-r--r--   0        0        0      725 2024-04-17 07:06:37.175103 deltalake2db-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2539 1970-01-01 00:00:00.000000 deltalake2db-0.3.1/PKG-INFO
```

### Comparing `deltalake2db-0.3.0/README.md` & `deltalake2db-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `deltalake2db-0.3.0/deltalake2db/duckdb.py` & `deltalake2db-0.3.1/deltalake2db/duckdb.py`

 * *Files identical despite different names*

### Comparing `deltalake2db-0.3.0/deltalake2db/filter_by_meta.py` & `deltalake2db-0.3.1/deltalake2db/filter_by_meta.py`

 * *Files identical despite different names*

### Comparing `deltalake2db-0.3.0/deltalake2db/polars.py` & `deltalake2db-0.3.1/deltalake2db/polars.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,63 +1,92 @@
 from pathlib import Path
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, cast
 
 from deltalake2db.filter_by_meta import _can_filter
 
 if TYPE_CHECKING:
     import polars as pl
 from deltalake import DeltaTable, Field, DataType
 from deltalake.exceptions import DeltaProtocolError
 from deltalake.schema import StructType, ArrayType, PrimitiveType, MapType
 import os
 
 
 def _get_expr(
-    base_expr: "pl.Expr|None", dtype: "DataType", meta: Field | None
+    base_expr: "pl.Expr|None",
+    dtype: "DataType",
+    meta: Field | None,
+    parquet_field: "pl.PolarsDataType | None",
 ) -> "pl.Expr":
     import polars as pl
 
+    if parquet_field is None:
+        return (
+            pl.lit(None, _get_type(dtype)).alias(meta.name)
+            if meta
+            else pl.lit(None, _get_type(dtype))
+        )
+
     pn = (
         meta.metadata.get("delta.columnMapping.physicalName", meta.name)
         if meta
         else None
     )
     if base_expr is None:
         assert pn is not None
         base_expr = pl.col(pn)
     if isinstance(dtype, StructType):
 
+        def _get_sub_type(name: str) -> "pl.PolarsDataType| None":
+            if parquet_field is None:
+                return None
+            assert isinstance(parquet_field, pl.Struct)
+            for f in parquet_field.fields:
+                if f.name == name:
+                    return f.dtype
+            return None
+
         struct_vl = (
             pl.when(base_expr.is_null())
             .then(pl.lit(None))
             .otherwise(
                 pl.struct(
                     *[
                         _get_expr(
                             base_expr.struct.field(
                                 subfield.metadata.get(
                                     "delta.columnMapping.physicalName", subfield.name
                                 )
                             ),
                             subfield.type,
                             subfield,
+                            _get_sub_type(
+                                subfield.metadata.get(
+                                    "delta.columnMapping.physicalName", subfield.name
+                                )
+                            ),
                         )
                         for subfield in dtype.fields
                     ]
                 )
             )
         )
         return struct_vl.alias(meta.name) if meta else struct_vl
     elif isinstance(dtype, ArrayType):
         list_vl = (
             pl.when(base_expr.is_null())
             .then(pl.lit(None))
             .otherwise(
                 base_expr.list.eval(
-                    _get_expr(pl.element(), dtype=dtype.element_type, meta=meta)
+                    _get_expr(
+                        pl.element(),
+                        dtype=dtype.element_type,
+                        meta=meta,
+                        parquet_field=cast(pl.List, parquet_field).inner,
+                    )
                 )
             )
         )
         return list_vl.alias(meta.name) if meta else list_vl
     return base_expr.alias(meta.name) if meta else base_expr
 
 
@@ -144,15 +173,26 @@
                 # as of delta 0.14
                 part_vl = ac["partition." + field.name]
                 selects.append(pl.lit(part_vl, pl_dtype).alias(field.name))
             elif (
                 field.metadata.get("delta.columnMapping.physicalName", field.name)
                 in parquet_schema
             ):
-                selects.append(_get_expr(None, field.type, field))
+                selects.append(
+                    _get_expr(
+                        None,
+                        field.type,
+                        field,
+                        parquet_schema.get(
+                            field.metadata.get(
+                                "delta.columnMapping.physicalName", field.name
+                            )
+                        ),
+                    )
+                )
             else:
                 selects.append(pl.lit(None, pl_dtype).alias(field.name))
         ds = (
             _filter_cond(base_ds.select(*selects), conditions)
             if conditions is not None
             else base_ds.select(*selects)
         )
```

### Comparing `deltalake2db-0.3.0/deltalake2db/protocol_check.py` & `deltalake2db-0.3.1/deltalake2db/protocol_check.py`

 * *Files identical despite different names*

### Comparing `deltalake2db-0.3.0/deltalake2db/sql_utils.py` & `deltalake2db-0.3.1/deltalake2db/sql_utils.py`

 * *Files identical despite different names*

### Comparing `deltalake2db-0.3.0/pyproject.toml` & `deltalake2db-0.3.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deltalake2db"
-version = "0.3.0"
+version = "0.3.1"
 description = ""
 authors = ["Adrian Ehrsam <adrian.ehrsam@bmsuisse.ch>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -22,11 +22,12 @@
 pytest = "^8.1.0"
 polars = "^0.20.13"
 duckdb = "^0.10.0"
 docker = "^7.0.0"
 azure-storage-blob = "^12.19.1"
 python-dotenv = "^1.0.1"
 pandas = "^2.2.1"
+azure-identity = "^1.16.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `deltalake2db-0.3.0/PKG-INFO` & `deltalake2db-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltalake2db
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 License: MIT
 Author: Adrian Ehrsam
 Author-email: adrian.ehrsam@bmsuisse.ch
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

