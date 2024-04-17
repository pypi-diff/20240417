# Comparing `tmp/PyMARE-0.0.4rc2.tar.gz` & `tmp/PyMARE-0.0.4rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyMARE-0.0.4rc2.tar", last modified: Sun Jun 12 22:49:22 2022, max compression
+gzip compressed data, was "PyMARE-0.0.4rc6.tar", last modified: Wed Apr 17 19:03:33 2024, max compression
```

## Comparing `PyMARE-0.0.4rc2.tar` & `PyMARE-0.0.4rc6.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 22:49:22.000000 PyMARE-0.0.4rc2/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-06-12 22:49:14.000000 PyMARE-0.0.4rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1543 2022-06-12 22:49:22.000000 PyMARE-0.0.4rc2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 22:49:22.000000 PyMARE-0.0.4rc2/PyMARE.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1543 2022-06-12 22:49:22.000000 PyMARE-0.0.4rc2/PyMARE.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-06-12 22:49:22.000000 PyMARE-0.0.4rc2/PyMARE.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-12 22:49:22.000000 PyMARE-0.0.4rc2/PyMARE.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-12 22:49:22.000000 PyMARE-0.0.4rc2/PyMARE.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-06-12 22:49:22.000000 PyMARE-0.0.4rc2/PyMARE.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-06-12 22:49:22.000000 PyMARE-0.0.4rc2/PyMARE.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3300 2022-06-12 22:49:14.000000 PyMARE-0.0.4rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 22:49:22.000000 PyMARE-0.0.4rc2/pymare/
--rw-r--r--   0 runner    (1001) docker     (121)      394 2022-06-12 22:49:14.000000 PyMARE-0.0.4rc2/pymare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      500 2022-06-12 22:49:22.000000 PyMARE-0.0.4rc2/pymare/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     9901 2022-06-12 22:49:14.000000 PyMARE-0.0.4rc2/pymare/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 22:49:22.000000 PyMARE-0.0.4rc2/pymare/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-06-12 22:49:14.000000 PyMARE-0.0.4rc2/pymare/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2010 2022-06-12 22:49:14.000000 PyMARE-0.0.4rc2/pymare/datasets/metadat.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 22:49:22.000000 PyMARE-0.0.4rc2/pymare/effectsize/
--rw-r--r--   0 runner    (1001) docker     (121)      416 2022-06-12 22:49:14.000000 PyMARE-0.0.4rc2/pymare/effectsize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21690 2022-06-12 22:49:14.000000 PyMARE-0.0.4rc2/pymare/effectsize/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2688 2022-06-12 22:49:14.000000 PyMARE-0.0.4rc2/pymare/effectsize/expressions.json
--rw-r--r--   0 runner    (1001) docker     (121)     4372 2022-06-12 22:49:14.000000 PyMARE-0.0.4rc2/pymare/effectsize/expressions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 22:49:22.000000 PyMARE-0.0.4rc2/pymare/estimators/
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-06-12 22:49:14.000000 PyMARE-0.0.4rc2/pymare/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7326 2022-06-12 22:49:14.000000 PyMARE-0.0.4rc2/pymare/estimators/combination.py
--rw-r--r--   0 runner    (1001) docker     (121)    23304 2022-06-12 22:49:14.000000 PyMARE-0.0.4rc2/pymare/estimators/estimators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 22:49:22.000000 PyMARE-0.0.4rc2/pymare/resources/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-12 22:49:22.000000 PyMARE-0.0.4rc2/pymare/resources/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)     2198 2022-06-12 22:49:14.000000 PyMARE-0.0.4rc2/pymare/resources/datasets/michael2013.json
--rw-r--r--   0 runner    (1001) docker     (121)     1837 2022-06-12 22:49:14.000000 PyMARE-0.0.4rc2/pymare/resources/datasets/michael2013.tsv
--rw-r--r--   0 runner    (1001) docker     (121)    22188 2022-06-12 22:49:14.000000 PyMARE-0.0.4rc2/pymare/results.py
--rw-r--r--   0 runner    (1001) docker     (121)     6945 2022-06-12 22:49:14.000000 PyMARE-0.0.4rc2/pymare/stats.py
--rw-r--r--   0 runner    (1001) docker     (121)     1864 2022-06-12 22:49:14.000000 PyMARE-0.0.4rc2/pymare/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      452 2022-06-12 22:49:14.000000 PyMARE-0.0.4rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2256 2022-06-12 22:49:22.000000 PyMARE-0.0.4rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-06-12 22:49:14.000000 PyMARE-0.0.4rc2/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    79886 2022-06-12 22:49:14.000000 PyMARE-0.0.4rc2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:03:33.086545 PyMARE-0.0.4rc6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-17 19:03:33.086545 PyMARE-0.0.4rc6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:03:33.082545 PyMARE-0.0.4rc6/PyMARE.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-17 19:03:33.000000 PyMARE-0.0.4rc6/PyMARE.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-17 19:03:33.000000 PyMARE-0.0.4rc6/PyMARE.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 19:03:33.000000 PyMARE-0.0.4rc6/PyMARE.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 19:03:33.000000 PyMARE-0.0.4rc6/PyMARE.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-17 19:03:33.000000 PyMARE-0.0.4rc6/PyMARE.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 19:03:33.000000 PyMARE-0.0.4rc6/PyMARE.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:03:33.086545 PyMARE-0.0.4rc6/pymare/
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-17 19:03:33.086545 PyMARE-0.0.4rc6/pymare/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9900 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:03:33.082545 PyMARE-0.0.4rc6/pymare/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/datasets/metadat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:03:33.086545 PyMARE-0.0.4rc6/pymare/effectsize/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/effectsize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21695 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/effectsize/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/effectsize/expressions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/effectsize/expressions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:03:33.086545 PyMARE-0.0.4rc6/pymare/estimators/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9532 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/estimators/combination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23611 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/estimators/estimators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:03:33.082545 PyMARE-0.0.4rc6/pymare/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:03:33.086545 PyMARE-0.0.4rc6/pymare/resources/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/resources/datasets/michael2013.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/resources/datasets/michael2013.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)    22187 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pymare/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-17 19:03:33.086545 PyMARE-0.0.4rc6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79886 2024-04-17 19:03:25.000000 PyMARE-0.0.4rc6/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `PyMARE-0.0.4rc2/PKG-INFO` & `PyMARE-0.0.4rc6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMARE
-Version: 0.0.4rc2
+Version: 0.0.4rc6
 Summary: PyMARE: Python Meta-Analysis & Regression Engine
 Home-page: https://github.com/neurostuff/PyMARE
 Author: PyMARE developers
 Author-email: tsalo006@fiu.edu
 Maintainer: Taylor Salo
 Maintainer-email: tsalo006@fiu.edu
 License: MIT
@@ -24,18 +24,18 @@
         Copyright (c) 2019--, PyMARE developers
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: doc
 Provides-Extra: tests
 Provides-Extra: stan
 Provides-Extra: all
```

