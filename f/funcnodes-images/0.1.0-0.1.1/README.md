# Comparing `tmp/funcnodes_images-0.1.0.tar.gz` & `tmp/funcnodes_images-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcnodes_images-0.1.0.tar", max compression
+gzip compressed data, was "funcnodes_images-0.1.1.tar", max compression
```

## Comparing `funcnodes_images-0.1.0.tar` & `funcnodes_images-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      898 2024-04-15 17:25:44.952843 funcnodes_images-0.1.0/funcnodes_images/__init__.py
--rw-r--r--   0        0        0     1608 2024-04-15 12:02:49.342650 funcnodes_images-0.1.0/funcnodes_images/_numpy.py
--rw-r--r--   0        0        0     1003 2024-04-15 12:11:22.056972 funcnodes_images-0.1.0/funcnodes_images/_pillow.py
--rw-r--r--   0        0        0     2877 2024-04-15 17:23:28.413169 funcnodes_images-0.1.0/funcnodes_images/image_nodes.py
--rw-r--r--   0        0        0     4786 2024-04-15 17:21:01.509209 funcnodes_images-0.1.0/funcnodes_images/imagecontainer.py
--rw-r--r--   0        0        0      622 2024-04-15 17:08:15.921504 funcnodes_images-0.1.0/funcnodes_images/utils.py
--rw-r--r--   0        0        0      450 2024-04-15 10:21:01.120397 funcnodes_images-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      349 2024-04-15 13:38:48.307325 funcnodes_images-0.1.0/README.md
--rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 funcnodes_images-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      948 2024-04-17 08:26:14.008141 funcnodes_images-0.1.1/funcnodes_images/__init__.py
+-rw-r--r--   0        0        0     1737 2024-04-16 17:00:50.731308 funcnodes_images-0.1.1/funcnodes_images/_numpy.py
+-rw-r--r--   0        0        0     1127 2024-04-16 16:22:29.320118 funcnodes_images-0.1.1/funcnodes_images/_pillow.py
+-rw-r--r--   0        0        0     4971 2024-04-16 17:00:40.645038 funcnodes_images-0.1.1/funcnodes_images/image_nodes.py
+-rw-r--r--   0        0        0     5156 2024-04-16 16:21:39.581875 funcnodes_images-0.1.1/funcnodes_images/imagecontainer.py
+-rw-r--r--   0        0        0     1305 2024-04-16 16:47:30.447724 funcnodes_images-0.1.1/funcnodes_images/utils.py
+-rw-r--r--   0        0        0      450 2024-04-17 08:26:19.303928 funcnodes_images-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      349 2024-04-15 13:38:48.307325 funcnodes_images-0.1.1/README.md
+-rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 funcnodes_images-0.1.1/PKG-INFO
```

### Comparing `funcnodes_images-0.1.0/funcnodes_images/__init__.py` & `funcnodes_images-0.1.1/funcnodes_images/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,20 +21,22 @@
             return obj.to_thumbnail((200, 200)).to_jpeg(), True
         return obj.to_jpeg(), True
     return obj, False
 
 
 fn.JSONEncoder.add_encoder(imageFormatEncoder)
 
+NODE_SHELF = nodes.NODE_SHELF
+
 __all__ = [
     "register_imageformat",
     "NumpyImageFormat",
     "get_format",
     "PillowImageFormat",
     "ImageFormat",
     "nodes",
+    "FUNCNODES_RENDER_OPTIONS",
+    "NODE_SHELF",
 ]
 
 
-__version__ = "0.1.0"
-
-NODE_SHELF = nodes.NODE_SHELF
+__version__ = "0.1.1"
```

### Comparing `funcnodes_images-0.1.0/funcnodes_images/_numpy.py` & `funcnodes_images-0.1.1/funcnodes_images/_numpy.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,14 +22,20 @@
             raise ValueError("arr must have 3 or 1 channels")
 
         super().__init__(arr)
 
     def get_data_copy(self) -> np.ndarray:
         return self._data.copy()
 
+    def width(self) -> int:
+        return self._data.shape[1]
+
+    def height(self) -> int:
+        return self._data.shape[0]
+
     def to_uint8(self) -> np.ndarray:
         d = self.data
         if d.dtype == np.uint8:
             return d
 
         _max = d.max()
         _min = d.min()
```

### Comparing `funcnodes_images-0.1.0/funcnodes_images/_pillow.py` & `funcnodes_images-0.1.1/funcnodes_images/_pillow.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,20 @@
 
     def to_array(self) -> np.ndarray:
         return np.array(self._data)
 
     def get_data_copy(self) -> Image.Image:
         return self._data.copy()
 
+    def width(self) -> int:
+        return self._data.width
+
+    def height(self) -> int:
+        return self._data.height
+
 
 def pillow_to_numpy(img: PillowImageFormat) -> NumpyImageFormat:
     return NumpyImageFormat(np.array(img.data))
 
 
 PillowImageFormat.add_to_converter(NumpyImageFormat, pillow_to_numpy)
```

### Comparing `funcnodes_images-0.1.0/funcnodes_images/imagecontainer.py` & `funcnodes_images-0.1.1/funcnodes_images/imagecontainer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import ABC, abstractmethod
-from typing import Type
+from typing import Type, Optional
 import numpy as np
 from typing import Any, TYPE_CHECKING, Generic, TypeVar, Callable, Dict
 import io
 from PIL import Image
 import os
-from .utils import calc_new_size
+from .utils import calc_new_size, calc_crop_values
 
 
 if TYPE_CHECKING:
     from ._numpy import NumpyImageFormat
     from ._pillow import PillowImageFormat
 
 
@@ -31,14 +31,22 @@
     def data(self) -> T:
         return self.get_data_copy()
 
     @abstractmethod
     def get_data_copy(self) -> T:
         pass
 
+    @abstractmethod
+    def width(self) -> int:
+        pass
+
+    @abstractmethod
+    def height(self) -> int:
+        pass
+
     def to(self, cls: Type["ImageFormat"] | str) -> "ImageFormat":
         if isinstance(cls, str):
             cls = IMAGE_FORMATS[cls]
         if self.__class__ == cls:
             return self
         if cls in ImageFormat._to_converters[self.__class__]:
             return self._to_converters[self.__class__][cls](self)
@@ -116,16 +124,24 @@
         h: int = None,
     ) -> "ImageFormat[T]":
         img: Image = self.to_img().data
         new_x, new_y = calc_new_size(img.width, img.height, w, h)
         img = img.resize((new_x, new_y))
         return self.__class__.from_array(np.array(img))
 
-    def crop(self, x1, y1, x2, y2) -> "ImageFormat[T]":
+    def crop(
+        self,
+        x1: Optional[int] = None,
+        y1: Optional[int] = None,
+        x2: Optional[int] = None,
+        y2: Optional[int] = None,
+    ) -> "ImageFormat[T]":
         img: Image = self.to_img().data
+        x1, y1, x2, y2 = calc_crop_values(img.width, img.height, x1, y1, x2, y2)
+
         img = img.crop((x1, y1, x2, y2))
         return self.__class__.from_array(np.array(img))
 
     def scale(self, factor: float) -> "ImageFormat[T]":
         if factor <= 0:
             raise ValueError("factor must be greater than 0")
```

### Comparing `funcnodes_images-0.1.0/PKG-INFO` & `funcnodes_images-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcnodes-images
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Julian Kimmig
 Author-email: julian.kimmig@gmx.net
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

