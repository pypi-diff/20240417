# Comparing `tmp/mashlib-0.1.5.tar.gz` & `tmp/mashlib-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mashlib-0.1.5.tar", max compression
+gzip compressed data, was "mashlib-0.1.6.tar", max compression
```

## Comparing `mashlib-0.1.5.tar` & `mashlib-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1494 2024-02-22 21:59:02.047891 mashlib-0.1.5/README.md
--rw-r--r--   0        0        0        0 2024-02-19 18:07:01.668680 mashlib-0.1.5/mash/__init__.py
--rw-r--r--   0        0        0       55 2024-02-19 18:08:36.328590 mashlib-0.1.5/mash/cloud/__init__.py
--rw-r--r--   0        0        0     1503 2024-02-19 18:07:01.668680 mashlib-0.1.5/mash/cloud/file_exists.py
--rw-r--r--   0        0        0     1339 2024-02-19 18:07:01.668680 mashlib-0.1.5/mash/cloud/file_exists_test.py
--rw-r--r--   0        0        0     2184 2024-02-19 18:07:01.668680 mashlib-0.1.5/mash/cloud/glob.py
--rw-r--r--   0        0        0     2804 2024-02-19 18:07:01.668680 mashlib-0.1.5/mash/cloud/glob_test.py
--rw-r--r--   0        0        0      391 2024-03-10 06:07:15.291782 mashlib-0.1.5/mash/images/__init__.py
--rw-r--r--   0        0        0     3426 2024-02-19 18:07:01.668680 mashlib-0.1.5/mash/images/conversion.py
--rw-r--r--   0        0        0     4640 2024-02-19 18:07:01.668680 mashlib-0.1.5/mash/images/conversion_test.py
--rw-r--r--   0        0        0     5553 2024-02-19 18:07:01.668680 mashlib-0.1.5/mash/images/crop.py
--rw-r--r--   0        0        0     8798 2024-02-19 18:07:01.668680 mashlib-0.1.5/mash/images/crop_test.py
--rw-r--r--   0        0        0     1875 2024-02-19 18:07:01.668680 mashlib-0.1.5/mash/images/normalization.py
--rw-r--r--   0        0        0     2714 2024-02-19 18:07:01.668680 mashlib-0.1.5/mash/images/normalization_test.py
--rw-r--r--   0        0        0     2153 2024-02-19 18:07:01.668680 mashlib-0.1.5/mash/images/resize.py
--rw-r--r--   0        0        0     1753 2024-02-19 18:07:01.668680 mashlib-0.1.5/mash/images/resize_test.py
--rw-r--r--   0        0        0     2496 2024-03-10 06:08:34.335884 mashlib-0.1.5/mash/images/tile.py
--rw-r--r--   0        0        0     2239 2024-03-10 06:07:09.203773 mashlib-0.1.5/mash/images/tile_test.py
--rw-r--r--   0        0        0      848 2024-02-19 18:07:01.668680 mashlib-0.1.5/mash/images/truecolor.py
--rw-r--r--   0        0        0     1797 2024-02-19 18:07:01.668680 mashlib-0.1.5/mash/images/truecolor_test.py
--rw-r--r--   0        0        0       46 2024-02-19 18:07:01.668680 mashlib-0.1.5/mash/ui/__init__.py
--rw-r--r--   0        0        0     1538 2024-02-19 18:07:01.668680 mashlib-0.1.5/mash/ui/console.py
--rw-r--r--   0        0        0      460 2024-02-19 18:07:01.668680 mashlib-0.1.5/mash/ui/logs.py
--rw-r--r--   0        0        0     1562 2024-02-19 18:07:01.668680 mashlib-0.1.5/mash/ui/logs_test.py
--rw-r--r--   0        0        0     1199 2024-03-10 06:09:39.323945 mashlib-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2540 1970-01-01 00:00:00.000000 mashlib-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     2540 2024-04-17 02:48:19.920246 mashlib-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-02-19 18:07:01.668680 mashlib-0.1.6/mash/__init__.py
+-rw-r--r--   0        0        0       55 2024-02-19 18:08:36.328590 mashlib-0.1.6/mash/cloud/__init__.py
+-rw-r--r--   0        0        0     1503 2024-02-19 18:07:01.668680 mashlib-0.1.6/mash/cloud/file_exists.py
+-rw-r--r--   0        0        0     1339 2024-02-19 18:07:01.668680 mashlib-0.1.6/mash/cloud/file_exists_test.py
+-rw-r--r--   0        0        0     2184 2024-02-19 18:07:01.668680 mashlib-0.1.6/mash/cloud/glob.py
+-rw-r--r--   0        0        0     2804 2024-02-19 18:07:01.668680 mashlib-0.1.6/mash/cloud/glob_test.py
+-rw-r--r--   0        0        0      391 2024-03-10 06:07:15.291782 mashlib-0.1.6/mash/images/__init__.py
+-rw-r--r--   0        0        0     3426 2024-02-19 18:07:01.668680 mashlib-0.1.6/mash/images/conversion.py
+-rw-r--r--   0        0        0     4640 2024-02-19 18:07:01.668680 mashlib-0.1.6/mash/images/conversion_test.py
+-rw-r--r--   0        0        0     5553 2024-02-19 18:07:01.668680 mashlib-0.1.6/mash/images/crop.py
+-rw-r--r--   0        0        0     8798 2024-02-19 18:07:01.668680 mashlib-0.1.6/mash/images/crop_test.py
+-rw-r--r--   0        0        0     1875 2024-02-19 18:07:01.668680 mashlib-0.1.6/mash/images/normalization.py
+-rw-r--r--   0        0        0     2714 2024-02-19 18:07:01.668680 mashlib-0.1.6/mash/images/normalization_test.py
+-rw-r--r--   0        0        0     2165 2024-04-17 02:08:41.519004 mashlib-0.1.6/mash/images/resize.py
+-rw-r--r--   0        0        0     1753 2024-02-19 18:07:01.668680 mashlib-0.1.6/mash/images/resize_test.py
+-rw-r--r--   0        0        0     2496 2024-03-10 06:08:34.335884 mashlib-0.1.6/mash/images/tile.py
+-rw-r--r--   0        0        0     2239 2024-03-10 06:07:09.203773 mashlib-0.1.6/mash/images/tile_test.py
+-rw-r--r--   0        0        0      848 2024-02-19 18:07:01.668680 mashlib-0.1.6/mash/images/truecolor.py
+-rw-r--r--   0        0        0     1797 2024-02-19 18:07:01.668680 mashlib-0.1.6/mash/images/truecolor_test.py
+-rw-r--r--   0        0        0       46 2024-02-19 18:07:01.668680 mashlib-0.1.6/mash/ui/__init__.py
+-rw-r--r--   0        0        0     1990 2024-04-15 00:06:54.154094 mashlib-0.1.6/mash/ui/console.py
+-rw-r--r--   0        0        0      643 2024-04-15 00:06:54.146094 mashlib-0.1.6/mash/ui/logs.py
+-rw-r--r--   0        0        0     1562 2024-02-19 18:07:01.668680 mashlib-0.1.6/mash/ui/logs_test.py
+-rw-r--r--   0        0        0     1322 2024-04-17 02:49:27.364158 mashlib-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3586 1970-01-01 00:00:00.000000 mashlib-0.1.6/PKG-INFO
```

### Comparing `mashlib-0.1.5/mash/cloud/file_exists.py` & `mashlib-0.1.6/mash/cloud/file_exists.py`

 * *Files identical despite different names*

### Comparing `mashlib-0.1.5/mash/cloud/file_exists_test.py` & `mashlib-0.1.6/mash/cloud/file_exists_test.py`

 * *Files identical despite different names*

### Comparing `mashlib-0.1.5/mash/cloud/glob.py` & `mashlib-0.1.6/mash/cloud/glob.py`

 * *Files identical despite different names*

### Comparing `mashlib-0.1.5/mash/cloud/glob_test.py` & `mashlib-0.1.6/mash/cloud/glob_test.py`

 * *Files identical despite different names*

### Comparing `mashlib-0.1.5/mash/images/conversion.py` & `mashlib-0.1.6/mash/images/conversion.py`

 * *Files identical despite different names*

### Comparing `mashlib-0.1.5/mash/images/conversion_test.py` & `mashlib-0.1.6/mash/images/conversion_test.py`

 * *Files identical despite different names*

### Comparing `mashlib-0.1.5/mash/images/crop.py` & `mashlib-0.1.6/mash/images/crop.py`

 * *Files identical despite different names*

### Comparing `mashlib-0.1.5/mash/images/crop_test.py` & `mashlib-0.1.6/mash/images/crop_test.py`

 * *Files identical despite different names*

### Comparing `mashlib-0.1.5/mash/images/normalization.py` & `mashlib-0.1.6/mash/images/normalization.py`

 * *Files identical despite different names*

### Comparing `mashlib-0.1.5/mash/images/normalization_test.py` & `mashlib-0.1.6/mash/images/normalization_test.py`

 * *Files identical despite different names*

### Comparing `mashlib-0.1.5/mash/images/resize.py` & `mashlib-0.1.6/mash/images/resize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 from skimage.transform import resize
 
 
 def _resize_image_fixed_side(
-    image: np.ndarray, side_len: int, method: str = "max", preserve_range: bool = False
+    image: np.ndarray, side_len: int, method: str = "max", preserve_range: bool = True
 ) -> np.ndarray:
     # Do some checking.
     if side_len <= 0:
         raise ValueError("Side length must be a positive integer.")
 
     # Need epsilon for floating point errors.
     epsilon = 1e-3
