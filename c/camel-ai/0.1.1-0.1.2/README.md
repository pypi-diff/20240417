# Comparing `tmp/camel_ai-0.1.1.tar.gz` & `tmp/camel_ai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camel_ai-0.1.1.tar", max compression
+gzip compressed data, was "camel_ai-0.1.2.tar", max compression
```

## Comparing `camel_ai-0.1.1.tar` & `camel_ai-0.1.2.tar`

### file list

```diff
@@ -1,75 +1,97 @@
--rw-r--r--   0        0        0    16095 2023-12-09 08:39:49.321787 camel_ai-0.1.1/README.md
--rw-r--r--   0        0        0      991 2023-12-09 08:39:49.321787 camel_ai-0.1.1/camel/__init__.py
--rw-r--r--   0        0        0     1412 2023-12-09 08:39:49.321787 camel_ai-0.1.1/camel/agents/__init__.py
--rw-r--r--   0        0        0     1130 2023-12-09 08:39:49.321787 camel_ai-0.1.1/camel/agents/base.py
--rw-r--r--   0        0        0    21214 2023-12-09 08:39:49.321787 camel_ai-0.1.1/camel/agents/chat_agent.py
--rw-r--r--   0        0        0     7303 2023-12-09 08:39:49.321787 camel_ai-0.1.1/camel/agents/critic_agent.py
--rw-r--r--   0        0        0     5847 2023-12-09 08:39:49.321787 camel_ai-0.1.1/camel/agents/embodied_agent.py
--rw-r--r--   0        0        0     4755 2023-12-09 08:39:49.321787 camel_ai-0.1.1/camel/agents/role_assignment_agent.py
--rw-r--r--   0        0        0    14785 2023-12-09 08:39:49.321787 camel_ai-0.1.1/camel/agents/task_agent.py
--rw-r--r--   0        0        0      862 2023-12-09 08:39:49.321787 camel_ai-0.1.1/camel/agents/tool_agents/__init__.py
--rw-r--r--   0        0        0     1400 2023-12-09 08:39:49.321787 camel_ai-0.1.1/camel/agents/tool_agents/base.py
--rw-r--r--   0        0        0     8691 2023-12-09 08:39:49.321787 camel_ai-0.1.1/camel/agents/tool_agents/hugging_face_tool_agent.py
--rw-r--r--   0        0        0     7440 2023-12-09 08:39:49.321787 camel_ai-0.1.1/camel/configs.py
--rw-r--r--   0        0        0      845 2023-12-09 08:39:49.321787 camel_ai-0.1.1/camel/embeddings/__init__.py
--rw-r--r--   0        0        0     2166 2023-12-09 08:39:49.321787 camel_ai-0.1.1/camel/embeddings/base.py
--rw-r--r--   0        0        0     2583 2023-12-09 08:39:49.321787 camel_ai-0.1.1/camel/embeddings/openai_embedding.py
--rw-r--r--   0        0        0     1061 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/functions/__init__.py
--rw-r--r--   0        0        0     8619 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/functions/base_io_functions.py
--rw-r--r--   0        0        0     1712 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/functions/math_functions.py
--rw-r--r--   0        0        0     3699 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/functions/openai_function.py
--rw-r--r--   0        0        0    10601 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/functions/search_functions.py
--rw-r--r--   0        0        0    23865 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/functions/unstructured_io_fuctions.py
--rw-r--r--   0        0        0     5731 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/functions/weather_functions.py
--rw-r--r--   0        0        0    10132 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/generators.py
--rw-r--r--   0        0        0     4922 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/human.py
--rw-r--r--   0        0        0     1116 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/memories/__init__.py
--rw-r--r--   0        0        0     3026 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/memories/base.py
--rw-r--r--   0        0        0     4821 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/memories/chat_history_memory.py
--rw-r--r--   0        0        0      858 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/memories/context_creators/__init__.py
--rw-r--r--   0        0        0     2743 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/memories/context_creators/base.py
--rw-r--r--   0        0        0     5065 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/memories/context_creators/score_based.py
--rw-r--r--   0        0        0     3618 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/memories/records.py
--rw-r--r--   0        0        0     1468 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/messages/__init__.py
--rw-r--r--   0        0        0     7872 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/messages/base.py
--rw-r--r--   0        0        0     3809 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/messages/func_message.py
--rw-r--r--   0        0        0     1026 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/models/__init__.py
--rw-r--r--   0        0        0     3703 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/models/base_model.py
--rw-r--r--   0        0        0     2007 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/models/model_factory.py
--rw-r--r--   0        0        0     5702 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/models/open_source_model.py
--rw-r--r--   0        0        0     3902 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/models/openai_model.py
--rw-r--r--   0        0        0     3520 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/models/stub_model.py
--rw-r--r--   0        0        0     1679 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/prompts/__init__.py
--rw-r--r--   0        0        0     6226 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/prompts/ai_society.py
--rw-r--r--   0        0        0     8272 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/prompts/base.py
--rw-r--r--   0        0        0     5784 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/prompts/code.py
--rw-r--r--   0        0        0     1556 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/prompts/evaluation.py
--rw-r--r--   0        0        0     4478 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/prompts/misalignment.py
--rw-r--r--   0        0        0     4074 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/prompts/prompt_templates.py
--rw-r--r--   0        0        0     2499 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/prompts/role_description_prompt_template.py
--rw-r--r--   0        0        0     2068 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/prompts/solution_extraction.py
--rw-r--r--   0        0        0     2197 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/prompts/task_prompt_template.py
--rw-r--r--   0        0        0     1861 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/prompts/translation.py
--rw-r--r--   0        0        0      795 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/responses/__init__.py
--rw-r--r--   0        0        0     1698 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/responses/agent_responses.py
--rw-r--r--   0        0        0      832 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/societies/__init__.py
--rw-r--r--   0        0        0    11768 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/societies/babyagi_playing.py
--rw-r--r--   0        0        0    21327 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/societies/role_playing.py
--rw-r--r--   0        0        0      973 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/storages/__init__.py
--rw-r--r--   0        0        0      916 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/storages/key_value_storages/__init__.py
--rw-r--r--   0        0        0     2192 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/storages/key_value_storages/base.py
--rw-r--r--   0        0        0     1964 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/storages/key_value_storages/in_memory.py
--rw-r--r--   0        0        0     3482 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/storages/key_value_storages/json.py
--rw-r--r--   0        0        0      997 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/terminators/__init__.py
--rw-r--r--   0        0        0     1397 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/terminators/base.py
--rw-r--r--   0        0        0     4910 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/terminators/response_terminator.py
--rw-r--r--   0        0        0     2065 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/terminators/token_limit_terminator.py
--rw-r--r--   0        0        0     1656 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/types/__init__.py
--rw-r--r--   0        0        0     5460 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/types/enums.py
--rw-r--r--   0        0        0     2045 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/types/openai_types.py
--rw-r--r--   0        0        0     1490 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/utils/__init__.py
--rw-r--r--   0        0        0     7105 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/utils/commons.py
--rw-r--r--   0        0        0    18989 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/utils/python_interpreter.py
--rw-r--r--   0        0        0     8061 2023-12-09 08:39:49.325787 camel_ai-0.1.1/camel/utils/token_counting.py
--rw-r--r--   0        0        0     3833 2023-12-09 08:39:49.337787 camel_ai-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    18492 1970-01-01 00:00:00.000000 camel_ai-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    19346 2024-04-07 07:37:05.972809 camel_ai-0.1.2/LICENSES/DATA_LICENSE
+-rw-r--r--   0        0        0    11343 2024-04-07 07:37:05.973056 camel_ai-0.1.2/LICENSES/LICENSE
+-rw-r--r--   0        0        0      707 2024-04-07 07:37:05.973183 camel_ai-0.1.2/LICENSES/license_template.txt
+-rw-r--r--   0        0        0     4457 2024-04-07 07:37:05.973322 camel_ai-0.1.2/LICENSES/update_license.py
+-rw-r--r--   0        0        0    17307 2024-04-12 16:58:57.520797 camel_ai-0.1.2/README.md
+-rw-r--r--   0        0        0      778 2024-04-07 07:37:05.937545 camel_ai-0.1.2/camel/__init__.py
+-rw-r--r--   0        0        0     1412 2024-04-07 07:37:05.937900 camel_ai-0.1.2/camel/agents/__init__.py
+-rw-r--r--   0        0        0     1130 2024-04-07 07:37:05.938155 camel_ai-0.1.2/camel/agents/base.py
+-rw-r--r--   0        0        0    21344 2024-04-12 16:35:03.023585 camel_ai-0.1.2/camel/agents/chat_agent.py
+-rw-r--r--   0        0        0     7305 2024-04-12 16:35:03.023953 camel_ai-0.1.2/camel/agents/critic_agent.py
+-rw-r--r--   0        0        0    12829 2024-04-07 07:37:05.938899 camel_ai-0.1.2/camel/agents/deductive_reasoner_agent.py
+-rw-r--r--   0        0        0     7063 2024-04-07 07:37:05.939051 camel_ai-0.1.2/camel/agents/embodied_agent.py
+-rw-r--r--   0        0        0     4755 2024-04-07 07:37:05.939458 camel_ai-0.1.2/camel/agents/role_assignment_agent.py
+-rw-r--r--   0        0        0    14785 2024-04-07 07:37:05.939733 camel_ai-0.1.2/camel/agents/task_agent.py
+-rw-r--r--   0        0        0      862 2024-04-07 07:37:05.940191 camel_ai-0.1.2/camel/agents/tool_agents/__init__.py
+-rw-r--r--   0        0        0     1400 2024-04-07 07:37:05.940552 camel_ai-0.1.2/camel/agents/tool_agents/base.py
+-rw-r--r--   0        0        0     8691 2024-04-07 07:37:05.940881 camel_ai-0.1.2/camel/agents/tool_agents/hugging_face_tool_agent.py
+-rw-r--r--   0        0        0     7562 2024-04-07 07:37:05.941107 camel_ai-0.1.2/camel/configs.py
+-rw-r--r--   0        0        0      952 2024-04-07 07:37:05.941357 camel_ai-0.1.2/camel/embeddings/__init__.py
+-rw-r--r--   0        0        0     2208 2024-04-07 07:37:05.941548 camel_ai-0.1.2/camel/embeddings/base.py
+-rw-r--r--   0        0        0     2583 2024-04-07 07:37:05.941873 camel_ai-0.1.2/camel/embeddings/openai_embedding.py
+-rw-r--r--   0        0        0     2317 2024-04-07 07:37:05.942514 camel_ai-0.1.2/camel/embeddings/sentence_transformers_embeddings.py
+-rw-r--r--   0        0        0     1245 2024-04-07 07:37:05.942814 camel_ai-0.1.2/camel/functions/__init__.py
+-rw-r--r--   0        0        0    12324 2024-04-07 07:37:05.943232 camel_ai-0.1.2/camel/functions/google_maps_function.py
+-rw-r--r--   0        0        0     1688 2024-04-07 07:37:05.943558 camel_ai-0.1.2/camel/functions/math_functions.py
+-rw-r--r--   0        0        0    14865 2024-04-07 07:37:05.943911 camel_ai-0.1.2/camel/functions/openai_function.py
+-rw-r--r--   0        0        0    12577 2024-04-12 16:35:03.024484 camel_ai-0.1.2/camel/functions/search_functions.py
+-rw-r--r--   0        0        0     5831 2024-04-07 07:37:05.944767 camel_ai-0.1.2/camel/functions/weather_functions.py
+-rw-r--r--   0        0        0    10132 2024-04-07 07:37:05.945034 camel_ai-0.1.2/camel/generators.py
+-rw-r--r--   0        0        0     4922 2024-04-07 07:37:05.945275 camel_ai-0.1.2/camel/human.py
+-rw-r--r--   0        0        0     1040 2024-04-07 07:37:05.945619 camel_ai-0.1.2/camel/interpreters/__init__.py
+-rw-r--r--   0        0        0     1904 2024-04-07 07:37:05.945843 camel_ai-0.1.2/camel/interpreters/base.py
+-rw-r--r--   0        0        0    21617 2024-04-07 07:37:05.945979 camel_ai-0.1.2/camel/interpreters/internal_python_interpreter.py
+-rw-r--r--   0        0        0      834 2024-04-07 07:37:05.946137 camel_ai-0.1.2/camel/interpreters/interpreter_error.py
+-rw-r--r--   0        0        0     6648 2024-04-07 07:37:05.946315 camel_ai-0.1.2/camel/interpreters/subprocess_interpreter.py
+-rw-r--r--   0        0        0      856 2024-04-07 07:37:05.946593 camel_ai-0.1.2/camel/loaders/__init__.py
+-rw-r--r--   0        0        0     8651 2024-04-07 07:37:05.946766 camel_ai-0.1.2/camel/loaders/base_io.py
+-rw-r--r--   0        0        0    23647 2024-04-07 07:37:05.947167 camel_ai-0.1.2/camel/loaders/unstructured_io.py
+-rw-r--r--   0        0        0     1364 2024-04-12 16:35:03.024866 camel_ai-0.1.2/camel/memories/__init__.py
+-rw-r--r--   0        0        0     6070 2024-04-12 16:35:03.025033 camel_ai-0.1.2/camel/memories/agent_memories.py
+-rw-r--r--   0        0        0     4995 2024-04-12 16:35:03.025402 camel_ai-0.1.2/camel/memories/base.py
+-rw-r--r--   0        0        0      860 2024-04-12 16:35:03.025747 camel_ai-0.1.2/camel/memories/blocks/__init__.py
+-rw-r--r--   0        0        0     4570 2024-04-12 16:35:03.081821 camel_ai-0.1.2/camel/memories/blocks/chat_history_block.py
+-rw-r--r--   0        0        0     3775 2024-04-12 16:35:03.026520 camel_ai-0.1.2/camel/memories/blocks/vectordb_block.py
+-rw-r--r--   0        0        0      806 2024-04-12 16:35:03.027014 camel_ai-0.1.2/camel/memories/context_creators/__init__.py
+-rw-r--r--   0        0        0     5292 2024-04-12 16:35:03.027292 camel_ai-0.1.2/camel/memories/context_creators/score_based.py
+-rw-r--r--   0        0        0     3613 2024-04-12 16:35:03.027735 camel_ai-0.1.2/camel/memories/records.py
+-rw-r--r--   0        0        0     1468 2024-04-07 07:37:05.949444 camel_ai-0.1.2/camel/messages/__init__.py
+-rw-r--r--   0        0        0     7872 2024-04-07 07:37:05.949594 camel_ai-0.1.2/camel/messages/base.py
+-rw-r--r--   0        0        0     3813 2024-04-07 07:37:05.949788 camel_ai-0.1.2/camel/messages/func_message.py
+-rw-r--r--   0        0        0     1026 2024-04-07 07:37:05.950038 camel_ai-0.1.2/camel/models/__init__.py
+-rw-r--r--   0        0        0     3703 2024-04-07 07:37:05.950211 camel_ai-0.1.2/camel/models/base_model.py
+-rw-r--r--   0        0        0     2007 2024-04-07 07:37:05.950401 camel_ai-0.1.2/camel/models/model_factory.py
+-rw-r--r--   0        0        0     5734 2024-04-07 07:37:05.950575 camel_ai-0.1.2/camel/models/open_source_model.py
+-rw-r--r--   0        0        0     3902 2024-04-07 07:37:05.950734 camel_ai-0.1.2/camel/models/openai_model.py
+-rw-r--r--   0        0        0     3555 2024-04-07 07:37:05.950879 camel_ai-0.1.2/camel/models/stub_model.py
+-rw-r--r--   0        0        0     1679 2024-04-07 07:37:05.951177 camel_ai-0.1.2/camel/prompts/__init__.py
+-rw-r--r--   0        0        0     6226 2024-04-07 07:37:05.951347 camel_ai-0.1.2/camel/prompts/ai_society.py
+-rw-r--r--   0        0        0     8385 2024-04-07 07:37:05.951499 camel_ai-0.1.2/camel/prompts/base.py
+-rw-r--r--   0        0        0     5784 2024-04-07 07:37:05.951643 camel_ai-0.1.2/camel/prompts/code.py
+-rw-r--r--   0        0        0     1556 2024-04-07 07:37:05.951860 camel_ai-0.1.2/camel/prompts/evaluation.py
+-rw-r--r--   0        0        0     4478 2024-04-07 07:37:05.952001 camel_ai-0.1.2/camel/prompts/misalignment.py
+-rw-r--r--   0        0        0     4074 2024-04-07 07:37:05.952135 camel_ai-0.1.2/camel/prompts/prompt_templates.py
+-rw-r--r--   0        0        0     2499 2024-04-07 07:37:05.952288 camel_ai-0.1.2/camel/prompts/role_description_prompt_template.py
+-rw-r--r--   0        0        0     2068 2024-04-07 07:37:05.952430 camel_ai-0.1.2/camel/prompts/solution_extraction.py
+-rw-r--r--   0        0        0     2197 2024-04-07 07:37:05.952554 camel_ai-0.1.2/camel/prompts/task_prompt_template.py
+-rw-r--r--   0        0        0     1861 2024-04-07 07:37:05.952674 camel_ai-0.1.2/camel/prompts/translation.py
+-rw-r--r--   0        0        0      795 2024-04-07 07:37:05.952868 camel_ai-0.1.2/camel/responses/__init__.py
+-rw-r--r--   0        0        0     1698 2024-04-07 07:37:05.953066 camel_ai-0.1.2/camel/responses/agent_responses.py
+-rw-r--r--   0        0        0      908 2024-04-12 16:56:43.847428 camel_ai-0.1.2/camel/retrievers/__init__.py
+-rw-r--r--   0        0        0    12000 2024-04-07 07:37:05.953434 camel_ai-0.1.2/camel/retrievers/auto_retriever.py
+-rw-r--r--   0        0        0     2123 2024-04-12 16:56:43.848583 camel_ai-0.1.2/camel/retrievers/base.py
+-rw-r--r--   0        0        0     6432 2024-04-12 16:56:43.849751 camel_ai-0.1.2/camel/retrievers/vector_retriever.py
+-rw-r--r--   0        0        0      832 2024-04-07 07:37:05.953929 camel_ai-0.1.2/camel/societies/__init__.py
+-rw-r--r--   0        0        0    11768 2024-04-07 07:37:05.954127 camel_ai-0.1.2/camel/societies/babyagi_playing.py
+-rw-r--r--   0        0        0    21824 2024-04-07 07:37:05.954453 camel_ai-0.1.2/camel/societies/role_playing.py
+-rw-r--r--   0        0        0     1337 2024-04-07 07:37:05.954699 camel_ai-0.1.2/camel/storages/__init__.py
+-rw-r--r--   0        0        0      916 2024-04-07 07:37:05.954924 camel_ai-0.1.2/camel/storages/key_value_storages/__init__.py
+-rw-r--r--   0        0        0     2192 2024-04-07 07:37:05.955045 camel_ai-0.1.2/camel/storages/key_value_storages/base.py
+-rw-r--r--   0        0        0     1964 2024-04-07 07:37:05.955165 camel_ai-0.1.2/camel/storages/key_value_storages/in_memory.py
+-rw-r--r--   0        0        0     3399 2024-04-07 07:37:05.955273 camel_ai-0.1.2/camel/storages/key_value_storages/json.py
+-rw-r--r--   0        0        0     1076 2024-04-07 07:37:05.955446 camel_ai-0.1.2/camel/storages/vectordb_storages/__init__.py
+-rw-r--r--   0        0        0     5985 2024-04-07 07:37:05.955680 camel_ai-0.1.2/camel/storages/vectordb_storages/base.py
+-rw-r--r--   0        0        0    13426 2024-04-07 07:37:05.955907 camel_ai-0.1.2/camel/storages/vectordb_storages/milvus.py
+-rw-r--r--   0        0        0    13452 2024-04-07 07:37:05.956121 camel_ai-0.1.2/camel/storages/vectordb_storages/qdrant.py
+-rw-r--r--   0        0        0      997 2024-04-07 07:37:05.956356 camel_ai-0.1.2/camel/terminators/__init__.py
+-rw-r--r--   0        0        0     1397 2024-04-07 07:37:05.956514 camel_ai-0.1.2/camel/terminators/base.py
+-rw-r--r--   0        0        0     4910 2024-04-07 07:37:05.956631 camel_ai-0.1.2/camel/terminators/response_terminator.py
+-rw-r--r--   0        0        0     2065 2024-04-07 07:37:05.956756 camel_ai-0.1.2/camel/terminators/token_limit_terminator.py
+-rw-r--r--   0        0        0     1692 2024-04-07 07:37:05.956946 camel_ai-0.1.2/camel/types/__init__.py
+-rw-r--r--   0        0        0     5834 2024-04-07 07:37:05.957209 camel_ai-0.1.2/camel/types/enums.py
+-rw-r--r--   0        0        0     2045 2024-04-07 07:37:05.957332 camel_ai-0.1.2/camel/types/openai_types.py
+-rw-r--r--   0        0        0     1536 2024-04-07 07:37:05.957547 camel_ai-0.1.2/camel/utils/__init__.py
+-rw-r--r--   0        0        0    12366 2024-04-12 16:56:43.850856 camel_ai-0.1.2/camel/utils/commons.py
+-rw-r--r--   0        0        0     8061 2024-04-07 07:37:05.957963 camel_ai-0.1.2/camel/utils/token_counting.py
+-rw-r--r--   0        0        0     4607 2024-04-12 16:57:29.543796 camel_ai-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    20256 1970-01-01 00:00:00.000000 camel_ai-0.1.2/PKG-INFO
```

### Comparing `camel_ai-0.1.1/camel/__init__.py` & `camel_ai-0.1.2/camel/societies/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,24 +7,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
-import camel.agents
-import camel.configs
-import camel.generators
-import camel.messages
-import camel.prompts
-import camel.types
-import camel.utils
-import camel.functions
-import camel.memories
-import camel.storages
-
-__version__ = '0.1.1'
+from .role_playing import RolePlaying
+from .babyagi_playing import BabyAGI
 
 __all__ = [
-    '__version__',
-    'camel',
+    'RolePlaying',
+    'BabyAGI',
 ]
```

### Comparing `camel_ai-0.1.1/camel/agents/__init__.py` & `camel_ai-0.1.2/camel/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/agents/base.py` & `camel_ai-0.1.2/camel/agents/base.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/agents/chat_agent.py` & `camel_ai-0.1.2/camel/agents/chat_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,43 +7,48 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
+from __future__ import annotations
+
 import json
 from collections import defaultdict
 from dataclasses import dataclass
-from typing import Any, Callable, Dict, List, Optional, Tuple
-
-from openai import Stream
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple
 
 from camel.agents import BaseAgent
-from camel.configs import BaseConfig, ChatGPTConfig
-from camel.functions import OpenAIFunction
+from camel.configs import ChatGPTConfig
 from camel.memories import (
-    BaseMemory,
+    AgentMemory,
     ChatHistoryMemory,
     MemoryRecord,
     ScoreBasedContextCreator,
 )
 from camel.messages import BaseMessage, FunctionCallingMessage, OpenAIMessage
 from camel.models import BaseModelBackend, ModelFactory
 from camel.responses import ChatAgentResponse
