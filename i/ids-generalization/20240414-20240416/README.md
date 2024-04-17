# Comparing `tmp/ids_generalization-20240414-py3-none-any.whl.zip` & `tmp/ids_generalization-20240416-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,42 +1,36 @@
-Zip file size: 37296 bytes, number of entries: 40
--rw-rw-r--  2.0 unx      804 b- defN 23-Nov-07 18:08 generalization/__init__.py
--rw-rw-r--  2.0 unx       25 b- defN 24-Apr-14 23:06 generalization/version.py
--rw-rw-r--  2.0 unx      272 b- defN 23-Nov-07 18:08 generalization/models/__init__.py
--rw-rw-r--  2.0 unx     3817 b- defN 23-Nov-07 18:22 generalization/models/factory.py
--rw-rw-r--  2.0 unx      253 b- defN 23-Nov-07 18:08 generalization/models/jax/__init__.py
--rw-rw-r--  2.0 unx     3792 b- defN 23-Nov-07 18:08 generalization/models/jax/alexnet.py
--rw-rw-r--  2.0 unx    10649 b- defN 23-Nov-07 18:08 generalization/models/jax/inception.py
+Zip file size: 32495 bytes, number of entries: 34
+-rw-rw-r--  2.0 unx      503 b- defN 24-Apr-17 03:03 generalization/__init__.py
+-rw-rw-r--  2.0 unx       25 b- defN 24-Apr-17 03:14 generalization/version.py
+-rw-rw-r--  2.0 unx      272 b- defN 24-Apr-15 17:11 generalization/models/__init__.py
+-rw-rw-r--  2.0 unx     4337 b- defN 24-Apr-16 23:23 generalization/models/factory.py
 -rw-rw-r--  2.0 unx      325 b- defN 23-Nov-07 18:08 generalization/models/pytorch/__init__.py
--rw-rw-r--  2.0 unx     1458 b- defN 23-Nov-07 18:08 generalization/models/pytorch/alexnet.py
--rw-rw-r--  2.0 unx     3218 b- defN 23-Nov-07 18:08 generalization/models/pytorch/inception.py
--rw-rw-r--  2.0 unx      979 b- defN 23-Nov-07 18:08 generalization/models/pytorch/mlp.py
--rw-rw-r--  2.0 unx      386 b- defN 23-Nov-07 18:08 generalization/models/pytorch/resnet.py
--rw-rw-r--  2.0 unx      376 b- defN 23-Nov-07 18:08 generalization/randomization/__init__.py
--rw-rw-r--  2.0 unx     2110 b- defN 23-Nov-07 18:08 generalization/randomization/builders.py
--rw-rw-r--  2.0 unx     4945 b- defN 23-Nov-07 18:08 generalization/randomization/corruptions.py
--rw-rw-r--  2.0 unx     8863 b- defN 23-Nov-07 18:08 generalization/randomization/dataset.py
--rw-rw-r--  2.0 unx      752 b- defN 23-Nov-07 18:39 generalization/randomization/transforms.py
--rw-rw-r--  2.0 unx     5105 b- defN 23-Nov-07 18:08 generalization/randomization/utils.py
+-rw-rw-r--  2.0 unx     2040 b- defN 24-Apr-15 17:08 generalization/models/pytorch/alexnet.py
+-rw-rw-r--  2.0 unx     4373 b- defN 24-Apr-15 17:11 generalization/models/pytorch/inception.py
+-rw-rw-r--  2.0 unx     1334 b- defN 24-Apr-15 17:16 generalization/models/pytorch/mlp.py
+-rw-rw-r--  2.0 unx      590 b- defN 24-Apr-15 17:13 generalization/models/pytorch/resnet.py
+-rw-rw-r--  2.0 unx      230 b- defN 24-Apr-15 15:12 generalization/randomization/__init__.py
+-rw-rw-r--  2.0 unx     3526 b- defN 24-Apr-16 23:32 generalization/randomization/builders.py
+-rw-rw-r--  2.0 unx     4925 b- defN 24-Apr-15 15:19 generalization/randomization/corruptions.py
+-rw-rw-r--  2.0 unx    14672 b- defN 24-Apr-16 22:08 generalization/randomization/dataset.py
+-rw-rw-r--  2.0 unx      752 b- defN 24-Apr-16 22:34 generalization/randomization/transforms.py
+-rw-rw-r--  2.0 unx     5169 b- defN 24-Apr-17 03:06 generalization/randomization/utils.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Nov-07 18:08 generalization/randomization/inputs/__init__.py
--rw-rw-r--  2.0 unx      863 b- defN 23-Nov-07 18:08 generalization/randomization/inputs/gaussian_pixels.py
--rw-rw-r--  2.0 unx      814 b- defN 23-Sep-27 18:41 generalization/randomization/inputs/random_labels.py
--rw-rw-r--  2.0 unx     1347 b- defN 23-Nov-07 18:08 generalization/randomization/inputs/random_pixels.py
--rw-rw-r--  2.0 unx     1817 b- defN 23-Nov-07 18:08 generalization/randomization/inputs/shuffled_pixels.py
+-rw-rw-r--  2.0 unx      860 b- defN 24-Apr-15 19:50 generalization/randomization/inputs/gaussian_pixels.py
+-rw-rw-r--  2.0 unx     1016 b- defN 24-Apr-15 18:06 generalization/randomization/inputs/random_pixels.py
+-rw-rw-r--  2.0 unx     1823 b- defN 24-Apr-15 18:06 generalization/randomization/inputs/shuffled_pixels.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Nov-07 18:08 generalization/randomization/labels/__init__.py
--rw-rw-r--  2.0 unx      878 b- defN 23-Sep-27 18:40 generalization/randomization/labels/gaussian_pixels.py
--rw-rw-r--  2.0 unx      797 b- defN 23-Nov-07 18:08 generalization/randomization/labels/partial_labels.py
--rw-rw-r--  2.0 unx      858 b- defN 23-Nov-07 18:08 generalization/randomization/labels/random_labels.py
--rw-rw-r--  2.0 unx     1309 b- defN 23-Sep-27 18:41 generalization/randomization/labels/random_pixels.py
--rw-rw-r--  2.0 unx     1897 b- defN 23-Sep-27 18:40 generalization/randomization/labels/shuffled_pixels.py
--rw-rw-r--  2.0 unx      315 b- defN 23-Nov-07 18:08 generalization/utils/__init__.py
--rw-rw-r--  2.0 unx     2755 b- defN 23-Nov-07 18:08 generalization/utils/data.py
--rw-rw-r--  2.0 unx    13516 b- defN 23-Nov-07 18:08 generalization/utils/model.py
+-rw-rw-r--  2.0 unx      803 b- defN 24-Apr-15 18:06 generalization/randomization/labels/partial_labels.py
+-rw-rw-r--  2.0 unx      749 b- defN 24-Apr-15 18:06 generalization/randomization/labels/random_labels.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-Apr-15 21:48 generalization/utils/__init__.py
+-rw-rw-r--  2.0 unx      573 b- defN 24-Apr-17 02:59 generalization/utils/data.py
+-rw-rw-r--  2.0 unx     2557 b- defN 24-Apr-16 23:30 generalization/utils/experiment.py
+-rw-rw-r--  2.0 unx    13144 b- defN 24-Apr-17 03:00 generalization/utils/model.py
 -rw-rw-r--  2.0 unx      574 b- defN 23-Nov-07 18:40 generalization/utils/scores.py
--rw-rw-r--  2.0 unx     7366 b- defN 23-Nov-07 18:08 generalization/utils/train.py
+-rw-rw-r--  2.0 unx     7961 b- defN 24-Apr-17 03:01 generalization/utils/train.py
 -rw-rw-r--  2.0 unx     5290 b- defN 23-Aug-31 18:09 generalization/utils/viz.py
--rw-rw-r--  2.0 unx     1497 b- defN 24-Apr-14 23:09 ids_generalization-20240414.dist-info/LICENSE
--rw-rw-r--  2.0 unx     5215 b- defN 24-Apr-14 23:09 ids_generalization-20240414.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-14 23:09 ids_generalization-20240414.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 24-Apr-14 23:09 ids_generalization-20240414.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     3842 b- defN 24-Apr-14 23:09 ids_generalization-20240414.dist-info/RECORD
-40 files, 99186 bytes uncompressed, 30952 bytes compressed:  68.8%
+-rw-r--r--  2.0 unx     1497 b- defN 24-Apr-17 03:15 ids_generalization-20240416.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     4734 b- defN 24-Apr-17 03:15 ids_generalization-20240416.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-17 03:15 ids_generalization-20240416.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 24-Apr-17 03:15 ids_generalization-20240416.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3212 b- defN 24-Apr-17 03:15 ids_generalization-20240416.dist-info/RECORD
+34 files, 87973 bytes uncompressed, 27185 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -6,23 +6,14 @@
 
 Filename: generalization/models/__init__.py
 Comment: 
 
 Filename: generalization/models/factory.py
 Comment: 
 
-Filename: generalization/models/jax/__init__.py
-Comment: 
-
-Filename: generalization/models/jax/alexnet.py
-Comment: 
-
-Filename: generalization/models/jax/inception.py
-Comment: 
-
 Filename: generalization/models/pytorch/__init__.py
 Comment: 
 
 Filename: generalization/models/pytorch/alexnet.py
 Comment: 
 
 Filename: generalization/models/pytorch/inception.py
@@ -54,68 +45,59 @@
 
 Filename: generalization/randomization/inputs/__init__.py
 Comment: 
 
 Filename: generalization/randomization/inputs/gaussian_pixels.py
 Comment: 
 
-Filename: generalization/randomization/inputs/random_labels.py
-Comment: 
-
 Filename: generalization/randomization/inputs/random_pixels.py
 Comment: 
 
 Filename: generalization/randomization/inputs/shuffled_pixels.py
 Comment: 
 
 Filename: generalization/randomization/labels/__init__.py
 Comment: 
 
-Filename: generalization/randomization/labels/gaussian_pixels.py
-Comment: 
-
 Filename: generalization/randomization/labels/partial_labels.py
 Comment: 
 
 Filename: generalization/randomization/labels/random_labels.py
 Comment: 
 
-Filename: generalization/randomization/labels/random_pixels.py
-Comment: 
-
-Filename: generalization/randomization/labels/shuffled_pixels.py
-Comment: 
-
 Filename: generalization/utils/__init__.py
 Comment: 
 
 Filename: generalization/utils/data.py
 Comment: 
 
+Filename: generalization/utils/experiment.py
+Comment: 
+
 Filename: generalization/utils/model.py
 Comment: 
 
 Filename: generalization/utils/scores.py
 Comment: 
 
 Filename: generalization/utils/train.py
 Comment: 
 
 Filename: generalization/utils/viz.py
 Comment: 
 
