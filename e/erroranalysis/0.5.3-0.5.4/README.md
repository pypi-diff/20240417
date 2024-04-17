# Comparing `tmp/erroranalysis-0.5.3.tar.gz` & `tmp/erroranalysis-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erroranalysis-0.5.3.tar", last modified: Fri Dec 22 19:33:49 2023, max compression
+gzip compressed data, was "erroranalysis-0.5.4.tar", last modified: Wed Apr 17 04:42:04 2024, max compression
```

## Comparing `erroranalysis-0.5.3.tar` & `erroranalysis-0.5.4.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 19:33:49.031963 erroranalysis-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2023-12-22 19:33:49.031963 erroranalysis-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 19:33:49.027963 erroranalysis-0.5.3/erroranalysis/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/erroranalysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 19:33:49.027963 erroranalysis-0.5.3/erroranalysis/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/erroranalysis/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20250 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/erroranalysis/_internal/cohort_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6632 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/erroranalysis/_internal/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 19:33:49.027963 erroranalysis-0.5.3/erroranalysis/_internal/error_analyzer/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/erroranalysis/_internal/error_analyzer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 19:33:49.031963 erroranalysis-0.5.3/erroranalysis/_internal/error_report/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/erroranalysis/_internal/error_report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35409 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/erroranalysis/_internal/matrix_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8917 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/erroranalysis/_internal/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/erroranalysis/_internal/process_categoricals.py
--rw-r--r--   0 runner    (1001) docker     (127)    43602 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/erroranalysis/_internal/surrogate_error_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/erroranalysis/_internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/erroranalysis/_internal/version_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 19:33:49.031963 erroranalysis-0.5.3/erroranalysis/analyzer/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/erroranalysis/analyzer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33657 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/erroranalysis/analyzer/error_analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 19:33:49.031963 erroranalysis-0.5.3/erroranalysis/error_correlation_methods/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/erroranalysis/error_correlation_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/erroranalysis/error_correlation_methods/ebm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/erroranalysis/error_correlation_methods/gbm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 19:33:49.031963 erroranalysis-0.5.3/erroranalysis/report/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/erroranalysis/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7895 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/erroranalysis/report/error_report.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/erroranalysis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 19:33:49.031963 erroranalysis-0.5.3/erroranalysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2023-12-22 19:33:48.000000 erroranalysis-0.5.3/erroranalysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2023-12-22 19:33:48.000000 erroranalysis-0.5.3/erroranalysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 19:33:48.000000 erroranalysis-0.5.3/erroranalysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2023-12-22 19:33:48.000000 erroranalysis-0.5.3/erroranalysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-12-22 19:33:48.000000 erroranalysis-0.5.3/erroranalysis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-22 19:33:49.031963 erroranalysis-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 19:33:49.031963 erroranalysis-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    18507 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/tests/test_cohort_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/tests/test_error_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     9599 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/tests/test_importances.py
--rw-r--r--   0 runner    (1001) docker     (127)    32680 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/tests/test_matrix_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/tests/test_pyspark_surrogate_error_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     5184 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/tests/test_root_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    21666 2023-12-22 19:33:12.000000 erroranalysis-0.5.3/tests/test_surrogate_error_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:42:04.351643 erroranalysis-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-17 04:42:04.351643 erroranalysis-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:42:04.347643 erroranalysis-0.5.4/erroranalysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/erroranalysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:42:04.347643 erroranalysis-0.5.4/erroranalysis/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/erroranalysis/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20250 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/erroranalysis/_internal/cohort_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6632 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/erroranalysis/_internal/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:42:04.347643 erroranalysis-0.5.4/erroranalysis/_internal/error_analyzer/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/erroranalysis/_internal/error_analyzer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:42:04.347643 erroranalysis-0.5.4/erroranalysis/_internal/error_report/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/erroranalysis/_internal/error_report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35409 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/erroranalysis/_internal/matrix_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8917 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/erroranalysis/_internal/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/erroranalysis/_internal/process_categoricals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43602 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/erroranalysis/_internal/surrogate_error_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/erroranalysis/_internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/erroranalysis/_internal/version_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:42:04.351643 erroranalysis-0.5.4/erroranalysis/analyzer/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/erroranalysis/analyzer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33657 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/erroranalysis/analyzer/error_analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:42:04.351643 erroranalysis-0.5.4/erroranalysis/error_correlation_methods/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/erroranalysis/error_correlation_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/erroranalysis/error_correlation_methods/ebm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/erroranalysis/error_correlation_methods/gbm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:42:04.351643 erroranalysis-0.5.4/erroranalysis/report/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/erroranalysis/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/erroranalysis/report/error_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/erroranalysis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:42:04.351643 erroranalysis-0.5.4/erroranalysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-17 04:42:04.000000 erroranalysis-0.5.4/erroranalysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-17 04:42:04.000000 erroranalysis-0.5.4/erroranalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 04:42:04.000000 erroranalysis-0.5.4/erroranalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-17 04:42:04.000000 erroranalysis-0.5.4/erroranalysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-17 04:42:04.000000 erroranalysis-0.5.4/erroranalysis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/requirements-object-detection.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 04:42:04.351643 erroranalysis-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 04:42:04.351643 erroranalysis-0.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/tests/test_cohort_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/tests/test_error_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/tests/test_importances.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32680 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/tests/test_matrix_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/tests/test_pyspark_surrogate_error_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/tests/test_root_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21666 2024-04-17 04:41:26.000000 erroranalysis-0.5.4/tests/test_surrogate_error_tree.py
```

### Comparing `erroranalysis-0.5.3/LICENSE` & `erroranalysis-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.5.3/PKG-INFO` & `erroranalysis-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erroranalysis
-Version: 0.5.3
+Version: 0.5.4
 Summary: Core error analysis APIs
 Home-page: https://github.com/microsoft/responsible-ai-widgets
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.17.2
 Requires-Dist: pandas<2.0.0,>=0.25.1
 Requires-Dist: scipy>=1.4.1
 Requires-Dist: scikit-learn>=0.22.1
 Requires-Dist: lightgbm>=2.0.11
