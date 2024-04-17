# Comparing `tmp/ms-swift-2.0.0.tar.gz` & `tmp/ms-swift-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ms-swift-2.0.0.tar", last modified: Mon Apr 15 08:42:44 2024, max compression
+gzip compressed data, was "dist/ms-swift-2.0.1.tar", last modified: Wed Apr 17 03:41:13 2024, max compression
```

## Comparing `ms-swift-2.0.0.tar` & `ms-swift-2.0.1.tar`

### file list

```diff
@@ -1,227 +1,227 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-15 08:42:39.000000 ms-swift-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    54434 2024-04-15 08:42:44.000000 ms-swift-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    49082 2024-04-15 08:42:39.000000 ms-swift-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/ms_swift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    54434 2024-04-15 08:42:44.000000 ms-swift-2.0.0/ms_swift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-04-15 08:42:44.000000 ms-swift-2.0.0/ms_swift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:42:44.000000 ms-swift-2.0.0/ms_swift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-15 08:42:44.000000 ms-swift-2.0.0/ms_swift.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:42:44.000000 ms-swift-2.0.0/ms_swift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-15 08:42:44.000000 ms-swift-2.0.0/ms_swift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-15 08:42:44.000000 ms-swift-2.0.0/ms_swift.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-15 08:42:39.000000 ms-swift-2.0.0/requirements/aigc.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-15 08:42:39.000000 ms-swift-2.0.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 08:42:39.000000 ms-swift-2.0.0/requirements/eval.txt
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-15 08:42:39.000000 ms-swift-2.0.0/requirements/framework.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-15 08:42:39.000000 ms-swift-2.0.0/requirements/llm.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-15 08:42:39.000000 ms-swift-2.0.0/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-15 08:42:44.000000 ms-swift-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-04-15 08:42:39.000000 ms-swift-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/aigc/
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23301 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/animatediff.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/animatediff_infer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/aigc/diffusers/
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/infer_controlnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/infer_controlnet_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/infer_dreambooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/infer_dreambooth_lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/infer_dreambooth_lora_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/infer_text_to_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/infer_text_to_image_lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/infer_text_to_image_lora_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/infer_text_to_image_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)    48449 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/train_controlnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    54249 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/train_controlnet_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)    60203 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/train_dreambooth.py
--rw-r--r--   0 runner    (1001) docker     (127)    58211 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/train_dreambooth_lora.py
--rw-r--r--   0 runner    (1001) docker     (127)    71598 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/train_dreambooth_lora_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)    46799 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/train_text_to_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    42456 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/train_text_to_image_lora.py
--rw-r--r--   0 runner    (1001) docker     (127)    53924 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/train_text_to_image_lora_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)    57714 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/diffusers/train_text_to_image_sdxl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/aigc/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/aigc/utils/argument.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/cli/app_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/cli/dpo.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/cli/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/cli/export.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/cli/infer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/cli/merge_lora.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/cli/sft.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/cli/web_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/hub/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30552 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/hub/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/hub/check_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/hub/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/hub/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    12719 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/hub/file_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/hub/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/hub/push_to_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)    13006 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/hub/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/hub/snapshot_download.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/hub/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/hub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9906 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/hub/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/hub/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/llm/
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/accelerator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/llm/agent/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/agent/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/app_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/llm/data/
--rw-r--r--   0 runner    (1001) docker     (127)    27203 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/data/self_cognition.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/dpo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/llm/ds_config/
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/ds_config/zero2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/ds_config/zero3.json
--rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     7804 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/export.py
--rw-r--r--   0 runner    (1001) docker     (127)    20092 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/infer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/rome.py
--rw-r--r--   0 runner    (1001) docker     (127)    12944 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/sft.py
--rw-r--r--   0 runner    (1001) docker     (127)    10739 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/llm/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51305 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/utils/argument.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/utils/client_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    52727 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)   107400 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/utils/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8830 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/utils/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/utils/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    51488 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/utils/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    34502 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17195 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/llm/utils/vllm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11731 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/torchacc_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/trainers/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/trainers/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/trainers/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)    14917 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/trainers/dpo_trainers.py
--rw-r--r--   0 runner    (1001) docker     (127)    30353 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/trainers/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/trainers/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/trainers/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/trainers/optimizers/galore/
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/trainers/optimizers/galore/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11202 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/trainers/optimizers/galore/adafactor.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6229 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/trainers/optimizers/galore/adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/trainers/optimizers/galore/adamw8bit.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5700 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/trainers/optimizers/galore/galore_projector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/trainers/optimizers/galore/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14440 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/trainers/trainers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/trainers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/tuners/
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    43987 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/llamapro.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/tuners/longlora/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/longlora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19267 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/longlora/llama.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/longlora/longlora.py
--rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)    40712 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/lora_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/module_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/neftune.py
--rw-r--r--   0 runner    (1001) docker     (127)    14847 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/peft.py
--rw-r--r--   0 runner    (1001) docker     (127)    10487 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)    17294 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/restuning.py
--rw-r--r--   0 runner    (1001) docker     (127)    13552 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/restuning_components.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/tuners/rome/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/rome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/rome/compute_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/rome/compute_v.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/rome/context_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/rome/hparams.py
--rw-r--r--   0 runner    (1001) docker     (127)    15874 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/rome/nethook.py
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/rome/repr_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/rome/rome.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/rome/rome_hparams.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/tuners/scetuning/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/scetuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/scetuning/scetuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/scetuning/scetuning_components.py
--rw-r--r--   0 runner    (1001) docker     (127)    10583 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/side.py
--rw-r--r--   0 runner    (1001) docker     (127)    16154 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/tuners/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/ui/llm_infer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_infer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_infer/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    18409 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_infer/llm_infer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_infer/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10432 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_infer/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/ui/llm_train/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_train/advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_train/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_train/hyper.py
--rw-r--r--   0 runner    (1001) docker     (127)    15339 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_train/llm_train.py
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_train/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_train/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_train/quantization.py
--rw-r--r--   0 runner    (1001) docker     (127)    15690 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_train/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_train/save.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_train/self_cog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/ui/llm_train/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/swift/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/utils/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/utils/import_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/utils/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/utils/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/utils/np_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/utils/run_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/utils/tb_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-15 08:42:39.000000 ms-swift-2.0.0/swift/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/tests/hub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/hub/test_check_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/tests/llm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/llm/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    20380 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/llm/test_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    27223 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/llm/test_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/llm/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/llm/test_vllm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/model_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)    22281 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/run.py
--rw-r--r--   0 runner    (1001) docker     (127)    12312 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/tests/tuners/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/tuners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/tuners/test_extra_state_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/tuners/test_merged_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/tuners/test_neft.py
--rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/tuners/test_peft.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/tuners/test_rome.py
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/tuners/test_scetuning.py
--rw-r--r--   0 runner    (1001) docker     (127)    23706 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/tuners/test_swift_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/tuners/test_swift_device_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/tuners/test_swift_restuning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:44.000000 ms-swift-2.0.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/utils/test_io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-15 08:42:39.000000 ms-swift-2.0.0/tests/utils/test_torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:13.000000 ms-swift-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-17 03:41:11.000000 ms-swift-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    55120 2024-04-17 03:41:13.000000 ms-swift-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    49736 2024-04-17 03:41:11.000000 ms-swift-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:13.000000 ms-swift-2.0.1/ms_swift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    55120 2024-04-17 03:41:13.000000 ms-swift-2.0.1/ms_swift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-04-17 03:41:13.000000 ms-swift-2.0.1/ms_swift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 03:41:13.000000 ms-swift-2.0.1/ms_swift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-17 03:41:13.000000 ms-swift-2.0.1/ms_swift.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 03:41:13.000000 ms-swift-2.0.1/ms_swift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-17 03:41:13.000000 ms-swift-2.0.1/ms_swift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-17 03:41:13.000000 ms-swift-2.0.1/ms_swift.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:13.000000 ms-swift-2.0.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 03:41:11.000000 ms-swift-2.0.1/requirements/aigc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-17 03:41:11.000000 ms-swift-2.0.1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 03:41:11.000000 ms-swift-2.0.1/requirements/eval.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-17 03:41:11.000000 ms-swift-2.0.1/requirements/framework.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-17 03:41:11.000000 ms-swift-2.0.1/requirements/llm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-17 03:41:11.000000 ms-swift-2.0.1/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-17 03:41:13.000000 ms-swift-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-04-17 03:41:11.000000 ms-swift-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:13.000000 ms-swift-2.0.1/swift/
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:13.000000 ms-swift-2.0.1/swift/aigc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/aigc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23301 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/aigc/animatediff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/aigc/animatediff_infer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:13.000000 ms-swift-2.0.1/swift/aigc/diffusers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/aigc/diffusers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/aigc/diffusers/infer_controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/aigc/diffusers/infer_controlnet_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/aigc/diffusers/infer_dreambooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/aigc/diffusers/infer_dreambooth_lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/aigc/diffusers/infer_dreambooth_lora_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/aigc/diffusers/infer_text_to_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/aigc/diffusers/infer_text_to_image_lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/aigc/diffusers/infer_text_to_image_lora_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/aigc/diffusers/infer_text_to_image_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48449 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/aigc/diffusers/train_controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54249 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/aigc/diffusers/train_controlnet_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60203 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/aigc/diffusers/train_dreambooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58211 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/aigc/diffusers/train_dreambooth_lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71598 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/aigc/diffusers/train_dreambooth_lora_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46799 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/aigc/diffusers/train_text_to_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42456 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/aigc/diffusers/train_text_to_image_lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53924 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/aigc/diffusers/train_text_to_image_lora_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57714 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/aigc/diffusers/train_text_to_image_sdxl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:13.000000 ms-swift-2.0.1/swift/aigc/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/aigc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/aigc/utils/argument.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:13.000000 ms-swift-2.0.1/swift/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/cli/app_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/cli/dpo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/cli/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/cli/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/cli/infer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/cli/merge_lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/cli/sft.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/cli/web_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:13.000000 ms-swift-2.0.1/swift/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30552 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/hub/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/hub/check_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/hub/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/hub/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12719 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/hub/file_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/hub/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/hub/push_to_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13006 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/hub/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/hub/snapshot_download.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:13.000000 ms-swift-2.0.1/swift/hub/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/hub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9906 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/hub/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/hub/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:13.000000 ms-swift-2.0.1/swift/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/llm/accelerator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:13.000000 ms-swift-2.0.1/swift/llm/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/llm/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/llm/agent/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/llm/app_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:13.000000 ms-swift-2.0.1/swift/llm/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    27203 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/llm/data/self_cognition.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/llm/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/llm/dpo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:13.000000 ms-swift-2.0.1/swift/llm/ds_config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/llm/ds_config/zero2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/llm/ds_config/zero3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/llm/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7842 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/llm/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20318 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/llm/infer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/llm/rome.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12944 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/llm/sft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10683 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/llm/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:13.000000 ms-swift-2.0.1/swift/llm/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/llm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51349 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/llm/utils/argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/llm/utils/client_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52727 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/llm/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)   112933 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/llm/utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8830 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/llm/utils/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/llm/utils/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53634 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/llm/utils/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34502 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/llm/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17195 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/llm/utils/vllm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11731 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/torchacc_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:13.000000 ms-swift-2.0.1/swift/trainers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/trainers/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/trainers/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14917 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/trainers/dpo_trainers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30575 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/trainers/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:13.000000 ms-swift-2.0.1/swift/trainers/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/trainers/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:13.000000 ms-swift-2.0.1/swift/trainers/optimizers/galore/
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/trainers/optimizers/galore/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11202 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/trainers/optimizers/galore/adafactor.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6229 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/trainers/optimizers/galore/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/trainers/optimizers/galore/adamw8bit.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5700 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/trainers/optimizers/galore/galore_projector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/trainers/optimizers/galore/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15709 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/trainers/trainers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/trainers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:13.000000 ms-swift-2.0.1/swift/tuners/
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/tuners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/tuners/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43987 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/tuners/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/tuners/llamapro.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:13.000000 ms-swift-2.0.1/swift/tuners/longlora/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/tuners/longlora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/tuners/longlora/llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/tuners/longlora/longlora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/tuners/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40224 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/tuners/lora_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/tuners/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/tuners/module_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/tuners/neftune.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14325 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/tuners/peft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10487 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/tuners/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17294 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/tuners/restuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13552 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/tuners/restuning_components.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:13.000000 ms-swift-2.0.1/swift/tuners/rome/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/tuners/rome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/tuners/rome/compute_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/tuners/rome/compute_v.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/tuners/rome/context_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/tuners/rome/hparams.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15874 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/tuners/rome/nethook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/tuners/rome/repr_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/tuners/rome/rome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/tuners/rome/rome_hparams.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:13.000000 ms-swift-2.0.1/swift/tuners/scetuning/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/tuners/scetuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/tuners/scetuning/scetuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/tuners/scetuning/scetuning_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10583 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/tuners/side.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16154 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/tuners/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:13.000000 ms-swift-2.0.1/swift/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/ui/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/ui/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:13.000000 ms-swift-2.0.1/swift/ui/llm_infer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/ui/llm_infer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/ui/llm_infer/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18467 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/ui/llm_infer/llm_infer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/ui/llm_infer/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10432 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/ui/llm_infer/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:13.000000 ms-swift-2.0.1/swift/ui/llm_train/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/ui/llm_train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/ui/llm_train/advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/ui/llm_train/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/ui/llm_train/hyper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15408 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/ui/llm_train/llm_train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/ui/llm_train/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/ui/llm_train/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/ui/llm_train/quantization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16332 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/ui/llm_train/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/ui/llm_train/save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/ui/llm_train/self_cog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/ui/llm_train/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:13.000000 ms-swift-2.0.1/swift/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/utils/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/utils/import_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/utils/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/utils/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/utils/np_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/utils/run_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/utils/tb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-17 03:41:11.000000 ms-swift-2.0.1/swift/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:13.000000 ms-swift-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:11.000000 ms-swift-2.0.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:13.000000 ms-swift-2.0.1/tests/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:11.000000 ms-swift-2.0.1/tests/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-17 03:41:11.000000 ms-swift-2.0.1/tests/hub/test_check_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:13.000000 ms-swift-2.0.1/tests/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:11.000000 ms-swift-2.0.1/tests/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-17 03:41:11.000000 ms-swift-2.0.1/tests/llm/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20380 2024-04-17 03:41:11.000000 ms-swift-2.0.1/tests/llm/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27223 2024-04-17 03:41:11.000000 ms-swift-2.0.1/tests/llm/test_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-17 03:41:11.000000 ms-swift-2.0.1/tests/llm/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-17 03:41:11.000000 ms-swift-2.0.1/tests/llm/test_vllm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-04-17 03:41:11.000000 ms-swift-2.0.1/tests/model_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22281 2024-04-17 03:41:11.000000 ms-swift-2.0.1/tests/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12312 2024-04-17 03:41:11.000000 ms-swift-2.0.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:13.000000 ms-swift-2.0.1/tests/tuners/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:11.000000 ms-swift-2.0.1/tests/tuners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-04-17 03:41:11.000000 ms-swift-2.0.1/tests/tuners/test_extra_state_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-17 03:41:11.000000 ms-swift-2.0.1/tests/tuners/test_merged_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-04-17 03:41:11.000000 ms-swift-2.0.1/tests/tuners/test_neft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-04-17 03:41:11.000000 ms-swift-2.0.1/tests/tuners/test_peft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-17 03:41:11.000000 ms-swift-2.0.1/tests/tuners/test_rome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-17 03:41:11.000000 ms-swift-2.0.1/tests/tuners/test_scetuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23706 2024-04-17 03:41:11.000000 ms-swift-2.0.1/tests/tuners/test_swift_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-17 03:41:11.000000 ms-swift-2.0.1/tests/tuners/test_swift_device_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-04-17 03:41:11.000000 ms-swift-2.0.1/tests/tuners/test_swift_restuning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:13.000000 ms-swift-2.0.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 03:41:11.000000 ms-swift-2.0.1/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-17 03:41:11.000000 ms-swift-2.0.1/tests/utils/test_io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-17 03:41:11.000000 ms-swift-2.0.1/tests/utils/test_torch_utils.py
```

### Comparing `ms-swift-2.0.0/PKG-INFO` & `ms-swift-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-swift
-Version: 2.0.0
+Version: 2.0.1
 Summary: Swift: Scalable lightWeight Infrastructure for Fine-Tuning
 Home-page: https://github.com/modelscope/swift
 Author: DAMO ModelScope teams
 Author-email: contact@modelscope.cn
 License: Apache License 2.0
 Description: # SWIFT (Scalable lightWeight Infrastructure for Fine-Tuning)
         
@@ -43,29 +43,31 @@
         SWIFT supports training, inference, evaluation and deployment of nearly **200 LLMs and MLLMs** (multimodal large models). Developers can directly apply our framework to their own research and production environments to realize the complete workflow from model training and evaluation to application. In addition to supporting the lightweight training solutions provided by [PEFT](https://github.com/huggingface/peft), we also provide a complete **Adapters library** to support the latest training techniques such as NEFTune, LoRA+, LLaMA-PRO, etc. This adapter library can be used directly in your own custom workflow without our training scripts.
         
         To facilitate use by users unfamiliar with deep learning, we provide a Gradio web-ui for controlling training and inference, as well as accompanying deep learning courses and best practices for beginners.
         
         Additionally, we are expanding capabilities for other modalities. Currently, we support full-parameter training and LoRA training for AnimateDiff.
         
         ## 🎉 News
+        - 🔥2024.04.17: Support **CodeQwen1.5-7B** series: CodeQwen1.5-7B, CodeQwen1.5-7B-Chat,CodeQwen1.5-7B-Chat-AWQ, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/codeqwen1half_7b_chat/lora/sft.sh) to train.
+        - 2024.04.16: Supports inference and fine-tuning of llava-v1.6-34b model. For best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/llava-best-practice.md).
         - 2024.04.13: Support the fine-tuning and inference of Mixtral-8x22B-v0.1 model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mixtral_moe_8x22b_v1/lora_ddp_ds/sft.sh) to start training!
         - 2024.04.13: Support the newly launched **MiniCPM** series: MiniCPM-V-2.0、MiniCPM-2B-128k、MiniCPM-MoE-8x2B and MiniCPM-1B.use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/minicpm_moe_8x2b/lora_ddp/sft.sh) to start training!
         - 🔥2024.04.11: Support Model Evaluation with MMLU/ARC/CEval datasets(also user custom eval datasets) with one command! Check [this documentation](docs/source_en/LLM/LLM-eval.md) for details. Meanwhile, we support a trick way to do multiple ablation experiments, check [this documentation](docs/source_en/LLM/LLM-exp.md) to use.
-        - 🔥2024.04.11: Support **c4ai-command-r** series: c4ai-command-r-plus, c4ai-command-r-v01, [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/c4ai-command-r-plus/lora_mp/sft.sh) to train.
+        - 🔥2024.04.11: Support **c4ai-command-r** series: c4ai-command-r-plus, c4ai-command-r-v01, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/c4ai_command_r_plus/lora_mp/sft.sh) to train.
         - 2024.04.10: Use SWIFT to fine-tune the qwen-7b-chat model to enhance its function call capabilities, and combine it with [Modelscope-Agent](https://github.com/modelscope/modelscope-agent) for best practices, which can be found [here](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Agent-best-practice.md#Usage-with-Modelscope_Agent).
         - 🔥2024.04.09: Support ruozhiba dataset. Search `ruozhiba` in [this documentation](docs/source_en/LLM/Supported-models-datasets.md) to begin training!
         - 2024.04.08: Support the fine-tuning and inference of XVERSE-MoE-A4.2B model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/xverse_moe_a4_2b/lora/sft.sh) to start training!
         - 2024.04.04: Support **QLoRA+FSDP** to train a 70B model with two 24G memory GPUs, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/llama2_70b_chat/qlora_fsdp/sft.sh) to train.
         - 🔥2024.04.03: Support **Qwen1.5-32B** series: Qwen1.5-32B, Qwen1.5-32B-Chat, Qwen1.5-32B-Chat-GPTQ-Int4.use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen1half_32b_chat/lora_mp/sft.sh) to start training!
         - 🔥2024.04.02: Support the fine-tuning and inference of Mengzi3-13B-Base model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mengzi3_13b_base/lora_ddp_ds/sft.sh) to start training!
         - 🔥2024.04.01: Support **dbrx** series: dbrx-base and dbrx-instruct, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/dbrx-instruct/lora_mp/sft.sh) to start training!
         - 🔥2024.03.29: Support **Qwen1.5-MoE** series: Qwen1.5-MoE-A2.7B, Qwen1.5-MoE-A2.7B-Chat, Qwen1.5-MoE-A2.7B-Chat-GPTQ-Int4.
         - 🔥2024.03.29: Support the fine-tuning and inference of **Grok-1** 300B MoE, please view details [here](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Grok-1-best-practice.md).
         - 🔥2024.03.25: Supports inference and fine-tuning of TeleChat-7b and TeleChat-12b model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/telechat_12b/lora/sft.sh) to start training!
