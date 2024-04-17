# Comparing `tmp/binarize2pcalcium-0.1.8.tar.gz` & `tmp/binarize2pcalcium-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/binarize2pcalcium-0.1.8.tar", last modified: Wed Nov 15 10:09:08 2023, max compression
+gzip compressed data, was "binarize2pcalcium-0.1.9.tar", last modified: Wed Nov 15 10:16:33 2023, max compression
```

## Comparing `binarize2pcalcium-0.1.8.tar` & `binarize2pcalcium-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 cat       (1000) cat       (1000)        0 2023-11-15 10:09:08.535449 binarize2pcalcium-0.1.8/
--rw-rw-r--   0 cat       (1000) cat       (1000)     1063 2023-11-15 08:53:09.000000 binarize2pcalcium-0.1.8/LICENSE
--rw-rw-r--   0 cat       (1000) cat       (1000)     1801 2023-11-15 10:09:08.535449 binarize2pcalcium-0.1.8/PKG-INFO
--rw-rw-r--   0 cat       (1000) cat       (1000)     1344 2023-11-15 09:49:51.000000 binarize2pcalcium-0.1.8/README.md
-drwxrwxr-x   0 cat       (1000) cat       (1000)        0 2023-11-15 10:09:08.531449 binarize2pcalcium-0.1.8/binarize2pcalcium/
--rw-rw-r--   0 cat       (1000) cat       (1000)        0 2021-10-07 14:51:11.000000 binarize2pcalcium-0.1.8/binarize2pcalcium/__init__.py
--rw-rw-r--   0 cat       (1000) cat       (1000)   141148 2023-11-15 06:55:51.000000 binarize2pcalcium-0.1.8/binarize2pcalcium/binarize2pcalcium.py
-drwxrwxr-x   0 cat       (1000) cat       (1000)        0 2023-11-15 10:09:08.535449 binarize2pcalcium-0.1.8/binarize2pcalcium.egg-info/
--rw-rw-r--   0 cat       (1000) cat       (1000)     1801 2023-11-15 10:09:08.000000 binarize2pcalcium-0.1.8/binarize2pcalcium.egg-info/PKG-INFO
--rw-rw-r--   0 cat       (1000) cat       (1000)      299 2023-11-15 10:09:08.000000 binarize2pcalcium-0.1.8/binarize2pcalcium.egg-info/SOURCES.txt
--rw-rw-r--   0 cat       (1000) cat       (1000)        1 2023-11-15 10:09:08.000000 binarize2pcalcium-0.1.8/binarize2pcalcium.egg-info/dependency_links.txt
--rw-rw-r--   0 cat       (1000) cat       (1000)       85 2023-11-15 10:09:08.000000 binarize2pcalcium-0.1.8/binarize2pcalcium.egg-info/requires.txt
--rw-rw-r--   0 cat       (1000) cat       (1000)       18 2023-11-15 10:09:08.000000 binarize2pcalcium-0.1.8/binarize2pcalcium.egg-info/top_level.txt
--rw-rw-r--   0 cat       (1000) cat       (1000)       38 2023-11-15 10:09:08.535449 binarize2pcalcium-0.1.8/setup.cfg
--rw-rw-r--   0 cat       (1000) cat       (1000)     2107 2023-11-15 10:09:00.000000 binarize2pcalcium-0.1.8/setup.py
+drwxrwxr-x   0 cat       (1000) cat       (1000)        0 2023-11-15 10:16:33.725621 binarize2pcalcium-0.1.9/
+-rw-rw-r--   0 cat       (1000) cat       (1000)     1063 2023-11-15 08:53:09.000000 binarize2pcalcium-0.1.9/LICENSE
+-rw-rw-r--   0 cat       (1000) cat       (1000)     1801 2023-11-15 10:16:33.725621 binarize2pcalcium-0.1.9/PKG-INFO
+-rw-rw-r--   0 cat       (1000) cat       (1000)     1344 2023-11-15 09:49:51.000000 binarize2pcalcium-0.1.9/README.md
+drwxrwxr-x   0 cat       (1000) cat       (1000)        0 2023-11-15 10:16:33.725621 binarize2pcalcium-0.1.9/binarize2pcalcium/
+-rw-rw-r--   0 cat       (1000) cat       (1000)        0 2021-10-07 14:51:11.000000 binarize2pcalcium-0.1.9/binarize2pcalcium/__init__.py
+-rw-rw-r--   0 cat       (1000) cat       (1000)   140921 2023-11-15 10:15:20.000000 binarize2pcalcium-0.1.9/binarize2pcalcium/binarize2pcalcium.py
+drwxrwxr-x   0 cat       (1000) cat       (1000)        0 2023-11-15 10:16:33.725621 binarize2pcalcium-0.1.9/binarize2pcalcium.egg-info/
+-rw-rw-r--   0 cat       (1000) cat       (1000)     1801 2023-11-15 10:16:33.000000 binarize2pcalcium-0.1.9/binarize2pcalcium.egg-info/PKG-INFO
+-rw-rw-r--   0 cat       (1000) cat       (1000)      299 2023-11-15 10:16:33.000000 binarize2pcalcium-0.1.9/binarize2pcalcium.egg-info/SOURCES.txt
+-rw-rw-r--   0 cat       (1000) cat       (1000)        1 2023-11-15 10:16:33.000000 binarize2pcalcium-0.1.9/binarize2pcalcium.egg-info/dependency_links.txt
+-rw-rw-r--   0 cat       (1000) cat       (1000)       85 2023-11-15 10:16:33.000000 binarize2pcalcium-0.1.9/binarize2pcalcium.egg-info/requires.txt
+-rw-rw-r--   0 cat       (1000) cat       (1000)       18 2023-11-15 10:16:33.000000 binarize2pcalcium-0.1.9/binarize2pcalcium.egg-info/top_level.txt
+-rw-rw-r--   0 cat       (1000) cat       (1000)       38 2023-11-15 10:16:33.725621 binarize2pcalcium-0.1.9/setup.cfg
+-rw-rw-r--   0 cat       (1000) cat       (1000)     2107 2023-11-15 10:16:16.000000 binarize2pcalcium-0.1.9/setup.py
```

### Comparing `binarize2pcalcium-0.1.8/LICENSE` & `binarize2pcalcium-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `binarize2pcalcium-0.1.8/PKG-INFO` & `binarize2pcalcium-0.1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binarize2pcalcium
-Version: 0.1.8
+Version: 0.1.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 	Binarize2PCalcium
 	=================
```

