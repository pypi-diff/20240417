# Comparing `tmp/autora-experimentalist-falsification-2.0.1.tar.gz` & `tmp/autora-experimentalist-falsification-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-experimentalist-falsification-2.0.1.tar", last modified: Wed Nov  8 15:04:34 2023, max compression
+gzip compressed data, was "autora-experimentalist-falsification-2.0.2.tar", last modified: Wed Nov 29 16:17:23 2023, max compression
```

## Comparing `autora-experimentalist-falsification-2.0.1.tar` & `autora-experimentalist-falsification-2.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 15:04:34.005839 autora-experimentalist-falsification-2.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 15:04:33.997839 autora-experimentalist-falsification-2.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 15:04:34.001839 autora-experimentalist-falsification-2.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-11-08 15:04:23.000000 autora-experimentalist-falsification-2.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      781 2023-11-08 15:04:23.000000 autora-experimentalist-falsification-2.0.1/.github/workflows/test-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (127)      959 2023-11-08 15:04:23.000000 autora-experimentalist-falsification-2.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      674 2023-11-08 15:04:23.000000 autora-experimentalist-falsification-2.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2023-11-08 15:04:23.000000 autora-experimentalist-falsification-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2023-11-08 15:04:34.005839 autora-experimentalist-falsification-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      918 2023-11-08 15:04:23.000000 autora-experimentalist-falsification-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 15:04:34.001839 autora-experimentalist-falsification-2.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)   352623 2023-11-08 15:04:23.000000 autora-experimentalist-falsification-2.0.1/docs/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2023-11-08 15:04:23.000000 autora-experimentalist-falsification-2.0.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 15:04:34.001839 autora-experimentalist-falsification-2.0.1/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2023-11-08 15:04:23.000000 autora-experimentalist-falsification-2.0.1/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (127)    58500 2023-11-08 15:04:23.000000 autora-experimentalist-falsification-2.0.1/docs/model-vs-data.png
--rw-r--r--   0 runner    (1001) docker     (127)    60582 2023-11-08 15:04:23.000000 autora-experimentalist-falsification-2.0.1/docs/mse.png
--rw-r--r--   0 runner    (1001) docker     (127)      404 2023-11-08 15:04:23.000000 autora-experimentalist-falsification-2.0.1/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 15:04:34.001839 autora-experimentalist-falsification-2.0.1/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2023-11-08 15:04:23.000000 autora-experimentalist-falsification-2.0.1/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (127)      418 2023-11-08 15:04:23.000000 autora-experimentalist-falsification-2.0.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      781 2023-11-08 15:04:23.000000 autora-experimentalist-falsification-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-08 15:04:34.005839 autora-experimentalist-falsification-2.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 15:04:33.997839 autora-experimentalist-falsification-2.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 15:04:33.997839 autora-experimentalist-falsification-2.0.1/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 15:04:33.997839 autora-experimentalist-falsification-2.0.1/src/autora/experimentalist/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 15:04:34.005839 autora-experimentalist-falsification-2.0.1/src/autora/experimentalist/falsification/
--rw-r--r--   0 runner    (1001) docker     (127)    19288 2023-11-08 15:04:23.000000 autora-experimentalist-falsification-2.0.1/src/autora/experimentalist/falsification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7245 2023-11-08 15:04:23.000000 autora-experimentalist-falsification-2.0.1/src/autora/experimentalist/falsification/popper_net.py
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2023-11-08 15:04:23.000000 autora-experimentalist-falsification-2.0.1/src/autora/experimentalist/falsification/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 15:04:34.005839 autora-experimentalist-falsification-2.0.1/src/autora_experimentalist_falsification.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2023-11-08 15:04:33.000000 autora-experimentalist-falsification-2.0.1/src/autora_experimentalist_falsification.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      875 2023-11-08 15:04:33.000000 autora-experimentalist-falsification-2.0.1/src/autora_experimentalist_falsification.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-08 15:04:33.000000 autora-experimentalist-falsification-2.0.1/src/autora_experimentalist_falsification.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-11-08 15:04:33.000000 autora-experimentalist-falsification-2.0.1/src/autora_experimentalist_falsification.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-08 15:04:33.000000 autora-experimentalist-falsification-2.0.1/src/autora_experimentalist_falsification.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 15:04:34.005839 autora-experimentalist-falsification-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2023-11-08 15:04:23.000000 autora-experimentalist-falsification-2.0.1/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-08 15:04:23.000000 autora-experimentalist-falsification-2.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6930 2023-11-08 15:04:23.000000 autora-experimentalist-falsification-2.0.1/tests/test_exp_falsification_pooler.py
--rw-r--r--   0 runner    (1001) docker     (127)    13665 2023-11-08 15:04:23.000000 autora-experimentalist-falsification-2.0.1/tests/test_exp_falsification_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 16:17:23.540901 autora-experimentalist-falsification-2.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 16:17:23.532901 autora-experimentalist-falsification-2.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 16:17:23.532901 autora-experimentalist-falsification-2.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-11-29 16:17:10.000000 autora-experimentalist-falsification-2.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2023-11-29 16:17:10.000000 autora-experimentalist-falsification-2.0.2/.github/workflows/test-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2023-11-29 16:17:10.000000 autora-experimentalist-falsification-2.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2023-11-29 16:17:10.000000 autora-experimentalist-falsification-2.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2023-11-29 16:17:10.000000 autora-experimentalist-falsification-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2023-11-29 16:17:23.540901 autora-experimentalist-falsification-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2023-11-29 16:17:10.000000 autora-experimentalist-falsification-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 16:17:23.536901 autora-experimentalist-falsification-2.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)   352623 2023-11-29 16:17:10.000000 autora-experimentalist-falsification-2.0.2/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2023-11-29 16:17:10.000000 autora-experimentalist-falsification-2.0.2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 16:17:23.536901 autora-experimentalist-falsification-2.0.2/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2023-11-29 16:17:10.000000 autora-experimentalist-falsification-2.0.2/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (127)    58500 2023-11-29 16:17:10.000000 autora-experimentalist-falsification-2.0.2/docs/model-vs-data.png
+-rw-r--r--   0 runner    (1001) docker     (127)    60582 2023-11-29 16:17:10.000000 autora-experimentalist-falsification-2.0.2/docs/mse.png
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2023-11-29 16:17:10.000000 autora-experimentalist-falsification-2.0.2/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 16:17:23.536901 autora-experimentalist-falsification-2.0.2/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2023-11-29 16:17:10.000000 autora-experimentalist-falsification-2.0.2/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2023-11-29 16:17:10.000000 autora-experimentalist-falsification-2.0.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2023-11-29 16:17:10.000000 autora-experimentalist-falsification-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-29 16:17:23.540901 autora-experimentalist-falsification-2.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 16:17:23.532901 autora-experimentalist-falsification-2.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 16:17:23.532901 autora-experimentalist-falsification-2.0.2/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 16:17:23.532901 autora-experimentalist-falsification-2.0.2/src/autora/experimentalist/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 16:17:23.536901 autora-experimentalist-falsification-2.0.2/src/autora/experimentalist/falsification/
+-rw-r--r--   0 runner    (1001) docker     (127)    19290 2023-11-29 16:17:10.000000 autora-experimentalist-falsification-2.0.2/src/autora/experimentalist/falsification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7245 2023-11-29 16:17:10.000000 autora-experimentalist-falsification-2.0.2/src/autora/experimentalist/falsification/popper_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2023-11-29 16:17:10.000000 autora-experimentalist-falsification-2.0.2/src/autora/experimentalist/falsification/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 16:17:23.536901 autora-experimentalist-falsification-2.0.2/src/autora_experimentalist_falsification.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2023-11-29 16:17:23.000000 autora-experimentalist-falsification-2.0.2/src/autora_experimentalist_falsification.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2023-11-29 16:17:23.000000 autora-experimentalist-falsification-2.0.2/src/autora_experimentalist_falsification.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-29 16:17:23.000000 autora-experimentalist-falsification-2.0.2/src/autora_experimentalist_falsification.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2023-11-29 16:17:23.000000 autora-experimentalist-falsification-2.0.2/src/autora_experimentalist_falsification.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-29 16:17:23.000000 autora-experimentalist-falsification-2.0.2/src/autora_experimentalist_falsification.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 16:17:23.536901 autora-experimentalist-falsification-2.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2023-11-29 16:17:10.000000 autora-experimentalist-falsification-2.0.2/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 16:17:10.000000 autora-experimentalist-falsification-2.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6930 2023-11-29 16:17:10.000000 autora-experimentalist-falsification-2.0.2/tests/test_exp_falsification_pooler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13626 2023-11-29 16:17:10.000000 autora-experimentalist-falsification-2.0.2/tests/test_exp_falsification_sampler.py
```

### Comparing `autora-experimentalist-falsification-2.0.1/.github/workflows/python-publish.yml` & `autora-experimentalist-falsification-2.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-2.0.1/.github/workflows/test-pytest.yml` & `autora-experimentalist-falsification-2.0.2/.github/workflows/test-pytest.yml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-2.0.1/.gitignore` & `autora-experimentalist-falsification-2.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-2.0.1/LICENSE` & `autora-experimentalist-falsification-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-2.0.1/PKG-INFO` & `autora-experimentalist-falsification-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-falsification
-Version: 2.0.1
+Version: 2.0.2
 Summary: AutoRA Falsification Experimentalist
 Author-email: Sebastian Musslick <sebastian@musslick.de>
 License: MIT License
         
         Copyright (c) 2023 Autonomous Empirical Research Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -60,9 +60,9 @@
 ```shell
 pip install -U autora["experimentalist-falsification"]
 ```
 
 
 Check your installation by running:
 ```shell
-python -c "from autora.experimentalist.pooler.falsification import falsification_pool"
+python -c "from autora.experimentalist.falsification import falsification_pool"
 ```