-        - 🔥2024.03.20: Supports inference and fine-tuning for the **llava** series. For best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source/Multi-Modal/llava最佳实践.md).
+        - 🔥2024.03.20: Supports inference and fine-tuning for the **llava** series. For best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/llava-best-practice.md).
         - 🔥2024.03.12: Support inference and fine-tuning for **deepseek-vl** series. Best practices can be found [here](docs/source_en/Multi-Modal/deepseek-vl-best-practice.md).
         - 🔥2024.03.11: Support [GaLore](https://arxiv.org/abs/2403.03507) for effectively reducing memory usage to 1/2 of the original in full-parameter training.
         - 🔥2024.03.10: [End-to-end best practices](docs/source_en/LLM/Qwen1.5-best-practice.md) from fine-tuning to deployment for Qwen1.5-7B-Chat and Qwen1.5-72B-Chat.
         - 🔥2024.03.09: Support training and inference of MAMBA model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mamba-1.4b/lora/sft.sh) to start training!
         - 2024.03.09: Support training and inference of AQLM quantized model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/llama2_7b_aqlm_2bit_1x16/lora/sft.sh) to start training!
         - 2024.03.06: Support training and inference of AWQ quantized model, use [this Qwen1.5-AWQ model script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen1half_7b_chat_awq/lora/sft.sh) to start training, and support training and inference of [yi-9b](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_9b/lora_zero3).
         - 🔥2024.02.29: Support [LLaMA PRO](https://arxiv.org/pdf/2401.02415.pdf), simply use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_6b_chat/llamapro/sft.sh) to start training.
@@ -89,15 +91,16 @@
         - 🔥2024.01.26: Support [yi-vl-6b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/yi_vl_6b_chat), yi-vl-34b-chat.
         - 2024.01.24: Support codefuse-codegeex2-6b-chat, codefuse-qwen-14b-chat.
         - 2024.01.23: Support orion series: orion-14b, [orion-14b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/orion_14b_chat).
         - 2024.01.20: Support [xverse-13b-256k](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/xverse_13b_256k), xverse-65b-v2, xverse-65b-chat.
         - 🔥2024.01.17: Support internlm2 series: internlm2-7b-base, internlm2-7b, [internlm2-7b-sft-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/internlm2_7b_sft_chat), internlm2-7b-chat, internlm2-20b-base, internlm2-20b, internlm2-20b-sft-chat, internlm2-20b-chat.
         - 2024.01.15: Support yuan series: yuan2-2b-instruct, [yuan2-2b-janus-instruct](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/yuan2_2b_janus_instruct), yuan2-51b-instruct, yuan2-102b-instruct.
         - 🔥2024.01.12: Support **deepseek-moe** series: deepseek-moe-16b, [deepseek-moe-16b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/deepseek_moe_16b_chat).
-        - 🔥2024.01.04: Support **VLLM deployment**, compatible with **OpenAI API** style, see [VLLM Inference Acceleration and Deployment](https://github.com/modelscope/swift/blob/main/docs/source/LLM/VLLM推理加速与部署.md#部署) for details.
+        - 🔥2024.01.04: Support **VLLM deployment**, compatible with **OpenAI API** style, see [VLLM Inference Acceleration and Deployment](https://github.com/modelscope/swift/blob/main/docs/source_en/LLM/VLLM-inference-acceleration-and-deployment.md#Deployment) for details.
+        
         - 2024.01.04: Update [Benchmark](https://github.com/modelscope/swift/blob/main/docs/source/LLM/Benchmark.md) for convenient viewing of training speed and memory usage of different models.
         - 🔥2023.12.29: Support web-ui for sft training and inference, use `swift web-ui` after installing ms-swift to start.
         - 🔥2023.12.29: Support DPO RLHF (Reinforcement Learning from Human Feedback) and three datasets for this task: AI-ModelScope/stack-exchange-paired, AI-ModelScope/hh-rlhf and AI-ModelScope/hh_rlhf_cn. See [documentation](https://github.com/modelscope/swift/blob/main/docs/source/LLM/LLM%E4%BA%BA%E7%B1%BB%E5%AF%B9%E9%BD%90%E8%AE%AD%E7%BB%83%E6%96%87%E6%A1%A3.md) to start training!
         - 🔥2023.12.28: Support SCEdit! This tuner can significantly reduce memory usage in U-Net and support low-memory controllable image generation (replacing ControlNet), read the section below to learn more.
         - 2023.12.23: Support [codegeex2-6b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/codegeex2_6b).
         - 2023.12.19: Support [phi2-3b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/phi2_3b).
         - 2023.12.18: Support VLLM for inference acceleration.
@@ -383,15 +386,15 @@
         
         ### Supported Models
         
         #### LLMs
         
         | Model Type                                     | Model Introduction                                                     | Language           | Model Size                             | Model Type                                 |
         |------------------------------------------------|------------------------------------------------------------------------|--------------------|----------------------------------------|------------------------------------------- |
-        | Qwen<br>Qwen1.5                                   | [Tongyi Qwen 1.0 and 1.5 series models](https://github.com/QwenLM)  | Chinese<br>English    | 0.5B-72B<br>including quantized versions | base model<br>chat model<br>MoE model                      |
+        | Qwen<br>Qwen1.5                                   | [Tongyi Qwen 1.0 and 1.5 series models](https://github.com/QwenLM)  | Chinese<br>English    | 0.5B-72B<br>including quantized versions | base model<br>chat model<br>MoE model<br>code model                      |
         | ChatGLM2<br>ChatGLM3<br>Codegeex2                    | [Zhipu ChatGLM series models](https://github.com/THUDM)               | Chinese<br>English    | 6B                                     | base model<br>chat model<br>code model  |
         | Baichuan/Baichuan2                             | [Baichuan 1 and Baichuan 2](https://github.com/baichuan-inc)           | Chinese<br>English    | 7B-13B<br>including quantized versions             | base model<br>chat model                       |
         | Yuan2                                          | [Langchao Yuan series models](https://github.com/IEIT-Yuan)             | Chinese<br>English    | 2B-102B                                | instruct model                                 |
         | XVerse                                         | [XVerse series models](https://github.com/xverse-ai)                    | Chinese<br>English    | 7B-65B                                 | base model<br>chat model<br>long text model<br>MoE model                |
         | LLaMA2                                         | [LLaMA2 series models](https://github.com/facebookresearch/llama)       | English            | 7B-70B<br>including quantized versions   | base model<br>chat model                       |
         | Mistral<br>Mixtral                            | [Mistral series models](https://github.com/mistralai/mistral-src)       | English            | 7B-22B     | base model<br>instruct model<br>MoE model                     |
         | YI                                             | [01AI's YI series models](https://github.com/01-ai)                     | Chinese<br>English    | 6B-34B                                 | base model<br>chat model<br>long text model            |
@@ -426,15 +429,16 @@
         | Qwen-VL          | [Tongyi Qwen vision model](https://github.com/QwenLM)               | Chinese<br>English    | 7B<br>including quantized versions | base model<br>chat model |
         | Qwen-Audio       | [Tongyi Qwen speech model](https://github.com/QwenLM)               | Chinese<br>English    | 7B                | base model<br>chat model |
         | YI-VL            | [01AI's YI series vision models](https://github.com/01-ai)             | Chinese<br>English    | 6B-34B            | chat model         |
         | XComposer2       | [Pujiang AI Lab InternLM vision model](https://github.com/InternLM/InternLM) | Chinese<br>English | 7B              | chat model         |
         | DeepSeek-VL      | [DeepSeek series vision models](https://github.com/deepseek-ai) | Chinese<br>English    | 1.3B-7B           | chat model         |
         | MiniCPM-V       | [OpenBmB MiniCPM vision model](https://github.com/OpenBMB/MiniCPM)     | Chinese<br>English    | 3B                | chat model         |
         | CogVLM<br>CogAgent  | [Zhipu ChatGLM visual QA and Agent model](https://github.com/THUDM/)   | English    | 17B-18B           | chat model         |
-        | Llava      | [Llava series models](https://github.com/haotian-liu/LLaVA)                | English | 7B               | chat model |
+        | Llava      | [Llava series models](https://github.com/haotian-liu/LLaVA)                | English | 7B-34B               | chat model |
+        | mPLUG-Owl      | [mPLUG-Owl series models](https://github.com/X-PLUG/mPLUG-Owl)         | English | 11B               | chat model |
         
         #### Diffusion Models
         
         | Model Type          | Model Introduction                                                    | Language | Model Type        |
         |---------------------|----------------------------------------------------------------------|----------|------------------ |
         | AnimateDiff         | [AnimateDiff animation model](https://github.com/guoyww/AnimateDiff) | English  | text-to-video     |
         | SD1.5/SD2.0/SDXL    | [StabilityAI series diffusion models](https://github.com/Stability-AI) | English | text-to-image    |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ms-swift Version: 2.0.0 Summary: Swift: Scalable
+Metadata-Version: 2.1 Name: ms-swift Version: 2.0.1 Summary: Swift: Scalable
 lightWeight Infrastructure for Fine-Tuning Home-page: https://github.com/
 modelscope/swift Author: DAMO ModelScope teams Author-email:
 contact@modelscope.cn License: Apache License 2.0 Description: # SWIFT
 (Scalable lightWeight Infrastructure for Fine-Tuning)
 
                             [resources/banner.png]
                          _M_o_d_e_l_S_c_o_p_e_ _C_o_m_m_u_n_i_t_y_ _W_e_b_s_i_t_e
@@ -26,34 +26,41 @@
 the latest training techniques such as NEFTune, LoRA+, LLaMA-PRO, etc. This
 adapter library can be used directly in your own custom workflow without our
 training scripts. To facilitate use by users unfamiliar with deep learning, we
 provide a Gradio web-ui for controlling training and inference, as well as
 accompanying deep learning courses and best practices for beginners.
 Additionally, we are expanding capabilities for other modalities. Currently, we
 support full-parameter training and LoRA training for AnimateDiff. ## ð News
-- 2024.04.13: Support the fine-tuning and inference of Mixtral-8x22B-v0.1
-model, use [this script](https://github.com/modelscope/swift/blob/main/
-examples/pytorch/llm/scripts/mixtral_moe_8x22b_v1/lora_ddp_ds/sft.sh) to start
-training! - 2024.04.13: Support the newly launched **MiniCPM** series: MiniCPM-
-V-2.0ãMiniCPM-2B-128kãMiniCPM-MoE-8x2B and MiniCPM-1B.use [this script]
-(https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
-minicpm_moe_8x2b/lora_ddp/sft.sh) to start training! - ð¥2024.04.11: Support
-Model Evaluation with MMLU/ARC/CEval datasets(also user custom eval datasets)
-with one command! Check [this documentation](docs/source_en/LLM/LLM-eval.md)
-for details. Meanwhile, we support a trick way to do multiple ablation
-experiments, check [this documentation](docs/source_en/LLM/LLM-exp.md) to use.
-- ð¥2024.04.11: Support **c4ai-command-r** series: c4ai-command-r-plus, c4ai-
-command-r-v01, [this script](https://github.com/modelscope/swift/blob/main/
-examples/pytorch/llm/scripts/c4ai-command-r-plus/lora_mp/sft.sh) to train. -
-2024.04.10: Use SWIFT to fine-tune the qwen-7b-chat model to enhance its
-function call capabilities, and combine it with [Modelscope-Agent](https://
-github.com/modelscope/modelscope-agent) for best practices, which can be found
-[here](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Agent-
-best-practice.md#Usage-with-Modelscope_Agent). - ð¥2024.04.09: Support
-ruozhiba dataset. Search `ruozhiba` in [this documentation](docs/source_en/LLM/
+- ð¥2024.04.17: Support **CodeQwen1.5-7B** series: CodeQwen1.5-7B,
+CodeQwen1.5-7B-Chat,CodeQwen1.5-7B-Chat-AWQ, use [this script](https://
+github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
+codeqwen1half_7b_chat/lora/sft.sh) to train. - 2024.04.16: Supports inference
+and fine-tuning of llava-v1.6-34b model. For best practice, you can refer to
+[here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-
+Modal/llava-best-practice.md). - 2024.04.13: Support the fine-tuning and
+inference of Mixtral-8x22B-v0.1 model, use [this script](https://github.com/
+modelscope/swift/blob/main/examples/pytorch/llm/scripts/mixtral_moe_8x22b_v1/
+lora_ddp_ds/sft.sh) to start training! - 2024.04.13: Support the newly launched
+**MiniCPM** series: MiniCPM-V-2.0ãMiniCPM-2B-128kãMiniCPM-MoE-8x2B and
+MiniCPM-1B.use [this script](https://github.com/modelscope/swift/blob/main/
+examples/pytorch/llm/scripts/minicpm_moe_8x2b/lora_ddp/sft.sh) to start
+training! - ð¥2024.04.11: Support Model Evaluation with MMLU/ARC/CEval
+datasets(also user custom eval datasets) with one command! Check [this
+documentation](docs/source_en/LLM/LLM-eval.md) for details. Meanwhile, we
+support a trick way to do multiple ablation experiments, check [this
+documentation](docs/source_en/LLM/LLM-exp.md) to use. - ð¥2024.04.11: Support
+**c4ai-command-r** series: c4ai-command-r-plus, c4ai-command-r-v01, use [this
+script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/
+scripts/c4ai_command_r_plus/lora_mp/sft.sh) to train. - 2024.04.10: Use SWIFT
+to fine-tune the qwen-7b-chat model to enhance its function call capabilities,
+and combine it with [Modelscope-Agent](https://github.com/modelscope/
+modelscope-agent) for best practices, which can be found [here](https://
+github.com/modelscope/swift/tree/main/docs/source_en/LLM/Agent-best-
+practice.md#Usage-with-Modelscope_Agent). - ð¥2024.04.09: Support ruozhiba
+dataset. Search `ruozhiba` in [this documentation](docs/source_en/LLM/
 Supported-models-datasets.md) to begin training! - 2024.04.08: Support the
 fine-tuning and inference of XVERSE-MoE-A4.2B model, use [this script](https://
 github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
 xverse_moe_a4_2b/lora/sft.sh) to start training! - 2024.04.04: Support
 **QLoRA+FSDP** to train a 70B model with two 24G memory GPUs, use [this script]
 (https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
 llama2_70b_chat/qlora_fsdp/sft.sh) to train. - ð¥2024.04.03: Support
@@ -71,16 +78,16 @@
 fine-tuning and inference of **Grok-1** 300B MoE, please view details [here]
 (https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Grok-1-best-
 practice.md). - ð¥2024.03.25: Supports inference and fine-tuning of TeleChat-
 7b and TeleChat-12b model, use [this script](https://github.com/modelscope/
 swift/blob/main/examples/pytorch/llm/scripts/telechat_12b/lora/sft.sh) to start
 training! - ð¥2024.03.20: Supports inference and fine-tuning for the
 **llava** series. For best practice, you can refer to [here](https://
-github.com/modelscope/swift/tree/main/docs/source/Multi-Modal/
-llavaæä½³å®è·µ.md). - ð¥2024.03.12: Support inference and fine-tuning for
+github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/llava-best-
+practice.md). - ð¥2024.03.12: Support inference and fine-tuning for
 **deepseek-vl** series. Best practices can be found [here](docs/source_en/
 Multi-Modal/deepseek-vl-best-practice.md). - ð¥2024.03.11: Support [GaLore]
 (https://arxiv.org/abs/2403.03507) for effectively reducing memory usage to 1/
 2 of the original in full-parameter training. - ð¥2024.03.10: [End-to-end
 best practices](docs/source_en/LLM/Qwen1.5-best-practice.md) from fine-tuning
 to deployment for Qwen1.5-7B-Chat and Qwen1.5-72B-Chat. - ð¥2024.03.09:
 Support training and inference of MAMBA model, use [this script](https://
@@ -152,23 +159,24 @@
 [yuan2-2b-janus-instruct](https://github.com/modelscope/swift/tree/main/
 examples/pytorch/llm/scripts/yuan2_2b_janus_instruct), yuan2-51b-instruct,
 yuan2-102b-instruct. - ð¥2024.01.12: Support **deepseek-moe** series:
 deepseek-moe-16b, [deepseek-moe-16b-chat](https://github.com/modelscope/swift/
 tree/main/examples/pytorch/llm/scripts/deepseek_moe_16b_chat). -
 ð¥2024.01.04: Support **VLLM deployment**, compatible with **OpenAI API**
 style, see [VLLM Inference Acceleration and Deployment](https://github.com/
-modelscope/swift/blob/main/docs/source/LLM/VLLMæ¨çå éä¸é¨ç½².md#é¨ç½²)
-for details. - 2024.01.04: Update [Benchmark](https://github.com/modelscope/
-swift/blob/main/docs/source/LLM/Benchmark.md) for convenient viewing of
-training speed and memory usage of different models. - ð¥2023.12.29: Support
-web-ui for sft training and inference, use `swift web-ui` after installing ms-
-swift to start. - ð¥2023.12.29: Support DPO RLHF (Reinforcement Learning from
-Human Feedback) and three datasets for this task: AI-ModelScope/stack-exchange-
-paired, AI-ModelScope/hh-rlhf and AI-ModelScope/hh_rlhf_cn. See [documentation]
-(https://github.com/modelscope/swift/blob/main/docs/source/LLM/
+modelscope/swift/blob/main/docs/source_en/LLM/VLLM-inference-acceleration-and-
+deployment.md#Deployment) for details. - 2024.01.04: Update [Benchmark](https:/
+/github.com/modelscope/swift/blob/main/docs/source/LLM/Benchmark.md) for
+convenient viewing of training speed and memory usage of different models. -
+ð¥2023.12.29: Support web-ui for sft training and inference, use `swift web-
+ui` after installing ms-swift to start. - ð¥2023.12.29: Support DPO RLHF
+(Reinforcement Learning from Human Feedback) and three datasets for this task:
+AI-ModelScope/stack-exchange-paired, AI-ModelScope/hh-rlhf and AI-ModelScope/
+hh_rlhf_cn. See [documentation](https://github.com/modelscope/swift/blob/main/
+docs/source/LLM/
 LLM%E4%BA%BA%E7%B1%BB%E5%AF%B9%E9%BD%90%E8%AE%AD%E7%BB%83%E6%96%87%E6%A1%A3.md)
 to start training! - ð¥2023.12.28: Support SCEdit! This tuner can
 significantly reduce memory usage in U-Net and support low-memory controllable
 image generation (replacing ControlNet), read the section below to learn more.
 - 2023.12.23: Support [codegeex2-6b](https://github.com/modelscope/swift/tree/
 main/examples/pytorch/llm/scripts/codegeex2_6b). - 2023.12.19: Support [phi2-
 3b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
@@ -357,15 +365,16 @@
 -------------|----------------------------------------|------------------------
 ------------------- | | Qwen
 Qwen1.5 | [Tongyi Qwen 1.0 and 1.5 series models](https://github.com/QwenLM) |
 Chinese
 English | 0.5B-72B
 including quantized versions | base model
 chat model
-MoE model | | ChatGLM2
+MoE model
+code model | | ChatGLM2
 ChatGLM3
 Codegeex2 | [Zhipu ChatGLM series models](https://github.com/THUDM) | Chinese
 English | 6B | base model
 chat model
 code model | | Baichuan/Baichuan2 | [Baichuan 1 and Baichuan 2](https://
 github.com/baichuan-inc) | Chinese
 English | 7B-13B
@@ -468,81 +477,83 @@
 English | 7B | chat model | | DeepSeek-VL | [DeepSeek series vision models]
 (https://github.com/deepseek-ai) | Chinese
 English | 1.3B-7B | chat model | | MiniCPM-V | [OpenBmB MiniCPM vision model]
 (https://github.com/OpenBMB/MiniCPM) | Chinese
 English | 3B | chat model | | CogVLM
 CogAgent | [Zhipu ChatGLM visual QA and Agent model](https://github.com/THUDM/
 ) | English | 17B-18B | chat model | | Llava | [Llava series models](https://
-github.com/haotian-liu/LLaVA) | English | 7B | chat model | #### Diffusion
-Models | Model Type | Model Introduction | Language | Model Type | |-----------
-----------|--------------------------------------------------------------------
---|----------|------------------ | | AnimateDiff | [AnimateDiff animation
-model](https://github.com/guoyww/AnimateDiff) | English | text-to-video | |
-SD1.5/SD2.0/SDXL | [StabilityAI series diffusion models](https://github.com/
-Stability-AI) | English | text-to-image | ### Supported Open Source Datasets |
-Dataset Type | Training Task | Documentation | |--------------|:---------------
-|--------------------------------------------------------------- | | General |
-Fine-tuning | ð¥ruozhiba, ð¥ms-bench, ð¥ms-bench-mini, ð¥alpaca-en
-(gpt4), ð¥alpaca-zh(gpt4), multi-alpaca-all, instinwild-en, instinwild-zh,
-cot-en, cot-zh, firefly-all-zh, instruct-en, gpt4all-en, sharegpt-en, sharegpt-
-zh, tulu-v2-sft-mixture, wikipedia-zh, open-orca, open-orca-gpt4, sharegpt-
-gpt4, ð¥sharegpt-gpt4-mini. | | Agent | Fine-tuning | ð¥ms-agent, ms-agent-
-for-agentfabric-default, ms-agent-for-agentfabric-addition, damo-mini-agent-zh,
-damo-agent-zh, agent-instruct-all-en. | | General | Human Alignment | ð¥hh-
-rlhf-cn, stack-exchange-paired, hh-rlhf-harmless-base, hh-rlhf-helpful-base,
-hh-rlhf-helpful-online, hh-rlhf-helpful-rejection-sampled, hh-rlhf-red-team-
-attempts, hh-rlhf-cn-harmless-base-cn, hh-rlhf-cn-helpful-base-cn, hh-rlhf-cn-
-harmless-base-en, hh-rlhf-cn-helpful-base-en. | | Code | Fine-tuning | code-
-alpaca-en, ð¥leetcode-python-en, ð¥codefuse-python-en, ð¥codefuse-evol-
-instruction-zh. | | Medical | Fine-tuning | medical-en, medical-zh, medical-
-mini-zh, ð¥disc-med-sft-zh. | | Legal | Fine-tuning | lawyer-llama-zh,
-tigerbot-law-zh, ð¥disc-law-sft-zh. | | Math | Fine-tuning | ð¥blossom-
-math-zh, school-math-zh, open-platypus-en. | | SQL | Fine-tuning | text2sql-en,
-ð¥sql-create-context-en. | | Text Generation | Fine-tuning | ð¥advertise-
-gen-zh, ð¥dureader-robust-zh. | | Classification | Fine-tuning | cmnli-zh,
-ð¥cmnli-mini-zh, ð¥jd-sentiment-zh, ð¥hc3-zh, ð¥hc3-en. | |
-Quantization Assist | Quantization | pileval. | | Other | Fine-tuning |
-finance-en, poetry-zh, webnovel-zh, generated-chat-zh, cls-fudan-news-zh, ner-
-jave-zh. | | Vision | Fine-tuning | coco-en, ð¥coco-mini-en, coco-mini-en-2,
-capcha-images. | | Audio | Fine-tuning | aishell1-zh, ð¥aishell1-mini-zh. |
-### Supported Technologies | Technology Name | |-------------------------------
--------------------------------- | | ð¥LoRA: [LORA: LOW-RANK ADAPTATION OF
-LARGE LANGUAGE MODELS](https://arxiv.org/abs/2106.09685) | | ð¥LoRA+: [LoRA+:
-Efficient Low Rank Adaptation of Large Models](https://arxiv.org/pdf/
-2402.12354.pdf) | | ð¥LLaMA PRO: [LLAMA PRO: Progressive LLaMA with Block
-Expansion](https://arxiv.org/pdf/2401.02415.pdf) | | ð¥SCEdit: [SCEdit:
-Efficient and Controllable Image Diffusion Generation via Skip Connection
-Editing](https://arxiv.org/abs/2312.11392) < [arXiv](https://arxiv.org/abs/
-2312.11392) \| [Project Page](https://scedit.github.io/) > | | ð¥NEFTune:
-[Noisy Embeddings Improve Instruction Finetuning](https://arxiv.org/abs/
-2310.05914) | | QA-LoRA:[Quantization-Aware Low-Rank Adaptation of Large
-Language Models](https://arxiv.org/abs/2309.14717) | | LongLoRA: [Efficient
-Fine-tuning of Long-Context Large Language Models](https://arxiv.org/abs/
-2309.12307) | | ROME: [Rank-One Editing of Encoder-Decoder Models](https://
-arxiv.org/abs/2211.13317) | | Adapter: [Parameter-Efficient Transfer Learning
-for NLP](http://arxiv.org/abs/1902.00751) | | Prompt Tuning: [Visual Prompt
-Tuning](https://arxiv.org/abs/2203.12119) | | Side: [Side-Tuning: A Baseline
-for Network Adaptation via Additive Side Networks](https://arxiv.org/abs/
-1912.13503) | | Res-Tuning: [Res-Tuning: A Flexible and Efficient Tuning
-Paradigm via Unbinding Tuner from Backbone](https://arxiv.org/abs/2310.19859) <
-[arXiv](https://arxiv.org/abs/2310.19859) \| [Project Page](https://res-
-tuning.github.io/) \| [Usage](docs/source/GetStarted/ResTuning.md) > | | Tuners
-provided by [PEFT](https://github.com/huggingface/peft), such as IA3, AdaLoRA,
-etc. | ### Supported Hardware | Hardware Environment | Notes | |---------------
------------------|-------------------------------------------------| | CPU | |
-| RTX 20/30/40 series, etc. | After 30 series, BF16 and FlashAttn can be used |
-| Computing cards T4/V100, etc. | BF16 and FlashAttn not supported | |
-Computing cards A10/A100, etc. | Support BF16 and FlashAttn | | Huawei Ascend
-NPU | | ## ð Documentation ### Documentation Compiling ```shell make docs #
-Check docs/build/html/index.html in web-browser ``` ### User Guide | Document
-Name | | ------------------------------------------------------------ | |
-[Using Web-UI](docs/source_en/GetStarted/Web-ui.md) | | [Using Tuners](docs/
-source_en/GetStarted/Tuners.md) | | [LLM Fine-tuning](docs/source_en/LLM/LLM-
-fine-tuning.md) | | [LLM Inference](docs/source_en/LLM/LLM-inference.md) | |
-[LLM Quantization](docs/source_en/LLM/LLM-quantization.md) | | [LLM Deployment]
+github.com/haotian-liu/LLaVA) | English | 7B-34B | chat model | | mPLUG-Owl |
+[mPLUG-Owl series models](https://github.com/X-PLUG/mPLUG-Owl) | English | 11B
+| chat model | #### Diffusion Models | Model Type | Model Introduction |
+Language | Model Type | |---------------------|--------------------------------
+--------------------------------------|----------|------------------ | |
+AnimateDiff | [AnimateDiff animation model](https://github.com/guoyww/
+AnimateDiff) | English | text-to-video | | SD1.5/SD2.0/SDXL | [StabilityAI
+series diffusion models](https://github.com/Stability-AI) | English | text-to-
+image | ### Supported Open Source Datasets | Dataset Type | Training Task |
+Documentation | |--------------|:---------------|------------------------------
+--------------------------------- | | General | Fine-tuning | ð¥ruozhiba,
+ð¥ms-bench, ð¥ms-bench-mini, ð¥alpaca-en(gpt4), ð¥alpaca-zh(gpt4),
+multi-alpaca-all, instinwild-en, instinwild-zh, cot-en, cot-zh, firefly-all-zh,
+instruct-en, gpt4all-en, sharegpt-en, sharegpt-zh, tulu-v2-sft-mixture,
+wikipedia-zh, open-orca, open-orca-gpt4, sharegpt-gpt4, ð¥sharegpt-gpt4-mini.
+| | Agent | Fine-tuning | ð¥ms-agent, ms-agent-for-agentfabric-default, ms-
+agent-for-agentfabric-addition, damo-mini-agent-zh, damo-agent-zh, agent-
+instruct-all-en. | | General | Human Alignment | ð¥hh-rlhf-cn, stack-
+exchange-paired, hh-rlhf-harmless-base, hh-rlhf-helpful-base, hh-rlhf-helpful-
+online, hh-rlhf-helpful-rejection-sampled, hh-rlhf-red-team-attempts, hh-rlhf-
+cn-harmless-base-cn, hh-rlhf-cn-helpful-base-cn, hh-rlhf-cn-harmless-base-en,
+hh-rlhf-cn-helpful-base-en. | | Code | Fine-tuning | code-alpaca-en,
+ð¥leetcode-python-en, ð¥codefuse-python-en, ð¥codefuse-evol-instruction-
+zh. | | Medical | Fine-tuning | medical-en, medical-zh, medical-mini-zh,
+ð¥disc-med-sft-zh. | | Legal | Fine-tuning | lawyer-llama-zh, tigerbot-law-
+zh, ð¥disc-law-sft-zh. | | Math | Fine-tuning | ð¥blossom-math-zh, school-
+math-zh, open-platypus-en. | | SQL | Fine-tuning | text2sql-en, ð¥sql-create-
+context-en. | | Text Generation | Fine-tuning | ð¥advertise-gen-zh,
+ð¥dureader-robust-zh. | | Classification | Fine-tuning | cmnli-zh, ð¥cmnli-
+mini-zh, ð¥jd-sentiment-zh, ð¥hc3-zh, ð¥hc3-en. | | Quantization Assist |
+Quantization | pileval. | | Other | Fine-tuning | finance-en, poetry-zh,
+webnovel-zh, generated-chat-zh, cls-fudan-news-zh, ner-jave-zh. | | Vision |
+Fine-tuning | coco-en, ð¥coco-mini-en, coco-mini-en-2, capcha-images. | |
+Audio | Fine-tuning | aishell1-zh, ð¥aishell1-mini-zh. | ### Supported
+Technologies | Technology Name | |---------------------------------------------
+------------------ | | ð¥LoRA: [LORA: LOW-RANK ADAPTATION OF LARGE LANGUAGE
+MODELS](https://arxiv.org/abs/2106.09685) | | ð¥LoRA+: [LoRA+: Efficient Low
+Rank Adaptation of Large Models](https://arxiv.org/pdf/2402.12354.pdf) | |
+ð¥LLaMA PRO: [LLAMA PRO: Progressive LLaMA with Block Expansion](https://
+arxiv.org/pdf/2401.02415.pdf) | | ð¥SCEdit: [SCEdit: Efficient and
+Controllable Image Diffusion Generation via Skip Connection Editing](https://
+arxiv.org/abs/2312.11392) < [arXiv](https://arxiv.org/abs/2312.11392) \|
+[Project Page](https://scedit.github.io/) > | | ð¥NEFTune: [Noisy Embeddings
+Improve Instruction Finetuning](https://arxiv.org/abs/2310.05914) | | QA-LoRA:
+[Quantization-Aware Low-Rank Adaptation of Large Language Models](https://
+arxiv.org/abs/2309.14717) | | LongLoRA: [Efficient Fine-tuning of Long-Context
+Large Language Models](https://arxiv.org/abs/2309.12307) | | ROME: [Rank-One
+Editing of Encoder-Decoder Models](https://arxiv.org/abs/2211.13317) | |
+Adapter: [Parameter-Efficient Transfer Learning for NLP](http://arxiv.org/abs/
+1902.00751) | | Prompt Tuning: [Visual Prompt Tuning](https://arxiv.org/abs/
+2203.12119) | | Side: [Side-Tuning: A Baseline for Network Adaptation via
+Additive Side Networks](https://arxiv.org/abs/1912.13503) | | Res-Tuning: [Res-
+Tuning: A Flexible and Efficient Tuning Paradigm via Unbinding Tuner from
+Backbone](https://arxiv.org/abs/2310.19859) < [arXiv](https://arxiv.org/abs/
+2310.19859) \| [Project Page](https://res-tuning.github.io/) \| [Usage](docs/
+source/GetStarted/ResTuning.md) > | | Tuners provided by [PEFT](https://
+github.com/huggingface/peft), such as IA3, AdaLoRA, etc. | ### Supported
+Hardware | Hardware Environment | Notes | |--------------------------------|---
+----------------------------------------------| | CPU | | | RTX 20/30/40
+series, etc. | After 30 series, BF16 and FlashAttn can be used | | Computing
+cards T4/V100, etc. | BF16 and FlashAttn not supported | | Computing cards A10/
+A100, etc. | Support BF16 and FlashAttn | | Huawei Ascend NPU | | ## ð
+Documentation ### Documentation Compiling ```shell make docs # Check docs/
+build/html/index.html in web-browser ``` ### User Guide | Document Name | | ---
+--------------------------------------------------------- | | [Using Web-UI]
+(docs/source_en/GetStarted/Web-ui.md) | | [Using Tuners](docs/source_en/
+GetStarted/Tuners.md) | | [LLM Fine-tuning](docs/source_en/LLM/LLM-fine-
+tuning.md) | | [LLM Inference](docs/source_en/LLM/LLM-inference.md) | | [LLM
+Quantization](docs/source_en/LLM/LLM-quantization.md) | | [LLM Deployment]
 (docs/source_en/LLM/VLLM-inference-acceleration-and-deployment.md) | | [DPO
 Human Alignment Training](docs/source_en/LLM/RLHF.md) | | [AnimateDiff
 Training](docs/source_en/AIGC/AnimateDiff-train-infer.md) | ### Reference
 Documentation | Document Name | | ---------------------------------------------
 --------------- | | [Command Line Arguments](docs/source_en/LLM/Command-line-
 parameters.md) | | [Customizing New Models and Datasets](docs/source_en/LLM/
 Customization.md) | | [Supported Models and Datasets List](docs/source_en/LLM/
```

### Comparing `ms-swift-2.0.0/README.md` & `ms-swift-2.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -35,29 +35,31 @@
 SWIFT supports training, inference, evaluation and deployment of nearly **200 LLMs and MLLMs** (multimodal large models). Developers can directly apply our framework to their own research and production environments to realize the complete workflow from model training and evaluation to application. In addition to supporting the lightweight training solutions provided by [PEFT](https://github.com/huggingface/peft), we also provide a complete **Adapters library** to support the latest training techniques such as NEFTune, LoRA+, LLaMA-PRO, etc. This adapter library can be used directly in your own custom workflow without our training scripts.
 
 To facilitate use by users unfamiliar with deep learning, we provide a Gradio web-ui for controlling training and inference, as well as accompanying deep learning courses and best practices for beginners.
 
 Additionally, we are expanding capabilities for other modalities. Currently, we support full-parameter training and LoRA training for AnimateDiff.
 
 ## 🎉 News
+- 🔥2024.04.17: Support **CodeQwen1.5-7B** series: CodeQwen1.5-7B, CodeQwen1.5-7B-Chat,CodeQwen1.5-7B-Chat-AWQ, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/codeqwen1half_7b_chat/lora/sft.sh) to train.
+- 2024.04.16: Supports inference and fine-tuning of llava-v1.6-34b model. For best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/llava-best-practice.md).
 - 2024.04.13: Support the fine-tuning and inference of Mixtral-8x22B-v0.1 model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mixtral_moe_8x22b_v1/lora_ddp_ds/sft.sh) to start training!
 - 2024.04.13: Support the newly launched **MiniCPM** series: MiniCPM-V-2.0、MiniCPM-2B-128k、MiniCPM-MoE-8x2B and MiniCPM-1B.use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/minicpm_moe_8x2b/lora_ddp/sft.sh) to start training!
 - 🔥2024.04.11: Support Model Evaluation with MMLU/ARC/CEval datasets(also user custom eval datasets) with one command! Check [this documentation](docs/source_en/LLM/LLM-eval.md) for details. Meanwhile, we support a trick way to do multiple ablation experiments, check [this documentation](docs/source_en/LLM/LLM-exp.md) to use.
-- 🔥2024.04.11: Support **c4ai-command-r** series: c4ai-command-r-plus, c4ai-command-r-v01, [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/c4ai-command-r-plus/lora_mp/sft.sh) to train.
+- 🔥2024.04.11: Support **c4ai-command-r** series: c4ai-command-r-plus, c4ai-command-r-v01, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/c4ai_command_r_plus/lora_mp/sft.sh) to train.
 - 2024.04.10: Use SWIFT to fine-tune the qwen-7b-chat model to enhance its function call capabilities, and combine it with [Modelscope-Agent](https://github.com/modelscope/modelscope-agent) for best practices, which can be found [here](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Agent-best-practice.md#Usage-with-Modelscope_Agent).
 - 🔥2024.04.09: Support ruozhiba dataset. Search `ruozhiba` in [this documentation](docs/source_en/LLM/Supported-models-datasets.md) to begin training!
 - 2024.04.08: Support the fine-tuning and inference of XVERSE-MoE-A4.2B model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/xverse_moe_a4_2b/lora/sft.sh) to start training!
 - 2024.04.04: Support **QLoRA+FSDP** to train a 70B model with two 24G memory GPUs, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/llama2_70b_chat/qlora_fsdp/sft.sh) to train.
 - 🔥2024.04.03: Support **Qwen1.5-32B** series: Qwen1.5-32B, Qwen1.5-32B-Chat, Qwen1.5-32B-Chat-GPTQ-Int4.use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen1half_32b_chat/lora_mp/sft.sh) to start training!
 - 🔥2024.04.02: Support the fine-tuning and inference of Mengzi3-13B-Base model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mengzi3_13b_base/lora_ddp_ds/sft.sh) to start training!
 - 🔥2024.04.01: Support **dbrx** series: dbrx-base and dbrx-instruct, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/dbrx-instruct/lora_mp/sft.sh) to start training!
 - 🔥2024.03.29: Support **Qwen1.5-MoE** series: Qwen1.5-MoE-A2.7B, Qwen1.5-MoE-A2.7B-Chat, Qwen1.5-MoE-A2.7B-Chat-GPTQ-Int4.
 - 🔥2024.03.29: Support the fine-tuning and inference of **Grok-1** 300B MoE, please view details [here](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Grok-1-best-practice.md).
 - 🔥2024.03.25: Supports inference and fine-tuning of TeleChat-7b and TeleChat-12b model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/telechat_12b/lora/sft.sh) to start training!
-- 🔥2024.03.20: Supports inference and fine-tuning for the **llava** series. For best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source/Multi-Modal/llava最佳实践.md).
+- 🔥2024.03.20: Supports inference and fine-tuning for the **llava** series. For best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/llava-best-practice.md).
 - 🔥2024.03.12: Support inference and fine-tuning for **deepseek-vl** series. Best practices can be found [here](docs/source_en/Multi-Modal/deepseek-vl-best-practice.md).
 - 🔥2024.03.11: Support [GaLore](https://arxiv.org/abs/2403.03507) for effectively reducing memory usage to 1/2 of the original in full-parameter training.
 - 🔥2024.03.10: [End-to-end best practices](docs/source_en/LLM/Qwen1.5-best-practice.md) from fine-tuning to deployment for Qwen1.5-7B-Chat and Qwen1.5-72B-Chat.
 - 🔥2024.03.09: Support training and inference of MAMBA model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mamba-1.4b/lora/sft.sh) to start training!
 - 2024.03.09: Support training and inference of AQLM quantized model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/llama2_7b_aqlm_2bit_1x16/lora/sft.sh) to start training!
 - 2024.03.06: Support training and inference of AWQ quantized model, use [this Qwen1.5-AWQ model script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen1half_7b_chat_awq/lora/sft.sh) to start training, and support training and inference of [yi-9b](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_9b/lora_zero3).
 - 🔥2024.02.29: Support [LLaMA PRO](https://arxiv.org/pdf/2401.02415.pdf), simply use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_6b_chat/llamapro/sft.sh) to start training.
@@ -81,15 +83,16 @@
 - 🔥2024.01.26: Support [yi-vl-6b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/yi_vl_6b_chat), yi-vl-34b-chat.
 - 2024.01.24: Support codefuse-codegeex2-6b-chat, codefuse-qwen-14b-chat.
 - 2024.01.23: Support orion series: orion-14b, [orion-14b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/orion_14b_chat).
 - 2024.01.20: Support [xverse-13b-256k](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/xverse_13b_256k), xverse-65b-v2, xverse-65b-chat.
 - 🔥2024.01.17: Support internlm2 series: internlm2-7b-base, internlm2-7b, [internlm2-7b-sft-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/internlm2_7b_sft_chat), internlm2-7b-chat, internlm2-20b-base, internlm2-20b, internlm2-20b-sft-chat, internlm2-20b-chat.
 - 2024.01.15: Support yuan series: yuan2-2b-instruct, [yuan2-2b-janus-instruct](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/yuan2_2b_janus_instruct), yuan2-51b-instruct, yuan2-102b-instruct.
 - 🔥2024.01.12: Support **deepseek-moe** series: deepseek-moe-16b, [deepseek-moe-16b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/deepseek_moe_16b_chat).
-- 🔥2024.01.04: Support **VLLM deployment**, compatible with **OpenAI API** style, see [VLLM Inference Acceleration and Deployment](https://github.com/modelscope/swift/blob/main/docs/source/LLM/VLLM推理加速与部署.md#部署) for details.
+- 🔥2024.01.04: Support **VLLM deployment**, compatible with **OpenAI API** style, see [VLLM Inference Acceleration and Deployment](https://github.com/modelscope/swift/blob/main/docs/source_en/LLM/VLLM-inference-acceleration-and-deployment.md#Deployment) for details.
+
 - 2024.01.04: Update [Benchmark](https://github.com/modelscope/swift/blob/main/docs/source/LLM/Benchmark.md) for convenient viewing of training speed and memory usage of different models.
 - 🔥2023.12.29: Support web-ui for sft training and inference, use `swift web-ui` after installing ms-swift to start.
 - 🔥2023.12.29: Support DPO RLHF (Reinforcement Learning from Human Feedback) and three datasets for this task: AI-ModelScope/stack-exchange-paired, AI-ModelScope/hh-rlhf and AI-ModelScope/hh_rlhf_cn. See [documentation](https://github.com/modelscope/swift/blob/main/docs/source/LLM/LLM%E4%BA%BA%E7%B1%BB%E5%AF%B9%E9%BD%90%E8%AE%AD%E7%BB%83%E6%96%87%E6%A1%A3.md) to start training!
 - 🔥2023.12.28: Support SCEdit! This tuner can significantly reduce memory usage in U-Net and support low-memory controllable image generation (replacing ControlNet), read the section below to learn more.
 - 2023.12.23: Support [codegeex2-6b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/codegeex2_6b).
 - 2023.12.19: Support [phi2-3b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/phi2_3b).
 - 2023.12.18: Support VLLM for inference acceleration.
@@ -375,15 +378,15 @@
 
 ### Supported Models
 
 #### LLMs
 
 | Model Type                                     | Model Introduction                                                     | Language           | Model Size                             | Model Type                                 |
 |------------------------------------------------|------------------------------------------------------------------------|--------------------|----------------------------------------|------------------------------------------- |
-| Qwen<br>Qwen1.5                                   | [Tongyi Qwen 1.0 and 1.5 series models](https://github.com/QwenLM)  | Chinese<br>English    | 0.5B-72B<br>including quantized versions | base model<br>chat model<br>MoE model                      |
+| Qwen<br>Qwen1.5                                   | [Tongyi Qwen 1.0 and 1.5 series models](https://github.com/QwenLM)  | Chinese<br>English    | 0.5B-72B<br>including quantized versions | base model<br>chat model<br>MoE model<br>code model                      |
 | ChatGLM2<br>ChatGLM3<br>Codegeex2                    | [Zhipu ChatGLM series models](https://github.com/THUDM)               | Chinese<br>English    | 6B                                     | base model<br>chat model<br>code model  |
 | Baichuan/Baichuan2                             | [Baichuan 1 and Baichuan 2](https://github.com/baichuan-inc)           | Chinese<br>English    | 7B-13B<br>including quantized versions             | base model<br>chat model                       |
 | Yuan2                                          | [Langchao Yuan series models](https://github.com/IEIT-Yuan)             | Chinese<br>English    | 2B-102B                                | instruct model                                 |
 | XVerse                                         | [XVerse series models](https://github.com/xverse-ai)                    | Chinese<br>English    | 7B-65B                                 | base model<br>chat model<br>long text model<br>MoE model                |
 | LLaMA2                                         | [LLaMA2 series models](https://github.com/facebookresearch/llama)       | English            | 7B-70B<br>including quantized versions   | base model<br>chat model                       |
 | Mistral<br>Mixtral                            | [Mistral series models](https://github.com/mistralai/mistral-src)       | English            | 7B-22B     | base model<br>instruct model<br>MoE model                     |
 | YI                                             | [01AI's YI series models](https://github.com/01-ai)                     | Chinese<br>English    | 6B-34B                                 | base model<br>chat model<br>long text model            |
@@ -418,15 +421,16 @@
 | Qwen-VL          | [Tongyi Qwen vision model](https://github.com/QwenLM)               | Chinese<br>English    | 7B<br>including quantized versions | base model<br>chat model |
 | Qwen-Audio       | [Tongyi Qwen speech model](https://github.com/QwenLM)               | Chinese<br>English    | 7B                | base model<br>chat model |
 | YI-VL            | [01AI's YI series vision models](https://github.com/01-ai)             | Chinese<br>English    | 6B-34B            | chat model         |
 | XComposer2       | [Pujiang AI Lab InternLM vision model](https://github.com/InternLM/InternLM) | Chinese<br>English | 7B              | chat model         |
 | DeepSeek-VL      | [DeepSeek series vision models](https://github.com/deepseek-ai) | Chinese<br>English    | 1.3B-7B           | chat model         |
 | MiniCPM-V       | [OpenBmB MiniCPM vision model](https://github.com/OpenBMB/MiniCPM)     | Chinese<br>English    | 3B                | chat model         |
 | CogVLM<br>CogAgent  | [Zhipu ChatGLM visual QA and Agent model](https://github.com/THUDM/)   | English    | 17B-18B           | chat model         |
-| Llava      | [Llava series models](https://github.com/haotian-liu/LLaVA)                | English | 7B               | chat model |
+| Llava      | [Llava series models](https://github.com/haotian-liu/LLaVA)                | English | 7B-34B               | chat model |
+| mPLUG-Owl      | [mPLUG-Owl series models](https://github.com/X-PLUG/mPLUG-Owl)         | English | 11B               | chat model |
 
 #### Diffusion Models
 
 | Model Type          | Model Introduction                                                    | Language | Model Type        |
 |---------------------|----------------------------------------------------------------------|----------|------------------ |
 | AnimateDiff         | [AnimateDiff animation model](https://github.com/guoyww/AnimateDiff) | English  | text-to-video     |
 | SD1.5/SD2.0/SDXL    | [StabilityAI series diffusion models](https://github.com/Stability-AI) | English | text-to-image    |
```

#### html2text {}

```diff
@@ -22,34 +22,41 @@
 the latest training techniques such as NEFTune, LoRA+, LLaMA-PRO, etc. This
 adapter library can be used directly in your own custom workflow without our
 training scripts. To facilitate use by users unfamiliar with deep learning, we
 provide a Gradio web-ui for controlling training and inference, as well as
 accompanying deep learning courses and best practices for beginners.
 Additionally, we are expanding capabilities for other modalities. Currently, we
 support full-parameter training and LoRA training for AnimateDiff. ## ð News
-- 2024.04.13: Support the fine-tuning and inference of Mixtral-8x22B-v0.1
-model, use [this script](https://github.com/modelscope/swift/blob/main/
-examples/pytorch/llm/scripts/mixtral_moe_8x22b_v1/lora_ddp_ds/sft.sh) to start
-training! - 2024.04.13: Support the newly launched **MiniCPM** series: MiniCPM-
-V-2.0ãMiniCPM-2B-128kãMiniCPM-MoE-8x2B and MiniCPM-1B.use [this script]
-(https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
-minicpm_moe_8x2b/lora_ddp/sft.sh) to start training! - ð¥2024.04.11: Support
-Model Evaluation with MMLU/ARC/CEval datasets(also user custom eval datasets)
-with one command! Check [this documentation](docs/source_en/LLM/LLM-eval.md)
-for details. Meanwhile, we support a trick way to do multiple ablation
-experiments, check [this documentation](docs/source_en/LLM/LLM-exp.md) to use.
-- ð¥2024.04.11: Support **c4ai-command-r** series: c4ai-command-r-plus, c4ai-
-command-r-v01, [this script](https://github.com/modelscope/swift/blob/main/
-examples/pytorch/llm/scripts/c4ai-command-r-plus/lora_mp/sft.sh) to train. -
-2024.04.10: Use SWIFT to fine-tune the qwen-7b-chat model to enhance its
-function call capabilities, and combine it with [Modelscope-Agent](https://
-github.com/modelscope/modelscope-agent) for best practices, which can be found
-[here](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Agent-
-best-practice.md#Usage-with-Modelscope_Agent). - ð¥2024.04.09: Support
-ruozhiba dataset. Search `ruozhiba` in [this documentation](docs/source_en/LLM/
+- ð¥2024.04.17: Support **CodeQwen1.5-7B** series: CodeQwen1.5-7B,
+CodeQwen1.5-7B-Chat,CodeQwen1.5-7B-Chat-AWQ, use [this script](https://
+github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
+codeqwen1half_7b_chat/lora/sft.sh) to train. - 2024.04.16: Supports inference
+and fine-tuning of llava-v1.6-34b model. For best practice, you can refer to
+[here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-
+Modal/llava-best-practice.md). - 2024.04.13: Support the fine-tuning and
+inference of Mixtral-8x22B-v0.1 model, use [this script](https://github.com/
+modelscope/swift/blob/main/examples/pytorch/llm/scripts/mixtral_moe_8x22b_v1/
+lora_ddp_ds/sft.sh) to start training! - 2024.04.13: Support the newly launched
+**MiniCPM** series: MiniCPM-V-2.0ãMiniCPM-2B-128kãMiniCPM-MoE-8x2B and
+MiniCPM-1B.use [this script](https://github.com/modelscope/swift/blob/main/
+examples/pytorch/llm/scripts/minicpm_moe_8x2b/lora_ddp/sft.sh) to start
+training! - ð¥2024.04.11: Support Model Evaluation with MMLU/ARC/CEval
+datasets(also user custom eval datasets) with one command! Check [this
+documentation](docs/source_en/LLM/LLM-eval.md) for details. Meanwhile, we
+support a trick way to do multiple ablation experiments, check [this
+documentation](docs/source_en/LLM/LLM-exp.md) to use. - ð¥2024.04.11: Support
+**c4ai-command-r** series: c4ai-command-r-plus, c4ai-command-r-v01, use [this
+script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/
+scripts/c4ai_command_r_plus/lora_mp/sft.sh) to train. - 2024.04.10: Use SWIFT
+to fine-tune the qwen-7b-chat model to enhance its function call capabilities,
+and combine it with [Modelscope-Agent](https://github.com/modelscope/
+modelscope-agent) for best practices, which can be found [here](https://
+github.com/modelscope/swift/tree/main/docs/source_en/LLM/Agent-best-
+practice.md#Usage-with-Modelscope_Agent). - ð¥2024.04.09: Support ruozhiba
+dataset. Search `ruozhiba` in [this documentation](docs/source_en/LLM/
 Supported-models-datasets.md) to begin training! - 2024.04.08: Support the
 fine-tuning and inference of XVERSE-MoE-A4.2B model, use [this script](https://
 github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
 xverse_moe_a4_2b/lora/sft.sh) to start training! - 2024.04.04: Support
 **QLoRA+FSDP** to train a 70B model with two 24G memory GPUs, use [this script]
 (https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
 llama2_70b_chat/qlora_fsdp/sft.sh) to train. - ð¥2024.04.03: Support
@@ -67,16 +74,16 @@
 fine-tuning and inference of **Grok-1** 300B MoE, please view details [here]
 (https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Grok-1-best-
 practice.md). - ð¥2024.03.25: Supports inference and fine-tuning of TeleChat-
 7b and TeleChat-12b model, use [this script](https://github.com/modelscope/
 swift/blob/main/examples/pytorch/llm/scripts/telechat_12b/lora/sft.sh) to start
 training! - ð¥2024.03.20: Supports inference and fine-tuning for the
 **llava** series. For best practice, you can refer to [here](https://
-github.com/modelscope/swift/tree/main/docs/source/Multi-Modal/
-llavaæä½³å®è·µ.md). - ð¥2024.03.12: Support inference and fine-tuning for
+github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/llava-best-
+practice.md). - ð¥2024.03.12: Support inference and fine-tuning for
 **deepseek-vl** series. Best practices can be found [here](docs/source_en/
 Multi-Modal/deepseek-vl-best-practice.md). - ð¥2024.03.11: Support [GaLore]
 (https://arxiv.org/abs/2403.03507) for effectively reducing memory usage to 1/
 2 of the original in full-parameter training. - ð¥2024.03.10: [End-to-end
 best practices](docs/source_en/LLM/Qwen1.5-best-practice.md) from fine-tuning
 to deployment for Qwen1.5-7B-Chat and Qwen1.5-72B-Chat. - ð¥2024.03.09:
 Support training and inference of MAMBA model, use [this script](https://
@@ -148,23 +155,24 @@
 [yuan2-2b-janus-instruct](https://github.com/modelscope/swift/tree/main/
 examples/pytorch/llm/scripts/yuan2_2b_janus_instruct), yuan2-51b-instruct,
 yuan2-102b-instruct. - ð¥2024.01.12: Support **deepseek-moe** series:
 deepseek-moe-16b, [deepseek-moe-16b-chat](https://github.com/modelscope/swift/
 tree/main/examples/pytorch/llm/scripts/deepseek_moe_16b_chat). -
 ð¥2024.01.04: Support **VLLM deployment**, compatible with **OpenAI API**
 style, see [VLLM Inference Acceleration and Deployment](https://github.com/
-modelscope/swift/blob/main/docs/source/LLM/VLLMæ¨çå éä¸é¨ç½².md#é¨ç½²)
-for details. - 2024.01.04: Update [Benchmark](https://github.com/modelscope/
-swift/blob/main/docs/source/LLM/Benchmark.md) for convenient viewing of
-training speed and memory usage of different models. - ð¥2023.12.29: Support
-web-ui for sft training and inference, use `swift web-ui` after installing ms-
-swift to start. - ð¥2023.12.29: Support DPO RLHF (Reinforcement Learning from
-Human Feedback) and three datasets for this task: AI-ModelScope/stack-exchange-
-paired, AI-ModelScope/hh-rlhf and AI-ModelScope/hh_rlhf_cn. See [documentation]
-(https://github.com/modelscope/swift/blob/main/docs/source/LLM/
+modelscope/swift/blob/main/docs/source_en/LLM/VLLM-inference-acceleration-and-
+deployment.md#Deployment) for details. - 2024.01.04: Update [Benchmark](https:/
+/github.com/modelscope/swift/blob/main/docs/source/LLM/Benchmark.md) for
+convenient viewing of training speed and memory usage of different models. -
+ð¥2023.12.29: Support web-ui for sft training and inference, use `swift web-
+ui` after installing ms-swift to start. - ð¥2023.12.29: Support DPO RLHF
+(Reinforcement Learning from Human Feedback) and three datasets for this task:
+AI-ModelScope/stack-exchange-paired, AI-ModelScope/hh-rlhf and AI-ModelScope/
+hh_rlhf_cn. See [documentation](https://github.com/modelscope/swift/blob/main/
+docs/source/LLM/
 LLM%E4%BA%BA%E7%B1%BB%E5%AF%B9%E9%BD%90%E8%AE%AD%E7%BB%83%E6%96%87%E6%A1%A3.md)
 to start training! - ð¥2023.12.28: Support SCEdit! This tuner can
 significantly reduce memory usage in U-Net and support low-memory controllable
 image generation (replacing ControlNet), read the section below to learn more.
 - 2023.12.23: Support [codegeex2-6b](https://github.com/modelscope/swift/tree/
 main/examples/pytorch/llm/scripts/codegeex2_6b). - 2023.12.19: Support [phi2-
 3b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
@@ -353,15 +361,16 @@
 -------------|----------------------------------------|------------------------
 ------------------- | | Qwen
 Qwen1.5 | [Tongyi Qwen 1.0 and 1.5 series models](https://github.com/QwenLM) |
 Chinese
 English | 0.5B-72B
 including quantized versions | base model
 chat model
-MoE model | | ChatGLM2
+MoE model
+code model | | ChatGLM2
 ChatGLM3
 Codegeex2 | [Zhipu ChatGLM series models](https://github.com/THUDM) | Chinese
 English | 6B | base model
 chat model
 code model | | Baichuan/Baichuan2 | [Baichuan 1 and Baichuan 2](https://
 github.com/baichuan-inc) | Chinese
 English | 7B-13B
@@ -464,81 +473,83 @@
 English | 7B | chat model | | DeepSeek-VL | [DeepSeek series vision models]
 (https://github.com/deepseek-ai) | Chinese
 English | 1.3B-7B | chat model | | MiniCPM-V | [OpenBmB MiniCPM vision model]
 (https://github.com/OpenBMB/MiniCPM) | Chinese
 English | 3B | chat model | | CogVLM
 CogAgent | [Zhipu ChatGLM visual QA and Agent model](https://github.com/THUDM/
 ) | English | 17B-18B | chat model | | Llava | [Llava series models](https://
-github.com/haotian-liu/LLaVA) | English | 7B | chat model | #### Diffusion
-Models | Model Type | Model Introduction | Language | Model Type | |-----------
-----------|--------------------------------------------------------------------
---|----------|------------------ | | AnimateDiff | [AnimateDiff animation
-model](https://github.com/guoyww/AnimateDiff) | English | text-to-video | |
-SD1.5/SD2.0/SDXL | [StabilityAI series diffusion models](https://github.com/
-Stability-AI) | English | text-to-image | ### Supported Open Source Datasets |
-Dataset Type | Training Task | Documentation | |--------------|:---------------
-|--------------------------------------------------------------- | | General |
-Fine-tuning | ð¥ruozhiba, ð¥ms-bench, ð¥ms-bench-mini, ð¥alpaca-en
-(gpt4), ð¥alpaca-zh(gpt4), multi-alpaca-all, instinwild-en, instinwild-zh,
-cot-en, cot-zh, firefly-all-zh, instruct-en, gpt4all-en, sharegpt-en, sharegpt-
-zh, tulu-v2-sft-mixture, wikipedia-zh, open-orca, open-orca-gpt4, sharegpt-
-gpt4, ð¥sharegpt-gpt4-mini. | | Agent | Fine-tuning | ð¥ms-agent, ms-agent-
-for-agentfabric-default, ms-agent-for-agentfabric-addition, damo-mini-agent-zh,
-damo-agent-zh, agent-instruct-all-en. | | General | Human Alignment | ð¥hh-
-rlhf-cn, stack-exchange-paired, hh-rlhf-harmless-base, hh-rlhf-helpful-base,
-hh-rlhf-helpful-online, hh-rlhf-helpful-rejection-sampled, hh-rlhf-red-team-
-attempts, hh-rlhf-cn-harmless-base-cn, hh-rlhf-cn-helpful-base-cn, hh-rlhf-cn-
-harmless-base-en, hh-rlhf-cn-helpful-base-en. | | Code | Fine-tuning | code-
-alpaca-en, ð¥leetcode-python-en, ð¥codefuse-python-en, ð¥codefuse-evol-
-instruction-zh. | | Medical | Fine-tuning | medical-en, medical-zh, medical-
-mini-zh, ð¥disc-med-sft-zh. | | Legal | Fine-tuning | lawyer-llama-zh,
-tigerbot-law-zh, ð¥disc-law-sft-zh. | | Math | Fine-tuning | ð¥blossom-
-math-zh, school-math-zh, open-platypus-en. | | SQL | Fine-tuning | text2sql-en,
-ð¥sql-create-context-en. | | Text Generation | Fine-tuning | ð¥advertise-
-gen-zh, ð¥dureader-robust-zh. | | Classification | Fine-tuning | cmnli-zh,
-ð¥cmnli-mini-zh, ð¥jd-sentiment-zh, ð¥hc3-zh, ð¥hc3-en. | |
-Quantization Assist | Quantization | pileval. | | Other | Fine-tuning |
-finance-en, poetry-zh, webnovel-zh, generated-chat-zh, cls-fudan-news-zh, ner-
-jave-zh. | | Vision | Fine-tuning | coco-en, ð¥coco-mini-en, coco-mini-en-2,
-capcha-images. | | Audio | Fine-tuning | aishell1-zh, ð¥aishell1-mini-zh. |
-### Supported Technologies | Technology Name | |-------------------------------
--------------------------------- | | ð¥LoRA: [LORA: LOW-RANK ADAPTATION OF
-LARGE LANGUAGE MODELS](https://arxiv.org/abs/2106.09685) | | ð¥LoRA+: [LoRA+:
-Efficient Low Rank Adaptation of Large Models](https://arxiv.org/pdf/
-2402.12354.pdf) | | ð¥LLaMA PRO: [LLAMA PRO: Progressive LLaMA with Block
-Expansion](https://arxiv.org/pdf/2401.02415.pdf) | | ð¥SCEdit: [SCEdit:
-Efficient and Controllable Image Diffusion Generation via Skip Connection
-Editing](https://arxiv.org/abs/2312.11392) < [arXiv](https://arxiv.org/abs/
-2312.11392) \| [Project Page](https://scedit.github.io/) > | | ð¥NEFTune:
-[Noisy Embeddings Improve Instruction Finetuning](https://arxiv.org/abs/
-2310.05914) | | QA-LoRA:[Quantization-Aware Low-Rank Adaptation of Large
-Language Models](https://arxiv.org/abs/2309.14717) | | LongLoRA: [Efficient
-Fine-tuning of Long-Context Large Language Models](https://arxiv.org/abs/
-2309.12307) | | ROME: [Rank-One Editing of Encoder-Decoder Models](https://
-arxiv.org/abs/2211.13317) | | Adapter: [Parameter-Efficient Transfer Learning
-for NLP](http://arxiv.org/abs/1902.00751) | | Prompt Tuning: [Visual Prompt
-Tuning](https://arxiv.org/abs/2203.12119) | | Side: [Side-Tuning: A Baseline
-for Network Adaptation via Additive Side Networks](https://arxiv.org/abs/
-1912.13503) | | Res-Tuning: [Res-Tuning: A Flexible and Efficient Tuning
-Paradigm via Unbinding Tuner from Backbone](https://arxiv.org/abs/2310.19859) <
-[arXiv](https://arxiv.org/abs/2310.19859) \| [Project Page](https://res-
-tuning.github.io/) \| [Usage](docs/source/GetStarted/ResTuning.md) > | | Tuners
-provided by [PEFT](https://github.com/huggingface/peft), such as IA3, AdaLoRA,
-etc. | ### Supported Hardware | Hardware Environment | Notes | |---------------
------------------|-------------------------------------------------| | CPU | |
-| RTX 20/30/40 series, etc. | After 30 series, BF16 and FlashAttn can be used |
-| Computing cards T4/V100, etc. | BF16 and FlashAttn not supported | |
-Computing cards A10/A100, etc. | Support BF16 and FlashAttn | | Huawei Ascend
-NPU | | ## ð Documentation ### Documentation Compiling ```shell make docs #
-Check docs/build/html/index.html in web-browser ``` ### User Guide | Document
-Name | | ------------------------------------------------------------ | |
-[Using Web-UI](docs/source_en/GetStarted/Web-ui.md) | | [Using Tuners](docs/
-source_en/GetStarted/Tuners.md) | | [LLM Fine-tuning](docs/source_en/LLM/LLM-
-fine-tuning.md) | | [LLM Inference](docs/source_en/LLM/LLM-inference.md) | |
-[LLM Quantization](docs/source_en/LLM/LLM-quantization.md) | | [LLM Deployment]
+github.com/haotian-liu/LLaVA) | English | 7B-34B | chat model | | mPLUG-Owl |
+[mPLUG-Owl series models](https://github.com/X-PLUG/mPLUG-Owl) | English | 11B
+| chat model | #### Diffusion Models | Model Type | Model Introduction |
+Language | Model Type | |---------------------|--------------------------------
+--------------------------------------|----------|------------------ | |
+AnimateDiff | [AnimateDiff animation model](https://github.com/guoyww/
+AnimateDiff) | English | text-to-video | | SD1.5/SD2.0/SDXL | [StabilityAI
+series diffusion models](https://github.com/Stability-AI) | English | text-to-
+image | ### Supported Open Source Datasets | Dataset Type | Training Task |
+Documentation | |--------------|:---------------|------------------------------
+--------------------------------- | | General | Fine-tuning | ð¥ruozhiba,
+ð¥ms-bench, ð¥ms-bench-mini, ð¥alpaca-en(gpt4), ð¥alpaca-zh(gpt4),
+multi-alpaca-all, instinwild-en, instinwild-zh, cot-en, cot-zh, firefly-all-zh,
+instruct-en, gpt4all-en, sharegpt-en, sharegpt-zh, tulu-v2-sft-mixture,
+wikipedia-zh, open-orca, open-orca-gpt4, sharegpt-gpt4, ð¥sharegpt-gpt4-mini.
+| | Agent | Fine-tuning | ð¥ms-agent, ms-agent-for-agentfabric-default, ms-
+agent-for-agentfabric-addition, damo-mini-agent-zh, damo-agent-zh, agent-
+instruct-all-en. | | General | Human Alignment | ð¥hh-rlhf-cn, stack-
+exchange-paired, hh-rlhf-harmless-base, hh-rlhf-helpful-base, hh-rlhf-helpful-
+online, hh-rlhf-helpful-rejection-sampled, hh-rlhf-red-team-attempts, hh-rlhf-
+cn-harmless-base-cn, hh-rlhf-cn-helpful-base-cn, hh-rlhf-cn-harmless-base-en,
+hh-rlhf-cn-helpful-base-en. | | Code | Fine-tuning | code-alpaca-en,
+ð¥leetcode-python-en, ð¥codefuse-python-en, ð¥codefuse-evol-instruction-
+zh. | | Medical | Fine-tuning | medical-en, medical-zh, medical-mini-zh,
+ð¥disc-med-sft-zh. | | Legal | Fine-tuning | lawyer-llama-zh, tigerbot-law-
+zh, ð¥disc-law-sft-zh. | | Math | Fine-tuning | ð¥blossom-math-zh, school-
+math-zh, open-platypus-en. | | SQL | Fine-tuning | text2sql-en, ð¥sql-create-
+context-en. | | Text Generation | Fine-tuning | ð¥advertise-gen-zh,
+ð¥dureader-robust-zh. | | Classification | Fine-tuning | cmnli-zh, ð¥cmnli-
+mini-zh, ð¥jd-sentiment-zh, ð¥hc3-zh, ð¥hc3-en. | | Quantization Assist |
+Quantization | pileval. | | Other | Fine-tuning | finance-en, poetry-zh,
+webnovel-zh, generated-chat-zh, cls-fudan-news-zh, ner-jave-zh. | | Vision |
+Fine-tuning | coco-en, ð¥coco-mini-en, coco-mini-en-2, capcha-images. | |
+Audio | Fine-tuning | aishell1-zh, ð¥aishell1-mini-zh. | ### Supported
+Technologies | Technology Name | |---------------------------------------------
+------------------ | | ð¥LoRA: [LORA: LOW-RANK ADAPTATION OF LARGE LANGUAGE
+MODELS](https://arxiv.org/abs/2106.09685) | | ð¥LoRA+: [LoRA+: Efficient Low
+Rank Adaptation of Large Models](https://arxiv.org/pdf/2402.12354.pdf) | |
+ð¥LLaMA PRO: [LLAMA PRO: Progressive LLaMA with Block Expansion](https://
+arxiv.org/pdf/2401.02415.pdf) | | ð¥SCEdit: [SCEdit: Efficient and
+Controllable Image Diffusion Generation via Skip Connection Editing](https://
+arxiv.org/abs/2312.11392) < [arXiv](https://arxiv.org/abs/2312.11392) \|
+[Project Page](https://scedit.github.io/) > | | ð¥NEFTune: [Noisy Embeddings
+Improve Instruction Finetuning](https://arxiv.org/abs/2310.05914) | | QA-LoRA:
+[Quantization-Aware Low-Rank Adaptation of Large Language Models](https://
+arxiv.org/abs/2309.14717) | | LongLoRA: [Efficient Fine-tuning of Long-Context
+Large Language Models](https://arxiv.org/abs/2309.12307) | | ROME: [Rank-One
+Editing of Encoder-Decoder Models](https://arxiv.org/abs/2211.13317) | |
+Adapter: [Parameter-Efficient Transfer Learning for NLP](http://arxiv.org/abs/
+1902.00751) | | Prompt Tuning: [Visual Prompt Tuning](https://arxiv.org/abs/
+2203.12119) | | Side: [Side-Tuning: A Baseline for Network Adaptation via
+Additive Side Networks](https://arxiv.org/abs/1912.13503) | | Res-Tuning: [Res-
+Tuning: A Flexible and Efficient Tuning Paradigm via Unbinding Tuner from
+Backbone](https://arxiv.org/abs/2310.19859) < [arXiv](https://arxiv.org/abs/
+2310.19859) \| [Project Page](https://res-tuning.github.io/) \| [Usage](docs/
+source/GetStarted/ResTuning.md) > | | Tuners provided by [PEFT](https://
+github.com/huggingface/peft), such as IA3, AdaLoRA, etc. | ### Supported
+Hardware | Hardware Environment | Notes | |--------------------------------|---
+----------------------------------------------| | CPU | | | RTX 20/30/40
+series, etc. | After 30 series, BF16 and FlashAttn can be used | | Computing
+cards T4/V100, etc. | BF16 and FlashAttn not supported | | Computing cards A10/
+A100, etc. | Support BF16 and FlashAttn | | Huawei Ascend NPU | | ## ð
+Documentation ### Documentation Compiling ```shell make docs # Check docs/
+build/html/index.html in web-browser ``` ### User Guide | Document Name | | ---
+--------------------------------------------------------- | | [Using Web-UI]
+(docs/source_en/GetStarted/Web-ui.md) | | [Using Tuners](docs/source_en/
+GetStarted/Tuners.md) | | [LLM Fine-tuning](docs/source_en/LLM/LLM-fine-
+tuning.md) | | [LLM Inference](docs/source_en/LLM/LLM-inference.md) | | [LLM
+Quantization](docs/source_en/LLM/LLM-quantization.md) | | [LLM Deployment]
 (docs/source_en/LLM/VLLM-inference-acceleration-and-deployment.md) | | [DPO
 Human Alignment Training](docs/source_en/LLM/RLHF.md) | | [AnimateDiff
 Training](docs/source_en/AIGC/AnimateDiff-train-infer.md) | ### Reference
 Documentation | Document Name | | ---------------------------------------------
 --------------- | | [Command Line Arguments](docs/source_en/LLM/Command-line-
 parameters.md) | | [Customizing New Models and Datasets](docs/source_en/LLM/
 Customization.md) | | [Supported Models and Datasets List](docs/source_en/LLM/
```

### Comparing `ms-swift-2.0.0/ms_swift.egg-info/PKG-INFO` & `ms-swift-2.0.1/ms_swift.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-swift
-Version: 2.0.0
+Version: 2.0.1
 Summary: Swift: Scalable lightWeight Infrastructure for Fine-Tuning
 Home-page: https://github.com/modelscope/swift
 Author: DAMO ModelScope teams
 Author-email: contact@modelscope.cn
 License: Apache License 2.0
 Description: # SWIFT (Scalable lightWeight Infrastructure for Fine-Tuning)
         
@@ -43,29 +43,31 @@
         SWIFT supports training, inference, evaluation and deployment of nearly **200 LLMs and MLLMs** (multimodal large models). Developers can directly apply our framework to their own research and production environments to realize the complete workflow from model training and evaluation to application. In addition to supporting the lightweight training solutions provided by [PEFT](https://github.com/huggingface/peft), we also provide a complete **Adapters library** to support the latest training techniques such as NEFTune, LoRA+, LLaMA-PRO, etc. This adapter library can be used directly in your own custom workflow without our training scripts.
         
         To facilitate use by users unfamiliar with deep learning, we provide a Gradio web-ui for controlling training and inference, as well as accompanying deep learning courses and best practices for beginners.
         
         Additionally, we are expanding capabilities for other modalities. Currently, we support full-parameter training and LoRA training for AnimateDiff.
         
         ## 🎉 News
+        - 🔥2024.04.17: Support **CodeQwen1.5-7B** series: CodeQwen1.5-7B, CodeQwen1.5-7B-Chat,CodeQwen1.5-7B-Chat-AWQ, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/codeqwen1half_7b_chat/lora/sft.sh) to train.
+        - 2024.04.16: Supports inference and fine-tuning of llava-v1.6-34b model. For best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/llava-best-practice.md).
         - 2024.04.13: Support the fine-tuning and inference of Mixtral-8x22B-v0.1 model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mixtral_moe_8x22b_v1/lora_ddp_ds/sft.sh) to start training!
         - 2024.04.13: Support the newly launched **MiniCPM** series: MiniCPM-V-2.0、MiniCPM-2B-128k、MiniCPM-MoE-8x2B and MiniCPM-1B.use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/minicpm_moe_8x2b/lora_ddp/sft.sh) to start training!
         - 🔥2024.04.11: Support Model Evaluation with MMLU/ARC/CEval datasets(also user custom eval datasets) with one command! Check [this documentation](docs/source_en/LLM/LLM-eval.md) for details. Meanwhile, we support a trick way to do multiple ablation experiments, check [this documentation](docs/source_en/LLM/LLM-exp.md) to use.
-        - 🔥2024.04.11: Support **c4ai-command-r** series: c4ai-command-r-plus, c4ai-command-r-v01, [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/c4ai-command-r-plus/lora_mp/sft.sh) to train.
+        - 🔥2024.04.11: Support **c4ai-command-r** series: c4ai-command-r-plus, c4ai-command-r-v01, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/c4ai_command_r_plus/lora_mp/sft.sh) to train.
         - 2024.04.10: Use SWIFT to fine-tune the qwen-7b-chat model to enhance its function call capabilities, and combine it with [Modelscope-Agent](https://github.com/modelscope/modelscope-agent) for best practices, which can be found [here](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Agent-best-practice.md#Usage-with-Modelscope_Agent).
         - 🔥2024.04.09: Support ruozhiba dataset. Search `ruozhiba` in [this documentation](docs/source_en/LLM/Supported-models-datasets.md) to begin training!
         - 2024.04.08: Support the fine-tuning and inference of XVERSE-MoE-A4.2B model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/xverse_moe_a4_2b/lora/sft.sh) to start training!
         - 2024.04.04: Support **QLoRA+FSDP** to train a 70B model with two 24G memory GPUs, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/llama2_70b_chat/qlora_fsdp/sft.sh) to train.
         - 🔥2024.04.03: Support **Qwen1.5-32B** series: Qwen1.5-32B, Qwen1.5-32B-Chat, Qwen1.5-32B-Chat-GPTQ-Int4.use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen1half_32b_chat/lora_mp/sft.sh) to start training!
         - 🔥2024.04.02: Support the fine-tuning and inference of Mengzi3-13B-Base model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mengzi3_13b_base/lora_ddp_ds/sft.sh) to start training!
         - 🔥2024.04.01: Support **dbrx** series: dbrx-base and dbrx-instruct, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/dbrx-instruct/lora_mp/sft.sh) to start training!
         - 🔥2024.03.29: Support **Qwen1.5-MoE** series: Qwen1.5-MoE-A2.7B, Qwen1.5-MoE-A2.7B-Chat, Qwen1.5-MoE-A2.7B-Chat-GPTQ-Int4.
         - 🔥2024.03.29: Support the fine-tuning and inference of **Grok-1** 300B MoE, please view details [here](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Grok-1-best-practice.md).
         - 🔥2024.03.25: Supports inference and fine-tuning of TeleChat-7b and TeleChat-12b model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/telechat_12b/lora/sft.sh) to start training!
-        - 🔥2024.03.20: Supports inference and fine-tuning for the **llava** series. For best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source/Multi-Modal/llava最佳实践.md).
+        - 🔥2024.03.20: Supports inference and fine-tuning for the **llava** series. For best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/llava-best-practice.md).
         - 🔥2024.03.12: Support inference and fine-tuning for **deepseek-vl** series. Best practices can be found [here](docs/source_en/Multi-Modal/deepseek-vl-best-practice.md).
         - 🔥2024.03.11: Support [GaLore](https://arxiv.org/abs/2403.03507) for effectively reducing memory usage to 1/2 of the original in full-parameter training.
         - 🔥2024.03.10: [End-to-end best practices](docs/source_en/LLM/Qwen1.5-best-practice.md) from fine-tuning to deployment for Qwen1.5-7B-Chat and Qwen1.5-72B-Chat.
         - 🔥2024.03.09: Support training and inference of MAMBA model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mamba-1.4b/lora/sft.sh) to start training!
         - 2024.03.09: Support training and inference of AQLM quantized model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/llama2_7b_aqlm_2bit_1x16/lora/sft.sh) to start training!
         - 2024.03.06: Support training and inference of AWQ quantized model, use [this Qwen1.5-AWQ model script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen1half_7b_chat_awq/lora/sft.sh) to start training, and support training and inference of [yi-9b](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_9b/lora_zero3).
         - 🔥2024.02.29: Support [LLaMA PRO](https://arxiv.org/pdf/2401.02415.pdf), simply use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_6b_chat/llamapro/sft.sh) to start training.
@@ -89,15 +91,16 @@
         - 🔥2024.01.26: Support [yi-vl-6b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/yi_vl_6b_chat), yi-vl-34b-chat.
         - 2024.01.24: Support codefuse-codegeex2-6b-chat, codefuse-qwen-14b-chat.
         - 2024.01.23: Support orion series: orion-14b, [orion-14b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/orion_14b_chat).
         - 2024.01.20: Support [xverse-13b-256k](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/xverse_13b_256k), xverse-65b-v2, xverse-65b-chat.
         - 🔥2024.01.17: Support internlm2 series: internlm2-7b-base, internlm2-7b, [internlm2-7b-sft-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/internlm2_7b_sft_chat), internlm2-7b-chat, internlm2-20b-base, internlm2-20b, internlm2-20b-sft-chat, internlm2-20b-chat.
         - 2024.01.15: Support yuan series: yuan2-2b-instruct, [yuan2-2b-janus-instruct](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/yuan2_2b_janus_instruct), yuan2-51b-instruct, yuan2-102b-instruct.
         - 🔥2024.01.12: Support **deepseek-moe** series: deepseek-moe-16b, [deepseek-moe-16b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/deepseek_moe_16b_chat).
-        - 🔥2024.01.04: Support **VLLM deployment**, compatible with **OpenAI API** style, see [VLLM Inference Acceleration and Deployment](https://github.com/modelscope/swift/blob/main/docs/source/LLM/VLLM推理加速与部署.md#部署) for details.
+        - 🔥2024.01.04: Support **VLLM deployment**, compatible with **OpenAI API** style, see [VLLM Inference Acceleration and Deployment](https://github.com/modelscope/swift/blob/main/docs/source_en/LLM/VLLM-inference-acceleration-and-deployment.md#Deployment) for details.
+        
         - 2024.01.04: Update [Benchmark](https://github.com/modelscope/swift/blob/main/docs/source/LLM/Benchmark.md) for convenient viewing of training speed and memory usage of different models.
         - 🔥2023.12.29: Support web-ui for sft training and inference, use `swift web-ui` after installing ms-swift to start.
         - 🔥2023.12.29: Support DPO RLHF (Reinforcement Learning from Human Feedback) and three datasets for this task: AI-ModelScope/stack-exchange-paired, AI-ModelScope/hh-rlhf and AI-ModelScope/hh_rlhf_cn. See [documentation](https://github.com/modelscope/swift/blob/main/docs/source/LLM/LLM%E4%BA%BA%E7%B1%BB%E5%AF%B9%E9%BD%90%E8%AE%AD%E7%BB%83%E6%96%87%E6%A1%A3.md) to start training!
         - 🔥2023.12.28: Support SCEdit! This tuner can significantly reduce memory usage in U-Net and support low-memory controllable image generation (replacing ControlNet), read the section below to learn more.
         - 2023.12.23: Support [codegeex2-6b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/codegeex2_6b).
         - 2023.12.19: Support [phi2-3b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/phi2_3b).
         - 2023.12.18: Support VLLM for inference acceleration.
@@ -383,15 +386,15 @@
         
         ### Supported Models
         
         #### LLMs
         
         | Model Type                                     | Model Introduction                                                     | Language           | Model Size                             | Model Type                                 |
         |------------------------------------------------|------------------------------------------------------------------------|--------------------|----------------------------------------|------------------------------------------- |
-        | Qwen<br>Qwen1.5                                   | [Tongyi Qwen 1.0 and 1.5 series models](https://github.com/QwenLM)  | Chinese<br>English    | 0.5B-72B<br>including quantized versions | base model<br>chat model<br>MoE model                      |
+        | Qwen<br>Qwen1.5                                   | [Tongyi Qwen 1.0 and 1.5 series models](https://github.com/QwenLM)  | Chinese<br>English    | 0.5B-72B<br>including quantized versions | base model<br>chat model<br>MoE model<br>code model                      |
         | ChatGLM2<br>ChatGLM3<br>Codegeex2                    | [Zhipu ChatGLM series models](https://github.com/THUDM)               | Chinese<br>English    | 6B                                     | base model<br>chat model<br>code model  |
         | Baichuan/Baichuan2                             | [Baichuan 1 and Baichuan 2](https://github.com/baichuan-inc)           | Chinese<br>English    | 7B-13B<br>including quantized versions             | base model<br>chat model                       |
         | Yuan2                                          | [Langchao Yuan series models](https://github.com/IEIT-Yuan)             | Chinese<br>English    | 2B-102B                                | instruct model                                 |
         | XVerse                                         | [XVerse series models](https://github.com/xverse-ai)                    | Chinese<br>English    | 7B-65B                                 | base model<br>chat model<br>long text model<br>MoE model                |
         | LLaMA2                                         | [LLaMA2 series models](https://github.com/facebookresearch/llama)       | English            | 7B-70B<br>including quantized versions   | base model<br>chat model                       |
         | Mistral<br>Mixtral                            | [Mistral series models](https://github.com/mistralai/mistral-src)       | English            | 7B-22B     | base model<br>instruct model<br>MoE model                     |
         | YI                                             | [01AI's YI series models](https://github.com/01-ai)                     | Chinese<br>English    | 6B-34B                                 | base model<br>chat model<br>long text model            |
@@ -426,15 +429,16 @@
         | Qwen-VL          | [Tongyi Qwen vision model](https://github.com/QwenLM)               | Chinese<br>English    | 7B<br>including quantized versions | base model<br>chat model |
         | Qwen-Audio       | [Tongyi Qwen speech model](https://github.com/QwenLM)               | Chinese<br>English    | 7B                | base model<br>chat model |
         | YI-VL            | [01AI's YI series vision models](https://github.com/01-ai)             | Chinese<br>English    | 6B-34B            | chat model         |
         | XComposer2       | [Pujiang AI Lab InternLM vision model](https://github.com/InternLM/InternLM) | Chinese<br>English | 7B              | chat model         |
         | DeepSeek-VL      | [DeepSeek series vision models](https://github.com/deepseek-ai) | Chinese<br>English    | 1.3B-7B           | chat model         |
         | MiniCPM-V       | [OpenBmB MiniCPM vision model](https://github.com/OpenBMB/MiniCPM)     | Chinese<br>English    | 3B                | chat model         |
         | CogVLM<br>CogAgent  | [Zhipu ChatGLM visual QA and Agent model](https://github.com/THUDM/)   | English    | 17B-18B           | chat model         |
-        | Llava      | [Llava series models](https://github.com/haotian-liu/LLaVA)                | English | 7B               | chat model |
+        | Llava      | [Llava series models](https://github.com/haotian-liu/LLaVA)                | English | 7B-34B               | chat model |
+        | mPLUG-Owl      | [mPLUG-Owl series models](https://github.com/X-PLUG/mPLUG-Owl)         | English | 11B               | chat model |
         
         #### Diffusion Models
         
         | Model Type          | Model Introduction                                                    | Language | Model Type        |
         |---------------------|----------------------------------------------------------------------|----------|------------------ |
         | AnimateDiff         | [AnimateDiff animation model](https://github.com/guoyww/AnimateDiff) | English  | text-to-video     |
         | SD1.5/SD2.0/SDXL    | [StabilityAI series diffusion models](https://github.com/Stability-AI) | English | text-to-image    |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ms-swift Version: 2.0.0 Summary: Swift: Scalable
+Metadata-Version: 2.1 Name: ms-swift Version: 2.0.1 Summary: Swift: Scalable
 lightWeight Infrastructure for Fine-Tuning Home-page: https://github.com/
 modelscope/swift Author: DAMO ModelScope teams Author-email:
 contact@modelscope.cn License: Apache License 2.0 Description: # SWIFT
 (Scalable lightWeight Infrastructure for Fine-Tuning)
 
                             [resources/banner.png]
                          _M_o_d_e_l_S_c_o_p_e_ _C_o_m_m_u_n_i_t_y_ _W_e_b_s_i_t_e
@@ -26,34 +26,41 @@
 the latest training techniques such as NEFTune, LoRA+, LLaMA-PRO, etc. This
 adapter library can be used directly in your own custom workflow without our
 training scripts. To facilitate use by users unfamiliar with deep learning, we
 provide a Gradio web-ui for controlling training and inference, as well as
 accompanying deep learning courses and best practices for beginners.
 Additionally, we are expanding capabilities for other modalities. Currently, we
 support full-parameter training and LoRA training for AnimateDiff. ## ð News
-- 2024.04.13: Support the fine-tuning and inference of Mixtral-8x22B-v0.1
-model, use [this script](https://github.com/modelscope/swift/blob/main/
-examples/pytorch/llm/scripts/mixtral_moe_8x22b_v1/lora_ddp_ds/sft.sh) to start
-training! - 2024.04.13: Support the newly launched **MiniCPM** series: MiniCPM-
-V-2.0ãMiniCPM-2B-128kãMiniCPM-MoE-8x2B and MiniCPM-1B.use [this script]
-(https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
-minicpm_moe_8x2b/lora_ddp/sft.sh) to start training! - ð¥2024.04.11: Support
-Model Evaluation with MMLU/ARC/CEval datasets(also user custom eval datasets)
-with one command! Check [this documentation](docs/source_en/LLM/LLM-eval.md)
-for details. Meanwhile, we support a trick way to do multiple ablation
-experiments, check [this documentation](docs/source_en/LLM/LLM-exp.md) to use.
-- ð¥2024.04.11: Support **c4ai-command-r** series: c4ai-command-r-plus, c4ai-
-command-r-v01, [this script](https://github.com/modelscope/swift/blob/main/
-examples/pytorch/llm/scripts/c4ai-command-r-plus/lora_mp/sft.sh) to train. -
-2024.04.10: Use SWIFT to fine-tune the qwen-7b-chat model to enhance its
-function call capabilities, and combine it with [Modelscope-Agent](https://
-github.com/modelscope/modelscope-agent) for best practices, which can be found
-[here](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Agent-
-best-practice.md#Usage-with-Modelscope_Agent). - ð¥2024.04.09: Support
-ruozhiba dataset. Search `ruozhiba` in [this documentation](docs/source_en/LLM/
+- ð¥2024.04.17: Support **CodeQwen1.5-7B** series: CodeQwen1.5-7B,
+CodeQwen1.5-7B-Chat,CodeQwen1.5-7B-Chat-AWQ, use [this script](https://
+github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
+codeqwen1half_7b_chat/lora/sft.sh) to train. - 2024.04.16: Supports inference
+and fine-tuning of llava-v1.6-34b model. For best practice, you can refer to
+[here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-
+Modal/llava-best-practice.md). - 2024.04.13: Support the fine-tuning and
+inference of Mixtral-8x22B-v0.1 model, use [this script](https://github.com/
+modelscope/swift/blob/main/examples/pytorch/llm/scripts/mixtral_moe_8x22b_v1/
+lora_ddp_ds/sft.sh) to start training! - 2024.04.13: Support the newly launched
+**MiniCPM** series: MiniCPM-V-2.0ãMiniCPM-2B-128kãMiniCPM-MoE-8x2B and
+MiniCPM-1B.use [this script](https://github.com/modelscope/swift/blob/main/
+examples/pytorch/llm/scripts/minicpm_moe_8x2b/lora_ddp/sft.sh) to start
+training! - ð¥2024.04.11: Support Model Evaluation with MMLU/ARC/CEval
+datasets(also user custom eval datasets) with one command! Check [this
+documentation](docs/source_en/LLM/LLM-eval.md) for details. Meanwhile, we
+support a trick way to do multiple ablation experiments, check [this
+documentation](docs/source_en/LLM/LLM-exp.md) to use. - ð¥2024.04.11: Support
+**c4ai-command-r** series: c4ai-command-r-plus, c4ai-command-r-v01, use [this
+script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/
+scripts/c4ai_command_r_plus/lora_mp/sft.sh) to train. - 2024.04.10: Use SWIFT
+to fine-tune the qwen-7b-chat model to enhance its function call capabilities,
+and combine it with [Modelscope-Agent](https://github.com/modelscope/
+modelscope-agent) for best practices, which can be found [here](https://
+github.com/modelscope/swift/tree/main/docs/source_en/LLM/Agent-best-
+practice.md#Usage-with-Modelscope_Agent). - ð¥2024.04.09: Support ruozhiba
+dataset. Search `ruozhiba` in [this documentation](docs/source_en/LLM/
 Supported-models-datasets.md) to begin training! - 2024.04.08: Support the
 fine-tuning and inference of XVERSE-MoE-A4.2B model, use [this script](https://
 github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
 xverse_moe_a4_2b/lora/sft.sh) to start training! - 2024.04.04: Support
 **QLoRA+FSDP** to train a 70B model with two 24G memory GPUs, use [this script]
 (https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
 llama2_70b_chat/qlora_fsdp/sft.sh) to train. - ð¥2024.04.03: Support
@@ -71,16 +78,16 @@
 fine-tuning and inference of **Grok-1** 300B MoE, please view details [here]
 (https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Grok-1-best-
 practice.md). - ð¥2024.03.25: Supports inference and fine-tuning of TeleChat-
 7b and TeleChat-12b model, use [this script](https://github.com/modelscope/
 swift/blob/main/examples/pytorch/llm/scripts/telechat_12b/lora/sft.sh) to start
 training! - ð¥2024.03.20: Supports inference and fine-tuning for the
 **llava** series. For best practice, you can refer to [here](https://
-github.com/modelscope/swift/tree/main/docs/source/Multi-Modal/
-llavaæä½³å®è·µ.md). - ð¥2024.03.12: Support inference and fine-tuning for
+github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/llava-best-
+practice.md). - ð¥2024.03.12: Support inference and fine-tuning for
 **deepseek-vl** series. Best practices can be found [here](docs/source_en/
 Multi-Modal/deepseek-vl-best-practice.md). - ð¥2024.03.11: Support [GaLore]
 (https://arxiv.org/abs/2403.03507) for effectively reducing memory usage to 1/
 2 of the original in full-parameter training. - ð¥2024.03.10: [End-to-end
 best practices](docs/source_en/LLM/Qwen1.5-best-practice.md) from fine-tuning
 to deployment for Qwen1.5-7B-Chat and Qwen1.5-72B-Chat. - ð¥2024.03.09:
 Support training and inference of MAMBA model, use [this script](https://
@@ -152,23 +159,24 @@
 [yuan2-2b-janus-instruct](https://github.com/modelscope/swift/tree/main/
 examples/pytorch/llm/scripts/yuan2_2b_janus_instruct), yuan2-51b-instruct,
 yuan2-102b-instruct. - ð¥2024.01.12: Support **deepseek-moe** series:
 deepseek-moe-16b, [deepseek-moe-16b-chat](https://github.com/modelscope/swift/
 tree/main/examples/pytorch/llm/scripts/deepseek_moe_16b_chat). -
 ð¥2024.01.04: Support **VLLM deployment**, compatible with **OpenAI API**
 style, see [VLLM Inference Acceleration and Deployment](https://github.com/
-modelscope/swift/blob/main/docs/source/LLM/VLLMæ¨çå éä¸é¨ç½².md#é¨ç½²)
-for details. - 2024.01.04: Update [Benchmark](https://github.com/modelscope/
-swift/blob/main/docs/source/LLM/Benchmark.md) for convenient viewing of
-training speed and memory usage of different models. - ð¥2023.12.29: Support
-web-ui for sft training and inference, use `swift web-ui` after installing ms-
-swift to start. - ð¥2023.12.29: Support DPO RLHF (Reinforcement Learning from
-Human Feedback) and three datasets for this task: AI-ModelScope/stack-exchange-
-paired, AI-ModelScope/hh-rlhf and AI-ModelScope/hh_rlhf_cn. See [documentation]
-(https://github.com/modelscope/swift/blob/main/docs/source/LLM/
+modelscope/swift/blob/main/docs/source_en/LLM/VLLM-inference-acceleration-and-
+deployment.md#Deployment) for details. - 2024.01.04: Update [Benchmark](https:/
+/github.com/modelscope/swift/blob/main/docs/source/LLM/Benchmark.md) for
+convenient viewing of training speed and memory usage of different models. -
+ð¥2023.12.29: Support web-ui for sft training and inference, use `swift web-
+ui` after installing ms-swift to start. - ð¥2023.12.29: Support DPO RLHF
+(Reinforcement Learning from Human Feedback) and three datasets for this task:
+AI-ModelScope/stack-exchange-paired, AI-ModelScope/hh-rlhf and AI-ModelScope/
+hh_rlhf_cn. See [documentation](https://github.com/modelscope/swift/blob/main/
+docs/source/LLM/
 LLM%E4%BA%BA%E7%B1%BB%E5%AF%B9%E9%BD%90%E8%AE%AD%E7%BB%83%E6%96%87%E6%A1%A3.md)
 to start training! - ð¥2023.12.28: Support SCEdit! This tuner can
 significantly reduce memory usage in U-Net and support low-memory controllable
 image generation (replacing ControlNet), read the section below to learn more.
 - 2023.12.23: Support [codegeex2-6b](https://github.com/modelscope/swift/tree/
 main/examples/pytorch/llm/scripts/codegeex2_6b). - 2023.12.19: Support [phi2-
 3b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
@@ -357,15 +365,16 @@
 -------------|----------------------------------------|------------------------
 ------------------- | | Qwen
 Qwen1.5 | [Tongyi Qwen 1.0 and 1.5 series models](https://github.com/QwenLM) |
 Chinese
 English | 0.5B-72B
 including quantized versions | base model
 chat model
-MoE model | | ChatGLM2
+MoE model
+code model | | ChatGLM2
 ChatGLM3
 Codegeex2 | [Zhipu ChatGLM series models](https://github.com/THUDM) | Chinese
 English | 6B | base model
 chat model
 code model | | Baichuan/Baichuan2 | [Baichuan 1 and Baichuan 2](https://
 github.com/baichuan-inc) | Chinese
 English | 7B-13B
@@ -468,81 +477,83 @@
 English | 7B | chat model | | DeepSeek-VL | [DeepSeek series vision models]
 (https://github.com/deepseek-ai) | Chinese
 English | 1.3B-7B | chat model | | MiniCPM-V | [OpenBmB MiniCPM vision model]
 (https://github.com/OpenBMB/MiniCPM) | Chinese
 English | 3B | chat model | | CogVLM
 CogAgent | [Zhipu ChatGLM visual QA and Agent model](https://github.com/THUDM/
 ) | English | 17B-18B | chat model | | Llava | [Llava series models](https://
-github.com/haotian-liu/LLaVA) | English | 7B | chat model | #### Diffusion
-Models | Model Type | Model Introduction | Language | Model Type | |-----------
-----------|--------------------------------------------------------------------
---|----------|------------------ | | AnimateDiff | [AnimateDiff animation
-model](https://github.com/guoyww/AnimateDiff) | English | text-to-video | |
-SD1.5/SD2.0/SDXL | [StabilityAI series diffusion models](https://github.com/
-Stability-AI) | English | text-to-image | ### Supported Open Source Datasets |
-Dataset Type | Training Task | Documentation | |--------------|:---------------
-|--------------------------------------------------------------- | | General |
-Fine-tuning | ð¥ruozhiba, ð¥ms-bench, ð¥ms-bench-mini, ð¥alpaca-en
-(gpt4), ð¥alpaca-zh(gpt4), multi-alpaca-all, instinwild-en, instinwild-zh,
-cot-en, cot-zh, firefly-all-zh, instruct-en, gpt4all-en, sharegpt-en, sharegpt-
-zh, tulu-v2-sft-mixture, wikipedia-zh, open-orca, open-orca-gpt4, sharegpt-
-gpt4, ð¥sharegpt-gpt4-mini. | | Agent | Fine-tuning | ð¥ms-agent, ms-agent-
-for-agentfabric-default, ms-agent-for-agentfabric-addition, damo-mini-agent-zh,
-damo-agent-zh, agent-instruct-all-en. | | General | Human Alignment | ð¥hh-
-rlhf-cn, stack-exchange-paired, hh-rlhf-harmless-base, hh-rlhf-helpful-base,
-hh-rlhf-helpful-online, hh-rlhf-helpful-rejection-sampled, hh-rlhf-red-team-
-attempts, hh-rlhf-cn-harmless-base-cn, hh-rlhf-cn-helpful-base-cn, hh-rlhf-cn-
-harmless-base-en, hh-rlhf-cn-helpful-base-en. | | Code | Fine-tuning | code-
-alpaca-en, ð¥leetcode-python-en, ð¥codefuse-python-en, ð¥codefuse-evol-
-instruction-zh. | | Medical | Fine-tuning | medical-en, medical-zh, medical-
-mini-zh, ð¥disc-med-sft-zh. | | Legal | Fine-tuning | lawyer-llama-zh,
-tigerbot-law-zh, ð¥disc-law-sft-zh. | | Math | Fine-tuning | ð¥blossom-
-math-zh, school-math-zh, open-platypus-en. | | SQL | Fine-tuning | text2sql-en,
-ð¥sql-create-context-en. | | Text Generation | Fine-tuning | ð¥advertise-
-gen-zh, ð¥dureader-robust-zh. | | Classification | Fine-tuning | cmnli-zh,
-ð¥cmnli-mini-zh, ð¥jd-sentiment-zh, ð¥hc3-zh, ð¥hc3-en. | |
-Quantization Assist | Quantization | pileval. | | Other | Fine-tuning |
-finance-en, poetry-zh, webnovel-zh, generated-chat-zh, cls-fudan-news-zh, ner-
-jave-zh. | | Vision | Fine-tuning | coco-en, ð¥coco-mini-en, coco-mini-en-2,
-capcha-images. | | Audio | Fine-tuning | aishell1-zh, ð¥aishell1-mini-zh. |
-### Supported Technologies | Technology Name | |-------------------------------
--------------------------------- | | ð¥LoRA: [LORA: LOW-RANK ADAPTATION OF
-LARGE LANGUAGE MODELS](https://arxiv.org/abs/2106.09685) | | ð¥LoRA+: [LoRA+:
-Efficient Low Rank Adaptation of Large Models](https://arxiv.org/pdf/
-2402.12354.pdf) | | ð¥LLaMA PRO: [LLAMA PRO: Progressive LLaMA with Block
-Expansion](https://arxiv.org/pdf/2401.02415.pdf) | | ð¥SCEdit: [SCEdit:
-Efficient and Controllable Image Diffusion Generation via Skip Connection
-Editing](https://arxiv.org/abs/2312.11392) < [arXiv](https://arxiv.org/abs/
-2312.11392) \| [Project Page](https://scedit.github.io/) > | | ð¥NEFTune:
-[Noisy Embeddings Improve Instruction Finetuning](https://arxiv.org/abs/
-2310.05914) | | QA-LoRA:[Quantization-Aware Low-Rank Adaptation of Large
-Language Models](https://arxiv.org/abs/2309.14717) | | LongLoRA: [Efficient
-Fine-tuning of Long-Context Large Language Models](https://arxiv.org/abs/
-2309.12307) | | ROME: [Rank-One Editing of Encoder-Decoder Models](https://
-arxiv.org/abs/2211.13317) | | Adapter: [Parameter-Efficient Transfer Learning
-for NLP](http://arxiv.org/abs/1902.00751) | | Prompt Tuning: [Visual Prompt
-Tuning](https://arxiv.org/abs/2203.12119) | | Side: [Side-Tuning: A Baseline
-for Network Adaptation via Additive Side Networks](https://arxiv.org/abs/
-1912.13503) | | Res-Tuning: [Res-Tuning: A Flexible and Efficient Tuning
-Paradigm via Unbinding Tuner from Backbone](https://arxiv.org/abs/2310.19859) <
-[arXiv](https://arxiv.org/abs/2310.19859) \| [Project Page](https://res-
-tuning.github.io/) \| [Usage](docs/source/GetStarted/ResTuning.md) > | | Tuners
-provided by [PEFT](https://github.com/huggingface/peft), such as IA3, AdaLoRA,
-etc. | ### Supported Hardware | Hardware Environment | Notes | |---------------
------------------|-------------------------------------------------| | CPU | |
-| RTX 20/30/40 series, etc. | After 30 series, BF16 and FlashAttn can be used |
-| Computing cards T4/V100, etc. | BF16 and FlashAttn not supported | |
-Computing cards A10/A100, etc. | Support BF16 and FlashAttn | | Huawei Ascend
-NPU | | ## ð Documentation ### Documentation Compiling ```shell make docs #
-Check docs/build/html/index.html in web-browser ``` ### User Guide | Document
-Name | | ------------------------------------------------------------ | |
-[Using Web-UI](docs/source_en/GetStarted/Web-ui.md) | | [Using Tuners](docs/
-source_en/GetStarted/Tuners.md) | | [LLM Fine-tuning](docs/source_en/LLM/LLM-
-fine-tuning.md) | | [LLM Inference](docs/source_en/LLM/LLM-inference.md) | |
-[LLM Quantization](docs/source_en/LLM/LLM-quantization.md) | | [LLM Deployment]
+github.com/haotian-liu/LLaVA) | English | 7B-34B | chat model | | mPLUG-Owl |
+[mPLUG-Owl series models](https://github.com/X-PLUG/mPLUG-Owl) | English | 11B
+| chat model | #### Diffusion Models | Model Type | Model Introduction |
+Language | Model Type | |---------------------|--------------------------------
+--------------------------------------|----------|------------------ | |
+AnimateDiff | [AnimateDiff animation model](https://github.com/guoyww/
+AnimateDiff) | English | text-to-video | | SD1.5/SD2.0/SDXL | [StabilityAI
+series diffusion models](https://github.com/Stability-AI) | English | text-to-
+image | ### Supported Open Source Datasets | Dataset Type | Training Task |
+Documentation | |--------------|:---------------|------------------------------
+--------------------------------- | | General | Fine-tuning | ð¥ruozhiba,
+ð¥ms-bench, ð¥ms-bench-mini, ð¥alpaca-en(gpt4), ð¥alpaca-zh(gpt4),
+multi-alpaca-all, instinwild-en, instinwild-zh, cot-en, cot-zh, firefly-all-zh,
+instruct-en, gpt4all-en, sharegpt-en, sharegpt-zh, tulu-v2-sft-mixture,
+wikipedia-zh, open-orca, open-orca-gpt4, sharegpt-gpt4, ð¥sharegpt-gpt4-mini.
+| | Agent | Fine-tuning | ð¥ms-agent, ms-agent-for-agentfabric-default, ms-
+agent-for-agentfabric-addition, damo-mini-agent-zh, damo-agent-zh, agent-
+instruct-all-en. | | General | Human Alignment | ð¥hh-rlhf-cn, stack-
+exchange-paired, hh-rlhf-harmless-base, hh-rlhf-helpful-base, hh-rlhf-helpful-
+online, hh-rlhf-helpful-rejection-sampled, hh-rlhf-red-team-attempts, hh-rlhf-
+cn-harmless-base-cn, hh-rlhf-cn-helpful-base-cn, hh-rlhf-cn-harmless-base-en,
+hh-rlhf-cn-helpful-base-en. | | Code | Fine-tuning | code-alpaca-en,
+ð¥leetcode-python-en, ð¥codefuse-python-en, ð¥codefuse-evol-instruction-
+zh. | | Medical | Fine-tuning | medical-en, medical-zh, medical-mini-zh,
+ð¥disc-med-sft-zh. | | Legal | Fine-tuning | lawyer-llama-zh, tigerbot-law-
+zh, ð¥disc-law-sft-zh. | | Math | Fine-tuning | ð¥blossom-math-zh, school-
+math-zh, open-platypus-en. | | SQL | Fine-tuning | text2sql-en, ð¥sql-create-
+context-en. | | Text Generation | Fine-tuning | ð¥advertise-gen-zh,
+ð¥dureader-robust-zh. | | Classification | Fine-tuning | cmnli-zh, ð¥cmnli-
+mini-zh, ð¥jd-sentiment-zh, ð¥hc3-zh, ð¥hc3-en. | | Quantization Assist |
+Quantization | pileval. | | Other | Fine-tuning | finance-en, poetry-zh,
+webnovel-zh, generated-chat-zh, cls-fudan-news-zh, ner-jave-zh. | | Vision |
+Fine-tuning | coco-en, ð¥coco-mini-en, coco-mini-en-2, capcha-images. | |
+Audio | Fine-tuning | aishell1-zh, ð¥aishell1-mini-zh. | ### Supported
+Technologies | Technology Name | |---------------------------------------------
+------------------ | | ð¥LoRA: [LORA: LOW-RANK ADAPTATION OF LARGE LANGUAGE
+MODELS](https://arxiv.org/abs/2106.09685) | | ð¥LoRA+: [LoRA+: Efficient Low
+Rank Adaptation of Large Models](https://arxiv.org/pdf/2402.12354.pdf) | |
+ð¥LLaMA PRO: [LLAMA PRO: Progressive LLaMA with Block Expansion](https://
+arxiv.org/pdf/2401.02415.pdf) | | ð¥SCEdit: [SCEdit: Efficient and
+Controllable Image Diffusion Generation via Skip Connection Editing](https://
+arxiv.org/abs/2312.11392) < [arXiv](https://arxiv.org/abs/2312.11392) \|
+[Project Page](https://scedit.github.io/) > | | ð¥NEFTune: [Noisy Embeddings
+Improve Instruction Finetuning](https://arxiv.org/abs/2310.05914) | | QA-LoRA:
+[Quantization-Aware Low-Rank Adaptation of Large Language Models](https://
+arxiv.org/abs/2309.14717) | | LongLoRA: [Efficient Fine-tuning of Long-Context
+Large Language Models](https://arxiv.org/abs/2309.12307) | | ROME: [Rank-One
+Editing of Encoder-Decoder Models](https://arxiv.org/abs/2211.13317) | |
+Adapter: [Parameter-Efficient Transfer Learning for NLP](http://arxiv.org/abs/
+1902.00751) | | Prompt Tuning: [Visual Prompt Tuning](https://arxiv.org/abs/
+2203.12119) | | Side: [Side-Tuning: A Baseline for Network Adaptation via
+Additive Side Networks](https://arxiv.org/abs/1912.13503) | | Res-Tuning: [Res-
+Tuning: A Flexible and Efficient Tuning Paradigm via Unbinding Tuner from
+Backbone](https://arxiv.org/abs/2310.19859) < [arXiv](https://arxiv.org/abs/
+2310.19859) \| [Project Page](https://res-tuning.github.io/) \| [Usage](docs/
+source/GetStarted/ResTuning.md) > | | Tuners provided by [PEFT](https://
+github.com/huggingface/peft), such as IA3, AdaLoRA, etc. | ### Supported
+Hardware | Hardware Environment | Notes | |--------------------------------|---
+----------------------------------------------| | CPU | | | RTX 20/30/40
+series, etc. | After 30 series, BF16 and FlashAttn can be used | | Computing
+cards T4/V100, etc. | BF16 and FlashAttn not supported | | Computing cards A10/
+A100, etc. | Support BF16 and FlashAttn | | Huawei Ascend NPU | | ## ð
+Documentation ### Documentation Compiling ```shell make docs # Check docs/
+build/html/index.html in web-browser ``` ### User Guide | Document Name | | ---
+--------------------------------------------------------- | | [Using Web-UI]
+(docs/source_en/GetStarted/Web-ui.md) | | [Using Tuners](docs/source_en/
+GetStarted/Tuners.md) | | [LLM Fine-tuning](docs/source_en/LLM/LLM-fine-
+tuning.md) | | [LLM Inference](docs/source_en/LLM/LLM-inference.md) | | [LLM
+Quantization](docs/source_en/LLM/LLM-quantization.md) | | [LLM Deployment]
 (docs/source_en/LLM/VLLM-inference-acceleration-and-deployment.md) | | [DPO
 Human Alignment Training](docs/source_en/LLM/RLHF.md) | | [AnimateDiff
 Training](docs/source_en/AIGC/AnimateDiff-train-infer.md) | ### Reference
 Documentation | Document Name | | ---------------------------------------------
 --------------- | | [Command Line Arguments](docs/source_en/LLM/Command-line-
 parameters.md) | | [Customizing New Models and Datasets](docs/source_en/LLM/
 Customization.md) | | [Supported Models and Datasets List](docs/source_en/LLM/
```

### Comparing `ms-swift-2.0.0/ms_swift.egg-info/SOURCES.txt` & `ms-swift-2.0.1/ms_swift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/ms_swift.egg-info/requires.txt` & `ms-swift-2.0.1/ms_swift.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/setup.cfg` & `ms-swift-2.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/setup.py` & `ms-swift-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/__init__.py` & `ms-swift-2.0.1/swift/__init__.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/aigc/__init__.py` & `ms-swift-2.0.1/swift/aigc/__init__.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/aigc/animatediff.py` & `ms-swift-2.0.1/swift/aigc/animatediff.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/aigc/animatediff_infer.py` & `ms-swift-2.0.1/swift/aigc/animatediff_infer.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/aigc/diffusers/__init__.py` & `ms-swift-2.0.1/swift/aigc/diffusers/__init__.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/aigc/diffusers/infer_controlnet.py` & `ms-swift-2.0.1/swift/aigc/diffusers/infer_controlnet.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/aigc/diffusers/infer_controlnet_sdxl.py` & `ms-swift-2.0.1/swift/aigc/diffusers/infer_controlnet_sdxl.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/aigc/diffusers/infer_dreambooth.py` & `ms-swift-2.0.1/swift/aigc/diffusers/infer_dreambooth.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/aigc/diffusers/infer_dreambooth_lora.py` & `ms-swift-2.0.1/swift/aigc/diffusers/infer_dreambooth_lora.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/aigc/diffusers/infer_dreambooth_lora_sdxl.py` & `ms-swift-2.0.1/swift/aigc/diffusers/infer_dreambooth_lora_sdxl.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/aigc/diffusers/infer_text_to_image.py` & `ms-swift-2.0.1/swift/aigc/diffusers/infer_text_to_image.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/aigc/diffusers/infer_text_to_image_lora.py` & `ms-swift-2.0.1/swift/aigc/diffusers/infer_text_to_image_lora.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/aigc/diffusers/infer_text_to_image_lora_sdxl.py` & `ms-swift-2.0.1/swift/aigc/diffusers/infer_text_to_image_lora_sdxl.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/aigc/diffusers/infer_text_to_image_sdxl.py` & `ms-swift-2.0.1/swift/aigc/diffusers/infer_text_to_image_sdxl.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/aigc/diffusers/train_controlnet.py` & `ms-swift-2.0.1/swift/aigc/diffusers/train_controlnet.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/aigc/diffusers/train_controlnet_sdxl.py` & `ms-swift-2.0.1/swift/aigc/diffusers/train_controlnet_sdxl.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/aigc/diffusers/train_dreambooth.py` & `ms-swift-2.0.1/swift/aigc/diffusers/train_dreambooth.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/aigc/diffusers/train_dreambooth_lora.py` & `ms-swift-2.0.1/swift/aigc/diffusers/train_dreambooth_lora.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/aigc/diffusers/train_dreambooth_lora_sdxl.py` & `ms-swift-2.0.1/swift/aigc/diffusers/train_dreambooth_lora_sdxl.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/aigc/diffusers/train_text_to_image.py` & `ms-swift-2.0.1/swift/aigc/diffusers/train_text_to_image.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/aigc/diffusers/train_text_to_image_lora.py` & `ms-swift-2.0.1/swift/aigc/diffusers/train_text_to_image_lora.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/aigc/diffusers/train_text_to_image_lora_sdxl.py` & `ms-swift-2.0.1/swift/aigc/diffusers/train_text_to_image_lora_sdxl.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/aigc/diffusers/train_text_to_image_sdxl.py` & `ms-swift-2.0.1/swift/aigc/diffusers/train_text_to_image_sdxl.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/aigc/utils/argument.py` & `ms-swift-2.0.1/swift/aigc/utils/argument.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/cli/main.py` & `ms-swift-2.0.1/swift/cli/main.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/hub/api.py` & `ms-swift-2.0.1/swift/hub/api.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/hub/check_model.py` & `ms-swift-2.0.1/swift/hub/check_model.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/hub/constants.py` & `ms-swift-2.0.1/swift/hub/constants.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/hub/errors.py` & `ms-swift-2.0.1/swift/hub/errors.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/hub/file_download.py` & `ms-swift-2.0.1/swift/hub/file_download.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/hub/git.py` & `ms-swift-2.0.1/swift/hub/git.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/hub/push_to_hub.py` & `ms-swift-2.0.1/swift/hub/push_to_hub.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/hub/repository.py` & `ms-swift-2.0.1/swift/hub/repository.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/hub/snapshot_download.py` & `ms-swift-2.0.1/swift/hub/snapshot_download.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/hub/utils/caching.py` & `ms-swift-2.0.1/swift/hub/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/hub/utils/utils.py` & `ms-swift-2.0.1/swift/hub/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/llm/__init__.py` & `ms-swift-2.0.1/swift/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/llm/accelerator.py` & `ms-swift-2.0.1/swift/llm/accelerator.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/llm/agent/utils.py` & `ms-swift-2.0.1/swift/llm/agent/utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/llm/app_ui.py` & `ms-swift-2.0.1/swift/llm/app_ui.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/llm/data/self_cognition.jsonl` & `ms-swift-2.0.1/swift/llm/data/self_cognition.jsonl`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/llm/deploy.py` & `ms-swift-2.0.1/swift/llm/deploy.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/llm/dpo.py` & `ms-swift-2.0.1/swift/llm/dpo.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 from transformers import IntervalStrategy
 from transformers.integrations import is_deepspeed_zero3_enabled
 
 from swift.trainers.dpo_trainers import DPOTrainer
 from swift.utils import (check_json_format, get_dist_setting, get_logger,
                          get_main, get_model_info, is_ddp_plus_mp, is_dist,
                          is_master, plot_images, seed_everything, show_layers)
-from . import get_time_info
 from .tuner import prepare_model
 from .utils import (DPOArguments, Template, get_dataset, get_model_tokenizer,
-                    get_template, set_generation_config)
+                    get_template, get_time_info, set_generation_config)
 
 logger = get_logger()
 
 
 def llm_dpo(args: DPOArguments) -> str:
     logger.info(f'args: {args}')
     training_args = args.training_args
```

### Comparing `ms-swift-2.0.0/swift/llm/ds_config/zero2.json` & `ms-swift-2.0.1/swift/llm/ds_config/zero2.json`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/llm/ds_config/zero3.json` & `ms-swift-2.0.1/swift/llm/ds_config/zero3.json`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/llm/eval.py` & `ms-swift-2.0.1/swift/llm/eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
                     _ds['dataset'],
                     subset_list=_ds.get('subset_list'))
     eval_model = EvalModel(args, model_name, config=record or {})
 
     task_configs = TaskConfig.load(
         custom_model=eval_model, tasks=args.eval_dataset + custom_names)
     for task_config in task_configs:
-        task_config.use_cache = False
+        task_config.use_cache = args.eval_use_cache
         if args.eval_limit:
             task_config.limit = args.eval_limit
         if args.eval_few_shot is not None:
             for dataset in task_config.datasets:
                 if not task_config.dataset_args.get(dataset):
                     task_config.dataset_args[dataset] = {}
                 task_config.dataset_args[dataset][
```

### Comparing `ms-swift-2.0.0/swift/llm/export.py` & `ms-swift-2.0.1/swift/llm/export.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) Alibaba, Inc. and its affiliates.
 import os
 from typing import List, Tuple, Union
 
 import torch
 from datasets import concatenate_datasets
 from modelscope import GenerationConfig
-from transformers import AwqConfig, PreTrainedModel
+from transformers import PreTrainedModel
 
 from swift.utils import (get_logger, get_main, get_model_info, push_to_ms_hub,
                          seed_everything, show_layers)
 from .infer import merge_lora, prepare_model_template, save_checkpoint
 from .utils import (ExportArguments, Template, get_dataset,
                     get_model_tokenizer, get_template, set_generation_config,
                     swift_to_peft_format)
@@ -114,14 +114,15 @@
                 'attention_mask': attention_mask
             })
         return res
 
 
 def awq_model_quantize(awq_model, tokenizer) -> None:
     from awq.quantize import quantizer
+    from transformers import AwqConfig
     assert _args is not None
     logger.info(f'Quantization dataset: {_args.dataset}')
     _origin_get_calib_dataset = quantizer.get_calib_dataset
     quantizer.get_calib_dataset = _get_dataset
     group_size = 128
     quant_config = {
         'zero_point': True,
@@ -140,15 +141,15 @@
 
 
 def gptq_model_quantize(model, tokenizer):
     from optimum.gptq import GPTQQuantizer, quantizer
     global _args
     logger.info(f'Quantization dataset: {_args.dataset}')
     gptq_quantizer = GPTQQuantizer(
-        bits=_args.quant_bits, dataset=_args.dataset)
+        bits=_args.quant_bits, dataset=','.join(_args.dataset))
     _origin_get_dataset = quantizer.get_dataset
     quantizer.get_dataset = _get_dataset
     logger.info('Start quantizing the model...')
     logger.warning(
         'The process of packing the model takes a long time and there is no progress bar. '
         'Please be patient and wait...')
     gptq_quantizer.quantize_model(model, tokenizer)
```

### Comparing `ms-swift-2.0.0/swift/llm/infer.py` & `ms-swift-2.0.1/swift/llm/infer.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                     target_dir: str,
                     *,
                     save_safetensors: bool = True) -> None:
     if model is not None:
         model.save_pretrained(target_dir, safe_serialization=save_safetensors)
     tokenizer.save_pretrained(target_dir)
     model_type = getattr(tokenizer, 'model_type')
-    fname_list = ['generation_config.json']
+    fname_list = ['generation_config.json', 'preprocessor_config.json']
     if model_type is not None:
         fname_list += get_additional_saved_files(model_type)
 
     for fname in fname_list:
         tgt_path = os.path.join(target_dir, fname)
         for model_dir in [ckpt_dir, model_cache_dir]:
             if model_dir is None:
@@ -103,18 +103,21 @@
             'skipping the saving process. '
             'you can pass `replace_if_exists=True` to overwrite it.')
         return
 
     model_kwargs = {}
     if is_torch_npu_available():
         logger.info(f'device_count: {torch.npu.device_count()}')
-        device_map = 'npu:0'
+        if device_map is None:
+            device_map = 'npu:0'
     else:
         logger.info(f'device_count: {torch.cuda.device_count()}')
-        device_map = 'auto'
+        if device_map is None:
+            device_map = 'auto'
+    if device_map == 'auto':
         model_kwargs['low_cpu_mem_usage'] = True
     model_kwargs['device_map'] = device_map
 
     # Loading Model and Tokenizer
     model_id_or_path = None
     if args.model_id_or_path is not None:
         model_id_or_path = args.model_id_or_path
@@ -146,18 +149,21 @@
         device_map: Optional[str] = None) -> Tuple[PreTrainedModel, Template]:
 
     seed_everything(args.seed)
 
     model_kwargs = {}
     if is_torch_npu_available():
         logger.info(f'device_count: {torch.npu.device_count()}')
-        device_map = 'npu:0'
+        if device_map is None:
+            device_map = 'npu:0'
     else:
         logger.info(f'device_count: {torch.cuda.device_count()}')
-        device_map = 'auto'
+        if device_map is None:
+            device_map = 'auto'
+    if device_map == 'auto':
         model_kwargs['low_cpu_mem_usage'] = True
     model_kwargs['device_map'] = device_map
 
     # Loading Model and Tokenizer
     if args.load_in_8bit or args.load_in_4bit:
         quantization_config = BitsAndBytesConfig(
             args.load_in_8bit,
```

### Comparing `ms-swift-2.0.0/swift/llm/rome.py` & `ms-swift-2.0.1/swift/llm/rome.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/llm/sft.py` & `ms-swift-2.0.1/swift/llm/sft.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/llm/tuner.py` & `ms-swift-2.0.1/swift/llm/tuner.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,34 +73,32 @@
                 'lora_dropout': args.lora_dropout_p,
                 'bias': args.lora_bias_trainable,
                 'modules_to_save': args.lora_modules_to_save,
                 'use_rslora': args.use_rslora,
                 'use_dora': args.use_dora,
                 'lorap_lr_ratio': args.lora_lr_ratio,
             }
-            if args.sft_type == 'lora':
+            if args.sft_type in ('lora', 'longlora'):
                 if args.tuner_backend == 'swift':
                     lora_config = LoRAConfig(
                         lora_dtype=args.lora_dtype, **lora_kwargs)
                 elif args.tuner_backend == 'peft':
                     lora_config = LoraConfig(
                         task_type='CAUSAL_LM',
                         lora_dtype=args.lora_dtype,
                         **lora_kwargs)
                 model = Swift.prepare_model(model, lora_config)
                 logger.info(f'lora_config: {lora_config}')
-            elif args.sft_type == 'longlora':
-                assert args.tuner_backend == 'swift'
-                assert LongLoRAModelType.LLAMA in args.model_type
-                longlora_config = LongLoRAConfig(
-                    lora_dtype=args.lora_dtype,
-                    model_type=LongLoRAModelType.LLAMA,
-                    **lora_kwargs)
-                model = Swift.prepare_model(model, longlora_config)
-                logger.info(f'longlora_config: {longlora_config}')
+                if args.sft_type == 'longlora':
+                    assert LongLoRAModelType.LLAMA in args.model_type
+                    assert version.parse(
+                        transformers.__version__) >= version.parse('4.39.3')
+                    from swift.tuners.longlora.llama import replace_llama_attn
+                    replace_llama_attn(model)
+                    model.config.group_size_ratio = 0.25
             elif args.sft_type == 'adalora':
                 lora_kwargs.pop('lorap_lr_ratio', None)
                 lora_kwargs['rank_pattern'] = None
                 adalora_config = AdaLoraConfig(
                     task_type='CAUSAL_LM',
                     **lora_kwargs,
                     target_r=args.adalora_target_r,
```

### Comparing `ms-swift-2.0.0/swift/llm/utils/__init__.py` & `ms-swift-2.0.1/swift/llm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/llm/utils/argument.py` & `ms-swift-2.0.1/swift/llm/utils/argument.py`

 * *Files 0% similar despite different names*

```diff
@@ -787,14 +787,16 @@
 
     eval_few_shot: Optional[int] = None
 
     eval_limit: Optional[int] = None
 
     custom_eval_config: Optional[str] = None
 
+    eval_use_cache: Optional[bool] = False
+
 
 @dataclass
 class ExportArguments(InferArguments):
     to_peft_format: bool = False
     # The parameter has been defined in InferArguments.
     # merge_lora: bool = False
```

### Comparing `ms-swift-2.0.0/swift/llm/utils/client_utils.py` & `ms-swift-2.0.1/swift/llm/utils/client_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/llm/utils/dataset.py` & `ms-swift-2.0.1/swift/llm/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/llm/utils/model.py` & `ms-swift-2.0.1/swift/llm/utils/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,23 +59,25 @@
     qwen1half_0_5b = 'qwen1half-0_5b'
     qwen1half_1_8b = 'qwen1half-1_8b'
     qwen1half_4b = 'qwen1half-4b'
     qwen1half_7b = 'qwen1half-7b'
     qwen1half_14b = 'qwen1half-14b'
     qwen1half_32b = 'qwen1half-32b'
     qwen1half_72b = 'qwen1half-72b'
+    codeqwen1half_7b = 'codeqwen1half-7b'
     qwen1half_moe_a2_7b = 'qwen1half-moe-a2_7b'
     qwen1half_0_5b_chat = 'qwen1half-0_5b-chat'
     qwen1half_1_8b_chat = 'qwen1half-1_8b-chat'
     qwen1half_4b_chat = 'qwen1half-4b-chat'
     qwen1half_7b_chat = 'qwen1half-7b-chat'
     qwen1half_14b_chat = 'qwen1half-14b-chat'
     qwen1half_32b_chat = 'qwen1half-32b-chat'
     qwen1half_72b_chat = 'qwen1half-72b-chat'
     qwen1half_moe_a2_7b_chat = 'qwen1half-moe-a2_7b-chat'
+    codeqwen1half_7b_chat = 'codeqwen1half-7b-chat'
 
     # qwen1.5 gptq
     qwen1half_0_5b_chat_int4 = 'qwen1half-0_5b-chat-int4'
     qwen1half_1_8b_chat_int4 = 'qwen1half-1_8b-chat-int4'
     qwen1half_4b_chat_int4 = 'qwen1half-4b-chat-int4'
     qwen1half_7b_chat_int4 = 'qwen1half-7b-chat-int4'
     qwen1half_14b_chat_int4 = 'qwen1half-14b-chat-int4'
@@ -91,15 +93,17 @@
 
     # qwen1.5 awq
     qwen1half_0_5b_chat_awq = 'qwen1half-0_5b-chat-awq'
     qwen1half_1_8b_chat_awq = 'qwen1half-1_8b-chat-awq'
     qwen1half_4b_chat_awq = 'qwen1half-4b-chat-awq'
     qwen1half_7b_chat_awq = 'qwen1half-7b-chat-awq'
     qwen1half_14b_chat_awq = 'qwen1half-14b-chat-awq'
+    qwen1half_32b_chat_awq = 'qwen1half-32b-chat-awq'
     qwen1half_72b_chat_awq = 'qwen1half-72b-chat-awq'
+    codeqwen1half_7b_chat_awq = 'codeqwen1half-7b-chat-awq'
 
     # qwen-vl
     qwen_vl = 'qwen-vl'
     qwen_vl_chat = 'qwen-vl-chat'
     qwen_vl_chat_int4 = 'qwen-vl-chat-int4'
     # qwen-audio
     qwen_audio = 'qwen-audio'
@@ -117,19 +121,21 @@
     llama2_13b = 'llama2-13b'
     llama2_13b_chat = 'llama2-13b-chat'
     llama2_70b = 'llama2-70b'
     llama2_70b_chat = 'llama2-70b-chat'
     llama2_7b_aqlm_2bit_1x16 = 'llama2-7b-aqlm-2bit-1x16'  # aqlm
     # llava
     llava1d6_mistral_7b_instruct = 'llava1d6-mistral-7b-instruct'
+    llava1d6_yi_34b_instruct = 'llava1d6-yi-34b-instruct'
     # yi
     yi_6b = 'yi-6b'
     yi_6b_200k = 'yi-6b-200k'
     yi_6b_chat = 'yi-6b-chat'
     yi_9b = 'yi-9b'
+    yi_9b_200k = 'yi-9b-200k'
     yi_34b = 'yi-34b'
     yi_34b_200k = 'yi-34b-200k'
     yi_34b_chat = 'yi-34b-chat'
     # yi-vl
     yi_vl_6b_chat = 'yi-vl-6b-chat'
     yi_vl_34b_chat = 'yi-vl-34b-chat'
     # internlm
@@ -216,14 +222,17 @@
     # baichuan2
     baichuan2_7b = 'baichuan2-7b'
     baichuan2_7b_chat = 'baichuan2-7b-chat'
     baichuan2_7b_chat_int4 = 'baichuan2-7b-chat-int4'
     baichuan2_13b = 'baichuan2-13b'
     baichuan2_13b_chat = 'baichuan2-13b-chat'
     baichuan2_13b_chat_int4 = 'baichuan2-13b-chat-int4'
+    # owl
+    mplug_owl2_chat = 'mplug-owl2-chat'  # llama
+    mplug_owl2d1_chat = 'mplug-owl2d1-chat'  # qwen
     # yuan
     yuan2_2b_instruct = 'yuan2-2b-instruct'
     yuan2_2b_janus_instruct = 'yuan2-2b-janus-instruct'
     yuan2_51b_instruct = 'yuan2-51b-instruct'
     yuan2_102b_instruct = 'yuan2-102b-instruct'
     # xverse
     xverse_7b = 'xverse-7b'
@@ -321,14 +330,25 @@
     ]
     phi = ['Wqkv']
     internlm2 = ['wqkv']
     mamba = ['in_proj', 'x_proj', 'embeddings', 'out_proj']
     telechat = ['key_value', 'query']
     grok_1 = ['q_proj', 'k_proj', 'v_proj']
     dbrx = ['attn.Wqkv']
+    mplug_owl2 = [
+        'q_proj',
+        'k_proj.multiway.0',
+        'k_proj.multiway.1',
+        'v_proj.multiway.0',
+        'v_proj.multiway.1',
+    ]
+    mplug_owl2d1 = [
+        'c_attn.multiway.0',
+        'c_attn.multiway.1',
+    ]
 
 
 GetModelTokenizerFunction = Callable[..., Tuple[Optional[PreTrainedModel],
                                                 PreTrainedTokenizerBase]]
 
 
 def register_model(
@@ -1035,14 +1055,22 @@
     'qwen/Qwen1.5-72B',
     LoRATM.qwen1half,
     TemplateType.default_generation,
     support_flash_attn=True,
     support_vllm=True,
     requires=['transformers>=4.37'])
 @register_model(
+    ModelType.codeqwen1half_7b,
+    'qwen/CodeQwen1.5-7B',
+    LoRATM.qwen1half,
+    TemplateType.default_generation,
+    support_flash_attn=True,
+    support_vllm=True,
+    requires=['transformers>=4.37'])
+@register_model(
     ModelType.qwen1half_moe_a2_7b,
     'qwen/Qwen1.5-MoE-A2.7B',
     LoRATM.qwen1half,
     TemplateType.default_generation,
     support_flash_attn=True,
     support_vllm=True,
     requires=['transformers>=4.37'])
@@ -1196,14 +1224,21 @@
     ModelType.yi_9b,
     '01ai/Yi-9B',
     LoRATM.llama2,
     TemplateType.default_generation,
     support_flash_attn=True,
     support_vllm=True)
 @register_model(
+    ModelType.yi_9b_200k,
+    '01ai/Yi-9B-200K',
+    LoRATM.llama2,
+    TemplateType.default_generation,
+    support_flash_attn=True,
+    support_vllm=True)
+@register_model(
     ModelType.yi_6b,
     '01ai/Yi-6B',
     LoRATM.llama2,
     TemplateType.default_generation,
     support_flash_attn=True,
     support_vllm=True)
 @register_model(
@@ -1434,23 +1469,41 @@
     LoRATM.qwen1half,
     TemplateType.qwen,
     support_flash_attn=True,
     support_vllm=True,
     function_kwargs={'is_awq': True},
     requires=['transformers>=4.37', 'autoawq'])
 @register_model(
+    ModelType.qwen1half_32b_chat_awq,
+    'qwen/Qwen1.5-32B-Chat-AWQ',
+    LoRATM.qwen1half,
+    TemplateType.qwen,
+    support_flash_attn=True,
+    support_vllm=True,
+    function_kwargs={'is_awq': True},
+    requires=['transformers>=4.37', 'autoawq'])
+@register_model(
     ModelType.qwen1half_72b_chat_awq,
     'qwen/Qwen1.5-72B-Chat-AWQ',
     LoRATM.qwen1half,
     TemplateType.qwen,
     support_flash_attn=True,
     support_vllm=True,
     function_kwargs={'is_awq': True},
     requires=['transformers>=4.37', 'autoawq'])
 @register_model(
+    ModelType.codeqwen1half_7b_chat_awq,
+    'qwen/CodeQwen1.5-7B-Chat-AWQ',
+    LoRATM.qwen1half,
+    TemplateType.qwen,
+    support_flash_attn=True,
+    support_vllm=True,
+    function_kwargs={'is_awq': True},
+    requires=['transformers>=4.37', 'autoawq'])
+@register_model(
     ModelType.qwen1half_0_5b_chat,
     'qwen/Qwen1.5-0.5B-Chat',
     LoRATM.qwen1half,
     TemplateType.qwen,
     support_flash_attn=True,
     support_vllm=True,
     requires=['transformers>=4.37'])
@@ -1506,14 +1559,22 @@
     ModelType.qwen1half_moe_a2_7b_chat,
     'qwen/Qwen1.5-MoE-A2.7B-Chat',
     LoRATM.qwen1half,
     TemplateType.qwen,
     support_flash_attn=True,
     support_vllm=True,
     requires=['transformers>=4.37'])
+@register_model(
+    ModelType.codeqwen1half_7b_chat,
+    'qwen/CodeQwen1.5-7B-Chat',
+    LoRATM.qwen1half,
+    TemplateType.qwen,
+    support_flash_attn=True,
+    support_vllm=True,
+    requires=['transformers>=4.37'])
 def get_model_tokenizer_qwen1half(model_dir: str,
                                   torch_dtype: Dtype,
                                   model_kwargs: Dict[str, Any],
                                   load_model: bool = True,
                                   **kwargs):
     is_awq = kwargs.pop('is_awq', False)
     is_training = kwargs.pop('is_training', False)
@@ -2075,17 +2136,19 @@
 }
 
 
 def get_model_tokenizer_qwen(model_dir: str,
                              torch_dtype: Dtype,
                              model_kwargs: Dict[str, Any],
                              load_model: bool = True,
+                             model_config=None,
                              **kwargs):
-    model_config = AutoConfig.from_pretrained(
-        model_dir, trust_remote_code=True)
+    if model_config is None:
+        model_config = AutoConfig.from_pretrained(
+            model_dir, trust_remote_code=True)
     if torch_dtype is not None:
         k_true = dtype_mapping[torch_dtype]
         for k in dtype_mapping.values():
             v = False
             if k == k_true:
                 v = True
             setattr(model_config, k, v)
@@ -2278,14 +2341,23 @@
                                 **kwargs):
     if (model_kwargs.get('quantization_config') is not None and isinstance(
             model_kwargs['quantization_config'], BitsAndBytesConfig)):
         # https://github.com/pytorch/pytorch/issues/58969
         model_kwargs['quantization_config'].llm_int8_skip_modules = [
             'lm_head', 'attn_pool.attn'
         ]
+        _TransformerBlock = get_class_from_dynamic_module(
+            'visual.TransformerBlock', model_dir)
+
+        def _get_cast_dtype(self) -> torch.dtype:
+            return self.resblocks[0].ln_1.weight.dtype
+
+        _TransformerBlock.__old_get_cast_dtype = _TransformerBlock.get_cast_dtype
+        _TransformerBlock.get_cast_dtype = _get_cast_dtype
+
     get_qwen_function = kwargs.pop('get_qwen_function',
                                    get_model_tokenizer_qwen_chat)
     tokenizer_config = get_tokenizer_config(model_dir)
     class_ref = tokenizer_config['auto_map']['AutoTokenizer'][0]
     tokenizer_cls = get_class_from_dynamic_module(class_ref, model_dir)
     tokenizer_cls._auto_class = 'AutoTokenizer'
     tokenizer_cls.IMAGE_ST = ()  # fix no attr `self.IMAGE_ST` bug
@@ -2891,54 +2963,139 @@
             inputs = input_ids
         return generate(inputs, *args, **kwargs)
 
     model.generate = _new_generate
 
 
 @register_model(
+    ModelType.llava1d6_yi_34b_instruct,
+    'AI-ModelScope/llava-v1.6-34b',
+    LoRATM.llama2,
+    TemplateType.llava_yi_instruct,
+    eos_token='<|im_end|>',
+    support_flash_attn=True,
+    function_kwargs={'llm_model_type': 'llama'},
+    tags=['multi-modal', 'vision'],
+    hf_model_id='liuhaotian/llava-v1.6-34b')
+@register_model(
     ModelType.llava1d6_mistral_7b_instruct,
     'AI-ModelScope/llava-v1.6-mistral-7b',
     LoRATM.llama2,
     TemplateType.llava_mistral_instruct,
     requires=['transformers>=4.34'],
     support_flash_attn=True,
-    tags=['multi-modal', 'vision'])
+    function_kwargs={'llm_model_type': 'mistral'},
+    tags=['multi-modal', 'vision'],
+    hf_model_id='liuhaotian/llava-v1.6-mistral-7b')
 def get_model_tokenizer_llava(model_dir: str,
                               torch_dtype: Dtype,
                               model_kwargs: Dict[str, Any],
                               load_model: bool = True,
                               **kwargs):
     local_repo_path = _git_clone_github(
         'https://github.com/haotian-liu/LLaVA.git')
     sys.path.append(os.path.join(local_repo_path))
 
-    from llava.model import LlavaMistralForCausalLM, LlavaMistralConfig
-    model_config = LlavaMistralConfig.from_pretrained(model_dir)
+    llm_model_type = kwargs.pop('llm_model_type')
+    if llm_model_type == 'mistral':
+        from llava.model import LlavaMistralForCausalLM, LlavaMistralConfig
+        model_config = LlavaMistralConfig.from_pretrained(model_dir)
+        automodel_class = LlavaMistralForCausalLM
+    else:  # llama
+        from llava.model import LlavaLlamaForCausalLM, LlavaConfig
+        if not hasattr(LlavaLlamaForCausalLM,
+                       '__old_forward'):  # Avoid double patching
+            forward = LlavaLlamaForCausalLM.forward
+            LlavaLlamaForCausalLM.__old_forward = forward
+
+            @wraps(forward)
+            def _new_forward(*args, **kwargs):
+                kwargs.pop('cache_position', None)
+                return forward(*args, **kwargs)
+
+            LlavaLlamaForCausalLM.forward = _new_forward
+        model_config = LlavaConfig.from_pretrained(model_dir)
+        automodel_class = LlavaLlamaForCausalLM
     model_config.mm_vision_tower = snapshot_download(
         'AI-ModelScope/clip-vit-large-patch14-336')
     model, tokenizer = get_model_tokenizer_with_flash_attn(
         model_dir,
         torch_dtype,
         model_kwargs,
         load_model,
         model_config=model_config,
-        automodel_class=LlavaMistralForCausalLM,
+        automodel_class=automodel_class,
         **kwargs)
 
     model.resize_token_embeddings(len(tokenizer))
     vision_tower = model.get_vision_tower()
     device_map = str(model_kwargs.get('device_map', str(model.device)))
     if not vision_tower.is_loaded:
         vision_tower.load_model(device_map=device_map)
     if not hasattr(model.config, 'max_sequence_length'):
         model.config.max_sequence_length = 2048
     _patch_llava(model)
     return model, tokenizer
 
 
+@register_model(
+    ModelType.mplug_owl2_chat,
+    'iic/mPLUG-Owl2',
+    LoRATM.mplug_owl2,
+    TemplateType.mplug_owl2,
+    requires=['transformers<4.35', 'icecream'],
+    eos_token='</s>',
+    function_kwargs={
+        'get_model_tokenizer_function': get_model_tokenizer_with_flash_attn
+    },
+    support_flash_attn=True)
+@register_model(
+    ModelType.mplug_owl2d1_chat,
+    'iic/mPLUG-Owl2.1',
+    LoRATM.mplug_owl2d1,
+    TemplateType.mplug_owl2,
+    requires=['transformers<4.35', 'icecream'],
+    eos_token='<|endoftext|>',
+    function_kwargs={
+        'vocab_size': 151851,
+        'get_model_tokenizer_function': get_model_tokenizer_qwen
+    },
+    support_flash_attn=True)
+def get_model_tokenizer_mplug_owl2(model_dir: str,
+                                   torch_dtype: Dtype,
+                                   model_kwargs: Dict[str, Any],
+                                   load_model: bool = True,
+                                   **kwargs):
+    local_repo_path = _git_clone_github('https://github.com/X-PLUG/mPLUG-Owl')
+    local_repo_path = os.path.join(local_repo_path, 'mPLUG-Owl2')
+    sys.path.append(os.path.join(local_repo_path))
+
+    # register
+    # https://github.com/X-PLUG/mPLUG-Owl/blob/main/mPLUG-Owl2/mplug_owl2/model/modeling_mplug_owl2.py#L447
+    from mplug_owl2 import MPLUGOwl2LlamaForCausalLM
+    from transformers.models.clip.image_processing_clip import CLIPImageProcessor
+    model_config = AutoConfig.from_pretrained(
+        model_dir, trust_remote_code=True)
+    vocab_size = kwargs.pop('vocab_size', None)
+    if vocab_size is not None:
+        model_config.vocab_size = vocab_size
+    get_model_tokenizer_function = kwargs.pop('get_model_tokenizer_function')
+    model, tokenizer = get_model_tokenizer_function(
+        model_dir,
+        torch_dtype,
+        model_kwargs,
+        load_model,
+        model_config=model_config,
+        **kwargs)
+    logger.info('Please ignore the unimported warning.')
+    image_processor = CLIPImageProcessor.from_pretrained(model_dir)
+    tokenizer.image_processor = image_processor
+    return model, tokenizer
+
+
 def fix_transformers_upgrade(module: PreTrainedModel) -> None:
     # from 4.35, transformers changes its arguments of _set_gradient_checkpointing
     if version.parse(transformers.__version__) >= version.parse('4.35'):
         if isinstance(module, PreTrainedModel) and hasattr(module, '_set_gradient_checkpointing') \
                 and 'value' in inspect.signature(module._set_gradient_checkpointing).parameters.keys():
             module._set_gradient_checkpointing = MethodType(
                 PreTrainedModel._set_gradient_checkpointing, module)
@@ -3108,15 +3265,14 @@
     return model, tokenizer
 
 
 def get_additional_saved_files(model_type: str) -> List[str]:
     files_mapping = {
         'qwen-vl': ['SimSun.ttf'],
         'qwen-audio': ['mel_filters.npz'],
-        'deepseek-vl': ['preprocessor_config.json'],
         'yi-vl': ['vit']
     }
     for key, files_list in files_mapping.items():
         if key in model_type:
             return files_list
     return []
```

### Comparing `ms-swift-2.0.0/swift/llm/utils/preprocess.py` & `ms-swift-2.0.1/swift/llm/utils/preprocess.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/llm/utils/protocol.py` & `ms-swift-2.0.1/swift/llm/utils/protocol.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/llm/utils/template.py` & `ms-swift-2.0.1/swift/llm/utils/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     qwen = 'qwen'
     qwen_audio = 'qwen-audio'
     baichuan = 'baichuan'
     chatglm2 = 'chatglm2'
     chatglm3 = 'chatglm3'
     llama = 'llama'
     llava_mistral_instruct = 'llava-mistral-instruct'
+    llava_yi_instruct = 'llava-yi-instruct'
     openbuddy = 'openbuddy'
     internlm = 'internlm'
     internlm2 = 'internlm2'
     internlm_xcomposer2 = 'internlm-xcomposer2'
     yi = 'yi'
     yi_vl = 'yi-vl'
     yuan = 'yuan'
@@ -55,14 +56,15 @@
     cogvlm_instruct = 'cogvlm-instruct'
     cogagent_chat = 'cogagent-chat'
     cogagent_instruct = 'cogagent-instruct'
     orion = 'orion'
     minicpm = 'minicpm'
     minicpm_v = 'minicpm-v'
     gemma = 'gemma'
+    mplug_owl2 = 'mplug-owl2'
     # compatibility. (Deprecated)
     chatml = 'chatml'
     telechat = 'telechat'
     dbrx = 'dbrx'
     mengzi = 'mengzi'
     c4ai = 'c4ai'
 
@@ -79,15 +81,15 @@
 Prompt = List[Union[str, List[Union[str, int]]]]
 StopWords = Prompt
 
 Context = Union[str, List[int]]
 
 
 class StopWordsCriteria(StoppingCriteria):
-
+    # The returned sentence includes stop words.
     def __init__(self, tokenizer: PreTrainedTokenizerBase,
                  stop_words: StopWords, **tokenizer_kwargs) -> None:
         self.tokenizer = tokenizer
         self.stop_words = stop_words
         self.tokenizer_kwargs = tokenizer_kwargs
         self.start_idx = -1
 
@@ -936,14 +938,30 @@
     TemplateType.llava_mistral_instruct,
     LLavaTemplate(),
     use_model=True,
     infer_media_type='round',
     lazy_tokenize=True)
 
 
+class LLavaYiTemplate(LLavaTemplate):
+    llavayi_query_template = '\n<|im_start|>user\n{{QUERY}}<|im_end|>\n<|im_start|>assistant\n'
+
+    def __init__(self):
+        Template.__init__(self, [], [[-200], self.llavayi_query_template],
+                          None, ['<|im_end|>'])
+
+
+register_template(
+    TemplateType.llava_yi_instruct,
+    LLavaYiTemplate(),
+    use_model=True,
+    infer_media_type='round',
+    lazy_tokenize=True)
+
+
 def _findall(token_list: List[int], token: int) -> List[int]:
     """Find the index of a token in the token_list."""
     res = []
     idx = -1
     try:
         while True:
             idx = token_list.index(token, idx + 1)
@@ -1190,15 +1208,15 @@
             placeholder_id = self.tokenizer.encode(
                 placeholder, add_special_tokens=False)
             input_ids = (
                 input_ids[:idx - 1] + placeholder_id + input_ids[idx + 2:])
             if labels is not None:
                 labels = (
                     labels[:idx - 1] + [-100] * len(placeholder_id)
-                    + labels[idx + 2])
+                    + labels[idx + 2:])
             input_tensor_ids = torch.tensor(input_ids)
             image_start_idx = torch.where(
                 input_tensor_ids == self.tokenizer.im_start_id)[0]
             image_start_idx += 1
             image_end_idx = torch.where(
                 input_tensor_ids == self.tokenizer.im_end_id)[0]
             valid_image_nums = max(len(image_start_idx), len(image_end_idx))
@@ -1299,14 +1317,57 @@
     Template(['<BOS_TOKEN>'], [
         '<|START_OF_TURN_TOKEN|><|USER_TOKEN|>{{QUERY}}<|END_OF_TURN_TOKEN|><|START_OF_TURN_TOKEN|><|CHATBOT_TOKEN|>'
     ], ['<|END_OF_TURN_TOKEN|>'], ['<|END_OF_TURN_TOKEN|>'], C4AI_SYSTEM, [
         '<|START_OF_TURN_TOKEN|><|SYSTEM_TOKEN|>{{SYSTEM}}<|END_OF_TURN_TOKEN|'
     ]))
 
 
+class mPlugOwl2Template(Template):
+
+    def __init__(self):
+        return super().__init__(['{{SYSTEM}}'],
+                                ['USER: ', [-200], '{{QUERY}}ASSISTANT:'],
+                                ['</s>'], [['eos_token_id']])
+
+    def encode(
+            self, example: Dict[str,
+                                Any]) -> Tuple[Dict[str, Any], Dict[str, Any]]:
+        from mplug_owl2.mm_utils import process_images
+        image_processor = self.tokenizer.image_processor
+        images_path = example['images']
+        images = []
+        for image_path in images_path:
+            image = _read_from_path(image_path)
+            # ref: https://modelscope.cn/models/iic/mPLUG-Owl2.1/summary
+            max_edge = max(image.size)
+            image = image.resize((max_edge, max_edge))
+            images.append(image)
+        inputs, _ = super().encode(example)
+        input_ids = inputs['input_ids']
+        labels = inputs['labels']
+        images = process_images(images, image_processor)
+        images = images.to(self.model.dtype)
+        return {'input_ids': input_ids, 'labels': labels, 'images': images}, {}
+
+    def data_collator(self,
+                      batch: List[Dict[str, Any]],
+                      padding_to: Optional[int] = None) -> Dict[str, Any]:
+        res = super().data_collator(batch, padding_to)
+        res['images'] = torch.concat([b['images'] for b in batch])
+        return res
+
+
+register_template(
+    TemplateType.mplug_owl2,
+    mPlugOwl2Template(),
+    infer_media_type='round',
+    use_model=True,
+    lazy_tokenize=True)
+
+
 def get_template(
     template_type: str,
     tokenizer: PreTrainedTokenizerBase,
     default_system: Optional[str] = None,
     max_length: Optional[int] = None,
     truncation_strategy: Literal['delete', 'truncation_left'] = 'delete',
     **kwargs,
```

### Comparing `ms-swift-2.0.0/swift/llm/utils/utils.py` & `ms-swift-2.0.1/swift/llm/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/llm/utils/vllm_utils.py` & `ms-swift-2.0.1/swift/llm/utils/vllm_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/torchacc_utils.py` & `ms-swift-2.0.1/swift/torchacc_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/trainers/__init__.py` & `ms-swift-2.0.1/swift/trainers/__init__.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/trainers/arguments.py` & `ms-swift-2.0.1/swift/trainers/arguments.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/trainers/callback.py` & `ms-swift-2.0.1/swift/trainers/callback.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/trainers/dpo_trainers.py` & `ms-swift-2.0.1/swift/trainers/dpo_trainers.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/trainers/mixin.py` & `ms-swift-2.0.1/swift/trainers/mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -443,23 +443,26 @@
                 safe_serialization=save_safetensors)
         # tokenizer
         if self.tokenizer is not None:
             self.tokenizer.save_pretrained(output_dir)
         # training_args.bin
         torch.save(self.args, os.path.join(output_dir, 'training_args.bin'))
         # additional files
-        additional_files = getattr(self.args, 'additional_saved_files', [])
-        if model_dir is not None:
-            for file in additional_files:
-                src_path = os.path.join(model_dir, file)
-                dst_path = os.path.join(output_dir, file)
-                if os.path.isfile(src_path):
-                    shutil.copy(src_path, dst_path)
-                elif os.path.isdir(src_path):
-                    shutil.copytree(src_path, dst_path)
+        sft_args = getattr(self, 'sft_args', None)
+        if sft_args is not None and sft_args.sft_type == 'full':
+            additional_files = getattr(self.args, 'additional_saved_files',
+                                       []) + ['preprocessor_config.json']
+            if model_dir is not None:
+                for file in additional_files:
+                    src_path = os.path.join(model_dir, file)
+                    dst_path = os.path.join(output_dir, file)
+                    if os.path.isfile(src_path):
+                        shutil.copy(src_path, dst_path)
+                    elif os.path.isdir(src_path):
+                        shutil.copytree(src_path, dst_path)
 
     def _save_checkpoint(self, model, trial, metrics=None):
         self.state.last_model_checkpoint = os.path.join(
             self.args.output_dir, f'checkpoint-{self.state.global_step}')
         logger.info(
             f'Saving model checkpoint to {self.state.last_model_checkpoint}')
         if version.parse(transformers.__version__) >= version.parse(
```

### Comparing `ms-swift-2.0.0/swift/trainers/optimizers/galore/__init__.py` & `ms-swift-2.0.1/swift/trainers/optimizers/galore/__init__.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/trainers/optimizers/galore/adafactor.py` & `ms-swift-2.0.1/swift/trainers/optimizers/galore/adafactor.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/trainers/optimizers/galore/adamw.py` & `ms-swift-2.0.1/swift/trainers/optimizers/galore/adamw.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/trainers/optimizers/galore/adamw8bit.py` & `ms-swift-2.0.1/swift/trainers/optimizers/galore/adamw8bit.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/trainers/optimizers/galore/galore_projector.py` & `ms-swift-2.0.1/swift/trainers/optimizers/galore/galore_projector.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/trainers/optimizers/galore/utils.py` & `ms-swift-2.0.1/swift/trainers/optimizers/galore/utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/trainers/trainers.py` & `ms-swift-2.0.1/swift/trainers/trainers.py`

 * *Files 12% similar despite different names*

```diff
@@ -263,16 +263,49 @@
             if 'acc' not in self._custom_metrics:
                 self._custom_metrics['acc'] = self._acc
             self._custom_metrics['acc'] = self._custom_metrics[
                 'acc'] + acc / self.args.gradient_accumulation_steps
         return (loss, outputs) if return_outputs else loss
 
     def get_train_dataloader(self):
+
+        def __iter__(self):
+            self._num_yielded = 0
+            if self._iterator is None:
+                self._iterator = self.__original_iter__()
+            return self
+
+        def __next__(self):
+            if self._num_yielded >= len(self):
+                raise StopIteration
+            self._num_yielded += 1
+            try:
+                return next(self._iterator)
+            except StopIteration:
+                self._iterator = self.__original_iter__()
+            return next(self._iterator)
+
         if not use_torchacc():
-            return super().get_train_dataloader()
+            origin_loader = super().get_train_dataloader()
+            grad_acc_steps = self.args.gradient_accumulation_steps
+            if grad_acc_steps is None or grad_acc_steps <= 1:
+                return origin_loader
+
+            length = len(origin_loader) // grad_acc_steps * grad_acc_steps
+            origin_loader_type = type(origin_loader)
+            loader = type(
+                origin_loader_type.__name__, (origin_loader_type, ), {
+                    '__len__': lambda _: length,
+                    '__iter__': __iter__,
+                    '__next__': __next__
+                })(
+                    origin_loader.dataset)
+            loader.__dict__.update(origin_loader.__dict__)
+            loader.__original_iter__ = origin_loader.__iter__
+            return loader
         else:
             if trainer.is_datasets_available():
                 import datasets
 
             if self.train_dataset is None:
                 raise ValueError('Trainer: training requires a train_dataset.')
```

### Comparing `ms-swift-2.0.0/swift/trainers/utils.py` & `ms-swift-2.0.1/swift/trainers/utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/tuners/__init__.py` & `ms-swift-2.0.1/swift/tuners/__init__.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/tuners/adapter.py` & `ms-swift-2.0.1/swift/tuners/adapter.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/tuners/base.py` & `ms-swift-2.0.1/swift/tuners/base.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/tuners/llamapro.py` & `ms-swift-2.0.1/swift/tuners/llamapro.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/tuners/longlora/llama.py` & `ms-swift-2.0.1/swift/tuners/longlora/llama.py`

 * *Files 1% similar despite different names*

```diff
@@ -427,15 +427,21 @@
 
     attn_output = self.o_proj(attn_output)
 
     return attn_output, None, past_key_value
 
 
 def replace_llama_attn(model: nn.Module):
-    for idx, m in enumerate(model.model.layers):
+    layers = None
+    for module in model.modules():
+        if isinstance(module, torch.nn.ModuleList):
+            layers = module
+            break
+    assert layers is not None
+    for idx, m in enumerate(layers):
         if model.config._attn_implementation == 'flash_attention_2':
             cuda_major, cuda_minor = torch.cuda.get_device_capability()
             if cuda_major < 8:
                 logger.warn(
                     'Flash attention is only supported on A100 or H100 GPU during training due to head dim > 64 backward.'  # noqa
                     'ref: https://github.com/HazyResearch/flash-attention/issues/190#issuecomment-1523359593'
                 )
```

### Comparing `ms-swift-2.0.0/swift/tuners/longlora/longlora.py` & `ms-swift-2.0.1/swift/tuners/longlora/longlora.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/tuners/lora.py` & `ms-swift-2.0.1/swift/tuners/lora.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,17 +87,14 @@
         super(peft.LoraConfig, self).save_pretrained(save_directory, **kwargs)
 
 
 class LoRA(SwiftAdapter):
 
     @staticmethod
     def prepare_model(model: nn.Module, config: LoRAConfig, adapter_name: str):
-        if version.parse(peft.__version__) >= version.parse('0.10.0'):
-            logger.error('The swift LoRA adapter only supports peft<0.10.0')
-
         assert not config.use_qa_lora, 'Do not use qa-lora'
         if config.use_qa_lora:
             auto_gptq_config = get_quantization_config(model, method='gptq')
             if auto_gptq_config:
                 config.group_size = getattr(auto_gptq_config, 'group_size',
                                             None)
         LoraModel(model, config, adapter_name)
```

### Comparing `ms-swift-2.0.0/swift/tuners/lora_layers.py` & `ms-swift-2.0.1/swift/tuners/lora_layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,29 +107,14 @@
         if not self.unique_thread:
             raise AssertionError(
                 'Merge is unsupported in multiple thread, '
                 'please set `USE_UNIQUE_THREAD=1` in env variable to merge LoRA.'
             )
         return super().merge(*args, **kwargs)
 
-    def _apply_dora(self, x, lora_A, lora_B, scaling, active_adapter):
-        """
-        From LoraLayer._apply_dora, to support `weight.to(x.dtype)`
-        """
-        lora_weight = lora_B.weight @ lora_A.weight
-        magnitude = self.lora_magnitude_vector[active_adapter]
-        weight = self.get_base_layer().weight
-        weight_norm = self._get_weight_norm(weight, lora_weight, scaling)
-        weight_norm = weight_norm.detach()
-        mag_norm_scale = (magnitude / weight_norm).view(1, -1)
-        result_dora = (mag_norm_scale - 1) * (F.linear(
-            x, transpose(weight.to(x.dtype), self.fan_in_fan_out)
-        )) + mag_norm_scale * lora_B(lora_A(x)) * scaling
-        return result_dora
-
 
 if is_bnb_available():
     import bitsandbytes as bnb
     from peft.tuners.lora.bnb import Linear8bitLt as _Linear8bitLt
 
     class Linear8bitLt(LoRAActivationMixin, _Linear8bitLt):
 
@@ -531,16 +516,17 @@
     def __init__(self, *args, module_key: str, **kwargs):
         super(Linear, self).__init__(module_key)
         self.set_activation(args[1], True)
         super(ActivationMixin, self).__init__(*args, **kwargs)
 
         def device_hook(module, args):
             for active_adapter in self.active_adapters:
-                self.lora_A[active_adapter].to(args[0].device)
-                self.lora_B[active_adapter].to(args[0].device)
+                if active_adapter in self.lora_A:
+                    self.lora_A[active_adapter].to(args[0].device)
+                    self.lora_B[active_adapter].to(args[0].device)
 
         self.register_forward_pre_hook(device_hook)
 
     def update_layer(self,
                      adapter_name,
                      r,
                      lora_alpha,
@@ -670,14 +656,17 @@
 
         peft_config = self._prepare_adapter_config(peft_config, model_config)
 
         if version.parse(peft.__version__) > version.parse('0.8.2'):
             from peft.tuners.tuners_utils import _maybe_include_all_linear_layers
             # update peft_config.target_modules if required
             peft_config = _maybe_include_all_linear_layers(peft_config, model)
+        if version.parse(peft.__version__) >= version.parse('0.10.0'):
+            self._prepare_model(peft_config, model)
+
         for key in key_list:
             # Check for modules_to_save in case
             if _check_for_modules_to_save and any(
                     key.endswith(f'{module_to_save}')
                     for module_to_save in peft_config.modules_to_save):
                 # Optionally set the modules to save
                 parent, target, target_name = _get_submodules(model, key)
@@ -802,17 +791,17 @@
                       LoraLayer) and not isinstance(target, AdaLoraLayer):
             if target.__class__.__name__ == 'NonDynamicallyQuantizableLinear':
                 # Fix issue: https://github.com/modelscope/swift/issues/342
                 return
             target.update_layer(
                 adapter_name,
                 r,
-                alpha,
-                lora_config.lora_dropout,
-                lora_config.init_lora_weights,
+                lora_alpha=alpha,
+                lora_dropout=lora_config.lora_dropout,
+                init_lora_weights=lora_config.init_lora_weights,
                 use_rslora=lora_config.use_rslora,
                 use_dora=lora_config.use_dora,
             )
             self._convert_dtype(target, lora_config.lora_dtype)
         else:
             new_module = self._create_new_module(
                 lora_config,
```

### Comparing `ms-swift-2.0.0/swift/tuners/mapping.py` & `ms-swift-2.0.1/swift/tuners/mapping.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/tuners/module_mapping.py` & `ms-swift-2.0.1/swift/tuners/module_mapping.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/tuners/neftune.py` & `ms-swift-2.0.1/swift/tuners/neftune.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/tuners/peft.py` & `ms-swift-2.0.1/swift/tuners/peft.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,26 +5,24 @@
 from functools import partial, reduce
 from typing import Dict, Optional
 
 import json
 import peft
 import torch
 import torch.nn
-import torch.nn.functional as F
 from peft import (AdaLoraConfig, IA3Config, LoftQConfig, LoHaConfig,
                   LoKrConfig, LoraModel, OFTConfig, PeftConfig, PeftModel,
                   PeftModelForCausalLM, PeftModelForSeq2SeqLM,
                   PeftModelForSequenceClassification,
                   PeftModelForTokenClassification, PrefixTuningConfig,
                   PromptEncoderConfig, PromptLearningConfig,
                   PromptTuningConfig, get_peft_config, get_peft_model,
                   get_peft_model_state_dict)
 from peft.config import PeftConfigMixin
 from peft.tuners.lora import Embedding
-from peft.utils.other import transpose
 from transformers import Trainer
 
 from swift import get_logger
 from swift.hub.snapshot_download import snapshot_download
 
 logger = get_logger()
 dispatchers = []
@@ -88,30 +86,14 @@
                 _json = json.load(f)
                 for key, value in _json.items():
                     setattr(self, key, value)
 
         return self
 
 
-def _apply_dora(self, x, lora_A, lora_B, scaling, active_adapter):
-    """
-    From LoraLayer._apply_dora, to support `weight.to(x.dtype)`
-    """
-    lora_weight = lora_B.weight @ lora_A.weight
-    magnitude = self.lora_magnitude_vector[active_adapter]
-    weight = self.get_base_layer().weight
-    weight_norm = self._get_weight_norm(weight, lora_weight, scaling)
-    weight_norm = weight_norm.detach()
-    mag_norm_scale = (magnitude / weight_norm).view(1, -1)
-    result_dora = (mag_norm_scale - 1) * (F.linear(
-        x, transpose(weight.to(x.dtype), self.fan_in_fan_out)
-    )) + mag_norm_scale * lora_B(lora_A(x)) * scaling
-    return result_dora
-
-
 def _create_and_replace_hook(self, *args, **kwargs):
     target = None
     if 'target' in kwargs:
         target = kwargs['target']
     else:
         for arg in args:
             if isinstance(arg, torch.nn.Module):
@@ -205,14 +187,15 @@
             'lr': lr * self.peft_config[self.active_adapter].lorap_lr_ratio,
         },
     ]
     return param_groups
 
 
 def adalora_forward(self, *args, **kwargs):
+    from peft.utils.integrations import gather_params_ctx
     outputs = self.model.forward(*args, **kwargs)
 
     if (getattr(outputs, 'loss', None) is not None) and isinstance(
             outputs.loss, torch.Tensor):
         # Calculate the orthogonal regularization
         orth_reg_weight = self.peft_config[
             self.trainable_adapter_name].orth_reg_weight
@@ -221,15 +204,19 @@
             raise ValueError('orth_reg_weight should be greater than 0. ')
 
         regu_loss = 0
         num_param = 0
         for n, p in self.model.named_parameters():
             if ('lora_A' in n
                     or 'lora_B' in n) and self.trainable_adapter_name in n:
-                para_cov = p @ p.T if 'lora_A' in n else p.T @ p
+                if p.shape == torch.Size([0]):
+                    with gather_params_ctx(p, fwd_module=self):
+                        para_cov = p @ p.T if 'lora_A' in n else p.T @ p
+                else:
+                    para_cov = p @ p.T if 'lora_A' in n else p.T @ p
                 I = torch.eye(
                     *para_cov.size(),
                     out=torch.empty_like(para_cov))  # noqa: E741
                 I.requires_grad = False
                 num_param += 1
                 if isinstance(regu_loss, torch.Tensor):
                     regu_loss = regu_loss.to(para_cov.device)
@@ -305,17 +292,14 @@
 def hot_patch_peft_module():
     from peft.tuners.lora import LoraLayer
 
     # Fix Lora does not support NonDynamicallyQuantizableLinear
     LoraModel._create_and_replace_origin = LoraModel._create_and_replace
     LoraModel._create_and_replace = _create_and_replace_hook
 
-    # Fix dora dtype
-    LoraLayer._apply_dora = _apply_dora
-
     # Support type conversion
     def init(self, model: torch.nn.Module, config: Dict[str, LoraConfig],
              adapter_name):
         self.__init_origin__(model, config, adapter_name)
         active_config = config[self.active_adapter] if isinstance(
             config, dict) else config
         if hasattr(active_config, 'lora_dtype'):
```

### Comparing `ms-swift-2.0.0/swift/tuners/prompt.py` & `ms-swift-2.0.1/swift/tuners/prompt.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/tuners/restuning.py` & `ms-swift-2.0.1/swift/tuners/restuning.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/tuners/restuning_components.py` & `ms-swift-2.0.1/swift/tuners/restuning_components.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/tuners/rome/compute_u.py` & `ms-swift-2.0.1/swift/tuners/rome/compute_u.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/tuners/rome/compute_v.py` & `ms-swift-2.0.1/swift/tuners/rome/compute_v.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/tuners/rome/context_template.py` & `ms-swift-2.0.1/swift/tuners/rome/context_template.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/tuners/rome/nethook.py` & `ms-swift-2.0.1/swift/tuners/rome/nethook.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/tuners/rome/repr_tools.py` & `ms-swift-2.0.1/swift/tuners/rome/repr_tools.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/tuners/rome/rome.py` & `ms-swift-2.0.1/swift/tuners/rome/rome.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/tuners/rome/rome_hparams.py` & `ms-swift-2.0.1/swift/tuners/rome/rome_hparams.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/tuners/scetuning/scetuning.py` & `ms-swift-2.0.1/swift/tuners/scetuning/scetuning.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/tuners/scetuning/scetuning_components.py` & `ms-swift-2.0.1/swift/tuners/scetuning/scetuning_components.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/tuners/side.py` & `ms-swift-2.0.1/swift/tuners/side.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/tuners/utils.py` & `ms-swift-2.0.1/swift/tuners/utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/ui/app.py` & `ms-swift-2.0.1/swift/ui/app.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/ui/base.py` & `ms-swift-2.0.1/swift/ui/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -43,14 +43,17 @@
                 values = builder.locale(elem_id, lang)
                 if 'info' in values:
                     kwargs['info'] = values['info']
                 if 'value' in values:
                     kwargs['value'] = values['value']
                 if 'label' in values:
                     kwargs['label'] = values['label']
+                argument = base_builder.argument(elem_id)
+                if argument and 'label' in kwargs:
+                    kwargs['label'] = kwargs['label'] + f'({argument})'
 
         ret = fn(self, **kwargs)
         self.constructor_args.update(kwargs)
 
         if builder is not None:
             builder.element_dict[elem_id] = self
         return ret
@@ -69,14 +72,15 @@
 
 class BaseUI:
 
     choice_dict: Dict[str, List] = {}
     default_dict: Dict[str, Any] = {}
     locale_dict: Dict[str, Dict] = {}
     element_dict: Dict[str, Dict] = {}
+    arguments: Dict[str, str] = {}
     sub_ui: List[Type['BaseUI']] = []
     group: str = None
     lang: str = all_langs[0]
     int_regex = r'^[-+]?[0-9]+$'
     float_regex = r'[-+]?(?:\d*\.*\d+)'
 
     @classmethod
@@ -144,14 +148,19 @@
     @classmethod
     def element(cls, elem_id):
         """Get element by elem_id"""
         elements = cls.elements()
         return elements[elem_id]
 
     @classmethod
+    def argument(cls, elem_id):
+        """Get argument by elem_id"""
+        return cls.arguments.get(elem_id)
+
+    @classmethod
     def set_lang(cls, lang):
         cls.lang = lang
         for sub_ui in cls.sub_ui:
             sub_ui.lang = lang
 
     @staticmethod
     def get_choices_from_dataclass(dataclass):
@@ -170,10 +179,17 @@
             if hasattr(dataclass, f.name):
                 default_dict[f.name] = getattr(dataclass, f.name)
             else:
                 default_dict[f.name] = None
         return default_dict
 
     @staticmethod
+    def get_argument_names(dataclass):
+        arguments = {}
+        for f in fields(dataclass):
+            arguments[f.name] = f'--{f.name}'
+        return arguments
+
+    @staticmethod
     def get_custom_name_list():
         return list(
             set(MODEL_MAPPING.keys()) - set(ModelType.get_model_name_list()))
```

### Comparing `ms-swift-2.0.0/swift/ui/llm_infer/generate.py` & `ms-swift-2.0.1/swift/ui/llm_infer/generate.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/ui/llm_infer/llm_infer.py` & `ms-swift-2.0.1/swift/ui/llm_infer/llm_infer.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,15 @@
                 'zh': '选择训练使用的GPU号，如CUDA不可用只能选择CPU',
                 'en': 'Select GPU to train'
             }
         },
     }
 
     choice_dict = BaseUI.get_choices_from_dataclass(InferArguments)
+    arguments = BaseUI.get_argument_names(InferArguments)
 
     @classmethod
     def do_build_ui(cls, base_tab: Type['BaseUI']):
         with gr.TabItem(elem_id='llm_infer', label=''):
             gpu_count = 0
             default_device = 'cpu'
             if torch.cuda.is_available():
```

### Comparing `ms-swift-2.0.0/swift/ui/llm_infer/model.py` & `ms-swift-2.0.1/swift/ui/llm_infer/model.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/ui/llm_infer/runtime.py` & `ms-swift-2.0.1/swift/ui/llm_infer/runtime.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/ui/llm_train/advanced.py` & `ms-swift-2.0.1/swift/ui/llm_train/advanced.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/ui/llm_train/dataset.py` & `ms-swift-2.0.1/swift/ui/llm_train/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,17 +107,17 @@
                 elem_id='custom_val_dataset_path', is_list=True, scale=20)
         with gr.Row():
             gr.Slider(
                 elem_id='dataset_test_ratio',
                 minimum=0.0,
                 maximum=1.0,
                 step=0.05,
-                scale=10)
+                scale=20)
             gr.Slider(
                 elem_id='max_length',
                 minimum=32,
                 maximum=8192,
                 step=32,
                 scale=20)
             gr.Textbox(elem_id='train_dataset_sample', scale=20)
             gr.Textbox(elem_id='val_dataset_sample', scale=20)
-            gr.Dropdown(elem_id='truncation_strategy', scale=10)
+            gr.Dropdown(elem_id='truncation_strategy', scale=20)
```

### Comparing `ms-swift-2.0.0/swift/ui/llm_train/hyper.py` & `ms-swift-2.0.1/swift/ui/llm_train/hyper.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/ui/llm_train/llm_train.py` & `ms-swift-2.0.1/swift/ui/llm_train/llm_train.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,14 +196,15 @@
                 'en': 'Create unique optimizer for per Galore parameter'
             },
         }
     }
 
     choice_dict = BaseUI.get_choices_from_dataclass(SftArguments)
     default_dict = BaseUI.get_default_value_from_dataclass(SftArguments)
+    arguments = BaseUI.get_argument_names(SftArguments)
 
     @classmethod
     def do_build_ui(cls, base_tab: Type['BaseUI']):
         with gr.TabItem(elem_id='llm_train', label=''):
             gpu_count = 0
             default_device = 'cpu'
             if torch.cuda.is_available():
@@ -342,18 +343,19 @@
 
         if os.path.exists(kwargs['model_id_or_path']):
             kwargs['model_type'] = model_type
 
         kwargs.update(more_params)
         if 'dataset' not in kwargs and 'custom_train_dataset_path' not in kwargs:
             raise gr.Error(cls.locale('dataset_alert', cls.lang)['value'])
+
         sft_args = SftArguments(
             **{
-                key: value.split(' ')
-                if key in kwargs_is_list and kwargs_is_list[key] else value
+                key: value.split(' ') if kwargs_is_list.get(key, False)
+                and isinstance(value, str) else value
                 for key, value in kwargs.items()
             })
         params = ''
 
         for e in kwargs:
             if e in kwargs_is_list and kwargs_is_list[e]:
                 params += f'--{e} {kwargs[e]} '
```

### Comparing `ms-swift-2.0.0/swift/ui/llm_train/lora.py` & `ms-swift-2.0.1/swift/ui/llm_train/lora.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/ui/llm_train/model.py` & `ms-swift-2.0.1/swift/ui/llm_train/model.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/ui/llm_train/quantization.py` & `ms-swift-2.0.1/swift/ui/llm_train/quantization.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/ui/llm_train/runtime.py` & `ms-swift-2.0.1/swift/ui/llm_train/runtime.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os.path
 import time
 import webbrowser
 from datetime import datetime
 from typing import Dict, List, Tuple, Type
 
 import gradio as gr
+import json
 import matplotlib.pyplot as plt
 import psutil
 from gradio import Accordion, Tab
 from transformers import is_tensorboard_available
 
 from swift.ui.base import BaseUI
 from swift.ui.llm_train.utils import close_loop, run_command_in_subprocess
@@ -388,14 +389,27 @@
         args = task.split('swift sft')[1]
         args = [arg.strip() for arg in args.split('--') if arg.strip()]
         all_args = {}
         for i in range(len(args)):
             space = args[i].find(' ')
             splits = args[i][:space], args[i][space + 1:]
             all_args[splits[0]] = splits[1]
+
+        output_dir = all_args['output_dir']
+        if os.path.exists(os.path.join(output_dir, 'sft_args.json')):
+            with open(os.path.join(output_dir, 'sft_args.json'), 'r') as f:
+                _json = json.load(f)
+            for key in all_args.keys():
+                all_args[key] = _json[key]
+                if isinstance(all_args[key], list):
+                    if any([' ' in value for value in all_args[key]]):
+                        all_args[key] = [
+                            f'"{value}"' for value in all_args[key]
+                        ]
+                    all_args[key] = ' '.join(all_args[key])
         return all_args
 
     @staticmethod
     def kill_task(task):
         all_args = Runtime.parse_info_from_cmdline(task)
         output_dir = all_args['output_dir']
         os.system(f'pkill -9 -f {output_dir}')
```

### Comparing `ms-swift-2.0.0/swift/ui/llm_train/save.py` & `ms-swift-2.0.1/swift/ui/llm_train/save.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/ui/llm_train/self_cog.py` & `ms-swift-2.0.1/swift/ui/llm_train/self_cog.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/ui/llm_train/utils.py` & `ms-swift-2.0.1/swift/ui/llm_train/utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/utils/__init__.py` & `ms-swift-2.0.1/swift/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/utils/constants.py` & `ms-swift-2.0.1/swift/utils/constants.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/utils/hub.py` & `ms-swift-2.0.1/swift/utils/hub.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/utils/import_utils.py` & `ms-swift-2.0.1/swift/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/utils/io_utils.py` & `ms-swift-2.0.1/swift/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/utils/logger.py` & `ms-swift-2.0.1/swift/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/utils/metric.py` & `ms-swift-2.0.1/swift/utils/metric.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/utils/np_utils.py` & `ms-swift-2.0.1/swift/utils/np_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/utils/run_utils.py` & `ms-swift-2.0.1/swift/utils/run_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/utils/tb_utils.py` & `ms-swift-2.0.1/swift/utils/tb_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/utils/torch_utils.py` & `ms-swift-2.0.1/swift/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/swift/utils/utils.py` & `ms-swift-2.0.1/swift/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/tests/hub/test_check_model.py` & `ms-swift-2.0.1/tests/hub/test_check_model.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/tests/llm/test_dataset.py` & `ms-swift-2.0.1/tests/llm/test_dataset.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/tests/llm/test_run.py` & `ms-swift-2.0.1/tests/llm/test_run.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/tests/llm/test_template.py` & `ms-swift-2.0.1/tests/llm/test_template.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/tests/llm/test_utils.py` & `ms-swift-2.0.1/tests/llm/test_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/tests/llm/test_vllm_utils.py` & `ms-swift-2.0.1/tests/llm/test_vllm_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/tests/model_tag.py` & `ms-swift-2.0.1/tests/model_tag.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/tests/run.py` & `ms-swift-2.0.1/tests/run.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/tests/test_utils.py` & `ms-swift-2.0.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/tests/tuners/test_extra_state_dict.py` & `ms-swift-2.0.1/tests/tuners/test_extra_state_dict.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/tests/tuners/test_merged_linear.py` & `ms-swift-2.0.1/tests/tuners/test_merged_linear.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/tests/tuners/test_neft.py` & `ms-swift-2.0.1/tests/tuners/test_neft.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/tests/tuners/test_peft.py` & `ms-swift-2.0.1/tests/tuners/test_peft.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/tests/tuners/test_rome.py` & `ms-swift-2.0.1/tests/tuners/test_rome.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/tests/tuners/test_scetuning.py` & `ms-swift-2.0.1/tests/tuners/test_scetuning.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/tests/tuners/test_swift_base.py` & `ms-swift-2.0.1/tests/tuners/test_swift_base.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/tests/tuners/test_swift_device_map.py` & `ms-swift-2.0.1/tests/tuners/test_swift_device_map.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/tests/tuners/test_swift_restuning.py` & `ms-swift-2.0.1/tests/tuners/test_swift_restuning.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.0/tests/utils/test_io_utils.py` & `ms-swift-2.0.1/tests/utils/test_io_utils.py`

 * *Files identical despite different names*