-Filename: ids_generalization-20240414.dist-info/LICENSE
+Filename: ids_generalization-20240416.dist-info/LICENSE
 Comment: 
 
-Filename: ids_generalization-20240414.dist-info/METADATA
+Filename: ids_generalization-20240416.dist-info/METADATA
 Comment: 
 
-Filename: ids_generalization-20240414.dist-info/WHEEL
+Filename: ids_generalization-20240416.dist-info/WHEEL
 Comment: 
 
-Filename: ids_generalization-20240414.dist-info/top_level.txt
+Filename: ids_generalization-20240416.dist-info/top_level.txt
 Comment: 
 
-Filename: ids_generalization-20240414.dist-info/RECORD
+Filename: ids_generalization-20240416.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## generalization/__init__.py

```diff
@@ -1,34 +1,28 @@
-from torchvision.datasets import CIFAR10
-
-from .randomization import RandomizedDataset
-from .utils.data import DEFAULT_PARAMS, build_experiment, get_num_cpus
+from .randomization import (
+    RandomizedDataset,
+    create_corrupted_dataset,
+    get_randomization,
+)
+from .utils.data import seed_everything
 
 """
 This file contains the functions to load the datasets.
 
 corruption_name must be one of the following:
 
 "random_labels"
 "partial_labels"
 "gaussian_pixels"
 "random_pixels"
 "shuffled_pixels"
 """
 
-corruptions = [
+CORRUPTIONS = [
     "random_labels",
     "partial_labels",
     "gaussian_pixels",
     "random_pixels",
     "shuffled_pixels",
 ]
 
-
-def load_randomized_cifar10(corruption_name, corruption_prob=0.3, train=True):
-    return RandomizedDataset(
-        CIFAR10(root="./data/cifar10", download=True, train=train),
-        corruption_name=corruption_name,
-        corruption_prob=corruption_prob,
-        apply_corruption=False,
-        train=train,
-    )
+RANDOMIZATIONS = CORRUPTIONS
```

## generalization/version.py

```diff
@@ -1 +1 @@
-__version__ = "20240414"
+__version__ = "20240416"
```

## generalization/models/factory.py

```diff
@@ -4,136 +4,140 @@
 2. CIFAR10: A smaller version of Inception,
             Alexnet (Krizhevsky et al., 2012),
             MLPs with 1 and 3 hidden layers
 
 Author: Stepp1
 """
 
-
 from functools import partial
 
-import jax
+JAX_ERROR = NotImplementedError("JAX models will not be implemented.")
 
 
 class ModelFactory:
     def __init__(self):
         self.lib: str = None
         self.key = None
         self.model_creators_torch = {
             "resnet18": partial(create_resnet, resnet_size=18, lib="torch"),
             "resnet34": partial(create_resnet, resnet_size=34, lib="torch"),
             "alexnet": partial(create_alexnet, lib="torch"),
             "mlp_1x512": partial(
                 create_mlp,
-                in_size=28 * 28 * 3,
                 hidden_sizes=[512],
                 out_size=10,
                 lib="torch",
             ),
             "mlp_3x512": partial(
                 create_mlp,
-                in_size=28 * 28 * 3,
                 hidden_sizes=[512] * 3,
                 out_size=10,
                 lib="torch",
             ),
             "inception": partial(create_inception, lib="torch"),
         }
 
+        try:
+            assert self.lib != "jax"
+        except AssertionError:
+            raise JAX_ERROR
+
     def create_model(self, model_type: str, lib: str = None, **kwargs):
         self.lib = lib or self.lib
         if self.lib == "jax":
-            raise NotImplementedError
-
+            raise JAX_ERROR
         elif self.lib == "torch":
             model = self.model_creators_torch[model_type](**kwargs)
-
         else:
             raise ValueError(f"Unknown library: {self.lib}")
 
         return model
 
-    def get_cifar_models(self, model_name: str = None, lib: str = "torch"):
+    def get_cifar_models(self, model_name: str = None, lib: str = "torch", **kwargs):
         self.lib = lib or self.lib
         models = {
-            "resnet18": self.create_model("resnet18", cifar=True),
-            "alexnet": self.create_model("alexnet", cifar=True),
-            "inception": self.create_model("inception", cifar=True),
-            "mlp_3x512": self.create_model("mlp_3x512"),
+            "resnet18": self.create_model("resnet18", cifar=True, **kwargs),
+            "alexnet": self.create_model("alexnet", cifar=True, **kwargs),
+            "inception": self.create_model("inception", cifar=True, **kwargs),
+            "mlp_3x512": self.create_model("mlp_3x512", **kwargs),
         }
         return models if model_name is None else {model_name: models[model_name]}
 
     def get_imagenet_models(self, model_name: str = None, lib: str = "torch"):
         self.lib = lib or self.lib
         models = {
             "inception": self.create_model("inception"),
             "resnet18": self.create_model("resnet18"),
             "resnet34": self.create_model("resnet34"),
         }
 
         return models if model_name is None else {model_name: models[model_name]}
 
 
-def create_mlp(
-    in_size: int, hidden_sizes: int, out_size: int, lib: str = "torch", key=None
-):
+def create_mlp(hidden_sizes: int, out_size: int, lib: str = "torch", **kwargs):
     if lib == "jax":
-        raise NotImplementedError
+        raise JAX_ERROR
     elif lib == "torch":
         from .pytorch import mlp
 
-        model = mlp(in_size, hidden_sizes, out_size)
-
+        in_size = kwargs.get("in_size", 3 * 32 * 32)
+        if "in_size" in kwargs:
+            kwargs.pop("in_size")
+        model = mlp(
+            in_size=in_size, hidden_sizes=hidden_sizes, out_size=out_size, **kwargs
+        )
     else:
         raise ValueError(f"Unknown library: {lib}")
 
     return model
 
 
 def create_resnet(
     resnet_size: int = 18,
     weights: str = None,
     cifar: bool = False,
     lib: str = "torch",
+    **kwargs,
 ):
     if lib == "jax":
-        raise NotImplementedError
-
+        raise JAX_ERROR
     elif lib == "torch":
         from .pytorch import resnet
 
-        model = resnet(resnet_size=resnet_size, weights=weights, cifar=cifar)
-
+        if "in_size" in kwargs:
+            kwargs.pop("in_size")
+        model = resnet(resnet_size=resnet_size, weights=weights, cifar=cifar, **kwargs)
     else:
         raise ValueError(f"Unknown library: {lib}")
 
     return model
 
 
-def create_alexnet(weights=None, cifar=False, lib="torch"):
+def create_alexnet(weights=None, cifar=False, lib="torch", **kwargs):
     if lib == "jax":
-        raise NotImplementedError
-
+        raise JAX_ERROR
     elif lib == "torch":
         from .pytorch import alexnet
 
-        model = alexnet(weights=weights, cifar=cifar)
-
+        if "in_size" in kwargs:
+            kwargs.pop("in_size")
+        model = alexnet(weights=weights, cifar=cifar, **kwargs)
     else:
         raise ValueError(f"Unknown library: {lib}")
 
     return model
 
 
-def create_inception(weights=None, cifar=False, small="False", lib="torch"):
+def create_inception(weights=None, cifar=False, small="False", lib="torch", **kwargs):
     cifar = small or cifar
     if lib == "jax":
         raise NotImplementedError
-
     elif lib == "torch":
         from .pytorch import inception
 
-        model = inception(weights=weights, cifar=cifar)
+        if "in_size" in kwargs:
+            kwargs.pop("in_size")
+        model = inception(weights=weights, cifar=cifar, **kwargs)
     else:
         raise ValueError(f"Unknown library: {lib}")
 
     return model
```

## generalization/models/pytorch/alexnet.py

```diff
@@ -1,47 +1,58 @@
 import torch.nn as nn
 import torchvision
 
 NUM_CLASSES = 10
 
 
 class SmallAlexNet(nn.Module):
-    def __init__(self, num_classes=NUM_CLASSES):
+    def __init__(
+        self,
+        num_classes=NUM_CLASSES,
+        use_batch_norm=False,
+        use_dropout=False,
+        dropout_rate=0.5,
+    ):
         super(SmallAlexNet, self).__init__()
         self.features = nn.Sequential(
             nn.Conv2d(3, 64, kernel_size=3, stride=2, padding=1),
+            nn.BatchNorm2d(64) if use_batch_norm else nn.Identity(),
             nn.LeakyReLU(),
             nn.MaxPool2d(kernel_size=2),
             nn.Conv2d(64, 192, kernel_size=3, padding=1),
+            nn.BatchNorm2d(192) if use_batch_norm else nn.Identity(),
             nn.LeakyReLU(),
             nn.MaxPool2d(kernel_size=2),
             nn.Conv2d(192, 384, kernel_size=3, padding=1),
+            nn.BatchNorm2d(384) if use_batch_norm else nn.Identity(),
             nn.LeakyReLU(),
             nn.Conv2d(384, 256, kernel_size=3, padding=1),
+            nn.BatchNorm2d(256) if use_batch_norm else nn.Identity(),
             nn.LeakyReLU(),
             nn.Conv2d(256, 256, kernel_size=3, padding=1),
+            nn.BatchNorm2d(256) if use_batch_norm else nn.Identity(),
             nn.LeakyReLU(),
             nn.MaxPool2d(kernel_size=2),
         )
         self.avgpool = nn.AdaptiveAvgPool2d((6, 6))
         self.classifier = nn.Sequential(
-            nn.Dropout(),
+            nn.Dropout(dropout_rate) if use_dropout else nn.Identity(),
             nn.Linear(256 * 6 * 6, 4096),
             nn.LeakyReLU(),
-            nn.Dropout(),
-            nn.Linear(4096, 4096),
-            nn.LeakyReLU(),
+            nn.Dropout(dropout_rate) if use_dropout else nn.Identity(),
             nn.Linear(4096, num_classes),
         )
+        self.use_dropout = use_dropout
+        self.dropout_rate = dropout_rate
 
     def forward(self, x):
         x = self.features(x)
         x = self.avgpool(x)
         x = x.view(x.size(0), 256 * 6 * 6)
         x = self.classifier(x)
         return x
 
 
-def alexnet(weights=None, cifar=False):
+def alexnet(weights=None, cifar=False, **kwargs):
     if cifar:
-        return SmallAlexNet()
+        return SmallAlexNet(**kwargs)
     return torchvision.models.get_model("alexnet", weights=weights)
```

## generalization/models/pytorch/inception.py

