# Comparing `tmp/bbm25_haystack-0.1.2.tar.gz` & `tmp/bbm25_haystack-0.1.3.tar.gz`

## Comparing `bbm25_haystack-0.1.2.tar` & `bbm25_haystack-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.2/.github/workflows/release.yml
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.2/.github/workflows/test.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.2/benchmarks/.gitkeep
--rw-r--r--   0        0        0     7092 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.2/scripts/benchmark_beir.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.2/src/bbm25_haystack/__about__.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.2/src/bbm25_haystack/__init__.py
--rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.2/src/bbm25_haystack/bbm25_retriever.py
--rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.2/src/bbm25_haystack/bbm25_store.py
--rw-r--r--   0        0        0   499723 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.2/src/bbm25_haystack/default.model
--rw-r--r--   0        0        0     8512 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.2/src/bbm25_haystack/filters.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.2/tests/test_document_store.py
--rw-r--r--   0        0        0     7523 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.2/tests/test_retriever.py
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.2/LICENSE
--rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.2/README.md
--rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/benchmarks/.gitkeep
+-rw-r--r--   0        0        0     7092 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/scripts/benchmark_beir.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/src/bbm25_haystack/__about__.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/src/bbm25_haystack/__init__.py
+-rw-r--r--   0        0        0     5128 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/src/bbm25_haystack/bbm25_retriever.py
+-rw-r--r--   0        0        0    11363 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/src/bbm25_haystack/bbm25_store.py
+-rw-r--r--   0        0        0   499723 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/src/bbm25_haystack/default.model
+-rw-r--r--   0        0        0     8512 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/src/bbm25_haystack/filters.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/tests/test_document_store.py
+-rw-r--r--   0        0        0     7623 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/tests/test_retriever.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/LICENSE
+-rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/README.md
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 bbm25_haystack-0.1.3/PKG-INFO
```

### Comparing `bbm25_haystack-0.1.2/.github/workflows/test.yml` & `bbm25_haystack-0.1.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `bbm25_haystack-0.1.2/scripts/benchmark_beir.py` & `bbm25_haystack-0.1.3/scripts/benchmark_beir.py`

 * *Files identical despite different names*

### Comparing `bbm25_haystack-0.1.2/src/bbm25_haystack/bbm25_retriever.py` & `bbm25_haystack-0.1.3/src/bbm25_haystack/bbm25_retriever.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,50 +48,59 @@
 
     def __init__(
         self,
         document_store: BetterBM25DocumentStore,
         *,
         filters: Optional[dict[str, Any]] = None,
         top_k: int = 10,
-    ):
+        set_score: bool = True,
+    ) -> None:
         """
         Create an BetterBM25Retriever component.
 
         :param document_store: A Document Store object used to
             retrieve documents
         :type document_store: BetterBM25DocumentStore
         :param filters: A dictionary with filters to narrow down the
             search space (default is None).
         :type filters: Optional[dict[str, Any]]
         :param top_k: The maximum number of documents to retrieve
             (default is 10).
         :type top_k: int
+        :param set_score: Whether to set the similarity scores
+            to retrieved documents (default is True).
+        :type set_score: bool
 
         :raises ValueError: If the specified top_k is not > 0.
         """
         _validate_search_params(filters, top_k)
 
         self.filters = filters
         self.top_k = top_k
+        self.set_score = set_score
 
         if not isinstance(document_store, BetterBM25DocumentStore):
             msg = "document_store must be an instance of BetterBM25DocumentStore"
             raise TypeError(msg)
         self.document_store = document_store
 
+    @component.output_types(documents=list[Document])
     def run(
         self,
         query: str,
         *,
         filters: Optional[dict[str, Any]] = None,
         top_k: Optional[int] = None,
     ) -> dict[str, list[Document]]:
         """
         Run the Retriever on the given query.
 
+        This method always return copies of the documents
+        retrieved from the document store.
+
         :param query: The query to run the Retriever on.
         :type query: str
         :param filters: A dictionary with filters to narrow
             down the search space (default is None).
         :type filters: Optional[dict[str, Any]]
         :param top_k: The maximum number of documents to
             retrieve (default is None).
@@ -100,27 +109,36 @@
         """
         filters = filters or self.filters
         top_k = top_k or self.top_k
 
         _validate_search_params(filters, top_k)
 
         sim = self.document_store._retrieval(query, filters=filters, top_k=top_k)
