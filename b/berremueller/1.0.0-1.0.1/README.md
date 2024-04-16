# Comparing `tmp/berremueller-1.0.0.tar.gz` & `tmp/berremueller-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "berremueller-1.0.0.tar", last modified: Mon Apr 15 22:45:33 2024, max compression
+gzip compressed data, was "berremueller-1.0.1.tar", last modified: Tue Apr 16 23:09:53 2024, max compression
```

## Comparing `berremueller-1.0.0.tar` & `berremueller-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 22:45:33.884325 berremueller-1.0.0/
--rw-rw-rw-   0        0        0    35823 2023-09-01 00:44:10.000000 berremueller-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1735 2024-04-15 22:45:33.884325 berremueller-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1347 2024-01-02 02:45:51.000000 berremueller-1.0.0/README.md
--rw-rw-rw-   0        0        0      475 2024-04-15 22:45:19.000000 berremueller-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-15 22:45:33.884325 berremueller-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-15 22:45:33.846606 berremueller-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-15 22:45:33.864461 berremueller-1.0.0/src/berremueller/
--rw-rw-rw-   0        0        0        0 2024-04-15 22:10:08.000000 berremueller-1.0.0/src/berremueller/__init__.py
--rw-rw-rw-   0        0        0    45100 2024-01-10 20:46:11.000000 berremueller-1.0.0/src/berremueller/berreman_mueller.py
--rw-rw-rw-   0        0        0     4818 2024-01-08 17:48:37.000000 berremueller-1.0.0/src/berremueller/cholesteric.py
--rw-rw-rw-   0        0        0    77842 2024-04-12 23:19:17.000000 berremueller-1.0.0/src/berremueller/dielectric_tensor.py
--rw-rw-rw-   0        0        0     3607 2024-01-10 20:46:11.000000 berremueller-1.0.0/src/berremueller/field_plotting.py
--rw-rw-rw-   0        0        0     3318 2023-12-13 19:38:52.000000 berremueller-1.0.0/src/berremueller/full_berreman.py
--rw-rw-rw-   0        0        0    61593 2024-01-08 01:39:15.000000 berremueller-1.0.0/src/berremueller/mueller.py
--rw-rw-rw-   0        0        0   157171 2024-03-22 01:59:54.000000 berremueller-1.0.0/src/berremueller/pyllama.py
--rw-rw-rw-   0        0        0     5071 2024-01-10 20:46:11.000000 berremueller-1.0.0/src/berremueller/python_util.py
-drwxrwxrwx   0        0        0        0 2024-04-15 22:45:33.883325 berremueller-1.0.0/src/berremueller.egg-info/
--rw-rw-rw-   0        0        0     1735 2024-04-15 22:45:33.000000 berremueller-1.0.0/src/berremueller.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      524 2024-04-15 22:45:33.000000 berremueller-1.0.0/src/berremueller.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 22:45:33.000000 berremueller-1.0.0/src/berremueller.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-04-15 22:45:33.000000 berremueller-1.0.0/src/berremueller.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-15 22:45:33.000000 berremueller-1.0.0/src/berremueller.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 23:09:53.252728 berremueller-1.0.1/
+-rw-rw-rw-   0        0        0    35823 2023-09-01 00:44:10.000000 berremueller-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1735 2024-04-16 23:09:53.251729 berremueller-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1347 2024-01-02 02:45:51.000000 berremueller-1.0.1/README.md
+-rw-rw-rw-   0        0        0      475 2024-04-16 23:08:39.000000 berremueller-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-16 23:09:53.252728 berremueller-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0       41 2024-04-16 23:09:45.000000 berremueller-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 23:09:53.213038 berremueller-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-16 23:09:53.235626 berremueller-1.0.1/src/berremueller/
+-rw-rw-rw-   0        0        0        2 2024-04-16 23:07:11.000000 berremueller-1.0.1/src/berremueller/__init__.py
+-rw-rw-rw-   0        0        0    45170 2024-04-16 22:52:50.000000 berremueller-1.0.1/src/berremueller/berreman_mueller.py
+-rw-rw-rw-   0        0        0     4818 2024-01-08 17:48:37.000000 berremueller-1.0.1/src/berremueller/cholesteric.py
+-rw-rw-rw-   0        0        0    77864 2024-04-16 22:52:50.000000 berremueller-1.0.1/src/berremueller/dielectric_tensor.py
+-rw-rw-rw-   0        0        0     3607 2024-01-10 20:46:11.000000 berremueller-1.0.1/src/berremueller/field_plotting.py
+-rw-rw-rw-   0        0        0     3318 2023-12-13 19:38:52.000000 berremueller-1.0.1/src/berremueller/full_berreman.py
+-rw-rw-rw-   0        0        0    61615 2024-04-16 22:52:50.000000 berremueller-1.0.1/src/berremueller/mueller.py
+-rw-rw-rw-   0        0        0   157215 2024-04-16 22:52:50.000000 berremueller-1.0.1/src/berremueller/pyllama.py
+-rw-rw-rw-   0        0        0     5071 2024-01-10 20:46:11.000000 berremueller-1.0.1/src/berremueller/python_util.py
+drwxrwxrwx   0        0        0        0 2024-04-16 23:09:53.250728 berremueller-1.0.1/src/berremueller.egg-info/
+-rw-rw-rw-   0        0        0     1735 2024-04-16 23:09:53.000000 berremueller-1.0.1/src/berremueller.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      533 2024-04-16 23:09:53.000000 berremueller-1.0.1/src/berremueller.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 23:09:53.000000 berremueller-1.0.1/src/berremueller.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-04-16 23:09:53.000000 berremueller-1.0.1/src/berremueller.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-16 23:09:53.000000 berremueller-1.0.1/src/berremueller.egg-info/top_level.txt
```

### Comparing `berremueller-1.0.0/LICENSE` & `berremueller-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `berremueller-1.0.0/PKG-INFO` & `berremueller-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: berremueller
-Version: 1.0.0
+Version: 1.0.1
 Summary: A library for implementing the Berreman 4X4 matrix method alongside Mueller matrices
 Author-email: Andrew Salij <andrewsalij@gmail.com>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: scipy
```

