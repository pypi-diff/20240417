# Comparing `tmp/clfutils4r-1.0.0.tar.gz` & `tmp/clfutils4r-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clfutils4r-1.0.0.tar", last modified: Sat Apr 13 05:59:46 2024, max compression
+gzip compressed data, was "clfutils4r-1.0.1.tar", last modified: Wed Apr 17 12:04:42 2024, max compression
```

## Comparing `clfutils4r-1.0.0.tar` & `clfutils4r-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-04-13 05:59:46.767143 clfutils4r-1.0.0/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    35128 2022-07-24 06:54:15.000000 clfutils4r-1.0.0/LICENSE
--rw-r--r--   0 rgura001 (52843) rgura001 (52843)     6798 2024-04-13 05:59:46.767143 clfutils4r-1.0.0/PKG-INFO
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     6154 2024-04-13 05:58:30.000000 clfutils4r-1.0.0/README.md
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      673 2024-04-13 05:59:39.000000 clfutils4r-1.0.0/pyproject.toml
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       38 2024-04-13 05:59:46.767143 clfutils4r-1.0.0/setup.cfg
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     1001 2023-07-24 04:54:18.000000 clfutils4r-1.0.0/setup.py
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-04-13 05:59:46.767143 clfutils4r-1.0.0/src/
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-04-13 05:59:46.767143 clfutils4r-1.0.0/src/clfutils4r/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        0 2022-07-24 06:54:15.000000 clfutils4r-1.0.0/src/clfutils4r/__init__.py
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    27602 2024-04-13 05:53:50.000000 clfutils4r-1.0.0/src/clfutils4r/eval_classification.py
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    13221 2024-04-13 03:17:53.000000 clfutils4r-1.0.0/src/clfutils4r/gridsearch_classification.py
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    10883 2024-04-13 04:18:23.000000 clfutils4r-1.0.0/src/clfutils4r/pretty_cm.py
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-04-13 05:59:46.767143 clfutils4r-1.0.0/src/clfutils4r.egg-info/
--rw-r--r--   0 rgura001 (52843) rgura001 (52843)     6798 2024-04-13 05:59:46.000000 clfutils4r-1.0.0/src/clfutils4r.egg-info/PKG-INFO
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      330 2024-04-13 05:59:46.000000 clfutils4r-1.0.0/src/clfutils4r.egg-info/SOURCES.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        1 2024-04-13 05:59:46.000000 clfutils4r-1.0.0/src/clfutils4r.egg-info/dependency_links.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       11 2024-04-13 05:59:46.000000 clfutils4r-1.0.0/src/clfutils4r.egg-info/top_level.txt
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-04-17 12:04:42.882320 clfutils4r-1.0.1/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    35128 2022-07-24 06:54:15.000000 clfutils4r-1.0.1/LICENSE
+-rw-r--r--   0 rgura001 (52843) rgura001 (52843)     7046 2024-04-17 12:04:42.882320 clfutils4r-1.0.1/PKG-INFO
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     6402 2024-04-13 06:08:41.000000 clfutils4r-1.0.1/README.md
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      673 2024-04-17 12:04:23.000000 clfutils4r-1.0.1/pyproject.toml
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       38 2024-04-17 12:04:42.882320 clfutils4r-1.0.1/setup.cfg
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     1001 2023-07-24 04:54:18.000000 clfutils4r-1.0.1/setup.py
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-04-17 12:04:42.882320 clfutils4r-1.0.1/src/
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-04-17 12:04:42.882320 clfutils4r-1.0.1/src/clfutils4r/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        0 2022-07-24 06:54:15.000000 clfutils4r-1.0.1/src/clfutils4r/__init__.py
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    27610 2024-04-17 11:25:32.000000 clfutils4r-1.0.1/src/clfutils4r/eval_classification.py
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    14173 2024-04-17 11:48:43.000000 clfutils4r-1.0.1/src/clfutils4r/gridsearch_classification.py
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    10883 2024-04-13 04:18:23.000000 clfutils4r-1.0.1/src/clfutils4r/pretty_cm.py
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-04-17 12:04:42.882320 clfutils4r-1.0.1/src/clfutils4r.egg-info/
+-rw-r--r--   0 rgura001 (52843) rgura001 (52843)     7046 2024-04-17 12:04:42.000000 clfutils4r-1.0.1/src/clfutils4r.egg-info/PKG-INFO
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      330 2024-04-17 12:04:42.000000 clfutils4r-1.0.1/src/clfutils4r.egg-info/SOURCES.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        1 2024-04-17 12:04:42.000000 clfutils4r-1.0.1/src/clfutils4r.egg-info/dependency_links.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       11 2024-04-17 12:04:42.000000 clfutils4r-1.0.1/src/clfutils4r.egg-info/top_level.txt
```

### Comparing `clfutils4r-1.0.0/LICENSE` & `clfutils4r-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clfutils4r-1.0.0/PKG-INFO` & `clfutils4r-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clfutils4r
-Version: 1.0.0
+Version: 1.0.1
 Summary: Wrapper around some basic sklearn and scikit-plot utilities for classification.
 Home-page: https://github.com/rutujagurav/clfutils4r
 Author: Rutuja Gurav
 Author-email: Rutuja Gurav <rutujagurav100@gmail.com>
 Project-URL: Homepage, https://github.com/rutujagurav/clfutils4r
 Project-URL: Bug Tracker, https://github.com/rutujagurav/clfutils4r/issues
 Classifier: Programming Language :: Python :: 3
