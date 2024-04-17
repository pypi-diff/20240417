# Comparing `tmp/spotGUI-0.5.0.tar.gz` & `tmp/spotgui-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotGUI-0.5.0.tar", last modified: Mon Apr  8 13:05:41 2024, max compression
+gzip compressed data, was "spotgui-0.5.1.tar", last modified: Wed Apr 17 20:48:33 2024, max compression
```

## Comparing `spotGUI-0.5.0.tar` & `spotgui-0.5.1.tar`

### file list

```diff
@@ -1,102 +1,104 @@
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-08 13:05:41.785472 spotGUI-0.5.0/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-08 13:05:41.682130 spotGUI-0.5.0/.github/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-08 13:05:41.685832 spotGUI-0.5.0/.github/workflows/
--rw-r--r--   0 bartz      (501) staff       (20)      557 2024-02-13 13:06:51.000000 spotGUI-0.5.0/.github/workflows/test.yml
--rw-r--r--   0 bartz      (501) staff       (20)     1954 2024-03-27 21:06:14.000000 spotGUI-0.5.0/.gitignore
--rw-r--r--   0 bartz      (501) staff       (20)        0 2024-02-13 13:06:51.000000 spotGUI-0.5.0/.nojekyll
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-08 13:05:41.686164 spotGUI-0.5.0/.vscode/
--rw-r--r--   0 bartz      (501) staff       (20)      823 2024-02-13 13:06:51.000000 spotGUI-0.5.0/.vscode/settings.json
--rw-r--r--   0 bartz      (501) staff       (20)    34523 2024-02-13 13:06:51.000000 spotGUI-0.5.0/LICENSE.txt
--rw-r--r--   0 bartz      (501) staff       (20)      131 2024-02-13 13:06:51.000000 spotGUI-0.5.0/MANIFEST.in
--rw-r--r--   0 bartz      (501) staff       (20)     8431 2024-04-08 13:05:41.785210 spotGUI-0.5.0/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)     6814 2024-02-13 13:06:51.000000 spotGUI-0.5.0/README.md
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-08 13:05:41.687502 spotGUI-0.5.0/docs/
--rw-r--r--   0 bartz      (501) staff       (20)    46499 2024-02-13 13:06:51.000000 spotGUI-0.5.0/docs/about.md
--rw-r--r--   0 bartz      (501) staff       (20)       73 2024-02-13 13:06:51.000000 spotGUI-0.5.0/docs/download.md
--rw-r--r--   0 bartz      (501) staff       (20)     1823 2024-02-13 13:06:51.000000 spotGUI-0.5.0/docs/examples.md
--rw-r--r--   0 bartz      (501) staff       (20)      947 2024-02-13 13:06:51.000000 spotGUI-0.5.0/docs/gen_ref_pages.py
--rw-r--r--   0 bartz      (501) staff       (20)      350 2024-02-13 13:06:51.000000 spotGUI-0.5.0/docs/hyperparameter-tuning-cookbook.md
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-08 13:05:41.688296 spotGUI-0.5.0/docs/images/
--rw-r--r--   0 bartz      (501) staff       (20)    11605 2024-02-13 13:06:51.000000 spotGUI-0.5.0/docs/images/favicon.png
--rw-r--r--   0 bartz      (501) staff       (20)    11253 2024-02-13 13:06:51.000000 spotGUI-0.5.0/docs/images/plot-progress.png
--rw-r--r--   0 bartz      (501) staff       (20)    11605 2024-02-13 13:06:51.000000 spotGUI-0.5.0/docs/images/spotlogo.png
--rw-r--r--   0 bartz      (501) staff       (20)   122656 2024-02-13 13:06:51.000000 spotGUI-0.5.0/docs/images/surrogate-plot.png
--rw-r--r--   0 bartz      (501) staff       (20)      392 2024-02-13 13:06:51.000000 spotGUI-0.5.0/docs/index.md
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-08 13:05:41.689185 spotGUI-0.5.0/img/
--rw-r--r--   0 bartz      (501) staff       (20)    11605 2024-02-13 13:06:51.000000 spotGUI-0.5.0/img/favicon.png
--rw-r--r--   0 bartz      (501) staff       (20)    67674 2024-02-13 13:06:51.000000 spotGUI-0.5.0/img/spotLogo.png
--rwxr-xr-x   0 bartz      (501) staff       (20)      114 2024-02-13 13:06:51.000000 spotGUI-0.5.0/makeSpotGUI.sh
--rw-r--r--   0 bartz      (501) staff       (20)     2026 2024-02-13 13:06:51.000000 spotGUI-0.5.0/mkdocs.yml
--rw-r--r--   0 bartz      (501) staff       (20)     1762 2024-04-08 13:05:24.000000 spotGUI-0.5.0/pyproject.toml
--rw-r--r--   0 bartz      (501) staff       (20)       38 2024-04-08 13:05:41.785519 spotGUI-0.5.0/setup.cfg
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-08 13:05:41.689916 spotGUI-0.5.0/spotPythonGUI/
--rw-r--r--   0 bartz      (501) staff       (20)    13611 2024-02-14 12:30:00.000000 spotGUI-0.5.0/spotPythonGUI/00_test_spotGUI.ipynb
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-08 13:05:41.690073 spotGUI-0.5.0/spotPythonGUI/images/
--rw-r--r--   0 bartz      (501) staff       (20)     3932 2024-02-14 12:30:00.000000 spotGUI-0.5.0/spotPythonGUI/images/spotlogo.png
--rw-r--r--   0 bartz      (501) staff       (20)    24526 2024-03-27 18:20:51.000000 spotGUI-0.5.0/spotPythonGUI/spotPythonGUI.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-08 13:05:41.742213 spotGUI-0.5.0/spotPythonGUI/userData/
--rw-r--r--   0 bartz      (501) staff       (20)      698 2024-02-14 12:30:00.000000 spotGUI-0.5.0/spotPythonGUI/userData/README.txt
--rw-r--r--   0 bartz      (501) staff       (20)     2323 2024-02-14 12:30:00.000000 spotGUI-0.5.0/spotPythonGUI/userData/data.csv
--rw-r--r--   0 bartz      (501) staff       (20)     7422 2024-02-14 12:30:00.000000 spotGUI-0.5.0/spotPythonGUI/userData/data.pkl
--rw-r--r--   0 bartz      (501) staff       (20) 60425445 2024-02-14 12:30:00.000000 spotGUI-0.5.0/spotPythonGUI/userData/data_sensitive.pkl
--rw-r--r--   0 bartz      (501) staff       (20)    90292 2024-02-14 12:30:00.000000 spotGUI-0.5.0/spotPythonGUI/userData/diabetes.arff
--rw-r--r--   0 bartz      (501) staff       (20)    88796 2024-02-14 12:30:00.000000 spotGUI-0.5.0/spotPythonGUI/userData/diabetes.csv
--rw-r--r--   0 bartz      (501) staff       (20)    39642 2024-02-14 12:30:00.000000 spotGUI-0.5.0/spotPythonGUI/userData/diabetes.pkl
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-08 13:05:41.742669 spotGUI-0.5.0/spotPythonGUI/userModel/
--rw-r--r--   0 bartz      (501) staff       (20)        0 2024-02-14 12:30:00.000000 spotGUI-0.5.0/spotPythonGUI/userModel/__init__.py
--rw-r--r--   0 bartz      (501) staff       (20)     2497 2024-02-14 12:30:00.000000 spotGUI-0.5.0/spotPythonGUI/userModel/netlightregression.json
--rw-r--r--   0 bartz      (501) staff       (20)    11553 2024-02-14 12:30:00.000000 spotGUI-0.5.0/spotPythonGUI/userModel/netlightregression.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-08 13:05:41.743406 spotGUI-0.5.0/spotRiverGUI/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-08 13:05:41.747122 spotGUI-0.5.0/spotRiverGUI/db_dicts/
--rw-r--r--   0 bartz      (501) staff       (20)   142672 2024-04-05 13:39:16.000000 spotGUI-0.5.0/spotRiverGUI/db_dicts/0001_spotRiver_db.json
--rw-r--r--   0 bartz      (501) staff       (20)  3433186 2024-04-04 21:00:24.000000 spotGUI-0.5.0/spotRiverGUI/db_dicts/000_spotRiver_db.json
--rw-r--r--   0 bartz      (501) staff       (20)    42213 2024-04-05 18:50:05.000000 spotGUI-0.5.0/spotRiverGUI/db_dicts/spotRiver_db.json
--rw-r--r--   0 bartz      (501) staff       (20)      404 2024-04-05 15:35:43.000000 spotGUI-0.5.0/spotRiverGUI/db_dicts/spotRiver_db_default.json
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-08 13:05:41.771528 spotGUI-0.5.0/spotRiverGUI/demos/
--rw-r--r--   0 bartz      (501) staff       (20)  2142279 2024-03-17 09:55:25.000000 spotGUI-0.5.0/spotRiverGUI/demos/spot_HARTR_Bike_sharing_00_experiment.pickle
--rw-r--r--   0 bartz      (501) staff       (20) 17140699 2024-03-20 00:13:29.000000 spotGUI-0.5.0/spotRiverGUI/demos/spot_HTR_Bikes_00_experiment.pickle
--rw-r--r--   0 bartz      (501) staff       (20)   153829 2024-03-12 18:03:51.000000 spotGUI-0.5.0/spotRiverGUI/demos/spot_demo_00_experiment.pickle
--rw-r--r--   0 bartz      (501) staff       (20)   234875 2024-03-18 18:33:57.000000 spotGUI-0.5.0/spotRiverGUI/demos/spot_linreg_trump_00_experiment.pickle
--rw-r--r--   0 bartz      (501) staff       (20)   102481 2024-03-18 18:33:57.000000 spotGUI-0.5.0/spotRiverGUI/demos/spot_linreg_trump_02_experiment.pickle
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-08 13:05:41.772224 spotGUI-0.5.0/spotRiverGUI/images/
--rw-r--r--   0 bartz      (501) staff       (20)     3932 2024-02-14 12:30:00.000000 spotGUI-0.5.0/spotRiverGUI/images/spotlogo.png
--rw-r--r--   0 bartz      (501) staff       (20)    64117 2024-04-04 20:58:42.000000 spotGUI-0.5.0/spotRiverGUI/spotRiverGUI.py
--rwxr-xr-x   0 bartz      (501) staff       (20)    43139 2024-03-27 18:20:51.000000 spotGUI-0.5.0/spotRiverGUI/spotRiverGUI_v01.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-08 13:05:41.779708 spotGUI-0.5.0/spotRiverGUI/userData/
--rw-r--r--   0 bartz      (501) staff       (20)    33179 2024-02-14 12:30:00.000000 spotGUI-0.5.0/spotRiverGUI/userData/PhishingData.csv
--rw-r--r--   0 bartz      (501) staff       (20)      477 2024-02-15 08:36:58.000000 spotGUI-0.5.0/spotRiverGUI/userData/PhishingData_license.txt
--rw-r--r--   0 bartz      (501) staff       (20)  1493626 2024-03-17 22:09:34.000000 spotGUI-0.5.0/spotRiverGUI/userData/bike_sharing_demand.csv
--rw-r--r--   0 bartz      (501) staff       (20)  1633709 2024-03-17 22:09:34.000000 spotGUI-0.5.0/spotRiverGUI/userData/bike_sharing_demand_lagged.csv
--rw-r--r--   0 bartz      (501) staff       (20)  1387328 2024-03-18 23:08:42.000000 spotGUI-0.5.0/spotRiverGUI/userData/bike_sharing_demand_sklearn.csv
--rw-r--r--   0 bartz      (501) staff       (20)    42652 2024-02-15 08:36:58.000000 spotGUI-0.5.0/spotRiverGUI/userData/phishingRiver.csv
--rw-r--r--   0 bartz      (501) staff       (20)  1993321 2024-02-14 12:30:00.000000 spotGUI-0.5.0/spotRiverGUI/userData/user_data.csv
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-08 13:05:41.781386 spotGUI-0.5.0/spotRiverGUI/userModel/
--rw-r--r--   0 bartz      (501) staff       (20)        0 2024-02-14 12:30:00.000000 spotGUI-0.5.0/spotRiverGUI/userModel/__init__.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-08 13:05:45.117106 spotGUI-0.5.0/spotRiverGUI/userPrepModel/
--rw-r--r--   0 bartz      (501) staff       (20)        0 2024-02-14 12:30:00.000000 spotGUI-0.5.0/spotRiverGUI/userPrepModel/__init__.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-08 13:05:45.117618 spotGUI-0.5.0/spotRiverGUI/userPrepModel/__pycache__/
--rw-r--r--   0 bartz      (501) staff       (20)     1143 2024-04-08 13:05:45.117506 spotGUI-0.5.0/spotRiverGUI/userPrepModel/__pycache__/prep_test.cpython-311-pytest-7.4.4.pyc
--rw-r--r--   0 bartz      (501) staff       (20)     1033 2024-03-27 18:20:51.000000 spotGUI-0.5.0/spotRiverGUI/userPrepModel/prep_Bikes_river.py
--rw-r--r--   0 bartz      (501) staff       (20)      288 2024-03-27 18:20:51.000000 spotGUI-0.5.0/spotRiverGUI/userPrepModel/prep_generic_num_cat.py
--rw-r--r--   0 bartz      (501) staff       (20)     1265 2024-03-27 18:20:51.000000 spotGUI-0.5.0/spotRiverGUI/userPrepModel/prep_test.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-08 13:05:41.683299 spotGUI-0.5.0/src/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-08 13:05:41.683454 spotGUI-0.5.0/src/spotGUI/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-08 13:05:41.782350 spotGUI-0.5.0/src/spotGUI/eda/
--rw-r--r--   0 bartz      (501) staff       (20)      921 2024-02-21 13:54:55.000000 spotGUI-0.5.0/src/spotGUI/eda/pairplot.py
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-08 13:05:41.783928 spotGUI-0.5.0/src/spotGUI/tuner/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-08 13:05:41.784397 spotGUI-0.5.0/src/spotGUI/tuner/images/
--rw-r--r--   0 bartz      (501) staff       (20)     3932 2024-02-13 13:06:51.000000 spotGUI-0.5.0/src/spotGUI/tuner/images/spotlogo.png
--rw-r--r--   0 bartz      (501) staff       (20)    42500 2024-02-13 13:06:51.000000 spotGUI-0.5.0/src/spotGUI/tuner/plot.png
--rw-r--r--   0 bartz      (501) staff       (20)    29347 2024-04-08 13:05:32.000000 spotGUI-0.5.0/src/spotGUI/tuner/spotRun.py
--rw-r--r--   0 bartz      (501) staff       (20)    67715 2024-02-13 13:06:51.000000 spotGUI-0.5.0/src/spotGUI/tuner/spot_00experiment.pickle
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-08 13:05:41.784829 spotGUI-0.5.0/src/spotGUI.egg-info/
--rw-r--r--   0 bartz      (501) staff       (20)     8431 2024-04-08 13:05:41.000000 spotGUI-0.5.0/src/spotGUI.egg-info/PKG-INFO
--rw-r--r--   0 bartz      (501) staff       (20)     2342 2024-04-08 13:05:41.000000 spotGUI-0.5.0/src/spotGUI.egg-info/SOURCES.txt
--rw-r--r--   0 bartz      (501) staff       (20)        1 2024-04-08 13:05:41.000000 spotGUI-0.5.0/src/spotGUI.egg-info/dependency_links.txt
--rw-r--r--   0 bartz      (501) staff       (20)      397 2024-04-08 13:05:41.000000 spotGUI-0.5.0/src/spotGUI.egg-info/requires.txt
--rw-r--r--   0 bartz      (501) staff       (20)        8 2024-04-08 13:05:41.000000 spotGUI-0.5.0/src/spotGUI.egg-info/top_level.txt
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-08 13:05:45.481635 spotGUI-0.5.0/test/
-drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-08 13:05:45.482243 spotGUI-0.5.0/test/__pycache__/
--rw-r--r--   0 bartz      (501) staff       (20)     1921 2024-04-08 13:05:45.482118 spotGUI-0.5.0/test/__pycache__/test_spotRun.cpython-311-pytest-7.4.4.pyc
--rw-r--r--   0 bartz      (501) staff       (20)     1255 2024-04-04 08:28:25.000000 spotGUI-0.5.0/test/test_spotRun.py
--rw-r--r--   0 bartz      (501) staff       (20)      130 2024-02-13 13:06:51.000000 spotGUI-0.5.0/tox.ini
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.646877 spotgui-0.5.1/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.578486 spotgui-0.5.1/.github/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.581374 spotgui-0.5.1/.github/workflows/
+-rw-r--r--   0 bartz      (501) staff       (20)      557 2024-02-13 13:06:51.000000 spotgui-0.5.1/.github/workflows/test.yml
+-rw-r--r--   0 bartz      (501) staff       (20)     1954 2024-03-27 21:06:14.000000 spotgui-0.5.1/.gitignore
+-rw-r--r--   0 bartz      (501) staff       (20)        0 2024-02-13 13:06:51.000000 spotgui-0.5.1/.nojekyll
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.581531 spotgui-0.5.1/.vscode/
+-rw-r--r--   0 bartz      (501) staff       (20)      823 2024-02-13 13:06:51.000000 spotgui-0.5.1/.vscode/settings.json
+-rw-r--r--   0 bartz      (501) staff       (20)    34523 2024-02-13 13:06:51.000000 spotgui-0.5.1/LICENSE.txt
+-rw-r--r--   0 bartz      (501) staff       (20)      131 2024-02-13 13:06:51.000000 spotgui-0.5.1/MANIFEST.in
+-rw-r--r--   0 bartz      (501) staff       (20)     8431 2024-04-17 20:48:33.646651 spotgui-0.5.1/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)     6814 2024-02-13 13:06:51.000000 spotgui-0.5.1/README.md
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.582707 spotgui-0.5.1/docs/
+-rw-r--r--   0 bartz      (501) staff       (20)    46499 2024-02-13 13:06:51.000000 spotgui-0.5.1/docs/about.md
+-rw-r--r--   0 bartz      (501) staff       (20)       73 2024-02-13 13:06:51.000000 spotgui-0.5.1/docs/download.md
+-rw-r--r--   0 bartz      (501) staff       (20)     1823 2024-02-13 13:06:51.000000 spotgui-0.5.1/docs/examples.md
+-rw-r--r--   0 bartz      (501) staff       (20)      947 2024-02-13 13:06:51.000000 spotgui-0.5.1/docs/gen_ref_pages.py
+-rw-r--r--   0 bartz      (501) staff       (20)      350 2024-02-13 13:06:51.000000 spotgui-0.5.1/docs/hyperparameter-tuning-cookbook.md
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.583680 spotgui-0.5.1/docs/images/
+-rw-r--r--   0 bartz      (501) staff       (20)    11605 2024-02-13 13:06:51.000000 spotgui-0.5.1/docs/images/favicon.png
+-rw-r--r--   0 bartz      (501) staff       (20)    11253 2024-02-13 13:06:51.000000 spotgui-0.5.1/docs/images/plot-progress.png
+-rw-r--r--   0 bartz      (501) staff       (20)    11605 2024-02-13 13:06:51.000000 spotgui-0.5.1/docs/images/spotlogo.png
+-rw-r--r--   0 bartz      (501) staff       (20)   122656 2024-02-13 13:06:51.000000 spotgui-0.5.1/docs/images/surrogate-plot.png
+-rw-r--r--   0 bartz      (501) staff       (20)      392 2024-02-13 13:06:51.000000 spotgui-0.5.1/docs/index.md
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.584649 spotgui-0.5.1/img/
+-rw-r--r--   0 bartz      (501) staff       (20)    11605 2024-02-13 13:06:51.000000 spotgui-0.5.1/img/favicon.png
+-rw-r--r--   0 bartz      (501) staff       (20)    67674 2024-02-13 13:06:51.000000 spotgui-0.5.1/img/spotLogo.png
+-rwxr-xr-x   0 bartz      (501) staff       (20)      114 2024-04-17 20:40:08.000000 spotgui-0.5.1/makeSpotGUI.sh
+-rw-r--r--   0 bartz      (501) staff       (20)     2026 2024-02-13 13:06:51.000000 spotgui-0.5.1/mkdocs.yml
+-rw-r--r--   0 bartz      (501) staff       (20)     1762 2024-04-17 20:38:56.000000 spotgui-0.5.1/pyproject.toml
+-rw-r--r--   0 bartz      (501) staff       (20)       38 2024-04-17 20:48:33.646912 spotgui-0.5.1/setup.cfg
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.585434 spotgui-0.5.1/spotPythonGUI/
+-rw-r--r--   0 bartz      (501) staff       (20)    13611 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotPythonGUI/00_test_spotGUI.ipynb
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.585585 spotgui-0.5.1/spotPythonGUI/images/
+-rw-r--r--   0 bartz      (501) staff       (20)     3932 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotPythonGUI/images/spotlogo.png
+-rw-r--r--   0 bartz      (501) staff       (20)    24526 2024-03-27 18:20:51.000000 spotgui-0.5.1/spotPythonGUI/spotPythonGUI.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.621537 spotgui-0.5.1/spotPythonGUI/userData/
+-rw-r--r--   0 bartz      (501) staff       (20)      698 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotPythonGUI/userData/README.txt
+-rw-r--r--   0 bartz      (501) staff       (20)     2323 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotPythonGUI/userData/data.csv
+-rw-r--r--   0 bartz      (501) staff       (20)     7422 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotPythonGUI/userData/data.pkl
+-rw-r--r--   0 bartz      (501) staff       (20) 60425445 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotPythonGUI/userData/data_sensitive.pkl
+-rw-r--r--   0 bartz      (501) staff       (20)    90292 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotPythonGUI/userData/diabetes.arff
+-rw-r--r--   0 bartz      (501) staff       (20)    88796 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotPythonGUI/userData/diabetes.csv
+-rw-r--r--   0 bartz      (501) staff       (20)    39642 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotPythonGUI/userData/diabetes.pkl
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.622323 spotgui-0.5.1/spotPythonGUI/userModel/
+-rw-r--r--   0 bartz      (501) staff       (20)        0 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotPythonGUI/userModel/__init__.py
+-rw-r--r--   0 bartz      (501) staff       (20)     2497 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotPythonGUI/userModel/netlightregression.json
+-rw-r--r--   0 bartz      (501) staff       (20)    11553 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotPythonGUI/userModel/netlightregression.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.622774 spotgui-0.5.1/spotRiverGUI/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.626288 spotgui-0.5.1/spotRiverGUI/db_dicts/
+-rw-r--r--   0 bartz      (501) staff       (20)   142672 2024-04-05 13:39:16.000000 spotgui-0.5.1/spotRiverGUI/db_dicts/0001_spotRiver_db.json
+-rw-r--r--   0 bartz      (501) staff       (20)  3433186 2024-04-04 21:00:24.000000 spotgui-0.5.1/spotRiverGUI/db_dicts/000_spotRiver_db.json
+-rw-r--r--   0 bartz      (501) staff       (20)   128965 2024-04-17 20:41:09.000000 spotgui-0.5.1/spotRiverGUI/db_dicts/spotRiver_db.json
+-rw-r--r--   0 bartz      (501) staff       (20)      404 2024-04-05 15:35:43.000000 spotgui-0.5.1/spotRiverGUI/db_dicts/spotRiver_db_default.json
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.638829 spotgui-0.5.1/spotRiverGUI/demos/
+-rw-r--r--   0 bartz      (501) staff       (20)  2142279 2024-03-17 09:55:25.000000 spotgui-0.5.1/spotRiverGUI/demos/spot_HARTR_Bike_sharing_00_experiment.pickle
+-rw-r--r--   0 bartz      (501) staff       (20) 17140699 2024-03-20 00:13:29.000000 spotgui-0.5.1/spotRiverGUI/demos/spot_HTR_Bikes_00_experiment.pickle
+-rw-r--r--   0 bartz      (501) staff       (20)   153829 2024-03-12 18:03:51.000000 spotgui-0.5.1/spotRiverGUI/demos/spot_demo_00_experiment.pickle
+-rw-r--r--   0 bartz      (501) staff       (20)   234875 2024-03-18 18:33:57.000000 spotgui-0.5.1/spotRiverGUI/demos/spot_linreg_trump_00_experiment.pickle
+-rw-r--r--   0 bartz      (501) staff       (20)   102481 2024-03-18 18:33:57.000000 spotgui-0.5.1/spotRiverGUI/demos/spot_linreg_trump_02_experiment.pickle
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.639033 spotgui-0.5.1/spotRiverGUI/images/
+-rw-r--r--   0 bartz      (501) staff       (20)     3932 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotRiverGUI/images/spotlogo.png
+-rw-r--r--   0 bartz      (501) staff       (20)    63958 2024-04-17 20:47:54.000000 spotgui-0.5.1/spotRiverGUI/spotRiverGUI.py
+-rwxr-xr-x   0 bartz      (501) staff       (20)    43139 2024-03-27 18:20:51.000000 spotgui-0.5.1/spotRiverGUI/spotRiverGUI_v01.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.642888 spotgui-0.5.1/spotRiverGUI/userData/
+-rw-r--r--   0 bartz      (501) staff       (20)    33179 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotRiverGUI/userData/PhishingData.csv
+-rw-r--r--   0 bartz      (501) staff       (20)      477 2024-02-15 08:36:58.000000 spotgui-0.5.1/spotRiverGUI/userData/PhishingData_license.txt
+-rw-r--r--   0 bartz      (501) staff       (20)  1493626 2024-03-17 22:09:34.000000 spotgui-0.5.1/spotRiverGUI/userData/bike_sharing_demand.csv
+-rw-r--r--   0 bartz      (501) staff       (20)  1633709 2024-03-17 22:09:34.000000 spotgui-0.5.1/spotRiverGUI/userData/bike_sharing_demand_lagged.csv
+-rw-r--r--   0 bartz      (501) staff       (20)  1387328 2024-03-18 23:08:42.000000 spotgui-0.5.1/spotRiverGUI/userData/bike_sharing_demand_sklearn.csv
+-rw-r--r--   0 bartz      (501) staff       (20)    42652 2024-02-15 08:36:58.000000 spotgui-0.5.1/spotRiverGUI/userData/phishingRiver.csv
+-rw-r--r--   0 bartz      (501) staff       (20)  1993321 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotRiverGUI/userData/user_data.csv
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.643942 spotgui-0.5.1/spotRiverGUI/userModel/
+-rw-r--r--   0 bartz      (501) staff       (20)        0 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotRiverGUI/userModel/__init__.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:37.290888 spotgui-0.5.1/spotRiverGUI/userPrepModel/
+-rw-r--r--   0 bartz      (501) staff       (20)        0 2024-02-14 12:30:00.000000 spotgui-0.5.1/spotRiverGUI/userPrepModel/__init__.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:37.291356 spotgui-0.5.1/spotRiverGUI/userPrepModel/__pycache__/
+-rw-r--r--   0 bartz      (501) staff       (20)     1143 2024-04-17 20:48:37.291238 spotgui-0.5.1/spotRiverGUI/userPrepModel/__pycache__/prep_test.cpython-311-pytest-7.4.4.pyc
+-rw-r--r--   0 bartz      (501) staff       (20)     1033 2024-03-27 18:20:51.000000 spotgui-0.5.1/spotRiverGUI/userPrepModel/prep_Bikes_river.py
+-rw-r--r--   0 bartz      (501) staff       (20)      288 2024-03-27 18:20:51.000000 spotgui-0.5.1/spotRiverGUI/userPrepModel/prep_generic_num_cat.py
+-rw-r--r--   0 bartz      (501) staff       (20)     1265 2024-03-27 18:20:51.000000 spotgui-0.5.1/spotRiverGUI/userPrepModel/prep_test.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.579873 spotgui-0.5.1/src/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.579714 spotgui-0.5.1/src/spotGUI/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.644435 spotgui-0.5.1/src/spotGUI/ctk/
+-rw-r--r--   0 bartz      (501) staff       (20)      720 2024-04-17 20:48:15.000000 spotgui-0.5.1/src/spotGUI/ctk/CTk.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.644540 spotgui-0.5.1/src/spotGUI/eda/
+-rw-r--r--   0 bartz      (501) staff       (20)      921 2024-02-21 13:54:55.000000 spotgui-0.5.1/src/spotGUI/eda/pairplot.py
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.644918 spotgui-0.5.1/src/spotGUI/tuner/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.645388 spotgui-0.5.1/src/spotGUI/tuner/images/
+-rw-r--r--   0 bartz      (501) staff       (20)     3932 2024-02-13 13:06:51.000000 spotgui-0.5.1/src/spotGUI/tuner/images/spotlogo.png
+-rw-r--r--   0 bartz      (501) staff       (20)    42500 2024-02-13 13:06:51.000000 spotgui-0.5.1/src/spotGUI/tuner/plot.png
+-rw-r--r--   0 bartz      (501) staff       (20)    29347 2024-04-08 13:05:32.000000 spotgui-0.5.1/src/spotGUI/tuner/spotRun.py
+-rw-r--r--   0 bartz      (501) staff       (20)    67715 2024-02-13 13:06:51.000000 spotgui-0.5.1/src/spotGUI/tuner/spot_00experiment.pickle
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:33.646325 spotgui-0.5.1/src/spotgui.egg-info/
+-rw-r--r--   0 bartz      (501) staff       (20)     8431 2024-04-17 20:48:33.000000 spotgui-0.5.1/src/spotgui.egg-info/PKG-INFO
+-rw-r--r--   0 bartz      (501) staff       (20)     2365 2024-04-17 20:48:33.000000 spotgui-0.5.1/src/spotgui.egg-info/SOURCES.txt
+-rw-r--r--   0 bartz      (501) staff       (20)        1 2024-04-17 20:48:33.000000 spotgui-0.5.1/src/spotgui.egg-info/dependency_links.txt
+-rw-r--r--   0 bartz      (501) staff       (20)      397 2024-04-17 20:48:33.000000 spotgui-0.5.1/src/spotgui.egg-info/requires.txt
+-rw-r--r--   0 bartz      (501) staff       (20)        8 2024-04-17 20:48:33.000000 spotgui-0.5.1/src/spotgui.egg-info/top_level.txt
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:37.291979 spotgui-0.5.1/test/
+drwxr-xr-x   0 bartz      (501) staff       (20)        0 2024-04-17 20:48:37.292406 spotgui-0.5.1/test/__pycache__/
+-rw-r--r--   0 bartz      (501) staff       (20)     1921 2024-04-17 20:48:37.292321 spotgui-0.5.1/test/__pycache__/test_spotRun.cpython-311-pytest-7.4.4.pyc
+-rw-r--r--   0 bartz      (501) staff       (20)     1255 2024-04-04 08:28:25.000000 spotgui-0.5.1/test/test_spotRun.py
+-rw-r--r--   0 bartz      (501) staff       (20)      130 2024-02-13 13:06:51.000000 spotgui-0.5.1/tox.ini
```

### Comparing `spotGUI-0.5.0/.github/workflows/test.yml` & `spotgui-0.5.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/.gitignore` & `spotgui-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/.vscode/settings.json` & `spotgui-0.5.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/LICENSE.txt` & `spotgui-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/PKG-INFO` & `spotgui-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: spotGUI
-Version: 0.5.0
-Summary: spotGUI - GUI for the Sequential Parameter Optimization in Python
+Name: spotgui
+Version: 0.5.1
+Summary: spotgui - GUI for the Sequential Parameter Optimization in Python
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 License: AGPL-3.0-or-later
 Project-URL: Homepage, https://www.spotseven.de
