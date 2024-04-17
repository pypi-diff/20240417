# Comparing `tmp/scgraph-1.5.1.tar.gz` & `tmp/scgraph-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scgraph-1.5.1.tar", last modified: Mon Mar  4 21:57:46 2024, max compression
+gzip compressed data, was "scgraph-1.5.2.tar", last modified: Wed Apr 17 18:08:15 2024, max compression
```

## Comparing `scgraph-1.5.1.tar` & `scgraph-1.5.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-03-04 21:57:46.455042 scgraph-1.5.1/
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)     1072 2023-04-14 17:06:21.000000 scgraph-1.5.1/LICENSE
--rw-r--r--   0 conmak    (1000) conmak    (1000)    10269 2024-03-04 21:57:46.455042 scgraph-1.5.1/PKG-INFO
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)     9647 2024-02-27 15:29:33.000000 scgraph-1.5.1/README.md
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      857 2024-03-04 21:51:48.000000 scgraph-1.5.1/pyproject.toml
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-03-04 21:57:46.447042 scgraph-1.5.1/scgraph/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       96 2023-09-15 15:24:50.000000 scgraph-1.5.1/scgraph/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    33354 2023-09-21 11:44:59.000000 scgraph-1.5.1/scgraph/core.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-03-04 21:57:46.451042 scgraph-1.5.1/scgraph/geographs/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        0 2023-09-15 15:24:50.000000 scgraph-1.5.1/scgraph/geographs/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)  1143112 2024-03-04 21:44:33.000000 scgraph-1.5.1/scgraph/geographs/marnet.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)   923120 2024-03-04 21:46:50.000000 scgraph-1.5.1/scgraph/geographs/north_america_rail.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)   976574 2024-03-04 21:47:47.000000 scgraph-1.5.1/scgraph/geographs/oak_ridge_maritime.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)  1414756 2024-03-04 21:48:18.000000 scgraph-1.5.1/scgraph/geographs/us_freeway.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     3946 2024-02-27 15:33:35.000000 scgraph-1.5.1/scgraph/utils.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-03-04 21:57:46.455042 scgraph-1.5.1/scgraph.egg-info/
--rw-r--r--   0 conmak    (1000) conmak    (1000)    10269 2024-03-04 21:57:46.000000 scgraph-1.5.1/scgraph.egg-info/PKG-INFO
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      389 2024-03-04 21:57:46.000000 scgraph-1.5.1/scgraph.egg-info/SOURCES.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2024-03-04 21:57:46.000000 scgraph-1.5.1/scgraph.egg-info/dependency_links.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        8 2024-03-04 21:57:46.000000 scgraph-1.5.1/scgraph.egg-info/top_level.txt
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      138 2024-03-04 21:57:46.455042 scgraph-1.5.1/setup.cfg
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-17 18:08:15.314331 scgraph-1.5.2/
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)     1072 2023-04-14 17:06:21.000000 scgraph-1.5.2/LICENSE
+-rw-r--r--   0 conmak    (1000) conmak    (1000)    10269 2024-04-17 18:08:15.314331 scgraph-1.5.2/PKG-INFO
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)     9647 2024-02-27 15:29:33.000000 scgraph-1.5.2/README.md
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      857 2024-04-17 16:57:16.000000 scgraph-1.5.2/pyproject.toml
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-17 18:08:15.306331 scgraph-1.5.2/scgraph/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       96 2023-09-15 15:24:50.000000 scgraph-1.5.2/scgraph/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    33414 2024-04-17 17:55:15.000000 scgraph-1.5.2/scgraph/core.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-17 18:08:15.310331 scgraph-1.5.2/scgraph/geographs/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        0 2023-09-15 15:24:50.000000 scgraph-1.5.2/scgraph/geographs/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)  1143112 2024-03-04 21:44:33.000000 scgraph-1.5.2/scgraph/geographs/marnet.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)   923120 2024-03-04 21:46:50.000000 scgraph-1.5.2/scgraph/geographs/north_america_rail.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)   976574 2024-03-04 21:47:47.000000 scgraph-1.5.2/scgraph/geographs/oak_ridge_maritime.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)  1414756 2024-03-04 21:48:18.000000 scgraph-1.5.2/scgraph/geographs/us_freeway.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     3946 2024-02-27 15:33:35.000000 scgraph-1.5.2/scgraph/utils.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-17 18:08:15.314331 scgraph-1.5.2/scgraph.egg-info/
+-rw-r--r--   0 conmak    (1000) conmak    (1000)    10269 2024-04-17 18:08:15.000000 scgraph-1.5.2/scgraph.egg-info/PKG-INFO
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      389 2024-04-17 18:08:15.000000 scgraph-1.5.2/scgraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2024-04-17 18:08:15.000000 scgraph-1.5.2/scgraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        8 2024-04-17 18:08:15.000000 scgraph-1.5.2/scgraph.egg-info/top_level.txt
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      138 2024-04-17 18:08:15.314331 scgraph-1.5.2/setup.cfg
```

### Comparing `scgraph-1.5.1/LICENSE` & `scgraph-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scgraph-1.5.1/PKG-INFO` & `scgraph-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scgraph
-Version: 1.5.1
+Version: 1.5.2
 Summary: Determine an approximate route between two points on earth.
 Author-email: Connor Makowski <conmak@mit.edu>
 Project-URL: Homepage, https://github.com/connor-makowski/scgraph
 Project-URL: Bug Tracker, https://github.com/connor-makowski/scgraph/issues
 Project-URL: Documentation, https://connor-makowski.github.io/scgraph/core.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `scgraph-1.5.1/README.md` & `scgraph-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `scgraph-1.5.1/pyproject.toml` & `scgraph-1.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scgraph"
