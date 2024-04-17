# Comparing `tmp/eidolon_ai_sdk-0.1.26.tar.gz` & `tmp/eidolon_ai_sdk-0.1.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eidolon_ai_sdk-0.1.26.tar", max compression
+gzip compressed data, was "eidolon_ai_sdk-0.1.27.tar", max compression
```

## Comparing `eidolon_ai_sdk-0.1.26.tar` & `eidolon_ai_sdk-0.1.27.tar`

### file list

```diff
@@ -1,143 +1,143 @@
--rw-r--r--   0        0        0     2569 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/README.md
--rw-r--r--   0        0        0        0 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/__init__.py
--rw-r--r--   0        0        0     2400 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/agent.py
--rw-r--r--   0        0        0        0 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/__init__.py
--rw-r--r--   0        0        0     3025 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/document_manager.py
--rw-r--r--   0        0        0     2710 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/document_processor.py
--rw-r--r--   0        0        0        0 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/loaders/__init__.py
--rw-r--r--   0        0        0      971 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py
--rw-r--r--   0        0        0     3405 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py
--rw-r--r--   0        0        0     4173 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py
--rw-r--r--   0        0        0        0 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/__init__.py
--rw-r--r--   0        0        0     2805 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py
--rw-r--r--   0        0        0     4519 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py
--rw-r--r--   0        0        0        0 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/__init__.py
--rw-r--r--   0        0        0      448 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/base_ast_generator.py
--rw-r--r--   0        0        0     3699 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py
--rw-r--r--   0        0        0     2053 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py
--rw-r--r--   0        0        0     3212 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py
--rw-r--r--   0        0        0     1647 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py
--rw-r--r--   0        0        0     1328 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py
--rw-r--r--   0        0        0     3356 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py
--rw-r--r--   0        0        0     1400 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py
--rw-r--r--   0        0        0        0 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/transformer/__init__.py
--rw-r--r--   0        0        0     1398 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py
--rw-r--r--   0        0        0     4786 2024-04-15 19:20:40.601152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py
--rw-r--r--   0        0        0    43465 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py
--rw-r--r--   0        0        0     4825 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/generic_agent.py
--rw-r--r--   0        0        0     1924 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/openai_whisper_agent.py
--rw-r--r--   0        0        0        0 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/retriever_agent/__init__.py
--rw-r--r--   0        0        0     2078 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py
--rw-r--r--   0        0        0     1434 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py
--rw-r--r--   0        0        0     2329 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py
--rw-r--r--   0        0        0      559 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py
--rw-r--r--   0        0        0     2904 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/retriever_agent/retriever.py
--rw-r--r--   0        0        0     3721 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py
--rw-r--r--   0        0        0    12896 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/simple_agent.py
--rw-r--r--   0        0        0        0 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/tot_agent/__init__.py
--rw-r--r--   0        0        0     1815 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/tot_agent/checker.py
--rw-r--r--   0        0        0     2468 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/tot_agent/controller.py
--rw-r--r--   0        0        0     1503 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/tot_agent/memory.py
--rw-r--r--   0        0        0     1423 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/tot_agent/prompts.py
--rw-r--r--   0        0        0      364 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/tot_agent/thought.py
--rw-r--r--   0        0        0     4951 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/tot_agent/thought_generators.py
--rw-r--r--   0        0        0     7614 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/tot_agent/tot_agent.py
--rw-r--r--   0        0        0     4563 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent_os.py
--rw-r--r--   0        0        0    12721 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent_os_interfaces.py
--rw-r--r--   0        0        0        0 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/bin/__init__.py
--rwxr-xr-x   0        0        0     9444 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/bin/agent_creator.py
--rw-r--r--   0        0        0     7743 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/bin/agent_http_server.py
--rwxr-xr-x   0        0        0     3789 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/bin/replay.py
--rw-r--r--   0        0        0        0 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/__init__.py
--rw-r--r--   0        0        0     8742 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/code_builtins.py
--rw-r--r--   0        0        0        0 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/components/__init__.py
--rw-r--r--   0        0        0     2223 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/components/opentelemetry.py
--rw-r--r--   0        0        0     4256 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/components/usage.py
--rw-r--r--   0        0        0        0 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/logic_units/__init__.py
--rw-r--r--   0        0        0     5662 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/logic_units/web_search.py
--rw-r--r--   0        0        0      234 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml
--rw-r--r--   0        0        0      231 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/resources/claude_opus.yaml
--rw-r--r--   0        0        0      237 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml
--rw-r--r--   0        0        0      181 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/resources/machine.yaml
--rw-r--r--   0        0        0      226 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/resources/mistral_large.yaml
--rw-r--r--   0        0        0      252 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml
--rw-r--r--   0        0        0      226 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/resources/mistral_small.yaml
--rw-r--r--   0        0        0      225 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/resources/openai_35.yaml
--rw-r--r--   0        0        0      229 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/resources/openai_4.yaml
--rw-r--r--   0        0        0        0 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/__init__.py
--rw-r--r--   0        0        0     1843 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/agent_call_history.py
--rw-r--r--   0        0        0     4638 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/agent_cpu.py
--rw-r--r--   0        0        0     2474 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/agent_io.py
--rw-r--r--   0        0        0     7916 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/agents_logic_unit.py
--rw-r--r--   0        0        0     1641 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/audio_unit.py
--rw-r--r--   0        0        0      292 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/call_context.py
--rw-r--r--   0        0        0     2833 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/conversation_memory_unit.py
--rw-r--r--   0        0        0    14068 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/conversational_apu.py
--rw-r--r--   0        0        0     1856 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/image_unit.py
--rw-r--r--   0        0        0        0 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/llm/__init__.py
--rw-r--r--   0        0        0    11215 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py
--rw-r--r--   0        0        0    13115 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py
--rw-r--r--   0        0        0     6166 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py
--rw-r--r--   0        0        0     5631 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py
--rw-r--r--   0        0        0    10361 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py
--rw-r--r--   0        0        0     3375 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/llm/open_ai_speech.py
--rw-r--r--   0        0        0     3930 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/llm_message.py
--rw-r--r--   0        0        0     3443 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/llm_unit.py
--rw-r--r--   0        0        0     4199 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/logic_unit.py
--rw-r--r--   0        0        0     3541 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/memory_unit.py
--rw-r--r--   0        0        0      825 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/processing_unit.py
--rw-r--r--   0        0        0        0 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/io/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/__init__.py
--rw-r--r--   0        0        0     1193 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/agent_memory.py
--rw-r--r--   0        0        0     5309 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/chroma_vector_store.py
--rw-r--r--   0        0        0      641 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/document.py
--rw-r--r--   0        0        0     2620 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/embeddings.py
--rw-r--r--   0        0        0      907 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/file_memory.py
--rw-r--r--   0        0        0     4203 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/file_system_vector_store.py
--rw-r--r--   0        0        0     3974 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/in_memory_file_memory.py
--rw-r--r--   0        0        0     5788 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/local_file_memory.py
--rw-r--r--   0        0        0     4845 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/local_symbolic_memory.py
--rw-r--r--   0        0        0     3770 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/mongo_symbolic_memory.py
--rw-r--r--   0        0        0      996 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/noop_memory.py
--rw-r--r--   0        0        0     1984 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/s3_file_memory.py
--rw-r--r--   0        0        0      975 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/semantic_memory.py
--rw-r--r--   0        0        0     2809 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/similarity_memory.py
--rw-r--r--   0        0        0     1516 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/vector_store.py
--rw-r--r--   0        0        0        0 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/__init__.py
--rw-r--r--   0        0        0      771 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/authentication_processor.py
--rw-r--r--   0        0        0     2091 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/azure_authorizer.py
--rw-r--r--   0        0        0     1277 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/functional_authorizer.py
--rw-r--r--   0        0        0     2001 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/google_auth.py
--rw-r--r--   0        0        0     1867 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/jwt_processor.py
--rw-r--r--   0        0        0      484 2024-04-15 19:20:40.605152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/okta_authorizor.py
--rw-r--r--   0        0        0     1017 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/permissions.py
--rw-r--r--   0        0        0     2508 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/process_authorizer.py
--rw-r--r--   0        0        0     2977 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/security_manager.py
--rw-r--r--   0        0        0     1035 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/security_middleware.py
--rw-r--r--   0        0        0      428 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/user.py
--rw-r--r--   0        0        0        0 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/__init__.py
--rw-r--r--   0        0        0     1377 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/agent_contract.py
--rw-r--r--   0        0        0    21672 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/agent_controller.py
--rw-r--r--   0        0        0    13943 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/agent_machine.py
--rw-r--r--   0        0        0     1149 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/dynamic_middleware.py
--rw-r--r--   0        0        0     3432 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/fn_handler.py
--rw-r--r--   0        0        0     4880 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/process_file_system.py
--rw-r--r--   0        0        0     4275 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/processes.py
--rw-r--r--   0        0        0     6895 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/reference_model.py
--rw-r--r--   0        0        0        0 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/resources/__init__.py
--rw-r--r--   0        0        0      314 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/resources/agent_resource.py
--rw-r--r--   0        0        0      414 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/resources/machine_resource.py
--rw-r--r--   0        0        0      684 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/resources/reference_resource.py
--rw-r--r--   0        0        0     1663 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/resources/resources_base.py
--rw-r--r--   0        0        0        0 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/util/__init__.py
--rw-r--r--   0        0        0      509 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/util/async_wrapper.py
--rw-r--r--   0        0        0     2806 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/util/class_utils.py
--rw-r--r--   0        0        0     1604 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/util/image_utils.py
--rw-r--r--   0        0        0     3812 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/util/replay.py
--rw-r--r--   0        0        0     6483 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/util/schema_to_model.py
--rw-r--r--   0        0        0      900 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/util/str_utils.py
--rw-r--r--   0        0        0     3445 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/util/stream_collector.py
--rw-r--r--   0        0        0      565 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/logging.conf
--rw-r--r--   0        0        0     2030 2024-04-15 19:20:40.609152 eidolon_ai_sdk-0.1.26/pyproject.toml
--rw-r--r--   0        0        0     4807 1970-01-01 00:00:00.000000 eidolon_ai_sdk-0.1.26/PKG-INFO
+-rw-r--r--   0        0        0     2569 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/README.md
+-rw-r--r--   0        0        0        0 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/__init__.py
+-rw-r--r--   0        0        0     2400 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/agent.py
+-rw-r--r--   0        0        0        0 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/__init__.py
+-rw-r--r--   0        0        0     3025 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/document_manager.py
+-rw-r--r--   0        0        0     2710 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/document_processor.py
+-rw-r--r--   0        0        0        0 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/loaders/__init__.py
+-rw-r--r--   0        0        0      971 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py
+-rw-r--r--   0        0        0     3405 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py
+-rw-r--r--   0        0        0     4173 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py
+-rw-r--r--   0        0        0        0 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/__init__.py
+-rw-r--r--   0        0        0     2805 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py
+-rw-r--r--   0        0        0     4519 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py
+-rw-r--r--   0        0        0        0 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/__init__.py
+-rw-r--r--   0        0        0      448 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/base_ast_generator.py
+-rw-r--r--   0        0        0     3699 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py
+-rw-r--r--   0        0        0     2053 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py
+-rw-r--r--   0        0        0     3212 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py
+-rw-r--r--   0        0        0     1647 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py
+-rw-r--r--   0        0        0     1328 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py
+-rw-r--r--   0        0        0     3356 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py
+-rw-r--r--   0        0        0     1400 2024-04-16 01:35:04.010934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py
+-rw-r--r--   0        0        0        0 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/transformer/__init__.py
+-rw-r--r--   0        0        0     1398 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py
+-rw-r--r--   0        0        0     4786 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py
+-rw-r--r--   0        0        0    43465 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py
+-rw-r--r--   0        0        0     4825 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/generic_agent.py
+-rw-r--r--   0        0        0     1924 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/openai_whisper_agent.py
+-rw-r--r--   0        0        0        0 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/retriever_agent/__init__.py
+-rw-r--r--   0        0        0     2078 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py
+-rw-r--r--   0        0        0     1434 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py
+-rw-r--r--   0        0        0     2329 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py
+-rw-r--r--   0        0        0      559 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py
+-rw-r--r--   0        0        0     2904 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/retriever_agent/retriever.py
+-rw-r--r--   0        0        0     3721 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py
+-rw-r--r--   0        0        0    12896 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/simple_agent.py
+-rw-r--r--   0        0        0        0 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/tot_agent/__init__.py
+-rw-r--r--   0        0        0     1815 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/tot_agent/checker.py
+-rw-r--r--   0        0        0     2468 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/tot_agent/controller.py
+-rw-r--r--   0        0        0     1503 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/tot_agent/memory.py
+-rw-r--r--   0        0        0     1423 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/tot_agent/prompts.py
+-rw-r--r--   0        0        0      364 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/tot_agent/thought.py
+-rw-r--r--   0        0        0     4951 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/tot_agent/thought_generators.py
+-rw-r--r--   0        0        0     7614 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/tot_agent/tot_agent.py
+-rw-r--r--   0        0        0     4563 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent_os.py
+-rw-r--r--   0        0        0    12721 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent_os_interfaces.py
+-rw-r--r--   0        0        0        0 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/bin/__init__.py
+-rwxr-xr-x   0        0        0     9444 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/bin/agent_creator.py
+-rw-r--r--   0        0        0     7743 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/bin/agent_http_server.py
+-rwxr-xr-x   0        0        0     3789 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/bin/replay.py
+-rw-r--r--   0        0        0        0 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/__init__.py
+-rw-r--r--   0        0        0     8852 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/code_builtins.py
+-rw-r--r--   0        0        0        0 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/components/__init__.py
+-rw-r--r--   0        0        0     2223 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/components/opentelemetry.py
+-rw-r--r--   0        0        0     4256 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/components/usage.py
+-rw-r--r--   0        0        0        0 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/logic_units/__init__.py
+-rw-r--r--   0        0        0     5662 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/logic_units/web_search.py
+-rw-r--r--   0        0        0      550 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml
+-rw-r--r--   0        0        0      544 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/resources/claude_opus.yaml
+-rw-r--r--   0        0        0      557 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml
+-rw-r--r--   0        0        0      181 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/resources/machine.yaml
+-rw-r--r--   0        0        0      540 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/resources/mistral_large.yaml
+-rw-r--r--   0        0        0      547 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml
+-rw-r--r--   0        0        0      540 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/resources/mistral_small.yaml
+-rw-r--r--   0        0        0      534 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/resources/openai_35.yaml
+-rw-r--r--   0        0        0      557 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/resources/openai_4.yaml
+-rw-r--r--   0        0        0        0 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/__init__.py
+-rw-r--r--   0        0        0     1843 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/agent_call_history.py
+-rw-r--r--   0        0        0     4638 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/agent_cpu.py
+-rw-r--r--   0        0        0     2474 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/agent_io.py
+-rw-r--r--   0        0        0     7916 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/agents_logic_unit.py
+-rw-r--r--   0        0        0     1641 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/audio_unit.py
+-rw-r--r--   0        0        0      292 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/call_context.py
+-rw-r--r--   0        0        0     2833 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/conversation_memory_unit.py
+-rw-r--r--   0        0        0    14068 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/conversational_apu.py
+-rw-r--r--   0        0        0     1856 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/image_unit.py
+-rw-r--r--   0        0        0        0 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm/__init__.py
+-rw-r--r--   0        0        0    10023 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py
+-rw-r--r--   0        0        0    11932 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py
+-rw-r--r--   0        0        0     5396 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py
+-rw-r--r--   0        0        0     5631 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py
+-rw-r--r--   0        0        0     9485 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py
+-rw-r--r--   0        0        0     3375 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm/open_ai_speech.py
+-rw-r--r--   0        0        0     3930 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm_message.py
+-rw-r--r--   0        0        0     2421 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm_unit.py
+-rw-r--r--   0        0        0     4199 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/logic_unit.py
+-rw-r--r--   0        0        0     3541 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/memory_unit.py
+-rw-r--r--   0        0        0      825 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/processing_unit.py
+-rw-r--r--   0        0        0        0 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/io/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/__init__.py
+-rw-r--r--   0        0        0     1193 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/agent_memory.py
+-rw-r--r--   0        0        0     5309 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/chroma_vector_store.py
+-rw-r--r--   0        0        0      641 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/document.py
+-rw-r--r--   0        0        0     2766 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/embeddings.py
+-rw-r--r--   0        0        0      907 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/file_memory.py
+-rw-r--r--   0        0        0     4203 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/file_system_vector_store.py
+-rw-r--r--   0        0        0     3974 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/in_memory_file_memory.py
+-rw-r--r--   0        0        0     5788 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/local_file_memory.py
+-rw-r--r--   0        0        0     4845 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/local_symbolic_memory.py
+-rw-r--r--   0        0        0     3770 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/mongo_symbolic_memory.py
+-rw-r--r--   0        0        0      996 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/noop_memory.py
+-rw-r--r--   0        0        0     1984 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/s3_file_memory.py
+-rw-r--r--   0        0        0      975 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/semantic_memory.py
+-rw-r--r--   0        0        0     2809 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/similarity_memory.py
+-rw-r--r--   0        0        0     1516 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/vector_store.py
+-rw-r--r--   0        0        0        0 2024-04-16 01:35:04.014934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/__init__.py
+-rw-r--r--   0        0        0      771 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/authentication_processor.py
+-rw-r--r--   0        0        0     2091 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/azure_authorizer.py
+-rw-r--r--   0        0        0     1277 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/functional_authorizer.py
+-rw-r--r--   0        0        0     2001 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/google_auth.py
+-rw-r--r--   0        0        0     1867 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/jwt_processor.py
+-rw-r--r--   0        0        0      484 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/okta_authorizor.py
+-rw-r--r--   0        0        0     1017 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/permissions.py
+-rw-r--r--   0        0        0     2508 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/process_authorizer.py
+-rw-r--r--   0        0        0     2977 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/security_manager.py
+-rw-r--r--   0        0        0     1035 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/security_middleware.py
+-rw-r--r--   0        0        0      428 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/user.py
+-rw-r--r--   0        0        0        0 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/__init__.py
+-rw-r--r--   0        0        0     1377 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/agent_contract.py
+-rw-r--r--   0        0        0    21672 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/agent_controller.py
+-rw-r--r--   0        0        0    14143 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/agent_machine.py
+-rw-r--r--   0        0        0     1149 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/dynamic_middleware.py
+-rw-r--r--   0        0        0     3432 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/fn_handler.py
+-rw-r--r--   0        0        0     4880 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/process_file_system.py
+-rw-r--r--   0        0        0     4275 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/processes.py
+-rw-r--r--   0        0        0     6895 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/reference_model.py
+-rw-r--r--   0        0        0        0 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/resources/__init__.py
+-rw-r--r--   0        0        0      314 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/resources/agent_resource.py
+-rw-r--r--   0        0        0      414 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/resources/machine_resource.py
+-rw-r--r--   0        0        0      684 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/resources/reference_resource.py
+-rw-r--r--   0        0        0     1663 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/resources/resources_base.py
+-rw-r--r--   0        0        0        0 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/util/__init__.py
+-rw-r--r--   0        0        0      509 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/util/async_wrapper.py
+-rw-r--r--   0        0        0     2806 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/util/class_utils.py
+-rw-r--r--   0        0        0     1604 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/util/image_utils.py
+-rw-r--r--   0        0        0     3812 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/util/replay.py
+-rw-r--r--   0        0        0     6483 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/util/schema_to_model.py
+-rw-r--r--   0        0        0      900 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/util/str_utils.py
+-rw-r--r--   0        0        0     3445 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/util/stream_collector.py
+-rw-r--r--   0        0        0      565 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/logging.conf
+-rw-r--r--   0        0        0     2030 2024-04-16 01:35:04.018934 eidolon_ai_sdk-0.1.27/pyproject.toml
+-rw-r--r--   0        0        0     4807 1970-01-01 00:00:00.000000 eidolon_ai_sdk-0.1.27/PKG-INFO
```

### Comparing `eidolon_ai_sdk-0.1.26/README.md` & `eidolon_ai_sdk-0.1.27/README.md`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/agent.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/document_manager.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/document_manager.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/document_processor.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/document_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/generic_agent.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/generic_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/openai_whisper_agent.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/openai_whisper_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/retriever_agent/retriever.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/retriever_agent/retriever.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/simple_agent.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/simple_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/tot_agent/checker.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/tot_agent/checker.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/tot_agent/controller.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/tot_agent/controller.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/tot_agent/memory.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/tot_agent/memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/tot_agent/prompts.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/tot_agent/prompts.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/tot_agent/thought_generators.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/tot_agent/thought_generators.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent/tot_agent/tot_agent.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent/tot_agent/tot_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent_os.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent_os.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/agent_os_interfaces.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/agent_os_interfaces.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/bin/agent_creator.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/bin/agent_creator.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/bin/agent_http_server.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/bin/agent_http_server.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/bin/replay.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/bin/replay.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/code_builtins.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/code_builtins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Tuple
 
+from azure.identity import DefaultAzureCredential
 from openai import AsyncOpenAI
 from openai.lib.azure import AsyncAzureOpenAI
 from opentelemetry.exporter.otlp.proto.grpc.trace_exporter import OTLPSpanExporter
 from opentelemetry.sdk.trace import SpanProcessor
 from opentelemetry.sdk.trace.export import BatchSpanProcessor, SpanExporter
 from opentelemetry.sdk.trace.sampling import Sampler
 
@@ -37,15 +38,15 @@
 from eidolon_ai_sdk.cpu.conversational_apu import ConversationalAPU
 from eidolon_ai_sdk.agent_os_interfaces import FileMemory, SymbolicMemory, SimilarityMemory, SecurityManager
 from eidolon_ai_sdk.cpu.llm.anthropic_llm_unit import AnthropicLLMUnit
 from eidolon_ai_sdk.cpu.llm.mistral_llm_unit import MistralGPT
 from eidolon_ai_sdk.cpu.llm.open_ai_connection_handler import OpenAIConnectionHandler, AzureOpenAIConnectionHandler
 from eidolon_ai_sdk.cpu.llm.open_ai_llm_unit import OpenAIGPT
 from eidolon_ai_sdk.cpu.llm.open_ai_speech import OpenAiSpeech
-from eidolon_ai_sdk.cpu.llm_unit import LLMUnit
+from eidolon_ai_sdk.cpu.llm_unit import LLMUnit, LLMModel
 from eidolon_ai_sdk.cpu.memory_unit import MemoryUnit
 from eidolon_ai_sdk.memory.s3_file_memory import S3FileMemory
 from eidolon_ai_sdk.security.azure_authorizer import AzureJWTProcessor
 from eidolon_ai_sdk.security.google_auth import GoogleJWTProcessor
 from eidolon_ai_sdk.system.dynamic_middleware import Middleware, MultiMiddleware
 from eidolon_ai_sdk.system.process_file_system import ProcessFileSystem, ProcessFileSystemImpl
 from eidolon_ai_usage_client.client import UsageClient
@@ -130,14 +131,15 @@
         ConversationalAPU,
         # cpu components
         IOUnit,
         (LLMUnit, OpenAIGPT),
         OpenAIGPT,
         MistralGPT,
         AnthropicLLMUnit,
+        LLMModel,
         (MemoryUnit, RawMemoryUnit),
         RawMemoryUnit,
         WebSearch,
         Search,
         Browser,
         Retriever,
         # machine components
@@ -189,11 +191,12 @@
         ToTChecker,
         OpenAiSpeech,
         AsyncOpenAI,
         AsyncAzureOpenAI,
         UsageClient,
         OpenAIConnectionHandler,
         AzureOpenAIConnectionHandler,
+        DefaultAzureCredential,
         # config objects
         ReplayConfig,
     ]
     return [_to_resource(maybe_tuple) for maybe_tuple in builtin_list if maybe_tuple]
```

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/components/opentelemetry.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/components/opentelemetry.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/components/usage.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/components/usage.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/builtins/logic_units/web_search.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/builtins/logic_units/web_search.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/agent_call_history.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/agent_call_history.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/agent_cpu.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/agent_cpu.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/agent_io.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/agent_io.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/agents_logic_unit.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/agents_logic_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/audio_unit.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/audio_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/conversation_memory_unit.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/conversation_memory_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/conversational_apu.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/conversational_apu.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/image_unit.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/image_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from io import BytesIO
 from typing import List, Optional, Union, Literal, Dict, Any, AsyncIterator
 
 import yaml
 from PIL import Image
 from anthropic import AsyncAnthropic, APIConnectionError, RateLimitError, APIStatusError
 from fastapi import HTTPException
