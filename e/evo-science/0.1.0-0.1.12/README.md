# Comparing `tmp/evo-science-0.1.0.tar.gz` & `tmp/evo_science-0.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evo-science-0.1.0.tar", last modified: Thu Mar 14 06:20:09 2024, max compression
+gzip compressed data, was "evo_science-0.1.12.tar", last modified: Wed Apr 17 02:47:13 2024, max compression
```

## Comparing `evo-science-0.1.0.tar` & `evo_science-0.1.12.tar`

### file list

```diff
@@ -1,55 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 06:20:09.472062 evo-science-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-14 06:19:53.000000 evo-science-0.1.0/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-14 06:19:53.000000 evo-science-0.1.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-14 06:19:53.000000 evo-science-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-14 06:19:53.000000 evo-science-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-03-14 06:20:09.472062 evo-science-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-03-14 06:19:53.000000 evo-science-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 06:20:09.468062 evo-science-0.1.0/evo_science/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-14 06:19:53.000000 evo-science-0.1.0/evo_science/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-14 06:19:53.000000 evo-science-0.1.0/evo_science/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-14 06:19:53.000000 evo-science-0.1.0/evo_science/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-14 06:19:53.000000 evo-science-0.1.0/evo_science/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-14 06:19:53.000000 evo-science-0.1.0/evo_science/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-14 06:19:53.000000 evo-science-0.1.0/evo_science/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 06:20:09.468062 evo-science-0.1.0/evo_science/entities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 06:19:53.000000 evo-science-0.1.0/evo_science/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-14 06:19:53.000000 evo-science-0.1.0/evo_science/entities/cpa_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 06:20:09.468062 evo-science-0.1.0/evo_science/entities/features/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 06:19:53.000000 evo-science-0.1.0/evo_science/entities/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-03-14 06:19:53.000000 evo-science-0.1.0/evo_science/entities/features/base_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-03-14 06:19:53.000000 evo-science-0.1.0/evo_science/entities/features/feature_set.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-14 06:19:53.000000 evo-science-0.1.0/evo_science/entities/features/feature_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 06:20:09.472062 evo-science-0.1.0/evo_science/entities/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-14 06:19:53.000000 evo-science-0.1.0/evo_science/entities/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-03-14 06:19:53.000000 evo-science-0.1.0/evo_science/entities/metrics/base_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-14 06:19:53.000000 evo-science-0.1.0/evo_science/entities/metrics/error_ave.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-14 06:19:53.000000 evo-science-0.1.0/evo_science/entities/metrics/error_std.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-14 06:19:53.000000 evo-science-0.1.0/evo_science/entities/metrics/intercept.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-14 06:19:53.000000 evo-science-0.1.0/evo_science/entities/metrics/mae.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-14 06:19:53.000000 evo-science-0.1.0/evo_science/entities/metrics/mse.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-14 06:19:53.000000 evo-science-0.1.0/evo_science/entities/metrics/r_squared.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-14 06:19:53.000000 evo-science-0.1.0/evo_science/entities/metrics/rmse.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-14 06:19:53.000000 evo-science-0.1.0/evo_science/entities/metrics/slope.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 06:20:09.472062 evo-science-0.1.0/evo_science/entities/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 06:19:53.000000 evo-science-0.1.0/evo_science/entities/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-03-14 06:19:53.000000 evo-science-0.1.0/evo_science/entities/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-03-14 06:19:53.000000 evo-science-0.1.0/evo_science/entities/models/decision_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-03-14 06:19:53.000000 evo-science-0.1.0/evo_science/entities/models/linear_regression_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-14 06:19:53.000000 evo-science-0.1.0/evo_science/entities/models/logistic_regression_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-14 06:19:53.000000 evo-science-0.1.0/evo_science/entities/models/xg_boost.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-14 06:19:53.000000 evo-science-0.1.0/evo_science/metric_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 06:20:09.472062 evo-science-0.1.0/evo_science.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-03-14 06:20:09.000000 evo-science-0.1.0/evo_science.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-03-14 06:20:09.000000 evo-science-0.1.0/evo_science.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 06:20:09.000000 evo-science-0.1.0/evo_science.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-14 06:20:09.000000 evo-science-0.1.0/evo_science.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-14 06:20:09.000000 evo-science-0.1.0/evo_science.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-14 06:20:09.000000 evo-science-0.1.0/evo_science.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 06:20:09.472062 evo-science-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-03-14 06:19:53.000000 evo-science-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 06:20:09.472062 evo-science-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 06:19:53.000000 evo-science-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-14 06:19:53.000000 evo-science-0.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-14 06:19:53.000000 evo-science-0.1.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-14 06:19:53.000000 evo-science-0.1.0/tests/test_execute_lr_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:47:13.349712 evo_science-0.1.12/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-17 02:47:04.000000 evo_science-0.1.12/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-17 02:47:04.000000 evo_science-0.1.12/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-17 02:47:04.000000 evo_science-0.1.12/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-17 02:47:04.000000 evo_science-0.1.12/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-17 02:47:13.349712 evo_science-0.1.12/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-17 02:47:04.000000 evo_science-0.1.12/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:47:13.341711 evo_science-0.1.12/evo_science/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:47:13.341711 evo_science-0.1.12/evo_science/entities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/entities/evs_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:47:13.341711 evo_science-0.1.12/evo_science/entities/features/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/entities/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/entities/features/base_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/entities/features/feature_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/entities/features/feature_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:47:13.345711 evo_science-0.1.12/evo_science/entities/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/entities/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/entities/metrics/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/entities/metrics/auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/entities/metrics/base_binary_classify_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/entities/metrics/base_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/entities/metrics/error_ave.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/entities/metrics/error_std.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/entities/metrics/f1_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/entities/metrics/intercept.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/entities/metrics/mae.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/entities/metrics/mse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/entities/metrics/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/entities/metrics/r_squared.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/entities/metrics/recall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/entities/metrics/rmse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/entities/metrics/roc_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/entities/metrics/slope.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:47:13.345711 evo_science-0.1.12/evo_science/entities/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/entities/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/entities/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/entities/models/decision_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/entities/models/linear_regression_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/entities/models/logistic_regression_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/entities/models/xg_boost.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-17 02:47:04.000000 evo_science-0.1.12/evo_science/metric_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:47:13.345711 evo_science-0.1.12/evo_science.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-17 02:47:13.000000 evo_science-0.1.12/evo_science.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-17 02:47:13.000000 evo_science-0.1.12/evo_science.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 02:47:13.000000 evo_science-0.1.12/evo_science.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-17 02:47:13.000000 evo_science-0.1.12/evo_science.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-17 02:47:13.000000 evo_science-0.1.12/evo_science.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 02:47:13.000000 evo_science-0.1.12/evo_science.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 02:47:13.349712 evo_science-0.1.12/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-17 02:47:04.000000 evo_science-0.1.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:47:13.345711 evo_science-0.1.12/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:47:04.000000 evo_science-0.1.12/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-17 02:47:04.000000 evo_science-0.1.12/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-17 02:47:04.000000 evo_science-0.1.12/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-17 02:47:04.000000 evo_science-0.1.12/tests/test_execute_lr_example.py
```

### Comparing `evo-science-0.1.0/LICENSE` & `evo_science-0.1.12/LICENSE`

 * *Files identical despite different names*

### Comparing `evo-science-0.1.0/PKG-INFO` & `evo_science-0.1.12/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: evo-science
-Version: 0.1.0
+Version: 0.1.12
 Summary: Awesome evo_science created by maycuatroi
 Home-page: https://github.com/maycuatroi/evo-science/
 Author: maycuatroi
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scikit-learn
 Requires-Dist: matplotlib
 Requires-Dist: xgboost
 Requires-Dist: dtreeviz
 Requires-Dist: tabulate
 Requires-Dist: seaborn
 Requires-Dist: pandas
