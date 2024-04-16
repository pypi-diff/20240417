# Comparing `tmp/vocode_api-0.0.8.tar.gz` & `tmp/vocode_api-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocode_api-0.0.8.tar", max compression
+gzip compressed data, was "vocode_api-0.0.9.tar", max compression
```

## Comparing `vocode_api-0.0.8.tar` & `vocode_api-0.0.9.tar`

### file list

```diff
@@ -1,142 +1,142 @@
--rw-r--r--   0        0        0     2777 2023-08-19 23:21:56.849484 vocode_api-0.0.8/README.md
--rw-r--r--   0        0        0      391 2023-08-19 23:21:56.849484 vocode_api-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    11676 2023-08-19 23:21:56.849484 vocode_api-0.0.8/src/vocode/__init__.py
--rw-r--r--   0        0        0     2334 2023-08-19 23:21:56.849484 vocode_api-0.0.8/src/vocode/client.py
--rw-r--r--   0        0        0      519 2023-08-19 23:21:56.849484 vocode_api-0.0.8/src/vocode/core/__init__.py
--rw-r--r--   0        0        0      426 2023-08-19 23:21:56.849484 vocode_api-0.0.8/src/vocode/core/api_error.py
--rw-r--r--   0        0        0     1384 2023-08-19 23:21:56.849484 vocode_api-0.0.8/src/vocode/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2023-08-19 23:21:56.849484 vocode_api-0.0.8/src/vocode/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-08-19 23:21:56.849484 vocode_api-0.0.8/src/vocode/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2023-08-19 23:21:56.849484 vocode_api-0.0.8/src/vocode/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      170 2023-08-19 23:21:56.849484 vocode_api-0.0.8/src/vocode/errors/__init__.py
--rw-r--r--   0        0        0      313 2023-08-19 23:21:56.849484 vocode_api-0.0.8/src/vocode/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2023-08-19 23:21:56.849484 vocode_api-0.0.8/src/vocode/py.typed
--rw-r--r--   0        0        0      220 2023-08-19 23:21:56.849484 vocode_api-0.0.8/src/vocode/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-08-19 23:21:56.849484 vocode_api-0.0.8/src/vocode/resources/actions/__init__.py
--rw-r--r--   0        0        0     9846 2023-08-19 23:21:56.849484 vocode_api-0.0.8/src/vocode/resources/actions/client.py
--rw-r--r--   0        0        0       65 2023-08-19 23:21:56.849484 vocode_api-0.0.8/src/vocode/resources/agents/__init__.py
--rw-r--r--   0        0        0    13277 2023-08-19 23:21:56.849484 vocode_api-0.0.8/src/vocode/resources/agents/client.py
--rw-r--r--   0        0        0       65 2023-08-19 23:21:56.849484 vocode_api-0.0.8/src/vocode/resources/calls/__init__.py
--rw-r--r--   0        0        0    11571 2023-08-19 23:21:56.849484 vocode_api-0.0.8/src/vocode/resources/calls/client.py
--rw-r--r--   0        0        0       65 2023-08-19 23:21:56.849484 vocode_api-0.0.8/src/vocode/resources/numbers/__init__.py
--rw-r--r--   0        0        0    12280 2023-08-19 23:21:56.849484 vocode_api-0.0.8/src/vocode/resources/numbers/client.py
--rw-r--r--   0        0        0       65 2023-08-19 23:21:56.849484 vocode_api-0.0.8/src/vocode/resources/usage/__init__.py
--rw-r--r--   0        0        0     1921 2023-08-19 23:21:56.849484 vocode_api-0.0.8/src/vocode/resources/usage/client.py
--rw-r--r--   0        0        0       65 2023-08-19 23:21:56.849484 vocode_api-0.0.8/src/vocode/resources/voices/__init__.py
--rw-r--r--   0        0        0     9796 2023-08-19 23:21:56.849484 vocode_api-0.0.8/src/vocode/resources/voices/client.py
--rw-r--r--   0        0        0       65 2023-08-19 23:21:56.849484 vocode_api-0.0.8/src/vocode/resources/webhooks/__init__.py
--rw-r--r--   0        0        0     9640 2023-08-19 23:21:56.849484 vocode_api-0.0.8/src/vocode/resources/webhooks/client.py
--rw-r--r--   0        0        0    15334 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/__init__.py
--rw-r--r--   0        0        0      904 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/action_page.py
--rw-r--r--   0        0        0     1158 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/action_page_items_item.py
--rw-r--r--   0        0        0     1215 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/action_params_request.py
--rw-r--r--   0        0        0     1158 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/action_response_model.py
--rw-r--r--   0        0        0     1323 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/action_update_params_request.py
--rw-r--r--   0        0        0     1413 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/agent.py
--rw-r--r--   0        0        0     1137 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/agent_actions_item.py
--rw-r--r--   0        0        0      889 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/agent_page.py
--rw-r--r--   0        0        0      220 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/agent_params_actions_item.py
--rw-r--r--   0        0        0     1266 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/agent_params_actions_item_one.py
--rw-r--r--   0        0        0      231 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/agent_params_vector_database.py
--rw-r--r--   0        0        0      195 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/agent_params_voice.py
--rw-r--r--   0        0        0     1448 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/agent_params_voice_one.py
--rw-r--r--   0        0        0      177 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/agent_params_webhook.py
--rw-r--r--   0        0        0     1993 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/agent_update_params.py
--rw-r--r--   0        0        0      283 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/agent_update_params_actions.py
--rw-r--r--   0        0        0      245 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/agent_update_params_actions_item.py
--rw-r--r--   0        0        0     1365 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/agent_update_params_actions_item_one.py
--rw-r--r--   0        0        0      178 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/agent_update_params_context_endpoint.py
--rw-r--r--   0        0        0      177 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/agent_update_params_initial_message.py
--rw-r--r--   0        0        0      256 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/agent_update_params_interrupt_sensitivity.py
--rw-r--r--   0        0        0      207 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/agent_update_params_language.py
--rw-r--r--   0        0        0      169 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/agent_update_params_prompt.py
--rw-r--r--   0        0        0      300 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/agent_update_params_vector_database.py
--rw-r--r--   0        0        0      264 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/agent_update_params_voice.py
--rw-r--r--   0        0        0     1578 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/agent_update_params_voice_one.py
--rw-r--r--   0        0        0      246 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/agent_update_params_webhook.py
--rw-r--r--   0        0        0     1278 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/agent_voice.py
--rw-r--r--   0        0        0      869 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/azure_voice.py
--rw-r--r--   0        0        0      846 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/azure_voice_params.py
--rw-r--r--   0        0        0     1170 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/azure_voice_update_params.py
--rw-r--r--   0        0        0      173 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/azure_voice_update_params_pitch.py
--rw-r--r--   0        0        0      172 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/azure_voice_update_params_rate.py
--rw-r--r--   0        0        0      177 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/azure_voice_update_params_voice_name.py
--rw-r--r--   0        0        0     1178 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/call.py
--rw-r--r--   0        0        0      885 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/call_page.py
--rw-r--r--   0        0        0      832 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/call_status.py
--rw-r--r--   0        0        0     1645 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/create_call_agent_params.py
--rw-r--r--   0        0        0      262 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/create_call_agent_params_actions_item.py
--rw-r--r--   0        0        0     1336 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/create_call_agent_params_actions_item_one.py
--rw-r--r--   0        0        0      241 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/create_call_agent_params_vector_database.py
--rw-r--r--   0        0        0      237 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/create_call_agent_params_voice.py
--rw-r--r--   0        0        0     1538 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/create_call_agent_params_voice_one.py
--rw-r--r--   0        0        0      187 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/create_call_agent_params_webhook.py
--rw-r--r--   0        0        0      207 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/create_call_request_agent.py
--rw-r--r--   0        0        0      884 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/dtmf_action.py
--rw-r--r--   0        0        0      861 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/dtmf_action_params.py
--rw-r--r--   0        0        0      902 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/dtmf_action_update_params.py
--rw-r--r--   0        0        0      239 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/dtmf_action_update_params_config.py
--rw-r--r--   0        0        0      909 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/eleven_labs_voice.py
--rw-r--r--   0        0        0      886 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/eleven_labs_voice_params.py
--rw-r--r--   0        0        0     1428 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/eleven_labs_voice_update_params.py
--rw-r--r--   0        0        0      179 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/eleven_labs_voice_update_params_api_key.py
--rw-r--r--   0        0        0      190 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/eleven_labs_voice_update_params_similarity_boost.py
--rw-r--r--   0        0        0      184 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/eleven_labs_voice_update_params_stability.py
--rw-r--r--   0        0        0      180 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/eleven_labs_voice_update_params_voice_id.py
--rw-r--r--   0        0        0      763 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/empty_action_config.py
--rw-r--r--   0        0        0      895 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/end_conversation_action.py
--rw-r--r--   0        0        0      872 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/end_conversation_action_params.py
--rw-r--r--   0        0        0      947 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/end_conversation_action_update_params.py
--rw-r--r--   0        0        0      250 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/end_conversation_action_update_params_config.py
--rw-r--r--   0        0        0     1395 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/event_type.py
--rw-r--r--   0        0        0      466 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/http_method.py
--rw-r--r--   0        0        0      870 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/http_validation_error.py
--rw-r--r--   0        0        0      496 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/interrupt_sensitivity.py
--rw-r--r--   0        0        0      564 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/language.py
--rw-r--r--   0        0        0     1307 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/normalized_agent.py
--rw-r--r--   0        0        0      235 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/normalized_agent_vector_database.py
--rw-r--r--   0        0        0     1161 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/normalized_call.py
--rw-r--r--   0        0        0      902 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/normalized_phone_number.py
--rw-r--r--   0        0        0      919 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/phone_number.py
--rw-r--r--   0        0        0      914 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/phone_number_page.py
--rw-r--r--   0        0        0      944 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/pinecone_vector_database.py
--rw-r--r--   0        0        0      921 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/pinecone_vector_database_params.py
--rw-r--r--   0        0        0     1412 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/pinecone_vector_database_update_params.py
--rw-r--r--   0        0        0      194 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/pinecone_vector_database_update_params_api_environment.py
--rw-r--r--   0        0        0      186 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/pinecone_vector_database_update_params_api_key.py
--rw-r--r--   0        0        0      185 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/pinecone_vector_database_update_params_index.py
--rw-r--r--   0        0        0      749 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/plan_type.py
--rw-r--r--   0        0        0      843 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/play_ht_voice.py
--rw-r--r--   0        0        0      820 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/play_ht_voice_params.py
--rw-r--r--   0        0        0     1205 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/play_ht_voice_update_params.py
--rw-r--r--   0        0        0      175 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/play_ht_voice_update_params_api_key.py
--rw-r--r--   0        0        0      178 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/play_ht_voice_update_params_api_user_id.py
--rw-r--r--   0        0        0      176 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/play_ht_voice_update_params_voice_id.py
--rw-r--r--   0        0        0      802 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/rime_voice.py
--rw-r--r--   0        0        0      779 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/rime_voice_params.py
--rw-r--r--   0        0        0      902 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/rime_voice_update_params.py
--rw-r--r--   0        0        0      174 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/rime_voice_update_params_speaker.py
--rw-r--r--   0        0        0      878 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/transfer_call_action.py
--rw-r--r--   0        0        0      855 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/transfer_call_action_params.py
--rw-r--r--   0        0        0      935 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/transfer_call_action_update_params.py
--rw-r--r--   0        0        0      250 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/transfer_call_action_update_params_config.py
--rw-r--r--   0        0        0      787 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/transfer_call_config.py
--rw-r--r--   0        0        0      755 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/undefined.py
--rw-r--r--   0        0        0      247 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/update_number_request_inbound_agent.py
--rw-r--r--   0        0        0      170 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/update_number_request_label.py
--rw-r--r--   0        0        0      893 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/usage.py
--rw-r--r--   0        0        0      896 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/validation_error.py
--rw-r--r--   0        0        0      128 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/validation_error_loc_item.py
--rw-r--r--   0        0        0      900 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/voice_page.py
--rw-r--r--   0        0        0     1363 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/voice_page_items_item.py
--rw-r--r--   0        0        0     1439 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/voice_params_request.py
--rw-r--r--   0        0        0     1363 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/voice_response_model.py
--rw-r--r--   0        0        0     1569 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/voice_update_params_request.py
--rw-r--r--   0        0        0      948 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/webhook.py
--rw-r--r--   0        0        0      866 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/webhook_page.py
--rw-r--r--   0        0        0      925 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/webhook_params.py
--rw-r--r--   0        0        0     1151 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/webhook_update_params.py
--rw-r--r--   0        0        0      214 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/webhook_update_params_method.py
--rw-r--r--   0        0        0      231 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/webhook_update_params_subscriptions.py
--rw-r--r--   0        0        0      168 2023-08-19 23:21:56.853484 vocode_api-0.0.8/src/vocode/types/webhook_update_params_url.py
--rw-r--r--   0        0        0     3185 1970-01-01 00:00:00.000000 vocode_api-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     2777 2023-08-20 01:24:05.105211 vocode_api-0.0.9/README.md
+-rw-r--r--   0        0        0      391 2023-08-20 01:24:05.105211 vocode_api-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    11676 2023-08-20 01:24:05.105211 vocode_api-0.0.9/src/vocode/__init__.py
+-rw-r--r--   0        0        0     2334 2023-08-20 01:24:05.105211 vocode_api-0.0.9/src/vocode/client.py
+-rw-r--r--   0        0        0      519 2023-08-20 01:24:05.105211 vocode_api-0.0.9/src/vocode/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-08-20 01:24:05.105211 vocode_api-0.0.9/src/vocode/core/api_error.py
+-rw-r--r--   0        0        0     1384 2023-08-20 01:24:05.105211 vocode_api-0.0.9/src/vocode/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2023-08-20 01:24:05.105211 vocode_api-0.0.9/src/vocode/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-08-20 01:24:05.105211 vocode_api-0.0.9/src/vocode/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2023-08-20 01:24:05.105211 vocode_api-0.0.9/src/vocode/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      170 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/errors/__init__.py
+-rw-r--r--   0        0        0      313 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/py.typed
+-rw-r--r--   0        0        0      220 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/resources/actions/__init__.py
+-rw-r--r--   0        0        0     9846 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/resources/actions/client.py
+-rw-r--r--   0        0        0       65 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/resources/agents/__init__.py
+-rw-r--r--   0        0        0    13277 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/resources/agents/client.py
+-rw-r--r--   0        0        0       65 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/resources/calls/__init__.py
+-rw-r--r--   0        0        0    11571 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/resources/calls/client.py
+-rw-r--r--   0        0        0       65 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/resources/numbers/__init__.py
+-rw-r--r--   0        0        0    12280 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/resources/numbers/client.py
+-rw-r--r--   0        0        0       65 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/resources/usage/__init__.py
+-rw-r--r--   0        0        0     1921 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/resources/usage/client.py
+-rw-r--r--   0        0        0       65 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/resources/voices/__init__.py
+-rw-r--r--   0        0        0     9796 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/resources/voices/client.py
+-rw-r--r--   0        0        0       65 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/resources/webhooks/__init__.py
+-rw-r--r--   0        0        0     9640 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/resources/webhooks/client.py
+-rw-r--r--   0        0        0    15334 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/__init__.py
+-rw-r--r--   0        0        0      904 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/action_page.py
+-rw-r--r--   0        0        0     1158 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/action_page_items_item.py
+-rw-r--r--   0        0        0     1215 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/action_params_request.py
+-rw-r--r--   0        0        0     1158 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/action_response_model.py
+-rw-r--r--   0        0        0     1323 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/action_update_params_request.py
+-rw-r--r--   0        0        0     1413 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/agent.py
+-rw-r--r--   0        0        0     1137 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/agent_actions_item.py
+-rw-r--r--   0        0        0      889 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/agent_page.py
+-rw-r--r--   0        0        0      220 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/agent_params_actions_item.py
+-rw-r--r--   0        0        0     1266 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/agent_params_actions_item_one.py
+-rw-r--r--   0        0        0      231 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/agent_params_vector_database.py
+-rw-r--r--   0        0        0      195 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/agent_params_voice.py
+-rw-r--r--   0        0        0     1448 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/agent_params_voice_one.py
+-rw-r--r--   0        0        0      177 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/agent_params_webhook.py
+-rw-r--r--   0        0        0     1993 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/agent_update_params.py
+-rw-r--r--   0        0        0      283 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/agent_update_params_actions.py
+-rw-r--r--   0        0        0      245 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/agent_update_params_actions_item.py
+-rw-r--r--   0        0        0     1365 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/agent_update_params_actions_item_one.py
+-rw-r--r--   0        0        0      178 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/agent_update_params_context_endpoint.py
+-rw-r--r--   0        0        0      177 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/agent_update_params_initial_message.py
+-rw-r--r--   0        0        0      256 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/agent_update_params_interrupt_sensitivity.py
+-rw-r--r--   0        0        0      207 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/agent_update_params_language.py
+-rw-r--r--   0        0        0      169 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/agent_update_params_prompt.py
+-rw-r--r--   0        0        0      300 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/agent_update_params_vector_database.py
+-rw-r--r--   0        0        0      264 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/agent_update_params_voice.py
+-rw-r--r--   0        0        0     1315 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/agent_update_params_voice_one.py
+-rw-r--r--   0        0        0      246 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/agent_update_params_webhook.py
+-rw-r--r--   0        0        0     1278 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/agent_voice.py
+-rw-r--r--   0        0        0      869 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/azure_voice.py
+-rw-r--r--   0        0        0      846 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/azure_voice_params.py
+-rw-r--r--   0        0        0     1247 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/azure_voice_update_params.py
+-rw-r--r--   0        0        0      173 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/azure_voice_update_params_pitch.py
+-rw-r--r--   0        0        0      172 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/azure_voice_update_params_rate.py
+-rw-r--r--   0        0        0      177 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/azure_voice_update_params_voice_name.py
+-rw-r--r--   0        0        0     1178 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/call.py
+-rw-r--r--   0        0        0      885 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/call_page.py
+-rw-r--r--   0        0        0      832 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/call_status.py
+-rw-r--r--   0        0        0     1645 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/create_call_agent_params.py
+-rw-r--r--   0        0        0      262 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/create_call_agent_params_actions_item.py
+-rw-r--r--   0        0        0     1072 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/create_call_agent_params_actions_item_one.py
+-rw-r--r--   0        0        0      241 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/create_call_agent_params_vector_database.py
+-rw-r--r--   0        0        0      237 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/create_call_agent_params_voice.py
+-rw-r--r--   0        0        0     1538 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/create_call_agent_params_voice_one.py
+-rw-r--r--   0        0        0      187 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/create_call_agent_params_webhook.py
+-rw-r--r--   0        0        0      207 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/create_call_request_agent.py
+-rw-r--r--   0        0        0      884 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/dtmf_action.py
+-rw-r--r--   0        0        0      938 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/dtmf_action_params.py
+-rw-r--r--   0        0        0      902 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/dtmf_action_update_params.py
+-rw-r--r--   0        0        0      239 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/dtmf_action_update_params_config.py
+-rw-r--r--   0        0        0      909 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/eleven_labs_voice.py
+-rw-r--r--   0        0        0      886 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/eleven_labs_voice_params.py
+-rw-r--r--   0        0        0     1511 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/eleven_labs_voice_update_params.py
+-rw-r--r--   0        0        0      179 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/eleven_labs_voice_update_params_api_key.py
+-rw-r--r--   0        0        0      190 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/eleven_labs_voice_update_params_similarity_boost.py
+-rw-r--r--   0        0        0      184 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/eleven_labs_voice_update_params_stability.py
+-rw-r--r--   0        0        0      180 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/eleven_labs_voice_update_params_voice_id.py
+-rw-r--r--   0        0        0      763 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/empty_action_config.py
+-rw-r--r--   0        0        0      895 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/end_conversation_action.py
+-rw-r--r--   0        0        0      961 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/end_conversation_action_params.py
+-rw-r--r--   0        0        0      947 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/end_conversation_action_update_params.py
+-rw-r--r--   0        0        0      250 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/end_conversation_action_update_params_config.py
+-rw-r--r--   0        0        0     1395 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/event_type.py
+-rw-r--r--   0        0        0      466 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/http_method.py
+-rw-r--r--   0        0        0      870 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/http_validation_error.py
+-rw-r--r--   0        0        0      496 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/interrupt_sensitivity.py
+-rw-r--r--   0        0        0      564 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/language.py
+-rw-r--r--   0        0        0     1307 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/normalized_agent.py
+-rw-r--r--   0        0        0      235 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/normalized_agent_vector_database.py
+-rw-r--r--   0        0        0     1161 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/normalized_call.py
+-rw-r--r--   0        0        0      902 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/normalized_phone_number.py
+-rw-r--r--   0        0        0      919 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/phone_number.py
+-rw-r--r--   0        0        0      914 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/phone_number_page.py
+-rw-r--r--   0        0        0      944 2023-08-20 01:24:05.109211 vocode_api-0.0.9/src/vocode/types/pinecone_vector_database.py
+-rw-r--r--   0        0        0      921 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/pinecone_vector_database_params.py
+-rw-r--r--   0        0        0     1412 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/pinecone_vector_database_update_params.py
+-rw-r--r--   0        0        0      194 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/pinecone_vector_database_update_params_api_environment.py
+-rw-r--r--   0        0        0      186 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/pinecone_vector_database_update_params_api_key.py
+-rw-r--r--   0        0        0      185 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/pinecone_vector_database_update_params_index.py
+-rw-r--r--   0        0        0      749 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/plan_type.py
+-rw-r--r--   0        0        0      843 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/play_ht_voice.py
+-rw-r--r--   0        0        0      820 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/play_ht_voice_params.py
+-rw-r--r--   0        0        0     1284 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/play_ht_voice_update_params.py
+-rw-r--r--   0        0        0      175 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/play_ht_voice_update_params_api_key.py
+-rw-r--r--   0        0        0      178 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/play_ht_voice_update_params_api_user_id.py
+-rw-r--r--   0        0        0      176 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/play_ht_voice_update_params_voice_id.py
+-rw-r--r--   0        0        0      802 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/rime_voice.py
+-rw-r--r--   0        0        0      779 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/rime_voice_params.py
+-rw-r--r--   0        0        0      978 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/rime_voice_update_params.py
+-rw-r--r--   0        0        0      174 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/rime_voice_update_params_speaker.py
+-rw-r--r--   0        0        0      878 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/transfer_call_action.py
+-rw-r--r--   0        0        0      941 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/transfer_call_action_params.py
+-rw-r--r--   0        0        0      935 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/transfer_call_action_update_params.py
+-rw-r--r--   0        0        0      250 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/transfer_call_action_update_params_config.py
+-rw-r--r--   0        0        0      787 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/transfer_call_config.py
+-rw-r--r--   0        0        0      755 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/undefined.py
+-rw-r--r--   0        0        0      247 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/update_number_request_inbound_agent.py
+-rw-r--r--   0        0        0      170 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/update_number_request_label.py
+-rw-r--r--   0        0        0      893 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/usage.py
+-rw-r--r--   0        0        0      896 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/validation_error.py
+-rw-r--r--   0        0        0      128 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0      900 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/voice_page.py
+-rw-r--r--   0        0        0     1363 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/voice_page_items_item.py
+-rw-r--r--   0        0        0     1439 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/voice_params_request.py
+-rw-r--r--   0        0        0     1363 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/voice_response_model.py
+-rw-r--r--   0        0        0     1302 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/voice_update_params_request.py
+-rw-r--r--   0        0        0      948 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/webhook.py
+-rw-r--r--   0        0        0      866 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/webhook_page.py
+-rw-r--r--   0        0        0      925 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/webhook_params.py
+-rw-r--r--   0        0        0     1151 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/webhook_update_params.py
+-rw-r--r--   0        0        0      214 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/webhook_update_params_method.py
+-rw-r--r--   0        0        0      231 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/webhook_update_params_subscriptions.py
+-rw-r--r--   0        0        0      168 2023-08-20 01:24:05.113211 vocode_api-0.0.9/src/vocode/types/webhook_update_params_url.py
+-rw-r--r--   0        0        0     3185 1970-01-01 00:00:00.000000 vocode_api-0.0.9/PKG-INFO
```

### Comparing `vocode_api-0.0.8/README.md` & `vocode_api-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/__init__.py` & `vocode_api-0.0.9/src/vocode/__init__.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/client.py` & `vocode_api-0.0.9/src/vocode/client.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/core/__init__.py` & `vocode_api-0.0.9/src/vocode/core/__init__.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/core/client_wrapper.py` & `vocode_api-0.0.9/src/vocode/core/client_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         self._token = token
         self._base_url = base_url
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "vocode-api",
-            "X-Fern-SDK-Version": "0.0.8",
+            "X-Fern-SDK-Version": "0.0.9",
         }
         headers["Authorization"] = f"Bearer {self._get_token()}"
         return headers
 
     def _get_token(self) -> str:
         if isinstance(self._token, str):
             return self._token
