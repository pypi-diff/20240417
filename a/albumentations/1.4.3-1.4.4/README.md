# Comparing `tmp/albumentations-1.4.3.tar.gz` & `tmp/albumentations-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "albumentations-1.4.3.tar", last modified: Wed Apr  3 01:50:59 2024, max compression
+gzip compressed data, was "albumentations-1.4.4.tar", last modified: Wed Apr 17 02:43:53 2024, max compression
```

## Comparing `albumentations-1.4.3.tar` & `albumentations-1.4.4.tar`

### file list

```diff
@@ -1,76 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:50:59.672591 albumentations-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-03 01:50:48.000000 albumentations-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-03 01:50:48.000000 albumentations-1.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    37024 2024-04-03 01:50:59.672591 albumentations-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    35267 2024-04-03 01:50:48.000000 albumentations-1.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:50:59.660591 albumentations-1.4.3/albumentations/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:50:59.664591 albumentations-1.4.3/albumentations/augmentations/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:50:59.664591 albumentations-1.4.3/albumentations/augmentations/blur/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/blur/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/blur/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    20466 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/blur/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:50:59.664591 albumentations-1.4.3/albumentations/augmentations/crops/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/crops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10110 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/crops/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    44695 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/crops/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    14384 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/domain_adaptation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/domain_adaptation_functional.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:50:59.664591 albumentations-1.4.3/albumentations/augmentations/dropout/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/dropout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/dropout/channel_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/dropout/coarse_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/dropout/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     8644 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/dropout/grid_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/dropout/mask_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     8596 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/dropout/xy_masking.py
--rw-r--r--   0 runner    (1001) docker     (127)    45479 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:50:59.664591 albumentations-1.4.3/albumentations/augmentations/geometric/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/geometric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39909 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/geometric/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     8251 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/geometric/resize.py
--rw-r--r--   0 runner    (1001) docker     (127)    13823 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/geometric/rotate.py
--rw-r--r--   0 runner    (1001) docker     (127)    68133 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/geometric/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:50:59.664591 albumentations-1.4.3/albumentations/augmentations/mixing/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/mixing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/mixing/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    10427 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/mixing/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)   108319 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/augmentations/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:50:59.668591 albumentations-1.4.3/albumentations/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20398 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/core/bbox_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21759 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/core/composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/core/keypoints_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12736 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/core/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)    14314 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/core/transforms_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/core/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:50:59.668591 albumentations-1.4.3/albumentations/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/pytorch/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-04-03 01:50:48.000000 albumentations-1.4.3/albumentations/random_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:50:59.672591 albumentations-1.4.3/albumentations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    37024 2024-04-03 01:50:59.000000 albumentations-1.4.3/albumentations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-03 01:50:59.000000 albumentations-1.4.3/albumentations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 01:50:59.000000 albumentations-1.4.3/albumentations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-03 01:50:59.000000 albumentations-1.4.3/albumentations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-03 01:50:59.000000 albumentations-1.4.3/albumentations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-03 01:50:48.000000 albumentations-1.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 01:50:59.672591 albumentations-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-03 01:50:48.000000 albumentations-1.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:50:59.672591 albumentations-1.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    39987 2024-04-03 01:50:48.000000 albumentations-1.4.3/tests/test_augmentations.py
--rw-r--r--   0 runner    (1001) docker     (127)    11658 2024-04-03 01:50:48.000000 albumentations-1.4.3/tests/test_bbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-04-03 01:50:48.000000 albumentations-1.4.3/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    46127 2024-04-03 01:50:48.000000 albumentations-1.4.3/tests/test_functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-03 01:50:48.000000 albumentations-1.4.3/tests/test_functional_cutout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-03 01:50:48.000000 albumentations-1.4.3/tests/test_functional_mixing.py
--rw-r--r--   0 runner    (1001) docker     (127)    12548 2024-04-03 01:50:48.000000 albumentations-1.4.3/tests/test_keypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-04-03 01:50:48.000000 albumentations-1.4.3/tests/test_mixing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-04-03 01:50:48.000000 albumentations-1.4.3/tests/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-03 01:50:48.000000 albumentations-1.4.3/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)    36764 2024-04-03 01:50:48.000000 albumentations-1.4.3/tests/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8112 2024-04-03 01:50:48.000000 albumentations-1.4.3/tests/test_targets.py
--rw-r--r--   0 runner    (1001) docker     (127)    53341 2024-04-03 01:50:48.000000 albumentations-1.4.3/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:43:53.151548 albumentations-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-17 02:43:43.000000 albumentations-1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-17 02:43:43.000000 albumentations-1.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    37431 2024-04-17 02:43:53.151548 albumentations-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    35643 2024-04-17 02:43:43.000000 albumentations-1.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:43:53.139548 albumentations-1.4.4/albumentations/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:43:53.143548 albumentations-1.4.4/albumentations/augmentations/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:43:53.143548 albumentations-1.4.4/albumentations/augmentations/blur/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/blur/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/blur/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23021 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/blur/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:43:53.143548 albumentations-1.4.4/albumentations/augmentations/crops/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/crops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10272 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/crops/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51295 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/crops/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15132 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/domain_adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/domain_adaptation_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:43:53.143548 albumentations-1.4.4/albumentations/augmentations/dropout/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/dropout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/dropout/channel_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/dropout/coarse_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/dropout/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/dropout/grid_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/dropout/mask_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8688 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/dropout/xy_masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51483 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:43:53.147548 albumentations-1.4.4/albumentations/augmentations/geometric/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/geometric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43928 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/geometric/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10298 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/geometric/resize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14771 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/geometric/rotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79800 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/geometric/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:43:53.147548 albumentations-1.4.4/albumentations/augmentations/mixing/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/mixing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/mixing/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10877 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/mixing/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)   125104 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/augmentations/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:43:53.147548 albumentations-1.4.4/albumentations/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20469 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/core/bbox_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22377 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/core/composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9107 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/core/keypoints_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/core/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12747 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/core/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13427 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/core/transforms_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/core/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:43:53.147548 albumentations-1.4.4/albumentations/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/pytorch/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-17 02:43:43.000000 albumentations-1.4.4/albumentations/random_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:43:53.151548 albumentations-1.4.4/albumentations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    37431 2024-04-17 02:43:53.000000 albumentations-1.4.4/albumentations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-17 02:43:53.000000 albumentations-1.4.4/albumentations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 02:43:53.000000 albumentations-1.4.4/albumentations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-17 02:43:53.000000 albumentations-1.4.4/albumentations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 02:43:53.000000 albumentations-1.4.4/albumentations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-17 02:43:43.000000 albumentations-1.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 02:43:53.151548 albumentations-1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-17 02:43:43.000000 albumentations-1.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:43:53.151548 albumentations-1.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    39987 2024-04-17 02:43:43.000000 albumentations-1.4.4/tests/test_augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11647 2024-04-17 02:43:43.000000 albumentations-1.4.4/tests/test_bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18039 2024-04-17 02:43:43.000000 albumentations-1.4.4/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52080 2024-04-17 02:43:43.000000 albumentations-1.4.4/tests/test_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-17 02:43:43.000000 albumentations-1.4.4/tests/test_functional_cutout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-17 02:43:43.000000 albumentations-1.4.4/tests/test_functional_mixing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12432 2024-04-17 02:43:43.000000 albumentations-1.4.4/tests/test_keypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-04-17 02:43:43.000000 albumentations-1.4.4/tests/test_mixing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-04-17 02:43:43.000000 albumentations-1.4.4/tests/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7484 2024-04-17 02:43:43.000000 albumentations-1.4.4/tests/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-17 02:43:43.000000 albumentations-1.4.4/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37460 2024-04-17 02:43:43.000000 albumentations-1.4.4/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-04-17 02:43:43.000000 albumentations-1.4.4/tests/test_targets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52422 2024-04-17 02:43:43.000000 albumentations-1.4.4/tests/test_transforms.py
```

### Comparing `albumentations-1.4.3/LICENSE` & `albumentations-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.3/PKG-INFO` & `albumentations-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: albumentations
-Version: 1.4.3
+Version: 1.4.4
 Summary: An efficient library for image augmentation, providing extensive transformations to support machine learning and computer vision tasks.
 Home-page: https://albumentations.ai
 Author: Vladimir I. Iglovikov, Mikhail Druzhinin, Alex Parinov, Alexander Buslaev, Eugene Khvedchenya
 License: MIT
 Keywords: image augmentation,data augmentation,computer vision,deep learning,machine learning,image processing,artificial intelligence,augmentation library,image transformation,vision augmentation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -28,22 +28,24 @@
 License-File: LICENSE
 Requires-Dist: numpy>=1.24.4
 Requires-Dist: scipy>=1.10.0
 Requires-Dist: scikit-image>=0.21.0
 Requires-Dist: PyYAML
 Requires-Dist: typing-extensions>=4.9.0
 Requires-Dist: scikit-learn>=1.3.2
+Requires-Dist: pydantic>=2.6.4
 Requires-Dist: opencv-python-headless>=4.9.0
 
 # Albumentations
 
 [![PyPI version](https://badge.fury.io/py/albumentations.svg)](https://badge.fury.io/py/albumentations)
 ![CI](https://github.com/albumentations-team/albumentations/workflows/CI/badge.svg)
 [![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![Pydantic v2](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/main/docs/badge/v2.json)](https://pydantic.dev)
 
 [Docs](https://albumentations.ai/docs/) | [Discord](https://discord.gg/AKPrrDYNAt) | [Twitter](https://twitter.com/albumentations) | [LinkedIn](https://www.linkedin.com/company/100504475/)
 
 Albumentations is a Python library for image augmentation. Image augmentation is used in deep learning and computer vision tasks to increase the quality of trained models. The purpose of image augmentation is to create new training samples from the existing data.
 
 Here is an example of how you can apply some [pixel-level](#pixel-level-transforms) augmentations from Albumentations to create new images from the original one:
 ![parrot](https://habrastorage.org/webt/bd/ne/rv/bdnerv5ctkudmsaznhw4crsdfiw.jpeg)
@@ -249,14 +251,15 @@
 | [Affine](https://albumentations.ai/docs/api_reference/augmentations/geometric/transforms/#albumentations.augmentations.geometric.transforms.Affine)                             | ✓     | ✓    | ✓      | ✓         |
 | [BBoxSafeRandomCrop](https://albumentations.ai/docs/api_reference/augmentations/crops/transforms/#albumentations.augmentations.crops.transforms.BBoxSafeRandomCrop)             | ✓     | ✓    | ✓      |           |
 | [CenterCrop](https://albumentations.ai/docs/api_reference/augmentations/crops/transforms/#albumentations.augmentations.crops.transforms.CenterCrop)                             | ✓     | ✓    | ✓      | ✓         |
 | [CoarseDropout](https://albumentations.ai/docs/api_reference/augmentations/dropout/coarse_dropout/#albumentations.augmentations.dropout.coarse_dropout.CoarseDropout)           | ✓     | ✓    |        | ✓         |
 | [Crop](https://albumentations.ai/docs/api_reference/augmentations/crops/transforms/#albumentations.augmentations.crops.transforms.Crop)                                         | ✓     | ✓    | ✓      | ✓         |
 | [CropAndPad](https://albumentations.ai/docs/api_reference/augmentations/crops/transforms/#albumentations.augmentations.crops.transforms.CropAndPad)                             | ✓     | ✓    | ✓      | ✓         |
 | [CropNonEmptyMaskIfExists](https://albumentations.ai/docs/api_reference/augmentations/crops/transforms/#albumentations.augmentations.crops.transforms.CropNonEmptyMaskIfExists) | ✓     | ✓    | ✓      | ✓         |
+| [D4](https://albumentations.ai/docs/api_reference/augmentations/geometric/transforms/#albumentations.augmentations.geometric.transforms.D4)                                     | ✓     | ✓    | ✓      | ✓         |
 | [ElasticTransform](https://albumentations.ai/docs/api_reference/augmentations/geometric/transforms/#albumentations.augmentations.geometric.transforms.ElasticTransform)         | ✓     | ✓    | ✓      |           |
 | [Flip](https://albumentations.ai/docs/api_reference/augmentations/geometric/transforms/#albumentations.augmentations.geometric.transforms.Flip)                                 | ✓     | ✓    | ✓      | ✓         |
 | [GridDistortion](https://albumentations.ai/docs/api_reference/augmentations/geometric/transforms/#albumentations.augmentations.geometric.transforms.GridDistortion)             | ✓     | ✓    | ✓      |           |
 | [GridDropout](https://albumentations.ai/docs/api_reference/augmentations/dropout/grid_dropout/#albumentations.augmentations.dropout.grid_dropout.GridDropout)                   | ✓     | ✓    |        |           |
 | [HorizontalFlip](https://albumentations.ai/docs/api_reference/augmentations/geometric/transforms/#albumentations.augmentations.geometric.transforms.HorizontalFlip)             | ✓     | ✓    | ✓      | ✓         |
 | [Lambda](https://albumentations.ai/docs/api_reference/augmentations/transforms/#albumentations.augmentations.transforms.Lambda)                                                 | ✓     | ✓    | ✓      | ✓         |
 | [LongestMaxSize](https://albumentations.ai/docs/api_reference/augmentations/geometric/resize/#albumentations.augmentations.geometric.resize.LongestMaxSize)                     | ✓     | ✓    | ✓      | ✓         |
```

### Comparing `albumentations-1.4.3/README.md` & `albumentations-1.4.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Albumentations
 
 [![PyPI version](https://badge.fury.io/py/albumentations.svg)](https://badge.fury.io/py/albumentations)
 ![CI](https://github.com/albumentations-team/albumentations/workflows/CI/badge.svg)
 [![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![Pydantic v2](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/main/docs/badge/v2.json)](https://pydantic.dev)
 
 [Docs](https://albumentations.ai/docs/) | [Discord](https://discord.gg/AKPrrDYNAt) | [Twitter](https://twitter.com/albumentations) | [LinkedIn](https://www.linkedin.com/company/100504475/)
 
 Albumentations is a Python library for image augmentation. Image augmentation is used in deep learning and computer vision tasks to increase the quality of trained models. The purpose of image augmentation is to create new training samples from the existing data.
 
 Here is an example of how you can apply some [pixel-level](#pixel-level-transforms) augmentations from Albumentations to create new images from the original one:
 ![parrot](https://habrastorage.org/webt/bd/ne/rv/bdnerv5ctkudmsaznhw4crsdfiw.jpeg)
@@ -213,14 +214,15 @@
 | [Affine](https://albumentations.ai/docs/api_reference/augmentations/geometric/transforms/#albumentations.augmentations.geometric.transforms.Affine)                             | ✓     | ✓    | ✓      | ✓         |
 | [BBoxSafeRandomCrop](https://albumentations.ai/docs/api_reference/augmentations/crops/transforms/#albumentations.augmentations.crops.transforms.BBoxSafeRandomCrop)             | ✓     | ✓    | ✓      |           |
 | [CenterCrop](https://albumentations.ai/docs/api_reference/augmentations/crops/transforms/#albumentations.augmentations.crops.transforms.CenterCrop)                             | ✓     | ✓    | ✓      | ✓         |
 | [CoarseDropout](https://albumentations.ai/docs/api_reference/augmentations/dropout/coarse_dropout/#albumentations.augmentations.dropout.coarse_dropout.CoarseDropout)           | ✓     | ✓    |        | ✓         |
 | [Crop](https://albumentations.ai/docs/api_reference/augmentations/crops/transforms/#albumentations.augmentations.crops.transforms.Crop)                                         | ✓     | ✓    | ✓      | ✓         |
 | [CropAndPad](https://albumentations.ai/docs/api_reference/augmentations/crops/transforms/#albumentations.augmentations.crops.transforms.CropAndPad)                             | ✓     | ✓    | ✓      | ✓         |
 | [CropNonEmptyMaskIfExists](https://albumentations.ai/docs/api_reference/augmentations/crops/transforms/#albumentations.augmentations.crops.transforms.CropNonEmptyMaskIfExists) | ✓     | ✓    | ✓      | ✓         |
+| [D4](https://albumentations.ai/docs/api_reference/augmentations/geometric/transforms/#albumentations.augmentations.geometric.transforms.D4)                                     | ✓     | ✓    | ✓      | ✓         |
 | [ElasticTransform](https://albumentations.ai/docs/api_reference/augmentations/geometric/transforms/#albumentations.augmentations.geometric.transforms.ElasticTransform)         | ✓     | ✓    | ✓      |           |
 | [Flip](https://albumentations.ai/docs/api_reference/augmentations/geometric/transforms/#albumentations.augmentations.geometric.transforms.Flip)                                 | ✓     | ✓    | ✓      | ✓         |
 | [GridDistortion](https://albumentations.ai/docs/api_reference/augmentations/geometric/transforms/#albumentations.augmentations.geometric.transforms.GridDistortion)             | ✓     | ✓    | ✓      |           |
 | [GridDropout](https://albumentations.ai/docs/api_reference/augmentations/dropout/grid_dropout/#albumentations.augmentations.dropout.grid_dropout.GridDropout)                   | ✓     | ✓    |        |           |
 | [HorizontalFlip](https://albumentations.ai/docs/api_reference/augmentations/geometric/transforms/#albumentations.augmentations.geometric.transforms.HorizontalFlip)             | ✓     | ✓    | ✓      | ✓         |
 | [Lambda](https://albumentations.ai/docs/api_reference/augmentations/transforms/#albumentations.augmentations.transforms.Lambda)                                                 | ✓     | ✓    | ✓      | ✓         |
 | [LongestMaxSize](https://albumentations.ai/docs/api_reference/augmentations/geometric/resize/#albumentations.augmentations.geometric.resize.LongestMaxSize)                     | ✓     | ✓    | ✓      | ✓         |
```

#### html2text {}

```diff
@@ -1,14 +1,16 @@
 # Albumentations [![PyPI version](https://badge.fury.io/py/albumentations.svg)]
 (https://badge.fury.io/py/albumentations) ![CI](https://github.com/
 albumentations-team/albumentations/workflows/CI/badge.svg) [![License: MIT]
 (https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://
 opensource.org/licenses/MIT) [![Ruff](https://img.shields.io/
 endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/
-badge/v2.json)](https://github.com/astral-sh/ruff) [Docs](https://
+badge/v2.json)](https://github.com/astral-sh/ruff) [![Pydantic v2](https://
+img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/
+pydantic/main/docs/badge/v2.json)](https://pydantic.dev) [Docs](https://
 albumentations.ai/docs/) | [Discord](https://discord.gg/AKPrrDYNAt) | [Twitter]
 (https://twitter.com/albumentations) | [LinkedIn](https://www.linkedin.com/
 company/100504475/) Albumentations is a Python library for image augmentation.
 Image augmentation is used in deep learning and computer vision tasks to
 increase the quality of trained models. The purpose of image augmentation is to
 create new training samples from the existing data. Here is an example of how
 you can apply some [pixel-level](#pixel-level-transforms) augmentations from
@@ -254,16 +256,19 @@
 crops/transforms/#albumentations.augmentations.crops.transforms.Crop) | â |
 â | â | â | | [CropAndPad](https://albumentations.ai/docs/api_reference/
 augmentations/crops/transforms/
 #albumentations.augmentations.crops.transforms.CropAndPad) | â | â | â |
 â | | [CropNonEmptyMaskIfExists](https://albumentations.ai/docs/
 api_reference/augmentations/crops/transforms/
 #albumentations.augmentations.crops.transforms.CropNonEmptyMaskIfExists) | â
-| â | â | â | | [ElasticTransform](https://albumentations.ai/docs/
-api_reference/augmentations/geometric/transforms/
+| â | â | â | | [D4](https://albumentations.ai/docs/api_reference/
+augmentations/geometric/transforms/
+#albumentations.augmentations.geometric.transforms.D4) | â | â | â | â
+| | [ElasticTransform](https://albumentations.ai/docs/api_reference/
+augmentations/geometric/transforms/
 #albumentations.augmentations.geometric.transforms.ElasticTransform) | â |
 â | â | | | [Flip](https://albumentations.ai/docs/api_reference/
 augmentations/geometric/transforms/
 #albumentations.augmentations.geometric.transforms.Flip) | â | â | â |
 â | | [GridDistortion](https://albumentations.ai/docs/api_reference/
 augmentations/geometric/transforms/
 #albumentations.augmentations.geometric.transforms.GridDistortion) | â | â
```

### Comparing `albumentations-1.4.3/albumentations/augmentations/__init__.py` & `albumentations-1.4.4/albumentations/augmentations/__init__.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.3/albumentations/augmentations/blur/functional.py` & `albumentations-1.4.4/albumentations/augmentations/blur/functional.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,20 @@
     # When sigma=0, it is computed as `sigma = 0.3*((ksize-1)*0.5 - 1) + 0.8`
     blur_fn = _maybe_process_in_chunks(cv2.GaussianBlur, ksize=(ksize, ksize), sigmaX=sigma)
     return blur_fn(img)
 
 
 @preserve_shape
 def glass_blur(
-    img: np.ndarray, sigma: float, max_delta: int, iterations: int, dxy: np.ndarray, mode: str
+    img: np.ndarray,
+    sigma: float,
+    max_delta: int,
+    iterations: int,
+    dxy: np.ndarray,
+    mode: str,
 ) -> np.ndarray:
     x = cv2.GaussianBlur(np.array(img), sigmaX=sigma, ksize=(0, 0))
 
     if mode == "fast":
         hs = np.arange(img.shape[0] - max_delta, max_delta, -1)
         ws = np.arange(img.shape[1] - max_delta, max_delta, -1)
         h: Union[int, np.ndarray] = np.tile(hs, ws.shape[0])
@@ -60,15 +65,15 @@
 
     elif mode == "exact":
         for ind, (i, h, w) in enumerate(
             product(
                 range(iterations),
                 range(img.shape[0] - max_delta, max_delta, -1),
                 range(img.shape[1] - max_delta, max_delta, -1),
-            )
+            ),
         ):
             idx = ind if ind < len(dxy) else ind % len(dxy)
             dy = dxy[idx, i, 0]
             dx = dxy[idx, i, 1]
             x[h, w], x[h + dy, w + dx] = x[h + dy, w + dx], x[h, w]
     else:
         ValueError(f"Unsupported mode `{mode}`. Supports only `fast` and `exact`.")
```

### Comparing `albumentations-1.4.3/albumentations/augmentations/blur/transforms.py` & `albumentations-1.4.4/albumentations/augmentations/blur/transforms.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,58 @@
 import random
 import warnings
-from typing import Any, Dict, List, Optional, Sequence, Tuple, cast
+from typing import Any, Dict, List, Literal, Optional, Tuple, cast
 
 import cv2
 import numpy as np
+from pydantic import Field, ValidationInfo, field_validator, model_validator
+from typing_extensions import Self
 
 from albumentations import random_utils
 from albumentations.augmentations import functional as FMain
-from albumentations.core.transforms_interface import ImageOnlyTransform, to_tuple
+from albumentations.augmentations.utils import check_range
+from albumentations.core.pydantic import (
+    NonNegativeFloatRangeType,
+    OnePlusFloatRangeType,
+    OnePlusIntRangeType,
+    SymmetricRangeType,
+)
+from albumentations.core.transforms_interface import BaseTransformInitSchema, ImageOnlyTransform
 from albumentations.core.types import ScaleFloatType, ScaleIntType
+from albumentations.core.utils import to_tuple
 
 from . import functional as F
 
 __all__ = ["Blur", "MotionBlur", "GaussianBlur", "GlassBlur", "AdvancedBlur", "MedianBlur", "Defocus", "ZoomBlur"]
 
 
-HALF = 0
+HALF = 0.5
 TWO = 2
 
 
+def process_blur_limit(value: ScaleIntType, info: ValidationInfo, min_value: float = 0) -> Tuple[int, int]:
+    bounds = 0, float("inf")
+    result = to_tuple(value, min_value)
+    check_range(result, *bounds, info.field_name)
+
+    for v in result:
+        if v != 0 and v % 2 != 1:
+            raise ValueError(f"Blur limit must be 0 or odd. Got: {result}")
+    return cast(Tuple[int, int], result)
+
+
+class BlurInitSchema(BaseTransformInitSchema):
+    blur_limit: ScaleIntType = Field(default=(3, 7), description="Maximum kernel size for blurring the input image.")
+
+    @field_validator("blur_limit")
+    @classmethod
+    def process_blur(cls, value: ScaleIntType, info: ValidationInfo) -> Tuple[int, int]:
+        return process_blur_limit(value, info, min_value=3)
+
+
 class Blur(ImageOnlyTransform):
     """Blur the input image using a random-sized kernel.
 
     Args:
         blur_limit: maximum kernel size for blurring the input image.
             Should be in range [3, inf). Default: (3, 7).
         p: probability of applying the transform. Default: 0.5.
@@ -31,17 +61,20 @@
         image
 
     Image types:
         uint8, float32
 
     """
 
+    class InitSchema(BlurInitSchema):
+        pass
+
     def __init__(self, blur_limit: ScaleIntType = 7, always_apply: bool = False, p: float = 0.5):
         super().__init__(always_apply, p)
-        self.blur_limit = cast(Tuple[int, int], to_tuple(blur_limit, 3))
+        self.blur_limit = cast(Tuple[int, int], blur_limit)
 
     def apply(self, img: np.ndarray, kernel: int = 3, **params: Any) -> np.ndarray:
         return F.blur(img, kernel)
 
     def get_params(self) -> Dict[str, Any]:
         return {"ksize": int(random.choice(list(range(self.blur_limit[0], self.blur_limit[1] + 1, 2))))}
 
@@ -63,26 +96,43 @@
         image
 
     Image types:
         uint8, float32
 
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        allow_shifted: bool = Field(
+            default=True,
+            description="If set to true creates non-shifted kernels only, otherwise creates randomly shifted kernels.",
+        )
+        blur_limit: ScaleIntType = Field(
+            default=(3, 7),
+            description="Maximum kernel size for blurring the input image.",
+        )
+
+        @model_validator(mode="after")
+        def process_blur(self) -> Self:
+            self.blur_limit = cast(Tuple[int, int], to_tuple(self.blur_limit, 3))
+
+            if self.allow_shifted and isinstance(self.blur_limit, tuple) and any(x % 2 != 1 for x in self.blur_limit):
+                raise ValueError(f"Blur limit must be odd when centered=True. Got: {self.blur_limit}")
+
+            return self
+
     def __init__(
         self,
         blur_limit: ScaleIntType = 7,
         allow_shifted: bool = True,
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(blur_limit=blur_limit, always_apply=always_apply, p=p)
         self.allow_shifted = allow_shifted
-
-        if not allow_shifted and self.blur_limit[0] % 2 != 1 or self.blur_limit[1] % 2 != 1:
-            raise ValueError(f"Blur limit must be odd when centered=True. Got: {self.blur_limit}")
+        self.blur_limit = cast(Tuple[int, int], blur_limit)
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return (*super().get_transform_init_args_names(), "allow_shifted")
 
     def apply(self, img: np.ndarray, kernel: Optional[np.ndarray] = None, **params: Any) -> np.ndarray:
         return FMain.convolve(img, kernel=kernel)
 
@@ -140,18 +190,14 @@
         uint8, float32
 
     """
 
     def __init__(self, blur_limit: ScaleIntType = 7, always_apply: bool = False, p: float = 0.5):
         super().__init__(blur_limit, always_apply, p)
 
-        if self.blur_limit[0] % 2 != 1 or self.blur_limit[1] % 2 != 1:
-            msg = "MedianBlur supports only odd blur limits."
-            raise ValueError(msg)
-
     def apply(self, img: np.ndarray, kernel: int = 3, **params: Any) -> np.ndarray:
         return F.median_blur(img, kernel)
 
 
 class GaussianBlur(ImageOnlyTransform):
     """Blur the input image using a Gaussian filter with a random kernel size.
 
@@ -170,37 +216,53 @@
         image
 
     Image types:
         uint8, float32
 
     """
 
+    class InitSchema(BlurInitSchema):
+        sigma_limit: NonNegativeFloatRangeType = 0
+
+        @field_validator("blur_limit")
+        @classmethod
+        def process_blur(cls, value: ScaleIntType, info: ValidationInfo) -> Tuple[int, int]:
+            return process_blur_limit(value, info, min_value=0)
+
+        @model_validator(mode="after")
+        def validate_limits(self) -> Self:
+            if (
+                isinstance(self.blur_limit, (tuple, list))
+                and self.blur_limit[0] == 0
+                and isinstance(self.sigma_limit, (tuple, list))
+                and self.sigma_limit[0] == 0
+            ):
+                self.blur_limit = 3, max(3, self.blur_limit[1])
+                warnings.warn(
+                    "blur_limit and sigma_limit minimum value can not be both equal to 0. "
+                    "blur_limit minimum value changed to 3.",
+                )
+
+            if isinstance(self.blur_limit, tuple):
+                for v in self.blur_limit:
+                    if v != 0 and v % 2 != 1:
+                        raise ValueError(f"Blur limit must be 0 or odd. Got: {self.blur_limit}")
+
+            return self
+
     def __init__(
         self,
         blur_limit: ScaleIntType = (3, 7),
         sigma_limit: ScaleFloatType = 0,
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
-        self.blur_limit = cast(Tuple[int, int], to_tuple(blur_limit, 0))
-        self.sigma_limit = to_tuple(sigma_limit if sigma_limit is not None else 0, 0)
-
-        if self.blur_limit[0] == 0 and self.sigma_limit[0] == 0:
-            self.blur_limit = 3, max(3, self.blur_limit[1])
-            warnings.warn(
-                "blur_limit and sigma_limit minimum value can not be both equal to 0. "
-                "blur_limit minimum value changed to 3."
-            )
-
-        if (self.blur_limit[0] != 0 and self.blur_limit[0] % 2 != 1) or (
-            self.blur_limit[1] != 0 and self.blur_limit[1] % 2 != 1
-        ):
-            msg = "GaussianBlur supports only odd blur limits."
-            raise ValueError(msg)
+        self.blur_limit = cast(Tuple[int, int], blur_limit)
+        self.sigma_limit = cast(Tuple[float, float], sigma_limit)
 
     def apply(self, img: np.ndarray, ksize: int = 3, sigma: float = 0, **params: Any) -> np.ndarray:
         return F.gaussian_blur(img, ksize, sigma=sigma)
 
     def get_params(self) -> Dict[str, float]:
         ksize = random.randrange(self.blur_limit[0], self.blur_limit[1] + 1)
         if ksize != 0 and ksize % 2 != 1:
@@ -208,15 +270,15 @@
 
         return {"ksize": ksize, "sigma": random.uniform(*self.sigma_limit)}
 
     def get_transform_init_args_names(self) -> Tuple[str, str]:
         return ("blur_limit", "sigma_limit")
 
 
-class GlassBlur(Blur):
+class GlassBlur(ImageOnlyTransform):
     """Apply glass noise to the input image.
 
     Args:
         sigma (float): standard deviation for Gaussian kernel.
         max_delta (int): max distance between pixels which are swapped.
         iterations (int): number of repeats.
             Should be in range [1, inf). Default: (2).
@@ -226,35 +288,35 @@
     Targets:
         image
 
     Image types:
         uint8, float32
 
     Reference:
-    |  https://arxiv.org/abs/1903.12261
-    |  https://github.com/hendrycks/robustness/blob/master/ImageNet-C/create_c/make_imagenet_c.py
+        https://arxiv.org/abs/1903.12261
+        https://github.com/hendrycks/robustness/blob/master/ImageNet-C/create_c/make_imagenet_c.py
 
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        sigma: float = Field(default=0.7, ge=0, description="Standard deviation for the Gaussian kernel.")
+        max_delta: int = Field(default=4, ge=1, description="Maximum distance between pixels that are swapped.")
+        iterations: int = Field(default=2, ge=1, description="Number of times the glass noise effect is applied.")
+        mode: Literal["fast", "exact"] = "fast"
+
     def __init__(
         self,
         sigma: float = 0.7,
         max_delta: int = 4,
         iterations: int = 2,
+        mode: Literal["fast", "exact"] = "fast",
         always_apply: bool = False,
-        mode: str = "fast",
         p: float = 0.5,
     ):
         super().__init__(always_apply=always_apply, p=p)
-        if iterations < 1:
-            raise ValueError(f"Iterations should be more or equal to 1, but we got {iterations}")
-
-        if mode not in ["fast", "exact"]:
-            raise ValueError(f"Mode should be 'fast' or 'exact', but we got {mode}")
-
         self.sigma = sigma
         self.max_delta = max_delta
         self.iterations = iterations
         self.mode = mode
 
     def apply(self, img: np.ndarray, *args: Any, dxy: np.ndarray = None, **params: Any) -> np.ndarray:
         if dxy is None:
@@ -262,17 +324,19 @@
             raise ValueError(msg)
 
         return F.glass_blur(img, self.sigma, self.max_delta, self.iterations, dxy, self.mode)
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, np.ndarray]:
         img = params["image"]
 
+        height, width = img.shape[:2]
+
         # generate array containing all necessary values for transformations
-        width_pixels = img.shape[0] - self.max_delta * 2
-        height_pixels = img.shape[1] - self.max_delta * 2
+        width_pixels = height - self.max_delta * 2
+        height_pixels = width - self.max_delta * 2
         total_pixels = int(width_pixels * height_pixels)
         dxy = random_utils.randint(-self.max_delta, self.max_delta, size=(total_pixels, self.iterations, 2))
 
         return {"dxy": dxy}
 
     def get_transform_init_args_names(self) -> Tuple[str, str, str, str]:
         return ("sigma", "max_delta", "iterations", "mode")
@@ -324,74 +388,79 @@
         image
 
     Image types:
         uint8, float32
 
     """
 
+    class InitSchema(BlurInitSchema):
+        sigma_x_limit: NonNegativeFloatRangeType = (0.2, 1.0)
+        sigma_y_limit: NonNegativeFloatRangeType = (0.2, 1.0)
+        beta_limit: NonNegativeFloatRangeType = (0.5, 8.0)
+        noise_limit: NonNegativeFloatRangeType = (0.75, 1.25)
+        rotate_limit: SymmetricRangeType = (-90, 90)
+
+        @field_validator("beta_limit")
+        @classmethod
+        def check_beta_limit(cls, value: ScaleFloatType) -> Tuple[float, float]:
+            result = to_tuple(value, low=0)
+            if not (result[0] < 1.0 < result[1]):
+                msg = "beta_limit is expected to include 1.0."
+                raise ValueError(msg)
+            return result
+
+        @model_validator(mode="after")
+        def validate_limits(self) -> Self:
+            if (
+                isinstance(self.sigma_x_limit, (tuple, list))
+                and self.sigma_x_limit[0] == 0
+                and isinstance(self.sigma_y_limit, (tuple, list))
+                and self.sigma_y_limit[0] == 0
+            ):
+                msg = "sigma_x_limit and sigma_y_limit minimum value cannot be both equal to 0."
+                raise ValueError(msg)
+            return self
+
     def __init__(
         self,
         blur_limit: ScaleIntType = (3, 7),
         sigma_x_limit: ScaleFloatType = (0.2, 1.0),
         sigma_y_limit: ScaleFloatType = (0.2, 1.0),
         sigmaX_limit: Optional[ScaleFloatType] = None,  # noqa: N803
         sigmaY_limit: Optional[ScaleFloatType] = None,  # noqa: N803
         rotate_limit: ScaleIntType = 90,
         beta_limit: ScaleFloatType = (0.5, 8.0),
         noise_limit: ScaleFloatType = (0.9, 1.1),
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
-        self.blur_limit = cast(Tuple[int, int], to_tuple(blur_limit, 3))
 
-        # Handle deprecation of sigmaX_limit and sigmaY_limit
         if sigmaX_limit is not None:
             warnings.warn("sigmaX_limit is deprecated; use sigma_x_limit instead.", DeprecationWarning)
             sigma_x_limit = sigmaX_limit
 
         if sigmaY_limit is not None:
             warnings.warn("sigmaY_limit is deprecated; use sigma_y_limit instead.", DeprecationWarning)
             sigma_y_limit = sigmaY_limit
 
-        self.sigma_x_limit = self.__check_values(to_tuple(sigma_x_limit, 0.0), name="sigma_x_limit")
-        self.sigma_y_limit = self.__check_values(to_tuple(sigma_y_limit, 0.0), name="sigma_y_limit")
-        self.rotate_limit = to_tuple(rotate_limit)
-        self.beta_limit = to_tuple(beta_limit, low=0.0)
-        self.noise_limit = self.__check_values(to_tuple(noise_limit, 0.0), name="noise_limit")
-
-        if (self.blur_limit[0] != 0 and self.blur_limit[0] % 2 != 1) or (
-            self.blur_limit[1] != 0 and self.blur_limit[1] % 2 != 1
-        ):
-            msg = "AdvancedBlur supports only odd blur limits."
-            raise ValueError(msg)
-
-        if self.sigma_x_limit[0] == 0 and self.sigma_y_limit[0] == 0:
-            msg = "sigma_x_limit and sigma_y_limit minimum value cannot be both equal to 0."
-            raise ValueError(msg)
-
-        if not (self.beta_limit[0] < 1.0 < self.beta_limit[1]):
-            msg = "Beta limit is expected to include 1.0."
-            raise ValueError(msg)
-
-    @staticmethod
-    def __check_values(
-        value: Sequence[float], name: str, bounds: Tuple[float, float] = (0, float("inf"))
-    ) -> Sequence[float]:
-        if not bounds[0] <= value[0] <= value[1] <= bounds[1]:
-            raise ValueError(f"{name} values should be between {bounds}")
-        return value
+        self.blur_limit = cast(Tuple[int, int], blur_limit)
+        self.sigma_x_limit = cast(Tuple[float, float], sigma_x_limit)
+        self.sigma_y_limit = cast(Tuple[float, float], sigma_y_limit)
+        self.rotate_limit = cast(Tuple[int, int], rotate_limit)
+        self.beta_limit = cast(Tuple[float, float], beta_limit)
+        self.noise_limit = cast(Tuple[float, float], noise_limit)
 
     def apply(self, img: np.ndarray, kernel: Optional[np.ndarray] = None, **params: Any) -> np.ndarray:
         return FMain.convolve(img, kernel=kernel)
 
     def get_params(self) -> Dict[str, np.ndarray]:
         ksize = random.randrange(self.blur_limit[0], self.blur_limit[1] + 1, 2)
-        sigma_x = random.uniform(*self.sigma_x_limit)
-        sigma_y = random.uniform(*self.sigma_y_limit)
+        sigma_x = random_utils.uniform(*self.sigma_x_limit)
+        sigma_y = random_utils.uniform(*self.sigma_y_limit)
         angle = np.deg2rad(random.uniform(*self.rotate_limit))
 
         # Split into 2 cases to avoid selection of narrow kernels (beta > 1) too often.
         beta = (
             random.uniform(self.beta_limit[0], 1) if random.random() < HALF else random.uniform(1, self.beta_limit[1])
         )
 
@@ -425,49 +494,47 @@
             "rotate_limit",
             "beta_limit",
             "noise_limit",
         )
 
 
 class Defocus(ImageOnlyTransform):
-    """Apply defocus transform. See https://arxiv.org/abs/1903.12261.
+    """Apply defocus transform.
 
     Args:
         radius ((int, int) or int): range for radius of defocusing.
             If limit is a single int, the range will be [1, limit]. Default: (3, 10).
         alias_blur ((float, float) or float): range for alias_blur of defocusing (sigma of gaussian blur).
             If limit is a single float, the range will be (0, limit). Default: (0.1, 0.5).
         p (float): probability of applying the transform. Default: 0.5.
 
     Targets:
         image
 
     Image types:
-        Any
+        unit8, float32
 
+    Reference:
+        https://arxiv.org/abs/1903.12261
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        radius: OnePlusIntRangeType = (3, 10)
+        alias_blur: NonNegativeFloatRangeType = (0.1, 0.5)
+
     def __init__(
         self,
         radius: ScaleIntType = (3, 10),
         alias_blur: ScaleFloatType = (0.1, 0.5),
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
-        self.radius = to_tuple(radius, low=1)
-        self.alias_blur = to_tuple(alias_blur, low=0)
-
-        if self.radius[0] <= 0:
-            msg = "Parameter radius must be positive"
-            raise ValueError(msg)
-
-        if self.alias_blur[0] < 0:
-            msg = "Parameter alias_blur must be non-negative"
-            raise ValueError(msg)
+        self.radius = cast(Tuple[int, int], radius)
+        self.alias_blur = cast(Tuple[float, float], alias_blur)
 
     def apply(self, img: np.ndarray, radius: int = 3, alias_blur: float = 0.5, **params: Any) -> np.ndarray:
         return F.defocus(img, radius, alias_blur)
 
     def get_params(self) -> Dict[str, Any]:
         return {
             "radius": random_utils.randint(self.radius[0], self.radius[1] + 1),
@@ -475,50 +542,49 @@
         }
 
     def get_transform_init_args_names(self) -> Tuple[str, str]:
         return ("radius", "alias_blur")
 
 
 class ZoomBlur(ImageOnlyTransform):
-    """Apply zoom blur transform. See https://arxiv.org/abs/1903.12261.
+    """Apply zoom blur transform.
 
     Args:
         max_factor ((float, float) or float): range for max factor for blurring.
             If max_factor is a single float, the range will be (1, limit). Default: (1, 1.31).
             All max_factor values should be larger than 1.
         step_factor ((float, float) or float): If single float will be used as step parameter for np.arange.
             If tuple of float step_factor will be in range `[step_factor[0], step_factor[1])`. Default: (0.01, 0.03).
             All step_factor values should be positive.
         p (float): probability of applying the transform. Default: 0.5.
 
     Targets:
         image
 
     Image types:
-        Any
+        unit8, float32
 
+    Reference:
+        https://arxiv.org/abs/1903.12261
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        max_factor: OnePlusFloatRangeType = (1, 1.31)
+        step_factor: NonNegativeFloatRangeType = (0.01, 0.03)
+
     def __init__(
         self,
-        max_factor: ScaleFloatType = 1.31,
+        max_factor: ScaleFloatType = (1, 1.31),
         step_factor: ScaleFloatType = (0.01, 0.03),
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
-        self.max_factor = to_tuple(max_factor, low=1.0)
-        self.step_factor = to_tuple(step_factor, step_factor)
-
-        if self.max_factor[0] < 1:
-            msg = "Max factor must be larger or equal 1"
-            raise ValueError(msg)
-        if self.step_factor[0] <= 0:
-            msg = "Step factor must be positive"
-            raise ValueError(msg)
+        self.max_factor = cast(Tuple[float, float], max_factor)
+        self.step_factor = cast(Tuple[float, float], step_factor)
 
     def apply(self, img: np.ndarray, zoom_factors: Optional[np.ndarray] = None, **params: Any) -> np.ndarray:
         if zoom_factors is None:
             msg = "zoom_factors is None"
             raise ValueError(msg)
 
         return F.zoom_blur(img, zoom_factors)
```

### Comparing `albumentations-1.4.3/albumentations/augmentations/crops/functional.py` & `albumentations-1.4.4/albumentations/augmentations/crops/functional.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,20 @@
     "crop_and_pad",
     "crop_and_pad_bbox",
     "crop_and_pad_keypoint",
 ]
 
 
 def get_random_crop_coords(
-    height: int, width: int, crop_height: int, crop_width: int, h_start: float, w_start: float
+    height: int,
+    width: int,
+    crop_height: int,
+    crop_width: int,
+    h_start: float,
+    w_start: float,
 ) -> Tuple[int, int, int, int]:
     # h_start is [0, 1) and should map to [0, (height - crop_height)]  (note inclusive)
     # This is conceptually equivalent to mapping onto `range(0, (height - crop_height + 1))`
     # See: https://github.com/albumentations-team/albumentations/pull/1080
     y1 = int((height - crop_height + 1) * h_start)
     y2 = y1 + crop_height
     x1 = int((width - crop_width + 1) * w_start)
@@ -44,15 +49,15 @@
     return x1, y1, x2, y2
 
 
 def random_crop(img: np.ndarray, crop_height: int, crop_width: int, h_start: float, w_start: float) -> np.ndarray:
     height, width = img.shape[:2]
     if height < crop_height or width < crop_width:
         raise ValueError(
-            f"Requested crop size ({crop_height}, {crop_width}) is " f"larger than the image size ({height}, {width})"
+            f"Requested crop size ({crop_height}, {crop_width}) is larger than the image size ({height}, {width})",
         )
     x1, y1, x2, y2 = get_random_crop_coords(height, width, crop_height, crop_width, h_start, w_start)
     return img[y1:y2, x1:x2]
 
 
 def crop_bbox_by_coords(
     bbox: BoxInternalType,
@@ -81,22 +86,29 @@
     x_min, y_min, x_max, y_max = normalized_bbox[:4]
     x1, y1 = crop_coords[:2]
     cropped_bbox = x_min - x1, y_min - y1, x_max - x1, y_max - y1
     return cast(BoxInternalType, normalize_bbox(cropped_bbox, crop_height, crop_width))
 
 
 def bbox_random_crop(
-    bbox: BoxInternalType, crop_height: int, crop_width: int, h_start: float, w_start: float, rows: int, cols: int
+    bbox: BoxInternalType,
+    crop_height: int,
+    crop_width: int,
+    h_start: float,
+    w_start: float,
+    rows: int,
+    cols: int,
 ) -> BoxInternalType:
     crop_coords = get_random_crop_coords(rows, cols, crop_height, crop_width, h_start, w_start)
     return crop_bbox_by_coords(bbox, crop_coords, crop_height, crop_width, rows, cols)
 
 
 def crop_keypoint_by_coords(
-    keypoint: KeypointInternalType, crop_coords: Tuple[int, int, int, int]
+    keypoint: KeypointInternalType,
+    crop_coords: Tuple[int, int, int, int],
 ) -> KeypointInternalType:
     """Crop a keypoint using the provided coordinates of bottom-left and top-right corners in pixels and the
     required height and width of the crop.
 
     Args:
         keypoint (tuple): A keypoint `(x, y, angle, scale)`.
         crop_coords (tuple): Crop box coords `(x1, x2, y1, y2)`.
@@ -146,27 +158,31 @@
     return x1, y1, x2, y2
 
 
 def center_crop(img: np.ndarray, crop_height: int, crop_width: int) -> np.ndarray:
     height, width = img.shape[:2]
     if height < crop_height or width < crop_width:
         raise ValueError(
-            f"Requested crop size ({crop_height}, {crop_width}) is " f"larger than the image size ({height}, {width})"
+            f"Requested crop size ({crop_height}, {crop_width}) is larger than the image size ({height}, {width})",
         )
     x1, y1, x2, y2 = get_center_crop_coords(height, width, crop_height, crop_width)
     return img[y1:y2, x1:x2]
 
 
 def bbox_center_crop(bbox: BoxInternalType, crop_height: int, crop_width: int, rows: int, cols: int) -> BoxInternalType:
     crop_coords = get_center_crop_coords(rows, cols, crop_height, crop_width)
     return crop_bbox_by_coords(bbox, crop_coords, crop_height, crop_width, rows, cols)
 
 
 def keypoint_center_crop(
-    keypoint: KeypointInternalType, crop_height: int, crop_width: int, rows: int, cols: int
+    keypoint: KeypointInternalType,
+    crop_height: int,
+    crop_width: int,
+    rows: int,
+    cols: int,
 ) -> KeypointInternalType:
     """Keypoint center crop.
 
     Args:
         keypoint: A keypoint `(x, y, angle, scale)`.
         crop_height: Crop height.
         crop_width: Crop width.
@@ -182,29 +198,35 @@
 
 
 def crop(img: np.ndarray, x_min: int, y_min: int, x_max: int, y_max: int) -> np.ndarray:
     height, width = img.shape[:2]
     if x_max <= x_min or y_max <= y_min:
         raise ValueError(
             "We should have x_min < x_max and y_min < y_max. But we got"
-            f" (x_min = {x_min}, y_min = {y_min}, x_max = {x_max}, y_max = {y_max})"
+            f" (x_min = {x_min}, y_min = {y_min}, x_max = {x_max}, y_max = {y_max})",
         )
 
     if x_min < 0 or x_max > width or y_min < 0 or y_max > height:
         raise ValueError(
             "Values for crop should be non negative and equal or smaller than image sizes"
             f"(x_min = {x_min}, y_min = {y_min}, x_max = {x_max}, y_max = {y_max}, "
-            f"height = {height}, width = {width})"
+            f"height = {height}, width = {width})",
         )
 
     return img[y_min:y_max, x_min:x_max]
 
 
 def bbox_crop(
-    bbox: BoxInternalType, x_min: int, y_min: int, x_max: int, y_max: int, rows: int, cols: int
+    bbox: BoxInternalType,
+    x_min: int,
+    y_min: int,
+    x_max: int,
+    y_max: int,
+    rows: int,
+    cols: int,
 ) -> BoxInternalType:
     """Crop a bounding box.
 
     Args:
         bbox: A bounding box `(x_min, y_min, x_max, y_max)`.
         x_min:
         y_min:
@@ -248,15 +270,21 @@
     pad_mode: int,
     keep_size: bool,
 ) -> np.ndarray:
     if crop_params is not None and any(i != 0 for i in crop_params):
         img = crop(img, *crop_params)
     if pad_params is not None and any(i != 0 for i in pad_params):
         img = FGeometric.pad_with_params(
-            img, pad_params[0], pad_params[1], pad_params[2], pad_params[3], border_mode=pad_mode, value=pad_value
+            img,
+            pad_params[0],
+            pad_params[1],
+            pad_params[2],
+            pad_params[3],
+            border_mode=pad_mode,
+            value=pad_value,
         )
 
     if keep_size:
         resize_fn = _maybe_process_in_chunks(cv2.resize, dsize=(cols, rows), interpolation=interpolation)
         return resize_fn(img)
 
     return img
```

### Comparing `albumentations-1.4.3/albumentations/augmentations/crops/transforms.py` & `albumentations-1.4.4/albumentations/augmentations/crops/transforms.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,37 @@
 import math
 import random
-from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
+from typing import Any, Dict, List, Optional, Sequence, Tuple, Union, cast
 from warnings import warn
 
 import cv2
 import numpy as np
+from pydantic import Field, field_validator, model_validator
+from typing_extensions import Annotated, Self
 
+from albumentations import random_utils
 from albumentations.augmentations.geometric import functional as FGeometric
 from albumentations.core.bbox_utils import union_of_bboxes
-from albumentations.core.transforms_interface import DualTransform, to_tuple
-from albumentations.core.types import BoxInternalType, KeypointInternalType, ScaleFloatType, Targets
+from albumentations.core.pydantic import (
+    BorderModeType,
+    InterpolationType,
+    NonNegativeFloatRangeType,
+    OnePlusIntRangeType,
+    ProbabilityType,
+    ZeroOneRangeType,
+)
+from albumentations.core.transforms_interface import BaseTransformInitSchema, DualTransform
+from albumentations.core.types import (
+    BoxInternalType,
+    ColorType,
+    KeypointInternalType,
+    ScaleFloatType,
+    ScaleIntType,
+    Targets,
+)
 
 from . import functional as F
 
 __all__ = [
     "RandomCrop",
     "CenterCrop",
     "Crop",
@@ -27,14 +45,20 @@
     "BBoxSafeRandomCrop",
 ]
 
 TWO = 2
 THREE = 3
 
 
+class CropInitSchema(BaseTransformInitSchema):
+    height: Optional[int] = Field(description="Height of the crop", ge=1)
+    width: Optional[int] = Field(description="Width of the crop", ge=1)
+    p: ProbabilityType = 1
+
+
 class RandomCrop(DualTransform):
     """Crop a random part of the input.
 
     Args:
         height: height of the crop.
         width: width of the crop.
         p: probability of applying the transform. Default: 1.
@@ -45,14 +69,17 @@
     Image types:
         uint8, float32
 
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS)
 
+    class InitSchema(CropInitSchema):
+        pass
+
     def __init__(self, height: int, width: int, always_apply: bool = False, p: float = 1.0):
         super().__init__(always_apply, p)
         self.height = height
         self.width = width
 
     def apply(self, img: np.ndarray, h_start: int = 0, w_start: int = 0, **params: Any) -> np.ndarray:
         return F.random_crop(img, self.height, self.width, h_start, w_start)
@@ -80,23 +107,21 @@
 
     Targets:
         image, mask, bboxes, keypoints
 
     Image types:
         uint8, float32
 
-    Note:
-        It is recommended to use uint8 images as input.
-        Otherwise the operation will require internal conversion
-        float32 -> uint8 -> float32 that causes worse performance.
-
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS)
 
+    class InitSchema(CropInitSchema):
+        pass
+
     def __init__(self, height: int, width: int, always_apply: bool = False, p: float = 1.0):
         super().__init__(always_apply, p)
         self.height = height
         self.width = width
 
     def apply(self, img: np.ndarray, **params: Any) -> np.ndarray:
         return F.center_crop(img, self.height, self.width)
@@ -126,14 +151,31 @@
     Image types:
         uint8, float32
 
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS)
 
+    class InitSchema(BaseTransformInitSchema):
+        x_min: Annotated[int, Field(ge=0, description="Minimum upper left x coordinate")]
+        y_min: Annotated[int, Field(ge=0, description="Minimum upper left y coordinate")]
+        x_max: Annotated[int, Field(gt=0, description="Maximum lower right x coordinate")]
+        y_max: Annotated[int, Field(gt=0, description="Maximum lower right y coordinate")]
+        p: ProbabilityType = 1
+
+        @model_validator(mode="after")
+        def validate_coordinates(self) -> Self:
+            if not self.x_min < self.x_max:
+                msg = "x_max must be greater than x_min"
+                raise ValueError(msg)
+            if not self.y_min < self.y_max:
+                msg = "y_max must be greater than y_min"
+                raise ValueError(msg)
+            return self
+
     def __init__(
         self,
         x_min: int = 0,
         y_min: int = 0,
         x_max: int = 1024,
         y_max: int = 1024,
         always_apply: bool = False,
@@ -176,45 +218,65 @@
     Image types:
         uint8, float32
 
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS)
 
+    class InitSchema(CropInitSchema):
+        ignore_values: Optional[List[int]] = Field(
+            default=None,
+            description="Values to ignore in mask, `0` values are always ignored",
+        )
+        ignore_channels: Optional[List[int]] = Field(default=None, description="Channels to ignore in mask")
+
     def __init__(
         self,
         height: int,
         width: int,
         ignore_values: Optional[List[int]] = None,
         ignore_channels: Optional[List[int]] = None,
         always_apply: bool = False,
         p: float = 1.0,
     ):
         super().__init__(always_apply, p)
 
-        if ignore_values is not None and not isinstance(ignore_values, list):
-            raise ValueError(f"Expected `ignore_values` of type `list`, got `{type(ignore_values)}`")
-        if ignore_channels is not None and not isinstance(ignore_channels, list):
-            raise ValueError(f"Expected `ignore_channels` of type `list`, got `{type(ignore_channels)}`")
-
         self.height = height
         self.width = width
         self.ignore_values = ignore_values
         self.ignore_channels = ignore_channels
 
     def apply(
-        self, img: np.ndarray, x_min: int = 0, x_max: int = 0, y_min: int = 0, y_max: int = 0, **params: Any
+        self,
+        img: np.ndarray,
+        x_min: int = 0,
+        x_max: int = 0,
+        y_min: int = 0,
+        y_max: int = 0,
+        **params: Any,
     ) -> np.ndarray:
         return F.crop(img, x_min, y_min, x_max, y_max)
 
     def apply_to_bbox(
-        self, bbox: BoxInternalType, x_min: int = 0, x_max: int = 0, y_min: int = 0, y_max: int = 0, **params: Any
+        self,
+        bbox: BoxInternalType,
+        x_min: int = 0,
+        x_max: int = 0,
+        y_min: int = 0,
+        y_max: int = 0,
+        **params: Any,
     ) -> BoxInternalType:
         return F.bbox_crop(
-            bbox, x_min=x_min, x_max=x_max, y_min=y_min, y_max=y_max, rows=params["rows"], cols=params["cols"]
+            bbox,
+            x_min=x_min,
+            x_max=x_max,
+            y_min=y_min,
+            y_max=y_max,
+            rows=params["rows"],
+            cols=params["cols"],
         )
 
     def apply_to_keypoint(
         self,
         keypoint: KeypointInternalType,
         x_min: int = 0,
         x_max: int = 0,
@@ -233,15 +295,15 @@
 
         if mask.ndim == THREE and self.ignore_channels is not None:
             target_channels = np.array([ch for ch in range(mask.shape[-1]) if ch not in self.ignore_channels])
             mask = np.take(mask, target_channels, axis=-1)
 
         if self.height > mask_height or self.width > mask_width:
             raise ValueError(
-                f"Crop size ({self.height},{self.width}) is larger than image ({mask_height},{mask_width})"
+                f"Crop size ({self.height},{self.width}) is larger than image ({mask_height},{mask_width})",
             )
 
         return mask
 
     def update_params(self, params: Dict[str, Any], **kwargs: Any) -> Dict[str, Any]:
         super().update_params(params, **kwargs)
         if "mask" in kwargs:
@@ -275,37 +337,54 @@
         params.update({"x_min": x_min, "x_max": x_max, "y_min": y_min, "y_max": y_max})
         return params
 
     def get_transform_init_args_names(self) -> Tuple[str, str, str, str]:
         return ("height", "width", "ignore_values", "ignore_channels")
 
 
+class BaseRandomSizedCropInitSchema(BaseTransformInitSchema):
+    size: Tuple[int, int]
+
+    @field_validator("size")
+    @classmethod
+    def check_size(cls, value: Tuple[int, int]) -> Tuple[int, int]:
+        if any(x <= 0 for x in value):
+            raise ValueError("All elements of 'size' must be positive integers.")
+        return value
+
+
 class _BaseRandomSizedCrop(DualTransform):
     # Base class for RandomSizedCrop and RandomResizedCrop
 
+    class InitSchema(BaseRandomSizedCropInitSchema):
+        pass
+
     def __init__(
-        self, height: int, width: int, interpolation: int = cv2.INTER_LINEAR, always_apply: bool = False, p: float = 1.0
+        self,
+        size: Tuple[int, int],
+        interpolation: int = cv2.INTER_LINEAR,
+        always_apply: bool = False,
+        p: float = 1.0,
     ):
         super().__init__(always_apply, p)
-        self.height = height
-        self.width = width
+        self.size = size
         self.interpolation = interpolation
 
     def apply(
         self,
         img: np.ndarray,
         crop_height: int = 0,
         crop_width: int = 0,
         h_start: int = 0,
         w_start: int = 0,
         interpolation: int = cv2.INTER_LINEAR,
         **params: Any,
     ) -> np.ndarray:
         crop = F.random_crop(img, crop_height, crop_width, h_start, w_start)
-        return FGeometric.resize(crop, self.height, self.width, interpolation)
+        return FGeometric.resize(crop, self.size[0], self.size[1], interpolation)
 
     def apply_to_bbox(
         self,
         bbox: BoxInternalType,
         crop_height: int = 0,
         crop_width: int = 0,
         h_start: int = 0,
@@ -324,25 +403,25 @@
         h_start: int = 0,
         w_start: int = 0,
         rows: int = 0,
         cols: int = 0,
         **params: Any,
     ) -> KeypointInternalType:
         keypoint = F.keypoint_random_crop(keypoint, crop_height, crop_width, h_start, w_start, rows, cols)
-        scale_x = self.width / crop_width
-        scale_y = self.height / crop_height
+        scale_y = self.size[0] / crop_height
+        scale_x = self.size[1] / crop_width
         return FGeometric.keypoint_scale(keypoint, scale_x, scale_y)
 
 
 class RandomSizedCrop(_BaseRandomSizedCrop):
     """Crop a random portion of the input and rescale it to a specific size.
 
     Args:
         min_max_height ((int, int)): crop size limits.
-        size (tuple[int]): target size for the output image, i.e. (height, width) after crop and resize
+        size ((int, int)): target size for the output image, i.e. (height, width) after crop and resize
         w2h_ratio (float): aspect ratio of crop.
         interpolation (OpenCV flag): flag that is used to specify the interpolation algorithm. Should be one of:
             cv2.INTER_NEAREST, cv2.INTER_LINEAR, cv2.INTER_CUBIC, cv2.INTER_AREA, cv2.INTER_LANCZOS4.
             Default: cv2.INTER_LINEAR.
         p (float): probability of applying the transform. Default: 1.
 
     Targets:
@@ -350,80 +429,88 @@
 
     Image types:
         uint8, float32
 
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS)
-    _size_len = 2
+
+    class InitSchema(BaseTransformInitSchema):
+        interpolation: InterpolationType = cv2.INTER_LINEAR
+        p: ProbabilityType = 1
+        min_max_height: OnePlusIntRangeType
+        w2h_ratio: Annotated[float, Field(gt=0, description="Aspect ratio of crop.")]
+        width: Optional[int] = None
+        height: Optional[int] = None
+        size: Optional[ScaleIntType] = None
+
+        @model_validator(mode="after")
+        def process(self) -> Self:
+            if isinstance(self.size, int):
+                if isinstance(self.width, int):
+                    self.size = (self.size, self.width)
+                    warn(
+                        "Initializing with 'size' as an integer and a separate 'width' is deprecated. "
+                        "Please use a tuple (height, width) for the 'size' argument.",
+                        DeprecationWarning,
+                        stacklevel=2,
+                    )
+                else:
+                    msg = "If size is an integer, width as integer must be specified."
+                    raise TypeError(msg)
+
+            if self.size is None:
+                if self.height is None or self.width is None:
+                    message = "If 'size' is not provided, both 'height' and 'width' must be specified."
+                    raise ValueError(message)
+                self.size = (self.height, self.width)
+                warn(
+                    "Initializing with 'height' and 'width' is deprecated. "
+                    "Please use a tuple (height, width) for the 'size' argument.",
+                    DeprecationWarning,
+                    stacklevel=2,
+                )
+
+            return self
 
     def __init__(
         self,
         min_max_height: Tuple[int, int],
         # NOTE @zetyquickly: when (width, height) are deprecated, make 'size' non optional
-        size: Optional[Union[int, Tuple[int, int]]] = None,
+        size: Optional[ScaleIntType] = None,
         width: Optional[int] = None,
         height: Optional[int] = None,
         *,
         w2h_ratio: float = 1.0,
         interpolation: int = cv2.INTER_LINEAR,
         always_apply: bool = False,
         p: float = 1.0,
     ):
-        if isinstance(size, tuple):
-            if len(size) != self._size_len:
-                message = "Size must be a tuple of two integers (height, width)."
-                raise ValueError(message)
-            height, width = size
-        elif size is None:
-            if height is None or width is None:
-                message = "If 'size' is not provided, both 'height' and 'width' must be specified."
-                raise ValueError(message)
-            size = (height, width)
-            warn(
-                "Initializing with 'height' and 'width' is deprecated. "
-                "Please use a tuple (height, width) for the 'size' argument.",
-                DeprecationWarning,
-                stacklevel=2,
-            )
-        else:
-            if width is None:
-                message = "When 'size' is an integer, 'width' must be provided."
-                raise ValueError(message)
-            height = size
-            warn(
-                "Initializing with 'size' as an integer and a separate 'width' is deprecated. "
-                "Please use a tuple (height, width) for the 'size' argument.",
-                DeprecationWarning,
-                stacklevel=2,
-            )
-
-        super().__init__(height=height, width=width, interpolation=interpolation, always_apply=always_apply, p=p)
-
+        super().__init__(size=cast(Tuple[int, int], size), interpolation=interpolation, always_apply=always_apply, p=p)
         self.min_max_height = min_max_height
         self.w2h_ratio = w2h_ratio
 
     def get_params(self) -> Dict[str, Union[int, float]]:
-        crop_height = random.randint(self.min_max_height[0], self.min_max_height[1])
+        crop_height = random_utils.randint(self.min_max_height[0], self.min_max_height[1])
         return {
             "h_start": random.random(),
             "w_start": random.random(),
             "crop_height": crop_height,
             "crop_width": int(crop_height * self.w2h_ratio),
         }
 
-    def get_transform_init_args_names(self) -> Tuple[str, str, str, str, str]:
-        return "min_max_height", "height", "width", "w2h_ratio", "interpolation"
+    def get_transform_init_args_names(self) -> Tuple[str, ...]:
+        return "min_max_height", "size", "w2h_ratio", "interpolation"
 
 
 class RandomResizedCrop(_BaseRandomSizedCrop):
     """Torchvision's variant of crop a random part of the input and rescale it to some size.
 
     Args:
-        size (tuple[int]): target size for the output image, i.e. (height, width) after crop and resize
+        size (int, int): target size for the output image, i.e. (height, width) after crop and resize
         scale ((float, float)): range of size of the origin size cropped
         ratio ((float, float)): range of aspect ratio of the origin aspect ratio cropped
         interpolation (OpenCV flag): flag that is used to specify the interpolation algorithm. Should be one of:
             cv2.INTER_NEAREST, cv2.INTER_LINEAR, cv2.INTER_CUBIC, cv2.INTER_AREA, cv2.INTER_LANCZOS4.
             Default: cv2.INTER_LINEAR.
         p (float): probability of applying the transform. Default: 1.
 
@@ -432,122 +519,132 @@
 
     Image types:
         uint8, float32
 
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS)
-    _size_len = 2
+
+    class InitSchema(BaseTransformInitSchema):
+        scale: ZeroOneRangeType = (0.08, 1.0)
+        ratio: NonNegativeFloatRangeType = (0.75, 1.3333333333333333)
+        width: Optional[int] = None
+        height: Optional[int] = None
+        size: Optional[ScaleIntType] = None
+        p: ProbabilityType = 1
+        interpolation: InterpolationType = cv2.INTER_LINEAR
+
+        @model_validator(mode="after")
+        def process(self) -> Self:
+            if isinstance(self.size, int):
+                if isinstance(self.width, int):
+                    self.size = (self.size, self.width)
+                    warn(
+                        "Initializing with 'size' as an integer and a separate 'width' is deprecated. "
+                        "Please use a tuple (height, width) for the 'size' argument.",
+                        DeprecationWarning,
+                        stacklevel=2,
+                    )
+                else:
+                    msg = "If size is an integer, width as integer must be specified."
+                    raise TypeError(msg)
+
+            if self.size is None:
+                if self.height is None or self.width is None:
+                    message = "If 'size' is not provided, both 'height' and 'width' must be specified."
+                    raise ValueError(message)
+                self.size = (self.height, self.width)
+                warn(
+                    "Initializing with 'height' and 'width' is deprecated. "
+                    "Please use a tuple (height, width) for the 'size' argument.",
+                    DeprecationWarning,
+                    stacklevel=2,
+                )
+
+            return self
 
     def __init__(
         self,
         # NOTE @zetyquickly: when (width, height) are deprecated, make 'size' non optional
-        size: Optional[Union[int, Tuple[int, int]]] = None,
+        size: Optional[ScaleIntType] = None,
         width: Optional[int] = None,
         height: Optional[int] = None,
         *,
         scale: Tuple[float, float] = (0.08, 1.0),
         ratio: Tuple[float, float] = (0.75, 1.3333333333333333),
         interpolation: int = cv2.INTER_LINEAR,
         always_apply: bool = False,
         p: float = 1.0,
     ):
-        if isinstance(size, tuple):
-            if len(size) != self._size_len:
-                message = "Size must be a tuple of two integers (height, width)."
-                raise ValueError(message)
-            height, width = size
-        elif size is None:
-            if height is None or width is None:
-                message = "If 'size' is not provided, both 'height' and 'width' must be specified."
-                raise ValueError(message)
-            size = (height, width)
-            warn(
-                "Initializing with 'height' and 'width' is deprecated. "
-                "Please use a tuple (height, width) for the 'size' argument.",
-                DeprecationWarning,
-                stacklevel=2,
-            )
-        else:
-            if width is None:
-                message = "When 'size' is an integer, 'width' must be provided."
-                raise ValueError(message)
-            height = size
-            warn(
-                "Initializing with 'size' as an integer and a separate 'width' is deprecated. "
-                "Please use a tuple (height, width) for the 'size' argument.",
-                DeprecationWarning,
-                stacklevel=2,
-            )
-
-        super().__init__(height=height, width=width, interpolation=interpolation, always_apply=always_apply, p=p)
+        super().__init__(size=cast(Tuple[int, int], size), interpolation=interpolation, always_apply=always_apply, p=p)
         self.scale = scale
         self.ratio = ratio
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, Union[int, float]]:
         img = params["image"]
-        area = img.shape[0] * img.shape[1]
+        img_height, img_width = img.shape[:2]
+        area = img_height * img_width
 
         for _ in range(10):
-            target_area = random.uniform(*self.scale) * area
+            target_area = random_utils.uniform(*self.scale) * area
             log_ratio = (math.log(self.ratio[0]), math.log(self.ratio[1]))
-            aspect_ratio = math.exp(random.uniform(*log_ratio))
+            aspect_ratio = math.exp(random_utils.uniform(*log_ratio))
 
             width = int(round(math.sqrt(target_area * aspect_ratio)))
             height = int(round(math.sqrt(target_area / aspect_ratio)))
 
-            if 0 < width <= img.shape[1] and 0 < height <= img.shape[0]:
-                i = random.randint(0, img.shape[0] - height)
-                j = random.randint(0, img.shape[1] - width)
+            if 0 < width <= img_width and 0 < height <= img_height:
+                i = random.randint(0, img_height - height)
+                j = random.randint(0, img_width - width)
                 return {
                     "crop_height": height,
                     "crop_width": width,
-                    "h_start": i * 1.0 / (img.shape[0] - height + 1e-10),
-                    "w_start": j * 1.0 / (img.shape[1] - width + 1e-10),
+                    "h_start": i * 1.0 / (img_height - height + 1e-10),
+                    "w_start": j * 1.0 / (img_width - width + 1e-10),
                 }
 
         # Fallback to central crop
-        in_ratio = img.shape[1] / img.shape[0]
+        in_ratio = img_width / img_height
         if in_ratio < min(self.ratio):
-            width = img.shape[1]
-            height = int(round(width / min(self.ratio)))
+            width = img_width
+            height = int(round(img_width / min(self.ratio)))
         elif in_ratio > max(self.ratio):
-            height = img.shape[0]
+            height = img_height
             width = int(round(height * max(self.ratio)))
         else:  # whole image
-            width = img.shape[1]
-            height = img.shape[0]
-        i = (img.shape[0] - height) // 2
-        j = (img.shape[1] - width) // 2
+            width = img_width
+            height = img_height
+        i = (img_height - height) // 2
+        j = (img_width - width) // 2
         return {
             "crop_height": height,
             "crop_width": width,
-            "h_start": i * 1.0 / (img.shape[0] - height + 1e-10),
-            "w_start": j * 1.0 / (img.shape[1] - width + 1e-10),
+            "h_start": i * 1.0 / (img_height - height + 1e-10),
+            "w_start": j * 1.0 / (img_width - width + 1e-10),
         }
 
     def get_params(self) -> Dict[str, Any]:
         return {}
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["image"]
 
-    def get_transform_init_args_names(self) -> Tuple[str, str, str, str, str]:
-        return "height", "width", "scale", "ratio", "interpolation"
+    def get_transform_init_args_names(self) -> Tuple[str, ...]:
+        return "size", "scale", "ratio", "interpolation"
 
 
 class RandomCropNearBBox(DualTransform):
     """Crop bbox from image with random shift by x,y coordinates
 
     Args:
         max_part_shift (float, (float, float)): Max shift in `height` and `width` dimensions relative
             to `cropping_bbox` dimension.
-            If max_part_shift is a single float, the range will be (max_part_shift, max_part_shift).
-            Default (0.3, 0.3).
+            If max_part_shift is a single float, the range will be (0, max_part_shift).
+            Default (0, 0.3).
         cropping_bbox_key (str): Additional target key for cropping box. Default `cropping_bbox`.
         cropping_box_key (str): [Deprecated] Use `cropping_bbox_key` instead.
         p (float): probability of applying the transform. Default: 1.
 
     Targets:
         image, mask, bboxes, keypoints
 
@@ -559,43 +656,50 @@
         >>>              bbox_params=BboxParams("pascal_voc"))
         >>> result = aug(image=image, bboxes=bboxes, test_box=[0, 5, 10, 20])
 
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS)
 
+    class InitSchema(BaseTransformInitSchema):
+        max_part_shift: ZeroOneRangeType = (0, 0.3)
+        cropping_bbox_key: str = Field(default="cropping_bbox", description="Additional target key for cropping box.")
+        p: ProbabilityType = 1
+
     def __init__(
         self,
-        max_part_shift: ScaleFloatType = (0.3, 0.3),
+        max_part_shift: ScaleFloatType = (0, 0.3),
         cropping_bbox_key: str = "cropping_bbox",
         cropping_box_key: Optional[str] = None,  # Deprecated
         always_apply: bool = False,
         p: float = 1.0,
     ):
         super().__init__(always_apply, p)
-        self.max_part_shift = to_tuple(max_part_shift, low=max_part_shift)
-
         # Check for deprecated parameter and issue warning
         if cropping_box_key is not None:
             warn(
                 "The parameter 'cropping_box_key' is deprecated and will be removed in future versions. "
                 "Use 'cropping_bbox_key' instead.",
                 DeprecationWarning,
                 stacklevel=2,
             )
             # Ensure the new parameter is used even if the old one is passed
             cropping_bbox_key = cropping_box_key
 
+        self.max_part_shift = cast(Tuple[float, float], max_part_shift)
         self.cropping_bbox_key = cropping_bbox_key
 
-        if min(self.max_part_shift) < 0 or max(self.max_part_shift) > 1:
-            raise ValueError(f"Invalid max_part_shift. Got: {max_part_shift}")
-
     def apply(
-        self, img: np.ndarray, x_min: int = 0, x_max: int = 0, y_min: int = 0, y_max: int = 0, **params: Any
+        self,
+        img: np.ndarray,
+        x_min: int = 0,
+        x_max: int = 0,
+        y_min: int = 0,
+        y_max: int = 0,
+        **params: Any,
     ) -> np.ndarray:
         return F.clamping_crop(img, x_min, y_min, x_max, y_max)
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, int]:
         bbox = params[self.cropping_bbox_key]
         h_max_shift = round((bbox[3] - bbox[1]) * self.max_part_shift[0])
         w_max_shift = round((bbox[2] - bbox[0]) * self.max_part_shift[1])
@@ -644,14 +748,23 @@
     Image types:
         uint8, float32
 
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES)
 
+    class InitSchema(BaseTransformInitSchema):
+        erosion_rate: float = Field(
+            default=0.0,
+            ge=0.0,
+            le=1.0,
+            description="Erosion rate applied on input image height before crop.",
+        )
+        p: ProbabilityType = 1
+
     def __init__(self, erosion_rate: float = 0.0, always_apply: bool = False, p: float = 1.0):
         super().__init__(always_apply, p)
         self.erosion_rate = erosion_rate
 
     def apply(
         self,
         img: np.ndarray,
@@ -672,15 +785,18 @@
                 "h_start": random.random(),
                 "w_start": random.random(),
                 "crop_height": crop_height,
                 "crop_width": int(crop_height * img_w / img_h),
             }
         # get union of all bboxes
         x, y, x2, y2 = union_of_bboxes(
-            width=img_w, height=img_h, bboxes=params["bboxes"], erosion_rate=self.erosion_rate
+            width=img_w,
+            height=img_h,
+            bboxes=params["bboxes"],
+            erosion_rate=self.erosion_rate,
         )
         # find bigger region
         bx, by = x * random.random(), y * random.random()
         bx2, by2 = x2 + (1 - x2) * random.random(), y2 + (1 - y2) * random.random()
         bw, bh = bx2 - bx, by2 - by
         crop_height = img_h if bh >= 1.0 else int(img_h * bh)
         crop_width = img_w if bw >= 1.0 else int(img_w * bw)
@@ -725,14 +841,23 @@
     Image types:
         uint8, float32
 
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES)
 
+    class InitSchema(CropInitSchema):
+        erosion_rate: float = Field(
+            default=0.0,
+            ge=0.0,
+            le=1.0,
+            description="Erosion rate applied on input image height before crop.",
+        )
+        interpolation: InterpolationType = cv2.INTER_LINEAR
+
     def __init__(
         self,
         height: int,
         width: int,
         erosion_rate: float = 0.0,
         interpolation: int = cv2.INTER_LINEAR,
         always_apply: bool = False,
@@ -846,36 +971,65 @@
     Image types:
         any
 
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS)
 
+    class InitSchema(BaseTransformInitSchema):
+        px: Optional[Union[int, Tuple[int, int], Tuple[int, int, int, int]]] = Field(
+            default=None,
+            description="Number of pixels to crop (negative) or pad (positive).",
+        )
+        percent: Optional[Union[float, Tuple[float, float], Tuple[float, float, float, float]]] = Field(
+            default=None,
+            description="Fraction of image size to crop (negative) or pad (positive).",
+        )
+        pad_mode: BorderModeType = cv2.BORDER_CONSTANT
+        pad_cval: ColorType = Field(default=0, description="Padding value if pad_mode is BORDER_CONSTANT.")
+        pad_cval_mask: ColorType = Field(
+            default=0,
+            description="Padding value for masks if pad_mode is BORDER_CONSTANT.",
+        )
+        keep_size: bool = Field(
+            default=True,
+            description="Whether to resize the image back to the original size after cropping and padding.",
+        )
+        sample_independently: bool = Field(
+            default=True,
+            description="Whether to sample the crop/pad size independently for each side.",
+        )
+        interpolation: InterpolationType = cv2.INTER_LINEAR
+        p: ProbabilityType = 1
+
+        @model_validator(mode="after")
+        def check_px_percent(self) -> Self:
+            if self.px is None and self.percent is None:
+                msg = "px and percent are empty!"
+                raise ValueError(msg)
+            if self.px is not None and self.percent is not None:
+                msg = "Only px or percent may be set!"
+                raise ValueError(msg)
+            return self
+
     def __init__(
         self,
         px: Optional[Union[int, List[int]]] = None,
         percent: Optional[Union[float, List[float]]] = None,
         pad_mode: int = cv2.BORDER_CONSTANT,
-        pad_cval: Union[float, Sequence[float]] = 0,
-        pad_cval_mask: Union[float, Sequence[float]] = 0,
+        pad_cval: ColorType = 0,
+        pad_cval_mask: ColorType = 0,
         keep_size: bool = True,
         sample_independently: bool = True,
         interpolation: int = cv2.INTER_LINEAR,
         always_apply: bool = False,
         p: float = 1.0,
     ):
         super().__init__(always_apply, p)
 
-        if px is None and percent is None:
-            msg = "px and percent are empty!"
-            raise ValueError(msg)
-        if px is not None and percent is not None:
-            msg = "Only px or percent may be set!"
-            raise ValueError(msg)
-
         self.px = px
         self.percent = percent
 
         self.pad_mode = pad_mode
         self.pad_cval = pad_cval
         self.pad_cval_mask = pad_cval_mask
 
@@ -892,30 +1046,46 @@
         pad_value: float = 0,
         rows: int = 0,
         cols: int = 0,
         interpolation: int = cv2.INTER_LINEAR,
         **params: Any,
     ) -> np.ndarray:
         return F.crop_and_pad(
-            img, crop_params, pad_params, pad_value, rows, cols, interpolation, self.pad_mode, self.keep_size
+            img,
+            crop_params,
+            pad_params,
+            pad_value,
+            rows,
+            cols,
+            interpolation,
+            self.pad_mode,
+            self.keep_size,
         )
 
     def apply_to_mask(
         self,
         mask: np.ndarray,
         crop_params: Optional[Sequence[int]] = None,
         pad_params: Optional[Sequence[int]] = None,
         pad_value_mask: Optional[float] = None,
         rows: int = 0,
         cols: int = 0,
         interpolation: int = cv2.INTER_NEAREST,
         **params: Any,
     ) -> np.ndarray:
         return F.crop_and_pad(
-            mask, crop_params, pad_params, pad_value_mask, rows, cols, interpolation, self.pad_mode, self.keep_size
+            mask,
+            crop_params,
+            pad_params,
+            pad_value_mask,
+            rows,
+            cols,
+            interpolation,
+            self.pad_mode,
+            self.keep_size,
         )
 
     def apply_to_bbox(
         self,
         bbox: BoxInternalType,
         crop_params: Optional[Sequence[int]] = None,
         pad_params: Optional[Sequence[int]] = None,
@@ -935,15 +1105,22 @@
         rows: int = 0,
         cols: int = 0,
         result_rows: int = 0,
         result_cols: int = 0,
         **params: Any,
     ) -> KeypointInternalType:
         return F.crop_and_pad_keypoint(
-            keypoint, crop_params, pad_params, rows, cols, result_rows, result_cols, self.keep_size
+            keypoint,
+            crop_params,
+            pad_params,
+            rows,
+            cols,
+            result_rows,
+            result_cols,
+            self.keep_size,
         )
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["image"]
 
     @staticmethod
@@ -1111,14 +1288,51 @@
     Image types:
         uint8, float32
 
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS)
 
+    class InitSchema(BaseTransformInitSchema):
+        crop_left: float = Field(
+            default=0.1,
+            ge=0.0,
+            le=1.0,
+            description="Fraction of width to randomly crop from the left side.",
+        )
+        crop_right: float = Field(
+            default=0.1,
+            ge=0.0,
+            le=1.0,
+            description="Fraction of width to randomly crop from the right side.",
+        )
+        crop_top: float = Field(
+            default=0.1,
+            ge=0.0,
+            le=1.0,
+            description="Fraction of height to randomly crop from the top side.",
+        )
+        crop_bottom: float = Field(
+            default=0.1,
+            ge=0.0,
+            le=1.0,
+            description="Fraction of height to randomly crop from the bottom side.",
+        )
+        p: ProbabilityType = 1
+
+        @model_validator(mode="after")
+        def validate_crop_values(self) -> Self:
+            if self.crop_left + self.crop_right >= 1.0:
+                msg = "The sum of crop_left and crop_right must be less than 1."
+                raise ValueError(msg)
+            if self.crop_top + self.crop_bottom >= 1.0:
+                msg = "The sum of crop_top and crop_bottom must be less than 1."
+                raise ValueError(msg)
+            return self
+
     def __init__(
         self,
         crop_left: float = 0.1,
         crop_right: float = 0.1,
         crop_top: float = 0.1,
         crop_bottom: float = 0.1,
         always_apply: bool = False,
@@ -1128,32 +1342,50 @@
         self.crop_left = crop_left
         self.crop_right = crop_right
         self.crop_top = crop_top
         self.crop_bottom = crop_bottom
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, int]:
         img = params["image"]
-        x_min = random.randint(0, int(self.crop_left * img.shape[1]))
-        x_max = random.randint(max(x_min + 1, int((1 - self.crop_right) * img.shape[1])), img.shape[1])
-        y_min = random.randint(0, int(self.crop_top * img.shape[0]))
-        y_max = random.randint(max(y_min + 1, int((1 - self.crop_bottom) * img.shape[0])), img.shape[0])
+        x_min = random_utils.randint(0, int(self.crop_left * img.shape[1]))
+        x_max = random_utils.randint(max(x_min + 1, int((1 - self.crop_right) * img.shape[1])), img.shape[1])
+        y_min = random_utils.randint(0, int(self.crop_top * img.shape[0]))
+        y_max = random_utils.randint(max(y_min + 1, int((1 - self.crop_bottom) * img.shape[0])), img.shape[0])
         return {"x_min": x_min, "x_max": x_max, "y_min": y_min, "y_max": y_max}
 
     def apply(
-        self, img: np.ndarray, x_min: int = 0, x_max: int = 0, y_min: int = 0, y_max: int = 0, **params: Any
+        self,
+        img: np.ndarray,
+        x_min: int = 0,
+        x_max: int = 0,
+        y_min: int = 0,
+        y_max: int = 0,
+        **params: Any,
     ) -> np.ndarray:
         return F.clamping_crop(img, x_min, y_min, x_max, y_max)
 
     def apply_to_mask(
-        self, mask: np.ndarray, x_min: int = 0, x_max: int = 0, y_min: int = 0, y_max: int = 0, **params: Any
+        self,
+        mask: np.ndarray,
+        x_min: int = 0,
+        x_max: int = 0,
+        y_min: int = 0,
+        y_max: int = 0,
+        **params: Any,
     ) -> np.ndarray:
         return F.clamping_crop(mask, x_min, y_min, x_max, y_max)
 
     def apply_to_bbox(
-        self, bbox: BoxInternalType, x_min: int = 0, x_max: int = 0, y_min: int = 0, y_max: int = 0, **params: Any
+        self,
+        bbox: BoxInternalType,
+        x_min: int = 0,
+        x_max: int = 0,
+        y_min: int = 0,
+        y_max: int = 0,
+        **params: Any,
     ) -> BoxInternalType:
         rows, cols = params["rows"], params["cols"]
         return F.bbox_crop(bbox, x_min, y_min, x_max, y_max, rows, cols)
 
     def apply_to_keypoint(
         self,
         keypoint: KeypointInternalType,
```

### Comparing `albumentations-1.4.3/albumentations/augmentations/domain_adaptation.py` & `albumentations-1.4.4/albumentations/augmentations/domain_adaptation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import random
-from typing import Any, Callable, Dict, List, Literal, Optional, Sequence, Tuple
+from typing import Any, Callable, Dict, List, Literal, Optional, Sequence, Tuple, cast
 
 import cv2
 import numpy as np
+from pydantic import field_validator
 
 from albumentations.augmentations.domain_adaptation_functional import (
     adapt_pixel_distribution,
     apply_histogram,
     fourier_domain_adaptation,
 )
 from albumentations.augmentations.utils import (
     is_grayscale_image,
     is_multispectral_image,
     read_rgb_image,
 )
-from albumentations.core.transforms_interface import ImageOnlyTransform, to_tuple
+from albumentations.core.pydantic import NonNegativeFloatRangeType, ZeroOneRangeType
+from albumentations.core.transforms_interface import BaseTransformInitSchema, ImageOnlyTransform
 from albumentations.core.types import ScaleFloatType
 
 __all__ = [
     "HistogramMatching",
     "FDA",
     "PixelDistributionAdaptation",
 ]
@@ -67,14 +69,19 @@
         >>> import albumentations as A
         >>> image = np.random.randint(0, 256, [100, 100, 3], dtype=np.uint8)
         >>> target_image = np.random.randint(0, 256, [100, 100, 3], dtype=np.uint8)
         >>> aug = A.Compose([A.HistogramMatching([target_image], p=1, read_fn=lambda x: x)])
         >>> result = aug(image=image)
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        reference_images: Sequence[Any]
+        blend_ratio: ZeroOneRangeType = (0.5, 1.0)
+        read_fn: Callable[[Any], np.ndarray]
+
     def __init__(
         self,
         reference_images: Sequence[Any],
         blend_ratio: Tuple[float, float] = (0.5, 1.0),
         read_fn: Callable[[Any], np.ndarray] = read_rgb_image,
         always_apply: bool = False,
         p: float = 0.5,
@@ -153,33 +160,46 @@
 
     Note:
         FDA is a powerful tool for domain adaptation, particularly in unsupervised settings where annotated target
         domain samples are unavailable. It enables significant improvements in model generalization by aligning
         the low-level statistics of source and target images through a simple yet effective Fourier-based method.
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        reference_images: Sequence[Any]
+        read_fn: Callable[[Any], np.ndarray]
+        beta_limit: NonNegativeFloatRangeType = (0, 0.1)
+
+        @field_validator("beta_limit")
+        @classmethod
+        def check_ranges(cls, value: Tuple[float, float]) -> Tuple[float, float]:
+            bounds = 0, MAX_BETA_LIMIT
+            if not bounds[0] <= value[0] <= value[1] <= bounds[1]:
+                raise ValueError(f"Values should be in the range {bounds} got {value} ")
+            return value
+
     def __init__(
         self,
-        reference_images: Sequence[np.ndarray],
-        beta_limit: ScaleFloatType = 0.1,
+        reference_images: Sequence[Any],
+        beta_limit: ScaleFloatType = (0, 0.1),
         read_fn: Callable[[Any], np.ndarray] = read_rgb_image,
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply=always_apply, p=p)
         self.reference_images = reference_images
         self.read_fn = read_fn
-        if isinstance(beta_limit, float) and not 0 <= beta_limit <= MAX_BETA_LIMIT:
-            msg = "The beta_limit should be within [0, 0.5]."
-            raise ValueError(msg)
-
-        self.beta_limit = to_tuple(beta_limit, low=0)
+        self.beta_limit = cast(Tuple[float, float], beta_limit)
 
     def apply(
-        self, img: np.ndarray, target_image: Optional[np.ndarray] = None, beta: float = 0.1, **params: Any
+        self,
+        img: np.ndarray,
+        target_image: Optional[np.ndarray] = None,
+        beta: float = 0.1,
+        **params: Any,
     ) -> np.ndarray:
         return fourier_domain_adaptation(img, target_image, beta)
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, np.ndarray]:
         img = params["image"]
         target_img = self.read_fn(random.choice(self.reference_images))
         target_img = cv2.resize(target_img, dsize=(img.shape[1], img.shape[0]))
@@ -241,38 +261,41 @@
 
     Note:
         The PixelDistributionAdaptation transform is a novel way to perform domain adaptation at the pixel level,
         suitable for adjusting images across different conditions without complex modeling. It is effective
         for preparing images before more advanced processing or analysis.
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        reference_images: Sequence[Any]
+        blend_ratio: ZeroOneRangeType = (0.25, 1.0)
+        read_fn: Callable[[Any], np.ndarray]
+        transform_type: Literal["pca", "standard", "minmax"]
+
     def __init__(
         self,
         reference_images: Sequence[Any],
         blend_ratio: Tuple[float, float] = (0.25, 1.0),
         read_fn: Callable[[Any], np.ndarray] = read_rgb_image,
         transform_type: Literal["pca", "standard", "minmax"] = "pca",
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply=always_apply, p=p)
         self.reference_images = reference_images
         self.read_fn = read_fn
         self.blend_ratio = blend_ratio
-        expected_transformers = ("pca", "standard", "minmax")
-        if transform_type not in expected_transformers:
-            raise ValueError(f"Got unexpected transform_type {transform_type}. Expected one of {expected_transformers}")
         self.transform_type = transform_type
 
     @staticmethod
     def _validate_shape(img: np.ndarray) -> None:
         if is_grayscale_image(img) or is_multispectral_image(img):
             raise ValueError(
                 f"Unexpected image shape: expected 3 dimensions, got {len(img.shape)}."
-                f"Is it a grayscale or multispectral image? It's not supported for now."
+                f"Is it a grayscale or multispectral image? It's not supported for now.",
             )
 
     def ensure_uint8(self, img: np.ndarray) -> Tuple[np.ndarray, bool]:
         if img.dtype == np.float32:
             if img.min() < 0 or img.max() > 1:
                 message = (
                     "PixelDistributionAdaptation uses uint8 under the hood, so float32 should be converted,"
```

### Comparing `albumentations-1.4.3/albumentations/augmentations/domain_adaptation_functional.py` & `albumentations-1.4.4/albumentations/augmentations/domain_adaptation_functional.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,18 @@
         representation = self.source_transformer.transform(pixels)
         result = self.target_transformer.inverse_transform(representation)
         return self.reconstruct(result, height, width)
 
 
 @preserve_shape
 def adapt_pixel_distribution(
-    img: np.ndarray, ref: np.ndarray, transform_type: str = "pca", weight: float = 0.5
+    img: np.ndarray,
+    ref: np.ndarray,
+    transform_type: str = "pca",
+    weight: float = 0.5,
 ) -> np.ndarray:
     initial_type = img.dtype
     transformer = {"pca": PCA, "standard": StandardScaler, "minmax": MinMaxScaler}[transform_type]()
     adapter = DomainAdapter(transformer=transformer, ref_img=ref)
     result = adapter(img).astype("float32")
     return (img.astype("float32") * (1 - weight) + result * weight).astype(initial_type)
```

### Comparing `albumentations-1.4.3/albumentations/augmentations/dropout/coarse_dropout.py` & `albumentations-1.4.4/albumentations/augmentations/dropout/coarse_dropout.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import random
-from typing import Any, Dict, Iterable, List, Optional, Sequence, Tuple
+from typing import Any, Dict, Iterable, List, Optional, Sequence, Tuple, cast
 
 import numpy as np
+from pydantic import Field, model_validator
+from typing_extensions import Self
 
-from albumentations.core.transforms_interface import DualTransform
-from albumentations.core.types import KeypointType, ScalarType, Targets
+from albumentations.core.transforms_interface import BaseTransformInitSchema, DualTransform
+from albumentations.core.types import ColorType, KeypointType, ScalarType, Targets
 
 from .functional import cutout, keypoint_in_hole
 
 __all__ = ["CoarseDropout"]
 
 
 class CoarseDropout(DualTransform):
@@ -36,61 +38,75 @@
     Targets:
         image, mask, keypoints
 
     Image types:
         uint8, float32
 
     Reference:
-    |  https://arxiv.org/abs/1708.04552
-    |  https://github.com/uoguelph-mlrg/Cutout/blob/master/util/cutout.py
-    |  https://github.com/aleju/imgaug/blob/master/imgaug/augmenters/arithmetic.py
+        https://arxiv.org/abs/1708.04552
+        https://github.com/uoguelph-mlrg/Cutout/blob/master/util/cutout.py
+        https://github.com/aleju/imgaug/blob/master/imgaug/augmenters/arithmetic.py
 
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.KEYPOINTS)
 
+    class InitSchema(BaseTransformInitSchema):
+        max_holes: int = Field(default=8, ge=0, description="Maximum number of regions to zero out.")
+        max_height: ScalarType = Field(default=8, ge=0, description="Maximum height of the hole.")
+        max_width: ScalarType = Field(default=8, ge=0, description="Maximum width of the hole.")
+        min_holes: Optional[int] = Field(default=None, ge=0, description="Minimum number of regions to zero out.")
+        min_height: Optional[ScalarType] = Field(default=None, ge=0, description="Minimum height of the hole.")
+        min_width: Optional[ScalarType] = Field(default=None, ge=0, description="Minimum width of the hole.")
+        fill_value: ColorType = Field(default=0, description="Value for dropped pixels.")
+        mask_fill_value: Optional[ColorType] = Field(default=None, description="Fill value for dropped pixels in mask.")
+
+        @model_validator(mode="after")
+        def check_holes_and_dimensions(self) -> Self:
+            self.min_holes = self.min_holes if self.min_holes is not None else self.max_holes
+
+            self.min_height = self.min_height if self.min_height is not None else self.max_height
+            self.min_width = self.min_width if self.min_width is not None else self.max_width
+
+            if not 0 < self.min_height <= self.max_height:
+                raise ValueError(
+                    f"Invalid combination of min_height and max_height. Got: {[self.min_height, self.max_height]}",
+                )
+            if not 0 < self.min_width <= self.max_width:
+                raise ValueError(
+                    f"Invalid combination of min_width and max_width. Got: {[self.min_width, self.max_width]}",
+                )
+            if not 0 < self.min_holes <= self.max_holes:
+                raise ValueError(
+                    f"Invalid combination of min_holes and max_holes. Got: {[self.min_holes, self.max_holes]}",
+                )
+            return self
+
     def __init__(
         self,
         max_holes: int = 8,
-        max_height: int = 8,
-        max_width: int = 8,
+        max_height: ScalarType = 8,
+        max_width: ScalarType = 8,
         min_holes: Optional[int] = None,
-        min_height: Optional[int] = None,
-        min_width: Optional[int] = None,
-        fill_value: int = 0,
-        mask_fill_value: Optional[int] = None,
+        min_height: Optional[ScalarType] = None,
+        min_width: Optional[ScalarType] = None,
+        fill_value: ColorType = 0,
+        mask_fill_value: Optional[ColorType] = None,
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
+        self.min_holes = cast(int, min_holes)
         self.max_holes = max_holes
+        self.min_height = cast(ScalarType, min_height)
         self.max_height = max_height
+        self.min_width = cast(ScalarType, min_width)
         self.max_width = max_width
-        self.min_holes = min_holes if min_holes is not None else max_holes
-        self.min_height = min_height if min_height is not None else max_height
-        self.min_width = min_width if min_width is not None else max_width
         self.fill_value = fill_value
         self.mask_fill_value = mask_fill_value
-        if not 0 < self.min_holes <= self.max_holes:
-            raise ValueError(f"Invalid combination of min_holes and max_holes. Got: {[min_holes, max_holes]}")
-
-        self.check_range(self.max_height)
-        self.check_range(self.min_height)
-        self.check_range(self.max_width)
-        self.check_range(self.min_width)
-
-        if not 0 < self.min_height <= self.max_height:
-            raise ValueError(f"Invalid combination of min_height and max_height. Got: {[min_height, max_height]}")
-        if not 0 < self.min_width <= self.max_width:
-            raise ValueError(f"Invalid combination of min_width and max_width. Got: {[min_width, max_width]}")
-
-    @staticmethod
-    def check_range(dimension: ScalarType) -> None:
-        if isinstance(dimension, float) and not 0 <= dimension < 1.0:
-            raise ValueError(f"Invalid value {dimension}. If using floats, the value should be in the range [0.0, 1.0)")
 
     def apply(
         self,
         img: np.ndarray,
         fill_value: ScalarType = 0,
         holes: Iterable[Tuple[int, int, int, int]] = (),
         **params: Any,
@@ -116,39 +132,39 @@
         for _ in range(random.randint(self.min_holes, self.max_holes)):
             if all(
                 [
                     isinstance(self.min_height, int),
                     isinstance(self.min_width, int),
                     isinstance(self.max_height, int),
                     isinstance(self.max_width, int),
-                ]
+                ],
             ):
-                hole_height = random.randint(self.min_height, self.max_height)
-                hole_width = random.randint(self.min_width, self.max_width)
+                hole_height = random.randint(int(self.min_height), int(self.max_height))
+                hole_width = random.randint(int(self.min_width), int(self.max_width))
             elif all(
                 [
                     isinstance(self.min_height, float),
                     isinstance(self.min_width, float),
                     isinstance(self.max_height, float),
                     isinstance(self.max_width, float),
-                ]
+                ],
             ):
                 hole_height = int(height * random.uniform(self.min_height, self.max_height))
                 hole_width = int(width * random.uniform(self.min_width, self.max_width))
             else:
                 msg = "Min width, max width, \
                     min height and max height \
                     should all either be ints or floats. \
                     Got: {} respectively".format(
                     [
                         type(self.min_width),
                         type(self.max_width),
                         type(self.min_height),
                         type(self.max_height),
-                    ]
+                    ],
                 )
                 raise ValueError(msg)
 
             y1 = random.randint(0, height - hole_height)
             x1 = random.randint(0, width - hole_width)
             y2 = y1 + hole_height
             x2 = x1 + hole_width
@@ -157,15 +173,18 @@
         return {"holes": holes}
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["image"]
 
     def apply_to_keypoints(
-        self, keypoints: Sequence[KeypointType], holes: Iterable[Tuple[int, int, int, int]] = (), **params: Any
+        self,
+        keypoints: Sequence[KeypointType],
+        holes: Iterable[Tuple[int, int, int, int]] = (),
+        **params: Any,
     ) -> List[KeypointType]:
         return [keypoint for keypoint in keypoints if not any(keypoint_in_hole(keypoint, hole) for hole in holes)]
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return (
             "max_holes",
             "max_height",
```

### Comparing `albumentations-1.4.3/albumentations/augmentations/dropout/functional.py` & `albumentations-1.4.4/albumentations/augmentations/dropout/functional.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 TWO = 2
 
 __all__ = ["cutout", "channel_dropout", "keypoint_in_hole"]
 
 
 @preserve_shape
 def channel_dropout(
-    img: np.ndarray, channels_to_drop: Union[int, Tuple[int, ...], np.ndarray], fill_value: ColorType = 0
+    img: np.ndarray,
+    channels_to_drop: Union[int, Tuple[int, ...], np.ndarray],
+    fill_value: ColorType = 0,
 ) -> np.ndarray:
     if len(img.shape) == TWO or img.shape[2] == 1:
         msg = "Only one channel. ChannelDropout is not defined."
         raise NotImplementedError(msg)
 
     img = img.copy()
     img[..., channels_to_drop] = fill_value
```

### Comparing `albumentations-1.4.3/albumentations/augmentations/dropout/grid_dropout.py` & `albumentations-1.4.4/albumentations/augmentations/dropout/grid_dropout.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import random
 from typing import Any, Dict, Iterable, List, Optional, Tuple
 
 import numpy as np
+from pydantic import Field
 
-from albumentations.core.transforms_interface import DualTransform
-from albumentations.core.types import ScalarType, Targets
+from albumentations.core.transforms_interface import BaseTransformInitSchema, DualTransform
+from albumentations.core.types import ColorType, ScalarType, Targets
 
 from . import functional as F
 
 __all__ = ["GridDropout"]
 
 TWO = 2
 
@@ -39,32 +40,44 @@
 
     Targets:
         image, mask
 
     Image types:
         uint8, float32
 
-    References:
+    Reference:
         https://arxiv.org/abs/2001.04086
 
     """
 
     _targets = (Targets.IMAGE, Targets.MASK)
 
+    class InitSchema(BaseTransformInitSchema):
+        ratio: float = Field(description="The ratio of the mask holes to the unit_size.", ge=0, le=1)
+        unit_size_min: Optional[int] = Field(None, description="Minimum size of the grid unit.", ge=2)
+        unit_size_max: Optional[int] = Field(None, description="Maximum size of the grid unit.", ge=2)
+        holes_number_x: Optional[int] = Field(None, description="The number of grid units in x direction.", ge=1)
+        holes_number_y: Optional[int] = Field(None, description="The number of grid units in y direction.", ge=1)
+        shift_x: int = Field(0, description="Offsets of the grid start in x direction.", ge=0)
+        shift_y: int = Field(0, description="Offsets of the grid start in y direction.", ge=0)
+        random_offset: bool = Field(False, description="Whether to offset the grid randomly.")
+        fill_value: Optional[ColorType] = Field(0, description="Value for the dropped pixels.")
+        mask_fill_value: Optional[ColorType] = Field(None, description="Value for the dropped pixels in mask.")
+
     def __init__(
         self,
         ratio: float = 0.5,
         unit_size_min: Optional[int] = None,
         unit_size_max: Optional[int] = None,
         holes_number_x: Optional[int] = None,
         holes_number_y: Optional[int] = None,
         shift_x: int = 0,
         shift_y: int = 0,
         random_offset: bool = False,
-        fill_value: int = 0,
+        fill_value: float = 0,
         mask_fill_value: Optional[ScalarType] = None,
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
         self.ratio = ratio
         self.unit_size_min = unit_size_min
@@ -72,23 +85,23 @@
         self.holes_number_x = holes_number_x
         self.holes_number_y = holes_number_y
         self.shift_x = shift_x
         self.shift_y = shift_y
         self.random_offset = random_offset
         self.fill_value = fill_value
         self.mask_fill_value = mask_fill_value
-        if not 0 < self.ratio <= 1:
-            msg = "ratio must be between 0 and 1."
-            raise ValueError(msg)
 
     def apply(self, img: np.ndarray, holes: Iterable[Tuple[int, int, int, int]] = (), **params: Any) -> np.ndarray:
         return F.cutout(img, holes, self.fill_value)
 
     def apply_to_mask(
-        self, mask: np.ndarray, holes: Iterable[Tuple[int, int, int, int]] = (), **params: Any
+        self,
+        mask: np.ndarray,
+        holes: Iterable[Tuple[int, int, int, int]] = (),
+        **params: Any,
     ) -> np.ndarray:
         if self.mask_fill_value is None:
             return mask
 
         return F.cutout(mask, holes, self.mask_fill_value)
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, Any]:
@@ -142,15 +155,19 @@
         hole_width = int(unit_width * self.ratio)
         hole_height = int(unit_height * self.ratio)
         hole_width = min(max(hole_width, 1), unit_width - 1)
         hole_height = min(max(hole_height, 1), unit_height - 1)
         return hole_width, hole_height
 
     def _calculate_shifts(
-        self, unit_width: int, unit_height: int, hole_width: int, hole_height: int
+        self,
+        unit_width: int,
+        unit_height: int,
+        hole_width: int,
+        hole_height: int,
     ) -> Tuple[int, int]:
         """Calculates the shifts for the grid start."""
         if self.random_offset:
             shift_x = random.randint(0, unit_width - hole_width)
             shift_y = random.randint(0, unit_height - hole_height)
         else:
             shift_x = 0 if self.shift_x is None else min(max(0, self.shift_x), unit_width - hole_width)
```

### Comparing `albumentations-1.4.3/albumentations/augmentations/dropout/mask_dropout.py` & `albumentations-1.4.4/albumentations/augmentations/dropout/mask_dropout.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,55 +1,71 @@
 import random
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Union, cast
 
 import cv2
 import numpy as np
+from pydantic import Field
 from skimage.measure import label
+from typing_extensions import Literal
 
-from albumentations.core.transforms_interface import DualTransform, to_tuple
-from albumentations.core.types import ScalarType, Targets
+from albumentations.core.pydantic import OnePlusIntRangeType
+from albumentations.core.transforms_interface import BaseTransformInitSchema, DualTransform
+from albumentations.core.types import ScalarType, ScaleIntType, Targets
 
 __all__ = ["MaskDropout"]
 
 
 class MaskDropout(DualTransform):
     """Image & mask augmentation that zero out mask and image regions corresponding
     to randomly chosen object instance from mask.
 
     Mask must be single-channel image, zero values treated as background.
     Image can be any number of channels.
 
-    Inspired by https://www.kaggle.com/c/severstal-steel-defect-detection/discussion/114254
-
     Args:
         max_objects: Maximum number of labels that can be zeroed out. Can be tuple, in this case it's [min, max]
         image_fill_value: Fill value to use when filling image.
             Can be 'inpaint' to apply inpainting (works only  for 3-channel images)
         mask_fill_value: Fill value to use when filling mask.
 
     Targets:
         image, mask
 
     Image types:
         uint8, float32
 
+    Reference:
+        https://www.kaggle.com/c/severstal-steel-defect-detection/discussion/114254
+
     """
 
     _targets = (Targets.IMAGE, Targets.MASK)
 
+    class InitSchema(BaseTransformInitSchema):
+        max_objects: OnePlusIntRangeType = (1, 1)
+
+        image_fill_value: Union[float, Literal["inpaint"]] = Field(
+            default=0,
+            description=(
+                "Fill value to use when filling image. "
+                "Can be 'inpaint' to apply inpainting (works only for 3-channel images)."
+            ),
+        )
+        mask_fill_value: float = Field(default=0, description="Fill value to use when filling mask.")
+
     def __init__(
         self,
-        max_objects: int = 1,
-        image_fill_value: Union[float, str] = 0,
+        max_objects: ScaleIntType = (1, 1),
+        image_fill_value: Union[float, Literal["inpaint"]] = 0,
         mask_fill_value: ScalarType = 0,
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
-        self.max_objects = to_tuple(max_objects, 1)
+        self.max_objects = cast(Tuple[int, int], max_objects)
         self.image_fill_value = image_fill_value
         self.mask_fill_value = mask_fill_value
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["mask"]
 
@@ -57,15 +73,15 @@
         mask = params["mask"]
 
         label_image, num_labels = label(mask, return_num=True)
 
         if num_labels == 0:
             dropout_mask = None
         else:
-            objects_to_drop = random.randint(int(self.max_objects[0]), int(self.max_objects[1]))
+            objects_to_drop = random.randint(self.max_objects[0], self.max_objects[1])
             objects_to_drop = min(num_labels, objects_to_drop)
 
             if objects_to_drop == num_labels:
                 dropout_mask = mask > 0
             else:
                 labels_index = random.sample(range(1, num_labels + 1), objects_to_drop)
                 dropout_mask = np.zeros((mask.shape[0], mask.shape[1]), dtype=bool)
```

### Comparing `albumentations-1.4.3/albumentations/augmentations/dropout/xy_masking.py` & `albumentations-1.4.4/albumentations/augmentations/dropout/xy_masking.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import random
-from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
+from typing import Any, Dict, List, Optional, Sequence, Tuple, cast
 
 import numpy as np
+from pydantic import Field, model_validator
+from typing_extensions import Self
 
-from albumentations.core.transforms_interface import DualTransform
+from albumentations import random_utils
+from albumentations.core.pydantic import NonNegativeIntRangeType
+from albumentations.core.transforms_interface import BaseTransformInitSchema, DualTransform
 from albumentations.core.types import ColorType, KeypointType, ScaleIntType, Targets
 
 from .functional import cutout, keypoint_in_hole
 
 __all__ = ["XYMasking"]
 
 
@@ -46,56 +50,52 @@
 
     Note: Either `max_x_length` or `max_y_length` or both must be defined.
 
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.KEYPOINTS)
 
+    class InitSchema(BaseTransformInitSchema):
+        num_masks_x: NonNegativeIntRangeType = 0
+        num_masks_y: NonNegativeIntRangeType = 0
+        mask_x_length: NonNegativeIntRangeType = 0
+        mask_y_length: NonNegativeIntRangeType = 0
+
+        fill_value: ColorType = Field(default=0, description="Value to fill image masks.")
+        mask_fill_value: ColorType = Field(default=0, description="Value to fill masks in the mask.")
+
+        @model_validator(mode="after")
+        def check_mask_length(self) -> Self:
+            if (
+                isinstance(self.mask_x_length, int)
+                and self.mask_x_length <= 0
+                and isinstance(self.mask_y_length, int)
+                and self.mask_y_length <= 0
+            ):
+                msg = "At least one of `mask_x_length` or `mask_y_length` Should be a positive number."
+                raise ValueError(msg)
+            return self
+
     def __init__(
         self,
         num_masks_x: ScaleIntType = 0,
         num_masks_y: ScaleIntType = 0,
         mask_x_length: ScaleIntType = 0,
         mask_y_length: ScaleIntType = 0,
         fill_value: ColorType = 0,
         mask_fill_value: ColorType = 0,
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
+        self.num_masks_x = cast(Tuple[int, int], num_masks_x)
+        self.num_masks_y = cast(Tuple[int, int], num_masks_y)
 
-        if (
-            isinstance(mask_x_length, (int, float))
-            and mask_x_length <= 0
-            and isinstance(mask_y_length, (int, float))
-            and mask_y_length <= 0
-        ):
-            msg = "At least one of `mask_x_length` or `mask_y_length` Should be a positive number."
-            raise ValueError(msg)
-
-        if isinstance(num_masks_x, int) and num_masks_x <= 0 and isinstance(num_masks_y, int) and num_masks_y <= 0:
-            msg = (
-                "At least one of `num_masks_x` or `num_masks_y` "
-                "should be a positive number or tuple of two positive numbers."
-            )
-            raise ValueError(msg)
-
-        if isinstance(num_masks_x, (tuple, list)) and min(num_masks_x) <= 0:
-            msg = "All values in `num_masks_x` should be non negative integers."
-            raise ValueError(msg)
-
-        if isinstance(num_masks_y, (tuple, list)) and min(num_masks_y) <= 0:
-            msg = "All values in `num_masks_y` should be non negative integers."
-            raise ValueError(msg)
-
-        self.num_masks_x = num_masks_x
-        self.num_masks_y = num_masks_y
-
-        self.mask_x_length = mask_x_length
-        self.mask_y_length = mask_y_length
+        self.mask_x_length = cast(Tuple[int, int], mask_x_length)
+        self.mask_y_length = cast(Tuple[int, int], mask_y_length)
         self.fill_value = fill_value
         self.mask_fill_value = mask_fill_value
 
     def apply(
         self,
         img: np.ndarray,
         masks_x: List[Tuple[int, int, int, int]],
@@ -112,30 +112,33 @@
         **params: Any,
     ) -> np.ndarray:
         if self.mask_fill_value is None:
             return mask
         return cutout(mask, masks_x + masks_y, self.mask_fill_value)
 
     def validate_mask_length(
-        self, mask_length: Optional[ScaleIntType], dimension_size: int, dimension_name: str
+        self,
+        mask_length: Optional[Tuple[int, int]],
+        dimension_size: int,
+        dimension_name: str,
     ) -> None:
         """Validate the mask length against the corresponding image dimension size.
 
         Args:
-            mask_length (Optional[Union[int, Tuple[int, int]]]): The length of the mask to be validated.
+            mask_length (Optional[Tuple[int, int]]): The length of the mask to be validated.
             dimension_size (int): The size of the image dimension (width or height)
                 against which to validate the mask length.
             dimension_name (str): The name of the dimension ('width' or 'height') for error messaging.
 
         """
         if mask_length is not None:
             if isinstance(mask_length, (tuple, list)):
                 if mask_length[0] < 0 or mask_length[1] > dimension_size:
                     raise ValueError(
-                        f"{dimension_name} range {mask_length} is out of valid range [0, {dimension_size}]"
+                        f"{dimension_name} range {mask_length} is out of valid range [0, {dimension_size}]",
                     )
             elif mask_length < 0 or mask_length > dimension_size:
                 raise ValueError(f"{dimension_name} {mask_length} exceeds image {dimension_name} {dimension_size}")
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, List[Tuple[int, int, int, int]]]:
         img = params["image"]
         height, width = img.shape[:2]
@@ -146,34 +149,33 @@
 
         masks_x = self.generate_masks(self.num_masks_x, width, height, self.mask_x_length, axis="x")
         masks_y = self.generate_masks(self.num_masks_y, width, height, self.mask_y_length, axis="y")
 
         return {"masks_x": masks_x, "masks_y": masks_y}
 
     @staticmethod
-    def generate_mask_size(mask_length: Union[ScaleIntType]) -> int:
-        if isinstance(mask_length, int):
-            return mask_length  # Use fixed size or adjust to dimension size
-
-        return random.randint(min(mask_length), max(mask_length))
+    def generate_mask_size(mask_length: Tuple[int, int]) -> int:
+        return random.randint(mask_length[0], mask_length[1])
 
     def generate_masks(
         self,
-        num_masks: ScaleIntType,
+        num_masks: Tuple[int, int],
         width: int,
         height: int,
-        max_length: Optional[ScaleIntType],
+        max_length: Optional[Tuple[int, int]],
         axis: str,
     ) -> List[Tuple[int, int, int, int]]:
         if max_length is None or max_length == 0 or isinstance(num_masks, (int, float)) and num_masks == 0:
             return []
 
         masks = []
 
-        num_masks_integer = num_masks if isinstance(num_masks, int) else random.randint(num_masks[0], num_masks[1])
+        num_masks_integer = (
+            num_masks if isinstance(num_masks, int) else random_utils.randint(num_masks[0], num_masks[1])
+        )
 
         for _ in range(num_masks_integer):
             length = self.generate_mask_size(max_length)
 
             if axis == "x":
                 x1 = random.randint(0, width - length)
                 y1 = 0
```

### Comparing `albumentations-1.4.3/albumentations/augmentations/functional.py` & `albumentations-1.4.4/albumentations/augmentations/functional.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from typing import Any, List, Optional, Sequence, Tuple, Union
+from collections import defaultdict
+from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 from warnings import warn
 
 import cv2
 import numpy as np
 import skimage
+from typing_extensions import Literal
 
 from albumentations import random_utils
 from albumentations.augmentations.utils import (
     MAX_VALUES_BY_DTYPE,
     _maybe_process_in_chunks,
     clip,
     clipped,
@@ -19,15 +21,14 @@
     preserve_shape,
 )
 from albumentations.core.types import (
     ColorType,
     ImageMode,
     ScalarType,
     SpatterMode,
-    image_modes,
 )
 
 __all__ = [
     "add_fog",
     "add_rain",
     "add_shadow",
     "add_gravel",
@@ -71,14 +72,16 @@
     "chromatic_aberration",
     "erode",
     "dilate",
 ]
 
 TWO = 2
 THREE = 3
+NUM_RGB_CHANNELS = 3
+GRAYSCALE_SHAPE_LENGTH = 2
 FOUR = 4
 EIGHT = 8
 THREE_SIXTY = 360
 
 
 def normalize_cv2(img: np.ndarray, mean: np.ndarray, denominator: np.ndarray) -> np.ndarray:
     if mean.shape and len(mean) != FOUR and mean.shape != img.shape:
@@ -97,30 +100,90 @@
 def normalize_numpy(img: np.ndarray, mean: np.ndarray, denominator: np.ndarray) -> np.ndarray:
     img = img.astype(np.float32)
     img -= mean
     img *= denominator
     return img
 
 
-def normalize(img: np.ndarray, mean: np.ndarray, std: np.ndarray, max_pixel_value: float = 255.0) -> np.ndarray:
-    mean = np.array(mean, dtype=np.float32)
-    mean *= max_pixel_value
-
-    std = np.array(std, dtype=np.float32)
-    std *= max_pixel_value
-
-    denominator = np.reciprocal(std, dtype=np.float32)
-
-    if img.ndim == THREE and img.shape[-1] == THREE:
-        return normalize_cv2(img, mean, denominator)
-    return normalize_numpy(img, mean, denominator)
+@preserve_shape
+def normalize(img: np.ndarray, mean: ColorType, std: ColorType, max_pixel_value: float = 255.0) -> np.ndarray:
+    mean_np = np.array(mean, dtype=np.float32)
+    mean_np *= max_pixel_value
+
+    std_np = np.array(std, dtype=np.float32)
+    std_np *= max_pixel_value
+
+    denominator = np.reciprocal(std_np, dtype=np.float32)
+
+    if is_rgb_image(img):
+        return normalize_cv2(img, mean_np, denominator)
+
+    return normalize_numpy(img, mean_np, denominator)
+
+
+@preserve_shape
+def normalize_per_image(
+    img: np.ndarray,
+    normalization: Literal["image", "image_per_channel", "min_max", "min_max_per_channel"],
+) -> np.ndarray:
+    """Apply per-image normalization based on the specified strategy.
+
+    Args:
+        img (np.ndarray): The image to be normalized, expected to be in HWC format.
+        normalization (str): The normalization strategy to apply. Options include:
+                             "image", "image_per_channel", "min_max", "min_max_per_channel".
+
+    Returns:
+        np.ndarray: The normalized image.
+
+    Reference:
+        https://github.com/ChristofHenkel/kaggle-landmark-2021-1st-place/blob/main/data/ch_ds_1.py
+    """
+    img = img.astype(np.float32)
+
+    if img.ndim == GRAYSCALE_SHAPE_LENGTH:
+        img = np.expand_dims(img, axis=-1)  # Ensure the image is at least 3D
+
+    if normalization == "image":
+        # Normalize the whole image based on its global mean and std
+        mean = img.mean()
+        std = img.std() + 1e-4  # Adding a small epsilon to avoid division by zero
+        normalized_img = (img - mean) / std
+        normalized_img = normalized_img.clip(-20, 20)  # Clipping outliers
+
+    elif normalization == "image_per_channel":
+        # Normalize the image per channel based on each channel's mean and std
+        pixel_mean = img.mean(axis=(0, 1))
+        pixel_std = img.std(axis=(0, 1)) + 1e-4
+        normalized_img = (img - pixel_mean[None, None, :]) / pixel_std[None, None, :]
+        normalized_img = normalized_img.clip(-20, 20)
+
+    elif normalization == "min_max":
+        # Apply min-max normalization to the whole image
+        img_min = img.min()
+        img_max = img.max()
+        normalized_img = (img - img_min) / (img_max - img_min)
+
+    elif normalization == "min_max_per_channel":
+        # Apply min-max normalization per channel
+        img_min = img.min(axis=(0, 1), keepdims=True)
+        img_max = img.max(axis=(0, 1), keepdims=True)
+        normalized_img = (img - img_min) / (img_max - img_min)
+
+    else:
+        raise ValueError(f"Unknown normalization method: {normalization}")
+
+    return normalized_img
 
 
 def _shift_hsv_uint8(
-    img: np.ndarray, hue_shift: np.ndarray, sat_shift: np.ndarray, val_shift: np.ndarray
+    img: np.ndarray,
+    hue_shift: np.ndarray,
+    sat_shift: np.ndarray,
+    val_shift: np.ndarray,
 ) -> np.ndarray:
     dtype = img.dtype
     img = cv2.cvtColor(img, cv2.COLOR_RGB2HSV)
     hue, sat, val = cv2.split(img)
 
     if hue_shift != 0:
         lut_hue = np.arange(0, 256, dtype=np.int16)
@@ -138,15 +201,18 @@
         val = cv2.LUT(val, lut_val)
 
     img = cv2.merge((hue, sat, val)).astype(dtype)
     return cv2.cvtColor(img, cv2.COLOR_HSV2RGB)
 
 
 def _shift_hsv_non_uint8(
-    img: np.ndarray, hue_shift: np.ndarray, sat_shift: np.ndarray, val_shift: np.ndarray
+    img: np.ndarray,
+    hue_shift: np.ndarray,
+    sat_shift: np.ndarray,
+    val_shift: np.ndarray,
 ) -> np.ndarray:
     dtype = img.dtype
     img = cv2.cvtColor(img, cv2.COLOR_RGB2HSV)
     hue, sat, val = cv2.split(img)
 
     if hue_shift != 0:
         hue = cv2.add(hue, hue_shift)
@@ -170,15 +236,15 @@
     is_gray = is_grayscale_image(img)
     if is_gray:
         if hue_shift != 0 or sat_shift != 0:
             hue_shift = 0
             sat_shift = 0
             warn(
                 "HueSaturationValue: hue_shift and sat_shift are not applicable to grayscale image. "
-                "Set them to 0 or use RGB image"
+                "Set them to 0 or use RGB image",
             )
         img = cv2.cvtColor(img, cv2.COLOR_GRAY2RGB)
 
     if img.dtype == np.uint8:
         img = _shift_hsv_uint8(img, hue_shift, sat_shift, val_shift)
     else:
         img = _shift_hsv_non_uint8(img, hue_shift, sat_shift, val_shift)
@@ -316,47 +382,50 @@
     for idx in range(i + 1, len(histogram)):
         _sum += histogram[idx]
         lut[idx] = clip(round(_sum * scale), np.dtype("uint8"), 255)
 
     return cv2.LUT(img, lut)
 
 
-def _check_preconditions(img: np.ndarray, mask: Optional[np.ndarray], mode: str, by_channels: bool) -> None:
+def _check_preconditions(img: np.ndarray, mask: Optional[np.ndarray], by_channels: bool) -> None:
     if img.dtype != np.uint8:
         msg = "Image must have uint8 channel type"
         raise TypeError(msg)
 
-    if mode not in image_modes:
-        raise ValueError(f"Unsupported equalization mode. Supports: {image_modes}. Got: {mode}")
-
     if mask is not None:
         if is_rgb_image(mask) and is_grayscale_image(img):
             raise ValueError(f"Wrong mask shape. Image shape: {img.shape}. Mask shape: {mask.shape}")
         if not by_channels and not is_grayscale_image(mask):
             msg = f"When by_channels=False only 1-channel mask supports. Mask shape: {mask.shape}"
             raise ValueError(msg)
 
 
 def _handle_mask(
-    mask: Optional[np.ndarray], img: np.ndarray, by_channels: bool, i: Optional[int] = None
+    mask: Optional[np.ndarray],
+    img: np.ndarray,
+    by_channels: bool,
+    i: Optional[int] = None,
 ) -> Optional[np.ndarray]:
     if mask is None:
         return None
     mask = mask.astype(np.uint8)
     if is_grayscale_image(mask) or i is None:
         return mask
 
     return mask[..., i]
 
 
 @preserve_channel_dim
 def equalize(
-    img: np.ndarray, mask: Optional[np.ndarray] = None, mode: ImageMode = "cv", by_channels: bool = True
+    img: np.ndarray,
+    mask: Optional[np.ndarray] = None,
+    mode: ImageMode = "cv",
+    by_channels: bool = True,
 ) -> np.ndarray:
-    _check_preconditions(img, mask, mode, by_channels)
+    _check_preconditions(img, mask, by_channels)
 
     function = _equalize_pil if mode == "pil" else _equalize_cv
 
     if is_grayscale_image(img):
         return function(img, _handle_mask(mask, img, by_channels))
 
     if not by_channels:
@@ -462,17 +531,17 @@
 
 @preserve_channel_dim
 def clahe(img: np.ndarray, clip_limit: float = 2.0, tile_grid_size: Tuple[int, int] = (8, 8)) -> np.ndarray:
     if img.dtype != np.uint8:
         msg = "clahe supports only uint8 inputs"
         raise TypeError(msg)
 
-    clahe_mat = cv2.createCLAHE(clipLimit=clip_limit, tileGridSize=tile_grid_size)
+    clahe_mat = cv2.createCLAHE(clipLimit=clip_limit, tileGridSize=[int(x) for x in tile_grid_size])
 
-    if len(img.shape) == TWO or img.shape[2] == 1:
+    if is_grayscale_image(img):
         return clahe_mat.apply(img)
 
     img = cv2.cvtColor(img, cv2.COLOR_RGB2LAB)
     img[:, :, 0] = clahe_mat.apply(img[:, :, 0])
     return cv2.cvtColor(img, cv2.COLOR_LAB2RGB)
 
 
@@ -736,26 +805,26 @@
         image_rgb = to_float(image_rgb, max_value=255)
 
     return image_rgb
 
 
 @ensure_contiguous
 @preserve_shape
-def add_shadow(img: np.ndarray, vertices_list: List[List[Tuple[int, int]]]) -> np.ndarray:
+def add_shadow(img: np.ndarray, vertices_list: List[np.ndarray]) -> np.ndarray:
     """Add shadows to the image.
 
-    From https://github.com/UjjwalSaxena/Automold--Road-Augmentation-Library
-
     Args:
         img (numpy.ndarray):
-        vertices_list (list):
+        vertices_list (list[numpy.ndarray]):
 
     Returns:
         numpy.ndarray:
 
+    Reference:
+        https://github.com/UjjwalSaxena/Automold--Road-Augmentation-Library
     """
     non_rgb_warning(img)
     input_dtype = img.dtype
     needs_float = False
 
     if input_dtype == np.float32:
         img = from_float(img, dtype=np.dtype("uint8"))
@@ -763,16 +832,15 @@
     elif input_dtype not in (np.uint8, np.float32):
         raise ValueError(f"Unexpected dtype {input_dtype} for RandomShadow augmentation")
 
     image_hls = cv2.cvtColor(img, cv2.COLOR_RGB2HLS)
     mask = np.zeros_like(img)
 
     # adding all shadow polygons on empty mask, single 255 denotes only red channel
-    for vertices in vertices_list:
-        cv2.fillPoly(mask, vertices, 255)
+    cv2.fillPoly(mask, vertices_list, 255)
 
     # if red channel is hot, image's "Lightness" channel's brightness is lowered
     red_max_value_ind = mask[:, :, 0] == MAX_VALUES_BY_DTYPE[np.dtype("uint8")]
     image_hls[:, :, 1][red_max_value_ind] = image_hls[:, :, 1][red_max_value_ind] * 0.5
 
     image_rgb = cv2.cvtColor(image_hls, cv2.COLOR_HLS2RGB)
 
@@ -844,15 +912,18 @@
 def gauss_noise(image: np.ndarray, gauss: np.ndarray) -> np.ndarray:
     image = image.astype("float32")
     return image + gauss
 
 
 @clipped
 def _brightness_contrast_adjust_non_uint(
-    img: np.ndarray, alpha: float = 1, beta: float = 0, beta_by_max: bool = False
+    img: np.ndarray,
+    alpha: float = 1,
+    beta: float = 0,
+    beta_by_max: bool = False,
 ) -> np.ndarray:
     dtype = img.dtype
     img = img.astype("float32")
 
     if alpha != 1:
         img *= alpha
     if beta != 0:
@@ -862,15 +933,18 @@
         else:
             img += beta * np.mean(img)
     return img
 
 
 @preserve_shape
 def _brightness_contrast_adjust_uint(
-    img: np.ndarray, alpha: float = 1, beta: float = 0, beta_by_max: bool = False
+    img: np.ndarray,
+    alpha: float = 1,
+    beta: float = 0,
+    beta_by_max: bool = False,
 ) -> np.ndarray:
     dtype = np.dtype("uint8")
 
     max_value = MAX_VALUES_BY_DTYPE[dtype]
 
     lut = np.arange(0, max_value + 1).astype("float32")
 
@@ -883,15 +957,18 @@
             lut += (alpha * beta) * np.mean(img)
 
     lut = np.clip(lut, 0, max_value).astype(dtype)
     return cv2.LUT(img, lut)
 
 
 def brightness_contrast_adjust(
-    img: np.ndarray, alpha: float = 1, beta: float = 0, beta_by_max: bool = False
+    img: np.ndarray,
+    alpha: float = 1,
+    beta: float = 0,
+    beta_by_max: bool = False,
 ) -> np.ndarray:
     if img.dtype == np.uint8:
         return _brightness_contrast_adjust_uint(img, alpha, beta, beta_by_max)
 
     return _brightness_contrast_adjust_non_uint(img, alpha, beta, beta_by_max)
 
 
@@ -950,15 +1027,18 @@
 
 def gray_to_rgb(img: np.ndarray) -> np.ndarray:
     return cv2.cvtColor(img, cv2.COLOR_GRAY2RGB)
 
 
 @preserve_shape
 def downscale(
-    img: np.ndarray, scale: float, down_interpolation: int = cv2.INTER_AREA, up_interpolation: int = cv2.INTER_LINEAR
+    img: np.ndarray,
+    scale: float,
+    down_interpolation: int = cv2.INTER_AREA,
+    up_interpolation: int = cv2.INTER_LINEAR,
 ) -> np.ndarray:
     height, width = img.shape[:2]
 
     need_cast = (
         up_interpolation != cv2.INTER_NEAREST or down_interpolation != cv2.INTER_NEAREST
     ) and img.dtype == np.uint8
     if need_cast:
@@ -991,33 +1071,36 @@
     return (img * max_value).astype(dtype)
 
 
 def noop(input_obj: Any, **params: Any) -> Any:
     return input_obj
 
 
-def swap_tiles_on_image(image: np.ndarray, tiles: np.ndarray) -> np.ndarray:
+def swap_tiles_on_image(image: np.ndarray, tiles: np.ndarray, mapping: Optional[List[int]] = None) -> np.ndarray:
     """Swap tiles on the image according to the new format.
 
     Args:
         image: Input image.
         tiles: Array of tiles with each tile as [start_y, start_x, end_y, end_x].
+        mapping: List of new tile indices.
 
     Returns:
         np.ndarray: Output image with tiles swapped according to the random shuffle.
     """
     # If no tiles are provided, return a copy of the original image
-    if tiles.size == 0:
+    if tiles.size == 0 or mapping is None:
         return image.copy()
 
     # Create a copy of the image to retain original for reference
     new_image = np.empty_like(image)
-    for start_y, start_x, end_y, end_x in tiles:
+    for num, new_index in enumerate(mapping):
+        start_y, start_x, end_y, end_x = tiles[new_index]
+        start_y_orig, start_x_orig, end_y_orig, end_x_orig = tiles[num]
         # Assign the corresponding tile from the original image to the new image
-        new_image[start_y:end_y, start_x:end_x] = image[start_y:end_y, start_x:end_x]
+        new_image[start_y:end_y, start_x:end_x] = image[start_y_orig:end_y_orig, start_x_orig:end_x_orig]
 
     return new_image
 
 
 @clipped
 def _multiply_uint8(img: np.ndarray, multiplier: np.ndarray) -> np.ndarray:
     img = img.astype(np.float32)
@@ -1268,15 +1351,19 @@
     img = cv2.cvtColor(img, cv2.COLOR_RGB2HSV)
     img[..., 0] = np.mod(img[..., 0] + factor * 360, 360)
     return cv2.cvtColor(img, cv2.COLOR_HSV2RGB)
 
 
 @preserve_shape
 def superpixels(
-    image: np.ndarray, n_segments: int, replace_samples: Sequence[bool], max_size: Optional[int], interpolation: int
+    image: np.ndarray,
+    n_segments: int,
+    replace_samples: Sequence[bool],
+    max_size: Optional[int],
+    interpolation: int,
 ) -> np.ndarray:
     if not np.any(replace_samples):
         return image
 
     orig_shape = image.shape
     if max_size is not None:
         size = max(image.shape[:2])
@@ -1284,15 +1371,18 @@
             scale = max_size / size
             height, width = image.shape[:2]
             new_height, new_width = int(height * scale), int(width * scale)
             resize_fn = _maybe_process_in_chunks(cv2.resize, dsize=(new_width, new_height), interpolation=interpolation)
             image = resize_fn(image)
 
     segments = skimage.segmentation.slic(
-        image, n_segments=n_segments, compactness=10, channel_axis=-1 if image.ndim > TWO else None
+        image,
+        n_segments=n_segments,
+        compactness=10,
+        channel_axis=-1 if image.ndim > TWO else None,
     )
 
     min_value = 0
     max_value = MAX_VALUES_BY_DTYPE[image.dtype]
     image = np.copy(image)
     if image.ndim == TWO:
         image = image.reshape(*image.shape, 1)
@@ -1317,30 +1407,38 @@
                 else:
                     value = mean_intensity
 
                 image_sp_c[segments == ridx] = value
 
     if orig_shape != image.shape:
         resize_fn = _maybe_process_in_chunks(
-            cv2.resize, dsize=(orig_shape[1], orig_shape[0]), interpolation=interpolation
+            cv2.resize,
+            dsize=(orig_shape[1], orig_shape[0]),
+            interpolation=interpolation,
         )
         return resize_fn(image)
 
     return image
 
 
 @clipped
+@preserve_shape
 def add_weighted(img1: np.ndarray, alpha: float, img2: np.ndarray, beta: float) -> np.ndarray:
-    return img1.astype(float) * alpha + img2.astype(float) * beta
+    img2 = img2.reshape(img1.shape).astype(img1.dtype)
+    return cv2.addWeighted(img1, alpha, img2, beta, 0)
 
 
 @clipped
 @preserve_shape
 def unsharp_mask(
-    image: np.ndarray, ksize: int, sigma: float = 0.0, alpha: float = 0.2, threshold: int = 10
+    image: np.ndarray,
+    ksize: int,
+    sigma: float = 0.0,
+    alpha: float = 0.2,
+    threshold: int = 10,
 ) -> np.ndarray:
     blur_fn = _maybe_process_in_chunks(cv2.GaussianBlur, ksize=(ksize, ksize), sigmaX=sigma)
 
     input_dtype = image.dtype
     if input_dtype == np.uint8:
         image = to_float(image)
     elif input_dtype not in (np.uint8, np.float32):
@@ -1402,41 +1500,125 @@
         img = img * non_mud + mud
     else:
         raise ValueError("Unsupported spatter mode: " + str(mode))
 
     return img * 255
 
 
-def split_uniform_grid(image_shape: Tuple[int, int], grid: Tuple[int, int]) -> np.ndarray:
+def almost_equal_intervals(n: int, parts: int) -> np.ndarray:
+    """Generates an array of nearly equal integer intervals that sum up to `n`.
+
+    This function divides the number `n` into `parts` nearly equal parts. It ensures that
+    the sum of all parts equals `n`, and the difference between any two parts is at most one.
+    This is useful for distributing a total amount into nearly equal discrete parts.
+
+    Args:
+        n (int): The total value to be split.
+        parts (int): The number of parts to split into.
+
+    Returns:
+        np.ndarray: An array of integers where each integer represents the size of a part.
+
+    Example:
+        >>> almost_equal_intervals(20, 3)
+        array([7, 7, 6])  # Splits 20 into three parts: 7, 7, and 6
+        >>> almost_equal_intervals(16, 4)
+        array([4, 4, 4, 4])  # Splits 16 into four equal parts
+    """
+    part_size, remainder = divmod(n, parts)
+    # Create an array with the base part size and adjust the first `remainder` parts by adding 1
+    return np.array([part_size + 1 if i < remainder else part_size for i in range(parts)])
+
+
+def generate_shuffled_splits(
+    size: int,
+    divisions: int,
+    random_state: Optional[np.random.RandomState] = None,
+) -> np.ndarray:
+    """Generate shuffled splits for a given dimension size and number of divisions.
+
+    Args:
+        size (int): Total size of the dimension (height or width).
+        divisions (int): Number of divisions (rows or columns).
+        random_state (Optional[np.random.RandomState]): Seed for the random number generator for reproducibility.
+
+    Returns:
+        np.ndarray: Cumulative edges of the shuffled intervals.
+    """
+    intervals = almost_equal_intervals(size, divisions)
+    intervals = random_utils.shuffle(intervals, random_state=random_state)
+    return np.insert(np.cumsum(intervals), 0, 0)
+
+
+def split_uniform_grid(
+    image_shape: Tuple[int, int],
+    grid: Tuple[int, int],
+    random_state: Optional[np.random.RandomState] = None,
+) -> np.ndarray:
     """Splits an image shape into a uniform grid specified by the grid dimensions.
 
     Args:
         image_shape (Tuple[int, int]): The shape of the image as (height, width).
         grid (Tuple[int, int]): The grid size as (rows, columns).
 
     Returns:
         np.ndarray: An array containing the tiles' coordinates in the format (start_y, start_x, end_y, end_x).
     """
-    height, width = image_shape
     n_rows, n_cols = grid
 
-    # Compute split points for the grid
-    height_splits = np.linspace(0, height, n_rows + 1, dtype=int)
-    width_splits = np.linspace(0, width, n_cols + 1, dtype=int)
+    height_splits = generate_shuffled_splits(image_shape[0], grid[0], random_state)
+    width_splits = generate_shuffled_splits(image_shape[1], grid[1], random_state)
 
     # Calculate tiles coordinates
     tiles = [
         (height_splits[i], width_splits[j], height_splits[i + 1], width_splits[j + 1])
         for i in range(n_rows)
         for j in range(n_cols)
     ]
 
     return np.array(tiles)
 
 
+def create_shape_groups(tiles: np.ndarray) -> Dict[Tuple[int, int], List[int]]:
+    """Groups tiles by their shape and stores the indices for each shape."""
+    shape_groups = defaultdict(list)
+    for index, (start_y, start_x, end_y, end_x) in enumerate(tiles):
+        shape = (end_y - start_y, end_x - start_x)
+        shape_groups[shape].append(index)
+    return shape_groups
+
+
+def shuffle_tiles_within_shape_groups(
+    shape_groups: Dict[Tuple[int, int], List[int]],
+    random_state: Optional[np.random.RandomState] = None,
+) -> List[int]:
+    """Shuffles indices within each group of similar shapes and creates a list where each
+    index points to the index of the tile it should be mapped to.
+
+    Args:
+        shape_groups (Dict[Tuple[int, int], List[int]]): Groups of tile indices categorized by shape.
+        random_state (Optional[np.random.RandomState]): Seed for the random number generator for reproducibility.
+
+    Returns:
+        List[int]: A list where each index is mapped to the new index of the tile after shuffling.
+    """
+    # Initialize the output list with the same size as the total number of tiles, filled with -1
+    num_tiles = sum(len(indices) for indices in shape_groups.values())
+    mapping = [-1] * num_tiles
+
+    # Prepare the random number generator
+
+    for indices in shape_groups.values():
+        shuffled_indices = random_utils.shuffle(indices.copy(), random_state=random_state)
+        for old, new in zip(indices, shuffled_indices):
+            mapping[old] = new
+
+    return mapping
+
+
 def chromatic_aberration(
     img: np.ndarray,
     primary_distortion_red: float,
     secondary_distortion_red: float,
     primary_distortion_blue: float,
     secondary_distortion_blue: float,
     interpolation: int,
```

### Comparing `albumentations-1.4.3/albumentations/augmentations/geometric/functional.py` & `albumentations-1.4.4/albumentations/augmentations/geometric/functional.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,30 +11,27 @@
     _maybe_process_in_chunks,
     angle_2pi_range,
     clipped,
     preserve_channel_dim,
     preserve_shape,
 )
 from albumentations.core.bbox_utils import denormalize_bbox, normalize_bbox
-from albumentations.core.types import BoxInternalType, ColorType, ImageColorType, KeypointInternalType
+from albumentations.core.types import BoxInternalType, ColorType, D4Type, KeypointInternalType
 
 __all__ = [
     "optical_distortion",
     "elastic_transform_approx",
     "grid_distortion",
     "pad",
     "pad_with_params",
     "bbox_rot90",
     "keypoint_rot90",
     "rotate",
     "bbox_rotate",
     "keypoint_rotate",
-    "shift_scale_rotate",
-    "keypoint_shift_scale_rotate",
-    "bbox_shift_scale_rotate",
     "elastic_transform",
     "resize",
     "scale",
     "keypoint_scale",
     "_func_max_size",
     "longest_max_size",
     "smallest_max_size",
@@ -64,19 +61,25 @@
     "keypoint_flip",
     "keypoint_hflip",
     "keypoint_transpose",
     "keypoint_vflip",
     "normalize_bbox",
     "denormalize_bbox",
     "vflip",
+    "d4",
+    "bbox_d4",
+    "keypoint_d4",
 ]
 
 TWO = 2
 THREE = 3
 
+ROT90_180_FACTOR = 2
+ROT90_270_FACTOR = 3
+
 
 def bbox_rot90(bbox: BoxInternalType, factor: int, rows: int, cols: int) -> BoxInternalType:
     """Rotates a bounding box by 90 degrees CCW (see np.rot90)
 
     Args:
         bbox: A bounding box tuple (x_min, y_min, x_max, y_max).
         factor: Number of CCW rotations. Must be in set {0, 1, 2, 3} See np.rot90.
@@ -89,24 +92,72 @@
     """
     if factor not in {0, 1, 2, 3}:
         msg = "Parameter n must be in set {0, 1, 2, 3}"
         raise ValueError(msg)
     x_min, y_min, x_max, y_max = bbox[:4]
     if factor == 1:
         bbox = y_min, 1 - x_max, y_max, 1 - x_min
-    elif factor == TWO:
+    elif factor == ROT90_180_FACTOR:
         bbox = 1 - x_max, 1 - y_max, 1 - x_min, 1 - y_min
-    elif factor == THREE:
+    elif factor == ROT90_270_FACTOR:
         bbox = 1 - y_max, x_min, 1 - y_min, x_max
     return bbox
 
 
+def bbox_d4(bbox: BoxInternalType, group_member: D4Type, rows: int, cols: int) -> BoxInternalType:
+    """Applies a `D_4` symmetry group transformation to a bounding box.
+
+    The function transforms a bounding box according to the specified group member from the `D_4` group.
+    These transformations include rotations and reflections, specified to work on an image's bounding box given
+    its dimensions.
+
+    Parameters:
+    - bbox (BoxInternalType): The bounding box to transform. This should be a structure specifying coordinates
+        like (xmin, ymin, xmax, ymax).
+    - group_member (D4Type): A string identifier for the `D_4` group transformation to apply.
+        Valid values are 'e', 'r90', 'r180', 'r270', 'v', 'hvt', 'h', 't'.
+    - rows (int): The number of rows in the image, used to adjust transformations that depend on image dimensions.
+    - cols (int): The number of columns in the image, used for the same purposes as rows.
+
+    Returns:
+    - BoxInternalType: The transformed bounding box.
+
+    Raises:
+    - ValueError: If an invalid group member is specified.
+
+    Examples:
+    - Applying a 90-degree rotation:
+      `bbox_d4((10, 20, 110, 120), 'r90', 100, 100)`
+      This would rotate the bounding box 90 degrees within a 100x100 image.
+    """
+    transformations = {
+        "e": lambda x: x,  # Identity transformation
+        "r90": lambda x: bbox_rot90(x, 1, rows, cols),  # Rotate 90 degrees
+        "r180": lambda x: bbox_rot90(x, 2, rows, cols),  # Rotate 180 degrees
+        "r270": lambda x: bbox_rot90(x, 3, rows, cols),  # Rotate 270 degrees
+        "v": lambda x: bbox_vflip(x, rows, cols),  # Vertical flip
+        "hvt": lambda x: bbox_transpose(bbox_rot90(x, 2, rows, cols), rows, cols),  # Reflect over anti-diagonal
+        "h": lambda x: bbox_hflip(x, rows, cols),  # Horizontal flip
+        "t": lambda x: bbox_transpose(x, rows, cols),  # Transpose (reflect over main diagonal)
+    }
+
+    # Execute the appropriate transformation
+    if group_member in transformations:
+        return transformations[group_member](bbox)
+
+    raise ValueError(f"Invalid group member: {group_member}")
+
+
 @angle_2pi_range
 def keypoint_rot90(
-    keypoint: KeypointInternalType, factor: int, rows: int, cols: int, **params: Any
+    keypoint: KeypointInternalType,
+    factor: int,
+    rows: int,
+    cols: int,
+    **params: Any,
 ) -> KeypointInternalType:
     """Rotates a keypoint by 90 degrees CCW (see np.rot90)
 
     Args:
         keypoint: A keypoint `(x, y, angle, scale)`.
         factor: Number of CCW rotations. Must be in range [0;3] See np.rot90.
         rows: Image height.
@@ -123,37 +174,93 @@
 
     if factor not in {0, 1, 2, 3}:
         msg = "Parameter n must be in set {0, 1, 2, 3}"
         raise ValueError(msg)
 
     if factor == 1:
         x, y, angle = y, (cols - 1) - x, angle - math.pi / 2
-    elif factor == TWO:
+    elif factor == ROT90_180_FACTOR:
         x, y, angle = (cols - 1) - x, (rows - 1) - y, angle - math.pi
-    elif factor == THREE:
+    elif factor == ROT90_270_FACTOR:
         x, y, angle = (rows - 1) - y, x, angle + math.pi / 2
 
     return x, y, angle, scale
 
 
+def keypoint_d4(
+    keypoint: KeypointInternalType,
+    group_member: D4Type,
+    rows: int,
+    cols: int,
+    **params: Any,
+) -> KeypointInternalType:
+    """Applies a `D_4` symmetry group transformation to a keypoint.
+
+    This function adjusts a keypoint's coordinates according to the specified `D_4` group transformation,
+    which includes rotations and reflections suitable for image processing tasks. These transformations account
+    for the dimensions of the image to ensure the keypoint remains within its boundaries.
+
+    Parameters:
+    - keypoint (KeypointInternalType): The keypoint to transform. T
+        his should be a structure or tuple specifying coordinates
+        like (x, y, [additional parameters]).
+    - group_member (D4Type): A string identifier for the `D_4` group transformation to apply.
+        Valid values are 'e', 'r90', 'r180', 'r270', 'v', 'hv', 'h', 't'.
+    - rows (int): The number of rows in the image.
+    - cols (int): The number of columns in the image.
+    - params (Any): Not used
+
+    Returns:
+    - KeypointInternalType: The transformed keypoint.
+
+    Raises:
+    - ValueError: If an invalid group member is specified, indicating that the specified transformation does not exist.
+
+    Examples:
+    - Rotating a keypoint by 90 degrees in a 100x100 image:
+      `keypoint_d4((50, 30), 'r90', 100, 100)`
+      This would move the keypoint from (50, 30) to (70, 50) assuming standard coordinate transformations.
+    """
+    transformations = {
+        "e": lambda x: x,  # Identity transformation
+        "r90": lambda x: keypoint_rot90(x, 1, rows, cols),  # Rotate 90 degrees
+        "r180": lambda x: keypoint_rot90(x, 2, rows, cols),  # Rotate 180 degrees
+        "r270": lambda x: keypoint_rot90(x, 3, rows, cols),  # Rotate 270 degrees
+        "v": lambda x: keypoint_vflip(x, rows, cols),  # Vertical flip
+        "hvt": lambda x: keypoint_transpose(keypoint_rot90(x, 2, rows, cols), rows, cols),  # Reflect over anti diagonal
+        "h": lambda x: keypoint_hflip(x, rows, cols),  # Horizontal flip
+        "t": lambda x: keypoint_transpose(x, rows, cols),  # Transpose (reflect over main diagonal)
+    }
+    # Execute the appropriate transformation
+    if group_member in transformations:
+        return transformations[group_member](keypoint)
+
+    raise ValueError(f"Invalid group member: {group_member}")
+
+
 @preserve_channel_dim
 def rotate(
     img: np.ndarray,
     angle: float,
     interpolation: int = cv2.INTER_LINEAR,
     border_mode: int = cv2.BORDER_REFLECT_101,
-    value: Optional[ImageColorType] = None,
+    value: Optional[ColorType] = None,
 ) -> np.ndarray:
     height, width = img.shape[:2]
     # for images we use additional shifts of (0.5, 0.5) as otherwise
     # we get an ugly black border for 90deg rotations
     matrix = cv2.getRotationMatrix2D((width / 2 - 0.5, height / 2 - 0.5), angle, 1.0)
 
     warp_fn = _maybe_process_in_chunks(
-        cv2.warpAffine, M=matrix, dsize=(width, height), flags=interpolation, borderMode=border_mode, borderValue=value
+        cv2.warpAffine,
+        M=matrix,
+        dsize=(width, height),
+        flags=interpolation,
+        borderMode=border_mode,
+        borderValue=value,
     )
     return warp_fn(img)
 
 
 def bbox_rotate(bbox: BoxInternalType, angle: float, method: str, rows: int, cols: int) -> BoxInternalType:
     """Rotates a bounding box by angle degrees.
 
@@ -194,15 +301,19 @@
     y_min, y_max = min(y_t), max(y_t)
 
     return x_min, y_min, x_max, y_max
 
 
 @angle_2pi_range
 def keypoint_rotate(
-    keypoint: KeypointInternalType, angle: float, rows: int, cols: int, **params: Any
+    keypoint: KeypointInternalType,
+    angle: float,
+    rows: int,
+    cols: int,
+    **params: Any,
 ) -> KeypointInternalType:
     """Rotate a keypoint by angle.
 
     Args:
         keypoint: A keypoint `(x, y, angle, scale)`.
         angle: Rotation angle.
         rows: Image height.
@@ -215,127 +326,23 @@
     center = (cols - 1) * 0.5, (rows - 1) * 0.5
     matrix = cv2.getRotationMatrix2D(center, angle, 1.0)
     x, y, a, s = keypoint[:4]
     x, y = cv2.transform(np.array([[[x, y]]]), matrix).squeeze()
     return x, y, a + math.radians(angle), s
 
 
-@preserve_channel_dim
-def shift_scale_rotate(
-    img: np.ndarray,
-    angle: float,
-    scale: float,
-    dx: int,
-    dy: int,
-    interpolation: int = cv2.INTER_LINEAR,
-    border_mode: int = cv2.BORDER_REFLECT_101,
-    value: Optional[Tuple[int, ...]] = None,
-) -> np.ndarray:
-    height, width = img.shape[:2]
-    # for images we use additional shifts of (0.5, 0.5) as otherwise
-    # we get an ugly black border for 90deg rotations
-    center = (width / 2 - 0.5, height / 2 - 0.5)
-    matrix = cv2.getRotationMatrix2D(center, angle, scale)
-    matrix[0, 2] += dx * width
-    matrix[1, 2] += dy * height
-
-    warp_affine_fn = _maybe_process_in_chunks(
-        cv2.warpAffine, M=matrix, dsize=(width, height), flags=interpolation, borderMode=border_mode, borderValue=value
-    )
-    return warp_affine_fn(img)
-
-
-@angle_2pi_range
-def keypoint_shift_scale_rotate(
-    keypoint: KeypointInternalType, angle: float, scale: float, dx: int, dy: int, rows: int, cols: int, **params: Any
-) -> KeypointInternalType:
-    (
-        x,
-        y,
-        a,
-        s,
-    ) = keypoint[:4]
-    height, width = rows, cols
-    center = (cols - 1) * 0.5, (rows - 1) * 0.5
-    matrix = cv2.getRotationMatrix2D(center, angle, scale)
-    matrix[0, 2] += dx * width
-    matrix[1, 2] += dy * height
-
-    x, y = cv2.transform(np.array([[[x, y]]]), matrix).squeeze()
-    angle = a + math.radians(angle)
-    scale *= s
-
-    return x, y, angle, scale
-
-
-def bbox_shift_scale_rotate(
-    bbox: BoxInternalType,
-    angle: float,
-    scale: float,
-    dx: int,
-    dy: int,
-    rotate_method: str,
-    rows: int,
-    cols: int,
-    **kwargs: Any,
-) -> BoxInternalType:
-    """Rotates, shifts and scales a bounding box. Rotation is made by angle degrees,
-    scaling is made by scale factor and shifting is made by dx and dy.
-
-
-    Args:
-        bbox (tuple): A bounding box `(x_min, y_min, x_max, y_max)`.
-        angle (int): Angle of rotation in degrees.
-        scale (int): Scale factor.
-        dx (int): Shift along x-axis in pixel units.
-        dy (int): Shift along y-axis in pixel units.
-        rotate_method(str): Rotation method used. Should be one of: "largest_box", "ellipse".
-            Default: "largest_box".
-        rows (int): Image rows.
-        cols (int): Image cols.
-
-    Returns:
-        A bounding box `(x_min, y_min, x_max, y_max)`.
-
-    """
-    height, width = rows, cols
-    center = (width / 2, height / 2)
-    if rotate_method == "ellipse":
-        x_min, y_min, x_max, y_max = bbox_rotate(bbox, angle, rotate_method, rows, cols)
-        matrix = cv2.getRotationMatrix2D(center, 0, scale)
-    else:
-        x_min, y_min, x_max, y_max = bbox[:4]
-        matrix = cv2.getRotationMatrix2D(center, angle, scale)
-    matrix[0, 2] += dx * width
-    matrix[1, 2] += dy * height
-    x = np.array([x_min, x_max, x_max, x_min])
-    y = np.array([y_min, y_min, y_max, y_max])
-    ones = np.ones(shape=(len(x)))
-    points_ones = np.vstack([x, y, ones]).transpose()
-    points_ones[:, 0] *= width
-    points_ones[:, 1] *= height
-    tr_points = matrix.dot(points_ones.T).T
-    tr_points[:, 0] /= width
-    tr_points[:, 1] /= height
-
-    x_min, x_max = min(tr_points[:, 0]), max(tr_points[:, 0])
-    y_min, y_max = min(tr_points[:, 1]), max(tr_points[:, 1])
-
-    return x_min, y_min, x_max, y_max
-
-
 @preserve_shape
 def elastic_transform(
     img: np.ndarray,
     alpha: float,
     sigma: float,
     alpha_affine: float,
     interpolation: int = cv2.INTER_LINEAR,
     border_mode: int = cv2.BORDER_REFLECT_101,
-    value: Optional[ImageColorType] = None,
+    value: Optional[ColorType] = None,
     random_state: Optional[np.random.RandomState] = None,
     approximate: bool = False,
     same_dxdy: bool = False,
 ) -> np.ndarray:
     """Elastic deformation of images as described in [Simard2003]_ (with modifications).
     Based on https://gist.github.com/ernestum/601cdf56d2b424757de5
 
@@ -358,20 +365,25 @@
             center_square + square_size,
             [center_square[0] + square_size, center_square[1] - square_size],
             center_square - square_size,
         ],
         dtype=np.float32,
     )
     pts2 = pts1 + random_utils.uniform(-alpha_affine, alpha_affine, size=pts1.shape, random_state=random_state).astype(
-        np.float32
+        np.float32,
     )
     matrix = cv2.getAffineTransform(pts1, pts2)
 
     warp_fn = _maybe_process_in_chunks(
-        cv2.warpAffine, M=matrix, dsize=(width, height), flags=interpolation, borderMode=border_mode, borderValue=value
+        cv2.warpAffine,
+        M=matrix,
+        dsize=(width, height),
+        flags=interpolation,
+        borderMode=border_mode,
+        borderValue=value,
     )
     img = warp_fn(img)
 
     if approximate:
         # Approximate computation smooth displacement map with a large enough kernel.
         # On large images (512+) this is approximately 2X times faster
         dx = random_utils.rand(height, width, random_state=random_state).astype(np.float32) * 2 - 1
@@ -382,31 +394,36 @@
             dy = dx
         else:
             dy = random_utils.rand(height, width, random_state=random_state).astype(np.float32) * 2 - 1
             cv2.GaussianBlur(dy, (17, 17), sigma, dst=dy)
             dy *= alpha
     else:
         dx = np.float32(
-            gaussian_filter((random_utils.rand(height, width, random_state=random_state) * 2 - 1), sigma) * alpha
+            gaussian_filter((random_utils.rand(height, width, random_state=random_state) * 2 - 1), sigma) * alpha,
         )
         if same_dxdy:
             # Speed up
             dy = dx
         else:
             dy = np.float32(
-                gaussian_filter((random_utils.rand(height, width, random_state=random_state) * 2 - 1), sigma) * alpha
+                gaussian_filter((random_utils.rand(height, width, random_state=random_state) * 2 - 1), sigma) * alpha,
             )
 
     x, y = np.meshgrid(np.arange(width), np.arange(height))
 
     map_x = np.float32(x + dx)
     map_y = np.float32(y + dy)
 
     remap_fn = _maybe_process_in_chunks(
-        cv2.remap, map1=map_x, map2=map_y, interpolation=interpolation, borderMode=border_mode, borderValue=value
+        cv2.remap,
+        map1=map_x,
+        map2=map_y,
+        interpolation=interpolation,
+        borderMode=border_mode,
+        borderValue=value,
     )
     return remap_fn(img)
 
 
 @preserve_channel_dim
 def resize(img: np.ndarray, height: int, width: int, interpolation: int = cv2.INTER_LINEAR) -> np.ndarray:
     img_height, img_width = img.shape[:2]
@@ -570,15 +587,20 @@
     output_shape: Sequence[int],
 ) -> np.ndarray:
     if _is_identity_matrix(matrix):
         return image
 
     dsize = int(np.round(output_shape[1])), int(np.round(output_shape[0]))
     warp_fn = _maybe_process_in_chunks(
-        cv2.warpAffine, M=matrix.params[:2], dsize=dsize, flags=interpolation, borderMode=mode, borderValue=cval
+        cv2.warpAffine,
+        M=matrix.params[:2],
+        dsize=dsize,
+        flags=interpolation,
+        borderMode=mode,
+        borderValue=cval,
     )
     return warp_fn(image)
 
 
 @angle_2pi_range
 def keypoint_affine(
     keypoint: KeypointInternalType,
@@ -609,15 +631,15 @@
     if rotate_method == "largest_box":
         points = np.array(
             [
                 [x_min, y_min],
                 [x_max, y_min],
                 [x_max, y_max],
                 [x_min, y_max],
-            ]
+            ],
         )
     elif rotate_method == "ellipse":
         w = (x_max - x_min) / 2
         h = (y_max - y_min) / 2
         data = np.arange(0, 360, dtype=np.float32)
         x = w * np.sin(np.radians(data)) + (w + x_min - 0.5)
         y = h * np.cos(np.radians(data)) + (h + y_min - 0.5)
@@ -657,15 +679,15 @@
     x1, y1, x2, y2 = denormalize_bbox(bbox, rows, cols)[:4]
     points = np.array(
         [
             [x1, y1, 1],
             [x2, y1, 1],
             [x2, y2, 1],
             [x1, y2, 1],
-        ]
+        ],
     )
     points = points @ matrix.T
     x1 = points[:, 0].min()
     x2 = points[:, 0].max()
     y1 = points[:, 1].min()
     y2 = points[:, 1].max()
 
@@ -712,20 +734,29 @@
     interpolation: int,
     mode: str,
     cval: float,
 ) -> np.ndarray:
     if matrix is None:
         return img
     return skimage.transform.warp(
-        img, matrix, order=interpolation, mode=mode, cval=cval, preserve_range=True, output_shape=img.shape
+        img,
+        matrix,
+        order=interpolation,
+        mode=mode,
+        cval=cval,
+        preserve_range=True,
+        output_shape=img.shape,
     )
 
 
 def to_distance_maps(
-    keypoints: Sequence[Tuple[float, float]], height: int, width: int, inverted: bool = False
+    keypoints: Sequence[Tuple[float, float]],
+    height: int,
+    width: int,
+    inverted: bool = False,
 ) -> np.ndarray:
     """Generate a ``(H,W,N)`` array of distance maps for ``N`` keypoints.
 
     The ``n``-th distance map contains at every location ``(y, x)`` the
     euclidean distance to the ``n``-th keypoint.
 
     This function can be used as a helper when augmenting keypoints with a
@@ -780,15 +811,18 @@
         return False, if_not_found_coords["x"], if_not_found_coords["y"]
 
     msg = "Expected if_not_found_coords to be None, tuple, list, or dict."
     raise ValueError(msg)
 
 
 def find_keypoint(
-    position: Tuple[int, int], distance_map: np.ndarray, threshold: Optional[float], inverted: bool
+    position: Tuple[int, int],
+    distance_map: np.ndarray,
+    threshold: Optional[float],
+    inverted: bool,
 ) -> Optional[Tuple[float, float]]:
     """Determine if a valid keypoint can be found at the given position."""
     y, x = position
     value = distance_map[y, x]
     if not inverted and threshold is not None and value >= threshold:
         return None
     if inverted and threshold is not None and value < threshold:
@@ -878,20 +912,84 @@
 
 
 def hflip_cv2(img: np.ndarray) -> np.ndarray:
     return cv2.flip(img, 1)
 
 
 @preserve_shape
+def d4(img: np.ndarray, group_member: D4Type) -> np.ndarray:
+    """Applies a `D_4` symmetry group transformation to an image array.
+
+    This function manipulates an image using transformations such as rotations and flips,
+    corresponding to the `D_4` dihedral group symmetry operations.
+    Each transformation is identified by a unique group member code.
+
+    Parameters:
+    - img (np.ndarray): The input image array to transform.
+    - group_member (D4Type): A string identifier indicating the specific transformation to apply. Valid codes include:
+      - 'e': Identity (no transformation).
+      - 'r90': Rotate 90 degrees counterclockwise.
+      - 'r180': Rotate 180 degrees.
+      - 'r270': Rotate 270 degrees counterclockwise.
+      - 'v': Vertical flip.
+      - 'hvt': Transpose over second diagonal
+      - 'h': Horizontal flip.
+      - 't': Transpose (reflect over the main diagonal).
+
+    Returns:
+    - np.ndarray: The transformed image array.
+
+    Raises:
+    - ValueError: If an invalid group member is specified.
+
+    Examples:
+    - Rotating an image by 90 degrees:
+      `transformed_image = d4(original_image, 'r90')`
+    - Applying a horizontal flip to an image:
+      `transformed_image = d4(original_image, 'h')`
+    """
+    transformations = {
+        "e": lambda x: x,  # Identity transformation
+        "r90": lambda x: rot90(x, 1),  # Rotate 90 degrees
+        "r180": lambda x: rot90(x, 2),  # Rotate 180 degrees
+        "r270": lambda x: rot90(x, 3),  # Rotate 270 degrees
+        "v": vflip,  # Vertical flip
+        "hvt": lambda x: transpose(rot90(x, 2)),  # Reflect over anti-diagonal
+        "h": hflip,  # Horizontal flip
+        "t": transpose,  # Transpose (reflect over main diagonal)
+    }
+
+    # Execute the appropriate transformation
+    if group_member in transformations:
+        return np.ascontiguousarray(transformations[group_member](img))
+
+    raise ValueError(f"Invalid group member: {group_member}")
+
+
+@preserve_shape
 def random_flip(img: np.ndarray, code: int) -> np.ndarray:
     return cv2.flip(img, code)
 
 
 def transpose(img: np.ndarray) -> np.ndarray:
-    return img.transpose(1, 0, 2) if len(img.shape) > TWO else img.transpose(1, 0)
+    """Transposes the first two dimensions of an array of any dimensionality.
+    Retains the order of any additional dimensions.
+
+    Args:
+        img (np.ndarray): Input array.
+
+    Returns:
+        np.ndarray: Transposed array.
+    """
+    # Generate the new axes order
+    new_axes = list(range(img.ndim))
+    new_axes[0], new_axes[1] = 1, 0  # Swap the first two dimensions
+
+    # Transpose the array using the new axes order
+    return img.transpose(new_axes)
 
 
 def rot90(img: np.ndarray, factor: int) -> np.ndarray:
     img = np.rot90(img, factor)
     return np.ascontiguousarray(img)
 
 
@@ -951,39 +1049,31 @@
         bbox = bbox_hflip(bbox, rows, cols)
         bbox = bbox_vflip(bbox, rows, cols)
     else:
         raise ValueError(f"Invalid d value {d}. Valid values are -1, 0 and 1")
     return bbox
 
 
-def bbox_transpose(bbox: KeypointInternalType, axis: int, rows: int, cols: int) -> KeypointInternalType:
+def bbox_transpose(bbox: KeypointInternalType, rows: int, cols: int) -> KeypointInternalType:
     """Transposes a bounding box along given axis.
 
     Args:
         bbox: A bounding box `(x_min, y_min, x_max, y_max)`.
-        axis: 0 - main axis, 1 - secondary axis.
         rows: Image rows.
         cols: Image cols.
 
     Returns:
         A bounding box tuple `(x_min, y_min, x_max, y_max)`.
 
     Raises:
         ValueError: If axis not equal to 0 or 1.
 
     """
     x_min, y_min, x_max, y_max = bbox[:4]
-    if axis not in {0, 1}:
-        msg = "Axis must be either 0 or 1."
-        raise ValueError(msg)
-    if axis == 0:
-        bbox = (y_min, x_min, y_max, x_max)
-    if axis == 1:
-        bbox = (1 - y_max, 1 - x_max, 1 - y_min, 1 - x_min)
-    return bbox
+    return (y_min, x_min, y_max, x_max)
 
 
 @angle_2pi_range
 def keypoint_vflip(keypoint: KeypointInternalType, rows: int, cols: int) -> KeypointInternalType:
     """Flip a keypoint vertically around the x-axis.
 
     Args:
@@ -1014,14 +1104,15 @@
 
     """
     x, y, angle, scale = keypoint[:4]
     angle = math.pi - angle
     return (cols - 1) - x, y, angle, scale
 
 
+@angle_2pi_range
 def keypoint_flip(keypoint: KeypointInternalType, d: int, rows: int, cols: int) -> KeypointInternalType:
     """Flip a keypoint either vertically, horizontally or both depending on the value of `d`.
 
     Args:
         keypoint: A keypoint `(x, y, angle, scale)`.
         d: Number of flip. Must be -1, 0 or 1:
             * 0 - vertical flip,
@@ -1045,38 +1136,47 @@
         keypoint = keypoint_hflip(keypoint, rows, cols)
         keypoint = keypoint_vflip(keypoint, rows, cols)
     else:
         raise ValueError(f"Invalid d value {d}. Valid values are -1, 0 and 1")
     return keypoint
 
 
-def keypoint_transpose(keypoint: KeypointInternalType) -> KeypointInternalType:
-    """Rotate a keypoint by angle.
+@angle_2pi_range
+def keypoint_transpose(keypoint: KeypointInternalType, rows: int, cols: int) -> KeypointInternalType:
+    """Transposes a keypoint along a specified axis: main diagonal (0) or secondary diagonal (1).
 
     Args:
         keypoint: A keypoint `(x, y, angle, scale)`.
+        rows: Total number of rows (height) in the image.
+        cols: Total number of columns (width) in the image.
 
     Returns:
-        A keypoint `(x, y, angle, scale)`.
+        A transformed keypoint `(x, y, angle, scale)`.
+
+    Raises:
+        ValueError: If axis is not 0 or 1.
 
     """
     x, y, angle, scale = keypoint[:4]
 
-    angle = np.pi - angle if angle <= np.pi else 3 * np.pi - angle
+    # Transpose over the main diagonal: swap x and y.
+    new_x, new_y = y, x
+    # Adjust angle to reflect the coordinate swap.
+    angle = np.pi / 2 - angle if angle <= np.pi else 3 * np.pi / 2 - angle
 
-    return y, x, angle, scale
+    return new_x, new_y, angle, scale
 
 
 @preserve_channel_dim
 def pad(
     img: np.ndarray,
     min_height: int,
     min_width: int,
     border_mode: int = cv2.BORDER_REFLECT_101,
-    value: Optional[ImageColorType] = None,
+    value: Optional[ColorType] = None,
 ) -> np.ndarray:
     height, width = img.shape[:2]
 
     if height < min_height:
         h_pad_top = int((min_height - height) / 2.0)
         h_pad_bottom = min_height - height - h_pad_top
     else:
@@ -1090,29 +1190,29 @@
         w_pad_left = 0
         w_pad_right = 0
 
     img = pad_with_params(img, h_pad_top, h_pad_bottom, w_pad_left, w_pad_right, border_mode, value)
 
     if img.shape[:2] != (max(min_height, height), max(min_width, width)):
         raise RuntimeError(
-            f"Invalid result shape. Got: {img.shape[:2]}. Expected: {(max(min_height, height), max(min_width, width))}"
+            f"Invalid result shape. Got: {img.shape[:2]}. Expected: {(max(min_height, height), max(min_width, width))}",
         )
 
     return img
 
 
 @preserve_channel_dim
 def pad_with_params(
     img: np.ndarray,
     h_pad_top: int,
     h_pad_bottom: int,
     w_pad_left: int,
     w_pad_right: int,
     border_mode: int = cv2.BORDER_REFLECT_101,
-    value: Optional[ImageColorType] = None,
+    value: Optional[ColorType] = None,
 ) -> np.ndarray:
     pad_fn = _maybe_process_in_chunks(
         cv2.copyMakeBorder,
         top=h_pad_top,
         bottom=h_pad_bottom,
         left=w_pad_left,
         right=w_pad_right,
@@ -1126,15 +1226,15 @@
 def optical_distortion(
     img: np.ndarray,
     k: int = 0,
     dx: int = 0,
     dy: int = 0,
     interpolation: int = cv2.INTER_LINEAR,
     border_mode: int = cv2.BORDER_REFLECT_101,
-    value: Optional[ImageColorType] = None,
+    value: Optional[ColorType] = None,
 ) -> np.ndarray:
     """Barrel / pincushion distortion. Unconventional augment.
 
     Reference:
         |  https://stackoverflow.com/questions/6199636/formulas-for-barrel-pincushion-distortion
         |  https://stackoverflow.com/questions/10364201/image-transformation-in-opencv
         |  https://stackoverflow.com/questions/2477774/correcting-fisheye-distortion-programmatically
@@ -1159,15 +1259,15 @@
 def grid_distortion(
     img: np.ndarray,
     num_steps: int = 10,
     xsteps: Tuple[()] = (),
     ysteps: Tuple[()] = (),
     interpolation: int = cv2.INTER_LINEAR,
     border_mode: int = cv2.BORDER_REFLECT_101,
-    value: Optional[ImageColorType] = None,
+    value: Optional[ColorType] = None,
 ) -> np.ndarray:
     """Perform a grid distortion of an input image.
 
     Reference:
         http://pythology.blogspot.sg/2014/03/interpolation-on-regular-distorted-grid.html
     """
     height, width = img.shape[:2]
@@ -1223,15 +1323,15 @@
 def elastic_transform_approx(
     img: np.ndarray,
     alpha: float,
     sigma: float,
     alpha_affine: float,
     interpolation: int = cv2.INTER_LINEAR,
     border_mode: int = cv2.BORDER_REFLECT_101,
-    value: Optional[ImageColorType] = None,
+    value: Optional[ColorType] = None,
     random_state: Optional[np.random.RandomState] = None,
 ) -> np.ndarray:
     """Elastic deformation of images as described in [Simard2003]_ (with modifications for speed).
     Based on https://gist.github.com/ernestum/601cdf56d2b424757de5
 
     .. [Simard2003] Simard, Steinkraus and Platt, "Best Practices for
          Convolutional Neural Networks applied to Visual Document Analysis", in
@@ -1252,15 +1352,15 @@
             center_square + square_size,
             [center_square[0] + square_size, center_square[1] - square_size],
             center_square - square_size,
         ],
         dtype=np.float32,
     )
     pts2 = pts1 + random_utils.uniform(-alpha_affine, alpha_affine, size=pts1.shape, random_state=random_state).astype(
-        np.float32
+        np.float32,
     )
     matrix = cv2.getAffineTransform(pts1, pts2)
 
     warp_fn = _maybe_process_in_chunks(
         cv2.warpAffine,
         M=matrix,
         dsize=(width, height),
```

### Comparing `albumentations-1.4.3/albumentations/augmentations/geometric/rotate.py` & `albumentations-1.4.4/albumentations/augmentations/geometric/rotate.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 import math
 import random
-from typing import Any, Dict, List, Optional, Tuple, Union, cast
+from typing import Any, Dict, List, Optional, Tuple, cast
 
 import cv2
 import numpy as np
+from pydantic import Field
+from typing_extensions import Literal
 
 from albumentations.augmentations.crops import functional as FCrops
-from albumentations.core.transforms_interface import DualTransform, to_tuple
-from albumentations.core.types import BoxInternalType, ColorType, KeypointInternalType, ScaleIntType, Targets
+from albumentations.core.pydantic import BorderModeType, InterpolationType, SymmetricRangeType
+from albumentations.core.transforms_interface import BaseTransformInitSchema, DualTransform
+from albumentations.core.types import (
+    BoxInternalType,
+    ColorType,
+    KeypointInternalType,
+    ScaleFloatType,
+    Targets,
+)
 
 from . import functional as F
 
 __all__ = ["Rotate", "RandomRotate90", "SafeRotate"]
 
 SMALL_NUMBER = 1e-10
 
@@ -49,14 +58,27 @@
     def apply_to_keypoint(self, keypoint: KeypointInternalType, factor: int = 0, **params: Any) -> BoxInternalType:
         return F.keypoint_rot90(keypoint, factor, **params)
 
     def get_transform_init_args_names(self) -> Tuple[()]:
         return ()
 
 
+class RotateInitSchema(BaseTransformInitSchema):
+    limit: SymmetricRangeType = (-90, 90)
+
+    interpolation: InterpolationType = cv2.INTER_LINEAR
+    border_mode: BorderModeType = cv2.BORDER_CONSTANT
+
+    value: Optional[ColorType] = Field(default=None, description="Padding value if border_mode is cv2.BORDER_CONSTANT.")
+    mask_value: Optional[ColorType] = Field(
+        default=None,
+        description="Padding value if border_mode is cv2.BORDER_CONSTANT applied for masks.",
+    )
+
+
 class Rotate(DualTransform):
     """Rotate the input by an angle selected randomly from the uniform distribution.
 
     Args:
         limit: range from which a random angle is picked. If limit is a single int
             an angle is picked from (-limit, limit). Default: (-90, 90)
         interpolation (OpenCV flag): flag that is used to specify the interpolation algorithm. Should be one of:
@@ -80,38 +102,42 @@
     Image types:
         uint8, float32
 
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS)
 
+    class InitSchema(RotateInitSchema):
+        rotate_method: Literal["largest_box", "ellipse"] = "largest_box"
+        crop_border: bool = Field(
+            default=False,
+            description="If True, makes a largest possible crop within the rotated image.",
+        )
+
     def __init__(
         self,
-        limit: ScaleIntType = 90,
+        limit: ScaleFloatType = 90,
         interpolation: int = cv2.INTER_LINEAR,
         border_mode: int = cv2.BORDER_REFLECT_101,
-        value: Optional[Union[int, float, Tuple[int, int], Tuple[float, float]]] = None,
-        mask_value: Optional[Union[int, float, Tuple[int, int], Tuple[float, float]]] = None,
-        rotate_method: str = "largest_box",
+        value: Optional[ColorType] = None,
+        mask_value: Optional[ColorType] = None,
+        rotate_method: Literal["largest_box", "ellipse"] = "largest_box",
         crop_border: bool = False,
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
-        self.limit = to_tuple(limit)
+        self.limit = cast(Tuple[float, float], limit)
         self.interpolation = interpolation
         self.border_mode = border_mode
         self.value = value
         self.mask_value = mask_value
         self.rotate_method = rotate_method
         self.crop_border = crop_border
 
-        if rotate_method not in ["largest_box", "ellipse"]:
-            raise ValueError(f"Rotation method {self.rotate_method} is not valid.")
-
     def apply(
         self,
         img: np.ndarray,
         angle: float = 0,
         interpolation: int = cv2.INTER_LINEAR,
         x_min: Optional[int] = None,
         x_max: Optional[int] = None,
@@ -170,54 +196,55 @@
     ) -> KeypointInternalType:
         keypoint_out = F.keypoint_rotate(keypoint, angle, rows, cols, **params)
         if self.crop_border and x_min is not None and x_max is not None and y_min is not None and y_max is not None:
             return FCrops.crop_keypoint_by_coords(keypoint_out, (x_min, y_min, x_max, y_max))
         return keypoint_out
 
     @staticmethod
-    def _rotated_rect_with_max_area(h: int, w: int, angle: float) -> Dict[str, int]:
+    def _rotated_rect_with_max_area(height: int, width: int, angle: float) -> Dict[str, int]:
         """Given a rectangle of size wxh that has been rotated by 'angle' (in
         degrees), computes the width and height of the largest possible
         axis-aligned rectangle (maximal area) within the rotated rectangle.
 
-        Code from: https://stackoverflow.com/questions/16702966/rotate-image-and-crop-out-black-borders
+        Reference:
+            https://stackoverflow.com/questions/16702966/rotate-image-and-crop-out-black-borders
         """
         angle = math.radians(angle)
-        width_is_longer = w >= h
-        side_long, side_short = (w, h) if width_is_longer else (h, w)
+        width_is_longer = width >= height
+        side_long, side_short = (width, height) if width_is_longer else (height, width)
 
         # since the solutions for angle, -angle and 180-angle are all the same,
         # it is sufficient to look at the first quadrant and the absolute values of sin,cos:
         sin_a, cos_a = abs(math.sin(angle)), abs(math.cos(angle))
         if side_short <= 2.0 * sin_a * cos_a * side_long or abs(sin_a - cos_a) < SMALL_NUMBER:
             # half constrained case: two crop corners touch the longer side,
             # the other two corners are on the mid-line parallel to the longer line
             x = 0.5 * side_short
             wr, hr = (x / sin_a, x / cos_a) if width_is_longer else (x / cos_a, x / sin_a)
         else:
             # fully constrained case: crop touches all 4 sides
             cos_2a = cos_a * cos_a - sin_a * sin_a
-            wr, hr = (w * cos_a - h * sin_a) / cos_2a, (h * cos_a - w * sin_a) / cos_2a
+            wr, hr = (width * cos_a - height * sin_a) / cos_2a, (height * cos_a - width * sin_a) / cos_2a
 
         return {
-            "x_min": max(0, int(w / 2 - wr / 2)),
-            "x_max": min(w, int(w / 2 + wr / 2)),
-            "y_min": max(0, int(h / 2 - hr / 2)),
-            "y_max": min(h, int(h / 2 + hr / 2)),
+            "x_min": max(0, int(width / 2 - wr / 2)),
+            "x_max": min(width, int(width / 2 + wr / 2)),
+            "y_min": max(0, int(height / 2 - hr / 2)),
+            "y_max": min(height, int(height / 2 + hr / 2)),
         }
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["image"]
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, Any]:
         out_params = {"angle": random.uniform(self.limit[0], self.limit[1])}
         if self.crop_border:
-            h, w = params["image"].shape[:2]
-            out_params.update(self._rotated_rect_with_max_area(h, w, out_params["angle"]))
+            height, width = params["image"].shape[:2]
+            out_params.update(self._rotated_rect_with_max_area(height, width, out_params["angle"]))
         return out_params
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return ("limit", "interpolation", "border_mode", "value", "mask_value", "rotate_method", "crop_border")
 
 
 class SafeRotate(DualTransform):
@@ -248,26 +275,29 @@
     Image types:
         uint8, float32
 
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS)
 
+    class InitSchema(RotateInitSchema):
+        pass
+
     def __init__(
         self,
-        limit: Union[float, Tuple[float, float]] = 90,
+        limit: ScaleFloatType = (-90, 90),
         interpolation: int = cv2.INTER_LINEAR,
         border_mode: int = cv2.BORDER_REFLECT_101,
         value: Optional[ColorType] = None,
         mask_value: Optional[ColorType] = None,
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
-        self.limit = to_tuple(limit)
+        self.limit = cast(Tuple[float, float], limit)
         self.interpolation = interpolation
         self.border_mode = border_mode
         self.value = value
         self.mask_value = mask_value
 
     def apply(self, img: np.ndarray, matrix: Optional[np.ndarray] = None, **params: Any) -> np.ndarray:
         return F.safe_rotate(img, matrix, cast(int, self.interpolation), self.value, self.border_mode)
```

### Comparing `albumentations-1.4.3/albumentations/augmentations/geometric/transforms.py` & `albumentations-1.4.4/albumentations/augmentations/geometric/transforms.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,43 @@
 import math
 import random
 from enum import Enum
-from typing import Any, Dict, List, Optional, Sequence, Tuple, Union, cast
+from typing import Any, Dict, List, Literal, Optional, Sequence, Tuple, Union, cast
+from warnings import warn
 
 import cv2
 import numpy as np
 import skimage.transform
+from pydantic import Field, ValidationInfo, field_validator, model_validator
+from typing_extensions import Annotated, Self
 
 from albumentations import random_utils
 from albumentations.augmentations.functional import bbox_from_mask
+from albumentations.augmentations.utils import BIG_INTEGER, check_range
 from albumentations.core.bbox_utils import denormalize_bbox, normalize_bbox
-from albumentations.core.transforms_interface import DualTransform, to_tuple
+from albumentations.core.pydantic import (
+    BorderModeType,
+    InterpolationType,
+    NonNegativeFloatRangeType,
+    ProbabilityType,
+    SymmetricRangeType,
+)
+from albumentations.core.transforms_interface import BaseTransformInitSchema, DualTransform
 from albumentations.core.types import (
     BoxInternalType,
-    ImageColorType,
+    ColorType,
+    D4Type,
     KeypointInternalType,
     ScaleFloatType,
     ScaleIntType,
     SizeType,
     Targets,
+    d4_group_elements,
 )
+from albumentations.core.utils import to_tuple
 
 from . import functional as F
 
 __all__ = [
     "ShiftScaleRotate",
     "ElasticTransform",
     "Perspective",
@@ -32,154 +46,23 @@
     "VerticalFlip",
     "HorizontalFlip",
     "Flip",
     "Transpose",
     "OpticalDistortion",
     "GridDistortion",
     "PadIfNeeded",
+    "D4",
 ]
 
 TWO = 2
 THREE = 3
 
 
-class ShiftScaleRotate(DualTransform):
-    """Randomly apply affine transforms: translate, scale and rotate the input.
-
-    Args:
-        shift_limit ((float, float) or float): shift factor range for both height and width. If shift_limit
-            is a single float value, the range will be (-shift_limit, shift_limit). Absolute values for lower and
-            upper bounds should lie in range [0, 1]. Default: (-0.0625, 0.0625).
-        scale_limit ((float, float) or float): scaling factor range. If scale_limit is a single float value, the
-            range will be (-scale_limit, scale_limit). Note that the scale_limit will be biased by 1.
-            If scale_limit is a tuple, like (low, high), sampling will be done from the range (1 + low, 1 + high).
-            Default: (-0.1, 0.1).
-        rotate_limit ((int, int) or int): rotation range. If rotate_limit is a single int value, the
-            range will be (-rotate_limit, rotate_limit). Default: (-45, 45).
-        interpolation (OpenCV flag): flag that is used to specify the interpolation algorithm. Should be one of:
-            cv2.INTER_NEAREST, cv2.INTER_LINEAR, cv2.INTER_CUBIC, cv2.INTER_AREA, cv2.INTER_LANCZOS4.
-            Default: cv2.INTER_LINEAR.
-        border_mode (OpenCV flag): flag that is used to specify the pixel extrapolation method. Should be one of:
-            cv2.BORDER_CONSTANT, cv2.BORDER_REPLICATE, cv2.BORDER_REFLECT, cv2.BORDER_WRAP, cv2.BORDER_REFLECT_101.
-            Default: cv2.BORDER_REFLECT_101
-        value (int, float, list of int, list of float): padding value if border_mode is cv2.BORDER_CONSTANT.
-        mask_value (int, float,
-                    list of int,
-                    list of float): padding value if border_mode is cv2.BORDER_CONSTANT applied for masks.
-        shift_limit_x ((float, float) or float): shift factor range for width. If it is set then this value
-            instead of shift_limit will be used for shifting width.  If shift_limit_x is a single float value,
-            the range will be (-shift_limit_x, shift_limit_x). Absolute values for lower and upper bounds should lie in
-            the range [0, 1]. Default: None.
-        shift_limit_y ((float, float) or float): shift factor range for height. If it is set then this value
-            instead of shift_limit will be used for shifting height.  If shift_limit_y is a single float value,
-            the range will be (-shift_limit_y, shift_limit_y). Absolute values for lower and upper bounds should lie
-            in the range [0, 1]. Default: None.
-        rotate_method (str): rotation method used for the bounding boxes. Should be one of "largest_box" or "ellipse".
-            Default: "largest_box"
-        p (float): probability of applying the transform. Default: 0.5.
-
-    Targets:
-        image, mask, keypoints, bboxes
-
-    Image types:
-        uint8, float32
-
-    """
-
-    _targets = (Targets.IMAGE, Targets.MASK, Targets.KEYPOINTS, Targets.BBOXES)
-
-    def __init__(
-        self,
-        shift_limit: ScaleFloatType = 0.0625,
-        scale_limit: ScaleFloatType = 0.1,
-        rotate_limit: int = 45,
-        interpolation: int = cv2.INTER_LINEAR,
-        border_mode: int = cv2.BORDER_REFLECT_101,
-        value: Optional[Tuple[int, ...]] = None,
-        mask_value: Optional[Tuple[int, ...]] = None,
-        shift_limit_x: Optional[ScaleFloatType] = None,
-        shift_limit_y: Optional[ScaleFloatType] = None,
-        rotate_method: str = "largest_box",
-        always_apply: bool = False,
-        p: float = 0.5,
-    ):
-        super().__init__(always_apply, p)
-        self.shift_limit_x = to_tuple(shift_limit_x if shift_limit_x is not None else shift_limit)
-        self.shift_limit_y = to_tuple(shift_limit_y if shift_limit_y is not None else shift_limit)
-        self.scale_limit = to_tuple(scale_limit, bias=1.0)
-        self.rotate_limit = to_tuple(rotate_limit)
-        self.interpolation = interpolation
-        self.border_mode = border_mode
-        self.value = value
-        self.mask_value = mask_value
-        self.rotate_method = rotate_method
-
-        if self.rotate_method not in ["largest_box", "ellipse"]:
-            raise ValueError(f"Rotation method {self.rotate_method} is not valid.")
-
-    def apply(
-        self,
-        img: np.ndarray,
-        angle: float = 0,
-        scale: float = 0,
-        dx: int = 0,
-        dy: int = 0,
-        interpolation: int = cv2.INTER_LINEAR,
-        **params: Any,
-    ) -> np.ndarray:
-        return F.shift_scale_rotate(img, angle, scale, dx, dy, interpolation, self.border_mode, self.value)
-
-    def apply_to_mask(
-        self, mask: np.ndarray, angle: float = 0, scale: float = 0, dx: int = 0, dy: int = 0, **params: Any
-    ) -> np.ndarray:
-        return F.shift_scale_rotate(mask, angle, scale, dx, dy, cv2.INTER_NEAREST, self.border_mode, self.mask_value)
-
-    def apply_to_keypoint(
-        self,
-        keypoint: KeypointInternalType,
-        angle: float = 0,
-        scale: float = 0,
-        dx: int = 0,
-        dy: int = 0,
-        rows: int = 0,
-        cols: int = 0,
-        **params: Any,
-    ) -> KeypointInternalType:
-        return F.keypoint_shift_scale_rotate(keypoint, angle, scale, dx, dy, rows, cols)
-
-    def get_params(self) -> Dict[str, Any]:
-        return {
-            "angle": random.uniform(self.rotate_limit[0], self.rotate_limit[1]),
-            "scale": random.uniform(self.scale_limit[0], self.scale_limit[1]),
-            "dx": random.uniform(self.shift_limit_x[0], self.shift_limit_x[1]),
-            "dy": random.uniform(self.shift_limit_y[0], self.shift_limit_y[1]),
-        }
-
-    def apply_to_bbox(
-        self, bbox: BoxInternalType, angle: float, scale: float, dx: int, dy: int, **params: Any
-    ) -> BoxInternalType:
-        return F.bbox_shift_scale_rotate(bbox, angle, scale, dx, dy, self.rotate_method, **params)
-
-    def get_transform_init_args(self) -> Dict[str, Any]:
-        return {
-            "shift_limit_x": self.shift_limit_x,
-            "shift_limit_y": self.shift_limit_y,
-            "scale_limit": to_tuple(self.scale_limit, bias=-1.0),
-            "rotate_limit": self.rotate_limit,
-            "interpolation": self.interpolation,
-            "border_mode": self.border_mode,
-            "value": self.value,
-            "mask_value": self.mask_value,
-            "rotate_method": self.rotate_method,
-        }
-
-
 class ElasticTransform(DualTransform):
     """Elastic deformation of images as described in [Simard2003]_ (with modifications).
-    Based on https://gist.github.com/ernestum/601cdf56d2b424757de5
 
     .. [Simard2003] Simard, Steinkraus and Platt, "Best Practices for
          Convolutional Neural Networks applied to Visual Document Analysis", in
          Proc. of the International Conference on Document Analysis and
          Recognition, 2003.
 
     Args:
@@ -203,18 +86,38 @@
 
     Targets:
         image, mask, bboxes
 
     Image types:
         uint8, float32
 
+    Reference:
+        https://gist.github.com/ernestum/601cdf56d2b424757de5
+
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES)
 
+    class InitSchema(BaseTransformInitSchema):
+        alpha: Annotated[float, Field(default=1, description="Alpha parameter.", ge=0)]
+        sigma: Annotated[float, Field(default=50, description="Sigma parameter for Gaussian filter.", ge=0)]
+        alpha_affine: Annotated[float, Field(default=50, description="Alpha affine parameter.", ge=0)]
+        interpolation: InterpolationType = cv2.INTER_LINEAR
+        border_mode: BorderModeType = cv2.BORDER_REFLECT_101
+        value: Optional[Union[int, float, List[int], List[float]]] = Field(
+            default=None,
+            description="Padding value if border_mode is cv2.BORDER_CONSTANT.",
+        )
+        mask_value: Optional[Union[float, List[int], List[float]]] = Field(
+            default=None,
+            description="Padding value if border_mode is cv2.BORDER_CONSTANT applied for masks.",
+        )
+        approximate: Annotated[bool, Field(default=False, description="Approximate displacement map smoothing.")]
+        same_dxdy: Annotated[bool, Field(default=False, description="Use same shift for x and y.")]
+
     def __init__(
         self,
         alpha: float = 1,
         sigma: float = 50,
         alpha_affine: float = 50,
         interpolation: int = cv2.INTER_LINEAR,
         border_mode: int = cv2.BORDER_REFLECT_101,
@@ -233,15 +136,19 @@
         self.border_mode = border_mode
         self.value = value
         self.mask_value = mask_value
         self.approximate = approximate
         self.same_dxdy = same_dxdy
 
     def apply(
-        self, img: np.ndarray, random_state: Optional[int] = None, interpolation: int = cv2.INTER_LINEAR, **params: Any
+        self,
+        img: np.ndarray,
+        random_state: Optional[int] = None,
+        interpolation: int = cv2.INTER_LINEAR,
+        **params: Any,
     ) -> np.ndarray:
         return F.elastic_transform(
             img,
             self.alpha,
             self.sigma,
             self.alpha_affine,
             interpolation,
@@ -263,15 +170,18 @@
             self.mask_value,
             np.random.RandomState(random_state),
             self.approximate,
             self.same_dxdy,
         )
 
     def apply_to_bbox(
-        self, bbox: BoxInternalType, random_state: Optional[int] = None, **params: Any
+        self,
+        bbox: BoxInternalType,
+        random_state: Optional[int] = None,
+        **params: Any,
     ) -> BoxInternalType:
         rows, cols = params["rows"], params["cols"]
         mask = np.zeros((rows, cols), dtype=np.uint8)
         bbox_denorm = F.denormalize_bbox(bbox, rows, cols)
         x_min, y_min, x_max, y_max = bbox_denorm[:4]
         x_min, y_min, x_max, y_max = int(x_min), int(y_min), int(x_max), int(y_max)
         mask[y_min:y_max, x_min:x_max] = 1
@@ -334,28 +244,43 @@
     Image types:
         uint8, float32
 
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.KEYPOINTS, Targets.BBOXES)
 
+    class InitSchema(BaseTransformInitSchema):
+        scale: NonNegativeFloatRangeType = (0.05, 0.1)
+        keep_size: Annotated[bool, Field(default=True, description="Keep size after transform.")]
+        pad_mode: BorderModeType = cv2.BORDER_CONSTANT
+        pad_val: Optional[ColorType] = Field(
+            default=0,
+            description="Padding value if border_mode is cv2.BORDER_CONSTANT.",
+        )
+        mask_pad_val: Optional[ColorType] = Field(
+            default=0,
+            description="Mask padding value if border_mode is cv2.BORDER_CONSTANT.",
+        )
+        fit_output: Annotated[bool, Field(default=False, description="Adjust image plane to capture whole image.")]
+        interpolation: InterpolationType = cv2.INTER_LINEAR
+
     def __init__(
         self,
         scale: ScaleFloatType = (0.05, 0.1),
         keep_size: bool = True,
         pad_mode: int = cv2.BORDER_CONSTANT,
-        pad_val: Union[float, List[float]] = 0,
-        mask_pad_val: Union[float, List[float]] = 0,
+        pad_val: Union[ColorType] = 0,
+        mask_pad_val: Union[ColorType] = 0,
         fit_output: bool = False,
         interpolation: int = cv2.INTER_LINEAR,
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
-        self.scale = to_tuple(scale, 0)
+        self.scale = cast(Tuple[float, float], scale)
         self.keep_size = keep_size
         self.pad_mode = pad_mode
         self.pad_val = pad_val
         self.mask_pad_val = mask_pad_val
         self.fit_output = fit_output
         self.interpolation = interpolation
 
@@ -364,15 +289,22 @@
         img: np.ndarray,
         matrix: np.ndarray,
         max_height: int,
         max_width: int,
         **params: Any,
     ) -> np.ndarray:
         return F.perspective(
-            img, matrix, max_width, max_height, self.pad_val, self.pad_mode, self.keep_size, params["interpolation"]
+            img,
+            matrix,
+            max_width,
+            max_height,
+            self.pad_val,
+            self.pad_mode,
+            self.keep_size,
+            params["interpolation"],
         )
 
     def apply_to_bbox(
         self,
         bbox: BoxInternalType,
         matrix: np.ndarray,
         max_height: int,
@@ -386,15 +318,21 @@
         keypoint: KeypointInternalType,
         matrix: np.ndarray,
         max_height: int,
         max_width: int,
         **params: Any,
     ) -> np.ndarray:
         return F.perspective_keypoint(
-            keypoint, params["rows"], params["cols"], matrix, max_width, max_height, self.keep_size
+            keypoint,
+            params["rows"],
+            params["cols"],
+            matrix,
+            max_width,
+            max_height,
+            self.keep_size,
         )
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["image"]
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, Any]:
@@ -606,29 +544,57 @@
     Reference:
         [1] https://arxiv.org/abs/2109.13488
 
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS)
 
+    class InitSchema(BaseTransformInitSchema):
+        scale: Optional[Union[ScaleFloatType, Dict[str, Any]]] = Field(
+            default=None,
+            description="Scaling factor or dictionary for independent axis scaling.",
+        )
+        translate_percent: Optional[Union[ScaleFloatType, Dict[str, Any]]] = Field(
+            default=None,
+            description="Translation as a fraction of the image dimension.",
+        )
+        translate_px: Optional[Union[ScaleIntType, Dict[str, Any]]] = Field(
+            default=None,
+            description="Translation in pixels.",
+        )
+        rotate: Optional[ScaleFloatType] = Field(default=None, description="Rotation angle in degrees.")
+        shear: Optional[Union[ScaleFloatType, Dict[str, Any]]] = Field(
+            default=None,
+            description="Shear angle in degrees.",
+        )
+        interpolation: InterpolationType = cv2.INTER_LINEAR
+        mask_interpolation: InterpolationType = cv2.INTER_NEAREST
+
+        cval: ColorType = Field(default=0, description="Value used for constant padding.")
+        cval_mask: ColorType = Field(default=0, description="Value used for mask constant padding.")
+        mode: BorderModeType = cv2.BORDER_CONSTANT
+        fit_output: Annotated[bool, Field(default=False, description="Adjust output to capture whole image.")]
+        keep_ratio: Annotated[bool, Field(default=False, description="Maintain aspect ratio when scaling.")]
+        rotate_method: Literal["largest_box", "ellipse"] = "largest_box"
+
     def __init__(
         self,
         scale: Optional[Union[ScaleFloatType, Dict[str, Any]]] = None,
-        translate_percent: Optional[Union[float, Tuple[float, float], Dict[str, Any]]] = None,
-        translate_px: Optional[Union[int, Tuple[int, int], Dict[str, Any]]] = None,
+        translate_percent: Optional[Union[ScaleFloatType, Dict[str, Any]]] = None,
+        translate_px: Optional[Union[ScaleIntType, Dict[str, Any]]] = None,
         rotate: Optional[ScaleFloatType] = None,
         shear: Optional[Union[ScaleFloatType, Dict[str, Any]]] = None,
         interpolation: int = cv2.INTER_LINEAR,
         mask_interpolation: int = cv2.INTER_NEAREST,
-        cval: Union[float, Tuple[float, float]] = 0,
-        cval_mask: Union[float, Tuple[float, float]] = 0,
+        cval: ColorType = 0,
+        cval_mask: ColorType = 0,
         mode: int = cv2.BORDER_CONSTANT,
         fit_output: bool = False,
         keep_ratio: bool = False,
-        rotate_method: str = "largest_box",
+        rotate_method: Literal["largest_box", "ellipse"] = "largest_box",
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply=always_apply, p=p)
 
         params = [scale, translate_percent, translate_px, rotate, shear]
         if all(p is None for p in params):
@@ -672,37 +638,39 @@
             "cval_mask",
             "keep_ratio",
             "rotate_method",
         )
 
     @staticmethod
     def _handle_dict_arg(
-        val: Union[float, Tuple[float, float], Dict[str, Any]], name: str, default: float = 1.0
+        val: Union[float, Tuple[float, float], Dict[str, Any]],
+        name: str,
+        default: float = 1.0,
     ) -> Dict[str, Any]:
         if isinstance(val, dict):
             if "x" not in val and "y" not in val:
                 raise ValueError(
-                    f'Expected {name} dictionary to contain at least key "x" or ' 'key "y". Found neither of them.'
+                    f'Expected {name} dictionary to contain at least key "x" or key "y". Found neither of them.',
                 )
             x = val.get("x", default)
             y = val.get("y", default)
             return {"x": to_tuple(x, x), "y": to_tuple(y, y)}
         return {"x": to_tuple(val, val), "y": to_tuple(val, val)}
 
     @classmethod
     def _handle_translate_arg(
         cls,
-        translate_px: Optional[Union[float, Tuple[float, float], Dict[str, Any]]],
-        translate_percent: Optional[Union[float, Tuple[float, float], Dict[str, Any]]],
+        translate_px: Optional[Union[ScaleFloatType, Dict[str, Any]]],
+        translate_percent: Optional[Union[ScaleFloatType, Dict[str, Any]]],
     ) -> Any:
         if translate_percent is None and translate_px is None:
             translate_px = 0
 
         if translate_percent is not None and translate_px is not None:
-            msg = "Expected either translate_percent or translate_px to be " "provided, " "but neither of them was."
+            msg = "Expected either translate_percent or translate_px to be provided, but both were provided."
             raise ValueError(msg)
 
         if translate_percent is not None:
             # translate by percent
             return cls._handle_dict_arg(translate_percent, "translate_percent", default=0.0), translate_px
 
         if translate_px is None:
@@ -830,15 +798,16 @@
             "scale": scale,
             "matrix": matrix,
             "output_shape": output_shape,
         }
 
     @staticmethod
     def _compute_affine_warp_output_shape(
-        matrix: skimage.transform.ProjectiveTransform, input_shape: Sequence[int]
+        matrix: skimage.transform.ProjectiveTransform,
+        input_shape: Sequence[int],
     ) -> Tuple[skimage.transform.ProjectiveTransform, Sequence[int]]:
         height, width = input_shape[:2]
 
         if height == 0 or width == 0:
             return matrix, input_shape
 
         # determine shape of output image
@@ -858,17 +827,149 @@
         # fit output image in new shape
         translation = (-minc, -minr)
         matrix_to_fit = skimage.transform.SimilarityTransform(translation=translation)
         matrix = matrix + matrix_to_fit
         return matrix, output_shape_tuple
 
 
+class ShiftScaleRotate(Affine):
+    """Randomly apply affine transforms: translate, scale and rotate the input.
+
+    Args:
+        shift_limit ((float, float) or float): shift factor range for both height and width. If shift_limit
+            is a single float value, the range will be (-shift_limit, shift_limit). Absolute values for lower and
+            upper bounds should lie in range [-1, 1]. Default: (-0.0625, 0.0625).
+        scale_limit ((float, float) or float): scaling factor range. If scale_limit is a single float value, the
+            range will be (-scale_limit, scale_limit). Note that the scale_limit will be biased by 1.
+            If scale_limit is a tuple, like (low, high), sampling will be done from the range (1 + low, 1 + high).
+            Default: (-0.1, 0.1).
+        rotate_limit ((int, int) or int): rotation range. If rotate_limit is a single int value, the
+            range will be (-rotate_limit, rotate_limit). Default: (-45, 45).
+        interpolation (OpenCV flag): flag that is used to specify the interpolation algorithm. Should be one of:
+            cv2.INTER_NEAREST, cv2.INTER_LINEAR, cv2.INTER_CUBIC, cv2.INTER_AREA, cv2.INTER_LANCZOS4.
+            Default: cv2.INTER_LINEAR.
+        border_mode (OpenCV flag): flag that is used to specify the pixel extrapolation method. Should be one of:
+            cv2.BORDER_CONSTANT, cv2.BORDER_REPLICATE, cv2.BORDER_REFLECT, cv2.BORDER_WRAP, cv2.BORDER_REFLECT_101.
+            Default: cv2.BORDER_REFLECT_101
+        value (int, float, list of int, list of float): padding value if border_mode is cv2.BORDER_CONSTANT.
+        mask_value (int, float,
+                    list of int,
+                    list of float): padding value if border_mode is cv2.BORDER_CONSTANT applied for masks.
+        shift_limit_x ((float, float) or float): shift factor range for width. If it is set then this value
+            instead of shift_limit will be used for shifting width.  If shift_limit_x is a single float value,
+            the range will be (-shift_limit_x, shift_limit_x). Absolute values for lower and upper bounds should lie in
+            the range [-1, 1]. Default: None.
+        shift_limit_y ((float, float) or float): shift factor range for height. If it is set then this value
+            instead of shift_limit will be used for shifting height.  If shift_limit_y is a single float value,
+            the range will be (-shift_limit_y, shift_limit_y). Absolute values for lower and upper bounds should lie
+            in the range [-, 1]. Default: None.
+        rotate_method (str): rotation method used for the bounding boxes. Should be one of "largest_box" or "ellipse".
+            Default: "largest_box"
+        p (float): probability of applying the transform. Default: 0.5.
+
+    Targets:
+        image, mask, keypoints, bboxes
+
+    Image types:
+        uint8, float32
+
+    """
+
+    _targets = (Targets.IMAGE, Targets.MASK, Targets.KEYPOINTS, Targets.BBOXES)
+
+    class InitSchema(BaseTransformInitSchema):
+        shift_limit: SymmetricRangeType = (-0.0625, 0.0625)
+        scale_limit: SymmetricRangeType = (-0.1, 0.1)
+        rotate_limit: SymmetricRangeType = (-45, 45)
+        interpolation: InterpolationType = cv2.INTER_LINEAR
+        border_mode: BorderModeType = cv2.BORDER_REFLECT_101
+        value: ColorType = 0
+        mask_value: ColorType = 0
+        shift_limit_x: Optional[ScaleFloatType] = Field(default=None)
+        shift_limit_y: Optional[ScaleFloatType] = Field(default=None)
+        rotate_method: Literal["largest_box", "ellipse"] = "largest_box"
+
+        @model_validator(mode="after")
+        def check_shift_limit(self) -> Self:
+            bounds = -1, 1
+            self.shift_limit_x = to_tuple(self.shift_limit_x if self.shift_limit_x is not None else self.shift_limit)
+            check_range(self.shift_limit_x, *bounds, "shift_limit_x")
+            self.shift_limit_y = to_tuple(self.shift_limit_y if self.shift_limit_y is not None else self.shift_limit)
+            check_range(self.shift_limit_y, *bounds, "shift_limit_y")
+            return self
+
+        @field_validator("scale_limit")
+        @classmethod
+        def check_scale_limit(cls, value: ScaleFloatType, info: ValidationInfo) -> ScaleFloatType:
+            bounds = 0, float("inf")
+            result = to_tuple(value, bias=1.0)
+            check_range(result, *bounds, str(info.field_name))
+            return result
+
+    def __init__(
+        self,
+        shift_limit: ScaleFloatType = (-0.0625, 0.0625),
+        scale_limit: ScaleFloatType = (-0.1, 0.1),
+        rotate_limit: ScaleFloatType = (-45, 45),
+        interpolation: int = cv2.INTER_LINEAR,
+        border_mode: int = cv2.BORDER_REFLECT_101,
+        value: ColorType = 0,
+        mask_value: ColorType = 0,
+        shift_limit_x: Optional[ScaleFloatType] = None,
+        shift_limit_y: Optional[ScaleFloatType] = None,
+        rotate_method: Literal["largest_box", "ellipse"] = "largest_box",
+        always_apply: bool = False,
+        p: float = 0.5,
+    ):
+        super().__init__(
+            scale=scale_limit,
+            translate_percent={"x": shift_limit_x, "y": shift_limit_y},
+            rotate=rotate_limit,
+            shear=(0, 0),
+            interpolation=interpolation,
+            mask_interpolation=cv2.INTER_NEAREST,
+            cval=value,
+            cval_mask=mask_value,
+            mode=border_mode,
+            fit_output=False,
+            keep_ratio=False,
+            rotate_method=rotate_method,
+            always_apply=always_apply,
+            p=p,
+        )
+        warn(
+            "ShiftScaleRotate is deprecated. Please use Affine transform instead .",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        self.shift_limit_x = cast(Tuple[float, float], shift_limit_x)
+        self.shift_limit_y = cast(Tuple[float, float], shift_limit_y)
+        self.scale_limit = cast(Tuple[float, float], scale_limit)
+        self.rotate_limit = cast(Tuple[int, int], rotate_limit)
+        self.border_mode = border_mode
+        self.value = value
+        self.mask_value = mask_value
+
+    def get_transform_init_args(self) -> Dict[str, Any]:
+        return {
+            "shift_limit_x": self.shift_limit_x,
+            "shift_limit_y": self.shift_limit_y,
+            "scale_limit": to_tuple(self.scale_limit, bias=-1.0),
+            "rotate_limit": self.rotate_limit,
+            "interpolation": self.interpolation,
+            "border_mode": self.border_mode,
+            "value": self.value,
+            "mask_value": self.mask_value,
+            "rotate_method": self.rotate_method,
+        }
+
+
 class PiecewiseAffine(DualTransform):
-    """Apply affine transformations that differ between local neighbourhoods.
-    This augmentation places a regular grid of points on an image and randomly moves the neighbourhood of these point
+    """Apply affine transformations that differ between local neighborhoods.
+    This augmentation places a regular grid of points on an image and randomly moves the neighborhood of these point
     around via affine transformations. This leads to local distortions.
 
     This is mostly a wrapper around scikit-image's ``PiecewiseAffine``.
     See also ``Affine`` for a similar technique.
 
     Note:
         This augmenter is very slow. Try to use ``ElasticTransformation`` instead, which is at least 10x faster.
@@ -920,34 +1021,62 @@
     Image types:
         uint8, float32
 
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS)
 
+    class InitSchema(BaseTransformInitSchema):
+        scale: NonNegativeFloatRangeType = (0.03, 0.05)
+        nb_rows: ScaleIntType = Field(default=4, description="Number of rows in the regular grid.")
+        nb_cols: ScaleIntType = Field(default=4, description="Number of columns in the regular grid.")
+        interpolation: InterpolationType = cv2.INTER_LINEAR
+        mask_interpolation: InterpolationType = cv2.INTER_NEAREST
+        cval: int = Field(default=0, description="Constant value used for newly created pixels.")
+        cval_mask: int = Field(default=0, description="Constant value used for newly created mask pixels.")
+        mode: Literal["constant", "edge", "symmetric", "reflect", "wrap"] = "constant"
+        absolute_scale: bool = Field(
+            default=False,
+            description="Whether scale is an absolute value rather than relative.",
+        )
+        keypoints_threshold: float = Field(
+            default=0.01,
+            description="Threshold for conversion from distance maps to keypoints.",
+        )
+
+        @field_validator("nb_rows", "nb_cols")
+        @classmethod
+        def process_range(cls, value: ScaleFloatType, info: ValidationInfo) -> Tuple[float, float]:
+            bounds = 2, BIG_INTEGER
+            result = to_tuple(value, value)
+            check_range(result, *bounds, info.field_name)
+            return result
+
     def __init__(
         self,
         scale: ScaleFloatType = (0.03, 0.05),
-        nb_rows: Union[ScaleIntType] = 4,
-        nb_cols: Union[ScaleIntType] = 4,
-        interpolation: int = 1,
-        mask_interpolation: int = 0,
+        nb_rows: ScaleIntType = 4,
+        nb_cols: ScaleIntType = 4,
+        interpolation: int = cv2.INTER_LINEAR,
+        mask_interpolation: int = cv2.INTER_NEAREST,
         cval: int = 0,
         cval_mask: int = 0,
-        mode: str = "constant",
+        mode: Literal["constant", "edge", "symmetric", "reflect", "wrap"] = "constant",
         absolute_scale: bool = False,
         always_apply: bool = False,
         keypoints_threshold: float = 0.01,
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
 
-        self.scale = to_tuple(scale, scale)
-        self.nb_rows = to_tuple(nb_rows, nb_rows)
-        self.nb_cols = to_tuple(nb_cols, nb_cols)
+        warn("This augmenter is very slow. Try to use ``ElasticTransformation`` instead, which is at least 10x faster.")
+
+        self.scale = cast(Tuple[float, float], scale)
+        self.nb_rows = cast(Tuple[int, int], nb_rows)
+        self.nb_cols = cast(Tuple[int, int], nb_cols)
         self.interpolation = interpolation
         self.mask_interpolation = mask_interpolation
         self.cval = cval
         self.cval_mask = cval_mask
         self.mode = mode
         self.absolute_scale = absolute_scale
         self.keypoints_threshold = keypoints_threshold
@@ -1018,20 +1147,26 @@
         matrix.estimate(points_src[:, ::-1], points_dest[:, ::-1])
 
         return {
             "matrix": matrix,
         }
 
     def apply(
-        self, img: np.ndarray, matrix: Optional[skimage.transform.PiecewiseAffineTransform] = None, **params: Any
+        self,
+        img: np.ndarray,
+        matrix: Optional[skimage.transform.PiecewiseAffineTransform] = None,
+        **params: Any,
     ) -> np.ndarray:
         return F.piecewise_affine(img, matrix, cast(int, self.interpolation), self.mode, self.cval)
 
     def apply_to_mask(
-        self, mask: np.ndarray, matrix: Optional[skimage.transform.PiecewiseAffineTransform] = None, **params: Any
+        self,
+        mask: np.ndarray,
+        matrix: Optional[skimage.transform.PiecewiseAffineTransform] = None,
+        **params: Any,
     ) -> np.ndarray:
         return F.piecewise_affine(mask, matrix, self.mask_interpolation, self.mode, self.cval_mask)
 
     def apply_to_bbox(
         self,
         bbox: BoxInternalType,
         rows: int = 0,
@@ -1100,35 +1235,59 @@
         TOP_RIGHT = "top_right"
         BOTTOM_LEFT = "bottom_left"
         BOTTOM_RIGHT = "bottom_right"
         RANDOM = "random"
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS)
 
+    class InitSchema(BaseTransformInitSchema):
+        min_height: Optional[int] = Field(default=None, ge=1, description="Minimal result image height.")
+        min_width: Optional[int] = Field(default=None, ge=1, description="Minimal result image width.")
+        pad_height_divisor: Optional[int] = Field(
+            default=None,
+            ge=1,
+            description="Ensures image height is divisible by this value.",
+        )
+        pad_width_divisor: Optional[int] = Field(
+            default=None,
+            ge=1,
+            description="Ensures image width is divisible by this value.",
+        )
+        position: str = Field(default="center", description="Position of the padded image.")
+        border_mode: BorderModeType = cv2.BORDER_REFLECT_101
+        value: Optional[ColorType] = Field(default=None, description="Value for border if BORDER_CONSTANT is used.")
+        mask_value: Optional[ColorType] = Field(
+            default=None,
+            description="Value for mask border if BORDER_CONSTANT is used.",
+        )
+        p: ProbabilityType = 1.0
+
+        @model_validator(mode="after")
+        def validate_divisibility(self) -> Self:
+            if (self.min_height is None) == (self.pad_height_divisor is None):
+                msg = "Only one of 'min_height' and 'pad_height_divisor' parameters must be set"
+                raise ValueError(msg)
+            if (self.min_width is None) == (self.pad_width_divisor is None):
+                msg = "Only one of 'min_width' and 'pad_width_divisor' parameters must be set"
+                raise ValueError(msg)
+            return self
+
     def __init__(
         self,
         min_height: Optional[int] = 1024,
         min_width: Optional[int] = 1024,
         pad_height_divisor: Optional[int] = None,
         pad_width_divisor: Optional[int] = None,
         position: Union[PositionType, str] = PositionType.CENTER,
         border_mode: int = cv2.BORDER_REFLECT_101,
-        value: Optional[ImageColorType] = None,
-        mask_value: Optional[ImageColorType] = None,
+        value: Optional[ColorType] = None,
+        mask_value: Optional[ColorType] = None,
         always_apply: bool = False,
         p: float = 1.0,
     ):
-        if (min_height is None) == (pad_height_divisor is None):
-            msg = "Only one of 'min_height' and 'pad_height_divisor' parameters must be set"
-            raise ValueError(msg)
-
-        if (min_width is None) == (pad_width_divisor is None):
-            msg = "Only one of 'min_width' and 'pad_width_divisor' parameters must be set"
-            raise ValueError(msg)
-
         super().__init__(always_apply, p)
         self.min_height = min_height
         self.min_width = min_width
         self.pad_width_divisor = pad_width_divisor
         self.pad_height_divisor = pad_height_divisor
         self.position = PadIfNeeded.PositionType(position)
         self.border_mode = border_mode
@@ -1165,24 +1324,27 @@
             pad_remainder = cols % self.pad_width_divisor
             pad_cols = self.pad_width_divisor - pad_remainder if pad_remainder > 0 else 0
 
             w_pad_left = pad_cols // 2
             w_pad_right = pad_cols - w_pad_left
 
         h_pad_top, h_pad_bottom, w_pad_left, w_pad_right = self.__update_position_params(
-            h_top=h_pad_top, h_bottom=h_pad_bottom, w_left=w_pad_left, w_right=w_pad_right
+            h_top=h_pad_top,
+            h_bottom=h_pad_bottom,
+            w_left=w_pad_left,
+            w_right=w_pad_right,
         )
 
         params.update(
             {
                 "pad_top": h_pad_top,
                 "pad_bottom": h_pad_bottom,
                 "pad_left": w_pad_left,
                 "pad_right": w_pad_right,
-            }
+            },
         )
         return params
 
     def apply(
         self,
         img: np.ndarray,
         pad_top: int = 0,
@@ -1256,15 +1418,19 @@
             "position",
             "border_mode",
             "value",
             "mask_value",
         )
 
     def __update_position_params(
-        self, h_top: int, h_bottom: int, w_left: int, w_right: int
+        self,
+        h_top: int,
+        h_bottom: int,
+        w_left: int,
+        w_right: int,
     ) -> Tuple[int, int, int, int]:
         if self.position == PadIfNeeded.PositionType.TOP_LEFT:
             h_bottom += h_top
             w_right += w_left
             h_top = 0
             w_left = 0
 
@@ -1410,25 +1576,22 @@
     Image types:
         uint8, float32
 
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS)
 
-    def __init__(self, always_apply: bool = False, p: float = 0.5):
-        super().__init__(always_apply, p)
-
     def apply(self, img: np.ndarray, **params: Any) -> np.ndarray:
         return F.transpose(img)
 
     def apply_to_bbox(self, bbox: BoxInternalType, **params: Any) -> BoxInternalType:
-        return F.bbox_transpose(bbox, 0, **params)
+        return F.bbox_transpose(bbox, **params)
 
     def apply_to_keypoint(self, keypoint: KeypointInternalType, **params: Any) -> KeypointInternalType:
-        return F.keypoint_transpose(keypoint)
+        return F.keypoint_transpose(keypoint, **params)
 
     def get_transform_init_args_names(self) -> Tuple[()]:
         return ()
 
 
 class OpticalDistortion(DualTransform):
     """Args:
@@ -1453,28 +1616,42 @@
     Image types:
         uint8, float32
 
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES)
 
+    class InitSchema(BaseTransformInitSchema):
+        distort_limit: SymmetricRangeType = (-0.05, 0.05)
+        shift_limit: SymmetricRangeType = (-0.05, 0.05)
+        interpolation: InterpolationType = cv2.INTER_LINEAR
+        border_mode: BorderModeType = cv2.BORDER_REFLECT_101
+        value: Optional[ColorType] = Field(
+            default=None,
+            description="Padding value if border_mode is cv2.BORDER_CONSTANT.",
+        )
+        mask_value: Optional[ColorType] = Field(
+            default=None,
+            description="Padding value for mask if border_mode is cv2.BORDER_CONSTANT.",
+        )
+
     def __init__(
         self,
-        distort_limit: ScaleFloatType = 0.05,
-        shift_limit: ScaleFloatType = 0.05,
+        distort_limit: ScaleFloatType = (-0.05, 0.05),
+        shift_limit: ScaleFloatType = (-0.05, 0.05),
         interpolation: int = cv2.INTER_LINEAR,
         border_mode: int = cv2.BORDER_REFLECT_101,
-        value: Optional[ImageColorType] = None,
-        mask_value: Optional[ImageColorType] = None,
+        value: Optional[ColorType] = None,
+        mask_value: Optional[ColorType] = None,
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
-        self.shift_limit = to_tuple(shift_limit)
-        self.distort_limit = to_tuple(distort_limit)
+        self.shift_limit = cast(Tuple[float, float], shift_limit)
+        self.distort_limit = cast(Tuple[float, float], distort_limit)
         self.interpolation = interpolation
         self.border_mode = border_mode
         self.value = value
         self.mask_value = mask_value
 
     def apply(
         self,
@@ -1487,15 +1664,20 @@
     ) -> np.ndarray:
         return F.optical_distortion(img, k, dx, dy, interpolation, self.border_mode, self.value)
 
     def apply_to_mask(self, mask: np.ndarray, k: int = 0, dx: int = 0, dy: int = 0, **params: Any) -> np.ndarray:
         return F.optical_distortion(mask, k, dx, dy, cv2.INTER_NEAREST, self.border_mode, self.mask_value)
 
     def apply_to_bbox(
-        self, bbox: BoxInternalType, k: int = 0, dx: int = 0, dy: int = 0, **params: Any
+        self,
+        bbox: BoxInternalType,
+        k: int = 0,
+        dx: int = 0,
+        dy: int = 0,
+        **params: Any,
     ) -> BoxInternalType:
         rows, cols = params["rows"], params["cols"]
         mask = np.zeros((rows, cols), dtype=np.uint8)
         bbox_denorm = F.denormalize_bbox(bbox, rows, cols)
         x_min, y_min, x_max, y_max = bbox_denorm[:4]
         x_min, y_min, x_max, y_max = int(x_min), int(y_min), int(x_max), int(y_max)
         mask[y_min:y_max, x_min:x_max] = 1
@@ -1545,30 +1727,56 @@
     Image types:
         uint8, float32
 
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES)
 
+    class InitSchema(BaseTransformInitSchema):
+        num_steps: Annotated[int, Field(ge=1, description="Count of grid cells on each side.")]
+        distort_limit: SymmetricRangeType = (-0.03, 0.03)
+        interpolation: InterpolationType = cv2.INTER_LINEAR
+        border_mode: BorderModeType = cv2.BORDER_REFLECT_101
+        value: Optional[ColorType] = Field(
+            default=None,
+            description="Padding value if border_mode is cv2.BORDER_CONSTANT.",
+        )
+        mask_value: Optional[ColorType] = Field(
+            default=None,
+            description="Padding value for mask if border_mode is cv2.BORDER_CONSTANT.",
+        )
+        normalized: bool = Field(
+            default=False,
+            description="If true, distortion will be normalized to not go outside the image.",
+        )
+
+        @field_validator("distort_limit")
+        @classmethod
+        def check_limits(cls, v: Tuple[float, float], info: ValidationInfo) -> Tuple[float, float]:
+            bounds = -1, 1
+            result = to_tuple(v)
+            check_range(result, *bounds, info.field_name)
+            return result
+
     def __init__(
         self,
         num_steps: int = 5,
-        distort_limit: ScaleFloatType = 0.3,
+        distort_limit: ScaleFloatType = (-0.3, 0.3),
         interpolation: int = cv2.INTER_LINEAR,
         border_mode: int = cv2.BORDER_REFLECT_101,
-        value: Optional[ImageColorType] = None,
-        mask_value: Optional[ImageColorType] = None,
+        value: Optional[ColorType] = None,
+        mask_value: Optional[ColorType] = None,
         normalized: bool = False,
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
 
         self.num_steps = num_steps
-        self.distort_limit = to_tuple(distort_limit)
+        self.distort_limit = cast(Tuple[float, float], distort_limit)
         self.interpolation = interpolation
         self.border_mode = border_mode
         self.value = value
         self.mask_value = mask_value
         self.normalized = normalized
 
     def apply(
@@ -1578,31 +1786,51 @@
         stepsy: Tuple[()] = (),
         interpolation: int = cv2.INTER_LINEAR,
         **params: Any,
     ) -> np.ndarray:
         return F.grid_distortion(img, self.num_steps, stepsx, stepsy, interpolation, self.border_mode, self.value)
 
     def apply_to_mask(
-        self, mask: np.ndarray, stepsx: Tuple[()] = (), stepsy: Tuple[()] = (), **params: Any
+        self,
+        mask: np.ndarray,
+        stepsx: Tuple[()] = (),
+        stepsy: Tuple[()] = (),
+        **params: Any,
     ) -> np.ndarray:
         return F.grid_distortion(
-            mask, self.num_steps, stepsx, stepsy, cv2.INTER_NEAREST, self.border_mode, self.mask_value
+            mask,
+            self.num_steps,
+            stepsx,
+            stepsy,
+            cv2.INTER_NEAREST,
+            self.border_mode,
+            self.mask_value,
         )
 
     def apply_to_bbox(
-        self, bbox: BoxInternalType, stepsx: Tuple[()] = (), stepsy: Tuple[()] = (), **params: Any
+        self,
+        bbox: BoxInternalType,
+        stepsx: Tuple[()] = (),
+        stepsy: Tuple[()] = (),
+        **params: Any,
     ) -> BoxInternalType:
         rows, cols = params["rows"], params["cols"]
         mask = np.zeros((rows, cols), dtype=np.uint8)
         bbox_denorm = F.denormalize_bbox(bbox, rows, cols)
         x_min, y_min, x_max, y_max = bbox_denorm[:4]
         x_min, y_min, x_max, y_max = int(x_min), int(y_min), int(x_max), int(y_max)
         mask[y_min:y_max, x_min:x_max] = 1
         mask = F.grid_distortion(
-            mask, self.num_steps, stepsx, stepsy, cv2.INTER_NEAREST, self.border_mode, self.mask_value
+            mask,
+            self.num_steps,
+            stepsx,
+            stepsy,
+            cv2.INTER_NEAREST,
+            self.border_mode,
+            self.mask_value,
         )
         bbox_returned = bbox_from_mask(mask)
         return cast(BoxInternalType, F.normalize_bbox(bbox_returned, rows, cols))
 
     def _normalize(self, h: int, w: int, xsteps: List[float], ysteps: List[float]) -> Dict[str, Any]:
         # compensate for smaller last steps in source image.
         x_step = w // self.num_steps
@@ -1624,17 +1852,91 @@
     @property
     def targets_as_params(self) -> List[str]:
         return ["image"]
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, Any]:
         height, width = params["image"].shape[:2]
 
-        stepsx = [1 + random.uniform(self.distort_limit[0], self.distort_limit[1]) for _ in range(self.num_steps + 1)]
-        stepsy = [1 + random.uniform(self.distort_limit[0], self.distort_limit[1]) for _ in range(self.num_steps + 1)]
+        stepsx = [
+            1 + random_utils.uniform(self.distort_limit[0], self.distort_limit[1]) for _ in range(self.num_steps + 1)
+        ]
+        stepsy = [
+            1 + random_utils.uniform(self.distort_limit[0], self.distort_limit[1]) for _ in range(self.num_steps + 1)
+        ]
 
         if self.normalized:
             return self._normalize(height, width, stepsx, stepsy)
 
         return {"stepsx": stepsx, "stepsy": stepsy}
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return "num_steps", "distort_limit", "interpolation", "border_mode", "value", "mask_value", "normalized"
+
+
+class D4(DualTransform):
+    """Applies one of the eight possible D4 dihedral group transformations to a square-shaped input,
+        maintaining the square shape. These transformations correspond to the symmetries of a square,
+        including rotations and reflections.
+
+    The D4 group transformations include:
+    - 'e' (identity): No transformation is applied.
+    - 'r90' (rotation by 90 degrees counterclockwise)
+    - 'r180' (rotation by 180 degrees)
+    - 'r270' (rotation by 270 degrees counterclockwise)
+    - 'v' (reflection across the vertical midline)
+    - 'hvt' (reflection across the anti-diagonal)
+    - 'h' (reflection across the horizontal midline)
+    - 't' (reflection across the main diagonal)
+
+    Even if the probability (`p`) of applying the transform is set to 1, the identity transformation
+    'e' may still occur, which means the input will remain unchanged in one out of eight cases.
+
+    Args:
+        p (float): Probability of applying the transform. Default is 1, meaning the
+                   transform is applied every time it is called.
+
+    Targets:
+        image, mask, bboxes, keypoints
+
+    Image types:
+        uint8, float32
+
+    Note:
+        This transform is particularly useful when augmenting data that does not have a clear orientation:
+        - Top view satellite or drone imagery
+        - Medical images
+
+    """
+
+    _targets = (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS)
+
+    class InitSchema(BaseTransformInitSchema):
+        p: ProbabilityType = 1
+
+    def __init__(
+        self,
+        always_apply: bool = False,
+        p: float = 1,
+    ):
+        super().__init__(always_apply, p)
+
+    def apply(self, img: np.ndarray, group_element: D4Type, **params: Any) -> np.ndarray:
+        return F.d4(img, group_element)
+
+    def apply_to_bbox(self, bbox: BoxInternalType, group_element: D4Type, **params: Any) -> BoxInternalType:
+        return F.bbox_d4(bbox, group_element, **params)
+
+    def apply_to_keypoint(
+        self,
+        keypoint: KeypointInternalType,
+        group_element: D4Type,
+        **params: Any,
+    ) -> KeypointInternalType:
+        return F.keypoint_d4(keypoint, group_element, **params)
+
+    def get_params(self) -> Dict[str, D4Type]:
+        return {
+            "group_element": random_utils.choice(d4_group_elements),
+        }
+
+    def get_transform_init_args_names(self) -> Tuple[()]:
+        return ()
```

### Comparing `albumentations-1.4.3/albumentations/augmentations/mixing/transforms.py` & `albumentations-1.4.4/albumentations/augmentations/mixing/transforms.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import random
 import types
 from typing import Any, Callable, Dict, Generator, Iterable, Iterator, List, Optional, Sequence, Tuple, Union
 from warnings import warn
 
 import numpy as np
+from pydantic import Field
+from typing_extensions import Annotated
 
+from albumentations.augmentations.functional import add_weighted
 from albumentations.augmentations.utils import is_grayscale_image
-from albumentations.core.transforms_interface import ReferenceBasedTransform
+from albumentations.core.transforms_interface import BaseTransformInitSchema, ReferenceBasedTransform
 from albumentations.core.types import BoxType, KeypointType, ReferenceImage, Targets
 from albumentations.random_utils import beta
 
-from .functional import mix_arrays
-
 __all__ = ["MixUp"]
 
 
 class MixUp(ReferenceBasedTransform):
     """Performs MixUp data augmentation, blending images, masks, and class labels with reference data.
 
     MixUp augmentation linearly combines an input (image, mask, and class label) with another set from a predefined
@@ -103,30 +104,32 @@
 
         # Print applied mix coefficient
         print(data["mix_coef"])  # Output: e.g., 0.9991580344142427
     """
 
     _targets = (Targets.IMAGE, Targets.MASK, Targets.GLOBAL_LABEL)
 
+    class InitSchema(BaseTransformInitSchema):
+        reference_data: Optional[Union[Generator[Any, None, None], Sequence[Any]]] = None
+        read_fn: Callable[[ReferenceImage], Any]
+        alpha: Annotated[float, Field(default=0.4, ge=0, le=1)]
+        mix_coef_return_name: str = "mix_coef"
+
     def __init__(
         self,
-        reference_data: Optional[Union[Generator[ReferenceImage, None, None], Sequence[Any]]] = None,
+        reference_data: Optional[Union[Generator[Any, None, None], Sequence[Any]]] = None,
         read_fn: Callable[[ReferenceImage], Any] = lambda x: {"image": x, "mask": None, "class_label": None},
         alpha: float = 0.4,
         mix_coef_return_name: str = "mix_coef",
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
         self.mix_coef_return_name = mix_coef_return_name
 
-        if alpha < 0:
-            msg = "Alpha must be >= 0."
-            raise ValueError(msg)
-
         self.read_fn = read_fn
         self.alpha = alpha
 
         if reference_data is None:
             warn("No reference data provided for MixUp. This transform will act as a no-op.")
             # Create an empty generator
             self.reference_data: List[Any] = []
@@ -137,40 +140,50 @@
         ):
             self.reference_data = reference_data  # type: ignore[assignment]
         else:
             msg = "reference_data must be a list, tuple, generator, or None."
             raise TypeError(msg)
 
     def apply(self, img: np.ndarray, mix_data: ReferenceImage, mix_coef: float, **params: Any) -> np.ndarray:
-        mix_img = mix_data.get("image")
+        if not mix_data:
+            return img
 
-        if not is_grayscale_image(img) and img.shape != img.shape:
+        mix_img = mix_data["image"]
+
+        if not is_grayscale_image(img) and img.shape != mix_img.shape:
             msg = "The shape of the reference image should be the same as the input image."
             raise ValueError(msg)
 
-        return mix_arrays(img, mix_img, mix_coef) if mix_img is not None else img
+        return add_weighted(img, mix_coef, mix_img, 1 - mix_coef) if mix_img is not None else img
 
     def apply_to_mask(self, mask: np.ndarray, mix_data: ReferenceImage, mix_coef: float, **params: Any) -> np.ndarray:
         mix_mask = mix_data.get("mask")
-        return mix_arrays(mask, mix_mask, mix_coef) if mix_mask is not None else mask
+        return add_weighted(mask, mix_coef, mix_mask, 1 - mix_coef) if mix_mask is not None else mask
 
     def apply_to_global_label(
-        self, label: np.ndarray, mix_data: ReferenceImage, mix_coef: float, **params: Any
+        self,
+        label: np.ndarray,
+        mix_data: ReferenceImage,
+        mix_coef: float,
+        **params: Any,
     ) -> np.ndarray:
         mix_label = mix_data.get("global_label")
         if mix_label is not None and label is not None:
             return mix_coef * label + (1 - mix_coef) * mix_label
         return label
 
     def apply_to_bboxes(self, bboxes: Sequence[BoxType], mix_data: ReferenceImage, **params: Any) -> Sequence[BoxType]:
         msg = "MixUp does not support bounding boxes yet, feel free to submit pull request to https://github.com/albumentations-team/albumentations/."
         raise NotImplementedError(msg)
 
     def apply_to_keypoints(
-        self, keypoints: Sequence[KeypointType], *args: Any, **params: Any
+        self,
+        keypoints: Sequence[KeypointType],
+        *args: Any,
+        **params: Any,
     ) -> Sequence[KeypointType]:
         msg = "MixUp does not support keypoints yet, feel free to submit pull request to https://github.com/albumentations-team/albumentations/."
         raise NotImplementedError(msg)
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return "reference_data", "alpha"
```

### Comparing `albumentations-1.4.3/albumentations/augmentations/transforms.py` & `albumentations-1.4.4/albumentations/augmentations/transforms.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,63 @@
 import math
 import numbers
 import random
 import warnings
-from enum import IntEnum
 from types import LambdaType
 from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union, cast
 from warnings import warn
 
 import cv2
 import numpy as np
+from pydantic import Field, ValidationInfo, field_validator, model_validator
 from scipy import special
 from scipy.ndimage import gaussian_filter
+from typing_extensions import Annotated, Literal, Self
 
 from albumentations import random_utils
 from albumentations.augmentations.blur.functional import blur
+from albumentations.augmentations.blur.transforms import BlurInitSchema, process_blur_limit
 from albumentations.augmentations.utils import (
+    check_range,
     get_num_channels,
     is_grayscale_image,
     is_rgb_image,
 )
-from albumentations.core.transforms_interface import DualTransform, ImageOnlyTransform, Interpolation, NoOp, to_tuple
+from albumentations.core.pydantic import (
+    InterpolationType,
+    NonNegativeFloatRangeType,
+    OnePlusFloatRangeType,
+    OnePlusIntRangeType,
+    ProbabilityType,
+    SymmetricRangeType,
+    ZeroOneRangeType,
+)
+from albumentations.core.transforms_interface import (
+    BaseTransformInitSchema,
+    DualTransform,
+    ImageOnlyTransform,
+    Interpolation,
+    NoOp,
+)
 from albumentations.core.types import (
     BoxInternalType,
     ChromaticAberrationMode,
+    ColorType,
+    ImageCompressionType,
     ImageMode,
     KeypointInternalType,
     MorphologyMode,
+    RainMode,
     ScaleFloatType,
     ScaleIntType,
     ScaleType,
     SpatterMode,
     Targets,
-    image_modes,
 )
-from albumentations.core.utils import format_args
+from albumentations.core.utils import format_args, to_tuple
 
 from . import functional as F
 
 __all__ = [
     "Normalize",
     "RandomGamma",
     "RandomGridShuffle",
@@ -78,67 +98,86 @@
     "UnsharpMask",
     "PixelDropout",
     "Spatter",
     "ChromaticAberration",
     "Morphological",
 ]
 
+NUM_BITS_ARRAY_LENGTH = 3
+GRAYSCALE_SHAPE_LEN = 2
+NUM_RGB_CHANNELS = 3
+NUM_BITS_ARRAY_LENGTH = 3
 MAX_JPEG_QUALITY = 100
 TWENTY = 20
-FIVE = 5
-THREE = 3
-TWO = 2
+PAIR = 2
 
 
 class RandomGridShuffle(DualTransform):
-    """Random shuffle grid's cells on image.
+    """Randomly shuffles the grid's cells on an image, mask, or keypoints,
+    effectively rearranging patches within the image.
+    This transformation divides the image into a grid and then permutes these grid cells based on a random mapping.
+
 
     Args:
-        grid ((int, int)): size of grid for splitting image.
+        grid (Tuple[int, int]): Size of the grid for splitting the image into cells. Each cell is shuffled randomly.
+        p (float): Probability that the transform will be applied.
 
     Targets:
         image, mask, keypoints
 
     Image types:
         uint8, float32
 
+    Examples:
+        >>> import albumentations as A
+        >>> transform = A.Compose([
+            A.RandomGridShuffle(grid=(3, 3), always_apply=False, p=1.0)
+        ])
+        >>> transformed = transform(image=my_image, mask=my_mask)
+        >>> image, mask = transformed['image'], transformed['mask']
+        # This will shuffle the 3x3 grid cells of `my_image` and `my_mask` randomly.
+        # Mask and image are shuffled in a consistent way
+    Note:
+        This transform could be useful when only micro features are important for the model, and memorizing
+        the global structure could be harmful. For example:
+        - Identifying the type of cell phone used to take a picture based on micro artifacts generated by
+        phone post-processing algorithms, rather than the semantic features of the photo.
+        See more at https://ieeexplore.ieee.org/abstract/document/8622031
+        - Identifying stress, glucose, hydration levels based on skin images.
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        grid: OnePlusIntRangeType = (3, 3)
+
     _targets = (Targets.IMAGE, Targets.MASK, Targets.KEYPOINTS)
 
     def __init__(self, grid: Tuple[int, int] = (3, 3), always_apply: bool = False, p: float = 0.5):
-        super().__init__(always_apply, p)
-
-        n, m = grid
-
-        if not all(isinstance(dim, int) and dim > 0 for dim in [n, m]):
-            raise ValueError(f"Grid dimensions must be positive integers. Current grid dimensions: [{n}, {m}]")
-
+        super().__init__(always_apply=always_apply, p=p)
         self.grid = grid
 
-    def apply(self, img: np.ndarray, tiles: Optional[np.ndarray] = None, **params: Any) -> np.ndarray:
-        return F.swap_tiles_on_image(img, tiles)
+    def apply(self, img: np.ndarray, tiles: np.ndarray, mapping: List[int], **params: Any) -> np.ndarray:
+        return F.swap_tiles_on_image(img, tiles, mapping)
 
-    def apply_to_mask(self, mask: np.ndarray, tiles: Optional[np.ndarray] = None, **params: Any) -> np.ndarray:
-        return F.swap_tiles_on_image(mask, tiles)
+    def apply_to_mask(self, mask: np.ndarray, tiles: np.ndarray, mapping: List[int], **params: Any) -> np.ndarray:
+        return F.swap_tiles_on_image(mask, tiles, mapping)
 
     def apply_to_keypoint(
         self,
         keypoint: KeypointInternalType,
         tiles: np.ndarray,
-        mapping: Dict[int, int],
+        mapping: List[int],
         **params: Any,
     ) -> KeypointInternalType:
         x, y = keypoint[:2]
 
         # Find which original tile the keypoint belongs to
-        for original_index, (start_y, start_x, end_y, end_x) in enumerate(tiles):
+        for original_index, new_index in enumerate(mapping):
+            start_y, start_x, end_y, end_x = tiles[original_index]
+            # check if the keypoint is in this tile
             if start_y <= y < end_y and start_x <= x < end_x:
-                # Find this tile's new index after shuffling
-                new_index = mapping[original_index]
                 # Get the new tile's coordinates
                 new_start_y, new_start_x = tiles[new_index][:2]
 
                 # Map the keypoint to the new tile's position
                 new_x = (x - start_x) + new_start_x
                 new_y = (y - start_y) + new_start_y
 
@@ -147,74 +186,140 @@
         # If the keypoint wasn't in any tile (shouldn't happen), log a warning for debugging purposes
         warn(
             "Keypoint not in any tile, returning it unchanged. This is unexpected and should be investigated.",
             RuntimeWarning,
         )
         return keypoint
 
-    def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, Any]:
-        # Generate the original grid
-        original_tiles = F.split_uniform_grid(params["image"].shape[:2], self.grid)
-
-        # Copy the original grid to keep track of the initial positions
-        indexed_tiles = np.array(list(enumerate(original_tiles)), dtype=object)
-
-        # Shuffle the tiles while keeping track of original indices
-        random_utils.shuffle(indexed_tiles)
-
-        # Create a mapping from original positions to new positions
-        mapping = {original_index: i for i, (original_index, tile) in enumerate(indexed_tiles)}
-
-        # Extract the shuffled tiles without indices
-        shuffled_tiles = np.array([tile for _, tile in indexed_tiles])
+    def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, np.ndarray]:
+        height, weight = params["image"].shape[:2]
+        random_state = random_utils.get_random_state()
+        original_tiles = F.split_uniform_grid(
+            (height, weight),
+            self.grid,
+            random_state=random_state,
+        )
+        shape_groups = F.create_shape_groups(original_tiles)
+        mapping = F.shuffle_tiles_within_shape_groups(shape_groups, random_state=random_state)
 
-        return {"tiles": shuffled_tiles, "mapping": mapping}
+        return {"tiles": original_tiles, "mapping": mapping}
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["image"]
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return ("grid",)
 
 
 class Normalize(ImageOnlyTransform):
-    """Normalization is applied by the formula: `img = (img - mean * max_pixel_value) / (std * max_pixel_value)`
+    """Applies various normalization techniques to an image. The specific normalization technique can be selected
+        with the `normalization` parameter.
+
+    Standard normalization is applied using the formula:
+        `img = (img - mean * max_pixel_value) / (std * max_pixel_value)`.
+        Other normalization techniques adjust the image based on global or per-channel statistics,
+        or scale pixel values to a specified range.
 
     Args:
-        mean: mean values
-        std: std values
-        max_pixel_value: maximum possible pixel value
+        mean (Optional[ColorType]): Mean values for standard normalization.
+            For "standard" normalization, the default values are ImageNet mean values: (0.485, 0.456, 0.406).
+            For "inception" normalization, use mean values of (0.5, 0.5, 0.5).
+        std (Optional[ColorType]): Standard deviation values for standard normalization.
+            For "standard" normalization, the default values are ImageNet standard deviation :(0.229, 0.224, 0.225).
+            For "inception" normalization, use standard deviation values of (0.5, 0.5, 0.5).
+        max_pixel_value (Optional[float]): Maximum possible pixel value, used for scaling in standard normalization.
+            Defaults to 255.0.
+        normalization (Literal["standard", "image", "image_per_channel", "min_max", "min_max_per_channel", "inception"])
+            Specifies the normalization technique to apply. Defaults to "standard".
+            - "standard": Applies the formula `(img - mean * max_pixel_value) / (std * max_pixel_value)`.
+                The default mean and std are based on ImageNet.
+            - "image": Normalizes the whole image based on its global mean and standard deviation.
+            - "image_per_channel": Normalizes the image per channel based on each channel's mean and standard deviation.
+            - "min_max": Scales the image pixel values to a [0, 1] range based on the global
+                minimum and maximum pixel values.
+            - "min_max_per_channel": Scales each channel of the image pixel values to a [0, 1]
+                range based on the per-channel minimum and maximum pixel values.
+            - "inception": Applies normalization suitable for Inception models
+                with mean and std values of (0.5, 0.5, 0.5) respectively.
+
+        p (float): Probability of applying the transform. Defaults to 1.0.
 
     Targets:
         image
 
     Image types:
         uint8, float32
 
+    Note:
+        For "standard" normalization, `mean`, `std`, and `max_pixel_value` must be provided.
+        For "inception" normalization, the specific mean and std values should be used.
+        For other normalization types, these parameters are ignored.
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        mean: Optional[ColorType] = Field(
+            default=(0.485, 0.456, 0.406),
+            description="Mean values for normalization, defaulting to ImageNet mean values.",
+        )
+        std: Optional[ColorType] = Field(
+            default=(0.229, 0.224, 0.225),
+            description="Standard deviation values for normalization, defaulting to ImageNet std values.",
+        )
+        max_pixel_value: Optional[float] = Field(default=255.0, description="Maximum possible pixel value.")
+        normalization: Literal[
+            "standard",
+            "image",
+            "image_per_channel",
+            "min_max",
+            "min_max_per_channel",
+            "inception",
+        ] = "standard"
+        p: ProbabilityType = 1
+
+        @model_validator(mode="after")
+        def validate_normalization(self) -> Self:
+            if (
+                self.mean is None
+                or self.std is None
+                or self.max_pixel_value is None
+                and self.normalization == "standard"
+            ):
+                raise ValueError("mean, std, and max_pixel_value must be provided for standard normalization.")
+            return self
+
     def __init__(
         self,
-        mean: Union[float, Sequence[float]] = (0.485, 0.456, 0.406),
-        std: Union[float, Sequence[float]] = (0.229, 0.224, 0.225),
-        max_pixel_value: float = 255.0,
+        mean: Optional[ColorType] = (0.485, 0.456, 0.406),
+        std: Optional[ColorType] = (0.229, 0.224, 0.225),
+        max_pixel_value: Optional[float] = 255.0,
+        normalization: Literal["standard", "image", "image_per_channel", "min_max", "min_max_per_channel"] = "standard",
         always_apply: bool = False,
         p: float = 1.0,
     ):
-        super().__init__(always_apply, p)
+        super().__init__(always_apply=always_apply, p=p)
         self.mean = mean
         self.std = std
         self.max_pixel_value = max_pixel_value
+        self.normalization = normalization
 
     def apply(self, img: np.ndarray, **params: Any) -> np.ndarray:
-        return F.normalize(img, self.mean, self.std, self.max_pixel_value)
+        if self.normalization == "standard":
+            return F.normalize(
+                img,
+                cast(ColorType, self.mean),
+                cast(ColorType, self.std),
+                cast(float, self.max_pixel_value),
+            )
+        if self.normalization in {"image", "image_per_channel", "min_max", "min_max_per_channel"}:
+            return F.normalize_per_image(img, self.normalization)
+        raise ValueError(f"Unknown normalization type: {self.normalization}")
 
-    def get_transform_init_args_names(self) -> Tuple[str, str, str]:
-        return ("mean", "std", "max_pixel_value")
+    def get_transform_init_args_names(self) -> Tuple[str, ...]:
+        return ("mean", "std", "max_pixel_value", "normalization")
 
 
 class ImageCompression(ImageOnlyTransform):
     """Decreases image quality by Jpeg, WebP compression of an image.
 
     Args:
         quality_lower: lower bound on the image quality. Should be in [0, 100] range for jpeg and [1, 100] for webp.
@@ -226,66 +331,57 @@
         image
 
     Image types:
         uint8, float32
 
     """
 
-    class ImageCompressionType(IntEnum):
-        """Defines the types of image compression.
-
-        This Enum class is used to specify the image compression format.
-
-        Attributes:
-            JPEG (int): Represents the JPEG image compression format.
-            WEBP (int): Represents the WEBP image compression format.
-
-        """
+    class InitSchema(BaseTransformInitSchema):
+        quality_lower: int = Field(default=99, description="Lower bound on the image quality", ge=1, le=100)
+        quality_upper: int = Field(default=100, description="Upper bound on the image quality", ge=1, le=100)
+        compression_type: ImageCompressionType = Field(
+            default=ImageCompressionType.JPEG,
+            description="Image compression format",
+        )
 
-        JPEG = 0
-        WEBP = 1
+        @model_validator(mode="after")
+        def validate_quality(self) -> Self:
+            if self.quality_lower >= self.quality_upper:
+                msg = "quality_lower must be less than quality_upper"
+                raise ValueError(msg)
+            return self
 
     def __init__(
         self,
         quality_lower: int = 99,
         quality_upper: int = 100,
         compression_type: ImageCompressionType = ImageCompressionType.JPEG,
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
 
-        self.compression_type = ImageCompression.ImageCompressionType(compression_type)
-        low_thresh_quality_assert = 0
-
-        if self.compression_type == ImageCompression.ImageCompressionType.WEBP:
-            low_thresh_quality_assert = 1
-
-        if not low_thresh_quality_assert <= quality_lower <= MAX_JPEG_QUALITY:
-            raise ValueError(f"Invalid quality_lower. Got: {quality_lower}")
-        if not low_thresh_quality_assert <= quality_upper <= MAX_JPEG_QUALITY:
-            raise ValueError(f"Invalid quality_upper. Got: {quality_upper}")
-
         self.quality_lower = quality_lower
         self.quality_upper = quality_upper
+        self.compression_type = compression_type
 
     def apply(self, img: np.ndarray, quality: int = 100, image_type: str = ".jpg", **params: Any) -> np.ndarray:
-        if img.ndim != TWO and img.shape[-1] not in (1, 3, 4):
+        if img.ndim != GRAYSCALE_SHAPE_LEN and img.shape[-1] not in (1, 3, 4):
             msg = "ImageCompression transformation expects 1, 3 or 4 channel images."
             raise TypeError(msg)
         return F.image_compression(img, quality, image_type)
 
     def get_params(self) -> Dict[str, Any]:
         image_type = ".jpg"
 
-        if self.compression_type == ImageCompression.ImageCompressionType.WEBP:
+        if self.compression_type == ImageCompressionType.WEBP:
             image_type = ".webp"
 
         return {
-            "quality": random.randint(self.quality_lower, self.quality_upper),
+            "quality": random_utils.randint(self.quality_lower, self.quality_upper + 1),
             "image_type": image_type,
         }
 
     def get_transform_init_args(self) -> Dict[str, Any]:
         return {
             "quality_lower": self.quality_lower,
             "quality_upper": self.quality_upper,
@@ -307,33 +403,36 @@
         image
 
     Image types:
         uint8, float32
 
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        snow_point_lower: float = Field(default=0.1, description="Lower bound of the amount of snow", ge=0, le=1)
+        snow_point_upper: float = Field(default=0.3, description="Upper bound of the amount of snow", ge=0, le=1)
+        brightness_coeff: float = Field(default=2.5, description="Brightness coefficient, must be >= 0", ge=0)
+
+        @model_validator(mode="after")
+        def validate_snow_points(self) -> Self:
+            if self.snow_point_lower > self.snow_point_upper:
+                msg = "snow_point_lower must be less than or equal to snow_point_upper."
+                raise ValueError(msg)
+            return self
+
     def __init__(
         self,
         snow_point_lower: float = 0.1,
         snow_point_upper: float = 0.3,
         brightness_coeff: float = 2.5,
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
 
-        if not 0 <= snow_point_lower <= snow_point_upper <= 1:
-            msg = (
-                "Invalid combination of snow_point_lower and snow_point_upper. "
-                f"Got: {(snow_point_lower, snow_point_upper)}"
-            )
-            raise ValueError(msg)
-        if brightness_coeff < 0:
-            raise ValueError(f"brightness_coeff must be greater than 0. Got: {brightness_coeff}")
-
         self.snow_point_lower = snow_point_lower
         self.snow_point_upper = snow_point_upper
         self.brightness_coeff = brightness_coeff
 
     def apply(self, img: np.ndarray, snow_point: float = 0.1, **params: Any) -> np.ndarray:
         return F.add_snow(img, snow_point, self.brightness_coeff)
 
@@ -358,30 +457,36 @@
         image
 
     Image types:
         uint8, float32
 
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        gravel_roi: Tuple[float, float, float, float] = Field(
+            default=(0.1, 0.4, 0.9, 0.9),
+            description="Region of interest for gravel placement",
+        )
+        number_of_patches: int = Field(default=2, description="Number of gravel patches", ge=1)
+
+        @model_validator(mode="after")
+        def validate_gravel_roi(self) -> Self:
+            gravel_lower_x, gravel_lower_y, gravel_upper_x, gravel_upper_y = self.gravel_roi
+            if not 0 <= gravel_lower_x < gravel_upper_x <= 1 or not 0 <= gravel_lower_y < gravel_upper_y <= 1:
+                raise ValueError(f"Invalid gravel_roi. Got: {self.gravel_roi}.")
+            return self
+
     def __init__(
         self,
         gravel_roi: Tuple[float, float, float, float] = (0.1, 0.4, 0.9, 0.9),
         number_of_patches: int = 2,
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
-
-        (gravel_lower_x, gravel_lower_y, gravel_upper_x, gravel_upper_y) = gravel_roi
-
-        if not 0 <= gravel_lower_x < gravel_upper_x <= 1 or not 0 <= gravel_lower_y < gravel_upper_y <= 1:
-            raise ValueError(f"Invalid gravel_roi. Got: {gravel_roi}.")
-        if number_of_patches < 1:
-            raise ValueError(f"Invalid gravel number_of_patches. Got: {number_of_patches}.")
-
         self.gravel_roi = gravel_roi
         self.number_of_patches = number_of_patches
 
     def generate_gravel_patch(self, rectangular_roi: Tuple[int, int, int, int]) -> np.ndarray:
         x1, y1, x2, y2 = rectangular_roi
         area = abs((x2 - x1) * (y2 - y1))
         count = area // 10
@@ -446,15 +551,15 @@
                     np.concatenate(miny),
                     np.concatenate(maxy),
                     np.concatenate(minx),
                     np.concatenate(maxx),
                     np.concatenate(val),
                 ],
                 1,
-            )
+            ),
         }
 
     def get_transform_init_args_names(self) -> Tuple[str, str]:
         return "gravel_roi", "number_of_patches"
 
 
 class RandomRain(ImageOnlyTransform):
@@ -476,44 +581,52 @@
         image
 
     Image types:
         uint8, float32
 
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        slant_lower: int = Field(default=-10, description="Lower bound for rain slant angle", ge=-20, le=20)
+        slant_upper: int = Field(default=10, description="Upper bound for rain slant angle", ge=-20, le=20)
+        drop_length: int = Field(default=20, description="Length of raindrops", ge=0, le=100)
+        drop_width: int = Field(default=1, description="Width of raindrops", ge=1, le=5)
+        drop_color: Tuple[int, int, int] = Field(default=(200, 200, 200), description="Color of raindrops")
+        blur_value: int = Field(default=7, description="Blur value for simulating rain effect", ge=0)
+        brightness_coefficient: float = Field(
+            default=0.7,
+            description="Brightness coefficient for rainy effect",
+            ge=0,
+            le=1,
+        )
+        rain_type: Optional[RainMode] = Field(default=None, description="Type of rain to simulate")
+
+        @model_validator(mode="after")
+        def validate_slant_range_and_rain_type(self) -> Self:
+            if self.slant_lower >= self.slant_upper:
+                msg = "slant_upper must be greater than or equal to slant_lower."
+                raise ValueError(msg)
+            return self
+
     def __init__(
         self,
         slant_lower: int = -10,
         slant_upper: int = 10,
         drop_length: int = 20,
         drop_width: int = 1,
         drop_color: Tuple[int, int, int] = (200, 200, 200),
         blur_value: int = 7,
         brightness_coefficient: float = 0.7,
-        rain_type: Optional[str] = None,
+        rain_type: Optional[RainMode] = None,
         always_apply: bool = False,
         p: float = 0.5,
     ):
-        super().__init__(always_apply, p)
-
-        if rain_type not in ["drizzle", "heavy", "torrential", None]:
-            msg = "raint_type must be one of ({}). Got: {}".format(["drizzle", "heavy", "torrential", None], rain_type)
-            raise ValueError(msg)
-        if not -TWENTY <= slant_lower <= slant_upper <= TWENTY:
-            raise ValueError(f"Invalid combination of slant_lower and slant_upper. Got: {(slant_lower, slant_upper)}")
-        if not 1 <= drop_width <= FIVE:
-            raise ValueError(f"drop_width must be in range [1, 5]. Got: {drop_width}")
-        if not 0 <= drop_length <= MAX_JPEG_QUALITY:
-            raise ValueError(f"drop_length must be in range [0, 100]. Got: {drop_length}")
-        if not 0 <= brightness_coefficient <= 1:
-            raise ValueError(f"brightness_coefficient must be in range [0, 1]. Got: {brightness_coefficient}")
-
+        super().__init__(always_apply=always_apply, p=p)
         self.slant_lower = slant_lower
         self.slant_upper = slant_upper
-
         self.drop_length = drop_length
         self.drop_width = drop_width
         self.drop_color = drop_color
         self.blur_value = blur_value
         self.brightness_coefficient = brightness_coefficient
         self.rain_type = rain_type
 
@@ -561,17 +674,17 @@
         else:
             drop_length = self.drop_length
             num_drops = area // 600
 
         rain_drops = []
 
         for _ in range(num_drops):  # If You want heavy rain, try increasing this
-            x = random.randint(slant, width) if slant < 0 else random.randint(0, width - slant)
+            x = random_utils.randint(slant, width + 1) if slant < 0 else random_utils.randint(0, width - slant + 1)
 
-            y = random.randint(0, height - drop_length)
+            y = random_utils.randint(0, height - drop_length + 1)
 
             rain_drops.append((x, y))
 
         return {"drop_length": drop_length, "slant": slant, "rain_drops": rain_drops}
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return (
@@ -585,46 +698,52 @@
             "rain_type",
         )
 
 
 class RandomFog(ImageOnlyTransform):
     """Simulates fog for the image
 
-    From https://github.com/UjjwalSaxena/Automold--Road-Augmentation-Library
-
     Args:
         fog_coef_lower: lower limit for fog intensity coefficient. Should be in [0, 1] range.
         fog_coef_upper: upper limit for fog intensity coefficient. Should be in [0, 1] range.
         alpha_coef: transparency of the fog circles. Should be in [0, 1] range.
 
     Targets:
         image
 
     Image types:
         uint8, float32
 
+    Reference:
+        https://github.com/UjjwalSaxena/Automold--Road-Augmentation-Library
+
+
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        fog_coef_lower: float = Field(default=0.3, description="Lower limit for fog intensity coefficient", ge=0, le=1)
+        fog_coef_upper: float = Field(default=1, description="Upper limit for fog intensity coefficient", ge=0, le=1)
+        alpha_coef: float = Field(default=0.08, description="Transparency of the fog circles", ge=0, le=1)
+
+        @model_validator(mode="after")
+        def validate_fog_coefficients(self) -> Self:
+            if self.fog_coef_lower > self.fog_coef_upper:
+                msg = "fog_coef_upper must be greater than or equal to fog_coef_lower."
+                raise ValueError(msg)
+            return self
+
     def __init__(
         self,
         fog_coef_lower: float = 0.3,
         fog_coef_upper: float = 1,
         alpha_coef: float = 0.08,
         always_apply: bool = False,
         p: float = 0.5,
     ):
-        super().__init__(always_apply, p)
-
-        if not 0 <= fog_coef_lower <= fog_coef_upper <= 1:
-            raise ValueError(
-                f"Invalid combination if fog_coef_lower and fog_coef_upper. Got: {(fog_coef_lower, fog_coef_upper)}"
-            )
-        if not 0 <= alpha_coef <= 1:
-            raise ValueError(f"alpha_coef must be in range [0, 1]. Got: {alpha_coef}")
-
+        super().__init__(always_apply=always_apply, p=p)
         self.fog_coef_lower = fog_coef_lower
         self.fog_coef_upper = fog_coef_upper
         self.alpha_coef = alpha_coef
 
     def apply(
         self,
         img: np.ndarray,
@@ -651,16 +770,16 @@
         haze_list = []
         midx = width // 2 - 2 * hw
         midy = height // 2 - hw
         index = 1
 
         while midx > -hw or midy > -hw:
             for _ in range(hw // 10 * index):
-                x = random.randint(midx, width - midx - hw)
-                y = random.randint(midy, height - midy - hw)
+                x = random_utils.randint(midx, width - midx - hw + 1)
+                y = random_utils.randint(midy, height - midy - hw + 1)
                 haze_list.append((x, y))
 
             midx -= 3 * hw * width // sum(imshape)
             midy -= 3 * hw * height // sum(imshape)
             index += 1
 
         return {"haze_list": haze_list, "fog_coef": fog_coef}
@@ -690,62 +809,68 @@
         image
 
     Image types:
         uint8, float32
 
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        flare_roi: Tuple[float, float, float, float] = Field(
+            default=(0, 0, 1, 0.5),
+            description="Region of the image where flare will appear",
+        )
+        angle_lower: float = Field(default=0, description="Lower bound for the angle", ge=0, le=1)
+        angle_upper: float = Field(default=1, description="Upper bound for the angle", ge=0, le=1)
+        num_flare_circles_lower: int = Field(default=6, description="Lower limit for the number of flare circles", ge=0)
+        num_flare_circles_upper: int = Field(
+            default=10,
+            description="Upper limit for the number of flare circles",
+            gt=0,
+        )
+        src_radius: int = Field(default=400, description="Source radius for the flare")
+        src_color: Tuple[int, int, int] = Field(default=(255, 255, 255), description="Color of the flare")
+
+        @model_validator(mode="after")
+        def validate_parameters(self) -> Self:
+            flare_center_lower_x, flare_center_lower_y, flare_center_upper_x, flare_center_upper_y = self.flare_roi
+            if (
+                not 0 <= flare_center_lower_x < flare_center_upper_x <= 1
+                or not 0 <= flare_center_lower_y < flare_center_upper_y <= 1
+            ):
+                raise ValueError(f"Invalid flare_roi. Got: {self.flare_roi}")
+            if self.angle_lower >= self.angle_upper:
+                raise ValueError(
+                    f"angle_upper must be greater than angle_lower. Got: {self.angle_lower}, {self.angle_upper}",
+                )
+            if self.num_flare_circles_lower >= self.num_flare_circles_upper:
+                msg = "num_flare_circles_upper must be greater than num_flare_circles_lower."
+                raise ValueError(msg)
+            return self
+
     def __init__(
         self,
         flare_roi: Tuple[float, float, float, float] = (0, 0, 1, 0.5),
         angle_lower: float = 0,
         angle_upper: float = 1,
         num_flare_circles_lower: int = 6,
         num_flare_circles_upper: int = 10,
         src_radius: int = 400,
         src_color: Tuple[int, int, int] = (255, 255, 255),
         always_apply: bool = False,
         p: float = 0.5,
     ):
-        super().__init__(always_apply, p)
-
-        (
-            flare_center_lower_x,
-            flare_center_lower_y,
-            flare_center_upper_x,
-            flare_center_upper_y,
-        ) = flare_roi
-
-        if (
-            not 0 <= flare_center_lower_x < flare_center_upper_x <= 1
-            or not 0 <= flare_center_lower_y < flare_center_upper_y <= 1
-        ):
-            raise ValueError(f"Invalid flare_roi. Got: {flare_roi}")
-        if not 0 <= angle_lower < angle_upper <= 1:
-            raise ValueError(f"Invalid combination of angle_lower nad angle_upper. Got: {(angle_lower, angle_upper)}")
-        if not 0 <= num_flare_circles_lower < num_flare_circles_upper:
-            msg = (
-                "Invalid combination of num_flare_circles_lower and num_flare_circles_upper. "
-                f"Got: {(num_flare_circles_lower, num_flare_circles_upper)}"
-            )
-            raise ValueError(msg)
-
-        self.flare_center_lower_x = flare_center_lower_x
-        self.flare_center_upper_x = flare_center_upper_x
-
-        self.flare_center_lower_y = flare_center_lower_y
-        self.flare_center_upper_y = flare_center_upper_y
+        super().__init__(always_apply=always_apply, p=p)
 
         self.angle_lower = angle_lower
         self.angle_upper = angle_upper
         self.num_flare_circles_lower = num_flare_circles_lower
         self.num_flare_circles_upper = num_flare_circles_upper
-
         self.src_radius = src_radius
         self.src_color = src_color
+        self.flare_roi = flare_roi
 
     def apply(
         self,
         img: np.ndarray,
         flare_center_x: float = 0.5,
         flare_center_y: float = 0.5,
         circles: Optional[List[Any]] = None,
@@ -768,21 +893,23 @@
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, Any]:
         img = params["image"]
         height, width = img.shape[:2]
 
         angle = 2 * math.pi * random.uniform(self.angle_lower, self.angle_upper)
 
-        flare_center_x = random.uniform(self.flare_center_lower_x, self.flare_center_upper_x)
-        flare_center_y = random.uniform(self.flare_center_lower_y, self.flare_center_upper_y)
+        (flare_center_lower_x, flare_center_lower_y, flare_center_upper_x, flare_center_upper_y) = self.flare_roi
+
+        flare_center_x = random.uniform(flare_center_lower_x, flare_center_upper_x)
+        flare_center_y = random.uniform(flare_center_lower_y, flare_center_upper_y)
 
         flare_center_x = int(width * flare_center_x)
         flare_center_y = int(height * flare_center_y)
 
-        num_circles = random.randint(self.num_flare_circles_lower, self.num_flare_circles_upper)
+        num_circles = random_utils.randint(self.num_flare_circles_lower, self.num_flare_circles_upper + 1)
 
         circles = []
 
         x = []
         y = []
 
         def line(t: float) -> Tuple[float, float]:
@@ -790,172 +917,198 @@
 
         for t_val in range(-flare_center_x, width - flare_center_x, 10):
             rand_x, rand_y = line(t_val)
             x.append(rand_x)
             y.append(rand_y)
 
         for _ in range(num_circles):
-            alpha = random.uniform(0.05, 0.2)
-            r = random.randint(0, len(x) - 1)
+            alpha = random_utils.uniform(0.05, 0.2)
+            r = random_utils.randint(0, len(x))
             rad = random.randint(1, max(height // 100 - 2, 2))
 
             r_color = random.randint(max(self.src_color[0] - 50, 0), self.src_color[0])
             g_color = random.randint(max(self.src_color[1] - 50, 0), self.src_color[1])
             b_color = random.randint(max(self.src_color[2] - 50, 0), self.src_color[2])
 
             circles += [
                 (
                     alpha,
                     (int(x[r]), int(y[r])),
                     pow(rad, 3),
                     (r_color, g_color, b_color),
-                )
+                ),
             ]
 
         return {
             "circles": circles,
             "flare_center_x": flare_center_x,
             "flare_center_y": flare_center_y,
         }
 
     def get_transform_init_args(self) -> Dict[str, Any]:
         return {
-            "flare_roi": (
-                self.flare_center_lower_x,
-                self.flare_center_lower_y,
-                self.flare_center_upper_x,
-                self.flare_center_upper_y,
-            ),
+            "flare_roi": self.flare_roi,
             "angle_lower": self.angle_lower,
             "angle_upper": self.angle_upper,
             "num_flare_circles_lower": self.num_flare_circles_lower,
             "num_flare_circles_upper": self.num_flare_circles_upper,
             "src_radius": self.src_radius,
             "src_color": self.src_color,
         }
 
 
 class RandomShadow(ImageOnlyTransform):
     """Simulates shadows for the image
 
-    From https://github.com/UjjwalSaxena/Automold--Road-Augmentation-Library
-
     Args:
         shadow_roi: region of the image where shadows
             will appear. All values should be in range [0, 1].
-        num_shadows_lower: Lower limit for the possible number of shadows.
-            Should be in range [0, `num_shadows_upper`].
-        num_shadows_upper: Lower limit for the possible number of shadows.
-            Should be in range [`num_shadows_lower`, inf].
+        num_shadows_limit: Lower and upper limits for the possible number of shadows.
         shadow_dimension: number of edges in the shadow polygons
 
     Targets:
         image
 
     Image types:
         uint8, float32
 
+    Reference:
+        https://github.com/UjjwalSaxena/Automold--Road-Augmentation-Library
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        shadow_roi: Tuple[float, float, float, float] = Field(
+            default=(0, 0.5, 1, 1),
+            description="Region of the image where shadows will appear",
+        )
+        num_shadows_limit: Tuple[int, int] = Field(default=(1, 2))
+        num_shadows_lower: Optional[int] = Field(
+            default=None,
+            description="Lower limit for the possible number of shadows",
+        )
+        num_shadows_upper: Optional[int] = Field(
+            default=None,
+            description="Upper limit for the possible number of shadows",
+        )
+        shadow_dimension: int = Field(default=5, description="Number of edges in the shadow polygons", gt=0)
+
+        @model_validator(mode="after")
+        def validate_shadows(self) -> Self:
+            if self.num_shadows_limit[0] > self.num_shadows_limit[1]:
+                msg = "num_shadows_limit[0] must be less than or equal to num_shadows_limit[1]."
+                raise ValueError(msg)
+
+            shadow_lower_x, shadow_lower_y, shadow_upper_x, shadow_upper_y = self.shadow_roi
+
+            if not 0 <= shadow_lower_x <= shadow_upper_x <= 1 or not 0 <= shadow_lower_y <= shadow_upper_y <= 1:
+                raise ValueError(f"Invalid shadow_roi. Got: {self.shadow_roi}")
+
+            if self.num_shadows_lower is not None or self.num_shadows_upper is not None:
+                warn(
+                    "`num_shadows_lower` and `num_shadows_upper` are deprecated. "
+                    "Use `num_shadows_limit` as tuple (num_shadows_lower, num_shadows_upper) instead.",
+                    DeprecationWarning,
+                    stacklevel=2,
+                )
+                self.num_shadows_limit = cast(Tuple[int, int], (self.num_shadows_lower, self.num_shadows_upper))
+                self.num_shadows_lower = None
+                self.num_shadows_upper = None
+
+            return self
+
     def __init__(
         self,
         shadow_roi: Tuple[float, float, float, float] = (0, 0.5, 1, 1),
-        num_shadows_lower: int = 1,
-        num_shadows_upper: int = 2,
+        num_shadows_limit: Tuple[int, int] = (1, 2),
+        num_shadows_lower: Optional[int] = None,
+        num_shadows_upper: Optional[int] = None,
         shadow_dimension: int = 5,
         always_apply: bool = False,
         p: float = 0.5,
     ):
-        super().__init__(always_apply, p)
-
-        (shadow_lower_x, shadow_lower_y, shadow_upper_x, shadow_upper_y) = shadow_roi
-
-        if not 0 <= shadow_lower_x <= shadow_upper_x <= 1 or not 0 <= shadow_lower_y <= shadow_upper_y <= 1:
-            raise ValueError(f"Invalid shadow_roi. Got: {shadow_roi}")
-        if not 0 <= num_shadows_lower <= num_shadows_upper:
-            msg = "Invalid combination of num_shadows_lower nad num_shadows_upper. "
-            f"Got: {(num_shadows_lower, num_shadows_upper)}"
-            raise ValueError(msg)
+        super().__init__(always_apply=always_apply, p=p)
 
         self.shadow_roi = shadow_roi
-
-        self.num_shadows_lower = num_shadows_lower
-        self.num_shadows_upper = num_shadows_upper
-
         self.shadow_dimension = shadow_dimension
+        self.num_shadows_limit = num_shadows_limit
 
-    def apply(
-        self, img: np.ndarray, vertices_list: Optional[List[List[Tuple[int, int]]]] = None, **params: Any
-    ) -> np.ndarray:
+    def apply(self, img: np.ndarray, vertices_list: Optional[List[np.ndarray]] = None, **params: Any) -> np.ndarray:
         if vertices_list is None:
             vertices_list = []
         return F.add_shadow(img, vertices_list)
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["image"]
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, List[np.ndarray]]:
         img = params["image"]
         height, width = img.shape[:2]
 
-        num_shadows = random.randint(self.num_shadows_lower, self.num_shadows_upper)
+        num_shadows = random_utils.randint(self.num_shadows_limit[0], self.num_shadows_limit[1] + 1)
 
         x_min, y_min, x_max, y_max = self.shadow_roi
 
         x_min = int(x_min * width)
         x_max = int(x_max * width)
         y_min = int(y_min * height)
         y_max = int(y_max * height)
 
-        vertices_list = []
-
-        for _ in range(num_shadows):
-            vertex = [
-                (random.randint(x_min, x_max), random.randint(y_min, y_max)) for _ in range(self.shadow_dimension)
-            ]
-
-            vertices = np.array([vertex], dtype=np.int32)
-            vertices_list.append(vertices)
+        vertices_list = [
+            np.stack(
+                [
+                    random_utils.randint(x_min, x_max, size=5),
+                    random_utils.randint(y_min, y_max, size=5),
+                ],
+                axis=1,
+            )
+            for _ in range(num_shadows)
+        ]
 
         return {"vertices_list": vertices_list}
 
-    def get_transform_init_args_names(self) -> Tuple[str, str, str, str]:
+    def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return (
             "shadow_roi",
-            "num_shadows_lower",
-            "num_shadows_upper",
+            "num_shadows_limit",
             "shadow_dimension",
         )
 
 
 class RandomToneCurve(ImageOnlyTransform):
     """Randomly change the relationship between bright and dark areas of the image by manipulating its tone curve.
 
     Args:
         scale: standard deviation of the normal distribution.
             Used to sample random distances to move two control points that modify the image's curve.
             Values should be in range [0, 1]. Default: 0.1
 
-
     Targets:
         image
 
     Image types:
         uint8
 
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        scale: float = Field(
+            default=0.1,
+            description="Standard deviation of the normal distribution used to sample random distances",
+            ge=0,
+            le=1,
+        )
+
     def __init__(
         self,
         scale: float = 0.1,
         always_apply: bool = False,
         p: float = 0.5,
     ):
-        super().__init__(always_apply, p)
+        super().__init__(always_apply=always_apply, p=p)
         self.scale = scale
 
     def apply(self, img: np.ndarray, low_y: float, high_y: float, **params: Any) -> np.ndarray:
         return F.move_tone_curve(img, low_y, high_y)
 
     def get_params(self) -> Dict[str, float]:
         return {
@@ -983,29 +1136,39 @@
         image
 
     Image types:
         uint8, float32
 
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        hue_shift_limit: SymmetricRangeType = (-20, 20)
+        sat_shift_limit: SymmetricRangeType = (-30, 30)
+        val_shift_limit: SymmetricRangeType = (-20, 20)
+
     def __init__(
         self,
         hue_shift_limit: ScaleIntType = 20,
         sat_shift_limit: ScaleIntType = 30,
         val_shift_limit: ScaleIntType = 20,
         always_apply: bool = False,
         p: float = 0.5,
     ):
-        super().__init__(always_apply, p)
-        self.hue_shift_limit = to_tuple(hue_shift_limit)
-        self.sat_shift_limit = to_tuple(sat_shift_limit)
-        self.val_shift_limit = to_tuple(val_shift_limit)
+        super().__init__(always_apply=always_apply, p=p)
+        self.hue_shift_limit = cast(Tuple[float, float], hue_shift_limit)
+        self.sat_shift_limit = cast(Tuple[float, float], sat_shift_limit)
+        self.val_shift_limit = cast(Tuple[float, float], val_shift_limit)
 
     def apply(
-        self, img: np.ndarray, hue_shift: int = 0, sat_shift: int = 0, val_shift: int = 0, **params: Any
+        self,
+        img: np.ndarray,
+        hue_shift: int = 0,
+        sat_shift: int = 0,
+        val_shift: int = 0,
+        **params: Any,
     ) -> np.ndarray:
         if not is_rgb_image(img) and not is_grayscale_image(img):
             msg = "HueSaturationValue transformation expects 1-channel or 3-channel images."
             raise TypeError(msg)
         return F.shift_hsv(img, hue_shift, sat_shift, val_shift)
 
     def get_params(self) -> Dict[str, float]:
@@ -1020,34 +1183,31 @@
 
 
 class Solarize(ImageOnlyTransform):
     """Invert all pixel values above a threshold.
 
     Args:
         threshold: range for solarizing threshold.
-            If threshold is a single value, the range will be [threshold, threshold]. Default: 128.
+            If threshold is a single value, the range will be [1, threshold]. Default: 128.
         p: probability of applying the transform. Default: 0.5.
 
     Targets:
         image
 
     Image types:
         any
 
     """
 
-    def __init__(self, threshold: ScaleType = 128, always_apply: bool = False, p: float = 0.5):
-        super().__init__(always_apply, p)
-
-        if isinstance(threshold, (int, float)):
-            self.threshold = to_tuple(threshold, low=threshold)
-        else:
-            self.threshold = to_tuple(threshold, low=0)
+    class InitSchema(BaseTransformInitSchema):
+        threshold: OnePlusFloatRangeType = (128, 128)
 
-        self.threshold = self.threshold
+    def __init__(self, threshold: ScaleType = (128, 128), always_apply: bool = False, p: float = 0.5):
+        super().__init__(always_apply=always_apply, p=p)
+        self.threshold = cast(Tuple[float, float], threshold)
 
     def apply(self, img: np.ndarray, threshold: int = 0, **params: Any) -> np.ndarray:
         return F.solarize(img, threshold)
 
     def get_params(self) -> Dict[str, float]:
         return {"threshold": random.uniform(self.threshold[0], self.threshold[1])}
 
@@ -1070,37 +1230,46 @@
     image
 
     Image types:
         uint8
 
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        num_bits: Annotated[
+            Union[int, Tuple[int, int], Tuple[int, int, int]],
+            Field(default=4, description="Number of high bits"),
+        ]
+
+        @field_validator("num_bits")
+        @classmethod
+        def validate_num_bits(cls, num_bits: Any) -> Union[Tuple[int, int], List[Tuple[int, int]]]:
+            if isinstance(num_bits, int):
+                return cast(Tuple[int, int], to_tuple(num_bits, num_bits))
+            if isinstance(num_bits, Sequence) and len(num_bits) == NUM_BITS_ARRAY_LENGTH:
+                return [cast(Tuple[int, int], to_tuple(i, 0)) for i in num_bits]
+            return cast(Tuple[int, int], to_tuple(num_bits, 0))
+
     def __init__(
         self,
         num_bits: Union[int, Tuple[int, int], Tuple[int, int, int]] = 4,
         always_apply: bool = False,
         p: float = 0.5,
     ):
-        super().__init__(always_apply, p)
-
-        if isinstance(num_bits, int):
-            self.num_bits = to_tuple(num_bits, num_bits)
-        elif isinstance(num_bits, Sequence) and len(num_bits) == THREE:
-            self.num_bits = [to_tuple(i, 0) for i in num_bits]  # type: ignore[assignment]
-        else:
-            self.num_bits = to_tuple(num_bits, 0)  # type: ignore[arg-type]
+        super().__init__(always_apply=always_apply, p=p)
+        self.num_bits = cast(Union[Tuple[int, ...], List[Tuple[int, ...]]], num_bits)
 
     def apply(self, img: np.ndarray, num_bits: int = 1, **params: Any) -> np.ndarray:
         return F.posterize(img, num_bits)
 
     def get_params(self) -> Dict[str, Any]:
-        if len(self.num_bits) == THREE:
+        if len(self.num_bits) == NUM_BITS_ARRAY_LENGTH:
             return {"num_bits": [random.randint(int(i[0]), int(i[1])) for i in self.num_bits]}  # type: ignore[index]
         num_bits = self.num_bits
-        return {"num_bits": random.randint(int(num_bits[0]), int(num_bits[1]))}
+        return {"num_bits": random.randint(int(num_bits[0]), int(num_bits[1]))}  # type: ignore[arg-type]
 
     def get_transform_init_args_names(self) -> Tuple[str]:
         return ("num_bits",)
 
 
 class Equalize(ImageOnlyTransform):
     """Equalize the image histogram.
@@ -1118,27 +1287,34 @@
         image
 
     Image types:
         uint8
 
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        mode: ImageMode = "cv"
+        by_channels: Annotated[bool, Field(default=True, description="Equalize channels separately if True")]
+        mask: Annotated[
+            Optional[Union[np.ndarray, Callable[..., Any]]],
+            Field(default=None, description="Mask to apply for equalization"),
+        ]
+        mask_params: Annotated[Sequence[str], Field(default=[], description="Parameters for mask function")]
+
     def __init__(
         self,
         mode: ImageMode = "cv",
         by_channels: bool = True,
-        mask: Optional[np.ndarray] = None,
-        mask_params: Tuple[()] = (),
+        mask: Optional[Union[np.ndarray, Callable[..., Any]]] = None,
+        mask_params: Sequence[str] = (),
         always_apply: bool = False,
         p: float = 0.5,
     ):
-        if mode not in image_modes:
-            raise ValueError(f"Unsupported equalization mode. Supports: {image_modes}. " f"Got: {mode}")
+        super().__init__(always_apply=always_apply, p=p)
 
-        super().__init__(always_apply, p)
         self.mode = mode
         self.by_channels = by_channels
         self.mask = mask
         self.mask_params = mask_params
 
     def apply(self, img: np.ndarray, mask: Optional[np.ndarray] = None, **params: Any) -> np.ndarray:
         return F.equalize(img, mode=self.mode, by_channels=self.by_channels, mask=mask)
@@ -1173,26 +1349,31 @@
         image
 
     Image types:
         uint8, float32
 
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        r_shift_limit: SymmetricRangeType = (-20, 20)
+        g_shift_limit: SymmetricRangeType = (-20, 20)
+        b_shift_limit: SymmetricRangeType = (-20, 20)
+
     def __init__(
         self,
-        r_shift_limit: ScaleIntType = 20,
-        g_shift_limit: ScaleIntType = 20,
-        b_shift_limit: ScaleIntType = 20,
+        r_shift_limit: ScaleIntType = (-20, 20),
+        g_shift_limit: ScaleIntType = (-20, 20),
+        b_shift_limit: ScaleIntType = (-20, 20),
         always_apply: bool = False,
         p: float = 0.5,
     ):
-        super().__init__(always_apply, p)
-        self.r_shift_limit = to_tuple(r_shift_limit)
-        self.g_shift_limit = to_tuple(g_shift_limit)
-        self.b_shift_limit = to_tuple(b_shift_limit)
+        super().__init__(always_apply=always_apply, p=p)
+        self.r_shift_limit = cast(Tuple[float, float], r_shift_limit)
+        self.g_shift_limit = cast(Tuple[float, float], g_shift_limit)
+        self.b_shift_limit = cast(Tuple[float, float], b_shift_limit)
 
     def apply(self, img: np.ndarray, r_shift: int = 0, g_shift: int = 0, b_shift: int = 0, **params: Any) -> np.ndarray:
         if not is_rgb_image(img):
             msg = "RGBShift transformation expects 3-channel images."
             raise TypeError(msg)
         return F.shift_rgb(img, r_shift, g_shift, b_shift)
 
@@ -1223,25 +1404,30 @@
         image
 
     Image types:
         uint8, float32
 
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        brightness_limit: SymmetricRangeType = (-0.2, 0.2)
+        contrast_limit: SymmetricRangeType = (-0.2, 0.2)
+        brightness_by_max: bool = Field(default=True, description="Adjust brightness by image dtype maximum if True.")
+
     def __init__(
         self,
-        brightness_limit: ScaleFloatType = 0.2,
-        contrast_limit: ScaleFloatType = 0.2,
+        brightness_limit: ScaleFloatType = (-0.2, 0.2),
+        contrast_limit: ScaleFloatType = (-0.2, 0.2),
         brightness_by_max: bool = True,
         always_apply: bool = False,
         p: float = 0.5,
     ):
-        super().__init__(always_apply, p)
-        self.brightness_limit = to_tuple(brightness_limit)
-        self.contrast_limit = to_tuple(contrast_limit)
+        super().__init__(always_apply=always_apply, p=p)
+        self.brightness_limit = cast(Tuple[float, float], brightness_limit)
+        self.contrast_limit = cast(Tuple[float, float], contrast_limit)
         self.brightness_by_max = brightness_by_max
 
     def apply(self, img: np.ndarray, alpha: float = 1.0, beta: float = 0.0, **params: Any) -> np.ndarray:
         return F.brightness_contrast_adjust(img, alpha, beta, self.brightness_by_max)
 
     def get_params(self) -> Dict[str, float]:
         return {
@@ -1268,40 +1454,29 @@
         image
 
     Image types:
         uint8, float32
 
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        var_limit: NonNegativeFloatRangeType = Field(default=(10.0, 50.0), description="Variance range for noise.")
+        mean: float = Field(default=0, description="Mean of the noise.")
+        per_channel: bool = Field(default=True, description="Apply noise per channel.")
+
     def __init__(
         self,
         var_limit: ScaleFloatType = (10.0, 50.0),
         mean: float = 0,
         per_channel: bool = True,
         always_apply: bool = False,
         p: float = 0.5,
     ):
-        super().__init__(always_apply, p)
-        if isinstance(var_limit, (tuple, list)):
-            if var_limit[0] < 0:
-                msg = "Lower var_limit should be non negative."
-                raise ValueError(msg)
-            if var_limit[1] < 0:
-                msg = "Upper var_limit should be non negative."
-                raise ValueError(msg)
-            self.var_limit = var_limit
-        elif isinstance(var_limit, (int, float)):
-            if var_limit < 0:
-                msg = "var_limit should be non negative."
-                raise ValueError(msg)
-
-            self.var_limit = (0, var_limit)
-        else:
-            raise TypeError(f"Expected var_limit type to be one of (int, float, tuple, list), got {type(var_limit)}")
-
+        super().__init__(always_apply=always_apply, p=p)
+        self.var_limit = cast(Tuple[float, float], var_limit)
         self.mean = mean
         self.per_channel = per_channel
 
     def apply(self, img: np.ndarray, gauss: Optional[float] = None, **params: Any) -> np.ndarray:
         return F.gauss_noise(img, gauss=gauss)
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, float]:
@@ -1309,15 +1484,15 @@
         var = random.uniform(self.var_limit[0], self.var_limit[1])
         sigma = var**0.5
 
         if self.per_channel:
             gauss = random_utils.normal(self.mean, sigma, image.shape)
         else:
             gauss = random_utils.normal(self.mean, sigma, image.shape[:2])
-            if len(image.shape) == THREE:
+            if len(image.shape) > GRAYSCALE_SHAPE_LEN:
                 gauss = np.expand_dims(gauss, -1)
 
         return {"gauss": gauss}
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["image"]
@@ -1340,22 +1515,34 @@
         image
 
     Image types:
         uint8
 
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        color_shift: Tuple[float, float] = Field(
+            default=(0.01, 0.05),
+            description=(
+                "Variance range for color hue change. Measured as a fraction of 360 degree Hue angle in HLS colorspace."
+            ),
+        )
+        intensity: Tuple[float, float] = Field(
+            default=(0.1, 0.5),
+            description="Multiplicative factor that control strength of color and luminance noise.",
+        )
+
     def __init__(
         self,
         color_shift: Tuple[float, float] = (0.01, 0.05),
         intensity: Tuple[float, float] = (0.1, 0.5),
         always_apply: bool = False,
         p: float = 0.5,
     ):
-        super().__init__(always_apply, p)
+        super().__init__(always_apply=always_apply, p=p)
         self.intensity = intensity
         self.color_shift = color_shift
 
     def apply(
         self,
         img: np.ndarray,
         color_shift: float = 0.05,
@@ -1363,17 +1550,17 @@
         random_state: Optional[int] = None,
         **params: Any,
     ) -> np.ndarray:
         return F.iso_noise(img, color_shift, intensity, np.random.RandomState(random_state))
 
     def get_params(self) -> Dict[str, Any]:
         return {
-            "color_shift": random.uniform(self.color_shift[0], self.color_shift[1]),
-            "intensity": random.uniform(self.intensity[0], self.intensity[1]),
-            "random_state": random.randint(0, 65536),
+            "color_shift": random_utils.uniform(self.color_shift[0], self.color_shift[1]),
+            "intensity": random_utils.uniform(self.intensity[0], self.intensity[1]),
+            "random_state": random_utils.randint(0, 65536),
         }
 
     def get_transform_init_args_names(self) -> Tuple[str, str]:
         return ("intensity", "color_shift")
 
 
 class CLAHE(ImageOnlyTransform):
@@ -1389,24 +1576,28 @@
         image
 
     Image types:
         uint8
 
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        clip_limit: OnePlusFloatRangeType = (1.0, 4.0)
+        tile_grid_size: OnePlusIntRangeType = (8, 8)
+
     def __init__(
         self,
         clip_limit: ScaleFloatType = 4.0,
         tile_grid_size: Tuple[int, int] = (8, 8),
         always_apply: bool = False,
         p: float = 0.5,
     ):
-        super().__init__(always_apply, p)
-        self.clip_limit = to_tuple(clip_limit, 1)
-        self.tile_grid_size = cast(Tuple[int, int], tuple(tile_grid_size))
+        super().__init__(always_apply=always_apply, p=p)
+        self.clip_limit = cast(Tuple[float, float], clip_limit)
+        self.tile_grid_size = tile_grid_size
 
     def apply(self, img: np.ndarray, clip_limit: float = 2, **params: Any) -> np.ndarray:
         if not is_rgb_image(img) and not is_grayscale_image(img):
             msg = "CLAHE transformation expects 1-channel or 3-channel images."
             raise TypeError(msg)
 
         return F.clahe(img, clip_limit, self.tile_grid_size)
@@ -1438,15 +1629,15 @@
 
     def apply(self, img: np.ndarray, channels_shuffled: Tuple[int, int, int] = (0, 1, 2), **params: Any) -> np.ndarray:
         return F.channel_shuffle(img, channels_shuffled)
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, Any]:
         img = params["image"]
         ch_arr = list(range(img.shape[2]))
-        random.shuffle(ch_arr)
+        ch_arr = random_utils.shuffle(ch_arr)
         return {"channels_shuffled": ch_arr}
 
     def get_transform_init_args_names(self) -> Tuple[()]:
         return ()
 
 
 class InvertImg(ImageOnlyTransform):
@@ -1472,16 +1663,15 @@
 
 
 class RandomGamma(ImageOnlyTransform):
     """Applies random gamma correction to an image as a form of data augmentation.
 
     This class adjusts the luminance of an image by applying gamma correction with a randomly
     selected gamma value from a specified range. Gamma correction can simulate various lighting
-    conditions, potentially enhancing model generalization. For more details on gamma correction,
-    see: https://en.wikipedia.org/wiki/Gamma_correction
+    conditions, potentially enhancing model generalization.
 
     Attributes:
         gamma_limit (Union[int, Tuple[int, int]]): The range for gamma adjustment. If `gamma_limit` is a single
             int, the range will be interpreted as (-gamma_limit, gamma_limit), defining how much
             to adjust the image's gamma. Default is (80, 120).
         always_apply (bool): If `True`, the transform will always be applied, regardless of `p`.
             Default is `False`.
@@ -1489,24 +1679,30 @@
 
     Targets:
         image
 
     Image types:
         uint8, float32
 
+    Reference:
+         https://en.wikipedia.org/wiki/Gamma_correction
+
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        gamma_limit: OnePlusFloatRangeType = (80, 120)
+
     def __init__(
         self,
         gamma_limit: ScaleIntType = (80, 120),
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
-        self.gamma_limit = to_tuple(gamma_limit)
+        self.gamma_limit = cast(Tuple[float, float], gamma_limit)
 
     def apply(self, img: np.ndarray, gamma: float = 1, **params: Any) -> np.ndarray:
         return F.gamma_transform(img, gamma=gamma)
 
     def get_params(self) -> Dict[str, float]:
         return {"gamma": random.uniform(self.gamma_limit[0], self.gamma_limit[1]) / 100.0}
 
@@ -1587,15 +1783,15 @@
         uint8, float32
 
     """
 
     def __init__(self, always_apply: bool = False, p: float = 0.5):
         super().__init__(always_apply, p)
         self.sepia_transformation_matrix = np.array(
-            [[0.393, 0.769, 0.189], [0.349, 0.686, 0.168], [0.272, 0.534, 0.131]]
+            [[0.393, 0.769, 0.189], [0.349, 0.686, 0.168], [0.272, 0.534, 0.131]],
         )
 
     def apply(self, img: np.ndarray, **params: Any) -> np.ndarray:
         if not is_rgb_image(img):
             msg = "ToSepia transformation expects 3-channel images."
             raise TypeError(msg)
         return F.linear_transformation_rgb(img, self.sepia_transformation_matrix)
@@ -1620,14 +1816,18 @@
         image
 
     Image types:
         any type
 
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        max_value: Optional[float] = Field(default=None, description="Maximum possible input value.")
+        p: ProbabilityType = 1
+
     def __init__(self, max_value: Optional[float] = None, always_apply: bool = False, p: float = 1.0):
         super().__init__(always_apply, p)
         self.max_value = max_value
 
     def apply(self, img: np.ndarray, **params: Any) -> np.ndarray:
         return F.to_float(img, self.max_value)
 
@@ -1655,18 +1855,27 @@
         float32
 
     .. _'Data types' page from the NumPy docs:
        https://docs.scipy.org/doc/numpy/user/basics.types.html
 
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        dtype: Literal["uint8", "uint16", "float32", "float64"]
+        max_value: Optional[float] = Field(default=None, description="Maximum possible input value.")
+        p: ProbabilityType = 1
+
     def __init__(
-        self, dtype: str = "uint16", max_value: Optional[float] = None, always_apply: bool = False, p: float = 1.0
+        self,
+        dtype: Literal["uint8", "uint16", "float32", "float64"] = "uint16",
+        max_value: Optional[float] = None,
+        always_apply: bool = False,
+        p: float = 1.0,
     ):
-        super().__init__(always_apply, p)
+        super().__init__(always_apply=always_apply, p=p)
         self.dtype = np.dtype(dtype)
         self.max_value = max_value
 
     def apply(self, img: np.ndarray, **params: Any) -> np.ndarray:
         return F.from_float(img, self.dtype, self.max_value)
 
     def get_transform_init_args(self) -> Dict[str, Any]:
@@ -1689,48 +1898,59 @@
         image
 
     Image types:
         uint8, float32
 
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        scale_min: float = Field(default=0.25, ge=0, le=1, description="Lower bound on the image scale.")
+        scale_max: float = Field(default=0.25, ge=0, lt=1, description="Upper bound on the image scale.")
+        interpolation: Optional[Union[int, Interpolation, Dict[str, int]]] = Field(
+            default_factory=lambda: Interpolation(downscale=cv2.INTER_NEAREST, upscale=cv2.INTER_NEAREST),
+            description="CV2 interpolation method or a dictionary specifying downscale and upscale methods.",
+        )
+
+        @model_validator(mode="after")
+        def validate_scale(self) -> Self:
+            if self.scale_min > self.scale_max:
+                msg = "scale_min must be less than or equal to scale_max"
+                raise ValueError(msg)
+            return self
+
+        @field_validator("interpolation")
+        @classmethod
+        def set_interpolation(cls, v: Any) -> Interpolation:
+            if isinstance(v, dict):
+                return Interpolation(**v)
+            if isinstance(v, int):
+                return Interpolation(downscale=v, upscale=v)
+            if isinstance(v, Interpolation):
+                return v
+            if v is None:
+                return Interpolation(downscale=cv2.INTER_NEAREST, upscale=cv2.INTER_NEAREST)
+
+            msg = (
+                "Interpolation must be an int, Interpolation instance, "
+                "or dict specifying downscale and upscale methods."
+            )
+            raise ValueError(msg)
+
     def __init__(
         self,
         scale_min: float = 0.25,
         scale_max: float = 0.25,
         interpolation: Optional[Union[int, Interpolation, Dict[str, int]]] = None,
         always_apply: bool = False,
         p: float = 0.5,
     ):
-        super().__init__(always_apply, p)
-        if interpolation is None:
-            self.interpolation = Interpolation(downscale=cv2.INTER_NEAREST, upscale=cv2.INTER_NEAREST)
-            warnings.warn(
-                "Using default interpolation INTER_NEAREST, which is sub-optimal."
-                "Please specify interpolation mode for downscale and upscale explicitly."
-                "For additional information see this PR https://github.com/albumentations-team/albumentations/pull/584"
-            )
-        elif isinstance(interpolation, int):
-            self.interpolation = Interpolation(downscale=interpolation, upscale=interpolation)
-        elif isinstance(interpolation, Interpolation):
-            self.interpolation = interpolation
-        elif isinstance(interpolation, dict):
-            self.interpolation = Interpolation(**interpolation)
-        else:
-            raise ValueError(
-                "Wrong interpolation data type. Supported types: `Optional[Union[int, Interpolation, Dict[str, int]]]`."
-                f" Got: {type(interpolation)}"
-            )
-
-        if scale_min > scale_max:
-            raise ValueError(f"Expected scale_min be less or equal scale_max, got {scale_min} {scale_max}")
-        if scale_max >= 1:
-            raise ValueError(f"Expected scale_max to be less than 1, got {scale_max}")
+        super().__init__(always_apply=always_apply, p=p)
         self.scale_min = scale_min
         self.scale_max = scale_max
+        self.interpolation = cast(Interpolation, interpolation)
 
     def apply(self, img: np.ndarray, scale: float, **params: Any) -> np.ndarray:
         if isinstance(self.interpolation, int):
             msg = "Should not be here, added for typing purposes. Please report this issue."
             raise TypeError(msg)
         return F.downscale(
             img,
@@ -1799,15 +2019,15 @@
             "bbox": bbox,
             "global_label": global_label,
         }.items():
             if custom_apply_fn is not None:
                 if isinstance(custom_apply_fn, LambdaType) and custom_apply_fn.__name__ == "<lambda>":
                     warnings.warn(
                         "Using lambda is incompatible with multiprocessing. "
-                        "Consider using regular functions or partial()."
+                        "Consider using regular functions or partial().",
                     )
 
                 self.custom_apply_fns[target_name] = custom_apply_fn
 
     def apply(self, img: np.ndarray, **params: Any) -> np.ndarray:
         fn = self.custom_apply_fns["image"]
         return fn(img, **params)
@@ -1863,24 +2083,29 @@
         image
 
     Image types:
         Any
 
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        multiplier: NonNegativeFloatRangeType = (0.9, 1.1)
+        per_channel: bool = Field(default=False, description="Apply multiplier per channel.")
+        elementwise: bool = Field(default=False, description="Apply multiplier element-wise to pixels.")
+
     def __init__(
         self,
         multiplier: ScaleFloatType = (0.9, 1.1),
         per_channel: bool = False,
         elementwise: bool = False,
         always_apply: bool = False,
         p: float = 0.5,
     ):
-        super().__init__(always_apply, p)
-        self.multiplier = to_tuple(multiplier, multiplier)
+        super().__init__(always_apply=always_apply, p=p)
+        self.multiplier = cast(Tuple[float, float], multiplier)
         self.per_channel = per_channel
         self.elementwise = elementwise
 
     def apply(self, img: np.ndarray, multiplier: float = np.array([1]), **kwargs: Any) -> np.ndarray:
         return F.multiply(img, multiplier)
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, Any]:
@@ -1892,15 +2117,15 @@
         height, width = img.shape[:2]
 
         num_channels = (1 if is_grayscale_image(img) else img.shape[-1]) if self.per_channel else 1
 
         shape = [height, width, num_channels] if self.elementwise else [num_channels]
 
         multiplier = random_utils.uniform(self.multiplier[0], self.multiplier[1], tuple(shape))
-        if is_grayscale_image(img) and img.ndim == TWO:
+        if is_grayscale_image(img) and img.ndim == GRAYSCALE_SHAPE_LEN:
             multiplier = np.squeeze(multiplier)
 
         return {"multiplier": multiplier}
 
     @property
     def targets_as_params(self) -> List[str]:
         return ["image"]
@@ -1926,14 +2151,17 @@
     Credit:
         http://papers.nips.cc/paper/4824-imagenet-classification-with-deep-convolutional-neural-networks.pdf
         https://deshanadesai.github.io/notes/Fancy-PCA-with-Scikit-Image
         https://pixelatedbrian.github.io/2018-04-29-fancy_pca/
 
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        alpha: float = Field(default=0.1, description="Scale for perturbing the eigen vectors and values", ge=0)
+
     def __init__(self, alpha: float = 0.1, always_apply: bool = False, p: float = 0.5):
         super().__init__(always_apply=always_apply, p=p)
         self.alpha = alpha
 
     def apply(self, img: np.ndarray, alpha: float = 0.1, **params: Any) -> np.ndarray:
         return F.fancy_pca(img, alpha)
 
@@ -1948,81 +2176,92 @@
     """Randomly changes the brightness, contrast, and saturation of an image. Compared to ColorJitter from torchvision,
     this transform gives a little bit different results because Pillow (used in torchvision) and OpenCV (used in
     Albumentations) transform an image to HSV format by different formulas. Another difference - Pillow uses uint8
     overflow, but we use value saturation.
 
     Args:
         brightness (float or tuple of float (min, max)): How much to jitter brightness.
-            brightness_factor is chosen uniformly from [max(0, 1 - brightness), 1 + brightness]
-            or the given [min, max]. Should be non negative numbers.
+            If float:
+                brightness_factor is chosen uniformly from [max(0, 1 - brightness), 1 + brightness]
+            If Tuple[float, float]] will be sampled from that range. Both values should be non negative numbers.
         contrast (float or tuple of float (min, max)): How much to jitter contrast.
-            contrast_factor is chosen uniformly from [max(0, 1 - contrast), 1 + contrast]
-            or the given [min, max]. Should be non negative numbers.
+            If float:
+                contrast_factor is chosen uniformly from [max(0, 1 - brightness), 1 + brightness]
+            If Tuple[float, float]] will be sampled from that range. Both values should be non negative numbers.
         saturation (float or tuple of float (min, max)): How much to jitter saturation.
-            saturation_factor is chosen uniformly from [max(0, 1 - saturation), 1 + saturation]
-            or the given [min, max]. Should be non negative numbers.
+            If float:
+               saturation_factor is chosen uniformly from [max(0, 1 - brightness), 1 + brightness]
+            If Tuple[float, float]] will be sampled from that range. Both values should be non negative numbers.
         hue (float or tuple of float (min, max)): How much to jitter hue.
-            hue_factor is chosen uniformly from [-hue, hue] or the given [min, max].
-            Should have 0 <= hue <= 0.5 or -0.5 <= min <= max <= 0.5.
+            If float:
+               saturation_factor is chosen uniformly from [-hue, hue]. Should have 0 <= hue <= 0.5.
+            If Tuple[float, float]] will be sampled from that range. Both values should be in range [-0.5, 0.5].
 
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        brightness: Annotated[ScaleFloatType, Field(default=0.2, description="Range for jittering brightness.")]
+        contrast: Annotated[ScaleFloatType, Field(default=0.2, description="Range for jittering contrast.")]
+        saturation: Annotated[ScaleFloatType, Field(default=0.2, description="Range for jittering saturation.")]
+        hue: Annotated[ScaleFloatType, Field(default=0.2, description="Range for jittering hue.")]
+
+        @field_validator("brightness", "contrast", "saturation", "hue")
+        @classmethod
+        def check_ranges(cls, value: ScaleFloatType, info: ValidationInfo) -> Tuple[float, float]:
+            if info.field_name == "hue":
+                bounds = -0.5, 0.5
+                bias = 0
+                clip = False
+            elif info.field_name in ["brightness", "contrast", "saturation"]:
+                bounds = 0, float("inf")
+                bias = 1
+                clip = True
+
+            if isinstance(value, numbers.Number):
+                if value < 0:
+                    raise ValueError(f"If {info.field_name} is a single number, it must be non negative.")
+                value = [bias - value, bias + value]
+                if clip:
+                    value[0] = max(value[0], 0)
+            elif isinstance(value, (tuple, list)) and len(value) == PAIR:
+                check_range(value, *bounds, info.field_name)
+
+            return cast(Tuple[float, float], value)
+
     def __init__(
         self,
-        brightness: ScaleFloatType = 0.2,
-        contrast: ScaleFloatType = 0.2,
-        saturation: ScaleFloatType = 0.2,
-        hue: ScaleFloatType = 0.2,
+        brightness: ScaleFloatType = (0.8, 1),
+        contrast: ScaleFloatType = (0.8, 1),
+        saturation: ScaleFloatType = (0.8, 1),
+        hue: ScaleFloatType = (-0.5, 0.5),
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply=always_apply, p=p)
 
-        self.brightness = self.__check_values(brightness, "brightness")
-        self.contrast = self.__check_values(contrast, "contrast")
-        self.saturation = self.__check_values(saturation, "saturation")
-        self.hue = self.__check_values(hue, "hue", offset=0, bounds=(-0.5, 0.5), clip=False)
+        self.brightness = cast(Tuple[float, float], brightness)
+        self.contrast = cast(Tuple[float, float], contrast)
+        self.saturation = cast(Tuple[float, float], saturation)
+        self.hue = cast(Tuple[float, float], hue)
 
         self.transforms = [
             F.adjust_brightness_torchvision,
             F.adjust_contrast_torchvision,
             F.adjust_saturation_torchvision,
             F.adjust_hue_torchvision,
         ]
 
-    @staticmethod
-    def __check_values(
-        value: ScaleFloatType,
-        name: str,
-        offset: float = 1,
-        bounds: Tuple[float, float] = (0, float("inf")),
-        clip: bool = True,
-    ) -> Tuple[float, float]:
-        if isinstance(value, numbers.Number):
-            if value < 0:
-                raise ValueError(f"If {name} is a single number, it must be non negative.")
-            value = [offset - value, offset + value]
-            if clip:
-                value[0] = max(value[0], 0)
-        elif isinstance(value, (tuple, list)) and len(value) == TWO:
-            if not bounds[0] <= value[0] <= value[1] <= bounds[1]:
-                raise ValueError(f"{name} values should be between {bounds}")
-        else:
-            raise TypeError(f"{name} should be a single number or a list/tuple with length 2.")
-
-        return value
-
     def get_params(self) -> Dict[str, Any]:
         brightness = random.uniform(self.brightness[0], self.brightness[1])
         contrast = random.uniform(self.contrast[0], self.contrast[1])
         saturation = random.uniform(self.saturation[0], self.saturation[1])
         hue = random.uniform(self.hue[0], self.hue[1])
 
         order = [0, 1, 2, 3]
-        random.shuffle(order)
+        order = random_utils.shuffle(order)
 
         return {
             "brightness": brightness,
             "contrast": contrast,
             "saturation": saturation,
             "hue": hue,
             "order": order,
@@ -2062,32 +2301,28 @@
         p: probability of applying the transform. Default: 0.5.
 
     Targets:
         image
 
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        alpha: ZeroOneRangeType = (0.2, 0.5)
+        lightness: NonNegativeFloatRangeType = (0.5, 1.0)
+
     def __init__(
         self,
         alpha: Tuple[float, float] = (0.2, 0.5),
         lightness: Tuple[float, float] = (0.5, 1.0),
         always_apply: bool = False,
         p: float = 0.5,
     ):
-        super().__init__(always_apply, p)
-        self.alpha = self.__check_values(to_tuple(alpha, 0.0), name="alpha", bounds=(0.0, 1.0))
-        self.lightness = self.__check_values(to_tuple(lightness, 0.0), name="lightness")
-
-    @staticmethod
-    def __check_values(
-        value: Tuple[float, float], name: str, bounds: Tuple[float, float] = (0, float("inf"))
-    ) -> Tuple[float, float]:
-        if not bounds[0] <= value[0] <= value[1] <= bounds[1]:
-            raise ValueError(f"{name} values should be between {bounds}")
-        return value
+        super().__init__(always_apply=always_apply, p=p)
+        self.alpha = alpha
+        self.lightness = lightness
 
     @staticmethod
     def __generate_sharpening_matrix(alpha_sample: np.ndarray, lightness_sample: np.ndarray) -> np.ndarray:
         matrix_nochange = np.array([[0, 0, 0], [0, 1, 0], [0, 0, 0]], dtype=np.float32)
         matrix_effect = np.array(
             [[-1, -1, -1], [-1, 8 + lightness_sample, -1], [-1, -1, -1]],
             dtype=np.float32,
@@ -2118,32 +2353,28 @@
         p: probability of applying the transform. Default: 0.5.
 
     Targets:
         image
 
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        alpha: ZeroOneRangeType = (0.2, 0.5)
+        strength: NonNegativeFloatRangeType = (0.2, 0.7)
+
     def __init__(
         self,
         alpha: Tuple[float, float] = (0.2, 0.5),
         strength: Tuple[float, float] = (0.2, 0.7),
         always_apply: bool = False,
         p: float = 0.5,
     ):
-        super().__init__(always_apply, p)
-        self.alpha = self.__check_values(to_tuple(alpha, 0.0), name="alpha", bounds=(0.0, 1.0))
-        self.strength = self.__check_values(to_tuple(strength, 0.0), name="strength")
-
-    @staticmethod
-    def __check_values(
-        value: Tuple[float, float], name: str, bounds: Tuple[float, float] = (0, float("inf"))
-    ) -> Tuple[float, float]:
-        if not bounds[0] <= value[0] <= value[1] <= bounds[1]:
-            raise ValueError(f"{name} values should be between {bounds}")
-        return value
+        super().__init__(always_apply=always_apply, p=p)
+        self.alpha = alpha
+        self.strength = strength
 
     @staticmethod
     def __generate_emboss_matrix(alpha_sample: np.ndarray, strength_sample: np.ndarray) -> np.ndarray:
         matrix_nochange = np.array([[0, 0, 0], [0, 1, 0], [0, 0, 0]], dtype=np.float32)
         matrix_effect = np.array(
             [
                 [-1 - strength_sample, 0 - strength_sample, 0],
@@ -2184,21 +2415,20 @@
                 * A probability of ``1.0`` would mean, that all segments are
                   replaced by their average color (resulting in a voronoi
                   image).
             Behaviour based on chosen data types for this parameter:
                 * If a ``float``, then that ``flat`` will always be used.
                 * If ``tuple`` ``(a, b)``, then a random probability will be
                   sampled from the interval ``[a, b]`` per image.
-        n_segments (int, or tuple of int): Rough target number of how many superpixels to generate (the algorithm
+        n_segments (tuple of int): Rough target number of how many superpixels to generate (the algorithm
             may deviate from this number). Lower value will lead to coarser superpixels.
             Higher values are computationally more intensive and will hence lead to a slowdown
-            * If a single ``int``, then that value will always be used as the
-              number of segments.
-            * If a ``tuple`` ``(a, b)``, then a value from the discrete
-              interval ``[a..b]`` will be sampled per image.
+            Then a value from the discrete interval ``[a..b]`` will be sampled per image.
+            If input is a single integer, the range will be ``(1, n_segments)``.
+            If interested in a fixed number of segments, use ``(n_segments, n_segments)``.
         max_size (int or None): Maximum image size at which the augmentation is performed.
             If the width or height of an image exceeds this value, it will be
             downscaled before the augmentation so that the longest side matches `max_size`.
             This is done to speed up the process. The final output image has the same size as the input image.
             Note that in case `p_replace` is below ``1.0``,
             the down-/upscaling will affect the not-replaced pixels too.
             Use ``None`` to apply no down-/upscaling.
@@ -2208,80 +2438,112 @@
         p (float): probability of applying the transform. Default: 0.5.
 
     Targets:
         image
 
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        p_replace: ZeroOneRangeType = (0, 0.1)
+        n_segments: OnePlusIntRangeType = (100, 100)
+        max_size: Optional[int] = Field(default=128, ge=1, description="Maximum image size for the transformation.")
+        interpolation: InterpolationType = cv2.INTER_LINEAR
+
     def __init__(
         self,
-        p_replace: ScaleFloatType = 0.1,
-        n_segments: ScaleIntType = 100,
+        p_replace: ScaleFloatType = (0, 0.1),
+        n_segments: ScaleIntType = (100, 100),
         max_size: Optional[int] = 128,
         interpolation: int = cv2.INTER_LINEAR,
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply=always_apply, p=p)
-        self.p_replace = to_tuple(p_replace, p_replace)
-        self.n_segments = to_tuple(n_segments, n_segments)
+        self.p_replace = cast(Tuple[float, float], p_replace)
+        self.n_segments = cast(Tuple[int, int], n_segments)
         self.max_size = max_size
         self.interpolation = interpolation
 
-        if min(self.n_segments) < 1:
-            raise ValueError(f"n_segments must be >= 1. Got: {n_segments}")
-
     def get_transform_init_args_names(self) -> Tuple[str, str, str, str]:
         return ("p_replace", "n_segments", "max_size", "interpolation")
 
     def get_params(self) -> Dict[str, Any]:
-        n_segments = random.randint(*self.n_segments)
+        n_segments = random_utils.randint(self.n_segments[0], self.n_segments[1] + 1)
         p = random.uniform(*self.p_replace)
         return {"replace_samples": random_utils.random(n_segments) < p, "n_segments": n_segments}
 
     def apply(
-        self, img: np.ndarray, replace_samples: Sequence[bool] = (False,), n_segments: int = 1, **kwargs: Any
+        self,
+        img: np.ndarray,
+        replace_samples: Sequence[bool] = (False,),
+        n_segments: int = 1,
+        **kwargs: Any,
     ) -> np.ndarray:
         return F.superpixels(img, n_segments, replace_samples, self.max_size, cast(int, self.interpolation))
 
 
 class TemplateTransform(ImageOnlyTransform):
     """Apply blending of input image with specified templates
     Args:
         templates (numpy array or list of numpy arrays): Images as template for transform.
-        img_weight: If single float will be used as weight for input image.
-            If tuple of float img_weight will be in range `[img_weight[0], img_weight[1])`. Default: 0.5.
-        template_weight: If single float will be used as weight for template.
+        img_weight: If single float weight will be sampled from (0, img_weight).
+            If tuple of float img_weight will be in range `[img_weight[0], img_weight[1])`.
+            If you want fixed weight, use (img_weight, img_weight)
+            Default: (0.5, 0.5).
+        template_weight: If single float weight will be sampled from (0, template_weight).
             If tuple of float template_weight will be in range `[template_weight[0], template_weight[1])`.
-            Default: 0.5.
+            If you want fixed weight, use (template_weight, template_weight)
+            Default: (0.5, 0.5).
         template_transform: transformation object which could be applied to template,
             must produce template the same size as input image.
         name: (Optional) Name of transform, used only for deserialization.
         p: probability of applying the transform. Default: 0.5.
     Targets:
         image
     Image types:
         uint8, float32
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        templates: Union[np.ndarray, Sequence[np.ndarray]] = Field(..., description="Images as template for transform.")
+        img_weight: ZeroOneRangeType = (0.5, 0.5)
+        template_weight: ZeroOneRangeType = (0.5, 0.5)
+        template_transform: Optional[Callable[..., Any]] = Field(
+            default=None,
+            description="Transformation object applied to template.",
+        )
+        name: Optional[str] = Field(default=None, description="Name of transform, used only for deserialization.")
+
+        @field_validator("templates")
+        @classmethod
+        def validate_templates(cls, v: Union[np.ndarray, List[np.ndarray]]) -> List[np.ndarray]:
+            if isinstance(v, np.ndarray):
+                return [v]
+            if isinstance(v, list):
+                if not all(isinstance(item, np.ndarray) for item in v):
+                    msg = "All templates must be numpy arrays."
+                    raise ValueError(msg)
+                return v
+            msg = "Templates must be a numpy array or a list of numpy arrays."
+            raise TypeError(msg)
+
     def __init__(
         self,
         templates: Union[np.ndarray, List[np.ndarray]],
-        img_weight: ScaleFloatType = 0.5,
-        template_weight: ScaleFloatType = 0.5,
+        img_weight: ScaleFloatType = (0.5, 0.5),
+        template_weight: ScaleFloatType = (0.5, 0.5),
         template_transform: Optional[Callable[..., Any]] = None,
         name: Optional[str] = None,
         always_apply: bool = False,
         p: float = 0.5,
     ):
-        super().__init__(always_apply, p)
-
-        self.templates = templates if isinstance(templates, (list, tuple)) else [templates]
-        self.img_weight = to_tuple(img_weight, img_weight)
-        self.template_weight = to_tuple(template_weight, template_weight)
+        super().__init__(always_apply=always_apply, p=p)
+        self.templates = templates
+        self.img_weight = cast(Tuple[float, float], img_weight)
+        self.template_weight = cast(Tuple[float, float], template_weight)
         self.template_transform = template_transform
         self.name = name
 
     def apply(
         self,
         img: np.ndarray,
         template: Optional[np.ndarray] = None,
@@ -2361,32 +2623,36 @@
         https://arxiv.org/abs/2107.10833
 
     Targets:
         image
 
     """
 
+    class InitSchema(BlurInitSchema):
+        blur_limit: ScaleIntType = Field(default=(7, 15), description="Maximum kernel size for sinc filter.")
+        cutoff: ScaleFloatType = Field(default=(np.pi / 4, np.pi / 2), description="Cutoff frequency range in radians.")
+
+        @field_validator("cutoff")
+        @classmethod
+        def check_cutoff(cls, v: ScaleFloatType, info: ValidationInfo) -> Tuple[float, float]:
+            bounds = 0, np.pi
+            result = to_tuple(v, v)
+            check_range(result, *bounds, info.field_name)
+            return result
+
     def __init__(
         self,
         blur_limit: ScaleIntType = (7, 15),
         cutoff: ScaleFloatType = (np.pi / 4, np.pi / 2),
         always_apply: bool = False,
         p: float = 0.5,
     ):
-        super().__init__(always_apply, p)
-        self.blur_limit = cast(Tuple[int, int], to_tuple(blur_limit, 3))
-        self.cutoff = self.__check_values(to_tuple(cutoff, np.pi / 2), name="cutoff", bounds=(0, np.pi))
-
-    @staticmethod
-    def __check_values(
-        value: Tuple[float, float], name: str, bounds: Tuple[float, float] = (0, float("inf"))
-    ) -> Tuple[float, float]:
-        if not bounds[0] <= value[0] <= value[1] <= bounds[1]:
-            raise ValueError(f"{name} values should be between {bounds}")
-        return value
+        super().__init__(always_apply=always_apply, p=p)
+        self.blur_limit = cast(Tuple[int, int], blur_limit)
+        self.cutoff = cast(Tuple[float, float], cutoff)
 
     def get_params(self) -> Dict[str, np.ndarray]:
         ksize = random.randrange(self.blur_limit[0], self.blur_limit[1] + 1, 2)
         if ksize % 2 == 0:
             raise ValueError(f"Kernel size must be odd. Got: {ksize}")
 
         cutoff = random.uniform(*self.cutoff)
@@ -2437,48 +2703,44 @@
         arxiv.org/pdf/2107.10833.pdf
 
     Targets:
         image
 
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        sigma_limit: NonNegativeFloatRangeType = 0
+        alpha: ZeroOneRangeType = (0.2, 0.5)
+        threshold: int = Field(default=10, ge=0, le=255, description="Threshold for limiting sharpening.")
+
+        blur_limit: ScaleIntType = Field(
+            default=(3, 7),
+            description="Maximum kernel size for blurring the input image.",
+        )
+
+        @field_validator("blur_limit")
+        @classmethod
+        def process_blur(cls, value: ScaleIntType, info: ValidationInfo) -> Tuple[int, int]:
+            return process_blur_limit(value, info, min_value=3)
+
     def __init__(
         self,
         blur_limit: ScaleIntType = (3, 7),
         sigma_limit: ScaleFloatType = 0.0,
         alpha: ScaleFloatType = (0.2, 0.5),
         threshold: int = 10,
         always_apply: bool = False,
         p: float = 0.5,
     ):
-        super().__init__(always_apply, p)
-        self.blur_limit = cast(Tuple[int, int], to_tuple(blur_limit, 3))
-        self.sigma_limit = self.__check_values(to_tuple(sigma_limit, 0.0), name="sigma_limit")
-        self.alpha = self.__check_values(to_tuple(alpha, 0.0), name="alpha", bounds=(0.0, 1.0))
+        super().__init__(always_apply=always_apply, p=p)
+        self.blur_limit = cast(Tuple[int, int], blur_limit)
+        self.sigma_limit = cast(Tuple[float, float], sigma_limit)
+        self.alpha = cast(Tuple[float, float], alpha)
         self.threshold = threshold
 
-        if self.blur_limit[0] == 0 and self.sigma_limit[0] == 0:
-            self.blur_limit = 3, max(3, self.blur_limit[1])
-            msg = "blur_limit and sigma_limit minimum value can not be both equal to 0."
-            raise ValueError(msg)
-
-        if (self.blur_limit[0] != 0 and self.blur_limit[0] % 2 != 1) or (
-            self.blur_limit[1] != 0 and self.blur_limit[1] % 2 != 1
-        ):
-            msg = "UnsharpMask supports only odd blur limits."
-            raise ValueError(msg)
-
-    @staticmethod
-    def __check_values(
-        value: Union[Tuple[int, int], Tuple[float, float]], name: str, bounds: Tuple[float, float] = (0, float("inf"))
-    ) -> Tuple[float, float]:
-        if not bounds[0] <= value[0] <= value[1] <= bounds[1]:
-            raise ValueError(f"{name} values should be between {bounds}")
-        return value
-
     def get_params(self) -> Dict[str, Any]:
         return {
             "ksize": random.randrange(self.blur_limit[0], self.blur_limit[1] + 1, 2),
             "sigma": random.uniform(*self.sigma_limit),
             "alpha": random.uniform(*self.alpha),
         }
 
@@ -2510,49 +2772,64 @@
     Targets:
         image, mask
     Image types:
         any
 
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        dropout_prob: ProbabilityType = 0.01
+        per_channel: bool = Field(default=False, description="Sample drop mask per channel.")
+        drop_value: Optional[ScaleFloatType] = Field(
+            default=0,
+            description="Value to set in dropped pixels. None for random sampling.",
+        )
+        mask_drop_value: Optional[ScaleFloatType] = Field(
+            default=None,
+            description="Value to set in dropped pixels in masks. None to leave masks unchanged.",
+        )
+
+        @model_validator(mode="after")
+        def validate_mask_drop_value(self) -> Self:
+            if self.mask_drop_value is not None and self.per_channel:
+                msg = "PixelDropout supports mask only with per_channel=False."
+                raise ValueError(msg)
+            return self
+
     _targets = (Targets.IMAGE, Targets.MASK)
 
     def __init__(
         self,
         dropout_prob: float = 0.01,
         per_channel: bool = False,
         drop_value: Optional[ScaleFloatType] = 0,
         mask_drop_value: Optional[ScaleFloatType] = None,
         always_apply: bool = False,
         p: float = 0.5,
     ):
-        super().__init__(always_apply, p)
+        super().__init__(always_apply=always_apply, p=p)
         self.dropout_prob = dropout_prob
         self.per_channel = per_channel
         self.drop_value = drop_value
         self.mask_drop_value = mask_drop_value
 
-        if self.mask_drop_value is not None and self.per_channel:
-            msg = "PixelDropout supports mask only with per_channel=False"
-            raise ValueError(msg)
-
     def apply(
         self,
         img: np.ndarray,
         drop_mask: Optional[np.ndarray] = None,
         drop_value: Union[float, Sequence[float]] = (),
         **params: Any,
     ) -> np.ndarray:
         return F.pixel_dropout(img, drop_mask, drop_value)
 
     def apply_to_mask(self, mask: np.ndarray, drop_mask: Optional[np.ndarray] = None, **params: Any) -> np.ndarray:
         if self.mask_drop_value is None:
             return mask
 
-        if mask.ndim == TWO:
+        if mask.ndim == GRAYSCALE_SHAPE_LEN:
             drop_mask = np.squeeze(drop_mask)
 
         return F.pixel_dropout(mask, drop_mask, self.mask_drop_value)
 
     def apply_to_bbox(self, bbox: BoxInternalType, **params: Any) -> BoxInternalType:
         return bbox
 
@@ -2593,29 +2870,39 @@
 
 
 class Spatter(ImageOnlyTransform):
     """Apply spatter transform. It simulates corruption which can occlude a lens in the form of rain or mud.
 
     Args:
         mean (float, or tuple of floats): Mean value of normal distribution for generating liquid layer.
-            If single float it will be used as mean.
-            If tuple of float mean will be sampled from range `[mean[0], mean[1])`. Default: (0.65).
+            If single float mean will be sampled from `(0, mean)`
+            If tuple of float mean will be sampled from range `(mean[0], mean[1])`.
+            If you want constant value use (mean, mean).
+            Default (0.65, 0.65)
         std (float, or tuple of floats): Standard deviation value of normal distribution for generating liquid layer.
-            If single float it will be used as std.
-            If tuple of float std will be sampled from range `[std[0], std[1])`. Default: (0.3).
+            If single float the number will be sampled from `(0, std)`.
+            If tuple of float std will be sampled from range `(std[0], std[1])`.
+            If you want constant value use (std, std).
+            Default: (0.3, 0.3).
         gauss_sigma (float, or tuple of floats): Sigma value for gaussian filtering of liquid layer.
-            If single float it will be used as gauss_sigma.
-            If tuple of float gauss_sigma will be sampled from range `[sigma[0], sigma[1])`. Default: (2).
+            If single float the number will be sampled from `(0, gauss_sigma)`.
+            If tuple of float gauss_sigma will be sampled from range `(gauss_sigma[0], gauss_sigma[1])`.
+            If you want constant value use (gauss_sigma, gauss_sigma).
+            Default: (2, 3).
         cutout_threshold (float, or tuple of floats): Threshold for filtering liqued layer
             (determines number of drops). If single float it will used as cutout_threshold.
-            If tuple of float cutout_threshold will be sampled from range `[cutout_threshold[0], cutout_threshold[1])`.
-            Default: (0.68).
+            If single float the number will be sampled from `(0, cutout_threshold)`.
+            If tuple of float cutout_threshold will be sampled from range `(cutout_threshold[0], cutout_threshold[1])`.
+            If you want constant value use `(cutout_threshold, cutout_threshold)`.
+            Default: (0.68, 0.68).
         intensity (float, or tuple of floats): Intensity of corruption.
-            If single float it will be used as intensity.
-            If tuple of float intensity will be sampled from range `[intensity[0], intensity[1])`. Default: (0.6).
+            If single float the number will be sampled from `(0, intensity)`.
+            If tuple of float intensity will be sampled from range `(intensity[0], intensity[1])`.
+            If you want constant value use `(intensity, intensity)`.
+            Default: (0.6, 0.6).
         mode (string, or list of strings): Type of corruption. Currently, supported options are 'rain' and 'mud'.
              If list is provided type of corruption will be sampled list. Default: ("rain").
         color (list of (r, g, b) or dict or None): Corruption elements color.
             If list uses provided list as color for specified mode.
             If dict uses provided color for specified mode. Color for each specified mode should be provided in dict.
             If None uses default colors (rain: (238, 238, 175), mud: (20, 42, 63)).
         p (float): probability of applying the transform. Default: 0.5.
@@ -2623,66 +2910,81 @@
     Targets:
         image
 
     Image types:
         uint8, float32
 
     Reference:
-    |  https://arxiv.org/pdf/1903.12261.pdf
-    |  https://github.com/hendrycks/robustness/blob/master/ImageNet-C/create_c/make_imagenet_c.py
+        https://arxiv.org/abs/1903.12261
+        https://github.com/hendrycks/robustness/blob/master/ImageNet-C/create_c/make_imagenet_c.py
 
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        mean: ZeroOneRangeType = (0.65, 0.65)
+        std: ZeroOneRangeType = (0.3, 0.3)
+        gauss_sigma: NonNegativeFloatRangeType = (2, 2)
+        cutout_threshold: ZeroOneRangeType = (0.68, 0.68)
+        intensity: ZeroOneRangeType = (0.6, 0.6)
+        mode: Union[SpatterMode, Sequence[SpatterMode]] = Field(
+            default="rain",
+            description="Type of corruption ('rain', 'mud').",
+        )
+        color: Optional[Union[Sequence[int], Dict[str, Sequence[int]]]] = None
+
+        @field_validator("mode")
+        @classmethod
+        def check_mode(cls, mode: Union[SpatterMode, Sequence[SpatterMode]]) -> Sequence[SpatterMode]:
+            if isinstance(mode, str):
+                return [mode]
+            return mode
+
+        @model_validator(mode="after")
+        def check_color(self) -> Self:
+            if self.color is None:
+                self.color = {"rain": [238, 238, 175], "mud": [20, 42, 63]}
+
+            elif isinstance(self.color, (list, tuple)) and len(self.mode) == 1:
+                if len(self.color) != NUM_RGB_CHANNELS:
+                    msg = "Color must be a list of three integers for RGB format."
+                    raise ValueError(msg)
+                self.color = {self.mode[0]: self.color}
+            elif isinstance(self.color, dict):
+                result = {}
+                for mode in self.mode:
+                    if mode not in self.color:
+                        raise ValueError(f"Color for mode {mode} is not specified.")
+                    if len(self.color[mode]) != NUM_RGB_CHANNELS:
+                        raise ValueError(f"Color for mode {mode} must be in RGB format.")
+                    result[mode] = self.color[mode]
+            else:
+                msg = "Color must be a list of RGB values or a dict mapping mode to RGB values."
+                raise ValueError(msg)
+            return self
+
     def __init__(
         self,
-        mean: ScaleFloatType = 0.65,
-        std: ScaleFloatType = 0.3,
-        gauss_sigma: ScaleFloatType = 2,
-        cutout_threshold: ScaleFloatType = 0.68,
-        intensity: ScaleFloatType = 0.6,
+        mean: ScaleFloatType = (0.65, 0.65),
+        std: ScaleFloatType = (0.3, 0.3),
+        gauss_sigma: ScaleFloatType = (2, 2),
+        cutout_threshold: ScaleFloatType = (0.68, 0.68),
+        intensity: ScaleFloatType = (0.6, 0.6),
         mode: Union[SpatterMode, Sequence[SpatterMode]] = "rain",
         color: Optional[Union[Sequence[int], Dict[str, Sequence[int]]]] = None,
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply=always_apply, p=p)
-
-        self.mean = to_tuple(mean, mean)
-        self.std = to_tuple(std, std)
-        self.gauss_sigma = to_tuple(gauss_sigma, gauss_sigma)
-        self.intensity = to_tuple(intensity, intensity)
-        self.cutout_threshold = to_tuple(cutout_threshold, cutout_threshold)
-        self.color = (
-            color
-            if color is not None
-            else {
-                "rain": [238, 238, 175],
-                "mud": [20, 42, 63],
-            }
-        )
-        self.mode = mode if isinstance(mode, (list, tuple)) else [mode]
-
-        if len(set(self.mode)) > 1 and not isinstance(self.color, dict):
-            raise ValueError(f"Unsupported color: {self.color}. Please specify color for each mode (use dict for it).")
-
-        for i in self.mode:
-            if i not in ["rain", "mud"]:
-                raise ValueError(f"Unsupported color mode: {mode}. Transform supports only `rain` and `mud` mods.")
-            if isinstance(self.color, dict):
-                if i not in self.color:
-                    raise ValueError(f"Wrong color definition: {self.color}. Color for mode: {i} not specified.")
-                if len(self.color[i]) != THREE:
-                    raise ValueError(
-                        f"Unsupported color: {self.color[i]} for mode {i}. Color should be presented in RGB format."
-                    )
-
-        if isinstance(self.color, (list, tuple)):
-            if len(self.color) != THREE:
-                raise ValueError(f"Unsupported color: {self.color}. Color should be presented in RGB format.")
-            self.color = {self.mode[0]: self.color}
+        self.mean = cast(Tuple[float, float], mean)
+        self.std = cast(Tuple[float, float], std)
+        self.gauss_sigma = cast(Tuple[float, float], gauss_sigma)
+        self.cutout_threshold = cast(Tuple[float, float], cutout_threshold)
+        self.intensity = cast(Tuple[float, float], intensity)
+        self.mode = mode
+        self.color = cast(Dict[str, Sequence[int]], color)
 
     def apply(
         self,
         img: np.ndarray,
         non_mud: Optional[np.ndarray] = None,
         mud: Optional[np.ndarray] = None,
         drops: Optional[np.ndarray] = None,
@@ -2779,39 +3081,35 @@
         image
 
     Image types:
         uint8, float32
 
     """
 
+    class InitSchema(BaseTransformInitSchema):
+        primary_distortion_limit: SymmetricRangeType = (-0.02, 0.02)
+        secondary_distortion_limit: SymmetricRangeType = (-0.05, 0.05)
+        mode: ChromaticAberrationMode = Field(default="green_purple", description="Type of color fringing.")
+        interpolation: InterpolationType = cv2.INTER_LINEAR
+
     def __init__(
         self,
-        primary_distortion_limit: ScaleFloatType = 0.02,
-        secondary_distortion_limit: ScaleFloatType = 0.05,
+        primary_distortion_limit: ScaleFloatType = (-0.02, 0.02),
+        secondary_distortion_limit: ScaleFloatType = (-0.05, 0.05),
         mode: ChromaticAberrationMode = "green_purple",
         interpolation: int = cv2.INTER_LINEAR,
         always_apply: bool = False,
         p: float = 0.5,
     ):
-        super().__init__(always_apply, p)
-        self.primary_distortion_limit = to_tuple(primary_distortion_limit)
-        self.secondary_distortion_limit = to_tuple(secondary_distortion_limit)
-        self.mode = self._validate_mode(mode)
+        super().__init__(always_apply=always_apply, p=p)
+        self.primary_distortion_limit = cast(Tuple[float, float], primary_distortion_limit)
+        self.secondary_distortion_limit = cast(Tuple[float, float], secondary_distortion_limit)
+        self.mode = mode
         self.interpolation = interpolation
 
-    @staticmethod
-    def _validate_mode(
-        mode: ChromaticAberrationMode,
-    ) -> ChromaticAberrationMode:
-        valid_modes = ["green_purple", "red_blue", "random"]
-        if mode not in valid_modes:
-            msg = f"Unsupported mode: {mode}. Supported modes are 'green_purple', 'red_blue', 'random'."
-            raise ValueError(msg)
-        return mode
-
     def apply(
         self,
         img: np.ndarray,
         primary_distortion_red: float = -0.02,
         secondary_distortion_red: float = -0.05,
         primary_distortion_blue: float = -0.02,
         secondary_distortion_blue: float = -0.05,
@@ -2851,22 +3149,22 @@
             "secondary_distortion_blue": secondary_distortion_blue,
         }
 
     @staticmethod
     def _match_sign(a: float, b: float) -> float:
         # Match the sign of b to a
         if (a < 0 < b) or (a > 0 > b):
-            b = -b
+            return -b
         return b
 
     @staticmethod
     def _unmatch_sign(a: float, b: float) -> float:
         # Unmatch the sign of b to a
         if (a < 0 and b < 0) or (a > 0 and b > 0):
-            b = -b
+            return -b
         return b
 
     def get_transform_init_args_names(self) -> Tuple[str, str, str, str]:
         return "primary_distortion_limit", "secondary_distortion_limit", "mode", "interpolation"
 
 
 class Morphological(DualTransform):
@@ -2906,34 +3204,35 @@
         >>>     A.Morphological(scale=(2, 3), operation='dilation', p=0.5)
         >>> ])
         >>> image = transform(image=image)["image"]
     """
 
     _targets = (Targets.IMAGE, Targets.MASK)
 
+    class InitSchema(BaseTransformInitSchema):
+        scale: OnePlusIntRangeType = (2, 3)
+        operation: MorphologyMode = "dilation"
+
     def __init__(
         self,
         scale: ScaleIntType = (2, 3),
         operation: MorphologyMode = "dilation",
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
-        self.scale = to_tuple(scale, scale)
+        self.scale = cast(Tuple[int, int], scale)
         self.operation = operation
 
     def apply(self, img: np.ndarray, kernel: Tuple[int, int], **params: Any) -> np.ndarray:
         return F.morphology(img, kernel, self.operation)
 
     def apply_to_mask(self, mask: np.ndarray, kernel: Tuple[int, int], **params: Any) -> np.ndarray:
         return F.morphology(mask, kernel, self.operation)
 
     def get_params(self) -> Dict[str, float]:
-        kernel = cv2.getStructuringElement(
-            cv2.MORPH_ELLIPSE, tuple(random_utils.randint(self.scale[0], self.scale[1], 2))
-        )
         return {
-            "kernel": kernel,
+            "kernel": cv2.getStructuringElement(cv2.MORPH_ELLIPSE, self.scale),
         }
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return ("scale", "operation")
```

### Comparing `albumentations-1.4.3/albumentations/augmentations/utils.py` & `albumentations-1.4.4/albumentations/augmentations/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from functools import wraps
 from pathlib import Path
-from typing import Any, Callable, Union
+from typing import Any, Callable, Optional, Tuple, Union
 
 import cv2
 import numpy as np
 from typing_extensions import Concatenate, ParamSpec
 
 from albumentations.core.keypoints_utils import angle_to_2pi_range
 from albumentations.core.types import KeypointInternalType
@@ -56,14 +56,15 @@
     np.dtype("float64"): cv2.CV_64F,
 }
 
 TWO = 2
 THREE = 3
 RGB_NUM_CHANNELS = 3
 FOUR = 4
+BIG_INTEGER = MAX_VALUES_BY_DTYPE[np.uint32]
 
 
 def read_bgr_image(path: Union[str, Path]) -> np.ndarray:
     return cv2.imread(str(path), cv2.IMREAD_COLOR)
 
 
 def read_rgb_image(path: Union[str, Path]) -> np.ndarray:
@@ -177,15 +178,16 @@
         if is_multispectral_image(image):  # Any image with a number of channels other than 1 and 3
             message += "\nThis transformation cannot be applied to multi-spectral images"
 
         raise ValueError(message)
 
 
 def _maybe_process_in_chunks(
-    process_fn: Callable[Concatenate[np.ndarray, P], np.ndarray], **kwargs: Any
+    process_fn: Callable[Concatenate[np.ndarray, P], np.ndarray],
+    **kwargs: Any,
 ) -> Callable[[np.ndarray], np.ndarray]:
     """Wrap OpenCV function to enable processing images with more than 4 channels.
 
     Limitations:
         This wrapper requires image to be the first argument and rest must be sent via named arguments.
 
     Args:
@@ -215,7 +217,25 @@
                     chunk = process_fn(chunk, **kwargs)
                     chunks.append(chunk)
             return np.dstack(chunks)
 
         return process_fn(img, **kwargs)
 
     return __process_fn
+
+
+def check_range(value: Tuple[float, float], lower_bound: float, upper_bound: float, name: Optional[str]) -> None:
+    """Checks if the given value is within the specified bounds
+
+    Args:
+        value: The value to check and convert. Can be a single float or a tuple of floats.
+        lower_bound: The lower bound for the range check.
+        upper_bound: The upper bound for the range check.
+        name: The name of the parameter being checked. Used for error messages.
+
+    Raises:
+        ValueError: If the value is outside the bounds or if the tuple values are not ordered correctly.
+    """
+    if not all(lower_bound <= x <= upper_bound for x in value):
+        raise ValueError(f"All values in {name} must be within [{lower_bound}, {upper_bound}] for tuple inputs.")
+    if not value[0] <= value[1]:
+        raise ValueError(f"{name!s} tuple values must be ordered as (min, max). Got: {value}")
```

### Comparing `albumentations-1.4.3/albumentations/core/bbox_utils.py` & `albumentations-1.4.4/albumentations/core/bbox_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         data.update(
             {
                 "min_area": self.min_area,
                 "min_visibility": self.min_visibility,
                 "min_width": self.min_width,
                 "min_height": self.min_height,
                 "check_each_transform": self.check_each_transform,
-            }
+            },
         )
         return data
 
     @classmethod
     def is_serializable(cls) -> bool:
         return True
 
@@ -289,15 +289,19 @@
         visibility = transformed_bbox_area / bbox_area
         if visibility >= threshold:
             visible_bboxes.append(transformed_bbox)
     return visible_bboxes
 
 
 def convert_bbox_to_albumentations(
-    bbox: BoxType, source_format: str, rows: int, cols: int, check_validity: bool = False
+    bbox: BoxType,
+    source_format: str,
+    rows: int,
+    cols: int,
+    check_validity: bool = False,
 ) -> BoxType:
     """Convert a bounding box from a format specified in `source_format` to the format used by albumentations:
     normalized coordinates of top-left and bottom-right corners of the bounding box in a form of
     `(x_min, y_min, x_max, y_max)` e.g. `(0.15, 0.27, 0.67, 0.5)`.
 
     Args:
         bbox: A bounding box tuple.
@@ -318,15 +322,15 @@
     Raises:
         ValueError: if `target_format` is not equal to `coco` or `pascal_voc`, or `yolo`.
         ValueError: If in YOLO format all labels not in range (0, 1).
 
     """
     if source_format not in {"coco", "pascal_voc", "yolo"}:
         raise ValueError(
-            f"Unknown source_format {source_format}. Supported formats are: 'coco', 'pascal_voc' and 'yolo'"
+            f"Unknown source_format {source_format}. Supported formats are: 'coco', 'pascal_voc' and 'yolo'",
         )
 
     if source_format == "coco":
         (x_min, y_min, width, height), tail = bbox[:4], bbox[4:]
         x_max = x_min + width
         y_max = y_min + height
     elif source_format == "yolo":
@@ -352,15 +356,19 @@
         bbox = normalize_bbox(bbox, rows, cols)
     if check_validity:
         check_bbox(bbox)
     return bbox
 
 
 def convert_bbox_from_albumentations(
-    bbox: BoxType, target_format: str, rows: int, cols: int, check_validity: bool = False
+    bbox: BoxType,
+    target_format: str,
+    rows: int,
+    cols: int,
+    check_validity: bool = False,
 ) -> BoxType:
     """Convert a bounding box from the format used by albumentations to a format, specified in `target_format`.
 
     Args:
         bbox: An albumentations bounding box `(x_min, y_min, x_max, y_max)`.
         target_format: required format of the output bounding box. Should be 'coco', 'pascal_voc' or 'yolo'.
         rows: Image height.
@@ -377,15 +385,15 @@
 
     Raises:
         ValueError: if `target_format` is not equal to `coco`, `pascal_voc` or `yolo`.
 
     """
     if target_format not in {"coco", "pascal_voc", "yolo"}:
         raise ValueError(
-            f"Unknown target_format {target_format}. Supported formats are: 'coco', 'pascal_voc' and 'yolo'"
+            f"Unknown target_format {target_format}. Supported formats are: 'coco', 'pascal_voc' and 'yolo'",
         )
     if check_validity:
         check_bbox(bbox)
 
     if target_format != "yolo":
         bbox = denormalize_bbox(bbox, rows, cols)
     if target_format == "coco":
@@ -400,22 +408,30 @@
         w = x_max - x_min
         h = y_max - y_min
         bbox = cast(BoxType, (x, y, w, h, *tail))
     return bbox
 
 
 def convert_bboxes_to_albumentations(
-    bboxes: Sequence[BoxType], source_format: str, rows: int, cols: int, check_validity: bool = False
+    bboxes: Sequence[BoxType],
+    source_format: str,
+    rows: int,
+    cols: int,
+    check_validity: bool = False,
 ) -> List[BoxType]:
     """Convert a list bounding boxes from a format specified in `source_format` to the format used by albumentations"""
     return [convert_bbox_to_albumentations(bbox, source_format, rows, cols, check_validity) for bbox in bboxes]
 
 
 def convert_bboxes_from_albumentations(
-    bboxes: Sequence[BoxType], target_format: str, rows: int, cols: int, check_validity: bool = False
+    bboxes: Sequence[BoxType],
+    target_format: str,
+    rows: int,
+    cols: int,
+    check_validity: bool = False,
 ) -> List[BoxType]:
     """Convert a list of bounding boxes from the format used by albumentations to a format, specified
     in `target_format`.
 
     Args:
         bboxes: List of albumentations bounding box `(x_min, y_min, x_max, y_max)`.
         target_format: required format of the output bounding box. Should be 'coco', 'pascal_voc' or 'yolo'.
```

### Comparing `albumentations-1.4.3/albumentations/core/composition.py` & `albumentations-1.4.4/albumentations/core/composition.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,23 +50,25 @@
     return new_transforms
 
 
 class BaseCompose(Serializable):
     def __init__(self, transforms: TransformsSeqType, p: float):
         if isinstance(transforms, (BaseCompose, BasicTransform)):
             warnings.warn(
-                "transforms is single transform, but a sequence is expected! Transform will be wrapped into list."
+                "transforms is single transform, but a sequence is expected! Transform will be wrapped into list.",
             )
             transforms = [transforms]
 
         self.transforms = transforms
         self.p = p
 
         self.replay_mode = False
         self.applied_in_replay = False
+        self._additional_targets: Dict[str, str] = {}
+        self.processors: Dict[str, Union[BboxProcessor, KeypointsProcessor]] = {}
 
     def __iter__(self) -> Iterator[TransformType]:
         return iter(self.transforms)
 
     def __len__(self) -> int:
         return len(self.transforms)
 
@@ -75,14 +77,18 @@
 
     def __getitem__(self, item: int) -> TransformType:
         return self.transforms[item]
 
     def __repr__(self) -> str:
         return self.indented_repr()
 
+    @property
+    def additional_targets(self) -> Dict[str, str]:
+        return self._additional_targets
+
     def indented_repr(self, indent: int = REPR_INDENT_STEP) -> str:
         args = {k: v for k, v in self.to_dict_private().items() if not (k.startswith("__") or k == "transforms")}
         repr_string = self.__class__.__name__ + "(["
         for t in self.transforms:
             repr_string += "\n"
             t_repr = t.indented_repr(indent + REPR_INDENT_STEP) if hasattr(t, "indented_repr") else repr(t)
             repr_string += " " * indent + t_repr + ","
@@ -110,16 +116,25 @@
             "id": id(self),
             "params": None,
             "transforms": [t.get_dict_with_id() for t in self.transforms],
         }
 
     def add_targets(self, additional_targets: Optional[Dict[str, str]]) -> None:
         if additional_targets:
+            for k, v in additional_targets.items():
+                if k in self._additional_targets and v != self._additional_targets[k]:
+                    raise ValueError(
+                        f"Trying to overwrite existed additional targets. "
+                        f"Key={k} Exists={self._additional_targets[k]} New value: {v}",
+                    )
+                self._additional_targets.update(additional_targets)
             for t in self.transforms:
                 t.add_targets(additional_targets)
+            for proc in self.processors.values():
+                proc.add_targets(additional_targets)
 
     def set_deterministic(self, flag: bool, save_key: str = "replay") -> None:
         for t in self.transforms:
             t.set_deterministic(flag, save_key)
 
 
 class Compose(BaseCompose):
@@ -143,39 +158,33 @@
         keypoint_params: Optional[Union[Dict[str, Any], "KeypointParams"]] = None,
         additional_targets: Optional[Dict[str, str]] = None,
         p: float = 1.0,
         is_check_shapes: bool = True,
     ):
         super().__init__(transforms, p)
 
-        self.processors: Dict[str, Union[BboxProcessor, KeypointsProcessor]] = {}
         if bbox_params:
             if isinstance(bbox_params, dict):
                 b_params = BboxParams(**bbox_params)
             elif isinstance(bbox_params, BboxParams):
                 b_params = bbox_params
             else:
                 msg = "unknown format of bbox_params, please use `dict` or `BboxParams`"
                 raise ValueError(msg)
-            self.processors["bboxes"] = BboxProcessor(b_params, additional_targets)
+            self.processors["bboxes"] = BboxProcessor(b_params)
 
         if keypoint_params:
             if isinstance(keypoint_params, dict):
                 k_params = KeypointParams(**keypoint_params)
             elif isinstance(keypoint_params, KeypointParams):
                 k_params = keypoint_params
             else:
                 msg = "unknown format of keypoint_params, please use `dict` or `KeypointParams`"
                 raise ValueError(msg)
-            self.processors["keypoints"] = KeypointsProcessor(k_params, additional_targets)
-
-        if additional_targets is None:
-            additional_targets = {}
-
-        self.additional_targets = additional_targets
+            self.processors["keypoints"] = KeypointsProcessor(k_params)
 
         for proc in self.processors.values():
             proc.ensure_transforms_valid(self.transforms)
 
         self.add_targets(additional_targets)
 
         self.is_check_args = True
@@ -247,40 +256,40 @@
         keypoints_processor = self.processors.get("keypoints")
         dictionary.update(
             {
                 "bbox_params": bbox_processor.params.to_dict_private() if bbox_processor else None,
                 "keypoint_params": (keypoints_processor.params.to_dict_private() if keypoints_processor else None),
                 "additional_targets": self.additional_targets,
                 "is_check_shapes": self.is_check_shapes,
-            }
+            },
         )
         return dictionary
 
     def get_dict_with_id(self) -> Dict[str, Any]:
         dictionary = super().get_dict_with_id()
         bbox_processor = self.processors.get("bboxes")
         keypoints_processor = self.processors.get("keypoints")
         dictionary.update(
             {
                 "bbox_params": bbox_processor.params.to_dict_private() if bbox_processor else None,
                 "keypoint_params": (keypoints_processor.params.to_dict_private() if keypoints_processor else None),
                 "additional_targets": self.additional_targets,
                 "params": None,
                 "is_check_shapes": self.is_check_shapes,
-            }
+            },
         )
         return dictionary
 
     def _check_args(self, **kwargs: Any) -> None:
         checked_single = ["image", "mask"]
         checked_multi = ["masks"]
         check_bbox_param = ["bboxes"]
         shapes = []
         for data_name, data in kwargs.items():
-            internal_data_name = self.additional_targets.get(data_name, data_name)
+            internal_data_name = self._additional_targets.get(data_name, data_name)
             if internal_data_name in checked_single:
                 if not isinstance(data, np.ndarray):
                     raise TypeError(f"{data_name} must be numpy array type")
                 shapes.append(data.shape[:2])
             if internal_data_name in checked_multi and data is not None and len(data):
                 if not isinstance(data[0], np.ndarray):
                     raise TypeError(f"{data_name} must be list of numpy arrays")
@@ -470,15 +479,16 @@
     @staticmethod
     def replay(saved_augmentations: Dict[str, Any], **kwargs: Any) -> Dict[str, Any]:
         augs = ReplayCompose._restore_for_replay(saved_augmentations)
         return augs(force_apply=True, **kwargs)
 
     @staticmethod
     def _restore_for_replay(
-        transform_dict: Dict[str, Any], lambda_transforms: Optional[Dict[str, Any]] = None
+        transform_dict: Dict[str, Any],
+        lambda_transforms: Optional[Dict[str, Any]] = None,
     ) -> TransformType:
         """Args:
         lambda_transforms (dict): A dictionary that contains lambda transforms, that
         is instances of the Lambda class.
             This dictionary is required when you are restoring a pipeline that contains lambda transforms. Keys
             in that dictionary should be named same as `name` arguments in respective lambda transforms from
             a serialized pipeline.
@@ -554,10 +564,11 @@
 
     """
 
     def __init__(self, transforms: TransformsSeqType, p: float = 0.5):
         super().__init__(transforms, p)
 
     def __call__(self, *args: Any, force_apply: bool = False, **data: Any) -> Dict[str, Any]:
-        for t in self.transforms:
-            data = t(**data)
+        if self.replay_mode or force_apply or random.random() < self.p:
+            for t in self.transforms:
+                data = t(**data)
         return data
```

### Comparing `albumentations-1.4.3/albumentations/core/keypoints_utils.py` & `albumentations-1.4.4/albumentations/core/keypoints_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     def to_dict_private(self) -> Dict[str, Any]:
         data = super().to_dict_private()
         data.update(
             {
                 "remove_invisible": self.remove_invisible,
                 "angle_in_degrees": self.angle_in_degrees,
                 "check_each_transform": self.check_each_transform,
-            }
+            },
         )
         return data
 
     @classmethod
     def is_serializable(cls) -> bool:
         return True
 
@@ -83,15 +83,15 @@
 
     @property
     def default_data_name(self) -> str:
         return "keypoints"
 
     def ensure_data_valid(self, data: Dict[str, Any]) -> None:
         if self.params.label_fields and not all(i in data for i in self.params.label_fields):
-            msg = "Your 'label_fields' are not valid - them must have same names as params in " "'keypoint_params' dict"
+            msg = "Your 'label_fields' are not valid - them must have same names as params in 'keypoint_params' dict"
             raise ValueError(msg)
 
     def filter(self, data: Sequence[KeypointType], rows: int, cols: int) -> Sequence[KeypointType]:
         """The function filters a sequence of data based on the number of rows and columns, and returns a
         sequence of keypoints.
 
         :param data: The `data` parameter is a sequence of sequences. Each inner sequence represents a
@@ -134,29 +134,32 @@
         )
 
 
 def check_keypoint(kp: KeypointType, rows: int, cols: int) -> None:
     """Check if keypoint coordinates are less than image shapes"""
     for name, value, size in zip(["x", "y"], kp[:2], [cols, rows]):
         if not 0 <= value < size:
-            raise ValueError(f"Expected {name} for keypoint {kp} " f"to be in the range [0.0, {size}], got {value}.")
+            raise ValueError(f"Expected {name} for keypoint {kp} to be in the range [0.0, {size}], got {value}.")
 
     angle = kp[2]
     if not (0 <= angle < 2 * math.pi):
         raise ValueError(f"Keypoint angle must be in range [0, 2 * PI). Got: {angle}")
 
 
 def check_keypoints(keypoints: Sequence[KeypointType], rows: int, cols: int) -> None:
     """Check if keypoints boundaries are less than image shapes"""
     for kp in keypoints:
         check_keypoint(kp, rows, cols)
 
 
 def filter_keypoints(
-    keypoints: Sequence[KeypointType], rows: int, cols: int, remove_invisible: bool
+    keypoints: Sequence[KeypointType],
+    rows: int,
+    cols: int,
+    remove_invisible: bool,
 ) -> Sequence[KeypointType]:
     if not remove_invisible:
         return keypoints
 
     resulting_keypoints = []
     for kp in keypoints:
         x, y = kp[:2]
```

### Comparing `albumentations-1.4.3/albumentations/core/serialization.py` & `albumentations-1.4.4/albumentations/core/serialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
                 raise
 
             transform_dict = {}
             warnings.warn(
                 f"Got NotImplementedError while trying to serialize {self}. Object arguments are not preserved. "
                 f"Implement either '{self.__class__.__name__}.get_transform_init_args_names' "
                 f"or '{self.__class__.__name__}.get_transform_init_args' "
-                "method to make the transform serializable"
+                "method to make the transform serializable",
             )
         return {"__version__": __version__, "transform": transform_dict}
 
 
 def to_dict(transform: Serializable, on_not_implemented_error: str = "raise") -> Dict[str, Any]:
     """Take a transform pipeline and convert it to a serializable representation that uses only standard
     python data types: dictionaries, lists, strings, integers, and floats.
@@ -120,15 +120,16 @@
         on_not_implemented_error (str): `raise` or `warn`.
 
     """
     return transform.to_dict(on_not_implemented_error)
 
 
 def instantiate_nonserializable(
-    transform: Dict[str, Any], nonserializable: Optional[Dict[str, Any]] = None
+    transform: Dict[str, Any],
+    nonserializable: Optional[Dict[str, Any]] = None,
 ) -> Optional[Serializable]:
     if transform.get("__class_fullname__") in NON_SERIALIZABLE_REGISTRY:
         name = transform["__name__"]
         if nonserializable is None:
             msg = f"To deserialize a non-serializable transform with name {name} you need to pass a dict with"
             "this transform as the `lambda_transforms` argument"
             raise ValueError(msg)
@@ -136,15 +137,16 @@
         if transform is None:
             raise ValueError(f"Non-serializable transform with {name} was not found in `nonserializable`")
         return result_transform
     return None
 
 
 def from_dict(
-    transform_dict: Dict[str, Any], nonserializable: Optional[Dict[str, Any]] = None
+    transform_dict: Dict[str, Any],
+    nonserializable: Optional[Dict[str, Any]] = None,
 ) -> Optional[Serializable]:
     """Args:
     transform_dict: A dictionary with serialized transform pipeline.
     nonserializable (dict): A dictionary that contains non-serializable transforms.
         This dictionary is required when you are restoring a pipeline that contains non-serializable transforms.
         Keys in that dictionary should be named same as `name` arguments in respective transforms from
         a serialized pipeline.
```

### Comparing `albumentations-1.4.3/albumentations/core/transforms_interface.py` & `albumentations-1.4.4/albumentations/core/transforms_interface.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,89 +1,60 @@
 import random
 from copy import deepcopy
 from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union, cast
 from warnings import warn
 
 import cv2
 import numpy as np
+from pydantic import BaseModel, ConfigDict, Field
+from typing_extensions import Annotated
 
-from .serialization import Serializable, get_shortest_class_fullname
+from albumentations.core.validation import ValidatedTransformMeta
+
+from .serialization import Serializable, SerializableMeta, get_shortest_class_fullname
 from .types import (
     BoxInternalType,
     BoxType,
     ColorType,
     KeypointInternalType,
     KeypointType,
-    ScalarType,
-    ScaleType,
     Targets,
 )
 from .utils import format_args
 
-__all__ = ["to_tuple", "BasicTransform", "DualTransform", "ImageOnlyTransform", "NoOp", "ReferenceBasedTransform"]
+__all__ = ["BasicTransform", "DualTransform", "ImageOnlyTransform", "NoOp", "ReferenceBasedTransform"]
 
 PAIR = 2
 
 
-def to_tuple(
-    param: ScaleType,
-    low: Optional[ScaleType] = None,
-    bias: Optional[ScalarType] = None,
-) -> Union[Tuple[int, int], Tuple[float, float]]:
-    """Convert input argument to a min-max tuple.
-
-    Args:
-        param: Input value which could be a scalar or a sequence of exactly 2 scalars.
-        low: Second element of the tuple, provided as an optional argument for when `param` is a scalar.
-        bias: An offset added to both elements of the tuple.
-
-    Returns:
-        A tuple of two scalars, optionally adjusted by `bias`.
-        Raises ValueError for invalid combinations or types of arguments.
-
-    """
-    # Validate mutually exclusive arguments
-    if low is not None and bias is not None:
-        msg = "Arguments 'low' and 'bias' cannot be used together."
-        raise ValueError(msg)
-
-    if isinstance(param, Sequence) and len(param) == PAIR:
-        min_val, max_val = min(param), max(param)
-
-    # Handle scalar input
-    elif isinstance(param, (int, float)):
-        if isinstance(low, (int, float)):
-            # Use low and param to create a tuple
-            min_val, max_val = (low, param) if low < param else (param, low)
-        else:
-            # Create a symmetric tuple around 0
-            min_val, max_val = -param, param
-    else:
-        msg = "Argument 'param' must be either a scalar or a sequence of 2 elements."
-        raise ValueError(msg)
-
-    # Apply bias if provided
-    if bias is not None:
-        return (bias + min_val, bias + max_val)
-
-    return min_val, max_val
-
-
 class Interpolation:
     def __init__(self, downscale: int = cv2.INTER_NEAREST, upscale: int = cv2.INTER_NEAREST):
         self.downscale = downscale
         self.upscale = upscale
 
 
-class BasicTransform(Serializable):
+class BaseTransformInitSchema(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+    always_apply: bool = Field(default=False, description="Always apply the transform")
+    p: Annotated[float, Field(default=0.5, description="Probability of applying the transform", ge=0, le=1)]
+
+
+class CombinedMeta(SerializableMeta, ValidatedTransformMeta):
+    pass
+
+
+class BasicTransform(Serializable, metaclass=CombinedMeta):
     call_backup = None
     interpolation: Union[int, Interpolation]
     fill_value: ColorType
     mask_fill_value: Optional[ColorType]
 
+    class InitSchema(BaseTransformInitSchema):
+        pass
+
     def __init__(self, always_apply: bool = False, p: float = 0.5):
         self.p = p
         self.always_apply = always_apply
         self._additional_targets: Dict[str, str] = {}
 
         # replay mode params
         self.deterministic = False
@@ -113,15 +84,15 @@
                 targets_as_params = {k: kwargs[k] for k in self.targets_as_params}
                 params_dependent_on_targets = self.get_params_dependent_on_targets(targets_as_params)
                 params.update(params_dependent_on_targets)
             if self.deterministic:
                 if self.targets_as_params:
                     warn(
                         self.get_class_fullname() + " could work incorrectly in ReplayMode for other input data"
-                        " because its' params depend on targets."
+                        " because its' params depend on targets.",
                     )
                 kwargs[self.save_key][id(self)] = deepcopy(params)
             return self.apply_with_params(params, **kwargs)
 
         return kwargs
 
     def apply_with_params(self, params: Dict[str, Any], *args: Any, **kwargs: Any) -> Dict[str, Any]:
@@ -193,23 +164,23 @@
         ex: {'obj1_mask': 'mask', 'obj2_mask': 'mask'}
         by the way you must have at least one object with key 'image'
 
         Args:
             additional_targets (dict): keys - new target name, values - old target name. ex: {'image2': 'image'}
 
         """
-        self._additional_targets = additional_targets
+        self._additional_targets = {**self._additional_targets, **additional_targets}
 
     @property
     def targets_as_params(self) -> List[str]:
         return []
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, Any]:
         raise NotImplementedError(
-            "Method get_params_dependent_on_targets is not implemented in class " + self.__class__.__name__
+            "Method get_params_dependent_on_targets is not implemented in class " + self.__class__.__name__,
         )
 
     @classmethod
     def get_class_fullname(cls) -> str:
         return get_shortest_class_fullname(cls)
 
     @classmethod
@@ -227,14 +198,15 @@
     def get_transform_init_args(self) -> Dict[str, Any]:
         return {k: getattr(self, k) for k in self.get_transform_init_args_names()}
 
     def to_dict_private(self) -> Dict[str, Any]:
         state = {"__class_fullname__": self.get_class_fullname()}
         state.update(self.get_base_init_args())
         state.update(self.get_transform_init_args())
+
         return state
 
     def get_dict_with_id(self) -> Dict[str, Any]:
         d = self.to_dict_private()
         d["id"] = id(self)
         return d
 
@@ -300,15 +272,18 @@
         return [
             self.apply_to_bbox(cast(BoxInternalType, tuple(cast(BoxInternalType, bbox[:4]))), **params)
             + tuple(bbox[4:])
             for bbox in bboxes
         ]
 
     def apply_to_keypoints(
-        self, keypoints: Sequence[KeypointType], *args: Any, **params: Any
+        self,
+        keypoints: Sequence[KeypointType],
+        *args: Any,
+        **params: Any,
     ) -> Sequence[KeypointType]:
         return [
             self.apply_to_keypoint(cast(KeypointInternalType, tuple(keypoint[:4])), **params) + tuple(keypoint[4:])
             for keypoint in keypoints
         ]
 
     def apply_to_mask(self, mask: np.ndarray, *args: Any, **params: Any) -> np.ndarray:
```

### Comparing `albumentations-1.4.3/albumentations/core/utils.py` & `albumentations-1.4.4/albumentations/core/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Sequence, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 
 from .serialization import Serializable
-from .types import BoxOrKeypointType, SizeType
+from .types import BoxOrKeypointType, ScalarType, ScaleType, SizeType
 
 if TYPE_CHECKING:
     import torch
 
+PAIR = 2
+
 
 def get_shape(img: Union["np.ndarray", "torch.Tensor"]) -> SizeType:
     if isinstance(img, np.ndarray):
         rows, cols = img.shape[:2]
         return rows, cols
 
     try:
@@ -20,15 +22,15 @@
 
         if torch.is_tensor(img):
             return img.shape[-2:]
     except ImportError:
         pass
 
     raise RuntimeError(
-        f"Albumentations supports only numpy.ndarray and torch.Tensor data type for image. Got: {type(img)}"
+        f"Albumentations supports only numpy.ndarray and torch.Tensor data type for image. Got: {type(img)}",
     )
 
 
 def format_args(args_dict: Dict[str, Any]) -> str:
     formatted_args = []
     for k, v in args_dict.items():
         v_formatted = f"'{v}'" if isinstance(v, str) else str(v)
@@ -46,23 +48,27 @@
 
 
 class DataProcessor(ABC):
     def __init__(self, params: Params, additional_targets: Optional[Dict[str, str]] = None):
         self.params = params
         self.data_fields = [self.default_data_name]
         if additional_targets is not None:
-            for k, v in additional_targets.items():
-                if v == self.default_data_name:
-                    self.data_fields.append(k)
+            self.add_targets(additional_targets)
 
     @property
     @abstractmethod
     def default_data_name(self) -> str:
         raise NotImplementedError
 
+    def add_targets(self, additional_targets: Dict[str, str]) -> None:
+        """Add targets to transform them the same way as one of existing targets"""
+        for k, v in additional_targets.items():
+            if v == self.default_data_name and k not in self.data_fields:
+                self.data_fields.append(k)
+
     def ensure_data_valid(self, data: Dict[str, Any]) -> None:
         pass
 
     def ensure_transforms_valid(self, transforms: Sequence[object]) -> None:
         pass
 
     def postprocess(self, data: Dict[str, Any]) -> Dict[str, Any]:
@@ -78,15 +84,19 @@
         data = self.add_label_fields_to_data(data)
 
         rows, cols = data["image"].shape[:2]
         for data_name in self.data_fields:
             data[data_name] = self.check_and_convert(data[data_name], rows, cols, direction="to")
 
     def check_and_convert(
-        self, data: List[BoxOrKeypointType], rows: int, cols: int, direction: str = "to"
+        self,
+        data: List[BoxOrKeypointType],
+        rows: int,
+        cols: int,
+        direction: str = "to",
     ) -> List[BoxOrKeypointType]:
         if self.params.format == "albumentations":
             self.check(data, rows, cols)
             return data
 
         if direction == "to":
             return self.convert_to_albumentations(data, rows, cols)
@@ -105,15 +115,18 @@
 
     @abstractmethod
     def convert_to_albumentations(self, data: List[BoxOrKeypointType], rows: int, cols: int) -> List[BoxOrKeypointType]:
         pass
 
     @abstractmethod
     def convert_from_albumentations(
-        self, data: List[BoxOrKeypointType], rows: int, cols: int
+        self,
+        data: List[BoxOrKeypointType],
+        rows: int,
+        cols: int,
     ) -> List[BoxOrKeypointType]:
         pass
 
     def add_label_fields_to_data(self, data: Dict[str, Any]) -> Dict[str, Any]:
         if self.params.label_fields is None:
             return data
         for data_name in self.data_fields:
@@ -133,7 +146,51 @@
         for data_name in self.data_fields:
             label_fields_len = len(self.params.label_fields)
             for idx, field in enumerate(self.params.label_fields):
                 data[field] = [bbox[-label_fields_len + idx] for bbox in data[data_name]]
             if label_fields_len:
                 data[data_name] = [d[:-label_fields_len] for d in data[data_name]]
         return data
+
+
+def to_tuple(
+    param: ScaleType,
+    low: Optional[ScaleType] = None,
+    bias: Optional[ScalarType] = None,
+) -> Union[Tuple[int, int], Tuple[float, float]]:
+    """Convert input argument to a min-max tuple.
+
+    Args:
+        param: Input value which could be a scalar or a sequence of exactly 2 scalars.
+        low: Second element of the tuple, provided as an optional argument for when `param` is a scalar.
+        bias: An offset added to both elements of the tuple.
+
+    Returns:
+        A tuple of two scalars, optionally adjusted by `bias`.
+        Raises ValueError for invalid combinations or types of arguments.
+
+    """
+    # Validate mutually exclusive arguments
+    if low is not None and bias is not None:
+        msg = "Arguments 'low' and 'bias' cannot be used together."
+        raise ValueError(msg)
+
+    if isinstance(param, Sequence) and len(param) == PAIR:
+        min_val, max_val = min(param), max(param)
+
+    # Handle scalar input
+    elif isinstance(param, (int, float)):
+        if isinstance(low, (int, float)):
+            # Use low and param to create a tuple
+            min_val, max_val = (low, param) if low < param else (param, low)
+        else:
+            # Create a symmetric tuple around 0
+            min_val, max_val = -param, param
+    else:
+        msg = "Argument 'param' must be either a scalar or a sequence of 2 elements."
+        raise ValueError(msg)
+
+    # Apply bias if provided
+    if bias is not None:
+        return (bias + min_val, bias + max_val)
+
+    return min_val, max_val
```

### Comparing `albumentations-1.4.3/albumentations/pytorch/transforms.py` & `albumentations-1.4.4/albumentations/pytorch/transforms.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.3/albumentations/random_utils.py` & `albumentations-1.4.4/albumentations/random_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,23 +29,31 @@
 ) -> FloatNumType:
     if random_state is None:
         random_state = get_random_state()
     return random_state.beta(alpha, beta)
 
 
 def rand(
-    d0: NumType, d1: NumType, *more: Any, random_state: Optional[np.random.RandomState] = None, **kwargs: Any
+    d0: NumType,
+    d1: NumType,
+    *more: Any,
+    random_state: Optional[np.random.RandomState] = None,
+    **kwargs: Any,
 ) -> np.ndarray:
     if random_state is None:
         random_state = get_random_state()
     return random_state.rand(d0, d1, *more, **kwargs)
 
 
 def randn(
-    d0: NumType, d1: NumType, *more: Any, random_state: Optional[np.random.RandomState] = None, **kwargs: Any
+    d0: NumType,
+    d1: NumType,
+    *more: Any,
+    random_state: Optional[np.random.RandomState] = None,
+    **kwargs: Any,
 ) -> np.ndarray:
     if random_state is None:
         random_state = get_random_state()
     return random_state.randn(d0, d1, *more, **kwargs)
 
 
 def normal(
@@ -56,23 +64,26 @@
 ) -> FloatNumType:
     if random_state is None:
         random_state = get_random_state()
     return random_state.normal(loc, scale, size)
 
 
 def poisson(
-    lam: NumType = 1.0, size: Optional[SizeType] = None, random_state: Optional[np.random.RandomState] = None
+    lam: NumType = 1.0,
+    size: Optional[SizeType] = None,
+    random_state: Optional[np.random.RandomState] = None,
 ) -> IntNumType:
     if random_state is None:
         random_state = get_random_state()
     return random_state.poisson(lam, size)
 
 
 def permutation(
-    x: Union[int, Sequence[float], np.ndarray], random_state: Optional[np.random.RandomState] = None
+    x: Union[int, Sequence[float], np.ndarray],
+    random_state: Optional[np.random.RandomState] = None,
 ) -> np.ndarray:
     if random_state is None:
         random_state = get_random_state()
     return random_state.permutation(x)
 
 
 def randint(
```

### Comparing `albumentations-1.4.3/albumentations.egg-info/PKG-INFO` & `albumentations-1.4.4/albumentations.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: albumentations
-Version: 1.4.3
+Version: 1.4.4
 Summary: An efficient library for image augmentation, providing extensive transformations to support machine learning and computer vision tasks.
 Home-page: https://albumentations.ai
 Author: Vladimir I. Iglovikov, Mikhail Druzhinin, Alex Parinov, Alexander Buslaev, Eugene Khvedchenya
 License: MIT
 Keywords: image augmentation,data augmentation,computer vision,deep learning,machine learning,image processing,artificial intelligence,augmentation library,image transformation,vision augmentation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -28,22 +28,24 @@
 License-File: LICENSE
 Requires-Dist: numpy>=1.24.4
 Requires-Dist: scipy>=1.10.0
 Requires-Dist: scikit-image>=0.21.0
 Requires-Dist: PyYAML
 Requires-Dist: typing-extensions>=4.9.0
 Requires-Dist: scikit-learn>=1.3.2
+Requires-Dist: pydantic>=2.6.4
 Requires-Dist: opencv-python-headless>=4.9.0
 
 # Albumentations
 
 [![PyPI version](https://badge.fury.io/py/albumentations.svg)](https://badge.fury.io/py/albumentations)
 ![CI](https://github.com/albumentations-team/albumentations/workflows/CI/badge.svg)
 [![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![Pydantic v2](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/main/docs/badge/v2.json)](https://pydantic.dev)
 
 [Docs](https://albumentations.ai/docs/) | [Discord](https://discord.gg/AKPrrDYNAt) | [Twitter](https://twitter.com/albumentations) | [LinkedIn](https://www.linkedin.com/company/100504475/)
 
 Albumentations is a Python library for image augmentation. Image augmentation is used in deep learning and computer vision tasks to increase the quality of trained models. The purpose of image augmentation is to create new training samples from the existing data.
 
 Here is an example of how you can apply some [pixel-level](#pixel-level-transforms) augmentations from Albumentations to create new images from the original one:
 ![parrot](https://habrastorage.org/webt/bd/ne/rv/bdnerv5ctkudmsaznhw4crsdfiw.jpeg)
@@ -249,14 +251,15 @@
 | [Affine](https://albumentations.ai/docs/api_reference/augmentations/geometric/transforms/#albumentations.augmentations.geometric.transforms.Affine)                             | ✓     | ✓    | ✓      | ✓         |
 | [BBoxSafeRandomCrop](https://albumentations.ai/docs/api_reference/augmentations/crops/transforms/#albumentations.augmentations.crops.transforms.BBoxSafeRandomCrop)             | ✓     | ✓    | ✓      |           |
 | [CenterCrop](https://albumentations.ai/docs/api_reference/augmentations/crops/transforms/#albumentations.augmentations.crops.transforms.CenterCrop)                             | ✓     | ✓    | ✓      | ✓         |
 | [CoarseDropout](https://albumentations.ai/docs/api_reference/augmentations/dropout/coarse_dropout/#albumentations.augmentations.dropout.coarse_dropout.CoarseDropout)           | ✓     | ✓    |        | ✓         |
 | [Crop](https://albumentations.ai/docs/api_reference/augmentations/crops/transforms/#albumentations.augmentations.crops.transforms.Crop)                                         | ✓     | ✓    | ✓      | ✓         |
 | [CropAndPad](https://albumentations.ai/docs/api_reference/augmentations/crops/transforms/#albumentations.augmentations.crops.transforms.CropAndPad)                             | ✓     | ✓    | ✓      | ✓         |
 | [CropNonEmptyMaskIfExists](https://albumentations.ai/docs/api_reference/augmentations/crops/transforms/#albumentations.augmentations.crops.transforms.CropNonEmptyMaskIfExists) | ✓     | ✓    | ✓      | ✓         |
+| [D4](https://albumentations.ai/docs/api_reference/augmentations/geometric/transforms/#albumentations.augmentations.geometric.transforms.D4)                                     | ✓     | ✓    | ✓      | ✓         |
 | [ElasticTransform](https://albumentations.ai/docs/api_reference/augmentations/geometric/transforms/#albumentations.augmentations.geometric.transforms.ElasticTransform)         | ✓     | ✓    | ✓      |           |
 | [Flip](https://albumentations.ai/docs/api_reference/augmentations/geometric/transforms/#albumentations.augmentations.geometric.transforms.Flip)                                 | ✓     | ✓    | ✓      | ✓         |
 | [GridDistortion](https://albumentations.ai/docs/api_reference/augmentations/geometric/transforms/#albumentations.augmentations.geometric.transforms.GridDistortion)             | ✓     | ✓    | ✓      |           |
 | [GridDropout](https://albumentations.ai/docs/api_reference/augmentations/dropout/grid_dropout/#albumentations.augmentations.dropout.grid_dropout.GridDropout)                   | ✓     | ✓    |        |           |
 | [HorizontalFlip](https://albumentations.ai/docs/api_reference/augmentations/geometric/transforms/#albumentations.augmentations.geometric.transforms.HorizontalFlip)             | ✓     | ✓    | ✓      | ✓         |
 | [Lambda](https://albumentations.ai/docs/api_reference/augmentations/transforms/#albumentations.augmentations.transforms.Lambda)                                                 | ✓     | ✓    | ✓      | ✓         |
 | [LongestMaxSize](https://albumentations.ai/docs/api_reference/augmentations/geometric/resize/#albumentations.augmentations.geometric.resize.LongestMaxSize)                     | ✓     | ✓    | ✓      | ✓         |
```

### Comparing `albumentations-1.4.3/albumentations.egg-info/SOURCES.txt` & `albumentations-1.4.4/albumentations.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -37,26 +37,29 @@
 albumentations/augmentations/mixing/__init__.py
 albumentations/augmentations/mixing/functional.py
 albumentations/augmentations/mixing/transforms.py
 albumentations/core/__init__.py
 albumentations/core/bbox_utils.py
 albumentations/core/composition.py
 albumentations/core/keypoints_utils.py
+albumentations/core/pydantic.py
 albumentations/core/serialization.py
 albumentations/core/transforms_interface.py
 albumentations/core/types.py
 albumentations/core/utils.py
+albumentations/core/validation.py
 albumentations/pytorch/__init__.py
 albumentations/pytorch/transforms.py
 tests/test_augmentations.py
 tests/test_bbox.py
 tests/test_core.py
 tests/test_functional.py
 tests/test_functional_cutout.py
 tests/test_functional_mixing.py
 tests/test_keypoint.py
 tests/test_mixing.py
+tests/test_pydantic.py
 tests/test_pytorch.py
 tests/test_random.py
 tests/test_serialization.py
 tests/test_targets.py
 tests/test_transforms.py
```

### Comparing `albumentations-1.4.3/pyproject.toml` & `albumentations-1.4.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -39,14 +39,16 @@
     "dist",
     "node_modules",
     "site-packages",
     "venv",
     "tests",
     "setup.py",
     "tools",
+    "benchmark",
+    "site",
 ]
 
 line-length = 120
 indent-width = 4
 
 # Assume Python 3.8
 target-version = "py38"
@@ -120,23 +122,19 @@
     "ANN204",
     "ARG002",
     "S311",
     "F403",
     "PLR0913",
     "FBT001",
     "FBT002",
-    "ISC001",
-    "COM812",
     "ANN102",
     "EM102",
     "TRY003",
-    "D401",
     "A002",
     "PTH123",
-    "B028",
     "ARG001",
     "ARG005",
     "B028",
     "N812",
     "FBT003",
     "B027",
     "D104",
@@ -144,19 +142,16 @@
     "D103",
     "D102",
     "D415",
     "D101",
     "D205",
     "D105",
     "D417",
-    "PD901",
-    "B023",
-    "N801",
-    "T201",
-    "PERF203",
+    "D106",
+    "EM101",
 ]
 
 # Allow fix for all enabled rules (when `--fix`) is provided.
 fixable = ["ALL"]
 unfixable = []
 
 # Allow unused variables when underscore-prefixed.
@@ -175,18 +170,25 @@
 # Like Black, automatically detect the appropriate line ending.
 line-ending = "auto"
 
 [tool.ruff.lint.pydocstyle]
 convention = "google"
 
 [tool.mypy]
+plugins = ["pydantic.mypy"]
+
 python_version = "3.8"
 ignore_missing_imports = true
 follow_imports = "silent"
 warn_redundant_casts = true
 warn_unused_ignores = true
 disallow_any_generics = true
 check_untyped_defs = true
 no_implicit_reexport = true
 
 # for strict mypy: (this is the tricky one :-))
 disallow_untyped_defs = true
+
+[tool.pydantic-mypy]
+init_forbid_extra = true
+init_typed = true
+warn_required_dynamic_aliases = true
```

### Comparing `albumentations-1.4.3/setup.py` & `albumentations-1.4.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 from typing import List, Tuple
 
 from pkg_resources import DistributionNotFound, get_distribution
 from setuptools import find_packages, setup
 
 INSTALL_REQUIRES = [
     "numpy>=1.24.4", "scipy>=1.10.0", "scikit-image>=0.21.0",
-    "PyYAML", "typing-extensions>=4.9.0", "scikit-learn>=1.3.2"
+    "PyYAML", "typing-extensions>=4.9.0", "scikit-learn>=1.3.2",
+    "pydantic>=2.6.4"
 ]
 
 CHOOSE_INSTALL_REQUIRES = [
     (
         ("opencv-python>=4.9.0", "opencv-contrib-python>=4.9.0", "opencv-contrib-python-headless>=4.9.0"),
         "opencv-python-headless>=4.9.0",
     ),
```

### Comparing `albumentations-1.4.3/tests/test_augmentations.py` & `albumentations-1.4.4/tests/test_augmentations.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.3/tests/test_bbox.py` & `albumentations-1.4.4/tests/test_bbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,24 +226,24 @@
     for k, v in labels.items():
         assert transformed[k] == v
 
 
 def test_random_sized_crop_size():
     image = np.ones((100, 100, 3))
     bboxes = [(0.2, 0.3, 0.6, 0.8), (0.3, 0.4, 0.7, 0.9, 99)]
-    aug = RandomSizedCrop(min_max_height=(70, 90), height=50, width=50, p=1.0)
+    aug = RandomSizedCrop(min_max_height=(70, 90), size= (50, 50), p=1.0)
     transformed = aug(image=image, bboxes=bboxes)
     assert transformed["image"].shape == (50, 50, 3)
     assert len(bboxes) == len(transformed["bboxes"])
 
 
 def test_random_resized_crop_size():
     image = np.ones((100, 100, 3))
     bboxes = [(0.2, 0.3, 0.6, 0.8), (0.3, 0.4, 0.7, 0.9, 99)]
-    aug = RandomResizedCrop(height=50, width=50, p=1.0)
+    aug = RandomResizedCrop(size=(50, 50), p=1.0)
     transformed = aug(image=image, bboxes=bboxes)
     assert transformed["image"].shape == (50, 50, 3)
     assert len(bboxes) == len(transformed["bboxes"])
 
 
 def test_random_rotate():
     image = np.ones((192, 192, 3))
```

### Comparing `albumentations-1.4.3/tests/test_core.py` & `albumentations-1.4.4/tests/test_core.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import typing
 from unittest import mock
-from unittest.mock import MagicMock, Mock, call
+from unittest.mock import MagicMock, Mock, call, patch
+
+import albumentations as A
+from albumentations.core.composition import BaseCompose
 
 import cv2
 import numpy as np
 import pytest
 
 from albumentations import (
     BasicTransform,
@@ -29,17 +32,17 @@
     PerChannel,
     ReplayCompose,
     Sequential,
     SomeOf,
 )
 from albumentations.core.transforms_interface import (
     DualTransform,
-    ImageOnlyTransform,
-    to_tuple,
+    ImageOnlyTransform
 )
+from albumentations.core.utils import to_tuple
 
 from .utils import get_filtered_transforms
 
 
 def test_one_or_other():
     first = MagicMock()
     second = MagicMock()
@@ -100,22 +103,26 @@
     transforms = [Mock(side_effect=lambda **kw: kw) for _ in range(10)]
     augmentation = Sequential(transforms, p=1)
     image = np.ones((8, 8))
     augmentation(image=image)
     assert len([transform for transform in transforms if transform.called]) == len(transforms)
 
 
-def test_to_tuple():
-    assert to_tuple(10) == (-10, 10)
-    assert to_tuple(0.5) == (-0.5, 0.5)
-    assert to_tuple((-20, 20)) == (-20, 20)
-    assert to_tuple([-20, 20]) == (-20, 20)
-    assert to_tuple(100, low=30) == (30, 100)
-    assert to_tuple(10, bias=1) == (-9, 11)
-    assert to_tuple(100, bias=2) == (-98, 102)
+@pytest.mark.parametrize("input,kwargs,expected", [
+    (10, {}, (-10, 10)),
+    (0.5, {}, (-0.5, 0.5)),
+    ((-20, 20), {}, (-20, 20)),
+    ([-20, 20], {}, (-20, 20)),
+    ((1, 2), {"low": 1}, (1, 2)),
+    (100, {"low": 30}, (30, 100)),
+    (10, {"bias": 1}, (-9, 11)),
+    (100, {"bias": 2}, (-98, 102)),
+])
+def test_to_tuple(input, kwargs, expected):
+    assert to_tuple(input, **kwargs) == expected
 
 
 def test_image_only_transform(image, mask):
     height, width = image.shape[:2]
     with mock.patch.object(ImageOnlyTransform, "apply") as mocked_apply:
         with mock.patch.object(ImageOnlyTransform, "get_params", return_value={"interpolation": cv2.INTER_LINEAR}):
             aug = ImageOnlyTransform(p=1)
@@ -260,14 +267,20 @@
 def test_targets_type_check(targets, additional_targets, err_message):
     aug = Compose([], additional_targets=additional_targets)
 
     with pytest.raises(TypeError) as exc_info:
         aug(**targets)
     assert str(exc_info.value) == err_message
 
+    aug = Compose([])
+    aug.add_targets(additional_targets)
+    with pytest.raises(TypeError) as exc_info:
+        aug(**targets)
+    assert str(exc_info.value) == err_message
+
 
 @pytest.mark.parametrize(
     ["targets", "bbox_params", "keypoint_params", "expected"],
     [
         [
             {"keypoints": [[10, 10], [70, 70], [10, 70], [70, 10]]},
             None,
@@ -428,7 +441,58 @@
         "Height and Width of image, mask or masks should be equal. "
         "You can disable shapes check by setting a parameter is_check_shapes=False "
         "of Compose class (do it only if you are sure about your data consistency)."
     )
     # test after disabling shapes check
     transforms = Compose([], is_check_shapes=False)
     transforms(**targets)
+
+
+def test_additional_targets():
+    """Check add_target rises error if trying add existing target."""
+    transforms = Compose([], additional_targets={"image2": "image"})
+    # add same name, same target, OK
+    transforms.add_targets({"image2": "image"})
+    with pytest.raises(ValueError) as exc_info:
+        transforms.add_targets({"image2": "mask"})
+    assert str(exc_info.value) == "Trying to overwrite existed additional targets. Key=image2 Exists=image New value: mask"
+
+
+# Test 1: Probability 1 with HorizontalFlip
+def test_sequential_with_horizontal_flip_prob_1(image, mask):
+    # Setup transformations
+    transform = Sequential([HorizontalFlip(p=1)], p=1)
+    expected_transform = Compose([HorizontalFlip(p=1)])
+
+    with patch('random.random', return_value=0.1):  # Mocking probability less than 1
+        result = transform(image=image, mask=mask)
+        expected = expected_transform(image=image, mask=mask)
+
+    assert np.array_equal(result['image'], expected['image'])
+    assert np.array_equal(result['mask'], expected['mask'])
+
+# Test 2: Probability 0 with HorizontalFlip
+def test_sequential_with_horizontal_flip_prob_0(image, mask):
+    transform = Sequential([HorizontalFlip(p=1)], p=0)
+
+    with patch('random.random', return_value=0.99):  # Mocking probability greater than 0
+        result = transform(image=image, mask=mask)
+
+    assert np.array_equal(result['image'], image)
+    assert np.array_equal(result['mask'], mask)
+
+
+# Test 3: Multiple flips and transpose
+
+@pytest.mark.parametrize("aug", [A.HorizontalFlip, A.VerticalFlip, A.Transpose])
+def test_sequential_multiple_transformations(image, mask, aug):
+    transform = A.Sequential([
+        aug(p=1),
+        aug(p=1),
+    ], p=1)
+
+    with patch('random.random', return_value=0.1):  # Ensuring all transforms are applied
+        result = transform(image=image, mask=mask)
+
+    # Since HorizontalFlip, VerticalFlip, and Transpose are all applied twice, the image should be the same
+    assert np.array_equal(result['image'], image)
+    assert np.array_equal(result['mask'], mask)
```

### Comparing `albumentations-1.4.3/tests/test_functional.py` & `albumentations-1.4.4/tests/test_functional.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+import hashlib
 import cv2
 import numpy as np
 import pytest
 from numpy.testing import assert_array_almost_equal_nulp, assert_almost_equal
+import skimage
 
 import albumentations as A
 import albumentations.augmentations.functional as F
 import albumentations.augmentations.geometric.functional as FGeometric
 from albumentations.augmentations.utils import get_opencv_dtype_from_numpy, is_multispectral_image, MAX_VALUES_BY_DTYPE
 from albumentations.core.bbox_utils import filter_bboxes
-from tests.utils import convert_2d_to_target_format
+from albumentations.core.types import d4_group_elements
+from tests.utils import convert_2d_to_target_format, set_seed
 
 
 @pytest.mark.parametrize("target", ["image", "mask"])
 def test_vflip(target):
     img = np.array([[1, 1, 1], [0, 1, 1], [0, 0, 1]], dtype=np.uint8)
     expected = np.array([[0, 0, 1], [0, 1, 1], [1, 1, 1]], dtype=np.uint8)
     img, expected = convert_2d_to_target_format([img, expected], target=target)
@@ -103,33 +106,107 @@
 
 def test_normalize():
     img = np.ones((100, 100, 3), dtype=np.uint8) * 127
     normalized = F.normalize(img, mean=50, std=3)
     expected = (np.ones((100, 100, 3), dtype=np.float32) * 127 / 255 - 50) / 3
     assert_array_almost_equal_nulp(normalized, expected)
 
+# Parameterize tests for all combinations
+@pytest.mark.parametrize("shape", [
+    (100, 100),  # height, width
+    (100, 100, 1),  # height, width, 1 channel
+    (100, 100, 3),  # height, width, 3 channels
+    (100, 100, 7),  # height, width, 7 channels
+])
+@pytest.mark.parametrize("normalization", [
+    "image",
+    "image_per_channel",
+    "min_max",
+    "min_max_per_channel",
+])
+@pytest.mark.parametrize("dtype", [
+    np.uint8,
+    np.float32,
+])
+def test_normalize_per_image(shape, normalization, dtype):
+    # Generate a random image of the specified shape and dtype
+    if dtype is np.uint8:
+        img = np.random.randint(0, 256, size=shape, dtype=dtype)
+    else:  # float32
+        img = np.random.random(size=shape).astype(dtype) * 255
+
+    # Normalize the image
+    normalized_img = F.normalize_per_image(img, normalization)
+
+    # Assert the output shape matches the input shape
+    assert normalized_img.shape == img.shape, "Output shape should match input shape"
+    assert normalized_img.dtype == np.float32, "Output dtype should be float32"
+
+    # Additional checks based on normalization type
+    if normalization in ["min_max", "min_max_per_channel"]:
+        # For min-max normalization, values should be in [0, 1]
+        assert normalized_img.min() >= 0, "Min value should be >= 0"
+        assert normalized_img.max() <= 1, "Max value should be <= 1"
+    elif normalization in ["image", "image_per_channel"]:
+        # For other normalizations, just ensure output dtype is float32
+        # and check for expected normalization effects
+        assert normalized_img.dtype == np.float32, "Output dtype should be float32"
+        if normalization == "image":
+            assert np.isclose(normalized_img.mean(), 0, atol=1e-3), "Mean should be close to 0 for 'image' normalization"
+            assert np.isclose(normalized_img.std(), 1, atol=1e-3), "STD should be close to 1 for 'image' normalization"
+        elif normalization == "image_per_channel":
+            # Check channel-wise normalization for multi-channel images
+            if len(shape) == 3 and shape[2] > 1:
+                for c in range(shape[2]):
+                    channel_mean = normalized_img[:, :, c].mean()
+                    channel_std = normalized_img[:, :, c].std()
+                    assert np.isclose(channel_mean, 0, atol=1e-3), f"Mean for channel {c} should be close to 0"
+                    assert np.isclose(channel_std, 1, atol=1e-3), f"STD for channel {c} should be close to 1"
+
 
 def test_normalize_float():
     img = np.ones((100, 100, 3), dtype=np.float32) * 0.4
     normalized = F.normalize(img, mean=50, std=3, max_pixel_value=1.0)
     expected = (np.ones((100, 100, 3), dtype=np.float32) * 0.4 - 50) / 3
     assert_array_almost_equal_nulp(normalized, expected)
 
 
-def test_compare_rotate_and_shift_scale_rotate(image):
-    rotated_img_1 = FGeometric.rotate(image, angle=60)
-    rotated_img_2 = FGeometric.shift_scale_rotate(image, angle=60, scale=1, dx=0, dy=0)
-    assert np.array_equal(rotated_img_1, rotated_img_2)
-
-
-def test_compare_rotate_float_and_shift_scale_rotate_float(float_image):
-    rotated_img_1 = FGeometric.rotate(float_image, angle=60)
-    rotated_img_2 = FGeometric.shift_scale_rotate(float_image, angle=60, scale=1, dx=0, dy=0)
-    assert np.array_equal(rotated_img_1, rotated_img_2)
+def generate_rotation_matrix(image: np.ndarray, angle: float) -> np.ndarray:
+    """
+    Generates a rotation matrix for the given angle with rotation around the center of the image.
+    """
+    height, width = image.shape[:2]
+    center = (width / 2 - 0.5, height / 2 - 0.5)
+    return cv2.getRotationMatrix2D(center, angle, 1.0)
+
+@pytest.mark.parametrize("image_type", ['image', 'float_image'])
+def test_compare_rotate_and_affine_with_fixtures(request, image_type):
+    test_image = request.getfixturevalue(image_type)
+    # Generate the rotation matrix for a 60-degree rotation around the image center
+    rotation_matrix = generate_rotation_matrix(test_image, 60)
+
+    # Apply rotation using FGeometric.rotate
+    rotated_img_1 = FGeometric.rotate(test_image, angle=60, border_mode = cv2.BORDER_CONSTANT, value = 0)
+
+    # Convert 2x3 cv2 matrix to 3x3 for skimage's ProjectiveTransform
+    full_matrix = np.vstack([rotation_matrix, [0, 0, 1]])
+    projective_transform = skimage.transform.ProjectiveTransform(matrix=full_matrix)
+
+    # Apply rotation using warp_affine
+    rotated_img_2 = FGeometric.warp_affine(
+        img=test_image,
+        matrix=projective_transform,
+        interpolation=cv2.INTER_LINEAR,
+        cval=0,
+        mode=cv2.BORDER_CONSTANT,
+        output_shape=test_image.shape[:2]
+    )
 
+    # Assert that the two rotated images are equal
+    assert np.array_equal(rotated_img_1, rotated_img_2), "Rotated images should be identical."
 
 @pytest.mark.parametrize("target", ["image", "mask"])
 def test_center_crop(target):
     img = np.array([[1, 1, 1, 1], [0, 1, 1, 1], [0, 0, 1, 1], [0, 0, 0, 1]], dtype=np.uint8)
     expected = np.array([[1, 1], [0, 1]], dtype=np.uint8)
     img, expected = convert_2d_to_target_format([img, expected], target=target)
     cropped_img = A.center_crop(img, 2, 2)
@@ -222,127 +299,14 @@
         [[0.4, 0.3, 0.4, 0.3], [0.2, 0.1, 0.2, 0.1], [0.4, 0.3, 0.4, 0.3], [0.2, 0.1, 0.2, 0.1]], dtype=np.float32
     )
     img, expected = convert_2d_to_target_format([img, expected], target=target)
     padded_img = FGeometric.pad(img, min_height=4, min_width=4)
     assert_array_almost_equal_nulp(padded_img, expected)
 
 
-@pytest.mark.parametrize("target", ["image", "mask"])
-def test_rotate_from_shift_scale_rotate(target):
-    img = np.array([[1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12], [13, 14, 15, 16]], dtype=np.uint8)
-    expected = np.array([[4, 8, 12, 16], [3, 7, 11, 15], [2, 6, 10, 14], [1, 5, 9, 13]], dtype=np.uint8)
-
-    img, expected = convert_2d_to_target_format([img, expected], target=target)
-    rotated_img = FGeometric.shift_scale_rotate(
-        img, angle=90, scale=1, dx=0, dy=0, interpolation=cv2.INTER_NEAREST, border_mode=cv2.BORDER_CONSTANT
-    )
-    assert np.array_equal(rotated_img, expected)
-
-
-@pytest.mark.parametrize("target", ["image", "image_4_channels"])
-def test_rotate_float_from_shift_scale_rotate(target):
-    img = np.array(
-        [[0.01, 0.02, 0.03, 0.04], [0.05, 0.06, 0.07, 0.08], [0.09, 0.10, 0.11, 0.12], [0.13, 0.14, 0.15, 0.16]],
-        dtype=np.float32,
-    )
-    expected = np.array(
-        [[0.04, 0.08, 0.12, 0.16], [0.03, 0.07, 0.11, 0.15], [0.02, 0.06, 0.10, 0.14], [0.01, 0.05, 0.09, 0.13]],
-        dtype=np.float32,
-    )
-    img, expected = convert_2d_to_target_format([img, expected], target=target)
-    rotated_img = FGeometric.shift_scale_rotate(
-        img, angle=90, scale=1, dx=0, dy=0, interpolation=cv2.INTER_NEAREST, border_mode=cv2.BORDER_CONSTANT
-    )
-    assert_array_almost_equal_nulp(rotated_img, expected)
-
-
-@pytest.mark.parametrize("target", ["image", "mask"])
-def test_scale_from_shift_scale_rotate(target):
-    img = np.array([[1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12], [13, 14, 15, 16]], dtype=np.uint8)
-    expected = np.array([[6, 6, 7, 7], [6, 6, 7, 7], [10, 10, 11, 11], [10, 10, 11, 11]], dtype=np.uint8)
-    img, expected = convert_2d_to_target_format([img, expected], target=target)
-    scaled_img = FGeometric.shift_scale_rotate(
-        img, angle=0, scale=2, dx=0, dy=0, interpolation=cv2.INTER_NEAREST, border_mode=cv2.BORDER_CONSTANT
-    )
-    assert np.array_equal(scaled_img, expected)
-
-
-@pytest.mark.parametrize("target", ["image", "image_4_channels"])
-def test_scale_float_from_shift_scale_rotate(target):
-    img = np.array(
-        [[0.01, 0.02, 0.03, 0.04], [0.05, 0.06, 0.07, 0.08], [0.09, 0.10, 0.11, 0.12], [0.13, 0.14, 0.15, 0.16]],
-        dtype=np.float32,
-    )
-    expected = np.array(
-        [[0.06, 0.06, 0.07, 0.07], [0.06, 0.06, 0.07, 0.07], [0.10, 0.10, 0.11, 0.11], [0.10, 0.10, 0.11, 0.11]],
-        dtype=np.float32,
-    )
-    img, expected = convert_2d_to_target_format([img, expected], target=target)
-    scaled_img = FGeometric.shift_scale_rotate(
-        img, angle=0, scale=2, dx=0, dy=0, interpolation=cv2.INTER_NEAREST, border_mode=cv2.BORDER_CONSTANT
-    )
-    assert_array_almost_equal_nulp(scaled_img, expected)
-
-
-@pytest.mark.parametrize("target", ["image", "mask"])
-def test_shift_x_from_shift_scale_rotate(target):
-    img = np.array([[1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12], [13, 14, 15, 16]], dtype=np.uint8)
-    expected = np.array([[0, 0, 1, 2], [0, 0, 5, 6], [0, 0, 9, 10], [0, 0, 13, 14]], dtype=np.uint8)
-    img, expected = convert_2d_to_target_format([img, expected], target=target)
-    shifted_along_x_img = FGeometric.shift_scale_rotate(
-        img, angle=0, scale=1, dx=0.5, dy=0, interpolation=cv2.INTER_NEAREST, border_mode=cv2.BORDER_CONSTANT
-    )
-    assert np.array_equal(shifted_along_x_img, expected)
-
-
-@pytest.mark.parametrize("target", ["image", "image_4_channels"])
-def test_shift_x_float_from_shift_scale_rotate(target):
-    img = np.array(
-        [[0.01, 0.02, 0.03, 0.04], [0.05, 0.06, 0.07, 0.08], [0.09, 0.10, 0.11, 0.12], [0.13, 0.14, 0.15, 0.16]],
-        dtype=np.float32,
-    )
-    expected = np.array(
-        [[0.00, 0.00, 0.01, 0.02], [0.00, 0.00, 0.05, 0.06], [0.00, 0.00, 0.09, 0.10], [0.00, 0.00, 0.13, 0.14]],
-        dtype=np.float32,
-    )
-    img, expected = convert_2d_to_target_format([img, expected], target=target)
-    shifted_along_x_img = FGeometric.shift_scale_rotate(
-        img, angle=0, scale=1, dx=0.5, dy=0, interpolation=cv2.INTER_NEAREST, border_mode=cv2.BORDER_CONSTANT
-    )
-    assert_array_almost_equal_nulp(shifted_along_x_img, expected)
-
-
-@pytest.mark.parametrize("target", ["image", "mask"])
-def test_shift_y_from_shift_scale_rotate(target):
-    img = np.array([[1, 2, 3, 4], [5, 6, 7, 8], [9, 10, 11, 12], [13, 14, 15, 16]], dtype=np.uint8)
-    expected = np.array([[0, 0, 0, 0], [0, 0, 0, 0], [1, 2, 3, 4], [5, 6, 7, 8]], dtype=np.uint8)
-    img, expected = convert_2d_to_target_format([img, expected], target=target)
-    shifted_along_y_img = FGeometric.shift_scale_rotate(
-        img, angle=0, scale=1, dx=0, dy=0.5, interpolation=cv2.INTER_NEAREST, border_mode=cv2.BORDER_CONSTANT
-    )
-    assert np.array_equal(shifted_along_y_img, expected)
-
-
-@pytest.mark.parametrize("target", ["image", "image_4_channels"])
-def test_shift_y_float_from_shift_scale_rotate(target):
-    img = np.array(
-        [[0.01, 0.02, 0.03, 0.04], [0.05, 0.06, 0.07, 0.08], [0.09, 0.10, 0.11, 0.12], [0.13, 0.14, 0.15, 0.16]],
-        dtype=np.float32,
-    )
-    expected = np.array(
-        [[0.00, 0.00, 0.00, 0.00], [0.00, 0.00, 0.00, 0.00], [0.01, 0.02, 0.03, 0.04], [0.05, 0.06, 0.07, 0.08]],
-        dtype=np.float32,
-    )
-    img, expected = convert_2d_to_target_format([img, expected], target=target)
-    shifted_along_y_img = FGeometric.shift_scale_rotate(
-        img, angle=0, scale=1, dx=0, dy=0.5, interpolation=cv2.INTER_NEAREST, border_mode=cv2.BORDER_CONSTANT
-    )
-    assert_array_almost_equal_nulp(shifted_along_y_img, expected)
-
-
 @pytest.mark.parametrize(
     ["shift_params", "expected"], [[(-10, 0, 10), (117, 127, 137)], [(-200, 0, 200), (0, 127, 255)]]
 )
 def test_shift_rgb(shift_params, expected):
     img = np.ones((100, 100, 3), dtype=np.uint8) * 127
     r_shift, g_shift, b_shift = shift_params
     img = F.shift_rgb(img, r_shift=r_shift, g_shift=g_shift, b_shift=b_shift)
@@ -687,16 +651,18 @@
     assert FGeometric.bbox_rot90((0.1, 0.2, 0.3, 0.4), 0, 100, 200) == (0.1, 0.2, 0.3, 0.4)
     assert FGeometric.bbox_rot90((0.1, 0.2, 0.3, 0.4), 1, 100, 200) == (0.2, 0.7, 0.4, 0.9)
     assert FGeometric.bbox_rot90((0.1, 0.2, 0.3, 0.4), 2, 100, 200) == (0.7, 0.6, 0.9, 0.8)
     assert FGeometric.bbox_rot90((0.1, 0.2, 0.3, 0.4), 3, 100, 200) == (0.6, 0.1, 0.8, 0.3)
 
 
 def test_bbox_transpose():
-    assert np.allclose(FGeometric.bbox_transpose((0.7, 0.1, 0.8, 0.4), 0, 100, 200), (0.1, 0.7, 0.4, 0.8))
-    assert np.allclose(FGeometric.bbox_transpose((0.7, 0.1, 0.8, 0.4), 1, 100, 200), (0.6, 0.2, 0.9, 0.3))
+    assert np.allclose(FGeometric.bbox_transpose((0.7, 0.1, 0.8, 0.4), 100, 200), (0.1, 0.7, 0.4, 0.8))
+    rot90 = FGeometric.bbox_rot90((0.7, 0.1, 0.8, 0.4), 2, 100, 200)
+    reflected_anti_diagonal = FGeometric.bbox_transpose(rot90, 100, 200)
+    assert np.allclose(reflected_anti_diagonal, (0.6, 0.2, 0.9, 0.3))
 
 
 @pytest.mark.parametrize(
     ["bboxes", "min_area", "min_visibility", "target"],
     [
         (
             [(0.1, 0.5, 1.1, 0.9), (-0.1, 0.5, 0.8, 0.9), (0.1, 0.5, 0.8, 0.9)],
@@ -838,49 +804,63 @@
 
     assert np.array_equal(
         F.brightness_contrast_adjust(image_float), F._brightness_contrast_adjust_non_uint(image_float)
     )
 
 
 @pytest.mark.parametrize(
-    "img, tiles, expected",
+    "img, tiles, mapping, expected",
     [
         # Test with empty tiles - image should remain unchanged
         (
             np.array([[1, 1], [2, 2]], dtype=np.uint8),
             np.empty((0, 4), dtype=np.int32),
+            [0],
+            np.array([[1, 1], [2, 2]], dtype=np.uint8)
+        ),
+
+        # Test with empty mapping - image should remain unchanged
+        (
+            np.array([[1, 1], [2, 2]], dtype=np.uint8),
+            np.array([[0, 0, 2, 2]]),
+            None,
             np.array([[1, 1], [2, 2]], dtype=np.uint8)
         ),
 
         # Test with one tile that covers the whole image - should behave as if the image is unchanged
         (
             np.array([[1, 1], [2, 2]], dtype=np.uint8),
             np.array([[0, 0, 2, 2]]),
+            [0],
             np.array([[1, 1], [2, 2]], dtype=np.uint8)
         ),
 
-        # Test with splitting tiles horizontally - since we're not actually swapping, the expected result should match the original
+        # Test with splitting tiles horizontally
         (
             np.array([[1, 2], [3, 4]], dtype=np.uint8),
             np.array([[0, 0, 2, 1], [0, 1, 2, 2]]),
-            np.array([[1, 2], [3, 4]], dtype=np.uint8)  # Corrected expectation
+            [1, 0],
+            np.array([[2, 1], [4, 3]], dtype=np.uint8)  # Corrected expectation
         ),
 
-        # Test with splitting tiles vertically - similarly, expect original image as output
+        # Test with splitting tiles vertically
         (
             np.array([[1, 2], [3, 4]], dtype=np.uint8),
             np.array([[0, 0, 1, 2], [1, 0, 2, 2]]),
-            np.array([[1, 2], [3, 4]], dtype=np.uint8)  # Corrected expectation
+            [1, 0],
+            np.array([[3, 4], [1, 2]], dtype=np.uint8)  # Corrected expectation
         ),
 
+        # Test with splitting tiles diag
+
         # Other tests remain the same if they correctly represent what your function does
     ]
 )
-def test_swap_tiles_on_image(img, tiles, expected):
-    result_img = F.swap_tiles_on_image(img, tiles)
+def test_swap_tiles_on_image(img, tiles, mapping, expected):
+    result_img = F.swap_tiles_on_image(img, tiles, mapping)
     assert np.array_equal(result_img, expected)
 
 
 @pytest.mark.parametrize("dtype", list(F.MAX_VALUES_BY_DTYPE.keys()))
 def test_solarize(dtype):
     max_value = F.MAX_VALUES_BY_DTYPE[dtype]
 
@@ -917,18 +897,14 @@
         F.posterize(img, [1, 2, 3])
     assert str(exc_info.value) == "If bits is iterable image must be RGB"
 
 
 def test_equalize_checks():
     img = np.random.randint(0, 255, [256, 256], dtype=np.uint8)
 
-    with pytest.raises(ValueError) as exc_info:
-        F.equalize(img, mode="other")
-    assert str(exc_info.value) == "Unsupported equalization mode. Supports: ['cv', 'pil']. Got: other"
-
     mask = np.random.randint(0, 1, [256, 256, 3], dtype=bool)
     with pytest.raises(ValueError) as exc_info:
         F.equalize(img, mask=mask)
     assert str(exc_info.value) == f"Wrong mask shape. Image shape: {img.shape}. Mask shape: {mask.shape}"
 
     img = np.random.randint(0, 255, [256, 256, 3], dtype=np.uint8)
     with pytest.raises(ValueError) as exc_info:
@@ -1129,9 +1105,171 @@
             [0, 0, 35, 51], [0, 51, 35, 102], [0, 102, 35, 153], [0, 153, 35, 205],  # First row splits
             [35, 0, 70, 51], [35, 51, 70, 102], [35, 102, 70, 153], [35, 153, 70, 205],  # Second row splits
             [70, 0, 105, 51], [70, 51, 105, 102], [70, 102, 105, 153], [70, 153, 105, 205]  # Third row splits
         ])),
     ]
 )
 def test_split_uniform_grid(image_shape, grid, expected):
-    result = F.split_uniform_grid(image_shape, grid)
+    random_seed = 42
+    result = F.split_uniform_grid(image_shape, grid, random_state=np.random.RandomState(random_seed))
     np.testing.assert_array_equal(result, expected)
+
+
+@pytest.mark.parametrize("size, divisions, random_state, expected", [
+    (10, 2, None, [0, 5, 10]),
+    (10, 2, 42, [0, 5, 10]),  # Consistent shuffling with seed
+    (9, 3, None, [0, 3, 6, 9]),
+    (9, 3, 42, [0, 3, 6, 9]),  # Expected shuffle result with a specific seed
+    (20, 5, 42, [0, 4, 8, 12, 16, 20]),  # Regular intervals
+    (7, 3, 42, [0, 3, 5, 7]),  # Irregular intervals, specific seed
+    (7, 3, 41, [0, 2, 4, 7]),  # Irregular intervals, specific seed
+])
+def test_generate_shuffled_splits(size, divisions, random_state, expected):
+    result = F.generate_shuffled_splits(size, divisions, random_state=np.random.RandomState(random_state) if random_state else None)
+    assert len(result) == divisions + 1
+    assert np.array_equal(result, expected), f"Failed for size={size}, divisions={divisions}, random_state={random_state}"
+
+@pytest.mark.parametrize("size, divisions, random_state", [
+    (10, 2, 42),
+    (9, 3, 99),
+    (20, 5, 101),
+    (7, 3, 42),
+])
+def test_consistent_shuffling(size, divisions, random_state):
+    set_seed(random_state)
+    result1 = F.generate_shuffled_splits(size, divisions, random_state = np.random.RandomState(random_state))
+    assert len(result1) == divisions + 1
+    set_seed(random_state)
+    result2 = F.generate_shuffled_splits(size, divisions, random_state = np.random.RandomState(random_state))
+    assert len(result2) == divisions + 1
+    assert np.array_equal(result1, result2), "Shuffling is not consistent with the given random state"
+
+
+@pytest.mark.parametrize("tiles, expected", [
+    # Simple case with two different shapes
+    (np.array([[0, 0, 2, 2], [0, 2, 2, 4], [2, 0, 4, 2], [2, 2, 4, 4]]),
+     {(2, 2): [0, 1, 2, 3]}),
+    # Tiles with three different shapes
+    (np.array([[0, 0, 1, 3], [0, 3, 1, 6], [1, 0, 4, 3], [1, 3, 4, 6]]),
+     {(1, 3): [0, 1], (3, 3): [2, 3]}),
+    # Single tile
+    (np.array([[0, 0, 1, 1]]),
+     {(1, 1): [0]}),
+    # No tiles
+    (np.array([]).reshape(0, 4),
+     {}),
+    # All tiles having the same shape
+    (np.array([[0, 0, 2, 2], [2, 2, 4, 4], [4, 4, 6, 6]]),
+     {(2, 2): [0, 1, 2]}),
+])
+def test_create_shape_groups(tiles, expected):
+    result = F.create_shape_groups(tiles)
+    assert len(result) == len(expected), "Incorrect number of shape groups"
+    for shape in expected:
+        assert shape in result, f"Shape {shape} is not in the result"
+        assert sorted(result[shape]) == sorted(expected[shape]), f"Incorrect indices for shape {shape}"
+
+
+@pytest.mark.parametrize("shape_groups, random_state, expected_output", [
+    # Test with a simple case of one group
+    ({(2, 2): [0, 1, 2, 3]}, 42, [1, 3, 0, 2]),
+    # Test with multiple groups and ensure that random state affects the shuffle consistently
+    ({(2, 2): [0, 1, 2, 3], (1, 1): [4]}, 42, [1, 3, 0, 2, 4]),
+    # All tiles having the same shape should be shuffled within themselves
+    ({(2, 2): [0, 1, 2]}, 2, [2, 1, 0])
+])
+def test_shuffle_tiles_within_shape_groups(shape_groups, random_state, expected_output):
+    random_state = np.random.RandomState(random_state)
+    actual_output = F.shuffle_tiles_within_shape_groups(shape_groups, random_state)
+    assert actual_output == expected_output, "Output did not match expected mapping"
+
+
+@pytest.mark.parametrize("group_member,expected", [
+    ("e", np.array([[0, 1, 2], [3, 4, 5], [6, 7, 8]])),  # Identity
+    ("r90", np.array([[2, 5, 8], [1, 4, 7], [0, 3, 6]])),  # Rotate 90 degrees counterclockwise
+    ("r180", np.array([[8, 7, 6], [5, 4, 3], [2, 1, 0]])),  # Rotate 180 degrees
+    ("r270", np.array([[6, 3, 0], [7, 4, 1], [8, 5, 2]])),  # Rotate 270 degrees counterclockwise
+    ("v", np.array([[6, 7, 8], [3, 4, 5], [0, 1, 2]])),  # Vertical flip
+    ("t", np.array([[0, 3, 6], [1, 4, 7], [2, 5, 8]])),  # Transpose (reflect over main diagonal)
+    ("h", np.array([[2, 1, 0], [5, 4, 3], [8, 7, 6]])),  # Horizontal flip
+    ("hvt", np.array([[8, 5, 2], [7, 4, 1], [6, 3, 0]]))  # Transpose (reflect over anti-diagonal)
+])
+def test_d4_transformations(group_member, expected):
+    img = np.array([[0, 1, 2], [3, 4, 5], [6, 7, 8]], dtype=np.uint8)
+    transformed_img = FGeometric.d4(img, group_member)
+    assert np.array_equal(transformed_img, expected), f"Failed for transformation {group_member}"
+
+def get_md5_hash(image):
+    image_bytes = image.tobytes()
+    hash_md5 = hashlib.md5()
+    hash_md5.update(image_bytes)
+    return hash_md5.hexdigest()
+
+
+def test_d4_unique(image):
+    hashes = set()
+    for element in d4_group_elements:
+        hashes.add(get_md5_hash(FGeometric.d4(image, element)))
+
+    assert len(hashes) == len(set(hashes)), "d4 should generate unique images for all group elements"
+
+
+
+@pytest.mark.parametrize("bbox, group_member, rows, cols, expected", [
+    ((0.05, 0.1, 0.55, 0.6), 'e', 200, 200, (0.05, 0.1, 0.55, 0.6)),  # Identity
+    ((0.05, 0.1, 0.55, 0.6), 'r90', 200, 200, (0.1, 0.45, 0.6, 0.95)),  # Rotate 90 degrees CCW
+    ((0.05, 0.1, 0.55, 0.6), 'r180', 200, 200, (0.45, 0.4, 0.95, 0.9)),  # Rotate 180 degrees
+    ((0.05, 0.1, 0.55, 0.6), 'r270', 200, 200, (0.4, 0.05, 0.9, 0.55)),  # Rotate 270 degrees CCW
+    ((0.05, 0.1, 0.55, 0.6), 'v', 200, 200, (0.05, 0.4, 0.55, 0.9)),  # Vertical flip
+    ((0.05, 0.1, 0.55, 0.6), 't', 200, 200, (0.1, 0.05, 0.6, 0.55)),  # Transpose around main diagonal
+    ((0.05, 0.1, 0.55, 0.6), 'h', 200, 200, (0.45, 0.1, 0.95, 0.6)),  # Horizontal flip
+    ((0.05, 0.1, 0.55, 0.6), 'hvt', 200, 200, (1 - 0.6, 1 - 0.55, 1 - 0.1, 1 - 0.05)), # Transpose around second diagonal
+])
+def test_bbox_d4(bbox, group_member, rows, cols, expected):
+    result = FGeometric.bbox_d4(bbox, group_member, rows, cols)
+    assert result == pytest.approx(expected, rel=1e-5), f"Failed for transformation {group_member} with bbox {bbox}"
+
+
+@pytest.mark.parametrize("keypoint, rows, cols", [
+    ((100, 150, 0, 1), 300, 400),  # Example keypoint with arbitrary angle and scale
+    ((200, 100, np.pi/4, 0.5), 300, 400),
+    ((50, 250, np.pi/2, 2), 300, 400),
+])
+def test_keypoint_vh_flip_equivalence(keypoint, rows, cols):
+
+    # Perform vertical and then horizontal flip
+    hflipped_keypoint = FGeometric.keypoint_hflip(keypoint, rows, cols)
+    vhflipped_keypoint = FGeometric.keypoint_vflip(hflipped_keypoint, rows, cols)
+
+    vflipped_keypoint = FGeometric.keypoint_vflip(keypoint, rows, cols)
+    hvflipped_keypoint = FGeometric.keypoint_hflip(vflipped_keypoint, rows, cols)
+
+    assert vhflipped_keypoint == pytest.approx(hvflipped_keypoint), "Sequential vflip + hflip not equivalent to hflip + vflip"
+    assert vhflipped_keypoint == pytest.approx(FGeometric.keypoint_rot90(keypoint, 2, rows, cols)), "rot180 not equivalent to vflip + hflip"
+
+
+base_matrix = np.array([[1, 2, 3],
+                        [4, 5, 6],
+                        [7, 8, 9]])
+expected_main_diagonal = np.array([[1, 4, 7],
+                                   [2, 5, 8],
+                                   [3, 6, 9]])
+expected_second_diagonal = np.array([[9, 6, 3],
+                                     [8, 5, 2],
+                                     [7, 4, 1]])
+
+def create_test_matrix(matrix, shape):
+    if len(shape) == 2:
+        return matrix
+    elif len(shape) == 3:
+        return np.stack([matrix] * shape[2], axis=-1)
+
+
+@pytest.mark.parametrize("shape", [(3, 3), (3, 3, 1), (3, 3, 3), (3, 3, 7)])
+def test_transpose(shape):
+    img = create_test_matrix(base_matrix, shape)
+    expected_main = create_test_matrix(expected_main_diagonal, shape)
+    expected_second = create_test_matrix(expected_second_diagonal, shape)
+
+    assert np.array_equal(FGeometric.transpose(img), expected_main)
+    transposed_axis1 = FGeometric.transpose(FGeometric.rot90(img, 2))
+    assert np.array_equal(transposed_axis1, expected_second)
```

### Comparing `albumentations-1.4.3/tests/test_functional_cutout.py` & `albumentations-1.4.4/tests/test_functional_cutout.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.3/tests/test_functional_mixing.py` & `albumentations-1.4.4/tests/test_functional_mixing.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 import pytest
-from albumentations.augmentations.mixing.functional import mix_arrays
+from albumentations.augmentations.functional import add_weighted
+
 
 def find_mix_coef(r: np.ndarray, array1: np.ndarray, array2: np.ndarray) -> float:
     """
     Finds the mixing coefficient used to combine array1 and array2 into r,
     based on the cv2.addWeighted operation.
 
     Args:
@@ -41,16 +42,16 @@
 
         # Test case 3: First array is of shape (100, 100), second array is of shape (100, 100, 1)
         (np.zeros((100, 100)), np.ones((100, 100, 1)), 0.5, (100, 100)),
 
         # Additional test cases can be added here.
     ]
 )
-def test_mix_arrays_shapes(array1, array2, mix_coef, expected_shape):
-    result = mix_arrays(array1, array2, mix_coef)
+def test_add_weighted_shapes(array1, array2, mix_coef, expected_shape):
+    result = add_weighted(array1, mix_coef, array2, 1 - mix_coef)
     assert result.shape == expected_shape, f"Expected shape {expected_shape}, got {result.shape}"
 
     # Additionally, you can check if the result type matches the first array type
     assert result.dtype == array1.dtype, f"Expected dtype {array1.dtype}, got {result.dtype}"
 
     deduced_mix_coef = find_mix_coef(result, array1, array2)
```

### Comparing `albumentations-1.4.3/tests/test_keypoint.py` & `albumentations-1.4.4/tests/test_keypoint.py`

 * *Files 8% similar despite different names*

```diff
@@ -150,24 +150,24 @@
     for k, v in labels.items():
         assert transformed[k] == v
 
 
 def test_random_sized_crop_size():
     image = np.ones((100, 100, 3))
     keypoints = [(0.2, 0.3, 0.6, 0.8), (0.3, 0.4, 0.7, 0.9, 99)]
-    aug = A.RandomSizedCrop(min_max_height=(70, 90), height=50, width=50, p=1.0)
+    aug = A.RandomSizedCrop(min_max_height=(70, 90), size=(50, 50), p=1.0)
     transformed = aug(image=image, keypoints=keypoints)
     assert transformed["image"].shape == (50, 50, 3)
     assert len(keypoints) == len(transformed["keypoints"])
 
 
 def test_random_resized_crop_size():
     image = np.ones((100, 100, 3))
     keypoints = [(0.2, 0.3, 0.6, 0.8), (0.3, 0.4, 0.7, 0.9, 99)]
-    aug = A.RandomResizedCrop(height=50, width=50, p=1.0)
+    aug = A.RandomResizedCrop(size=(50, 50), p=1.0)
     transformed = aug(image=image, keypoints=keypoints)
     assert transformed["image"].shape == (50, 50, 3)
     assert len(keypoints) == len(transformed["keypoints"])
 
 
 @pytest.mark.parametrize(
     ["aug", "keypoints", "expected"],
@@ -255,32 +255,29 @@
     ],
 )
 def test_keypoint_scale(keypoint, expected, scale):
     actual = FGeometric.keypoint_scale(keypoint, scale, scale)
     np.testing.assert_allclose(actual, expected, atol=1e-7)
 
 
-@pytest.mark.parametrize(
-    ["keypoint", "expected", "angle", "scale", "dx", "dy"],
-    [[[50, 50, 0, 5], [120, 158, math.pi / 2, 10], 90, 2, 0.1, 0.1]],
-)
-def test_keypoint_shift_scale_rotate(keypoint, expected, angle, scale, dx, dy):
-    actual = FGeometric.keypoint_shift_scale_rotate(keypoint, angle, scale, dx, dy, rows=100, cols=200)
-    np.testing.assert_allclose(actual, expected, rtol=1e-4)
-
-
 def test_compose_with_additional_targets():
     image = np.ones((100, 100, 3))
     keypoints = [(10, 10), (50, 50)]
     kp1 = [(15, 15), (55, 55)]
+
     aug = A.Compose([A.CenterCrop(50, 50)], keypoint_params={"format": "xy"}, additional_targets={"kp1": "keypoints"})
     transformed = aug(image=image, keypoints=keypoints, kp1=kp1)
     assert transformed["keypoints"] == [(25, 25)]
     assert transformed["kp1"] == [(30, 30)]
 
+    aug = A.Compose([A.CenterCrop(50, 50)], keypoint_params={"format": "xy"})
+    aug.add_targets( additional_targets={"kp1": "keypoints"})
+    transformed = aug(image=image, keypoints=keypoints, kp1=kp1)
+    assert transformed["keypoints"] == [(25, 25)]
+    assert transformed["kp1"] == [(30, 30)]
 
 @pytest.mark.parametrize(
     ["angle", "expected"],
     [
         [0, 0],
         [np.pi / 2, np.pi / 2],
         [np.pi, np.pi],
```

### Comparing `albumentations-1.4.3/tests/test_mixing.py` & `albumentations-1.4.4/tests/test_mixing.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.3/tests/test_pytorch.py` & `albumentations-1.4.4/tests/test_pytorch.py`

 * *Files 9% similar despite different names*

```diff
@@ -76,14 +76,40 @@
             image2_width,
         )
         assert isinstance(res["mask"], torch.Tensor) and res["mask"].shape == mask1.shape
         assert isinstance(res["mask2"], torch.Tensor) and res["mask2"].shape == mask2.shape
         assert np.array_equal(res["image"], res["image2"])
         assert np.array_equal(res["mask"], res["mask2"])
 
+    aug = A.Compose([ToTensorV2()])
+    aug.add_targets(additional_targets={"image2": "image", "mask2": "mask"})
+    for _i in range(10):
+        image1 = np.random.randint(low=0, high=256, size=(100, 100, 3), dtype=np.uint8)
+        image2 = image1.copy()
+        mask1 = np.random.randint(low=0, high=256, size=(100, 100, 4), dtype=np.uint8)
+        mask2 = mask1.copy()
+        res = aug(image=image1, image2=image2, mask=mask1, mask2=mask2)
+
+        image1_height, image1_width, image1_num_channels = image1.shape
+        image2_height, image2_width, image2_num_channels = image2.shape
+        assert isinstance(res["image"], torch.Tensor) and res["image"].shape == (
+            image1_num_channels,
+            image1_height,
+            image1_width,
+        )
+        assert isinstance(res["image2"], torch.Tensor) and res["image2"].shape == (
+            image2_num_channels,
+            image2_height,
+            image2_width,
+        )
+        assert isinstance(res["mask"], torch.Tensor) and res["mask"].shape == mask1.shape
+        assert isinstance(res["mask2"], torch.Tensor) and res["mask2"].shape == mask2.shape
+        assert np.array_equal(res["image"], res["image2"])
+        assert np.array_equal(res["mask"], res["mask2"])
+
 
 def test_torch_to_tensor_v2_on_gray_scale_images():
     aug = ToTensorV2()
     grayscale_image = np.random.randint(low=0, high=256, size=(100, 100), dtype=np.uint8)
     data = aug(image=grayscale_image)
     assert isinstance(data["image"], torch.Tensor)
     assert len(data["image"].shape) == 3
```

### Comparing `albumentations-1.4.3/tests/test_serialization.py` & `albumentations-1.4.4/tests/test_serialization.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 import io
 from pathlib import Path
 from unittest.mock import patch
 
 import cv2
 import numpy as np
+
 import pytest
 from deepdiff import DeepDiff
-import inspect
 
 import albumentations as A
 import albumentations.augmentations.geometric.functional as FGeometric
 from albumentations.core.serialization import SERIALIZABLE_REGISTRY, shorten_class_name
 from albumentations.core.transforms_interface import ImageOnlyTransform
+from albumentations.core.types import ImageCompressionType
 
 from .utils import (
     OpenMock,
     check_all_augs_exists,
     get_image_only_transforms,
     get_transforms,
     set_seed,
 )
 
 TEST_SEEDS = (0, 1, 42)
 
-
 @pytest.mark.parametrize(
     ["augmentation_cls", "params"],
     get_transforms(
         custom_arguments={
             A.Crop: {"y_min": 0, "y_max": 10, "x_min": 0, "x_max": 10},
             A.CenterCrop: {"height": 10, "width": 10},
             A.CropNonEmptyMaskIfExists: {"height": 10, "width": 10},
             A.RandomCrop: {"height": 10, "width": 10},
-            A.RandomResizedCrop: {"height": 10, "width": 10},
-            A.RandomSizedCrop: {"min_max_height": (4, 8), "height": 10, "width": 10},
+            A.RandomResizedCrop: {"size": (10, 10)},
+            A.RandomSizedCrop: {"min_max_height": (4, 8), "size": (10, 10)},
             A.CropAndPad: {"px": 10},
             A.Resize: {"height": 10, "width": 10},
             A.XYMasking: {
                 "num_masks_x": (1, 3),
                 "num_masks_y": 3,
                 "mask_x_length": (10, 20),
                 "mask_y_length": 10,
@@ -90,15 +90,15 @@
 
 AUGMENTATION_CLS_PARAMS = [
     [
         A.ImageCompression,
         {
             "quality_lower": 10,
             "quality_upper": 80,
-            "compression_type": A.ImageCompression.ImageCompressionType.WEBP,
+            "compression_type": ImageCompressionType.WEBP,
         },
     ],
     [
         A.HueSaturationValue,
         {"hue_shift_limit": 70, "sat_shift_limit": 95, "val_shift_limit": 55},
     ],
     [A.RGBShift, {"r_shift_limit": 70, "g_shift_limit": 80, "b_shift_limit": 40}],
@@ -148,16 +148,15 @@
             "number_of_patches": 2,
         },
     ],
     [
         A.RandomShadow,
         {
             "shadow_roi": (0.1, 0.4, 0.9, 0.9),
-            "num_shadows_lower": 2,
-            "num_shadows_upper": 4,
+            "num_shadows_limit": (2, 4),
             "shadow_dimension": 8,
         },
     ],
     [
         A.PadIfNeeded,
         {
             "min_height": 512,
@@ -184,29 +183,29 @@
             "border_mode": cv2.BORDER_CONSTANT,
             "value": (10, 10, 10),
         },
     ],
     [
         A.ShiftScaleRotate,
         {
-            "shift_limit": 0.2,
-            "scale_limit": 0.2,
-            "rotate_limit": 70,
+            "shift_limit": (-0.2, 0.2),
+            "scale_limit": (-0.2, 0.2),
+            "rotate_limit": (-70, 70),
             "interpolation": cv2.INTER_CUBIC,
             "border_mode": cv2.BORDER_CONSTANT,
             "value": (10, 10, 10),
         },
     ],
     [
         A.ShiftScaleRotate,
         {
-            "shift_limit_x": 0.3,
-            "shift_limit_y": 0.4,
-            "scale_limit": 0.2,
-            "rotate_limit": 70,
+            "shift_limit_x": (-0.3, 0.3),
+            "shift_limit_y": (-0.4, 0.4),
+            "scale_limit": (-0.2, 0.2),
+            "rotate_limit": (-70, 70),
             "interpolation": cv2.INTER_CUBIC,
             "border_mode": cv2.BORDER_CONSTANT,
             "value": (10, 10, 10),
         },
     ],
     [
         A.OpticalDistortion,
@@ -253,15 +252,15 @@
             "max_pixel_value": 100.0,
         },
     ],
     [A.RandomScale, {"scale_limit": 0.2, "interpolation": cv2.INTER_CUBIC}],
     [A.Resize, {"height": 64, "width": 64}],
     [A.SmallestMaxSize, {"max_size": 64, "interpolation": cv2.INTER_CUBIC}],
     [A.LongestMaxSize, {"max_size": 128, "interpolation": cv2.INTER_CUBIC}],
-    [A.RandomGridShuffle, {"grid": (5, 5)}],
+    [A.RandomGridShuffle, {"grid": (4, 4)}],
     [A.Solarize, {"threshold": 32}],
     [A.Posterize, {"num_bits": 1}],
     [A.Equalize, {"mode": "pil", "by_channels": False}],
     [
         A.MultiplicativeNoise,
         {"multiplier": (0.7, 2.3), "per_channel": True, "elementwise": True},
     ],
@@ -446,15 +445,16 @@
             shift_x=10,
             shift_y=20,
             random_offset=True,
             fill_value=10,
             mask_fill_value=20,
         )
     ],
-    [A.Morphological, {}]
+    [A.Morphological, {}],
+    [A.D4, {}]
 ]
 
 AUGMENTATION_CLS_EXCEPT = {
     A.FDA,
     A.HistogramMatching,
     A.PixelDistributionAdaptation,
     A.Lambda,
@@ -669,37 +669,35 @@
 def test_transform_pipeline_serialization(seed, image, mask):
     aug = A.Compose(
         [
             A.OneOrOther(
                 A.Compose(
                     [
                         A.Resize(1024, 1024),
-                        A.RandomSizedCrop(min_max_height=(256, 1024), height=512, width=512, p=1),
+                        A.RandomSizedCrop(min_max_height=(256, 1024), size=(512, 512), p=1),
                         A.OneOf(
                             [
                                 A.RandomSizedCrop(
                                     min_max_height=(256, 512),
-                                    height=384,
-                                    width=384,
+                                    size= (384, 384),
                                     p=0.5,
                                 ),
                                 A.RandomSizedCrop(
                                     min_max_height=(256, 512),
-                                    height=512,
-                                    width=512,
+                                    size=(512, 512),
                                     p=0.5,
                                 ),
                             ]
                         ),
                     ]
                 ),
                 A.Compose(
                     [
                         A.Resize(1024, 1024),
-                        A.RandomSizedCrop(min_max_height=(256, 1025), height=256, width=256, p=1),
+                        A.RandomSizedCrop(min_max_height=(256, 1025), size=(256, 256), p=1),
                         A.OneOf([A.HueSaturationValue(p=0.5), A.RGBShift(p=0.7)], p=1),
                     ]
                 ),
             ),
             A.SomeOf(
                 [
                     A.HorizontalFlip(p=1),
@@ -844,14 +842,15 @@
 
     serialized_aug = A.to_dict(aug)
     deserialized_aug = A.from_dict(serialized_aug)
     set_seed(seed)
     aug_data = aug(image=image, image2=image2)
     set_seed(seed)
     deserialized_aug_data = deserialized_aug(image=image, image2=image2)
+
     assert np.array_equal(aug_data["image"], deserialized_aug_data["image"])
     assert np.array_equal(aug_data["image2"], deserialized_aug_data["image2"])
 
 
 @pytest.mark.parametrize("seed", TEST_SEEDS)
 @pytest.mark.parametrize("p", [1])
 def test_lambda_serialization(image, mask, albumentations_bboxes, keypoints, seed, p):
@@ -1016,16 +1015,16 @@
 
 
 @pytest.mark.parametrize( ["augmentation_cls", "params"], get_transforms(custom_arguments={
             A.Crop: {"y_min": 0, "y_max": 10, "x_min": 0, "x_max": 10},
             A.CenterCrop: {"height": 10, "width": 10},
             A.CropNonEmptyMaskIfExists: {"height": 10, "width": 10},
             A.RandomCrop: {"height": 10, "width": 10},
-            A.RandomResizedCrop: {"height": 10, "width": 10},
-            A.RandomSizedCrop: {"min_max_height": (4, 8), "height": 10, "width": 10},
+            A.RandomResizedCrop: {"size": (10, 10)},
+            A.RandomSizedCrop: {"min_max_height": (4, 8), "size" : (10, 10)},
             A.CropAndPad: {"px": 10},
             A.Resize: {"height": 10, "width": 10},
             A.XYMasking: {
                 "num_masks_x": (1, 3),
                 "num_masks_y": 3,
                 "mask_x_length": (10, 20),
                 "mask_y_length": 10,
@@ -1048,16 +1047,40 @@
             A.TemplateTransform,
             A.MixUp,
             A.ShiftScaleRotate,
         }) )
 def test_augmentations_serialization(augmentation_cls, params):
     instance = augmentation_cls(**params)
 
-    # Retrieve the constructor's parameters, except 'self', "always_apply"\
-    init_params = inspect.signature(augmentation_cls.__init__).parameters
-    expected_args = set(init_params.keys()) - {'self', "always_apply"}
+    def get_all_init_schema_fields(model_cls):
+        """
+        Recursively collects fields from InitSchema classes defined in the given augmentation class
+        and its base classes.
+
+        Args:
+            model_cls (Type): The augmentation class possibly containing an InitSchema class.
+
+        Returns:
+            Set[str]: A set of field names collected from all InitSchema classes.
+        """
+        fields = set()
+        if hasattr(model_cls, 'InitSchema'):
+            fields |= set(model_cls.InitSchema.model_fields.keys())
+
+        for base in model_cls.__bases__:
+            fields |= get_all_init_schema_fields(base)
+
+        return fields
+
+    model_fields = get_all_init_schema_fields(augmentation_cls)
+
+    # Note: You might want to adjust this based on how you handle default fields in your models
+    expected_args = model_fields - {'__class_fullname__'}
+
+    achieved_args = set(instance.to_dict()["transform"].keys())
 
-    # Retrieve the arguments reported by the instance's get_transform_init_args_names
-    reported_args = set(instance.to_dict()["transform"].keys()) - {'__class_fullname__', "always_apply"}
+    # Retrieve the arguments reported by the instance's to_dict method
+    # Adjust this logic based on how your serialization excludes or includes certain fields
+    reported_args = achieved_args - {'__class_fullname__'}
 
     # Check if the reported arguments match the expected arguments
     assert expected_args == reported_args, f"Mismatch in {augmentation_cls.__name__}: Expected {expected_args}, got {reported_args}"
```

### Comparing `albumentations-1.4.3/tests/test_targets.py` & `albumentations-1.4.4/tests/test_targets.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
     A.CropNonEmptyMaskIfExists: (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS),
     A.XYMasking: (Targets.IMAGE, Targets.MASK, Targets.KEYPOINTS),
     A.RandomCropNearBBox: (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS),
     A.Perspective: (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS),
     A.RandomSizedBBoxSafeCrop: (Targets.IMAGE, Targets.MASK, Targets.BBOXES),
     A.MixUp: (Targets.IMAGE, Targets.MASK, Targets.GLOBAL_LABEL),
     A.Lambda: (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS, Targets.GLOBAL_LABEL),
+    A.D4: (Targets.IMAGE, Targets.MASK, Targets.BBOXES, Targets.KEYPOINTS),
 }
 
 str2target = {
     'image': Targets.IMAGE, 'mask': Targets.MASK, 'bboxes': Targets.BBOXES, 'keypoints': Targets.KEYPOINTS, 'global_label': Targets.GLOBAL_LABEL
 }
 
 @pytest.mark.parametrize(
```

### Comparing `albumentations-1.4.3/tests/test_transforms.py` & `albumentations-1.4.4/tests/test_transforms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import random
 from functools import partial
+from typing import Optional, Tuple, Type
 
 import cv2
 import numpy as np
+
 import pytest
 import warnings
 from torchvision import transforms as torch_transforms
 
 import albumentations as A
 import albumentations.augmentations.functional as F
 import albumentations.augmentations.geometric.functional as FGeometric
@@ -44,32 +46,14 @@
     aug_img = aug(image=image)["image"]
     expected_size = int(np.round(100 / np.sqrt(2)))
     assert aug_img.shape[0] == expected_size
     assert (aug_img == border_value).sum() == 0
 
 
 @pytest.mark.parametrize("interpolation", [cv2.INTER_NEAREST, cv2.INTER_LINEAR, cv2.INTER_CUBIC])
-def test_shift_scale_rotate_interpolation(interpolation):
-    image = np.random.randint(low=0, high=256, size=(100, 100, 3), dtype=np.uint8)
-    mask = np.random.randint(low=0, high=2, size=(100, 100), dtype=np.uint8)
-    aug = A.ShiftScaleRotate(
-        shift_limit=(0.2, 0.2), scale_limit=(1.1, 1.1), rotate_limit=(45, 45), interpolation=interpolation, p=1
-    )
-    data = aug(image=image, mask=mask)
-    expected_image = FGeometric.shift_scale_rotate(
-        image, angle=45, scale=2.1, dx=0.2, dy=0.2, interpolation=interpolation, border_mode=cv2.BORDER_REFLECT_101
-    )
-    expected_mask = FGeometric.shift_scale_rotate(
-        mask, angle=45, scale=2.1, dx=0.2, dy=0.2, interpolation=cv2.INTER_NEAREST, border_mode=cv2.BORDER_REFLECT_101
-    )
-    assert np.array_equal(data["image"], expected_image)
-    assert np.array_equal(data["mask"], expected_mask)
-
-
-@pytest.mark.parametrize("interpolation", [cv2.INTER_NEAREST, cv2.INTER_LINEAR, cv2.INTER_CUBIC])
 def test_optical_distortion_interpolation(interpolation):
     image = np.random.randint(low=0, high=256, size=(100, 100, 3), dtype=np.uint8)
     mask = np.random.randint(low=0, high=2, size=(100, 100), dtype=np.uint8)
     aug = A.OpticalDistortion(distort_limit=(0.05, 0.05), shift_limit=(0, 0), interpolation=interpolation, p=1)
     data = aug(image=image, mask=mask)
     expected_image = FGeometric.optical_distortion(
         image, k=0.05, dx=0, dy=0, interpolation=interpolation, border_mode=cv2.BORDER_REFLECT_101
@@ -158,14 +142,15 @@
                 "num_masks_x": (1, 3),
                 "num_masks_y": (1, 3),
                 "mask_x_length": 10,
                 "mask_y_length": 10,
                 "mask_fill_value": 1,
                 "fill_value": 0,
             },
+            A.D4: {},
         },
         except_augmentations={A.RandomCropNearBBox, A.RandomSizedBBoxSafeCrop, A.BBoxSafeRandomCrop, A.PixelDropout,
                               A.MixUp},
     ),
 )
 def test_binary_mask_interpolation(augmentation_cls, params):
     """Checks whether transformations based on DualTransform does not introduce a mask interpolation artifacts"""
@@ -324,14 +309,23 @@
         image1 = np.random.randint(low=0, high=256, size=(100, 100, 3), dtype=np.uint8)
         image2 = image1.copy()
         res = aug(image=image1, image2=image2)
         aug1 = res["image"]
         aug2 = res["image2"]
         assert np.array_equal(aug1, aug2)
 
+    aug = A.Compose([augmentation_cls(always_apply=True, **params)])
+    aug.add_targets(additional_targets={"image2": "image"})
+    for _i in range(10):
+        image1 = np.random.randint(low=0, high=256, size=(100, 100, 3), dtype=np.uint8)
+        image2 = image1.copy()
+        res = aug(image=image1, image2=image2)
+        aug1 = res["image"]
+        aug2 = res["image2"]
+        assert np.array_equal(aug1, aug2)
 
 def test_image_invert():
     for _ in range(10):
         # test for np.uint8 dtype
         image1 = np.random.randint(low=0, high=256, size=(100, 100, 3), dtype=np.uint8)
         image2 = A.to_float(image1)
         r_int = F.invert(F.invert(image1))
@@ -542,15 +536,15 @@
         np.random.random([256, 320]).astype(np.float32),
         np.random.randint(0, 256, [256, 320, 1], np.uint8),
         np.random.random([256, 320, 1]).astype(np.float32),
     ],
 )
 def test_multiplicative_noise_grayscale(image):
     m = 0.5
-    aug = A.MultiplicativeNoise(m, p=1)
+    aug = A.MultiplicativeNoise((m, m), p=1)
     result = aug(image=image)["image"]
     image = F.clip(image * m, image.dtype, F.MAX_VALUES_BY_DTYPE[image.dtype])
     assert np.allclose(image, result)
 
     aug = A.MultiplicativeNoise(elementwise=True, p=1)
     params = aug.get_params_dependent_on_targets({"image": image})
     mul = params["multiplier"]
@@ -565,15 +559,15 @@
 @pytest.mark.parametrize(
     "image", [np.random.randint(0, 256, [256, 320, 3], np.uint8), np.random.random([256, 320, 3]).astype(np.float32)]
 )
 def test_multiplicative_noise_rgb(image):
     dtype = image.dtype
 
     m = 0.5
-    aug = A.MultiplicativeNoise(m, p=1)
+    aug = A.MultiplicativeNoise((m, m), p=1)
     result = aug(image=image)["image"]
     image = F.clip(image * m, dtype, F.MAX_VALUES_BY_DTYPE[dtype])
     assert np.allclose(image, result)
 
     aug = A.MultiplicativeNoise(elementwise=True, p=1)
     params = aug.get_params_dependent_on_targets({"image": image})
     mul = params["multiplier"]
@@ -656,15 +650,15 @@
 
 @pytest.mark.parametrize(
     ["ratio", "holes_number_x", "holes_number_y", "unit_size_min", "unit_size_max", "shift_x", "shift_y"],
     [
         (0.00001, 10, 10, 100, 100, 50, 50),
         (0.9, 100, None, 200, None, 0, 0),
         (0.4556, 10, 20, None, 200, 0, 0),
-        (0.00004, None, None, 2, 100, None, None),
+        (0.00004, None, None, 2, 100, 0, 0),
     ],
 )
 def test_grid_dropout_params(ratio, holes_number_x, holes_number_y, unit_size_min, unit_size_max, shift_x, shift_y):
     img = np.random.randint(0, 256, [256, 320], np.uint8)
 
     aug = A.GridDropout(
         ratio=ratio,
@@ -698,21 +692,14 @@
     if unit_size_min and unit_size_max:
         assert max(1, unit_size_min * ratio) <= (holes[0][2] - holes[0][0]) <= min(max(1, unit_size_max * ratio), 256)
     elif holes_number_x and holes_number_y:
         assert (holes[0][2] - holes[0][0]) == max(1, int(ratio * 320 // holes_number_x))
         assert (holes[0][3] - holes[0][1]) == max(1, int(ratio * 256 // holes_number_y))
 
 
-def test_gauss_noise_incorrect_var_limit_type():
-    with pytest.raises(TypeError) as exc_info:
-        A.GaussNoise(var_limit={"low": 70, "high": 90})
-    message = "Expected var_limit type to be one of (int, float, tuple, list), got <class 'dict'>"
-    assert str(exc_info.value) == message
-
-
 @pytest.mark.parametrize(
     ["blur_limit", "sigma", "result_blur", "result_sigma"],
     [
         [[0, 0], [1, 1], 0, 1],
         [[1, 1], [0, 0], 1, 0],
         [[1, 1], [1, 1], 1, 1],
         [[0, 0], [0, 0], 3, 0],
@@ -854,27 +841,14 @@
             res1 = t1(image=img)["image"]
             res2 = (t2(image=img.astype(np.float32) / 255.0)["image"] * 255).astype(np.uint8)
 
             _max = np.abs(res1.astype(np.int32) - res2).max()
             assert _max <= 10, f"Max value: {_max}"
 
 
-def test_shift_scale_separate_shift_x_shift_y(image, mask):
-    aug = A.ShiftScaleRotate(shift_limit=(0.3, 0.3), shift_limit_y=(0.4, 0.4), scale_limit=0, rotate_limit=0, p=1)
-    data = aug(image=image, mask=mask)
-    expected_image = FGeometric.shift_scale_rotate(
-        image, angle=0, scale=1, dx=0.3, dy=0.4, interpolation=cv2.INTER_LINEAR, border_mode=cv2.BORDER_REFLECT_101
-    )
-    expected_mask = FGeometric.shift_scale_rotate(
-        mask, angle=0, scale=1, dx=0.3, dy=0.4, interpolation=cv2.INTER_NEAREST, border_mode=cv2.BORDER_REFLECT_101
-    )
-    assert np.array_equal(data["image"], expected_image)
-    assert np.array_equal(data["mask"], expected_mask)
-
-
 @pytest.mark.parametrize(["val_uint8"], [[0], [1], [128], [255]])
 def test_glass_blur_float_uint8_diff_less_than_two(val_uint8):
     x_uint8 = np.zeros((5, 5)).astype(np.uint8)
     x_uint8[2, 2] = val_uint8
 
     x_float32 = np.zeros((5, 5)).astype(np.float32)
     x_float32[2, 2] = val_uint8 / 255.0
@@ -946,32 +920,32 @@
     assert result["image"].shape in [(250, 50), (500, 100)]
     assert result["keypoints"] in [[(45, 25, 0, 0)], [(90, 50, 0, 0)]]
 
 
 @pytest.mark.parametrize(
     ["img_weight", "template_weight", "template_transform", "image_size", "template_size"],
     [
-        (0.5, 0.5, A.RandomSizedCrop((50, 200), 513, 450, always_apply=True), (513, 450), (224, 224)),
-        (0.3, 0.5, A.RandomResizedCrop(513, 450, always_apply=True), (513, 450), (224, 224)),
+        (0.5, 0.5, A.RandomSizedCrop((50, 200), size=(513, 450), always_apply=True), (513, 450), (224, 224)),
+        (0.3, 0.5, A.RandomResizedCrop(size=(513, 450), always_apply=True), (513, 450), (224, 224)),
         (1.0, 0.5, A.CenterCrop(500, 450, always_apply=True), (500, 450, 3), (512, 512, 3)),
         (0.5, 0.8, A.Resize(513, 450, always_apply=True), (513, 450), (512, 512)),
         (0.5, 0.2, A.NoOp(), (224, 224), (224, 224)),
         (0.5, 0.9, A.NoOp(), (512, 512, 3), (512, 512, 3)),
         (0.5, 0.5, None, (512, 512), (512, 512)),
         (0.8, 0.7, None, (512, 512, 3), (512, 512, 3)),
         (
             0.5,
             0.5,
-            A.Compose([A.Blur(), A.RandomSizedCrop((50, 200), 512, 512, always_apply=True), A.HorizontalFlip()]),
+            A.Compose([A.Blur(always_apply=True), A.RandomSizedCrop((50, 200), size=(512, 512), always_apply=True), A.HorizontalFlip(always_apply=True)]),
             (512, 512),
             (512, 512),
         ),
     ],
 )
-def test_template_transform(image, img_weight, template_weight, template_transform, image_size, template_size):
+def test_template_transform(img_weight, template_weight, template_transform, image_size, template_size):
     img = np.random.randint(0, 256, image_size, np.uint8)
     template = np.random.randint(0, 256, template_size, np.uint8)
 
     aug = A.TemplateTransform(template, img_weight, template_weight, template_transform)
     result = aug(image=img)["image"]
 
     assert result.shape == img.shape
@@ -1306,60 +1280,14 @@
 
     with pytest.raises(ValueError) as exc_info:
         augmentation(image=img, force_apply=True)
 
     message = "This transformation expects 3-channel images"
     assert str(exc_info.value).startswith(message)
 
-
-def test_spatter_incorrect_mode(image):
-    unsupported_mode = "unsupported"
-    with pytest.raises(ValueError) as exc_info:
-        A.Spatter(mode=unsupported_mode)
-
-    message = f"Unsupported color mode: {unsupported_mode}. Transform supports only `rain` and `mud` mods."
-    assert str(exc_info.value).startswith(message)
-
-
-def test_chromatic_aberration_incorrect_mode(image):
-    unsupported_mode = "unsupported"
-    with pytest.raises(ValueError) as exc_info:
-        A.ChromaticAberration(mode=unsupported_mode)
-
-    message = f"Unsupported mode: {unsupported_mode}. Supported modes are 'green_purple', 'red_blue', 'random'."
-    assert str(exc_info.value).startswith(message)
-
-
-@pytest.mark.parametrize(
-    "unsupported_color,mode,message",
-    [
-        ([255, 255], "rain", "Unsupported color: [255, 255]. Color should be presented in RGB format."),
-        (
-            {"rain": [255, 255, 255]},
-            "mud",
-            "Wrong color definition: {'rain': [255, 255, 255]}. Color for mode: mud not specified.",
-        ),
-        (
-            {"rain": [255, 255]},
-            "rain",
-            "Unsupported color: [255, 255] for mode rain. Color should be presented in RGB format.",
-        ),
-        (
-            [255, 255, 255],
-            ["rain", "mud"],
-            "Unsupported color: [255, 255, 255]. Please specify color for each mode (use dict for it).",
-        ),
-    ],
-)
-def test_spatter_incorrect_color(unsupported_color, mode, message):
-    with pytest.raises(ValueError) as exc_info:
-        A.Spatter(mode=mode, color=unsupported_color)
-
-    assert str(exc_info.value).startswith(message)
-
 @pytest.mark.parametrize("height, width", [(100, 200), (200, 100)])
 @pytest.mark.parametrize("scale", [(0.08, 1.0), (0.5, 1.0)])
 @pytest.mark.parametrize("ratio", [(0.75, 1.33), (1.0, 1.0)])
 def test_random_crop_interfaces_vs_torchvision(height, width, scale, ratio):
     # NOTE: below will fail when height, width is no longer expected as first two positional arguments
     transform_albu = A.RandomResizedCrop(height, width, scale=scale, ratio=ratio, p=1)
     transform_albu_new = A.RandomResizedCrop(size=(height, width), scale=scale, ratio=ratio, p=1)
@@ -1394,23 +1322,78 @@
     transform_albu_height_is_size = transform_albu_new(image=image)['image']
     assert transformed_image_albu.shape == transformed_image_pt_np.shape
     assert transform_albu_height_is_size.shape == transformed_image_pt_np.shape
 
 @pytest.mark.parametrize("size, width, height, expected_warning", [
     ((100, 200), None, None, None),
     (None, 200, 100, DeprecationWarning),
-    (100, None, None, ValueError),
+    (100, None, None, TypeError),
 ])
 def test_deprecation_warnings(size, width, height, expected_warning):
     with warnings.catch_warnings(record=True) as w:
         warnings.simplefilter("always")
-        if expected_warning == ValueError:
-            with pytest.raises(ValueError):
+        if expected_warning == TypeError:
+            with pytest.raises(TypeError):
                 A.RandomResizedCrop(size=size, width=width, height=height)
         else:
             A.RandomResizedCrop(size=size, width=width, height=height)
         if expected_warning is DeprecationWarning:
             assert len(w) == 1
             assert issubclass(w[-1].category, expected_warning)
         else:
             assert not w
     warnings.resetwarnings()
+
+
+@pytest.mark.parametrize("num_shadows_limit, num_shadows_lower, num_shadows_upper, expected_warning", [
+    ((1, 2), None, None, None),
+    ((2, 3), None, None, None),
+    ((1, 2), 1, None, DeprecationWarning),
+    ((1, 2), None, 2, DeprecationWarning),
+    ((1, 2), 1, 2, DeprecationWarning),
+    ((2, 1), None, None, ValueError),
+])
+def test_deprecation_warnings_random_shadow(
+    num_shadows_limit: Tuple[int, int],
+    num_shadows_lower: Optional[int],
+    num_shadows_upper: Optional[int],
+    expected_warning: Optional[Type[Warning]],
+) -> None:
+    """
+    Test deprecation warnings for RandomShadow
+    """
+    with warnings.catch_warnings(record=True) as w:
+        warnings.simplefilter("always")
+        if expected_warning == ValueError:
+            with pytest.raises(ValueError):
+                A.RandomShadow(num_shadows_limit=num_shadows_limit, num_shadows_lower=num_shadows_lower,
+                               num_shadows_upper=num_shadows_upper, p=1)
+        else:
+            A.RandomShadow(num_shadows_limit=num_shadows_limit, num_shadows_lower=num_shadows_lower,
+                           num_shadows_upper=num_shadows_upper, p=1)
+        if expected_warning is DeprecationWarning:
+            assert len(w) == 1
+            assert issubclass(w[-1].category, expected_warning)
+        else:
+            assert not w
+    warnings.resetwarnings()
+
+
+@pytest.mark.parametrize("grid", [
+    (2, 2), (3, 3), (4, 4), (5, 7)
+])
+def test_grid_shuffle(image, mask, grid):
+    set_seed(4)
+    aug = A.Compose([A.RandomGridShuffle(grid=grid, p=1)])
+
+    res = aug(image=image, mask=mask)
+    assert res["image"].shape == image.shape
+    assert res["mask"].shape == mask.shape
+
+    assert not np.array_equal(res["image"], image)
+    assert not np.array_equal(res["mask"], mask)
+
+    assert np.array_equal(res["image"].mean(axis=(0, 1)), image.mean(axis=(0, 1)))
+    assert np.array_equal(res["image"].sum(axis=(0, 1)), image.sum(axis=(0, 1)))
+
+    assert np.array_equal(res["mask"].mean(axis=(0, 1)), mask.mean(axis=(0, 1)))
+    assert np.array_equal(res["mask"].sum(axis=(0, 1)), mask.sum(axis=(0, 1)))
```

