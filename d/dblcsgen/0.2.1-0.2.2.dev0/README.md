# Comparing `tmp/dblcsgen-0.2.1.tar.gz` & `tmp/dblcsgen-0.2.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dblcsgen-0.2.1.tar", last modified: Tue Apr 16 19:42:13 2024, max compression
+gzip compressed data, was "dblcsgen-0.2.2.dev0.tar", last modified: Wed Apr 17 09:13:29 2024, max compression
```

## Comparing `dblcsgen-0.2.1.tar` & `dblcsgen-0.2.2.dev0.tar`

### file list

```diff
@@ -1,83 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:42:13.357708 dblcsgen-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 19:42:11.000000 dblcsgen-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    28296 2024-04-16 19:42:13.357708 dblcsgen-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14259 2024-04-16 19:42:11.000000 dblcsgen-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:42:13.357708 dblcsgen-0.2.1/dblcsgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28296 2024-04-16 19:42:13.000000 dblcsgen-0.2.1/dblcsgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-16 19:42:13.000000 dblcsgen-0.2.1/dblcsgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:42:13.000000 dblcsgen-0.2.1/dblcsgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-16 19:42:13.000000 dblcsgen-0.2.1/dblcsgen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 19:42:13.000000 dblcsgen-0.2.1/dblcsgen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 19:42:13.357708 dblcsgen-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:42:13.345708 dblcsgen-0.2.1/sglang/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:42:13.345708 dblcsgen-0.2.1/sglang/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/backend/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/backend/base_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     9578 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/backend/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/backend/runtime_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/backend/vertexai.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/global_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:42:13.345708 dblcsgen-0.2.1/sglang/lang/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/lang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/lang/chat_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/lang/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    26999 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/lang/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13320 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/lang/ir.py
--rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/lang/tracer.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/launch_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:42:13.349708 dblcsgen-0.2.1/sglang/srt/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/backend_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:42:13.349708 dblcsgen-0.2.1/sglang/srt/constrained/
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/constrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/constrained/base_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/constrained/fsm_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/constrained/jump_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)    15496 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/hf_transformers_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:42:13.349708 dblcsgen-0.2.1/sglang/srt/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/layers/context_flashattention_nopad.py
--rw-r--r--   0 runner    (1001) docker     (127)    12622 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/layers/extend_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/layers/logits_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/layers/radix_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     8516 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/layers/token_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:42:13.349708 dblcsgen-0.2.1/sglang/srt/managers/
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/managers/detokenizer_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/managers/io_struct.py
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/managers/openai_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:42:13.353708 dblcsgen-0.2.1/sglang/srt/managers/router/
--rw-r--r--   0 runner    (1001) docker     (127)    19922 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/managers/router/infer_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/managers/router/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    28007 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/managers/router/model_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    16926 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/managers/router/model_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/managers/router/radix_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/managers/router/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9743 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/managers/tokenizer_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/memory_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     8889 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/mm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/model_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:42:13.353708 dblcsgen-0.2.1/sglang/srt/models/
--rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/models/dbrx.py
--rw-r--r--   0 runner    (1001) docker     (127)    11071 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/models/dbrx_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/models/gemma.py
--rw-r--r--   0 runner    (1001) docker     (127)    11611 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/models/llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14922 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/models/llava.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/models/mistral.py
--rw-r--r--   0 runner    (1001) docker     (127)    13915 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/models/mixtral.py
--rw-r--r--   0 runner    (1001) docker     (127)     9225 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/models/qwen.py
--rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/models/qwen2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10816 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/models/stablelm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/models/yivl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/sampling_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    27702 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     9143 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/server_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/srt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:42:13.353708 dblcsgen-0.2.1/sglang/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/test/test_conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/test/test_openai_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/test/test_programs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-04-16 19:42:07.000000 dblcsgen-0.2.1/sglang/utils.py
+drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-17 09:13:29.173236 dblcsgen-0.2.2.dev0/
+-rw-r--r--   0 theneault   (502) staff       (20)    11357 2024-04-17 09:13:27.000000 dblcsgen-0.2.2.dev0/LICENSE
+-rw-r--r--   0 theneault   (502) staff       (20)    28301 2024-04-17 09:13:29.173031 dblcsgen-0.2.2.dev0/PKG-INFO
+-rw-r--r--   0 theneault   (502) staff       (20)    14259 2024-04-17 09:13:27.000000 dblcsgen-0.2.2.dev0/README.md
+drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-17 09:13:29.171983 dblcsgen-0.2.2.dev0/dblcsgen.egg-info/
+-rw-r--r--   0 theneault   (502) staff       (20)    28301 2024-04-17 09:13:29.000000 dblcsgen-0.2.2.dev0/dblcsgen.egg-info/PKG-INFO
+-rw-r--r--   0 theneault   (502) staff       (20)     1970 2024-04-17 09:13:29.000000 dblcsgen-0.2.2.dev0/dblcsgen.egg-info/SOURCES.txt
+-rw-r--r--   0 theneault   (502) staff       (20)        1 2024-04-17 09:13:29.000000 dblcsgen-0.2.2.dev0/dblcsgen.egg-info/dependency_links.txt
+-rw-r--r--   0 theneault   (502) staff       (20)      150 2024-04-17 09:13:29.000000 dblcsgen-0.2.2.dev0/dblcsgen.egg-info/requires.txt
+-rw-r--r--   0 theneault   (502) staff       (20)        7 2024-04-17 09:13:29.000000 dblcsgen-0.2.2.dev0/dblcsgen.egg-info/top_level.txt
+-rw-r--r--   0 theneault   (502) staff       (20)     1017 2024-04-17 09:13:26.000000 dblcsgen-0.2.2.dev0/pyproject.toml
+-rw-r--r--   0 theneault   (502) staff       (20)       38 2024-04-17 09:13:29.173281 dblcsgen-0.2.2.dev0/setup.cfg
+drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-17 09:13:29.157775 dblcsgen-0.2.2.dev0/sglang/
+-rw-r--r--   0 theneault   (502) staff       (20)       96 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/__init__.py
+-rw-r--r--   0 theneault   (502) staff       (20)     4576 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/api.py
+drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-17 09:13:29.158477 dblcsgen-0.2.2.dev0/sglang/backend/
+-rw-r--r--   0 theneault   (502) staff       (20)        0 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/backend/__init__.py
+-rw-r--r--   0 theneault   (502) staff       (20)     1831 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/backend/base_backend.py
+-rw-r--r--   0 theneault   (502) staff       (20)     8319 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/backend/runtime_endpoint.py
+-rw-r--r--   0 theneault   (502) staff       (20)      797 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/global_config.py
+drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-17 09:13:29.159946 dblcsgen-0.2.2.dev0/sglang/lang/
+-rw-r--r--   0 theneault   (502) staff       (20)        0 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/lang/__init__.py
+-rw-r--r--   0 theneault   (502) staff       (20)     9633 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/lang/chat_template.py
+-rw-r--r--   0 theneault   (502) staff       (20)     7527 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/lang/compiler.py
+-rw-r--r--   0 theneault   (502) staff       (20)    26999 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/lang/interpreter.py
+-rw-r--r--   0 theneault   (502) staff       (20)    13320 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/lang/ir.py
+-rw-r--r--   0 theneault   (502) staff       (20)     8260 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/lang/tracer.py
+-rw-r--r--   0 theneault   (502) staff       (20)      433 2024-04-16 18:25:50.000000 dblcsgen-0.2.2.dev0/sglang/launch_server.py
+drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-17 09:13:29.162740 dblcsgen-0.2.2.dev0/sglang/srt/
+-rw-r--r--   0 theneault   (502) staff       (20)      227 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/backend_config.py
+drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-17 09:13:29.163402 dblcsgen-0.2.2.dev0/sglang/srt/constrained/
+-rw-r--r--   0 theneault   (502) staff       (20)     1236 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/constrained/__init__.py
+-rw-r--r--   0 theneault   (502) staff       (20)     1405 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/constrained/base_cache.py
+-rw-r--r--   0 theneault   (502) staff       (20)      902 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/constrained/fsm_cache.py
+-rw-r--r--   0 theneault   (502) staff       (20)     2482 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/constrained/jump_forward.py
+-rw-r--r--   0 theneault   (502) staff       (20)    15496 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/conversation.py
+-rw-r--r--   0 theneault   (502) staff       (20)     5285 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/hf_transformers_utils.py
+drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-17 09:13:29.164864 dblcsgen-0.2.2.dev0/sglang/srt/layers/
+-rw-r--r--   0 theneault   (502) staff       (20)     5209 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/layers/context_flashattention_nopad.py
+-rw-r--r--   0 theneault   (502) staff       (20)    12622 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/layers/extend_attention.py
+-rw-r--r--   0 theneault   (502) staff       (20)     6887 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/layers/logits_processor.py
+-rw-r--r--   0 theneault   (502) staff       (20)     5597 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/layers/radix_attention.py
+-rw-r--r--   0 theneault   (502) staff       (20)     8516 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/layers/token_attention.py
+drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-17 09:13:29.165654 dblcsgen-0.2.2.dev0/sglang/srt/managers/
+-rw-r--r--   0 theneault   (502) staff       (20)     3292 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/managers/detokenizer_manager.py
+-rw-r--r--   0 theneault   (502) staff       (20)     3670 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/managers/io_struct.py
+-rw-r--r--   0 theneault   (502) staff       (20)     4563 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/managers/openai_protocol.py
+drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-17 09:13:29.167650 dblcsgen-0.2.2.dev0/sglang/srt/managers/router/
+-rw-r--r--   0 theneault   (502) staff       (20)    19922 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/managers/router/infer_batch.py
+-rw-r--r--   0 theneault   (502) staff       (20)     2682 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/managers/router/manager.py
+-rw-r--r--   0 theneault   (502) staff       (20)    28007 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/managers/router/model_rpc.py
+-rw-r--r--   0 theneault   (502) staff       (20)    16926 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/managers/router/model_runner.py
+-rw-r--r--   0 theneault   (502) staff       (20)     6484 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/managers/router/radix_cache.py
+-rw-r--r--   0 theneault   (502) staff       (20)     2818 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/managers/router/scheduler.py
+-rw-r--r--   0 theneault   (502) staff       (20)     9743 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/managers/tokenizer_manager.py
+-rw-r--r--   0 theneault   (502) staff       (20)     3609 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/memory_pool.py
+-rw-r--r--   0 theneault   (502) staff       (20)     8889 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/mm_utils.py
+-rw-r--r--   0 theneault   (502) staff       (20)     1546 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/model_config.py
+drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-17 09:13:29.170590 dblcsgen-0.2.2.dev0/sglang/srt/models/
+-rw-r--r--   0 theneault   (502) staff       (20)    14112 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/models/dbrx.py
+-rw-r--r--   0 theneault   (502) staff       (20)    11071 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/models/dbrx_config.py
+-rw-r--r--   0 theneault   (502) staff       (20)    11587 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/models/gemma.py
+-rw-r--r--   0 theneault   (502) staff       (20)    11611 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/models/llama2.py
+-rw-r--r--   0 theneault   (502) staff       (20)    14922 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/models/llava.py
+-rw-r--r--   0 theneault   (502) staff       (20)      254 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/models/mistral.py
+-rw-r--r--   0 theneault   (502) staff       (20)    13915 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/models/mixtral.py
+-rw-r--r--   0 theneault   (502) staff       (20)     9225 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/models/qwen.py
+-rw-r--r--   0 theneault   (502) staff       (20)    11307 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/models/qwen2.py
+-rw-r--r--   0 theneault   (502) staff       (20)    10816 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/models/stablelm.py
+-rw-r--r--   0 theneault   (502) staff       (20)     4414 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/models/yivl.py
+-rw-r--r--   0 theneault   (502) staff       (20)     2896 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/sampling_params.py
+-rw-r--r--   0 theneault   (502) staff       (20)    27702 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/server.py
+-rw-r--r--   0 theneault   (502) staff       (20)     9143 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/server_args.py
+-rw-r--r--   0 theneault   (502) staff       (20)     7582 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/srt/utils.py
+drwxr-xr-x   0 theneault   (502) staff       (20)        0 2024-04-17 09:13:29.171574 dblcsgen-0.2.2.dev0/sglang/test/
+-rw-r--r--   0 theneault   (502) staff       (20)     1592 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/test/test_conversation.py
+-rw-r--r--   0 theneault   (502) staff       (20)     1657 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/test/test_openai_protocol.py
+-rw-r--r--   0 theneault   (502) staff       (20)    11421 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/test/test_programs.py
+-rw-r--r--   0 theneault   (502) staff       (20)     4830 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/test/test_utils.py
+-rw-r--r--   0 theneault   (502) staff       (20)     6237 2024-04-13 18:48:15.000000 dblcsgen-0.2.2.dev0/sglang/utils.py
```

### Comparing `dblcsgen-0.2.1/LICENSE` & `dblcsgen-0.2.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/PKG-INFO` & `dblcsgen-0.2.2.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dblcsgen
-Version: 0.2.1
+Version: 0.2.2.dev0
 Summary: DBLC Fast Structured Generation
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -222,15 +222,15 @@
 Requires-Dist: uvloop; extra == "srt"
 Requires-Dist: uvicorn; extra == "srt"
 Requires-Dist: zmq; extra == "srt"
 Requires-Dist: vllm>=0.3.3; extra == "srt"
 Requires-Dist: interegular; extra == "srt"
 Requires-Dist: pydantic; extra == "srt"
 Requires-Dist: pillow; extra == "srt"
