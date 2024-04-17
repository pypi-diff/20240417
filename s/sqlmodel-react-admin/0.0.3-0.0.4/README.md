# Comparing `tmp/sqlmodel_react_admin-0.0.3.tar.gz` & `tmp/sqlmodel_react_admin-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmodel_react_admin-0.0.3.tar", max compression
+gzip compressed data, was "sqlmodel_react_admin-0.0.4.tar", max compression
```

## Comparing `sqlmodel_react_admin-0.0.3.tar` & `sqlmodel_react_admin-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2024-04-17 07:50:51.516989 sqlmodel_react_admin-0.0.3/LICENSE
--rw-r--r--   0        0        0      114 2024-04-17 07:53:35.781555 sqlmodel_react_admin-0.0.3/README.md
--rw-r--r--   0        0        0      506 2024-04-17 08:42:30.158894 sqlmodel_react_admin-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      190 2024-04-17 08:16:39.104617 sqlmodel_react_admin-0.0.3/sqlmodel_react_admin/client.py
--rw-r--r--   0        0        0      396 2024-04-17 07:51:08.677471 sqlmodel_react_admin-0.0.3/sqlmodel_react_admin/models.py
--rw-r--r--   0        0        0    17829 2024-04-17 08:41:14.326912 sqlmodel_react_admin-0.0.3/sqlmodel_react_admin/routers.py
--rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 sqlmodel_react_admin-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-17 07:50:51.516989 sqlmodel_react_admin-0.0.4/LICENSE
+-rw-r--r--   0        0        0      114 2024-04-17 07:53:35.781555 sqlmodel_react_admin-0.0.4/README.md
+-rw-r--r--   0        0        0      506 2024-04-17 08:51:03.875606 sqlmodel_react_admin-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      190 2024-04-17 08:16:39.104617 sqlmodel_react_admin-0.0.4/sqlmodel_react_admin/client.py
+-rw-r--r--   0        0        0      396 2024-04-17 07:51:08.677471 sqlmodel_react_admin-0.0.4/sqlmodel_react_admin/models.py
+-rw-r--r--   0        0        0    17683 2024-04-17 09:03:01.788016 sqlmodel_react_admin-0.0.4/sqlmodel_react_admin/routers.py
+-rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 sqlmodel_react_admin-0.0.4/PKG-INFO
```

### Comparing `sqlmodel_react_admin-0.0.3/LICENSE` & `sqlmodel_react_admin-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmodel_react_admin-0.0.3/sqlmodel_react_admin/routers.py` & `sqlmodel_react_admin-0.0.4/sqlmodel_react_admin/routers.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from sqlalchemy.orm import sessionmaker
 from sqlalchemy import func
 from sqlmodel_react_admin.client import get_async_client
 from sqlmodel.ext.asyncio.session import AsyncSession
 from fastapi.responses import StreamingResponse
 from starlette.background import BackgroundTask
 from typing import Any
-from typing import AsyncGenerator
 from uuid import UUID
 import json
 import httpx
 
 
 class ReactAdminRouter:
     def __init__(
@@ -113,20 +112,14 @@
             "/{id}",
             self.delete,
             methods=["DELETE"],
             name=f"Delete {a_or_an} {self.name_singular}",
             description=f"Delete a {self.name_singular} by its id",
         )
 
-    async def get_session(
-        self,
-    ) -> AsyncGenerator[AsyncSession, None]:
-        async with self.async_session() as session:
-            yield session
-
     @property
     def exact_match_fields(
         self,
     ) -> list[str]:
         """Returns a list of all the UUID fields in the model
 
         These cannot be performed with a likeness query and must have an
@@ -160,15 +153,15 @@
 
     async def update(
         self,
         id: UUID,
         request: Request,
     ) -> SQLModel:
 
-        async with self.get_session() as session:
+        async with self.async_session() as session:
             raw_body = await request.body()
             update_obj = self.update_model.model_validate(json.loads(raw_body))
             res = await session.exec(
                 select(self.db_model).where(self.db_model.id == id)
             )
             db_obj = res.one()
             update_fields = update_obj.model_dump(exclude_unset=True)
@@ -192,30 +185,30 @@
             return db_obj
 
     async def delete(
         self,
         id: UUID,
     ) -> None:
 
-        async with self.get_session() as session:
+        async with self.async_session() as session:
             res = await session.exec(
                 select(self.db_model).where(self.db_model.id == id)
             )
             obj = res.one_or_none()
 
             if obj:
                 await session.delete(obj)
                 await session.commit()
 
     async def create(
         self,
         request: Request,
     ) -> SQLModel:
 
-        async with self.get_session() as session:
+        async with self.async_session() as session:
             raw_body = await request.body()
             create_obj = self.create_model.model_validate(json.loads(raw_body))
             db_obj = self.db_model.model_validate(create_obj)
 
             session.add(db_obj)
             await session.commit()
             await session.refresh(db_obj)
@@ -224,15 +217,15 @@
 
     async def get_one(
         self,
         *,
         id: UUID,
     ) -> SQLModel:
 
-        async with self.get_session() as session:
+        async with self.async_session() as session:
             res = await session.exec(
                 select(self.db_model).where(self.db_model.id == id)
             )
             obj = res.one_or_none()
 
             return obj
 
@@ -240,15 +233,16 @@
         self,
         response: Response,
         filter: str = Query(None),
         sort: str = Query(None),
         range: str = Query(None),
     ) -> SQLModel:
 
-        async with self.get_session() as session:
+        async with self.async_session() as session:
+            session = self.async_session()
             sort = json.loads(sort) if sort else []
             range = json.loads(range) if range else []
             filter = json.loads(filter) if filter else {}
 
             query = select(self.db_model)
 
             # Do a query to satisfy total count for "Content-Range" header
```

### Comparing `sqlmodel_react_admin-0.0.3/PKG-INFO` & `sqlmodel_react_admin-0.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlmodel-react-admin
-Version: 0.0.3
+Version: 0.0.4
 Summary: Create fast SQLModel/FastAPI APIs/BFFs for React Admin
 License: MIT
 Author: Evan Thomas
 Author-email: evan@evanjt.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