-Project-URL: Issues, https://github.com/sequential-parameter-optimization/spotGUI/issues
-Project-URL: Repository, https://github.com/sequential-parameter-optimization/spotGUI
+Project-URL: Issues, https://github.com/sequential-parameter-optimization/spotgui/issues
+Project-URL: Repository, https://github.com/sequential-parameter-optimization/spotgui
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `spotGUI-0.5.0/README.md` & `spotgui-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/docs/about.md` & `spotgui-0.5.1/docs/about.md`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/docs/examples.md` & `spotgui-0.5.1/docs/examples.md`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/docs/gen_ref_pages.py` & `spotgui-0.5.1/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/docs/images/favicon.png` & `spotgui-0.5.1/docs/images/favicon.png`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/docs/images/plot-progress.png` & `spotgui-0.5.1/docs/images/plot-progress.png`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/docs/images/spotlogo.png` & `spotgui-0.5.1/docs/images/spotlogo.png`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/docs/images/surrogate-plot.png` & `spotgui-0.5.1/docs/images/surrogate-plot.png`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/img/favicon.png` & `spotgui-0.5.1/img/favicon.png`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/img/spotLogo.png` & `spotgui-0.5.1/img/spotLogo.png`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/mkdocs.yml` & `spotgui-0.5.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/pyproject.toml` & `spotgui-0.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 requires = [
   "setuptools>=61.0",
   "setuptools_scm[toml]"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
-name = "spotGUI"
-version = "0.5.0"
+name = "spotgui"
+version = "0.5.1"
 authors = [
   { name="T. Bartz-Beielstein", email="tbb@bartzundbartz.de" }
 ]
-description = "spotGUI - GUI for the Sequential Parameter Optimization in Python"
+description = "spotgui - GUI for the Sequential Parameter Optimization in Python"
 readme = "README.md"
 license = { text="AGPL-3.0-or-later" }
 requires-python = ">=3.10"
 classifiers = [
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
@@ -55,16 +55,16 @@
   "torchmetrics",
   "torchvision",
 ]
 # dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://www.spotseven.de"
-Issues = "https://github.com/sequential-parameter-optimization/spotGUI/issues"
-Repository = "https://github.com/sequential-parameter-optimization/spotGUI"
+Issues = "https://github.com/sequential-parameter-optimization/spotgui/issues"
+Repository = "https://github.com/sequential-parameter-optimization/spotgui"
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 namespaces = true
 where = ["src"]
```

