# Comparing `tmp/julep-0.2.8.tar.gz` & `tmp/julep-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "julep-0.2.8.tar", max compression
+gzip compressed data, was "julep-0.2.9.tar", max compression
```

## Comparing `julep-0.2.8.tar` & `julep-0.2.9.tar`

### file list

```diff
@@ -1,82 +1,105 @@
--rw-r--r--   0        0        0      121 2024-02-10 10:42:24.049214 julep-0.2.8/README.md
--rw-r--r--   0        0        0      326 2024-02-29 08:57:18.582002 julep-0.2.8/julep/__init__.py
--rw-r--r--   0        0        0     2667 2024-03-07 13:20:14.421168 julep-0.2.8/julep/api/__init__.py
--rw-r--r--   0        0        0   105258 2024-03-07 13:20:14.421168 julep-0.2.8/julep/api/client.py
--rw-r--r--   0        0        0      519 2024-03-07 07:10:29.082169 julep-0.2.8/julep/api/core/__init__.py
--rw-r--r--   0        0        0      440 2024-03-07 10:51:15.571790 julep-0.2.8/julep/api/core/api_error.py
--rw-r--r--   0        0        0      972 2024-03-07 07:10:29.082169 julep-0.2.8/julep/api/core/client_wrapper.py
--rw-r--r--   0        0        0     1069 2024-03-07 10:51:15.579789 julep-0.2.8/julep/api/core/datetime_utils.py
--rw-r--r--   0        0        0     3825 2024-03-07 10:51:15.647783 julep-0.2.8/julep/api/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-03-07 07:10:29.082169 julep-0.2.8/julep/api/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      164 2024-03-07 07:10:29.082169 julep-0.2.8/julep/api/environment.py
--rw-r--r--   0        0        0     4022 2024-03-07 13:20:14.421168 julep-0.2.8/julep/api/types/__init__.py
--rw-r--r--   0        0        0     1858 2024-03-07 13:20:14.421168 julep-0.2.8/julep/api/types/agent.py
--rw-r--r--   0        0        0     3189 2024-03-07 10:51:15.611786 julep-0.2.8/julep/api/types/agent_default_settings.py
--rw-r--r--   0        0        0     1883 2024-03-07 07:10:29.102170 julep-0.2.8/julep/api/types/agent_default_settings_preset.py
--rw-r--r--   0        0        0     1750 2024-03-07 10:51:15.599787 julep-0.2.8/julep/api/types/belief.py
--rw-r--r--   0        0        0     1675 2024-03-07 10:51:15.619786 julep-0.2.8/julep/api/types/chat_input_data.py
--rw-r--r--   0        0        0      251 2024-03-07 10:51:31.494532 julep-0.2.8/julep/api/types/chat_input_data_tool_choice.py
--rw-r--r--   0        0        0     1447 2024-03-07 10:51:15.595788 julep-0.2.8/julep/api/types/chat_ml_message.py
--rw-r--r--   0        0        0      901 2024-03-07 07:10:29.102170 julep-0.2.8/julep/api/types/chat_ml_message_role.py
--rw-r--r--   0        0        0     2118 2024-03-07 10:51:15.599787 julep-0.2.8/julep/api/types/chat_response.py
--rw-r--r--   0        0        0     1479 2024-03-07 07:10:29.094170 julep-0.2.8/julep/api/types/chat_response_finish_reason.py
--rw-r--r--   0        0        0     6263 2024-03-07 10:51:15.635784 julep-0.2.8/julep/api/types/chat_settings.py
--rw-r--r--   0        0        0     1803 2024-03-07 07:10:29.102170 julep-0.2.8/julep/api/types/chat_settings_preset.py
--rw-r--r--   0        0        0     2352 2024-03-07 10:51:15.595788 julep-0.2.8/julep/api/types/chat_settings_response_format.py
--rw-r--r--   0        0        0     1037 2024-03-07 10:51:15.583788 julep-0.2.8/julep/api/types/chat_settings_response_format_schema.py
--rw-r--r--   0        0        0      786 2024-03-07 07:10:29.090170 julep-0.2.8/julep/api/types/chat_settings_response_format_type.py
--rw-r--r--   0        0        0      152 2024-03-07 07:10:29.090170 julep-0.2.8/julep/api/types/chat_settings_stop.py
--rw-r--r--   0        0        0     1358 2024-03-07 10:51:15.591788 julep-0.2.8/julep/api/types/completion_usage.py
--rw-r--r--   0        0        0     1131 2024-03-07 13:20:14.421168 julep-0.2.8/julep/api/types/create_doc.py
--rw-r--r--   0        0        0     1329 2024-03-07 10:51:15.595788 julep-0.2.8/julep/api/types/create_tool_request.py
--rw-r--r--   0        0        0      646 2024-03-07 10:51:15.583788 julep-0.2.8/julep/api/types/create_tool_request_type.py
--rw-r--r--   0        0        0     1254 2024-03-07 13:20:14.421168 julep-0.2.8/julep/api/types/doc.py
--rw-r--r--   0        0        0     1029 2024-03-07 10:51:15.607787 julep-0.2.8/julep/api/types/entity.py
--rw-r--r--   0        0        0     1849 2024-03-07 10:51:15.623785 julep-0.2.8/julep/api/types/episode.py
--rw-r--r--   0        0        0     1159 2024-03-07 10:51:15.607787 julep-0.2.8/julep/api/types/function_call_option.py
--rw-r--r--   0        0        0     1493 2024-03-07 10:51:15.615786 julep-0.2.8/julep/api/types/function_def.py
--rw-r--r--   0        0        0      130 2024-03-07 07:10:29.102170 julep-0.2.8/julep/api/types/function_parameters.py
--rw-r--r--   0        0        0     1023 2024-03-07 10:51:15.611786 julep-0.2.8/julep/api/types/get_agent_docs_response.py
--rw-r--r--   0        0        0     1036 2024-03-07 10:51:15.615786 julep-0.2.8/julep/api/types/get_agent_memories_response.py
--rw-r--r--   0        0        0     1027 2024-03-07 10:51:15.615786 julep-0.2.8/julep/api/types/get_agent_tools_response.py
--rw-r--r--   0        0        0     1053 2024-03-07 10:51:15.619786 julep-0.2.8/julep/api/types/get_history_response.py
--rw-r--r--   0        0        0     1046 2024-03-07 10:51:15.619786 julep-0.2.8/julep/api/types/get_suggestions_response.py
--rw-r--r--   0        0        0     1022 2024-03-07 10:51:15.619786 julep-0.2.8/julep/api/types/get_user_docs_response.py
--rw-r--r--   0        0        0     1511 2024-03-07 10:51:15.631785 julep-0.2.8/julep/api/types/input_chat_ml_message.py
--rw-r--r--   0        0        0      926 2024-03-07 07:10:29.102170 julep-0.2.8/julep/api/types/input_chat_ml_message_role.py
--rw-r--r--   0        0        0     1224 2024-03-07 10:51:15.631785 julep-0.2.8/julep/api/types/instruction.py
--rw-r--r--   0        0        0     1819 2024-03-07 10:51:15.643784 julep-0.2.8/julep/api/types/job_status.py
--rw-r--r--   0        0        0     1361 2024-03-07 07:10:29.094170 julep-0.2.8/julep/api/types/job_status_state.py
--rw-r--r--   0        0        0     1010 2024-03-07 10:51:15.627785 julep-0.2.8/julep/api/types/list_agents_response.py
--rw-r--r--   0        0        0     1018 2024-03-07 10:51:15.627785 julep-0.2.8/julep/api/types/list_sessions_response.py
--rw-r--r--   0        0        0     1006 2024-03-07 10:51:15.631785 julep-0.2.8/julep/api/types/list_users_response.py
--rw-r--r--   0        0        0      211 2024-03-07 07:10:29.098170 julep-0.2.8/julep/api/types/memory.py
--rw-r--r--   0        0        0     1231 2024-03-07 10:51:15.635784 julep-0.2.8/julep/api/types/memory_access_options.py
--rw-r--r--   0        0        0     1240 2024-03-07 10:51:15.639784 julep-0.2.8/julep/api/types/named_tool_choice.py
--rw-r--r--   0        0        0     1040 2024-03-07 10:51:15.639784 julep-0.2.8/julep/api/types/named_tool_choice_function.py
--rw-r--r--   0        0        0     1143 2024-03-07 10:51:15.639784 julep-0.2.8/julep/api/types/resource_created_response.py
--rw-r--r--   0        0        0     1000 2024-03-07 10:51:15.639784 julep-0.2.8/julep/api/types/resource_deleted_response.py
--rw-r--r--   0        0        0     1143 2024-03-07 10:51:15.643784 julep-0.2.8/julep/api/types/resource_updated_response.py
--rw-r--r--   0        0        0     1780 2024-03-07 13:20:14.421168 julep-0.2.8/julep/api/types/session.py
--rw-r--r--   0        0        0     1502 2024-03-07 10:51:15.651783 julep-0.2.8/julep/api/types/suggestion.py
--rw-r--r--   0        0        0      546 2024-03-07 10:51:15.635784 julep-0.2.8/julep/api/types/suggestion_target.py
--rw-r--r--   0        0        0     1327 2024-03-07 10:51:15.655783 julep-0.2.8/julep/api/types/tool.py
--rw-r--r--   0        0        0       88 2024-03-07 07:10:29.094170 julep-0.2.8/julep/api/types/tool_choice_option.py
--rw-r--r--   0        0        0      607 2024-03-07 10:51:15.643784 julep-0.2.8/julep/api/types/tool_type.py
--rw-r--r--   0        0        0     1409 2024-03-07 13:20:14.421168 julep-0.2.8/julep/api/types/user.py
--rw-r--r--   0        0        0    11123 2024-02-29 13:58:39.962965 julep-0.2.8/julep/client.py
--rw-r--r--   0        0        0      277 2024-03-07 17:28:11.011345 julep-0.2.8/julep/env.py
--rw-r--r--   0        0        0        0 2024-02-10 10:42:24.053213 julep-0.2.8/julep/managers/__init__.py
--rw-r--r--   0        0        0    30946 2024-03-07 07:04:30.290309 julep-0.2.8/julep/managers/agent.py
--rw-r--r--   0        0        0     1015 2024-02-10 10:42:24.053213 julep-0.2.8/julep/managers/base.py
--rw-r--r--   0        0        0    20101 2024-03-07 07:04:30.290309 julep-0.2.8/julep/managers/doc.py
--rw-r--r--   0        0        0     7674 2024-02-10 10:42:24.053213 julep-0.2.8/julep/managers/memory.py
--rw-r--r--   0        0        0    43472 2024-03-07 07:04:30.290309 julep-0.2.8/julep/managers/session.py
--rw-r--r--   0        0        0    18487 2024-02-16 12:27:51.553366 julep-0.2.8/julep/managers/tool.py
--rw-r--r--   0        0        0     1297 2024-03-07 07:04:30.290309 julep-0.2.8/julep/managers/types.py
--rw-r--r--   0        0        0    18419 2024-03-07 07:04:30.294309 julep-0.2.8/julep/managers/user.py
--rw-r--r--   0        0        0     1115 2024-03-07 07:04:30.294309 julep-0.2.8/julep/managers/utils.py
--rw-r--r--   0        0        0        0 2024-02-29 13:58:39.962965 julep-0.2.8/julep/utils/__init__.py
--rw-r--r--   0        0        0    12819 2024-02-29 13:58:39.962965 julep-0.2.8/julep/utils/openai_patch.py
--rw-r--r--   0        0        0     1659 2024-03-07 17:29:05.271242 julep-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      923 1970-01-01 00:00:00.000000 julep-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      121 2024-02-10 10:42:24.049214 julep-0.2.9/README.md
+-rw-r--r--   0        0        0      326 2024-02-29 08:57:18.582002 julep-0.2.9/julep/__init__.py
+-rw-r--r--   0        0        0     4077 2024-03-14 08:00:14.081169 julep-0.2.9/julep/api/__init__.py
+-rw-r--r--   0        0        0   132894 2024-03-14 08:01:07.660220 julep-0.2.9/julep/api/client.py
+-rw-r--r--   0        0        0      519 2024-03-14 07:55:57.885744 julep-0.2.9/julep/api/core/__init__.py
+-rw-r--r--   0        0        0      440 2024-03-14 07:56:06.133596 julep-0.2.9/julep/api/core/api_error.py
+-rw-r--r--   0        0        0      972 2024-03-14 07:55:57.885744 julep-0.2.9/julep/api/core/client_wrapper.py
+-rw-r--r--   0        0        0     1069 2024-03-14 07:56:06.141595 julep-0.2.9/julep/api/core/datetime_utils.py
+-rw-r--r--   0        0        0     3825 2024-03-14 07:56:06.213594 julep-0.2.9/julep/api/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-03-14 07:55:57.885744 julep-0.2.9/julep/api/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      164 2024-03-14 07:55:57.889744 julep-0.2.9/julep/api/environment.py
+-rw-r--r--   0        0        0     6258 2024-03-14 08:00:14.085168 julep-0.2.9/julep/api/types/__init__.py
+-rw-r--r--   0        0        0     2026 2024-03-14 07:56:06.169595 julep-0.2.9/julep/api/types/agent.py
+-rw-r--r--   0        0        0     3189 2024-03-14 07:56:06.169595 julep-0.2.9/julep/api/types/agent_default_settings.py
+-rw-r--r--   0        0        0     1883 2024-03-14 07:55:57.909744 julep-0.2.9/julep/api/types/agent_default_settings_preset.py
+-rw-r--r--   0        0        0      988 2024-03-14 07:56:06.145595 julep-0.2.9/julep/api/types/agent_metadata.py
+-rw-r--r--   0        0        0     1675 2024-03-14 07:56:06.157595 julep-0.2.9/julep/api/types/chat_input_data.py
+-rw-r--r--   0        0        0      251 2024-03-14 08:00:14.085168 julep-0.2.9/julep/api/types/chat_input_data_tool_choice.py
+-rw-r--r--   0        0        0     1447 2024-03-14 07:56:06.157595 julep-0.2.9/julep/api/types/chat_ml_message.py
+-rw-r--r--   0        0        0      901 2024-03-14 07:55:57.913744 julep-0.2.9/julep/api/types/chat_ml_message_role.py
+-rw-r--r--   0        0        0     2118 2024-03-14 07:56:06.161595 julep-0.2.9/julep/api/types/chat_response.py
+-rw-r--r--   0        0        0     1479 2024-03-14 07:55:57.901744 julep-0.2.9/julep/api/types/chat_response_finish_reason.py
+-rw-r--r--   0        0        0     6401 2024-03-14 07:56:06.201594 julep-0.2.9/julep/api/types/chat_settings.py
+-rw-r--r--   0        0        0     1787 2024-03-14 07:55:57.913744 julep-0.2.9/julep/api/types/chat_settings_preset.py
+-rw-r--r--   0        0        0     2352 2024-03-14 07:56:06.157595 julep-0.2.9/julep/api/types/chat_settings_response_format.py
+-rw-r--r--   0        0        0     1037 2024-03-14 07:56:06.129596 julep-0.2.9/julep/api/types/chat_settings_response_format_schema.py
+-rw-r--r--   0        0        0      786 2024-03-14 07:55:57.897744 julep-0.2.9/julep/api/types/chat_settings_response_format_type.py
+-rw-r--r--   0        0        0      152 2024-03-14 07:55:57.893744 julep-0.2.9/julep/api/types/chat_settings_stop.py
+-rw-r--r--   0        0        0     1358 2024-03-14 07:56:06.149595 julep-0.2.9/julep/api/types/completion_usage.py
+-rw-r--r--   0        0        0     1001 2024-03-14 07:56:06.161595 julep-0.2.9/julep/api/types/create_agent_request_metadata.py
+-rw-r--r--   0        0        0     1295 2024-03-14 07:56:06.153595 julep-0.2.9/julep/api/types/create_doc.py
+-rw-r--r--   0        0        0      992 2024-03-14 07:56:06.149595 julep-0.2.9/julep/api/types/create_doc_metadata.py
+-rw-r--r--   0        0        0     1003 2024-03-14 07:56:06.149595 julep-0.2.9/julep/api/types/create_session_request_metadata.py
+-rw-r--r--   0        0        0     1329 2024-03-14 07:56:06.161595 julep-0.2.9/julep/api/types/create_tool_request.py
+-rw-r--r--   0        0        0      646 2024-03-14 07:56:06.141595 julep-0.2.9/julep/api/types/create_tool_request_type.py
+-rw-r--r--   0        0        0     1000 2024-03-14 07:56:06.157595 julep-0.2.9/julep/api/types/create_user_request_metadata.py
+-rw-r--r--   0        0        0     1399 2024-03-14 07:56:06.169595 julep-0.2.9/julep/api/types/doc.py
+-rw-r--r--   0        0        0      986 2024-03-14 07:56:06.161595 julep-0.2.9/julep/api/types/doc_metadata.py
+-rw-r--r--   0        0        0     1159 2024-03-14 07:56:06.165595 julep-0.2.9/julep/api/types/function_call_option.py
+-rw-r--r--   0        0        0     1493 2024-03-14 07:56:06.177595 julep-0.2.9/julep/api/types/function_def.py
+-rw-r--r--   0        0        0      130 2024-03-14 07:55:57.909744 julep-0.2.9/julep/api/types/function_parameters.py
+-rw-r--r--   0        0        0      485 2024-03-14 07:56:06.161595 julep-0.2.9/julep/api/types/get_agent_docs_request_order.py
+-rw-r--r--   0        0        0      570 2024-03-14 07:56:06.161595 julep-0.2.9/julep/api/types/get_agent_docs_request_sort_by.py
+-rw-r--r--   0        0        0     1023 2024-03-14 07:56:06.173595 julep-0.2.9/julep/api/types/get_agent_docs_response.py
+-rw-r--r--   0        0        0     1036 2024-03-14 07:56:06.177595 julep-0.2.9/julep/api/types/get_agent_memories_response.py
+-rw-r--r--   0        0        0     1027 2024-03-14 07:56:06.177595 julep-0.2.9/julep/api/types/get_agent_tools_response.py
+-rw-r--r--   0        0        0     1053 2024-03-14 07:56:06.181595 julep-0.2.9/julep/api/types/get_history_response.py
+-rw-r--r--   0        0        0     1046 2024-03-14 07:56:06.185595 julep-0.2.9/julep/api/types/get_suggestions_response.py
+-rw-r--r--   0        0        0      482 2024-03-14 07:56:06.173595 julep-0.2.9/julep/api/types/get_user_docs_request_order.py
+-rw-r--r--   0        0        0      567 2024-03-14 07:56:06.173595 julep-0.2.9/julep/api/types/get_user_docs_request_sort_by.py
+-rw-r--r--   0        0        0     1022 2024-03-14 07:56:06.181595 julep-0.2.9/julep/api/types/get_user_docs_response.py
+-rw-r--r--   0        0        0     1511 2024-03-14 07:56:06.201594 julep-0.2.9/julep/api/types/input_chat_ml_message.py
+-rw-r--r--   0        0        0     1063 2024-03-14 07:55:57.913744 julep-0.2.9/julep/api/types/input_chat_ml_message_role.py
+-rw-r--r--   0        0        0     1224 2024-03-14 07:56:06.185595 julep-0.2.9/julep/api/types/instruction.py
+-rw-r--r--   0        0        0     1819 2024-03-14 07:56:06.201594 julep-0.2.9/julep/api/types/job_status.py
+-rw-r--r--   0        0        0     1361 2024-03-14 07:55:57.901744 julep-0.2.9/julep/api/types/job_status_state.py
+-rw-r--r--   0        0        0      479 2024-03-14 07:56:06.177595 julep-0.2.9/julep/api/types/list_agents_request_order.py
+-rw-r--r--   0        0        0      564 2024-03-14 07:56:06.193595 julep-0.2.9/julep/api/types/list_agents_request_sort_by.py
+-rw-r--r--   0        0        0     1010 2024-03-14 07:56:06.189595 julep-0.2.9/julep/api/types/list_agents_response.py
+-rw-r--r--   0        0        0      485 2024-03-14 07:56:06.181595 julep-0.2.9/julep/api/types/list_sessions_request_order.py
+-rw-r--r--   0        0        0      570 2024-03-14 07:56:06.181595 julep-0.2.9/julep/api/types/list_sessions_request_sort_by.py
+-rw-r--r--   0        0        0     1018 2024-03-14 07:56:06.193595 julep-0.2.9/julep/api/types/list_sessions_response.py
+-rw-r--r--   0        0        0      476 2024-03-14 07:56:06.185595 julep-0.2.9/julep/api/types/list_users_request_order.py
+-rw-r--r--   0        0        0      561 2024-03-14 07:56:06.185595 julep-0.2.9/julep/api/types/list_users_request_sort_by.py
+-rw-r--r--   0        0        0     1006 2024-03-14 07:56:06.197595 julep-0.2.9/julep/api/types/list_users_response.py
+-rw-r--r--   0        0        0     2233 2024-03-14 07:56:06.221594 julep-0.2.9/julep/api/types/memory.py
+-rw-r--r--   0        0        0     1231 2024-03-14 08:00:14.085168 julep-0.2.9/julep/api/types/memory_access_options.py
+-rw-r--r--   0        0        0     4640 2024-03-14 07:55:57.913744 julep-0.2.9/julep/api/types/memory_emotions_item.py
+-rw-r--r--   0        0        0      550 2024-03-14 07:56:06.193595 julep-0.2.9/julep/api/types/memory_type.py
+-rw-r--r--   0        0        0     1240 2024-03-14 07:56:06.217594 julep-0.2.9/julep/api/types/named_tool_choice.py
+-rw-r--r--   0        0        0     1040 2024-03-14 07:56:06.209594 julep-0.2.9/julep/api/types/named_tool_choice_function.py
+-rw-r--r--   0        0        0     1000 2024-03-14 07:56:06.205594 julep-0.2.9/julep/api/types/patch_agent_request_metadata.py
+-rw-r--r--   0        0        0     1002 2024-03-14 07:56:06.205594 julep-0.2.9/julep/api/types/patch_session_request_metadata.py
+-rw-r--r--   0        0        0      999 2024-03-14 07:56:06.209594 julep-0.2.9/julep/api/types/patch_user_request_metadata.py
+-rw-r--r--   0        0        0     1143 2024-03-14 07:56:06.217594 julep-0.2.9/julep/api/types/resource_created_response.py
+-rw-r--r--   0        0        0     1000 2024-03-14 08:00:14.085168 julep-0.2.9/julep/api/types/resource_deleted_response.py
+-rw-r--r--   0        0        0     1143 2024-03-14 07:56:06.213594 julep-0.2.9/julep/api/types/resource_updated_response.py
+-rw-r--r--   0        0        0     1937 2024-03-14 07:56:06.225594 julep-0.2.9/julep/api/types/session.py
+-rw-r--r--   0        0        0      990 2024-03-14 07:56:06.217594 julep-0.2.9/julep/api/types/session_metadata.py
+-rw-r--r--   0        0        0     1502 2024-03-14 07:56:06.233594 julep-0.2.9/julep/api/types/suggestion.py
+-rw-r--r--   0        0        0      546 2024-03-14 07:56:06.213594 julep-0.2.9/julep/api/types/suggestion_target.py
+-rw-r--r--   0        0        0     1327 2024-03-14 07:56:06.225594 julep-0.2.9/julep/api/types/tool.py
+-rw-r--r--   0        0        0       88 2024-03-14 07:55:57.897744 julep-0.2.9/julep/api/types/tool_choice_option.py
+-rw-r--r--   0        0        0      607 2024-03-14 07:56:06.217594 julep-0.2.9/julep/api/types/tool_type.py
+-rw-r--r--   0        0        0     1001 2024-03-14 07:56:06.225594 julep-0.2.9/julep/api/types/update_agent_request_metadata.py
+-rw-r--r--   0        0        0     1003 2024-03-14 07:56:06.225594 julep-0.2.9/julep/api/types/update_session_request_metadata.py
+-rw-r--r--   0        0        0     1000 2024-03-14 07:56:06.229594 julep-0.2.9/julep/api/types/update_user_request_metadata.py
+-rw-r--r--   0        0        0     1557 2024-03-14 07:56:06.233594 julep-0.2.9/julep/api/types/user.py
+-rw-r--r--   0        0        0      987 2024-03-14 07:56:06.225594 julep-0.2.9/julep/api/types/user_metadata.py
+-rw-r--r--   0        0        0    11519 2024-03-14 08:00:32.588841 julep-0.2.9/julep/client.py
+-rw-r--r--   0        0        0      277 2024-03-09 05:49:53.102445 julep-0.2.9/julep/env.py
+-rw-r--r--   0        0        0        0 2024-02-10 10:42:24.053213 julep-0.2.9/julep/managers/__init__.py
+-rw-r--r--   0        0        0    31392 2024-03-14 05:13:36.947764 julep-0.2.9/julep/managers/agent.py
+-rw-r--r--   0        0        0     1015 2024-02-10 10:42:24.053213 julep-0.2.9/julep/managers/base.py
+-rw-r--r--   0        0        0    20539 2024-03-14 05:13:36.947764 julep-0.2.9/julep/managers/doc.py
+-rw-r--r--   0        0        0     7674 2024-02-10 10:42:24.053213 julep-0.2.9/julep/managers/memory.py
+-rw-r--r--   0        0        0    43912 2024-03-14 05:13:36.951764 julep-0.2.9/julep/managers/session.py
+-rw-r--r--   0        0        0    18487 2024-02-16 12:27:51.553366 julep-0.2.9/julep/managers/tool.py
+-rw-r--r--   0        0        0     1297 2024-03-09 05:49:53.102445 julep-0.2.9/julep/managers/types.py
+-rw-r--r--   0        0        0    18865 2024-03-14 05:13:36.951764 julep-0.2.9/julep/managers/user.py
+-rw-r--r--   0        0        0     1115 2024-03-09 05:49:53.102445 julep-0.2.9/julep/managers/utils.py
+-rw-r--r--   0        0        0        0 2024-03-09 05:49:53.102445 julep-0.2.9/julep/utils/__init__.py
+-rw-r--r--   0        0        0    12819 2024-03-09 05:49:53.102445 julep-0.2.9/julep/utils/openai_patch.py
+-rw-r--r--   0        0        0     1659 2024-03-14 08:33:37.007294 julep-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      974 1970-01-01 00:00:00.000000 julep-0.2.9/PKG-INFO
```

### Comparing `julep-0.2.8/julep/api/__init__.py` & `julep-0.2.9/julep/api/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,117 +1,163 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .types import (
     Agent,
     AgentDefaultSettings,
     AgentDefaultSettingsPreset,
-    Belief,
+    AgentMetadata,
     ChatInputData,
     ChatInputDataToolChoice,
     ChatMlMessage,
     ChatMlMessageRole,
     ChatResponse,
     ChatResponseFinishReason,
     ChatSettings,
     ChatSettingsPreset,
     ChatSettingsResponseFormat,
     ChatSettingsResponseFormatSchema,
     ChatSettingsResponseFormatType,
     ChatSettingsStop,
     CompletionUsage,
+    CreateAgentRequestMetadata,
     CreateDoc,
+    CreateDocMetadata,
+    CreateSessionRequestMetadata,
     CreateToolRequest,
     CreateToolRequestType,
+    CreateUserRequestMetadata,
     Doc,
-    Entity,
-    Episode,
+    DocMetadata,
     FunctionCallOption,
     FunctionDef,
     FunctionParameters,
+    GetAgentDocsRequestOrder,
+    GetAgentDocsRequestSortBy,
     GetAgentDocsResponse,
     GetAgentMemoriesResponse,
     GetAgentToolsResponse,
     GetHistoryResponse,
     GetSuggestionsResponse,
+    GetUserDocsRequestOrder,
+    GetUserDocsRequestSortBy,
     GetUserDocsResponse,
     InputChatMlMessage,
     InputChatMlMessageRole,
     Instruction,
     JobStatus,
     JobStatusState,
+    ListAgentsRequestOrder,
+    ListAgentsRequestSortBy,
     ListAgentsResponse,
+    ListSessionsRequestOrder,
+    ListSessionsRequestSortBy,
     ListSessionsResponse,
+    ListUsersRequestOrder,
+    ListUsersRequestSortBy,
     ListUsersResponse,
     Memory,
     MemoryAccessOptions,
+    MemoryEmotionsItem,
+    MemoryType,
     NamedToolChoice,
     NamedToolChoiceFunction,
+    PatchAgentRequestMetadata,
+    PatchSessionRequestMetadata,
+    PatchUserRequestMetadata,
     ResourceCreatedResponse,
     ResourceDeletedResponse,
     ResourceUpdatedResponse,
     Session,
+    SessionMetadata,
     Suggestion,
     SuggestionTarget,
     Tool,
     ToolChoiceOption,
     ToolType,
+    UpdateAgentRequestMetadata,
+    UpdateSessionRequestMetadata,
+    UpdateUserRequestMetadata,
     User,
+    UserMetadata,
 )
 from .environment import JulepApiEnvironment
 
 __all__ = [
     "Agent",
     "AgentDefaultSettings",
     "AgentDefaultSettingsPreset",
-    "Belief",
+    "AgentMetadata",
     "ChatInputData",
     "ChatInputDataToolChoice",
     "ChatMlMessage",
     "ChatMlMessageRole",
     "ChatResponse",
     "ChatResponseFinishReason",
     "ChatSettings",
     "ChatSettingsPreset",
     "ChatSettingsResponseFormat",
     "ChatSettingsResponseFormatSchema",
     "ChatSettingsResponseFormatType",
     "ChatSettingsStop",
     "CompletionUsage",
+    "CreateAgentRequestMetadata",
     "CreateDoc",
+    "CreateDocMetadata",
+    "CreateSessionRequestMetadata",
     "CreateToolRequest",
     "CreateToolRequestType",
+    "CreateUserRequestMetadata",
     "Doc",
-    "Entity",
-    "Episode",
+    "DocMetadata",
     "FunctionCallOption",
     "FunctionDef",
     "FunctionParameters",
+    "GetAgentDocsRequestOrder",
+    "GetAgentDocsRequestSortBy",
     "GetAgentDocsResponse",
     "GetAgentMemoriesResponse",
     "GetAgentToolsResponse",
     "GetHistoryResponse",
     "GetSuggestionsResponse",
+    "GetUserDocsRequestOrder",
+    "GetUserDocsRequestSortBy",
     "GetUserDocsResponse",
     "InputChatMlMessage",
     "InputChatMlMessageRole",
     "Instruction",
     "JobStatus",
     "JobStatusState",
     "JulepApiEnvironment",
+    "ListAgentsRequestOrder",
+    "ListAgentsRequestSortBy",
     "ListAgentsResponse",
+    "ListSessionsRequestOrder",
+    "ListSessionsRequestSortBy",
     "ListSessionsResponse",
+    "ListUsersRequestOrder",
+    "ListUsersRequestSortBy",
     "ListUsersResponse",
     "Memory",
     "MemoryAccessOptions",
+    "MemoryEmotionsItem",
+    "MemoryType",
     "NamedToolChoice",
     "NamedToolChoiceFunction",
+    "PatchAgentRequestMetadata",
+    "PatchSessionRequestMetadata",
+    "PatchUserRequestMetadata",
     "ResourceCreatedResponse",
     "ResourceDeletedResponse",
     "ResourceUpdatedResponse",
     "Session",
+    "SessionMetadata",
     "Suggestion",
     "SuggestionTarget",
     "Tool",
     "ToolChoiceOption",
     "ToolType",
+    "UpdateAgentRequestMetadata",
+    "UpdateSessionRequestMetadata",
+    "UpdateUserRequestMetadata",
     "User",
+    "UserMetadata",
 ]
