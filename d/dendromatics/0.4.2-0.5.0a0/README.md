# Comparing `tmp/dendromatics-0.4.2.tar.gz` & `tmp/dendromatics-0.5.0a0.tar.gz`

## Comparing `dendromatics-0.4.2.tar` & `dendromatics-0.5.0a0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 dendromatics-0.4.2/CHANGELOG.md
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 dendromatics-0.4.2/readthedocs.yaml
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 dendromatics-0.4.2/.github/workflows/build.yml
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 dendromatics-0.4.2/.github/workflows/test.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 dendromatics-0.4.2/docs/Makefile
--rw-r--r--   0        0        0     7188 2020-02-02 00:00:00.000000 dendromatics-0.4.2/docs/algorithm.rst
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 dendromatics-0.4.2/docs/cc_plugin.rst
--rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 dendromatics-0.4.2/docs/conf.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 dendromatics-0.4.2/docs/dendromatics.rst
--rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 dendromatics-0.4.2/docs/examples.rst
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 dendromatics-0.4.2/docs/executable.rst
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 dendromatics-0.4.2/docs/index.rst
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 dendromatics-0.4.2/docs/installation.rst
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 dendromatics-0.4.2/docs/make.bat
--rw-r--r--   0        0        0   252269 2020-02-02 00:00:00.000000 dendromatics-0.4.2/docs/_static/3dfin_logo.png
--rw-r--r--   0        0        0   270012 2020-02-02 00:00:00.000000 dendromatics-0.4.2/docs/_static/dendromatics_logo.png
--rw-r--r--   0        0        0   113056 2020-02-02 00:00:00.000000 dendromatics-0.4.2/docs/_static/height-normalization.jpg
--rw-r--r--   0        0        0    45823 2020-02-02 00:00:00.000000 dendromatics-0.4.2/docs/_static/individualized_trees.jpg
--rw-r--r--   0        0        0   109342 2020-02-02 00:00:00.000000 dendromatics-0.4.2/docs/_static/sections_and_axes.jpg
--rw-r--r--   0        0        0   210688 2020-02-02 00:00:00.000000 dendromatics-0.4.2/docs/_static/stripe_and_groups.jpg
--rw-r--r--   0        0        0    29602 2020-02-02 00:00:00.000000 dendromatics-0.4.2/docs/_static/tree_height.jpg
--rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 dendromatics-0.4.2/examples/example.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 dendromatics-0.4.2/src/dendromatics/__about__.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 dendromatics-0.4.2/src/dendromatics/__init__.py
--rw-r--r--   0        0        0    13668 2020-02-02 00:00:00.000000 dendromatics-0.4.2/src/dendromatics/draw.py
--rw-r--r--   0        0        0    12754 2020-02-02 00:00:00.000000 dendromatics-0.4.2/src/dendromatics/ground.py
--rw-r--r--   0        0        0    19282 2020-02-02 00:00:00.000000 dendromatics-0.4.2/src/dendromatics/individualize.py
--rw-r--r--   0        0        0    42854 2020-02-02 00:00:00.000000 dendromatics-0.4.2/src/dendromatics/sections.py
--rw-r--r--   0        0        0     9211 2020-02-02 00:00:00.000000 dendromatics-0.4.2/src/dendromatics/stripe.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 dendromatics-0.4.2/src/dendromatics/voxel/__init__.py
--rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 dendromatics-0.4.2/src/dendromatics/voxel/voxel.py
--rw-r--r--   0        0        0     4253 2020-02-02 00:00:00.000000 dendromatics-0.4.2/tests/test_ground.py
--rw-r--r--   0        0        0     4428 2020-02-02 00:00:00.000000 dendromatics-0.4.2/tests/test_voxel.py
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 dendromatics-0.4.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 dendromatics-0.4.2/LICENSE
--rw-r--r--   0        0        0     6713 2020-02-02 00:00:00.000000 dendromatics-0.4.2/README.rst
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 dendromatics-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     8073 2020-02-02 00:00:00.000000 dendromatics-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/CHANGELOG.md
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/readthedocs.yaml
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/docs/Makefile
+-rw-r--r--   0        0        0     7188 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/docs/algorithm.rst
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/docs/cc_plugin.rst
+-rw-r--r--   0        0        0     3176 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/docs/conf.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/docs/dendromatics.rst
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/docs/examples.rst
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/docs/executable.rst
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/docs/index.rst
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/docs/installation.rst
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/docs/make.bat
+-rw-r--r--   0        0        0   252269 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/docs/_static/3dfin_logo.png
+-rw-r--r--   0        0        0   270012 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/docs/_static/dendromatics_logo.png
+-rw-r--r--   0        0        0   113056 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/docs/_static/height-normalization.jpg
+-rw-r--r--   0        0        0    45823 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/docs/_static/individualized_trees.jpg
+-rw-r--r--   0        0        0   109342 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/docs/_static/sections_and_axes.jpg
+-rw-r--r--   0        0        0   210688 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/docs/_static/stripe_and_groups.jpg
+-rw-r--r--   0        0        0    29602 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/docs/_static/tree_height.jpg
+-rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/examples/example.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/src/dendromatics/__about__.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/src/dendromatics/__init__.py
+-rw-r--r--   0        0        0    13668 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/src/dendromatics/draw.py
+-rw-r--r--   0        0        0    12754 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/src/dendromatics/ground.py
+-rw-r--r--   0        0        0    19282 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/src/dendromatics/individualize.py
+-rw-r--r--   0        0        0    42854 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/src/dendromatics/sections.py
+-rw-r--r--   0        0        0     9271 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/src/dendromatics/stripe.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/src/dendromatics/voxel/__init__.py
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/src/dendromatics/voxel/voxel.py
+-rw-r--r--   0        0        0     4253 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/tests/test_ground.py
+-rw-r--r--   0        0        0     4428 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/tests/test_voxel.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/LICENSE
+-rw-r--r--   0        0        0     6713 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/README.rst
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/pyproject.toml
+-rw-r--r--   0        0        0     8064 2020-02-02 00:00:00.000000 dendromatics-0.5.0a0/PKG-INFO
```

### Comparing `dendromatics-0.4.2/CHANGELOG.md` & `dendromatics-0.5.0a0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,21 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+### Changed
+
+- Replace `jakteristics` by `pgeof` for verticality computation. This should result in a slight 
+  but noticeable speed improvement.
+
+- Minimum python version is now 3.9.
+
 ## [0.4.2] - 2024-03-14
 
 ### Changed
 
 - Take advantage of multiple CPU cores during `DBSCAN` clustering.
 
 ### Fixed
