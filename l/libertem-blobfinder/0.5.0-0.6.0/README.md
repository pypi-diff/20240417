# Comparing `tmp/libertem-blobfinder-0.5.0.tar.gz` & `tmp/libertem_blobfinder-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libertem-blobfinder-0.5.0.tar", last modified: Mon May  8 12:58:12 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `libertem-blobfinder-0.5.0.tar` & `libertem_blobfinder-0.6.0.tar`

### file list

```diff
@@ -1,39 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:12.790321 libertem-blobfinder-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-08 12:58:12.790321 libertem-blobfinder-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:12.778321 libertem-blobfinder-0.5.0/libertem_blobfinder/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-08 12:58:12.782321 libertem-blobfinder-0.5.0/libertem_blobfinder/_baked_revision.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-08 12:58:12.790321 libertem-blobfinder-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:12.782321 libertem-blobfinder-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:12.786321 libertem-blobfinder-0.5.0/src/libertem_blobfinder/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:12.786321 libertem-blobfinder-0.5.0/src/libertem_blobfinder/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16944 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder/base/correlation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:12.786321 libertem-blobfinder-0.5.0/src/libertem_blobfinder/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder/common/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder/common/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:12.786321 libertem-blobfinder-0.5.0/src/libertem_blobfinder/udf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder/udf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15201 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder/udf/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder/udf/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder/udf/refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder/udf/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder/versioning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:12.786321 libertem-blobfinder-0.5.0/src/libertem_blobfinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-05-08 12:58:12.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-08 12:58:12.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:58:12.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:58:12.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-08 12:58:12.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-08 12:58:12.000000 libertem-blobfinder-0.5.0/src/libertem_blobfinder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:12.790321 libertem-blobfinder-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    20203 2023-05-08 12:57:48.000000 libertem-blobfinder-0.5.0/tests/test_udf.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/.codeclimate.yml
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/.travis.yml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/MANIFEST.in
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/README.rst
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/codecov.yml
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/conftest.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/docs_requirements.txt
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/pytest.ini
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/setup.cfg
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/test_requirements.txt
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/tox.ini
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/.github/PULL_REQUEST_TEMPLATE
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/corporatedesign/logo/favicon.ico
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/docs/Makefile
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/docs/make.bat
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/docs/source/acknowledgments.rst
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/docs/source/changelog.rst
+-rw-r--r--   0        0        0     6990 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/docs/source/conf.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/docs/source/examples.rst
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/docs/source/index.rst
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/docs/source/install.rst
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/docs/source/reference.rst
+-rw-r--r--   0        0        0    49854 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/docs/source/references-libertem_blobfinder.bib
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/docs/source/strainmap-SiGe.nblink
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/docs/source/strainmap-poly.nblink
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/docs/source/upsampling.nblink
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/docs/source/usage.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/docs/source/_static/.gitignore
+-rw-r--r--   0        0        0    46287 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/docs/source/_static/logo.png
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/docs/source/_static/css/custom.css
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/docs/source/autogenerated/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/docs/source/changelog/bugfix/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/docs/source/changelog/documentation/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/docs/source/changelog/features/.gitignore
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/docs/source/changelog/features/gpu_and_sparse.rst
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/docs/source/changelog/features/upsampling.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/docs/source/changelog/misc/.gitignore
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/docs/source/changelog/misc/dependency-refactor.rst
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/docs/source/changelog/misc/gridmatching.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/docs/source/changelog/obsolescence/.gitignore
+-rw-r--r--   0        0        0  1223158 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/examples/peak_selector.ipynb
+-rw-r--r--   0        0        0  3104710 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/examples/strainmap-SiGe.ipynb
+-rw-r--r--   0        0        0  6357608 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/examples/strainmap-poly.ipynb
+-rw-r--r--   0        0        0   194147 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/examples/upsampling-refinement.ipynb
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/packaging/contributors.json
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/packaging/creators.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/packaging/zenodo-upload.json
+-rw-r--r--   0        0        0   223203 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/prototypes/integration.ipynb
+-rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/scripts/creatorlist.ipynb
+-rwxr-xr-x   0        0        0    20296 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/scripts/release
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/scripts/requirements.txt
+-rw-r--r--   0        0        0    11719 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/scripts/zenodo_upload
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/src/libertem_blobfinder/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/src/libertem_blobfinder/__version__.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/src/libertem_blobfinder/versioning.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/src/libertem_blobfinder/base/__init__.py
+-rw-r--r--   0        0        0    26542 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/src/libertem_blobfinder/base/correlation.py
+-rw-r--r--   0        0        0    13505 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/src/libertem_blobfinder/base/masks.py
+-rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/src/libertem_blobfinder/base/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/src/libertem_blobfinder/common/__init__.py
+-rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/src/libertem_blobfinder/common/correlation.py
+-rw-r--r--   0        0        0    16828 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/src/libertem_blobfinder/common/fullmatch.py
+-rw-r--r--   0        0        0    18504 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/src/libertem_blobfinder/common/gridmatching.py
+-rw-r--r--   0        0        0    11695 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/src/libertem_blobfinder/common/patterns.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/src/libertem_blobfinder/udf/__init__.py
+-rw-r--r--   0        0        0    19630 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/src/libertem_blobfinder/udf/correlation.py
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/src/libertem_blobfinder/udf/integration.py
+-rw-r--r--   0        0        0    10760 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/src/libertem_blobfinder/udf/refinement.py
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/src/libertem_blobfinder/udf/utils.py
+-rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/tests/test_base.py
+-rw-r--r--   0        0        0     5464 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/tests/test_common.py
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/tests/test_fullmatch.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/tests/test_gridmatching.py
+-rw-r--r--   0        0        0     4298 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/tests/test_masks.py
+-rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/tests/utils.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/tests/udf/conftest.py
+-rw-r--r--   0        0        0    23917 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/tests/udf/test_udf.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/hatch_build.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 libertem_blobfinder-0.6.0/PKG-INFO
```

### Comparing `libertem-blobfinder-0.5.0/LICENSE` & `libertem_blobfinder-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libertem-blobfinder-0.5.0/README.rst` & `libertem_blobfinder-0.6.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Installation
 ------------
 
 The quick version from PyPI:
 
 .. code-block:: shell
 
-    $ pip install libertem-blobfinder[pyfftw]
+    $ pip install libertem-blobfinder[udf]
 
 See `full installation instructions
 <https://libertem.github.io/LiberTEM-blobfinder/install.html>`_ for more
 details!
 
 .. rubric:: Reference
```

### Comparing `libertem-blobfinder-0.5.0/src/libertem_blobfinder/base/correlation.py` & `libertem_blobfinder-0.6.0/src/libertem_blobfinder/base/correlation.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,118 @@
 import os
+from typing import Union, Tuple
 
 import numpy as np
+import numpy.typing as npt
 import numba
+import sparseconverter
 
 
-# FIXME There's work on flexible FFT backends in scipy
-# https://github.com/scipy/scipy/wiki/GSoC-2019-project-ideas#revamp-scipyfftpack
-# and discussions about pyfftw performance vs other implementations
-# https://github.com/pyFFTW/pyFFTW/issues/264
-# For that reason we shoud review the state of Python FFT implementations
-# regularly and adapt our choices accordingly
-try:
-    import pyfftw
-    fft = pyfftw.interfaces.numpy_fft
-    pyfftw.interfaces.cache.enable()
-    zeros = pyfftw.zeros_aligned
-except ImportError:
-    fft = np.fft
-    zeros = np.zeros
+fft = np.fft
+zeros = np.zeros
 
 # Necessary to work with JIT disabled for coverage and testing purposes
 # https://github.com/LiberTEM/LiberTEM/issues/539
 if os.getenv('NUMBA_DISABLE_JIT'):
     def to_fixed_tuple(array, length):
         return tuple(array)
 else:
     from numba.np.unsafe.ndarray import to_fixed_tuple
 
 
+def _upsampled_dft(
+    corrspecs: npt.NDArray,
+    frequencies: Tuple[np.ndarray, np.ndarray],
+    upsampled_region_size: int,
+    axis_offsets: Tuple[float, float],
+) -> np.ndarray:
+    """
+    Heavily adapted from skimage.registration._phase_cross_correlation.py
+    which is itself based on code by Manuel Guizar released initially under a
+    BSD 3-Clause license @ https://www.mathworks.com/matlabcentral/fileexchange/18401
+
+    :meta private:
+    """
+    im2pi = -1j * 2 * np.pi
+    upsampled = corrspecs
+    for (ax_freq, ax_offset) in zip(frequencies[::-1], axis_offsets[::-1]):
+        kernel = np.linspace(
+            -ax_offset,
+            (-ax_offset + upsampled_region_size - 1),
+            num=int(upsampled_region_size),
+        )
+        kernel = np.exp(kernel[:, None] * ax_freq * im2pi, dtype=np.complex64)
+        # Equivalent to:
+        #   data[i, j, k] = kernel[i, :] @ data[j, k].T
+        upsampled = np.tensordot(kernel, upsampled, axes=(1, -1))
+    return upsampled
+
+
+def refine_center_upsampling(
+    corrmap_center: npt.NDArray,
+    upsample_pos: npt.NDArray,
+    corrspecs: npt.NDArray,
+    frequencies: Tuple[npt.NDArray, npt.NDArray],
+    upsample_factor: int,
+) -> npt.NDArray:
+    '''
+    Parameters
+    ----------
+    corrmap_center : np.ndarray[(2,), np.float32]
+        The centre of the correlation map resulting from irfft(corrspecs)
+    upsample_pos : np.ndarray[(2,), np.float32]
+        (y, x) coordinates of the argmax position within the correlation map
+    corrspecs : np.ndarray[(2,), np.float32]
+        The rfft2 of the correlation map (last dimension halved + 1, normally)
+    frequencies : Tuple[np.ndarray[(2,), np.float32]]
+        The fft frequencies corresponding to the axes of corrspecs
+    upsample_factor : int
+        The number of upsampled pixels per pixel in the original correlation map
+        when finding the refined position. Directly determines the precision of the
+        result (e.g. 20 => 0.05 pixel precision).
+
+    Returns
+    -------
+    refined : np.ndarray[(2,), np.float32]
+        The position of the refined maximum
+
+    :meta private:
+    '''
+    # Same license info as in the function _upsampled_dft
+
+    # Move the real position in corr to the position
+    # in the fft (essentially apply fftshift without wrapping)
+    shift = upsample_pos - corrmap_center
+    shift_us = np.round(shift * upsample_factor)
+
+    upsampled_region_size = np.ceil(upsample_factor * 1.5)
+    dftshift = np.fix(upsampled_region_size / 2.0)
+    sample_region_offset = dftshift - shift_us
+
+    cross_correlation_us = _upsampled_dft(
+        corrspecs=corrspecs.conj(),
+        frequencies=frequencies,
+        upsampled_region_size=upsampled_region_size,
+        axis_offsets=sample_region_offset,
+    ).conj()
+
+    # Find the argmax in the upsampled corrmap
+    maxima = np.unravel_index(
+        np.abs(cross_correlation_us).argmax(),
+        cross_correlation_us.shape,
+    )
+    maxima = np.stack(maxima).astype(np.float32, copy=False)
+    maxima -= dftshift
+
+    # Transform the maximum back into the coordinate system of corr
+    shift += maxima / upsample_factor
+    shift += corrmap_center
+    return shift.astype(np.float32)
+
+
 @numba.njit
 def center_of_mass(arr):
     r_y = r_x = np.float32(0)
     for y in range(arr.shape[0]):
         for x in range(arr.shape[1]):
             r_y += np.float32(arr[y, x]*y)
             r_x += np.float32(arr[y, x]*x)
@@ -56,15 +137,15 @@
         refined_y = y + ry - r
         refined_x = x + rx - r
         # print(y, x, refined_y, refined_x, "\n", cutout)
         return (np.float32(refined_y), np.float32(refined_x))
 
 
 @numba.njit
-def peak_elevation(center, corrmap, height, r_min=1.5, r_max=float('inf')):
+def peak_elevation(center, corrmap, height, r_min=1.5, r_max=np.inf):
     '''
     Return the slope of the tightest cone around :code:`center` with height :code:`height`
     that touches :code:`corrmap` between :code:`r_min` and :code:`r_max`.
 
     The correlation of two disks -- mask and perfect diffraction spot -- has the shape of a cone.
     The function's return value correlates with the quality of a correlation. Higher slope
     means a strong peak and
@@ -100,36 +181,50 @@
         for x in range(size_x):
             dist = np.sqrt((y - peak_y)**2 + (x - peak_x)**2)
             if (dist >= r_min) and (dist < r_max):
                 result = min((result, np.float32((height - corrmap[y, x]) / dist)))
     return max(0, result)
 
 
-def do_correlations(template, crop_parts):
+def do_correlations(template, crop_parts, with_specs: bool = False):
     '''
     Calculate the correlation of the pre-calculated template with a stack
     of cropped peaks using fast correlation.
 
     Parameters
     ----------
     template : numpy.ndarray
         Real Fourier transform of the correlation pattern.
         The source pattern should have the same size as the cropped parts. Please note that
         the real Fourier transform (fft.rfft2) of the source pattern has a different shape!
     crop_parts : numpy.ndarray
         Stack of peaks cropped from the frame.
