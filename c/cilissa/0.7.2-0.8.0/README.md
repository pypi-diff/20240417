# Comparing `tmp/cilissa-0.7.2.tar.gz` & `tmp/cilissa-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cilissa-0.7.2.tar", max compression
+gzip compressed data, was "cilissa-0.8.0.tar", max compression
```

## Comparing `cilissa-0.7.2.tar` & `cilissa-0.8.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1998 2021-12-08 18:43:31.972753 cilissa-0.7.2/README.md
--rw-r--r--   0        0        0      169 2021-12-08 18:43:31.972753 cilissa-0.7.2/cilissa/__init__.py
--rw-r--r--   0        0        0     2054 2021-12-08 18:43:31.972753 cilissa-0.7.2/cilissa/__main__.py
--rw-r--r--   0        0        0     2698 2021-12-08 18:43:31.972753 cilissa-0.7.2/cilissa/classes.py
--rw-r--r--   0        0        0      201 2021-12-08 18:43:31.972753 cilissa-0.7.2/cilissa/exceptions.py
--rw-r--r--   0        0        0     1096 2021-12-08 18:43:31.972753 cilissa-0.7.2/cilissa/helpers.py
--rw-r--r--   0        0        0     9167 2021-12-08 18:43:31.972753 cilissa-0.7.2/cilissa/images.py
--rw-r--r--   0        0        0    10392 2021-12-08 18:43:31.972753 cilissa-0.7.2/cilissa/metrics.py
--rw-r--r--   0        0        0     3524 2021-12-08 18:43:31.972753 cilissa-0.7.2/cilissa/operations.py
--rw-r--r--   0        0        0     3201 2021-12-08 18:43:31.972753 cilissa-0.7.2/cilissa/parsers.py
--rw-r--r--   0        0        0      211 2021-12-08 18:43:31.972753 cilissa-0.7.2/cilissa/plugins/__init__.py
--rw-r--r--   0        0        0     4820 2021-12-08 18:43:31.972753 cilissa-0.7.2/cilissa/results.py
--rw-r--r--   0        0        0      445 2021-12-08 18:43:31.972753 cilissa-0.7.2/cilissa/roi.py
--rw-r--r--   0        0        0     6008 2021-12-08 18:43:31.972753 cilissa-0.7.2/cilissa/transformations.py
--rw-r--r--   0        0        0      107 2021-12-08 18:43:31.972753 cilissa-0.7.2/cilissa/utils.py
--rw-r--r--   0        0        0     1553 2021-12-08 18:43:31.984754 cilissa-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     2978 2021-12-08 18:44:22.013913 cilissa-0.7.2/setup.py
--rw-r--r--   0        0        0     3064 2021-12-08 18:44:22.014361 cilissa-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-16 23:21:58.498687 cilissa-0.8.0/LICENSE
+-rw-r--r--   0        0        0     2168 2024-04-16 23:21:58.498687 cilissa-0.8.0/README.md
+-rw-r--r--   0        0        0      169 2024-04-16 23:21:58.498687 cilissa-0.8.0/cilissa/__init__.py
+-rw-r--r--   0        0        0     2054 2024-04-16 23:21:58.498687 cilissa-0.8.0/cilissa/__main__.py
+-rw-r--r--   0        0        0     2698 2024-04-16 23:21:58.498687 cilissa-0.8.0/cilissa/classes.py
+-rw-r--r--   0        0        0      201 2024-04-16 23:21:58.498687 cilissa-0.8.0/cilissa/exceptions.py
+-rw-r--r--   0        0        0     1096 2024-04-16 23:21:58.498687 cilissa-0.8.0/cilissa/helpers.py
+-rw-r--r--   0        0        0     9167 2024-04-16 23:21:58.498687 cilissa-0.8.0/cilissa/images.py
+-rw-r--r--   0        0        0    10362 2024-04-16 23:21:58.498687 cilissa-0.8.0/cilissa/metrics.py
+-rw-r--r--   0        0        0     3524 2024-04-16 23:21:58.498687 cilissa-0.8.0/cilissa/operations.py
+-rw-r--r--   0        0        0     3201 2024-04-16 23:21:58.498687 cilissa-0.8.0/cilissa/parsers.py
+-rw-r--r--   0        0        0      211 2024-04-16 23:21:58.498687 cilissa-0.8.0/cilissa/plugins/__init__.py
+-rw-r--r--   0        0        0     4820 2024-04-16 23:21:58.498687 cilissa-0.8.0/cilissa/results.py
+-rw-r--r--   0        0        0      445 2024-04-16 23:21:58.498687 cilissa-0.8.0/cilissa/roi.py
+-rw-r--r--   0        0        0     6008 2024-04-16 23:21:58.498687 cilissa-0.8.0/cilissa/transformations.py
+-rw-r--r--   0        0        0      107 2024-04-16 23:21:58.498687 cilissa-0.8.0/cilissa/utils.py
+-rw-r--r--   0        0        0     1539 2024-04-16 23:21:58.506687 cilissa-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3191 1970-01-01 00:00:00.000000 cilissa-0.8.0/PKG-INFO
```

### Comparing `cilissa-0.7.2/README.md` & `cilissa-0.8.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 It features the most popular full-reference image quality metrics, image transformations and translations. 
 CILISSA is also very extensible and new operations can be easily added.
 
 CILISSA has an optional Qt-based graphical interface that lets you experiment with various operations, their orders and properties.
 
 ## Requirements
 