```

### Comparing `dendromatics-0.4.2/readthedocs.yaml` & `dendromatics-0.5.0a0/readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `dendromatics-0.4.2/.github/workflows/build.yml` & `dendromatics-0.5.0a0/.github/workflows/build.yml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 jobs:
   build:
     name: Build dendromatics source package and wheel
     runs-on: ubuntu-latest
 
     steps:
       - name: Checkout
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Install Hatch
         run: python -m pip install --upgrade hatch
 
       - name: Build artifacts
```

### Comparing `dendromatics-0.4.2/.github/workflows/test.yml` & `dendromatics-0.5.0a0/.github/workflows/test.yml`

 * *Files 12% similar despite different names*

```diff
@@ -14,22 +14,25 @@
 jobs:
   run:
     name: Python ${{ matrix.python-version }} on ${{ startsWith(matrix.os, 'macos-') && 'macOS' || startsWith(matrix.os, 'windows-') && 'Windows' || 'Linux' }}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false # the full workflow does not fail if one build fail in order to get full report
       matrix:
-        os: [ubuntu-latest, windows-latest] # we need to modify jakteristics to renable macOS.
-        python-version: ["3.8","3.9", "3.10", "3.11", "3.12"]
+        os: [ubuntu-latest, windows-latest, macos-latest]
+        python-version: ["3.9", "3.10", "3.11", "3.12"]
+        exclude:
+          - os: macos-latest
+            python-version: "3.9"
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Get latest hatch version
         run: python -m pip install --upgrade hatch
 
       - name: Run static and style checks
```

### Comparing `dendromatics-0.4.2/docs/Makefile` & `dendromatics-0.5.0a0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dendromatics-0.4.2/docs/algorithm.rst` & `dendromatics-0.5.0a0/docs/algorithm.rst`

 * *Files identical despite different names*

### Comparing `dendromatics-0.4.2/docs/conf.py` & `dendromatics-0.5.0a0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dendromatics-0.4.2/docs/dendromatics.rst` & `dendromatics-0.5.0a0/docs/dendromatics.rst`

 * *Files identical despite different names*

### Comparing `dendromatics-0.4.2/docs/examples.rst` & `dendromatics-0.5.0a0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `dendromatics-0.4.2/docs/executable.rst` & `dendromatics-0.5.0a0/docs/executable.rst`

 * *Files identical despite different names*

