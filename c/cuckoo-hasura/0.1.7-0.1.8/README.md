# Comparing `tmp/cuckoo-hasura-0.1.7.tar.gz` & `tmp/cuckoo_hasura-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuckoo-hasura-0.1.7.tar", last modified: Thu Apr 11 16:38:47 2024, max compression
+gzip compressed data, was "cuckoo_hasura-0.1.8.tar", last modified: Wed Apr 17 19:21:55 2024, max compression
```

## Comparing `cuckoo-hasura-0.1.7.tar` & `cuckoo_hasura-0.1.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:38:47.518962 cuckoo-hasura-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    29627 2024-04-11 16:38:47.518962 cuckoo-hasura-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27567 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:38:47.510962 cuckoo-hasura-0.1.7/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/codegen/default_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/codegen/example_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7218 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/codegen/graphql_2_python.py
--rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/codegen/model_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:38:47.514962 cuckoo-hasura-0.1.7/cuckoo/
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10618 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/binary_tree_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    20580 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/finalizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/include.py
--rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/insert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:38:47.514962 cuckoo-hasura-0.1.7/cuckoo/models/
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/models/builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/models/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/models/providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9803 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)    16085 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     7720 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/root_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     9741 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/cuckoo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:38:47.518962 cuckoo-hasura-0.1.7/cuckoo_hasura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    29627 2024-04-11 16:38:47.000000 cuckoo-hasura-0.1.7/cuckoo_hasura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-11 16:38:47.000000 cuckoo-hasura-0.1.7/cuckoo_hasura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:38:47.000000 cuckoo-hasura-0.1.7/cuckoo_hasura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-11 16:38:47.000000 cuckoo-hasura-0.1.7/cuckoo_hasura.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-11 16:38:47.000000 cuckoo-hasura-0.1.7/cuckoo_hasura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 16:38:47.000000 cuckoo-hasura-0.1.7/cuckoo_hasura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 16:38:47.518962 cuckoo-hasura-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:38:47.518962 cuckoo-hasura-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/tests/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)    11413 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/tests/test_include.py
--rw-r--r--   0 runner    (1001) docker     (127)    11763 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/tests/test_insert.py
--rw-r--r--   0 runner    (1001) docker     (127)    14856 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/tests/test_mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)    34934 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    10001 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/tests/test_root_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    13633 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/tests/test_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-04-11 16:38:40.000000 cuckoo-hasura-0.1.7/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:21:55.056230 cuckoo_hasura-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    29653 2024-04-17 19:21:55.056230 cuckoo_hasura-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27567 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:21:55.052230 cuckoo_hasura-0.1.8/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/codegen/default_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/codegen/example_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7218 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/codegen/graphql_2_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/codegen/model_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:21:55.052230 cuckoo_hasura-0.1.8/cuckoo/
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10610 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/binary_tree_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20447 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/finalizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/include.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/insert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:21:55.052230 cuckoo_hasura-0.1.8/cuckoo/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/models/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/models/providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9788 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16454 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/root_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:21:55.056230 cuckoo_hasura-0.1.8/cuckoo_hasura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    29653 2024-04-17 19:21:55.000000 cuckoo_hasura-0.1.8/cuckoo_hasura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-17 19:21:55.000000 cuckoo_hasura-0.1.8/cuckoo_hasura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 19:21:55.000000 cuckoo_hasura-0.1.8/cuckoo_hasura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-17 19:21:55.000000 cuckoo_hasura-0.1.8/cuckoo_hasura.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-17 19:21:55.000000 cuckoo_hasura-0.1.8/cuckoo_hasura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 19:21:55.000000 cuckoo_hasura-0.1.8/cuckoo_hasura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 19:21:55.056230 cuckoo_hasura-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:21:55.056230 cuckoo_hasura-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/tests/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11413 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/tests/test_include.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11763 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/tests/test_insert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14856 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/tests/test_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35318 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10001 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/tests/test_root_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13633 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/tests/test_utils.py
```

### Comparing `cuckoo-hasura-0.1.7/LICENSE` & `cuckoo_hasura-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cuckoo-hasura-0.1.7/PKG-INFO` & `cuckoo_hasura-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuckoo-hasura
-Version: 0.1.7
+Version: 0.1.8
 Summary: An easy to use GraphQL query builder, optimized for Hasura.
 Author-email: Kenta Fried <kenta.fried@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Kenta Fried
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,14 +30,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx>=0.24.0
+Requires-Dist: ijson>=3.0
 Requires-Dist: orjson>=3.0.0
 Requires-Dist: pydantic<2.0.0,>=1.0.0
 Requires-Dist: tenacity>=8.0.0
 Provides-Extra: codegen
 Requires-Dist: case-converter>=1.1.0; extra == "codegen"
 Requires-Dist: graphql-core>=3.2.3; extra == "codegen"
```

### Comparing `cuckoo-hasura-0.1.7/README.md` & `cuckoo_hasura-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `cuckoo-hasura-0.1.7/codegen/default_config.py` & `cuckoo_hasura-0.1.8/codegen/default_config.py`

 * *Files identical despite different names*

### Comparing `cuckoo-hasura-0.1.7/codegen/example_config.py` & `cuckoo_hasura-0.1.8/codegen/example_config.py`

 * *Files identical despite different names*

### Comparing `cuckoo-hasura-0.1.7/codegen/graphql_2_python.py` & `cuckoo_hasura-0.1.8/codegen/graphql_2_python.py`

 * *Files identical despite different names*

### Comparing `cuckoo-hasura-0.1.7/codegen/model_module.py` & `cuckoo_hasura-0.1.8/codegen/model_module.py`

 * *Files identical despite different names*

### Comparing `cuckoo-hasura-0.1.7/cuckoo/__init__.py` & `cuckoo_hasura-0.1.8/cuckoo/__init__.py`

 * *Files identical despite different names*

### Comparing `cuckoo-hasura-0.1.7/cuckoo/binary_tree_node.py` & `cuckoo_hasura-0.1.8/cuckoo/binary_tree_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Generic,
     Optional,
     Type,
     TypeVar,
     Union,
 )
 
-from cuckoo.constants import ORDER_BY, WHERE
+from cuckoo.constants import DISTINCT_UPDATES, ORDER_BY, WHERE
 from cuckoo.models import TMODEL, TableModel
 from cuckoo.utils import BracketStyle, in_brackets
 
 if TYPE_CHECKING:
     from cuckoo.finalizers import AggregatesDict, CountDict
     from cuckoo.include import TCOLUMNS
     from cuckoo.root_node import HasuraClientError, RootNode
