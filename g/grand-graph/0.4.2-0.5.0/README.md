# Comparing `tmp/grand-graph-0.4.2.tar.gz` & `tmp/grand-graph-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grand-graph-0.4.2.tar", last modified: Sat May  7 21:02:32 2022, max compression
+gzip compressed data, was "grand-graph-0.5.0.tar", last modified: Wed Apr 17 13:57:38 2024, max compression
```

## Comparing `grand-graph-0.4.2.tar` & `grand-graph-0.5.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 mateljk1   (502) staff       (20)        0 2022-05-07 21:02:32.198057 grand-graph-0.4.2/
--rw-r--r--   0 mateljk1   (502) staff       (20)    10140 2022-02-04 17:02:41.000000 grand-graph-0.4.2/LICENSE
--rw-r--r--   0 mateljk1   (502) staff       (20)     5707 2022-05-07 21:02:32.197666 grand-graph-0.4.2/PKG-INFO
--rw-r--r--   0 mateljk1   (502) staff       (20)     5148 2022-05-07 21:01:23.000000 grand-graph-0.4.2/README.md
-drwxr-xr-x   0 mateljk1   (502) staff       (20)        0 2022-05-07 21:02:32.184641 grand-graph-0.4.2/grand/
--rw-r--r--   0 mateljk1   (502) staff       (20)     1108 2022-05-07 21:02:06.000000 grand-graph-0.4.2/grand/__init__.py
-drwxr-xr-x   0 mateljk1   (502) staff       (20)        0 2022-05-07 21:02:32.192599 grand-graph-0.4.2/grand/backends/
--rw-r--r--   0 mateljk1   (502) staff       (20)      572 2022-05-03 21:44:09.000000 grand-graph-0.4.2/grand/backends/__init__.py
--rw-r--r--   0 mateljk1   (502) staff       (20)    15497 2022-05-03 21:44:09.000000 grand-graph-0.4.2/grand/backends/_dataframe.py
--rw-r--r--   0 mateljk1   (502) staff       (20)    16291 2022-02-04 20:42:48.000000 grand-graph-0.4.2/grand/backends/_dynamodb.py
--rw-r--r--   0 mateljk1   (502) staff       (20)     8762 2022-02-04 20:42:48.000000 grand-graph-0.4.2/grand/backends/_gremlin.py
--rw-r--r--   0 mateljk1   (502) staff       (20)     7200 2022-05-07 20:59:17.000000 grand-graph-0.4.2/grand/backends/_igraph.py
--rw-r--r--   0 mateljk1   (502) staff       (20)     8963 2022-02-04 20:42:48.000000 grand-graph-0.4.2/grand/backends/_networkit.py
--rw-r--r--   0 mateljk1   (502) staff       (20)     5335 2022-02-04 20:42:48.000000 grand-graph-0.4.2/grand/backends/_networkx.py
--rw-r--r--   0 mateljk1   (502) staff       (20)    19406 2022-02-04 20:42:48.000000 grand-graph-0.4.2/grand/backends/_sqlbackend.py
--rw-r--r--   0 mateljk1   (502) staff       (20)     9881 2022-02-04 23:13:55.000000 grand-graph-0.4.2/grand/backends/backend.py
--rw-r--r--   0 mateljk1   (502) staff       (20)     1645 2022-02-04 17:02:41.000000 grand-graph-0.4.2/grand/backends/metadatastore.py
--rw-r--r--   0 mateljk1   (502) staff       (20)    11358 2022-05-07 20:59:17.000000 grand-graph-0.4.2/grand/backends/test_backends.py
--rw-r--r--   0 mateljk1   (502) staff       (20)     2467 2022-02-04 23:13:55.000000 grand-graph-0.4.2/grand/backends/test_cached_backend.py
--rw-r--r--   0 mateljk1   (502) staff       (20)     1086 2022-04-28 14:30:30.000000 grand-graph-0.4.2/grand/backends/test_metadatastore.py
-drwxr-xr-x   0 mateljk1   (502) staff       (20)        0 2022-05-07 21:02:32.193716 grand-graph-0.4.2/grand/dialects/
--rw-r--r--   0 mateljk1   (502) staff       (20)     8326 2022-02-18 00:30:00.000000 grand-graph-0.4.2/grand/dialects/__init__.py
--rw-r--r--   0 mateljk1   (502) staff       (20)     1540 2022-02-18 00:30:00.000000 grand-graph-0.4.2/grand/dialects/test_dialect.py
--rw-r--r--   0 mateljk1   (502) staff       (20)      199 2022-02-04 17:02:41.000000 grand-graph-0.4.2/grand/test_graph.py
-drwxr-xr-x   0 mateljk1   (502) staff       (20)        0 2022-05-07 21:02:32.196955 grand-graph-0.4.2/grand_graph.egg-info/
--rw-r--r--   0 mateljk1   (502) staff       (20)     5707 2022-05-07 21:02:32.000000 grand-graph-0.4.2/grand_graph.egg-info/PKG-INFO
--rw-r--r--   0 mateljk1   (502) staff       (20)      685 2022-05-07 21:02:32.000000 grand-graph-0.4.2/grand_graph.egg-info/SOURCES.txt
--rw-r--r--   0 mateljk1   (502) staff       (20)        1 2022-05-07 21:02:32.000000 grand-graph-0.4.2/grand_graph.egg-info/dependency_links.txt
--rw-r--r--   0 mateljk1   (502) staff       (20)      132 2022-05-07 21:02:32.000000 grand-graph-0.4.2/grand_graph.egg-info/requires.txt
--rw-r--r--   0 mateljk1   (502) staff       (20)        6 2022-05-07 21:02:32.000000 grand-graph-0.4.2/grand_graph.egg-info/top_level.txt
--rw-r--r--   0 mateljk1   (502) staff       (20)       38 2022-05-07 21:02:32.198233 grand-graph-0.4.2/setup.cfg
--rw-r--r--   0 mateljk1   (502) staff       (20)      892 2022-05-07 21:01:54.000000 grand-graph-0.4.2/setup.py
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2024-04-17 13:57:38.291848 grand-graph-0.5.0/
+-rw-r--r--   0 mateljk1   (501) staff       (20)    10140 2024-04-17 13:53:45.000000 grand-graph-0.5.0/LICENSE
+-rw-r--r--   0 mateljk1   (501) staff       (20)     5790 2024-04-17 13:57:38.291674 grand-graph-0.5.0/PKG-INFO
+-rw-r--r--   0 mateljk1   (501) staff       (20)     5268 2024-04-17 13:53:45.000000 grand-graph-0.5.0/README.md
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2024-04-17 13:57:38.225326 grand-graph-0.5.0/grand/
+-rw-r--r--   0 mateljk1   (501) staff       (20)     2378 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/__init__.py
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2024-04-17 13:57:38.227855 grand-graph-0.5.0/grand/backends/
+-rw-r--r--   0 mateljk1   (501) staff       (20)      572 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/backends/__init__.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)    15497 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/backends/_dataframe.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)    16291 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/backends/_dynamodb.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)     8762 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/backends/_gremlin.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)     7200 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/backends/_igraph.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)     8963 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/backends/_networkit.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)     5335 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/backends/_networkx.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)    20274 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/backends/_sqlbackend.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)    10763 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/backends/backend.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)     1915 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/backends/metadatastore.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)    12799 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/backends/test_backends.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)     2467 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/backends/test_cached_backend.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)     1411 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/backends/test_metadatastore.py
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2024-04-17 13:57:38.228231 grand-graph-0.5.0/grand/dialects/
+-rw-r--r--   0 mateljk1   (501) staff       (20)     8702 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/dialects/__init__.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)     5411 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/dialects/test_dialect.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)      405 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/test_graph.py
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2024-04-17 13:57:38.229103 grand-graph-0.5.0/grand_graph.egg-info/
+-rw-r--r--   0 mateljk1   (501) staff       (20)     5790 2024-04-17 13:57:38.000000 grand-graph-0.5.0/grand_graph.egg-info/PKG-INFO
+-rw-r--r--   0 mateljk1   (501) staff       (20)      685 2024-04-17 13:57:38.000000 grand-graph-0.5.0/grand_graph.egg-info/SOURCES.txt
+-rw-r--r--   0 mateljk1   (501) staff       (20)        1 2024-04-17 13:57:38.000000 grand-graph-0.5.0/grand_graph.egg-info/dependency_links.txt
+-rw-r--r--   0 mateljk1   (501) staff       (20)      132 2024-04-17 13:57:38.000000 grand-graph-0.5.0/grand_graph.egg-info/requires.txt
+-rw-r--r--   0 mateljk1   (501) staff       (20)        6 2024-04-17 13:57:38.000000 grand-graph-0.5.0/grand_graph.egg-info/top_level.txt
+-rw-r--r--   0 mateljk1   (501) staff       (20)       38 2024-04-17 13:57:38.291907 grand-graph-0.5.0/setup.cfg
+-rw-r--r--   0 mateljk1   (501) staff       (20)      892 2024-04-17 13:57:23.000000 grand-graph-0.5.0/setup.py
```

### Comparing `grand-graph-0.4.2/LICENSE` & `grand-graph-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grand-graph-0.4.2/PKG-INFO` & `grand-graph-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: grand-graph
-Version: 0.4.2
+Version: 0.5.0
 Summary: Graph database wrapper for non-graph datastores
 Home-page: https://github.com/aplbrain/grand
 Author: Jordan Matelsky
 Author-email: opensource@matelsky.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: sql
 Provides-Extra: dynamodb
 Provides-Extra: igraph
 Provides-Extra: networkit
 License-File: LICENSE
 
 <div align=center><img src="docs/grand.png" width=400 /></div>
 
