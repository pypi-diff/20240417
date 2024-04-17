# Comparing `tmp/expected_cost-0.0.5.tar.gz` & `tmp/expected_cost-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expected_cost-0.0.5.tar", last modified: Fri Sep  1 20:31:20 2023, max compression
+gzip compressed data, was "expected_cost-0.0.6.tar", last modified: Wed Apr 17 17:17:33 2024, max compression
```

## Comparing `expected_cost-0.0.5.tar` & `expected_cost-0.0.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 lferrer    (501) staff       (20)        0 2023-09-01 20:31:20.349599 expected_cost-0.0.5/
--rw-r--r--   0 lferrer    (501) staff       (20)     1071 2023-07-05 13:01:22.000000 expected_cost-0.0.5/LICENSE.md
--rw-r--r--   0 lferrer    (501) staff       (20)     4094 2023-09-01 20:31:20.349779 expected_cost-0.0.5/PKG-INFO
--rw-r--r--   0 lferrer    (501) staff       (20)     3597 2023-09-01 13:22:13.000000 expected_cost-0.0.5/README.md
-drwxr-xr-x   0 lferrer    (501) staff       (20)        0 2023-09-01 20:31:20.333854 expected_cost-0.0.5/expected_cost/
--rw-r--r--   0 lferrer    (501) staff       (20)        1 2023-06-22 14:36:03.000000 expected_cost-0.0.5/expected_cost/__init__.py
--rw-r--r--   0 lferrer    (501) staff       (20)     4279 2023-06-15 20:46:03.000000 expected_cost-0.0.5/expected_cost/calibration.py
--rw-r--r--   0 lferrer    (501) staff       (20)    11682 2023-08-31 18:57:55.000000 expected_cost-0.0.5/expected_cost/data.py
--rw-r--r--   0 lferrer    (501) staff       (20)    22199 2023-08-31 18:58:56.000000 expected_cost-0.0.5/expected_cost/ec.py
--rw-r--r--   0 lferrer    (501) staff       (20)     1846 2023-08-03 12:35:57.000000 expected_cost-0.0.5/expected_cost/psrcal_wrappers.py
--rw-r--r--   0 lferrer    (501) staff       (20)     7531 2023-08-31 18:52:18.000000 expected_cost-0.0.5/expected_cost/utils.py
-drwxr-xr-x   0 lferrer    (501) staff       (20)        0 2023-09-01 20:31:20.337465 expected_cost-0.0.5/expected_cost.egg-info/
--rw-r--r--   0 lferrer    (501) staff       (20)     4094 2023-09-01 20:31:20.000000 expected_cost-0.0.5/expected_cost.egg-info/PKG-INFO
--rw-r--r--   0 lferrer    (501) staff       (20)      696 2023-09-01 20:31:20.000000 expected_cost-0.0.5/expected_cost.egg-info/SOURCES.txt
--rw-r--r--   0 lferrer    (501) staff       (20)        1 2023-09-01 20:31:20.000000 expected_cost-0.0.5/expected_cost.egg-info/dependency_links.txt
--rw-r--r--   0 lferrer    (501) staff       (20)       65 2023-09-01 20:31:20.000000 expected_cost-0.0.5/expected_cost.egg-info/requires.txt
--rw-r--r--   0 lferrer    (501) staff       (20)       31 2023-09-01 20:31:20.000000 expected_cost-0.0.5/expected_cost.egg-info/top_level.txt
-drwxr-xr-x   0 lferrer    (501) staff       (20)        0 2023-09-01 20:31:20.337834 expected_cost-0.0.5/notebooks/
--rw-r--r--   0 lferrer    (501) staff       (20)        1 2023-06-22 14:55:57.000000 expected_cost-0.0.5/notebooks/__init__.py
-drwxr-xr-x   0 lferrer    (501) staff       (20)        0 2023-09-01 20:31:20.342514 expected_cost-0.0.5/psrcal/
--rw-r--r--   0 lferrer    (501) staff       (20)        0 2023-06-08 15:20:51.000000 expected_cost-0.0.5/psrcal/__init.__.py
--rw-r--r--   0 lferrer    (501) staff       (20)        0 2023-06-08 15:20:51.000000 expected_cost-0.0.5/psrcal/__init__.py
--rw-r--r--   0 lferrer    (501) staff       (20)     5536 2023-06-28 12:01:53.000000 expected_cost-0.0.5/psrcal/calibration.py
--rw-r--r--   0 lferrer    (501) staff       (20)     8974 2023-08-03 10:05:22.000000 expected_cost-0.0.5/psrcal/losses.py
-drwxr-xr-x   0 lferrer    (501) staff       (20)        0 2023-09-01 20:31:20.347842 expected_cost-0.0.5/psrcal/optim/
--rw-r--r--   0 lferrer    (501) staff       (20)        0 2023-06-08 15:20:51.000000 expected_cost-0.0.5/psrcal/optim/__init__.py
--rw-r--r--   0 lferrer    (501) staff       (20)      504 2023-06-08 15:20:51.000000 expected_cost-0.0.5/psrcal/optim/example.py
--rw-r--r--   0 lferrer    (501) staff       (20)     1768 2023-06-08 15:20:51.000000 expected_cost-0.0.5/psrcal/optim/fullbatch_optim.py
--rw-r--r--   0 lferrer    (501) staff       (20)     3514 2023-06-08 15:20:51.000000 expected_cost-0.0.5/psrcal/optim/vecmodule.py
--rw-r--r--   0 lferrer    (501) staff       (20)      567 2023-06-08 15:20:51.000000 expected_cost-0.0.5/psrcal/psr.py
--rw-r--r--   0 lferrer    (501) staff       (20)      706 2023-06-08 15:20:51.000000 expected_cost-0.0.5/psrcal/utils.py
--rw-r--r--   0 lferrer    (501) staff       (20)       84 2023-06-22 15:01:18.000000 expected_cost-0.0.5/pyproject.toml
--rw-r--r--   0 lferrer    (501) staff       (20)      701 2023-09-01 20:31:20.350705 expected_cost-0.0.5/setup.cfg
-drwxr-xr-x   0 lferrer    (501) staff       (20)        0 2023-09-01 20:31:20.348832 expected_cost-0.0.5/test/
--rw-r--r--   0 lferrer    (501) staff       (20)      850 2023-06-28 15:25:15.000000 expected_cost-0.0.5/test/test.py
--rw-r--r--   0 lferrer    (501) staff       (20)      782 2023-06-28 15:46:12.000000 expected_cost-0.0.5/test/test_psrcal.py
+drwxr-xr-x   0 lferrer    (501) staff       (20)        0 2024-04-17 17:17:33.981073 expected_cost-0.0.6/
+-rw-r--r--   0 lferrer    (501) staff       (20)     1071 2023-07-05 13:01:22.000000 expected_cost-0.0.6/LICENSE.md
+-rw-r--r--   0 lferrer    (501) staff       (20)     4219 2024-04-17 17:17:33.980926 expected_cost-0.0.6/PKG-INFO
+-rw-r--r--   0 lferrer    (501) staff       (20)     3597 2023-09-01 13:22:13.000000 expected_cost-0.0.6/README.md
+drwxr-xr-x   0 lferrer    (501) staff       (20)        0 2024-04-17 17:17:33.929694 expected_cost-0.0.6/expected_cost/
+-rw-r--r--   0 lferrer    (501) staff       (20)        1 2023-06-22 14:36:03.000000 expected_cost-0.0.6/expected_cost/__init__.py
+-rw-r--r--   0 lferrer    (501) staff       (20)     4279 2023-06-15 20:46:03.000000 expected_cost-0.0.6/expected_cost/calibration.py
+-rw-r--r--   0 lferrer    (501) staff       (20)    12630 2024-04-11 13:25:04.000000 expected_cost-0.0.6/expected_cost/data.py
+-rw-r--r--   0 lferrer    (501) staff       (20)    22346 2024-04-09 12:20:38.000000 expected_cost-0.0.6/expected_cost/ec.py
+-rw-r--r--   0 lferrer    (501) staff       (20)     2010 2024-04-04 18:52:07.000000 expected_cost-0.0.6/expected_cost/psrcal_wrappers.py
+-rw-r--r--   0 lferrer    (501) staff       (20)     7765 2024-02-07 22:04:31.000000 expected_cost-0.0.6/expected_cost/utils.py
+drwxr-xr-x   0 lferrer    (501) staff       (20)        0 2024-04-17 17:17:33.950116 expected_cost-0.0.6/expected_cost.egg-info/
+-rw-r--r--   0 lferrer    (501) staff       (20)     4219 2024-04-17 17:17:33.000000 expected_cost-0.0.6/expected_cost.egg-info/PKG-INFO
+-rw-r--r--   0 lferrer    (501) staff       (20)      696 2024-04-17 17:17:33.000000 expected_cost-0.0.6/expected_cost.egg-info/SOURCES.txt
+-rw-r--r--   0 lferrer    (501) staff       (20)        1 2024-04-17 17:17:33.000000 expected_cost-0.0.6/expected_cost.egg-info/dependency_links.txt
+-rw-r--r--   0 lferrer    (501) staff       (20)       65 2024-04-17 17:17:33.000000 expected_cost-0.0.6/expected_cost.egg-info/requires.txt
+-rw-r--r--   0 lferrer    (501) staff       (20)       31 2024-04-17 17:17:33.000000 expected_cost-0.0.6/expected_cost.egg-info/top_level.txt
+drwxr-xr-x   0 lferrer    (501) staff       (20)        0 2024-04-17 17:17:33.935395 expected_cost-0.0.6/notebooks/
+-rw-r--r--   0 lferrer    (501) staff       (20)        1 2023-06-22 14:55:57.000000 expected_cost-0.0.6/notebooks/__init__.py
+drwxr-xr-x   0 lferrer    (501) staff       (20)        0 2024-04-17 17:17:33.939408 expected_cost-0.0.6/psrcal/
+-rw-r--r--   0 lferrer    (501) staff       (20)        0 2023-06-08 15:20:51.000000 expected_cost-0.0.6/psrcal/__init.__.py
+-rw-r--r--   0 lferrer    (501) staff       (20)        0 2023-06-08 15:20:51.000000 expected_cost-0.0.6/psrcal/__init__.py
+-rw-r--r--   0 lferrer    (501) staff       (20)     5536 2023-06-28 12:01:53.000000 expected_cost-0.0.6/psrcal/calibration.py
+-rw-r--r--   0 lferrer    (501) staff       (20)     8974 2023-08-03 10:05:22.000000 expected_cost-0.0.6/psrcal/losses.py
+drwxr-xr-x   0 lferrer    (501) staff       (20)        0 2024-04-17 17:17:33.942073 expected_cost-0.0.6/psrcal/optim/
+-rw-r--r--   0 lferrer    (501) staff       (20)        0 2023-06-08 15:20:51.000000 expected_cost-0.0.6/psrcal/optim/__init__.py
+-rw-r--r--   0 lferrer    (501) staff       (20)      504 2023-06-08 15:20:51.000000 expected_cost-0.0.6/psrcal/optim/example.py
+-rw-r--r--   0 lferrer    (501) staff       (20)     1768 2023-06-08 15:20:51.000000 expected_cost-0.0.6/psrcal/optim/fullbatch_optim.py
+-rw-r--r--   0 lferrer    (501) staff       (20)     3514 2023-06-08 15:20:51.000000 expected_cost-0.0.6/psrcal/optim/vecmodule.py
+-rw-r--r--   0 lferrer    (501) staff       (20)      567 2023-06-08 15:20:51.000000 expected_cost-0.0.6/psrcal/psr.py
+-rw-r--r--   0 lferrer    (501) staff       (20)      706 2023-06-08 15:20:51.000000 expected_cost-0.0.6/psrcal/utils.py
+-rw-r--r--   0 lferrer    (501) staff       (20)       84 2023-06-22 15:01:18.000000 expected_cost-0.0.6/pyproject.toml
+-rw-r--r--   0 lferrer    (501) staff       (20)      701 2024-04-17 17:17:33.981728 expected_cost-0.0.6/setup.cfg
+drwxr-xr-x   0 lferrer    (501) staff       (20)        0 2024-04-17 17:17:33.949292 expected_cost-0.0.6/test/
+-rw-r--r--   0 lferrer    (501) staff       (20)      850 2023-06-28 15:25:15.000000 expected_cost-0.0.6/test/test.py
+-rw-r--r--   0 lferrer    (501) staff       (20)      782 2023-06-28 15:46:12.000000 expected_cost-0.0.6/test/test_psrcal.py
```

### Comparing `expected_cost-0.0.5/LICENSE.md` & `expected_cost-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `expected_cost-0.0.5/PKG-INFO` & `expected_cost-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: expected_cost
-Version: 0.0.5
+Version: 0.0.6
 Summary: Methods for computing the expected cost metric for evaluation of classification systems
 Home-page: https://github.com/luferrer/expected_cost
 Author: Luciana Ferrer
 Author-email: lferrer@dc.uba.ar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: matplotlib>=3.5.2
+Requires-Dist: numpy>=1.24.1
+Requires-Dist: scipy>=1.9.1
+Requires-Dist: scikit_learn>=1.2.2
 
 # Expected cost
 
 Methods for computing the expected cost (EC) on an evaluation dataset, as defined in statistical learning text books (e.g., Bishop's "Pattern recognition and machine learning", and Hastie's et al "The elements of statistical learning"). 
 Given a matrix of user-defined costs with elements $c_{y\ d}$, where $y$ is the true class of a sample and $d$ is the decision made by the system for that sample, 
 this metric is estimated as the average of the costs across all samples in the dataset. That is:
```

