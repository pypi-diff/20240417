# Comparing `tmp/vit-pytorch-1.6.5.tar.gz` & `tmp/vit_pytorch-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vit-pytorch-1.6.5.tar", last modified: Sat Dec 23 16:12:17 2023, max compression
+gzip compressed data, was "vit_pytorch-1.6.6.tar", last modified: Wed Apr 17 16:40:45 2024, max compression
```

## Comparing `vit-pytorch-1.6.5.tar` & `vit_pytorch-1.6.6.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 16:12:17.464836 vit-pytorch-1.6.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      694 2023-12-23 16:12:17.464836 vit-pytorch-1.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    65041 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-23 16:12:17.464836 vit-pytorch-1.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      959 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 16:12:17.452835 vit-pytorch-1.6.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/tests/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 16:12:17.460836 vit-pytorch-1.6.5/vit_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10095 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/ats_vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/cait.py
--rw-r--r--   0 runner    (1001) docker     (127)    12001 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/cct.py
--rw-r--r--   0 runner    (1001) docker     (127)    12186 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/cct_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8980 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/cross_vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     8347 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/crossformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5935 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/cvt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/deepvit.py
--rw-r--r--   0 runner    (1001) docker     (127)     9662 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/dino.py
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/distill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/efficient.py
--rw-r--r--   0 runner    (1001) docker     (127)    12657 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/es_vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7308 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/learnable_memory_vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/levit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/local_vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/mae.py
--rw-r--r--   0 runner    (1001) docker     (127)     8315 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/max_vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     9892 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/max_vit_with_registers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7675 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/mobile_vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     6160 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/mp3.py
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/mpp.py
--rw-r--r--   0 runner    (1001) docker     (127)    12364 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/na_vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5837 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/nest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/parallel_vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5666 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/pit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/recorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     9055 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/regionvit.py
--rw-r--r--   0 runner    (1001) docker     (127)     7626 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/rvt.py
--rw-r--r--   0 runner    (1001) docker     (127)     9585 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/scalable_vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     8857 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/sep_vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/simmim.py
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/simple_flash_attn_vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3834 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/simple_vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/simple_vit_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/simple_vit_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/simple_vit_with_fft.py
--rw-r--r--   0 runner    (1001) docker     (127)     4652 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/simple_vit_with_patch_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/simple_vit_with_qk_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/simple_vit_with_register_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/t2t.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/twins_svt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/vit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/vit_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/vit_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4829 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/vit_for_small_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/vit_with_patch_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/vit_with_patch_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/vivit.py
--rw-r--r--   0 runner    (1001) docker     (127)     8539 2023-12-23 16:12:08.000000 vit-pytorch-1.6.5/vit_pytorch/xcit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 16:12:17.464836 vit-pytorch-1.6.5/vit_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2023-12-23 16:12:17.000000 vit-pytorch-1.6.5/vit_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2023-12-23 16:12:17.000000 vit-pytorch-1.6.5/vit_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-23 16:12:17.000000 vit-pytorch-1.6.5/vit_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-23 16:12:17.000000 vit-pytorch-1.6.5/vit_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-23 16:12:17.000000 vit-pytorch-1.6.5/vit_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:40:45.813581 vit_pytorch-1.6.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    65736 2024-04-17 16:40:45.813581 vit_pytorch-1.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    65041 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 16:40:45.813581 vit_pytorch-1.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:40:45.801581 vit_pytorch-1.6.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:40:45.809581 vit_pytorch-1.6.6/vit_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10095 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/ats_vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/cait.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12001 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/cct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12186 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/cct_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/cross_vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/crossformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/cvt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/deepvit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9662 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/dino.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/distill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/efficient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12657 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/es_vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/learnable_memory_vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/levit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/local_vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/mae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8315 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/max_vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9892 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/max_vit_with_registers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7675 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/mobile_vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/mp3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/mpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12364 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/na_vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/nest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/parallel_vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/pit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/recorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9055 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/regionvit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7626 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/rvt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9585 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/scalable_vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/sep_vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/simmim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/simple_flash_attn_vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/simple_vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/simple_vit_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/simple_vit_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/simple_vit_with_fft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/simple_vit_with_patch_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/simple_vit_with_qk_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/simple_vit_with_register_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/t2t.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/twins_svt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/vit_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/vit_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/vit_for_small_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/vit_with_patch_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/vit_with_patch_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/vivit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-04-17 16:40:37.000000 vit_pytorch-1.6.6/vit_pytorch/xcit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:40:45.813581 vit_pytorch-1.6.6/vit_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    65736 2024-04-17 16:40:45.000000 vit_pytorch-1.6.6/vit_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-17 16:40:45.000000 vit_pytorch-1.6.6/vit_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:40:45.000000 vit_pytorch-1.6.6/vit_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 16:40:45.000000 vit_pytorch-1.6.6/vit_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 16:40:45.000000 vit_pytorch-1.6.6/vit_pytorch.egg-info/top_level.txt
```

### Comparing `vit-pytorch-1.6.5/LICENSE` & `vit_pytorch-1.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/README.md` & `vit_pytorch-1.6.6/README.md`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/setup.py` & `vit_pytorch-1.6.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from setuptools import setup, find_packages
 
+with open('README.md') as f:
+    long_description = f.read()
+
 setup(
   name = 'vit-pytorch',
   packages = find_packages(exclude=['examples']),
-  version = '1.6.5',
+  version = '1.6.6',
   license='MIT',
   description = 'Vision Transformer (ViT) - Pytorch',
+  long_description=long_description,
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/vit-pytorch',
   keywords = [
     'artificial intelligence',
     'attention mechanism',
```