-<div align=center><a href="https://pypi.org/project/grand-graph/"><img src="https://img.shields.io/pypi/v/grand-graph?style=for-the-badge" /></a> <a href="https://app.codecov.io/gh/aplbrain/grand"><img alt="Codecov" src="https://img.shields.io/codecov/c/github/aplbrain/grand?style=for-the-badge"></a> <img alt="GitHub Workflow Status" src="https://img.shields.io/github/workflow/status/aplbrain/grand/Python%20package?style=for-the-badge"></div>
+<div align=center><a href="https://pypi.org/project/grand-graph/"><img src="https://img.shields.io/pypi/v/grand-graph?style=for-the-badge" /></a> <a href="https://app.codecov.io/gh/aplbrain/grand"><img alt="Codecov" src="https://img.shields.io/codecov/c/github/aplbrain/grand?style=for-the-badge"></a></div>
+
+<!--  <a href="https://github.com/aplbrain/grand/actions/workflows/python-package.yml"><img alt="GitHub Workflow Status (with branch)" src="https://img.shields.io/github/actions/workflow/status/aplbrain/grand/python-package.yml?style=for-the-badge"></a> -->
 
 <br />
 
 <p align=center>Graph toolkit interoperability and scalability for Python</p>
 
 ## Installation
 
@@ -149,9 +149,7 @@
     month={Jun}
 }
 ```
 
 ---
 
 <p align=center><b>Made with 💙 at <a href="https://jhuapl.edu"><img alt="JHU APL" src="https://user-images.githubusercontent.com/693511/116814564-9b268800-ab27-11eb-98bb-dfddb2e405a1.png" height="23px" /></a></b></p>
-
-
```

#### html2text {}

```diff
@@ -1,18 +1,16 @@
-Metadata-Version: 2.1 Name: grand-graph Version: 0.4.2 Summary: Graph database
+Metadata-Version: 2.1 Name: grand-graph Version: 0.5.0 Summary: Graph database
 wrapper for non-graph datastores Home-page: https://github.com/aplbrain/grand
-Author: Jordan Matelsky Author-email: opensource@matelsky.com License: UNKNOWN
-Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Description-Content-Type: text/markdown Provides-Extra: sql
-Provides-Extra: dynamodb Provides-Extra: igraph Provides-Extra: networkit
-License-File: LICENSE
+Author: Jordan Matelsky Author-email: opensource@matelsky.com Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Description-Content-
+Type: text/markdown Provides-Extra: sql Provides-Extra: dynamodb Provides-
+Extra: igraph Provides-Extra: networkit License-File: LICENSE
                                [docs/grand.png]
-_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_g_r_a_n_d_-_g_r_a_p_h_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_C_o_d_e_c_o_v_][GitHub
-                               Workflow Status]
+   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_g_r_a_n_d_-_g_r_a_p_h_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_C_o_d_e_c_o_v_]
 
            Graph toolkit interoperability and scalability for Python
 ## Installation ```shell pip install grand-graph ``` ## Example use-cases -
 Write NetworkX commands to analyze true-serverless graph databases using
 DynamoDB\* - Query a host graph in SQL for subgraph isomorphisms with DotMotif
 - Write iGraph code to construct a graph, and then play with it in Networkit -
 Attach node and edge attributes to Networkit or IGraph graphs > \* [Neptune is
```

### Comparing `grand-graph-0.4.2/README.md` & `grand-graph-0.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 <div align=center><img src="docs/grand.png" width=400 /></div>
 
-<div align=center><a href="https://pypi.org/project/grand-graph/"><img src="https://img.shields.io/pypi/v/grand-graph?style=for-the-badge" /></a> <a href="https://app.codecov.io/gh/aplbrain/grand"><img alt="Codecov" src="https://img.shields.io/codecov/c/github/aplbrain/grand?style=for-the-badge"></a> <img alt="GitHub Workflow Status" src="https://img.shields.io/github/workflow/status/aplbrain/grand/Python%20package?style=for-the-badge"></div>
+<div align=center><a href="https://pypi.org/project/grand-graph/"><img src="https://img.shields.io/pypi/v/grand-graph?style=for-the-badge" /></a> <a href="https://app.codecov.io/gh/aplbrain/grand"><img alt="Codecov" src="https://img.shields.io/codecov/c/github/aplbrain/grand?style=for-the-badge"></a></div>
+
+<!--  <a href="https://github.com/aplbrain/grand/actions/workflows/python-package.yml"><img alt="GitHub Workflow Status (with branch)" src="https://img.shields.io/github/actions/workflow/status/aplbrain/grand/python-package.yml?style=for-the-badge"></a> -->
 
 <br />
 
 <p align=center>Graph toolkit interoperability and scalability for Python</p>
 
 ## Installation
```

#### html2text {}

```diff
@@ -1,10 +1,9 @@
                                [docs/grand.png]