```diff
@@ -6,47 +6,68 @@
 
 import torch
 import torchvision
 from torch import nn
 
 
 class ConvModule(nn.Module):
-    def __init__(self, in_channels, out_channels, kernel_size, stride, padding):
+    def __init__(
+        self,
+        in_channels,
+        out_channels,
+        kernel_size,
+        stride,
+        padding,
+        use_batch_norm=False,
+        activation_layer=nn.ReLU,
+    ):
         super(ConvModule, self).__init__()
         self.conv = nn.Conv2d(in_channels, out_channels, kernel_size, stride, padding)
-        self.bn = nn.BatchNorm2d(out_channels)
-        self.act = nn.ReLU()
+        self.bn = nn.BatchNorm2d(out_channels) if use_batch_norm else nn.Identity()
+        self.act = activation_layer()
 
     def forward(self, x):
         x = self.conv(x)
         x = self.bn(x)
         x = self.act(x)
         return x
 
 
 class InceptionModule(nn.Module):
-    def __init__(self, in_channels, out_1x1, out_3x3):
+    def __init__(self, in_channels, out_1x1, out_3x3, **kwargs):
         super(InceptionModule, self).__init__()
         self.conv1 = ConvModule(
-            in_channels, out_1x1, kernel_size=1, stride=1, padding=0
+            in_channels,
+            out_1x1,
+            kernel_size=1,
+            stride=1,
+            padding=0,
+            **kwargs,
         )
         self.conv3 = ConvModule(
-            in_channels, out_3x3, kernel_size=3, stride=1, padding=1
+            in_channels,
+            out_3x3,
+            kernel_size=3,
+            stride=1,
+            padding=1,
+            **kwargs,
         )
 
     def forward(self, x):
         out_1 = self.conv1(x)
         out_2 = self.conv3(x)
         return torch.cat([out_1, out_2], 1)
 
 
 class DownsampleModule(nn.Module):
-    def __init__(self, in_channels, out_3x3):
+    def __init__(self, in_channels, out_3x3, **kwargs):
         super(DownsampleModule, self).__init__()
-        self.conv = ConvModule(in_channels, out_3x3, kernel_size=3, stride=2, padding=0)
+        self.conv = ConvModule(
+            in_channels, out_3x3, kernel_size=3, stride=2, padding=0, **kwargs
+        )
         self.maxpool = nn.MaxPool2d(kernel_size=3, stride=2)
 
     def forward(self, x):
         out_1 = self.conv(x)
         out_2 = self.maxpool(x)
         return torch.cat([out_1, out_2], 1)
 
@@ -54,59 +75,70 @@
 class InceptionSmall(nn.Module):
     """
     Inception Small as shown in the Appendix A of the paper.
 
     The implementation follows the blocks from Figure 3.
     """
 
-    def __init__(self):
+    def __init__(
+        self, num_outputs=10, use_batch_norm=False, use_dropout=False, dropout_rate=0.5
+    ):
         super(InceptionSmall, self).__init__()
+        self.num_outputs = num_outputs
+        self.use_batch_norm = use_batch_norm
+        self.use_dropout = use_dropout
+        inception_module_kwargs = {
+            "use_batch_norm": self.use_batch_norm,
+            "activation_layer": nn.LeakyReLU,
+        }
+
         self.conv1 = ConvModule(3, 96, kernel_size=3, stride=1, padding=0)
         self.inception1 = nn.Sequential(
-            InceptionModule(96, 32, 32),
-            InceptionModule(64, 32, 48),
-            DownsampleModule(80, 80),
+            InceptionModule(96, 32, 32, **inception_module_kwargs),
+            InceptionModule(64, 32, 48, **inception_module_kwargs),
+            DownsampleModule(80, 80, **inception_module_kwargs),
         )
         self.inception2 = nn.Sequential(
-            InceptionModule(160, 112, 48),
-            InceptionModule(160, 96, 64),
-            InceptionModule(160, 80, 80),
-            InceptionModule(160, 48, 96),
-            DownsampleModule(144, 96),
+            InceptionModule(160, 112, 48, **inception_module_kwargs),
+            InceptionModule(160, 96, 64, **inception_module_kwargs),
+            InceptionModule(160, 80, 80, **inception_module_kwargs),
+            InceptionModule(160, 48, 96, **inception_module_kwargs),
+            DownsampleModule(144, 96, **inception_module_kwargs),
         )
         self.inception3 = nn.Sequential(
-            InceptionModule(240, 176, 160),
-            InceptionModule(336, 176, 160),
+            InceptionModule(240, 176, 160, **inception_module_kwargs),
+            InceptionModule(336, 176, 160, **inception_module_kwargs),
         )
 
         self.mean_pool = nn.AdaptiveAvgPool2d((7, 7))
 
         self.fc = nn.Sequential(
-            nn.Dropout(),
+            nn.Dropout(dropout_rate) if self.use_dropout else nn.Identity(),
             nn.Linear(16464, 384),
-            nn.ReLU(),
+            nn.LeakyReLU(),
             nn.Linear(384, 192),
-            nn.ReLU(),
-            nn.Linear(192, 10),
+            nn.Dropout(dropout_rate) if self.use_dropout else nn.Identity(),
+            nn.LeakyReLU(),
+            nn.Linear(192, self.num_outputs),
         )
 
     def forward(self, x):
         x = self.conv1(x)
         x = self.inception1(x)
         x = self.inception2(x)
         x = self.inception3(x)
         x = self.mean_pool(x)
         x = torch.flatten(x, 1)
         x = self.fc(x)
         return x
 
 
-def inception(weights=None, cifar=False):
+def inception(weights=None, cifar=False, **kwargs):
     if cifar:
-        return InceptionSmall()
+        return InceptionSmall(**kwargs)
     return torchvision.models.get_model("inception_v3", weights=weights)
 
 
 if __name__ == "__main__":
     model = inception(cifar=True)
     model.cpu()
     x = torch.randn(1, 3, 28, 28)
```

## generalization/models/pytorch/mlp.py

```diff
@@ -1,42 +1,50 @@
 """
 Defines a multi-layer perceptron model and related functions.
 
 Author: Stepp1
 """
+
 import copy
 
 import torch.nn as nn
 
 
 class MLP(nn.Module):
-    def __init__(self, n_units):
+    def __init__(self, n_units, use_dropout=False, dropout_rate=0.5):
         super(MLP, self).__init__()
 
         self.n_units = copy.copy(n_units)
         self.layers = []
-        self.relu = nn.ReLU()
+        self.relu = nn.LeakyReLU()
 
         for i in range(1, len(n_units)):
-            layer = nn.Linear(n_units[i - 1], n_units[i], bias=False)
+            layer = nn.Linear(n_units[i - 1], n_units[i], bias=True)
 
             self.layers.append(layer)
 
             name = "fc%d" % i
             if i == len(n_units) - 1:
                 name = "fc"  # the prediction layer is just called fc
             self.add_module(name, layer)
 
+        self.dropout = nn.Dropout(dropout_rate) if use_dropout else nn.Identity()
+
     def forward(self, x):
-        x = x.view(-1, self.n_units[0])
+        x = x.view(x.size(0), -1)
         out = self.layers[0](x)
 
-        for layer in self.layers[1:]:
+        for i, layer in enumerate(self.layers[1:]):
             out = self.relu(out)
+            if i == len(self.layers) - 2:
+                out = self.dropout(out)
             out = layer(out)
 
         return out
 
 
-def mlp(in_size, hidden_sizes, out_size):
-    model = MLP([in_size] + hidden_sizes + [out_size])
+def mlp(in_size, hidden_sizes, out_size, **kwargs):
+    use_dropout = kwargs.get("use_dropout", False)
+    dropout_rate = kwargs.get("dropout_rate", 0.5)
+
+    model = MLP([in_size] + hidden_sizes + [out_size], use_dropout, dropout_rate)
     return model
```

## generalization/models/pytorch/resnet.py

```diff
@@ -1,13 +1,21 @@
 import torch
 import torchvision
 
 
-def resnet(resnet_size=18, weights=None, cifar=False):
+def resnet(resnet_size=18, weights=None, cifar=False, **kwargs):
     resnet = "resnet"
-    model = torchvision.models.get_model(resnet + str(resnet_size), weights=weights)
+
+    if "use_batch_norm" in kwargs and kwargs["use_batch_norm"]:
+        norm_layer = torch.nn.BatchNorm2d
+    else:
+        norm_layer = torch.nn.Identity
+
+    model = torchvision.models.get_model(
+        resnet + str(resnet_size), weights=weights, norm_layer=norm_layer
+    )
     if cifar:
         model.conv1 = torch.nn.Conv2d(
             3, 64, kernel_size=3, stride=1, padding=1, bias=False
         )
         model.fc = torch.nn.Linear(512, 10)
     return model
```

## generalization/randomization/__init__.py

```diff
@@ -1,16 +1,7 @@
 from .builders import build_cifar10, create_corrupted_dataset
-from .corruptions import _IMPORT_TABLE, get_randomization
+from .corruptions import RANDOMIZATIONS, get_randomization
 from .dataset import RandomizedDataset
 
 
 def available_corruptions():
-    return list(_IMPORT_TABLE.keys())
-
-
-__all__ = [
-    "available_corruptions",
-    "build_cifar10",
-    "create_corrupted_dataset",
-    "RandomizedDataset",
-    "get_randomization",
-]
+    return list(RANDOMIZATIONS.keys())
```

## generalization/randomization/builders.py