```

### Comparing `vocode_api-0.0.8/src/vocode/core/datetime_utils.py` & `vocode_api-0.0.9/src/vocode/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/core/jsonable_encoder.py` & `vocode_api-0.0.9/src/vocode/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/resources/actions/client.py` & `vocode_api-0.0.9/src/vocode/resources/actions/client.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/resources/agents/client.py` & `vocode_api-0.0.9/src/vocode/resources/agents/client.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/resources/calls/client.py` & `vocode_api-0.0.9/src/vocode/resources/calls/client.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/resources/numbers/client.py` & `vocode_api-0.0.9/src/vocode/resources/numbers/client.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/resources/usage/client.py` & `vocode_api-0.0.9/src/vocode/resources/usage/client.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/resources/voices/client.py` & `vocode_api-0.0.9/src/vocode/resources/voices/client.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/resources/webhooks/client.py` & `vocode_api-0.0.9/src/vocode/resources/webhooks/client.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/__init__.py` & `vocode_api-0.0.9/src/vocode/types/__init__.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/action_page.py` & `vocode_api-0.0.9/src/vocode/types/action_page.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/action_page_items_item.py` & `vocode_api-0.0.9/src/vocode/types/action_page_items_item.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/action_params_request.py` & `vocode_api-0.0.9/src/vocode/types/action_params_request.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/action_response_model.py` & `vocode_api-0.0.9/src/vocode/types/action_response_model.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/action_update_params_request.py` & `vocode_api-0.0.9/src/vocode/types/action_update_params_request.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/agent.py` & `vocode_api-0.0.9/src/vocode/types/agent.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/agent_actions_item.py` & `vocode_api-0.0.9/src/vocode/types/agent_actions_item.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/agent_page.py` & `vocode_api-0.0.9/src/vocode/types/agent_page.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/agent_params_actions_item_one.py` & `vocode_api-0.0.9/src/vocode/types/agent_params_actions_item_one.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/agent_params_voice_one.py` & `vocode_api-0.0.9/src/vocode/types/agent_params_voice_one.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/agent_update_params.py` & `vocode_api-0.0.9/src/vocode/types/agent_update_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/agent_update_params_actions_item_one.py` & `vocode_api-0.0.9/src/vocode/types/agent_update_params_actions_item_one.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/agent_update_params_voice_one.py` & `vocode_api-0.0.9/src/vocode/types/agent_update_params_voice_one.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,48 +9,44 @@
 from .azure_voice_update_params import AzureVoiceUpdateParams
 from .eleven_labs_voice_update_params import ElevenLabsVoiceUpdateParams
 from .play_ht_voice_update_params import PlayHtVoiceUpdateParams
 from .rime_voice_update_params import RimeVoiceUpdateParams
 
 
 class AgentUpdateParamsVoiceOne_VoiceAzure(AzureVoiceUpdateParams):
