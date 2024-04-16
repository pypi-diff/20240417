# Comparing `tmp/leoid-1.1.4.tar.gz` & `tmp/leoid-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leoid-1.1.4.tar", last modified: Tue Apr  2 21:19:50 2024, max compression
+gzip compressed data, was "leoid-1.1.5.tar", last modified: Tue Apr 16 23:00:12 2024, max compression
```

## Comparing `leoid-1.1.4.tar` & `leoid-1.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jayticku   (501) staff       (20)        0 2024-04-02 21:19:50.418295 leoid-1.1.4/
--rw-r--r--   0 jayticku   (501) staff       (20)       19 2024-03-28 19:04:31.000000 leoid-1.1.4/MANIFEST.in
--rw-r--r--   0 jayticku   (501) staff       (20)      844 2024-04-02 21:19:50.418072 leoid-1.1.4/PKG-INFO
--rw-r--r--   0 jayticku   (501) staff       (20)      363 2024-04-02 21:19:20.000000 leoid-1.1.4/README.md
-drwxr-xr-x   0 jayticku   (501) staff       (20)        0 2024-04-02 21:19:50.406624 leoid-1.1.4/leoid/
--rw-r--r--   0 jayticku   (501) staff       (20)       25 2024-03-28 18:09:40.000000 leoid-1.1.4/leoid/__init__.py
--rw-r--r--   0 jayticku   (501) staff       (20)     1192 2024-03-31 22:41:24.000000 leoid-1.1.4/leoid/leoid.py
--rw-r--r--   0 jayticku   (501) staff       (20)   560307 2024-03-28 20:02:00.000000 leoid-1.1.4/leoid/stage_1.pkl
--rw-r--r--   0 jayticku   (501) staff       (20) 10242284 2024-03-28 19:56:06.000000 leoid-1.1.4/leoid/stage_2.pkl
-drwxr-xr-x   0 jayticku   (501) staff       (20)        0 2024-04-02 21:19:50.417852 leoid-1.1.4/leoid.egg-info/
--rw-r--r--   0 jayticku   (501) staff       (20)      844 2024-04-02 21:19:50.000000 leoid-1.1.4/leoid.egg-info/PKG-INFO
--rw-r--r--   0 jayticku   (501) staff       (20)      243 2024-04-02 21:19:50.000000 leoid-1.1.4/leoid.egg-info/SOURCES.txt
--rw-r--r--   0 jayticku   (501) staff       (20)        1 2024-04-02 21:19:50.000000 leoid-1.1.4/leoid.egg-info/dependency_links.txt
--rw-r--r--   0 jayticku   (501) staff       (20)       61 2024-04-02 21:19:50.000000 leoid-1.1.4/leoid.egg-info/requires.txt
--rw-r--r--   0 jayticku   (501) staff       (20)        6 2024-04-02 21:19:50.000000 leoid-1.1.4/leoid.egg-info/top_level.txt
--rw-r--r--   0 jayticku   (501) staff       (20)       38 2024-04-02 21:19:50.418343 leoid-1.1.4/setup.cfg
--rw-r--r--   0 jayticku   (501) staff       (20)      774 2024-04-02 21:19:34.000000 leoid-1.1.4/setup.py
+drwxr-xr-x   0 jayticku   (501) staff       (20)        0 2024-04-16 23:00:12.522822 leoid-1.1.5/
+-rw-r--r--   0 jayticku   (501) staff       (20)       19 2024-03-28 19:04:31.000000 leoid-1.1.5/MANIFEST.in
+-rw-r--r--   0 jayticku   (501) staff       (20)      876 2024-04-16 23:00:12.522613 leoid-1.1.5/PKG-INFO
+-rw-r--r--   0 jayticku   (501) staff       (20)      363 2024-04-02 21:19:20.000000 leoid-1.1.5/README.md
+drwxr-xr-x   0 jayticku   (501) staff       (20)        0 2024-04-16 23:00:12.511701 leoid-1.1.5/leoid/
+-rw-r--r--   0 jayticku   (501) staff       (20)       25 2024-03-28 18:09:40.000000 leoid-1.1.5/leoid/__init__.py
+-rw-r--r--   0 jayticku   (501) staff       (20)     1437 2024-04-16 22:59:07.000000 leoid-1.1.5/leoid/leoid.py
+-rw-r--r--   0 jayticku   (501) staff       (20)   560307 2024-03-28 20:02:00.000000 leoid-1.1.5/leoid/stage_1.pkl
+-rw-r--r--   0 jayticku   (501) staff       (20) 10242284 2024-03-28 19:56:06.000000 leoid-1.1.5/leoid/stage_2.pkl
+drwxr-xr-x   0 jayticku   (501) staff       (20)        0 2024-04-16 23:00:12.522367 leoid-1.1.5/leoid.egg-info/
+-rw-r--r--   0 jayticku   (501) staff       (20)      876 2024-04-16 23:00:12.000000 leoid-1.1.5/leoid.egg-info/PKG-INFO
+-rw-r--r--   0 jayticku   (501) staff       (20)      243 2024-04-16 23:00:12.000000 leoid-1.1.5/leoid.egg-info/SOURCES.txt
+-rw-r--r--   0 jayticku   (501) staff       (20)        1 2024-04-16 23:00:12.000000 leoid-1.1.5/leoid.egg-info/dependency_links.txt
+-rw-r--r--   0 jayticku   (501) staff       (20)       78 2024-04-16 23:00:12.000000 leoid-1.1.5/leoid.egg-info/requires.txt
+-rw-r--r--   0 jayticku   (501) staff       (20)        6 2024-04-16 23:00:12.000000 leoid-1.1.5/leoid.egg-info/top_level.txt
+-rw-r--r--   0 jayticku   (501) staff       (20)       38 2024-04-16 23:00:12.523494 leoid-1.1.5/setup.cfg
+-rw-r--r--   0 jayticku   (501) staff       (20)      802 2024-04-16 22:58:20.000000 leoid-1.1.5/setup.py
```

### Comparing `leoid-1.1.4/PKG-INFO` & `leoid-1.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: leoid
-Version: 1.1.4
+Version: 1.1.5
 Summary: LEOID Python Package
 Author: Jay Ticku
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: imbalanced-learn==0.12.0
 Requires-Dist: scikit-learn==1.2.2
 Requires-Dist: lightgbm==4.2.0