@@ -31,15 +31,15 @@
         image, (new_height, new_width), preserve_range=preserve_range
     )
 
     return resized_image
 
 
 def resize_image_min_side(
-    image: np.ndarray, min_side_len: int = 224, preserve_range: bool = False
+    image: np.ndarray, min_side_len: int = 224, preserve_range: bool = True
 ) -> np.ndarray:
     """Resize the image such that the smallest side is equal to the specified length.
 
     Args:
         image: The image to resize.
         min_side_len: The length of the smallest side.
         preserve_range: Preserve the range of the image.
@@ -49,22 +49,22 @@
     """
     return _resize_image_fixed_side(
         image, min_side_len, method="min", preserve_range=preserve_range
     )
 
 
 def resize_image_max_side(
-    image: np.ndarray, max_side_len: int = 224, preserve_range: bool = False
+    image: np.ndarray, max_side_len: int = 224, preserve_range: bool = True
 ) -> np.ndarray:
     """Resize the image such that the longest side is equal to the specified length.
 
     Args:
         image: The image to resize.
         max_side_len: The length of the smallest side.
-        preserve_range: Preserve the range of the image.
+        preserve_range: Preserve the range of the image, False for 0-1.
 
     Returns:
         The resized image.
     """
     return _resize_image_fixed_side(
         image, max_side_len, method="max", preserve_range=preserve_range
     )
