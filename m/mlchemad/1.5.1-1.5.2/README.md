# Comparing `tmp/mlchemad-1.5.1.tar.gz` & `tmp/mlchemad-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlchemad-1.5.1.tar", last modified: Fri Feb 23 10:09:10 2024, max compression
+gzip compressed data, was "mlchemad-1.5.2.tar", last modified: Wed Apr 17 11:44:56 2024, max compression
```

## Comparing `mlchemad-1.5.1.tar` & `mlchemad-1.5.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-02-23 10:09:10.803766 mlchemad-1.5.1/
--rw-rw-rw-   0        0        0     1087 2023-12-07 22:30:44.000000 mlchemad-1.5.1/LICENSE
--rw-rw-rw-   0        0        0     3038 2024-02-23 10:09:10.803766 mlchemad-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     1891 2024-02-23 10:06:55.000000 mlchemad-1.5.1/README.md
--rw-rw-rw-   0        0        0     1377 2024-02-23 10:09:10.803766 mlchemad-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0      123 2023-06-08 11:50:24.000000 mlchemad-1.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-23 10:09:10.725628 mlchemad-1.5.1/src/
-drwxrwxrwx   0        0        0        0 2024-02-23 10:09:10.772518 mlchemad-1.5.1/src/mlchemad/
--rw-rw-rw-   0        0        0      703 2024-02-23 10:08:37.000000 mlchemad-1.5.1/src/mlchemad/__init__.py
--rw-rw-rw-   0        0        0     3780 2024-01-12 09:29:09.000000 mlchemad-1.5.1/src/mlchemad/_data.py
--rw-rw-rw-   0        0        0    29611 2024-02-23 10:07:52.000000 mlchemad-1.5.1/src/mlchemad/applicability_domains.py
--rw-rw-rw-   0        0        0     2253 2023-12-13 11:50:48.000000 mlchemad-1.5.1/src/mlchemad/base.py
--rw-rw-rw-   0        0        0  5087154 2024-01-12 09:29:09.000000 mlchemad-1.5.1/src/mlchemad/broccatelli2011.json
--rw-rw-rw-   0        0        0     4124 2023-12-19 12:22:06.000000 mlchemad-1.5.1/src/mlchemad/fisher1936.json
--rw-rw-rw-   0        0        0   473108 2024-01-12 10:27:04.000000 mlchemad-1.5.1/src/mlchemad/hemmerich2020.json
--rw-rw-rw-   0        0        0     5214 2023-12-19 12:23:03.000000 mlchemad-1.5.1/src/mlchemad/mekenyan1993.json
--rw-rw-rw-   0        0        0     2485 2023-12-08 12:10:46.000000 mlchemad-1.5.1/src/mlchemad/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-23 10:09:10.803766 mlchemad-1.5.1/src/mlchemad.egg-info/
--rw-rw-rw-   0        0        0     3038 2024-02-23 10:09:10.000000 mlchemad-1.5.1/src/mlchemad.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      485 2024-02-23 10:09:10.000000 mlchemad-1.5.1/src/mlchemad.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-23 10:09:10.000000 mlchemad-1.5.1/src/mlchemad.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-02-23 10:09:10.000000 mlchemad-1.5.1/src/mlchemad.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-02-23 10:09:10.000000 mlchemad-1.5.1/src/mlchemad.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-23 10:09:10.803766 mlchemad-1.5.1/test/
--rw-rw-rw-   0        0        0    17552 2024-01-12 10:28:11.000000 mlchemad-1.5.1/test/test_ad.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:44:56.134222 mlchemad-1.5.2/
+-rw-rw-rw-   0        0        0     1087 2023-12-07 22:30:44.000000 mlchemad-1.5.2/LICENSE
+-rw-rw-rw-   0        0        0     3038 2024-04-17 11:44:56.134222 mlchemad-1.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1891 2024-02-23 10:06:55.000000 mlchemad-1.5.2/README.md
+-rw-rw-rw-   0        0        0     1377 2024-04-17 11:44:56.134222 mlchemad-1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      123 2023-06-08 11:50:24.000000 mlchemad-1.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:44:56.047477 mlchemad-1.5.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-17 11:44:56.099013 mlchemad-1.5.2/src/mlchemad/
+-rw-rw-rw-   0        0        0      703 2024-04-17 11:44:10.000000 mlchemad-1.5.2/src/mlchemad/__init__.py
+-rw-rw-rw-   0        0        0     3780 2024-01-12 09:29:09.000000 mlchemad-1.5.2/src/mlchemad/_data.py
+-rw-rw-rw-   0        0        0    30003 2024-04-17 11:43:00.000000 mlchemad-1.5.2/src/mlchemad/applicability_domains.py
+-rw-rw-rw-   0        0        0     2253 2023-12-13 11:50:48.000000 mlchemad-1.5.2/src/mlchemad/base.py
+-rw-rw-rw-   0        0        0  5087154 2024-01-12 09:29:09.000000 mlchemad-1.5.2/src/mlchemad/broccatelli2011.json
+-rw-rw-rw-   0        0        0     4124 2023-12-19 12:22:06.000000 mlchemad-1.5.2/src/mlchemad/fisher1936.json
+-rw-rw-rw-   0        0        0   473108 2024-01-12 10:27:04.000000 mlchemad-1.5.2/src/mlchemad/hemmerich2020.json
+-rw-rw-rw-   0        0        0     5214 2023-12-19 12:23:03.000000 mlchemad-1.5.2/src/mlchemad/mekenyan1993.json
+-rw-rw-rw-   0        0        0     2485 2023-12-08 12:10:46.000000 mlchemad-1.5.2/src/mlchemad/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:44:56.134222 mlchemad-1.5.2/src/mlchemad.egg-info/
+-rw-rw-rw-   0        0        0     3038 2024-04-17 11:44:56.000000 mlchemad-1.5.2/src/mlchemad.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      485 2024-04-17 11:44:56.000000 mlchemad-1.5.2/src/mlchemad.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 11:44:56.000000 mlchemad-1.5.2/src/mlchemad.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-17 11:44:56.000000 mlchemad-1.5.2/src/mlchemad.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-17 11:44:56.000000 mlchemad-1.5.2/src/mlchemad.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 11:44:56.134222 mlchemad-1.5.2/test/
+-rw-rw-rw-   0        0        0    18261 2024-04-17 11:43:00.000000 mlchemad-1.5.2/test/test_ad.py
```

### Comparing `mlchemad-1.5.1/LICENSE` & `mlchemad-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mlchemad-1.5.1/PKG-INFO` & `mlchemad-1.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlchemad
-Version: 1.5.1
+Version: 1.5.2
 Summary: Applicability domains for cheminformactics.
 Home-page: https://github.com/OlivierBeq/mlchemad
 Author: Olivier J.M. Béquignon
 Author-email: olivier.bequignon.maintainer@gmail.com
 Maintainer: Olivier J.M. Béquignon
 Maintainer-email: olivier.bequignon.maintainer@gmail.com
 License: MIT
