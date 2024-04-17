# Comparing `tmp/ilastik-napari-0.2.3.tar.gz` & `tmp/ilastik_napari-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilastik-napari-0.2.3.tar", last modified: Fri Jun  9 11:12:54 2023, max compression
+gzip compressed data, was "ilastik_napari-0.2.4.tar", last modified: Wed Apr 17 10:05:50 2024, max compression
```

## Comparing `ilastik-napari-0.2.3.tar` & `ilastik_napari-0.2.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:12:54.704064 ilastik-napari-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-09 11:12:43.000000 ilastik-napari-0.2.3/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:12:54.696064 ilastik-napari-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:12:54.700064 ilastik-napari-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-09 11:12:43.000000 ilastik-napari-0.2.3/.github/workflows/build-upload.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-09 11:12:43.000000 ilastik-napari-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-09 11:12:43.000000 ilastik-napari-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-06-09 11:12:54.700064 ilastik-napari-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-06-09 11:12:43.000000 ilastik-napari-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:12:54.700064 ilastik-napari-0.2.3/conda-recipe/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-09 11:12:43.000000 ilastik-napari-0.2.3/conda-recipe/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:12:54.700064 ilastik-napari-0.2.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-09 11:12:43.000000 ilastik-napari-0.2.3/examples/simple_labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-09 11:12:43.000000 ilastik-napari-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 11:12:54.704064 ilastik-napari-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-09 11:12:43.000000 ilastik-napari-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:12:54.696064 ilastik-napari-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:12:54.696064 ilastik-napari-0.2.3/src/ilastik/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:12:54.700064 ilastik-napari-0.2.3/src/ilastik/napari/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-09 11:12:43.000000 ilastik-napari-0.2.3/src/ilastik/napari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-09 11:12:43.000000 ilastik-napari-0.2.3/src/ilastik/napari/classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-09 11:12:43.000000 ilastik-napari-0.2.3/src/ilastik/napari/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-09 11:12:43.000000 ilastik-napari-0.2.3/src/ilastik/napari/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-06-09 11:12:43.000000 ilastik-napari-0.2.3/src/ilastik/napari/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-09 11:12:43.000000 ilastik-napari-0.2.3/src/ilastik/napari/plugin.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:12:54.700064 ilastik-napari-0.2.3/src/ilastik_napari.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-06-09 11:12:54.000000 ilastik-napari-0.2.3/src/ilastik_napari.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-09 11:12:54.000000 ilastik-napari-0.2.3/src/ilastik_napari.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 11:12:54.000000 ilastik-napari-0.2.3/src/ilastik_napari.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-09 11:12:54.000000 ilastik-napari-0.2.3/src/ilastik_napari.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-09 11:12:54.000000 ilastik-napari-0.2.3/src/ilastik_napari.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 11:12:54.000000 ilastik-napari-0.2.3/src/ilastik_napari.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:50.828374 ilastik_napari-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-17 10:05:46.000000 ilastik_napari-0.2.4/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:50.824374 ilastik_napari-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:50.824374 ilastik_napari-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-17 10:05:46.000000 ilastik_napari-0.2.4/.github/workflows/build-upload.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-17 10:05:46.000000 ilastik_napari-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-17 10:05:46.000000 ilastik_napari-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-04-17 10:05:50.828374 ilastik_napari-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-04-17 10:05:46.000000 ilastik_napari-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:50.828374 ilastik_napari-0.2.4/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-17 10:05:46.000000 ilastik_napari-0.2.4/conda-recipe/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:50.828374 ilastik_napari-0.2.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-17 10:05:46.000000 ilastik_napari-0.2.4/examples/simple_labeling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-17 10:05:46.000000 ilastik_napari-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 10:05:50.828374 ilastik_napari-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-17 10:05:46.000000 ilastik_napari-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:50.824374 ilastik_napari-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:50.824374 ilastik_napari-0.2.4/src/ilastik/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:50.828374 ilastik_napari-0.2.4/src/ilastik/napari/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-17 10:05:46.000000 ilastik_napari-0.2.4/src/ilastik/napari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-17 10:05:46.000000 ilastik_napari-0.2.4/src/ilastik/napari/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-17 10:05:46.000000 ilastik_napari-0.2.4/src/ilastik/napari/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-17 10:05:46.000000 ilastik_napari-0.2.4/src/ilastik/napari/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-17 10:05:46.000000 ilastik_napari-0.2.4/src/ilastik/napari/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-17 10:05:46.000000 ilastik_napari-0.2.4/src/ilastik/napari/plugin.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:05:50.828374 ilastik_napari-0.2.4/src/ilastik_napari.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-04-17 10:05:50.000000 ilastik_napari-0.2.4/src/ilastik_napari.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-17 10:05:50.000000 ilastik_napari-0.2.4/src/ilastik_napari.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 10:05:50.000000 ilastik_napari-0.2.4/src/ilastik_napari.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-17 10:05:50.000000 ilastik_napari-0.2.4/src/ilastik_napari.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-17 10:05:50.000000 ilastik_napari-0.2.4/src/ilastik_napari.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 10:05:50.000000 ilastik_napari-0.2.4/src/ilastik_napari.egg-info/top_level.txt
```

### Comparing `ilastik-napari-0.2.3/LICENSE` & `ilastik_napari-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ilastik-napari-0.2.3/PKG-INFO` & `ilastik_napari-0.2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilastik-napari
-Version: 0.2.3
+Version: 0.2.4
 Summary: ilastik plugin for napari
 Author-email: Emil Melnikov <emilmelnikov@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/ilastik/ilastik-napari
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: End Users/Desktop
@@ -20,14 +20,19 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: napari>=0.4.13
+Requires-Dist: numpy>=1.20
+Requires-Dist: qtpy
+Requires-Dist: scikit-learn
+Requires-Dist: sparse
 
 # ilastik-napari
 
 [Napari][napari] plugin for interactive pixel classification.
 Designed to be similar to the pixel classification workflow in [classic ilastik][ilastik].
 
 ## Installation
