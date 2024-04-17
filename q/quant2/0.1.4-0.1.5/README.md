# Comparing `tmp/quant2-0.1.4.tar.gz` & `tmp/quant2-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quant2-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "quant2-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `quant2-0.1.4.tar` & `quant2-0.1.5.tar`

### file list

```diff
@@ -1,53 +1,54 @@
--rw-r--r--   0        0        0      574 2024-04-06 14:41:03.615629 quant2-0.1.4/.gitignore
--rw-r--r--   0        0        0    11357 2024-03-20 11:12:02.832412 quant2-0.1.4/LICENSE
--rw-r--r--   0        0        0        7 2024-03-20 11:12:02.832412 quant2-0.1.4/README.md
--rw-r--r--   0        0        0      971 2024-04-14 08:14:34.409434 quant2-0.1.4/configs/stnetv3/stnetv3_table20240326_2201to2312.cfg
--rw-r--r--   0        0        0     1049 2024-04-12 08:57:23.226862 quant2-0.1.4/configs/stnetv4/stnetv4_table20240410_2201to2312.cfg
--rw-r--r--   0        0        0      664 2024-04-10 00:12:18.347578 quant2-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1841 2024-03-23 05:01:23.359992 quant2-0.1.4/quant/README.md
--rw-r--r--   0        0        0      559 2024-04-16 02:25:09.504593 quant2-0.1.4/quant/__init__.py
--rw-r--r--   0        0        0       67 2024-03-23 04:17:48.269987 quant2-0.1.4/quant/__main__.py
--rw-r--r--   0        0        0        0 2024-04-08 01:35:10.284089 quant2-0.1.4/quant/evaluate/__init__.py
--rw-r--r--   0        0        0     2646 2024-04-12 06:45:48.719809 quant2-0.1.4/quant/evaluate/table20240326.py
--rw-r--r--   0        0        0     2006 2024-04-12 04:48:31.980573 quant2-0.1.4/quant/evaluate/utils.py
--rw-r--r--   0        0        0      422 2024-03-23 04:21:50.819993 quant2-0.1.4/quant/football/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 14:09:03.305285 quant2-0.1.4/quant/football/data/__init__.py
--rw-r--r--   0        0        0     4348 2024-04-14 08:11:01.537268 quant2-0.1.4/quant/football/data/dataset.py
--rw-r--r--   0        0        0        0 2024-04-08 10:24:35.916611 quant2-0.1.4/quant/football/data/functional.py
--rw-r--r--   0        0        0     1336 2024-04-15 11:24:33.080117 quant2-0.1.4/quant/football/data/preprocessing.py
--rw-r--r--   0        0        0        0 2024-04-08 11:08:36.928001 quant2-0.1.4/quant/football/data/stats.py
--rw-r--r--   0        0        0     4560 2024-04-13 08:19:58.059662 quant2-0.1.4/quant/football/data/utils.py
--rw-r--r--   0        0        0        0 2024-04-11 16:55:37.649284 quant2-0.1.4/quant/football/infer/__init__.py
--rw-r--r--   0        0        0     2024 2024-04-16 01:19:44.599739 quant2-0.1.4/quant/football/infer/fastapi_app.py
--rw-r--r--   0        0        0      468 2024-04-11 16:55:50.160241 quant2-0.1.4/quant/football/infer/fastapi_app_test.py
--rw-r--r--   0        0        0     8033 2024-04-16 02:00:09.037054 quant2-0.1.4/quant/football/infer/football_infer_overunder_v1.py
--rw-r--r--   0        0        0      473 2024-04-11 16:56:07.430215 quant2-0.1.4/quant/football/models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 04:22:28.629548 quant2-0.1.4/quant/football/models/mtnet.py
--rw-r--r--   0        0        0     6110 2024-04-11 17:12:37.365849 quant2-0.1.4/quant/football/models/stnet.py
--rw-r--r--   0        0        0      463 2024-04-15 20:54:36.028514 quant2-0.1.4/quant/football/transforms/__init__.py
--rw-r--r--   0        0        0     6622 2024-04-16 00:40:54.525920 quant2-0.1.4/quant/football/transforms/table20240326.py
--rw-r--r--   0        0        0     8541 2024-04-16 01:19:10.126956 quant2-0.1.4/quant/football/transforms/table20240410.py
--rw-r--r--   0        0        0     8825 2024-04-16 00:40:14.674251 quant2-0.1.4/quant/football/transforms/table20240414.py
--rw-r--r--   0        0        0     8396 2024-04-16 02:25:15.544645 quant2-0.1.4/quant/football/transforms/table20240415.py
--rw-r--r--   0        0        0        0 2024-03-31 10:26:04.538951 quant2-0.1.4/quant/layers/__init__.py
--rw-r--r--   0        0        0      483 2024-03-28 09:12:19.609652 quant2-0.1.4/quant/layers/layer_scale.py
--rw-r--r--   0        0        0     1070 2024-03-28 09:13:06.741829 quant2-0.1.4/quant/layers/mlp.py
--rw-r--r--   0        0        0     1314 2024-03-28 09:40:33.643889 quant2-0.1.4/quant/layers/normalization.py
--rw-r--r--   0        0        0      852 2024-03-28 09:16:09.540017 quant2-0.1.4/quant/layers/swiglu_ffn.py
--rw-r--r--   0        0        0        0 2024-04-03 13:03:10.745509 quant2-0.1.4/quant/utils/__init__.py
--rw-r--r--   0        0        0     1695 2024-04-11 16:56:25.721657 quant2-0.1.4/quant/utils/archive.py
--rw-r--r--   0        0        0     1884 2024-04-14 08:14:07.935771 quant2-0.1.4/quant/utils/config.py
--rw-r--r--   0        0        0     1047 2024-04-09 01:40:57.919653 quant2-0.1.4/quant/utils/io.py
--rw-r--r--   0        0        0     1006 2024-04-03 13:19:59.255567 quant2-0.1.4/quant/utils/logging.py
--rw-r--r--   0        0        0      182 2024-03-28 01:09:02.081511 quant2-0.1.4/tests/football/data/test_utils.py
--rw-r--r--   0        0        0     1632 2024-04-12 06:45:57.389803 quant2-0.1.4/tools/analysis_tools/analyze_cls_results.py
--rw-r--r--   0        0        0     2645 2024-04-16 01:48:23.763355 quant2-0.1.4/tools/experimental/make_dataset.py
--rw-r--r--   0        0        0     1580 2024-04-13 14:41:36.176420 quant2-0.1.4/tools/experimental/make_split.py
--rw-r--r--   0        0        0     6485 2024-04-15 11:07:06.081414 quant2-0.1.4/tools/experimental/nni_football.py
--rw-r--r--   0        0        0      476 2024-04-15 19:50:59.765841 quant2-0.1.4/tools/experimental/nni_football_config.yaml
--rw-r--r--   0        0        0     1556 2024-04-15 20:08:48.206604 quant2-0.1.4/tools/experimental/nni_football_config_search_space.json
--rw-r--r--   0        0        0      523 2024-04-14 02:37:47.884925 quant2-0.1.4/tools/experimental/nni_model.py
--rw-r--r--   0        0        0      441 2024-04-14 04:00:22.459245 quant2-0.1.4/tools/experimental/nni_model_config.yaml
--rw-r--r--   0        0        0     2855 2024-04-15 11:07:14.941468 quant2-0.1.4/tools/fb_cls_test.py
--rw-r--r--   0        0        0     6353 2024-04-15 11:07:20.811492 quant2-0.1.4/tools/fb_cls_train.py
--rw-r--r--   0        0        0     2187 1970-01-01 00:00:00.000000 quant2-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      574 2024-04-06 14:41:03.615629 quant2-0.1.5/.gitignore
+-rw-r--r--   0        0        0    11357 2024-03-20 11:12:02.832412 quant2-0.1.5/LICENSE
+-rw-r--r--   0        0        0        7 2024-03-20 11:12:02.832412 quant2-0.1.5/README.md
+-rw-r--r--   0        0        0      971 2024-04-14 08:14:34.409434 quant2-0.1.5/configs/stnetv3/stnetv3_table20240326_2201to2312.cfg
+-rw-r--r--   0        0        0     1049 2024-04-12 08:57:23.226862 quant2-0.1.5/configs/stnetv4/stnetv4_table20240410_2201to2312.cfg
+-rw-r--r--   0        0        0      664 2024-04-10 00:12:18.347578 quant2-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1841 2024-03-23 05:01:23.359992 quant2-0.1.5/quant/README.md
+-rw-r--r--   0        0        0      559 2024-04-17 08:12:03.953448 quant2-0.1.5/quant/__init__.py
+-rw-r--r--   0        0        0       67 2024-03-23 04:17:48.269987 quant2-0.1.5/quant/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-08 01:35:10.284089 quant2-0.1.5/quant/evaluate/__init__.py
+-rw-r--r--   0        0        0     2646 2024-04-12 06:45:48.719809 quant2-0.1.5/quant/evaluate/table20240326.py
+-rw-r--r--   0        0        0     2006 2024-04-12 04:48:31.980573 quant2-0.1.5/quant/evaluate/utils.py
+-rw-r--r--   0        0        0      422 2024-03-23 04:21:50.819993 quant2-0.1.5/quant/football/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 14:09:03.305285 quant2-0.1.5/quant/football/data/__init__.py
+-rw-r--r--   0        0        0     4348 2024-04-14 08:11:01.537268 quant2-0.1.5/quant/football/data/dataset.py
+-rw-r--r--   0        0        0        0 2024-04-08 10:24:35.916611 quant2-0.1.5/quant/football/data/functional.py
+-rw-r--r--   0        0        0     1336 2024-04-15 11:24:33.080117 quant2-0.1.5/quant/football/data/preprocessing.py
+-rw-r--r--   0        0        0      993 2024-04-17 06:41:14.170874 quant2-0.1.5/quant/football/data/sampler.py
+-rw-r--r--   0        0        0        0 2024-04-08 11:08:36.928001 quant2-0.1.5/quant/football/data/stats.py
+-rw-r--r--   0        0        0     4560 2024-04-13 08:19:58.059662 quant2-0.1.5/quant/football/data/utils.py
+-rw-r--r--   0        0        0        0 2024-04-11 16:55:37.649284 quant2-0.1.5/quant/football/infer/__init__.py
+-rw-r--r--   0        0        0     2024 2024-04-16 01:19:44.599739 quant2-0.1.5/quant/football/infer/fastapi_app.py
+-rw-r--r--   0        0        0      468 2024-04-11 16:55:50.160241 quant2-0.1.5/quant/football/infer/fastapi_app_test.py
+-rw-r--r--   0        0        0     8033 2024-04-16 02:00:09.037054 quant2-0.1.5/quant/football/infer/football_infer_overunder_v1.py
+-rw-r--r--   0        0        0      473 2024-04-11 16:56:07.430215 quant2-0.1.5/quant/football/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 04:22:28.629548 quant2-0.1.5/quant/football/models/mtnet.py
+-rw-r--r--   0        0        0     6110 2024-04-11 17:12:37.365849 quant2-0.1.5/quant/football/models/stnet.py
+-rw-r--r--   0        0        0      463 2024-04-15 20:54:36.028514 quant2-0.1.5/quant/football/transforms/__init__.py
+-rw-r--r--   0        0        0     6622 2024-04-16 00:40:54.525920 quant2-0.1.5/quant/football/transforms/table20240326.py
+-rw-r--r--   0        0        0     8541 2024-04-16 01:19:10.126956 quant2-0.1.5/quant/football/transforms/table20240410.py
+-rw-r--r--   0        0        0     8825 2024-04-16 00:40:14.674251 quant2-0.1.5/quant/football/transforms/table20240414.py
+-rw-r--r--   0        0        0     8396 2024-04-16 02:25:15.544645 quant2-0.1.5/quant/football/transforms/table20240415.py
+-rw-r--r--   0        0        0        0 2024-03-31 10:26:04.538951 quant2-0.1.5/quant/layers/__init__.py
+-rw-r--r--   0        0        0      483 2024-03-28 09:12:19.609652 quant2-0.1.5/quant/layers/layer_scale.py
+-rw-r--r--   0        0        0     1070 2024-03-28 09:13:06.741829 quant2-0.1.5/quant/layers/mlp.py
+-rw-r--r--   0        0        0     1314 2024-03-28 09:40:33.643889 quant2-0.1.5/quant/layers/normalization.py
+-rw-r--r--   0        0        0      852 2024-03-28 09:16:09.540017 quant2-0.1.5/quant/layers/swiglu_ffn.py
+-rw-r--r--   0        0        0        0 2024-04-03 13:03:10.745509 quant2-0.1.5/quant/utils/__init__.py
+-rw-r--r--   0        0        0     1695 2024-04-11 16:56:25.721657 quant2-0.1.5/quant/utils/archive.py
+-rw-r--r--   0        0        0     1884 2024-04-14 08:14:07.935771 quant2-0.1.5/quant/utils/config.py
+-rw-r--r--   0        0        0     1047 2024-04-09 01:40:57.919653 quant2-0.1.5/quant/utils/io.py
+-rw-r--r--   0        0        0     1006 2024-04-03 13:19:59.255567 quant2-0.1.5/quant/utils/logging.py
+-rw-r--r--   0        0        0      182 2024-03-28 01:09:02.081511 quant2-0.1.5/tests/football/data/test_utils.py
+-rw-r--r--   0        0        0     1632 2024-04-12 06:45:57.389803 quant2-0.1.5/tools/analysis_tools/analyze_cls_results.py
+-rw-r--r--   0        0        0     2645 2024-04-16 01:48:23.763355 quant2-0.1.5/tools/experimental/make_dataset.py
+-rw-r--r--   0        0        0     1580 2024-04-13 14:41:36.176420 quant2-0.1.5/tools/experimental/make_split.py
+-rw-r--r--   0        0        0     8078 2024-04-17 06:34:03.034798 quant2-0.1.5/tools/experimental/nni_football.py
+-rw-r--r--   0        0        0      600 2024-04-17 07:13:13.694051 quant2-0.1.5/tools/experimental/nni_football_config.yaml
+-rw-r--r--   0        0        0     1832 2024-04-17 08:12:07.193491 quant2-0.1.5/tools/experimental/nni_football_config_search_space.json
+-rw-r--r--   0        0        0      523 2024-04-14 02:37:47.884925 quant2-0.1.5/tools/experimental/nni_model.py
+-rw-r--r--   0        0        0      441 2024-04-14 04:00:22.459245 quant2-0.1.5/tools/experimental/nni_model_config.yaml
+-rw-r--r--   0        0        0     2855 2024-04-15 11:07:14.941468 quant2-0.1.5/tools/fb_cls_test.py
+-rw-r--r--   0        0        0     7897 2024-04-17 06:33:07.892275 quant2-0.1.5/tools/fb_cls_train.py
+-rw-r--r--   0        0        0     2187 1970-01-01 00:00:00.000000 quant2-0.1.5/PKG-INFO
```