-_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_g_r_a_n_d_-_g_r_a_p_h_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_C_o_d_e_c_o_v_][GitHub
-                               Workflow Status]
+   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_g_r_a_n_d_-_g_r_a_p_h_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_C_o_d_e_c_o_v_]
 
            Graph toolkit interoperability and scalability for Python
 ## Installation ```shell pip install grand-graph ``` ## Example use-cases -
 Write NetworkX commands to analyze true-serverless graph databases using
 DynamoDB\* - Query a host graph in SQL for subgraph isomorphisms with DotMotif
 - Write iGraph code to construct a graph, and then play with it in Networkit -
 Attach node and edge attributes to Networkit or IGraph graphs > \* [Neptune is
```

### Comparing `grand-graph-0.4.2/grand/__init__.py` & `grand-graph-0.5.0/grand/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,83 @@
 """
-Grand graph databasifier.
+Grand graphs package.
 
-Aug 2020
 """
 
+from typing import Optional
 from .backends import Backend, NetworkXBackend
-from .dialects import NetworkXDialect, IGraphDialect
+from .dialects import NetworkXDialect, IGraphDialect, NetworkitDialect
 
 
 _DEFAULT_BACKEND = NetworkXBackend
 
-__version__ = "0.4.2"
+__version__ = "0.5.0"
 
 
 class Graph:
     """
     A grand.Graph enables you to manipulate a graph using multiple dialects.
 
     """
 
-    def __init__(
-        self, backend: Backend = None, directed: bool = True, dialects: dict = None
-    ):
+    nx: NetworkXDialect
+    networkit: NetworkitDialect
+    igraph: IGraphDialect
+
+    def __init__(self, backend: Optional[Backend] = None, **backend_kwargs: dict):
         """
         Create a new grand.Graph.
 
+        The only positional argument is the backend to use. All other arguments
+        are passed to the backend's constructor, if a type is provided.
+        Otherwise, kwargs are ignored.
+
         Arguments:
             backend (Backend): The backend to use. If none is provided, will
                 default to _DEFAULT_BACKEND.
 
-        Returns:
-            None
-
         """
-        self.backend = backend or _DEFAULT_BACKEND(directed=directed)
+        self.backend = backend or _DEFAULT_BACKEND
+
+        # If you passed a class instead of an instance, instantiate it with
+        # kwargs from the constructor:
+        if isinstance(self.backend, type):
+            self.backend = self.backend(**backend_kwargs)
 
         # Attach dialects:
-        self.nx = NetworkXDialect(self)
-        self.igraph = IGraphDialect(self)
+        self.attach_dialect("nx", NetworkXDialect)
+        self.attach_dialect("igraph", IGraphDialect)
+        self.attach_dialect("networkit", NetworkitDialect)
 
-        if dialects:
-            self.dialects = {k: v(self) for k, v in dialects.items()}
+    def attach_dialect(self, name: str, dialect: type):
+        """
+        Attach a dialect to the graph.
 
-    def save(self, filename: str) -> str:
-        raise NotImplementedError()
+        Arguments:
+            name (str): The name of the dialect.
+            dialect (type): The dialect class to attach.
+
+        """
+        setattr(self, name, dialect(self))
+
+
+class DiGraph(Graph):
+    """
+    A grand.DiGraph enables you to manipulate a directed graph. This is a
+    convenience class that inherits from grand.Graph.
 
-    @staticmethod
-    def load(self, filename: str) -> str:
-        raise NotImplementedError()
+    """
+
+    def __init__(self, backend: Optional[Backend] = None, **backend_kwargs: dict):
+        """
+        Create a new grand.DiGraph.
+
+        The only positional argument is the backend to use. All other arguments
+        are passed to the backend's constructor, if a type is provided.
+        Otherwise, kwargs are ignored.
+
+        Arguments:
+            backend (Backend): The backend to use. If none is provided, will
+                default to _DEFAULT_BACKEND.
+
+        """
+        super().__init__(backend, **{**backend_kwargs, "directed": True})
```

### Comparing `grand-graph-0.4.2/grand/backends/__init__.py` & `grand-graph-0.5.0/grand/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `grand-graph-0.4.2/grand/backends/_dataframe.py` & `grand-graph-0.5.0/grand/backends/_dataframe.py`

 * *Files identical despite different names*

### Comparing `grand-graph-0.4.2/grand/backends/_dynamodb.py` & `grand-graph-0.5.0/grand/backends/_dynamodb.py`

 * *Files identical despite different names*

### Comparing `grand-graph-0.4.2/grand/backends/_gremlin.py` & `grand-graph-0.5.0/grand/backends/_gremlin.py`

 * *Files identical despite different names*

### Comparing `grand-graph-0.4.2/grand/backends/_igraph.py` & `grand-graph-0.5.0/grand/backends/_igraph.py`

 * *Files identical despite different names*

### Comparing `grand-graph-0.4.2/grand/backends/_networkit.py` & `grand-graph-0.5.0/grand/backends/_networkit.py`

 * *Files identical despite different names*

### Comparing `grand-graph-0.4.2/grand/backends/_networkx.py` & `grand-graph-0.5.0/grand/backends/_networkx.py`

 * *Files identical despite different names*

### Comparing `grand-graph-0.4.2/grand/backends/_sqlbackend.py` & `grand-graph-0.5.0/grand/backends/_sqlbackend.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Hashable, Generator, Optional, Iterable
 import time
 
 import pandas as pd
 import sqlalchemy
 from sqlalchemy.pool import NullPool
 from sqlalchemy.sql import select
-from sqlalchemy import and_, or_, func
+from sqlalchemy import and_, or_, func, Index
 
 from .backend import Backend
 
 _DEFAULT_SQL_URL = "sqlite:///"
 _DEFAULT_SQL_STR_LEN = 64
 
 
@@ -56,59 +56,56 @@
         self._edge_target_key = edge_table_target_column or "Target"
 
         sqlalchemy_kwargs = sqlalchemy_kwargs or {}
         self._engine = sqlalchemy.create_engine(db_url, **sqlalchemy_kwargs)
         self._connection = self._engine.connect()
         self._metadata = sqlalchemy.MetaData()
 
-        if not self._engine.dialect.has_table(self._connection, self._node_table_name):
-            self._node_table = sqlalchemy.Table(
-                self._node_table_name,
-                self._metadata,
-                sqlalchemy.Column(
-                    self._primary_key,
-                    sqlalchemy.String(_DEFAULT_SQL_STR_LEN),
-                    primary_key=True,
-                ),
-                sqlalchemy.Column("_metadata", sqlalchemy.JSON),
-            )
-            self._node_table.create(self._engine)
-        else:
-            self._node_table = sqlalchemy.Table(
-                self._node_table_name,
-                self._metadata,
-                autoload=True,
-                autoload_with=self._engine,
-            )
+        # Create nodes table
+        self._node_table = sqlalchemy.Table(
+            self._node_table_name,
+            self._metadata,
+            sqlalchemy.Column(
+                self._primary_key,
+                sqlalchemy.String(_DEFAULT_SQL_STR_LEN),
+                primary_key=True,
+            ),
+            sqlalchemy.Column("_metadata", sqlalchemy.JSON),
+        )
+        self._node_table.create(self._engine, checkfirst=True)
 
-        if not self._engine.dialect.has_table(self._connection, self._edge_table_name):
-            self._edge_table = sqlalchemy.Table(
-                self._edge_table_name,
-                self._metadata,
-                sqlalchemy.Column(
-                    self._primary_key,
-                    sqlalchemy.String(_DEFAULT_SQL_STR_LEN),
-                    primary_key=True,
-                ),
-                sqlalchemy.Column("_metadata", sqlalchemy.JSON),
-                sqlalchemy.Column(
-                    self._edge_source_key, sqlalchemy.String(_DEFAULT_SQL_STR_LEN)
-                ),
-                sqlalchemy.Column(
-                    self._edge_target_key, sqlalchemy.String(_DEFAULT_SQL_STR_LEN)
-                ),
-            )
-            self._edge_table.create(self._engine)
-        else:
-            self._edge_table = sqlalchemy.Table(
-                self._edge_table_name,
-                self._metadata,
-                autoload=True,
-                autoload_with=self._engine,
-            )
+        source_column = sqlalchemy.Column(
+                self._edge_source_key, sqlalchemy.String(_DEFAULT_SQL_STR_LEN)
+        )
+
+        target_column = sqlalchemy.Column(
+                self._edge_target_key, sqlalchemy.String(_DEFAULT_SQL_STR_LEN)
+        )
+
+        # Create edges table
+        self._edge_table = sqlalchemy.Table(
+            self._edge_table_name,
+            self._metadata,
+            sqlalchemy.Column(
+                self._primary_key,
+                sqlalchemy.String(_DEFAULT_SQL_STR_LEN),
+                primary_key=True,
+            ),
+            sqlalchemy.Column("_metadata", sqlalchemy.JSON),
+            source_column,
+            target_column
+        )
+        self._edge_table.create(self._engine, checkfirst=True)
+
+        # Create source and target index
+        sindex = Index("edge_source", source_column)
+        sindex.create(self._engine, checkfirst=True)
+
+        tindex = Index("edge_target", target_column)
+        tindex.create(self._engine, checkfirst=True)
 
     def is_directed(self) -> bool:
         """
         Return True if the backend graph is directed.
 
         Arguments:
             None
@@ -143,25 +140,33 @@
 
         """
         if self.has_node(node_name):
             existing_metadata = self.get_node_by_id(node_name)
             existing_metadata.update(metadata)
             self._connection.execute(
                 self._node_table.update().where(
-                    self._node_table.c[self._primary_key] == node_name
+                    self._node_table.c[self._primary_key] == str(node_name)
                 ),
-                **{"_metadata": existing_metadata},
+                parameters={"_metadata": existing_metadata},
             )
         else:
             self._connection.execute(
                 self._node_table.insert(),
-                **{self._primary_key: node_name, "_metadata": metadata},
+                parameters={self._primary_key: node_name, "_metadata": metadata},
             )
         return node_name
 
+    def add_nodes_from(self, nodes_for_adding, **attr):
+        nodes = [{
+            self._primary_key: node,
+            "_metadata": {**attr, **metadata},
+        } for node, metadata in nodes_for_adding]
+
+        self._connection.execute(self._node_table.insert(), nodes)
+
     def _upsert_node(self, node_name: Hashable, metadata: dict) -> Hashable:
         """
         Add a new node to the graph, or update an existing one.
 
         Arguments:
             node_name (Hashable): The ID of the node
             metadata (dict: None): An optional dictionary of metadata
@@ -170,55 +175,61 @@
             Hashable: The ID of this node, as inserted
 
         """
         node_exists = self.has_node(node_name)
         if node_exists:
             self._connection.execute(
                 self._node_table.update().where(
-                    self._node_table.c[self._primary_key] == node_name
+                    self._node_table.c[self._primary_key] == str(node_name)
                 ),
-                **{"_metadata": metadata},
+                parameters={"_metadata": metadata},
             )
         else:
             self._connection.execute(
                 self._node_table.insert(),
-                **{self._primary_key: node_name, "_metadata": metadata},
+                parameters={self._primary_key: node_name, "_metadata": metadata},
             )
 
     def all_nodes_as_iterable(self, include_metadata: bool = False) -> Generator:
         """
         Get a generator of all of the nodes in this graph.
 
         Arguments:
             include_metadata (bool: False): Whether to include node metadata in
                 the response
 
         Returns:
             Generator: A generator of all nodes (arbitrary sort)
 
         """
-        results = self._connection.execute(self._node_table.select()).fetchall()
         if include_metadata:
-            return [(row[self._primary_key], row["_metadata"]) for row in results]
-        return [row[self._primary_key] for row in results]
+            sql = self._node_table.select()
+        else:
+            sql = self._node_table.select().with_only_columns(self._node_table.c[self._primary_key])
+
+        results = []
+        for x in self._connection.execute(sql):
+            results.append(x if include_metadata else x[0])
+
+        return results
 
     def has_node(self, u: Hashable) -> bool:
         """
         Return true if the node exists in the graph.
 
         Arguments:
             u (Hashable): The ID of the node to check
 
         Returns:
             bool: True if the node exists
         """
         return len(
             self._connection.execute(
                 self._node_table.select().where(
-                    self._node_table.c[self._primary_key] == u
+                    self._node_table.c[self._primary_key] == str(u)
                 )
             ).fetchall()
         )
 
     def add_edge(self, u: Hashable, v: Hashable, metadata: dict):
         """
         Add a new edge to the graph between two nodes.
@@ -241,69 +252,82 @@
             self.add_node(u, {})
         if not self.has_node(v):
             self.add_node(v, {})
 
         try:
             self._connection.execute(
                 self._edge_table.insert(),
-                **{
+                parameters={
                     self._primary_key: pk,
                     self._edge_source_key: u,
                     self._edge_target_key: v,
                     "_metadata": metadata,
                 },
             )
         except sqlalchemy.exc.IntegrityError:
             # Edge already exists, perform the update:
             existing_metadata = self.get_edge_by_id(u, v)
             existing_metadata.update(metadata)
             self._connection.execute(
                 self._edge_table.update().where(
                     self._edge_table.c[self._primary_key] == pk
                 ),
-                **{"_metadata": existing_metadata},
+                parameters={"_metadata": existing_metadata},
             )
 
         return pk
 
+    def add_edges_from(self, ebunch_to_add, **attr):
+        edges = [{
+            self._primary_key: f"__{u}__{v}",
+            self._edge_source_key: u,
+            self._edge_target_key: v,
+            "_metadata": {**attr, **metadata},
+        } for u, v, metadata in ebunch_to_add]
+
+        self._connection.execute(self._edge_table.insert(), edges)
+
     def all_edges_as_iterable(self, include_metadata: bool = False) -> Generator:
         """
         Get a list of all edges in this graph, arbitrary sort.
 
         Arguments:
             include_metadata (bool: False): Whether to include edge metadata
 
         Returns:
             Generator: A generator of all edges (arbitrary sort)
-
         """
-        return iter(
-            [
-                (e.Source, e.Target, e._metadata)
-                if include_metadata
-                else (e.Source, e.Target)
-                for e in self._connection.execute(self._edge_table.select()).fetchall()
-            ]
-        )
+
+        columns = [
+            self._node_table.c[self._edge_source_key],
+            self._node_table.c[self._edge_target_key]
+        ]
+
+        if include_metadata:
+            columns.append(self._node_table.c["_metadata"])
+
+        sql = self._node_table.select().with_only_columns(columns)
+        return self._connection.execute(sql).fetchall()
 
     def get_node_by_id(self, node_name: Hashable):
         """
         Return the data associated with a node.
 
         Arguments:
             node_name (Hashable): The node ID to look up
 
         Returns:
             dict: The metadata associated with this node
 
         """
+
         res = (
             self._connection.execute(
                 self._node_table.select().where(
-                    self._node_table.c[self._primary_key] == node_name
+                    self._node_table.c[self._primary_key] == str(node_name)
                 )
             )
             .fetchone()
             ._metadata
         )
         return res
 
@@ -353,45 +377,48 @@
         Arguments:
             u (Hashable): The source node ID
 
         Returns:
             Generator
 
         """
+
         if self._directed:
             res = self._connection.execute(
                 self._edge_table.select().where(
-                    self._edge_table.c[self._edge_source_key] == u
-                )
+                    self._edge_table.c[self._edge_source_key] == str(u)
+                ).order_by(self._edge_table.c[self._primary_key])
             ).fetchall()
         else:
             res = self._connection.execute(
                 self._edge_table.select().where(
                     or_(
-                        (self._edge_table.c[self._edge_source_key] == u),
-                        (self._edge_table.c[self._edge_target_key] == u),
+                        (self._edge_table.c[self._edge_source_key] == str(u)),
+                        (self._edge_table.c[self._edge_target_key] == str(u)),
                     )
-                )
+                ).order_by(self._edge_table.c[self._primary_key])
             ).fetchall()
 
