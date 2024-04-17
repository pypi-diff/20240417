# Comparing `tmp/rush_py-3.0.0.tar.gz` & `tmp/rush_py-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rush_py-3.0.0.tar", max compression
+gzip compressed data, was "rush_py-3.0.1.tar", max compression
```

## Comparing `rush_py-3.0.0.tar` & `rush_py-3.0.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0     9914 2024-04-12 09:38:51.148131 rush_py-3.0.0/README.md
--rw-r--r--   0        0        0     2718 2024-04-12 08:49:08.158655 rush_py-3.0.0/pyproject.toml
--rw-r--r--   0        0        0      481 2024-03-25 07:43:11.134075 rush_py-3.0.0/rush/__init__.py
--rw-r--r--   0        0        0     1569 2024-04-12 08:48:59.531260 rush_py-3.0.0/rush/async_utils.py
--rw-r--r--   0        0        0       23 2024-01-29 10:45:57.136914 rush_py-3.0.0/rush/data.py
--rw-r--r--   0        0        0     1326 2024-03-25 07:43:11.134075 rush_py-3.0.0/rush/doc.py
--rw-r--r--   0        0        0     7663 2024-04-12 08:48:59.531260 rush_py-3.0.0/rush/graphql_client/__init__.py
--rw-r--r--   0        0        0      267 2024-04-12 08:48:59.531260 rush_py-3.0.0/rush/graphql_client/argument.py
--rw-r--r--   0        0        0     1036 2024-04-12 08:48:59.532260 rush_py-3.0.0/rush/graphql_client/arguments.py
--rw-r--r--   0        0        0    12272 2024-04-07 11:13:59.841910 rush_py-3.0.0/rush/graphql_client/async_base_client.py
--rw-r--r--   0        0        0      620 2024-04-07 11:51:36.271482 rush_py-3.0.0/rush/graphql_client/base_model.py
--rw-r--r--   0        0        0      174 2024-04-07 11:13:28.065432 rush_py-3.0.0/rush/graphql_client/cancel_module_instance.py
--rw-r--r--   0        0        0    28860 2024-04-12 08:48:59.532260 rush_py-3.0.0/rush/graphql_client/client.py
--rw-r--r--   0        0        0      253 2024-02-28 07:01:47.459725 rush_py-3.0.0/rush/graphql_client/create_entity.py
--rw-r--r--   0        0        0      277 2024-02-28 07:01:47.461725 rush_py-3.0.0/rush/graphql_client/create_experiment.py
--rw-r--r--   0        0        0      259 2024-02-28 07:01:47.463725 rush_py-3.0.0/rush/graphql_client/create_project.py
--rw-r--r--   0        0        0      259 2024-02-28 07:01:47.467725 rush_py-3.0.0/rush/graphql_client/create_protein.py
--rw-r--r--   0        0        0      314 2024-02-28 07:01:47.465725 rush_py-3.0.0/rush/graphql_client/create_protein_conformer.py
--rw-r--r--   0        0        0      241 2024-02-28 07:01:47.566729 rush_py-3.0.0/rush/graphql_client/create_smol.py
--rw-r--r--   0        0        0      296 2024-02-28 07:01:47.564729 rush_py-3.0.0/rush/graphql_client/create_smol_conformer.py
--rw-r--r--   0        0        0      290 2024-02-28 07:01:47.568729 rush_py-3.0.0/rush/graphql_client/create_smol_tautomer.py
--rw-r--r--   0        0        0      271 2024-02-28 07:01:47.570730 rush_py-3.0.0/rush/graphql_client/create_structure.py
--rw-r--r--   0        0        0      341 2024-04-12 08:48:59.532260 rush_py-3.0.0/rush/graphql_client/delete_module_instance.py
--rw-r--r--   0        0        0      255 2024-04-12 08:48:59.533260 rush_py-3.0.0/rush/graphql_client/deploy.py
--rw-r--r--   0        0        0      510 2024-02-28 07:01:47.506727 rush_py-3.0.0/rush/graphql_client/entity.py
--rw-r--r--   0        0        0     1491 2024-04-12 08:48:59.533260 rush_py-3.0.0/rush/graphql_client/enums.py
--rw-r--r--   0        0        0     2411 2024-04-07 11:13:28.519453 rush_py-3.0.0/rush/graphql_client/exceptions.py
--rw-r--r--   0        0        0      679 2024-02-28 07:01:47.557729 rush_py-3.0.0/rush/graphql_client/experiment.py
--rw-r--r--   0        0        0     3769 2024-04-12 08:48:59.533260 rush_py-3.0.0/rush/graphql_client/fragments.py
--rw-r--r--   0        0        0     5332 2024-04-12 08:48:59.533260 rush_py-3.0.0/rush/graphql_client/input_types.py
--rw-r--r--   0        0        0      825 2024-04-12 08:48:59.534260 rush_py-3.0.0/rush/graphql_client/latest_modules.py
--rw-r--r--   0        0        0     2004 2024-04-12 08:48:59.534260 rush_py-3.0.0/rush/graphql_client/module_instance_details.py
--rw-r--r--   0        0        0     4300 2024-01-29 10:45:57.143915 rush_py-3.0.0/rush/graphql_client/module_instance_full.py
--rw-r--r--   0        0        0      354 2024-04-12 08:48:59.534260 rush_py-3.0.0/rush/graphql_client/module_instance_minimal.py
--rw-r--r--   0        0        0      403 2024-01-29 10:45:57.144914 rush_py-3.0.0/rush/graphql_client/module_instance_status.py
--rw-r--r--   0        0        0     3104 2024-04-12 08:48:59.534260 rush_py-3.0.0/rush/graphql_client/module_instances.py
--rw-r--r--   0        0        0     2804 2024-01-29 10:45:57.145915 rush_py-3.0.0/rush/graphql_client/module_instances_full.py
--rw-r--r--   0        0        0      686 2024-04-12 08:48:59.534260 rush_py-3.0.0/rush/graphql_client/modules.py
--rw-r--r--   0        0        0      160 2024-02-13 05:21:55.039019 rush_py-3.0.0/rush/graphql_client/object.py
--rw-r--r--   0        0        0      292 2024-04-12 08:48:59.535260 rush_py-3.0.0/rush/graphql_client/object_contents.py
--rw-r--r--   0        0        0      243 2024-04-12 08:48:59.535260 rush_py-3.0.0/rush/graphql_client/object_url.py
--rw-r--r--   0        0        0     2121 2024-02-28 07:01:47.518727 rush_py-3.0.0/rush/graphql_client/project.py
--rw-r--r--   0        0        0      604 2024-02-28 07:01:47.523728 rush_py-3.0.0/rush/graphql_client/protein.py
--rw-r--r--   0        0        0      687 2024-02-28 07:01:47.528728 rush_py-3.0.0/rush/graphql_client/protein_conformer.py
--rw-r--r--   0        0        0      234 2024-04-12 08:48:59.535260 rush_py-3.0.0/rush/graphql_client/retry.py
--rw-r--r--   0        0        0      340 2024-04-12 08:48:59.535260 rush_py-3.0.0/rush/graphql_client/run.py
--rw-r--r--   0        0        0      571 2024-02-28 07:01:47.533728 rush_py-3.0.0/rush/graphql_client/smol.py
--rw-r--r--   0        0        0      657 2024-02-28 07:01:47.537728 rush_py-3.0.0/rush/graphql_client/smol_conformer.py
--rw-r--r--   0        0        0      662 2024-02-28 07:01:47.543728 rush_py-3.0.0/rush/graphql_client/smol_tautomer.py
--rw-r--r--   0        0        0     1139 2024-02-28 07:01:47.551729 rush_py-3.0.0/rush/graphql_client/structure.py
--rw-r--r--   0        0        0      161 2024-04-07 11:13:28.358446 rush_py-3.0.0/rush/graphql_client/tag.py
--rw-r--r--   0        0        0      381 2024-04-12 08:48:59.535260 rush_py-3.0.0/rush/graphql_client/track_utilization.py
--rw-r--r--   0        0        0      165 2024-04-07 11:13:28.369446 rush_py-3.0.0/rush/graphql_client/untag.py
--rw-r--r--   0        0        0      414 2024-04-12 08:48:59.536260 rush_py-3.0.0/rush/graphql_client/update_module_instance.py
--rw-r--r--   0        0        0      328 2024-01-29 10:45:57.148915 rush_py-3.0.0/rush/graphql_client/upload.py
--rw-r--r--   0        0        0      321 2024-04-12 08:48:59.536260 rush_py-3.0.0/rush/graphql_client/upload_arg.py
--rw-r--r--   0        0        0      506 2024-04-12 08:48:59.536260 rush_py-3.0.0/rush/graphql_client/upload_object.py
--rw-r--r--   0        0        0     1226 2024-03-25 07:43:11.134075 rush_py-3.0.0/rush/legacy_types.py
--rw-r--r--   0        0        0     7403 2024-02-16 09:06:54.345722 rush_py-3.0.0/rush/local.py
--rw-r--r--   0        0        0     5733 2024-02-16 09:06:54.345722 rush_py-3.0.0/rush/protocols.py
--rw-r--r--   0        0        0    65171 2024-04-12 08:48:59.536260 rush_py-3.0.0/rush/provider.py
--rw-r--r--   0        0        0       98 2024-02-16 09:06:54.345722 rush_py-3.0.0/rush/tests/test_provider.py
--rw-r--r--   0        0        0     1070 2024-02-01 03:43:42.619708 rush_py-3.0.0/rush/tests/test_typedef.py
--rw-r--r--   0        0        0    10193 2024-04-12 08:48:59.536260 rush_py-3.0.0/rush/typedef.py
--rw-r--r--   0        0        0      747 2024-04-07 11:51:36.271482 rush_py-3.0.0/rush/types.py
--rw-r--r--   0        0        0    10796 1970-01-01 00:00:00.000000 rush_py-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     9914 2024-04-14 07:42:20.019580 rush_py-3.0.1/README.md
+-rw-r--r--   0        0        0     2718 2024-04-17 04:40:42.341556 rush_py-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0      481 2024-03-25 07:43:11.134075 rush_py-3.0.1/rush/__init__.py
+-rw-r--r--   0        0        0     1569 2024-04-12 08:48:59.531260 rush_py-3.0.1/rush/async_utils.py
+-rw-r--r--   0        0        0       23 2024-01-29 10:45:57.136914 rush_py-3.0.1/rush/data.py
+-rw-r--r--   0        0        0     1326 2024-04-17 04:40:42.341556 rush_py-3.0.1/rush/doc.py
+-rw-r--r--   0        0        0     7663 2024-04-16 06:00:37.048276 rush_py-3.0.1/rush/graphql_client/__init__.py
+-rw-r--r--   0        0        0      267 2024-04-16 06:00:36.589255 rush_py-3.0.1/rush/graphql_client/argument.py
+-rw-r--r--   0        0        0     1036 2024-04-16 06:00:36.599256 rush_py-3.0.1/rush/graphql_client/arguments.py
+-rw-r--r--   0        0        0    12272 2024-04-17 02:47:58.375356 rush_py-3.0.1/rush/graphql_client/async_base_client.py
+-rw-r--r--   0        0        0      620 2024-04-16 06:00:36.758263 rush_py-3.0.1/rush/graphql_client/base_model.py
+-rw-r--r--   0        0        0      174 2024-04-16 06:00:36.547253 rush_py-3.0.1/rush/graphql_client/cancel_module_instance.py
+-rw-r--r--   0        0        0    28860 2024-04-17 02:47:58.496361 rush_py-3.0.1/rush/graphql_client/client.py
+-rw-r--r--   0        0        0      253 2024-02-28 07:01:47.459725 rush_py-3.0.1/rush/graphql_client/create_entity.py
+-rw-r--r--   0        0        0      277 2024-02-28 07:01:47.461725 rush_py-3.0.1/rush/graphql_client/create_experiment.py
+-rw-r--r--   0        0        0      259 2024-02-28 07:01:47.463725 rush_py-3.0.1/rush/graphql_client/create_project.py
+-rw-r--r--   0        0        0      259 2024-02-28 07:01:47.467725 rush_py-3.0.1/rush/graphql_client/create_protein.py
+-rw-r--r--   0        0        0      314 2024-02-28 07:01:47.465725 rush_py-3.0.1/rush/graphql_client/create_protein_conformer.py
+-rw-r--r--   0        0        0      241 2024-02-28 07:01:47.566729 rush_py-3.0.1/rush/graphql_client/create_smol.py
+-rw-r--r--   0        0        0      296 2024-02-28 07:01:47.564729 rush_py-3.0.1/rush/graphql_client/create_smol_conformer.py
+-rw-r--r--   0        0        0      290 2024-02-28 07:01:47.568729 rush_py-3.0.1/rush/graphql_client/create_smol_tautomer.py
+-rw-r--r--   0        0        0      271 2024-02-28 07:01:47.570730 rush_py-3.0.1/rush/graphql_client/create_structure.py
+-rw-r--r--   0        0        0      341 2024-04-16 06:00:36.551254 rush_py-3.0.1/rush/graphql_client/delete_module_instance.py
+-rw-r--r--   0        0        0      255 2024-04-16 06:00:36.554254 rush_py-3.0.1/rush/graphql_client/deploy.py
+-rw-r--r--   0        0        0      510 2024-02-28 07:01:47.506727 rush_py-3.0.1/rush/graphql_client/entity.py
+-rw-r--r--   0        0        0     1477 2024-04-17 04:40:42.341556 rush_py-3.0.1/rush/graphql_client/enums.py
+-rw-r--r--   0        0        0     2411 2024-04-16 06:00:36.757263 rush_py-3.0.1/rush/graphql_client/exceptions.py
+-rw-r--r--   0        0        0      679 2024-02-28 07:01:47.557729 rush_py-3.0.1/rush/graphql_client/experiment.py
+-rw-r--r--   0        0        0     3769 2024-04-16 06:00:36.757263 rush_py-3.0.1/rush/graphql_client/fragments.py
+-rw-r--r--   0        0        0     5332 2024-04-16 06:00:36.545253 rush_py-3.0.1/rush/graphql_client/input_types.py
+-rw-r--r--   0        0        0      825 2024-04-16 06:00:36.607256 rush_py-3.0.1/rush/graphql_client/latest_modules.py
+-rw-r--r--   0        0        0     2004 2024-04-17 02:47:58.096344 rush_py-3.0.1/rush/graphql_client/module_instance_details.py
+-rw-r--r--   0        0        0     4300 2024-01-29 10:45:57.143915 rush_py-3.0.1/rush/graphql_client/module_instance_full.py
+-rw-r--r--   0        0        0      354 2024-04-16 06:00:36.634257 rush_py-3.0.1/rush/graphql_client/module_instance_minimal.py
+-rw-r--r--   0        0        0      403 2024-01-29 10:45:57.144914 rush_py-3.0.1/rush/graphql_client/module_instance_status.py
+-rw-r--r--   0        0        0     3104 2024-04-17 02:47:58.134345 rush_py-3.0.1/rush/graphql_client/module_instances.py
+-rw-r--r--   0        0        0     2804 2024-01-29 10:45:57.145915 rush_py-3.0.1/rush/graphql_client/module_instances_full.py
+-rw-r--r--   0        0        0      686 2024-04-16 06:00:36.615257 rush_py-3.0.1/rush/graphql_client/modules.py
+-rw-r--r--   0        0        0      160 2024-02-13 05:21:55.039019 rush_py-3.0.1/rush/graphql_client/object.py
+-rw-r--r--   0        0        0      292 2024-04-16 06:00:36.640258 rush_py-3.0.1/rush/graphql_client/object_contents.py
+-rw-r--r--   0        0        0      243 2024-04-16 06:00:36.637258 rush_py-3.0.1/rush/graphql_client/object_url.py
+-rw-r--r--   0        0        0     2121 2024-02-28 07:01:47.518727 rush_py-3.0.1/rush/graphql_client/project.py
+-rw-r--r--   0        0        0      604 2024-02-28 07:01:47.523728 rush_py-3.0.1/rush/graphql_client/protein.py
+-rw-r--r--   0        0        0      687 2024-02-28 07:01:47.528728 rush_py-3.0.1/rush/graphql_client/protein_conformer.py
+-rw-r--r--   0        0        0      234 2024-04-16 06:00:36.643258 rush_py-3.0.1/rush/graphql_client/retry.py
+-rw-r--r--   0        0        0      340 2024-04-16 06:00:36.649258 rush_py-3.0.1/rush/graphql_client/run.py
+-rw-r--r--   0        0        0      571 2024-02-28 07:01:47.533728 rush_py-3.0.1/rush/graphql_client/smol.py
+-rw-r--r--   0        0        0      657 2024-02-28 07:01:47.537728 rush_py-3.0.1/rush/graphql_client/smol_conformer.py
+-rw-r--r--   0        0        0      662 2024-02-28 07:01:47.543728 rush_py-3.0.1/rush/graphql_client/smol_tautomer.py
+-rw-r--r--   0        0        0     1139 2024-02-28 07:01:47.551729 rush_py-3.0.1/rush/graphql_client/structure.py
+-rw-r--r--   0        0        0      161 2024-04-16 06:00:36.651258 rush_py-3.0.1/rush/graphql_client/tag.py
+-rw-r--r--   0        0        0      381 2024-04-16 06:00:36.655259 rush_py-3.0.1/rush/graphql_client/track_utilization.py
+-rw-r--r--   0        0        0      165 2024-04-16 06:00:36.658259 rush_py-3.0.1/rush/graphql_client/untag.py
+-rw-r--r--   0        0        0      414 2024-04-16 06:00:36.681260 rush_py-3.0.1/rush/graphql_client/update_module_instance.py
+-rw-r--r--   0        0        0      328 2024-01-29 10:45:57.148915 rush_py-3.0.1/rush/graphql_client/upload.py
+-rw-r--r--   0        0        0      321 2024-04-16 06:00:36.685260 rush_py-3.0.1/rush/graphql_client/upload_arg.py
+-rw-r--r--   0        0        0      506 2024-04-16 06:00:36.691260 rush_py-3.0.1/rush/graphql_client/upload_object.py
+-rw-r--r--   0        0        0     1226 2024-03-25 07:43:11.134075 rush_py-3.0.1/rush/legacy_types.py
+-rw-r--r--   0        0        0     7403 2024-02-16 09:06:54.345722 rush_py-3.0.1/rush/local.py
+-rw-r--r--   0        0        0     5733 2024-02-16 09:06:54.345722 rush_py-3.0.1/rush/protocols.py
+-rw-r--r--   0        0        0    65355 2024-04-17 04:40:42.342556 rush_py-3.0.1/rush/provider.py
+-rw-r--r--   0        0        0       98 2024-02-16 09:06:54.345722 rush_py-3.0.1/rush/tests/test_provider.py
+-rw-r--r--   0        0        0     1070 2024-02-01 03:43:42.619708 rush_py-3.0.1/rush/tests/test_typedef.py
+-rw-r--r--   0        0        0    10193 2024-04-12 08:48:59.536260 rush_py-3.0.1/rush/typedef.py
+-rw-r--r--   0        0        0      747 2024-04-07 11:51:36.271482 rush_py-3.0.1/rush/types.py
+-rw-r--r--   0        0        0    10796 1970-01-01 00:00:00.000000 rush_py-3.0.1/PKG-INFO
```

### Comparing `rush_py-3.0.0/README.md` & `rush_py-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.0/pyproject.toml` & `rush_py-3.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rush-py"
-version = "3.0.0"
+version = "3.0.1"
 description = "Python SDK for interacting with the QDX Rush API and modules"
 authors = ["Ryan Swart <ryan.swart@qdx.co>", "Sean Laguna <sean.laguna@qdx.co>"]
 readme = "README.md"
 packages = [{include = "rush"}]
 documentation = "https://talo.github.io/rush-py"
 homepage = "https://rush.qdx.co"