-from pydantic import Field
 
 from eidolon_ai_client.events import (
     StringOutputEvent,
     ObjectOutputEvent,
     ToolCall,
 )
 from eidolon_ai_client.util.logger import logger as eidolon_logger
@@ -22,15 +21,15 @@
     LLMMessage,
     AssistantMessage,
     ToolResponseMessage,
     UserMessage,
     SystemMessage,
 )
 from eidolon_ai_sdk.cpu.llm_unit import LLMUnit, LLMCallFunction, LLMModel, LLMUnitSpec
-from eidolon_ai_sdk.system.reference_model import Specable
+from eidolon_ai_sdk.system.reference_model import Specable, AnnotatedReference
 from eidolon_ai_sdk.util.replay import replayable
 
 logger = eidolon_logger.getChild("llm_unit")
 
 
 def scale_dimensions(width, height, max_size=2048, min_size=768):
     # Check if the dimensions are less than or equal to max_size.
@@ -121,16 +120,19 @@
             "tool_call_id": message.tool_call_id,
             "content": json.dumps(message.result),
         }
     else:
         raise ValueError(f"Unknown message type {message.type}")
 
 
+claude_opus = "claude-3-opus-20240229"
+
+
 class AnthropicLLMUnitSpec(LLMUnitSpec):
