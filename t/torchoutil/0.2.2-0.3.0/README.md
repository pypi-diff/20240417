# Comparing `tmp/torchoutil-0.2.2.tar.gz` & `tmp/torchoutil-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchoutil-0.2.2.tar", last modified: Fri Mar  8 10:25:34 2024, max compression
+gzip compressed data, was "torchoutil-0.3.0.tar", last modified: Wed Apr 17 14:13:33 2024, max compression
```

## Comparing `torchoutil-0.2.2.tar` & `torchoutil-0.3.0.tar`

### file list

```diff
@@ -1,84 +1,89 @@
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-03-08 10:25:34.177938 torchoutil-0.2.2/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1064 2024-03-01 09:46:35.000000 torchoutil-0.2.2/LICENSE
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5988 2024-03-08 10:25:34.173938 torchoutil-0.2.2/PKG-INFO
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3412 2024-03-07 15:01:16.000000 torchoutil-0.2.2/README.md
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1959 2024-03-07 15:01:16.000000 torchoutil-0.2.2/pyproject.toml
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      108 2024-03-07 15:01:16.000000 torchoutil-0.2.2/requirements-dev.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       53 2024-03-04 17:33:08.000000 torchoutil-0.2.2/requirements-extras.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       57 2024-03-04 17:33:08.000000 torchoutil-0.2.2/requirements.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       38 2024-03-08 10:25:34.177938 torchoutil-0.2.2/setup.cfg
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      117 2024-03-04 17:33:08.000000 torchoutil-0.2.2/setup.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-03-08 10:25:34.165938 torchoutil-0.2.2/src/
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-03-08 10:25:34.169938 torchoutil-0.2.2/src/torchoutil/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      376 2024-03-08 10:17:47.000000 torchoutil-0.2.2/src/torchoutil/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      137 2024-03-04 17:33:08.000000 torchoutil-0.2.2/src/torchoutil/__main__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1032 2024-03-04 17:33:08.000000 torchoutil-0.2.2/src/torchoutil/info.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-03-08 10:25:34.169938 torchoutil-0.2.2/src/torchoutil/nn/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       70 2024-03-01 09:46:35.000000 torchoutil-0.2.2/src/torchoutil/nn/__init__.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-03-08 10:25:34.169938 torchoutil-0.2.2/src/torchoutil/nn/functional/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      292 2024-03-04 17:33:08.000000 torchoutil-0.2.2/src/torchoutil/nn/functional/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      404 2024-03-04 17:33:08.000000 torchoutil-0.2.2/src/torchoutil/nn/functional/activation.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2566 2024-03-04 17:33:08.000000 torchoutil-0.2.2/src/torchoutil/nn/functional/crop.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      460 2024-03-04 17:33:08.000000 torchoutil-0.2.2/src/torchoutil/nn/functional/get.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4475 2024-03-08 10:17:47.000000 torchoutil-0.2.2/src/torchoutil/nn/functional/indices.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    12716 2024-03-04 17:33:08.000000 torchoutil-0.2.2/src/torchoutil/nn/functional/mask.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4311 2024-03-08 10:17:47.000000 torchoutil-0.2.2/src/torchoutil/nn/functional/multiclass.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6945 2024-03-08 10:17:47.000000 torchoutil-0.2.2/src/torchoutil/nn/functional/multilabel.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      816 2024-03-04 17:33:08.000000 torchoutil-0.2.2/src/torchoutil/nn/functional/numpy.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3597 2024-03-07 10:19:13.000000 torchoutil-0.2.2/src/torchoutil/nn/functional/others.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     8389 2024-03-08 10:19:22.000000 torchoutil-0.2.2/src/torchoutil/nn/functional/pad.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1108 2024-03-04 17:33:08.000000 torchoutil-0.2.2/src/torchoutil/nn/functional/repeat.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-03-08 10:25:34.173938 torchoutil-0.2.2/src/torchoutil/nn/modules/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      270 2024-03-04 17:33:08.000000 torchoutil-0.2.2/src/torchoutil/nn/modules/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      700 2024-03-04 17:33:08.000000 torchoutil-0.2.2/src/torchoutil/nn/modules/activation.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1871 2024-03-04 17:33:08.000000 torchoutil-0.2.2/src/torchoutil/nn/modules/crop.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1184 2024-03-08 10:17:47.000000 torchoutil-0.2.2/src/torchoutil/nn/modules/mask.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4670 2024-03-08 10:17:47.000000 torchoutil-0.2.2/src/torchoutil/nn/modules/multiclass.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5188 2024-03-08 10:17:47.000000 torchoutil-0.2.2/src/torchoutil/nn/modules/multilabel.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      988 2024-03-04 17:33:08.000000 torchoutil-0.2.2/src/torchoutil/nn/modules/numpy.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3205 2024-03-04 17:33:08.000000 torchoutil-0.2.2/src/torchoutil/nn/modules/pad.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1259 2024-03-01 09:46:35.000000 torchoutil-0.2.2/src/torchoutil/nn/modules/repeat.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9607 2024-03-04 17:33:08.000000 torchoutil-0.2.2/src/torchoutil/nn/modules/tensor.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5825 2024-03-08 10:17:47.000000 torchoutil-0.2.2/src/torchoutil/nn/modules/typed.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-03-08 10:25:34.173938 torchoutil-0.2.2/src/torchoutil/optim/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       46 2024-03-04 17:33:08.000000 torchoutil-0.2.2/src/torchoutil/optim/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      638 2024-03-04 17:33:08.000000 torchoutil-0.2.2/src/torchoutil/optim/utils.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-03-08 10:25:34.173938 torchoutil-0.2.2/src/torchoutil/utils/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       46 2024-03-01 09:46:35.000000 torchoutil-0.2.2/src/torchoutil/utils/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5444 2024-03-08 10:19:47.000000 torchoutil-0.2.2/src/torchoutil/utils/ckpt.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4586 2024-03-07 15:01:16.000000 torchoutil-0.2.2/src/torchoutil/utils/collections.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-03-08 10:25:34.173938 torchoutil-0.2.2/src/torchoutil/utils/data/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       46 2024-03-01 09:46:35.000000 torchoutil-0.2.2/src/torchoutil/utils/data/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2333 2024-03-07 15:01:16.000000 torchoutil-0.2.2/src/torchoutil/utils/data/collate.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      507 2024-03-04 17:33:08.000000 torchoutil-0.2.2/src/torchoutil/utils/data/dataloader.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1488 2024-03-07 15:01:16.000000 torchoutil-0.2.2/src/torchoutil/utils/data/dataset.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4099 2024-03-04 17:33:08.000000 torchoutil-0.2.2/src/torchoutil/utils/data/split.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-03-08 10:25:34.173938 torchoutil-0.2.2/src/torchoutil/utils/hdf/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      394 2024-03-04 17:33:08.000000 torchoutil-0.2.2/src/torchoutil/utils/hdf/__init__.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      593 2024-03-07 14:09:27.000000 torchoutil-0.2.2/src/torchoutil/utils/hdf/common.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    15013 2024-03-07 15:01:16.000000 torchoutil-0.2.2/src/torchoutil/utils/hdf/dataset.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    15927 2024-03-08 10:17:47.000000 torchoutil-0.2.2/src/torchoutil/utils/hdf/pack.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      624 2024-03-04 17:33:08.000000 torchoutil-0.2.2/src/torchoutil/utils/packaging.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      528 2024-03-04 17:33:08.000000 torchoutil-0.2.2/src/torchoutil/utils/return_types.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5299 2024-03-04 17:33:08.000000 torchoutil-0.2.2/src/torchoutil/utils/tensorboard.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1157 2024-03-07 15:01:16.000000 torchoutil-0.2.2/src/torchoutil/utils/type_checks.py
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-03-08 10:25:34.169938 torchoutil-0.2.2/src/torchoutil.egg-info/
--rw-r--r--   0 labbeti   (1000) labbeti   (1000)     5988 2024-03-08 10:25:34.000000 torchoutil-0.2.2/src/torchoutil.egg-info/PKG-INFO
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2326 2024-03-08 10:25:34.000000 torchoutil-0.2.2/src/torchoutil.egg-info/SOURCES.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        1 2024-03-08 10:25:34.000000 torchoutil-0.2.2/src/torchoutil.egg-info/dependency_links.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       71 2024-03-08 10:25:34.000000 torchoutil-0.2.2/src/torchoutil.egg-info/entry_points.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      160 2024-03-08 10:25:34.000000 torchoutil-0.2.2/src/torchoutil.egg-info/requires.txt
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       11 2024-03-08 10:25:34.000000 torchoutil-0.2.2/src/torchoutil.egg-info/top_level.txt
-drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-03-08 10:25:34.173938 torchoutil-0.2.2/tests/
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      472 2024-03-04 17:33:08.000000 torchoutil-0.2.2/tests/test_nn_functional_crop.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      620 2024-03-07 15:01:16.000000 torchoutil-0.2.2/tests/test_nn_functional_indices.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    10920 2024-03-07 12:43:25.000000 torchoutil-0.2.2/tests/test_nn_functional_mask.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3836 2024-03-07 15:01:16.000000 torchoutil-0.2.2/tests/test_nn_functional_multilabel.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1032 2024-03-01 09:46:35.000000 torchoutil-0.2.2/tests/test_nn_functional_others.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7010 2024-03-07 12:42:21.000000 torchoutil-0.2.2/tests/test_nn_functional_pad.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      577 2024-03-01 09:46:35.000000 torchoutil-0.2.2/tests/test_nn_functional_repeat.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1238 2024-03-01 09:46:35.000000 torchoutil-0.2.2/tests/test_nn_modules_multilabel.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2239 2024-03-01 09:46:35.000000 torchoutil-0.2.2/tests/test_readme.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1131 2024-03-08 10:17:47.000000 torchoutil-0.2.2/tests/test_utils_ckpt.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1424 2024-03-07 15:01:16.000000 torchoutil-0.2.2/tests/test_utils_collections.py
--rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1967 2024-03-07 15:01:16.000000 torchoutil-0.2.2/tests/test_utils_hdf.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-17 14:13:33.942098 torchoutil-0.3.0/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1064 2024-03-01 09:46:35.000000 torchoutil-0.3.0/LICENSE
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6273 2024-04-17 14:13:33.942098 torchoutil-0.3.0/PKG-INFO
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3697 2024-04-17 14:04:29.000000 torchoutil-0.3.0/README.md
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1959 2024-03-07 15:01:16.000000 torchoutil-0.3.0/pyproject.toml
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      108 2024-03-07 15:01:16.000000 torchoutil-0.3.0/requirements-dev.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       53 2024-03-04 17:33:08.000000 torchoutil-0.3.0/requirements-extras.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       57 2024-03-04 17:33:08.000000 torchoutil-0.3.0/requirements.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       38 2024-04-17 14:13:33.942098 torchoutil-0.3.0/setup.cfg
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      117 2024-03-04 17:33:08.000000 torchoutil-0.3.0/setup.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-17 14:13:33.934098 torchoutil-0.3.0/src/
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-17 14:13:33.938099 torchoutil-0.3.0/src/torchoutil/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      376 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      137 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/__main__.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-17 14:13:33.938099 torchoutil-0.3.0/src/torchoutil/hub/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       96 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/hub/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      996 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/hub/download.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6856 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/hub/registry.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1032 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/info.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-17 14:13:33.938099 torchoutil-0.3.0/src/torchoutil/nn/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       70 2024-04-17 12:32:36.000000 torchoutil-0.3.0/src/torchoutil/nn/__init__.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-17 14:13:33.938099 torchoutil-0.3.0/src/torchoutil/nn/functional/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      292 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/nn/functional/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      404 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/nn/functional/activation.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2566 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/nn/functional/crop.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      460 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/nn/functional/get.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4475 2024-03-08 10:17:47.000000 torchoutil-0.3.0/src/torchoutil/nn/functional/indices.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    12723 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/nn/functional/mask.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4311 2024-03-08 10:17:47.000000 torchoutil-0.3.0/src/torchoutil/nn/functional/multiclass.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6945 2024-03-08 10:17:47.000000 torchoutil-0.3.0/src/torchoutil/nn/functional/multilabel.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      992 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/nn/functional/numpy.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4196 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/nn/functional/others.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     8421 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/nn/functional/pad.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1108 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/nn/functional/repeat.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-17 14:13:33.938099 torchoutil-0.3.0/src/torchoutil/nn/modules/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      270 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/nn/modules/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      700 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/nn/modules/activation.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1871 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/nn/modules/crop.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1643 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/nn/modules/layer.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1184 2024-03-08 10:17:47.000000 torchoutil-0.3.0/src/torchoutil/nn/modules/mask.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4703 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/nn/modules/multiclass.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5188 2024-03-08 10:17:47.000000 torchoutil-0.3.0/src/torchoutil/nn/modules/multilabel.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1005 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/nn/modules/numpy.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3311 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/nn/modules/pad.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1259 2024-03-01 09:46:35.000000 torchoutil-0.3.0/src/torchoutil/nn/modules/repeat.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     9618 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/nn/modules/tensor.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5825 2024-03-08 10:17:47.000000 torchoutil-0.3.0/src/torchoutil/nn/modules/typed.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-17 14:13:33.938099 torchoutil-0.3.0/src/torchoutil/optim/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       46 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/optim/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1761 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/optim/utils.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-17 14:13:33.938099 torchoutil-0.3.0/src/torchoutil/utils/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       46 2024-03-01 09:46:35.000000 torchoutil-0.3.0/src/torchoutil/utils/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     6934 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/utils/collections.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-17 14:13:33.942098 torchoutil-0.3.0/src/torchoutil/utils/data/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      141 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/utils/data/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2370 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/utils/data/collate.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      523 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/utils/data/dataloader.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1497 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/utils/data/dataset.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     4099 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/utils/data/split.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-17 14:13:33.942098 torchoutil-0.3.0/src/torchoutil/utils/hdf/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      394 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/utils/hdf/__init__.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      593 2024-03-07 14:09:27.000000 torchoutil-0.3.0/src/torchoutil/utils/hdf/common.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    16579 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/utils/hdf/dataset.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    16689 2024-04-17 14:04:29.000000 torchoutil-0.3.0/src/torchoutil/utils/hdf/pack.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      624 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/utils/packaging.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      528 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/utils/return_types.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     5299 2024-03-04 17:33:08.000000 torchoutil-0.3.0/src/torchoutil/utils/tensorboard.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1157 2024-03-07 15:01:16.000000 torchoutil-0.3.0/src/torchoutil/utils/type_checks.py
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-17 14:13:33.938099 torchoutil-0.3.0/src/torchoutil.egg-info/
+-rw-r--r--   0 labbeti   (1000) labbeti   (1000)     6273 2024-04-17 14:13:33.000000 torchoutil-0.3.0/src/torchoutil.egg-info/PKG-INFO
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2443 2024-04-17 14:13:33.000000 torchoutil-0.3.0/src/torchoutil.egg-info/SOURCES.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)        1 2024-04-17 14:13:33.000000 torchoutil-0.3.0/src/torchoutil.egg-info/dependency_links.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       71 2024-04-17 14:13:33.000000 torchoutil-0.3.0/src/torchoutil.egg-info/entry_points.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      160 2024-04-17 14:13:33.000000 torchoutil-0.3.0/src/torchoutil.egg-info/requires.txt
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)       11 2024-04-17 14:13:33.000000 torchoutil-0.3.0/src/torchoutil.egg-info/top_level.txt
+drwxrwxr-x   0 labbeti   (1000) labbeti   (1000)        0 2024-04-17 14:13:33.942098 torchoutil-0.3.0/tests/
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1172 2024-04-17 14:04:29.000000 torchoutil-0.3.0/tests/test_hub.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      472 2024-03-04 17:33:08.000000 torchoutil-0.3.0/tests/test_nn_functional_crop.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      620 2024-03-07 15:01:16.000000 torchoutil-0.3.0/tests/test_nn_functional_indices.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)    10920 2024-03-07 12:43:25.000000 torchoutil-0.3.0/tests/test_nn_functional_mask.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     3836 2024-03-07 15:01:16.000000 torchoutil-0.3.0/tests/test_nn_functional_multilabel.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1463 2024-04-17 14:04:29.000000 torchoutil-0.3.0/tests/test_nn_functional_others.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     7010 2024-03-07 12:42:21.000000 torchoutil-0.3.0/tests/test_nn_functional_pad.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)      577 2024-03-01 09:46:35.000000 torchoutil-0.3.0/tests/test_nn_functional_repeat.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1238 2024-03-01 09:46:35.000000 torchoutil-0.3.0/tests/test_nn_modules_multilabel.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2239 2024-03-01 09:46:35.000000 torchoutil-0.3.0/tests/test_readme.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1131 2024-04-17 14:04:20.000000 torchoutil-0.3.0/tests/test_utils_ckpt.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     2335 2024-04-17 14:04:29.000000 torchoutil-0.3.0/tests/test_utils_collections.py
+-rw-rw-r--   0 labbeti   (1000) labbeti   (1000)     1967 2024-03-07 15:01:16.000000 torchoutil-0.3.0/tests/test_utils_hdf.py
```

### Comparing `torchoutil-0.2.2/LICENSE` & `torchoutil-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torchoutil-0.2.2/PKG-INFO` & `torchoutil-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchoutil
-Version: 0.2.2
+Version: 0.3.0
 Summary: Collection of functions and modules to help development in PyTorch.
 Author-email: "Étienne Labbé (Labbeti)" <labbeti.pub@gmail.com>
 Maintainer-email: "Étienne Labbé (Labbeti)" <labbeti.pub@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Labbeti
         