-* Python >= 3.7
+* Python >=3.9,<3.12
 
 ## Installation
 
 ### Install from PyPI
 ```bash
 $ pip install cilissa
 ```
@@ -55,7 +55,11 @@
 <operation-name>-<parameter-name>=<value>
 ``` 
 where `parameter-name` uses hyphens (-) instead of underscores (_)
 
 ## Documentation
 
 Documentation is hosted on [Read the Docs](https://cilissa.readthedocs.io/).
+
+## License
+
+`CILISSA` is under the terms of the [MIT License](https://www.tldrlegal.com/l/mit), following all clarifications stated in the [license file](LICENSE).
```

#### html2text {}

```diff
@@ -5,17 +5,20 @@
   _/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_e_x_l_e_r_/_C_I_L_I_S_S_A_/_b_r_a_n_c_h_/_m_a_i_n_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_D_i_x_b_5_b_u_M_Q_r_]
                  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_r_e_a_d_t_h_e_d_o_c_s_/_c_i_l_i_s_s_a_]
 ## Overview CILISSA allows for the use of various metrics to perform full-
 reference image comparisons. It features the most popular full-reference image
 quality metrics, image transformations and translations. CILISSA is also very
 extensible and new operations can be easily added. CILISSA has an optional Qt-
 based graphical interface that lets you experiment with various operations,
-their orders and properties. ## Requirements * Python >= 3.7 ## Installation
-### Install from PyPI ```bash $ pip install cilissa ``` ### Releases Binaries
-for Windows and Linux can be found on [GitHub releases](https://github.com/
-exler/CILISSA/releases). ## Usage ### GUI Information about the GUI can be
-found in the [cilissa_gui/README.md](cilissa_gui/README.md) file. ### CLI
-Currently the CLI only supports working with a single pair of images. The
-parameters of metrics and transformations can be modified by passing them to
-the `--kwargs` argument using the following format: ``` -= ``` where
-`parameter-name` uses hyphens (-) instead of underscores (_) ## Documentation
-Documentation is hosted on [Read the Docs](https://cilissa.readthedocs.io/).
+their orders and properties. ## Requirements * Python >=3.9,<3.12 ##
+Installation ### Install from PyPI ```bash $ pip install cilissa ``` ###
+Releases Binaries for Windows and Linux can be found on [GitHub releases]
+(https://github.com/exler/CILISSA/releases). ## Usage ### GUI Information about
+the GUI can be found in the [cilissa_gui/README.md](cilissa_gui/README.md)
+file. ### CLI Currently the CLI only supports working with a single pair of
+images. The parameters of metrics and transformations can be modified by
+passing them to the `--kwargs` argument using the following format: ``` -= ```
+where `parameter-name` uses hyphens (-) instead of underscores (_) ##
+Documentation Documentation is hosted on [Read the Docs](https://
+cilissa.readthedocs.io/). ## License `CILISSA` is under the terms of the [MIT
+License](https://www.tldrlegal.com/l/mit), following all clarifications stated
+in the [license file](LICENSE).
```

