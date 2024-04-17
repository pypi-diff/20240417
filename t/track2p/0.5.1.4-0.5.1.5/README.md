# Comparing `tmp/track2p-0.5.1.4.tar.gz` & `tmp/track2p-0.5.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "track2p-0.5.1.4.tar", last modified: Wed Apr 17 14:19:39 2024, max compression
+gzip compressed data, was "track2p-0.5.1.5.tar", last modified: Wed Apr 17 14:32:47 2024, max compression
```

## Comparing `track2p-0.5.1.4.tar` & `track2p-0.5.1.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 14:19:39.745749 track2p-0.5.1.4/
--rw-r--r--   0 manonmantez   (501) staff       (20)    35149 2024-02-12 15:58:33.000000 track2p-0.5.1.4/LICENSE
--rw-r--r--   0 manonmantez   (501) staff       (20)     5075 2024-04-17 14:19:39.745396 track2p-0.5.1.4/PKG-INFO
--rw-r--r--   0 manonmantez   (501) staff       (20)     4646 2024-04-16 14:56:02.000000 track2p-0.5.1.4/README.md
--rw-r--r--   0 manonmantez   (501) staff       (20)       38 2024-04-17 14:19:39.745811 track2p-0.5.1.4/setup.cfg
--rw-r--r--   0 manonmantez   (501) staff       (20)      593 2024-04-17 14:19:38.000000 track2p-0.5.1.4/setup.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 14:19:39.735471 track2p-0.5.1.4/track2p/
--rw-r--r--   0 manonmantez   (501) staff       (20)       48 2024-02-22 09:56:18.000000 track2p-0.5.1.4/track2p/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      417 2024-02-21 12:46:39.000000 track2p-0.5.1.4/track2p/__main__.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 14:19:39.739659 track2p-0.5.1.4/track2p/gui/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.4/track2p/gui/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     8413 2024-04-16 14:56:02.000000 track2p-0.5.1.4/track2p/gui/cell_plot.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     6456 2024-04-16 14:56:02.000000 track2p-0.5.1.4/track2p/gui/fluo_plot.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     2622 2024-04-16 14:56:02.000000 track2p-0.5.1.4/track2p/gui/import_wd.py
--rw-r--r--   0 manonmantez   (501) staff       (20)    22751 2024-04-16 14:56:02.000000 track2p-0.5.1.4/track2p/gui/main_wd.py
--rw-r--r--   0 manonmantez   (501) staff       (20)    15418 2024-04-16 14:56:02.000000 track2p-0.5.1.4/track2p/gui/raster_wd.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     8677 2024-04-16 14:56:02.000000 track2p-0.5.1.4/track2p/gui/roi_plot.py
--rw-r--r--   0 manonmantez   (501) staff       (20)    10842 2024-04-17 13:16:13.000000 track2p-0.5.1.4/track2p/gui/t2p_wd.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 14:19:39.741183 track2p-0.5.1.4/track2p/io/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.4/track2p/io/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     1726 2024-04-16 14:56:02.000000 track2p-0.5.1.4/track2p/io/loaders.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     4238 2024-04-16 14:56:02.000000 track2p-0.5.1.4/track2p/io/s2p_loaders.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      773 2024-02-12 11:04:52.000000 track2p-0.5.1.4/track2p/io/savers.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      252 2024-01-09 12:56:24.000000 track2p-0.5.1.4/track2p/io/utils.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 14:19:39.742072 track2p-0.5.1.4/track2p/match/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.4/track2p/match/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     4471 2024-01-09 12:56:24.000000 track2p-0.5.1.4/track2p/match/loop.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     5807 2024-04-16 14:56:02.000000 track2p-0.5.1.4/track2p/match/utils.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 14:19:39.742538 track2p-0.5.1.4/track2p/ops/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.4/track2p/ops/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     3470 2024-04-17 13:25:55.000000 track2p-0.5.1.4/track2p/ops/default.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 14:19:39.743704 track2p-0.5.1.4/track2p/plot/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.4/track2p/plot/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)    15443 2024-04-16 14:56:02.000000 track2p-0.5.1.4/track2p/plot/output.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      990 2024-04-17 14:17:24.000000 track2p-0.5.1.4/track2p/plot/progress.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     1905 2024-04-17 14:17:21.000000 track2p-0.5.1.4/track2p/plot/utils.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 14:19:39.744837 track2p-0.5.1.4/track2p/register/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.4/track2p/register/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     1348 2024-01-10 11:16:47.000000 track2p-0.5.1.4/track2p/register/elastix.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     4054 2024-01-09 12:56:24.000000 track2p-0.5.1.4/track2p/register/loop.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     2345 2024-01-09 12:56:24.000000 track2p-0.5.1.4/track2p/register/utils.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     9791 2024-04-17 14:17:29.000000 track2p-0.5.1.4/track2p/t2p.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 14:19:39.736500 track2p-0.5.1.4/track2p.egg-info/
--rw-r--r--   0 manonmantez   (501) staff       (20)     5075 2024-04-17 14:19:39.000000 track2p-0.5.1.4/track2p.egg-info/PKG-INFO
--rw-r--r--   0 manonmantez   (501) staff       (20)      861 2024-04-17 14:19:39.000000 track2p-0.5.1.4/track2p.egg-info/SOURCES.txt
--rw-r--r--   0 manonmantez   (501) staff       (20)        1 2024-04-17 14:19:39.000000 track2p-0.5.1.4/track2p.egg-info/dependency_links.txt
--rw-r--r--   0 manonmantez   (501) staff       (20)      163 2024-04-17 14:19:39.000000 track2p-0.5.1.4/track2p.egg-info/requires.txt
--rw-r--r--   0 manonmantez   (501) staff       (20)        8 2024-04-17 14:19:39.000000 track2p-0.5.1.4/track2p.egg-info/top_level.txt
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 14:32:47.632754 track2p-0.5.1.5/
+-rw-r--r--   0 manonmantez   (501) staff       (20)    35149 2024-02-12 15:58:33.000000 track2p-0.5.1.5/LICENSE
+-rw-r--r--   0 manonmantez   (501) staff       (20)     5075 2024-04-17 14:32:47.632393 track2p-0.5.1.5/PKG-INFO
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4646 2024-04-16 14:56:02.000000 track2p-0.5.1.5/README.md
+-rw-r--r--   0 manonmantez   (501) staff       (20)       38 2024-04-17 14:32:47.632824 track2p-0.5.1.5/setup.cfg
+-rw-r--r--   0 manonmantez   (501) staff       (20)      593 2024-04-17 14:32:12.000000 track2p-0.5.1.5/setup.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 14:32:47.622769 track2p-0.5.1.5/track2p/
+-rw-r--r--   0 manonmantez   (501) staff       (20)       48 2024-02-22 09:56:18.000000 track2p-0.5.1.5/track2p/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)      417 2024-02-21 12:46:39.000000 track2p-0.5.1.5/track2p/__main__.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 14:32:47.627024 track2p-0.5.1.5/track2p/gui/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.5/track2p/gui/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     8413 2024-04-16 14:56:02.000000 track2p-0.5.1.5/track2p/gui/cell_plot.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     6456 2024-04-16 14:56:02.000000 track2p-0.5.1.5/track2p/gui/fluo_plot.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     2622 2024-04-16 14:56:02.000000 track2p-0.5.1.5/track2p/gui/import_wd.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    22751 2024-04-16 14:56:02.000000 track2p-0.5.1.5/track2p/gui/main_wd.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    15418 2024-04-16 14:56:02.000000 track2p-0.5.1.5/track2p/gui/raster_wd.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     8677 2024-04-16 14:56:02.000000 track2p-0.5.1.5/track2p/gui/roi_plot.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    10842 2024-04-17 13:16:13.000000 track2p-0.5.1.5/track2p/gui/t2p_wd.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 14:32:47.628419 track2p-0.5.1.5/track2p/io/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.5/track2p/io/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     1726 2024-04-16 14:56:02.000000 track2p-0.5.1.5/track2p/io/loaders.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4238 2024-04-16 14:56:02.000000 track2p-0.5.1.5/track2p/io/s2p_loaders.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)      773 2024-02-12 11:04:52.000000 track2p-0.5.1.5/track2p/io/savers.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)      252 2024-01-09 12:56:24.000000 track2p-0.5.1.5/track2p/io/utils.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 14:32:47.629279 track2p-0.5.1.5/track2p/match/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.5/track2p/match/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4471 2024-01-09 12:56:24.000000 track2p-0.5.1.5/track2p/match/loop.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     5807 2024-04-16 14:56:02.000000 track2p-0.5.1.5/track2p/match/utils.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 14:32:47.629780 track2p-0.5.1.5/track2p/ops/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.5/track2p/ops/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     3470 2024-04-17 13:25:55.000000 track2p-0.5.1.5/track2p/ops/default.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 14:32:47.630887 track2p-0.5.1.5/track2p/plot/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.5/track2p/plot/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    15443 2024-04-16 14:56:02.000000 track2p-0.5.1.5/track2p/plot/output.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     1008 2024-04-17 14:31:55.000000 track2p-0.5.1.5/track2p/plot/progress.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     1905 2024-04-17 14:32:00.000000 track2p-0.5.1.5/track2p/plot/utils.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 14:32:47.631908 track2p-0.5.1.5/track2p/register/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.5/track2p/register/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     1348 2024-01-10 11:16:47.000000 track2p-0.5.1.5/track2p/register/elastix.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4054 2024-01-09 12:56:24.000000 track2p-0.5.1.5/track2p/register/loop.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     2391 2024-04-17 14:32:03.000000 track2p-0.5.1.5/track2p/register/utils.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     9791 2024-04-17 14:17:29.000000 track2p-0.5.1.5/track2p/t2p.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 14:32:47.623815 track2p-0.5.1.5/track2p.egg-info/
+-rw-r--r--   0 manonmantez   (501) staff       (20)     5075 2024-04-17 14:32:47.000000 track2p-0.5.1.5/track2p.egg-info/PKG-INFO
+-rw-r--r--   0 manonmantez   (501) staff       (20)      861 2024-04-17 14:32:47.000000 track2p-0.5.1.5/track2p.egg-info/SOURCES.txt
+-rw-r--r--   0 manonmantez   (501) staff       (20)        1 2024-04-17 14:32:47.000000 track2p-0.5.1.5/track2p.egg-info/dependency_links.txt
+-rw-r--r--   0 manonmantez   (501) staff       (20)      163 2024-04-17 14:32:47.000000 track2p-0.5.1.5/track2p.egg-info/requires.txt
+-rw-r--r--   0 manonmantez   (501) staff       (20)        8 2024-04-17 14:32:47.000000 track2p-0.5.1.5/track2p.egg-info/top_level.txt
```

### Comparing `track2p-0.5.1.4/LICENSE` & `track2p-0.5.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.4/PKG-INFO` & `track2p-0.5.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: track2p
-Version: 0.5.1.4
+Version: 0.5.1.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.23.5
 Requires-Dist: matplotlib==3.5.3
 Requires-Dist: scikit-image==0.20.0
 Requires-Dist: itk-elastix==0.19.1
 Requires-Dist: PyQt5==5.15.10