```diff
@@ -1,72 +1,117 @@
+import logging
+import os
+import random
+
 import numpy as np
 import torch
 from torchvision.datasets import CIFAR10, ImageNet
 
 from .dataset import RandomizedDataset
 from .transforms import get_cifar10_transforms
 from .utils import image_grid
 
 
 def create_corrupted_dataset(
-    dataset_name,
-    corruption_name,
+    dataset_name="cifar10",
+    dataset=None,
+    corruption_name=None,
     corruption_prob=0.0,
     train=True,
-    root="/data/cifar10",
-    apply_corruption=False,
-    return_corruption=False,
+    root="./data/cifar10",
     transform=None,
     target_transform=None,
+    save_ds=False,
+    attempt_load=True,
+    seed=0,
 ):
-    if dataset_name.lower() == "imagenet":
-        dataset = ImageNet(root=root, download=True, train=train)
-    elif dataset_name.lower() == "cifar10":
-        dataset = CIFAR10(root=root, download=True, train=train)
-    else:
-        raise ValueError("Dataset name must be either 'imagenet' or 'cifar10'")
+    if seed is not None:
+        from ..utils.data import seed_everything
+
+        seed_everything(seed)
+    train_str = "train" if train else "test"
+    if corruption_name is None:
+        corruption_name = "normal_labels"
+        corruption_prob = 0.0
+
+    possible_path = root + f"/{seed}/{corruption_name}/{corruption_prob}/{train_str}"
+
+    if attempt_load:
+        logging.info(f"Checking for dataset at {possible_path}")
+    if os.path.exists(possible_path) and attempt_load:
+        logging.info(f"Loading dataset from {possible_path}")
+        return RandomizedDataset.load_dataset(
+            root_path=root,
+            filepath=f"/{seed}/{corruption_name}/{corruption_prob}/{train_str}",
+            transform=transform,
+            target_transform=target_transform,
+        )
+
+    # either pass the dataset or the dataset name
+    # if both are passed, raise an error
+    if dataset is not None and dataset_name is not None:
+        raise ValueError("Either pass the dataset or the dataset name, not both.")
+    if dataset is None:
+        assert dataset_name is not None, "Dataset name must be provided."
+        if dataset_name.lower() == "imagenet":
+            dataset = ImageNet(root=root, download=True, train=train)
+        elif dataset_name.lower() == "cifar10":
+            dataset = CIFAR10(root=root, download=True, train=train)
+        else:
+            raise ValueError("Dataset name must be either 'imagenet' or 'cifar10'")
 
-    return RandomizedDataset(
+    dataset = RandomizedDataset(
         dataset=dataset,
         corruption_name=corruption_name,
         corruption_prob=corruption_prob,
-        apply_corruption=apply_corruption,
-        return_corruption=return_corruption,
         train=train,
         transform=transform,
         target_transform=target_transform,
+        seed=seed,
     )
+    if save_ds:
+        dataset.save_dataset(
+            root_path=root,
+        )
+    logging.info(f"Dataset saved at {possible_path}")
+    return dataset
 
 
 def build_cifar10(
     corruption_name,
     corruption_prob=0.0,
-    root="/data/cifar10",
+    root="./data/cifar10",
+    seed=0,
+    save_ds=False,
+    attempt_load=True,
     show_images=False,
     verbose=False,
 ):
     base_transforms = get_cifar10_transforms()
     train_dset = create_corrupted_dataset(
         dataset_name="cifar10",
         corruption_name=corruption_name,
         corruption_prob=corruption_prob,
         train=True,
         root=root,
-        apply_corruption=True,
-        return_corruption=False,
         transform=base_transforms,
+        seed=seed,
+        save_ds=save_ds,
+        attempt_load=attempt_load,
     )
 
     test_dset = create_corrupted_dataset(
         dataset_name="cifar10",
         train=False,
         root=root,
         corruption_name="normal_labels",
-        apply_corruption=True,
         transform=base_transforms,
+        seed=seed,
+        save_ds=False,
+        attempt_load=False,
     )
     random_idxs = np.random.choice(len(test_dset), 10)
     if verbose:
         print("Output Shape:", test_dset[random_idxs[0]][0].shape)
     if show_images:
         image_grid(train_dset, random_idxs, no_transform=True)
         image_grid(test_dset, random_idxs, no_transform=True)
```

## generalization/randomization/corruptions.py

```diff
@@ -19,21 +19,20 @@
 #   - If a dataset is provided, the class assumes that the dataset is a torch.utils.data.Dataset and uses it directly
 #   - We make use of self.classes and self.class_to_idx to manage the label permutations [A MUST!]
 #   - We make use of the self.train flag to determine if the dataset is used for training or testing
 #   - We make use of the self.corruption_name to determine the corruption function to use
 #   - We make use of the self.corruption_prob to determine the probability of corruption
 
 
-import functools
 import importlib
 from typing import Callable, List
 
 from absl import logging
 
-_IMPORT_TABLE = {
+RANDOMIZATIONS = {
     "random_labels": "generalization.randomization.labels.random_labels",
     "partial_labels": "generalization.randomization.labels.partial_labels",
     "random_pixels": "generalization.randomization.inputs.random_pixels",
     "shuffled_pixels": "generalization.randomization.inputs.shuffled_pixels",
     "gaussian_pixels": "generalization.randomization.inputs.gaussian_pixels",
 }
 
@@ -52,15 +51,17 @@
           builder_fn: Function to be called to corruption a sample. Must accept
             randomization-specific arguments and return a corrupted sample.
 
         Raises:
           KeyError: If the provided name is not unique.
         """
         if name in cls._REGISTRY:
-            raise KeyError(f"Randomization with name ({name}) already registered.")
+            raise KeyError(
+                f"Randomization with name ({name}) already registered."
+            )
         cls._REGISTRY[name] = builder_fn
 
     @classmethod
     def get(cls, name: str) -> Callable:
         """Get a Randomization from the registry by its name.
 
         Args:
@@ -70,16 +71,16 @@
           Randomization function that accepts randomization-specific parameters and
           returns a corrupted sample.
 
         Raises:
           KeyError: If the randomization is not found.
         """
         if name not in cls._REGISTRY:
-            if name in _IMPORT_TABLE:
-                module = _IMPORT_TABLE[name]
+            if name in RANDOMIZATIONS:
+                module = RANDOMIZATIONS[name]
                 importlib.import_module(module)
                 logging.info(
                     "On-demand import of randomization (%s) from module (%s).",
                     name,
                     module,
                 )
                 if name not in cls._REGISTRY:
@@ -100,15 +101,15 @@
         return list(cls._REGISTRY.keys())
 
 
 def add_randomization(name: str, *args, **kwargs):
     """Decorator for shorthand randomization registdation."""
 
     def inner(builder_fn: Callable) -> Callable:
-        RandomizationRegistry.add(name, functools.partial(builder_fn, *args, **kwargs))
+        RandomizationRegistry.add(name, builder_fn)
         return builder_fn
 
     return inner
 
 
 def get_randomization(randomization_name: str) -> Callable:
     """Maps dataset name to a dataset_builder.
```

## generalization/randomization/dataset.py

