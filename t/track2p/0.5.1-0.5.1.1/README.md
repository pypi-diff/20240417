# Comparing `tmp/track2p-0.5.1.tar.gz` & `tmp/track2p-0.5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "track2p-0.5.1.tar", last modified: Tue Apr 16 15:14:01 2024, max compression
+gzip compressed data, was "track2p-0.5.1.1.tar", last modified: Wed Apr 17 12:55:59 2024, max compression
```

## Comparing `track2p-0.5.1.tar` & `track2p-0.5.1.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-16 15:14:01.009960 track2p-0.5.1/
--rw-r--r--   0 manonmantez   (501) staff       (20)    35149 2024-02-12 15:58:33.000000 track2p-0.5.1/LICENSE
--rw-r--r--   0 manonmantez   (501) staff       (20)     5073 2024-04-16 15:14:01.009626 track2p-0.5.1/PKG-INFO
--rw-r--r--   0 manonmantez   (501) staff       (20)     4646 2024-04-16 14:56:02.000000 track2p-0.5.1/README.md
--rw-r--r--   0 manonmantez   (501) staff       (20)       38 2024-04-16 15:14:01.010021 track2p-0.5.1/setup.cfg
--rw-r--r--   0 manonmantez   (501) staff       (20)      591 2024-04-16 15:13:05.000000 track2p-0.5.1/setup.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-16 15:14:01.000571 track2p-0.5.1/track2p/
--rw-r--r--   0 manonmantez   (501) staff       (20)       48 2024-02-22 09:56:18.000000 track2p-0.5.1/track2p/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      417 2024-02-21 12:46:39.000000 track2p-0.5.1/track2p/__main__.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-16 15:14:01.004501 track2p-0.5.1/track2p/gui/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1/track2p/gui/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     8413 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/gui/cell_plot.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     6456 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/gui/fluo_plot.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     2622 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/gui/import_wd.py
--rw-r--r--   0 manonmantez   (501) staff       (20)    22751 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/gui/main_wd.py
--rw-r--r--   0 manonmantez   (501) staff       (20)    15418 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/gui/raster_wd.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     8677 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/gui/roi_plot.py
--rw-r--r--   0 manonmantez   (501) staff       (20)    10427 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/gui/t2p_wd.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-16 15:14:01.005757 track2p-0.5.1/track2p/io/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1/track2p/io/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     1726 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/io/loaders.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     4238 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/io/s2p_loaders.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      773 2024-02-12 11:04:52.000000 track2p-0.5.1/track2p/io/savers.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      252 2024-01-09 12:56:24.000000 track2p-0.5.1/track2p/io/utils.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-16 15:14:01.006576 track2p-0.5.1/track2p/match/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1/track2p/match/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     4471 2024-01-09 12:56:24.000000 track2p-0.5.1/track2p/match/loop.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     5807 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/match/utils.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-16 15:14:01.006976 track2p-0.5.1/track2p/ops/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1/track2p/ops/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     3348 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/ops/default.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-16 15:14:01.007909 track2p-0.5.1/track2p/plot/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1/track2p/plot/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)    15443 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/plot/output.py
--rw-r--r--   0 manonmantez   (501) staff       (20)      926 2024-02-12 11:04:52.000000 track2p-0.5.1/track2p/plot/progress.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     1859 2024-02-12 11:04:52.000000 track2p-0.5.1/track2p/plot/utils.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-16 15:14:01.009057 track2p-0.5.1/track2p/register/
--rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1/track2p/register/__init__.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     1348 2024-01-10 11:16:47.000000 track2p-0.5.1/track2p/register/elastix.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     4054 2024-01-09 12:56:24.000000 track2p-0.5.1/track2p/register/loop.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     2345 2024-01-09 12:56:24.000000 track2p-0.5.1/track2p/register/utils.py
--rw-r--r--   0 manonmantez   (501) staff       (20)     9791 2024-04-16 14:56:02.000000 track2p-0.5.1/track2p/t2p.py
-drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-16 15:14:01.001743 track2p-0.5.1/track2p.egg-info/
--rw-r--r--   0 manonmantez   (501) staff       (20)     5073 2024-04-16 15:14:00.000000 track2p-0.5.1/track2p.egg-info/PKG-INFO
--rw-r--r--   0 manonmantez   (501) staff       (20)      861 2024-04-16 15:14:00.000000 track2p-0.5.1/track2p.egg-info/SOURCES.txt
--rw-r--r--   0 manonmantez   (501) staff       (20)        1 2024-04-16 15:14:00.000000 track2p-0.5.1/track2p.egg-info/dependency_links.txt
--rw-r--r--   0 manonmantez   (501) staff       (20)      163 2024-04-16 15:14:00.000000 track2p-0.5.1/track2p.egg-info/requires.txt
--rw-r--r--   0 manonmantez   (501) staff       (20)        8 2024-04-16 15:14:00.000000 track2p-0.5.1/track2p.egg-info/top_level.txt
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 12:55:59.051789 track2p-0.5.1.1/
+-rw-r--r--   0 manonmantez   (501) staff       (20)    35149 2024-02-12 15:58:33.000000 track2p-0.5.1.1/LICENSE
+-rw-r--r--   0 manonmantez   (501) staff       (20)     5075 2024-04-17 12:55:59.051430 track2p-0.5.1.1/PKG-INFO
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4646 2024-04-16 14:56:02.000000 track2p-0.5.1.1/README.md
+-rw-r--r--   0 manonmantez   (501) staff       (20)       38 2024-04-17 12:55:59.051864 track2p-0.5.1.1/setup.cfg
+-rw-r--r--   0 manonmantez   (501) staff       (20)      593 2024-04-17 12:55:32.000000 track2p-0.5.1.1/setup.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 12:55:59.041689 track2p-0.5.1.1/track2p/
+-rw-r--r--   0 manonmantez   (501) staff       (20)       48 2024-02-22 09:56:18.000000 track2p-0.5.1.1/track2p/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)      417 2024-02-21 12:46:39.000000 track2p-0.5.1.1/track2p/__main__.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 12:55:59.045958 track2p-0.5.1.1/track2p/gui/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.1/track2p/gui/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     8413 2024-04-16 14:56:02.000000 track2p-0.5.1.1/track2p/gui/cell_plot.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     6456 2024-04-16 14:56:02.000000 track2p-0.5.1.1/track2p/gui/fluo_plot.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     2622 2024-04-16 14:56:02.000000 track2p-0.5.1.1/track2p/gui/import_wd.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    22751 2024-04-16 14:56:02.000000 track2p-0.5.1.1/track2p/gui/main_wd.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    15418 2024-04-16 14:56:02.000000 track2p-0.5.1.1/track2p/gui/raster_wd.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     8677 2024-04-16 14:56:02.000000 track2p-0.5.1.1/track2p/gui/roi_plot.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    10661 2024-04-17 12:49:47.000000 track2p-0.5.1.1/track2p/gui/t2p_wd.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 12:55:59.047324 track2p-0.5.1.1/track2p/io/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.1/track2p/io/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     1726 2024-04-16 14:56:02.000000 track2p-0.5.1.1/track2p/io/loaders.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4238 2024-04-16 14:56:02.000000 track2p-0.5.1.1/track2p/io/s2p_loaders.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)      773 2024-02-12 11:04:52.000000 track2p-0.5.1.1/track2p/io/savers.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)      252 2024-01-09 12:56:24.000000 track2p-0.5.1.1/track2p/io/utils.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 12:55:59.048272 track2p-0.5.1.1/track2p/match/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.1/track2p/match/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4471 2024-01-09 12:56:24.000000 track2p-0.5.1.1/track2p/match/loop.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     5807 2024-04-16 14:56:02.000000 track2p-0.5.1.1/track2p/match/utils.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 12:55:59.048694 track2p-0.5.1.1/track2p/ops/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.1/track2p/ops/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     3348 2024-04-16 14:56:02.000000 track2p-0.5.1.1/track2p/ops/default.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 12:55:59.049689 track2p-0.5.1.1/track2p/plot/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.1/track2p/plot/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)    15443 2024-04-16 14:56:02.000000 track2p-0.5.1.1/track2p/plot/output.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)      926 2024-02-12 11:04:52.000000 track2p-0.5.1.1/track2p/plot/progress.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     1859 2024-02-12 11:04:52.000000 track2p-0.5.1.1/track2p/plot/utils.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 12:55:59.050841 track2p-0.5.1.1/track2p/register/
+-rw-r--r--   0 manonmantez   (501) staff       (20)        0 2024-02-21 13:37:36.000000 track2p-0.5.1.1/track2p/register/__init__.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     1348 2024-01-10 11:16:47.000000 track2p-0.5.1.1/track2p/register/elastix.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     4054 2024-01-09 12:56:24.000000 track2p-0.5.1.1/track2p/register/loop.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     2345 2024-01-09 12:56:24.000000 track2p-0.5.1.1/track2p/register/utils.py
+-rw-r--r--   0 manonmantez   (501) staff       (20)     9791 2024-04-16 14:56:02.000000 track2p-0.5.1.1/track2p/t2p.py
+drwxr-xr-x   0 manonmantez   (501) staff       (20)        0 2024-04-17 12:55:59.042881 track2p-0.5.1.1/track2p.egg-info/
+-rw-r--r--   0 manonmantez   (501) staff       (20)     5075 2024-04-17 12:55:58.000000 track2p-0.5.1.1/track2p.egg-info/PKG-INFO
+-rw-r--r--   0 manonmantez   (501) staff       (20)      861 2024-04-17 12:55:58.000000 track2p-0.5.1.1/track2p.egg-info/SOURCES.txt
+-rw-r--r--   0 manonmantez   (501) staff       (20)        1 2024-04-17 12:55:58.000000 track2p-0.5.1.1/track2p.egg-info/dependency_links.txt
+-rw-r--r--   0 manonmantez   (501) staff       (20)      163 2024-04-17 12:55:58.000000 track2p-0.5.1.1/track2p.egg-info/requires.txt
+-rw-r--r--   0 manonmantez   (501) staff       (20)        8 2024-04-17 12:55:58.000000 track2p-0.5.1.1/track2p.egg-info/top_level.txt
```

### Comparing `track2p-0.5.1/LICENSE` & `track2p-0.5.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/PKG-INFO` & `track2p-0.5.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: track2p
-Version: 0.5.1
+Version: 0.5.1.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.23.5
 Requires-Dist: matplotlib==3.5.3
 Requires-Dist: scikit-image==0.20.0
 Requires-Dist: itk-elastix==0.19.1
 Requires-Dist: PyQt5==5.15.10
