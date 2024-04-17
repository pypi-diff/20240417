# Comparing `tmp/jageocoder-2.1.4.tar.gz` & `tmp/jageocoder-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jageocoder-2.1.4.tar", max compression
+gzip compressed data, was "jageocoder-2.1.5.tar", max compression
```

## Comparing `jageocoder-2.1.4.tar` & `jageocoder-2.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      113 2023-08-03 02:25:59.197434 jageocoder-2.1.4/LICENSE
--rw-r--r--   0        0        0     8253 2023-08-03 02:25:59.197434 jageocoder-2.1.4/README.md
--rw-r--r--   0        0        0     1364 2024-04-13 05:06:33.848811 jageocoder-2.1.4/jageocoder/__init__.py
--rw-r--r--   0        0        0     5605 2023-09-27 08:08:26.315234 jageocoder-2.1.4/jageocoder/__main__.py
--rw-r--r--   0        0        0     2574 2023-08-03 02:25:59.209435 jageocoder-2.1.4/jageocoder/address.py
--rw-r--r--   0        0        0     1421 2023-08-03 02:25:59.209435 jageocoder-2.1.4/jageocoder/aliases.json
--rw-r--r--   0        0        0     8320 2024-04-10 08:33:59.049176 jageocoder-2.1.4/jageocoder/aza_master.py
--rw-r--r--   0        0        0     1171 2023-08-03 02:25:59.209435 jageocoder-2.1.4/jageocoder/dataset.py
--rw-r--r--   0        0        0      691 2023-08-03 02:25:59.209435 jageocoder-2.1.4/jageocoder/exceptions.py
--rw-r--r--   0        0        0    19415 2024-01-04 06:10:34.702570 jageocoder-2.1.4/jageocoder/itaiji.py
--rw-r--r--   0        0        0    14220 2023-08-03 02:25:59.209435 jageocoder-2.1.4/jageocoder/itaiji_dic.json
--rw-r--r--   0        0        0    11718 2023-09-27 08:08:26.315234 jageocoder-2.1.4/jageocoder/module.py
--rw-r--r--   0        0        0    53416 2024-04-13 04:34:54.673227 jageocoder-2.1.4/jageocoder/node.py
--rw-r--r--   0        0        0     2631 2023-08-03 02:25:59.209435 jageocoder-2.1.4/jageocoder/result.py
--rw-r--r--   0        0        0    15475 2023-12-08 05:15:55.172087 jageocoder-2.1.4/jageocoder/rtree.py
--rw-r--r--   0        0        0     7795 2023-09-27 08:08:26.315234 jageocoder-2.1.4/jageocoder/strlib.py
--rw-r--r--   0        0        0    52841 2024-04-10 07:13:06.853053 jageocoder-2.1.4/jageocoder/tree.py
--rw-r--r--   0        0        0     4995 2023-08-03 02:25:59.213435 jageocoder-2.1.4/jageocoder/trie.py
--rw-r--r--   0        0        0     1287 2024-04-13 05:03:29.014148 jageocoder-2.1.4/pyproject.toml
--rw-r--r--   0        0        0     9773 1970-01-01 00:00:00.000000 jageocoder-2.1.4/PKG-INFO
+-rw-r--r--   0        0        0      113 2023-08-03 02:25:59.197434 jageocoder-2.1.5/LICENSE
+-rw-r--r--   0        0        0     8253 2024-04-15 00:39:42.101477 jageocoder-2.1.5/README.md
+-rw-r--r--   0        0        0     1364 2024-04-17 05:59:03.198988 jageocoder-2.1.5/jageocoder/__init__.py
+-rw-r--r--   0        0        0     5605 2024-04-16 08:30:01.122082 jageocoder-2.1.5/jageocoder/__main__.py
+-rw-r--r--   0        0        0     2574 2023-08-03 02:25:59.209435 jageocoder-2.1.5/jageocoder/address.py
+-rw-r--r--   0        0        0     1421 2023-08-03 02:25:59.209435 jageocoder-2.1.5/jageocoder/aliases.json
+-rw-r--r--   0        0        0     8320 2024-04-15 00:39:35.469528 jageocoder-2.1.5/jageocoder/aza_master.py
+-rw-r--r--   0        0        0     1171 2023-08-03 02:25:59.209435 jageocoder-2.1.5/jageocoder/dataset.py
+-rw-r--r--   0        0        0      691 2023-08-03 02:25:59.209435 jageocoder-2.1.5/jageocoder/exceptions.py
+-rw-r--r--   0        0        0    19415 2024-04-15 00:39:35.469528 jageocoder-2.1.5/jageocoder/itaiji.py
+-rw-r--r--   0        0        0    14220 2023-08-03 02:25:59.209435 jageocoder-2.1.5/jageocoder/itaiji_dic.json
+-rw-r--r--   0        0        0    12256 2024-04-16 08:41:18.843470 jageocoder-2.1.5/jageocoder/module.py
+-rw-r--r--   0        0        0    53418 2024-04-17 06:36:23.572171 jageocoder-2.1.5/jageocoder/node.py
+-rw-r--r--   0        0        0     3660 2024-04-17 06:27:31.657403 jageocoder-2.1.5/jageocoder/result.py
+-rw-r--r--   0        0        0    15687 2024-04-16 08:33:55.201079 jageocoder-2.1.5/jageocoder/rtree.py
+-rw-r--r--   0        0        0     7795 2023-09-27 08:08:26.315234 jageocoder-2.1.5/jageocoder/strlib.py
+-rw-r--r--   0        0        0    52841 2024-04-15 00:39:35.473528 jageocoder-2.1.5/jageocoder/tree.py
+-rw-r--r--   0        0        0     4995 2023-08-03 02:25:59.213435 jageocoder-2.1.5/jageocoder/trie.py
+-rw-r--r--   0        0        0     1287 2024-04-17 05:59:12.079264 jageocoder-2.1.5/pyproject.toml
+-rw-r--r--   0        0        0     9773 1970-01-01 00:00:00.000000 jageocoder-2.1.5/PKG-INFO
```

### Comparing `jageocoder-2.1.4/README.md` & `jageocoder-2.1.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 - Install the package with `pip install jageocoder`
 - Download an address database file compatible with that version from 
   [here](https://www.info-proto.com/static/jageocoder/latest/v2/)
 - Install the dictionary with `install-dictionary` command
 
 ```sh
 pip install jageocoder
-wget https://www.info-proto.com/static/jageocoder/latest/v2/jukyo_all_v20.zip
+wget https://www.info-proto.com/static/jageocoder/latest/v2/jukyo_all_v21.zip
 jageocoder install-dictionary jukyo_all_v20.zip
 ```
 
 The dictionary database will be installed under
 `{sys.prefix}/jageocoder/db2/` by default,
 however if the user doesn't have write permission there,
 `{site.USER_DATA}/jageocoder/db2/` instead.
```

### Comparing `jageocoder-2.1.4/jageocoder/__init__.py` & `jageocoder-2.1.5/jageocoder/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 running the following steps.
 
     >>> import jageocoder
     >>> jageocoder.init()
     >>> jageocoder.searchNode('<Japanese-address>')
 """
 
-__version__ = '2.1.4'  # The package version
+__version__ = '2.1.5'  # The package version
 __dictionary_version__ = '20230927'  # Compatible dictionary version
 __author__ = 'Takeshi Sagara <sagara@info-proto.com>'
 
 __all__ = [
     'init',
     'free',
     'is_initialized',
@@ -37,15 +37,15 @@
     'create_trie_index',
     'search',
     'searchNode',
     'reverse',
     'version',
     'dictionary_version',
     'installed_dictionary_version',
-    'instaleld_dictionary_readme',
+    'installed_dictionary_readme',
 ]
 
 from jageocoder.module import init, free, is_initialized, \
     get_db_dir, set_search_config, get_search_config, \
     get_module_tree, download_dictionary, install_dictionary, \
     uninstall_dictionary, create_trie_index, \
     search, searchNode, reverse, version, dictionary_version, \
```

### Comparing `jageocoder-2.1.4/jageocoder/__main__.py` & `jageocoder-2.1.5/jageocoder/__main__.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.4/jageocoder/address.py` & `jageocoder-2.1.5/jageocoder/address.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.4/jageocoder/aliases.json` & `jageocoder-2.1.5/jageocoder/aliases.json`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.4/jageocoder/aza_master.py` & `jageocoder-2.1.5/jageocoder/aza_master.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.4/jageocoder/dataset.py` & `jageocoder-2.1.5/jageocoder/dataset.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.4/jageocoder/exceptions.py` & `jageocoder-2.1.5/jageocoder/exceptions.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.4/jageocoder/itaiji.py` & `jageocoder-2.1.5/jageocoder/itaiji.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.4/jageocoder/itaiji_dic.json` & `jageocoder-2.1.5/jageocoder/itaiji_dic.json`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.4/jageocoder/module.py` & `jageocoder-2.1.5/jageocoder/module.py`

 * *Files 3% similar despite different names*

```diff
@@ -393,25 +393,51 @@
     if not is_initialized():
         raise JageocoderError("Not initialized. Call 'init()' first.")
 
     global _tree
     return _tree.searchNode(query)
 
 
-def reverse(x: float, y: float, level: Optional[int] = None) -> dict:
+def reverse(
+    x: float,
+    y: float,
+    level: Optional[int] = None,
+    as_dict: Optional[bool] = True
+) -> list:
     """
     Reverse geocoding.
+
+    Parameters
+    ----------
+    x: float
+        Longitude of the point.
+    y: float
+        Latitude of the point.
+    level: int, optional
+        Target node level.
+    as_dict: bool, default=True
+        If True, returns candidates as dict objects.
+
+    Returns
+    -------
+    list
+
+    Notes
+    -----
+    - The result list contains up to 3 nodes.
+    - Each element is a dict type with the following structure:
+        {"candidate":AddressNode, "dist":float} 
     """
     if not is_initialized():
         raise JageocoderError("Not initialized. Call 'init()' first.")
     from jageocoder.rtree import Index
 
     global _tree
     idx = Index(tree=_tree)
-    return idx.nearest(x=x, y=y, level=level)
+    return idx.nearest(x=x, y=y, level=level, as_dict=as_dict)
 
 
 def create_trie_index() -> None:
     """
     Create the TRIE index from the database file.
 
     This function is a shortcut for AddressTree.create_trie_index().
```

### Comparing `jageocoder-2.1.4/jageocoder/node.py` & `jageocoder-2.1.5/jageocoder/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,14 +197,15 @@
 
         return self.name
 
     @property
     def dataset(self):
         """
         Get dataset record.
+
         """
         return self.table.datasets.get(id=self.priority)
 
     @classmethod
     def from_record(cls, record) -> AddressNode:
         """
         Convert from a record of AddressNodeTable to an AddressNode object.
@@ -391,14 +392,15 @@
         """
         Get child nodes of the node.
 
         Returns
         -------
         List[AddressNode]
             The list of the child nodes.
+
         """
         return self.get_children()
 
     def get_children(self) -> List[AddressNode]:
         """
         Get child nodes of the node.
```

### Comparing `jageocoder-2.1.4/jageocoder/result.py` & `jageocoder-2.1.5/jageocoder/result.py`

 * *Files 26% similar despite different names*

```diff
@@ -20,24 +20,30 @@
     matched: str
         The matched substring of the query.
     nchars: int
         The number of matched characters.
         It is used only for recursive search.
     """
 
-    def __init__(self,
-                 node: Optional[AddressNode] = None,
-                 matched: str = '',
-                 nchars: int = 0):
+    def __init__(
+        self,
+        node: Optional[AddressNode] = None,
+        matched: str = '',
+        nchars: int = 0
+    ):
         self.node = node
         self.matched = matched
         self.nchars = nchars
 
-    def set(self, node: AddressNode,
-            matched: str, nchars: int = 0) -> 'Result':
+    def set(
+        self,
+        node: AddressNode,
+        matched: str,
+        nchars: int = 0
+    ) -> 'Result':
         """
         Set node and matched string.
         """
         self.node = node
         self.matched = matched
         self.matched = nchars or len(matched)
         return self
@@ -61,44 +67,87 @@
         ------
         str:
             The matched substring.
         """
         return self.matched
 
     def get_matched_nchars(self) -> int:
+        """
+        Get the the number of matched characters.
+
+        Return
+        ------
+        int
+            Number of characters in the matched substring.
+        """
         return self.nchars
 
-    def __getitem__(self, pos) -> Union[AddressNode, str]:
+    def __getitem__(
+        self,
+        pos
+    ) -> Union[AddressNode, str]:
         if pos == 0:
             return self.node
         elif pos == 1:
             return self.matched
         elif pos == 2:
             return self.nchars
 
         raise IndexError()
 
-    def __setitem__(self, pos, val: Union[AddressNode, str]) -> None:
+    def __setitem__(
+        self,
+        pos,
+        val: Union[AddressNode, str]
+    ) -> None:
         from jageocoder.node import AddressNode
         if pos == 0 and isinstance(val, AddressNode):
             self.node = val
         elif pos == 1 and isinstance(val, str):
             self.matched = val
         elif pos == 2 and isinstance(val, int):
             self.nchars = val
 
         raise RuntimeError()
 
     def as_dict(self) -> dict:
+        """
+        Convert Result object to dict type for display.
+
+        Return
+        ------
+        dict
+            A dict object containing the following elements;
+
+            "node"
+                AddressNode object converted to dict type.
+
+            "matched"
+                The substring matching the query.
+        """
         return {
             "node": self.node.as_dict(),
             "matched": self.matched,
-            # "nchars": self.nchars
         }
 
     def as_geojson(self) -> dict:
+        """
+        Convert Result to GeoJSON dict type for display.
+
+        Return
+        ------
+        dict
+            A GeoJSON dict object containing the following elements;
+
+            "type"
+                Always "Feature".
+            "geometry"
+                A point type geometry containing latitude and longitude.
+            "properties"
+                Include in "matched" the substring that matched the query, in addition to the attributes of the node.
+        """
         geojson = self.node.as_geojson()
         geojson['properties']['matched'] = self.matched
         return geojson
 
     def __repr__(self) -> str:
         return json.dumps(self.as_dict(), ensure_ascii=False)
```

### Comparing `jageocoder-2.1.4/jageocoder/rtree.py` & `jageocoder-2.1.5/jageocoder/rtree.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,32 +404,36 @@
         results.sort(key=lambda x: x[1])
         return [x[0] for x in results]
 
     def nearest(
         self,
         x: float,
         y: float,
-        level: Optional[int] = None
+        level: Optional[int] = None,
+        as_dict: Optional[bool] = True,
     ):
         """
         Search nearest nodes of the target point.
 
         Parameters
         ----------
         x: float
             The longitude of the target point.
         y: float
             The latitude of the target point.
         level: int, optional
             The level of the address ndoes to be retrieved as a result.
             If omitted, search down to the AZA level.
+        as_dict: bool, default=True
+            If False is specified, the addressNode object is stored
+            in the "candidate" field.
 
         Returns
         -------
-        [{"candidate":AddressNode, "dist":float}]
+        [{"candidate":AddressNode or dict, "dist":float}]
             Returns the results of retrieval up to 3 nodes.
         """
         level = level or AddressLevel.AZA
 
         # Search nodes by Rtree Index
         nodes = []
         ancestors = set()
@@ -493,15 +497,15 @@
             while node.level > level:
                 node = node.parent
 
             if node.id in registered:
                 continue
 
             results.append({
-                "candidate": node.as_dict(),
+                "candidate": node.as_dict() if as_dict else node,
                 "dist": self.distance(x, y, node.x, node.y)
             })
             registered.add(node.id)
 
         # Sort by distance
         results = sorted(results, key=lambda r: r['dist'])
```

### Comparing `jageocoder-2.1.4/jageocoder/strlib.py` & `jageocoder-2.1.5/jageocoder/strlib.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.4/jageocoder/tree.py` & `jageocoder-2.1.5/jageocoder/tree.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.4/jageocoder/trie.py` & `jageocoder-2.1.5/jageocoder/trie.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.4/pyproject.toml` & `jageocoder-2.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jageocoder"
-version = "2.1.4"
+version = "2.1.5"
 description = "A Japanese-address geocoder for Python."
 authors = ["Takeshi Sagara <sagara@info-proto.com>"]
 repository = "https://github.com/t-sagara/jageocoder/"
 license = "The MIT License"
 readme = "README.md"
 documentation = "https://jageocoder.readthedocs.io/"
 packages = [
```

### Comparing `jageocoder-2.1.4/PKG-INFO` & `jageocoder-2.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jageocoder
-Version: 2.1.4
+Version: 2.1.5
 Summary: A Japanese-address geocoder for Python.
 Home-page: https://github.com/t-sagara/jageocoder/
 License: The MIT License
 Author: Takeshi Sagara
 Author-email: sagara@info-proto.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -67,15 +67,15 @@
 - Install the package with `pip install jageocoder`
 - Download an address database file compatible with that version from 
   [here](https://www.info-proto.com/static/jageocoder/latest/v2/)
 - Install the dictionary with `install-dictionary` command
 
 ```sh
 pip install jageocoder
-wget https://www.info-proto.com/static/jageocoder/latest/v2/jukyo_all_v20.zip
+wget https://www.info-proto.com/static/jageocoder/latest/v2/jukyo_all_v21.zip
 jageocoder install-dictionary jukyo_all_v20.zip
 ```
 
 The dictionary database will be installed under
 `{sys.prefix}/jageocoder/db2/` by default,
 however if the user doesn't have write permission there,
 `{site.USER_DATA}/jageocoder/db2/` instead.
```

