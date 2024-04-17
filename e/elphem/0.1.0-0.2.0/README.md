# Comparing `tmp/elphem-0.1.0.tar.gz` & `tmp/elphem-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elphem-0.1.0.tar", last modified: Thu Oct 26 15:39:05 2023, max compression
+gzip compressed data, was "elphem-0.2.0.tar", last modified: Wed Apr 17 09:09:59 2024, max compression
```

## Comparing `elphem-0.1.0.tar` & `elphem-0.2.0.tar`

### file list

```diff
@@ -1,52 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 15:39:05.628712 elphem-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-10-26 15:38:53.000000 elphem-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7361 2023-10-26 15:39:05.628712 elphem-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6747 2023-10-26 15:38:53.000000 elphem-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 15:39:05.624712 elphem-0.1.0/elphem/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-10-26 15:38:53.000000 elphem-0.1.0/elphem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 15:39:05.624712 elphem-0.1.0/elphem/const/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-10-26 15:38:53.000000 elphem-0.1.0/elphem/const/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2023-10-26 15:38:53.000000 elphem-0.1.0/elphem/const/atomic_weight.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2023-10-26 15:38:53.000000 elphem-0.1.0/elphem/const/brillouin.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2425 2023-10-26 15:38:53.000000 elphem-0.1.0/elphem/const/unit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 15:39:05.624712 elphem-0.1.0/elphem/electron/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-10-26 15:38:53.000000 elphem-0.1.0/elphem/electron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2023-10-26 15:38:53.000000 elphem-0.1.0/elphem/electron/free.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 15:39:05.624712 elphem-0.1.0/elphem/elph/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-10-26 15:38:53.000000 elphem-0.1.0/elphem/elph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2023-10-26 15:38:53.000000 elphem-0.1.0/elphem/elph/distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     4692 2023-10-26 15:38:53.000000 elphem-0.1.0/elphem/elph/self_energy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 15:39:05.624712 elphem-0.1.0/elphem/lattice/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-10-26 15:38:53.000000 elphem-0.1.0/elphem/lattice/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4453 2023-10-26 15:38:53.000000 elphem-0.1.0/elphem/lattice/empty.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3070 2023-10-26 15:38:53.000000 elphem-0.1.0/elphem/lattice/rotation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 15:39:05.624712 elphem-0.1.0/elphem/phonon/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-26 15:38:53.000000 elphem-0.1.0/elphem/phonon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2023-10-26 15:38:53.000000 elphem-0.1.0/elphem/phonon/debye.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 15:39:05.624712 elphem-0.1.0/elphem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7361 2023-10-26 15:39:05.000000 elphem-0.1.0/elphem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2023-10-26 15:39:05.000000 elphem-0.1.0/elphem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-26 15:39:05.000000 elphem-0.1.0/elphem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-26 15:39:05.000000 elphem-0.1.0/elphem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-26 15:39:05.000000 elphem-0.1.0/elphem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-26 15:39:05.628712 elphem-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2023-10-26 15:38:53.000000 elphem-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 15:39:05.624712 elphem-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-26 15:38:53.000000 elphem-0.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 15:39:05.624712 elphem-0.1.0/tests/const/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-26 15:38:53.000000 elphem-0.1.0/tests/const/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2023-10-26 15:38:53.000000 elphem-0.1.0/tests/const/test_atomic_weight.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2023-10-26 15:38:53.000000 elphem-0.1.0/tests/const/test_brillouin.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2023-10-26 15:38:53.000000 elphem-0.1.0/tests/const/test_unit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 15:39:05.624712 elphem-0.1.0/tests/electron/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-26 15:38:53.000000 elphem-0.1.0/tests/electron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2023-10-26 15:38:53.000000 elphem-0.1.0/tests/electron/test_free.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 15:39:05.624712 elphem-0.1.0/tests/elph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-26 15:38:53.000000 elphem-0.1.0/tests/elph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2023-10-26 15:38:53.000000 elphem-0.1.0/tests/elph/test_self_energy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 15:39:05.624712 elphem-0.1.0/tests/lattice/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-26 15:38:53.000000 elphem-0.1.0/tests/lattice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2023-10-26 15:38:53.000000 elphem-0.1.0/tests/lattice/test_empty_lattice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 15:39:05.628712 elphem-0.1.0/tests/phonon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-26 15:38:53.000000 elphem-0.1.0/tests/phonon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2023-10-26 15:38:53.000000 elphem-0.1.0/tests/phonon/test_debye.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:59.025802 elphem-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-17 09:09:55.000000 elphem-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6902 2024-04-17 09:09:59.025802 elphem-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-04-17 09:09:55.000000 elphem-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:59.021802 elphem-0.2.0/elphem/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:59.021802 elphem-0.2.0/elphem/const/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/const/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/const/atomic_weight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/const/brillouin.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3006 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/const/unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:59.021802 elphem-0.2.0/elphem/electron/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/electron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/electron/free.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:59.021802 elphem-0.2.0/elphem/elph/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/elph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/elph/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/elph/epr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5802 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/elph/self_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/elph/spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:59.021802 elphem-0.2.0/elphem/lattice/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/lattice/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9629 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/lattice/empty.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4768 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/lattice/rotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:59.021802 elphem-0.2.0/elphem/phonon/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/phonon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-17 09:09:55.000000 elphem-0.2.0/elphem/phonon/debye.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:59.025802 elphem-0.2.0/elphem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6902 2024-04-17 09:09:59.000000 elphem-0.2.0/elphem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-17 09:09:59.000000 elphem-0.2.0/elphem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:09:59.000000 elphem-0.2.0/elphem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 09:09:59.000000 elphem-0.2.0/elphem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 09:09:59.000000 elphem-0.2.0/elphem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 09:09:59.025802 elphem-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-17 09:09:55.000000 elphem-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:59.021802 elphem-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:55.000000 elphem-0.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:59.025802 elphem-0.2.0/tests/const/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:55.000000 elphem-0.2.0/tests/const/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-17 09:09:55.000000 elphem-0.2.0/tests/const/test_atomic_weight.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-17 09:09:55.000000 elphem-0.2.0/tests/const/test_brillouin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-17 09:09:55.000000 elphem-0.2.0/tests/const/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:59.025802 elphem-0.2.0/tests/electron/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:55.000000 elphem-0.2.0/tests/electron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-17 09:09:55.000000 elphem-0.2.0/tests/electron/test_free.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:59.025802 elphem-0.2.0/tests/elph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:55.000000 elphem-0.2.0/tests/elph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-17 09:09:55.000000 elphem-0.2.0/tests/elph/test_epr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-17 09:09:55.000000 elphem-0.2.0/tests/elph/test_self_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-17 09:09:55.000000 elphem-0.2.0/tests/elph/test_spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:59.025802 elphem-0.2.0/tests/lattice/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:55.000000 elphem-0.2.0/tests/lattice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-17 09:09:55.000000 elphem-0.2.0/tests/lattice/test_empty_lattice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:59.025802 elphem-0.2.0/tests/phonon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:09:55.000000 elphem-0.2.0/tests/phonon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-17 09:09:55.000000 elphem-0.2.0/tests/phonon/test_debye.py
```

### Comparing `elphem-0.1.0/LICENSE` & `elphem-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elphem-0.1.0/PKG-INFO` & `elphem-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,267 +1,245 @@
 Metadata-Version: 2.1
 Name: elphem
-Version: 0.1.0
+Version: 0.2.0
 Summary: Elphem: Calculating electron-phonon interactions with the empty lattice.
 Home-page: https://github.com/cohsh/elphem
 Download-URL: https://github.com/cohsh/elphem
 Author: Kohei Ishii
 Author-email: 
 Maintainer: Kohei Ishii
 Maintainer-email: 
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 
 # Elphem