-Requires-Dist: outlines>=0.0.27; extra == "srt"
+Requires-Dist: outlines==0.0.34; extra == "srt"
 Provides-Extra: all
 Requires-Dist: sglang[srt]; extra == "all"
 
 <div align="center">
 <img src="assets/logo.png" alt="logo" width="400"></img>
 </div>
```

### Comparing `dblcsgen-0.2.1/README.md` & `dblcsgen-0.2.2.dev0/README.md`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/dblcsgen.egg-info/PKG-INFO` & `dblcsgen-0.2.2.dev0/dblcsgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dblcsgen
-Version: 0.2.1
+Version: 0.2.2.dev0
 Summary: DBLC Fast Structured Generation
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -222,15 +222,15 @@
 Requires-Dist: uvloop; extra == "srt"
 Requires-Dist: uvicorn; extra == "srt"
 Requires-Dist: zmq; extra == "srt"
 Requires-Dist: vllm>=0.3.3; extra == "srt"
 Requires-Dist: interegular; extra == "srt"
 Requires-Dist: pydantic; extra == "srt"
 Requires-Dist: pillow; extra == "srt"
-Requires-Dist: outlines>=0.0.27; extra == "srt"
+Requires-Dist: outlines==0.0.34; extra == "srt"
 Provides-Extra: all
 Requires-Dist: sglang[srt]; extra == "all"
 
 <div align="center">
 <img src="assets/logo.png" alt="logo" width="400"></img>
 </div>
```