### Comparing `cilissa-0.7.2/cilissa/__main__.py` & `cilissa-0.8.0/cilissa/__main__.py`

 * *Files identical despite different names*

### Comparing `cilissa-0.7.2/cilissa/classes.py` & `cilissa-0.8.0/cilissa/classes.py`

 * *Files identical despite different names*

### Comparing `cilissa-0.7.2/cilissa/helpers.py` & `cilissa-0.8.0/cilissa/helpers.py`

 * *Files identical despite different names*

### Comparing `cilissa-0.7.2/cilissa/images.py` & `cilissa-0.8.0/cilissa/images.py`

 * *Files identical despite different names*

### Comparing `cilissa-0.7.2/cilissa/metrics.py` & `cilissa-0.8.0/cilissa/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,28 +110,28 @@
         drange = dmax - dmin
 
         # Compute weighted means using Gaussian weighting function
         ux = cv2.GaussianBlur(im1, (0, 0), self.sigma)
         uy = cv2.GaussianBlur(im2, (0, 0), self.sigma)
 
         # Compute weighted variances and covariances
-        uxx = cv2.GaussianBlur(im1 ** 2, (0, 0), self.sigma)
-        uyy = cv2.GaussianBlur(im2 ** 2, (0, 0), self.sigma)
+        uxx = cv2.GaussianBlur(im1**2, (0, 0), self.sigma)
+        uyy = cv2.GaussianBlur(im2**2, (0, 0), self.sigma)
         uxy = cv2.GaussianBlur(im1 * im2, (0, 0), self.sigma)
         vx = uxx - ux * ux
         vy = uyy - uy * uy
         vxy = uxy - ux * uy
 
         # Constants to avoid instability when ux**2 + uy**2 are close to zero (formula 7)
         L = drange
         C1 = (self.K1 * L) ** 2
         C2 = (self.K2 * L) ** 2
 
         # Final form of the SSIM index (formula 13, page 605)
-        A1, A2, B1, B2 = (2 * ux * uy + C1, 2 * vxy + C2, ux ** 2 + uy ** 2 + C1, vx + vy + C2)
+        A1, A2, B1, B2 = (2 * ux * uy + C1, 2 * vxy + C2, ux**2 + uy**2 + C1, vx + vy + C2)
         D = B1 * B2
         S = (A1 * A2) / D
 
         # Avoid edge effects by ignoring filter radius around edges
         # Pad equal to radius as in scipy gaussian_filter
         # https://github.com/scipy/scipy/blob/v1.7.0/scipy/ndimage/filters.py#L258
         pad = int(self.truncate * self.sigma + 0.5)
@@ -161,30 +161,30 @@
     def __init__(self, channels_num: Optional[int] = None, block_size: int = 8) -> None:
         self.channels_num = channels_num
 
         # Sliding window size
         self.block_size = block_size
 
     def uiqi_single_channel(self, im1: np.ndarray, im2: np.ndarray) -> float:
-        N = self.block_size ** 2
+        N = self.block_size**2
 
-        im1_sq = im1 ** 2
-        im2_sq = im2 ** 2
+        im1_sq = im1**2
+        im2_sq = im2**2
         im12 = im1 * im2
 
-        unif_filter = np.ones(self.block_size, np.float32) / (self.block_size ** 2)
+        unif_filter = np.ones(self.block_size, np.float32) / (self.block_size**2)
 
         im1_sum = cv2.filter2D(im1, ddepth=-1, kernel=unif_filter)
         im2_sum = cv2.filter2D(im2, ddepth=-1, kernel=unif_filter)
         im1_sq_sum = cv2.filter2D(im1_sq, ddepth=-1, kernel=unif_filter)
         im2_sq_sum = cv2.filter2D(im2_sq, ddepth=-1, kernel=unif_filter)
         im12_sum = cv2.filter2D(im12, ddepth=-1, kernel=unif_filter)
 
         im12_sum_mul = im1_sum * im2_sum