@@ -137,15 +137,15 @@
 y_pred_proba = best_model.predict_proba(X_test)
 
 ## Evaluate best model on test set
 from eval_classification import eval_classification
 ## Make metrics plots
 eval_classification(make_metrics_plots=True, y_test=y_test, y_pred=y_pred, y_pred_proba=y_pred_proba,  
                     class_names=class_names, feature_names=feature_names,
-                    titlestr="Breast Cancer Detection",
+                    titlestr="Breast Cancer Classification",
                     show=True, save=True, 
                     RESULTS_DIR=os.getcwd()+'/test_results')
 
 ```
 <!-- ### Grid Search -->
 ![grid_search](tests/example_classification/gridsearch_results/models/RandomForestClassifier/parcoord_plot.png)
 
@@ -176,7 +176,12 @@
 <!-- ### Shapley Analysis Summary Plot -->
 ![shap](tests/example_classification/test_results/shap_summary_plot.png)
 <!-- ![shap](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/shap_summary_plot.png) -->
 
 
 ## Developer Notes:
 This package is the updated version of `bcutils4r` which supported only binary classification. `bcutils4r` is now defunct.
+
+## Credits:
+1. For pretty confusion matrix - https://github.com/phongsathorn1/pretty-confusion-matrix
+2. Scikit Plot package  - https://scikit-plot.readthedocs.io/en/stable
+3. Shapley Analysis - https://shap-lrjball.readthedocs.io/en/latest/
```

### Comparing `clfutils4r-1.0.0/README.md` & `clfutils4r-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 y_pred_proba = best_model.predict_proba(X_test)
 
 ## Evaluate best model on test set
 from eval_classification import eval_classification
 ## Make metrics plots
 eval_classification(make_metrics_plots=True, y_test=y_test, y_pred=y_pred, y_pred_proba=y_pred_proba,  
                     class_names=class_names, feature_names=feature_names,
-                    titlestr="Breast Cancer Detection",
+                    titlestr="Breast Cancer Classification",
                     show=True, save=True, 
                     RESULTS_DIR=os.getcwd()+'/test_results')
 
 ```
 <!-- ### Grid Search -->
 ![grid_search](tests/example_classification/gridsearch_results/models/RandomForestClassifier/parcoord_plot.png)
 
@@ -159,8 +159,13 @@
 
 <!-- ### Shapley Analysis Summary Plot -->
 ![shap](tests/example_classification/test_results/shap_summary_plot.png)
 <!-- ![shap](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/shap_summary_plot.png) -->
 
 
 ## Developer Notes:
-This package is the updated version of `bcutils4r` which supported only binary classification. `bcutils4r` is now defunct.
+This package is the updated version of `bcutils4r` which supported only binary classification. `bcutils4r` is now defunct.
+
+## Credits:
+1. For pretty confusion matrix - https://github.com/phongsathorn1/pretty-confusion-matrix
+2. Scikit Plot package  - https://scikit-plot.readthedocs.io/en/stable
+3. Shapley Analysis - https://shap-lrjball.readthedocs.io/en/latest/
```

