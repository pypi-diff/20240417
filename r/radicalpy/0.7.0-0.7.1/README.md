# Comparing `tmp/radicalpy-0.7.0.tar.gz` & `tmp/radicalpy-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radicalpy-0.7.0.tar", last modified: Sun Apr 14 12:45:24 2024, max compression
+gzip compressed data, was "radicalpy-0.7.1.tar", last modified: Wed Apr 17 06:43:57 2024, max compression
```

## Comparing `radicalpy-0.7.0.tar` & `radicalpy-0.7.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:45:24.296968 radicalpy-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-14 12:45:19.000000 radicalpy-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-14 12:45:24.296968 radicalpy-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-14 12:45:19.000000 radicalpy-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-14 12:45:19.000000 radicalpy-0.7.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:45:24.296968 radicalpy-0.7.0/radicalpy/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8052 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/classical.py
--rw-r--r--   0 runner    (1001) docker     (127)    20549 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:45:24.296968 radicalpy-0.7.0/radicalpy/data_files/
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/data_files/constants.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:45:24.296968 radicalpy-0.7.0/radicalpy/data_files/molecules/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/data_files/molecules/2_6_aqds.json
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/data_files/molecules/adenine_cation.json
--rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/data_files/molecules/fad.json
--rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/data_files/molecules/flavin_anion.json
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/data_files/molecules/flavin_neutral.json
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/data_files/molecules/tryptophan_cation.json
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/data_files/molecules/tyrosine_neutral.json
--rw-r--r--   0 runner    (1001) docker     (127)    27847 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/data_files/spin_data.json
--rw-r--r--   0 runner    (1001) docker     (127)    23002 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/estimations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/experiments.py
--rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/kinetics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9475 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9707 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/relaxation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)    41184 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:45:24.296968 radicalpy-0.7.0/radicalpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-14 12:45:24.000000 radicalpy-0.7.0/radicalpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-14 12:45:24.000000 radicalpy-0.7.0/radicalpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 12:45:24.000000 radicalpy-0.7.0/radicalpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-14 12:45:24.000000 radicalpy-0.7.0/radicalpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-14 12:45:24.000000 radicalpy-0.7.0/radicalpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-14 12:45:19.000000 radicalpy-0.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 12:45:24.296968 radicalpy-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:45:24.296968 radicalpy-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-14 12:45:19.000000 radicalpy-0.7.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-14 12:45:19.000000 radicalpy-0.7.0/tests/test_estimations.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-14 12:45:19.000000 radicalpy-0.7.0/tests/test_relaxations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-14 12:45:19.000000 radicalpy-0.7.0/tests/test_shared.py
--rw-r--r--   0 runner    (1001) docker     (127)    21203 2024-04-14 12:45:19.000000 radicalpy-0.7.0/tests/test_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:43:57.801317 radicalpy-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-17 06:43:54.000000 radicalpy-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-17 06:43:57.801317 radicalpy-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-17 06:43:54.000000 radicalpy-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-17 06:43:54.000000 radicalpy-0.7.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:43:57.797317 radicalpy-0.7.1/radicalpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-17 06:43:54.000000 radicalpy-0.7.1/radicalpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8052 2024-04-17 06:43:54.000000 radicalpy-0.7.1/radicalpy/classical.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20559 2024-04-17 06:43:54.000000 radicalpy-0.7.1/radicalpy/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:43:57.797317 radicalpy-0.7.1/radicalpy/data_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-17 06:43:54.000000 radicalpy-0.7.1/radicalpy/data_files/constants.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:43:57.801317 radicalpy-0.7.1/radicalpy/data_files/molecules/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-17 06:43:54.000000 radicalpy-0.7.1/radicalpy/data_files/molecules/2_6_aqds.json
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-17 06:43:54.000000 radicalpy-0.7.1/radicalpy/data_files/molecules/adenine_cation.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-04-17 06:43:54.000000 radicalpy-0.7.1/radicalpy/data_files/molecules/fad.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-04-17 06:43:54.000000 radicalpy-0.7.1/radicalpy/data_files/molecules/flavin_anion.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-17 06:43:54.000000 radicalpy-0.7.1/radicalpy/data_files/molecules/flavin_neutral.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-17 06:43:54.000000 radicalpy-0.7.1/radicalpy/data_files/molecules/tryptophan_cation.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-17 06:43:54.000000 radicalpy-0.7.1/radicalpy/data_files/molecules/tyrosine_neutral.json
+-rw-r--r--   0 runner    (1001) docker     (127)    27847 2024-04-17 06:43:54.000000 radicalpy-0.7.1/radicalpy/data_files/spin_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23002 2024-04-17 06:43:54.000000 radicalpy-0.7.1/radicalpy/estimations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10980 2024-04-17 06:43:54.000000 radicalpy-0.7.1/radicalpy/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-04-17 06:43:54.000000 radicalpy-0.7.1/radicalpy/kinetics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-04-17 06:43:54.000000 radicalpy-0.7.1/radicalpy/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:43:54.000000 radicalpy-0.7.1/radicalpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9707 2024-04-17 06:43:54.000000 radicalpy-0.7.1/radicalpy/relaxation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-17 06:43:54.000000 radicalpy-0.7.1/radicalpy/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36064 2024-04-17 06:43:54.000000 radicalpy-0.7.1/radicalpy/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-04-17 06:43:54.000000 radicalpy-0.7.1/radicalpy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:43:57.801317 radicalpy-0.7.1/radicalpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-17 06:43:57.000000 radicalpy-0.7.1/radicalpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-17 06:43:57.000000 radicalpy-0.7.1/radicalpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:43:57.000000 radicalpy-0.7.1/radicalpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-17 06:43:57.000000 radicalpy-0.7.1/radicalpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-17 06:43:57.000000 radicalpy-0.7.1/radicalpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-17 06:43:54.000000 radicalpy-0.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 06:43:57.801317 radicalpy-0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:43:57.801317 radicalpy-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-17 06:43:54.000000 radicalpy-0.7.1/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-17 06:43:54.000000 radicalpy-0.7.1/tests/test_estimations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-17 06:43:54.000000 radicalpy-0.7.1/tests/test_relaxations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-17 06:43:54.000000 radicalpy-0.7.1/tests/test_shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21203 2024-04-17 06:43:54.000000 radicalpy-0.7.1/tests/test_simulation.py
```

### Comparing `radicalpy-0.7.0/LICENSE` & `radicalpy-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `radicalpy-0.7.0/PKG-INFO` & `radicalpy-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radicalpy
-Version: 0.7.0
+Version: 0.7.1
 Summary: RadicalPy: a toolbox for radical pair spin dynamics
 Author-email: "Lewis M. Antill" <lewismantill@gmail.com>, Emil Vatai <emil.vatai@gmail.com>
 Maintainer-email: Emil Vatai <emil.vatai@gmail.com>, "Lewis M. Antill" <lewismantill@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Spin-Chemistry-Labs/radicalpy
 Project-URL: Documentation, https://radicalpy.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/Spin-Chemistry-Labs/radicalpy
```