### Comparing `expected_cost-0.0.5/README.md` & `expected_cost-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `expected_cost-0.0.5/expected_cost/calibration.py` & `expected_cost-0.0.6/expected_cost/calibration.py`

 * *Files identical despite different names*

### Comparing `expected_cost-0.0.5/expected_cost/data.py` & `expected_cost-0.0.6/expected_cost/data.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,75 +1,44 @@
 """ Utilities for loading scores or creating simulated data.
 """
 
 import numpy as np
-from scipy.stats import norm, multivariate_normal
+from scipy.stats import multivariate_normal
 from scipy.special import logsumexp 
 from expected_cost import utils
 import os
 
 try:
     import torch
     from expected_cost.calibration import calibration_with_crossval, calibration_train_on_test
     from psrcal.calibration import HistogramBinningCal
     has_psr = True
 #    print("Found psr calibration library = %s"%has_psr)
 except:
     has_psr = False
 
 
-def get_llks_for_multi_classif_task(dataset, priors=None, N=100000, sim_params=None):
-    """ Load or create multi-class log (potentially scaled) likelihoods (llks).
+def get_llks_for_multi_classif_task(dataset, priors=None, N=100000, sim_params=None, logpost=False, 
+        seed=0, train_cal_on_test=False, one_vs_other=None):
+    """ Load or create multi-class scores.
     The method outputs both the raw (potentially miscalibrated) scores and 