```

### Comparing `julep-0.2.8/julep/api/client.py` & `julep-0.2.9/julep/api/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# type: ignore
 # This file was auto-generated by Fern from our API Definition.
 
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 import httpx
@@ -14,33 +15,52 @@
 from .types.agent import Agent
 from .types.agent_default_settings import AgentDefaultSettings
 from .types.chat_input_data_tool_choice import ChatInputDataToolChoice
 from .types.chat_response import ChatResponse
 from .types.chat_settings_preset import ChatSettingsPreset
 from .types.chat_settings_response_format import ChatSettingsResponseFormat
 from .types.chat_settings_stop import ChatSettingsStop
+from .types.create_agent_request_metadata import CreateAgentRequestMetadata
 from .types.create_doc import CreateDoc
+from .types.create_session_request_metadata import CreateSessionRequestMetadata
 from .types.create_tool_request import CreateToolRequest
+from .types.create_user_request_metadata import CreateUserRequestMetadata
 from .types.function_def import FunctionDef
+from .types.get_agent_docs_request_order import GetAgentDocsRequestOrder
+from .types.get_agent_docs_request_sort_by import GetAgentDocsRequestSortBy
 from .types.get_agent_docs_response import GetAgentDocsResponse
 from .types.get_agent_memories_response import GetAgentMemoriesResponse
 from .types.get_agent_tools_response import GetAgentToolsResponse
 from .types.get_history_response import GetHistoryResponse
 from .types.get_suggestions_response import GetSuggestionsResponse