### Comparing `spotGUI-0.5.0/spotPythonGUI/00_test_spotGUI.ipynb` & `spotgui-0.5.1/spotPythonGUI/00_test_spotGUI.ipynb`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/spotPythonGUI/images/spotlogo.png` & `spotgui-0.5.1/spotPythonGUI/images/spotlogo.png`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/spotPythonGUI/spotPythonGUI.py` & `spotgui-0.5.1/spotPythonGUI/spotPythonGUI.py`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/spotPythonGUI/userData/README.txt` & `spotgui-0.5.1/spotPythonGUI/userData/README.txt`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/spotPythonGUI/userData/data.csv` & `spotgui-0.5.1/spotPythonGUI/userData/data.csv`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/spotPythonGUI/userData/data.pkl` & `spotgui-0.5.1/spotPythonGUI/userData/data.pkl`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/spotPythonGUI/userData/data_sensitive.pkl` & `spotgui-0.5.1/spotPythonGUI/userData/data_sensitive.pkl`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/spotPythonGUI/userData/diabetes.arff` & `spotgui-0.5.1/spotPythonGUI/userData/diabetes.arff`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/spotPythonGUI/userData/diabetes.csv` & `spotgui-0.5.1/spotPythonGUI/userData/diabetes.csv`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/spotPythonGUI/userData/diabetes.pkl` & `spotgui-0.5.1/spotPythonGUI/userData/diabetes.pkl`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/spotPythonGUI/userModel/netlightregression.json` & `spotgui-0.5.1/spotPythonGUI/userModel/netlightregression.json`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/spotPythonGUI/userModel/netlightregression.py` & `spotgui-0.5.1/spotPythonGUI/userModel/netlightregression.py`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/spotRiverGUI/db_dicts/0001_spotRiver_db.json` & `spotgui-0.5.1/spotRiverGUI/db_dicts/0001_spotRiver_db.json`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/spotRiverGUI/db_dicts/000_spotRiver_db.json` & `spotgui-0.5.1/spotRiverGUI/db_dicts/000_spotRiver_db.json`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/spotRiverGUI/demos/spot_HARTR_Bike_sharing_00_experiment.pickle` & `spotgui-0.5.1/spotRiverGUI/demos/spot_HARTR_Bike_sharing_00_experiment.pickle`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/spotRiverGUI/demos/spot_HTR_Bikes_00_experiment.pickle` & `spotgui-0.5.1/spotRiverGUI/demos/spot_HTR_Bikes_00_experiment.pickle`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/spotRiverGUI/demos/spot_demo_00_experiment.pickle` & `spotgui-0.5.1/spotRiverGUI/demos/spot_demo_00_experiment.pickle`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/spotRiverGUI/demos/spot_linreg_trump_00_experiment.pickle` & `spotgui-0.5.1/spotRiverGUI/demos/spot_linreg_trump_00_experiment.pickle`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/spotRiverGUI/demos/spot_linreg_trump_02_experiment.pickle` & `spotgui-0.5.1/spotRiverGUI/demos/spot_linreg_trump_02_experiment.pickle`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/spotRiverGUI/images/spotlogo.png` & `spotgui-0.5.1/spotRiverGUI/images/spotlogo.png`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/spotRiverGUI/spotRiverGUI.py` & `spotgui-0.5.1/spotRiverGUI/spotRiverGUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import webbrowser
 import os
 import numpy as np
 import copy
 import sys
 from PIL import Image
 from spotPython.utils.init import fun_control_init, design_control_init, surrogate_control_init, optimizer_control_init
