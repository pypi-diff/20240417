# Comparing `tmp/sqlmodel_react_admin-0.0.1.tar.gz` & `tmp/sqlmodel_react_admin-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmodel_react_admin-0.0.1.tar", max compression
+gzip compressed data, was "sqlmodel_react_admin-0.0.2.tar", max compression
```

## Comparing `sqlmodel_react_admin-0.0.1.tar` & `sqlmodel_react_admin-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2024-04-17 07:50:51.516989 sqlmodel_react_admin-0.0.1/LICENSE
--rw-r--r--   0        0        0      114 2024-04-17 07:53:35.781555 sqlmodel_react_admin-0.0.1/README.md
--rw-r--r--   0        0        0      488 2024-04-17 07:51:08.677471 sqlmodel_react_admin-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      527 2024-04-17 07:51:08.677471 sqlmodel_react_admin-0.0.1/sqlmodel_react_admin/generic/db.py
--rw-r--r--   0        0        0      396 2024-04-17 07:51:08.677471 sqlmodel_react_admin-0.0.1/sqlmodel_react_admin/generic/models.py
--rw-r--r--   0        0        0     9842 2024-04-17 07:51:08.677471 sqlmodel_react_admin-0.0.1/sqlmodel_react_admin/generic/routers.py
--rw-r--r--   0        0        0      706 1970-01-01 00:00:00.000000 sqlmodel_react_admin-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-17 07:50:51.516989 sqlmodel_react_admin-0.0.2/LICENSE
+-rw-r--r--   0        0        0      114 2024-04-17 07:53:35.781555 sqlmodel_react_admin-0.0.2/README.md
+-rw-r--r--   0        0        0      488 2024-04-17 08:04:41.732663 sqlmodel_react_admin-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      527 2024-04-17 07:51:08.677471 sqlmodel_react_admin-0.0.2/sqlmodel_react_admin/db.py
+-rw-r--r--   0        0        0      396 2024-04-17 07:51:08.677471 sqlmodel_react_admin-0.0.2/sqlmodel_react_admin/models.py
+-rw-r--r--   0        0        0     9859 2024-04-17 08:03:52.238033 sqlmodel_react_admin-0.0.2/sqlmodel_react_admin/routers.py
+-rw-r--r--   0        0        0      706 1970-01-01 00:00:00.000000 sqlmodel_react_admin-0.0.2/PKG-INFO
```

### Comparing `sqlmodel_react_admin-0.0.1/LICENSE` & `sqlmodel_react_admin-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmodel_react_admin-0.0.1/sqlmodel_react_admin/generic/db.py` & `sqlmodel_react_admin-0.0.2/sqlmodel_react_admin/db.py`

 * *Files identical despite different names*

### Comparing `sqlmodel_react_admin-0.0.1/sqlmodel_react_admin/generic/routers.py` & `sqlmodel_react_admin-0.0.2/sqlmodel_react_admin/routers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from sqlmodel import SQLModel
 from fastapi import Depends, APIRouter, Query, Response, HTTPException, Request
 from sqlmodel import select
-from app.db import get_session, AsyncSession
+from sqlmodel_react_admin.db import get_session, AsyncSession
 from uuid import UUID
 from sqlalchemy import func
 import json
 
 
 class ReactAdminRouter:
     def __init__(
```

### Comparing `sqlmodel_react_admin-0.0.1/PKG-INFO` & `sqlmodel_react_admin-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlmodel-react-admin
-Version: 0.0.1
+Version: 0.0.2
 Summary: Create fast SQLModel/FastAPI APIs/BFFs for React Admin
 License: MIT
 Author: Evan Thomas
 Author-email: evan@evanjt.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