### Comparing `vit-pytorch-1.6.5/vit_pytorch/ats_vit.py` & `vit_pytorch-1.6.6/vit_pytorch/ats_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/cait.py` & `vit_pytorch-1.6.6/vit_pytorch/cait.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/cct.py` & `vit_pytorch-1.6.6/vit_pytorch/cct.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/cct_3d.py` & `vit_pytorch-1.6.6/vit_pytorch/cct_3d.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/cross_vit.py` & `vit_pytorch-1.6.6/vit_pytorch/cross_vit.py`

 * *Files 5% similar despite different names*

```diff
@@ -166,20 +166,21 @@
 class ImageEmbedder(nn.Module):
     def __init__(
         self,
         *,
         dim,
         image_size,
         patch_size,
-        dropout = 0.
+        dropout = 0.,
+        channels = 3
     ):
         super().__init__()
         assert image_size % patch_size == 0, 'Image dimensions must be divisible by the patch size.'
         num_patches = (image_size // patch_size) ** 2
-        patch_dim = 3 * patch_size ** 2
+        patch_dim = channels * patch_size ** 2
 
         self.to_patch_embedding = nn.Sequential(
             Rearrange('b c (h p1) (w p2) -> b (h w) (p1 p2 c)', p1 = patch_size, p2 = patch_size),
             nn.LayerNorm(patch_dim),
             nn.Linear(patch_dim, dim),
             nn.LayerNorm(dim)
         )
@@ -219,19 +220,20 @@
         lg_enc_mlp_dim = 2048,
         lg_enc_dim_head = 64,
         cross_attn_depth = 2,
         cross_attn_heads = 8,
         cross_attn_dim_head = 64,
         depth = 3,
         dropout = 0.1,
-        emb_dropout = 0.1
+        emb_dropout = 0.1,
+        channels = 3
     ):
         super().__init__()
-        self.sm_image_embedder = ImageEmbedder(dim = sm_dim, image_size = image_size, patch_size = sm_patch_size, dropout = emb_dropout)
-        self.lg_image_embedder = ImageEmbedder(dim = lg_dim, image_size = image_size, patch_size = lg_patch_size, dropout = emb_dropout)
+        self.sm_image_embedder = ImageEmbedder(dim = sm_dim, channels= channels, image_size = image_size, patch_size = sm_patch_size, dropout = emb_dropout)
+        self.lg_image_embedder = ImageEmbedder(dim = lg_dim, channels = channels, image_size = image_size, patch_size = lg_patch_size, dropout = emb_dropout)
 
         self.multi_scale_encoder = MultiScaleEncoder(
             depth = depth,
             sm_dim = sm_dim,
             lg_dim = lg_dim,
             cross_attn_heads = cross_attn_heads,
             cross_attn_dim_head = cross_attn_dim_head,
```

