# Comparing `tmp/ampo-0.2.3.tar.gz` & `tmp/ampo-0.2.4.tar.gz`

## Comparing `ampo-0.2.3.tar` & `ampo-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 ampo-0.2.3/changelog.md
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 ampo-0.2.3/requirements.txt
--rwxr-xr-x   0        0        0      688 2020-02-02 00:00:00.000000 ampo-0.2.3/test.py
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 ampo-0.2.3/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 ampo-0.2.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 ampo-0.2.3/ampo/__init__.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 ampo-0.2.3/ampo/db.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 ampo-0.2.3/ampo/log.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 ampo-0.2.3/ampo/utils.py
--rw-r--r--   0        0        0     5999 2020-02-02 00:00:00.000000 ampo-0.2.3/ampo/worker.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ampo-0.2.3/.gitignore
--rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 ampo-0.2.3/README.md
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 ampo-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 ampo-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ampo-0.2.4/changelog.md
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 ampo-0.2.4/requirements.txt
+-rwxr-xr-x   0        0        0      688 2020-02-02 00:00:00.000000 ampo-0.2.4/test.py
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 ampo-0.2.4/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 ampo-0.2.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 ampo-0.2.4/ampo/__init__.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 ampo-0.2.4/ampo/db.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 ampo-0.2.4/ampo/log.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 ampo-0.2.4/ampo/utils.py
+-rw-r--r--   0        0        0     6217 2020-02-02 00:00:00.000000 ampo-0.2.4/ampo/worker.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ampo-0.2.4/.gitignore
+-rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 ampo-0.2.4/README.md
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 ampo-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 ampo-0.2.4/PKG-INFO
```

### Comparing `ampo-0.2.3/changelog.md` & `ampo-0.2.4/changelog.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 Types of changes: Added, Changed, Deprecated, Removed, Fixed, Security
 
 ## [Unreleased]
 
 
+## [0.2.4] - 2024-04-17
+
+### Added
+
+- The Method 'count' was added
+
+
 ## [0.2.3] - 2024-04-01
 
 ### Changed
 
 - The method 'db.AMPODatabase.get_db' is not longer a 'classmethod'
 
 ### Added
```

### Comparing `ampo-0.2.3/test.py` & `ampo-0.2.4/test.py`

 * *Files identical despite different names*

### Comparing `ampo-0.2.3/.github/workflows/python-package.yml` & `ampo-0.2.4/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `ampo-0.2.3/.github/workflows/python-publish.yml` & `ampo-0.2.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ampo-0.2.3/ampo/db.py` & `ampo-0.2.4/ampo/db.py`

 * *Files identical despite different names*

### Comparing `ampo-0.2.3/ampo/utils.py` & `ampo-0.2.4/ampo/utils.py`

 * *Files identical despite different names*

### Comparing `ampo-0.2.3/ampo/worker.py` & `ampo-0.2.4/ampo/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,20 @@
         """
         collection = self._get_collection()
         if self._id is None:
             raise ValueError("Object not created")
         await collection.delete_one({"_id": self._id})
 
     @classmethod
+    async def count(cls, **kwargs) -> int:
+        """Return count of objects"""
+        return await cls._get_collection().count_documents(
+            CollectionWorker._prepea_filter_get(**kwargs))
+
+    @classmethod
     def update_expiration_value(
         cls: Type[T], field: str, expire_seconds: int
     ):
         """Update expire index for collections by field name
 
         Parameters
         ----------
```

### Comparing `ampo-0.2.3/README.md` & `ampo-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `ampo-0.2.3/pyproject.toml` & `ampo-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ampo-0.2.3/PKG-INFO` & `ampo-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ampo
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python library async ORM for mongodb. Object as pyDantic
 Project-URL: Homepage, https://github.com/shizacat/ampo
 Author: Alexey Matveev
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