-    calibrated scores.
-         
-    Two datasets are implemented here:
-    * cifar10: pre-generated scores for cifar10 data
+    calibrated scores. If logpost is False, output log-likelihoods. This is the default. 
+    If logpost is True, output log posteriors.
+
+    Two ways of getting data are implemented here:
     * gaussian_sim: simulated data with Gaussian distributions. In this case,
       the priors and N need to be set to determine the class priors and the 
       total number of samples required.
+    * <dataset>: pre-generated scores that will be loaded from data/<dataset>
       
-    The cifar10 example can be used as template to add a loader for your own set 
-    of scores. If your scores are posteriors instead of llks, you can either: 
-    * ignore this fact and have this method output the posteriors (in this case,  
-      remember to call the expected cost methods with score_type="log-posteriors")
-    * convert them to estimated llks by using logpost_to_log_scaled_lks where the 
-      priors can be estimated as those used in training.
-
     """
 
-    if 'cifar10' in dataset:
+    np.random.seed(seed=seed)
 
-        # Load pre-generated scores for cifar10 data
-        print("\n**** Loading in CIFAR10 data ****\n")
-        dir = os.path.dirname(__file__)+"/data/resnet-50_cifar10/"
-        print(dir)
-        preacts = np.load(dir+"predictions.npy")
-        targets = np.load(dir+"targets.npy")
-
-        # Compute log-softmax to get log posteriors. 
-        raw_logpost = preacts - logsumexp(preacts, axis=-1, keepdims=True)
-
-        if has_psr:
-            # Calibrate the scores with cross-validation using an affine transform
-            # trained with log-loss (cross-entropy)
-            print("Calibrating data")
-            cal_logpost = calibration_with_crossval(raw_logpost, targets)
-        else:
-            # If calibration code is not available, load a pre-generated file
-            cal_logpost = np.load(dir+"predictions_cal_10classes.npy")
-
-        # For this dataset, the posteriors coincide with the scaled likelihoods
-        # because the priors are uniform. If that was not the case, we would use
-        # utils.logpost_to_log_scaled_lks(logpost, priors), where the priors are 
-        # those used in training.
-        raw_llks = raw_logpost
-        cal_llks = cal_logpost
-
-    elif dataset == 'gaussian_sim':
+    if dataset == 'gaussian_sim':
 
         if sim_params is None:
             sim_params = {}
 
 
         feat_std    = sim_params.get('feat_std', 1.0)
         score_shift = sim_params.get('score_shift', 0)
@@ -77,15 +46,14 @@
         counts = np.array(np.array(priors)*N, dtype=int)
         K = len(counts)
 
         # Create data (features) using a Gaussian distribution for each class. 
         # Make the features unidimensional for simplicity, with same std and
         # evenly distributed means.
         #print("\n**** Creating simulated data with Gaussian class distributions for %d classes ****\n"%K)
-        np.random.seed(0)
 
         # Put the mean at 0, 1, ..., K-1. 
         means = np.arange(0, K)
 
         # Use the same diagonal covariance matrix for all classes.
         # The value of std will determine the difficulty of the problem.
         stds   = np.ones(K) * feat_std
@@ -98,19 +66,75 @@
         # These are well-calibrated by definition, since we know the generating
         # distribution.
         cal_llks = get_llks_for_gaussian_model(feats, means, stds)
 
         # Now generate misscalibrated llks with the provided shift and scale 
         raw_llks = score_scale * cal_llks + score_shift
 
+        if logpost:
+            raw_logpost = utils.llks_to_logpost(raw_llks, priors)
+            cal_logpost = utils.llks_to_logpost(cal_llks, priors)
+
     else:
-        raise Exception(f"Unrecognized dataset name: {dataset}")
+        # load logits from a directory
+        preacts = np.load(dataset+"/scores.npy")
+        targets = np.array(np.load(dataset+"/targets.npy"), dtype=int)
+
+        counts = np.bincount(targets)
+        data_priors = counts/len(targets)
+        if priors is not None:
+            # Resample the data to get the requested priors
+            new_counts = priors * len(targets)
+            ratio = new_counts / counts
+            new_counts /= np.max(ratio)
+            for c in np.sort(np.unique(targets)):
+                idx = targets==c
+                p = preacts[idx]
+                t = targets[idx]
+                keep_idx = np.random.choice(np.arange(len(t)), int(new_counts[c]), replace=False)
+                if c==0:
+                    new_targets = t[keep_idx]
+                    new_preacts = p[keep_idx]
+                else:
+                    new_targets = np.r_[new_targets, t[keep_idx]]
+                    new_preacts = np.r_[new_preacts, p[keep_idx]]
 
+            targets = new_targets
+            preacts = new_preacts            
 
-    return targets, raw_llks, cal_llks
+        # Compute log-softmax to get log posteriors. 
+        raw_logpost = preacts - logsumexp(preacts, axis=-1, keepdims=True)
+
+        if one_vs_other is not None:
+            # Map the multi-class problem into a new one vs other problem
+            raw_logpost_1 = raw_logpost[:,one_vs_other]
+            raw_logpost_0 = logsumexp(np.delete(raw_logpost, one_vs_other, axis=1), axis=1)
+
+            raw_logpost = np.c_[raw_logpost_0, raw_logpost_1]
+            targets = np.array(targets == one_vs_other, dtype=int)
+
+        if has_psr:
+            # Calibrate the scores with cross-validation using an affine transform
+            # trained with log-loss (cross-entropy)
+            if train_cal_on_test:
+                cal_logpost = calibration_train_on_test(raw_logpost, targets)
+            else:
+                cal_logpost = calibration_with_crossval(raw_logpost, targets, seed=seed)
+        else:
+            # If calibration code is not available, load a pre-generated file
+            cal_logpost = np.load(dir+"predictions_cal_10classes.npy")
+
+        if not logpost:
+            raw_llks = utils.logpost_to_log_scaled_lks(raw_logpost, priors)
+            cal_llks = utils.logpost_to_log_scaled_lks(cal_logpost, priors)
+
+    if logpost:
+        return targets, raw_logpost, cal_logpost
+    else:
+        return targets, raw_llks, cal_llks
 
 
 def print_score_stats(scores, targets):
 
     for c in np.unique(targets):
         scores_c = scores[targets==c]
         print("Class %d :  mean  %5.2f    std   %5.2f"%(c, np.mean(scores_c, axis=0), np.std(scores_c, axis=0)))
```

### Comparing `expected_cost-0.0.5/expected_cost/ec.py` & `expected_cost-0.0.6/expected_cost/ec.py`

 * *Files 1% similar despite different names*

```diff
@@ -489,15 +489,15 @@
 
     decisions, posteriors = bayes_decisions(scores, costs, priors, score_type, silent=silent)
     cost = average_cost(targets, decisions, costs, priors, sample_weight, adjusted)
 
     return cost, decisions
 
 def average_cost_for_optimal_decisions(targets, scores, costs=None, priors=None, sample_weight=None, 
-    adjusted=False, score_type='log_posteriors'):
+    adjusted=False, score_type='log_posteriors', return_threshold=False):
     """ Average cost for optimal decisions given the provided scores. 
     Only applicable to binary classification when the cost matrix has 
     the following form:
     
                              0  c01
                             c10  0
 