@@ -137,15 +137,15 @@
         inc: Optional[dict] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         on_conflict: Optional[dict[str, str]] = None,
         order_by: Optional[ORDER_BY] = None,
         pk_columns: Optional[dict] = None,
         prepend: Optional[dict] = None,
-        updates: Optional[list[dict]] = None,
+        updates: Optional[DISTINCT_UPDATES] = None,
         where_req: Optional[WHERE] = None,
         where: Optional[WHERE] = None,
         args: Optional[tuple[dict, str]] = None,  # (args_dict, function_name)
     ):
         table_name = self._node._get_table_name_by_model()
         fragments_by_arg = filter(
             lambda arg: arg[0] is not None,
@@ -227,15 +227,15 @@
     - `_bind_to_parent(parent)`: bind the node to another by setting the `_parent` and
         `_children` references in both nodes accordingly.
     - `_recurse(function)`: apply a function to each child node and append the result of
         each call to a resulting list of results.
     """
 
     def __init__(
-        self: BinaryTreeNode,
+        self,
         model: Type[TMODEL],
         parent: Optional[BinaryTreeNode] = None,
     ):
         super().__init__()
         self.model: Type[TMODEL] = model
         self._root: RootNode
         self._parent: BinaryTreeNode[TableModel]
@@ -245,15 +245,15 @@
         if parent:
             self._bind_to_parent(parent)
             self._table_name = self._get_table_name_by_model()
             self._query_alias = self._root._generate_var_name()
         else:
             self._root = self._parent = self  # make self a root node
 
-    def __str__(self: BinaryTreeNode):
+    def __str__(self):
         inner_args = self._fragments.inner_args
         return f"""
             {self._fragments.query_name}{
                 in_brackets(', '.join(inner_args), condition=bool(inner_args))
             } {{
                 {" ".join(str(rk) for rk in self._fragments.response_keys)}
             }}
```

### Comparing `cuckoo-hasura-0.1.7/cuckoo/constants.py` & `cuckoo_hasura-0.1.8/cuckoo/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -66,7 +66,15 @@
     "wait": wait_random_exponential(multiplier=1, max=60),
     "stop": stop_after_attempt(5),
 }
 
 WHERE: TypeAlias = dict[str, Any]
 ORDER_DIRECTION: TypeAlias = Union[Literal["asc"], Literal["desc"]]
 ORDER_BY: TypeAlias = dict[str, Union[ORDER_DIRECTION, "ORDER_BY"]]
+
+
+class UpdateManyDistinct(TypedDict):
+    _set: dict[str, Any]
+    where: WHERE
+
+
+DISTINCT_UPDATES: TypeAlias = list[UpdateManyDistinct]
```

### Comparing `cuckoo-hasura-0.1.7/cuckoo/delete.py` & `cuckoo_hasura-0.1.8/cuckoo/delete.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from __future__ import annotations
+
 from logging import Logger
 from typing import (
     Any,
     Generator,
     Generic,
     Optional,
     Type,
 )
 from uuid import UUID
 
 from httpx import AsyncClient, Client
 
-from cuckoo.root_node import BinaryTreeNode, RootNode
 from cuckoo.constants import WHERE, CuckooConfig
 from cuckoo.errors import RecordNotFoundError
 from cuckoo.finalizers import (
     TFIN_MANY,
     TFIN_ONE,
     AffectedRowsFinalizer,
     ReturningFinalizer,
     YieldingAffectedRowsFinalizer,
     YieldingFinalizer,
 )
 from cuckoo.models import TMODEL
 from cuckoo.mutation import MutationBase