+        res = [x._asdict() for x in res]
+
         if include_metadata:
             return {
                 (
                     r[self._edge_source_key]
-                    if r[self._edge_source_key] != u
+                    if r[self._edge_source_key] != str(u)
                     else r[self._edge_target_key]
                 ): r["_metadata"]
                 for r in res
             }
 
         return iter(
             [
                 (
                     r[self._edge_source_key]
-                    if r[self._edge_source_key] != u
+                    if r[self._edge_source_key] != str(u)
                     else r[self._edge_target_key]
                 )
                 for r in res
             ]
         )
 
     def get_node_predecessors(
@@ -406,42 +433,44 @@
         Returns:
             Generator
 
         """
         if self._directed:
             res = self._connection.execute(
                 self._edge_table.select().where(
-                    self._edge_table.c[self._edge_target_key] == u
-                )
+                    self._edge_table.c[self._edge_target_key] == str(u)
+                ).order_by(self._edge_table.c[self._primary_key])
             ).fetchall()
         else:
             res = self._connection.execute(
                 self._edge_table.select().where(
                     or_(
-                        (self._edge_table.c[self._edge_target_key] == u),
-                        (self._edge_table.c[self._edge_source_key] == u),
+                        (self._edge_table.c[self._edge_target_key] == str(u)),
+                        (self._edge_table.c[self._edge_source_key] == str(u)),
                     )
-                )
+                ).order_by(self._edge_table.c[self._primary_key])
             ).fetchall()
 
+        res = [x._asdict() for x in res]
+
         if include_metadata:
             return {
                 (
                     r[self._edge_source_key]
-                    if r[self._edge_source_key] != u
+                    if r[self._edge_source_key] != str(u)
                     else r[self._edge_target_key]
                 ): r["_metadata"]
                 for r in res
             }
 
         return iter(
             [
                 (
                     r[self._edge_source_key]
-                    if r[self._edge_source_key] != u
+                    if r[self._edge_source_key] != str(u)
                     else r[self._edge_target_key]
                 )
                 for r in res
             ]
         )
 
     def get_node_count(self) -> Iterable:
@@ -452,15 +481,15 @@
             None
 
         Returns:
             int: The count of nodes
 
         """
         return self._connection.execute(
-            select([func.count()]).select_from(self._node_table)
+            select(func.count()).select_from(self._node_table)
         ).scalar()
 
     def out_degrees(self, nbunch=None):
         """
         Return the in-degree of each node in the graph.
 
         Arguments:
@@ -470,38 +499,38 @@
             dict: A dictionary of node: in-degree pairs
 
         """
 
         if nbunch is None:
             where_clause = None
         elif isinstance(nbunch, (list, tuple)):
-            where_clause = self._edge_table.c[self._edge_source_key].in_(nbunch)
+            where_clause = self._edge_table.c[self._edge_source_key].in_([str(x) for x in nbunch])
         else:
             # single node:
-            where_clause = self._edge_table.c[self._edge_source_key] == nbunch
+            where_clause = self._edge_table.c[self._edge_source_key] == str(nbunch)
 
         if self._directed:
             query = (
-                select([self._edge_table.c[self._edge_source_key], func.count()])
+                select(self._edge_table.c[self._edge_source_key], func.count())
                 .select_from(self._edge_table)
                 .group_by(self._edge_table.c[self._edge_source_key])
             )
         else:
             query = (
-                select([self._edge_table.c[self._edge_source_key], func.count()])
+                select(self._edge_table.c[self._edge_source_key], func.count())
                 .select_from(self._edge_table)
                 .group_by(self._edge_table.c[self._edge_source_key])
             )
 
         if where_clause is not None:
             query = query.where(where_clause)
 
         results = {
-            r[self._edge_source_key]: r[1]
-            for r in self._connection.execute(query).fetchall()
+            r[0]: r[1]
+            for r in self._connection.execute(query)
         }
 
         if nbunch and not isinstance(nbunch, (list, tuple)):
             return results.get(nbunch, 0)
         return results
 
     def in_degrees(self, nbunch=None):
@@ -515,38 +544,38 @@
             dict: A dictionary of node: in-degree pairs
 
         """
 
         if nbunch is None:
             where_clause = None
         elif isinstance(nbunch, (list, tuple)):
-            where_clause = self._edge_table.c[self._edge_target_key].in_(nbunch)
+            where_clause = self._edge_table.c[self._edge_target_key].in_([str(x) for x in nbunch])
         else:
             # single node:
-            where_clause = self._edge_table.c[self._edge_target_key] == nbunch
+            where_clause = self._edge_table.c[self._edge_target_key] == str(nbunch)
 
         if self._directed:
             query = (
-                select([self._edge_table.c[self._edge_target_key], func.count()])
+                select(self._edge_table.c[self._edge_target_key], func.count())
                 .select_from(self._edge_table)
                 .group_by(self._edge_table.c[self._edge_target_key])
             )
         else:
             query = (
-                select([self._edge_table.c[self._edge_target_key], func.count()])
+                select(self._edge_table.c[self._edge_target_key], func.count())
                 .select_from(self._edge_table)
                 .group_by(self._edge_table.c[self._edge_target_key])
             )
 
         if where_clause is not None:
             query = query.where(where_clause)
 
         results = {
-            r[self._edge_target_key]: r[1]
-            for r in self._connection.execute(query).fetchall()
+            r[0]: r[1]
+            for r in self._connection.execute(query)
         }
 
         if nbunch and not isinstance(nbunch, (list, tuple)):
             return results.get(nbunch, 0)
         return results
 
     def ingest_from_edgelist_dataframe(
```

### Comparing `grand-graph-0.4.2/grand/backends/backend.py` & `grand-graph-0.5.0/grand/backends/backend.py`

 * *Files 10% similar despite different names*

```diff
@@ -61,14 +61,25 @@
 
         Returns:
             Hashable: The ID of this node, as inserted
 
         """
         ...
 
+    def add_nodes_from(self, nodes_for_adding, **attr):
+        """
+        Add nodes to the graph.
+
+        Arguments:
+            nodes_for_adding: nodes to add
+            attr: additional attributes
+        """
+        for node, metadata in nodes_for_adding:
+            self.add_node(node, {**attr, **metadata})
+
     def get_node_by_id(self, node_name: Hashable):
         """
         Return the data associated with a node.
 
         Arguments:
             node_name (Hashable): The node ID to look up
 
@@ -98,15 +109,18 @@
 
         Arguments:
             u (Hashable): The ID of the node to check
 
         Returns:
             bool: True if the node exists
         """
-        ...
+        try:
+            return self.get_node_by_id(u) is not None
+        except KeyError:
+            return False
 
     def add_edge(self, u: Hashable, v: Hashable, metadata: dict):
         """
         Add a new edge to the graph between two nodes.
 
         If the graph is directed, this edge will start (source) at the `u` node
         and end (target) at the `v` node.
@@ -118,14 +132,25 @@
 
         Returns:
             Hashable: The edge ID, as inserted.
 
         """
         ...
 
+    def add_edges_from(self, ebunch_to_add, **attr):
+        """
+        Add new edges to the graph.
+
+        Arguments:
+            ebunch_to_add: list of (source, target, metadata)
+            attr: additional common attributes
+        """
+        for u, v, metadata in ebunch_to_add:
+            self.add_edge(u, v, {**attr, **metadata})
+
     def all_edges_as_iterable(self, include_metadata: bool = False) -> Collection:
         """
         Get a list of all edges in this graph, arbitrary sort.
 
         Arguments:
             include_metadata (bool: False): Whether to include edge metadata
 
@@ -204,15 +229,15 @@
         Arguments:
             u (Hashable): The node ID
 
         Returns:
             int: The degree of the node
 
         """
-        return len(self.get_node_neighbors(u))
+        return len([i for i in self.get_node_neighbors(u)])
 
     def degrees(self, nbunch=None) -> Collection:
         return {
             node: self.degree(node) for node in (nbunch or self.all_nodes_as_iterable())
         }
 
     def in_degree(self, u: Hashable) -> int:
@@ -280,21 +305,25 @@
         "LRUCache": cachetools.func.lru_cache,
         "TTLCache": cachetools.func.ttl_cache,
         "LFUCache": cachetools.func.lfu_cache,
     }
 
     _default_uncacheable_methods = [
         "add_node",
+        "add_nodes_from",
         "add_edge",
+        "add_edges_from",
         "ingest_from_edgelist_dataframe",
     ]
 
     _default_write_methods = [
         "add_node",
+        "add_nodes_from",
         "add_edge",
+        "add_edges_from",
         "ingest_from_edgelist_dataframe",
     ]
 
     def __init__(
         self,
         backend: Backend,
         dirty_cache_on_write: bool = True,
```

### Comparing `grand-graph-0.4.2/grand/backends/metadatastore.py` & `grand-graph-0.5.0/grand/backends/metadatastore.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,20 +19,28 @@
     def __init__(self):
         self.ndata = {}
         self.edata = {}
 
     def add_node(self, node_name: Hashable, metadata: dict) -> Hashable:
         if metadata is None:
             metadata = {}
-        self.ndata[node_name] = metadata
+        # Add or update metadata
+        if node_name in self.ndata:
+            self.ndata[node_name].update(metadata)
+        else:
+            self.ndata[node_name] = metadata
 
     def add_edge(self, u: Hashable, v: Hashable, metadata: dict) -> Hashable:
         if metadata is None:
             metadata = {}
-        self.edata[(u, v)] = metadata
+        # Add or update metadata
+        if (u, v) in self.edata:
+            self.edata[(u, v)].update(metadata)
+        else:
+            self.edata[(u, v)] = metadata
 
     def get_node(self, node_name: Hashable) -> dict:
         return self.ndata[node_name]
 
     def get_edge(self, u: Hashable, v: Hashable) -> dict:
         return self.edata[(u, v)]
```

### Comparing `grand-graph-0.4.2/grand/backends/test_backends.py` & `grand-graph-0.5.0/grand/backends/test_backends.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,170 +16,194 @@
     from ._igraph import IGraphBackend
 
     _CAN_IMPORT_IGRAPH = True
 except ImportError:
     _CAN_IMPORT_IGRAPH = False
 
 try:
+    from ._networkit import NetworkitBackend
+
+    _CAN_IMPORT_NETWORKIT = True
+except ImportError:
+    _CAN_IMPORT_NETWORKIT = False
+
+try:
     from ._sqlbackend import SQLBackend
 
     _CAN_IMPORT_SQL = True
 except ImportError:
     _CAN_IMPORT_SQL = False
 
 from .. import Graph
 
 
 backend_test_params = [
     pytest.param(
-        NetworkXBackend,
+        (NetworkXBackend, {}),
         marks=pytest.mark.skipif(
             os.environ.get("TEST_NETWORKXBACKEND", default="1") != "1",
             reason="NetworkX Backend skipped because $TEST_NETWORKXBACKEND != 1.",
         ),
     ),
 ]
 backend_test_params = [
     pytest.param(
-        DataFrameBackend,
+        (DataFrameBackend, {}),
         marks=pytest.mark.skipif(
             os.environ.get("TEST_DATAFRAMEBACKEND", default="1") != "1",
             reason="DataFrameBackend skipped because $TEST_DATAFRAMEBACKEND != 1.",
         ),
     ),
 ]
 
 if _CAN_IMPORT_DYNAMODB:
     backend_test_params.append(
         pytest.param(
-            DynamoDBBackend,
+            (DynamoDBBackend, {}),
             marks=pytest.mark.skipif(
                 os.environ.get("TEST_DYNAMODB", default="1") != "1",
                 reason="DynamoDB Backend skipped because $TEST_DYNAMODB != 0 or boto3 is not installed",
             ),
         ),
     )
 
 if _CAN_IMPORT_SQL:
     backend_test_params.append(
         pytest.param(
-            SQLBackend,
+            (SQLBackend, {"db_url": "sqlite:///:memory:"}),
             marks=pytest.mark.skipif(
-                os.environ.get("TEST_SQLBACKEND", default="1") != "1"
-                or not _CAN_IMPORT_SQL,
+                os.environ.get("TEST_SQLBACKEND", default="1") != "1",
                 reason="SQL Backend skipped because $TEST_SQLBACKEND != 1 or sqlalchemy is not installed.",
             ),
         ),
     )
 if _CAN_IMPORT_IGRAPH:
     backend_test_params.append(
         pytest.param(
-            IGraphBackend,
+            (IGraphBackend, {}),
+            marks=pytest.mark.skipif(
+                os.environ.get("TEST_IGRAPHBACKEND", default="1") != "1",
+                reason="IGraph Backend skipped because $TEST_IGRAPHBACKEND != 1 or igraph is not installed.",
+            ),
+        ),
+    )
+if _CAN_IMPORT_NETWORKIT:
+    backend_test_params.append(
+        pytest.param(
+            (NetworkitBackend, {}),
             marks=pytest.mark.skipif(
-                os.environ.get("TEST_IGRAPBACKEND", default="1") != "1"
-                or not _CAN_IMPORT_SQL,
-                reason="IGraph Backend skipped because $TEST_IGRAPBACKEND != 1 or igraph is not installed.",
+                os.environ.get("TEST_NETWORKIT", default="1") != "1",
+                reason="Networkit Backend skipped because $TEST_NETWORKIT != 1 or networkit is not installed.",
             ),
         ),
     )
 
 if os.environ.get("TEST_NETWORKITBACKEND") == "1":
     from ._networkit import NetworkitBackend
 
     backend_test_params.append(
         pytest.param(
-            NetworkitBackend,
+            (NetworkitBackend, {}),
             marks=pytest.mark.skipif(
                 os.environ.get("TEST_NETWORKITBACKEND") != "1",
                 reason="Networkit Backend skipped because $TEST_NETWORKITBACKEND != 1.",
             ),
         ),
     )
 
 if os.environ.get("TEST_IGRAPHBACKEND") == "1":
     from ._igraph import IGraphBackend
 
     backend_test_params.append(
         pytest.param(
-            IGraphBackend,
+            (IGraphBackend, {}),
             marks=pytest.mark.skipif(
                 os.environ.get("TEST_IGRAPHBACKEND") != "1",
                 reason="Networkit Backend skipped because $TEST_IGRAPHBACKEND != 1.",
             ),
         ),
     )
 
 
 @pytest.mark.parametrize("backend", backend_test_params)
 class TestBackend:
     def test_can_create(self, backend):
-        backend()
+        backend, kwargs = backend
+        backend(**kwargs)
 
     def test_can_create_directed_and_undirected_backends(self, backend):
-        b = backend(directed=True)
+        backend, kwargs = backend
+        b = backend(directed=True, **kwargs)
         assert b.is_directed() == True
 
-        b = backend(directed=False)
+        b = backend(directed=False, **kwargs)
         assert b.is_directed() == False
 
     def test_can_add_node(self, backend):
-        G = Graph(backend=backend())
+        backend, kwargs = backend
+        G = Graph(backend=backend(**kwargs))
         nxG = nx.Graph()
         G.nx.add_node("A", k="v")
         nxG.add_node("A", k="v")
         assert len(G.nx.nodes()) == len(nxG.nodes())
         G.nx.add_node("B", k="v")
         nxG.add_node("B", k="v")
         assert len(G.nx.nodes()) == len(nxG.nodes())
 
     def test_can_update_node(self, backend):
-        G = Graph(backend=backend())
+        backend, kwargs = backend
+        G = Graph(backend=backend(**kwargs))
         G.nx.add_node("A", k="v", z=3)
         G.nx.add_node("A", k="v2", x=4)
         assert G.nx.nodes["A"]["k"] == "v2"
         assert G.nx.nodes["A"]["x"] == 4
         assert G.nx.nodes["A"]["z"] == 3
 
     def test_can_add_edge(self, backend):
-        G = Graph(backend=backend())
+        backend, kwargs = backend
+        G = Graph(backend=backend(**kwargs))
         nxG = nx.Graph()
         G.nx.add_edge("A", "B")
         nxG.add_edge("A", "B")
         assert len(G.nx.edges()) == len(nxG.edges())
         G.nx.add_edge("A", "B")
         nxG.add_edge("A", "B")
         assert len(G.nx.edges()) == len(nxG.edges())
 
     def test_can_update_edge(self, backend):
-        G = Graph(backend=backend())
+        backend, kwargs = backend
+        G = Graph(backend=backend(**kwargs))
         G.nx.add_edge("A", "B", k="v", z=3)
         G.nx.add_edge("A", "B", k="v2", x=4)
         assert G.nx.get_edge_data("A", "B")["k"] == "v2"
         assert G.nx.get_edge_data("A", "B")["x"] == 4
         assert G.nx.get_edge_data("A", "B")["z"] == 3
         assert len(G.nx.nodes()) == 2
 
     def test_can_get_node(self, backend):
-        G = Graph(backend=backend())
+        backend, kwargs = backend
+        G = Graph(backend=backend(**kwargs))
         nxG = nx.Graph()
         md = dict(k="B")
         G.nx.add_node("A", **md)
         nxG.add_node("A", **md)
         assert G.nx.nodes["A"] == nxG.nodes["A"]
 
     def test_can_get_edge(self, backend):
-        G = Graph(backend=backend())
+        backend, kwargs = backend
+        G = Graph(backend=backend(**kwargs))
         nxG = nx.Graph()
         md = {"k": "B"}
         G.nx.add_edge("A", "B", **md)
         nxG.add_edge("A", "B", **md)
         assert G.nx.get_edge_data("A", "B") == nxG.get_edge_data("A", "B")
 
     def test_can_get_neighbors(self, backend):
-        G = Graph(backend=backend())
+        backend, kwargs = backend
+        G = Graph(backend=backend(**kwargs))
         nxG = nx.Graph()
         G.nx.add_edge("A", "B")
         nxG.add_edge("A", "B")
         assert sorted([i for i in G.nx.neighbors("A")]) == sorted(
             [i for i in nxG.neighbors("A")]
         )
         assert sorted([i for i in G.nx.neighbors("B")]) == sorted(
@@ -194,61 +218,66 @@
             [i for i in nxG.neighbors("B")]
         )
         assert sorted([i for i in G.nx.neighbors("C")]) == sorted(
             [i for i in nxG.neighbors("C")]
         )
 
     def test_undirected_adj(self, backend):
-        G = Graph(backend=backend())
+        backend, kwargs = backend
+        G = Graph(backend=backend(**kwargs))
         nxG = nx.Graph()
         assert G.nx._adj == nxG._adj
         G.nx.add_edge("A", "B")
         nxG.add_edge("A", "B")
         assert G.nx._adj == nxG._adj
 
     def test_directed_adj(self, backend):
-        G = Graph(backend=backend(directed=True))
+        backend, kwargs = backend
+        G = Graph(backend=backend(directed=True, **kwargs))
         nxG = nx.DiGraph()
         assert G.nx._adj == nxG._adj
         G.nx.add_edge("A", "B")
         nxG.add_edge("A", "B")
         assert G.nx._adj == nxG._adj
 
     def test_can_traverse_undirected_graph(self, backend):
-        G = Graph(backend=backend())
+        backend, kwargs = backend
+        G = Graph(backend=backend(**kwargs))
         nxG = nx.Graph()
         md = dict(k="B")
         G.nx.add_edge("A", "B", **md)
         nxG.add_edge("A", "B", **md)
         assert dict(nx.bfs_successors(G.nx, "A")) == dict(nx.bfs_successors(nxG, "A"))
         G.nx.add_edge("B", "C", **md)
         nxG.add_edge("B", "C", **md)
         assert dict(nx.bfs_successors(G.nx, "A")) == dict(nx.bfs_successors(nxG, "A"))
         G.nx.add_edge("B", "D", **md)
         nxG.add_edge("B", "D", **md)
         assert dict(nx.bfs_successors(G.nx, "A")) == dict(nx.bfs_successors(nxG, "A"))
         assert dict(nx.bfs_successors(G.nx, "C")) == dict(nx.bfs_successors(nxG, "C"))
 
     def test_can_traverse_directed_graph(self, backend):
-        G = Graph(backend=backend(directed=True))
+        backend, kwargs = backend
+        G = Graph(backend=backend(directed=True, **kwargs))
         nxG = nx.DiGraph()
         md = dict(k="B")
         G.nx.add_edge("A", "B", **md)
         nxG.add_edge("A", "B", **md)
         assert dict(nx.bfs_successors(G.nx, "A")) == dict(nx.bfs_successors(nxG, "A"))
         G.nx.add_edge("B", "C", **md)
         nxG.add_edge("B", "C", **md)
         assert dict(nx.bfs_successors(G.nx, "A")) == dict(nx.bfs_successors(nxG, "A"))
         G.nx.add_edge("B", "D", **md)
         nxG.add_edge("B", "D", **md)
         assert dict(nx.bfs_successors(G.nx, "A")) == dict(nx.bfs_successors(nxG, "A"))
         assert dict(nx.bfs_successors(G.nx, "C")) == dict(nx.bfs_successors(nxG, "C"))
 
     def test_subgraph_isomorphism_undirected(self, backend):
-        G = Graph(backend=backend(directed=False))
+        backend, kwargs = backend
+        G = Graph(backend=backend(directed=False, **kwargs))
         nxG = nx.Graph()
 
         G.nx.add_edge("A", "B")
         nxG.add_edge("A", "B")
         G.nx.add_edge("B", "C")
         nxG.add_edge("B", "C")
         G.nx.add_edge("C", "A")
@@ -257,15 +286,16 @@
         from networkx.algorithms.isomorphism import GraphMatcher
 
         assert len(
             [i for i in GraphMatcher(G.nx, G.nx).subgraph_monomorphisms_iter()]
         ) == len([i for i in GraphMatcher(nxG, nxG).subgraph_monomorphisms_iter()])
 
     def test_subgraph_isomorphism_directed(self, backend):
-        G = Graph(backend=backend(directed=True))
+        backend, kwargs = backend
+        G = Graph(backend=backend(directed=True, **kwargs))
         nxG = nx.DiGraph()
 
         G.nx.add_edge("A", "B")
         nxG.add_edge("A", "B")
         G.nx.add_edge("B", "C")
         nxG.add_edge("B", "C")
         G.nx.add_edge("C", "A")
@@ -274,57 +304,64 @@
         from networkx.algorithms.isomorphism import DiGraphMatcher
 
         assert len(
             [i for i in DiGraphMatcher(G.nx, G.nx).subgraph_monomorphisms_iter()]
         ) == len([i for i in DiGraphMatcher(nxG, nxG).subgraph_monomorphisms_iter()])
 
     def test_can_get_edge_metadata(self, backend):
-        G = Graph(backend=backend())
+        backend, kwargs = backend
+        G = Graph(backend=backend(**kwargs))
         G.nx.add_edge("foo", "bar", baz=True)
         assert list(G.nx.edges(data=True)) == [("foo", "bar", {"baz": True})]
 
     def test_edge_dne_raises(self, backend):
-        G = Graph(backend=backend())
+        backend, kwargs = backend
+        G = Graph(backend=backend(**kwargs))
         G.nx.add_edge("foo", "bar", baz=True)
 
         assert G.nx.has_edge("foo", "crab") == False
         assert G.nx.has_edge("foo", "bar") == True
         # assert G.nx.edges[("foo", "bar")] != None
         # with pytest.raises(Exception):
         #     G.nx.edges[("foo", "crab")]
 
     def test_reverse_edges_in_undirected(self, backend):
-        G = Graph(backend=backend(directed=False), directed=False)
+        backend, kwargs = backend
+        G = Graph(backend=backend(directed=False, **kwargs))
         G.nx.add_edge("foo", "bar", baz=True)
 
         assert G.nx.has_edge("foo", "bar") == True
         assert G.nx.has_edge("bar", "foo") == True
 
     def test_undirected_degree(self, backend):
-        G = Graph(backend=backend(directed=False))
+        backend, kwargs = backend
+        G = Graph(backend=backend(directed=False, **kwargs))
         G.nx.add_edge("foo", "bar", baz=True)
         assert G.nx.degree("foo") == 1
         assert G.nx.degree("bar") == 1
 
     def test_directed_degree(self, backend):
-        G = Graph(backend=backend(directed=True))
+        backend, kwargs = backend
+        G = Graph(backend=backend(directed=True, **kwargs))
         G.nx.add_edge("foo", "bar", baz=True)
         assert G.nx.degree("foo") == 1
         assert G.nx.degree("bar") == 0
 
     def test_undirected_degree_multiple(self, backend):
-        G = Graph(backend=backend(directed=False))
+        backend, kwargs = backend
+        G = Graph(backend=backend(directed=False, **kwargs))
         G.nx.add_edge("foo", "bar", baz=True)
         G.nx.add_edge("foo", "baz", baz=True)
         assert G.nx.degree("foo") == 2
         assert G.nx.degree("bar") == 1
         assert G.nx.degree("baz") == 1
 
     def test_directed_degree_multiple(self, backend):
-        G = Graph(backend=backend(directed=True))
+        backend, kwargs = backend
+        G = Graph(backend=backend(directed=True, **kwargs))
         G.nx.add_edge("foo", "bar", baz=True)
         G.nx.add_edge("foo", "baz", baz=True)
         assert G.nx.degree("foo") == 2
         assert G.nx.degree("bar") == 0
         assert G.nx.degree("baz") == 0
         assert G.nx.out_degree("foo") == 2
         assert G.nx.out_degree("bar") == 0
```

### Comparing `grand-graph-0.4.2/grand/backends/test_cached_backend.py` & `grand-graph-0.5.0/grand/backends/test_cached_backend.py`

 * *Files identical despite different names*

### Comparing `grand-graph-0.4.2/grand/backends/test_metadatastore.py` & `grand-graph-0.5.0/grand/backends/test_metadatastore.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,24 @@
 
 def test_can_add_edge():
     store = DictMetadataStore()
     store.add_edge("a", "b", {"b": 2})
     assert store.get_edge("a", "b") == {"b": 2}
 
 
+def test_can_update_edge():
+    store = DictMetadataStore()
+    store.add_edge("a", "b", {"b": 2})
+    store.add_edge("a", "b", {"x": "x"})
+    store.add_edge("a", "b", {"z": "z"})
+    assert store.get_edge("a", "b")["b"] == 2
+    assert store.get_edge("a", "b")["x"] == "x"
+    assert store.get_edge("a", "b")["z"] == "z"
+
+
 def test_cannot_get_invalid_node():
     store = DictMetadataStore()
     with pytest.raises(KeyError):
         store.get_node("a")
 
 
 def test_can_create_dict_name_manager():
```

### Comparing `grand-graph-0.4.2/grand/dialects/__init__.py` & `grand-graph-0.5.0/grand/dialects/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                 neighbor: metadata
                 for neighbor, metadata in self._parent.backend.get_node_successors(
                     name, include_metadata=True
                 ).items()
             }
 
     def __len__(self):
