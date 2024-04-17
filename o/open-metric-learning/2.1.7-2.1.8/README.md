# Comparing `tmp/open-metric-learning-2.1.7.tar.gz` & `tmp/open_metric_learning-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/open-metric-learning-2.1.7.tar", last modified: Mon Apr  1 16:12:26 2024, max compression
+gzip compressed data, was "dist/open_metric_learning-2.1.8.tar", last modified: Wed Apr 17 19:10:11 2024, max compression
```

## Comparing `open-metric-learning-2.1.7.tar` & `open_metric_learning-2.1.8.tar`

### file list

```diff
@@ -1,233 +1,232 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.010306 open-metric-learning-2.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    33670 2024-04-01 16:12:26.010306 open-metric-learning-2.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    31845 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.986306 open-metric-learning-2.1.7/oml/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.986306 open-metric-learning-2.1.7/oml/configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.990306 open-metric-learning-2.1.7/oml/configs/criterion/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/criterion/arcface.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/criterion/mlp_arcface.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/criterion/surrogate_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/criterion/triplet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/criterion/triplet_plain.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/criterion/triplet_with_miner.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.990306 open-metric-learning-2.1.7/oml/configs/extractor/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/extractor/extractor_with_mlp.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/extractor/resnet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/extractor/vit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/extractor/vit_clip.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/extractor/vit_unicom.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.990306 open-metric-learning-2.1.7/oml/configs/logger/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/logger/mlflow.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/logger/neptune.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/logger/tensorboard.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/logger/wandb.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.990306 open-metric-learning-2.1.7/oml/configs/miner/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/miner/all_triplets.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/miner/hard_cluster.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/miner/hard_triplets.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/miner/miner_with_bank.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/miner/n_hard_triplets.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/miner/triplets_with_memory.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.990306 open-metric-learning-2.1.7/oml/configs/optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/optimizer/adadelta.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/optimizer/adagrad.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/optimizer/adam.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/optimizer/adamax.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/optimizer/adamw.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/optimizer/asgd.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/optimizer/lbfgs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/optimizer/rmsprop.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/optimizer/rprop.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/optimizer/sgd.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.994306 open-metric-learning-2.1.7/oml/configs/pairwise_model/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/pairwise_model/concat_siamese.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/pairwise_model/linear_siamese.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/pairwise_model/trivial_distance_siamese.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.994306 open-metric-learning-2.1.7/oml/configs/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/postprocessor/pairwise_embeddings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/postprocessor/pairwise_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.994306 open-metric-learning-2.1.7/oml/configs/sampler/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/sampler/balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/sampler/category_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/sampler/distinct_category_balance.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.994306 open-metric-learning-2.1.7/oml/configs/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/scheduler/cosine_annealing.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/scheduler/cyclic.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/scheduler/exponential.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/scheduler/lambda.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/scheduler/multi_step.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/scheduler/multiplicative.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/scheduler/one_cycle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/scheduler/reduce_on_plateau.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/scheduler/step.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.994306 open-metric-learning-2.1.7/oml/configs/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/transforms/augs_albu.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/transforms/augs_hypvit_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/transforms/augs_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/transforms/norm_albu.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/transforms/norm_resize_albu.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/transforms/norm_resize_albu_clip.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/transforms/norm_resize_hypvit_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/transforms/norm_resize_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/transforms/norm_torch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/configs/transforms/unicom_transforms.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.994306 open-metric-learning-2.1.7/oml/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12636 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/datasets/list_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/datasets/pairs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/datasets/triplet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.998306 open-metric-learning-2.1.7/oml/ddp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/ddp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/ddp/patching.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/ddp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.998306 open-metric-learning-2.1.7/oml/functional/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/functional/label_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/functional/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)    25080 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/functional/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.998306 open-metric-learning-2.1.7/oml/inference/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/inference/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/inference/flat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/inference/pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.998306 open-metric-learning-2.1.7/oml/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/interfaces/criterions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/interfaces/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/interfaces/loggers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/interfaces/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/interfaces/miners.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/interfaces/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/interfaces/retrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/interfaces/samplers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.998306 open-metric-learning-2.1.7/oml/lightning/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/lightning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.998306 open-metric-learning-2.1.7/oml/lightning/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/lightning/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8972 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/lightning/callbacks/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:25.998306 open-metric-learning-2.1.7/oml/lightning/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/lightning/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/lightning/modules/ddp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/lightning/modules/extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/lightning/modules/pairwise_postprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.002306 open-metric-learning-2.1.7/oml/lightning/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/lightning/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/lightning/pipelines/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/lightning/pipelines/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/lightning/pipelines/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/lightning/pipelines/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/lightning/pipelines/train_postprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/lightning/pipelines/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.002306 open-metric-learning-2.1.7/oml/losses/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/losses/arcface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/losses/surrogate_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/losses/triplet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.002306 open-metric-learning-2.1.7/oml/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/metrics/accumulation.py
--rw-r--r--   0 runner    (1001) docker     (127)    16385 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/metrics/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/metrics/triplets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.002306 open-metric-learning-2.1.7/oml/miners/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/miners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/miners/cross_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/miners/inbatch_all_tri.py
--rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/miners/inbatch_hard_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/miners/inbatch_hard_tri.py
--rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/miners/inbatch_nhard_tri.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/miners/miner_with_bank.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/miners/pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.002306 open-metric-learning-2.1.7/oml/models/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.002306 open-metric-learning-2.1.7/oml/models/meta/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/meta/projection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/meta/siamese.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.002306 open-metric-learning-2.1.7/oml/models/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/resnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/resnet/extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/resnet/pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.002306 open-metric-learning-2.1.7/oml/models/vit_clip/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_clip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.002306 open-metric-learning-2.1.7/oml/models/vit_clip/external/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_clip/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_clip/external/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6598 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_clip/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.006306 open-metric-learning-2.1.7/oml/models/vit_dino/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_dino/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.006306 open-metric-learning-2.1.7/oml/models/vit_dino/external/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_dino/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_dino/external/hubconf.py
--rw-r--r--   0 runner    (1001) docker     (127)    13388 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_dino/external/vision_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.006306 open-metric-learning-2.1.7/oml/models/vit_dino/external_v2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_dino/external_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_dino/external_v2/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_dino/external_v2/hubconf.py
--rw-r--r--   0 runner    (1001) docker     (127)    21318 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_dino/external_v2/vision_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10541 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_dino/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.006306 open-metric-learning-2.1.7/oml/models/vit_unicom/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_unicom/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.006306 open-metric-learning-2.1.7/oml/models/vit_unicom/external/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_unicom/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_unicom/external/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11680 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_unicom/external/vision_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/models/vit_unicom/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.006306 open-metric-learning-2.1.7/oml/registry/
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/registry/loggers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/registry/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/registry/miners.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/registry/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/registry/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/registry/postprocessors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/registry/samplers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/registry/schedulers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/registry/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.006306 open-metric-learning-2.1.7/oml/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/retrieval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.006306 open-metric-learning-2.1.7/oml/retrieval/postprocessors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/retrieval/postprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10876 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/retrieval/postprocessors/pairwise.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.006306 open-metric-learning-2.1.7/oml/samplers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/samplers/balance.py
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/samplers/category_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/samplers/distinct_category_balance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.006306 open-metric-learning-2.1.7/oml/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.010306 open-metric-learning-2.1.7/oml/transforms/images/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/transforms/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/transforms/images/albumentations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/transforms/images/torchvision.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/transforms/images/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.010306 open-metric-learning-2.1.7/oml/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/utils/dataframe_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/utils/download_mock_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.010306 open-metric-learning-2.1.7/oml/utils/images/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/utils/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/utils/images/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     6600 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/utils/images/images_resize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    16347 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/utils/misc_torch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/oml/utils/remote_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.010306 open-metric-learning-2.1.7/open_metric_learning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    33670 2024-04-01 16:12:25.000000 open-metric-learning-2.1.7/open_metric_learning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-04-01 16:12:25.000000 open-metric-learning-2.1.7/open_metric_learning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 16:12:25.000000 open-metric-learning-2.1.7/open_metric_learning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-01 16:12:25.000000 open-metric-learning-2.1.7/open_metric_learning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-01 16:12:25.000000 open-metric-learning-2.1.7/open_metric_learning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-01 16:12:26.010306 open-metric-learning-2.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 16:12:26.010306 open-metric-learning-2.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/tests/test_build_readme.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-01 16:12:12.000000 open-metric-learning-2.1.7/tests/test_outdated_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.830245 open_metric_learning-2.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    34019 2024-04-17 19:10:11.830245 open_metric_learning-2.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    32194 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.802244 open_metric_learning-2.1.8/oml/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.802244 open_metric_learning-2.1.8/oml/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.806244 open_metric_learning-2.1.8/oml/configs/criterion/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/criterion/arcface.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/criterion/mlp_arcface.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/criterion/surrogate_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/criterion/triplet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/criterion/triplet_plain.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/criterion/triplet_with_miner.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.806244 open_metric_learning-2.1.8/oml/configs/extractor/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/extractor/extractor_with_mlp.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/extractor/resnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/extractor/vit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/extractor/vit_clip.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/extractor/vit_unicom.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.806244 open_metric_learning-2.1.8/oml/configs/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/logger/clearml.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/logger/mlflow.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/logger/neptune.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/logger/tensorboard.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/logger/wandb.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.806244 open_metric_learning-2.1.8/oml/configs/miner/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/miner/all_triplets.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/miner/hard_cluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/miner/hard_triplets.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/miner/miner_with_bank.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/miner/n_hard_triplets.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/miner/triplets_with_memory.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.810244 open_metric_learning-2.1.8/oml/configs/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/optimizer/adadelta.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/optimizer/adagrad.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/optimizer/adam.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/optimizer/adamax.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/optimizer/adamw.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/optimizer/asgd.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/optimizer/lbfgs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/optimizer/rmsprop.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/optimizer/rprop.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/optimizer/sgd.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.810244 open_metric_learning-2.1.8/oml/configs/pairwise_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/pairwise_model/concat_siamese.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/pairwise_model/linear_siamese.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/pairwise_model/trivial_distance_siamese.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.810244 open_metric_learning-2.1.8/oml/configs/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/postprocessor/pairwise_embeddings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/postprocessor/pairwise_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.810244 open_metric_learning-2.1.8/oml/configs/sampler/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/sampler/balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/sampler/category_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/sampler/distinct_category_balance.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.810244 open_metric_learning-2.1.8/oml/configs/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/scheduler/cosine_annealing.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/scheduler/cyclic.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/scheduler/exponential.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/scheduler/lambda.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/scheduler/multi_step.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/scheduler/multiplicative.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/scheduler/one_cycle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/scheduler/reduce_on_plateau.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/scheduler/step.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.814244 open_metric_learning-2.1.8/oml/configs/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/transforms/augs_albu.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/transforms/augs_hypvit_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/transforms/augs_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/transforms/norm_albu.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/transforms/norm_resize_albu.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/transforms/norm_resize_albu_clip.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/transforms/norm_resize_hypvit_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/transforms/norm_resize_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/transforms/norm_torch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/configs/transforms/unicom_transforms.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.814244 open_metric_learning-2.1.8/oml/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12636 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/datasets/list_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/datasets/pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.814244 open_metric_learning-2.1.8/oml/ddp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/ddp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/ddp/patching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/ddp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.814244 open_metric_learning-2.1.8/oml/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/functional/label_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/functional/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24429 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/functional/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.814244 open_metric_learning-2.1.8/oml/inference/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/inference/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/inference/flat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/inference/pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.814244 open_metric_learning-2.1.8/oml/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/interfaces/criterions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/interfaces/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/interfaces/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/interfaces/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/interfaces/miners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/interfaces/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/interfaces/retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/interfaces/samplers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.814244 open_metric_learning-2.1.8/oml/lightning/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/lightning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.814244 open_metric_learning-2.1.8/oml/lightning/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/lightning/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8972 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/lightning/callbacks/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.818245 open_metric_learning-2.1.8/oml/lightning/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/lightning/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/lightning/modules/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/lightning/modules/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/lightning/modules/pairwise_postprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.818245 open_metric_learning-2.1.8/oml/lightning/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/lightning/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/lightning/pipelines/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/lightning/pipelines/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/lightning/pipelines/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/lightning/pipelines/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/lightning/pipelines/train_postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/lightning/pipelines/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.818245 open_metric_learning-2.1.8/oml/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5958 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/losses/arcface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/losses/surrogate_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/losses/triplet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.818245 open_metric_learning-2.1.8/oml/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/metrics/accumulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16385 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/metrics/embeddings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.818245 open_metric_learning-2.1.8/oml/miners/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/miners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/miners/cross_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/miners/inbatch_all_tri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/miners/inbatch_hard_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/miners/inbatch_hard_tri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/miners/inbatch_nhard_tri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/miners/miner_with_bank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/miners/pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.818245 open_metric_learning-2.1.8/oml/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.822245 open_metric_learning-2.1.8/oml/models/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/models/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/models/meta/projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/models/meta/siamese.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.822245 open_metric_learning-2.1.8/oml/models/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/models/resnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8164 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/models/resnet/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/models/resnet/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.822245 open_metric_learning-2.1.8/oml/models/vit_clip/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/models/vit_clip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.822245 open_metric_learning-2.1.8/oml/models/vit_clip/external/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/models/vit_clip/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/models/vit_clip/external/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6598 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/models/vit_clip/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.822245 open_metric_learning-2.1.8/oml/models/vit_dino/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/models/vit_dino/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.822245 open_metric_learning-2.1.8/oml/models/vit_dino/external/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/models/vit_dino/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/models/vit_dino/external/hubconf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13388 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/models/vit_dino/external/vision_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.822245 open_metric_learning-2.1.8/oml/models/vit_dino/external_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/models/vit_dino/external_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/models/vit_dino/external_v2/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/models/vit_dino/external_v2/hubconf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21318 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/models/vit_dino/external_v2/vision_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10541 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/models/vit_dino/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.822245 open_metric_learning-2.1.8/oml/models/vit_unicom/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/models/vit_unicom/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.822245 open_metric_learning-2.1.8/oml/models/vit_unicom/external/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/models/vit_unicom/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/models/vit_unicom/external/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11680 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/models/vit_unicom/external/vision_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/models/vit_unicom/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.826244 open_metric_learning-2.1.8/oml/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/registry/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/registry/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/registry/miners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/registry/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/registry/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/registry/postprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/registry/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/registry/schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/registry/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.826244 open_metric_learning-2.1.8/oml/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/retrieval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.826244 open_metric_learning-2.1.8/oml/retrieval/postprocessors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/retrieval/postprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10876 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/retrieval/postprocessors/pairwise.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.826244 open_metric_learning-2.1.8/oml/samplers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/samplers/balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/samplers/category_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/samplers/distinct_category_balance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.826244 open_metric_learning-2.1.8/oml/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.826244 open_metric_learning-2.1.8/oml/transforms/images/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/transforms/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/transforms/images/albumentations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/transforms/images/torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/transforms/images/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.826244 open_metric_learning-2.1.8/oml/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/utils/dataframe_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/utils/download_mock_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.830245 open_metric_learning-2.1.8/oml/utils/images/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/utils/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/utils/images/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6600 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/utils/images/images_resize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16347 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/utils/misc_torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/oml/utils/remote_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.830245 open_metric_learning-2.1.8/open_metric_learning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    34019 2024-04-17 19:10:11.000000 open_metric_learning-2.1.8/open_metric_learning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6085 2024-04-17 19:10:11.000000 open_metric_learning-2.1.8/open_metric_learning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 19:10:11.000000 open_metric_learning-2.1.8/open_metric_learning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-17 19:10:11.000000 open_metric_learning-2.1.8/open_metric_learning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-17 19:10:11.000000 open_metric_learning-2.1.8/open_metric_learning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-17 19:10:11.830245 open_metric_learning-2.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:10:11.830245 open_metric_learning-2.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/tests/test_build_readme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-17 19:09:57.000000 open_metric_learning-2.1.8/tests/test_outdated_docs.py
```

### Comparing `open-metric-learning-2.1.7/LICENSE` & `open_metric_learning-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/PKG-INFO` & `open_metric_learning-2.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-metric-learning
-Version: 2.1.7
+Version: 2.1.8
 Summary: OML is a PyTorch-based framework to train and validate the models producing high-quality embeddings.
 Home-page: https://github.com/OML-Team/open-metric-learning
 Author: Shabanov Aleksei
 Author-email: shabanoff.aleksei@gmail.com
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/OML-Team/open-metric-learning
 Project-URL: Bug Tracker, https://github.com/OML-Team/open-metric-learning/issues
