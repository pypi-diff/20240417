# Comparing `tmp/qwen-agent-0.0.1.tar.gz` & `tmp/qwen-agent-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwen-agent-0.0.1.tar", last modified: Sun Apr  7 13:10:00 2024, max compression
+gzip compressed data, was "qwen-agent-0.0.2.tar", last modified: Wed Apr 17 06:08:26 2024, max compression
```

## Comparing `qwen-agent-0.0.1.tar` & `qwen-agent-0.0.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 13:10:00.611123 qwen-agent-0.0.1/
--rw-r--r--   0 tujianhong   (502) staff       (20)     6897 2024-04-07 07:48:44.000000 qwen-agent-0.0.1/LICENSE
--rw-r--r--   0 tujianhong   (502) staff       (20)       85 2024-04-07 13:01:29.000000 qwen-agent-0.0.1/MANIFEST.in
--rw-r--r--   0 tujianhong   (502) staff       (20)      124 2024-04-07 13:10:00.609840 qwen-agent-0.0.1/PKG-INFO
--rw-r--r--   0 tujianhong   (502) staff       (20)     8736 2024-04-07 07:48:44.000000 qwen-agent-0.0.1/README.md
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 13:10:00.484329 qwen-agent-0.0.1/qwen_agent/
--rw-r--r--   0 tujianhong   (502) staff       (20)       46 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/__init__.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     8672 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/agent.py
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 13:10:00.490680 qwen-agent-0.0.1/qwen_agent/agents/
--rw-r--r--   0 tujianhong   (502) staff       (20)      626 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/agents/__init__.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     1598 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/agents/article_agent.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     2780 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/agents/assistant.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     1766 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/agents/docqa_agent.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     4155 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/agents/fncall_agent.py
--rw-r--r--   0 tujianhong   (502) staff       (20)    13817 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/agents/group_chat.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     3496 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/agents/group_chat_auto_router.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     6592 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/agents/group_chat_creator.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     7873 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/agents/react_chat.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     4204 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/agents/router.py
--rw-r--r--   0 tujianhong   (502) staff       (20)      504 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/agents/user_agent.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     3956 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/agents/write_from_scratch.py
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 13:10:00.537865 qwen-agent-0.0.1/qwen_agent/llm/
--rw-r--r--   0 tujianhong   (502) staff       (20)     1908 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/llm/__init__.py
--rw-r--r--   0 tujianhong   (502) staff       (20)    13188 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/llm/base.py
--rw-r--r--   0 tujianhong   (502) staff       (20)    13002 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/llm/function_calling.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     4269 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/llm/oai.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     6404 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/llm/qwen_dashscope.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     3012 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/llm/qwenvl_dashscope.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     3322 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/llm/schema.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     1596 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/llm/text_base.py
--rw-r--r--   0 tujianhong   (502) staff       (20)      599 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/log.py
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 13:10:00.539488 qwen-agent-0.0.1/qwen_agent/memory/
--rw-r--r--   0 tujianhong   (502) staff       (20)       49 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/memory/__init__.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     4097 2024-04-07 13:01:29.000000 qwen-agent-0.0.1/qwen_agent/memory/memory.py
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 13:10:00.547631 qwen-agent-0.0.1/qwen_agent/prompts/
--rw-r--r--   0 tujianhong   (502) staff       (20)      368 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/prompts/__init__.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     1343 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/prompts/continue_writing.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     1107 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/prompts/doc_qa.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     2248 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/prompts/expand_writing.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     3248 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/prompts/gen_keyword.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     1495 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/prompts/outline_writing.py
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 13:10:00.559253 qwen-agent-0.0.1/qwen_agent/tools/
--rw-r--r--   0 tujianhong   (502) staff       (20)      714 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/tools/__init__.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     2021 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/tools/amap_weather.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     3141 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/tools/base.py
--rw-r--r--   0 tujianhong   (502) staff       (20)    12040 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/tools/code_interpreter.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     5351 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/tools/doc_parser.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     1123 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/tools/image_gen.py
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 13:10:00.592799 qwen-agent-0.0.1/qwen_agent/tools/resource/
--rw-r--r--   0 tujianhong   (502) staff       (20)  8559848 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/tools/resource/AlibabaPuHuiTi-3-45-Light.ttf
--rw-r--r--   0 tujianhong   (502) staff       (20)     1169 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/tools/resource/code_interpreter_init_kernel.py
--rw-r--r--   0 tujianhong   (502) staff       (20)      553 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/tools/resource/image_service.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     3627 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/tools/retrieval.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     4898 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/tools/similarity_search.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     3584 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/tools/storage.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     1376 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/tools/web_extractor.py
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 13:10:00.606868 qwen-agent-0.0.1/qwen_agent/utils/
--rw-r--r--   0 tujianhong   (502) staff       (20)        0 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/utils/__init__.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     2728 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/utils/doc_parser.py
--rw-r--r--   0 tujianhong   (502) staff       (20)  2561218 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/utils/qwen.tiktoken
--rw-r--r--   0 tujianhong   (502) staff       (20)    10526 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/utils/tokenization_qwen.py
--rw-r--r--   0 tujianhong   (502) staff       (20)     9829 2024-04-07 07:48:45.000000 qwen-agent-0.0.1/qwen_agent/utils/utils.py
-drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-07 13:10:00.487155 qwen-agent-0.0.1/qwen_agent.egg-info/
--rw-r--r--   0 tujianhong   (502) staff       (20)      124 2024-04-07 13:10:00.000000 qwen-agent-0.0.1/qwen_agent.egg-info/PKG-INFO
--rw-r--r--   0 tujianhong   (502) staff       (20)     1800 2024-04-07 13:10:00.000000 qwen-agent-0.0.1/qwen_agent.egg-info/SOURCES.txt
--rw-r--r--   0 tujianhong   (502) staff       (20)        1 2024-04-07 13:10:00.000000 qwen-agent-0.0.1/qwen_agent.egg-info/dependency_links.txt
--rw-r--r--   0 tujianhong   (502) staff       (20)      237 2024-04-07 13:10:00.000000 qwen-agent-0.0.1/qwen_agent.egg-info/requires.txt
--rw-r--r--   0 tujianhong   (502) staff       (20)       11 2024-04-07 13:10:00.000000 qwen-agent-0.0.1/qwen_agent.egg-info/top_level.txt
--rw-r--r--   0 tujianhong   (502) staff       (20)       38 2024-04-07 13:10:00.611208 qwen-agent-0.0.1/setup.cfg
--rw-r--r--   0 tujianhong   (502) staff       (20)      585 2024-04-07 13:08:40.000000 qwen-agent-0.0.1/setup.py
+drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-17 06:08:26.410491 qwen-agent-0.0.2/
+-rw-r--r--   0 tujianhong   (502) staff       (20)     6897 2024-04-07 07:48:44.000000 qwen-agent-0.0.2/LICENSE
+-rw-r--r--   0 tujianhong   (502) staff       (20)       85 2024-04-07 13:01:29.000000 qwen-agent-0.0.2/MANIFEST.in
+-rw-r--r--   0 tujianhong   (502) staff       (20)     6240 2024-04-17 06:08:26.409614 qwen-agent-0.0.2/PKG-INFO
+-rw-r--r--   0 tujianhong   (502) staff       (20)     5851 2024-04-17 06:03:40.000000 qwen-agent-0.0.2/README.md
+drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-17 06:08:26.308863 qwen-agent-0.0.2/qwen_agent/
+-rw-r--r--   0 tujianhong   (502) staff       (20)       68 2024-04-17 06:03:40.000000 qwen-agent-0.0.2/qwen_agent/__init__.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     8672 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/agent.py
+drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-17 06:08:26.336956 qwen-agent-0.0.2/qwen_agent/agents/
+-rw-r--r--   0 tujianhong   (502) staff       (20)      626 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/agents/__init__.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1598 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/agents/article_agent.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     2780 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/agents/assistant.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1766 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/agents/docqa_agent.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     4155 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/agents/fncall_agent.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)    13817 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/agents/group_chat.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     3496 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/agents/group_chat_auto_router.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     6592 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/agents/group_chat_creator.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     7873 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/agents/react_chat.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     4204 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/agents/router.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)      504 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/agents/user_agent.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     3956 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/agents/write_from_scratch.py
+drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-17 06:08:26.345991 qwen-agent-0.0.2/qwen_agent/llm/
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1908 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/llm/__init__.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)    13188 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/llm/base.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)    13002 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/llm/function_calling.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     4257 2024-04-17 06:03:40.000000 qwen-agent-0.0.2/qwen_agent/llm/oai.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     6404 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/llm/qwen_dashscope.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     4050 2024-04-17 03:07:41.000000 qwen-agent-0.0.2/qwen_agent/llm/qwenvl_dashscope.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     3322 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/llm/schema.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1596 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/llm/text_base.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)      599 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/log.py
+drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-17 06:08:26.347455 qwen-agent-0.0.2/qwen_agent/memory/
+-rw-r--r--   0 tujianhong   (502) staff       (20)       49 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/memory/__init__.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     4331 2024-04-17 06:03:40.000000 qwen-agent-0.0.2/qwen_agent/memory/memory.py
+drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-17 06:08:26.351756 qwen-agent-0.0.2/qwen_agent/prompts/
+-rw-r--r--   0 tujianhong   (502) staff       (20)      368 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/prompts/__init__.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1343 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/prompts/continue_writing.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1107 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/prompts/doc_qa.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     2248 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/prompts/expand_writing.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     3248 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/prompts/gen_keyword.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1495 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/prompts/outline_writing.py
+drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-17 06:08:26.360671 qwen-agent-0.0.2/qwen_agent/tools/
+-rw-r--r--   0 tujianhong   (502) staff       (20)      714 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/tools/__init__.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     2021 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/tools/amap_weather.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     3141 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/tools/base.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)    12040 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/tools/code_interpreter.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     5351 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/tools/doc_parser.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1123 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/tools/image_gen.py
+drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-17 06:08:26.378143 qwen-agent-0.0.2/qwen_agent/tools/resource/
+-rw-r--r--   0 tujianhong   (502) staff       (20)  8559848 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/tools/resource/AlibabaPuHuiTi-3-45-Light.ttf
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1169 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/tools/resource/code_interpreter_init_kernel.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)      553 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/tools/resource/image_service.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     3627 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/tools/retrieval.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     4898 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/tools/similarity_search.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     3584 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/tools/storage.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1376 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/tools/web_extractor.py
+drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-17 06:08:26.409130 qwen-agent-0.0.2/qwen_agent/utils/
+-rw-r--r--   0 tujianhong   (502) staff       (20)        0 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/utils/__init__.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     2728 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/utils/doc_parser.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)  2561218 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/utils/qwen.tiktoken
+-rw-r--r--   0 tujianhong   (502) staff       (20)    10526 2024-04-07 07:48:45.000000 qwen-agent-0.0.2/qwen_agent/utils/tokenization_qwen.py
+-rw-r--r--   0 tujianhong   (502) staff       (20)     9828 2024-04-17 03:07:41.000000 qwen-agent-0.0.2/qwen_agent/utils/utils.py
+drwxr-xr-x   0 tujianhong   (502) staff       (20)        0 2024-04-17 06:08:26.310683 qwen-agent-0.0.2/qwen_agent.egg-info/
+-rw-r--r--   0 tujianhong   (502) staff       (20)     6240 2024-04-17 06:08:26.000000 qwen-agent-0.0.2/qwen_agent.egg-info/PKG-INFO
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1800 2024-04-17 06:08:26.000000 qwen-agent-0.0.2/qwen_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 tujianhong   (502) staff       (20)        1 2024-04-17 06:08:26.000000 qwen-agent-0.0.2/qwen_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 tujianhong   (502) staff       (20)      237 2024-04-17 06:08:26.000000 qwen-agent-0.0.2/qwen_agent.egg-info/requires.txt
+-rw-r--r--   0 tujianhong   (502) staff       (20)       11 2024-04-17 06:08:26.000000 qwen-agent-0.0.2/qwen_agent.egg-info/top_level.txt
+-rw-r--r--   0 tujianhong   (502) staff       (20)       38 2024-04-17 06:08:26.410552 qwen-agent-0.0.2/setup.cfg
+-rw-r--r--   0 tujianhong   (502) staff       (20)     1444 2024-04-17 06:04:46.000000 qwen-agent-0.0.2/setup.py
```

### Comparing `qwen-agent-0.0.1/LICENSE` & `qwen-agent-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/agent.py` & `qwen-agent-0.0.2/qwen_agent/agent.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/agents/__init__.py` & `qwen-agent-0.0.2/qwen_agent/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/agents/article_agent.py` & `qwen-agent-0.0.2/qwen_agent/agents/article_agent.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/agents/assistant.py` & `qwen-agent-0.0.2/qwen_agent/agents/assistant.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/agents/docqa_agent.py` & `qwen-agent-0.0.2/qwen_agent/agents/docqa_agent.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/agents/fncall_agent.py` & `qwen-agent-0.0.2/qwen_agent/agents/fncall_agent.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/agents/group_chat.py` & `qwen-agent-0.0.2/qwen_agent/agents/group_chat.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/agents/group_chat_auto_router.py` & `qwen-agent-0.0.2/qwen_agent/agents/group_chat_auto_router.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/agents/group_chat_creator.py` & `qwen-agent-0.0.2/qwen_agent/agents/group_chat_creator.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/agents/react_chat.py` & `qwen-agent-0.0.2/qwen_agent/agents/react_chat.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/agents/router.py` & `qwen-agent-0.0.2/qwen_agent/agents/router.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/agents/write_from_scratch.py` & `qwen-agent-0.0.2/qwen_agent/agents/write_from_scratch.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/llm/__init__.py` & `qwen-agent-0.0.2/qwen_agent/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/llm/base.py` & `qwen-agent-0.0.2/qwen_agent/llm/base.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/llm/function_calling.py` & `qwen-agent-0.0.2/qwen_agent/llm/function_calling.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/llm/oai.py` & `qwen-agent-0.0.2/qwen_agent/llm/oai.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import copy
 import os
 from pprint import pformat
 from typing import Dict, Iterator, List, Optional
 
 import openai
 
 if openai.__version__.startswith('0.'):
