# Comparing `tmp/pykwl-0.0.2.tar.gz` & `tmp/pykwl-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykwl-0.0.2.tar", last modified: Wed Apr 17 12:52:26 2024, max compression
+gzip compressed data, was "pykwl-0.0.3.tar", last modified: Wed Apr 17 14:16:22 2024, max compression
```

## Comparing `pykwl-0.0.2.tar` & `pykwl-0.0.3.tar`

### file list

```diff
@@ -1,42 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:52:26.052431 pykwl-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-17 12:52:12.000000 pykwl-0.0.2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-17 12:52:12.000000 pykwl-0.0.2/Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-17 12:52:12.000000 pykwl-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-17 12:52:12.000000 pykwl-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-17 12:52:26.052431 pykwl-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-17 12:52:12.000000 pykwl-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:52:26.048431 pykwl-0.0.2/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-17 12:52:12.000000 pykwl-0.0.2/cmake/configure_ccache.cmake
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:52:26.048431 pykwl-0.0.2/dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-17 12:52:12.000000 pykwl-0.0.2/dependencies/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:52:26.048431 pykwl-0.0.2/dependencies/pybind11/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-17 12:52:12.000000 pykwl-0.0.2/dependencies/pybind11/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:52:26.048431 pykwl-0.0.2/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:52:26.048431 pykwl-0.0.2/include/wl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:52:26.048431 pykwl-0.0.2/include/wl/details/
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-17 12:52:12.000000 pykwl-0.0.2/include/wl/details/graph.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-17 12:52:12.000000 pykwl-0.0.2/include/wl/details/weisfeiler_leman.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-17 12:52:12.000000 pykwl-0.0.2/include/wl/wl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-17 12:52:12.000000 pykwl-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:52:26.048431 pykwl-0.0.2/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:52:26.048431 pykwl-0.0.2/python/src/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-17 12:52:12.000000 pykwl-0.0.2/python/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-17 12:52:12.000000 pykwl-0.0.2/python/src/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:52:26.052431 pykwl-0.0.2/python/src/pykwl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-17 12:52:26.000000 pykwl-0.0.2/python/src/pykwl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-17 12:52:26.000000 pykwl-0.0.2/python/src/pykwl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 12:52:26.000000 pykwl-0.0.2/python/src/pykwl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 12:52:26.000000 pykwl-0.0.2/python/src/pykwl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-17 12:52:26.000000 pykwl-0.0.2/python/src/pykwl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 12:52:26.000000 pykwl-0.0.2/python/src/pykwl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 12:52:26.052431 pykwl-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-17 12:52:12.000000 pykwl-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:52:26.052431 pykwl-0.0.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-17 12:52:12.000000 pykwl-0.0.2/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-17 12:52:12.000000 pykwl-0.0.2/src/graph.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-04-17 12:52:12.000000 pykwl-0.0.2/src/weisfeiler_leman.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:52:26.052431 pykwl-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 12:52:12.000000 pykwl-0.0.2/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:52:26.052431 pykwl-0.0.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 12:52:12.000000 pykwl-0.0.2/tests/unit/CMakeLists copy.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 12:52:12.000000 pykwl-0.0.2/tests/unit/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:22.290118 pykwl-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-17 14:16:07.000000 pykwl-0.0.3/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-17 14:16:07.000000 pykwl-0.0.3/Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-17 14:16:07.000000 pykwl-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-17 14:16:07.000000 pykwl-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-17 14:16:22.290118 pykwl-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-17 14:16:07.000000 pykwl-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:22.286118 pykwl-0.0.3/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-17 14:16:07.000000 pykwl-0.0.3/cmake/configure_ccache.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:22.286118 pykwl-0.0.3/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-17 14:16:07.000000 pykwl-0.0.3/dependencies/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:22.286118 pykwl-0.0.3/dependencies/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-17 14:16:07.000000 pykwl-0.0.3/dependencies/pybind11/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:22.286118 pykwl-0.0.3/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:22.286118 pykwl-0.0.3/include/wl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:22.286118 pykwl-0.0.3/include/wl/details/
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-17 14:16:07.000000 pykwl-0.0.3/include/wl/details/graph.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-17 14:16:07.000000 pykwl-0.0.3/include/wl/details/weisfeiler_leman.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-17 14:16:07.000000 pykwl-0.0.3/include/wl/wl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-17 14:16:07.000000 pykwl-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:22.286118 pykwl-0.0.3/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:22.290118 pykwl-0.0.3/python/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-17 14:16:07.000000 pykwl-0.0.3/python/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-17 14:16:07.000000 pykwl-0.0.3/python/src/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:22.290118 pykwl-0.0.3/python/src/pykwl/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-17 14:16:07.000000 pykwl-0.0.3/python/src/pykwl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-17 14:16:07.000000 pykwl-0.0.3/python/src/pykwl/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-17 14:16:07.000000 pykwl-0.0.3/python/src/pykwl/bindings.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:22.290118 pykwl-0.0.3/python/src/pykwl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-17 14:16:22.000000 pykwl-0.0.3/python/src/pykwl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-17 14:16:22.000000 pykwl-0.0.3/python/src/pykwl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 14:16:22.000000 pykwl-0.0.3/python/src/pykwl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 14:16:22.000000 pykwl-0.0.3/python/src/pykwl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-17 14:16:22.000000 pykwl-0.0.3/python/src/pykwl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 14:16:22.000000 pykwl-0.0.3/python/src/pykwl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 14:16:22.290118 pykwl-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-17 14:16:07.000000 pykwl-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:22.290118 pykwl-0.0.3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-17 14:16:07.000000 pykwl-0.0.3/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-17 14:16:07.000000 pykwl-0.0.3/src/graph.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-04-17 14:16:07.000000 pykwl-0.0.3/src/weisfeiler_leman.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:22.290118 pykwl-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:07.000000 pykwl-0.0.3/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:22.290118 pykwl-0.0.3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:07.000000 pykwl-0.0.3/tests/unit/CMakeLists copy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 14:16:07.000000 pykwl-0.0.3/tests/unit/CMakeLists.txt
```

### Comparing `pykwl-0.0.2/CMakeLists.txt` & `pykwl-0.0.3/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.2/Config.cmake.in` & `pykwl-0.0.3/Config.cmake.in`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.2/LICENSE` & `pykwl-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.2/README.md` & `pykwl-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.2/cmake/configure_ccache.cmake` & `pykwl-0.0.3/cmake/configure_ccache.cmake`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.2/dependencies/pybind11/CMakeLists.txt` & `pykwl-0.0.3/dependencies/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.2/include/wl/details/graph.hpp` & `pykwl-0.0.3/include/wl/details/graph.hpp`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.2/include/wl/details/weisfeiler_leman.hpp` & `pykwl-0.0.3/include/wl/details/weisfeiler_leman.hpp`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.2/pyproject.toml` & `pykwl-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.2/python/src/pykwl.egg-info/SOURCES.txt` & `pykwl-0.0.3/python/src/pykwl.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 dependencies/CMakeLists.txt
 dependencies/pybind11/CMakeLists.txt
 include/wl/wl.hpp
 include/wl/details/graph.hpp
 include/wl/details/weisfeiler_leman.hpp
 python/src/CMakeLists.txt
 python/src/main.cpp