```diff
@@ -20,37 +20,41 @@
 #   - We make use of self.classes and self.class_to_idx to manage the label permutations [A MUST!]
 #   - We make use of the self.train flag to apply corruptions (training) or not (testing)
 #   - We make use of the self.corruption_name to determine the corruption function to use
 #   - We make use of the self.corruption_prob to determine the probability of corruption
 #
 # All corruption functions are defined in generalization/data/corruptions.py
 
+import json
+import os
 import warnings
 from functools import partial
 
+import numpy as np
 import torch
+from matplotlib import pyplot as plt
+from safetensors.numpy import load_file, save_file
 from torchvision import transforms
 from torchvision.datasets import VisionDataset
 from tqdm import tqdm
 
+from ..utils.data import seed_everything
 from .corruptions import *
 from .utils import get_dimensions, open_data
 
 
 class RandomizedDataset(VisionDataset):
     """Dataset that applies Randomization Attacks as shown in https://arxiv.org/abs/1611.03530.
 
     Args:
         dataset (torch.utils.data.Dataset): Dataset to be randomized
         data (torch.Tensor): Data tensor
         targets (torch.Tensor): Target tensor
         corruption_name (str): Name of the corruption to be applied
-        corruption_probtarget_idx (float): Probability of corruption
-        apply_corruption (bool): If True, the corruption is applied to the returned image
-        return_corruption (bool): If True, the corruption is returned along with the image
+        corruption_prob (float): Probability of corruption
         train (bool): If True, the dataset is used for training
         transform (callable, optional): A function/transform that takes in an PIL image and returns a transformed version. E.g, ``transforms.RandomCrop``
         target_transform (callable, optional): A function/transform that takes in the target and transforms it.
 
 
     Allowed corruption names:
         - "random_labels": all the labels are replaced with random ones
@@ -65,51 +69,59 @@
     def __init__(
         self,
         data=None,
         targets=None,
         dataset=None,
         corruption_name=None,
         corruption_prob=0.0,
-        apply_corruption=False,
-        return_corruption=False,
         train=True,
         transform=None,
         target_transform=None,
+        seed=0,
         **kwargs,
     ):
         super().__init__(
             root=None, transform=transform, target_transform=target_transform
         )
 
+        seed_everything(seed)
+        self.seed = seed
+        self.train = train
+        self.corruption_name = corruption_name
+        self.corruption_prob = corruption_prob
+
         if data is not None and targets is not None:
             self.data = data
             self.targets = targets
-            self.classes = None
-            self.class_to_idx = None
-            self.original_repr = "RandomizedDataset"
+            self.classes = kwargs.get("classes", None)
+            self.class_to_idx = kwargs.get("class_to_idx", None)
+            self.original_repr = f"RandomizedDataset(seed={seed}, corruption_name={corruption_name}, corruption_prob={corruption_prob})"
 
-        if dataset is not None and isinstance(dataset, torch.utils.data.Dataset):
+        elif dataset is not None and isinstance(dataset, torch.utils.data.Dataset):
             self.data = dataset.data
             self.targets = dataset.targets
             self.classes = dataset.classes
             self.class_to_idx = dataset.class_to_idx
-            self.original_repr = repr(dataset)
+            self.original_repr = (
+                repr(dataset)
+                + f", seed={seed}, corruption_name={corruption_name}, corruption_prob={corruption_prob})"
+            )
 
         else:
             raise ValueError(
                 "Either dataset or data+targets must be provided as arguments"
             )
 
         self.indices = list(range(len(self.data)))
-        self.train = train
-        self.corruption_name = corruption_name
-        self.corruption_prob = corruption_prob
+        self.corrupted = kwargs.get("corrupted", [])
+        if len(self.corrupted) > 0 and kwargs.get("applied_corruptions", False):
+            self.applied_corruptions = True
+        else:
+            self.applied_corruptions = False
 
-        self.kwargs = kwargs if kwargs is not None else {}
-        self.corrupted = []
         self.setup_corruption_func()
         self.apply_corruptions()
 
     def setup_corruption_func(self):
         c, w, h = get_dimensions(open_data(self.data[0]))
         permutation_size = h * w * c // c
 
@@ -117,16 +129,16 @@
 
         if self.corruption_name in ["random_labels", "partial_labels"]:
             # choose a permutation of the labels
             self.label_permutation = torch.randperm(len(self.class_to_idx))
 
             # given a permutation and the true label, return a corrupted label
             self.get_random_label = lambda true_label: self.label_permutation[
-                true_label
-            ].item()
+                true_label[None]
+            ]
 
             self.corruption_func = partial(
                 get_randomization(self.corruption_name),
                 corruption_prob=self.corruption_prob,
                 get_random_label=self.get_random_label,
             )
 
@@ -140,74 +152,225 @@
                 permutation=self.pixel_permutation,
             )
 
         elif self.corruption_name == "random_pixels":
             self.corruption_func = partial(
                 get_randomization(self.corruption_name),
                 corruption_prob=self.corruption_prob,
-                permutation_size=permutation_size,
             )
         elif self.corruption_name == "gaussian_pixels":
             self.corruption_func = partial(
                 get_randomization(self.corruption_name),
                 corruption_prob=self.corruption_prob,
+                shape=(c, w, h),
                 use_cifar=True,
             )
 
         else:
-            self.corruption_func = lambda img, target, **kwargs: (img, target, False)
+            self.corruption_func = lambda img, target, **kwargs: (
+                img,
+                target,
+                False,
+            )
 
     def apply_corruptions(self):
+        if self.applied_corruptions or len(self.corrupted) > 0:
+            logging.info("Corruptions already applied, skipping .apply_corruptions()")
+            return
+
         for index in tqdm(range(len(self.data))):
             x = transforms.functional.to_tensor(open_data(self.data[index]))
             y = torch.tensor(self.targets[index])
 
             x, y, is_corrupt = self.corruption_func(x, y)
 
             self.corrupted.append(is_corrupt)
             self.data[index] = transforms.functional.to_pil_image(x)
             self.targets[index] = y
 
+        self.corrupted = torch.as_tensor(self.corrupted)
+        self.applied_corruptions = True
+
     def __getitem__(self, index):
-        x = transforms.functional.to_tensor(open_data(self.data[index]))
+        x = transforms.functional.to_tensor(self.data[index])
         y = torch.as_tensor(self.targets[index])
 
         if self.transform is not None:
             x = self.transform(x)
 
         if self.target_transform is not None:
             y = self.target_transform(y)
 
         return (x, y, index)
 
     def __len__(self):
         return len(self.data)
 
     def __repr__(self):
-        return self.original_repr + self.extra_repr()
+        return self.original_repr
 
-    def extra_repr(self) -> str:
-        corruption = self.corruption_name
-        return f", Corruption: {corruption}"
-
-    def replace_transform(self, transform, target_transform=None):
+    def replace_transform(self, transform, target_transform=None) -> None:
         self.transform = transform
-
         if target_transform is not None:
             self.target_transform = target_transform
 
-    def corruption_checks(self):
-        is_full_random = self.corruption_name in ["random_labels", "random_pixels"]
+    def corruption_checks(self) -> None:
+        is_full_random = self.corruption_name in [
+            "random_labels",
+            "random_pixels",
+        ]
         if is_full_random:
             check_corrupt_prob = not self.corruption_prob in [0.0, 1.0]
             if check_corrupt_prob:
                 warnings.warn(
                     "corruption_prob is ignored when corruption_name is 'random_*'"
                 )
             self.corruption_prob = 1.0
         else:
             is_normal = self.corruption_name == "normal_labels"
             not_using_corruption_prob = self.corruption_prob == 0.0
             if not_using_corruption_prob and not is_normal:
                 warnings.warn(
                     "corruption_prob is not provided, using default value of 0.0"
                 )
+
+    def sample_random_grid(self, n_samples: int = 2, **kwargs) -> tuple:
+        """Make a grid of random samples from the dataset.
+
+        Args:
+            nrow (int, optional): Number of images per row. Defaults to 2.
+
+        Returns:
+            tuple: A tuple containing the grid, the labels and the corruption status
+        """
+
+        sample_idxs = torch.randint(0, len(self), (n_samples,))
+        samples = [self[idx] for idx in sample_idxs]
+        is_corrupt = [self.corrupted[idx] for idx in sample_idxs]
+
+        return (
+            [sample[0] for sample in samples],
+            [sample[1] for sample in samples],
+            is_corrupt,
+        )
+
+    def show_images(self, n_samples=5, **kwargs):
+        """Display a grid of random samples from the dataset.
+        Shows if the tensors are corrupted or not as titles.
+
+        Args:
+            nrow (int, optional): Number of images per row. Defaults to 2.
+        """
+
+        tensor_list, labels, is_corrupt = self.sample_random_grid(
+            n_samples=n_samples, **kwargs
+        )
+
+        fig, axs = plt.subplots(tight_layout=True, ncols=n_samples)
+        plt.axis("off")
+
+        grid_titles = [
+            (
+                f"{self.classes[label.item()]}\n(corrupted)"
+                if corrupt
+                else f"{self.classes[label.item()]}"
+            )
+            for label, corrupt in zip(labels, is_corrupt)
+        ]
+        dataset_label = f"Randomized Dataset with {self.corruption_name} (prob = {self.corruption_prob})"
+        plt.suptitle(dataset_label, y=0.72, fontsize=14)
+        # given grid's width, set a text on top of each image
+        # that text is the corresponding grid_titles element
+        size_oneimg = tensor_list[0].shape[-1]
+        for i, ax in enumerate(axs):
+            ax.imshow(tensor_list[i].permute(1, 2, 0))
+            ax.set_title(grid_titles[i], fontsize=12)
+            ax.axis("off")
+
+        if "save_path" in kwargs:
+            plt.savefig(kwargs["save_path"], bbox_inches="tight", dpi=300)
+        plt.show()
+
+    @staticmethod
+    def load_dataset(
+        root_path,
+        filepath,
+        transform=None,
+        target_transform=None,
+    ) -> "RandomizedDataset":
+        """Loads the Dataset from a file.
+
+        filepath must follow the following structure:
+        filepath = "seed/dataset_name/corruption_name/corruption_prob"
+        e.g. "42/cifar10/random_labels/0.2"
+        """
+        path = f"{root_path}/{filepath}"
+
+        filepath_split = filepath.split("/")
+        filepath_split.remove("")
+        seed, corruption_name, corruption_prob, train_str = filepath_split
+
+        tensors = load_file(filename=f"{path}/dataset.safetensors")
+        meta = json.load(open(f"{path}/metadata.json", "r"))
+
+        # check what we can assert from the metadata
+        assert meta["seed"] == int(seed)
+        assert meta["corruption_name"] == corruption_name
+        assert meta["corruption_prob"] == float(corruption_prob)
+        assert meta["train"] == (train_str == "train")
+
+        dataset = RandomizedDataset(
+            data=tensors["data"],
+            targets=tensors["targets"],
+            corruption_name=corruption_name,
+            corruption_prob=float(corruption_prob),
+            transform=transform,
+            target_transform=target_transform,
+            ## Loaded from metadata:
+            seed=int(seed),
+            train=bool(meta["train"]),
+            class_to_idx=meta["classes_to_idx"],
+            classes=meta["classes"],
+            corrupted=tensors["corrupted"],
+            applied_corruptions=True,
+        )
+        dataset.original_repr = meta["__repr__"]
+        return dataset
+
+    @staticmethod
+    def save(dataset, root_path, seed, corruption_name, corruption_prob, train):
+        """Saves the dataset to a file using SafeTensors."""
+        if corruption_name == None:
+            corruption_name = "normal_labels"
+            corruption_prob = 0.0
+        train_str = "train" if train else "test"
+        filepath = f"{seed}/{corruption_name}/{corruption_prob}/{train_str}"
+        fullpath = f"{root_path}/{filepath}"
+        os.makedirs(fullpath, exist_ok=True)
+        tensors = {
+            "data": np.asarray(dataset.data),
+            "targets": np.asarray(torch.as_tensor(dataset.targets)),
+            "corrupted": np.asarray(dataset.corrupted),
+        }
+        meta = {
+            "seed": seed,
+            "corruption_name": dataset.corruption_name,
+            "corruption_prob": dataset.corruption_prob,
+            "classes_to_idx": dataset.class_to_idx,
+            "classes": dataset.classes,
+            "train": dataset.train,
+            "__repr__": repr(dataset),
+        }
+        save_file(tensor_dict=tensors, filename=f"{fullpath}/dataset.safetensors")
+        json.dump(meta, open(f"{fullpath}/metadata.json", "w"))
+
+        return filepath
+
+    def save_dataset(self, root_path):
+        return RandomizedDataset.save(
+            dataset=self,
+            root_path=root_path,
+            seed=self.seed,
+            corruption_name=self.corruption_name,
+            corruption_prob=self.corruption_prob,
+            train=self.train,
+        )
```

## generalization/randomization/utils.py

```diff
@@ -22,14 +22,15 @@
 IMAGENET_CHANNEL_STD = tuple((IMAGENET_NORMALIZE_STD[c] * 255.0 for c in range(3)))
 
 
 def image_grid(dataset, idxs, no_transform=False, save_fname=None):
     if save_fname:
         # increase font size
         plt.rcParams.update({"font.size": 16})
+    assert len(idxs) == 10, "Only 10 images can be displayed at a time."
 
     fig, axs = plt.subplots(2, 5, figsize=(10, 5))
 
     if no_transform:
         dset_transform = dataset.transform
         # remove Normalize from dset_transform.transforms
         dataset.replace_transform(
@@ -60,18 +61,18 @@
     if no_transform:
         dataset.replace_transform(dset_transform)
 
     if save_fname:
         fig.savefig(f"{save_fname}-grid.png", bbox_inches="tight", dpi=300)
 
     plt.tight_layout()
-    fig.show()
+    return fig
 
 
-def image_grid_comparision(dataset, idxs, no_transform=False, save_fname=None):
+def image_grid_comparison(dataset, idxs, no_transform=False, save_fname=None):
     if save_fname:
         # increase font size
         plt.rcParams.update({"font.size": 16})
 
     fig, axs = plt.subplots(2, 5, figsize=(10, 5))
 
     if no_transform:
@@ -132,15 +133,15 @@
 
 
 def _assert_image_tensor(img: Tensor) -> None:
     if not _is_tensor_a_torch_image(img):
         raise TypeError("Tensor is not a torch image.")
 
 
-def get_dimensions(img: Tensor) -> List[int]:
+def get_dimensions(img) -> List[int]:
     """Returns the dimensions of an image as [channels, height, width].
 
     Args:
         img (PIL Image or Tensor): The image to be checked.
 
     Returns:
         List[int]: The image dimensions.
```

## generalization/randomization/inputs/gaussian_pixels.py

```diff
@@ -1,15 +1,17 @@
 import torch
-from generalization.randomization import corruptions
-from generalization.randomization import utils as dataset_utils
+
+from .. import corruptions
+from .. import utils as dataset_utils
 
 
 @corruptions.add_randomization("gaussian_pixels")
-def gaussian_pixels(img, target, corruption_prob, use_cifar=False):
-    c, w, h = img.size()
+def gaussian_pixels(img, target, corruption_prob, shape, use_cifar=False):
+    w = shape[1]
+    h = shape[2]
 
     sampled = None
     corrupted = False
     if torch.rand(1) <= corruption_prob:
         corrupted = True
         if use_cifar:
             mean = dataset_utils.CIFAR10_CHANNEL_MEAN
@@ -18,8 +20,8 @@
             mean = dataset_utils.IMAGENET_CHANNEL_MEAN
             std = dataset_utils.IMAGENET_CHANNEL_STD
         normal = torch.distributions.Normal(torch.tensor(mean), torch.tensor(std))
         sampled = normal.sample((h, w)).permute(2, 0, 1).clamp(0, 255).type(torch.uint8)
 
         img = sampled
 
-    return img, target, corrupted
+    return img, target, torch.tensor(corrupted, dtype=torch.bool)
```