```

### Comparing `mlchemad-1.5.1/README.md` & `mlchemad-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `mlchemad-1.5.1/setup.cfg` & `mlchemad-1.5.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `mlchemad-1.5.1/src/mlchemad/__init__.py` & `mlchemad-1.5.2/src/mlchemad/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 
-__version__ = '1.5.1'
+__version__ = '1.5.2'
 
 
 from .applicability_domains import (BoundingBoxApplicabilityDomain, CentroidDistanceApplicabilityDomain,
                                     ConvexHullApplicabilityDomain, HotellingT2ApplicabilityDomain,
                                     IsolationForestApplicabilityDomain, KNNApplicabilityDomain,
                                     KernelDensityApplicabilityDomain, LeverageApplicabilityDomain,
                                     PCABoundingBoxApplicabilityDomain, TopKatApplicabilityDomain,
```

### Comparing `mlchemad-1.5.1/src/mlchemad/_data.py` & `mlchemad-1.5.2/src/mlchemad/_data.py`

 * *Files identical despite different names*

### Comparing `mlchemad-1.5.1/src/mlchemad/applicability_domains.py` & `mlchemad-1.5.2/src/mlchemad/applicability_domains.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,63 +147,65 @@
                                                     ).success
                              for sample_ in samples])
 
 
 class PCABoundingBoxApplicabilityDomain(ApplicabilityDomain):
     """Applicability domain defined as the bounding box around the principal components of the training feature matrix."""
 
