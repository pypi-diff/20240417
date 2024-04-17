# Comparing `tmp/abc_network-0.1.1.tar.gz` & `tmp/abc_network-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abc_network-0.1.1.tar", last modified: Wed Apr 17 16:11:12 2024, max compression
+gzip compressed data, was "abc_network-0.1.2.tar", last modified: Wed Apr 17 16:15:37 2024, max compression
```

## Comparing `abc_network-0.1.1.tar` & `abc_network-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 guillermo  (1000) guillermo  (1000)        0 2024-04-17 16:11:12.507397 abc_network-0.1.1/
-drwxrwxr-x   0 guillermo  (1000) guillermo  (1000)        0 2024-04-17 16:11:12.503397 abc_network-0.1.1/ABC/
--rw-rw-r--   0 guillermo  (1000) guillermo  (1000)       22 2024-04-17 16:10:59.000000 abc_network-0.1.1/ABC/__init__.py
--rw-rw-r--   0 guillermo  (1000) guillermo  (1000)     7240 2024-04-15 14:28:31.000000 abc_network-0.1.1/ABC/data.py
--rw-rw-r--   0 guillermo  (1000) guillermo  (1000)    63021 2024-04-17 16:03:23.000000 abc_network-0.1.1/ABC/model.py
--rw-rw-r--   0 guillermo  (1000) guillermo  (1000)    22287 2024-04-15 14:28:31.000000 abc_network-0.1.1/ABC/results.py
--rw-rw-r--   0 guillermo  (1000) guillermo  (1000)     9365 2024-04-03 10:59:23.000000 abc_network-0.1.1/ABC/utils.py
--rw-rw-r--   0 guillermo  (1000) guillermo  (1000)    35149 2024-03-12 17:00:51.000000 abc_network-0.1.1/LICENSE
--rw-r--r--   0 guillermo  (1000) guillermo  (1000)     6573 2024-04-17 16:11:12.507397 abc_network-0.1.1/PKG-INFO
--rw-rw-r--   0 guillermo  (1000) guillermo  (1000)     5695 2024-04-17 16:04:56.000000 abc_network-0.1.1/README.md
-drwxrwxr-x   0 guillermo  (1000) guillermo  (1000)        0 2024-04-17 16:11:12.503397 abc_network-0.1.1/abc_network.egg-info/
--rw-r--r--   0 guillermo  (1000) guillermo  (1000)     6573 2024-04-17 16:11:12.000000 abc_network-0.1.1/abc_network.egg-info/PKG-INFO
--rw-rw-r--   0 guillermo  (1000) guillermo  (1000)      357 2024-04-17 16:11:12.000000 abc_network-0.1.1/abc_network.egg-info/SOURCES.txt
--rw-rw-r--   0 guillermo  (1000) guillermo  (1000)        1 2024-04-17 16:11:12.000000 abc_network-0.1.1/abc_network.egg-info/dependency_links.txt
--rw-rw-r--   0 guillermo  (1000) guillermo  (1000)       39 2024-04-17 16:11:12.000000 abc_network-0.1.1/abc_network.egg-info/entry_points.txt
--rw-rw-r--   0 guillermo  (1000) guillermo  (1000)        1 2024-04-17 11:38:45.000000 abc_network-0.1.1/abc_network.egg-info/not-zip-safe
--rw-rw-r--   0 guillermo  (1000) guillermo  (1000)       88 2024-04-17 16:11:12.000000 abc_network-0.1.1/abc_network.egg-info/requires.txt
--rw-rw-r--   0 guillermo  (1000) guillermo  (1000)        4 2024-04-17 16:11:12.000000 abc_network-0.1.1/abc_network.egg-info/top_level.txt
--rw-rw-r--   0 guillermo  (1000) guillermo  (1000)       81 2024-04-17 09:49:35.000000 abc_network-0.1.1/pyproject.toml
--rw-rw-r--   0 guillermo  (1000) guillermo  (1000)      995 2024-04-17 16:11:12.507397 abc_network-0.1.1/setup.cfg
+drwxrwxr-x   0 guillermo  (1000) guillermo  (1000)        0 2024-04-17 16:15:37.347993 abc_network-0.1.2/
+drwxrwxr-x   0 guillermo  (1000) guillermo  (1000)        0 2024-04-17 16:15:37.347993 abc_network-0.1.2/ABC/
+-rw-rw-r--   0 guillermo  (1000) guillermo  (1000)       22 2024-04-17 16:15:32.000000 abc_network-0.1.2/ABC/__init__.py
+-rw-rw-r--   0 guillermo  (1000) guillermo  (1000)     7240 2024-04-15 14:28:31.000000 abc_network-0.1.2/ABC/data.py
+-rw-rw-r--   0 guillermo  (1000) guillermo  (1000)    63021 2024-04-17 16:03:23.000000 abc_network-0.1.2/ABC/model.py
+-rw-rw-r--   0 guillermo  (1000) guillermo  (1000)    22287 2024-04-15 14:28:31.000000 abc_network-0.1.2/ABC/results.py
+-rw-rw-r--   0 guillermo  (1000) guillermo  (1000)     9372 2024-04-17 16:14:39.000000 abc_network-0.1.2/ABC/utils.py
+-rw-rw-r--   0 guillermo  (1000) guillermo  (1000)    35149 2024-03-12 17:00:51.000000 abc_network-0.1.2/LICENSE
+-rw-r--r--   0 guillermo  (1000) guillermo  (1000)     6573 2024-04-17 16:15:37.347993 abc_network-0.1.2/PKG-INFO
+-rw-rw-r--   0 guillermo  (1000) guillermo  (1000)     5695 2024-04-17 16:04:56.000000 abc_network-0.1.2/README.md
+drwxrwxr-x   0 guillermo  (1000) guillermo  (1000)        0 2024-04-17 16:15:37.347993 abc_network-0.1.2/abc_network.egg-info/
+-rw-r--r--   0 guillermo  (1000) guillermo  (1000)     6573 2024-04-17 16:15:37.000000 abc_network-0.1.2/abc_network.egg-info/PKG-INFO
+-rw-rw-r--   0 guillermo  (1000) guillermo  (1000)      357 2024-04-17 16:15:37.000000 abc_network-0.1.2/abc_network.egg-info/SOURCES.txt
+-rw-rw-r--   0 guillermo  (1000) guillermo  (1000)        1 2024-04-17 16:15:37.000000 abc_network-0.1.2/abc_network.egg-info/dependency_links.txt
+-rw-rw-r--   0 guillermo  (1000) guillermo  (1000)       39 2024-04-17 16:15:37.000000 abc_network-0.1.2/abc_network.egg-info/entry_points.txt
+-rw-rw-r--   0 guillermo  (1000) guillermo  (1000)        1 2024-04-17 11:38:45.000000 abc_network-0.1.2/abc_network.egg-info/not-zip-safe
+-rw-rw-r--   0 guillermo  (1000) guillermo  (1000)       88 2024-04-17 16:15:37.000000 abc_network-0.1.2/abc_network.egg-info/requires.txt
+-rw-rw-r--   0 guillermo  (1000) guillermo  (1000)        4 2024-04-17 16:15:37.000000 abc_network-0.1.2/abc_network.egg-info/top_level.txt
+-rw-rw-r--   0 guillermo  (1000) guillermo  (1000)       81 2024-04-17 09:49:35.000000 abc_network-0.1.2/pyproject.toml
+-rw-rw-r--   0 guillermo  (1000) guillermo  (1000)      995 2024-04-17 16:15:37.347993 abc_network-0.1.2/setup.cfg
```

### Comparing `abc_network-0.1.1/ABC/data.py` & `abc_network-0.1.2/ABC/data.py`

 * *Files identical despite different names*

### Comparing `abc_network-0.1.1/ABC/model.py` & `abc_network-0.1.2/ABC/model.py`

 * *Files identical despite different names*

### Comparing `abc_network-0.1.1/ABC/results.py` & `abc_network-0.1.2/ABC/results.py`

 * *Files identical despite different names*

### Comparing `abc_network-0.1.1/ABC/utils.py` & `abc_network-0.1.2/ABC/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 import numpy as np
 import pandas as pd
 import scipy as sp
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 
-THIS_DIR = osp.dirname(osp.realpath(__file__))
-PROJECT_DIR = osp.abspath(osp.join(THIS_DIR, os.pardir))
+PACKAGE_DIR = osp.dirname(osp.realpath(__file__))
+PROJECT_DIR = osp.abspath(osp.join(PACKAGE_DIR, os.pardir))
 
 
 def plot_pairwise_relations(mat, names, title="", cbar_label="", sym=False, ax: plt.Axes = None, row: int = None,
                             log: bool = False, vmin=None, vmax=None, cbar: bool = True, norm_kwargs: dict = {},
                             boundaries=None, cbar_ticklabels=None, cbar_kwargs: dict = {}, bubbles: bool = False,
                             bubble_area_multiplier=30, **im_kwargs):
     """
@@ -197,7 +197,8 @@
     :param df: pandas.DataFrame in 'long-format', ie with rows as patients and columns as variables
     :param columns: list of columns containing LTC information (values must be binary)
     :return: X (np.ndarray), square matrix with co-occurrence counts in the off-diagonals and LTC counts in the diagonal
     """
     long_mat = df[columns].values
     assert (valid := ((long_mat == 0) | (long_mat == 1))).all(), f"{(~valid).sum()} cells don't contain binary values."
     return np.matmul(long_mat.T, long_mat)