-        return len(self._parent.backend.get_node_count())
+        return self._parent.backend.get_node_count()
 
     def __iter__(self):
         return iter(self._parent.backend.all_nodes_as_iterable(include_metadata=False))
 
     def copy(self):
         raise NotImplementedError()
 
@@ -97,17 +97,23 @@
 
         """
         self.parent = parent
 
     def add_node(self, name: Hashable, **kwargs):
         return self.parent.backend.add_node(name, kwargs)
 
+    def add_nodes_from(self, nodes_for_adding, **attr):
+        return self.parent.backend.add_nodes_from(nodes_for_adding, **attr)
+
     def add_edge(self, u: Hashable, v: Hashable, **kwargs):
         return self.parent.backend.add_edge(u, v, kwargs)
 
+    def add_edges_from(self, ebunch_to_add, **attr):
+        return self.parent.backend.add_edges_from(ebunch_to_add, **attr)
+
     def remove_node(self, name: Hashable):
         if hasattr(self.parent.backend, "remove_node"):
             return self.parent.backend.remove_node(name)
         raise NotImplementedError
 
     def remove_edge(self, u: Hashable, v: Hashable):
         raise NotImplementedError
@@ -157,20 +163,27 @@
     @property
     def _pred(self):
         """
         https://github.com/networkx/networkx/blob/master/networkx/classes/digraph.py#L323
         """
         return _GrandAdjacencyView(self, "pred")
 
+    @property
+    def graph(self):
+        return {}
+
     def in_degree(self, nbunch=None):
         return self.parent.backend.in_degrees(nbunch)
 
     def out_degree(self, nbunch=None):
         return self.parent.backend.out_degrees(nbunch)
 
+    def is_directed(self):
+        return self.parent.backend.is_directed()
+
 
 class IGraphDialect(nx.Graph):
     """
     An IGraphDialect provides a python-igraph-like interface
 
     """
 
@@ -186,15 +199,15 @@
 
         """
         self.parent = parent
 
     def add_vertices(self, num_verts: int):
         old_max = len(self.vs)
         for new_v_index in range(num_verts):
