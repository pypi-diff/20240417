# Comparing `tmp/abc_network-0.1.0.tar.gz` & `tmp/abc_network-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abc_network-0.1.0.tar", last modified: Wed Apr 17 11:38:45 2024, max compression
+gzip compressed data, was "abc_network-0.1.1.tar", last modified: Wed Apr 17 16:11:12 2024, max compression
```

## Comparing `abc_network-0.1.0.tar` & `abc_network-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 guillermo  (1000) guillermo  (1000)        0 2024-04-17 11:38:45.333043 abc_network-0.1.0/
-drwxrwxr-x   0 guillermo  (1000) guillermo  (1000)        0 2024-04-17 11:38:45.333043 abc_network-0.1.0/ABC/
--rw-rw-r--   0 guillermo  (1000) guillermo  (1000)       22 2024-04-17 10:04:38.000000 abc_network-0.1.0/ABC/__init__.py
--rw-rw-r--   0 guillermo  (1000) guillermo  (1000)     7240 2024-04-15 14:28:31.000000 abc_network-0.1.0/ABC/data.py
--rw-rw-r--   0 guillermo  (1000) guillermo  (1000)    63020 2024-04-15 17:09:56.000000 abc_network-0.1.0/ABC/model.py
--rw-rw-r--   0 guillermo  (1000) guillermo  (1000)    22287 2024-04-15 14:28:31.000000 abc_network-0.1.0/ABC/results.py
--rw-rw-r--   0 guillermo  (1000) guillermo  (1000)     9365 2024-04-03 10:59:23.000000 abc_network-0.1.0/ABC/utils.py
--rw-rw-r--   0 guillermo  (1000) guillermo  (1000)    35149 2024-03-12 17:00:51.000000 abc_network-0.1.0/LICENSE
--rw-r--r--   0 guillermo  (1000) guillermo  (1000)     6549 2024-04-17 11:38:45.333043 abc_network-0.1.0/PKG-INFO
--rw-rw-r--   0 guillermo  (1000) guillermo  (1000)     5671 2024-04-15 17:08:15.000000 abc_network-0.1.0/README.md
-drwxrwxr-x   0 guillermo  (1000) guillermo  (1000)        0 2024-04-17 11:38:45.333043 abc_network-0.1.0/abc_network.egg-info/
--rw-r--r--   0 guillermo  (1000) guillermo  (1000)     6549 2024-04-17 11:38:45.000000 abc_network-0.1.0/abc_network.egg-info/PKG-INFO
--rw-rw-r--   0 guillermo  (1000) guillermo  (1000)      357 2024-04-17 11:38:45.000000 abc_network-0.1.0/abc_network.egg-info/SOURCES.txt
--rw-rw-r--   0 guillermo  (1000) guillermo  (1000)        1 2024-04-17 11:38:45.000000 abc_network-0.1.0/abc_network.egg-info/dependency_links.txt
--rw-rw-r--   0 guillermo  (1000) guillermo  (1000)       39 2024-04-17 11:38:45.000000 abc_network-0.1.0/abc_network.egg-info/entry_points.txt
--rw-rw-r--   0 guillermo  (1000) guillermo  (1000)        1 2024-04-17 11:38:45.000000 abc_network-0.1.0/abc_network.egg-info/not-zip-safe
--rw-rw-r--   0 guillermo  (1000) guillermo  (1000)       88 2024-04-17 11:38:45.000000 abc_network-0.1.0/abc_network.egg-info/requires.txt
--rw-rw-r--   0 guillermo  (1000) guillermo  (1000)        4 2024-04-17 11:38:45.000000 abc_network-0.1.0/abc_network.egg-info/top_level.txt
--rw-rw-r--   0 guillermo  (1000) guillermo  (1000)       81 2024-04-17 09:49:35.000000 abc_network-0.1.0/pyproject.toml
--rw-rw-r--   0 guillermo  (1000) guillermo  (1000)      995 2024-04-17 11:38:45.333043 abc_network-0.1.0/setup.cfg
+drwxrwxr-x   0 guillermo  (1000) guillermo  (1000)        0 2024-04-17 16:11:12.507397 abc_network-0.1.1/
+drwxrwxr-x   0 guillermo  (1000) guillermo  (1000)        0 2024-04-17 16:11:12.503397 abc_network-0.1.1/ABC/
+-rw-rw-r--   0 guillermo  (1000) guillermo  (1000)       22 2024-04-17 16:10:59.000000 abc_network-0.1.1/ABC/__init__.py
+-rw-rw-r--   0 guillermo  (1000) guillermo  (1000)     7240 2024-04-15 14:28:31.000000 abc_network-0.1.1/ABC/data.py
+-rw-rw-r--   0 guillermo  (1000) guillermo  (1000)    63021 2024-04-17 16:03:23.000000 abc_network-0.1.1/ABC/model.py
+-rw-rw-r--   0 guillermo  (1000) guillermo  (1000)    22287 2024-04-15 14:28:31.000000 abc_network-0.1.1/ABC/results.py
+-rw-rw-r--   0 guillermo  (1000) guillermo  (1000)     9365 2024-04-03 10:59:23.000000 abc_network-0.1.1/ABC/utils.py
+-rw-rw-r--   0 guillermo  (1000) guillermo  (1000)    35149 2024-03-12 17:00:51.000000 abc_network-0.1.1/LICENSE
+-rw-r--r--   0 guillermo  (1000) guillermo  (1000)     6573 2024-04-17 16:11:12.507397 abc_network-0.1.1/PKG-INFO
+-rw-rw-r--   0 guillermo  (1000) guillermo  (1000)     5695 2024-04-17 16:04:56.000000 abc_network-0.1.1/README.md
+drwxrwxr-x   0 guillermo  (1000) guillermo  (1000)        0 2024-04-17 16:11:12.503397 abc_network-0.1.1/abc_network.egg-info/
+-rw-r--r--   0 guillermo  (1000) guillermo  (1000)     6573 2024-04-17 16:11:12.000000 abc_network-0.1.1/abc_network.egg-info/PKG-INFO
+-rw-rw-r--   0 guillermo  (1000) guillermo  (1000)      357 2024-04-17 16:11:12.000000 abc_network-0.1.1/abc_network.egg-info/SOURCES.txt
+-rw-rw-r--   0 guillermo  (1000) guillermo  (1000)        1 2024-04-17 16:11:12.000000 abc_network-0.1.1/abc_network.egg-info/dependency_links.txt
+-rw-rw-r--   0 guillermo  (1000) guillermo  (1000)       39 2024-04-17 16:11:12.000000 abc_network-0.1.1/abc_network.egg-info/entry_points.txt
+-rw-rw-r--   0 guillermo  (1000) guillermo  (1000)        1 2024-04-17 11:38:45.000000 abc_network-0.1.1/abc_network.egg-info/not-zip-safe
+-rw-rw-r--   0 guillermo  (1000) guillermo  (1000)       88 2024-04-17 16:11:12.000000 abc_network-0.1.1/abc_network.egg-info/requires.txt
+-rw-rw-r--   0 guillermo  (1000) guillermo  (1000)        4 2024-04-17 16:11:12.000000 abc_network-0.1.1/abc_network.egg-info/top_level.txt
+-rw-rw-r--   0 guillermo  (1000) guillermo  (1000)       81 2024-04-17 09:49:35.000000 abc_network-0.1.1/pyproject.toml
+-rw-rw-r--   0 guillermo  (1000) guillermo  (1000)      995 2024-04-17 16:11:12.507397 abc_network-0.1.1/setup.cfg
```

### Comparing `abc_network-0.1.0/ABC/data.py` & `abc_network-0.1.1/ABC/data.py`

 * *Files identical despite different names*

### Comparing `abc_network-0.1.0/ABC/model.py` & `abc_network-0.1.1/ABC/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 import scipy as sp
 import pandas as pd
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import seaborn as sns
 
 # Own packages
