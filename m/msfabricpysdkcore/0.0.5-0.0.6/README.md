# Comparing `tmp/msfabricpysdkcore-0.0.5.tar.gz` & `tmp/msfabricpysdkcore-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msfabricpysdkcore-0.0.5.tar", last modified: Thu Apr 11 17:35:20 2024, max compression
+gzip compressed data, was "msfabricpysdkcore-0.0.6.tar", last modified: Wed Apr 17 12:38:20 2024, max compression
```

## Comparing `msfabricpysdkcore-0.0.5.tar` & `msfabricpysdkcore-0.0.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 17:35:20.495555 msfabricpysdkcore-0.0.5/
--rw-rw-rw-   0        0        0     1156 2024-04-10 07:49:21.000000 msfabricpysdkcore-0.0.5/LICENSE
--rw-rw-rw-   0        0        0    16184 2024-04-11 17:35:20.483603 msfabricpysdkcore-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0    15666 2024-04-11 09:50:11.000000 msfabricpysdkcore-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 17:35:20.381876 msfabricpysdkcore-0.0.5/msfabricpysdkcore/
--rw-rw-rw-   0        0        0       78 2024-04-10 09:59:59.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/__init__.py
--rw-rw-rw-   0        0        0     3778 2024-04-11 09:28:32.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/admin_item.py
--rw-rw-rw-   0        0        0     4248 2024-04-11 07:13:04.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/admin_workspace.py
--rw-rw-rw-   0        0        0    21039 2024-04-11 09:11:00.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/adminapi.py
--rw-rw-rw-   0        0        0     1929 2024-04-02 10:11:53.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/auth.py
--rw-rw-rw-   0        0        0     1761 2024-04-10 09:00:53.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/capacity.py
--rw-rw-rw-   0        0        0     1060 2024-04-10 09:50:03.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/client.py
--rw-rw-rw-   0        0        0    14423 2024-04-11 14:22:24.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/coreapi.py
--rw-rw-rw-   0        0        0    14722 2024-04-10 15:15:40.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/domain.py
--rw-rw-rw-   0        0        0    11296 2024-04-11 14:34:03.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/item.py
--rw-rw-rw-   0        0        0     2745 2024-04-11 11:55:54.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/job_instance.py
--rw-rw-rw-   0        0        0     3928 2024-04-11 11:55:24.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/lakehouse.py
--rw-rw-rw-   0        0        0     2848 2024-04-11 16:24:05.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/long_running_operation.py
--rw-rw-rw-   0        0        0     2102 2024-04-10 09:00:15.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/onelakeshortcut.py
--rw-rw-rw-   0        0        0      737 2024-04-11 13:45:47.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/otheritems.py
-drwxrwxrwx   0        0        0        0 2024-04-11 17:35:20.465140 msfabricpysdkcore-0.0.5/msfabricpysdkcore/tests/
--rw-rw-rw-   0        0        0        0 2024-03-22 16:16:45.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/tests/__init__.py
--rw-rw-rw-   0        0        0     2062 2024-04-11 09:34:12.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/tests/test_admin_apis.py
--rw-rw-rw-   0        0        0     4649 2024-04-10 15:12:58.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/tests/test_domains.py
--rw-rw-rw-   0        0        0     2398 2024-04-10 09:53:02.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/tests/test_git.py
--rw-rw-rw-   0        0        0     4627 2024-04-11 15:34:34.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/tests/test_items_incl_lakehouse.py
--rw-rw-rw-   0        0        0     1581 2024-04-10 09:53:00.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/tests/test_jobs.py
--rw-rw-rw-   0        0        0     2390 2024-04-10 09:53:04.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/tests/test_shortcuts.py
--rw-rw-rw-   0        0        0     6563 2024-04-10 09:53:06.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/tests/test_workspaces_capacities.py
--rw-rw-rw-   0        0        0    26160 2024-04-11 14:25:12.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore/workspace.py
-drwxrwxrwx   0        0        0        0 2024-04-11 17:35:20.483603 msfabricpysdkcore-0.0.5/msfabricpysdkcore.egg-info/
--rw-rw-rw-   0        0        0    16184 2024-04-11 17:35:20.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1091 2024-04-11 17:35:20.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 17:35:20.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-04-11 17:35:20.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-11 17:35:20.000000 msfabricpysdkcore-0.0.5/msfabricpysdkcore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      564 2024-04-11 10:42:03.000000 msfabricpysdkcore-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-11 17:35:20.496556 msfabricpysdkcore-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      235 2024-04-11 10:41:58.000000 msfabricpysdkcore-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:38:20.846543 msfabricpysdkcore-0.0.6/
+-rw-rw-rw-   0        0        0     1156 2024-04-10 07:49:21.000000 msfabricpysdkcore-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0    16383 2024-04-17 12:38:20.843721 msfabricpysdkcore-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0    15865 2024-04-17 08:55:42.000000 msfabricpysdkcore-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 12:38:20.690564 msfabricpysdkcore-0.0.6/msfabricpysdkcore/
+-rw-rw-rw-   0        0        0       78 2024-04-10 09:59:59.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/__init__.py
+-rw-rw-rw-   0        0        0     3778 2024-04-11 09:28:32.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/admin_item.py
+-rw-rw-rw-   0        0        0     4248 2024-04-11 07:13:04.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/admin_workspace.py
+-rw-rw-rw-   0        0        0    21039 2024-04-11 09:11:00.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/adminapi.py
+-rw-rw-rw-   0        0        0     1929 2024-04-12 14:12:32.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/auth.py
+-rw-rw-rw-   0        0        0     1761 2024-04-10 09:00:53.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/capacity.py
+-rw-rw-rw-   0        0        0     1060 2024-04-10 09:50:03.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/client.py
+-rw-rw-rw-   0        0        0    32048 2024-04-16 15:03:12.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/coreapi.py
+-rw-rw-rw-   0        0        0    14722 2024-04-10 15:15:40.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/domain.py
+-rw-rw-rw-   0        0        0    11570 2024-04-16 14:02:36.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/item.py
+-rw-rw-rw-   0        0        0     2745 2024-04-11 11:55:54.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/job_instance.py
+-rw-rw-rw-   0        0        0     3928 2024-04-11 11:55:24.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/lakehouse.py
+-rw-rw-rw-   0        0        0     2848 2024-04-11 16:24:05.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/long_running_operation.py
+-rw-rw-rw-   0        0        0     2102 2024-04-10 09:00:15.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/onelakeshortcut.py
+-rw-rw-rw-   0        0        0     3834 2024-04-15 14:15:34.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/otheritems.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:38:20.834665 msfabricpysdkcore-0.0.6/msfabricpysdkcore/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-22 16:16:45.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/tests/__init__.py
+-rw-rw-rw-   0        0        0     2062 2024-04-11 09:34:12.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/tests/test_admin_apis.py
+-rw-rw-rw-   0        0        0     4649 2024-04-10 15:12:58.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/tests/test_domains.py
+-rw-rw-rw-   0        0        0     2398 2024-04-10 09:53:02.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/tests/test_git.py
+-rw-rw-rw-   0        0        0    21116 2024-04-17 07:45:33.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/tests/test_items_incl_lakehouse.py
+-rw-rw-rw-   0        0        0     1581 2024-04-10 09:53:00.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/tests/test_jobs.py
+-rw-rw-rw-   0        0        0     2390 2024-04-10 09:53:04.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/tests/test_shortcuts.py
+-rw-rw-rw-   0        0        0     6563 2024-04-10 09:53:06.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/tests/test_workspaces_capacities.py
+-rw-rw-rw-   0        0        0    48660 2024-04-16 15:03:00.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore/workspace.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:38:20.840708 msfabricpysdkcore-0.0.6/msfabricpysdkcore.egg-info/
+-rw-rw-rw-   0        0        0    16383 2024-04-17 12:38:20.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1091 2024-04-17 12:38:20.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 12:38:20.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-04-17 12:38:20.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-17 12:38:20.000000 msfabricpysdkcore-0.0.6/msfabricpysdkcore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      564 2024-04-15 14:48:54.000000 msfabricpysdkcore-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-17 12:38:20.846543 msfabricpysdkcore-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      235 2024-04-15 14:48:59.000000 msfabricpysdkcore-0.0.6/setup.py
```

### Comparing `msfabricpysdkcore-0.0.5/LICENSE` & `msfabricpysdkcore-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.5/PKG-INFO` & `msfabricpysdkcore-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msfabricpysdkcore
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python SDK for Microsoft Fabric
 Author: Andreas Rederer
 Project-URL: Homepage, https://github.com/DaSenf1860/ms-fabric-sdk-core
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
@@ -30,15 +30,15 @@
 - Referencing objects by name instead of ID
 - More granular objects, e.g. a Workspace and Item object instead of referencing IDs all the time
 - Do bulk operations (see [Usage Patterns](usage_patterns.md))
 - Pagination support
 
 See the latest release notes [here](releasenotes/release_notes.md).
 
