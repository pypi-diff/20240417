# Comparing `tmp/epochalyst-0.3.tar.gz` & `tmp/epochalyst-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epochalyst-0.3.tar", last modified: Tue Apr 16 15:34:47 2024, max compression
+gzip compressed data, was "epochalyst-0.3.1.tar", last modified: Wed Apr 17 09:47:46 2024, max compression
```

## Comparing `epochalyst-0.3.tar` & `epochalyst-0.3.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:47.414889 epochalyst-0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-16 15:34:39.000000 epochalyst-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-16 15:34:47.414889 epochalyst-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-16 15:34:39.000000 epochalyst-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:47.406889 epochalyst-0.3/epochalyst/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:47.410889 epochalyst-0.3/epochalyst/_core/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:47.410889 epochalyst-0.3/epochalyst/_core/_caching/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/_core/_caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15786 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/_core/_caching/_cacher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:47.410889 epochalyst-0.3/epochalyst/_core/_logging/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/_core/_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/_core/_logging/_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:47.410889 epochalyst-0.3/epochalyst/_core/_pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/_core/_pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/_core/_pipeline/_custom_data_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:47.410889 epochalyst-0.3/epochalyst/logging/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/logging/section_separator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:47.410889 epochalyst-0.3/epochalyst/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:47.410889 epochalyst-0.3/epochalyst/pipeline/model/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:47.414889 epochalyst-0.3/epochalyst/pipeline/model/training/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/training/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:47.414889 epochalyst-0.3/epochalyst/pipeline/model/training/augmentation/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/training/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/training/augmentation/image_augmentations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6889 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/training/augmentation/time_series_augmentations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/training/augmentation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:47.414889 epochalyst-0.3/epochalyst/pipeline/model/training/models/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/training/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/training/models/timm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/training/pretrain_block.py
--rw-r--r--   0 runner    (1001) docker     (127)    29781 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/training/torch_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/training/training.py
--rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/training/training_block.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:47.414889 epochalyst-0.3/epochalyst/pipeline/model/transformation/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/transformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/transformation/transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-16 15:34:39.000000 epochalyst-0.3/epochalyst/pipeline/model/transformation/transformation_block.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:34:47.414889 epochalyst-0.3/epochalyst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-16 15:34:47.000000 epochalyst-0.3/epochalyst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-16 15:34:47.000000 epochalyst-0.3/epochalyst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:34:47.000000 epochalyst-0.3/epochalyst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-16 15:34:47.000000 epochalyst-0.3/epochalyst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 15:34:47.000000 epochalyst-0.3/epochalyst.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-16 15:34:39.000000 epochalyst-0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:34:47.414889 epochalyst-0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:47:46.656628 epochalyst-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-17 09:47:43.000000 epochalyst-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-17 09:47:46.656628 epochalyst-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-17 09:47:43.000000 epochalyst-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:47:46.648627 epochalyst-0.3.1/epochalyst/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-17 09:47:43.000000 epochalyst-0.3.1/epochalyst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:47:46.648627 epochalyst-0.3.1/epochalyst/_core/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-17 09:47:43.000000 epochalyst-0.3.1/epochalyst/_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:47:46.652628 epochalyst-0.3.1/epochalyst/_core/_caching/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-17 09:47:43.000000 epochalyst-0.3.1/epochalyst/_core/_caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15786 2024-04-17 09:47:43.000000 epochalyst-0.3.1/epochalyst/_core/_caching/_cacher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:47:46.652628 epochalyst-0.3.1/epochalyst/_core/_logging/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-17 09:47:43.000000 epochalyst-0.3.1/epochalyst/_core/_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-17 09:47:43.000000 epochalyst-0.3.1/epochalyst/_core/_logging/_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:47:46.652628 epochalyst-0.3.1/epochalyst/_core/_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-17 09:47:43.000000 epochalyst-0.3.1/epochalyst/_core/_pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-17 09:47:43.000000 epochalyst-0.3.1/epochalyst/_core/_pipeline/_custom_data_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:47:46.652628 epochalyst-0.3.1/epochalyst/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-17 09:47:43.000000 epochalyst-0.3.1/epochalyst/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-17 09:47:43.000000 epochalyst-0.3.1/epochalyst/logging/section_separator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:47:46.652628 epochalyst-0.3.1/epochalyst/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-17 09:47:43.000000 epochalyst-0.3.1/epochalyst/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-17 09:47:43.000000 epochalyst-0.3.1/epochalyst/pipeline/ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:47:46.652628 epochalyst-0.3.1/epochalyst/pipeline/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-17 09:47:43.000000 epochalyst-0.3.1/epochalyst/pipeline/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-17 09:47:43.000000 epochalyst-0.3.1/epochalyst/pipeline/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:47:46.652628 epochalyst-0.3.1/epochalyst/pipeline/model/training/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-17 09:47:43.000000 epochalyst-0.3.1/epochalyst/pipeline/model/training/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:47:46.652628 epochalyst-0.3.1/epochalyst/pipeline/model/training/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-17 09:47:43.000000 epochalyst-0.3.1/epochalyst/pipeline/model/training/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-17 09:47:43.000000 epochalyst-0.3.1/epochalyst/pipeline/model/training/augmentation/image_augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6889 2024-04-17 09:47:43.000000 epochalyst-0.3.1/epochalyst/pipeline/model/training/augmentation/time_series_augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-17 09:47:43.000000 epochalyst-0.3.1/epochalyst/pipeline/model/training/augmentation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:47:46.652628 epochalyst-0.3.1/epochalyst/pipeline/model/training/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-17 09:47:43.000000 epochalyst-0.3.1/epochalyst/pipeline/model/training/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-17 09:47:43.000000 epochalyst-0.3.1/epochalyst/pipeline/model/training/models/timm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-17 09:47:43.000000 epochalyst-0.3.1/epochalyst/pipeline/model/training/pretrain_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30668 2024-04-17 09:47:43.000000 epochalyst-0.3.1/epochalyst/pipeline/model/training/torch_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-17 09:47:43.000000 epochalyst-0.3.1/epochalyst/pipeline/model/training/training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-04-17 09:47:43.000000 epochalyst-0.3.1/epochalyst/pipeline/model/training/training_block.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:47:46.656628 epochalyst-0.3.1/epochalyst/pipeline/model/transformation/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-17 09:47:43.000000 epochalyst-0.3.1/epochalyst/pipeline/model/transformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-17 09:47:43.000000 epochalyst-0.3.1/epochalyst/pipeline/model/transformation/transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-17 09:47:43.000000 epochalyst-0.3.1/epochalyst/pipeline/model/transformation/transformation_block.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:47:46.656628 epochalyst-0.3.1/epochalyst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-17 09:47:46.000000 epochalyst-0.3.1/epochalyst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-17 09:47:46.000000 epochalyst-0.3.1/epochalyst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:47:46.000000 epochalyst-0.3.1/epochalyst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-17 09:47:46.000000 epochalyst-0.3.1/epochalyst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-17 09:47:46.000000 epochalyst-0.3.1/epochalyst.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-04-17 09:47:43.000000 epochalyst-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 09:47:46.656628 epochalyst-0.3.1/setup.cfg
```

### Comparing `epochalyst-0.3/LICENSE` & `epochalyst-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `epochalyst-0.3/PKG-INFO` & `epochalyst-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epochalyst
-Version: 0.3
+Version: 0.3.1
 Summary: This package contains the code for team Epoch's pipeline
 Author-email: Jasper van Selm <jmvanselm@gmail.com>, Ariel Ebersberger <arielebersberger@gmail.com>, Tolga Kopar <cahittolgakopar@gmail.com>, Jeffrey Lim <jeffrey-lim@outlook.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `epochalyst-0.3/README.md` & `epochalyst-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `epochalyst-0.3/epochalyst/_core/_caching/_cacher.py` & `epochalyst-0.3.1/epochalyst/_core/_caching/_cacher.py`

 * *Files identical despite different names*