```

### Comparing `track2p-0.5.1/README.md` & `track2p-0.5.1.1/README.md`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/setup.py` & `track2p-0.5.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='track2p',
-    version='0.5.1',
+    version='0.5.1.1',
     packages=find_packages(),
     install_requires=[
         'numpy==1.23.5',
         'matplotlib==3.5.3',
         'scikit-image==0.20.0',
         'itk-elastix==0.19.1',
         'PyQt5==5.15.10',
```

### Comparing `track2p-0.5.1/track2p/gui/cell_plot.py` & `track2p-0.5.1.1/track2p/gui/cell_plot.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/track2p/gui/fluo_plot.py` & `track2p-0.5.1.1/track2p/gui/fluo_plot.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/track2p/gui/import_wd.py` & `track2p-0.5.1.1/track2p/gui/import_wd.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/track2p/gui/main_wd.py` & `track2p-0.5.1.1/track2p/gui/main_wd.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/track2p/gui/raster_wd.py` & `track2p-0.5.1.1/track2p/gui/raster_wd.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/track2p/gui/roi_plot.py` & `track2p-0.5.1.1/track2p/gui/roi_plot.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/track2p/gui/t2p_wd.py` & `track2p-0.5.1.1/track2p/gui/t2p_wd.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,20 @@
         def run(self):
             # Store the text in a variable
             self.is_cell= self.is_cell_thr.text()
             self.reg_channel= self.reg_chan.text()
             self.save_track2p_path= self.savedirectory
             self.stored_all_ds_path = []
             for i in range(self.paths_list.count()):
