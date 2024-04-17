# Comparing `tmp/lvc-1.0.tar.gz` & `tmp/lvc-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lvc-1.0.tar", last modified: Wed Apr 17 01:18:54 2024, max compression
+gzip compressed data, was "lvc-1.0.1.tar", last modified: Wed Apr 17 01:25:09 2024, max compression
```

## Comparing `lvc-1.0.tar` & `lvc-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-17 01:18:54.315785 lvc-1.0/
--rw-r--r--   0 benjaminlee   (501) staff       (20)     1086 2024-04-17 00:55:00.000000 lvc-1.0/LICENSE
--rw-r--r--   0 benjaminlee   (501) staff       (20)     1229 2024-04-17 01:18:54.315528 lvc-1.0/PKG-INFO
--rw-r--r--   0 benjaminlee   (501) staff       (20)      668 2024-04-17 01:15:40.000000 lvc-1.0/README.md
-drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-17 01:18:54.312872 lvc-1.0/lvc/
--rw-r--r--   0 benjaminlee   (501) staff       (20)     9955 2024-04-17 01:13:16.000000 lvc-1.0/lvc/__init__.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)    14165 2024-04-17 01:11:34.000000 lvc-1.0/lvc/dataset.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)     7131 2024-04-17 01:11:40.000000 lvc-1.0/lvc/inference_spect.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)     9819 2024-04-17 01:11:43.000000 lvc-1.0/lvc/inference_wav2vec.py
-drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-17 01:18:54.315228 lvc-1.0/lvc/model/
--rw-r--r--   0 benjaminlee   (501) staff       (20)     3537 2024-04-17 00:30:05.000000 lvc-1.0/lvc/model/ResNetBlocks.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)     6533 2024-04-17 00:30:05.000000 lvc-1.0/lvc/model/ResNetSE34L.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)        0 2024-04-17 00:30:05.000000 lvc-1.0/lvc/model/__init__.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)      878 2024-04-17 00:30:05.000000 lvc-1.0/lvc/model/discriminator.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)     6783 2024-04-17 00:30:05.000000 lvc-1.0/lvc/model/ecapa_tdnn.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)     4934 2024-04-17 00:30:05.000000 lvc-1.0/lvc/model/generator.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)    12606 2024-04-17 00:30:05.000000 lvc-1.0/lvc/model/lvcnet.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)     2649 2024-04-17 00:30:05.000000 lvc-1.0/lvc/model/mpd.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)     3144 2024-04-17 00:30:05.000000 lvc-1.0/lvc/model/mrd.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)     1632 2024-04-17 00:30:05.000000 lvc-1.0/lvc/model/ssc.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)    15041 2024-04-17 01:11:47.000000 lvc-1.0/lvc/train.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)     1040 2024-04-17 00:30:05.000000 lvc-1.0/lvc/trainer.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)     3660 2024-04-17 00:30:05.000000 lvc-1.0/lvc/validation.py
--rw-r--r--   0 benjaminlee   (501) staff       (20)     9442 2024-04-17 01:11:16.000000 lvc-1.0/lvc/weights.py
-drwxr-xr-x   0 benjaminlee   (501) staff       (20)        0 2024-04-17 01:18:54.313640 lvc-1.0/lvc.egg-info/
--rw-r--r--   0 benjaminlee   (501) staff       (20)     1229 2024-04-17 01:18:54.000000 lvc-1.0/lvc.egg-info/PKG-INFO
--rw-r--r--   0 benjaminlee   (501) staff       (20)      518 2024-04-17 01:18:54.000000 lvc-1.0/lvc.egg-info/SOURCES.txt
--rw-r--r--   0 benjaminlee   (501) staff       (20)        1 2024-04-17 01:18:54.000000 lvc-1.0/lvc.egg-info/dependency_links.txt
--rw-r--r--   0 benjaminlee   (501) staff       (20)      128 2024-04-17 01:18:54.000000 lvc-1.0/lvc.egg-info/requires.txt
--rw-r--r--   0 benjaminlee   (501) staff       (20)        4 2024-04-17 01:18:54.000000 lvc-1.0/lvc.egg-info/top_level.txt
--rw-r--r--   0 benjaminlee   (501) staff       (20)       38 2024-04-17 01:18:54.315841 lvc-1.0/setup.cfg
--rw-r--r--   0 benjaminlee   (501) staff       (20)      704 2024-04-17 01:16:31.000000 lvc-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:25:09.919911 lvc-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-17 01:25:01.000000 lvc-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-17 01:25:09.919911 lvc-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-17 01:25:01.000000 lvc-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:25:09.915911 lvc-1.0.1/lvc/
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-17 01:25:01.000000 lvc-1.0.1/lvc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14165 2024-04-17 01:25:01.000000 lvc-1.0.1/lvc/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-04-17 01:25:01.000000 lvc-1.0.1/lvc/inference_spect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9819 2024-04-17 01:25:01.000000 lvc-1.0.1/lvc/inference_wav2vec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:25:09.919911 lvc-1.0.1/lvc/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-17 01:25:01.000000 lvc-1.0.1/lvc/model/ResNetBlocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-04-17 01:25:01.000000 lvc-1.0.1/lvc/model/ResNetSE34L.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 01:25:01.000000 lvc-1.0.1/lvc/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-17 01:25:01.000000 lvc-1.0.1/lvc/model/discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-04-17 01:25:01.000000 lvc-1.0.1/lvc/model/ecapa_tdnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-17 01:25:01.000000 lvc-1.0.1/lvc/model/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12606 2024-04-17 01:25:01.000000 lvc-1.0.1/lvc/model/lvcnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-17 01:25:01.000000 lvc-1.0.1/lvc/model/mpd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-17 01:25:01.000000 lvc-1.0.1/lvc/model/mrd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-17 01:25:01.000000 lvc-1.0.1/lvc/model/ssc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15041 2024-04-17 01:25:01.000000 lvc-1.0.1/lvc/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-17 01:25:01.000000 lvc-1.0.1/lvc/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-17 01:25:01.000000 lvc-1.0.1/lvc/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-04-17 01:25:01.000000 lvc-1.0.1/lvc/weights.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:25:09.919911 lvc-1.0.1/lvc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-17 01:25:09.000000 lvc-1.0.1/lvc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-17 01:25:09.000000 lvc-1.0.1/lvc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 01:25:09.000000 lvc-1.0.1/lvc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-17 01:25:09.000000 lvc-1.0.1/lvc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-17 01:25:09.000000 lvc-1.0.1/lvc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 01:25:09.919911 lvc-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-17 01:25:01.000000 lvc-1.0.1/setup.py
```

### Comparing `lvc-1.0/LICENSE` & `lvc-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lvc-1.0/PKG-INFO` & `lvc-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lvc
-Version: 1.0
+Version: 1.0.1
 Summary: Unofficial pip package for zero-shot voice conversion
 Home-page: https://github.com/fakerybakery/lvc
 Author: mrfakename
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: librosa
 Requires-Dist: soundfile
