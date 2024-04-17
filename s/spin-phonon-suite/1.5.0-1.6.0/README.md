# Comparing `tmp/spin_phonon_suite-1.5.0.tar.gz` & `tmp/spin_phonon_suite-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spin_phonon_suite-1.5.0.tar", last modified: Tue Dec 19 11:26:44 2023, max compression
+gzip compressed data, was "spin_phonon_suite-1.6.0.tar", last modified: Wed Apr 17 13:50:50 2024, max compression
```

## Comparing `spin_phonon_suite-1.5.0.tar` & `spin_phonon_suite-1.6.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-19 11:26:44.102488 spin_phonon_suite-1.5.0/
--rw-rw-rw-   0 root         (0) root         (0)    35085 2023-12-19 11:26:08.000000 spin_phonon_suite-1.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4105 2023-12-19 11:26:44.101488 spin_phonon_suite-1.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3031 2023-12-19 11:26:08.000000 spin_phonon_suite-1.5.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      215 2023-12-19 11:26:08.000000 spin_phonon_suite-1.5.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-12-19 11:26:44.102488 spin_phonon_suite-1.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1681 2023-12-19 11:26:41.000000 spin_phonon_suite-1.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-19 11:26:44.098488 spin_phonon_suite-1.5.0/spin_phonon_suite/
--rw-rw-rw-   0 root         (0) root         (0)      152 2023-12-19 11:26:08.000000 spin_phonon_suite-1.5.0/spin_phonon_suite/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      105 2023-12-19 11:26:41.000000 spin_phonon_suite-1.5.0/spin_phonon_suite/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)    23150 2023-12-19 11:26:08.000000 spin_phonon_suite-1.5.0/spin_phonon_suite/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1309 2023-12-19 11:26:08.000000 spin_phonon_suite-1.5.0/spin_phonon_suite/derivative.py
--rw-rw-rw-   0 root         (0) root         (0)    22652 2023-12-19 11:26:08.000000 spin_phonon_suite-1.5.0/spin_phonon_suite/lvc.py
--rw-rw-rw-   0 root         (0) root         (0)    19535 2023-12-19 11:26:08.000000 spin_phonon_suite-1.5.0/spin_phonon_suite/vibrations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-19 11:26:44.101488 spin_phonon_suite-1.5.0/spin_phonon_suite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4105 2023-12-19 11:26:44.000000 spin_phonon_suite-1.5.0/spin_phonon_suite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      466 2023-12-19 11:26:44.000000 spin_phonon_suite-1.5.0/spin_phonon_suite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-19 11:26:44.000000 spin_phonon_suite-1.5.0/spin_phonon_suite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-12-19 11:26:44.000000 spin_phonon_suite-1.5.0/spin_phonon_suite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      160 2023-12-19 11:26:44.000000 spin_phonon_suite-1.5.0/spin_phonon_suite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-12-19 11:26:44.000000 spin_phonon_suite-1.5.0/spin_phonon_suite.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 13:50:50.112896 spin_phonon_suite-1.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35085 2024-04-17 13:50:08.000000 spin_phonon_suite-1.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4105 2024-04-17 13:50:50.111895 spin_phonon_suite-1.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3031 2024-04-17 13:50:08.000000 spin_phonon_suite-1.6.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1151 2024-04-17 13:50:08.000000 spin_phonon_suite-1.6.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 13:50:50.112896 spin_phonon_suite-1.6.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2024-04-17 13:50:08.000000 spin_phonon_suite-1.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 13:50:50.109896 spin_phonon_suite-1.6.0/spin_phonon_suite/
+-rw-rw-rw-   0 root         (0) root         (0)      152 2024-04-17 13:50:08.000000 spin_phonon_suite-1.6.0/spin_phonon_suite/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      105 2024-04-17 13:50:08.000000 spin_phonon_suite-1.6.0/spin_phonon_suite/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23327 2024-04-17 13:50:08.000000 spin_phonon_suite-1.6.0/spin_phonon_suite/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1309 2024-04-17 13:50:08.000000 spin_phonon_suite-1.6.0/spin_phonon_suite/derivative.py
+-rw-rw-rw-   0 root         (0) root         (0)    23113 2024-04-17 13:50:08.000000 spin_phonon_suite-1.6.0/spin_phonon_suite/lvc.py
+-rw-rw-rw-   0 root         (0) root         (0)    20208 2024-04-17 13:50:08.000000 spin_phonon_suite-1.6.0/spin_phonon_suite/vibrations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 13:50:50.111895 spin_phonon_suite-1.6.0/spin_phonon_suite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4105 2024-04-17 13:50:50.000000 spin_phonon_suite-1.6.0/spin_phonon_suite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      466 2024-04-17 13:50:50.000000 spin_phonon_suite-1.6.0/spin_phonon_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 13:50:50.000000 spin_phonon_suite-1.6.0/spin_phonon_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2024-04-17 13:50:50.000000 spin_phonon_suite-1.6.0/spin_phonon_suite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      160 2024-04-17 13:50:50.000000 spin_phonon_suite-1.6.0/spin_phonon_suite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-17 13:50:50.000000 spin_phonon_suite-1.6.0/spin_phonon_suite.egg-info/top_level.txt
```

### Comparing `spin_phonon_suite-1.5.0/LICENSE` & `spin_phonon_suite-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-1.5.0/PKG-INFO` & `spin_phonon_suite-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spin_phonon_suite
-Version: 1.5.0
+Version: 1.6.0
 Summary: A package for performing spin-phonon coupling calculations with openMOLCAS, VASP, and Gaussian
 Home-page: https://gitlab.com/chilton-group/spin_phonon_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/spin_phonon_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/spin_phonon_suite
 Classifier: Programming Language :: Python :: 3