-        im12_sq_sum_mul = im1_sum ** 2 + im2_sum ** 2
+        im12_sq_sum_mul = im1_sum**2 + im2_sum**2
         numerator = 4 * (N * im12_sum - im12_sum_mul) * im12_sum_mul
         denominator1 = N * (im1_sq_sum + im2_sq_sum) - im12_sq_sum_mul
         denominator = denominator1 * im12_sq_sum_mul
 
         q_map = np.ones(denominator.shape)
         index = np.logical_and((denominator1 == 0), (im12_sq_sum_mul != 0))
         q_map[index] = (2 * im12_sum_mul[index]) / (im12_sq_sum_mul[index])
@@ -235,20 +235,20 @@
 
             if scale > 1:
                 im1 = cv2.GaussianBlur(im1, (0, 0), sd)
                 im2 = cv2.GaussianBlur(im2, (0, 0), sd)
 
             mu1 = cv2.GaussianBlur(im1, (0, 0), sd)
             mu2 = cv2.GaussianBlur(im2, (0, 0), sd)
-            mu1_sq = mu1 ** 2
-            mu2_sq = mu2 ** 2
+            mu1_sq = mu1**2
+            mu2_sq = mu2**2
             mu12 = mu1 * mu2
 
-            sigma1_sq = cv2.GaussianBlur(im1 ** 2, (0, 0), sd) - mu1_sq
-            sigma2_sq = cv2.GaussianBlur(im2 ** 2, (0, 0), sd) - mu2_sq
+            sigma1_sq = cv2.GaussianBlur(im1**2, (0, 0), sd) - mu1_sq
+            sigma2_sq = cv2.GaussianBlur(im2**2, (0, 0), sd) - mu2_sq
             sigma12 = cv2.GaussianBlur(im1 * im2, (0, 0), sd) - mu12
 
             sigma1_sq[sigma1_sq < 0] = 0
             sigma2_sq[sigma2_sq < 0] = 0
 
             g = sigma12 / (sigma1_sq + eps)
             sv_sq = sigma2_sq - (g * sigma12)
@@ -260,15 +260,15 @@
             g[sigma2_sq < eps] = 0
             sv_sq[sigma2_sq < eps] = 0
 
             sv_sq[g < 0] = sigma2_sq[g < 0]
             g[g < 0] = 0
             sv_sq[sv_sq <= eps] = eps
 
-            numerator += np.sum(np.log10(1 + g ** 2 * (sigma1_sq / (sv_sq + self.sigma))))
+            numerator += np.sum(np.log10(1 + g**2 * (sigma1_sq / (sv_sq + self.sigma))))
             denominator += np.sum(np.log10(1 + (sigma1_sq / self.sigma)))
 
         return numerator / denominator
 
     def analyze(self, image_pair: ImagePair) -> float:
         im1, im2 = image_pair.as_floats()
```

### Comparing `cilissa-0.7.2/cilissa/operations.py` & `cilissa-0.8.0/cilissa/operations.py`

 * *Files identical despite different names*

### Comparing `cilissa-0.7.2/cilissa/parsers.py` & `cilissa-0.8.0/cilissa/parsers.py`

 * *Files identical despite different names*

### Comparing `cilissa-0.7.2/cilissa/results.py` & `cilissa-0.8.0/cilissa/results.py`

 * *Files identical despite different names*

### Comparing `cilissa-0.7.2/cilissa/transformations.py` & `cilissa-0.8.0/cilissa/transformations.py`

 * *Files identical despite different names*

### Comparing `cilissa-0.7.2/pyproject.toml` & `cilissa-0.8.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cilissa"
-version = "0.7.2"
+version = "0.8.0"
 description = "Interactive tool for assessing digital image similarity"
 authors = ["Kamil Marut <kamil@kamilmarut.com>"]
 readme = "README.md"
 homepage = "https://github.com/exler/CILISSA"
 repository = "https://github.com/exler/CILISSA"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -15,35 +15,34 @@
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/exler/CILISSA/issues"
 
 [tool.poetry.dependencies]