@@ -562,8 +562,11 @@
         # When adjusted is true, normalize the average cost
         # with the cost of a naive system that always makes
         # the min cost decision.
         norm_value = np.min(np.dot(priors.T, cmatrix))
     else:
         norm_value = 1.0
 
-    return np.min(ave_cost)/norm_value
+    if return_threshold:
+        return np.min(ave_cost)/norm_value, post1_with_target[np.argmin(ave_cost),0]
+    else:
+        return np.min(ave_cost)/norm_value
```

### Comparing `expected_cost-0.0.5/expected_cost/psrcal_wrappers.py` & `expected_cost-0.0.6/expected_cost/psrcal_wrappers.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,18 @@
 
 
 def LogLoss(log_probs, labels, norm=True, priors=None):
 
     return loss_from_psrcal(losses.LogLoss, log_probs, labels, norm, priors)
 
 
+def LogLossSE(log_probs, ref_log_probs, norm=True):
+
+    return losses.LogLossSE(torch.tensor(log_probs), torch.tensor(ref_log_probs), norm=norm).detach().numpy()
+
 def ECE(log_probs, labels, M=15, return_values=False):
 
     out = losses.ECE(torch.tensor(log_probs), torch.tensor(labels), M, return_values)
     return [v.detach().numpy() if torch.is_tensor(v) else v for v in out] if return_values else out.detach().numpy()
 
 
 def ECEbin(log_probs, labels, M=15, return_values=False):