-from ABC.utils import plot_pairwise_relations, identify_LTC, MLTC_count, PROJECT_DIR, compute_RR
+from ABC.utils import plot_pairwise_relations, identify_LTC, MLTC_count, compute_RR, PACKAGE_DIR
 
-MODELS_PATH = osp.abspath(osp.join(PROJECT_DIR, 'models'))  # directory from which to load model specifications
+MODELS_PATH = osp.abspath(osp.join(PACKAGE_DIR, 'models'))  # directory from which to load model specifications
 FIT_MODELS_PATH = "output"  # directory to which to save the parameters of fit models
 os.makedirs(FIT_MODELS_PATH, exist_ok=True)  # create the directory if it doesn't exist
 
 
 def find_mode_data_groups(samples, window_width=0.01) -> tuple:
     """
     Find the mode of a unimodal distribution from a set of samples. It slides a window including
@@ -1239,7 +1239,8 @@
     results.to_csv(results_file := f"{FIT_MODELS_PATH}/results-{fname}.csv")
 
     print(f"Results have been saved into files '{ABC_file}' and '{results_file}'.")
 
 
 if __name__ == "__main__":
     main()
+
```

### Comparing `abc_network-0.1.0/ABC/results.py` & `abc_network-0.1.1/ABC/results.py`

 * *Files identical despite different names*

### Comparing `abc_network-0.1.0/ABC/utils.py` & `abc_network-0.1.1/ABC/utils.py`

 * *Files identical despite different names*

### Comparing `abc_network-0.1.0/LICENSE` & `abc_network-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `abc_network-0.1.0/PKG-INFO` & `abc_network-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abc_network
-Version: 0.1.0
+Version: 0.1.1
 Summary: This package provides code linked to the paper "Multimorbidity analysis with low condition counts: a robust Bayesian approach for small but important subgroups" <https://authors.elsevier.com/sd/article/S2352396424001166>.
 Home-page: https://github.com/Juillermo/ABC.git
 Author: Guillermo Romero Moreno
 Author-email: Guillermo.RomeroMoreno@ed.ac.uk
 License: GNU GENERAL PUBLIC LICENSE
 Keywords: Bayesian,Multimorbidity
 Classifier: Programming Language :: Python :: 3
@@ -55,15 +55,15 @@
 
 - Install [Anaconda](https://docs.anaconda.com/) (if not already installed)  
 - Execute `conda env create -n ABC --file packages.yml`* in a terminal for creating an environment called `ABC` with all the required packages. *Be aware that it may take a few GB of space.*
 - Activate the environment with `conda activate ABC`, and run the code or set up a jupyter notebook server (by running `jupyter notebook`)
 
 > .* Or you can directly execute `conda create -n ABC -c conda-forge numpy=1.22.3 scipy=1.8.0 pandas=1.4.2 matplotlib=3.5.1 seaborn=0.13.1 networkx=2.8 bokeh=3.3.0 cmdstanpy=1.1.0 jupyter`.
 
-While the code is in *python*, Bayesian inference is performed via [Stan](http://mc-stan.org) through the package `cmdstanpy` (version 1.1.0), providing a python API to the *Stan* library. The model (defined in the file [`models/MLTC_atomic_hyp_mult.stan`](models/MLTC_atomic_hyp_mult.stan)) could also work with [any stan interface](https://mc-stan.org/users/interfaces/index.html).
+While the code is in *python*, Bayesian inference is performed via [Stan](http://mc-stan.org) through the package `cmdstanpy` (version 1.1.0), providing a python API to the *Stan* library. The model (defined in the file [`ABC/models/MLTC_atomic_hyp_mult.stan`](ABC/models/MLTC_atomic_hyp_mult.stan)) could also work with [any stan interface](https://mc-stan.org/users/interfaces/index.html).
 
 ## Using the model
 
 Our model can be used simply by running `ABC "path/to/dataset_file.csv"`, which will fit the model and generate output files with the results. For more information on additional argumnets, run `ABC --help`.
 
 Additionally, you can integrate our model into other *python* code directly. You can see an example snippet on how to do so below.
 
@@ -93,16 +93,16 @@
 
 You can still reproduce the results shown in that notebook on a different dataset, for which you will need to adapt all functions and variables within the file [`ABC/data.py`](ABC/data.py) to your dataset characteristics and then rerun [`notebooks/results.ipynb`](notebooks/results.ipynb) --- or use the functions in the file [`ABC/results.py`](ABC/results.py).
 
 
 ## Repository structure
 
 * [`ABC/`](ABC/): python files with the basic classes and functions.
-* [`models/`](models/): files defining *Stan* models.
-* [`output/`](output/): folder in which to save the fitted models.
+* [`ABC/models/`](ABC/models/): files defining *Stan* models.
+* [`ABC/output/`](ABC/output/): folder in which to save the fitted models.
 * [`notebooks/`](notebooks/): results and examples implementing our models and code.
 * [`figs/`](figs/): folder in which to save the figures produced in the notebooks.
 
 
 ## Acknowledgements
 
 Functions and notebooks were inspired by [this repository](https://github.com/jg-you/plant-pollinator-inference/tree/master).
```

### Comparing `abc_network-0.1.0/README.md` & `abc_network-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 - Install [Anaconda](https://docs.anaconda.com/) (if not already installed)  
 - Execute `conda env create -n ABC --file packages.yml`* in a terminal for creating an environment called `ABC` with all the required packages. *Be aware that it may take a few GB of space.*
 - Activate the environment with `conda activate ABC`, and run the code or set up a jupyter notebook server (by running `jupyter notebook`)
 
 > .* Or you can directly execute `conda create -n ABC -c conda-forge numpy=1.22.3 scipy=1.8.0 pandas=1.4.2 matplotlib=3.5.1 seaborn=0.13.1 networkx=2.8 bokeh=3.3.0 cmdstanpy=1.1.0 jupyter`.
 
-While the code is in *python*, Bayesian inference is performed via [Stan](http://mc-stan.org) through the package `cmdstanpy` (version 1.1.0), providing a python API to the *Stan* library. The model (defined in the file [`models/MLTC_atomic_hyp_mult.stan`](models/MLTC_atomic_hyp_mult.stan)) could also work with [any stan interface](https://mc-stan.org/users/interfaces/index.html).
+While the code is in *python*, Bayesian inference is performed via [Stan](http://mc-stan.org) through the package `cmdstanpy` (version 1.1.0), providing a python API to the *Stan* library. The model (defined in the file [`ABC/models/MLTC_atomic_hyp_mult.stan`](ABC/models/MLTC_atomic_hyp_mult.stan)) could also work with [any stan interface](https://mc-stan.org/users/interfaces/index.html).
 
 ## Using the model
 
 Our model can be used simply by running `ABC "path/to/dataset_file.csv"`, which will fit the model and generate output files with the results. For more information on additional argumnets, run `ABC --help`.
 
 Additionally, you can integrate our model into other *python* code directly. You can see an example snippet on how to do so below.
 
@@ -69,16 +69,16 @@
 
 You can still reproduce the results shown in that notebook on a different dataset, for which you will need to adapt all functions and variables within the file [`ABC/data.py`](ABC/data.py) to your dataset characteristics and then rerun [`notebooks/results.ipynb`](notebooks/results.ipynb) --- or use the functions in the file [`ABC/results.py`](ABC/results.py).
 
 
 ## Repository structure
 
 * [`ABC/`](ABC/): python files with the basic classes and functions.
-* [`models/`](models/): files defining *Stan* models.
-* [`output/`](output/): folder in which to save the fitted models.
+* [`ABC/models/`](ABC/models/): files defining *Stan* models.
+* [`ABC/output/`](ABC/output/): folder in which to save the fitted models.
 * [`notebooks/`](notebooks/): results and examples implementing our models and code.
 * [`figs/`](figs/): folder in which to save the figures produced in the notebooks.
 
 
 ## Acknowledgements
 
 Functions and notebooks were inspired by [this repository](https://github.com/jg-you/plant-pollinator-inference/tree/master).
```

### Comparing `abc_network-0.1.0/abc_network.egg-info/PKG-INFO` & `abc_network-0.1.1/abc_network.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abc_network
-Version: 0.1.0
+Version: 0.1.1
 Summary: This package provides code linked to the paper "Multimorbidity analysis with low condition counts: a robust Bayesian approach for small but important subgroups" <https://authors.elsevier.com/sd/article/S2352396424001166>.
 Home-page: https://github.com/Juillermo/ABC.git
 Author: Guillermo Romero Moreno
 Author-email: Guillermo.RomeroMoreno@ed.ac.uk
 License: GNU GENERAL PUBLIC LICENSE
 Keywords: Bayesian,Multimorbidity
 Classifier: Programming Language :: Python :: 3
@@ -55,15 +55,15 @@
 
 - Install [Anaconda](https://docs.anaconda.com/) (if not already installed)  
 - Execute `conda env create -n ABC --file packages.yml`* in a terminal for creating an environment called `ABC` with all the required packages. *Be aware that it may take a few GB of space.*
 - Activate the environment with `conda activate ABC`, and run the code or set up a jupyter notebook server (by running `jupyter notebook`)
 
 > .* Or you can directly execute `conda create -n ABC -c conda-forge numpy=1.22.3 scipy=1.8.0 pandas=1.4.2 matplotlib=3.5.1 seaborn=0.13.1 networkx=2.8 bokeh=3.3.0 cmdstanpy=1.1.0 jupyter`.
 
-While the code is in *python*, Bayesian inference is performed via [Stan](http://mc-stan.org) through the package `cmdstanpy` (version 1.1.0), providing a python API to the *Stan* library. The model (defined in the file [`models/MLTC_atomic_hyp_mult.stan`](models/MLTC_atomic_hyp_mult.stan)) could also work with [any stan interface](https://mc-stan.org/users/interfaces/index.html).
+While the code is in *python*, Bayesian inference is performed via [Stan](http://mc-stan.org) through the package `cmdstanpy` (version 1.1.0), providing a python API to the *Stan* library. The model (defined in the file [`ABC/models/MLTC_atomic_hyp_mult.stan`](ABC/models/MLTC_atomic_hyp_mult.stan)) could also work with [any stan interface](https://mc-stan.org/users/interfaces/index.html).
 
 ## Using the model
 
 Our model can be used simply by running `ABC "path/to/dataset_file.csv"`, which will fit the model and generate output files with the results. For more information on additional argumnets, run `ABC --help`.
 
 Additionally, you can integrate our model into other *python* code directly. You can see an example snippet on how to do so below.
 
@@ -93,16 +93,16 @@
 
 You can still reproduce the results shown in that notebook on a different dataset, for which you will need to adapt all functions and variables within the file [`ABC/data.py`](ABC/data.py) to your dataset characteristics and then rerun [`notebooks/results.ipynb`](notebooks/results.ipynb) --- or use the functions in the file [`ABC/results.py`](ABC/results.py).
 
 
 ## Repository structure
 
 * [`ABC/`](ABC/): python files with the basic classes and functions.
-* [`models/`](models/): files defining *Stan* models.
-* [`output/`](output/): folder in which to save the fitted models.
+* [`ABC/models/`](ABC/models/): files defining *Stan* models.
+* [`ABC/output/`](ABC/output/): folder in which to save the fitted models.
 * [`notebooks/`](notebooks/): results and examples implementing our models and code.
 * [`figs/`](figs/): folder in which to save the figures produced in the notebooks.
 
 
 ## Acknowledgements
 
 Functions and notebooks were inspired by [this repository](https://github.com/jg-you/plant-pollinator-inference/tree/master).
```

### Comparing `abc_network-0.1.0/setup.cfg` & `abc_network-0.1.1/setup.cfg`

 * *Files identical despite different names*

