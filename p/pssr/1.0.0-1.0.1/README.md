# Comparing `tmp/pssr-1.0.0.tar.gz` & `tmp/pssr-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pssr-1.0.0.tar", max compression
+gzip compressed data, was "pssr-1.0.1.tar", max compression
```

## Comparing `pssr-1.0.0.tar` & `pssr-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1070 2024-04-16 22:30:44.098815 pssr-1.0.0/LICENSE
--rw-r--r--   0        0        0     1109 2024-04-16 23:04:32.970974 pssr-1.0.0/README.rst
--rw-r--r--   0        0        0        0 2024-03-07 21:39:47.125640 pssr-1.0.0/pssr/__init__.py
--rw-r--r--   0        0        0     2891 2024-04-16 02:07:03.589014 pssr-1.0.0/pssr/crappifiers.py
--rw-r--r--   0        0        0    23032 2024-04-16 22:47:32.941554 pssr-1.0.0/pssr/data.py
--rw-r--r--   0        0        0     2365 2024-04-16 22:40:37.212832 pssr-1.0.0/pssr/loss.py
--rw-r--r--   0        0        0       60 2024-03-11 21:20:49.404375 pssr-1.0.0/pssr/models/__init__.py
--rw-r--r--   0        0        0     1538 2024-03-07 21:39:47.125640 pssr-1.0.0/pssr/models/_blocks.py
--rw-r--r--   0        0        0     3167 2024-04-16 22:49:22.863791 pssr-1.0.0/pssr/models/resunet.py
--rw-r--r--   0        0        0     5394 2024-04-16 22:51:06.069875 pssr-1.0.0/pssr/models/resuneta.py
--rw-r--r--   0        0        0    11190 2024-04-16 22:12:45.003742 pssr-1.0.0/pssr/predict.py
--rw-r--r--   0        0        0    12905 2024-04-16 21:43:09.824278 pssr-1.0.0/pssr/train.py
--rw-r--r--   0        0        0      825 2024-04-16 22:38:52.978548 pssr-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2255 1970-01-01 00:00:00.000000 pssr-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-16 23:21:24.739071 pssr-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1129 2024-04-17 01:46:32.503705 pssr-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2024-03-07 21:39:47.125640 pssr-1.0.1/pssr/__init__.py
+-rw-r--r--   0        0        0     2891 2024-04-16 23:21:24.747072 pssr-1.0.1/pssr/crappifiers.py
+-rw-r--r--   0        0        0    23918 2024-04-17 21:06:33.049096 pssr-1.0.1/pssr/data.py
+-rw-r--r--   0        0        0     2365 2024-04-16 23:21:24.747072 pssr-1.0.1/pssr/loss.py
+-rw-r--r--   0        0        0       60 2024-04-16 23:21:24.747072 pssr-1.0.1/pssr/models/__init__.py
+-rw-r--r--   0        0        0     1538 2024-03-07 21:39:47.125640 pssr-1.0.1/pssr/models/_blocks.py
+-rw-r--r--   0        0        0     3167 2024-04-16 23:21:24.747072 pssr-1.0.1/pssr/models/resunet.py
+-rw-r--r--   0        0        0     5394 2024-04-16 23:21:24.747072 pssr-1.0.1/pssr/models/resuneta.py
+-rw-r--r--   0        0        0    11190 2024-04-16 23:21:24.751072 pssr-1.0.1/pssr/predict.py
+-rw-r--r--   0        0        0    12905 2024-04-16 23:21:24.751072 pssr-1.0.1/pssr/train.py
+-rw-r--r--   0        0        0     1046 2024-04-17 21:22:52.443580 pssr-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2475 1970-01-01 00:00:00.000000 pssr-1.0.1/PKG-INFO
```

### Comparing `pssr-1.0.0/LICENSE` & `pssr-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pssr-1.0.0/README.rst` & `pssr-1.0.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-Point-Scanning Super-Resolution (**PSSR**)
-===========================================
+# Point-Scanning Super-Resolution (**PSSR**)
 