-from camel.terminators import ResponseTerminator
 from camel.types import (
     ChatCompletion,
     ChatCompletionChunk,
     ModelType,
     OpenAIBackendRole,
     RoleType,
 )
 from camel.utils import get_model_encoding
 
+if TYPE_CHECKING:
+    from openai import Stream
+
+    from camel.configs import BaseConfig
+    from camel.functions import OpenAIFunction
+    from camel.terminators import ResponseTerminator
+
 
 @dataclass(frozen=True)
 class FunctionCallingRecord:
     r"""Historical records of functions called in the conversation.
 
     Attributes:
         func_name (str): The name of the function being called.
@@ -72,21 +77,21 @@
 
     Args:
         system_message (BaseMessage): The system message for the chat agent.
         model_type (ModelType, optional): The LLM model to use for generating
             responses. (default :obj:`ModelType.GPT_3_5_TURBO`)
         model_config (BaseConfig, optional): Configuration options for the
             LLM model. (default: :obj:`None`)
-        memory (BaseMemory, optional): The agent memory for managing chat
+        memory (AgentMemory, optional): The agent memory for managing chat
             messages. If `None`, a :obj:`ChatHistoryMemory` will be used.
             (default: :obj:`None`)
         message_window_size (int, optional): The maximum number of previous
             messages to include in the context window. If `None`, no windowing
             is performed. (default: :obj:`None`)
-        token_limit (int, optional): The maxinum number of tokens in a context.
+        token_limit (int, optional): The maximum number of tokens in a context.
             The context will be automatically pruned to fulfill the limitation.
             If `None`, it will be set according to the backend model.
             (default: :obj:`None`)
         output_language (str, optional): The language to be output by the
             agent. (default: :obj:`None`)
         function_list (List[OpenAIFunction], optional): List of available
             :obj:`OpenAIFunction`. (default: :obj:`None`)
@@ -96,15 +101,15 @@
     """
 
     def __init__(
         self,
         system_message: BaseMessage,
         model_type: Optional[ModelType] = None,
         model_config: Optional[BaseConfig] = None,
-        memory: Optional[BaseMemory] = None,
+        memory: Optional[AgentMemory] = None,
         message_window_size: Optional[int] = None,
         token_limit: Optional[int] = None,
         output_language: Optional[str] = None,
         function_list: Optional[List[OpenAIFunction]] = None,
         response_terminators: Optional[List[ResponseTerminator]] = None,
     ) -> None:
 
@@ -118,25 +123,25 @@
 
         self.model_type: ModelType = (model_type if model_type is not None else
                                       ModelType.GPT_3_5_TURBO)
 
         self.func_dict: Dict[str, Callable] = {}
         if function_list is not None:
             for func in function_list:
-                self.func_dict[func.name] = func.func
+                self.func_dict[func.get_function_name()] = func.func
         self.model_config = model_config or ChatGPTConfig()
 
         self.model_backend: BaseModelBackend = ModelFactory.create(
             self.model_type, self.model_config.__dict__)
         self.model_token_limit = token_limit or self.model_backend.token_limit
         context_creator = ScoreBasedContextCreator(
             self.model_backend.token_counter,
             self.model_token_limit,
         )
-        self.memory: BaseMemory = memory or ChatHistoryMemory(
+        self.memory: AgentMemory = memory or ChatHistoryMemory(
             context_creator, window_size=message_window_size)
 
         self.terminated: bool = False
         self.response_terminators = response_terminators or []
         self.init_messages()
 
     def reset(self):
```

### Comparing `camel_ai-0.1.1/camel/agents/critic_agent.py` & `camel_ai-0.1.2/camel/agents/critic_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import random
 import warnings
 from typing import Any, Dict, Optional, Sequence
 
 from colorama import Fore
 
 from camel.agents import ChatAgent
-from camel.memories import BaseMemory
+from camel.memories import AgentMemory
 from camel.messages import BaseMessage
 from camel.responses import ChatAgentResponse
 from camel.types import ModelType
 from camel.utils import get_first_int, print_text_animated
 
 
 class CriticAgent(ChatAgent):
@@ -46,15 +46,15 @@
     """
 
     def __init__(
         self,
         system_message: BaseMessage,
         model_type: ModelType = ModelType.GPT_3_5_TURBO,
         model_config: Optional[Any] = None,
-        memory: Optional[BaseMemory] = None,
+        memory: Optional[AgentMemory] = None,
         message_window_size: int = 6,
         retry_attempts: int = 2,
         verbose: bool = False,
         logger_color: Any = Fore.MAGENTA,
     ) -> None:
         super().__init__(system_message, model_type=model_type,
                          model_config=model_config, memory=memory,
```

### Comparing `camel_ai-0.1.1/camel/agents/embodied_agent.py` & `camel_ai-0.1.2/camel/agents/embodied_agent.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,81 +7,120 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
-from typing import Any, Dict, List, Optional
+from typing import Any, List, Optional
 
 from colorama import Fore
 
-from camel.agents import BaseToolAgent, ChatAgent, HuggingFaceToolAgent
+from camel.agents import BaseToolAgent, ChatAgent
+from camel.interpreters import (
+    BaseInterpreter,
+    InternalPythonInterpreter,
+    SubprocessInterpreter,
+)
 from camel.messages import BaseMessage
 from camel.responses import ChatAgentResponse
 from camel.types import ModelType
-from camel.utils import PythonInterpreter, print_text_animated
+from camel.utils import print_text_animated
 
 
 class EmbodiedAgent(ChatAgent):
     r"""Class for managing conversations of CAMEL Embodied Agents.
 
     Args:
         system_message (BaseMessage): The system message for the chat agent.
         model_type (ModelType, optional): The LLM model to use for generating
             responses. (default :obj:`ModelType.GPT_4`)
         model_config (Any, optional): Configuration options for the LLM model.
             (default: :obj:`None`)
         message_window_size (int, optional): The maximum number of previous
             messages to include in the context window. If `None`, no windowing
             is performed. (default: :obj:`None`)
-        action_space (List[Any], optional): The action space for the embodied
-            agent. (default: :obj:`None`)
+        tool_agents (List[BaseToolAgent], optional): The tools agents to use in
+            the embodied agent. (default: :obj:`None`)
+        code_interpreter (BaseInterpreter, optional): The code interpreter to
+            execute codes. If `code_interpreter` and `tool_agent` are both
+            `None`, default to `SubProcessInterpreter`. If `code_interpreter`
+            is `None` and `tool_agents` is not `None`, default to
+            `InternalPythonInterpreter`.  (default: :obj:`None`)
         verbose (bool, optional): Whether to print the critic's messages.
         logger_color (Any): The color of the logger displayed to the user.
             (default: :obj:`Fore.MAGENTA`)
     """
 
     def __init__(
         self,
         system_message: BaseMessage,
         model_type: ModelType = ModelType.GPT_4,
         model_config: Optional[Any] = None,
         message_window_size: Optional[int] = None,
-        action_space: Optional[List[BaseToolAgent]] = None,
+        tool_agents: Optional[List[BaseToolAgent]] = None,
+        code_interpreter: Optional[BaseInterpreter] = None,
         verbose: bool = False,
         logger_color: Any = Fore.MAGENTA,
     ) -> None:
-        default_action_space = [
-            HuggingFaceToolAgent('hugging_face_tool_agent',
-                                 model_type=model_type.value),
-        ]
-        self.action_space = action_space or default_action_space
-        action_space_prompt = self.get_action_space_prompt()
-        system_message.content = system_message.content.format(
-            action_space=action_space_prompt)
+        self.tool_agents = tool_agents
+        self.code_interpreter: BaseInterpreter
+        if code_interpreter is not None:
+            self.code_interpreter = code_interpreter
+        elif self.tool_agents:
+            self.code_interpreter = InternalPythonInterpreter()
+        else:
+            self.code_interpreter = SubprocessInterpreter()
+
+        if self.tool_agents:
+            system_message = self._set_tool_agents(system_message)
         self.verbose = verbose
         self.logger_color = logger_color
         super().__init__(
             system_message=system_message,
             model_type=model_type,
             model_config=model_config,
             message_window_size=message_window_size,
         )
 
-    def get_action_space_prompt(self) -> str:
+    def _set_tool_agents(self, system_message: BaseMessage) -> BaseMessage:
+        action_space_prompt = self._get_tool_agents_prompt()
+        result_message = system_message.create_new_instance(
+            content=system_message.content.format(
+                action_space=action_space_prompt))
+        if self.tool_agents is not None:
+            self.code_interpreter.update_action_space(
+                {tool.name: tool
+                 for tool in self.tool_agents})
+        return result_message
+
+    def _get_tool_agents_prompt(self) -> str:
         r"""Returns the action space prompt.
 
         Returns:
             str: The action space prompt.
         """
-        return "\n".join([
-            f"*** {action.name} ***:\n {action.description}"
-            for action in self.action_space
-        ])
+        if self.tool_agents is not None:
+            return "\n".join([
+                f"*** {tool.name} ***:\n {tool.description}"
+                for tool in self.tool_agents
+            ])
+        else:
+            return ""
+
+    def get_tool_agent_names(self) -> List[str]:
+        r"""Returns the names of tool agents.
+
+        Returns:
+            List[str]: The names of tool agents.
+        """
+        if self.tool_agents is not None:
+            return [tool.name for tool in self.tool_agents]
+        else:
+            return []
 
     def step(
         self,
         input_message: BaseMessage,
     ) -> ChatAgentResponse:
         r"""Performs a step in the conversation.
 
@@ -107,32 +146,28 @@
             for explanation, code in zip(explanations, codes):
                 print_text_animated(self.logger_color +
                                     f"> Explanation:\n{explanation}")
                 print_text_animated(self.logger_color + f"> Code:\n{code}")
 
             if len(explanations) > len(codes):
                 print_text_animated(self.logger_color +
-                                    f"> Explanation:\n{explanations}")
+                                    f"> Explanation:\n{explanations[-1]}")
 
         content = response.msg.content
 
         if codes is not None:
-            content = "\n> Executed Results:"
-            action_space: Dict[str, Any] = {
-                action.name: action
-                for action in self.action_space
-            }
-            action_space.update({"print": print, "enumerate": enumerate})
-            interpreter = PythonInterpreter(action_space=action_space)
-            for block_idx, code in enumerate(codes):
-                executed_outputs, _ = code.execute(interpreter)
-                content += (f"Executing code block {block_idx}:\n"
-                            f"  - execution output:\n{executed_outputs}\n"
-                            f"  - Local variables:\n{interpreter.state}\n")
-                content += "*" * 50 + "\n"
+            try:
+                content = "\n> Executed Results:\n"
+                for block_idx, code in enumerate(codes):
+                    executed_output = self.code_interpreter.run(
+                        code, code.code_type)
+                    content += (f"Executing code block {block_idx}: {{\n" +
+                                executed_output + "}\n")
+            except InterruptedError as e:
+                content = (f"\n> Running code fail: {e}\n"
+                           "Please regenerate the code.")
 
         # TODO: Handle errors
-        content = input_message.content + (Fore.RESET +
-                                           f"\n> Embodied Actions:\n{content}")
+        content = input_message.content + f"\n> Embodied Actions:\n{content}"
         message = BaseMessage(input_message.role_name, input_message.role_type,
                               input_message.meta_dict, content)
         return ChatAgentResponse([message], response.terminated, response.info)
```

### Comparing `camel_ai-0.1.1/camel/agents/role_assignment_agent.py` & `camel_ai-0.1.2/camel/agents/role_assignment_agent.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/agents/task_agent.py` & `camel_ai-0.1.2/camel/agents/task_agent.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/agents/tool_agents/__init__.py` & `camel_ai-0.1.2/camel/agents/tool_agents/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/agents/tool_agents/base.py` & `camel_ai-0.1.2/camel/agents/tool_agents/base.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/agents/tool_agents/hugging_face_tool_agent.py` & `camel_ai-0.1.2/camel/agents/tool_agents/hugging_face_tool_agent.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/configs.py` & `camel_ai-0.1.2/camel/configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
+from __future__ import annotations
+
 from abc import ABC
 from dataclasses import asdict, dataclass, field
-from typing import Any, Dict, List, Optional, Sequence, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Sequence, Union
 
-from camel.functions import OpenAIFunction
+if TYPE_CHECKING:
+    from camel.functions import OpenAIFunction
 
 
 @dataclass(frozen=True)
 class BaseConfig(ABC):
     pass
 
 
@@ -124,15 +127,17 @@
 
         Return:
             FunctionCallingConfig: A new instance which loads the given
                 function list into a list of dictionaries and the input
                 :obj:`function_call` argument.
         """
         return cls(
-            functions=[func.as_dict() for func in function_list],
+            functions=[
+                func.get_openai_function_schema() for func in function_list
+            ],
             function_call=function_call,
             **(kwargs or {}),
         )
 
 
 @dataclass(frozen=True)
 class OpenSourceConfig(BaseConfig):
```

### Comparing `camel_ai-0.1.1/camel/embeddings/__init__.py` & `camel_ai-0.1.2/camel/memories/context_creators/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,14 +7,13 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
-from .base import BaseEmbedding
-from .openai_embedding import OpenAIEmbedding
+
+from .score_based import ScoreBasedContextCreator
 
 __all__ = [
-    "BaseEmbedding",
-    "OpenAIEmbedding",
+    'ScoreBasedContextCreator',
 ]
```

### Comparing `camel_ai-0.1.1/camel/embeddings/base.py` & `camel_ai-0.1.2/camel/embeddings/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,16 +29,17 @@
         r"""Generates embeddings for the given texts.
 
         Args:
             objs (List[T]): The objects for which to generate the embeddings.
             **kwargs (Any): Extra kwargs passed to the embedding API.
 
         Returns:
-            List[List[float]]: A list that represents the generated embedding
-                as a list of floating-point numbers.
+            List[List[float]]: A list that represents the
+            generated embedding as a list of floating-point numbers or a
+            numpy matrix with embeddings.
         """
         pass
 
     def embed(
         self,
         obj: T,
         **kwargs: Any,
```

### Comparing `camel_ai-0.1.1/camel/embeddings/openai_embedding.py` & `camel_ai-0.1.2/camel/embeddings/openai_embedding.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/functions/__init__.py` & `camel_ai-0.1.2/camel/storages/key_value_storages/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,20 +8,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
 
-from .math_functions import MATH_FUNCS
-from .openai_function import OpenAIFunction
-from .search_functions import SEARCH_FUNCS
-from .weather_functions import WEATHER_FUNCS
-from .unstructured_io_fuctions import UnstructuredModules
+from .base import BaseKeyValueStorage
+from .in_memory import InMemoryKeyValueStorage
+from .json import JsonStorage
 
 __all__ = [
-    'OpenAIFunction',
-    'MATH_FUNCS',
-    'SEARCH_FUNCS',
-    'WEATHER_FUNCS',
-    'UnstructuredModules',
+    'BaseKeyValueStorage',
+    'InMemoryKeyValueStorage',
+    'JsonStorage',
 ]
```

### Comparing `camel_ai-0.1.1/camel/functions/base_io_functions.py` & `camel_ai-0.1.2/camel/loaders/base_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,32 +31,32 @@
         docs: Optional[List[Dict[str, Any]]] = None,
     ):
         r"""
 
         Args:
             name (str): The name of the file.
             id (str): The unique identifier of the file.
-            metadata (Dict[str, Any], optional):
-            Additional metadata associated with the file. Defaults to None.
-            docs (List[Dict[str, Any]], optional):
-            A list of documents contained within the file. Defaults to None.
+            metadata (Dict[str, Any], optional): Additional metadata
+                associated with the file. Defaults to None.
+            docs (List[Dict[str, Any]], optional): A list of documents
+                contained within the file. Defaults to None.
         """
         self.name = name
         self.id = id
         self.metadata = metadata or {}
         self.docs = docs or []
 
     @classmethod
     @abstractmethod
     def from_bytes(cls, file: BytesIO) -> "File":
         r"""Creates a File object from a BytesIO object.
 
         Args:
-            file (BytesIO):
-            A BytesIO object representing the contents of the file.
+            file (BytesIO): A BytesIO object representing the contents of the
+                file.
 
         Returns:
             File: A File object.
         """
 
     def __repr__(self) -> str:
         return (f"File(name={self.name}, id={self.id}, "
@@ -92,16 +92,16 @@
 class DocxFile(File):
 
     @classmethod
     def from_bytes(cls, file: BytesIO) -> "DocxFile":
         r"""Creates a DocxFile object from a BytesIO object.
 
         Args:
-            file (BytesIO):
-            A BytesIO object representing the contents of the docx file.
+            file (BytesIO): A BytesIO object representing the contents of the
+                docx file.
 
         Returns:
             DocxFile: A DocxFile object.
         """
         # Use docx2txt to extract text from docx files
         try:
             import docx2txt
@@ -123,16 +123,16 @@
 class PdfFile(File):
 
     @classmethod
     def from_bytes(cls, file: BytesIO) -> "PdfFile":
         r"""Creates a PdfFile object from a BytesIO object.
 
         Args:
-            file (BytesIO):
-            A BytesIO object representing the contents of the pdf file.
+            file (BytesIO): A BytesIO object representing the contents of the
+                pdf file.
 
         Returns:
             PdfFile: A PdfFile object.
         """
         # Use fitz to extract text from pdf files
         try:
             import fitz
@@ -158,16 +158,16 @@
 class TxtFile(File):
 
     @classmethod
     def from_bytes(cls, file: BytesIO) -> "TxtFile":
         r"""Creates a TxtFile object from a BytesIO object.
 
         Args:
-            file (BytesIO):
-            A BytesIO object representing the contents of the txt file.
+            file (BytesIO): A BytesIO object representing the contents of the
+                txt file.
 
         Returns:
             TxtFile: A TxtFile object.
         """
         # Read the text from the file
         text = file.read().decode("utf-8")
         text = strip_consecutive_newlines(text)
@@ -183,16 +183,16 @@
 class JsonFile(File):
 
     @classmethod
     def from_bytes(cls, file: BytesIO) -> "JsonFile":
         r"""Creates a JsonFile object from a BytesIO object.
 
         Args:
-            file (BytesIO):
-            A BytesIO object representing the contents of the json file.
+            file (BytesIO): A BytesIO object representing the contents of the
+                json file.
 
         Returns:
             JsonFile: A JsonFile object.
         """
         # Parse the JSON data from the file
         data = json.load(file)
         # Create a dictionary with the parsed data
@@ -207,16 +207,16 @@
 class HtmlFile(File):
 
     @classmethod
     def from_bytes(cls, file: BytesIO) -> "HtmlFile":
         r"""Creates a HtmlFile object from a BytesIO object.
 
         Args:
-            file (BytesIO):
-            A BytesIO object representing the contents of the html file.
+            file (BytesIO): A BytesIO object representing the contents of the
+                html file.
 
         Returns:
             HtmlFile: A HtmlFile object.
         """
         # Parse the HTML data from the file
         try:
             from bs4 import BeautifulSoup
```

### Comparing `camel_ai-0.1.1/camel/functions/math_functions.py` & `camel_ai-0.1.2/camel/functions/math_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,42 +17,42 @@
 from .openai_function import OpenAIFunction
 
 
 def add(a: int, b: int) -> int:
     r"""Adds two numbers.
 
     Args:
-        a (integer): The first number to be added.
-        b (integer): The second number to be added.
+        a (int): The first number to be added.
+        b (int): The second number to be added.
 
     Returns:
         integer: The sum of the two numbers.
     """
     return a + b
 
 
 def sub(a: int, b: int) -> int:
     r"""Do subtraction between two numbers.
 
     Args:
-        a (integer): The minuend in subtraction.
-        b (integer): The subtrahend in subtraction.
+        a (int): The minuend in subtraction.
+        b (int): The subtrahend in subtraction.
 
     Returns:
         integer: The result of subtracting :obj:`b` from :obj:`a`.
     """
     return a - b
 
 
 def mul(a: int, b: int) -> int:
     r"""Multiplies two integers.
 
     Args:
-        a (integer): The multiplier in the multiplication.
-        b (integer): The multiplicand in the multiplication.
+        a (int): The multiplier in the multiplication.
+        b (int): The multiplicand in the multiplication.
 
     Returns:
         integer: The product of the two numbers.
     """
     return a * b
```

### Comparing `camel_ai-0.1.1/camel/functions/search_functions.py` & `camel_ai-0.1.2/camel/functions/search_functions.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,29 +10,29 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
 import os
 from typing import Any, Dict, List
 
-import camel.agents
+from camel.agents import ChatAgent
 from camel.functions import OpenAIFunction
 from camel.messages import BaseMessage
 from camel.prompts import TextPrompt
 
 
 def search_wiki(entity: str) -> str:
     r"""Search the entity in WikiPedia and return the summary of the
     required page, containing factual information about the given entity.
 
     Args:
-        entity (string): The entity to be searched.
+        entity (str): The entity to be searched.
 
     Returns:
-        string: The search result. If the page corresponding to the entity
+        str: The search result. If the page corresponding to the entity
             exists, return the summary of this entity in a string.
     """
     try:
         import wikipedia
     except ImportError:
         raise ImportError(
             "Please install `wikipedia` first. You can install it by running "
@@ -55,15 +55,15 @@
     return result
 
 
 def search_google(query: str) -> List[Dict[str, Any]]:
     r"""Use Google search engine to search information for the given query.
 
     Args:
-        query (string): The query to be searched.
+        query (str): The query to be searched.
 
     Returns:
         List[Dict[str, Any]]: A list of dictionaries where each dictionary
         represents a website.
             Each dictionary contains the following keys:
             - 'result_id': A number in order.
             - 'title': The title of the website.
@@ -79,15 +79,15 @@
                 artificial general intelligence benefits all of humanity.',
                 'long_description': 'OpenAI is a non-profit artificial
                  intelligence research company. Our goal is to advance digital
                 intelligence in the way that is most likely to benefit humanity
                 as a whole',
                 'url': 'https://www.openai.com'
             }
-        title, descrption, url of a website.
+        title, description, url of a website.
     """
     import requests
 
     # https://developers.google.com/custom-search/v1/overview
     GOOGLE_API_KEY = os.getenv("GOOGLE_API_KEY")
     # https://cse.google.com/cse/all
     SEARCH_ENGINE_ID = os.getenv("SEARCH_ENGINE_ID")
@@ -146,18 +146,18 @@
     return responses
 
 
 def text_extract_from_web(url: str) -> str:
     r"""Get the text information from given url.
 
     Args:
-        url (string): The web site you want to search.
+        url (str): The website you want to search.
 
     Returns:
-        string: All texts extract from the web.
+        str: All texts extract from the web.
     """
     import requests
     from bs4 import BeautifulSoup
 
     try:
         # Request the target page
         response_text = requests.get(url).text
@@ -182,19 +182,19 @@
 
 
 # Split a text into smaller chunks of size n
 def create_chunks(text: str, n: int) -> List[str]:
     r"""Returns successive n-sized chunks from provided text."
 
     Args:
-        text (string): The text to be split.
+        text (str): The text to be split.
         n (int): The max length of a single chunk.
 
     Returns:
-        List[str]: A list of splited texts.
+        List[str]: A list of split texts.
     """
 
     chunks = []
     i = 0
     while i < len(text):
         # Find the nearest end of sentence within a range of 0.5 * n
         # and 1.5 * n tokens
@@ -216,15 +216,15 @@
 def prompt_single_step_agent(prompt: str) -> str:
     """Prompt a single-step agent to summarize texts or answer a question."""
 
     assistant_sys_msg = BaseMessage.make_assistant_message(
         role_name="Assistant",
         content="You are a helpful assistant.",
     )
-    agent = camel.agents.ChatAgent(assistant_sys_msg)
+    agent = ChatAgent(assistant_sys_msg)
     agent.reset()
 
     user_msg = BaseMessage.make_user_message(
         role_name="User",
         content=prompt,
     )
     assistant_response = agent.step(user_msg)
@@ -234,19 +234,19 @@
 
 
 def summarize_text(text: str, query: str) -> str:
     r"""Summarize the information from the text, base on the query if query is
     given.
 
     Args:
-        text (string): Text to summarise.
-        query (string): What information you want.
+        text (str): Text to summarize.
+        query (str): What information you want.
 
     Returns:
-        string: Strings with information.
+        str: Strings with information.
     """
     summary_prompt = TextPrompt(
         '''Gather information from this text that relative to the question, but
          do not directly answer the question.\nquestion: {query}\ntext ''')
     summary_prompt = summary_prompt.format(query=query)
     # Max length of each chunk
     max_len = 3000
@@ -272,18 +272,18 @@
 
 def search_google_and_summarize(query: str) -> str:
     r"""Search webs for information. Given a query, this function will use
     the Google search engine to search for related information from the
     internet, and then return a summarized answer.
 
     Args:
-        query (string): Question you want to be answered.
+        query (str): Question you want to be answered.
 
     Returns:
-        string: Summarized information from webs.
+        str: Summarized information from webs.
     """
     # Google search will return a list of urls
     responses = search_google(query)
     for item in responses:
         if "url" in item:
             url = item.get("url")
             # Extract text
@@ -299,11 +299,64 @@
             reply = prompt_single_step_agent(prompt)
             if "yes" in str(reply).lower():
                 return answer
 
     return "Failed to find the answer from google search."
 
 
+def search_wolfram_alpha(query: str, is_detailed: bool) -> str:
+    r"""Queries Wolfram|Alpha and returns the result. Wolfram|Alpha is a
+    search engine that uses algorithms, knowledgebase and AI to compute
+    expert-level answers for math, science, society, everyday life and more.
+
+    Args:
+        query (str): The query to send to Wolfram Alpha.
+        is_detailed (bool): Whether to include additional details in the
+            result.
+
+    Returns:
+        str: The result from Wolfram Alpha, formatted as a string.
+    """
+    try:
+        import wolframalpha
+    except ImportError:
+        raise ImportError(
+            "Please install `wolframalpha` first. You can install it by "
+            "running `pip install wolframalpha`.")
+
+    WOLFRAMALPHA_APP_ID = os.environ.get('WOLFRAMALPHA_APP_ID')
+    if not WOLFRAMALPHA_APP_ID:
+        raise ValueError("`WOLFRAMALPHA_APP_ID` not found in environment "
+                         "variables. Get `WOLFRAMALPHA_APP_ID` here: "
+                         "`https://products.wolframalpha.com/api/`.")
+
+    try:
+        client = wolframalpha.Client(WOLFRAMALPHA_APP_ID)
+        res = client.query(query)
+        assumption = next(res.pods).text or "No assumption made."
+        answer = next(res.results).text or "No answer found."
+    except Exception as e:
+        if isinstance(e, StopIteration):
+            return "Wolfram Alpha wasn't able to answer it"
+        else:
+            error_message = (f"Wolfram Alpha wasn't able to answer it"
+                             f"{str(e)}.")
+            return error_message
+
+    result = f"Assumption:\n{assumption}\n\nAnswer:\n{answer}"
+
+    # Add additional details in the result
+    if is_detailed:
+        result += '\n'
+        for pod in res.pods:
+            result += '\n' + pod['@title'] + ':\n'
+            for sub in pod.subpods:
+                result += (sub.plaintext or "None") + '\n'
+
+    return result.rstrip()  # Remove trailing whitespace
+
+
 SEARCH_FUNCS: List[OpenAIFunction] = [
-    OpenAIFunction(func)
-    for func in [search_wiki, search_google_and_summarize]
+    OpenAIFunction(func)  # type: ignore
+    for func in
+    [search_wiki, search_google_and_summarize, search_wolfram_alpha]
 ]
```

### Comparing `camel_ai-0.1.1/camel/functions/unstructured_io_fuctions.py` & `camel_ai-0.1.2/camel/loaders/unstructured_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,38 +8,38 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
 
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Literal, Optional, Tuple, Union
 
 
-class UnstructuredModules:
+class UnstructuredIO:
     r"""A class to handle various functionalities provided by the
     Unstructured library, including version checking, parsing, cleaning,
     extracting, staging, chunking data, and integrating with cloud
     services like S3 and Azure for data connection.
 
     Attributes:
         UNSTRUCTURED_MIN_VERSION (str): The minimum required version of
             the Unstructured library.
     """
 
     UNSTRUCTURED_MIN_VERSION = "0.10.30"  # Define the minimum version
 
     def __init__(self):
-        r"""Initializes the UnstructuredModules class and ensures the
+        r"""Initializes the UnstructuredIO class and ensures the
         installed version of Unstructured library meets the minimum
         requirements.
         """
-        self.ensure_unstructured_version(self.UNSTRUCTURED_MIN_VERSION)
+        self._ensure_unstructured_version(self.UNSTRUCTURED_MIN_VERSION)
 
-    def ensure_unstructured_version(self, min_version: str) -> None:
+    def _ensure_unstructured_version(self, min_version: str) -> None:
         r"""Validates that the installed 'Unstructured' library version
         satisfies the specified minimum version requirement. This function is
         essential for ensuring compatibility with features that depend on a
         certain version of the 'Unstructured' package.
 
         Args:
             min_version (str): The minimum version required, specified in
@@ -70,19 +70,22 @@
         if installed_ver < min_ver:
             raise ValueError(f"Require `unstructured>={min_version}`, "
                              f"you have {__version__}.")
 
     def parse_file_or_url(
         self,
         input_path: str,
+        **kwargs: Any,
     ) -> Union[Any, List[Any]]:
         r"""Loads a file or a URL and parses its contents as unstructured data.
 
         Args:
             input_path (str): Path to the file or URL to be parsed.
+            **kwargs: Extra kwargs passed to the partition function.
+
         Returns:
             List[Any]: The elements after parsing the file or URL, could be a
                 dict, list, etc., depending on the content. If return_str is
                 True, returns a tuple with a string representation of the
                 elements and the elements themselves.
 
         Raises:
@@ -111,15 +114,15 @@
         is_url = all([parsed_url.scheme, parsed_url.netloc])
 
         if is_url:
             # Handling URL
             from unstructured.partition.html import partition_html
 
             try:
-                elements = partition_html(url=input_path)
+                elements = partition_html(url=input_path, **kwargs)
                 return elements
             except Exception as e:
                 raise Exception("Failed to parse the URL.") from e
 
         else:
             # Handling file
             from unstructured.partition.auto import partition
@@ -128,70 +131,61 @@
             if not os.path.exists(input_path):
                 raise FileNotFoundError(
                     f"The file {input_path} was not found.")
 
             # Read the file
             try:
                 with open(input_path, "rb") as f:
-                    elements = partition(file=f)
+                    elements = partition(file=f, **kwargs)
                     return elements
             except Exception as e:
                 raise Exception(
                     "Failed to parse the unstructured file.") from e
 
     def clean_text_data(
         self,
         text: str,
         clean_options: Optional[List[Tuple[str, Dict[str, Any]]]] = None,
     ) -> str:
         r"""Cleans text data using a variety of cleaning functions provided by
-        the `'unstructured'` library.
+        the `unstructured` library.
 
         This function applies multiple text cleaning utilities by calling the
-        `'unstructured'` library's cleaning bricks for operations like
+        `unstructured` library's cleaning bricks for operations like
         replacing unicode quotes, removing extra whitespace, dashes, non-ascii
         characters, and more.
 
         If no cleaning options are provided, a default set of cleaning
         operations is applied. These defaults including operations
         "replace_unicode_quotes", "clean_non_ascii_chars",
         "group_broken_paragraphs", and "clean_extra_whitespace".
 
         Args:
             text (str): The text to be cleaned.
-            clean_options (dict): A dictionary specifying which
-                                cleaning options to apply. The keys should
-                                match the names of the cleaning functions,
-                                and the values should be dictionaries
-                                containing the parameters for each
-                                function. Supported types:
-                                'clean_extra_whitespace',
-                                'clean_bullets',
-                                'clean_ordered_bullets',
-                                'clean_postfix',
-                                'clean_prefix',
-                                'clean_dashes',
-                                'clean_trailing_punctuation',
-                                'clean_non_ascii_chars',
-                                'group_broken_paragraphs',
-                                'remove_punctuation',
-                                'replace_unicode_quotes',
-                                'bytes_string_to_string',
-                                'translate_text'.
+            clean_options (dict): A dictionary specifying which cleaning
+                options to apply. The keys should match the names of the
+                cleaning functions, and the values should be dictionaries
+                containing the parameters for each function. Supported types:
+                'clean_extra_whitespace', 'clean_bullets',
+                'clean_ordered_bullets', 'clean_postfix', 'clean_prefix',
+                'clean_dashes', 'clean_trailing_punctuation',
+                'clean_non_ascii_chars', 'group_broken_paragraphs',
+                'remove_punctuation', 'replace_unicode_quotes',
+                'bytes_string_to_string', 'translate_text'.
 
         Returns:
             str: The cleaned text.
 
         Raises:
             AttributeError: If a cleaning option does not correspond to a
-                valid cleaning function in 'unstructured'.
+                valid cleaning function in `unstructured`.
 
         Notes:
             The 'options' dictionary keys must correspond to valid cleaning
-            brick names from the 'unstructured' library.
+            brick names from the `unstructured` library.
             Each brick's parameters must be provided in a nested dictionary
             as the value for the key.
 
         References:
             https://unstructured-io.github.io/unstructured/
         """
 
@@ -239,36 +233,40 @@
         cleaned_text = text
         for func_name, params in clean_options:
             if func_name in cleaning_functions:
                 cleaned_text = cleaning_functions[func_name](cleaned_text,
                                                              **params)
             else:
                 raise ValueError(
-                    f"'{func_name}' is not a valid function in 'unstructured'."
+                    f"'{func_name}' is not a valid function in `unstructured`."
                 )
 
         return cleaned_text
 
-    def extract_data_from_text(self, text: str, extract_type: str,
-                               **kwargs) -> Any:
+    def extract_data_from_text(
+        self,
+        text: str,
+        extract_type: Literal['extract_datetimetz', 'extract_email_address',
+                              'extract_ip_address', 'extract_ip_address_name',
+                              'extract_mapi_id', 'extract_ordered_bullets',
+                              'extract_text_after', 'extract_text_before',
+                              'extract_us_phone_number'],
+        **kwargs,
+    ) -> Any:
         r"""Extracts various types of data from text using functions from
         unstructured.cleaners.extract.
 
         Args:
             text (str): Text to extract data from.
-            extract_type (str): Type of data to extract. Supported types:
-                                'extract_datetimetz',
-                                'extract_email_address',
-                                'extract_ip_address',
-                                'extract_ip_address_name',
-                                'extract_mapi_id',
-                                'extract_ordered_bullets',
-                                'extract_text_after',
-                                'extract_text_before',
-                                'extract_us_phone_number'.
+            extract_type (Literal['extract_datetimetz',
+                'extract_email_address', 'extract_ip_address',
+                'extract_ip_address_name', 'extract_mapi_id',
+                'extract_ordered_bullets', 'extract_text_after',
+                'extract_text_before', 'extract_us_phone_number']): Type of
+                data to extract.
             **kwargs: Additional keyword arguments for specific
                 extraction functions.
 
         Returns:
             Any: The extracted data, type depends on extract_type.
 
         References:
@@ -300,40 +298,42 @@
         }
 
         if extract_type not in extraction_functions:
             raise ValueError(f"Unsupported extract_type: {extract_type}")
 
         return extraction_functions[extract_type](text, **kwargs)
 
-    def stage_elements(self, elements: List[Any], stage_type: str,
-                       **kwargs) -> Union[str, List[Dict], Any]:
+    def stage_elements(
+        self,
+        elements: List[Any],
+        stage_type: Literal['convert_to_csv', 'convert_to_dataframe',
+                            'convert_to_dict', 'dict_to_elements',
+                            'stage_csv_for_prodigy', 'stage_for_prodigy',
+                            'stage_for_baseplate', 'stage_for_datasaur',
+                            'stage_for_label_box', 'stage_for_label_studio',
+                            'stage_for_weaviate'],
+        **kwargs,
+    ) -> Union[str, List[Dict], Any]:
         r"""Stages elements for various platforms based on the
         specified staging type.
 
         This function applies multiple staging utilities to format data
         for different NLP annotation and machine learning tools. It uses
         the 'unstructured.staging' module's functions for operations like
         converting to CSV, DataFrame, dictionary, or formatting for
         specific platforms like Prodigy, etc.
 
         Args:
             elements (List[Any]): List of Element objects to be staged.
-            stage_type (str): Type of staging to perform. Supported types:
-                            'convert_to_csv',
-                            'convert_to_dataframe',
-                            'convert_to_dict',
-                            'dict_to_elements',
-                            'stage_csv_for_prodigy',
-                            'stage_for_prodigy',
-                            'stage_for_argilla',
-                            'stage_for_baseplate',
-                            'stage_for_datasaur',
-                            'stage_for_label_box',
-                            'stage_for_label_studio',
-                            'stage_for_weaviate'.
+            stage_type (Literal['convert_to_csv', 'convert_to_dataframe',
+                'convert_to_dict', 'dict_to_elements',
+                'stage_csv_for_prodigy', 'stage_for_prodigy',
+                'stage_for_baseplate', 'stage_for_datasaur',
+                'stage_for_label_box', 'stage_for_label_studio',
+                'stage_for_weaviate']): Type of staging to perform.
             **kwargs: Additional keyword arguments specific to
                 the staging type.
 
         Returns:
             Union[str, List[Dict], Any]: Staged data in the
                 format appropriate for the specified staging type.
 
@@ -341,15 +341,14 @@
             ValueError: If the staging type is not supported or a required
                 argument is missing.
         References:
             https://unstructured-io.github.io/unstructured/
         """
 
         from unstructured.staging import (
-            argilla,
             base,
             baseplate,
             datasaur,
             label_box,
             label_studio,
             prodigy,
             weaviate,
@@ -366,16 +365,14 @@
             base.dict_to_elements,
             "stage_csv_for_prodigy":
             lambda els, **kw: prodigy.stage_csv_for_prodigy(
                 els, kw.get('metadata', [])),
             "stage_for_prodigy":
             lambda els, **kw: prodigy.stage_for_prodigy(
                 els, kw.get('metadata', [])),
-            "stage_for_argilla":
-            lambda els, **kw: argilla.stage_for_argilla(els, **kw),
             "stage_for_baseplate":
             baseplate.stage_for_baseplate,
             "stage_for_datasaur":
             lambda els, **kw: datasaur.stage_for_datasaur(
                 els, kw.get('entities', [])),
             "stage_for_label_box":
             lambda els, **kw: label_box.stage_for_label_box(els, **kw),
@@ -393,15 +390,15 @@
     def chunk_elements(self, elements: List[Any], chunk_type: str,
                        **kwargs) -> List[Any]:
         r"""Chunks elements by titles.
 
         Args:
             elements (List[Any]): List of Element objects to be chunked.
             chunk_type (str): Type chunk going to apply. Supported types:
-                            'chunk_by_title'.
+                'chunk_by_title'.
             **kwargs: Additional keyword arguments for chunking.
 
         Returns:
             List[Dict]: List of chunked sections.
 
         References:
             https://unstructured-io.github.io/unstructured/
```

### Comparing `camel_ai-0.1.1/camel/functions/weather_functions.py` & `camel_ai-0.1.2/camel/functions/weather_functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
 import os
-from typing import List
+from typing import List, Literal
 
 from camel.functions import OpenAIFunction
 
 
 def get_openweathermap_api_key() -> str:
     r"""Retrieve the OpenWeatherMap API key from environment variables.
 
@@ -31,39 +31,43 @@
     if not OPENWEATHERMAP_API_KEY:
         raise ValueError("`OPENWEATHERMAP_API_KEY` not found in environment "
                          "variables. Get `OPENWEATHERMAP_API_KEY` here: "
                          "`https://openweathermap.org`.")
     return OPENWEATHERMAP_API_KEY
 
 
-def get_weather_data(city: str, temp_units: str = 'kelvin',
-                     wind_units: str = 'meters_sec',
-                     visibility_units: str = 'meters',
-                     time_units: str = 'unix') -> str:
+def get_weather_data(
+    city: str,
+    temp_units: Literal['kelvin', 'celsius', 'fahrenheit'] = 'kelvin',
+    wind_units: Literal['meters_sec', 'miles_hour', 'knots',
+                        'beaufort'] = 'meters_sec',
+    visibility_units: Literal['meters', 'miles'] = 'meters',
+    time_units: Literal['unix', 'iso', 'date'] = 'unix',
+) -> str:
     r"""Fetch and return a comprehensive weather report for a given city as a
     string. The report includes current weather conditions, temperature,
     wind details, visibility, and sunrise/sunset times, all formatted as
 
     The function interacts with the OpenWeatherMap API to retrieve the data.
 
     Args:
-        city (string): The name of the city for which the weather information
+        city (str): The name of the city for which the weather information
             is desired. Format "City, CountryCode" (e.g., "Paris, FR"
             for Paris, France). If the country code is not provided,
             the API will search for the city in all countries, which
             may yield incorrect results if multiple cities with the
             same name exist.
-        temp_units (string): Units for temperature. Options: 'kelvin',
-            'celsius', 'fahrenheit'. (default: :obj:`kelvin`)
-        wind_units (string): Units for wind speed. Options: 'meters_sec',
-            'miles_hour', 'knots', 'beaufort'. (default: :obj:`meters_sec`)
-        visibility_units (string): Units for visibility distance. Options:
-            'meters', 'miles'. (default: :obj:`meters`)
-        time_units (string): Format for sunrise and sunset times. Options:
-            'unix', 'iso', 'date'. (default: :obj:`unix`)
+        temp_units (Literal['kelvin', 'celsius', 'fahrenheit']): Units for
+            temperature. (default: :obj:`kelvin`)
+        wind_units (Literal['meters_sec', 'miles_hour', 'knots', 'beaufort']):
+            Units for wind speed. (default: :obj:`meters_sec`)
+        visibility_units (Literal['meters', 'miles']): Units for visibility
+            distance. (default: :obj:`meters`)
+        time_units (Literal['unix', 'iso', 'date']): Format for sunrise and
+            sunset times. (default: :obj:`unix`)
 
     Returns:
         str: A string containing the fetched weather data, formatted in a
             readable manner. If an error occurs, a message indicating the
             error will be returned instead.
 
     Example of return string:
```

### Comparing `camel_ai-0.1.1/camel/generators.py` & `camel_ai-0.1.2/camel/generators.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/human.py` & `camel_ai-0.1.2/camel/human.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/memories/__init__.py` & `camel_ai-0.1.2/camel/memories/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,20 +9,30 @@
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
 
 from .records import MemoryRecord, ContextRecord
-from .base import BaseMemory
-from .context_creators.base import BaseContextCreator
+from .base import MemoryBlock, AgentMemory, BaseContextCreator
 from .context_creators.score_based import ScoreBasedContextCreator
-from .chat_history_memory import ChatHistoryMemory
+from .blocks.chat_history_block import ChatHistoryBlock
+from .blocks.vectordb_block import VectorDBBlock
+from .agent_memories import (
+    VectorDBMemory,
+    ChatHistoryMemory,
+    LongtermAgentMemory,
+)
 
 __all__ = [
     'MemoryRecord',
     'ContextRecord',
-    'BaseMemory',
+    'MemoryBlock',
+    "AgentMemory",
+    'BaseContextCreator',
+    'ScoreBasedContextCreator',
     'ChatHistoryMemory',
-    "BaseContextCreator",
-    "ScoreBasedContextCreator",
+    'VectorDBMemory',
+    'ChatHistoryBlock',
+    'VectorDBBlock',
+    'LongtermAgentMemory',
 ]
```

### Comparing `camel_ai-0.1.1/camel/memories/chat_history_memory.py` & `camel_ai-0.1.2/camel/memories/blocks/chat_history_block.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,94 +7,94 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
-from typing import List, Optional, Tuple
+import warnings
+from typing import List, Optional
 
-from camel.memories import BaseMemory, ContextRecord, MemoryRecord
-from camel.memories.context_creators import BaseContextCreator
-from camel.messages import OpenAIMessage
+from camel.memories import ContextRecord, MemoryBlock, MemoryRecord
 from camel.storages import BaseKeyValueStorage, InMemoryKeyValueStorage
 from camel.types import OpenAIBackendRole
 
 
-class ChatHistoryMemory(BaseMemory):
-    r"""An implementation of the :obj:`BaseMemory` abstract base class for
+class ChatHistoryBlock(MemoryBlock):
+    r"""An implementation of the :obj:`MemoryBlock` abstract base class for
     maintaining a record of chat histories.
 
-    This memory class helps manage conversation histories with a designated
-    storage mechanism, either provided by the user or using a default
+    This memory block helps manage conversation histories with a key-value
+    storage backend, either provided by the user or using a default
     in-memory storage. It offers a windowed approach to retrieving chat
     histories, allowing users to specify how many recent messages they'd
     like to fetch.
 
-    `ChatHistoryMemory` requires messages to be stored with certain
-    metadata (e.g., `role_at_backend`) to maintain consistency and validate
-    the chat history.
-
     Args:
-        context_creator (BaseContextCreator): A context creator contianing
-            the context limit and the message pruning strategy.
         storage (BaseKeyValueStorage, optional): A storage mechanism for
             storing chat history. If `None`, an :obj:`InMemoryKeyValueStorage`
             will be used. (default: :obj:`None`)
