# Comparing `tmp/track2p-0.5.1.3.tar.gz` & `tmp/track2p-0.5.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "track2p-0.5.1.3.tar", last modified: Wed Apr 17 13:28:02 2024, max compression
+gzip compressed data, was "track2p-0.5.1.4.tar", last modified: Wed Apr 17 14:19:39 2024, max compression
```

## Comparing `track2p-0.5.1.3.tar` & `track2p-0.5.1.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 13:28:02.566491 track2p-0.5.1.3/
--rw-r--r--   0 manonmantez   (501) staff       (20)    35149 2024-02-12 15:58:33.000000 track2p-0.5.1.3/LICENSE
--rw-r--r--   0 manonmantez   (501) staff       (20)     5075 2024-04-17 13:28:02.566105 track2p-0.5.1.3/PKG-INFO
--rw-r--r--   0 manonmantez   (501) staff       (20)     4646 2024-04-16 14:56:02.000000 track2p-0.5.1.3/README.md
--rw-r--r--   0 manonmantez   (501) staff       (20)       38 2024-04-17 13:28:02.566565 track2p-0.5.1.3/setup.cfg
--rw-r--r--   0 manonmantez   (501) staff       (20)      593 2024-04-17 13:27:56.000000 track2p-0.5.1.3/setup.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 13:28:02.556210 track2p-0.5.1.3/track2p/
--rw-r--r--   0 manonmantez   (501) staff       (20)       48 2024-02-22 09:56:18.000000 track2p-0.5.1.3/track2p/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      417 2024-02-21 12:46:39.000000 track2p-0.5.1.3/track2p/__main__.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 13:28:02.560413 track2p-0.5.1.3/track2p/gui/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.3/track2p/gui/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     8413 2024-04-16 14:56:02.000000 track2p-0.5.1.3/track2p/gui/cell_plot.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     6456 2024-04-16 14:56:02.000000 track2p-0.5.1.3/track2p/gui/fluo_plot.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     2622 2024-04-16 14:56:02.000000 track2p-0.5.1.3/track2p/gui/import_wd.py
--rw-r--r--   0 manonmantez   (501) staff       (20)    22751 2024-04-16 14:56:02.000000 track2p-0.5.1.3/track2p/gui/main_wd.py
--rw-r--r--   0 manonmantez   (501) staff       (20)    15418 2024-04-16 14:56:02.000000 track2p-0.5.1.3/track2p/gui/raster_wd.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     8677 2024-04-16 14:56:02.000000 track2p-0.5.1.3/track2p/gui/roi_plot.py
--rw-r--r--   0 manonmantez   (501) staff       (20)    10842 2024-04-17 13:16:13.000000 track2p-0.5.1.3/track2p/gui/t2p_wd.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 13:28:02.561755 track2p-0.5.1.3/track2p/io/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.3/track2p/io/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     1726 2024-04-16 14:56:02.000000 track2p-0.5.1.3/track2p/io/loaders.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     4238 2024-04-16 14:56:02.000000 track2p-0.5.1.3/track2p/io/s2p_loaders.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      773 2024-02-12 11:04:52.000000 track2p-0.5.1.3/track2p/io/savers.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      252 2024-01-09 12:56:24.000000 track2p-0.5.1.3/track2p/io/utils.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 13:28:02.562765 track2p-0.5.1.3/track2p/match/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.3/track2p/match/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     4471 2024-01-09 12:56:24.000000 track2p-0.5.1.3/track2p/match/loop.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     5807 2024-04-16 14:56:02.000000 track2p-0.5.1.3/track2p/match/utils.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 13:28:02.563185 track2p-0.5.1.3/track2p/ops/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.3/track2p/ops/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     3470 2024-04-17 13:25:55.000000 track2p-0.5.1.3/track2p/ops/default.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 13:28:02.564290 track2p-0.5.1.3/track2p/plot/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.3/track2p/plot/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)    15443 2024-04-16 14:56:02.000000 track2p-0.5.1.3/track2p/plot/output.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      926 2024-02-12 11:04:52.000000 track2p-0.5.1.3/track2p/plot/progress.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     1859 2024-02-12 11:04:52.000000 track2p-0.5.1.3/track2p/plot/utils.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 13:28:02.565443 track2p-0.5.1.3/track2p/register/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.3/track2p/register/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     1348 2024-01-10 11:16:47.000000 track2p-0.5.1.3/track2p/register/elastix.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     4054 2024-01-09 12:56:24.000000 track2p-0.5.1.3/track2p/register/loop.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     2345 2024-01-09 12:56:24.000000 track2p-0.5.1.3/track2p/register/utils.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     9791 2024-04-16 14:56:02.000000 track2p-0.5.1.3/track2p/t2p.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 13:28:02.557255 track2p-0.5.1.3/track2p.egg-info/
--rw-r--r--   0 manonmantez   (501) staff       (20)     5075 2024-04-17 13:28:02.000000 track2p-0.5.1.3/track2p.egg-info/PKG-INFO
--rw-r--r--   0 manonmantez   (501) staff       (20)      861 2024-04-17 13:28:02.000000 track2p-0.5.1.3/track2p.egg-info/SOURCES.txt
--rw-r--r--   0 manonmantez   (501) staff       (20)        1 2024-04-17 13:28:02.000000 track2p-0.5.1.3/track2p.egg-info/dependency_links.txt
--rw-r--r--   0 manonmantez   (501) staff       (20)      163 2024-04-17 13:28:02.000000 track2p-0.5.1.3/track2p.egg-info/requires.txt
--rw-r--r--   0 manonmantez   (501) staff       (20)        8 2024-04-17 13:28:02.000000 track2p-0.5.1.3/track2p.egg-info/top_level.txt
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 14:19:39.745749 track2p-0.5.1.4/
+-rw-r--r--   0 manonmantez   (501) staff       (20)    35149 2024-02-12 15:58:33.000000 track2p-0.5.1.4/LICENSE
+-rw-r--r--   0 manonmantez   (501) staff       (20)     5075 2024-04-17 14:19:39.745396 track2p-0.5.1.4/PKG-INFO
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4646 2024-04-16 14:56:02.000000 track2p-0.5.1.4/README.md
+-rw-r--r--   0 manonmantez   (501) staff       (20)       38 2024-04-17 14:19:39.745811 track2p-0.5.1.4/setup.cfg
+-rw-r--r--   0 manonmantez   (501) staff       (20)      593 2024-04-17 14:19:38.000000 track2p-0.5.1.4/setup.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 14:19:39.735471 track2p-0.5.1.4/track2p/
+-rw-r--r--   0 manonmantez   (501) staff       (20)       48 2024-02-22 09:56:18.000000 track2p-0.5.1.4/track2p/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)      417 2024-02-21 12:46:39.000000 track2p-0.5.1.4/track2p/__main__.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 14:19:39.739659 track2p-0.5.1.4/track2p/gui/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.4/track2p/gui/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     8413 2024-04-16 14:56:02.000000 track2p-0.5.1.4/track2p/gui/cell_plot.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     6456 2024-04-16 14:56:02.000000 track2p-0.5.1.4/track2p/gui/fluo_plot.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     2622 2024-04-16 14:56:02.000000 track2p-0.5.1.4/track2p/gui/import_wd.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    22751 2024-04-16 14:56:02.000000 track2p-0.5.1.4/track2p/gui/main_wd.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    15418 2024-04-16 14:56:02.000000 track2p-0.5.1.4/track2p/gui/raster_wd.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     8677 2024-04-16 14:56:02.000000 track2p-0.5.1.4/track2p/gui/roi_plot.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    10842 2024-04-17 13:16:13.000000 track2p-0.5.1.4/track2p/gui/t2p_wd.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 14:19:39.741183 track2p-0.5.1.4/track2p/io/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.4/track2p/io/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     1726 2024-04-16 14:56:02.000000 track2p-0.5.1.4/track2p/io/loaders.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4238 2024-04-16 14:56:02.000000 track2p-0.5.1.4/track2p/io/s2p_loaders.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)      773 2024-02-12 11:04:52.000000 track2p-0.5.1.4/track2p/io/savers.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)      252 2024-01-09 12:56:24.000000 track2p-0.5.1.4/track2p/io/utils.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 14:19:39.742072 track2p-0.5.1.4/track2p/match/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.4/track2p/match/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4471 2024-01-09 12:56:24.000000 track2p-0.5.1.4/track2p/match/loop.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     5807 2024-04-16 14:56:02.000000 track2p-0.5.1.4/track2p/match/utils.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 14:19:39.742538 track2p-0.5.1.4/track2p/ops/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.4/track2p/ops/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     3470 2024-04-17 13:25:55.000000 track2p-0.5.1.4/track2p/ops/default.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 14:19:39.743704 track2p-0.5.1.4/track2p/plot/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.4/track2p/plot/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    15443 2024-04-16 14:56:02.000000 track2p-0.5.1.4/track2p/plot/output.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)      990 2024-04-17 14:17:24.000000 track2p-0.5.1.4/track2p/plot/progress.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     1905 2024-04-17 14:17:21.000000 track2p-0.5.1.4/track2p/plot/utils.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 14:19:39.744837 track2p-0.5.1.4/track2p/register/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.4/track2p/register/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     1348 2024-01-10 11:16:47.000000 track2p-0.5.1.4/track2p/register/elastix.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4054 2024-01-09 12:56:24.000000 track2p-0.5.1.4/track2p/register/loop.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     2345 2024-01-09 12:56:24.000000 track2p-0.5.1.4/track2p/register/utils.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     9791 2024-04-17 14:17:29.000000 track2p-0.5.1.4/track2p/t2p.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 14:19:39.736500 track2p-0.5.1.4/track2p.egg-info/
+-rw-r--r--   0 manonmantez   (501) staff       (20)     5075 2024-04-17 14:19:39.000000 track2p-0.5.1.4/track2p.egg-info/PKG-INFO
+-rw-r--r--   0 manonmantez   (501) staff       (20)      861 2024-04-17 14:19:39.000000 track2p-0.5.1.4/track2p.egg-info/SOURCES.txt
+-rw-r--r--   0 manonmantez   (501) staff       (20)        1 2024-04-17 14:19:39.000000 track2p-0.5.1.4/track2p.egg-info/dependency_links.txt
+-rw-r--r--   0 manonmantez   (501) staff       (20)      163 2024-04-17 14:19:39.000000 track2p-0.5.1.4/track2p.egg-info/requires.txt
+-rw-r--r--   0 manonmantez   (501) staff       (20)        8 2024-04-17 14:19:39.000000 track2p-0.5.1.4/track2p.egg-info/top_level.txt
```

### Comparing `track2p-0.5.1.3/LICENSE` & `track2p-0.5.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.3/PKG-INFO` & `track2p-0.5.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: track2p
-Version: 0.5.1.3
+Version: 0.5.1.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.23.5
 Requires-Dist: matplotlib==3.5.3
 Requires-Dist: scikit-image==0.20.0
 Requires-Dist: itk-elastix==0.19.1
 Requires-Dist: PyQt5==5.15.10
