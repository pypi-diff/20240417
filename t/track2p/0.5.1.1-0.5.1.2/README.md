# Comparing `tmp/track2p-0.5.1.1.tar.gz` & `tmp/track2p-0.5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "track2p-0.5.1.1.tar", last modified: Wed Apr 17 12:55:59 2024, max compression
+gzip compressed data, was "track2p-0.5.1.2.tar", last modified: Wed Apr 17 13:17:22 2024, max compression
```

## Comparing `track2p-0.5.1.1.tar` & `track2p-0.5.1.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 12:55:59.051789 track2p-0.5.1.1/
--rw-r--r--   0 manonmantez   (501) staff       (20)    35149 2024-02-12 15:58:33.000000 track2p-0.5.1.1/LICENSE
--rw-r--r--   0 manonmantez   (501) staff       (20)     5075 2024-04-17 12:55:59.051430 track2p-0.5.1.1/PKG-INFO
--rw-r--r--   0 manonmantez   (501) staff       (20)     4646 2024-04-16 14:56:02.000000 track2p-0.5.1.1/README.md
--rw-r--r--   0 manonmantez   (501) staff       (20)       38 2024-04-17 12:55:59.051864 track2p-0.5.1.1/setup.cfg
--rw-r--r--   0 manonmantez   (501) staff       (20)      593 2024-04-17 12:55:32.000000 track2p-0.5.1.1/setup.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 12:55:59.041689 track2p-0.5.1.1/track2p/
--rw-r--r--   0 manonmantez   (501) staff       (20)       48 2024-02-22 09:56:18.000000 track2p-0.5.1.1/track2p/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      417 2024-02-21 12:46:39.000000 track2p-0.5.1.1/track2p/__main__.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 12:55:59.045958 track2p-0.5.1.1/track2p/gui/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.1/track2p/gui/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     8413 2024-04-16 14:56:02.000000 track2p-0.5.1.1/track2p/gui/cell_plot.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     6456 2024-04-16 14:56:02.000000 track2p-0.5.1.1/track2p/gui/fluo_plot.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     2622 2024-04-16 14:56:02.000000 track2p-0.5.1.1/track2p/gui/import_wd.py
--rw-r--r--   0 manonmantez   (501) staff       (20)    22751 2024-04-16 14:56:02.000000 track2p-0.5.1.1/track2p/gui/main_wd.py
--rw-r--r--   0 manonmantez   (501) staff       (20)    15418 2024-04-16 14:56:02.000000 track2p-0.5.1.1/track2p/gui/raster_wd.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     8677 2024-04-16 14:56:02.000000 track2p-0.5.1.1/track2p/gui/roi_plot.py
--rw-r--r--   0 manonmantez   (501) staff       (20)    10661 2024-04-17 12:49:47.000000 track2p-0.5.1.1/track2p/gui/t2p_wd.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 12:55:59.047324 track2p-0.5.1.1/track2p/io/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.1/track2p/io/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     1726 2024-04-16 14:56:02.000000 track2p-0.5.1.1/track2p/io/loaders.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     4238 2024-04-16 14:56:02.000000 track2p-0.5.1.1/track2p/io/s2p_loaders.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      773 2024-02-12 11:04:52.000000 track2p-0.5.1.1/track2p/io/savers.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      252 2024-01-09 12:56:24.000000 track2p-0.5.1.1/track2p/io/utils.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 12:55:59.048272 track2p-0.5.1.1/track2p/match/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.1/track2p/match/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     4471 2024-01-09 12:56:24.000000 track2p-0.5.1.1/track2p/match/loop.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     5807 2024-04-16 14:56:02.000000 track2p-0.5.1.1/track2p/match/utils.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 12:55:59.048694 track2p-0.5.1.1/track2p/ops/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.1/track2p/ops/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     3348 2024-04-16 14:56:02.000000 track2p-0.5.1.1/track2p/ops/default.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 12:55:59.049689 track2p-0.5.1.1/track2p/plot/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.1/track2p/plot/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)    15443 2024-04-16 14:56:02.000000 track2p-0.5.1.1/track2p/plot/output.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      926 2024-02-12 11:04:52.000000 track2p-0.5.1.1/track2p/plot/progress.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     1859 2024-02-12 11:04:52.000000 track2p-0.5.1.1/track2p/plot/utils.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 12:55:59.050841 track2p-0.5.1.1/track2p/register/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.1/track2p/register/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     1348 2024-01-10 11:16:47.000000 track2p-0.5.1.1/track2p/register/elastix.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     4054 2024-01-09 12:56:24.000000 track2p-0.5.1.1/track2p/register/loop.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     2345 2024-01-09 12:56:24.000000 track2p-0.5.1.1/track2p/register/utils.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     9791 2024-04-16 14:56:02.000000 track2p-0.5.1.1/track2p/t2p.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 12:55:59.042881 track2p-0.5.1.1/track2p.egg-info/
--rw-r--r--   0 manonmantez   (501) staff       (20)     5075 2024-04-17 12:55:58.000000 track2p-0.5.1.1/track2p.egg-info/PKG-INFO
--rw-r--r--   0 manonmantez   (501) staff       (20)      861 2024-04-17 12:55:58.000000 track2p-0.5.1.1/track2p.egg-info/SOURCES.txt
--rw-r--r--   0 manonmantez   (501) staff       (20)        1 2024-04-17 12:55:58.000000 track2p-0.5.1.1/track2p.egg-info/dependency_links.txt
--rw-r--r--   0 manonmantez   (501) staff       (20)      163 2024-04-17 12:55:58.000000 track2p-0.5.1.1/track2p.egg-info/requires.txt
--rw-r--r--   0 manonmantez   (501) staff       (20)        8 2024-04-17 12:55:58.000000 track2p-0.5.1.1/track2p.egg-info/top_level.txt
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 13:17:22.788514 track2p-0.5.1.2/
+-rw-r--r--   0 manonmantez   (501) staff       (20)    35149 2024-02-12 15:58:33.000000 track2p-0.5.1.2/LICENSE
+-rw-r--r--   0 manonmantez   (501) staff       (20)     5075 2024-04-17 13:17:22.788148 track2p-0.5.1.2/PKG-INFO
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4646 2024-04-16 14:56:02.000000 track2p-0.5.1.2/README.md
+-rw-r--r--   0 manonmantez   (501) staff       (20)       38 2024-04-17 13:17:22.788578 track2p-0.5.1.2/setup.cfg
+-rw-r--r--   0 manonmantez   (501) staff       (20)      593 2024-04-17 13:17:16.000000 track2p-0.5.1.2/setup.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 13:17:22.778781 track2p-0.5.1.2/track2p/
+-rw-r--r--   0 manonmantez   (501) staff       (20)       48 2024-02-22 09:56:18.000000 track2p-0.5.1.2/track2p/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)      417 2024-02-21 12:46:39.000000 track2p-0.5.1.2/track2p/__main__.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 13:17:22.782686 track2p-0.5.1.2/track2p/gui/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.2/track2p/gui/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     8413 2024-04-16 14:56:02.000000 track2p-0.5.1.2/track2p/gui/cell_plot.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     6456 2024-04-16 14:56:02.000000 track2p-0.5.1.2/track2p/gui/fluo_plot.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     2622 2024-04-16 14:56:02.000000 track2p-0.5.1.2/track2p/gui/import_wd.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    22751 2024-04-16 14:56:02.000000 track2p-0.5.1.2/track2p/gui/main_wd.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    15418 2024-04-16 14:56:02.000000 track2p-0.5.1.2/track2p/gui/raster_wd.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     8677 2024-04-16 14:56:02.000000 track2p-0.5.1.2/track2p/gui/roi_plot.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    10842 2024-04-17 13:16:13.000000 track2p-0.5.1.2/track2p/gui/t2p_wd.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 13:17:22.784049 track2p-0.5.1.2/track2p/io/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.2/track2p/io/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     1726 2024-04-16 14:56:02.000000 track2p-0.5.1.2/track2p/io/loaders.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4238 2024-04-16 14:56:02.000000 track2p-0.5.1.2/track2p/io/s2p_loaders.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)      773 2024-02-12 11:04:52.000000 track2p-0.5.1.2/track2p/io/savers.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)      252 2024-01-09 12:56:24.000000 track2p-0.5.1.2/track2p/io/utils.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 13:17:22.784930 track2p-0.5.1.2/track2p/match/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.2/track2p/match/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4471 2024-01-09 12:56:24.000000 track2p-0.5.1.2/track2p/match/loop.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     5807 2024-04-16 14:56:02.000000 track2p-0.5.1.2/track2p/match/utils.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 13:17:22.785352 track2p-0.5.1.2/track2p/ops/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.2/track2p/ops/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     3348 2024-04-16 14:56:02.000000 track2p-0.5.1.2/track2p/ops/default.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 13:17:22.786375 track2p-0.5.1.2/track2p/plot/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.2/track2p/plot/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    15443 2024-04-16 14:56:02.000000 track2p-0.5.1.2/track2p/plot/output.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)      926 2024-02-12 11:04:52.000000 track2p-0.5.1.2/track2p/plot/progress.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     1859 2024-02-12 11:04:52.000000 track2p-0.5.1.2/track2p/plot/utils.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 13:17:22.787532 track2p-0.5.1.2/track2p/register/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.2/track2p/register/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     1348 2024-01-10 11:16:47.000000 track2p-0.5.1.2/track2p/register/elastix.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4054 2024-01-09 12:56:24.000000 track2p-0.5.1.2/track2p/register/loop.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     2345 2024-01-09 12:56:24.000000 track2p-0.5.1.2/track2p/register/utils.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     9791 2024-04-16 14:56:02.000000 track2p-0.5.1.2/track2p/t2p.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 13:17:22.779856 track2p-0.5.1.2/track2p.egg-info/
+-rw-r--r--   0 manonmantez   (501) staff       (20)     5075 2024-04-17 13:17:22.000000 track2p-0.5.1.2/track2p.egg-info/PKG-INFO
+-rw-r--r--   0 manonmantez   (501) staff       (20)      861 2024-04-17 13:17:22.000000 track2p-0.5.1.2/track2p.egg-info/SOURCES.txt
+-rw-r--r--   0 manonmantez   (501) staff       (20)        1 2024-04-17 13:17:22.000000 track2p-0.5.1.2/track2p.egg-info/dependency_links.txt
+-rw-r--r--   0 manonmantez   (501) staff       (20)      163 2024-04-17 13:17:22.000000 track2p-0.5.1.2/track2p.egg-info/requires.txt
+-rw-r--r--   0 manonmantez   (501) staff       (20)        8 2024-04-17 13:17:22.000000 track2p-0.5.1.2/track2p.egg-info/top_level.txt
```

### Comparing `track2p-0.5.1.1/LICENSE` & `track2p-0.5.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.1/PKG-INFO` & `track2p-0.5.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: track2p
-Version: 0.5.1.1
+Version: 0.5.1.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.23.5
 Requires-Dist: matplotlib==3.5.3
 Requires-Dist: scikit-image==0.20.0
 Requires-Dist: itk-elastix==0.19.1
 Requires-Dist: PyQt5==5.15.10