```

### Comparing `autora-experimentalist-falsification-2.0.1/README.md` & `autora-experimentalist-falsification-2.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,9 +22,9 @@
 ```shell
 pip install -U autora["experimentalist-falsification"]
 ```
 
 
 Check your installation by running:
 ```shell
-python -c "from autora.experimentalist.pooler.falsification import falsification_pool"
+python -c "from autora.experimentalist.falsification import falsification_pool"
 ```
```

### Comparing `autora-experimentalist-falsification-2.0.1/docs/Basic Usage.ipynb` & `autora-experimentalist-falsification-2.0.2/docs/Basic Usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-2.0.1/docs/index.md` & `autora-experimentalist-falsification-2.0.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-2.0.1/docs/model-vs-data.png` & `autora-experimentalist-falsification-2.0.2/docs/model-vs-data.png`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-2.0.1/docs/mse.png` & `autora-experimentalist-falsification-2.0.2/docs/mse.png`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-2.0.1/mkdocs/base.yml` & `autora-experimentalist-falsification-2.0.2/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-2.0.1/pyproject.toml` & `autora-experimentalist-falsification-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-2.0.1/src/autora/experimentalist/falsification/__init__.py` & `autora-experimentalist-falsification-2.0.2/src/autora/experimentalist/falsification/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -408,11 +408,11 @@
     return sorted_conditions[0:num_samples], sorted_score[0:num_samples]
 
 falsification_pool = pool
 falsification_pool.__doc__ = """Alias for pool"""
 falsification_pooler = deprecated_alias(falsification_pool, "falsification_pooler")
 
 falsification_sample = sample