### Comparing `dendromatics-0.4.2/docs/index.rst` & `dendromatics-0.5.0a0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dendromatics-0.4.2/docs/make.bat` & `dendromatics-0.5.0a0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dendromatics-0.4.2/docs/_static/3dfin_logo.png` & `dendromatics-0.5.0a0/docs/_static/3dfin_logo.png`

 * *Files identical despite different names*

### Comparing `dendromatics-0.4.2/docs/_static/dendromatics_logo.png` & `dendromatics-0.5.0a0/docs/_static/dendromatics_logo.png`

 * *Files identical despite different names*

### Comparing `dendromatics-0.4.2/docs/_static/height-normalization.jpg` & `dendromatics-0.5.0a0/docs/_static/height-normalization.jpg`

 * *Files identical despite different names*

### Comparing `dendromatics-0.4.2/docs/_static/individualized_trees.jpg` & `dendromatics-0.5.0a0/docs/_static/individualized_trees.jpg`

 * *Files identical despite different names*

### Comparing `dendromatics-0.4.2/docs/_static/sections_and_axes.jpg` & `dendromatics-0.5.0a0/docs/_static/sections_and_axes.jpg`

 * *Files identical despite different names*

### Comparing `dendromatics-0.4.2/docs/_static/stripe_and_groups.jpg` & `dendromatics-0.5.0a0/docs/_static/stripe_and_groups.jpg`

 * *Files identical despite different names*

### Comparing `dendromatics-0.4.2/docs/_static/tree_height.jpg` & `dendromatics-0.5.0a0/docs/_static/tree_height.jpg`

 * *Files identical despite different names*

### Comparing `dendromatics-0.4.2/examples/example.py` & `dendromatics-0.5.0a0/examples/example.py`

 * *Files identical despite different names*

### Comparing `dendromatics-0.4.2/src/dendromatics/draw.py` & `dendromatics-0.5.0a0/src/dendromatics/draw.py`

 * *Files identical despite different names*

### Comparing `dendromatics-0.4.2/src/dendromatics/ground.py` & `dendromatics-0.5.0a0/src/dendromatics/ground.py`

 * *Files identical despite different names*

### Comparing `dendromatics-0.4.2/src/dendromatics/individualize.py` & `dendromatics-0.5.0a0/src/dendromatics/individualize.py`

 * *Files identical despite different names*

### Comparing `dendromatics-0.4.2/src/dendromatics/sections.py` & `dendromatics-0.5.0a0/src/dendromatics/sections.py`

 * *Files identical despite different names*

### Comparing `dendromatics-0.4.2/src/dendromatics/stripe.py` & `dendromatics-0.5.0a0/src/dendromatics/stripe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import timeit
 
-import jakteristics as jak
 import numpy as np
+import pgeof
+from pgeof import EFeatureID
 from sklearn.cluster import DBSCAN
 
 from .voxel.voxel import *
 
 # -----------------------------------------------------------------------------
 # verticality_clustering_iteration
 # -----------------------------------------------------------------------------
@@ -32,15 +33,15 @@
     Parameters
     ----------
     stripe : numpy.ndarray
         The point cloud containing the stripe. It is expected to have X, Y, Z0
         fields. 3D or higher array containing data with `float` type.
     vert_scale : float
         Scale to be used during verticality computation to define a
-        neighbourhood arounda given point. Verticality will be computed from
+        neighbourhood around a given point. Verticality will be computed from
         the structure tensor of said neighbourhood via eigendecomposition.
     vert_threshold : float
         Minimum verticality value associated to a point to consider it as part
         of a stem.
     n_points : int
         Minimum number of points in a cluster for it to be considered as a
         potential stem.
@@ -69,16 +70,17 @@
     # Call to 'voxelate' function to voxelate the cloud.
     voxelated_stripe, vox_to_stripe_ind, _ = voxelate(
         stripe, resolution_xy, resolution_z, n_digits, with_n_points=False
     )
     # Computation of verticality values associated to voxels using
     # 'compute_features' function. It needs a vicinity radius, provided by
     # 'vert_scale'.