### Comparing `quant2-0.1.4/.gitignore` & `quant2-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `quant2-0.1.4/LICENSE` & `quant2-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `quant2-0.1.4/configs/stnetv3/stnetv3_table20240326_2201to2312.cfg` & `quant2-0.1.5/configs/stnetv3/stnetv3_table20240326_2201to2312.cfg`

 * *Files identical despite different names*

### Comparing `quant2-0.1.4/configs/stnetv4/stnetv4_table20240410_2201to2312.cfg` & `quant2-0.1.5/configs/stnetv4/stnetv4_table20240410_2201to2312.cfg`

 * *Files identical despite different names*

### Comparing `quant2-0.1.4/pyproject.toml` & `quant2-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quant2-0.1.4/quant/README.md` & `quant2-0.1.5/quant/README.md`

 * *Files identical despite different names*

### Comparing `quant2-0.1.4/quant/__init__.py` & `quant2-0.1.5/quant/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """A collection of useful tools!"""
 import sys
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
 
 help_doc_str = """\
 usage: quant [--version] [--help]
 
 shell command:
     quant -h
```

### Comparing `quant2-0.1.4/quant/evaluate/table20240326.py` & `quant2-0.1.5/quant/evaluate/table20240326.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.4/quant/evaluate/utils.py` & `quant2-0.1.5/quant/evaluate/utils.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.4/quant/football/data/dataset.py` & `quant2-0.1.5/quant/football/data/dataset.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.4/quant/football/data/preprocessing.py` & `quant2-0.1.5/quant/football/data/preprocessing.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.4/quant/football/data/utils.py` & `quant2-0.1.5/quant/football/data/utils.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.4/quant/football/infer/fastapi_app.py` & `quant2-0.1.5/quant/football/infer/fastapi_app.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.4/quant/football/infer/football_infer_overunder_v1.py` & `quant2-0.1.5/quant/football/infer/football_infer_overunder_v1.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.4/quant/football/models/stnet.py` & `quant2-0.1.5/quant/football/models/stnet.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.4/quant/football/transforms/table20240326.py` & `quant2-0.1.5/quant/football/transforms/table20240326.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.4/quant/football/transforms/table20240410.py` & `quant2-0.1.5/quant/football/transforms/table20240410.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.4/quant/football/transforms/table20240414.py` & `quant2-0.1.5/quant/football/transforms/table20240414.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.4/quant/football/transforms/table20240415.py` & `quant2-0.1.5/quant/football/transforms/table20240415.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.4/quant/layers/mlp.py` & `quant2-0.1.5/quant/layers/mlp.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.4/quant/layers/normalization.py` & `quant2-0.1.5/quant/layers/normalization.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.4/quant/layers/swiglu_ffn.py` & `quant2-0.1.5/quant/layers/swiglu_ffn.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.4/quant/utils/archive.py` & `quant2-0.1.5/quant/utils/archive.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.4/quant/utils/config.py` & `quant2-0.1.5/quant/utils/config.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.4/quant/utils/io.py` & `quant2-0.1.5/quant/utils/io.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.4/quant/utils/logging.py` & `quant2-0.1.5/quant/utils/logging.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.4/tools/analysis_tools/analyze_cls_results.py` & `quant2-0.1.5/tools/analysis_tools/analyze_cls_results.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.4/tools/experimental/make_dataset.py` & `quant2-0.1.5/tools/experimental/make_dataset.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.4/tools/experimental/make_split.py` & `quant2-0.1.5/tools/experimental/make_split.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.4/tools/experimental/nni_football.py` & `quant2-0.1.5/tools/fb_cls_train.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-import nni
+# PYTHONPATH=$(pwd) python tools/fb_cls_train.py
 import numpy as np
 import random
 import sys
 import time
 import torch
 from copy import deepcopy
 from pathlib import Path
 from quant.football.data.dataset import get_dataset
+from quant.football.data.sampler import RandomSubsetSampler
 from quant.football.models import get_model
 from quant.utils.config import get_config, merge_from_dict
 from quant.utils.io import copy_file, save_json
 from quant.utils.logging import get_logger, print_log
 
 
 def train(model, device, train_loader, loss_fn, optimizer, epoch, log_interval, verbose, logger):
@@ -52,77 +53,110 @@
     print_log(
         f"\nTest set: Avg loss: {test_loss:.6f}, Acc: {correct}/{dataset_size} ({test_acc:.4f})\n", verbose, logger)
     return test_acc
 
 
 def main(cfg, verbose=True):
     _cfg = deepcopy(cfg)
-    data, model, loss, optimizer, scheduler, runtime = \
+    data_cfg, model_cfg, loss_cfg, optimizer_cfg, scheduler_cfg, runtime_cfg = \
         cfg["data"], cfg["model"], cfg["loss"], cfg["optimizer"], cfg["scheduler"], cfg["runtime"]
 
-    seed = runtime.get("seed", 1)
-    epochs = runtime.get("epochs", 90)
-    device = runtime.get("device", "cuda")
-    log_interval = runtime.get("log_interval", 10)
+    seed = runtime_cfg.get("seed", 1)
+    epochs = runtime_cfg.get("epochs", 90)
+    device = runtime_cfg.get("device", "cuda")
+    log_interval = runtime_cfg.get("log_interval", 10)
 
     random.seed(seed)
     np.random.seed(seed)
     torch.manual_seed(seed)
-    torch.backends.cudnn.deterministic = False
-    torch.backends.cudnn.benchmark = True
+    torch.backends.cudnn.deterministic = True
+    torch.backends.cudnn.benchmark = False
 
     if device == "cuda" and torch.cuda.is_available():
         device = torch.device("cuda")
     else:
         device = torch.device("cpu")
 
-    dataset_type = data.pop("type")
-    data_root = Path(data["data_root"])
-    train_dataset = get_dataset(dataset_type, data_root / data["train_file"])
-    test_dataset = get_dataset(dataset_type, data_root / data["test_file"])
+    dataset_type = data_cfg.pop("type")
+    data_root = Path(data_cfg["data_root"])
+    train_dataset = get_dataset(dataset_type, data_root / data_cfg["train_file"])
+    test_dataset = get_dataset(dataset_type, data_root / data_cfg["test_file"])
+
+    fraction = data_cfg.get("fraction", None)
+    num_samples = data_cfg.get("num_samples", None)
+    sampler = RandomSubsetSampler(len(train_dataset), num_samples, fraction)
+
+    num_workers = data_cfg.get("num_workers", 8)
 
     train_loader = torch.utils.data.DataLoader(
-        train_dataset, batch_size=data["batch_size"], shuffle=True
+        train_dataset, batch_size=data_cfg["batch_size"], sampler=sampler, num_workers=num_workers, drop_last=True
     )
     test_loader = torch.utils.data.DataLoader(
-        test_dataset, batch_size=128
+        test_dataset, batch_size=128, num_workers=num_workers
     )
 
-    model_type = model.pop("type")
-    model = get_model(model_type, **model).to(device)
+    model_type = model_cfg.pop("type")
+    model = get_model(model_type, **model_cfg)
+
+    checkpoint = model_cfg.get("checkpoint", None)
+    if checkpoint is not None:
+        model.load_state_dict(torch.load(checkpoint, map_location=torch.device("cpu")))
+
+    # layers, layers.0, layers.0.1, norm, head.weight, head.bias
+    frozen_layers = model_cfg.get("frozen_layers", None)
+    if frozen_layers is not None:
+        for name, param in model.named_parameters():
+            param.requires_grad = True
+            for layer_name in frozen_layers:
+                if layer_name in name:
+                    param.requires_grad = False
+                    break
+
+    # season_embedding, team_embedding, stem
+    trainable_layers = model_cfg.get("trainable_layers", None)
+    if trainable_layers is not None:
+        for name, param in model.named_parameters():
+            param.requires_grad = False
+            for layer_name in trainable_layers:
+                if layer_name in name:
+                    param.requires_grad = True
+                    break
 
-    loss_type = loss.pop("type")
+    model = model.to(device)
+
+    loss_type = loss_cfg.pop("type")
     if loss_type == "CrossEntropyLoss":
         from torch.nn import CrossEntropyLoss
-        loss_fn = CrossEntropyLoss(**loss).to(device)
+        loss_fn = CrossEntropyLoss(**loss_cfg).to(device)
     else:
         raise NotImplementedError(f"Not supported <{loss_type}>.")
 
-    optimizer_type = optimizer.pop("type")
+    params = [param for param in model.parameters() if param.requires_grad]
+    optimizer_type = optimizer_cfg.pop("type")
     if optimizer_type == "SGD":
         from torch.optim import SGD
-        optimizer.setdefault("momentum", 0.9)
-        optimizer = SGD(model.parameters(), **optimizer)
+        optimizer_cfg.setdefault("momentum", 0.9)
+        optimizer = SGD(params, **optimizer_cfg)
     elif optimizer_type == "AdamW":
         from torch.optim import AdamW
-        optimizer.setdefault("betas", (0.9, 0.999))
-        if isinstance(optimizer["betas"], str):
-            optimizer["betas"] = eval(optimizer["betas"])
-        optimizer = AdamW(model.parameters(), **optimizer)
+        optimizer_cfg.setdefault("betas", (0.9, 0.999))
+        if isinstance(optimizer_cfg["betas"], str):
+            optimizer_cfg["betas"] = eval(optimizer_cfg["betas"])
+        optimizer = AdamW(params, **optimizer_cfg)
     else:
         raise NotImplementedError(f"Not supported <{optimizer_type}>.")
 
-    scheduler_type = scheduler.pop("type")
+    scheduler_type = scheduler_cfg.pop("type")
     if scheduler_type == "StepLR":
         from torch.optim.lr_scheduler import StepLR
-        scheduler = StepLR(optimizer, **scheduler)
+        scheduler = StepLR(optimizer, **scheduler_cfg)
     else:
         raise NotImplementedError(f"Not supported <{scheduler_type}>.")
 
-    trial_name = time.strftime("%Y%m%d") + f"_{nni.get_experiment_id()}_{nni.get_sequence_id():04d}"
+    trial_name = time.strftime("%Y%m%d%H%M%S")
     out_dir = Path("runs") / data_root.name / trial_name
     out_dir.mkdir(parents=True, exist_ok=True)
     copy_file(data_root, out_dir, "*.json")
 
     logger = get_logger(__name__, False, out_dir / "log.txt")
 
     best_acc, best_epoch = 0.0, -1
@@ -139,15 +173,15 @@
     last_acc_test = curr_acc
 
     print_log("[best model]", verbose, logger)
     print_log(f"\noutput dir: {out_dir}", verbose, logger)
     print_log(f"{best_acc=:.4f}, {best_epoch=:03d}\n", verbose, logger)
 
     print_log("[check train dataset]", verbose, logger)
-    check_loader = torch.utils.data.DataLoader(train_dataset, batch_size=128)
+    check_loader = torch.utils.data.DataLoader(train_dataset, batch_size=128, num_workers=num_workers)
     last_acc_train = test(model, device, check_loader, loss_fn,
                           verbose, logger)
 
     _cfg["log"] = {
         "out_dir": str(out_dir),
         "date": time.strftime("%Y-%m-%d %H:%M:%S"),
         "best_acc": best_acc,
@@ -165,12 +199,9 @@
     for arg in sys.argv[1:]:
         key, val = arg.split("=", maxsplit=1)
         options[key] = eval(val)
 
     cfg = get_config(options.get("config", None))
     cfg = merge_from_dict(cfg, options)
 
-    optimized_params = nni.get_next_parameter()
-    cfg = merge_from_dict(cfg, optimized_params)
-
     best_acc, _cfg = main(cfg, verbose=False)
-    nni.report_final_result({"default": best_acc, "log": _cfg["log"]})
+    print({"default": best_acc, "log": _cfg["log"]})
```

### Comparing `quant2-0.1.4/tools/experimental/nni_football_config_search_space.json` & `quant2-0.1.5/tools/experimental/nni_football_config_search_space.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7836647727272728%*

 * *Differences: {"'data.batch_size'": "{'_value': {delete: [2, 0]}}",*

 * * "'data.fraction'": "OrderedDict([('_type', 'choice'), ('_value', [0.3])])",*

 * * "'data.num_workers'": "OrderedDict([('_type', 'choice'), ('_value', [8])])",*

 * * "'model.checkpoint'": "OrderedDict([('_type', 'choice'), ('_value', [None])])",*

 * * "'model.drop'": "{'_value': {delete: [5, 3, 1]}}",*

 * * "'model.hidden_features'": "{'_value': {delete: [7, 3, 1]}}",*

 * * "'model.in_features'": "{'_value': [111]}",*

 * * "'model.team_embedding_dim'": "{'_value': {delete: [3]}}",*

 * * " […]*

```diff
@@ -1,71 +1,81 @@
 {
     "data.batch_size": {
         "_type": "choice",
         "_value": [
-            96,
             128,
-            192,
             256
         ]
     },
     "data.data_root": {
         "_type": "choice",
         "_value": [
             "/datasets/table20240415_train_2301_2312_2403_lb_5_15_label_whole_c20_maxabs_direct"
         ]
     },
+    "data.fraction": {
+        "_type": "choice",
+        "_value": [
+            0.3
+        ]
+    },
+    "data.num_workers": {
+        "_type": "choice",
+        "_value": [
+            8
+        ]
+    },
     "data.type": {
         "_type": "choice",
         "_value": [
             "FootballDatasetV2"
         ]
     },
     "model.bias": {
         "_type": "choice",
         "_value": [
             true,
             false
         ]
     },
+    "model.checkpoint": {
+        "_type": "choice",
+        "_value": [
+            null
+        ]
+    },
     "model.drop": {
         "_type": "choice",
         "_value": [
             0.0,
-            0.1,
             0.2,
-            0.3,
-            0.5,
-            0.7
+            0.5
         ]
     },
     "model.enable_skip": {
         "_type": "choice",
         "_value": [
             true,
             false
         ]
     },
     "model.hidden_features": {
         "_type": "choice",
         "_value": [
             128,
-            192,
             256,
-            320,
             384,
             512,
-            640,
-            768
+            640
         ]
     },
     "model.in_features": {
         "_type": "choice",
         "_value": [
-            122
+            111
         ]
     },
     "model.n_layers": {
         "_type": "choice",
         "_value": [
             1,
             5,
@@ -95,44 +105,53 @@
     },
     "model.team_embedding_dim": {
         "_type": "choice",
         "_value": [
             10,
             30,
             50,
-            70,
             100
         ]
     },
     "model.team_embeddings": {
         "_type": "choice",
         "_value": [
             4000
         ]
     },
+    "model.trainable_layers": {
+        "_type": "choice",
+        "_value": [
+            null
+        ]
+    },
     "model.type": {
         "_type": "choice",
         "_value": [
             "STNetV4"
         ]
     },
     "optimizer.lr": {
-        "_type": "uniform",
+        "_type": "choice",
         "_value": [
-            0.0002,
-            0.005
+            5e-05,
+            0.0001,
+            0.001,
+            0.002
         ]
     },
     "optimizer.type": {
         "_type": "choice",
         "_value": [
             "AdamW"
         ]
     },
     "optimizer.weight_decay": {
-        "_type": "uniform",
+        "_type": "choice",
         "_value": [
+            5e-05,
             0.0001,
-            0.05
+            0.05,
+            0.1
         ]
     }
 }
```

### Comparing `quant2-0.1.4/tools/experimental/nni_model.py` & `quant2-0.1.5/tools/experimental/nni_model.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.4/tools/fb_cls_test.py` & `quant2-0.1.5/tools/fb_cls_test.py`

 * *Files identical despite different names*

### Comparing `quant2-0.1.4/tools/fb_cls_train.py` & `quant2-0.1.5/tools/experimental/nni_football.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-# PYTHONPATH=$(pwd) python tools/fb_cls_train.py
+import nni
 import numpy as np
 import random
 import sys
 import time
 import torch
 from copy import deepcopy
 from pathlib import Path
 from quant.football.data.dataset import get_dataset
+from quant.football.data.sampler import RandomSubsetSampler
 from quant.football.models import get_model
 from quant.utils.config import get_config, merge_from_dict
 from quant.utils.io import copy_file, save_json
 from quant.utils.logging import get_logger, print_log
 
 
 def train(model, device, train_loader, loss_fn, optimizer, epoch, log_interval, verbose, logger):
@@ -52,102 +53,136 @@
     print_log(
         f"\nTest set: Avg loss: {test_loss:.6f}, Acc: {correct}/{dataset_size} ({test_acc:.4f})\n", verbose, logger)
     return test_acc
 
 
 def main(cfg, verbose=True):
     _cfg = deepcopy(cfg)
-    data, model, loss, optimizer, scheduler, runtime = \
+    data_cfg, model_cfg, loss_cfg, optimizer_cfg, scheduler_cfg, runtime_cfg = \
         cfg["data"], cfg["model"], cfg["loss"], cfg["optimizer"], cfg["scheduler"], cfg["runtime"]
 
-    seed = runtime.get("seed", 1)
-    epochs = runtime.get("epochs", 90)
-    device = runtime.get("device", "cuda")
-    log_interval = runtime.get("log_interval", 10)
+    seed = runtime_cfg.get("seed", 1)
+    epochs = runtime_cfg.get("epochs", 90)
+    device = runtime_cfg.get("device", "cuda")
+    log_interval = runtime_cfg.get("log_interval", 10)
 
     random.seed(seed)
     np.random.seed(seed)
     torch.manual_seed(seed)
-    torch.backends.cudnn.deterministic = True
-    torch.backends.cudnn.benchmark = False
+    torch.backends.cudnn.deterministic = False
+    torch.backends.cudnn.benchmark = True
 
     if device == "cuda" and torch.cuda.is_available():
         device = torch.device("cuda")
     else:
         device = torch.device("cpu")
 
-    dataset_type = data.pop("type")
-    data_root = Path(data["data_root"])
-    train_dataset = get_dataset(dataset_type, data_root / data["train_file"])
-    test_dataset = get_dataset(dataset_type, data_root / data["test_file"])
+    dataset_type = data_cfg.pop("type")
+    data_root = Path(data_cfg["data_root"])
+    train_dataset = get_dataset(dataset_type, data_root / data_cfg["train_file"])
+    test_dataset = get_dataset(dataset_type, data_root / data_cfg["test_file"])
+
+    fraction = data_cfg.get("fraction", None)
+    num_samples = data_cfg.get("num_samples", None)
+    sampler = RandomSubsetSampler(len(train_dataset), num_samples, fraction)
+
+    num_workers = data_cfg.get("num_workers", 8)
 
     train_loader = torch.utils.data.DataLoader(
-        train_dataset, batch_size=data["batch_size"], shuffle=True
+        train_dataset, batch_size=data_cfg["batch_size"], sampler=sampler, num_workers=num_workers, drop_last=True
     )
     test_loader = torch.utils.data.DataLoader(
-        test_dataset, batch_size=128
+        test_dataset, batch_size=128, num_workers=num_workers
     )
 
-    model_type = model.pop("type")
-    model = get_model(model_type, **model).to(device)
+    model_type = model_cfg.pop("type")
+    model = get_model(model_type, **model_cfg)
+
+    checkpoint = model_cfg.get("checkpoint", None)
+    if checkpoint is not None:
+        model.load_state_dict(torch.load(checkpoint, map_location=torch.device("cpu")))
+
+    # layers, layers.0, layers.0.1, norm, head.weight, head.bias
+    frozen_layers = model_cfg.get("frozen_layers", None)
+    if frozen_layers is not None:
+        for name, param in model.named_parameters():
+            param.requires_grad = True
+            for layer_name in frozen_layers:
+                if layer_name in name:
+                    param.requires_grad = False
+                    break
+
+    # season_embedding, team_embedding, stem
+    trainable_layers = model_cfg.get("trainable_layers", None)
+    if trainable_layers is not None:
+        for name, param in model.named_parameters():
+            param.requires_grad = False
+            for layer_name in trainable_layers:
+                if layer_name in name:
+                    param.requires_grad = True
+                    break
 
-    loss_type = loss.pop("type")
+    model = model.to(device)
+
+    loss_type = loss_cfg.pop("type")
     if loss_type == "CrossEntropyLoss":
         from torch.nn import CrossEntropyLoss
-        loss_fn = CrossEntropyLoss(**loss).to(device)
+        loss_fn = CrossEntropyLoss(**loss_cfg).to(device)
     else:
         raise NotImplementedError(f"Not supported <{loss_type}>.")
 
-    optimizer_type = optimizer.pop("type")
+    params = [param for param in model.parameters() if param.requires_grad]
+    optimizer_type = optimizer_cfg.pop("type")
     if optimizer_type == "SGD":
         from torch.optim import SGD
-        optimizer.setdefault("momentum", 0.9)
-        optimizer = SGD(model.parameters(), **optimizer)
+        optimizer_cfg.setdefault("momentum", 0.9)
+        optimizer = SGD(params, **optimizer_cfg)
     elif optimizer_type == "AdamW":
         from torch.optim import AdamW
-        optimizer.setdefault("betas", (0.9, 0.999))
-        if isinstance(optimizer["betas"], str):
-            optimizer["betas"] = eval(optimizer["betas"])
-        optimizer = AdamW(model.parameters(), **optimizer)
+        optimizer_cfg.setdefault("betas", (0.9, 0.999))
+        if isinstance(optimizer_cfg["betas"], str):
+            optimizer_cfg["betas"] = eval(optimizer_cfg["betas"])
+        optimizer = AdamW(params, **optimizer_cfg)
     else:
         raise NotImplementedError(f"Not supported <{optimizer_type}>.")
 
-    scheduler_type = scheduler.pop("type")
+    scheduler_type = scheduler_cfg.pop("type")
     if scheduler_type == "StepLR":
         from torch.optim.lr_scheduler import StepLR
-        scheduler = StepLR(optimizer, **scheduler)
+        scheduler = StepLR(optimizer, **scheduler_cfg)
     else:
         raise NotImplementedError(f"Not supported <{scheduler_type}>.")
 
-    trial_name = time.strftime("%Y%m%d%H%M%S")
+    trial_name = time.strftime("%Y%m%d") + f"_{nni.get_experiment_id()}_{nni.get_sequence_id():04d}"
     out_dir = Path("runs") / data_root.name / trial_name
     out_dir.mkdir(parents=True, exist_ok=True)
     copy_file(data_root, out_dir, "*.json")
 
     logger = get_logger(__name__, False, out_dir / "log.txt")
 
     best_acc, best_epoch = 0.0, -1
     for epoch in range(1, epochs + 1):
         train(model, device, train_loader, loss_fn, optimizer,
               epoch, log_interval, verbose, logger)
         curr_acc = test(model, device, test_loader, loss_fn,
                         verbose, logger)
+        nni.report_intermediate_result(curr_acc)
         if curr_acc > best_acc:
             best_acc, best_epoch = curr_acc, epoch
             torch.save(model.state_dict(), out_dir / "best.pt")
         scheduler.step()
     torch.save(model.state_dict(), out_dir / "last.pt")
     last_acc_test = curr_acc
 
     print_log("[best model]", verbose, logger)
     print_log(f"\noutput dir: {out_dir}", verbose, logger)
     print_log(f"{best_acc=:.4f}, {best_epoch=:03d}\n", verbose, logger)
 
     print_log("[check train dataset]", verbose, logger)
-    check_loader = torch.utils.data.DataLoader(train_dataset, batch_size=128)
+    check_loader = torch.utils.data.DataLoader(train_dataset, batch_size=128, num_workers=num_workers)
     last_acc_train = test(model, device, check_loader, loss_fn,
                           verbose, logger)
 
     _cfg["log"] = {
         "out_dir": str(out_dir),
         "date": time.strftime("%Y-%m-%d %H:%M:%S"),
         "best_acc": best_acc,
@@ -165,9 +200,12 @@
     for arg in sys.argv[1:]:
         key, val = arg.split("=", maxsplit=1)
         options[key] = eval(val)
 
     cfg = get_config(options.get("config", None))
     cfg = merge_from_dict(cfg, options)
 
+    optimized_params = nni.get_next_parameter()
+    cfg = merge_from_dict(cfg, optimized_params)
+
     best_acc, _cfg = main(cfg, verbose=False)
-    print({"default": best_acc, "log": _cfg["log"]})
+    nni.report_final_result({"default": best_acc, "log": _cfg["log"]})
```

### Comparing `quant2-0.1.4/PKG-INFO` & `quant2-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quant2
-Version: 0.1.4
+Version: 0.1.5
 Summary: A collection of useful tools!
 Author-email: Hejian <flystarhe@qq.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: prettytable
 Requires-Dist: scikit-learn
```