### Comparing `binarize2pcalcium-0.1.8/README.md` & `binarize2pcalcium-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `binarize2pcalcium-0.1.8/binarize2pcalcium/binarize2pcalcium.py` & `binarize2pcalcium-0.1.9/binarize2pcalcium/binarize2pcalcium.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,35 +22,24 @@
 from sklearn import datasets, linear_model
 from scipy import stats
 
 import sys
 module_path = os.path.abspath(os.path.join('..'))
 sys.path.append(module_path)
 
-try:
-    from utils.wheel import wheel
-except:
-    from manifolds.donlabtools.utils.wheel import wheel
 #from utils.calcium import calcium
 #from utils.animal_database import animal_database
 from statistics import NormalDist#, mode
 from scipy.stats import mode
 
 from sklearn import metrics
 from sklearn import datasets, linear_model
 from sklearn.metrics import mean_squared_error, r2_score
 
 
-import sys
-module_path = os.path.abspath(os.path.join('..'))
-sys.path.append(module_path)
-
-#from utils.wheel import wheel
-
-
 #
 def butter_highpass(cutoff, fs, order=5):
     nyq = 0.5 * fs
     normal_cutoff = cutoff / nyq
     b, a = butter(order, normal_cutoff, btype='high', analog=False)
     return b, a
```

### Comparing `binarize2pcalcium-0.1.8/binarize2pcalcium.egg-info/PKG-INFO` & `binarize2pcalcium-0.1.9/binarize2pcalcium.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binarize2pcalcium
-Version: 0.1.8
+Version: 0.1.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 	Binarize2PCalcium
 	=================
```

### Comparing `binarize2pcalcium-0.1.8/setup.py` & `binarize2pcalcium-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='binarize2pcalcium',
-    version='0.1.8',
+    version='0.1.9',
     packages=['binarize2pcalcium'],
     install_requires=[
         'numpy',
         'tqdm',
         'scipy',
         'matplotlib',
         'pyyaml',
```

