# Comparing `tmp/ml2json-0.3.1.tar.gz` & `tmp/ml2json-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml2json-0.3.1.tar", last modified: Wed Feb 14 17:45:56 2024, max compression
+gzip compressed data, was "ml2json-0.3.2.tar", last modified: Wed Apr 17 11:56:19 2024, max compression
```

## Comparing `ml2json-0.3.1.tar` & `ml2json-0.3.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-02-14 17:45:56.826263 ml2json-0.3.1/
--rw-rw-rw-   0        0        0     1084 2023-06-13 17:13:46.000000 ml2json-0.3.1/LICENSE
--rw-rw-rw-   0        0        0    43527 2024-02-14 17:45:56.825286 ml2json-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0    41937 2024-02-14 17:42:17.000000 ml2json-0.3.1/README.md
--rw-rw-rw-   0        0        0     1386 2024-02-14 17:45:56.887853 ml2json-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      123 2023-06-13 17:13:46.000000 ml2json-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-14 17:45:53.125011 ml2json-0.3.1/src/
-drwxrwxrwx   0        0        0        0 2024-02-14 17:45:54.605121 ml2json-0.3.1/src/ml2json/
--rw-rw-rw-   0        0        0    45800 2024-02-14 17:44:20.000000 ml2json-0.3.1/src/ml2json/__init__.py
--rw-rw-rw-   0        0        0    14744 2024-02-14 17:42:17.000000 ml2json-0.3.1/src/ml2json/applicability_domain.py
--rw-rw-rw-   0        0        0    60863 2024-02-14 17:42:17.000000 ml2json-0.3.1/src/ml2json/classification.py
--rw-rw-rw-   0        0        0    33438 2023-10-26 20:49:24.000000 ml2json-0.3.1/src/ml2json/cluster.py
--rw-rw-rw-   0        0        0    10988 2024-02-14 17:42:17.000000 ml2json-0.3.1/src/ml2json/cross_decomposition.py
--rw-rw-rw-   0        0        0    21059 2024-02-14 17:42:17.000000 ml2json-0.3.1/src/ml2json/decomposition.py
--rw-rw-rw-   0        0        0      862 2023-06-13 17:13:46.000000 ml2json-0.3.1/src/ml2json/feature_extraction.py
--rw-rw-rw-   0        0        0    13005 2023-10-26 20:49:24.000000 ml2json-0.3.1/src/ml2json/manifold.py
--rw-rw-rw-   0        0        0     8015 2024-02-14 17:42:17.000000 ml2json-0.3.1/src/ml2json/neighbors.py
--rw-rw-rw-   0        0        0    11094 2024-02-14 17:42:17.000000 ml2json-0.3.1/src/ml2json/preprocessing.py
--rw-rw-rw-   0        0        0    42745 2024-02-14 17:42:17.000000 ml2json-0.3.1/src/ml2json/regression.py
-drwxrwxrwx   0        0        0        0 2024-02-14 17:45:55.035271 ml2json-0.3.1/src/ml2json/utils/
--rw-rw-rw-   0        0        0      811 2023-06-13 17:13:46.000000 ml2json-0.3.1/src/ml2json/utils/__init__.py
--rw-rw-rw-   0        0        0      803 2023-06-13 17:13:46.000000 ml2json-0.3.1/src/ml2json/utils/csr.py
--rw-rw-rw-   0        0        0     1117 2023-06-13 17:13:46.000000 ml2json-0.3.1/src/ml2json/utils/memory.py
--rw-rw-rw-   0        0        0      476 2023-06-13 17:13:46.000000 ml2json-0.3.1/src/ml2json/utils/random_state.py
-drwxrwxrwx   0        0        0        0 2024-02-14 17:45:56.767605 ml2json-0.3.1/src/ml2json.egg-info/
--rw-rw-rw-   0        0        0    43527 2024-02-14 17:45:52.000000 ml2json-0.3.1/src/ml2json.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      913 2024-02-14 17:45:52.000000 ml2json-0.3.1/src/ml2json.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-14 17:45:52.000000 ml2json-0.3.1/src/ml2json.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      211 2024-02-14 17:45:52.000000 ml2json-0.3.1/src/ml2json.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-02-14 17:45:52.000000 ml2json-0.3.1/src/ml2json.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-14 17:45:56.743165 ml2json-0.3.1/test/
--rw-rw-rw-   0        0        0     6361 2024-02-14 17:42:17.000000 ml2json-0.3.1/test/test_applicability_domain.py
--rw-rw-rw-   0        0        0    15342 2023-06-13 17:13:46.000000 ml2json-0.3.1/test/test_classification.py
--rw-rw-rw-   0        0        0    14606 2023-06-13 17:13:46.000000 ml2json-0.3.1/test/test_cluster.py
--rw-rw-rw-   0        0        0     5599 2023-06-13 17:13:46.000000 ml2json-0.3.1/test/test_cross_decomposition.py
--rw-rw-rw-   0        0        0    14586 2024-02-14 17:42:17.000000 ml2json-0.3.1/test/test_decomposition.py
--rw-rw-rw-   0        0        0     2072 2023-06-13 17:13:46.000000 ml2json-0.3.1/test/test_feature_extraction.py
--rw-rw-rw-   0        0        0     4218 2023-06-13 17:13:46.000000 ml2json-0.3.1/test/test_manifold.py
--rw-rw-rw-   0        0        0     3393 2024-02-14 17:42:17.000000 ml2json-0.3.1/test/test_neighbors.py
--rw-rw-rw-   0        0        0     8120 2024-02-14 17:42:17.000000 ml2json-0.3.1/test/test_preprocessing.py
--rw-rw-rw-   0        0        0    13020 2024-02-14 17:42:17.000000 ml2json-0.3.1/test/test_regression.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:56:19.763953 ml2json-0.3.2/
+-rw-rw-rw-   0        0        0     1084 2023-06-08 11:50:24.000000 ml2json-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0    43527 2024-04-17 11:56:19.763953 ml2json-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0    41937 2024-04-17 11:51:29.000000 ml2json-0.3.2/README.md
+-rw-rw-rw-   0        0        0     1386 2024-04-17 11:56:19.768032 ml2json-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      123 2023-06-08 11:50:24.000000 ml2json-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:56:19.532507 ml2json-0.3.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-17 11:56:19.634403 ml2json-0.3.2/src/ml2json/
+-rw-rw-rw-   0        0        0    45800 2024-04-17 11:55:30.000000 ml2json-0.3.2/src/ml2json/__init__.py
+-rw-rw-rw-   0        0        0    14855 2024-04-17 11:51:29.000000 ml2json-0.3.2/src/ml2json/applicability_domain.py
+-rw-rw-rw-   0        0        0    60863 2024-04-17 11:51:29.000000 ml2json-0.3.2/src/ml2json/classification.py
+-rw-rw-rw-   0        0        0    33438 2023-12-01 13:05:09.000000 ml2json-0.3.2/src/ml2json/cluster.py
+-rw-rw-rw-   0        0        0    10988 2024-01-22 08:03:22.000000 ml2json-0.3.2/src/ml2json/cross_decomposition.py
+-rw-rw-rw-   0        0        0    21059 2024-01-22 08:03:22.000000 ml2json-0.3.2/src/ml2json/decomposition.py
+-rw-rw-rw-   0        0        0      862 2023-06-08 11:50:24.000000 ml2json-0.3.2/src/ml2json/feature_extraction.py
+-rw-rw-rw-   0        0        0    13005 2023-12-01 13:05:09.000000 ml2json-0.3.2/src/ml2json/manifold.py
+-rw-rw-rw-   0        0        0     8015 2024-01-22 08:03:22.000000 ml2json-0.3.2/src/ml2json/neighbors.py
+-rw-rw-rw-   0        0        0    11094 2024-01-22 08:03:22.000000 ml2json-0.3.2/src/ml2json/preprocessing.py
+-rw-rw-rw-   0        0        0    42745 2024-04-17 11:51:29.000000 ml2json-0.3.2/src/ml2json/regression.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:56:19.679465 ml2json-0.3.2/src/ml2json/utils/
+-rw-rw-rw-   0        0        0      811 2023-06-08 11:50:24.000000 ml2json-0.3.2/src/ml2json/utils/__init__.py
+-rw-rw-rw-   0        0        0      803 2023-06-08 11:50:24.000000 ml2json-0.3.2/src/ml2json/utils/csr.py
+-rw-rw-rw-   0        0        0     1117 2023-06-08 11:50:24.000000 ml2json-0.3.2/src/ml2json/utils/memory.py
+-rw-rw-rw-   0        0        0      476 2023-06-08 11:50:24.000000 ml2json-0.3.2/src/ml2json/utils/random_state.py
+drwxrwxrwx   0        0        0        0 2024-04-17 11:56:19.760954 ml2json-0.3.2/src/ml2json.egg-info/
+-rw-rw-rw-   0        0        0    43527 2024-04-17 11:56:19.000000 ml2json-0.3.2/src/ml2json.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      913 2024-04-17 11:56:19.000000 ml2json-0.3.2/src/ml2json.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 11:56:19.000000 ml2json-0.3.2/src/ml2json.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      211 2024-04-17 11:56:19.000000 ml2json-0.3.2/src/ml2json.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-17 11:56:19.000000 ml2json-0.3.2/src/ml2json.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 11:56:19.759961 ml2json-0.3.2/test/
+-rw-rw-rw-   0        0        0     6550 2024-04-17 11:51:29.000000 ml2json-0.3.2/test/test_applicability_domain.py
+-rw-rw-rw-   0        0        0    15342 2023-06-09 07:04:02.000000 ml2json-0.3.2/test/test_classification.py
+-rw-rw-rw-   0        0        0    14606 2023-06-09 07:05:37.000000 ml2json-0.3.2/test/test_cluster.py
+-rw-rw-rw-   0        0        0     5599 2023-06-09 07:04:22.000000 ml2json-0.3.2/test/test_cross_decomposition.py
+-rw-rw-rw-   0        0        0    14586 2024-01-22 14:10:38.000000 ml2json-0.3.2/test/test_decomposition.py
+-rw-rw-rw-   0        0        0     2072 2023-06-09 07:04:12.000000 ml2json-0.3.2/test/test_feature_extraction.py
+-rw-rw-rw-   0        0        0     4218 2023-06-09 07:04:02.000000 ml2json-0.3.2/test/test_manifold.py
+-rw-rw-rw-   0        0        0     3393 2024-01-22 08:03:22.000000 ml2json-0.3.2/test/test_neighbors.py
+-rw-rw-rw-   0        0        0     8120 2024-01-22 08:03:22.000000 ml2json-0.3.2/test/test_preprocessing.py
+-rw-rw-rw-   0        0        0    13020 2024-01-24 09:24:39.000000 ml2json-0.3.2/test/test_regression.py
```

### Comparing `ml2json-0.3.1/LICENSE` & `ml2json-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ml2json-0.3.1/PKG-INFO` & `ml2json-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml2json
-Version: 0.3.1
+Version: 0.3.2
 Summary: A safe, transparent way to share and deploy scikit-learn models.
 Home-page: https://github.com/OlivierBeq/ml2json
 Author: Mathieu Rodrigue
 Author-email: support@mlrequest.com
 Maintainer: Olivier J.M. Béquignon
 Maintainer-email: olivier.bequignon.maintainer@gmail.com
 License: MIT