-    model: str = Field(default="claude-3-opus-20240229", description="The model to use for the LLM.")
+    model: AnnotatedReference[LLMModel, claude_opus]
     temperature: float = 0.3
     max_tokens: Optional[int] = None
     client_args: dict = {}
 
 
 class AnthropicLLMUnit(LLMUnit, Specable[AnthropicLLMUnitSpec]):
     temperature: float
@@ -138,48 +140,14 @@
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         LLMUnit.__init__(self, **kwargs)
         Specable.__init__(self, **kwargs)
 
         self.temperature = self.spec.temperature
 
-    def get_models(self) -> List[LLMModel]:
-        if self.spec.supported_models:
-            return self.spec.supported_models
-
-        return [
-            LLMModel(
-                human_name="Claude Opus",
-                name="claude-3-opus-20240229",
-                input_context_limit=200000,
-                output_context_limit=4096,
-                supports_tools=False,
-                supports_image_input=True,
-                supports_audio_input=False,
-            ),
-            LLMModel(
-                human_name="Claude Sonnet",
-                name="claude-3-sonnet-20240229",
-                input_context_limit=200000,
-                output_context_limit=4096,
-                supports_tools=False,
-                supports_image_input=True,
-                supports_audio_input=False,
-            ),
-            LLMModel(
-                human_name="Claude Haiku",
-                name="claude-3-haiku-20240307",
-                input_context_limit=200000,
-                output_context_limit=4096,
-                supports_tools=False,
-                supports_image_input=True,
-                supports_audio_input=False,
-            )
-        ]
-
     async def execute_llm(
             self,
             call_context: CallContext,
             messages: List[LLMMessage],
             tools: List[LLMCallFunction],
             output_format: Union[Literal["str"], Dict[str, Any]],
     ) -> AsyncIterator[AssistantMessage]:
```

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 import yaml
 from PIL import Image
 from fastapi import HTTPException
 from mistralai.async_client import MistralAsyncClient
 from mistralai.exceptions import MistralConnectionException, MistralAPIStatusException, MistralAPIException
 from mistralai.models.chat_completion import ChatCompletionStreamResponse, ResponseFormat, ResponseFormats, Function
-from pydantic import Field
 
 from eidolon_ai_client.events import (
     StringOutputEvent,
     ObjectOutputEvent,
     LLMToolCallRequestEvent,
     ToolCall,
 )
@@ -23,15 +22,15 @@
     LLMMessage,
     AssistantMessage,
     ToolResponseMessage,
     UserMessage,
     SystemMessage,
 )
 from eidolon_ai_sdk.cpu.llm_unit import LLMUnit, LLMCallFunction, LLMModel, LLMUnitSpec
-from eidolon_ai_sdk.system.reference_model import Specable
+from eidolon_ai_sdk.system.reference_model import Specable, AnnotatedReference
 from eidolon_ai_sdk.util.replay import replayable
 
 logger = eidolon_logger.getChild("llm_unit")
 
 
 def scale_dimensions(width, height, max_size=2048, min_size=768):
     # Check if the dimensions are less than or equal to max_size.
@@ -112,62 +111,31 @@
             "tool_call_id": message.tool_call_id,
             "content": json.dumps(message.result),
         }
     else:
         raise ValueError(f"Unknown message type {message.type}")
 
 
+mistral_large = "mistral-large-latest"
+
+
 class MistralGPTSpec(LLMUnitSpec):
-    model: str = Field(default="mistral-large-latest", description="The model to use for the LLM.")
+    model: AnnotatedReference[LLMModel, mistral_large]
     temperature: float = 0.3
     force_json: bool = True
     max_tokens: Optional[int] = None
     client_args: dict = {}
 
 
 class MistralGPT(LLMUnit, Specable[MistralGPTSpec]):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         LLMUnit.__init__(self, **kwargs)
         Specable.__init__(self, **kwargs)
 
-    def get_models(self) -> List[LLMModel]:
-        if self.spec.supported_models:
-            return self.spec.supported_models
-
-        return [
-            LLMModel(
-                human_name="Mistral Large",
-                name="mistral-large-latest",
-                input_context_limit=32000,
-                output_context_limit=4096,
-                supports_tools=True,
-                supports_image_input=False,
-                supports_audio_input=False,
-            ),
-            LLMModel(
-                human_name="Mistral Medium",
-                name="mistral-medium-latest",
-                input_context_limit=32000,
-                output_context_limit=4096,
-                supports_tools=False,
-                supports_image_input=False,
-                supports_audio_input=False,
-            ),
-            LLMModel(
-                human_name="Mistral Small",
-                name="mistral-small-latest",
-                input_context_limit=32000,
-                output_context_limit=4096,
-                supports_tools=False,
-                supports_image_input=False,
-                supports_audio_input=False,
-            )
-        ]
-
     async def execute_llm(
             self,
             call_context: CallContext,
             messages: List[LLMMessage],
             tools: List[LLMCallFunction],
             output_format: Union[Literal["str"], Dict[str, Any]],
     ) -> AsyncIterator[AssistantMessage]:
```

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-from typing import Optional, cast
+from typing import Optional, cast, List
 
 from azure.identity import DefaultAzureCredential, get_bearer_token_provider
 from fastapi import HTTPException
 from openai import AsyncOpenAI, AsyncStream, APIConnectionError, RateLimitError, APIStatusError
 from openai.lib.azure import AsyncAzureOpenAI
 from openai.types import ImagesResponse
 from openai.types.chat import ChatCompletionChunk, ChatCompletion
 from pydantic import BaseModel
 