-python = ">=3.7,<3.11"
-numpy = "^1.20.3"
-opencv-python = "^4.5.2"
-PySide6 = { version = "^6.1.2", optional = true }
+python = ">=3.9,<3.12"
+numpy = "^1.26.4"
+opencv-python = "^4.9.0.80"
+PySide6 = { version = "^6.7.0", optional = true }
 
 [tool.poetry.dev-dependencies]
-black = "^21.6b0"
-flake8 = "^3.9.2"
-flake8-annotations = "^2.6.2"
-bandit = "^1.7.0"
-mypy = "^0.902"
-isort = "^5.8.0"
-pytest = "^6.2.4"
-pytest-sugar = "^0.9.4"
+black = "^24.4.0"
+flake8 = "^7.0.0"
+flake8-annotations = "^3.0.1"
+mypy = "^1.9.0"
+isort = "^5.13.2"
+pytest = "^8.1.1"
+pytest-sugar = "^1.0.0"
 pytest-clarity = "^1.0.1"
-pyinstaller = "^4.5.1"
+pyinstaller = "^6.6.0"
 verdandi = "^0.2.3"
-Sphinx = "^4.2.0"
-sphinx-autoapi = "^1.8.4"
-sphinx-rtd-theme = "^1.0.0"
-coverage = "^6.0.2"
+Sphinx = "^7.2.6"
+sphinx-autoapi = "^3.0.0"
+sphinx-rtd-theme = "^2.0.0"
+coverage = "^7.4.4"
 
 [tool.poetry.extras]
 gui = ["PySide6"]
 
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
```

### Comparing `cilissa-0.7.2/PKG-INFO` & `cilissa-0.8.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: cilissa
-Version: 0.7.2
+Version: 0.8.0
 Summary: Interactive tool for assessing digital image similarity
 Home-page: https://github.com/exler/CILISSA
 Author: Kamil Marut
 Author-email: kamil@kamilmarut.com
-Requires-Python: >=3.7,<3.11
+Requires-Python: >=3.9,<3.12
 Classifier: Environment :: Console
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Provides-Extra: gui
-Requires-Dist: PySide6 (>=6.1.2,<7.0.0); extra == "gui"
-Requires-Dist: numpy (>=1.20.3,<2.0.0)
-Requires-Dist: opencv-python (>=4.5.2,<5.0.0)
+Requires-Dist: PySide6 (>=6.7.0,<7.0.0) ; extra == "gui"
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: opencv-python (>=4.9.0.80,<5.0.0.0)
 Project-URL: Bug Tracker, https://github.com/exler/CILISSA/issues
 Project-URL: Repository, https://github.com/exler/CILISSA
 Description-Content-Type: text/markdown
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/exler/CILISSA/main/docs/_static/logo.png" width="328">
 </p>
@@ -49,15 +48,15 @@
 It features the most popular full-reference image quality metrics, image transformations and translations. 
 CILISSA is also very extensible and new operations can be easily added.
 
 CILISSA has an optional Qt-based graphical interface that lets you experiment with various operations, their orders and properties.
 
 ## Requirements
 
-* Python >= 3.7
+* Python >=3.9,<3.12
 
 ## Installation
 
 ### Install from PyPI
 ```bash
 $ pip install cilissa
 ```
@@ -82,7 +81,11 @@
 ``` 
 where `parameter-name` uses hyphens (-) instead of underscores (_)
 
 ## Documentation
 
 Documentation is hosted on [Read the Docs](https://cilissa.readthedocs.io/).
 
+## License
+
+`CILISSA` is under the terms of the [MIT License](https://www.tldrlegal.com/l/mit), following all clarifications stated in the [license file](LICENSE).
+
```

#### html2text {}