+
```

### Comparing `abc_network-0.1.1/LICENSE` & `abc_network-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `abc_network-0.1.1/PKG-INFO` & `abc_network-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abc_network
-Version: 0.1.1
+Version: 0.1.2
 Summary: This package provides code linked to the paper "Multimorbidity analysis with low condition counts: a robust Bayesian approach for small but important subgroups" <https://authors.elsevier.com/sd/article/S2352396424001166>.
 Home-page: https://github.com/Juillermo/ABC.git
 Author: Guillermo Romero Moreno
 Author-email: Guillermo.RomeroMoreno@ed.ac.uk
 License: GNU GENERAL PUBLIC LICENSE
 Keywords: Bayesian,Multimorbidity
 Classifier: Programming Language :: Python :: 3
```

### Comparing `abc_network-0.1.1/README.md` & `abc_network-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `abc_network-0.1.1/abc_network.egg-info/PKG-INFO` & `abc_network-0.1.2/abc_network.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abc_network
-Version: 0.1.1
+Version: 0.1.2
 Summary: This package provides code linked to the paper "Multimorbidity analysis with low condition counts: a robust Bayesian approach for small but important subgroups" <https://authors.elsevier.com/sd/article/S2352396424001166>.
 Home-page: https://github.com/Juillermo/ABC.git
 Author: Guillermo Romero Moreno
 Author-email: Guillermo.RomeroMoreno@ed.ac.uk
 License: GNU GENERAL PUBLIC LICENSE
 Keywords: Bayesian,Multimorbidity
 Classifier: Programming Language :: Python :: 3
```

### Comparing `abc_network-0.1.1/setup.cfg` & `abc_network-0.1.2/setup.cfg`

 * *Files identical despite different names*