```

### Comparing `track2p-0.5.1.4/README.md` & `track2p-0.5.1.5/README.md`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.4/setup.py` & `track2p-0.5.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='track2p',
-    version='0.5.1.4',
+    version='0.5.1.5',
     packages=find_packages(),
     install_requires=[
         'numpy==1.23.5',
         'matplotlib==3.5.3',
         'scikit-image==0.20.0',
         'itk-elastix==0.19.1',
         'PyQt5==5.15.10',
```

### Comparing `track2p-0.5.1.4/track2p/gui/cell_plot.py` & `track2p-0.5.1.5/track2p/gui/cell_plot.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.4/track2p/gui/fluo_plot.py` & `track2p-0.5.1.5/track2p/gui/fluo_plot.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.4/track2p/gui/import_wd.py` & `track2p-0.5.1.5/track2p/gui/import_wd.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.4/track2p/gui/main_wd.py` & `track2p-0.5.1.5/track2p/gui/main_wd.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.4/track2p/gui/raster_wd.py` & `track2p-0.5.1.5/track2p/gui/raster_wd.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.4/track2p/gui/roi_plot.py` & `track2p-0.5.1.5/track2p/gui/roi_plot.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.4/track2p/gui/t2p_wd.py` & `track2p-0.5.1.5/track2p/gui/t2p_wd.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.4/track2p/io/loaders.py` & `track2p-0.5.1.5/track2p/io/loaders.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.4/track2p/io/s2p_loaders.py` & `track2p-0.5.1.5/track2p/io/s2p_loaders.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.4/track2p/io/savers.py` & `track2p-0.5.1.5/track2p/io/savers.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.4/track2p/match/loop.py` & `track2p-0.5.1.5/track2p/match/loop.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.4/track2p/match/utils.py` & `track2p-0.5.1.5/track2p/match/utils.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.4/track2p/ops/default.py` & `track2p-0.5.1.5/track2p/ops/default.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.4/track2p/plot/output.py` & `track2p-0.5.1.5/track2p/plot/output.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.4/track2p/plot/progress.py` & `track2p-0.5.1.5/track2p/plot/progress.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,9 +20,10 @@
         for j in range(len(track_ops.all_ds_path)):
             img = all_ds_avg_ch_matched[j][i]
             axs[i, j].imshow(img, cmap='gray', vmin=0, vmax=np.percentile(img, sat_perc))
             axs[i, j].set_title('Plane ' + str(i) + ' in dataset ' + str(j))
             axs[i, j].axis('off')
     print("done")
     plt.close(fig)