+    with_specs: bool, optional
+        Whether to return the FFT correlation maps before inversion,
+        used for FFT upsampling. By default, False.
 
     Returns
     -------
     corrs : numpy.ndarray
         Correlation of the correlation pattern and the peaks.
+    corrspecs : numpy.ndarray
+        The FFT correlation maps before inversion, returned only
+        if with_specs is True.
     '''
     spec_parts = fft.rfft2(crop_parts)
     corrspecs = template * spec_parts
-    corrs = fft.fftshift(fft.irfft2(corrspecs), axes=(-1, -2))
+    corrs = fft.ifftshift(
+        fft.irfft2(
+            corrspecs,
+            s=crop_parts.shape[-2:],
+        ),
+        axes=(-2, -1),
+    )
+    if with_specs:
+        return corrs, corrspecs
     return corrs
 
 
 @numba.njit
 def unravel_index(index, shape):
     sizes = np.zeros(len(shape), dtype=np.int64)
     result = np.zeros(len(shape), dtype=np.int64)
@@ -153,14 +248,82 @@
         height = np.float32(corr[center])
         out_centers[i] = _shift(np.array(center), peaks[i], crop_size)
         out_refineds[i] = _shift(refined, peaks[i], crop_size)
         out_heights[i] = height
         out_elevations[i] = np.float32(peak_elevation(refined, corr, height))
 
 
+def evaluate_upsampling(corrspecs, corrs, peaks, crop_size, sig_shape, upsample_factor,
+        out_centers, out_refineds):
+    """
+    Evaluate the refined peak positions using DFT upsampling
+
+    Internally re-inverts corrspecs with upsampling around
+    the positions found in out_centers, and places the
+    argmax of these new corrmaps into out_refineds.
+
+    This function operates either on a full-frame corrspecs (ndim of 2)
+    or a stack of corrspecs (ndim of 3) when using the 'fast' processing
+    mode (crops of the frame).
+
+    Parameters
+    ----------
+    corrspecs : numpy.ndarray
+        The rFFT correlations before inversion. If :code:`ndim == 3`
+        we are processing a stack of crops from a frame, while if
+        :code:`ndim == 2` we are processing the correlation map of
+        the whole frame.
+    corrs : numpy.ndarray
+        Stack of correlation maps, either matching the stack of corrspecs
+        (fast processing), or crops from the full-frame correlation map.
+    peaks : np.ndarray
+        List of peaks of shape (n_peaks, 2) in full-frame frame coordinates,
+        matching the order of corrs if processing crops.
+    crop_size : int
+        Half the size of the correlation pattern used to compute corrspecs.
+    sig_shape : Tuple[int, int]
+        The shape of the full frame
+    upsample_factor : int
+        The degree to upsample the frame, determines the precision
+        of the result (:code:`1 / upsample_factor`).
+    out_centers : np.ndarray
+        Buffer filled with for unrefined peak positions of shape (n_peaks, 2).
+        These are read to know the upsampling location.
+    out_refineds : np.ndarray
+        Output buffer for refined center positions of shape (n_peaks, 2)
+        and float dtype, values will be overwritten with the upsampled coordinates.
+
+    :meta private:
+    """
+    # A corrspec stack means we are processing corrspecs of crops of the frame
+    # and corrs are the irfft2 of each corrspec. Otherwise, corrspecs is the single rfft2
+    # of the whole frame and corrs are the crops from the irfft2 of corrspecs.
+    # An alternative to these gynmastics is specialise evaluate_upsampling into
+    # evaluate_upsampling_fast and evaluate_upsampling_full
+    corrspec_stack = corrspecs.ndim == 3
+    corr_shape = corrs.shape[1:] if corrspec_stack else sig_shape
+    corr_center = np.ceil(np.asarray(corr_shape) / 2, dtype=np.float32)
+
+    frequencies = (
+        fft.fftfreq(corr_shape[0], upsample_factor),
+        fft.rfftfreq(corr_shape[1], upsample_factor),
+    )
+
+    for i in range(len(corrs)):
+        corrspec = corrspecs[i] if corrspec_stack else corrspecs
+        center = out_centers[i]
+        if corrspec_stack:
+            center = _unshift(center, peaks[i], crop_size)
+        out_refineds[i] = refine_center_upsampling(
+            corr_center, center, corrspec, frequencies, upsample_factor=upsample_factor
+        )
+        if corrspec_stack:
+            out_refineds[i] = _shift(out_refineds[i], peaks[i], crop_size)
+
+
 def log_scale(data, out):
     return np.log(data - np.min(data) + 1, out=out)
 
 
 def log_scale_cropbufs_inplace(crop_bufs):
     m = np.min(crop_bufs, axis=(-1, -2)) - 1
     np.log(crop_bufs - m[:, np.newaxis, np.newaxis], out=crop_bufs)
@@ -186,19 +349,59 @@
                 x_outside = xx < 0 or xx >= fx
                 if y_outside or x_outside:
                     out_crop_bufs[i, y, x] = 0
                 else:
                     out_crop_bufs[i, y, x] = frame[yy, xx]
 
 
+def crop_disks_from_frame_slicing(peaks, frame, crop_size, out_crop_bufs):
+
+    def frame_coord_y(peak, y):
+        return y + peak[0] - crop_size
+
+    def frame_coord_x(peak, x):
+        return x + peak[1] - crop_size
+
+    fy, fx = frame.shape
+    target_backend = sparseconverter.get_backend(out_crop_bufs)
+    for i in range(len(peaks)):
+        peak = peaks[i]
+        origin_y = frame_coord_y(peak, 0)
+        origin_x = frame_coord_x(peak, 0)
+        end_y = frame_coord_y(peak, out_crop_bufs.shape[1])
+        end_x = frame_coord_x(peak, out_crop_bufs.shape[2])
+        skip_y = max(-origin_y, 0)
+        skip_x = max(-origin_x, 0)
+
+        cut_y = fy - end_y
+        if cut_y >= 0:
+            cut_y = None
+        cut_x = fx - end_x
+        if cut_x >= 0:
+            cut_x = None
+
+        out_crop_bufs[i, skip_y:cut_y, skip_x:cut_x] = sparseconverter.for_backend(
+            frame[
+                max(origin_y, 0):max(end_y, 0),
+                max(origin_x, 0):max(end_x, 0)
+            ],
+            target_backend
+        )
+
+
 @numba.njit
 def _shift(relative_center, anchor, crop_size):
     return relative_center + anchor - np.array((crop_size, crop_size))
 
 
+@numba.njit
+def _unshift(center, anchor, crop_size):
+    return center - anchor + np.array((crop_size, crop_size))
+
+
 def get_buf_count(crop_size, n_peaks, dtype, limit=2**19):
     '''
     Calculate the optimal number of peaks in a stack to fit
     within the limit.
 
     Parameters
     ----------
@@ -216,15 +419,15 @@
     int
     '''
     dtype = np.dtype(dtype)
     full_size = (2 * crop_size)**2 * dtype.itemsize
     return min(max(1, limit // full_size), n_peaks)
 
 
-def allocate_crop_bufs(crop_size, n_peaks, dtype, limit=2**19):
+def allocate_crop_bufs(crop_size, n_peaks, dtype, limit=2**19, xp=np):
     '''
     Allocate buffer for stack of cropped peaks
 
     The size is optimized to fit within :code:`limit`. An aligned buffer for the FFT
     back-end is created if possible.
 
     Parameters
@@ -240,21 +443,24 @@
 
     Returns
     -------
     crop_bufs: np.ndarray
         Shape (n, 2*crop_size, 2*crop_size)
     '''
     buf_count = get_buf_count(crop_size, n_peaks, dtype, limit)
-    crop_bufs = zeros((buf_count, 2 * crop_size, 2 * crop_size), dtype=dtype)
+    crop_bufs = xp.zeros((buf_count, 2 * crop_size, 2 * crop_size), dtype=dtype)
     return crop_bufs
 
 
-def process_frame_fast(template, crop_size, frame, peaks,
-        out_centers, out_refineds, out_heights, out_elevations,
-        crop_bufs):
+def process_frame_fast(
+    template, crop_size, frame, peaks,
+    out_centers, out_refineds, out_heights, out_elevations,
+    crop_bufs, upsample: Union[bool, int] = False,
+    crop_function=crop_disks_from_frame,
+):
     '''
     Find the parameters of peaks in a diffraction pattern by correlation with a template
 
     This function is designed to be used in an optimized pipeline with a pre-calculated
     Fourier transform of the match pattern and optional pre-allocated buffers.
     It is the engine of the :class:`libertem_blobfinder.udf.correlation.FastCorrelationUDF` for
     stand-alone use independent of LiberTEM.
@@ -262,16 +468,17 @@
     :meth:`libertem_blobfinder.common.correlation.process_frames_fast` offers a more
     convenient interface for batch processing.
 
     Parameters
     ----------
     template : numpy.ndarray
         Real Fourier transform of the correlation pattern.
-        The source pattern should have size (2 * crop_size, 2 * crop_size). Please note that
-        the real Fourier transform (fft.rfft2) of the source pattern has a different shape!
+        The source pattern shape should match the shape[1:] of crop_bufs.
+        Please note that the real Fourier transform (fft.rfft2) of the
+        source pattern has a different shape!
     crop_size : int
         Half the size of the correlation pattern. Given as a parameter since real Fourier
         transform changes the size.
     frame : np.ndarray
         Frame data. Currently, only Real values are supported.
     peaks : np.ndarray
         List of peaks of shape (n_peaks, 2)
@@ -280,30 +487,35 @@
     out_refineds : np.ndarray
         Output buffer for refined center positions of shape (n_peaks, 2) and float dtype.
     out_heights : np.ndarray
         Output buffer for peak height in log scaled frame. Shape (n_peaks, ) and float dtype.
     out_elevations : np.ndarray
         Output buffer for peak elevation in log scaled frame. Shape (n_peaks, ) and float dtype.
     crop_bufs : np.ndarray
-        Aligned buffer for pyfftw. Shape (n, 2 * crop_size, 2 * crop_size) and float dtype.
+        Temporary buffers for cropping. Shape (n, 2 * crop_size, 2 * crop_size) and float dtype.
         n doesn't have to match the number of peaks. Instead, it should be chosen for good L3 cache
         efficiency. :meth:`allocate_crop_bufs` can be used to allocate this buffer.
+    upsample : Union[bool, int], optional
+        Whether to use upsampling DFT for refinement. False to deactivate (default) or a positive
+        integer >1 to upsample by this factor when refining the correlation peak positions. Upsample
+        True will choose a sensible upsampling factor.
 
     Returns
     -------
     None
         The values are placed in the provided output buffers.
 
     Example
     -------
 
     >>> from libertem_blobfinder.common.patterns import RadialGradient
     >>> from libertem_blobfinder.base.correlation import allocate_crop_bufs
+    >>> from libertem_blobfinder.base.utils import cbed_frame
     >>>
-    >>> frames, indices, peaks = libertem.utils.generate.cbed_frame(radius=4)
+    >>> frames, indices, peaks = cbed_frame(radius=4)
     >>> pattern = RadialGradient(radius=4)
     >>> crop_size = pattern.get_crop_size()
     >>> template = pattern.get_template(sig_shape=(2 * crop_size, 2 * crop_size))
     >>>
     >>> centers = np.zeros((len(frames), len(peaks), 2), dtype=np.uint16)
     >>> refineds = np.zeros((len(frames), len(peaks), 2), dtype=np.float32)
     >>> heights = np.zeros((len(frames), len(peaks)), dtype=np.float32)
@@ -323,30 +535,49 @@
     '''
     buf_count = len(crop_bufs)
     block_count = (len(peaks) - 1) // buf_count + 1
     for block in range(block_count):
         start = block * buf_count
         stop = min((block + 1) * buf_count, len(peaks))
         size = stop - start
-        crop_disks_from_frame(
+        crop_function(
             peaks=peaks[start:stop], frame=frame, crop_size=crop_size,
             out_crop_bufs=crop_bufs[:size]
         )
         log_scale_cropbufs_inplace(crop_bufs[:size])
-        corrs = do_correlations(template, crop_bufs[:size])
+        corrs, corrspecs = do_correlations(
+            template,
+            crop_bufs[:size],
+            with_specs=True
+        )
+        corrs = sparseconverter.for_backend(
+            corrs,
+            sparseconverter.NUMPY,
+        )
+        corrspecs = sparseconverter.for_backend(
+            corrspecs,
+            sparseconverter.NUMPY,
+        )
         evaluate_correlations(
             corrs=corrs, peaks=peaks[start:stop], crop_size=crop_size,
             out_centers=out_centers[start:stop], out_refineds=out_refineds[start:stop],
             out_heights=out_heights[start:stop], out_elevations=out_elevations[start:stop]
         )
+        if int(upsample) > 1:
+            evaluate_upsampling(
+                corrspecs=corrspecs, corrs=crop_bufs[:size], peaks=peaks[start:stop],
+                crop_size=crop_size, sig_shape=frame.shape, upsample_factor=int(upsample),
+                out_centers=out_centers[start:stop], out_refineds=out_refineds[start:stop],
+            )
 
 
 def process_frame_full(template, crop_size, frame, peaks,
         out_centers=None, out_refineds=None, out_heights=None, out_elevations=None,
-        frame_buf=None, buf_count=None):
+        frame_buf=None, buf_count=None, upsample: Union[bool, int] = False,
+        crop_function=crop_disks_from_frame):
     '''
     Find the parameters of peaks in a diffraction pattern by correlation with a template
 
     This function is designed to be used in an optimized pipeline with a pre-calculated
     Fourier transform of the match pattern and optional pre-allocated buffers. It is the
     engine of the :class:`libertem_blobfinder.udf.correlation.FullFrameCorrelationUDF`
     for stand-alone use independent of LiberTEM.