+Requires-Dist: python-dotenv
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: isort; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: codecov; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: gitchangelog; extra == "test"
 Requires-Dist: mkdocs; extra == "test"
+Provides-Extra: keras
+Requires-Dist: jax[cuda12_pip]; extra == "keras"
+Requires-Dist: keras; extra == "keras"
 
 # Evolution Science
 
 [![codecov](https://codecov.io/gh/maycuatroi/evo-science/branch/main/graph/badge.svg?token=evo-science_token_here)](https://codecov.io/gh/maycuatroi/evo-science)
 [![CI](https://github.com/maycuatroi/evo-science/actions/workflows/main.yml/badge.svg)](https://github.com/maycuatroi/evo-science/actions/workflows/main.yml)
 
 Awesome evo_science created by maycuatroi
```

### Comparing `evo-science-0.1.0/README.md` & `evo_science-0.1.12/README.md`

 * *Files identical despite different names*

### Comparing `evo-science-0.1.0/evo_science/cli.py` & `evo_science-0.1.12/evo_science/cli.py`

 * *Files identical despite different names*

### Comparing `evo-science-0.1.0/evo_science/entities/features/base_feature.py` & `evo_science-0.1.12/evo_science/entities/features/base_feature.py`

 * *Files identical despite different names*

### Comparing `evo-science-0.1.0/evo_science/entities/features/feature_set.py` & `evo_science-0.1.12/evo_science/entities/features/feature_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing
 
 import numpy as np
 import pandas as pd
 from tabulate import tabulate
 
 from evo_science import BaseFeature
-from evo_science.entities.cpa_logger import EvoScienceLogger
+from evo_science.entities.evs_logger import EvoScienceLogger
 
 
 class FeatureSet:
     def __init__(
         self,
         features: typing.List["BaseFeature | type"],
         auto_skip_nan: bool = True,
```

### Comparing `evo-science-0.1.0/evo_science/entities/metrics/base_metric.py` & `evo_science-0.1.12/evo_science/entities/metrics/base_metric.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-import numpy as np
-
 import typing
 
+import numpy as np
+
 if typing.TYPE_CHECKING:
     from evo_science import BaseModel, FeatureSet, BaseFeature
 
 
 class BaseMetric:
     name = "base_metric"
 
     def __init__(
         self,
-        model: "BaseModel",
-        feature_set: "FeatureSet",
-        target_feature: "BaseFeature",
+        model: "BaseModel" = None,
+        feature_set: "FeatureSet" = None,
+        target_feature: "BaseFeature" = None,
+        **kwargs
     ):
         self.feature_set = feature_set
         self.target_feature = target_feature
         self.model = model
+        self._on_init(**kwargs)
 
     def _calculate_np(self, y_true: np.array, y_pred: np.array):
         """
         Calculate the metric using numpy arrays.
         Args:
             y_true (np.array): True target values.
             y_pred (np.array): Predicted target values.
@@ -37,7 +39,17 @@
         Returns:
             float: Slope of the model predictions.
         """
         y_true_np = self.target_feature.to_numpy(is_train=False)
         y_pred_np = self.model.predict(self.feature_set.to_numpy(is_train=False))
 
         return self._calculate_np(y_true_np, y_pred_np)
+
+    def _on_call(self, *args, **kwargs):
+        pass
+
+    def __call__(self, *args, **kwargs):
+        self._on_call()
+        return self
+
+    def _on_init(self):
+        pass
```

### Comparing `evo-science-0.1.0/evo_science/entities/models/base_model.py` & `evo_science-0.1.12/evo_science/entities/models/base_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 from evo_science import FeatureSet
 from evo_science.entities.metrics import BaseMetric
 from evo_science.metric_lib import MetricLib
 
 
 class BaseModel:
-
     def __init__(self, **kwargs):
         self.model = None
 
     def fit(self, x: FeatureSet, y: FeatureSet):
         """
         Fit the model to the data.
 
@@ -60,27 +59,29 @@
         table_records = []
         for i, metric in enumerate(metrics):
             if isinstance(metric, str):
                 metric: type = MetricLib.get_metric(metric)
                 metrics[i] = metric(model=self, feature_set=x, target_feature=y)
             elif isinstance(metric, type):
                 metrics[i] = metric(model=self, feature_set=x, target_feature=y)
+            elif issubclass(metric.__class__, BaseMetric):
+                metric.model = self
+                metric.feature_set = x
+                metric.target_feature = y
             else:
                 assert issubclass(
                     metric.__class__, BaseMetric
                 ), f"{metric.__class__.__name__} is not a subclass of BaseMetric"
 
         for metric in metrics:
             metric_value = metric.calculate()
             table_records.append([metric.name, metric_value])
 
         table = tabulate(
-            tabular_data=table_records,
-            headers=["Metric", "Value"],
-            tablefmt="orgtbl",
+            tabular_data=table_records, headers=["Metric", "Value"], tablefmt="orgtbl",
         )
         print(table)
 
     def calculate_coefficients(self, x: FeatureSet) -> pd.DataFrame:
         """
         Get the coefficients of the features x to the target y.
         """
```

### Comparing `evo-science-0.1.0/evo_science/entities/models/linear_regression_model.py` & `evo_science-0.1.12/evo_science/entities/models/linear_regression_model.py`

 * *Files identical despite different names*

### Comparing `evo-science-0.1.0/evo_science/entities/models/xg_boost.py` & `evo_science-0.1.12/evo_science/entities/models/xg_boost.py`

 * *Files identical despite different names*

### Comparing `evo-science-0.1.0/evo_science.egg-info/PKG-INFO` & `evo_science-0.1.12/evo_science.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: evo-science
-Version: 0.1.0
+Version: 0.1.12
 Summary: Awesome evo_science created by maycuatroi
 Home-page: https://github.com/maycuatroi/evo-science/
 Author: maycuatroi
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scikit-learn
 Requires-Dist: matplotlib
 Requires-Dist: xgboost
 Requires-Dist: dtreeviz
 Requires-Dist: tabulate
 Requires-Dist: seaborn
 Requires-Dist: pandas
+Requires-Dist: python-dotenv
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: isort; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: codecov; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: gitchangelog; extra == "test"
 Requires-Dist: mkdocs; extra == "test"
+Provides-Extra: keras
+Requires-Dist: jax[cuda12_pip]; extra == "keras"
+Requires-Dist: keras; extra == "keras"
 
 # Evolution Science
 
 [![codecov](https://codecov.io/gh/maycuatroi/evo-science/branch/main/graph/badge.svg?token=evo-science_token_here)](https://codecov.io/gh/maycuatroi/evo-science)
 [![CI](https://github.com/maycuatroi/evo-science/actions/workflows/main.yml/badge.svg)](https://github.com/maycuatroi/evo-science/actions/workflows/main.yml)
 
 Awesome evo_science created by maycuatroi
```

### Comparing `evo-science-0.1.0/evo_science.egg-info/SOURCES.txt` & `evo_science-0.1.12/evo_science.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -14,28 +14,35 @@
 evo_science.egg-info/PKG-INFO
 evo_science.egg-info/SOURCES.txt
 evo_science.egg-info/dependency_links.txt
 evo_science.egg-info/entry_points.txt
 evo_science.egg-info/requires.txt
 evo_science.egg-info/top_level.txt
 evo_science/entities/__init__.py
-evo_science/entities/cpa_logger.py
+evo_science/entities/evs_logger.py
 evo_science/entities/features/__init__.py
 evo_science/entities/features/base_feature.py
 evo_science/entities/features/feature_set.py
 evo_science/entities/features/feature_types.py
 evo_science/entities/metrics/__init__.py
+evo_science/entities/metrics/accuracy.py
+evo_science/entities/metrics/auc.py
+evo_science/entities/metrics/base_binary_classify_metric.py
 evo_science/entities/metrics/base_metric.py
 evo_science/entities/metrics/error_ave.py
 evo_science/entities/metrics/error_std.py
+evo_science/entities/metrics/f1_score.py
 evo_science/entities/metrics/intercept.py
 evo_science/entities/metrics/mae.py
 evo_science/entities/metrics/mse.py
+evo_science/entities/metrics/precision.py
 evo_science/entities/metrics/r_squared.py
+evo_science/entities/metrics/recall.py
 evo_science/entities/metrics/rmse.py
+evo_science/entities/metrics/roc_curve.py
 evo_science/entities/metrics/slope.py
 evo_science/entities/models/__init__.py
 evo_science/entities/models/base_model.py
 evo_science/entities/models/decision_tree.py
 evo_science/entities/models/linear_regression_model.py
 evo_science/entities/models/logistic_regression_model.py
 evo_science/entities/models/xg_boost.py
```

### Comparing `evo-science-0.1.0/setup.py` & `evo_science-0.1.12/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,9 +37,12 @@
     url="https://github.com/maycuatroi/evo-science/",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     author="maycuatroi",
     packages=find_packages(exclude=["tests", ".github"]),
     install_requires=read_requirements("requirements.txt"),
     entry_points={"console_scripts": ["evo_science = evo_science.__main__:main"]},
-    extras_require={"test": read_requirements("requirements-test.txt")},
+    extras_require={
+        "test": read_requirements("requirements-test.txt"),
+        "keras": read_requirements("requirements-keras.txt"),
+    },
 )
```

