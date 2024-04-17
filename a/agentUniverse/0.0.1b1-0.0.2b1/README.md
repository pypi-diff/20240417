# Comparing `tmp/agentUniverse-0.0.1b1.tar.gz` & `tmp/agentuniverse-0.0.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentUniverse-0.0.1b1.tar", last modified: Fri Apr 12 13:34:29 2024, max compression
+gzip compressed data, was "agentuniverse-0.0.2b1.tar", last modified: Wed Apr 17 10:21:50 2024, max compression
```

## Comparing `agentUniverse-0.0.1b1.tar` & `agentuniverse-0.0.2b1.tar`

### file list

```diff
@@ -1,260 +1,261 @@
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.813884 agentUniverse-0.0.1b1/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)    11335 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/LICENSE
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1984 2024-04-12 13:34:29.813595 agentUniverse-0.0.1b1/PKG-INFO
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1944 2024-04-12 13:32:53.000000 agentUniverse-0.0.1b1/README.md
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.813269 agentUniverse-0.0.1b1/agentUniverse.egg-info/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1984 2024-04-12 13:34:29.000000 agentUniverse-0.0.1b1/agentUniverse.egg-info/PKG-INFO
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     9793 2024-04-12 13:34:29.000000 agentUniverse-0.0.1b1/agentUniverse.egg-info/SOURCES.txt
--rw-r--r--   0 jerry.zzw   (501) staff       (20)        1 2024-04-12 13:34:29.000000 agentUniverse-0.0.1b1/agentUniverse.egg-info/dependency_links.txt
--rw-r--r--   0 jerry.zzw   (501) staff       (20)       68 2024-04-12 13:34:29.000000 agentUniverse-0.0.1b1/agentUniverse.egg-info/top_level.txt
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.765979 agentUniverse-0.0.1b1/agentuniverse/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:12:13.000000 agentUniverse-0.0.1b1/agentuniverse/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.767990 agentUniverse-0.0.1b1/agentuniverse/agent/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/agent/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.768308 agentUniverse-0.0.1b1/agentuniverse/agent/action/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/agent/action/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.769236 agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.769935 agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/embedding/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/embedding/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      959 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/embedding/embedding.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     4460 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/embedding/openai_embedding.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3097 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/knowledge.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      655 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/knowledge_manager.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.770527 agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/reader/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/reader/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.772407 agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/reader/file/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/reader/file/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1160 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/reader/file/docx_reader.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1638 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/reader/file/file_reader.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1568 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/reader/file/pdf_reader.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1460 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/reader/file/pptx_reader.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1465 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/reader/file/web_pdf_reader.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      552 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/reader/reader.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.773500 agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/store/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/store/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     4648 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/store/chroma_store.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1971 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/store/document.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      662 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/store/query.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3190 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/store/store.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.774411 agentUniverse-0.0.1b1/agentuniverse/agent/action/tool/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/agent/action/tool/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      276 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/agent/action/tool/enum.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3855 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/action/tool/tool.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      626 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/action/tool/tool_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     5371 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      639 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/agent_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      526 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/agent/agent_model.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.777331 agentUniverse-0.0.1b1/agentuniverse/agent/default/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/agent/default/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3034 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/default/executing_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      365 2024-04-12 13:26:06.000000 agentUniverse-0.0.1b1/agentuniverse/agent/default/executing_agent.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1937 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/default/expressing_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      362 2024-04-12 13:26:06.000000 agentUniverse-0.0.1b1/agentuniverse/agent/default/expressing_agent.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1532 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/default/planning_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      352 2024-04-12 13:26:06.000000 agentUniverse-0.0.1b1/agentuniverse/agent/default/planning_agent.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1247 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/default/rag_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      266 2024-04-12 13:26:06.000000 agentUniverse-0.0.1b1/agentuniverse/agent/default/rag_agent.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1862 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/default/reviewing_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      357 2024-04-12 13:26:06.000000 agentUniverse-0.0.1b1/agentuniverse/agent/default/reviewing_agent.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      657 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/agent/input_object.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.779514 agentUniverse-0.0.1b1/agentuniverse/agent/memory/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-09 07:08:39.000000 agentUniverse-0.0.1b1/agentuniverse/agent/memory/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3675 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/memory/chat_memory.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      402 2024-04-01 06:19:56.000000 agentUniverse-0.0.1b1/agentuniverse/agent/memory/enum.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     7755 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/memory/langchain_instance.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3042 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/memory/memory.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      635 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/memory/memory_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      508 2024-04-09 16:15:17.000000 agentUniverse-0.0.1b1/agentuniverse/agent/memory/message.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1759 2024-04-09 06:57:56.000000 agentUniverse-0.0.1b1/agentuniverse/agent/memory/prompt.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      572 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/agent/output_object.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.779789 agentUniverse-0.0.1b1/agentuniverse/agent/plan/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/agent/plan/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.780624 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.781619 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/executing_planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/executing_planner/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3103 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/executing_planner/executing_planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      195 2024-04-12 13:26:06.000000 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/executing_planner/executing_planner.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1287 2024-04-09 16:15:17.000000 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/executing_planner/prompt.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.782679 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/expressing_planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/expressing_planner/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3040 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      200 2024-04-12 13:26:06.000000 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1493 2024-04-09 16:15:17.000000 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/expressing_planner/prompt.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.783575 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/peer_planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      158 2024-04-09 16:15:17.000000 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/peer_planner/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     7621 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/peer_planner/peer_planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      170 2024-04-12 13:26:06.000000 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/peer_planner/peer_planner.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     6397 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      659 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/planner_manager.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.784582 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/planning_planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/planning_planner/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2987 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/planning_planner/planning_planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      190 2024-04-12 13:26:06.000000 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/planning_planner/planning_planner.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1178 2024-04-09 16:15:17.000000 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/planning_planner/prompt.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.785435 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/rag_planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/rag_planner/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      675 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/rag_planner/prompt.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2784 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/rag_planner/rag_planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-12 13:26:06.000000 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/rag_planner/rag_planner.yaml
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.786301 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/reviewing_planner/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/reviewing_planner/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1212 2024-04-09 16:15:17.000000 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/reviewing_planner/prompt.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3041 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      195 2024-04-12 13:26:06.000000 agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.yaml
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.787293 agentUniverse-0.0.1b1/agentuniverse/agent_serve/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)        0 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/agent_serve/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1944 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/agent_serve/service.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3152 2024-04-12 13:26:06.000000 agentUniverse-0.0.1b1/agentuniverse/agent_serve/service_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1161 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/agent_serve/service_instance.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      402 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/agent_serve/service_manager.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.788901 agentUniverse-0.0.1b1/agentuniverse/agent_serve/web/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/agent_serve/web/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.789274 agentUniverse-0.0.1b1/agentuniverse/agent_serve/web/dal/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/agent_serve/web/dal/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.789741 agentUniverse-0.0.1b1/agentuniverse/agent_serve/web/dal/entity/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/agent_serve/web/dal/entity/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1075 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/agent_serve/web/dal/entity/request_do.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     5231 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent_serve/web/dal/request_library.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     9326 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent_serve/web/request_task.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1146 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/agent_serve/web/thread_with_result.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2573 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent_serve/web/web_booster.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     5064 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/agent_serve/web/web_server.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2434 2024-04-09 16:15:17.000000 agentUniverse-0.0.1b1/agentuniverse/agent_serve/web/web_util.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.790393 agentUniverse-0.0.1b1/agentuniverse/base/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/base/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     9452 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/base/agentuniverse.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.791079 agentUniverse-0.0.1b1/agentuniverse/base/annotation/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/base/annotation/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      515 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/base/annotation/singleton.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.792524 agentUniverse-0.0.1b1/agentuniverse/base/component/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/base/component/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1081 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/base/component/application_component_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1264 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/base/component/component_base.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     4129 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/base/component/component_configer_util.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      604 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/base/component/component_enum.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2576 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/base/component/component_manager_base.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.793185 agentUniverse-0.0.1b1/agentuniverse/base/config/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/base/config/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.794043 agentUniverse-0.0.1b1/agentuniverse/base/config/application_configer/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/base/config/application_configer/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3885 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/base/config/application_configer/app_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1006 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/base/config/application_configer/application_config_manager.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.794692 agentUniverse-0.0.1b1/agentuniverse/base/config/component_configer/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/base/config/component_configer/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2557 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/base/config/component_configer/component_configer.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.796212 agentUniverse-0.0.1b1/agentuniverse/base/config/component_configer/configers/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/base/config/component_configer/configers/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2599 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/base/config/component_configer/configers/agent_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2053 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/base/config/component_configer/configers/knowledge_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3272 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/base/config/component_configer/configers/llm_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2540 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/base/config/component_configer/configers/memory_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2392 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/base/config/component_configer/configers/planner_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2192 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/base/config/component_configer/configers/tool_configer.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      423 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/base/config/config_type_enum.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     4828 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/base/config/configer.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.796669 agentUniverse-0.0.1b1/agentuniverse/base/config/custom_configer/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/base/config/custom_configer/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      707 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/base/config/custom_configer/custom_key_configer.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.797372 agentUniverse-0.0.1b1/agentuniverse/base/context/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/base/context/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1447 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/base/context/framework_context.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2768 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/base/context/framework_context_manager.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.798763 agentUniverse-0.0.1b1/agentuniverse/base/util/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/base/util/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      307 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/base/util/env_util.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.799906 agentUniverse-0.0.1b1/agentuniverse/base/util/logging/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/base/util/logging/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     6600 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/base/util/logging/general_logger.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     5132 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/base/util/logging/logging_config.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     6395 2024-04-12 13:26:06.000000 agentUniverse-0.0.1b1/agentuniverse/base/util/logging/logging_util.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      502 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/base/util/memory_util.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     6379 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/base/util/prompt_util.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      715 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/base/util/system_util.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.801386 agentUniverse-0.0.1b1/agentuniverse/llm/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/llm/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.802179 agentUniverse-0.0.1b1/agentuniverse/llm/default/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/llm/default/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1422 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/llm/default/default_openai_llm.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      223 2024-04-12 13:26:06.000000 agentUniverse-0.0.1b1/agentuniverse/llm/default/default_openai_llm.yaml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2911 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/llm/langchain_instance.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     4946 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/llm/llm.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      619 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/llm/llm_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      328 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/llm/llm_output.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     4514 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/llm/openai_llm.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.802738 agentUniverse-0.0.1b1/agentuniverse/prompt/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/prompt/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1931 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/agentuniverse/prompt/prompt.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      834 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse/prompt/prompt_model.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.802920 agentUniverse-0.0.1b1/agentuniverse_connector/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:12:13.000000 agentUniverse-0.0.1b1/agentuniverse_connector/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.803184 agentUniverse-0.0.1b1/agentuniverse_extension/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:13:12.000000 agentUniverse-0.0.1b1/agentuniverse_extension/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.803686 agentUniverse-0.0.1b1/agentuniverse_extension/logger/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse_extension/logger/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     7321 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/agentuniverse_extension/logger/sls_sink.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     2160 2024-04-12 13:26:06.000000 agentUniverse-0.0.1b1/pyproject.toml
--rw-r--r--   0 jerry.zzw   (501) staff       (20)       38 2024-04-12 13:34:29.813932 agentUniverse-0.0.1b1/setup.cfg
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      911 2024-04-12 13:34:13.000000 agentUniverse-0.0.1b1/setup.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.803926 agentUniverse-0.0.1b1/tests/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:13:12.000000 agentUniverse-0.0.1b1/tests/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.804095 agentUniverse-0.0.1b1/tests/test_agentuniverse/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.804382 agentUniverse-0.0.1b1/tests/test_agentuniverse/mock/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse/mock/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.805412 agentUniverse-0.0.1b1/tests/test_agentuniverse/mock/agent_serve/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse/mock/agent_serve/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      535 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse/mock/agent_serve/mock_agent.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      475 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse/mock/agent_serve/mock_application_config_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      896 2024-04-12 13:26:06.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse/mock/agent_serve/mock_service_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      509 2024-04-12 13:26:06.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse/mock/agent_serve/mock_simple_service.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.805650 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.806060 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/agent/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/agent/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.806339 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/agent/action/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/agent/action/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.806876 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/agent/action/knowledge/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/agent/action/knowledge/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.807358 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/agent/action/knowledge/embedding/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/agent/action/knowledge/embedding/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1097 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/agent/action/knowledge/embedding/test_embedding.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1566 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/agent/action/knowledge/test_knowledge.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.807914 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/agent/memory/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/agent/memory/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     3894 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/agent/memory/test_memory.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      776 2024-04-12 13:27:46.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/agent/test_agent.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.809213 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/agent_serve/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/agent_serve/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1237 2024-04-12 13:26:06.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/agent_serve/test_service.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      920 2024-04-12 13:26:06.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/agent_serve/test_service_instance.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1613 2024-04-12 13:26:06.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/agent_serve/test_service_manager.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      524 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/agent_serve/test_web_booster.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.809435 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/base/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/base/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.809990 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/base/context/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/base/context/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1442 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/base/context/test_framework_context.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.810247 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/base/util/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/base/util/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.810649 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/base/util/logging/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/base/util/logging/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1670 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/base/util/logging/test_logging_util.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.811107 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/llm/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/llm/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1264 2024-04-12 13:21:51.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/llm/test_llm.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.811386 agentUniverse-0.0.1b1/tests/test_agentuniverse_connector/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse_connector/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.811678 agentUniverse-0.0.1b1/tests/test_agentuniverse_extension/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse_extension/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.811985 agentUniverse-0.0.1b1/tests/test_agentuniverse_extension/mock/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse_extension/mock/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.812398 agentUniverse-0.0.1b1/tests/test_agentuniverse_extension/mock/logger/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse_extension/mock/logger/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      620 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse_extension/mock/logger/mock_log_client.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.812593 agentUniverse-0.0.1b1/tests/test_agentuniverse_extension/unit/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse_extension/unit/__init__.py
-drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-12 13:34:29.812991 agentUniverse-0.0.1b1/tests/test_agentuniverse_extension/unit/logger/
--rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse_extension/unit/logger/__init__.py
--rw-r--r--   0 jerry.zzw   (501) staff       (20)     1288 2024-04-12 13:26:06.000000 agentUniverse-0.0.1b1/tests/test_agentuniverse_extension/unit/logger/test_sls_sink.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.257498 agentuniverse-0.0.2b1/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)    11335 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/LICENSE
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2723 2024-04-17 10:21:50.257058 agentuniverse-0.0.2b1/PKG-INFO
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1944 2024-04-12 13:32:53.000000 agentuniverse-0.0.2b1/README.md
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.256647 agentuniverse-0.0.2b1/agentUniverse.egg-info/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2723 2024-04-17 10:21:50.000000 agentuniverse-0.0.2b1/agentUniverse.egg-info/PKG-INFO
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     9829 2024-04-17 10:21:50.000000 agentuniverse-0.0.2b1/agentUniverse.egg-info/SOURCES.txt
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)        1 2024-04-17 10:21:50.000000 agentuniverse-0.0.2b1/agentUniverse.egg-info/dependency_links.txt
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      362 2024-04-17 10:21:50.000000 agentuniverse-0.0.2b1/agentUniverse.egg-info/requires.txt
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)       68 2024-04-17 10:21:50.000000 agentuniverse-0.0.2b1/agentUniverse.egg-info/top_level.txt
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.225573 agentuniverse-0.0.2b1/agentuniverse/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:12:13.000000 agentuniverse-0.0.2b1/agentuniverse/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.226498 agentuniverse-0.0.2b1/agentuniverse/agent/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.226653 agentuniverse-0.0.2b1/agentuniverse/agent/action/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.227144 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.227609 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/embedding/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/embedding/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      959 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/embedding/embedding.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     4460 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/embedding/openai_embedding.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3097 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/knowledge.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      655 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/knowledge_manager.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.227910 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.228812 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/file/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/file/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1160 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/file/docx_reader.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1638 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/file/file_reader.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1568 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/file/pdf_reader.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1460 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/file/pptx_reader.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1465 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/file/web_pdf_reader.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      552 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/reader.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.229569 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/store/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/store/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     4648 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/store/chroma_store.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1971 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/store/document.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      662 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/store/query.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3190 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/store/store.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.230157 agentuniverse-0.0.2b1/agentuniverse/agent/action/tool/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/tool/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      276 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/tool/enum.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3855 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/tool/tool.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      626 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/action/tool/tool_manager.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     5371 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/agent.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      639 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/agent_manager.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      526 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/agent_model.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.231772 agentuniverse-0.0.2b1/agentuniverse/agent/default/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/default/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3034 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/default/executing_agent.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      365 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/agentuniverse/agent/default/executing_agent.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1937 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/default/expressing_agent.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      362 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/agentuniverse/agent/default/expressing_agent.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1532 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/default/planning_agent.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      352 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/agentuniverse/agent/default/planning_agent.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1247 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/default/rag_agent.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      266 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/agentuniverse/agent/default/rag_agent.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1862 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/default/reviewing_agent.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      357 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/agentuniverse/agent/default/reviewing_agent.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      657 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/input_object.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.232961 agentuniverse-0.0.2b1/agentuniverse/agent/memory/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-09 07:08:39.000000 agentuniverse-0.0.2b1/agentuniverse/agent/memory/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3675 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/memory/chat_memory.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      402 2024-04-01 06:19:56.000000 agentuniverse-0.0.2b1/agentuniverse/agent/memory/enum.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     7755 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/memory/langchain_instance.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3042 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/memory/memory.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      635 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/memory/memory_manager.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      508 2024-04-09 16:15:17.000000 agentuniverse-0.0.2b1/agentuniverse/agent/memory/message.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1759 2024-04-09 06:57:56.000000 agentuniverse-0.0.2b1/agentuniverse/agent/memory/prompt.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      572 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/output_object.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.233116 agentuniverse-0.0.2b1/agentuniverse/agent/plan/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.233550 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.234170 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/executing_planner/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/executing_planner/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3103 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/executing_planner/executing_planner.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      195 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/executing_planner/executing_planner.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1287 2024-04-09 16:15:17.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/executing_planner/prompt.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.234771 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/expressing_planner/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/expressing_planner/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3040 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      200 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1493 2024-04-09 16:15:17.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/expressing_planner/prompt.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.235220 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/peer_planner/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      158 2024-04-09 16:15:17.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/peer_planner/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     7621 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/peer_planner/peer_planner.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      170 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/peer_planner/peer_planner.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     6397 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/planner.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      659 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/planner_manager.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.235814 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/planning_planner/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/planning_planner/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2987 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/planning_planner/planning_planner.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      190 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/planning_planner/planning_planner.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1178 2024-04-09 16:15:17.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/planning_planner/prompt.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.236411 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/rag_planner/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/rag_planner/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      675 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/rag_planner/prompt.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2784 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/rag_planner/rag_planner.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/rag_planner/rag_planner.yaml
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.237008 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/reviewing_planner/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      157 2024-04-09 16:15:17.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/reviewing_planner/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1212 2024-04-09 16:15:17.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/reviewing_planner/prompt.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3041 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      195 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.yaml
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.237748 agentuniverse-0.0.2b1/agentuniverse/agent_serve/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)        0 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent_serve/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1944 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent_serve/service.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3152 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/agentuniverse/agent_serve/service_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1161 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent_serve/service_instance.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      402 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent_serve/service_manager.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.238660 agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.238970 agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/dal/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/dal/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.239273 agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/dal/entity/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/dal/entity/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1075 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/dal/entity/request_do.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     5231 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/dal/request_library.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     9326 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/request_task.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1146 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/thread_with_result.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2573 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/web_booster.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     5064 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/web_server.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2434 2024-04-09 16:15:17.000000 agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/web_util.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.239569 agentuniverse-0.0.2b1/agentuniverse/base/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     9452 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/agentuniverse.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.239864 agentuniverse-0.0.2b1/agentuniverse/base/annotation/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/annotation/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      515 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/annotation/singleton.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.241006 agentuniverse-0.0.2b1/agentuniverse/base/component/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/component/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1081 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/component/application_component_manager.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1264 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/component/component_base.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     4129 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/component/component_configer_util.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      604 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/component/component_enum.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2576 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/component/component_manager_base.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.241495 agentuniverse-0.0.2b1/agentuniverse/base/config/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.242242 agentuniverse-0.0.2b1/agentuniverse/base/config/application_configer/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/application_configer/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3885 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/application_configer/app_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1006 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/application_configer/application_config_manager.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.242791 agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2557 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/component_configer.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.244172 agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/configers/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      165 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/configers/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2599 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/configers/agent_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2053 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/configers/knowledge_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3272 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/configers/llm_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2540 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/configers/memory_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2392 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/configers/planner_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2192 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/configers/tool_configer.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      423 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/config_type_enum.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     4828 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/configer.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.244503 agentuniverse-0.0.2b1/agentuniverse/base/config/custom_configer/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/custom_configer/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      707 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/config/custom_configer/custom_key_configer.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.245015 agentuniverse-0.0.2b1/agentuniverse/base/context/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/context/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1447 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/context/framework_context.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2768 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/context/framework_context_manager.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.245822 agentuniverse-0.0.2b1/agentuniverse/base/util/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/util/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      307 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/util/env_util.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.246435 agentuniverse-0.0.2b1/agentuniverse/base/util/logging/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/util/logging/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     6600 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/util/logging/general_logger.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     5132 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/util/logging/logging_config.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     6395 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/agentuniverse/base/util/logging/logging_util.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      502 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/util/memory_util.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     6379 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/base/util/prompt_util.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      715 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/base/util/system_util.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.247325 agentuniverse-0.0.2b1/agentuniverse/llm/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/llm/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.247769 agentuniverse-0.0.2b1/agentuniverse/llm/default/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/llm/default/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1422 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/llm/default/default_openai_llm.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      223 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/agentuniverse/llm/default/default_openai_llm.yaml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2911 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/llm/langchain_instance.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     4946 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/llm/llm.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      619 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/llm/llm_manager.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      328 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/llm/llm_output.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     4514 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/llm/openai_llm.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.248248 agentuniverse-0.0.2b1/agentuniverse/prompt/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      156 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/prompt/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1931 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/agentuniverse/prompt/prompt.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      834 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse/prompt/prompt_model.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.248409 agentuniverse-0.0.2b1/agentuniverse_connector/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:12:13.000000 agentuniverse-0.0.2b1/agentuniverse_connector/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.248566 agentuniverse-0.0.2b1/agentuniverse_extension/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:13:12.000000 agentuniverse-0.0.2b1/agentuniverse_extension/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.248899 agentuniverse-0.0.2b1/agentuniverse_extension/logger/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse_extension/logger/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     7321 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/agentuniverse_extension/logger/sls_sink.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     2160 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/pyproject.toml
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)       38 2024-04-17 10:21:50.257551 agentuniverse-0.0.2b1/setup.cfg
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1201 2024-04-17 10:21:46.000000 agentuniverse-0.0.2b1/setup.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.249083 agentuniverse-0.0.2b1/tests/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 03:13:12.000000 agentuniverse-0.0.2b1/tests/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.249259 agentuniverse-0.0.2b1/tests/test_agentuniverse/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.249417 agentuniverse-0.0.2b1/tests/test_agentuniverse/mock/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/mock/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.250179 agentuniverse-0.0.2b1/tests/test_agentuniverse/mock/agent_serve/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/mock/agent_serve/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      535 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/mock/agent_serve/mock_agent.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      475 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/mock/agent_serve/mock_application_config_manager.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      896 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/mock/agent_serve/mock_service_manager.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      509 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/mock/agent_serve/mock_simple_service.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.250366 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.251082 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.251330 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/action/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/action/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.251745 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/action/knowledge/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/action/knowledge/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.252242 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/action/knowledge/embedding/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/action/knowledge/embedding/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1097 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/action/knowledge/embedding/test_embedding.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1566 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/action/knowledge/test_knowledge.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.252683 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/memory/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/memory/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     3894 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/memory/test_memory.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      776 2024-04-12 13:27:46.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/test_agent.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.253684 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent_serve/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent_serve/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1237 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent_serve/test_service.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      920 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent_serve/test_service_instance.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1613 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent_serve/test_service_manager.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      524 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent_serve/test_web_booster.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.253883 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/base/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/base/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.254266 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/base/context/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/base/context/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1442 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/base/context/test_framework_context.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.254450 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/base/util/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/base/util/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.254799 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/base/util/logging/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/base/util/logging/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1670 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/base/util/logging/test_logging_util.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.255138 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/llm/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      173 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/llm/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1264 2024-04-12 13:21:51.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/llm/test_llm.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.255285 agentuniverse-0.0.2b1/tests/test_agentuniverse_connector/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse_connector/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.255437 agentuniverse-0.0.2b1/tests/test_agentuniverse_extension/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      164 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse_extension/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.255592 agentuniverse-0.0.2b1/tests/test_agentuniverse_extension/mock/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse_extension/mock/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.255951 agentuniverse-0.0.2b1/tests/test_agentuniverse_extension/mock/logger/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse_extension/mock/logger/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      620 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse_extension/mock/logger/mock_log_client.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.256110 agentuniverse-0.0.2b1/tests/test_agentuniverse_extension/unit/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse_extension/unit/__init__.py
+drwxr-xr-x   0 jerry.zzw   (501) staff       (20)        0 2024-04-17 10:21:50.256428 agentuniverse-0.0.2b1/tests/test_agentuniverse_extension/unit/logger/
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)      163 2024-04-02 12:08:01.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse_extension/unit/logger/__init__.py
+-rw-r--r--   0 jerry.zzw   (501) staff       (20)     1288 2024-04-12 13:26:06.000000 agentuniverse-0.0.2b1/tests/test_agentuniverse_extension/unit/logger/test_sls_sink.py
```

### Comparing `agentUniverse-0.0.1b1/LICENSE` & `agentuniverse-0.0.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/PKG-INFO` & `agentuniverse-0.0.2b1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-Metadata-Version: 2.1
-Name: agentUniverse
-Version: 0.0.1b1
-Summary: AgentUniverse is a framework for developing applications powered by multi-agent base on large language model.
-Author: AntGroup
-Author-email: jerry.zzw@antgroup.com
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# AgentUniverse
+# agentUniverse
+****************************************
+Language version: [English](./README.md) | [中文](./README_zh.md)
+
+![](https://img.shields.io/badge/framework-aU-pink)
+![](https://img.shields.io/badge/python-3.10%2B-blue?logo=Python)
+[![](https://img.shields.io/badge/%20license-Apache--2.0-yellow)](LICENSE)
+****************************************
 
 ## Overview
 AgentUniverse is a framework for developing applications powered by multi-agent base on large language model.  It provides all the essential components for building a single agent, and a multi-agent collaboration mechanism which  serves as a pattern factory that allowing developers to buid and customize multi-agent collaboration patterns. With this framework,  developers can easily construct multi-agent applications, and share the pattern practices from different technical  and business fields.
 
 The framework will come with serveral pre-install multi-agent collaboration patterns which have been proven effective in real business scenarios, and will continue to be enriched in the future. Patterns that are currently about to be released include:
 
 - PEER pattern：
 This pattern utilizes four distinct agent roles: Plan, Execute, Express, and Review, to achieve a multi-step breakdown and sequential execution of a complex task. It also performs autonomous iteration based on evaluative feedback which enhancing performance in reasoning and analytical tasks. 
 
 
 - DOE pattern：
 This pattern consists of three agents: Data-fining agent, which is designed to solve data-intensive and high-computational-precision task; Opinion-inject agent, which combines the data results from first agent and the expert opinions which are pre-collected and structured; the third agent, Express agent generates the final result base on given document type and language style.
 
 More patterns are coming soon...
+
+## Quick Installation
+Using pip:
+```shell
+pip install agentUniverse
+```
```

### Comparing `agentUniverse-0.0.1b1/agentUniverse.egg-info/SOURCES.txt` & `agentuniverse-0.0.2b1/agentUniverse.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 agentUniverse.egg-info/PKG-INFO
 agentUniverse.egg-info/SOURCES.txt
 agentUniverse.egg-info/dependency_links.txt
+agentUniverse.egg-info/requires.txt
 agentUniverse.egg-info/top_level.txt
 agentuniverse/__init__.py
 agentuniverse/agent/__init__.py
 agentuniverse/agent/agent.py
 agentuniverse/agent/agent_manager.py
 agentuniverse/agent/agent_model.py
 agentuniverse/agent/input_object.py
```

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/embedding/embedding.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/embedding/embedding.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/embedding/openai_embedding.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/embedding/openai_embedding.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/knowledge.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/knowledge.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/knowledge_manager.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/knowledge_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/reader/file/docx_reader.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/file/docx_reader.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/reader/file/file_reader.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/file/file_reader.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/reader/file/pdf_reader.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/file/pdf_reader.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/reader/file/pptx_reader.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/file/pptx_reader.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/reader/file/web_pdf_reader.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/file/web_pdf_reader.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/reader/reader.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/reader/reader.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/store/chroma_store.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/store/chroma_store.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/store/document.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/store/document.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/store/query.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/store/query.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/action/knowledge/store/store.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/action/knowledge/store/store.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/action/tool/tool.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/action/tool/tool.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/action/tool/tool_manager.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/action/tool/tool_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/agent.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/agent.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/agent_manager.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/agent_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/agent_model.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/agent_model.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/default/executing_agent.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/default/executing_agent.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/default/expressing_agent.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/default/expressing_agent.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/default/planning_agent.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/default/planning_agent.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/default/rag_agent.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/default/rag_agent.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/default/reviewing_agent.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/default/reviewing_agent.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/input_object.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/input_object.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/memory/chat_memory.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/memory/chat_memory.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/memory/langchain_instance.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/memory/langchain_instance.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/memory/memory.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/memory/memory.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/memory/memory_manager.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/memory/memory_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/memory/prompt.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/memory/prompt.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/output_object.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/output_object.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/executing_planner/executing_planner.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/executing_planner/executing_planner.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/executing_planner/prompt.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/executing_planner/prompt.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/expressing_planner/prompt.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/expressing_planner/prompt.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/peer_planner/peer_planner.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/peer_planner/peer_planner.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/planner.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/planner.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/planner_manager.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/planner_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/planning_planner/planning_planner.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/planning_planner/planning_planner.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/planning_planner/prompt.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/planning_planner/prompt.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/rag_planner/prompt.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/rag_planner/prompt.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/rag_planner/rag_planner.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/rag_planner/rag_planner.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/reviewing_planner/prompt.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/reviewing_planner/prompt.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.py` & `agentuniverse-0.0.2b1/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent_serve/service.py` & `agentuniverse-0.0.2b1/agentuniverse/agent_serve/service.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent_serve/service_configer.py` & `agentuniverse-0.0.2b1/agentuniverse/agent_serve/service_configer.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent_serve/service_instance.py` & `agentuniverse-0.0.2b1/agentuniverse/agent_serve/service_instance.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent_serve/web/dal/entity/request_do.py` & `agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/dal/entity/request_do.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent_serve/web/dal/request_library.py` & `agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/dal/request_library.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent_serve/web/request_task.py` & `agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/request_task.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent_serve/web/thread_with_result.py` & `agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/thread_with_result.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent_serve/web/web_booster.py` & `agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/web_booster.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent_serve/web/web_server.py` & `agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/web_server.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/agent_serve/web/web_util.py` & `agentuniverse-0.0.2b1/agentuniverse/agent_serve/web/web_util.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/base/agentuniverse.py` & `agentuniverse-0.0.2b1/agentuniverse/base/agentuniverse.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/base/annotation/singleton.py` & `agentuniverse-0.0.2b1/agentuniverse/base/annotation/singleton.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/base/component/application_component_manager.py` & `agentuniverse-0.0.2b1/agentuniverse/base/component/application_component_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/base/component/component_base.py` & `agentuniverse-0.0.2b1/agentuniverse/base/component/component_base.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/base/component/component_configer_util.py` & `agentuniverse-0.0.2b1/agentuniverse/base/component/component_configer_util.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/base/component/component_enum.py` & `agentuniverse-0.0.2b1/agentuniverse/base/component/component_enum.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/base/component/component_manager_base.py` & `agentuniverse-0.0.2b1/agentuniverse/base/component/component_manager_base.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/base/config/application_configer/app_configer.py` & `agentuniverse-0.0.2b1/agentuniverse/base/config/application_configer/app_configer.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/base/config/application_configer/application_config_manager.py` & `agentuniverse-0.0.2b1/agentuniverse/base/config/application_configer/application_config_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/base/config/component_configer/component_configer.py` & `agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/component_configer.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/base/config/component_configer/configers/agent_configer.py` & `agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/configers/agent_configer.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/base/config/component_configer/configers/knowledge_configer.py` & `agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/configers/knowledge_configer.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/base/config/component_configer/configers/llm_configer.py` & `agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/configers/llm_configer.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/base/config/component_configer/configers/memory_configer.py` & `agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/configers/memory_configer.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/base/config/component_configer/configers/planner_configer.py` & `agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/configers/planner_configer.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/base/config/component_configer/configers/tool_configer.py` & `agentuniverse-0.0.2b1/agentuniverse/base/config/component_configer/configers/tool_configer.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/base/config/configer.py` & `agentuniverse-0.0.2b1/agentuniverse/base/config/configer.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/base/config/custom_configer/custom_key_configer.py` & `agentuniverse-0.0.2b1/agentuniverse/base/config/custom_configer/custom_key_configer.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/base/context/framework_context.py` & `agentuniverse-0.0.2b1/agentuniverse/base/context/framework_context.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/base/context/framework_context_manager.py` & `agentuniverse-0.0.2b1/agentuniverse/base/context/framework_context_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/base/util/logging/general_logger.py` & `agentuniverse-0.0.2b1/agentuniverse/base/util/logging/general_logger.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/base/util/logging/logging_config.py` & `agentuniverse-0.0.2b1/agentuniverse/base/util/logging/logging_config.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/base/util/logging/logging_util.py` & `agentuniverse-0.0.2b1/agentuniverse/base/util/logging/logging_util.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/base/util/prompt_util.py` & `agentuniverse-0.0.2b1/agentuniverse/base/util/prompt_util.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/base/util/system_util.py` & `agentuniverse-0.0.2b1/agentuniverse/base/util/system_util.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/llm/default/default_openai_llm.py` & `agentuniverse-0.0.2b1/agentuniverse/llm/default/default_openai_llm.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/llm/langchain_instance.py` & `agentuniverse-0.0.2b1/agentuniverse/llm/langchain_instance.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/llm/llm.py` & `agentuniverse-0.0.2b1/agentuniverse/llm/llm.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/llm/llm_manager.py` & `agentuniverse-0.0.2b1/agentuniverse/llm/llm_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/llm/openai_llm.py` & `agentuniverse-0.0.2b1/agentuniverse/llm/openai_llm.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/prompt/prompt.py` & `agentuniverse-0.0.2b1/agentuniverse/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse/prompt/prompt_model.py` & `agentuniverse-0.0.2b1/agentuniverse/prompt/prompt_model.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/agentuniverse_extension/logger/sls_sink.py` & `agentuniverse-0.0.2b1/agentuniverse_extension/logger/sls_sink.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/pyproject.toml` & `agentuniverse-0.0.2b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/setup.py` & `agentuniverse-0.0.2b1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,26 +7,37 @@
 # @FileName: setup.py
 
 import setuptools
 
 with open("README_PYPI.md", "r") as fh:
     long_description = fh.read()
 
+
+def read_requirements():
+    with open('requirements.txt', 'r') as req:
+        content = req.read()
+        requirements = content.split('\n')
+
+    return requirements
+
+
 setuptools.setup(
     name="agentUniverse",
-    version="0.0.1.beta1",
+    version="0.0.2.beta1",
     author="AntGroup",
     author_email="jerry.zzw@antgroup.com",
-    description="AgentUniverse is a framework for developing applications powered "
+    description="agentUniverse is a framework for developing applications powered "
                 "by multi-agent base on large language model.",
     long_description=long_description,
     long_description_content_type="text/markdown",
+    url="https://gitee.com/ant-fin-agent-framework/ant-fin-agent-framework",
     packages=setuptools.find_packages(),
     package_data={
             '': ['*.yaml'],
         },
+    install_requires=read_requirements(),
     classifiers=[
         'Programming Language :: Python :: 3.10',
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
-)
+)
```

### Comparing `agentUniverse-0.0.1b1/tests/test_agentuniverse/mock/agent_serve/mock_agent.py` & `agentuniverse-0.0.2b1/tests/test_agentuniverse/mock/agent_serve/mock_agent.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/tests/test_agentuniverse/mock/agent_serve/mock_service_manager.py` & `agentuniverse-0.0.2b1/tests/test_agentuniverse/mock/agent_serve/mock_service_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/agent/action/knowledge/embedding/test_embedding.py` & `agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/action/knowledge/embedding/test_embedding.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/agent/action/knowledge/test_knowledge.py` & `agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/action/knowledge/test_knowledge.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/agent/memory/test_memory.py` & `agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/memory/test_memory.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/agent/test_agent.py` & `agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent/test_agent.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/agent_serve/test_service.py` & `agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent_serve/test_service.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/agent_serve/test_service_instance.py` & `agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent_serve/test_service_instance.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/agent_serve/test_service_manager.py` & `agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent_serve/test_service_manager.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/agent_serve/test_web_booster.py` & `agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/agent_serve/test_web_booster.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/base/context/test_framework_context.py` & `agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/base/context/test_framework_context.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/base/util/logging/test_logging_util.py` & `agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/base/util/logging/test_logging_util.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/tests/test_agentuniverse/unit/llm/test_llm.py` & `agentuniverse-0.0.2b1/tests/test_agentuniverse/unit/llm/test_llm.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/tests/test_agentuniverse_extension/mock/logger/mock_log_client.py` & `agentuniverse-0.0.2b1/tests/test_agentuniverse_extension/mock/logger/mock_log_client.py`

 * *Files identical despite different names*

### Comparing `agentUniverse-0.0.1b1/tests/test_agentuniverse_extension/unit/logger/test_sls_sink.py` & `agentuniverse-0.0.2b1/tests/test_agentuniverse_extension/unit/logger/test_sls_sink.py`

 * *Files identical despite different names*