-            return self.parent.backend.add_node(new_v_index + old_max, {})
+            self.parent.backend.add_node(new_v_index + old_max, {})
 
     @property
     def vs(self):
         return [
             i for i in self.parent.backend.all_nodes_as_iterable(include_metadata=True)
         ]
 
@@ -202,15 +215,15 @@
     def es(self):
         return [
             i for i in self.parent.backend.all_edges_as_iterable(include_metadata=True)
         ]
 
     def add_edges(self, edgelist: List[Tuple[Hashable, Hashable]]):
         for (u, v) in edgelist:
-            return self.parent.backend.add_edge(u, v, {})
+            self.parent.backend.add_edge(u, v, {})
 
     def get_edgelist(self):
         return self.parent.backend.all_edges_as_iterable(include_metadata=False)
 
 
 class NetworkitDialect:
     """
@@ -222,15 +235,15 @@
     """
 
     def __init__(self, parent: "Graph") -> None:
         self.parent = parent
 
     def addNode(self):
         new_id = self.parent.backend.get_node_count()
-        self.parent.backend.add_node(new_id)
+        self.parent.backend.add_node(new_id, {})
         return new_id
 
     def addEdge(self, u: Hashable, v: Hashable) -> None:
         self.parent.backend.add_edge(u, v, {})
 
     def nodes(self):
         return [i for i in self.iterNodes()]