-falsification_pool.__doc__ = """Alias for pool"""
+falsification_pool.__doc__ = """Alias for sample"""
 falsification_sampler = deprecated_alias(falsification_sample, "falsification_sampler")
 falsification_score_sampler = deprecated_alias(falsification_score_sample, "falsification_score_sampler")
 falsification_score_sampler_from_predictions = deprecated_alias(falsification_score_sample_from_predictions, "falsification_score_sampler_from_predictions")
```

### Comparing `autora-experimentalist-falsification-2.0.1/src/autora/experimentalist/falsification/popper_net.py` & `autora-experimentalist-falsification-2.0.2/src/autora/experimentalist/falsification/popper_net.py`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-2.0.1/src/autora/experimentalist/falsification/utils.py` & `autora-experimentalist-falsification-2.0.2/src/autora/experimentalist/falsification/utils.py`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-2.0.1/src/autora_experimentalist_falsification.egg-info/PKG-INFO` & `autora-experimentalist-falsification-2.0.2/src/autora_experimentalist_falsification.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-falsification
-Version: 2.0.1
+Version: 2.0.2
 Summary: AutoRA Falsification Experimentalist
 Author-email: Sebastian Musslick <sebastian@musslick.de>
 License: MIT License
         
         Copyright (c) 2023 Autonomous Empirical Research Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -60,9 +60,9 @@
 ```shell
 pip install -U autora["experimentalist-falsification"]
 ```
 
 
 Check your installation by running:
 ```shell
-python -c "from autora.experimentalist.pooler.falsification import falsification_pool"
+python -c "from autora.experimentalist.falsification import falsification_pool"
 ```
```

### Comparing `autora-experimentalist-falsification-2.0.1/src/autora_experimentalist_falsification.egg-info/SOURCES.txt` & `autora-experimentalist-falsification-2.0.2/src/autora_experimentalist_falsification.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-2.0.1/tests/README.md` & `autora-experimentalist-falsification-2.0.2/tests/README.md`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-2.0.1/tests/test_exp_falsification_pooler.py` & `autora-experimentalist-falsification-2.0.2/tests/test_exp_falsification_pooler.py`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-2.0.1/tests/test_exp_falsification_sampler.py` & `autora-experimentalist-falsification-2.0.2/tests/test_exp_falsification_sampler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import pandas as pd
 import pytest
 import torch
 from sklearn.linear_model import LinearRegression, LogisticRegression
 
 from autora.experimentalist.pipeline import Pipeline
-from autora.experimentalist.pooler.grid import grid_pool
+from autora.experimentalist.grid import pool
 from autora.experimentalist.falsification import (
     falsification_sample,
     falsification_score_sample,
     falsification_score_sample_from_predictions,
 )
 from autora.variable import DV, IV, ValueType, VariableCollection
 from tests.test_exp_falsification_pooler import get_sin_data, get_xor_data
@@ -305,15 +305,15 @@
 
     # Variable collection with ivs and dvs
     metadata = VariableCollection(
         independent_variables=[iv],
         dependent_variables=[dv],
     )
 
-    X = grid_pool(metadata.independent_variables)
+    X = pool(metadata)
 
     new_conditions = falsification_sample(
                 conditions=X,
                 model=model,
                 reference_conditions=X_train,
                 reference_observations=Y_train,
                 metadata=metadata,
```