```

### Comparing `expected_cost-0.0.5/expected_cost/utils.py` & `expected_cost-0.0.6/expected_cost/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,7 +241,14 @@
 
 def LRplus(N10, N01, N0, N1):
     R10 = N10 / N1
     R01 = N01 / N0
     return (1-R10)/R01 if R01>0 else np.inf
 
 
+def effective_priors(costs, priors):
+    """ Compute the effective priors: the equivalent priors that would lead to the same cost function
+    if the costs are were all set to 1 
+    """
+
+    return costs*priors/np.sum(costs*priors)
+
```

### Comparing `expected_cost-0.0.5/expected_cost.egg-info/PKG-INFO` & `expected_cost-0.0.6/expected_cost.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
-Name: expected-cost
-Version: 0.0.5
+Name: expected_cost
+Version: 0.0.6
 Summary: Methods for computing the expected cost metric for evaluation of classification systems
 Home-page: https://github.com/luferrer/expected_cost
 Author: Luciana Ferrer
 Author-email: lferrer@dc.uba.ar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: matplotlib>=3.5.2
+Requires-Dist: numpy>=1.24.1
+Requires-Dist: scipy>=1.9.1
+Requires-Dist: scikit_learn>=1.2.2
 
 # Expected cost
 
 Methods for computing the expected cost (EC) on an evaluation dataset, as defined in statistical learning text books (e.g., Bishop's "Pattern recognition and machine learning", and Hastie's et al "The elements of statistical learning"). 
 Given a matrix of user-defined costs with elements $c_{y\ d}$, where $y$ is the true class of a sample and $d$ is the decision made by the system for that sample, 
 this metric is estimated as the average of the costs across all samples in the dataset. That is:
```

### Comparing `expected_cost-0.0.5/expected_cost.egg-info/SOURCES.txt` & `expected_cost-0.0.6/expected_cost.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `expected_cost-0.0.5/psrcal/calibration.py` & `expected_cost-0.0.6/psrcal/calibration.py`

 * *Files identical despite different names*

### Comparing `expected_cost-0.0.5/psrcal/losses.py` & `expected_cost-0.0.6/psrcal/losses.py`

 * *Files identical despite different names*

### Comparing `expected_cost-0.0.5/psrcal/optim/fullbatch_optim.py` & `expected_cost-0.0.6/psrcal/optim/fullbatch_optim.py`

 * *Files identical despite different names*

### Comparing `expected_cost-0.0.5/psrcal/optim/vecmodule.py` & `expected_cost-0.0.6/psrcal/optim/vecmodule.py`

 * *Files identical despite different names*

### Comparing `expected_cost-0.0.5/psrcal/psr.py` & `expected_cost-0.0.6/psrcal/psr.py`

 * *Files identical despite different names*

### Comparing `expected_cost-0.0.5/psrcal/utils.py` & `expected_cost-0.0.6/psrcal/utils.py`

 * *Files identical despite different names*

### Comparing `expected_cost-0.0.5/setup.cfg` & `expected_cost-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = expected_cost
-version = 0.0.5
+version = 0.0.6
 author = Luciana Ferrer
 author_email = lferrer@dc.uba.ar
 description = Methods for computing the expected cost metric for evaluation of classification systems
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/luferrer/expected_cost
 classifiers =
```

### Comparing `expected_cost-0.0.5/test/test.py` & `expected_cost-0.0.6/test/test.py`

 * *Files identical despite different names*

### Comparing `expected_cost-0.0.5/test/test_psrcal.py` & `expected_cost-0.0.6/test/test_psrcal.py`

 * *Files identical despite different names*