```

### Comparing `grand-graph-0.4.2/grand_graph.egg-info/PKG-INFO` & `grand-graph-0.5.0/grand_graph.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: grand-graph
-Version: 0.4.2
+Version: 0.5.0
 Summary: Graph database wrapper for non-graph datastores
 Home-page: https://github.com/aplbrain/grand
 Author: Jordan Matelsky
 Author-email: opensource@matelsky.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: sql
 Provides-Extra: dynamodb
 Provides-Extra: igraph
 Provides-Extra: networkit
 License-File: LICENSE
 
 <div align=center><img src="docs/grand.png" width=400 /></div>
 
-<div align=center><a href="https://pypi.org/project/grand-graph/"><img src="https://img.shields.io/pypi/v/grand-graph?style=for-the-badge" /></a> <a href="https://app.codecov.io/gh/aplbrain/grand"><img alt="Codecov" src="https://img.shields.io/codecov/c/github/aplbrain/grand?style=for-the-badge"></a> <img alt="GitHub Workflow Status" src="https://img.shields.io/github/workflow/status/aplbrain/grand/Python%20package?style=for-the-badge"></div>
+<div align=center><a href="https://pypi.org/project/grand-graph/"><img src="https://img.shields.io/pypi/v/grand-graph?style=for-the-badge" /></a> <a href="https://app.codecov.io/gh/aplbrain/grand"><img alt="Codecov" src="https://img.shields.io/codecov/c/github/aplbrain/grand?style=for-the-badge"></a></div>
+
+<!--  <a href="https://github.com/aplbrain/grand/actions/workflows/python-package.yml"><img alt="GitHub Workflow Status (with branch)" src="https://img.shields.io/github/actions/workflow/status/aplbrain/grand/python-package.yml?style=for-the-badge"></a> -->
 
 <br />
 
 <p align=center>Graph toolkit interoperability and scalability for Python</p>
 
 ## Installation
 