```diff
@@ -1,35 +1,38 @@
-Metadata-Version: 2.1 Name: cilissa Version: 0.7.2 Summary: Interactive tool
+Metadata-Version: 2.1 Name: cilissa Version: 0.8.0 Summary: Interactive tool
 for assessing digital image similarity Home-page: https://github.com/exler/
 CILISSA Author: Kamil Marut Author-email: kamil@kamilmarut.com Requires-Python:
->=3.7,<3.11 Classifier: Environment :: Console Classifier: Environment :: X11
+>=3.9,<3.12 Classifier: Environment :: Console Classifier: Environment :: X11
 Applications :: Qt Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Topic :: Scientific/Engineering :: Image Processing Provides-Extra: gui
-Requires-Dist: PySide6 (>=6.1.2,<7.0.0); extra == "gui" Requires-Dist: numpy
-(>=1.20.3,<2.0.0) Requires-Dist: opencv-python (>=4.5.2,<5.0.0) Project-URL:
-Bug Tracker, https://github.com/exler/CILISSA/issues Project-URL: Repository,
-https://github.com/exler/CILISSA Description-Content-Type: text/markdown
+:: Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Topic :: Scientific/Engineering :: Image Processing
+Provides-Extra: gui Requires-Dist: PySide6 (>=6.7.0,<7.0.0) ; extra == "gui"
+Requires-Dist: numpy (>=1.26.4,<2.0.0) Requires-Dist: opencv-python
+(>=4.9.0.80,<5.0.0.0) Project-URL: Bug Tracker, https://github.com/exler/
+CILISSA/issues Project-URL: Repository, https://github.com/exler/CILISSA
+Description-Content-Type: text/markdown
  [https://raw.githubusercontent.com/exler/CILISSA/main/docs/_static/logo.png]
                  CComputer IImage LLiikeness Assssessing AAutomation
   [https://github.com/exler/CILISSA/actions/workflows/quality.yml/badge.svg]
 [https://github.com/exler/CILISSA/actions/workflows/tests.yml/badge.svg]_[_h_t_t_p_s_:
   _/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_e_x_l_e_r_/_C_I_L_I_S_S_A_/_b_r_a_n_c_h_/_m_a_i_n_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_D_i_x_b_5_b_u_M_Q_r_]
                  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_r_e_a_d_t_h_e_d_o_c_s_/_c_i_l_i_s_s_a_]
 ## Overview CILISSA allows for the use of various metrics to perform full-
 reference image comparisons. It features the most popular full-reference image
 quality metrics, image transformations and translations. CILISSA is also very
 extensible and new operations can be easily added. CILISSA has an optional Qt-
 based graphical interface that lets you experiment with various operations,
-their orders and properties. ## Requirements * Python >= 3.7 ## Installation
-### Install from PyPI ```bash $ pip install cilissa ``` ### Releases Binaries
-for Windows and Linux can be found on [GitHub releases](https://github.com/
-exler/CILISSA/releases). ## Usage ### GUI Information about the GUI can be
-found in the [cilissa_gui/README.md](cilissa_gui/README.md) file. ### CLI
-Currently the CLI only supports working with a single pair of images. The
-parameters of metrics and transformations can be modified by passing them to
-the `--kwargs` argument using the following format: ``` -= ``` where
-`parameter-name` uses hyphens (-) instead of underscores (_) ## Documentation
-Documentation is hosted on [Read the Docs](https://cilissa.readthedocs.io/).
+their orders and properties. ## Requirements * Python >=3.9,<3.12 ##
+Installation ### Install from PyPI ```bash $ pip install cilissa ``` ###
+Releases Binaries for Windows and Linux can be found on [GitHub releases]
+(https://github.com/exler/CILISSA/releases). ## Usage ### GUI Information about
+the GUI can be found in the [cilissa_gui/README.md](cilissa_gui/README.md)
+file. ### CLI Currently the CLI only supports working with a single pair of
+images. The parameters of metrics and transformations can be modified by
+passing them to the `--kwargs` argument using the following format: ``` -= ```
+where `parameter-name` uses hyphens (-) instead of underscores (_) ##
+Documentation Documentation is hosted on [Read the Docs](https://
+cilissa.readthedocs.io/). ## License `CILISSA` is under the terms of the [MIT
+License](https://www.tldrlegal.com/l/mit), following all clarifications stated
+in the [license file](LICENSE).
```

