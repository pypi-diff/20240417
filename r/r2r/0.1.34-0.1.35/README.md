# Comparing `tmp/r2r-0.1.34.tar.gz` & `tmp/r2r-0.1.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r2r-0.1.34.tar", max compression
+gzip compressed data, was "r2r-0.1.35.tar", max compression
```

## Comparing `r2r-0.1.34.tar` & `r2r-0.1.35.tar`

### file list

```diff
@@ -1,87 +1,88 @@
--rw-r--r--   0        0        0     1082 2024-04-10 06:23:50.304037 r2r-0.1.34/LICENSE.md
--rw-r--r--   0        0        0     7195 2024-04-10 06:23:50.304037 r2r-0.1.34/README.md
--rw-r--r--   0        0        0      680 2024-04-10 06:23:50.304037 r2r-0.1.34/config.json
--rw-r--r--   0        0        0     2201 2024-04-10 06:23:50.340037 r2r-0.1.34/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/__init__.py
--rw-r--r--   0        0        0       53 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/client/__init__.py
--rw-r--r--   0        0        0     5956 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/client/base.py
--rw-r--r--   0        0        0     1123 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/core/__init__.py
--rw-r--r--   0        0        0      110 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/core/abstractions/document.py
--rw-r--r--   0        0        0      781 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/core/abstractions/output.py
--rw-r--r--   0        0        0      249 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/core/adapters/__init__.py
--rw-r--r--   0        0        0     2928 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/core/adapters/advanced/reducto.py
--rw-r--r--   0        0        0     2803 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/core/adapters/base.py
--rw-r--r--   0        0        0     2407 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/core/pipelines/embedding.py
--rw-r--r--   0        0        0     1334 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/core/pipelines/eval.py
--rw-r--r--   0        0        0     2175 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/core/pipelines/ingestion.py
--rw-r--r--   0        0        0     1515 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/core/pipelines/pipeline.py
--rw-r--r--   0        0        0     6227 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/core/pipelines/rag.py
--rw-r--r--   0        0        0      935 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/core/providers/embedding.py
--rw-r--r--   0        0        0     1015 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/core/providers/eval.py
--rw-r--r--   0        0        0     1808 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/core/providers/llm.py
--rw-r--r--   0        0        0    11873 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/core/providers/logging.py
--rw-r--r--   0        0        0     1249 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/core/providers/prompt.py
--rw-r--r--   0        0        0     3833 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/core/providers/vector_db.py
--rw-r--r--   0        0        0      256 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/core/utils/__init__.py
--rw-r--r--   0        0        0      176 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/core/utils/base.py
--rw-r--r--   0        0        0       95 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/core/utils/splitter/__init__.py
--rw-r--r--   0        0        0    66651 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/core/utils/splitter/text.py
--rw-r--r--   0        0        0      203 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/embeddings/__init__.py
--rw-r--r--   0        0        0     1676 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/embeddings/modal/base.py
--rw-r--r--   0        0        0     3311 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/embeddings/openai/base.py
--rw-r--r--   0        0        0     1923 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/embeddings/setence_transformer/base.py
--rw-r--r--   0        0        0      139 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/eval/__init__.py
--rw-r--r--   0        0        0     2169 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/eval/deepeval/base.py
--rw-r--r--   0        0        0     2710 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/eval/parea/base.py
--rw-r--r--   0        0        0        0 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/examples/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/examples/clients/__init__.py
--rw-r--r--   0        0        0     3244 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/examples/clients/run_basic_client.py
--rw-r--r--   0        0        0     4249 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/examples/clients/run_basic_client_old.py
--rw-r--r--   0        0        0     1625 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/examples/clients/run_synthetic_query_client.py
--rw-r--r--   0        0        0      689 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/examples/configs/local_llama_cpp.json
--rw-r--r--   0        0        0      687 2024-04-10 06:23:50.340037 r2r-0.1.34/r2r/examples/configs/local_ollama.json
--rw-r--r--   0        0        0   802904 2024-04-10 06:23:50.344037 r2r-0.1.34/r2r/examples/data/meditations.pdf
--rw-r--r--   0        0        0    14812 2024-04-10 06:23:50.344037 r2r-0.1.34/r2r/examples/data/test.pdf
--rw-r--r--   0        0        0  1307590 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/examples/data/the_republic.pdf
--rw-r--r--   0        0        0        0 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/examples/servers/__init__.py
--rw-r--r--   0        0        0      975 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/examples/servers/basic_pipeline.py
--rw-r--r--   0        0        0      533 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/examples/servers/reducto_pipeline.py
--rw-r--r--   0        0        0     6746 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/examples/servers/synthetic_query_pipeline.py
--rw-r--r--   0        0        0      504 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/examples/servers/web_search_pipeline.py
--rw-r--r--   0        0        0      101 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/integrations/__init__.py
--rw-r--r--   0        0        0     1839 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/integrations/exa.py
--rw-r--r--   0        0        0     1184 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/integrations/ionic.py
--rw-r--r--   0        0        0     3905 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/integrations/serper.py
--rw-r--r--   0        0        0      277 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/llms/__init__.py
--rw-r--r--   0        0        0     3602 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/llms/litellm/base.py
--rw-r--r--   0        0        0     4467 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/llms/llama_cpp/base.py
--rw-r--r--   0        0        0        0 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/llms/llama_cpp/model/__init__.py
--rw-r--r--   0        0        0     3794 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/llms/openai/base.py
--rw-r--r--   0        0        0      217 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/main/__init__.py
--rw-r--r--   0        0        0    16309 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/main/app.py
--rw-r--r--   0        0        0     5108 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/main/factory.py
--rw-r--r--   0        0        0     3280 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/main/models.py
--rw-r--r--   0        0        0    10797 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/main/utils.py
--rw-r--r--   0        0        0      541 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/pipelines/__init__.py
--rw-r--r--   0        0        0     5948 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/pipelines/basic/embedding.py
--rw-r--r--   0        0        0     1830 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/pipelines/basic/eval.py
--rw-r--r--   0        0        0     2978 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/pipelines/basic/ingestion.py
--rw-r--r--   0        0        0     1002 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/pipelines/basic/prompt_provider.py
--rw-r--r--   0        0        0     3079 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/pipelines/basic/rag.py
--rw-r--r--   0        0        0     2392 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/pipelines/web_search/rag.py
--rw-r--r--   0        0        0     6035 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/tests/end_to_end.py
--rw-r--r--   0        0        0    14812 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/tests/test.pdf
--rw-r--r--   0        0        0      539 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/vecs/__init__.py
--rw-r--r--   0        0        0      363 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/vecs/adapter/__init__.py
--rw-r--r--   0        0        0     3269 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/vecs/adapter/base.py
--rw-r--r--   0        0        0     3170 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/vecs/adapter/markdown.py
--rw-r--r--   0        0        0     1668 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/vecs/adapter/noop.py
--rw-r--r--   0        0        0     5299 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/vecs/adapter/text.py
--rw-r--r--   0        0        0     9298 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/vecs/client.py
--rw-r--r--   0        0        0    35441 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/vecs/collection.py
--rw-r--r--   0        0        0     1687 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/vecs/exc.py
--rw-r--r--   0        0        0      166 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/vector_dbs/__init__.py
--rw-r--r--   0        0        0     5881 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/vector_dbs/local/base.py
--rw-r--r--   0        0        0     5607 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/vector_dbs/pg_vector/base.py
--rw-r--r--   0        0        0     7125 2024-04-10 06:23:50.352037 r2r-0.1.34/r2r/vector_dbs/qdrant/base.py
--rw-r--r--   0        0        0     9636 1970-01-01 00:00:00.000000 r2r-0.1.34/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-04-17 01:01:26.034450 r2r-0.1.35/LICENSE.md
+-rw-r--r--   0        0        0     7421 2024-04-17 01:01:26.034450 r2r-0.1.35/README.md
+-rw-r--r--   0        0        0      680 2024-04-17 01:01:26.034450 r2r-0.1.35/config.json
+-rw-r--r--   0        0        0     2218 2024-04-17 01:01:26.066450 r2r-0.1.35/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/__init__.py
+-rw-r--r--   0        0        0       53 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/client/__init__.py
+-rw-r--r--   0        0        0     5956 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/client/base.py
+-rw-r--r--   0        0        0     1121 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/__init__.py
+-rw-r--r--   0        0        0      139 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/abstractions/document.py
+-rw-r--r--   0        0        0      781 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/abstractions/output.py
+-rw-r--r--   0        0        0      249 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/adapters/__init__.py
+-rw-r--r--   0        0        0     2928 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/adapters/advanced/reducto.py
+-rw-r--r--   0        0        0     2803 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/adapters/base.py
+-rw-r--r--   0        0        0     1654 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/pipelines/embedding.py
+-rw-r--r--   0        0        0     1334 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/pipelines/eval.py
+-rw-r--r--   0        0        0     1815 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/pipelines/ingestion.py
+-rw-r--r--   0        0        0     1515 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/pipelines/pipeline.py
+-rw-r--r--   0        0        0     6227 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/pipelines/rag.py
+-rw-r--r--   0        0        0      935 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/providers/embedding.py
+-rw-r--r--   0        0        0     1015 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/providers/eval.py
+-rw-r--r--   0        0        0     1808 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/providers/llm.py
+-rw-r--r--   0        0        0    11889 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/providers/logging.py
+-rw-r--r--   0        0        0     1249 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/providers/prompt.py
+-rw-r--r--   0        0        0     3833 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/providers/vector_db.py
+-rw-r--r--   0        0        0      256 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/utils/__init__.py
+-rw-r--r--   0        0        0      176 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/utils/base.py
+-rw-r--r--   0        0        0       95 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/utils/splitter/__init__.py
+-rw-r--r--   0        0        0    66651 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/core/utils/splitter/text.py
+-rw-r--r--   0        0        0      203 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/embeddings/__init__.py
+-rw-r--r--   0        0        0     1676 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/embeddings/modal/base.py
+-rw-r--r--   0        0        0     3311 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/embeddings/openai/base.py
+-rw-r--r--   0        0        0     1923 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/embeddings/setence_transformer/base.py
+-rw-r--r--   0        0        0      139 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/eval/__init__.py
+-rw-r--r--   0        0        0     2169 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/eval/deepeval/base.py
+-rw-r--r--   0        0        0     2710 2024-04-17 01:01:26.066450 r2r-0.1.35/r2r/eval/parea/base.py
+-rw-r--r--   0        0        0        0 2024-04-17 01:01:26.070450 r2r-0.1.35/r2r/examples/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 01:01:26.070450 r2r-0.1.35/r2r/examples/clients/__init__.py
+-rw-r--r--   0        0        0     3244 2024-04-17 01:01:26.070450 r2r-0.1.35/r2r/examples/clients/run_basic_client.py
+-rw-r--r--   0        0        0     4063 2024-04-17 01:01:26.070450 r2r-0.1.35/r2r/examples/clients/run_basic_client_old.py
+-rw-r--r--   0        0        0     1625 2024-04-17 01:01:26.070450 r2r-0.1.35/r2r/examples/clients/run_synthetic_query_client.py
+-rw-r--r--   0        0        0      760 2024-04-17 01:01:26.070450 r2r-0.1.35/r2r/examples/configs/local_embedding_qdrant.json
+-rw-r--r--   0        0        0      689 2024-04-17 01:01:26.070450 r2r-0.1.35/r2r/examples/configs/local_llama_cpp.json
+-rw-r--r--   0        0        0      687 2024-04-17 01:01:26.070450 r2r-0.1.35/r2r/examples/configs/local_ollama.json
+-rw-r--r--   0        0        0   802904 2024-04-17 01:01:26.070450 r2r-0.1.35/r2r/examples/data/meditations.pdf
+-rw-r--r--   0        0        0    14812 2024-04-17 01:01:26.074450 r2r-0.1.35/r2r/examples/data/test.pdf
+-rw-r--r--   0        0        0  1307590 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/examples/data/the_republic.pdf
+-rw-r--r--   0        0        0        0 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/examples/servers/__init__.py
+-rw-r--r--   0        0        0     1139 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/examples/servers/basic_pipeline.py
+-rw-r--r--   0        0        0      529 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/examples/servers/reducto_pipeline.py
+-rw-r--r--   0        0        0     6746 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/examples/servers/synthetic_query_pipeline.py
+-rw-r--r--   0        0        0      479 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/examples/servers/web_search_pipeline.py
+-rw-r--r--   0        0        0      147 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/integrations/__init__.py
+-rw-r--r--   0        0        0     1839 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/integrations/exa.py
+-rw-r--r--   0        0        0     1571 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/integrations/ionic.py
+-rw-r--r--   0        0        0     3905 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/integrations/serper.py
+-rw-r--r--   0        0        0      277 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/llms/__init__.py
+-rw-r--r--   0        0        0     3602 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/llms/litellm/base.py
+-rw-r--r--   0        0        0     4467 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/llms/llama_cpp/base.py
+-rw-r--r--   0        0        0        0 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/llms/llama_cpp/model/__init__.py
+-rw-r--r--   0        0        0     3794 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/llms/openai/base.py
+-rw-r--r--   0        0        0      217 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/main/__init__.py
+-rw-r--r--   0        0        0    16309 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/main/app.py
+-rw-r--r--   0        0        0     5108 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/main/factory.py
+-rw-r--r--   0        0        0     3278 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/main/models.py
+-rw-r--r--   0        0        0    10941 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/main/utils.py
+-rw-r--r--   0        0        0      493 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/pipelines/__init__.py
+-rw-r--r--   0        0        0     6331 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/pipelines/basic/embedding.py
+-rw-r--r--   0        0        0     1830 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/pipelines/basic/eval.py
+-rw-r--r--   0        0        0     3059 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/pipelines/basic/ingestion.py
+-rw-r--r--   0        0        0     1002 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/pipelines/basic/prompt_provider.py
+-rw-r--r--   0        0        0     3080 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/pipelines/basic/rag.py
+-rw-r--r--   0        0        0     3766 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/pipelines/web_search/rag.py
+-rw-r--r--   0        0        0     6035 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/tests/end_to_end.py
+-rw-r--r--   0        0        0    14812 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/tests/test.pdf
+-rw-r--r--   0        0        0      539 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/vecs/__init__.py
+-rw-r--r--   0        0        0      363 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/vecs/adapter/__init__.py
+-rw-r--r--   0        0        0     3269 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/vecs/adapter/base.py
+-rw-r--r--   0        0        0     3170 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/vecs/adapter/markdown.py
+-rw-r--r--   0        0        0     1668 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/vecs/adapter/noop.py
+-rw-r--r--   0        0        0     5299 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/vecs/adapter/text.py
+-rw-r--r--   0        0        0     9298 2024-04-17 01:01:26.078450 r2r-0.1.35/r2r/vecs/client.py
+-rw-r--r--   0        0        0    35441 2024-04-17 01:01:26.082450 r2r-0.1.35/r2r/vecs/collection.py
+-rw-r--r--   0        0        0     1687 2024-04-17 01:01:26.082450 r2r-0.1.35/r2r/vecs/exc.py
+-rw-r--r--   0        0        0      166 2024-04-17 01:01:26.082450 r2r-0.1.35/r2r/vector_dbs/__init__.py
+-rw-r--r--   0        0        0     5919 2024-04-17 01:01:26.082450 r2r-0.1.35/r2r/vector_dbs/local/base.py
+-rw-r--r--   0        0        0     5607 2024-04-17 01:01:26.082450 r2r-0.1.35/r2r/vector_dbs/pg_vector/base.py
+-rw-r--r--   0        0        0     7125 2024-04-17 01:01:26.082450 r2r-0.1.35/r2r/vector_dbs/qdrant/base.py
+-rw-r--r--   0        0        0     9880 1970-01-01 00:00:00.000000 r2r-0.1.35/PKG-INFO
```

### Comparing `r2r-0.1.34/LICENSE.md` & `r2r-0.1.35/LICENSE.md`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/README.md` & `r2r-0.1.35/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,24 +40,26 @@
 
 [Join the Discord server](https://discord.gg/p6KqD2kjtB)
 
 [R2R Docs Quickstart](https://r2r-docs.sciphi.ai/getting-started/quick-install)
 
 [SciPhi Cloud](https://docs.sciphi.ai/)
 
+[Local RAG Tutorial](https://r2r-docs.sciphi.ai/tutorials/local_rag)
+
 ## Quick Install:
 
 ```bash
 # use the `'r2r[all]'` to download all required deps
 pip install 'r2r[eval]'
 
 # setup env 
 export OPENAI_API_KEY=sk-...
 # Set `LOCAL_DB_PATH` for local testing
