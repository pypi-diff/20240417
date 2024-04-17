# Comparing `tmp/rnaformer-1.0.2.tar.gz` & `tmp/rnaformer-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rnaformer-1.0.2.tar", last modified: Tue Apr 16 14:21:52 2024, max compression
+gzip compressed data, was "rnaformer-1.0.3.tar", last modified: Tue Apr 16 14:44:06 2024, max compression
```

## Comparing `rnaformer-1.0.2.tar` & `rnaformer-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-04-16 14:21:52.823467 rnaformer-1.0.2/
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)    11347 2024-04-10 11:44:16.000000 rnaformer-1.0.2/LICENSE
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     4970 2024-04-16 14:21:52.823467 rnaformer-1.0.2/PKG-INFO
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     4381 2024-04-10 11:44:16.000000 rnaformer-1.0.2/README.md
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)      626 2024-04-16 14:21:24.000000 rnaformer-1.0.2/pyproject.toml
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-04-16 14:21:52.823467 rnaformer-1.0.2/rnaformer.egg-info/
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     4970 2024-04-16 14:21:52.000000 rnaformer-1.0.2/rnaformer.egg-info/PKG-INFO
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)      173 2024-04-16 14:21:52.000000 rnaformer-1.0.2/rnaformer.egg-info/SOURCES.txt
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)        1 2024-04-16 14:21:52.000000 rnaformer-1.0.2/rnaformer.egg-info/dependency_links.txt
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)        1 2024-04-16 14:21:52.000000 rnaformer-1.0.2/rnaformer.egg-info/top_level.txt
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)       38 2024-04-16 14:21:52.823467 rnaformer-1.0.2/setup.cfg
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)      253 2024-04-16 14:20:11.000000 rnaformer-1.0.2/setup.py
+drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-04-16 14:44:06.584848 rnaformer-1.0.3/
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)    11347 2024-04-10 11:44:16.000000 rnaformer-1.0.3/LICENSE
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     4970 2024-04-16 14:44:06.584848 rnaformer-1.0.3/PKG-INFO
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     4381 2024-04-10 11:44:16.000000 rnaformer-1.0.3/README.md
+drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-04-16 14:44:06.584848 rnaformer-1.0.3/RNAformer.egg-info/
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     4970 2024-04-16 14:44:06.000000 rnaformer-1.0.3/RNAformer.egg-info/PKG-INFO
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)      173 2024-04-16 14:44:06.000000 rnaformer-1.0.3/RNAformer.egg-info/SOURCES.txt
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)        1 2024-04-16 14:44:06.000000 rnaformer-1.0.3/RNAformer.egg-info/dependency_links.txt
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)        1 2024-04-16 14:44:06.000000 rnaformer-1.0.3/RNAformer.egg-info/top_level.txt
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)      626 2024-04-16 14:42:59.000000 rnaformer-1.0.3/pyproject.toml
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)       38 2024-04-16 14:44:06.584848 rnaformer-1.0.3/setup.cfg
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)      253 2024-04-16 14:43:06.000000 rnaformer-1.0.3/setup.py
```

### Comparing `rnaformer-1.0.2/LICENSE` & `rnaformer-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rnaformer-1.0.2/PKG-INFO` & `rnaformer-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rnaformer
-Version: 1.0.2
+Name: RNAformer
+Version: 1.0.3
 Summary: RNAformer: a simple single-sequence-based deep learning model for RNA secondary structure prediction.
 Author: Frederic Runge, Rolf Backofen, Frank Hutter
 Author-email: "Joerg K.H. Franke" <frankej@cs.uni-freiburg.de>, Ryan Koeksal <koeksalr@informatik.uni-freiburg.de>
 Project-URL: Homepage, https://github.com/automl/RNAformer
 Project-URL: Issues, https://github.com/automl/RNAformer/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

### Comparing `rnaformer-1.0.2/README.md` & `rnaformer-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `rnaformer-1.0.2/pyproject.toml` & `rnaformer-1.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
-name = "rnaformer"
-version = "1.0.2"
+name = "RNAformer"
+version = "1.0.3"
 authors = [
   { name="Joerg K.H. Franke", email="frankej@cs.uni-freiburg.de" },
   { name="Frederic Runge"},
   { name="Ryan Koeksal", email="koeksalr@informatik.uni-freiburg.de" },
   { name="Rolf Backofen"},
   { name="Frank Hutter"},
 ]
```

### Comparing `rnaformer-1.0.2/rnaformer.egg-info/PKG-INFO` & `rnaformer-1.0.3/RNAformer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rnaformer
-Version: 1.0.2
+Name: RNAformer
+Version: 1.0.3
 Summary: RNAformer: a simple single-sequence-based deep learning model for RNA secondary structure prediction.
 Author: Frederic Runge, Rolf Backofen, Frank Hutter
 Author-email: "Joerg K.H. Franke" <frankej@cs.uni-freiburg.de>, Ryan Koeksal <koeksalr@informatik.uni-freiburg.de>
 Project-URL: Homepage, https://github.com/automl/RNAformer
 Project-URL: Issues, https://github.com/automl/RNAformer/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