-version = "1.5.1"
+version = "1.5.2"
 description = "Determine an approximate route between two points on earth."
 authors = [
     {name="Connor Makowski", email="conmak@mit.edu"}
 ]
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `scgraph-1.5.1/scgraph/core.py` & `scgraph-1.5.2/scgraph/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -670,38 +670,39 @@
         assert circuity > 0, "Circuity must be greater than 0"
         assert node_addition_type in [
             "quadrant",
             "all",
             "closest",
         ], f"Invalid node addition type provided ({node_addition_type}), valid options are: ['quadrant', 'all', 'closest']"
 
-        # Create the node
-        new_node_id = max(self.graph) + 1
-        self.nodes[new_node_id] = node
-        self.graph[new_node_id] = {}
-
+        # Get the distances to all other nodes
         distances = {
             node_i_id: {
                 "distance": round(
                     haversine(node, node_i, circuity=circuity), 4
                 ),
                 "quadrant": (
                     "n" if node["latitude"] > node_i["latitude"] else "s"
                 )
                 + ("e" if node["longitude"] > node_i["longitude"] else "w"),
             }
             for node_i_id, node_i in self.nodes.items()
         }
 
+        # Create the node
+        new_node_id = max(self.graph) + 1
+        self.nodes[new_node_id] = node
+        self.graph[new_node_id] = {}
+
         if node_addition_type == "all":
-            for node_i_id, node_i in self.nodes.items():
-                self.graph[new_node_id][node_i_id] = distances[node_i_id][
+            for node_i_id, node_i_distnace_dict in distances.items():
+                self.graph[new_node_id][node_i_id] = node_i_distnace_dict[
                     "distance"
                 ]
-                self.graph[node_i_id][new_node_id] = distances[node_i_id][
+                self.graph[node_i_id][new_node_id] = node_i_distnace_dict[
                     "distance"
                 ]
         elif node_addition_type == "closest":
             min_node_id = min(distances, key=lambda x: distances[x]["distance"])
             self.graph[new_node_id][min_node_id] = distances[min_node_id][
                 "distance"
             ]
```

### Comparing `scgraph-1.5.1/scgraph/geographs/marnet.py` & `scgraph-1.5.2/scgraph/geographs/marnet.py`

 * *Files identical despite different names*

### Comparing `scgraph-1.5.1/scgraph/geographs/north_america_rail.py` & `scgraph-1.5.2/scgraph/geographs/north_america_rail.py`

 * *Files identical despite different names*

### Comparing `scgraph-1.5.1/scgraph/geographs/oak_ridge_maritime.py` & `scgraph-1.5.2/scgraph/geographs/oak_ridge_maritime.py`

 * *Files identical despite different names*

### Comparing `scgraph-1.5.1/scgraph/geographs/us_freeway.py` & `scgraph-1.5.2/scgraph/geographs/us_freeway.py`

 * *Files identical despite different names*

### Comparing `scgraph-1.5.1/scgraph/utils.py` & `scgraph-1.5.2/scgraph/utils.py`

 * *Files identical despite different names*

### Comparing `scgraph-1.5.1/scgraph.egg-info/PKG-INFO` & `scgraph-1.5.2/scgraph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scgraph
-Version: 1.5.1
+Version: 1.5.2
 Summary: Determine an approximate route between two points on earth.
 Author-email: Connor Makowski <conmak@mit.edu>
 Project-URL: Homepage, https://github.com/connor-makowski/scgraph
 Project-URL: Bug Tracker, https://github.com/connor-makowski/scgraph/issues
 Project-URL: Documentation, https://connor-makowski.github.io/scgraph/core.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