```

### Comparing `spin_phonon_suite-1.5.0/README.md` & `spin_phonon_suite-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-1.5.0/setup.py` & `spin_phonon_suite-1.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 # DO NOT EDIT THIS NUMBER!
 # IT IS AUTOMATICALLY CHANGED BY python-semantic-release
-__version__ = "1.5.0"
+__version__ = "1.6.0"
 
 setuptools.setup(
     name='spin_phonon_suite',
     version=__version__,
     author='Chilton Group',
     author_email='nicholas.chilton@manchester.ac.uk',
     description='A package for performing spin-phonon coupling calculations with openMOLCAS, VASP, and Gaussian', # noqa
```

### Comparing `spin_phonon_suite-1.5.0/spin_phonon_suite/cli.py` & `spin_phonon_suite-1.6.0/spin_phonon_suite/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,16 +154,18 @@
             args.phonopy_hdf5,
             trans=args.trans,
             cluster_expansion=args.cluster_expansion,
             cluster_cutoff=args.cluster_cutoff,
             central_idc=args.central_index
         )
 
-    if args.remove_imaginary:
+    if args.imaginary=='remove':
         ho = ho.remove_imaginary(verbose=True)
+    elif args.imaginary=='absolute':
+        ho = ho.abs_imaginary(verbose=True)
 
     if args.active_atoms is not None:
         ho = ho.subset_atoms(active_atom_idc=args.active_atoms)
 
     elif args.ref_coordinates is not None:
         _, coords = xyzp.load_xyz(args.ref_coordinates)
         ho = ho.subset_atoms(ref_coords=coords)
@@ -681,20 +683,22 @@
         '--rot',
         action=BooleanOptionalAction,
         default=True,
         help='Project out three rigid body rotations.'
     )
 
     vibrate.add_argument(
-        '--remove_imaginary',
-        action=BooleanOptionalAction,
-        default=True,
-        help='Remove modes with imaginary frequency.'
+        '--imaginary',
+        default='remove',
+        choices=['remove', 'keep', 'absolute'],
+        help=('Remove modes with imaginary frequencies (default), '
+             'keep without altering, or set to their absolute value.')
     )
 
