# Comparing `tmp/hyperon_das_atomdb-0.6.4.tar.gz` & `tmp/hyperon_das_atomdb-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperon_das_atomdb-0.6.4.tar", max compression
+gzip compressed data, was "hyperon_das_atomdb-0.6.5.tar", max compression
```

## Comparing `hyperon_das_atomdb-0.6.4.tar` & `hyperon_das_atomdb-0.6.5.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0     1081 2024-04-05 20:46:52.669988 hyperon_das_atomdb-0.6.4/LICENCE
--rw-r--r--   0        0        0     2687 2024-04-05 20:46:52.673987 hyperon_das_atomdb-0.6.4/README.md
--rw-r--r--   0        0        0      306 2024-04-05 20:46:52.673987 hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/__init__.py
--rw-r--r--   0        0        0      116 2024-04-05 20:46:52.673987 hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/adapters/__init__.py
--rw-r--r--   0        0        0    20238 2024-04-05 20:46:52.673987 hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/adapters/ram_only.py
--rw-r--r--   0        0        0    36861 2024-04-05 20:46:52.673987 hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/adapters/redis_mongo_db.py
--rw-r--r--   0        0        0    19708 2024-04-05 20:46:52.677987 hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/database.py
--rw-r--r--   0        0        0      877 2024-04-05 20:46:52.677987 hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/exceptions.py
--rw-r--r--   0        0        0     1122 2024-04-05 20:46:52.677987 hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/index.py
--rw-r--r--   0        0        0     1052 2024-04-05 20:46:52.677987 hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/logger.py
--rw-r--r--   0        0        0        0 2024-04-05 20:46:52.677987 hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/utils/__init__.py
--rw-r--r--   0        0        0     1947 2024-04-05 20:46:52.677987 hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/utils/expression_hasher.py
--rw-r--r--   0        0        0     1388 2024-04-05 20:46:52.677987 hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/utils/patterns.py
--rw-r--r--   0        0        0       65 2024-04-05 20:46:52.677987 hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/utils/settings.py
--rw-r--r--   0        0        0     1161 2024-04-05 20:47:02.089933 hyperon_das_atomdb-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     3605 1970-01-01 00:00:00.000000 hyperon_das_atomdb-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-17 12:50:59.446086 hyperon_das_atomdb-0.6.5/LICENCE
+-rw-r--r--   0        0        0     2687 2024-04-17 12:50:59.446086 hyperon_das_atomdb-0.6.5/README.md
+-rw-r--r--   0        0        0      306 2024-04-17 12:50:59.446086 hyperon_das_atomdb-0.6.5/hyperon_das_atomdb/__init__.py
+-rw-r--r--   0        0        0      194 2024-04-17 12:50:59.446086 hyperon_das_atomdb-0.6.5/hyperon_das_atomdb/adapters/__init__.py
+-rw-r--r--   0        0        0    20557 2024-04-17 12:50:59.446086 hyperon_das_atomdb-0.6.5/hyperon_das_atomdb/adapters/ram_only.py
+-rw-r--r--   0        0        0    37055 2024-04-17 12:50:59.450086 hyperon_das_atomdb-0.6.5/hyperon_das_atomdb/adapters/redis_mongo_db.py
+-rw-r--r--   0        0        0    12546 2024-04-17 12:50:59.450086 hyperon_das_atomdb-0.6.5/hyperon_das_atomdb/adapters/redis_postgreslobe_db.py
+-rw-r--r--   0        0        0    19820 2024-04-17 12:50:59.450086 hyperon_das_atomdb-0.6.5/hyperon_das_atomdb/database.py
+-rw-r--r--   0        0        0      939 2024-04-17 12:50:59.450086 hyperon_das_atomdb-0.6.5/hyperon_das_atomdb/exceptions.py
+-rw-r--r--   0        0        0     1122 2024-04-17 12:50:59.450086 hyperon_das_atomdb-0.6.5/hyperon_das_atomdb/index.py
+-rw-r--r--   0        0        0     1052 2024-04-17 12:50:59.450086 hyperon_das_atomdb-0.6.5/hyperon_das_atomdb/logger.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:50:59.450086 hyperon_das_atomdb-0.6.5/hyperon_das_atomdb/utils/__init__.py
+-rw-r--r--   0        0        0     1947 2024-04-17 12:50:59.450086 hyperon_das_atomdb-0.6.5/hyperon_das_atomdb/utils/expression_hasher.py
+-rw-r--r--   0        0        0     5695 2024-04-17 12:50:59.450086 hyperon_das_atomdb-0.6.5/hyperon_das_atomdb/utils/mapper.py
+-rw-r--r--   0        0        0     1388 2024-04-17 12:50:59.450086 hyperon_das_atomdb-0.6.5/hyperon_das_atomdb/utils/patterns.py
+-rw-r--r--   0        0        0       65 2024-04-17 12:50:59.450086 hyperon_das_atomdb-0.6.5/hyperon_das_atomdb/utils/settings.py
+-rw-r--r--   0        0        0     1134 2024-04-17 12:51:09.018113 hyperon_das_atomdb-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     3557 1970-01-01 00:00:00.000000 hyperon_das_atomdb-0.6.5/PKG-INFO
```

### Comparing `hyperon_das_atomdb-0.6.4/LICENCE` & `hyperon_das_atomdb-0.6.5/LICENCE`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.4/README.md` & `hyperon_das_atomdb-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/adapters/ram_only.py` & `hyperon_das_atomdb-0.6.5/hyperon_das_atomdb/adapters/ram_only.py`

 * *Files 2% similar despite different names*