```

### Comparing `rush_py-3.0.0/rush/async_utils.py` & `rush_py-3.0.1/rush/async_utils.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.0/rush/doc.py` & `rush_py-3.0.1/rush/doc.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,13 +33,13 @@
 As an output argument, you can expect:
   - a URL for non-JSON files,
   - a `Conformer` or `Record` (i.e. `dict`) for JSON files, or
   - the expected containers or values for other types (`list`, `float`, et cetera).
 """
 
 _x = provider.Provider()
-_fns = asyncio.run(_x.get_module_functions(tags=["rush-py-v2.0.0"]))
+_fns = asyncio.run(_x.get_module_functions(tags=["rush-py-v3.0.0"]))
 RushProvider = type(
     "RushProvider",
     (provider.Provider,),
     _fns | {n: getattr(_x, n) for n in dir(_x)},
 )
```

### Comparing `rush_py-3.0.0/rush/graphql_client/__init__.py` & `rush_py-3.0.1/rush/graphql_client/__init__.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.0/rush/graphql_client/arguments.py` & `rush_py-3.0.1/rush/graphql_client/arguments.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.0/rush/graphql_client/async_base_client.py` & `rush_py-3.0.1/rush/graphql_client/async_base_client.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.0/rush/graphql_client/base_model.py` & `rush_py-3.0.1/rush/graphql_client/base_model.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.0/rush/graphql_client/client.py` & `rush_py-3.0.1/rush/graphql_client/client.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.0/rush/graphql_client/exceptions.py` & `rush_py-3.0.1/rush/graphql_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.0/rush/graphql_client/experiment.py` & `rush_py-3.0.1/rush/graphql_client/experiment.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.0/rush/graphql_client/fragments.py` & `rush_py-3.0.1/rush/graphql_client/fragments.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.0/rush/graphql_client/input_types.py` & `rush_py-3.0.1/rush/graphql_client/input_types.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.0/rush/graphql_client/latest_modules.py` & `rush_py-3.0.1/rush/graphql_client/latest_modules.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.0/rush/graphql_client/module_instance_details.py` & `rush_py-3.0.1/rush/graphql_client/module_instance_details.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.0/rush/graphql_client/module_instance_full.py` & `rush_py-3.0.1/rush/graphql_client/module_instance_full.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.0/rush/graphql_client/module_instances.py` & `rush_py-3.0.1/rush/graphql_client/module_instances.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.0/rush/graphql_client/module_instances_full.py` & `rush_py-3.0.1/rush/graphql_client/module_instances_full.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.0/rush/graphql_client/modules.py` & `rush_py-3.0.1/rush/graphql_client/modules.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.0/rush/graphql_client/project.py` & `rush_py-3.0.1/rush/graphql_client/project.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.0/rush/graphql_client/protein.py` & `rush_py-3.0.1/rush/graphql_client/protein.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.0/rush/graphql_client/protein_conformer.py` & `rush_py-3.0.1/rush/graphql_client/protein_conformer.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.0/rush/graphql_client/smol.py` & `rush_py-3.0.1/rush/graphql_client/smol.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.0/rush/graphql_client/smol_conformer.py` & `rush_py-3.0.1/rush/graphql_client/smol_conformer.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.0/rush/graphql_client/smol_tautomer.py` & `rush_py-3.0.1/rush/graphql_client/smol_tautomer.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.0/rush/graphql_client/structure.py` & `rush_py-3.0.1/rush/graphql_client/structure.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.0/rush/legacy_types.py` & `rush_py-3.0.1/rush/legacy_types.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.0/rush/local.py` & `rush_py-3.0.1/rush/local.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.0/rush/protocols.py` & `rush_py-3.0.1/rush/protocols.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.0/rush/provider.py` & `rush_py-3.0.1/rush/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,24 +251,24 @@
         self.__is_blocking__ = False
 
         if workspace:
             self.workspace: Path | None = Path(workspace)
             if not self.workspace.exists():
                 raise Exception("Workspace directory does not exist")
             if (self.workspace / "rush.lock").exists():
-                self.config_dir: Path | None = self.workspace
+                self._config_dir: Path | None = self.workspace
             else:
-                self.config_dir = self.workspace / ".rush"
-                if not self.config_dir.exists():
-                    self.config_dir.mkdir()
+                self._config_dir = self.workspace / ".rush"
+                if not self._config_dir.exists():
+                    self._config_dir.mkdir()
 
             self.restore(workspace)
         else:
             self.workspace = None
-            self.config_dir = None
+            self._config_dir = None
 
         if not self.history:
             self.history = History(tags=batch_tags or [], instances=[])
         self.batch_tags = batch_tags or []
 
     @staticmethod
     def _load_history(history_file: str | Path):
@@ -322,37 +322,37 @@
     def restore(self, workspace: str | Path):
         """
         Restore the workspace.
         """
         self.workspace = Path(workspace)
 
         if (self.workspace / "rush.lock").exists():
-            self.config_dir = self.workspace
+            self._config_dir = self.workspace
         else:
-            self.config_dir = self.workspace / ".rush"
-            if not self.config_dir.exists():
-                self.config_dir.mkdir()
+            self._config_dir = self.workspace / ".rush"
+            if not self._config_dir.exists():
+                self._config_dir.mkdir()
         # read the workspace history file
         # if it exists, load the history
-        workspace_history = self.config_dir / "history.json"
+        workspace_history = self._config_dir / "history.json"
         if workspace_history.exists():
             self.history = self._load_history(workspace_history)
 
-        if (self.config_dir / "rush.lock").exists():
-            self.load_module_paths(self.config_dir / "rush.lock")
+        if (self._config_dir / "rush.lock").exists():
+            self.load_module_paths(self._config_dir / "rush.lock")
 
     def save(self, history_file: str | Path | None = None):
         """
         Save the workspace.
         """
-        if self.config_dir is None:
+        if self._config_dir is None:
             raise Exception("No workspace provided")
         if history_file is None:
-            history_file = self.config_dir / "history.json"
-        self.save_module_paths(self.module_paths, self.config_dir / "rush.lock")
+            history_file = self._config_dir / "history.json"
+        self.save_module_paths(self.module_paths, self._config_dir / "rush.lock")
         with open(history_file, "w") as f:
             json.dump(self.history, f, default=to_jsonable_python, indent=2)
 
     async def status(
         self,
         instance_ids: list[ModuleInstanceId] | None = None,
         workspace: str | Path | None = None,
@@ -516,24 +516,28 @@
                 json.dump(obj.contents, open(filepath, "w"))
             elif obj:
                 with httpx.stream(method="get", url=obj.url) as r:
                     r.raise_for_status()
 
                     buf = ""
                     with open(filepath, "wb") as f:
+                        if not decode:
+                            for chunk in r.iter_bytes():
+                                f.write(chunk)
+                            return filepath
                         first_chunk = True
                         is_encoded = False
                         for chunk in r.iter_text():
                             if not first_chunk and not is_encoded:
                                 f.write(chunk.encode("utf-8"))
                                 continue
 
                             # handle json
                             if first_chunk:
-                                if len(chunk) > 0 and (chunk[0] == "[" or chunk[0] == "{") or not decode:
+                                if len(chunk) > 0 and (chunk[0] == "[" or chunk[0] == "{"):
                                     f.write(chunk.encode("utf-8"))
                                     first_chunk = False
                                     continue
                                 else:
                                     first_chunk = False
                                     is_encoded = True
 
@@ -893,15 +897,15 @@
         """
 
         ret: dict[str, RushModuleRunner[Any]] = {}
         if lockfile is not None:
             module_paths = self.load_module_paths(lockfile)
             module_pages = self.get_modules_for_paths(list(module_paths.values()))
         else:
-            if self.config_dir:
+            if self._config_dir:
                 if self.module_paths.items():
                     # we have already loaded a lock via the workspace
                     module_pages = self.get_modules_for_paths(list(self.module_paths.values()))
                 else:
                     # lets load the latest paths and lock them
                     if tags:
                         module_pages = await self.modules(tags=tags)
@@ -913,15 +917,15 @@
                                 if (names and name in names) and path:
                                     self.module_paths[name] = path
                         module_pages = await self.modules(tags=tags)
                     else:
                         paths = await self.get_latest_module_paths(names)
                         module_pages = self.get_modules_for_paths(list(paths.values()))
                         self.module_paths = paths
-                        self.save_module_paths(self.module_paths, self.config_dir / "rush.lock")
+                        self.save_module_paths(self.module_paths, self._config_dir / "rush.lock")
             elif tags:
                 # no workspace, so up the user to lock it
                 module_pages = await self.modules(tags=tags)
             else:
                 # no workspace, so up the user to lock it
                 module_pages = await self.latest_modules(names=names)
 
@@ -940,17 +944,17 @@
 
         for name, module in sorted(modules):
             path = module.path
 
             out_types = tuple(type_from_typedef(i) for i in module.outs)
 
             def random_target():
-                allowed_default_targets = ["NIX_SSH", "NIX_SSH_2"]
-                if "NIX_SSH_3" in str(module.targets) or "NIX_SSH_3_GPU" in str(module.targets):
-                    allowed_default_targets.append("NIX_SSH_3")
+                allowed_default_targets = ["BULLET", "BULLET_2"]
+                if "BULLET_3" in str(module.targets) or "BULLET_3_GPU" in str(module.targets):
+                    allowed_default_targets.append("BULLET_3")
                 return random.choice(allowed_default_targets)
 
             default_resources = None
             if module.resource_bounds:
                 default_resources = {
                     "storage": module.resource_bounds.storage_min + 10,
                     "storage_units": "MB",
@@ -1101,15 +1105,15 @@
 
         :param file: The file to be uploaded.
         :param typeinfo: The typeinfo of the file.
         """
         if isinstance(file, str):
             file = Path(file)
         with open(file, "rb") as f:
-            format = ObjectFormat.JSON if file.suffix == ".json" else ObjectFormat.BIN
+            format = ObjectFormat.json if file.suffix == ".json" else ObjectFormat.bin
             mimetype = mimetypes.guess_type(file)[0]
             return await self.client.upload_object(
                 typeinfo=typeinfo,
                 format=format,
                 file=Upload(filename=f.name, content=f, content_type=mimetype or "text/plain"),
             )
 
@@ -1179,34 +1183,34 @@
     async def update_modules(self, names: list[str] | None = None, tags: list[str] | None = None):
         """
         Update the module paths in the lockfile.
 
         :param names: Optional list of names to update.
         :param tags: Optionally only upate modules with this tag.
         """
-        if not self.config_dir:
+        if not self._config_dir:
             raise Exception("No workspace provided")
 
         if tags:
             module_pages = await self.modules(tags=tags)
             self.module_paths = {}
             async for module_page in module_pages:
                 for edge in module_page.edges:
                     path = edge.node.path
                     name = get_name_from_path(edge.node.path)
                     if names:
                         if name in names and path:
                             self.module_paths[name] = path
                     else:
                         self.module_paths[name] = path
-            self.save_module_paths(self.module_paths, self.config_dir / "rush.lock")
+            self.save_module_paths(self.module_paths, self._config_dir / "rush.lock")
         else:
             paths = await self.get_latest_module_paths(names)
             self.module_paths = paths
-            self.save_module_paths(self.module_paths, self.config_dir / "rush.lock")
+            self.save_module_paths(self.module_paths, self._config_dir / "rush.lock")
 
     async def delete_module_instance(self, id: ModuleInstanceId):
         """
         Delete a module instance with a given ID.
 
         :param id: The ID of the module instance to be deleted.
         :return: The ID of the deleted module instance.
@@ -1338,15 +1342,15 @@
                     (self.typeinfo["k"] == "record" and self.typeinfo["n"] == "Object")
                     or (
                         self.typeinfo["k"] == "optional"
                         and (self.typeinfo["t"]["k"] == "record" and self.typeinfo["t"]["n"] == "Object")
                     )
                 ):
                     signed = "$" in json.dumps(self.typeinfo)