## generalization/randomization/inputs/random_pixels.py

```diff
@@ -1,37 +1,30 @@
 import torch
-from generalization.randomization.corruptions import add_randomization
-from generalization.randomization.labels.shuffled_pixels import apply_pixel_permutation
+
+from ..corruptions import add_randomization
+from .shuffled_pixels import apply_pixel_permutation
 
 
 @add_randomization("random_pixels")
-def random_pixels(
-    img, target, corruption_prob, permutation_size, apply_corruption=False
-):
+def random_pixels(img, target, corruption_prob):
     """
     Applies a random permutation to the pixels of the image.
 
     Args:
         img (torch.Tensor): Image tensor
         target (torch.Tensor): Target tensor
         corruption_prob (float): Probability of corruption
-        permutation_size (int): Size of the permutation, e.g. 32x32 = 1024
         apply_corruption (bool): If True, the corruption is applied to the returned image
     """
     # permutated idx are original indices
-    permutation_pixels = torch.arange(permutation_size)
+    permutation_pixels = torch.arange(img.size(1) * img.size(2))
     c, h, w = img.size()
-
-    # check if the permutation size matches the image size
-    assert permutation_size == h * w, "Permutation size does not match image size"
-
     corrupted = False
     if torch.rand(1) <= corruption_prob:
         corrupted = True
         # choose different random permutation for each image
-        permutation_pixels = torch.randperm(permutation_size)
+        permutation_pixels = torch.randperm(h * w)
 
         # apply it to the image
-        if apply_corruption:
-            img = apply_pixel_permutation(img, permutation_pixels)
+        img = apply_pixel_permutation(img, permutation_pixels)
 
-    return img, target, corrupted
+    return img, target, torch.tensor(corrupted, dtype=torch.bool)
```

## generalization/randomization/inputs/shuffled_pixels.py

```diff
@@ -1,9 +1,10 @@
 import torch
-from generalization.randomization.corruptions import add_randomization
+
+from ..corruptions import add_randomization
 
 
 @add_randomization("shuffled_pixels")
 def shuffled_pixels(img, target, corruption_prob, permutation):
     """
     Applies the given permutation to the pixels of the image.
 
@@ -25,15 +26,15 @@
     if torch.rand(1) <= corruption_prob:
         corrupted = True
         permutation_pixels = permutation
 
         # apply it to the image
         img = apply_pixel_permutation(img, permutation_pixels)
 
-    return img, target, corrupted
+    return img, target, torch.tensor(corrupted, dtype=torch.bool)
 
 
 def apply_pixel_permutation(img, pixel_perm):
     """
     Applies the given permutation of the pixels to the image.
     """
     c, w, h = img.size()
```

## generalization/randomization/labels/partial_labels.py

```diff
@@ -1,9 +1,10 @@
 import torch
-from generalization.randomization.corruptions import add_randomization
+
+from ..corruptions import add_randomization
 
 
 @add_randomization("partial_labels")
 def partial_labels(img, target, corruption_prob, get_random_label):
     """
     Randomizes the labels of the dataset.
 
@@ -18,8 +19,8 @@
     corrupted = False
     if torch.rand(1) <= corruption_prob:
         corrupted = True
         random_label = get_random_label(target)
 
         target = random_label
 
-    return img, target, corrupted
+    return img, target, torch.tensor(corrupted, dtype=torch.bool)
```

## generalization/randomization/labels/random_labels.py

```diff
@@ -1,28 +1,21 @@
 import torch
-from generalization.randomization.corruptions import add_randomization
+
+from ..corruptions import add_randomization
 
 
 @add_randomization("random_labels")
-def random_labels(
-    img, target, corruption_prob, get_random_label, apply_corruption=False
-):
+def random_labels(img, target, corruption_prob, get_random_label):
     """
     Randomizes the labels of the dataset.
 
     Args:
         img (torch.Tensor): Image tensor
         target (torch.Tensor): Target tensor
         corruption_prob (float): Probability of corruption
+            Not used in this function, but maintained for consistency.
         get_random_label (callable): Function that returns a random label
         apply_corruption (bool): If True, the corruption is applied to the returned image
     """
-    random_label = target
-    corrupted = False
-    if torch.rand(1) <= corruption_prob:
-        corrupted = True
-        random_label = get_random_label(target)
-
-        if apply_corruption:
-            target = random_label
-
-    return img, target, corrupted
+    corrupted = True
+    random_label = get_random_label(target)
+    return img, random_label, torch.tensor(corrupted, dtype=torch.bool)
```

## generalization/utils/__init__.py

```diff
@@ -1,20 +0,0 @@
-00000000: 6672 6f6d 202e 6461 7461 2069 6d70 6f72  from .data impor
-00000010: 7420 6275 696c 645f 6578 7065 7269 6d65  t build_experime
-00000020: 6e74 0a0a 7472 793a 2020 2320 4c69 6768  nt..try:  # Ligh
-00000030: 746e 696e 6720 6973 206f 7074 696f 6e61  tning is optiona
-00000040: 6c0a 2020 2020 6672 6f6d 202e 6d6f 6465  l.    from .mode
-00000050: 6c20 696d 706f 7274 2043 6c61 7373 6966  l import Classif
-00000060: 6965 722c 204c 6974 4461 7461 4d6f 6475  ier, LitDataModu
-00000070: 6c65 2c20 4c69 744d 6f64 656c 0a65 7863  le, LitModel.exc
-00000080: 6570 7420 496d 706f 7274 4572 726f 723a  ept ImportError:
-00000090: 0a20 2020 2070 6173 730a 6672 6f6d 202e  .    pass.from .
-000000a0: 7363 6f72 6573 2069 6d70 6f72 7420 636f  scores import co
-000000b0: 6d70 7574 655f 656c 326e 5f73 636f 7265  mpute_el2n_score
-000000c0: 730a 0a5f 5f61 6c6c 5f5f 203d 205b 0a20  s..__all__ = [. 
-000000d0: 2020 2022 436c 6173 7369 6669 6572 222c     "Classifier",
-000000e0: 0a20 2020 2022 4c69 7444 6174 614d 6f64  .    "LitDataMod
-000000f0: 756c 6522 2c0a 2020 2020 224c 6974 4d6f  ule",.    "LitMo
-00000100: 6465 6c22 2c0a 2020 2020 2263 6f6d 7075  del",.    "compu
-00000110: 7465 5f65 6c32 6e5f 7363 6f72 6573 222c  te_el2n_scores",
-00000120: 0a20 2020 2022 6275 696c 645f 6578 7065  .    "build_expe
-00000130: 7269 6d65 6e74 222c 0a5d 0a              riment",.].
```

## generalization/utils/data.py

```diff
@@ -1,17 +1,24 @@
 import os
+import random
 
+import numpy as np
 import torch
-from generalization.randomization import available_corruptions, build_cifar10
 
 
 def get_num_cpus():
     return len(os.sched_getaffinity(0))
 
 
+def seed_everything(seed):
+    random.seed(seed)
+    np.random.seed(seed)
+    torch.manual_seed(seed)
+
+
 def collate_drop_return_index(batch):
     """
     Drops the return index from the batch
 
     Parameters:
     -----------
         batch (list): list of tuples (x, y, index)
@@ -19,88 +26,7 @@
     Returns:
     --------
         x, y (Tuple[torch.Tensor, torch.Tensor]): batch of data
     """
     x, y, _ = list(zip(*batch))
 
     return (torch.stack(x), torch.stack(y))
-
-
-DEFAULT_PARAMS = {
-    "seed": 88,
-    "batch_size": 256,
-    "learning_rate": 0.1,
-    "epochs": 60,
-    "val_every": 1,
-    "log_dir": "logs",
-}
-
-
-def build_experiment(
-    corrupt_prob,
-    corrupt_name=None,
-    batch_size=128,
-    drop_return_index=False,
-    *,
-    build_dl=True
-):
-    corruptions = available_corruptions()
-
-    experiments = dict()
-
-    if corrupt_name is not None:
-        corruptions = [corrupt_name]
-
-    for corrupt_name in corruptions:
-        train_set, test_set = build_cifar10(
-            corruption_name=corrupt_name,
-            corruption_prob=corrupt_prob,
-            show_images=False,
-            verbose=False,
-        )
-
-        val_set, test_set = torch.utils.data.random_split(
-            test_set, [len(test_set) // 2, len(test_set) - len(test_set) // 2]
-        )
-
-        experiments[corrupt_name] = {
-            "train_set": train_set,
-            "val_set": val_set,
-            "test_set": test_set,
-        }
-
-        if build_dl:
-            train_loader = torch.utils.data.DataLoader(
-                train_set,
-                batch_size=batch_size,
-                shuffle=True,
-                num_workers=get_num_cpus(),
-                pin_memory=True,
-                collate_fn=collate_drop_return_index if drop_return_index else None,
-            )
-
-            val_loader = torch.utils.data.DataLoader(
-                val_set,
-                batch_size=batch_size * 2,
-                shuffle=False,
-                num_workers=get_num_cpus(),
-                pin_memory=True,
-                collate_fn=collate_drop_return_index if drop_return_index else None,
-            )
-
-            test_loader = torch.utils.data.DataLoader(
-                test_set,
-                batch_size=batch_size * 2,
-                shuffle=False,
-                num_workers=get_num_cpus(),
-                pin_memory=True,
-                collate_fn=collate_drop_return_index if drop_return_index else None,
-            )
-
-            experiments[corrupt_name].update(
-                {
-                    "train_loader": train_loader,
-                    "val_loader": val_loader,
-                    "test_loader": test_loader,
-                }
-            )
-    return experiments
```

## generalization/utils/model.py