### Comparing `radicalpy-0.7.0/README.md` & `radicalpy-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `radicalpy-0.7.0/pyproject.toml` & `radicalpy-0.7.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 
 [tool.black]
 line-length = 88
 
 [tool.pylint]
 max-line-length = 88
 disable = ["C0103"]
+load-plugins='pylint.extensions.docparams'
 
 [tool.isort]
 line_length = 88
 profile = "black"
 
 [tool.mypy]
 plugins = ["numpy.typing.mypy_plugin"]
```

### Comparing `radicalpy-0.7.0/radicalpy/classical.py` & `radicalpy-0.7.1/radicalpy/classical.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.7.0/radicalpy/data.py` & `radicalpy-0.7.1/radicalpy/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,15 @@
     >>> Nucleus(0.001, 2, Hfc(3.0), "Adamantium")
     Adamantium(1.0, 2, 3.0 <anisotropic not available>)
     """
 
     magnetogyric_ratio: float
     multiplicity: int
     hfc: Hfc
-    name: str
+    name: Optional[str]
 
     def __repr__(self) -> str:  # noqa D105
         name = self.name if self.name else "Nucleus"
         return f"{name}({self.magnetogyric_ratio}, {self.multiplicity}, {self.hfc})"
 
     def __init__(
         self,
```

### Comparing `radicalpy-0.7.0/radicalpy/data_files/constants.json` & `radicalpy-0.7.1/radicalpy/data_files/constants.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.7.0/radicalpy/data_files/molecules/fad.json` & `radicalpy-0.7.1/radicalpy/data_files/molecules/fad.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.7.0/radicalpy/data_files/molecules/flavin_anion.json` & `radicalpy-0.7.1/radicalpy/data_files/molecules/flavin_anion.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.7.0/radicalpy/data_files/molecules/flavin_neutral.json` & `radicalpy-0.7.1/radicalpy/data_files/molecules/flavin_neutral.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.7.0/radicalpy/data_files/molecules/tryptophan_cation.json` & `radicalpy-0.7.1/radicalpy/data_files/molecules/tryptophan_cation.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.7.0/radicalpy/data_files/molecules/tyrosine_neutral.json` & `radicalpy-0.7.1/radicalpy/data_files/molecules/tyrosine_neutral.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.7.0/radicalpy/data_files/spin_data.json` & `radicalpy-0.7.1/radicalpy/data_files/spin_data.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.7.0/radicalpy/estimations.py` & `radicalpy-0.7.1/radicalpy/estimations.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.7.0/radicalpy/kinetics.py` & `radicalpy-0.7.1/radicalpy/kinetics.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.7.0/radicalpy/plot.py` & `radicalpy-0.7.1/radicalpy/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 def anisotropy_surface(theta, phi, Y):
     # TODO(vatai): clean up
     PH, TH = np.meshgrid(phi, theta)
     xyz = np.array([np.sin(TH) * np.cos(PH), np.sin(TH) * np.sin(PH), np.cos(TH)])
 
-    Yx, Yy, Yz = Y.real * spherical_to_cartesian(TH, PH)
+    Yx, Yy, Yz = Y.real * spherical_to_cartesian(TH, PH).T
 
     # Colour the plotted surface according to the sign of Y
     # cmap = plt.cm.ScalarMappable(cmap=plt.get_cmap("Accent_r"))
     cmap = plt.cm.ScalarMappable(cmap=plt.get_cmap("viridis"))
     cmap.set_clim(-0.01, 0.01)
 
     fig = plt.figure(figsize=plt.figaspect(1.0))
```

### Comparing `radicalpy-0.7.0/radicalpy/relaxation.py` & `radicalpy-0.7.1/radicalpy/relaxation.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.7.0/radicalpy/shared.py` & `radicalpy-0.7.1/radicalpy/shared.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.7.0/radicalpy/simulation.py` & `radicalpy-0.7.1/radicalpy/simulation.py`

 * *Files 6% similar despite different names*

```diff
@@ -229,15 +229,15 @@
 
         Args:
 
             idx1 (int): Index of the first particle.
 
             idx2 (int): Index of the second particle.
 
-            h (float): Isotopic interaction constant.
+            h (float): Isotropic interaction constant.
 
         Returns:
             np.ndarray:
 
                 Product operator for particles corresponding to `idx1`
                 and `idx2` with isotropic interaction constant `h`.
 
@@ -581,20 +581,23 @@
             np.ndarray:
 
                 The 3D Dipolar Hamiltonian corresponding to the system
                 described by the `HilbertSimulation` object and
                 dipolar interaction tensor `D`.
 
         """