+    print("done")
```

### Comparing `track2p-0.5.1.4/track2p/plot/utils.py` & `track2p-0.5.1.5/track2p/plot/utils.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.4/track2p/register/elastix.py` & `track2p-0.5.1.5/track2p/register/elastix.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.4/track2p/register/loop.py` & `track2p-0.5.1.5/track2p/register/loop.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.4/track2p/register/utils.py` & `track2p-0.5.1.5/track2p/register/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 
 def get_all_ds_img_for_reg(all_ds_avg_ch1, all_ds_avg_ch2, track_ops): # chooses which channel to use for registration and returns all_ref_img and all_mov_img (shifted by one day to always register to previous day)
+    print("starting get_all_ds_img_for_reg ")
     if track_ops.reg_chan==0:
         all_ds_avg = all_ds_avg_ch1
     elif track_ops.reg_chan==1:
         all_ds_avg = all_ds_avg_ch2
         print('WARNING: using anatomical channel for registration (this is not always available)')
 
     all_ds_ref_img = []
```

### Comparing `track2p-0.5.1.4/track2p/t2p.py` & `track2p-0.5.1.5/track2p/t2p.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.4/track2p.egg-info/PKG-INFO` & `track2p-0.5.1.5/track2p.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: track2p
-Version: 0.5.1.4
+Version: 0.5.1.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.23.5
 Requires-Dist: matplotlib==3.5.3
 Requires-Dist: scikit-image==0.20.0
 Requires-Dist: itk-elastix==0.19.1
 Requires-Dist: PyQt5==5.15.10
```

### Comparing `track2p-0.5.1.4/track2p.egg-info/SOURCES.txt` & `track2p-0.5.1.5/track2p.egg-info/SOURCES.txt`

 * *Files identical despite different names*