```diff
@@ -522,7 +522,16 @@
                     self.db.node[handle] = document
                 else:
                     self.db.link[handle] = document
                 self._update_index(document)
         except Exception:
             logger().error("Error bulk inserting documents")
             return None
+
+    def retrieve_all_atoms(self) -> List[Dict[str, Any]]:
+        try:
+            answer = list(self.db.node.items())
+            answer.extend(list(self.db.link.items()))
+            return answer
+        except Exception as e:
+            logger().error(f"Error retrieving all atoms: {str(e)}")
+            raise e
```

### Comparing `hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/adapters/redis_mongo_db.py` & `hyperon_das_atomdb-0.6.5/hyperon_das_atomdb/adapters/redis_mongo_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,34 +278,34 @@
         #      of this lazy hashmap, we should load the hashmap during prefetch
         named_type_hash = self.named_type_hash.get(atom_type, None)
         if named_type_hash is None:
             named_type_hash = ExpressionHasher.named_type_hash(atom_type)
             self.named_type_hash[atom_type] = named_type_hash
         return named_type_hash
 
-    def _retrieve_mongo_document(self, handle: str) -> dict:
+    def _retrieve_document(self, handle: str) -> dict:
         mongo_filter = {MongoFieldNames.ID_HASH: handle}
         document = self.mongo_atoms_collection.find_one(mongo_filter)
         if document := self.mongo_atoms_collection.find_one(mongo_filter):
             if self._is_document_link(document):
-                document["targets"] = self._get_mongo_document_keys(document)
+                document["targets"] = self._get_document_keys(document)
             return document
         return None
 
     def _build_named_type_hash_template(self, template: Union[str, List[Any]]) -> List[Any]:
         if isinstance(template, str):
             return self._get_atom_type_hash(template)
         else:
             answer = []
             for element in template:
                 v = self._build_named_type_hash_template(element)
                 answer.append(v)
             return answer
 
-    def _get_mongo_document_keys(self, document: Dict) -> List[str]:
+    def _get_document_keys(self, document: Dict) -> List[str]:
         answer = document.get(MongoFieldNames.KEYS, None)
         if answer is not None:
             return answer
         answer = []
         index = 0
         while True:
             key = document.get(f"{MongoFieldNames.KEY_PREFIX.value}_{index}", None)
@@ -318,22 +318,22 @@
     def _filter_non_toplevel(self, matches: list) -> list:
         matches_toplevel_only = []
         if len(matches) > 0:
             # if isinstance(matches[0], list):
             #    matches = matches[0]
             for match in matches:
                 link_handle = match[0]
-                link = self._retrieve_mongo_document(link_handle)
+                link = self._retrieve_document(link_handle)
                 if link['is_toplevel']:
                     matches_toplevel_only.append(match)
         return matches_toplevel_only
 
     def get_node_handle(self, node_type: str, node_name: str) -> str:
         node_handle = self.node_handle(node_type, node_name)