-export LOCAL_DB_PATH=local.sqlite
+export LOCAL_DB_PATH=local.sqlite # robust providers available (e.g. qdrant, pgvector, ..)
 
 # OR do `vim .env.example && cp .env.example .env`
 # INCLUDE secrets and modify config.json
 # if using cloud providers (e.g. pgvector, qdrant, ...)
 ```
 
 ## Docker:
@@ -65,23 +67,23 @@
 ```bash
 docker pull emrgntcmplxty/r2r:latest
 
 # Choose from CONFIG_OPTION in {`default`, `local_ollama`}
 # For cloud deployment, select `default` and pass `--env-file .env`
 # For local deployment, select `local_ollama`
 docker run -d --name r2r_container -p 8000:8000 -e CONFIG_OPTION=local_ollama  emrgntcmplxty/r2r:latest
-
 ```
 
 ## Basic Example
 
 [`basic_pipeline.py`](r2r/examples/servers/basic_pipeline.py): Execute this script to initiate the default **backend server**. It establishes a basic RAG pipeline that encompasses ingestion, embedding, and RAG processes, all accessible via FastAPI.
 
    ```bash
    # launch the server
+   # Do `export CONFIG_OPTION=local_ollama` to run the pipeline with local ollama instead of OpenAI
    python -m r2r.examples.servers.basic_pipeline
    ```
 
 [`run_basic_client.py`](r2r/examples/clients/run_basic_client.py): This **client script** should be executed subsequent to the server startup above. It facilitates the upload of text entries and PDFs to the server using the Python client and demonstrates the management of document and user-level vectors through its built-in features.
 
    ```bash
    # run the client
