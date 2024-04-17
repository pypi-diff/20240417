# Comparing `tmp/fhdw_modelling-7.2.0.tar.gz` & `tmp/fhdw_modelling-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fhdw_modelling-7.2.0.tar", max compression
+gzip compressed data, was "fhdw_modelling-7.2.1.tar", max compression
```

## Comparing `fhdw_modelling-7.2.0.tar` & `fhdw_modelling-7.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     3234 2024-03-07 15:23:05.955446 fhdw_modelling-7.2.0/README.md
--rw-r--r--   0        0        0       35 2024-03-07 15:23:05.959446 fhdw_modelling-7.2.0/fhdw/modelling/__init__.py
--rw-r--r--   0        0        0     1474 2024-03-07 15:23:05.959446 fhdw_modelling-7.2.0/fhdw/modelling/base.py
--rw-r--r--   0        0        0     7397 2024-03-07 15:23:05.959446 fhdw_modelling-7.2.0/fhdw/modelling/evaluation.py
--rw-r--r--   0        0        0     3239 2024-03-07 15:23:05.959446 fhdw_modelling-7.2.0/fhdw/modelling/preprocessing.py
--rw-r--r--   0        0        0    14394 2024-03-07 15:23:05.959446 fhdw_modelling-7.2.0/fhdw/modelling/pycaret.py
--rw-r--r--   0        0        0     5160 2024-03-07 15:23:05.959446 fhdw_modelling-7.2.0/fhdw/modelling/tracking.py
--rw-r--r--   0        0        0       22 2024-03-07 15:23:05.959446 fhdw_modelling-7.2.0/fhdw/tests/__init__.py
--rw-r--r--   0        0        0      328 2024-03-07 15:23:05.959446 fhdw_modelling-7.2.0/fhdw/tests/conftest.py
--rw-r--r--   0        0        0     6613 2024-03-07 15:23:05.959446 fhdw_modelling-7.2.0/fhdw/tests/data/automobile.csv
--rw-r--r--   0        0        0     3246 2024-03-07 15:23:05.959446 fhdw_modelling-7.2.0/fhdw/tests/test_base.py
--rw-r--r--   0        0        0     5356 2024-03-07 15:23:05.959446 fhdw_modelling-7.2.0/fhdw/tests/test_evaluation.py
--rw-r--r--   0        0        0      854 2024-03-07 15:23:05.959446 fhdw_modelling-7.2.0/fhdw/tests/test_preprocessing.py
--rw-r--r--   0        0        0     9950 2024-03-07 15:23:05.959446 fhdw_modelling-7.2.0/fhdw/tests/test_pycaret.py
--rw-r--r--   0        0        0     3351 2024-03-07 15:23:05.959446 fhdw_modelling-7.2.0/fhdw/tests/test_tracking.py
--rw-r--r--   0        0        0     1196 2024-03-07 15:23:05.959446 fhdw_modelling-7.2.0/pyproject.toml
--rw-r--r--   0        0        0     4218 1970-01-01 00:00:00.000000 fhdw_modelling-7.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3234 2024-04-17 14:56:30.420921 fhdw_modelling-7.2.1/README.md
+-rw-r--r--   0        0        0       35 2024-04-17 14:56:30.420921 fhdw_modelling-7.2.1/fhdw/modelling/__init__.py
+-rw-r--r--   0        0        0     1496 2024-04-17 14:56:30.420921 fhdw_modelling-7.2.1/fhdw/modelling/base.py
+-rw-r--r--   0        0        0     7387 2024-04-17 14:56:30.420921 fhdw_modelling-7.2.1/fhdw/modelling/evaluation.py
+-rw-r--r--   0        0        0     3239 2024-04-17 14:56:30.420921 fhdw_modelling-7.2.1/fhdw/modelling/preprocessing.py
+-rw-r--r--   0        0        0    14394 2024-04-17 14:56:30.420921 fhdw_modelling-7.2.1/fhdw/modelling/pycaret.py
+-rw-r--r--   0        0        0     5160 2024-04-17 14:56:30.420921 fhdw_modelling-7.2.1/fhdw/modelling/tracking.py
+-rw-r--r--   0        0        0       22 2024-04-17 14:56:30.420921 fhdw_modelling-7.2.1/fhdw/tests/__init__.py
+-rw-r--r--   0        0        0      328 2024-04-17 14:56:30.420921 fhdw_modelling-7.2.1/fhdw/tests/conftest.py
+-rw-r--r--   0        0        0     6613 2024-04-17 14:56:30.420921 fhdw_modelling-7.2.1/fhdw/tests/data/automobile.csv
+-rw-r--r--   0        0        0     3246 2024-04-17 14:56:30.420921 fhdw_modelling-7.2.1/fhdw/tests/test_base.py
+-rw-r--r--   0        0        0     5356 2024-04-17 14:56:30.420921 fhdw_modelling-7.2.1/fhdw/tests/test_evaluation.py
+-rw-r--r--   0        0        0      854 2024-04-17 14:56:30.420921 fhdw_modelling-7.2.1/fhdw/tests/test_preprocessing.py
+-rw-r--r--   0        0        0     9950 2024-04-17 14:56:30.420921 fhdw_modelling-7.2.1/fhdw/tests/test_pycaret.py
+-rw-r--r--   0        0        0     3351 2024-04-17 14:56:30.424921 fhdw_modelling-7.2.1/fhdw/tests/test_tracking.py
+-rw-r--r--   0        0        0     1196 2024-04-17 14:56:30.424921 fhdw_modelling-7.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4218 1970-01-01 00:00:00.000000 fhdw_modelling-7.2.1/PKG-INFO
```

### Comparing `fhdw_modelling-7.2.0/README.md` & `fhdw_modelling-7.2.1/README.md`

 * *Files identical despite different names*

### Comparing `fhdw_modelling-7.2.0/fhdw/modelling/base.py` & `fhdw_modelling-7.2.1/fhdw/modelling/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,16 @@
 
     Args:
         target (``str``): The target variable for the experiment.
 
         prefix (``str``, optional): An optional prefix to be added to the experiment
             name.
 
