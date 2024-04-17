# Comparing `tmp/adaptive_neighbourhoods-0.0.2.tar.gz` & `tmp/adaptive_neighbourhoods-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "adaptive_neighbourhoods-0.1.0.tar", last modified: Wed Apr 17 15:00:02 2024, max compression
```

## Comparing `adaptive_neighbourhoods-0.0.2.tar` & `adaptive_neighbourhoods-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,17 @@
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 adaptive_neighbourhoods-0.0.2/Makefile
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 adaptive_neighbourhoods-0.0.2/environment.yml
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 adaptive_neighbourhoods-0.0.2/adaptive_neighbourhoods/__init__.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 adaptive_neighbourhoods-0.0.2/adaptive_neighbourhoods/_types.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 adaptive_neighbourhoods-0.0.2/adaptive_neighbourhoods/distances.py
--rw-r--r--   0        0        0     3869 2020-02-02 00:00:00.000000 adaptive_neighbourhoods-0.0.2/adaptive_neighbourhoods/neighbourhoods.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 adaptive_neighbourhoods-0.0.2/docs/Makefile
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 adaptive_neighbourhoods-0.0.2/docs/api.rst
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 adaptive_neighbourhoods-0.0.2/docs/conf.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 adaptive_neighbourhoods-0.0.2/docs/contributing.rst
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 adaptive_neighbourhoods-0.0.2/docs/examples.rst
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 adaptive_neighbourhoods-0.0.2/docs/index.rst
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 adaptive_neighbourhoods-0.0.2/docs/installation.rst
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 adaptive_neighbourhoods-0.0.2/docs/iris.org
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 adaptive_neighbourhoods-0.0.2/docs/make.bat
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 adaptive_neighbourhoods-0.0.2/docs/performance.rst
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 adaptive_neighbourhoods-0.0.2/docs/requirements.txt
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 adaptive_neighbourhoods-0.0.2/docs/generated/adaptive_neighbourhoods.neighbourhoods.rst
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 adaptive_neighbourhoods-0.0.2/docs/generated/adaptive_neighbourhoods.rst
--rw-r--r--   0        0        0    30168 2020-02-02 00:00:00.000000 adaptive_neighbourhoods-0.0.2/docs/images/iris.png
--rw-r--r--   0        0        0    82021 2020-02-02 00:00:00.000000 adaptive_neighbourhoods-0.0.2/docs/images/iris_1.png
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 adaptive_neighbourhoods-0.0.2/tests/test_distances.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 adaptive_neighbourhoods-0.0.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 adaptive_neighbourhoods-0.0.2/LICENSE
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 adaptive_neighbourhoods-0.0.2/README.md
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 adaptive_neighbourhoods-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 adaptive_neighbourhoods-0.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:00:02.871542 adaptive_neighbourhoods-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-17 14:59:29.000000 adaptive_neighbourhoods-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-17 15:00:02.871542 adaptive_neighbourhoods-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-17 14:59:29.000000 adaptive_neighbourhoods-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-17 14:59:29.000000 adaptive_neighbourhoods-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 15:00:02.871542 adaptive_neighbourhoods-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-17 14:59:29.000000 adaptive_neighbourhoods-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:00:02.867542 adaptive_neighbourhoods-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:00:02.871542 adaptive_neighbourhoods-0.1.0/src/adaptive_neighbourhoods.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-17 15:00:02.000000 adaptive_neighbourhoods-0.1.0/src/adaptive_neighbourhoods.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-17 15:00:02.000000 adaptive_neighbourhoods-0.1.0/src/adaptive_neighbourhoods.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 15:00:02.000000 adaptive_neighbourhoods-0.1.0/src/adaptive_neighbourhoods.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-17 15:00:02.000000 adaptive_neighbourhoods-0.1.0/src/adaptive_neighbourhoods.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 15:00:02.000000 adaptive_neighbourhoods-0.1.0/src/adaptive_neighbourhoods.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-04-17 14:59:29.000000 adaptive_neighbourhoods-0.1.0/src/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:00:02.867542 adaptive_neighbourhoods-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-17 14:59:29.000000 adaptive_neighbourhoods-0.1.0/tests/test_iris.py
```

### Comparing `adaptive_neighbourhoods-0.0.2/LICENSE` & `adaptive_neighbourhoods-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adaptive_neighbourhoods-0.0.2/README.md` & `adaptive_neighbourhoods-0.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 <div align="center">
 