-        window_size (int, optional): Specifies the number of recent chat
-            messages to retrieve. If not provided, the entire chat history
-            will be retrieved. (default: :obj:`None`)
+        keep_rate (float, optional): In historical messages, the score of the
+            last message is 1.0, and with each step taken backward, the score
+            of the message is multiplied by the `keep_rate`. Higher `keep_rate`
+            leads to high possiblity to keep history messages during context
+            creation.
     """
 
     def __init__(
         self,
-        context_creator: BaseContextCreator,
         storage: Optional[BaseKeyValueStorage] = None,
-        window_size: Optional[int] = None,
+        keep_rate: float = 0.9,
     ) -> None:
-        self.context_creator = context_creator
+        if keep_rate > 1 or keep_rate < 0:
+            raise ValueError("`keep_rate` should be in [0,1]")
         self.storage = storage or InMemoryKeyValueStorage()
-        self.window_size = window_size
+        self.keep_rate = keep_rate
 
-    def get_context(self) -> Tuple[List[OpenAIMessage], int]:
-        r"""Gets chat context with a proper size for the agent from the memory
+    def retrieve(
+        self,
+        window_size: Optional[int] = None,
+    ) -> List[ContextRecord]:
+        r"""Retrieves records with a proper size for the agent from the memory
         based on the window size or fetches the entire chat history if no
         window size is specified.
 
+        Args:
+            window_size (int, optional): Specifies the number of recent chat
+                messages to retrieve. If not provided, the entire chat history
+                will be retrieved. (default: :obj:`None`)
+
         Returns:
-            (List[OpenAIMessage], int): A tuple containing the constructed
-                context in OpenAIMessage format and the total token count.
-        Raises:
-            ValueError: If the memory is empty or if the first message in the
-                memory is not a system message.
+            List[ContextRecord]: A list of retrieved records.
         """
         record_dicts = self.storage.load()
         if len(record_dicts) == 0:
-            raise ValueError("The `ChatHistoryMemory` is empty.")
+            warnings.warn("The `ChatHistoryMemory` is empty.")
+            return list()
 
         chat_records: List[MemoryRecord] = []
-        truncate_idx = -self.window_size if self.window_size is not None else 0
+        truncate_idx = -window_size if window_size is not None else 0
         for record_dict in record_dicts[truncate_idx:]:
             chat_records.append(MemoryRecord.from_dict(record_dict))
 
         # We assume that, in the chat history memory, the closer the record is
         # to the current message, the more score it will be.
         output_records = []
         score = 1.0
         for record in reversed(chat_records):
             if record.role_at_backend == OpenAIBackendRole.SYSTEM:
                 # System messages are always kept.
                 output_records.append(ContextRecord(record, 1.0))
             else:
                 # Other messages' score drops down gradually
-                score *= 0.99
+                score *= self.keep_rate
                 output_records.append(ContextRecord(record, score))
 
         output_records.reverse()
-        return self.context_creator.create_context(output_records)
+        return output_records
 
     def write_records(self, records: List[MemoryRecord]) -> None:
         r"""Writes memory records to the memory. Additionally, performs
         validation checks on the messages.
 
         Args:
             records (List[MemoryRecord]): Memory records to be added to the
@@ -102,10 +102,9 @@
         """
         stored_records = []
         for record in records:
             stored_records.append(record.to_dict())
         self.storage.save(stored_records)
 
     def clear(self) -> None:
-        r"""Clears all chat messages from the memory.
-        """
+        r"""Clears all chat messages from the memory."""
         self.storage.clear()
```

### Comparing `camel_ai-0.1.1/camel/memories/context_creators/__init__.py` & `camel_ai-0.1.2/camel/models/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,12 +7,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
+from .base_model import BaseModelBackend
+from .openai_model import OpenAIModel
+from .stub_model import StubModel
+from .open_source_model import OpenSourceModel
+from .model_factory import ModelFactory
 
-from .base import BaseContextCreator
-from .score_based import ScoreBasedContextCreator
-
-__all__ = ['BaseContextCreator', 'ScoreBasedContextCreator']
+__all__ = [
+    'BaseModelBackend',
+    'OpenAIModel',
+    'StubModel',
+    'OpenSourceModel',
+    'ModelFactory',
+]
```

### Comparing `camel_ai-0.1.1/camel/memories/context_creators/base.py` & `camel_ai-0.1.2/camel/storages/key_value_storages/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,66 +7,51 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
+
 from abc import ABC, abstractmethod
-from typing import List, Tuple
+from typing import Any, Dict, List
+
+
+class BaseKeyValueStorage(ABC):
+    r"""An abstract base class for key-value storage systems. Provides a
+    consistent interface for saving, loading, and clearing data records without
+    any loss of information.
+
+    An abstract base class designed to serve as a foundation for various
+    key-value storage systems. The class primarily interacts through Python
+    dictionaries.
 
-from camel.memories import ContextRecord
-from camel.messages import OpenAIMessage
-from camel.utils import BaseTokenCounter
-
-
-class BaseContextCreator(ABC):
-    r"""An abstract base class defining the interface for context creation
-    strategies.
-
-    This class provides a foundational structure for different strategies to
-    generate conversational context from a list of context records. The
-    primary goal is to create a context that is aligned with a specified token
-    count limit, allowing subclasses to define their specific approach.
-
-    Subclasses should implement the `token_counter`, `token_limit`, and
-    `create_context` methods to provide specific context creation logic.
-
-    Attributes:
-        token_counter (BaseTokenCounter): A token counter instance responsible
-            for counting tokens in a message.
-        token_limit (int): The maximum number of tokens allowed in the
-            generated context.
+    This class is meant to be inherited by multiple types of key-value storage
+    implementations, including, but not limited to, JSON file storage, NoSQL
+    databases like MongoDB and Redis, as well as in-memory Python dictionaries.
     """
 
-    @property
     @abstractmethod
-    def token_counter(self) -> BaseTokenCounter:
-        pass
+    def save(self, records: List[Dict[str, Any]]) -> None:
+        r"""Saves a batch of records to the key-value storage system.
 
-    @property
-    @abstractmethod
-    def token_limit(self) -> int:
+        Args:
+            records (List[Dict[str, Any]]): A list of dictionaries, where each
+                dictionary represents a unique record to be stored.
+        """
         pass
 
     @abstractmethod
-    def create_context(
-        self,
-        records: List[ContextRecord],
-    ) -> Tuple[List[OpenAIMessage], int]:
-        r"""An abstract method to create conversational context from the chat
-        history.
-
-        Constructs the context from provided records. The specifics of how this
-        is done and how the token count is managed should be provided by
-        subclasses implementing this method. The the output messages order
-        should keep same as the input order.
-
-        Args:
-            records (List[ContextRecord]): A list of context records from
-                which to generate the context.
+    def load(self) -> List[Dict[str, Any]]:
+        r"""Loads all stored records from the key-value storage system.
 
         Returns:
-            Tuple[List[OpenAIMessage], int]: A tuple containing the constructed
-                context in OpenAIMessage format and the total token count.
+            List[Dict[str, Any]]: A list of dictionaries, where each dictionary
+                represents a stored record.
+        """
+        pass
+
+    @abstractmethod
+    def clear(self) -> None:
+        r"""Removes all records from the key-value storage system.
         """
         pass
```

### Comparing `camel_ai-0.1.1/camel/memories/context_creators/score_based.py` & `camel_ai-0.1.2/camel/memories/context_creators/score_based.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
 from dataclasses import dataclass
 from typing import List, Tuple
 
-from camel.memories import ContextRecord
-from camel.memories.context_creators import BaseContextCreator
+from camel.memories import BaseContextCreator, ContextRecord
 from camel.messages import OpenAIMessage
 from camel.utils import BaseTokenCounter
 
 
 @dataclass(frozen=True)
 class _ContextUnit:
     idx: int
@@ -75,22 +74,28 @@
             Tuple[List[OpenAIMessage], int]: A tuple containing the constructed
                 context in OpenAIMessage format and the total token count.
 
         Raises:
             RuntimeError: If it's impossible to create a valid context without
                 exceeding the token limit.
         """
-        context_units = [
-            _ContextUnit(
-                idx,
-                record,
-                self.token_counter.count_tokens_from_messages(
-                    [record.memory_record.to_openai_message()]),
-            ) for idx, record in enumerate(records)
-        ]
+        # Create unique context units list
+        uuid_set = set()
+        context_units = []
+        for idx, record in enumerate(records):
+            if record.memory_record.uuid not in uuid_set:
+                uuid_set.add(record.memory_record.uuid)
+                context_units.append(
+                    _ContextUnit(
+                        idx,
+                        record,
+                        self.token_counter.count_tokens_from_messages(
+                            [record.memory_record.to_openai_message()]),
+                    ))
+
         # TODO: optimize the process, may give information back to memory
 
         # If not exceed token limit, simply return
         total_tokens = sum([unit.num_tokens for unit in context_units])
         if total_tokens <= self.token_limit:
             return self._create_output(context_units)
```

### Comparing `camel_ai-0.1.1/camel/memories/records.py` & `camel_ai-0.1.2/camel/memories/records.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,11 +82,10 @@
     def to_openai_message(self) -> OpenAIMessage:
         r"""Converts the record to an :obj:`OpenAIMessage` object."""
         return self.message.to_openai_message(self.role_at_backend)
 
 
 @dataclass(frozen=True)
 class ContextRecord:
-    r"""The result of memory retrieving.
-    """
+    r"""The result of memory retrieving."""
     memory_record: MemoryRecord
     score: float
```

### Comparing `camel_ai-0.1.1/camel/messages/__init__.py` & `camel_ai-0.1.2/camel/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/messages/base.py` & `camel_ai-0.1.2/camel/messages/base.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/messages/func_message.py` & `camel_ai-0.1.2/camel/messages/func_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     def to_openai_assistant_message(self) -> OpenAIAssistantMessage:
         r"""Converts the message to an :obj:`OpenAIAssistantMessage` object.
 
         Returns:
             OpenAIAssistantMessage: The converted :obj:`OpenAIAssistantMessage`
                 object.
         """
-        if (not self.func_name) or (not self.args):
+        if (not self.func_name) or (self.args is None):
             raise ValueError(
                 "Invalid request for converting into assistant message"
                 " due to missing function name or arguments.")
 
         msg_dict: OpenAIAssistantMessage = {
             "role": "assistant",
             "content": self.content,
```

### Comparing `camel_ai-0.1.1/camel/models/__init__.py` & `camel_ai-0.1.2/camel/interpreters/interpreter_error.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,20 +7,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
-from .base_model import BaseModelBackend
-from .openai_model import OpenAIModel
-from .stub_model import StubModel
-from .open_source_model import OpenSourceModel
-from .model_factory import ModelFactory
 
-__all__ = [
-    'BaseModelBackend',
-    'OpenAIModel',
-    'StubModel',
-    'OpenSourceModel',
-    'ModelFactory',
-]
+
+class InterpreterError(Exception):
+    r"""Exception raised for errors that can be solved by regenerating code """
+    pass
```

### Comparing `camel_ai-0.1.1/camel/models/base_model.py` & `camel_ai-0.1.2/camel/models/base_model.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/models/model_factory.py` & `camel_ai-0.1.2/camel/models/model_factory.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/models/open_source_model.py` & `camel_ai-0.1.2/camel/models/open_source_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,14 +68,15 @@
             raise ValueError(
                 "URL to server running open-source LLM is not provided.")
         self.server_url: str = server_url
         self._client = OpenAI(
             base_url=self.server_url,
             timeout=60,
             max_retries=3,
+            api_key="fake_key",
         )
 
         # Replace `model_config_dict` with only the params to be
         # passed to OpenAI API
         self.model_config_dict = self.model_config_dict["api_params"].__dict__
 
     @property
```

### Comparing `camel_ai-0.1.1/camel/models/openai_model.py` & `camel_ai-0.1.2/camel/models/openai_model.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/models/stub_model.py` & `camel_ai-0.1.2/camel/models/stub_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,15 @@
                 Choice(
                     finish_reason="stop",
                     index=0,
                     message=ChatCompletionMessage(
                         content=ARBITRARY_STRING,
                         role="assistant",
                     ),
+                    logprobs=None,
                 )
             ],
             usage=CompletionUsage(
                 completion_tokens=10,
                 prompt_tokens=10,
                 total_tokens=20,
             ),
```

### Comparing `camel_ai-0.1.1/camel/prompts/__init__.py` & `camel_ai-0.1.2/camel/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/prompts/ai_society.py` & `camel_ai-0.1.2/camel/prompts/ai_society.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/prompts/base.py` & `camel_ai-0.1.2/camel/prompts/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,28 +8,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
 import inspect
-from typing import (
-    Any,
-    Callable,
-    Dict,
-    List,
-    Optional,
-    Set,
-    Tuple,
-    TypeVar,
-    Union,
-)
+from typing import Any, Callable, Dict, Optional, Set, TypeVar, Union
 
+from camel.interpreters import BaseInterpreter, SubprocessInterpreter
 from camel.types import RoleType
-from camel.utils import PythonInterpreter
+from camel.utils import get_system_information
 
 T = TypeVar('T')
 
 
 def return_prompt_wrapper(
     cls: Any,
     func: Callable,
@@ -168,60 +159,69 @@
 
         Args:
             code_type (str): The type of code.
         """
         self._code_type = code_type
 
     def execute(
-        self, interpreter: Optional[PythonInterpreter] = None,
-        user_variable: Optional[Dict[str, Any]] = None
-    ) -> Tuple[Any, PythonInterpreter]:
-        r"""Executes the code string by a given python interpreter.
+        self,
+        interpreter: Optional[BaseInterpreter] = None,
+        **kwargs: Any,
+    ) -> str:
+        r"""Executes the code string using the provided interpreter.
+
+        This method runs a code string through either a specified interpreter
+        or a default one. It supports additional keyword arguments for
+        flexibility.
 
         Args:
-            interpreter (PythonInterpreter, optional): interpreter to be used
-                during code execution. (default: :obj:`None`)
-            user_variable (Optional[Dict[str, Any]]): varibales that can be
-                used in the code, which applying fuzzy matching, such as images
-                or documents. (default: :obj:`None`)
+            interpreter (Optional[BaseInterpreter]): The interpreter instance
+                to use for execution. If `None`, a default interpreter is used.
+                (default: :obj:`None`)
+            **kwargs: Additional keyword arguments passed to the interpreter to
+                run the code.
 
         Returns:
-            Tuple[Any, PythonInterpreter]: A tuple containing the execution
-                result and the used interpreter. The execution result
-                represents the value of the last statement (excluding "import")
-                in the code. This value could potentially be the desired result
-                of the LLM-generated code.        
-    """
-        # NOTE: Only supports Python code for now.
-        if not interpreter:
-            interpreter = PythonInterpreter(action_space=globals())
-        execution_res = interpreter.execute(self, fuzz_state=user_variable,
-                                            keep_state=True)
-        return execution_res, interpreter
+            str: The result of the code execution. If the execution fails, this
+                should include sufficient information to diagnose and correct
+                the issue.
+
+        Raises:
+            InterpreterError: If the code execution encounters errors that
+                could be resolved by modifying or regenerating the code.
+    """
+        if interpreter is None:
+            execution_res = SubprocessInterpreter().run(
+                self, self._code_type, **kwargs)
+        else:
+            execution_res = interpreter.run(self, self._code_type, **kwargs)
+        return execution_res
 
 
 # flake8: noqa :E501
 class TextPromptDict(Dict[Any, TextPrompt]):
     r"""A dictionary class that maps from key to :obj:`TextPrompt` object.
     """
     EMBODIMENT_PROMPT = TextPrompt(
+        "System information :" +
+        "\n".join(f"{key}: {value}"
+                  for key, value in get_system_information().items()) + "\n" +
         """You are the physical embodiment of the {role} who is working on solving a task: {task}.
 You can do things in the physical world including browsing the Internet, reading documents, drawing images, creating videos, executing code and so on.
 Your job is to perform the physical actions necessary to interact with the physical world.
 You will receive thoughts from the {role} and you will need to perform the actions described in the thoughts.
-You can write a series of simple commands in Python to act.
-You can perform a set of actions by calling the available Python functions.
+You can write a series of simple commands in to act.
+You can perform a set of actions by calling the available functions.
 You should perform actions based on the descriptions of the functions.
 
-Here is your action space:
+Here is your action space but it is not limited:
 {action_space}
 
-You should only perform actions in the action space.
 You can perform multiple actions.
 You can perform actions in any order.
-First, explain the actions you will perform and your reasons, then write Python code to implement your actions.
-If you decide to perform actions, you must write Python code to implement the actions.
+First, explain the actions you will perform and your reasons, then write code to implement your actions.
+If you decide to perform actions, you must write code to implement the actions.
 You may print intermediate results if necessary.""")
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self.update({RoleType.EMBODIMENT: self.EMBODIMENT_PROMPT})
```

### Comparing `camel_ai-0.1.1/camel/prompts/code.py` & `camel_ai-0.1.2/camel/prompts/code.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/prompts/evaluation.py` & `camel_ai-0.1.2/camel/prompts/evaluation.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/prompts/misalignment.py` & `camel_ai-0.1.2/camel/prompts/misalignment.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/prompts/prompt_templates.py` & `camel_ai-0.1.2/camel/prompts/prompt_templates.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/prompts/role_description_prompt_template.py` & `camel_ai-0.1.2/camel/prompts/role_description_prompt_template.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/prompts/solution_extraction.py` & `camel_ai-0.1.2/camel/prompts/solution_extraction.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/prompts/task_prompt_template.py` & `camel_ai-0.1.2/camel/prompts/task_prompt_template.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/prompts/translation.py` & `camel_ai-0.1.2/camel/prompts/translation.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/responses/__init__.py` & `camel_ai-0.1.2/camel/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/responses/agent_responses.py` & `camel_ai-0.1.2/camel/responses/agent_responses.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/societies/__init__.py` & `camel_ai-0.1.2/LICENSES/license_template.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
-from .role_playing import RolePlaying
-from .babyagi_playing import BabyAGI
-
-__all__ = [
-    'RolePlaying',
-    'BabyAGI',
-]
+# =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
```

### Comparing `camel_ai-0.1.1/camel/societies/babyagi_playing.py` & `camel_ai-0.1.2/camel/societies/babyagi_playing.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/societies/role_playing.py` & `camel_ai-0.1.2/camel/societies/role_playing.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 class RolePlaying:
     r"""Role playing between two agents.
 
     Args:
         assistant_role_name (str): The name of the role played by the
             assistant.
         user_role_name (str): The name of the role played by the user.
-        critic_role_name (str): The name of the role played by the critic.
-            Role name with :obj:`"human"` will set critic as a :obj:`Human`
-            agent, else will create a :obj:`CriticAgent`.
+        critic_role_name (str, optional): The name of the role played by the
+            critic. Role name with :obj:`"human"` will set critic as a
+            :obj:`Human` agent, else will create a :obj:`CriticAgent`.
             (default: :obj:`"critic"`)
         task_prompt (str, optional): A prompt for the task to be performed.
             (default: :obj:`""`)
         with_task_specify (bool, optional): Whether to use a task specify
             agent. (default: :obj:`True`)
         with_task_planner (bool, optional): Whether to use a task planner
             agent. (default: :obj:`False`)
@@ -100,67 +100,88 @@
         self.with_task_planner = with_task_planner
         self.with_critic_in_the_loop = with_critic_in_the_loop
         self.model_type = model_type
         self.task_type = task_type
         self.task_prompt = task_prompt
 
         self.specified_task_prompt: Optional[TextPrompt] = None
-        self.init_specified_task_prompt(assistant_role_name, user_role_name,
-                                        task_specify_agent_kwargs,
-                                        extend_task_specify_meta_dict,
-                                        output_language)
+        self._init_specified_task_prompt(
+            assistant_role_name,
+            user_role_name,
+            task_specify_agent_kwargs=task_specify_agent_kwargs,
+            extend_task_specify_meta_dict=extend_task_specify_meta_dict,
+            output_language=output_language,
+        )
 
         self.planned_task_prompt: Optional[TextPrompt] = None
-        self.init_planned_task_prompt(task_planner_agent_kwargs,
-                                      output_language)
+        self._init_planned_task_prompt(
+            task_planner_agent_kwargs=task_planner_agent_kwargs,
+            output_language=output_language,
+        )
 
         sys_msg_generator = SystemMessageGenerator(
-            task_type=self.task_type, **(sys_msg_generator_kwargs or {}))
+            task_type=self.task_type,
+            **(sys_msg_generator_kwargs or {}),
+        )
 
-        (init_assistant_sys_msg, init_user_sys_msg,
-         sys_msg_meta_dicts) = self.get_sys_message_info(
-             assistant_role_name, user_role_name, sys_msg_generator,
-             extend_sys_msg_meta_dicts)
+        (
+            init_assistant_sys_msg,
+            init_user_sys_msg,
+            sys_msg_meta_dicts,
+        ) = self._get_sys_message_info(
+            assistant_role_name,
+            user_role_name,
+            sys_msg_generator,
+            extend_sys_msg_meta_dicts=extend_sys_msg_meta_dicts,
+        )
 
         self.assistant_agent: ChatAgent
         self.user_agent: ChatAgent
         self.assistant_sys_msg: BaseMessage
         self.user_sys_msg: BaseMessage
-        self.init_agents(
+        self._init_agents(
             init_assistant_sys_msg,
-            assistant_agent_kwargs,
             init_user_sys_msg,
-            user_agent_kwargs,
-            output_language,
+            assistant_agent_kwargs=assistant_agent_kwargs,
+            user_agent_kwargs=user_agent_kwargs,
+            output_language=output_language,
         )
         self.critic: Optional[Union[CriticAgent, Human]] = None
         self.critic_sys_msg: Optional[BaseMessage] = None
-        self.init_critic(critic_role_name, critic_criteria, critic_kwargs,
-                         sys_msg_generator, sys_msg_meta_dicts)
+        self._init_critic(
+            sys_msg_generator,
+            sys_msg_meta_dicts,
+            critic_role_name,
+            critic_criteria=critic_criteria,
+            critic_kwargs=critic_kwargs,
+        )
 
-    def init_specified_task_prompt(
-            self, assistant_role_name: str, user_role_name: str,
-            task_specify_agent_kwargs: Optional[Dict],
-            extend_task_specify_meta_dict: Optional[Dict],
-            output_language: Optional[str]):
+    def _init_specified_task_prompt(
+        self,
+        assistant_role_name: str,
+        user_role_name: str,
+        task_specify_agent_kwargs: Optional[Dict] = None,
+        extend_task_specify_meta_dict: Optional[Dict] = None,
+        output_language: Optional[str] = None,
+    ) -> None:
         r"""Use a task specify agent to generate a specified task prompt.
         Generated specified task prompt will be used to replace original
         task prompt. If there is no task specify agent, specified task
         prompt will not be generated.
 
         Args:
             assistant_role_name (str): The name of the role played by the
                 assistant.
             user_role_name (str): The name of the role played by the user.
             task_specify_agent_kwargs (Dict, optional): Additional arguments
-                to pass to the task specify agent.
+                to pass to the task specify agent. (default: :obj:`None`)
             extend_task_specify_meta_dict (Dict, optional): A dict to extend
-                the task specify meta dict with.
+                the task specify meta dict with. (default: :obj:`None`)
             output_language (str, optional): The language to be output by the