-from eidolon_ai_sdk.system.reference_model import Specable
+from eidolon_ai_sdk.system.reference_model import Specable, Reference
 from eidolon_ai_sdk.util.replay import replayable
 
 
-class OpenAIConnectionHandlerSpec(BaseModel):
-    api_key: Optional[str] = None
+class OpenAIConnectionHandlerSpec(BaseModel, extra='allow'):
+    pass
 
 
 class OpenAIConnectionHandler(Specable[OpenAIConnectionHandlerSpec]):
     def makeClient(self) -> AsyncOpenAI:
-        if self.spec.api_key:
-            return AsyncOpenAI(api_key=self.spec.api_key)
-        return AsyncOpenAI()
+        return AsyncOpenAI(**self.spec.model_extra)
 
     async def completion(self, kwargs: dict) -> ChatCompletion | AsyncStream[ChatCompletionChunk]:
         return await self._do_request(self.makeClient().chat.completions.create, kwargs)
 
     async def generate_image(self, kwargs: dict) -> ImagesResponse:
         return await self._do_request(self.makeClient().images.generate, kwargs)
 
@@ -62,46 +60,25 @@
     Automatically infers the values from environment variables for:
         - `api_key` from `AZURE_OPENAI_API_KEY` (IFF `api_key` AND 'azure_ad_token_provider' is not provided)
         - `organization` from `OPENAI_ORG_ID`
         - `azure_ad_token` from `AZURE_OPENAI_AD_TOKEN`
         - `api_version` from `OPENAI_API_VERSION`
         - `azure_endpoint` from `AZURE_OPENAI_ENDPOINT`
         """
-    api_key: Optional[str] = None
-    use_default_token_provider: Optional[bool] = False
-    organization: Optional[str] = None
-    azure_ad_token: Optional[str] = None
-    api_version: str
-    azure_endpoint: Optional[str] = None
+    token_provider: Optional[Reference[DefaultAzureCredential]] = None
+    token_provider_scopes: List[str] = ["https://cognitiveservices.azure.com/.default"]
 
 
 class AzureOpenAIConnectionHandler(OpenAIConnectionHandler, Specable[AzureOpenAIConnectionHandlerSpec]):
-    def __init__(self, spec: AzureOpenAIConnectionHandlerSpec):
-        super().__init__(spec=spec)
-        Specable.__init__(self, spec=spec)
-
     def makeClient(self):
-        params = {}
-        if self.spec.api_key:
-            params["api_key"] = self.spec.api_key
-        if self.spec.use_default_token_provider:
-            # noinspection PyTypeChecker
-            token_provider = get_bearer_token_provider(
-                DefaultAzureCredential(), "https://cognitiveservices.azure.com/.default"
-            )
+        params = self.spec.model_extra
+        if self.spec.token_provider:
+            provider = self.spec.token_provider.instantiate()
+            token_provider = get_bearer_token_provider(provider, *self.spec.token_provider_scopes)
             params["token_provider"] = token_provider
-        if self.spec.organization:
-            params["organization"] = self.spec.organization
-        if self.spec.azure_ad_token:
-            params["azure_ad_token"] = self.spec.azure_ad_token
-        if self.spec.api_version:
-            params["api_version"] = self.spec.api_version
-        if self.spec.azure_endpoint:
-            params["endpoint"] = self.spec.azure_endpoint
-
         return AsyncAzureOpenAI(**params)
 
 
 async def _open_ai_replay_parser(resp):
     """
     Parses responses from openai and yield strings to accumulate to a human-readable message.
