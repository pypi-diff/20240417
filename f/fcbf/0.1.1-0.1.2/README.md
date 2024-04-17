# Comparing `tmp/fcbf-0.1.1.tar.gz` & `tmp/fcbf-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcbf-0.1.1.tar", max compression
+gzip compressed data, was "fcbf-0.1.2.tar", max compression
```

## Comparing `fcbf-0.1.1.tar` & `fcbf-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0      400 2022-09-21 18:54:27.674384 fcbf-0.1.1/DESCRIPTION.md
--rw-r--r--   0        0        0      139 2022-09-21 19:36:36.733317 fcbf-0.1.1/fcbf/__init__.py
--rw-r--r--   0        0        0       37 2022-09-21 19:26:52.754445 fcbf-0.1.1/fcbf/data/__init__.py
--rw-r--r--   0        0        0      199 2022-09-21 19:31:40.130901 fcbf-0.1.1/fcbf/data/datasets.py
--rw-r--r--   0        0        0     3649 2022-09-19 15:11:18.350906 fcbf-0.1.1/fcbf/data/lung-cancer.data
--rw-r--r--   0        0        0     7196 2022-09-21 19:32:25.443996 fcbf-0.1.1/fcbf/fcbf.py
--rw-r--r--   0        0        0     1089 2022-09-19 19:40:38.717646 fcbf-0.1.1/LICENSE
--rw-r--r--   0        0        0      738 2022-09-21 19:36:36.733317 fcbf-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1102 2022-09-21 19:38:55.869753 fcbf-0.1.1/setup.py
--rw-r--r--   0        0        0     1252 2022-09-21 19:38:55.870753 fcbf-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      400 2022-09-21 18:54:27.674384 fcbf-0.1.2/DESCRIPTION.md
+-rw-r--r--   0        0        0      139 2024-04-17 06:31:43.084898 fcbf-0.1.2/fcbf/__init__.py
+-rw-r--r--   0        0        0       37 2024-04-17 06:29:28.120365 fcbf-0.1.2/fcbf/data/__init__.py
+-rw-r--r--   0        0        0      199 2024-04-17 06:29:30.274635 fcbf-0.1.2/fcbf/data/datasets.py
+-rw-r--r--   0        0        0     3649 2022-09-19 15:11:18.350906 fcbf-0.1.2/fcbf/data/lung-cancer.data
+-rw-r--r--   0        0        0     7207 2024-04-17 06:28:02.566563 fcbf-0.1.2/fcbf/fcbf.py
+-rw-r--r--   0        0        0     1089 2024-04-17 06:31:01.801304 fcbf-0.1.2/LICENSE
+-rw-r--r--   0        0        0      755 2024-04-17 06:31:39.609670 fcbf-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1307 1970-01-01 00:00:00.000000 fcbf-0.1.2/PKG-INFO
```

### Comparing `fcbf-0.1.1/fcbf/data/lung-cancer.data` & `fcbf-0.1.2/fcbf/data/lung-cancer.data`

 * *Files identical despite different names*

### Comparing `fcbf-0.1.1/fcbf/fcbf.py` & `fcbf-0.1.2/fcbf/fcbf.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,45 +18,48 @@
 
     Returns:
         pd.Series: The prior.
     """
     n = X.size
     return X.value_counts()/n
 
+
 def cond_proba(X: pd.Series, y: pd.Series) -> pd.Series:
     """Calculates the conditional probability of a feature given the class.
     # TODO: accept a nx2 df containing X and y
 
     Args:
         X (pd.Series): The series of a feature's values.
         y (pd.Series): The class values. Need to correspond to X.
 
     Returns:
         pd.Series: The conditional probability.
     """
-    sample = pd.concat([X, y], axis=1, )
+    sample = pd.concat([X, y], axis=1)
     return sample.groupby([X.name, y.name]).size().div(len(sample.index)).div(prior(y), axis=0, level=y.name)
 
-def cond_entropy(X: pd.Series, y: pd.Series, base: float =np.e) -> float:
+
+def cond_entropy(X: pd.Series, y: pd.Series, base: float = np.e) -> float:
     """Calculates the conditional entropy of a feature given the class.
 
     Args:
         X (pd.Series): The series of a feature's values.
         y (pd.Series): The class values. Need to correspond to X.
         base (float, optional): The logarithm base to apply. Defaults to np.e.
 
     Returns:
         float: The conditional entropy.
     """
     cond_proba_ = cond_proba(X, y)
     logged_cond_proba_ = np.log(cond_proba_) / np.log(base)
     prod = cond_proba_ * logged_cond_proba_
-    return -1 * prod.sum(axis=0, level=y.name).mul(prior(y)).sum(axis=0)
+    return -1 * prod.groupby(level=y.name).sum().mul(prior(y)).sum()
+
 
-def information_gain(X: pd.Series, y: pd.Series, base: float=np.e) -> float:
+def information_gain(X: pd.Series, y: pd.Series, base: float = np.e) -> float:
     """Calculates the information gain IG of a feature regarding the class.
     Formula: IG(X|y) = entropy(X) - cond_entropy(X|y)
 
     Args:
         X (pd.Series): The series of a feature's values.
         y (pd.Series): The class values. Need to correspond to X.
         base (float, optional): The logarithm base to apply. Defaults to np.e.
