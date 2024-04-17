# Comparing `tmp/muben-0.0.1.tar.gz` & `tmp/muben-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muben-0.0.1.tar", last modified: Thu Feb 29 16:38:46 2024, max compression
+gzip compressed data, was "muben-0.0.2.tar", last modified: Wed Apr 17 16:22:52 2024, max compression
```

## Comparing `muben-0.0.1.tar` & `muben-0.0.2.tar`

### file list

```diff
@@ -1,126 +1,127 @@
-drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-02-29 16:38:46.963407 muben-0.0.1/
--rw-r--r--   0 yli       (1000) yli       (1000)    11357 2024-02-29 16:24:46.000000 muben-0.0.1/LICENSE
--rw-r--r--   0 yli       (1000) yli       (1000)    15115 2024-02-29 16:38:46.963407 muben-0.0.1/PKG-INFO
--rw-r--r--   0 yli       (1000) yli       (1000)    14371 2024-02-29 16:24:46.000000 muben-0.0.1/README.md
-drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-02-29 16:38:46.963407 muben-0.0.1/muben/
--rw-r--r--   0 yli       (1000) yli       (1000)        0 2024-02-29 16:24:46.000000 muben-0.0.1/muben/__init__.py
-drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-02-29 16:38:46.963407 muben-0.0.1/muben/args/
--rw-r--r--   0 yli       (1000) yli       (1000)      674 2024-02-29 16:24:46.000000 muben-0.0.1/muben/args/__init__.py
--rw-r--r--   0 yli       (1000) yli       (1000)    22530 2024-02-29 16:24:46.000000 muben-0.0.1/muben/args/args.py
--rw-r--r--   0 yli       (1000) yli       (1000)     1652 2024-02-29 16:24:46.000000 muben-0.0.1/muben/args/args_2d.py
--rw-r--r--   0 yli       (1000) yli       (1000)     2298 2024-02-29 16:24:46.000000 muben-0.0.1/muben/args/args_3d.py
--rw-r--r--   0 yli       (1000) yli       (1000)     2756 2024-02-29 16:24:46.000000 muben-0.0.1/muben/args/args_grover.py
--rw-r--r--   0 yli       (1000) yli       (1000)      918 2024-02-29 16:24:46.000000 muben-0.0.1/muben/args/args_linear.py
--rw-r--r--   0 yli       (1000) yli       (1000)     2000 2024-02-29 16:24:46.000000 muben-0.0.1/muben/args/args_rdkit.py
--rw-r--r--   0 yli       (1000) yli       (1000)     4861 2024-02-29 16:24:46.000000 muben-0.0.1/muben/args/args_unimol.py
-drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-02-29 16:38:46.963407 muben-0.0.1/muben/dataset/
--rw-r--r--   0 yli       (1000) yli       (1000)      683 2024-02-29 16:24:46.000000 muben-0.0.1/muben/dataset/__init__.py
--rw-r--r--   0 yli       (1000) yli       (1000)    11415 2024-02-29 16:24:46.000000 muben-0.0.1/muben/dataset/dataset.py
-drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-02-29 16:38:46.963407 muben-0.0.1/muben/dataset/dataset_2d/
--rw-r--r--   0 yli       (1000) yli       (1000)      102 2024-02-29 16:24:46.000000 muben-0.0.1/muben/dataset/dataset_2d/__init__.py
--rw-r--r--   0 yli       (1000) yli       (1000)     1838 2024-02-29 16:24:46.000000 muben-0.0.1/muben/dataset/dataset_2d/collate.py
--rw-r--r--   0 yli       (1000) yli       (1000)     2176 2024-02-29 16:24:46.000000 muben-0.0.1/muben/dataset/dataset_2d/dataset.py
-drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-02-29 16:38:46.963407 muben-0.0.1/muben/dataset/dataset_3d/
--rw-r--r--   0 yli       (1000) yli       (1000)      102 2024-02-29 16:24:46.000000 muben-0.0.1/muben/dataset/dataset_3d/__init__.py
--rw-r--r--   0 yli       (1000) yli       (1000)     2531 2024-02-29 16:24:46.000000 muben-0.0.1/muben/dataset/dataset_3d/collate.py
--rw-r--r--   0 yli       (1000) yli       (1000)     4596 2024-02-29 16:24:46.000000 muben-0.0.1/muben/dataset/dataset_3d/dataset.py
-drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-02-29 16:38:46.963407 muben-0.0.1/muben/dataset/dataset_grover/
--rw-r--r--   0 yli       (1000) yli       (1000)      171 2024-02-29 16:24:46.000000 muben-0.0.1/muben/dataset/dataset_grover/__init__.py
--rw-r--r--   0 yli       (1000) yli       (1000)     2233 2024-02-29 16:24:46.000000 muben-0.0.1/muben/dataset/dataset_grover/collate.py
--rw-r--r--   0 yli       (1000) yli       (1000)     2593 2024-02-29 16:24:46.000000 muben-0.0.1/muben/dataset/dataset_grover/dataset.py
--rw-r--r--   0 yli       (1000) yli       (1000)    12702 2024-02-29 16:24:46.000000 muben-0.0.1/muben/dataset/dataset_grover/molgraph.py
-drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-02-29 16:38:46.963407 muben-0.0.1/muben/dataset/dataset_linear/
--rw-r--r--   0 yli       (1000) yli       (1000)      118 2024-02-29 16:24:46.000000 muben-0.0.1/muben/dataset/dataset_linear/__init__.py
--rw-r--r--   0 yli       (1000) yli       (1000)     2545 2024-02-29 16:24:46.000000 muben-0.0.1/muben/dataset/dataset_linear/collate.py
--rw-r--r--   0 yli       (1000) yli       (1000)     2057 2024-02-29 16:24:46.000000 muben-0.0.1/muben/dataset/dataset_linear/dataset.py
-drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-02-29 16:38:46.963407 muben-0.0.1/muben/dataset/dataset_rdkit/
--rw-r--r--   0 yli       (1000) yli       (1000)      114 2024-02-29 16:24:46.000000 muben-0.0.1/muben/dataset/dataset_rdkit/__init__.py
--rw-r--r--   0 yli       (1000) yli       (1000)     1607 2024-02-29 16:24:46.000000 muben-0.0.1/muben/dataset/dataset_rdkit/collate.py
--rw-r--r--   0 yli       (1000) yli       (1000)     3413 2024-02-29 16:24:46.000000 muben-0.0.1/muben/dataset/dataset_rdkit/dataset.py
-drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-02-29 16:38:46.963407 muben-0.0.1/muben/dataset/dataset_unimol/
--rw-r--r--   0 yli       (1000) yli       (1000)      179 2024-02-29 16:24:46.000000 muben-0.0.1/muben/dataset/dataset_unimol/__init__.py
--rw-r--r--   0 yli       (1000) yli       (1000)     3361 2024-02-29 16:24:46.000000 muben-0.0.1/muben/dataset/dataset_unimol/collate.py
--rw-r--r--   0 yli       (1000) yli       (1000)     5872 2024-02-29 16:24:46.000000 muben-0.0.1/muben/dataset/dataset_unimol/dataset.py
--rw-r--r--   0 yli       (1000) yli       (1000)     5124 2024-02-29 16:24:46.000000 muben-0.0.1/muben/dataset/dataset_unimol/dictionary.py
--rw-r--r--   0 yli       (1000) yli       (1000)    11657 2024-02-29 16:24:46.000000 muben-0.0.1/muben/dataset/dataset_unimol/process.py
-drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-02-29 16:38:46.963407 muben-0.0.1/muben/layers/
--rw-r--r--   0 yli       (1000) yli       (1000)       60 2024-02-29 16:24:46.000000 muben-0.0.1/muben/layers/__init__.py
--rw-r--r--   0 yli       (1000) yli       (1000)     3707 2024-02-29 16:24:46.000000 muben-0.0.1/muben/layers/layers.py
-drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-02-29 16:38:46.963407 muben-0.0.1/muben/model/
--rw-r--r--   0 yli       (1000) yli       (1000)      433 2024-02-29 16:24:46.000000 muben-0.0.1/muben/model/__init__.py
-drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-02-29 16:38:46.963407 muben-0.0.1/muben/model/dnn/
--rw-r--r--   0 yli       (1000) yli       (1000)       47 2024-02-29 16:24:46.000000 muben-0.0.1/muben/model/dnn/__init__.py
--rw-r--r--   0 yli       (1000) yli       (1000)     4263 2024-02-29 16:24:46.000000 muben-0.0.1/muben/model/dnn/dnn.py
-drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-02-29 16:38:46.963407 muben-0.0.1/muben/model/gin/
--rw-r--r--   0 yli       (1000) yli       (1000)       40 2024-02-29 16:24:46.000000 muben-0.0.1/muben/model/gin/__init__.py
--rw-r--r--   0 yli       (1000) yli       (1000)     3091 2024-02-29 16:24:46.000000 muben-0.0.1/muben/model/gin/gin.py
-drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-02-29 16:38:46.963407 muben-0.0.1/muben/model/grover/
--rw-r--r--   0 yli       (1000) yli       (1000)      119 2024-02-29 16:24:46.000000 muben-0.0.1/muben/model/grover/__init__.py
--rw-r--r--   0 yli       (1000) yli       (1000)    34312 2024-02-29 16:24:46.000000 muben-0.0.1/muben/model/grover/layers.py
--rw-r--r--   0 yli       (1000) yli       (1000)     8779 2024-02-29 16:24:46.000000 muben-0.0.1/muben/model/grover/model.py
--rw-r--r--   0 yli       (1000) yli       (1000)     1387 2024-02-29 16:24:46.000000 muben-0.0.1/muben/model/grover/ts.py
--rw-r--r--   0 yli       (1000) yli       (1000)     3620 2024-02-29 16:24:46.000000 muben-0.0.1/muben/model/grover/utils.py
-drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-02-29 16:38:46.963407 muben-0.0.1/muben/model/linear_transformer/
--rw-r--r--   0 yli       (1000) yli       (1000)       90 2024-02-29 16:24:46.000000 muben-0.0.1/muben/model/linear_transformer/__init__.py
--rw-r--r--   0 yli       (1000) yli       (1000)     2915 2024-02-29 16:24:46.000000 muben-0.0.1/muben/model/linear_transformer/linear_transformer.py
-drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-02-29 16:38:46.963407 muben-0.0.1/muben/model/torchmdnet/
--rw-r--r--   0 yli       (1000) yli       (1000)      307 2024-02-29 16:24:46.000000 muben-0.0.1/muben/model/torchmdnet/__init__.py
--rw-r--r--   0 yli       (1000) yli       (1000)    21436 2024-02-29 16:24:46.000000 muben-0.0.1/muben/model/torchmdnet/et.py
--rw-r--r--   0 yli       (1000) yli       (1000)     3650 2024-02-29 16:24:46.000000 muben-0.0.1/muben/model/torchmdnet/layers.py
--rw-r--r--   0 yli       (1000) yli       (1000)    14045 2024-02-29 16:24:46.000000 muben-0.0.1/muben/model/torchmdnet/modules.py
--rw-r--r--   0 yli       (1000) yli       (1000)     4806 2024-02-29 16:24:46.000000 muben-0.0.1/muben/model/torchmdnet/torchmdnet.py
-drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-02-29 16:38:46.963407 muben-0.0.1/muben/model/unimol/
--rw-r--r--   0 yli       (1000) yli       (1000)       50 2024-02-29 16:24:46.000000 muben-0.0.1/muben/model/unimol/__init__.py
--rw-r--r--   0 yli       (1000) yli       (1000)     5091 2024-02-29 16:24:46.000000 muben-0.0.1/muben/model/unimol/encoder.py
-drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-02-29 16:38:46.963407 muben-0.0.1/muben/model/unimol/layers/
--rw-r--r--   0 yli       (1000) yli       (1000)      356 2024-02-29 16:24:46.000000 muben-0.0.1/muben/model/unimol/layers/__init__.py
--rw-r--r--   0 yli       (1000) yli       (1000)     2495 2024-02-29 16:24:46.000000 muben-0.0.1/muben/model/unimol/layers/layer_norm.py
--rw-r--r--   0 yli       (1000) yli       (1000)     7202 2024-02-29 16:24:46.000000 muben-0.0.1/muben/model/unimol/layers/multihead_attention.py
--rw-r--r--   0 yli       (1000) yli       (1000)     1112 2024-02-29 16:24:46.000000 muben-0.0.1/muben/model/unimol/layers/softmax_dropout.py
--rw-r--r--   0 yli       (1000) yli       (1000)     6006 2024-02-29 16:24:46.000000 muben-0.0.1/muben/model/unimol/layers/transformer_encoder.py
--rw-r--r--   0 yli       (1000) yli       (1000)     3103 2024-02-29 16:24:46.000000 muben-0.0.1/muben/model/unimol/layers/transformer_encoder_layer.py
--rw-r--r--   0 yli       (1000) yli       (1000)     2738 2024-02-29 16:24:46.000000 muben-0.0.1/muben/model/unimol/layers/utils.py
--rw-r--r--   0 yli       (1000) yli       (1000)     5920 2024-02-29 16:24:46.000000 muben-0.0.1/muben/model/unimol/module.py
--rw-r--r--   0 yli       (1000) yli       (1000)     5502 2024-02-29 16:24:46.000000 muben-0.0.1/muben/model/unimol/unimol.py
-drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-02-29 16:38:46.963407 muben-0.0.1/muben/train/
--rw-r--r--   0 yli       (1000) yli       (1000)      193 2024-02-29 16:24:46.000000 muben-0.0.1/muben/train/__init__.py
-drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-02-29 16:38:46.963407 muben-0.0.1/muben/train/trainer/
--rw-r--r--   0 yli       (1000) yli       (1000)      240 2024-02-29 16:24:46.000000 muben-0.0.1/muben/train/trainer/__init__.py
--rw-r--r--   0 yli       (1000) yli       (1000)     4615 2024-02-29 16:24:46.000000 muben-0.0.1/muben/train/trainer/container.py
--rw-r--r--   0 yli       (1000) yli       (1000)     2081 2024-02-29 16:24:46.000000 muben-0.0.1/muben/train/trainer/loss.py
--rw-r--r--   0 yli       (1000) yli       (1000)     4331 2024-02-29 16:24:46.000000 muben-0.0.1/muben/train/trainer/metric.py
--rw-r--r--   0 yli       (1000) yli       (1000)     3738 2024-02-29 16:24:46.000000 muben-0.0.1/muben/train/trainer/scaler.py
--rw-r--r--   0 yli       (1000) yli       (1000)     3004 2024-02-29 16:24:46.000000 muben-0.0.1/muben/train/trainer/state.py
--rw-r--r--   0 yli       (1000) yli       (1000)     3395 2024-02-29 16:24:46.000000 muben-0.0.1/muben/train/trainer/timer.py
--rw-r--r--   0 yli       (1000) yli       (1000)    56774 2024-02-29 16:24:46.000000 muben-0.0.1/muben/train/trainer/trainer.py
--rw-r--r--   0 yli       (1000) yli       (1000)     7562 2024-02-29 16:24:46.000000 muben-0.0.1/muben/train/trainer_grover.py
--rw-r--r--   0 yli       (1000) yli       (1000)     4235 2024-02-29 16:24:46.000000 muben-0.0.1/muben/train/trainer_unimol.py
-drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-02-29 16:38:46.963407 muben-0.0.1/muben/uncertainty/
--rw-r--r--   0 yli       (1000) yli       (1000)      601 2024-02-29 16:24:46.000000 muben-0.0.1/muben/uncertainty/__init__.py
--rw-r--r--   0 yli       (1000) yli       (1000)     4484 2024-02-29 16:24:46.000000 muben-0.0.1/muben/uncertainty/bbp.py
-drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-02-29 16:38:46.963407 muben-0.0.1/muben/uncertainty/evidential/
--rw-r--r--   0 yli       (1000) yli       (1000)      208 2024-02-29 16:24:46.000000 muben-0.0.1/muben/uncertainty/evidential/__init__.py
--rw-r--r--   0 yli       (1000) yli       (1000)     3559 2024-02-29 16:24:46.000000 muben-0.0.1/muben/uncertainty/evidential/loss.py
--rw-r--r--   0 yli       (1000) yli       (1000)     1036 2024-02-29 16:24:46.000000 muben-0.0.1/muben/uncertainty/evidential/model.py
--rw-r--r--   0 yli       (1000) yli       (1000)     1987 2024-02-29 16:24:46.000000 muben-0.0.1/muben/uncertainty/focal_loss.py
--rw-r--r--   0 yli       (1000) yli       (1000)     9830 2024-02-29 16:24:46.000000 muben-0.0.1/muben/uncertainty/iso.py
--rw-r--r--   0 yli       (1000) yli       (1000)     5867 2024-02-29 16:24:46.000000 muben-0.0.1/muben/uncertainty/sgld.py
--rw-r--r--   0 yli       (1000) yli       (1000)     8130 2024-02-29 16:24:46.000000 muben-0.0.1/muben/uncertainty/swag.py
--rw-r--r--   0 yli       (1000) yli       (1000)     2201 2024-02-29 16:24:46.000000 muben-0.0.1/muben/uncertainty/ts.py
-drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-02-29 16:38:46.963407 muben-0.0.1/muben/utils/
--rw-r--r--   0 yli       (1000) yli       (1000)        0 2024-02-29 16:24:46.000000 muben-0.0.1/muben/utils/__init__.py
--rw-r--r--   0 yli       (1000) yli       (1000)    17389 2024-02-29 16:24:46.000000 muben-0.0.1/muben/utils/argparser.py
--rw-r--r--   0 yli       (1000) yli       (1000)     8480 2024-02-29 16:24:46.000000 muben-0.0.1/muben/utils/chem.py
--rw-r--r--   0 yli       (1000) yli       (1000)    10449 2024-02-29 16:24:46.000000 muben-0.0.1/muben/utils/io.py
--rw-r--r--   0 yli       (1000) yli       (1000)     5893 2024-02-29 16:24:46.000000 muben-0.0.1/muben/utils/macro.py
--rw-r--r--   0 yli       (1000) yli       (1000)     8075 2024-02-29 16:24:46.000000 muben-0.0.1/muben/utils/metrics.py
--rw-r--r--   0 yli       (1000) yli       (1000)     2638 2024-02-29 16:24:46.000000 muben-0.0.1/muben/utils/selectors.py
-drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-02-29 16:38:46.963407 muben-0.0.1/muben.egg-info/
--rw-r--r--   0 yli       (1000) yli       (1000)    15115 2024-02-29 16:38:46.000000 muben-0.0.1/muben.egg-info/PKG-INFO
--rw-r--r--   0 yli       (1000) yli       (1000)     3061 2024-02-29 16:38:46.000000 muben-0.0.1/muben.egg-info/SOURCES.txt
--rw-r--r--   0 yli       (1000) yli       (1000)        1 2024-02-29 16:38:46.000000 muben-0.0.1/muben.egg-info/dependency_links.txt
--rw-r--r--   0 yli       (1000) yli       (1000)        1 2024-02-29 16:33:45.000000 muben-0.0.1/muben.egg-info/not-zip-safe
--rw-r--r--   0 yli       (1000) yli       (1000)        6 2024-02-29 16:38:46.000000 muben-0.0.1/muben.egg-info/top_level.txt
--rw-r--r--   0 yli       (1000) yli       (1000)       85 2024-02-29 16:26:49.000000 muben-0.0.1/pyproject.toml
--rw-r--r--   0 yli       (1000) yli       (1000)       38 2024-02-29 16:38:46.963407 muben-0.0.1/setup.cfg
--rw-r--r--   0 yli       (1000) yli       (1000)     1010 2024-02-29 16:38:40.000000 muben-0.0.1/setup.py
+drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-04-17 16:22:52.841419 muben-0.0.2/
+-rw-r--r--   0 yli       (1000) yli       (1000)    11357 2024-03-17 02:09:15.000000 muben-0.0.2/LICENSE
+-rw-r--r--   0 yli       (1000) yli       (1000)    14852 2024-04-17 16:22:52.841419 muben-0.0.2/PKG-INFO
+-rw-r--r--   0 yli       (1000) yli       (1000)    14108 2024-04-17 14:56:15.000000 muben-0.0.2/README.md
+drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-04-17 16:22:52.831419 muben-0.0.2/muben/
+-rw-r--r--   0 yli       (1000) yli       (1000)        0 2024-03-17 02:09:15.000000 muben-0.0.2/muben/__init__.py
+drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-04-17 16:22:52.831419 muben-0.0.2/muben/args/
+-rw-r--r--   0 yli       (1000) yli       (1000)      674 2024-03-17 02:09:15.000000 muben-0.0.2/muben/args/__init__.py
+-rw-r--r--   0 yli       (1000) yli       (1000)    32811 2024-04-17 14:56:15.000000 muben-0.0.2/muben/args/args.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     1652 2024-03-17 02:09:15.000000 muben-0.0.2/muben/args/args_2d.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     2298 2024-03-17 02:09:15.000000 muben-0.0.2/muben/args/args_3d.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     2756 2024-03-17 02:09:15.000000 muben-0.0.2/muben/args/args_grover.py
+-rw-r--r--   0 yli       (1000) yli       (1000)      918 2024-03-17 02:09:15.000000 muben-0.0.2/muben/args/args_linear.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     2000 2024-03-17 02:09:15.000000 muben-0.0.2/muben/args/args_rdkit.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     4861 2024-03-17 02:09:15.000000 muben-0.0.2/muben/args/args_unimol.py
+drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-04-17 16:22:52.831419 muben-0.0.2/muben/dataset/
+-rw-r--r--   0 yli       (1000) yli       (1000)      683 2024-03-17 02:09:15.000000 muben-0.0.2/muben/dataset/__init__.py
+-rw-r--r--   0 yli       (1000) yli       (1000)    15841 2024-04-17 14:56:15.000000 muben-0.0.2/muben/dataset/dataset.py
+drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-04-17 16:22:52.831419 muben-0.0.2/muben/dataset/dataset_2d/
+-rw-r--r--   0 yli       (1000) yli       (1000)      102 2024-03-17 02:09:15.000000 muben-0.0.2/muben/dataset/dataset_2d/__init__.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     1838 2024-03-17 02:09:15.000000 muben-0.0.2/muben/dataset/dataset_2d/collate.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     2176 2024-03-17 02:09:15.000000 muben-0.0.2/muben/dataset/dataset_2d/dataset.py
+drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-04-17 16:22:52.831419 muben-0.0.2/muben/dataset/dataset_3d/
+-rw-r--r--   0 yli       (1000) yli       (1000)      102 2024-03-17 02:09:15.000000 muben-0.0.2/muben/dataset/dataset_3d/__init__.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     2531 2024-03-17 02:09:15.000000 muben-0.0.2/muben/dataset/dataset_3d/collate.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     4596 2024-03-17 02:09:15.000000 muben-0.0.2/muben/dataset/dataset_3d/dataset.py
+drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-04-17 16:22:52.831419 muben-0.0.2/muben/dataset/dataset_grover/
+-rw-r--r--   0 yli       (1000) yli       (1000)      171 2024-03-17 02:09:15.000000 muben-0.0.2/muben/dataset/dataset_grover/__init__.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     2233 2024-03-17 02:09:15.000000 muben-0.0.2/muben/dataset/dataset_grover/collate.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     2593 2024-03-17 02:09:15.000000 muben-0.0.2/muben/dataset/dataset_grover/dataset.py
+-rw-r--r--   0 yli       (1000) yli       (1000)    12702 2024-03-17 02:09:15.000000 muben-0.0.2/muben/dataset/dataset_grover/molgraph.py
+drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-04-17 16:22:52.831419 muben-0.0.2/muben/dataset/dataset_linear/
+-rw-r--r--   0 yli       (1000) yli       (1000)      118 2024-03-17 02:09:15.000000 muben-0.0.2/muben/dataset/dataset_linear/__init__.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     2545 2024-03-17 02:09:15.000000 muben-0.0.2/muben/dataset/dataset_linear/collate.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     2057 2024-03-17 02:09:15.000000 muben-0.0.2/muben/dataset/dataset_linear/dataset.py
+drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-04-17 16:22:52.831419 muben-0.0.2/muben/dataset/dataset_rdkit/
+-rw-r--r--   0 yli       (1000) yli       (1000)      114 2024-03-17 02:09:15.000000 muben-0.0.2/muben/dataset/dataset_rdkit/__init__.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     1607 2024-03-17 02:09:15.000000 muben-0.0.2/muben/dataset/dataset_rdkit/collate.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     3413 2024-03-17 02:09:15.000000 muben-0.0.2/muben/dataset/dataset_rdkit/dataset.py
+drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-04-17 16:22:52.831419 muben-0.0.2/muben/dataset/dataset_unimol/
+-rw-r--r--   0 yli       (1000) yli       (1000)      179 2024-03-17 02:09:15.000000 muben-0.0.2/muben/dataset/dataset_unimol/__init__.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     3361 2024-03-17 02:09:15.000000 muben-0.0.2/muben/dataset/dataset_unimol/collate.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     6249 2024-04-17 14:56:15.000000 muben-0.0.2/muben/dataset/dataset_unimol/dataset.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     5124 2024-03-17 02:09:15.000000 muben-0.0.2/muben/dataset/dataset_unimol/dictionary.py
+-rw-r--r--   0 yli       (1000) yli       (1000)    11657 2024-03-17 02:09:15.000000 muben-0.0.2/muben/dataset/dataset_unimol/process.py
+drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-04-17 16:22:52.831419 muben-0.0.2/muben/layers/
+-rw-r--r--   0 yli       (1000) yli       (1000)       60 2024-03-17 02:09:15.000000 muben-0.0.2/muben/layers/__init__.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     4805 2024-03-17 02:09:15.000000 muben-0.0.2/muben/layers/layers.py
+drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-04-17 16:22:52.831419 muben-0.0.2/muben/model/
+-rw-r--r--   0 yli       (1000) yli       (1000)      433 2024-03-17 02:09:15.000000 muben-0.0.2/muben/model/__init__.py
+drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-04-17 16:22:52.831419 muben-0.0.2/muben/model/dnn/
+-rw-r--r--   0 yli       (1000) yli       (1000)       47 2024-03-17 02:09:15.000000 muben-0.0.2/muben/model/dnn/__init__.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     4263 2024-03-17 02:09:15.000000 muben-0.0.2/muben/model/dnn/dnn.py
+drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-04-17 16:22:52.831419 muben-0.0.2/muben/model/gin/
+-rw-r--r--   0 yli       (1000) yli       (1000)       40 2024-03-17 02:09:15.000000 muben-0.0.2/muben/model/gin/__init__.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     3091 2024-03-17 02:09:15.000000 muben-0.0.2/muben/model/gin/gin.py
+drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-04-17 16:22:52.831419 muben-0.0.2/muben/model/grover/
+-rw-r--r--   0 yli       (1000) yli       (1000)      119 2024-03-17 02:09:15.000000 muben-0.0.2/muben/model/grover/__init__.py
+-rw-r--r--   0 yli       (1000) yli       (1000)    34312 2024-03-17 02:09:15.000000 muben-0.0.2/muben/model/grover/layers.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     8910 2024-03-17 02:09:15.000000 muben-0.0.2/muben/model/grover/model.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     1387 2024-03-17 02:09:15.000000 muben-0.0.2/muben/model/grover/ts.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     3620 2024-03-17 02:09:15.000000 muben-0.0.2/muben/model/grover/utils.py
+drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-04-17 16:22:52.831419 muben-0.0.2/muben/model/linear_transformer/
+-rw-r--r--   0 yli       (1000) yli       (1000)       90 2024-03-17 02:09:15.000000 muben-0.0.2/muben/model/linear_transformer/__init__.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     2915 2024-03-17 02:09:15.000000 muben-0.0.2/muben/model/linear_transformer/linear_transformer.py
+drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-04-17 16:22:52.831419 muben-0.0.2/muben/model/torchmdnet/
+-rw-r--r--   0 yli       (1000) yli       (1000)      307 2024-03-17 02:09:15.000000 muben-0.0.2/muben/model/torchmdnet/__init__.py
+-rw-r--r--   0 yli       (1000) yli       (1000)    21436 2024-03-17 02:09:15.000000 muben-0.0.2/muben/model/torchmdnet/et.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     3650 2024-03-17 02:09:15.000000 muben-0.0.2/muben/model/torchmdnet/layers.py
+-rw-r--r--   0 yli       (1000) yli       (1000)    14045 2024-03-17 02:09:15.000000 muben-0.0.2/muben/model/torchmdnet/modules.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     4806 2024-03-17 02:09:15.000000 muben-0.0.2/muben/model/torchmdnet/torchmdnet.py
+drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-04-17 16:22:52.831419 muben-0.0.2/muben/model/unimol/
+-rw-r--r--   0 yli       (1000) yli       (1000)       50 2024-03-17 02:09:15.000000 muben-0.0.2/muben/model/unimol/__init__.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     5091 2024-03-17 02:09:15.000000 muben-0.0.2/muben/model/unimol/encoder.py
+drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-04-17 16:22:52.831419 muben-0.0.2/muben/model/unimol/layers/
+-rw-r--r--   0 yli       (1000) yli       (1000)      356 2024-03-17 02:09:15.000000 muben-0.0.2/muben/model/unimol/layers/__init__.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     2495 2024-03-17 02:09:15.000000 muben-0.0.2/muben/model/unimol/layers/layer_norm.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     7202 2024-03-17 02:09:15.000000 muben-0.0.2/muben/model/unimol/layers/multihead_attention.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     1112 2024-03-17 02:09:15.000000 muben-0.0.2/muben/model/unimol/layers/softmax_dropout.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     6006 2024-03-17 02:09:15.000000 muben-0.0.2/muben/model/unimol/layers/transformer_encoder.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     3103 2024-03-17 02:09:15.000000 muben-0.0.2/muben/model/unimol/layers/transformer_encoder_layer.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     2738 2024-03-17 02:09:15.000000 muben-0.0.2/muben/model/unimol/layers/utils.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     5920 2024-03-17 02:09:15.000000 muben-0.0.2/muben/model/unimol/module.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     5556 2024-03-17 02:09:15.000000 muben-0.0.2/muben/model/unimol/unimol.py
+drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-04-17 16:22:52.831419 muben-0.0.2/muben/train/
+-rw-r--r--   0 yli       (1000) yli       (1000)      193 2024-03-17 02:09:15.000000 muben-0.0.2/muben/train/__init__.py
+drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-04-17 16:22:52.831419 muben-0.0.2/muben/train/trainer/
+-rw-r--r--   0 yli       (1000) yli       (1000)      240 2024-03-17 02:09:15.000000 muben-0.0.2/muben/train/trainer/__init__.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     4615 2024-03-17 02:09:15.000000 muben-0.0.2/muben/train/trainer/container.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     2081 2024-03-17 02:09:15.000000 muben-0.0.2/muben/train/trainer/loss.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     4331 2024-03-17 02:09:15.000000 muben-0.0.2/muben/train/trainer/metric.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     3738 2024-03-17 02:09:15.000000 muben-0.0.2/muben/train/trainer/scaler.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     3004 2024-03-17 02:09:15.000000 muben-0.0.2/muben/train/trainer/state.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     3395 2024-03-17 02:09:15.000000 muben-0.0.2/muben/train/trainer/timer.py
+-rw-r--r--   0 yli       (1000) yli       (1000)    57977 2024-04-17 14:56:15.000000 muben-0.0.2/muben/train/trainer/trainer.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     7562 2024-03-17 02:09:15.000000 muben-0.0.2/muben/train/trainer_grover.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     4248 2024-03-17 02:09:15.000000 muben-0.0.2/muben/train/trainer_unimol.py
+drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-04-17 16:22:52.841419 muben-0.0.2/muben/uncertainty/
+-rw-r--r--   0 yli       (1000) yli       (1000)      601 2024-03-17 02:09:15.000000 muben-0.0.2/muben/uncertainty/__init__.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     4484 2024-03-17 02:09:15.000000 muben-0.0.2/muben/uncertainty/bbp.py
+drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-04-17 16:22:52.841419 muben-0.0.2/muben/uncertainty/evidential/
+-rw-r--r--   0 yli       (1000) yli       (1000)      208 2024-03-17 02:09:15.000000 muben-0.0.2/muben/uncertainty/evidential/__init__.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     3559 2024-03-17 02:09:15.000000 muben-0.0.2/muben/uncertainty/evidential/loss.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     1036 2024-03-17 02:09:15.000000 muben-0.0.2/muben/uncertainty/evidential/model.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     1987 2024-03-17 02:09:15.000000 muben-0.0.2/muben/uncertainty/focal_loss.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     9830 2024-03-17 02:09:15.000000 muben-0.0.2/muben/uncertainty/iso.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     5867 2024-03-17 02:09:15.000000 muben-0.0.2/muben/uncertainty/sgld.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     8130 2024-03-17 02:09:15.000000 muben-0.0.2/muben/uncertainty/swag.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     2201 2024-03-17 02:09:15.000000 muben-0.0.2/muben/uncertainty/ts.py
+drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-04-17 16:22:52.841419 muben-0.0.2/muben/utils/
+-rw-r--r--   0 yli       (1000) yli       (1000)        0 2024-03-17 02:09:15.000000 muben-0.0.2/muben/utils/__init__.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     8758 2024-03-17 02:09:15.000000 muben-0.0.2/muben/utils/chem.py
+-rw-r--r--   0 yli       (1000) yli       (1000)    11476 2024-04-17 16:07:17.000000 muben-0.0.2/muben/utils/io.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     5890 2024-04-17 14:56:15.000000 muben-0.0.2/muben/utils/macro.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     8695 2024-03-17 02:09:15.000000 muben-0.0.2/muben/utils/metrics.py
+-rw-r--r--   0 yli       (1000) yli       (1000)     3910 2024-03-17 02:09:15.000000 muben-0.0.2/muben/utils/selectors.py
+drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-04-17 16:22:52.841419 muben-0.0.2/muben.egg-info/
+-rw-r--r--   0 yli       (1000) yli       (1000)    14852 2024-04-17 16:22:52.000000 muben-0.0.2/muben.egg-info/PKG-INFO
+-rw-r--r--   0 yli       (1000) yli       (1000)     3049 2024-04-17 16:22:52.000000 muben-0.0.2/muben.egg-info/SOURCES.txt
+-rw-r--r--   0 yli       (1000) yli       (1000)        1 2024-04-17 16:22:52.000000 muben-0.0.2/muben.egg-info/dependency_links.txt
+-rw-r--r--   0 yli       (1000) yli       (1000)        1 2024-04-17 16:22:52.000000 muben-0.0.2/muben.egg-info/not-zip-safe
+-rw-r--r--   0 yli       (1000) yli       (1000)        6 2024-04-17 16:22:52.000000 muben-0.0.2/muben.egg-info/top_level.txt
+-rw-r--r--   0 yli       (1000) yli       (1000)       85 2024-03-17 02:09:15.000000 muben-0.0.2/pyproject.toml
+-rw-r--r--   0 yli       (1000) yli       (1000)       38 2024-04-17 16:22:52.841419 muben-0.0.2/setup.cfg
+-rw-r--r--   0 yli       (1000) yli       (1000)     1010 2024-04-17 16:22:16.000000 muben-0.0.2/setup.py
+drwxr-xr-x   0 yli       (1000) yli       (1000)        0 2024-04-17 16:22:52.841419 muben-0.0.2/test/
+-rw-r--r--   0 yli       (1000) yli       (1000)     9284 2024-02-29 18:56:17.000000 muben-0.0.2/test/test.py
```

### Comparing `muben-0.0.1/LICENSE` & `muben-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/PKG-INFO` & `muben-0.0.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,247 +1,216 @@
-Metadata-Version: 2.1
-Name: muben
-Version: 0.0.1
-Summary: Benchmark for molecular uncertainty estimation.
-Home-page: https://github.com/Yinghao-Li/MUBen
-Author: Yinghao Li
-Author-email: yinghaoli@gatech.edu
-License: MIT
-Keywords: machine-learning uncertainty-estimation materials-science materials-property-prediction
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Text Processing
-Classifier: Topic :: Text Processing :: Linguistic
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # MUBen: **M**olecular **U**ncertainty **Ben**mark
-Code associated with paper *MUBen: Benchmarking the Uncertainty of Pre-Trained Models for Molecular Property Prediction*.
+Code associated with paper *MUBen: **Ben**chmarking the **U**ncertainty of **M**olecular Representation Models*.
+
+[![Documentation](https://img.shields.io/badge/%F0%9F%93%96%20Documentation-Link-blue)](https://yinghao-li.github.io/MUBen/)
+[![OpenReview](https://img.shields.io/badge/%F0%9F%94%97%20OpenReview-TMLR-darkred)](https://openreview.net/forum?id=qYceFeHgm4)
+[![arXiv](https://img.shields.io/badge/arXiv-2306.10060-b31b1b.svg)](https://arxiv.org/abs/2306.10060)
+[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/Yinghao-Li/MUBen/)
+[![PyPI version](https://badge.fury.io/py/muben.svg)](https://badge.fury.io/py/muben)
 
-The code is built to expose implementation details as much as possible and be easily extendable.
-Questions and suggestions are welcome if you find any issues while using our code.
+Please visit [📕 Documentation](https://yinghao-li.github.io/MUBen/) for the full documentation of this project, which contains more comprehensive API introductions and examples.
+
+![](./figures/f1.summarization.png)
 
-## 0. ABOUT
 
 MUBen is a benchmark that aims to investigate the performance of uncertainty quantification (UQ) methods built upon backbone molecular representation models.
 It implements 6 backbone models (4 pre-trained and 2 non-pre-trained), 8 UQ methods (8 compatible for classification and 6 for regression), and 14 datasets from [MoleculeNet](https://moleculenet.org/) (8 for classification and 6 for regression).
-We are actively expanding the benchmark to include more backbones, UQ methods and datasets.
+We are actively expanding the benchmark to include more backbones, UQ methods, and datasets.
 This is an arduous task, and we welcome contribution or collaboration in any form.
 
-### Backbones
-| Backbone Models      | Paper | Official Repo | Our Implementation|
-| ----------- | ----------- | ----------- | ----------- |
-|*Pre-Trained Backbones* |||
-| ChemBERTa |[link](https://arxiv.org/abs/2209.01712) | [link](https://github.com/seyonechithrananda/bert-loves-chemistry) | [link](https://github.com/Yinghao-Li/UncertaintyBenchmark/tree/main/muben/chemberta) | 
-| GROVER   | [link](https://arxiv.org/abs/2007.02835) | [link](https://github.com/tencent-ailab/grover)| [link](https://github.com/Yinghao-Li/UncertaintyBenchmark/tree/main/muben/grover)|
-|Uni-Mol| [link](https://openreview.net/forum?id=6K2RM6wVqKu) | [link](https://github.com/dptech-corp/Uni-Mol/tree/main/unimol) | [link](https://github.com/Yinghao-Li/UncertaintyBenchmark/tree/main/muben/unimol)|
-|TorchMD-NET | [Architecture](https://arxiv.org/abs/2202.02541); [Pre-training](https://arxiv.org/abs/2206.00133) | [link](https://github.com/shehzaidi/pre-training-via-denoising) | [link](https://github.com/Yinghao-Li/UncertaintyBenchmark/tree/main/muben/torchmdnet)|
-| *Non-Pre-Trained Backbones* |||
-|DNN|-|-|[link](https://github.com/Yinghao-Li/UncertaintyBenchmark/tree/main/muben/dnn)|
-|GIN| [link](https://arxiv.org/pdf/1810.00826.pdf) | [pyg](https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.nn.models.GIN.html) | [link](https://github.com/Yinghao-Li/UncertaintyBenchmark/tree/main/muben/gin)|
+## Backbones
 
-### Uncertainty Quantification Methods
+| Backbone Models      | Paper | Official Repo |
+| ----------- | ----------- | ----------- |
+|***Pre-Trained*** |||
+| ChemBERTa |[link](https://arxiv.org/abs/2209.01712) | [link](https://github.com/seyonechithrananda/bert-loves-chemistry) | 
+| GROVER   | [link](https://arxiv.org/abs/2007.02835) | [link](https://github.com/tencent-ailab/grover)|
+|Uni-Mol| [link](https://openreview.net/forum?id=6K2RM6wVqKu) | [link](https://github.com/dptech-corp/Uni-Mol/tree/main/unimol) |
+|TorchMD-NET | [Architecture](https://arxiv.org/abs/2202.02541); [Pre-training](https://arxiv.org/abs/2206.00133) | [link](https://github.com/shehzaidi/pre-training-via-denoising) |
+| ***Trained from Scratch*** |||
+|DNN|-|-|
+|GIN| [link](https://arxiv.org/pdf/1810.00826.pdf) | [pyg](https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.nn.models.GIN.html) |
+
+
+## Uncertainty Quantification Methods
 | UQ Method | Classification | Regression | Paper |
 | ----------- | ----------- | ----------- | ----------- |
-| *Included* |||
+| ***Included in Paper*** |||
 | Deterministic | ✅︎ | ✅︎ | - |
 | Temperature Scaling | ✅︎ | - | [link](https://arxiv.org/abs/1706.04599) |
 | Focal Loss | ✅︎ | - | [link](https://arxiv.org/abs/1708.02002) |
 | Deep Ensembles | ✅︎ | ✅︎ | [link](https://arxiv.org/abs/1612.01474) |
 | SWAG | ✅︎ | ✅︎ | [link](https://arxiv.org/abs/1808.05326) |
 | Bayes by Backprop | ✅︎ | ✅︎ | [link](https://arxiv.org/abs/1505.05424) |
 | SGLD | ✅︎ | ✅︎ | [link](https://www.stats.ox.ac.uk/~teh/research/compstats/WelTeh2011a.pdf) |
 | MC Dropout | ✅︎ | ✅︎ | [link](https://arxiv.org/abs/1506.02142) |
+| ***Additional in Repo*** |||
+| Evidential Networks |✅︎|✅︎|[link](https://openreview.net/forum?id=xqS8k9E75c)|
+| Conformal Prediction |-|✅︎| [link](https://arxiv.org/abs/2107.07511) |
+| Isotonic Calibration| - | ✅︎ | [link](https://arxiv.org/abs/1905.06023)|
 
-### Data
+## Data
 
-Please check [MoleculeNet](https://moleculenet.org/datasets-1) for a detailed description.
-We use a subset of the MoleculeNet benckmark, including BBBP, Tox21, ToxCast, SIDER, ClinTox, BACE, MUV, HIV, ESOL, FreeSolv, Lipophilicity, QM7, QM8, QM9.
+> The prepared scaffold-split data is available in the [./data/files/](https://github.com/Yinghao-Li/UncertaintyBenchmark/tree/main/data/files) directory.
 
-## 1. DATA
+This documentation utilizes a selection from the MoleculeNet benchmark, which includes datasets such as BBBP, Tox21, ToxCast, SIDER, ClinTox, BACE, MUV, HIV, ESOL, FreeSolv, Lipophilicity, QM7, QM8, and QM9.
+For detailed descriptions of these datasets, please refer to the [MoleculeNet website](https://moleculenet.org/datasets-1).
 
-> A set of partitioned datasets are already included in this repo. You can find them under the `./data/` folder: [[scaffold split](https://github.com/Yinghao-Li/UncertaintyBenchmark/tree/main/data/files)]; [[random split](https://github.com/Yinghao-Li/UncertaintyBenchmark/tree/main/data/files-random)].
+We employ the "molecular property" datasets curated by [Uni-Mol](https://github.com/dptech-corp/Uni-Mol/tree/main/unimol), which are accessible for download [here](https://bioos-hermite-beijing.tos-cn-beijing.volces.com/unimol_data/finetune/molecular_property_prediction.tar.gz).
+While the original Uni-Mol dataset is generally not necessary, it is used to provide pre-defined molecule conformations for running the Uni-Mol model.
+To use the Uni-Mol data, download and unzip the files into the `./data/UniMol/` directory.
+For ease of reference, you are suggested to rename the `qm7dft`, `qm8dft`, and `qm9dft` directories to `qm7`, `qm8`, and `qm9`, respectively.
+The conversion of the dataset format from Uni-Mol to our specifications can be viewed in the script [dataset_build_from_unimol.py](https://github.com/Yinghao-Li/MUBen/blob/main/assist/dataset_build_from_unimol.py).
 
-We utilize the datasets prepared by [Uni-Mol](https://github.com/dptech-corp/Uni-Mol/tree/main/unimol).
-You find the data [here](https://github.com/dptech-corp/Uni-Mol/tree/main/unimol#:~:text=pockets.tar.gz-,molecular%20property,-3.506GB) or directly download it through [this link](https://bioos-hermite-beijing.tos-cn-beijing.volces.com/unimol_data/finetune/molecular_property_prediction.tar.gz).
-We place the unzipped files into `./data/UniMol` by default.
-For convenience, you are suggested to rename the `qm7dft`, `qm8dft`, and `qm9dft` folders to `qm7`, `qm8`, and `qm9`.
-
-Afterwards, you can transfer the dataset format into ours by running
-```bash
-PYTHONPATH="." python ./assist/dataset_build_from_unimol.py
-``` 
-suppose you are in the project root directory.
-You can specify the input (Uni-Mol) and output data directories with `--unimol_data_dir` and `--output_dir` arguments.
-The script will convert *all* datasets by default (excluding PCBA).
-If you want to specify a subset of datasets, you can specify the argument `--dataset_names` with the target dataset names with lowercase letters.
+Typically, each dataset comprises 4 files: `train.csv`, `valid.csv`, `test.csv`, and `meta.json`.
+The `.csv` files partition the data into training, validation, and testing sets, while `meta.json` contains metadata such as task type (classification or regression), number of tasks, and number of classes (for classification tasks).
+Each `.csv` file contains three columns:
+- `smiles`: A string representing the SMILES notation of a molecule.
+- `labels`: A list of integers or floats representing the property values to be predicted for each molecule. The length of the list corresponds to the number of tasks.
+- `masks`: A binary list (containing 0s and 1s) where 1 indicates a valid property value and 0 indicates an invalid value to be ignored during training and testing.
 
-**Notice**: If you would like to run the Uni-Mol model, you are suggested to keep the original `UniMol` data as we will use the pre-defined molecule conformations.
-Otherwise, it is safe to remove the original data.
+The dataset is automatically loaded during training through the method `muben.dataset.Dataset.prepare()`.
+For a practical example, visit the [example](./train.python.md) page.
 
-### Other Options
+## Environment Setup
 
-If you do not want to use Uni-Mol data, you can try the scripts within the `legacy` folder, including `build_dgllife_datasets.py`, and `build_qm[7,8,9]_dataset.py`.
-Notice that this may result in training/validation/test partitions different from what is being used in our experiments.
+Our code is developed with `Python 3.10`, and does **not** work with `Python < 3.9`.
 
-### Using Customized Datasets
+### Installation
 
-If you want to test the UQ methods on your own dataset, you can use `pandas.DataFrame` structure with the following keys:
-```
-{
-  "smiles": list of `str`,
-  "labels": list of list of int/float,
-  "masks": list of list of int/float (with values within {0,1})
-}
+MUBen is available as a Python package on [PyPI](https://pypi.org/project/muben/) and can be installed using pip.
+If you prefer to use MUBen as a standalone package and do not need to modify the source code, you can simply run:
+```bash
+pip install muben
 ```
-and store them as `train.csv`, `valid.csv`, and `test.csv` files.
-`mask=1` indicates the existence informative label at the position and `mask=0` indicates missing label.
-You can check the prepared datasets included in our program for reference.
-You are recommended to put the dataset files in the `./data/file/<dataset name>` directory, but you can of course choose your favorite location and specify the `--data_folder` argument.
-
-The `.csv` files should be accompanied by a `meta.json` file within the same directory.
-It stores some constant dataset properties, *e.g.*, `task_type` (classification or regression), `n_tasks`, or `classes` (`[0,1]` for all our classification datasets).
-For the customized dataset, one **required** property is the `eval_metric` for validation and test (*e.g.*, roc-auc, rmse, *etc.*) since it is not specified in the macro file.
-Please refer to `./assist/dataset_build_roe.py` for an example (unfortunately, we are not allowed to release the dataset).
-
-## 2. REQUIREMENTS
 
-Please find the required packages in `requirements.txt`.
-Our code is developed with `Python 3.10` and does not work with Python versions earlier than `3.9`.
-It is recommended to create a new `conda` environment with
+To download the source code and datasets, you can fork the project on GitHub and clone your fork, or directly clone the original repository:
 
 ```bash
-conda create --name <env_name> --file requirements.txt
+# Clone your fork of the repository
+git clone https://github.com/<your GitHub username>/MUBen.git
+
+# Or clone the original repository with git
+git clone https://github.com/Yinghao-Li/MUBen.git --single-branch --branch main
 ```
 
-### Docker
-Alternatively, you can run this project in a docker container.
-You can build your image through
+
+### Anaconda
+
+Suppose you have anaconda or miniconda installed in your local machine, you can create a new `conda` environment for this project using `conda create`.
 ```bash
-docker build -t muben ./docker
+conda create -n muben python=3.10
 ```
-and run your container in an interactive shell with
+
+The required packages are listed in `requirements.txt`.
+It is recommended to install these dependencies with `pip install` as `conda install` may sometimes encounter dependency resolution issue.
 ```bash
-docker run --gpus all -it --rm  muben
+conda activate muben
+pip install -r requirements.txt
 ```
 
-### External Dependencies
+### Backbone Checkpoints
 
-The backbone models `GROVER` and `Uni-Mol` require loading pre-trained model checkpoints.
+Some backbone models require loading pre-trained model checkpoints.
 
+- For ChemBERTa, we use the `DeepChem/ChemBERTa-77M-MLM` checkpoint hosted on Hugging Face's [Model Hub](https://huggingface.co/models). You can specify the model name to the argument `--pretrained_model_name_or_path` (which is set to default), or you can download the model and pass the path to the model to the argument.
 - The `GROVER-base` checkpoint is available at GROVER's [project repo](https://github.com/tencent-ailab/grover) or can be directly downloaded through [this link](https://ai.tencent.com/ailab/ml/ml-data/grover-models/pretrain/grover_base.tar.gz).
 Unzip the downloaded `.tar.gz` file to get the `.pt` checkpoint.
 - The `Uni-Mol` checkpoint is available at Uni-Mol's [project repo](https://github.com/dptech-corp/Uni-Mol/tree/main/unimol) or can be directly downloaded through [this link](https://github.com/dptech-corp/Uni-Mol/releases/download/v0.1/mol_pre_no_h_220816.pt).
+- The `TorchMD-NET` checkpoint is available at this [project repo](https://github.com/shehzaidi/pre-training-via-denoising) or can be directly downloaded through [this link](https://github.com/shehzaidi/pre-training-via-denoising/raw/main/checkpoints/denoised-pcqm4mv2.ckpt).
 
-By default, the code will look for the models at locations `./models/grover_base.pt` and `./models/unimol_base.pt`, respectively.
-You need to specify the `--checkpoint_path` argument if you prefer other locations and checkpoint names.
 
-## 3. RUN
+## Fine-Tuning the Models
 
-> A simple demo of running our project can be found at `./demo/demo.ipynb`.
+> Please visit [this Documentation page](https://yinghao-li.github.io/MUBen/train.python/) for a guideline of using the `muben` package, or [this Documentation page](https://yinghao-li.github.io/MUBen/customize/) for an instruction about incorporating customized datasets or backbone models.
 
-To run each of the four backbone models with uncertainty estimation methods, you can check the `run_*.py` files in the root directory.
-Example shell scripts are provided in the `./scripts` folder as `.sh` files.
-You can use them through
-```bash
-./scripts/run_dnn_rdkit.sh <CUDA_VISIBLE_DEVICES>
-```
-as an example.
-Notice that we need to comment out the variables `train_on_<dataset name>` in the `.sh` files to skip training on the corresponding datasets.
-Setting their value to `false` **does not work**.
+The [./run/](https://github.com/Yinghao-Li/MUBen/tree/main/run) directory contains the entry scripts to fine-tuning each of the backbone-UQ combinations.
+Currently, the script [./run/run.py](https://github.com/Yinghao-Li/MUBen/blob/main/run/run.py) is adopted to run all backbone models except for GROVER and Uni-Mol, whose entry scripts are [./run/grover.py](https://github.com/Yinghao-Li/MUBen/blob/main/run/grover.py) and [./run/unimol.py](https://github.com/Yinghao-Li/MUBen/blob/main/run/unimol.py), respectively.
 
-Another way of specifying arguments is through the `.json` scripts, for example:
-```bash
-PYTHONPATH="." CUDA_VISIBLE_DEVICES=0 python ./run/dnn.py ./scripts/config_dnn.json
-```
-This approach could be helpful for debugging the code through vscode.
+### Specify Arguments Using Command Lines
 
-To get a detailed description of each argument, you can use `--help`:
+An example of running the **DNN** model with **RDKit** features with the **MC Dropout** UQ method on the **BBBP** dataset is
 ```bash
-PYTHONPATH="." python ./run/dnn.py --help
+CUDA_VISIBLE_DEVICES=0 \
+PYTHONPATH="." \
+python ./run/run.py \
+    --descriptor_type "RDKit" \
+    --data_folder "./data/files" \
+    --dataset_name "bbbp" \
+    --uncertainty_method "MCDropout" \
+    --lr 0.0001 \
+    --n_epochs 200 \
+    --batch_size 256 \
+    --seed 0
 ```
+In the example, the `--descriptor_type` argument is used to select the backbone models used in our experiments.
+It has 4 options: {"RDKit", "Linear", "2D", "3D"}, which corresponds to the DNN, ChemBERTa, GIN and TorchMD-NET backbone models in the CLI, respectively.
+In the future versions, we may consider including multiple backbone models that correspond to one descriptor, which requires us to specify the `--model_name` argument to separate the backbones.
+But currently, we do not need to worry about that and can leave `--model_name` as default.
 
-### Logging and WandB
+> For the interpretation of each argument, please check the [`muben.args` API](./muben.args.md) or directly refer to the [code implementation](https://github.com/Yinghao-Li/MUBen/tree/main/muben/args).
+> Notice that the API documentation may not be entirely comprehensive.
 
-By default, this project uses local logging files (`*.log`) and [WandB](https://wandb.ai/site) to track training status.
-
-The log files are stored as `./logs/<dataset>/<model>/<uncertainty>/<running_time>.log`.
-You can change the file path by specifying the `--log_path` argument, or disable log saving by setting `--log_path="disabled"`.
-
-To use WandB, you first need to register an account and sign in on your machine with `wandb login`.
-If you are running your code on a public device, you can instead use program-wise signing in by specifying the `--wandb_api_key` argument while running our code.
-You can find your API key in your browser here: https://wandb.ai/authorize.
-To disable WandB, use `--disable_wandb [true]`.
-By default, we use `MUBen-<dataset>` as WandB project name and `<model>-<uncertainty>` as the model name.
-You can change this behavior by specifying the `--wandb_project` and `--wandb_name` arguments.
-
-### Data Loading
+To run GROVER or Uni-Mol, we just need to replace `run.py` by the corresponding script, and slightly modify the arguments:
+```bash
+CUDA_VISIBLE_DEVICES=0 \
+PYTHONPATH="." \
+python ./run/unimol.py \
+    --data_folder "./data/files" \
+    --unimol_feature_folder "./data/UniMol/" \
+    --dataset_name "esol" \
+    --checkpoint_path "./models/unimol_base.pt" \
+    --uncertainty_method "MCDropout" \
+    --regression_with_variance \
+    ...
+```
+> For regression tasks, the argument `--regression_with_variance` is vital to guarantee a valid result with predicted variance.
 
-The progress will automatically create the necessary features (molecular descriptors) required by backbone models from the SMILES strings if they are loaded properly.
-The processed features are stored in the `<bottom-level data folder>/processed/` directory as `<train/valid/test>.pt` files by default, and will be automatically loaded the next time you apply the same backbone model on the same dataset.
-You can change this behavior with `--disable_dataset_saving` for disabling dataset saving or `--ignore_preprocessed_dataset` for not loading from the saved (processed) dataset.
+### Specify Arguments using `.yaml` Files
 
-Constructing Morgan fingerprint, RDKit features or 3D conformations for Uni-Mol may take a while.
-You can accelerate this process by utilizing multiple threads `--num_preprocess_workers=n>1` (default is 8).
-For 3D conformations, we directly take advantage of the results from Uni-Mol but still keep the choice of generating them by ourselves if the Uni-Mol data files are not found.
+Another way of specifying arguments is through the `.yaml` scripts, which provides more readable data structure than `.json` files.
+We have provided an [example configuration script](https://github.com/Yinghao-Li/MUBen/blob/main/scripts/config-example.yaml) within the [./scripts/](https://github.com/Yinghao-Li/MUBen/tree/main/scripts) directory, which runs GIN on the FreeSolv dataset with deterministic ("none") UQ method.
+To use it to specify arguments, we can run the python program with
+```bash
+PYTHONPATH="." CUDA_VISIBLE_DEVICES=0 python ./run/run.py ./scripts/config-example.yaml
+```
+This approach could be helpful while debugging the code on VSCode.
 
-### Calculating Metrics
+## Calculating Metrics
 
 During training, we only calculate metrics necessary for early stopping and simple prediction performance evaluation.
 To get other metrics, you need to use the `./assist/results_get_metrics.py` file.
 
-Specifically, you need to save the model predictions by **not** setting `--disable_dataset_saving`.
-The results are saved as `./<result_folder>/<dataset_name>/<model_name>/<uncertainty_method>/seed-<seed>/preds/<test_idx>.pt` files.
-When the training is finished, you can run the `./assist/results_get_metrics.py` file to generate all metrics for your model predictions.
+After training, the results are saved as `./<result_folder>/<dataset_name>/<model_name>/<uncertainty_method>/seed-<seed>/preds/<test_idx>.pt` files.
+You can run the `./assist/results_get_metrics.py` file to generate all metrics for your model predictions.
 For example:
 ```bash
-PYTHONPATH="." python ./assist/results_get_metrics.py ./scripts/config_metrics.json
+PYTHONPATH="." python ./assist/results_get_metrics.py [arguments]
 ```
-Make sure the hyper-parameters in the configuration file are updated to your needs.
-
-The metrics will be saved in the `./<result_folder>/RESULTS/<model_name>-<dataset_name>.csv` files.
-~~Notice that these files already exist in the repo if you keep the default `--result_folder=./output` argument and you need to check whether it is updated to reveal your experiment results.~~
+Make sure the arguments are updated to your needs.
 
-### Results
 
-We provided a more comprehensive copy of our experiment results [here](https://github.com/Yinghao-Li/UncertaintyBenchmark/tree/main/output) that are presented in the tables in our paper's appendix.
-We hope it can ease some effort if you want to further analyze the behavior of our backbone models and uncertainty quantification methods. 
+## Experimental Results
 
-## 4. ONGOING WORKS
+We have made our experimental results available in the [./reports/](https://github.com/Yinghao-Li/MUBen/tree/main/reports) directory.
+These results are organized into different folders based on the nature of the experiments:
 
-### 4.1. Active Learning
+- `primary`: Contains the most comprehensive set of results derived from experiments on scaffold-split datasets.
+- `random`: Includes results from experiments conducted on datasets that were split randomly.
+- `frozen`: Features results from experiments where the pre-trained model's weights were frozen, except for the last output layer, which was updatable.
+- `distribution`: Offers results from the QM9 dataset, where the test set was categorized into five bins based on the average Tanimoto similarities to the training scaffolds.
 
-We are developing code to integrate *active learning* into the pipeline.
-Specifically, we assume we have a small set of labeled data points (`--n_init_instances`) at the beginning.
-Within each active learning iteration, we use the labeled dataset to fine-tune the model parameters and select a batch of data points (`--n_al_select`) from the unlabeled set with the least predicted certainty (*i.e.*, max predicted entropy for classification and max predicted variance for regression).
-The process is repeated for several loops (`--n_al_loops`), and the intermediate performance is tracked.
+Files within these directories are named following the pattern `<backbone>-<dataset>.csv`.
+Each file provides a comparison of different UQ methods.
+The rows detail the performance of each UQ method, while the columns display the mean and standard deviation from three random runs for each metric.
 
-The code is still under construction and currently is **only available under the `dev` branch**.
-In addition, several points are worth attention:
-
-- Currently, only DNN and ChemBERTa backbones are supported (`./run/dnn_al.py` and `./run/chemberta_al.py`). Migrating AL to other backbones is not difficult but requires updating some Trainer functions if they are reloaded.
-- To enable active learning, make sure you set `--enable_active_learning` to `true`.
-- Currently, Deep Ensembles is not supported for AL.
-- We cannot guarantee the correctness of our implementation. If you notice any abnormalities in the code, please do not hesitate to post an issue.
-
-One example is
-```bash
-python ./run/dnn_al.py \
-  --enable_active_learning \
-  --n_init_instances 100 \
-  --n_al_loops 20 \
-  --n_al_select 20 \
-  # other model and training hyper-parameters...
-```
+Additional post-processing scripts can be found in the [./assist/](https://github.com/Yinghao-Li/MUBen/tree/main/assist) directory, which include files starting with `plot_` or `results_`.
+These scripts are useful for further analysis and visualization of the experimental data.
 
-## 5. CITATION
+## Citation
 
 If you find our work helpful, please consider citing it as
 ```latex
 @misc{li2023muben,
     title={MUBen: Benchmarking the Uncertainty of Pre-Trained Models for Molecular Property Prediction},
     author={Yinghao Li and Lingkai Kong and Yuanqi Du and Yue Yu and Yuchen Zhuang and Wenhao Mu and Chao Zhang},
     year={2023},
```

### Comparing `muben-0.0.1/README.md` & `muben-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,227 +1,236 @@
+Metadata-Version: 2.1
+Name: muben
+Version: 0.0.2
+Summary: Benchmark for molecular uncertainty estimation.
+Home-page: https://github.com/Yinghao-Li/MUBen
+Author: Yinghao Li
+Author-email: yinghaoli@gatech.edu
+License: MIT
+Keywords: machine-learning uncertainty-estimation materials-science materials-property-prediction
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Text Processing
+Classifier: Topic :: Text Processing :: Linguistic
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # MUBen: **M**olecular **U**ncertainty **Ben**mark
-Code associated with paper *MUBen: Benchmarking the Uncertainty of Pre-Trained Models for Molecular Property Prediction*.
+Code associated with paper *MUBen: **Ben**chmarking the **U**ncertainty of **M**olecular Representation Models*.
+
+[![Documentation](https://img.shields.io/badge/%F0%9F%93%96%20Documentation-Link-blue)](https://yinghao-li.github.io/MUBen/)
+[![OpenReview](https://img.shields.io/badge/%F0%9F%94%97%20OpenReview-TMLR-darkred)](https://openreview.net/forum?id=qYceFeHgm4)
+[![arXiv](https://img.shields.io/badge/arXiv-2306.10060-b31b1b.svg)](https://arxiv.org/abs/2306.10060)
+[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/Yinghao-Li/MUBen/)
+[![PyPI version](https://badge.fury.io/py/muben.svg)](https://badge.fury.io/py/muben)
 
-The code is built to expose implementation details as much as possible and be easily extendable.
-Questions and suggestions are welcome if you find any issues while using our code.
+Please visit [📕 Documentation](https://yinghao-li.github.io/MUBen/) for the full documentation of this project, which contains more comprehensive API introductions and examples.
+
+![](./figures/f1.summarization.png)
 
-## 0. ABOUT
 
 MUBen is a benchmark that aims to investigate the performance of uncertainty quantification (UQ) methods built upon backbone molecular representation models.
 It implements 6 backbone models (4 pre-trained and 2 non-pre-trained), 8 UQ methods (8 compatible for classification and 6 for regression), and 14 datasets from [MoleculeNet](https://moleculenet.org/) (8 for classification and 6 for regression).
-We are actively expanding the benchmark to include more backbones, UQ methods and datasets.
+We are actively expanding the benchmark to include more backbones, UQ methods, and datasets.
 This is an arduous task, and we welcome contribution or collaboration in any form.
 
-### Backbones
-| Backbone Models      | Paper | Official Repo | Our Implementation|
-| ----------- | ----------- | ----------- | ----------- |
-|*Pre-Trained Backbones* |||
-| ChemBERTa |[link](https://arxiv.org/abs/2209.01712) | [link](https://github.com/seyonechithrananda/bert-loves-chemistry) | [link](https://github.com/Yinghao-Li/UncertaintyBenchmark/tree/main/muben/chemberta) | 
-| GROVER   | [link](https://arxiv.org/abs/2007.02835) | [link](https://github.com/tencent-ailab/grover)| [link](https://github.com/Yinghao-Li/UncertaintyBenchmark/tree/main/muben/grover)|
-|Uni-Mol| [link](https://openreview.net/forum?id=6K2RM6wVqKu) | [link](https://github.com/dptech-corp/Uni-Mol/tree/main/unimol) | [link](https://github.com/Yinghao-Li/UncertaintyBenchmark/tree/main/muben/unimol)|
-|TorchMD-NET | [Architecture](https://arxiv.org/abs/2202.02541); [Pre-training](https://arxiv.org/abs/2206.00133) | [link](https://github.com/shehzaidi/pre-training-via-denoising) | [link](https://github.com/Yinghao-Li/UncertaintyBenchmark/tree/main/muben/torchmdnet)|
-| *Non-Pre-Trained Backbones* |||
-|DNN|-|-|[link](https://github.com/Yinghao-Li/UncertaintyBenchmark/tree/main/muben/dnn)|
-|GIN| [link](https://arxiv.org/pdf/1810.00826.pdf) | [pyg](https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.nn.models.GIN.html) | [link](https://github.com/Yinghao-Li/UncertaintyBenchmark/tree/main/muben/gin)|
+## Backbones
 
-### Uncertainty Quantification Methods
+| Backbone Models      | Paper | Official Repo |
+| ----------- | ----------- | ----------- |
+|***Pre-Trained*** |||
+| ChemBERTa |[link](https://arxiv.org/abs/2209.01712) | [link](https://github.com/seyonechithrananda/bert-loves-chemistry) | 
+| GROVER   | [link](https://arxiv.org/abs/2007.02835) | [link](https://github.com/tencent-ailab/grover)|
+|Uni-Mol| [link](https://openreview.net/forum?id=6K2RM6wVqKu) | [link](https://github.com/dptech-corp/Uni-Mol/tree/main/unimol) |
+|TorchMD-NET | [Architecture](https://arxiv.org/abs/2202.02541); [Pre-training](https://arxiv.org/abs/2206.00133) | [link](https://github.com/shehzaidi/pre-training-via-denoising) |
+| ***Trained from Scratch*** |||
+|DNN|-|-|
+|GIN| [link](https://arxiv.org/pdf/1810.00826.pdf) | [pyg](https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.nn.models.GIN.html) |
+
+
+## Uncertainty Quantification Methods
 | UQ Method | Classification | Regression | Paper |
 | ----------- | ----------- | ----------- | ----------- |
-| *Included* |||
+| ***Included in Paper*** |||
 | Deterministic | ✅︎ | ✅︎ | - |
 | Temperature Scaling | ✅︎ | - | [link](https://arxiv.org/abs/1706.04599) |
 | Focal Loss | ✅︎ | - | [link](https://arxiv.org/abs/1708.02002) |
 | Deep Ensembles | ✅︎ | ✅︎ | [link](https://arxiv.org/abs/1612.01474) |
 | SWAG | ✅︎ | ✅︎ | [link](https://arxiv.org/abs/1808.05326) |
 | Bayes by Backprop | ✅︎ | ✅︎ | [link](https://arxiv.org/abs/1505.05424) |
 | SGLD | ✅︎ | ✅︎ | [link](https://www.stats.ox.ac.uk/~teh/research/compstats/WelTeh2011a.pdf) |
 | MC Dropout | ✅︎ | ✅︎ | [link](https://arxiv.org/abs/1506.02142) |
+| ***Additional in Repo*** |||
+| Evidential Networks |✅︎|✅︎|[link](https://openreview.net/forum?id=xqS8k9E75c)|
+| Conformal Prediction |-|✅︎| [link](https://arxiv.org/abs/2107.07511) |
+| Isotonic Calibration| - | ✅︎ | [link](https://arxiv.org/abs/1905.06023)|
 
-### Data
+## Data
 
-Please check [MoleculeNet](https://moleculenet.org/datasets-1) for a detailed description.
-We use a subset of the MoleculeNet benckmark, including BBBP, Tox21, ToxCast, SIDER, ClinTox, BACE, MUV, HIV, ESOL, FreeSolv, Lipophilicity, QM7, QM8, QM9.
+> The prepared scaffold-split data is available in the [./data/files/](https://github.com/Yinghao-Li/UncertaintyBenchmark/tree/main/data/files) directory.
 
-## 1. DATA
+This documentation utilizes a selection from the MoleculeNet benchmark, which includes datasets such as BBBP, Tox21, ToxCast, SIDER, ClinTox, BACE, MUV, HIV, ESOL, FreeSolv, Lipophilicity, QM7, QM8, and QM9.
+For detailed descriptions of these datasets, please refer to the [MoleculeNet website](https://moleculenet.org/datasets-1).
 
-> A set of partitioned datasets are already included in this repo. You can find them under the `./data/` folder: [[scaffold split](https://github.com/Yinghao-Li/UncertaintyBenchmark/tree/main/data/files)]; [[random split](https://github.com/Yinghao-Li/UncertaintyBenchmark/tree/main/data/files-random)].
+We employ the "molecular property" datasets curated by [Uni-Mol](https://github.com/dptech-corp/Uni-Mol/tree/main/unimol), which are accessible for download [here](https://bioos-hermite-beijing.tos-cn-beijing.volces.com/unimol_data/finetune/molecular_property_prediction.tar.gz).
+While the original Uni-Mol dataset is generally not necessary, it is used to provide pre-defined molecule conformations for running the Uni-Mol model.
+To use the Uni-Mol data, download and unzip the files into the `./data/UniMol/` directory.
+For ease of reference, you are suggested to rename the `qm7dft`, `qm8dft`, and `qm9dft` directories to `qm7`, `qm8`, and `qm9`, respectively.
+The conversion of the dataset format from Uni-Mol to our specifications can be viewed in the script [dataset_build_from_unimol.py](https://github.com/Yinghao-Li/MUBen/blob/main/assist/dataset_build_from_unimol.py).
 
-We utilize the datasets prepared by [Uni-Mol](https://github.com/dptech-corp/Uni-Mol/tree/main/unimol).
-You find the data [here](https://github.com/dptech-corp/Uni-Mol/tree/main/unimol#:~:text=pockets.tar.gz-,molecular%20property,-3.506GB) or directly download it through [this link](https://bioos-hermite-beijing.tos-cn-beijing.volces.com/unimol_data/finetune/molecular_property_prediction.tar.gz).
-We place the unzipped files into `./data/UniMol` by default.
-For convenience, you are suggested to rename the `qm7dft`, `qm8dft`, and `qm9dft` folders to `qm7`, `qm8`, and `qm9`.
-
-Afterwards, you can transfer the dataset format into ours by running
-```bash
-PYTHONPATH="." python ./assist/dataset_build_from_unimol.py
-``` 
-suppose you are in the project root directory.
-You can specify the input (Uni-Mol) and output data directories with `--unimol_data_dir` and `--output_dir` arguments.
-The script will convert *all* datasets by default (excluding PCBA).
-If you want to specify a subset of datasets, you can specify the argument `--dataset_names` with the target dataset names with lowercase letters.
+Typically, each dataset comprises 4 files: `train.csv`, `valid.csv`, `test.csv`, and `meta.json`.
+The `.csv` files partition the data into training, validation, and testing sets, while `meta.json` contains metadata such as task type (classification or regression), number of tasks, and number of classes (for classification tasks).
+Each `.csv` file contains three columns:
+- `smiles`: A string representing the SMILES notation of a molecule.
+- `labels`: A list of integers or floats representing the property values to be predicted for each molecule. The length of the list corresponds to the number of tasks.
+- `masks`: A binary list (containing 0s and 1s) where 1 indicates a valid property value and 0 indicates an invalid value to be ignored during training and testing.
 
-**Notice**: If you would like to run the Uni-Mol model, you are suggested to keep the original `UniMol` data as we will use the pre-defined molecule conformations.
-Otherwise, it is safe to remove the original data.
+The dataset is automatically loaded during training through the method `muben.dataset.Dataset.prepare()`.
+For a practical example, visit the [example](./train.python.md) page.
 
-### Other Options
+## Environment Setup
 
-If you do not want to use Uni-Mol data, you can try the scripts within the `legacy` folder, including `build_dgllife_datasets.py`, and `build_qm[7,8,9]_dataset.py`.
-Notice that this may result in training/validation/test partitions different from what is being used in our experiments.
+Our code is developed with `Python 3.10`, and does **not** work with `Python < 3.9`.
 
-### Using Customized Datasets
+### Installation
 
-If you want to test the UQ methods on your own dataset, you can use `pandas.DataFrame` structure with the following keys:
-```
-{
-  "smiles": list of `str`,
-  "labels": list of list of int/float,
-  "masks": list of list of int/float (with values within {0,1})
-}
+MUBen is available as a Python package on [PyPI](https://pypi.org/project/muben/) and can be installed using pip.
+If you prefer to use MUBen as a standalone package and do not need to modify the source code, you can simply run:
+```bash
+pip install muben
 ```
-and store them as `train.csv`, `valid.csv`, and `test.csv` files.
-`mask=1` indicates the existence informative label at the position and `mask=0` indicates missing label.
-You can check the prepared datasets included in our program for reference.
-You are recommended to put the dataset files in the `./data/file/<dataset name>` directory, but you can of course choose your favorite location and specify the `--data_folder` argument.
-
-The `.csv` files should be accompanied by a `meta.json` file within the same directory.
-It stores some constant dataset properties, *e.g.*, `task_type` (classification or regression), `n_tasks`, or `classes` (`[0,1]` for all our classification datasets).
-For the customized dataset, one **required** property is the `eval_metric` for validation and test (*e.g.*, roc-auc, rmse, *etc.*) since it is not specified in the macro file.
-Please refer to `./assist/dataset_build_roe.py` for an example (unfortunately, we are not allowed to release the dataset).
-
-## 2. REQUIREMENTS
 
-Please find the required packages in `requirements.txt`.
-Our code is developed with `Python 3.10` and does not work with Python versions earlier than `3.9`.
-It is recommended to create a new `conda` environment with
+To download the source code and datasets, you can fork the project on GitHub and clone your fork, or directly clone the original repository:
 
 ```bash
-conda create --name <env_name> --file requirements.txt
+# Clone your fork of the repository
+git clone https://github.com/<your GitHub username>/MUBen.git
+
+# Or clone the original repository with git
+git clone https://github.com/Yinghao-Li/MUBen.git --single-branch --branch main
 ```
 
-### Docker
-Alternatively, you can run this project in a docker container.
-You can build your image through
+
+### Anaconda
+
+Suppose you have anaconda or miniconda installed in your local machine, you can create a new `conda` environment for this project using `conda create`.
 ```bash
-docker build -t muben ./docker
+conda create -n muben python=3.10
 ```
-and run your container in an interactive shell with
+
+The required packages are listed in `requirements.txt`.
+It is recommended to install these dependencies with `pip install` as `conda install` may sometimes encounter dependency resolution issue.
 ```bash
-docker run --gpus all -it --rm  muben
+conda activate muben
+pip install -r requirements.txt
 ```
 
-### External Dependencies
+### Backbone Checkpoints
 
-The backbone models `GROVER` and `Uni-Mol` require loading pre-trained model checkpoints.
+Some backbone models require loading pre-trained model checkpoints.
 
+- For ChemBERTa, we use the `DeepChem/ChemBERTa-77M-MLM` checkpoint hosted on Hugging Face's [Model Hub](https://huggingface.co/models). You can specify the model name to the argument `--pretrained_model_name_or_path` (which is set to default), or you can download the model and pass the path to the model to the argument.
 - The `GROVER-base` checkpoint is available at GROVER's [project repo](https://github.com/tencent-ailab/grover) or can be directly downloaded through [this link](https://ai.tencent.com/ailab/ml/ml-data/grover-models/pretrain/grover_base.tar.gz).
 Unzip the downloaded `.tar.gz` file to get the `.pt` checkpoint.
 - The `Uni-Mol` checkpoint is available at Uni-Mol's [project repo](https://github.com/dptech-corp/Uni-Mol/tree/main/unimol) or can be directly downloaded through [this link](https://github.com/dptech-corp/Uni-Mol/releases/download/v0.1/mol_pre_no_h_220816.pt).
+- The `TorchMD-NET` checkpoint is available at this [project repo](https://github.com/shehzaidi/pre-training-via-denoising) or can be directly downloaded through [this link](https://github.com/shehzaidi/pre-training-via-denoising/raw/main/checkpoints/denoised-pcqm4mv2.ckpt).
 
-By default, the code will look for the models at locations `./models/grover_base.pt` and `./models/unimol_base.pt`, respectively.
-You need to specify the `--checkpoint_path` argument if you prefer other locations and checkpoint names.
 
-## 3. RUN
+## Fine-Tuning the Models
 
-> A simple demo of running our project can be found at `./demo/demo.ipynb`.
+> Please visit [this Documentation page](https://yinghao-li.github.io/MUBen/train.python/) for a guideline of using the `muben` package, or [this Documentation page](https://yinghao-li.github.io/MUBen/customize/) for an instruction about incorporating customized datasets or backbone models.
 
-To run each of the four backbone models with uncertainty estimation methods, you can check the `run_*.py` files in the root directory.
-Example shell scripts are provided in the `./scripts` folder as `.sh` files.
-You can use them through
-```bash
-./scripts/run_dnn_rdkit.sh <CUDA_VISIBLE_DEVICES>
-```
-as an example.
-Notice that we need to comment out the variables `train_on_<dataset name>` in the `.sh` files to skip training on the corresponding datasets.
-Setting their value to `false` **does not work**.
+The [./run/](https://github.com/Yinghao-Li/MUBen/tree/main/run) directory contains the entry scripts to fine-tuning each of the backbone-UQ combinations.
+Currently, the script [./run/run.py](https://github.com/Yinghao-Li/MUBen/blob/main/run/run.py) is adopted to run all backbone models except for GROVER and Uni-Mol, whose entry scripts are [./run/grover.py](https://github.com/Yinghao-Li/MUBen/blob/main/run/grover.py) and [./run/unimol.py](https://github.com/Yinghao-Li/MUBen/blob/main/run/unimol.py), respectively.
 
-Another way of specifying arguments is through the `.json` scripts, for example:
-```bash
-PYTHONPATH="." CUDA_VISIBLE_DEVICES=0 python ./run/dnn.py ./scripts/config_dnn.json
-```
-This approach could be helpful for debugging the code through vscode.
+### Specify Arguments Using Command Lines
 
-To get a detailed description of each argument, you can use `--help`:
+An example of running the **DNN** model with **RDKit** features with the **MC Dropout** UQ method on the **BBBP** dataset is
 ```bash
-PYTHONPATH="." python ./run/dnn.py --help
+CUDA_VISIBLE_DEVICES=0 \
+PYTHONPATH="." \
+python ./run/run.py \
+    --descriptor_type "RDKit" \
+    --data_folder "./data/files" \
+    --dataset_name "bbbp" \
+    --uncertainty_method "MCDropout" \
+    --lr 0.0001 \
+    --n_epochs 200 \
+    --batch_size 256 \
+    --seed 0
 ```
+In the example, the `--descriptor_type` argument is used to select the backbone models used in our experiments.
+It has 4 options: {"RDKit", "Linear", "2D", "3D"}, which corresponds to the DNN, ChemBERTa, GIN and TorchMD-NET backbone models in the CLI, respectively.
+In the future versions, we may consider including multiple backbone models that correspond to one descriptor, which requires us to specify the `--model_name` argument to separate the backbones.
+But currently, we do not need to worry about that and can leave `--model_name` as default.
 
-### Logging and WandB
+> For the interpretation of each argument, please check the [`muben.args` API](./muben.args.md) or directly refer to the [code implementation](https://github.com/Yinghao-Li/MUBen/tree/main/muben/args).
+> Notice that the API documentation may not be entirely comprehensive.
 
-By default, this project uses local logging files (`*.log`) and [WandB](https://wandb.ai/site) to track training status.
-
-The log files are stored as `./logs/<dataset>/<model>/<uncertainty>/<running_time>.log`.
-You can change the file path by specifying the `--log_path` argument, or disable log saving by setting `--log_path="disabled"`.
-
-To use WandB, you first need to register an account and sign in on your machine with `wandb login`.
-If you are running your code on a public device, you can instead use program-wise signing in by specifying the `--wandb_api_key` argument while running our code.
-You can find your API key in your browser here: https://wandb.ai/authorize.
-To disable WandB, use `--disable_wandb [true]`.
-By default, we use `MUBen-<dataset>` as WandB project name and `<model>-<uncertainty>` as the model name.
-You can change this behavior by specifying the `--wandb_project` and `--wandb_name` arguments.
-
-### Data Loading
+To run GROVER or Uni-Mol, we just need to replace `run.py` by the corresponding script, and slightly modify the arguments:
+```bash
+CUDA_VISIBLE_DEVICES=0 \
+PYTHONPATH="." \
+python ./run/unimol.py \
+    --data_folder "./data/files" \
+    --unimol_feature_folder "./data/UniMol/" \
+    --dataset_name "esol" \
+    --checkpoint_path "./models/unimol_base.pt" \
+    --uncertainty_method "MCDropout" \
+    --regression_with_variance \
+    ...
+```
+> For regression tasks, the argument `--regression_with_variance` is vital to guarantee a valid result with predicted variance.
 
-The progress will automatically create the necessary features (molecular descriptors) required by backbone models from the SMILES strings if they are loaded properly.
-The processed features are stored in the `<bottom-level data folder>/processed/` directory as `<train/valid/test>.pt` files by default, and will be automatically loaded the next time you apply the same backbone model on the same dataset.
-You can change this behavior with `--disable_dataset_saving` for disabling dataset saving or `--ignore_preprocessed_dataset` for not loading from the saved (processed) dataset.
+### Specify Arguments using `.yaml` Files
 
-Constructing Morgan fingerprint, RDKit features or 3D conformations for Uni-Mol may take a while.
-You can accelerate this process by utilizing multiple threads `--num_preprocess_workers=n>1` (default is 8).
-For 3D conformations, we directly take advantage of the results from Uni-Mol but still keep the choice of generating them by ourselves if the Uni-Mol data files are not found.
+Another way of specifying arguments is through the `.yaml` scripts, which provides more readable data structure than `.json` files.
+We have provided an [example configuration script](https://github.com/Yinghao-Li/MUBen/blob/main/scripts/config-example.yaml) within the [./scripts/](https://github.com/Yinghao-Li/MUBen/tree/main/scripts) directory, which runs GIN on the FreeSolv dataset with deterministic ("none") UQ method.
+To use it to specify arguments, we can run the python program with
+```bash
+PYTHONPATH="." CUDA_VISIBLE_DEVICES=0 python ./run/run.py ./scripts/config-example.yaml
+```
+This approach could be helpful while debugging the code on VSCode.
 
-### Calculating Metrics
+## Calculating Metrics
 
 During training, we only calculate metrics necessary for early stopping and simple prediction performance evaluation.
 To get other metrics, you need to use the `./assist/results_get_metrics.py` file.
 
-Specifically, you need to save the model predictions by **not** setting `--disable_dataset_saving`.
-The results are saved as `./<result_folder>/<dataset_name>/<model_name>/<uncertainty_method>/seed-<seed>/preds/<test_idx>.pt` files.
-When the training is finished, you can run the `./assist/results_get_metrics.py` file to generate all metrics for your model predictions.
+After training, the results are saved as `./<result_folder>/<dataset_name>/<model_name>/<uncertainty_method>/seed-<seed>/preds/<test_idx>.pt` files.
+You can run the `./assist/results_get_metrics.py` file to generate all metrics for your model predictions.
 For example:
 ```bash
-PYTHONPATH="." python ./assist/results_get_metrics.py ./scripts/config_metrics.json
+PYTHONPATH="." python ./assist/results_get_metrics.py [arguments]
 ```
-Make sure the hyper-parameters in the configuration file are updated to your needs.
-
-The metrics will be saved in the `./<result_folder>/RESULTS/<model_name>-<dataset_name>.csv` files.
-~~Notice that these files already exist in the repo if you keep the default `--result_folder=./output` argument and you need to check whether it is updated to reveal your experiment results.~~
+Make sure the arguments are updated to your needs.
 
-### Results
 
-We provided a more comprehensive copy of our experiment results [here](https://github.com/Yinghao-Li/UncertaintyBenchmark/tree/main/output) that are presented in the tables in our paper's appendix.
-We hope it can ease some effort if you want to further analyze the behavior of our backbone models and uncertainty quantification methods. 
+## Experimental Results
 
-## 4. ONGOING WORKS
+We have made our experimental results available in the [./reports/](https://github.com/Yinghao-Li/MUBen/tree/main/reports) directory.
+These results are organized into different folders based on the nature of the experiments:
 
-### 4.1. Active Learning
+- `primary`: Contains the most comprehensive set of results derived from experiments on scaffold-split datasets.
+- `random`: Includes results from experiments conducted on datasets that were split randomly.
+- `frozen`: Features results from experiments where the pre-trained model's weights were frozen, except for the last output layer, which was updatable.
+- `distribution`: Offers results from the QM9 dataset, where the test set was categorized into five bins based on the average Tanimoto similarities to the training scaffolds.
 
-We are developing code to integrate *active learning* into the pipeline.
-Specifically, we assume we have a small set of labeled data points (`--n_init_instances`) at the beginning.
-Within each active learning iteration, we use the labeled dataset to fine-tune the model parameters and select a batch of data points (`--n_al_select`) from the unlabeled set with the least predicted certainty (*i.e.*, max predicted entropy for classification and max predicted variance for regression).
-The process is repeated for several loops (`--n_al_loops`), and the intermediate performance is tracked.
+Files within these directories are named following the pattern `<backbone>-<dataset>.csv`.
+Each file provides a comparison of different UQ methods.
+The rows detail the performance of each UQ method, while the columns display the mean and standard deviation from three random runs for each metric.
 
-The code is still under construction and currently is **only available under the `dev` branch**.
-In addition, several points are worth attention:
-
-- Currently, only DNN and ChemBERTa backbones are supported (`./run/dnn_al.py` and `./run/chemberta_al.py`). Migrating AL to other backbones is not difficult but requires updating some Trainer functions if they are reloaded.
-- To enable active learning, make sure you set `--enable_active_learning` to `true`.
-- Currently, Deep Ensembles is not supported for AL.
-- We cannot guarantee the correctness of our implementation. If you notice any abnormalities in the code, please do not hesitate to post an issue.
-
-One example is
-```bash
-python ./run/dnn_al.py \
-  --enable_active_learning \
-  --n_init_instances 100 \
-  --n_al_loops 20 \
-  --n_al_select 20 \
-  # other model and training hyper-parameters...
-```
+Additional post-processing scripts can be found in the [./assist/](https://github.com/Yinghao-Li/MUBen/tree/main/assist) directory, which include files starting with `plot_` or `results_`.
+These scripts are useful for further analysis and visualization of the experimental data.
 
-## 5. CITATION
+## Citation
 
 If you find our work helpful, please consider citing it as
 ```latex
 @misc{li2023muben,
     title={MUBen: Benchmarking the Uncertainty of Pre-Trained Models for Molecular Property Prediction},
     author={Yinghao Li and Lingkai Kong and Yuanqi Du and Yue Yu and Yuchen Zhuang and Wenhao Mu and Chao Zhang},
     year={2023},
```

### Comparing `muben-0.0.1/muben/args/__init__.py` & `muben-0.0.2/muben/args/__init__.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/args/args_2d.py` & `muben-0.0.2/muben/args/args_2d.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/args/args_3d.py` & `muben-0.0.2/muben/args/args_3d.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/args/args_grover.py` & `muben-0.0.2/muben/args/args_grover.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/args/args_linear.py` & `muben-0.0.2/muben/args/args_linear.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/args/args_rdkit.py` & `muben-0.0.2/muben/args/args_rdkit.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/args/args_unimol.py` & `muben-0.0.2/muben/args/args_unimol.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/dataset/__init__.py` & `muben-0.0.2/muben/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/dataset/dataset.py` & `muben-0.0.2/muben/dataset/dataset_grover/molgraph.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,376 +1,327 @@
 """
-# Author: Yinghao Li
-# Modified: February 28th, 2024
-# ---------------------------------------
-# Description: Base classes for dataset creation and batch processing.
+The data structure of Molecules.
+This implementation is adapted from
+https://github.com/chemprop/chemprop/blob/master/chemprop/features/featurization.py
 """
 
-import json
-import os
-import regex
-import torch
-import logging
-import pandas as pd
-import numpy as np
-
-from ast import literal_eval
-from typing import Union, Optional
-from functools import cached_property
-from torch.utils.data import Dataset as TorchDataset
+from typing import List, Union
 
+import logging
+import torch
+from dataclasses import dataclass
+from rdkit import Chem
+from muben.dataset.dataset import Batch
 
 logger = logging.getLogger(__name__)
 
-__all__ = ["Dataset", "Batch", "pack_instances", "unpack_instances"]
+MAX_ATOMIC_NUM = 100
 
+ATOM_FEATURES = {
+    "atomic_num": list(range(MAX_ATOMIC_NUM)),
+    "degree": [0, 1, 2, 3, 4, 5],
+    "formal_charge": [-1, -2, 1, 2, 0],
+    "chiral_tag": [0, 1, 2, 3],
+    "num_Hs": [0, 1, 2, 3, 4],
+    "hybridization": [
+        Chem.rdchem.HybridizationType.SP,
+        Chem.rdchem.HybridizationType.SP2,
+        Chem.rdchem.HybridizationType.SP3,
+        Chem.rdchem.HybridizationType.SP3D,
+        Chem.rdchem.HybridizationType.SP3D2,
+    ],
+}
+
+# len(choices) + 1 to include room for uncommon values; + 2 at end for IsAromatic and mass
+ATOM_FDIM = sum(len(choices) + 1 for choices in ATOM_FEATURES.values()) + 2
+BOND_FDIM = 14
 
-class Dataset(TorchDataset):
-    """
-    Custom Dataset class to handle data storage, manipulation, and preprocessing operations.
 
-    Attributes:
-        _smiles (Union[list[str], None]): Chemical structures represented as strings.
-        _lbs (Union[np.ndarray, None]): Label data.
-        _masks (Union[np.ndarray, None]): Data masks.
-        _ori_ids (Union[np.ndarray, None]): Original IDs, specifically useful for randomly split datasets.
-        data_instances: Packed instances of data.
+def get_atom_fdim() -> int:
     """
+    Gets the dimensionality of atom features.
 
-    def __init__(self):
-        super().__init__()
-
-        self._smiles: Union[list[str], None] = None
-        self._lbs: Union[np.ndarray, None] = None
-        self._masks: Union[np.ndarray, None] = None
-        self._ori_ids: Union[np.ndarray, None] = None
-
-        self.data_instances_all = None
-        self.data_instances_selected = None
-        self.selected_ids = None
-        self.use_full_dataset = False
-
-        self._lbs_standardized: Union[np.ndarray, None] = None
-        self._use_standardized_lbs = False
-        self.has_standardized_lbs = False
-
-    @property
-    def data_instances(self):
-        """
-        Be careful with this property and the setter below
-        """
-        if self.use_full_dataset:
-            return self.data_instances_all
-        return self.data_instances_selected if self.data_instances_selected is not None else self.data_instances_all
+    :param: Arguments.
+    """
+    return ATOM_FDIM + 18
 
-    @data_instances.setter
-    def data_instances(self, x):
-        """
-        Be careful with this property and the setter below
-        """
-        self.data_instances_all = x
 
-    @property
-    def smiles(self) -> list[str]:
-        return self._smiles
+def get_bond_fdim() -> int:
+    """
+    Gets the dimensionality of bond features.
 
-    @property
-    def lbs(self) -> np.ndarray:
-        if self.has_standardized_lbs and self._use_standardized_lbs:
-            return self._lbs_standardized
-        return self._lbs
+    :param: Arguments.
+    """
+    return BOND_FDIM
 
-    def toggle_standardized_lbs(self, use_standardized_lbs: bool = None):
-        """
-        Toggle between standardized and unstandardized labels
 
-        Parameters
-        ----------
-        use_standardized_lbs: bool, optional
-            whether to use standardized labels
-
-        Returns
-        -------
-        self
-        """
-        if use_standardized_lbs is None:
-            self._use_standardized_lbs = not self._use_standardized_lbs
-            self.data_instances = self.get_instances()
-        else:
-            unchanged = use_standardized_lbs == self._use_standardized_lbs
-            self._use_standardized_lbs = use_standardized_lbs
-            if not unchanged:
-                self.data_instances = self.get_instances()
-        return self
+def onek_encoding_unk(value: int, choices: List[int]) -> List[int]:
+    """
+    Creates a one-hot encoding.
 
-    @cached_property
-    def masks(self) -> np.ndarray:
-        """
-        Return masks, and if not present, generate masks with ones.
-        """
-        return self._masks if self._masks is not None else np.ones_like(self.lbs).astype(int)
+    :param value: The value for which the encoding should be one.
+    :param choices: A list of possible values.
+    :return: A one-hot encoding of the value in a list of length len(choices) + 1.
+    If value is not in the list of choices, then the final element in the encoding is 1.
+    """
+    encoding = [0] * (len(choices) + 1)
+    if min(choices) < 0:
+        index = value
+    else:
+        index = choices.index(value) if value in choices else -1
+    encoding[index] = 1
 
-    def __len__(self):
-        if self.data_instances is not None:
-            return len(self.data_instances)
-        return len(self._smiles)
+    return encoding
 
-    def __getitem__(self, idx):
-        return self.data_instances[idx]
 
-    def update_lbs(self, lbs):
-        """
-        Update dataset labels and instance list accordingly
-        """
-        self._lbs = lbs
-        self.data_instances = self.get_instances()
-        return self
+class MolGraph:
+    """
+    A MolGraph represents the graph structure and featurization of a single molecule.
 
-    def set_standardized_lbs(self, lbs):
-        """
-        Update dataset labels and instance list accordingly
-        """
-        self._lbs_standardized = lbs
-        self.has_standardized_lbs = True
-        return self
+    A MolGraph computes the following attributes:
+    - smiles: Smiles string.
+    - n_atoms: The number of atoms in the molecule.
+    - n_bonds: The number of bonds in the molecule.
+    - f_atoms: A mapping from an atom index to a list atom features.
+    - f_bonds: A mapping from a bond index to a list of bond features.
+    - a2b: A mapping from an atom index to a list of incoming bond indices.
+    - b2a: A mapping from a bond index to the index of the atom the bond originates from.
+    - b2revb: A mapping from a bond index to the index of the reverse bond.
+    """
 
-    def prepare(self, config, partition, **kwargs):
+    def __init__(self, smiles: str):
         """
-        Prepare dataset for training and test
+        Computes the graph structure and featurization of a molecule.
 
-        Parameters
-        ----------
-        config: configurations
-        partition: dataset partition; in [train, valid, test]
-
-        Returns
-        -------
-        self
+        :param smiles: A smiles string.
         """
-
-        assert partition in ["train", "valid", "test"], ValueError(
-            f"Argument `partition` should be one of 'train', 'valid' or 'test'!"
+        self.smiles = smiles
+        self.n_atoms = 0  # number of atoms
+        self.n_bonds = 0  # number of bonds
+        self.f_atoms = []  # mapping from atom index to atom features
+        self.f_bonds = []  # mapping from bond index to concat(in_atom, bond) features
+        self.a2b = []  # mapping from atom index to incoming bond indices
+        self.b2a = []  # mapping from bond index to the index of the atom the bond is coming from
+        self.b2revb = []  # mapping from bond index to the index of the reverse bond
+
+        # Convert smiles to molecule
+        mol = Chem.MolFromSmiles(smiles)
+
+        self.hydrogen_donor = Chem.MolFromSmarts("[$([N;!H0;v3,v4&+1]),$([O,S;H1;+0]),n&H1&+0]")
+        self.hydrogen_acceptor = Chem.MolFromSmarts(
+            "[$([O,S;H1;v2;!$(*-*=[O,N,P,S])]),$([O,S;H0;v2]),$([O,S;-]),$([N;v3;!$(N-*=[O,N,P,S])]),"
+            "n&H0&+0,$([o,s;+0;!$([o,s]:n);!$([o,s]:c:n)])]"
+        )
+        self.acidic = Chem.MolFromSmarts("[$([C,S](=[O,S,P])-[O;H1,-1])]")
+        self.basic = Chem.MolFromSmarts(
+            "[#7;+,$([N;H2&+0][$([C,a]);!$([C,a](=O))]),$([N;H1&+0]([$([C,a]);!$([C,a](=O))])[$([C,a]);"
+            "!$([C,a](=O))]),$([N;H0&+0]([C;!$(C(=O))])([C;!$(C(=O))])[C;!$(C(=O))])]"
         )
 
-        method_identifier = (
-            f"{config.model_name}-{config.feature_type}" if config.feature_type != "none" else config.model_name
+        self.hydrogen_donor_match = sum(mol.GetSubstructMatches(self.hydrogen_donor), ())
+        self.hydrogen_acceptor_match = sum(mol.GetSubstructMatches(self.hydrogen_acceptor), ())
+        self.acidic_match = sum(mol.GetSubstructMatches(self.acidic), ())
+        self.basic_match = sum(mol.GetSubstructMatches(self.basic), ())
+        self.ring_info = mol.GetRingInfo()
+
+        # fake the number of "atoms" if we are collapsing substructures
+        self.n_atoms = mol.GetNumAtoms()
+
+        # Get atom features
+        for _, atom in enumerate(mol.GetAtoms()):
+            self.f_atoms.append(self.atom_features(atom))
+        self.f_atoms = [self.f_atoms[i] for i in range(self.n_atoms)]
+
+        for _ in range(self.n_atoms):
+            self.a2b.append([])
+
+        # Get bond features
+        for a1 in range(self.n_atoms):
+            for a2 in range(a1 + 1, self.n_atoms):
+                bond = mol.GetBondBetweenAtoms(a1, a2)
+
+                if bond is None:
+                    continue
+
+                f_bond = self.bond_features(bond)
+
+                # Always treat the bond as directed.
+                self.f_bonds.append(self.f_atoms[a1] + f_bond)
+                self.f_bonds.append(self.f_atoms[a2] + f_bond)
+
+                # Update index mappings
+                b1 = self.n_bonds
+                b2 = b1 + 1
+                self.a2b[a2].append(b1)  # b1 = a1 --> a2
+                self.b2a.append(a1)
+                self.a2b[a1].append(b2)  # b2 = a2 --> a1
+                self.b2a.append(a2)
+                self.b2revb.append(b2)
+                self.b2revb.append(b1)
+                self.n_bonds += 2
+
+    def atom_features(self, atom: Chem.rdchem.Atom) -> List[Union[bool, int, float]]:
+        """
+        Builds a feature vector for an atom.
+
+        :param atom: An RDKit atom.
+        :return: A list containing the atom features.
+        """
+        features = (
+            onek_encoding_unk(atom.GetAtomicNum() - 1, ATOM_FEATURES["atomic_num"])
+            + onek_encoding_unk(atom.GetTotalDegree(), ATOM_FEATURES["degree"])
+            + onek_encoding_unk(atom.GetFormalCharge(), ATOM_FEATURES["formal_charge"])
+            + onek_encoding_unk(int(atom.GetChiralTag()), ATOM_FEATURES["chiral_tag"])
+            + onek_encoding_unk(int(atom.GetTotalNumHs()), ATOM_FEATURES["num_Hs"])
+            + onek_encoding_unk(int(atom.GetHybridization()), ATOM_FEATURES["hybridization"])
+            + [1 if atom.GetIsAromatic() else 0]
+            + [atom.GetMass() * 0.01]
         )
-        preprocessed_path = os.path.normpath(
-            os.path.join(
-                config.data_dir,
-                "processed",
-                method_identifier,
-                f"{partition}.pt",
-            )
+        atom_idx = atom.GetIdx()
+        features = (
+            features
+            + onek_encoding_unk(atom.GetImplicitValence(), [0, 1, 2, 3, 4, 5, 6])
+            + [atom_idx in self.hydrogen_acceptor_match]
+            + [atom_idx in self.hydrogen_donor_match]
+            + [atom_idx in self.acidic_match]
+            + [atom_idx in self.basic_match]
+            + [
+                self.ring_info.IsAtomInRingOfSize(atom_idx, 3),
+                self.ring_info.IsAtomInRingOfSize(atom_idx, 4),
+                self.ring_info.IsAtomInRingOfSize(atom_idx, 5),
+                self.ring_info.IsAtomInRingOfSize(atom_idx, 6),
+                self.ring_info.IsAtomInRingOfSize(atom_idx, 7),
+                self.ring_info.IsAtomInRingOfSize(atom_idx, 8),
+            ]
         )
-        # Load Pre-processed dataset if exist
-        if os.path.exists(preprocessed_path) and not config.ignore_preprocessed_dataset:
-            logger.info(f"Loading pre-processed dataset {preprocessed_path}")
-            self.load(preprocessed_path)
-        # else, load dataset from csv and generate features
-        else:
-            self.read_csv(config.data_dir, partition)
-
-            logger.info("Creating features")
-            self.create_features(config)
+        return features
 
-            # Always save pre-processed dataset to disk
-            if not config.disable_dataset_saving:
-                logger.info("Saving pre-processed dataset")
-                self.save(preprocessed_path)
-
-        self.data_instances = self.get_instances()
-        return self
-
-    def downsample_by(self, file_path: str = None, ids: list[int] = None):
+    @staticmethod
+    def bond_features(bond: Chem.rdchem.Bond) -> List[Union[bool, int, float]]:
         """
-        Down-sample the instances to a subset with the specified indices
+        Builds a feature vector for a bond.
 
-        Parameters
-        ----------
-        file_path: str, optional
-            path to the file containing the indices of the selected instances
-        ids: list[int], optional
-            indices of the selected instances
-
-        Returns
-        -------
-        self
+        :param bond: A RDKit bond.
+        :return: A list containing the bond features.
         """
-        assert ids is not None or file_path is not None, ValueError("Either `ids` or `file_path` should be specified!")
-
-        if file_path:
-            with open(file_path, "r", encoding="utf-8") as f:
-                ids = json.load(f)
-
-        self.selected_ids = ids
-        self.data_instances_selected = [self.data_instances_all[idx] for idx in self.selected_ids]
-        return self
-
-    def add_sample_by_ids(self, ids: list[int] = None):
-        """
-        Append a subset of data instances to the data_instances_selected
-
-
-        Parameters
-        ----------
-        ids: list[int], optional
-            indices of the selected instances
-
-        Returns
-        -------
-        self
-        """
-        assert ids is not None, ValueError("`ids` should be specified!")
-
-        intersection = set(ids).intersection(set(self.selected_ids))
-        if intersection:
-            logger.warning(f"IDs {ids} already exist in the selected instances.")
-            return self
-
-        self.selected_ids = list(set(self.selected_ids).union(set(ids)))
-        self.data_instances_selected = [self.data_instances_all[idx] for idx in self.selected_ids]
-
-        return self
-
-    # noinspection PyTypeChecker
-    def create_features(self, config):
-        """
-        Create data features
-
-        Returns
-        -------
-        self
-        """
-        raise NotImplementedError
-
-    def get_instances(self):
-        raise NotImplementedError
-
-    def save(self, file_path: str):
-        """
-        Save the entire dataset for future usage
-
-        Parameters
-        ----------
-        file_path: path to the saved file
-
-        Returns
-        -------
-        self
-        """
-        attr_dict = dict()
-        for attr, value in self.__dict__.items():
-            if regex.match(f"^_[a-z]", attr):
-                attr_dict[attr] = value
-
-        os.makedirs(os.path.dirname(os.path.normpath(file_path)), exist_ok=True)
-        torch.save(attr_dict, file_path)
-
-        return self
-
-    def load(self, file_path: str):
-        """
-        Load the entire dataset from disk
-
-        Parameters
-        ----------
-        file_path: path to the saved file
-
-        Returns
-        -------
-        self
-        """
-        attr_dict = torch.load(file_path)
-
-        for attr, value in attr_dict.items():
-            if attr not in self.__dict__:
-                logger.warning(f"Attribute {attr} is not natively defined in dataset!")
-
-            setattr(self, attr, value)
-
-        return self
-
-    def read_csv(self, data_dir: str, partition: str):
-        """
-        Read data from csv files
-        """
-        file_path = os.path.normpath(os.path.join(data_dir, f"{partition}.csv"))
-        logger.info(f"Loading dataset {file_path}")
-
-        if not (file_path and os.path.exists(file_path)):
-            raise FileNotFoundError(f"File {file_path} does not exist!")
-
-        df = pd.read_csv(file_path)
-        self._smiles = df.smiles.tolist()
-        self._lbs = np.asarray(df.labels.map(literal_eval).to_list())
-        self._masks = np.asarray(df.masks.map(literal_eval).to_list()) if not df.masks.isnull().all() else None
-        self._ori_ids = df.ori_ids.to_numpy() if "ori_ids" in df.keys() else None  # for randomly split dataset
 
+        if bond is None:
+            fbond = [1] + [0] * (BOND_FDIM - 1)
+        else:
+            bt = bond.GetBondType()
+            fbond = [
+                0,  # bond is not None
+                bt == Chem.rdchem.BondType.SINGLE,
+                bt == Chem.rdchem.BondType.DOUBLE,
+                bt == Chem.rdchem.BondType.TRIPLE,
+                bt == Chem.rdchem.BondType.AROMATIC,
+                (bond.GetIsConjugated() if bt is not None else 0),
+                (bond.IsInRing() if bt is not None else 0),
+            ]
+            fbond += onek_encoding_unk(int(bond.GetStereo()), list(range(6)))
+        return fbond
+
+
+@dataclass
+class MolGraphAttrs:
+    n_atoms = None
+    n_bonds = None
+    f_atoms = None
+    f_bonds = None
+    a2b = None
+    b2a = None
+    b2revb = None
+
+    def from_mol_graph(self, graph: MolGraph):
+        attrs = ("n_atoms", "n_bonds", "f_atoms", "f_bonds", "a2b", "b2a", "b2revb")
+        for attr in attrs:
+            setattr(self, attr, getattr(graph, attr))
         return self
 
 
-class Batch:
-    """
-    A batch of data instances, each is initialized with a dict with attribute names as keys
+class BatchMolGraph(Batch):
     """
+    A BatchMolGraph represents the graph structure and featurization of a batch of molecules.
 
-    def __init__(self, **kwargs):
-        self.size = 0
-        self._tensor_members = dict()
-        for k, v in kwargs.items():
-            if k == "batch_size":
-                self.size = v
-            setattr(self, k, v)
-            self._register_tensor_members(k, v)
-
-    def _register_tensor_members(self, k, v):
-        """
-        Register tensor members to the batch
-        """
-        if isinstance(v, torch.Tensor) or callable(getattr(v, "to", None)):
-            self._tensor_members[k] = v
-
-    def to(self, device):
-        """
-        Move all tensor members to the target device
-        """
-        for k, v in self._tensor_members.items():
-            setattr(self, k, v.to(device))
-        return self
-
-    def __len__(self):
-        return len(tuple(self._tensor_members.values())[0]) if not self.size else self.size
-
-
-def pack_instances(**kwargs) -> list[dict]:
-    """
-    Convert attribute lists to a list of data instances, each is a dict with attribute names as keys
-    and one datapoint attribute values as values
+    A BatchMolGraph contains the attributes of a MolGraph plus:
+    - atom_fdim: The dimensionality of the atom features.
+    - bond_fdim: The dimensionality of the bond features (technically the combined atom/bond features).
+    - a_scope: A list of tuples indicating the start and end atom indices for each molecule.
+    - b_scope: A list of tuples indicating the start and end bond indices for each molecule.
+    - max_num_bonds: The maximum number of bonds neighboring an atom in this batch.
+    - b2b: (Optional) A mapping from a bond index to incoming bond indices.
+    - a2a: (Optional): A mapping from an atom index to neighboring atom indices.
     """
 
-    instance_list = list()
-    keys = tuple(kwargs.keys())
-
-    for inst_attrs in zip(*tuple(kwargs.values())):
-        inst = dict(zip(keys, inst_attrs))
-        instance_list.append(inst)
-
-    return instance_list
+    def __init__(self, mol_graphs: List[MolGraphAttrs]):
+        super().__init__()
 
+        self.atom_fdim = get_atom_fdim()
+        self.bond_fdim = get_bond_fdim() + self.atom_fdim
 
-def unpack_instances(instance_list: list[dict], attr_names: Optional[list[str]] = None):
-    """
-    Convert a list of dict-type instances to a list of value lists,
-    each contains all values within a batch of each attribute
+        # Start n_atoms and n_bonds at 1 b/c zero padding
+        self.n_atoms = 1  # number of atoms (start at 1 b/c need index 0 as padding)
+        self.n_bonds = 1  # number of bonds (start at 1 b/c need index 0 as padding)
+        self.a_scope = []  # list of tuples indicating (start_atom_index, num_atoms) for each molecule
+        self.b_scope = []  # list of tuples indicating (start_bond_index, num_bonds) for each molecule
+
+        # All start with zero padding so that indexing with zero padding returns zeros
+        f_atoms = [[0] * self.atom_fdim]  # atom features
+        f_bonds = [[0] * self.bond_fdim]  # combined atom/bond features
+        a2b = [[]]  # mapping from atom index to incoming bond indices
+        b2a = [0]  # mapping from bond index to the index of the atom the bond is coming from
+        b2revb = [0]  # mapping from bond index to the index of the reverse bond
+
+        for mol_graph in mol_graphs:
+            f_atoms.extend(mol_graph.f_atoms)
+            f_bonds.extend(mol_graph.f_bonds)
+
+            for a in range(mol_graph.n_atoms):
+                a2b.append([b + self.n_bonds for b in mol_graph.a2b[a]])
+
+            for b in range(mol_graph.n_bonds):
+                b2a.append(self.n_atoms + mol_graph.b2a[b])
+                b2revb.append(self.n_bonds + mol_graph.b2revb[b])
+
+            self.a_scope.append((self.n_atoms, mol_graph.n_atoms))
+            self.b_scope.append((self.n_bonds, mol_graph.n_bonds))
+            self.n_atoms += mol_graph.n_atoms
+            self.n_bonds += mol_graph.n_bonds
+
+        # max with 1 to fix a crash in rare case of all single-heavy-atom mols
+        self.max_num_bonds = max(1, max(len(in_bonds) for in_bonds in a2b))
+
+        self.f_atoms = torch.tensor(f_atoms, dtype=torch.float)
+        self.f_bonds = torch.tensor(f_bonds, dtype=torch.float)
+        self.a2b = torch.tensor(
+            [a2b[a] + [0] * (self.max_num_bonds - len(a2b[a])) for a in range(self.n_atoms)],
+            dtype=torch.long,
+        )
+        self.b2a = torch.tensor(b2a, dtype=torch.long)
+        self.b2revb = torch.tensor(b2revb, dtype=torch.long)
+        self.b2b = None  # try to avoid computing b2b b/c O(n_atoms^3)
+        self.a2a = self.b2a[self.a2b]  # only needed if using atom messages
+        self.a_scope = torch.tensor(self.a_scope, dtype=torch.long)
+        self.b_scope = torch.tensor(self.b_scope, dtype=torch.long)
+
+        for k, v in self.__dict__.items():
+            if isinstance(v, torch.Tensor):
+                self._register_tensor_members(k, v)
 
-    Parameters
-    ----------
-    instance_list: a list of attributes
-    attr_names: the name of the needed attributes. Notice that this variable should be specified
-        for Python versions that does not natively support ordered dict
-    """
-    if not attr_names:
-        attr_names = list(instance_list[0].keys())
-    attribute_tuple = [[inst[name] for inst in instance_list] for name in attr_names]
+    @property
+    def components(self):
+        """
+        Returns the components of the BatchMolGraph.
 
-    return attribute_tuple
+        :return: A tuple containing PyTorch tensors with the atom features, bond features, and graph structure
+        and two lists indicating the scope of the atoms and bonds (i.e. which molecules they belong to).
+        """
+        return (
+            self.f_atoms,
+            self.f_bonds,
+            self.a2b,
+            self.b2a,
+            self.b2revb,
+            self.a_scope,
+            self.b_scope,
+            self.a2a,
+        )
```

### Comparing `muben-0.0.1/muben/dataset/dataset_2d/collate.py` & `muben-0.0.2/muben/dataset/dataset_2d/collate.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/dataset/dataset_2d/dataset.py` & `muben-0.0.2/muben/dataset/dataset_2d/dataset.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/dataset/dataset_3d/collate.py` & `muben-0.0.2/muben/dataset/dataset_3d/collate.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/dataset/dataset_3d/dataset.py` & `muben-0.0.2/muben/dataset/dataset_3d/dataset.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/dataset/dataset_grover/collate.py` & `muben-0.0.2/muben/dataset/dataset_grover/collate.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/dataset/dataset_grover/dataset.py` & `muben-0.0.2/muben/dataset/dataset_grover/dataset.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/dataset/dataset_linear/collate.py` & `muben-0.0.2/muben/dataset/dataset_linear/collate.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/dataset/dataset_linear/dataset.py` & `muben-0.0.2/muben/dataset/dataset_linear/dataset.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/dataset/dataset_rdkit/collate.py` & `muben-0.0.2/muben/dataset/dataset_rdkit/collate.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/dataset/dataset_rdkit/dataset.py` & `muben-0.0.2/muben/dataset/dataset_rdkit/dataset.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/dataset/dataset_unimol/collate.py` & `muben-0.0.2/muben/dataset/dataset_unimol/collate.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/dataset/dataset_unimol/dataset.py` & `muben-0.0.2/muben/dataset/dataset_unimol/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 # Author: Yinghao Li
-# Modified: February 28th, 2024
+# Modified: April 10th, 2024
 # ---------------------------------------
 # Description: Dataset class for Uni-Mol
 """
 
 import os.path as op
 import logging
 from functools import partial
@@ -43,14 +43,26 @@
 
         self._partition = None
         self._atoms = None
         self._coordinates = None
         self.processing_pipeline = None
         self.data_processor = None
 
+    @property
+    def atoms(self):
+        if self.selected_ids is not None:
+            return [self._atoms[idx] for idx in self.selected_ids]
+        return self._atoms
+
+    @property
+    def coordinates(self):
+        if self.selected_ids is not None:
+            return [self._coordinates[idx] for idx in self.selected_ids]
+        return self._coordinates
+
     def __getitem__(self, idx):
         """
         Retrieve a specific instance from the dataset.
 
         Parameters
         ----------
         idx : int
@@ -58,15 +70,15 @@
 
         Returns
         -------
         dict
             Dictionary containing features of the specific instance.
         """
         atoms, coordinates, distances, edge_types = self.data_processor(
-            atoms=self._atoms[idx], coordinates=self._coordinates[idx]
+            atoms=self.atoms[idx], coordinates=self.coordinates[idx]
         )
         feature_dict = {
             "atoms": atoms,
             "coordinates": coordinates,
             "distances": distances,
             "edge_types": edge_types,
             "lbs": self.lbs[idx],
@@ -91,15 +103,15 @@
         assert variant in (
             "training",
             "inference",
         ), "Processor variant must be `training` or `inference`"
         self.data_processor = getattr(self.processing_pipeline, f"process_{variant}")
         return self
 
-    def prepare(self, config, partition, dictionary=None):
+    def prepare(self, config, partition, dictionary=None, **kwargs):
         """
         Prepare the dataset based on the given configuration.
 
         Parameters
         ----------
         config : object
             Configuration object containing necessary settings.
@@ -125,15 +137,15 @@
             max_atoms=config.max_atoms,
             max_seq_len=config.max_seq_len,
             remove_hydrogen_flag=config.remove_hydrogen,
             remove_polar_hydrogen_flag=config.remove_polar_hydrogen,
         )
         self.set_processor_variant(processor_variant)
 
-        super().prepare(config, partition)
+        super().prepare(config, partition, **kwargs)
 
         return self
 
     def create_features(self, config):
         """
         Create or load data features for the dataset.
```

### Comparing `muben-0.0.1/muben/dataset/dataset_unimol/dictionary.py` & `muben-0.0.2/muben/dataset/dataset_unimol/dictionary.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/dataset/dataset_unimol/process.py` & `muben-0.0.2/muben/dataset/dataset_unimol/process.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/layers/layers.py` & `muben-0.0.2/muben/layers/layers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 # Author: Yinghao Li
-# Modified: February 27th, 2024
+# Modified: February 29th, 2024
 # ---------------------------------------
 # Description: 
 
 Versatile Output Layer for Backbone Models
 
 This module implements an output layer that can be applied to various
 backbone models. It provides the option of utilizing different uncertainty 
@@ -19,41 +19,51 @@
 from muben.utils.macro import UncertaintyMethods
 
 
 class OutputLayer(nn.Module):
     """
     Customizable output layer for various backbone models.
 
-    This class provides an interface to add an output layer with or without uncertainty methods.
+    This class provides an interface to add an output layer with or without uncertainty methods
+    to various backbone models. It supports both classification and regression tasks and allows
+    for the introduction of uncertainty into the model's output.
+
+    Args:
+        last_hidden_dim (int): Dimensionality of the last hidden state from the backbone model.
+        n_output_heads (int): Number of output heads (e.g., number of classes for classification).
+        uncertainty_method (str, optional): Method to introduce uncertainty in the output layer.
+            Available methods are defined in UncertaintyMethods. Defaults to UncertaintyMethods.none.
+        task_type (str, optional): Type of task - "classification" or "regression". Defaults to "classification".
+        **kwargs: Additional keyword arguments to be passed to the specific output layers.
+
+    Attributes:
+        _uncertainty_method (str): The uncertainty method used in the output layer.
+        _task_type (str): The type of task the model is configured for (classification or regression).
+        output_layer (nn.Module): The specific output layer instance used in the model.
+        kld (Optional[torch.Tensor]): Kullback-Leibler Divergence for Bayesian methods, if applicable.
     """
 
     def __init__(
         self,
         last_hidden_dim,
         n_output_heads,
         uncertainty_method=UncertaintyMethods.none,
         task_type="classification",
         **kwargs
     ):
         """
-        Initialize the model output layer.
+        Initializes the OutputLayer instance.
 
-        Parameters
-        ----------
-        last_hidden_dim : int
-            Dimensionality of the last hidden state from the backbone model.
-        n_output_heads : int
-            Number of output heads (e.g., number of classes for classification).
-        uncertainty_method : str, optional
-            Method to introduce uncertainty in the output layer.
-            Available methods are defined in UncertaintyMethods.
-        task_type : str, optional
-            Type of task - "classification" or "regression".
-        kwargs : dict
-            Additional keyword arguments to be passed to the specific output layers.
+        Args:
+            last_hidden_dim (int): Dimensionality of the last hidden state from the backbone model.
+            n_output_heads (int): Number of output heads (e.g., number of classes for classification).
+            uncertainty_method (str, optional): Method to introduce uncertainty in the output layer.
+                Available methods are defined in UncertaintyMethods. Defaults to UncertaintyMethods.none.
+            task_type (str, optional): Type of task - "classification" or "regression". Defaults to "classification".
+            **kwargs: Additional keyword arguments to be passed to the specific output layers.
         """
 
         super().__init__()
 
         self._uncertainty_method = uncertainty_method
         self._task_type = task_type
 
@@ -67,46 +77,42 @@
 
         # Kullback-Leibler Divergence for Bayesian methods
         self.kld = None
         self.initialize()
 
     def initialize(self) -> "OutputLayer":
         """
-        Initialize the weights of the output layer.
+        Initializes the weights of the output layer.
 
         Different initializations are applied based on the uncertainty method and task type.
 
-        Returns
-        -------
-        OutputLayer
-            Initialized model instance.
+        Returns:
+            OutputLayer: The initialized model instance.
         """
+
         if self._uncertainty_method == UncertaintyMethods.bbp:
             self.output_layer.initialize()
             self.kld = None
         elif self._uncertainty_method == UncertaintyMethods.evidential and self._task_type == "regression":
             self.output_layer.initialize()
         else:
             nn.init.xavier_uniform_(self.output_layer.weight)
             self.output_layer.bias.data.fill_(0.01)
         return self
 
     def forward(self, x: torch.Tensor, **kwargs) -> torch.Tensor:
         """
         Forward pass of the output layer.
 
-        Parameters
-        ----------
-        x : torch.Tensor
-            Input tensor for the output layer.
-
-        Returns
-        -------
-        logits : torch.Tensor
-            The output logits or values of the model.
+        Args:
+            x (torch.Tensor): Input tensor for the output layer.
+
+        Returns:
+            torch.Tensor: The output logits or values of the model.
         """
+
         if self._uncertainty_method == UncertaintyMethods.bbp:
             logits, self.kld = self.output_layer(x)
         else:
             logits = self.output_layer(x)
 
         return logits
```

### Comparing `muben-0.0.1/muben/model/dnn/dnn.py` & `muben-0.0.2/muben/model/dnn/dnn.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/model/gin/gin.py` & `muben-0.0.2/muben/model/gin/gin.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/model/grover/layers.py` & `muben-0.0.2/muben/model/grover/layers.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/model/grover/model.py` & `muben-0.0.2/muben/model/grover/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,36 +153,38 @@
             config.ffn_hidden_size,
             config.n_lbs * config.n_tasks,
             config.uncertainty_method,
             task_type=config.task_type,
             bbp_prior_sigma=config.bbp_prior_sigma,
         )
 
-        # Build model
-        model_state_dict = self.state_dict()
+        if not config.disable_checkpoint_loading:
 
-        # Skip missing parameters and parameters of mismatched size
-        pretrained_state_dict = {}
-        for param_name in loaded_state_dict.keys():
-            new_param_name = param_name
-            if new_param_name not in model_state_dict:
-                logger.info(f'Pretrained parameter "{param_name}" cannot be found in model parameters.')
-            elif model_state_dict[new_param_name].shape != loaded_state_dict[param_name].shape:
-                logger.info(
-                    f'Pretrained parameter "{param_name}" '
-                    f"of shape {loaded_state_dict[param_name].shape} does not match corresponding "
-                    f"model parameter of shape {model_state_dict[new_param_name].shape}."
-                )
-            else:
-                pretrained_state_dict[new_param_name] = loaded_state_dict[param_name]
-        logger.info(f"Pretrained parameter loaded.")
-        # Load pretrained weights
-        model_state_dict.update(pretrained_state_dict)
+            # Build model
+            model_state_dict = self.state_dict()
+
+            # Skip missing parameters and parameters of mismatched size
+            pretrained_state_dict = {}
+            for param_name in loaded_state_dict.keys():
+                new_param_name = param_name
+                if new_param_name not in model_state_dict:
+                    logger.info(f'Pretrained parameter "{param_name}" cannot be found in model parameters.')
+                elif model_state_dict[new_param_name].shape != loaded_state_dict[param_name].shape:
+                    logger.info(
+                        f'Pretrained parameter "{param_name}" '
+                        f"of shape {loaded_state_dict[param_name].shape} does not match corresponding "
+                        f"model parameter of shape {model_state_dict[new_param_name].shape}."
+                    )
+                else:
+                    pretrained_state_dict[new_param_name] = loaded_state_dict[param_name]
+            logger.info(f"Pretrained parameter loaded.")
+            # Load pretrained weights
+            model_state_dict.update(pretrained_state_dict)
 
-        self.load_state_dict(model_state_dict)
+            self.load_state_dict(model_state_dict)
 
     def init_backbone_weights(self):
         for param in self.parameters():
             if param.dim() == 1:
                 nn.init.constant_(param, 0)
             else:
                 nn.init.xavier_normal_(param)
```

### Comparing `muben-0.0.1/muben/model/grover/ts.py` & `muben-0.0.2/muben/model/grover/ts.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/model/grover/utils.py` & `muben-0.0.2/muben/model/grover/utils.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/model/linear_transformer/linear_transformer.py` & `muben-0.0.2/muben/model/linear_transformer/linear_transformer.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/model/torchmdnet/et.py` & `muben-0.0.2/muben/model/torchmdnet/et.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/model/torchmdnet/layers.py` & `muben-0.0.2/muben/model/torchmdnet/layers.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/model/torchmdnet/modules.py` & `muben-0.0.2/muben/model/torchmdnet/modules.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/model/torchmdnet/torchmdnet.py` & `muben-0.0.2/muben/model/torchmdnet/torchmdnet.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/model/unimol/encoder.py` & `muben-0.0.2/muben/model/unimol/encoder.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/model/unimol/layers/layer_norm.py` & `muben-0.0.2/muben/model/unimol/layers/layer_norm.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/model/unimol/layers/multihead_attention.py` & `muben-0.0.2/muben/model/unimol/layers/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/model/unimol/layers/softmax_dropout.py` & `muben-0.0.2/muben/model/unimol/layers/softmax_dropout.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/model/unimol/layers/transformer_encoder.py` & `muben-0.0.2/muben/model/unimol/layers/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/model/unimol/layers/transformer_encoder_layer.py` & `muben-0.0.2/muben/model/unimol/layers/transformer_encoder_layer.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/model/unimol/layers/utils.py` & `muben-0.0.2/muben/model/unimol/layers/utils.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/model/unimol/module.py` & `muben-0.0.2/muben/model/unimol/module.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/model/unimol/unimol.py` & `muben-0.0.2/muben/model/unimol/unimol.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 # Author: Yinghao Li
-# Modified: February 28th, 2024
+# Modified: March 4th, 2024
 # ---------------------------------------
 # Description: The Uni-Mol model
 # Reference: Modified from https://github.com/dptech-corp/Uni-Mol/tree/main/unimol
 """
 
 # Original copyright:
 # Copyright (c) DP Technology.
@@ -81,16 +81,17 @@
             config.encoder_embed_dim,
             config.n_lbs * config.n_tasks,
             config.uncertainty_method,
             task_type=config.task_type,
             bbp_prior_sigma=config.bbp_prior_sigma,
         )
 
-        state = self.load_checkpoint(self.config.checkpoint_path)
-        self.load_state_dict(state["model"], strict=False)
+        if not config.disable_checkpoint_loading:
+            state = self.load_checkpoint(self.config.checkpoint_path)
+            self.load_state_dict(state["model"], strict=False)
 
     def load_checkpoint(self, path, arg_overrides=None):
         """
         Load a checkpoint to CPU.
 
         If present, the function also applies overrides to arguments present
         in the checkpoint.
```

### Comparing `muben-0.0.1/muben/train/trainer/container.py` & `muben-0.0.2/muben/train/trainer/container.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/train/trainer/loss.py` & `muben-0.0.2/muben/train/trainer/loss.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/train/trainer/metric.py` & `muben-0.0.2/muben/train/trainer/metric.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/train/trainer/scaler.py` & `muben-0.0.2/muben/train/trainer/scaler.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/train/trainer/state.py` & `muben-0.0.2/muben/train/trainer/state.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/train/trainer/timer.py` & `muben-0.0.2/muben/train/trainer/timer.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/train/trainer/trainer.py` & `muben-0.0.2/muben/train/trainer/trainer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 # Author: Yinghao Li
-# Modified: February 27th, 2024
+# Modified: April 16th, 2024
 # ---------------------------------------
 # Description:
 
 Base trainer functions to facilitate training, validation, and testing 
 of machine learning models. This Trainer class is designed to seamlessly 
 integrate with various datasets, loss functions, metrics, and uncertainty 
 estimation methods. It provides convenient mechanisms to standardize, 
@@ -12,15 +12,15 @@
 and Weights & Biases (wandb) for experiment tracking.
 """
 
 import copy
 import wandb
 import logging
 import numpy as np
-import os.path as op
+import os.path as osp
 import torch
 import torch.nn.functional as F
 import torch.nn as nn
 from torch.optim import AdamW
 from torch.utils.data import DataLoader
 
 from typing import Optional, Union, Tuple
@@ -54,44 +54,43 @@
 
 logger = logging.getLogger(__name__)
 
 __all__ = ["Trainer"]
 
 
 class Trainer:
+    """
+    This Trainer class is designed to facilitate the training, validation, and testing of machine learning models.
+    It integrates with various datasets, loss functions, metrics, and uncertainty estimation methods, providing
+    mechanisms to standardize, initialize, and manage training states. It supports logging and integration with
+    Weights & Biases (wandb) for experiment tracking.
+    """
+
     def __init__(
         self,
         config,
         model_class=None,
         training_dataset=None,
         valid_dataset=None,
         test_dataset=None,
         collate_fn=None,
         scalar=None,
         **kwargs,
     ):
-        """
-        Initialize the Trainer object.
+        """Initializes the Trainer object.
 
-        Parameters
-        ----------
-        config : Config
-            Configuration object containing all necessary parameters for training.
-        training_dataset : Dataset, optional
-            Dataset for training the model.
-        valid_dataset : Dataset, optional
-            Dataset for validating the model.
-        test_dataset : Dataset, optional
-            Dataset for testing the model.
-        collate_fn : Callable, optional
-            Function to collate data samples into batches.
-        scalar : StandardScaler, optional
-            Scaler for standardizing input data.
-        **kwargs : dict, optional
-            Additional keyword arguments.
+        Args:
+            config (Config): Configuration object containing all necessary parameters for training.
+            model_class (optional): The class of the model to be trained.
+            training_dataset (Dataset, optional): Dataset for training the model.
+            valid_dataset (Dataset, optional): Dataset for validating the model.
+            test_dataset (Dataset, optional): Dataset for testing the model.
+            collate_fn (Callable, optional): Function to collate data samples into batches.
+            scalar (StandardScaler, optional): Scaler for standardizing input data.
+            **kwargs: Additional keyword arguments for configuration adjustments.
         """
         # make a deep copy of the config to avoid modifying the original config
         for k, v in kwargs.items():
             setattr(config, k, v)
 
         self._config = config
         self._model_class = model_class
@@ -107,19 +106,21 @@
         self._scheduler = None
         self._loss_fn = None
         self._timer = Timer(device=self._device)
 
         # --- initialize wandb ---
         if config.apply_wandb and config.wandb_api_key:
             wandb.login(key=config.wandb_api_key)
+        elif config.apply_wandb:  # use default login if not specified
+            wandb.login()
 
         wandb.init(
             project=config.wandb_project,
             name=config.wandb_name,
-            config=config.__dict__,
+            config=config.to_dict(),
             mode="online" if config.apply_wandb else "disabled",
         )
 
         # Validation variables and flags
         self._valid_metric = (
             EVAL_METRICS[config.dataset_name].replace("-", "_") if not config.eval_metric else config.eval_metric
         )
@@ -158,130 +159,142 @@
         self._backbone_frozen = False
 
         # normalize training dataset labels for regression task
         self.standardize_training_lbs()
 
         # initialize training modules
         # self.initialize()
+        self._init_args = None
+        self._init_kwargs = None
 
     @property
     def model(self):
-        """
-        Retrieve the scaled model if available, else return the base model.
+        """Retrieves the scaled model if available, otherwise returns the base model.
 
-        Returns
-        -------
-        torch.nn.Module
-            The model (possibly scaled).
+        Returns:
+            torch.nn.Module: The model, potentially after applying temperature scaling.
         """
         if self._ts_model:
             return self._ts_model
         return self._model
 
     @property
     def config(self):
-        """
-        Retrieve the configuration of the Trainer.
+        """Retrieves the configuration of the Trainer.
 
-        Returns
-        -------
-        Config
-            The configuration object.
+        Returns:
+            Config: The configuration object used by the Trainer.
         """
         return self._config
 
     @property
     def n_model_parameters(self):
-        """
-        Compute the total number of trainable parameters in the model.
+        """Computes the total number of trainable parameters in the model.
 
-        Returns
-        -------
-        int
-            Total number of trainable parameters.
+        Returns:
+            int: Total number of trainable parameters.
         """
         return sum(p.numel() for p in self.model.parameters() if p.requires_grad)
 
     @property
     def n_update_steps_per_epoch(self):
-        """
-        Calculate the number of update steps required per epoch, based on
-        the size of the training dataset and batch size.
+        """Calculates the number of update steps required per epoch.
+
+        This is based on the size of the training dataset and the configured batch size.
 
-        Returns
-        -------
-        int
-            Number of update steps per epoch.
+        Returns:
+            int: Number of update steps per epoch.
         """
         return int(np.ceil(len(self._training_dataset) / self.config.batch_size))
 
     @property
     def backbone_params(self):
-        """
-        Retrieve the parameters of the model's backbone (excluding the output layer).
+        """Retrieves parameters of the model's backbone, excluding the output layer.
 
-        Returns
-        -------
-        list
-            List of parameters of the model's backbone.
+        Useful for operations that need to differentiate between backbone and output layer parameters,
+        such as freezing the backbone during training.
+
+        Returns:
+            list: Parameters of the model's backbone.
         """
         output_param_ids = [id(x[1]) for x in self._model.named_parameters() if "output_layer" in x[0]]
         backbone_params = list(
             filter(
                 lambda p: id(p) not in output_param_ids,
                 self._model.parameters(),
             )
         )
         return backbone_params
 
     def initialize(self, *args, **kwargs):
-        """
-        Initialize the trainer's status and its key components including the model,
+        """Initializes the trainer's status and its key components including the model,
         optimizer, learning rate scheduler, and loss function.
 
-        Returns
-        -------
-        self : Trainer
-            Initialized Trainer instance.
+        This method sets up the training environment by initializing the model, optimizer,
+        learning rate scheduler, and the loss function based on the provided configuration.
+        It also prepares the trainer for logging and checkpointing mechanisms.
+
+        Args:
+            *args: Variable length argument list for model initialization.
+            **kwargs: Arbitrary keyword arguments for model initialization.
+
+        Returns:
+            Trainer: The initialized Trainer instance ready for training.
         """
         self.initialize_model(*args, **kwargs)
-        self.initialize_optimizer()
+        self.initialize_optimizer(*args, **kwargs)
         self.initialize_scheduler()
         self.initialize_loss()
         self._timer.init()
         self._status.init()
         self._checkpoint_container = CheckpointContainer(self._update_criteria)
 
         if self.config.freeze_backbone:
             self.freeze_backbone()
 
         logger.info(f"Trainer initialized. The model contains {self.n_model_parameters} parameters")
+
+        self._init_args = args
+        self._init_kwargs = kwargs
+
         return self
 
-    def initialize_model(self, *args, **kwargs):
+    def re_initialize(self):
+        """Reinitializes the trainer's status and key components. Designed for Deep Ensembles.
+
+        Returns:
+            Trainer: The reinitialized Trainer instance.
         """
-        Abstract method to initialize the model. Implementations are expected in
-        subclasses of Trainer.
+        return self.initialize(*self._init_args, **self._init_kwargs)
+
+    def initialize_model(self, *args, **kwargs):
+        """Abstract method to initialize the model.
 
-        Raises
-        ------
-        NotImplementedError
-            If the method is not implemented.
+        This method should be implemented in subclasses of Trainer, providing the specific
+        logic to initialize the model that will be used for training.
+
+        Returns:
+            Trainer: The Trainer instance with the model initialized.
         """
         self._model = self._model_class(*args, **kwargs)
+        return self
 
     def initialize_optimizer(self, *args, **kwargs):
-        """
-        Initialize the model's optimizer based on the set configurations.
-        Special handling is provided for SGLD-based uncertainty methods.
+        """Initializes the model's optimizer based on the set configurations.
+
+        This method sets up the optimizer for the model's parameters. It includes special
+        handling for SGLD-based uncertainty methods by differentiating between backbone
+        and output layer parameters.
+
+        Args:
+            *args: Variable length argument list for optimizer initialization.
+            **kwargs: Arbitrary keyword arguments for optimizer initialization.
 
-        Returns
-        -------
-        self : Trainer
-            Updated Trainer instance with initialized optimizer.
+        Returns:
+            Trainer: The Trainer instance with the initialized optimizer.
         """
         params = [p for p in self.model.parameters() if p.requires_grad]
         self._optimizer = AdamW(params, lr=self._status.lr)
 
         # for sgld compatibility
         if self.config.uncertainty_method == UncertaintyMethods.sgld:
             output_param_ids = [id(x[1]) for x in self._model.named_parameters() if "output_layer" in x[0]]
@@ -298,49 +311,46 @@
                 lr=self._status.lr,
                 norm_sigma=self.config.sgld_prior_sigma,
             )
 
         return self
 
     def initialize_scheduler(self):
-        """
-        Initialize the learning rate scheduler based on the number of training steps
-        and the specified warmup ratio.
+        """Initializes the learning rate scheduler based on the training configuration.
 
-        Returns
-        -------
-        self : Trainer
-            Updated Trainer instance with initialized scheduler.
+        This method sets up the learning rate scheduler using the total number of training
+        steps and the specified warmup ratio.
+
+        Returns:
+            Trainer: The Trainer instance with the initialized scheduler.
         """
         n_training_steps = int(np.ceil(self.n_update_steps_per_epoch * self._status.n_epochs))
         n_warmup_steps = int(np.ceil(n_training_steps * self.config.warmup_ratio))
 
         self._scheduler = get_scheduler(
             self._status.lr_scheduler_type,
             self._optimizer,
             num_warmup_steps=n_warmup_steps,
             num_training_steps=n_training_steps,
         )
         return self
 
     def initialize_loss(self, disable_focal_loss=False):
-        """
-        Initialize the loss function based on the task type and uncertainty method
-        specified in the configuration.
+        """Initializes the loss function based on the task type and specified uncertainty method.
 
-        Parameters
-        ----------
-        disable_focal_loss : bool, optional
-            If True, disables the use of focal loss, even if the uncertainty method
-            specifies it. Defaults to False.
-
-        Returns
-        -------
-        self : Trainer
-            Updated Trainer instance with initialized loss function.
+        This method sets up the appropriate loss function for the training process, considering
+        the task type (classification or regression) and whether any specific uncertainty
+        methods (e.g., evidential or focal loss) are applied.
+
+        Args:
+            disable_focal_loss (bool, optional): If True, disables the use of focal loss, even if
+                                                 specified by the uncertainty method. Defaults to False.
+
+        Returns:
+            Trainer: The Trainer instance with the initialized loss function.
         """
         # Notice that the reduction should always be 'none' here for the following masking operation
         if self.config.task_type == "classification":
             # evidential classification
             if self.config.uncertainty_method == UncertaintyMethods.evidential:
                 self._loss_fn = EvidentialClassificationLoss(
                     n_classes=2 if self.config.n_lbs == 1 else self.config.n_lbs,
@@ -375,22 +385,21 @@
         return self._valid_dataset
 
     @property
     def test_dataset(self):
         return self._test_dataset
 
     def standardize_training_lbs(self):
-        """
-        Standardize the label distribution of the training dataset to a standerd Gaussian
-        distribution. This function is applicable only for regression tasks.
+        """Standardizes the label distribution of the training dataset for regression tasks.
+
+        This method applies standardization to the labels of the training dataset, transforming
+        them to a standard Gaussian distribution. It's applicable only for regression tasks.
 
-        Returns
-        -------
-        self : Trainer
-            Updated Trainer instance with standardized training labels.
+        Returns:
+            Trainer: The Trainer instance with standardized training labels.
         """
         if self.config.task_type == "classification":
             return self
 
         if self._training_dataset is None and self._scaler is None:
             logger.warning(
                 "Encounter regression task with no training dataset specified and label scaling disabled! "
@@ -423,27 +432,25 @@
         """
         The number of total validation steps
         """
         n_steps_per_epoch = int(np.ceil(len(self._valid_dataset) / self.config.batch_size))
         return n_steps_per_epoch * self._status.n_epochs
 
     def set_mode(self, mode: str):
-        """
-        Set the training mode for the model. Depending on the mode, the model
-        can either be set to training, evaluation, or testing.
+        """Sets the training mode for the model.
+
+        Depending on the mode, the model is set to training, evaluation, or testing. This method
+        is essential for correctly configuring the model's state for different phases of the
+        training and evaluation process.
 
-        Parameters
-        ----------
-        mode : str
-            Mode to set the model into. Should be one of 'train', 'eval', or 'test'.
-
-        Returns
-        -------
-        self : Trainer
-            Updated Trainer instance with the model set to the specified mode.
+        Args:
+            mode (str): The mode to set the model to. Should be one of 'train', 'eval', or 'test'.
+
+        Returns:
+            Trainer: The Trainer instance with the model set to the specified mode.
         """
 
         if mode == "train":
             self.model.train()
 
         elif mode == "eval":
             self.model.eval()
@@ -458,21 +465,22 @@
                         m.train()
         else:
             raise ValueError(f"Argument `mode` should be 'train', 'eval' or 'test'.")
 
         return self
 
     def run(self):
-        """
-        Execute the training and evaluation process based on the specified uncertainty
-        method. This method serves as the main entry point for the entire training process.
+        """Executes the training and evaluation process.
+
+        This method serves as the main entry point for the training process, orchestrating the
+        execution based on the specified uncertainty method. It handles different training
+        strategies like ensembles, SWAG, temperature scaling, and more.
 
-        Returns
-        -------
-        None
+        Returns:
+            None
         """
 
         # deep ensembles
         if self.config.uncertainty_method == UncertaintyMethods.ensembles:
             self.run_ensembles()
         # swag
         elif self.config.uncertainty_method == UncertaintyMethods.swag:
@@ -496,142 +504,140 @@
         wandb.finish()
 
         logger.info("Done.")
 
         return None
 
     def run_single_shot(self, apply_test=True):
-        """
-        Run the training and evaluation pipeline for a single iteration.
+        """Runs the training and evaluation pipeline for a single iteration.
+
+        This method handles the process of training the model and optionally evaluating it on a test dataset.
+        It is designed for a straightforward, single iteration of training and testing.
 
-        Parameters
-        ----------
-        apply_test : bool, optional
-            Whether to run the test function as part of the process. Default is True.
-
-        Returns
-        -------
-        Trainer
-            Self reference to the Trainer object.
+        Args:
+            apply_test (bool, optional): Whether to run the test function as part of the process. Defaults to True.
+
+        Returns:
+            Trainer: Self reference to the Trainer object, allowing for method chaining.
         """
 
         set_seed(self.config.seed)
         if not self.load_checkpoint():
             logger.info("Training model")
             self.train()
 
         if apply_test:
             test_metrics = self.test()
-            logger.info("[Single Shot] Test results:")
-            self.log_results(test_metrics)
-
-            # log results to wandb
-            for k, v in test_metrics.items():
-                wandb.run.summary[f"test-single_shot/{k}"] = v
+            if test_metrics is not None:
+                logger.info("[Single Shot] Test results:")
+                self.log_results(test_metrics)
+
+                # log results to wandb
+                for k, v in test_metrics.items():
+                    wandb.run.summary[f"test-single_shot/{k}"] = v
 
             if self.config.test_on_training_data:
                 logger.info("[Single Shot] Testing on training data.")
                 self.test_on_training_data()
 
         self.save_checkpoint()
 
         return self
 
     def run_ensembles(self):
-        """
-        Train and evaluate an ensemble of models.
-        This is primarily used for uncertainty estimation through model ensembles.
+        """Trains and evaluates an ensemble of models.
+
+        This method is used for uncertainty estimation through model ensembles, training multiple
+        models with different seeds and evaluating their collective performance.
 
-        Returns
-        -------
-        Trainer
-            Self reference to the Trainer object.
+        Returns:
+            Trainer: Self reference to the Trainer object, allowing for method chaining.
         """
 
         for ensemble_idx in range(self.config.n_ensembles):
             # update random seed and re-initialize training status
             individual_seed = self.config.seed + ensemble_idx
 
             del self._model
             set_seed(individual_seed)
-            self.initialize()
+            self.re_initialize()
             logger.info(f"[Ensemble {ensemble_idx}] seed: {individual_seed}")
 
             # update result dir
-            self._status.result_dir = op.join(
-                op.dirname(op.normpath(self._status.result_dir)),
+            self._status.result_dir = osp.join(
+                osp.dirname(osp.normpath(self._status.result_dir)),
                 f"seed-{individual_seed}",
             )
-            self._status.result_dir_no_uncertainty = op.join(
-                op.dirname(op.normpath(self._status.result_dir_no_uncertainty)),
+            self._status.result_dir_no_uncertainty = osp.join(
+                osp.dirname(osp.normpath(self._status.result_dir_no_uncertainty)),
                 f"seed-{individual_seed}",
             )
 
             if not self.load_checkpoint():
                 logger.info("Training model")
                 self.train()
 
             test_metrics = self.test()
-            logger.info(f"[Ensemble {ensemble_idx}] Test results:")
-            self.log_results(test_metrics)
-
-            # log results to wandb
-            for k, v in test_metrics.items():
-                wandb.run.summary[f"test-ensemble_{ensemble_idx}/{k}"] = v
+            if test_metrics is not None:
+                logger.info(f"[Ensemble {ensemble_idx}] Test results:")
+                self.log_results(test_metrics)
+
+                # log results to wandb
+                for k, v in test_metrics.items():
+                    wandb.run.summary[f"test-ensemble_{ensemble_idx}/{k}"] = v
 
             if self.config.test_on_training_data:
                 logger.info(f"[Ensemble {ensemble_idx}] Testing on training data.")
                 self.test_on_training_data()
 
             self.save_checkpoint()
 
         return self
 
     def run_swag(self):
-        """
-        Execute the training and evaluation pipeline using the SWAG (Stochastic Weight Averaging Gaussian)
-        method for uncertainty estimation.
+        """Executes the training and evaluation pipeline using the SWAG method.
 
-        Returns
-        -------
-        Trainer
-            Self reference to the Trainer object.
+        Stochastic Weight Averaging Gaussian (SWAG) is used for uncertainty estimation. This method
+        involves training the model with early stopping and applying SWAG for post-training uncertainty
+        estimation.
+
+        Returns:
+            Trainer: Self reference to the Trainer object, allowing for method chaining.
         """
 
         # Train the model with early stopping.
         self.run_single_shot(apply_test=False)
         self._load_model_state_dict()
 
         logger.info("SWA session start")
         self.swa_session()
 
         test_metrics = self.test(load_best_model=False)
-        logger.info("[SWAG] Test results:")
-        self.log_results(test_metrics)
+        if test_metrics is not None:
+            logger.info("[SWAG] Test results:")
+            self.log_results(test_metrics)
 
-        # log results to wandb
-        for k, v in test_metrics.items():
-            wandb.run.summary[f"test-swag/{k}"] = v
+            # log results to wandb
+            for k, v in test_metrics.items():
+                wandb.run.summary[f"test-swag/{k}"] = v
 
         if self.config.test_on_training_data:
             logger.info("[SWAG] Testing on training data.")
             self.test_on_training_data(load_best_model=False)
 
         return self
 
     def swa_session(self):
-        """
-        Execute the SWA session. This function should be inherited by
-        child classes if special handling for optimizer or model initialization
-        if required.
-
-        Returns
-        -------
-        Trainer
-            Self reference to the Trainer object.
+        """Executes the SWA session.
+
+        This method is intended to be overridden by child classes for specialized handling of
+        optimizer or model initialization required by SWA (Stochastic Weight Averaging).
+
+        Returns:
+            Trainer: Self reference to the Trainer object, allowing for method chaining.
         """
         # update hyper parameters
         self._status.lr *= self.config.swa_lr_decay
         self._status.lr_scheduler_type = "constant"
         self._status.n_epochs = self.config.n_swa_epochs
         # Can also set this to None; disable validation
         self._status.valid_epoch_interval = 0
@@ -647,52 +653,52 @@
         )
 
         logger.info("Training model")
         self.train()
         return self
 
     def run_temperature_scaling(self):
-        """
-        Execute the training and evaluation pipeline with temperature scaling as a post-processing step.
+        """Executes the training and evaluation pipeline with temperature scaling.
+
+        Temperature scaling is applied as a post-processing step to calibrate the confidence of the model's predictions.
 
-        Returns
-        -------
-        Trainer
-            Self reference to the Trainer object.
+        Returns:
+            Trainer: Self reference to the Trainer object, allowing for method chaining.
         """
 
         # Train the model with early stopping.
         self.run_single_shot(apply_test=False)
         self._load_model_state_dict()
 
         logger.info("Temperature Scaling session start.")
         self.ts_session()
 
         test_metrics = self.test(load_best_model=False)
-        logger.info("[Temperature Scaling] Test results:")
-        self.log_results(test_metrics)
+        if test_metrics is not None:
+            logger.info("[Temperature Scaling] Test results:")
+            self.log_results(test_metrics)
 
-        # log results to wandb
-        for k, v in test_metrics.items():
-            wandb.run.summary[f"test-temperature_scaling/{k}"] = v
+            # log results to wandb
+            for k, v in test_metrics.items():
+                wandb.run.summary[f"test-temperature_scaling/{k}"] = v
 
         if self.config.test_on_training_data:
             logger.info("[Temperature Scaling] Testing on training data.")
             self.test_on_training_data(load_best_model=False)
 
         return self
 
     def ts_session(self):
-        """
-        Execute the temperature scaling session.
+        """Executes the temperature scaling session.
+
+        This session involves retraining the model on the validation set with a modified learning rate and
+        epochs to apply temperature scaling for model calibration.
 
-        Returns
-        -------
-        Trainer
-            Self reference to the Trainer object.
+        Returns:
+            Trainer: Self reference to the Trainer object, allowing for method chaining.
         """
         # update hyper parameters
         self._status.lr = self.config.ts_lr
         self._status.lr_scheduler_type = "constant"
         self._status.n_epochs = self.config.n_ts_epochs
         self._status.valid_epoch_interval = 0  # Can also set this to None; disable validation
 
@@ -706,22 +712,21 @@
 
         logger.info("Training model on validation")
         self.train(use_valid_dataset=True)
         self.unfreeze()
         return self
 
     def run_iso_calibration(self):
-        """
-        Perform isotonic calibration as described in the paper:
-        'Accurate Uncertainties for Deep Learning Using Calibrated Regression'.
+        """Performs isotonic calibration.
+
+        Isotonic calibration is applied to calibrate the uncertainties of the model's predictions,
+        based on the approach described in 'Accurate Uncertainties for Deep Learning Using Calibrated Regression'.
 
-        Returns
-        -------
-        Trainer
-            Self reference to the Trainer object.
+        Returns:
+            Trainer: Self reference to the Trainer object, allowing for method chaining.
         """
         # Train the model with early stopping.
         self.run_single_shot(apply_test=False)
         self._load_model_state_dict()
 
         logger.info("Isotonic calibration session start.")
 
@@ -733,93 +738,92 @@
 
         mean_test, var_test = self.inverse_standardize_preds(self.process_logits(self.inference(self.test_dataset)))
         iso_calibrator.calibrate(mean_test, var_test, self.test_dataset.lbs, self.test_dataset.masks)
 
         return self
 
     def run_focal_loss(self):
-        """
-        Run the training and evaluation pipeline utilizing the focal loss.
-        Temperature scaling can be applied post-training if specified in the configuration.
+        """Runs the training and evaluation pipeline utilizing focal loss.
 
-        Returns
-        -------
-        Trainer
-            Self reference to the Trainer object.
+        Focal loss is used to address class imbalance by focusing more on hard-to-classify examples.
+        Temperature scaling can optionally be applied after training with focal loss.
+
+        Returns:
+            Trainer: Self reference to the Trainer object, allowing for method chaining.
         """
         # Train the model with early stopping. Do not need to load state dict as it is done during test
         self.run_single_shot()
 
         if self.config.apply_temperature_scaling_after_focal_loss:
             logger.info("[Focal Loss] Temperature Scaling session start.")
             self.ts_session()
 
             test_metrics = self.test(load_best_model=False)
-            logger.info("[Temperature Scaling] Test results:")
-            self.log_results(test_metrics)
 
-            # log results to wandb
-            for k, v in test_metrics.items():
-                wandb.run.summary[f"test-temperature_scaling/{k}"] = v
+            if test_metrics is not None:
+                logger.info("[Temperature Scaling] Test results:")
+                self.log_results(test_metrics)
+
+                # log results to wandb
+                for k, v in test_metrics.items():
+                    wandb.run.summary[f"test-temperature_scaling/{k}"] = v
 
             if self.config.test_on_training_data:
                 logger.info("[Temperature Scaling] Testing on training data.")
                 self.test_on_training_data(load_best_model=False)
 
         return self
 
     def run_sgld(self):
-        """
-        Execute the training and evaluation procedures with Stochastic Gradient Langevin Dynamics (SGLD)
-        for uncertainty estimation.
+        """Executes training and evaluation with Stochastic Gradient Langevin Dynamics (SGLD).
 
-        Returns
-        -------
-        Trainer
-            Self reference to the Trainer object.
+        SGLD is used for uncertainty estimation, incorporating random noise into the gradients to
+        explore the model's parameter space more broadly.
+
+        Returns:
+            Trainer: Self reference to the Trainer object, allowing for method chaining.
         """
         self.run_single_shot(apply_test=False)
         self._load_model_state_dict()
 
         logger.info("Langevin Dynamics session start.")
         self._sgld_model_buffer = list()
         self._status.n_epochs = self.config.n_langevin_samples * self.config.sgld_sampling_interval
         self._status.valid_epoch_interval = 0  # Can also set this to None; disable validation
 
         logger.info("Training model")
         self.train()
 
         test_metrics = self.test(load_best_model=False)
-        logger.info("[SGLD] Test results:")
-        self.log_results(test_metrics)
+        if test_metrics is not None:
+            logger.info("[SGLD] Test results:")
+            self.log_results(test_metrics)
 
-        # log results to wandb
-        for k, v in test_metrics.items():
-            wandb.run.summary[f"test-sgld/{k}"] = v
+            # log results to wandb
+            for k, v in test_metrics.items():
+                wandb.run.summary[f"test-sgld/{k}"] = v
 
         if self.config.test_on_training_data:
             logger.info("[SGLD] Testing on training data.")
             self.test_on_training_data(load_best_model=False)
 
         return self
 
     def train(self, use_valid_dataset=False):
-        """
-        Execute the training process for the model.
+        """Executes the training process for the model.
+
+        Optionally allows for training using the validation dataset instead of the training dataset.
+        This option can be useful for certain model calibration techniques like temperature scaling.
+
+        Args:
+            use_valid_dataset (bool, optional): Determines if the validation dataset should be used
+                for training instead of the training dataset. Defaults to False.
 
-        Parameters
-        ----------
-        use_valid_dataset : bool, optional
-            Determines if the validation dataset should be used for training.
-            This can be set to True during processes like temperature scaling.
-            Default is False.
-
-        Returns
-        -------
-        None
+        Returns:
+            None: This method returns None.
         """
 
         self.model.to(self._device)
         self.training_dataset.toggle_standardized_lbs(True)
         data_loader = self.get_dataloader(
             self.training_dataset if not use_valid_dataset else self.valid_dataset,
             shuffle=True,
@@ -861,26 +865,24 @@
                 self._status.n_eval_no_improve = 0
                 break
 
         self.training_dataset.toggle_standardized_lbs()
         return None
 
     def training_epoch(self, data_loader):
-        """
-        Perform a single epoch of training for the model using the provided data loader.
+        """Performs a single epoch of training using the provided data loader.
+
+        This method iterates over the data loader, performs the forward pass, computes the loss,
+        and updates the model parameters.
 
-        Parameters
-        ----------
-        data_loader : DataLoader
-            DataLoader object that provides batches of training data.
-
-        Returns
-        -------
-        float
-            Average training loss for the epoch.
+        Args:
+            data_loader (DataLoader): DataLoader object providing batches of training data.
+
+        Returns:
+            float: The average training loss for the epoch.
         """
 
         self.set_mode("train")
         self.model.to(self._device)
 
         total_loss = 0.0
         n_instances = 0
@@ -917,33 +919,26 @@
 
         self._status.train_log_idx += 1
         avg_loss = total_loss / n_instances
 
         return avg_loss
 
     def get_loss(self, logits, batch, n_steps_per_epoch=None) -> torch.Tensor:
-        """
-        Compute the loss for a batch of data. This function can be overridden
-        by child trainers to implement custom loss computation logic.
+        """Computes the loss for a batch of data.
+
+        This method can be overridden by subclasses to implement custom loss computation logic.
 
-        Parameters
-        ----------
-        logits : torch.Tensor
-            The predictions or logits produced by the model for the given batch.
-        batch : Batch
-            The batch of training data.
-        n_steps_per_epoch : int, optional
-            Represents the number of batches in a training epoch. This is used
-            specifically when uncertainty method is Bayesian Backpropagation (BBP).
-            Default is None.
-
-        Returns
-        -------
-        torch.Tensor
-            The computed loss for the batch.
+        Args:
+            logits (torch.Tensor): The predictions or logits produced by the model for the given batch.
+            batch (Batch): The batch of training data.
+            n_steps_per_epoch (int, optional): Represents the number of batches in a training epoch,
+                used specifically for certain uncertainty methods like Bayesian Backpropagation (BBP).
+
+        Returns:
+            torch.Tensor: The computed loss for the batch.
         """
 
         # modify data shapes to accommodate different tasks
         lbs, masks = (
             batch.lbs,
             batch.masks,
         )  # so that we don't mess up batch instances
@@ -973,28 +968,22 @@
 
         # for bbp
         if self.config.uncertainty_method == UncertaintyMethods.bbp and n_steps_per_epoch is not None:
             loss += self.model.output_layer.kld / n_steps_per_epoch / len(batch)
         return loss
 
     def inference(self, dataset, **kwargs):
-        """
-        Conduct inference over an entire dataset using the model.
+        """Conducts inference over an entire dataset using the model.
 
-        Parameters
-        ----------
-        dataset : Dataset
-            The dataset for which inference needs to be performed.
-        **kwargs
-            Additional keyword arguments.
-
-        Returns
-        -------
-        numpy.ndarray
-            Model outputs as logits or tuple of logits.
+        Args:
+            dataset (Dataset): The dataset for which inference needs to be performed.
+            **kwargs: Additional keyword arguments.
+
+        Returns:
+            numpy.ndarray: The model outputs as logits or a tuple of logits.
         """
 
         dataloader = self.get_dataloader(dataset, batch_size=self.config.batch_size_inference, shuffle=False)
         self.model.to(self._device)
 
         logits_list = list()
 
@@ -1006,26 +995,22 @@
                 logits_list.append(logits.detach().cpu())
 
         logits = torch.cat(logits_list, dim=0).numpy()
 
         return logits
 
     def process_logits(self, logits: np.ndarray) -> Union[np.ndarray, Tuple[np.ndarray, np.ndarray]]:
-        """
-        Process the output logits based on the training tasks or variants.
+        """Processes the output logits based on the training tasks or variants.
+
+        Args:
+            logits (numpy.ndarray): The raw logits produced by the model.
 
-        Parameters
-        ----------
-        logits : numpy.ndarray
-            The raw logits produced by the model.
-
-        Returns
-        -------
-        numpy.ndarray or Tuple[numpy.ndarray, numpy.ndarray]
-            Processed logits or tuple containing processed logits based on the task type.
+        Returns:
+            numpy.ndarray or Tuple[numpy.ndarray, numpy.ndarray]: Processed logits or a tuple containing
+            processed logits based on the task type.
         """
 
         if self.config.task_type == "classification":
             if self.config.uncertainty_method == UncertaintyMethods.evidential:
                 logits = logits.reshape((-1, self.config.n_tasks, self.config.n_lbs))
 
                 evidence = logits * (logits > 0)  # relu
@@ -1059,26 +1044,22 @@
 
         else:
             raise ValueError(f"Unrecognized task type: {self.config.task_type}")
 
     def inverse_standardize_preds(
         self, preds: Union[np.ndarray, Tuple[np.ndarray, np.ndarray]]
     ) -> Union[np.ndarray, Tuple[np.ndarray, np.ndarray]]:
-        """
-        Transform predictions back to their original scale if they have been standardized.
+        """Transforms predictions back to their original scale if they have been standardized.
+
+        Args:
+            preds (numpy.ndarray or Tuple[numpy.ndarray, numpy.ndarray]): Model predictions, can either be a single
+                array or a tuple containing two arrays for mean and variance, respectively.
 
-        Parameters
-        ----------
-        preds : numpy.ndarray or Tuple[numpy.ndarray, numpy.ndarray]
-            Model predictions. Can either be a single array or tuple containing two arrays.
-
-        Returns
-        -------
-        numpy.ndarray or Tuple[numpy.ndarray, numpy.ndarray]
-            Inverse-standardized predictions.
+        Returns:
+            numpy.ndarray or Tuple[numpy.ndarray, numpy.ndarray]: Inverse-standardized predictions.
         """
         if self._scaler is None:
             return preds
 
         if isinstance(preds, np.ndarray):
             return self._scaler.inverse_transform(preds)
         elif isinstance(preds, tuple):
@@ -1089,30 +1070,24 @@
 
     def evaluate(
         self,
         dataset,
         n_run: Optional[int] = 1,
         return_preds: Optional[bool] = False,
     ):
-        """
-        Evaluate the model's performance on the given dataset.
+        """Evaluates the model's performance on the given dataset.
 
-        Parameters
-        ----------
-        dataset : Dataset
-            The dataset to evaluate the model on.
-        n_run : int, optional
-            Number of runs for evaluation, default is 1.
-        return_preds : bool, optional
-            Whether to return the predictions along with metrics, default is False.
-
-        Returns
-        -------
-        dict or (dict, numpy.ndarray or Tuple[numpy.ndarray, numpy.ndarray])
-            Evaluation metrics or tuple containing metrics and predictions based on `return_preds`.
+        Args:
+            dataset (Dataset): The dataset to evaluate the model on.
+            n_run (int, optional): Number of runs for evaluation. Defaults to 1.
+            return_preds (bool, optional): Whether to return the predictions along with metrics. Defaults to False.
+
+        Returns:
+            dict, or (dict, numpy.ndarray or Tuple[numpy.ndarray, numpy.ndarray]): Evaluation metrics, or tuple
+            containing metrics and predictions based on `return_preds`.
         """
         if self._sgld_model_buffer is not None and len(self._sgld_model_buffer) > 0:
             n_run = len(self._sgld_model_buffer)
 
         if n_run == 1:
             preds = self.inverse_standardize_preds(self.process_logits(self.inference(dataset)))
             if isinstance(preds, np.ndarray):
@@ -1158,24 +1133,25 @@
             return metrics
         elif vars_array is None:
             return metrics, preds_array
         else:
             return metrics, (preds_array, vars_array)
 
     def eval_and_save(self):
-        """
-        Evaluate the model's performance on the validation dataset and save it
-        if its performance is better than previous evaluations.
+        """Evaluates the model's performance on the validation dataset and saves it if its performance is improved.
+
+        This method is part of the training loop where the model is periodically evaluated on the validation dataset,
+        and the best-performing model state is saved.
         """
         self.set_mode("eval")
 
         valid_results = self.evaluate(self.valid_dataset)
 
         result_dict = {f"valid/{k}": v for k, v in valid_results.items()}
-        wandb.log(data=result_dict, step=self._status.eval_log_idx)
+        wandb.log(data=result_dict, step=self._status.train_log_idx)
 
         logger.info(f"[Valid step {self._status.eval_log_idx}] results:")
         self.log_results(valid_results)
 
         # ----- check model performance and update buffer -----
         if self._checkpoint_container.check_and_update(self.model, valid_results[self._valid_metric]):
             self._status.n_eval_no_improve = 0
@@ -1183,29 +1159,28 @@
         else:
             self._status.n_eval_no_improve += 1
         self._status.eval_log_idx += 1
 
         return None
 
     def test(self, load_best_model=True, return_preds=False):
-        """
-        Test the model's performance on the test dataset.
+        """Tests the model's performance on the test dataset.
+
+        Args:
+            load_best_model (bool, optional): Whether to load the best model saved during training for testing. Defaults to True.
+            return_preds (bool, optional): Whether to return the predictions along with metrics. Defaults to False.
+
+        Returns:
+            dict, or tuple[dict, numpy.ndarray or Tuple[numpy.ndarray, numpy.ndarray]]: Evaluation metrics (and predictions)
+            for the test dataset.
+        """
+        if self.config.disable_test:
+            logger.warning("Test is disabled!")
+            return None
 
-        Parameters
-        ----------
-        load_best_model : bool, optional
-            Whether to load the best model saved during training for testing, default is True.
-        return_preds : bool, optional
-            Whether to return the predictions along with metrics, default is False.
-
-        Returns
-        -------
-        dict, tuple[dict, numpy.ndarray or Tuple[numpy.ndarray, numpy.ndarray]
-            Evaluation metrics (and predictions) for the test dataset.
-        """
         self.set_mode("test")
 
         if load_best_model and self._checkpoint_container.state_dict:
             self._load_model_state_dict()
 
         metrics, preds = self.evaluate(self._test_dataset, n_run=self.config.n_test, return_preds=True)
 
@@ -1220,40 +1195,47 @@
             variances = [None] * len(preds)
         elif isinstance(preds, tuple) and len(preds) == 2:
             preds, variances = preds
         else:
             raise ValueError("Unrecognized type or shape of `preds`.")
 
         for idx, (pred, variance) in enumerate(zip(preds, variances)):
-            file_path = op.join(self._status.result_dir, "preds", f"{idx}.pt")
+            if self.config.test_subset_ids_file_name:
+                subset_ids_file_name_no_ext = (
+                    osp.splitext(self.config.test_subset_ids_file_name)[0]
+                    if "." in self.config.test_subset_ids_file_name
+                    else self.config.test_subset_ids_file_name
+                )
+                file_path = osp.join(self._status.result_dir, f"preds-{subset_ids_file_name_no_ext}", f"{idx}.pt")
+            else:
+                file_path = osp.join(self._status.result_dir, "preds", f"{idx}.pt")
+
             self.save_results(
                 path=file_path,
                 preds=pred,
                 variances=variance,
                 lbs=self._test_dataset.lbs,
                 masks=self.test_dataset.masks,
             )
 
         return metrics
 
     def test_on_training_data(self, load_best_model=True, return_preds=False, disable_result_saving=False):
-        """
-        Test the model's performance on the training dataset.
+        """Tests the model's performance on the training dataset.
+
+        This method is useful for understanding the model's performance on the data it was trained on,
+        which can provide insights into overfitting or underfitting.
+
+        Args:
+            load_best_model (bool, optional): If True, loads the best model saved during training. Defaults to True.
+            return_preds (bool, optional): If True, returns the predictions along with the evaluation metrics. Defaults to False.
+            disable_result_saving (bool, optional): If True, disables saving the results to disk. Defaults to False.
 
-        Parameters
-        ----------
-        load_best_model : bool, optional
-            Whether to load the best model saved during training for testing, default is True.
-        return_preds : bool, optional
-            Whether to return the predictions along with metrics, default is False.
-
-        Returns
-        -------
-        dict, tuple[dict, numpy.ndarray or Tuple[numpy.ndarray, numpy.ndarray]
-            Evaluation metrics (and predictions) for the training dataset.
+        Returns:
+            dict, or tuple[dict, numpy.ndarray or Tuple[numpy.ndarray, numpy.ndarray]]: Evaluation metrics, or a tuple containing metrics and predictions if `return_preds` is True.
         """
         self.set_mode("test")
         self._training_dataset.use_full_dataset = True
         self._training_dataset.toggle_standardized_lbs(False)
 
         if load_best_model and self._checkpoint_container.state_dict:
             self._load_model_state_dict()
@@ -1273,44 +1255,39 @@
         elif isinstance(preds, tuple) and len(preds) == 2:
             means, variances = preds
         else:
             raise ValueError("Unrecognized type or shape of `preds`.")
 
         if not disable_result_saving:
             for idx, (mean, variance) in enumerate(zip(means, variances)):
-                file_path = op.join(self._status.result_dir, "preds-train", f"{idx}.pt")
+                file_path = osp.join(self._status.result_dir, "preds-train", f"{idx}.pt")
                 self.save_results(
                     path=file_path,
                     preds=mean,
                     variances=variance,
                     lbs=self._test_dataset.lbs,
                     masks=self.test_dataset.masks,
                 )
 
         self._training_dataset.use_full_dataset = False
 
         return (metrics, preds) if return_preds else metrics
 
     def get_metrics(self, lbs, preds, masks):
-        """
-        Calculate evaluation metrics based on the given labels, predictions, and masks.
+        """Calculates evaluation metrics based on the given labels, predictions, and masks.
+
+        This method computes the appropriate metrics based on the task type (classification or regression).
 
-        Parameters
-        ----------
-        lbs : numpy.ndarray
-            Ground truth labels.
-        preds : numpy.ndarray
-            Model predictions.
-        masks : numpy.ndarray
-            Masks indicating valid entries in labels and predictions.
-
-        Returns
-        -------
-        dict
-            Computed metrics for evaluation.
+        Args:
+            lbs (numpy.ndarray): Ground truth labels.
+            preds (numpy.ndarray): Model predictions.
+            masks (numpy.ndarray): Masks indicating valid entries in labels and predictions.
+
+        Returns:
+            dict: Computed metrics for evaluation.
         """
         if masks.shape[-1] == 1 and len(masks.shape) > 1:
             masks = masks.squeeze(-1)
         bool_masks = masks.astype(bool)
 
         if lbs.shape[-1] == 1 and len(lbs.shape) > 1:
             lbs = lbs.squeeze(-1)
@@ -1327,203 +1304,165 @@
         else:
             metrics = calculate_regression_metrics(lbs, preds, bool_masks, self._valid_metric)
 
         return metrics
 
     @staticmethod
     def log_results(metrics: dict, logging_func=logger.info):
-        """
-        Log evaluation metrics to the specified logging function.
+        """Logs evaluation metrics using the specified logging function.
+
+        Args:
+            metrics (dict): Dictionary containing evaluation metrics to be logged.
+            logging_func (function, optional): Logging function to which metrics will be sent. Defaults to `logger.info`.
 
-        Parameters
-        ----------
-        metrics : dict
-            Dictionary containing evaluation metrics to be logged.
-        logging_func : function, optional
-            Logging function to which metrics will be sent.
-            Defaults to `logger.info`.
-
-        Returns
-        -------
-        None
+        Returns:
+            None
         """
         for k, v in metrics.items():
             try:
                 logging_func(f"  {k}: {v:.4f}.")
             except TypeError:
                 pass
         return None
 
     def freeze(self):
-        """
-        Freeze all model parameters, preventing them from being updated during training.
+        """Freezes all model parameters, preventing them from being updated during training.
 
-        Returns
-        -------
-        Trainer
-            Returns the current instance with model parameters frozen.
+        Returns:
+            Trainer: The current instance with model parameters frozen.
         """
         for parameter in self.model.parameters():
             parameter.requires_grad = False
 
         self._model_frozen = True
         return self
 
     def unfreeze(self):
-        """
-        Unfreeze all model parameters, allowing them to be updated during training.
+        """Unfreezes all model parameters, allowing them to be updated during training.
 
-        Returns
-        -------
-        Trainer
-            Returns the current instance with model parameters unfrozen.
+        Returns:
+            Trainer: The current instance with model parameters unfrozen.
         """
         for parameter in self.model.parameters():
             parameter.requires_grad = True
 
         self._model_frozen = False
         return self
 
     def freeze_backbone(self):
-        """
-        Freeze the backbone parameters of the model, preventing them from being updated during training.
+        """Freezes the backbone parameters of the model, preventing them from being updated during training.
 
-        Returns
-        -------
-        Trainer
-            Returns the current instance with backbone parameters frozen.
+        Returns:
+            Trainer: The current instance with backbone parameters frozen.
         """
         for params in self.backbone_params:
             params.requires_grad = False
 
         self._backbone_frozen = True
         return self
 
     def unfreeze_backbone(self):
-        """
-        Unfreeze the backbone parameters of the model, allowing them to be updated during training.
+        """Unfreezes the backbone parameters of the model, allowing them to be updated during training.
 
-        Returns
-        -------
-        Trainer
-            Returns the current instance with backbone parameters unfrozen.
+        Returns:
+            Trainer: The current instance with backbone parameters unfrozen.
         """
         for params in self.backbone_params:
             params.requires_grad = True
 
         self._backbone_frozen = False
         return self
 
     def save_checkpoint(self):
-        """
-        Save the current model state as a checkpoint.
+        """Saves the current model state as a checkpoint.
 
-        If the `disable_result_saving` flag is set in the configuration,
-        a warning will be logged and no save operation will be performed.
+        This method checks the `disable_result_saving` configuration flag before saving. If saving is disabled,
+        it logs a warning and does not perform the save operation.
 
-        Returns
-        -------
-        Trainer
-            Returns the current instance after attempting to save the model checkpoint.
+        Returns:
+            Trainer: The current instance after attempting to save the model checkpoint.
         """
         if not self.config.disable_result_saving:
             init_dir(self._status.result_dir, clear_original_content=False)
-            self._checkpoint_container.save(op.join(self._status.result_dir, self._status.model_name))
+            self._checkpoint_container.save(osp.join(self._status.result_dir, self._status.model_name))
         else:
             logger.warning("Model is not saved because of `disable_result_saving` flag is set to `True`.")
 
         return self
 
     def _load_model_state_dict(self):
-        """
-        Private method to load the model state dictionary from the checkpoint container.
+        """Loads the model state dictionary from the checkpoint container.
 
-        If the `freeze_backbone` flag is set in the configuration, the backbone will be frozen after loading.
+        This private method is used internally to load model parameters from a saved checkpoint. If the `freeze_backbone`
+        configuration flag is set, the backbone parameters are frozen after loading.
 
-        Returns
-        -------
-        Trainer
-            Returns the current instance with the model state loaded.
+        Returns:
+            Trainer: The current instance with the model state loaded.
         """
         self._model.load_state_dict(self._checkpoint_container.state_dict)
         if self.config.freeze_backbone:
             self.freeze_backbone()
         return self
 
     def _load_from_container(self, model_path):
-        """
-        Private method to load a trained model from a given path.
+        """Loads a trained model from the specified path.
+
+        Args:
+            model_path (str): Path to the saved model.
 
-        Parameters
-        ----------
-        model_path : str
-            Path to the saved model.
-
-        Returns
-        -------
-        bool
-            Returns True if the model is successfully loaded, otherwise False.
+        Returns:
+            bool: True if the model is successfully loaded, otherwise False.
         """
-        if not op.exists(model_path):
+        if not osp.exists(model_path):
             return False
         logger.info(f"Loading trained model from {model_path}.")
         self._checkpoint_container.load(model_path)
         self._load_model_state_dict()
         self._model.to(self._device)
         return True
 
     def load_checkpoint(self):
-        """
-        Load the model from a checkpoint.
-        This function allows loading the checkpoint from the path where the model is trained without
-        the uncertainty estimation method. This is useful when the uncertainty estimation method can be
-        trained from the checkpoint.
-
-        Returns
-        -------
-        bool
-            Returns True if the model is successfully loaded from a checkpoint, otherwise False.
+        """Loads the model from a checkpoint.
+
+        This method attempts to load the model checkpoint from the configured path. It supports loading with and without
+        considering the uncertainty estimation method used during training.
+
+        Returns:
+            bool: True if the model is successfully loaded from a checkpoint, otherwise False.
         """
         if self.config.retrain_model:
             return False
 
         if not self.config.ignore_uncertainty_output:
-            model_path = op.join(self._status.result_dir, self._status.model_name)
+            model_path = osp.join(self._status.result_dir, self._status.model_name)
             if self._load_from_container(model_path):
                 return True
 
         if not self.config.ignore_no_uncertainty_output:
-            model_path = op.join(self._status.result_dir_no_uncertainty, self._status.model_name)
+            model_path = osp.join(self._status.result_dir_no_uncertainty, self._status.model_name)
             if self._load_from_container(model_path):
                 return True
 
         return False
 
     def get_dataloader(
         self,
         dataset,
         shuffle: Optional[bool] = False,
         batch_size: Optional[int] = 0,
     ):
-        """
-        Create a DataLoader for the provided dataset.
+        """Creates a DataLoader for the specified dataset.
+
+        Args:
+            dataset: Dataset for which the DataLoader is to be created.
+            shuffle (bool, optional): Whether to shuffle the data. Defaults to False.
+            batch_size (int, optional): Batch size for the DataLoader. Uses the batch size from the configuration if not specified.
 
-        Parameters
-        ----------
-        dataset : Dataset
-            Dataset for which the DataLoader is to be created.
-        shuffle : bool, optional
-            Whether to shuffle the data. Defaults to False.
-        batch_size : int, optional
-            Batch size for the DataLoader. If not provided, will use the batch size from the configuration.
-
-        Returns
-        -------
-        DataLoader
-            Returns the created DataLoader for the provided dataset.
+        Returns:
+            DataLoader: The created DataLoader for the provided dataset.
         """
         try:
             dataloader = DataLoader(
                 dataset=dataset,
                 collate_fn=self._collate_fn,
                 batch_size=batch_size if batch_size else self.config.batch_size,
                 num_workers=getattr(self.config, "num_workers", 0),
@@ -1533,145 +1472,31 @@
             )
         except Exception as e:
             logger.exception(e)
             raise e
 
         return dataloader
 
-    def save(
-        self,
-        output_dir: Optional[str] = None,
-        save_optimizer: Optional[bool] = False,
-        save_scheduler: Optional[bool] = False,
-        model_name: Optional[str] = "model.ckpt",
-        optimizer_name: Optional[str] = "optimizer.ckpt",
-        scheduler_name: Optional[str] = "scheduler.ckpt",
-    ):
-        """
-        Save model parameters as well as trainer parameters
-
-        Parameters
-        ----------
-        output_dir: model directory
-        save_optimizer: whether to save optimizer
-        save_scheduler: whether to save scheduler
-        model_name: model name (suffix free)
-        optimizer_name: optimizer name (suffix free)
-        scheduler_name: scheduler name (suffix free)
-
-        Returns
-        -------
-        None
-        """
-        output_dir = output_dir if output_dir is not None else self._status.result_dir
-
-        model_state_dict = self._model.state_dict()
-        torch.save(model_state_dict, op.join(output_dir, model_name))
-
-        self.config.save(output_dir)
-
-        if save_optimizer:
-            torch.save(
-                self._optimizer.state_dict(),
-                op.join(output_dir, optimizer_name),
-            )
-        if save_scheduler and self._scheduler is not None:
-            torch.save(
-                self._scheduler.state_dict(),
-                op.join(output_dir, scheduler_name),
-            )
-
-        return None
-
-    def load(
-        self,
-        input_dir: Optional[str] = None,
-        load_optimizer: Optional[bool] = False,
-        load_scheduler: Optional[bool] = False,
-        model_name: Optional[str] = "model.ckpt",
-        optimizer_name: Optional[str] = "optimizer.ckpt",
-        scheduler_name: Optional[str] = "scheduler.ckpt",
-    ):
-        """
-        Load model parameters.
-
-        Parameters
-        ----------
-        input_dir: model directory
-        load_optimizer: whether load other trainer parameters
-        load_scheduler: whether load scheduler
-        model_name: model name (suffix free)
-        optimizer_name: optimizer name (suffix free)
-        scheduler_name: scheduler name
-
-        Returns
-        -------
-        self
-        """
-        input_dir = input_dir if input_dir is not None else self._status.result_dir
-
-        logger.info(f"Loading model from {input_dir}")
-
-        self.initialize_model()
-        self._model.load_state_dict(torch.load(op.join(input_dir, model_name)))
-        self._model.to(self._device)
-
-        if load_optimizer:
-            logger.info("Loading optimizer")
-
-            if self._optimizer is None:
-                self.initialize_optimizer()
-
-            if op.isfile(op.join(input_dir, optimizer_name)):
-                self._optimizer.load_state_dict(
-                    torch.load(
-                        op.join(input_dir, optimizer_name),
-                        map_location=self._device,
-                    )
-                )
-            else:
-                logger.warning("Optimizer file does not exist!")
-
-        if load_scheduler:
-            logger.info("Loading scheduler")
-
-            if self._scheduler is None:
-                self.initialize_scheduler()
-
-            if op.isfile(op.join(input_dir, scheduler_name)):
-                self._optimizer.load_state_dict(
-                    torch.load(
-                        op.join(input_dir, scheduler_name),
-                        map_location=self._device,
-                    )
-                )
-            else:
-                logger.warning("Scheduler file does not exist!")
-        return self
-
     def save_results(self, path, preds, variances, lbs, masks):
-        """
-        Save results to disk in the specified format.
+        """Saves the model predictions, variances, ground truth labels, and masks to disk.
+
+        This method saves the results of model predictions to a specified path. It is capable of handling
+        both the predictions and their associated variances, along with the ground truth labels and masks that
+        indicate which data points should be considered in the analysis. If the configuration flag
+        `disable_result_saving` is set to True, the method will log a warning and not perform any saving operation.
+
+        Args:
+            path (str): The destination path where the results will be saved.
+            preds (array_like): The predictions generated by the model.
+            variances (array_like): The variances associated with each prediction, indicating the uncertainty of the predictions.
+            lbs (array_like): The ground truth labels against which the model's predictions can be evaluated.
+            masks (array_like): Masks indicating which data points are valid and should be considered in the evaluation.
 
-        Parameters
-        ----------
-        path : str
-            Destination path to save the results.
-        preds : array_like
-            Predictions from the model.
-        variances : array_like
-            Variance values associated with the predictions.
-        lbs : array_like
-            Ground truth labels.
-        masks : array_like
-            Masks associated with the data.
-
-        Returns
-        -------
-        None
+        Returns:
+            None: This method does not return any value.
         """
         if not self.config.disable_result_saving:
             save_results(path, preds, variances, lbs, masks)
         else:
             logger.warning("Results are not saved because `disable_result_saving` flag is set to `True`.")
 
         return None
```

### Comparing `muben-0.0.1/muben/train/trainer_grover.py` & `muben-0.0.2/muben/train/trainer_grover.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/train/trainer_unimol.py` & `muben-0.0.2/muben/train/trainer_unimol.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 # Author: Yinghao Li
-# Modified: February 28th, 2024
+# Modified: March 4th, 2024
 # ---------------------------------------
 # Description: Trainer function for Uni-Mol.
 """
 
 from abc import ABC
 
 import logging
@@ -21,15 +21,15 @@
 
 
 class Trainer(BaseTrainer, ABC):
     """
     Trainer class responsible for training and managing the Uni-Mol model.
     """
 
-    def initialize_optimizer(self):
+    def initialize_optimizer(self, *args, **kwargs):
         """
         Initialize the optimizer for the model.
 
         Depending on the uncertainty estimation method, it initializes
         either a standard AdamW optimizer or an SGLD optimizer.
         """
         # Original implementation seems set weight decay to 0, which is weird.
```

### Comparing `muben-0.0.1/muben/uncertainty/__init__.py` & `muben-0.0.2/muben/uncertainty/__init__.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/uncertainty/bbp.py` & `muben-0.0.2/muben/uncertainty/bbp.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/uncertainty/evidential/loss.py` & `muben-0.0.2/muben/uncertainty/evidential/loss.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/uncertainty/evidential/model.py` & `muben-0.0.2/muben/uncertainty/evidential/model.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/uncertainty/focal_loss.py` & `muben-0.0.2/muben/uncertainty/focal_loss.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/uncertainty/iso.py` & `muben-0.0.2/muben/uncertainty/iso.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/uncertainty/sgld.py` & `muben-0.0.2/muben/uncertainty/sgld.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/uncertainty/swag.py` & `muben-0.0.2/muben/uncertainty/swag.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/uncertainty/ts.py` & `muben-0.0.2/muben/uncertainty/ts.py`

 * *Files identical despite different names*

### Comparing `muben-0.0.1/muben/utils/chem.py` & `muben-0.0.2/muben/utils/chem.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 # Author: Yinghao Li
-# Modified: August 26th, 2023
+# Modified: February 29th, 2024
 # ---------------------------------------
 # Description: Molecular descriptors and features
 """
 
-
 import warnings
 import logging
 import numpy as np
 from rdkit import Chem, RDLogger
 from rdkit.Chem import AllChem
 
 RDLogger.DisableLog("rdApp.*")
@@ -24,106 +23,84 @@
     "atom_to_atom_ids",
     "rdkit_2d_features_normalized_generator",
     "morgan_binary_features_generator",
 ]
 
 
 def smiles_to_2d_coords(smiles):
-    """
-    Convert smiles to 2d coordinates
+    """Converts SMILES strings to 2D coordinates.
+
+    Args:
+        smiles (str): A SMILES string representing the molecule.
 
-    Parameters
-    ----------
-    smiles: smiles strings
-
-    Returns
-    -------
-    2d coordinates in numpy array
+    Returns:
+        numpy.ndarray: A 2D array of coordinates for the molecule.
     """
     mol = Chem.MolFromSmiles(smiles)
     mol = AllChem.AddHs(mol)
     AllChem.Compute2DCoords(mol)
     coordinates = mol.GetConformer().GetPositions().astype(np.float32)
-    assert len(mol.GetAtoms()) == len(
-        coordinates
-    ), f"2D coordinates shape is not align with {smiles}"
+    assert len(mol.GetAtoms()) == len(coordinates), f"2D coordinates shape is not align with {smiles}"
     return coordinates
 
 
 def smiles_to_3d_coords(smiles, n_conformer):
-    """
-    Convert smiles to 3d coordinates
+    """Converts SMILES strings to 3D coordinates.
+
+    Args:
+        smiles (str): A SMILES string representing the molecule.
+        n_conformer (int): Number of conformers to generate for the molecule.
 
-    Parameters
-    ----------
-    smiles: smiles strings
-    n_conformer: conformer num, default (uni-mol) all==11, 10 3d + 1 2d
-
-    Returns
-    -------
-    3d coordinates in list of numpy array
+    Returns:
+        list[numpy.ndarray]: A list of 3D arrays of coordinates for each conformer of the molecule.
     """
     mol = Chem.MolFromSmiles(smiles)
     mol = AllChem.AddHs(mol)
     coordinate_list = []
     for seed in range(n_conformer):
         coordinates = list()
         try:
             # will random generate conformer with seed equal to -1. else fixed random seed.
             res = AllChem.EmbedMolecule(mol, randomSeed=seed)
             if res == 0:
                 try:
-                    AllChem.MMFFOptimizeMolecule(
-                        mol
-                    )  # some conformer can not use MMFF optimize
+                    AllChem.MMFFOptimizeMolecule(mol)  # some conformer can not use MMFF optimize
                     coordinates = mol.GetConformer().GetPositions()
                 except Exception as e:
-                    logger.warning(
-                        f"Failed to generate 3D, replace with 2D: {e}"
-                    )
+                    logger.warning(f"Failed to generate 3D, replace with 2D: {e}")
                     coordinates = smiles_to_2d_coords(smiles)
 
             elif res == -1:
                 mol_tmp = Chem.MolFromSmiles(smiles)
-                AllChem.EmbedMolecule(
-                    mol_tmp, maxAttempts=5000, randomSeed=seed
-                )
+                AllChem.EmbedMolecule(mol_tmp, maxAttempts=5000, randomSeed=seed)
                 mol_tmp = AllChem.AddHs(mol_tmp, addCoords=True)
                 try:
-                    AllChem.MMFFOptimizeMolecule(
-                        mol_tmp
-                    )  # some conformer can not use MMFF optimize
+                    AllChem.MMFFOptimizeMolecule(mol_tmp)  # some conformer can not use MMFF optimize
                     coordinates = mol_tmp.GetConformer().GetPositions()
                 except Exception as e:
-                    logger.warning(
-                        f"Failed to generate 3D, replace with 2D: {e}"
-                    )
+                    logger.warning(f"Failed to generate 3D, replace with 2D: {e}")
                     coordinates = smiles_to_2d_coords(smiles)
         except Exception as e:
             logger.warning(f"Failed to generate 3D, replace with 2D: {e}")
             coordinates = smiles_to_2d_coords(smiles)
 
-        assert len(mol.GetAtoms()) == len(
-            coordinates
-        ), f"3D coordinates shape is not align with {smiles}"
+        assert len(mol.GetAtoms()) == len(coordinates), f"3D coordinates shape is not align with {smiles}"
         coordinate_list.append(coordinates.astype(np.float32))
     return coordinate_list
 
 
 def smiles_to_coords(smiles, n_conformer=10):
-    """
+    """Converts SMILES strings to 3D coordinates.
+
+    Args:
+        smiles (str): A SMILES string representing the molecule.
+        n_conformer (int): Number of conformers to generate for the molecule.
 
-    Parameters
-    ----------
-    smiles: the smile string
-    n_conformer: conformer num, default (uni-mol) all==11, 10 3d + 1 2d
-
-    Returns
-    -------
-    atoms and coordinates
+    Returns:
+        list[numpy.ndarray]: A list of 3D arrays of coordinates for each conformer of the molecule.
     """
 
     mol = Chem.MolFromSmiles(smiles)
     if len(mol.GetAtoms()) > 400:
         coordinates = [smiles_to_2d_coords(smiles)] * (n_conformer + 1)
         logger.warning("atom num > 400, use 2D coords", smiles)
     else:
@@ -131,80 +108,65 @@
         coordinates.append(smiles_to_2d_coords(smiles).astype(np.float32))
     mol = AllChem.AddHs(mol)
     atoms = [atom.GetSymbol() for atom in mol.GetAtoms()]  # after add H
     return atoms, coordinates
 
 
 def rdkit_2d_features_normalized_generator(mol) -> np.ndarray:
-    """
-    Generates RDKit 2D normalized features for a molecule.
+    """Generates RDKit 2D normalized features for a molecule.
+
+    Args:
+        mol (str or Chem.Mol): A molecule represented as a SMILES string or an RDKit molecule object.
 
-    Parameters
-    ----------
-    mol: A molecule (i.e. either a SMILES string or an RDKit molecule).
-
-    Returns
-    -------
-    An 1D numpy array containing the RDKit 2D normalized features.
+    Returns:
+        numpy.ndarray: An array containing the RDKit 2D normalized features.
     """
     from rdkit import Chem
     from descriptastorus.descriptors import rdNormalizedDescriptors
 
-    smiles = (
-        Chem.MolToSmiles(mol, isomericSmiles=True) if type(mol) != str else mol
-    )
+    smiles = Chem.MolToSmiles(mol, isomericSmiles=True) if type(mol) != str else mol
     generator = rdNormalizedDescriptors.RDKit2DNormalized()
     features = generator.process(smiles)[1:]
     # replace nan values
     features = np.where(np.isnan(features), 0, features)
     return features
 
 
-def morgan_binary_features_generator(
-    mol, radius: int = 2, num_bits: int = 1024
-) -> np.ndarray:
-    """
-    Generates a binary Morgan fingerprint for a molecule.
+def morgan_binary_features_generator(mol, radius: int = 2, num_bits: int = 1024) -> np.ndarray:
+    """Generates a binary Morgan fingerprint for a molecule.
+
+    Args:
+        mol (str or Chem.Mol): A molecule represented as a SMILES string or an RDKit molecule object.
+        radius (int): Radius of the Morgan fingerprint.
+        num_bits (int): Number of bits in the Morgan fingerprint.
 
-    Parameters
-    ----------
-    mol: A molecule (i.e. either a SMILES string or an RDKit molecule).
-    radius: Morgan fingerprint radius.
-    num_bits: Number of bits in Morgan fingerprint.
-
-    Returns
-    -------
-    An 1-D numpy array containing the binary Morgan fingerprint.
+    Returns:
+        numpy.ndarray: An array containing the binary Morgan fingerprint.
     """
     from rdkit import Chem, DataStructs
     from rdkit.Chem import AllChem
 
     mol = Chem.MolFromSmiles(mol) if type(mol) == str else mol
-    features_vec = AllChem.GetMorganFingerprintAsBitVect(
-        mol, radius, nBits=num_bits
-    )
+    features_vec = AllChem.GetMorganFingerprintAsBitVect(mol, radius, nBits=num_bits)
     features = np.zeros((1,))
     DataStructs.ConvertToNumpyArray(features_vec, features)
 
     # replace nan values
     features = np.where(np.isnan(features), 0, features)
     return features
 
 
 def smiles_to_atom_ids(smiles: str) -> list[int]:
-    """
-    Convert smiles strings to a list of atom ids with H included
+    """Converts SMILES strings to a list of atom IDs with hydrogens included.
+
+    Args:
+        smiles (str): A SMILES string representing the molecule.
 
-    Parameters
-    ----------
-    smiles: a smiles string
-
-    Returns
-    -------
-    atom ids
+    Returns:
+        list[int]: A list of atomic numbers corresponding to the atoms in the molecule.
     """
 
     mol = Chem.AddHs(Chem.MolFromSmiles(smiles))
     atom_ids = [atom.GetAtomicNum() for atom in mol.GetAtoms()]
     return atom_ids
 
 
@@ -321,40 +283,34 @@
     "Lv": 116,
     "Ts": 117,
     "Og": 118,
 }
 
 
 def atom_to_atom_ids(atoms: list[str]) -> list[int]:
-    """
-    Convert a list of atoms strings to a list of atom ids
+    """Converts a list of atom symbols to a list of atom IDs.
+
+    Args:
+        atoms (list[str]): A list of atom symbols.
 
-    Parameters
-    ----------
-    atoms: a list of atoms strings
-
-    Returns
-    -------
-    atom ids
+    Returns:
+        list[int]: A list of atomic numbers corresponding to the provided atom symbols.
     """
     atoms_ids = [ATOMIC_NUMBER_MAP[atom] for atom in atoms]
     return atoms_ids
 
 
 def smiles_to_2d_graph(smiles):
-    """
-    Convert smiles to 2d graphs
+    """Converts SMILES strings to 2D graph representations.
+
+    Args:
+        smiles (str): A SMILES string representing the molecule.
 
-    Parameters
-    ----------
-    smiles: smiles strings
-
-    Returns
-    -------
-    atom ids and bonds
+    Returns:
+        tuple[list[int], list[list[int]]]: A tuple containing a list of atom IDs and a list of bonds represented as pairs of atom indices.
     """
     mol = Chem.AddHs(Chem.MolFromSmiles(smiles))
     atoms = smiles_to_atom_ids(smiles)
     bonds = list()
     for bond in mol.GetBonds():
         start, end = bond.GetBeginAtomIdx(), bond.GetEndAtomIdx()
         bonds.append([start, end])
```

### Comparing `muben-0.0.1/muben/utils/io.py` & `muben-0.0.2/muben/utils/io.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 # Author: Yinghao Li
-# Modified: August 26th, 2023
+# Modified: April 17th, 2024
 # ---------------------------------------
 # Description: IO functions
 """
 
-
 import os
 import os.path as op
 import regex
 import pickle
 import json
 import shutil
 import lmdb
 import torch
 import logging
 import numpy as np
 from pathlib import Path
 from typing import Optional
+from rich.logging import RichHandler
 
 logger = logging.getLogger(__name__)
 
 __all__ = [
     "set_log_path",
     "set_logging",
     "logging_args",
@@ -31,135 +31,156 @@
     "load_results",
     "load_lmdb",
     "load_unimol_preprocessed",
 ]
 
 
 def set_log_path(args, time):
-    """
-    Setup log path.
-    Notice that the log path is specified for muben and may not be
-    directly compatible with other projects.
+    """Sets up the log path based on given arguments and time.
+
+    Args:
+        args: Command-line arguments or any object with attributes `dataset_name`, `model_name`, `feature_type`, and `uncertainty_method`.
+        time (str): A string representing the current time or a unique identifier for the log file.
+
+    Returns:
+        str: The constructed log path.
     """
     log_path = op.join(
         "logs",
         args.dataset_name,
-        args.model_name
-        if args.feature_type == "none"
-        else f"{args.model_name}-{args.feature_type}",
+        args.model_name if args.feature_type == "none" else f"{args.model_name}-{args.feature_type}",
         args.uncertainty_method,
         f"{time}.log",
     )
     return log_path
 
 
+# def set_logging(log_path: Optional[str] = None):
+#     """Sets up logging format and file handler.
+
+#     Args:
+#         log_path (Optional[str]): Path where to save the logging file. If None, no log file is saved.
+#     """
+#     stream_handler = logging.StreamHandler()
+#     stream_handler.setLevel(logging.INFO)
+
+#     if log_path and log_path != "disabled":
+#         log_path = op.abspath(log_path)
+#         if not op.isdir(op.split(log_path)[0]):
+#             os.makedirs(op.abspath(op.normpath(op.split(log_path)[0])))
+#         if op.isfile(log_path):
+#             os.remove(log_path)
+
+#         file_handler = logging.FileHandler(filename=log_path)
+#         file_handler.setLevel(logging.DEBUG)
+
+#         logging.basicConfig(
+#             format="%(asctime)s - %(levelname)s - %(name)s -   %(message)s",
+#             datefmt="%m/%d/%Y %H:%M:%S",
+#             level=0,
+#             handlers=[stream_handler, file_handler],
+#         )
+#     else:
+#         logging.basicConfig(
+#             format="%(asctime)s - %(levelname)s - %(name)s -   %(message)s",
+#             datefmt="%m/%d/%Y %H:%M:%S",
+#             level=logging.INFO,
+#             handlers=[stream_handler],
+#         )
+
+#     return None
+
+
 def set_logging(log_path: Optional[str] = None):
-    """
-    setup logging format
+    """Sets up logging format and file handler.
 
-    Parameters
-    ----------
-    log_path: where to save logging file. Leave None to save no log files
-
-    Returns
-    -------
-    None
+    Args:
+        log_path (Optional[str]): Path where to save the logging file. If None, no log file is saved.
     """
-    stream_handler = logging.StreamHandler()
-    stream_handler.setLevel(logging.INFO)
+    rh = RichHandler()
+    rh.setFormatter(logging.Formatter("%(message)s", datefmt="[%m/%d %X]"))
 
     if log_path and log_path != "disabled":
         log_path = op.abspath(log_path)
         if not op.isdir(op.split(log_path)[0]):
             os.makedirs(op.abspath(op.normpath(op.split(log_path)[0])))
         if op.isfile(log_path):
             os.remove(log_path)
 
         file_handler = logging.FileHandler(filename=log_path)
         file_handler.setLevel(logging.DEBUG)
 
         logging.basicConfig(
-            format="%(asctime)s - %(levelname)s - %(name)s -   %(message)s",
-            datefmt="%m/%d/%Y %H:%M:%S",
-            level=0,
-            handlers=[stream_handler, file_handler],
+            level="NOTSET",
+            format="%(asctime)s %(levelname)-8s %(message)-80s     @ %(pathname)-s:%(lineno)d",
+            datefmt="[%m/%d %X]",
+            handlers=[file_handler, rh],
         )
+
     else:
         logging.basicConfig(
-            format="%(asctime)s - %(levelname)s - %(name)s -   %(message)s",
-            datefmt="%m/%d/%Y %H:%M:%S",
-            level=logging.INFO,
-            handlers=[stream_handler],
+            datefmt="[%m/%d %X]",
+            level="NOTSET",
+            handlers=[rh],
         )
 
     return None
 
 
 def logging_args(args):
-    """
-    Logging model arguments into logs
-    Last modified: 08/19/21
+    """Logs model arguments.
 
-    Parameters
-    ----------
-    args: arguments
-
-    Returns
-    -------
-    None
+    Args:
+        args: The arguments to be logged. Can be an argparse Namespace or similar object.
     """
     arg_elements = {
         attr: getattr(args, attr)
         for attr in dir(args)
-        if not callable(getattr(args, attr))
-        and not attr.startswith("__")
-        and not attr.startswith("_")
+        if not callable(getattr(args, attr)) and not attr.startswith("__") and not attr.startswith("_")
     }
     logger.info(f"Configurations: ({type(args)})")
     for arg_element, value in arg_elements.items():
         logger.info(f"  {arg_element}: {value}")
 
     return None
 
 
 def remove_dir(directory: str):
-    """
-    Remove a directory and its subtree folders/files
+    """Removes a directory and its subtree.
+
+    Args:
+        directory (str): The directory to remove.
     """
     dirpath = Path(directory)
     if dirpath.exists() and dirpath.is_dir():
         shutil.rmtree(dirpath)
     return None
 
 
 def init_dir(directory: str, clear_original_content: Optional[bool] = True):
-    """
-    Create the target directory. If the directory exists, remove all subtree folders/files in it.
+    """Initializes a directory. Clears content if specified and directory exists.
+
+    Args:
+        directory (str): The directory to initialize.
+        clear_original_content (Optional[bool]): Whether to clear the original content of the directory if it exists.
     """
 
     if clear_original_content:
         remove_dir(directory)
     os.makedirs(op.normpath(directory), exist_ok=True)
     return None
 
 
 def save_json(obj, path: str, collapse_level: Optional[int] = None):
-    """
-    Save objective to a json file.
-    Create this function so that we don't need to worry about creating parent folders every time
+    """Saves an object to a JSON file.
 
-    Parameters
-    ----------
-    obj: the objective to save
-    path: the path to save
-    collapse_level: set to any collapse value to prettify output json accordingly
-
-    Returns
-    -------
-    None
+    Args:
+        obj: The object to save.
+        path (str): The path to the file where the object will be saved.
+        collapse_level (Optional[int]): Specifies how to prettify the JSON output. If set, collapses levels greater than this.
     """
     file_dir = op.dirname(op.normpath(path))
     if file_dir:
         os.makedirs(file_dir, exist_ok=True)
 
     json_obj = json.dumps(obj, indent=2, ensure_ascii=False)
     if collapse_level:
@@ -168,83 +189,64 @@
     with open(path, "w", encoding="utf-8") as f:
         f.write(json_obj)
 
     return None
 
 
 def prettify_json(text, indent=2, collapse_level=4):
-    """
-    Make json file more readable by collapsing indent levels higher than `collapse_level`.
+    """Prettifies JSON text by collapsing indent levels higher than `collapse_level`.
+
+    Args:
+        text (str): Input JSON text.
+        indent (int): The indentation value of the JSON text.
+        collapse_level (int): The level from which to stop adding new lines.
 
-    Parameters
-    ----------
-    text: input json text obj
-    indent: the indent value of your json text. Notice that this value needs to be larger than 0
-    collapse_level: the level from which the program stops adding new lines
-
-    Usage
-    -----
-    ```
-    my_instance = list()  # user-defined serializable data structure
-    json_obj = json.dumps(my_instance, indent=2, ensure_ascii=False)
-    json_obj = prettify_json(json_text, indent=2, collapse_level=4)
-    with open(path_to_file, 'w', encoding='utf=8') as f:
-        f.write(json_text)
-    ```
+    Returns:
+        str: The prettified JSON text.
     """
     pattern = r"[\r\n]+ {%d,}" % (indent * collapse_level)
     text = regex.sub(pattern, " ", text)
     text = regex.sub(r"([\[({])+ +", r"\g<1>", text)
     text = regex.sub(
         r"[\r\n]+ {%d}([])}])" % (indent * (collapse_level - 1)),
         r"\g<1>",
         text,
     )
     text = regex.sub(r"(\S) +([])}])", r"\g<1>\g<2>", text)
     return text
 
 
 def convert_arguments_from_argparse(args):
-    """
-    Convert argparse Namespace to transformers style arguments parser strings.
-    Used to transfer code style.
+    """Converts argparse Namespace to transformers-style arguments.
+
+    Args:
+        args: argparse Namespace object.
 
-    Parameters
-    ----------
-    args: Namespace
-
-    Returns
-    -------
-    str
+    Returns:
+        str: Transformers style arguments string.
     """
     args_string = ""
     for k, v in args.__dict__.items():
         default_value = f"'{v}'" if isinstance(v, str) else v
         arg_str = f"{k}: Optional[{type(v).__name__}] = field(\n"
         arg_str += f"    default={default_value}, metadata={{'help': ''}}\n"
         arg_str += f")\n\n"
         args_string += arg_str
     return args_string
 
 
 def save_results(path, preds, variances, lbs, masks):
-    """
-    Save muben prediction results.
+    """Saves prediction results to a file.
 
-    Parameters
-    ----------
-    path: path to save
-    preds: model predictions
-    variances: variances for regression tasks
-    lbs: ground truth labels
-    masks: label masks
-
-    Returns
-    -------
-    None
+    Args:
+        path (str): Path where to save the results.
+        preds: Predictions to save.
+        variances: Variances associated with predictions.
+        lbs: Ground truth labels.
+        masks: Masks indicating valid entries.
     """
     if not path.endswith(".pt"):
         path = f"{path}.pt"
 
     data_dict = {
         "version": 2,
         "preds": preds,
@@ -255,21 +257,21 @@
 
     os.makedirs(op.dirname(op.normpath(path)), exist_ok=True)
     torch.save(data_dict, path)
     return None
 
 
 def load_results(result_paths: list[str]):
-    """
-    Load muben prediction results.
+    """Loads prediction results from files.
+
+    Args:
+        result_paths (list[str]): Paths to the result files.
 
-    Parameters
-    ----------
-    result_paths : list[str]
-        paths to the result files
+    Returns:
+        tuple: Predictions, variances, labels, and masks loaded from the files.
     """
     lbs = masks = np.nan
     preds_list = list()
     variances_list = list()
 
     for test_result_path in result_paths:
         results = torch.load(test_result_path)
@@ -293,46 +295,37 @@
         elif results.get("version", 1) == 2:
             preds_list.append(results["preds"])
             try:
                 variances_list.append(results["vars"])
             except KeyError:
                 pass
         else:
-            raise ValueError(
-                f"Undefined result version: {results.get('version', 1)}"
-            )
+            raise ValueError(f"Undefined result version: {results.get('version', 1)}")
 
     # aggregate mean and variance
     preds = np.stack(preds_list).mean(axis=0)
-    if (
-        variances_list and not (np.asarray(variances_list) == None).any()
-    ):  # regression
+    if variances_list and not (np.asarray(variances_list) == None).any():  # regression
         # variances = np.mean(np.stack(preds_list) ** 2 + np.stack(variances_list), axis=0) - preds ** 2
         variances = np.stack(variances_list).mean(axis=0)
     else:
         variances = None
 
     return preds, variances, lbs, masks
 
 
-def load_lmdb(
-    data_path, keys_to_load: list[str] = None, return_dict: bool = False
-):
-    """
-    Load the lmdb-formatted dataset splits used in Uni-Mol
-
-    Parameters
-    ----------
-    data_path: path to data split (*.lmdb)
-    keys_to_load: dict keys to load. The argument `return_dict` is forced to be True if `keys_to_load` is left None
-    return_dict: whether to return a dictionary, will be forced to be True if `keys_to_load` is left None
-
-    Returns
-    -------
-    tuple if return_dict is False else dict of loaded values corresponding to specified keys
+def load_lmdb(data_path, keys_to_load: list[str] = None, return_dict: bool = False):
+    """Loads data from an LMDB file.
+
+    Args:
+        data_path (str): Path to the LMDB file.
+        keys_to_load (list[str], optional): Specific keys to load from the LMDB file. Loads all keys if None.
+        return_dict (bool): Whether to return a dictionary of loaded values.
+
+    Returns:
+        dict or tuple: Loaded values from the LMDB file. The format depends on `return_dict`.
     """
 
     if keys_to_load is None:
         result_dict = None
         return_dict = True
     elif isinstance(keys_to_load, str):
         result_dict = {keys_to_load: list()}
@@ -366,24 +359,21 @@
     if return_dict:
         return result_dict
     else:
         return (v for v in result_dict.values())
 
 
 def load_unimol_preprocessed(data_dir: str):
-    """
-    Load all lmdb-formatted dataset training & valid& test splits used in Uni-Mol
+    """Loads preprocessed UniMol dataset splits from an LMDB file.
+
+    Args:
+        data_dir (str): Directory containing the LMDB dataset splits.
 
-    Parameters
-    ----------
-    data_dir: dir to data splits
-
-    Returns
-    -------
-    tuple if return_dict is False else dict of loaded values corresponding to specified keys
+    Returns:
+        dict: Loaded dataset splits (train, valid, test).
     """
 
     result_dict = None
     for partition in ("train", "valid", "test"):
         # read data points
         lmdb_path = os.path.join(data_dir, f"{partition}.lmdb")
         results = load_lmdb(lmdb_path)
```

### Comparing `muben-0.0.1/muben/utils/macro.py` & `muben-0.0.2/muben/utils/macro.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 """
 # Author: Yinghao Li
-# Modified: December 1st, 2023
+# Modified: April 11th, 2024
 # ---------------------------------------
 # Description: Constants
 """
 
-
 import logging
 from enum import Enum
 
 logger = logging.getLogger(__name__)
 
 __all__ = [
     "DATASET_NAMES",
     "CLASSIFICATION_DATASET",
     "REGRESSION_DATASET",
     "dataset_mapping",
     "EVAL_METRICS",
     "CLASSIFICATION_METRICS",
     "REGRESSION_METRICS",
-    "metrics_mapping",
+    "METRICS_MAPPING",
     "MODEL_NAMES",
     "UncertaintyMethods",
     "DatasetNames",
     "ModelNames",
     "FINGERPRINT_FEATURE_TYPES",
     "StrEnum",
     "QM_DATASET",
@@ -132,15 +131,15 @@
     "qm9": "mae",
 }
 
 MODEL_NAMES = ["DNN", "ChemBERTa", "GROVER", "Uni-Mol", "TorchMD-NET", "GIN"]
 
 CLASSIFICATION_METRICS = ["roc-auc", "ece", "nll", "brier"]
 REGRESSION_METRICS = ["rmse", "mae", "nll", "ce"]
-metrics_mapping = {
+METRICS_MAPPING = {
     "roc-auc": "ROC-AUC",
     "ece": "ECE",
     "nll": "NLL",
     "brier": "BS",
     "rmse": "RMSE",
     "mae": "MAE",
     "ce": "CE",
```

### Comparing `muben-0.0.1/muben/utils/metrics.py` & `muben-0.0.2/muben/utils/metrics.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 # Author: Yinghao Li
-# Modified: December 1st, 2023
+# Modified: February 29th, 2024
 # ---------------------------------------
-# Description: Calculate the metrics for the uncertainty quantification
-"""
+# Description:
 
+These Python functions are designed to calculate various metrics for classification and regression tasks,
+particularly focusing on evaluating the performance of models on tasks involving predictions with associated uncertainties.
+"""
 
 import torch
 import torch.nn.functional as F
 import numpy as np
 
 from torchmetrics.functional.classification import binary_calibration_error
 from sklearn.metrics import (
@@ -19,30 +21,26 @@
     auc,
     brier_score_loss,
 )
 from scipy.stats import norm as gaussian
 
 
 def classification_metrics(preds, lbs, masks, exclude: list = None):
-    """
-    Calculate the metrics for classification tasks
+    """Calculates various metrics for classification tasks.
 
-    Parameters
-    ----------
-    preds : numpy array
-        The predicted values
-    lbs : numpy array
-        The ground truth values
-    masks : numpy array
-        The mask for the ground truth values
-
-    Returns
-    -------
-    result_metrics_dict : dict
-        The dictionary of the metrics
+    This function computes ROC-AUC, PRC-AUC, ECE, MCE, NLL, and Brier score for classification predictions.
+
+    Args:
+        preds (numpy.ndarray): Predicted probabilities for each class.
+        lbs (numpy.ndarray): Ground truth labels.
+        masks (numpy.ndarray): Masks indicating valid data points for evaluation.
+        exclude (list, optional): List of metrics to exclude from the calculation.
+
+    Returns:
+        dict: A dictionary containing calculated metrics.
     """
     if not exclude:
         exclude = list()
 
     result_metrics_dict = dict()
 
     roc_auc_list = list()
@@ -156,32 +154,27 @@
             "macro-avg": brier_avg,
         }
 
     return result_metrics_dict
 
 
 def regression_metrics(preds, variances, lbs, masks, exclude: list = None):
-    """
-    Calculate the metrics for regression tasks
+    """Calculates various metrics for regression tasks.
 
-    Parameters
-    ----------
-    preds : numpy array
-        The predicted values (means)
-    variances : numpy array
-        The predicted variances
-    lbs : numpy array
-        The ground truth values
-    masks : numpy array
-        The mask for the ground truth values
-
-    Returns
-    -------
-    result_metrics_dict : dict
-        The dictionary of the metrics
+    Computes RMSE, MAE, NLL, and calibration error for regression predictions and their associated uncertainties.
+
+    Args:
+        preds (numpy.ndarray): Predicted values (means).
+        variances (numpy.ndarray): Predicted variances.
+        lbs (numpy.ndarray): Ground truth values.
+        masks (numpy.ndarray): Masks indicating valid data points for evaluation.
+        exclude (list, optional): List of metrics to exclude from the calculation.
+
+    Returns:
+        dict: A dictionary containing calculated metrics.
     """
     if not exclude:
         exclude = list()
 
     if len(preds.shape) == 1:
         preds = preds[:, np.newaxis]
 
@@ -241,32 +234,26 @@
         ce_avg = np.mean(ce_list)
         result_metrics_dict["ce"] = {"all": ce_list, "macro-avg": ce_avg}
 
     return result_metrics_dict
 
 
 def regression_calibration_error(lbs, preds, variances, n_bins=20):
-    """
-    Calculate the calibration error for regression tasks
+    """Calculates the calibration error for regression tasks.
+
+    Uses the predicted means and variances to estimate the calibration error across a specified number of bins.
+
+    Args:
+        lbs (numpy.ndarray): Ground truth values.
+        preds (numpy.ndarray): Predicted values (means).
+        variances (numpy.ndarray): Predicted variances.
+        n_bins (int, optional): Number of bins to use for calculating calibration error. Defaults to 20.
 
-    Parameters
-    ----------
-    lbs : numpy array
-        The ground truth values
-    preds : numpy array
-        The predicted values (means)
-    variances : numpy array
-        The predicted variances
-    n_bins : int
-        The number of bins to use
-
-    Returns
-    -------
-    calibration_error : float
-        The calibration error
+    Returns:
+        float: The calculated calibration error.
     """
     sigma = np.sqrt(variances)
     phi_lbs = gaussian.cdf(lbs, loc=preds.reshape(-1, 1), scale=sigma.reshape(-1, 1))
 
     expected_confidence = np.linspace(0, 1, n_bins + 1)[1:-1]
     observed_confidence = np.zeros_like(expected_confidence)
```

### Comparing `muben-0.0.1/muben.egg-info/PKG-INFO` & `muben-0.0.2/muben.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muben
-Version: 0.0.1
+Version: 0.0.2
 Summary: Benchmark for molecular uncertainty estimation.
 Home-page: https://github.com/Yinghao-Li/MUBen
 Author: Yinghao Li
 Author-email: yinghaoli@gatech.edu
 License: MIT
 Keywords: machine-learning uncertainty-estimation materials-science materials-property-prediction
 Classifier: Intended Audience :: Developers
@@ -15,233 +15,222 @@
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MUBen: **M**olecular **U**ncertainty **Ben**mark
-Code associated with paper *MUBen: Benchmarking the Uncertainty of Pre-Trained Models for Molecular Property Prediction*.
+Code associated with paper *MUBen: **Ben**chmarking the **U**ncertainty of **M**olecular Representation Models*.
 
-The code is built to expose implementation details as much as possible and be easily extendable.
-Questions and suggestions are welcome if you find any issues while using our code.
+[![Documentation](https://img.shields.io/badge/%F0%9F%93%96%20Documentation-Link-blue)](https://yinghao-li.github.io/MUBen/)
+[![OpenReview](https://img.shields.io/badge/%F0%9F%94%97%20OpenReview-TMLR-darkred)](https://openreview.net/forum?id=qYceFeHgm4)
+[![arXiv](https://img.shields.io/badge/arXiv-2306.10060-b31b1b.svg)](https://arxiv.org/abs/2306.10060)
+[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/Yinghao-Li/MUBen/)
+[![PyPI version](https://badge.fury.io/py/muben.svg)](https://badge.fury.io/py/muben)
+
+Please visit [📕 Documentation](https://yinghao-li.github.io/MUBen/) for the full documentation of this project, which contains more comprehensive API introductions and examples.
+
+![](./figures/f1.summarization.png)
 
-## 0. ABOUT
 
 MUBen is a benchmark that aims to investigate the performance of uncertainty quantification (UQ) methods built upon backbone molecular representation models.
 It implements 6 backbone models (4 pre-trained and 2 non-pre-trained), 8 UQ methods (8 compatible for classification and 6 for regression), and 14 datasets from [MoleculeNet](https://moleculenet.org/) (8 for classification and 6 for regression).
-We are actively expanding the benchmark to include more backbones, UQ methods and datasets.
+We are actively expanding the benchmark to include more backbones, UQ methods, and datasets.
 This is an arduous task, and we welcome contribution or collaboration in any form.
 
-### Backbones
-| Backbone Models      | Paper | Official Repo | Our Implementation|
-| ----------- | ----------- | ----------- | ----------- |
-|*Pre-Trained Backbones* |||
-| ChemBERTa |[link](https://arxiv.org/abs/2209.01712) | [link](https://github.com/seyonechithrananda/bert-loves-chemistry) | [link](https://github.com/Yinghao-Li/UncertaintyBenchmark/tree/main/muben/chemberta) | 
-| GROVER   | [link](https://arxiv.org/abs/2007.02835) | [link](https://github.com/tencent-ailab/grover)| [link](https://github.com/Yinghao-Li/UncertaintyBenchmark/tree/main/muben/grover)|
-|Uni-Mol| [link](https://openreview.net/forum?id=6K2RM6wVqKu) | [link](https://github.com/dptech-corp/Uni-Mol/tree/main/unimol) | [link](https://github.com/Yinghao-Li/UncertaintyBenchmark/tree/main/muben/unimol)|
-|TorchMD-NET | [Architecture](https://arxiv.org/abs/2202.02541); [Pre-training](https://arxiv.org/abs/2206.00133) | [link](https://github.com/shehzaidi/pre-training-via-denoising) | [link](https://github.com/Yinghao-Li/UncertaintyBenchmark/tree/main/muben/torchmdnet)|
-| *Non-Pre-Trained Backbones* |||
-|DNN|-|-|[link](https://github.com/Yinghao-Li/UncertaintyBenchmark/tree/main/muben/dnn)|
-|GIN| [link](https://arxiv.org/pdf/1810.00826.pdf) | [pyg](https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.nn.models.GIN.html) | [link](https://github.com/Yinghao-Li/UncertaintyBenchmark/tree/main/muben/gin)|
+## Backbones
+
+| Backbone Models      | Paper | Official Repo |
+| ----------- | ----------- | ----------- |
+|***Pre-Trained*** |||
+| ChemBERTa |[link](https://arxiv.org/abs/2209.01712) | [link](https://github.com/seyonechithrananda/bert-loves-chemistry) | 
+| GROVER   | [link](https://arxiv.org/abs/2007.02835) | [link](https://github.com/tencent-ailab/grover)|
+|Uni-Mol| [link](https://openreview.net/forum?id=6K2RM6wVqKu) | [link](https://github.com/dptech-corp/Uni-Mol/tree/main/unimol) |
+|TorchMD-NET | [Architecture](https://arxiv.org/abs/2202.02541); [Pre-training](https://arxiv.org/abs/2206.00133) | [link](https://github.com/shehzaidi/pre-training-via-denoising) |
+| ***Trained from Scratch*** |||
+|DNN|-|-|
+|GIN| [link](https://arxiv.org/pdf/1810.00826.pdf) | [pyg](https://pytorch-geometric.readthedocs.io/en/latest/generated/torch_geometric.nn.models.GIN.html) |
 
-### Uncertainty Quantification Methods
+
+## Uncertainty Quantification Methods
 | UQ Method | Classification | Regression | Paper |
 | ----------- | ----------- | ----------- | ----------- |
-| *Included* |||
+| ***Included in Paper*** |||
 | Deterministic | ✅︎ | ✅︎ | - |
 | Temperature Scaling | ✅︎ | - | [link](https://arxiv.org/abs/1706.04599) |
 | Focal Loss | ✅︎ | - | [link](https://arxiv.org/abs/1708.02002) |
 | Deep Ensembles | ✅︎ | ✅︎ | [link](https://arxiv.org/abs/1612.01474) |
 | SWAG | ✅︎ | ✅︎ | [link](https://arxiv.org/abs/1808.05326) |
 | Bayes by Backprop | ✅︎ | ✅︎ | [link](https://arxiv.org/abs/1505.05424) |
 | SGLD | ✅︎ | ✅︎ | [link](https://www.stats.ox.ac.uk/~teh/research/compstats/WelTeh2011a.pdf) |
 | MC Dropout | ✅︎ | ✅︎ | [link](https://arxiv.org/abs/1506.02142) |
+| ***Additional in Repo*** |||
+| Evidential Networks |✅︎|✅︎|[link](https://openreview.net/forum?id=xqS8k9E75c)|
+| Conformal Prediction |-|✅︎| [link](https://arxiv.org/abs/2107.07511) |
+| Isotonic Calibration| - | ✅︎ | [link](https://arxiv.org/abs/1905.06023)|
 
-### Data
-
-Please check [MoleculeNet](https://moleculenet.org/datasets-1) for a detailed description.
-We use a subset of the MoleculeNet benckmark, including BBBP, Tox21, ToxCast, SIDER, ClinTox, BACE, MUV, HIV, ESOL, FreeSolv, Lipophilicity, QM7, QM8, QM9.
+## Data
 
-## 1. DATA
+> The prepared scaffold-split data is available in the [./data/files/](https://github.com/Yinghao-Li/UncertaintyBenchmark/tree/main/data/files) directory.
 
-> A set of partitioned datasets are already included in this repo. You can find them under the `./data/` folder: [[scaffold split](https://github.com/Yinghao-Li/UncertaintyBenchmark/tree/main/data/files)]; [[random split](https://github.com/Yinghao-Li/UncertaintyBenchmark/tree/main/data/files-random)].
+This documentation utilizes a selection from the MoleculeNet benchmark, which includes datasets such as BBBP, Tox21, ToxCast, SIDER, ClinTox, BACE, MUV, HIV, ESOL, FreeSolv, Lipophilicity, QM7, QM8, and QM9.
+For detailed descriptions of these datasets, please refer to the [MoleculeNet website](https://moleculenet.org/datasets-1).
 
-We utilize the datasets prepared by [Uni-Mol](https://github.com/dptech-corp/Uni-Mol/tree/main/unimol).
-You find the data [here](https://github.com/dptech-corp/Uni-Mol/tree/main/unimol#:~:text=pockets.tar.gz-,molecular%20property,-3.506GB) or directly download it through [this link](https://bioos-hermite-beijing.tos-cn-beijing.volces.com/unimol_data/finetune/molecular_property_prediction.tar.gz).
-We place the unzipped files into `./data/UniMol` by default.
-For convenience, you are suggested to rename the `qm7dft`, `qm8dft`, and `qm9dft` folders to `qm7`, `qm8`, and `qm9`.
+We employ the "molecular property" datasets curated by [Uni-Mol](https://github.com/dptech-corp/Uni-Mol/tree/main/unimol), which are accessible for download [here](https://bioos-hermite-beijing.tos-cn-beijing.volces.com/unimol_data/finetune/molecular_property_prediction.tar.gz).
+While the original Uni-Mol dataset is generally not necessary, it is used to provide pre-defined molecule conformations for running the Uni-Mol model.
+To use the Uni-Mol data, download and unzip the files into the `./data/UniMol/` directory.
+For ease of reference, you are suggested to rename the `qm7dft`, `qm8dft`, and `qm9dft` directories to `qm7`, `qm8`, and `qm9`, respectively.
+The conversion of the dataset format from Uni-Mol to our specifications can be viewed in the script [dataset_build_from_unimol.py](https://github.com/Yinghao-Li/MUBen/blob/main/assist/dataset_build_from_unimol.py).
 
-Afterwards, you can transfer the dataset format into ours by running
-```bash
-PYTHONPATH="." python ./assist/dataset_build_from_unimol.py
-``` 
-suppose you are in the project root directory.
-You can specify the input (Uni-Mol) and output data directories with `--unimol_data_dir` and `--output_dir` arguments.
-The script will convert *all* datasets by default (excluding PCBA).
-If you want to specify a subset of datasets, you can specify the argument `--dataset_names` with the target dataset names with lowercase letters.
+Typically, each dataset comprises 4 files: `train.csv`, `valid.csv`, `test.csv`, and `meta.json`.
+The `.csv` files partition the data into training, validation, and testing sets, while `meta.json` contains metadata such as task type (classification or regression), number of tasks, and number of classes (for classification tasks).
+Each `.csv` file contains three columns:
+- `smiles`: A string representing the SMILES notation of a molecule.
+- `labels`: A list of integers or floats representing the property values to be predicted for each molecule. The length of the list corresponds to the number of tasks.
+- `masks`: A binary list (containing 0s and 1s) where 1 indicates a valid property value and 0 indicates an invalid value to be ignored during training and testing.
 
-**Notice**: If you would like to run the Uni-Mol model, you are suggested to keep the original `UniMol` data as we will use the pre-defined molecule conformations.
-Otherwise, it is safe to remove the original data.
+The dataset is automatically loaded during training through the method `muben.dataset.Dataset.prepare()`.
+For a practical example, visit the [example](./train.python.md) page.
 
-### Other Options
+## Environment Setup
 
-If you do not want to use Uni-Mol data, you can try the scripts within the `legacy` folder, including `build_dgllife_datasets.py`, and `build_qm[7,8,9]_dataset.py`.
-Notice that this may result in training/validation/test partitions different from what is being used in our experiments.
+Our code is developed with `Python 3.10`, and does **not** work with `Python < 3.9`.
 
-### Using Customized Datasets
+### Installation
 
-If you want to test the UQ methods on your own dataset, you can use `pandas.DataFrame` structure with the following keys:
-```
-{
-  "smiles": list of `str`,
-  "labels": list of list of int/float,
-  "masks": list of list of int/float (with values within {0,1})
-}
+MUBen is available as a Python package on [PyPI](https://pypi.org/project/muben/) and can be installed using pip.
+If you prefer to use MUBen as a standalone package and do not need to modify the source code, you can simply run:
+```bash
+pip install muben
 ```
-and store them as `train.csv`, `valid.csv`, and `test.csv` files.
-`mask=1` indicates the existence informative label at the position and `mask=0` indicates missing label.
-You can check the prepared datasets included in our program for reference.
-You are recommended to put the dataset files in the `./data/file/<dataset name>` directory, but you can of course choose your favorite location and specify the `--data_folder` argument.
-
-The `.csv` files should be accompanied by a `meta.json` file within the same directory.
-It stores some constant dataset properties, *e.g.*, `task_type` (classification or regression), `n_tasks`, or `classes` (`[0,1]` for all our classification datasets).
-For the customized dataset, one **required** property is the `eval_metric` for validation and test (*e.g.*, roc-auc, rmse, *etc.*) since it is not specified in the macro file.
-Please refer to `./assist/dataset_build_roe.py` for an example (unfortunately, we are not allowed to release the dataset).
 
-## 2. REQUIREMENTS
-
-Please find the required packages in `requirements.txt`.
-Our code is developed with `Python 3.10` and does not work with Python versions earlier than `3.9`.
-It is recommended to create a new `conda` environment with
+To download the source code and datasets, you can fork the project on GitHub and clone your fork, or directly clone the original repository:
 
 ```bash
-conda create --name <env_name> --file requirements.txt
+# Clone your fork of the repository
+git clone https://github.com/<your GitHub username>/MUBen.git
+
+# Or clone the original repository with git
+git clone https://github.com/Yinghao-Li/MUBen.git --single-branch --branch main
 ```
 
-### Docker
-Alternatively, you can run this project in a docker container.
-You can build your image through
+
+### Anaconda
+
+Suppose you have anaconda or miniconda installed in your local machine, you can create a new `conda` environment for this project using `conda create`.
 ```bash
-docker build -t muben ./docker
+conda create -n muben python=3.10
 ```
-and run your container in an interactive shell with
+
+The required packages are listed in `requirements.txt`.
+It is recommended to install these dependencies with `pip install` as `conda install` may sometimes encounter dependency resolution issue.
 ```bash
-docker run --gpus all -it --rm  muben
+conda activate muben
+pip install -r requirements.txt
 ```
 
-### External Dependencies
+### Backbone Checkpoints
 
-The backbone models `GROVER` and `Uni-Mol` require loading pre-trained model checkpoints.
+Some backbone models require loading pre-trained model checkpoints.
 
+- For ChemBERTa, we use the `DeepChem/ChemBERTa-77M-MLM` checkpoint hosted on Hugging Face's [Model Hub](https://huggingface.co/models). You can specify the model name to the argument `--pretrained_model_name_or_path` (which is set to default), or you can download the model and pass the path to the model to the argument.
 - The `GROVER-base` checkpoint is available at GROVER's [project repo](https://github.com/tencent-ailab/grover) or can be directly downloaded through [this link](https://ai.tencent.com/ailab/ml/ml-data/grover-models/pretrain/grover_base.tar.gz).
 Unzip the downloaded `.tar.gz` file to get the `.pt` checkpoint.
 - The `Uni-Mol` checkpoint is available at Uni-Mol's [project repo](https://github.com/dptech-corp/Uni-Mol/tree/main/unimol) or can be directly downloaded through [this link](https://github.com/dptech-corp/Uni-Mol/releases/download/v0.1/mol_pre_no_h_220816.pt).
+- The `TorchMD-NET` checkpoint is available at this [project repo](https://github.com/shehzaidi/pre-training-via-denoising) or can be directly downloaded through [this link](https://github.com/shehzaidi/pre-training-via-denoising/raw/main/checkpoints/denoised-pcqm4mv2.ckpt).
 
-By default, the code will look for the models at locations `./models/grover_base.pt` and `./models/unimol_base.pt`, respectively.
-You need to specify the `--checkpoint_path` argument if you prefer other locations and checkpoint names.
 
-## 3. RUN
+## Fine-Tuning the Models
 
-> A simple demo of running our project can be found at `./demo/demo.ipynb`.
+> Please visit [this Documentation page](https://yinghao-li.github.io/MUBen/train.python/) for a guideline of using the `muben` package, or [this Documentation page](https://yinghao-li.github.io/MUBen/customize/) for an instruction about incorporating customized datasets or backbone models.
 
-To run each of the four backbone models with uncertainty estimation methods, you can check the `run_*.py` files in the root directory.
-Example shell scripts are provided in the `./scripts` folder as `.sh` files.
-You can use them through
-```bash
-./scripts/run_dnn_rdkit.sh <CUDA_VISIBLE_DEVICES>
-```
-as an example.
-Notice that we need to comment out the variables `train_on_<dataset name>` in the `.sh` files to skip training on the corresponding datasets.
-Setting their value to `false` **does not work**.
+The [./run/](https://github.com/Yinghao-Li/MUBen/tree/main/run) directory contains the entry scripts to fine-tuning each of the backbone-UQ combinations.
+Currently, the script [./run/run.py](https://github.com/Yinghao-Li/MUBen/blob/main/run/run.py) is adopted to run all backbone models except for GROVER and Uni-Mol, whose entry scripts are [./run/grover.py](https://github.com/Yinghao-Li/MUBen/blob/main/run/grover.py) and [./run/unimol.py](https://github.com/Yinghao-Li/MUBen/blob/main/run/unimol.py), respectively.
 
-Another way of specifying arguments is through the `.json` scripts, for example:
-```bash
-PYTHONPATH="." CUDA_VISIBLE_DEVICES=0 python ./run/dnn.py ./scripts/config_dnn.json
-```
-This approach could be helpful for debugging the code through vscode.
+### Specify Arguments Using Command Lines
 
-To get a detailed description of each argument, you can use `--help`:
+An example of running the **DNN** model with **RDKit** features with the **MC Dropout** UQ method on the **BBBP** dataset is
 ```bash
-PYTHONPATH="." python ./run/dnn.py --help
+CUDA_VISIBLE_DEVICES=0 \
+PYTHONPATH="." \
+python ./run/run.py \
+    --descriptor_type "RDKit" \
+    --data_folder "./data/files" \
+    --dataset_name "bbbp" \
+    --uncertainty_method "MCDropout" \
+    --lr 0.0001 \
+    --n_epochs 200 \
+    --batch_size 256 \
+    --seed 0
 ```
+In the example, the `--descriptor_type` argument is used to select the backbone models used in our experiments.
+It has 4 options: {"RDKit", "Linear", "2D", "3D"}, which corresponds to the DNN, ChemBERTa, GIN and TorchMD-NET backbone models in the CLI, respectively.
+In the future versions, we may consider including multiple backbone models that correspond to one descriptor, which requires us to specify the `--model_name` argument to separate the backbones.
+But currently, we do not need to worry about that and can leave `--model_name` as default.
 
-### Logging and WandB
-
-By default, this project uses local logging files (`*.log`) and [WandB](https://wandb.ai/site) to track training status.
+> For the interpretation of each argument, please check the [`muben.args` API](./muben.args.md) or directly refer to the [code implementation](https://github.com/Yinghao-Li/MUBen/tree/main/muben/args).
+> Notice that the API documentation may not be entirely comprehensive.
 
-The log files are stored as `./logs/<dataset>/<model>/<uncertainty>/<running_time>.log`.
-You can change the file path by specifying the `--log_path` argument, or disable log saving by setting `--log_path="disabled"`.
-
-To use WandB, you first need to register an account and sign in on your machine with `wandb login`.
-If you are running your code on a public device, you can instead use program-wise signing in by specifying the `--wandb_api_key` argument while running our code.
-You can find your API key in your browser here: https://wandb.ai/authorize.
-To disable WandB, use `--disable_wandb [true]`.
-By default, we use `MUBen-<dataset>` as WandB project name and `<model>-<uncertainty>` as the model name.
-You can change this behavior by specifying the `--wandb_project` and `--wandb_name` arguments.
-
-### Data Loading
+To run GROVER or Uni-Mol, we just need to replace `run.py` by the corresponding script, and slightly modify the arguments:
+```bash
+CUDA_VISIBLE_DEVICES=0 \
+PYTHONPATH="." \
+python ./run/unimol.py \
+    --data_folder "./data/files" \
+    --unimol_feature_folder "./data/UniMol/" \
+    --dataset_name "esol" \
+    --checkpoint_path "./models/unimol_base.pt" \
+    --uncertainty_method "MCDropout" \
+    --regression_with_variance \
+    ...
+```
+> For regression tasks, the argument `--regression_with_variance` is vital to guarantee a valid result with predicted variance.
 
-The progress will automatically create the necessary features (molecular descriptors) required by backbone models from the SMILES strings if they are loaded properly.
-The processed features are stored in the `<bottom-level data folder>/processed/` directory as `<train/valid/test>.pt` files by default, and will be automatically loaded the next time you apply the same backbone model on the same dataset.
-You can change this behavior with `--disable_dataset_saving` for disabling dataset saving or `--ignore_preprocessed_dataset` for not loading from the saved (processed) dataset.
+### Specify Arguments using `.yaml` Files
 
-Constructing Morgan fingerprint, RDKit features or 3D conformations for Uni-Mol may take a while.
-You can accelerate this process by utilizing multiple threads `--num_preprocess_workers=n>1` (default is 8).
-For 3D conformations, we directly take advantage of the results from Uni-Mol but still keep the choice of generating them by ourselves if the Uni-Mol data files are not found.
+Another way of specifying arguments is through the `.yaml` scripts, which provides more readable data structure than `.json` files.
+We have provided an [example configuration script](https://github.com/Yinghao-Li/MUBen/blob/main/scripts/config-example.yaml) within the [./scripts/](https://github.com/Yinghao-Li/MUBen/tree/main/scripts) directory, which runs GIN on the FreeSolv dataset with deterministic ("none") UQ method.
+To use it to specify arguments, we can run the python program with
+```bash
+PYTHONPATH="." CUDA_VISIBLE_DEVICES=0 python ./run/run.py ./scripts/config-example.yaml
+```
+This approach could be helpful while debugging the code on VSCode.
 
-### Calculating Metrics
+## Calculating Metrics
 
 During training, we only calculate metrics necessary for early stopping and simple prediction performance evaluation.
 To get other metrics, you need to use the `./assist/results_get_metrics.py` file.
 
-Specifically, you need to save the model predictions by **not** setting `--disable_dataset_saving`.
-The results are saved as `./<result_folder>/<dataset_name>/<model_name>/<uncertainty_method>/seed-<seed>/preds/<test_idx>.pt` files.
-When the training is finished, you can run the `./assist/results_get_metrics.py` file to generate all metrics for your model predictions.
+After training, the results are saved as `./<result_folder>/<dataset_name>/<model_name>/<uncertainty_method>/seed-<seed>/preds/<test_idx>.pt` files.
+You can run the `./assist/results_get_metrics.py` file to generate all metrics for your model predictions.
 For example:
 ```bash
-PYTHONPATH="." python ./assist/results_get_metrics.py ./scripts/config_metrics.json
+PYTHONPATH="." python ./assist/results_get_metrics.py [arguments]
 ```
-Make sure the hyper-parameters in the configuration file are updated to your needs.
-
-The metrics will be saved in the `./<result_folder>/RESULTS/<model_name>-<dataset_name>.csv` files.
-~~Notice that these files already exist in the repo if you keep the default `--result_folder=./output` argument and you need to check whether it is updated to reveal your experiment results.~~
-
-### Results
+Make sure the arguments are updated to your needs.
 
-We provided a more comprehensive copy of our experiment results [here](https://github.com/Yinghao-Li/UncertaintyBenchmark/tree/main/output) that are presented in the tables in our paper's appendix.
-We hope it can ease some effort if you want to further analyze the behavior of our backbone models and uncertainty quantification methods. 
 
-## 4. ONGOING WORKS
+## Experimental Results
 
-### 4.1. Active Learning
+We have made our experimental results available in the [./reports/](https://github.com/Yinghao-Li/MUBen/tree/main/reports) directory.
+These results are organized into different folders based on the nature of the experiments:
 
-We are developing code to integrate *active learning* into the pipeline.
-Specifically, we assume we have a small set of labeled data points (`--n_init_instances`) at the beginning.
-Within each active learning iteration, we use the labeled dataset to fine-tune the model parameters and select a batch of data points (`--n_al_select`) from the unlabeled set with the least predicted certainty (*i.e.*, max predicted entropy for classification and max predicted variance for regression).
-The process is repeated for several loops (`--n_al_loops`), and the intermediate performance is tracked.
+- `primary`: Contains the most comprehensive set of results derived from experiments on scaffold-split datasets.
+- `random`: Includes results from experiments conducted on datasets that were split randomly.
+- `frozen`: Features results from experiments where the pre-trained model's weights were frozen, except for the last output layer, which was updatable.
+- `distribution`: Offers results from the QM9 dataset, where the test set was categorized into five bins based on the average Tanimoto similarities to the training scaffolds.
 
-The code is still under construction and currently is **only available under the `dev` branch**.
-In addition, several points are worth attention:
+Files within these directories are named following the pattern `<backbone>-<dataset>.csv`.
+Each file provides a comparison of different UQ methods.
+The rows detail the performance of each UQ method, while the columns display the mean and standard deviation from three random runs for each metric.
 
-- Currently, only DNN and ChemBERTa backbones are supported (`./run/dnn_al.py` and `./run/chemberta_al.py`). Migrating AL to other backbones is not difficult but requires updating some Trainer functions if they are reloaded.
-- To enable active learning, make sure you set `--enable_active_learning` to `true`.
-- Currently, Deep Ensembles is not supported for AL.
-- We cannot guarantee the correctness of our implementation. If you notice any abnormalities in the code, please do not hesitate to post an issue.
-
-One example is
-```bash
-python ./run/dnn_al.py \
-  --enable_active_learning \
-  --n_init_instances 100 \
-  --n_al_loops 20 \
-  --n_al_select 20 \
-  # other model and training hyper-parameters...
-```
+Additional post-processing scripts can be found in the [./assist/](https://github.com/Yinghao-Li/MUBen/tree/main/assist) directory, which include files starting with `plot_` or `results_`.
+These scripts are useful for further analysis and visualization of the experimental data.
 
-## 5. CITATION
+## Citation
 
 If you find our work helpful, please consider citing it as
 ```latex
 @misc{li2023muben,
     title={MUBen: Benchmarking the Uncertainty of Pre-Trained Models for Molecular Property Prediction},
     author={Yinghao Li and Lingkai Kong and Yuanqi Du and Yue Yu and Yuchen Zhuang and Wenhao Mu and Chao Zhang},
     year={2023},
```

### Comparing `muben-0.0.1/muben.egg-info/SOURCES.txt` & `muben-0.0.2/muben.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -87,13 +87,13 @@
 muben/uncertainty/sgld.py
 muben/uncertainty/swag.py
 muben/uncertainty/ts.py
 muben/uncertainty/evidential/__init__.py
 muben/uncertainty/evidential/loss.py
 muben/uncertainty/evidential/model.py
 muben/utils/__init__.py
-muben/utils/argparser.py
 muben/utils/chem.py
 muben/utils/io.py
 muben/utils/macro.py
 muben/utils/metrics.py
-muben/utils/selectors.py
+muben/utils/selectors.py
+test/test.py
```

### Comparing `muben-0.0.1/setup.py` & `muben-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="muben",
-    version="0.0.1",
+    version="0.0.2",
     author="Yinghao Li",
     author_email="yinghaoli@gatech.edu",
     license="MIT",
     url="https://github.com/Yinghao-Li/MUBen",
     description="Benchmark for molecular uncertainty estimation.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