-        document = self._retrieve_mongo_document(node_handle)
+        document = self._retrieve_document(node_handle)
         if document is not None:
             return document[MongoFieldNames.ID_HASH]
         else:
             logger().error(
                 f'Failed to retrieve node handle for {node_type}:{node_name}. This node may not exist.'
             )
             raise NodeDoesNotExist(
@@ -386,15 +386,15 @@
         documents = self.mongo_atoms_collection.find({MongoFieldNames.TYPE_NAME: link_type})
         for document in documents:
             links_handle.append(document[MongoFieldNames.ID_HASH])
         return links_handle
 
     def get_link_handle(self, link_type: str, target_handles: List[str]) -> str:
         link_handle = self.link_handle(link_type, target_handles)
-        document = self._retrieve_mongo_document(link_handle)
+        document = self._retrieve_document(link_handle)
         if document is not None:
             return document[MongoFieldNames.ID_HASH]
         else:
             logger().error(
                 f'Failed to retrieve link handle for {link_type}:{target_handles}. This link may not exist.'
             )
             raise LinkDoesNotExist(
@@ -408,15 +408,15 @@
             logger().error(
                 f'Failed to retrieve link targets for handle: {link_handle}. The handle may be invalid or the corresponding link does not exist.'
             )
             raise ValueError(f"Invalid handle: {link_handle}")
         return answer
 
     def is_ordered(self, link_handle: str) -> bool:
-        document = self._retrieve_mongo_document(link_handle)
+        document = self._retrieve_document(link_handle)
         if document is None:
             logger().error(
                 'Failed to retrieve document for link handle: {link_handle}. The handle may be invalid or the corresponding link does not exist.'
             )
             raise ValueError(f"Invalid handle: {link_handle}")
         return True
 
@@ -486,15 +486,15 @@
         return self._process_matched_results(templates_matched, cursor, toplevel_only)
 
     def get_link_type(self, link_handle: str) -> str:
         document = self.get_atom(link_handle)
         return document[MongoFieldNames.TYPE_NAME]
 
     def get_atom(self, handle: str, **kwargs) -> Dict[str, Any]:
-        document = self._retrieve_mongo_document(handle)
+        document = self._retrieve_document(handle)
         if document:
             if not kwargs.get('no_target_format', False):
                 return self._transform_to_target_format(document, **kwargs)
             else:
                 return document
         else:
             logger().error(
@@ -502,21 +502,21 @@
             )
             raise AtomDoesNotExist(
                 message='Nonexistent atom',
                 details=f'handle: {handle}',
             )
 
     def get_atom_type(self, handle: str) -> str:
-        atom = self._retrieve_mongo_document(handle)
+        atom = self._retrieve_document(handle)
         if atom is not None:
             return atom['named_type']
 
     def get_atom_as_dict(self, handle) -> dict:
         answer = {}
-        document = self._retrieve_mongo_document(handle)
+        document = self._retrieve_document(handle)
         if document:
             answer["handle"] = document[MongoFieldNames.ID_HASH]
             answer["type"] = document[MongoFieldNames.TYPE_NAME]
             if "targets" in document:
                 answer["targets"] = document["targets"]
             else:
                 answer["name"] = document["name"]
@@ -730,15 +730,15 @@
                 for document in documents:
                     self._update_link_index(document, delete_atom=True)
         else:
             self.redis.set(key, node_name)
 
     def _update_link_index(self, document: Dict[str, Any], **kwargs) -> None:
         handle = document[MongoFieldNames.ID_HASH]
-        targets = self._get_mongo_document_keys(document)
+        targets = self._get_document_keys(document)
         targets_str = "".join(targets)
         arity = len(targets)
         named_type = document[MongoFieldNames.TYPE_NAME]
         named_type_hash = document[MongoFieldNames.TYPE_NAME_HASH]
         value = f"{handle}{targets_str}"
 
         if self.pattern_index_templates:
@@ -815,15 +815,15 @@
                 else:
                     response.append(ExpressionHasher.named_type_hash(type))
             return response
 
         composite_type_hashes_list = calculate_composite_type_hashes(composite_type)
         return ExpressionHasher.composite_hash(composite_type_hashes_list)
 
-    def _retrieve_mongo_documents_by_index(
+    def _retrieve_documents_by_index(
         self, collection: Collection, index_id: str, **kwargs
     ) -> Tuple[int, List[Dict[str, Any]]]:
         if MongoDBIndex(collection).index_exists(index_id):
             cursor = kwargs.pop('cursor', None)
             chunk_size = kwargs.pop('chunk_size', 500)
 
             try:
@@ -918,23 +918,30 @@
                     else "Index creation failed"
                 )
 
         return index_id
 
     def get_atoms_by_index(self, index_id: str, **kwargs) -> Union[Tuple[int, list], list]:
         try:
-            documents = self._retrieve_mongo_documents_by_index(
+            documents = self._retrieve_documents_by_index(
                 self.mongo_atoms_collection, index_id, **kwargs
             )
             cursor, documents = documents
             return cursor, [self.get_atom(document['_id']) for document in documents]
         except Exception as e:
             logger().error(f"Error retrieving atoms by index: {str(e)}")
             raise e
 
+    def retrieve_all_atoms(self) -> List[Dict[str, Any]]:
+        try:
+            return [document for document in self.mongo_atoms_collection.find()]
+        except Exception as e:
+            logger().error(f"Error retrieving all atoms: {str(e)}")
+            raise e
+
     def bulk_insert(self, documents: List[Dict[str, Any]]) -> None:
         try:
             _id = MongoFieldNames.ID_HASH
             [
                 self.mongo_atoms_collection.replace_one({_id: document[_id]}, document, upsert=True)
                 for document in documents
             ]
```

### Comparing `hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/database.py` & `hyperon_das_atomdb-0.6.5/hyperon_das_atomdb/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,25 +122,27 @@
             )
 
         link_type_hash = ExpressionHasher.named_type_hash(link_type)
 
         targets_hash = []
         composite_type = [link_type_hash]
         composite_type_hash = [link_type_hash]
+
         for target in targets:
             if 'targets' not in target.keys():
                 atom = self.add_node(target)
                 atom_hash = ExpressionHasher.named_type_hash(atom['named_type'])
                 composite_type.append(atom_hash)
             else:
                 atom = self.add_link(target, toplevel=False)
                 composite_type.append(atom['composite_type'])
                 atom_hash = atom['composite_type_hash']
             composite_type_hash.append(atom_hash)
             targets_hash.append(atom['_id'])
+
         handle = ExpressionHasher.expression_hash(link_type_hash, targets_hash)
 
         arity = len(targets)
         link = {
             '_id': handle,
             'composite_type_hash': ExpressionHasher.composite_hash(composite_type_hash),
             'is_toplevel': toplevel,
@@ -602,7 +604,11 @@
         composite_type: Optional[List[Any]] = None,
     ) -> str:
         ...  # pragma no cover
 
     @abstractmethod
     def bulk_insert(self, documents: List[Dict[str, Any]]) -> None:
         ...  # pragma no cover
+
+    @abstractmethod
+    def retrieve_all_atoms(self) -> List[Dict[str, Any]]:
+        ...  # pragma no cover
```

### Comparing `hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/exceptions.py` & `hyperon_das_atomdb-0.6.5/hyperon_das_atomdb/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,7 +40,11 @@
 
 class RetryException(BaseException):
     ...  # pragma no cover
 
 
 class InvalidAtomDB(BaseException):
     ...  # pragma no cover
+
+
+class InvalidSQL(BaseException):
+    ...  # pragma no cover
```

### Comparing `hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/index.py` & `hyperon_das_atomdb-0.6.5/hyperon_das_atomdb/index.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/logger.py` & `hyperon_das_atomdb-0.6.5/hyperon_das_atomdb/logger.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/utils/expression_hasher.py` & `hyperon_das_atomdb-0.6.5/hyperon_das_atomdb/utils/expression_hasher.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.4/hyperon_das_atomdb/utils/patterns.py` & `hyperon_das_atomdb-0.6.5/hyperon_das_atomdb/utils/patterns.py`

 * *Files identical despite different names*

### Comparing `hyperon_das_atomdb-0.6.4/pyproject.toml` & `hyperon_das_atomdb-0.6.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 [tool.poetry]
 name = "hyperon-das-atomdb"
-version = "0.6.4"
+version = "0.6.5"
 description = "Persistence layer for Distributed AtomSpace"
 authors = ["marcocapozzoli <marcocapozzoli90@gmail.com>"]
 readme = "README.md"
 packages = [{include = "hyperon_das_atomdb"}]
 
 [tool.poetry.urls]
 "Code" = "https://github.com/singnet/das-atom-db"
 "Bug Tracker" = "https://github.com/singnet/das-atom-db/issues"
 "Releases" = "https://github.com/singnet/das-atom-db/releases"
 
 [tool.poetry.dependencies]
 python = "^3.8.5"
 redis = "^5.0.0"
 pymongo = "^4.5.0"
-requests = "^2.31.0"
-requests-mock = "^1.11.0"
 python-dotenv = "^1.0.0"
+psycopg2 = "^2.9.9"
 
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.1.0"
 isort = "^5.12.0"
 black = "^23.7.0"
 pytest = "^7.4.2"
```

### Comparing `hyperon_das_atomdb-0.6.4/PKG-INFO` & `hyperon_das_atomdb-0.6.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: hyperon-das-atomdb
-Version: 0.6.4
+Version: 0.6.5
 Summary: Persistence layer for Distributed AtomSpace
 Author: marcocapozzoli
 Author-email: marcocapozzoli90@gmail.com
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: psycopg2 (>=2.9.9,<3.0.0)
 Requires-Dist: pymongo (>=4.5.0,<5.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: redis (>=5.0.0,<6.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: requests-mock (>=1.11.0,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/singnet/das-atom-db/issues
 Project-URL: Code, https://github.com/singnet/das-atom-db
 Project-URL: Releases, https://github.com/singnet/das-atom-db/releases
 Description-Content-Type: text/markdown
 
 # Hyperon DAS AtomDB
```