```

### Comparing `ilastik-napari-0.2.3/README.md` & `ilastik_napari-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `ilastik-napari-0.2.3/conda-recipe/meta.yaml` & `ilastik_napari-0.2.4/conda-recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `ilastik-napari-0.2.3/examples/simple_labeling.py` & `ilastik_napari-0.2.4/examples/simple_labeling.py`

 * *Files identical despite different names*

### Comparing `ilastik-napari-0.2.3/pyproject.toml` & `ilastik_napari-0.2.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Image Processing",
 ]
 dependencies = [
-    "napari",
+    "napari>=0.4.13",
     "numpy>=1.20",
     "qtpy",
     "scikit-learn",
     "sparse",
 ]
 dynamic = ["version"]
```

### Comparing `ilastik-napari-0.2.3/src/ilastik/napari/classifier.py` & `ilastik_napari-0.2.4/src/ilastik/napari/classifier.py`

 * *Files identical despite different names*

### Comparing `ilastik-napari-0.2.3/src/ilastik/napari/filters.py` & `ilastik_napari-0.2.4/src/ilastik/napari/filters.py`

 * *Files identical despite different names*

### Comparing `ilastik-napari-0.2.3/src/ilastik/napari/gui.py` & `ilastik_napari-0.2.4/src/ilastik/napari/gui.py`

 * *Files identical despite different names*

### Comparing `ilastik-napari-0.2.3/src/ilastik/napari/plugin.py` & `ilastik_napari-0.2.4/src/ilastik/napari/plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Any
 
 import numpy
 import sparse
+from PyQt5.QtGui import QStandardItemModel, QStandardItem
 from napari import Viewer