@@ -354,15 +585,16 @@
     :meth:`libertem_blobfinder.common.correlation.process_frames_full` offers a more
     convenient interface for batch processing.
 
     Parameters
     ----------
     template : numpy.ndarray
         Real Fourier transform of the correlation pattern.
-        The source pattern should have size (2 * crop_size, 2 * crop_size). Please note that
+        The source pattern shape should match the argument crop_size, either the supplied
+        shape or (2 * crop_size, 2 * crop_size) if default. Please note that
         the real Fourier transform (fft.rfft2) of the source pattern has a different shape!
     crop_size : int
         Half the size of the correlation pattern. Given as a parameter since real Fourier
         transform changes the size.
     frame : np.ndarray
         Frame data. Currently, only real values are supported.
     peaks : np.ndarray
@@ -376,33 +608,38 @@
     out_heights : np.ndarray, optional
         Output buffer for peak height in log scaled frame. Shape (n_peaks, ) and float dtype. Will
         be allocated if needed.
     out_elevations : np.ndarray, optional
         Output buffer for peak elevation in log scaled frame. Shape (n_peaks, ) and float dtype.
         Will be allocated if needed.
     frame_buf : np.ndarray
-        Aligned buffer for FFT back-end, such as pyfftw. Shape of a frame and float dtype.
+        Temporary buffer for the FFT back-end. Shape of a frame and float dtype.
         :meth:`libertem_blobfinder.base.correlation.zero` can be used.
     buf_count : int
         Number of peaks to process per outer loop iteration. This allows optimization of L3 cache
         efficiency.
+    upsample : Union[bool, int], optional
+        Whether to use upsampling DFT for refinement. False to deactivate (default) or a positive
+        integer >1 to upsample by this factor when refining the correlation peak positions. Upsample
+        True will choose a sensible upsampling factor.
 
 
     Returns
     -------
     None
         The values are placed in the provided output buffers.
 
     Example
     -------
 
     >>> from libertem_blobfinder.common.patterns import RadialGradient
     >>> from libertem_blobfinder.base.correlation import get_buf_count, zeros
+    >>> from libertem_blobfinder.base.utils import cbed_frame
     >>>
-    >>> frames, indices, peaks = libertem.utils.generate.cbed_frame()
+    >>> frames, indices, peaks = cbed_frame()
     >>> pattern = RadialGradient(radius=4)
     >>> crop_size = pattern.get_crop_size()
     >>> template = pattern.get_template(sig_shape=frames[0].shape)
     >>>
     >>> centers = np.zeros((len(frames), len(peaks), 2), dtype=np.uint16)
     >>> refineds = np.zeros((len(frames), len(peaks), 2), dtype=np.float32)
     >>> heights = np.zeros((len(frames), len(peaks)), dtype=np.float32)
@@ -417,26 +654,48 @@
     ...         frame=f, peaks=peaks.astype(np.int32),
     ...         out_centers=centers[i], out_refineds=refineds[i],
     ...         out_heights=heights[i], out_elevations=elevations[i],
     ...         frame_buf=frame_buf, buf_count=buf_count
     ...     )
     >>> assert np.allclose(refineds[0], peaks, atol=0.1)
     '''
+    if upsample is True:
+        upsample = 20
     log_scale(frame, out=frame_buf)
     spec_part = fft.rfft2(frame_buf)
     corrspec = template * spec_part
-    corr = fft.fftshift(fft.irfft2(corrspec))
-    crop_bufs = np.zeros((buf_count, 2 * crop_size, 2 * crop_size), dtype=corr.dtype)
+    corr = fft.ifftshift(
+        fft.irfft2(
+            corrspec, s=frame_buf.shape[-2:],
+        ),
+        axes=(-2, -1),
+    )
+    corr = sparseconverter.for_backend(
+        corr,
+        sparseconverter.NUMPY,
+    )
+    corrspec = sparseconverter.for_backend(
+        corrspec,
+        sparseconverter.NUMPY,
+    )
+    crop_shape = (2 * crop_size, 2 * crop_size)
+    crop_bufs = np.zeros((buf_count, *crop_shape), dtype=corr.dtype)
     block_count = (len(peaks) - 1) // buf_count + 1
     for block in range(block_count):
         start = block * buf_count
         stop = min(len(peaks), (block + 1) * buf_count)
         size = stop - start
-        crop_disks_from_frame(
+        crop_function(
             peaks=peaks[start:stop], frame=corr, crop_size=crop_size,
             out_crop_bufs=crop_bufs[:size]
         )
         evaluate_correlations(
             corrs=crop_bufs[:size], peaks=peaks[start:stop], crop_size=crop_size,
             out_centers=out_centers[start:stop], out_refineds=out_refineds[start:stop],
             out_heights=out_heights[start:stop], out_elevations=out_elevations[start:stop]
         )
+        if int(upsample) > 1:
+            evaluate_upsampling(
+                corrspecs=corrspec, corrs=crop_bufs[:size], peaks=peaks[start:stop],
+                crop_size=crop_size, sig_shape=frame.shape, upsample_factor=int(upsample),
+                out_centers=out_centers[start:stop], out_refineds=out_refineds[start:stop],
+            )
```

### Comparing `libertem-blobfinder-0.5.0/src/libertem_blobfinder/common/correlation.py` & `libertem_blobfinder-0.6.0/src/libertem_blobfinder/common/correlation.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from typing import Union
+
 import numpy as np
 from skimage.feature import peak_local_max
 
 from libertem_blobfinder.common.patterns import MatchPattern
-from libertem_blobfinder import base
+from libertem_blobfinder.base import correlation
 
 
 def get_correlation(sum_result, match_pattern: MatchPattern):
     '''
     Calculate the correlation between :code:`sum_result` and :code:`match_pattern`.
 
     .. versionadded:: 0.4.0.dev0
@@ -17,25 +19,25 @@
     sum_result: numpy.ndarray
         2D result frame as correlation input
     match_pattern : MatchPattern
         Instance of :class:`~libertem_blobfinder.MatchPattern` to correlate
         :code:`sum_result` with
     '''
     spec_mask = match_pattern.get_template(sig_shape=sum_result.shape)
-    spec_sum = base.correlation.fft.rfft2(sum_result)
+    spec_sum = correlation.fft.rfft2(sum_result)
     corrspec = spec_mask * spec_sum
-    return base.correlation.fft.fftshift(base.correlation.fft.irfft2(corrspec))
+    return correlation.fft.fftshift(correlation.fft.irfft2(corrspec))
 
 
 def get_peaks(sum_result, match_pattern: MatchPattern, num_peaks):
     '''
     Find peaks of the correlation between :code:`sum_result` and :code:`match_pattern`.
 
     The result  can then be used as input to
-    :meth:`~libertem.analysis.fullmatch.FullMatcher.full_match`
+    :meth:`~libertem_blobfinder.common.fullmatch.FullMatcher.full_match`
     to extract grid parameters, :meth:`~libertem_blobfinder.correlation.run_fastcorrelation`
     to find the position in each frame or to construct a mask to extract feature vectors with
     :meth:`~libertem_blobfinder.common.patterns.feature_vector`.
 
     Parameters
     ----------
 
@@ -45,16 +47,17 @@
         Instance of :class:`~libertem_blobfinder.MatchPattern` to correlate
         :code:`sum_result` with
     num_peaks : int
         Number of peaks to find
 
     Example
     -------
-
-    >>> frame, _, _ = libertem.utils.generate.cbed_frame(radius=4)
+    >>> from libertem_blobfinder.base.utils import cbed_frame
+    >>>
+    >>> frame, _, _ = cbed_frame(radius=4)
     >>> pattern = libertem_blobfinder.common.patterns.RadialGradient(radius=4)
     >>> peaks = get_peaks(frame[0], pattern, 7)
     >>> print(peaks)
     [[64 64]
      [64 80]
      [80 80]
      [80 64]
@@ -63,15 +66,18 @@
      [64 96]]
     '''
     corr = get_correlation(sum_result, match_pattern)
     peaks = peak_local_max(corr, num_peaks=num_peaks)
     return peaks
 
 
-def process_frames_fast(pattern: MatchPattern, frames, peaks):
+def process_frames_fast(
+    pattern: MatchPattern, frames, peaks,
+    upsample: Union[bool, int] = False
+):
     '''
     Find the parameters of peaks in a diffraction pattern by correlation with a match pattern.
 
     This method crops regions of interest around the peaks from the frames before correlation,
     which is usually fastest for a moderate amount of moderately sized peaks per frame.
 
     .. note::
@@ -82,60 +88,71 @@
     ----------
     pattern : MatchPattern
         Pattern to correlate with.
     frames : np.ndarray
         Frame data. Currently, only Real values are supported.
     peaks : np.ndarray
         List of peaks of shape (n_peaks, 2)
+    upsample: Union[bool, int], optional
+        Use DFT upsampling for the refinement step, by default False. Supplying
+        True will choose a reasonable default upsampling factor, while any
+        positive integer > 1 will upsample the correlation peak by this factor.
+        DFT upsampling can provide more accurate center values, especially when
+        peak shifts are small, but does require more computation time.
 
     Returns
     -------
     centers : np.ndarray
         Center positions of shape (n_peaks, 2) and integer dtype.
     refineds : np.ndarray
         Refined center positions of shape (n_peaks, 2) and float dtype.
     heights : np.ndarray
         Peak height in log scaled frame. Shape (n_peaks, ) and float dtype.
     elevations : np.ndarray
         Peak elevation in log scaled frame. Shape (n_peaks, ) and float dtype
 
     Example
     -------
-
-    >>> frames, indices, peaks = libertem.utils.generate.cbed_frame()
+    >>> from libertem_blobfinder.base.utils import cbed_frame
+    >>>
+    >>> frames, indices, peaks = cbed_frame()
     >>> pattern = libertem_blobfinder.common.patterns.RadialGradient(radius=4)
     >>> (centers, refineds, heights, elevations) = process_frames_fast(
     ...     pattern=pattern,
     ...     frames=frames,
     ...     peaks=peaks.astype(np.int32),
     ... )
     >>> assert np.allclose(refineds[0], peaks, atol=0.1)
     '''
+
     crop_size = pattern.get_crop_size()
     template = pattern.get_template(sig_shape=(2 * crop_size, 2 * crop_size))
 
-    centers = np.zeros((len(frames), len(peaks), 2), dtype=np.uint16)
+    centers = np.zeros((len(frames), len(peaks), 2), dtype=np.int16)
     refineds = np.zeros((len(frames), len(peaks), 2), dtype=np.float32)
     heights = np.zeros((len(frames), len(peaks)), dtype=np.float32)
     elevations = np.zeros((len(frames), len(peaks)), dtype=np.float32)
 
-    crop_bufs = base.correlation.allocate_crop_bufs(crop_size, len(peaks), frames.dtype)
+    crop_bufs = correlation.allocate_crop_bufs(crop_size, len(peaks), frames.dtype)
 
     for i, f in enumerate(frames):
-        base.correlation.process_frame_fast(
+        correlation.process_frame_fast(
             template=template, crop_size=crop_size,
             frame=f, peaks=peaks.astype(np.int32),
             out_centers=centers[i], out_refineds=refineds[i],
             out_heights=heights[i], out_elevations=elevations[i],
-            crop_bufs=crop_bufs
+            crop_bufs=crop_bufs, upsample=upsample,
         )
     return (centers, refineds, heights, elevations)
 
 
-def process_frames_full(pattern: MatchPattern, frames, peaks):
+def process_frames_full(
+    pattern: MatchPattern, frames, peaks,
+    upsample: Union[bool, int] = False
+):
     '''
     Find the parameters of peaks in a diffraction pattern by correlation with a match pattern.
 
     This method crops regions of interest around the peaks after correlation,
     which can be faster for many peaks on smaller frames.
 
     .. note::
@@ -147,14 +164,20 @@
     ----------
     pattern : MatchPattern
         Pattern to correlate with.
     frame : np.ndarray
         Frame data. Currently, only real values are supported.
     peaks : np.ndarray
         List of peaks of shape (n_peaks, 2)
+    upsample: Union[bool, int], optional
+        Use DFT upsampling for the refinement step, by default False. Supplying
+        True will choose a reasonable default upsampling factor, while any
+        positive integer > 1 will upsample the correlation peak by this factor.
+        DFT upsampling can provide more accurate center values, especially when
+        peak shifts are small, but does require more computation time.
 
     Returns
     -------
     centers : np.ndarray
         Center positions of shape (n_peaks, 2) and integer dtype.
     refineds : np.ndarray
         Refined center positions of shape (n_peaks, 2) and float dtype.