### Comparing `dblcsgen-0.2.1/dblcsgen.egg-info/SOURCES.txt` & `dblcsgen-0.2.2.dev0/dblcsgen.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,19 +8,16 @@
 dblcsgen.egg-info/top_level.txt
 sglang/__init__.py
 sglang/api.py
 sglang/global_config.py
 sglang/launch_server.py
 sglang/utils.py
 sglang/backend/__init__.py
-sglang/backend/anthropic.py
 sglang/backend/base_backend.py
-sglang/backend/openai.py
 sglang/backend/runtime_endpoint.py
-sglang/backend/vertexai.py
 sglang/lang/__init__.py
 sglang/lang/chat_template.py
 sglang/lang/compiler.py
 sglang/lang/interpreter.py
 sglang/lang/ir.py
 sglang/lang/tracer.py
 sglang/srt/backend_config.py
```

### Comparing `dblcsgen-0.2.1/pyproject.toml` & `dblcsgen-0.2.2.dev0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dblcsgen"
-version = "0.2.1"
+version = "0.2.2.dev0"
 description = "DBLC Fast Structured Generation"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
@@ -16,15 +16,15 @@
 dependencies = [
     "requests",
     "tqdm",
 ]
 
 [project.optional-dependencies]
 srt = ["aiohttp", "fastapi", "psutil", "rpyc", "torch", "uvloop", "uvicorn",
-       "zmq", "vllm>=0.3.3", "interegular", "pydantic", "pillow", "outlines>=0.0.27"]
+       "zmq", "vllm>=0.3.3", "interegular", "pydantic", "pillow", "outlines==0.0.34"]
 all = ["sglang[srt]"]
 
 [project.urls]
 "Homepage" = "https://github.com/sgl-project/sglang"
 "Bug Tracker" = "https://github.com/sgl-project/sglang/issues"
 
 [tool.setuptools.packages.find]