```

### Comparing `mashlib-0.1.5/mash/images/resize_test.py` & `mashlib-0.1.6/mash/images/resize_test.py`

 * *Files identical despite different names*

### Comparing `mashlib-0.1.5/mash/images/tile.py` & `mashlib-0.1.6/mash/images/tile.py`

 * *Files identical despite different names*

### Comparing `mashlib-0.1.5/mash/images/tile_test.py` & `mashlib-0.1.6/mash/images/tile_test.py`

 * *Files identical despite different names*

### Comparing `mashlib-0.1.5/mash/images/truecolor.py` & `mashlib-0.1.6/mash/images/truecolor.py`

 * *Files identical despite different names*

### Comparing `mashlib-0.1.5/mash/images/truecolor_test.py` & `mashlib-0.1.6/mash/images/truecolor_test.py`

 * *Files identical despite different names*

### Comparing `mashlib-0.1.5/mash/ui/logs_test.py` & `mashlib-0.1.6/mash/ui/logs_test.py`

 * *Files identical despite different names*

### Comparing `mashlib-0.1.5/pyproject.toml` & `mashlib-0.1.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mashlib"
-version = "0.1.5"
+version = "0.1.6"
 description = "Common library tools for Moonshine AI"
 license = "MIT"
 
 authors = [
     "Nate Harada <mash@moonshinelabs.ai>"
 ]
 repository = "https://github.com/moonshinelabs-ai/mash"