-                    decode = not (self.value and dict.get(self.value, "format") == "Bin")
+                    decode = not (self.value and dict.get(self.value, "format") == "bin")
                     return await self.provider.download_object(
                         self.value["path"], filename, filepath, overwrite, signed, decode
                     )
                 else:
                     raise Exception("Cannot download non-object argument")
             else:
                 raise Exception("Cannot download argument without typeinfo")
@@ -1450,17 +1454,17 @@
 
         :param access_token: The access token to use.
         :param url: The url to use.
         :param workspace: The workspace directory to use.
         :param batch_tags: The tags that will be placed on all runs by default.
         """
         if workspace is None:
-            workspace = os.getcwd()
+            workspace = Path(".")
         if workspace is True:
-            workspace = os.getcwd()
+            workspace = Path(".")
         if workspace is False:
             workspace = None
 
         if not logger:
             logger = logging.getLogger("rush")
             if len(logger.handlers) == 0:
                 stderr_handler = logging.StreamHandler()
```

### Comparing `rush_py-3.0.0/rush/tests/test_typedef.py` & `rush_py-3.0.1/rush/tests/test_typedef.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.0/rush/typedef.py` & `rush_py-3.0.1/rush/typedef.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.0/rush/types.py` & `rush_py-3.0.1/rush/types.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.0/PKG-INFO` & `rush_py-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rush-py
-Version: 3.0.0
+Version: 3.0.1
 Summary: Python SDK for interacting with the QDX Rush API and modules
 Home-page: https://rush.qdx.co
 Author: Ryan Swart
 Author-email: ryan.swart@qdx.co
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

