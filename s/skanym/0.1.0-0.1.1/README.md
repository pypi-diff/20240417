# Comparing `tmp/skanym-0.1.0.tar.gz` & `tmp/skanym-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skanym-0.1.0.tar", last modified: Thu Apr 11 09:18:07 2024, max compression
+gzip compressed data, was "skanym-0.1.1.tar", last modified: Wed Apr 17 12:29:28 2024, max compression
```

## Comparing `skanym-0.1.0.tar` & `skanym-0.1.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 09:18:07.836931 skanym-0.1.0/
--rw-rw-rw-   0        0        0     1090 2023-11-07 12:29:13.000000 skanym-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     2425 2024-04-11 09:18:07.832898 skanym-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-11-21 09:04:08.000000 skanym-0.1.0/README.md
--rw-rw-rw-   0        0        0     1077 2024-04-08 11:54:24.000000 skanym-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-11 09:18:07.837942 skanym-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-11 09:18:06.925871 skanym-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-11 09:18:06.961786 skanym-0.1.0/src/skanym/
--rw-rw-rw-   0        0        0        0 2024-04-08 11:54:24.000000 skanym-0.1.0/src/skanym/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:18:07.118103 skanym-0.1.0/src/skanym/animators/
--rw-rw-rw-   0        0        0        0 2024-04-08 11:54:24.000000 skanym-0.1.0/src/skanym/animators/__init__.py
--rw-rw-rw-   0        0        0     2315 2024-04-10 13:40:13.000000 skanym-0.1.0/src/skanym/animators/baseAnimator.py
--rw-rw-rw-   0        0        0    10365 2024-04-10 13:40:13.000000 skanym-0.1.0/src/skanym/animators/baseFkAnimator.py
--rw-rw-rw-   0        0        0     2019 2024-04-10 13:40:13.000000 skanym-0.1.0/src/skanym/animators/globalFkAnimator.py
--rw-rw-rw-   0        0        0     1391 2024-04-10 13:40:13.000000 skanym-0.1.0/src/skanym/animators/localFkAnimator.py
--rw-rw-rw-   0        0        0     9316 2024-04-10 13:40:13.000000 skanym-0.1.0/src/skanym/animators/pcaAnimator.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:18:07.180815 skanym-0.1.0/src/skanym/loaders/
--rw-rw-rw-   0        0        0        0 2024-04-08 11:54:24.000000 skanym-0.1.0/src/skanym/loaders/__init__.py
--rw-rw-rw-   0        0        0    10632 2024-04-11 09:17:24.000000 skanym-0.1.0/src/skanym/loaders/fbxLoader.py
--rw-rw-rw-   0        0        0     7899 2024-04-08 11:54:24.000000 skanym-0.1.0/src/skanym/loaders/glbLoader.py
--rw-rw-rw-   0        0        0      655 2024-04-08 11:54:24.000000 skanym-0.1.0/src/skanym/loaders/iFileLoader.py
--rw-rw-rw-   0        0        0      423 2024-04-08 11:54:24.000000 skanym-0.1.0/src/skanym/loaders/objectLoader.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:18:07.185338 skanym-0.1.0/src/skanym/structures/
--rw-rw-rw-   0        0        0        0 2024-04-08 11:54:24.000000 skanym-0.1.0/src/skanym/structures/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:18:07.328876 skanym-0.1.0/src/skanym/structures/animation/
--rw-rw-rw-   0        0        0        0 2024-04-08 11:54:24.000000 skanym-0.1.0/src/skanym/structures/animation/__init__.py
--rw-rw-rw-   0        0        0     1644 2024-04-10 13:40:13.000000 skanym-0.1.0/src/skanym/structures/animation/animation.py
--rw-rw-rw-   0        0        0      547 2024-04-08 11:54:24.000000 skanym-0.1.0/src/skanym/structures/animation/animationCurve.py
--rw-rw-rw-   0        0        0     2041 2024-04-08 11:54:24.000000 skanym-0.1.0/src/skanym/structures/animation/iCurve.py
--rw-rw-rw-   0        0        0      890 2024-04-08 11:54:24.000000 skanym-0.1.0/src/skanym/structures/animation/key.py
--rw-rw-rw-   0        0        0     1146 2024-04-10 13:40:13.000000 skanym-0.1.0/src/skanym/structures/animation/positionCurve.py
--rw-rw-rw-   0        0        0     1208 2024-04-10 13:40:13.000000 skanym-0.1.0/src/skanym/structures/animation/quaternionCurve.py
--rw-rw-rw-   0        0        0      784 2024-04-08 11:54:24.000000 skanym-0.1.0/src/skanym/structures/animation/scalarCurve.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:18:07.375085 skanym-0.1.0/src/skanym/structures/character/
--rw-rw-rw-   0        0        0        0 2024-04-08 11:54:24.000000 skanym-0.1.0/src/skanym/structures/character/__init__.py
--rw-rw-rw-   0        0        0     5439 2024-04-10 13:40:13.000000 skanym-0.1.0/src/skanym/structures/character/joint.py
--rw-rw-rw-   0        0        0     4233 2024-04-10 13:40:13.000000 skanym-0.1.0/src/skanym/structures/character/skeleton.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:18:07.451118 skanym-0.1.0/src/skanym/structures/data/
--rw-rw-rw-   0        0        0        0 2024-04-10 13:40:13.000000 skanym-0.1.0/src/skanym/structures/data/__init__.py
--rw-rw-rw-   0        0        0      771 2024-04-10 13:40:13.000000 skanym-0.1.0/src/skanym/structures/data/iTransform.py
--rw-rw-rw-   0        0        0     1305 2024-04-10 13:40:13.000000 skanym-0.1.0/src/skanym/structures/data/transform.py
--rw-rw-rw-   0        0        0     1179 2024-04-10 13:40:13.000000 skanym-0.1.0/src/skanym/structures/data/transformMatrix.py
--rw-rw-rw-   0        0        0     2305 2024-04-10 13:40:13.000000 skanym-0.1.0/src/skanym/structures/data/vectorizedArray.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:18:07.478515 skanym-0.1.0/src/skanym/utils/
--rw-rw-rw-   0        0        0        0 2024-03-20 13:33:29.000000 skanym-0.1.0/src/skanym/utils/__init__.py
--rw-rw-rw-   0        0        0    10909 2024-04-09 13:24:52.000000 skanym-0.1.0/src/skanym/utils/conversion.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:18:07.818353 skanym-0.1.0/src/skanym/utils/fbx_bindings/
--rw-rw-rw-   0        0        0     3075 2023-11-07 11:28:47.000000 skanym-0.1.0/src/skanym/utils/fbx_bindings/FbxCommon.py
--rw-rw-rw-   0        0        0        0 2024-03-19 18:17:16.000000 skanym-0.1.0/src/skanym/utils/fbx_bindings/__init__.py
--rw-rw-rw-   0        0        0  9286144 2023-11-07 11:28:47.000000 skanym-0.1.0/src/skanym/utils/fbx_bindings/fbx.pyd
--rw-rw-rw-   0        0        0   105472 2023-11-07 11:28:47.000000 skanym-0.1.0/src/skanym/utils/fbx_bindings/sip.pyd
-drwxrwxrwx   0        0        0        0 2024-04-11 09:18:07.827807 skanym-0.1.0/src/skanym.egg-info/
--rw-rw-rw-   0        0        0     2425 2024-04-11 09:18:06.000000 skanym-0.1.0/src/skanym.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1581 2024-04-11 09:18:06.000000 skanym-0.1.0/src/skanym.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 09:18:06.000000 skanym-0.1.0/src/skanym.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2024-04-11 09:18:06.000000 skanym-0.1.0/src/skanym.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-11 09:18:06.000000 skanym-0.1.0/src/skanym.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 12:29:28.027674 skanym-0.1.1/
+-rw-rw-rw-   0        0        0     1090 2023-11-07 12:29:13.000000 skanym-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     2425 2024-04-17 12:29:28.024524 skanym-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-11-21 09:04:08.000000 skanym-0.1.1/README.md
+-rw-rw-rw-   0        0        0     1077 2024-04-17 12:29:03.000000 skanym-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-17 12:29:28.027674 skanym-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 12:29:27.679499 skanym-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-17 12:29:27.700057 skanym-0.1.1/src/skanym/
+-rw-rw-rw-   0        0        0        0 2024-04-08 11:54:24.000000 skanym-0.1.1/src/skanym/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:29:27.736803 skanym-0.1.1/src/skanym/animators/
+-rw-rw-rw-   0        0        0        0 2024-04-08 11:54:24.000000 skanym-0.1.1/src/skanym/animators/__init__.py
+-rw-rw-rw-   0        0        0     2315 2024-04-16 12:41:55.000000 skanym-0.1.1/src/skanym/animators/baseAnimator.py
+-rw-rw-rw-   0        0        0    10365 2024-04-10 13:40:13.000000 skanym-0.1.1/src/skanym/animators/baseFkAnimator.py
+-rw-rw-rw-   0        0        0     2019 2024-04-10 13:40:13.000000 skanym-0.1.1/src/skanym/animators/globalFkAnimator.py
+-rw-rw-rw-   0        0        0     1391 2024-04-10 13:40:13.000000 skanym-0.1.1/src/skanym/animators/localFkAnimator.py
+-rw-rw-rw-   0        0        0     9332 2024-04-16 13:47:14.000000 skanym-0.1.1/src/skanym/animators/pcaAnimator.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:29:27.754565 skanym-0.1.1/src/skanym/loaders/
+-rw-rw-rw-   0        0        0        0 2024-04-08 11:54:24.000000 skanym-0.1.1/src/skanym/loaders/__init__.py
+-rw-rw-rw-   0        0        0    10632 2024-04-17 12:28:36.000000 skanym-0.1.1/src/skanym/loaders/fbxLoader.py
+-rw-rw-rw-   0        0        0     7899 2024-04-08 11:54:24.000000 skanym-0.1.1/src/skanym/loaders/glbLoader.py
+-rw-rw-rw-   0        0        0      655 2024-04-08 11:54:24.000000 skanym-0.1.1/src/skanym/loaders/iFileLoader.py
+-rw-rw-rw-   0        0        0      423 2024-04-08 11:54:24.000000 skanym-0.1.1/src/skanym/loaders/objectLoader.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:29:27.758606 skanym-0.1.1/src/skanym/structures/
+-rw-rw-rw-   0        0        0        0 2024-04-08 11:54:24.000000 skanym-0.1.1/src/skanym/structures/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:29:27.786856 skanym-0.1.1/src/skanym/structures/animation/
+-rw-rw-rw-   0        0        0        0 2024-04-08 11:54:24.000000 skanym-0.1.1/src/skanym/structures/animation/__init__.py
+-rw-rw-rw-   0        0        0     1644 2024-04-10 13:40:13.000000 skanym-0.1.1/src/skanym/structures/animation/animation.py
+-rw-rw-rw-   0        0        0      547 2024-04-08 11:54:24.000000 skanym-0.1.1/src/skanym/structures/animation/animationCurve.py
+-rw-rw-rw-   0        0        0     2041 2024-04-08 11:54:24.000000 skanym-0.1.1/src/skanym/structures/animation/iCurve.py
+-rw-rw-rw-   0        0        0      890 2024-04-08 11:54:24.000000 skanym-0.1.1/src/skanym/structures/animation/key.py
+-rw-rw-rw-   0        0        0     1146 2024-04-10 13:40:13.000000 skanym-0.1.1/src/skanym/structures/animation/positionCurve.py
+-rw-rw-rw-   0        0        0     1208 2024-04-10 13:40:13.000000 skanym-0.1.1/src/skanym/structures/animation/quaternionCurve.py
+-rw-rw-rw-   0        0        0      784 2024-04-08 11:54:24.000000 skanym-0.1.1/src/skanym/structures/animation/scalarCurve.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:29:27.797365 skanym-0.1.1/src/skanym/structures/character/
+-rw-rw-rw-   0        0        0        0 2024-04-08 11:54:24.000000 skanym-0.1.1/src/skanym/structures/character/__init__.py
+-rw-rw-rw-   0        0        0     5439 2024-04-10 13:40:13.000000 skanym-0.1.1/src/skanym/structures/character/joint.py
+-rw-rw-rw-   0        0        0     4233 2024-04-10 13:40:13.000000 skanym-0.1.1/src/skanym/structures/character/skeleton.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:29:27.816887 skanym-0.1.1/src/skanym/structures/data/
+-rw-rw-rw-   0        0        0        0 2024-04-10 13:40:13.000000 skanym-0.1.1/src/skanym/structures/data/__init__.py
+-rw-rw-rw-   0        0        0      771 2024-04-10 13:40:13.000000 skanym-0.1.1/src/skanym/structures/data/iTransform.py
+-rw-rw-rw-   0        0        0     1305 2024-04-10 13:40:13.000000 skanym-0.1.1/src/skanym/structures/data/transform.py
+-rw-rw-rw-   0        0        0     1179 2024-04-10 13:40:13.000000 skanym-0.1.1/src/skanym/structures/data/transformMatrix.py
+-rw-rw-rw-   0        0        0     2305 2024-04-10 13:40:13.000000 skanym-0.1.1/src/skanym/structures/data/vectorizedArray.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:29:27.823702 skanym-0.1.1/src/skanym/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-20 13:33:29.000000 skanym-0.1.1/src/skanym/utils/__init__.py
+-rw-rw-rw-   0        0        0    10909 2024-04-09 13:24:52.000000 skanym-0.1.1/src/skanym/utils/conversion.py
+drwxrwxrwx   0        0        0        0 2024-04-17 12:29:28.013246 skanym-0.1.1/src/skanym/utils/fbx_bindings/
+-rw-rw-rw-   0        0        0     3075 2023-11-07 11:28:47.000000 skanym-0.1.1/src/skanym/utils/fbx_bindings/FbxCommon.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 18:17:16.000000 skanym-0.1.1/src/skanym/utils/fbx_bindings/__init__.py
+-rw-rw-rw-   0        0        0  9286144 2023-11-07 11:28:47.000000 skanym-0.1.1/src/skanym/utils/fbx_bindings/fbx.pyd
+-rw-rw-rw-   0        0        0   105472 2023-11-07 11:28:47.000000 skanym-0.1.1/src/skanym/utils/fbx_bindings/sip.pyd
+drwxrwxrwx   0        0        0        0 2024-04-17 12:29:28.020523 skanym-0.1.1/src/skanym.egg-info/
+-rw-rw-rw-   0        0        0     2425 2024-04-17 12:29:27.000000 skanym-0.1.1/src/skanym.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1581 2024-04-17 12:29:27.000000 skanym-0.1.1/src/skanym.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 12:29:27.000000 skanym-0.1.1/src/skanym.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2024-04-17 12:29:27.000000 skanym-0.1.1/src/skanym.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-17 12:29:27.000000 skanym-0.1.1/src/skanym.egg-info/top_level.txt
```

### Comparing `skanym-0.1.0/LICENSE.txt` & `skanym-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `skanym-0.1.0/PKG-INFO` & `skanym-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skanym
-Version: 0.1.0
+Version: 0.1.1
 Summary: Standalone package for skeletal animation
 Author-email: Dimitri Kohler <dimitri.kohler@he-arc.ch>
 License: MIT License
         
         Copyright (c) 2022 Dimitri Kohler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `skanym-0.1.0/pyproject.toml` & `skanym-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "skanym"
