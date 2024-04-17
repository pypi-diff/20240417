# Comparing `tmp/cardiac_geometries-1.1.2.tar.gz` & `tmp/cardiac_geometries-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardiac_geometries-1.1.2.tar", last modified: Tue Apr  2 19:43:46 2024, max compression
+gzip compressed data, was "cardiac_geometries-1.1.3.tar", last modified: Wed Apr 17 06:26:42 2024, max compression
```

## Comparing `cardiac_geometries-1.1.2.tar` & `cardiac_geometries-1.1.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 19:43:46.012398 cardiac_geometries-1.1.2/
--rw-r--r--   0 root         (0) root         (0)     1072 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3096 2024-04-02 19:43:46.012398 cardiac_geometries-1.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1730 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/README.md
--rw-r--r--   0 root         (0) root         (0)     2983 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 19:43:46.012398 cardiac_geometries-1.1.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 19:43:46.004398 cardiac_geometries-1.1.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 19:43:46.008398 cardiac_geometries-1.1.2/src/cardiac_geometries/
--rw-r--r--   0 root         (0) root         (0)     1650 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/__init__.py
--rw-r--r--   0 root         (0) root         (0)       77 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/__main__.py
--rw-r--r--   0 root         (0) root         (0)      620 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/_import_checks.py
--rw-r--r--   0 root         (0) root         (0)    28768 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/_mesh.py
--rw-r--r--   0 root         (0) root         (0)     4247 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/aha.py
--rw-r--r--   0 root         (0) root         (0)     4165 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/calculus.py
--rw-r--r--   0 root         (0) root         (0)    23522 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/cli.py
--rw-r--r--   0 root         (0) root         (0)     5070 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/dolfin_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 19:43:46.012398 cardiac_geometries-1.1.2/src/cardiac_geometries/fibers/
--rw-r--r--   0 root         (0) root         (0)      133 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/fibers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4517 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/fibers/_biv_ellipsoid.py
--rw-r--r--   0 root         (0) root         (0)     6592 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/fibers/_lv_ellipsoid.py
--rw-r--r--   0 root         (0) root         (0)     5783 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/fibers/_slab.py
--rw-r--r--   0 root         (0) root         (0)     2104 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/fibers/_utils.py
--rw-r--r--   0 root         (0) root         (0)    16869 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/geometry.py
--rw-r--r--   0 root         (0) root         (0)      254 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/utils.py
--rw-r--r--   0 root         (0) root         (0)    10038 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/viz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 19:43:46.012398 cardiac_geometries-1.1.2/src/cardiac_geometries.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3096 2024-04-02 19:43:45.000000 cardiac_geometries-1.1.2/src/cardiac_geometries.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      986 2024-04-02 19:43:46.000000 cardiac_geometries-1.1.2/src/cardiac_geometries.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 19:43:45.000000 cardiac_geometries-1.1.2/src/cardiac_geometries.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2024-04-02 19:43:46.000000 cardiac_geometries-1.1.2/src/cardiac_geometries.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 19:43:36.000000 cardiac_geometries-1.1.2/src/cardiac_geometries.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      234 2024-04-02 19:43:46.000000 cardiac_geometries-1.1.2/src/cardiac_geometries.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-04-02 19:43:46.000000 cardiac_geometries-1.1.2/src/cardiac_geometries.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 19:43:46.012398 cardiac_geometries-1.1.2/tests/
--rw-r--r--   0 root         (0) root         (0)     3396 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     4553 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/tests/test_geometry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 06:26:42.261170 cardiac_geometries-1.1.3/
+-rw-r--r--   0 root         (0) root         (0)     1072 2024-04-17 06:26:32.000000 cardiac_geometries-1.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3096 2024-04-17 06:26:42.261170 cardiac_geometries-1.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-04-17 06:26:32.000000 cardiac_geometries-1.1.3/README.md
+-rw-r--r--   0 root         (0) root         (0)     2983 2024-04-17 06:26:32.000000 cardiac_geometries-1.1.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 06:26:42.261170 cardiac_geometries-1.1.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 06:26:42.253169 cardiac_geometries-1.1.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 06:26:42.257169 cardiac_geometries-1.1.3/src/cardiac_geometries/
+-rw-r--r--   0 root         (0) root         (0)     1650 2024-04-17 06:26:32.000000 cardiac_geometries-1.1.3/src/cardiac_geometries/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       77 2024-04-17 06:26:32.000000 cardiac_geometries-1.1.3/src/cardiac_geometries/__main__.py
+-rw-r--r--   0 root         (0) root         (0)      620 2024-04-17 06:26:32.000000 cardiac_geometries-1.1.3/src/cardiac_geometries/_import_checks.py
+-rw-r--r--   0 root         (0) root         (0)    28768 2024-04-17 06:26:32.000000 cardiac_geometries-1.1.3/src/cardiac_geometries/_mesh.py
+-rw-r--r--   0 root         (0) root         (0)     4247 2024-04-17 06:26:32.000000 cardiac_geometries-1.1.3/src/cardiac_geometries/aha.py
+-rw-r--r--   0 root         (0) root         (0)     4165 2024-04-17 06:26:32.000000 cardiac_geometries-1.1.3/src/cardiac_geometries/calculus.py
+-rw-r--r--   0 root         (0) root         (0)    23522 2024-04-17 06:26:32.000000 cardiac_geometries-1.1.3/src/cardiac_geometries/cli.py
+-rw-r--r--   0 root         (0) root         (0)     5070 2024-04-17 06:26:32.000000 cardiac_geometries-1.1.3/src/cardiac_geometries/dolfin_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 06:26:42.261170 cardiac_geometries-1.1.3/src/cardiac_geometries/fibers/
+-rw-r--r--   0 root         (0) root         (0)      133 2024-04-17 06:26:32.000000 cardiac_geometries-1.1.3/src/cardiac_geometries/fibers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4517 2024-04-17 06:26:32.000000 cardiac_geometries-1.1.3/src/cardiac_geometries/fibers/_biv_ellipsoid.py
+-rw-r--r--   0 root         (0) root         (0)     6592 2024-04-17 06:26:32.000000 cardiac_geometries-1.1.3/src/cardiac_geometries/fibers/_lv_ellipsoid.py
+-rw-r--r--   0 root         (0) root         (0)     5783 2024-04-17 06:26:32.000000 cardiac_geometries-1.1.3/src/cardiac_geometries/fibers/_slab.py
+-rw-r--r--   0 root         (0) root         (0)     2104 2024-04-17 06:26:32.000000 cardiac_geometries-1.1.3/src/cardiac_geometries/fibers/_utils.py
+-rw-r--r--   0 root         (0) root         (0)    16803 2024-04-17 06:26:32.000000 cardiac_geometries-1.1.3/src/cardiac_geometries/geometry.py
+-rw-r--r--   0 root         (0) root         (0)      254 2024-04-17 06:26:32.000000 cardiac_geometries-1.1.3/src/cardiac_geometries/utils.py
+-rw-r--r--   0 root         (0) root         (0)    10038 2024-04-17 06:26:32.000000 cardiac_geometries-1.1.3/src/cardiac_geometries/viz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 06:26:42.261170 cardiac_geometries-1.1.3/src/cardiac_geometries.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3096 2024-04-17 06:26:42.000000 cardiac_geometries-1.1.3/src/cardiac_geometries.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      986 2024-04-17 06:26:42.000000 cardiac_geometries-1.1.3/src/cardiac_geometries.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 06:26:42.000000 cardiac_geometries-1.1.3/src/cardiac_geometries.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2024-04-17 06:26:42.000000 cardiac_geometries-1.1.3/src/cardiac_geometries.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 06:26:34.000000 cardiac_geometries-1.1.3/src/cardiac_geometries.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      234 2024-04-17 06:26:42.000000 cardiac_geometries-1.1.3/src/cardiac_geometries.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-04-17 06:26:42.000000 cardiac_geometries-1.1.3/src/cardiac_geometries.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 06:26:42.261170 cardiac_geometries-1.1.3/tests/
+-rw-r--r--   0 root         (0) root         (0)     3396 2024-04-17 06:26:32.000000 cardiac_geometries-1.1.3/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     4553 2024-04-17 06:26:32.000000 cardiac_geometries-1.1.3/tests/test_geometry.py
```

### Comparing `cardiac_geometries-1.1.2/LICENSE` & `cardiac_geometries-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-1.1.2/PKG-INFO` & `cardiac_geometries-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardiac_geometries
-Version: 1.1.2
+Version: 1.1.3
 Summary: A python library for cardiac geometries
 Author-email: Henrik Finsberg <henriknf@simula.no>
 License: MIT
 Project-URL: Homepage, https://github.com/ComputationalPhysiology/cardiac_geometries
 Keywords: cardiac,geometry,mesh,gmsh
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cardiac_geometries-1.1.2/README.md` & `cardiac_geometries-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-1.1.2/pyproject.toml` & `cardiac_geometries-1.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cardiac_geometries"
-version = "1.1.2"
+version = "1.1.3"
 description = "A python library for cardiac geometries"
 authors = [{name = "Henrik Finsberg", email = "henriknf@simula.no"}]
 license = {text = "MIT"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
@@ -136,14 +136,14 @@
 allow_dirty = false
 commit = true
 message = "Bump version: {current_version} → {new_version}"
 tag = true
 sign_tags = false
 tag_name = "v{new_version}"
 tag_message = "Bump version: {current_version} → {new_version}"
-current_version = "1.1.2"
+current_version = "1.1.3"
 
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `cardiac_geometries-1.1.2/src/cardiac_geometries/__init__.py` & `cardiac_geometries-1.1.3/src/cardiac_geometries/__init__.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-1.1.2/src/cardiac_geometries/_import_checks.py` & `cardiac_geometries-1.1.3/src/cardiac_geometries/_import_checks.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-1.1.2/src/cardiac_geometries/_mesh.py` & `cardiac_geometries-1.1.3/src/cardiac_geometries/_mesh.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-1.1.2/src/cardiac_geometries/aha.py` & `cardiac_geometries-1.1.3/src/cardiac_geometries/aha.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-1.1.2/src/cardiac_geometries/calculus.py` & `cardiac_geometries-1.1.3/src/cardiac_geometries/calculus.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-1.1.2/src/cardiac_geometries/cli.py` & `cardiac_geometries-1.1.3/src/cardiac_geometries/cli.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-1.1.2/src/cardiac_geometries/dolfin_utils.py` & `cardiac_geometries-1.1.3/src/cardiac_geometries/dolfin_utils.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-1.1.2/src/cardiac_geometries/fibers/_biv_ellipsoid.py` & `cardiac_geometries-1.1.3/src/cardiac_geometries/fibers/_biv_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-1.1.2/src/cardiac_geometries/fibers/_lv_ellipsoid.py` & `cardiac_geometries-1.1.3/src/cardiac_geometries/fibers/_lv_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-1.1.2/src/cardiac_geometries/fibers/_slab.py` & `cardiac_geometries-1.1.3/src/cardiac_geometries/fibers/_slab.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-1.1.2/src/cardiac_geometries/fibers/_utils.py` & `cardiac_geometries-1.1.3/src/cardiac_geometries/fibers/_utils.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-1.1.2/src/cardiac_geometries/geometry.py` & `cardiac_geometries-1.1.3/src/cardiac_geometries/geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,26 +8,23 @@
 from typing import Dict
 from typing import NamedTuple
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Union
 
-try:
-    import dolfin
-    from ufl_legacy import FiniteElement  # noqa: F401
-    from ufl_legacy import tetrahedron  # noqa: F401
-    from ufl_legacy import Cell  # noqa: F401
-    from ufl_legacy import VectorElement  # noqa: F401
+import dolfin
+from ufl_legacy import FiniteElement  # noqa: F401
+from ufl_legacy import tetrahedron  # noqa: F401
+from ufl_legacy import Cell  # noqa: F401
+from ufl_legacy import VectorElement  # noqa: F401
 
-    from .viz import dict_to_h5
-    from .viz import h5_to_dict
-    from .viz import h5pyfile
-except ImportError:
-    pass
+from .viz import dict_to_h5
+from .viz import h5_to_dict
+from .viz import h5pyfile
 
 logger = logging.getLogger(__name__)
 
 
 class MeshTypes(Enum):
     slab = auto()
     lv_ellipsoid = auto()
```

### Comparing `cardiac_geometries-1.1.2/src/cardiac_geometries/viz.py` & `cardiac_geometries-1.1.3/src/cardiac_geometries/viz.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-1.1.2/src/cardiac_geometries.egg-info/PKG-INFO` & `cardiac_geometries-1.1.3/src/cardiac_geometries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardiac_geometries
-Version: 1.1.2
+Version: 1.1.3
 Summary: A python library for cardiac geometries
 Author-email: Henrik Finsberg <henriknf@simula.no>
 License: MIT
 Project-URL: Homepage, https://github.com/ComputationalPhysiology/cardiac_geometries
 Keywords: cardiac,geometry,mesh,gmsh
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cardiac_geometries-1.1.2/src/cardiac_geometries.egg-info/SOURCES.txt` & `cardiac_geometries-1.1.3/src/cardiac_geometries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-1.1.2/tests/test_cli.py` & `cardiac_geometries-1.1.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-1.1.2/tests/test_geometry.py` & `cardiac_geometries-1.1.3/tests/test_geometry.py`

 * *Files identical despite different names*