+
     subset = vibrate.add_mutually_exclusive_group()
 
     subset.add_argument(
         '--active_atoms',
         nargs='+',
         type=parse_index,
         help=(
```

### Comparing `spin_phonon_suite-1.5.0/spin_phonon_suite/derivative.py` & `spin_phonon_suite-1.6.0/spin_phonon_suite/derivative.py`

 * *Files identical despite different names*

### Comparing `spin_phonon_suite-1.5.0/spin_phonon_suite/lvc.py` & `spin_phonon_suite-1.6.0/spin_phonon_suite/lvc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from fractions import Fraction
 from functools import lru_cache, partial
+import warnings
 
 import h5py
 
 import numpy as np
 from jax import jvp, jit
 from jax.lax import stop_gradient
 import jax.numpy as jnp
@@ -264,14 +265,22 @@
                      for mult, nroots in sf_mult.items()}
 
         for mult, (root1, root2), val in sf_linear_iter:
             couplings[mult][root1, root2, :] = val
             if root1 != root2:
                 couplings[mult][root2, root1, :] = val
 
+        # check if any expected couplings have not been supplied
+        for mult, nroots in sf_mult.items():
+            for root1 in range(nroots):
+                for root2 in range(root1, nroots):
+                    if not couplings[mult][root1, root2].any():
+                        warnings.warn("Missing couplings between roots "
+                                      f"{root1+1} and {root2+1} of spin state with multiplicity {mult}!")
+
         return cls(sf_ener, list(couplings.values()), sf_mult, geom,
                    sf_amfi=sf_amfi, sf_angm=sf_angm)
 
     def join(self, other, ref_geom):
 
         if not (sfy(np.array_equal, sf=1)(self.sf_mult, other.sf_mult) and
                 sfy(np.array_equal, sf=1)(self.sf_ener, other.sf_ener) and
```

### Comparing `spin_phonon_suite-1.5.0/spin_phonon_suite/vibrations.py` & `spin_phonon_suite-1.6.0/spin_phonon_suite/vibrations.py`

 * *Files 2% similar despite different names*

```diff
@@ -354,14 +354,28 @@
         idc = list(tuple(zip(*filter(is_real, enumerate(self.freqs))))[0])
 
         return Harmonic(self.freqs[idc], self.displacements[idc], coords=self.coords,
                         weights=None if self.weights is None else self.weights[idc],
                         band_indices=None if self.band_indices is None else self.band_indices[idc],
                         q_points=None if self.q_points is None else self.q_points[idc])
 
+    def abs_imaginary(self, verbose=False):
+        
+        if verbose: 
+            for idx, freq in enumerate(self.freqs):
+                if freq < 0: print(f"Setting imaginary mode: {idx+1} {freq: .2f} cm^-1 to {abs(freq): .2f} cm^-1")
+
+        self.freqs=abs(self.freqs)
+        idc=np.argsort(self.freqs)
+
+        return Harmonic(self.freqs[idc], self.displacements[idc], coords=self.coords,
+                        weights=None if self.weights is None else self.weights[idc],
+                        band_indices=None if self.band_indices is None else self.band_indices[idc],
+                        q_points=None if self.q_points is None else self.q_points[idc])
+
     def __add__(self, other):
 
         if not np.allclose(self.coords, other.coords):
             raise ValueError("Coordinates are incompatible!")
 
         order = np.argsort(np.concatenate((self.freqs, other.freqs)))
```

### Comparing `spin_phonon_suite-1.5.0/spin_phonon_suite.egg-info/PKG-INFO` & `spin_phonon_suite-1.6.0/spin_phonon_suite.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: spin-phonon-suite
-Version: 1.5.0
+Name: spin_phonon_suite
+Version: 1.6.0
 Summary: A package for performing spin-phonon coupling calculations with openMOLCAS, VASP, and Gaussian
 Home-page: https://gitlab.com/chilton-group/spin_phonon_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/spin_phonon_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/spin_phonon_suite
 Classifier: Programming Language :: Python :: 3
```