-Requires-Dist: raiutils>=0.4.0
+Requires-Dist: raiutils>=0.4.2
 Provides-Extra: object-detection
 Requires-Dist: vision_explanation_methods; extra == "object-detection"
 
 # Error Analysis SDK for Python
 
 ### This package has been tested with Python 3.7, 3.8, 3.9, 3.10 and 3.11
```

### Comparing `erroranalysis-0.5.3/README.md` & `erroranalysis-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.5.3/erroranalysis/_internal/cohort_filter.py` & `erroranalysis-0.5.4/erroranalysis/_internal/cohort_filter.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.5.3/erroranalysis/_internal/constants.py` & `erroranalysis-0.5.4/erroranalysis/_internal/constants.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.5.3/erroranalysis/_internal/matrix_filter.py` & `erroranalysis-0.5.4/erroranalysis/_internal/matrix_filter.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.5.3/erroranalysis/_internal/metrics.py` & `erroranalysis-0.5.4/erroranalysis/_internal/metrics.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.5.3/erroranalysis/_internal/process_categoricals.py` & `erroranalysis-0.5.4/erroranalysis/_internal/process_categoricals.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.5.3/erroranalysis/_internal/surrogate_error_tree.py` & `erroranalysis-0.5.4/erroranalysis/_internal/surrogate_error_tree.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.5.3/erroranalysis/_internal/utils.py` & `erroranalysis-0.5.4/erroranalysis/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.5.3/erroranalysis/_internal/version_checker.py` & `erroranalysis-0.5.4/erroranalysis/_internal/version_checker.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.5.3/erroranalysis/analyzer/error_analyzer.py` & `erroranalysis-0.5.4/erroranalysis/analyzer/error_analyzer.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.5.3/erroranalysis/error_correlation_methods/ebm.py` & `erroranalysis-0.5.4/erroranalysis/error_correlation_methods/ebm.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.5.3/erroranalysis/error_correlation_methods/gbm.py` & `erroranalysis-0.5.4/erroranalysis/error_correlation_methods/gbm.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,32 +8,37 @@
 from lightgbm import LGBMClassifier, LGBMRegressor
 
 from erroranalysis._internal.constants import ModelTask
 
 
 def compute_gbm_global_importance(input_data, diff, model_task,
                                   categorical_indexes):
