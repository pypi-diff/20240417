# Comparing `tmp/dbally-0.0.1.dev0.tar.gz` & `tmp/dbally-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbally-0.0.1.dev0.tar", last modified: Wed Mar 20 12:00:11 2024, max compression
+gzip compressed data, was "dbally-0.0.2.tar", last modified: Wed Apr 17 13:10:20 2024, max compression
```

## Comparing `dbally-0.0.1.dev0.tar` & `dbally-0.0.2.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.682801 dbally-0.0.1.dev0/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1078 2024-03-20 11:52:45.000000 dbally-0.0.1.dev0/LICENSE
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       97 2024-02-02 13:52:13.000000 dbally-0.0.1.dev0/MANIFEST.in
--rw-r--r--   0 mateusz   (1001) mateusz   (1001)     1413 2024-03-20 12:00:11.678801 dbally-0.0.1.dev0/PKG-INFO
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     4022 2024-03-20 11:48:39.000000 dbally-0.0.1.dev0/README.md
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2969 2024-03-06 13:57:39.000000 dbally-0.0.1.dev0/pyproject.toml
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1358 2024-03-20 12:00:11.682801 dbally-0.0.1.dev0/setup.cfg
--rwxrwxr-x   0 mateusz   (1001) mateusz   (1001)      150 2024-02-02 13:52:13.000000 dbally-0.0.1.dev0/setup.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.614801 dbally-0.0.1.dev0/src/
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.618801 dbally-0.0.1.dev0/src/dbally/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        9 2024-03-19 08:38:07.000000 dbally-0.0.1.dev0/src/dbally/VERSION
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      372 2024-02-28 12:45:09.000000 dbally-0.0.1.dev0/src/dbally/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      180 2024-02-02 13:52:13.000000 dbally-0.0.1.dev0/src/dbally/__version__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     6149 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/_collection.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2302 2024-02-29 12:56:28.000000 dbally-0.0.1.dev0/src/dbally/_main.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.626801 dbally-0.0.1.dev0/src/dbally/audit/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      347 2024-03-14 12:16:46.000000 dbally-0.0.1.dev0/src/dbally/audit/__init__.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.630801 dbally-0.0.1.dev0/src/dbally/audit/event_handlers/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       59 2024-03-19 15:18:26.000000 dbally-0.0.1.dev0/src/dbally/audit/event_handlers/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1613 2024-02-27 12:41:08.000000 dbally-0.0.1.dev0/src/dbally/audit/event_handlers/base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3243 2024-02-28 12:45:09.000000 dbally-0.0.1.dev0/src/dbally/audit/event_handlers/cli_event_handler.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2734 2024-02-27 13:41:27.000000 dbally-0.0.1.dev0/src/dbally/audit/event_handlers/langsmith_event_handler.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      409 2024-02-27 12:41:08.000000 dbally-0.0.1.dev0/src/dbally/audit/event_span.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2670 2024-02-27 12:41:08.000000 dbally-0.0.1.dev0/src/dbally/audit/event_tracker.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.634801 dbally-0.0.1.dev0/src/dbally/data_models/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-02-02 13:52:13.000000 dbally-0.0.1.dev0/src/dbally/data_models/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      820 2024-02-27 13:41:27.000000 dbally-0.0.1.dev0/src/dbally/data_models/audit.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      330 2024-02-29 12:56:28.000000 dbally-0.0.1.dev0/src/dbally/data_models/execution_result.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      573 2024-02-05 10:47:54.000000 dbally-0.0.1.dev0/src/dbally/data_models/llm_options.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.642801 dbally-0.0.1.dev0/src/dbally/data_models/prompts/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      522 2024-02-27 12:41:08.000000 dbally-0.0.1.dev0/src/dbally/data_models/prompts/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1379 2024-02-27 12:41:08.000000 dbally-0.0.1.dev0/src/dbally/data_models/prompts/common_validation_utils.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1948 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/data_models/prompts/iql_explainer_prompt_template.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2192 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/data_models/prompts/iql_prompt_template.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1686 2024-02-29 12:56:28.000000 dbally-0.0.1.dev0/src/dbally/data_models/prompts/nl_responder_prompt_template.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2638 2024-03-01 15:02:22.000000 dbally-0.0.1.dev0/src/dbally/data_models/prompts/prompt_template.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1777 2024-02-27 12:41:08.000000 dbally-0.0.1.dev0/src/dbally/data_models/prompts/view_selector_prompt_template.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.642801 dbally-0.0.1.dev0/src/dbally/embedding_client/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-03-13 10:43:31.000000 dbally-0.0.1.dev0/src/dbally/embedding_client/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      545 2024-03-13 10:43:31.000000 dbally-0.0.1.dev0/src/dbally/embedding_client/base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1661 2024-03-13 10:43:31.000000 dbally-0.0.1.dev0/src/dbally/embedding_client/openai.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.646801 dbally-0.0.1.dev0/src/dbally/examples/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/examples/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3147 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/examples/db.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3994 2024-03-19 15:18:26.000000 dbally-0.0.1.dev0/src/dbally/examples/recruiting.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2155 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/examples/views.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.650801 dbally-0.0.1.dev0/src/dbally/iql/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      238 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/iql/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1510 2024-02-29 12:56:28.000000 dbally-0.0.1.dev0/src/dbally/iql/_exceptions.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     5064 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/iql/_processor.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      834 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/iql/_query.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2573 2024-03-12 07:48:26.000000 dbally-0.0.1.dev0/src/dbally/iql/_type_validators.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2396 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/iql/syntax.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.654801 dbally-0.0.1.dev0/src/dbally/iql_generator/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-02-27 12:41:08.000000 dbally-0.0.1.dev0/src/dbally/iql_generator/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3716 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/iql_generator/iql_generator.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.654801 dbally-0.0.1.dev0/src/dbally/llm_client/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-02-05 10:36:27.000000 dbally-0.0.1.dev0/src/dbally/llm_client/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2512 2024-03-12 08:02:42.000000 dbally-0.0.1.dev0/src/dbally/llm_client/base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1935 2024-03-12 08:02:42.000000 dbally-0.0.1.dev0/src/dbally/llm_client/openai_client.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.658801 dbally-0.0.1.dev0/src/dbally/nl_responder/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-03-19 15:18:26.000000 dbally-0.0.1.dev0/src/dbally/nl_responder/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3921 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/nl_responder/nl_responder.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2057 2024-03-12 08:02:42.000000 dbally-0.0.1.dev0/src/dbally/nl_responder/token_counters.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.658801 dbally-0.0.1.dev0/src/dbally/prompts/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       71 2024-02-02 13:52:13.000000 dbally-0.0.1.dev0/src/dbally/prompts/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2193 2024-02-05 10:36:27.000000 dbally-0.0.1.dev0/src/dbally/prompts/prompt_builder.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-02-02 13:52:13.000000 dbally-0.0.1.dev0/src/dbally/py.typed
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.666801 dbally-0.0.1.dev0/src/dbally/similarity/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      391 2024-03-14 12:16:46.000000 dbally-0.0.1.dev0/src/dbally/similarity/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3381 2024-03-14 12:16:46.000000 dbally-0.0.1.dev0/src/dbally/similarity/faiss_store.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      382 2024-03-06 13:57:39.000000 dbally-0.0.1.dev0/src/dbally/similarity/fetcher.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1986 2024-03-12 07:48:26.000000 dbally-0.0.1.dev0/src/dbally/similarity/index.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3594 2024-03-06 13:57:39.000000 dbally-0.0.1.dev0/src/dbally/similarity/sqlalchemy_base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      780 2024-03-06 13:57:39.000000 dbally-0.0.1.dev0/src/dbally/similarity/store.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.666801 dbally-0.0.1.dev0/src/dbally/utils/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-03-19 15:18:26.000000 dbally-0.0.1.dev0/src/dbally/utils/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      249 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/utils/errors.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.670801 dbally-0.0.1.dev0/src/dbally/view_selection/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-02-02 13:52:13.000000 dbally-0.0.1.dev0/src/dbally/view_selection/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      673 2024-02-27 12:41:08.000000 dbally-0.0.1.dev0/src/dbally/view_selection/base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2398 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/view_selection/llm_view_selector.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      865 2024-02-27 12:41:08.000000 dbally-0.0.1.dev0/src/dbally/view_selection/random_view_selector.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.674801 dbally-0.0.1.dev0/src/dbally/views/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-03-19 15:18:26.000000 dbally-0.0.1.dev0/src/dbally/views/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2253 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/views/base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      406 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/views/decorators.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1695 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/views/methods_base.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     4767 2024-03-14 08:59:44.000000 dbally-0.0.1.dev0/src/dbally/views/sqlalchemy_base.py
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.678801 dbally-0.0.1.dev0/src/dbally.egg-info/
--rw-r--r--   0 mateusz   (1001) mateusz   (1001)     1413 2024-03-20 12:00:11.000000 dbally-0.0.1.dev0/src/dbally.egg-info/PKG-INFO
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2747 2024-03-20 12:00:11.000000 dbally-0.0.1.dev0/src/dbally.egg-info/SOURCES.txt
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        1 2024-03-20 12:00:11.000000 dbally-0.0.1.dev0/src/dbally.egg-info/dependency_links.txt
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       47 2024-03-20 12:00:11.000000 dbally-0.0.1.dev0/src/dbally.egg-info/entry_points.txt
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        1 2024-01-26 12:33:13.000000 dbally-0.0.1.dev0/src/dbally.egg-info/not-zip-safe
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      261 2024-03-20 12:00:11.000000 dbally-0.0.1.dev0/src/dbally.egg-info/requires.txt
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       18 2024-03-20 12:00:11.000000 dbally-0.0.1.dev0/src/dbally.egg-info/top_level.txt
-drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-03-20 12:00:11.678801 dbally-0.0.1.dev0/src/dbally_cli/
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-03-06 13:57:39.000000 dbally-0.0.1.dev0/src/dbally_cli/__init__.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      112 2024-03-06 13:57:39.000000 dbally-0.0.1.dev0/src/dbally_cli/example1.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      294 2024-03-06 13:57:39.000000 dbally-0.0.1.dev0/src/dbally_cli/example2.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      235 2024-03-06 13:57:39.000000 dbally-0.0.1.dev0/src/dbally_cli/main.py
--rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-02-02 13:52:13.000000 dbally-0.0.1.dev0/src/py.typed
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.619255 dbally-0.0.2/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1089 2024-04-17 13:06:55.000000 dbally-0.0.2/LICENSE
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       97 2024-04-03 11:01:33.000000 dbally-0.0.2/MANIFEST.in
+-rw-r--r--   0 mateusz   (1001) mateusz   (1001)     2140 2024-04-17 13:10:20.619255 dbally-0.0.2/PKG-INFO
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     6104 2024-04-17 13:06:58.000000 dbally-0.0.2/README.md
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2969 2024-04-03 11:01:33.000000 dbally-0.0.2/pyproject.toml
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1655 2024-04-17 13:10:20.623255 dbally-0.0.2/setup.cfg
+-rwxrwxr-x   0 mateusz   (1001) mateusz   (1001)      150 2024-04-03 11:01:33.000000 dbally-0.0.2/setup.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.515254 dbally-0.0.2/src/
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.519254 dbally-0.0.2/src/dbally/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        5 2024-04-17 13:07:28.000000 dbally-0.0.2/src/dbally/VERSION
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      658 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      180 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/__version__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3106 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/_main.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.531254 dbally-0.0.2/src/dbally/assistants/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/assistants/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     4192 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/assistants/base.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     6238 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/assistants/openai.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.535254 dbally-0.0.2/src/dbally/audit/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      347 2024-04-10 06:42:50.000000 dbally-0.0.2/src/dbally/audit/__init__.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.539255 dbally-0.0.2/src/dbally/audit/event_handlers/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       59 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/audit/event_handlers/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2060 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/audit/event_handlers/base.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3988 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/audit/event_handlers/cli_event_handler.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2938 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/audit/event_handlers/langsmith_event_handler.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      409 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/audit/event_span.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2670 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/audit/event_tracker.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)    12040 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/collection.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.543254 dbally-0.0.2/src/dbally/data_models/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/data_models/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      838 2024-04-10 07:45:19.000000 dbally-0.0.2/src/dbally/data_models/audit.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1817 2024-04-10 07:45:19.000000 dbally-0.0.2/src/dbally/data_models/execution_result.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      610 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/data_models/llm_options.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.555255 dbally-0.0.2/src/dbally/data_models/prompts/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      522 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/data_models/prompts/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1379 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/data_models/prompts/common_validation_utils.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1948 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/data_models/prompts/iql_explainer_prompt_template.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2192 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/data_models/prompts/iql_prompt_template.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1686 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/data_models/prompts/nl_responder_prompt_template.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2638 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/data_models/prompts/prompt_template.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1777 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/data_models/prompts/view_selector_prompt_template.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.563254 dbally-0.0.2/src/dbally/embedding_client/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      132 2024-04-10 06:42:50.000000 dbally-0.0.2/src/dbally/embedding_client/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      545 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/embedding_client/base.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1661 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/embedding_client/openai.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.571255 dbally-0.0.2/src/dbally/iql/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      238 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/iql/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1510 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/iql/_exceptions.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     4839 2024-04-17 13:06:55.000000 dbally-0.0.2/src/dbally/iql/_processor.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      834 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/iql/_query.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2573 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/iql/_type_validators.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2440 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/iql/syntax.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.571255 dbally-0.0.2/src/dbally/iql_generator/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/iql_generator/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     4243 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/iql_generator/iql_generator.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.575255 dbally-0.0.2/src/dbally/llm_client/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/llm_client/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3020 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/llm_client/base.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2393 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/llm_client/openai_client.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.579255 dbally-0.0.2/src/dbally/nl_responder/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/nl_responder/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     4025 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/nl_responder/nl_responder.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2060 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/nl_responder/token_counters.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.583255 dbally-0.0.2/src/dbally/prompts/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       71 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/prompts/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2361 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/prompts/prompt_builder.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/py.typed
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.595255 dbally-0.0.2/src/dbally/similarity/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      503 2024-04-10 06:42:50.000000 dbally-0.0.2/src/dbally/similarity/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     7653 2024-04-17 13:06:55.000000 dbally-0.0.2/src/dbally/similarity/detector.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3388 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/similarity/faiss_store.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      432 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/similarity/fetcher.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2146 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/similarity/index.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3560 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/similarity/sqlalchemy_base.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1000 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/similarity/store.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.599255 dbally-0.0.2/src/dbally/utils/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/utils/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      249 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/utils/errors.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.603255 dbally-0.0.2/src/dbally/view_selection/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       99 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/view_selection/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      748 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/view_selection/base.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3012 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/view_selection/llm_view_selector.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      865 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/view_selection/random_view_selector.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.611255 dbally-0.0.2/src/dbally/views/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally/views/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2879 2024-04-17 13:06:55.000000 dbally-0.0.2/src/dbally/views/base.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      414 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/views/decorators.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3422 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/views/methods_base.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3296 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/views/pandas_base.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     3484 2024-04-17 13:06:58.000000 dbally-0.0.2/src/dbally/views/sqlalchemy_base.py
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.615255 dbally-0.0.2/src/dbally.egg-info/
+-rw-r--r--   0 mateusz   (1001) mateusz   (1001)     2140 2024-04-17 13:10:20.000000 dbally-0.0.2/src/dbally.egg-info/PKG-INFO
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     2762 2024-04-17 13:10:20.000000 dbally-0.0.2/src/dbally.egg-info/SOURCES.txt
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        1 2024-04-17 13:10:20.000000 dbally-0.0.2/src/dbally.egg-info/dependency_links.txt
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       47 2024-04-17 13:10:20.000000 dbally-0.0.2/src/dbally.egg-info/entry_points.txt
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        1 2024-01-26 12:33:13.000000 dbally-0.0.2/src/dbally.egg-info/not-zip-safe
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      496 2024-04-17 13:10:20.000000 dbally-0.0.2/src/dbally.egg-info/requires.txt
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)       18 2024-04-17 13:10:20.000000 dbally-0.0.2/src/dbally.egg-info/top_level.txt
+drwxrwxr-x   0 mateusz   (1001) mateusz   (1001)        0 2024-04-17 13:10:20.611255 dbally-0.0.2/src/dbally_cli/
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.2/src/dbally_cli/__init__.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)      178 2024-04-17 13:06:55.000000 dbally-0.0.2/src/dbally_cli/main.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)     1842 2024-04-17 13:06:55.000000 dbally-0.0.2/src/dbally_cli/similarity.py
+-rw-rw-r--   0 mateusz   (1001) mateusz   (1001)        0 2024-04-03 11:01:33.000000 dbally-0.0.2/src/py.typed
```

### Comparing `dbally-0.0.1.dev0/LICENSE` & `dbally-0.0.2/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2024 deepsense.ai
+Copyright (c) 2024 deepsense.ai sp. z o.o.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `dbally-0.0.1.dev0/PKG-INFO` & `dbally-0.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,50 @@
 Metadata-Version: 2.1
 Name: dbally
-Version: 0.0.1.dev0
+Version: 0.0.2
 Summary: "Efficient, consistent and secure library for querying structured data with natural language"
 Author: deepsense.ai
 Author-email: contact@deepsense.ai
 License: MIT
 Project-URL: Documentation, https://db-ally.deepsense.ai/
+Project-URL: Source, https://github.com/deepsense-ai/db-ally
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: pandas~=2.0.3
 Requires-Dist: python-dotenv>=0.5.1
 Requires-Dist: SQLAlchemy==2.0.25
 Requires-Dist: tabulate>=0.9.0
-Requires-Dist: transformers>=4.37.1
 Requires-Dist: click~=8.1.7
 Requires-Dist: numpy>=1.24.0
 Provides-Extra: openai
 Requires-Dist: openai>=1.10.0; extra == "openai"
 Requires-Dist: tiktoken>=0.6.0; extra == "openai"
 Provides-Extra: faiss
 Requires-Dist: faiss-cpu>=1.8.0; extra == "faiss"
 Provides-Extra: examples
 Requires-Dist: pydantic~=2.6.0; extra == "examples"
 Requires-Dist: pydantic_settings~=2.1.0; extra == "examples"
 Requires-Dist: psycopg2-binary~=2.9.9; extra == "examples"
+Provides-Extra: langsmith
+Requires-Dist: langsmith>=0.0.87; extra == "langsmith"
+Provides-Extra: transformers
+Requires-Dist: transformers>=4.37.1; extra == "transformers"
+Provides-Extra: benchmark
+Requires-Dist: asyncpg~=0.28.0; extra == "benchmark"
+Requires-Dist: eval-type-backport~=0.1.3; extra == "benchmark"
+Requires-Dist: hydra-core~=1.3.2; extra == "benchmark"
+Requires-Dist: loguru~=0.7.0; extra == "benchmark"
+Requires-Dist: neptune~=1.6.3; extra == "benchmark"
+Requires-Dist: pydantic~=2.6.1; extra == "benchmark"
+Requires-Dist: pydantic-core~=2.16.2; extra == "benchmark"
+Requires-Dist: pydantic-settings~=2.0.3; extra == "benchmark"
+Requires-Dist: psycopg2-binary~=2.9.9; extra == "benchmark"
```

