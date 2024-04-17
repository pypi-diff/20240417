# Comparing `tmp/decodanda-0.6.8.tar.gz` & `tmp/decodanda-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decodanda-0.6.8.tar", last modified: Thu Dec 21 20:00:39 2023, max compression
+gzip compressed data, was "decodanda-0.6.9.tar", last modified: Thu Jan  4 19:37:10 2024, max compression
```

## Comparing `decodanda-0.6.8.tar` & `decodanda-0.6.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-12-21 20:00:39.474849 decodanda-0.6.8/
--rw-r--r--   0 lorenzo    (501) staff       (20)    35149 2023-02-15 23:52:18.000000 decodanda-0.6.8/LICENSE.md
--rw-r--r--   0 lorenzo    (501) staff       (20)     1202 2023-12-21 20:00:39.474655 decodanda-0.6.8/PKG-INFO
--rw-r--r--   0 lorenzo    (501) staff       (20)    36482 2023-04-19 18:21:22.000000 decodanda-0.6.8/README.md
-drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-12-21 20:00:39.473089 decodanda-0.6.8/decodanda/
--rw-r--r--   0 lorenzo    (501) staff       (20)      251 2023-02-17 22:21:32.000000 decodanda-0.6.8/decodanda/__init__.py
--rw-r--r--   0 lorenzo    (501) staff       (20)   115099 2023-12-21 20:00:02.000000 decodanda-0.6.8/decodanda/classes.py
--rw-r--r--   0 lorenzo    (501) staff       (20)     1194 2023-02-15 00:18:50.000000 decodanda-0.6.8/decodanda/imports.py
--rw-r--r--   0 lorenzo    (501) staff       (20)    11400 2023-07-20 21:34:26.000000 decodanda-0.6.8/decodanda/in_time.py
--rw-r--r--   0 lorenzo    (501) staff       (20)    40617 2023-06-08 16:31:08.000000 decodanda-0.6.8/decodanda/utilities.py
--rw-r--r--   0 lorenzo    (501) staff       (20)    24407 2023-07-21 17:56:09.000000 decodanda-0.6.8/decodanda/visualize.py
-drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2023-12-21 20:00:39.474419 decodanda-0.6.8/decodanda.egg-info/
--rw-r--r--   0 lorenzo    (501) staff       (20)     1202 2023-12-21 20:00:39.000000 decodanda-0.6.8/decodanda.egg-info/PKG-INFO
--rw-r--r--   0 lorenzo    (501) staff       (20)      324 2023-12-21 20:00:39.000000 decodanda-0.6.8/decodanda.egg-info/SOURCES.txt
--rw-r--r--   0 lorenzo    (501) staff       (20)        1 2023-12-21 20:00:39.000000 decodanda-0.6.8/decodanda.egg-info/dependency_links.txt
--rw-r--r--   0 lorenzo    (501) staff       (20)      109 2023-12-21 20:00:39.000000 decodanda-0.6.8/decodanda.egg-info/requires.txt
--rw-r--r--   0 lorenzo    (501) staff       (20)       10 2023-12-21 20:00:39.000000 decodanda-0.6.8/decodanda.egg-info/top_level.txt
--rw-r--r--   0 lorenzo    (501) staff       (20)       38 2023-12-21 20:00:39.474887 decodanda-0.6.8/setup.cfg
--rw-r--r--   0 lorenzo    (501) staff       (20)     1385 2023-12-21 20:00:15.000000 decodanda-0.6.8/setup.py
+drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2024-01-04 19:37:10.649910 decodanda-0.6.9/
+-rw-r--r--   0 lorenzo    (501) staff       (20)    35149 2023-02-15 23:52:18.000000 decodanda-0.6.9/LICENSE.md
+-rw-r--r--   0 lorenzo    (501) staff       (20)     1202 2024-01-04 19:37:10.649724 decodanda-0.6.9/PKG-INFO
+-rw-r--r--   0 lorenzo    (501) staff       (20)    36482 2023-04-19 18:21:22.000000 decodanda-0.6.9/README.md
+drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2024-01-04 19:37:10.648086 decodanda-0.6.9/decodanda/
+-rw-r--r--   0 lorenzo    (501) staff       (20)      251 2023-02-17 22:21:32.000000 decodanda-0.6.9/decodanda/__init__.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)   116345 2024-01-04 19:35:16.000000 decodanda-0.6.9/decodanda/classes.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)     1194 2023-02-15 00:18:50.000000 decodanda-0.6.9/decodanda/imports.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)    11400 2023-07-20 21:34:26.000000 decodanda-0.6.9/decodanda/in_time.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)    40617 2023-06-08 16:31:08.000000 decodanda-0.6.9/decodanda/utilities.py
+-rw-r--r--   0 lorenzo    (501) staff       (20)    24407 2023-07-21 17:56:09.000000 decodanda-0.6.9/decodanda/visualize.py
+drwxr-xr-x   0 lorenzo    (501) staff       (20)        0 2024-01-04 19:37:10.649505 decodanda-0.6.9/decodanda.egg-info/
+-rw-r--r--   0 lorenzo    (501) staff       (20)     1202 2024-01-04 19:37:10.000000 decodanda-0.6.9/decodanda.egg-info/PKG-INFO
+-rw-r--r--   0 lorenzo    (501) staff       (20)      324 2024-01-04 19:37:10.000000 decodanda-0.6.9/decodanda.egg-info/SOURCES.txt
+-rw-r--r--   0 lorenzo    (501) staff       (20)        1 2024-01-04 19:37:10.000000 decodanda-0.6.9/decodanda.egg-info/dependency_links.txt
+-rw-r--r--   0 lorenzo    (501) staff       (20)      109 2024-01-04 19:37:10.000000 decodanda-0.6.9/decodanda.egg-info/requires.txt
+-rw-r--r--   0 lorenzo    (501) staff       (20)       10 2024-01-04 19:37:10.000000 decodanda-0.6.9/decodanda.egg-info/top_level.txt
+-rw-r--r--   0 lorenzo    (501) staff       (20)       38 2024-01-04 19:37:10.649957 decodanda-0.6.9/setup.cfg
+-rw-r--r--   0 lorenzo    (501) staff       (20)     1385 2024-01-04 19:36:08.000000 decodanda-0.6.9/setup.py
```

### Comparing `decodanda-0.6.8/LICENSE.md` & `decodanda-0.6.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.8/PKG-INFO` & `decodanda-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decodanda
-Version: 0.6.8
+Version: 0.6.9
 Summary: Geometric decoding of neural data with built-in best practices.
 Home-page: https://github.com/lposani/decodanda
 Author: Lorenzo Posani
 Author-email: lorenzo.posani@gmail.com
 Keywords: python,decoding,neuroscience,ccgp,neural activity,population activity,neural decoding,geometry
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `decodanda-0.6.8/README.md` & `decodanda-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.8/decodanda/classes.py` & `decodanda-0.6.9/decodanda/classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -530,32 +530,35 @@
             activityrate = np.nanmean(X > 0, 0)
             for key in resampled_rasters_A:
                 resampled_rasters_A[key] = resampled_rasters_A[key][:, activityrate > min_ar]
                 resampled_rasters_B[key] = resampled_rasters_B[key][:, activityrate > min_ar]
 
         return resampled_rasters_A, resampled_rasters_B
 
-    split_resample
-
     # Dichotomy analysis functions
 
-    def decode_dichotomy(self, dichotomy: Union[str, list], training_fraction: float,
-                         cross_validations: int = 10, ndata: Optional[int] = None,
-                         shuffled: bool = False, parallel: bool = False,
+    def decode_dichotomy(self,
+                         dichotomy: Union[str, list],
+                         training_fraction: float,
+                         cross_validations: int = 10,
+                         ndata: Optional[int] = None,
+                         shuffled: bool = False,
+                         parallel: bool = False,
                          testing_trials: Optional[list] = None,
-                         dic_key: Optional[str] = None, **kwargs) -> ndarray:
+                         dic_key: Optional[str] = None,
+                         subsample: Optional[float] = 0,
+                         **kwargs) -> ndarray:
         """
         Function that performs cross-validated decoding of a specific dichotomy.
         Decoding is performed by sampling a balanced amount of data points from each condition in each class of the
         dichotomy, so to ensure that only the desired variable is analyzed by balancing confounds.
         Before sampling, each condition is individually divided into training and testing bins
         by using the ``self.trial`` array specified in the data structure when constructing the ``Decodanda`` object.
 
 
-
         Parameters
         ----------
             dichotomy : str || list
                 The dichotomy to be decoded, expressed in a double-list binary format, e.g. [['10', '11'], ['01', '00']], or as a variable name.
             training_fraction:
                 the fraction of trials used for training in each cross-validation fold.
             cross_validations:
@@ -566,14 +569,16 @@
                 if True, population vectors for each condition are sampled in a random way compatibly with a null model for decoding performance.
             parallel:
                 if True, each cross-validation is performed by a dedicated thread (experimental, use with caution).
             testing_trials:
                 if specified, data sampled from the specified trial numbers will be used for testing, and the remaining ones for training.
             dic_key:
                 if specified, weights of the decoding analysis will be saved in self.decoding_weights using dic_key as the dictionary key.
+            subsample:
+                if >0, a random subsample of neurons of size=subsample will be used at each cross-validation
 
         Returns
         -------
             performances: list of decoding performance values for each cross-validation.
 
         Note
         ----
@@ -644,14 +649,15 @@
             print(dic, ndata)
             log_dichotomy(self, dic, ndata, 'Decoding')
             count = tqdm(range(cross_validations))
         else:
             count = range(cross_validations)
 
         if parallel:
+            # TODO: add subsample to the parallel routine
             pool = Pool()
             res = pool.map(CrossValidator(classifier=self.classifier,
                                           conditioned_rasters=self.conditioned_rasters,
                                           conditioned_trial_index=self.conditioned_trial_index,
                                           dic=dic,
                                           training_fraction=training_fraction,
                                           ndata=ndata,
@@ -669,17 +675,21 @@
             print(performances, weights)
 
         else:
             performances = np.zeros(cross_validations)
             if self._verbose and not shuffled:
                 print('\nLooping over decoding cross validation folds:')
             for i in count:
+                if subsample:
+                    self._generate_random_subset(subsample)
+
                 performances[i] = self._one_cv_step(dic=dic, training_fraction=training_fraction, ndata=ndata,
                                                     shuffled=shuffled, testing_trials=testing_trials, dic_key=dic_key)
-
+                if subsample:
+                    self._generate_random_subset(self.n_neurons)
         if shuffled:
             self._order_conditioned_rasters()
         return np.asarray(performances)
 
     def CCGP_dichotomy(self, dichotomy: Union[str, list],
                        resamplings: int = 3,
                        ndata: Optional[int] = None,
@@ -919,14 +929,15 @@
                               nshuffles: int = 10,
                               ndata: Optional[int] = None,
                               parallel: bool = False,
                               return_CV: bool = False,
                               testing_trials: Optional[list] = None,
                               plot: bool = False,
                               dic_key: Optional[str] = None,
+                              subsample: Optional[int] = 0,
                               **kwargs) -> Tuple[Union[list, ndarray], ndarray]:
         """
         Function that performs cross-validated decoding of a specific dichotomy and compares the resulting values with
         a null model where the relationship between the neural data and the two sides of the dichotomy is
         shuffled.
 
         Decoding is performed by sampling a balanced amount of data points from each condition in each class of the
@@ -954,14 +965,16 @@
                 if True, invidual cross-validation values are returned in a list. Otherwise, the average performance over the cross-validation folds is returned.
             testing_trials:
                 if specified, data sampled from the specified trial numbers will be used for testing, and the remaining ones for training.
             plot:
                 if True, a visualization of the decoding results is shown.
             dic_key:
                 if specified, weights of the decoding analysis will be saved in self.decoding_weights using dic_key as the dictionary key.
+            subsample:
+                if >0, a random subsample of neurons of size=subsample will be used at each cross-validation
 
 
         Returns
         -------
             performances, null_performances: list of decoding performance values for each cross-validation.
 
 
@@ -1031,15 +1044,16 @@
 
         d_performances = self.decode_dichotomy(dichotomy=dic,
                                                training_fraction=training_fraction,
                                                cross_validations=cross_validations,
                                                ndata=ndata,
                                                parallel=parallel,
                                                testing_trials=testing_trials,
-                                               dic_key=dic_key)
+                                               dic_key=dic_key,
+                                               subsample=subsample)
         if return_CV:
             data_performance = d_performances
         else:
             data_performance = np.nanmean(d_performances)
 
         if self._verbose and nshuffles:
             print(
@@ -1055,15 +1069,16 @@
             performances = self.decode_dichotomy(dichotomy=dic,
                                                  training_fraction=training_fraction,
                                                  cross_validations=cross_validations,
                                                  ndata=ndata,
                                                  parallel=parallel,
                                                  testing_trials=testing_trials,
                                                  shuffled=True,
-                                                 dic_key=dic_key)
+                                                 dic_key=dic_key,
+                                                 subsample=subsample)
 
             null_model_performances[n] = np.nanmean(performances)
 
         if plot:
             visualize_decoding(self, dic, d_performances, null_model_performances,
                                training_fraction=training_fraction, ndata=ndata, testing_trials=testing_trials)
 
@@ -1226,14 +1241,15 @@
 
     # Decoding analysis for semantic dichotomies
 
     def decode(self, training_fraction: float,
                cross_validations: int = 10,
                nshuffles: int = 10,
                ndata: Optional[int] = None,
+               subsample: Optional[int] = 0,
                parallel: bool = False,
                non_semantic: bool = False,
                return_CV: bool = False,
                testing_trials: Optional[list] = None,
                plot: bool = False,
                ax: Optional[plt.Axes] = None,
                plot_all: bool = False,
@@ -1279,14 +1295,16 @@
             the fraction of trials used for training in each cross-validation fold.
         cross_validations:
             the number of cross-validations.
         nshuffles:
             the number of null-model iterations of the decoding procedure.
         ndata:
             the number of data points (population vectors) sampled for training and for testing for each condition.
+        subsample:
+            if >0, a random subsample of neurons of size=subsample will be used at each cross-validation
         parallel:
             if True, each cross-validation is performed by a dedicated thread (experimental, use with caution).
         return_CV:
             if True, invidual cross-validation values are returned in a list. Otherwise, the average performance over the cross-validation folds is returned.
         testing_trials:
             if specified, data sampled from the specified trial numbers will be used for testing, and the remaining ones for training.
         non_semantic:
@@ -1335,30 +1353,32 @@
                 training_fraction,
                 cross_validations=cross_validations,
                 ndata=ndata,
                 nshuffles=nshuffles,
                 parallel=parallel,
                 return_CV=return_CV,
                 testing_trials=testing_trials,
-                plot=plot_all)
+                plot=plot_all,
+                subsample=subsample)
 
             perfs[key] = performance
             perfs_nullmodel[key] = null_model_performances
 
         if non_semantic and len(self.conditions) == 2:
             xor_dic = [['01', '10'], ['00', '11']]
             perfs_xor, perfs_null_xor = self.decode_with_nullmodel(dichotomy=xor_dic,
                                                                    training_fraction=training_fraction,
                                                                    cross_validations=cross_validations,
                                                                    nshuffles=nshuffles,
                                                                    parallel=parallel,
                                                                    ndata=ndata,
                                                                    return_CV=return_CV,
                                                                    testing_trials=testing_trials,
-                                                                   plot=plot_all)
+                                                                   plot=plot_all,
+                                                                   subsample=subsample)
             perfs['XOR'] = perfs_xor
             perfs_nullmodel['XOR'] = perfs_null_xor
 
         if non_semantic and len(self.conditions) > 2:
             dics = self._find_nonsemantic_dichotomies()
             for dic in dics:
                 dic_key = '_'.join(dic[0]) + '__' + '_'.join(dic[1])
@@ -1366,15 +1386,16 @@
                                                                  training_fraction=training_fraction,
                                                                  cross_validations=cross_validations,
                                                                  nshuffles=nshuffles,
                                                                  parallel=parallel,
                                                                  ndata=ndata,
                                                                  return_CV=return_CV,
                                                                  testing_trials=testing_trials,
-                                                                 plot=plot_all)
+                                                                 plot=plot_all,
+                                                                 subsample=subsample)
                 perfs[dic_key] = perfs_dic
                 perfs_nullmodel[dic_key] = null_dic
 
         if plot:
             if not ax:
                 f, ax = plt.subplots(figsize=(0.5 + 1.8 * len(perfs.keys()), 3.5))
             plot_perfs_null_model(perfs, perfs_nullmodel, ylabel='Decoding performance', ax=ax, **kwargs)
```