-version = "0.1.0"
+version = "0.1.1"
 description = "Standalone package for skeletal animation"
 readme = "README.md"
 requires-python = "==3.10.*"
 license = {file = "LICENSE.txt"} 
 authors = [
     {name = "Dimitri Kohler", email = "dimitri.kohler@he-arc.ch"},
 ]
```

### Comparing `skanym-0.1.0/src/skanym/animators/baseAnimator.py` & `skanym-0.1.1/src/skanym/animators/baseAnimator.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.0/src/skanym/animators/baseFkAnimator.py` & `skanym-0.1.1/src/skanym/animators/baseFkAnimator.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.0/src/skanym/animators/globalFkAnimator.py` & `skanym-0.1.1/src/skanym/animators/globalFkAnimator.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.0/src/skanym/animators/localFkAnimator.py` & `skanym-0.1.1/src/skanym/animators/localFkAnimator.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.0/src/skanym/animators/pcaAnimator.py` & `skanym-0.1.1/src/skanym/animators/pcaAnimator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Dict, Tuple
+from typing import List
 
 import numpy as np
 import quaternion
 from sklearn.decomposition import PCA
 from sklearn.preprocessing import StandardScaler, MinMaxScaler
 
 from line_profiler import profile
@@ -91,14 +91,16 @@
 
         scaled_input_data = self.input_scaler.fit_transform(input_data)
         output_data = self.model.fit_transform(scaled_input_data)
         self.scaled_output_data = self.output_scaler.fit_transform(output_data)
 
         self.vec_parent_ids = self.skeleton.as_parent_id_vector()
 