### Comparing `vit-pytorch-1.6.5/vit_pytorch/crossformer.py` & `vit_pytorch-1.6.6/vit_pytorch/crossformer.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/cvt.py` & `vit_pytorch-1.6.6/vit_pytorch/cvt.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/deepvit.py` & `vit_pytorch-1.6.6/vit_pytorch/deepvit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/dino.py` & `vit_pytorch-1.6.6/vit_pytorch/dino.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/distill.py` & `vit_pytorch-1.6.6/vit_pytorch/distill.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/efficient.py` & `vit_pytorch-1.6.6/vit_pytorch/efficient.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/es_vit.py` & `vit_pytorch-1.6.6/vit_pytorch/es_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/extractor.py` & `vit_pytorch-1.6.6/vit_pytorch/extractor.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/learnable_memory_vit.py` & `vit_pytorch-1.6.6/vit_pytorch/learnable_memory_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/levit.py` & `vit_pytorch-1.6.6/vit_pytorch/levit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/local_vit.py` & `vit_pytorch-1.6.6/vit_pytorch/local_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/mae.py` & `vit_pytorch-1.6.6/vit_pytorch/mae.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/max_vit.py` & `vit_pytorch-1.6.6/vit_pytorch/max_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/max_vit_with_registers.py` & `vit_pytorch-1.6.6/vit_pytorch/max_vit_with_registers.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/mobile_vit.py` & `vit_pytorch-1.6.6/vit_pytorch/mobile_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/mp3.py` & `vit_pytorch-1.6.6/vit_pytorch/mp3.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/mpp.py` & `vit_pytorch-1.6.6/vit_pytorch/mpp.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/na_vit.py` & `vit_pytorch-1.6.6/vit_pytorch/na_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/nest.py` & `vit_pytorch-1.6.6/vit_pytorch/nest.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/parallel_vit.py` & `vit_pytorch-1.6.6/vit_pytorch/parallel_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/pit.py` & `vit_pytorch-1.6.6/vit_pytorch/pit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/recorder.py` & `vit_pytorch-1.6.6/vit_pytorch/recorder.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/regionvit.py` & `vit_pytorch-1.6.6/vit_pytorch/regionvit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/rvt.py` & `vit_pytorch-1.6.6/vit_pytorch/rvt.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/scalable_vit.py` & `vit_pytorch-1.6.6/vit_pytorch/scalable_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/sep_vit.py` & `vit_pytorch-1.6.6/vit_pytorch/sep_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/simmim.py` & `vit_pytorch-1.6.6/vit_pytorch/simmim.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/simple_flash_attn_vit.py` & `vit_pytorch-1.6.6/vit_pytorch/simple_flash_attn_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/simple_vit.py` & `vit_pytorch-1.6.6/vit_pytorch/simple_vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/simple_vit_1d.py` & `vit_pytorch-1.6.6/vit_pytorch/simple_vit_1d.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/simple_vit_3d.py` & `vit_pytorch-1.6.6/vit_pytorch/simple_vit_3d.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/simple_vit_with_fft.py` & `vit_pytorch-1.6.6/vit_pytorch/simple_vit_with_fft.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/simple_vit_with_patch_dropout.py` & `vit_pytorch-1.6.6/vit_pytorch/simple_vit_with_patch_dropout.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/simple_vit_with_qk_norm.py` & `vit_pytorch-1.6.6/vit_pytorch/simple_vit_with_qk_norm.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/simple_vit_with_register_tokens.py` & `vit_pytorch-1.6.6/vit_pytorch/simple_vit_with_register_tokens.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/t2t.py` & `vit_pytorch-1.6.6/vit_pytorch/t2t.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/twins_svt.py` & `vit_pytorch-1.6.6/vit_pytorch/twins_svt.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/vit.py` & `vit_pytorch-1.6.6/vit_pytorch/vit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/vit_1d.py` & `vit_pytorch-1.6.6/vit_pytorch/vit_1d.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/vit_3d.py` & `vit_pytorch-1.6.6/vit_pytorch/vit_3d.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/vit_for_small_dataset.py` & `vit_pytorch-1.6.6/vit_pytorch/vit_for_small_dataset.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/vit_with_patch_dropout.py` & `vit_pytorch-1.6.6/vit_pytorch/vit_with_patch_dropout.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/vit_with_patch_merger.py` & `vit_pytorch-1.6.6/vit_pytorch/vit_with_patch_merger.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/vivit.py` & `vit_pytorch-1.6.6/vit_pytorch/vivit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch/xcit.py` & `vit_pytorch-1.6.6/vit_pytorch/xcit.py`

 * *Files identical despite different names*

### Comparing `vit-pytorch-1.6.5/vit_pytorch.egg-info/SOURCES.txt` & `vit_pytorch-1.6.6/vit_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