### Comparing `decodanda-0.6.8/decodanda/imports.py` & `decodanda-0.6.9/decodanda/imports.py`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.8/decodanda/in_time.py` & `decodanda-0.6.9/decodanda/in_time.py`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.8/decodanda/utilities.py` & `decodanda-0.6.9/decodanda/utilities.py`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.8/decodanda/visualize.py` & `decodanda-0.6.9/decodanda/visualize.py`

 * *Files identical despite different names*

### Comparing `decodanda-0.6.8/decodanda.egg-info/PKG-INFO` & `decodanda-0.6.9/decodanda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decodanda
-Version: 0.6.8
+Version: 0.6.9
 Summary: Geometric decoding of neural data with built-in best practices.
 Home-page: https://github.com/lposani/decodanda
 Author: Lorenzo Posani
 Author-email: lorenzo.posani@gmail.com
 Keywords: python,decoding,neuroscience,ccgp,neural activity,population activity,neural decoding,geometry
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `decodanda-0.6.8/setup.py` & `decodanda-0.6.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.6.8'
+VERSION = '0.6.9'
 DESCRIPTION = 'Geometric decoding of neural data with built-in best practices.'
 LONG_DESCRIPTION = 'Decodanda (dog latin for "to be decoded") is a best-practices-made-easy Python package for decoding neural data. Decodanda is designed to expose a user-friendly and flexible interface for population activity decoding, with a series of built-in best practices to avoid the most common pitfalls. In addition, Decodanda exposes a series of functions to compute the Cross-Condition Generalization Performance (CCGP, Bernardi et al. 2020) for the geometrical analysis of neural population activity.'
 
 setup(
     name="decodanda",
     version=VERSION,
     author="Lorenzo Posani",
```

