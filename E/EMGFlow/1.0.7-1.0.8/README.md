# Comparing `tmp/emgflow-1.0.7.tar.gz` & `tmp/emgflow-1.0.8.tar.gz`

## Comparing `emgflow-1.0.7.tar` & `emgflow-1.0.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 emgflow-1.0.7/src/EMGFlow/OutlierFinder.py
--rw-r--r--   0        0        0     8818 2020-02-02 00:00:00.000000 emgflow-1.0.7/src/EMGFlow/PlotSignals.py
--rw-r--r--   0        0        0    49356 2020-02-02 00:00:00.000000 emgflow-1.0.7/src/EMGFlow/SignalFilterer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 emgflow-1.0.7/src/EMGFlow/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 emgflow-1.0.7/.gitignore
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 emgflow-1.0.7/README.md
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 emgflow-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 emgflow-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     6070 2020-02-02 00:00:00.000000 emgflow-1.0.8/src/EMGFlow/OutlierFinder.py
+-rw-r--r--   0        0        0     8819 2020-02-02 00:00:00.000000 emgflow-1.0.8/src/EMGFlow/PlotSignals.py
+-rw-r--r--   0        0        0    49356 2020-02-02 00:00:00.000000 emgflow-1.0.8/src/EMGFlow/SignalFilterer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 emgflow-1.0.8/src/EMGFlow/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 emgflow-1.0.8/.gitignore
+-rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 emgflow-1.0.8/README.md
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 emgflow-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 emgflow-1.0.8/PKG-INFO
```

### Comparing `emgflow-1.0.7/src/EMGFlow/OutlierFinder.py` & `emgflow-1.0.8/src/EMGFlow/OutlierFinder.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 import scipy.optimize
 import os
 import re
 from scipy.signal import argrelextrema
 from tqdm import tqdm
 
-from SignalFilterer import MapFiles, EMG2PSD
+from .SignalFilterer import MapFiles, EMG2PSD
 
 #
 # =============================================================================
 #
 
 """
 A collection of functions for finding outliers while testing
```

### Comparing `emgflow-1.0.7/src/EMGFlow/PlotSignals.py` & `emgflow-1.0.8/src/EMGFlow/PlotSignals.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import matplotlib.pyplot as plt
 import random
 import webbrowser
 from tqdm import tqdm
 
 from shiny import App, render, ui
 
-from SignalFilterer import ConvertMapFiles, MapFilesFuse, EMG2PSD
+from .SignalFilterer import ConvertMapFiles, MapFilesFuse, EMG2PSD
 
 #
 # =============================================================================
 #
 
 """
 A collection of functions for plotting subject data
```

### Comparing `emgflow-1.0.7/src/EMGFlow/SignalFilterer.py` & `emgflow-1.0.8/src/EMGFlow/SignalFilterer.py`

 * *Files identical despite different names*

### Comparing `emgflow-1.0.7/README.md` & `emgflow-1.0.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -73,11 +73,11 @@
 
 ```bibtex
 @software{Conley_EMGFlow_2024,
   author = {Conley {\tt william@cconley.ca}, William and Livingstone, Steven R},
   month = {03},
   title = {{EMGFlow Package}},
   url = {https://github.com/WiIIson/EMGFlow-Python-Package},
-  version = {1.0.7},
+  version = {1.0.8},
   year = {2024}
 }
 ```
```

### Comparing `emgflow-1.0.7/pyproject.toml` & `emgflow-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "EMGFlow"
-version = "1.0.7"
+version = "1.0.8"
 dependencies = [
     "pandas",
     "numpy",
     "scipy",
     "matplotlib",
     "opencv-python", 
     "tqdm",
```

### Comparing `emgflow-1.0.7/PKG-INFO` & `emgflow-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: EMGFlow
-Version: 1.0.7
+Version: 1.0.8
 Summary: A general EMG processing and feature extraction package.
 Project-URL: Home, https://github.com/WiIIson/EMGFlow-Python-Package
 Author-email: William Conley and Steven Livingstone <william@cconley.ca>
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
@@ -93,11 +93,11 @@
 
 ```bibtex
 @software{Conley_EMGFlow_2024,
   author = {Conley {\tt william@cconley.ca}, William and Livingstone, Steven R},
   month = {03},
   title = {{EMGFlow Package}},
   url = {https://github.com/WiIIson/EMGFlow-Python-Package},
-  version = {1.0.7},
+  version = {1.0.8},
   year = {2024}
 }
 ```
```