### Comparing `epochalyst-0.3/epochalyst/_core/_logging/_logger.py` & `epochalyst-0.3.1/epochalyst/_core/_logging/_logger.py`

 * *Files identical despite different names*

### Comparing `epochalyst-0.3/epochalyst/logging/section_separator.py` & `epochalyst-0.3.1/epochalyst/logging/section_separator.py`

 * *Files identical despite different names*

### Comparing `epochalyst-0.3/epochalyst/pipeline/ensemble.py` & `epochalyst-0.3.1/epochalyst/pipeline/ensemble.py`

 * *Files identical despite different names*

### Comparing `epochalyst-0.3/epochalyst/pipeline/model/model.py` & `epochalyst-0.3.1/epochalyst/pipeline/model/model.py`

 * *Files identical despite different names*

### Comparing `epochalyst-0.3/epochalyst/pipeline/model/training/augmentation/image_augmentations.py` & `epochalyst-0.3.1/epochalyst/pipeline/model/training/augmentation/image_augmentations.py`

 * *Files identical despite different names*

### Comparing `epochalyst-0.3/epochalyst/pipeline/model/training/augmentation/time_series_augmentations.py` & `epochalyst-0.3.1/epochalyst/pipeline/model/training/augmentation/time_series_augmentations.py`

 * *Files identical despite different names*