-from napari._qt.containers import QtLayerList
+from napari.components import LayerList
 from napari.layers import Image, Labels, Layer
 from napari.qt.threading import thread_worker
 from qtpy.QtCore import QModelIndex, QSortFilterProxyModel, Qt
 from qtpy.QtWidgets import (
     QCheckBox,
     QComboBox,
     QFormLayout,
@@ -50,17 +51,21 @@
     filters.StructureTensorEigenvalues,
     filters.HessianOfGaussianEigenvalues,
 )
 scale_list = (0.3, 0.7, 1.0, 1.6, 3.5, 5.0, 10.0)
 
 
 class LayerModel(QSortFilterProxyModel):
-    def __init__(self, layers: QtLayerList, parent=None):
+    def __init__(self, layers: LayerList, parent=None):
         super().__init__(parent)
-        self.setSourceModel(layers)
+        self.setSourceModel(QStandardItemModel())
+        self.napari_layers = layers
+        self.update_model()
+        self.napari_layers.events.inserted.connect(self.update_model)
+        self.napari_layers.events.removed.connect(self.update_model)
 
     def filterAcceptsRow(self, row: int, parent: QModelIndex) -> bool:
         model = self.sourceModel()
         index = model.index(row, self.filterKeyColumn(), parent)
         layer = model.data(index, Qt.UserRole)
         return self.should_accept_layer(layer)
 
@@ -68,14 +73,22 @@
         return True
 
     def data(self, index: QModelIndex, role: int = Qt.DisplayRole) -> Any:
         if role in (Qt.DisplayRole, Qt.DecorationRole, Qt.UserRole):
             return super().data(index, role)
         return None
 
+    def update_model(self):
+        model = self.sourceModel()
+        model.clear()
+        for layer in self.napari_layers:
+            item = QStandardItem(layer.name)
+            item.setData(layer, Qt.UserRole)
+            model.appendRow(item)
+
 
 class ImageLayerModel(LayerModel):
     def should_accept_layer(self, layer: Layer) -> bool:
         return isinstance(layer, Image) and not isinstance(layer, Labels)
 
 
 class LabelsLayerModel(LayerModel):
@@ -86,15 +99,15 @@
 class PixelClassificationWidget(QWidget):
     SEG_LAYER_PARAMS = dict(name="ilastik-segmentation", opacity=1)
     PROBA_LAYER_PARAMS = dict(name="ilastik-probabilities", opacity=0.75)
 
     def __init__(self, napari_viewer: Viewer, parent=None):
         super().__init__(parent)
 
-        layer_model = napari_viewer.window.qt_viewer.layers.model()
+        layer_model = napari_viewer.layers
 
         image_combo = QComboBox()
         image_combo.setModel(ImageLayerModel(layer_model, self))
         image_combo.currentIndexChanged.connect(lambda _index: self._update_widgets())
 
         labels_combo = QComboBox()
         labels_combo.setModel(LabelsLayerModel(layer_model, self))
```

### Comparing `ilastik-napari-0.2.3/src/ilastik_napari.egg-info/PKG-INFO` & `ilastik_napari-0.2.4/src/ilastik_napari.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilastik-napari
-Version: 0.2.3
+Version: 0.2.4
 Summary: ilastik plugin for napari
 Author-email: Emil Melnikov <emilmelnikov@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/ilastik/ilastik-napari
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: End Users/Desktop
@@ -20,14 +20,19 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: napari>=0.4.13
+Requires-Dist: numpy>=1.20
+Requires-Dist: qtpy
+Requires-Dist: scikit-learn
+Requires-Dist: sparse
 
 # ilastik-napari
 
 [Napari][napari] plugin for interactive pixel classification.
 Designed to be similar to the pixel classification workflow in [classic ilastik][ilastik].
 
 ## Installation
```

### Comparing `ilastik-napari-0.2.3/src/ilastik_napari.egg-info/SOURCES.txt` & `ilastik_napari-0.2.4/src/ilastik_napari.egg-info/SOURCES.txt`

 * *Files identical despite different names*

