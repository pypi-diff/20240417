# Comparing `tmp/relation_validator-0.5.0.tar.gz` & `tmp/relation_validator-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relation_validator-0.5.0.tar", max compression
+gzip compressed data, was "relation_validator-0.5.1.tar", max compression
```

## Comparing `relation_validator-0.5.0.tar` & `relation_validator-0.5.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-04-13 10:51:27.886165 relation_validator-0.5.0/LICENSE
--rw-r--r--   0        0        0     3378 2024-03-05 14:56:24.694753 relation_validator-0.5.0/README.md
--rw-r--r--   0        0        0      634 2024-03-05 15:38:01.316892 relation_validator-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-13 10:51:27.888196 relation_validator-0.5.0/src/relation_validator/__init__.py
--rw-r--r--   0        0        0     1335 2024-01-26 14:16:12.324379 relation_validator-0.5.0/src/relation_validator/__main__.py
--rw-r--r--   0        0        0       64 2024-01-31 19:20:41.384974 relation_validator-0.5.0/src/relation_validator/conf/__init__.py
--rw-r--r--   0        0        0     3501 2024-01-31 12:47:05.067412 relation_validator-0.5.0/src/relation_validator/conf/obograph-style.json
--rw-r--r--   0        0        0        0 2023-04-13 10:51:27.888431 relation_validator-0.5.0/src/relation_validator/utils/__init__.py
--rw-r--r--   0        0        0     5390 2024-03-05 14:37:20.137381 relation_validator-0.5.0/src/relation_validator/utils/utils.py
--rw-r--r--   0        0        0     1803 2024-03-05 14:38:39.905088 relation_validator-0.5.0/src/relation_validator/validator.py
--rw-r--r--   0        0        0     4179 1970-01-01 00:00:00.000000 relation_validator-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-13 10:51:27.886165 relation_validator-0.5.1/LICENSE
+-rw-r--r--   0        0        0     3378 2024-03-05 14:56:24.694753 relation_validator-0.5.1/README.md
+-rw-r--r--   0        0        0      634 2024-04-17 14:04:25.796246 relation_validator-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-13 10:51:27.888196 relation_validator-0.5.1/src/relation_validator/__init__.py
+-rw-r--r--   0        0        0     1335 2024-01-26 14:16:12.324379 relation_validator-0.5.1/src/relation_validator/__main__.py
+-rw-r--r--   0        0        0       64 2024-01-31 19:20:41.384974 relation_validator-0.5.1/src/relation_validator/conf/__init__.py
+-rw-r--r--   0        0        0     3501 2024-04-17 12:31:00.197193 relation_validator-0.5.1/src/relation_validator/conf/obograph-style.json
+-rw-r--r--   0        0        0        0 2023-04-13 10:51:27.888431 relation_validator-0.5.1/src/relation_validator/utils/__init__.py
+-rw-r--r--   0        0        0     5583 2024-04-17 13:51:06.172161 relation_validator-0.5.1/src/relation_validator/utils/utils.py
+-rw-r--r--   0        0        0     1828 2024-04-17 13:42:53.613924 relation_validator-0.5.1/src/relation_validator/validator.py
+-rw-r--r--   0        0        0     4179 1970-01-01 00:00:00.000000 relation_validator-0.5.1/PKG-INFO
```

### Comparing `relation_validator-0.5.0/LICENSE` & `relation_validator-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `relation_validator-0.5.0/README.md` & `relation_validator-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `relation_validator-0.5.0/pyproject.toml` & `relation_validator-0.5.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "relation-validator"
-version = "0.5.0"
+version = "0.5.1"
 description = "This package validates a list of relationships between two terms against the specified ontologies."
 authors = ["Anita Caron <anitac@ebi.ac.uk>"]
 readme = "README.md"
 packages = [{include = "relation_validator", from="src"}]
 repository = "https://github.com/INCATools/relation-validator"
 
 [tool.poetry.dependencies]
```

### Comparing `relation_validator-0.5.0/src/relation_validator/__main__.py` & `relation_validator-0.5.1/src/relation_validator/__main__.py`

 * *Files identical despite different names*

### Comparing `relation_validator-0.5.0/src/relation_validator/conf/obograph-style.json` & `relation_validator-0.5.1/src/relation_validator/conf/obograph-style.json`

 * *Files identical despite different names*

### Comparing `relation_validator-0.5.0/src/relation_validator/utils/utils.py` & `relation_validator-0.5.1/src/relation_validator/utils/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -159,27 +159,31 @@
 
     response = query_ubergraph(QUERY_VERSION)
     return response
 
 
 def get_obograph(
     rel_terms: Dict[str, List[Tuple[str, str]]],
-    labels: Dict[str, str]
+    labels: Dict[str, str],
+    properties: Dict[str, str]
 ) -> Graph:
     """
     Transform graph into OBOGgraph
     """
     edges = []
     nodes = {}
+    properties_ = {v: k for k, v in properties.items()}
 
     for rel, terms in rel_terms.items():
         for sub, obj in terms:
             edges.append(Edge(sub=sub, pred=rel, obj=obj))
             nodes[sub] = Node(id=sub, lbl=labels[sub])
             nodes[obj] = Node(id=obj, lbl=labels[obj])
+            if "not_matched" not in rel:
+                nodes[rel] = Node(id=rel, lbl=properties_[rel])
 
     return Graph(id="valid", nodes=list(nodes.values()), edges=edges)
 
 
 def save_obograph(
     graph: Graph,
     output: Path,
```

### Comparing `relation_validator-0.5.0/src/relation_validator/validator.py` & `relation_validator-0.5.1/src/relation_validator/validator.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     report, rel_terms = run_validation(data, config["relationships"])
 
     output_filename = args.output
     _, sep = tsv_or_csv(output_filename)
     report.to_csv(output_filename, sep=sep, index=False)
 
     labels = get_labels(data)
-    graph = get_obograph(rel_terms, labels)
+    graph = get_obograph(rel_terms, labels, config["relationships"])
     save_obograph(graph, f"{temp_filename}.png")
     return True
 
 
 def ontologies_version(args):
     """
     Get ontologies' version
```

### Comparing `relation_validator-0.5.0/PKG-INFO` & `relation_validator-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relation-validator
-Version: 0.5.0
+Version: 0.5.1
 Summary: This package validates a list of relationships between two terms against the specified ontologies.
 Home-page: https://github.com/INCATools/relation-validator
 Author: Anita Caron
 Author-email: anitac@ebi.ac.uk
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