### Comparing `PyMARE-0.0.4rc2/PyMARE.egg-info/PKG-INFO` & `PyMARE-0.0.4rc6/PyMARE.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMARE
-Version: 0.0.4rc2
+Version: 0.0.4rc6
 Summary: PyMARE: Python Meta-Analysis & Regression Engine
 Home-page: https://github.com/neurostuff/PyMARE
 Author: PyMARE developers
 Author-email: tsalo006@fiu.edu
 Maintainer: Taylor Salo
 Maintainer-email: tsalo006@fiu.edu
 License: MIT
@@ -24,18 +24,18 @@
         Copyright (c) 2019--, PyMARE developers
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: doc
 Provides-Extra: tests
 Provides-Extra: stan
 Provides-Extra: all
```

### Comparing `PyMARE-0.0.4rc2/PyMARE.egg-info/SOURCES.txt` & `PyMARE-0.0.4rc6/PyMARE.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 versioneer.py
 PyMARE.egg-info/PKG-INFO
```

### Comparing `PyMARE-0.0.4rc2/PyMARE.egg-info/requires.txt` & `PyMARE-0.0.4rc6/PyMARE.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 numpy>=1.8.0
 pandas
-scipy
+scipy<1.13.0
 sympy
 wrapt
 
 [all]
 m2r
 matplotlib
 mistune<2
 numpydoc
 pillow
 recommonmark
 seaborn
 sphinx>=3.5
 sphinx-argparse
 sphinx-copybutton
-sphinx_gallery==0.10.1
+sphinx_gallery
 sphinx_rtd_theme
 sphinxcontrib-bibtex
 codecov
 coverage
 coveralls
 flake8
 flake8-black
 flake8-docstrings
 flake8-isort
 pytest
 pytest-cov