### Comparing `epochalyst-0.3/epochalyst/pipeline/model/training/augmentation/utils.py` & `epochalyst-0.3.1/epochalyst/pipeline/model/training/augmentation/utils.py`

 * *Files identical despite different names*

### Comparing `epochalyst-0.3/epochalyst/pipeline/model/training/models/timm.py` & `epochalyst-0.3.1/epochalyst/pipeline/model/training/models/timm.py`

 * *Files identical despite different names*

### Comparing `epochalyst-0.3/epochalyst/pipeline/model/training/pretrain_block.py` & `epochalyst-0.3.1/epochalyst/pipeline/model/training/pretrain_block.py`

 * *Files identical despite different names*

### Comparing `epochalyst-0.3/epochalyst/pipeline/model/training/torch_trainer.py` & `epochalyst-0.3.1/epochalyst/pipeline/model/training/torch_trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     - `optimizer` (functools.partial[Optimizer]): Optimizer to use for training.
     - `criterion` (nn.Module): Criterion to use for training.
     - `scheduler` (Callable[[Optimizer], LRScheduler] | None): Scheduler to use for training.
     - `epochs` (int): Number of epochs
     - `batch_size` (int): Batch size
     - `patience` (int): Patience for early stopping
     - `test_size` (float): Relative size of the test set