-                agents.
+                agents. (default: :obj:`None`)
         """
         if self.with_task_specify:
             task_specify_meta_dict = dict()
             if self.task_type in [TaskType.AI_SOCIETY, TaskType.MISALIGNMENT]:
                 task_specify_meta_dict.update(
                     dict(assistant_role=assistant_role_name,
                          user_role=user_role_name))
@@ -177,28 +198,30 @@
             )
             self.specified_task_prompt = task_specify_agent.run(
                 self.task_prompt,
                 meta_dict=task_specify_meta_dict,
             )
             self.task_prompt = self.specified_task_prompt
 
-    def init_planned_task_prompt(self,
-                                 task_planner_agent_kwargs: Optional[Dict],
-                                 output_language: Optional[str]):
+    def _init_planned_task_prompt(
+        self,
+        task_planner_agent_kwargs: Optional[Dict] = None,
+        output_language: Optional[str] = None,
+    ) -> None:
         r"""Use a task plan agent to append a planned task prompt to task
         prompt. The planned task prompt is generated based on the task
         prompt, which can be original task prompt or specified task prompt
         if available. If there is no task plan agent, planned task prompt
         will not be generated.
 
         Args:
             task_planner_agent_kwargs (Dict, optional): Additional arguments
-                to pass to the task planner agent.
+                to pass to the task planner agent. (default: :obj:`None`)
             output_language (str, optional): The language to be output by the
-                agents.
+                agents. (default: :obj:`None`)
         """
         if self.with_task_planner:
             if self.model_type is not None:
                 if task_planner_agent_kwargs is None:
                     task_planner_agent_kwargs = {}
                 task_planner_agent_kwargs.update(
                     dict(model_type=self.model_type))
@@ -208,15 +231,15 @@
             )
             self.planned_task_prompt = task_planner_agent.run(self.task_prompt)
             self.task_prompt = (f"{self.task_prompt}\n"
                                 f"{self.planned_task_prompt}")
         else:
             self.planned_task_prompt = None
 
-    def get_sys_message_info(
+    def _get_sys_message_info(
         self,
         assistant_role_name: str,
         user_role_name: str,
         sys_msg_generator: SystemMessageGenerator,
         extend_sys_msg_meta_dicts: Optional[List[Dict]] = None,
     ) -> Tuple[BaseMessage, BaseMessage, List[Dict]]:
         r"""Get initial assistant and user system message with a list of
@@ -226,19 +249,21 @@
             assistant_role_name (str): The name of the role played by the
                 assistant.
             user_role_name (str): The name of the role played by the user.
             sys_msg_generator (SystemMessageGenerator): A system message
                 generator for agents.
             extend_sys_msg_meta_dicts (List[Dict], optional): A list of dicts
                 to extend the system message meta dicts with.
+                (default: :obj:`None`)
 
         Returns:
-            A tuple containing a `BaseMessage` representing the assistant's
-            initial system message, a `BaseMessage` representing the user's
-            initial system message, and a list of system message meta dicts.
+            Tuple[BaseMessage, BaseMessage, List[Dict]]: A tuple containing a
+                `BaseMessage` representing the assistant's initial system
+                message, a `BaseMessage` representing the user's initial system
+                message, and a list of system message meta dicts.
         """
         sys_msg_meta_dicts = [dict(task=self.task_prompt) for _ in range(2)]
         if (extend_sys_msg_meta_dicts is None and self.task_type in [
                 TaskType.AI_SOCIETY,
                 TaskType.MISALIGNMENT,
         ]):
             extend_sys_msg_meta_dicts = [
@@ -259,35 +284,35 @@
                 role_tuples=[
                     (assistant_role_name, RoleType.ASSISTANT),
                     (user_role_name, RoleType.USER),
                 ],
             ))
         return init_assistant_sys_msg, init_user_sys_msg, sys_msg_meta_dicts
 
-    def init_agents(
+    def _init_agents(
         self,
         init_assistant_sys_msg: BaseMessage,
-        assistant_agent_kwargs: Optional[Dict],
         init_user_sys_msg: BaseMessage,
-        user_agent_kwargs: Optional[Dict],
-        output_language: Optional[str],
-    ):
+        assistant_agent_kwargs: Optional[Dict] = None,
+        user_agent_kwargs: Optional[Dict] = None,
+        output_language: Optional[str] = None,
+    ) -> None:
         r"""Initialize assistant and user agents with their system messages.
 
         Args:
             init_assistant_sys_msg (BaseMessage): Assistant agent's initial
                 system message.
-            assistant_agent_kwargs (Dict, optional): Additional arguments to
-                pass to the assistant agent.
             init_user_sys_msg (BaseMessage): User agent's initial system
                 message.
+            assistant_agent_kwargs (Dict, optional): Additional arguments to
+                pass to the assistant agent. (default: :obj:`None`)
             user_agent_kwargs (Dict, optional): Additional arguments to
-                pass to the user agent.
+                pass to the user agent. (default: :obj:`None`)
             output_language (str, optional): The language to be output by the
-                agents.
+                agents. (default: :obj:`None`)
         """
         if self.model_type is not None:
             if assistant_agent_kwargs is None:
                 assistant_agent_kwargs = {}
             assistant_agent_kwargs.update(dict(model_type=self.model_type))
             if user_agent_kwargs is None:
                 user_agent_kwargs = {}
@@ -303,34 +328,37 @@
         self.user_agent = ChatAgent(
             init_user_sys_msg,
             output_language=output_language,
             **(user_agent_kwargs or {}),
         )
         self.user_sys_msg = self.user_agent.system_message
 
-    def init_critic(self, critic_role_name: str,
-                    critic_criteria: Optional[str],
-                    critic_kwargs: Optional[Dict],
-                    sys_msg_generator: SystemMessageGenerator,
-                    sys_msg_meta_dicts: List[Dict]):
+    def _init_critic(
+        self,
+        sys_msg_generator: SystemMessageGenerator,
+        sys_msg_meta_dicts: List[Dict],
+        critic_role_name: str,
+        critic_criteria: Optional[str] = None,
+        critic_kwargs: Optional[Dict] = None,
+    ) -> None:
         r"""Initialize critic agent. If critic role name is :obj:`"human"`,
         create a :obj:`Human` critic agent. Else, create a :obj:`CriticAgent`
         critic agent with specified critic criteria. If the critic criteria
         is not specified, set it to improve task performance.
 
         Args:
+            sys_msg_generator (SystemMessageGenerator): A system message
+                generator for agents.
+            sys_msg_meta_dicts (list): A list of system message meta dicts.
             critic_role_name (str): The name of the role played by the critic.
             critic_criteria (str, optional): Critic criteria for the
                 critic agent. If not specified, set the criteria to
-                improve task performance.
+                improve task performance. (default: :obj:`None`)
             critic_kwargs (Dict, optional): Additional arguments to
-                pass to the critic.
-            sys_msg_generator (SystemMessageGenerator): A system message
-                generator for agents.
-            sys_msg_meta_dicts (list): A list of system message meta dicts.
+                pass to the critic. (default: :obj:`None`)
         """
         if self.with_critic_in_the_loop:
             if critic_role_name.lower() == "human":
                 self.critic = Human(**(critic_kwargs or {}))
             else:
                 critic_criteria = (critic_criteria
                                    or "improving the task performance")
@@ -346,72 +374,72 @@
                         critic_kwargs = {}
                     critic_kwargs.update(dict(model_type=self.model_type))
                 self.critic = CriticAgent(
                     self.critic_sys_msg,
                     **(critic_kwargs or {}),
                 )
 
-    def init_chat(self) -> Tuple[BaseMessage, List[BaseMessage]]:
-        r"""Initializes the chat by resetting both of the assistant and user
-        agents, and sending the system messages again to the agents using
-        chat messages. Returns the assistant's introductory message and the
-        user's response messages.
-
-        Returns:
-            A tuple containing a `BaseMessage` representing the assistant's
-            introductory message, and a list of `BaseMessage` representing
-            the user's response messages.
-        """
-        self.assistant_agent.reset()
-        self.user_agent.reset()
-
-        # Send the system messages again to the agents using chat messages
-        assistant_msg = BaseMessage.make_assistant_message(
-            role_name=self.assistant_sys_msg.role_name,
-            content=(f"{self.user_sys_msg.content}. "
-                     "Now start to give me instructions one by one. "
-                     "Only reply with Instruction and Input."))
-        user_msg = BaseMessage.make_user_message(
-            role_name=self.user_sys_msg.role_name,
-            content=f"{self.assistant_sys_msg.content}")
-        assistant_response = self.assistant_agent.step(user_msg)
-        if assistant_response.terminated or assistant_response.msgs is None:
-            raise ValueError(f"Assistant agent terminated unexpectedly. "
-                             f"Error info: {assistant_response.info}")
-
-        return assistant_msg, assistant_response.msgs
-
-    def reduce_message_options(
+    def _reduce_message_options(
         self,
         messages: Sequence[BaseMessage],
     ) -> BaseMessage:
         r"""Processes a sequence of chat messages, returning the processed
         message. If multiple messages are provided and
         `with_critic_in_the_loop` is `False`, raises a `ValueError`.
         If no messages are provided, a `ValueError` will be raised.
 
         Args:
-            messages: A sequence of `BaseMessage` objects to process.
+            messages (Sequence[BaseMessage]): A sequence of `BaseMessage`
+                objects to process.
 
         Returns:
-            A single `BaseMessage` representing the processed message.
+            BaseMessage: A single `BaseMessage` representing the processed
+                message.
         """
         if len(messages) == 0:
             raise ValueError("No messages to process.")
         if len(messages) > 1 and not self.with_critic_in_the_loop:
             raise ValueError("Got than one message to process. "
                              f"Num of messages: {len(messages)}.")
         elif self.with_critic_in_the_loop and self.critic is not None:
             critic_response = self.critic.reduce_step(messages)
             processed_msg = critic_response.msg
         else:
             processed_msg = messages[0]
 
         return processed_msg
 
+    def init_chat(self, init_msg_content: Optional[str] = None) -> BaseMessage:
+        r"""Initializes the chat by resetting both of the assistant and user
+        agents. Returns an initial message for the role-playing session.
+
+        Args:
+            init_msg_content (str, optional): A user-specified initial message.
+                Will be sent to the role-playing session as the initial
+                message. (default: :obj:`None`)
+
+        Returns:
+            BaseMessage: A single `BaseMessage` representing the initial
+                message.
+        """
+        self.assistant_agent.reset()
+        self.user_agent.reset()
+        default_init_msg_content = (
+            "Now start to give me instructions one by one. "
+            "Only reply with Instruction and Input.")
+        if init_msg_content is None:
+            init_msg_content = default_init_msg_content
+        # Initialize a message sent by the assistant
+        init_msg = BaseMessage.make_assistant_message(
+            role_name=self.assistant_sys_msg.role_name,
+            content=init_msg_content,
+        )
+
+        return init_msg
+
     def step(
         self,
         assistant_msg: BaseMessage,
     ) -> Tuple[ChatAgentResponse, ChatAgentResponse]:
         r"""Advances the conversation by taking a message from the assistant,
         processing it using the user agent, and then processing the resulting
         message using the assistant agent. Returns a tuple containing the
@@ -421,35 +449,36 @@
         terminated the conversation, and any additional user information.
 
         Args:
             assistant_msg: A `BaseMessage` representing the message from the
                 assistant.
 
         Returns:
-            A tuple containing two ChatAgentResponse: the first struct contains
-            the resulting assistant message, whether the assistant agent
-            terminated the conversation, and any additional assistant
-            information; the second struct contains the resulting user message,
-            whether the user agent terminated the conversation, and any
-            additional user information.
+            Tuple[ChatAgentResponse, ChatAgentResponse]: A tuple containing two
+                ChatAgentResponse: the first struct contains the resulting
+                assistant message, whether the assistant agent terminated the
+                conversation, and any additional assistant information; the
+                second struct contains the resulting user message, whether the
+                user agent terminated the conversation, and any additional user
+                information.
         """
         user_response = self.user_agent.step(assistant_msg)
         if user_response.terminated or user_response.msgs is None:
             return (ChatAgentResponse([], False, {}),
                     ChatAgentResponse([], user_response.terminated,
                                       user_response.info))
-        user_msg = self.reduce_message_options(user_response.msgs)
+        user_msg = self._reduce_message_options(user_response.msgs)
         self.user_agent.record_message(user_msg)
 
         assistant_response = self.assistant_agent.step(user_msg)
         if assistant_response.terminated or assistant_response.msgs is None:
             return (ChatAgentResponse([], assistant_response.terminated,
                                       assistant_response.info),
                     ChatAgentResponse([user_msg], False, user_response.info))
-        assistant_msg = self.reduce_message_options(assistant_response.msgs)
+        assistant_msg = self._reduce_message_options(assistant_response.msgs)
         self.assistant_agent.record_message(assistant_msg)
 
         return (
             ChatAgentResponse([assistant_msg], assistant_response.terminated,
                               assistant_response.info),
             ChatAgentResponse([user_msg], user_response.terminated,
                               user_response.info),
```

### Comparing `camel_ai-0.1.1/camel/storages/__init__.py` & `camel_ai-0.1.2/camel/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,16 +8,13 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
 
-from .key_value_storages.base import BaseKeyValueStorage
-from .key_value_storages.in_memory import InMemoryKeyValueStorage
-from .key_value_storages.json import JsonStorage
+__version__ = '0.1.1'
 
 __all__ = [
-    'BaseKeyValueStorage',
-    'InMemoryKeyValueStorage',
-    'JsonStorage',
+    '__version__',
+    'camel',
 ]
```

### Comparing `camel_ai-0.1.1/camel/storages/key_value_storages/__init__.py` & `camel_ai-0.1.2/camel/retrievers/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,17 +7,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
-
-from .base import BaseKeyValueStorage
-from .in_memory import InMemoryKeyValueStorage
-from .json import JsonStorage
+from .base import BaseRetriever
+from .vector_retriever import VectorRetriever
+from .auto_retriever import AutoRetriever
 
 __all__ = [
-    'BaseKeyValueStorage',
-    'InMemoryKeyValueStorage',
-    'JsonStorage',
+    'BaseRetriever',
+    'VectorRetriever',
+    'AutoRetriever',
 ]
```

### Comparing `camel_ai-0.1.1/camel/storages/key_value_storages/base.py` & `camel_ai-0.1.2/camel/storages/key_value_storages/json.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,50 +8,83 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
 
-from abc import ABC, abstractmethod
-from typing import Any, Dict, List
+import json
+from pathlib import Path
+from typing import Any, Dict, List, Optional
 
+from camel.storages.key_value_storages import BaseKeyValueStorage
+from camel.types import ModelType, OpenAIBackendRole, RoleType, TaskType
 
-class BaseKeyValueStorage(ABC):
-    r"""An abstract base class for key-value storage systems. Provides a
-    consistent interface for saving, loading, and clearing data records without
-    any loss of information.
-
-    An abstract base class designed to serve as a foundation for various
-    key-value storage systems. The class primarily interacts through Python
-    dictionaries.
-
-    This class is meant to be inherited by multiple types of key-value storage
-    implementations, including, but not limited to, JSON file storage, NoSQL
-    databases like MongoDB and Redis, as well as in-memory Python dictionaries.
+
+class _CamelJSONEncoder(json.JSONEncoder):
+    r"""A custom JSON encoder for serializing specifically enumerated types.
+    Ensures enumerated types can be stored in and retrieved from JSON format.
+    """
+    CAMEL_ENUMS = {
+        "RoleType": RoleType,
+        "TaskType": TaskType,
+        "ModelType": ModelType,
+        "OpenAIBackendRole": OpenAIBackendRole,
+    }
+
+    def default(self, obj) -> Any:
+        if type(obj) in self.CAMEL_ENUMS.values():
+            return {"__enum__": str(obj)}
+        # Let the base class default method raise the TypeError
+        return json.JSONEncoder.default(self, obj)
+
+
+class JsonStorage(BaseKeyValueStorage):
+    r"""A concrete implementation of the :obj:`BaseKeyValueStorage` using JSON
+    files. Allows for persistent storage of records in a human-readable format.
+
+    Args:
+        path (Path, optional): Path to the desired JSON file. If `None`, a
+            default path `./chat_history.json` will be used.
+            (default: :obj:`None`)
     """
 
-    @abstractmethod
+    def __init__(self, path: Optional[Path] = None) -> None:
+        self.json_path = path or Path("./chat_history.json")
+        self.json_path.touch()
+
+    def _json_object_hook(self, d) -> Any:
+        if "__enum__" in d:
+            name, member = d["__enum__"].split(".")
+            return getattr(_CamelJSONEncoder.CAMEL_ENUMS[name], member)
+        else:
+            return d
+
     def save(self, records: List[Dict[str, Any]]) -> None:
         r"""Saves a batch of records to the key-value storage system.
 
         Args:
             records (List[Dict[str, Any]]): A list of dictionaries, where each
                 dictionary represents a unique record to be stored.
         """
-        pass
+        with self.json_path.open("a") as f:
+            f.writelines(
+                [json.dumps(r, cls=_CamelJSONEncoder) + "\n" for r in records])
 
-    @abstractmethod
     def load(self) -> List[Dict[str, Any]]:
         r"""Loads all stored records from the key-value storage system.
 
         Returns:
             List[Dict[str, Any]]: A list of dictionaries, where each dictionary
                 represents a stored record.
         """
-        pass
+        with self.json_path.open("r") as f:
+            return [
+                json.loads(r, object_hook=self._json_object_hook)
+                for r in f.readlines()
+            ]
 
-    @abstractmethod
     def clear(self) -> None:
         r"""Removes all records from the key-value storage system.
         """
-        pass
+        with self.json_path.open("w"):
+            pass
```

### Comparing `camel_ai-0.1.1/camel/storages/key_value_storages/in_memory.py` & `camel_ai-0.1.2/camel/storages/key_value_storages/in_memory.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/storages/key_value_storages/json.py` & `camel_ai-0.1.2/camel/memories/blocks/vectordb_block.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,90 +8,90 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
 