### Comparing `berremueller-1.0.0/README.md` & `berremueller-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `berremueller-1.0.0/src/berremueller/berreman_mueller.py` & `berremueller-1.0.1/src/berremueller/berreman_mueller.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import copy
 
 import numpy as np
 from numpy.linalg import inv
 from numpy.linalg import multi_dot
 
-import cholesteric
-import mueller
-import pyllama
-import dielectric_tensor as dt
+from src.berremueller import cholesteric
+from src.berremueller import  mueller
+from src.berremueller import pyllama
+from src.berremueller import dielectric_tensor as dt
 import warnings
-import pandas as pd
+
 
 '''Handling of Jones vectors and Mueller matrices, particularly those coming from
 numeric calculations
 
 Mostly an extension of mueller.py with specific focus on transfer/scattering matrix calcs
 
 Also includes functions for the construction of cavity systems for transfer/scattering matrix
```

### Comparing `berremueller-1.0.0/src/berremueller/cholesteric.py` & `berremueller-1.0.1/src/berremueller/cholesteric.py`

 * *Files identical despite different names*

### Comparing `berremueller-1.0.0/src/berremueller/dielectric_tensor.py` & `berremueller-1.0.1/src/berremueller/dielectric_tensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from scipy.special import factorial
 from scipy.signal import find_peaks
 import scipy.spatial as scp_spa
-import python_util as pu
+from src.berremueller import python_util as pu
 from scipy.spatial.transform import Rotation
 from warnings import warn
 
 '''
 Handles the dielectric function in 3D for sets of Lorentz oscillators.
 Also handles the core of LDLB theory (https://doi.org/10.1021/jacs.1c06752)
```

### Comparing `berremueller-1.0.0/src/berremueller/field_plotting.py` & `berremueller-1.0.1/src/berremueller/field_plotting.py`

 * *Files identical despite different names*

### Comparing `berremueller-1.0.0/src/berremueller/full_berreman.py` & `berremueller-1.0.1/src/berremueller/full_berreman.py`

 * *Files identical despite different names*

### Comparing `berremueller-1.0.0/src/berremueller/mueller.py` & `berremueller-1.0.1/src/berremueller/mueller.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from scipy.linalg import expm
 import matplotlib.pyplot as plt
-import python_util as pu
+from src.berremueller import python_util as pu
 import scipy.linalg
 import scipy
 import collections
 
 
 '''Numeric and symbolic handling of Mueller matrices with some plotting functions
```

### Comparing `berremueller-1.0.0/src/berremueller/pyllama.py` & `berremueller-1.0.1/src/berremueller/pyllama.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import numpy as np
 from numpy import linalg as la_np
 from scipy import linalg as la_sp
 import warnings
 import time  # to calculate the time elapsed for a spectrum
 import pickle  # to save as Pickle file
 import scipy.io  # to save as Matlab file
-import cholesteric
-import full_berreman
+from src.berremueller import cholesteric
+from src.berremueller import full_berreman
 
 
 '''
 This is a modified version of the open source Pyllama project
 (https://doi.org/10.1016/j.cpc.2021.108256)
 
 Note that the circular polarization convention here is that RHP is (1,-1j) as a Jones vector,
```

### Comparing `berremueller-1.0.0/src/berremueller/python_util.py` & `berremueller-1.0.1/src/berremueller/python_util.py`

 * *Files identical despite different names*

### Comparing `berremueller-1.0.0/src/berremueller.egg-info/PKG-INFO` & `berremueller-1.0.1/src/berremueller.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: berremueller
-Version: 1.0.0
+Version: 1.0.1
 Summary: A library for implementing the Berreman 4X4 matrix method alongside Mueller matrices
 Author-email: Andrew Salij <andrewsalij@gmail.com>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: scipy
```

### Comparing `berremueller-1.0.0/src/berremueller.egg-info/SOURCES.txt` & `berremueller-1.0.1/src/berremueller.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
+setup.py
 src/berremueller/__init__.py
 src/berremueller/berreman_mueller.py
 src/berremueller/cholesteric.py
 src/berremueller/dielectric_tensor.py
 src/berremueller/field_plotting.py
 src/berremueller/full_berreman.py
 src/berremueller/mueller.py
```