```

#### html2text {}

```diff
@@ -18,43 +18,47 @@
 deployment. ## Demo(s) Using the cloud application to deploy the pre-built
 basic pipeline: https://www.loom.com/share/e3b934b554484787b005702ced650ac9
 Note - the example above uses [SciPhi Cloud](https://app.sciphi.ai) to pair
 with the R2R framework for deployment and observability. SciPhi is working to
 launch a self-hosted version of their cloud platform as R2R matures. ## Links
 [Join the Discord server](https://discord.gg/p6KqD2kjtB) [R2R Docs Quickstart]
 (https://r2r-docs.sciphi.ai/getting-started/quick-install) [SciPhi Cloud]
-(https://docs.sciphi.ai/) ## Quick Install: ```bash # use the `'r2r[all]'` to
+(https://docs.sciphi.ai/) [Local RAG Tutorial](https://r2r-docs.sciphi.ai/
+tutorials/local_rag) ## Quick Install: ```bash # use the `'r2r[all]'` to
 download all required deps pip install 'r2r[eval]' # setup env export
 OPENAI_API_KEY=sk-... # Set `LOCAL_DB_PATH` for local testing export
-LOCAL_DB_PATH=local.sqlite # OR do `vim .env.example && cp .env.example .env` #
-INCLUDE secrets and modify config.json # if using cloud providers (e.g.
-pgvector, qdrant, ...) ``` ## Docker: ```bash docker pull emrgntcmplxty/r2r:
-latest # Choose from CONFIG_OPTION in {`default`, `local_ollama`} # For cloud
-deployment, select `default` and pass `--env-file .env` # For local deployment,
-select `local_ollama` docker run -d --name r2r_container -p 8000:8000 -
+LOCAL_DB_PATH=local.sqlite # robust providers available (e.g. qdrant, pgvector,
+..) # OR do `vim .env.example && cp .env.example .env` # INCLUDE secrets and
+modify config.json # if using cloud providers (e.g. pgvector, qdrant, ...) ```
+## Docker: ```bash docker pull emrgntcmplxty/r2r:latest # Choose from
+CONFIG_OPTION in {`default`, `local_ollama`} # For cloud deployment, select
+`default` and pass `--env-file .env` # For local deployment, select
+`local_ollama` docker run -d --name r2r_container -p 8000:8000 -
 e CONFIG_OPTION=local_ollama emrgntcmplxty/r2r:latest ``` ## Basic Example
 [`basic_pipeline.py`](r2r/examples/servers/basic_pipeline.py): Execute this
 script to initiate the default **backend server**. It establishes a basic RAG
 pipeline that encompasses ingestion, embedding, and RAG processes, all
-accessible via FastAPI. ```bash # launch the server python -
-m r2r.examples.servers.basic_pipeline ``` [`run_basic_client.py`](r2r/examples/
-clients/run_basic_client.py): This **client script** should be executed
-subsequent to the server startup above. It facilitates the upload of text
-entries and PDFs to the server using the Python client and demonstrates the
-management of document and user-level vectors through its built-in features.
-```bash # run the client python -m r2r.examples.clients.run_basic_client ingest
-python -m r2r.examples.clients.run_basic_client search --query="What is the
-meaning of life?" ``` ### Running Basic Local RAG [Refer here](https://r2r-
-docs.sciphi.ai/tutorials/local_rag) for a tutorial on how to modify the
-commands above to use local providers. ## Synthetic Queries Example
-[`synthetic_query_pipeline.py`](r2r/examples/servers/
-synthetic_query_pipeline.py): Execute this script to start a backend server
-equipped with an advanced pipeline. This pipeline is designed to create
-synthetic queries, enhancing the RAG system's learning and performance. ```bash
-# launch the server python -m r2r.examples.servers.synthetic_query_pipeline ```
+accessible via FastAPI. ```bash # launch the server # Do `export
+CONFIG_OPTION=local_ollama` to run the pipeline with local ollama instead of
+OpenAI python -m r2r.examples.servers.basic_pipeline ```
+[`run_basic_client.py`](r2r/examples/clients/run_basic_client.py): This
+**client script** should be executed subsequent to the server startup above. It
+facilitates the upload of text entries and PDFs to the server using the Python
+client and demonstrates the management of document and user-level vectors
+through its built-in features. ```bash # run the client python -
+m r2r.examples.clients.run_basic_client ingest python -
+m r2r.examples.clients.run_basic_client search --query="What is the meaning of
+life?" ``` ### Running Basic Local RAG [Refer here](https://r2r-docs.sciphi.ai/
+tutorials/local_rag) for a tutorial on how to modify the commands above to use
+local providers. ## Synthetic Queries Example [`synthetic_query_pipeline.py`]
+(r2r/examples/servers/synthetic_query_pipeline.py): Execute this script to
+start a backend server equipped with an advanced pipeline. This pipeline is
+designed to create synthetic queries, enhancing the RAG system's learning and
+performance. ```bash # launch the server python -
+m r2r.examples.servers.synthetic_query_pipeline ```
 [`run_synthetic_query_client.py`](r2r/examples/clients/
 run_synthetic_query_client.py): Use this client script after the synthetic
 query pipeline is running. It's tailored for use with the synthetic query
 pipeline, demonstrating the improved features of the RAG system. ```bash # run
 the client python -m r2r.examples.clients.run_synthetic_query_client ``` ##
 Extra Examples [`reducto_pipeline.py`](r2r/examples/servers/
 reducto_pipeline.py): Launch this script to activate a backend server that
```

### Comparing `r2r-0.1.34/config.json` & `r2r-0.1.35/config.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9910714285714286%*

 * *Differences: {"'embedding'": "{'model': 'text-embedding-3-large'}"}*

```diff
@@ -2,15 +2,15 @@
     "app": {
         "max_file_size_in_mb": 100,
         "max_logs": 100
     },
     "embedding": {
         "batch_size": 32,
         "dimension": 1536,
-        "model": "text-embedding-3-small",
+        "model": "text-embedding-3-large",
         "provider": "openai"
     },
     "evals": {
         "frequency": 1.0,
         "provider": "parea"
     },
     "ingestion": {
```

### Comparing `r2r-0.1.34/pyproject.toml` & `r2r-0.1.35/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "setuptools", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "r2r"
-version = "0.1.34"
+version = "0.1.35"
 description = "SciPhi R2R"
 authors = ["Owen Colegrove <owen@sciphi.ai>"]
 license = "MIT"
 readme = "README.md"
 include = ["config.json"]
 
 [tool.poetry.dependencies]
@@ -56,15 +56,15 @@
 deepeval = ["deepeval"]
 eval = ["parea-ai"]
 ionic = ["ionic-api-sdk"]
 reducto = ["boto3"]
 exa = ["exa-py"]
 sentence_transformers = ["sentence-transformers"]
 local_llm = ["llama-cpp-python", "sentence-transformers"]
-all = ["tiktoken", "datasets", "qdrant_client", "psycopg2-binary", "sentry-sdk", "parea-ai", "boto3", "exa-py", "llama-cpp-python"]
+all = ["tiktoken", "datasets", "qdrant_client", "psycopg2-binary", "sentry-sdk", "parea-ai", "boto3", "exa-py", "llama-cpp-python", "ionic-api-sdk"]
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.3.0"
 flake8 = "6.1.0"
 isort = "5.12.0"
 mypy = "^1.5.1"
```

### Comparing `r2r-0.1.34/r2r/client/base.py` & `r2r-0.1.35/r2r/client/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/core/__init__.py` & `r2r-0.1.35/r2r/core/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .abstractions.document import BasicDocument
+from .abstractions.document import DocumentPage
 from .abstractions.output import RAGPipelineOutput
 from .pipelines.embedding import EmbeddingPipeline
 from .pipelines.eval import EvalPipeline
 from .pipelines.ingestion import IngestionPipeline
 from .pipelines.rag import RAGPipeline
 from .providers.embedding import EmbeddingProvider
 from .providers.eval import EvalProvider