-    type: typing_extensions.Literal["voice_azure"]
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
 
 
 class AgentUpdateParamsVoiceOne_VoiceRime(RimeVoiceUpdateParams):
-    type: typing_extensions.Literal["voice_rime"]
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
 
 
 class AgentUpdateParamsVoiceOne_VoiceElevenLabs(ElevenLabsVoiceUpdateParams):
-    type: typing_extensions.Literal["voice_eleven_labs"]
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
 
 
 class AgentUpdateParamsVoiceOne_VoicePlayHt(PlayHtVoiceUpdateParams):
-    type: typing_extensions.Literal["voice_play_ht"]
-
+    
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
 
 
 AgentUpdateParamsVoiceOne = typing.Union[
-    AgentUpdateParamsVoiceOne_VoiceAzure,
-    AgentUpdateParamsVoiceOne_VoiceRime,
-    AgentUpdateParamsVoiceOne_VoiceElevenLabs,
-    AgentUpdateParamsVoiceOne_VoicePlayHt,
+    AzureVoiceUpdateParams,
+    RimeVoiceUpdateParams,
+    ElevenLabsVoiceUpdateParams,
+    PlayHtVoiceUpdateParams,
 ]
```

### Comparing `vocode_api-0.0.8/src/vocode/types/agent_voice.py` & `vocode_api-0.0.9/src/vocode/types/agent_voice.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/azure_voice.py` & `vocode_api-0.0.9/src/vocode/types/azure_voice.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/azure_voice_params.py` & `vocode_api-0.0.9/src/vocode/types/azure_voice_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/azure_voice_update_params.py` & `vocode_api-0.0.9/src/vocode/types/azure_voice_update_params.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
+import typing_extensions
+
 from ..core.datetime_utils import serialize_datetime
 from .azure_voice_update_params_pitch import AzureVoiceUpdateParamsPitch
 from .azure_voice_update_params_rate import AzureVoiceUpdateParamsRate
 from .azure_voice_update_params_voice_name import AzureVoiceUpdateParamsVoiceName
 
 
 class AzureVoiceUpdateParams(pydantic.BaseModel):