-    vert_values = jak.compute_features(
-        voxelated_stripe, search_radius=vert_scale, feature_names=["verticality"]
+    # use a large max_knn like jakteristics
+    vert_values = pgeof.compute_features_selected(
+        voxelated_stripe, vert_scale, 50000, [EFeatureID.Verticality]
     )
 
     elapsed = timeit.default_timer() - t
     print("   %.2f" % elapsed, "s")
     t1 = elapsed
 
     # Verticality values are appended to the ORIGINAL cloud, using voxel-to-
@@ -186,15 +188,15 @@
     Parameters
     ----------
     stripe : numpy.ndarray
         The point cloud containing the stripe. It is expected to have X, Y, Z0
         fields. 3D or higher array containing data with `float` type.
     scale : float
         Scale to be used during verticality computation to define a
-        neighbourhood arounda given point. Verticality will be computed from
+        neighbourhood around a given point. Verticality will be computed from
         the structure tensor of said neighbourhood via eigendecomposition.
         Defaults to 0.1.
     vert_threshold : float
         Minimum verticality value associated to a point to consider it as part
         of a stem. Defaults to 0.7.
     n_points : int
         Minimum number of points in a cluster for it to be considered as a
```

### Comparing `dendromatics-0.4.2/src/dendromatics/voxel/voxel.py` & `dendromatics-0.5.0a0/src/dendromatics/voxel/voxel.py`

 * *Files identical despite different names*

### Comparing `dendromatics-0.4.2/tests/test_ground.py` & `dendromatics-0.5.0a0/tests/test_ground.py`

 * *Files identical despite different names*

### Comparing `dendromatics-0.4.2/tests/test_voxel.py` & `dendromatics-0.5.0a0/tests/test_voxel.py`

 * *Files identical despite different names*

### Comparing `dendromatics-0.4.2/.gitignore` & `dendromatics-0.5.0a0/.gitignore`

 * *Files identical despite different names*

### Comparing `dendromatics-0.4.2/LICENSE` & `dendromatics-0.5.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `dendromatics-0.4.2/README.rst` & `dendromatics-0.5.0a0/README.rst`

 * *Files identical despite different names*

### Comparing `dendromatics-0.4.2/pyproject.toml` & `dendromatics-0.5.0a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "dendromatics"
 dynamic = ["version"]
 description = "Automatic dendrometry and forest inventory for terrestrial point clouds"
 readme = "README.rst"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = "GPL-3.0-or-later"
 authors = [
     { name = "Carlos Cabo", email = "carloscabo@uniovi.es" },
     { name = "Diego Laino", email = "diegolainor@gmail.com" },
 ]
 keywords = [
     "forestry",
@@ -27,16 +27,16 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
     "csf_3dfin==1.3.0",
-    "jakteristics~=0.6.0",
-    "laspy~=2.5.3",
+    "pgeof~=0.2",
+    "laspy~=2.5",
     "numpy~=1.24",
     "scikit_learn~=1.2",
     "scipy~=1.10",
 ]
 
 [project.optional-dependencies]
 docs = [
@@ -60,15 +60,15 @@
   "pytest-randomly",
 ]
 [tool.hatch.envs.default.scripts]
 cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=src/dendromatics --cov=tests --randomly-seed=1 {args}"
 no-cov = "cov --no-cov {args}"
 
 [[tool.hatch.envs.test.matrix]]
-python = ["38","39", "310", "311", "312"]
+python = ["39", "310", "311", "312"]
 
 [tool.coverage.run]
 branch = true
 parallel = true
 omit = [
     "src/dendromatics/__about__.py",
 ]
```

### Comparing `dendromatics-0.4.2/PKG-INFO` & `dendromatics-0.5.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: dendromatics
-Version: 0.4.2
+Version: 0.5.0a0
 Summary: Automatic dendrometry and forest inventory for terrestrial point clouds
 Project-URL: Source, https://github.com/3DFin/dendromatics
 Project-URL: Documentation, https://dendromatics.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/3DFin/dendromatics/issues
 Author-email: Carlos Cabo <carloscabo@uniovi.es>, Diego Laino <diegolainor@gmail.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
@@ -14,19 +14,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: GIS
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Requires-Dist: csf-3dfin==1.3.0
-Requires-Dist: jakteristics~=0.6.0
-Requires-Dist: laspy~=2.5.3
+Requires-Dist: laspy~=2.5
 Requires-Dist: numpy~=1.24
+Requires-Dist: pgeof~=0.2
 Requires-Dist: scikit-learn~=1.2
 Requires-Dist: scipy~=1.10
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == 'docs'
 Requires-Dist: sphinx-reference-rename; extra == 'docs'
 Requires-Dist: sphinx-rtd-theme; extra == 'docs'
 Description-Content-Type: text/x-rst
```

