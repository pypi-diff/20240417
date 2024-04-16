# Comparing `tmp/PyGRF-0.0.2.tar.gz` & `tmp/PyGRF-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGRF-0.0.2.tar", last modified: Tue Apr 16 18:40:31 2024, max compression
+gzip compressed data, was "PyGRF-0.0.3.tar", last modified: Tue Apr 16 21:59:41 2024, max compression
```

## Comparing `PyGRF-0.0.2.tar` & `PyGRF-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 18:40:31.931265 PyGRF-0.0.2/
--rw-rw-rw-   0        0        0     1088 2024-03-16 20:45:00.000000 PyGRF-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2171 2024-04-16 18:40:31.931265 PyGRF-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-16 18:40:31.895526 PyGRF-0.0.2/PyGRF/
--rw-rw-rw-   0        0        0    22907 2024-04-16 14:02:33.000000 PyGRF-0.0.2/PyGRF/PyGRF.py
--rw-rw-rw-   0        0        0      105 2024-03-17 01:02:06.000000 PyGRF-0.0.2/PyGRF/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 18:40:31.931265 PyGRF-0.0.2/PyGRF.egg-info/
--rw-rw-rw-   0        0        0     2171 2024-04-16 18:40:31.000000 PyGRF-0.0.2/PyGRF.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2024-04-16 18:40:31.000000 PyGRF-0.0.2/PyGRF.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 18:40:31.000000 PyGRF-0.0.2/PyGRF.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-04-16 18:40:31.000000 PyGRF-0.0.2/PyGRF.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-16 18:40:31.000000 PyGRF-0.0.2/PyGRF.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1278 2024-04-16 14:34:06.000000 PyGRF-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-16 18:40:31.931265 PyGRF-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2993 2024-04-16 18:40:09.000000 PyGRF-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 21:59:41.215407 PyGRF-0.0.3/
+-rw-rw-rw-   0        0        0     1088 2024-03-16 20:45:00.000000 PyGRF-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2171 2024-04-16 21:59:41.215407 PyGRF-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-16 21:59:41.199385 PyGRF-0.0.3/PyGRF/
+-rw-rw-rw-   0        0        0    22910 2024-04-16 21:55:56.000000 PyGRF-0.0.3/PyGRF/PyGRF.py
+-rw-rw-rw-   0        0        0      105 2024-03-17 01:02:06.000000 PyGRF-0.0.3/PyGRF/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 21:59:41.215407 PyGRF-0.0.3/PyGRF.egg-info/
+-rw-rw-rw-   0        0        0     2171 2024-04-16 21:59:41.000000 PyGRF-0.0.3/PyGRF.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2024-04-16 21:59:41.000000 PyGRF-0.0.3/PyGRF.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 21:59:41.000000 PyGRF-0.0.3/PyGRF.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-16 21:59:41.000000 PyGRF-0.0.3/PyGRF.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-16 21:59:41.000000 PyGRF-0.0.3/PyGRF.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1278 2024-04-16 14:34:06.000000 PyGRF-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-16 21:59:41.215407 PyGRF-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2993 2024-04-16 21:59:28.000000 PyGRF-0.0.3/setup.py
```

### Comparing `PyGRF-0.0.2/LICENSE` & `PyGRF-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyGRF-0.0.2/PKG-INFO` & `PyGRF-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyGRF
-Version: 0.0.2
+Version: 0.0.3
 Summary: PyGRF: An improved Python Geographical Random Forest model.
 Home-page: https://github.com/geoai-lab/PyGRF
 Author: Kai Sun, Ryan Zhenqi Zhou, Jiyeon Kim, and Yingjie Hu
 Author-email: ksun4@buffalo.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `PyGRF-0.0.2/PyGRF/PyGRF.py` & `PyGRF-0.0.3/PyGRF/PyGRF.py`

 * *Files 0% similar despite different names*

```diff
@@ -336,15 +336,15 @@
     # compute the default values for bw_min and bw_max
     if bw_min is None:
         bw_min = 1
     if bw_max is None:
         bw_max = len(y)
 
     # build the k-d tree using spatial coordinates of data records
-    coords['coordinate'] = coords.apply(lambda row: tuple(row), axis=1)
+    coords[:, 'coordinate'] = coords.apply(lambda row: tuple(row), axis=1)
     kd = libpysal.cg.KDTree(np.array(coords['coordinate'].tolist()))
 
     # create lists for saving the ISA result
     bandwidth_list, moran_I_list, z_score_list, p_value_list = [], [], [], []
 
     # compute the moran's I, z-score, and p_value using the sequence of bandwidths
     for current_bw in range(bw_min, bw_max, step):
```

### Comparing `PyGRF-0.0.2/PyGRF.egg-info/PKG-INFO` & `PyGRF-0.0.3/PyGRF.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyGRF
-Version: 0.0.2
+Version: 0.0.3
 Summary: PyGRF: An improved Python Geographical Random Forest model.
 Home-page: https://github.com/geoai-lab/PyGRF
 Author: Kai Sun, Ryan Zhenqi Zhou, Jiyeon Kim, and Yingjie Hu
 Author-email: ksun4@buffalo.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `PyGRF-0.0.2/README.md` & `PyGRF-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `PyGRF-0.0.2/setup.py` & `PyGRF-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Package meta-data.
 NAME = 'PyGRF'
 DESCRIPTION = 'PyGRF: An improved Python Geographical Random Forest model.'
 URL = 'https://github.com/geoai-lab/PyGRF'
 EMAIL = 'ksun4@buffalo.edu'
 AUTHOR = 'Kai Sun, Ryan Zhenqi Zhou, Jiyeon Kim, and Yingjie Hu'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 
 # Packages are required for this module to be executed.
 REQUIRED = [
     'pandas', 'numpy', 'scikit-learn', 'scipy', 'libpysal', 'esda'
 ]
 
 here = os.path.abspath(os.path.dirname(__file__))
```