@@ -58,15 +58,16 @@
 
 <div align="center">
 <a href="https://docs.neptune.ai/integrations/community_developed/" target="_blank"><img src="https://security.neptune.ai/api/share/b707f1e8-e287-4f01-b590-39a6fa7e9faa/logo.png" width="100"/></a>ㅤㅤ
 <a href="https://www.newyorker.de/" target="_blank"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d8/New_Yorker.svg/1280px-New_Yorker.svg.png" width="100"/></a>ㅤㅤ
 <a href="https://www.epoch8.co/" target="_blank"><img src="https://i.ibb.co/GdNVTyt/Screenshot-2023-07-04-at-11-19-24.png" width="100"/></a>ㅤㅤ
 <a href="https://www.meituan.com" target="_blank"><img src="https://upload.wikimedia.org/wikipedia/commons/6/61/Meituan_English_Logo.png" width="100"/></a>ㅤㅤ
 <a href="https://constructor.io/" target="_blank"><img src="https://rethink.industries/wp-content/uploads/2022/04/constructor.io-logo.png" width="100"/></a>ㅤㅤ
-<a href="https://edgify.ai/" target="_blank"><img src="https://edgify.ai/wp-content/themes/edgifyai/dist/assets/logo.svg" width="100" height="30"/></a>
+<a href="https://edgify.ai/" target="_blank"><img src="https://edgify.ai/wp-content/themes/edgifyai/dist/assets/logo.svg" width="100" height="30"/></a>ㅤㅤ
+<a href="https://inspector-cloud.ru/" target="_blank"><img src="https://thumb.tildacdn.com/tild6533-6433-4137-a266-613963373637/-/resize/540x/-/format/webp/photo.png" width="100" height="30"/></a>
 
 
 <a href="https://www.ox.ac.uk/" target="_blank"><img src="https://i.ibb.co/zhWL6tD/21-05-2019-16-08-10-6922268.png" width="120"/></a>ㅤㅤ
 <a href="https://www.hse.ru/en/" target="_blank"><img src="https://www.hse.ru/data/2020/11/16/1367274044/HSE_University_blue.jpg.(230x86x123).jpg" width="100"/></a>
 
 There is a number of people from
 [Oxford](https://www.ox.ac.uk/) and
@@ -429,15 +430,21 @@
 from oml.lightning.callbacks.metric import MetricValCallback
 from oml.losses.triplet import TripletLossWithMiner
 from oml.metrics.embeddings import EmbeddingMetrics
 from oml.miners.inbatch_all_tri import AllTripletsMiner
 from oml.models import ViTExtractor
 from oml.samplers.balance import BalanceSampler
 from oml.utils.download_mock_dataset import download_mock_dataset
-from oml.lightning.pipelines.logging import NeptunePipelineLogger, TensorBoardPipelineLogger, WandBPipelineLogger, MLFlowPipelineLogger
+from oml.lightning.pipelines.logging import (
+    ClearMLPipelineLogger,
+    MLFlowPipelineLogger,
+    NeptunePipelineLogger,
+    TensorBoardPipelineLogger,
+    WandBPipelineLogger,
+)
 
 dataset_root = "mock_dataset/"
 df_train, df_val = download_mock_dataset(dataset_root)
 
 # model
 extractor = ViTExtractor("vits16_dino", arch="vits16", normalise_features=False)
 
@@ -463,14 +470,17 @@
 # import os
 # os.environ["WANDB_API_KEY"] = ""
 # logger = WandBPipelineLogger(project="test_project", log_model=False)
 
 # 4) Logging with MLFlow locally
 # logger = MLFlowPipelineLogger(experiment_name="exp", tracking_uri="file:./ml-runs")
 
+# 5) Logging with ClearML
+# logger = ClearMLPipelineLogger(project_name="exp", task_name="test")
+
 # run
 pl_model = ExtractorModule(extractor, criterion, optimizer)
 trainer = pl.Trainer(max_epochs=3, callbacks=[metric_callback], num_sanity_val_steps=0, logger=logger)
 trainer.fit(pl_model, train_dataloaders=train_loader, val_dataloaders=val_loader)
 
 ```
 [comment]:lightning-end
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: open-metric-learning Version: 2.1.7 Summary: OML is
+Metadata-Version: 2.1 Name: open-metric-learning Version: 2.1.8 Summary: OML is
 a PyTorch-based framework to train and validate the models producing high-
 quality embeddings. Home-page: https://github.com/OML-Team/open-metric-learning
 Author: Shabanov Aleksei Author-email: shabanoff.aleksei@gmail.com License:
 Apache License 2.0 Project-URL: Homepage, https://github.com/OML-Team/open-
 metric-learning Project-URL: Bug Tracker, https://github.com/OML-Team/open-
 metric-learning/issues Keywords: data-science,computer-vision,deep-
 learning,pytorch,metric-learning,representation-learning,pytorch-lightning
@@ -42,22 +42,24 @@
                                 ### Trusted by
  _[_h_t_t_p_s_:_/_/_s_e_c_u_r_i_t_y_._n_e_p_t_u_n_e_._a_i_/_a_p_i_/_s_h_a_r_e_/_b_7_0_7_f_1_e_8_-_e_2_8_7_-_4_f_0_1_-_b_5_9_0_-_3_9_a_6_f_a_7_e_9_f_a_a_/
   _l_o_g_o_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/_u_p_l_o_a_d_._w_i_k_i_m_e_d_i_a_._o_r_g_/_w_i_k_i_p_e_d_i_a_/_c_o_m_m_o_n_s_/_t_h_u_m_b_/_d_/_d_8_/
   _N_e_w___Y_o_r_k_e_r_._s_v_g_/_1_2_8_0_p_x_-_N_e_w___Y_o_r_k_e_r_._s_v_g_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/_i_._i_b_b_._c_o_/_G_d_N_V_T_y_t_/
   _S_c_r_e_e_n_s_h_o_t_-_2_0_2_3_-_0_7_-_0_4_-_a_t_-_1_1_-_1_9_-_2_4_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/_u_p_l_o_a_d_._w_i_k_i_m_e_d_i_a_._o_r_g_/
        _w_i_k_i_p_e_d_i_a_/_c_o_m_m_o_n_s_/_6_/_6_1_/_M_e_i_t_u_a_n___E_n_g_l_i_s_h___L_o_g_o_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/
  _r_e_t_h_i_n_k_._i_n_d_u_s_t_r_i_e_s_/_w_p_-_c_o_n_t_e_n_t_/_u_p_l_o_a_d_s_/_2_0_2_2_/_0_4_/_c_o_n_s_t_r_u_c_t_o_r_._i_o_-_l_o_g_o_._p_n_g_]ã¤ã¤
- _[_h_t_t_p_s_:_/_/_e_d_g_i_f_y_._a_i_/_w_p_-_c_o_n_t_e_n_t_/_t_h_e_m_e_s_/_e_d_g_i_f_y_a_i_/_d_i_s_t_/_a_s_s_e_t_s_/_l_o_g_o_._s_v_g_]_[_h_t_t_p_s_:_/_/
- _i_._i_b_b_._c_o_/_z_h_W_L_6_t_D_/_2_1_-_0_5_-_2_0_1_9_-_1_6_-_0_8_-_1_0_-_6_9_2_2_2_6_8_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/_w_w_w_._h_s_e_._r_u_/
-_d_a_t_a_/_2_0_2_0_/_1_1_/_1_6_/_1_3_6_7_2_7_4_0_4_4_/_H_S_E___U_n_i_v_e_r_s_i_t_y___b_l_u_e_._j_p_g_._(_2_3_0_x_8_6_x_1_2_3_)_._j_p_g_]There is a
-   number of people from [Oxford](https://www.ox.ac.uk/) and [HSE](https://
-www.hse.ru/en/) universities who have used OML in their theses. [[1]](https://
- github.com/nilomr/open-metric-learning/tree/great-tit/great-tit-train) [[2]]
- (https://github.com/nastygorodi/PROJECT-Deep_Metric_Learning) [[3]](https://
-              github.com/nik-fedorov/term_paper_metric_learning)
+  _[_h_t_t_p_s_:_/_/_e_d_g_i_f_y_._a_i_/_w_p_-_c_o_n_t_e_n_t_/_t_h_e_m_e_s_/_e_d_g_i_f_y_a_i_/_d_i_s_t_/_a_s_s_e_t_s_/_l_o_g_o_._s_v_g_]ã¤ã¤
+_[_h_t_t_p_s_:_/_/_t_h_u_m_b_._t_i_l_d_a_c_d_n_._c_o_m_/_t_i_l_d_6_5_3_3_-_6_4_3_3_-_4_1_3_7_-_a_2_6_6_-_6_1_3_9_6_3_3_7_3_6_3_7_/_-_/_r_e_s_i_z_e_/_5_4_0_x_/
+    _-_/_f_o_r_m_a_t_/_w_e_b_p_/_p_h_o_t_o_._p_n_g_]_[_h_t_t_p_s_:_/_/_i_._i_b_b_._c_o_/_z_h_W_L_6_t_D_/_2_1_-_0_5_-_2_0_1_9_-_1_6_-_0_8_-_1_0_-
+      _6_9_2_2_2_6_8_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/_w_w_w_._h_s_e_._r_u_/_d_a_t_a_/_2_0_2_0_/_1_1_/_1_6_/_1_3_6_7_2_7_4_0_4_4_/
+  _H_S_E___U_n_i_v_e_r_s_i_t_y___b_l_u_e_._j_p_g_._(_2_3_0_x_8_6_x_1_2_3_)_._j_p_g_]There is a number of people from
+[Oxford](https://www.ox.ac.uk/) and [HSE](https://www.hse.ru/en/) universities
+who have used OML in their theses. [[1]](https://github.com/nilomr/open-metric-
+learning/tree/great-tit/great-tit-train) [[2]](https://github.com/nastygorodi/
+      PROJECT-Deep_Metric_Learning) [[3]](https://github.com/nik-fedorov/
+                          term_paper_metric_learning)
 ## [FAQ](https://open-metric-learning.readthedocs.io/en/latest/oml/faq.html)
 Why do I need OML?
 You may think *"If I need image embeddings I can simply train a vanilla
 classifier and take its penultimate layer"*. Well, it makes sense as a starting
 point. But there are several possible drawbacks: * If you want to use
 embeddings to perform searching you need to calculate some distance among them
 (for example, cosine or L2). Usually, **you don't directly optimize these
@@ -266,36 +268,38 @@
 from oml.datasets.base import DatasetQueryGallery, DatasetWithLabels from
 oml.lightning.modules.extractor import ExtractorModule from
 oml.lightning.callbacks.metric import MetricValCallback from oml.losses.triplet
 import TripletLossWithMiner from oml.metrics.embeddings import EmbeddingMetrics
 from oml.miners.inbatch_all_tri import AllTripletsMiner from oml.models import
 ViTExtractor from oml.samplers.balance import BalanceSampler from
 oml.utils.download_mock_dataset import download_mock_dataset from
-oml.lightning.pipelines.logging import NeptunePipelineLogger,
-TensorBoardPipelineLogger, WandBPipelineLogger, MLFlowPipelineLogger
-dataset_root = "mock_dataset/" df_train, df_val = download_mock_dataset
-(dataset_root) # model extractor = ViTExtractor("vits16_dino", arch="vits16",
-normalise_features=False) # train optimizer = torch.optim.SGD
-(extractor.parameters(), lr=1e-6) train_dataset = DatasetWithLabels(df_train,
-dataset_root=dataset_root) criterion = TripletLossWithMiner(margin=0.1,
-miner=AllTripletsMiner()) batch_sampler = BalanceSampler
-(train_dataset.get_labels(), n_labels=2, n_instances=3) train_loader =
-torch.utils.data.DataLoader(train_dataset, batch_sampler=batch_sampler) # val
-val_dataset = DatasetQueryGallery(df_val, dataset_root=dataset_root) val_loader
-= torch.utils.data.DataLoader(val_dataset, batch_size=4) metric_callback =
-MetricValCallback(metric=EmbeddingMetrics(extra_keys=
-[train_dataset.paths_key,]), log_images=True) # 1) Logging with Tensorboard
-logger = TensorBoardPipelineLogger(".") # 2) Logging with Neptune # logger =
+oml.lightning.pipelines.logging import ( ClearMLPipelineLogger,
+MLFlowPipelineLogger, NeptunePipelineLogger, TensorBoardPipelineLogger,
+WandBPipelineLogger, ) dataset_root = "mock_dataset/" df_train, df_val =
+download_mock_dataset(dataset_root) # model extractor = ViTExtractor
+("vits16_dino", arch="vits16", normalise_features=False) # train optimizer =
+torch.optim.SGD(extractor.parameters(), lr=1e-6) train_dataset =
+DatasetWithLabels(df_train, dataset_root=dataset_root) criterion =
+TripletLossWithMiner(margin=0.1, miner=AllTripletsMiner()) batch_sampler =
+BalanceSampler(train_dataset.get_labels(), n_labels=2, n_instances=3)
+train_loader = torch.utils.data.DataLoader(train_dataset,
+batch_sampler=batch_sampler) # val val_dataset = DatasetQueryGallery(df_val,
+dataset_root=dataset_root) val_loader = torch.utils.data.DataLoader
+(val_dataset, batch_size=4) metric_callback = MetricValCallback
+(metric=EmbeddingMetrics(extra_keys=[train_dataset.paths_key,]),
+log_images=True) # 1) Logging with Tensorboard logger =
+TensorBoardPipelineLogger(".") # 2) Logging with Neptune # logger =
 NeptunePipelineLogger(api_key="", project="", log_model_checkpoints=False) # 3)
 Logging with Weights and Biases # import os # os.environ["WANDB_API_KEY"] = ""
 # logger = WandBPipelineLogger(project="test_project", log_model=False) # 4)
 Logging with MLFlow locally # logger = MLFlowPipelineLogger
-(experiment_name="exp", tracking_uri="file:./ml-runs") # run pl_model =
-ExtractorModule(extractor, criterion, optimizer) trainer = pl.Trainer
-(max_epochs=3, callbacks=[metric_callback], num_sanity_val_steps=0,
+(experiment_name="exp", tracking_uri="file:./ml-runs") # 5) Logging with
+ClearML # logger = ClearMLPipelineLogger(project_name="exp", task_name="test")
+# run pl_model = ExtractorModule(extractor, criterion, optimizer) trainer =
+pl.Trainer(max_epochs=3, callbacks=[metric_callback], num_sanity_val_steps=0,
 logger=logger) trainer.fit(pl_model, train_dataloaders=train_loader,
 val_dataloaders=val_loader) ``` [comment]:lightning-end
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/drive/
 1bVUgdBGWvQgCkba2YtaIRVlUQUz7Q60Z?usp=share_link) Using a trained model for
 retrieval
 [comment]:usage-retrieval-start ```python import torch from oml.const import
```