+pystan
+arviz
 
 [doc]
 m2r
 matplotlib
 mistune<2
 numpydoc
 pillow
 recommonmark
 seaborn
 sphinx>=3.5
 sphinx-argparse
 sphinx-copybutton
-sphinx_gallery==0.10.1
+sphinx_gallery
 sphinx_rtd_theme
 sphinxcontrib-bibtex
 
 [stan]
 pystan
 arviz
```

### Comparing `PyMARE-0.0.4rc2/README.md` & `PyMARE-0.0.4rc6/README.md`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.4rc2/pymare/core.py` & `PyMARE-0.0.4rc6/pymare/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,14 @@
         If False, the predictors matrix is passed as-is to estimators.
         Default = True.
     """
 
     def __init__(
         self, y=None, v=None, X=None, n=None, data=None, X_names=None, add_intercept=True
     ):
-
         if y is None and data is None:
             raise ValueError(
                 "If no y values are provided, a pandas DataFrame "
                 "containing a 'y' column must be passed to the "
                 "data argument."
             )
```

### Comparing `PyMARE-0.0.4rc2/pymare/datasets/metadat.py` & `PyMARE-0.0.4rc6/pymare/datasets/metadat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Datasets from metadat."""
+
 import json
 import os.path as op
 
 import pandas as pd
 
 from pymare.utils import get_resource_path
```

### Comparing `PyMARE-0.0.4rc2/pymare/effectsize/base.py` & `PyMARE-0.0.4rc6/pymare/effectsize/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     solutions = solve(system, symbols)
 
     if not solutions:
         return {}
 
     # solver will return a dict if there's only one non-dummy expression
     if isinstance(solutions, dict):
-        solutions = [list(solutions.values())]
+        solutions = [[solutions[s] for s in symbols]]
 
     # Prepare the dummy list and data args in a fixed order
     dummy_list = list(dummies)
     data_args = [known_vars[var.name.strip("_")] for var in dummy_list]
 
     # Compute any solved vars via numpy and store in new dict
     results = {}
@@ -86,15 +86,14 @@
     return results
 
 
 class EffectSizeConverter(metaclass=ABCMeta):
     """Base class for effect size converters."""
 
     def __init__(self, data=None, **kwargs):
-
         kwargs = {k: v for k, v in kwargs.items() if v is not None}
 
         if data is not None:
             kwargs = self._collect_variables(data, kwargs)
 
         # Do any subclass-specific validation
         kwargs = self._validate(kwargs)
@@ -505,15 +504,14 @@
     if measure not in valid_measures:
         raise ValueError(
             "Invalid measures '{}'; must be one of {}.".format(measure, valid_measures)
         )
 
     # Select or infer converter class
     if comparison == "infer":
-
         one_samp_inputs = {"m", "sd", "n", "r"}
         two_samp_inputs = {"m1", "m2", "sd1", "sd2", "n1", "n2"}
 
         if measure in {"RM", "SM", "R", "ZR"}:
             comparison = 1
         elif measure in {"RMD", "SMD"}:
             comparison = 2
```

### Comparing `PyMARE-0.0.4rc2/pymare/effectsize/expressions.json` & `PyMARE-0.0.4rc6/pymare/effectsize/expressions.json`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.4rc2/pymare/effectsize/expressions.py` & `PyMARE-0.0.4rc6/pymare/effectsize/expressions.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Statistical expressions."""
+
 import json
 from collections import defaultdict
 from itertools import chain
 from pathlib import Path
 
 from sympy import Symbol, sympify
 
@@ -86,15 +87,14 @@
                 exp_dict[sym.name].append(exp)
 
     def df_search(sym, exprs, known, visited):
         """Recursively select expressions needed to solve for sym."""
         results = []
 
         for exp in exp_dict[sym]:
-
             candidates = []
 
             sym_names = set(s.name for s in exp.symbols)
 
             # Abort if we're cycling
             if visited & sym_names:
                 continue
```