-    """Compute global importance score for EBM between the features and error.
-    :param input_data: The input data to compute the EBM global importance
+    """Compute global importance score for GBM between the features and error.
+    :param input_data: The input data to compute the GBM global importance
         score on.
     :type input_data: numpy.ndarray
     :param diff: The difference between the label and prediction
         columns.
     :type diff: numpy.ndarray
     :param model_task: The model task.
     :type model_task: str
-    :return: The computed EBM global importance score between the features and
+    :return: The computed GBM global importance score between the features and
         error.
     :rtype: list[float]
     """
     is_classification = model_task == ModelTask.CLASSIFICATION
     if is_classification:
         model = LGBMClassifier()
     else:
         model = LGBMRegressor()
     model.fit(input_data, diff, categorical_feature=categorical_indexes)
     explainer = shap.TreeExplainer(model)
     shap_values = explainer.shap_values(input_data)
+    dims = np.shape(shap_values)
+    # fix some inconsistencies in the shape of the shap_values
+    # for newer versions of shap>=0.45.0 for single-valued target column
+    if is_classification and len(dims) == 2:
+        shap_values = np.expand_dims(shap_values, axis=0)
     shap_mean_abs = np.abs(shap_values).mean(axis=0)
     if is_classification:
         shap_mean_abs = shap_mean_abs.mean(axis=0)
     return shap_mean_abs.tolist()
```

### Comparing `erroranalysis-0.5.3/erroranalysis/report/error_report.py` & `erroranalysis-0.5.4/erroranalysis/report/error_report.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.5.3/erroranalysis.egg-info/PKG-INFO` & `erroranalysis-0.5.4/erroranalysis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erroranalysis
-Version: 0.5.3
+Version: 0.5.4
 Summary: Core error analysis APIs
 Home-page: https://github.com/microsoft/responsible-ai-widgets
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.17.2
 Requires-Dist: pandas<2.0.0,>=0.25.1
 Requires-Dist: scipy>=1.4.1
 Requires-Dist: scikit-learn>=0.22.1
 Requires-Dist: lightgbm>=2.0.11
-Requires-Dist: raiutils>=0.4.0
+Requires-Dist: raiutils>=0.4.2
 Provides-Extra: object-detection
 Requires-Dist: vision_explanation_methods; extra == "object-detection"
 
 # Error Analysis SDK for Python
 
 ### This package has been tested with Python 3.7, 3.8, 3.9, 3.10 and 3.11
```

### Comparing `erroranalysis-0.5.3/erroranalysis.egg-info/SOURCES.txt` & `erroranalysis-0.5.4/erroranalysis.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+requirements-object-detection.txt
 requirements.txt
 setup.py
 erroranalysis/__init__.py
 erroranalysis/version.py
 erroranalysis.egg-info/PKG-INFO
 erroranalysis.egg-info/SOURCES.txt
 erroranalysis.egg-info/dependency_links.txt
```

### Comparing `erroranalysis-0.5.3/setup.py` & `erroranalysis-0.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.5.3/tests/test_cohort_filter.py` & `erroranalysis-0.5.4/tests/test_cohort_filter.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.5.3/tests/test_error_report.py` & `erroranalysis-0.5.4/tests/test_error_report.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.5.3/tests/test_importances.py` & `erroranalysis-0.5.4/tests/test_importances.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.5.3/tests/test_matrix_filter.py` & `erroranalysis-0.5.4/tests/test_matrix_filter.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.5.3/tests/test_metrics.py` & `erroranalysis-0.5.4/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.5.3/tests/test_pyspark_surrogate_error_tree.py` & `erroranalysis-0.5.4/tests/test_pyspark_surrogate_error_tree.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.5.3/tests/test_root_stats.py` & `erroranalysis-0.5.4/tests/test_root_stats.py`

 * *Files identical despite different names*

### Comparing `erroranalysis-0.5.3/tests/test_surrogate_error_tree.py` & `erroranalysis-0.5.4/tests/test_surrogate_error_tree.py`

 * *Files identical despite different names*