+        self.nb_anims = 1
+
     # @profile
     def _execute(self):
         rescaled_values = self.output_scaler.inverse_transform(
             self.pca_values.reshape(1, -1)
         )
         generated_input = self.model.inverse_transform(rescaled_values)
         rescaled_input = self.input_scaler.inverse_transform(generated_input)
```

### Comparing `skanym-0.1.0/src/skanym/loaders/fbxLoader.py` & `skanym-0.1.1/src/skanym/loaders/fbxLoader.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.0/src/skanym/loaders/glbLoader.py` & `skanym-0.1.1/src/skanym/loaders/glbLoader.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.0/src/skanym/loaders/iFileLoader.py` & `skanym-0.1.1/src/skanym/loaders/iFileLoader.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.0/src/skanym/structures/animation/animation.py` & `skanym-0.1.1/src/skanym/structures/animation/animation.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.0/src/skanym/structures/animation/animationCurve.py` & `skanym-0.1.1/src/skanym/structures/animation/animationCurve.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.0/src/skanym/structures/animation/iCurve.py` & `skanym-0.1.1/src/skanym/structures/animation/iCurve.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.0/src/skanym/structures/animation/key.py` & `skanym-0.1.1/src/skanym/structures/animation/key.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.0/src/skanym/structures/animation/positionCurve.py` & `skanym-0.1.1/src/skanym/structures/animation/positionCurve.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.0/src/skanym/structures/animation/quaternionCurve.py` & `skanym-0.1.1/src/skanym/structures/animation/quaternionCurve.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.0/src/skanym/structures/animation/scalarCurve.py` & `skanym-0.1.1/src/skanym/structures/animation/scalarCurve.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.0/src/skanym/structures/character/joint.py` & `skanym-0.1.1/src/skanym/structures/character/joint.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.0/src/skanym/structures/character/skeleton.py` & `skanym-0.1.1/src/skanym/structures/character/skeleton.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.0/src/skanym/structures/data/iTransform.py` & `skanym-0.1.1/src/skanym/structures/data/iTransform.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.0/src/skanym/structures/data/transform.py` & `skanym-0.1.1/src/skanym/structures/data/transform.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.0/src/skanym/structures/data/transformMatrix.py` & `skanym-0.1.1/src/skanym/structures/data/transformMatrix.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.0/src/skanym/structures/data/vectorizedArray.py` & `skanym-0.1.1/src/skanym/structures/data/vectorizedArray.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.0/src/skanym/utils/conversion.py` & `skanym-0.1.1/src/skanym/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.0/src/skanym/utils/fbx_bindings/FbxCommon.py` & `skanym-0.1.1/src/skanym/utils/fbx_bindings/FbxCommon.py`

 * *Files identical despite different names*

### Comparing `skanym-0.1.0/src/skanym.egg-info/PKG-INFO` & `skanym-0.1.1/src/skanym.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skanym
-Version: 0.1.0
+Version: 0.1.1
 Summary: Standalone package for skeletal animation
 Author-email: Dimitri Kohler <dimitri.kohler@he-arc.ch>
 License: MIT License
         
         Copyright (c) 2022 Dimitri Kohler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `skanym-0.1.0/src/skanym.egg-info/SOURCES.txt` & `skanym-0.1.1/src/skanym.egg-info/SOURCES.txt`

 * *Files identical despite different names*