-import json
-from pathlib import Path
-from typing import Any, Dict, List, Optional
-
-from camel.storages.key_value_storages import BaseKeyValueStorage
-from camel.types import (
-    ModelType,
-    OpenAIBackendRole,
-    RoleType,
-    TaskType,
-    VectorDistance,
+from typing import List, Optional
+
+from camel.embeddings import BaseEmbedding, OpenAIEmbedding
+from camel.memories import ContextRecord, MemoryBlock, MemoryRecord
+from camel.storages.vectordb_storages import (
+    BaseVectorStorage,
+    QdrantStorage,
+    VectorDBQuery,
+    VectorRecord,
 )
 
 
-class _CamelJSONEncoder(json.JSONEncoder):
-    r"""A custom JSON encoder for serializing specifically enumerated types.
-    Ensures enumerated types can be stored in and retrieved from JSON format.
-    """
-    CAMEL_ENUMS = {
-        "RoleType": RoleType,
-        "TaskType": TaskType,
-        "ModelType": ModelType,
-        "OpenAIBackendRole": OpenAIBackendRole,
-        "VectorDistance": VectorDistance,
-    }
-
-    def default(self, obj) -> Any:
-        if type(obj) in self.CAMEL_ENUMS.values():
-            return {"__enum__": str(obj)}
-        # Let the base class default method raise the TypeError
-        return json.JSONEncoder.default(self, obj)
-
-
-class JsonStorage(BaseKeyValueStorage):
-    r"""A concrete implementation of the :obj:`BaseKeyValueStorage` using JSON
-    files. Allows for persistent storage of records in a human-readable format.
+class VectorDBBlock(MemoryBlock):
+    r"""An implementation of the :obj:`MemoryBlock` abstract base class for
+    maintaining and retrieving information using vector embeddings within a
+    vector database.
 
     Args:
-        path (Path, optional): Path to the desired JSON file. If `None`, a
-            default path `./chat_history.json` will be used.
-            (default: :obj:`None`)
+        storage (Optional[BaseVectorStorage], optional): The storage mechanism
+            for the vector database. Defaults to in-memory :obj:`Qdrant` if not
+            provided. (default: :obj:`None`)
+        embedding (Optional[BaseEmbedding], optional): Embedding mechanism to
+            convert chat messages into vector representations. Defaults to
+            :obj:`OpenAiEmbedding` if not provided. (default: :obj:`None`)
     """
 
-    def __init__(self, path: Optional[Path] = None) -> None:
-        self.json_path = path or Path("./chat_history.json")
-        self.json_path.touch()
-
-    def _json_object_hook(self, d) -> Any:
-        if "__enum__" in d:
-            name, member = d["__enum__"].split(".")
-            return getattr(_CamelJSONEncoder.CAMEL_ENUMS[name], member)
-        else:
-            return d
-
-    def save(self, records: List[Dict[str, Any]]) -> None:
-        r"""Saves a batch of records to the key-value storage system.
+    def __init__(
+        self,
+        storage: Optional[BaseVectorStorage] = None,
+        embedding: Optional[BaseEmbedding] = None,
+    ) -> None:
+        self.embedding = embedding or OpenAIEmbedding()
+        self.vector_dim = self.embedding.get_output_dim()
+        self.storage = storage or QdrantStorage(vector_dim=self.vector_dim)
+
+    def retrieve(
+        self,
+        keyword: str,
+        limit: int = 3,
+    ) -> List[ContextRecord]:
+        r"""Retrieves similar records from the vector database based on the
+        content of the keyword.
 
         Args:
-            records (List[Dict[str, Any]]): A list of dictionaries, where each
-                dictionary represents a unique record to be stored.
+            keyword (str): This string will be converted into a vector
+                representation to query the database.
+            limit (int, optional): The maximum number of similar messages to
+                retrieve. (default: :obj:`3`).
+
+        Returns:
+            List[ContextRecord]: A list of memory records retrieved from the
+                vector database based on similarity to :obj:`current_state`.
         """
-        with self.json_path.open("a") as f:
-            f.writelines(
-                [json.dumps(r, cls=_CamelJSONEncoder) + "\n" for r in records])
+        query_vector = self.embedding.embed(keyword)
+        results = self.storage.query(VectorDBQuery(query_vector, top_k=limit))
+        return [
+            ContextRecord(
+                memory_record=MemoryRecord.from_dict(result.record.payload),
+                score=result.similarity,
+            ) for result in results if result.record.payload is not None
+        ]
 
-    def load(self) -> List[Dict[str, Any]]:
-        r"""Loads all stored records from the key-value storage system.
+    def write_records(self, records: List[MemoryRecord]) -> None:
+        """
+        Converts the provided chat messages into vector representations and
+        writes them to the vector database.
 
-        Returns:
-            List[Dict[str, Any]]: A list of dictionaries, where each dictionary
-                represents a stored record.
+        Args:
+            records (List[MemoryRecord]): Memory records to be added to the
+                memory.
         """
-        with self.json_path.open("r") as f:
-            return [
-                json.loads(r, object_hook=self._json_object_hook)
-                for r in f.readlines()
-            ]
+        v_records = [
+            VectorRecord(
+                vector=self.embedding.embed(record.message.content),
+                payload=record.to_dict(),
+                id=str(record.uuid),
+            ) for record in records
+        ]
+        self.storage.add(v_records)
 
     def clear(self) -> None:
-        r"""Removes all records from the key-value storage system.
-        """
-        with self.json_path.open("w"):
-            pass
+        r"""Removes all records from the vector database memory."""
+        self.storage.clear()
```

### Comparing `camel_ai-0.1.1/camel/terminators/__init__.py` & `camel_ai-0.1.2/camel/terminators/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/terminators/base.py` & `camel_ai-0.1.2/camel/terminators/base.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/terminators/response_terminator.py` & `camel_ai-0.1.2/camel/terminators/response_terminator.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/terminators/token_limit_terminator.py` & `camel_ai-0.1.2/camel/terminators/token_limit_terminator.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/types/__init__.py` & `camel_ai-0.1.2/camel/types/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     RoleType,
     ModelType,
     TaskType,
     TerminationMode,
     OpenAIBackendRole,
     EmbeddingModelType,
     VectorDistance,
+    StorageType,
 )
 from .openai_types import (
     Choice,
     ChatCompletion,
     ChatCompletionChunk,
     ChatCompletionMessage,
     ChatCompletionMessageParam,
@@ -37,14 +38,15 @@
     'RoleType',
     'ModelType',
     'TaskType',
     'TerminationMode',
     'OpenAIBackendRole',
     'EmbeddingModelType',
     'VectorDistance',
+    'StorageType',
     'Choice',
     'ChatCompletion',
     'ChatCompletionChunk',
     'ChatCompletionMessage',
     'ChatCompletionMessageParam',
     'ChatCompletionSystemMessageParam',
     'ChatCompletionUserMessageParam',
```

### Comparing `camel_ai-0.1.1/camel/types/enums.py` & `camel_ai-0.1.2/camel/types/enums.py`

 * *Files 18% similar despite different names*

```diff
@@ -155,22 +155,34 @@
     EVALUATION = "evaluation"
     SOLUTION_EXTRACTION = "solution_extraction"
     ROLE_DESCRIPTION = "role_description"
     DEFAULT = "default"
 
 
 class VectorDistance(Enum):
-    DOT = 1
-    COSINE = 2
-    EUCLIDEAN = 3
+    r"""Distance metrics used in a vector database."""
+
+    DOT = "dot"
+    r"""Dot product. https://en.wikipedia.org/wiki/Dot_product"""
+
+    COSINE = "cosine"
+    r"""Cosine similarity. https://en.wikipedia.org/wiki/Cosine_similarity"""
+
+    EUCLIDEAN = "euclidean"
+    r"""Euclidean distance. https://en.wikipedia.org/wiki/Euclidean_distance"""
 
 
 class OpenAIBackendRole(Enum):
     ASSISTANT = "assistant"
     SYSTEM = "system"
     USER = "user"
     FUNCTION = "function"
 
 
 class TerminationMode(Enum):
     ANY = "any"
     ALL = "all"
+
+
+class StorageType(Enum):
+    MILVUS = "milvus"
+    QDRANT = "qdrant"
```

### Comparing `camel_ai-0.1.1/camel/types/openai_types.py` & `camel_ai-0.1.2/camel/types/openai_types.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/camel/utils/__init__.py` & `camel_ai-0.1.2/camel/utils/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,41 +7,44 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an “AS IS” BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
-from .python_interpreter import PythonInterpreter
 from .commons import (
     openai_api_key_required,
     print_text_animated,
     get_prompt_template_key_words,
     get_first_int,
     download_tasks,
-    parse_doc,
     get_task_list,
     check_server_running,
+    role_playing_with_function,
+    get_system_information,
+    to_pascal,
+    PYDANTIC_V2,
 )
 from .token_counting import (
     get_model_encoding,
     BaseTokenCounter,
     OpenAITokenCounter,
     OpenSourceTokenCounter,
 )
 
 __all__ = [
-    'count_tokens_openai_chat_models',
     'openai_api_key_required',
     'print_text_animated',
     'get_prompt_template_key_words',
     'get_first_int',
     'download_tasks',
-    'PythonInterpreter',
-    'parse_doc',
     'get_task_list',
-    'get_model_encoding',
     'check_server_running',
+    'get_system_information',
+    'to_pascal',
+    'PYDANTIC_V2',
+    'get_model_encoding',
     'BaseTokenCounter',
     'OpenAITokenCounter',
     'OpenSourceTokenCounter',
+    'role_playing_with_function',
 ]
```

### Comparing `camel_ai-0.1.1/camel/utils/python_interpreter.py` & `camel_ai-0.1.2/camel/interpreters/internal_python_interpreter.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,28 +13,22 @@
 # =========== Copyright 2023 @ CAMEL-AI.org. All Rights Reserved. ===========
 import ast
 import difflib
 import importlib
 import typing
 from typing import Any, Dict, List, Optional
 
-
-class InterpreterError(ValueError):
-    r"""An error raised when the interpreter cannot evaluate a Python
-    expression, due to syntax error or unsupported operations.
-    """
-
-    pass
+from camel.interpreters import BaseInterpreter, InterpreterError
 
 
-class PythonInterpreter():
+class InternalPythonInterpreter(BaseInterpreter):
     r"""A customized python interpreter to control the execution of
     LLM-generated codes. The interpreter makes sure the code can only execute
     functions given in action space and import white list. It also supports
-    fuzzy variable matching to reveive uncertain input variable name.
+    fuzzy variable matching to retrieve uncertain input variable name.
 
     .. highlight:: none
 
     This class is adapted from the hugging face implementation
     `python_interpreter.py <https://github.com/huggingface/transformers/blob/8f
     093fb799246f7dd9104ff44728da0c53a9f67a/src/transformers/tools/python_interp
     reter.py>`_. The original license applies::
@@ -60,48 +54,104 @@
     have added import white list to keep `import` statement safe. Additionally,
     we have modified the variable matching logic and introduced the
     :obj:`fuzz_state` for fuzzy matching.
 
     Modifications copyright (C) 2023 CAMEL-AI.org
 
     Args:
-        action_space (Dict[str, Any]): A dictionary that maps action names to
-            their corresponding functions or objects. The interpreter can only
-            execute functions that are either directly listed in this
+        action_space (Dict[str, Any], optional): A dictionary that maps action
+            names to their corresponding functions or objects. The interpreter
+            can only execute functions that are either directly listed in this
             dictionary or are member functions of objects listed in this
             dictionary. The concept of :obj:`action_space` is derived from
             EmbodiedAgent, representing the actions that an agent is capable of
-            performing.
-        import_white_list (Optional[List[str]], optional): A list that stores
+            performing. If `None`, set to empty dict. (default: :obj:`None`)
+        import_white_list (List[str], optional): A list that stores
             the Python modules or functions that can be imported in the code.
             All submodules and functions of the modules listed in this list are
             importable. Any other import statements will be rejected. The
             module and its submodule or function name are separated by a period
             (:obj:`.`). (default: :obj:`None`)
+        unsafe_mode (bool, optional): If `True`, the interpreter runs the code
+            by `eval()` without any security check. (default: :obj:`False`)
+        raise_error (bool, optional): Raise error if the interpreter fails.
+            (default: :obj:`False`)
     """
 
-    def __init__(self, action_space: Dict[str, Any],
-                 import_white_list: Optional[List[str]] = None) -> None:
-        self.action_space = action_space
+    _CODE_TYPES = ["python", "py", "python3", "python2"]
+
+    def __init__(
+        self,
+        action_space: Optional[Dict[str, Any]] = None,
+        import_white_list: Optional[List[str]] = None,
+        unsafe_mode: bool = False,
+        raise_error: bool = False,
+    ) -> None:
+        self.action_space = action_space or dict()
         self.state = self.action_space.copy()
-        self.fuzz_state: Dict[str, Any] = {}
-        self.import_white_list = import_white_list or []
+        self.fuzz_state: Dict[str, Any] = dict()
+        self.import_white_list = import_white_list or list()
+        self.raise_error = raise_error
+        self.unsafe_mode = unsafe_mode
+
+    def run(self, code: str, code_type: str) -> str:
+        r"""Executes the given code with specified code type in the
+        interpreter.
+
+        This method takes a string of code and its type, checks if the code
+        type is supported, and then executes the code. If `unsafe_mode` is
+        set to `False`, the code is executed in a controlled environment using
+        the `execute` method. If `unsafe_mode` is `True`, the code is executed
+        using `eval()` with the action space as the global context. An
+        `InterpreterError` is raised if the code type is unsupported or if any
+        runtime error occurs during execution.
+
+        Args:
+            code (str): The python code to be executed.
+            code_type (str): The type of the code, which should be one of the
+            supported code types (`python`, `py`, `python3`, `python2`).
+
+
+        Returns:
+            str: The string representation of the output of the executed code.
+
+        Raises:
+            InterpreterError: If the `code_type` is not supported or if any
+                runtime error occurs during the execution of the code.
+    """
+        if code_type not in self._CODE_TYPES:
+            raise InterpreterError(
+                f"Unsupported code type {code_type}. "
+                f"`{self.__class__.__name__}` only supports "
+                f"{', '.join(self._CODE_TYPES)}.")
+        if not self.unsafe_mode:
+            return str(self.execute(code))
+        else:
+            return str(eval(code, self.action_space))
+
+    def update_action_space(self, action_space: Dict[str, Any]) -> None:
+        r"""Updates action space for *python* interpreter."""
+        self.action_space.update(action_space)
+
+    def supported_code_types(self) -> List[str]:
+        r"""Provides supported code types by the interpreter."""
+        return self._CODE_TYPES
 
     def execute(self, code: str, state: Optional[Dict[str, Any]] = None,
                 fuzz_state: Optional[Dict[str, Any]] = None,
                 keep_state: bool = True) -> Any:
-        r""" Execute the input python codes in a security environment.
+        r"""Execute the input python codes in a security environment.
 
         Args:
             code (str): Generated python code to be executed.
             state (Optional[Dict[str, Any]], optional): External variables that
                 may be used in the generated code. (default: :obj:`None`)
-            fuzz_state (Optional[Dict[str, Any]], optional): External varibles
-                that do not have certain varible names. The interpreter will
-                use fuzzy matching to access these varibales. For example, if
+            fuzz_state (Optional[Dict[str, Any]], optional): External variables
+                that do not have certain variable names. The interpreter will
+                use fuzzy matching to access these variables. For example, if
                 :obj:`fuzz_state` has a variable :obj:`image`, the generated
                 code can use :obj:`input_image` to access it. (default:
                 :obj:`None`)
             keep_state (bool, optional):  If :obj:`True`, :obj:`state` and
                 :obj:`fuzz_state` will be kept for later execution. Otherwise,
                 they will be cleared. (default: :obj:`True`)
 
@@ -116,38 +166,46 @@
             self.state.update(state)
         if fuzz_state is not None:
             self.fuzz_state.update(fuzz_state)
 
         try:
             expression = ast.parse(code)
         except SyntaxError as e:
-            raise InterpreterError(f"Syntax error in code: {e}")
+            if self.raise_error:
+                raise InterpreterError(f"Syntax error in code: {e}")
+            else:
+                import traceback
+                return traceback.format_exc()
 
         result = None
         for idx, node in enumerate(expression.body):
             try:
                 line_result = self._execute_ast(node)
             except InterpreterError as e:
                 if not keep_state:
                     self.clear_state()
                 msg = (f"Evaluation of the code stopped at node {idx}. "
                        f"See:\n{e}")
                 # More information can be provided by `ast.unparse()`,
                 # which is new in python 3.9.
-                raise InterpreterError(msg)
+                if self.raise_error:
+                    raise InterpreterError(msg)
+                else:
+                    import traceback
+                    return traceback.format_exc()
             if line_result is not None:
                 result = line_result
 
         if not keep_state:
             self.clear_state()
 
         return result
 
     def clear_state(self) -> None:
-        r"""Initialize :obj:`state` and :obj:`fuzz_state`"""
+        r"""Initialize :obj:`state` and :obj:`fuzz_state`."""
         self.state = self.action_space.copy()
         self.fuzz_state = {}
 
     # ast.Index is deprecated after python 3.9, which cannot pass type check,
     # but is still necessary for older versions.
     @typing.no_type_check
     def _execute_ast(self, expression: ast.AST) -> Any:
```

### Comparing `camel_ai-0.1.1/camel/utils/token_counting.py` & `camel_ai-0.1.2/camel/utils/token_counting.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.1/pyproject.toml` & `camel_ai-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "camel-ai"
-version = "0.1.1"
+version = "0.1.2"
 authors = ["CAMEL-AI.org"]
 description = "Communicative Agents for AI Society Study"
 readme = "README.md"
 keywords = [
     "communicative-ai",
     "ai-societies",
     "artificial-intelligence",
@@ -30,30 +30,46 @@
 python = ">=3.8.1,<3.12"
 numpy = "^1"
 openai = "^1.2.3"
 tiktoken = "^0"
 colorama = "^0"
 jsonschema = "^4"
 protobuf = "^4"
+pathlib = "^1.0.1"   
+docstring-parser = "^0.15"
+pydantic = ">=1.9,<3"
 
+# huggingface-agent
 transformers = { version = "^4", optional = true }
 diffusers = { version = "^0", optional = true }
 accelerate = { version = "^0", optional = true }
 datasets = { version = "^2", optional = true }
 torch = { version = "^1", optional = true }
 soundfile = { version = "^0", optional = true }
 sentencepiece = { version = "^0", optional = true }
 opencv-python = { version = "^4", optional = true }
+
+# tools
 beautifulsoup4 = { version = "^4", optional = true }
 docx2txt = { version = "^0.8", optional = true }
 PyMuPDF = { version = "^1.22.5", optional = true }
 wikipedia = { version = "^1", optional = true }
+wolframalpha = { version = "^5.0.0", optional = true }
 pyowm = { version = "^3.3.0", optional = true }
-unstructured = { version = "^0.10.30", optional = true }
-argilla = { version = "^1.19.0", optional = true }
+googlemaps = { version = "^4.10.0", optional = true }
+unstructured = { extras = ["all-docs"], version = "^0.10.30", optional = true }
+
+# encoders
+sentence-transformers = { version = "^2.2.2", optional = true }
+
+# vector-databases
+qdrant-client = { version = "^1.6.4", optional = true }
+pymilvus = { version = "^2.4.0", optional = true }
+
+# test
 pytest = { version = "^7", optional = true}
 mock = { version = "^5", optional = true}
 
 [tool.poetry.extras]
 test = ["pytest", "mock"]
 
 huggingface-agent = [
@@ -63,40 +79,58 @@
     "datasets",
     "torch",
     "soundfile",
     "sentencepiece",
     "opencv-python",
 ]
 
+encoders = [
+    "sentence-transformers",
+]
+
 tools = [
     "beautifulsoup4",
     "docx2txt",
     "PyMuPDF",
     "wikipedia",
+    "wolframalpha",
     "pyowm",
+    "googlemaps",
     "unstructured",
-    "argilla",
+]
+
+vector-databases = [
+    "qdrant-client",
+    "pymilvus",
 ]
 
 all = [
+    # huggingface-agent
     "transformers",
     "diffusers",
     "accelerate",
     "datasets",
     "torch",
     "soundfile",
     "sentencepiece",
     "opencv-python",
+    # tools
     "beautifulsoup4",
     "docx2txt",
     "PyMuPDF",
     "wikipedia",
+    "wolframalpha",
     "pyowm",
+    "googlemaps",
     "unstructured",
-    "argilla",
+    # vector-database
+    "qdrant-client",
+    "pymilvus",
+    # encoders
+    "sentence-transformers",
 ]
 
 [tool.poetry.group.dev]
 optional = true
 [tool.poetry.group.dev.dependencies]
 yapf = "0.32.0"
 isort = "5.12.0"
@@ -161,17 +195,21 @@
     "sqlalchemy",
     "google.cloud.sql.connector",
     "gradio",
     "database_connection",
     "huggingface_hub",
     "huggingface_hub.utils._errors",
     "wikipedia",
+    "wolframalpha",
     "pyowm",
+    "googlemaps",
     "jsonschema.*",
     "bs4.*",
     "docx2txt",
     "PyMuPDF",
     "fitz",
+    "qdrant_client.*",
     "unstructured.*",
-    "argilla.*",
+    "sentence_transformers.*",
+    "pymilvus",
 ]
 ignore_missing_imports = true
```

### Comparing `camel_ai-0.1.1/PKG-INFO` & `camel_ai-0.1.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,171 +1,175 @@
 Metadata-Version: 2.1
 Name: camel-ai
-Version: 0.1.1
+Version: 0.1.2
 Summary: Communicative Agents for AI Society Study
 Home-page: https://www.camel-ai.org/
 License: Apache-2.0
 Keywords: communicative-ai,ai-societies,artificial-intelligence,deep-learning,multi-agent-systems,cooperative-ai,natural-language-processing,large-language-models
 Author: CAMEL-AI.org
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
+Provides-Extra: encoders
 Provides-Extra: huggingface-agent
 Provides-Extra: test
 Provides-Extra: tools
+Provides-Extra: vector-databases
 Requires-Dist: PyMuPDF (>=1.22.5,<2.0.0) ; extra == "tools" or extra == "all"
 Requires-Dist: accelerate (>=0,<1) ; extra == "huggingface-agent" or extra == "all"
-Requires-Dist: argilla (>=1.19.0,<2.0.0) ; extra == "tools" or extra == "all"
 Requires-Dist: beautifulsoup4 (>=4,<5) ; extra == "tools" or extra == "all"
 Requires-Dist: colorama (>=0,<1)
 Requires-Dist: datasets (>=2,<3) ; extra == "huggingface-agent" or extra == "all"
 Requires-Dist: diffusers (>=0,<1) ; extra == "huggingface-agent" or extra == "all"
+Requires-Dist: docstring-parser (>=0.15,<0.16)
 Requires-Dist: docx2txt (>=0.8,<0.9) ; extra == "tools" or extra == "all"
+Requires-Dist: googlemaps (>=4.10.0,<5.0.0) ; extra == "tools" or extra == "all"
 Requires-Dist: jsonschema (>=4,<5)
 Requires-Dist: mock (>=5,<6) ; extra == "test"
 Requires-Dist: numpy (>=1,<2)
 Requires-Dist: openai (>=1.2.3,<2.0.0)
 Requires-Dist: opencv-python (>=4,<5) ; extra == "huggingface-agent" or extra == "all"
+Requires-Dist: pathlib (>=1.0.1,<2.0.0)
 Requires-Dist: protobuf (>=4,<5)
+Requires-Dist: pydantic (>=1.9,<3)
+Requires-Dist: pymilvus (>=2.4.0,<3.0.0) ; extra == "vector-databases" or extra == "all"
 Requires-Dist: pyowm (>=3.3.0,<4.0.0) ; extra == "tools" or extra == "all"
 Requires-Dist: pytest (>=7,<8) ; extra == "test"
+Requires-Dist: qdrant-client (>=1.6.4,<2.0.0) ; extra == "vector-databases" or extra == "all"
+Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0) ; extra == "encoders" or extra == "all"
 Requires-Dist: sentencepiece (>=0,<1) ; extra == "huggingface-agent" or extra == "all"
 Requires-Dist: soundfile (>=0,<1) ; extra == "huggingface-agent" or extra == "all"
 Requires-Dist: tiktoken (>=0,<1)
 Requires-Dist: torch (>=1,<2) ; extra == "huggingface-agent" or extra == "all"
 Requires-Dist: transformers (>=4,<5) ; extra == "huggingface-agent" or extra == "all"
-Requires-Dist: unstructured (>=0.10.30,<0.11.0) ; extra == "tools" or extra == "all"
+Requires-Dist: unstructured[all-docs] (>=0.10.30,<0.11.0) ; extra == "tools" or extra == "all"
 Requires-Dist: wikipedia (>=1,<2) ; extra == "tools" or extra == "all"
+Requires-Dist: wolframalpha (>=5.0.0,<6.0.0) ; extra == "tools" or extra == "all"
 Project-URL: Documentation, https://docs.camel-ai.org
 Project-URL: Repository, https://github.com/camel-ai/camel
 Description-Content-Type: text/markdown
 