### Comparing `PyMARE-0.0.4rc2/pymare/estimators/__init__.py` & `PyMARE-0.0.4rc6/pymare/estimators/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Estimators for meta-analyses and meta-regressions."""
+
 from .combination import FisherCombinationTest, StoufferCombinationTest
 from .estimators import (
     DerSimonianLaird,
     Hedges,
     SampleSizeBasedLikelihoodEstimator,
     StanMetaRegression,
     VarianceBasedLikelihoodEstimator,
```

### Comparing `PyMARE-0.0.4rc2/pymare/estimators/combination.py` & `PyMARE-0.0.4rc6/pymare/estimators/combination.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Estimators for combination (p/z) tests."""
+
 import warnings
 from abc import abstractmethod
 
 import numpy as np
 import scipy.stats as ss
 
 from ..results import CombinationTestResults
@@ -106,25 +107,85 @@
 
     References
     ----------
     .. footbibliography::
     """
 
     # Maps Dataset attributes onto fit() args; see BaseEstimator for details.
-    _dataset_attr_map = {"z": "y", "w": "v"}
+    _dataset_attr_map = {"z": "y", "w": "n", "g": "v"}
+
+    def _inflation_term(self, z, w, g):
+        """Calculate the variance inflation term for each group.
+
+        This term is used to adjust the variance of the combined z-score when
+        multiple sample come from the same study.
 
-    def fit(self, z, w=None):
-        """Fit the estimator to z-values, optionally with weights."""
-        return super().fit(z, w=w)
+        Parameters
+        ----------
+        z : :obj:`numpy.ndarray` of shape (n, d)
+            Array of z-values.
+        w : :obj:`numpy.ndarray` of shape (n, d)
+            Array of weights.
+        g : :obj:`numpy.ndarray` of shape (n, d)
+            Array of group labels.
+
+        Returns
+        -------
+        sigma : float
+            The variance inflation term.
+        """
+        # Only center if the samples are not all the same, to prevent division by zero
+        # when calculating the correlation matrix.
+        # This centering is problematic for N=2
+        all_samples_same = np.all(np.equal(z, z[0]), axis=0).all()
+        z = z if all_samples_same else z - z.mean(0)
+
+        # Use the value from one feature, as all features have the same groups and weights
+        groups = g[:, 0]
+        weights = w[:, 0]
+
+        # Loop over groups
+        unique_groups = np.unique(groups)
+
+        sigma = 0
+        for group in unique_groups:
+            group_indices = np.where(groups == group)[0]
+            group_z = z[group_indices]
+
+            # For groups with only one sample the contribution to the summand is 0
+            n_samples = len(group_indices)
+            if n_samples < 2:
+                continue
+
+            # Calculate the within group correlation matrix and sum the non-diagonal elements
+            corr = np.corrcoef(group_z, rowvar=True)
+            upper_indices = np.triu_indices(n_samples, k=1)
+            non_diag_corr = corr[upper_indices]
+            w_i, w_j = weights[upper_indices[0]], weights[upper_indices[1]]
+
+            sigma += (2 * w_i * w_j * non_diag_corr).sum()
+
+        return sigma
+
+    def fit(self, z, w=None, g=None):
+        """Fit the estimator to z-values, optionally with weights and groups."""
+        return super().fit(z, w=w, g=g)
 
-    def p_value(self, z, w=None):
+    def p_value(self, z, w=None, g=None):
         """Calculate p-values."""
         if w is None:
             w = np.ones_like(z)
-        cz = (z * w).sum(0) / np.sqrt((w**2).sum(0))
+
+        # Calculate the variance inflation term, sum of non-diagonal elements of sigma.
+        sigma = self._inflation_term(z, w, g) if g is not None else 0
+
+        # The sum of diagonal elements of sigma is given by (w**2).sum(0).
+        variance = (w**2).sum(0) + sigma
+
+        cz = (z * w).sum(0) / np.sqrt(variance)
         return ss.norm.sf(cz)
 
 
 class FisherCombinationTest(CombinationTest):
     """Fisher's method for combining p-values.
 
     Takes a set of independent z-scores and combines them via Fisher's
```

### Comparing `PyMARE-0.0.4rc2/pymare/estimators/estimators.py` & `PyMARE-0.0.4rc6/pymare/estimators/estimators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Meta-regression estimator classes."""
 
+import sys
 from abc import ABCMeta, abstractmethod
 from inspect import getfullargspec
 from warnings import warn
 
 import numpy as np
 import wrapt
 from scipy.optimize import Bounds, minimize
@@ -549,37 +550,44 @@
     stan() estimator. The object-oriented interface is useful primarily
     when fitting the meta-regression model repeatedly to different data;
     the separation of .compile() and .fit() steps allows one to compile
     the model only once.
 
     Warning
     -------
-    With changes to Stan in version 3, which requires Python 3.7, this class no longer works for
-    Python 3.7+. We will try to fix it in the future.
+    :obj:`~pymare.estimators.StanMetaRegression` uses Pystan 3, which requires Python 3.7.
+    Pystan 3 should not be used with PyMARE and Python 3.6 or earlier.
     """
 
     _result_cls = BayesianMetaRegressionResults
 
     def __init__(self, **sampling_kwargs):
         self.sampling_kwargs = sampling_kwargs
         self.model = None
         self.result_ = None
 
+        if sys.version_info < (3, 7):
+            raise RuntimeError(
+                "StanMetaRegression uses Pystan 3, which requires python 3.7 or higher. "
+                f"You are running Python {sys.version_info.major}.{sys.version_info.minor}. "
+                "Pystan 3 should not be used with PyMARE and Python 3.6 or earlier."
+            )
+
     def compile(self):
         """Compile the Stan model."""
         # Note: we deliberately use a centered parameterization for the
         # thetas at the moment. This is sub-optimal in terms of estimation,
         # but allows us to avoid having to add extra logic to detect and
         # handle intercepts in X.
         spec = """
         data {
             int<lower=1> N;
             int<lower=1> K;
             vector[N] y;
-            int<lower=1,upper=K> id[N];
+            array[N] int<lower=1,upper=K> id;
             int<lower=1> C;
             matrix[K, C] X;
             vector[N] sigma;
         }
         parameters {
             vector[C] beta;
             vector[K] theta;
@@ -591,21 +599,19 @@
         }
         model {
             y ~ normal(mu, sigma);
             theta ~ normal(0, tau2);
         }
         """
         try:
-            from pystan import StanModel
+            import stan
         except ImportError:
-            raise ImportError(
-                "Please install pystan or, if using Python 3.7+, switch to Python 3.6."
-            )
+            raise ImportError("Please install pystan.")
 
-        self.model = StanModel(model_code=spec)
+        self.model = stan.build(spec, data=self.data)
 
     def fit(self, y, v, X, groups=None):
         """Run the Stan sampler and return results.
 
         Parameters
         ----------
         y : :obj:`numpy.ndarray` of shape (K,)
@@ -641,32 +647,34 @@
         if y.ndim > 1 and y.shape[1] > 1:
             raise ValueError(
                 "The StanMetaRegression estimator currently does "
                 "not support 2-dimensional inputs. Passed y has "
                 "shape {}.".format(y.shape)
             )
 
-        if self.model is None:
-            self.compile()
-
         N = y.shape[0]
         groups = groups or np.arange(1, N + 1, dtype=int)
         K = len(np.unique(groups))
 
         data = {
             "K": K,
             "N": N,
             "id": groups,
             "C": X.shape[1],
             "X": X,
             "y": y.ravel(),
             "sigma": v.ravel(),
         }
 
-        self.result_ = self.model.sampling(data=data, **self.sampling_kwargs)
+        self.data = data
+
+        if self.model is None:
+            self.compile()
+
+        self.result_ = self.model.sample(**self.sampling_kwargs)
         return self
 
     def summary(self, ci=95):
         """Generate a BayesianMetaRegressionResults object from the fitted estimator."""
         if self.result_ is None:
             name = self.__class__.__name__
             raise ValueError(
```

### Comparing `PyMARE-0.0.4rc2/pymare/resources/datasets/michael2013.json` & `PyMARE-0.0.4rc6/pymare/resources/datasets/michael2013.json`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.4rc2/pymare/resources/datasets/michael2013.tsv` & `PyMARE-0.0.4rc6/pymare/resources/datasets/michael2013.tsv`

 * *Files identical despite different names*

### Comparing `PyMARE-0.0.4rc2/pymare/results.py` & `PyMARE-0.0.4rc6/pymare/results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tools for representing and manipulating meta-regression results."""
+
 import itertools
 from functools import lru_cache
 from inspect import getfullargspec
 from warnings import warn
 
 import numpy as np
 import pandas as pd
@@ -327,15 +328,14 @@
 
         exact = n_exact < n_perm
         if exact:
             n_perm = n_exact
 
         # Loop over parallel datasets
         for i in range(n_datasets):
-
             y = self.dataset.y[:, i]
             y_perm = np.repeat(y[:, None], n_perm, axis=1)
 
             # for v, we might actually be working with n, depending on estimator
             has_v = "v" in getfullargspec(self.estimator.fit).args[1:]
             v = self.dataset.v[:, i] if has_v else self.dataset.n[:, i]
 
@@ -467,15 +467,14 @@
             exact = False
 
         # Initialize a copy of the estimator to prevent overwriting results
         est = self.estimator.__class__(mode=self.estimator.mode)
 
         # Loop over parallel datasets
         for i in range(n_datasets):
-
             y = self.dataset.y[:, i]
             y_perm = np.repeat(y[:, None], n_perm, axis=1)
 
             if exact:
                 y_perm *= perms
             else:
                 signs = np.random.choice(np.array([-1, 1]), (n_obs, n_perm))
```

### Comparing `PyMARE-0.0.4rc2/pymare/stats.py` & `PyMARE-0.0.4rc6/pymare/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     # Use the D-L estimate of tau^2 as a starting point; when using a fixed
     # value, minimize() sometimes fails to stay in bounds.
     from .estimators import DerSimonianLaird
 
     ub_start = 2 * DerSimonianLaird().fit(y, v, X).params_["tau2"]
 
     lb = minimize(lambda x: (q_gen(*args, x) - l_crit) ** 2, [0], bounds=bds).x[0]
-    ub = minimize(lambda x: (q_gen(*args, x) - u_crit) ** 2, [ub_start], bounds=bds).x[0]
+    ub = minimize(lambda x: (q_gen(*args, x) - u_crit) ** 2, ub_start, bounds=bds).x[0]
     return {"ci_l": lb, "ci_u": ub}
 
 
 def q_gen(y, v, X, tau2):
     """Calculate a generalized form of Cochran's Q-statistic.
 
     This version of the Q statistic is described in :footcite:t:`veroniki2016methods`.
```

### Comparing `PyMARE-0.0.4rc2/pymare/utils.py` & `PyMARE-0.0.4rc6/pymare/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Miscellaneous utility functions."""
+
 import os.path as op
 
 import numpy as np
 
 
 def get_resource_path():
     """Return the path to general resources, terminated with separator.
```

### Comparing `PyMARE-0.0.4rc2/setup.cfg` & `PyMARE-0.0.4rc6/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 url = https://github.com/neurostuff/PyMARE
 license = MIT
 author = PyMARE developers
 author_email = tsalo006@fiu.edu
 maintainer = Taylor Salo
 maintainer_email = tsalo006@fiu.edu
 description = PyMARE: Python Meta-Analysis & Regression Engine
-description-file = README.md
+description_file = README.md
 long_description = 
 	PyMARE: Python Meta-Analysis & Regression Engine
 	================================================
 	A Python library for mixed-effects meta-regression (including meta-analysis).
 	
 	License
 	=======
@@ -24,26 +24,26 @@
 long_description_content_type = text/x-rst
 classifiers = 
 	Development Status :: 3 - Alpha
 	Environment :: Console
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering
 
 [options]
-python_requires = >= 3.6
+python_requires = >= 3.8
 install_requires = 
 	numpy>=1.8.0
 	pandas
-	scipy
+	scipy<1.13.0  # https://github.com/arviz-devs/arviz/issues/2336
 	sympy
 	wrapt
 packages = find:
 include_package_data = False
 
 [options.extras_require]
 doc = 
@@ -53,15 +53,15 @@
 	numpydoc
 	pillow
 	recommonmark
 	seaborn
 	sphinx>=3.5
 	sphinx-argparse
 	sphinx-copybutton
-	sphinx_gallery==0.10.1
+	sphinx_gallery
 	sphinx_rtd_theme
 	sphinxcontrib-bibtex
 tests = 
 	codecov
 	coverage
 	coveralls
 	flake8
@@ -72,14 +72,15 @@
 	pytest-cov
 stan = 
 	pystan
 	arviz
 all = 
 	%(doc)s
 	%(tests)s
+	%(stan)s
 
 [options.package_data]
 * = 
 	tests/data/*
 	resources/*
 	resources/datasets/*
 	effectsize/*.json
@@ -93,14 +94,16 @@
 parentdir_prefix = 
 
 [flake8]
 max-line-length = 99
 exclude = *build/,_version.py
 putty-ignore = 
 	*/__init__.py : +F401
+per-file-ignores = 
+	*/__init__.py:D401
 ignore = E203,E402,E722,W503
 docstring-convention = numpy
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `PyMARE-0.0.4rc2/versioneer.py` & `PyMARE-0.0.4rc6/versioneer.py`

 * *Files identical despite different names*