### Comparing `open-metric-learning-2.1.7/README.md` & `open_metric_learning-2.1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 
 <div align="center">
 <a href="https://docs.neptune.ai/integrations/community_developed/" target="_blank"><img src="https://security.neptune.ai/api/share/b707f1e8-e287-4f01-b590-39a6fa7e9faa/logo.png" width="100"/></a>ㅤㅤ
 <a href="https://www.newyorker.de/" target="_blank"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d8/New_Yorker.svg/1280px-New_Yorker.svg.png" width="100"/></a>ㅤㅤ
 <a href="https://www.epoch8.co/" target="_blank"><img src="https://i.ibb.co/GdNVTyt/Screenshot-2023-07-04-at-11-19-24.png" width="100"/></a>ㅤㅤ
 <a href="https://www.meituan.com" target="_blank"><img src="https://upload.wikimedia.org/wikipedia/commons/6/61/Meituan_English_Logo.png" width="100"/></a>ㅤㅤ
 <a href="https://constructor.io/" target="_blank"><img src="https://rethink.industries/wp-content/uploads/2022/04/constructor.io-logo.png" width="100"/></a>ㅤㅤ
-<a href="https://edgify.ai/" target="_blank"><img src="https://edgify.ai/wp-content/themes/edgifyai/dist/assets/logo.svg" width="100" height="30"/></a>
+<a href="https://edgify.ai/" target="_blank"><img src="https://edgify.ai/wp-content/themes/edgifyai/dist/assets/logo.svg" width="100" height="30"/></a>ㅤㅤ
+<a href="https://inspector-cloud.ru/" target="_blank"><img src="https://thumb.tildacdn.com/tild6533-6433-4137-a266-613963373637/-/resize/540x/-/format/webp/photo.png" width="100" height="30"/></a>
 
 
 <a href="https://www.ox.ac.uk/" target="_blank"><img src="https://i.ibb.co/zhWL6tD/21-05-2019-16-08-10-6922268.png" width="120"/></a>ㅤㅤ
 <a href="https://www.hse.ru/en/" target="_blank"><img src="https://www.hse.ru/data/2020/11/16/1367274044/HSE_University_blue.jpg.(230x86x123).jpg" width="100"/></a>
 
 There is a number of people from
 [Oxford](https://www.ox.ac.uk/) and
@@ -388,15 +389,21 @@
 from oml.lightning.callbacks.metric import MetricValCallback
 from oml.losses.triplet import TripletLossWithMiner
 from oml.metrics.embeddings import EmbeddingMetrics
 from oml.miners.inbatch_all_tri import AllTripletsMiner
 from oml.models import ViTExtractor
 from oml.samplers.balance import BalanceSampler
 from oml.utils.download_mock_dataset import download_mock_dataset
-from oml.lightning.pipelines.logging import NeptunePipelineLogger, TensorBoardPipelineLogger, WandBPipelineLogger, MLFlowPipelineLogger
+from oml.lightning.pipelines.logging import (
+    ClearMLPipelineLogger,
+    MLFlowPipelineLogger,
+    NeptunePipelineLogger,
+    TensorBoardPipelineLogger,
+    WandBPipelineLogger,
+)
 
 dataset_root = "mock_dataset/"
 df_train, df_val = download_mock_dataset(dataset_root)
 
 # model
 extractor = ViTExtractor("vits16_dino", arch="vits16", normalise_features=False)
 
@@ -422,14 +429,17 @@
 # import os
 # os.environ["WANDB_API_KEY"] = ""
 # logger = WandBPipelineLogger(project="test_project", log_model=False)
 
 # 4) Logging with MLFlow locally
 # logger = MLFlowPipelineLogger(experiment_name="exp", tracking_uri="file:./ml-runs")
 
+# 5) Logging with ClearML
+# logger = ClearMLPipelineLogger(project_name="exp", task_name="test")
+
 # run
 pl_model = ExtractorModule(extractor, criterion, optimizer)
 trainer = pl.Trainer(max_epochs=3, callbacks=[metric_callback], num_sanity_val_steps=0, logger=logger)
 trainer.fit(pl_model, train_dataloaders=train_loader, val_dataloaders=val_loader)
 
 ```
 [comment]:lightning-end
```

#### html2text {}

```diff
@@ -17,22 +17,24 @@
                                 ### Trusted by
  _[_h_t_t_p_s_:_/_/_s_e_c_u_r_i_t_y_._n_e_p_t_u_n_e_._a_i_/_a_p_i_/_s_h_a_r_e_/_b_7_0_7_f_1_e_8_-_e_2_8_7_-_4_f_0_1_-_b_5_9_0_-_3_9_a_6_f_a_7_e_9_f_a_a_/
   _l_o_g_o_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/_u_p_l_o_a_d_._w_i_k_i_m_e_d_i_a_._o_r_g_/_w_i_k_i_p_e_d_i_a_/_c_o_m_m_o_n_s_/_t_h_u_m_b_/_d_/_d_8_/
   _N_e_w___Y_o_r_k_e_r_._s_v_g_/_1_2_8_0_p_x_-_N_e_w___Y_o_r_k_e_r_._s_v_g_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/_i_._i_b_b_._c_o_/_G_d_N_V_T_y_t_/
   _S_c_r_e_e_n_s_h_o_t_-_2_0_2_3_-_0_7_-_0_4_-_a_t_-_1_1_-_1_9_-_2_4_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/_u_p_l_o_a_d_._w_i_k_i_m_e_d_i_a_._o_r_g_/
        _w_i_k_i_p_e_d_i_a_/_c_o_m_m_o_n_s_/_6_/_6_1_/_M_e_i_t_u_a_n___E_n_g_l_i_s_h___L_o_g_o_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/
  _r_e_t_h_i_n_k_._i_n_d_u_s_t_r_i_e_s_/_w_p_-_c_o_n_t_e_n_t_/_u_p_l_o_a_d_s_/_2_0_2_2_/_0_4_/_c_o_n_s_t_r_u_c_t_o_r_._i_o_-_l_o_g_o_._p_n_g_]ã¤ã¤
- _[_h_t_t_p_s_:_/_/_e_d_g_i_f_y_._a_i_/_w_p_-_c_o_n_t_e_n_t_/_t_h_e_m_e_s_/_e_d_g_i_f_y_a_i_/_d_i_s_t_/_a_s_s_e_t_s_/_l_o_g_o_._s_v_g_]_[_h_t_t_p_s_:_/_/
- _i_._i_b_b_._c_o_/_z_h_W_L_6_t_D_/_2_1_-_0_5_-_2_0_1_9_-_1_6_-_0_8_-_1_0_-_6_9_2_2_2_6_8_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/_w_w_w_._h_s_e_._r_u_/
-_d_a_t_a_/_2_0_2_0_/_1_1_/_1_6_/_1_3_6_7_2_7_4_0_4_4_/_H_S_E___U_n_i_v_e_r_s_i_t_y___b_l_u_e_._j_p_g_._(_2_3_0_x_8_6_x_1_2_3_)_._j_p_g_]There is a
-   number of people from [Oxford](https://www.ox.ac.uk/) and [HSE](https://
-www.hse.ru/en/) universities who have used OML in their theses. [[1]](https://
- github.com/nilomr/open-metric-learning/tree/great-tit/great-tit-train) [[2]]
- (https://github.com/nastygorodi/PROJECT-Deep_Metric_Learning) [[3]](https://
-              github.com/nik-fedorov/term_paper_metric_learning)
+  _[_h_t_t_p_s_:_/_/_e_d_g_i_f_y_._a_i_/_w_p_-_c_o_n_t_e_n_t_/_t_h_e_m_e_s_/_e_d_g_i_f_y_a_i_/_d_i_s_t_/_a_s_s_e_t_s_/_l_o_g_o_._s_v_g_]ã¤ã¤
+_[_h_t_t_p_s_:_/_/_t_h_u_m_b_._t_i_l_d_a_c_d_n_._c_o_m_/_t_i_l_d_6_5_3_3_-_6_4_3_3_-_4_1_3_7_-_a_2_6_6_-_6_1_3_9_6_3_3_7_3_6_3_7_/_-_/_r_e_s_i_z_e_/_5_4_0_x_/
+    _-_/_f_o_r_m_a_t_/_w_e_b_p_/_p_h_o_t_o_._p_n_g_]_[_h_t_t_p_s_:_/_/_i_._i_b_b_._c_o_/_z_h_W_L_6_t_D_/_2_1_-_0_5_-_2_0_1_9_-_1_6_-_0_8_-_1_0_-
+      _6_9_2_2_2_6_8_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/_w_w_w_._h_s_e_._r_u_/_d_a_t_a_/_2_0_2_0_/_1_1_/_1_6_/_1_3_6_7_2_7_4_0_4_4_/
+  _H_S_E___U_n_i_v_e_r_s_i_t_y___b_l_u_e_._j_p_g_._(_2_3_0_x_8_6_x_1_2_3_)_._j_p_g_]There is a number of people from
+[Oxford](https://www.ox.ac.uk/) and [HSE](https://www.hse.ru/en/) universities
+who have used OML in their theses. [[1]](https://github.com/nilomr/open-metric-
+learning/tree/great-tit/great-tit-train) [[2]](https://github.com/nastygorodi/
+      PROJECT-Deep_Metric_Learning) [[3]](https://github.com/nik-fedorov/
+                          term_paper_metric_learning)
 ## [FAQ](https://open-metric-learning.readthedocs.io/en/latest/oml/faq.html)
 Why do I need OML?
 You may think *"If I need image embeddings I can simply train a vanilla
 classifier and take its penultimate layer"*. Well, it makes sense as a starting
 point. But there are several possible drawbacks: * If you want to use
 embeddings to perform searching you need to calculate some distance among them
 (for example, cosine or L2). Usually, **you don't directly optimize these
@@ -241,36 +243,38 @@
 from oml.datasets.base import DatasetQueryGallery, DatasetWithLabels from
 oml.lightning.modules.extractor import ExtractorModule from
 oml.lightning.callbacks.metric import MetricValCallback from oml.losses.triplet
 import TripletLossWithMiner from oml.metrics.embeddings import EmbeddingMetrics
 from oml.miners.inbatch_all_tri import AllTripletsMiner from oml.models import
 ViTExtractor from oml.samplers.balance import BalanceSampler from
 oml.utils.download_mock_dataset import download_mock_dataset from
-oml.lightning.pipelines.logging import NeptunePipelineLogger,
-TensorBoardPipelineLogger, WandBPipelineLogger, MLFlowPipelineLogger
-dataset_root = "mock_dataset/" df_train, df_val = download_mock_dataset
-(dataset_root) # model extractor = ViTExtractor("vits16_dino", arch="vits16",
-normalise_features=False) # train optimizer = torch.optim.SGD
-(extractor.parameters(), lr=1e-6) train_dataset = DatasetWithLabels(df_train,
-dataset_root=dataset_root) criterion = TripletLossWithMiner(margin=0.1,
-miner=AllTripletsMiner()) batch_sampler = BalanceSampler
-(train_dataset.get_labels(), n_labels=2, n_instances=3) train_loader =
-torch.utils.data.DataLoader(train_dataset, batch_sampler=batch_sampler) # val
-val_dataset = DatasetQueryGallery(df_val, dataset_root=dataset_root) val_loader
-= torch.utils.data.DataLoader(val_dataset, batch_size=4) metric_callback =
-MetricValCallback(metric=EmbeddingMetrics(extra_keys=
-[train_dataset.paths_key,]), log_images=True) # 1) Logging with Tensorboard
-logger = TensorBoardPipelineLogger(".") # 2) Logging with Neptune # logger =
+oml.lightning.pipelines.logging import ( ClearMLPipelineLogger,
+MLFlowPipelineLogger, NeptunePipelineLogger, TensorBoardPipelineLogger,
+WandBPipelineLogger, ) dataset_root = "mock_dataset/" df_train, df_val =
+download_mock_dataset(dataset_root) # model extractor = ViTExtractor
+("vits16_dino", arch="vits16", normalise_features=False) # train optimizer =
+torch.optim.SGD(extractor.parameters(), lr=1e-6) train_dataset =
+DatasetWithLabels(df_train, dataset_root=dataset_root) criterion =
+TripletLossWithMiner(margin=0.1, miner=AllTripletsMiner()) batch_sampler =
+BalanceSampler(train_dataset.get_labels(), n_labels=2, n_instances=3)
+train_loader = torch.utils.data.DataLoader(train_dataset,
+batch_sampler=batch_sampler) # val val_dataset = DatasetQueryGallery(df_val,
+dataset_root=dataset_root) val_loader = torch.utils.data.DataLoader
+(val_dataset, batch_size=4) metric_callback = MetricValCallback
+(metric=EmbeddingMetrics(extra_keys=[train_dataset.paths_key,]),
+log_images=True) # 1) Logging with Tensorboard logger =
+TensorBoardPipelineLogger(".") # 2) Logging with Neptune # logger =
 NeptunePipelineLogger(api_key="", project="", log_model_checkpoints=False) # 3)
 Logging with Weights and Biases # import os # os.environ["WANDB_API_KEY"] = ""
 # logger = WandBPipelineLogger(project="test_project", log_model=False) # 4)
 Logging with MLFlow locally # logger = MLFlowPipelineLogger
-(experiment_name="exp", tracking_uri="file:./ml-runs") # run pl_model =
-ExtractorModule(extractor, criterion, optimizer) trainer = pl.Trainer
-(max_epochs=3, callbacks=[metric_callback], num_sanity_val_steps=0,
+(experiment_name="exp", tracking_uri="file:./ml-runs") # 5) Logging with
+ClearML # logger = ClearMLPipelineLogger(project_name="exp", task_name="test")
+# run pl_model = ExtractorModule(extractor, criterion, optimizer) trainer =
+pl.Trainer(max_epochs=3, callbacks=[metric_callback], num_sanity_val_steps=0,
 logger=logger) trainer.fit(pl_model, train_dataloaders=train_loader,
 val_dataloaders=val_loader) ``` [comment]:lightning-end
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/drive/
 1bVUgdBGWvQgCkba2YtaIRVlUQUz7Q60Z?usp=share_link) Using a trained model for
 retrieval
 [comment]:usage-retrieval-start ```python import torch from oml.const import
```