-    def __init__(self, scaling: str = 'robust', explained_var: float = 0.9,
+    def __init__(self, scaling: str | None = 'robust', explained_var: float = 0.9,
                  random_state: Union[int, RandomState] = 1234,
                  scaler_kwargs=None, pca_kwargs=None):
         """Create the convex hull applicability domain. Transforms the input features
         with principal component analysis (PCA) to ensure a convex hull is found.
 
-        :param scaling: scaling method; must be one of 'robust', 'minmax', 'maxabs' or 'standard' (default: 'robust')
+        :param scaling: scaling method; must be one of 'robust', 'minmax', 'maxabs', 'standard' or None (default: 'robust')
         :param explained_var: minimum value principal components' cumulative variance must reach to be included
         :param random_state: random state of the principal component analysis (PCA)
         :param scaler_kwargs: additional parameters to supply to the scaler
         :param pca_kwargs: additional parameters to supply to the PCA
         """
         super().__init__()
         if pca_kwargs is None:
             pca_kwargs = {}
         if scaler_kwargs is None:
             scaler_kwargs = {}
         scaling_methods = ('robust', 'minmax', 'maxabs', 'standard')
-        if scaling not in scaling_methods:
+        if scaling not in scaling_methods and scaling is not None:
             raise ValueError(f'scaling method must be one of {scaling_methods}')
         if 'random_state' in pca_kwargs:
             raise ValueError('pca_kwargs must not set the following parameters: \'random_state\'')
         # Scaler for input data
         if scaling == 'robust':
             self.scaler = RobustScaler(**scaler_kwargs)
         elif scaling == 'minmax':
             self.scaler = MinMaxScaler(**scaler_kwargs)
         elif scaling == 'maxabs':
             self.scaler = MaxAbsScaler(**scaler_kwargs)
         elif scaling == 'standard':
             self.scaler = StandardScaler(**scaler_kwargs)
+        elif scaling is None:
+            self.scaler = None
         else:
-            raise NotImplementedError('scaling methof not implemented')
+            raise NotImplementedError('scaling method not implemented')
         self.min_explained_var = explained_var
         # PCA ensuring the simplex is not flat
         self.pca = PCA(random_state=random_state,
                        **pca_kwargs)
 
     def _fit(self, X):
         """Fit the applicability domain to the given feature matrix
 
         :param X: feature matrix
         """
         # Fit scaler and PCA
-        X = self.scaler.fit_transform(X)
+        X = self.scaler.fit_transform(X) if self.scaler is not None else X
         self.pca.fit(X)
         # Determine the number of components
         ratio_cumsum = stable_cumsum(self.pca.explained_variance_ratio_)
-        n_components = np.searchsorted(ratio_cumsum, self.pca.n_components_, side="right") + 1
+        n_components = np.searchsorted(ratio_cumsum, self.min_explained_var, side="right") + 1
         # Modify the PCA object in place
         self.pca.components_ = self.pca.components_[:n_components]
         self.pca.n_components_ = n_components
         self.pca.explained_variance_ = self.pca.explained_variance_[:n_components]
         self.pca.explained_variance_ratio_ = self.pca.explained_variance_ratio_[:n_components]
         self.pca.singular_values_ = self.pca.singular_values_[:n_components]
         # Determine extremum values
@@ -216,17 +218,20 @@
     def _contains(self, sample):
         """Determine if a sample is in the applicability domain.
 
         :param sample: sample to check the applicability domain membership of.
         """
         # Scale input features
         if sample.ndim == 1:
-            sample = self.pca.transform(self.scaler.transform(sample.reshape((1, len(sample)))))
+            sample = sample.reshape((1, len(sample)))
+            sample = self.scaler.transform(sample) if self.scaler is not None else sample
+            sample = self.pca.transform(sample)
             return ((sample >= self.min_) & (sample <= self.max_)).all()
-        sample = self.pca.transform(self.scaler.transform(sample))
+        sample = self.scaler.transform(sample) if self.scaler is not None else sample
+        sample = self.pca.transform(sample)
         return ((sample >= self.min_) & (sample <= self.max_)).all(axis=1)
 
 
 class TopKatApplicabilityDomain(ApplicabilityDomain):
     """Applicability domain defined as TOPKAT's Optimal Prediction Space (OPS).
 
     Reference:
@@ -513,16 +518,16 @@
 
         :param X: feature matrix
         """
         # Normalize the data
         self.X_norm = self.scaler.fit_transform(X) if self.scaler is not None else X
         # Fit the NN
         self.nn.fit(self.X_norm)
-        # Find the distance to the kNN
-        self.kNN_dist = self.nn.kneighbors(self.X_norm, return_distance=True)[0].mean(axis=1)
+        # Find the distance to the kNN neighbors (ignoring the first neighbor, which is the sample itself)
+        self.kNN_dist = self.nn.kneighbors(self.X_norm, return_distance=True, n_neighbors=self.k+1)[0][:, 1:].mean(axis=1)
         kNN_train_distance_sorted_ = np.trim_zeros(np.sort(self.kNN_dist))
         # Find the confidence threshold
         if self.hard_threshold:
             self.threshold_ = self.hard_threshold
         else:
             self.threshold_ = kNN_train_distance_sorted_[floor(kNN_train_distance_sorted_.shape[0] * self.alpha) - 1]
         return self
```

### Comparing `mlchemad-1.5.1/src/mlchemad/base.py` & `mlchemad-1.5.2/src/mlchemad/base.py`

 * *Files identical despite different names*

### Comparing `mlchemad-1.5.1/src/mlchemad/broccatelli2011.json` & `mlchemad-1.5.2/src/mlchemad/broccatelli2011.json`

 * *Files identical despite different names*

### Comparing `mlchemad-1.5.1/src/mlchemad/fisher1936.json` & `mlchemad-1.5.2/src/mlchemad/fisher1936.json`

 * *Files identical despite different names*

### Comparing `mlchemad-1.5.1/src/mlchemad/hemmerich2020.json` & `mlchemad-1.5.2/src/mlchemad/hemmerich2020.json`

 * *Files identical despite different names*

### Comparing `mlchemad-1.5.1/src/mlchemad/mekenyan1993.json` & `mlchemad-1.5.2/src/mlchemad/mekenyan1993.json`

 * *Files identical despite different names*

### Comparing `mlchemad-1.5.1/src/mlchemad/utils.py` & `mlchemad-1.5.2/src/mlchemad/utils.py`

 * *Files identical despite different names*

### Comparing `mlchemad-1.5.1/src/mlchemad.egg-info/PKG-INFO` & `mlchemad-1.5.2/src/mlchemad.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlchemad
-Version: 1.5.1
+Version: 1.5.2
 Summary: Applicability domains for cheminformactics.
 Home-page: https://github.com/OlivierBeq/mlchemad
 Author: Olivier J.M. Béquignon
 Author-email: olivier.bequignon.maintainer@gmail.com
 Maintainer: Olivier J.M. Béquignon
 Maintainer-email: olivier.bequignon.maintainer@gmail.com
 License: MIT
```

### Comparing `mlchemad-1.5.1/test/test_ad.py` & `mlchemad-1.5.2/test/test_ad.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,27 @@
         self.assertEquals(sum(ad.contains(self.X_cent6_sd1)),
                           0)
         self.assertLess(sum(ad.contains(self.X_cent1_sd3)),
                         len(self.X_cent1_sd3))
         ad.fit(self.mekenyan_veith.training)
         self.assertGreaterEqual(sum(ad.contains(self.mekenyan_veith.test)), 0)
         self.assertLessEqual(sum(ad.contains(self.mekenyan_veith.test)), self.mekenyan_veith.test.shape[0])
+        
+    def test_pca_none_boundingbox(self):
+        ad = PCABoundingBoxApplicabilityDomain(scaling=None)
+        ad.fit(self.X_cent1_sd1)
+        self.assertGreater(sum(ad.contains(self.X_cent1_sd1)),
+                            0.9 * len(self.X_cent1_sd1))
+        self.assertEquals(sum(ad.contains(self.X_cent6_sd1)),
+                            0)
+        self.assertLess(sum(ad.contains(self.X_cent1_sd3)),
+                        len(self.X_cent1_sd3))
+        ad.fit(self.mekenyan_veith.training)
+        self.assertGreaterEqual(sum(ad.contains(self.mekenyan_veith.test)), 0)
+        self.assertLessEqual(sum(ad.contains(self.mekenyan_veith.test)), self.mekenyan_veith.test.shape[0])
 
     def test_leverage(self):
         ad = LeverageApplicabilityDomain()
         ad.fit(self.X_cent1_sd1)
         self.assertGreater(sum(ad.contains(self.X_cent1_sd1)),
                            0.9 * len(self.X_cent1_sd1))
         self.assertEquals(sum(ad.contains(self.X_cent6_sd3)),
```