```

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import logging
 from typing import List, Optional, Union, Literal, Dict, Any, AsyncIterator, cast
 
 import yaml
 from openai import AsyncStream
 from openai.types.chat import ChatCompletionToolParam, ChatCompletionChunk
 from openai.types.chat.completion_create_params import ResponseFormat
-from pydantic import Field
 
 from eidolon_ai_client.events import (
     StringOutputEvent,
     ObjectOutputEvent,
     LLMToolCallRequestEvent,
     ToolCall,
 )
@@ -80,16 +79,19 @@
             "tool_call_id": message.tool_call_id,
             "content": json.dumps(message.result),
         }
     else:
         raise ValueError(f"Unknown message type {message.type}")
 
 
+gpt_4 = "gpt-4-turbo-preview"
+
+
 class OpenAiGPTSpec(LLMUnitSpec):
-    model: str = Field(default="gpt-4-turbo-preview", description="The model to use for the LLM.")
+    model: AnnotatedReference[LLMModel, gpt_4]
     temperature: float = 0.3
     force_json: bool = True
     max_tokens: Optional[int] = None
     connection_handler: AnnotatedReference[OpenAIConnectionHandler]
 
 
 class OpenAIGPT(LLMUnit, Specable[OpenAiGPTSpec]):
@@ -98,39 +100,14 @@
 
     def __init__(self, **kwargs):
         LLMUnit.__init__(self, **kwargs)
         Specable.__init__(self, **kwargs)
         self.temperature = self.spec.temperature
         self.connection_handler = self.spec.connection_handler.instantiate()
 
-    def get_models(self) -> List[LLMModel]:
-        if self.spec.supported_models:
-            return self.spec.supported_models
-
-        return [
-            LLMModel(
-                human_name="GPT-4 Turbo Preview",
-                name="gpt-4-turbo-preview",
-                input_context_limit=128000,
-                output_context_limit=4096,
-                supports_tools=True,
-                supports_image_input=True,
-                supports_audio_input=False,
-            ),
-            LLMModel(
-                human_name="GPT-3.5 Turbo",
-                name="gpt-3.5-turbo",
-                input_context_limit=16385,
-                output_context_limit=4096,
-                supports_tools=True,
-                supports_image_input=False,
-                supports_audio_input=False,
-            )
-        ]
-
     async def execute_llm(
             self,
             call_context: CallContext,
             messages: List[LLMMessage],
             tools: List[LLMCallFunction],
             output_format: Union[Literal["str"], Dict[str, Any]],
     ) -> AsyncIterator[AssistantMessage]:
```

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/llm/open_ai_speech.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm/open_ai_speech.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/llm_message.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm_message.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/llm_unit.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/llm_unit.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,35 +3,15 @@
 
 from pydantic import BaseModel, Field
 
 from eidolon_ai_client.events import StreamEvent
 from eidolon_ai_sdk.cpu.call_context import CallContext
 from eidolon_ai_sdk.cpu.llm_message import LLMMessage
 from eidolon_ai_sdk.cpu.processing_unit import ProcessingUnit