```diff
@@ -1,38 +1,36 @@
 from pathlib import Path
 
-import lightning as L
 import numpy as np
 import pandas as pd
+import pytorch_lightning as pl
 import torch
 import torchmetrics
 import wandb
-from generalization.utils.data import build_experiment, get_num_cpus
+from generalization.utils.data import get_num_cpus
+from generalization.utils.experiment import build_experiment
 from torch import nn
 from torch.nn import functional as F
 
 
-class Classifier(L.LightningModule):
+class Classifier(pl.LightningModule):
     def __init__(self, net: nn.Module, hparams: dict):
         super().__init__()
         self.net = net
         self.hparams.update(hparams)
         self.save_hyperparameters(ignore=["net"])
         self.lr = self.hparams["learning_rate"]
         self.n_classes = self.hparams["n_classes"]
 
         self.train_acc = torchmetrics.Accuracy(
             task="multiclass", num_classes=self.n_classes, average=None
         )
         self.valid_acc = torchmetrics.Accuracy(
             task="multiclass", num_classes=self.n_classes, average=None
         )
-        self.valid_f1 = torchmetrics.F1Score(
-            task="multiclass", num_classes=self.n_classes, average=None
-        )
 
         self.test_acc = torchmetrics.Accuracy(
             task="multiclass", num_classes=self.n_classes, average=None
         )
 
     def forward(self, x):
         out = self.net(x)
@@ -64,18 +62,14 @@
     def validation_step(self, batch, batch_idx):
         loss, logits, y = self.step(batch, batch_idx, reduction="mean")
 
         preds = logits.argmax(dim=1)
         self.valid_acc.update(preds, y)
         acc = self.valid_acc.compute()
 
-        self.valid_f1.update(preds, y)
-        f1 = self.valid_f1.compute()
-        print(f"acc: {acc}, f1: {f1}")
-
         self.log("valid/loss", loss, prog_bar=True, logger=True)
         self.log("valid/acc", acc.mean(), prog_bar=True, logger=True)
 
     def test_step(self, batch, batch_idx):
         loss, logits, y = self.step(batch, batch_idx, reduction="mean")
         preds = logits.argmax(dim=1)
         self.test_acc.update(preds, y)
@@ -237,15 +231,15 @@
     ):
         sample_state["epoch"] = self.current_epoch * np.ones(
             len(sample_state["batch_index"])
         )
         sample_state["stage"] = [stage] * len(sample_state["batch_index"])
 
         sample_state["corrupted"] = [
-            dataset.corrupted[i] for i in sample_state["batch_index"]
+            bool(dataset.corrupted[i]) for i in sample_state["batch_index"]
         ]
 
         sample_state["label"] = list(map(int, sample_state["batch_label"]))
 
         epoch_df = pd.DataFrame.from_dict(sample_state)
         # remove "batch_" prefix if present
         epoch_df.columns = epoch_df.columns.str.replace("batch_", "sample_")
@@ -308,30 +302,23 @@
             f"valid/loss",
             loss_per_sample.mean(),
             prog_bar=True,
             logger=True,
         )
         self.valid_acc.update(logits, y)
         self.valid_top5_acc.update(logits, y)
-        self.valid_f1.update(logits, y)
         self.log(
             "valid/acc",
             self.valid_acc.compute().mean(),
             prog_bar=True,
         )
         self.log(
             "valid/top5_acc",
             self.valid_top5_acc.compute(),
         )
-        self.log(
-            "valid/f1",
-            self.valid_f1.compute().mean(),
-            prog_bar=True,
-            logger=True,
-        )
 
         self.valid_sample_state = self.step_metrics(
             self.valid_sample_state,
             indices=batch[2],
             losses=loss_per_sample,
             y=y,
             y_pred=logits.argmax(dim=1),
@@ -356,15 +343,15 @@
         self.log(
             "test/top5_acc",
             self.test_top5_acc.compute(),
         )
         return loss_per_batch
 
 
-class LitDataModule(L.LightningDataModule):
+class LitDataModule(pl.LightningDataModule):
     def __init__(self, hparams, corrupt_prob=0.0):
         super().__init__()
         self.hparams.update(hparams)
         self.corrupt_prob = corrupt_prob
 
     def setup(self, stage=None):
         experiment_data = build_experiment(
```

## generalization/utils/train.py

```diff
@@ -1,20 +1,19 @@
 import time
 from pathlib import Path
 
-import lightning as L
 import ml_collections
-import numpy as np
+import pytorch_lightning as pl
 import torch
 import wandb
 import yaml
 from generalization.models import get_cifar_models
 from generalization.randomization import available_corruptions
-from lightning.pytorch.loggers import CSVLogger, WandbLogger
 from model import LitDataModule, LitModel
+from pytorch_lightning.loggers import CSVLogger, WandbLogger
 
 DEFAULT_PARAMS = {
     "seed": 88,
     "batch_size": 256,
     "learning_rate": 0.1,
     "epochs": 30,
     "val_every": 1,
@@ -55,15 +54,15 @@
                 [hparams.model_name, hparams.corrupt_name, corrupt_prob],
             )
         ),
     )
 
     logger_csv = CSVLogger(save_dir=f"{log_dir}/{project_name}", name=experiment_name)
 
-    trainer = L.Trainer(
+    trainer = pl.Trainer(
         max_epochs=hparams.epochs,
         logger=[logger, logger_csv],
         default_root_dir=log_dir,
         check_val_every_n_epoch=hparams.val_every,
     )
     pl_model = LitModel(model, hparams=hparams)
 
@@ -115,22 +114,40 @@
             print(f"Corruption prob: {corrupt_prob}")
             dm = LitDataModule(hparams=hparams, corrupt_prob=corrupt_prob)
             if dataset_size == -1:
                 dm.setup()
                 dataset_size = len(dm.train_dataloader().dataset)
 
             if hparams.model_name != "all" and isinstance(hparams.model_name, str):
-                models = get_cifar_models(model_name=hparams.model_name, lib="torch")
+                get_cifar_models(in_size=32 * 32 * 3)
+                models = get_cifar_models(
+                    model_name=hparams.model_name,
+                    use_batch_norm=True,
+                    use_dropout=True,
+                    lib="torch",
+                    in_size=32 * 32 * 3,
+                )
             elif hparams.model_name != "all" and isinstance(hparams.model_name, list):
                 models = {
-                    model_name: get_cifar_models(model_name=model_name, lib="torch")
+                    model_name: get_cifar_models(
+                        model_name=model_name,
+                        use_batch_norm=True,
+                        use_dropout=True,
+                        lib="torch",
+                        in_size=32 * 32 * 3,
+                    )
                     for model_name in hparams.model_name
                 }
             else:
-                models = get_cifar_models(lib="torch")
+                models = get_cifar_models(
+                    lib="torch",
+                    use_batch_norm=True,
+                    use_dropout=True,
+                    in_size=32 * 32 * 3,
+                )
 
             for model_name, model in models.items():
                 print(f"Model: {model_name}")
 
                 MODEL_NAME = model_name
                 CORRUPT_NAME = corrupt_name
                 CORRUPT_PROB = corrupt_prob
@@ -184,15 +201,15 @@
     SEED = args.seed
     BATCH_SIZE = args.batch_size
     LEARNING_RATE = args.lr
     EPOCHS = args.epochs
     VAL_EVERY = args.val_every
 
     torch.set_float32_matmul_precision("medium")
-    L.seed_everything(SEED)
+    pl.seed_everything(SEED)
 
     hparams = ml_collections.ConfigDict()
     hparams.update(
         {
             "seed": SEED,
             "batch_size": BATCH_SIZE,
             "learning_rate": LEARNING_RATE,
@@ -209,16 +226,16 @@
     )
     hparams.update({"subset": args.subset, "offline": False, "debug": args.debug})
 
     if args.test:
         hparams.update(
             {
                 "epochs": 5,
-                "corrupt_prob": [0.5]
-                if args.corrupt_name != "normal_labels"
-                else [0.0],
+                "corrupt_prob": (
+                    [0.5] if args.corrupt_name != "normal_labels" else [0.0]
+                ),
                 "debug": True,
                 "offline": True,
             }
         )
 
     main(hparams)
```

## Comparing `ids_generalization-20240414.dist-info/LICENSE` & `ids_generalization-20240416.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ids_generalization-20240414.dist-info/METADATA` & `ids_generalization-20240416.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 Metadata-Version: 2.1
 Name: ids-generalization
-Version: 20240414
+Version: 20240416
 Summary: Experiment Suite for Understanding and Rethinking Generalization
 Home-page: https://github.com/ids-uchile/Generalization
 Author: Stepp1
 License: BSD-3-Clause
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: torch
 Requires-Dist: numpy