### Comparing `dbally-0.0.1.dev0/pyproject.toml` & `dbally-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1.dev0/setup.cfg` & `dbally-0.0.2/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -6,51 +6,65 @@
 author_email = contact@deepsense.ai
 license = MIT
 license_files = LICENSE
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
 	Environment :: Console
 	Intended Audience :: Developers
-	License :: Other/Proprietary License
+	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.12
 project_urls = 
 	Documentation = https://db-ally.deepsense.ai/
+	Source = https://github.com/deepsense-ai/db-ally
 
 [options]
 package_dir = 
 	=src
 packages = find:
 zip_safe = False
 platforms = any
 include_package_data = True
 python_requires = >=3.8
 install_requires = 
 	pandas~=2.0.3
 	python-dotenv>=0.5.1
 	SQLAlchemy==2.0.25
 	tabulate>=0.9.0
-	transformers>=4.37.1
 	click~=8.1.7
 	numpy>=1.24.0
 
 [options.extras_require]
 openai = 
 	openai>=1.10.0
 	tiktoken>=0.6.0
 faiss = 
 	faiss-cpu>=1.8.0
 examples = 
 	pydantic~=2.6.0
 	pydantic_settings~=2.1.0
 	psycopg2-binary~=2.9.9
+langsmith = 
+	langsmith>=0.0.87
+transformers = 
+	transformers>=4.37.1
+benchmark = 
+	asyncpg~=0.28.0
+	eval-type-backport~=0.1.3
+	hydra-core~=1.3.2
+	loguru~=0.7.0
+	neptune~=1.6.3
+	pydantic~=2.6.1
+	pydantic-core~=2.16.2
+	pydantic-settings~=2.0.3
+	psycopg2-binary~=2.9.9
 
 [options.packages.find]
 where = src
 
 [bdist_wheel]
 universal = 1