### Comparing `clfutils4r-1.0.0/pyproject.toml` & `clfutils4r-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clfutils4r"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Rutuja Gurav", email="rutujagurav100@gmail.com" },
 ]
 description = "Wrapper around some basic sklearn and scikit-plot utilities for classification."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers=[
```

### Comparing `clfutils4r-1.0.0/setup.py` & `clfutils4r-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `clfutils4r-1.0.0/src/clfutils4r/eval_classification.py` & `clfutils4r-1.0.1/src/clfutils4r/eval_classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -428,16 +428,17 @@
     if show:
         plt.show()
     plt.close()
 
 def plot_shap_summary(model=None, nsamples=50, X_train=None, X_test=None, feature_names=None, titlestr='', show=False, save=False, RESULTS_DIR=None, dpi=300):
     print("No. of samples used to build explainer and generate shap values: ", nsamples)
     explainer = shap.KernelExplainer(model.predict, shap.sample(X_train, nsamples))
-    shap_values = explainer.shap_values(X=X_test, nsamples=nsamples)
-    shap.summary_plot(shap_values=shap_values, features=X_test, feature_names=feature_names, show=False)
+    X_test_sample = shap.sample(X_test, nsamples)
+    shap_values = explainer.shap_values(X=X_test_sample)
+    shap.summary_plot(shap_values=shap_values, features=X_test_sample, feature_names=feature_names, show=False)
     # shap.plots.violin(shap_values=shap_values, features=X_test, plot_type="layered_violin", show=False)
     plt.title(titlestr+'Shapley Analysis')
     plt.tight_layout()
     
     if save:
         plt.savefig(RESULTS_DIR+'/shap_summary_plot.png', bbox_inches='tight',dpi=dpi)   
     if show:
@@ -495,16 +496,15 @@
     else:
         # titlestr_cls = "("+classes_titlestr+")\n\n"
         # titlestr_nocls = titlestr
         titlestr_cls = titlestr_nocls = ""
 
     if save:
         if RESULTS_DIR is not None:
-            if not os.path.exists(RESULTS_DIR):
-                os.makedirs(RESULTS_DIR)
+            os.makedirs(RESULTS_DIR, exist_ok=True)
             print("Saving results in {}".format(RESULTS_DIR))   
         else:
             print("Hey! You asked me to save results but did not provide a RESULTS_DIR !!!")
 
     if make_metrics_plots:
         if y_test is not None and y_pred is not None:
             assert len(y_test) == len(y_pred), "[Length Mismatch]: Number of test samples not equal to number of predictions"
```

### Comparing `clfutils4r-1.0.0/src/clfutils4r/gridsearch_classification.py` & `clfutils4r-1.0.1/src/clfutils4r/gridsearch_classification.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,29 +13,31 @@
 
 from sklearn.manifold import Isomap, SpectralEmbedding
 from sklearn.manifold import TSNE
 # from openTSNE import TSNE
 from sklearn.decomposition import PCA
 
 from sklearn.datasets import make_classification, load_iris, load_digits
-from sklearn.model_selection import GridSearchCV
 from sklearn.preprocessing import LabelEncoder
 
 ## Classification models
 from sklearn.ensemble import RandomForestClassifier, ExtraTreesClassifier
 from sklearn.gaussian_process import GaussianProcessClassifier
 from sklearn.linear_model import LogisticRegression, RidgeClassifier
 from sklearn.naive_bayes import GaussianNB
 from sklearn.neighbors import KNeighborsClassifier
 from sklearn.svm import LinearSVC
 from sklearn.tree import DecisionTreeClassifier, ExtraTreeClassifier
 
 from sklearn.metrics import confusion_matrix, classification_report, roc_curve, precision_recall_curve
 from sklearn.metrics import accuracy_score, precision_score, recall_score, f1_score, roc_auc_score, dcg_score, ndcg_score, cohen_kappa_score
 
+from sklearn.model_selection import GridSearchCV, RandomizedSearchCV
+from skopt import BayesSearchCV
+
 import matplotlib.pyplot as plt
 import matplotlib.cm as cm
 import plotly.graph_objects as go
 import numpy as np
 import pandas as pd
 import collections, os, sys, random, functools, pdb, joblib, json, inspect
 from pprint import pprint
@@ -44,15 +46,16 @@
 
 def plot_grid_search_metrics(hparam_search_results, metric="F1", show=False, save=False, save_dir=None):
     hparams = [col for col in hparam_search_results.columns if col.startswith("param_")]
     metrics = [col for col in hparam_search_results.columns if col.startswith("mean_test_")]
 
     dimslist4parcoordplot = []
     for hparam_name in hparams:
-        if hparam_search_results[hparam_name].dtype in ["object", "categorical"]: 
+        # print(hparam_name, hparam_search_results[hparam_name].dtype)
+        if hparam_search_results[hparam_name].dtype in ["object", "categorical", "bool"]: 
             le = LabelEncoder()
             encoded_hparam = le.fit_transform(hparam_search_results[hparam_name])
             dimslist4parcoordplot.append(
                 dict(   
                         ticktext=le.classes_, tickvals=le.transform(le.classes_),
                         label=hparam_name.split("param_")[-1], 
                         values=encoded_hparam
@@ -65,58 +68,60 @@
                         values=hparam_search_results[hparam_name].values
                     )
             )
     for metric_name in metrics:
         dimslist4parcoordplot.append(
             dict(
                     label=metric_name.split("mean_test_")[-1], 
-                    values=hparam_search_results[metric_name].values
+                    values=hparam_search_results[metric_name].values,
+                    range=[0,1]
                 )
         )
 
     fig = go.Figure(data=
         go.Parcoords(
             line = dict(color = hparam_search_results[f'mean_test_{metric}'],
                     colorscale = 'Viridis',
                     showscale = True,
                 ),
             dimensions = dimslist4parcoordplot
         )
     )
-    # fig.update_layout(width=1500, height=500)
+    fig.update_layout(width=1500, height=500)
     if save:
         fig.write_html(save_dir+"/parcoord_plot.html")
         fig.write_image(save_dir+"/parcoord_plot.png")
     if show:
         fig.show()
 
 def classify_feats(X=None, gt_labels=[],
                     classification_algorithms=["LogisticRegression",
                                                 "GaussianNB", "KNeighborsClassifier",
-                                                "DecisionTreeClassifier", "ExtraTreeClassifier", 
                                                 "RandomForestClassifier", "ExtraTreesClassifier",
+                                                "DecisionTreeClassifier", "ExtraTreeClassifier", 
                                             ], 
+                    search_space = [], # TODO: If provided, will override the classification_algorithms
                     num_runs=5, best_model_metric="F1",
                     show=False, save=False, save_dir=None
                 ):
     num_classes = len(np.unique(gt_labels))
     print(f"No. of classes: {num_classes}")
     print(f"Class counts: {collections.Counter(gt_labels)}")
 
     def scorer(estimator, X, y_true):
         estimator.fit(X, y_true)
         y_pred = estimator.predict(X)
         y_pred_proba = estimator.predict_proba(X)
         if num_classes == 2:
             return {
-                    "Accuracy": accuracy_score(y_true, y_pred > 0.5),
-                    "Precision": precision_score(y_true, y_pred > 0.5),
-                    "Recall": recall_score(y_true, y_pred > 0.5),
-                    "F1": f1_score(y_true, y_pred > 0.5),
-                    "AUROC": roc_auc_score(y_true, y_pred),
+                    "Accuracy": accuracy_score(y_true, y_pred),
+                    "Precision": precision_score(y_true, y_pred, average='binary'),
+                    "Recall": recall_score(y_true, y_pred, average='binary'),
+                    "F1": f1_score(y_true, y_pred, average='binary'),
+                    "AUROC": roc_auc_score(y_true, y_pred_proba[:,1]),
                     # "Discounted_Cumulative_Gain": dcg_score(y_true, y_pred),
                     # "Normalized_Discounted_Cumulative_Gain": ndcg_score(y_true, y_pred),
                     # "Cohen_Kappa": cohen_kappa_score(y_true, y_pred)
                 }
         elif num_classes > 2:
             return {
                     "Accuracy": accuracy_score(y_true, y_pred),
@@ -149,32 +154,32 @@
     if "ExtraTreeClassifier" in classification_algorithms:
         search_space.append([ExtraTreeClassifier(), {
                                                         "criterion": ['gini', 'entropy', 'log_loss'],
                                                         "splitter": ['best', 'random']
 
                                                     }])
     if "GaussianNB" in classification_algorithms:
-        search_space.append([GaussianNB(), {}])
+        search_space.append([GaussianNB(), {"var_smoothing": [1e-9, 1e-5, 1e-3]}])
 
     if "KNeighborsClassifier" in classification_algorithms:
         search_space.append([KNeighborsClassifier(), {
                                                         "n_neighbors": [1, 5, 10],
                                                         "weights": ['uniform', 'distance'],
                                                         "algorithm": ['auto', 'ball_tree', 'kd_tree', 'brute'],
                                                         "p": [1,2]
                                                     }])
     if "RandomForestClassifier" in classification_algorithms:
         search_space.append([RandomForestClassifier(), {
-                                                        "n_estimators": [10, 50, 100, 200],
+                                                        "n_estimators": [10, 50, 100, 200, 500],
                                                         "criterion": ['gini', 'entropy', 'log_loss'],
                                                         "bootstrap": [True, False]
                                                     }])
     if "ExtraTreesClassifier" in classification_algorithms:
         search_space.append([ExtraTreesClassifier(), {
-                                                        "n_estimators": [10, 50, 100, 200],
+                                                        "n_estimators": [10, 50, 100, 200, 500],
                                                         "criterion": ['gini', 'entropy', 'log_loss'],
                                                         "bootstrap": [True, False]
                                                     }])
     if "GaussianProcessClassifier" in classification_algorithms:
         search_space.append([GaussianProcessClassifier(), {}])
     if "LinearSVC" in classification_algorithms:
         search_space.append([LinearSVC(), {
@@ -199,21 +204,32 @@
 
         if save:
             save_dir_ = os.path.join(save_dir, "models", estimator_name)
             if not os.path.exists(save_dir_): os.makedirs(save_dir_)
         else:
             save_dir_ = None
 
-        classifier_hpopt = GridSearchCV(estimator=estimator,
-                                        param_grid=param_grid,
-                                        scoring=scorer,
-                                        refit=best_model_metric,
-                                        cv=num_runs, n_jobs=-1,
-                                        verbose=0,
-                                    )
+        # print(f"Using GridSearchCV for {estimator_name}...")
+        # classifier_hpopt = GridSearchCV(estimator=estimator,
+        #                                 param_grid=param_grid,
+        #                                 scoring=scorer,
+        #                                 refit=best_model_metric,
+        #                                 cv=num_runs, n_jobs=-1,
+        #                                 verbose=0,
+        #                             )
+        
+        print(f"Using RandomizedSearchCV for {estimator_name}...")
+        classifier_hpopt = RandomizedSearchCV(estimator=estimator,
+                                            param_distributions=param_grid,
+                                            scoring=scorer,
+                                            refit=best_model_metric,
+                                            cv=num_runs, n_jobs=-1,
+                                            verbose=0,
+                                        )
+        
         classifier_hpopt.fit(X, gt_labels)
 
         best_model = classifier_hpopt.best_estimator_
 
         # Check if current score is better than best score and update if true
         if classifier_hpopt.best_score_ > best_score_overall:
             best_score_overall = classifier_hpopt.best_score_
```

### Comparing `clfutils4r-1.0.0/src/clfutils4r/pretty_cm.py` & `clfutils4r-1.0.1/src/clfutils4r/pretty_cm.py`

 * *Files identical despite different names*

### Comparing `clfutils4r-1.0.0/src/clfutils4r.egg-info/PKG-INFO` & `clfutils4r-1.0.1/src/clfutils4r.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clfutils4r
-Version: 1.0.0
+Version: 1.0.1
 Summary: Wrapper around some basic sklearn and scikit-plot utilities for classification.
 Home-page: https://github.com/rutujagurav/clfutils4r
 Author: Rutuja Gurav
 Author-email: Rutuja Gurav <rutujagurav100@gmail.com>
 Project-URL: Homepage, https://github.com/rutujagurav/clfutils4r
 Project-URL: Bug Tracker, https://github.com/rutujagurav/clfutils4r/issues
 Classifier: Programming Language :: Python :: 3
@@ -137,15 +137,15 @@
 y_pred_proba = best_model.predict_proba(X_test)
 
 ## Evaluate best model on test set
 from eval_classification import eval_classification
 ## Make metrics plots
 eval_classification(make_metrics_plots=True, y_test=y_test, y_pred=y_pred, y_pred_proba=y_pred_proba,  
                     class_names=class_names, feature_names=feature_names,
-                    titlestr="Breast Cancer Detection",
+                    titlestr="Breast Cancer Classification",
                     show=True, save=True, 
                     RESULTS_DIR=os.getcwd()+'/test_results')
 
 ```
 <!-- ### Grid Search -->
 ![grid_search](tests/example_classification/gridsearch_results/models/RandomForestClassifier/parcoord_plot.png)
 
@@ -176,7 +176,12 @@
 <!-- ### Shapley Analysis Summary Plot -->
 ![shap](tests/example_classification/test_results/shap_summary_plot.png)
 <!-- ![shap](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/shap_summary_plot.png) -->
 
 
 ## Developer Notes:
 This package is the updated version of `bcutils4r` which supported only binary classification. `bcutils4r` is now defunct.
+
+## Credits:
+1. For pretty confusion matrix - https://github.com/phongsathorn1/pretty-confusion-matrix
+2. Scikit Plot package  - https://scikit-plot.readthedocs.io/en/stable
+3. Shapley Analysis - https://shap-lrjball.readthedocs.io/en/latest/
```