+Requires-Dist: aiofiles==23.2.1
 
 ## Python Package for Machine Learning Model LEOID (Level-based Ensemble for Overcoming Imbalanced Data)
 \
 More information about LEOID and example usage is available on Kaggle. [www.kaggle.com/models/jayticku/leoid](https://www.kaggle.com/models/jayticku/leoid)
 \
 To see LEOID in action, go to [www.diabetes-predictor.com](https://www.diabetes-predictor.com).
```

### Comparing `leoid-1.1.4/leoid/leoid.py` & `leoid-1.1.5/leoid/leoid.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 import pickle
 import numpy as np
 import os
+import asyncio
+import aiofiles
 import imblearn
 
 class LEOID():
     """Level-based Ensemble for Overcoming Imbalanced Data"""
 
     def __init__(self):
+        asyncio.run(self._load_models())
+
+    async def _load_models(self):
         current_dir = os.path.dirname(__file__)
         stage_1_path = os.path.join(current_dir, "stage_1.pkl")
         stage_2_path = os.path.join(current_dir, "stage_2.pkl")
+    
+        async with aiofiles.open(stage_1_path, "rb") as f:
+            model_1_data = await f.read()
+            self.model_1 = pickle.loads(model_1_data)
 
-        with open(stage_1_path, "rb") as f:
-            self.model_1 = pickle.load(f)
+        async with aiofiles.open(stage_2_path, "rb") as f:
+            model_2_data = await f.read()
+            self.model_2 = pickle.loads(model_2_data)
 
-        with open(stage_2_path, "rb") as f:
-            self.model_2 = pickle.load(f)
-    
     def predict(self, X):
         X = np.array(X)
         if X.ndim == 1:
             X = X.reshape(1, -1)
             
         model_1_predictions = self.model_1.predict(X)
         predictions = []
```

### Comparing `leoid-1.1.4/leoid/stage_1.pkl` & `leoid-1.1.5/leoid/stage_1.pkl`

 * *Files identical despite different names*

### Comparing `leoid-1.1.4/leoid/stage_2.pkl` & `leoid-1.1.5/leoid/stage_2.pkl`

 * *Files identical despite different names*

### Comparing `leoid-1.1.4/leoid.egg-info/PKG-INFO` & `leoid-1.1.5/leoid.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: leoid
-Version: 1.1.4
+Version: 1.1.5
 Summary: LEOID Python Package
 Author: Jay Ticku
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: imbalanced-learn==0.12.0
 Requires-Dist: scikit-learn==1.2.2
 Requires-Dist: lightgbm==4.2.0
+Requires-Dist: aiofiles==23.2.1
 
 ## Python Package for Machine Learning Model LEOID (Level-based Ensemble for Overcoming Imbalanced Data)
 \
 More information about LEOID and example usage is available on Kaggle. [www.kaggle.com/models/jayticku/leoid](https://www.kaggle.com/models/jayticku/leoid)
 \
 To see LEOID in action, go to [www.diabetes-predictor.com](https://www.diabetes-predictor.com).
```

### Comparing `leoid-1.1.4/setup.py` & `leoid-1.1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name = 'leoid',
-    version = '1.1.4',
+    version = '1.1.5',
     author = 'Jay Ticku',
     description = 'LEOID Python Package',
     long_description = long_description,
     long_description_content_type='text/markdown',
     install_requires = [
         'imbalanced-learn==0.12.0',
         'scikit-learn==1.2.2',
-        'lightgbm==4.2.0'
+        'lightgbm==4.2.0',
+        'aiofiles==23.2.1'
     ],
     classifiers=[
     'Development Status :: 5 - Production/Stable',
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: Apache Software License',
     'Operating System :: OS Independent',
     ],
```