```

### Comparing `dbally-0.0.1.dev0/src/dbally/_main.py` & `dbally-0.0.2/src/dbally/_main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,70 @@
 from typing import List, Optional
 
-from ._collection import Collection
 from .audit.event_handlers.base import EventHandler
+from .collection import Collection
 from .iql_generator.iql_generator import IQLGenerator
 from .llm_client.base import LLMClient
-from .llm_client.openai_client import OpenAIClient
 from .nl_responder.nl_responder import NLResponder
+from .view_selection.base import ViewSelector
 from .view_selection.llm_view_selector import LLMViewSelector
 
-default_llm_client: Optional[LLMClient] = None
-default_event_handlers: List[EventHandler] = []
 
+def create_collection(
+    name: str,
+    llm_client: LLMClient,
+    event_handlers: Optional[List[EventHandler]] = None,
+    view_selector: Optional[ViewSelector] = None,
+    iql_generator: Optional[IQLGenerator] = None,
+    nl_responder: Optional[NLResponder] = None,
+) -> Collection:
+    """
+    Create a new [Collection](collection.md) that is a container for registering views and the\
+    main entrypoint to db-ally features.
+
+    Unlike instantiating a [Collection][dbally.Collection] directly, this function\
+    provides a set of default values for various dependencies like LLM client, view selector,\
+    IQL generator, and NL responder.
+
+    ##Example
+
+    ```python
+        from dbally import create_collection
+        from dbally.llm_client.openai_client import OpenAIClient
 
-def use_openai_llm(model_name: str = "gpt-3.5-turbo", openai_api_key: Optional[str] = None) -> None:
-    """
-    Set default LLM client to use OpenAI.
-
-    Args:
-        model_name: which OpenAI's model should be used
-        openai_api_key: OpenAI's API key - if None OPENAI_API_KEY environment variable will be used
-    """
-    global default_llm_client  # pylint: disable=W0603
-    default_llm_client = OpenAIClient(model_name=model_name, api_key=openai_api_key)
-
-
-def use_event_handler(event_handler: EventHandler) -> None:
-    """
-    Set default event handler to be used by all collections.
+        collection = create_collection("my_collection", llm_client=OpenAIClient())
+    ```
 
     Args:
-        event_handler: The event handler to be used.
-    """
-    global default_event_handlers  # pylint: disable=W0602
-    default_event_handlers.append(event_handler)
-
-
-def create_collection(name: str, event_handlers: Optional[List[EventHandler]] = None) -> Collection:
-    """
-    Create a new collection that is a container for registering views, configuration and main entrypoint to db-ally
-    features.
-
-    Args:
-         name: The name of the collection
-         event_handlers: The event handlers to be used by the collection
+        name: Name of the collection is available for [Event handlers](event_handlers/index.md) and is\
+        used to distinguish different db-ally runs.
+        llm_client: LLM client used by the collection to generate views and respond to natural language\
+        queries.
+        event_handlers: Event handlers used by the collection during query executions. Can be used to\
+        log events as [CLIEventHandler](event_handlers/cli_handler.md) or to validate system performance as\
+        [LangSmithEventHandler](event_handlers/langsmith_handler.md).
+        view_selector: View selector used by the collection to select the best view for the given query.\
+        If None, a new instance of [LLMViewSelector][dbally.view_selection.llm_view_selector.LLMViewSelector]\
+        will be used.
+        iql_generator: IQL generator used by the collection to generate IQL queries from natural language\
+        queries. If None, a new instance of [IQLGenerator][dbally.iql_generator.iql_generator.IQLGenerator]\
+        will be used.
+        nl_responder: NL responder used by the collection to respond to natural language queries. If None,\
+        a new instance of [NLResponder][dbally.nl_responder.nl_responder.NLResponder] will be used.
 
     Returns:
-        a new instance of DBAllyCollection
+        a new instance of db-ally Collection
 
     Raises:
         ValueError: if default LLM client is not configured
     """
-    if not default_llm_client:
-        raise ValueError("LLM client is not set.")
-
-    llm_client = default_llm_client
-    view_selector = LLMViewSelector(llm_client=llm_client)
-    iql_generator = IQLGenerator(llm_client=llm_client)
-    nl_responder = NLResponder(llm_client=llm_client)
-    event_handlers = event_handlers or default_event_handlers
+    view_selector = view_selector or LLMViewSelector(llm_client=llm_client)
+    iql_generator = iql_generator or IQLGenerator(llm_client=llm_client)
+    nl_responder = nl_responder or NLResponder(llm_client=llm_client)
+    event_handlers = event_handlers or []
 
     return Collection(
         name,
         nl_responder=nl_responder,
         view_selector=view_selector,
         iql_generator=iql_generator,
         event_handlers=event_handlers,
```