+from cuckoo.root_node import BinaryTreeNode, RootNode
 
 
 class InnerDelete(
     BinaryTreeNode[TMODEL],
     Generic[TMODEL, TFIN_ONE, TFIN_MANY],
 ):
     def __init__(
@@ -37,15 +38,15 @@
         parent: Optional[BinaryTreeNode] = None,
         **kwargs,
     ):
         super().__init__(model=model, parent=parent, **kwargs)
         self._one_finalizer, self._many_finalizer = finalizers
 
     def one_by_pk(
-        self: InnerDelete,
+        self,
         uuid: UUID,
     ) -> TFIN_ONE:
         inner_delete = self._get_inner_delete()
         var_name = self._root._generate_var_name()
 
         inner_delete._fragments.query_name = (
             f"{inner_delete._query_alias}: delete_{inner_delete._table_name}_by_pk"
@@ -57,15 +58,15 @@
         return self._one_finalizer(
             node=inner_delete,
             returning_fn=inner_delete._build_one_model,
             gen_to_val={"returning": next},
         )
 
     def many(
-        self: InnerDelete,
+        self,
         where: WHERE,
     ) -> TFIN_MANY:
         inner_delete = self._get_inner_delete()
 
         inner_delete._fragments.query_name = (
             f"{inner_delete._query_alias}: delete_{inner_delete._table_name}"
         )
@@ -99,15 +100,15 @@
         for data in self._root._get_response(self._query_alias, "returning"):
             yield self.model(**data)
 
     def _get_rows(self):
         rows: int = self._root._get_response(self._query_alias, "affected_rows")
         yield rows
 
-    def _get_inner_delete(self: InnerDelete):
+    def _get_inner_delete(self):
         return (
             InnerDelete(
                 model=self.model,
                 parent=self,
                 finalizers=(self._one_finalizer, self._many_finalizer),
             )
             if isinstance(self, Delete)
```

### Comparing `cuckoo-hasura-0.1.7/cuckoo/encoders.py` & `cuckoo_hasura-0.1.8/cuckoo/encoders.py`

 * *Files identical despite different names*

### Comparing `cuckoo-hasura-0.1.7/cuckoo/finalizers.py` & `cuckoo_hasura-0.1.8/cuckoo/finalizers.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,17 +121,17 @@
             else:
                 raise ValueError(
                     "Elements in `returning` need to be of type `str` or "
                     "an instance of `Include`. "
                     f"Found type={type(str_or_constructor)}."
                 )
 
-    def _execute(self):
+    def _execute(self, stream=False):
         if not self._node._root._is_batch:
-            self._node._root._execute()
+            self._node._root._execute(stream=stream)
 
     async def _execute_async(self):
         if not self._node._root._is_batch:
             await self._node._root._execute_async()
 
 
 class AggregateBaseFinalizer(Finalizer):
@@ -185,56 +185,62 @@
 
 
 class YieldingFinalizer(
     ExecutingFinalizer,
     Generic[TYIELD],
 ):
     def __init__(
-        self: YieldingFinalizer,
+        self,
         node: BinaryTreeNode,
-        returning_fn: Callable[[], Generator[TYIELD, None, None]],
         gen_to_val: dict,
+        returning_fn: Optional[Callable[[], Generator[TYIELD, None, None]]] = None,
+        streaming_fn=None,
         response_key=ColumnResponseKey,
         **kwargs,
     ):
         super().__init__(node=node, **kwargs)
+        self._gen_to_val = gen_to_val
         self._returning_fn = returning_fn
+        self._streaming_fn = streaming_fn
         self._response_key = response_key
-        self._gen_to_val = gen_to_val
 
     def yielding(
-        self: YieldingFinalizer,
+        self,
         columns: Optional[TCOLUMNS] = None,
         *,
         invert_selection=False,
     ) -> Generator[TYIELD, None, None]:
         resolved_columns = self._resolve_column_selection(columns, invert_selection)
         self._node._fragments.response_keys.append(self._response_key(resolved_columns))
         ExecutingFinalizer._bind_includes(self._node)
-        self._execute()
 
-        return self._returning_fn()
+        if self._streaming_fn:
+            self._execute(stream=True)
+            return self._streaming_fn()
+        else:
+            self._execute()
+            return self._returning_fn()
 
 
 class ReturningFinalizer(
     YieldingFinalizer[TYIELD],
     Generic[TYIELD, TRETURN],
 ):
     def returning(
-        self: ReturningFinalizer,
+        self,
         columns: Optional[TCOLUMNS] = None,
         *,
         invert_selection=False,
     ) -> TRETURN:
         return self._gen_to_val["returning"](
             super().yielding(columns=columns, invert_selection=invert_selection)
         )
 
     async def returning_async(
-        self: ReturningFinalizer,
+        self,
         columns: Optional[TCOLUMNS] = None,
         *,
         invert_selection=False,
     ) -> TRETURN:
         resolved_columns = self._resolve_column_selection(columns, invert_selection)
         self._node._fragments.response_keys.append(self._response_key(resolved_columns))
         ExecutingFinalizer._bind_includes(self._node)
@@ -244,15 +250,15 @@
 
 
 class YieldingAffectedRowsFinalizer(
     YieldingFinalizer[TYIELD],
     Generic[TYIELD, TYIELD_WITH, TYIELD_ROWS],
 ):
     def __init__(
-        self: YieldingAffectedRowsFinalizer,
+        self,
         node: BinaryTreeNode,
         returning_fn: Callable[[], Generator[TYIELD, None, None]],
         affected_rows_fn: Callable[[], TYIELD_ROWS],
         returning_with_rows_fn: Callable[[], TYIELD_WITH],
         gen_to_val: dict,
     ):
         super().__init__(
@@ -261,23 +267,23 @@
             response_key=ReturningResponseKey,
             gen_to_val=gen_to_val,
         )
         self._affected_rows_fn = affected_rows_fn
         self._returning_with_rows_fn = returning_with_rows_fn
 
     def yield_affected_rows(
-        self: YieldingAffectedRowsFinalizer,
+        self,
     ) -> Generator[TYIELD_ROWS, None, None]:
         self._node._fragments.response_keys.append(AffectedRowsResponseKey())
         self._execute()
 
         return self._affected_rows_fn()
 
     def yielding_with_rows(
-        self: YieldingAffectedRowsFinalizer,
+        self,
         columns: Optional[TCOLUMNS] = None,
         *,
         invert_selection=False,
     ) -> TYIELD_WITH:
         resolved_columns = self._resolve_column_selection(columns, invert_selection)
         self._node._fragments.response_keys.extend(
             [
@@ -292,39 +298,37 @@
 
 
 class AffectedRowsFinalizer(
     ReturningFinalizer[TYIELD, TRETURN],
     YieldingAffectedRowsFinalizer[TYIELD, TYIELD_WITH, TYIELD_ROWS],
     Generic[TYIELD, TRETURN, TYIELD_WITH, TRETURN_WITH, TYIELD_ROWS, TRETURN_ROWS],
 ):
-    def affected_rows(self: AffectedRowsFinalizer) -> TRETURN_ROWS:
+    def affected_rows(self) -> TRETURN_ROWS:
         return self._gen_to_val["affected_rows"](super().yield_affected_rows())
 
-    async def affected_rows_async(
-        self: YieldingAffectedRowsFinalizer,
-    ) -> TRETURN_ROWS:
+    async def affected_rows_async(self) -> TRETURN_ROWS:
         self._node._fragments.response_keys.append(AffectedRowsResponseKey())
         await self._execute_async()
 
         return self._gen_to_val["affected_rows"](self._affected_rows_fn())
 
     def returning_with_rows(
-        self: AffectedRowsFinalizer,
+        self,
         columns: Optional[TCOLUMNS] = None,
         *,
         invert_selection=False,
     ) -> TRETURN_WITH:
         return self._gen_to_val["returning_with_rows"](
             super().yielding_with_rows(
                 columns=columns, invert_selection=invert_selection
             )
         )
 
     async def returning_with_rows_async(
-        self: YieldingAffectedRowsFinalizer,
+        self,
         columns: Optional[TCOLUMNS] = None,
         *,
         invert_selection=False,
     ) -> TRETURN_WITH:
         resolved_columns = self._resolve_column_selection(columns, invert_selection)
         self._node._fragments.response_keys.extend(
             [
@@ -340,15 +344,15 @@
 
 class YieldingAggregateFinalizer(
     ExecutingFinalizer,
     AggregateBaseFinalizer,
     Generic[TMODEL_BASE, TNUM_PROPS, TMODEL],
 ):
     def __init__(
-        self: YieldingAggregateFinalizer,
+        self,
         node: BinaryTreeNode,
         aggregate_fn: Callable[
             [], Generator[Aggregate[TMODEL_BASE, TNUM_PROPS], None, None]
         ],
         nodes_fn: Callable[[], Generator[TMODEL, None, None]],
         **kwargs,
     ):
@@ -356,15 +360,15 @@
             node=node,
             **kwargs,
         )
         self._aggregate_fn = aggregate_fn
         self._nodes_fn = nodes_fn
 
     def yield_on(
-        self: YieldingAggregateFinalizer,
+        self,
         *,
         count: Optional[Union[bool, CountDict]] = None,
         avg: Optional[set[str]] = None,
         max: Optional[set[str]] = None,
         min: Optional[set[str]] = None,
         stddev: Optional[set[str]] = None,
         stddev_pop: Optional[set[str]] = None,
@@ -392,15 +396,15 @@
             AggregateResponseKey(resolved_aggregates)
         )
         self._execute()
 
         return self._aggregate_fn()
 
     def yield_with_nodes(
-        self: YieldingAggregateFinalizer,
+        self,
         aggregates: AggregatesDict,
         columns: Optional[TCOLUMNS] = None,
         *,
         invert_selection=False,
     ) -> tuple[Generator[Aggregate, None, None], Generator[TMODEL, None, None]]:
         resolved_columns = self._resolve_column_selection(columns, invert_selection)
         resolved_aggregates = self._resolve_aggr_args(aggregates)
```

### Comparing `cuckoo-hasura-0.1.7/cuckoo/include.py` & `cuckoo_hasura-0.1.8/cuckoo/include.py`

 * *Files identical despite different names*

### Comparing `cuckoo-hasura-0.1.7/cuckoo/insert.py` & `cuckoo_hasura-0.1.8/cuckoo/insert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 from __future__ import annotations
+
 from logging import Logger
 from typing import (
     Any,
     Generator,
     Generic,
     Optional,
     Type,
     TypedDict,
 )
-from typing_extensions import NotRequired
 
 from httpx import AsyncClient, Client
+from typing_extensions import NotRequired
 
-from cuckoo.root_node import BinaryTreeNode, RootNode
 from cuckoo.constants import CuckooConfig
 from cuckoo.errors import InsertFailedError
 from cuckoo.finalizers import (
     TFIN_MANY,
     TFIN_ONE,
     AffectedRowsFinalizer,
     ReturningFinalizer,
     YieldingAffectedRowsFinalizer,
     YieldingFinalizer,
 )
 from cuckoo.models import TMODEL
 from cuckoo.mutation import MutationBase
+from cuckoo.root_node import BinaryTreeNode, RootNode
 
 
 class OnConflict(TypedDict):
     constraint: str
     update_columns: list[str]
     where: NotRequired[dict[str, Any]]
 
@@ -44,15 +45,15 @@
         parent: Optional[BinaryTreeNode] = None,
         **kwargs,
     ):
         super().__init__(model=model, parent=parent, **kwargs)
         self._one_finalizer, self._many_finalizer = finalizers
 
     def one(
-        self: InnerInsert,
+        self,
         data: dict[str, Any],
         on_conflict: Optional[OnConflict] = None,
     ) -> TFIN_ONE:
         object_var_name = self._root._generate_var_name()
         inner_insert = self._get_inner_insert()
         inner_insert._fragments.query_name = (
             f"{inner_insert._query_alias}:insert_{inner_insert._table_name}_one"
@@ -67,15 +68,15 @@
         return self._one_finalizer(
             node=inner_insert,
             returning_fn=inner_insert._build_one_model,
             gen_to_val={"returning": next},
         )
 
     def many(
-        self: InnerInsert,
+        self,
         data: list[dict[str, Any]],
         on_conflict: Optional[OnConflict] = None,
     ) -> TFIN_MANY:
         objects_var_name = self._root._generate_var_name()
         inner_insert = self._get_inner_insert()
         inner_insert._fragments.query_name = (
             f"{inner_insert._query_alias}:insert_{inner_insert._table_name}"
@@ -116,15 +117,15 @@
         for data in self._root._get_response(self._query_alias, "returning"):
             yield self.model(**data)
 
     def _get_rows(self) -> int:
         rows = self._root._get_response(self._query_alias, "affected_rows")
         yield rows
 
-    def _get_inner_insert(self: InnerInsert):
+    def _get_inner_insert(self):
         return (
             InnerInsert(
                 model=self.model,
                 parent=self,
                 finalizers=(self._one_finalizer, self._many_finalizer),
             )
             if isinstance(self, Insert)
```

### Comparing `cuckoo-hasura-0.1.7/cuckoo/models/__init__.py` & `cuckoo_hasura-0.1.8/cuckoo/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cuckoo-hasura-0.1.7/cuckoo/models/builtins.py` & `cuckoo_hasura-0.1.8/cuckoo/models/builtins.py`

 * *Files identical despite different names*

### Comparing `cuckoo-hasura-0.1.7/cuckoo/models/common.py` & `cuckoo_hasura-0.1.8/cuckoo/models/common.py`

 * *Files identical despite different names*

### Comparing `cuckoo-hasura-0.1.7/cuckoo/models/providers.py` & `cuckoo_hasura-0.1.8/cuckoo/models/providers.py`

 * *Files identical despite different names*

### Comparing `cuckoo-hasura-0.1.7/cuckoo/mutation.py` & `cuckoo_hasura-0.1.8/cuckoo/mutation.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
         return self._many_finalizer(
             node=inner_query,
             returning_fn=inner_query._build_many_models,
             gen_to_val={"returning": list},
         )
 
-    def _get_inner_mutation(self: InnerMutation):
+    def _get_inner_mutation(self):
         return (
             InnerMutation(
                 model=self.model,
                 parent=self,
                 finalizers=(
                     self._one_finalizer,
                     self._many_finalizer,
```

### Comparing `cuckoo-hasura-0.1.7/cuckoo/query.py` & `cuckoo_hasura-0.1.8/cuckoo/query.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     Generic,
     Optional,
     Type,
     cast,
 )
 from uuid import UUID
 
+import ijson
 from httpx import AsyncClient, Client
 
 from cuckoo.binary_tree_node import BinaryTreeNode
 from cuckoo.constants import ORDER_BY, WHERE, CuckooConfig
 from cuckoo.errors import RecordNotFoundError
 from cuckoo.finalizers import (
     TFIN_AGGR,
@@ -31,15 +32,15 @@
     TBATCHNUM_PROPS,
     TMODEL,
     TMODEL_BASE,
     TNUM_PROPS,
     Aggregate,
     UntypedModel,
 )
-from cuckoo.root_node import RootNode
+from cuckoo.root_node import IterByteIO, RootNode
 from cuckoo.utils import to_sql_function_args
 
 
 class InnerQuery(
     BinaryTreeNode[TMODEL],
     Generic[
         TMODEL,
@@ -168,15 +169,16 @@
             limit=limit,
             offset=offset,
             order_by=order_by,
         )
 
         return self._many_finalizer(
             node=inner_query,
-            returning_fn=inner_query._build_many_models,
+            streaming_fn=inner_query._build_many_models_stream,  # for `yielding` and `returning`
+            returning_fn=inner_query._build_many_models,  # for `returning_async` only
             gen_to_val={"returning": list},
         )
 
     def aggregate(
         self,
         *,
         where: Optional[WHERE] = None,
@@ -311,14 +313,21 @@
         yield self.model(**data)
 
     def _build_many_models(self):
         data_list: list[dict] = self._root._get_response(self._query_alias)
         for data in data_list:
             yield self.model(**data)
 
+    def _build_many_models_stream(self):
+        for item in ijson.items(
+            IterByteIO(self._root._response.iter_bytes()),
+            f"data.{self._query_alias}.item",
+        ):
+            yield self.model(**item)
+
     def _build_aggregate(self):
         response: dict[str, Any] = self._root._get_response(
             self._query_alias, "aggregate"
         )
 
         yield Aggregate[self._base_model, self._numeric_model](**response)
         # yield Aggregate[TMODEL_BASE, TNUM_PROPS](**response)
@@ -327,15 +336,15 @@
         data_list: list[dict[str, Any]] = self._root._get_response(
             self._query_alias, "nodes"
         )
 
         for data in data_list:
             yield self.model(**data)
 
-    def _get_inner_query(self: InnerQuery):
+    def _get_inner_query(self):
         return (
             InnerQuery(
                 model=self.model,
                 parent=self,
                 finalizers=(
                     self._one_by_pk_finalizer,
                     self._many_finalizer,
```

### Comparing `cuckoo-hasura-0.1.7/cuckoo/root_node.py` & `cuckoo_hasura-0.1.8/cuckoo/root_node.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,82 @@
 from __future__ import annotations
 
+from io import BytesIO
+from itertools import chain, islice
 from logging import Logger
 from types import GeneratorType
 from typing import (
     Any,
+    Iterable,
     Optional,
     Union,
 )
 
 import orjson
 from httpx import AsyncClient, Client, Response
 from pydantic import BaseModel
 from tenacity import AsyncRetrying, RetryError, Retrying
 
 from cuckoo.binary_tree_node import BinaryTreeNode
 from cuckoo.constants import HASURA_DEFAULT_CONFIG, RETRY_DEFAULT_CONFIG, CuckooConfig
 from cuckoo.encoders import jsonable_encoder
 from cuckoo.errors import HasuraClientError, HasuraServerError
 from cuckoo.models import TMODEL
-from cuckoo.utils import in_brackets, to_truncated_str
+from cuckoo.utils import in_brackets, to_compact_str, to_truncated_str
 
 
 class RootNode(BinaryTreeNode[TMODEL]):
     VAR_NAME_BASE = "var"
 
     def __init__(
-        self: RootNode,
+        self,
         config: Optional[CuckooConfig] = None,
         session: Optional[Client] = None,
         session_async: Optional[AsyncClient] = None,
         logger: Optional[Logger] = None,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self._config: CuckooConfig = {
             **HASURA_DEFAULT_CONFIG,  # type: ignore
             "retry": RETRY_DEFAULT_CONFIG,
             **(config if config else {}),
         }
-        self._session = session
-        self._session_async = session_async
         self._logger = logger
         self._var_name_counter: int = 0
+        self._response: Optional[Response] = None
         self._response_data: Optional[dict[str, Any]] = None
         self._is_batch = False
+
         self._close_session = False
+        if session is None:
+            self._close_session = True
+            self._session = Client(timeout=None)
+        else:
+            self._session = session
+
+        self._close_session_async = False
+        if session_async is None:
+            self._close_session_async = True
+            self._session_async = AsyncClient(timeout=None)
+        else:
+            self._session_async = session_async
 
-    def __str__(self: RootNode):
+    def __str__(self):
         outer_args = self._get_all_outer_args()
         return f"""
             {self._fragments.query_name}{
                 in_brackets(', '.join(outer_args), condition=bool(outer_args))
             } {{
                 {" ".join(str(child) for child in self._children)}
             }}
         """
 
     def _get_response(
-        self: RootNode,
+        self,
         query_alias: str,
         key: Optional[str] = None,
     ) -> Union[dict, list, int]:
         if self._response_data is None:
             raise HasuraClientError(
                 "Cannot access response data before calling `RootNode._make_request`"
             )
@@ -74,145 +89,118 @@
                     and isinstance(self._response_data[query_alias], dict)
                 )
                 else None
             )
         else:
             return self._response_data.pop(query_alias, None)
 
-    def _generate_var_name(self: RootNode):
+    def _generate_var_name(self):
         self._var_name_counter += 1
         return f"{self.VAR_NAME_BASE}{self._var_name_counter}"
 
-    def _compact(self: RootNode, gql_string: str):
-        return " ".join(gql_string.split())
-
-    def _get_or_create_session(self, use_async=False):
-        if use_async:
-            if self._session_async is None:
-                self._close_session = True
-                self._session_async = AsyncClient(timeout=None)
-            return self._session_async
-        else:
-            if self._session is None:
-                self._close_session = True
-                self._session = Client(timeout=None)
-            return self._session
-
-    def _process_response(
-        self,
-        response: Response,
-        query: str,
-        variables: dict,
-    ):
-        response.raise_for_status()
-        response_json: dict[str, Any] = response.json()
+    def _process_response(self):
+        response_json: dict[str, Any] = orjson.loads(self._response.content)
+        if self._logger:
+            response_text = to_truncated_str(self._response.text)
+            request_text = to_truncated_str(self._response.request.content.decode())
 
         if ("error" in response_json) or ("errors" in response_json):
             errors: list[dict[str, str]] = (
                 [response_json.get("error")] if "error" in response_json else []
             ) + response_json.get("errors", [])
             if self._logger:
                 self._logger.error(
-                    f"Query failed. query={self._compact(query)}, "
-                    f"variables={to_truncated_str(variables)}, response={str(errors)}."
+                    f"Query failed.  Request={request_text}, "
+                    f"response={response_text}, errors={str(errors)}."
                 )
             raise HasuraServerError(errors)
-
         elif "data" in response_json:
             if self._logger:
                 self._logger.debug(
-                    f"Query successful. query={self._compact(query)}, "
-                    f"variables={to_truncated_str(variables)}, "
-                    f"response={to_truncated_str(response_json['data'])}."
+                    f"Query successful. Request={request_text}, "
+                    f"response={response_text}."
                 )
-            return response_json["data"]
-
+            self._response_data = response_json["data"]
         else:
             raise NotImplementedError(
-                "response dict did not contain any errors nor data."
+                "Response did not contain any errors nor data. "
+                f"Response={self._response.text}."
             )
 
-    def _execute(self: RootNode):
-        query = str(self)
+    def _build_request(self):
+        query = to_compact_str(str(self))
         variables = self._get_all_variables()
-        json = {"query": self._compact(query)}
+        json = {"query": query}
         if variables:
             json["variables"] = RootNode._jsonify_variables(variables)
 
         if self._logger:
             self._logger.debug(
-                f"Executing query. query={self._compact(query)}, "
-                f"variables={to_truncated_str(variables)}."
+                f"Request created. {query=}, variables={to_truncated_str(variables)}."
             )
 
-        session = self._get_or_create_session()
+        return self._session.build_request(
+            method="POST",
+            url=self._config["url"],
+            headers=self._config["headers"],
+            json=json,
+        )
+
+    def _execute(self, stream=False):
+        request = self._build_request()
+        if self._logger:
+            if stream:
+                self._logger.debug("Dispatching http streaming request.")
+            else:
+                self._logger.debug("Dispatching http request.")
+
         try:
             for attempt in Retrying(**self._config["retry"]):
                 with attempt:
-                    response = session.post(
-                        url=self._config["url"],
-                        headers=self._config["headers"],
-                        json=json,
-                    )
+                    self._response = self._session.send(request=request, stream=stream)
+                    self._response.raise_for_status()
+                    if not stream:
+                        self._process_response()
         except RetryError as err:
             raise HasuraServerError(repr(err))
         finally:
             if self._close_session and self._session is not None:
                 self._session.close()
 
-        self._response_data = self._process_response(
-            response=response, query=query, variables=variables
-        )
-
     async def _execute_async(self):
-        query = str(self)
-        variables = self._get_all_variables()
-        json = {"query": self._compact(query)}
-        if variables:
-            json["variables"] = RootNode._jsonify_variables(variables)
-
+        request = self._build_request()
         if self._logger:
-            self._logger.debug(
-                f"Executing async query. query={self._compact(query)}, "
-                f"variables={to_truncated_str(variables)}."
-            )
+            self._logger.debug("Dispatching asynchronous http request.")
 
-        session = self._get_or_create_session(use_async=True)
         try:
             async for attempt in AsyncRetrying(**self._config["retry"]):
                 with attempt:
-                    response = await session.post(
-                        url=self._config["url"],
-                        headers=self._config["headers"],
-                        json=json,
-                    )
+                    self._response = await self._session_async.send(request=request)
+                    self._response.raise_for_status()
+                    self._process_response()
         except RetryError as err:
             raise HasuraServerError(repr(err))
         finally:
-            if self._close_session and self._session_async is not None:
+            if self._close_session_async and self._session_async is not None:
                 await self._session_async.aclose()
 
-        self._response_data = self._process_response(
-            response=response, query=query, variables=variables
-        )
-
     @staticmethod
     def _jsonify_variables(variables):
         return orjson.loads(orjson.dumps(variables, default=RootNode._orjson_default))
 
     def _get_all_variables(self):
         return {
             k: v
             for key_value_pairs in self._recurse(
                 lambda child: child._fragments.variables.items()
             )
             for k, v in key_value_pairs
         }
 
-    def _get_all_outer_args(self: RootNode):
+    def _get_all_outer_args(self):
         return [
             outer_arg_submodel
             for outer_args_submodel in self._recurse(
                 lambda node: node._fragments.outer_args
             )
             for outer_arg_submodel in outer_args_submodel
         ]
@@ -221,7 +209,37 @@
     def _orjson_default(obj):
         if isinstance(obj, (set, frozenset, GeneratorType)):
             return list(obj)
         elif isinstance(obj, BaseModel):
             return obj.dict()
         else:
             return jsonable_encoder(obj=obj)
+
+
+class IterByteIO(BytesIO):
+    """Convert an `Iterable[bytes]` into a file-like (read-only) object.
+
+    - uses `itertools.islice` internally to continuously read a chunk of bytes from the
+        generator. This is faster than using a `while` loop to fill the buffer, although
+        no performance testing has been conducted.
+
+    Note: Specifically intended to be used with the `ijson.items()` function that calls
+    the `read` and `readinto` methods only. Other use cases might call functions that
+    are not implemented here.
+
+    """
+
+    def __init__(self, iterable: Iterable[bytes]):
+        self.iter = chain.from_iterable(iterable)
+
+    def readable(self):
+        return True
+
+    def readinto(self, buffer: bytearray):
+        chunk = bytes(islice(self.iter, None, len(buffer)))
+        chunk_length = len(chunk)
+        buffer[:chunk_length] = chunk
+        return chunk_length
+
+    def read(self, chunk_size: Optional[int] = None):
+        chunk = islice(self.iter, None, chunk_size)
+        return bytes(chunk)
```

### Comparing `cuckoo-hasura-0.1.7/cuckoo/update.py` & `cuckoo_hasura-0.1.8/cuckoo/update.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 from __future__ import annotations
+
 from logging import Logger
 from typing import (
     Any,
     Generator,
     Generic,
     Optional,
     Type,
 )
 
 from httpx import AsyncClient, Client
 
-from cuckoo.root_node import BinaryTreeNode, RootNode
-from cuckoo.constants import WHERE, CuckooConfig
+from cuckoo.constants import DISTINCT_UPDATES, WHERE, CuckooConfig
+from cuckoo.errors import RecordNotFoundError
 from cuckoo.finalizers import (
     TFIN_MANY,
     TFIN_MANY_DISTINCT,
     TFIN_ONE,
     AffectedRowsFinalizer,
     ReturningFinalizer,
     YieldingAffectedRowsFinalizer,
     YieldingFinalizer,
 )
 from cuckoo.models import TMODEL
 from cuckoo.mutation import MutationBase
-from cuckoo.errors import RecordNotFoundError
+from cuckoo.root_node import BinaryTreeNode, RootNode
 
 
 class InnerUpdate(
     BinaryTreeNode[TMODEL],
     Generic[TMODEL, TFIN_ONE, TFIN_MANY, TFIN_MANY_DISTINCT],
 ):
     def __init__(
-        self: InnerUpdate,
+        self,
         model: Type[TMODEL],
         finalizers: tuple[Type[TFIN_ONE], Type[TFIN_MANY], Type[TFIN_MANY_DISTINCT]],
         parent: Optional[BinaryTreeNode] = None,
         **kwargs,
     ):
         super().__init__(model=model, parent=parent, **kwargs)
         (
             self._one_finalizer,
             self._many_finalizer,
             self._many_distinct_finalizer,
         ) = finalizers
 
     def one_by_pk(
-        self: InnerUpdate,
+        self,
         pk_columns: dict,
         data: Optional[dict] = None,
         inc: Optional[dict] = None,
         append: Optional[dict] = None,
         prepend: Optional[dict] = None,
         delete_key: Optional[dict] = None,
         delete_elem: Optional[dict] = None,
@@ -77,15 +78,15 @@
         return self._one_finalizer(
             node=inner_update,
             returning_fn=inner_update._build_one_model,
             gen_to_val={"returning": next},
         )
 
     def many(
-        self: InnerUpdate,
+        self,
         where: WHERE,
         data: Optional[dict] = None,
         inc: Optional[dict] = None,
         append: Optional[dict] = None,
         prepend: Optional[dict] = None,
         delete_key: Optional[dict] = None,
         delete_elem: Optional[dict] = None,
@@ -122,16 +123,16 @@
                 "returning": list,
                 "affected_rows": next,
                 "returning_with_rows": lambda tup: (list(tup[0]), next(tup[1])),
             },
         )
 
     def many_distinct(
-        self: InnerUpdate,
-        updates: list[dict],
+        self,
+        updates: DISTINCT_UPDATES,
     ) -> TFIN_MANY_DISTINCT:
         inner_update = self._get_inner_update()
         inner_update._fragments.query_name = (
             f"{inner_update._query_alias}:update_{inner_update._table_name}_many"
         )
         inner_update._fragments.build_from_conditionals(updates=updates)
 
@@ -176,30 +177,30 @@
         for data_list in self._root._get_response(self._query_alias):
             yield (self._build_model_from_list(data_list), data_list["affected_rows"])
 
     def _build_model_from_list(self, data_list: dict):
         for data in data_list["returning"]:
             yield self.model(**data)
 
-    def _get_inner_update(self: InnerUpdate):
+    def _get_inner_update(self):
         return (
             InnerUpdate(
                 model=self.model,
                 parent=self,
                 finalizers=(
                     self._one_finalizer,
                     self._many_finalizer,
                     self._many_distinct_finalizer,
                 ),
             )
             if isinstance(self, Update)
             else self
         )
 
-    def _assert_update_args(self: InnerUpdate, *args):
+    def _assert_update_args(self, *args):
         if not any([*args]):
             raise ValueError(
                 "Missing argument. At least one argument is required: data, inc, "
                 "prepend, append, delete_key, delete_elem, delete_at_path"
             )
```

### Comparing `cuckoo-hasura-0.1.7/cuckoo/utils.py` & `cuckoo_hasura-0.1.8/cuckoo/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from enum import Enum
 from itertools import zip_longest
 from types import GeneratorType
 from typing import Any, Generator, Iterable, TypeVar, Union
-import orjson
 
+import orjson
 from pydantic import BaseModel
 
 
 class BracketStyle(tuple, Enum):
     ROUND = ("(", ")")
     CURLY = ("{", "}")
     SQUARE = ("[", "]")
@@ -40,14 +40,18 @@
     num_chars = len(input_as_str)
     if num_chars > limit:
         return input_as_str[:limit] + "..."
     else:
         return input_as_str
 
 
+def to_compact_str(input_string: str):
+    return " ".join(input_string.split())
+
+
 T = TypeVar("T")
 
 
 def grouper(
     iterable: Iterable[T],
     group_size: int,
 ) -> Generator[tuple[T, ...], None, None]:
```

### Comparing `cuckoo-hasura-0.1.7/cuckoo_hasura.egg-info/PKG-INFO` & `cuckoo_hasura-0.1.8/cuckoo_hasura.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuckoo-hasura
-Version: 0.1.7
+Version: 0.1.8
 Summary: An easy to use GraphQL query builder, optimized for Hasura.
 Author-email: Kenta Fried <kenta.fried@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Kenta Fried
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,14 +30,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx>=0.24.0
+Requires-Dist: ijson>=3.0
 Requires-Dist: orjson>=3.0.0
 Requires-Dist: pydantic<2.0.0,>=1.0.0
 Requires-Dist: tenacity>=8.0.0
 Provides-Extra: codegen
 Requires-Dist: case-converter>=1.1.0; extra == "codegen"
 Requires-Dist: graphql-core>=3.2.3; extra == "codegen"
```

### Comparing `cuckoo-hasura-0.1.7/cuckoo_hasura.egg-info/SOURCES.txt` & `cuckoo_hasura-0.1.8/cuckoo_hasura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cuckoo-hasura-0.1.7/pyproject.toml` & `cuckoo_hasura-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cuckoo-hasura"
-version = "0.1.7"
+version = "0.1.8"
 description = "An easy to use GraphQL query builder, optimized for Hasura."
 readme = "README.md"
 requires-python = ">=3.9"
 license = { file = "LICENSE" }
 authors = [{ name = "Kenta Fried", email = "kenta.fried@gmail.com" }]
 keywords = []
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "httpx>=0.24.0",
+    "ijson>=3.0",
     "orjson>=3.0.0",
     "pydantic>=1.0.0,<2.0.0",
     "tenacity>=8.0.0",
 ]
 [project.urls]
 "Homepage" = "https://github.com/hotaru355/cuckoo-hasura"
 "Bug Tracker" = "https://github.com/hotaru355/cuckoo-hasura/issues"
```

### Comparing `cuckoo-hasura-0.1.7/tests/test_delete.py` & `cuckoo_hasura-0.1.8/tests/test_delete.py`

 * *Files identical despite different names*

### Comparing `cuckoo-hasura-0.1.7/tests/test_include.py` & `cuckoo_hasura-0.1.8/tests/test_include.py`

 * *Files identical despite different names*

### Comparing `cuckoo-hasura-0.1.7/tests/test_insert.py` & `cuckoo_hasura-0.1.8/tests/test_insert.py`

 * *Files identical despite different names*

### Comparing `cuckoo-hasura-0.1.7/tests/test_mutation.py` & `cuckoo_hasura-0.1.8/tests/test_mutation.py`

 * *Files identical despite different names*

### Comparing `cuckoo-hasura-0.1.7/tests/test_query.py` & `cuckoo_hasura-0.1.8/tests/test_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,18 +236,20 @@
                     rec.name == "test_logging"
                     and "Query successful." in rec.msg
                     and rec.levelname == "DEBUG"
                 ),
                 caplog.records,
             )
         )
-        assert record
-        assert "authors_by_pk" in record.msg
-        assert str(existing_uuid) in record.msg
-        assert f"{{'name': '{persisted_authors[0].name}'}}" in record.msg
+        assert record, "No debug log found containing 'Query successful.'"
+        assert "authors_by_pk" in record.msg, "Log does not contain query name."
+        assert str(existing_uuid) in record.msg, "Log does not contain query variable."
+        assert (
+            f'{{"name":"{persisted_authors[0].name}"}}' in record.msg
+        ), "Log does not contain query result."
 
     async def test_failed_query_gets_logged(
         self,
         finalize: FinalizeReturning[Query, Author],
         persisted_authors: list[Author],
         caplog: LogCaptureFixture,
         session: Client,
@@ -273,18 +275,20 @@
                     rec.name == "test_logging"
                     and "Query failed." in rec.msg
                     and rec.levelname == "ERROR"
                 ),
                 caplog.records,
             )
         )
-        assert record
-        assert "authors_by_pk" in record.msg
-        assert str(existing_uuid) in record.msg
-        assert "field 'does_not_exist' not found in type: 'authors'" in record.msg
+        assert record, "No error log found containing 'Query failed.'"
+        assert "authors_by_pk" in record.msg, "Log does not contain query name."
+        assert str(existing_uuid) in record.msg, "Log does not contain query variable."
+        assert (
+            "field 'does_not_exist' not found in type: 'authors'" in record.msg
+        ), "Log does not contain query error details."
 
 
 @mark.asyncio(scope="session")
 @mark.parametrize(**FinalizeParams(Query).returning_many())
 class TestMany:
     async def test_finding_all_records_with_default_column_if_no_condition_is_provided(
         self,
```

### Comparing `cuckoo-hasura-0.1.7/tests/test_root_node.py` & `cuckoo_hasura-0.1.8/tests/test_root_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,15 @@
     def test_default_config_stops_retrying_after_5_attempts(
         self,
         failing_session: MagicMock,
     ):
         with raises(HasuraServerError):
             Query(Author, session=failing_session).many(where={}).returning()
 
-        assert failing_session.post.call_count == 5
+        assert failing_session.send.call_count == 5
 
     def test_retry_config_can_be_changed(
         self,
         failing_session: MagicMock,
     ):
         with raises(HasuraServerError):
             Query(
@@ -161,15 +161,15 @@
                 config={
                     "retry": {
                         "stop": stop_after_attempt(3),
                     }
                 },
             ).many(where={}).returning()
 
-        assert failing_session.post.call_count == 3
+        assert failing_session.send.call_count == 3
 
     def test_default_session_gets_closed_for_successful_query(
         self,
         default_session_close: MagicMock,
     ):
         Query(Author).many(where={}).returning()
 
@@ -200,15 +200,15 @@
             Query(Author, session=failing_session).many(where={}).returning()
 
         failing_session.close.assert_not_called()
 
     @fixture
     def failing_session(self):
         mock = MagicMock(spec=Client)
-        mock.post.side_effect = [
+        mock.send.side_effect = [
             Exception("1"),
             Exception("2"),
             Exception("3"),
             Exception("4"),
             Exception("5"),
         ]
         return mock
@@ -238,15 +238,15 @@
         with raises(HasuraServerError):
             await (
                 Query(Author, session_async=failing_session)
                 .many(where={})
                 .returning_async()
             )
 
-        assert failing_session.post.call_count == 5
+        assert failing_session.send.call_count == 5
 
     async def test_retry_config_can_be_changed(
         self,
         failing_session: MagicMock,
     ):
         with raises(HasuraServerError):
             await (
@@ -259,15 +259,15 @@
                         }
                     },
                 )
                 .many(where={})
                 .returning_async()
             )
 
-        assert failing_session.post.call_count == 3
+        assert failing_session.send.call_count == 3
 
     async def test_default_session_gets_closed_for_successful_query(
         self,
         default_session_close: MagicMock,
     ):
         await Query(Author).many(where={}).returning_async()
 
@@ -304,15 +304,15 @@
             )
 
         failing_session.aclose.assert_not_called()
 
     @fixture
     def failing_session(self):
         mock = MagicMock(spec=AsyncClient)
-        mock.post.side_effect = [
+        mock.send.side_effect = [
             Exception("1"),
             Exception("2"),
             Exception("3"),
             Exception("4"),
             Exception("5"),
         ]
         return mock
```

### Comparing `cuckoo-hasura-0.1.7/tests/test_update.py` & `cuckoo_hasura-0.1.8/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `cuckoo-hasura-0.1.7/tests/test_utils.py` & `cuckoo_hasura-0.1.8/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,37 @@
 from typing import Generator
 
 from geojson_pydantic import Point
 from pytest import mark, raises
 
-from cuckoo.utils import Prop, grouper, to_sql_function_args, to_truncated_str
+from cuckoo.utils import (
+    Prop,
+    grouper,
+    to_compact_str,
+    to_sql_function_args,
+    to_truncated_str,
+)
+
+
+class TestToCompactStr:
+    def test_removes_extra_whitespaces(self):
+        input_str = " \n \t \r ABC DEF \n \t \r GHI \n \t \r "
+        expected = "ABC DEF GHI"
+
+        actual = to_compact_str(input_str)
+
+        assert actual == expected
+
+    def test_does_not_remove_any_non_consecutive_whitespaces(self):
+        input_str = "ABC DEF\nGHI\tJKL"
+        expected = "ABC DEF GHI JKL"
+
+        actual = to_compact_str(input_str)
+
+        assert actual == expected
 
 
 class TestToTruncatedStr:
     def test_string_longer_than_limit_gets_truncated(self):
         test_input = "A" * 2000
         expected = "A" * 1000 + "..."
```