-    - `to_predict` (str): Whether to predict on the test set, all data or none
+    - `to_predict` (str): Whether to predict on the 'test' set, 'all' data or 'none'
     - `model_name` (str): Name of the model
     - `n_folds` (float): Number of folds for cross validation (0 for train full,
     - `fold` (int): Fold number
 
     Methods
     -------
     .. code-block:: python
@@ -149,15 +149,15 @@
             raise ValueError("to_predict should be either 'test', 'all' or 'none'")
 
         if self.n_folds == -1:
             raise ValueError(
                 "Please specify the number of folds for cross validation or set n_folds to 0 for train full.",
             )
         self.save_model_to_disk = True
-        self.model_directory = "tm"
+        self._model_directory = Path("tm")
         self.best_model_state_dict: dict[Any, Any] = {}
 
         # Set optimizer
         self.initialized_optimizer = self.optimizer(self.model.parameters())
 
         # Set scheduler
         self.initialized_scheduler: LRScheduler | None
@@ -219,15 +219,15 @@
         )
 
         # Create dataloaders
         train_loader, test_loader = self.create_dataloaders(train_dataset, test_dataset)
 
         if self._model_exists():
             self.log_to_terminal(
-                f"Model exists in {self.model_directory}/{self.get_hash()}.pt, loading model",
+                f"Model exists in {self._model_directory}/{self.get_hash()}.pt, loading model",
             )
             self._load_model()
             # Return the predictions
 
             return self._predict_after_train(
                 x,
                 y,
@@ -333,16 +333,14 @@
 
     def custom_predict(self, x: Any, **pred_args: Any) -> npt.NDArray[np.float32]:  # noqa: ANN401
         """Predict on the test data.
 
         :param x: The input to the system.
         :return: The output of the system.
         """
-        self._load_model()
-
         print_section_separator(f"Predicting model: {self.model.__class__.__name__}")
         self.log_to_debug(f"Predicting model: {self.model.__class__.__name__}")
 
         # Parse pred_args
         curr_batch_size = pred_args.get("batch_size", self.batch_size)
 
         # Create dataset
@@ -350,19 +348,32 @@
         pred_dataloader = DataLoader(
             pred_dataset,
             batch_size=curr_batch_size,
             shuffle=False,
             collate_fn=(collate_fn if hasattr(pred_dataset, "__getitems__") else None),  # type: ignore[arg-type]
         )
 
+        # Predict with a single model
+        if self.n_folds < 1 or pred_args.get("use_single_model", False):
+            self._load_model()
+            return self.predict_on_loader(pred_dataloader)
+
         predictions = []
+        # Predict with multiple models
         for i in range(int(self.n_folds)):
-            self.log_to_terminal(f"Predicting with model fold {i + 1}/{self.n_folds}")
             self._fold = i  # set the fold, which updates the hash
-            self._load_model()  # load the model for this fold
+            # Try to load the next fold if it exists
+            try:
+                self._load_model()
+            except FileNotFoundError as e:
+                if i == 0:
+                    raise FileNotFoundError(f"First model of {self.n_folds} folds not found...") from e
+                self.log_to_warning(f"Model for fold {self._fold} not found, skipping the rest of the folds...")
+                break
+            self.log_to_terminal(f"Predicting with model fold {i + 1}/{self.n_folds}")
             predictions.append(self.predict_on_loader(pred_dataloader))
 
         # Average the predictions using numpy
         test_predictions = np.array(predictions)
 
         return np.mean(test_predictions, axis=0)
 
@@ -467,20 +478,26 @@
             test_dataset,
             batch_size=self.batch_size,
             shuffle=False,
             collate_fn=(collate_fn if hasattr(test_dataset, "__getitems__") else None),  # type: ignore[arg-type]
         )
         return train_loader, test_loader
 
-    def update_model_directory(self, model_directory: str) -> None:
+    def update_model_directory(self, model_directory: Path) -> None:
         """Update the model directory.
 
         :param model_directory: The model directory.
         """
-        self.model_directory = model_directory
+        if model_directory.exists() and model_directory.is_dir():
+            self._model_directory = model_directory
+        elif not model_directory.exists():
+            model_directory.mkdir()
+            self._model_directory = model_directory
+        else:
+            raise ValueError(f"{model_directory} is not a valid model_directory")
 
     def save_model_to_external(self) -> None:
         """Save model to external database."""
         self.log_to_warning(
             "Saving model to external is not implemented for TorchTrainer, if you want uploaded models. Please overwrite",
         )
 
@@ -639,59 +656,59 @@
                 pbar.set_description(desc=desc)
                 pbar.set_postfix(loss=sum(losses) / len(losses))
         return sum(losses) / len(losses)
 
     def _save_model(self) -> None:
         """Save the model in the model_directory folder."""
         self.log_to_terminal(
-            f"Saving model to {self.model_directory}/{self.get_hash()}.pt",
+            f"Saving model to {self._model_directory}/{self.get_hash()}.pt",
         )
-        path = Path(self.model_directory)
+        path = Path(self._model_directory)
         if not Path.exists(path):
             Path.mkdir(path)
 
-        torch.save(self.model, f"{self.model_directory}/{self.get_hash()}.pt")
+        torch.save(self.model, f"{self._model_directory}/{self.get_hash()}.pt")
         self.log_to_terminal(
-            f"Model saved to {self.model_directory}/{self.get_hash()}.pt",
+            f"Model saved to {self._model_directory}/{self.get_hash()}.pt",
         )
         self.save_model_to_external()
 
     def _load_model(self) -> None:
         """Load the model from the model_directory folder."""
         # Check if the model exists