-        sep (``str``, optional): An optional seperator, placed between prefix and name.
+        sep (``str``, optional): An optional seperator, placed between ``prefix`` and
+            ``target``.
 
     Returns:
         ``str``: A formatted experiment name in the pattern
         ``[{prefix}{sep}]{cleaned_target}``.
     """
     clean_target_name = clean_string(target)
     clean_prefix_name = clean_string(prefix)
```

### Comparing `fhdw_modelling-7.2.0/fhdw/modelling/evaluation.py` & `fhdw_modelling-7.2.1/fhdw/modelling/evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,44 +3,44 @@
 import warnings
 
 import pandas as pd
 import plotly.express as px
 from pandas import Series
 from sklearn.metrics import mean_absolute_error
 from sklearn.metrics import mean_absolute_percentage_error
-from sklearn.metrics import mean_squared_error
-from sklearn.metrics import mean_squared_log_error
 from sklearn.metrics import r2_score
+from sklearn.metrics import root_mean_squared_error
+from sklearn.metrics import root_mean_squared_log_error
 
 PASTEL_ORANGE = "#fa9f55"  # Pastel orange color
 PASTEL_BLUE = "#96ceff"  # Pastel blue color
 
 
 def get_regression_metrics(y_true: Series, y_pred: Series):
     """Get dictionary of common regression metrics.
 
     Args:
         y_true (``pandas.Series``): The actual values of the ground truth.
 
         y_pred (``pandas.Series``): The inference values made by the model.
     """
     try:
-        rmsle = mean_squared_log_error(y_true=y_true, y_pred=y_pred, squared=False)
+        rmsle = root_mean_squared_log_error(y_true=y_true, y_pred=y_pred)
     except ValueError:
         rmsle = None
 
         warnings.warn(
             "Mean Squared Logarithmic Error cannot be used when "
             "targets contain negative values. Therefore it is set to None here."
         )
 
     metrics = {
         "MAE": mean_absolute_error(y_true=y_true, y_pred=y_pred),
         "MAPE": mean_absolute_percentage_error(y_true=y_true, y_pred=y_pred),
-        "RMSE": mean_squared_error(y_true=y_true, y_pred=y_pred, squared=False),
+        "RMSE": root_mean_squared_error(y_true=y_true, y_pred=y_pred),
         "RMSLE": rmsle,
         "R2": r2_score(y_true=y_true, y_pred=y_pred),
     }
 
     return metrics
```

### Comparing `fhdw_modelling-7.2.0/fhdw/modelling/preprocessing.py` & `fhdw_modelling-7.2.1/fhdw/modelling/preprocessing.py`

 * *Files identical despite different names*

### Comparing `fhdw_modelling-7.2.0/fhdw/modelling/pycaret.py` & `fhdw_modelling-7.2.1/fhdw/modelling/pycaret.py`

 * *Files identical despite different names*

### Comparing `fhdw_modelling-7.2.0/fhdw/modelling/tracking.py` & `fhdw_modelling-7.2.1/fhdw/modelling/tracking.py`

 * *Files identical despite different names*

### Comparing `fhdw_modelling-7.2.0/fhdw/tests/data/automobile.csv` & `fhdw_modelling-7.2.1/fhdw/tests/data/automobile.csv`

 * *Files identical despite different names*

### Comparing `fhdw_modelling-7.2.0/fhdw/tests/test_base.py` & `fhdw_modelling-7.2.1/fhdw/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `fhdw_modelling-7.2.0/fhdw/tests/test_evaluation.py` & `fhdw_modelling-7.2.1/fhdw/tests/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `fhdw_modelling-7.2.0/fhdw/tests/test_preprocessing.py` & `fhdw_modelling-7.2.1/fhdw/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `fhdw_modelling-7.2.0/fhdw/tests/test_pycaret.py` & `fhdw_modelling-7.2.1/fhdw/tests/test_pycaret.py`

 * *Files identical despite different names*

### Comparing `fhdw_modelling-7.2.0/fhdw/tests/test_tracking.py` & `fhdw_modelling-7.2.1/fhdw/tests/test_tracking.py`

 * *Files identical despite different names*

### Comparing `fhdw_modelling-7.2.0/pyproject.toml` & `fhdw_modelling-7.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "fhdw-modelling"
-version = "7.2.0"
+version = "7.2.1"
 description = "A collection of modelling tools. Intended for generic usage in FHDW projects."
 authors = ["Pascal Niggemeier <pascal.niggemeier@fhdw.de>"]
 license = "MPL-2.0"
 readme = "README.md"
 repository = "https://github.com/fhdw-forschung/modelling-tools"
 packages = [{ include = "fhdw" }]
 documentation = "https://fhdw-forschung.github.io/modelling-tools/"
@@ -18,15 +18,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 
 fastapi = "^0.104.1"
 kaleido = "0.2.1"
 mlflow = "^2.10.2"
-pyarrow = "^14.0.1"
+pyarrow = "^15.0.2"
 pycaret = { version = "^3.3.0", extras = ["mlops", "models"] }
 pyyaml = "^6.0.1"
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.5"
 black = "^23.11.0"
 flake8 = "^6.1.0"
```

### Comparing `fhdw_modelling-7.2.0/PKG-INFO` & `fhdw_modelling-7.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: fhdw-modelling
-Version: 7.2.0
+Version: 7.2.1
 Summary: A collection of modelling tools. Intended for generic usage in FHDW projects.
 Home-page: https://github.com/fhdw-forschung/modelling-tools
 License: MPL-2.0
 Author: Pascal Niggemeier
 Author-email: pascal.niggemeier@fhdw.de
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastapi (>=0.104.1,<0.105.0)
 Requires-Dist: kaleido (==0.2.1)
 Requires-Dist: mlflow (>=2.10.2,<3.0.0)
-Requires-Dist: pyarrow (>=14.0.1,<15.0.0)
+Requires-Dist: pyarrow (>=15.0.2,<16.0.0)
 Requires-Dist: pycaret[mlops,models] (>=3.3.0,<4.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Project-URL: Bug Tracker, https://github.com/fhdw-forschung/modelling-tools/issues
 Project-URL: Documentation, https://fhdw-forschung.github.io/modelling-tools/
 Project-URL: Repository, https://github.com/fhdw-forschung/modelling-tools
 Description-Content-Type: text/markdown
```