-        return {"documents": next(zip(*sim))}  # type: ignore
+
+        ret = []
+        for doc, score in sim:
+            data = doc.to_dict()
+            if self.set_score:
+                data["score"] = score
+            ret.append(Document.from_dict(data))
+
+        return {"documents": ret}
 
     def to_dict(self) -> dict[str, Any]:
         """
         Serializes the component to a dictionary.
 
         :return: dictionary with serialized data.
         """
         return default_to_dict(
             self,
             filters=self.filters,
             top_k=self.top_k,
             document_store=self.document_store.to_dict(),
+            set_score=self.set_score,
         )
 
     @classmethod
     def from_dict(cls, data: dict[str, Any]) -> "BetterBM25Retriever":
         """
         Deserializes the component from a dictionary.
```

### Comparing `bbm25_haystack-0.1.2/src/bbm25_haystack/bbm25_store.py` & `bbm25_haystack-0.1.3/src/bbm25_haystack/bbm25_store.py`

 * *Files identical despite different names*

### Comparing `bbm25_haystack-0.1.2/src/bbm25_haystack/default.model` & `bbm25_haystack-0.1.3/src/bbm25_haystack/default.model`

 * *Files identical despite different names*

### Comparing `bbm25_haystack-0.1.2/src/bbm25_haystack/filters.py` & `bbm25_haystack-0.1.3/src/bbm25_haystack/filters.py`

 * *Files identical despite different names*

### Comparing `bbm25_haystack-0.1.2/tests/test_document_store.py` & `bbm25_haystack-0.1.3/tests/test_document_store.py`

 * *Files identical despite different names*

### Comparing `bbm25_haystack-0.1.2/tests/test_retriever.py` & `bbm25_haystack-0.1.3/tests/test_retriever.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,33 +64,36 @@
             "init_parameters": {
                 "document_store": {
                     "type": "MyFakeStore",
                     "init_parameters": {},
                 },
                 "filters": None,
                 "top_k": 10,
+                "set_score": True,
             },
         }
 
     def test_to_dict_with_custom_init_parameters(self):
         ds = BetterBM25DocumentStore()
         serialized_ds = ds.to_dict()
 
         component = BetterBM25Retriever(
             document_store=BetterBM25DocumentStore(),
             filters={"name": "test.txt"},
             top_k=5,
+            set_score=False,
         )
         data = component.to_dict()
         assert data == {
             "type": "bbm25_haystack.bbm25_retriever.BetterBM25Retriever",
             "init_parameters": {
                 "document_store": serialized_ds,
                 "filters": {"name": "test.txt"},
                 "top_k": 5,
+                "set_score": False,
             },
         }
 
     def test_from_dict(self):
         data = {
             "type": "bbm25_haystack.bbm25_retriever.BetterBM25Retriever",
             "init_parameters": {
```

### Comparing `bbm25_haystack-0.1.2/.gitignore` & `bbm25_haystack-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `bbm25_haystack-0.1.2/LICENSE` & `bbm25_haystack-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bbm25_haystack-0.1.2/README.md` & `bbm25_haystack-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `bbm25_haystack-0.1.2/pyproject.toml` & `bbm25_haystack-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bbm25_haystack-0.1.2/PKG-INFO` & `bbm25_haystack-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bbm25-haystack
-Version: 0.1.2
+Version: 0.1.3
 Summary: Haystack 2.x In-memory Document Store with Enhanced Efficiency
 Project-URL: Documentation, https://github.com/Guest400123064/bbm25-haystack#readme
 Project-URL: Issues, https://github.com/Guest400123064/bbm25-haystack/issues
 Project-URL: Source, https://github.com/Guest400123064/bbm25-haystack
 Author-email: Yuxuan Wang <wangy49@seas.upenn.edu>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