### Comparing `dbally-0.0.1.dev0/src/dbally/audit/event_handlers/base.py` & `dbally-0.0.2/src/dbally/audit/event_handlers/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,45 +6,52 @@
 
 RequestCtx = TypeVar("RequestCtx")
 EventCtx = TypeVar("EventCtx")
 
 
 class EventHandler(Generic[RequestCtx, EventCtx], ABC):
     """
-    Base event handler interface.
+    A base class that every custom handler should inherit from
     """
 
     @abc.abstractmethod
     async def request_start(self, user_request: RequestStart) -> RequestCtx:
         """
-        Log the start of the request.
+        Function that is called at the beginning of every `Collection.ask` execution.
 
         Args:
-            user_request: The start of the request.
+            user_request: Object containing name of collection and asked query
+
+        Returns:
+            Implementation-specific request context object, which is passed to the future callbacks
         """
 
     @abc.abstractmethod
     async def event_start(self, event: Union[LLMEvent], request_context: RequestCtx) -> EventCtx:
         """
-        Log the start of the event.
+        Function that is called during every event execution.
+
 
         Args:
-            event: Event to be logged.
+            event: LLMEvent to be logged with all the details.
             request_context: Optional context passed from request_start method
+
+        Returns:
+            Implementation-specific request context object, which is passed to the `event_end` callback
         """
 
     @abc.abstractmethod
     async def event_end(
         self, event: Union[None, LLMEvent], request_context: RequestCtx, event_context: EventCtx
     ) -> None:
         """
-        Log the end of the event.
+        Function that is called during every event execution.
 
         Args:
-            event: Event to be logged.
+            event: LLMEvent to be logged with all the details.
             request_context: Optional context passed from request_start method
             event_context: Optional context passed from event_start method
         """
 
     @abc.abstractmethod
     async def request_end(self, output: RequestEnd, request_context: RequestCtx) -> None:
         """
```

### Comparing `dbally-0.0.1.dev0/src/dbally/audit/event_handlers/cli_event_handler.py` & `dbally-0.0.2/src/dbally/audit/event_handlers/cli_event_handler.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,15 +13,29 @@
 
 from dbally.audit.event_handlers.base import EventHandler
 from dbally.data_models.audit import LLMEvent, RequestEnd, RequestStart
 
 
 class CLIEventHandler(EventHandler):
     """
-    CLI event handler interface.
+    This handler displays all interactions between LLM and user happending during `Collection.ask`\
+    execution inside the terminal.
+
+    ### Usage
+
+    ```python
+        import dbally
+        from dbally.audit.event_handlers.cli_event_handler import CLIEventHandler
+
+        my_collection = dbally.create_collection("my_collection", llm, event_handlers=[CLIEventHandler()])
+    ```
+
+    After using `CLIEventHandler`, during every `Collection.ask` execution you will see output similar to the one below:
+
+    ![Example output from CLIEventHandler](../../assets/event_handler_example.png)
     """
 
     def __init__(self) -> None:
         super().__init__()
         self._console = Console() if RICH_OUTPUT else None
 
     def _print_syntax(self, content: str, lexer: str) -> None:
@@ -29,30 +43,31 @@
             console_content = Syntax(content, lexer, word_wrap=True)
             self._console.print(console_content)
         else:
             print(content)
 
     async def request_start(self, user_request: RequestStart) -> None:
         """
-        Log the start of the request.
+        Displays information about event starting to the terminal.
 
         Args:
-            user_request: The start of the request.
+            user_request: Object containing name of collection and asked query
         """
 
         pprint(f"[orange3 bold]Request starts... \n[orange3 bold]MESSAGE: [grey53]{user_request.question}")
         pprint("[grey53]\n=======================================")
         pprint("[grey53]=======================================\n")
 
     async def event_start(self, event: Union[LLMEvent], request_context: None) -> None:
         """
-        Log the start of the event.
+        Displays information that event has started, then all messages inside the prompt
+
 
         Args:
-            event: Event to be logged.
+            event: LLMEvent to be logged with all the details.
             request_context: Optional context passed from request_start method
         """
 
         if isinstance(event, LLMEvent):
             pprint(f"[cyan bold]LLM event starts... \n[cyan bold]LLM EVENT PROMPT TYPE: [grey53]{event.type}")
 
             if isinstance(event.prompt, tuple):
@@ -60,33 +75,33 @@
                     pprint(f"\n[orange3]{msg['role']}")
                     self._print_syntax(msg["content"], "text")
             else:
                 self._print_syntax(f"{event.prompt}", "text")
 
     async def event_end(self, event: Union[None, LLMEvent], request_context: None, event_context: None) -> None:
         """
-        Log the end of the event.`
+        Displays the response from the LLM.
 
         Args:
-            event: Event to be logged.
+            event: LLMEvent to be logged with all the details.
             request_context: Optional context passed from request_start method
             event_context: Optional context passed from event_start method
         """
 
         if isinstance(event, LLMEvent):
             pprint(f"\n[green bold]RESPONSE: {event.response}")
             pprint("[grey53]\n=======================================")
             pprint("[grey53]=======================================\n")
 
     async def request_end(self, output: RequestEnd, request_context: Optional[dict] = None) -> None:
         """
-        Log the end of the request.
+        Displays the output of the request, namely the `results` and the `context`
 
         Args:
-            output: The output of the request. In this case - PSQL query.
+            output: The output of the request.
             request_context: Optional context passed from request_start method
         """
 
         pprint("[green bold]REQUEST OUTPUT:")
         pprint(f"Number of rows: {len(output.result.results)}")
         if "sql" in output.result.context:
             self._print_syntax(f"{output.result.context['sql']}", "psql")
```

### Comparing `dbally-0.0.1.dev0/src/dbally/audit/event_handlers/langsmith_event_handler.py` & `dbally-0.0.2/src/dbally/audit/event_handlers/langsmith_event_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,25 +5,30 @@
 from langsmith.client import Client
 from langsmith.run_trees import RunTree
 
 from dbally.audit.event_handlers.base import EventHandler
 from dbally.data_models.audit import LLMEvent, RequestEnd, RequestStart
 
 
-class LangsmithEventHandler(EventHandler[RunTree, RunTree]):
+class LangSmithEventHandler(EventHandler[RunTree, RunTree]):
     """
-    Logs events to a Langsmith instance.
+    This handler Logs events to a LangSmith instance.
+
+
+    !!! tip
+        To learn how to use `LangSmithEventHandler` visit
+        [How-To: Log db-ally runs to LangSmith](../../how-to/log_runs_to_langsmith.md)
     """
 
     def __init__(self, api_key: str):
         self._client = Client(api_key=api_key)
 
     async def request_start(self, user_request: RequestStart) -> RunTree:
         """
-        Log the start of the request.
+        Initializes the `RunTree` object with all required attributes.
 
         Args:
             user_request: The start of the request.
 
         Returns:
             run_tree object for a request span
         """
@@ -60,15 +65,15 @@
 
             return child_run
 
         raise ValueError("Unsupported event")
 
     async def event_end(self, event: Union[None, LLMEvent], request_context: RunTree, event_context: RunTree) -> None:
         """
-        Log the end of the event.`
+        Log the end of the event.
 
         Args:
             event: Event to be logged.
             request_context: Optional context passed from request_start method
             event_context: Optional context passed from event_start method
         """
         if isinstance(event, LLMEvent):
```

### Comparing `dbally-0.0.1.dev0/src/dbally/audit/event_tracker.py` & `dbally-0.0.2/src/dbally/audit/event_tracker.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1.dev0/src/dbally/data_models/audit.py` & `dbally-0.0.2/src/dbally/data_models/audit.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass
 from enum import Enum
 from typing import Optional, Union
 
+from dbally.data_models.execution_result import ExecutionResult
 from dbally.data_models.prompts.prompt_template import ChatFormat
-from dbally.views.base import ExecutionResult
 
 
 class EventType(Enum):
     """
     Enum for event types.
     """