@@ -70,15 +73,16 @@
     if entropy_ < 0:
         raise RuntimeError('entropy < 0 detected.')
     if entropy_ < cond_entropy_:
         raise RuntimeError('entropy < associated conditional entropy detected.')
 
     return entropy_ - cond_entropy_
 
-def symmetrical_uncertainty(X: pd.Series, y: pd.Series, base: float=np.e) -> float:
+
+def symmetrical_uncertainty(X: pd.Series, y: pd.Series, base: float = np.e) -> float:
     """Calculates the symmetrical uncertainty SU of a feature regarding the class.
     Formula: SU(X,y) = 2 * IG(X|y) / ( entropy(X) + entropy(y) )
 
     Args:
         X (pd.Series): The series of a feature's values.
         y (pd.Series): The class values. Need to correspond to X.
         base (float, optional): The logarithm base to apply. Defaults to np.e.
@@ -88,16 +92,17 @@
     """
     entropy_X = entropy(prior(X), base=base)
     entropy_y = entropy(prior(y), base=base)
     information_gain_ = information_gain(X, y, base=base)
 
     return 2 * information_gain_ / (entropy_X + entropy_y)
 
+
 def fcbf(X: pd.DataFrame, y: pd.Series,
-         su_threshold: float=0.0, base: float=np.e) -> Tuple[list, list, dict]:
+         su_threshold: float = 0.0, base: float = np.e) -> Tuple[list, list, dict]:
     """Fast correlation-based filter algorithm introduced by Yu and Liu.
     @inproceedings{inproceedings,
     author = {Yu, Lei and Liu, Huan},
     year = {2003},
     month = {01},
     pages = {856-863},
     title = {Feature Selection for High-Dimensional Data: A Fast Correlation-Based Filter Solution},
@@ -180,15 +185,14 @@
     return relevant_feature_names_sorted, irrelevant_feature_names, correlation_values
 
 
 if __name__ == '__main__':
 
     from fcbf import data
 
-
     dataset = data.lung_cancer
     X = dataset[dataset.columns[1:]]
     y = dataset[dataset.columns[0]].astype(int)
     print(X)
     print(y)
 
     relevant_features, irrelevant_features, correlations = fcbf(X, y, su_threshold=0.1, base=2)
```

### Comparing `fcbf-0.1.1/LICENSE` & `fcbf-0.1.2/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Martin Trat
+Copyright (c) 2024 Martin Trat
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `fcbf-0.1.1/PKG-INFO` & `fcbf-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: fcbf
-Version: 0.1.1
+Version: 0.1.2
 Summary: Categorical feature selection based on information theoretical considerations
 Home-page: https://github.com/m-martin-j/fcbf
 License: MIT
 Author: Martin Trat
 Author-email: martin.trat@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: scipy
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: pandas (>=2.2.2,<3.0.0)
+Requires-Dist: scipy (>=1.13.0,<2.0.0)
 Project-URL: Repository, https://github.com/m-martin-j/fcbf
 Description-Content-Type: text/markdown
 
 Implementation of the fast correlation-based filter (FCBF) proposed by Yu and Liu:
 
 @inproceedings{inproceedings,
 author = {Yu, Lei and Liu, Huan},
```