+from .types.get_user_docs_request_order import GetUserDocsRequestOrder
+from .types.get_user_docs_request_sort_by import GetUserDocsRequestSortBy
 from .types.get_user_docs_response import GetUserDocsResponse
 from .types.input_chat_ml_message import InputChatMlMessage
 from .types.instruction import Instruction
 from .types.job_status import JobStatus
+from .types.list_agents_request_order import ListAgentsRequestOrder
+from .types.list_agents_request_sort_by import ListAgentsRequestSortBy
 from .types.list_agents_response import ListAgentsResponse
+from .types.list_sessions_request_order import ListSessionsRequestOrder
+from .types.list_sessions_request_sort_by import ListSessionsRequestSortBy
 from .types.list_sessions_response import ListSessionsResponse
+from .types.list_users_request_order import ListUsersRequestOrder
+from .types.list_users_request_sort_by import ListUsersRequestSortBy
 from .types.list_users_response import ListUsersResponse
+from .types.patch_agent_request_metadata import PatchAgentRequestMetadata
+from .types.patch_session_request_metadata import PatchSessionRequestMetadata
+from .types.patch_user_request_metadata import PatchUserRequestMetadata
 from .types.resource_created_response import ResourceCreatedResponse
 from .types.resource_updated_response import ResourceUpdatedResponse
 from .types.session import Session
 from .types.tool import Tool
+from .types.update_agent_request_metadata import UpdateAgentRequestMetadata
+from .types.update_session_request_metadata import UpdateSessionRequestMetadata
+from .types.update_user_request_metadata import UpdateUserRequestMetadata
 from .types.user import User
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
@@ -63,58 +83,85 @@
             api_key=api_key,
             httpx_client=httpx.Client(timeout=timeout)
             if httpx_client is None
             else httpx_client,
         )
 
     def list_sessions(
-        self, *, limit: typing.Optional[int] = None, offset: typing.Optional[int] = None
+        self,
+        *,
+        limit: typing.Optional[int] = None,
+        offset: typing.Optional[int] = None,
+        metadata_filter: typing.Optional[str] = None,
+        sort_by: typing.Optional[ListSessionsRequestSortBy] = None,
+        order: typing.Optional[ListSessionsRequestOrder] = None,
     ) -> ListSessionsResponse:
         """
-        List sessions created (use limit/offset pagination to get large number of sessions; sorted by descending order of `created_at`)
+        List sessions created (use limit/offset pagination to get large number of sessions; sorted by descending order of `created_at` by default)
 
         Parameters:
             - limit: typing.Optional[int]. Number of sessions to return
 
             - offset: typing.Optional[int]. Number of sessions to skip (sorted created_at descending order)
+
+            - metadata_filter: typing.Optional[str]. JSON object that should be used to filter objects by metadata
+
+            - sort_by: typing.Optional[ListSessionsRequestSortBy]. Which field to sort by: `created_at` or `updated_at`
+
+            - order: typing.Optional[ListSessionsRequestOrder]. Which order should the sort be: `asc` (ascending) or `desc` (descending)
         ---
         from julep.client import JulepApi
 
         client = JulepApi(
             api_key="YOUR_API_KEY",
         )
         client.list_sessions()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "sessions"),
-            params=remove_none_from_dict({"limit": limit, "offset": offset}),
+            params=remove_none_from_dict(
+                {
+                    "limit": limit,
+                    "offset": offset,
+                    "metadata_filter": metadata_filter,
+                    "sort_by": sort_by,
+                    "order": order,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=300,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ListSessionsResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_session(
-        self, *, user_id: str, agent_id: str, situation: typing.Optional[str] = OMIT
+        self,
+        *,
+        user_id: str,
+        agent_id: str,
+        situation: typing.Optional[str] = OMIT,
+        metadata: typing.Optional[CreateSessionRequestMetadata] = OMIT,
     ) -> ResourceCreatedResponse:
         """
         Create a session between an agent and a user
 
         Parameters:
             - user_id: str. User ID of user to associate with this session
 
             - agent_id: str. Agent ID of agent to associate with this session
 
             - situation: typing.Optional[str]. A specific situation that sets the background for this session
+
+            - metadata: typing.Optional[CreateSessionRequestMetadata]. Optional metadata
         ---
         from julep.client import JulepApi
 
         client = JulepApi(
             api_key="YOUR_API_KEY",
         )
         client.create_session(
@@ -124,14 +171,16 @@
         """
         _request: typing.Dict[str, typing.Any] = {
             "user_id": user_id,
             "agent_id": agent_id,
         }
         if situation is not OMIT:
             _request["situation"] = situation
+        if metadata is not OMIT:
+            _request["metadata"] = metadata
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "sessions"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=300,
         )
@@ -140,35 +189,55 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def list_users(
-        self, *, limit: typing.Optional[int] = None, offset: typing.Optional[int] = None
+        self,
+        *,
+        limit: typing.Optional[int] = None,
+        offset: typing.Optional[int] = None,
+        metadata_filter: typing.Optional[str] = None,
+        sort_by: typing.Optional[ListUsersRequestSortBy] = None,
+        order: typing.Optional[ListUsersRequestOrder] = None,
     ) -> ListUsersResponse:
         """
-        List users created (use limit/offset pagination to get large number of sessions; sorted by descending order of `created_at`)
+        List users created (use limit/offset pagination to get large number of sessions; sorted by descending order of `created_at` by default)
 
         Parameters:
             - limit: typing.Optional[int]. Number of items to return
 
             - offset: typing.Optional[int]. Number of items to skip (sorted created_at descending order)
+
+            - metadata_filter: typing.Optional[str]. JSON object that should be used to filter objects by metadata
+
+            - sort_by: typing.Optional[ListUsersRequestSortBy]. Which field to sort by: `created_at` or `updated_at`
+
+            - order: typing.Optional[ListUsersRequestOrder]. Which order should the sort be: `asc` (ascending) or `desc` (descending)
         ---
         from julep.client import JulepApi
 
         client = JulepApi(
             api_key="YOUR_API_KEY",
         )
         client.list_users()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "users"),