@@ -12,15 +12,15 @@
 from .providers.vector_db import (
     VectorDBProvider,
     VectorEntry,
     VectorSearchResult,
 )
 
 __all__ = [
-    "BasicDocument",
+    "DocumentPage",
     "DefaultPromptProvider",
     "RAGPipelineOutput",
     "EmbeddingPipeline",
     "EvalPipeline",
     "IngestionPipeline",
     "RAGPipeline",
     "LoggingDatabaseConnection",
```

### Comparing `r2r-0.1.34/r2r/core/abstractions/output.py` & `r2r-0.1.35/r2r/core/abstractions/output.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/core/adapters/advanced/reducto.py` & `r2r-0.1.35/r2r/core/adapters/advanced/reducto.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/core/adapters/base.py` & `r2r-0.1.35/r2r/core/adapters/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/core/pipelines/embedding.py` & `r2r-0.1.35/r2r/core/pipelines/embedding.py`

 * *Files 14% similar despite different names*

```diff
@@ -55,26 +55,8 @@
         pass
 
     @abstractmethod
     def store_chunks(self, chunks: list[VectorEntry], *args, **kwargs) -> None:
         pass
 
     def run(self, document: Any, **kwargs):
-        self.initialize_pipeline()
-        logger.debug(
-            f"Running the `BasicEmbeddingPipeline` with pipeline_run_info={self.pipeline_run_info}."
-        )
-
-        documents = [document] if not isinstance(document, list) else document
-
-        for document in documents:
-            transformed_text = self.transform_text(document.text)
-            chunks = self.chunk_text(transformed_text)
-            transformed_chunks = self.transform_chunks(chunks, [])
-            embeddings = self.embed_chunks(transformed_chunks)
-            self.store_chunks(
-                [
-                    VectorEntry(document.id, embedding, document.metadata)
-                    for embedding in embeddings
-                ],
-                **kwargs,
-            )
+        pass
```

### Comparing `r2r-0.1.34/r2r/core/pipelines/eval.py` & `r2r-0.1.35/r2r/core/pipelines/eval.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/core/pipelines/ingestion.py` & `r2r-0.1.35/r2r/core/pipelines/ingestion.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import abstractmethod
 from typing import Any, Iterator, Optional
 
-from ..abstractions.document import BasicDocument
+from ..abstractions.document import DocumentPage
 from ..adapters import Adapter
 from ..providers.logging import LoggingDatabaseConnection
 from ..utils import generate_run_id
 from .pipeline import Pipeline
 
 
 class IngestionPipeline(Pipeline):
@@ -31,42 +31,34 @@
         Returns a list of supported data types.
         """
         pass
 
     @abstractmethod
     def process_data(
         self, entry_type: str, entry_data: Any
-    ) -> Iterator[BasicDocument]:
+    ) -> Iterator[DocumentPage]:
         """
-        Process data into plaintext based on the data type and yield BasicDocument objects.
+        Process data into plaintext based on the data type and yield DocumentPage objects.
         """
         pass
 
     @abstractmethod
     def parse_entry(
         self, entry_type: str, entry_data: Any
-    ) -> Iterator[BasicDocument]:
+    ) -> Iterator[DocumentPage]:
         """
-        Parse entry data into plaintext based on the entry type and yield BasicDocument objects.
+        Parse entry data into plaintext based on the entry type and yield DocumentPage objects.
         """
         pass
 
     def run(
         self,
         document_id: str,
         blobs: dict[str, Any],
         metadata: Optional[dict] = None,
         **kwargs,
-    ) -> Iterator[BasicDocument]:
+    ) -> Iterator[DocumentPage]:
         """
         Run the appropriate parsing method based on the data type and whether the data is a file or an entry.
-        Yields the processed BasicDocument objects.
+        Yields the processed DocumentPage objects.
         """
-        self.initialize_pipeline()
-
-        if len(blobs) == 0:
-            raise ValueError("No blobs provided to process.")
-
-        for entry_type, blob in blobs.items():
-            if entry_type not in self.supported_types:
-                raise ValueError(f"IngestionType {entry_type} not supported.")
-            yield from self.parse_entry(entry_type, blob)
+        pass
```

### Comparing `r2r-0.1.34/r2r/core/pipelines/pipeline.py` & `r2r-0.1.35/r2r/core/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/core/pipelines/rag.py` & `r2r-0.1.35/r2r/core/pipelines/rag.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/core/providers/embedding.py` & `r2r-0.1.35/r2r/core/providers/embedding.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/core/providers/eval.py` & `r2r-0.1.35/r2r/core/providers/eval.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/core/providers/llm.py` & `r2r-0.1.35/r2r/core/providers/llm.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/core/providers/logging.py` & `r2r-0.1.35/r2r/core/providers/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         return logs
 
 
 class LocalLoggingProvider(LoggingProvider):
     def __init__(self, collection_name="logs"):
         self.conn = None
         self.collection_name = collection_name
-        logging_path = os.getenv("LOCAL_DB_PATH")
+        logging_path = os.getenv("LOCAL_DB_PATH", "local.sqlite")
         if not logging_path:
             raise ValueError(
                 "Please set the environment variable LOCAL_DB_PATH to run `LoggingDatabaseConnection` with `local`."
             )
         self.logging_path = logging_path
         self.db_module = self._import_db_module()
         self._init()
```

### Comparing `r2r-0.1.34/r2r/core/providers/prompt.py` & `r2r-0.1.35/r2r/core/providers/prompt.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/core/providers/vector_db.py` & `r2r-0.1.35/r2r/core/providers/vector_db.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/core/utils/splitter/text.py` & `r2r-0.1.35/r2r/core/utils/splitter/text.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/embeddings/modal/base.py` & `r2r-0.1.35/r2r/embeddings/modal/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/embeddings/openai/base.py` & `r2r-0.1.35/r2r/embeddings/openai/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/embeddings/setence_transformer/base.py` & `r2r-0.1.35/r2r/embeddings/setence_transformer/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/eval/deepeval/base.py` & `r2r-0.1.35/r2r/eval/deepeval/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/eval/parea/base.py` & `r2r-0.1.35/r2r/eval/parea/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/examples/clients/run_basic_client.py` & `r2r-0.1.35/r2r/examples/clients/run_basic_client.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/examples/clients/run_basic_client_old.py` & `r2r-0.1.35/r2r/examples/clients/run_basic_client_old.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,119 +19,119 @@
     {"txt": "This is a test entry"},
     {"tags": ["example", "test"]},
     do_upsert=True,
 )
 print(f"Upsert entry response:\n{entry_response}\n\n")
 
 
-# entry_response = client.add_entry(
-#     generate_id_from_label("doc 1"),
-#     {"txt": "This is a test entry"},
-#     {"tags": ["example", "test"]},
-#     do_upsert=False,
-# )
-# print(f"Copy same entry response:\n{entry_response}\n\n")
-
-
-# print("Upserting entries to remote db...")
-# # Upsert multiple entries
-# entries = [
-#     {
-#         "document_id": generate_id_from_label("doc 2"),
-#         "blobs": {"txt": "Second test entry"},
-#         "metadata": {"tags": "bulk"},
-#     },
-#     {
-#         "document_id": generate_id_from_label("doc 3"),
-#         "blobs": {"txt": "Third test entry"},
-#         "metadata": {"tags": "example"},
-#     },
-# ]
-# bulk_upsert_response = client.add_entries(entries, do_upsert=True)
-# print(f"Upsert entries response:\n{bulk_upsert_response}\n\n")
-
-# # Perform a search
-# print("Searching remote db...")
-# search_response = client.search("test", 5)
-# print(f"Search response:\n{search_response}\n\n")
-
-# print("Searching remote db with filter...")
-# # Perform a search w/ filter
-# filtered_search_response = client.search("test", 5, filters={"tags": "bulk"})
-# print(f"Search response w/ filter:\n{filtered_search_response}\n\n")
-
-# print("Deleting sample document in remote db...")
-# # Delete a document
-# response = client.filtered_deletion(
-#     "document_id", generate_id_from_label("doc 2")
-# )
-# print(f"Deletion response:\n{response}\n\n")
-
-# print("Searching remote db with filter after deletion...")
-# # Perform a search w/ filter after deletion
-# post_deletion_filtered_search_response = client.search(
-#     "test", 5, filters={"tags": "bulk"}
-# )
-# print(
-#     f"Search response w/ filter+deletion:\n{post_deletion_filtered_search_response}\n\n"
-# )
-
-# # Example file path for upload
-# # get file directory
-# current_file_directory = os.path.dirname(os.path.realpath(__file__))
-
-# file_path = os.path.join(current_file_directory, "..", "data", "test.pdf")
-
-# print(f"Uploading and processing file: {file_path}...")
-# # # Upload and process a file
-# metadata = {"tags": ["example", "test"]}
-# upload_pdf_response = client.upload_and_process_file(
-#     generate_id_from_label("pdf 1"), file_path, metadata, None
-# )
-# print(f"Upload test pdf response:\n{upload_pdf_response}\n\n")
-
-# print("Searching remote db after upload...")
-# # Perform a search on this file
-# pdf_filtered_search_response = client.search(
-#     "what is a cool physics equation?",
-#     5,
-#     filters={"document_id": generate_id_from_label("pdf 1")},
-# )
-# print(
-#     f"Search response w/ uploaded pdf filter:\n{pdf_filtered_search_response}\n"
-# )
-
-
-# print("Performing RAG...")
-# # Perform a search on this file
-# pdf_filtered_search_response = client.rag_completion(
-#     "Are there any test documents?",
-#     5,
-#     filters={"document_id": generate_id_from_label("pdf 1")},
-# )
-# print(
-#     f"Search response w/ uploaded pdf filter:\n{pdf_filtered_search_response}\n"
-# )
-
-# print("Performing RAG with streaming...")
-
-
-# # Perform a RAG completion with streaming
-# async def stream_rag_completion():
-#     async for chunk in client.stream_rag_completion(
-#         "Are there any test documents?",
-#         5,
-#         filters={"document_id": generate_id_from_label("pdf 1")},
-#         generation_config={"stream": True},
-#     ):
-#         print(chunk, end="", flush=True)
-
-
-# asyncio.run(stream_rag_completion())
-
-# print("Fetching logs after all steps...")
-# logs_response = client.get_logs()
-# print(f"Logs response:\n{logs_response}\n")
-
-# print("Fetching logs summary after all steps...")
-# logs_summary_response = client.get_logs_summary()
-# print(f"Logs summary response:\n{logs_summary_response}\n")
+entry_response = client.add_entry(
+    generate_id_from_label("doc 1"),
+    {"txt": "This is a test entry"},
+    {"tags": ["example", "test"]},
+    do_upsert=False,
+)
+print(f"Copy same entry response:\n{entry_response}\n\n")
+
+
+print("Upserting entries to remote db...")
+# Upsert multiple entries
+entries = [
+    {
+        "document_id": generate_id_from_label("doc 2"),
+        "blobs": {"txt": "Second test entry"},
+        "metadata": {"tags": "bulk"},
+    },
+    {
+        "document_id": generate_id_from_label("doc 3"),
+        "blobs": {"txt": "Third test entry"},
+        "metadata": {"tags": "example"},
+    },
+]
+bulk_upsert_response = client.add_entries(entries, do_upsert=True)
+print(f"Upsert entries response:\n{bulk_upsert_response}\n\n")
+
+# Perform a search
+print("Searching remote db...")
+search_response = client.search("test", 5)
+print(f"Search response:\n{search_response}\n\n")
+
+print("Searching remote db with filter...")
+# Perform a search w/ filter
+filtered_search_response = client.search("test", 5, filters={"tags": "bulk"})
+print(f"Search response w/ filter:\n{filtered_search_response}\n\n")
+
+print("Deleting sample document in remote db...")
+# Delete a document
+response = client.filtered_deletion(
+    "document_id", generate_id_from_label("doc 2")
+)
+print(f"Deletion response:\n{response}\n\n")
+
+print("Searching remote db with filter after deletion...")
+# Perform a search w/ filter after deletion
+post_deletion_filtered_search_response = client.search(
+    "test", 5, filters={"tags": "bulk"}
+)
+print(
+    f"Search response w/ filter+deletion:\n{post_deletion_filtered_search_response}\n\n"
+)
+
+# Example file path for upload
+# get file directory
+current_file_directory = os.path.dirname(os.path.realpath(__file__))
+
+file_path = os.path.join(current_file_directory, "..", "data", "test.pdf")
+
+print(f"Uploading and processing file: {file_path}...")
+# # Upload and process a file
+metadata = {"tags": ["example", "test"]}
+upload_pdf_response = client.upload_and_process_file(
+    generate_id_from_label("pdf 1"), file_path, metadata, None
+)
+print(f"Upload test pdf response:\n{upload_pdf_response}\n\n")
+
+print("Searching remote db after upload...")
+# Perform a search on this file
+pdf_filtered_search_response = client.search(
+    "what is a cool physics equation?",
+    5,
+    filters={"document_id": generate_id_from_label("pdf 1")},
+)
+print(
+    f"Search response w/ uploaded pdf filter:\n{pdf_filtered_search_response}\n"
+)
+
+
+print("Performing RAG...")
+# Perform a search on this file
+pdf_filtered_search_response = client.rag_completion(
+    "Are there any test documents?",
+    5,
+    filters={"document_id": generate_id_from_label("pdf 1")},
+)
+print(
+    f"Search response w/ uploaded pdf filter:\n{pdf_filtered_search_response}\n"
+)
+
+print("Performing RAG with streaming...")
+
+
+# Perform a RAG completion with streaming
+async def stream_rag_completion():
+    async for chunk in client.stream_rag_completion(
+        "Are there any test documents?",
+        5,
+        filters={"document_id": generate_id_from_label("pdf 1")},
+        generation_config={"stream": True},
+    ):
+        print(chunk, end="", flush=True)
+
+
+asyncio.run(stream_rag_completion())
+
+print("Fetching logs after all steps...")
+logs_response = client.get_logs()
+print(f"Logs response:\n{logs_response}\n")
+
+print("Fetching logs summary after all steps...")
+logs_summary_response = client.get_logs_summary()
+print(f"Logs summary response:\n{logs_summary_response}\n")
```

### Comparing `r2r-0.1.34/r2r/examples/clients/run_synthetic_query_client.py` & `r2r-0.1.35/r2r/examples/clients/run_synthetic_query_client.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/examples/configs/local_llama_cpp.json` & `r2r-0.1.35/r2r/examples/configs/local_llama_cpp.json`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/examples/configs/local_ollama.json` & `r2r-0.1.35/r2r/examples/configs/local_ollama.json`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/examples/data/meditations.pdf` & `r2r-0.1.35/r2r/examples/data/meditations.pdf`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/examples/data/test.pdf` & `r2r-0.1.35/r2r/examples/data/test.pdf`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/examples/data/the_republic.pdf` & `r2r-0.1.35/r2r/examples/data/the_republic.pdf`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/examples/servers/basic_pipeline.py` & `r2r-0.1.35/r2r/examples/servers/basic_pipeline.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,33 +8,35 @@
 current_file_path = os.path.dirname(__file__)
 configs_path = os.path.join(current_file_path, "..", "configs")
 
 OPTIONS = {
     "default": None,
     "local_ollama": os.path.join(configs_path, "local_ollama.json"),
     "local_llama_cpp": os.path.join(configs_path, "local_llama_cpp.json"),
+    "local_embedding_qdrant": os.path.join(configs_path, "local_embedding_qdrant.json"),
 }
 
 
 def create_app(config_name: str = "default"):
+    config_name = os.getenv("CONFIG_OPTION") or config_name
     config_path = OPTIONS[config_name]
 
     app = E2EPipelineFactory.create_pipeline(
         config=R2RConfig.load_config(config_path)
     )
     return app
 
 
-app = create_app()
-
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description="R2R Pipeline")
     parser.add_argument(
         "--config",
         type=str,
         default="default",
         choices=OPTIONS.keys(),
         help="Configuration option for the pipeline",
     )
     args, _ = parser.parse_known_args()
 
+    app = create_app(args.config)
+
     uvicorn.run(app, host="0.0.0.0", port=8000)
```

### Comparing `r2r-0.1.34/r2r/examples/servers/reducto_pipeline.py` & `r2r-0.1.35/r2r/examples/servers/reducto_pipeline.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import uvicorn
 
 from r2r.core.adapters import ReductoAdapter
 from r2r.main import E2EPipelineFactory, R2RConfig
 from r2r.pipelines import IngestionType
 
-# Read more about the configuration in the documentation [https://r2r-docs.sciphi.ai/core-features/factory]
+# Read more about the configuration in the documentation [https://r2r-docs.sciphi.ai/deep-dive/factory]
 app = E2EPipelineFactory.create_pipeline(
     config=R2RConfig.load_config(),
     adapters={
         IngestionType.PDF: ReductoAdapter(),
     },
 )
```

### Comparing `r2r-0.1.34/r2r/examples/servers/synthetic_query_pipeline.py` & `r2r-0.1.35/r2r/examples/servers/synthetic_query_pipeline.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/integrations/exa.py` & `r2r-0.1.35/r2r/integrations/exa.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/integrations/ionic.py` & `r2r-0.1.35/r2r/integrations/ionic.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,53 @@
+
 import os
 from typing import Optional
 
 
 class IonicClient:
     def __init__(self, api_key: str = os.getenv("IONIC_API_KEY")) -> None:
         if not api_key:
             raise ValueError(
-                "Please set the `IONIC_API_KEY` env var or pass a parameter to use `IonicCLient`."
+                "Please set the `IONIC_API_KEY` env var or pass a parameter to use `IonicClient`."
             )
 
         # temp local import for dependency mgmt
         from ionic import Ionic as IonicSDK
 
         self.client = IonicSDK(api_key_header=api_key)
 
     def query(
         self,
         query: str,
-        num_results: Optional[int] = 5,
+        num_results: Optional[int] = 10,
     ):
         # temp local import for dependency mgmt
-        from ionic.models.components import Query as SDKQuery
         from ionic.models.components import QueryAPIRequest
+        from ionic.models.components import Query as SDKQuery
         from ionic.models.operations import QueryResponse, QuerySecurity
 
         request = QueryAPIRequest(
-            query=SDKQuery(query=query, num_results=num_results)
+            query=SDKQuery(
+                query=query,
+                num_results=num_results
+            )
         )
+
         response: QueryResponse = self.client.query(
             request=request,
             security=QuerySecurity(),
         )
 
         return [
-            product
+            {
+                "name": product.name,
+                "price": product.price,
+                "brand_name": product.brand_name,
+                "upc": product.upc,
+                "merchant_name": product.merchant_name,
+                "thumbnail": product.thumbnail,
+'link': product.links[0].url if product.links else None,
+            }
             for result in response.query_api_response.results
             for product in result.products
         ]
+
```

### Comparing `r2r-0.1.34/r2r/integrations/serper.py` & `r2r-0.1.35/r2r/integrations/serper.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/llms/litellm/base.py` & `r2r-0.1.35/r2r/llms/litellm/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/llms/llama_cpp/base.py` & `r2r-0.1.35/r2r/llms/llama_cpp/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/llms/openai/base.py` & `r2r-0.1.35/r2r/llms/openai/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/main/app.py` & `r2r-0.1.35/r2r/main/app.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/main/factory.py` & `r2r-0.1.35/r2r/main/factory.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/main/models.py` & `r2r-0.1.35/r2r/main/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime
 from typing import Optional
 
 from pydantic import BaseModel, Field
 
-from r2r.core import BasicDocument
+from r2r.core import DocumentPage
 
 
 class EmbeddingsSettingsModel(BaseModel):
     do_chunking: Optional[bool] = True
     do_upsert: Optional[bool] = True
 
 
@@ -107,13 +107,13 @@
     pipeline_run_type: str = Field(alias="pipelineRunType")
     method: str = Field(alias="method")
     embedding_chunks: Optional[str] = Field(alias="embeddingChunks")
     search_query: str = Field(alias="searchQuery")
     search_results: list[dict] = Field(alias="searchResults")
     completion_result: str = Field(alias="completionResult")
     eval_results: Optional[dict] = Field(alias="evalResults")
-    document: Optional[BasicDocument] = Field(alias="document")
+    document: Optional[DocumentPage] = Field(alias="document")
     outcome: str = Field(alias="outcome")
 
     class Config:
         alias_generator = to_camel
         populate_by_name = True
```

### Comparing `r2r-0.1.34/r2r/main/utils.py` & `r2r-0.1.35/r2r/main/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import re
 from logging.handlers import RotatingFileHandler
 from typing import Any, Union
 
 from fastapi.middleware.cors import CORSMiddleware
 
-from r2r.core import BasicDocument
+from r2r.core import DocumentPage
 
 logger = logging.getLogger(__name__)
 
 
 # Function to find the project root by looking for a .git folder or setup.py file
 def find_project_root(current_dir):
     for parent in current_dir.parents:
@@ -180,26 +180,28 @@
     if method == "ingress":
         try:
             processed_result["search_query"] = result
         except Exception as e:
             logger.error(f"Error {e} processing 'ingress' event: {event}")
     elif method == "ingress" and pipeline_type == "embedding":
         try:
-            id_match = re.search(r"'id': '([^']+)'", result)
+            id_match = re.search(r"'document_id': '([^']+)'", result)
+            page_number = re.search(r"'page_number': '([^']+)'", result)
             text_match = re.search(r"'text': '([^']+)'", result)
             metadata_match = re.search(r"'metadata': (\{[^}]+\})", result)
             if not id_match or not text_match or not metadata_match:
                 raise ValueError(
                     f"Missing 'id', 'text', or 'metadata' in result: {result}"
                 )
             metadata = metadata_match.group(1).replace("'", '"')
             metadata_json = json.loads(metadata)
 
-            processed_result["document"] = BasicDocument(
-                id=id_match.group(1),
+            processed_result["document"] = DocumentPage(
+                document_id=id_match.group(1),
+                page_number=int(page_number.group(1)),
                 text=text_match.group(1),
                 metadata=metadata_json,
             )
         except Exception as e:
             logger.error(f"Error {e} processing 'ingress' event: {event}")
     elif method == "search":
         try:
```

### Comparing `r2r-0.1.34/r2r/pipelines/basic/embedding.py` & `r2r-0.1.35/r2r/pipelines/basic/embedding.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 import copy
 import logging
 from typing import Any, Optional, Tuple
 
 from r2r.core import (
-    BasicDocument,
+    DocumentPage,
     EmbeddingPipeline,
     LoggingDatabaseConnection,
     VectorDBProvider,
     VectorEntry,
     log_execution_to_db,
 )
 from r2r.core.utils import TextSplitter, generate_id_from_label
@@ -50,26 +50,27 @@
         )
         self.text_splitter = text_splitter
         self.embedding_batch_size = embedding_batch_size
         self.id_prefix = id_prefix
         self.pipeline_run_info = None
 
     @log_execution_to_db
-    def ingress(self, document: BasicDocument) -> dict:
+    def ingress(self, document: DocumentPage) -> dict:
         """
         Extracts text from a document.
         """
         return {
-            "id": str(document.id),
+            "document_id": str(document.document_id),
+            "page_number": str(document.page_number),
             "metadata": document.metadata,
             "text": document.text,
         }
 
     def initialize_pipeline(
-        self, document: BasicDocument, *args, **kwargs
+        self, document: DocumentPage, *args, **kwargs
     ) -> None:
         super().initialize_pipeline(*args, **kwargs)
         self.ingress(document)
 
     def transform_text(self, text: str) -> str:
         """
         Transforms text before chunking, if necessary.
@@ -118,45 +119,47 @@
         if do_upsert:
             self.db.upsert_entries(chunks)
         else:
             self.db.copy_entries(chunks)
 
     def run(
         self,
-        document: BasicDocument,
+        document: DocumentPage,
         do_chunking=False,
         do_upsert=True,
         **kwargs: Any,
     ):
         """
         Executes the embedding pipeline: chunking, transforming, embedding, and storing documents.
         """
         self.initialize_pipeline(document=document)
 
         logger.debug(
             f"Running the `BasicEmbeddingPipeline` with pipeline_run_info={self.pipeline_run_info}."
         )
 
-        documents = [document] if not isinstance(document, list) else document
         batch_data = []
 
-        for document in documents:
-            chunks = (
-                self.chunk_text(document.text)
-                if do_chunking
-                else [document.text]
-            )
-            for chunk in chunks:
-                batch_data.append(
-                    (document.id, chunk, copy.copy(document.metadata))
+        chunks = (
+            self.chunk_text(document.text) if do_chunking else [document.text]
+        )
+        for chunk_iter, chunk in enumerate(chunks):
+            batch_data.append(
+                (
+                    document.document_id,
+                    document.page_number,
+                    chunk_iter,
+                    chunk,
+                    copy.copy(document.metadata),
                 )
+            )
 
-                if len(batch_data) == self.embedding_batch_size:
-                    self._process_batches(batch_data, do_upsert)
-                    batch_data = []
+            if len(batch_data) == self.embedding_batch_size:
+                self._process_batches(batch_data, do_upsert)
+                batch_data = []
 
         # Process any remaining batch
         if batch_data:
             self._process_batches(batch_data, do_upsert)
 
     def _process_batches(
         self, batch_data: list[Tuple[str, str, dict]], do_upsert: bool
@@ -165,23 +168,38 @@
         Processes batches of documents: transforms, embeds, and stores chunks.
         """
         logger.debug(f"Parsing batch of size {len(batch_data)}.")
 
         entries = []
 
         # Unpack document IDs, indices, and chunks for transformation and embedding
-        ids, raw_chunks, metadatas = zip(*batch_data)
+        document_ids, page_numbers, chunk_nums, raw_chunks, metadatas = zip(
+            *batch_data
+        )
         transformed_chunks = self.transform_chunks(raw_chunks, metadatas)
         embedded_chunks = self.embed_chunks(transformed_chunks)
 
-        chunk_count = 0
-        for doc_id, transformed_chunk, embedded_chunk, metadata in zip(
-            ids, transformed_chunks, embedded_chunks, metadatas
+        for (
+            document_id,
+            page_number,
+            chunk_num,
+            transformed_chunk,
+            embedded_chunk,
+            metadata,
+        ) in zip(
+            document_ids,
+            page_numbers,
+            chunk_nums,
+            transformed_chunks,
+            embedded_chunks,
+            metadatas,
         ):
             metadata = copy.deepcopy(metadata)
             metadata["pipeline_run_id"] = str(self.pipeline_run_info["run_id"])  # type: ignore
             metadata["text"] = transformed_chunk
-            metadata["document_id"] = doc_id
-            chunk_id = generate_id_from_label(f"{doc_id}-{chunk_count}")
-            chunk_count += 1
+            metadata["document_id"] = document_id
+            metadata["page_number"] = page_number
+            chunk_id = generate_id_from_label(
+                f"{document_id}-{page_number}-{chunk_num}"
+            )
             entries.append(VectorEntry(chunk_id, embedded_chunk, metadata))
         self.store_chunks(entries, do_upsert)
```

### Comparing `r2r-0.1.34/r2r/pipelines/basic/eval.py` & `r2r-0.1.35/r2r/pipelines/basic/eval.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/pipelines/basic/ingestion.py` & `r2r-0.1.35/r2r/pipelines/basic/ingestion.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,19 +2,15 @@
 A simple example to demonstrate the usage of `BasicIngestionPipeline`.
 """
 
 import logging
 from enum import Enum
 from typing import Any, Iterator, Optional, Union
 
-from r2r.core import (
-    BasicDocument,
-    IngestionPipeline,
-    LoggingDatabaseConnection,
-)
+from r2r.core import DocumentPage, IngestionPipeline, LoggingDatabaseConnection
 from r2r.core.adapters import (
     Adapter,
     HTMLAdapter,
     JSONAdapter,
     PDFAdapter,
     TextAdapter,
 )
@@ -66,36 +62,39 @@
         """
         return [entry_type.value for entry_type in IngestionType]
 
     def process_data(
         self,
         entry_type: IngestionType,
         entry_data: Union[bytes, str],
-    ) -> Iterator[BasicDocument]:
+    ) -> Iterator[DocumentPage]:
         adapter = self.adapters.get(
             entry_type, self.default_adapters[entry_type]
         )
         texts = adapter.adapt(entry_data)
-        for text in texts:
-            yield BasicDocument(
-                id=self.document_id, text=text, metadata=self.metadata
+        for iteration, text in enumerate(texts):
+            yield DocumentPage(
+                document_id=self.document_id,
+                page_number=iteration,
+                text=text,
+                metadata=self.metadata,
             )
 
     def parse_entry(
         self, entry_type: str, entry_data: Union[bytes, str]
-    ) -> Iterator[BasicDocument]:
+    ) -> Iterator[DocumentPage]:
         yield from self.process_data(IngestionType(entry_type), entry_data)
 
     def run(
         self,
         document_id: str,
         blobs: dict[str, Any],
         metadata: Optional[dict] = None,
         **kwargs,
-    ) -> Iterator[BasicDocument]:
+    ) -> Iterator[DocumentPage]:
         self.initialize_pipeline()
         self.document_id = document_id
         self.metadata = metadata or {}
 
         if len(blobs) == 0:
             raise ValueError("No blobs provided to process.")
```

### Comparing `r2r-0.1.34/r2r/pipelines/basic/prompt_provider.py` & `r2r-0.1.35/r2r/pipelines/basic/prompt_provider.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/pipelines/basic/rag.py` & `r2r-0.1.35/r2r/pipelines/basic/rag.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,14 +78,15 @@
             query_vector=self.embeddings_provider.get_embedding(
                 transformed_query,
                 self.embedding_model,
             ),
             filters=filters,
             limit=limit,
         )
+
         logger.debug(f"Retrieved the raw results shown:\n{results}\n")
 
         return results
 
     def rerank_results(
         self, results: list[VectorSearchResult]
     ) -> list[VectorSearchResult]:
```

### Comparing `r2r-0.1.34/r2r/tests/end_to_end.py` & `r2r-0.1.35/r2r/tests/end_to_end.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/tests/test.pdf` & `r2r-0.1.35/r2r/tests/test.pdf`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/vecs/__init__.py` & `r2r-0.1.35/r2r/vecs/__init__.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/vecs/adapter/base.py` & `r2r-0.1.35/r2r/vecs/adapter/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/vecs/adapter/markdown.py` & `r2r-0.1.35/r2r/vecs/adapter/markdown.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/vecs/adapter/noop.py` & `r2r-0.1.35/r2r/vecs/adapter/noop.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/vecs/adapter/text.py` & `r2r-0.1.35/r2r/vecs/adapter/text.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/vecs/client.py` & `r2r-0.1.35/r2r/vecs/client.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/vecs/collection.py` & `r2r-0.1.35/r2r/vecs/collection.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/vecs/exc.py` & `r2r-0.1.35/r2r/vecs/exc.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/vector_dbs/local/base.py` & `r2r-0.1.35/r2r/vector_dbs/local/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,17 @@
                 "LocalVectorDB must be initialized with provider `local`."
             )
 
         self.db_path = db_path
         self.collection_name: Optional[str] = None
 
     def _get_conn(self):
-        conn = sqlite3.connect(self.db_path or os.getenv("LOCAL_DB_PATH"))
+        conn = sqlite3.connect(
+            self.db_path or os.getenv("LOCAL_DB_PATH", "local.sqlite")
+        )
         return conn
 
     def _get_cursor(self, conn):
         return conn.cursor()
 
     def initialize_collection(
         self, collection_name: str, dimension: int
```

### Comparing `r2r-0.1.34/r2r/vector_dbs/pg_vector/base.py` & `r2r-0.1.35/r2r/vector_dbs/pg_vector/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/r2r/vector_dbs/qdrant/base.py` & `r2r-0.1.35/r2r/vector_dbs/qdrant/base.py`

 * *Files identical despite different names*

### Comparing `r2r-0.1.34/PKG-INFO` & `r2r-0.1.35/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r2r
-Version: 0.1.34
+Version: 0.1.35
 Summary: SciPhi R2R
 License: MIT
 Author: Owen Colegrove
 Author-email: owen@sciphi.ai
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -29,15 +29,15 @@
 Requires-Dist: bs4 (>=0.0.2,<0.0.3)
 Requires-Dist: datasets (>=2.16.1,<3.0.0) ; extra == "streaming" or extra == "all"
 Requires-Dist: deepeval (>=0.20.88,<0.21.0) ; extra == "deepeval"
 Requires-Dist: exa-py (>=1.0.9,<2.0.0) ; extra == "exa" or extra == "all"
 Requires-Dist: fastapi (>=0.109.2,<0.110.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: gunicorn (>=21.2.0,<22.0.0)
-Requires-Dist: ionic-api-sdk (==0.9.3) ; extra == "ionic"
+Requires-Dist: ionic-api-sdk (==0.9.3) ; extra == "ionic" or extra == "all"
 Requires-Dist: litellm (>=1.34.0,<2.0.0)
 Requires-Dist: llama-cpp-python (>=0.2.57,<0.3.0) ; extra == "local-llm" or extra == "all"
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: openai (>=1.11.1,<2.0.0)
 Requires-Dist: parea-ai (>=0.2.86,<0.3.0) ; extra == "eval" or extra == "all"
 Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0) ; extra == "postgres" or extra == "all"
 Requires-Dist: pydantic (>=2.6.3,<3.0.0)
@@ -96,24 +96,26 @@
 
 [Join the Discord server](https://discord.gg/p6KqD2kjtB)
 
 [R2R Docs Quickstart](https://r2r-docs.sciphi.ai/getting-started/quick-install)
 
 [SciPhi Cloud](https://docs.sciphi.ai/)
 
+[Local RAG Tutorial](https://r2r-docs.sciphi.ai/tutorials/local_rag)
+
 ## Quick Install:
 
 ```bash
 # use the `'r2r[all]'` to download all required deps
 pip install 'r2r[eval]'
 
 # setup env 
 export OPENAI_API_KEY=sk-...
 # Set `LOCAL_DB_PATH` for local testing
-export LOCAL_DB_PATH=local.sqlite
+export LOCAL_DB_PATH=local.sqlite # robust providers available (e.g. qdrant, pgvector, ..)
 
 # OR do `vim .env.example && cp .env.example .env`
 # INCLUDE secrets and modify config.json
 # if using cloud providers (e.g. pgvector, qdrant, ...)
 ```
 
 ## Docker:
@@ -121,23 +123,23 @@
 ```bash
 docker pull emrgntcmplxty/r2r:latest
 
 # Choose from CONFIG_OPTION in {`default`, `local_ollama`}
 # For cloud deployment, select `default` and pass `--env-file .env`
 # For local deployment, select `local_ollama`
 docker run -d --name r2r_container -p 8000:8000 -e CONFIG_OPTION=local_ollama  emrgntcmplxty/r2r:latest
-
 ```
 
 ## Basic Example
 
 [`basic_pipeline.py`](r2r/examples/servers/basic_pipeline.py): Execute this script to initiate the default **backend server**. It establishes a basic RAG pipeline that encompasses ingestion, embedding, and RAG processes, all accessible via FastAPI.
 
    ```bash
    # launch the server
+   # Do `export CONFIG_OPTION=local_ollama` to run the pipeline with local ollama instead of OpenAI
    python -m r2r.examples.servers.basic_pipeline
    ```
 
 [`run_basic_client.py`](r2r/examples/clients/run_basic_client.py): This **client script** should be executed subsequent to the server startup above. It facilitates the upload of text entries and PDFs to the server using the Python client and demonstrates the management of document and user-level vectors through its built-in features.
 
    ```bash
    # run the client
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: r2r Version: 0.1.34 Summary: SciPhi R2R License:
+Metadata-Version: 2.1 Name: r2r Version: 0.1.35 Summary: SciPhi R2R License:
 MIT Author: Owen Colegrove Author-email: owen@sciphi.ai Requires-Python:
 >=3.9,<3.13 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Provides-Extra: all Provides-Extra: deepeval Provides-Extra:
 embedding Provides-Extra: eval Provides-Extra: exa Provides-Extra: ionic
@@ -11,20 +11,20 @@
 transformers Provides-Extra: streaming Requires-Dist: boto3 (>=1.34.71,<2.0.0)
 ; extra == "reducto" or extra == "all" Requires-Dist: bs4 (>=0.0.2,<0.0.3)
 Requires-Dist: datasets (>=2.16.1,<3.0.0) ; extra == "streaming" or extra ==
 "all" Requires-Dist: deepeval (>=0.20.88,<0.21.0) ; extra == "deepeval"
 Requires-Dist: exa-py (>=1.0.9,<2.0.0) ; extra == "exa" or extra == "all"
 Requires-Dist: fastapi (>=0.109.2,<0.110.0) Requires-Dist: fire
 (>=0.5.0,<0.6.0) Requires-Dist: gunicorn (>=21.2.0,<22.0.0) Requires-Dist:
-ionic-api-sdk (==0.9.3) ; extra == "ionic" Requires-Dist: litellm
-(>=1.34.0,<2.0.0) Requires-Dist: llama-cpp-python (>=0.2.57,<0.3.0) ; extra ==
-"local-llm" or extra == "all" Requires-Dist: numpy (>=1.26.4,<2.0.0) Requires-
-Dist: openai (>=1.11.1,<2.0.0) Requires-Dist: parea-ai (>=0.2.86,<0.3.0) ;
-extra == "eval" or extra == "all" Requires-Dist: psycopg2-binary
-(>=2.9.9,<3.0.0) ; extra == "postgres" or extra == "all" Requires-Dist:
+ionic-api-sdk (==0.9.3) ; extra == "ionic" or extra == "all" Requires-Dist:
+litellm (>=1.34.0,<2.0.0) Requires-Dist: llama-cpp-python (>=0.2.57,<0.3.0) ;
+extra == "local-llm" or extra == "all" Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: openai (>=1.11.1,<2.0.0) Requires-Dist: parea-ai
+(>=0.2.86,<0.3.0) ; extra == "eval" or extra == "all" Requires-Dist: psycopg2-
+binary (>=2.9.9,<3.0.0) ; extra == "postgres" or extra == "all" Requires-Dist:
 pydantic (>=2.6.3,<3.0.0) Requires-Dist: pypdf (>=4.2.0,<5.0.0) Requires-Dist:
 python-dotenv (>=1.0.1,<2.0.0) Requires-Dist: python-multipart
 (>=0.0.9,<0.0.10) Requires-Dist: qdrant_client (>=1.7.0,<2.0.0) ; extra ==
 "qdrant" or extra == "all" Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-
 Dist: sentence-transformers (>=2.6.1,<3.0.0) ; extra == "sentence-transformers"
 or extra == "local-llm" Requires-Dist: sentry-sdk (>=1.40.4,<2.0.0) ; extra ==
 "monitoring" or extra == "all" Requires-Dist: tiktoken (>=0.5.2,<0.6.0) ; extra
@@ -51,43 +51,47 @@
 deployment. ## Demo(s) Using the cloud application to deploy the pre-built
 basic pipeline: https://www.loom.com/share/e3b934b554484787b005702ced650ac9
 Note - the example above uses [SciPhi Cloud](https://app.sciphi.ai) to pair
 with the R2R framework for deployment and observability. SciPhi is working to
 launch a self-hosted version of their cloud platform as R2R matures. ## Links
 [Join the Discord server](https://discord.gg/p6KqD2kjtB) [R2R Docs Quickstart]
 (https://r2r-docs.sciphi.ai/getting-started/quick-install) [SciPhi Cloud]
-(https://docs.sciphi.ai/) ## Quick Install: ```bash # use the `'r2r[all]'` to
+(https://docs.sciphi.ai/) [Local RAG Tutorial](https://r2r-docs.sciphi.ai/
+tutorials/local_rag) ## Quick Install: ```bash # use the `'r2r[all]'` to
 download all required deps pip install 'r2r[eval]' # setup env export
 OPENAI_API_KEY=sk-... # Set `LOCAL_DB_PATH` for local testing export
-LOCAL_DB_PATH=local.sqlite # OR do `vim .env.example && cp .env.example .env` #
-INCLUDE secrets and modify config.json # if using cloud providers (e.g.
-pgvector, qdrant, ...) ``` ## Docker: ```bash docker pull emrgntcmplxty/r2r:
-latest # Choose from CONFIG_OPTION in {`default`, `local_ollama`} # For cloud
-deployment, select `default` and pass `--env-file .env` # For local deployment,
-select `local_ollama` docker run -d --name r2r_container -p 8000:8000 -
+LOCAL_DB_PATH=local.sqlite # robust providers available (e.g. qdrant, pgvector,
+..) # OR do `vim .env.example && cp .env.example .env` # INCLUDE secrets and
+modify config.json # if using cloud providers (e.g. pgvector, qdrant, ...) ```
+## Docker: ```bash docker pull emrgntcmplxty/r2r:latest # Choose from
+CONFIG_OPTION in {`default`, `local_ollama`} # For cloud deployment, select
+`default` and pass `--env-file .env` # For local deployment, select
+`local_ollama` docker run -d --name r2r_container -p 8000:8000 -
 e CONFIG_OPTION=local_ollama emrgntcmplxty/r2r:latest ``` ## Basic Example
 [`basic_pipeline.py`](r2r/examples/servers/basic_pipeline.py): Execute this
 script to initiate the default **backend server**. It establishes a basic RAG
 pipeline that encompasses ingestion, embedding, and RAG processes, all
-accessible via FastAPI. ```bash # launch the server python -
-m r2r.examples.servers.basic_pipeline ``` [`run_basic_client.py`](r2r/examples/
-clients/run_basic_client.py): This **client script** should be executed
-subsequent to the server startup above. It facilitates the upload of text
-entries and PDFs to the server using the Python client and demonstrates the
-management of document and user-level vectors through its built-in features.
-```bash # run the client python -m r2r.examples.clients.run_basic_client ingest
-python -m r2r.examples.clients.run_basic_client search --query="What is the
-meaning of life?" ``` ### Running Basic Local RAG [Refer here](https://r2r-
-docs.sciphi.ai/tutorials/local_rag) for a tutorial on how to modify the
-commands above to use local providers. ## Synthetic Queries Example
-[`synthetic_query_pipeline.py`](r2r/examples/servers/
-synthetic_query_pipeline.py): Execute this script to start a backend server
-equipped with an advanced pipeline. This pipeline is designed to create
-synthetic queries, enhancing the RAG system's learning and performance. ```bash
-# launch the server python -m r2r.examples.servers.synthetic_query_pipeline ```
+accessible via FastAPI. ```bash # launch the server # Do `export
+CONFIG_OPTION=local_ollama` to run the pipeline with local ollama instead of
+OpenAI python -m r2r.examples.servers.basic_pipeline ```
+[`run_basic_client.py`](r2r/examples/clients/run_basic_client.py): This
+**client script** should be executed subsequent to the server startup above. It
+facilitates the upload of text entries and PDFs to the server using the Python
+client and demonstrates the management of document and user-level vectors
+through its built-in features. ```bash # run the client python -
+m r2r.examples.clients.run_basic_client ingest python -
+m r2r.examples.clients.run_basic_client search --query="What is the meaning of
+life?" ``` ### Running Basic Local RAG [Refer here](https://r2r-docs.sciphi.ai/
+tutorials/local_rag) for a tutorial on how to modify the commands above to use
+local providers. ## Synthetic Queries Example [`synthetic_query_pipeline.py`]
+(r2r/examples/servers/synthetic_query_pipeline.py): Execute this script to
+start a backend server equipped with an advanced pipeline. This pipeline is
+designed to create synthetic queries, enhancing the RAG system's learning and
+performance. ```bash # launch the server python -
+m r2r.examples.servers.synthetic_query_pipeline ```
 [`run_synthetic_query_client.py`](r2r/examples/clients/
 run_synthetic_query_client.py): Use this client script after the synthetic
 query pipeline is running. It's tailored for use with the synthetic query
 pipeline, demonstrating the improved features of the RAG system. ```bash # run
 the client python -m r2r.examples.clients.run_synthetic_query_client ``` ##
 Extra Examples [`reducto_pipeline.py`](r2r/examples/servers/
 reducto_pipeline.py): Launch this script to activate a backend server that
```