```

### Comparing `dblcsgen-0.2.1/sglang/api.py` & `dblcsgen-0.2.2.dev0/sglang/api.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/backend/base_backend.py` & `dblcsgen-0.2.2.dev0/sglang/backend/base_backend.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/backend/runtime_endpoint.py` & `dblcsgen-0.2.2.dev0/sglang/backend/runtime_endpoint.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/global_config.py` & `dblcsgen-0.2.2.dev0/sglang/global_config.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/lang/chat_template.py` & `dblcsgen-0.2.2.dev0/sglang/lang/chat_template.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/lang/compiler.py` & `dblcsgen-0.2.2.dev0/sglang/lang/compiler.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/lang/interpreter.py` & `dblcsgen-0.2.2.dev0/sglang/lang/interpreter.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/lang/ir.py` & `dblcsgen-0.2.2.dev0/sglang/lang/ir.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/lang/tracer.py` & `dblcsgen-0.2.2.dev0/sglang/lang/tracer.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/constrained/__init__.py` & `dblcsgen-0.2.2.dev0/sglang/srt/constrained/__init__.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/constrained/base_cache.py` & `dblcsgen-0.2.2.dev0/sglang/srt/constrained/base_cache.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/constrained/fsm_cache.py` & `dblcsgen-0.2.2.dev0/sglang/srt/constrained/fsm_cache.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/constrained/jump_forward.py` & `dblcsgen-0.2.2.dev0/sglang/srt/constrained/jump_forward.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/conversation.py` & `dblcsgen-0.2.2.dev0/sglang/srt/conversation.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/hf_transformers_utils.py` & `dblcsgen-0.2.2.dev0/sglang/srt/hf_transformers_utils.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/layers/context_flashattention_nopad.py` & `dblcsgen-0.2.2.dev0/sglang/srt/layers/context_flashattention_nopad.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/layers/extend_attention.py` & `dblcsgen-0.2.2.dev0/sglang/srt/layers/extend_attention.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/layers/logits_processor.py` & `dblcsgen-0.2.2.dev0/sglang/srt/layers/logits_processor.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/layers/radix_attention.py` & `dblcsgen-0.2.2.dev0/sglang/srt/layers/radix_attention.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/layers/token_attention.py` & `dblcsgen-0.2.2.dev0/sglang/srt/layers/token_attention.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/managers/detokenizer_manager.py` & `dblcsgen-0.2.2.dev0/sglang/srt/managers/detokenizer_manager.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/managers/io_struct.py` & `dblcsgen-0.2.2.dev0/sglang/srt/managers/io_struct.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/managers/openai_protocol.py` & `dblcsgen-0.2.2.dev0/sglang/srt/managers/openai_protocol.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/managers/router/infer_batch.py` & `dblcsgen-0.2.2.dev0/sglang/srt/managers/router/infer_batch.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/managers/router/manager.py` & `dblcsgen-0.2.2.dev0/sglang/srt/managers/router/manager.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/managers/router/model_rpc.py` & `dblcsgen-0.2.2.dev0/sglang/srt/managers/router/model_rpc.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/managers/router/model_runner.py` & `dblcsgen-0.2.2.dev0/sglang/srt/managers/router/model_runner.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/managers/router/radix_cache.py` & `dblcsgen-0.2.2.dev0/sglang/srt/managers/router/radix_cache.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/managers/router/scheduler.py` & `dblcsgen-0.2.2.dev0/sglang/srt/managers/router/scheduler.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/managers/tokenizer_manager.py` & `dblcsgen-0.2.2.dev0/sglang/srt/managers/tokenizer_manager.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/memory_pool.py` & `dblcsgen-0.2.2.dev0/sglang/srt/memory_pool.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/mm_utils.py` & `dblcsgen-0.2.2.dev0/sglang/srt/mm_utils.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/model_config.py` & `dblcsgen-0.2.2.dev0/sglang/srt/model_config.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/models/dbrx.py` & `dblcsgen-0.2.2.dev0/sglang/srt/models/dbrx.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/models/dbrx_config.py` & `dblcsgen-0.2.2.dev0/sglang/srt/models/dbrx_config.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/models/gemma.py` & `dblcsgen-0.2.2.dev0/sglang/srt/models/gemma.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/models/llama2.py` & `dblcsgen-0.2.2.dev0/sglang/srt/models/llama2.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/models/llava.py` & `dblcsgen-0.2.2.dev0/sglang/srt/models/llava.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/models/mixtral.py` & `dblcsgen-0.2.2.dev0/sglang/srt/models/mixtral.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/models/qwen.py` & `dblcsgen-0.2.2.dev0/sglang/srt/models/qwen.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/models/qwen2.py` & `dblcsgen-0.2.2.dev0/sglang/srt/models/qwen2.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/models/stablelm.py` & `dblcsgen-0.2.2.dev0/sglang/srt/models/stablelm.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/models/yivl.py` & `dblcsgen-0.2.2.dev0/sglang/srt/models/yivl.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/sampling_params.py` & `dblcsgen-0.2.2.dev0/sglang/srt/sampling_params.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/server.py` & `dblcsgen-0.2.2.dev0/sglang/srt/server.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/server_args.py` & `dblcsgen-0.2.2.dev0/sglang/srt/server_args.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/srt/utils.py` & `dblcsgen-0.2.2.dev0/sglang/srt/utils.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/test/test_conversation.py` & `dblcsgen-0.2.2.dev0/sglang/test/test_conversation.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/test/test_openai_protocol.py` & `dblcsgen-0.2.2.dev0/sglang/test/test_openai_protocol.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/test/test_programs.py` & `dblcsgen-0.2.2.dev0/sglang/test/test_programs.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/test/test_utils.py` & `dblcsgen-0.2.2.dev0/sglang/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.1/sglang/utils.py` & `dblcsgen-0.2.2.dev0/sglang/utils.py`

 * *Files identical despite different names*