-        if not Path(f"{self.model_directory}/{self.get_hash()}.pt").exists():
+        if not Path(f"{self._model_directory}/{self.get_hash()}.pt").exists():
             raise FileNotFoundError(
-                f"Model not found in {self.model_directory}/{self.get_hash()}.pt",
+                f"Model not found in {self._model_directory}/{self.get_hash()}.pt",
             )
 
         # Load model
         self.log_to_terminal(
-            f"Loading model from {self.model_directory}/{self.get_hash()}.pt",
+            f"Loading model from {self._model_directory}/{self.get_hash()}.pt",
         )
-        checkpoint = torch.load(f"{self.model_directory}/{self.get_hash()}.pt")
+        checkpoint = torch.load(f"{self._model_directory}/{self.get_hash()}.pt")
 
         # Load the weights from the checkpoint
         if isinstance(checkpoint, nn.DataParallel):
             model = checkpoint.module
         else:
             model = checkpoint
 
         # Set the current model to the loaded model
         if isinstance(self.model, nn.DataParallel):
             self.model.module.load_state_dict(model.state_dict())
         else:
             self.model.load_state_dict(model.state_dict())
 
         self.log_to_terminal(
-            f"Model loaded from {self.model_directory}/{self.get_hash()}.pt",
+            f"Model loaded from {self._model_directory}/{self.get_hash()}.pt",
         )
 
     def _model_exists(self) -> bool:
         """Check if the model exists in the model_directory folder."""
-        return Path(f"{self.model_directory}/{self.get_hash()}.pt").exists() and self.save_model_to_disk
+        return Path(f"{self._model_directory}/{self.get_hash()}.pt").exists() and self.save_model_to_disk
 
     def _early_stopping(self) -> bool:
         """Check if early stopping should be performed.
 
         :return: Whether to perform early stopping.
         """
         # Store the best model so far based on validation loss
```

### Comparing `epochalyst-0.3/epochalyst/pipeline/model/training/training.py` & `epochalyst-0.3.1/epochalyst/pipeline/model/training/training.py`

 * *Files identical despite different names*

### Comparing `epochalyst-0.3/epochalyst/pipeline/model/training/training_block.py` & `epochalyst-0.3.1/epochalyst/pipeline/model/training/training_block.py`

 * *Files identical despite different names*

### Comparing `epochalyst-0.3/epochalyst/pipeline/model/transformation/transformation.py` & `epochalyst-0.3.1/epochalyst/pipeline/model/transformation/transformation.py`

 * *Files identical despite different names*

### Comparing `epochalyst-0.3/epochalyst/pipeline/model/transformation/transformation_block.py` & `epochalyst-0.3.1/epochalyst/pipeline/model/transformation/transformation_block.py`

 * *Files identical despite different names*

### Comparing `epochalyst-0.3/epochalyst.egg-info/PKG-INFO` & `epochalyst-0.3.1/epochalyst.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epochalyst
-Version: 0.3
+Version: 0.3.1
 Summary: This package contains the code for team Epoch's pipeline
 Author-email: Jasper van Selm <jmvanselm@gmail.com>, Ariel Ebersberger <arielebersberger@gmail.com>, Tolga Kopar <cahittolgakopar@gmail.com>, Jeffrey Lim <jeffrey-lim@outlook.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `epochalyst-0.3/epochalyst.egg-info/SOURCES.txt` & `epochalyst-0.3.1/epochalyst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `epochalyst-0.3/pyproject.toml` & `epochalyst-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "epochalyst"
-version = "0.3"
+version = "0.3.1"
 authors = [
     { name = "Jasper van Selm", email = "jmvanselm@gmail.com" },
     { name = "Ariel Ebersberger", email = "arielebersberger@gmail.com" },
     { name = "Tolga Kopar", email = "cahittolgakopar@gmail.com" },
     { name = "Jeffrey Lim", email = "jeffrey-lim@outlook.com" },
 ]
 description = "This package contains the code for team Epoch's pipeline"
```

