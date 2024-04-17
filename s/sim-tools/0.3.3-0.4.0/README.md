# Comparing `tmp/sim-tools-0.3.3.tar.gz` & `tmp/sim_tools-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sim-tools-0.3.3.tar", last modified: Wed Feb  7 12:13:19 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `sim-tools-0.3.3.tar` & `sim_tools-0.4.0.tar`

### file list

```diff
@@ -1,27 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:13:19.237686 sim-tools-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-02-07 12:13:09.000000 sim-tools-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-02-07 12:13:19.237686 sim-tools-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-02-07 12:13:09.000000 sim-tools-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 12:13:19.237686 sim-tools-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-02-07 12:13:09.000000 sim-tools-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:13:19.237686 sim-tools-0.3.3/sim_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-07 12:13:09.000000 sim-tools-0.3.3/sim_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-02-07 12:13:09.000000 sim-tools-0.3.3/sim_tools/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    33120 2024-02-07 12:13:09.000000 sim-tools-0.3.3/sim_tools/distributions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:13:19.237686 sim-tools-0.3.3/sim_tools/ovs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 12:13:09.000000 sim-tools-0.3.3/sim_tools/ovs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-02-07 12:13:09.000000 sim-tools-0.3.3/sim_tools/ovs/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13787 2024-02-07 12:13:09.000000 sim-tools-0.3.3/sim_tools/ovs/fixed_budget.py
--rw-r--r--   0 runner    (1001) docker     (127)    15134 2024-02-07 12:13:09.000000 sim-tools-0.3.3/sim_tools/ovs/indifference_zone.py
--rw-r--r--   0 runner    (1001) docker     (127)     9430 2024-02-07 12:13:09.000000 sim-tools-0.3.3/sim_tools/ovs/toy_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-02-07 12:13:09.000000 sim-tools-0.3.3/sim_tools/time_dependent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:13:19.237686 sim-tools-0.3.3/sim_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-02-07 12:13:19.000000 sim-tools-0.3.3/sim_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-02-07 12:13:19.000000 sim-tools-0.3.3/sim_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 12:13:19.000000 sim-tools-0.3.3/sim_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-07 12:13:19.000000 sim-tools-0.3.3/sim_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-07 12:13:19.000000 sim-tools-0.3.3/sim_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 12:13:19.237686 sim-tools-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-07 12:13:09.000000 sim-tools-0.3.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-02-07 12:13:09.000000 sim-tools-0.3.3/tests/test_dists.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-02-07 12:13:09.000000 sim-tools-0.3.3/tests/test_time_dep.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 sim_tools-0.4.0/sim_tools/__init__.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 sim_tools-0.4.0/sim_tools/datasets.py
+-rw-r--r--   0        0        0    33120 2020-02-02 00:00:00.000000 sim_tools-0.4.0/sim_tools/distributions.py
+-rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 sim_tools-0.4.0/sim_tools/time_dependent.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 sim_tools-0.4.0/sim_tools/data/nspp_example1.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sim_tools-0.4.0/sim_tools/ovs/__init__.py
+-rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 sim_tools-0.4.0/sim_tools/ovs/evaluation.py
+-rw-r--r--   0        0        0    13787 2020-02-02 00:00:00.000000 sim_tools-0.4.0/sim_tools/ovs/fixed_budget.py
+-rw-r--r--   0        0        0    15134 2020-02-02 00:00:00.000000 sim_tools-0.4.0/sim_tools/ovs/indifference_zone.py
+-rw-r--r--   0        0        0     9430 2020-02-02 00:00:00.000000 sim_tools-0.4.0/sim_tools/ovs/toy_models.py
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 sim_tools-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 sim_tools-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 sim_tools-0.4.0/README.md
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 sim_tools-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 sim_tools-0.4.0/PKG-INFO
```

### Comparing `sim-tools-0.3.3/LICENSE` & `sim_tools-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sim-tools-0.3.3/PKG-INFO` & `sim_tools-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: sim-tools
-Version: 0.3.3
+Version: 0.4.0
 Summary: Simulation Tools for Education and Practice
-Home-page: https://github.com/TomMonks/sim-tools
-Author: Thomas Monks
-Author-email: t.m.w.monks@exeter.ac.uk
-License: The MIT License (MIT)
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Project-URL: Homepage, https://github.com/TomMonks/sim-tools
+Project-URL: Bug Tracker, https://github.com/TomMonks/sim-tools/issues
+Project-URL: Documentation, https://tommonks.github.io/sim-tools
+Author-email: Thomas Monks <t.m.w.monks@exeter.ac.uk>
+License-Expression: MIT
+License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: matplotlib>=3.1.3
 Requires-Dist: numpy>=1.18.1
 Requires-Dist: pandas>=2.0.0
-Requires-Dist: scipy>=1.4.1
 Requires-Dist: scikit-learn>=1.0.0
+Requires-Dist: scipy>=1.4.1
+Description-Content-Type: text/markdown
 
 # sim-tools: tools to support the simulation process in python.
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/TomMonks/sim-tools/HEAD)
 [![DOI](https://zenodo.org/badge/225608065.svg)](https://zenodo.org/badge/latestdoi/225608065)
 [![PyPI version fury.io](https://badge.fury.io/py/sim-tools.svg)](https://pypi.python.org/pypi/sim-tools/)
 [![Read the Docs](https://readthedocs.org/projects/pip/badge/?version=latest)](https://tommonks.github.io/sim-tools)
```

### Comparing `sim-tools-0.3.3/README.md` & `sim_tools-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `sim-tools-0.3.3/sim_tools/datasets.py` & `sim_tools-0.4.0/sim_tools/datasets.py`

 * *Files identical despite different names*

### Comparing `sim-tools-0.3.3/sim_tools/distributions.py` & `sim_tools-0.4.0/sim_tools/distributions.py`

 * *Files identical despite different names*

### Comparing `sim-tools-0.3.3/sim_tools/ovs/evaluation.py` & `sim_tools-0.4.0/sim_tools/ovs/evaluation.py`

 * *Files identical despite different names*

### Comparing `sim-tools-0.3.3/sim_tools/ovs/fixed_budget.py` & `sim_tools-0.4.0/sim_tools/ovs/fixed_budget.py`

 * *Files identical despite different names*

### Comparing `sim-tools-0.3.3/sim_tools/ovs/indifference_zone.py` & `sim_tools-0.4.0/sim_tools/ovs/indifference_zone.py`

 * *Files identical despite different names*

### Comparing `sim-tools-0.3.3/sim_tools/ovs/toy_models.py` & `sim_tools-0.4.0/sim_tools/ovs/toy_models.py`

 * *Files identical despite different names*

### Comparing `sim-tools-0.3.3/sim_tools/time_dependent.py` & `sim_tools-0.4.0/sim_tools/time_dependent.py`

 * *Files identical despite different names*