```

### Comparing `dbally-0.0.1.dev0/src/dbally/data_models/llm_options.py` & `dbally-0.0.2/src/dbally/data_models/llm_options.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from dataclasses import asdict, dataclass
 from typing import List, Optional, Union
 
 
 @dataclass
 class LLMOptions:
     """
-    Dataclass that represents all available LLM call options. Each of them is
-    described in details here: https://platform.openai.com/docs/api-reference/chat/create.
+    Dataclass that represents all available LLM call options for the OpenAI API. Each of them is
+    described in the [OpenAI API documentation](https://platform.openai.com/docs/api-reference/chat/create.)
     """
 
     frequency_penalty: Optional[float]
     max_tokens: Optional[int]
     n: Optional[int]
     presence_penalty: Optional[float]
     seed: Optional[int]
```

### Comparing `dbally-0.0.1.dev0/src/dbally/data_models/prompts/__init__.py` & `dbally-0.0.2/src/dbally/data_models/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1.dev0/src/dbally/data_models/prompts/common_validation_utils.py` & `dbally-0.0.2/src/dbally/data_models/prompts/common_validation_utils.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1.dev0/src/dbally/data_models/prompts/iql_explainer_prompt_template.py` & `dbally-0.0.2/src/dbally/data_models/prompts/iql_explainer_prompt_template.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1.dev0/src/dbally/data_models/prompts/iql_prompt_template.py` & `dbally-0.0.2/src/dbally/data_models/prompts/iql_prompt_template.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1.dev0/src/dbally/data_models/prompts/nl_responder_prompt_template.py` & `dbally-0.0.2/src/dbally/data_models/prompts/nl_responder_prompt_template.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1.dev0/src/dbally/data_models/prompts/prompt_template.py` & `dbally-0.0.2/src/dbally/data_models/prompts/prompt_template.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1.dev0/src/dbally/data_models/prompts/view_selector_prompt_template.py` & `dbally-0.0.2/src/dbally/data_models/prompts/view_selector_prompt_template.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1.dev0/src/dbally/embedding_client/base.py` & `dbally-0.0.2/src/dbally/embedding_client/base.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1.dev0/src/dbally/embedding_client/openai.py` & `dbally-0.0.2/src/dbally/embedding_client/openai.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1.dev0/src/dbally/iql/_exceptions.py` & `dbally-0.0.2/src/dbally/iql/_exceptions.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1.dev0/src/dbally/iql/_processor.py` & `dbally-0.0.2/src/dbally/iql/_processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     IQLArgumentParsingError,
     IQLArgumentValidationError,
     IQLError,
     IQLFunctionNotExists,
     IQLUnsupportedSyntaxError,
 )
 from dbally.iql._type_validators import validate_arg_type
-from dbally.similarity.index import SimilarityIndex
 
 if TYPE_CHECKING:
     from dbally.views.base import ExposedFunction
 
 
 class IQLProcessor:
     """
@@ -80,19 +79,16 @@
 
         if len(func_def.parameters) != len(node.args):
             raise ValueError(f"The method {func.id} has incorrect number of arguments")
 
         for arg, arg_def in zip(node.args, func_def.parameters):
             arg_value = self._parse_arg(arg)
 
-            if hasattr(arg_def.type, "__metadata__"):
-                similarity_indexes = [meta for meta in arg_def.type.__metadata__ if isinstance(meta, SimilarityIndex)]
-
-                if similarity_indexes:
-                    arg_value = await similarity_indexes[0].similar(arg_value)
+            if arg_def.similarity_index:
+                arg_value = await arg_def.similarity_index.similar(arg_value)
 
             check_result = validate_arg_type(arg_def.type, arg_value)
 
             if not check_result.valid:
                 raise IQLArgumentValidationError(message=check_result.reason or "", node=arg, source=self.source)
 
             args.append(check_result.casted_value if check_result.casted_value is not ... else arg_value)
```

### Comparing `dbally-0.0.1.dev0/src/dbally/iql/_query.py` & `dbally-0.0.2/src/dbally/iql/_query.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1.dev0/src/dbally/iql/_type_validators.py` & `dbally-0.0.2/src/dbally/iql/_type_validators.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1.dev0/src/dbally/iql/syntax.py` & `dbally-0.0.2/src/dbally/iql/syntax.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,45 +15,50 @@
 class Node:
     """
     Base class for all nodes in the IQL.
     """
 
     def is_bool_op(self) -> IsBoolOpType:
         """
-           Checks if node is a boolean operation.
+        Checks if node is a boolean operation.
 
-        :returns: True if the node is a boolean operation, otherwise False.
+        Returns:
+            True if the node is a boolean operation, otherwise False.
         """
         return isinstance(self, BoolOp)
 
     def is_function_call(self) -> IsFunctionCallType:
         """
-           Checks if node is a function call.
+        Checks if node is a function call.
 
-        :returns: True if the node is a function call, otherwise False.
+        Returns:
+            True if the node is a function call, otherwise False.
         """
         return isinstance(self, FunctionCall)
 
 
 class BoolOp(Node):
     """
     Base class for boolean operator nodes.
     """
 
     def match(self, not_: Callable[["Not"], Any], and_: Callable[["And"], Any], or_: Callable[["Or"], Any]) -> Any:
         """
         Match syntax for convenient query building based on BoolOp type.
 
-        :param not_: Callable executed when node is Not
-        :param and_: Callable executed when node is And
-        :param or_: Callable executed when node is Or
+        Args:
+            not_: Callable executed when node is Not
+            and_: Callable executed when node is And
+            or_: Callable executed when node is Or
 
-        :returns: Result of chosen callable.
+        Returns:
+            Result of chosen callable.
 
-        :raises ValueError: if node is not of any supported boolean types
+        Raises:
+            ValueError: if node is not of any supported boolean types
         """
         if isinstance(self, Not):
             return not_(self)
         if isinstance(self, And):
             return and_(self)
         if isinstance(self, Or):
             return or_(self)
```

### Comparing `dbally-0.0.1.dev0/src/dbally/iql_generator/iql_generator.py` & `dbally-0.0.2/src/dbally/iql_generator/iql_generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,47 +8,54 @@
 from dbally.views.base import ExposedFunction
 
 
 class IQLGenerator:
     """
     Class used to generate IQL from natural language question.
 
-    Attributes:
-        llm_client: LLM client used to generate IQL
-        prompt_template: template for the prompt
-        prompt_builder: PromptBuilder used to insert arguments into the prompt and adjust style per model
-        promptify_view: Function formatting filters for prompt
+    In db-ally, LLM uses IQL (Intermediate Query Language) to express complex queries in a simplified way.
+    The class used to generate IQL from natural language query is `IQLGenerator`.
+
+    IQL generation is done using the method `self.generate_iql`.
+    It uses LLM to generate text-based responses, passing in the prompt template, formatted filters, and user question.
     """
 
     _ERROR_MSG_PREFIX = "Unfortunately, generated IQL is not valid. Please try again, \
                         generation of correct IQL is very important. Below you have errors generated by the system: \n"
 
     TException = TypeVar("TException", bound=Exception)
 
     def __init__(
         self,
         llm_client: LLMClient,
         prompt_template: Optional[IQLPromptTemplate] = None,
         prompt_builder: Optional[PromptBuilder] = None,
         promptify_view: Optional[Callable] = None,
     ) -> None:
+        """
+        Args:
+            llm_client: LLM client used to generate IQL
+            prompt_template: If not provided by the users is set to `default_iql_template`
+            prompt_builder: PromptBuilder used to insert arguments into the prompt and adjust style per model.
+            promptify_view: Function formatting filters for prompt
+        """
         self._llm_client = llm_client
         self._prompt_template = prompt_template or copy.deepcopy(default_iql_template)
         self._prompt_builder = prompt_builder or PromptBuilder()
         self._promptify_view = promptify_view or _promptify_filters
 
     async def generate_iql(
         self,
         filters: List[ExposedFunction],
         question: str,
         event_tracker: EventTracker,
         conversation: Optional[IQLPromptTemplate] = None,
     ) -> Tuple[str, IQLPromptTemplate]:
-        # todo: add more generation-related arguments here once BaseLLM interface is established
-        """Uses LLM to generate IQL in text form
+        """
+        Uses LLM to generate IQL in text form
 
         Args:
             question: user question
             filters: list of filters exposed by the view
             event_tracker: event store used to audit the generation process
             conversation: conversation to be continued
 
@@ -71,22 +78,23 @@
             conversation = self._prompt_template
 
         conversation = conversation.add_assistant_message(content=llm_response)
 
         return iql_filters, conversation
 
     def add_error_msg(self, conversation: IQLPromptTemplate, errors: List[TException]) -> IQLPromptTemplate:
-        """_summary_
+        """
+        Appends to the conversation error messages returned due to the invalid IQL generated by the LLM.
 
         Args:
-            conversation (IQLPromptTemplate): _description_
-            errors (List[Exception]): _description_
+            conversation (IQLPromptTemplate): conversation containing current IQL generation trace
+            errors (List[Exception]): errors to be appended
 
         Returns:
-            IQLPromptTemplate: _description_
+            IQLPromptTemplate: Conversation extended with errors
         """
 
         msg = self._ERROR_MSG_PREFIX
         for error in errors:
             msg += str(error) + "\n"
 
         return conversation.add_user_message(content=msg)