-                self.stored_all_ds_path.append(self.paths_list.item(i).data(Qt.UserRole))
+                item=self.paths_list.item(i).data(Qt.UserRole)
+                print(item)
+                item_universel=item.replace("\\", "/")
+                print(item_universel)
+                #self.stored_all_ds_path.append(self.paths_list.item(i).data(Qt.UserRole))
+                self.stored_all_ds_path.append(item_universel)
             print("All parameters have been recorded ! The track2p algorithm is running...")
            # self.track_ops = DefaultTrackOps() #Initializes the self.track_ops object with the default parameters
             self.track_ops.all_ds_path= self.stored_all_ds_path
             #print(f'self.track_ops.all_ds_path : {self.track_ops.all_ds_path}')
             self.track_ops.save_path = self.save_track2p_path
             self.track_ops.reg_chan=int(self.reg_channel)
             if self.checkbox1.isChecked():
@@ -174,22 +179,22 @@
 
 
         def moveFileToBox(self):
             selectedItems = self.computer_file_list.selectedItems()
             for item in selectedItems:
                 self.computer_file_list.takeItem(self.computer_file_list.row(item))
                 self.paths_list.addItem(item)
-       
+     
 
         def moveFileToComputer(self):
             selectedItems = self.paths_list.selectedItems()
             for item in selectedItems:
                 self.paths_list.takeItem(self.paths_list.row(item))
                 self.computer_file_list.addItem(item)