```

### Comparing `track2p-0.5.1.3/README.md` & `track2p-0.5.1.4/README.md`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.3/setup.py` & `track2p-0.5.1.4/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='track2p',
-    version='0.5.1.3',
+    version='0.5.1.4',
     packages=find_packages(),
     install_requires=[
         'numpy==1.23.5',
         'matplotlib==3.5.3',
         'scikit-image==0.20.0',
         'itk-elastix==0.19.1',
         'PyQt5==5.15.10',
```

### Comparing `track2p-0.5.1.3/track2p/gui/cell_plot.py` & `track2p-0.5.1.4/track2p/gui/cell_plot.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.3/track2p/gui/fluo_plot.py` & `track2p-0.5.1.4/track2p/gui/fluo_plot.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.3/track2p/gui/import_wd.py` & `track2p-0.5.1.4/track2p/gui/import_wd.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.3/track2p/gui/main_wd.py` & `track2p-0.5.1.4/track2p/gui/main_wd.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.3/track2p/gui/raster_wd.py` & `track2p-0.5.1.4/track2p/gui/raster_wd.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.3/track2p/gui/roi_plot.py` & `track2p-0.5.1.4/track2p/gui/roi_plot.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.3/track2p/gui/t2p_wd.py` & `track2p-0.5.1.4/track2p/gui/t2p_wd.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.3/track2p/io/loaders.py` & `track2p-0.5.1.4/track2p/io/loaders.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.3/track2p/io/s2p_loaders.py` & `track2p-0.5.1.4/track2p/io/s2p_loaders.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.3/track2p/io/savers.py` & `track2p-0.5.1.4/track2p/io/savers.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.3/track2p/match/loop.py` & `track2p-0.5.1.4/track2p/match/loop.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.3/track2p/match/utils.py` & `track2p-0.5.1.4/track2p/match/utils.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.3/track2p/ops/default.py` & `track2p-0.5.1.4/track2p/ops/default.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.3/track2p/plot/output.py` & `track2p-0.5.1.4/track2p/plot/output.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.3/track2p/plot/progress.py` & `track2p-0.5.1.4/track2p/plot/progress.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 
 import numpy as np
 import matplotlib.pyplot as plt
 
 from track2p.plot.utils import match_hist_all
 
 def plot_all_planes(all_ds_avg_ch, track_ops, sat_perc=99):