@@ -75,15 +75,15 @@
 
 
 ## Installation
 ```bash
 pip install torchoutil
 ```
 
-The only requirement is **pytorch**.
+The only requirement is **PyTorch**.
 
 To check if the package is installed and show the package version, you can use the following command:
 ```bash
 torchoutil-info
 ```
 
 
@@ -101,15 +101,15 @@
 ```
 
 ```python
 import torch
 from torchoutil import lengths_to_non_pad_mask
 
 x = torch.as_tensor([3, 1, 2])
-pad_mask = lengths_to_non_pad_mask(x, max_len=4)
+mask = lengths_to_non_pad_mask(x, max_len=4)
 # Each row i contains x[i] True values for non-padding mask
 # tensor([[True, True, True, False],
 #         [True, False, False, False],
 #         [True, True, False, False]])
 ```
 
 ### Multilabel conversions
@@ -155,15 +155,15 @@
 # inv_perm are indices that allow us to get x3 from x2, i.e. x1 == x3 here
 ```
 
 ## Extras
 `torchoutil` also provides additional modules when some specific package are already installed in your environment.
 All extras can be installed with `pip install torchoutil[extras]`
 
-If `tensorboard` is installed, the function `load_event_file` can be used.
-If `numpy` is installed, the classes `FromNumpy` and  `ToNumpy` can be used and their related function.
-If `h5py` is installed, the function `pack_to_hdf` and class `HDFDataset` can be used.
+- If `tensorboard` is installed, the function `load_event_file` can be used. It is useful to load manually all data contained in an tensorboard event file.
+- If `numpy` is installed, the classes `FromNumpy` and  `ToNumpy` can be used and their related function. It is meant to be used to compose dynamic transforms into `Sequential` module.
+- If `h5py` is installed, the function `pack_to_hdf` and class `HDFDataset` can be used. Can be used to pack/read dataset to HDF files, and supports variable-length sequences of data.
 
 
 ## Contact
 Maintainer:
-- Étienne Labbé "Labbeti": labbeti.pub@gmail.com
+- [Étienne Labbé](https://labbeti.github.io/) "Labbeti": labbeti.pub@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchoutil Version: 0.2.2 Summary: Collection of
+Metadata-Version: 2.1 Name: torchoutil Version: 0.3.0 Summary: Collection of
 functions and modules to help development in PyTorch. Author-email: "Ãtienne
 LabbÃ© (Labbeti)"
 gmail.com> Maintainer-email: "Ãtienne LabbÃ© (Labbeti)"
 gmail.com> License: MIT License Copyright (c) 2024 Labbeti Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
@@ -30,21 +30,21 @@
 Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 extras Provides-Extra: dev License-File: LICENSE # torchoutil
 _[_P_y_t_h_o_n_]_[_P_y_T_o_r_c_h_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_B_u_i_l_d_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]Collection of
              functions and modules to help development in PyTorch.
 ## Installation ```bash pip install torchoutil ``` The only requirement is
-**pytorch**. To check if the package is installed and show the package version,
+**PyTorch**. To check if the package is installed and show the package version,
 you can use the following command: ```bash torchoutil-info ``` ## Usage ###
 Batch of padded sequences ```python import torch from torchoutil import
 masked_mean x = torch.as_tensor([1, 2, 3, 4]) mask = torch.as_tensor([True,
 True, False, False]) result = masked_mean(x, mask) # result contains the mean
 of the values marked as True: 1.5 ``` ```python import torch from torchoutil
-import lengths_to_non_pad_mask x = torch.as_tensor([3, 1, 2]) pad_mask =
+import lengths_to_non_pad_mask x = torch.as_tensor([3, 1, 2]) mask =
 lengths_to_non_pad_mask(x, max_len=4) # Each row i contains x[i] True values
 for non-padding mask # tensor([[True, True, True, False], # [True, False,
 False, False], # [True, True, False, False]]) ``` ### Multilabel conversions
 ```python import torch from torchoutil import probs_to_names probs =
 torch.as_tensor([[0.9, 0.1], [0.6, 0.9]]) names = probs_to_names(probs,
 threshold=0.5, idx_to_name={0: "Cat", 1: "Dog"}) # [["Cat"], ["Cat", "Dog"]]
 ``` ```python import torch from torchoutil import multihot_to_indices multihot
@@ -54,13 +54,16 @@
 x = torch.as_tensor([1, 2, 3, 4]) result = insert_at_indices(x, indices=[0, 2],
 values=5) # result contains tensor with inserted values: tensor([5, 1, 2, 5, 3,
 4]) ``` ```python import torch from torchoutil import get_inverse_perm perm =
 torch.randperm(10) inv_perm = get_inverse_perm(perm) x1 = torch.rand(10) x2 =
 x1[perm] x3 = x2[inv_perm] # inv_perm are indices that allow us to get x3 from
 x2, i.e. x1 == x3 here ``` ## Extras `torchoutil` also provides additional
 modules when some specific package are already installed in your environment.
-All extras can be installed with `pip install torchoutil[extras]` If
-`tensorboard` is installed, the function `load_event_file` can be used. If
+All extras can be installed with `pip install torchoutil[extras]` - If
+`tensorboard` is installed, the function `load_event_file` can be used. It is
+useful to load manually all data contained in an tensorboard event file. - If
 `numpy` is installed, the classes `FromNumpy` and `ToNumpy` can be used and
-their related function. If `h5py` is installed, the function `pack_to_hdf` and
-class `HDFDataset` can be used. ## Contact Maintainer: - Ãtienne LabbÃ©
-"Labbeti": labbeti.pub@gmail.com
+their related function. It is meant to be used to compose dynamic transforms
+into `Sequential` module. - If `h5py` is installed, the function `pack_to_hdf`
+and class `HDFDataset` can be used. Can be used to pack/read dataset to HDF
+files, and supports variable-length sequences of data. ## Contact Maintainer: -
+[Ãtienne LabbÃ©](https://labbeti.github.io/) "Labbeti": labbeti.pub@gmail.com
```

### Comparing `torchoutil-0.2.2/README.md` & `torchoutil-0.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 ## Installation
 ```bash
 pip install torchoutil
 ```
 
-The only requirement is **pytorch**.
+The only requirement is **PyTorch**.
 
 To check if the package is installed and show the package version, you can use the following command:
 ```bash
 torchoutil-info
 ```
 
 
@@ -50,15 +50,15 @@
 ```
 
 ```python
 import torch
 from torchoutil import lengths_to_non_pad_mask
 
 x = torch.as_tensor([3, 1, 2])
-pad_mask = lengths_to_non_pad_mask(x, max_len=4)
+mask = lengths_to_non_pad_mask(x, max_len=4)
 # Each row i contains x[i] True values for non-padding mask
 # tensor([[True, True, True, False],
 #         [True, False, False, False],
 #         [True, True, False, False]])
 ```
 
 ### Multilabel conversions
@@ -104,15 +104,15 @@
 # inv_perm are indices that allow us to get x3 from x2, i.e. x1 == x3 here
 ```
 
 ## Extras
 `torchoutil` also provides additional modules when some specific package are already installed in your environment.
 All extras can be installed with `pip install torchoutil[extras]`
 
-If `tensorboard` is installed, the function `load_event_file` can be used.
-If `numpy` is installed, the classes `FromNumpy` and  `ToNumpy` can be used and their related function.
-If `h5py` is installed, the function `pack_to_hdf` and class `HDFDataset` can be used.
+- If `tensorboard` is installed, the function `load_event_file` can be used. It is useful to load manually all data contained in an tensorboard event file.
+- If `numpy` is installed, the classes `FromNumpy` and  `ToNumpy` can be used and their related function. It is meant to be used to compose dynamic transforms into `Sequential` module.
+- If `h5py` is installed, the function `pack_to_hdf` and class `HDFDataset` can be used. Can be used to pack/read dataset to HDF files, and supports variable-length sequences of data.
 
 
 ## Contact
 Maintainer:
-- Étienne Labbé "Labbeti": labbeti.pub@gmail.com
+- [Étienne Labbé](https://labbeti.github.io/) "Labbeti": labbeti.pub@gmail.com
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
 # torchoutil
 _[_P_y_t_h_o_n_]_[_P_y_T_o_r_c_h_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_B_u_i_l_d_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]Collection of
              functions and modules to help development in PyTorch.
 ## Installation ```bash pip install torchoutil ``` The only requirement is
-**pytorch**. To check if the package is installed and show the package version,
+**PyTorch**. To check if the package is installed and show the package version,
 you can use the following command: ```bash torchoutil-info ``` ## Usage ###
 Batch of padded sequences ```python import torch from torchoutil import
 masked_mean x = torch.as_tensor([1, 2, 3, 4]) mask = torch.as_tensor([True,
 True, False, False]) result = masked_mean(x, mask) # result contains the mean
 of the values marked as True: 1.5 ``` ```python import torch from torchoutil
-import lengths_to_non_pad_mask x = torch.as_tensor([3, 1, 2]) pad_mask =
+import lengths_to_non_pad_mask x = torch.as_tensor([3, 1, 2]) mask =
 lengths_to_non_pad_mask(x, max_len=4) # Each row i contains x[i] True values
 for non-padding mask # tensor([[True, True, True, False], # [True, False,
 False, False], # [True, True, False, False]]) ``` ### Multilabel conversions
 ```python import torch from torchoutil import probs_to_names probs =
 torch.as_tensor([[0.9, 0.1], [0.6, 0.9]]) names = probs_to_names(probs,
 threshold=0.5, idx_to_name={0: "Cat", 1: "Dog"}) # [["Cat"], ["Cat", "Dog"]]
 ``` ```python import torch from torchoutil import multihot_to_indices multihot
@@ -22,13 +22,16 @@
 x = torch.as_tensor([1, 2, 3, 4]) result = insert_at_indices(x, indices=[0, 2],
 values=5) # result contains tensor with inserted values: tensor([5, 1, 2, 5, 3,
 4]) ``` ```python import torch from torchoutil import get_inverse_perm perm =
 torch.randperm(10) inv_perm = get_inverse_perm(perm) x1 = torch.rand(10) x2 =
 x1[perm] x3 = x2[inv_perm] # inv_perm are indices that allow us to get x3 from
 x2, i.e. x1 == x3 here ``` ## Extras `torchoutil` also provides additional
 modules when some specific package are already installed in your environment.
-All extras can be installed with `pip install torchoutil[extras]` If
-`tensorboard` is installed, the function `load_event_file` can be used. If
+All extras can be installed with `pip install torchoutil[extras]` - If
+`tensorboard` is installed, the function `load_event_file` can be used. It is
+useful to load manually all data contained in an tensorboard event file. - If
 `numpy` is installed, the classes `FromNumpy` and `ToNumpy` can be used and
-their related function. If `h5py` is installed, the function `pack_to_hdf` and
-class `HDFDataset` can be used. ## Contact Maintainer: - Ãtienne LabbÃ©
-"Labbeti": labbeti.pub@gmail.com
+their related function. It is meant to be used to compose dynamic transforms
+into `Sequential` module. - If `h5py` is installed, the function `pack_to_hdf`
+and class `HDFDataset` can be used. Can be used to pack/read dataset to HDF
+files, and supports variable-length sequences of data. ## Contact Maintainer: -
+[Ãtienne LabbÃ©](https://labbeti.github.io/) "Labbeti": labbeti.pub@gmail.com
```

### Comparing `torchoutil-0.2.2/pyproject.toml` & `torchoutil-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `torchoutil-0.2.2/src/torchoutil/info.py` & `torchoutil-0.3.0/src/torchoutil/info.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.2.2/src/torchoutil/nn/functional/crop.py` & `torchoutil-0.3.0/src/torchoutil/nn/functional/crop.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.2.2/src/torchoutil/nn/functional/indices.py` & `torchoutil-0.3.0/src/torchoutil/nn/functional/indices.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.2.2/src/torchoutil/nn/functional/mask.py` & `torchoutil-0.3.0/src/torchoutil/nn/functional/mask.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,14 +77,15 @@
     equal = mask.all().item()
     return equal
 
 
 def generate_square_subsequent_mask(
     size: int,
     diagonal: int = 0,
+    *,
     device: Union[str, torch.device, None] = None,
     dtype: Optional[torch.dtype] = None,
 ) -> Tensor:
     device = get_device(device)
     mask = torch.ones((size, size), device=device, dtype=torch.bool)
     mask = torch.tril(mask, diagonal=diagonal)
     mask = torch.where(mask, 0.0, -torch.inf)
```

### Comparing `torchoutil-0.2.2/src/torchoutil/nn/functional/multiclass.py` & `torchoutil-0.3.0/src/torchoutil/nn/functional/multiclass.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.2.2/src/torchoutil/nn/functional/multilabel.py` & `torchoutil-0.3.0/src/torchoutil/nn/functional/multilabel.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.2.2/src/torchoutil/nn/functional/numpy.py` & `torchoutil-0.3.0/src/torchoutil/nn/functional/numpy.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-from typing import Union
+from typing import Any, Union
 
 import torch
-
 from torch import Tensor
+from typing_extensions import TypeGuard
 
 from torchoutil.nn.functional.get import get_device
 from torchoutil.utils.packaging import _NUMPY_AVAILABLE
 
-
 if _NUMPY_AVAILABLE:
     import numpy as np
 
     def to_numpy(
         x: Union[Tensor, np.ndarray, list],
         dtype: Union[str, np.dtype, None] = None,
     ) -> np.ndarray:
@@ -26,7 +25,10 @@
     def from_numpy(
         x: np.ndarray,
         dtype: Union[torch.dtype, None] = None,
         device: Union[str, torch.device, None] = None,
     ) -> Tensor:
         device = get_device(device)
         return torch.from_numpy(x).to(dtype=dtype, device=device)
+
+    def is_numpy_scalar(x: Any) -> TypeGuard[np.generic]:
+        return np.isscalar(x) and x.__class__.__module__ != "__builtin__"
```

### Comparing `torchoutil-0.2.2/src/torchoutil/nn/functional/others.py` & `torchoutil-0.3.0/src/torchoutil/nn/functional/others.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,64 +19,69 @@
 
 import torch
 from torch import Tensor, nn
 from typing_extensions import TypeGuard
 
 from torchoutil.nn.functional.get import get_device
 
-
 T = TypeVar("T")
 U = TypeVar("U")
 
 
+def count_parameters(model: nn.Module, only_trainable: bool = False) -> int:
+    params = (p for p in model.parameters() if not only_trainable or p.requires_grad)
+    count = sum(p.numel() for p in params)
+    return count
+
+
 def find(
     x: Tensor,
     value: Any,
     default: Union[None, Tensor, int, float] = None,
     dim: int = -1,
 ) -> Tensor:
     """Return the index of the first occurrence of value in a tensor."""
     if x.ndim == 0:
         raise ValueError(
             f"Function find does not supports 0-d tensors. (found {x.ndim=} == 0)"
         )
     mask = x.eq(value)
-    contains_eos = mask.any(dim=dim)
-    indices_eos = mask.int().argmax(dim=dim)
+    contains = mask.any(dim=dim)
+    indices = mask.int().argmax(dim=dim)
 
     if default is None:
-        if not contains_eos.all():
+        if not contains.all():
             raise RuntimeError(f"Cannot find {value=} in tensor.")
-        return indices_eos
+        return indices
     else:
-        output = torch.where(contains_eos, indices_eos, default)
+        output = torch.where(contains, indices, default)
         return output
 
 
 @overload
 def move_to_rec(
     x: Mapping[T, U],
-    predicate: Optional[Callable[[Any], bool]] = None,
+    predicate: Optional[Callable[[Union[Tensor, nn.Module]], bool]] = None,
     **kwargs,
 ) -> Dict[T, U]:
     ...
 
 
 @overload
 def move_to_rec(
     x: T,
-    predicate: Optional[Callable[[Any], bool]] = None,
+    predicate: Optional[Callable[[Union[Tensor, nn.Module]], bool]] = None,
     **kwargs,
 ) -> T:
     ...
 
 
 def move_to_rec(
     x: Any,
-    predicate: Optional[Callable[[Any], bool]] = None,
+    predicate: Optional[Callable[[Union[Tensor, nn.Module]], bool]] = None,
     **kwargs,
 ) -> Any:
     """Move all modules and tensors recursively to a specific dtype or device."""
     if "device" in kwargs:
         kwargs["device"] = get_device(kwargs["device"])
 
     if isinstance(x, (Tensor, nn.Module)):
@@ -96,49 +101,62 @@
             return tuple(generator)
         else:
             return list(generator)
     else:
         return x
 
 
+def is_python_scalar(x: Any) -> TypeGuard[Union[int, float, bool, complex]]:
+    return isinstance(x, (int, float, bool, complex))
+
+
+def is_torch_scalar(x: Any) -> TypeGuard[Tensor]:
+    return isinstance(x, Tensor) and x.ndim == 0
+
+
 def is_scalar(x: Any) -> TypeGuard[Union[int, float, bool, complex, Tensor]]:
-    return isinstance(x, (int, float, bool, complex)) or (
-        isinstance(x, Tensor) and x.ndim == 0
-    )
+    return is_python_scalar(x) or is_torch_scalar(x)
 
 
 def can_be_stacked(
-    tensors: Union[List[Any], Tuple[Any, ...]]
+    tensors: Union[List[Any], Tuple[Any, ...]],
 ) -> TypeGuard[Union[List[Tensor], Tuple[Tensor, ...]]]:
     if len(tensors) == 0:
         return True
     if not all(isinstance(tensor, Tensor) for tensor in tensors):
         return False
     shape0 = tensors[0].shape
     result = all(tensor.shape == shape0 for tensor in tensors[1:])
     return result
 
 
 def can_be_converted_to_tensor(x: Any) -> bool:
-    if isinstance(x, (int, float, bool, complex)):
+    if isinstance(x, Tensor):
         return True
-    elif isinstance(x, (List, Tuple)):
-        return __can_be_converted_to_tensor_list_tuple(x)
     else:
-        return False
+        return __can_be_converted_to_tensor_nested(x)
 
 
 def __can_be_converted_to_tensor_list_tuple(x: Union[List, Tuple]) -> bool:
     if len(x) == 0:
         return True
 
-    valid_items = all(can_be_converted_to_tensor(xi) for xi in x)
+    valid_items = all(__can_be_converted_to_tensor_nested(xi) for xi in x)
     if not valid_items:
         return False
 
     if all(not isinstance(xi, Sized) for xi in x):
         return True
     elif all(isinstance(xi, Sized) for xi in x):
         len0 = len(x[0])
         return all(len(xi) == len0 for xi in x[1:])
     else:
         return False
+
+
+def __can_be_converted_to_tensor_nested(x: Any) -> bool:
+    if is_python_scalar(x):
+        return True
+    elif isinstance(x, (List, Tuple)):
+        return __can_be_converted_to_tensor_list_tuple(x)
+    else:
+        return False
```

### Comparing `torchoutil-0.2.2/src/torchoutil/nn/functional/pad.py` & `torchoutil-0.3.0/src/torchoutil/nn/functional/pad.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,16 +64,17 @@
     x = F.pad(x, pad_seq, mode=mode, value=pad_value)
     return x
 
 
 def pad_and_stack_rec(
     sequence: Union[Tensor, int, float, tuple, list],
     pad_value: Number,
-    dtype: Union[None, torch.dtype] = None,
+    *,
     device: Union[str, torch.device, None] = None,
+    dtype: Union[None, torch.dtype] = None,
 ) -> Tensor:
     """Recursive version of torch.nn.utils.rnn.pad_sequence, with padding of Tensors.
 
     Args:
         sequence: The sequence to pad. Must be convertable to tensor by having the correct number of dims in all sublists.
         pad_value: The pad value used.
         dtype: The dtype of the output Tensor. defaults to None.
@@ -98,15 +99,16 @@
         return sequence.to(dtype=dtype, device=device)
 
     elif is_scalar(sequence) or (isinstance(sequence, Sized) and len(sequence) == 0):
         return torch.as_tensor(sequence, dtype=dtype, device=device)  # type: ignore
 
     elif isinstance(sequence, (list, tuple)):
         sequence = [
-            pad_and_stack_rec(elt, pad_value, dtype, device) for elt in sequence
+            pad_and_stack_rec(elt, pad_value, dtype=dtype, device=device)
+            for elt in sequence
         ]
         if can_be_stacked(sequence):
             return torch.stack(sequence)
 
         shapes = [elt.shape for elt in sequence]
         shape0 = shapes[0]
```

### Comparing `torchoutil-0.2.2/src/torchoutil/nn/functional/repeat.py` & `torchoutil-0.3.0/src/torchoutil/nn/functional/repeat.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.2.2/src/torchoutil/nn/modules/activation.py` & `torchoutil-0.3.0/src/torchoutil/nn/modules/activation.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.2.2/src/torchoutil/nn/modules/crop.py` & `torchoutil-0.3.0/src/torchoutil/nn/modules/crop.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.2.2/src/torchoutil/nn/modules/mask.py` & `torchoutil-0.3.0/src/torchoutil/nn/modules/mask.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.2.2/src/torchoutil/nn/modules/multiclass.py` & `torchoutil-0.3.0/src/torchoutil/nn/modules/multiclass.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 T = TypeVar("T")
 
 
 class IndicesToOneHot(nn.Module):
     def __init__(
         self,
         num_classes: int,
+        *,
         device: Union[str, torch.device, None] = None,
         dtype: Union[torch.dtype, None] = torch.bool,
     ) -> None:
         super().__init__()
         self.num_classes = num_classes
         self.device = device
         self.dtype = dtype
@@ -117,14 +118,15 @@
         return indices
 
 
 class NamesToOneHot(nn.Module, Generic[T]):
     def __init__(
         self,
         idx_to_name: Mapping[int, T],
+        *,
         device: Union[str, torch.device, None] = None,
         dtype: Union[torch.dtype, None] = torch.bool,
     ) -> None:
         super().__init__()
         self.idx_to_name = idx_to_name
         self.device = device
         self.dtype = dtype
@@ -159,14 +161,15 @@
         indices = probs_to_indices(probs)
         return indices
 
 
 class ProbsToOneHot(nn.Module):
     def __init__(
         self,
+        *,
         device: Union[str, torch.device, None] = None,
         dtype: Union[torch.dtype, None] = torch.bool,
     ) -> None:
         super().__init__()
         self.device = device
         self.dtype = dtype
```

### Comparing `torchoutil-0.2.2/src/torchoutil/nn/modules/multilabel.py` & `torchoutil-0.3.0/src/torchoutil/nn/modules/multilabel.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.2.2/src/torchoutil/nn/modules/numpy.py` & `torchoutil-0.3.0/src/torchoutil/nn/modules/numpy.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 from typing import Union
 
 import torch
 from torch import Tensor, nn
 
 from torchoutil.utils.packaging import _NUMPY_AVAILABLE
 
-
 if _NUMPY_AVAILABLE:
     import numpy as np
 
-    from torchoutil.nn.functional.numpy import to_numpy, from_numpy
+    from torchoutil.nn.functional.numpy import from_numpy, to_numpy
 
     class ToNumpy(nn.Module):
-        def __init__(self, dtype: Union[str, np.dtype, None] = None) -> None:
+        def __init__(self, *, dtype: Union[str, np.dtype, None] = None) -> None:
             super().__init__()
             self.dtype = dtype
 
         def forward(self, x: Union[Tensor, np.ndarray, list]) -> np.ndarray:
             return to_numpy(x, self.dtype)
 
     class FromNumpy(nn.Module):
         def __init__(
             self,
-            dtype: Union[torch.dtype, None] = None,
+            *,
             device: Union[str, torch.device, None] = None,
+            dtype: Union[torch.dtype, None] = None,
         ) -> None:
             super().__init__()
             self.device = device
             self.dtype = dtype
 
         def forward(self, x: np.ndarray) -> Tensor:
             return from_numpy(x, self.dtype, self.device)
```

### Comparing `torchoutil-0.2.2/src/torchoutil/nn/modules/pad.py` & `torchoutil-0.3.0/src/torchoutil/nn/modules/pad.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-from typing import Iterable, Literal, Union
+from typing import Iterable, Union
 
 import torch
 from torch import Generator, Tensor, nn
+from torch.types import Number
 
-from torchoutil.nn.functional.pad import pad_and_stack_rec, pad_dim, pad_dims, PadAlign
+from torchoutil.nn.functional.pad import PadAlign, pad_and_stack_rec, pad_dim, pad_dims
 from torchoutil.utils.collections import dump_dict
 
 
 class PadDim(nn.Module):
     def __init__(
         self,
         target_length: int,
@@ -97,28 +98,34 @@
             )
         )
 
 
 class PadAndStackRec(nn.Module):
     def __init__(
         self,
-        pad_value: float,
-        dtype: Union[None, torch.dtype] = None,
+        pad_value: Number,
+        *,
         device: Union[str, torch.device, None] = None,
+        dtype: Union[None, torch.dtype] = None,
     ) -> None:
         super().__init__()
         self.pad_value = pad_value
-        self.dtype = dtype
         self.device = device
+        self.dtype = dtype
 
     def forward(
         self,
         sequence: Union[Tensor, int, float, tuple, list],
     ) -> Tensor:
-        return pad_and_stack_rec(sequence, self.pad_value, self.dtype, self.device)
+        return pad_and_stack_rec(
+            sequence,
+            self.pad_value,
+            dtype=self.dtype,
+            device=self.device,
+        )
 
     def extra_repr(self) -> str:
         return dump_dict(
             dict(
                 pad_value=self.pad_value,
                 dtype=self.dtype,
                 device=self.device,
```

### Comparing `torchoutil-0.2.2/src/torchoutil/nn/modules/repeat.py` & `torchoutil-0.3.0/src/torchoutil/nn/modules/repeat.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.2.2/src/torchoutil/nn/modules/tensor.py` & `torchoutil-0.3.0/src/torchoutil/nn/modules/tensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,14 +290,15 @@
     def forward(self, x: Tensor) -> Number:
         return x.item()
 
 
 class AsTensor(nn.Module):
     def __init__(
         self,
+        *,
         device: Union[str, torch.device, None] = None,
         dtype: Union[torch.dtype, None] = None,
     ) -> None:
         device = get_device(device)
         super().__init__()
         self.device = device
         self.dtype = dtype
```

### Comparing `torchoutil-0.2.2/src/torchoutil/nn/modules/typed.py` & `torchoutil-0.3.0/src/torchoutil/nn/modules/typed.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.2.2/src/torchoutil/utils/data/dataset.py` & `torchoutil-0.3.0/src/torchoutil/utils/data/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     def __len__(self) -> int:
         ...
 
 
 class TransformWrapper(Generic[T, U], Dataset[U]):
     def __init__(
         self,
-        dataset: Dataset[T],
+        dataset: SizedDatasetLike[T],
         transform: Optional[Callable[[T], U]],
     ) -> None:
         super().__init__()
         self._dataset = dataset
         self._transform = transform
 
     def __getitem__(self, index) -> Union[T, U]:
```

### Comparing `torchoutil-0.2.2/src/torchoutil/utils/data/split.py` & `torchoutil-0.3.0/src/torchoutil/utils/data/split.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.2.2/src/torchoutil/utils/hdf/common.py` & `torchoutil-0.3.0/src/torchoutil/utils/hdf/common.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.2.2/src/torchoutil/utils/hdf/dataset.py` & `torchoutil-0.3.0/src/torchoutil/utils/hdf/dataset.py`

 * *Files 22% similar despite different names*

```diff
@@ -73,43 +73,54 @@
     def __init__(
         self,
         hdf_fpath: Union[str, Path],
         transform: Optional[Callable[[T], U]] = None,
         keep_padding: Iterable[str] = (),
         return_added_columns: bool = False,
         open_hdf: bool = True,
+        auto_open: bool = False,
+        numpy_to_torch: bool = True,
+        file_kwargs: Optional[Dict[str, Any]] = None,
     ) -> None:
         """HDFDataset to read an packed hdf file.
 
         In HDF, all tensors are padded internally then cropped on-the-fly.
         Several options allows to extract non-padded tensors or return the internal shape of each column.
 
         Args:
             hdf_fpath: The path to the HDF file.
             transforms: The transform to apply values. default to None.
             keep_padding: Keys to keep padding values. defaults to ().
             return_added_columns: Returns the columns added by pack_to_hdf(.) function.
             open_hdf: If True, open the HDF file at start. defaults to True.
+            auto_open: If True, open HDF dataset only when __getitem__ or __len__ is called. defaults to False.
+            numpy_to_torch: If True, converts numpy array to PyTorch tensors. defaults to True.
+            file_kwargs: Options given to h5py file object. defaults to None.
         """
         hdf_fpath = Path(hdf_fpath).resolve()
         if not hdf_fpath.is_file():
             names = os.listdir(osp.dirname(hdf_fpath))
             names = [name for name in names if name.endswith(".hdf")]
             names = list(sorted(names))
             names_str = "\n - ".join(names)
             raise FileNotFoundError(
                 f"Cannot find HDF file in path {hdf_fpath=}. Possible HDF files are:\n - {names_str}"
             )
         keep_padding = list(keep_padding)
+        if file_kwargs is None:
+            file_kwargs = {}
 
         super().__init__()
         self._hdf_fpath = hdf_fpath
         self._transform = transform
         self._keep_padding = keep_padding
         self._return_added_columns = return_added_columns
+        self._auto_open = auto_open
+        self._numpy_to_torch = numpy_to_torch
+        self._file_kwargs = file_kwargs
 
         self._hdf_file: Any = None
 
         if open_hdf:
             self.open()
 
     # Properties
@@ -124,14 +135,18 @@
         return list(self.get_hdf_keys())
 
     @property
     def attrs(self) -> Dict[str, Any]:
         return dict(self._hdf_file.attrs)
 
     @property
+    def metadata(self) -> str:
+        return self.attrs.get("metadata", "")
+
+    @property
     def column_names(self) -> List[str]:
         """The name of each column of the dataset."""
         column_names = self.all_columns
         column_names = [
             name
             for name in column_names
             if self._return_added_columns or name not in self.added_columns
@@ -197,37 +212,38 @@
 
     def at(
         self,
         index: IndexType = None,
         column: ColumnType = None,
         raw: bool = False,
     ) -> Any:
-        if not self.is_open():
-            raise RuntimeError(
-                f"Cannot get_raw value with closed HDF file. ({self._hdf_file is not None=} and {bool(self._hdf_file)=})"
-            )
+        if self.is_closed():
+            if self._auto_open:
+                self.open()
+            else:
+                raise RuntimeError(
+                    f"Cannot get_raw value with closed HDF file. ({self._hdf_file is not None=} and {bool(self._hdf_file)=})"
+                )
 
         if index is None:
             index = slice(None)
         elif isinstance(index, Tensor):
             index = index.tolist()
         if column is None:
             column = self.column_names
 
         if is_iterable_str(column):
             return {column_i: self.at(index, column_i) for column_i in column}
 
-        if column not in self.column_names:
+        if column not in self.all_columns:
             raise ValueError(
-                f"Invalid argument {column=}. (expected one of {tuple(self.column_names)})"
+                f"Invalid argument {column=}. (expected one of {tuple(self.all_columns)})"
             )
 
-        if isinstance(index, slice):
-            is_mult = True
-        elif is_iterable_int(index):
+        if isinstance(index, slice) or is_iterable_int(index):
             is_mult = True
         elif isinstance(index, int):
             if not (-len(self) <= index < len(self)):
                 raise IndexError(
                     f"Invalid argument {index=}. (expected int in range [{-len(self)}, {len(self)-1}])"
                 )
             is_mult = False
@@ -269,31 +285,37 @@
                 hdf_value = hdf_value[slices]
 
             # Decode all bytes to string
             if hdf_dtype == HDF_STRING_DTYPE:
                 hdf_value = _decode_rec(hdf_value, HDF_ENCODING)
             # Convert numpy.array to torch.Tensor
             elif isinstance(hdf_value, np.ndarray):
-                if hdf_dtype != HDF_VOID_DTYPE:
+                if not self._numpy_to_torch:
+                    pass
+                elif hdf_dtype != HDF_VOID_DTYPE:
                     hdf_value = torch.from_numpy(hdf_value)
                 else:
                     hdf_value = hdf_value.tolist()
             # Convert numpy scalars
             elif np.isscalar(hdf_value) and hasattr(hdf_value, "item"):
                 hdf_value = hdf_value.item()  # type: ignore
 
             outputs.append(hdf_value)
 
         if not is_mult:
             outputs = outputs[0]
         return outputs
 
-    def close(self) -> None:
+    def close(self, ignore_if_closed: bool = False) -> None:
         if not self.is_open():
-            raise RuntimeError("Cannot close the HDF file twice.")
+            if ignore_if_closed:
+                return None
+            else:
+                raise RuntimeError("Cannot close the HDF file twice.")
+
         self._hdf_file.close()
         self._hdf_file = None
 
     def get_attrs(self) -> Dict[str, Any]:
         return self._hdf_file.attrs
 
     def get_hdf_fpath(self) -> Path:
@@ -313,18 +335,22 @@
 
     def is_closed(self) -> bool:
         return not self.is_open()
 
     def is_open(self) -> bool:
         return self._hdf_file is not None and bool(self._hdf_file)
 
-    def open(self) -> None:
+    def open(self, ignore_if_opened: bool = False) -> None:
         if self.is_open():
-            raise RuntimeError("Cannot open the HDF file twice.")
-        self._hdf_file = h5py.File(self._hdf_fpath, "r")
+            if ignore_if_opened:
+                return None
+            else:
+                raise RuntimeError("Cannot open the HDF file twice.")
+
+        self._hdf_file = h5py.File(self._hdf_fpath, "r", **self._file_kwargs)
         self._sanity_check()
 
     # Magic methods
     def __eq__(self, __o: object) -> bool:
         return isinstance(__o, HDFDataset) and pickle.dumps(self) == pickle.dumps(__o)
 
     def __exit__(self) -> None:
@@ -378,38 +404,50 @@
 
     def __getstate__(self) -> Dict[str, Any]:
         return {
             "hdf_fpath": self._hdf_fpath,
             "transform": self._transform,
             "keep_padding": self._keep_padding,
             "return_added_columns": self._return_added_columns,
+            "auto_open": self._auto_open,
+            "numpy_to_torch": self._numpy_to_torch,
+            "file_kwargs": self._file_kwargs,
             "is_open": self.is_open(),
         }
 
     def __hash__(self) -> int:
         hash_value = 0
         if self.is_open():
             hash_value += self._hdf_file.attrs["global_hash_value"]
         if self._transform is not None:
             hash_value += hash(self._transform)
         hash_value += sum(map(hash, self._keep_padding))
         return hash_value
 
     def __len__(self) -> int:
+        auto_close = False
         if self.is_closed():
-            msg = f"Cannot length of a closed HDF file. ({self._hdf_file is not None=} and {bool(self._hdf_file)=})"
-            raise RuntimeError(msg)
+            if self._auto_open:
+                self.open()
+                auto_close = True
+            else:
+                msg = f"Cannot length of a closed HDF file. ({self._hdf_file is not None=} and {bool(self._hdf_file)=})"
+                raise RuntimeError(msg)
 
         if "length" in self._hdf_file.attrs:
-            return self._hdf_file.attrs["length"]
+            length = self._hdf_file.attrs["length"]
         elif len(self._hdf_file) > 0:
             dataset: HDFRawDataset = next(iter(self._hdf_file.values()))
-            return len(dataset)
+            length = len(dataset)
         else:
-            return 0
+            length = 0
+
+        if auto_close:
+            self.close()
+        return length
 
     def __repr__(self) -> str:
         repr_hparams = {"file": osp.basename(self._hdf_fpath), "size": len(self)}
         repr_ = ", ".join(f"{k}={v}" for k, v in repr_hparams.items())
         return f"HDFDataset({repr_})"
 
     def __setstate__(self, data: Dict[str, Any]) -> None:
@@ -420,36 +458,42 @@
         if is_init and files_are_different and is_open:
             self.close()
 
         self._hdf_fpath = data["hdf_fpath"]
         self._transform = data["transform"]
         self._keep_padding = data["keep_padding"]
         self._return_added_columns = data["return_added_columns"]
+        self._auto_open = data["auto_open"]
+        self._numpy_to_torch = data["numpy_to_torch"]
+        self._file_kwargs = data["file_kwargs"]
+
         self._hdf_file = None
 
         if not is_init or (files_are_different and is_open):
             self.open()
 
     # Private methods
     def _sanity_check(self) -> None:
         lens = [dset.shape[0] for dset in self._hdf_file.values()]
         if not all_eq(lens) or lens[0] != len(self):
             logger.error(
                 f"Incorrect length stored in HDF file. (found {lens=} and {len(self)=})"
             )
 
-        if hasattr(self, "__orig_class__"):
-            t_type = self.__orig_class__.__args__[0]  # type: ignore
-            if t_type is not Any and (
-                (issubclass(t_type, dict) and self.item_type != "dict")
-                or (issubclass(t_type, tuple) and self.item_type != "tuple")
-            ):
-                raise TypeError(
-                    f"Invalid HDFDataset typing. (found specified type '{t_type.__name__}' but the internal dataset contains type '{self.item_type}')"
-                )
+        if not hasattr(self, "__orig_class__"):
+            return None
+
+        t_type = self.__orig_class__.__args__[0]  # type: ignore
+        if t_type is not Any and (
+            (issubclass(t_type, dict) and self.item_type != "dict")
+            or (issubclass(t_type, tuple) and self.item_type != "tuple")
+        ):
+            raise TypeError(
+                f"Invalid HDFDataset typing. (found specified type '{t_type.__name__}' but the internal dataset contains type '{self.item_type}')"
+            )
 
     def _raw_at(self, index: Union[int, Iterable[int], slice], column: str) -> Any:
         if isinstance(index, Iterable):
             sorted_idxs, local_idxs = torch.as_tensor(index).sort(dim=-1)
             sorted_idxs = sorted_idxs.numpy()
             hdf_value: Any = self._hdf_file[column][sorted_idxs]
             inv_local_idxs = get_inverse_perm(local_idxs)
```

### Comparing `torchoutil-0.2.2/src/torchoutil/utils/hdf/pack.py` & `torchoutil-0.3.0/src/torchoutil/utils/hdf/pack.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 import numpy as np
 import torch
 import tqdm
 from h5py import Dataset as HDFRawDataset
 from torch import Tensor, nn
 from torch.utils.data.dataloader import DataLoader
 
-from torchoutil.utils.collections import all_eq
+from torchoutil.nn.functional.numpy import is_numpy_scalar
+from torchoutil.utils.collections import all_eq, unzip
 from torchoutil.utils.data.dataloader import get_auto_num_cpus
 from torchoutil.utils.data.dataset import SizedDatasetLike
 from torchoutil.utils.hdf.common import (
     HDF_ENCODING,
     HDF_STRING_DTYPE,
     HDF_VOID_DTYPE,
     SHAPE_SUFFIX,
@@ -63,14 +64,16 @@
     pre_transform: Optional[Callable[[T], U]] = None,
     overwrite: bool = False,
     metadata: str = "",
     verbose: int = 0,
     batch_size: int = 32,
     num_workers: Union[int, Literal["auto"]] = "auto",
     shape_suffix: str = SHAPE_SUFFIX,
+    open_hdf: bool = True,
+    file_kwargs: Optional[Dict[str, Any]] = None,
 ) -> HDFDataset[U, U]:
     """Pack a dataset to HDF file.
 
     Args:
         dataset: The sized dataset to pack. Must be sized and all items must be of dict type.
             The key of each dictionaries are strings and values can be int, float, str, Tensor, non-empty List[int], non-empty List[float], non-empty List[str].
             If values are tensors or lists, the number of dimensions must be the same for all items in the dataset.
@@ -79,22 +82,27 @@
             Can be used for deterministic transforms like Resample, LogMelSpectrogram, etc. defaults to None.
         overwrite: If True, the file hdf_fpath can be overwritten. defaults to False.
         metadata: Additional metadata string to add to the hdf file. defaults to ''.
         verbose: Verbose level. defaults to 0.
         batch_size: The batch size of the dataloader. defaults to 32.
         num_workers: The number of workers of the dataloader.
             If "auto", it will be set to `len(os.sched_getaffinity(0))`. defaults to "auto".
+        shape_suffix: Shape column suffix in HDF file. defaults to "_shape".
+        open_hdf: If True, opens the output HDF dataset. defaults to True.
+        file_kwargs: Options given to h5py file object. defaults to None.
     """
     # Check inputs
     if not isinstance(dataset, SizedDatasetLike):
         raise TypeError(
             f"Cannot pack to hdf a non-sized-dataset '{dataset.__class__.__name__}'."
         )
     if len(dataset) == 0:
         raise ValueError("Cannot pack to hdf an empty dataset.")
+    if file_kwargs is None:
+        file_kwargs = {}
 
     hdf_fpath = Path(hdf_fpath).resolve()
     if hdf_fpath.exists() and not hdf_fpath.is_file():
         raise RuntimeError(f"Item {hdf_fpath=} exists but it is not a file.")
 
     if hdf_fpath.is_file() and not overwrite:
         raise ValueError(
@@ -131,15 +139,15 @@
     else:
         raise ValueError(
             f"Invalid item type for {dataset.__class__.__name__}. (expected dict[str, Any] or tuple but found {type(item_0)})"
         )
     del pre_transform, item_0
 
     for attr_name, value in item_0_dict.items():
-        shape, hdf_dtype = _get_shape_and_dtype(value)
+        shape, hdf_dtype, _src_dtype = _get_shape_and_dtype(value)
         shapes_0[attr_name] = shape
         hdf_dtypes_0[attr_name] = hdf_dtype
 
     max_shapes: Dict[str, Tuple[int, ...]] = shapes_0
     hdf_dtypes: Dict[str, str] = hdf_dtypes_0
     all_eq_shapes: Dict[str, bool] = {
         attr_name: True for attr_name in item_0_dict.keys()
@@ -160,15 +168,15 @@
         desc="Pre compute shapes...",
         disable=verbose <= 0,
     ):
         batch = [dict_pre_transform(item) for item in batch]
 
         for item in batch:
             for attr_name, value in item.items():
-                shape, hdf_dtype = _get_shape_and_dtype(value)
+                shape, hdf_dtype, _src_dtype = _get_shape_and_dtype(value)
                 all_eq_shapes[attr_name] &= max_shapes[attr_name] == shape
                 max_shapes[attr_name] = tuple(
                     map(max, zip(max_shapes[attr_name], shape))
                 )
                 if hdf_dtypes[attr_name] == hdf_dtype or hdf_dtype == HDF_VOID_DTYPE:
                     # Note: HDF_VOID_DTYPE is compatible
                     pass
@@ -197,15 +205,19 @@
         else:
             info = {}
     else:
         info = {}
 
     added_columns = []
 
-    with h5py.File(hdf_fpath, "w") as hdf_file:
+    with h5py.File(
+        hdf_fpath,
+        "w",
+        **file_kwargs,
+    ) as hdf_file:
         # Step 2: Build hdf datasets in file
         hdf_dsets: Dict[str, HDFRawDataset] = {}
 
         for attr_name, shape in max_shapes.items():
             hdf_dtype = hdf_dtypes.get(attr_name)
 
             kwargs: Dict[str, Any] = {}
@@ -273,15 +285,15 @@
             disable=verbose <= 0,
         ):
             batch = [dict_pre_transform(item) for item in batch]
 
             for item in batch:
                 for attr_name, value in item.items():
                     hdf_dset = hdf_dsets[attr_name]
-                    shape, hdf_dtype = _get_shape_and_dtype(value)
+                    shape, hdf_dtype, _src_dtype = _get_shape_and_dtype(value)
 
                     # Check every shape
                     if len(shape) != hdf_dset.ndim - 1:
                         raise ValueError(
                             f"Invalid number of dimension in audio (expected {len(shape)}, found {len(shape)})."
                         )
 
@@ -336,14 +348,15 @@
             "metadata": str(metadata),
             "encoding": HDF_ENCODING,
             "info": json.dumps(info),
             "global_hash_value": global_hash_value,
             "item_type": item_type,
             "added_columns": added_columns,
             "shape_suffix": shape_suffix,
+            "file_kwargs": json.dumps(info),
         }
         if verbose >= 2:
             dumped_attributes = json.dumps(attributes, indent="\t")
             pylog.debug(f"Saving attributes in HDF file:\n{dumped_attributes}")
 
         for attr_name, attr_val in attributes.items():
             try:
@@ -353,15 +366,15 @@
                     f"Cannot store attribute {attr_name=} with value {attr_val=} in HDF."
                 )
                 raise err
 
     if verbose >= 2:
         pylog.debug(f"Data into has been packed into HDF file '{hdf_fpath}'.")
 
-    hdf_dataset = HDFDataset(hdf_fpath, open_hdf=True, return_added_columns=False)
+    hdf_dataset = HDFDataset(hdf_fpath, open_hdf=open_hdf, return_added_columns=False)
     return hdf_dataset
 
 
 class Compose:
     def __init__(self, *fns: Callable) -> None:
         super().__init__()
         self.fns = fns
@@ -386,70 +399,79 @@
     elif isinstance(value, (list, tuple)):
         return sum(map(_checksum, value))
     else:
         raise TypeError(f"Invalid argument type {value.__class__.__name__}.")
 
 
 def _get_shape_and_dtype(
-    value: Union[int, float, str, Tensor, list]
-) -> Tuple[Tuple[int, ...], _HDFDType]:
+    x: Union[int, float, str, list, Tensor, np.ndarray]
+) -> Tuple[Tuple[int, ...], _HDFDType, str]:
     """Returns the shape and the hdf_dtype for an input."""
-    if isinstance(value, int):
+    if isinstance(x, int):
         shape = ()
         hdf_dtype = "i"
+        src_dtype = "int"
 
-    elif isinstance(value, float):
+    elif isinstance(x, float):
         shape = ()
         hdf_dtype = "f"
+        src_dtype = "float"
 
-    elif isinstance(value, str):
+    elif isinstance(x, str):
         shape = ()
         hdf_dtype = HDF_STRING_DTYPE
+        src_dtype = "str"
 
-    elif isinstance(value, Tensor):
-        shape = tuple(value.shape)
-        if value.is_floating_point():
+    elif isinstance(x, Tensor):
+        shape = tuple(x.shape)
+        if x.is_floating_point():
             hdf_dtype = "f"
         else:
             hdf_dtype = "i"
+        src_dtype = str(x.dtype)
 
-    elif isinstance(value, np.ndarray):
-        shape = tuple(value.shape)
-        hdf_dtype = value.dtype.kind
-        if hdf_dtype == "u":
+    elif isinstance(x, np.ndarray) or is_numpy_scalar(x):
+        shape = tuple(x.shape)
+        dtype_kind = x.dtype.kind
+        if dtype_kind == "u":
             hdf_dtype = "i"
+        else:
+            hdf_dtype = dtype_kind
+        src_dtype = str(x.dtype)
 
-    elif isinstance(value, (list, tuple)):
-        if len(value) == 0:
+    elif isinstance(x, (list, tuple)):
+        if len(x) == 0:
             shape = (0,)
             hdf_dtype = HDF_VOID_DTYPE
+            src_dtype = "void"
         else:
-            sub_shapes_and_dtypes = list(map(_get_shape_and_dtype, value))
-            sub_shapes = [shape for shape, _ in sub_shapes_and_dtypes]
-            sub_dtypes = [dtype for _, dtype in sub_shapes_and_dtypes]
+            sub_data = list(map(_get_shape_and_dtype, x))
+            sub_shapes, sub_hdf_dtypes, sub_src_dtypes = unzip(sub_data)
             sub_dims = list(map(len, sub_shapes))
 
             if not all_eq(sub_dims):
                 raise TypeError(
                     f"Unsupported list of heterogeneous shapes lengths. (found {sub_dims=})"
                 )
-            if not all_eq(sub_dtypes):
+            if not all_eq(sub_hdf_dtypes):
                 raise TypeError(
-                    f"Unsupported list of heterogeneous types. (found {sub_dtypes=})"
+                    f"Unsupported list of heterogeneous types. (found {sub_hdf_dtypes=})"
                 )
-            # Check for avoid ragged array like [["a", "b"], ["c"], ["d", "e"]]
+            # Check to avoid ragged array like [["a", "b"], ["c"], ["d", "e"]]
             if not all_eq(sub_shapes):
                 raise TypeError(
-                    f"Unsupported list of heterogeneous shapes. (found {sub_shapes=} for {value=})"
+                    f"Unsupported list of heterogeneous shapes. (found {sub_shapes=} for {x=})"
                 )
 
             max_subshape = tuple(
                 max(shape[i] for shape in sub_shapes) for i in range(len(sub_shapes[0]))
             )
-            shape = (len(value),) + max_subshape
-            hdf_dtype = sub_dtypes[0]
+            shape = (len(x),) + max_subshape
+            hdf_dtype = sub_hdf_dtypes[0]
+
+            src_dtype = str(list(dict.fromkeys(sub_src_dtypes)))
     else:
         raise TypeError(
-            f"Unsupported type {value.__class__.__name__} in function get_shape_and_dtype."
+            f"Unsupported type {x.__class__.__name__} in function get_shape_and_dtype."
         )
 
-    return shape, hdf_dtype
+    return shape, hdf_dtype, src_dtype
```

### Comparing `torchoutil-0.2.2/src/torchoutil/utils/packaging.py` & `torchoutil-0.3.0/src/torchoutil/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.2.2/src/torchoutil/utils/return_types.py` & `torchoutil-0.3.0/src/torchoutil/utils/return_types.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.2.2/src/torchoutil/utils/tensorboard.py` & `torchoutil-0.3.0/src/torchoutil/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.2.2/src/torchoutil/utils/type_checks.py` & `torchoutil-0.3.0/src/torchoutil/utils/type_checks.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.2.2/src/torchoutil.egg-info/PKG-INFO` & `torchoutil-0.3.0/src/torchoutil.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchoutil
-Version: 0.2.2
+Version: 0.3.0
 Summary: Collection of functions and modules to help development in PyTorch.
 Author-email: "Étienne Labbé (Labbeti)" <labbeti.pub@gmail.com>
 Maintainer-email: "Étienne Labbé (Labbeti)" <labbeti.pub@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Labbeti
         
@@ -75,15 +75,15 @@
 
 
 ## Installation
 ```bash
 pip install torchoutil
 ```
 
-The only requirement is **pytorch**.
+The only requirement is **PyTorch**.
 
 To check if the package is installed and show the package version, you can use the following command:
 ```bash
 torchoutil-info
 ```
 
 
@@ -101,15 +101,15 @@
 ```
 
 ```python
 import torch
 from torchoutil import lengths_to_non_pad_mask
 
 x = torch.as_tensor([3, 1, 2])
-pad_mask = lengths_to_non_pad_mask(x, max_len=4)
+mask = lengths_to_non_pad_mask(x, max_len=4)
 # Each row i contains x[i] True values for non-padding mask
 # tensor([[True, True, True, False],
 #         [True, False, False, False],
 #         [True, True, False, False]])
 ```
 
 ### Multilabel conversions
@@ -155,15 +155,15 @@
 # inv_perm are indices that allow us to get x3 from x2, i.e. x1 == x3 here
 ```
 
 ## Extras
 `torchoutil` also provides additional modules when some specific package are already installed in your environment.
 All extras can be installed with `pip install torchoutil[extras]`
 
-If `tensorboard` is installed, the function `load_event_file` can be used.
-If `numpy` is installed, the classes `FromNumpy` and  `ToNumpy` can be used and their related function.
-If `h5py` is installed, the function `pack_to_hdf` and class `HDFDataset` can be used.
+- If `tensorboard` is installed, the function `load_event_file` can be used. It is useful to load manually all data contained in an tensorboard event file.
+- If `numpy` is installed, the classes `FromNumpy` and  `ToNumpy` can be used and their related function. It is meant to be used to compose dynamic transforms into `Sequential` module.
+- If `h5py` is installed, the function `pack_to_hdf` and class `HDFDataset` can be used. Can be used to pack/read dataset to HDF files, and supports variable-length sequences of data.
 
 
 ## Contact
 Maintainer:
-- Étienne Labbé "Labbeti": labbeti.pub@gmail.com
+- [Étienne Labbé](https://labbeti.github.io/) "Labbeti": labbeti.pub@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchoutil Version: 0.2.2 Summary: Collection of
+Metadata-Version: 2.1 Name: torchoutil Version: 0.3.0 Summary: Collection of
 functions and modules to help development in PyTorch. Author-email: "Ãtienne
 LabbÃ© (Labbeti)"
 gmail.com> Maintainer-email: "Ãtienne LabbÃ© (Labbeti)"
 gmail.com> License: MIT License Copyright (c) 2024 Labbeti Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
@@ -30,21 +30,21 @@
 Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 extras Provides-Extra: dev License-File: LICENSE # torchoutil
 _[_P_y_t_h_o_n_]_[_P_y_T_o_r_c_h_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_B_u_i_l_d_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]Collection of
              functions and modules to help development in PyTorch.
 ## Installation ```bash pip install torchoutil ``` The only requirement is
-**pytorch**. To check if the package is installed and show the package version,
+**PyTorch**. To check if the package is installed and show the package version,
 you can use the following command: ```bash torchoutil-info ``` ## Usage ###
 Batch of padded sequences ```python import torch from torchoutil import
 masked_mean x = torch.as_tensor([1, 2, 3, 4]) mask = torch.as_tensor([True,
 True, False, False]) result = masked_mean(x, mask) # result contains the mean
 of the values marked as True: 1.5 ``` ```python import torch from torchoutil
-import lengths_to_non_pad_mask x = torch.as_tensor([3, 1, 2]) pad_mask =
+import lengths_to_non_pad_mask x = torch.as_tensor([3, 1, 2]) mask =
 lengths_to_non_pad_mask(x, max_len=4) # Each row i contains x[i] True values
 for non-padding mask # tensor([[True, True, True, False], # [True, False,
 False, False], # [True, True, False, False]]) ``` ### Multilabel conversions
 ```python import torch from torchoutil import probs_to_names probs =
 torch.as_tensor([[0.9, 0.1], [0.6, 0.9]]) names = probs_to_names(probs,
 threshold=0.5, idx_to_name={0: "Cat", 1: "Dog"}) # [["Cat"], ["Cat", "Dog"]]
 ``` ```python import torch from torchoutil import multihot_to_indices multihot
@@ -54,13 +54,16 @@
 x = torch.as_tensor([1, 2, 3, 4]) result = insert_at_indices(x, indices=[0, 2],
 values=5) # result contains tensor with inserted values: tensor([5, 1, 2, 5, 3,
 4]) ``` ```python import torch from torchoutil import get_inverse_perm perm =
 torch.randperm(10) inv_perm = get_inverse_perm(perm) x1 = torch.rand(10) x2 =
 x1[perm] x3 = x2[inv_perm] # inv_perm are indices that allow us to get x3 from
 x2, i.e. x1 == x3 here ``` ## Extras `torchoutil` also provides additional
 modules when some specific package are already installed in your environment.
-All extras can be installed with `pip install torchoutil[extras]` If
-`tensorboard` is installed, the function `load_event_file` can be used. If
+All extras can be installed with `pip install torchoutil[extras]` - If
+`tensorboard` is installed, the function `load_event_file` can be used. It is
+useful to load manually all data contained in an tensorboard event file. - If
 `numpy` is installed, the classes `FromNumpy` and `ToNumpy` can be used and
-their related function. If `h5py` is installed, the function `pack_to_hdf` and
-class `HDFDataset` can be used. ## Contact Maintainer: - Ãtienne LabbÃ©
-"Labbeti": labbeti.pub@gmail.com
+their related function. It is meant to be used to compose dynamic transforms
+into `Sequential` module. - If `h5py` is installed, the function `pack_to_hdf`
+and class `HDFDataset` can be used. Can be used to pack/read dataset to HDF
+files, and supports variable-length sequences of data. ## Contact Maintainer: -
+[Ãtienne LabbÃ©](https://labbeti.github.io/) "Labbeti": labbeti.pub@gmail.com
```

### Comparing `torchoutil-0.2.2/src/torchoutil.egg-info/SOURCES.txt` & `torchoutil-0.3.0/src/torchoutil.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 src/torchoutil/info.py
 src/torchoutil.egg-info/PKG-INFO
 src/torchoutil.egg-info/SOURCES.txt
 src/torchoutil.egg-info/dependency_links.txt
 src/torchoutil.egg-info/entry_points.txt
 src/torchoutil.egg-info/requires.txt
 src/torchoutil.egg-info/top_level.txt
+src/torchoutil/hub/__init__.py
+src/torchoutil/hub/download.py
+src/torchoutil/hub/registry.py
 src/torchoutil/nn/__init__.py
 src/torchoutil/nn/functional/__init__.py
 src/torchoutil/nn/functional/activation.py
 src/torchoutil/nn/functional/crop.py
 src/torchoutil/nn/functional/get.py
 src/torchoutil/nn/functional/indices.py
 src/torchoutil/nn/functional/mask.py
@@ -26,40 +29,41 @@
 src/torchoutil/nn/functional/numpy.py
 src/torchoutil/nn/functional/others.py
 src/torchoutil/nn/functional/pad.py
 src/torchoutil/nn/functional/repeat.py
 src/torchoutil/nn/modules/__init__.py
 src/torchoutil/nn/modules/activation.py
 src/torchoutil/nn/modules/crop.py
+src/torchoutil/nn/modules/layer.py
 src/torchoutil/nn/modules/mask.py
 src/torchoutil/nn/modules/multiclass.py
 src/torchoutil/nn/modules/multilabel.py
 src/torchoutil/nn/modules/numpy.py
 src/torchoutil/nn/modules/pad.py
 src/torchoutil/nn/modules/repeat.py
 src/torchoutil/nn/modules/tensor.py
 src/torchoutil/nn/modules/typed.py
 src/torchoutil/optim/__init__.py
 src/torchoutil/optim/utils.py
 src/torchoutil/utils/__init__.py
-src/torchoutil/utils/ckpt.py
 src/torchoutil/utils/collections.py
 src/torchoutil/utils/packaging.py
 src/torchoutil/utils/return_types.py
 src/torchoutil/utils/tensorboard.py
 src/torchoutil/utils/type_checks.py
 src/torchoutil/utils/data/__init__.py
 src/torchoutil/utils/data/collate.py
 src/torchoutil/utils/data/dataloader.py
 src/torchoutil/utils/data/dataset.py
 src/torchoutil/utils/data/split.py
 src/torchoutil/utils/hdf/__init__.py
 src/torchoutil/utils/hdf/common.py
 src/torchoutil/utils/hdf/dataset.py
 src/torchoutil/utils/hdf/pack.py
+tests/test_hub.py
 tests/test_nn_functional_crop.py
 tests/test_nn_functional_indices.py
 tests/test_nn_functional_mask.py
 tests/test_nn_functional_multilabel.py
 tests/test_nn_functional_others.py
 tests/test_nn_functional_pad.py
 tests/test_nn_functional_repeat.py
```

### Comparing `torchoutil-0.2.2/tests/test_nn_functional_indices.py` & `torchoutil-0.3.0/tests/test_nn_functional_indices.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.2.2/tests/test_nn_functional_mask.py` & `torchoutil-0.3.0/tests/test_nn_functional_mask.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.2.2/tests/test_nn_functional_multilabel.py` & `torchoutil-0.3.0/tests/test_nn_functional_multilabel.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.2.2/tests/test_nn_functional_others.py` & `torchoutil-0.3.0/tests/test_nn_functional_others.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,10 +26,22 @@
         lst = [[[]], [[]]]
         self.assertTrue(can_be_converted_to_tensor(lst))
 
     def test_can_be_converted_to_tensor_5(self) -> None:
         lst = [torch.rand(10), torch.rand(10)]
         self.assertFalse(can_be_converted_to_tensor(lst))
 
+    def test_can_be_converted_to_tensor_6(self) -> None:
+        lst = [[torch.rand(10)]]
+        self.assertFalse(can_be_converted_to_tensor(lst))
+
+    def test_can_be_converted_to_tensor_7(self) -> None:
+        lst = torch.rand(10)
+        self.assertTrue(can_be_converted_to_tensor(lst))
+
+    def test_can_be_converted_to_tensor_8(self) -> None:
+        lst = [(), []]
+        self.assertTrue(can_be_converted_to_tensor(lst))
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `torchoutil-0.2.2/tests/test_nn_functional_pad.py` & `torchoutil-0.3.0/tests/test_nn_functional_pad.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.2.2/tests/test_nn_functional_repeat.py` & `torchoutil-0.3.0/tests/test_nn_functional_repeat.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.2.2/tests/test_nn_modules_multilabel.py` & `torchoutil-0.3.0/tests/test_nn_modules_multilabel.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.2.2/tests/test_readme.py` & `torchoutil-0.3.0/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.2.2/tests/test_utils_ckpt.py` & `torchoutil-0.3.0/tests/test_utils_ckpt.py`

 * *Files identical despite different names*

### Comparing `torchoutil-0.2.2/tests/test_utils_collections.py` & `torchoutil-0.3.0/tests/test_utils_collections.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import unittest
 from unittest import TestCase
 
-from torchoutil.utils.collections import flat_dict_of_dict, list_dict_to_dict_list
+from torchoutil.utils.collections import (
+    flat_dict_of_dict,
+    intersect_lists,
+    list_dict_to_dict_list,
+)
 
 
 class TestCollections(TestCase):
     def test_example_1(self) -> None:
         x = {
             "a": 1,
             "b": {
@@ -42,10 +46,38 @@
 
 class TestListDictToDictList(TestCase):
     def test_example_1(self) -> None:
         lst = [{"a": 1, "b": 2}, {"a": 4, "b": 3, "c": 5}]
         output = list_dict_to_dict_list(lst, default_val=0)
         self.assertDictEqual(output, {"a": [1, 4], "b": [2, 3], "c": [0, 5]})
 
+    def test_example_2(self) -> None:
+        lst = [{"a": 1, "b": 2}, {"a": 4, "b": 3, "c": 5}]
+
+        with self.assertRaises(ValueError):
+            list_dict_to_dict_list(
+                lst,
+                default_val=None,
+                key_mode="same",
+            )
+
+    def test_example_3(self) -> None:
+        lst = [{"a": 1, "b": 2, "c": 3}, {"a": 11, "b": 22, "c": 33}]
+        output = list_dict_to_dict_list(
+            lst,
+            default_val=None,
+            key_mode="same",
+        )
+        self.assertDictEqual(output, {"a": [1, 11], "b": [2, 22], "c": [3, 33]})
+
+
+class TestIntersectLists(TestCase):
+    def test_example_1(self) -> None:
+        input_ = [["a", "b", "b", "c"], ["c", "d", "b", "a"], ["b", "a", "a", "e"]]
+        expected = ["a", "b"]
+
+        output = intersect_lists(input_)
+        self.assertListEqual(output, expected)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `torchoutil-0.2.2/tests/test_utils_hdf.py` & `torchoutil-0.3.0/tests/test_utils_hdf.py`

 * *Files identical despite different names*

