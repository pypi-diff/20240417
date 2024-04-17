# Comparing `tmp/sqlmodel_react_admin-0.0.2.tar.gz` & `tmp/sqlmodel_react_admin-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmodel_react_admin-0.0.2.tar", max compression
+gzip compressed data, was "sqlmodel_react_admin-0.0.3.tar", max compression
```

## Comparing `sqlmodel_react_admin-0.0.2.tar` & `sqlmodel_react_admin-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2024-04-17 07:50:51.516989 sqlmodel_react_admin-0.0.2/LICENSE
--rw-r--r--   0        0        0      114 2024-04-17 07:53:35.781555 sqlmodel_react_admin-0.0.2/README.md
--rw-r--r--   0        0        0      488 2024-04-17 08:04:41.732663 sqlmodel_react_admin-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      527 2024-04-17 07:51:08.677471 sqlmodel_react_admin-0.0.2/sqlmodel_react_admin/db.py
--rw-r--r--   0        0        0      396 2024-04-17 07:51:08.677471 sqlmodel_react_admin-0.0.2/sqlmodel_react_admin/models.py
--rw-r--r--   0        0        0     9859 2024-04-17 08:03:52.238033 sqlmodel_react_admin-0.0.2/sqlmodel_react_admin/routers.py
--rw-r--r--   0        0        0      706 1970-01-01 00:00:00.000000 sqlmodel_react_admin-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-17 07:50:51.516989 sqlmodel_react_admin-0.0.3/LICENSE
+-rw-r--r--   0        0        0      114 2024-04-17 07:53:35.781555 sqlmodel_react_admin-0.0.3/README.md
+-rw-r--r--   0        0        0      506 2024-04-17 08:42:30.158894 sqlmodel_react_admin-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      190 2024-04-17 08:16:39.104617 sqlmodel_react_admin-0.0.3/sqlmodel_react_admin/client.py
+-rw-r--r--   0        0        0      396 2024-04-17 07:51:08.677471 sqlmodel_react_admin-0.0.3/sqlmodel_react_admin/models.py
+-rw-r--r--   0        0        0    17829 2024-04-17 08:41:14.326912 sqlmodel_react_admin-0.0.3/sqlmodel_react_admin/routers.py
+-rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 sqlmodel_react_admin-0.0.3/PKG-INFO
```

### Comparing `sqlmodel_react_admin-0.0.2/LICENSE` & `sqlmodel_react_admin-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmodel_react_admin-0.0.2/PKG-INFO` & `sqlmodel_react_admin-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: sqlmodel-react-admin
-Version: 0.0.2
+Version: 0.0.3
 Summary: Create fast SQLModel/FastAPI APIs/BFFs for React Admin
 License: MIT
 Author: Evan Thomas
 Author-email: evan@evanjt.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: fastapi (>=0.110.1,<0.111.0)
+Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: sqlmodel (>=0.0.16,<0.0.17)
 Requires-Dist: uvicorn (>=0.29.0,<0.30.0)
 Description-Content-Type: text/markdown
 
 # sqlmodel-react-admin
 
 Some structures to generate routes for use in APIs and BFFs, using SQLModel, and
```