```

### Comparing `dbally-0.0.1.dev0/src/dbally/llm_client/base.py` & `dbally-0.0.2/src/dbally/llm_client/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,22 @@
 from dbally.audit.event_tracker import EventTracker
 from dbally.data_models.audit import LLMEvent
 from dbally.data_models.llm_options import LLMOptions
 from dbally.prompts.prompt_builder import ChatFormat, PromptBuilder, PromptTemplate
 
 
 class LLMClient(abc.ABC):
-    """Abstract client for interaction with LLM."""
+    """
+    Abstract client for interaction with LLM.
+
+    It accepts parameters including the template, format, event tracker,
+    and optional generation parameters like frequency_penalty, max_tokens, and temperature
+    (the full list of options is provided by the [`LLMOptions` class][dbally.data_models.llm_options.LLMOptions]).
+    It constructs a prompt using the `PromptBuilder` instance and generates text using the `self.call` method.
+    """
 
     def __init__(self, model_name: str):
         self.model_name = model_name
         self._prompt_builder = PromptBuilder(self.model_name)
 
     async def text_generation(  # pylint: disable=R0913
         self,
@@ -52,31 +59,32 @@
         )
 
         prompt = self._prompt_builder.build(template, fmt)
 
         event = LLMEvent(prompt=prompt, type=type(template).__name__)
 
         async with event_tracker.track_event(event) as span:
-            event.response = await self._call(prompt, template.response_format, options, event)
+            event.response = await self.call(prompt, template.response_format, options, event)
             span(event)
 
         return event.response
 
     @abc.abstractmethod