```

### Comparing `ml2json-0.3.1/README.md` & `ml2json-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ml2json-0.3.1/setup.cfg` & `ml2json-0.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `ml2json-0.3.1/src/ml2json/__init__.py` & `ml2json-0.3.2/src/ml2json/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
                                                 KernelDensityApplicabilityDomain,
                                                 IsolationForestApplicabilityDomain,
                                                 CentroidDistanceApplicabilityDomain,
                                                 KNNApplicabilityDomain,
                                                 StandardizationApproachApplicabilityDomain)
 
 
-__version__ = '0.3.1'
+__version__ = '0.3.2'
 
 
 def serialize_model(model, catboost_data: Pool = None) -> Dict:
     """Serialize a model into a dictionary.
 
     :param model: machine learning model to be serialized
     :param catboost_data: if `model` is a CatBoost model, the data `Pool` used to train it
```

### Comparing `ml2json-0.3.1/src/ml2json/applicability_domain.py` & `ml2json-0.3.2/src/ml2json/applicability_domain.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
         return model
 
 def serialize_pca_bounding_box_applicability_domain(model):
     serialized_model = {
         'meta': 'pca-bounding-box-ad',
         'fitted_': model.fitted_,
-        'scaler': ml2json.to_dict(model.scaler),
+        'scaler': ml2json.to_dict(model.scaler) if model.scaler is not None else None,
         'min_explained_var': model.min_explained_var,
         'pca': ml2json.to_dict(model.pca),
     }
     if model.fitted_:
         serialized_model.update(
             {
             'num_points': model.num_points,
@@ -119,15 +119,16 @@
 
     return serialized_model
 
 if 'PCABoundingBoxApplicabilityDomain' in __optionals__:
     def deserialize_pca_bounding_box_applicability_domain(model_dict):
         model = PCABoundingBoxApplicabilityDomain()
         model.fitted_ = model_dict['fitted_']
-        model.scaler = ml2json.from_dict(model_dict['scaler'])
+        model.scaler = (ml2json.from_dict(model_dict['scaler'])
+                        if model_dict['scaler'] is not None else None)
         model.min_explained_var = model_dict['min_explained_var']
         model.pca = ml2json.from_dict(model_dict['pca'])
 
         if model.fitted_:
             model.num_points = model_dict['num_points']
             model.num_dims = model_dict['num_dims']
             model.min_ = np.array(model_dict['min_'])
```

### Comparing `ml2json-0.3.1/src/ml2json/classification.py` & `ml2json-0.3.2/src/ml2json/classification.py`

 * *Files identical despite different names*

### Comparing `ml2json-0.3.1/src/ml2json/cluster.py` & `ml2json-0.3.2/src/ml2json/cluster.py`

 * *Files identical despite different names*

### Comparing `ml2json-0.3.1/src/ml2json/cross_decomposition.py` & `ml2json-0.3.2/src/ml2json/cross_decomposition.py`

 * *Files identical despite different names*

### Comparing `ml2json-0.3.1/src/ml2json/decomposition.py` & `ml2json-0.3.2/src/ml2json/decomposition.py`

 * *Files identical despite different names*

### Comparing `ml2json-0.3.1/src/ml2json/feature_extraction.py` & `ml2json-0.3.2/src/ml2json/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `ml2json-0.3.1/src/ml2json/manifold.py` & `ml2json-0.3.2/src/ml2json/manifold.py`

 * *Files identical despite different names*

### Comparing `ml2json-0.3.1/src/ml2json/neighbors.py` & `ml2json-0.3.2/src/ml2json/neighbors.py`

 * *Files identical despite different names*

### Comparing `ml2json-0.3.1/src/ml2json/preprocessing.py` & `ml2json-0.3.2/src/ml2json/preprocessing.py`

 * *Files identical despite different names*

### Comparing `ml2json-0.3.1/src/ml2json/regression.py` & `ml2json-0.3.2/src/ml2json/regression.py`

 * *Files identical despite different names*

### Comparing `ml2json-0.3.1/src/ml2json/utils/__init__.py` & `ml2json-0.3.2/src/ml2json/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ml2json-0.3.1/src/ml2json/utils/csr.py` & `ml2json-0.3.2/src/ml2json/utils/csr.py`

 * *Files identical despite different names*

### Comparing `ml2json-0.3.1/src/ml2json/utils/memory.py` & `ml2json-0.3.2/src/ml2json/utils/memory.py`

 * *Files identical despite different names*

### Comparing `ml2json-0.3.1/src/ml2json.egg-info/PKG-INFO` & `ml2json-0.3.2/src/ml2json.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml2json
-Version: 0.3.1
+Version: 0.3.2
 Summary: A safe, transparent way to share and deploy scikit-learn models.
 Home-page: https://github.com/OlivierBeq/ml2json
 Author: Mathieu Rodrigue
 Author-email: support@mlrequest.com
 Maintainer: Olivier J.M. Béquignon
 Maintainer-email: olivier.bequignon.maintainer@gmail.com
 License: MIT
```

### Comparing `ml2json-0.3.1/src/ml2json.egg-info/SOURCES.txt` & `ml2json-0.3.2/src/ml2json.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml2json-0.3.1/test/test_applicability_domain.py` & `ml2json-0.3.2/test/test_applicability_domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,18 @@
         model = ConvexHullApplicabilityDomain()
         self.check_applicability_domain(model, 'convex-hull-ad.json')
 
     @unittest.skipIf(len(__optionals__) == 0, 'Optional dependencies not installed.')
     def test_pca_bounding_box_applicability_domain(self):
         model = PCABoundingBoxApplicabilityDomain()
         self.check_applicability_domain(model, 'pca-bounding-box-ad.json')
+        
+        # check with scaling is None
+        model = PCABoundingBoxApplicabilityDomain(scaling=None)
+        self.check_applicability_domain(model, 'pca-bounding-box-ad.json')
 
     @unittest.skipIf(len(__optionals__) == 0, 'Optional dependencies not installed.')
     def test_topkat_applicability_domain(self):
         model = TopKatApplicabilityDomain()
         self.check_applicability_domain(model, 'topkat-ad.json')
 
     @unittest.skipIf(len(__optionals__) == 0, 'Optional dependencies not installed.')
```

### Comparing `ml2json-0.3.1/test/test_classification.py` & `ml2json-0.3.2/test/test_classification.py`

 * *Files identical despite different names*

### Comparing `ml2json-0.3.1/test/test_cluster.py` & `ml2json-0.3.2/test/test_cluster.py`

 * *Files identical despite different names*

### Comparing `ml2json-0.3.1/test/test_cross_decomposition.py` & `ml2json-0.3.2/test/test_cross_decomposition.py`

 * *Files identical despite different names*

### Comparing `ml2json-0.3.1/test/test_decomposition.py` & `ml2json-0.3.2/test/test_decomposition.py`

 * *Files identical despite different names*

### Comparing `ml2json-0.3.1/test/test_feature_extraction.py` & `ml2json-0.3.2/test/test_feature_extraction.py`

 * *Files identical despite different names*

### Comparing `ml2json-0.3.1/test/test_manifold.py` & `ml2json-0.3.2/test/test_manifold.py`

 * *Files identical despite different names*

### Comparing `ml2json-0.3.1/test/test_neighbors.py` & `ml2json-0.3.2/test/test_neighbors.py`

 * *Files identical despite different names*

### Comparing `ml2json-0.3.1/test/test_preprocessing.py` & `ml2json-0.3.2/test/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `ml2json-0.3.1/test/test_regression.py` & `ml2json-0.3.2/test/test_regression.py`

 * *Files identical despite different names*