@@ -162,15 +185,17 @@
         Peak height in log scaled frame. Shape (n_peaks, ) and float dtype.
     elevations : np.ndarray
         Peak elevation in log scaled frame. Shape (n_peaks, ) and float dtype
 
     Example
     -------
 
-    >>> frames, indices, peaks = libertem.utils.generate.cbed_frame(radius=4)
+    >>> from libertem_blobfinder.base.utils import cbed_frame
+    >>>
+    >>> frames, indices, peaks = cbed_frame(radius=4)
     >>> pattern = libertem_blobfinder.common.patterns.RadialGradient(radius=4)
     >>> (centers, refineds, heights, elevations) = process_frames_full(
     ...     pattern=pattern,
     ...     frames=frames,
     ...     peaks=peaks.astype(np.int32)
     ... )
     >>> assert np.allclose(refineds[0], peaks, atol=0.1)
@@ -179,20 +204,20 @@
     template = pattern.get_template(sig_shape=frames[0].shape)
 
     centers = np.zeros((len(frames), len(peaks), 2), dtype=np.uint16)
     refineds = np.zeros((len(frames), len(peaks), 2), dtype=np.float32)
     heights = np.zeros((len(frames), len(peaks)), dtype=np.float32)
     elevations = np.zeros((len(frames), len(peaks)), dtype=np.float32)
 
-    frame_buf = base.correlation.zeros(frames[0].shape, dtype=np.float32)
+    frame_buf = correlation.zeros(frames[0].shape, dtype=np.float32)
 
-    buf_count = base.correlation.get_buf_count(crop_size, len(peaks), frame_buf.dtype)
+    buf_count = correlation.get_buf_count(crop_size, len(peaks), frame_buf.dtype)
 
     for i, f in enumerate(frames):