```

### Comparing `track2p-0.5.1.1/README.md` & `track2p-0.5.1.2/README.md`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.1/setup.py` & `track2p-0.5.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='track2p',
-    version='0.5.1.1',
+    version='0.5.1.2',
     packages=find_packages(),
     install_requires=[
         'numpy==1.23.5',
         'matplotlib==3.5.3',
         'scikit-image==0.20.0',
         'itk-elastix==0.19.1',
         'PyQt5==5.15.10',
```

### Comparing `track2p-0.5.1.1/track2p/gui/cell_plot.py` & `track2p-0.5.1.2/track2p/gui/cell_plot.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.1/track2p/gui/fluo_plot.py` & `track2p-0.5.1.2/track2p/gui/fluo_plot.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.1/track2p/gui/import_wd.py` & `track2p-0.5.1.2/track2p/gui/import_wd.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.1/track2p/gui/main_wd.py` & `track2p-0.5.1.2/track2p/gui/main_wd.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.1/track2p/gui/raster_wd.py` & `track2p-0.5.1.2/track2p/gui/raster_wd.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.1/track2p/gui/roi_plot.py` & `track2p-0.5.1.2/track2p/gui/roi_plot.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.1/track2p/gui/t2p_wd.py` & `track2p-0.5.1.2/track2p/gui/t2p_wd.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,19 @@
                 print(item_universel)
                 #self.stored_all_ds_path.append(self.paths_list.item(i).data(Qt.UserRole))
                 self.stored_all_ds_path.append(item_universel)
             print("All parameters have been recorded ! The track2p algorithm is running...")
            # self.track_ops = DefaultTrackOps() #Initializes the self.track_ops object with the default parameters
             self.track_ops.all_ds_path= self.stored_all_ds_path
             #print(f'self.track_ops.all_ds_path : {self.track_ops.all_ds_path}')
