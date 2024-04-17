# Comparing `tmp/pz-rail-lephare-0.1.tar.gz` & `tmp/pz_rail_lephare-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-lephare-0.1.tar", last modified: Fri Apr  5 22:01:48 2024, max compression
+gzip compressed data, was "pz_rail_lephare-0.1.1.tar", last modified: Wed Apr 17 15:05:27 2024, max compression
```

## Comparing `pz-rail-lephare-0.1.tar` & `pz_rail_lephare-0.1.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:01:48.366022 pz-rail-lephare-0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-05 22:01:40.000000 pz-rail-lephare-0.1/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:01:48.362022 pz-rail-lephare-0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:01:48.362022 pz-rail-lephare-0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-05 22:01:40.000000 pz-rail-lephare-0.1/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-05 22:01:40.000000 pz-rail-lephare-0.1/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-05 22:01:40.000000 pz-rail-lephare-0.1/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-05 22:01:40.000000 pz-rail-lephare-0.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:01:48.366022 pz-rail-lephare-0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-05 22:01:40.000000 pz-rail-lephare-0.1/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-05 22:01:40.000000 pz-rail-lephare-0.1/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-05 22:01:40.000000 pz-rail-lephare-0.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-05 22:01:40.000000 pz-rail-lephare-0.1/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-05 22:01:40.000000 pz-rail-lephare-0.1/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-05 22:01:40.000000 pz-rail-lephare-0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-05 22:01:40.000000 pz-rail-lephare-0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-05 22:01:40.000000 pz-rail-lephare-0.1/.prepare_project.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-05 22:01:40.000000 pz-rail-lephare-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-05 22:01:48.366022 pz-rail-lephare-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-05 22:01:40.000000 pz-rail-lephare-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:01:48.366022 pz-rail-lephare-0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    30028 2024-04-05 22:01:40.000000 pz-rail-lephare-0.1/examples/LePhare_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-05 22:01:40.000000 pz-rail-lephare-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 22:01:48.366022 pz-rail-lephare-0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:01:48.362022 pz-rail-lephare-0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:01:48.366022 pz-rail-lephare-0.1/src/pz_rail_lephare.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-04-05 22:01:48.000000 pz-rail-lephare-0.1/src/pz_rail_lephare.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-05 22:01:48.000000 pz-rail-lephare-0.1/src/pz_rail_lephare.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 22:01:48.000000 pz-rail-lephare-0.1/src/pz_rail_lephare.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-05 22:01:48.000000 pz-rail-lephare-0.1/src/pz_rail_lephare.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-05 22:01:48.000000 pz-rail-lephare-0.1/src/pz_rail_lephare.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:01:48.362022 pz-rail-lephare-0.1/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:01:48.362022 pz-rail-lephare-0.1/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:01:48.366022 pz-rail-lephare-0.1/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-04-05 22:01:40.000000 pz-rail-lephare-0.1/src/rail/estimation/algos/lephare.py
--rw-r--r--   0 runner    (1001) docker     (127)    12157 2024-04-05 22:01:40.000000 pz-rail-lephare-0.1/src/rail/estimation/algos/lsst.para
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:01:48.366022 pz-rail-lephare-0.1/src/rail/lephare/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-05 22:01:40.000000 pz-rail-lephare-0.1/src/rail/lephare/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-05 22:01:40.000000 pz-rail-lephare-0.1/src/rail/lephare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-05 22:01:48.000000 pz-rail-lephare-0.1/src/rail/lephare/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:01:48.362022 pz-rail-lephare-0.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:01:48.366022 pz-rail-lephare-0.1/tests/lephare/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-05 22:01:40.000000 pz-rail-lephare-0.1/tests/lephare/test_algos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:05:27.907948 pz_rail_lephare-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:05:27.903948 pz_rail_lephare-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:05:27.903948 pz_rail_lephare-0.1.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:05:27.903948 pz_rail_lephare-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/.prepare_project.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-04-17 15:05:27.907948 pz_rail_lephare-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:05:27.903948 pz_rail_lephare-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    30028 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/examples/LePhare_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 15:05:27.907948 pz_rail_lephare-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:05:27.899948 pz_rail_lephare-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:05:27.907948 pz_rail_lephare-0.1.1/src/pz_rail_lephare.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-04-17 15:05:27.000000 pz_rail_lephare-0.1.1/src/pz_rail_lephare.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-17 15:05:27.000000 pz_rail_lephare-0.1.1/src/pz_rail_lephare.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 15:05:27.000000 pz_rail_lephare-0.1.1/src/pz_rail_lephare.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-17 15:05:27.000000 pz_rail_lephare-0.1.1/src/pz_rail_lephare.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-17 15:05:27.000000 pz_rail_lephare-0.1.1/src/pz_rail_lephare.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:05:27.903948 pz_rail_lephare-0.1.1/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:05:27.903948 pz_rail_lephare-0.1.1/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:05:27.907948 pz_rail_lephare-0.1.1/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/src/rail/estimation/algos/lephare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12157 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/src/rail/estimation/algos/lsst.para
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:05:27.907948 pz_rail_lephare-0.1.1/src/rail/lephare/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/src/rail/lephare/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/src/rail/lephare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-17 15:05:27.000000 pz_rail_lephare-0.1.1/src/rail/lephare/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:05:27.903948 pz_rail_lephare-0.1.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:05:27.907948 pz_rail_lephare-0.1.1/tests/lephare/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-17 15:05:21.000000 pz_rail_lephare-0.1.1/tests/lephare/test_algos.py
```

### Comparing `pz-rail-lephare-0.1/.github/ISSUE_TEMPLATE/1-bug_report.md` & `pz_rail_lephare-0.1.1/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `pz-rail-lephare-0.1/.github/ISSUE_TEMPLATE/2-feature_request.md` & `pz_rail_lephare-0.1.1/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `pz-rail-lephare-0.1/.github/pull_request_template.md` & `pz_rail_lephare-0.1.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz-rail-lephare-0.1/.github/workflows/linting.yml` & `pz_rail_lephare-0.1.1/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-lephare-0.1/.github/workflows/publish-to-pypi.yml` & `pz_rail_lephare-0.1.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-lephare-0.1/.github/workflows/smoke-test.yml` & `pz_rail_lephare-0.1.1/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-lephare-0.1/.github/workflows/testing-and-coverage.yml` & `pz_rail_lephare-0.1.1/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-lephare-0.1/.gitignore` & `pz_rail_lephare-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-lephare-0.1/.pre-commit-config.yaml` & `pz_rail_lephare-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-lephare-0.1/.prepare_project.sh` & `pz_rail_lephare-0.1.1/.prepare_project.sh`

 * *Files identical despite different names*

### Comparing `pz-rail-lephare-0.1/LICENSE` & `pz_rail_lephare-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-lephare-0.1/PKG-INFO` & `pz_rail_lephare-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-lephare
-Version: 0.1
+Version: 0.1.1
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <lsst-desc-rail-admin@slac.stanford.edu>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -42,55 +42,41 @@
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 
 # pz-rail-lephare
 
 [![Template](https://img.shields.io/badge/Template-LINCC%20Frameworks%20Python%20Project%20Template-brightgreen)](https://lincc-ppt.readthedocs.io/en/latest/)
 [![codecov](https://codecov.io/gh/LSSTDESC/pz-rail-lephare/branch/main/graph/badge.svg)](https://codecov.io/gh/LSSTDESC/pz-rail-lephare)
-[![PyPI](https://img.shields.io/pypi/v/lephare?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/lephare/)
+[![PyPI](https://img.shields.io/pypi/v/lephare?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/pz-rail-lephare/)
 
-## TODO List
+## RAIL LePHARE
 
-To ensure that your project and repository is stable from the very start there 
-are a few todo items that you should take care of. Unfortunately the RAIL project
-template can not do these for you, otherwise it would :) 
-
-### Immediate actions
-- ~~In your repository settings:~~
-  -  ~~Grant the `LSSTDESC/rail_admin` group administrator access~~
-  -  ~~Grant the `LSSTDESC/photo-z` group maintainer access~~
-- ~~Configure Codecov for the repository~~
-  - ~~Go here, https://github.com/apps/codecov, click the "Configure" button~~
-- ~~Log in to PyPI.org and configure Trusted Publishing following these instructions https://docs.pypi.org/trusted-publishers/creating-a-project-through-oidc/~~
-- ~~Create a Personal Access Token (PAT) to automatically add issues to the RAIL project tracker~~
-  - ~~Follow these instruction to create a PAT: https://github.com/actions/add-to-project#creating-a-pat-and-adding-it-to-your-repository ~~
-  - ~~Save your new PAT as a repository secret named `ADD_TO_PROJECT_PAT`~~
-
-### Before including in Rail ecosystem
-- ~~Make sure your `main` branch is protected~~
-- Update this README
-- ~~Create an example notebook~~
-- ~~Run `pylint` on your code~~
-- Remove this TODO list once all items are completed
+This package allows users to run the [LePHARE code](https://github.com/lephare-photoz/lephare/) 
+through [RAIL](https://github.com/LSSTDESC/RAIL). 
+It can be installed via pip with the following command. 
+Full documentation is available at the main [LePHARE documentation](https://lephare.readthedocs.io/en/latest/index.html).
 
+```console
+pip install pz-rail-lephare
+```
 
 ## RAIL: Redshift Assessment Infrastructure Layers
 
 This package is part of the larger ecosystem of Photometric Redshifts
 in [RAIL](https://github.com/LSSTDESC/RAIL). This package in particular
 is concerned with wrapping the [LePHARE](https://gitlab.lam.fr/Galaxies/LEPHARE/) template fitting code within RAIL.
 
-### Installation
+### Developer installation
 
-This package can be installed from source using the following commands:
+This package can be installed from source using the following commands to allow working on the code.
 ```console
 git clone https://github.com/LSSTDESC/rail_lephare.git
 cd rail_lephare
 conda install -c conda-forge pytables
-pip install '.[dev]'
+pip install -e '.[dev]'
 ```
 
 ### Citing RAIL
 
 This code, while public on GitHub, has not yet been released by DESC and is
 still under active development. Our release of v1.0 will be accompanied by a
 journal paper describing the development and validation of RAIL.
```

### Comparing `pz-rail-lephare-0.1/examples/LePhare_demo.ipynb` & `pz_rail_lephare-0.1.1/examples/LePhare_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-lephare-0.1/pyproject.toml` & `pz_rail_lephare-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz-rail-lephare-0.1/src/pz_rail_lephare.egg-info/PKG-INFO` & `pz_rail_lephare-0.1.1/src/pz_rail_lephare.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-lephare
-Version: 0.1
+Version: 0.1.1
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <lsst-desc-rail-admin@slac.stanford.edu>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -42,55 +42,41 @@
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 
 # pz-rail-lephare
 
 [![Template](https://img.shields.io/badge/Template-LINCC%20Frameworks%20Python%20Project%20Template-brightgreen)](https://lincc-ppt.readthedocs.io/en/latest/)
 [![codecov](https://codecov.io/gh/LSSTDESC/pz-rail-lephare/branch/main/graph/badge.svg)](https://codecov.io/gh/LSSTDESC/pz-rail-lephare)
-[![PyPI](https://img.shields.io/pypi/v/lephare?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/lephare/)
+[![PyPI](https://img.shields.io/pypi/v/lephare?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/pz-rail-lephare/)
 
-## TODO List
+## RAIL LePHARE
 
-To ensure that your project and repository is stable from the very start there 
-are a few todo items that you should take care of. Unfortunately the RAIL project
-template can not do these for you, otherwise it would :) 
-
-### Immediate actions
-- ~~In your repository settings:~~
-  -  ~~Grant the `LSSTDESC/rail_admin` group administrator access~~
-  -  ~~Grant the `LSSTDESC/photo-z` group maintainer access~~
-- ~~Configure Codecov for the repository~~
-  - ~~Go here, https://github.com/apps/codecov, click the "Configure" button~~
-- ~~Log in to PyPI.org and configure Trusted Publishing following these instructions https://docs.pypi.org/trusted-publishers/creating-a-project-through-oidc/~~
-- ~~Create a Personal Access Token (PAT) to automatically add issues to the RAIL project tracker~~
-  - ~~Follow these instruction to create a PAT: https://github.com/actions/add-to-project#creating-a-pat-and-adding-it-to-your-repository ~~
-  - ~~Save your new PAT as a repository secret named `ADD_TO_PROJECT_PAT`~~
-
-### Before including in Rail ecosystem
-- ~~Make sure your `main` branch is protected~~
-- Update this README
-- ~~Create an example notebook~~
-- ~~Run `pylint` on your code~~
-- Remove this TODO list once all items are completed
+This package allows users to run the [LePHARE code](https://github.com/lephare-photoz/lephare/) 
+through [RAIL](https://github.com/LSSTDESC/RAIL). 
+It can be installed via pip with the following command. 
+Full documentation is available at the main [LePHARE documentation](https://lephare.readthedocs.io/en/latest/index.html).
 
+```console
+pip install pz-rail-lephare
+```
 
 ## RAIL: Redshift Assessment Infrastructure Layers
 
 This package is part of the larger ecosystem of Photometric Redshifts
 in [RAIL](https://github.com/LSSTDESC/RAIL). This package in particular
 is concerned with wrapping the [LePHARE](https://gitlab.lam.fr/Galaxies/LEPHARE/) template fitting code within RAIL.
 
-### Installation
+### Developer installation
 
-This package can be installed from source using the following commands:
+This package can be installed from source using the following commands to allow working on the code.
 ```console
 git clone https://github.com/LSSTDESC/rail_lephare.git
 cd rail_lephare
 conda install -c conda-forge pytables
-pip install '.[dev]'
+pip install -e '.[dev]'
 ```
 
 ### Citing RAIL
 
 This code, while public on GitHub, has not yet been released by DESC and is
 still under active development. Our release of v1.0 will be accompanied by a
 journal paper describing the development and validation of RAIL.
```

### Comparing `pz-rail-lephare-0.1/src/pz_rail_lephare.egg-info/SOURCES.txt` & `pz_rail_lephare-0.1.1/src/pz_rail_lephare.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-lephare-0.1/src/rail/estimation/algos/lephare.py` & `pz_rail_lephare-0.1.1/src/rail/estimation/algos/lephare.py`

 * *Files identical despite different names*

### Comparing `pz-rail-lephare-0.1/src/rail/estimation/algos/lsst.para` & `pz_rail_lephare-0.1.1/src/rail/estimation/algos/lsst.para`

 * *Files identical despite different names*