-from eidolon_ai_sdk.system.reference_model import Specable
-
-LLM_MAX_TOKENS = {
-    "DEFAULT": 8192,
-    # OpenAI models: https://platform.openai.com/docs/models/overview
-    # gpt-4
-    "gpt-4-1106-preview": 128000,
-    "gpt-4": 8192,
-    "gpt-4-32k": 32768,
-    "gpt-4-0613": 8192,
-    "gpt-4-32k-0613": 32768,
-    "gpt-4-0314": 8192,  # legacy
-    "gpt-4-32k-0314": 32768,  # legacy
-    # gpt-3.5
-    "gpt-3.5-turbo-1106": 16385,
-    "gpt-3.5-turbo": 4096,
-    "gpt-3.5-turbo-16k": 16385,
-    "gpt-3.5-turbo-0613": 4096,  # legacy
-    "gpt-3.5-turbo-16k-0613": 16385,  # legacy
-    "gpt-3.5-turbo-0301": 4096,  # legacy
-}
+from eidolon_ai_sdk.system.reference_model import Specable, Reference
 
 
 class LLMModel(BaseModel):
     human_name: str
     name: str
     input_context_limit: int
     output_context_limit: int
@@ -62,47 +42,35 @@
 class LLMCallFunction(BaseModel):
     name: str = Field(..., description="The name of the function to call.")
     description: str = Field(..., description="The description of the function to call.")
     parameters: Dict[str, object] = Field(..., description="The json schema for the function parameters.")
 
 
 class LLMUnitSpec(BaseModel):
-    model: str = Field(description="The model to use for the LLM.")
-    supported_models: List[LLMModel] = Field(default=[], description="The list of supported models or leave empty for defaults.")
+    model: Reference[LLMModel]
 
 
 class LLMUnit(ProcessingUnit, Specable[LLMUnitSpec], ABC):
     model: LLMModel
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         Specable.__init__(self, **kwargs)
-
-        for model in self.get_models():
-            if model.name == self.spec.model:
-                self.model = model
-                break
-
-        if not hasattr(self, "model"):
-            raise ValueError(f"Model {self.spec.model} not found in {self.get_models()}")
+        self.model = self.spec.model.instantiate()
 
     def get_llm_capabilities(self) -> LLMCapabilities:
         return LLMCapabilities(
             input_context_limit=self.model.input_context_limit,
             output_context_limit=self.model.output_context_limit,
             supports_tools=self.model.supports_tools,
             supports_image_input=self.model.supports_image_input,
             supports_audio_input=self.model.supports_audio_input,
         )
 
     @abstractmethod
-    def get_models(self) -> List[LLMModel]:
-        pass
-
-    @abstractmethod
     async def execute_llm(
         self,
         call_context: CallContext,
         messages: List[LLMMessage],
         tools: List[LLMCallFunction],
         output_format: Union[Literal["str"], Dict[str, Any]],
     ) -> AsyncIterator[StreamEvent]:
```

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/logic_unit.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/logic_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/memory_unit.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/memory_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/cpu/processing_unit.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/cpu/processing_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/agent_memory.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/agent_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/chroma_vector_store.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/chroma_vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/document.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/document.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/embeddings.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/embeddings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from abc import ABC, abstractmethod
 from typing import Sequence, Any, AsyncGenerator, Optional, List
 
 from openai import AsyncOpenAI
 from pydantic import BaseModel, Field
 
+from eidolon_ai_sdk.cpu.llm.open_ai_connection_handler import OpenAIConnectionHandler
 from eidolon_ai_sdk.system.reference_model import Specable, AnnotatedReference
 from eidolon_ai_sdk.memory.document import Document, EmbeddedDocument
 
 
 class EmbeddingSpec(BaseModel):
     pass
 
@@ -55,28 +56,28 @@
 class NoopEmbedding(Embedding, Specable[EmbeddingSpec]):
     async def embed_text(self, text: str, **kwargs: Any) -> Sequence[float]:
         return []
 
 
 class OpenAIEmbeddingSpec(EmbeddingSpec):
     model: str = Field(default="text-embedding-ada-002", description="The name of the model to use.")
-    client: AnnotatedReference[AsyncOpenAI]
-    client_args: dict = {}
+    connection_handler: AnnotatedReference[OpenAIConnectionHandler]
 
 
 class OpenAIEmbedding(Embedding, Specable[OpenAIEmbeddingSpec]):
     llm: Optional[AsyncOpenAI] = None
 
     def __init__(self, spec: OpenAIEmbeddingSpec):
         super().__init__(spec)
         self.spec = spec
 
     async def start(self):
         await super().start()
-        self.llm = self.spec.client.instantiate(**self.spec.client_args)
+        conn_handler: OpenAIConnectionHandler = self.spec.connection_handler.instantiate()
+        self.llm = conn_handler.makeClient()
 
     async def stop(self):
         await super().stop()
         await self.llm.close()
         self.llm = None
 
     async def embed_text(self, text: str, **kwargs: Any) -> Sequence[float]:
```

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/file_memory.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/file_system_vector_store.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/file_system_vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/in_memory_file_memory.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/in_memory_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/local_file_memory.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/local_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/local_symbolic_memory.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/local_symbolic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/mongo_symbolic_memory.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/mongo_symbolic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/noop_memory.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/noop_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/s3_file_memory.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/s3_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/semantic_memory.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/semantic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/similarity_memory.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/similarity_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/memory/vector_store.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/memory/vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/authentication_processor.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/authentication_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/azure_authorizer.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/azure_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/functional_authorizer.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/functional_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/google_auth.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/google_auth.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/jwt_processor.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/jwt_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/permissions.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/permissions.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/process_authorizer.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/process_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/security_manager.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/security_manager.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/security/security_middleware.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/security/security_middleware.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/agent_contract.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/agent_contract.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/agent_controller.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/agent_controller.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/agent_machine.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/agent_machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -309,42 +309,45 @@
         """
         Create a new process. Use this method first to get a process id before calling any other action
         :param args: An optional title for the process
         :return:
         """
         controller = self._get_agent_controller(args.agent)
         if not controller:
+            logger.info(f"Agent {args.agent} does not exist")
             return JSONResponse(content={"detail": "Agent not found"}, status_code=404)
         return await controller.create_process(args.title)
 
     async def _delete_process(self, process_id: str):
         """
         Delete a process and all of its children
         """
         process_doc: ProcessDoc = await ProcessDoc.find_one(query={"_id": process_id})
         if not process_doc:
             logger.info(f"Process {process_id} does not exist")
             return JSONResponse(content={"detail": "Process Not Found"}, status_code=404)
 
         controller = self._get_agent_controller(process_doc.agent)
         if not controller:
+            logger.info(f"Agent {process_doc.agent} does not exist")
             return JSONResponse(content={"detail": "Agent not found"}, status_code=404)
         return await controller.delete_process(process_id)
 
     async def get_process_events(self, process_id: str):
         """
         Delete a process and all of its children
         """
         process_doc: ProcessDoc = await ProcessDoc.find_one(query={"_id": process_id})
         if not process_doc:
             logger.info(f"Process {process_id} does not exist")
             return JSONResponse(content={"detail": "Process Not Found"}, status_code=404)
 
         controller = self._get_agent_controller(process_doc.agent)
         if not controller:
+            logger.info(f"Agent {process_doc.agent} does not exist")
             return JSONResponse(content={"detail": "Agent not found"}, status_code=404)
         return await controller.get_process_events(process_id)
 
 
 @contextmanager
 def error_logger(filename: str = None):
     try:
```

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/dynamic_middleware.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/dynamic_middleware.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/fn_handler.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/fn_handler.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/process_file_system.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/process_file_system.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/processes.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/processes.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/reference_model.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/reference_model.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/resources/reference_resource.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/resources/reference_resource.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/system/resources/resources_base.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/system/resources/resources_base.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/util/class_utils.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/util/class_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/util/image_utils.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/util/image_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/util/replay.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/util/replay.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/util/schema_to_model.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/util/schema_to_model.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/util/str_utils.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/util/str_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/eidolon_ai_sdk/util/stream_collector.py` & `eidolon_ai_sdk-0.1.27/eidolon_ai_sdk/util/stream_collector.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/logging.conf` & `eidolon_ai_sdk-0.1.27/logging.conf`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.26/pyproject.toml` & `eidolon_ai_sdk-0.1.27/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eidolon-ai-sdk"
-version = "0.1.26"
+version = "0.1.27"
 description = "An Open Source Agent Services Framework"
 authors = ["Luke Lalor <lukehlalor@gmail.com>"]
 readme = "README.md"
 include = ["logging.conf"]
 
 [tool.poetry.urls]
 Github = "https://github.com/eidolon-ai/eidolon"
@@ -48,15 +48,15 @@
 sse-starlette = "^2.0.0"
 dill = "^0.3.8"
 typer = {extras = ["all"], version = "^0.9.0"}
 opentelemetry-instrumentation-fastapi = "^0.44b0"
 opentelemetry-instrumentation-logging = "^0.44b0"
 opentelemetry-sdk = "^1.23.0"
 eidolon-ai-mistralai = "^0.1.6a"
-eidolon-ai-client = "^0.1.5"
+eidolon-ai-client = "^0.1.6"
 eidolon-ai-usage-client =  "^0.1.0"
 boto3 = "^1.34.74"
 boto3-stubs = {extras = ["essential"], version = "^1.34.74"}
 azure-identity = "^1.16.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.4"
```

### Comparing `eidolon_ai_sdk-0.1.26/PKG-INFO` & `eidolon_ai_sdk-0.1.27/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: eidolon-ai-sdk
-Version: 0.1.26
+Version: 0.1.27
 Summary: An Open Source Agent Services Framework
 Author: Luke Lalor
 Author-email: lukehlalor@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anthropic (>=0.21.3,<0.22.0)
 Requires-Dist: authlib (>=1.3.0,<2.0.0)
 Requires-Dist: azure-identity (>=1.16.0,<2.0.0)
 Requires-Dist: boto3 (>=1.34.74,<2.0.0)
 Requires-Dist: boto3-stubs[essential] (>=1.34.74,<2.0.0)
 Requires-Dist: chromadb (>=0.4.18,<0.5.0)
 Requires-Dist: dill (>=0.3.8,<0.4.0)
-Requires-Dist: eidolon-ai-client (>=0.1.5,<0.2.0)
+Requires-Dist: eidolon-ai-client (>=0.1.6,<0.2.0)
 Requires-Dist: eidolon-ai-mistralai (>=0.1.6a,<0.2.0)
 Requires-Dist: eidolon-ai-usage-client (>=0.1.0,<0.2.0)
 Requires-Dist: esprima (>=4.0.1,<5.0.0)
 Requires-Dist: fastapi (>=0.109.0,<0.110.0)
 Requires-Dist: filetype (>=1.2.0,<2.0.0)
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: httpx-sse (>=0.4.0,<0.5.0)
```