-    async def _call(
+    async def call(
         self,
         prompt: Union[str, ChatFormat],
         response_format: Optional[Dict[str, str]],
         options: LLMOptions,
         event: LLMEvent,
     ) -> str:
         """
         Calls LLM API endpoint.
 
         Args:
-            prompt: Text to be asked.
-            response_format: Optional argument used in the OpenAI API - used to force json output
+            prompt: prompt passed to the LLM.
+            response_format: Optional argument used in the OpenAI API - used to force a json output
             options: Additional settings used by LLM.
+            event: an LLMEvent instance which fields should be filled during the method execution.
 
         Returns:
             Response string from LLM.
         """
```

### Comparing `dbally-0.0.1.dev0/src/dbally/nl_responder/nl_responder.py` & `dbally-0.0.2/src/dbally/nl_responder/nl_responder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import copy
 from typing import Dict, List, Optional
 
 import pandas as pd
 
 from dbally.audit.event_tracker import EventTracker
-from dbally.data_models.execution_result import ExecutionResult
+from dbally.data_models.execution_result import ViewExecutionResult
 from dbally.data_models.prompts.iql_explainer_prompt_template import (
     IQLExplainerPromptTemplate,
     default_iql_explainer_template,
 )
 from dbally.data_models.prompts.nl_responder_prompt_template import (
     NLResponderPromptTemplate,
     default_nl_responder_template,
@@ -24,34 +24,34 @@
         self,
         llm_client: LLMClient,
         iql_explainer_prompt_template: Optional[IQLExplainerPromptTemplate] = None,
         nl_responder_prompt_template: Optional[NLResponderPromptTemplate] = None,
         max_tokens_count: int = 4096,
     ) -> None:
         """
-        Initializes NLResponser class.
-
         Args:
             llm_client: LLM client used to generate natural language response
-            iql_explainer_prompt_template: template for the prompt used to generate the iql explanation
-            nl_responder_prompt_template: template for the prompt used to generate the NL response
+            iql_explainer_prompt_template: template for the prompt used to generate the iql explanation\
+            if not set defaults to `default_iql_explainer_template`
+            nl_responder_prompt_template: template for the prompt used to generate the NL response\
+            if not set defaults to `nl_responder_prompt_template`
             max_tokens_count: maximum number of tokens that can be used in the prompt
         """
 
         self._llm_client = llm_client
         self._nl_responder_prompt_template = nl_responder_prompt_template or copy.deepcopy(
             default_nl_responder_template
         )
         self._iql_explainer_prompt_template = iql_explainer_prompt_template or copy.deepcopy(
             default_iql_explainer_template
         )
         self._max_tokens_count = max_tokens_count
 
     async def generate_response(
-        self, result: ExecutionResult, question: str, filters: str, event_tracker: EventTracker
+        self, result: ViewExecutionResult, question: str, filters: str, event_tracker: EventTracker
     ) -> str:
         """
         Uses LLM to generate a response in natural language form.
 
         Args:
             result: object representing the result of the query execution
             question: user question
```

### Comparing `dbally-0.0.1.dev0/src/dbally/nl_responder/token_counters.py` & `dbally-0.0.2/src/dbally/nl_responder/token_counters.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     Raises:
         ImportError: If transformers package is not installed.
     """
 
     try:
         from transformers import AutoTokenizer  # pylint: disable=import-outside-toplevel
     except ImportError as exc:
-        raise ImportError("You need to install transformers package to use Anyscale models' tokenizers.") from exc
+        raise ImportError("You need to install transformers package to use huggingface models' tokenizers.") from exc
 
     tokenizer = AutoTokenizer.from_pretrained(model)
 
     for message in messages:
         message["content"] = message["content"].format(**fmt)
 
     return len(tokenizer.apply_chat_template(messages, tokenize=True, add_generation_prompt=True))
```

### Comparing `dbally-0.0.1.dev0/src/dbally/prompts/prompt_builder.py` & `dbally-0.0.2/src/dbally/prompts/prompt_builder.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,62 @@
-from typing import Dict, Optional, Union
-
-from transformers import AutoTokenizer
-from transformers.tokenization_utils import PreTrainedTokenizer
+from typing import TYPE_CHECKING, Dict, Optional, Union
 
 from dbally.data_models.prompts.prompt_template import ChatFormat, PromptTemplate
 
+if TYPE_CHECKING:
+    from transformers.tokenization_utils import PreTrainedTokenizer
+
 
 class PromptBuilder:
     """Class used to build prompts"""
 
     def __init__(self, model_name: Optional[str] = None) -> None:
         """
-        Init PromptBuilder.
-
         Args:
             model_name: Name of the model to load a tokenizer for.
                         Tokenizer is used to append special tokens to the prompt. If empty, no tokens will be added.
+
         Raises:
             OSError: If model_name is not found in huggingface.co/models
         """
-        self._tokenizer: Optional[PreTrainedTokenizer] = None
-        if model_name is not None:
-            # openAI client handles special tokens for gpt.
-            if not model_name.startswith("gpt"):
-                self._tokenizer = AutoTokenizer.from_pretrained(model_name)
+        self._tokenizer: Optional["PreTrainedTokenizer"] = None
+
+        if model_name is not None and not model_name.startswith("gpt"):
+            try:
+                from transformers import AutoTokenizer  # pylint: disable=import-outside-toplevel
+            except ImportError as exc:
+                raise ImportError("You need to install transformers package to use huggingface models.") from exc
+
+            self._tokenizer = AutoTokenizer.from_pretrained(model_name)
 
-    def _format_prompt(self, prompt_template: PromptTemplate, fmt: Dict[str, str]) -> ChatFormat:
+    def format_prompt(self, prompt_template: PromptTemplate, fmt: Dict[str, str]) -> ChatFormat:
         """
         Format prompt using provided arguments
 
         Args:
             prompt_template: this template will be modified in place
             fmt: formatting dict
 
         Returns:
             ChatFormat formatted prompt
         """
         return tuple({**msg, "content": msg["content"].format(**fmt)} for msg in prompt_template.chat)
 
     def build(self, prompt_template: PromptTemplate, fmt: Dict[str, str]) -> Union[str, ChatFormat]:
-        """Build prompt
+        """Build the prompt
 
         Args:
             prompt_template: Prompt template in system/user/assistant openAI format.
             fmt: Dictionary with formatting.
 
         Returns:
             Either prompt as a string (if it was formatted for a hf model, model_name provided), or prompt as an
             openAI client style list.
 
         Raises:
             KeyError: If fmt does not fill all template arguments.
         """
 
-        prompt = self._format_prompt(prompt_template, fmt)
+        prompt = self.format_prompt(prompt_template, fmt)
         if self._tokenizer is not None:
             prompt = self._tokenizer.apply_chat_template(prompt, tokenize=False, add_generation_prompt=True)
         return prompt
```

### Comparing `dbally-0.0.1.dev0/src/dbally/similarity/faiss_store.py` & `dbally-0.0.2/src/dbally/similarity/faiss_store.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from pathlib import Path
 from typing import List, Optional
 
 import faiss
 import numpy as np
 
 from dbally.embedding_client.base import EmbeddingClient
-from dbally.similarity.store import AbstractStore
+from dbally.similarity.store import SimilarityStore
 
 
-class FaissStore(AbstractStore):
+class FaissStore(SimilarityStore):
     """
-    Store for text embeddings using Meta Faiss.
+    The FaissStore class stores text embeddings using Meta Faiss.
     """
 
     def __init__(
         self,
         index_dir: str,
         index_name: str,
         embedding_client: EmbeddingClient,
@@ -26,15 +26,15 @@
 
         Args:
             index_dir: The directory to store the index file.
             index_name: The name of the index.
             max_distance: The maximum distance between two text embeddings to be considered similar.
             embedding_client: The client to use for creating text embeddings.
             index_type: The type of Faiss index to use. Defaults to faiss.IndexFlatL2. See
-                [https://github.com/facebookresearch/faiss/wiki/Faiss-indexes](Faiss wiki) for more information.
+                [Faiss wiki](https://github.com/facebookresearch/faiss/wiki/Faiss-indexes) for more information.
         """
         super().__init__()
         self.index_dir = index_dir
         self.index_name = index_name
         self.max_distance = max_distance
         self.embedding_client = embedding_client
         self.index_type = index_type
@@ -76,15 +76,15 @@
         """
         Finds the most similar text in the store or returns None if no similar text is found.
 
         Args:
             text: The text to find similar to.
 
         Returns:
-            Optional[str]: The most similar text or None if no similar text is found.
+            The most similar text or None if no similar text is found.
         """
         index = faiss.read_index(str(self.get_index_path()))
         embedding = np.array(await self.embedding_client.get_embeddings([text]), dtype=np.float32)
         scores, similar = index.search(embedding, 1)
         best_distance, best_idx = scores[0][0], similar[0][0]
 
         if best_idx != -1 and (self.max_distance is None or best_distance <= self.max_distance):
```

### Comparing `dbally-0.0.1.dev0/src/dbally/similarity/index.py` & `dbally-0.0.2/src/dbally/similarity/index.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import abc
 
-from dbally.similarity.fetcher import AbstractFetcher
-from dbally.similarity.store import AbstractStore
+from dbally.similarity.fetcher import SimilarityFetcher
+from dbally.similarity.store import SimilarityStore
 
 
 class AbstractSimilarityIndex(metaclass=abc.ABCMeta):
     """
     Base class for all similarity indexes.
 
     Usually it is recommended to use the SimilarityIndex class directly instead. AbstractSimilarityIndex may be used
@@ -31,18 +31,23 @@
             str: The most similar text or the original text if no similar text is found.
         """
 
 
 class SimilarityIndex(AbstractSimilarityIndex):
     """
     Merges the store and the fetcher to provide a simple interface for keeping
-    the data store and the similairty store in sync and finding similar texts.
+    the data store and the similarity store in sync and finding similar texts.
     """
 
-    def __init__(self, store: AbstractStore, fetcher: AbstractFetcher):
+    def __init__(self, store: SimilarityStore, fetcher: SimilarityFetcher):
+        """
+        Args:
+            store: stores values gathered by the fetcher
+            fetcher: fetches unique values to be indexed
+        """
         self.store = store
         self.fetcher = fetcher
 
     async def update(self) -> None:
         """
         Updates the store with the latest data from the fetcher.
         """
```

### Comparing `dbally-0.0.1.dev0/src/dbally/similarity/sqlalchemy_base.py` & `dbally-0.0.2/src/dbally/similarity/sqlalchemy_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import abc
 from typing import List, Optional
 
 import sqlalchemy
 from sqlalchemy.sql.elements import ColumnClause
 
-from dbally.similarity.fetcher import AbstractFetcher
-from dbally.similarity.store import AbstractStore
+from dbally.similarity.fetcher import SimilarityFetcher
+from dbally.similarity.store import SimilarityStore
 
 
-class SqlAlchemyFetcher(AbstractFetcher):
+class SqlAlchemyFetcher(SimilarityFetcher):
     """
     Fetches the data from the database using SQLAlchemy.
     """
 
     def __init__(self, sqlalchemy_engine: sqlalchemy.engine.Engine) -> None:
         self.sqlalchemy_engine = sqlalchemy_engine
 
@@ -26,15 +26,15 @@
         """
 
     async def fetch(self) -> List[str]:
         """
         Fetches the data from the source and returns it as a list of strings.
 
         Returns:
-            List[str]: The fetched data.
+            The fetched data.
         """
         with self.sqlalchemy_engine.connect() as conn:
             result = conn.execute(self.get_query())
             return [row[0] for row in result]
 
 
 class SimpleSqlAlchemyFetcher(SqlAlchemyFetcher):
@@ -50,29 +50,29 @@
         self.table = table
 
     def get_query(self) -> sqlalchemy.Select:
         """
         Returns query that will be used to fetch the data from the database.
 
         Returns:
-            sqlalchemy.Select: The query to fetch the data.
+            The query to fetch the data.
         """
         return sqlalchemy.select(self.column).select_from(self.table).distinct()
 
 
-class AbstractSqlAlchemyStore(AbstractStore, metaclass=abc.ABCMeta):
+class AbstractSqlAlchemyStore(SimilarityStore, metaclass=abc.ABCMeta):
     """
     Stores the data in the database using SQLAlchemy.
     """
 
-    def __init__(self, sqlalchemy_engine: sqlalchemy.engine.Engine, table_name: str, treshold: float = 0.8) -> None:
+    def __init__(self, sqlalchemy_engine: sqlalchemy.engine.Engine, table_name: str, threshold: float = 0.8) -> None:
         self.sqlalchemy_engine = sqlalchemy_engine
         self.table_name = table_name
         self.table = sqlalchemy.Table(table_name, sqlalchemy.MetaData(), sqlalchemy.Column("text", sqlalchemy.String))
-        self.treshold = treshold
+        self.threshold = threshold
 
     async def store(self, data: List[str]) -> None:
         """
         Stores the data. Should replace the previously stored data.
 
         Args:
             data: The data to store.
@@ -96,13 +96,13 @@
         """
         Finds the text from the store that differs from the given text only in case.
 
         Args:
             text: The text to find similar to.
 
         Returns:
-            Optional[str]: The most similar text or None if no similar text is found.
+            The most similar text or None if no similar text is found.
         """
         with self.sqlalchemy_engine.connect() as conn:
             result = conn.execute(sqlalchemy.select(self.table.c.text).where(self.table.c.text.ilike(text)))
             row = result.fetchone()
             return row[0] if row else None
```

### Comparing `dbally-0.0.1.dev0/src/dbally/view_selection/base.py` & `dbally-0.0.2/src/dbally/view_selection/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 class ViewSelector(abc.ABC):
     """Base class for view selectors."""
 
     @abc.abstractmethod
     async def select_view(self, question: str, views: Dict[str, str], event_tracker: EventTracker) -> str:
         """
-        Based on user question and list of available views select most relevant one.
+        Based on user question and list of available views select the most relevant one.
 
         Args:
-            question: user question.
+            question: user question asked in the natural language e.g "Do we have any data scientists?"
             views: dictionary of available view names with corresponding descriptions.
             event_tracker: event tracker used to audit the selection process.
 
         Returns:
-            most relevant view name.
+            The most relevant view name.
         """
```

### Comparing `dbally-0.0.1.dev0/src/dbally/view_selection/random_view_selector.py` & `dbally-0.0.2/src/dbally/view_selection/random_view_selector.py`

 * *Files identical despite different names*

### Comparing `dbally-0.0.1.dev0/src/dbally/views/base.py` & `dbally-0.0.2/src/dbally/views/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import abc
 import re
 from dataclasses import dataclass
 from typing import _GenericAlias  # type: ignore
-from typing import List, Union
+from typing import List, Optional, Union
 
-from dbally.data_models.execution_result import ExecutionResult
+from dbally.data_models.execution_result import ViewExecutionResult
 from dbally.iql import IQLQuery
+from dbally.similarity import AbstractSimilarityIndex
 
 
 def parse_param_type(param_type: Union[type, _GenericAlias]) -> str:
     """
     Parses the type of a method parameter and returns a string representation of it.
 
     Args:
@@ -34,14 +35,25 @@
 
     name: str
     type: Union[type, _GenericAlias]
 
     def __str__(self) -> str:
         return f"{self.name}: {parse_param_type(self.type)}"
 
+    @property
+    def similarity_index(self) -> Optional[AbstractSimilarityIndex]:
+        """
+        Returns the SimilarityIndex object if the type is annotated with it.
+        """
+        if hasattr(self.type, "__metadata__"):
+            similarity_indexes = [meta for meta in self.type.__metadata__ if isinstance(meta, AbstractSimilarityIndex)]
+            return similarity_indexes[0] if similarity_indexes else None
+
+        return None
+
 
 @dataclass
 class ExposedFunction:
     """
     Represents a function exposed to the AI model.
     """
 
@@ -56,32 +68,36 @@
             return f"{base_str} - {self.description}"
 
         return base_str
 
 
 class AbstractBaseView(metaclass=abc.ABCMeta):
     """
-    Base class for all views. Has to be able to list all available filters, apply them and generate SQL,
-    but ottherwise is implementation agnostic.
+    Base class for all [Views](../../concepts/views.md). All classes implementing this interface has\
+    to be able to list all available filters, apply them and execute queries.
     """
 
     @abc.abstractmethod
     def list_filters(self) -> List[ExposedFunction]:
         """
-        Lists all available filters.
+
+        Returns:
+            Filters defined inside the View.
         """
 
     @abc.abstractmethod
     async def apply_filters(self, filters: IQLQuery) -> None:
         """
         Applies the chosen filters to the view.
 
-        :param filters: IQLQuery object representing the filters to apply
+        Args:
+            filters: [IQLQuery](../../concepts/iql.md) object representing the filters to apply
         """
 
     @abc.abstractmethod
-    def execute(self, dry_run: bool = False) -> ExecutionResult:
+    def execute(self, dry_run: bool = False) -> ViewExecutionResult:
         """
         Executes the query and returns the result.
 
-        :param dry_run: if True, only generate the query without executing it
+        Args:
+            dry_run: if True, should only generate the query without executing it
         """
```

### Comparing `dbally-0.0.1.dev0/src/dbally.egg-info/PKG-INFO` & `dbally-0.0.2/src/dbally.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,50 @@
 Metadata-Version: 2.1
 Name: dbally
-Version: 0.0.1.dev0
+Version: 0.0.2
 Summary: "Efficient, consistent and secure library for querying structured data with natural language"
 Author: deepsense.ai
 Author-email: contact@deepsense.ai
 License: MIT
 Project-URL: Documentation, https://db-ally.deepsense.ai/
+Project-URL: Source, https://github.com/deepsense-ai/db-ally
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: pandas~=2.0.3
 Requires-Dist: python-dotenv>=0.5.1
 Requires-Dist: SQLAlchemy==2.0.25
 Requires-Dist: tabulate>=0.9.0
-Requires-Dist: transformers>=4.37.1
 Requires-Dist: click~=8.1.7
 Requires-Dist: numpy>=1.24.0
 Provides-Extra: openai
 Requires-Dist: openai>=1.10.0; extra == "openai"
 Requires-Dist: tiktoken>=0.6.0; extra == "openai"
 Provides-Extra: faiss
 Requires-Dist: faiss-cpu>=1.8.0; extra == "faiss"
 Provides-Extra: examples
 Requires-Dist: pydantic~=2.6.0; extra == "examples"
 Requires-Dist: pydantic_settings~=2.1.0; extra == "examples"
 Requires-Dist: psycopg2-binary~=2.9.9; extra == "examples"
+Provides-Extra: langsmith
+Requires-Dist: langsmith>=0.0.87; extra == "langsmith"
+Provides-Extra: transformers
+Requires-Dist: transformers>=4.37.1; extra == "transformers"
+Provides-Extra: benchmark
+Requires-Dist: asyncpg~=0.28.0; extra == "benchmark"
+Requires-Dist: eval-type-backport~=0.1.3; extra == "benchmark"
+Requires-Dist: hydra-core~=1.3.2; extra == "benchmark"
+Requires-Dist: loguru~=0.7.0; extra == "benchmark"
+Requires-Dist: neptune~=1.6.3; extra == "benchmark"
+Requires-Dist: pydantic~=2.6.1; extra == "benchmark"
+Requires-Dist: pydantic-core~=2.16.2; extra == "benchmark"
+Requires-Dist: pydantic-settings~=2.0.3; extra == "benchmark"
+Requires-Dist: psycopg2-binary~=2.9.9; extra == "benchmark"
```

### Comparing `dbally-0.0.1.dev0/src/dbally.egg-info/SOURCES.txt` & `dbally-0.0.2/src/dbally.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,24 +4,27 @@
 pyproject.toml
 setup.cfg
 setup.py
 src/py.typed
 src/dbally/VERSION
 src/dbally/__init__.py
 src/dbally/__version__.py
-src/dbally/_collection.py
 src/dbally/_main.py
+src/dbally/collection.py
 src/dbally/py.typed
 src/dbally.egg-info/PKG-INFO
 src/dbally.egg-info/SOURCES.txt
 src/dbally.egg-info/dependency_links.txt
 src/dbally.egg-info/entry_points.txt
 src/dbally.egg-info/not-zip-safe
 src/dbally.egg-info/requires.txt
 src/dbally.egg-info/top_level.txt
+src/dbally/assistants/__init__.py
+src/dbally/assistants/base.py
+src/dbally/assistants/openai.py
 src/dbally/audit/__init__.py
 src/dbally/audit/event_span.py
 src/dbally/audit/event_tracker.py
 src/dbally/audit/event_handlers/__init__.py
 src/dbally/audit/event_handlers/base.py
 src/dbally/audit/event_handlers/cli_event_handler.py
 src/dbally/audit/event_handlers/langsmith_event_handler.py
@@ -35,18 +38,14 @@
 src/dbally/data_models/prompts/iql_prompt_template.py
 src/dbally/data_models/prompts/nl_responder_prompt_template.py
 src/dbally/data_models/prompts/prompt_template.py
 src/dbally/data_models/prompts/view_selector_prompt_template.py
 src/dbally/embedding_client/__init__.py
 src/dbally/embedding_client/base.py
 src/dbally/embedding_client/openai.py
-src/dbally/examples/__init__.py
-src/dbally/examples/db.py
-src/dbally/examples/recruiting.py
-src/dbally/examples/views.py
 src/dbally/iql/__init__.py
 src/dbally/iql/_exceptions.py
 src/dbally/iql/_processor.py
 src/dbally/iql/_query.py
 src/dbally/iql/_type_validators.py
 src/dbally/iql/syntax.py
 src/dbally/iql_generator/__init__.py
@@ -56,14 +55,15 @@
 src/dbally/llm_client/openai_client.py
 src/dbally/nl_responder/__init__.py
 src/dbally/nl_responder/nl_responder.py
 src/dbally/nl_responder/token_counters.py
 src/dbally/prompts/__init__.py
 src/dbally/prompts/prompt_builder.py
 src/dbally/similarity/__init__.py
+src/dbally/similarity/detector.py
 src/dbally/similarity/faiss_store.py
 src/dbally/similarity/fetcher.py
 src/dbally/similarity/index.py
 src/dbally/similarity/sqlalchemy_base.py
 src/dbally/similarity/store.py
 src/dbally/utils/__init__.py
 src/dbally/utils/errors.py
@@ -71,12 +71,12 @@
 src/dbally/view_selection/base.py
 src/dbally/view_selection/llm_view_selector.py
 src/dbally/view_selection/random_view_selector.py
 src/dbally/views/__init__.py
 src/dbally/views/base.py
 src/dbally/views/decorators.py
 src/dbally/views/methods_base.py
+src/dbally/views/pandas_base.py
 src/dbally/views/sqlalchemy_base.py
 src/dbally_cli/__init__.py
-src/dbally_cli/example1.py
-src/dbally_cli/example2.py
-src/dbally_cli/main.py
+src/dbally_cli/main.py
+src/dbally_cli/similarity.py
```