@@ -18,15 +18,15 @@
 Requires-Dist: torchaudio
 Requires-Dist: tqdm
 Requires-Dist: transformers
 Requires-Dist: cached_path
 
 # LVC
 
-Unofficial package for LVC-VC (zero-shot voice conversion) by Wonjune Kang, Mark Hasegawa-Johnson, Deb Roy.
+Unofficial pip-installable Python package for [LVC-VC](https://github.com/wonjune-kang/lvc-vc) (zero-shot voice conversion) by Wonjune Kang, Mark Hasegawa-Johnson, Deb Roy.
 
 ## Installation
 
 ```
 pip install lvc
 ```
```

### Comparing `lvc-1.0/README.md` & `lvc-1.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # LVC
 
-Unofficial package for LVC-VC (zero-shot voice conversion) by Wonjune Kang, Mark Hasegawa-Johnson, Deb Roy.
+Unofficial pip-installable Python package for [LVC-VC](https://github.com/wonjune-kang/lvc-vc) (zero-shot voice conversion) by Wonjune Kang, Mark Hasegawa-Johnson, Deb Roy.
 
 ## Installation
 
 ```
 pip install lvc
 ```
```

### Comparing `lvc-1.0/lvc/__init__.py` & `lvc-1.0.1/lvc/__init__.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0/lvc/dataset.py` & `lvc-1.0.1/lvc/dataset.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0/lvc/inference_spect.py` & `lvc-1.0.1/lvc/inference_spect.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0/lvc/inference_wav2vec.py` & `lvc-1.0.1/lvc/inference_wav2vec.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0/lvc/model/ResNetBlocks.py` & `lvc-1.0.1/lvc/model/ResNetBlocks.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0/lvc/model/ResNetSE34L.py` & `lvc-1.0.1/lvc/model/ResNetSE34L.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0/lvc/model/discriminator.py` & `lvc-1.0.1/lvc/model/discriminator.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0/lvc/model/ecapa_tdnn.py` & `lvc-1.0.1/lvc/model/ecapa_tdnn.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0/lvc/model/generator.py` & `lvc-1.0.1/lvc/model/generator.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0/lvc/model/lvcnet.py` & `lvc-1.0.1/lvc/model/lvcnet.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0/lvc/model/mpd.py` & `lvc-1.0.1/lvc/model/mpd.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-from torch.nn.utils import weight_norm, spectral_norm
-
-class DiscriminatorP(nn.Module):
-    def __init__(self, hp, period):
-        super(DiscriminatorP, self).__init__()
-
-        self.LRELU_SLOPE = hp.mpd.lReLU_slope
-        self.period = period
-
-        kernel_size = hp.mpd.kernel_size
-        stride = hp.mpd.stride
-        norm_f = weight_norm if hp.mpd.use_spectral_norm == False else spectral_norm
-
-        self.convs = nn.ModuleList([
-            norm_f(nn.Conv2d(1, 64, (kernel_size, 1), (stride, 1), padding=(kernel_size // 2, 0))),
-            norm_f(nn.Conv2d(64, 128, (kernel_size, 1), (stride, 1), padding=(kernel_size // 2, 0))),
-            norm_f(nn.Conv2d(128, 256, (kernel_size, 1), (stride, 1), padding=(kernel_size // 2, 0))),
-            norm_f(nn.Conv2d(256, 512, (kernel_size, 1), (stride, 1), padding=(kernel_size // 2, 0))),
-            norm_f(nn.Conv2d(512, 1024, (kernel_size, 1), 1, padding=(kernel_size // 2, 0))),
-        ])
-        self.conv_post = norm_f(nn.Conv2d(1024, 1, (3, 1), 1, padding=(1, 0)))
-
-    def forward(self, x):
-        fmap = []
-
-        # Convert 1D time domain signal to 2D.
-        b, c, t = x.shape
-        if t % self.period != 0: # pad first
-            n_pad = self.period - (t % self.period)
-            x = F.pad(x, (0, n_pad), "reflect")
-            t = t + n_pad
-
-        # Reshape to match the given period in one dimension.
-        x = x.view(b, c, t // self.period, self.period)
-
-        # Pass reshaped signal through convolutional disciminator network.
-        for l in self.convs:
-            x = l(x)
-            x = F.leaky_relu(x, self.LRELU_SLOPE)
-            fmap.append(x)
-        x = self.conv_post(x)
-
-        # fmap is list of discriminator's layer-wise feature map outputs
-        # (for feature matching loss in HiFi-GAN; unused in UnivNet).
-        fmap.append(x)
-
-        # x is 1D tensor of frame-wise discriminator scores (0-1).
-        x = torch.flatten(x, 1, -1)
-
-        return fmap, x
-
-
-class MultiPeriodDiscriminator(nn.Module):
-    def __init__(self, hp):
-        super(MultiPeriodDiscriminator, self).__init__()
-
-        # Initialize discriminators for prime numbered periods.
-        self.discriminators = nn.ModuleList(
-            [DiscriminatorP(hp, period) for period in hp.mpd.periods]
-        )
-
-    def forward(self, x):
-        ret = list()
-        for disc in self.discriminators:
-            ret.append(disc(x))
-
-        return ret  # [(feat, score), (feat, score), (feat, score), (feat, score), (feat, score)]
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+from torch.nn.utils import weight_norm, spectral_norm
+
+class DiscriminatorP(nn.Module):
+    def __init__(self, hp, period):
+        super(DiscriminatorP, self).__init__()
+
+        self.LRELU_SLOPE = hp.mpd.lReLU_slope
+        self.period = period
+
+        kernel_size = hp.mpd.kernel_size
+        stride = hp.mpd.stride
+        norm_f = weight_norm if hp.mpd.use_spectral_norm == False else spectral_norm
+
+        self.convs = nn.ModuleList([
+            norm_f(nn.Conv2d(1, 64, (kernel_size, 1), (stride, 1), padding=(kernel_size // 2, 0))),
+            norm_f(nn.Conv2d(64, 128, (kernel_size, 1), (stride, 1), padding=(kernel_size // 2, 0))),
+            norm_f(nn.Conv2d(128, 256, (kernel_size, 1), (stride, 1), padding=(kernel_size // 2, 0))),
+            norm_f(nn.Conv2d(256, 512, (kernel_size, 1), (stride, 1), padding=(kernel_size // 2, 0))),
+            norm_f(nn.Conv2d(512, 1024, (kernel_size, 1), 1, padding=(kernel_size // 2, 0))),
+        ])
+        self.conv_post = norm_f(nn.Conv2d(1024, 1, (3, 1), 1, padding=(1, 0)))
+
+    def forward(self, x):
+        fmap = []
+
+        # Convert 1D time domain signal to 2D.
+        b, c, t = x.shape
+        if t % self.period != 0: # pad first
+            n_pad = self.period - (t % self.period)
+            x = F.pad(x, (0, n_pad), "reflect")
+            t = t + n_pad
+
+        # Reshape to match the given period in one dimension.
+        x = x.view(b, c, t // self.period, self.period)
+
+        # Pass reshaped signal through convolutional disciminator network.
+        for l in self.convs:
+            x = l(x)
+            x = F.leaky_relu(x, self.LRELU_SLOPE)
+            fmap.append(x)
+        x = self.conv_post(x)
+
+        # fmap is list of discriminator's layer-wise feature map outputs
+        # (for feature matching loss in HiFi-GAN; unused in UnivNet).
+        fmap.append(x)
+
+        # x is 1D tensor of frame-wise discriminator scores (0-1).
+        x = torch.flatten(x, 1, -1)
+
+        return fmap, x
+
+
+class MultiPeriodDiscriminator(nn.Module):
+    def __init__(self, hp):
+        super(MultiPeriodDiscriminator, self).__init__()
+
+        # Initialize discriminators for prime numbered periods.
+        self.discriminators = nn.ModuleList(
+            [DiscriminatorP(hp, period) for period in hp.mpd.periods]
+        )
+
+    def forward(self, x):
+        ret = list()
+        for disc in self.discriminators:
+            ret.append(disc(x))
+
+        return ret  # [(feat, score), (feat, score), (feat, score), (feat, score), (feat, score)]
```

### Comparing `lvc-1.0/lvc/model/ssc.py` & `lvc-1.0.1/lvc/model/ssc.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0/lvc/train.py` & `lvc-1.0.1/lvc/train.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0/lvc/trainer.py` & `lvc-1.0.1/lvc/trainer.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0/lvc/validation.py` & `lvc-1.0.1/lvc/validation.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0/lvc/weights.py` & `lvc-1.0.1/lvc/weights.py`

 * *Files identical despite different names*

### Comparing `lvc-1.0/lvc.egg-info/PKG-INFO` & `lvc-1.0.1/lvc.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lvc
-Version: 1.0
+Version: 1.0.1
 Summary: Unofficial pip package for zero-shot voice conversion
 Home-page: https://github.com/fakerybakery/lvc
 Author: mrfakename
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: librosa
 Requires-Dist: soundfile
@@ -18,15 +18,15 @@
 Requires-Dist: torchaudio
 Requires-Dist: tqdm
 Requires-Dist: transformers
 Requires-Dist: cached_path
 
 # LVC
 
-Unofficial package for LVC-VC (zero-shot voice conversion) by Wonjune Kang, Mark Hasegawa-Johnson, Deb Roy.
+Unofficial pip-installable Python package for [LVC-VC](https://github.com/wonjune-kang/lvc-vc) (zero-shot voice conversion) by Wonjune Kang, Mark Hasegawa-Johnson, Deb Roy.
 
 ## Installation
 
 ```
 pip install lvc
 ```
```

### Comparing `lvc-1.0/lvc.egg-info/SOURCES.txt` & `lvc-1.0.1/lvc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lvc-1.0/setup.py` & `lvc-1.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     longdesc = f.read()
 setup(
     name="lvc",
-    version="1.0",
+    version="1.0.1",
     author="mrfakename",
     description="Unofficial pip package for zero-shot voice conversion",
     long_description=longdesc,
     long_description_content_type="text/markdown",
     url="https://github.com/fakerybakery/lvc",
     packages=find_packages(),
     install_requires=[
```