+    type: typing_extensions.Literal["voice_azure"]
     voice_name: typing.Optional[AzureVoiceUpdateParamsVoiceName]
     pitch: typing.Optional[AzureVoiceUpdateParamsPitch]
     rate: typing.Optional[AzureVoiceUpdateParamsRate]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `vocode_api-0.0.8/src/vocode/types/call.py` & `vocode_api-0.0.9/src/vocode/types/call.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/call_page.py` & `vocode_api-0.0.9/src/vocode/types/call_page.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/call_status.py` & `vocode_api-0.0.9/src/vocode/types/call_status.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/create_call_agent_params.py` & `vocode_api-0.0.9/src/vocode/types/create_call_agent_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/create_call_agent_params_voice_one.py` & `vocode_api-0.0.9/src/vocode/types/create_call_agent_params_voice_one.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/dtmf_action.py` & `vocode_api-0.0.9/src/vocode/types/dtmf_action.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/dtmf_action_params.py` & `vocode_api-0.0.9/src/vocode/types/play_ht_voice_params.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .empty_action_config import EmptyActionConfig
 
 
-class DtmfActionParams(pydantic.BaseModel):
-    config: typing.Optional[EmptyActionConfig]
+class PlayHtVoiceParams(pydantic.BaseModel):
+    voice_id: str
+    api_user_id: str
+    api_key: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vocode_api-0.0.8/src/vocode/types/dtmf_action_update_params.py` & `vocode_api-0.0.9/src/vocode/types/dtmf_action_update_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/eleven_labs_voice.py` & `vocode_api-0.0.9/src/vocode/types/eleven_labs_voice.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/eleven_labs_voice_params.py` & `vocode_api-0.0.9/src/vocode/types/eleven_labs_voice_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/eleven_labs_voice_update_params.py` & `vocode_api-0.0.9/src/vocode/types/eleven_labs_voice_update_params.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
+import typing_extensions
+
 from ..core.datetime_utils import serialize_datetime
 from .eleven_labs_voice_update_params_api_key import ElevenLabsVoiceUpdateParamsApiKey
 from .eleven_labs_voice_update_params_similarity_boost import ElevenLabsVoiceUpdateParamsSimilarityBoost
 from .eleven_labs_voice_update_params_stability import ElevenLabsVoiceUpdateParamsStability
 from .eleven_labs_voice_update_params_voice_id import ElevenLabsVoiceUpdateParamsVoiceId
 
 
 class ElevenLabsVoiceUpdateParams(pydantic.BaseModel):
+    type: typing_extensions.Literal["voice_eleven_labs"]
     voice_id: typing.Optional[ElevenLabsVoiceUpdateParamsVoiceId]
     stability: typing.Optional[ElevenLabsVoiceUpdateParamsStability]
     similarity_boost: typing.Optional[ElevenLabsVoiceUpdateParamsSimilarityBoost]
     api_key: typing.Optional[ElevenLabsVoiceUpdateParamsApiKey]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vocode_api-0.0.8/src/vocode/types/empty_action_config.py` & `vocode_api-0.0.9/src/vocode/types/empty_action_config.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/end_conversation_action.py` & `vocode_api-0.0.9/src/vocode/types/end_conversation_action.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/end_conversation_action_params.py` & `vocode_api-0.0.9/src/vocode/types/dtmf_action_params.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
+import typing_extensions
+
 from ..core.datetime_utils import serialize_datetime
 from .empty_action_config import EmptyActionConfig
 
 
-class EndConversationActionParams(pydantic.BaseModel):
+class DtmfActionParams(pydantic.BaseModel):
+    type: typing_extensions.Literal["action_dtmf"]
     config: typing.Optional[EmptyActionConfig]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `vocode_api-0.0.8/src/vocode/types/end_conversation_action_update_params.py` & `vocode_api-0.0.9/src/vocode/types/end_conversation_action_update_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/event_type.py` & `vocode_api-0.0.9/src/vocode/types/event_type.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/http_validation_error.py` & `vocode_api-0.0.9/src/vocode/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/language.py` & `vocode_api-0.0.9/src/vocode/types/language.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/normalized_agent.py` & `vocode_api-0.0.9/src/vocode/types/normalized_agent.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/normalized_call.py` & `vocode_api-0.0.9/src/vocode/types/normalized_call.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/normalized_phone_number.py` & `vocode_api-0.0.9/src/vocode/types/normalized_phone_number.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/phone_number.py` & `vocode_api-0.0.9/src/vocode/types/phone_number.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/phone_number_page.py` & `vocode_api-0.0.9/src/vocode/types/phone_number_page.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/pinecone_vector_database.py` & `vocode_api-0.0.9/src/vocode/types/pinecone_vector_database.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/pinecone_vector_database_params.py` & `vocode_api-0.0.9/src/vocode/types/pinecone_vector_database_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/pinecone_vector_database_update_params.py` & `vocode_api-0.0.9/src/vocode/types/pinecone_vector_database_update_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/plan_type.py` & `vocode_api-0.0.9/src/vocode/types/plan_type.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/play_ht_voice.py` & `vocode_api-0.0.9/src/vocode/types/play_ht_voice.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/play_ht_voice_params.py` & `vocode_api-0.0.9/src/vocode/types/rime_voice.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class PlayHtVoiceParams(pydantic.BaseModel):