-        ne = len(self.radicals)
-        return -sum(
+        spinops = [
+            [self.spin_operator(r, ax) for ax in "xyz"]
+            for r, _ in enumerate(self.radicals)
+        ]
+        return sum(
             (
-                -self.radicals[0].gamma_mT
-                * self.product_operator_3d(ei, ne + ni, dipolar_tensor)
-                for ni, ei in enumerate(self.coupling)
+                dipolar_tensor[i, j] * (si @ sj)
+                for i, si in enumerate(spinops[0])
+                for j, sj in enumerate(spinops[1])
             )
         )
 
     def zero_field_splitting_hamiltonian(self, D, E) -> np.ndarray:
         """Construct the Zero Field Splitting (ZFS) Hamiltonian."""
         Dmod = D * -self.radicals[0].gamma_mT
         Emod = E * -self.radicals[0].gamma_mT
@@ -651,16 +654,15 @@
         return self.convert(H)
 
     def time_evolution(
         self, init_state: State, time: np.ndarray, H: np.ndarray
     ) -> np.ndarray:
         """Evolve the system through time.
 
-        See also:
-
+        See Also:
         - `HilbertSimulation.unitary_propagator`
         - `HilbertSimulation.propagate`
         - `LiouvilleSimulation.unitary_propagator`
         - `LiouvilleSimulation.propagate`
 
         Args:
 
@@ -676,15 +678,14 @@
             np.ndarray:
 
                 Return a sequence of density matrices evolved through
                 `time`, starting from a given initial `state` using
                 the Hamiltonian `H`.
 
         Examples:
-
             >>> molecules = [Molecule.fromdb("flavin_anion", ["N5"]),
             ...              Molecule("Z")]
             >>> sim = HilbertSimulation(molecules)
             >>> H = sim.total_hamiltonian(B0=0, J=0, D=0)
             >>> time = np.arange(0, 2e-6, 5e-9)
             >>> time.shape
             (400,)
@@ -826,157 +827,14 @@
             product_yields=product_yields,
             product_yield_sums=product_yield_sums,
             MARY=MARY,
             LFE=LFE,
             HFE=HFE,
         )
 
-    def anisotropy_loop(
-        self,
-        init_state: State,
-        time: np.ndarray,
-        B0: float,
-        H_base: np.ndarray,
-        theta: np.ndarray,
-        phi: np.ndarray,
-    ) -> np.ndarray:
-        """Inner loop of anisotropy experiment.
-
-        Args:
-
-            init_state (State): Initial `State` of the density matrix.
-
-            time (np.ndarray): An sequence of (uniform) time points,
-                usually created using `np.arange` or `np.linspace`.
-
-            B0 (float): External magnetic field intensity (milli
-                Tesla) (see `zeeman_hamiltonian`).
-
-            H_base (np.ndarray): A "base" Hamiltonian, i.e., the
-                Zeeman Hamiltonian will be added to this base, usually
-                obtained with `total_hamiltonian` and `B0=0`.
-
-            theta (np.ndarray): rotation (polar) angle between the
-                external magnetic field and the fixed molecule. See
-                `zeeman_hamiltonian_3d`.
-
-            phi (np.ndarray): rotation (azimuth) angle between the
-                external magnetic field and the fixed molecule. See
-                `zeeman_hamiltonian_3d`.
-
-        Returns:
-            np.ndarray:
-
-            A tensor which has a series of density matrices for each
-            angle `theta` and `phi` obtained by running
-            `time_evolution` for each of them (with `time`
-            time\-steps, `B0` magnetic intensity).
-
-        """
-        shape = self._get_rho_shape(H_base.shape[0])
-        rhos = np.zeros((len(theta), len(phi), len(time), *shape), dtype=complex)
-
-        iters = itertools.product(enumerate(theta), enumerate(phi))
-        for (i, th), (j, ph) in tqdm(list(iters)):
-            H_zee = self.zeeman_hamiltonian(B0, th, ph)
-            H = H_base + self.convert(H_zee)
-            rhos[i, j] = self.time_evolution(init_state, time, H)
-        return rhos
-
-    def anisotropy(
-        self,
-        init_state: State,
-        obs_state: State,
-        time: np.ndarray,
-        theta: np.ndarray | float,
-        phi: np.ndarray | float,
-        B0: float,
-        D: np.ndarray,
-        J: float,
-        kinetics: list[HilbertIncoherentProcessBase] = [],
-        relaxations: list[HilbertIncoherentProcessBase] = [],
-    ) -> dict:
-        """Anisotropy experiment.
-
-        Args:
-
-            init_state (State): Initial `State` of the density matrix.
-
-            obs_state (State): Observable `State` of the density matrix.
-
-            time (np.ndarray): An sequence of (uniform) time points,
-                usually created using `np.arange` or `np.linspace`.
-
-            H_base (np.ndarray): A "base" Hamiltonian, i.e., the
-                Zeeman Hamiltonian will be added to this base, usually
-                obtained with `total_hamiltonian` and `B0=0`.
-
-            theta (np.ndarray): rotation (polar) angle between the
-                external magnetic field and the fixed molecule. See
-                `zeeman_hamiltonian_3d`.
-
-            B0 (float): External magnetic field intensity (milli
-                Tesla) (see `zeeman_hamiltonian`).
-
-            phi (np.ndarray): rotation (azimuth) angle between the
-                external magnetic field and the fixed molecule. See
-                `zeeman_hamiltonian_3d`.
-
-            D (np.ndarray): Dipolar coupling constant (see
-                `dipolar_hamiltonian`).
-
-            J (float): Exchange coupling constant (see
-                `exchange_hamiltonian`).
-
-            kinetics (list): A list of kinetic (super)operators of
-                type `radicalpy.kinetics.HilbertKineticsBase` or
-                `radicalpy.kinetics.LiouvilleKineticsBase`.
-
-            relaxations (list): A list of relaxation superoperators of
-                type `radicalpy.relaxation.LiouvilleRelaxationBase`.
-
-        Returns:
-            dict:
-
-            - time: the original `time` object
-            - B0: `B0` parameter
-            - theta: `theta` parameter
-            - phi: `phi` parameter
-            - rhos: tensor of sequences of time evolution of density
-              matrices
-            - time_evolutions: product probabilities
-            - product_yields: product yields
-            - product_yield_sums: product yield sums
-
-        """
-        H = self.total_hamiltonian(B0=0, D=D, J=J, hfc_anisotropy=True)
-
-        self.apply_liouville_hamiltonian_modifiers(H, kinetics + relaxations)
-        theta, phi = utils.anisotropy_check(theta, phi)
-        rhos = self.anisotropy_loop(init_state, time, B0, H, theta=theta, phi=phi)
-        product_probabilities = self.product_probability(obs_state, rhos)
-
-        self.apply_hilbert_kinetics(time, product_probabilities, kinetics)
-        k = kinetics[0].rate_constant if kinetics else 1.0
-        product_yields, product_yield_sums = self.product_yield(
-            product_probabilities, time, k
-        )
-        rhos = self._square_liouville_rhos(rhos)
-
-        return dict(
-            time=time,
-            B0=B0,
-            theta=theta,
-            phi=phi,
-            rhos=rhos,
-            time_evolutions=product_probabilities,
-            product_yields=product_yields,
-            product_yield_sums=product_yield_sums,
-        )
-
     @staticmethod
     def convert(H: np.ndarray) -> np.ndarray:
         return H
 
     @staticmethod
     def _convert(Q: np.ndarray) -> np.ndarray:
         return Q
```

### Comparing `radicalpy-0.7.0/radicalpy/utils.py` & `radicalpy-0.7.1/radicalpy/utils.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.7.0/radicalpy.egg-info/PKG-INFO` & `radicalpy-0.7.1/radicalpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radicalpy
-Version: 0.7.0
+Version: 0.7.1
 Summary: RadicalPy: a toolbox for radical pair spin dynamics
 Author-email: "Lewis M. Antill" <lewismantill@gmail.com>, Emil Vatai <emil.vatai@gmail.com>
 Maintainer-email: Emil Vatai <emil.vatai@gmail.com>, "Lewis M. Antill" <lewismantill@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Spin-Chemistry-Labs/radicalpy
 Project-URL: Documentation, https://radicalpy.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/Spin-Chemistry-Labs/radicalpy
```

### Comparing `radicalpy-0.7.0/radicalpy.egg-info/SOURCES.txt` & `radicalpy-0.7.1/radicalpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `radicalpy-0.7.0/tests/test_data.py` & `radicalpy-0.7.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.7.0/tests/test_estimations.py` & `radicalpy-0.7.1/tests/test_estimations.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.7.0/tests/test_shared.py` & `radicalpy-0.7.1/tests/test_shared.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.7.0/tests/test_simulation.py` & `radicalpy-0.7.1/tests/test_simulation.py`

 * *Files identical despite different names*