+from spotGUI.ctk.CTk import CTkApp
 
 from spotRiver.data.river_hyper_dict import RiverHyperDict
 from spotGUI.tuner.spotRun import (
     run_spot_python_experiment,
     contour_plot,
     parallel_plot,
     importance_plot,
@@ -260,31 +261,31 @@
                 levels.destroy()
                 self.hp_list.remove(label)
                 self.default_list.remove(default)
                 self.lower_list.remove(levels)
                 return
 
 
-class App(customtkinter.CTk):
+class RiverApp(CTkApp):
     def __init__(self):
         super().__init__()
-        
+
         self.title("spotRiver GUI")
         self.geometry(f"{1600}x{900}")
         self.grid_columnconfigure((0, 1, 2, 3, 4), weight=1)
         self.grid_rowconfigure((0, 1), weight=1)
         self.entry_width = 80
         # dictionary name for the database
         # similar for all spotRiver experiments
         self.db_dict_name = "spotRiver_db.json"
         # name of the progress file
-        self.progress_file = "progress.txt"
+        # self.progress_file = "progress.txt"
         # if the progress file exists, delete it
-        if os.path.exists(self.progress_file):
-            os.remove(self.progress_file)
+        # if os.path.exists(self.progress_file):
+        #    os.remove(self.progress_file)
 
         current_path = os.path.dirname(os.path.abspath(__file__))
         image_path = os.path.join(current_path, "images")
         self.logo_image = customtkinter.CTkImage(Image.open(os.path.join(image_path, "spotlogo.png")), size=(85, 37))
 
         self.rhd = RiverHyperDict()
         self.task_name = "regression_tab"
@@ -292,15 +293,16 @@
         pprint.pprint(self.task_dict)
         self.core_model_name = self.task_dict[self.task_name]["core_model_names"][0]
         # Uncomment to get user defined core models (not useful for spotRiver):
         # for filename in os.listdir("userModel"):
         #     if filename.endswith(".json"):
         #         self.core_model_name.append(os.path.splitext(filename)[0])
 
-        # ---------------- Sidebar Frame --------------------------------------- #
+        # ---------------------------------------------------------------------- #
+        # ---------------- 0 Sidebar Frame --------------------------------------- #
         # ---------------------------------------------------------------------- #
         # create sidebar frame with widgets in row 0 and column 0
         self.sidebar_frame = customtkinter.CTkFrame(self, width=240, corner_radius=0)
         self.sidebar_frame.grid(row=0, column=0, sticky="nsew")
         self.sidebar_frame.grid_rowconfigure(4, weight=1)
         #
         # Inside the sidebar frame
@@ -383,16 +385,17 @@
         self.scaling_label = customtkinter.CTkLabel(self.appearance_frame, text="UI Scaling", anchor="w")
         self.scaling_label.grid(row=2, column=0, padx=20, pady=(10, 0))
         self.scaling_optionemenu = customtkinter.CTkOptionMenu(
             self.appearance_frame, values=["100%", "80%", "90%", "110%", "120%"], command=self.change_scaling_event
         )
         self.scaling_optionemenu.grid(row=3, column=0, padx=15, pady=15, sticky="ew")
         #
-        # ----------------- Experiment_Main Frame -------------------------------------- #
-        # ------------------------------------------------------------------------------ #
+        # ---------------------------------------------------------------------- #
+        # ----------------- 1 Experiment_Main Frame ------------------------------ #
+        # ---------------------------------------------------------------------- #
         # create experiment main frame with widgets in row 0 and column 1
         self.experiment_main_frame = customtkinter.CTkFrame(self, corner_radius=0)
         self.experiment_main_frame.grid(row=0, column=1, sticky="nsew")
         #
         # experiment frame title in experiment main frame
         self.experiment_main_frame_title = customtkinter.CTkLabel(
             self.experiment_main_frame,
@@ -554,16 +557,18 @@
         )
         self.oml_grace_period_label.grid(row=3, column=0, padx=0, pady=(10, 0), sticky="w")
         self.oml_grace_period_var = customtkinter.StringVar(value="None")
         self.oml_grace_period_entry = customtkinter.CTkEntry(
             self.experiment_eval_frame, textvariable=self.oml_grace_period_var, width=self.entry_width
         )
         self.oml_grace_period_entry.grid(row=3, column=1, padx=10, pady=10, sticky="w")
-        #
-        # ------------------ Hyperparameter Main Frame ------------------------------------- #
+
+        # ---------------------------------------------------------------------- #
+        # ------------------ 2 Hyperparameter Main Frame ----------------------- #
+        # ---------------------------------------------------------------------- #
         # create hyperparameter main frame with widgets in row 0 and column 2
         self.hp_main_frame = customtkinter.CTkFrame(self, corner_radius=0)
         self.hp_main_frame.grid(row=0, column=2, sticky="nsew")
         #
         # create hyperparameter title frame in hyperparameter main frame
         self.hp_main_frame_title = customtkinter.CTkLabel(
             self.hp_main_frame,
@@ -573,18 +578,20 @@
         )
         self.hp_main_frame_title.grid(row=0, column=0, padx=10, pady=10, sticky="nsew")
         #
         self.create_num_hp_frame()
         #
         self.create_cat_hp_frame()
         #
-        # ----------------- Execution_Main Frame -------------------------------------- #
+        # ---------------------------------------------------------------------- #
+        # ----------------- 3 Execution_Main Frame ----------------------------- #
+        # ---------------------------------------------------------------------- #
         # create execution_main frame with widgets in row 0 and column 4
         self.execution_main_frame = customtkinter.CTkFrame(self, corner_radius=0)
-        self.execution_main_frame.grid(row=0, column=4, sticky="nsew")
+        self.execution_main_frame.grid(row=0, column=3, sticky="nsew")
         #
         # execution frame title in execution main frame
         self.execution_main_frame_title = customtkinter.CTkLabel(
             self.execution_main_frame,
             text="Run Options",
             font=customtkinter.CTkFont(size=20, weight="bold"),
             corner_radius=6,
@@ -739,18 +746,20 @@
         self.save_button.grid(row=2, column=0, sticky="ew", padx=10, pady=10)
         # create run button
         self.run_button = customtkinter.CTkButton(
             master=self.experiment_run_frame, text="Run", command=self.run_button_event
         )
         self.run_button.grid(row=3, column=0, sticky="ew", padx=10, pady=10)
 
-        # ----------------- Analysis_Main Frame -------------------------------------- #
+        # ---------------------------------------------------------------------- #
+        # ----------------- 4 Analysis_Main Frame ------------------------------ #
+        # ---------------------------------------------------------------------- #
         # create analysis_main frame with widgets in row 0 and column 3
         self.analysis_main_frame = customtkinter.CTkFrame(self, corner_radius=0)
-        self.analysis_main_frame.grid(row=0, column=3, sticky="nsew")
+        self.analysis_main_frame.grid(row=0, column=4, sticky="nsew")
         #
         # analysis frame title in analysis main frame
         self.analysis_main_frame_title = customtkinter.CTkLabel(
             self.analysis_main_frame,
             text="Analysis",
             font=customtkinter.CTkFont(size=20, weight="bold"),
             corner_radius=6,
@@ -858,29 +867,33 @@
         self.confusion_button.grid(row=1, column=0, sticky="ew", padx=10, pady=10)
         #
         # create roc button
         self.roc_button = customtkinter.CTkButton(
             master=self.analysis_classification_frame, text="ROC", command=self.plot_roc_button_event
         )
         self.roc_button.grid(row=2, column=0, sticky="ew", padx=10, pady=10)
-        #
+
+        # ---------------------------------------------------------------------- #
         # ------------------- Textbox Frame ------------------------------------ #
+        # ---------------------------------------------------------------------- #
         # create textbox in row 1 and column 0
         self.textbox = customtkinter.CTkTextbox(self)
         self.textbox.grid(row=1, column=0, columnspan=5, padx=(10, 10), pady=10, sticky="nsew")
         self.textbox.configure(height=20, width=10)
         self.textbox.insert(tk.END, "Welcome to SPOTRiver\n")
         #
         # Start the thread that will update the text area
         # update_thread = threading.Thread(target=self.update_text, daemon=True)
         # update_thread.start()
         # e = ThreadPoolExecutor(max_workers=1)
         # e.submit(self.update_text)
         # e.shutdown(wait=False)
 
+        # ---------------------------------------------------------------------- #
+
     def print_tuned_design(self):
         text = gen_design_table(self.fun_control)
         self.textbox.delete("1.0", tk.END)
         self.textbox.insert(tk.END, text)
 
     def update_text(self):
         # This method runs in a separate thread to update the text area
@@ -926,22 +939,14 @@
     def plot_roc_button_event(self):
         if self.spot_tuner is not None:
             plot_rocs(spot_tuner=self.spot_tuner, fun_control=self.fun_control, show=True)
 
     def label_button_frame_event(self, item):
         print(f"label button frame clicked: {item}")
 
-    def change_appearance_mode_event(self, new_appearance_mode: str):
-        print(f"Appearance Mode changed to: {new_appearance_mode}")
-        customtkinter.set_appearance_mode(new_appearance_mode)
-
-    def change_scaling_event(self, new_scaling: str):
-        new_scaling_float = int(new_scaling.replace("%", "")) / 100
-        customtkinter.set_widget_scaling(new_scaling_float)
-
     def select_data_frame_event(self, new_data: str):
         print(f"Data modified: {new_data}")
         print(f"Data Selection modified: {self.select_data_frame.get_selected_optionmenu_item()}")
 
     def create_num_hp_frame(self, dict=None):
         # create new num_hp_frame
         self.num_hp_frame = NumHyperparameterFrame(
@@ -1149,40 +1154,46 @@
             self.loaded_label.configure(text=self.experiment_name)
             self.experiment_name_entry.delete(0, "end")
             self.experiment_name_entry.insert(0, self.experiment_name)
             #
             # self.print_tuned_design()
 
     def plot_data_button_event(self):
+        self.seed = int(self.seed_var.get())
+        self.test_size = float(self.test_size_var.get())
+        self.shuffle = map_to_True_False(self.shuffle_var.get())
         self.prepare_data()
         show_y_hist(train=self.train, test=self.test, target_column="y")
         # TODO: show_data
         # show_data(train=self.train,
         #           test=self.test,
         #           target_column=self.target_column,
         #           n_samples=1000)
         print("\nData shown. No result saved.")
 
-    def prepare_data(self):
+    def get_dataset(self):
         self.data_set_name = self.select_data_frame.get_selected_optionmenu_item()
-        dataset, self.n_samples = get_river_dataset_from_name(
+        self.dataset, self.n_samples = get_river_dataset_from_name(
             data_set_name=self.data_set_name,
             n_total=get_n_total(self.n_total_var.get()),
             river_datasets=self.task_dict[self.task_name]["datasets"],
         )
-        val = copy.deepcopy(dataset.iloc[0, -1])
+
+    def set_dataset_y_type(self):
+        val = copy.deepcopy(self.dataset.iloc[0, -1])
         self.target_type = check_type(val)
         if self.target_type == "bool" or self.target_type == "str":
             # convert the target column to 0 and 1
-            dataset["y"] = dataset["y"].astype(int)
-        self.test_size = float(self.test_size_var.get())
-        self.seed = int(self.seed_var.get())
-        self.shuffle = map_to_True_False(self.shuffle_var.get())
+            self.dataset["y"] = self.dataset["y"].astype(int)
+
+    def prepare_data(self):
+        self.get_dataset()
+        self.set_dataset_y_type()
         self.train, self.test, self.n_samples = split_df(
-            dataset=dataset,
+            dataset=self.dataset,
             test_size=self.test_size,
             target_type=self.target_type,
             seed=self.seed,
             shuffle=self.shuffle,
             stratify=None,
         )
 
@@ -1190,20 +1201,18 @@
         task_name = self.task_frame.get_selected_optionmenu_item()
         #
         core_model_name = self.select_core_model_frame.get_selected_optionmenu_item()
         #
         prep_model_name = self.select_prep_model_frame.get_selected_optionmenu_item()
         prepmodel = self.check_user_prep_model(prep_model_name=prep_model_name)
         #
+        self.seed = int(self.seed_var.get())
+        self.test_size = float(self.test_size_var.get())
+        self.shuffle = map_to_True_False(self.shuffle_var.get())
         self.prepare_data()
-        # data_set_name = self.select_data_frame.get_selected_optionmenu_item()
-        # dataset, n_samples = get_river_dataset_from_name(data_set_name=data_set_name,
-        #                                             n_total=get_n_total(self.n_total_var.get()),
-        #                                             river_datasets=self.task_dict[self.task_name]["datasets"])
-        #
         metric_sklearn_name = self.select_metric_sklearn_levels_frame.get_selected_optionmenu_item()
         metric_sklearn = get_metric_sklearn(self.select_metric_sklearn_levels_frame.get_selected_optionmenu_item())
         #
         n_total = get_n_total(self.n_total_var.get())
         #
         # test_size = float(self.test_size_var.get())
         #
@@ -1212,14 +1221,15 @@
         max_time = float(self.max_time_var.get())
         #
         fun_evals = get_fun_evals(self.fun_evals_var.get())
         #
         init_size = int(self.init_size_var.get())
         #
         lbd_min, lbd_max = get_lambda_min_max(self.lambda_min_max_var.get())
+        kriging_noise = get_kriging_noise(lbd_min, lbd_max)
         #
         max_surrogate_points = int(self.max_sp_var.get())
         #
         # seed = int(self.seed_var.get())
         #
         noise = map_to_True_False(self.noise_var.get())
         #
@@ -1233,25 +1243,14 @@
         oml_grace_period = get_oml_grace_period(self.oml_grace_period_var.get())
         #
         TENSORBOARD_CLEAN = map_to_True_False(self.tb_clean_var.get())
         tensorboard_start = map_to_True_False(self.tb_start_var.get())
         tensorboard_stop = map_to_True_False(self.tb_stop_var.get())
         PREFIX = self.experiment_name_entry.get()
         #
-        # val = copy.deepcopy(dataset.iloc[0, -1])
-        # target_type = check_type(val)
-        # if target_type == "bool" or target_type == "str":
-        #     # convert the target column to 0 and 1
-        #     dataset["y"] = dataset["y"].astype(int)
-        # train, test, n_samples = split_df(dataset=dataset,
-        #                                   test_size=test_size,
-        #                                   target_type=target_type,
-        #                                   seed=seed,
-        #                                   shuffle=shuffle,
-        #                                   stratify=None)
         fun_control = fun_control_init(
             PREFIX=PREFIX,
             TENSORBOARD_CLEAN=TENSORBOARD_CLEAN,
             core_model_name=core_model_name,
             data_set_name=self.data_set_name,
             db_dict_name=self.db_dict_name,
             fun_evals=fun_evals,
@@ -1298,15 +1297,15 @@
         design_control = design_control_init(
             init_size=init_size,
             repeats=1,
         )
         surrogate_control = surrogate_control_init(
             # If lambda is set to 0, no noise will be used in the surrogate
             # Otherwise use noise in the surrogate:
-            noise=get_kriging_noise(lbd_min, lbd_max),
+            noise=kriging_noise,
             n_theta=2,
             min_Lambda=lbd_min,
             max_Lambda=lbd_max,
             log_level=50,
         )
         print("surrogate_control in run_experiment():")
         pprint.pprint(surrogate_control)
@@ -1349,9 +1348,9 @@
 # Therefore, we set l1 bounds to 0.0:
 # modify_hyper_parameter_bounds(fun_control, "l1", bounds=[0.0, 0.0])
 # set_control_hyperparameter_value(fun_control, "l1", [0.0, 0.0])
 # modify_hyper_parameter_levels(fun_control, "optimizer", ["SGD"])
 
 if __name__ == "__main__":
     customtkinter.set_appearance_mode("light")
-    app = App()
+    app = RiverApp()
     app.mainloop()
```

### Comparing `spotGUI-0.5.0/spotRiverGUI/spotRiverGUI_v01.py` & `spotgui-0.5.1/spotRiverGUI/spotRiverGUI_v01.py`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/spotRiverGUI/userData/PhishingData.csv` & `spotgui-0.5.1/spotRiverGUI/userData/PhishingData.csv`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/spotRiverGUI/userData/bike_sharing_demand.csv` & `spotgui-0.5.1/spotRiverGUI/userData/bike_sharing_demand.csv`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/spotRiverGUI/userData/bike_sharing_demand_lagged.csv` & `spotgui-0.5.1/spotRiverGUI/userData/bike_sharing_demand_lagged.csv`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/spotRiverGUI/userData/bike_sharing_demand_sklearn.csv` & `spotgui-0.5.1/spotRiverGUI/userData/bike_sharing_demand_sklearn.csv`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/spotRiverGUI/userData/phishingRiver.csv` & `spotgui-0.5.1/spotRiverGUI/userData/phishingRiver.csv`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/spotRiverGUI/userData/user_data.csv` & `spotgui-0.5.1/spotRiverGUI/userData/user_data.csv`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/spotRiverGUI/userPrepModel/__pycache__/prep_test.cpython-311-pytest-7.4.4.pyc` & `spotgui-0.5.1/spotRiverGUI/userPrepModel/__pycache__/prep_test.cpython-311-pytest-7.4.4.pyc`

 * *Files 14% similar despite different names*

#### Python bytecode

```diff
@@ -62,15 +62,15 @@
      7          84 PUSH_NULL
                 86 LOAD_NAME               12 (print)
                 88 LOAD_CONST               6 ('Prep model for bike sharing demand prediction')
                 90 PRECALL                  1
                 94 CALL                     1
                104 POP_TOP
    
-    37         106 LOAD_CONST               7 (<code object set_prep_model, file "/Users/bartz/workspace/spotGUI/spotGUI-0.5.0/spotRiverGUI/userPrepModel/prep_test.py", line 37>)
+    37         106 LOAD_CONST               7 (<code object set_prep_model, file "/Users/bartz/workspace/spotGUI/spotgui-0.5.1/spotRiverGUI/userPrepModel/prep_test.py", line 37>)
                108 MAKE_FUNCTION            0
                110 STORE_NAME              13 (set_prep_model)
                112 LOAD_CONST               1 (None)
                114 RETURN_VALUE
    consts
       0
       None
@@ -134,19 +134,19 @@
             'x9'
             'x10'
             'x12'
          names      ('compose', 'Select', 'preprocessing', 'StandardScaler', 'SelectType', 'str', 'OneHotEncoder')
          varnames   ('num', 'cat', 'prepmodel')
          freevars   ()
          cellvars   ()
-         filename   '/Users/bartz/workspace/spotGUI/spotGUI-0.5.0/spotRiverGUI/userPrepModel/prep_test.py'
+         filename   '/Users/bartz/workspace/spotGUI/spotgui-0.5.1/spotRiverGUI/userPrepModel/prep_test.py'
          name       'set_prep_model'
          firstlineno 37
          lnotab 0x020156015a010a01
    names      ('builtins', '@py_builtins', '_pytest.assertion.rewrite', 'assertion', 'rewrite', '@pytest_ar', 'river', 'compose', 'preprocessing', 'feature_extraction', 'stats', 'numbers', 'print', 'set_prep_model')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/bartz/workspace/spotGUI/spotGUI-0.5.0/spotRiverGUI/userPrepModel/prep_test.py'
+   filename   '/Users/bartz/workspace/spotGUI/spotgui-0.5.1/spotRiverGUI/userPrepModel/prep_test.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020126010c010c010c010802161e
```

### Comparing `spotGUI-0.5.0/spotRiverGUI/userPrepModel/prep_Bikes_river.py` & `spotgui-0.5.1/spotRiverGUI/userPrepModel/prep_Bikes_river.py`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/spotRiverGUI/userPrepModel/prep_test.py` & `spotgui-0.5.1/spotRiverGUI/userPrepModel/prep_test.py`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/src/spotGUI/eda/pairplot.py` & `spotgui-0.5.1/src/spotGUI/eda/pairplot.py`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/src/spotGUI/tuner/images/spotlogo.png` & `spotgui-0.5.1/src/spotGUI/tuner/images/spotlogo.png`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/src/spotGUI/tuner/plot.png` & `spotgui-0.5.1/src/spotGUI/tuner/plot.png`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/src/spotGUI/tuner/spotRun.py` & `spotgui-0.5.1/src/spotGUI/tuner/spotRun.py`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/src/spotGUI/tuner/spot_00experiment.pickle` & `spotgui-0.5.1/src/spotGUI/tuner/spot_00experiment.pickle`

 * *Files identical despite different names*

### Comparing `spotGUI-0.5.0/src/spotGUI.egg-info/PKG-INFO` & `spotgui-0.5.1/src/spotgui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: spotGUI
-Version: 0.5.0
-Summary: spotGUI - GUI for the Sequential Parameter Optimization in Python
+Name: spotgui
+Version: 0.5.1
+Summary: spotgui - GUI for the Sequential Parameter Optimization in Python
 Author-email: "T. Bartz-Beielstein" <tbb@bartzundbartz.de>
 License: AGPL-3.0-or-later
 Project-URL: Homepage, https://www.spotseven.de
-Project-URL: Issues, https://github.com/sequential-parameter-optimization/spotGUI/issues
-Project-URL: Repository, https://github.com/sequential-parameter-optimization/spotGUI
+Project-URL: Issues, https://github.com/sequential-parameter-optimization/spotgui/issues
+Project-URL: Repository, https://github.com/sequential-parameter-optimization/spotgui
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `spotGUI-0.5.0/src/spotGUI.egg-info/SOURCES.txt` & `spotgui-0.5.1/src/spotgui.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -54,18 +54,19 @@
 spotRiverGUI/userData/phishingRiver.csv
 spotRiverGUI/userData/user_data.csv
 spotRiverGUI/userModel/__init__.py
 spotRiverGUI/userPrepModel/__init__.py
 spotRiverGUI/userPrepModel/prep_Bikes_river.py
 spotRiverGUI/userPrepModel/prep_generic_num_cat.py
 spotRiverGUI/userPrepModel/prep_test.py
-src/spotGUI.egg-info/PKG-INFO
-src/spotGUI.egg-info/SOURCES.txt
-src/spotGUI.egg-info/dependency_links.txt
-src/spotGUI.egg-info/requires.txt
-src/spotGUI.egg-info/top_level.txt
+src/spotGUI/ctk/CTk.py
 src/spotGUI/eda/pairplot.py
 src/spotGUI/tuner/plot.png
 src/spotGUI/tuner/spotRun.py
 src/spotGUI/tuner/spot_00experiment.pickle
 src/spotGUI/tuner/images/spotlogo.png
+src/spotgui.egg-info/PKG-INFO
+src/spotgui.egg-info/SOURCES.txt
+src/spotgui.egg-info/dependency_links.txt
+src/spotgui.egg-info/requires.txt
+src/spotgui.egg-info/top_level.txt
 test/test_spotRun.py
```

### Comparing `spotGUI-0.5.0/test/__pycache__/test_spotRun.cpython-311-pytest-7.4.4.pyc` & `spotgui-0.5.1/test/__pycache__/test_spotRun.cpython-311-pytest-7.4.4.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -76,15 +76,15 @@
      7         108 LOAD_CONST               0 (0)
                110 LOAD_CONST               7 (('spot',))
                112 IMPORT_NAME             20 (spotPython.spot)
                114 IMPORT_FROM             21 (spot)
                116 STORE_NAME              21 (spot)
                118 POP_TOP
    
-    10         120 LOAD_CONST               8 (<code object test_run_spot_python_experiment_save_only, file "/Users/bartz/workspace/spotGUI/spotGUI-0.5.0/test/test_spotRun.py", line 10>)
+    10         120 LOAD_CONST               8 (<code object test_run_spot_python_experiment_save_only, file "/Users/bartz/workspace/spotGUI/spotgui-0.5.1/test/test_spotRun.py", line 10>)
                122 MAKE_FUNCTION            0
                124 STORE_NAME              22 (test_run_spot_python_experiment_save_only)
                126 LOAD_CONST               1 (None)
                128 RETURN_VALUE
    consts
       0
       None
@@ -209,21 +209,21 @@
             ('PREFIX',)
             ('fun_control', 'core_model', 'hyper_dict')
             'run_spot_python_experiment(save_only) raised an exception: '
          names      ('fun_control_init', 'design_control_init', 'surrogate_control_init', 'optimizer_control_init', 'add_core_model_to_fun_control', 'NetLightRegression', 'LightHyperDict', 'run_spot_python_experiment', 'Exception', 'pytest', 'fail')
          varnames   ('save_only', 'fun_control', 'design_control', 'surrogate_control', 'optimizer_control', 'e')
          freevars   ()
          cellvars   ()
-         filename   '/Users/bartz/workspace/spotGUI/spotGUI-0.5.0/test/test_spotRun.py'
+         filename   '/Users/bartz/workspace/spotGUI/spotgui-0.5.1/test/test_spotRun.py'
          name       'test_run_spot_python_experiment_save_only'
          firstlineno 10
          lnotab
             0x0202040120011c011c011c02380302010c01020102010201020102fb16
             07120142ff
    names      ('builtins', '@py_builtins', '_pytest.assertion.rewrite', 'assertion', 'rewrite', '@pytest_ar', 'pytest', 'spotGUI.tuner.spotRun', 'run_spot_python_experiment', 'spotPython.utils.init', 'fun_control_init', 'design_control_init', 'surrogate_control_init', 'optimizer_control_init', 'spotPython.light.regression.netlightregression', 'NetLightRegression', 'spotPython.hyperdict.light_hyper_dict', 'LightHyperDict', 'spotPython.hyperparameters.values', 'add_core_model_to_fun_control', 'spotPython.spot', 'spot', 'test_run_spot_python_experiment_save_only')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/bartz/workspace/spotGUI/spotGUI-0.5.0/test/test_spotRun.py'
+   filename   '/Users/bartz/workspace/spotGUI/spotgui-0.5.1/test/test_spotRun.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020122010c0118010c010c010c010c03
```

### Comparing `spotGUI-0.5.0/test/test_spotRun.py` & `spotgui-0.5.1/test/test_spotRun.py`

 * *Files identical despite different names*

