# Comparing `tmp/ampo-0.2.4.tar.gz` & `tmp/ampo-0.2.5.tar.gz`

## Comparing `ampo-0.2.4.tar` & `ampo-0.2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ampo-0.2.4/changelog.md
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 ampo-0.2.4/requirements.txt
--rwxr-xr-x   0        0        0      688 2020-02-02 00:00:00.000000 ampo-0.2.4/test.py
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 ampo-0.2.4/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 ampo-0.2.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 ampo-0.2.4/ampo/__init__.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 ampo-0.2.4/ampo/db.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 ampo-0.2.4/ampo/log.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 ampo-0.2.4/ampo/utils.py
--rw-r--r--   0        0        0     6217 2020-02-02 00:00:00.000000 ampo-0.2.4/ampo/worker.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ampo-0.2.4/.gitignore
--rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 ampo-0.2.4/README.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 ampo-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 ampo-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 ampo-0.2.5/changelog.md
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 ampo-0.2.5/requirements.txt
+-rwxr-xr-x   0        0        0      688 2020-02-02 00:00:00.000000 ampo-0.2.5/test.py
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 ampo-0.2.5/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 ampo-0.2.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 ampo-0.2.5/ampo/__init__.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 ampo-0.2.5/ampo/db.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 ampo-0.2.5/ampo/log.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 ampo-0.2.5/ampo/utils.py
+-rw-r--r--   0        0        0     6829 2020-02-02 00:00:00.000000 ampo-0.2.5/ampo/worker.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ampo-0.2.5/.gitignore
+-rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 ampo-0.2.5/README.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 ampo-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 ampo-0.2.5/PKG-INFO
```

### Comparing `ampo-0.2.4/changelog.md` & `ampo-0.2.5/changelog.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,24 @@
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 Types of changes: Added, Changed, Deprecated, Removed, Fixed, Security
 
 ## [Unreleased]
 
+## [0.2.5] - 2024-04-17
+
+### Added
+
+- The method 'expiration_index_skip' was added
+
+## Changed
+
+- The method 'update_expiration_value' was renamed to 'expiration_index_update'
+
 
 ## [0.2.4] - 2024-04-17
 
 ### Added
 
 - The Method 'count' was added
```

### Comparing `ampo-0.2.4/test.py` & `ampo-0.2.5/test.py`

 * *Files identical despite different names*

### Comparing `ampo-0.2.4/.github/workflows/python-package.yml` & `ampo-0.2.5/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `ampo-0.2.4/.github/workflows/python-publish.yml` & `ampo-0.2.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ampo-0.2.4/ampo/db.py` & `ampo-0.2.5/ampo/db.py`

 * *Files identical despite different names*

### Comparing `ampo-0.2.4/ampo/utils.py` & `ampo-0.2.5/ampo/utils.py`

 * *Files identical despite different names*

### Comparing `ampo-0.2.4/ampo/worker.py` & `ampo-0.2.5/ampo/worker.py`

 * *Files 7% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     @classmethod
     async def count(cls, **kwargs) -> int:
         """Return count of objects"""
         return await cls._get_collection().count_documents(
             CollectionWorker._prepea_filter_get(**kwargs))
 
     @classmethod
-    def update_expiration_value(
+    def expiration_index_update(
         cls: Type[T], field: str, expire_seconds: int
     ):
         """Update expire index for collections by field name
 
         Parameters
         ----------
         field : str
@@ -104,14 +104,33 @@
             if len(keys) != 1 or keys[0] != field:
                 continue
             index["options"]["expireAfterSeconds"] = expire_seconds
             return
         raise ValueError(f"The index by '{field}' not found")
 
     @classmethod
+    def expiration_index_skip(cls: Type[T], field: str):
+        """Skip index for collections by field name
+
+        Parameters
+        ----------
+        field : str
+            Name of field, for which index will be skipped
+        """
+        indexes = cls.model_config.get(cfg_orm_indexes, [])
+        for i, index in enumerate(indexes):
+            keys = index.get("keys", [])
+            if len(keys) != 1 or keys[0] != field:
+                continue
+            indexes: list
+            indexes.pop(i)
+            return
+        raise ValueError(f"The index by '{field}' not found")
+
+    @classmethod
     def _create_obj(cls, **kwargs):
         """
         Create object from database data
         """
         object_id = kwargs.pop("_id", None)
         if object_id is None:
             raise ValueError("Arguments don't have _id")
```

### Comparing `ampo-0.2.4/README.md` & `ampo-0.2.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -109,14 +109,15 @@
 # optional, set new value
 ModelA.update_expiration_value("field1", 20)
 
 await init_collection()
 ```
 
 if you want to set the 'expireAfterSeconds' only from method 'update_expiration_value', set it to '-1'.
+if you want skip the index changed, call method 'expiration_index_skip' before init_collection.
 
 ## Relationships between documents
 
 ### Embeded
 
 It is supported by default. Just, you need create the embedded document as class of pydantic - 'BaseModel'. It will be stored into db as object.
```

### Comparing `ampo-0.2.4/pyproject.toml` & `ampo-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ampo-0.2.4/PKG-INFO` & `ampo-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ampo
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python library async ORM for mongodb. Object as pyDantic
 Project-URL: Homepage, https://github.com/shizacat/ampo
 Author: Alexey Matveev
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -125,14 +125,15 @@
 # optional, set new value
 ModelA.update_expiration_value("field1", 20)
 
 await init_collection()
 ```
 
 if you want to set the 'expireAfterSeconds' only from method 'update_expiration_value', set it to '-1'.
+if you want skip the index changed, call method 'expiration_index_skip' before init_collection.
 
 ## Relationships between documents
 
 ### Embeded
 
 It is supported by default. Just, you need create the embedded document as class of pydantic - 'BaseModel'. It will be stored into db as object.
```

