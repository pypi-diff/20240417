# Comparing `tmp/silicon_analyser-1.0.6.tar.gz` & `tmp/silicon_analyser-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silicon_analyser-1.0.6.tar", last modified: Mon Apr 15 16:13:13 2024, max compression
+gzip compressed data, was "silicon_analyser-1.0.7.tar", last modified: Wed Apr 17 18:29:27 2024, max compression
```

## Comparing `silicon_analyser-1.0.6.tar` & `silicon_analyser-1.0.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 16:13:12.000000 silicon_analyser-1.0.6/
--rw-rw-rw-   0        0        0     1087 2024-04-07 16:13:23.000000 silicon_analyser-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     3242 2024-04-15 16:13:13.000000 silicon_analyser-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2461 2024-04-14 16:45:54.000000 silicon_analyser-1.0.6/README.md
--rw-rw-rw-   0        0        0     1141 2024-04-15 15:27:19.000000 silicon_analyser-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-15 16:13:13.000000 silicon_analyser-1.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-15 16:13:12.000000 silicon_analyser-1.0.6/silicon_analyser/
-drwxrwxrwx   0        0        0        0 2024-04-15 16:13:12.000000 silicon_analyser-1.0.6/silicon_analyser/dialogs/
--rw-rw-rw-   0        0        0     3487 2024-04-13 14:15:10.000000 silicon_analyser-1.0.6/silicon_analyser/dialogs/compute_stats.py
--rw-rw-rw-   0        0        0     1508 2024-04-06 18:45:56.000000 silicon_analyser-1.0.6/silicon_analyser/dialogs/compute_stats.ui
--rw-rw-rw-   0        0        0     3340 2024-04-14 09:21:04.000000 silicon_analyser-1.0.6/silicon_analyser/dialogs/pixel_image.py
--rw-rw-rw-   0        0        0     3752 2024-04-14 09:20:00.000000 silicon_analyser-1.0.6/silicon_analyser/dialogs/pixel_image.ui
--rw-rw-rw-   0        0        0     3096 2024-04-15 15:27:03.000000 silicon_analyser-1.0.6/silicon_analyser/grid.py
-drwxrwxrwx   0        0        0        0 2024-04-15 16:13:12.000000 silicon_analyser-1.0.6/silicon_analyser/helper/
-drwxrwxrwx   0        0        0        0 2024-04-15 16:13:12.000000 silicon_analyser-1.0.6/silicon_analyser/helper/abstract/
--rw-rw-rw-   0        0        0     2313 2024-04-13 13:47:07.000000 silicon_analyser-1.0.6/silicon_analyser/helper/abstract/abstractimage.py
--rw-rw-rw-   0        0        0     2771 2024-04-14 06:57:02.000000 silicon_analyser-1.0.6/silicon_analyser/helper/abstract/abstractmywindow.py
--rw-rw-rw-   0        0        0     1024 2024-04-13 06:54:26.000000 silicon_analyser-1.0.6/silicon_analyser/helper/abstract/abstracttreehelper.py
--rw-rw-rw-   0        0        0      719 2024-04-13 07:29:28.000000 silicon_analyser-1.0.6/silicon_analyser/helper/addgridbtn.py
--rw-rw-rw-   0        0        0      696 2024-04-08 17:17:53.000000 silicon_analyser-1.0.6/silicon_analyser/helper/addlabelbtn.py
--rw-rw-rw-   0        0        0     1354 2024-04-14 11:44:59.000000 silicon_analyser-1.0.6/silicon_analyser/helper/ai.py
--rw-rw-rw-   0        0        0    14402 2024-04-14 16:49:50.000000 silicon_analyser-1.0.6/silicon_analyser/helper/computebtn.py
--rw-rw-rw-   0        0        0    20772 2024-04-15 15:38:08.000000 silicon_analyser-1.0.6/silicon_analyser/helper/fullimage.py
--rw-rw-rw-   0        0        0     1532 2024-04-13 13:40:26.000000 silicon_analyser-1.0.6/silicon_analyser/helper/minimap.py
--rw-rw-rw-   0        0        0     3499 2024-04-13 13:39:46.000000 silicon_analyser-1.0.6/silicon_analyser/helper/properties.py
--rw-rw-rw-   0        0        0    18962 2024-04-15 15:54:55.000000 silicon_analyser-1.0.6/silicon_analyser/helper/tree.py
--rw-rw-rw-   0        0        0      263 2024-04-08 17:15:10.000000 silicon_analyser-1.0.6/silicon_analyser/main.py
--rw-rw-rw-   0        0        0     6698 2024-04-15 15:57:44.000000 silicon_analyser-1.0.6/silicon_analyser/main_window.ui
--rw-rw-rw-   0        0        0     9837 2024-04-15 16:00:59.000000 silicon_analyser-1.0.6/silicon_analyser/mywindow.py
--rw-rw-rw-   0        0        0      134 2024-04-07 08:11:27.000000 silicon_analyser-1.0.6/silicon_analyser/rect.py
--rw-rw-rw-   0        0        0     2053 2024-04-13 13:22:20.000000 silicon_analyser-1.0.6/silicon_analyser/savefiles.py
--rw-rw-rw-   0        0        0     1365 2024-04-13 14:16:41.000000 silicon_analyser-1.0.6/silicon_analyser/treeitem.py
-drwxrwxrwx   0        0        0        0 2024-04-15 16:13:12.000000 silicon_analyser-1.0.6/silicon_analyser.egg-info/
--rw-rw-rw-   0        0        0     3242 2024-04-15 16:13:13.000000 silicon_analyser-1.0.6/silicon_analyser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1078 2024-04-15 16:13:13.000000 silicon_analyser-1.0.6/silicon_analyser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 16:13:13.000000 silicon_analyser-1.0.6/silicon_analyser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-04-15 16:13:13.000000 silicon_analyser-1.0.6/silicon_analyser.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2024-04-15 16:13:13.000000 silicon_analyser-1.0.6/silicon_analyser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-15 16:13:13.000000 silicon_analyser-1.0.6/silicon_analyser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 18:29:27.000000 silicon_analyser-1.0.7/
+-rw-rw-rw-   0        0        0     1087 2024-04-07 16:13:23.000000 silicon_analyser-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     3334 2024-04-17 18:29:27.000000 silicon_analyser-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2530 2024-04-16 18:45:45.000000 silicon_analyser-1.0.7/README.md
+-rw-rw-rw-   0        0        0     1154 2024-04-16 16:45:56.000000 silicon_analyser-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-17 18:29:27.000000 silicon_analyser-1.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 18:29:27.000000 silicon_analyser-1.0.7/silicon_analyser/
+drwxrwxrwx   0        0        0        0 2024-04-17 18:29:27.000000 silicon_analyser-1.0.7/silicon_analyser/dialogs/
+-rw-rw-rw-   0        0        0     3487 2024-04-13 14:15:10.000000 silicon_analyser-1.0.7/silicon_analyser/dialogs/compute_stats.py
+-rw-rw-rw-   0        0        0     1508 2024-04-06 18:45:56.000000 silicon_analyser-1.0.7/silicon_analyser/dialogs/compute_stats.ui
+-rw-rw-rw-   0        0        0     3340 2024-04-14 09:21:04.000000 silicon_analyser-1.0.7/silicon_analyser/dialogs/pixel_image.py
+-rw-rw-rw-   0        0        0     3752 2024-04-14 09:20:00.000000 silicon_analyser-1.0.7/silicon_analyser/dialogs/pixel_image.ui
+-rw-rw-rw-   0        0        0     3883 2024-04-16 18:29:36.000000 silicon_analyser-1.0.7/silicon_analyser/grid.py
+drwxrwxrwx   0        0        0        0 2024-04-17 18:29:27.000000 silicon_analyser-1.0.7/silicon_analyser/helper/
+drwxrwxrwx   0        0        0        0 2024-04-17 18:29:27.000000 silicon_analyser-1.0.7/silicon_analyser/helper/abstract/
+-rw-rw-rw-   0        0        0     2406 2024-04-16 16:39:34.000000 silicon_analyser-1.0.7/silicon_analyser/helper/abstract/abstractimage.py
+-rw-rw-rw-   0        0        0     2812 2024-04-16 16:00:12.000000 silicon_analyser-1.0.7/silicon_analyser/helper/abstract/abstractmywindow.py
+-rw-rw-rw-   0        0        0     1024 2024-04-13 06:54:26.000000 silicon_analyser-1.0.7/silicon_analyser/helper/abstract/abstracttreehelper.py
+-rw-rw-rw-   0        0        0      719 2024-04-13 07:29:28.000000 silicon_analyser-1.0.7/silicon_analyser/helper/addgridbtn.py
+-rw-rw-rw-   0        0        0      696 2024-04-08 17:17:53.000000 silicon_analyser-1.0.7/silicon_analyser/helper/addlabelbtn.py
+-rw-rw-rw-   0        0        0     1403 2024-04-16 18:13:14.000000 silicon_analyser-1.0.7/silicon_analyser/helper/ai.py
+-rw-rw-rw-   0        0        0    14568 2024-04-16 17:42:57.000000 silicon_analyser-1.0.7/silicon_analyser/helper/computebtn.py
+-rw-rw-rw-   0        0        0    21170 2024-04-17 15:20:05.000000 silicon_analyser-1.0.7/silicon_analyser/helper/fullimage.py
+-rw-rw-rw-   0        0        0     1532 2024-04-13 13:40:26.000000 silicon_analyser-1.0.7/silicon_analyser/helper/minimap.py
+-rw-rw-rw-   0        0        0     3989 2024-04-16 18:29:06.000000 silicon_analyser-1.0.7/silicon_analyser/helper/properties.py
+-rw-rw-rw-   0        0        0    20657 2024-04-16 18:12:59.000000 silicon_analyser-1.0.7/silicon_analyser/helper/tree.py
+-rw-rw-rw-   0        0        0      263 2024-04-08 17:15:10.000000 silicon_analyser-1.0.7/silicon_analyser/main.py
+-rw-rw-rw-   0        0        0     6845 2024-04-16 15:59:53.000000 silicon_analyser-1.0.7/silicon_analyser/main_window.ui
+-rw-rw-rw-   0        0        0     9878 2024-04-16 16:00:07.000000 silicon_analyser-1.0.7/silicon_analyser/mywindow.py
+-rw-rw-rw-   0        0        0      134 2024-04-07 08:11:27.000000 silicon_analyser-1.0.7/silicon_analyser/rect.py
+-rw-rw-rw-   0        0        0     2305 2024-04-16 18:10:57.000000 silicon_analyser-1.0.7/silicon_analyser/savefiles.py
+-rw-rw-rw-   0        0        0     1365 2024-04-13 14:16:41.000000 silicon_analyser-1.0.7/silicon_analyser/treeitem.py
+drwxrwxrwx   0        0        0        0 2024-04-17 18:29:27.000000 silicon_analyser-1.0.7/silicon_analyser.egg-info/
+-rw-rw-rw-   0        0        0     3334 2024-04-17 18:29:27.000000 silicon_analyser-1.0.7/silicon_analyser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1078 2024-04-17 18:29:27.000000 silicon_analyser-1.0.7/silicon_analyser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 18:29:27.000000 silicon_analyser-1.0.7/silicon_analyser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-04-17 18:29:27.000000 silicon_analyser-1.0.7/silicon_analyser.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       64 2024-04-17 18:29:27.000000 silicon_analyser-1.0.7/silicon_analyser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-17 18:29:27.000000 silicon_analyser-1.0.7/silicon_analyser.egg-info/top_level.txt
```

### Comparing `silicon_analyser-1.0.6/LICENSE` & `silicon_analyser-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.6/PKG-INFO` & `silicon_analyser-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: silicon-analyser
-Version: 1.0.6
+Version: 1.0.7
 Summary: helps to analyse integrated circuit die images (for example from siliconpr0n.org) with the help of ai.
 Author-email: CrazyT <crazyt2019+sa@gmail.com>
 Project-URL: Homepage, https://github.com/TheCrazyT/SiliconAnalyser
 Project-URL: Bug Tracker, https://github.com/TheCrazyT/SiliconAnalyser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: numpy