+![](./docs/logo.png)
+
 ## Adaptive Neighbourhoods for the Discovery<br/> of Adversarial Examples
 
 Python API for generating adapted and unique neighbourhoods for
 searching for adversarial examples
 
 [![PyPI](https://img.shields.io/pypi/v/adaptive-neighbourhoods?style=flat-square&color=green)](https://pypi.python.org/pypi/adaptive-neighbourhoods/)
 [![GitHub license](https://img.shields.io/github/license/jaypmorgan/adaptive-neighbourhoods.svg?style=flat-square)](https://github.com/jaypmorgan/adaptive-neighbourhoods/blob/master/LICENSE)
@@ -25,15 +27,15 @@
 from adaptive_neighbourhoods import epsilon_expand
 
 neighbourhoods = epsilon_expand(
     x,  # your input data
     y)  # the integer encoded labels for your data
 ```
 
-Move information on the variable parameters and general guidance on using this package can be found at: https://jaypmorgan.github.io/adaptive-neighbourhoods/
+Move information on the variable parameters and general guidance on using this package can be found at: https://adaptive-neighbourhoods.readthedocs.io/en/latest/
 
 ## Contributing
 
 All contributions and feedback are welcome!
 
 There are three main remote mirrors used for hosting this project. If
 you would like to contribute, please submit an
@@ -46,15 +48,15 @@
 ## Citing this work
 
 If you use this work in your research, please consider referencing our
 article using the following bibtex entry:
 
 ```
 @article{DBLP:journals/corr/abs-2101-09108,
-  author    = {Jay Morgan and
+  author    = {Jay Paul Morgan and
                Adeline Paiement and
                Arno Pauly and
                Monika Seisenberger},
   title     = {Adaptive Neighbourhoods for the Discovery of Adversarial Examples},
   journal   = {CoRR},
   volume    = {abs/2101.09108},
   year      = {2021},
```

### Comparing `adaptive_neighbourhoods-0.0.2/pyproject.toml` & `adaptive_neighbourhoods-0.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["setuptools>=42", "pybind11>=2.6.1"]
+build-backend = "setuptools.build_meta"
 
 [project]
 name = "adaptive_neighbourhoods"
-version = "0.0.2"
+version = "0.1.0"
 authors = [
-  {name="Jay Morgan", email="jaymiles17@gmail.com"},
+  {name="Jay Paul Morgan", email="j.p.morgan@swansea.ac.uk"},
   {name="Adeline Paiement"},
   {name="Arno Pauly"},
   {name="Monika Seisenberger"},
 ]
 description = "Python API for generating adapted and unique neighbourhoods for searching for adversarial examples."
 readme = "README.md"
 requires-python = ">=3.6"
@@ -19,7 +19,17 @@
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/jaypmorgan/adaptive-neighbourhoods"
 "Bug Tracker" = "https://github.com/jaypmorgan/adaptive-neighbourhoods/issues"
+
+[project.optional-dependencies]
+dev = [
+    "pandas",
+    "numpy",
+    "requests",
+    "build",
+    "twine",
+    "pytest",
+]
```

### Comparing `adaptive_neighbourhoods-0.0.2/PKG-INFO` & `adaptive_neighbourhoods-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 Metadata-Version: 2.1
 Name: adaptive_neighbourhoods
-Version: 0.0.2
+Version: 0.1.0
 Summary: Python API for generating adapted and unique neighbourhoods for searching for adversarial examples.
+Author: Adeline Paiement, Arno Pauly, Monika Seisenberger
+Author-email: Jay Paul Morgan <j.p.morgan@swansea.ac.uk>
 Project-URL: Homepage, https://github.com/jaypmorgan/adaptive-neighbourhoods
 Project-URL: Bug Tracker, https://github.com/jaypmorgan/adaptive-neighbourhoods/issues
-Author: Adeline Paiement, Arno Pauly, Monika Seisenberger
-Author-email: Jay Morgan <jaymiles17@gmail.com>
-License-File: LICENSE
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Provides-Extra: dev
+Requires-Dist: pandas; extra == "dev"
+Requires-Dist: numpy; extra == "dev"
+Requires-Dist: requests; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
 
 <div align="center">
 
+![](./docs/logo.png)
+
 ## Adaptive Neighbourhoods for the Discovery<br/> of Adversarial Examples
 
 Python API for generating adapted and unique neighbourhoods for
 searching for adversarial examples
 
 [![PyPI](https://img.shields.io/pypi/v/adaptive-neighbourhoods?style=flat-square&color=green)](https://pypi.python.org/pypi/adaptive-neighbourhoods/)
 [![GitHub license](https://img.shields.io/github/license/jaypmorgan/adaptive-neighbourhoods.svg?style=flat-square)](https://github.com/jaypmorgan/adaptive-neighbourhoods/blob/master/LICENSE)
@@ -40,15 +49,15 @@
 from adaptive_neighbourhoods import epsilon_expand
 
 neighbourhoods = epsilon_expand(
     x,  # your input data
     y)  # the integer encoded labels for your data
 ```
 
-Move information on the variable parameters and general guidance on using this package can be found at: https://jaypmorgan.github.io/adaptive-neighbourhoods/
+Move information on the variable parameters and general guidance on using this package can be found at: https://adaptive-neighbourhoods.readthedocs.io/en/latest/
 
 ## Contributing
 
 All contributions and feedback are welcome!
 
 There are three main remote mirrors used for hosting this project. If
 you would like to contribute, please submit an
@@ -61,15 +70,15 @@
 ## Citing this work
 
 If you use this work in your research, please consider referencing our
 article using the following bibtex entry:
 
 ```
 @article{DBLP:journals/corr/abs-2101-09108,
-  author    = {Jay Morgan and
+  author    = {Jay Paul Morgan and
                Adeline Paiement and
                Arno Pauly and
                Monika Seisenberger},
   title     = {Adaptive Neighbourhoods for the Discovery of Adversarial Examples},
   journal   = {CoRR},
   volume    = {abs/2101.09108},
   year      = {2021},
```