@@ -149,9 +149,7 @@
     month={Jun}
 }
 ```
 
 ---
 
 <p align=center><b>Made with 💙 at <a href="https://jhuapl.edu"><img alt="JHU APL" src="https://user-images.githubusercontent.com/693511/116814564-9b268800-ab27-11eb-98bb-dfddb2e405a1.png" height="23px" /></a></b></p>
-
-
```

#### html2text {}

```diff
@@ -1,18 +1,16 @@
-Metadata-Version: 2.1 Name: grand-graph Version: 0.4.2 Summary: Graph database
+Metadata-Version: 2.1 Name: grand-graph Version: 0.5.0 Summary: Graph database
 wrapper for non-graph datastores Home-page: https://github.com/aplbrain/grand
-Author: Jordan Matelsky Author-email: opensource@matelsky.com License: UNKNOWN
-Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Description-Content-Type: text/markdown Provides-Extra: sql
-Provides-Extra: dynamodb Provides-Extra: igraph Provides-Extra: networkit
-License-File: LICENSE
+Author: Jordan Matelsky Author-email: opensource@matelsky.com Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Description-Content-
+Type: text/markdown Provides-Extra: sql Provides-Extra: dynamodb Provides-
+Extra: igraph Provides-Extra: networkit License-File: LICENSE
                                [docs/grand.png]
-_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_g_r_a_n_d_-_g_r_a_p_h_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_C_o_d_e_c_o_v_][GitHub
-                               Workflow Status]
+   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_g_r_a_n_d_-_g_r_a_p_h_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_C_o_d_e_c_o_v_]
 
            Graph toolkit interoperability and scalability for Python
 ## Installation ```shell pip install grand-graph ``` ## Example use-cases -
 Write NetworkX commands to analyze true-serverless graph databases using
 DynamoDB\* - Query a host graph in SQL for subgraph isomorphisms with DotMotif
 - Write iGraph code to construct a graph, and then play with it in Networkit -
 Attach node and edge attributes to Networkit or IGraph graphs > \* [Neptune is
```

### Comparing `grand-graph-0.4.2/grand_graph.egg-info/SOURCES.txt` & `grand-graph-0.5.0/grand_graph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grand-graph-0.4.2/setup.py` & `grand-graph-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="grand-graph",
-    version="0.4.2",
+    version="0.5.0",
     author="Jordan Matelsky",
     author_email="opensource@matelsky.com",
     description="Graph database wrapper for non-graph datastores",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aplbrain/grand",
     packages=setuptools.find_packages(),
```