+Requires-Dist: pillow
 Requires-Dist: keras
 Requires-Dist: PyQt5
 Requires-Dist: pyqtgraph
 Requires-Dist: scikit-learn
 Requires-Dist: packaging
 
 # Installation
 
 Install from source:
 
-`pip install .`
+`pip install --upgrade .`
 
 Install from pip:
 
-`pip install silicon-analyser`
+`pip install --upgrade silicon-analyser`
 
 # Information
 
 Code will use your graphic card for acceleration.
 (but only if correct pytorch is installed, see "Additional info" below)
 
 Frameworks/Libraries used:
@@ -80,11 +81,12 @@
 * Right click on tree-items (left navigation menu) for additional options
 
 ![image](https://raw.githubusercontent.com/TheCrazyT/SiliconAnalyser/main/docs/small_tutorial.gif)
 
 # TODO
 
 * show loading screen on start (pytorch with cuda support takes a bit to load)
+* option to calculate/classify by decision tree
 * auto-compute to calculate in background while you are selecting new cells for your labels
 * ai-model configuration
 * possibility to rotate grid
 * maybe store your model on a public place? (for others to use)
```

### Comparing `silicon_analyser-1.0.6/README.md` & `silicon_analyser-1.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Installation
 
 Install from source:
 
-`pip install .`
+`pip install --upgrade .`
 
 Install from pip:
 
-`pip install silicon-analyser`
+`pip install --upgrade silicon-analyser`
 
 # Information
 
 Code will use your graphic card for acceleration.
 (but only if correct pytorch is installed, see "Additional info" below)
 
 Frameworks/Libraries used:
@@ -59,11 +59,12 @@
 * Right click on tree-items (left navigation menu) for additional options
 
 ![image](https://raw.githubusercontent.com/TheCrazyT/SiliconAnalyser/main/docs/small_tutorial.gif)
 
 # TODO
 
 * show loading screen on start (pytorch with cuda support takes a bit to load)
+* option to calculate/classify by decision tree
 * auto-compute to calculate in background while you are selecting new cells for your labels
 * ai-model configuration
 * possibility to rotate grid
 * maybe store your model on a public place? (for others to use)
```

### Comparing `silicon_analyser-1.0.6/pyproject.toml` & `silicon_analyser-1.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "silicon-analyser"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
   { name="CrazyT", email="crazyt2019+sa@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 description = "helps to analyse integrated circuit die images (for example from siliconpr0n.org) with the help of ai."
 dependencies = [
   "torch",
   "numpy",
+  "pillow",
   "keras",
   "PyQt5",
   "pyqtgraph",
   "scikit-learn",
   "packaging"
 ]
```

### Comparing `silicon_analyser-1.0.6/silicon_analyser/dialogs/compute_stats.py` & `silicon_analyser-1.0.7/silicon_analyser/dialogs/compute_stats.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.6/silicon_analyser/dialogs/compute_stats.ui` & `silicon_analyser-1.0.7/silicon_analyser/dialogs/compute_stats.ui`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.6/silicon_analyser/dialogs/pixel_image.py` & `silicon_analyser-1.0.7/silicon_analyser/dialogs/pixel_image.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.6/silicon_analyser/dialogs/pixel_image.ui` & `silicon_analyser-1.0.7/silicon_analyser/dialogs/pixel_image.ui`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.6/silicon_analyser/grid.py` & `silicon_analyser-1.0.7/silicon_analyser/grid.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,26 +5,51 @@
         self.name = name
         self.x = x
         self.y = y
         self.cols = cols
         self.rows = rows
         self.width = width
         self.height = height
+        self.shearX = 0
+        self.shearY = 0
         self._rects = {}
         self._rectsActive = {}
+        self.recalcCell()
         print(f"init grid:{id(self)}")
     
+    def recalcCell(self):
+        self._cellWidth = self.width / self.cols
+        self._cellHeight = self.height / self.rows
+    
+    def getCellWidth(self) -> float:
+        return self._cellWidth
+
+    def getCellHeight(self) -> float:
+        return self._cellHeight
+    
+    def absX(self, col:int, row:int) -> int:
+        w = self._cellWidth
+        return int(self.x + col*w + self.shearX*row)
+
+    def absY(self, row:int, col:int) -> int:
+        h = self._cellHeight
+        return int(self.y + row*h + self.shearY*col)
+    
     def replaceValues(self,grid):
         self.x = grid.x
         self.y = grid.y
         self.cols = grid.cols
         self.rows = grid.rows
         self.width = grid.width
         self.height = grid.height
         self._rects = grid._rects
+        self._cellHeight = grid._cellHeight
+        self._cellWidth = grid._cellWidth
+        self.shearX = grid.shearX
+        self.shearY = grid.shearY
         for k in self._rects:
             for cx,cy in list(self._rects[k]):
                 if cx < 0 or cy < 0:
                     self._rects[k].remove([cx,cy])
         self._rectsActive = grid._rectsActive
         
     def getLabels(self) -> list[str]:
```

### Comparing `silicon_analyser-1.0.6/silicon_analyser/helper/abstract/abstractimage.py` & `silicon_analyser-1.0.7/silicon_analyser/helper/abstract/abstractimage.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from PyQt5.QtWidgets import QLabel
-
+import typing
+import numpy as np
 from silicon_analyser.grid import Grid
 from silicon_analyser.rect import Rect
 
 class AbstractImage(QLabel):
     
     def clearAIRects(self):
         raise NotImplementedError()
     
-    def fetchData(self,x,y,ex,ey):
+    def fetchData(self,x,y,ex,ey) -> np.ndarray[int,typing.Any]:
         raise NotImplementedError()
     
     def drawImage(self):
         raise NotImplementedError()
     
-    def fetchFullData(self):
+    def fetchFullData(self) -> np.ndarray[int,typing.Any]:
         raise NotImplementedError()
     
     def appendRectGroup(self, text):
          raise NotImplementedError()
 
     def appendAIRectGroup(self, text):
          raise NotImplementedError()
```

### Comparing `silicon_analyser-1.0.6/silicon_analyser/helper/abstract/abstractmywindow.py` & `silicon_analyser-1.0.7/silicon_analyser/helper/abstract/abstractmywindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     _actionGridAddRowTop: QAction
     _actionSaveModel: QAction
     _actionLoadModel: QAction
     _actionRemoveGrid: QAction
     _actionRemoveLabel: QAction
     _actionSaveAsCsv: QAction
     _actionViewAsPixelimage: QAction
+    _actionExportCellsToImages: QAction
     autosave: bool
     def __init__(self):
         QMainWindow.__init__(self)
         
     def getManualItem(self) -> QStandardItem:
         raise NotImplementedError()
```

### Comparing `silicon_analyser-1.0.6/silicon_analyser/helper/abstract/abstracttreehelper.py` & `silicon_analyser-1.0.7/silicon_analyser/helper/abstract/abstracttreehelper.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.6/silicon_analyser/helper/addgridbtn.py` & `silicon_analyser-1.0.7/silicon_analyser/helper/addgridbtn.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.6/silicon_analyser/helper/addlabelbtn.py` & `silicon_analyser-1.0.7/silicon_analyser/helper/addlabelbtn.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.6/silicon_analyser/helper/ai.py` & `silicon_analyser-1.0.7/silicon_analyser/helper/ai.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,37 @@
+import typing
 import os
 import numpy as np
 os.environ["KERAS_BACKEND"] = "torch"
 import keras
 from silicon_analyser.grid import Grid, getAllCellRects
 from silicon_analyser.helper.abstract.abstractimage import AbstractImage
 
-def getDefaultMaxWMaxH(grid: Grid):
-    maxW = grid.width//grid.cols
-    maxH = grid.height//grid.rows
+def getDefaultMaxWMaxH(grid: Grid) -> tuple[int,int]:
+    maxW = int(grid.getCellWidth())
+    maxH = int(grid.getCellHeight())
     MP = 5
     if maxW % MP != 0:
         maxW += MP - (maxW % MP)
     if maxH % MP != 0:
         maxH += MP - (maxH % MP)
     return maxW, maxH
 
-def appendFoundCellRects(img: AbstractImage, grid: Grid, aiGrid: Grid, maxW, maxH, model: keras.Sequential):
+def appendFoundCellRects(img: AbstractImage, grid: Grid, aiGrid: Grid, maxW: int, maxH: int, model: keras.Sequential):
     if maxW is None or maxH is None:
         maxW, maxH = getDefaultMaxWMaxH(grid)
     labels = grid.getLabels()
     allCellRects = getAllCellRects(grid)
     dataList = []
     dataIndexes = []
     for cx,cy in allCellRects:
-        x = int(grid.x + cx*maxW)
-        y = int(grid.y + cy*maxH)
-        ex = x + maxW - 1
-        ey = y + maxH - 1
+        x = grid.absX(cx,cy)
+        y = grid.absY(cy,cx)
+        ex = int(x + maxW - 1)
+        ey = int(y + maxH - 1)
         dataList.append(img.fetchData(x,y,ex,ey))
         dataIndexes.append((cx,cy))
     data = np.array(dataList,dtype=np.float32)
     print("data.shape",data.shape)
     r = model.predict(data)
     print("r.shape",r.shape)
     for ri in range(0,r.shape[0]):
```

### Comparing `silicon_analyser-1.0.6/silicon_analyser/helper/computebtn.py` & `silicon_analyser-1.0.7/silicon_analyser/helper/computebtn.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
             callbacks = [MyPlottingCallback(self._computeStatsDlg),MyThresholdCallback(0.99,200)]
             model_train.compile(optimizer=keras.optimizers.Adam(learning_rate=0.002),loss="binary_crossentropy",metrics=["accuracy"])
             print("before fit")
             print("vals",vals)
             print("train.shape",train.shape)
             print("vals.shape",vals.shape)
             
-            xtraining, ytraining, xvalidation, yvalidation = train_test_split(train,vals,test_size=0.1) 
+            xtraining, ytraining, xvalidation, yvalidation = train_test_split(train,vals,shuffle = True,test_size=0.1) 
 
             history = model_train.fit(
                 x = xtraining,
                 y = xvalidation,
                 epochs = 100000,
                 verbose = 0,
                 validation_data=(ytraining,yvalidation),
@@ -169,15 +169,16 @@
             
             self._myWindow.getImage().drawImage()
             self._myWindow.setLastModel(aiGrid.name, model_train)
         except Exception as e:
             self._computeStatsDlg.setError(e)
         finally:
             self.finished.emit()
-        
+    
+    # TODO: maybe deprecated, not shure yet
     def initTrainAndValsForRects(self, rects, ignoreRects):
         maxW = 0
         maxH = 0
         cntTotal = 0
         for k in rects.keys():
             for x,y,ex,ey in rects[k]:
                 maxW = max(maxW, ex-x)
@@ -197,15 +198,15 @@
         countGroups = len(rects.keys())+1
         train = np.zeros(shape=(cntTotal,maxH,maxW,3),dtype=np.float32)
         vals = np.zeros(shape=(cntTotal,countGroups),dtype=np.float32)
         print("train.shape:",train.shape)
         print("vals.shape:",vals.shape)
         return maxW, maxH, countGroups, MP, train, vals
 
-    def initTrainAndValsForGrid(self, grid:Grid):
+    def initTrainAndValsForGrid(self, grid:Grid) -> tuple[int, int, list[str], int, int, np.ndarray, np.ndarray]:
         labels = grid.getLabels()
         countGroups = len(labels)
         cntTotal = 0
         for l in labels:
             for cx in range(0,grid.cols):
                 for cy in range(0,grid.rows):
                     if grid.isRectSet(cx,cy,l):
@@ -217,16 +218,17 @@
             maxW += MP - (maxW % MP)
         if maxH % MP != 0:
             maxH += MP - (maxH % MP)
         train = np.zeros(shape=(cntTotal,maxH,maxW,3),dtype=np.float32)
         vals = np.zeros(shape=(cntTotal,countGroups),dtype=np.float32)
         print("train.shape:",train.shape)
         print("vals.shape:",vals.shape)
-        return maxW, maxH, labels, countGroups, MP, train, vals
+        return  maxW, maxH, labels, countGroups, MP, train, vals
 
+    # TODO: maybe deprecated, not shure yet
     def prepareRectData(self, rects, countGroups, ignoreRects, maxW, maxH, train, vals):
         self._myWindow.getTree().clearAIItem()
         i = 0
         ii = 1
         print(f"adding ignore values ({len(ignoreRects)})")
             
         for n in range(0,100):
```

### Comparing `silicon_analyser-1.0.6/silicon_analyser/helper/fullimage.py` & `silicon_analyser-1.0.7/silicon_analyser/helper/fullimage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from PyQt5.QtCore import Qt, QRect, QSize, QTimer
 from PyQt5.QtWidgets import QLabel, QSizePolicy
 from PyQt5.QtGui import QImage, QPixmap, QColor, QMouseEvent, QPainter, QPen, QBrush
+import typing
 import numpy as np
 from silicon_analyser.helper.abstract.abstractmywindow import AbstractMyWindow
 from silicon_analyser.savefiles import triggerSaveGrids, triggerSaveRects, saveGrids, saveRects
 from silicon_analyser.grid import Grid
 from silicon_analyser.rect import Rect
 from silicon_analyser.treeitem import TreeItem
 
@@ -166,35 +167,36 @@
                 if selectedKey in self._grids:
                     grid: Grid = self._grids[selectedKey]
                     posX, posY = self._myWindow.getPos()
                     grid.x = posX+x
                     grid.y = posY+y
                     grid.width = ex-x
                     grid.height = ey-y
+                    grid.recalcCell()
                     self._grids[selectedKey] = grid
                     print(f"grid resized: {id(grid)}")
                     self._myWindow.reloadProperyWindowByGrid(grid)
                     if self._myWindow.autosave:
                         triggerSaveGrids()
                 self.drawImage()
         if event.button() == Qt.MouseButton.RightButton:
             print("right click")
             self.removeRectAt(event.x(),event.y())
-            
+    
     def removeRectGroup(self, label):
-        del self._rects[label]
-        del self._aiRects[label]
-        del self._rectActive[label]
-        del self._aiRectActive[label]
+        self._rects.pop(label, None)
+        self._aiRects.pop(label, None)
+        self._rectActive.pop(label, None)
+        self._aiRectActive.pop(label, None)
         
     def removeGrid(self, label):
-        del self._grids[label]
-        del self._aiGrids[label]
-        del self._gridsActive[label]
-        del self._aiGridsActive[label]
+        self._grids.pop(label, None)
+        self._aiGrids.pop(label, None)
+        self._gridsActive.pop(label, None)
+        self._aiGridsActive.pop(label, None)
 
     def removeRectAt(self, evx, evy):
         scale = self._myWindow.getScale()
         posX, posY = self._myWindow.getPos()
         sposX, sposY = posX*scale, posY*scale
         for k in self._rects.keys():
             toRemove = []
@@ -265,22 +267,22 @@
                 posX+ex,
                 posY+ey
             ))
                 
     def appendAIRect(self,key,x,y,ex,ey):
         self._appendRect(key, self._aiRects, x, y, ex, ey, True)
 
-    def fetchFullData(self):
+    def fetchFullData(self) -> np.ndarray[int,typing.Any]:
         temp = QImage(self._pixmap.toImage())
         ptr = temp.constBits()
         ptr.setsize(temp.byteCount())
         arr = np.frombuffer(ptr, dtype=np.ubyte).reshape(temp.height(), temp.width(), 4) # type: ignore
         return arr
     
-    def fetchData(self,x,y,ex,ey):
+    def fetchData(self,x,y,ex,ey) -> np.ndarray[int,typing.Any]:
         x = int(x)
         ex = int(ex)
         y = int(y)
         ey = int(ey)
         arr = self.fetchFullData()
         r = arr[y:ey+1,x:ex+1,0:3]
         return r
@@ -302,14 +304,15 @@
     
     def clearAIRects(self):
         self._aiGridsActive = {}
         self._aiGrids = {}
         self._aiRects = {}
         self._aiRectActive = {}
     
+    # TODO: maybe deprecated, not shure yet
     def drawRectOnScaledImg(self, scaledImg: QPixmap):
         qp = QPainter(scaledImg)
         brush = QBrush(QColor(0,0,255,80))
         pen = QPen(Qt.GlobalColor.blue, 2)
         qp.setBrush(brush)
         qp.setPen(pen)
         self._drawRectOnScaledImg(self._rects, self._rectActive, qp)
@@ -332,19 +335,19 @@
         pen = QPen(QColor(0,0,0,0), 2)
         qp.setBrush(brush)
         qp.setPen(pen)
         self._drawGridOnScaledImg(self._aiGrids, self._aiGridsActive, qp, TreeItem.TYPE_AI_GRID_ITEM, QColor(0,255,0,40), QColor(0,255,0,127), QColor(0,0,0,0))
 
         qp.end()
     
-    def calcGridCellsVisibleRange(self, grid):
+    def calcGridCellsVisibleRange(self, grid: Grid):
         posX, posY = self._myWindow.getPos()
         scale = self._myWindow.getScale()
-        cellWidth = grid.width / grid.cols
-        cellHeight = grid.height / grid.rows
+        cellWidth = grid.getCellWidth()
+        cellHeight = grid.getCellHeight()
         
         startCol = -(grid.x - posX)//cellWidth
         startCol = int(max(0, startCol))
         
         startRow = -(grid.y - posY)//cellHeight
         startRow = int(max(0, startRow))
         
@@ -367,28 +370,30 @@
     def _drawGridOnScaledImg(self, grids, gridsActive, qp:QPainter, gridItemType:str, rectSetColor:QColor = QColor(0,255,255,40), rectSetActiveColor:QColor = QColor(0,255,255,127), rectUnsetColor:QColor = QColor(0,0,255,20)):
         posX, posY = self._myWindow.getPos()
         scale = self._myWindow.getScale()
         sposX, sposY = posX*scale, posY*scale
         for k in grids.keys():
             if gridsActive[k]:
                 grid: Grid = grids[k]
-                cellWidth = grid.width / grid.cols
-                cellHeight = grid.height / grid.rows
+                cellWidth = grid.getCellWidth()
+                cellHeight = grid.getCellHeight()
                 startCol, startRow, endCol, endRow = self.calcGridCellsVisibleRange(grid)
                 for row in range(startRow,endRow):
                     if not self._drawGridOnScaledImgRow(qp, gridItemType, rectSetColor, rectSetActiveColor, rectUnsetColor, sposX, sposY, grid, cellWidth, cellHeight, startCol, endCol, row):
                         break
 
     def _drawGridOnScaledImgRow(self, qp:QPainter, gridItemType:str, rectSetColor:QColor, rectSetActiveColor:QColor, rectUnsetColor:QColor, sposX:float, sposY:float, grid:Grid, cellWidth:float, cellHeight:float, startCol:int, endCol:int, row:int):
-        oy = grid.y + row * cellHeight
+        oy = grid.absY(row, 0)
         y = int(self._translatePixelToScaled(oy)-sposY)
         if y >= self.height():
             return False
         for col in range(startCol,endCol):
-            ox = grid.x + col * cellWidth
+            oy = grid.absY(row, col)
+            y = int(self._translatePixelToScaled(oy)-sposY)
+            ox = grid.absX(col, row)
             ex = ox + cellWidth
             ey = oy + cellHeight
             x = int(self._translatePixelToScaled(ox)-sposX)
             if x > self.width():
                 break
             ex = int(self._translatePixelToScaled(ex)-sposX)
             ey = int(self._translatePixelToScaled(ey)-sposY)
@@ -403,15 +408,16 @@
                         brush = QBrush(rectSetColor)
                     qp.setBrush(brush)
                 else:
                     brush = QBrush(rectUnsetColor)
                     qp.setBrush(brush)
                 qp.drawRect(x,y,w,h)
         return True
-                        
+
+    # TODO: maybe deprecated, not shure yet                        
     def _drawRectOnScaledImg(self, rects, rectActive, qp:QPainter):
         posX, posY = self._myWindow.getPos()
         scale = self._myWindow.getScale()
         sposX, sposY = posX*scale, posY*scale
         for k in rects.keys():
             if rectActive[k]:
                 for r in rects[k]:
@@ -435,14 +441,16 @@
         self.drawRectOnScaledImg(scaled)
         self.drawGridOnScaledImg(scaled)
         self.setPixmap(scaled)
     
     def appendAIGrid(self, text):
         grid = self._grids[text]
         aiGrid = Grid(grid.name,grid.x,grid.y,grid.cols,grid.rows,grid.width,grid.height)
+        aiGrid.shearX = grid.shearX
+        aiGrid.shearY = grid.shearY
         self._aiGrids[text] = aiGrid
         return aiGrid
     
     def appendGrid(self, text):
         grid = Grid(text,0,0,20,20,20*10,20*10)
         self._grids[text] = grid
         self._myWindow.reloadProperyWindowByGrid(grid)
```

### Comparing `silicon_analyser-1.0.6/silicon_analyser/helper/minimap.py` & `silicon_analyser-1.0.7/silicon_analyser/helper/minimap.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.6/silicon_analyser/helper/properties.py` & `silicon_analyser-1.0.7/silicon_analyser/helper/properties.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,29 +19,34 @@
         if valueCol.column() != 1:
             return
         row = valueCol.row()
         model: QStandardItemModel = typing.cast(QStandardItemModel,self._properties.model())
         nameCol = model.item(row,0)
         name = nameCol.data(Qt.ItemDataRole.DisplayRole)
         value = valueCol.data(Qt.ItemDataRole.DisplayRole)
-        print(name)
-        print(value)
+        print(f"{name}: {value}")
         grid: Grid = self._myWindow.getTree().getSelectedGrid()
         if(name == "cols"):
             grid.cols = int(value)
         if(name == "rows"):
             grid.rows = int(value)
         if(name == "x"):
             grid.x = int(value)
         if(name == "y"):
             grid.y = int(value)
         if(name == "width"):
             grid.width = int(value)
+            grid.recalcCell()
         if(name == "height"):
             grid.height = int(value)
+            grid.recalcCell()
+        if(name == "shearX"):
+            grid.shearX = float(value)
+        if(name == "shearY"):
+            grid.shearY = float(value)
         self._myWindow.getImage().drawImage()
         saveGrids(self._myWindow.getImage().getGrids())
     
     def reloadPropertyWindow(self,selection: QItemSelection):
         table: QTableView = self._properties
         model = table.model()
         model.removeRows(0,model.rowCount())
@@ -52,15 +57,15 @@
         if(len(sel.indexes())==0):
             return
         typeStr = sel.indexes()[0].data(TreeItem.TYPE)
         if(typeStr == TreeItem.TYPE_GRID):
             grid: Grid = sel.indexes()[0].data(TreeItem.OBJECT)
             self.reloadProperyWindowByGrid(grid)
 
-    def reloadProperyWindowByGrid(self, grid):
+    def reloadProperyWindowByGrid(self, grid: Grid):
         table: QTableView = self._properties
         model: QStandardItemModel = typing.cast(QStandardItemModel, table.model())
         rowPosition = model.rowCount()
         model.removeRows(0,model.rowCount())
         model.insertRow(rowPosition,[QStandardItem("name"),QStandardItem(grid.name)])
         if grid is not None:
             rowPosition = model.rowCount()
@@ -71,9 +76,13 @@
             model.insertRow(rowPosition,[QStandardItem("cols"),QStandardItem(f"{grid.cols}")])
             rowPosition = model.rowCount()
             model.insertRow(rowPosition,[QStandardItem("rows"),QStandardItem(f"{grid.rows}")])
             rowPosition = model.rowCount()
             model.insertRow(rowPosition,[QStandardItem("width"),QStandardItem(f"{grid.width}")])
             rowPosition = model.rowCount()
             model.insertRow(rowPosition,[QStandardItem("height"),QStandardItem(f"{grid.height}")])
+            rowPosition = model.rowCount()
+            model.insertRow(rowPosition,[QStandardItem("shearX"),QStandardItem(f"{grid.shearX}")])
+            rowPosition = model.rowCount()
+            model.insertRow(rowPosition,[QStandardItem("shearY"),QStandardItem(f"{grid.shearY}")])
```

### Comparing `silicon_analyser-1.0.6/silicon_analyser/helper/tree.py` & `silicon_analyser-1.0.7/silicon_analyser/helper/tree.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+from PIL import Image
 import typing
+import numpy as np
+import re
 from PyQt5.QtCore import QItemSelection, pyqtSignal, QItemSelectionModel
 from PyQt5 import QtCore
 from PyQt5.QtWidgets import QTreeView, QWidget, QAction, QFileDialog
 from PyQt5.QtGui import QStandardItem, QStandardItemModel
 from silicon_analyser.helper.abstract.abstractmywindow import AbstractMyWindow
 from silicon_analyser.grid import Grid
 from silicon_analyser.helper.abstract.abstracttreehelper import AbstractTreeHelper
@@ -16,14 +19,15 @@
     _actionGridAddRowTop: QAction
     _actionSaveModel: QAction
     _actionLoadModel: QAction
     _actionRemoveGrid: QAction
     _actionRemoveLabel: QAction
     _actionSaveAsCsv: QAction
     _actionViewAsPixelimage: QAction
+    _actionExportCellsToImages: QAction
     _pixelImageDlg: PixelImageDlg
     evtTreeSelectionChanged: pyqtSignal = pyqtSignal(QItemSelection)
 
     def __init__(self, parent: QWidget | None = ...) -> None: # type: ignore
         super().__init__(parent)
     
     def initialize(self, myWindow: AbstractMyWindow):
@@ -32,30 +36,58 @@
         self._actionGridAddRowTop = self._myWindow._actionGridAddRowTop
         self._actionSaveModel = self._myWindow._actionSaveModel
         self._actionLoadModel = self._myWindow._actionLoadModel
         self._actionRemoveGrid = self._myWindow._actionRemoveGrid
         self._actionRemoveLabel = self._myWindow._actionRemoveLabel
         self._actionSaveAsCsv = self._myWindow._actionSaveAsCsv
         self._actionViewAsPixelimage = self._myWindow._actionViewAsPixelimage
+        self._actionExportCellsToImages = self._myWindow._actionExportCellsToImages
         self.addAction(self._actionGridAddRowTop)
         self.addAction(self._actionSaveModel)
         self.addAction(self._actionLoadModel)
         self.addAction(self._actionRemoveGrid)
         self.addAction(self._actionRemoveLabel)
         self.addAction(self._actionSaveAsCsv)
         self.addAction(self._actionViewAsPixelimage)
+        self.addAction(self._actionExportCellsToImages)
         self._actionGridAddRowTop.triggered.connect(self.addTopRow)
         self._actionSaveModel.triggered.connect(self.saveModel)
         self._actionLoadModel.triggered.connect(self.loadModel)
         self._actionRemoveGrid.triggered.connect(self.removeGrid)
         self._actionRemoveLabel.triggered.connect(self.removeLabel)
         self._actionSaveAsCsv.triggered.connect(self.saveAsCsv)
         self._actionViewAsPixelimage.triggered.connect(self.viewAsPixelimage)
+        self._actionExportCellsToImages.triggered.connect(self.exportCellsToImages)
         self._pixelImageDlg = PixelImageDlg()
     
+    def exportCellsToImages(self, *args, **kwargs):
+        print("exportCellsToImages")
+        grid: Grid|None = self.getSelectedGrid()
+        if grid is None:
+            return
+        dlg: QFileDialog = QFileDialog()
+        dlg.setLabelText(QFileDialog.DialogLabel.Accept, "Save")
+        directoryPath: str = dlg.getExistingDirectory()
+        if directoryPath is not None:
+            for label in grid.getLabels():
+                for rect in grid.getRects(label):
+                  x, y = rect[0:2]
+                  w = grid.width / grid.cols
+                  h = grid.height / grid.rows
+                  img: AbstractImage = self._myWindow.getImage()
+                  arr = img.fetchData(grid.absX(x,y),grid.absY(y,x),int(grid.absX(x,y)+w),int(grid.absY(y,x)+h))
+                  clean_label = re.sub("[^A-Za-z0-9]","_",label)
+                  imgArr = np.zeros(arr.shape,np.uint8)
+                  imgArr[:,:,0] = arr[:,:,2]
+                  imgArr[:,:,1] = arr[:,:,1]
+                  imgArr[:,:,2] = arr[:,:,0]
+                  imgToSave = Image.fromarray(imgArr)
+                  imgToSave.save(f"{directoryPath}/{clean_label}_{x:03}_{y:03}.png","PNG")
+        print("exportCellsToImages done")
+
     def viewAsPixelimage(self, *args, **kwargs):
         print("viewAsPixelimage")
         grid: Grid|None
         selectedType = self.selectedType()
         if selectedType == TreeItem.TYPE_GRID_ITEM:
             grid = self.getSelectedGrid()
         elif selectedType == TreeItem.TYPE_AI_GRID_ITEM:
@@ -198,17 +230,19 @@
         else:
             self._actionGridAddRowTop.setVisible(False)
             self._actionSaveModel.setVisible(False)
             self._actionLoadModel.setVisible(False)
         if(selectedType == TreeItem.TYPE_GRID):
             self._actionRemoveGrid.setVisible(True)
             self._actionSaveAsCsv.setVisible(True)
+            self._actionExportCellsToImages.setVisible(True)
         else:
             self._actionRemoveGrid.setVisible(False)
             self._actionSaveAsCsv.setVisible(False)
+            self._actionExportCellsToImages.setVisible(False)
         if(selectedType == TreeItem.TYPE_AI_GRID):
             self._actionSaveAsCsv.setVisible(True)
         else:
             self._actionSaveAsCsv.setVisible(False)
         if(selectedType == TreeItem.TYPE_MANUAL):
             self._actionRemoveLabel.setVisible(True)
         else:
```

### Comparing `silicon_analyser-1.0.6/silicon_analyser/main_window.ui` & `silicon_analyser-1.0.7/silicon_analyser/main_window.ui`

 * *Files 2% similar despite different names*

#### Comparing `silicon_analyser-1.0.6/silicon_analyser/main_window.ui` & `silicon_analyser-1.0.7/silicon_analyser/main_window.ui`

```diff
@@ -208,14 +208,19 @@
       </property>
     </action>
     <action name="_actionViewAsPixelimage">
       <property name="text">
         <string>View as pixelimage</string>
       </property>
     </action>
+    <action name="_actionExportCellsToImages">
+      <property name="text">
+        <string>Export cells to images</string>
+      </property>
+    </action>
   </widget>
   <customwidgets>
     <customwidget>
       <class>ComputeBtn</class>
       <extends>QPushButton</extends>
       <header>silicon_analyser.helper.computebtn</header>
     </customwidget>
```

### Comparing `silicon_analyser-1.0.6/silicon_analyser/mywindow.py` & `silicon_analyser-1.0.7/silicon_analyser/mywindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     _actionLoadModel: QAction
     _actionRemoveGrid: QAction
     _actionRemoveLabel: QAction
     _actionMade_by_TheCrazyT: QAction
     _actionUrl: QAction
     _actionSaveAsCsv: QAction
     _actionViewAsPixelimage: QAction
+    _actionExportCellsToImages: QAction
     autosave: bool
     menuBar: QMenu
     
     def __init__(self):
         AbstractMyWindow.__init__(self)
         path: str = p.abspath(p.join(p.dirname(__file__), '.')) + '/main_window.ui'
         uic.loadUi(path, self)
```

### Comparing `silicon_analyser-1.0.6/silicon_analyser/savefiles.py` & `silicon_analyser-1.0.7/silicon_analyser/savefiles.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,22 @@
             cols = item["cols"]
             rows = item["rows"]
             width = item["width"]
             height = item["height"]
             g: Grid = Grid(name, x , y, cols, rows, width, height)
             g._rects = item["_rects"]
             g._rectsActive = item["_rectsActive"]
+            if "shearX" in item:
+                g.shearX = item["shearX"]
+            else:
+                g.shearX = 0
+            if "shearY" in item:
+                g.shearY = item["shearY"]
+            else:
+                g.shearY = 0
             grids[gridName] = g
         return grids
         
 class MyJSONEncoder(JSONEncoder):
         def default(self, o):
             return o.__dict__
```

### Comparing `silicon_analyser-1.0.6/silicon_analyser/treeitem.py` & `silicon_analyser-1.0.7/silicon_analyser/treeitem.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.6/silicon_analyser.egg-info/PKG-INFO` & `silicon_analyser-1.0.7/silicon_analyser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: silicon-analyser
-Version: 1.0.6
+Version: 1.0.7
 Summary: helps to analyse integrated circuit die images (for example from siliconpr0n.org) with the help of ai.
 Author-email: CrazyT <crazyt2019+sa@gmail.com>
 Project-URL: Homepage, https://github.com/TheCrazyT/SiliconAnalyser
 Project-URL: Bug Tracker, https://github.com/TheCrazyT/SiliconAnalyser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: numpy
+Requires-Dist: pillow
 Requires-Dist: keras
 Requires-Dist: PyQt5
 Requires-Dist: pyqtgraph
 Requires-Dist: scikit-learn
 Requires-Dist: packaging
 
 # Installation
 
 Install from source:
 
-`pip install .`
+`pip install --upgrade .`
 
 Install from pip:
 
-`pip install silicon-analyser`
+`pip install --upgrade silicon-analyser`
 
 # Information
 
 Code will use your graphic card for acceleration.
 (but only if correct pytorch is installed, see "Additional info" below)
 
 Frameworks/Libraries used:
@@ -80,11 +81,12 @@
 * Right click on tree-items (left navigation menu) for additional options
 
 ![image](https://raw.githubusercontent.com/TheCrazyT/SiliconAnalyser/main/docs/small_tutorial.gif)
 
 # TODO
 
 * show loading screen on start (pytorch with cuda support takes a bit to load)
+* option to calculate/classify by decision tree
 * auto-compute to calculate in background while you are selecting new cells for your labels
 * ai-model configuration
 * possibility to rotate grid
 * maybe store your model on a public place? (for others to use)
```

### Comparing `silicon_analyser-1.0.6/silicon_analyser.egg-info/SOURCES.txt` & `silicon_analyser-1.0.7/silicon_analyser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