-Currently it supports all Core APIs, Admin APIs and Lakehouse APIs, i.e.:
+Currently it supports all Core APIs, Admin APIs, Lakehouse APIs and all other item specific CRUD APIs, i.e.:
 - Core APIs
   - [Capacities](#working-with-capacities)
   - [Git](#working-with-git)
   - [Items](#working-with-items)
   - [Job Scheduler](#working-with-job-scheduler)
   - Long Running Operations
   - [OneLakeShortcuts](#working-with-one-lake-shortcuts)
@@ -47,16 +47,18 @@
   - [Tables](#tables)
 - Admin APIs
   - [Domains](#admin-api-for-domains)
   - [Items](#admin-api-for-items)
   - [Tenants](#admin-api-for-tenants)
   - [Users](#admin-api-for-users)
   - [Workspaces](#admin-api-for-workspaces)
+- [Item Specific CRUD APIs](item_specific_apis.md), e.g.
+  - List, create, update, delete warehouses, notebooks, semantic models, kql databases,.....
 
-It is planned to support also the APIs of the user experiences and new APIs which are not released yet.
+It is planned to support also new APIs which are not released yet.
 Also we have plans to support APIs to interact with Fabric capacities on the Azure Side.
 Eventually Power BI APIs like the Scanner API will be covered as well.
 
 *Because this SDK uses the API in the background, all limitations and restrictions of the API apply to this SDK as well. This includes rate limits, permissions, etc.
 
 
 
@@ -354,14 +356,17 @@
 # Run a on demand item job
 fc.run_on_demand_item_job(workspace_id="workspace_id", item_id="item_id", job_type="RunNotebook", execution_data = None)
 # or
 ws.run_on_demand_item_job(item_id="item_id", job_type="RunNotebook", execution_data = None)
 # or
 item.run_on_demand_item_job(job_type="RunNotebook", execution_data = None)
 
+# Other job types are e.g.:
+jobType=Pipeline
+
 
 # Get an item job instance
 fc.get_item_job_instance(workspace_id="workspace_id", item_id="item_id", job_instance_id="job_instance_id")
 # or
 ws.get_item_job_instance(item_id="item_id", job_instance_id="job_instance_id")
 # or
 item.get_item_job_instance(job_instance_id="job_instance_id")
```

### Comparing `msfabricpysdkcore-0.0.5/README.md` & `msfabricpysdkcore-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 - Referencing objects by name instead of ID
 - More granular objects, e.g. a Workspace and Item object instead of referencing IDs all the time
 - Do bulk operations (see [Usage Patterns](usage_patterns.md))
 - Pagination support
 
 See the latest release notes [here](releasenotes/release_notes.md).
 
-Currently it supports all Core APIs, Admin APIs and Lakehouse APIs, i.e.:
+Currently it supports all Core APIs, Admin APIs, Lakehouse APIs and all other item specific CRUD APIs, i.e.:
 - Core APIs
   - [Capacities](#working-with-capacities)
   - [Git](#working-with-git)
   - [Items](#working-with-items)
   - [Job Scheduler](#working-with-job-scheduler)
   - Long Running Operations
   - [OneLakeShortcuts](#working-with-one-lake-shortcuts)
@@ -32,16 +32,18 @@
   - [Tables](#tables)
 - Admin APIs
   - [Domains](#admin-api-for-domains)
   - [Items](#admin-api-for-items)
   - [Tenants](#admin-api-for-tenants)
   - [Users](#admin-api-for-users)
   - [Workspaces](#admin-api-for-workspaces)
+- [Item Specific CRUD APIs](item_specific_apis.md), e.g.
+  - List, create, update, delete warehouses, notebooks, semantic models, kql databases,.....
 
-It is planned to support also the APIs of the user experiences and new APIs which are not released yet.
+It is planned to support also new APIs which are not released yet.
 Also we have plans to support APIs to interact with Fabric capacities on the Azure Side.
 Eventually Power BI APIs like the Scanner API will be covered as well.
 
 *Because this SDK uses the API in the background, all limitations and restrictions of the API apply to this SDK as well. This includes rate limits, permissions, etc.
 
 
 
@@ -339,14 +341,17 @@
 # Run a on demand item job
 fc.run_on_demand_item_job(workspace_id="workspace_id", item_id="item_id", job_type="RunNotebook", execution_data = None)
 # or
 ws.run_on_demand_item_job(item_id="item_id", job_type="RunNotebook", execution_data = None)
 # or
 item.run_on_demand_item_job(job_type="RunNotebook", execution_data = None)
 
+# Other job types are e.g.:
+jobType=Pipeline
+
 
 # Get an item job instance
 fc.get_item_job_instance(workspace_id="workspace_id", item_id="item_id", job_instance_id="job_instance_id")
 # or
 ws.get_item_job_instance(item_id="item_id", job_instance_id="job_instance_id")
 # or
 item.get_item_job_instance(job_instance_id="job_instance_id")
```

### Comparing `msfabricpysdkcore-0.0.5/msfabricpysdkcore/admin_item.py` & `msfabricpysdkcore-0.0.6/msfabricpysdkcore/admin_item.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.5/msfabricpysdkcore/admin_workspace.py` & `msfabricpysdkcore-0.0.6/msfabricpysdkcore/admin_workspace.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.5/msfabricpysdkcore/adminapi.py` & `msfabricpysdkcore-0.0.6/msfabricpysdkcore/adminapi.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.5/msfabricpysdkcore/auth.py` & `msfabricpysdkcore-0.0.6/msfabricpysdkcore/auth.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.5/msfabricpysdkcore/capacity.py` & `msfabricpysdkcore-0.0.6/msfabricpysdkcore/capacity.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.5/msfabricpysdkcore/client.py` & `msfabricpysdkcore-0.0.6/msfabricpysdkcore/client.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.5/msfabricpysdkcore/domain.py` & `msfabricpysdkcore-0.0.6/msfabricpysdkcore/domain.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.5/msfabricpysdkcore/item.py` & `msfabricpysdkcore-0.0.6/msfabricpysdkcore/item.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,17 +46,20 @@
             return Lakehouse(id=item_dict['id'], display_name=item_dict['displayName'], type=item_dict['type'], workspace_id=item_dict['workspaceId'],
                     properties=item_dict.get('properties', None),
                     definition=item_dict.get('definition', None), description=item_dict.get('description', ""), auth=auth)
         return Item(id=item_dict['id'], display_name=item_dict['displayName'], type=item_dict['type'], workspace_id=item_dict['workspaceId'],
                     properties=item_dict.get('properties', None),
                     definition=item_dict.get('definition', None), description=item_dict.get('description', ""), auth=auth)
 
-    def delete(self):
+    def delete(self, type = None):
         """Delete the workspace item"""
+
         url = f"https://api.fabric.microsoft.com/v1/workspaces/{self.workspace_id}/items/{self.id}"
+        if type:
+            url = f"https://api.fabric.microsoft.com/v1/workspaces/{self.workspace_id}/{type}/{self.id}"
         for _ in range(10):
             response = requests.delete(url=url, headers=self.auth.get_headers())
             if response.status_code == 429:
                 print("Too many requests, waiting 10 seconds")
                 sleep(10)
                 continue
             if response.status_code not in (200, 429):
@@ -90,24 +93,25 @@
                 raise Exception(f"Error getting item definition: {response.text}")
             break
         
         resp_dict = json.loads(response.text)
         self.definition = resp_dict['definition']
         return resp_dict
     
-    def update(self, display_name = None, description = None):
+    def update(self, display_name = None, description = None, type = None):
         """Update the item"""
         url = f"https://api.fabric.microsoft.com/v1/workspaces/{self.workspace_id}/items/{self.id}"
+        if type:
+            url = f"https://api.fabric.microsoft.com/v1/workspaces/{self.workspace_id}/{type}/{self.id}"
 
         payload = dict()
         if display_name:
             payload['displayName'] = display_name
         if description:
             payload['description'] = description
-
         for _ in range(10):
             response = requests.patch(url=url, headers=self.auth.get_headers(), json=payload)
             if response.status_code == 429:
                 print("Too many requests, waiting 10 seconds")
                 sleep(10)
                 continue
             if response.status_code not in (200, 429):
```

### Comparing `msfabricpysdkcore-0.0.5/msfabricpysdkcore/job_instance.py` & `msfabricpysdkcore-0.0.6/msfabricpysdkcore/job_instance.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.5/msfabricpysdkcore/lakehouse.py` & `msfabricpysdkcore-0.0.6/msfabricpysdkcore/lakehouse.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.5/msfabricpysdkcore/long_running_operation.py` & `msfabricpysdkcore-0.0.6/msfabricpysdkcore/long_running_operation.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.5/msfabricpysdkcore/onelakeshortcut.py` & `msfabricpysdkcore-0.0.6/msfabricpysdkcore/onelakeshortcut.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.5/msfabricpysdkcore/tests/test_admin_apis.py` & `msfabricpysdkcore-0.0.6/msfabricpysdkcore/tests/test_admin_apis.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.5/msfabricpysdkcore/tests/test_domains.py` & `msfabricpysdkcore-0.0.6/msfabricpysdkcore/tests/test_domains.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.5/msfabricpysdkcore/tests/test_git.py` & `msfabricpysdkcore-0.0.6/msfabricpysdkcore/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.5/msfabricpysdkcore/tests/test_jobs.py` & `msfabricpysdkcore-0.0.6/msfabricpysdkcore/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.5/msfabricpysdkcore/tests/test_shortcuts.py` & `msfabricpysdkcore-0.0.6/msfabricpysdkcore/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.5/msfabricpysdkcore/tests/test_workspaces_capacities.py` & `msfabricpysdkcore-0.0.6/msfabricpysdkcore/tests/test_workspaces_capacities.py`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.5/msfabricpysdkcore.egg-info/PKG-INFO` & `msfabricpysdkcore-0.0.6/msfabricpysdkcore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msfabricpysdkcore
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python SDK for Microsoft Fabric
 Author: Andreas Rederer
 Project-URL: Homepage, https://github.com/DaSenf1860/ms-fabric-sdk-core
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
@@ -30,15 +30,15 @@
 - Referencing objects by name instead of ID
 - More granular objects, e.g. a Workspace and Item object instead of referencing IDs all the time
 - Do bulk operations (see [Usage Patterns](usage_patterns.md))
 - Pagination support
 
 See the latest release notes [here](releasenotes/release_notes.md).
 
-Currently it supports all Core APIs, Admin APIs and Lakehouse APIs, i.e.:
+Currently it supports all Core APIs, Admin APIs, Lakehouse APIs and all other item specific CRUD APIs, i.e.:
 - Core APIs
   - [Capacities](#working-with-capacities)
   - [Git](#working-with-git)
   - [Items](#working-with-items)
   - [Job Scheduler](#working-with-job-scheduler)
   - Long Running Operations
   - [OneLakeShortcuts](#working-with-one-lake-shortcuts)
@@ -47,16 +47,18 @@
   - [Tables](#tables)
 - Admin APIs
   - [Domains](#admin-api-for-domains)
   - [Items](#admin-api-for-items)
   - [Tenants](#admin-api-for-tenants)
   - [Users](#admin-api-for-users)
   - [Workspaces](#admin-api-for-workspaces)
+- [Item Specific CRUD APIs](item_specific_apis.md), e.g.
+  - List, create, update, delete warehouses, notebooks, semantic models, kql databases,.....
 
-It is planned to support also the APIs of the user experiences and new APIs which are not released yet.
+It is planned to support also new APIs which are not released yet.
 Also we have plans to support APIs to interact with Fabric capacities on the Azure Side.
 Eventually Power BI APIs like the Scanner API will be covered as well.
 
 *Because this SDK uses the API in the background, all limitations and restrictions of the API apply to this SDK as well. This includes rate limits, permissions, etc.
 
 
 
@@ -354,14 +356,17 @@
 # Run a on demand item job
 fc.run_on_demand_item_job(workspace_id="workspace_id", item_id="item_id", job_type="RunNotebook", execution_data = None)
 # or
 ws.run_on_demand_item_job(item_id="item_id", job_type="RunNotebook", execution_data = None)
 # or
 item.run_on_demand_item_job(job_type="RunNotebook", execution_data = None)
 
+# Other job types are e.g.:
+jobType=Pipeline
+
 
 # Get an item job instance
 fc.get_item_job_instance(workspace_id="workspace_id", item_id="item_id", job_instance_id="job_instance_id")
 # or
 ws.get_item_job_instance(item_id="item_id", job_instance_id="job_instance_id")
 # or
 item.get_item_job_instance(job_instance_id="job_instance_id")
```

### Comparing `msfabricpysdkcore-0.0.5/msfabricpysdkcore.egg-info/SOURCES.txt` & `msfabricpysdkcore-0.0.6/msfabricpysdkcore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `msfabricpysdkcore-0.0.5/pyproject.toml` & `msfabricpysdkcore-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 65.5.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msfabricpysdkcore"
-version = "0.0.5"
+version = "0.0.6"
 dynamic = ["dependencies"]
 authors = [
   { name="Andreas Rederer"},
 ]
 description = "A Python SDK for Microsoft Fabric"
 readme = "README.md"
 requires-python = ">=3.11"
```