-<div style="left">
-  <a href="https://colab.research.google.com/drive/1AzP33O8rnMW__7ocWJhVBXjKziJXPtim?usp=sharing" target="_blank">
-    <img alt="Open In Colab" src="https://colab.research.google.com/assets/colab-badge.svg" />
-  </a>
-  <a href="https://huggingface.co/camel-ai" target="_blank">
-    <img alt="Hugging Face" src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-CAMEL--AI-ffc107?color=ffc107&logoColor=white" />
-  </a>
-  <a href="https://join.slack.com/t/camel-kwr1314/shared_invite/zt-1vy8u9lbo-ZQmhIAyWSEfSwLCl2r2eKA" target="_blank">
-      <img alt="Slack" src="https://img.shields.io/badge/Slack-CAMEL--AI-blueviolet?logo=slack" />
-  </a>
-  <a href="https://discord.gg/CNcNpquyDc" target="_blank">
-    <img alt="Discord" src="https://img.shields.io/badge/Discord-CAMEL--AI-7289da?logo=discord&logoColor=white&color=7289da" />
-  </a>
-  <a href="https://ghli.org/camel/wechat.png" target="_blank">
-    <img alt="Discord" src="https://img.shields.io/badge/WeChat-CamelAIOrg-brightgreen?logo=wechat&logoColor=white" />
-  </a>
-  <a href="https://twitter.com/CamelAIOrg" target="_blank">
-    <img alt="Twitter Follow" src="https://img.shields.io/twitter/follow/CamelAIOrg?style=social&color=brightgreen&logo=twitter" />
-  </a>
-</div>
-
-# CAMEL: Communicative Agents for “Mind” Exploration of Large Scale Language Model Society
-
-<div align="center">
-
-  <a>![Python 3.9+](https://img.shields.io/badge/Python-3.9%2B-brightgreen.svg)</a>
-  <a href="https://github.com/camel-ai/camel/actions/workflows/pytest_package.yml">![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/camel-ai/camel/pytest_package.yml?label=tests&logo=github)</a>
-  <a href="https://camel-ai.github.io/camel/">
-    ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/camel-ai/camel/documentation.yaml?label=docs&logo=github)
-  </a>
-  <a href="https://github.com/camel-ai/camel/stargazers" target="_blank">
-  <img alt="GitHub Repo Stars" src="https://img.shields.io/github/stars/camel-ai/camel?label=stars&logo=github&color=brightgreen" />
-  </a>
-  <a href="https://github.com/camel-ai/camel/blob/master/licenses/LICENSE">![License](https://img.shields.io/github/license/camel-ai/camel?label=license&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjI0IiBoZWlnaHQ9IjI0IiBmaWxsPSIjZmZmZmZmIj48cGF0aCBmaWxsLXJ1bGU9ImV2ZW5vZGQiIGQ9Ik0xMi43NSAyLjc1YS43NS43NSAwIDAwLTEuNSAwVjQuNUg5LjI3NmExLjc1IDEuNzUgMCAwMC0uOTg1LjMwM0w2LjU5NiA1Ljk1N0EuMjUuMjUgMCAwMTYuNDU1IDZIMi4zNTNhLjc1Ljc1IDAgMTAwIDEuNUgzLjkzTC41NjMgMTUuMThhLjc2Mi43NjIgMCAwMC4yMS44OGMuMDguMDY0LjE2MS4xMjUuMzA5LjIyMS4xODYuMTIxLjQ1Mi4yNzguNzkyLjQzMy42OC4zMTEgMS42NjIuNjIgMi44NzYuNjJhNi45MTkgNi45MTkgMCAwMDIuODc2LS42MmMuMzQtLjE1NS42MDYtLjMxMi43OTItLjQzMy4xNS0uMDk3LjIzLS4xNTguMzEtLjIyM2EuNzUuNzUgMCAwMC4yMDktLjg3OEw1LjU2OSA3LjVoLjg4NmMuMzUxIDAgLjY5NC0uMTA2Ljk4NC0uMzAzbDEuNjk2LTEuMTU0QS4yNS4yNSAwIDAxOS4yNzUgNmgxLjk3NXYxNC41SDYuNzYzYS43NS43NSAwIDAwMCAxLjVoMTAuNDc0YS43NS43NSAwIDAwMC0xLjVIMTIuNzVWNmgxLjk3NGMuMDUgMCAuMS4wMTUuMTQuMDQzbDEuNjk3IDEuMTU0Yy4yOS4xOTcuNjMzLjMwMy45ODQuMzAzaC44ODZsLTMuMzY4IDcuNjhhLjc1Ljc1IDAgMDAuMjMuODk2Yy4wMTIuMDA5IDAgMCAuMDAyIDBhMy4xNTQgMy4xNTQgMCAwMC4zMS4yMDZjLjE4NS4xMTIuNDUuMjU2Ljc5LjRhNy4zNDMgNy4zNDMgMCAwMDIuODU1LjU2OCA3LjM0MyA3LjM0MyAwIDAwMi44NTYtLjU2OWMuMzM4LS4xNDMuNjA0LS4yODcuNzktLjM5OWEzLjUgMy41IDAgMDAuMzEtLjIwNi43NS43NSAwIDAwLjIzLS44OTZMMjAuMDcgNy41aDEuNTc4YS43NS43NSAwIDAwMC0xLjVoLTQuMTAyYS4yNS4yNSAwIDAxLS4xNC0uMDQzbC0xLjY5Ny0xLjE1NGExLjc1IDEuNzUgMCAwMC0uOTg0LS4zMDNIMTIuNzVWMi43NXpNMi4xOTMgMTUuMTk4YTUuNDE4IDUuNDE4IDAgMDAyLjU1Ny42MzUgNS40MTggNS40MTggMCAwMDIuNTU3LS42MzVMNC43NSA5LjM2OGwtMi41NTcgNS44M3ptMTQuNTEtLjAyNGMuMDgyLjA0LjE3NC4wODMuMjc1LjEyNi41My4yMjMgMS4zMDUuNDUgMi4yNzIuNDVhNS44NDYgNS44NDYgMCAwMDIuNTQ3LS41NzZMMTkuMjUgOS4zNjdsLTIuNTQ3IDUuODA3eiI+PC9wYXRoPjwvc3ZnPgo=)</a>
-</div>
+[![Colab][colab-image]][colab-url]
+[![Hugging Face][huggingface-image]][huggingface-url]
+[![Slack][slack-image]][slack-url]
+[![Discord][discord-image]][discord-url]
+[![Wechat][wechat-image]][wechat-url]
+[![Twitter][twitter-image]][twitter-url]
+
+______________________________________________________________________
+
+# CAMEL: Communicative Agents for “Mind” Exploration of Large Language Model Society
+
+[![Python Version][python-image]][python-url]
+[![PyTest Status][pytest-image]][pytest-url]
+[![Documentation][docs-image]][docs-url]
+[![Star][star-image]][star-url]
+[![Package License][package-license-image]][package-license-url]
+[![Data License][data-license-image]][data-license-url]
 
 <p align="center">
-   <a href="https://github.com/camel-ai/camel#community">Community</a> |
+  <a href="https://github.com/camel-ai/camel#community">Community</a> |
   <a href="https://github.com/camel-ai/camel#installation">Installation</a> |
   <a href="https://camel-ai.github.io/camel/">Documentation</a> |
   <a href="https://github.com/camel-ai/camel/tree/HEAD/examples">Examples</a> |
   <a href="https://arxiv.org/abs/2303.17760">Paper</a> |
   <a href="https://github.com/camel-ai/camel#citation">Citation</a> |
   <a href="https://github.com/camel-ai/camel#contributing-to-camel-">Contributing</a> |
   <a href="https://www.camel-ai.org/">CAMEL-AI</a>
 </p>
 
 <p align="center">
-  <img src='./misc/logo.png' width=800>
+  <img src='https://raw.githubusercontent.com/camel-ai/camel/master/misc/primary_logo.png' width=800>
 </p>
 
 ## Overview
 The rapid advancement of conversational and chat-based language models has led to remarkable progress in complex task-solving. However, their success heavily relies on human input to guide the conversation, which can be challenging and time-consuming. This paper explores the potential of building scalable techniques to facilitate autonomous cooperation among communicative agents and provide insight into their "cognitive" processes. To address the challenges of achieving autonomous cooperation, we propose a novel communicative agent framework named *role-playing*. Our approach involves using *inception prompting* to guide chat agents toward task completion while maintaining consistency with human intentions. We showcase how role-playing can be used to generate conversational data for studying the behaviors and capabilities of chat agents, providing a valuable resource for investigating conversational language models. Our contributions include introducing a novel communicative agent framework, offering a scalable approach for studying the cooperative behaviors and capabilities of multi-agent systems, and open-sourcing our library to support research on communicative agents and beyond. The GitHub repository of this project is made publicly available on: [https://github.com/camel-ai/camel](https://github.com/camel-ai/camel).
 
 ## Community
 🐫 CAMEL is an open-source library designed for the study of autonomous and communicative agents. We believe that studying these agents on a large scale offers valuable insights into their behaviors, capabilities, and potential risks. To facilitate research in this field, we implement and support various types of agents, tasks, prompts, models, and simulated environments.
 
-Join us ([*Slack*](https://join.slack.com/t/camel-kwr1314/shared_invite/zt-1vy8u9lbo-ZQmhIAyWSEfSwLCl2r2eKA), [*Discord*](https://discord.gg/CNcNpquyDc) or [*WeChat*](https://ghli.org/camel/wechat.png)) in pushing the boundaries of building AI Societiy.
+Join us ([*Slack*](https://join.slack.com/t/camel-kwr1314/shared_invite/zt-1vy8u9lbo-ZQmhIAyWSEfSwLCl2r2eKA), [*Discord*](https://discord.gg/CNcNpquyDc) or [*WeChat*](https://ghli.org/camel/wechat.png)) in pushing the boundaries of building AI Society.
 
 ## Try it yourself
 We provide a [![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1AzP33O8rnMW__7ocWJhVBXjKziJXPtim?usp=sharing) demo showcasing a conversation between two ChatGPT agents playing roles as a python programmer and a stock trader collaborating on developing a trading bot for stock market.
 
 <p align="center">
-  <img src='./misc/framework.png' width=800>
+  <img src='https://raw.githubusercontent.com/camel-ai/camel/master/misc/framework.png' width=800>
 </p>
 
-## Documentation
+## Installation
 
-[CAMEL package documentation pages](https://camel-ai.github.io/camel/)
+### From PyPI
 
-## Installation
+To install the base camel library, simply run `pip install camel-ai`
+
+Some features require extra dependencies.
+
+To use hugging-face agent, run `pip install camel-ai[huggingface-agent]`
+
+To enable RAG or use agent memory, run `pip install camel-ai[tools]`
+
+To install with all dependencies, run `pip install camel-ai[all]`
+
+### From Source
 
 Install `CAMEL` from source with poetry (Recommended):
 ```sh
+# Make sure your python version is later than 3.9
+# You can use pyenv to manage multiple python verisons in your sytstem
+
 # Clone github repo
-# For the latest code:
 git clone https://github.com/camel-ai/camel.git
-# Or for the stable code:
-git clone -b v0.1.0 https://github.com/camel-ai/camel.git
 
 # Change directory into project directory
 cd camel
 
 # Activate camel virtual environment
 poetry shell
 
 # Install camel from source
 # It takes about 90 seconds to resolve dependencies
 poetry install
 
-# Or if you want to use "huggingface agent"
-poetry install -E huggingface-agent # (Optional)
-
-# do something with camel
+# Or if you want to use all other extra packages
+poetry install -E all  # (Optional)
 
 # Exit the virtual environment
 exit
 ```
 
 Install `CAMEL` from source with conda and pip:
 ```sh
 # Create a conda virtual environment
 conda create --name camel python=3.10
 
 # Activate camel conda environment
 conda activate camel
 
 # Clone github repo
-git clone -b v0.1.0 https://github.com/camel-ai/camel.git
+git clone -b v0.1.2 https://github.com/camel-ai/camel.git
 
 # Change directory into project directory
 cd camel
 
 # Install camel from source
 pip install -e .
 
-# Or if you want to use "huggingface agent"
-pip install -e .[huggingface-agent] # (Optional)
+# Or if you want to use all other extra packages
+pip install -e .[all] # (Optional)
 ```
+
+## Documentation
+
+[CAMEL package documentation pages](https://camel-ai.github.io/camel/)
+
 ## Example
 You can find a list of tasks for different set of assistant and user role pairs [here](https://drive.google.com/file/d/194PPaSTBR07m-PzjS-Ty6KlPLdFIPQDd/view?usp=share_link)
 
 Run the `role_playing.py` script
 
 First, you need to add your OpenAI API key to system environment variables. The method to do this depends on your operating system and the shell you're using.
 
@@ -252,29 +256,29 @@
 
 - LLaMA2-based models
   - example: [meta-llama/Llama-2-7b-chat-hf](https://huggingface.co/meta-llama/Llama-2-7b-chat-hf)
 - Vicuna-based models
   - example: [lmsys/vicuna-7b-v1.5](https://huggingface.co/lmsys/vicuna-7b-v1.5)
 
 ## Data (Hosted on Hugging Face)
-| Dataset | Chat format | Instruction format | Chat format (translated) |
-| -- | -- | -- | -- |
+| Dataset        | Chat format                                                                                         | Instruction format                                                                                               | Chat format (translated)                                                                   |
+|----------------|-----------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------|
 | **AI Society** | [Chat format](https://huggingface.co/datasets/camel-ai/ai_society/blob/main/ai_society_chat.tar.gz) | [Instruction format](https://huggingface.co/datasets/camel-ai/ai_society/blob/main/ai_society_instructions.json) | [Chat format (translated)](https://huggingface.co/datasets/camel-ai/ai_society_translated) |
-| **Code** | [Chat format](https://huggingface.co/datasets/camel-ai/code/blob/main/code_chat.tar.gz) | [Instruction format](https://huggingface.co/datasets/camel-ai/code/blob/main/code_instructions.json) | x |
-| **Math** | [Chat format](https://huggingface.co/datasets/camel-ai/math) | x | x|
-| **Physics** | [Chat format](https://huggingface.co/datasets/camel-ai/physics) | x | x |
-| **Chemistry** | [Chat format](https://huggingface.co/datasets/camel-ai/chemistry) | x | x |
-| **Biology** | [Chat format](https://huggingface.co/datasets/camel-ai/biology) | x | x |
+| **Code**       | [Chat format](https://huggingface.co/datasets/camel-ai/code/blob/main/code_chat.tar.gz)             | [Instruction format](https://huggingface.co/datasets/camel-ai/code/blob/main/code_instructions.json)             | x                                                                                          |
+| **Math**       | [Chat format](https://huggingface.co/datasets/camel-ai/math)                                        | x                                                                                                                | x                                                                                          |
+| **Physics**    | [Chat format](https://huggingface.co/datasets/camel-ai/physics)                                     | x                                                                                                                | x                                                                                          |
+| **Chemistry**  | [Chat format](https://huggingface.co/datasets/camel-ai/chemistry)                                   | x                                                                                                                | x                                                                                          |
+| **Biology**    | [Chat format](https://huggingface.co/datasets/camel-ai/biology)                                     | x                                                                                                                | x                                                                                          |
 
 ## Visualizations of Instructions and Tasks
 
-| Dataset | Instructions | Tasks |
-| -- | -- | -- |
-| **AI Society** | [Instructions](https://atlas.nomic.ai/map/3a559a06-87d0-4476-a879-962656242452/db961915-b254-48e8-8e5c-917f827b74c6) | [Tasks](https://atlas.nomic.ai/map/cb96f41b-a6fd-4fe4-ac40-08e101714483/ae06156c-a572-46e9-8345-ebe18586d02b) |
-| **Code** | [Instructions](https://atlas.nomic.ai/map/902d6ccb-0bbb-4294-83a8-1c7d2dae03c8/ace2e146-e49f-41db-a1f4-25a2c4be2457) | [Tasks](https://atlas.nomic.ai/map/efc38617-9180-490a-8630-43a05b35d22d/2576addf-a133-45d5-89a9-6b067b6652dd) |
+| Dataset          | Instructions                                                                                                         | Tasks                                                                                                         |
+|------------------|----------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------|
+| **AI Society**   | [Instructions](https://atlas.nomic.ai/map/3a559a06-87d0-4476-a879-962656242452/db961915-b254-48e8-8e5c-917f827b74c6) | [Tasks](https://atlas.nomic.ai/map/cb96f41b-a6fd-4fe4-ac40-08e101714483/ae06156c-a572-46e9-8345-ebe18586d02b) |
+| **Code**         | [Instructions](https://atlas.nomic.ai/map/902d6ccb-0bbb-4294-83a8-1c7d2dae03c8/ace2e146-e49f-41db-a1f4-25a2c4be2457) | [Tasks](https://atlas.nomic.ai/map/efc38617-9180-490a-8630-43a05b35d22d/2576addf-a133-45d5-89a9-6b067b6652dd) |
 | **Misalignment** | [Instructions](https://atlas.nomic.ai/map/5c491035-a26e-4a05-9593-82ffb2c3ab40/2bd98896-894e-4807-9ed8-a203ccb14d5e) | [Tasks](https://atlas.nomic.ai/map/abc357dd-9c04-4913-9541-63e259d7ac1f/825139a4-af66-427c-9d0e-f36b5492ab3f) |
 
 ## Implemented Research Ideas from Other Works
 We implemented amazing research ideas from other works for you to build, compare and customize your agents. If you use any of these modules, please kindly cite the original works:
 - `TaskCreationAgent`, `TaskPrioritizationAgent` and `BabyAGI` from *Nakajima et al.*: [Task-Driven Autonomous Agent](https://yoheinakajima.com/task-driven-autonomous-agent-utilizing-gpt-4-pinecone-and-langchain-for-diverse-applications/). [[Example](https://github.com/camel-ai/camel/blob/master/examples/ai_society/babyagi_playing.py)]
 
 ## News
@@ -289,23 +293,47 @@
   booktitle={Thirty-seventh Conference on Neural Information Processing Systems},
   year={2023}
 }
 ```
 ## Acknowledgement
 Special thanks to [Nomic AI](https://home.nomic.ai/) for giving us extended access to their data set exploration tool (Atlas).
 
-We would also like to thank Haya Hammoud for designing the logo of our project.
+We would also like to thank Haya Hammoud for designing the initial logo of our project.
 
 ## License
 
-The intended purpose and licensing of CAMEL is solely for research use.
-
 The source code is licensed under Apache 2.0.
 
 The datasets are licensed under CC BY NC 4.0, which permits only non-commercial usage. It is advised that any models trained using the dataset should not be utilized for anything other than research purposes.
 
 ## Contributing to CAMEL 🐫
 We appreciate your interest in contributing to our open-source initiative. We provide a document of [contributing guidelines](https://github.com/camel-ai/camel/blob/master/CONTRIBUTING.md) which outlines the steps for contributing to CAMEL. Please refer to this guide to ensure smooth collaboration and successful contributions. 🤝🚀
 
 ## Contact
 For more information please contact camel.ai.team@gmail.com.
 
+[python-image]: https://img.shields.io/badge/Python-3.9%2B-brightgreen.svg
+[python-url]: https://docs.python.org/3.9/
+[pytest-image]: https://github.com/camel-ai/camel/actions/workflows/pytest_package.yml/badge.svg
+[pytest-url]: https://github.com/camel-ai/camel/actions/workflows/pytest_package.yml
+[docs-image]: https://img.shields.io/badge/Documentation-grey.svg?logo=github
+[docs-url]: https://camel-ai.github.io/camel/index.html
+[star-image]: https://img.shields.io/github/stars/camel-ai/camel?label=stars&logo=github&color=brightgreen
+[star-url]: https://github.com/camel-ai/camel/stargazers
+[package-license-image]: https://img.shields.io/badge/License-Apache_2.0-blue.svg
+[package-license-url]: https://github.com/camel-ai/camel/blob/master/licenses/LICENSE
+[data-license-image]: https://img.shields.io/badge/License-CC_BY--NC_4.0-lightgrey.svg
+[data-license-url]: https://github.com/camel-ai/camel/blob/master/licenses/DATA_LICENSE
+
+[colab-url]: https://colab.research.google.com/drive/1AzP33O8rnMW__7ocWJhVBXjKziJXPtim?usp=sharing
+[colab-image]: https://colab.research.google.com/assets/colab-badge.svg
+[huggingface-url]: https://huggingface.co/camel-ai
+[huggingface-image]: https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-CAMEL--AI-ffc107?color=ffc107&logoColor=white
+[slack-url]: https://join.slack.com/t/camel-kwr1314/shared_invite/zt-1vy8u9lbo-ZQmhIAyWSEfSwLCl2r2eKA
+[slack-image]: https://img.shields.io/badge/Slack-CAMEL--AI-blueviolet?logo=slack
+[discord-url]: https://discord.gg/CNcNpquyDc
+[discord-image]: https://img.shields.io/badge/Discord-CAMEL--AI-7289da?logo=discord&logoColor=white&color=7289da
+[wechat-url]: https://ghli.org/camel/wechat.png
+[wechat-image]: https://img.shields.io/badge/WeChat-CamelAIOrg-brightgreen?logo=wechat&logoColor=white
+[twitter-url]: https://twitter.com/CamelAIOrg
+[twitter-image]: https://img.shields.io/twitter/follow/CamelAIOrg?style=social&color=brightgreen&logo=twitter
+
```

#### html2text {}

```diff
@@ -1,52 +1,58 @@
-Metadata-Version: 2.1 Name: camel-ai Version: 0.1.1 Summary: Communicative
+Metadata-Version: 2.1 Name: camel-ai Version: 0.1.2 Summary: Communicative
 Agents for AI Society Study Home-page: https://www.camel-ai.org/ License:
 Apache-2.0 Keywords: communicative-ai,ai-societies,artificial-
 intelligence,deep-learning,multi-agent-systems,cooperative-ai,natural-language-
 processing,large-language-models Author: CAMEL-AI.org Requires-Python:
 >=3.8.1,<3.12 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Provides-Extra: all
-Provides-Extra: huggingface-agent Provides-Extra: test Provides-Extra: tools
-Requires-Dist: PyMuPDF (>=1.22.5,<2.0.0) ; extra == "tools" or extra == "all"
-Requires-Dist: accelerate (>=0,<1) ; extra == "huggingface-agent" or extra ==
-"all" Requires-Dist: argilla (>=1.19.0,<2.0.0) ; extra == "tools" or extra ==
-"all" Requires-Dist: beautifulsoup4 (>=4,<5) ; extra == "tools" or extra ==
-"all" Requires-Dist: colorama (>=0,<1) Requires-Dist: datasets (>=2,<3) ; extra
-== "huggingface-agent" or extra == "all" Requires-Dist: diffusers (>=0,<1) ;
-extra == "huggingface-agent" or extra == "all" Requires-Dist: docx2txt
-(>=0.8,<0.9) ; extra == "tools" or extra == "all" Requires-Dist: jsonschema
-(>=4,<5) Requires-Dist: mock (>=5,<6) ; extra == "test" Requires-Dist: numpy
-(>=1,<2) Requires-Dist: openai (>=1.2.3,<2.0.0) Requires-Dist: opencv-python
-(>=4,<5) ; extra == "huggingface-agent" or extra == "all" Requires-Dist:
-protobuf (>=4,<5) Requires-Dist: pyowm (>=3.3.0,<4.0.0) ; extra == "tools" or
-extra == "all" Requires-Dist: pytest (>=7,<8) ; extra == "test" Requires-Dist:
-sentencepiece (>=0,<1) ; extra == "huggingface-agent" or extra == "all"
+Provides-Extra: encoders Provides-Extra: huggingface-agent Provides-Extra: test
+Provides-Extra: tools Provides-Extra: vector-databases Requires-Dist: PyMuPDF
+(>=1.22.5,<2.0.0) ; extra == "tools" or extra == "all" Requires-Dist:
+accelerate (>=0,<1) ; extra == "huggingface-agent" or extra == "all" Requires-
+Dist: beautifulsoup4 (>=4,<5) ; extra == "tools" or extra == "all" Requires-
+Dist: colorama (>=0,<1) Requires-Dist: datasets (>=2,<3) ; extra ==
+"huggingface-agent" or extra == "all" Requires-Dist: diffusers (>=0,<1) ; extra
+== "huggingface-agent" or extra == "all" Requires-Dist: docstring-parser
+(>=0.15,<0.16) Requires-Dist: docx2txt (>=0.8,<0.9) ; extra == "tools" or extra
+== "all" Requires-Dist: googlemaps (>=4.10.0,<5.0.0) ; extra == "tools" or
+extra == "all" Requires-Dist: jsonschema (>=4,<5) Requires-Dist: mock (>=5,<6)
+; extra == "test" Requires-Dist: numpy (>=1,<2) Requires-Dist: openai
+(>=1.2.3,<2.0.0) Requires-Dist: opencv-python (>=4,<5) ; extra == "huggingface-
+agent" or extra == "all" Requires-Dist: pathlib (>=1.0.1,<2.0.0) Requires-Dist:
+protobuf (>=4,<5) Requires-Dist: pydantic (>=1.9,<3) Requires-Dist: pymilvus
+(>=2.4.0,<3.0.0) ; extra == "vector-databases" or extra == "all" Requires-Dist:
+pyowm (>=3.3.0,<4.0.0) ; extra == "tools" or extra == "all" Requires-Dist:
+pytest (>=7,<8) ; extra == "test" Requires-Dist: qdrant-client (>=1.6.4,<2.0.0)
+; extra == "vector-databases" or extra == "all" Requires-Dist: sentence-
+transformers (>=2.2.2,<3.0.0) ; extra == "encoders" or extra == "all" Requires-
+Dist: sentencepiece (>=0,<1) ; extra == "huggingface-agent" or extra == "all"
 Requires-Dist: soundfile (>=0,<1) ; extra == "huggingface-agent" or extra ==
 "all" Requires-Dist: tiktoken (>=0,<1) Requires-Dist: torch (>=1,<2) ; extra ==
 "huggingface-agent" or extra == "all" Requires-Dist: transformers (>=4,<5) ;
-extra == "huggingface-agent" or extra == "all" Requires-Dist: unstructured
-(>=0.10.30,<0.11.0) ; extra == "tools" or extra == "all" Requires-Dist:
-wikipedia (>=1,<2) ; extra == "tools" or extra == "all" Project-URL:
+extra == "huggingface-agent" or extra == "all" Requires-Dist: unstructured[all-
+docs] (>=0.10.30,<0.11.0) ; extra == "tools" or extra == "all" Requires-Dist:
+wikipedia (>=1,<2) ; extra == "tools" or extra == "all" Requires-Dist:
+wolframalpha (>=5.0.0,<6.0.0) ; extra == "tools" or extra == "all" Project-URL:
 Documentation, https://docs.camel-ai.org Project-URL: Repository, https://
-github.com/camel-ai/camel Description-Content-Type: text/markdown
-_[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_[_H_u_g_g_i_n_g_ _F_a_c_e_]_[_S_l_a_c_k_]_[_D_i_s_c_o_r_d_]_[_D_i_s_c_o_r_d_]_[_T_w_i_t_t_e_r_ _F_o_l_l_o_w_]
-# CAMEL: Communicative Agents for âMindâ Exploration of Large Scale
-Language Model Society
- ![Python 3.9+](https://img.shields.io/badge/Python-3.9%2B-brightgreen.svg) _!
-_[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_/_s_t_a_t_u_s_/
- _c_a_m_e_l_-_a_i_/_c_a_m_e_l_/_p_y_t_e_s_t___p_a_c_k_a_g_e_._y_m_l_?_l_a_b_e_l_=_t_e_s_t_s_&_l_o_g_o_=_g_i_t_h_u_b_) _!_[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w
- _S_t_a_t_u_s_]_(_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_/_s_t_a_t_u_s_/_c_a_m_e_l_-_a_i_/_c_a_m_e_l_/
-_d_o_c_u_m_e_n_t_a_t_i_o_n_._y_a_m_l_?_l_a_b_e_l_=_d_o_c_s_&_l_o_g_o_=_g_i_t_h_u_b_)_ _[_G_i_t_H_u_b_ _R_e_p_o_ _S_t_a_r_s_]_!_[_L_i_c_e_n_s_e_]_(_h_t_t_p_s_:
- _/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_c_a_m_e_l_-_a_i_/_c_a_m_e_l_?_l_a_b_e_l_=_l_i_c_e_n_s_e_&_l_o_g_o_=_d_a_t_a_:_i_m_a_g_e_/
-_s_v_g_+_x_m_l_;_b_a_s_e_6_4_,_P_H_N_2_Z_y_B_4_b_W_x_u_c_z_0_i_a_H_R_0_c_D_o_v_L_3_d_3_d_y_5_3_M_y_5_v_c_m_c_v_M_j_A_w_M_C_9_z_d_m_c_i_I_H_Z_p_Z_X_d_C_b_3_g_9_I_j_A_g_M_C_A_y_N_C_A_y_N_C_I_g_d_2_l_k_d_G_g_9_I_j_I_0_I_i_B_o_Z_W_l_n_a_H_Q_9_I_j_I_0_I_i_B_m_a_W_x_s_P_S_I_j_Z_m_Z_m_Z_m_Z_m_I_j_4_8_c_G_F_0_a_C_B_m_a_W_x_s_L_X_J_1_b_G_U_9_I_m_V_2_Z_W_5_v_Z_G_Q_i_I_G_Q_9_I_k_0_x_M_i_4_3_N_S_A_y_L_j_c_1_Y_S_4_3_N_S_4_3_N_S_A_w_I_D_A_w_L_T_E_u_N_S_A_w_V_j_Q_u_N_U_g_5_L_j_I_3_N_m_E_x_L_j_c_1_I_D_E_u_N_z_U_g_M_C_A_w_M_C_0_u_O_T_g_1_L_j_M_w_M_0_w_2_L_j_U_5_N_i_A_1_L_j_k_1_N_0_E_u_M_j_U_u_M_j_U_g_M_C_A_w_M_T_Y_u_N_D_U_1_I_D_Z_I_M_i_4_z_N_T_N_h_L_j_c_1_L_j_c_1_I_D_A_g_M_T_A_w_I_D_E_u_N_U_g_z_L_j_k_z_T_C_4_1_N_j_M_g_M_T_U_u_M_T_h_h_L_j_c_2_M_i_4_3_N_j_I_g_M_C_A_w_M_C_4_y_M_S_4_4_O_G_M_u_M_D_g_u_M_D_Y_0_L_j_E_2_M_S_4_x_M_j_U_u_M_z_A_5_L_j_I_y_M_S_4_x_O_D_Y_u_M_T_I_x_L_j_Q_1_M_i_4_y_N_z_g_u_N_z_k_y_L_j_Q_z_M_y_4_2_O_C_4_z_M_T_E_g_M_S_4_2_N_j_I_u_N_j_I_g_M_i_4_4_N_z_Y_u_N_j_J_h_N_i_4_5_M_T_k_g_N_i_4_5_M_T_k_g_M_C_A_w_M_D_I_u_O_D_c_2_L_S_4_2_M_m_M_u_M_z_Q_t_L_j_E_1_N_S_4_2_M_D_Y_t_L_j_M_x_M_i_4_3_O_T_I_t_L_j_Q_z_M_y_4_x_N_S_0_u_M_D_k_3_L_j_I_z_L_S_4_x_N_T_g_u_M_z_E_t_L_j_I_y_M_2_E_u_N_z_U_u_N_z_U_g_M_C_A_w_M_C_4_y_M_D_k_t_L_j_g_3_O_E_w_1_L_j_U_2_O_S_A_3_L_j_V_o_L_j_g_4_N_m_M_u_M_z_U_x_I_D_A_g_L_j_Y_5_N_C_0_u_M_T_A_2_L_j_k_4_N_C_0_u_M_z_A_z_b_D_E_u_N_j_k_2_L_T_E_u_M_T_U_0_Q_S_4_y_N_S_4_y_N_S_A_w_I_D_A_x_O_S_4_y_N_z_U_g_N_m_g_x_L_j_k_3_N_X_Y_x_N_C_4_1_S_D_Y_u_N_z_Y_z_Y_S_4_3_N_S_4_3_N_S_A_w_I_D_A_w_M_C_A_x_L_j_V_o_M_T_A_u_N_D_c_0_Y_S_4_3_N_S_4_3_N_S_A_w_I_D_A_w_M_C_0_x_L_j_V_I_M_T_I_u_N_z_V_W_N_m_g_x_L_j_k_3_N_G_M_u_M_D_U_g_M_C_A_u_M_S_4_w_M_T_U_u_M_T_Q_u_M_D_Q_z_b_D_E_u_N_j_k_3_I_D_E_u_M_T_U_0_Y_y_4_y_O_S_4_x_O_T_c_u_N_j_M_z_L_j_M_w_M_y_4_5_O_D_Q_u_M_z_A_z_a_C_4_4_O_D_Z_s_L_T_M_u_M_z_Y_4_I_D_c_u_N_j_h_h_L_j_c_1_L_j_c_1_I_D_A_g_M_D_A_u_M_j_M_u_O_D_k_2_Y_y_4_w_M_T_I_u_M_D_A_5_I_D_A_g_M_C_A_u_M_D_A_y_I_D_B_h_M_y_4_x_N_T_Q_g_M_y_4_x_N_T_Q_g_M_C_A_w_M_C_4_z_M_S_4_y_M_D_Z_j_L_j_E_4_N_S_4_x_M_T_I_u_N_D_U_u_M_j_U_2_L_j_c_5_L_j_R_h_N_y_4_z_N_D_M_g_N_y_4_z_N_D_M_g_M_C_A_w_M_D_I_u_O_D_U_1_L_j_U_2_O_C_A_3_L_j_M_0_M_y_A_3_L_j_M_0_M_y_A_w_I_D_A_w_M_i_4_4_N_T_Y_t_L_j_U_2_O_W_M_u_M_z_M_4_L_S_4_x_N_D_M_u_N_j_A_0_L_S_4_y_O_D_c_u_N_z_k_t_L_j_M_5_O_W_E_z_L_j_U_g_M_y_4_1_I_D_A_g_M_D_A_u_M_z_E_t_L_j_I_w_N_i_4_3_N_S_4_3_N_S_A_w_I_D_A_w_L_j_I_z_L_S_4_4_O_T_Z_M_M_j_A_u_M_D_c_g_N_y_4_1_a_D_E_u_N_T_c_4_Y_S_4_3_N_S_4_3_N_S_A_w_I_D_A_w_M_C_0_x_L_j_V_o_L_T_Q_u_M_T_A_y_Y_S_4_y_N_S_4_y_N_S_A_w_I_D_A_x_L_S_4_x_N_C_0_u_M_D_Q_z_b_C_0_x_L_j_Y_5_N_y_0_x_L_j_E_1_N_G_E_x_L_j_c_1_I_D_E_u_N_z_U_g_M_C_A_w_M_C_0_u_O_T_g_0_L_S_4_z_M_D_N_I_M_T_I_u_N_z_V_W_M_i_4_3_N_X_p_N_M_i_4_x_O_T_M_g_M_T_U_u_M_T_k_4_Y_T_U_u_N_D_E_4_I_D_U_u_N_D_E_4_I_D_A_g_M_D_A_y_L_j_U_1_N_y_4_2_M_z_U_g_N_S_4_0_M_T_g_g_N_S_4_0_M_T_g_g_M_C_A_w_M_D_I_u_N_T_U_3_L_S_4_2_M_z_V_M_N_C_4_3_N_S_A_5_L_j_M_2_O_G_w_t_M_i_4_1_N_T_c_g_N_S_4_4_M_3_p_t_M_T_Q_u_N_T_E_t_L_j_A_y_N_G_M_u_M_D_g_y_L_j_A_0_L_j_E_3_N_C_4_w_O_D_M_u_M_j_c_1_L_j_E_y_N_i_4_1_M_y_4_y_M_j_M_g_M_S_4_z_M_D_U_u_N_D_U_g_M_i_4_y_N_z_I_u_N_D_V_h_N_S_4_4_N_D_Y_g_N_S_4_4_N_D_Y_g_M_C_A_w_M_D_I_u_N_T_Q_3_L_S_4_1_N_z_Z_M_M_T_k_u_M_j_U_g_O_S_4_z_N_j_d_s_L_T_I_u_N_T_Q_3_I_D_U_u_O_D_A_3_e_i_I_+_P_C_9_w_Y_X_R_o_P_j_w_v_c_3_Z_n_P_g_o_=_)
+github.com/camel-ai/camel Description-Content-Type: text/markdown [![Colab]
+[colab-image]][colab-url] [![Hugging Face][huggingface-image]][huggingface-url]
+[![Slack][slack-image]][slack-url] [![Discord][discord-image]][discord-url] [!
+[Wechat][wechat-image]][wechat-url] [![Twitter][twitter-image]][twitter-url]
+______________________________________________________________________ # CAMEL:
+Communicative Agents for âMindâ Exploration of Large Language Model Society
+[![Python Version][python-image]][python-url] [![PyTest Status][pytest-image]]
+[pytest-url] [![Documentation][docs-image]][docs-url] [![Star][star-image]]
+[star-url] [![Package License][package-license-image]][package-license-url] [!
+[Data License][data-license-image]][data-license-url]
    _C_o_m_m_u_n_i_t_y | _I_n_s_t_a_l_l_a_t_i_o_n | _D_o_c_u_m_e_n_t_a_t_i_o_n | _E_x_a_m_p_l_e_s | _P_a_p_e_r | _C_i_t_a_t_i_o_n |
                             _C_o_n_t_r_i_b_u_t_i_n_g | _C_A_M_E_L_-_A_I
-                               [./misc/logo.png]
+[https://raw.githubusercontent.com/camel-ai/camel/master/misc/primary_logo.png]
 ## Overview The rapid advancement of conversational and chat-based language
 models has led to remarkable progress in complex task-solving. However, their
 success heavily relies on human input to guide the conversation, which can be
 challenging and time-consuming. This paper explores the potential of building
 scalable techniques to facilitate autonomous cooperation among communicative
 agents and provide insight into their "cognitive" processes. To address the
 challenges of achieving autonomous cooperation, we propose a novel
@@ -65,38 +71,42 @@
 communicative agents. We believe that studying these agents on a large scale
 offers valuable insights into their behaviors, capabilities, and potential
 risks. To facilitate research in this field, we implement and support various
 types of agents, tasks, prompts, models, and simulated environments. Join us (
 [*Slack*](https://join.slack.com/t/camel-kwr1314/shared_invite/zt-1vy8u9lbo-
 ZQmhIAyWSEfSwLCl2r2eKA), [*Discord*](https://discord.gg/CNcNpquyDc) or
 [*WeChat*](https://ghli.org/camel/wechat.png)) in pushing the boundaries of
-building AI Societiy. ## Try it yourself We provide a [![Google Colab](https://
+building AI Society. ## Try it yourself We provide a [![Google Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1AzP33O8rnMW__7ocWJhVBXjKziJXPtim?usp=sharing)
 demo showcasing a conversation between two ChatGPT agents playing roles as a
 python programmer and a stock trader collaborating on developing a trading bot
 for stock market.
-                            [./misc/framework.png]
-## Documentation [CAMEL package documentation pages](https://camel-
-ai.github.io/camel/) ## Installation Install `CAMEL` from source with poetry
-(Recommended): ```sh # Clone github repo # For the latest code: git clone
-https://github.com/camel-ai/camel.git # Or for the stable code: git clone -
-b v0.1.0 https://github.com/camel-ai/camel.git # Change directory into project
-directory cd camel # Activate camel virtual environment poetry shell # Install
-camel from source # It takes about 90 seconds to resolve dependencies poetry
-install # Or if you want to use "huggingface agent" poetry install -
-E huggingface-agent # (Optional) # do something with camel # Exit the virtual
+ [https://raw.githubusercontent.com/camel-ai/camel/master/misc/framework.png]
+## Installation ### From PyPI To install the base camel library, simply run
+`pip install camel-ai` Some features require extra dependencies. To use
+hugging-face agent, run `pip install camel-ai[huggingface-agent]` To enable RAG
+or use agent memory, run `pip install camel-ai[tools]` To install with all
+dependencies, run `pip install camel-ai[all]` ### From Source Install `CAMEL`
+from source with poetry (Recommended): ```sh # Make sure your python version is
+later than 3.9 # You can use pyenv to manage multiple python verisons in your
+sytstem # Clone github repo git clone https://github.com/camel-ai/camel.git #
+Change directory into project directory cd camel # Activate camel virtual
+environment poetry shell # Install camel from source # It takes about 90
+seconds to resolve dependencies poetry install # Or if you want to use all
+other extra packages poetry install -E all # (Optional) # Exit the virtual
 environment exit ``` Install `CAMEL` from source with conda and pip: ```sh #
 Create a conda virtual environment conda create --name camel python=3.10 #
 Activate camel conda environment conda activate camel # Clone github repo git
-clone -b v0.1.0 https://github.com/camel-ai/camel.git # Change directory into
+clone -b v0.1.2 https://github.com/camel-ai/camel.git # Change directory into
 project directory cd camel # Install camel from source pip install -e . # Or if
-you want to use "huggingface agent" pip install -e .[huggingface-agent] #
-(Optional) ``` ## Example You can find a list of tasks for different set of
-assistant and user role pairs [here](https://drive.google.com/file/d/
+you want to use all other extra packages pip install -e .[all] # (Optional) ```
+## Documentation [CAMEL package documentation pages](https://camel-
+ai.github.io/camel/) ## Example You can find a list of tasks for different set
+of assistant and user role pairs [here](https://drive.google.com/file/d/
 194PPaSTBR07m-PzjS-Ty6KlPLdFIPQDd/view?usp=share_link) Run the
 `role_playing.py` script First, you need to add your OpenAI API key to system
 environment variables. The method to do this depends on your operating system
 and the shell you're using. **For Bash shell (Linux, macOS, Git Bash on
 Windows):** ```bash # Export your OpenAI API key export OPENAI_API_KEY=
 OPENAI_API_BASE_URL= #(Should you utilize an OpenAI proxy service, kindly
 specify this) ``` **For Windows Command Prompt:** ```cmd REM export your OpenAI
@@ -138,28 +148,35 @@
 ( model=model_type, model_config=OpenSourceConfig( model_path="meta-llama/
 Llama-2-7b-chat-hf", server_url="http://localhost:8000/v1", ), ) agent =
 ChatAgent( system_message, **agent_kwargs, ) ``` ### Supported Models - LLaMA2-
 based models - example: [meta-llama/Llama-2-7b-chat-hf](https://huggingface.co/
 meta-llama/Llama-2-7b-chat-hf) - Vicuna-based models - example: [lmsys/vicuna-
 7b-v1.5](https://huggingface.co/lmsys/vicuna-7b-v1.5) ## Data (Hosted on
 Hugging Face) | Dataset | Chat format | Instruction format | Chat format
-(translated) | | -- | -- | -- | -- | | **AI Society** | [Chat format](https://
+(translated) | |----------------|----------------------------------------------
+-------------------------------------------------------|-----------------------
+-------------------------------------------------------------------------------
+------------|------------------------------------------------------------------
+--------------------------| | **AI Society** | [Chat format](https://
 huggingface.co/datasets/camel-ai/ai_society/blob/main/ai_society_chat.tar.gz) |
 [Instruction format](https://huggingface.co/datasets/camel-ai/ai_society/blob/
 main/ai_society_instructions.json) | [Chat format (translated)](https://
 huggingface.co/datasets/camel-ai/ai_society_translated) | | **Code** | [Chat
 format](https://huggingface.co/datasets/camel-ai/code/blob/main/
 code_chat.tar.gz) | [Instruction format](https://huggingface.co/datasets/camel-
 ai/code/blob/main/code_instructions.json) | x | | **Math** | [Chat format]
-(https://huggingface.co/datasets/camel-ai/math) | x | x| | **Physics** | [Chat
+(https://huggingface.co/datasets/camel-ai/math) | x | x | | **Physics** | [Chat
 format](https://huggingface.co/datasets/camel-ai/physics) | x | x | |
 **Chemistry** | [Chat format](https://huggingface.co/datasets/camel-ai/
 chemistry) | x | x | | **Biology** | [Chat format](https://huggingface.co/
 datasets/camel-ai/biology) | x | x | ## Visualizations of Instructions and
-Tasks | Dataset | Instructions | Tasks | | -- | -- | -- | | **AI Society** |
+Tasks | Dataset | Instructions | Tasks | |------------------|------------------
+-------------------------------------------------------------------------------
+---------------------|---------------------------------------------------------
+------------------------------------------------------| | **AI Society** |
 [Instructions](https://atlas.nomic.ai/map/3a559a06-87d0-4476-a879-962656242452/
 db961915-b254-48e8-8e5c-917f827b74c6) | [Tasks](https://atlas.nomic.ai/map/
 cb96f41b-a6fd-4fe4-ac40-08e101714483/ae06156c-a572-46e9-8345-ebe18586d02b) | |
 **Code** | [Instructions](https://atlas.nomic.ai/map/902d6ccb-0bbb-4294-83a8-
 1c7d2dae03c8/ace2e146-e49f-41db-a1f4-25a2c4be2457) | [Tasks](https://
 atlas.nomic.ai/map/efc38617-9180-490a-8630-43a05b35d22d/2576addf-a133-45d5-
 89a9-6b067b6652dd) | | **Misalignment** | [Instructions](https://
@@ -178,18 +195,43 @@
 ``` @inproceedings{li2023camel, title={CAMEL: Communicative Agents for "Mind"
 Exploration of Large Language Model Society}, author={Li, Guohao and Hammoud,
 Hasan Abed Al Kader and Itani, Hani and Khizbullin, Dmitrii and Ghanem,
 Bernard}, booktitle={Thirty-seventh Conference on Neural Information Processing
 Systems}, year={2023} } ``` ## Acknowledgement Special thanks to [Nomic AI]
 (https://home.nomic.ai/) for giving us extended access to their data set
 exploration tool (Atlas). We would also like to thank Haya Hammoud for
-designing the logo of our project. ## License The intended purpose and
-licensing of CAMEL is solely for research use. The source code is licensed
-under Apache 2.0. The datasets are licensed under CC BY NC 4.0, which permits
-only non-commercial usage. It is advised that any models trained using the
-dataset should not be utilized for anything other than research purposes. ##
-Contributing to CAMEL ð« We appreciate your interest in contributing to our
-open-source initiative. We provide a document of [contributing guidelines]
+designing the initial logo of our project. ## License The source code is
+licensed under Apache 2.0. The datasets are licensed under CC BY NC 4.0, which
+permits only non-commercial usage. It is advised that any models trained using
+the dataset should not be utilized for anything other than research purposes.
+## Contributing to CAMEL ð« We appreciate your interest in contributing to
+our open-source initiative. We provide a document of [contributing guidelines]
 (https://github.com/camel-ai/camel/blob/master/CONTRIBUTING.md) which outlines
 the steps for contributing to CAMEL. Please refer to this guide to ensure
 smooth collaboration and successful contributions. ð¤ð ## Contact For more
-information please contact camel.ai.team@gmail.com.
+information please contact camel.ai.team@gmail.com. [python-image]: https://
+img.shields.io/badge/Python-3.9%2B-brightgreen.svg [python-url]: https://
+docs.python.org/3.9/ [pytest-image]: https://github.com/camel-ai/camel/actions/
+workflows/pytest_package.yml/badge.svg [pytest-url]: https://github.com/camel-
+ai/camel/actions/workflows/pytest_package.yml [docs-image]: https://
+img.shields.io/badge/Documentation-grey.svg?logo=github [docs-url]: https://
+camel-ai.github.io/camel/index.html [star-image]: https://img.shields.io/
+github/stars/camel-ai/camel?label=stars&logo=github&color=brightgreen [star-
+url]: https://github.com/camel-ai/camel/stargazers [package-license-image]:
+https://img.shields.io/badge/License-Apache_2.0-blue.svg [package-license-url]:
+https://github.com/camel-ai/camel/blob/master/licenses/LICENSE [data-license-
+image]: https://img.shields.io/badge/License-CC_BY--NC_4.0-lightgrey.svg [data-
+license-url]: https://github.com/camel-ai/camel/blob/master/licenses/
+DATA_LICENSE [colab-url]: https://colab.research.google.com/drive/
+1AzP33O8rnMW__7ocWJhVBXjKziJXPtim?usp=sharing [colab-image]: https://
+colab.research.google.com/assets/colab-badge.svg [huggingface-url]: https://
+huggingface.co/camel-ai [huggingface-image]: https://img.shields.io/badge/
+%F0%9F%A4%97%20Hugging%20Face-CAMEL--AI-ffc107?color=ffc107&logoColor=white
+[slack-url]: https://join.slack.com/t/camel-kwr1314/shared_invite/zt-1vy8u9lbo-
+ZQmhIAyWSEfSwLCl2r2eKA [slack-image]: https://img.shields.io/badge/Slack-CAMEL-
+-AI-blueviolet?logo=slack [discord-url]: https://discord.gg/CNcNpquyDc
+[discord-image]: https://img.shields.io/badge/Discord-CAMEL--AI-
+7289da?logo=discord&logoColor=white&color=7289da [wechat-url]: https://
+ghli.org/camel/wechat.png [wechat-image]: https://img.shields.io/badge/WeChat-
+CamelAIOrg-brightgreen?logo=wechat&logoColor=white [twitter-url]: https://
+twitter.com/CamelAIOrg [twitter-image]: https://img.shields.io/twitter/follow/
+CamelAIOrg?style=social&color=brightgreen&logo=twitter
```