@@ -30,16 +30,20 @@
 smart-open = "^6.4.0"
 boto3 = "^1.28.78"
 moto = "^4.2.7"
 
 [tool.poetry.group.docs]
 optional = true
 [tool.poetry.group.docs.dependencies]
-Sphinx = "^5.1.1"
+furo = "^2024.1.29"
+sphinx = "^7.2.6"
+myst-parser = "^2.0.0"
 
+[tool.poetry.group.dev]
+optional = true
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.2"
 parameterized = "^0.9.0"
 isort = "^5.13.2"
 black = "^24.2.0"
 types-pillow = "^10.0.0.3"
 types-requests = "^2.31.0.10"
@@ -48,10 +52,12 @@
 
 # MyPy is missing stubs, which is annoying
 [[tool.mypy.overrides]]
 module = [
     "parameterized",
     "pillow_heif",
     "moto",
+    "boto3",
+    "botocore.exceptions",
     "smart_open"
 ]
 ignore_missing_imports = true
```

### Comparing `mashlib-0.1.5/PKG-INFO` & `mashlib-0.1.6/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,20 @@
-Metadata-Version: 2.1
-Name: mashlib
-Version: 0.1.5
-Summary: Common library tools for Moonshine AI
-Home-page: https://github.com/moonshinelabs-ai/mash
-License: MIT
-Keywords: moonshine,library
-Author: Nate Harada
-Author-email: mash@moonshinelabs.ai
-Requires-Python: >=3.10,<3.13
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: boto3 (>=1.28.78,<2.0.0)
-Requires-Dist: loguru (>=0.7.2,<0.8.0)
-Requires-Dist: moto (>=4.2.7,<5.0.0)
-Requires-Dist: numpy (>=1.26.0,<2.0.0)
-Requires-Dist: pillow (>=10.0.1,<11.0.0)
-Requires-Dist: pillow-heif (>=0.13.0,<0.14.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: rich (>=13.6.0,<14.0.0)
-Requires-Dist: scikit-image (>=0.22.0,<0.23.0)
-Requires-Dist: smart-open (>=6.4.0,<7.0.0)
-Requires-Dist: torch (>=2.0.0,!=2.0.1,!=2.1.0)
-Project-URL: Repository, https://github.com/moonshinelabs-ai/mash
-Description-Content-Type: text/markdown
-
 <br />
 <p align="center">
     <a href="https://github.com/moonshinelabs-ai/moonshine">
       <img src="https://moonshine-assets.s3.us-west-2.amazonaws.com/mash_full_logo_light.png" width="50%"/>
     </a>
 </p>
 
 <h2><p align="center">Shared utility functions powering Moonshine tools.</p></h2>
 
 <p align="center">
+    <a href="https://moonshine-mash.readthedocs.io/en/latest/">
+        <img alt="Documentation" src="https://readthedocs.org/projects/moonshine-mash/badge/?version=latest">
+    </a>
     <a href="https://pypi.org/project/moonshinelabs-ai/">
         <img alt="PyPi Version" src="https://img.shields.io/pypi/pyversions/mashlib">
     </a>
     <a href="https://pypi.org/project/mashlib/">
         <img alt="PyPi Package Version" src="https://img.shields.io/pypi/v/mashlib">
     </a>
     <a href="https://pepy.tech/project/mashlib/">
@@ -54,8 +29,32 @@
 </p>
 <br />
 
 ## What is Mash?
 Mash is a straightforward utility library for common tasks in computer vision and deep model training. The library was broken out of previous Moonshine projects like Moonshine and Zeroshot.
 
 ## What can Mash Do?
-TODO
+Mash broadly supports a few utilities, but the main ones are:
+
+1. Easy image conversion: simply call `to_pil`, `to_numpy`, and `to_tensor` to convert image formats. Accepts other images, URLs, or local files.
+2. Image processing files: convenience functions like `crop_to_multiple_of_dimensions` for transformer based patch models like ViT.
+3. Console UI: for long running jobs, a fullscreen console utility that has a progress bar at the bottom and text logging.
+4. Cloud functions: use `glob` or `exists` on AWS or GCS links.
+
+For a complete list of functions, see [the documentation](https://moonshine-mash.readthedocs.io/en/latest/index.html)
+
+## Installation
+To install via pip:
+
+`pip install mashlib`
+
+## Usage
+To use:
+
+```python
+# Import base package
+import mash
+
+# Import image processing
+import mash.images as mi
+image = mi.to_numpy("/path/to/image.png")
+```
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: mashlib Version: 0.1.5 Summary: Common library
-tools for Moonshine AI Home-page: https://github.com/moonshinelabs-ai/mash
-License: MIT Keywords: moonshine,library Author: Nate Harada Author-email:
-mash@moonshinelabs.ai Requires-Python: >=3.10,<3.13 Classifier: License :: OSI
-Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Dist: boto3 (>=1.28.78,<2.0.0) Requires-
-Dist: loguru (>=0.7.2,<0.8.0) Requires-Dist: moto (>=4.2.7,<5.0.0) Requires-
-Dist: numpy (>=1.26.0,<2.0.0) Requires-Dist: pillow (>=10.0.1,<11.0.0)
-Requires-Dist: pillow-heif (>=0.13.0,<0.14.0) Requires-Dist: requests
-(>=2.31.0,<3.0.0) Requires-Dist: rich (>=13.6.0,<14.0.0) Requires-Dist: scikit-
-image (>=0.22.0,<0.23.0) Requires-Dist: smart-open (>=6.4.0,<7.0.0) Requires-
-Dist: torch (>=2.0.0,!=2.0.1,!=2.1.0) Project-URL: Repository, https://
-github.com/moonshinelabs-ai/mash Description-Content-Type: text/markdown
+
 _[_h_t_t_p_s_:_/_/_m_o_o_n_s_h_i_n_e_-_a_s_s_e_t_s_._s_3_._u_s_-_w_e_s_t_-_2_._a_m_a_z_o_n_a_w_s_._c_o_m_/_m_a_s_h___f_u_l_l___l_o_g_o___l_i_g_h_t_._p_n_g_]
 ********** SShhaarreedd uuttiilliittyy ffuunnccttiioonnss ppoowweerriinngg MMoooonnsshhiinnee ttoooollss.. **********
- _[_P_y_P_i_ _V_e_r_s_i_o_n_]_[_P_y_P_i_ _P_a_c_k_a_g_e_ _V_e_r_s_i_o_n_]_[_P_y_P_i_ _D_o_w_n_l_o_a_d_s_]_[_C_h_a_t_ _o_n_ _S_l_a_c_k_]_[_L_i_c_e_n_s_e_]
+  _[_D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_P_y_P_i_ _V_e_r_s_i_o_n_]_[_P_y_P_i_ _P_a_c_k_a_g_e_ _V_e_r_s_i_o_n_]_[_P_y_P_i_ _D_o_w_n_l_o_a_d_s_]_[_C_h_a_t_ _o_n
+                                _S_l_a_c_k_]_[_L_i_c_e_n_s_e_]
 
 ## What is Mash? Mash is a straightforward utility library for common tasks in
 computer vision and deep model training. The library was broken out of previous
-Moonshine projects like Moonshine and Zeroshot. ## What can Mash Do? TODO
+Moonshine projects like Moonshine and Zeroshot. ## What can Mash Do? Mash
+broadly supports a few utilities, but the main ones are: 1. Easy image
+conversion: simply call `to_pil`, `to_numpy`, and `to_tensor` to convert image
+formats. Accepts other images, URLs, or local files. 2. Image processing files:
+convenience functions like `crop_to_multiple_of_dimensions` for transformer
+based patch models like ViT. 3. Console UI: for long running jobs, a fullscreen
+console utility that has a progress bar at the bottom and text logging. 4.
+Cloud functions: use `glob` or `exists` on AWS or GCS links. For a complete
+list of functions, see [the documentation](https://moonshine-
+mash.readthedocs.io/en/latest/index.html) ## Installation To install via pip:
+`pip install mashlib` ## Usage To use: ```python # Import base package import
+mash # Import image processing import mash.images as mi image = mi.to_numpy("/
+path/to/image.png") ```
```