-                
+    
 
 class ComboBoxDialog(QDialog):
     def __init__(self, parent=None):
         super(ComboBoxDialog, self).__init__(parent)
         self.parent=parent
         self.layout = QFormLayout(self)
```

### Comparing `track2p-0.5.1/track2p/io/loaders.py` & `track2p-0.5.1.1/track2p/io/loaders.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/track2p/io/s2p_loaders.py` & `track2p-0.5.1.1/track2p/io/s2p_loaders.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/track2p/io/savers.py` & `track2p-0.5.1.1/track2p/io/savers.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/track2p/match/loop.py` & `track2p-0.5.1.1/track2p/match/loop.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/track2p/match/utils.py` & `track2p-0.5.1.1/track2p/match/utils.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/track2p/ops/default.py` & `track2p-0.5.1.1/track2p/ops/default.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/track2p/plot/output.py` & `track2p-0.5.1.1/track2p/plot/output.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/track2p/plot/progress.py` & `track2p-0.5.1.1/track2p/plot/progress.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/track2p/plot/utils.py` & `track2p-0.5.1.1/track2p/plot/utils.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/track2p/register/elastix.py` & `track2p-0.5.1.1/track2p/register/elastix.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/track2p/register/loop.py` & `track2p-0.5.1.1/track2p/register/loop.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/track2p/register/utils.py` & `track2p-0.5.1.1/track2p/register/utils.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/track2p/t2p.py` & `track2p-0.5.1.1/track2p/t2p.py`

 * *Files identical despite different names*

### Comparing `track2p-0.5.1/track2p.egg-info/PKG-INFO` & `track2p-0.5.1.1/track2p.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: track2p
-Version: 0.5.1
+Version: 0.5.1.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.23.5
 Requires-Dist: matplotlib==3.5.3
 Requires-Dist: scikit-image==0.20.0
 Requires-Dist: itk-elastix==0.19.1
 Requires-Dist: PyQt5==5.15.10
```

### Comparing `track2p-0.5.1/track2p.egg-info/SOURCES.txt` & `track2p-0.5.1.1/track2p.egg-info/SOURCES.txt`

 * *Files identical despite different names*