-            params=remove_none_from_dict({"limit": limit, "offset": offset}),
+            params=remove_none_from_dict(
+                {
+                    "limit": limit,
+                    "offset": offset,
+                    "metadata_filter": metadata_filter,
+                    "sort_by": sort_by,
+                    "order": order,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=300,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ListUsersResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -178,24 +247,27 @@
 
     def create_user(
         self,
         *,
         name: typing.Optional[str] = OMIT,
         about: typing.Optional[str] = OMIT,
         docs: typing.Optional[typing.List[CreateDoc]] = OMIT,
+        metadata: typing.Optional[CreateUserRequestMetadata] = OMIT,
     ) -> ResourceCreatedResponse:
         """
         Create a new user
 
         Parameters:
             - name: typing.Optional[str]. Name of the user
 
             - about: typing.Optional[str]. About the user
 
             - docs: typing.Optional[typing.List[CreateDoc]]. List of docs about user
+
+            - metadata: typing.Optional[CreateUserRequestMetadata]. Optional metadata
         ---
         from julep.client import JulepApi
 
         client = JulepApi(
             api_key="YOUR_API_KEY",
         )
         client.create_user()
@@ -203,14 +275,16 @@
         _request: typing.Dict[str, typing.Any] = {}
         if name is not OMIT:
             _request["name"] = name
         if about is not OMIT:
             _request["about"] = about
         if docs is not OMIT:
             _request["docs"] = docs
+        if metadata is not OMIT:
+            _request["metadata"] = metadata
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "users"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=300,
         )
@@ -219,35 +293,55 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def list_agents(
-        self, *, limit: typing.Optional[int] = None, offset: typing.Optional[int] = None
+        self,
+        *,
+        limit: typing.Optional[int] = None,
+        offset: typing.Optional[int] = None,
+        metadata_filter: typing.Optional[str] = None,
+        sort_by: typing.Optional[ListAgentsRequestSortBy] = None,
+        order: typing.Optional[ListAgentsRequestOrder] = None,
     ) -> ListAgentsResponse:
         """
-        List agents created (use limit/offset pagination to get large number of sessions; sorted by descending order of `created_at`)
+        List agents created (use limit/offset pagination to get large number of sessions; sorted by descending order of `created_at` by default)
 
         Parameters:
             - limit: typing.Optional[int]. Number of items to return
 
             - offset: typing.Optional[int]. Number of items to skip (sorted created_at descending order)
+
+            - metadata_filter: typing.Optional[str]. JSON object that should be used to filter objects by metadata
+
+            - sort_by: typing.Optional[ListAgentsRequestSortBy]. Which field to sort by: `created_at` or `updated_at`
+
+            - order: typing.Optional[ListAgentsRequestOrder]. Which order should the sort be: `asc` (ascending) or `desc` (descending)
         ---
         from julep.client import JulepApi
 
         client = JulepApi(
             api_key="YOUR_API_KEY",
         )
         client.list_agents()
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "agents"),
-            params=remove_none_from_dict({"limit": limit, "offset": offset}),
+            params=remove_none_from_dict(
+                {
+                    "limit": limit,
+                    "offset": offset,
+                    "metadata_filter": metadata_filter,
+                    "sort_by": sort_by,
+                    "order": order,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=300,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ListAgentsResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -255,63 +349,66 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_agent(
         self,
         *,
         name: str,
-        about: str,
+        about: typing.Optional[str] = OMIT,
         instructions: typing.Optional[typing.List[Instruction]] = OMIT,
         tools: typing.Optional[typing.List[CreateToolRequest]] = OMIT,
         default_settings: typing.Optional[AgentDefaultSettings] = OMIT,
-        model: str,
+        model: typing.Optional[str] = OMIT,
         docs: typing.Optional[typing.List[CreateDoc]] = OMIT,
+        metadata: typing.Optional[CreateAgentRequestMetadata] = OMIT,
     ) -> ResourceCreatedResponse:
         """
         Create a new agent
 
         Parameters:
             - name: str. Name of the agent
 
-            - about: str. About the agent
+            - about: typing.Optional[str]. About the agent
 
             - instructions: typing.Optional[typing.List[Instruction]]. List of instructions for the agent
 
             - tools: typing.Optional[typing.List[CreateToolRequest]]. A list of tools the model may call. Currently, only `function`s are supported as a tool. Use this to provide a list of functions the model may generate JSON inputs for.
 
             - default_settings: typing.Optional[AgentDefaultSettings]. Default model settings to start every session with
 
-            - model: str. Name of the model that the agent is supposed to use
+            - model: typing.Optional[str]. Name of the model that the agent is supposed to use
 
             - docs: typing.Optional[typing.List[CreateDoc]]. List of docs about agent
+
+            - metadata: typing.Optional[CreateAgentRequestMetadata]. Optional metadata
         ---
         from julep.client import JulepApi
 
         client = JulepApi(
             api_key="YOUR_API_KEY",
         )
         client.create_agent(
             name="name",
-            about="about",
-            model="model",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {
-            "name": name,
-            "about": about,
-            "model": model,
-        }
+        _request: typing.Dict[str, typing.Any] = {"name": name}
+        if about is not OMIT:
+            _request["about"] = about
         if instructions is not OMIT:
             _request["instructions"] = instructions
         if tools is not OMIT:
             _request["tools"] = tools
         if default_settings is not OMIT:
             _request["default_settings"] = default_settings
+        if model is not OMIT:
+            _request["model"] = model
         if docs is not OMIT:
             _request["docs"] = docs
+        if metadata is not OMIT:
+            _request["metadata"] = metadata
         _response = self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "agents"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=300,
         )
@@ -352,40 +449,50 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update_session(
-        self, session_id: str, *, situation: str
+        self,
+        session_id: str,
+        *,
+        situation: typing.Optional[str] = OMIT,
+        metadata: typing.Optional[UpdateSessionRequestMetadata] = OMIT,
     ) -> ResourceUpdatedResponse:
         """
 
 
         Parameters:
             - session_id: str.
 
-            - situation: str. Updated situation for this session
+            - situation: typing.Optional[str]. Updated situation for this session
+
+            - metadata: typing.Optional[UpdateSessionRequestMetadata]. Optional metadata
         ---
         from julep.client import JulepApi
 
         client = JulepApi(
             api_key="YOUR_API_KEY",
         )
         client.update_session(
             session_id="session_id",
-            situation="situation",
         )
         """
+        _request: typing.Dict[str, typing.Any] = {}
+        if situation is not OMIT:
+            _request["situation"] = situation
+        if metadata is not OMIT:
+            _request["metadata"] = metadata
         _response = self._client_wrapper.httpx_client.request(
             "PUT",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"sessions/{session_id}"
             ),
-            json=jsonable_encoder({"situation": situation}),
+            json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=300,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ResourceUpdatedResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -421,14 +528,62 @@
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    def patch_session(
+        self,
+        session_id: str,
+        *,
+        situation: typing.Optional[str] = OMIT,
+        metadata: typing.Optional[PatchSessionRequestMetadata] = OMIT,
+    ) -> ResourceUpdatedResponse:
+        """
+
+
+        Parameters:
+            - session_id: str.
+
+            - situation: typing.Optional[str]. Updated situation for this session
+
+            - metadata: typing.Optional[PatchSessionRequestMetadata]. Optional metadata
+        ---
+        from julep.client import JulepApi
+
+        client = JulepApi(
+            api_key="YOUR_API_KEY",
+        )
+        client.patch_session(
+            session_id="session_id",
+        )
+        """
+        _request: typing.Dict[str, typing.Any] = {}
+        if situation is not OMIT:
+            _request["situation"] = situation
+        if metadata is not OMIT:
+            _request["metadata"] = metadata
+        _response = self._client_wrapper.httpx_client.request(
+            "PATCH",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"sessions/{session_id}"
+            ),
+            json=jsonable_encoder(_request),
+            headers=self._client_wrapper.get_headers(),
+            timeout=300,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(ResourceUpdatedResponse, _response.json())  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
     def get_suggestions(
         self,
         session_id: str,
         *,
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
     ) -> GetSuggestionsResponse:
@@ -577,15 +732,15 @@
 
             - temperature: typing.Optional[float]. What sampling temperature to use, between 0 and 2. Higher values like 0.8 will make the output more random, while lower values like 0.2 will make it more focused and deterministic.
 
             - top_p: typing.Optional[float]. Defaults to 1 An alternative to sampling with temperature, called nucleus sampling, where the model considers the results of the tokens with top_p probability mass. So 0.1 means only the tokens comprising the top 10% probability mass are considered. We generally recommend altering this or temperature but not both.
 
             - min_p: typing.Optional[float]. Minimum probability compared to leading token to be considered
 
-            - preset: typing.Optional[ChatSettingsPreset]. Generation preset name (one of: problem_solving, conversational, fun, prose, creative, business, deterministic, code, multilingual)
+            - preset: typing.Optional[ChatSettingsPreset]. Generation preset name (problem_solving|conversational|fun|prose|creative|business|deterministic|code|multilingual)
 
             - recall: typing.Optional[bool]. Whether previous memories should be recalled or not
 
             - remember: typing.Optional[bool]. Whether this interaction should be recorded in memory or not
         ---
         from julep import InputChatMlMessage, InputChatMlMessageRole
         from julep.client import JulepApi
@@ -755,24 +910,27 @@
 
     def update_user(
         self,
         user_id: str,
         *,
         about: typing.Optional[str] = OMIT,
         name: typing.Optional[str] = OMIT,
+        metadata: typing.Optional[UpdateUserRequestMetadata] = OMIT,
     ) -> ResourceUpdatedResponse:
         """
 
 
         Parameters:
             - user_id: str.
 
             - about: typing.Optional[str]. About the user
 
             - name: typing.Optional[str]. Name of the user
+
+            - metadata: typing.Optional[UpdateUserRequestMetadata]. Optional metadata
         ---
         from julep.client import JulepApi
 
         client = JulepApi(
             api_key="YOUR_API_KEY",
         )
         client.update_user(
@@ -780,14 +938,16 @@
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if about is not OMIT:
             _request["about"] = about
         if name is not OMIT:
             _request["name"] = name
+        if metadata is not OMIT:
+            _request["metadata"] = metadata
         _response = self._client_wrapper.httpx_client.request(
             "PUT",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"users/{user_id}"
             ),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
@@ -829,14 +989,67 @@
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    def patch_user(
+        self,
+        user_id: str,
+        *,
+        about: typing.Optional[str] = OMIT,
+        name: typing.Optional[str] = OMIT,
+        metadata: typing.Optional[PatchUserRequestMetadata] = OMIT,
+    ) -> ResourceUpdatedResponse:
+        """
+
+
+        Parameters:
+            - user_id: str.
+
+            - about: typing.Optional[str]. About the user
+
+            - name: typing.Optional[str]. Name of the user
+
+            - metadata: typing.Optional[PatchUserRequestMetadata]. Optional metadata
+        ---
+        from julep.client import JulepApi
+
+        client = JulepApi(
+            api_key="YOUR_API_KEY",
+        )
+        client.patch_user(
+            user_id="user_id",
+        )
+        """
+        _request: typing.Dict[str, typing.Any] = {}
+        if about is not OMIT:
+            _request["about"] = about
+        if name is not OMIT:
+            _request["name"] = name
+        if metadata is not OMIT:
+            _request["metadata"] = metadata
+        _response = self._client_wrapper.httpx_client.request(
+            "PATCH",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"users/{user_id}"
+            ),
+            json=jsonable_encoder(_request),
+            headers=self._client_wrapper.get_headers(),
+            timeout=300,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(ResourceUpdatedResponse, _response.json())  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
     def get_agent(self, agent_id: str) -> Agent:
         """
 
 
         Parameters:
             - agent_id: str.
         ---
@@ -870,14 +1083,15 @@
         agent_id: str,
         *,
         about: typing.Optional[str] = OMIT,
         instructions: typing.Optional[typing.List[Instruction]] = OMIT,
         name: typing.Optional[str] = OMIT,
         model: typing.Optional[str] = OMIT,
         default_settings: typing.Optional[AgentDefaultSettings] = OMIT,
+        metadata: typing.Optional[UpdateAgentRequestMetadata] = OMIT,
     ) -> ResourceUpdatedResponse:
         """
 
 
         Parameters:
             - agent_id: str.
 
@@ -886,14 +1100,16 @@
             - instructions: typing.Optional[typing.List[Instruction]]. List of instructions for the agent
 
             - name: typing.Optional[str]. Name of the agent
 
             - model: typing.Optional[str]. Name of the model that the agent is supposed to use
 
             - default_settings: typing.Optional[AgentDefaultSettings]. Default model settings to start every session with
+
+            - metadata: typing.Optional[UpdateAgentRequestMetadata]. Optional metadata
         ---
         from julep.client import JulepApi
 
         client = JulepApi(
             api_key="YOUR_API_KEY",
         )
         client.update_agent(
@@ -907,14 +1123,16 @@
             _request["instructions"] = instructions
         if name is not OMIT:
             _request["name"] = name
         if model is not OMIT:
             _request["model"] = model
         if default_settings is not OMIT:
             _request["default_settings"] = default_settings
+        if metadata is not OMIT:
+            _request["metadata"] = metadata
         _response = self._client_wrapper.httpx_client.request(
             "PUT",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"agents/{agent_id}"
             ),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
@@ -956,30 +1174,107 @@
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    def patch_agent(
+        self,
+        agent_id: str,
+        *,
+        about: typing.Optional[str] = OMIT,
+        instructions: typing.Optional[typing.List[Instruction]] = OMIT,
+        name: typing.Optional[str] = OMIT,
+        model: typing.Optional[str] = OMIT,
+        default_settings: typing.Optional[AgentDefaultSettings] = OMIT,
+        metadata: typing.Optional[PatchAgentRequestMetadata] = OMIT,
+    ) -> ResourceUpdatedResponse:
+        """
+
+
+        Parameters:
+            - agent_id: str.
+
+            - about: typing.Optional[str]. About the agent
+
+            - instructions: typing.Optional[typing.List[Instruction]]. List of instructions for the agent
+
+            - name: typing.Optional[str]. Name of the agent
+
+            - model: typing.Optional[str]. Name of the model that the agent is supposed to use
+
+            - default_settings: typing.Optional[AgentDefaultSettings]. Default model settings to start every session with
+
+            - metadata: typing.Optional[PatchAgentRequestMetadata]. Optional metadata
+        ---
+        from julep.client import JulepApi
+
+        client = JulepApi(
+            api_key="YOUR_API_KEY",
+        )
+        client.patch_agent(
+            agent_id="agent_id",
+        )
+        """
+        _request: typing.Dict[str, typing.Any] = {}
+        if about is not OMIT:
+            _request["about"] = about
+        if instructions is not OMIT:
+            _request["instructions"] = instructions
+        if name is not OMIT:
+            _request["name"] = name
+        if model is not OMIT:
+            _request["model"] = model
+        if default_settings is not OMIT:
+            _request["default_settings"] = default_settings
+        if metadata is not OMIT:
+            _request["metadata"] = metadata
+        _response = self._client_wrapper.httpx_client.request(
+            "PATCH",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"agents/{agent_id}"
+            ),
+            json=jsonable_encoder(_request),
+            headers=self._client_wrapper.get_headers(),
+            timeout=300,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(ResourceUpdatedResponse, _response.json())  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
     def get_agent_docs(
         self,
         agent_id: str,
         *,
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
+        metadata_filter: typing.Optional[str] = None,
+        sort_by: typing.Optional[GetAgentDocsRequestSortBy] = None,
+        order: typing.Optional[GetAgentDocsRequestOrder] = None,
     ) -> GetAgentDocsResponse:
         """
         Sorted (created_at descending)
 
         Parameters:
             - agent_id: str.
 
             - limit: typing.Optional[int].
 
             - offset: typing.Optional[int].
+
+            - metadata_filter: typing.Optional[str]. JSON object that should be used to filter objects by metadata
+
+            - sort_by: typing.Optional[GetAgentDocsRequestSortBy]. Which field to sort by: `created_at` or `updated_at`
+
+            - order: typing.Optional[GetAgentDocsRequestOrder]. Which order should the sort be: `asc` (ascending) or `desc` (descending)
         ---
         from julep.client import JulepApi
 
         client = JulepApi(
             api_key="YOUR_API_KEY",
         )
         client.get_agent_docs(
@@ -987,15 +1282,23 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"agents/{agent_id}/docs"
             ),
-            params=remove_none_from_dict({"limit": limit, "offset": offset}),
+            params=remove_none_from_dict(
+                {
+                    "limit": limit,
+                    "offset": offset,
+                    "metadata_filter": metadata_filter,
+                    "sort_by": sort_by,
+                    "order": order,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=300,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GetAgentDocsResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -1047,24 +1350,33 @@
 
     def get_user_docs(
         self,
         user_id: str,
         *,
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
+        metadata_filter: typing.Optional[str] = None,
+        sort_by: typing.Optional[GetUserDocsRequestSortBy] = None,
+        order: typing.Optional[GetUserDocsRequestOrder] = None,
     ) -> GetUserDocsResponse:
         """
         Sorted (created_at descending)
 
         Parameters:
             - user_id: str.
 
             - limit: typing.Optional[int].
 
             - offset: typing.Optional[int].
+
+            - metadata_filter: typing.Optional[str]. JSON object that should be used to filter objects by metadata
+
+            - sort_by: typing.Optional[GetUserDocsRequestSortBy]. Which field to sort by: `created_at` or `updated_at`
+
+            - order: typing.Optional[GetUserDocsRequestOrder]. Which order should the sort be: `asc` (ascending) or `desc` (descending)
         ---
         from julep.client import JulepApi
 
         client = JulepApi(
             api_key="YOUR_API_KEY",
         )
         client.get_user_docs(
@@ -1072,15 +1384,23 @@
         )
         """
         _response = self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"users/{user_id}/docs"
             ),
-            params=remove_none_from_dict({"limit": limit, "offset": offset}),
+            params=remove_none_from_dict(
+                {
+                    "limit": limit,
+                    "offset": offset,
+                    "metadata_filter": metadata_filter,
+                    "sort_by": sort_by,
+                    "order": order,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=300,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GetUserDocsResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -1404,14 +1724,60 @@
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    def patch_agent_tool(
+        self, agent_id: str, tool_id: str, *, function: FunctionDef
+    ) -> ResourceUpdatedResponse:
+        """
+
+
+        Parameters:
+            - agent_id: str.
+
+            - tool_id: str.
+
+            - function: FunctionDef. Function definition and parameters
+        ---
+        from julep import FunctionDef
+        from julep.client import JulepApi
+
+        client = JulepApi(
+            api_key="YOUR_API_KEY",
+        )
+        client.patch_agent_tool(
+            agent_id="agent_id",
+            tool_id="tool_id",
+            function=FunctionDef(
+                name="name",
+                parameters={},
+            ),
+        )
+        """
+        _response = self._client_wrapper.httpx_client.request(
+            "PATCH",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"agents/{agent_id}/tools/{tool_id}",
+            ),
+            json=jsonable_encoder({"function": function}),
+            headers=self._client_wrapper.get_headers(),
+            timeout=300,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(ResourceUpdatedResponse, _response.json())  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
     def get_job_status(self, job_id: str) -> JobStatus:
         """
 
 
         Parameters:
             - job_id: str.
         ---
@@ -1456,58 +1822,85 @@
             api_key=api_key,
             httpx_client=httpx.AsyncClient(timeout=timeout)
             if httpx_client is None
             else httpx_client,
         )
 
     async def list_sessions(
-        self, *, limit: typing.Optional[int] = None, offset: typing.Optional[int] = None
+        self,
+        *,
+        limit: typing.Optional[int] = None,
+        offset: typing.Optional[int] = None,
+        metadata_filter: typing.Optional[str] = None,
+        sort_by: typing.Optional[ListSessionsRequestSortBy] = None,
+        order: typing.Optional[ListSessionsRequestOrder] = None,
     ) -> ListSessionsResponse:
         """
-        List sessions created (use limit/offset pagination to get large number of sessions; sorted by descending order of `created_at`)
+        List sessions created (use limit/offset pagination to get large number of sessions; sorted by descending order of `created_at` by default)
 
         Parameters:
             - limit: typing.Optional[int]. Number of sessions to return
 
             - offset: typing.Optional[int]. Number of sessions to skip (sorted created_at descending order)
+
+            - metadata_filter: typing.Optional[str]. JSON object that should be used to filter objects by metadata
+
+            - sort_by: typing.Optional[ListSessionsRequestSortBy]. Which field to sort by: `created_at` or `updated_at`
+
+            - order: typing.Optional[ListSessionsRequestOrder]. Which order should the sort be: `asc` (ascending) or `desc` (descending)
         ---
         from julep.client import AsyncJulepApi
 
         client = AsyncJulepApi(
             api_key="YOUR_API_KEY",
         )
         await client.list_sessions()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "sessions"),
-            params=remove_none_from_dict({"limit": limit, "offset": offset}),
+            params=remove_none_from_dict(
+                {
+                    "limit": limit,
+                    "offset": offset,
+                    "metadata_filter": metadata_filter,
+                    "sort_by": sort_by,
+                    "order": order,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=300,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ListSessionsResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create_session(
-        self, *, user_id: str, agent_id: str, situation: typing.Optional[str] = OMIT
+        self,
+        *,
+        user_id: str,
+        agent_id: str,
+        situation: typing.Optional[str] = OMIT,
+        metadata: typing.Optional[CreateSessionRequestMetadata] = OMIT,
     ) -> ResourceCreatedResponse:
         """
         Create a session between an agent and a user
 
         Parameters:
             - user_id: str. User ID of user to associate with this session
 
             - agent_id: str. Agent ID of agent to associate with this session
 
             - situation: typing.Optional[str]. A specific situation that sets the background for this session
+
+            - metadata: typing.Optional[CreateSessionRequestMetadata]. Optional metadata
         ---
         from julep.client import AsyncJulepApi
 
         client = AsyncJulepApi(
             api_key="YOUR_API_KEY",
         )
         await client.create_session(
@@ -1517,14 +1910,16 @@
         """
         _request: typing.Dict[str, typing.Any] = {
             "user_id": user_id,
             "agent_id": agent_id,
         }
         if situation is not OMIT:
             _request["situation"] = situation
+        if metadata is not OMIT:
+            _request["metadata"] = metadata
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "sessions"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=300,
         )
@@ -1533,35 +1928,55 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def list_users(
-        self, *, limit: typing.Optional[int] = None, offset: typing.Optional[int] = None
+        self,
+        *,
+        limit: typing.Optional[int] = None,
+        offset: typing.Optional[int] = None,
+        metadata_filter: typing.Optional[str] = None,
+        sort_by: typing.Optional[ListUsersRequestSortBy] = None,
+        order: typing.Optional[ListUsersRequestOrder] = None,
     ) -> ListUsersResponse:
         """
-        List users created (use limit/offset pagination to get large number of sessions; sorted by descending order of `created_at`)
+        List users created (use limit/offset pagination to get large number of sessions; sorted by descending order of `created_at` by default)
 
         Parameters:
             - limit: typing.Optional[int]. Number of items to return
 
             - offset: typing.Optional[int]. Number of items to skip (sorted created_at descending order)
+
+            - metadata_filter: typing.Optional[str]. JSON object that should be used to filter objects by metadata
+
+            - sort_by: typing.Optional[ListUsersRequestSortBy]. Which field to sort by: `created_at` or `updated_at`
+
+            - order: typing.Optional[ListUsersRequestOrder]. Which order should the sort be: `asc` (ascending) or `desc` (descending)
         ---
         from julep.client import AsyncJulepApi
 
         client = AsyncJulepApi(
             api_key="YOUR_API_KEY",
         )
         await client.list_users()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "users"),
-            params=remove_none_from_dict({"limit": limit, "offset": offset}),
+            params=remove_none_from_dict(
+                {
+                    "limit": limit,
+                    "offset": offset,
+                    "metadata_filter": metadata_filter,
+                    "sort_by": sort_by,
+                    "order": order,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=300,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ListUsersResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -1571,24 +1986,27 @@
 
     async def create_user(
         self,
         *,
         name: typing.Optional[str] = OMIT,
         about: typing.Optional[str] = OMIT,
         docs: typing.Optional[typing.List[CreateDoc]] = OMIT,
+        metadata: typing.Optional[CreateUserRequestMetadata] = OMIT,
     ) -> ResourceCreatedResponse:
         """
         Create a new user
 
         Parameters:
             - name: typing.Optional[str]. Name of the user
 
             - about: typing.Optional[str]. About the user
 
             - docs: typing.Optional[typing.List[CreateDoc]]. List of docs about user
+
+            - metadata: typing.Optional[CreateUserRequestMetadata]. Optional metadata
         ---
         from julep.client import AsyncJulepApi
 
         client = AsyncJulepApi(
             api_key="YOUR_API_KEY",
         )
         await client.create_user()
@@ -1596,14 +2014,16 @@
         _request: typing.Dict[str, typing.Any] = {}
         if name is not OMIT:
             _request["name"] = name
         if about is not OMIT:
             _request["about"] = about
         if docs is not OMIT:
             _request["docs"] = docs
+        if metadata is not OMIT:
+            _request["metadata"] = metadata
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "users"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=300,
         )
@@ -1612,35 +2032,55 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def list_agents(
-        self, *, limit: typing.Optional[int] = None, offset: typing.Optional[int] = None
+        self,
+        *,
+        limit: typing.Optional[int] = None,
+        offset: typing.Optional[int] = None,
+        metadata_filter: typing.Optional[str] = None,
+        sort_by: typing.Optional[ListAgentsRequestSortBy] = None,
+        order: typing.Optional[ListAgentsRequestOrder] = None,
     ) -> ListAgentsResponse:
         """
-        List agents created (use limit/offset pagination to get large number of sessions; sorted by descending order of `created_at`)
+        List agents created (use limit/offset pagination to get large number of sessions; sorted by descending order of `created_at` by default)
 
         Parameters:
             - limit: typing.Optional[int]. Number of items to return
 
             - offset: typing.Optional[int]. Number of items to skip (sorted created_at descending order)
+
+            - metadata_filter: typing.Optional[str]. JSON object that should be used to filter objects by metadata
+
+            - sort_by: typing.Optional[ListAgentsRequestSortBy]. Which field to sort by: `created_at` or `updated_at`
+
+            - order: typing.Optional[ListAgentsRequestOrder]. Which order should the sort be: `asc` (ascending) or `desc` (descending)
         ---
         from julep.client import AsyncJulepApi
 
         client = AsyncJulepApi(
             api_key="YOUR_API_KEY",
         )
         await client.list_agents()
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "agents"),
-            params=remove_none_from_dict({"limit": limit, "offset": offset}),
+            params=remove_none_from_dict(
+                {
+                    "limit": limit,
+                    "offset": offset,
+                    "metadata_filter": metadata_filter,
+                    "sort_by": sort_by,
+                    "order": order,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=300,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ListAgentsResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -1648,63 +2088,66 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create_agent(
         self,
         *,
         name: str,
-        about: str,
+        about: typing.Optional[str] = OMIT,
         instructions: typing.Optional[typing.List[Instruction]] = OMIT,
         tools: typing.Optional[typing.List[CreateToolRequest]] = OMIT,
         default_settings: typing.Optional[AgentDefaultSettings] = OMIT,
-        model: str,
+        model: typing.Optional[str] = OMIT,
         docs: typing.Optional[typing.List[CreateDoc]] = OMIT,
+        metadata: typing.Optional[CreateAgentRequestMetadata] = OMIT,
     ) -> ResourceCreatedResponse:
         """
         Create a new agent
 
         Parameters:
             - name: str. Name of the agent
 
-            - about: str. About the agent
+            - about: typing.Optional[str]. About the agent
 
             - instructions: typing.Optional[typing.List[Instruction]]. List of instructions for the agent
 
             - tools: typing.Optional[typing.List[CreateToolRequest]]. A list of tools the model may call. Currently, only `function`s are supported as a tool. Use this to provide a list of functions the model may generate JSON inputs for.
 
             - default_settings: typing.Optional[AgentDefaultSettings]. Default model settings to start every session with
 
-            - model: str. Name of the model that the agent is supposed to use
+            - model: typing.Optional[str]. Name of the model that the agent is supposed to use
 
             - docs: typing.Optional[typing.List[CreateDoc]]. List of docs about agent
+
+            - metadata: typing.Optional[CreateAgentRequestMetadata]. Optional metadata
         ---
         from julep.client import AsyncJulepApi
 
         client = AsyncJulepApi(
             api_key="YOUR_API_KEY",
         )
         await client.create_agent(
             name="name",
-            about="about",
-            model="model",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {
-            "name": name,
-            "about": about,
-            "model": model,
-        }
+        _request: typing.Dict[str, typing.Any] = {"name": name}
+        if about is not OMIT:
+            _request["about"] = about
         if instructions is not OMIT:
             _request["instructions"] = instructions
         if tools is not OMIT:
             _request["tools"] = tools
         if default_settings is not OMIT:
             _request["default_settings"] = default_settings
+        if model is not OMIT:
+            _request["model"] = model
         if docs is not OMIT:
             _request["docs"] = docs
+        if metadata is not OMIT:
+            _request["metadata"] = metadata
         _response = await self._client_wrapper.httpx_client.request(
             "POST",
             urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "agents"),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=300,
         )
@@ -1745,40 +2188,50 @@
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update_session(
-        self, session_id: str, *, situation: str
+        self,
+        session_id: str,
+        *,
+        situation: typing.Optional[str] = OMIT,
+        metadata: typing.Optional[UpdateSessionRequestMetadata] = OMIT,
     ) -> ResourceUpdatedResponse:
         """
 
 
         Parameters:
             - session_id: str.
 
-            - situation: str. Updated situation for this session
+            - situation: typing.Optional[str]. Updated situation for this session
+
+            - metadata: typing.Optional[UpdateSessionRequestMetadata]. Optional metadata
         ---
         from julep.client import AsyncJulepApi
 
         client = AsyncJulepApi(
             api_key="YOUR_API_KEY",
         )
         await client.update_session(
             session_id="session_id",
-            situation="situation",
         )
         """
+        _request: typing.Dict[str, typing.Any] = {}
+        if situation is not OMIT:
+            _request["situation"] = situation
+        if metadata is not OMIT:
+            _request["metadata"] = metadata
         _response = await self._client_wrapper.httpx_client.request(
             "PUT",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"sessions/{session_id}"
             ),
-            json=jsonable_encoder({"situation": situation}),
+            json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
             timeout=300,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(ResourceUpdatedResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -1814,14 +2267,62 @@
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    async def patch_session(
+        self,
+        session_id: str,
+        *,
+        situation: typing.Optional[str] = OMIT,
+        metadata: typing.Optional[PatchSessionRequestMetadata] = OMIT,
+    ) -> ResourceUpdatedResponse:
+        """
+
+
+        Parameters:
+            - session_id: str.
+
+            - situation: typing.Optional[str]. Updated situation for this session
+
+            - metadata: typing.Optional[PatchSessionRequestMetadata]. Optional metadata
+        ---
+        from julep.client import AsyncJulepApi
+
+        client = AsyncJulepApi(
+            api_key="YOUR_API_KEY",
+        )
+        await client.patch_session(
+            session_id="session_id",
+        )
+        """
+        _request: typing.Dict[str, typing.Any] = {}
+        if situation is not OMIT:
+            _request["situation"] = situation
+        if metadata is not OMIT:
+            _request["metadata"] = metadata
+        _response = await self._client_wrapper.httpx_client.request(
+            "PATCH",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"sessions/{session_id}"
+            ),
+            json=jsonable_encoder(_request),
+            headers=self._client_wrapper.get_headers(),
+            timeout=300,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(ResourceUpdatedResponse, _response.json())  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
     async def get_suggestions(
         self,
         session_id: str,
         *,
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
     ) -> GetSuggestionsResponse:
@@ -1970,15 +2471,15 @@
 
             - temperature: typing.Optional[float]. What sampling temperature to use, between 0 and 2. Higher values like 0.8 will make the output more random, while lower values like 0.2 will make it more focused and deterministic.
 
             - top_p: typing.Optional[float]. Defaults to 1 An alternative to sampling with temperature, called nucleus sampling, where the model considers the results of the tokens with top_p probability mass. So 0.1 means only the tokens comprising the top 10% probability mass are considered. We generally recommend altering this or temperature but not both.
 
             - min_p: typing.Optional[float]. Minimum probability compared to leading token to be considered
 
-            - preset: typing.Optional[ChatSettingsPreset]. Generation preset name (one of: problem_solving, conversational, fun, prose, creative, business, deterministic, code, multilingual)
+            - preset: typing.Optional[ChatSettingsPreset]. Generation preset name (problem_solving|conversational|fun|prose|creative|business|deterministic|code|multilingual)
 
             - recall: typing.Optional[bool]. Whether previous memories should be recalled or not
 
             - remember: typing.Optional[bool]. Whether this interaction should be recorded in memory or not
         ---
         from julep import InputChatMlMessage, InputChatMlMessageRole
         from julep.client import AsyncJulepApi
@@ -2148,24 +2649,27 @@
 
     async def update_user(
         self,
         user_id: str,
         *,
         about: typing.Optional[str] = OMIT,
         name: typing.Optional[str] = OMIT,
+        metadata: typing.Optional[UpdateUserRequestMetadata] = OMIT,
     ) -> ResourceUpdatedResponse:
         """
 
 
         Parameters:
             - user_id: str.
 
             - about: typing.Optional[str]. About the user
 
             - name: typing.Optional[str]. Name of the user
+
+            - metadata: typing.Optional[UpdateUserRequestMetadata]. Optional metadata
         ---
         from julep.client import AsyncJulepApi
 
         client = AsyncJulepApi(
             api_key="YOUR_API_KEY",
         )
         await client.update_user(
@@ -2173,14 +2677,16 @@
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
         if about is not OMIT:
             _request["about"] = about
         if name is not OMIT:
             _request["name"] = name
+        if metadata is not OMIT:
+            _request["metadata"] = metadata
         _response = await self._client_wrapper.httpx_client.request(
             "PUT",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"users/{user_id}"
             ),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
@@ -2222,14 +2728,67 @@
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    async def patch_user(
+        self,
+        user_id: str,
+        *,
+        about: typing.Optional[str] = OMIT,
+        name: typing.Optional[str] = OMIT,
+        metadata: typing.Optional[PatchUserRequestMetadata] = OMIT,
+    ) -> ResourceUpdatedResponse:
+        """
+
+
+        Parameters:
+            - user_id: str.
+
+            - about: typing.Optional[str]. About the user
+
+            - name: typing.Optional[str]. Name of the user
+
+            - metadata: typing.Optional[PatchUserRequestMetadata]. Optional metadata
+        ---
+        from julep.client import AsyncJulepApi
+
+        client = AsyncJulepApi(
+            api_key="YOUR_API_KEY",
+        )
+        await client.patch_user(
+            user_id="user_id",
+        )
+        """
+        _request: typing.Dict[str, typing.Any] = {}
+        if about is not OMIT:
+            _request["about"] = about
+        if name is not OMIT:
+            _request["name"] = name
+        if metadata is not OMIT:
+            _request["metadata"] = metadata
+        _response = await self._client_wrapper.httpx_client.request(
+            "PATCH",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"users/{user_id}"
+            ),
+            json=jsonable_encoder(_request),
+            headers=self._client_wrapper.get_headers(),
+            timeout=300,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(ResourceUpdatedResponse, _response.json())  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
     async def get_agent(self, agent_id: str) -> Agent:
         """
 
 
         Parameters:
             - agent_id: str.
         ---
@@ -2263,14 +2822,15 @@
         agent_id: str,
         *,
         about: typing.Optional[str] = OMIT,
         instructions: typing.Optional[typing.List[Instruction]] = OMIT,
         name: typing.Optional[str] = OMIT,
         model: typing.Optional[str] = OMIT,
         default_settings: typing.Optional[AgentDefaultSettings] = OMIT,
+        metadata: typing.Optional[UpdateAgentRequestMetadata] = OMIT,
     ) -> ResourceUpdatedResponse:
         """
 
 
         Parameters:
             - agent_id: str.
 
@@ -2279,14 +2839,16 @@
             - instructions: typing.Optional[typing.List[Instruction]]. List of instructions for the agent
 
             - name: typing.Optional[str]. Name of the agent
 
             - model: typing.Optional[str]. Name of the model that the agent is supposed to use
 
             - default_settings: typing.Optional[AgentDefaultSettings]. Default model settings to start every session with
+
+            - metadata: typing.Optional[UpdateAgentRequestMetadata]. Optional metadata
         ---
         from julep.client import AsyncJulepApi
 
         client = AsyncJulepApi(
             api_key="YOUR_API_KEY",
         )
         await client.update_agent(
@@ -2300,14 +2862,16 @@
             _request["instructions"] = instructions
         if name is not OMIT:
             _request["name"] = name
         if model is not OMIT:
             _request["model"] = model
         if default_settings is not OMIT:
             _request["default_settings"] = default_settings
+        if metadata is not OMIT:
+            _request["metadata"] = metadata
         _response = await self._client_wrapper.httpx_client.request(
             "PUT",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"agents/{agent_id}"
             ),
             json=jsonable_encoder(_request),
             headers=self._client_wrapper.get_headers(),
@@ -2349,30 +2913,107 @@
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    async def patch_agent(
+        self,
+        agent_id: str,
+        *,
+        about: typing.Optional[str] = OMIT,
+        instructions: typing.Optional[typing.List[Instruction]] = OMIT,
+        name: typing.Optional[str] = OMIT,
+        model: typing.Optional[str] = OMIT,
+        default_settings: typing.Optional[AgentDefaultSettings] = OMIT,
+        metadata: typing.Optional[PatchAgentRequestMetadata] = OMIT,
+    ) -> ResourceUpdatedResponse:
+        """
+
+
+        Parameters:
+            - agent_id: str.
+
+            - about: typing.Optional[str]. About the agent
+
+            - instructions: typing.Optional[typing.List[Instruction]]. List of instructions for the agent
+
+            - name: typing.Optional[str]. Name of the agent
+
+            - model: typing.Optional[str]. Name of the model that the agent is supposed to use
+
+            - default_settings: typing.Optional[AgentDefaultSettings]. Default model settings to start every session with
+
+            - metadata: typing.Optional[PatchAgentRequestMetadata]. Optional metadata
+        ---
+        from julep.client import AsyncJulepApi
+
+        client = AsyncJulepApi(
+            api_key="YOUR_API_KEY",
+        )
+        await client.patch_agent(
+            agent_id="agent_id",
+        )
+        """
+        _request: typing.Dict[str, typing.Any] = {}
+        if about is not OMIT:
+            _request["about"] = about
+        if instructions is not OMIT:
+            _request["instructions"] = instructions
+        if name is not OMIT:
+            _request["name"] = name
+        if model is not OMIT:
+            _request["model"] = model
+        if default_settings is not OMIT:
+            _request["default_settings"] = default_settings
+        if metadata is not OMIT:
+            _request["metadata"] = metadata
+        _response = await self._client_wrapper.httpx_client.request(
+            "PATCH",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"agents/{agent_id}"
+            ),
+            json=jsonable_encoder(_request),
+            headers=self._client_wrapper.get_headers(),
+            timeout=300,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(ResourceUpdatedResponse, _response.json())  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
     async def get_agent_docs(
         self,
         agent_id: str,
         *,
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
+        metadata_filter: typing.Optional[str] = None,
+        sort_by: typing.Optional[GetAgentDocsRequestSortBy] = None,
+        order: typing.Optional[GetAgentDocsRequestOrder] = None,
     ) -> GetAgentDocsResponse:
         """
         Sorted (created_at descending)
 
         Parameters:
             - agent_id: str.
 
             - limit: typing.Optional[int].
 
             - offset: typing.Optional[int].
+
+            - metadata_filter: typing.Optional[str]. JSON object that should be used to filter objects by metadata
+
+            - sort_by: typing.Optional[GetAgentDocsRequestSortBy]. Which field to sort by: `created_at` or `updated_at`
+
+            - order: typing.Optional[GetAgentDocsRequestOrder]. Which order should the sort be: `asc` (ascending) or `desc` (descending)
         ---
         from julep.client import AsyncJulepApi
 
         client = AsyncJulepApi(
             api_key="YOUR_API_KEY",
         )
         await client.get_agent_docs(
@@ -2380,15 +3021,23 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"agents/{agent_id}/docs"
             ),
-            params=remove_none_from_dict({"limit": limit, "offset": offset}),
+            params=remove_none_from_dict(
+                {
+                    "limit": limit,
+                    "offset": offset,
+                    "metadata_filter": metadata_filter,
+                    "sort_by": sort_by,
+                    "order": order,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=300,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GetAgentDocsResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -2440,24 +3089,33 @@
 
     async def get_user_docs(
         self,
         user_id: str,
         *,
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
+        metadata_filter: typing.Optional[str] = None,
+        sort_by: typing.Optional[GetUserDocsRequestSortBy] = None,
+        order: typing.Optional[GetUserDocsRequestOrder] = None,
     ) -> GetUserDocsResponse:
         """
         Sorted (created_at descending)
 
         Parameters:
             - user_id: str.
 
             - limit: typing.Optional[int].
 
             - offset: typing.Optional[int].
+
+            - metadata_filter: typing.Optional[str]. JSON object that should be used to filter objects by metadata
+
+            - sort_by: typing.Optional[GetUserDocsRequestSortBy]. Which field to sort by: `created_at` or `updated_at`
+
+            - order: typing.Optional[GetUserDocsRequestOrder]. Which order should the sort be: `asc` (ascending) or `desc` (descending)
         ---
         from julep.client import AsyncJulepApi
 
         client = AsyncJulepApi(
             api_key="YOUR_API_KEY",
         )
         await client.get_user_docs(
@@ -2465,15 +3123,23 @@
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"users/{user_id}/docs"
             ),
-            params=remove_none_from_dict({"limit": limit, "offset": offset}),
+            params=remove_none_from_dict(
+                {
+                    "limit": limit,
+                    "offset": offset,
+                    "metadata_filter": metadata_filter,
+                    "sort_by": sort_by,
+                    "order": order,
+                }
+            ),
             headers=self._client_wrapper.get_headers(),
             timeout=300,
         )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(GetUserDocsResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
@@ -2797,14 +3463,60 @@
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    async def patch_agent_tool(
+        self, agent_id: str, tool_id: str, *, function: FunctionDef
+    ) -> ResourceUpdatedResponse:
+        """
+
+
+        Parameters:
+            - agent_id: str.
+
+            - tool_id: str.
+
+            - function: FunctionDef. Function definition and parameters
+        ---
+        from julep import FunctionDef
+        from julep.client import AsyncJulepApi
+
+        client = AsyncJulepApi(
+            api_key="YOUR_API_KEY",
+        )
+        await client.patch_agent_tool(
+            agent_id="agent_id",
+            tool_id="tool_id",
+            function=FunctionDef(
+                name="name",
+                parameters={},
+            ),
+        )
+        """
+        _response = await self._client_wrapper.httpx_client.request(
+            "PATCH",
+            urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"agents/{agent_id}/tools/{tool_id}",
+            ),
+            json=jsonable_encoder({"function": function}),
+            headers=self._client_wrapper.get_headers(),
+            timeout=300,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(ResourceUpdatedResponse, _response.json())  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
     async def get_job_status(self, job_id: str) -> JobStatus:
         """
 
 
         Parameters:
             - job_id: str.
         ---
```

### Comparing `julep-0.2.8/julep/api/core/__init__.py` & `julep-0.2.9/julep/api/core/__init__.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/core/client_wrapper.py` & `julep-0.2.9/julep/api/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/core/datetime_utils.py` & `julep-0.2.9/julep/api/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/core/jsonable_encoder.py` & `julep-0.2.9/julep/api/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/agent.py` & `julep-0.2.9/julep/api/types/agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from .agent_default_settings import AgentDefaultSettings
+from .agent_metadata import AgentMetadata
 from .instruction import Instruction
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class Agent(pydantic.BaseModel):
     name: str = pydantic.Field(description="Name of the agent")
-    about: str = pydantic.Field(description="About the agent")
+    about: typing.Optional[str] = pydantic.Field(description="About the agent")
     instructions: typing.Optional[typing.List[Instruction]] = pydantic.Field(
         description="List of instructions for the agent"
     )
     created_at: typing.Optional[dt.datetime] = pydantic.Field(
         description="Agent created at (RFC-3339 format)"
     )
     updated_at: typing.Optional[dt.datetime] = pydantic.Field(
         description="Agent updated at (RFC-3339 format)"
     )
     id: str = pydantic.Field(description="Agent id (UUID)")
     default_settings: typing.Optional[AgentDefaultSettings] = pydantic.Field(
         description="Default settings for all sessions created by this agent"
     )
     model: str = pydantic.Field(description="The model to use with this agent")
+    metadata: typing.Optional[AgentMetadata] = pydantic.Field(
+        description="Optional metadata"
+    )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {
             "by_alias": True,
             "exclude_unset": True,
             **kwargs,
         }
```

### Comparing `julep-0.2.8/julep/api/types/agent_default_settings.py` & `julep-0.2.9/julep/api/types/agent_default_settings.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/agent_default_settings_preset.py` & `julep-0.2.9/julep/api/types/agent_default_settings_preset.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/belief.py` & `julep-0.2.9/julep/api/types/chat_ml_message.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import typing_extensions
-
 from ..core.datetime_utils import serialize_datetime
+from .chat_ml_message_role import ChatMlMessageRole
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class Belief(pydantic.BaseModel):
-    type: typing_extensions.Literal["belief"]
-    subject: typing.Optional[str] = pydantic.Field(
-        description="(Optional) ID of the subject user"
-    )
-    content: str = pydantic.Field(description="Content of the memory")
-    rationale: typing.Optional[str] = pydantic.Field(
-        description="Rationale: Why did the model decide to form this memory"
-    )
-    weight: float = pydantic.Field(
-        description="Weight (importance) of the memory on a scale of 0-100"
-    )
-    sentiment: float = pydantic.Field(
-        description="Sentiment (valence) of the memory on a scale of -1 to 1"
+class ChatMlMessage(pydantic.BaseModel):
+    role: ChatMlMessageRole = pydantic.Field(
+        description=("ChatML role (system\n" "assistant\n" "user\n" "function_call)\n")
     )
+    content: str = pydantic.Field(description="ChatML content")
+    name: typing.Optional[str] = pydantic.Field(description="ChatML name")
     created_at: dt.datetime = pydantic.Field(
-        description="Belief created at (RFC-3339 format)"
+        description="Message created at (RFC-3339 format)"
     )
-    id: str = pydantic.Field(description="Belief id (UUID)")
+    id: str = pydantic.Field(description="Message ID")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {
             "by_alias": True,
             "exclude_unset": True,
             **kwargs,
         }
```

### Comparing `julep-0.2.8/julep/api/types/chat_input_data.py` & `julep-0.2.9/julep/api/types/chat_input_data.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/chat_ml_message.py` & `julep-0.2.9/julep/api/types/create_doc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .chat_ml_message_role import ChatMlMessageRole
+from .create_doc_metadata import CreateDocMetadata
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ChatMlMessage(pydantic.BaseModel):
-    role: ChatMlMessageRole = pydantic.Field(
-        description=("ChatML role (system\n" "assistant\n" "user\n" "function_call)\n")
+class CreateDoc(pydantic.BaseModel):
+    title: str = pydantic.Field(
+        description="Title describing what this bit of information contains"
     )
-    content: str = pydantic.Field(description="ChatML content")
-    name: typing.Optional[str] = pydantic.Field(description="ChatML name")
-    created_at: dt.datetime = pydantic.Field(
-        description="Message created at (RFC-3339 format)"
+    content: str = pydantic.Field(description="Information content")
+    metadata: typing.Optional[CreateDocMetadata] = pydantic.Field(
+        description="Optional metadata"
     )
-    id: str = pydantic.Field(description="Message ID")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {
             "by_alias": True,
             "exclude_unset": True,
             **kwargs,
         }
```

### Comparing `julep-0.2.8/julep/api/types/chat_ml_message_role.py` & `julep-0.2.9/julep/api/types/chat_ml_message_role.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/chat_response.py` & `julep-0.2.9/julep/api/types/chat_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/chat_response_finish_reason.py` & `julep-0.2.9/julep/api/types/chat_response_finish_reason.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/chat_settings.py` & `julep-0.2.9/julep/api/types/chat_settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,15 +71,25 @@
     top_p: typing.Optional[float] = pydantic.Field(
         description="Defaults to 1 An alternative to sampling with temperature, called nucleus sampling, where the model considers the results of the tokens with top_p probability mass. So 0.1 means only the tokens comprising the top 10% probability mass are considered. We generally recommend altering this or temperature but not both."
     )
     min_p: typing.Optional[float] = pydantic.Field(
         description="Minimum probability compared to leading token to be considered"
     )
     preset: typing.Optional[ChatSettingsPreset] = pydantic.Field(
-        description="Generation preset name (one of: problem_solving, conversational, fun, prose, creative, business, deterministic, code, multilingual)"
+        description=(
+            "Generation preset name (problem_solving\n"
+            "conversational\n"
+            "fun\n"
+            "prose\n"
+            "creative\n"
+            "business\n"
+            "deterministic\n"
+            "code\n"
+            "multilingual)\n"
+        )
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {
             "by_alias": True,
             "exclude_unset": True,
             **kwargs,
```

### Comparing `julep-0.2.8/julep/api/types/chat_settings_preset.py` & `julep-0.2.9/julep/api/types/chat_settings_preset.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
 class ChatSettingsPreset(str, enum.Enum):
     """
-    Generation preset name (one of: problem_solving, conversational, fun, prose, creative, business, deterministic, code, multilingual)
+    Generation preset name (problem_solving|conversational|fun|prose|creative|business|deterministic|code|multilingual)
     """
 
     PROBLEM_SOLVING = "problem_solving"
     CONVERSATIONAL = "conversational"
     FUN = "fun"
     PROSE = "prose"
     CREATIVE = "creative"
```

### Comparing `julep-0.2.8/julep/api/types/chat_settings_response_format.py` & `julep-0.2.9/julep/api/types/chat_settings_response_format.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/chat_settings_response_format_schema.py` & `julep-0.2.9/julep/api/types/chat_settings_response_format_schema.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/chat_settings_response_format_type.py` & `julep-0.2.9/julep/api/types/chat_settings_response_format_type.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/completion_usage.py` & `julep-0.2.9/julep/api/types/completion_usage.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/create_doc.py` & `julep-0.2.9/julep/api/types/named_tool_choice_function.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,19 +7,16 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class CreateDoc(pydantic.BaseModel):
-    title: str = pydantic.Field(
-        description="Title describing what this bit of information contains"
-    )
-    content: str = pydantic.Field(description="Information content")
+class NamedToolChoiceFunction(pydantic.BaseModel):
+    name: str = pydantic.Field(description="The name of the function to call.")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {
             "by_alias": True,
             "exclude_unset": True,
             **kwargs,
         }
```

### Comparing `julep-0.2.8/julep/api/types/create_tool_request.py` & `julep-0.2.9/julep/api/types/create_tool_request.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/create_tool_request_type.py` & `julep-0.2.9/julep/api/types/create_tool_request_type.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/doc.py` & `julep-0.2.9/julep/api/types/doc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .doc_metadata import DocMetadata
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class Doc(pydantic.BaseModel):
     title: str = pydantic.Field(
         description="Title describing what this bit of information contains"
     )
     content: str = pydantic.Field(description="Information content")
     id: str = pydantic.Field(description="ID of doc")
     created_at: dt.datetime = pydantic.Field(description="Doc created at")
+    metadata: typing.Optional[DocMetadata] = pydantic.Field(
+        description="optional metadata"
+    )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {
             "by_alias": True,
             "exclude_unset": True,
             **kwargs,
         }
```

### Comparing `julep-0.2.8/julep/api/types/entity.py` & `julep-0.2.9/julep/api/types/get_history_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .chat_ml_message import ChatMlMessage
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class Entity(pydantic.BaseModel):
-    """
-    TBD
-    """
-
-    id: str = pydantic.Field(description="Entity id (UUID)")
+class GetHistoryResponse(pydantic.BaseModel):
+    items: typing.Optional[typing.List[ChatMlMessage]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {
             "by_alias": True,
             "exclude_unset": True,
             **kwargs,
         }
```

### Comparing `julep-0.2.8/julep/api/types/episode.py` & `julep-0.2.9/julep/api/types/user.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-import typing_extensions
-
 from ..core.datetime_utils import serialize_datetime
+from .user_metadata import UserMetadata
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class Episode(pydantic.BaseModel):
-    type: typing_extensions.Literal["episode"]
-    subject: typing.Optional[str] = pydantic.Field(
-        description="(Optional) ID of the subject user"
-    )
-    content: str = pydantic.Field(description="Content of the memory")
-    weight: float = pydantic.Field(
-        description="Weight (importance) of the memory on a scale of 0-100"
-    )
-    created_at: dt.datetime = pydantic.Field(
-        description="Episode created at (RFC-3339 format)"
-    )
-    last_accessed_at: dt.datetime = pydantic.Field(
-        description="Episode last accessed at (RFC-3339 format)"
-    )
-    happened_at: dt.datetime = pydantic.Field(
-        description="Episode happened at (RFC-3339 format)"
-    )
-    duration: typing.Optional[float] = pydantic.Field(
-        description="Duration of the episode (in seconds)"
+class User(pydantic.BaseModel):
+    name: typing.Optional[str] = pydantic.Field(description="Name of the user")
+    about: typing.Optional[str] = pydantic.Field(description="About the user")
+    created_at: typing.Optional[dt.datetime] = pydantic.Field(
+        description="User created at (RFC-3339 format)"
+    )
+    updated_at: typing.Optional[dt.datetime] = pydantic.Field(
+        description="User updated at (RFC-3339 format)"
+    )
+    id: str = pydantic.Field(description="User id (UUID)")
+    metadata: typing.Optional[UserMetadata] = pydantic.Field(
+        description="Optional metadata"
     )
-    id: str = pydantic.Field(description="Episode id (UUID)")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {
             "by_alias": True,
             "exclude_unset": True,
             **kwargs,
         }
```

### Comparing `julep-0.2.8/julep/api/types/function_call_option.py` & `julep-0.2.9/julep/api/types/function_call_option.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/function_def.py` & `julep-0.2.9/julep/api/types/function_def.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/get_agent_docs_response.py` & `julep-0.2.9/julep/api/types/get_agent_docs_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/get_agent_memories_response.py` & `julep-0.2.9/julep/api/types/get_agent_memories_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/get_agent_tools_response.py` & `julep-0.2.9/julep/api/types/get_agent_tools_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/get_history_response.py` & `julep-0.2.9/julep/api/types/get_user_docs_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .chat_ml_message import ChatMlMessage
+from .doc import Doc
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class GetHistoryResponse(pydantic.BaseModel):
-    items: typing.Optional[typing.List[ChatMlMessage]]
+class GetUserDocsResponse(pydantic.BaseModel):
+    items: typing.Optional[typing.List[Doc]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {
             "by_alias": True,
             "exclude_unset": True,
             **kwargs,
         }
```

### Comparing `julep-0.2.8/julep/api/types/get_suggestions_response.py` & `julep-0.2.9/julep/api/types/get_suggestions_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/get_user_docs_response.py` & `julep-0.2.9/julep/api/types/list_sessions_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .doc import Doc
+from .session import Session
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class GetUserDocsResponse(pydantic.BaseModel):
-    items: typing.Optional[typing.List[Doc]]
+class ListSessionsResponse(pydantic.BaseModel):
+    items: typing.List[Session]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {
             "by_alias": True,
             "exclude_unset": True,
             **kwargs,
         }
```

### Comparing `julep-0.2.8/julep/api/types/input_chat_ml_message.py` & `julep-0.2.9/julep/api/types/input_chat_ml_message.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/input_chat_ml_message_role.py` & `julep-0.2.9/julep/api/types/input_chat_ml_message_role.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,23 +11,27 @@
     ChatML role (system|assistant|user|function_call)
     """
 
     USER = "user"
     ASSISTANT = "assistant"
     SYSTEM = "system"
     FUNCTION_CALL = "function_call"
+    AUTO = "auto"
 
     def visit(
         self,
         user: typing.Callable[[], T_Result],
         assistant: typing.Callable[[], T_Result],
         system: typing.Callable[[], T_Result],
         function_call: typing.Callable[[], T_Result],
+        auto: typing.Callable[[], T_Result],
     ) -> T_Result:
         if self is InputChatMlMessageRole.USER:
             return user()
         if self is InputChatMlMessageRole.ASSISTANT:
             return assistant()
         if self is InputChatMlMessageRole.SYSTEM:
             return system()
         if self is InputChatMlMessageRole.FUNCTION_CALL:
             return function_call()
+        if self is InputChatMlMessageRole.AUTO:
+            return auto()
```

### Comparing `julep-0.2.8/julep/api/types/instruction.py` & `julep-0.2.9/julep/api/types/instruction.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/job_status.py` & `julep-0.2.9/julep/api/types/job_status.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/job_status_state.py` & `julep-0.2.9/julep/api/types/job_status_state.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/list_agents_response.py` & `julep-0.2.9/julep/api/types/list_agents_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/list_sessions_response.py` & `julep-0.2.9/julep/api/types/create_agent_request_metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .session import Session
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ListSessionsResponse(pydantic.BaseModel):
-    items: typing.List[Session]
+class CreateAgentRequestMetadata(pydantic.BaseModel):
+    """
+    Optional metadata
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {
             "by_alias": True,
             "exclude_unset": True,
             **kwargs,
         }
```

### Comparing `julep-0.2.8/julep/api/types/list_users_response.py` & `julep-0.2.9/julep/api/types/list_users_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/memory_access_options.py` & `julep-0.2.9/julep/api/types/memory_access_options.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/named_tool_choice.py` & `julep-0.2.9/julep/api/types/named_tool_choice.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/named_tool_choice_function.py` & `julep-0.2.9/julep/api/types/patch_session_request_metadata.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class NamedToolChoiceFunction(pydantic.BaseModel):
-    name: str = pydantic.Field(description="The name of the function to call.")
+class PatchSessionRequestMetadata(pydantic.BaseModel):
+    """
+    Optional metadata
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {
             "by_alias": True,
             "exclude_unset": True,
             **kwargs,
         }
```

### Comparing `julep-0.2.8/julep/api/types/resource_created_response.py` & `julep-0.2.9/julep/api/types/resource_created_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/resource_deleted_response.py` & `julep-0.2.9/julep/api/types/resource_deleted_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/resource_updated_response.py` & `julep-0.2.9/julep/api/types/resource_updated_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/session.py` & `julep-0.2.9/julep/api/types/session.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from .session_metadata import SessionMetadata
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
@@ -27,14 +28,17 @@
     )
     created_at: typing.Optional[dt.datetime] = pydantic.Field(
         description="Session created at (RFC-3339 format)"
     )
     updated_at: typing.Optional[dt.datetime] = pydantic.Field(
         description="Session updated at (RFC-3339 format)"
     )
+    metadata: typing.Optional[SessionMetadata] = pydantic.Field(
+        description="Optional metadata"
+    )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {
             "by_alias": True,
             "exclude_unset": True,
             **kwargs,
         }
```

### Comparing `julep-0.2.8/julep/api/types/suggestion.py` & `julep-0.2.9/julep/api/types/suggestion.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/suggestion_target.py` & `julep-0.2.9/julep/api/types/suggestion_target.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/tool.py` & `julep-0.2.9/julep/api/types/tool.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/tool_type.py` & `julep-0.2.9/julep/api/types/tool_type.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/api/types/user.py` & `julep-0.2.9/julep/api/types/update_session_request_metadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,24 +7,18 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class User(pydantic.BaseModel):
-    name: typing.Optional[str] = pydantic.Field(description="Name of the user")
-    about: typing.Optional[str] = pydantic.Field(description="About the user")
-    created_at: typing.Optional[dt.datetime] = pydantic.Field(
-        description="User created at (RFC-3339 format)"
-    )
-    updated_at: typing.Optional[dt.datetime] = pydantic.Field(
-        description="User updated at (RFC-3339 format)"
-    )
-    id: str = pydantic.Field(description="User id (UUID)")
+class UpdateSessionRequestMetadata(pydantic.BaseModel):
+    """
+    Optional metadata
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {
             "by_alias": True,
             "exclude_unset": True,
             **kwargs,
         }
```

### Comparing `julep-0.2.8/julep/client.py` & `julep-0.2.9/julep/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Optional
 from urllib.parse import urlparse
 
 from beartype import beartype
+import httpx
 from openai import AsyncOpenAI, OpenAI
 from openai.resources.chat.chat import AsyncChat, Chat
 from openai.resources.completions import AsyncCompletions, Completions
 
 # Note: This is just here because fern generates docs where it asks to:
 # `from julep_ai.client import AsyncJulepApi, JulepApi`
 from .api.client import AsyncJulepApi, JulepApi  # noqa: F401
@@ -75,14 +76,16 @@
     completions: Completions
 
     @beartype
     def __init__(
         self,
         api_key: Optional[str] = JULEP_API_KEY,
         base_url: Optional[str] = JULEP_API_URL,
+        timeout: int = 300,
+        _httpx_client: Optional[httpx.Client] = None,
         *args,
         **kwargs,
     ):
         """
         Initialize a new client object with the given API key and base URL.
 
             Args:
@@ -105,15 +108,27 @@
         assert (
             api_key is not None
         ), "api_key must be provided or set as env var JULEP_API_KEY"
         assert (
             base_url is not None
         ), "base_url must be provided or set as env var JULEP_API_URL"
 
-        self._api_client = JulepApi(api_key=api_key, base_url=base_url, *args, **kwargs)
+        # Create an httpz client that follows redirects and has a timeout
+        httpx_client = _httpx_client or httpx.Client(
+            timeout=timeout,
+            follow_redirects=True,
+        )
+
+        self._api_client = JulepApi(
+            api_key=api_key,
+            base_url=base_url,
+            httpx_client=httpx_client,
+            *args,
+            **kwargs,
+        )
 
         self.agents = AgentsManager(api_client=self._api_client)
         self.users = UsersManager(api_client=self._api_client)
         self.sessions = SessionsManager(api_client=self._api_client)
         self.docs = DocsManager(api_client=self._api_client)
         self.memories = MemoriesManager(api_client=self._api_client)
         self.tools = ToolsManager(api_client=self._api_client)
```

### Comparing `julep-0.2.8/julep/managers/agent.py` & `julep-0.2.9/julep/managers/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import json
+from typing import Optional, TypedDict
 from uuid import UUID
 
-from typing import Optional, TypedDict
 from beartype import beartype
-from beartype.typing import Awaitable, List, Literal, Union
+from beartype.typing import Any, Awaitable, Dict, List, Literal, Union
 
 from ..api.types import (
     Agent,
     AgentDefaultSettings,
     CreateDoc,
     CreateToolRequest,
     Instruction,
@@ -203,15 +204,18 @@
             tools=tools,
             default_settings=default_settings,
             model=model,
             docs=docs,
         )
 
     def _list_items(
-        self, limit: Optional[int] = None, offset: Optional[int] = None
+        self,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+        metadata_filter: str = "{}",
     ) -> Union[ListAgentsResponse, Awaitable[ListAgentsResponse]]:
         """
         Lists items with optional pagination.
 
             This method wraps the `list_agents` API call and includes optional limit and offset parameters for pagination.
 
             Args:
@@ -220,14 +224,15 @@
 
             Returns:
                 Union[ListAgentsResponse, Awaitable[ListAgentsResponse]]: A ListAgentsResponse object, or an awaitable that resolves to a ListAgentsResponse object.
         """
         return self.api_client.list_agents(
             limit=limit,
             offset=offset,
+            metadata_filter=metadata_filter,
         )
 
     def _delete(self, agent_id: Union[str, UUID]) -> Union[None, Awaitable[None]]:
         """
         Delete an agent by its ID.
 
         Args:
@@ -405,14 +410,15 @@
 
     @beartype
     def list(
         self,
         *,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
+        metadata_filter: Dict[str, Any] = {},
     ) -> List[Agent]:
         """
         List the Agent objects, possibly with pagination.
 
         Args:
           limit (Optional[int], optional): The maximum number of Agent objects to return.
                                            Defaults to None, meaning no limit is applied.
@@ -423,17 +429,20 @@
         Returns:
           List[Agent]: A list of Agent objects.
 
         Raises:
           BeartypeDecorHintPepParamViolation: If the function is called with incorrect types
                                               for the `limit` or `offset` parameters.
         """
+        metadata_filter_string = json.dumps(metadata_filter)
+
         return self._list_items(
             limit=limit,
             offset=offset,
+            metadata_filter=metadata_filter_string,
         ).items
 
     @beartype
     def delete(self, agent_id: Union[str, UUID]):
         """
         Delete the agent with the specified ID.
 
@@ -594,32 +603,36 @@
 
     @beartype
     async def list(
         self,
         *,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
+        metadata_filter: Dict[str, Any] = {},
     ) -> List[Agent]:
         """
         Asynchronously lists agents with optional limit and offset.
 
         This method wraps the call to a private method '_list_items' which performs the actual listing
         of agent items. It uses the 'beartype' decorator for runtime type checking.
 
         Args:
             limit (Optional[int], optional): The maximum number of agent items to return. Defaults to None, which means no limit.
             offset (Optional[int], optional): The offset from where to start the listing. Defaults to None, which means start from the beginning.
 
         Returns:
             List[Agent]: A list of agent items collected based on the provided 'limit' and 'offset' parameters.
         """
+        metadata_filter_string = json.dumps(metadata_filter)
+
         return (
             await self._list_items(
                 limit=limit,
                 offset=offset,
+                metadata_filter=metadata_filter_string,
             )
         ).items
 
     @beartype
     async def delete(self, agent_id: Union[str, UUID]):
         """
         Asynchronously deletes an agent given its identifier.
```

### Comparing `julep-0.2.8/julep/managers/base.py` & `julep-0.2.9/julep/managers/base.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/managers/doc.py` & `julep-0.2.9/julep/managers/doc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import json
+from typing import Optional, TypedDict
 from uuid import UUID
 
-from typing import Optional, TypedDict
 from beartype import beartype
-from beartype.typing import Awaitable, List, Union
+from beartype.typing import Any, Awaitable, Dict, List, Union
 
 from ..api.types import (
     CreateDoc,
     Doc,
     ResourceCreatedResponse,
     GetAgentDocsResponse,
 )
@@ -29,44 +30,45 @@
     Manages documents for agents or users by providing methods to get, create, and delete docsrmation.
 
     The class utilizes an API client to interact with a back-end service that handles the document management operations.
 
     Typical usage example:
 
         docs_manager = BaseDocsManager(api_client)
-        agent_docs = docs_manager._get(agent_id="some-agent-uuid")
-        user_docs = docs_manager._get(user_id="some-user-uuid")
+        agent_docs = docs_manager._list(agent_id="some-agent-uuid")
+        user_docs = docs_manager._list(user_id="some-user-uuid")
         created_doc = docs_manager._create(agent_id="some-agent-uuid", doc={"key": "value"})
         docs_manager._delete(user_id="some-user-uuid", doc_id="some-doc-uuid")
 
     Attributes:
         api_client: A client instance used to make API calls to the document management system.
 
     Methods:
-        _get(agent_id: Optional[Union[str, UUID]], user_id: Optional[Union[str, UUID]],
+        _list(agent_id: Optional[Union[str, UUID]], user_id: Optional[Union[str, UUID]],
              limit: Optional[int]=None, offset: Optional[int]=None) -> Union[GetAgentDocsResponse, Awaitable[GetAgentDocsResponse]]
             Retrieves docsrmation for either an agent or user.
             Must provide exactly one valid UUID v4 for either `agent_id` or `user_id`.
 
         _create(agent_id: Optional[Union[str, UUID]], user_id: Optional[Union[str, UUID]], doc: DocDict) -> Union[ResourceCreatedResponse, Awaitable[ResourceCreatedResponse]]
             Creates docsrmation for either an agent or user.
             Must provide exactly one valid UUID v4 for either `agent_id` or `user_id`.
             The `doc` parameter contains the document information to be created.
 
         _delete(agent_id: Optional[Union[str, UUID]], user_id: Optional[Union[str, UUID]], doc_id: Union[str, UUID]):
             Deletes docsrmation for either an agent or user.
             Must provide exactly one valid UUID v4 for either `agent_id` or `user_id`, and a valid UUID for `doc_id`.
     """
 
-    def _get(
+    def _list(
         self,
         agent_id: Optional[Union[str, UUID]],
         user_id: Optional[Union[str, UUID]],
         limit: Optional[int] = None,
         offset: Optional[int] = None,
+        metadata_filter: Dict[str, Any] = {},
     ) -> Union[GetAgentDocsResponse, Awaitable[GetAgentDocsResponse]]:
         """
         Retrieve docsrmation for an agent or user based on their ID.
 
         This internal method fetches docsrmation for either an agent or a user,
         but not both. If both or neither `agent_id` and `user_id` are provided, it will
         assert an error.
@@ -79,32 +81,36 @@
 
         Returns:
             Union[GetAgentDocsResponse, Awaitable[GetAgentDocsResponse]]: The response object containing docsrmation about the agent or user, or a promise of such an object if the call is asynchronous.
 
         Raises:
             AssertionError: If both `agent_id` and `user_id` are provided or neither is provided, or if the provided IDs are not valid UUID v4.
         """
+        metadata_filter_string = json.dumps(metadata_filter)
+
         assert (
             (agent_id and is_valid_uuid4(agent_id))
             or (user_id and is_valid_uuid4(user_id))
             and not (agent_id and user_id)
         ), "One and only one of user_id or agent_id must be given and must be valid UUID v4"
 
         if agent_id is not None:
             return self.api_client.get_agent_docs(
                 agent_id=agent_id,
                 limit=limit,
                 offset=offset,
+                metadata_filter=metadata_filter_string,
             )
 
         if user_id is not None:
             return self.api_client.get_user_docs(
                 user_id=user_id,
                 limit=limit,
                 offset=offset,
+                metadata_filter=metadata_filter_string,
             )
 
     def _create(
         self,
         doc: DocDict,
         agent_id: Optional[Union[str, UUID]] = None,
         user_id: Optional[Union[str, UUID]] = None,
@@ -234,21 +240,22 @@
                 user_id (Optional[Union[str, UUID]]): The user's identifier associated with the document, if any.
 
             Returns:
                 None, but the method may raise exceptions on failure.
     """
 
     @beartype
-    def get(
+    def list(
         self,
         *,
         agent_id: Optional[Union[str, UUID]] = None,
         user_id: Optional[Union[str, UUID]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
+        metadata_filter: Dict[str, Any] = {},
     ) -> List[Doc]:
         """
         Retrieve a list of documents based on specified criteria.
 
         This method supports filtering the documents by agent_id or user_id, and also supports pagination through the limit and offset parameters.
 
         Args:
@@ -259,19 +266,20 @@
 
         Returns:
             List[Doc]: A list of documents that match the provided criteria.
 
         Note:
             The `@beartype` decorator is used to ensure that the input arguments are of the expected types. If an argument is passed that does not match the expected type, a type error will be raised.
         """
-        return self._get(
+        return self._list(
             agent_id=agent_id,
             user_id=user_id,
             limit=limit,
             offset=offset,
+            metadata_filter=metadata_filter,
         ).items
 
     @beartype
     @rewrap_in_class(Doc)
     def create(self, **kwargs: DocsCreateArgs) -> Doc:
         """
         Create a new resource with the specified document.
@@ -330,15 +338,15 @@
 
     Inherits from BaseDocsManager to provide async document retrieval, creation, and deletion.
 
     Attributes:
         Inherited from BaseDocsManager.
 
     Methods:
-        async get(self, *, agent_id: Optional[Union[str, UUID]] = None, user_id: Optional[Union[str, UUID]] = None, limit: Optional[int] = None, offset: Optional[int] = None) -> List[Doc]:
+        async list(self, *, agent_id: Optional[Union[str, UUID]] = None, user_id: Optional[Union[str, UUID]] = None, limit: Optional[int] = None, offset: Optional[int] = None) -> List[Doc]:
             Asynchronously get a list of documents, with optional filtering based on agent_id, user_id, and pagination options limit and offset.
             Args:
                 agent_id (Optional[Union[str, UUID]]): The agent's identifier to filter documents.
                 user_id (Optional[Union[str, UUID]]): The user's identifier to filter documents.
                 limit (Optional[int]): The maximum number of documents to return.
                 offset (Optional[int]): The offset from where to start returning documents.
             Returns:
@@ -361,21 +369,22 @@
                 user_id (Optional[Union[str, UUID]]): The user's identifier associated with the document, if applicable.
 
     Note:
         The `@beartype` decorator is being used to perform runtime type checking on the function arguments.
     """
 
     @beartype
-    async def get(
+    async def list(
         self,
         *,
         agent_id: Optional[Union[str, UUID]] = None,
         user_id: Optional[Union[str, UUID]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
+        metadata_filter: Dict[str, Any] = {},
     ) -> List[Doc]:
         """
         Asynchronously get a list of documents.
 
         This function fetches documents based on the provided filtering criteria such as `agent_id`, `user_id`,
         and supports pagination through `limit` and `offset`.
 
@@ -391,19 +400,20 @@
         Note:
             The `@beartype` decorator is used to ensure that arguments conform to the expected types.
 
         Raises:
             BeartypeDecorHintPepParamException: If any of the parameters do not adhere to the declared types.
         """
         return (
-            await self._get(
+            await self._list(
                 agent_id=agent_id,
                 user_id=user_id,
                 limit=limit,
                 offset=offset,
+                metadata_filter=metadata_filter,
             )
         ).items
 
     @beartype
     @rewrap_in_class(Doc)
     async def create(self, **kwargs: DocsCreateArgs) -> Doc:
         """
```

### Comparing `julep-0.2.8/julep/managers/memory.py` & `julep-0.2.9/julep/managers/memory.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/managers/session.py` & `julep-0.2.9/julep/managers/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import json
+from typing import Optional, TypedDict
 from uuid import UUID
 
-from typing import Optional, TypedDict
 from beartype import beartype
-from beartype.typing import Awaitable, List, Union, Dict
+from beartype.typing import Any, Awaitable, Dict, List, Union
 
 from ..api.types import (
     ResourceCreatedResponse,
     ResourceUpdatedResponse,
     Session,
     ListSessionsResponse,
     ChatSettingsStop,
@@ -186,15 +187,18 @@
         return self.api_client.create_session(
             user_id=user_id,
             agent_id=agent_id,
             situation=situation,
         )
 
     def _list_items(
-        self, limit: Optional[int] = None, offset: Optional[int] = None
+        self,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+        metadata_filter: str = "{}",
     ) -> Union[ListSessionsResponse, Awaitable[ListSessionsResponse]]:
         """
         List items with optional pagination.
 
         Args:
             limit (Optional[int]): The maximum number of items to return. Defaults to None.
             offset (Optional[int]): The number of items to skip before starting to collect the result set. Defaults to None.
@@ -204,14 +208,15 @@
 
         Note:
             The '_list_items' function is assumed to be a method of a class that has an 'api_client' attribute capable of listing sessions.
         """
         return self.api_client.list_sessions(
             limit=limit,
             offset=offset,
+            metadata_filter=metadata_filter,
         )
 
     def _delete(self, session_id: Union[str, UUID]) -> Union[None, Awaitable[None]]:
         """
         Delete a session given its session ID.
 
             This is an internal method that asserts the provided session_id is a valid UUID v4
@@ -491,14 +496,15 @@
 
     @beartype
     def list(
         self,
         *,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
+        metadata_filter: Dict[str, Any] = {},
     ) -> List[Session]:
         """
         Retrieve a list of Session objects with optional pagination.
 
             Args:
                 limit (Optional[int]): The maximum number of Session objects to return.
                     Defaults to None, which indicates no limit.
@@ -507,17 +513,20 @@
 
             Returns:
                 List[Session]: A list of Session objects meeting the criteria.
 
             Raises:
                 BeartypeException: If the input arguments do not match their annotated types.
         """
+        metadata_filter_string = json.dumps(metadata_filter)
+
         return self._list_items(
             limit=limit,
             offset=offset,
+            metadata_filter=metadata_filter_string,
         ).items
 
     @beartype
     def delete(self, session_id: Union[str, UUID]):
         """
         Deletes a session based on its session ID.
 
@@ -791,31 +800,35 @@
 
     @beartype
     async def list(
         self,
         *,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
+        metadata_filter: Dict[str, Any] = {},
     ) -> List[Session]:
         """
         Asynchronously retrieves a list of sessions with optional pagination.
 
         This method utilizes `_list_items` internally to obtain session data with support for limit and offset parameters. The `beartype` decorator is used to ensure that the function parameters match the expected types.
 
         Args:
             limit (Optional[int], optional): The maximum number of sessions to retrieve. Default is None, which retrieves all available sessions.
             offset (Optional[int], optional): The number to skip before starting to collect the response set. Default is None.
 
         Returns:
             List[Session]: A list of `Session` objects containing session data.
         """
+        metadata_filter_string = json.dumps(metadata_filter)
+
         return (
             await self._list_items(
                 limit=limit,
                 offset=offset,
+                metadata_filter=metadata_filter_string,
             )
         ).items
 
     @beartype
     async def delete(self, session_id: Union[str, UUID]):
         """
         Asynchronously delete a session given its ID.
```

### Comparing `julep-0.2.8/julep/managers/tool.py` & `julep-0.2.9/julep/managers/tool.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/managers/types.py` & `julep-0.2.9/julep/managers/types.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/managers/user.py` & `julep-0.2.9/julep/managers/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import json
 from uuid import UUID
 from typing import Optional, TypedDict
 
 from beartype import beartype
-from beartype.typing import Awaitable, List, Union
+from beartype.typing import Any, Awaitable, Dict, List, Union
 
 from .utils import rewrap_in_class
 
 from ..api.types import (
     User,
     CreateDoc,
     ResourceCreatedResponse,
@@ -109,15 +110,18 @@
         return self.api_client.create_user(
             name=name,
             about=about,
             docs=docs,
         )
 
     def _list_items(
-        self, limit: Optional[int] = None, offset: Optional[int] = None
+        self,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+        metadata_filter: str = "{}",
     ) -> Union[ListUsersResponse, Awaitable[ListUsersResponse]]:
         """
         Fetch a list of users, with optional pagination parameters.
 
             Args:
                 limit (Optional[int], optional): The maximum number of users to return. Defaults to None.
                 offset (Optional[int], optional): The offset from the start of the list to begin returning users. Defaults to None.
@@ -125,14 +129,15 @@
             Returns:
                 Union[ListUsersResponse, Awaitable[ListUsersResponse]]: An instance of ListUsersResponse,
                 or an awaitable that will resolve to it, depending on the API client implementation.
         """
         return self.api_client.list_users(
             limit=limit,
             offset=offset,
+            metadata_filter=metadata_filter,
         )
 
     def _delete(self, user_id: Union[str, UUID]) -> Union[None, Awaitable[None]]:
         """
         Delete a user given their user ID.
 
             Args:
@@ -252,14 +257,15 @@
 
     @beartype
     def list(
         self,
         *,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
+        metadata_filter: Dict[str, Any] = {},
     ) -> List[User]:
         """
         Lists the users optionally applying limit and offset.
 
         Args:
             limit (Optional[int], optional): The maximum number of users to return.
                 None means no limit. Defaults to None.
@@ -268,17 +274,20 @@
 
         Returns:
             List[User]: A list of user objects.
 
         Raises:
             BeartypeException: If the type of `limit` or `offset` is not as expected.
         """
+        metadata_filter_string = json.dumps(metadata_filter)
+
         return self._list_items(
             limit=limit,
             offset=offset,
+            metadata_filter=metadata_filter_string,
         ).items
 
     @beartype
     def delete(
         self,
         *,
         user_id: Union[str, UUID],
@@ -392,14 +401,15 @@
 
     @beartype
     async def list(
         self,
         *,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
+        metadata_filter: Dict[str, Any] = {},
     ) -> List[User]:
         """
         Asynchronously lists users with optional limits and offsets.
 
         This function applies the `beartype` decorator for runtime type checking.
 
         Args:
@@ -412,18 +422,21 @@
         Raises:
             TypeError: If any input arguments are not of the expected type.
             Any other exception that might be raised during the retrieval of users from the data source.
 
         Note:
             The actual exception raised by the `beartype` decorator or during the users' retrieval will depend on the implementation detail of the `self._list_items` method and the `beartype` configuration.
         """
+        metadata_filter_string = json.dumps(metadata_filter)
+
         return (
             await self._list_items(
                 limit,
                 offset,
+                metadata_filter=metadata_filter_string,
             )
         ).items
 
     @beartype
     async def delete(
         self,
         *,
```

### Comparing `julep-0.2.8/julep/managers/utils.py` & `julep-0.2.9/julep/managers/utils.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/julep/utils/openai_patch.py` & `julep-0.2.9/julep/utils/openai_patch.py`

 * *Files identical despite different names*

### Comparing `julep-0.2.8/pyproject.toml` & `julep-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "julep"
-version = "0.2.8"
+version = "0.2.9"
 description = "Julep is a platform for creating agents with long-term memory"
 authors = ["Julep Developers <developers@julep.ai>"]
 license = "ISC"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.14"
```

### Comparing `julep-0.2.8/PKG-INFO` & `julep-0.2.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: julep
-Version: 0.2.8
+Version: 0.2.9
 Summary: Julep is a platform for creating agents with long-term memory
 License: ISC
 Author: Julep Developers
 Author-email: developers@julep.ai
 Requires-Python: >=3.8,<3.14
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beartype (>=0.14.0,<1.0.0)
 Requires-Dist: environs (>=9.0.0,<11.0.0)
 Requires-Dist: httpx (>=0.20.0,<1.0.0)
 Requires-Dist: openai (>=1.0.1,<2.0.0)
 Requires-Dist: pydantic (>=2.0.1,<3.0.0)
 Requires-Dist: typing-extensions (>=4.0.0,<5.0.0)
 Description-Content-Type: text/markdown
```