+    print("starting")
     nplanes = track_ops.nplanes
     fig, axs = plt.subplots(nplanes, len(track_ops.all_ds_path), figsize=(3 * len(track_ops.all_ds_path), 3 * nplanes), dpi=300)
     # add dummy dimension to axs if only one plane
     if nplanes==1:
         axs = np.expand_dims(axs, axis=0)
-    
+    print("starting match hist all")
     all_ds_avg_ch_matched = match_hist_all(all_ds_avg_ch)
 
 
     for i in range(nplanes):
         for j in range(len(track_ops.all_ds_path)):
             img = all_ds_avg_ch_matched[j][i]
             axs[i, j].imshow(img, cmap='gray', vmin=0, vmax=np.percentile(img, sat_perc))
             axs[i, j].set_title('Plane ' + str(i) + ' in dataset ' + str(j))
             axs[i, j].axis('off')
-            
+    print("done")
     plt.close(fig)
+
```

### Comparing `track2p-0.5.1.3/track2p/plot/utils.py` & `track2p-0.5.1.4/track2p/plot/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 from skimage.exposure import match_histograms
 
 
 def match_hist_all(all_ds_avg_ch):
+    print("starting macth hist all function")
     ref = all_ds_avg_ch[0][0]
     all_ds_avg_ch_matched = []
     for ds_avg_ch in all_ds_avg_ch:
         ds_avg_ch_matched = []
         for i in range(len(ds_avg_ch)):
             ds_avg_ch_matched.append(match_histograms(ds_avg_ch[i], ref))
         all_ds_avg_ch_matched.append(ds_avg_ch_matched)
```

### Comparing `track2p-0.5.1.3/track2p/register/elastix.py` & `track2p-0.5.1.4/track2p/register/elastix.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.3/track2p/register/loop.py` & `track2p-0.5.1.4/track2p/register/loop.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.3/track2p/register/utils.py` & `track2p-0.5.1.4/track2p/register/utils.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.3/track2p/t2p.py` & `track2p-0.5.1.4/track2p/t2p.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.3/track2p.egg-info/PKG-INFO` & `track2p-0.5.1.4/track2p.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: track2p
-Version: 0.5.1.3
+Version: 0.5.1.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.23.5
 Requires-Dist: matplotlib==3.5.3
 Requires-Dist: scikit-image==0.20.0
 Requires-Dist: itk-elastix==0.19.1
 Requires-Dist: PyQt5==5.15.10
```

### Comparing `track2p-0.5.1.3/track2p.egg-info/SOURCES.txt` & `track2p-0.5.1.4/track2p.egg-info/SOURCES.txt`

 * *Files identical despite different names*