-        base.correlation.process_frame_full(
+        correlation.process_frame_full(
             template=template, crop_size=crop_size,
             frame=f, peaks=peaks.astype(np.int32),
             out_centers=centers[i], out_refineds=refineds[i],
             out_heights=heights[i], out_elevations=elevations[i],
-            frame_buf=frame_buf, buf_count=buf_count
+            frame_buf=frame_buf, buf_count=buf_count, upsample=upsample,
         )
     return (centers, refineds, heights, elevations)
```

### Comparing `libertem-blobfinder-0.5.0/src/libertem_blobfinder/common/patterns.py` & `libertem_blobfinder-0.6.0/src/libertem_blobfinder/common/patterns.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
+from typing import Tuple
 
-import libertem.masks as masks
-
-from libertem_blobfinder.base.correlation import fft
+from libertem_blobfinder.base import masks
+from skimage.util import crop
 
 
 class MatchPattern:
     '''
     Abstract base class for correlation patterns.
 
     This class provides an API to provide a template for fast correlation-based peak finding.
@@ -26,15 +26,15 @@
     def get_crop_size(self):
         return int(np.ceil(self.search))
 
     def get_mask(self, sig_shape):
         raise NotImplementedError
 
     def get_template(self, sig_shape):
-        return fft.rfft2(self.get_mask(sig_shape))
+        return np.fft.rfft2(self.get_mask(sig_shape))
 
 
 class Circular(MatchPattern):
     '''
     Circular pattern with radius :code:`radius`.
 
     This pattern is useful for constructing feature vectors using
@@ -51,14 +51,19 @@
             Radius of the circular pattern in px
         search : float, optional
             Range from the center point in px to include in the correlation, 2x radius by default.
             Defining the size of the square correlation pattern.
         '''
         if search is None:
             search = 2*radius
+        if search < radius:
+            raise ValueError(
+                f"search {search} < radius {radius}, "
+                "search must contain the pattern."
+            )
         self.radius = radius
         super().__init__(search=search)
 
     def get_mask(self, sig_shape):
         return masks.circular(
             centerY=sig_shape[0] // 2,
             centerX=sig_shape[1] // 2,
@@ -84,14 +89,19 @@
             Radius of the circular pattern in px
         search : float, optional
             Range from the center point in px to include in the correlation, 2x radius by default.
             Defining the size of the square correlation pattern.
         '''
         if search is None:
             search = 2*radius
+        if search < radius:
+            raise ValueError(
+                f"search {search} < radius {radius}, "
+                "search must contain the pattern."
+            )
         self.radius = radius
         super().__init__(search=search)
 
     def get_mask(self, sig_shape):
         return masks.radial_gradient(
             centerY=sig_shape[0] // 2,
             centerX=sig_shape[1] // 2,
@@ -122,14 +132,21 @@
         radius_outer : float, optional
             Radius of the negative region in px. 1.5x radius by default.
         '''
         if radius_outer is None:
             radius_outer = radius * 1.5
         if search is None:
             search = max(2*radius, radius_outer)
+        if radius_outer <= radius:
+            raise ValueError(f"radius_outer {radius_outer} <= radius {radius}, must be larger.")
+        if search < radius_outer:
+            raise ValueError(
+                f"search {search} < radius_outer {radius_outer}, "
+                "search must contain the pattern."
+            )
         self.radius = radius
         self.radius_outer = radius_outer
         super().__init__(search=search)
 
     def get_mask(self, sig_shape):
         return masks.background_subtraction(
             centerY=sig_shape[0] // 2,
@@ -142,15 +159,15 @@
         )
 
 
 class UserTemplate(MatchPattern):
     '''
     User-defined template
     '''
-    def __init__(self, template, search=None):
+    def __init__(self, template: np.ndarray, search=None):
         '''
         Parameters
         ----------
 
         template : numpy.ndarray
             Correlation template as 2D numpy.ndarray
         search : float, optional
@@ -160,51 +177,55 @@
         '''
         if search is None:
             # Half diagonal
             search = np.sqrt(template.shape[0]**2 + template.shape[1]**2) / 2
         self.template = template
         super().__init__(search=search)
 
-    def get_mask(self, sig_shape):
-        result = np.zeros((sig_shape), dtype=self.template.dtype)
-        dy, dx = sig_shape
-        ty, tx = self.template.shape
-
-        left = dx / 2 - tx / 2
-        top = dy / 2 - ty / 2
-
-        r_left = max(0, left)
-        r_top = max(0, top)
-
-        t_left = max(0, -left)
-        t_top = max(0, -top)
-
-        crop_x = r_left - left
-        crop_y = r_top - top
-
-        h = int(ty - 2*crop_y)
-        w = int(tx - 2*crop_x)
-
-        r_left = int(r_left)
-        r_top = int(r_top)
-        t_left = int(t_left)
-        t_top = int(t_top)
-
-        result[r_top:r_top + h, r_left:r_left + w] = \
-            self.template[t_top:t_top + h, t_left:t_left + w]
-        return result
+    def get_mask(self, sig_shape: Tuple[int, int]) -> np.ndarray:
+        # Pad or Crop each dimension of self.template to
+        # match sig_shape at the ouput. For odd pads/crops
+        # the extra pixel is added/removed at the end of the axis
+        result = self.template.copy()
+        neutral = (0, 0)
+        for ax, (target, source) in enumerate(zip(sig_shape, self.template.shape)):
+            if target > source:
+                extra = target - source
+                fn = np.pad
+            elif target < source:
+                extra = source - target
+                fn = crop
+            else:
+                continue
+            before = after = extra // 2
+            if (before + after) != extra:
+                # In the default case sig_shape is always even (2 * crop_size)
+                # so this path implies the template has an odd dimension.
+                # therefore a choice here of how to centre the array
+                # before += 1
+                after += 1
+            result = fn(
+                result,
+                tuple(
+                    (before, after) if ax == i else neutral
+                    for i in range(result.ndim)
+                )
+            )
+        assert result.shape == tuple(sig_shape)
+        return result.astype(self.template.dtype)
 
 
 class RadialGradientBackgroundSubtraction(UserTemplate):
     '''
     Combination of radial gradient with background subtraction
     '''
     def __init__(self, radius, search=None, radius_outer=None, delta=1, radial_map=None):
         '''
-        See :meth:`~libertem.masks.radial_gradient_background_subtraction` for details.
+        See :meth:`~libertem_blobfinder.base.masks.radial_gradient_background_subtraction`
+        for details.
 
         Parameters
         ----------
 
         radius : float
             Radius of the circular pattern in px
         search : float, optional
@@ -214,22 +235,22 @@
         radius_outer : float, optional
             Radius of the negative region in px. 1.5x radius by default.
         delta : float, optional
             Width of the transition region between positive and negative in px
         radial_map : numpy.ndarray, optional
             Radius value of each pixel in px. This can be used to distort the shape as needed
             or work in physical coordinates instead of pixels.
-            A suitable map can be generated with :meth:`libertem.masks.polar_map`.
+            A suitable map can be generated with :meth:`libertem_blobfinder.base.masks.polar_map`.
 
         Example
         -------
 
         >>> import matplotlib.pyplot as plt
 
-        >>> (radius, phi) = libertem.masks.polar_map(
+        >>> (radius, phi) = libertem_blobfinder.base.masks.polar_map(
         ...     centerX=64, centerY=64,
         ...     imageSizeX=128, imageSizeY=128,
         ...     stretchY=2., angle=np.pi/4
         ... )
 
         >>> template = RadialGradientBackgroundSubtraction(
         ...     radius=30, radial_map=radius)
@@ -240,14 +261,21 @@
         <matplotlib.image.AxesImage object at ...>
         >>> plt.show() # doctest: +SKIP
         '''
         if radius_outer is None:
             radius_outer = radius * 1.5
         if search is None:
             search = max(2*radius, radius_outer)
+        if radius_outer <= radius:
+            raise ValueError(f"radius_outer {radius_outer} <= radius {radius}, must be larger.")
+        if search < radius_outer:
+            raise ValueError(
+                f"search {search} < radius_outer {radius_outer}, "
+                "search must contain the pattern."
+            )
         if radial_map is None:
             r = max(radius, radius_outer)
             radial_map, _ = masks.polar_map(
                 centerX=r + 1,
                 centerY=r + 1,
                 imageSizeX=int(np.ceil(2*r + 2)),
                 imageSizeY=int(np.ceil(2*r + 2)),
```

### Comparing `libertem-blobfinder-0.5.0/src/libertem_blobfinder/udf/correlation.py` & `libertem_blobfinder-0.6.0/src/libertem_blobfinder/udf/correlation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import functools
 
 import numpy as np
+import sparseconverter
 
 from libertem.udf import UDF
-import libertem.masks as masks
 from libertem.common.container import MaskContainer
 
+from libertem_blobfinder.base import masks
 from libertem_blobfinder.common.patterns import MatchPattern
 import libertem_blobfinder.base.correlation as ltbc
 from libertem_blobfinder.common.correlation import get_peaks
 
 
 class CorrelationUDF(UDF):
     '''
@@ -29,29 +30,31 @@
         super().__init__(peaks=np.round(peaks).astype(int), zero_shift=zero_shift, *args, **kwargs)
 
     def get_result_buffers(self):
         '''
         The common buffers for all correlation methods.
 
         :code:`centers`:
-            (y, x) integer positions.
+            (y, x) integer positions. NOTE: the returned positions
+            can be out-of-frame and the user should perform bounds
+            checking if directly indexing into the frame array.
         :code:`refineds`:
             (y, x) positions with subpixel refinement.
         :code:`peak_values`:
             Peak height in the log scaled frame.
         :code:`peak_elevations`:
             Peak quality (result of :meth:`peak_elevation`).
 
         See source code for details of the buffer declaration.
         '''
         num_disks = len(self.params.peaks)
 
         return {
             'centers': self.buffer(
-                kind="nav", extra_shape=(num_disks, 2), dtype="u2"
+                kind="nav", extra_shape=(num_disks, 2), dtype=np.int32,
             ),
             'refineds': self.buffer(
                 kind="nav", extra_shape=(num_disks, 2), dtype="float32"
             ),
             'peak_values': self.buffer(
                 kind="nav", extra_shape=(num_disks,), dtype="float32",
             ),
@@ -102,34 +105,51 @@
         peaks : numpy.ndarray
             Numpy array of (y, x) coordinates with peak positions in px to correlate
         match_pattern : MatchPattern
             Instance of :class:`~libertem_blobfinder.MatchPattern`
         zero_shift : Union[AUXBufferWrapper, numpy.ndarray, None], optional
             Zero shift, for example descan error. Can be :code:`None`, :code:`numpy.array((y, x))`
             or AUX data with :code:`(y, x)` for each frame.
+        upsample: Union[bool, int], optional
+            Use DFT upsampling for the refinement step, by default False. Supplying
+            True will choose a reasonable default upsampling factor, while any
+            positive integer > 1 will upsample the correlation peak by this factor.
+            DFT upsampling can provide more accurate center values, especially when
+            peak shifts are small, but does require more computation time.
         '''
         # For testing purposes, allow to inject a different limit via
         # an internal kwarg
         # It has to come through kwarg because of how UDFs are run
         self.limit = kwargs.get('__limit', 2**19)  # 1/2 MB
         super().__init__(
             peaks=peaks, match_pattern=match_pattern, zero_shift=zero_shift, *args, **kwargs
         )
 
     def get_task_data(self):
         ""
         n_peaks = len(self.get_peaks())
         mask = self.get_pattern()
         crop_size = mask.get_crop_size()
-        template = mask.get_template(sig_shape=(2 * crop_size, 2 * crop_size))
+        template = self.xp.array(mask.get_template(sig_shape=(2 * crop_size, 2 * crop_size)))
         dtype = np.result_type(self.meta.input_dtype, np.float32)
-        crop_bufs = ltbc.allocate_crop_bufs(crop_size, n_peaks, dtype=dtype, limit=self.limit)
+        crop_bufs = ltbc.allocate_crop_bufs(
+            crop_size, n_peaks, dtype=dtype, limit=self.limit, xp=self.xp
+        )
+        if self.meta.array_backend in (
+                self.BACKEND_SPARSE_COO, self.BACKEND_SPARSE_GCXS, self.BACKEND_CUPY):
+            crop_function = ltbc.crop_disks_from_frame_slicing
+        elif self.meta.array_backend in (self.BACKEND_NUMPY, ):
+            crop_function = ltbc.crop_disks_from_frame
+        else:  # pragma: no cover
+            raise RuntimeError(f"Unsupported array backend {self.meta.array_backend}")
+
         kwargs = {
             'crop_bufs': crop_bufs,
             'template': template,
+            'crop_function': crop_function,
         }
         return kwargs
 
     def get_pattern(self):
         return self.params.match_pattern
 
     def get_template(self):
@@ -139,15 +159,25 @@
         match_pattern = self.get_pattern()
         (centers, refineds, peak_values, peak_elevations) = self.output_buffers()
         ltbc.process_frame_fast(
             template=self.get_template(), crop_size=match_pattern.get_crop_size(),
             frame=frame, peaks=self.get_peaks() + np.round(self.get_zero_shift()).astype(int),
             out_centers=centers, out_refineds=refineds,
             out_heights=peak_values, out_elevations=peak_elevations,
-            crop_bufs=self.task_data.crop_bufs
+            crop_bufs=self.task_data.crop_bufs,
+            upsample=self.params.get('upsample', False),
+            crop_function=self.task_data.crop_function,
+        )
+
+    def get_backends(self):
+        return (
+            self.BACKEND_NUMPY,
+            self.BACKEND_CUPY,
+            self.BACKEND_SPARSE_COO,
+            self.BACKEND_SPARSE_GCXS,
         )
 
 
 class FullFrameCorrelationUDF(CorrelationUDF):
     '''
     Fourier-based correlation-based refinement of peak positions within a search
     frame for each peak using a single correlation step. This can be faster for
@@ -165,36 +195,54 @@
         peaks : numpy.ndarray
             Numpy array of (y, x) coordinates with peak positions in px to correlate
         match_pattern : MatchPattern
             Instance of :class:`~libertem_blobfinder.MatchPattern`
         zero_shift : Union[AUXBufferWrapper, numpy.ndarray, None], optional
             Zero shift, for example descan error. Can be :code:`None`, :code:`numpy.array((y, x))`
             or AUX data with :code:`(y, x)` for each frame.
+        upsample: Union[bool, int], optional
+            Use DFT upsampling for the refinement step, by default False. Supplying
+            True will choose a reasonable default upsampling factor, while any
+            positive integer > 1 will upsample the correlation peak by this factor.
+            DFT upsampling can provide more accurate center values, especially when
+            peak shifts are small, but does require more computation time.
         '''
         # For testing purposes, allow to inject a different limit via
         # an internal kwarg
         # It has to come through kwarg because of how UDFs are run
         self.limit = kwargs.get('__limit', 2**19)  # 1/2 MB
 
         super().__init__(
             peaks=peaks, match_pattern=match_pattern, zero_shift=zero_shift, *args, **kwargs
         )
 
     def get_task_data(self):
         ""
         mask = self.get_pattern()
         n_peaks = len(self.params.peaks)
-        template = mask.get_template(sig_shape=self.meta.dataset_shape.sig)
+        template = self.xp.array(mask.get_template(sig_shape=self.meta.dataset_shape.sig))
         dtype = np.result_type(self.meta.input_dtype, np.float32)
-        frame_buf = ltbc.zeros(shape=self.meta.dataset_shape.sig, dtype=dtype)
+        frame_buf = self.xp.array(
+            ltbc.zeros(shape=self.meta.dataset_shape.sig, dtype=dtype)
+        )
         crop_size = mask.get_crop_size()
+
+        if self.meta.array_backend in (
+                self.BACKEND_SPARSE_COO, self.BACKEND_SPARSE_GCXS, self.BACKEND_CUPY):
+            crop_function = ltbc.crop_disks_from_frame_slicing
+        elif self.meta.array_backend in (self.BACKEND_NUMPY, ):
+            crop_function = ltbc.crop_disks_from_frame
+        else:  # pragma: no cover
+            raise RuntimeError(f"Unsupported array backend {self.meta.array_backend}")
+
         kwargs = {
             'template': template,
             'frame_buf': frame_buf,
             'buf_count': ltbc.get_buf_count(crop_size, n_peaks, dtype, self.limit),
+            'crop_function': crop_function,
         }
         return kwargs
 
     def get_pattern(self):
         return self.params.match_pattern
 
     def get_template(self):
@@ -210,14 +258,24 @@
             peaks=self.get_peaks() + np.round(self.get_zero_shift()).astype(int),
             out_centers=centers,
             out_refineds=refineds,
             out_heights=peak_values,
             out_elevations=peak_elevations,
             frame_buf=self.task_data.frame_buf,
             buf_count=self.task_data.buf_count,
+            upsample=self.params.get('upsample', False),
+            crop_function=self.task_data.crop_function,
+        )
+
+    def get_backends(self):
+        # At this time cannot FFT on a full sparse frame so not
+        # specifying sparse backends to trigger auto-densification
+        return (
+            self.BACKEND_NUMPY,
+            self.BACKEND_CUPY,
         )
 
 
 class SparseCorrelationUDF(CorrelationUDF):
     '''
     Direct correlation using sparse matrices
 
@@ -281,35 +339,45 @@
             mask_index=range(len(offsetY)),
             offsetX=offsetX,
             offsetY=offsetY,
             template=template,
             imageSizeX=self.meta.dataset_shape.sig[1],
             imageSizeY=self.meta.dataset_shape.sig[0]
         )
+        if self.meta.array_backend in sparseconverter.CPU_BACKENDS:
+            backend = 'numpy'
+        elif self.meta.array_backend in sparseconverter.CUDA_BACKENDS:
+            backend = 'cupy'
+        else:  # pragma: no cover
+            raise ValueError("Unknown device class")
+        if self.meta.array_backend == self.BACKEND_SPARSE_COO:
+            use_sparse = 'sparse.pydata'
+        elif self.meta.array_backend == self.BACKEND_SPARSE_GCXS:
+            use_sparse = 'sparse.pydata.GCXS'
+        elif self.meta.array_backend in (self.BACKEND_CUPY, self.BACKEND_NUMPY):
+            use_sparse = 'scipy.sparse.csc'
+        else:  # pragma: no cover
+            raise RuntimeError(f'Unsupported array backend {self.meta.array_backend}')
         # CSC matrices in combination with transposed data are fastest
         container = MaskContainer(mask_factories=stack, dtype=np.float32,
-            use_sparse='scipy.sparse.csc')
+            use_sparse=use_sparse, backend=backend)
 
         kwargs = {
             'mask_container': container,
             'crop_size': crop_size,
         }
         return kwargs
 
     def process_tile(self, tile):
         tile_slice = self.meta.slice
         c = self.task_data.mask_container
-        tile_t = np.zeros(
-            (np.prod(tile.shape[1:]), tile.shape[0]),
-            dtype=tile.dtype
-        )
-        ltbc.log_scale(tile.reshape((tile.shape[0], -1)).T, out=tile_t)
+        tile_t = ltbc.log_scale(tile.reshape((tile.shape[0], -1)).T, out=None)
 
         sl = c.get(key=tile_slice, transpose=False)
-        self.results.corr[:] += sl.dot(tile_t).T
+        self.results.corr[:] += self.forbuf(sl.dot(tile_t).T, self.results.corr)
 
     def postprocess(self):
         """
         The correlation results are evaluated during postprocessing since this
         implementation uses tiled processing where the correlations are
         incomplete in :meth:`process_tile`.
         """
@@ -325,68 +393,92 @@
         for f in range(corrmaps.shape[0]):
             ltbc.evaluate_correlations(
                 corrs=corrmaps[f], peaks=peaks, crop_size=self.params.steps,
                 out_centers=centers[f], out_refineds=refineds[f],
                 out_heights=peak_values[f], out_elevations=peak_elevations[f]
             )
 
+    def get_backends(self):
+        return (
+            self.BACKEND_NUMPY,
+            self.BACKEND_CUPY,
+            self.BACKEND_SPARSE_COO,
+            self.BACKEND_SPARSE_GCXS
+        )
+
 
 def run_fastcorrelation(
-        ctx, dataset, peaks, match_pattern: MatchPattern, zero_shift=None, **kwargs):
+    ctx, dataset, peaks, match_pattern: MatchPattern, zero_shift=None, upsample=False, **kwargs
+):
     """
     Wrapper function to construct and run a :class:`FastCorrelationUDF`
 
     Parameters
     ----------
     ctx : libertem.api.Context
     dataset : libertem.io.dataset.base.DataSet
     peaks : numpy.ndarray
         List of peaks with (y, x) coordinates
     match_pattern : libertem_blobfinder.patterns.MatchPattern
     zero_shift : Union[AUXBufferWrapper, numpy.ndarray, None], optional
         Zero shift, for example descan error. Can be :code:`None`, :code:`numpy.array((y, x))`
         or AUX data with :code:`(y, x)` for each frame.
+    upsample : Union[bool, int], optional
+        Whether to use upsampling DFT for refinement. False to deactivate (default) or a positive
+        integer >1 to upsample by this factor when refining the correlation peak positions. Upsample
+        True will choose a sensible upsampling factor.
     kwargs : passed through to :meth:`~libertem.api.Context.run_udf`
 
     Returns
     -------
     buffers : Dict[libertem.common.buffers.BufferWrapper]
         See :meth:`CorrelationUDF.get_result_buffers` for details.
     """
     peaks = peaks.astype(int)
-    udf = FastCorrelationUDF(peaks=peaks, match_pattern=match_pattern, zero_shift=zero_shift)
+    udf = FastCorrelationUDF(
+        peaks=peaks, match_pattern=match_pattern, zero_shift=zero_shift, upsample=upsample,
+    )
     return ctx.run_udf(dataset=dataset, udf=udf, **kwargs)
 
 
-def run_blobfinder(ctx, dataset, match_pattern: MatchPattern, num_peaks, roi=None, progress=False):
+def run_blobfinder(
+    ctx, dataset, match_pattern: MatchPattern, num_peaks, roi=None, upsample=False, progress=False
+):
     """
     Wrapper function to find peaks in a dataset and refine their position using
     :class:`FastCorrelationUDF`
 
     Parameters
     ----------
     ctx : libertem.api.Context
     dataset : libertem.io.dataset.base.DataSet
     match_pattern : libertem_blobfinder.patterns.MatchPattern
     num_peaks : int
         Number of peaks to look for
     roi : numpy.ndarray, optional
         Boolean mask of the navigation dimension to select region of interest (ROI)
+    upsample : Union[bool, int], optional
+        Whether to use upsampling DFT for refinement. False to deactivate (default) or a positive
+        integer >1 to upsample by this factor when refining the correlation peak positions. Upsample
+        True will choose a sensible upsampling factor.
     progress : bool, optional
         Show progress bar
 
     Returns
     -------
     sum_result : numpy.ndarray
         Log-scaled sum frame of the dataset/ROI
     centers, refineds, peak_values, peak_elevations : libertem.common.buffers.BufferWrapper
         See :meth:`CorrelationUDF.get_result_buffers` for details.
     peaks : numpy.ndarray
         List of found peaks with (y, x) coordinates
     """
+    if upsample is True:
+        upsample = 20
+
     sum_analysis = ctx.create_sum_analysis(dataset=dataset)
     sum_result = ctx.run(sum_analysis, roi=roi)
 
     sum_result = ltbc.log_scale(sum_result.intensity.raw_data, out=None)
     peaks = get_peaks(
         sum_result=sum_result,
         match_pattern=match_pattern,
@@ -395,13 +487,14 @@
 
     pass_2_results = run_fastcorrelation(
         ctx=ctx,
         dataset=dataset,
         peaks=peaks,
         match_pattern=match_pattern,
         roi=roi,
+        upsample=upsample,
         progress=progress
     )
 
     return (sum_result, pass_2_results['centers'],
         pass_2_results['refineds'], pass_2_results['peak_values'],
         pass_2_results['peak_elevations'], peaks)
```

### Comparing `libertem-blobfinder-0.5.0/src/libertem_blobfinder/udf/integration.py` & `libertem_blobfinder-0.6.0/src/libertem_blobfinder/udf/integration.py`

 * *Files identical despite different names*

### Comparing `libertem-blobfinder-0.5.0/src/libertem_blobfinder/udf/refinement.py` & `libertem_blobfinder-0.6.0/src/libertem_blobfinder/udf/refinement.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import numpy as np
-from libertem.utils import frame_peaks
 
-import libertem.analysis.gridmatching as grm
+from libertem_blobfinder.base.utils import frame_peaks
+import libertem_blobfinder.common.gridmatching as grm
 
 from libertem_blobfinder.common.patterns import MatchPattern
-from libertem_blobfinder.udf.correlation import FastCorrelationUDF,\
-    SparseCorrelationUDF, FullFrameCorrelationUDF
+from libertem_blobfinder.udf.correlation import (
+    FastCorrelationUDF, SparseCorrelationUDF, FullFrameCorrelationUDF
+)
 
 
 class RefinementMixin():
     '''
     To be combined with a :class:`libertem_blobfinder.CorrelationUDF`
     using multiple inheritance.
 
@@ -74,23 +75,23 @@
         r.b[index] = match.b
         r.selector[index] = match.selector
         r.error[index] = match.error
 
 
 class FastmatchMixin(RefinementMixin):
     '''
-    Refinement using :meth:`~libertem.analysis.gridmatching.Matcher.fastmatch`
+    Refinement using :meth:`~libertem_blobfinder.common.gridmatching.Matcher.fastmatch`
     '''
     def __init__(self, *args, **kwargs):
         '''
         Parameters
         ----------
 
-        matcher : libertem.analysis.gridmatching.Matcher
-            Instance of :class:`~libertem.analysis.gridmatching.Matcher`
+        matcher : libertem_blobfinder.common.gridmatching.Matcher
+            Instance of :class:`~libertem_blobfinder.common.gridmatching.Matcher`
         start_zero : numpy.ndarray
             Approximate value (y, x) in px for "zero" point (origin, zero order peak)
         start_a : numpy.ndarray
             Approximate value (y, x) in px for "a" vector.
         start_b : numpy.ndarray
             Approximate value (y, x) in px for "b" vector.
         '''
@@ -111,28 +112,28 @@
                 b=p.start_b,
             )
             self.apply_match(index, match)
 
 
 class AffineMixin(RefinementMixin):
     '''
-    Refinement using :meth:`~libertem.analysis.gridmatching.Matcher.affinematch`
+    Refinement using :meth:`~libertem_blobfinder.common.gridmatching.Matcher.affinematch`
     '''
     def __init__(self, *args, **kwargs):
         '''
         Parameters
         ----------
 
-        matcher : libertem.analysis.gridmatching.Matcher
-            Instance of :class:`~libertem.analysis.gridmatching.Matcher`
+        matcher : libertem_blobfinder.common.gridmatching.Matcher
+            Instance of :class:`~libertem_blobfinder.common.gridmatching.Matcher`
         indices : numpy.ndarray
             List of indices [(h1, k1), (h2, k2), ...] of all peaks. The indices can be
             non-integer and relative to any base vectors, including virtual ones like
             (1, 0); (0, 1). See documentation of
-            :meth:`~libertem.analysis.gridmatching.Matcher.affinematch` for details.
+            :meth:`~libertem_blobfinder.common.gridmatching.Matcher.affinematch` for details.
         '''
         super().__init__(*args, **kwargs)
 
     def postprocess(self):
         super().postprocess()
         p = self.params
         r = self.results
@@ -145,15 +146,16 @@
                 indices=p.indices,
             )
             self.apply_match(index, match)
 
 
 def run_refine(
         ctx, dataset, zero, a, b, match_pattern: MatchPattern, matcher: grm.Matcher,
-        correlation='fast', match='fast', indices=None, steps=5, zero_shift=None, **kwargs):
+        correlation='fast', match='fast', indices=None, steps=5, zero_shift=None,
+        upsample=False, **kwargs):
     '''
     Wrapper function to refine the given lattice for each frame by calculating
     approximate peak positions and refining them for each frame using a
     combination of :class:`libertem_blobfinder.CorrelationUDF` and
     :class:`libertem_blobfinder.RefinementMixin`.
 
     .. versionchanged:: 0.3.0
@@ -172,16 +174,17 @@
         peak)
     a : numpy.ndarray
         Approximate value for "a" vector (y, x) in px.
     b : numpy.ndarray
         Approximate value for "b" vector (y, x) in px.
     match_pattern : MatchPattern
         Instance of :class:`~MatchPattern`
-    matcher : libertem.analysis.gridmatching.Matcher
-        Instance of :class:`~libertem.analysis.gridmatching.Matcher` to perform the matching
+    matcher : libertem_blobfinder.common.gridmatching.Matcher
+        Instance of :class:`~libertem_blobfinder.common.gridmatching.Matcher`
+        to perform the matching
     correlation : {'fast', 'sparse', 'fullframe'}, optional
         'fast', 'sparse' or 'fullframe' to select :class:`~FastCorrelationUDF`,
         :class:`~SparseCorrelationUDF` or :class:`~FullFrameCorrelationUDF`
     match : {'fast', 'affine'}, optional
         'fast' or 'affine' to select
         :class:`~FastmatchMixin` or :class:`~AffineMixin`
     indices : numpy.ndarray, optional
@@ -195,14 +198,20 @@
         Only for correlation == 'sparse': Correlation steps. See
         :meth:`~SparseCorelationUDF.__init__` for
         details.
     zero_shift : Union[AUXBufferWrapper, numpy.ndarray, None], optional
         Zero shift, for example descan error. Can be :code:`None`, :code:`numpy.array((y, x))`
         or AUX data with :code:`(y, x)` for each frame. Only supported for correlation methods
         :code:`fast` and `fullframe`.
+    upsample: Union[bool, int], optional
+        Use DFT upsampling for the refinement step, by default False. Supplying
+        True will choose a reasonable default upsampling factor, while any
+        positive integer > 1 will upsample the correlation peak by this factor.
+        DFT upsampling can provide more accurate center values, especially when
+        peak shifts are small, but does require more computation time.
     kwargs : passed through to :meth:`~libertem.api.Context.run_udf`
 
     Returns
     -------
     result : Dict[str, BufferWrapper]
         Result buffers of the UDF. See
         :meth:`libertem_blobfinder.correlation.CorrelationUDF.get_result_buffers` and
@@ -226,14 +235,17 @@
     ... )
     >>> result['centers'].data  #doctest: +ELLIPSIS
     array(...)
     '''
     if indices is None:
         indices = np.mgrid[-10:11, -10:11]
 
+    if upsample is True:
+        upsample = 20
+
     (fy, fx) = tuple(dataset.shape.sig)
 
     indices, peaks = frame_peaks(
         fy=fy, fx=fx, zero=zero, a=a, b=b,
         r=match_pattern.search, indices=indices
     )
     peaks = peaks.astype('int')
@@ -269,14 +281,15 @@
         start_zero=zero,
         start_a=a,
         start_b=b,
         match_pattern=match_pattern,
         matcher=matcher,
         steps=steps,
         zero_shift=zero_shift,
+        upsample=upsample,
     )
 
     result = ctx.run_udf(
         dataset=dataset,
         udf=udf,
         **kwargs
     )
```

### Comparing `libertem-blobfinder-0.5.0/src/libertem_blobfinder/udf/utils.py` & `libertem_blobfinder-0.6.0/src/libertem_blobfinder/udf/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import matplotlib.pyplot as plt
 
-import libertem.analysis.gridmatching as grm
+import libertem_blobfinder.common.gridmatching as grm
 
 
 def visualize_frame(ctx, ds, result, indices, r, y, x, axes, colors=None, stretch=10):
     '''
     Visualize the refinement of a specific frame in matplotlib axes
     '''
     # Get the frame from the dataset
```

### Comparing `libertem-blobfinder-0.5.0/tests/test_common.py` & `libertem_blobfinder-0.6.0/tests/test_common.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,42 @@
-import functools
-
 import numpy as np
 import pytest
 
-import libertem.masks as m
-from libertem.utils.generate import cbed_frame
-from libertem.io.dataset.memory import MemoryDataSet
-from libertem.udf.masks import ApplyMasksUDF
-
-from libertem_blobfinder import common
-import libertem_blobfinder.common.correlation
-import libertem_blobfinder.common.patterns
-import libertem_blobfinder.udf.refinement  # noqa F401
+import libertem_blobfinder.base.masks as m
+from libertem_blobfinder.common import patterns, correlation
+from libertem_blobfinder.base.utils import cbed_frame
+
+
+def test_circular_limits():
+    with pytest.raises(ValueError):
+        patterns.Circular(radius=5, search=4)
+
+
+def test_radial_gradient_limits():
+    with pytest.raises(ValueError):
+        patterns.RadialGradient(radius=5, search=4)
+
+
+def test_background_subtraction_limits():
+    with pytest.raises(ValueError):
+        patterns.BackgroundSubtraction(radius=5, search=4, radius_outer=6)
+    with pytest.raises(ValueError):
+        patterns.BackgroundSubtraction(radius=5, search=13, radius_outer=5)
+
+
+def test_radial_background_subtraction_limits():
+    with pytest.raises(ValueError):
+        patterns.RadialGradientBackgroundSubtraction(radius=5, search=4, radius_outer=6)
+    with pytest.raises(ValueError):
+        patterns.RadialGradientBackgroundSubtraction(radius=5, search=13, radius_outer=5)
 
 
 def test_custom_template():
     template = m.radial_gradient(centerX=10, centerY=10, imageSizeX=21, imageSizeY=23, radius=7)
-    custom = common.patterns.UserTemplate(template=template, search=18)
+    custom = patterns.UserTemplate(template=template, search=18)
 
     assert custom.get_crop_size() == 18
 
     same = custom.get_mask((23, 21))
     larger = custom.get_mask((25, 23))
     smaller = custom.get_mask((10, 10))
 
@@ -54,67 +70,19 @@
         print("mask_x:", mask_x)
 
         template = m.radial_gradient(
             centerX=center_x, centerY=center_y,
             imageSizeX=size_x, imageSizeY=size_y,
             radius=radius
         )
-        custom = common.patterns.UserTemplate(template=template, search=search)
+        custom = patterns.UserTemplate(template=template, search=search)
 
         mask = custom.get_mask((mask_y, mask_x))  # noqa
 
 
-def test_featurevector(lt_ctx):
-    shape = np.array([128, 128])
-    zero = shape // 2
-    a = np.array([24, 0.])
-    b = np.array([0., 30])
-    indices = np.mgrid[-2:3, -2:3]
-    indices = np.concatenate(indices.T)
-
-    radius = 5
-    radius_outer = 10
-
-    template = m.background_subtraction(
-        centerX=radius_outer + 1,
-        centerY=radius_outer + 1,
-        imageSizeX=radius_outer*2 + 2,
-        imageSizeY=radius_outer*2 + 2,
-        radius=radius_outer,
-        radius_inner=radius + 1,
-        antialiased=False
-    )
-
-    data, indices, peaks = cbed_frame(*shape, zero, a, b, indices, radius, all_equal=True)
-
-    dataset = MemoryDataSet(data=data, tileshape=(1, *shape),
-                            num_partitions=1, sig_dims=2)
-
-    match_pattern = common.patterns.UserTemplate(template=template)
-
-    stack = functools.partial(
-        common.patterns.feature_vector,
-        imageSizeX=shape[1],
-        imageSizeY=shape[0],
-        peaks=peaks,
-        match_pattern=match_pattern,
-    )
-
-    m_udf = ApplyMasksUDF(
-        mask_factories=stack, mask_count=len(peaks), mask_dtype=np.float32
-    )
-    res = lt_ctx.run_udf(dataset=dataset, udf=m_udf)
-
-    peak_data, _, _ = cbed_frame(*shape, zero, a, b, np.array([(0, 0)]), radius, all_equal=True)
-    peak_sum = peak_data.sum()
-
-    assert np.allclose(res['intensity'].data.sum(), data.sum())
-    assert np.allclose(res['intensity'].data, peak_sum)
-
-
 @pytest.mark.with_numba
 def test_standalone_fast():
     shape = np.array([128, 128])
     zero = shape / 2 + np.random.uniform(-1, 1, size=2)
     a = np.array([34.3, 0.]) + np.random.uniform(-1, 1, size=2)
     b = np.array([0., 42.19]) + np.random.uniform(-1, 1, size=2)
     indices = np.mgrid[-2:3, -2:3]
@@ -129,29 +97,29 @@
         centerY=radius+1,
         imageSizeX=2*radius+2,
         imageSizeY=2*radius+2,
         radius=radius
     )
 
     match_patterns = [
-        common.patterns.RadialGradient(radius=radius, search=radius*1.5),
-        common.patterns.BackgroundSubtraction(
+        patterns.RadialGradient(radius=radius, search=radius*1.5),
+        patterns.BackgroundSubtraction(
             radius=radius, radius_outer=radius*1.5, search=radius*1.8),
-        common.patterns.RadialGradientBackgroundSubtraction(
+        patterns.RadialGradientBackgroundSubtraction(
             radius=radius, radius_outer=radius*1.5, search=radius*1.8),
-        common.patterns.UserTemplate(template=template, search=radius*1.5)
+        patterns.UserTemplate(template=template, search=radius*1.5)
     ]
 
     print("zero: ", zero)
     print("a: ", a)
     print("b: ", b)
 
     for match_pattern in match_patterns:
         print("refining using template %s" % type(match_pattern))
-        (centers, refineds, heights, elevations) = common.correlation.process_frames_fast(
+        (centers, refineds, heights, elevations) = correlation.process_frames_fast(
             pattern=match_pattern,
             frames=data, peaks=peaks.astype(np.int32),
         )
 
         print(peaks - refineds)
 
         assert np.allclose(refineds[0], peaks, atol=0.5)
@@ -175,29 +143,29 @@
         centerY=radius+1,
         imageSizeX=2*radius+2,
         imageSizeY=2*radius+2,
         radius=radius
     )
 
     match_patterns = [
-        common.patterns.RadialGradient(radius=radius, search=radius*1.5),
-        common.patterns.BackgroundSubtraction(
+        patterns.RadialGradient(radius=radius, search=radius*1.5),
+        patterns.BackgroundSubtraction(
             radius=radius, radius_outer=radius*1.5, search=radius*1.8),
-        common.patterns.RadialGradientBackgroundSubtraction(
+        patterns.RadialGradientBackgroundSubtraction(
             radius=radius, radius_outer=radius*1.5, search=radius*1.8),
-        common.patterns.UserTemplate(template=template, search=radius*1.5)
+        patterns.UserTemplate(template=template, search=radius*1.5)
     ]
 
     print("zero: ", zero)
     print("a: ", a)
     print("b: ", b)
 
     for match_pattern in match_patterns:
         print("refining using template %s" % type(match_pattern))
-        (centers, refineds, heights, elevations) = common.correlation.process_frames_full(
+        (centers, refineds, heights, elevations) = correlation.process_frames_full(
             pattern=match_pattern,
             frames=data, peaks=peaks.astype(np.int32),
         )
 
         print(peaks - refineds)
 
         assert np.allclose(refineds[0], peaks, atol=0.5)
```

### Comparing `libertem-blobfinder-0.5.0/tests/test_udf.py` & `libertem_blobfinder-0.6.0/tests/udf/test_udf.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,32 @@
+import functools
 import numpy as np
 import pytest
+from numpy.testing import assert_allclose
 import matplotlib.pyplot as plt
+from sparseconverter import get_device_class
 
-import libertem.analysis.gridmatching as grm
-import libertem.masks as m
-from libertem.utils.generate import cbed_frame
 from libertem.io.dataset.memory import MemoryDataSet
 from libertem.udf.base import UDF
+from libertem.udf.masks import ApplyMasksUDF
+
 
 from libertem_blobfinder import common, udf
+import libertem_blobfinder.common.gridmatching as grm
+import libertem_blobfinder.base.masks as m
+from libertem_blobfinder.base.utils import cbed_frame
 import libertem_blobfinder.common.correlation
 import libertem_blobfinder.common.patterns
 import libertem_blobfinder.udf.refinement
 import libertem_blobfinder.udf.correlation
 import libertem_blobfinder.udf.integration
 import libertem_blobfinder.udf.utils  # noqa F401
+from libertem_blobfinder.udf.refinement import run_refine
 
-from utils import _mk_random
+from utils import _mk_random, set_device_class
 
 
 @pytest.mark.parametrize(
     "progress", [True, False]
 )
 @pytest.mark.with_numba
 def test_smoke(lt_ctx, progress):
@@ -34,77 +40,88 @@
     udf.correlation.run_blobfinder(
         ctx=lt_ctx, dataset=dataset, num_peaks=1, match_pattern=match_pattern,
         progress=progress
     )
 
 
 @pytest.mark.parametrize(
-    "progress", [True, False]
-)
-def test_run_refine_fastmatch(lt_ctx, progress):
-    shape = np.array([128, 128])
-    zero = shape / 2 + np.random.uniform(-1, 1, size=2)
-    a = np.array([27.17, 0.]) + np.random.uniform(-1, 1, size=2)
-    b = np.array([0., 29.19]) + np.random.uniform(-1, 1, size=2)
-    indices = np.mgrid[-2:3, -2:3]
-    indices = np.concatenate(indices.T)
-
-    drop = np.random.choice([True, False], size=len(indices), p=[0.9, 0.1])
-    indices = indices[drop]
-
-    radius = 10
-
-    data, indices, peaks = cbed_frame(*shape, zero, a, b, indices, radius)
-
-    dataset = MemoryDataSet(data=data, tileshape=(1, *shape),
-                            num_partitions=1, sig_dims=2)
-    matcher = grm.Matcher()
-
-    template = m.radial_gradient(
-        centerX=radius+1,
-        centerY=radius+1,
-        imageSizeX=2*radius+2,
-        imageSizeY=2*radius+2,
-        radius=radius
+    'backend', (None, ) + tuple(
+        libertem_blobfinder.udf.refinement.FastCorrelationUDF(0, None, None).get_backends()
     )
-
-    match_patterns = [
-        common.patterns.RadialGradient(radius=radius),
-        common.patterns.Circular(radius=radius),
-        common.patterns.BackgroundSubtraction(radius=radius),
-        common.patterns.RadialGradientBackgroundSubtraction(radius=radius),
-        common.patterns.UserTemplate(template=template)
-    ]
-
-    print("zero: ", zero)
-    print("a: ", a)
-    print("b: ", b)
-
-    for match_pattern in match_patterns:
-        print("refining using template %s" % type(match_pattern))
-        (res, real_indices) = udf.refinement.run_refine(
-            ctx=lt_ctx,
-            dataset=dataset,
-            zero=zero + np.random.uniform(-1, 1, size=2),
-            a=a + np.random.uniform(-1, 1, size=2),
-            b=b + np.random.uniform(-1, 1, size=2),
-            matcher=matcher,
-            match_pattern=match_pattern,
-            progress=progress
+)
+@pytest.mark.parametrize(
+    'upsample', (True, False)
+)
+def test_run_refine_fastmatch(lt_ctx, backend, upsample):
+    with set_device_class(get_device_class(backend)):
+        shape = np.array([128, 128])
+        zero = shape / 2 + np.random.uniform(-1, 1, size=2)
+        a = np.array([27.17, 0.]) + np.random.uniform(-1, 1, size=2)
+        b = np.array([0., 29.19]) + np.random.uniform(-1, 1, size=2)
+        indices = np.mgrid[-2:3, -2:3]
+        indices = np.concatenate(indices.T)
+
+        drop = np.random.choice([True, False], size=len(indices), p=[0.9, 0.1])
+        indices = indices[drop]
+
+        radius = 10
+
+        data, indices, peaks = cbed_frame(*shape, zero, a, b, indices, radius)
+
+        dataset = MemoryDataSet(
+            data=data,
+            tileshape=(1, *shape),
+            num_partitions=1,
+            sig_dims=2,
+            array_backends=(backend, ) if backend is not None else None
         )
-        print(peaks - grm.calc_coords(
-            res['zero'].data[0],
-            res['a'].data[0],
-            res['b'].data[0],
-            indices)
+        matcher = grm.Matcher()
+
+        template = m.radial_gradient(
+            centerX=radius+1,
+            centerY=radius+1,
+            imageSizeX=2*radius+2,
+            imageSizeY=2*radius+2,
+            radius=radius
         )
 
-        assert np.allclose(res['zero'].data[0], zero, atol=0.5)
-        assert np.allclose(res['a'].data[0], a, atol=0.2)
-        assert np.allclose(res['b'].data[0], b, atol=0.2)
+        match_patterns = [
+            common.patterns.RadialGradient(radius=radius),
+            common.patterns.Circular(radius=radius),
+            common.patterns.BackgroundSubtraction(radius=radius),
+            common.patterns.RadialGradientBackgroundSubtraction(radius=radius),
+            common.patterns.UserTemplate(template=template)
+        ]
+
+        print("zero: ", zero)
+        print("a: ", a)
+        print("b: ", b)
+
+        for match_pattern in match_patterns:
+            print("refining using template %s" % type(match_pattern))
+            (res, real_indices) = run_refine(
+                ctx=lt_ctx,
+                dataset=dataset,
+                zero=zero + np.random.uniform(-1, 1, size=2),
+                a=a + np.random.uniform(-1, 1, size=2),
+                b=b + np.random.uniform(-1, 1, size=2),
+                matcher=matcher,
+                match_pattern=match_pattern,
+                upsample=upsample,
+            )
+            print(peaks - grm.calc_coords(
+                res['zero'].data[0],
+                res['a'].data[0],
+                res['b'].data[0],
+                indices)
+            )
+
+            assert_allclose(res['zero'].data[0], zero, atol=0.5)
+            assert_allclose(res['a'].data[0], a, atol=0.2)
+            assert_allclose(res['b'].data[0], b, atol=0.2)
 
 
 def test_run_refine_affinematch(lt_ctx):
     for i in range(1):
         try:
             shape = np.array([128, 128])
 
@@ -128,129 +145,155 @@
             affine_indices = peaks - zero
 
             for j in range(5):
                 zzero = zero + np.random.uniform(-1, 1, size=2)
                 aa = np.array([1, 0]) + np.random.uniform(-0.05, 0.05, size=2)
                 bb = np.array([0, 1]) + np.random.uniform(-0.05, 0.05, size=2)
 
-                (res, real_indices) = udf.refinement.run_refine(
+                (res, real_indices) = run_refine(
                     ctx=lt_ctx,
                     dataset=dataset,
                     zero=zzero,
                     a=aa,
                     b=bb,
                     indices=affine_indices,
                     matcher=matcher,
                     match_pattern=match_pattern,
                     match='affine'
                 )
 
-                assert np.allclose(res['zero'].data[0], zero, atol=0.5)
-                assert np.allclose(res['a'].data[0], [1, 0], atol=0.05)
-                assert np.allclose(res['b'].data[0], [0, 1], atol=0.05)
+                assert_allclose(res['zero'].data[0], zero, atol=0.5)
+                assert_allclose(res['a'].data[0], [1, 0], atol=0.05)
+                assert_allclose(res['b'].data[0], [0, 1], atol=0.05)
         except Exception:
             print("zero = np.array([%s, %s])" % tuple(zero))
             print("a = np.array([%s, %s])" % tuple(a))
             print("b = np.array([%s, %s])" % tuple(b))
 
             print("zzero = np.array([%s, %s])" % tuple(zzero))
             print("aa = np.array([%s, %s])" % tuple(aa))
             print("bb = np.array([%s, %s])" % tuple(bb))
             raise
 
 
-def test_run_refine_sparse(lt_ctx):
-    shape = np.array([128, 128])
-    zero = shape / 2 + np.random.uniform(-1, 1, size=2)
-    a = np.array([27.17, 0.]) + np.random.uniform(-1, 1, size=2)
-    b = np.array([0., 29.19]) + np.random.uniform(-1, 1, size=2)
-    indices = np.mgrid[-2:3, -2:3]
-    indices = np.concatenate(indices.T)
-
-    radius = 10
-
-    data, indices, peaks = cbed_frame(*shape, zero, a, b, indices, radius)
-
-    dataset = MemoryDataSet(data=data, tileshape=(1, *shape),
-                            num_partitions=1, sig_dims=2)
-
-    matcher = grm.Matcher()
-    match_pattern = common.patterns.RadialGradient(radius=radius)
-
-    print("zero: ", zero)
-    print("a: ", a)
-    print("b: ", b)
-
-    (res, real_indices) = udf.refinement.run_refine(
-        ctx=lt_ctx,
-        dataset=dataset,
-        zero=zero + np.random.uniform(-0.5, 0.5, size=2),
-        a=a + np.random.uniform(-0.5, 0.5, size=2),
-        b=b + np.random.uniform(-0.5, 0.5, size=2),
-        matcher=matcher,
-        match_pattern=match_pattern,
-        correlation='sparse',
-        steps=3
+@pytest.mark.parametrize(
+    'backend', (None, ) + tuple(
+        libertem_blobfinder.udf.refinement.SparseCorrelationUDF(0, None, None).get_backends()
     )
+)
+def test_run_refine_sparse(lt_ctx, backend):
+    with set_device_class(get_device_class(backend)):
+        shape = np.array([128, 128])
+        zero = shape / 2 + np.random.uniform(-1, 1, size=2)
+        a = np.array([27.17, 0.]) + np.random.uniform(-1, 1, size=2)
+        b = np.array([0., 29.19]) + np.random.uniform(-1, 1, size=2)
+        indices = np.mgrid[-2:3, -2:3]
+        indices = np.concatenate(indices.T)
+
+        radius = 10
+
+        data, indices, peaks = cbed_frame(*shape, zero, a, b, indices, radius)
+
+        dataset = MemoryDataSet(
+            data=data,
+            tileshape=(1, *shape),
+            num_partitions=1,
+            sig_dims=2,
+            array_backends=(backend, ) if backend is not None else None
+        )
 
-    print(peaks - grm.calc_coords(
-        res['zero'].data[0],
-        res['a'].data[0],
-        res['b'].data[0],
-        indices)
-    )
+        matcher = grm.Matcher()
+        match_pattern = common.patterns.RadialGradient(radius=radius)
 
-    assert np.allclose(res['zero'].data[0], zero, atol=0.5)
-    assert np.allclose(res['a'].data[0], a, atol=0.2)
-    assert np.allclose(res['b'].data[0], b, atol=0.2)
+        print("zero: ", zero)
+        print("a: ", a)
+        print("b: ", b)
 
+        (res, real_indices) = run_refine(
+            ctx=lt_ctx,
+            dataset=dataset,
+            zero=zero + np.random.uniform(-0.5, 0.5, size=2),
+            a=a + np.random.uniform(-0.5, 0.5, size=2),
+            b=b + np.random.uniform(-0.5, 0.5, size=2),
+            matcher=matcher,
+            match_pattern=match_pattern,
+            correlation='sparse',
+            steps=3,
+        )
 
-def test_run_refine_fullframe(lt_ctx):
-    shape = np.array([128, 128])
-    zero = shape / 2 + np.random.uniform(-1, 1, size=2)
-    a = np.array([27.17, 0.]) + np.random.uniform(-1, 1, size=2)
-    b = np.array([0., 29.19]) + np.random.uniform(-1, 1, size=2)
-    indices = np.mgrid[-2:3, -2:3]
-    indices = np.concatenate(indices.T)
+        print(peaks - grm.calc_coords(
+            res['zero'].data[0],
+            res['a'].data[0],
+            res['b'].data[0],
+            indices)
+        )
 
-    radius = 10
+        assert_allclose(res['zero'].data[0], zero, atol=0.5)
+        assert_allclose(res['a'].data[0], a, atol=0.2)
+        assert_allclose(res['b'].data[0], b, atol=0.2)
 
-    data, indices, peaks = cbed_frame(*shape, zero, a, b, indices, radius)
 
-    dataset = MemoryDataSet(data=data, tileshape=(1, *shape),
-                            num_partitions=1, sig_dims=2)
+@pytest.mark.parametrize(
+    'backend', (None, ) + tuple(
+        libertem_blobfinder.udf.refinement.FullFrameCorrelationUDF(0, None, None).get_backends()
+    )
+)
+@pytest.mark.parametrize(
+    'upsample', (True, False)
+)
+def test_run_refine_fullframe(lt_ctx, backend, upsample):
+    with set_device_class(get_device_class(backend)):
+        shape = np.array([128, 128])
+        zero = shape / 2 + np.random.uniform(-1, 1, size=2)
+        a = np.array([27.17, 0.]) + np.random.uniform(-1, 1, size=2)
+        b = np.array([0., 29.19]) + np.random.uniform(-1, 1, size=2)
+        indices = np.mgrid[-2:3, -2:3]
+        indices = np.concatenate(indices.T)
+
+        radius = 10
+
+        data, indices, peaks = cbed_frame(*shape, zero, a, b, indices, radius)
+
+        dataset = MemoryDataSet(
+            data=data,
+            tileshape=(1, *shape),
+            num_partitions=1,
+            sig_dims=2,
+            array_backends=(backend, ) if backend is not None else None,
+        )
 
-    matcher = grm.Matcher()
-    match_pattern = common.patterns.RadialGradient(radius=radius)
+        matcher = grm.Matcher()
+        match_pattern = common.patterns.RadialGradient(radius=radius)
 
-    print("zero: ", zero)
-    print("a: ", a)
-    print("b: ", b)
+        print("zero: ", zero)
+        print("a: ", a)
+        print("b: ", b)
 
-    (res, real_indices) = udf.refinement.run_refine(
-        ctx=lt_ctx,
-        dataset=dataset,
-        zero=zero + np.random.uniform(-0.5, 0.5, size=2),
-        a=a + np.random.uniform(-0.5, 0.5, size=2),
-        b=b + np.random.uniform(-0.5, 0.5, size=2),
-        matcher=matcher,
-        match_pattern=match_pattern,
-        correlation='fullframe',
-    )
+        (res, real_indices) = run_refine(
+            ctx=lt_ctx,
+            dataset=dataset,
+            zero=zero + np.random.uniform(-0.5, 0.5, size=2),
+            a=a + np.random.uniform(-0.5, 0.5, size=2),
+            b=b + np.random.uniform(-0.5, 0.5, size=2),
+            matcher=matcher,
+            match_pattern=match_pattern,
+            correlation='fullframe',
+            upsample=upsample,
+        )
 
-    print(peaks - grm.calc_coords(
-        res['zero'].data[0],
-        res['a'].data[0],
-        res['b'].data[0],
-        indices)
-    )
+        print(peaks - grm.calc_coords(
+            res['zero'].data[0],
+            res['a'].data[0],
+            res['b'].data[0],
+            indices)
+        )
 
-    assert np.allclose(res['zero'].data[0], zero, atol=0.5)
-    assert np.allclose(res['a'].data[0], a, atol=0.2)
-    assert np.allclose(res['b'].data[0], b, atol=0.2)
+        assert_allclose(res['zero'].data[0], zero, atol=0.5)
+        assert_allclose(res['a'].data[0], a, atol=0.5)
+        assert_allclose(res['b'].data[0], b, atol=0.5)
 
 
 @pytest.mark.with_numba
 @pytest.mark.parametrize(
     "cls",
     [
         udf.correlation.FastCorrelationUDF,
@@ -294,24 +337,26 @@
             *np.random.randint(low=1, high=len(peaks)*nbytes + 3, size=5)):
         m_udf = cls(peaks=peaks, match_pattern=match_pattern, __limit=limit)
         res = lt_ctx.run_udf(udf=m_udf, dataset=dataset)
         print(limit)
         print(res['refineds'].data[0])
         print(peaks)
         print(peaks - res['refineds'].data[0])
-        assert np.allclose(res['refineds'].data[0], peaks, atol=0.5)
+        assert_allclose(res['refineds'].data[0], peaks, atol=0.5)
 
 
 @pytest.mark.with_numba
 @pytest.mark.parametrize(
     "cls,dtype,kwargs",
     [
         (udf.correlation.FastCorrelationUDF, int, {}),
         (udf.correlation.FastCorrelationUDF, float, {}),
         (udf.correlation.FastCorrelationUDF, float, {'zero_shift': (2, 3)}),
+        (udf.correlation.FastCorrelationUDF, int, {'upsample': True}),
+        (udf.correlation.FastCorrelationUDF, int, {'upsample': 15}),
         (udf.correlation.SparseCorrelationUDF, int, {'steps': 3}),
         (udf.correlation.SparseCorrelationUDF, float, {'steps': 3}),
         (udf.correlation.SparseCorrelationUDF, float, {'steps': 3, 'zero_shift': (2, 7)}),
     ]
 )
 def test_correlation_methods(lt_ctx, cls, dtype, kwargs):
     shape = np.array([128, 128])
@@ -364,24 +409,28 @@
 
             # import matplotlib.pyplot as plt
             # fig, ax = plt.subplots()
             # plt.imshow(data[0])
             # for p in np.flip(res['refineds'].data[0], axis=-1):
             #     ax.add_artist(plt.Circle(p, radius, fill=False, color='y'))
             # plt.show()
-
-            assert np.allclose(res['refineds'].data[0], peaks, atol=0.5)
+            atol = 0.5
+            # Because of rounding in cbed_frame, cannot be sure of tolerance!
+            # if 'upsample' in kwargs:
+            #     atol = 0.25
+            assert_allclose(res['refineds'].data[0], peaks, atol=atol)
 
 
 @pytest.mark.with_numba
 @pytest.mark.parametrize(
     "cls,dtype,kwargs",
     [
         (udf.correlation.FullFrameCorrelationUDF, int, {}),
         (udf.correlation.FullFrameCorrelationUDF, float, {}),
+        (udf.correlation.FullFrameCorrelationUDF, int, {'upsample': True}),
     ]
 )
 def test_correlation_method_fullframe(lt_ctx, cls, dtype, kwargs):
     shape = np.array([128, 128])
     zero = shape / 2 + np.random.uniform(-1, 1, size=2)
     a = np.array([34.3, 0.]) + np.random.uniform(-1, 1, size=2)
     b = np.array([0., 42.19]) + np.random.uniform(-1, 1, size=2)
@@ -424,16 +473,19 @@
 
         # import matplotlib.pyplot as plt
         # fig, ax = plt.subplots()
         # plt.imshow(data[0])
         # for p in np.flip(res['refineds'].data[0], axis=-1):
         #     ax.add_artist(plt.Circle(p, radius, fill=False, color='y'))
         # plt.show()
-
-        assert np.allclose(res['refineds'].data[0], peaks, atol=0.5)
+        atol = 0.5
+        # Because of rounding in cbed_frame, cannot be sure of tolerance!
+        # if 'upsample' in kwargs:
+        #     atol = 0.25
+        assert_allclose(res['refineds'].data[0], peaks, atol=atol)
 
 
 @pytest.mark.parametrize(
     "navshape", ((1, 1), (1, ))
 )
 def test_visualize_smoke(navshape, lt_ctx):
     shape = np.array([128, 128])
@@ -455,22 +507,23 @@
 
     match_pattern = common.patterns.RadialGradientBackgroundSubtraction(radius=radius)
 
     print("zero: ", zero)
     print("a: ", a)
     print("b: ", b)
 
-    (res, real_indices) = udf.refinement.run_refine(
+    (res, real_indices) = run_refine(
         ctx=lt_ctx,
         dataset=dataset,
         zero=zero + np.random.uniform(-1, 1, size=2),
         a=a + np.random.uniform(-1, 1, size=2),
         b=b + np.random.uniform(-1, 1, size=2),
         matcher=matcher,
-        match_pattern=match_pattern
+        match_pattern=match_pattern,
+        progress=True,
     )
 
     fig, axes = plt.subplots()
     if len(navshape) == 1:
         y = None
     elif len(navshape) == 2:
         y = 0
@@ -515,15 +568,15 @@
     print("zero: ", zero)
     print("a: ", a)
     print("b: ", b)
 
     for match_pattern in match_patterns:
         print("refining using template %s" % type(match_pattern))
         zero_shift = np.array([(0., 0.), shift]).astype(np.float32)
-        (res, real_indices) = udf.refinement.run_refine(
+        (res, real_indices) = run_refine(
             ctx=lt_ctx,
             dataset=dataset,
             zero=zero + np.random.uniform(-1, 1, size=2),
             a=a + np.random.uniform(-1, 1, size=2),
             b=b + np.random.uniform(-1, 1, size=2),
             matcher=matcher,
             match_pattern=match_pattern,
@@ -539,18 +592,18 @@
         print(peaks_1 - grm.calc_coords(
             res['zero'].data[1],
             res['a'].data[1],
             res['b'].data[1],
             indices_1)
         )
 
-        assert np.allclose(res['zero'].data[0], zero, atol=0.5)
-        assert np.allclose(res['zero'].data[1], zero + shift, atol=0.5)
-        assert np.allclose(res['a'].data, a, atol=0.2)
-        assert np.allclose(res['b'].data, b, atol=0.2)
+        assert_allclose(res['zero'].data[0], zero, atol=0.5)
+        assert_allclose(res['zero'].data[1], zero + shift, atol=0.5)
+        assert_allclose(res['a'].data, np.tile(a[np.newaxis, :], (2, 1)), atol=0.2)
+        assert_allclose(res['b'].data, np.tile(b[np.newaxis, :], (2, 1)), atol=0.2)
 
 
 def test_integration(lt_ctx):
     indices = np.mgrid[-3:4, -3:4]
     a = (15, 1)
     b = (-1, 17)
     zero = (62, 63)
@@ -598,9 +651,57 @@
         pattern=libertem_blobfinder.common.patterns.BackgroundSubtraction(
             radius=5, radius_outer=6
         )
     )
     res = lt_ctx.run_udf(udf=udf, dataset=ds)
 
     # Make sure the integration result matches exactly the sum of one peak
-    assert np.allclose(ref_frame.sum(), res['integration'].data)
+    assert_allclose(ref_frame.sum(), res['integration'].data)
     assert res['integration'].data.shape == peaks.shape[:-1]
+
+
+def test_featurevector(lt_ctx):
+    shape = np.array([128, 128])
+    zero = shape // 2
+    a = np.array([24, 0.])
+    b = np.array([0., 30])
+    indices = np.mgrid[-2:3, -2:3]
+    indices = np.concatenate(indices.T)
+
+    radius = 5
+    radius_outer = 10
+
+    template = m.background_subtraction(
+        centerX=radius_outer + 1,
+        centerY=radius_outer + 1,
+        imageSizeX=radius_outer*2 + 2,
+        imageSizeY=radius_outer*2 + 2,
+        radius=radius_outer,
+        radius_inner=radius + 1,
+        antialiased=False
+    )
+
+    data, indices, peaks = cbed_frame(*shape, zero, a, b, indices, radius, all_equal=True)
+
+    dataset = MemoryDataSet(data=data, tileshape=(1, *shape),
+                            num_partitions=1, sig_dims=2)
+
+    match_pattern = common.patterns.UserTemplate(template=template)
+
+    stack = functools.partial(
+        common.patterns.feature_vector,
+        imageSizeX=shape[1],
+        imageSizeY=shape[0],
+        peaks=peaks,
+        match_pattern=match_pattern,
+    )
+
+    m_udf = ApplyMasksUDF(
+        mask_factories=stack, mask_count=len(peaks), mask_dtype=np.float32
+    )
+    res = lt_ctx.run_udf(dataset=dataset, udf=m_udf)
+
+    peak_data, _, _ = cbed_frame(*shape, zero, a, b, np.array([(0, 0)]), radius, all_equal=True)
+    peak_sum = peak_data.sum()
+
+    assert np.allclose(res['intensity'].data.sum(), data.sum())
+    assert np.allclose(res['intensity'].data, peak_sum)
```

