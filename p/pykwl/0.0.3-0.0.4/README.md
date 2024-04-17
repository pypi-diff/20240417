# Comparing `tmp/pykwl-0.0.3.tar.gz` & `tmp/pykwl-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykwl-0.0.3.tar", last modified: Wed Apr 17 14:16:22 2024, max compression
+gzip compressed data, was "pykwl-0.0.4.tar", last modified: Wed Apr 17 16:47:56 2024, max compression
```

## Comparing `pykwl-0.0.3.tar` & `pykwl-0.0.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:22.290118 pykwl-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-17 14:16:07.000000 pykwl-0.0.3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-17 14:16:07.000000 pykwl-0.0.3/Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-17 14:16:07.000000 pykwl-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-17 14:16:07.000000 pykwl-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-17 14:16:22.290118 pykwl-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-17 14:16:07.000000 pykwl-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:22.286118 pykwl-0.0.3/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-17 14:16:07.000000 pykwl-0.0.3/cmake/configure_ccache.cmake
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:22.286118 pykwl-0.0.3/dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-17 14:16:07.000000 pykwl-0.0.3/dependencies/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:22.286118 pykwl-0.0.3/dependencies/pybind11/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-17 14:16:07.000000 pykwl-0.0.3/dependencies/pybind11/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:22.286118 pykwl-0.0.3/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:22.286118 pykwl-0.0.3/include/wl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:22.286118 pykwl-0.0.3/include/wl/details/
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-17 14:16:07.000000 pykwl-0.0.3/include/wl/details/graph.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-17 14:16:07.000000 pykwl-0.0.3/include/wl/details/weisfeiler_leman.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-17 14:16:07.000000 pykwl-0.0.3/include/wl/wl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-17 14:16:07.000000 pykwl-0.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:22.286118 pykwl-0.0.3/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:22.290118 pykwl-0.0.3/python/src/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-17 14:16:07.000000 pykwl-0.0.3/python/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-17 14:16:07.000000 pykwl-0.0.3/python/src/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:22.290118 pykwl-0.0.3/python/src/pykwl/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-17 14:16:07.000000 pykwl-0.0.3/python/src/pykwl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-17 14:16:07.000000 pykwl-0.0.3/python/src/pykwl/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-17 14:16:07.000000 pykwl-0.0.3/python/src/pykwl/bindings.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:22.290118 pykwl-0.0.3/python/src/pykwl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-17 14:16:22.000000 pykwl-0.0.3/python/src/pykwl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-17 14:16:22.000000 pykwl-0.0.3/python/src/pykwl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 14:16:22.000000 pykwl-0.0.3/python/src/pykwl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 14:16:22.000000 pykwl-0.0.3/python/src/pykwl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-17 14:16:22.000000 pykwl-0.0.3/python/src/pykwl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 14:16:22.000000 pykwl-0.0.3/python/src/pykwl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 14:16:22.290118 pykwl-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-17 14:16:07.000000 pykwl-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:22.290118 pykwl-0.0.3/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-17 14:16:07.000000 pykwl-0.0.3/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-17 14:16:07.000000 pykwl-0.0.3/src/graph.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-04-17 14:16:07.000000 pykwl-0.0.3/src/weisfeiler_leman.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:22.290118 pykwl-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:07.000000 pykwl-0.0.3/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:22.290118 pykwl-0.0.3/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:07.000000 pykwl-0.0.3/tests/unit/CMakeLists copy.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:07.000000 pykwl-0.0.3/tests/unit/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:56.826912 pykwl-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-17 16:47:44.000000 pykwl-0.0.4/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-17 16:47:44.000000 pykwl-0.0.4/Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-17 16:47:44.000000 pykwl-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-17 16:47:44.000000 pykwl-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-17 16:47:56.826912 pykwl-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-17 16:47:44.000000 pykwl-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:56.822912 pykwl-0.0.4/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-17 16:47:44.000000 pykwl-0.0.4/cmake/configure_ccache.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:56.822912 pykwl-0.0.4/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-17 16:47:44.000000 pykwl-0.0.4/dependencies/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:56.826912 pykwl-0.0.4/dependencies/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-17 16:47:44.000000 pykwl-0.0.4/dependencies/pybind11/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:56.822912 pykwl-0.0.4/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:56.826912 pykwl-0.0.4/include/wl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:56.826912 pykwl-0.0.4/include/wl/details/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-17 16:47:44.000000 pykwl-0.0.4/include/wl/details/graph.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-17 16:47:44.000000 pykwl-0.0.4/include/wl/details/weisfeiler_leman.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-17 16:47:44.000000 pykwl-0.0.4/include/wl/wl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-17 16:47:44.000000 pykwl-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:56.822912 pykwl-0.0.4/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:56.826912 pykwl-0.0.4/python/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-17 16:47:44.000000 pykwl-0.0.4/python/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-17 16:47:44.000000 pykwl-0.0.4/python/src/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:56.826912 pykwl-0.0.4/python/src/pykwl/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-17 16:47:44.000000 pykwl-0.0.4/python/src/pykwl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-17 16:47:44.000000 pykwl-0.0.4/python/src/pykwl/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-17 16:47:44.000000 pykwl-0.0.4/python/src/pykwl/bindings.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:56.826912 pykwl-0.0.4/python/src/pykwl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-17 16:47:56.000000 pykwl-0.0.4/python/src/pykwl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-17 16:47:56.000000 pykwl-0.0.4/python/src/pykwl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:47:56.000000 pykwl-0.0.4/python/src/pykwl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:47:56.000000 pykwl-0.0.4/python/src/pykwl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-17 16:47:56.000000 pykwl-0.0.4/python/src/pykwl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 16:47:56.000000 pykwl-0.0.4/python/src/pykwl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 16:47:56.826912 pykwl-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-17 16:47:44.000000 pykwl-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:56.826912 pykwl-0.0.4/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-17 16:47:44.000000 pykwl-0.0.4/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-17 16:47:44.000000 pykwl-0.0.4/src/graph.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-04-17 16:47:44.000000 pykwl-0.0.4/src/weisfeiler_leman.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:56.826912 pykwl-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:44.000000 pykwl-0.0.4/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:56.826912 pykwl-0.0.4/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:44.000000 pykwl-0.0.4/tests/unit/CMakeLists copy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:47:44.000000 pykwl-0.0.4/tests/unit/CMakeLists.txt
```

### Comparing `pykwl-0.0.3/CMakeLists.txt` & `pykwl-0.0.4/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.3/Config.cmake.in` & `pykwl-0.0.4/Config.cmake.in`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.3/LICENSE` & `pykwl-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.3/README.md` & `pykwl-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.3/cmake/configure_ccache.cmake` & `pykwl-0.0.4/cmake/configure_ccache.cmake`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.3/dependencies/pybind11/CMakeLists.txt` & `pykwl-0.0.4/dependencies/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.3/include/wl/details/graph.hpp` & `pykwl-0.0.4/include/wl/details/graph.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     std::vector<int> m_edge_sources;
     std::vector<int> m_edge_destinations;
     std::vector<int> m_node_labels;
     std::vector<int> m_edge_labels;
     bool m_directed;
 
 public:
-    Graph(bool directed);
+    explicit Graph(bool directed);
 
     int add_node(int label = 0);
 
     void add_edge(int src_node, int dst_node, int label = 0);
 
     int get_source(int edge) const;
```

### Comparing `pykwl-0.0.3/include/wl/details/weisfeiler_leman.hpp` & `pykwl-0.0.4/include/wl/details/weisfeiler_leman.hpp`

 * *Files 24% similar despite different names*

```diff
@@ -14,19 +14,21 @@
 {
 private:
     using ColorMultiset = std::tuple<int, std::vector<int>, std::vector<int>, std::vector<int>, std::vector<int>>;
 
     std::map<ColorMultiset, int> m_color_function;
     int m_k;
 
-    int get_color_k1(ColorMultiset&& key);
+    int get_color(ColorMultiset&& key);
 
-    std::tuple<int, std::vector<int>, std::vector<int>> compute_coloring_k1(const Graph& graph);
+    int get_subgraph_color(int src_node, int dst_node, const Graph& graph);
 
-    std::tuple<int, std::vector<int>, std::vector<int>> compute_coloring_k2(const Graph& graph);
+    std::tuple<int, std::vector<int>, std::vector<int>> k1_fwl(const Graph& graph);
+
+    std::tuple<int, std::vector<int>, std::vector<int>> k2_fwl(const Graph& graph);
 
 public:
     explicit WeisfeilerLeman(int k);
 
     std::tuple<int, std::vector<int>, std::vector<int>> compute_coloring(const Graph& graph);
 };
```

### Comparing `pykwl-0.0.3/pyproject.toml` & `pykwl-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.3/python/src/pykwl/bindings.cpp` & `pykwl-0.0.4/python/src/pykwl/bindings.cpp`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.3/python/src/pykwl.egg-info/SOURCES.txt` & `pykwl-0.0.4/python/src/pykwl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.3/setup.py` & `pykwl-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import multiprocessing
 
 from pathlib import Path
 
 from setuptools import setup, find_packages, Extension
 from setuptools.command.build_ext import build_ext
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 HERE = Path(__file__).resolve().parent
 
 
 # A CMakeExtension needs a sourcedir instead of a file list.
 # The name must be the _single_ output extension from the CMake build.
 # If you need multiple extensions, see scikit-build.
 class CMakeExtension(Extension):
```

### Comparing `pykwl-0.0.3/src/CMakeLists.txt` & `pykwl-0.0.4/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.3/src/graph.cpp` & `pykwl-0.0.4/src/graph.cpp`

 * *Files identical despite different names*