-Requires-Dist: torchvision
 Requires-Dist: matplotlib
 Provides-Extra: dev
 Requires-Dist: pytest ; extra == 'dev'
 Requires-Dist: black ; extra == 'dev'
 Requires-Dist: flake8 ; extra == 'dev'
 Requires-Dist: isort ; extra == 'dev'
 
 # Understanding Deep Learning Requires Rethinking Generalization
 
 >Reproducing results from the 2017 paper [1611.03530](https://arxiv.org/abs/1611.03530)
 
-## This Repo contributes:
-- A modular approach to using datasets with randomization tests.
-- Implements all models described in the paper, both in Flax and Pytorch.
-- Reproduces original experiments. See this [report](https://wandb.ai/stepp1/generalization-2/reports/Understanding-Rethinking-Generalization-CIFAR10--Vmlldzo0NTA3Njcz).
+![CIFAR10 Corruptions](./figures/cifar10_corruptions.png)
 
+![Results](./figures/cifar10-resnet18-loss-all_corruptions-epoch.png)
 
-## Contributions
+## Paper Contributions
 
 * **Randomization tests**: *Deep neural networks easily fit random labels.*
 >  At the heart of our methodology is a variant of the well-known randomization test from non-parametric statistics (Edgington & Onghena, 2007). In a first set of experiments, we train several standard architectures on a copy of the data where the true labels were replaced by random labels.
 
 * **The role of explicit regularization**: *Explicit regularization may improve generalization performance, but is neither necessary nor by itself sufficient for controlling generalization error.*
 > If the model architecture itself isn’t a sufficient regularizer, it remains to see how much explicit regularization helps. We show that explicit forms of regularization, such as weight decay, dropout, and data augmentation, do not adequately explain the generalization error of neural networks.
 
@@ -53,31 +49,25 @@
 | **Shuffled Pixels**            | A random permutation of the pixels is chosen and then the same permutation is applied to all the images in both training and test set |
 | **Random Pixels**              | A different random permutation is applied to each image independently |
 | **Gaussian**                   | A Gaussian distribution (with matching mean and variance to the original image dataset) is used to generate random pixels for each image |
 
 
 ## Installation
 
+First, install [torch](https://pytorch.org/get-started/locally/) and [torchvision](https://pytorch.org/get-started/locally/). Then, install the package using pip:
+
+
 ### From PyPI
 
 To install the latest release from PyPI:
 
 ```bash
 pip install -U ids-generalization
 ```
 
-Note that this package requires Jax to be installed separately. See [jax](https://github.com/google/jax/blob/main/README.md) repository for instructions.
-
 ### Latest version from GitHub
 
 To pull and install the latest commit from this repository, along with its Python dependencies:
 
 ```bash
 pip install git+https://github.com/ids-uchile/Rethinking-Generalization.git
 ```
-
-## Jax and Pytorch
-If you want to try both Jax and Pytorch's versions install first [jax](https://github.com/google/jax), [Equinox](https://github.com/patrick-kidger/equinox) and then for Pytorch:
-
-```bash
-mamba install fastai -c fastai
-```
```

## Comparing `ids_generalization-20240414.dist-info/RECORD` & `ids_generalization-20240416.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,34 @@
-generalization/__init__.py,sha256=eZlouJXf42SBdbYZVyBHQo-Iz2FsusSFulrFPFW0xbA,804
-generalization/version.py,sha256=ykNb7HYl1lUiEvEPAInqjSP5tz5XhkfewdKwWGQMHlo,25
+generalization/__init__.py,sha256=EQB9quQ2L4wMruUR7QM3W6nZy5rotV8le2cjI1iVWBE,503
+generalization/version.py,sha256=AD2md3w-WhUtTCZReTHEW0UVtkBAWMGWrNrWTo5G0Wk,25
 generalization/models/__init__.py,sha256=cAiFqC9Qf5MzsrczB3s4cIgjm0s3OrmahtH2QQvJ5AI,272
-generalization/models/factory.py,sha256=D2W1tc0lETY9ebZ67PxtM6SojIOzlEWvZjB0eliwBJY,3817
-generalization/models/jax/__init__.py,sha256=yZdjSb0-uVCedBJOf0sE4Vt0V4myeGczyjaotAI88ok,253
-generalization/models/jax/alexnet.py,sha256=HzwBojhc9xmJQiQR58ikqDSfLmssHcl2y1xy32IrQrI,3792
-generalization/models/jax/inception.py,sha256=Rva3DN2S-ctKs_wTZG7Eyi2R8c5GQeWX4w4AsiQtzPk,10649
+generalization/models/factory.py,sha256=QCsw9yiol44XB-3rsggc6RFJEyVB4wPlgv3peRPoe_A,4337
 generalization/models/pytorch/__init__.py,sha256=R7KKrONFaaBgKPbPHLroVk6tD2Nq6hTcFft-rM6R9iw,325
-generalization/models/pytorch/alexnet.py,sha256=MKHYjsQ8jfkXQjxuQP4r0qb72IPuPy1n6Mmu8aRpVTE,1458
-generalization/models/pytorch/inception.py,sha256=fy1VhYhX7iDWNNjbKYaBPqR9vmanXr23kOV12iWb464,3218
-generalization/models/pytorch/mlp.py,sha256=yq311wN_vlNDiEQjHy5Pgdy-gbeOdmQzz0duIhtyCbk,979
-generalization/models/pytorch/resnet.py,sha256=62XKguMAWJZgaeh6pZF533UIaA-H_AC1UFu3mJBqF28,386
-generalization/randomization/__init__.py,sha256=9eNM5HuICiTI9_tFyoDui-5zmT7vf3zQQvsm6ay1M58,376
-generalization/randomization/builders.py,sha256=GaOqIrF5hFdzkTY8kKDDOQCpgTrdLZJO4W8OYSbzAgs,2110
-generalization/randomization/corruptions.py,sha256=fdJdmjrwm75QF9KOFiyIMVQT8gVKYftqpqLaIo6Qfbs,4945
-generalization/randomization/dataset.py,sha256=rP59pZSW0MeOzEjXApukdK6XrMGSvZM0S3wGGLfUB6Y,8863
+generalization/models/pytorch/alexnet.py,sha256=L6f5kNU4MljYd-5JtntSoDWkuqmja5msyvdVWHoZXEU,2040
+generalization/models/pytorch/inception.py,sha256=SJ0Csltee7TRVXfJPoAfblczogi8_kzMQ_mECqJPyZA,4373
+generalization/models/pytorch/mlp.py,sha256=6KNAsZnzhUYVex4NC2p7KorzLaHNbHsR6_gz2u61H-g,1334
+generalization/models/pytorch/resnet.py,sha256=_27c_grgKDUB3N7RbBhEzf8SyzZ5NiMbyWpcuk8sZlk,590
+generalization/randomization/__init__.py,sha256=YAgAYb67Suxb436hzKz8VELZsfrfhoJNPB14HMHqDW0,230
+generalization/randomization/builders.py,sha256=WD23odaukrF0li8K8NCqeF3xMX9uhpfXT29CBt_dl0w,3526
+generalization/randomization/corruptions.py,sha256=VrTC3nXzEgbqq83OScAmfHNgui90AwZuncoPX_9JXd0,4925
+generalization/randomization/dataset.py,sha256=AARIP30rLl2sP0FEMidaMAcjJsaIXf3Hc0COT1AlhUs,14672
 generalization/randomization/transforms.py,sha256=fawqoy-8wvWO4NG7I_jdCSEIjW1a2EjsH4o5QsQUYiE,752
-generalization/randomization/utils.py,sha256=w7R16fexca_cQDqR--mHW8_Dwnhxoissxfw6UlN2mJs,5105
+generalization/randomization/utils.py,sha256=GxAmrgMTXaDagtbTtarHut8EpRoLOuHxZtrLesdrr0g,5169
 generalization/randomization/inputs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-generalization/randomization/inputs/gaussian_pixels.py,sha256=Zg9xhDC05we3QyxeS8mz5YDKIjPrfPYUYPtZ2Mj0f7c,863
-generalization/randomization/inputs/random_labels.py,sha256=cPn902gKq7hPF39bHhAtAeoez6abOrCzlmYBDIi2Tzw,814
-generalization/randomization/inputs/random_pixels.py,sha256=qVDLcObZ_Rs-Yyp_4sNECBo74FMZZgjQdFsTss0M4QM,1347
-generalization/randomization/inputs/shuffled_pixels.py,sha256=aTqka6_a16ty3TEzze0oGcpG_vchFXYYjnTUb1-UxKQ,1817
+generalization/randomization/inputs/gaussian_pixels.py,sha256=2iC4gr9xQI0BXWEIcoHQFgFMDW_qTobbaZxhjhRmVtY,860
+generalization/randomization/inputs/random_pixels.py,sha256=qXeuK4IuVTxzKElOSfZXTaY-f_gV5yZ35dmBV8bx3hY,1016
+generalization/randomization/inputs/shuffled_pixels.py,sha256=0P30LdKg6PyoBDWI-ny5x4BJ8P0BORR2TrkYR9v367A,1823
 generalization/randomization/labels/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-generalization/randomization/labels/gaussian_pixels.py,sha256=y-ITjoIYFFUQfW_b-EsGzCo039NuyFSaU_orTcQTxnk,878
-generalization/randomization/labels/partial_labels.py,sha256=aXZYJ4LUOIREBIj5upjNri1wgsZhiJg3HfM7C7Hk29w,797
-generalization/randomization/labels/random_labels.py,sha256=Ozk8znGyMM4ieL8vE9aTn9kyanov_jTA8WOpRqVRPlk,858
-generalization/randomization/labels/random_pixels.py,sha256=y7PUQG6wfXmyjK4n30c3M7Aci2_Fje14_5h7mMoi4eg,1309
-generalization/randomization/labels/shuffled_pixels.py,sha256=d18ziTHg6CZLhQDul5mZFQW-jPJ48D_MM5mTOm_8bQg,1897
-generalization/utils/__init__.py,sha256=mKLRyU_BfBNMbTlGeSaPHihidaQ7XBNgzYU3vH0-MFY,315
-generalization/utils/data.py,sha256=heNhThWrQXJ5e8zP6nZEbBUEOcVBTCelQFk7_rYteXM,2755
-generalization/utils/model.py,sha256=7oUu9Tl8NbVhxYtxloKo91Dt_5VNVxshxJ18XcGX0Zs,13516
+generalization/randomization/labels/partial_labels.py,sha256=sxf_YxTSQNFo5ZdhPoyORHDrmYqfa_qQXvLzbKUussA,803
+generalization/randomization/labels/random_labels.py,sha256=MaGVPZNCh0cS627cxH1JzrPL6gc1Iv-Ue9s4uFPKgvM,749
+generalization/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+generalization/utils/data.py,sha256=mbbuBqnazsi3H5U06Q8KpMMQgDrf0IubCk8k_ei3mr4,573
+generalization/utils/experiment.py,sha256=2yVWo5GfK29zBJWuvhIQiT_A2feX_BRdAshOsWR2Pvo,2557
+generalization/utils/model.py,sha256=1t3sSF2FYCH8w6iV4RkHHC5dPsTmQmglaqx5kbCw1mo,13144
 generalization/utils/scores.py,sha256=RNgshXcPUuQiO7ZA3XpI-gp2eHul9NXet2dDGZqGhyY,574
-generalization/utils/train.py,sha256=WsEeg0xVqFj0u5H7hxMl2ZbdaZgwHmnQWNMmdlYf9YQ,7366
+generalization/utils/train.py,sha256=oPZyv7dzLvhm29paKP4pDHnT7Mn4rC2r7ghEZw7jeHY,7961
 generalization/utils/viz.py,sha256=fWB22e_VtnNEgawW3Spd08FGvXsLJSx8l9pVBNleMGM,5290
-ids_generalization-20240414.dist-info/LICENSE,sha256=xb9NWUGXyxJIHxTxpfclBBNvvkIfLnEL5fUz6FNQlL4,1497
-ids_generalization-20240414.dist-info/METADATA,sha256=1-thTLnT5rnX4-vNJ-ZFOcBNLqfujs8CZbx0tgCXrjI,5215
-ids_generalization-20240414.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-ids_generalization-20240414.dist-info/top_level.txt,sha256=wpJoKxMfLmN-9bYXLqYFFx1opWFNqtgA4lqwoN-RE98,15
-ids_generalization-20240414.dist-info/RECORD,,
+ids_generalization-20240416.dist-info/LICENSE,sha256=xb9NWUGXyxJIHxTxpfclBBNvvkIfLnEL5fUz6FNQlL4,1497
+ids_generalization-20240416.dist-info/METADATA,sha256=NvhYSneX52FxhPAUSVwfu4OGBrpS5qDVuWjoVQsBPLE,4734
+ids_generalization-20240416.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ids_generalization-20240416.dist-info/top_level.txt,sha256=wpJoKxMfLmN-9bYXLqYFFx1opWFNqtgA4lqwoN-RE98,15
+ids_generalization-20240416.dist-info/RECORD,,
```