+[![Upload Python Package](https://github.com/cohsh/elphem/actions/workflows/python-publish.yml/badge.svg)](https://github.com/cohsh/elphem/actions/workflows/python-publish.yml)
 [![Python package](https://github.com/cohsh/elphem/actions/workflows/python-package.yml/badge.svg)](https://github.com/cohsh/elphem/actions/workflows/python-package.yml)
-![Python Version](https://img.shields.io/badge/Python-3.10%2C%203.11-blue?logo=python)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/elphem)
+![PyPI - Version](https://img.shields.io/pypi/v/elphem)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/elphem)
 ![GitHub](https://img.shields.io/github/license/cohsh/elphem)
 
-Python Library for Calculations of **El**ectron-**Ph**onon Interactions with **Em**pty Lattice
+**El**ectron-**Ph**onon Interactions with **Em**pty Lattice
 
-## Support
-- Python 3.10 and 3.11
+- PyPI: https://pypi.org/project/elphem
 
 ## Installation
+### From PyPI
+```shell
+pip install elphem
+```
+
+### From GitHub
 ```shell
 git clone git@github.com:cohsh/elphem.git
 cd elphem
-pip install .
+pip install -e .
 ```
 
 ## Features
 Currently, Elphem allows calculations of
 - (reciprocal) lattice vectors from lattice constants.
 - electronic structures with empty lattice approximation.
 - phonon dispersion relations with Debye model.
 - first-order electron-phonon couplings.
 - one-electron self-energies.
+- spectral functions.
 
 ## Examples
-### Calculation of the electronic band structure
-
-![band structure](images/band_structure.png)
+### Calculation of spectral functions (`examples/spectrum.py`)
+![spectrum](images/spectrum.png)
 
 ```python
+"""Example: bcc-Li"""
 import numpy as np
 import matplotlib.pyplot as plt
-
-from elphem import SpecialPoints, Energy, Length, LatticeConstant, EmptyLattice, FreeElectron
+from elphem import *
 
 def main():
-    # Example: Li (BCC)
     a = 2.98 * Length.ANGSTROM["->"]
-    alpha = 109.47
+    mass = AtomicWeight.table["Li"] * Mass.DALTON["->"]
 
-    lattice_constant = LatticeConstant(a,a,a,alpha,alpha,alpha)
-    lattice = EmptyLattice(lattice_constant)
+    debye_temperature = 344.0
+
+    lattice = EmptyLattice('bcc', a)
+    electron = FreeElectron(lattice, n_band=8, n_electron=1)
+    phonon = DebyeModel(lattice, debye_temperature, 1, mass)
+
+    temperature =  3 * debye_temperature
+    self_energy = SelfEnergy(lattice, electron, phonon, temperature, sigma=0.5, eta=0.1)
+
+    n_q = np.array([10]*3)
+    n_omega = 1000
+    range_omega = [-8 * Energy.EV["->"], 6 * Energy.EV["->"]]
     
-    n_cut = np.array([2] * 3)
-    electron = FreeElectron(lattice, 1)
-        
     k_names = ["G", "H", "N", "G", "P", "H"]
-    k_via = [SpecialPoints.BCC[name] for name in k_names]
-
-    x, eig, x_special = electron.get_band_structure(n_cut, *k_via)
+    n_split = 20
+    
+    x, y, spectrum, special_x = Spectrum(self_energy).calculate_with_path(k_names, n_split, n_q, n_omega, range_omega)
+    y_mesh, x_mesh = np.meshgrid(y, x)
 
-    fig, ax = plt.subplots()
-    for band in eig:
-        ax.plot(x, band * Energy.EV["<-"], color="tab:blue")
+    fig = plt.figure()
+    ax = fig.add_subplot(1, 1, 1)
+    
+    mappable = ax.pcolormesh(x_mesh, y_mesh * Energy.EV["<-"], spectrum / Energy.EV["<-"])
     
-    ax.vlines(x_special, ymin=-10, ymax=50, color="black", linewidth=0.3)
-    ax.set_xticks(x_special)
+    for x0 in special_x:
+        ax.axvline(x=x0, color="black", linewidth=0.3)
+    
+    ax.set_xticks(special_x)
     ax.set_xticklabels(k_names)
     ax.set_ylabel("Energy ($\mathrm{eV}$)")
-    ax.set_ylim([-10,50])
+    ax.set_title("Spectral function of bcc-Li")
+    
+    fig.colorbar(mappable, ax=ax)
 
-    fig.savefig("test_band_structure.png")
+    fig.savefig("example_spectrum.png")
 
 if __name__ == "__main__":
     main()
 ```
 
-### Calculation of the phonon dispersion
+### Calculation of the electron-phonon renormalization (EPR) (`examples/electron_phonon_renormalization.py`)
 
-![phonon dispersion](images/phonon_dispersion.png)
+![epr](images/epr.png)
 
 ```python
-import os
+"""Example: bcc-Li"""
+import numpy as np
 import matplotlib.pyplot as plt
-
-from elphem import LatticeConstant, EmptyLattice, DebyeModel, AtomicWeight, Energy, Mass, Length, SpecialPoints, Prefix
+from elphem import *
 
 def main():
-    # Example: \gamma-Fe (FCC)
-    a = 2.58 * Length.ANGSTROM["->"]
-    lattice_constant = LatticeConstant(a, a, a, 60, 60, 60)
-    lattice = EmptyLattice(lattice_constant)
-    
-    debye_temperature = 470.0
+    a = 2.98 * Length.ANGSTROM["->"]
+    mass = AtomicWeight.table["Li"] * Mass.DALTON["->"]
+    debye_temperature = 344.0
+    temperature = 3 * debye_temperature
+    n_band = 20
+
+    lattice = EmptyLattice('bcc', a)
+    electron = FreeElectron(lattice, n_band, 1)        
+    phonon = DebyeModel(lattice, temperature, 1, mass)
+
+    self_energy = SelfEnergy(lattice, electron, phonon, temperature, eta=0.05)
 
-    phonon = DebyeModel(lattice, debye_temperature, 1, AtomicWeight.table["Fe"] * Mass.DALTON["->"])
+    k_names = ["G", "H", "N", "G", "P", "H"]
 
-    q_names = ["G", "X", "G", "L"]
-    q_via = [SpecialPoints.FCC[name] for name in q_names]
+    n_split = 20
+    n_q = np.array([8]*3)
     
-    x, omega, x_special = phonon.get_dispersion(*q_via)
+    k, eig, epr, special_k = EPR(self_energy).calculate_with_path(k_names, n_split, n_q)
     
-    fig, ax = plt.subplots()
+    fig = plt.figure()
+    ax = fig.add_subplot(1, 1, 1)
 
-    ax.plot(x, omega * Energy.EV["<-"] / Prefix.MILLI, color="tab:blue")
+    for n in range(n_band):
+        if n == 0:
+            ax.plot(k, eig[n] * Energy.EV["<-"], color="tab:blue", label="w/o EPR")
+            ax.plot(k, (eig[n] + epr[n]) * Energy.EV["<-"], color="tab:orange", label="w/ EPR")
+        else:
+            ax.plot(k, eig[n] * Energy.EV["<-"], color="tab:blue")
+            ax.plot(k, (eig[n] + epr[n]) * Energy.EV["<-"], color="tab:orange")
     
-    for x0 in x_special:
-        ax.axvline(x=x0, color="black", linewidth=0.3)
+    for k0 in special_k:
+        ax.axvline(x=k0, color="black", linewidth=0.3)
     
-    ax.set_xticks(x_special)
-    ax.set_xticklabels(q_names)
-    ax.set_ylabel("Energy ($\mathrm{meV}$)")
+    ax.set_xticks(special_k)
+    ax.set_xticklabels(k_names)
+    ax.set_ylabel("Energy ($\mathrm{eV}$)")
+    ax.set_title("Example: Band structure of bcc-Li")
+    ax.set_ylim([-10,20])
+    ax.legend()
+
 
-    fig.savefig("test_phonon_dispersion.png")
+    fig.savefig("example_epr.png")
 
 if __name__ == "__main__":
     main()
 ```
 
-### Calculation of the electron-phonon renormalization (EPR)
+### Calculation of the electronic band structure (`examples/band_structure.py`)
 
-![epr](images/epr.png)
+![band structure](images/band_structure.png)
 
 ```python
-import numpy as np
+"""Example: bcc-Li"""
 import matplotlib.pyplot as plt
-
-from elphem import LatticeConstant, EmptyLattice, FreeElectron, DebyeModel, SelfEnergy2nd
-from elphem.const import Mass, Energy, Length, AtomicWeight, SpecialPoints
+from elphem import *
 
 def main():
-    # Example: Li (BCC)
     a = 2.98 * Length.ANGSTROM["->"]
-    alpha = 109.47
-    lattice_constant = LatticeConstant(a,a,a,alpha,alpha,alpha)
-    lattice = EmptyLattice(lattice_constant)
 
-    electron = FreeElectron(lattice, 1)
-    
-    mass = AtomicWeight.table["Li"] * Mass.DALTON["->"]
-    
-    debye_temperature = 344.0
-
-    phonon = DebyeModel(lattice, debye_temperature, 1, mass)
-
-    self_energy = SelfEnergy2nd(lattice, electron, phonon)
-
-    n_g = np.array([2]*3)
-    
-    g = lattice.grid(n_g).reshape(-1, 3)
-    
-    n_g_inter = np.array([1]*3)
-    n_q = np.array([10]*3)
+    lattice = EmptyLattice('bcc', a)
+    electron = FreeElectron(lattice, n_band=50, n_electron=1)
 
     k_names = ["G", "H", "N", "G", "P", "H"]
 
-    k_via = [SpecialPoints.BCC[name] for name in k_names]
-
-    x, k, special_x = lattice.reciprocal_cell.path(20, *k_via)
-    
-    selfen = np.empty((len(k)), dtype=complex)
-
-    fig = plt.figure()
-    ax = fig.add_subplot(1, 1, 1)
-
-    temperature = 2 * debye_temperature
+    k, eig, special_k = electron.get_band_structure(k_names, n_split=20)
 
-    for n in range(len(g)):
-        eig = electron.eigenenergy(k + g[n])
-        for i in range(len(k)):
-            selfen[i] = self_energy.calculate(temperature, g[n], k[i], n_g_inter, n_q)
-
-        epr = selfen.real
-
-        ax.plot(x, eig * Energy.EV["<-"], color="tab:blue")
-        ax.plot(x, (eig + epr) * Energy.EV["<-"], color="tab:orange")
-    
-    for x0 in special_x:
-        ax.axvline(x=x0, color="black", linewidth=0.3)
+    fig, ax = plt.subplots()
+    for band in eig:
+        ax.plot(k, band * Energy.EV["<-"], color="tab:blue")
     
-    ax.set_xticks(special_x)
+    ax.vlines(special_k, ymin=-10, ymax=50, color="black", linewidth=0.3)
+    ax.set_xticks(special_k)
     ax.set_xticklabels(k_names)
     ax.set_ylabel("Energy ($\mathrm{eV}$)")
-    ax.set_ylim([-7,Energy.EV["<-"]])
-    ax.set_title("Example: Band structure of bcc-Li")
+    ax.set_ylim([-10,50])
 
-    fig.savefig("test_epr.png")
+    fig.savefig("example_band_structure.png")
 
 if __name__ == "__main__":
     main()
 ```
 
-### Calculation of scattering rate
+### Calculation of the phonon dispersion (`examples/phonon_dispersion.py`)
 
-![scattering_rate](images/scattering_rate.png)
+![phonon dispersion](images/phonon_dispersion.png)
 
 ```python
-import numpy as np
+"""Example: bcc-Li"""
 import matplotlib.pyplot as plt
-
-from elphem import LatticeConstant, EmptyLattice, FreeElectron, DebyeModel, SelfEnergy2nd
-from elphem.const import Mass, Energy, Prefix, Time, Length, AtomicWeight
+from elphem import *
 
 def main():
-    # Example: Li (BCC)
     a = 2.98 * Length.ANGSTROM["->"]
-    alpha = 109.47
-    lattice_constant = LatticeConstant(a,a,a,alpha,alpha,alpha)
-    lattice = EmptyLattice(lattice_constant)
-
-    electron = FreeElectron(lattice, 1)
-    
     mass = AtomicWeight.table["Li"] * Mass.DALTON["->"]
-    
-    debye_temperature = 344.0
+    lattice = EmptyLattice('bcc', a)
 
+    debye_temperature = 344.0
     phonon = DebyeModel(lattice, debye_temperature, 1, mass)
 
-    temperature = debye_temperature
-
-    self_energy = SelfEnergy2nd(lattice, electron, phonon)
-
-    n_g = np.array([1]*3)
-    n_k = np.array([6]*3)
-    g, k = electron.grid(n_g, n_k)
+    q_names = ["G", "H", "N", "G", "P", "H"]
     
-    n_g_inter = np.array([1]*3)
-    n_q = np.array([10]*3)
-    selfen = self_energy.calculate(temperature, g, k, n_g_inter, n_q)
-
-    epsilon_nk = electron.eigenenergy(k + g)
-
-    fig = plt.figure()
-
-    ax1 = fig.add_subplot(2, 1, 1)
-    ax2 = fig.add_subplot(2, 1, 2)
-
-    for ax in [ax1, ax2]:
-        ax.scatter(epsilon_nk * Energy.EV["<-"], selfen.imag / (Time.SI["<-"] / Prefix.PICO), label="$\mathrm{Im}\Sigma^\mathrm{Fan}$")
-
-        ax.set_ylabel("Scattering rate ($\mathrm{ps}^{-1}$)")
-        ax.legend()
+    q, omega, special_q = phonon.get_dispersion(q_names, n_split=20)
+    
+    fig, ax = plt.subplots()
 
-    ax2.set_xlabel("Electron energy ($\mathrm{eV}$)")
-    ax2.set_yscale("log")
-    ax1.set_title("Example: Scattering rate of bcc-Li")
+    ax.plot(q, omega * Energy.EV["<-"] * 1.0e+3, color="tab:blue")
+    
+    for q0 in special_q:
+        ax.axvline(x=q0, color="black", linewidth=0.3)
     
-    file_name = "test_scattering_rate.png"
-    fig.savefig(file_name)
+    ax.set_xticks(special_q)
+    ax.set_xticklabels(q_names)
+    ax.set_ylabel("Energy ($\mathrm{meV}$)")
+
+    fig.savefig("example_phonon_dispersion.png")
 
 if __name__ == "__main__":
     main()
 ```
 
 ## License
 MIT
+
+## Author
+Kohei Ishii
```

### Comparing `elphem-0.1.0/README.md` & `elphem-0.2.0/elphem.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,247 +1,245 @@
+Metadata-Version: 2.1
+Name: elphem
+Version: 0.2.0
+Summary: Elphem: Calculating electron-phonon interactions with the empty lattice.
+Home-page: https://github.com/cohsh/elphem
+Download-URL: https://github.com/cohsh/elphem
+Author: Kohei Ishii
+Author-email: 
+Maintainer: Kohei Ishii
+Maintainer-email: 
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+
 # Elphem
+[![Upload Python Package](https://github.com/cohsh/elphem/actions/workflows/python-publish.yml/badge.svg)](https://github.com/cohsh/elphem/actions/workflows/python-publish.yml)
 [![Python package](https://github.com/cohsh/elphem/actions/workflows/python-package.yml/badge.svg)](https://github.com/cohsh/elphem/actions/workflows/python-package.yml)
-![Python Version](https://img.shields.io/badge/Python-3.10%2C%203.11-blue?logo=python)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/elphem)
+![PyPI - Version](https://img.shields.io/pypi/v/elphem)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/elphem)
 ![GitHub](https://img.shields.io/github/license/cohsh/elphem)
 
-Python Library for Calculations of **El**ectron-**Ph**onon Interactions with **Em**pty Lattice
+**El**ectron-**Ph**onon Interactions with **Em**pty Lattice
 
-## Support
-- Python 3.10 and 3.11
+- PyPI: https://pypi.org/project/elphem
 
 ## Installation
+### From PyPI
+```shell
+pip install elphem
+```
+
+### From GitHub
 ```shell
 git clone git@github.com:cohsh/elphem.git
 cd elphem
-pip install .
+pip install -e .
 ```
 
 ## Features
 Currently, Elphem allows calculations of
 - (reciprocal) lattice vectors from lattice constants.
 - electronic structures with empty lattice approximation.
 - phonon dispersion relations with Debye model.
 - first-order electron-phonon couplings.
 - one-electron self-energies.
+- spectral functions.
 
 ## Examples
-### Calculation of the electronic band structure
-
-![band structure](images/band_structure.png)
+### Calculation of spectral functions (`examples/spectrum.py`)
+![spectrum](images/spectrum.png)
 
 ```python
+"""Example: bcc-Li"""
 import numpy as np
 import matplotlib.pyplot as plt
-
-from elphem import SpecialPoints, Energy, Length, LatticeConstant, EmptyLattice, FreeElectron
+from elphem import *
 
 def main():
-    # Example: Li (BCC)
     a = 2.98 * Length.ANGSTROM["->"]
-    alpha = 109.47
+    mass = AtomicWeight.table["Li"] * Mass.DALTON["->"]
+
+    debye_temperature = 344.0
+
+    lattice = EmptyLattice('bcc', a)
+    electron = FreeElectron(lattice, n_band=8, n_electron=1)
+    phonon = DebyeModel(lattice, debye_temperature, 1, mass)
+
+    temperature =  3 * debye_temperature
+    self_energy = SelfEnergy(lattice, electron, phonon, temperature, sigma=0.5, eta=0.1)
 
-    lattice_constant = LatticeConstant(a,a,a,alpha,alpha,alpha)
-    lattice = EmptyLattice(lattice_constant)
+    n_q = np.array([10]*3)
+    n_omega = 1000
+    range_omega = [-8 * Energy.EV["->"], 6 * Energy.EV["->"]]
     
-    n_cut = np.array([2] * 3)
-    electron = FreeElectron(lattice, 1)
-        
     k_names = ["G", "H", "N", "G", "P", "H"]
-    k_via = [SpecialPoints.BCC[name] for name in k_names]
-
-    x, eig, x_special = electron.get_band_structure(n_cut, *k_via)
+    n_split = 20
+    
+    x, y, spectrum, special_x = Spectrum(self_energy).calculate_with_path(k_names, n_split, n_q, n_omega, range_omega)
+    y_mesh, x_mesh = np.meshgrid(y, x)
 
-    fig, ax = plt.subplots()
-    for band in eig:
-        ax.plot(x, band * Energy.EV["<-"], color="tab:blue")
+    fig = plt.figure()
+    ax = fig.add_subplot(1, 1, 1)
     
-    ax.vlines(x_special, ymin=-10, ymax=50, color="black", linewidth=0.3)
-    ax.set_xticks(x_special)
+    mappable = ax.pcolormesh(x_mesh, y_mesh * Energy.EV["<-"], spectrum / Energy.EV["<-"])
+    
+    for x0 in special_x:
+        ax.axvline(x=x0, color="black", linewidth=0.3)
+    
+    ax.set_xticks(special_x)
     ax.set_xticklabels(k_names)
     ax.set_ylabel("Energy ($\mathrm{eV}$)")
-    ax.set_ylim([-10,50])
+    ax.set_title("Spectral function of bcc-Li")
+    
+    fig.colorbar(mappable, ax=ax)
 
-    fig.savefig("test_band_structure.png")
+    fig.savefig("example_spectrum.png")
 
 if __name__ == "__main__":
     main()
 ```
 
-### Calculation of the phonon dispersion
+### Calculation of the electron-phonon renormalization (EPR) (`examples/electron_phonon_renormalization.py`)
 
-![phonon dispersion](images/phonon_dispersion.png)
+![epr](images/epr.png)
 
 ```python
-import os
+"""Example: bcc-Li"""
+import numpy as np
 import matplotlib.pyplot as plt
-
-from elphem import LatticeConstant, EmptyLattice, DebyeModel, AtomicWeight, Energy, Mass, Length, SpecialPoints, Prefix
+from elphem import *
 
 def main():
-    # Example: \gamma-Fe (FCC)
-    a = 2.58 * Length.ANGSTROM["->"]
-    lattice_constant = LatticeConstant(a, a, a, 60, 60, 60)
-    lattice = EmptyLattice(lattice_constant)
-    
-    debye_temperature = 470.0
+    a = 2.98 * Length.ANGSTROM["->"]
+    mass = AtomicWeight.table["Li"] * Mass.DALTON["->"]
+    debye_temperature = 344.0
+    temperature = 3 * debye_temperature
+    n_band = 20
+
+    lattice = EmptyLattice('bcc', a)
+    electron = FreeElectron(lattice, n_band, 1)        
+    phonon = DebyeModel(lattice, temperature, 1, mass)
 
-    phonon = DebyeModel(lattice, debye_temperature, 1, AtomicWeight.table["Fe"] * Mass.DALTON["->"])
+    self_energy = SelfEnergy(lattice, electron, phonon, temperature, eta=0.05)
 
-    q_names = ["G", "X", "G", "L"]
-    q_via = [SpecialPoints.FCC[name] for name in q_names]
+    k_names = ["G", "H", "N", "G", "P", "H"]
+
+    n_split = 20
+    n_q = np.array([8]*3)
     
-    x, omega, x_special = phonon.get_dispersion(*q_via)
+    k, eig, epr, special_k = EPR(self_energy).calculate_with_path(k_names, n_split, n_q)
     
-    fig, ax = plt.subplots()
+    fig = plt.figure()
+    ax = fig.add_subplot(1, 1, 1)
 
-    ax.plot(x, omega * Energy.EV["<-"] / Prefix.MILLI, color="tab:blue")
+    for n in range(n_band):
+        if n == 0:
+            ax.plot(k, eig[n] * Energy.EV["<-"], color="tab:blue", label="w/o EPR")
+            ax.plot(k, (eig[n] + epr[n]) * Energy.EV["<-"], color="tab:orange", label="w/ EPR")
+        else:
+            ax.plot(k, eig[n] * Energy.EV["<-"], color="tab:blue")
+            ax.plot(k, (eig[n] + epr[n]) * Energy.EV["<-"], color="tab:orange")
     
-    for x0 in x_special:
-        ax.axvline(x=x0, color="black", linewidth=0.3)
+    for k0 in special_k:
+        ax.axvline(x=k0, color="black", linewidth=0.3)
     
-    ax.set_xticks(x_special)
-    ax.set_xticklabels(q_names)
-    ax.set_ylabel("Energy ($\mathrm{meV}$)")
+    ax.set_xticks(special_k)
+    ax.set_xticklabels(k_names)
+    ax.set_ylabel("Energy ($\mathrm{eV}$)")
+    ax.set_title("Example: Band structure of bcc-Li")
+    ax.set_ylim([-10,20])
+    ax.legend()
+
 
-    fig.savefig("test_phonon_dispersion.png")
+    fig.savefig("example_epr.png")
 
 if __name__ == "__main__":
     main()
 ```
 
-### Calculation of the electron-phonon renormalization (EPR)
+### Calculation of the electronic band structure (`examples/band_structure.py`)
 
-![epr](images/epr.png)
+![band structure](images/band_structure.png)
 
 ```python
-import numpy as np
+"""Example: bcc-Li"""
 import matplotlib.pyplot as plt
-
-from elphem import LatticeConstant, EmptyLattice, FreeElectron, DebyeModel, SelfEnergy2nd
-from elphem.const import Mass, Energy, Length, AtomicWeight, SpecialPoints
+from elphem import *
 
 def main():
-    # Example: Li (BCC)
     a = 2.98 * Length.ANGSTROM["->"]
-    alpha = 109.47
-    lattice_constant = LatticeConstant(a,a,a,alpha,alpha,alpha)
-    lattice = EmptyLattice(lattice_constant)
 
-    electron = FreeElectron(lattice, 1)
-    
-    mass = AtomicWeight.table["Li"] * Mass.DALTON["->"]
-    
-    debye_temperature = 344.0
-
-    phonon = DebyeModel(lattice, debye_temperature, 1, mass)
-
-    self_energy = SelfEnergy2nd(lattice, electron, phonon)
-
-    n_g = np.array([2]*3)
-    
-    g = lattice.grid(n_g).reshape(-1, 3)
-    
-    n_g_inter = np.array([1]*3)
-    n_q = np.array([10]*3)
+    lattice = EmptyLattice('bcc', a)
+    electron = FreeElectron(lattice, n_band=50, n_electron=1)
 
     k_names = ["G", "H", "N", "G", "P", "H"]
 
-    k_via = [SpecialPoints.BCC[name] for name in k_names]
-
-    x, k, special_x = lattice.reciprocal_cell.path(20, *k_via)
-    
-    selfen = np.empty((len(k)), dtype=complex)
-
-    fig = plt.figure()
-    ax = fig.add_subplot(1, 1, 1)
-
-    temperature = 2 * debye_temperature
+    k, eig, special_k = electron.get_band_structure(k_names, n_split=20)
 
-    for n in range(len(g)):
-        eig = electron.eigenenergy(k + g[n])
-        for i in range(len(k)):
-            selfen[i] = self_energy.calculate(temperature, g[n], k[i], n_g_inter, n_q)
-
-        epr = selfen.real
-
-        ax.plot(x, eig * Energy.EV["<-"], color="tab:blue")
-        ax.plot(x, (eig + epr) * Energy.EV["<-"], color="tab:orange")
-    
-    for x0 in special_x:
-        ax.axvline(x=x0, color="black", linewidth=0.3)
+    fig, ax = plt.subplots()
+    for band in eig:
+        ax.plot(k, band * Energy.EV["<-"], color="tab:blue")
     
-    ax.set_xticks(special_x)
+    ax.vlines(special_k, ymin=-10, ymax=50, color="black", linewidth=0.3)
+    ax.set_xticks(special_k)
     ax.set_xticklabels(k_names)
     ax.set_ylabel("Energy ($\mathrm{eV}$)")
-    ax.set_ylim([-7,Energy.EV["<-"]])
-    ax.set_title("Example: Band structure of bcc-Li")
+    ax.set_ylim([-10,50])
 
-    fig.savefig("test_epr.png")
+    fig.savefig("example_band_structure.png")
 
 if __name__ == "__main__":
     main()
 ```
 
-### Calculation of scattering rate
+### Calculation of the phonon dispersion (`examples/phonon_dispersion.py`)
 
-![scattering_rate](images/scattering_rate.png)
+![phonon dispersion](images/phonon_dispersion.png)
 
 ```python
-import numpy as np
+"""Example: bcc-Li"""
 import matplotlib.pyplot as plt
-
-from elphem import LatticeConstant, EmptyLattice, FreeElectron, DebyeModel, SelfEnergy2nd
-from elphem.const import Mass, Energy, Prefix, Time, Length, AtomicWeight
+from elphem import *
 
 def main():
-    # Example: Li (BCC)
     a = 2.98 * Length.ANGSTROM["->"]
-    alpha = 109.47
-    lattice_constant = LatticeConstant(a,a,a,alpha,alpha,alpha)
-    lattice = EmptyLattice(lattice_constant)
-
-    electron = FreeElectron(lattice, 1)
-    
     mass = AtomicWeight.table["Li"] * Mass.DALTON["->"]
-    
-    debye_temperature = 344.0
+    lattice = EmptyLattice('bcc', a)
 
+    debye_temperature = 344.0
     phonon = DebyeModel(lattice, debye_temperature, 1, mass)
 
-    temperature = debye_temperature
-
-    self_energy = SelfEnergy2nd(lattice, electron, phonon)
-
-    n_g = np.array([1]*3)
-    n_k = np.array([6]*3)
-    g, k = electron.grid(n_g, n_k)
+    q_names = ["G", "H", "N", "G", "P", "H"]
     
-    n_g_inter = np.array([1]*3)
-    n_q = np.array([10]*3)
-    selfen = self_energy.calculate(temperature, g, k, n_g_inter, n_q)
-
-    epsilon_nk = electron.eigenenergy(k + g)
-
-    fig = plt.figure()
-
-    ax1 = fig.add_subplot(2, 1, 1)
-    ax2 = fig.add_subplot(2, 1, 2)
-
-    for ax in [ax1, ax2]:
-        ax.scatter(epsilon_nk * Energy.EV["<-"], selfen.imag / (Time.SI["<-"] / Prefix.PICO), label="$\mathrm{Im}\Sigma^\mathrm{Fan}$")
-
-        ax.set_ylabel("Scattering rate ($\mathrm{ps}^{-1}$)")
-        ax.legend()
+    q, omega, special_q = phonon.get_dispersion(q_names, n_split=20)
+    
+    fig, ax = plt.subplots()
 
-    ax2.set_xlabel("Electron energy ($\mathrm{eV}$)")
-    ax2.set_yscale("log")
-    ax1.set_title("Example: Scattering rate of bcc-Li")
+    ax.plot(q, omega * Energy.EV["<-"] * 1.0e+3, color="tab:blue")
+    
+    for q0 in special_q:
+        ax.axvline(x=q0, color="black", linewidth=0.3)
     
-    file_name = "test_scattering_rate.png"
-    fig.savefig(file_name)
+    ax.set_xticks(special_q)
+    ax.set_xticklabels(q_names)
+    ax.set_ylabel("Energy ($\mathrm{meV}$)")
+
+    fig.savefig("example_phonon_dispersion.png")
 
 if __name__ == "__main__":
     main()
 ```
 
 ## License
-MIT
+MIT
+
+## Author
+Kohei Ishii
```

### Comparing `elphem-0.1.0/elphem/const/atomic_weight.py` & `elphem-0.2.0/elphem/const/atomic_weight.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,14 @@
 class AtomicWeight:
+    """Provides a table of atomic weights and a method to retrieve the atomic masses based on a list of atomic symbols.
+
+    Attributes:
+        table (dict): Dictionary mapping atomic symbols to their average atomic masses.
+    """
+    
     table = {
     "H": 1.008,
     "He": 4.002602,
     "Li": 6.94,
     "Be": 9.0121831,
     "B": 10.81,
     "C": 12.011,
@@ -81,14 +87,30 @@
     "Au": 196.9665704,
     "Hg": 200.5923,
     "Tl": 204.38
     }
     
     @classmethod
     def get_from_list(cls, atomic_names: list) -> list:
+        """Returns a list of atomic masses corresponding to the given list of atomic symbols.
+
+        Args:
+            atomic_names (list of str): A list of atomic symbols.
+
+        Returns:
+            list of float: A list of atomic masses corresponding to the atomic symbols.
+
+        Raises:
+            TypeError: If the input is not a list or if the elements of the list are not strings.
+            ValueError: If one or more atomic symbols in the list are invalid.
+
+        Examples:
+            >>> AtomicWeight.get_from_list(['H', 'He', 'Li'])
+            [1.008, 4.002602, 6.94]
+        """
         if not isinstance(atomic_names, list):
             raise TypeError("Input must be a list of atomic symbols.")
             
         mass_list = []
         for name in atomic_names:
             if not isinstance(name, str):
                 raise TypeError("Each item in the list must be a string representing an atomic symbol.")
```

### Comparing `elphem-0.1.0/elphem/const/unit.py` & `elphem-0.2.0/elphem/const/unit.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,15 +27,25 @@
     GIGA = 2 ** 30
     TERA = 2 ** 40
     PETA = 2 ** 50
     EXA = 2 ** 60
 
     @staticmethod
     def get_str(size: int) -> str:
-        """ Returns a string representation of bytes in suitable unit. """
+        """Returns a human-readable string representation of digital information sizes, scaled to appropriate unit.
+
+        Args:
+            size (int): Size in bytes.
+
+        Returns:
+            str: Formatted string representing the size in appropriate unit (e.g., KB, MB).
+
+        Raises:
+            ValueError: If size is negative or too large to be represented.
+        """
         if size < 0:
             raise ValueError("Size should be a non-negative integer.")
         
         units = ("B", "KB", "MB", "GB", "TB", "PB", "EB", "ZB")
         i = math.floor(math.log(size, 1024)) if size > 0 else 0
         
         if i >= len(units):
@@ -44,15 +54,23 @@
         size = round(size / 1024 ** i, 2)
         return f"{size} {units[i]}"
 
 class AtomicUnits:
     """ Utility class for atomic unit conversions. """
     @staticmethod
     def convert(unit: float, value: float) -> dict:
-        """ Converts values based on given unit. """
+        """Converts a value to and from a base unit to facilitate comparisons and calculations.
+
+        Args:
+            unit (float): The unit to which the conversion is based.
+            value (float): The value to be converted.
+
+        Returns:
+            dict: A dictionary containing converted values.
+        """
         return {
             "->": value / unit,
             "<-": unit / value
         }
 
 class Length:
     """ Atomic units of length. """
```

### Comparing `elphem-0.1.0/elphem/elph/distribution.py` & `elphem-0.2.0/elphem/elph/distribution.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,78 +1,87 @@
 import sys
 import numpy as np
-import warnings
 
 from elphem.const.unit import Energy
 
 # Setting up system-related constants and warning filters
 float_min = sys.float_info.min
 float_max = sys.float_info.max
 
 def safe_divide(a: np.ndarray | float | int, b: np.ndarray | float | int, default=np.nan):
-    """Safely divide two numbers, arrays, or a combination thereof."""
+    """
+    Safely divides two numbers, arrays, or a combination thereof, with optional handling of division by zero.
+
+    Args:
+        a (np.ndarray | float | int): Numerator, can be a number or an array.
+        b (np.ndarray | float | int): Denominator, can be a number or an array.
+        default (float | int, optional): Value to use when division by zero occurs. Default is NaN.
+
+    Returns:
+        np.ndarray: Result of the division, with division by zero handled gracefully.
+    """
     a_array = np.full_like(b, a)
     with np.errstate(divide='ignore', invalid='ignore'):
         result = np.divide(a_array, b, out=np.full_like(b, default), where=b != 0)
     return result
 
 def boltzmann_distribution(temperature: float, energy: float | np.ndarray) -> float | np.ndarray:
     """
-    Calculates the occupation number of particles that follow the Boltzmann distribution.
+    Calculates the occupation number of particles following the Boltzmann distribution.
 
     Args:
-        temperature: Temperature in Kelvin
-        energy: Energy value(s) in Hartree atomic units
+        temperature (float): Temperature in Kelvin.
+        energy (float | np.ndarray): Energy value(s) in Hartree atomic units.
 
     Returns:
-        Occupation number based on the Boltzmann distribution
+        float | np.ndarray: Occupation number(s) based on the Boltzmann distribution.
     """
     kbt = max(temperature * Energy.KELVIN["->"], float_min)
     beta = safe_divide(1.0, kbt, default=float_max)
 
     ln = - beta * energy
     return np.exp(ln, out=np.zeros_like(energy), where=ln > -np.log(float_max))
 
 def fermi_distribution(temperature: float, energy: float | np.ndarray) -> float | np.ndarray:
     """
-    Calculates the occupation number of particles that follow the Fermi-Dirac distribution.
+    Calculates the occupation number of particles following the Fermi-Dirac distribution.
 
     Args:
-        temperature: Temperature in Kelvin.
-        energy: Energy value(s) in Hartree atomic units.
+        temperature (float): Temperature in Kelvin.
+        energy (float | np.ndarray): Energy value(s) in Hartree atomic units.
 
     Returns:
-        Occupation number(s) based on the Fermi-Dirac distribution.
+        float | np.ndarray: Occupation number(s) based on the Fermi-Dirac distribution.
     """
     boltzmann_factor = boltzmann_distribution(temperature, energy)
     inv_boltzmann_factor = safe_divide(1.0, boltzmann_factor)
     return safe_divide(1.0, inv_boltzmann_factor + 1.0)
 
 def bose_distribution(temperature: float, energy: float | np.ndarray) -> float | np.ndarray:
     """
-    Calculates the occupation number of particles that follow the Bose-Einstein distribution.
+    Calculates the occupation number of particles following the Bose-Einstein distribution.
 
     Args:
-        temperature: Temperature in Kelvin.
-        energy: Energy value(s) in Hartree atomic units.
+        temperature (float): Temperature in Kelvin.
+        energy (float | np.ndarray): Energy value(s) in Hartree atomic units.
 
     Returns:
-        Occupation number(s) based on the Bose-Einstein distribution.
+        float | np.ndarray: Occupation number(s) based on the Bose-Einstein distribution.
     """
     boltzmann_factor = boltzmann_distribution(temperature, energy)
     inv_boltzmann_factor = safe_divide(1.0, boltzmann_factor)
     return safe_divide(1.0, inv_boltzmann_factor - 1.0)
 
 def gaussian_distribution(sigma: float, energy: float | np.ndarray) -> float | np.ndarray:
     """
-    Calculates the occupation number of particles that follow the Gaussian distribution.
+    Calculates the probability density of particles following the Gaussian distribution.
 
     Args:
-        sigma: Standard deviation of the Gaussian distribution.
-        energy: Energy value(s) in Hartree atomic units.
+        sigma (float): Standard deviation of the Gaussian distribution.
+        energy (float | np.ndarray): Energy value(s) to evaluate the Gaussian function.
 
     Returns:
-        Occupation number(s) based on the Gaussian distribution.
+        float | np.ndarray: Probability density(s) based on the Gaussian distribution.
     """
     if sigma == 0:
         raise ValueError("Sigma must not be zero.")
     return np.exp(- energy ** 2 / (2.0 * sigma ** 2)) / (np.sqrt(2.0 * np.pi) * sigma)
```

### Comparing `elphem-0.1.0/elphem/elph/self_energy.py` & `elphem-0.2.0/elphem/elph/self_energy.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,111 +4,138 @@
 from elphem.lattice.empty import EmptyLattice
 from elphem.electron.free import FreeElectron
 from elphem.phonon.debye import DebyeModel
 from elphem.elph.distribution import fermi_distribution, bose_distribution, gaussian_distribution, safe_divide
 
 @dataclass
 class SelfEnergy:
+    """Calculate the self-energy components for electronic states in a lattice.
+
+    Attributes:
+        lattice (EmptyLattice): The crystal lattice being studied.
+        electron (FreeElectron): Free electron model for the lattice.
+        phonon (DebyeModel): Phonon model using Debye approximation.
+        temperature (float): Temperature of the system in Kelvin.
+        sigma (float): Smearing parameter for the Gaussian distribution, defaults to 0.01.
+        eta (float): Small positive constant to ensure numerical stability, defaults to 0.01.
+        effective_potential (float): Effective potential used in electron-phonon coupling calculation, defaults to 1.0 / 16.0.
+    """
     lattice: EmptyLattice
     electron: FreeElectron
     phonon: DebyeModel
+    temperature: float
     sigma: float = 0.01
-    effective_potential: float = 1 / 16
+    eta: float = 0.01
+    effective_potential: float = 1.0 / 16.0
+    
+    def coupling(self, g1: np.ndarray, g2: np.ndarray, q: np.ndarray) -> np.ndarray:
+        """Calculate the lowest-order electron-phonon coupling between states.
 
-@dataclass
-class SelfEnergy2nd(SelfEnergy):
-    def validate_inputs(self, temperature, g, k, n_g, n_q, eta):
-        if not isinstance(temperature, (int, float)) or temperature < 0:
-            raise ValueError("Temperature must be a not-negative number.")
-        if not isinstance(eta, (int, float)):
-            raise ValueError("eta must be a number.")
+        Args:
+            g1 (np.ndarray): Initial G-vector in reciprocal space.
+            g2 (np.ndarray): Final G-vector in reciprocal space.
+            q (np.ndarray): Phonon wave vector in reciprocal space.
 
-    def calculate(self, temperature: float, g: np.ndarray, k: np.ndarray,
-                    n_g: np.ndarray, n_q: np.ndarray, eta=0.01) -> np.ndarray:
+        Returns:
+            np.ndarray: The electron-phonon coupling strength for the given vectors.
         """
-        Calculate 2nd-order Fan self-energies.
-        
-        Args
-            temperature: A temperature in Kelvin.
-            g: A numpy array (meshgrid-type) representing G-vector
-            k: A numpy array (meshgrid-type) representing k-vector
-            n_g: A numpy array representing the dense of intermediate G-vectors
-            n_q: A numpy array representing the dense of intermediate q-vectors
-            eta: A value of the convergence factor. The default value is 0.01 Hartree.
-            
-        Return
-            A numpy array representing Fan self-energy.
-        """
-        self.validate_inputs(temperature, g, k, n_g, n_q, eta)
-        g_reshaped = g.reshape(-1, 3)
-        k_reshaped = k.reshape(-1, 3)
-        
-        value = np.array([self.calculate_fan(temperature, g_i, k_i, n_g, n_q, eta) for g_i, k_i in zip(g_reshaped, k_reshaped)])
+        q_norm = np.linalg.norm(q, axis=-1)
+        delta_g = g1 - g2
+        q_dot = np.sum(q * delta_g, axis=-1) 
+
+        mask = q_norm > 0
+        result = np.zeros_like(q_norm)
         
-        return value.reshape(k[..., 0].shape)
-    
-    def calculate_fan(self, temperature: float, g1: np.ndarray, k: np.ndarray, 
-                        n_g: np.ndarray, n_q: np.ndarray, eta=0.01) -> complex:
-        """
-        Calculate single values of Fan self-energy.
+        denominator = np.sqrt(2.0 * self.phonon.mass * self.phonon.speed) * q_norm ** 1.5
+        result[mask] = safe_divide(self.effective_potential * q_dot[mask], denominator[mask])
         
-        Args
-            temperature: A temperature in Kelvin.
-            g1: A numpy array representing G-vector
-            k: A numpy array representing k-vector
-            n_g: A numpy array representing the dense of intermediate G-vectors
-            n_q: A numpy array representing the dense of intermediate q-vectors
-            eta: A value of the convergence factor. The default value is 0.01 Hartree.
-            
-        Return
-            A complex value representing Fan self-energy.
-        """
-        g2, q = self.electron.grid(n_g, n_q) # Generate intermediate G, q grid.
+        return result
 
-        electron_energy_nk = self.electron.eigenenergy(k + g1)
-        electron_energy_mkq = self.electron.eigenenergy(k + g2 + q)
+    def calculate_fan_term(self, g: np.ndarray, k: np.ndarray, n_q: np.ndarray) -> complex:
+        """Calculate a single value of Fan self-energy for given wave vectors.
 
-        omega = self.phonon.eigenenergy(q)
-        bose = bose_distribution(temperature, omega)
-        fermi = fermi_distribution(temperature, electron_energy_mkq)
+        Args:
+            g (np.ndarray): G-vector in reciprocal space.
+            k (np.ndarray): k-vector of the electron state.
+            n_q (np.ndarray): Density of intermediate q-vectors for integration.
+
+        Returns:
+            complex: The Fan self-energy term as a complex number.
+        """        
+        g_inter, q = self.electron.grid(n_q) # Generate intermediate G, q grid.
 
-        g = self.coupling(g1, g2, k, q)
+        omega = self.phonon.eigenenergy(q)
         
-        delta_energy = electron_energy_nk - electron_energy_mkq
+        coeff = 2.0 * np.pi / np.prod(n_q)
+
+        epsilon = self.electron.eigenenergy(k + g)
+        epsilon_inter = self.electron.eigenenergy(k + g_inter + q)
+
+        fermi = fermi_distribution(self.temperature, epsilon_inter)
+        bose = bose_distribution(self.temperature, omega)
+
+        coupling = self.coupling(g, g_inter, q)
+    
+        delta_energy = epsilon - epsilon_inter
         # Real Part
-        green_part_real = ((1.0 - fermi + bose) / (delta_energy - omega + eta * 1.0j)
-                           + (fermi + bose) / (delta_energy + omega + eta * 1.0j))
+        green_part_real = (safe_divide(1.0 - fermi + bose, delta_energy - omega + self.eta * 1.0j)
+                            + safe_divide(fermi + bose, delta_energy + omega + self.eta * 1.0j)).real
 
         # Imaginary Part
         green_part_imag = ((1.0 - fermi + bose) * gaussian_distribution(self.sigma, delta_energy - omega)
-                           + (fermi + bose) * gaussian_distribution(self.sigma, delta_energy + omega))
+                        + (fermi + bose) * gaussian_distribution(self.sigma, delta_energy + omega))
 
-        selfen_real = np.nansum(np.abs(g) ** 2 * green_part_real).real
-        selfen_imag = np.nansum(np.abs(g) ** 2 * green_part_imag)
-        
-        coeff = 2.0 * np.pi / np.prod(n_q)
+        selfen = (np.nansum(np.abs(coupling) ** 2 * green_part_real) 
+                        + 1.0j * np.nansum(np.abs(coupling) ** 2 * green_part_imag))
         
-        return (selfen_real + 1.0j * selfen_imag) * coeff
-    
-    def coupling(self, g1: np.ndarray, g2: np.ndarray, k: np.ndarray, q: np.ndarray) -> np.ndarray:
+        return selfen * coeff
+
+    def calculate_coupling_strength(self, g: np.ndarray, k: np.ndarray, n_q: np.ndarray) -> float:
+        """Calculate the electron-phonon coupling strength for given wave vectors.
+
+        Args:
+            g (np.ndarray): G-vector in reciprocal space.
+            k (np.ndarray): k-vector of the electron state.
+            n_q (np.ndarray): Density of q-vectors for the integration.
+
+        Returns:
+            float: The calculated electron-phonon coupling strength.
         """
-        Calculate lowest-order electron-phonon couplings.
         
-        Args
-            g1, g2: A numpy array representing G-vector
-            k: A numpy array representing k-vector
-            q: A numpy array representing k-vector
-        
-        Return
-            A value of the elctron-phonon coupling.
-        """
-        q_norm = np.linalg.norm(q, axis=-1)
-        delta_g = g1 - g2
-        q_dot = np.sum(q * delta_g, axis=-1) 
+        g_inter, q = self.electron.grid(n_q) # Generate intermediate G, q grid.
 
-        mask = q_norm > 0
-        result = np.zeros_like(q_norm)
+        omega = self.phonon.eigenenergy(q)
+        bose = bose_distribution(self.temperature, omega)
         
-        denominator = np.sqrt(2.0 * self.phonon.mass * self.phonon.speed) * q_norm ** 1.5
-        result[mask] = safe_divide(self.effective_potential * q_dot[mask], denominator[mask])
+        coeff = 2.0 * np.pi / np.prod(n_q)
+
+        epsilon = self.electron.eigenenergy(k + g)
+        epsilon_inter = self.electron.eigenenergy(k + g_inter + q)
+
+        fermi = fermi_distribution(self.temperature, epsilon_inter)
+
+        coupling = self.coupling(g, g_inter, q)
+    
+        delta_energy = epsilon - epsilon_inter
+        # Real Part
+        partial_green_part_real = - (safe_divide(1.0 - fermi + bose, (delta_energy - omega + self.eta * 1.0j) ** 2)
+                                    + safe_divide(fermi + bose, (delta_energy + omega + self.eta * 1.0j) ** 2)).real
+
+        coupling_strength = - np.nansum(np.abs(coupling) ** 2 * partial_green_part_real)
         
-        return result
+        return coupling_strength * coeff
+    
+    def calculate_qp_strength(self, g: np.ndarray, k: np.ndarray, n_q: np.ndarray) -> float:
+        """Calculate the quasiparticle strength for given wave vectors.
+
+        Args:
+            g (np.ndarray): G-vector in reciprocal space.
+            k (np.ndarray): k-vector of the electron state.
+            n_q (np.ndarray): Density of q-vectors for the integration.
+
+        Returns:
+            float: The quasiparticle strength.
+        """
+        coupling_strength = self.calculate_coupling_strength(g, k, n_q)
+        qp_strength = safe_divide(1.0, 1.0 + coupling_strength)
+
+        return qp_strength
```

### Comparing `elphem-0.1.0/elphem.egg-info/PKG-INFO` & `elphem-0.2.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,267 +1,224 @@
-Metadata-Version: 2.1
-Name: elphem
-Version: 0.1.0
-Summary: Elphem: Calculating electron-phonon interactions with the empty lattice.
-Home-page: https://github.com/cohsh/elphem
-Download-URL: https://github.com/cohsh/elphem
-Author: Kohei Ishii
-Author-email: 
-Maintainer: Kohei Ishii
-Maintainer-email: 
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: scipy
-
 # Elphem
+[![Upload Python Package](https://github.com/cohsh/elphem/actions/workflows/python-publish.yml/badge.svg)](https://github.com/cohsh/elphem/actions/workflows/python-publish.yml)
 [![Python package](https://github.com/cohsh/elphem/actions/workflows/python-package.yml/badge.svg)](https://github.com/cohsh/elphem/actions/workflows/python-package.yml)
-![Python Version](https://img.shields.io/badge/Python-3.10%2C%203.11-blue?logo=python)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/elphem)
+![PyPI - Version](https://img.shields.io/pypi/v/elphem)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/elphem)
 ![GitHub](https://img.shields.io/github/license/cohsh/elphem)
 
-Python Library for Calculations of **El**ectron-**Ph**onon Interactions with **Em**pty Lattice
+**El**ectron-**Ph**onon Interactions with **Em**pty Lattice
 
-## Support
-- Python 3.10 and 3.11
+- PyPI: https://pypi.org/project/elphem
 
 ## Installation
+### From PyPI
+```shell
+pip install elphem
+```
+
+### From GitHub
 ```shell
 git clone git@github.com:cohsh/elphem.git
 cd elphem
-pip install .
+pip install -e .
 ```
 
 ## Features
 Currently, Elphem allows calculations of
 - (reciprocal) lattice vectors from lattice constants.
 - electronic structures with empty lattice approximation.
 - phonon dispersion relations with Debye model.
 - first-order electron-phonon couplings.
 - one-electron self-energies.
+- spectral functions.
 
 ## Examples
-### Calculation of the electronic band structure
-
-![band structure](images/band_structure.png)
+### Calculation of spectral functions (`examples/spectrum.py`)
+![spectrum](images/spectrum.png)
 
 ```python
+"""Example: bcc-Li"""
 import numpy as np
 import matplotlib.pyplot as plt
-
-from elphem import SpecialPoints, Energy, Length, LatticeConstant, EmptyLattice, FreeElectron
+from elphem import *
 
 def main():
-    # Example: Li (BCC)
     a = 2.98 * Length.ANGSTROM["->"]
-    alpha = 109.47
+    mass = AtomicWeight.table["Li"] * Mass.DALTON["->"]
+
+    debye_temperature = 344.0
+
+    lattice = EmptyLattice('bcc', a)
+    electron = FreeElectron(lattice, n_band=8, n_electron=1)
+    phonon = DebyeModel(lattice, debye_temperature, 1, mass)
+
+    temperature =  3 * debye_temperature
+    self_energy = SelfEnergy(lattice, electron, phonon, temperature, sigma=0.5, eta=0.1)
 
-    lattice_constant = LatticeConstant(a,a,a,alpha,alpha,alpha)
-    lattice = EmptyLattice(lattice_constant)
+    n_q = np.array([10]*3)
+    n_omega = 1000
+    range_omega = [-8 * Energy.EV["->"], 6 * Energy.EV["->"]]
     
-    n_cut = np.array([2] * 3)
-    electron = FreeElectron(lattice, 1)
-        
     k_names = ["G", "H", "N", "G", "P", "H"]
-    k_via = [SpecialPoints.BCC[name] for name in k_names]
-
-    x, eig, x_special = electron.get_band_structure(n_cut, *k_via)
+    n_split = 20
+    
+    x, y, spectrum, special_x = Spectrum(self_energy).calculate_with_path(k_names, n_split, n_q, n_omega, range_omega)
+    y_mesh, x_mesh = np.meshgrid(y, x)
 
-    fig, ax = plt.subplots()
-    for band in eig:
-        ax.plot(x, band * Energy.EV["<-"], color="tab:blue")
+    fig = plt.figure()
+    ax = fig.add_subplot(1, 1, 1)
     
-    ax.vlines(x_special, ymin=-10, ymax=50, color="black", linewidth=0.3)
-    ax.set_xticks(x_special)
+    mappable = ax.pcolormesh(x_mesh, y_mesh * Energy.EV["<-"], spectrum / Energy.EV["<-"])
+    
+    for x0 in special_x:
+        ax.axvline(x=x0, color="black", linewidth=0.3)
+    
+    ax.set_xticks(special_x)
     ax.set_xticklabels(k_names)
     ax.set_ylabel("Energy ($\mathrm{eV}$)")
-    ax.set_ylim([-10,50])
+    ax.set_title("Spectral function of bcc-Li")
+    
+    fig.colorbar(mappable, ax=ax)
 
-    fig.savefig("test_band_structure.png")
+    fig.savefig("example_spectrum.png")
 
 if __name__ == "__main__":
     main()
 ```
 
-### Calculation of the phonon dispersion
+### Calculation of the electron-phonon renormalization (EPR) (`examples/electron_phonon_renormalization.py`)
 
-![phonon dispersion](images/phonon_dispersion.png)
+![epr](images/epr.png)
 
 ```python
-import os
+"""Example: bcc-Li"""
+import numpy as np
 import matplotlib.pyplot as plt
-
-from elphem import LatticeConstant, EmptyLattice, DebyeModel, AtomicWeight, Energy, Mass, Length, SpecialPoints, Prefix
+from elphem import *
 
 def main():
-    # Example: \gamma-Fe (FCC)
-    a = 2.58 * Length.ANGSTROM["->"]
-    lattice_constant = LatticeConstant(a, a, a, 60, 60, 60)
-    lattice = EmptyLattice(lattice_constant)
-    
-    debye_temperature = 470.0
+    a = 2.98 * Length.ANGSTROM["->"]
+    mass = AtomicWeight.table["Li"] * Mass.DALTON["->"]
+    debye_temperature = 344.0
+    temperature = 3 * debye_temperature
+    n_band = 20
+
+    lattice = EmptyLattice('bcc', a)
+    electron = FreeElectron(lattice, n_band, 1)        
+    phonon = DebyeModel(lattice, temperature, 1, mass)
 
-    phonon = DebyeModel(lattice, debye_temperature, 1, AtomicWeight.table["Fe"] * Mass.DALTON["->"])
+    self_energy = SelfEnergy(lattice, electron, phonon, temperature, eta=0.05)
 
-    q_names = ["G", "X", "G", "L"]
-    q_via = [SpecialPoints.FCC[name] for name in q_names]
+    k_names = ["G", "H", "N", "G", "P", "H"]
+
+    n_split = 20
+    n_q = np.array([8]*3)
     
-    x, omega, x_special = phonon.get_dispersion(*q_via)
+    k, eig, epr, special_k = EPR(self_energy).calculate_with_path(k_names, n_split, n_q)
     
-    fig, ax = plt.subplots()
+    fig = plt.figure()
+    ax = fig.add_subplot(1, 1, 1)
 
-    ax.plot(x, omega * Energy.EV["<-"] / Prefix.MILLI, color="tab:blue")
+    for n in range(n_band):
+        if n == 0:
+            ax.plot(k, eig[n] * Energy.EV["<-"], color="tab:blue", label="w/o EPR")
+            ax.plot(k, (eig[n] + epr[n]) * Energy.EV["<-"], color="tab:orange", label="w/ EPR")
+        else:
+            ax.plot(k, eig[n] * Energy.EV["<-"], color="tab:blue")
+            ax.plot(k, (eig[n] + epr[n]) * Energy.EV["<-"], color="tab:orange")
     
-    for x0 in x_special:
-        ax.axvline(x=x0, color="black", linewidth=0.3)
+    for k0 in special_k:
+        ax.axvline(x=k0, color="black", linewidth=0.3)
     
-    ax.set_xticks(x_special)
-    ax.set_xticklabels(q_names)
-    ax.set_ylabel("Energy ($\mathrm{meV}$)")
+    ax.set_xticks(special_k)
+    ax.set_xticklabels(k_names)
+    ax.set_ylabel("Energy ($\mathrm{eV}$)")
+    ax.set_title("Example: Band structure of bcc-Li")
+    ax.set_ylim([-10,20])
+    ax.legend()
+
 
-    fig.savefig("test_phonon_dispersion.png")
+    fig.savefig("example_epr.png")
 
 if __name__ == "__main__":
     main()
 ```
 
-### Calculation of the electron-phonon renormalization (EPR)
+### Calculation of the electronic band structure (`examples/band_structure.py`)
 
-![epr](images/epr.png)
+![band structure](images/band_structure.png)
 
 ```python
-import numpy as np
+"""Example: bcc-Li"""
 import matplotlib.pyplot as plt
-
-from elphem import LatticeConstant, EmptyLattice, FreeElectron, DebyeModel, SelfEnergy2nd
-from elphem.const import Mass, Energy, Length, AtomicWeight, SpecialPoints
+from elphem import *
 
 def main():
-    # Example: Li (BCC)
     a = 2.98 * Length.ANGSTROM["->"]
-    alpha = 109.47
-    lattice_constant = LatticeConstant(a,a,a,alpha,alpha,alpha)
-    lattice = EmptyLattice(lattice_constant)
 
-    electron = FreeElectron(lattice, 1)
-    
-    mass = AtomicWeight.table["Li"] * Mass.DALTON["->"]
-    
-    debye_temperature = 344.0
-
-    phonon = DebyeModel(lattice, debye_temperature, 1, mass)
-
-    self_energy = SelfEnergy2nd(lattice, electron, phonon)
-
-    n_g = np.array([2]*3)
-    
-    g = lattice.grid(n_g).reshape(-1, 3)
-    
-    n_g_inter = np.array([1]*3)
-    n_q = np.array([10]*3)
+    lattice = EmptyLattice('bcc', a)
+    electron = FreeElectron(lattice, n_band=50, n_electron=1)
 
     k_names = ["G", "H", "N", "G", "P", "H"]
 
-    k_via = [SpecialPoints.BCC[name] for name in k_names]
-
-    x, k, special_x = lattice.reciprocal_cell.path(20, *k_via)
-    
-    selfen = np.empty((len(k)), dtype=complex)
-
-    fig = plt.figure()
-    ax = fig.add_subplot(1, 1, 1)
-
-    temperature = 2 * debye_temperature
+    k, eig, special_k = electron.get_band_structure(k_names, n_split=20)
 
-    for n in range(len(g)):
-        eig = electron.eigenenergy(k + g[n])
-        for i in range(len(k)):
-            selfen[i] = self_energy.calculate(temperature, g[n], k[i], n_g_inter, n_q)
-
-        epr = selfen.real
-
-        ax.plot(x, eig * Energy.EV["<-"], color="tab:blue")
-        ax.plot(x, (eig + epr) * Energy.EV["<-"], color="tab:orange")
-    
-    for x0 in special_x:
-        ax.axvline(x=x0, color="black", linewidth=0.3)
+    fig, ax = plt.subplots()
+    for band in eig:
+        ax.plot(k, band * Energy.EV["<-"], color="tab:blue")
     
-    ax.set_xticks(special_x)
+    ax.vlines(special_k, ymin=-10, ymax=50, color="black", linewidth=0.3)
+    ax.set_xticks(special_k)
     ax.set_xticklabels(k_names)
     ax.set_ylabel("Energy ($\mathrm{eV}$)")
-    ax.set_ylim([-7,Energy.EV["<-"]])
-    ax.set_title("Example: Band structure of bcc-Li")
+    ax.set_ylim([-10,50])
 
-    fig.savefig("test_epr.png")
+    fig.savefig("example_band_structure.png")
 
 if __name__ == "__main__":
     main()
 ```
 
-### Calculation of scattering rate
+### Calculation of the phonon dispersion (`examples/phonon_dispersion.py`)
 
-![scattering_rate](images/scattering_rate.png)
+![phonon dispersion](images/phonon_dispersion.png)
 
 ```python
-import numpy as np
+"""Example: bcc-Li"""
 import matplotlib.pyplot as plt
-
-from elphem import LatticeConstant, EmptyLattice, FreeElectron, DebyeModel, SelfEnergy2nd
-from elphem.const import Mass, Energy, Prefix, Time, Length, AtomicWeight
+from elphem import *
 
 def main():
-    # Example: Li (BCC)
     a = 2.98 * Length.ANGSTROM["->"]
-    alpha = 109.47
-    lattice_constant = LatticeConstant(a,a,a,alpha,alpha,alpha)
-    lattice = EmptyLattice(lattice_constant)
-
-    electron = FreeElectron(lattice, 1)
-    
     mass = AtomicWeight.table["Li"] * Mass.DALTON["->"]
-    
-    debye_temperature = 344.0
+    lattice = EmptyLattice('bcc', a)
 
+    debye_temperature = 344.0
     phonon = DebyeModel(lattice, debye_temperature, 1, mass)
 
-    temperature = debye_temperature
-
-    self_energy = SelfEnergy2nd(lattice, electron, phonon)
-
-    n_g = np.array([1]*3)
-    n_k = np.array([6]*3)
-    g, k = electron.grid(n_g, n_k)
+    q_names = ["G", "H", "N", "G", "P", "H"]
     
-    n_g_inter = np.array([1]*3)
-    n_q = np.array([10]*3)
-    selfen = self_energy.calculate(temperature, g, k, n_g_inter, n_q)
-
-    epsilon_nk = electron.eigenenergy(k + g)
-
-    fig = plt.figure()
-
-    ax1 = fig.add_subplot(2, 1, 1)
-    ax2 = fig.add_subplot(2, 1, 2)
-
-    for ax in [ax1, ax2]:
-        ax.scatter(epsilon_nk * Energy.EV["<-"], selfen.imag / (Time.SI["<-"] / Prefix.PICO), label="$\mathrm{Im}\Sigma^\mathrm{Fan}$")
-
-        ax.set_ylabel("Scattering rate ($\mathrm{ps}^{-1}$)")
-        ax.legend()
+    q, omega, special_q = phonon.get_dispersion(q_names, n_split=20)
+    
+    fig, ax = plt.subplots()
 
-    ax2.set_xlabel("Electron energy ($\mathrm{eV}$)")
-    ax2.set_yscale("log")
-    ax1.set_title("Example: Scattering rate of bcc-Li")
+    ax.plot(q, omega * Energy.EV["<-"] * 1.0e+3, color="tab:blue")
+    
+    for q0 in special_q:
+        ax.axvline(x=q0, color="black", linewidth=0.3)
     
-    file_name = "test_scattering_rate.png"
-    fig.savefig(file_name)
+    ax.set_xticks(special_q)
+    ax.set_xticklabels(q_names)
+    ax.set_ylabel("Energy ($\mathrm{meV}$)")
+
+    fig.savefig("example_phonon_dispersion.png")
 
 if __name__ == "__main__":
     main()
 ```
 
 ## License
 MIT
+
+## Author
+Kohei Ishii
```

### Comparing `elphem-0.1.0/elphem.egg-info/SOURCES.txt` & `elphem-0.2.0/elphem.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -11,26 +11,30 @@
 elphem/const/atomic_weight.py
 elphem/const/brillouin.py
 elphem/const/unit.py
 elphem/electron/__init__.py
 elphem/electron/free.py
 elphem/elph/__init__.py
 elphem/elph/distribution.py
+elphem/elph/epr.py
 elphem/elph/self_energy.py
+elphem/elph/spectrum.py
 elphem/lattice/__init__.py
 elphem/lattice/empty.py
 elphem/lattice/rotation.py
 elphem/phonon/__init__.py
 elphem/phonon/debye.py
 tests/__init__.py
 tests/const/__init__.py
 tests/const/test_atomic_weight.py
 tests/const/test_brillouin.py
 tests/const/test_unit.py
 tests/electron/__init__.py
 tests/electron/test_free.py
 tests/elph/__init__.py
+tests/elph/test_epr.py
 tests/elph/test_self_energy.py
+tests/elph/test_spectrum.py
 tests/lattice/__init__.py
 tests/lattice/test_empty_lattice.py
 tests/phonon/__init__.py
 tests/phonon/test_debye.py
```

### Comparing `elphem-0.1.0/setup.py` & `elphem-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 DESCRIPTION = 'Elphem: Calculating electron-phonon interactions with the empty lattice.'
 NAME = 'elphem'
 AUTHOR = 'Kohei Ishii'
 AUTHOR_EMAIL = ''
 URL = 'https://github.com/cohsh/elphem'
 LICENSE = 'MIT'
 DOWNLOAD_URL = URL
-VERSION = '0.1.0'
+VERSION = '0.2.0'
 PYTHON_REQUIRES = '>=3.10'
 INSTALL_REQUIRES = ['numpy', 'scipy']
 
 CLASSIFIERS=[
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3.10',
-    'Programming Language :: Python :: 3.11'
+    'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12'
 ]
 
 try:
     with open('README.md', 'r', encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
 except FileExistsError:
     LONG_DESCRIPTION = DESCRIPTION
```

### Comparing `elphem-0.1.0/tests/const/test_unit.py` & `elphem-0.2.0/tests/const/test_unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from unittest import TestCase
-
 from elphem.const.unit import *
 
 class TestUnit(TestCase):
     def test_byte(self):
         size = Byte.get_str(2**30)
         self.assertEqual(size, "1.0 GB")
```

### Comparing `elphem-0.1.0/tests/electron/test_free.py` & `elphem-0.2.0/tests/electron/test_free.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 from unittest import TestCase
-import numpy as np
-
-from elphem.const.brillouin import SpecialPoints
-from elphem.lattice.empty import LatticeConstant, EmptyLattice
+from elphem.lattice.empty import EmptyLattice
 from elphem.electron.free import FreeElectron
 
 class TestUnit(TestCase):
-    def test_band_structure(self):
-        lattice_constant = LatticeConstant(5,5,5,60,60,60)
-        lattice = EmptyLattice(lattice_constant)
-        n_cut = np.array([2]*3)
-        electron = FreeElectron(lattice, 4)
-            
-        k_names = ["L", "G", "X"]
-        k_via = []
+    def setUp(self) -> None:
+        lattice = EmptyLattice('fcc', 5.0)
+        n_band = 20
+        n_electron = 4
+        self.electron = FreeElectron(lattice, n_band, n_electron)
 
-        for name in k_names:
-            k_via.append(SpecialPoints.FCC[name])
+    def test_band_structure(self):
+        k_names = ["L", "G", "X"]        
+        x, eig, x_special = self.electron.get_band_structure(k_names, n_split=20)
         
-        x, eig, x_special = electron.get_band_structure(n_cut, *k_via)
+        self.assertEqual(eig.shape, (self.electron.n_band, len(x)))
+        self.assertEqual(len(k_names), len(x_special))
+    
+    def test_get_reciprocal_vector(self):
+        g = self.electron.get_reciprocal_vector()
         
-        n_band = np.prod(n_cut) * 8
-        self.assertEqual(len(eig), n_band)
-        self.assertEqual(len(eig[0]), len(x))
-        self.assertEqual(len(k_names), len(x_special))
+        self.assertEqual(g.shape, (self.electron.n_band,3))
```

### Comparing `elphem-0.1.0/tests/elph/test_self_energy.py` & `elphem-0.2.0/tests/elph/test_spectrum.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,48 @@
 import numpy as np
 from unittest import TestCase
 
-from elphem.const.unit import Mass
-from elphem.lattice.empty import EmptyLattice, LatticeConstant
+from elphem.const.unit import Mass, Length
+from elphem.const.atomic_weight import AtomicWeight
+from elphem.lattice.empty import EmptyLattice
 from elphem.electron.free import FreeElectron
 from elphem.phonon.debye import DebyeModel
-from elphem.elph.self_energy import SelfEnergy2nd
+from elphem.elph.self_energy import SelfEnergy
+from elphem.elph.spectrum import Spectrum
 
 class TestUnit(TestCase):
-    def test_calculate(self):
-        lattice_constant = LatticeConstant(5,5,5,60,60,60)
-        lattice = EmptyLattice(lattice_constant)
-
-        electron = FreeElectron(lattice, 4)
-        
-        mass = 12 * Mass.DALTON["->"]
+    def setUp(self) -> None:
+        a = 2.98 * Length.ANGSTROM["->"]
+        mass = AtomicWeight.table["Li"] * Mass.DALTON["->"]
+        debye_temperature = 344.0
+        n_band = 8
+
+        temperature = 0.3 * debye_temperature
+
+        lattice = EmptyLattice('bcc', a)
+        electron = FreeElectron(lattice, n_band, 1)
+        phonon = DebyeModel(lattice, temperature, 1, mass)
+
+        self_energy = SelfEnergy(lattice, electron, phonon, temperature)
+        self.spectrum = Spectrum(self_energy)
+
+    def test_calculate_with_grid(self):
+        n_k = np.full(3, 5)        
+        n_q = np.full(3, 5)
+        n_omega = 100
         
-        debye_temperature = 2300.0
-
-        phonon = DebyeModel(lattice, debye_temperature, 2, mass)
+        a = self.spectrum.calculate_with_grid(n_k, n_q, n_omega)
 
-        temperature = debye_temperature
-
-        self_energy = SelfEnergy2nd(lattice, electron, phonon)
-
-        n_g = np.array([1]*3)
-        n_k = np.array([5]*3)
-        g, k = electron.grid(n_g, n_k)
+        self.assertEqual(a.shape, (np.prod(n_k), n_omega))
+    
+    def test_calculate_with_path(self):
+        k_names = ["G", "H", "N", "G", "P", "H"]
+        n_split = 20
         
-        n_g_inter = np.array([1]*3)
         n_q = np.array([5]*3)
-        selfen = self_energy.calculate(temperature, g, k, n_g_inter, n_q)
+        n_omega = 200
+        range_omega = [-1.0, 2.0]
+        
+        k, omegas, a, special_k = self.spectrum.calculate_with_path(k_names, n_split, n_q, n_omega, range_omega)
         
-        self.assertEqual(selfen.shape, (n_g[0]*2, n_g[1]*2, n_g[2]*2) + (n_k[0], n_k[1], n_k[2]))
+        self.assertEqual(a.shape, (len(k), len(omegas)))
+        self.assertEqual(len(k_names), len(special_k))
```

### Comparing `elphem-0.1.0/tests/phonon/test_debye.py` & `elphem-0.2.0/tests/elph/test_epr.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,45 @@
-from unittest import TestCase
 import numpy as np
+from unittest import TestCase
 
-from elphem.const.unit import Mass
-from elphem.const.brillouin import SpecialPoints
+from elphem.const.unit import Mass, Length
 from elphem.const.atomic_weight import AtomicWeight
-from elphem.lattice.empty import EmptyLattice, LatticeConstant
+from elphem.lattice.empty import EmptyLattice
+from elphem.electron.free import FreeElectron
 from elphem.phonon.debye import DebyeModel
+from elphem.elph.self_energy import SelfEnergy
+from elphem.elph.epr import EPR
 
 class TestUnit(TestCase):
-    def test_debye(self):
-        # Example: FCC-Fe
-        lattice_constant = LatticeConstant(2.58, 2.58, 2.58, 60, 60, 60)
-        lattice = EmptyLattice(lattice_constant)
-
-        phonon = DebyeModel(lattice, 470.0, 1, AtomicWeight.table["Fe"] * Mass.DALTON["->"])
+    def setUp(self) -> None:
+        a = 2.98 * Length.ANGSTROM["->"]
+        mass = AtomicWeight.table["Li"] * Mass.DALTON["->"]
+        debye_temperature = 344.0
+        n_band = 8
+
+        temperature = 0.3 * debye_temperature
+
+        lattice = EmptyLattice('bcc', a)
+        electron = FreeElectron(lattice, n_band, 1)
+        phonon = DebyeModel(lattice, temperature, 1, mass)
+
+        self_energy = SelfEnergy(lattice, electron, phonon, temperature)
+        self.epr = EPR(self_energy)
+
+    def test_calculate_with_grid(self):
+        n_k = np.full(3, 5)        
+        n_q = np.full(3, 5)
         
-        nq = np.array([8]*3)
-        q = phonon.grid(nq)
-        omega = phonon.eigenenergy(q)
-        
-        self.assertEqual(omega.shape, (nq[0], nq[1], nq[2]))
-    
-    def test_get_dispersion(self):
-        # Example: FCC-Fe
-        lattice_constant = LatticeConstant(2.58, 2.58, 2.58, 60, 60, 60)
-        lattice = EmptyLattice(lattice_constant)
+        eig, delta_eig = self.epr.calculate_with_grid(n_k, n_q)
 
-        phonon = DebyeModel(lattice, 470.0, 1, AtomicWeight.table["Fe"] * Mass.DALTON["->"])
-
-        q_names = ["L", "G", "X"]
-        q_via = []
+        self.assertEqual(eig.shape, delta_eig.shape)
+    
+    def test_calculate_with_path(self):
+        k_names = ["G", "H", "N", "G", "P", "H"]
+        n_split = 20
         
-        for name in q_names:
-            q_via.append(SpecialPoints.FCC[name])
+        n_q = np.array([5]*3)
         
-        x, omega, x_special = phonon.get_dispersion(*q_via)
-
-        self.assertEqual(len(omega), len(x))
-        self.assertEqual(len(q_names), len(x_special))
+        k, eig, delta_eig, special_k = self.epr.calculate_with_path(k_names, n_split, n_q)
+        
+        self.assertEqual(eig.shape, delta_eig.shape)
+        self.assertEqual(len(k_names), len(special_k))
```