-            self.track_ops.save_path = self.save_track2p_path
+            #print(self.save_path)
+            save_path=self.save_track2p_path
+            save_path=save_path.replace("\\", "/")
+            #self.track_ops.save_path = self.save_track2p_path
+            self.track_ops.save_path = save_path
             self.track_ops.reg_chan=int(self.reg_channel)
             if self.checkbox1.isChecked():
                 self.track_ops.iscell_thr=None
             if self.checkbox2.isChecked():
                 self.track_ops.iscell_thr=float(self.is_cell)
             if self.checkbox3.isChecked():
                 self.track_ops.save_in_s2p_format=True
```

### Comparing `track2p-0.5.1.1/track2p/io/loaders.py` & `track2p-0.5.1.2/track2p/io/loaders.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.1/track2p/io/s2p_loaders.py` & `track2p-0.5.1.2/track2p/io/s2p_loaders.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.1/track2p/io/savers.py` & `track2p-0.5.1.2/track2p/io/savers.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.1/track2p/match/loop.py` & `track2p-0.5.1.2/track2p/match/loop.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.1/track2p/match/utils.py` & `track2p-0.5.1.2/track2p/match/utils.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.1/track2p/ops/default.py` & `track2p-0.5.1.2/track2p/ops/default.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.1/track2p/plot/output.py` & `track2p-0.5.1.2/track2p/plot/output.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.1/track2p/plot/progress.py` & `track2p-0.5.1.2/track2p/plot/progress.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.1/track2p/plot/utils.py` & `track2p-0.5.1.2/track2p/plot/utils.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.1/track2p/register/elastix.py` & `track2p-0.5.1.2/track2p/register/elastix.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.1/track2p/register/loop.py` & `track2p-0.5.1.2/track2p/register/loop.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.1/track2p/register/utils.py` & `track2p-0.5.1.2/track2p/register/utils.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.1/track2p/t2p.py` & `track2p-0.5.1.2/track2p/t2p.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1.1/track2p.egg-info/PKG-INFO` & `track2p-0.5.1.2/track2p.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: track2p
-Version: 0.5.1.1
+Version: 0.5.1.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.23.5
 Requires-Dist: matplotlib==3.5.3
 Requires-Dist: scikit-image==0.20.0
 Requires-Dist: itk-elastix==0.19.1
 Requires-Dist: PyQt5==5.15.10
```

### Comparing `track2p-0.5.1.1/track2p.egg-info/SOURCES.txt` & `track2p-0.5.1.2/track2p.egg-info/SOURCES.txt`

 * *Files identical despite different names*