-    voice_id: str
-    api_user_id: str
-    api_key: str
+class RimeVoice(pydantic.BaseModel):
+    id: str
+    user_id: str
+    speaker: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vocode_api-0.0.8/src/vocode/types/play_ht_voice_update_params.py` & `vocode_api-0.0.9/src/vocode/types/play_ht_voice_update_params.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
+import typing_extensions
+
 from ..core.datetime_utils import serialize_datetime
 from .play_ht_voice_update_params_api_key import PlayHtVoiceUpdateParamsApiKey
 from .play_ht_voice_update_params_api_user_id import PlayHtVoiceUpdateParamsApiUserId
 from .play_ht_voice_update_params_voice_id import PlayHtVoiceUpdateParamsVoiceId
 
 
 class PlayHtVoiceUpdateParams(pydantic.BaseModel):
+    type: typing_extensions.Literal["voice_play_ht"]
     voice_id: typing.Optional[PlayHtVoiceUpdateParamsVoiceId]
     api_user_id: typing.Optional[PlayHtVoiceUpdateParamsApiUserId]
     api_key: typing.Optional[PlayHtVoiceUpdateParamsApiKey]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `vocode_api-0.0.8/src/vocode/types/rime_voice.py` & `vocode_api-0.0.9/src/vocode/types/validation_error.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
+from .validation_error_loc_item import ValidationErrorLocItem
 
 
-class RimeVoice(pydantic.BaseModel):
-    id: str
-    user_id: str
-    speaker: str
+class ValidationError(pydantic.BaseModel):
+    loc: typing.List[ValidationErrorLocItem]
+    msg: str
+    type: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vocode_api-0.0.8/src/vocode/types/rime_voice_params.py` & `vocode_api-0.0.9/src/vocode/types/rime_voice_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/rime_voice_update_params.py` & `vocode_api-0.0.9/src/vocode/types/end_conversation_action_params.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
+import typing_extensions
+
 from ..core.datetime_utils import serialize_datetime
-from .rime_voice_update_params_speaker import RimeVoiceUpdateParamsSpeaker
+from .empty_action_config import EmptyActionConfig
 
 
-class RimeVoiceUpdateParams(pydantic.BaseModel):
-    speaker: typing.Optional[RimeVoiceUpdateParamsSpeaker]
+class EndConversationActionParams(pydantic.BaseModel):
+    type: typing_extensions.Literal["action_end_conversation"]
+    config: typing.Optional[EmptyActionConfig]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vocode_api-0.0.8/src/vocode/types/transfer_call_action.py` & `vocode_api-0.0.9/src/vocode/types/transfer_call_action.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/transfer_call_action_params.py` & `vocode_api-0.0.9/src/vocode/types/transfer_call_action_update_params.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .transfer_call_config import TransferCallConfig
+from .transfer_call_action_update_params_config import TransferCallActionUpdateParamsConfig
 
 
-class TransferCallActionParams(pydantic.BaseModel):
-    config: TransferCallConfig
+class TransferCallActionUpdateParams(pydantic.BaseModel):
+    config: typing.Optional[TransferCallActionUpdateParamsConfig]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vocode_api-0.0.8/src/vocode/types/transfer_call_action_update_params.py` & `vocode_api-0.0.9/src/vocode/types/usage.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,19 +2,22 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .transfer_call_action_update_params_config import TransferCallActionUpdateParamsConfig
+from .plan_type import PlanType
 
 
-class TransferCallActionUpdateParams(pydantic.BaseModel):
-    config: typing.Optional[TransferCallActionUpdateParamsConfig]
+class Usage(pydantic.BaseModel):
+    user_id: str
+    plan_type: PlanType
+    monthly_usage_minutes: int
+    monthly_usage_limit_minutes: int
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vocode_api-0.0.8/src/vocode/types/transfer_call_config.py` & `vocode_api-0.0.9/src/vocode/types/transfer_call_config.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/undefined.py` & `vocode_api-0.0.9/src/vocode/types/undefined.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/usage.py` & `vocode_api-0.0.9/src/vocode/types/rime_voice_update_params.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
+import typing_extensions
+
 from ..core.datetime_utils import serialize_datetime
-from .plan_type import PlanType
+from .rime_voice_update_params_speaker import RimeVoiceUpdateParamsSpeaker
 
 
-class Usage(pydantic.BaseModel):
-    user_id: str
-    plan_type: PlanType
-    monthly_usage_minutes: int
-    monthly_usage_limit_minutes: int
+class RimeVoiceUpdateParams(pydantic.BaseModel):
+    type: typing_extensions.Literal["voice_rime"]
+    speaker: typing.Optional[RimeVoiceUpdateParamsSpeaker]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vocode_api-0.0.8/src/vocode/types/validation_error.py` & `vocode_api-0.0.9/src/vocode/types/webhook_page.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .validation_error_loc_item import ValidationErrorLocItem
+from .webhook import Webhook
 
 
-class ValidationError(pydantic.BaseModel):
-    loc: typing.List[ValidationErrorLocItem]
-    msg: str
-    type: str
+class WebhookPage(pydantic.BaseModel):
+    items: typing.List[Webhook]
+    page: int
+    size: int
+    has_more: bool
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vocode_api-0.0.8/src/vocode/types/voice_page.py` & `vocode_api-0.0.9/src/vocode/types/voice_page.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/voice_page_items_item.py` & `vocode_api-0.0.9/src/vocode/types/voice_page_items_item.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/voice_params_request.py` & `vocode_api-0.0.9/src/vocode/types/voice_params_request.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/voice_response_model.py` & `vocode_api-0.0.9/src/vocode/types/voice_response_model.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/voice_update_params_request.py` & `vocode_api-0.0.9/src/vocode/types/voice_update_params_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,48 +9,40 @@
 from .azure_voice_update_params import AzureVoiceUpdateParams
 from .eleven_labs_voice_update_params import ElevenLabsVoiceUpdateParams
 from .play_ht_voice_update_params import PlayHtVoiceUpdateParams
 from .rime_voice_update_params import RimeVoiceUpdateParams
 
 
 class VoiceUpdateParamsRequest_VoiceAzure(AzureVoiceUpdateParams):
-    type: typing_extensions.Literal["voice_azure"]
-
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
 
 
 class VoiceUpdateParamsRequest_VoiceRime(RimeVoiceUpdateParams):
-    type: typing_extensions.Literal["voice_rime"]
-
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
 
 
 class VoiceUpdateParamsRequest_VoiceElevenLabs(ElevenLabsVoiceUpdateParams):
-    type: typing_extensions.Literal["voice_eleven_labs"]
-
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
 
 
 class VoiceUpdateParamsRequest_VoicePlayHt(PlayHtVoiceUpdateParams):
-    type: typing_extensions.Literal["voice_play_ht"]
-
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
 
 
 VoiceUpdateParamsRequest = typing.Union[
-    VoiceUpdateParamsRequest_VoiceAzure,
-    VoiceUpdateParamsRequest_VoiceRime,
-    VoiceUpdateParamsRequest_VoiceElevenLabs,
-    VoiceUpdateParamsRequest_VoicePlayHt,
+    AzureVoiceUpdateParams,
+    RimeVoiceUpdateParams,
+    ElevenLabsVoiceUpdateParams,
+    PlayHtVoiceUpdateParams,
 ]
```

### Comparing `vocode_api-0.0.8/src/vocode/types/webhook.py` & `vocode_api-0.0.9/src/vocode/types/webhook.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/src/vocode/types/webhook_page.py` & `vocode_api-0.0.9/src/vocode/types/webhook_params.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .webhook import Webhook
+from .event_type import EventType
+from .http_method import HttpMethod
 
 
-class WebhookPage(pydantic.BaseModel):
-    items: typing.List[Webhook]
-    page: int
-    size: int
-    has_more: bool
+class WebhookParams(pydantic.BaseModel):
+    subscriptions: typing.List[EventType]
+    url: str
+    method: typing.Optional[HttpMethod]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vocode_api-0.0.8/src/vocode/types/webhook_update_params.py` & `vocode_api-0.0.9/src/vocode/types/webhook_update_params.py`

 * *Files identical despite different names*

### Comparing `vocode_api-0.0.8/PKG-INFO` & `vocode_api-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vocode-api
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

