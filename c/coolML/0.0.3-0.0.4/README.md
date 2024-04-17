# Comparing `tmp/coolML-0.0.3.tar.gz` & `tmp/coolML-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolML-0.0.3.tar", last modified: Wed Apr 17 08:51:44 2024, max compression
+gzip compressed data, was "coolML-0.0.4.tar", last modified: Wed Apr 17 08:58:59 2024, max compression
```

## Comparing `coolML-0.0.3.tar` & `coolML-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 08:51:44.038751 coolML-0.0.3/
--rw-r--r--   0 root         (0) root         (0)     3619 2024-04-17 08:51:44.038751 coolML-0.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2913 2024-04-17 08:51:32.000000 coolML-0.0.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 08:51:44.038751 coolML-0.0.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1405 2024-04-17 08:51:32.000000 coolML-0.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 08:51:44.034751 coolML-0.0.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 08:51:44.038751 coolML-0.0.3/src/coolML/
--rw-rw-rw-   0 root         (0) root         (0)       99 2024-04-17 08:51:32.000000 coolML-0.0.3/src/coolML/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23002 2024-04-17 08:51:32.000000 coolML-0.0.3/src/coolML/data_processing.py
--rw-rw-rw-   0 root         (0) root         (0)     7840 2024-04-17 08:51:32.000000 coolML-0.0.3/src/coolML/model_fitting.py
--rw-rw-rw-   0 root         (0) root         (0)     8424 2024-04-17 08:51:32.000000 coolML-0.0.3/src/coolML/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 08:51:44.038751 coolML-0.0.3/src/coolML.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3619 2024-04-17 08:51:43.000000 coolML-0.0.3/src/coolML.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      289 2024-04-17 08:51:43.000000 coolML-0.0.3/src/coolML.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 08:51:43.000000 coolML-0.0.3/src/coolML.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-04-17 08:51:43.000000 coolML-0.0.3/src/coolML.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-17 08:51:43.000000 coolML-0.0.3/src/coolML.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 08:58:59.486967 coolML-0.0.4/
+-rw-r--r--   0 root         (0) root         (0)     3617 2024-04-17 08:58:59.482967 coolML-0.0.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2911 2024-04-17 08:58:47.000000 coolML-0.0.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 08:58:59.486967 coolML-0.0.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1405 2024-04-17 08:58:47.000000 coolML-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 08:58:59.482967 coolML-0.0.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 08:58:59.482967 coolML-0.0.4/src/coolML/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2024-04-17 08:58:47.000000 coolML-0.0.4/src/coolML/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23022 2024-04-17 08:58:47.000000 coolML-0.0.4/src/coolML/data_processing.py
+-rw-rw-rw-   0 root         (0) root         (0)     7840 2024-04-17 08:58:47.000000 coolML-0.0.4/src/coolML/model_fitting.py
+-rw-rw-rw-   0 root         (0) root         (0)     8424 2024-04-17 08:58:47.000000 coolML-0.0.4/src/coolML/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 08:58:59.482967 coolML-0.0.4/src/coolML.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3617 2024-04-17 08:58:59.000000 coolML-0.0.4/src/coolML.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      289 2024-04-17 08:58:59.000000 coolML-0.0.4/src/coolML.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 08:58:59.000000 coolML-0.0.4/src/coolML.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-17 08:58:59.000000 coolML-0.0.4/src/coolML.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-17 08:58:59.000000 coolML-0.0.4/src/coolML.egg-info/top_level.txt
```

### Comparing `coolML-0.0.3/PKG-INFO` & `coolML-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coolML
-Version: 0.0.3
+Version: 0.0.4
 Summary: Cool ML is a machine learning workflow developed to optimize thermionic double-assymmetric barrier heterostructures based on semiconductors
 Home-page: https://gitlab.citius.usc.es/julian.garcia.fernandez/coolML
 Author: Julian Garcia Fernandez 
 Author-email: julian.garcia.fernandez2@usc.es
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -35,19 +35,19 @@
     sudo apt update
     sudo apt install python3-pip
 
 **Instalation of MLFoMpy via pip3**
 
 For basic usage of the tool (figure of merit extraction), install the tool using pip3:
 