```

### Comparing `qwen-agent-0.0.1/qwen_agent/llm/qwen_dashscope.py` & `qwen-agent-0.0.2/qwen_agent/llm/qwen_dashscope.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/llm/schema.py` & `qwen-agent-0.0.2/qwen_agent/llm/schema.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/llm/text_base.py` & `qwen-agent-0.0.2/qwen_agent/llm/text_base.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/log.py` & `qwen-agent-0.0.2/qwen_agent/log.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/memory/memory.py` & `qwen-agent-0.0.2/qwen_agent/memory/memory.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,14 +76,19 @@
                     for item in messages[-1].content:
                         if item.text:
                             query += item.text
             if query:
                 # Gen keyword
                 *_, last = self.keygen.run([Message(USER, query)])
                 keyword = last[-1].content
+                keyword = keyword.strip()
+                if keyword.startswith('```json'):
+                    keyword = keyword[len('```json'):]
+                if keyword.endswith('```'):
+                    keyword = keyword[:-3]
                 try:
                     logger.info(keyword)
                     keyword_dict = json5.loads(keyword)
                     keyword_dict['text'] = query
                     query = json.dumps(keyword_dict, ensure_ascii=False)
                 except Exception:
                     query = query
```

### Comparing `qwen-agent-0.0.1/qwen_agent/prompts/continue_writing.py` & `qwen-agent-0.0.2/qwen_agent/prompts/continue_writing.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/prompts/doc_qa.py` & `qwen-agent-0.0.2/qwen_agent/prompts/doc_qa.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/prompts/expand_writing.py` & `qwen-agent-0.0.2/qwen_agent/prompts/expand_writing.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/prompts/gen_keyword.py` & `qwen-agent-0.0.2/qwen_agent/prompts/gen_keyword.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/prompts/outline_writing.py` & `qwen-agent-0.0.2/qwen_agent/prompts/outline_writing.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/tools/__init__.py` & `qwen-agent-0.0.2/qwen_agent/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/tools/amap_weather.py` & `qwen-agent-0.0.2/qwen_agent/tools/amap_weather.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/tools/base.py` & `qwen-agent-0.0.2/qwen_agent/tools/base.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/tools/code_interpreter.py` & `qwen-agent-0.0.2/qwen_agent/tools/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/tools/doc_parser.py` & `qwen-agent-0.0.2/qwen_agent/tools/doc_parser.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/tools/image_gen.py` & `qwen-agent-0.0.2/qwen_agent/tools/image_gen.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/tools/resource/AlibabaPuHuiTi-3-45-Light.ttf` & `qwen-agent-0.0.2/qwen_agent/tools/resource/AlibabaPuHuiTi-3-45-Light.ttf`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/tools/resource/code_interpreter_init_kernel.py` & `qwen-agent-0.0.2/qwen_agent/tools/resource/code_interpreter_init_kernel.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/tools/resource/image_service.py` & `qwen-agent-0.0.2/qwen_agent/tools/resource/image_service.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/tools/retrieval.py` & `qwen-agent-0.0.2/qwen_agent/tools/retrieval.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/tools/similarity_search.py` & `qwen-agent-0.0.2/qwen_agent/tools/similarity_search.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/tools/storage.py` & `qwen-agent-0.0.2/qwen_agent/tools/storage.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/tools/web_extractor.py` & `qwen-agent-0.0.2/qwen_agent/tools/web_extractor.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/utils/doc_parser.py` & `qwen-agent-0.0.2/qwen_agent/utils/doc_parser.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/utils/qwen.tiktoken` & `qwen-agent-0.0.2/qwen_agent/utils/qwen.tiktoken`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/utils/tokenization_qwen.py` & `qwen-agent-0.0.2/qwen_agent/utils/tokenization_qwen.py`

 * *Files identical despite different names*

### Comparing `qwen-agent-0.0.1/qwen_agent/utils/utils.py` & `qwen-agent-0.0.2/qwen_agent/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,15 +278,15 @@
     """
     Text description of function
     """
     tool_desc_template = {
         'zh':
         '### {name_for_human}\n\n{name_for_model}: {description_for_model} 输入参数：{parameters} {args_format}',
         'en':
-        '### {name_for_human}\n\n{name_for_model}: {description_for_model} Parameters：{parameters} {args_format}'
+        '### {name_for_human}\n\n{name_for_model}: {description_for_model} Parameters: {parameters} {args_format}'
     }
     if has_chinese_chars(function):
         tool_desc = tool_desc_template['zh']
     else:
         tool_desc = tool_desc_template['en']
 
     name = function.get('name', None)
```

### Comparing `qwen-agent-0.0.1/qwen_agent.egg-info/SOURCES.txt` & `qwen-agent-0.0.2/qwen_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