-**PSSR** is a standardized `PyTorch <https://pytorch.org/>`_ workflow for super-resolution tasks using microscopy images.
-This is the official reimplementation of the methods described in the original paper: `Deep learning-based point-scanning super-resolution imaging <https://www.nature.com/articles/s41592-021-01080-z>`_,
+**PSSR** is a standardized [PyTorch](https://pytorch.org) workflow for super-resolution tasks using microscopy images.
+This is the official reimplementation of the methods described in the original paper: [Deep learning-based point-scanning super-resolution imaging](https://www.nature.com/articles/s41592-021-01080-z),
 containing various improvements and new features.
 
-The **PSSR** User Guide and full API Reference is available in the `PSSR Documentation <https://haydenstites.github.io/PSSR>`_.
+The **PSSR** User Guide and full API Reference is available in the [PSSR Documentation](https://haydenstites.github.io/PSSR).
 
-If you have never used **PSSR** before, `Getting Started <https://haydenstites.github.io/PSSR/guide/start.html>`_ outlines installation and basic usage.
-Full reference and explanations of all **PSSR** tools is available in `API Reference <https://haydenstites.github.io/PSSR/reference/api.html>`_.
+If you have never used **PSSR** before, [Getting Started](https://haydenstites.github.io/PSSR/guide/start.html) outlines installation and basic usage.
+Full reference and explanations of all **PSSR** tools is available in [API Reference](https://haydenstites.github.io/PSSR/reference/api.html).
 
-The package is still in development. All code can be found here.
-If you experience any bugs, unexpected behaviors, or have any suggestions, make sure to `open a ticket <https://github.com/haydenstites/PSSR/issues>`_.
+The package is still in development. All code can be found at [https://github.com/haydenstites/PSSR](https://github.com/haydenstites/PSSR).
+If you experience any bugs, unexpected behaviors, or have any suggestions, make sure to [open a ticket](https://github.com/haydenstites/PSSR/issues).
```

### Comparing `pssr-1.0.0/pssr/crappifiers.py` & `pssr-1.0.1/pssr/crappifiers.py`

 * *Files identical despite different names*

### Comparing `pssr-1.0.0/pssr/data.py` & `pssr-1.0.1/pssr/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import torch, glob, os, random, czifile
+import torch, glob, os, random, czifile, warnings
 import numpy as np
 from torch.utils.data import Dataset
 from pathlib import Path
 from PIL import Image
 from .crappifiers import Crappifier, Poisson
 
 class ImageDataset(Dataset):
@@ -36,14 +36,16 @@
             transforms (list[nn.Module]) : Additional final data transforms to apply. Default is None.
         """
         super().__init__()
         self.path = Path(path) if type(path) is str else path
         assert self.path.exists(), f"Path {self.path} does not exist."
 
         self.hr_files = sorted(glob.glob(f"*.{extension}", root_dir=self.path))
+        assert len(self.hr_files) > 0, f"No {extension} files exist in {self.path}."
+
         self.val_idx = _get_val_idx(len(self.hr_files), val_split, split_seed)
 
         self.is_lr = all([size <= hr_res//lr_scale for size in Image.open(Path(self.path, self.hr_files[0])).size]) or (lr_scale == 1)
         self.crop_res = min(hr_res, max(Image.open(Path(self.path, self.hr_files[0])).size)) * (lr_scale if self.is_lr else 1)
 
         self.hr_res = hr_res
         self.lr_scale = lr_scale
@@ -52,14 +54,16 @@
         self.rotation = rotation if val_split < 1 else False
         self.transforms = transforms
 
     def __len__(self):
         return len(self.hr_files)
     
     def __getitem__(self, idx):
+        assert idx < len(self), "Tried to retrieve invalid image."
+
         hr = Image.open(Path(self.path, self.hr_files[idx]))
 
         hr = _frame_channel(hr, self.mode)
         
         if self.is_lr:
             # Rotation and crappifier is disabled in lr mode
             return _ready_lr(hr, self.hr_res//self.lr_scale, self.transforms)
@@ -102,16 +106,17 @@
             transforms (list[nn.Module]) : Additional final data transforms to apply. Default is None.
         """
         super().__init__()
         self.path = Path(path) if type(path) is str else path
         assert self.path.exists(), f"Path {self.path} does not exist."
         
         self.hr_files = sorted(glob.glob(f"*.{extension}", root_dir=self.path))
-        self.stride = hr_res - overlap
+        assert len(self.hr_files) > 0, f"No {extension} files exist in {self.path}."
 
+        self.stride = hr_res - overlap
         self.tiles = []
         for file in self.hr_files:
             image = _load_sheet(self.path, file, mode)
             tiles_x, tiles_y = _n_tiles(image, hr_res, self.stride)
             self.tiles.append(tiles_x * tiles_y)
 
         self.val_idx = _get_val_idx(sum(self.tiles), val_split, split_seed)
@@ -126,15 +131,15 @@
         self.rotation = rotation if val_split < 1 else False
         self.transforms = transforms
         
     def __len__(self):
         return sum(self.tiles)
     
     def __getitem__(self, idx):
-        assert idx < sum(self.tiles), "Tried to retrieve invalid tile."
+        assert idx < len(self), "Tried to retrieve invalid tile."
 
         # Find idx tile across all tiles
         image_idx = 0
         for size in self.tiles:
             if idx < size:
                 image = _sliding_window(_load_sheet(self.path, self.hr_files[image_idx], self.mode), self.hr_res, self.stride, idx)
                 break
@@ -183,17 +188,21 @@
 
             transforms (list[nn.Module]) : Additional final data transforms to apply. Default is None.
         """
         super().__init__()
         self.hr_path = Path(hr_path) if type(hr_path) is str else hr_path
         self.lr_path = Path(lr_path) if type(lr_path) is str else lr_path
         assert self.hr_path.exists() and self.lr_path.exists(), f"One path {self.hr_path} or {self.lr_path} does not exist."
+        if self.hr_path == self.lr_path:
+            warnings.warn("hr_path is equal to lr_path, this should not be done except for testing purposes. Consider using ImageDataset instead.")
 
         self.hr_files = sorted(glob.glob(f"*.{extension}", root_dir=self.hr_path))
         self.lr_files = sorted(glob.glob(f"*.{extension}", root_dir=self.lr_path))
+        for files, path in zip([self.hr_files, self.lr_files], [self.hr_path, self.lr_path]):
+            assert len(files) > 0, f"No {extension} files exist in {path}."
         assert len(self.hr_files) == len(self.lr_files), "Length mismatch between high-low-resolution images."
 
         self.val_idx = _get_val_idx(len(self.hr_files), val_split, split_seed)
 
         self.is_lr = False
         self.crop_res = min(hr_res, max(Image.open(Path(self.hr_path, self.hr_files[0])).size))
 
@@ -203,22 +212,23 @@
         self.rotation = rotation
         self.transforms = transforms
 
     def __len__(self):
         return len(self.hr_files)
     
     def __getitem__(self, idx):
+        assert idx < len(self), "Tried to retrieve invalid image."
+
         hr = Image.open(Path(self.hr_path, self.hr_files[idx]))
         lr = Image.open(Path(self.lr_path, self.lr_files[idx]))
 
         hr = _frame_channel(hr, self.mode)
         lr = _frame_channel(lr, self.mode)
 
         return _transform_pair(hr, lr, self.hr_res, self.hr_res//self.lr_scale, self.rotation, self.transforms)
-        # return (*pair, ) if name else pair
 
     def _get_name(self, idx):
         return self.lr_files[idx].split('.')[0]
 
 class PairedSlidingDataset(Dataset):
     def __init__(self, hr_path : Path, lr_path : Path, hr_res : int = 512, lr_scale : int = 4, overlap : int = 128, val_split : float = 1, extension : str = "czi", mode : str = "L", rotation : bool = False, split_seed : int = None, transforms : list[torch.nn.Module] = None):
         r"""Testing dataset for loading high-low-resolution image tiles from image sheets without crappification. Can also be used for approximating :class:`Crappifier` parameters.
@@ -248,17 +258,21 @@
 
             transforms (list[nn.Module]) : Additional final data transforms to apply. Default is None.
         """
         super().__init__()
         self.hr_path = Path(hr_path) if type(hr_path) is str else hr_path
         self.lr_path = Path(lr_path) if type(lr_path) is str else lr_path
         assert self.hr_path.exists() and self.lr_path.exists(), f"One path {self.hr_path} or {self.lr_path} does not exist."
+        if self.hr_path == self.lr_path:
+            warnings.warn("hr_path is equal to lr_path, this should not be done except for testing purposes. Consider using SlidingDataset instead.")
         
         self.hr_files = sorted(glob.glob(f"*.{extension}", root_dir=self.hr_path))
         self.lr_files = sorted(glob.glob(f"*.{extension}", root_dir=self.lr_path))
+        for files, path in zip([self.hr_files, self.lr_files], [self.hr_path, self.lr_path]):
+            assert len(files) > 0, f"No {extension} files exist in {path}."
         assert len(self.hr_files) == len(self.lr_files), "Length mismatch between high-low-resolution images."
 
         self.stride = hr_res - overlap
 
         self.tiles = []
         for file in self.hr_files:
             image = _load_sheet(self.hr_path, file, mode)
@@ -276,29 +290,28 @@
         self.rotation = rotation
         self.transforms = transforms
 
     def __len__(self):
         return sum(self.tiles)
     
     def __getitem__(self, idx):
-        assert idx < sum(self.tiles), "Tried to retrieve invalid tile."
+        assert idx < len(self), "Tried to retrieve invalid tile."
 
         # Find idx tile across all tiles
         image_idx = 0
         for size in self.tiles:
             if idx < size:
                 hr = _sliding_window(_load_sheet(self.hr_path, self.hr_files[image_idx], self.mode), self.hr_res, self.stride, idx)
                 lr = _sliding_window(_load_sheet(self.lr_path, self.lr_files[image_idx], self.mode), self.hr_res//self.lr_scale, self.stride//self.lr_scale, idx)
                 break
             else:
                 idx -= size
                 image_idx += 1
 
         return _transform_pair(hr, lr, self.hr_res, self.hr_res//self.lr_scale, self.rotation, self.transforms)
-        # return (*pair, f"{self.lr_files[image_idx].split('.')[0]}_{idx}") if name else pair
     
     def _get_name(self, idx):
         image_idx = 0
         for size in self.tiles:
             if idx < size:
                 break
             else:
```

### Comparing `pssr-1.0.0/pssr/loss.py` & `pssr-1.0.1/pssr/loss.py`

 * *Files identical despite different names*

### Comparing `pssr-1.0.0/pssr/models/_blocks.py` & `pssr-1.0.1/pssr/models/_blocks.py`

 * *Files identical despite different names*

### Comparing `pssr-1.0.0/pssr/models/resunet.py` & `pssr-1.0.1/pssr/models/resunet.py`

 * *Files identical despite different names*

### Comparing `pssr-1.0.0/pssr/models/resuneta.py` & `pssr-1.0.1/pssr/models/resuneta.py`

 * *Files identical despite different names*

### Comparing `pssr-1.0.0/pssr/predict.py` & `pssr-1.0.1/pssr/predict.py`

 * *Files identical despite different names*

### Comparing `pssr-1.0.0/pssr/train.py` & `pssr-1.0.1/pssr/train.py`

 * *Files identical despite different names*

### Comparing `pssr-1.0.0/PKG-INFO` & `pssr-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 Metadata-Version: 2.1
 Name: pssr
-Version: 1.0.0
+Version: 1.0.1
 Summary: Point-Scanning Super-Resolution
-Home-page: https://github.com/Hayden-Stites/TMBot
+Home-page: https://github.com/haydenstites/PSSR
 License: MIT
 Author: Hayden Stites
 Requires-Python: >=3.11,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: GPU :: NVIDIA CUDA
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Dist: czifile (>=2019.7.2,<2020.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: opencv-python (>=4.9.0.80,<5.0.0.0)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Requires-Dist: pytorch-msssim (>=1.0.0,<2.0.0)
 Requires-Dist: scikit-image (>=0.23.1,<0.24.0)
 Requires-Dist: scikit-optimize (>=0.9.0,<0.10.0)
 Requires-Dist: torch (>=2.0.0,<3.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Project-URL: Documentation, https://haydenstites.github.io/PSSR/
-Project-URL: Repository, https://github.com/Hayden-Stites/TMBot
-Description-Content-Type: text/x-rst
+Project-URL: Repository, https://github.com/haydenstites/PSSR
+Description-Content-Type: text/markdown
 
-Point-Scanning Super-Resolution (**PSSR**)
-===========================================
+# Point-Scanning Super-Resolution (**PSSR**)
 
-**PSSR** is a standardized `PyTorch <https://pytorch.org/>`_ workflow for super-resolution tasks using microscopy images.
-This is the official reimplementation of the methods described in the original paper: `Deep learning-based point-scanning super-resolution imaging <https://www.nature.com/articles/s41592-021-01080-z>`_,
+**PSSR** is a standardized [PyTorch](https://pytorch.org) workflow for super-resolution tasks using microscopy images.
+This is the official reimplementation of the methods described in the original paper: [Deep learning-based point-scanning super-resolution imaging](https://www.nature.com/articles/s41592-021-01080-z),
 containing various improvements and new features.
 
-The **PSSR** User Guide and full API Reference is available in the `PSSR Documentation <https://haydenstites.github.io/PSSR>`_.
+The **PSSR** User Guide and full API Reference is available in the [PSSR Documentation](https://haydenstites.github.io/PSSR).
 
-If you have never used **PSSR** before, `Getting Started <https://haydenstites.github.io/PSSR/guide/start.html>`_ outlines installation and basic usage.
-Full reference and explanations of all **PSSR** tools is available in `API Reference <https://haydenstites.github.io/PSSR/reference/api.html>`_.
+If you have never used **PSSR** before, [Getting Started](https://haydenstites.github.io/PSSR/guide/start.html) outlines installation and basic usage.
+Full reference and explanations of all **PSSR** tools is available in [API Reference](https://haydenstites.github.io/PSSR/reference/api.html).
 
-The package is still in development. All code can be found here.
-If you experience any bugs, unexpected behaviors, or have any suggestions, make sure to `open a ticket <https://github.com/haydenstites/PSSR/issues>`_.
+The package is still in development. All code can be found at [https://github.com/haydenstites/PSSR](https://github.com/haydenstites/PSSR).
+If you experience any bugs, unexpected behaviors, or have any suggestions, make sure to [open a ticket](https://github.com/haydenstites/PSSR/issues).
```