-    pip3 install cool-ml
+    pip3 install coolML
 
 and check the library is installed by importing it from a **python3 terminal**:
 
-    import cool_ml
+    import coolML
 
 Unless an error comes up, Cool ML is now installed on your environment.
 
 <!-- For more detailed explanation about instalation, please, check
 the [documentation](https://mlfompy.readthedocs.io/#getting-started). -->
 
 <!-- **Documentation generation**
```

### Comparing `coolML-0.0.3/README.md` & `coolML-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,19 +19,19 @@
     sudo apt update
     sudo apt install python3-pip
 
 **Instalation of MLFoMpy via pip3**
 
 For basic usage of the tool (figure of merit extraction), install the tool using pip3:
 
-    pip3 install cool-ml
+    pip3 install coolML
 
 and check the library is installed by importing it from a **python3 terminal**:
 
-    import cool_ml
+    import coolML
 
 Unless an error comes up, Cool ML is now installed on your environment.
 
 <!-- For more detailed explanation about instalation, please, check
 the [documentation](https://mlfompy.readthedocs.io/#getting-started). -->
 
 <!-- **Documentation generation**
```

### Comparing `coolML-0.0.3/setup.py` & `coolML-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description=''
     with open(Path(Path(__file__).parent,'README.md'), 'r') as fh:
         long_description=fh.read()
     return long_description
 
 setuptools.setup(
     name='coolML',
-    version='0.0.3',
+    version='0.0.4',
     description='Cool ML is a machine learning workflow developed to optimize thermionic double-assymmetric barrier heterostructures based on semiconductors',
     long_description=get_long_description(),
     long_description_content_type='text/markdown',
     author='Julian Garcia Fernandez ',
     author_email='julian.garcia.fernandez2@usc.es',
     url='https://gitlab.citius.usc.es/julian.garcia.fernandez/coolML',
     setup_requires=['setuptools'],
```

### Comparing `coolML-0.0.3/src/coolML/data_processing.py` & `coolML-0.0.4/src/coolML/data_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import pandas as pd 
 import torch
 import numpy as np
 from sklearn.model_selection import train_test_split
 from sklearn.decomposition import PCA
-from sklearn.metrics import r2_score 
 from sklearn.preprocessing import  StandardScaler, MinMaxScaler
 from pickle import dump
-from time import time
-
 
 def import_cooling_data(path):
     '''
     Import cooling data from csv to pandas dataframes
     Input:
     -----
     - path: path
@@ -349,15 +346,15 @@
     - scaler_ppo: fitted object for the PPo normalization
     '''
     if scaler == 'MinMax':
         scaler_pp = MinMaxScaler()
     else:
         scaler_pp = StandardScaler()
     pp_scaled = scaler_pp.fit_transform(data)
-    dump(scaler_pp, open('scaler_pp.pkl', 'wb'))
+    dump(scaler_pp, open('scaler_objects/scaler_pp.pkl', 'wb'))
     return torch.tensor(pp_scaled, dtype=torch.float32), scaler_pp
 
 def norm_diff_pp_ppo(data, scaler='MinMax'):
     '''
     Normalization of PP-ppo with MinMaxScaler
     -------
     Inputs:
@@ -373,15 +370,15 @@
         fitted object for the PP-PPo normalization
     '''
     if scaler == 'MinMax':
         scaler_pp_ppo = MinMaxScaler()
     else:
         scaler_pp_ppo = StandardScaler()
     diff_pp_ppo_list_scaled = scaler_pp_ppo.fit_transform(data)
-    dump(scaler_pp_ppo, open('scaler_pp_ppo.pkl', 'wb'))
+    dump(scaler_pp_ppo, open('scaler_objects/scaler_pp_ppo.pkl', 'wb'))
     return torch.tensor(diff_pp_ppo_list_scaled, dtype=torch.float32), scaler_pp_ppo
 
 
 def norm_thermal(data, scaler='MinMax'):
     '''
     Normalization of thermal properties CP, Te, W1 and W2 with MinMaxScaler
     -------
@@ -396,15 +393,15 @@
     - scaler_thermal: fitted object for the output normalization
     '''
     if scaler == 'MinMax':
         scaler_thermal = MinMaxScaler()
     else:
         scaler_thermal = StandardScaler()
     thermal = scaler_thermal.fit_transform(data)
-    dump(scaler_thermal, open('scaler_thermal.pkl', 'wb'))
+    dump(scaler_thermal, open('scaler_objects/scaler_thermal.pkl', 'wb'))
     return torch.tensor(thermal, dtype=torch.float32), scaler_thermal
 
 ###################################################################################################################
 ########################################### PCA SECTION ###########################################################
 ###################################################################################################################
 def pca_to_ppo(X_train, X_val, X_test, pc=0.9999, verbosity = False):
     '''
@@ -545,15 +542,15 @@
     '''
     if PC == None:
         PC = 0.95
     ppo_pca = PCA(PC)
     matrix_ppo = np.array(x, dtype=float)
     matrix_ppo_pca = ppo_pca.fit_transform(matrix_ppo)
     components_list_ppo = matrix_ppo_pca.tolist()
-    dump(ppo_pca, open('pca_ppo.joblib', 'wb'))
+    dump(ppo_pca, open('pca_objects/pca_ppo.joblib', 'wb'))
     return torch.tensor(components_list_ppo, dtype=torch.float32), ppo_pca
 
 def PCA_pp(x,PC=None):
     '''
     Performing PCA to ppo with the desired PC
     -------
     Inputs:
@@ -566,15 +563,15 @@
     '''
     if PC == None:
         PC = 0.95
     pp_pca = PCA(PC)
     matrix_pp = np.array(x, dtype=float)
     matrix_pp_pca = pp_pca.fit_transform(matrix_pp)
     components_list_pp = matrix_pp_pca.tolist()
-    dump(pp_pca, open('pca_pp.joblib', 'wb'))
+    dump(pp_pca, open('pca_objects/pca_pp.joblib', 'wb'))
     return torch.tensor(components_list_pp, dtype=torch.float32), pp_pca
 
 
 def PCA_diff_pp_ppo(x,PC=None):
     '''
     Performing PCA to PP-ppo with the desired PC
     -------
@@ -588,9 +585,9 @@
     '''
     if PC == None:
         PC = 0.95
     diff_pp_ppo_pca = PCA(PC)
     matrix_diff_pp_ppo = np.array(x, dtype=float)
     matrix_diff_pp_ppo_pca = diff_pp_ppo_pca.fit_transform(matrix_diff_pp_ppo)
     components_list_diff_pp_ppo = matrix_diff_pp_ppo_pca.tolist()
-    dump(diff_pp_ppo_pca, open('pca_diff_pp_ppo.joblib', 'wb'))
+    dump(diff_pp_ppo_pca, open('pca_objects/pca_diff_pp_ppo.joblib', 'wb'))
     return components_list_diff_pp_ppo, diff_pp_ppo_pca
```

### Comparing `coolML-0.0.3/src/coolML/model_fitting.py` & `coolML-0.0.4/src/coolML/model_fitting.py`

 * *Files identical despite different names*

### Comparing `coolML-0.0.3/src/coolML/models.py` & `coolML-0.0.4/src/coolML/models.py`

 * *Files identical despite different names*

### Comparing `coolML-0.0.3/src/coolML.egg-info/PKG-INFO` & `coolML-0.0.4/src/coolML.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coolML
-Version: 0.0.3
+Version: 0.0.4
 Summary: Cool ML is a machine learning workflow developed to optimize thermionic double-assymmetric barrier heterostructures based on semiconductors
 Home-page: https://gitlab.citius.usc.es/julian.garcia.fernandez/coolML
 Author: Julian Garcia Fernandez 
 Author-email: julian.garcia.fernandez2@usc.es
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -35,19 +35,19 @@
     sudo apt update
     sudo apt install python3-pip
 
 **Instalation of MLFoMpy via pip3**
 
 For basic usage of the tool (figure of merit extraction), install the tool using pip3:
 
-    pip3 install cool-ml
+    pip3 install coolML
 
 and check the library is installed by importing it from a **python3 terminal**:
 
-    import cool_ml
+    import coolML
 
 Unless an error comes up, Cool ML is now installed on your environment.
 
 <!-- For more detailed explanation about instalation, please, check
 the [documentation](https://mlfompy.readthedocs.io/#getting-started). -->
 
 <!-- **Documentation generation**
```