+python/src/pykwl/__init__.py
+python/src/pykwl/__init__.pyi
+python/src/pykwl/bindings.cpp
 python/src/pykwl.egg-info/PKG-INFO
 python/src/pykwl.egg-info/SOURCES.txt
 python/src/pykwl.egg-info/dependency_links.txt
 python/src/pykwl.egg-info/not-zip-safe
 python/src/pykwl.egg-info/requires.txt
 python/src/pykwl.egg-info/top_level.txt
 src/CMakeLists.txt
```

### Comparing `pykwl-0.0.2/setup.py` & `pykwl-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import multiprocessing
 
 from pathlib import Path
 
 from setuptools import setup, find_packages, Extension
 from setuptools.command.build_ext import build_ext
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 HERE = Path(__file__).resolve().parent
 
 
 # A CMakeExtension needs a sourcedir instead of a file list.
 # The name must be the _single_ output extension from the CMake build.
 # If you need multiple extensions, see scikit-build.
 class CMakeExtension(Extension):
```

### Comparing `pykwl-0.0.2/src/CMakeLists.txt` & `pykwl-0.0.3/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.2/src/graph.cpp` & `pykwl-0.0.3/src/graph.cpp`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.2/src/weisfeiler_leman.cpp` & `pykwl-0.0.3/src/weisfeiler_leman.cpp`

 * *Files identical despite different names*