### Comparing `open-metric-learning-2.1.7/oml/const.py` & `open_metric_learning-2.1.8/oml/const.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/datasets/base.py` & `open_metric_learning-2.1.8/oml/datasets/base.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/datasets/list_dataset.py` & `open_metric_learning-2.1.8/oml/datasets/list_dataset.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/datasets/pairs.py` & `open_metric_learning-2.1.8/oml/datasets/pairs.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/ddp/patching.py` & `open_metric_learning-2.1.8/oml/ddp/patching.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/ddp/utils.py` & `open_metric_learning-2.1.8/oml/ddp/utils.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/functional/label_smoothing.py` & `open_metric_learning-2.1.8/oml/functional/label_smoothing.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/functional/losses.py` & `open_metric_learning-2.1.8/oml/functional/losses.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/functional/metrics.py` & `open_metric_learning-2.1.8/oml/functional/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 from collections import defaultdict
 from typing import Dict, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import torch
 from torch import Tensor
 
-from oml.losses.triplet import get_tri_ids_in_plain
 from oml.utils.misc import check_if_nonempty_positive_integers, clip_max
-from oml.utils.misc_torch import PCA, elementwise_dist, pairwise_dist, take_2d
+from oml.utils.misc_torch import PCA, pairwise_dist, take_2d
 
 TMetricsDict = Dict[str, Dict[Union[int, float], Union[float, Tensor]]]
 
 
 def calc_retrieval_metrics(
     distances: Tensor,
     mask_gt: Tensor,
@@ -200,31 +199,14 @@
     gallery_embeddings = embeddings[gallery_mask]
 
     distance_matrix = pairwise_dist(x1=query_embeddings, x2=gallery_embeddings, p=2)
 
     return distance_matrix
 
 
-def calculate_accuracy_on_triplets(embeddings: Tensor, reduce_mean: bool = True) -> Tensor:
-    assert embeddings.ndim == 2
-    assert embeddings.shape[0] % 3 == 0
-
-    anchor_ii, positive_ii, negative_ii = get_tri_ids_in_plain(n=len(embeddings))
-
-    pos_dists = elementwise_dist(x1=embeddings[anchor_ii], x2=embeddings[positive_ii])
-    neg_dists = elementwise_dist(x1=embeddings[anchor_ii], x2=embeddings[negative_ii])
-
-    acc = (pos_dists < neg_dists).float()
-
-    if reduce_mean:
-        return acc.mean()
-    else:
-        return acc
-
-
 def calc_cmc(gt_tops: Tensor, top_k: Tuple[int, ...]) -> List[Tensor]:
     """
     Function to compute Cumulative Matching Characteristics (CMC) at cutoffs ``top_k``.
 
     ``cmc@k`` for a given query equals to 1 if there is at least 1 instance related to this query in top ``k``
     gallery instances sorted by distances to the query, and 0 otherwise.
     The final ``cmc@k`` could be obtained by averaging the results calculated for each query.
@@ -611,10 +593,9 @@
     "TMetricsDict",
     "calc_retrieval_metrics",
     "calc_topological_metrics",
     "apply_mask_to_ignore",
     "calc_gt_mask",
     "calc_mask_to_ignore",
     "calc_distance_matrix",
-    "calculate_accuracy_on_triplets",
     "reduce_metrics",
 ]
```

### Comparing `open-metric-learning-2.1.7/oml/inference/abstract.py` & `open_metric_learning-2.1.8/oml/inference/abstract.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/inference/flat.py` & `open_metric_learning-2.1.8/oml/inference/flat.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/inference/pairs.py` & `open_metric_learning-2.1.8/oml/inference/pairs.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/interfaces/criterions.py` & `open_metric_learning-2.1.8/oml/interfaces/criterions.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/interfaces/datasets.py` & `open_metric_learning-2.1.8/oml/interfaces/datasets.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/interfaces/metrics.py` & `open_metric_learning-2.1.8/oml/interfaces/metrics.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/interfaces/miners.py` & `open_metric_learning-2.1.8/oml/interfaces/miners.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/interfaces/models.py` & `open_metric_learning-2.1.8/oml/interfaces/models.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/interfaces/retrieval.py` & `open_metric_learning-2.1.8/oml/interfaces/retrieval.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/interfaces/samplers.py` & `open_metric_learning-2.1.8/oml/interfaces/samplers.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/lightning/callbacks/metric.py` & `open_metric_learning-2.1.8/oml/lightning/callbacks/metric.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/lightning/modules/ddp.py` & `open_metric_learning-2.1.8/oml/lightning/modules/ddp.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/lightning/modules/extractor.py` & `open_metric_learning-2.1.8/oml/lightning/modules/extractor.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/lightning/modules/pairwise_postprocessing.py` & `open_metric_learning-2.1.8/oml/lightning/modules/pairwise_postprocessing.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/lightning/pipelines/parser.py` & `open_metric_learning-2.1.8/oml/lightning/pipelines/parser.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/lightning/pipelines/predict.py` & `open_metric_learning-2.1.8/oml/lightning/pipelines/predict.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/lightning/pipelines/train.py` & `open_metric_learning-2.1.8/oml/lightning/pipelines/train.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/lightning/pipelines/train_postprocessor.py` & `open_metric_learning-2.1.8/oml/lightning/pipelines/train_postprocessor.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/lightning/pipelines/validate.py` & `open_metric_learning-2.1.8/oml/lightning/pipelines/validate.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/losses/arcface.py` & `open_metric_learning-2.1.8/oml/losses/arcface.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/losses/surrogate_precision.py` & `open_metric_learning-2.1.8/oml/losses/surrogate_precision.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/losses/triplet.py` & `open_metric_learning-2.1.8/oml/losses/triplet.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/metrics/accumulation.py` & `open_metric_learning-2.1.8/oml/metrics/accumulation.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/metrics/embeddings.py` & `open_metric_learning-2.1.8/oml/metrics/embeddings.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/miners/cross_batch.py` & `open_metric_learning-2.1.8/oml/miners/cross_batch.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/miners/inbatch_all_tri.py` & `open_metric_learning-2.1.8/oml/miners/inbatch_all_tri.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/miners/inbatch_hard_cluster.py` & `open_metric_learning-2.1.8/oml/miners/inbatch_hard_cluster.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/miners/inbatch_hard_tri.py` & `open_metric_learning-2.1.8/oml/miners/inbatch_hard_tri.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/miners/inbatch_nhard_tri.py` & `open_metric_learning-2.1.8/oml/miners/inbatch_nhard_tri.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/miners/miner_with_bank.py` & `open_metric_learning-2.1.8/oml/miners/miner_with_bank.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/miners/pairs.py` & `open_metric_learning-2.1.8/oml/miners/pairs.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/models/meta/projection.py` & `open_metric_learning-2.1.8/oml/models/meta/projection.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/models/meta/siamese.py` & `open_metric_learning-2.1.8/oml/models/meta/siamese.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/models/resnet/extractor.py` & `open_metric_learning-2.1.8/oml/models/resnet/extractor.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/models/resnet/pooling.py` & `open_metric_learning-2.1.8/oml/models/resnet/pooling.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/models/utils.py` & `open_metric_learning-2.1.8/oml/models/utils.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/models/vit_clip/external/model.py` & `open_metric_learning-2.1.8/oml/models/vit_clip/external/model.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/models/vit_clip/extractor.py` & `open_metric_learning-2.1.8/oml/models/vit_clip/extractor.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/models/vit_dino/external/hubconf.py` & `open_metric_learning-2.1.8/oml/models/vit_dino/external/hubconf.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/models/vit_dino/external/vision_transformer.py` & `open_metric_learning-2.1.8/oml/models/vit_dino/external/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/models/vit_dino/external_v2/config.py` & `open_metric_learning-2.1.8/oml/models/vit_dino/external_v2/config.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/models/vit_dino/external_v2/hubconf.py` & `open_metric_learning-2.1.8/oml/models/vit_dino/external_v2/hubconf.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/models/vit_dino/external_v2/vision_transformer.py` & `open_metric_learning-2.1.8/oml/models/vit_dino/external_v2/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/models/vit_dino/extractor.py` & `open_metric_learning-2.1.8/oml/models/vit_dino/extractor.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/models/vit_unicom/external/model.py` & `open_metric_learning-2.1.8/oml/models/vit_unicom/external/model.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/models/vit_unicom/external/vision_transformer.py` & `open_metric_learning-2.1.8/oml/models/vit_unicom/external/vision_transformer.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/models/vit_unicom/extractor.py` & `open_metric_learning-2.1.8/oml/models/vit_unicom/extractor.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/registry/__init__.py` & `open_metric_learning-2.1.8/oml/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/registry/loggers.py` & `open_metric_learning-2.1.8/oml/registry/loggers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import os
 from typing import Any, Dict
 
 from oml.const import TCfg
 from oml.interfaces.loggers import IPipelineLogger
 from oml.lightning.pipelines.logging import (
+    ClearMLPipelineLogger,
     MLFlowPipelineLogger,
     NeptunePipelineLogger,
     TensorBoardPipelineLogger,
     WandBPipelineLogger,
 )
 from oml.utils.misc import dictconfig_to_dict
 
 LOGGERS_REGISTRY = {
     "wandb": WandBPipelineLogger,
     "neptune": NeptunePipelineLogger,
     "tensorboard": TensorBoardPipelineLogger,
     "mlflow": MLFlowPipelineLogger,
+    "clearml": ClearMLPipelineLogger,
 }
 
 CLOUD_TOKEN_NAMES = {"wandb": "WANDB_API_KEY", "neptune": "NEPTUNE_API_TOKEN"}
 TOKEN_ERROR_MESSAGE = (
     "{} logger is specified in your config file, "
     "but <{}> is not provided as a global environment variable."
     "Please, execute `export {}=your_token` before running the script."
```

### Comparing `open-metric-learning-2.1.7/oml/registry/losses.py` & `open_metric_learning-2.1.8/oml/registry/losses.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/registry/miners.py` & `open_metric_learning-2.1.8/oml/registry/miners.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/registry/models.py` & `open_metric_learning-2.1.8/oml/registry/models.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/registry/optimizers.py` & `open_metric_learning-2.1.8/oml/registry/optimizers.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/registry/postprocessors.py` & `open_metric_learning-2.1.8/oml/registry/postprocessors.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/registry/samplers.py` & `open_metric_learning-2.1.8/oml/registry/samplers.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/registry/schedulers.py` & `open_metric_learning-2.1.8/oml/registry/schedulers.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/registry/transforms.py` & `open_metric_learning-2.1.8/oml/registry/transforms.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/retrieval/postprocessors/pairwise.py` & `open_metric_learning-2.1.8/oml/retrieval/postprocessors/pairwise.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/samplers/balance.py` & `open_metric_learning-2.1.8/oml/samplers/balance.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/samplers/category_balance.py` & `open_metric_learning-2.1.8/oml/samplers/category_balance.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/samplers/distinct_category_balance.py` & `open_metric_learning-2.1.8/oml/samplers/distinct_category_balance.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/transforms/images/albumentations.py` & `open_metric_learning-2.1.8/oml/transforms/images/albumentations.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/transforms/images/torchvision.py` & `open_metric_learning-2.1.8/oml/transforms/images/torchvision.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/utils/dataframe_format.py` & `open_metric_learning-2.1.8/oml/utils/dataframe_format.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/utils/download_mock_dataset.py` & `open_metric_learning-2.1.8/oml/utils/download_mock_dataset.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/utils/images/images.py` & `open_metric_learning-2.1.8/oml/utils/images/images.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/utils/images/images_resize.py` & `open_metric_learning-2.1.8/oml/utils/images/images_resize.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/utils/io.py` & `open_metric_learning-2.1.8/oml/utils/io.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/utils/misc.py` & `open_metric_learning-2.1.8/oml/utils/misc.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/utils/misc_torch.py` & `open_metric_learning-2.1.8/oml/utils/misc_torch.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/oml/utils/remote_storage.py` & `open_metric_learning-2.1.8/oml/utils/remote_storage.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/open_metric_learning.egg-info/PKG-INFO` & `open_metric_learning-2.1.8/open_metric_learning.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-metric-learning
-Version: 2.1.7
+Version: 2.1.8
 Summary: OML is a PyTorch-based framework to train and validate the models producing high-quality embeddings.
 Home-page: https://github.com/OML-Team/open-metric-learning
 Author: Shabanov Aleksei
 Author-email: shabanoff.aleksei@gmail.com
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/OML-Team/open-metric-learning
 Project-URL: Bug Tracker, https://github.com/OML-Team/open-metric-learning/issues
@@ -58,15 +58,16 @@
 
 <div align="center">
 <a href="https://docs.neptune.ai/integrations/community_developed/" target="_blank"><img src="https://security.neptune.ai/api/share/b707f1e8-e287-4f01-b590-39a6fa7e9faa/logo.png" width="100"/></a>ㅤㅤ
 <a href="https://www.newyorker.de/" target="_blank"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d8/New_Yorker.svg/1280px-New_Yorker.svg.png" width="100"/></a>ㅤㅤ
 <a href="https://www.epoch8.co/" target="_blank"><img src="https://i.ibb.co/GdNVTyt/Screenshot-2023-07-04-at-11-19-24.png" width="100"/></a>ㅤㅤ
 <a href="https://www.meituan.com" target="_blank"><img src="https://upload.wikimedia.org/wikipedia/commons/6/61/Meituan_English_Logo.png" width="100"/></a>ㅤㅤ
 <a href="https://constructor.io/" target="_blank"><img src="https://rethink.industries/wp-content/uploads/2022/04/constructor.io-logo.png" width="100"/></a>ㅤㅤ
-<a href="https://edgify.ai/" target="_blank"><img src="https://edgify.ai/wp-content/themes/edgifyai/dist/assets/logo.svg" width="100" height="30"/></a>
+<a href="https://edgify.ai/" target="_blank"><img src="https://edgify.ai/wp-content/themes/edgifyai/dist/assets/logo.svg" width="100" height="30"/></a>ㅤㅤ
+<a href="https://inspector-cloud.ru/" target="_blank"><img src="https://thumb.tildacdn.com/tild6533-6433-4137-a266-613963373637/-/resize/540x/-/format/webp/photo.png" width="100" height="30"/></a>
 
 
 <a href="https://www.ox.ac.uk/" target="_blank"><img src="https://i.ibb.co/zhWL6tD/21-05-2019-16-08-10-6922268.png" width="120"/></a>ㅤㅤ
 <a href="https://www.hse.ru/en/" target="_blank"><img src="https://www.hse.ru/data/2020/11/16/1367274044/HSE_University_blue.jpg.(230x86x123).jpg" width="100"/></a>
 
 There is a number of people from
 [Oxford](https://www.ox.ac.uk/) and
@@ -429,15 +430,21 @@
 from oml.lightning.callbacks.metric import MetricValCallback
 from oml.losses.triplet import TripletLossWithMiner
 from oml.metrics.embeddings import EmbeddingMetrics
 from oml.miners.inbatch_all_tri import AllTripletsMiner
 from oml.models import ViTExtractor
 from oml.samplers.balance import BalanceSampler
 from oml.utils.download_mock_dataset import download_mock_dataset
-from oml.lightning.pipelines.logging import NeptunePipelineLogger, TensorBoardPipelineLogger, WandBPipelineLogger, MLFlowPipelineLogger
+from oml.lightning.pipelines.logging import (
+    ClearMLPipelineLogger,
+    MLFlowPipelineLogger,
+    NeptunePipelineLogger,
+    TensorBoardPipelineLogger,
+    WandBPipelineLogger,
+)
 
 dataset_root = "mock_dataset/"
 df_train, df_val = download_mock_dataset(dataset_root)
 
 # model
 extractor = ViTExtractor("vits16_dino", arch="vits16", normalise_features=False)
 
@@ -463,14 +470,17 @@
 # import os
 # os.environ["WANDB_API_KEY"] = ""
 # logger = WandBPipelineLogger(project="test_project", log_model=False)
 
 # 4) Logging with MLFlow locally
 # logger = MLFlowPipelineLogger(experiment_name="exp", tracking_uri="file:./ml-runs")
 
+# 5) Logging with ClearML
+# logger = ClearMLPipelineLogger(project_name="exp", task_name="test")
+
 # run
 pl_model = ExtractorModule(extractor, criterion, optimizer)
 trainer = pl.Trainer(max_epochs=3, callbacks=[metric_callback], num_sanity_val_steps=0, logger=logger)
 trainer.fit(pl_model, train_dataloaders=train_loader, val_dataloaders=val_loader)
 
 ```
 [comment]:lightning-end
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: open-metric-learning Version: 2.1.7 Summary: OML is
+Metadata-Version: 2.1 Name: open-metric-learning Version: 2.1.8 Summary: OML is
 a PyTorch-based framework to train and validate the models producing high-
 quality embeddings. Home-page: https://github.com/OML-Team/open-metric-learning
 Author: Shabanov Aleksei Author-email: shabanoff.aleksei@gmail.com License:
 Apache License 2.0 Project-URL: Homepage, https://github.com/OML-Team/open-
 metric-learning Project-URL: Bug Tracker, https://github.com/OML-Team/open-
 metric-learning/issues Keywords: data-science,computer-vision,deep-
 learning,pytorch,metric-learning,representation-learning,pytorch-lightning
@@ -42,22 +42,24 @@
                                 ### Trusted by
  _[_h_t_t_p_s_:_/_/_s_e_c_u_r_i_t_y_._n_e_p_t_u_n_e_._a_i_/_a_p_i_/_s_h_a_r_e_/_b_7_0_7_f_1_e_8_-_e_2_8_7_-_4_f_0_1_-_b_5_9_0_-_3_9_a_6_f_a_7_e_9_f_a_a_/
   _l_o_g_o_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/_u_p_l_o_a_d_._w_i_k_i_m_e_d_i_a_._o_r_g_/_w_i_k_i_p_e_d_i_a_/_c_o_m_m_o_n_s_/_t_h_u_m_b_/_d_/_d_8_/
   _N_e_w___Y_o_r_k_e_r_._s_v_g_/_1_2_8_0_p_x_-_N_e_w___Y_o_r_k_e_r_._s_v_g_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/_i_._i_b_b_._c_o_/_G_d_N_V_T_y_t_/
   _S_c_r_e_e_n_s_h_o_t_-_2_0_2_3_-_0_7_-_0_4_-_a_t_-_1_1_-_1_9_-_2_4_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/_u_p_l_o_a_d_._w_i_k_i_m_e_d_i_a_._o_r_g_/
        _w_i_k_i_p_e_d_i_a_/_c_o_m_m_o_n_s_/_6_/_6_1_/_M_e_i_t_u_a_n___E_n_g_l_i_s_h___L_o_g_o_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/
  _r_e_t_h_i_n_k_._i_n_d_u_s_t_r_i_e_s_/_w_p_-_c_o_n_t_e_n_t_/_u_p_l_o_a_d_s_/_2_0_2_2_/_0_4_/_c_o_n_s_t_r_u_c_t_o_r_._i_o_-_l_o_g_o_._p_n_g_]ã¤ã¤
- _[_h_t_t_p_s_:_/_/_e_d_g_i_f_y_._a_i_/_w_p_-_c_o_n_t_e_n_t_/_t_h_e_m_e_s_/_e_d_g_i_f_y_a_i_/_d_i_s_t_/_a_s_s_e_t_s_/_l_o_g_o_._s_v_g_]_[_h_t_t_p_s_:_/_/
- _i_._i_b_b_._c_o_/_z_h_W_L_6_t_D_/_2_1_-_0_5_-_2_0_1_9_-_1_6_-_0_8_-_1_0_-_6_9_2_2_2_6_8_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/_w_w_w_._h_s_e_._r_u_/
-_d_a_t_a_/_2_0_2_0_/_1_1_/_1_6_/_1_3_6_7_2_7_4_0_4_4_/_H_S_E___U_n_i_v_e_r_s_i_t_y___b_l_u_e_._j_p_g_._(_2_3_0_x_8_6_x_1_2_3_)_._j_p_g_]There is a
-   number of people from [Oxford](https://www.ox.ac.uk/) and [HSE](https://
-www.hse.ru/en/) universities who have used OML in their theses. [[1]](https://
- github.com/nilomr/open-metric-learning/tree/great-tit/great-tit-train) [[2]]
- (https://github.com/nastygorodi/PROJECT-Deep_Metric_Learning) [[3]](https://
-              github.com/nik-fedorov/term_paper_metric_learning)
+  _[_h_t_t_p_s_:_/_/_e_d_g_i_f_y_._a_i_/_w_p_-_c_o_n_t_e_n_t_/_t_h_e_m_e_s_/_e_d_g_i_f_y_a_i_/_d_i_s_t_/_a_s_s_e_t_s_/_l_o_g_o_._s_v_g_]ã¤ã¤
+_[_h_t_t_p_s_:_/_/_t_h_u_m_b_._t_i_l_d_a_c_d_n_._c_o_m_/_t_i_l_d_6_5_3_3_-_6_4_3_3_-_4_1_3_7_-_a_2_6_6_-_6_1_3_9_6_3_3_7_3_6_3_7_/_-_/_r_e_s_i_z_e_/_5_4_0_x_/
+    _-_/_f_o_r_m_a_t_/_w_e_b_p_/_p_h_o_t_o_._p_n_g_]_[_h_t_t_p_s_:_/_/_i_._i_b_b_._c_o_/_z_h_W_L_6_t_D_/_2_1_-_0_5_-_2_0_1_9_-_1_6_-_0_8_-_1_0_-
+      _6_9_2_2_2_6_8_._p_n_g_]ã¤ã¤ _[_h_t_t_p_s_:_/_/_w_w_w_._h_s_e_._r_u_/_d_a_t_a_/_2_0_2_0_/_1_1_/_1_6_/_1_3_6_7_2_7_4_0_4_4_/
+  _H_S_E___U_n_i_v_e_r_s_i_t_y___b_l_u_e_._j_p_g_._(_2_3_0_x_8_6_x_1_2_3_)_._j_p_g_]There is a number of people from
+[Oxford](https://www.ox.ac.uk/) and [HSE](https://www.hse.ru/en/) universities
+who have used OML in their theses. [[1]](https://github.com/nilomr/open-metric-
+learning/tree/great-tit/great-tit-train) [[2]](https://github.com/nastygorodi/
+      PROJECT-Deep_Metric_Learning) [[3]](https://github.com/nik-fedorov/
+                          term_paper_metric_learning)
 ## [FAQ](https://open-metric-learning.readthedocs.io/en/latest/oml/faq.html)
 Why do I need OML?
 You may think *"If I need image embeddings I can simply train a vanilla
 classifier and take its penultimate layer"*. Well, it makes sense as a starting
 point. But there are several possible drawbacks: * If you want to use
 embeddings to perform searching you need to calculate some distance among them
 (for example, cosine or L2). Usually, **you don't directly optimize these
@@ -266,36 +268,38 @@
 from oml.datasets.base import DatasetQueryGallery, DatasetWithLabels from
 oml.lightning.modules.extractor import ExtractorModule from
 oml.lightning.callbacks.metric import MetricValCallback from oml.losses.triplet
 import TripletLossWithMiner from oml.metrics.embeddings import EmbeddingMetrics
 from oml.miners.inbatch_all_tri import AllTripletsMiner from oml.models import
 ViTExtractor from oml.samplers.balance import BalanceSampler from
 oml.utils.download_mock_dataset import download_mock_dataset from
-oml.lightning.pipelines.logging import NeptunePipelineLogger,
-TensorBoardPipelineLogger, WandBPipelineLogger, MLFlowPipelineLogger
-dataset_root = "mock_dataset/" df_train, df_val = download_mock_dataset
-(dataset_root) # model extractor = ViTExtractor("vits16_dino", arch="vits16",
-normalise_features=False) # train optimizer = torch.optim.SGD
-(extractor.parameters(), lr=1e-6) train_dataset = DatasetWithLabels(df_train,
-dataset_root=dataset_root) criterion = TripletLossWithMiner(margin=0.1,
-miner=AllTripletsMiner()) batch_sampler = BalanceSampler
-(train_dataset.get_labels(), n_labels=2, n_instances=3) train_loader =
-torch.utils.data.DataLoader(train_dataset, batch_sampler=batch_sampler) # val
-val_dataset = DatasetQueryGallery(df_val, dataset_root=dataset_root) val_loader
-= torch.utils.data.DataLoader(val_dataset, batch_size=4) metric_callback =
-MetricValCallback(metric=EmbeddingMetrics(extra_keys=
-[train_dataset.paths_key,]), log_images=True) # 1) Logging with Tensorboard
-logger = TensorBoardPipelineLogger(".") # 2) Logging with Neptune # logger =
+oml.lightning.pipelines.logging import ( ClearMLPipelineLogger,
+MLFlowPipelineLogger, NeptunePipelineLogger, TensorBoardPipelineLogger,
+WandBPipelineLogger, ) dataset_root = "mock_dataset/" df_train, df_val =
+download_mock_dataset(dataset_root) # model extractor = ViTExtractor
+("vits16_dino", arch="vits16", normalise_features=False) # train optimizer =
+torch.optim.SGD(extractor.parameters(), lr=1e-6) train_dataset =
+DatasetWithLabels(df_train, dataset_root=dataset_root) criterion =
+TripletLossWithMiner(margin=0.1, miner=AllTripletsMiner()) batch_sampler =
+BalanceSampler(train_dataset.get_labels(), n_labels=2, n_instances=3)
+train_loader = torch.utils.data.DataLoader(train_dataset,
+batch_sampler=batch_sampler) # val val_dataset = DatasetQueryGallery(df_val,
+dataset_root=dataset_root) val_loader = torch.utils.data.DataLoader
+(val_dataset, batch_size=4) metric_callback = MetricValCallback
+(metric=EmbeddingMetrics(extra_keys=[train_dataset.paths_key,]),
+log_images=True) # 1) Logging with Tensorboard logger =
+TensorBoardPipelineLogger(".") # 2) Logging with Neptune # logger =
 NeptunePipelineLogger(api_key="", project="", log_model_checkpoints=False) # 3)
 Logging with Weights and Biases # import os # os.environ["WANDB_API_KEY"] = ""
 # logger = WandBPipelineLogger(project="test_project", log_model=False) # 4)
 Logging with MLFlow locally # logger = MLFlowPipelineLogger
-(experiment_name="exp", tracking_uri="file:./ml-runs") # run pl_model =
-ExtractorModule(extractor, criterion, optimizer) trainer = pl.Trainer
-(max_epochs=3, callbacks=[metric_callback], num_sanity_val_steps=0,
+(experiment_name="exp", tracking_uri="file:./ml-runs") # 5) Logging with
+ClearML # logger = ClearMLPipelineLogger(project_name="exp", task_name="test")
+# run pl_model = ExtractorModule(extractor, criterion, optimizer) trainer =
+pl.Trainer(max_epochs=3, callbacks=[metric_callback], num_sanity_val_steps=0,
 logger=logger) trainer.fit(pl_model, train_dataloaders=train_loader,
 val_dataloaders=val_loader) ``` [comment]:lightning-end
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/drive/
 1bVUgdBGWvQgCkba2YtaIRVlUQUz7Q60Z?usp=share_link) Using a trained model for
 retrieval
 [comment]:usage-retrieval-start ```python import torch from oml.const import
```

### Comparing `open-metric-learning-2.1.7/open_metric_learning.egg-info/SOURCES.txt` & `open_metric_learning-2.1.8/open_metric_learning.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 oml/configs/criterion/triplet_plain.yaml
 oml/configs/criterion/triplet_with_miner.yaml
 oml/configs/extractor/extractor_with_mlp.yaml
 oml/configs/extractor/resnet.yaml
 oml/configs/extractor/vit.yaml
 oml/configs/extractor/vit_clip.yaml
 oml/configs/extractor/vit_unicom.yaml
+oml/configs/logger/clearml.yaml
 oml/configs/logger/mlflow.yaml
 oml/configs/logger/neptune.yaml
 oml/configs/logger/tensorboard.yaml
 oml/configs/logger/wandb.yaml
 oml/configs/miner/all_triplets.yaml
 oml/configs/miner/hard_cluster.yaml
 oml/configs/miner/hard_triplets.yaml
@@ -64,15 +65,14 @@
 oml/configs/transforms/norm_resize_torch.yaml
 oml/configs/transforms/norm_torch.yaml
 oml/configs/transforms/unicom_transforms.yaml
 oml/datasets/__init__.py
 oml/datasets/base.py
 oml/datasets/list_dataset.py
 oml/datasets/pairs.py
-oml/datasets/triplet.py
 oml/ddp/__init__.py
 oml/ddp/patching.py
 oml/ddp/utils.py
 oml/functional/__init__.py
 oml/functional/label_smoothing.py
 oml/functional/losses.py
 oml/functional/metrics.py
@@ -106,15 +106,14 @@
 oml/losses/__init__.py
 oml/losses/arcface.py
 oml/losses/surrogate_precision.py
 oml/losses/triplet.py
 oml/metrics/__init__.py
 oml/metrics/accumulation.py
 oml/metrics/embeddings.py
-oml/metrics/triplets.py
 oml/miners/__init__.py
 oml/miners/cross_batch.py
 oml/miners/inbatch_all_tri.py
 oml/miners/inbatch_hard_cluster.py
 oml/miners/inbatch_hard_tri.py
 oml/miners/inbatch_nhard_tri.py
 oml/miners/miner_with_bank.py
```

### Comparing `open-metric-learning-2.1.7/setup.py` & `open_metric_learning-2.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/tests/test_build_readme.py` & `open_metric_learning-2.1.8/tests/test_build_readme.py`

 * *Files identical despite different names*

### Comparing `open-metric-learning-2.1.7/tests/test_imports.py` & `open_metric_learning-2.1.8/tests/test_imports.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 from typing import List, Tuple
 
 import pytest
 
 from oml.const import PROJECT_ROOT
 
-LIBS_TO_IGNORE = ["torch_xla", "pytorch_grad_cam", "wandb", "neptune", "IPython"]
+LIBS_TO_IGNORE = ["torch_xla", "pytorch_grad_cam", "wandb", "neptune", "clearml", "IPython"]
 
 NEED_TO_TEST_NOTEBOOKS = True
 
 
 def get_imports_from_files() -> List[Tuple[str, str]]:
     files = get_files_with_imports()
```

### Comparing `open-metric-learning-2.1.7/tests/test_outdated_docs.py` & `open_metric_learning-2.1.8/tests/test_outdated_docs.py`

 * *Files identical despite different names*

