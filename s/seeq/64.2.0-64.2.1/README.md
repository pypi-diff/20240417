# Comparing `tmp/seeq-64.2.0.tar.gz` & `tmp/seeq-64.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seeq-64.2.0.tar", last modified: Thu Apr  4 21:35:31 2024, max compression
+gzip compressed data, was "seeq-64.2.1.tar", last modified: Wed Apr 17 04:38:09 2024, max compression
```

## Comparing `seeq-64.2.0.tar` & `seeq-64.2.1.tar`

### file list

```diff
@@ -1,447 +1,447 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-04 21:35:31.735692 seeq-64.2.0/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    33136 2024-04-04 20:20:12.000000 seeq-64.2.0/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-04-04 20:20:12.000000 seeq-64.2.0/MANIFEST.in
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3869 2024-04-04 21:35:31.731691 seeq-64.2.0/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3317 2024-04-04 20:20:12.000000 seeq-64.2.0/README.md
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-04 20:20:12.000000 seeq-64.2.0/pyproject.toml
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-04 21:35:31.691691 seeq-64.2.0/seeq/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-04 21:35:31.695691 seeq-64.2.0/seeq/sdk/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    26736 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-04 21:35:31.699691 seeq-64.2.0/seeq/sdk/api/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2159 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15396 2024-04-04 20:24:51.000000 seeq-64.2.0/seeq/sdk/api/access_keys_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    29293 2024-04-04 20:24:51.000000 seeq-64.2.0/seeq/sdk/api/add_ons_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   139189 2024-04-04 20:24:51.000000 seeq-64.2.0/seeq/sdk/api/agents_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    54975 2024-04-04 20:24:51.000000 seeq-64.2.0/seeq/sdk/api/annotations_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24078 2024-04-04 20:24:51.000000 seeq-64.2.0/seeq/sdk/api/assets_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5137 2024-04-04 20:24:51.000000 seeq-64.2.0/seeq/sdk/api/assistants_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8202 2024-04-04 20:24:51.000000 seeq-64.2.0/seeq/sdk/api/audit_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21842 2024-04-04 20:24:51.000000 seeq-64.2.0/seeq/sdk/api/auth_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27275 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/condition_monitors_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    52130 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/conditions_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   126123 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/content_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    83478 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/context_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    34507 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/datafiles_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    50775 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/datasources_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    25032 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/display_templates_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24305 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/displays_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    30080 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/export_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    50560 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/folders_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   107321 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/formulas_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5495 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/graph_ql_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   181052 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/items_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    35736 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/jobs_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21471 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/logs_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24612 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/metrics_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    32019 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/monitors_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5962 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/networks_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    33687 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/notification_configurations_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10156 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/notifier_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21444 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/plugins_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    35456 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/projects_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24605 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/report_templates_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5758 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/reports_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    38193 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/requests_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28492 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/scalars_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17482 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/scim_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   110312 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/signals_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20586 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/subscriptions_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   104888 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/system_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    45820 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/table_definitions_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    66306 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/trees_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8652 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/unstable_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12944 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/usage_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    52327 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/user_groups_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    49735 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/users_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    94800 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api/workbooks_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    32200 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/api_client.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9343 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/configuration.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-04 21:35:31.731691 seeq-64.2.0/seeq/sdk/models/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    22014 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/models/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4286 2024-04-04 20:24:44.000000 seeq-64.2.0/seeq/sdk/models/access_key_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7328 2024-04-04 20:24:44.000000 seeq-64.2.0/seeq/sdk/models/access_key_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14440 2024-04-04 20:24:44.000000 seeq-64.2.0/seeq/sdk/models/access_key_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4107 2024-04-04 20:24:44.000000 seeq-64.2.0/seeq/sdk/models/ace_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5730 2024-04-04 20:24:44.000000 seeq-64.2.0/seeq/sdk/models/ace_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6786 2024-04-04 20:24:44.000000 seeq-64.2.0/seeq/sdk/models/acl_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6589 2024-04-04 20:24:44.000000 seeq-64.2.0/seeq/sdk/models/acl_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3601 2024-04-04 20:24:44.000000 seeq-64.2.0/seeq/sdk/models/activity_graph_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7375 2024-04-04 20:24:44.000000 seeq-64.2.0/seeq/sdk/models/activity_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8578 2024-04-04 20:24:45.000000 seeq-64.2.0/seeq/sdk/models/add_on_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7271 2024-04-04 20:24:45.000000 seeq-64.2.0/seeq/sdk/models/add_on_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15975 2024-04-04 20:24:45.000000 seeq-64.2.0/seeq/sdk/models/add_on_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7513 2024-04-04 20:24:45.000000 seeq-64.2.0/seeq/sdk/models/add_on_preview_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6530 2024-04-04 20:24:45.000000 seeq-64.2.0/seeq/sdk/models/add_on_preview_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11088 2024-04-04 20:24:45.000000 seeq-64.2.0/seeq/sdk/models/add_on_tool_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17343 2024-04-04 20:24:45.000000 seeq-64.2.0/seeq/sdk/models/add_on_tool_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4143 2024-04-04 20:24:45.000000 seeq-64.2.0/seeq/sdk/models/administrator_contact_information_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4853 2024-04-04 20:24:45.000000 seeq-64.2.0/seeq/sdk/models/agent_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3128 2024-04-04 20:24:45.000000 seeq-64.2.0/seeq/sdk/models/agent_key_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7460 2024-04-04 20:24:45.000000 seeq-64.2.0/seeq/sdk/models/agent_orchestrator_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13856 2024-04-04 20:24:45.000000 seeq-64.2.0/seeq/sdk/models/agent_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8806 2024-04-04 20:24:45.000000 seeq-64.2.0/seeq/sdk/models/agent_status_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7833 2024-04-04 20:24:45.000000 seeq-64.2.0/seeq/sdk/models/agent_status_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4282 2024-04-04 20:24:45.000000 seeq-64.2.0/seeq/sdk/models/annotation_image_link_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11035 2024-04-04 20:24:45.000000 seeq-64.2.0/seeq/sdk/models/annotation_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4225 2024-04-04 20:24:45.000000 seeq-64.2.0/seeq/sdk/models/annotation_interest_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3750 2024-04-04 20:24:45.000000 seeq-64.2.0/seeq/sdk/models/annotation_interest_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7392 2024-04-04 20:24:45.000000 seeq-64.2.0/seeq/sdk/models/annotation_list_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    34976 2024-04-04 20:24:45.000000 seeq-64.2.0/seeq/sdk/models/annotation_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4433 2024-04-04 20:24:45.000000 seeq-64.2.0/seeq/sdk/models/archive_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4176 2024-04-04 20:24:45.000000 seeq-64.2.0/seeq/sdk/models/asset_batch_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4667 2024-04-04 20:24:45.000000 seeq-64.2.0/seeq/sdk/models/asset_error.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14717 2024-04-04 20:24:45.000000 seeq-64.2.0/seeq/sdk/models/asset_group_asset_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4038 2024-04-04 20:24:45.000000 seeq-64.2.0/seeq/sdk/models/asset_group_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3969 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/asset_group_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13792 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/asset_group_root_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6462 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/asset_group_tree_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11760 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/asset_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17564 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/asset_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8465 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/asset_selection_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13114 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/asset_selection_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7086 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/asset_tree_batch_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11209 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/asset_tree_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4432 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/asset_tree_single_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4890 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/assistant_status_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4866 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/attachment_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8190 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/audit_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9644 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/audit_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7075 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/auth_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3442 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/auth_providers_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4444 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/authoritative_region_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2455 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/boolean_configuration_field_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9542 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/cache_block.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4089 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/cache_info_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20746 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/calculated_item_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5332 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/capsule_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4348 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/capsule_property_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4161 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/capsule_property_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7480 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/capsule_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3259 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/capsules_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10294 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/capsules_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4020 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/capsules_overwrite_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7228 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/channel_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4181 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/column_definition_input_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8308 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/column_definition_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7370 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/column_definition_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4700 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/column_rule_ancestor_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4577 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/column_rule_concat_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3634 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/column_rule_event_property_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6087 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/column_rule_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4507 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/column_rule_item_property_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5485 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/column_rule_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5213 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/column_rule_path_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3409 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/condition_batch_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20503 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/condition_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9576 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/condition_monitor_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11131 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/condition_monitor_notification_configuration_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19957 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/condition_monitor_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9233 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/condition_notification_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6660 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/condition_notification_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24429 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/condition_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23781 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/condition_update_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7750 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/configuration_field_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4064 2024-04-04 20:24:46.000000 seeq-64.2.0/seeq/sdk/models/configuration_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4276 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/configuration_option_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3748 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/configuration_option_output_simple_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12329 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/configuration_option_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8813 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/configuration_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4959 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/configured_directives_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8527 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/connection_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27327 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/connection_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18799 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/connection_status_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16922 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/connection_status_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3253 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/connections_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4941 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/connector_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14854 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/connector_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3273 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/connectors_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15681 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/content_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    22574 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/content_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5298 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/content_with_metadata_list_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28438 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/content_with_metadata_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4040 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/context_comment_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9457 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/context_comment_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4025 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/context_label_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11193 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/context_label_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4920 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/context_opaque_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10177 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/context_opaque_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3446 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/csv_datafile_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    50145 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/datafile_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    53738 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/datafile_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3115 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/datafiles_csv_body.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9607 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/datasource_clean_up_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4283 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/datasource_clean_up_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13246 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/datasource_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7504 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/datasource_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20066 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/datasource_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8806 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/datasource_preview_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15846 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/datasource_statistics_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8689 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/datasource_status_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9118 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/datasource_status_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28984 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/datasource_summary_status_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11225 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/datasources_status_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9723 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/date_range_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16890 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/date_range_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4111 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/debug_cache_block_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4868 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/detailed_meter_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5727 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/detailed_timer_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5047 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/directive_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5244 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/display_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7354 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/display_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14727 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/display_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9431 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/display_template_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7791 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/display_template_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15926 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/display_template_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4899 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/document_backup_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4138 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/double_configuration_field_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5405 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/email_notification_recipient_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6366 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/emailer_configuration_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5314 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/export_item_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21966 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/export_items_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18512 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/export_items_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7286 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/export_preview_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10723 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/export_preview_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6490 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/folded_stack_node_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7686 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/folder_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5698 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/folder_navigation_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15863 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/folder_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3957 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/formula_compile_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6875 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/formula_compile_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8113 2024-04-04 20:24:47.000000 seeq-64.2.0/seeq/sdk/models/formula_compiler_error_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4330 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/formula_dependency_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4006 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/formula_doc_example_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3464 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/formula_doc_example_list_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7389 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/formula_doc_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3415 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/formula_doc_keyword_list_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21607 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/formula_doc_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3228 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/formula_doc_summaries_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8265 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/formula_doc_summary_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8265 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/formula_error_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3952 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/formula_example_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18896 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/formula_item_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20492 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/formula_item_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3933 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/formula_log_entry.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3718 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/formula_log_entry_details.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4453 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/formula_log_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6771 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/formula_package_import_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6060 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/formula_package_import_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9360 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/formula_package_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17867 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/formula_package_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6189 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/formula_parameter_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5572 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/formula_parameter_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12864 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/formula_run_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12280 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/formula_run_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4077 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/formula_token.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4064 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/formula_update_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4108 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/formula_upgrade_change_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4932 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/formula_upgrade_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13617 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/function_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4594 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/function_parameter_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6327 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/function_variant_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4834 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/gauge_datum_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4157 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/generic_table_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3286 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/get_add_on_tools_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7344 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/get_channels_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9186 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/get_condition_monitor_items_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7561 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/get_content_items_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7469 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/get_date_ranges_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7136 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/get_jobs_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7319 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/get_metrics_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7348 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/get_projects_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4191 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/get_request_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3122 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/get_requests_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6221 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/get_sample_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11225 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/get_samples_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7292 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/get_signals_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3806 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/graph_ql_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3765 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/graph_ql_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3087 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/id_images_body.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3541 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/identity_mapping_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6253 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/identity_mapping_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8348 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/identity_preview_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12927 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/identity_preview_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4212 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/indexing_parameters_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4947 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/installer_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4136 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/interval_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2997 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/invalid_swap_out_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5360 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/item_batch_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11549 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/item_dependency_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7047 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/item_finder_configuration_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8479 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/item_finder_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7639 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/item_finder_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15489 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/item_finder_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3168 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/item_id_list_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14649 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/item_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11275 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/item_parameter_of_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8178 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/item_preview_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6934 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/item_preview_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9485 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/item_preview_with_assets_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4196 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/item_search_preview_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8661 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/item_search_preview_paginated_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16178 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/item_search_preview_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4708 2024-04-04 20:24:48.000000 seeq-64.2.0/seeq/sdk/models/item_swap_result_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6537 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/item_update_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4220 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/item_user_attributes_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5888 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/item_user_attributes_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5144 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/item_with_swap_pairs_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4395 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/jira_attachment.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6025 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/jira_attachment_media_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6230 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/job_accepted_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14001 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/job_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4845 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/json_backup_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3798 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/label_category_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3222 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/label_category_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4490 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/label_category_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4621 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/label_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3062 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/label_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5063 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/label_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4381 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/license_importer_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13507 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/license_status_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6191 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/licensed_feature_status_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4668 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/log_message.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4136 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/long_configuration_field_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4693 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/meter_datum_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3177 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/migrate_editor_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4779 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/monitor_definition_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3420 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/monitor_definitions_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4520 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/monitor_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3189 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/monitor_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13074 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/monitor_values.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3164 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/monitors_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8926 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/notifiable_report_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8191 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/notifiable_report_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12017 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/notification_configuration_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6065 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/optional_report_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6206 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/parameter_doc_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4124 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/permissions_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8236 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/plugin_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16602 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/plugin_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3084 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/plugins_body.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6354 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/pre_provision_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3980 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/pre_provision_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4929 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/priority_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4011 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/progress_information_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10158 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/project_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20788 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/project_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4255 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/property_href_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4582 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/property_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6492 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/property_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5041 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/provision_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13320 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/put_asset_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19360 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/put_scalar_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7198 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/put_scalars_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3288 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/put_signals_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3413 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/put_user_groups_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3276 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/referenced_items_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11239 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/regression_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4575 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/remote_agent_directives_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16599 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/remote_agent_status_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16708 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/remote_agent_status_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5135 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/report_input_item_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4810 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/report_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8329 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/report_notification_configuration_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6225 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/report_template_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15217 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/report_template_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15198 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/request_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4385 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/sample_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4453 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/sample_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3237 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/samples_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3501 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/samples_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3994 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/samples_overwrite_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11225 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/scalar_evaluate_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17724 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/scalar_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5290 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/scalar_property_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4748 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/scalar_value_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4542 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/scale_across_tree_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8516 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/schedulable_admin_list_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16074 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/schedulable_admin_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4210 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/schedulable_summary_day_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3331 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/schedulable_summary_week_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4216 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/schedule_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4974 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/schedule_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9394 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/scheduled_notebook_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4611 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/scheduled_notebook_list_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20104 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/scheduled_notebook_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4186 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/scim_token_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4325 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/screenshot_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4142 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/secret_configuration_field_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5699 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/see_also_doc_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4926 2024-04-04 20:24:49.000000 seeq-64.2.0/seeq/sdk/models/send_email_attachment_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3804 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/send_email_contact_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7956 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/send_email_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5175 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/sent_email_attachment_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12471 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/sent_email_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3347 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/sent_emails_list_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3349 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/server_build_info_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4641 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/server_load_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6420 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/server_spec_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11947 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/server_status_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18077 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/signal_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27753 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/signal_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23062 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/signal_with_id_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3267 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/status_message.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3515 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/status_message_base.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3788 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/store_secret_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4142 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/string_configuration_field_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4368 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/subscription_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4908 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/subscription_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3389 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/subscription_update_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10912 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/support_request_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4180 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/support_request_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4302 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/supported_units_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4209 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/swap_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3559 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/swap_option_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5575 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/swap_option_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3784 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/swap_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11724 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/sync_progress.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18924 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/sync_progress_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3122 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/system_license_body.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4800 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/table_column_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10792 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/table_definition_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7909 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/table_definition_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16936 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/table_definition_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5426 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/table_definition_update_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19125 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/threshold_metric_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28187 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/threshold_metric_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5042 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/threshold_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4793 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/timer_datum_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20067 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/tree_item_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7244 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/treemap_item_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10190 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/treemap_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3553 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/units_of_measure_batch_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4051 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/units_of_measure_item_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3472 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/units_of_measure_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11015 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/unsubscribe_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4193 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/usage_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10238 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/usage_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3055 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/usage_types_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9888 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/user_group_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19622 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/user_group_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13170 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/user_group_with_id_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18031 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/user_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8124 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/user_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    29747 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/user_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4241 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/user_password_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5463 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/validate_cron_list_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3332 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/validate_cron_list_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7088 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/validate_cron_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9328 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/workbench_item_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20603 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/workbench_search_result_preview_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8268 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/workbook_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7400 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/workbook_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16804 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/workbook_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6769 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/worksheet_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7452 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/worksheet_output_list_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14268 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/worksheet_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3232 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/workstep_input_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13818 2024-04-04 20:24:50.000000 seeq-64.2.0/seeq/sdk/models/workstep_output_v1.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13450 2024-04-04 20:24:52.000000 seeq-64.2.0/seeq/sdk/rest.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-04 21:35:31.691691 seeq-64.2.0/seeq.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3869 2024-04-04 21:35:31.000000 seeq-64.2.0/seeq.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17759 2024-04-04 21:35:31.000000 seeq-64.2.0/seeq.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-04 21:35:31.000000 seeq-64.2.0/seeq.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-04 21:35:31.000000 seeq-64.2.0/seeq.egg-info/not-zip-safe
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       86 2024-04-04 21:35:31.000000 seeq-64.2.0/seeq.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        5 2024-04-04 21:35:31.000000 seeq-64.2.0/seeq.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-04 21:35:31.735692 seeq-64.2.0/setup.cfg
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1192 2024-04-04 20:22:02.000000 seeq-64.2.0/setup.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-17 04:38:09.845468 seeq-64.2.1/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    33136 2024-04-17 03:25:29.000000 seeq-64.2.1/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       18 2024-04-17 03:25:29.000000 seeq-64.2.1/MANIFEST.in
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3869 2024-04-17 04:38:09.845468 seeq-64.2.1/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3317 2024-04-17 03:25:29.000000 seeq-64.2.1/README.md
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-17 03:25:29.000000 seeq-64.2.1/pyproject.toml
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-17 04:38:09.809467 seeq-64.2.1/seeq/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-17 04:38:09.809467 seeq-64.2.1/seeq/sdk/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    26736 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-17 04:38:09.813468 seeq-64.2.1/seeq/sdk/api/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2159 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15396 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/access_keys_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    29293 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/add_ons_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   139189 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/agents_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    54975 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/annotations_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24078 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/assets_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5137 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/assistants_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8202 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/audit_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21842 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/auth_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27275 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/condition_monitors_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    52130 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/conditions_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   126123 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/content_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    83478 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/context_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    34507 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/datafiles_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    50775 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/datasources_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    25032 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/display_templates_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24305 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/displays_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    30080 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/export_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    50560 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/folders_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   107321 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/formulas_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5495 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/graph_ql_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   181052 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/items_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    35736 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/jobs_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21471 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/logs_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24612 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/metrics_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    32019 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/monitors_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5962 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/networks_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    33687 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/notification_configurations_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10156 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/notifier_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21444 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/plugins_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    35456 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/projects_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24605 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/report_templates_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5758 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/reports_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    38193 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/requests_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28492 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/scalars_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17482 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/scim_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   110312 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/signals_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20586 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/subscriptions_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   104888 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/system_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    45820 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/table_definitions_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    66306 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/trees_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8652 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/unstable_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12944 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/usage_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    52327 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/user_groups_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    49735 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/users_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    94800 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api/workbooks_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    32200 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/api_client.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9343 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/configuration.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-17 04:38:09.845468 seeq-64.2.1/seeq/sdk/models/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    22014 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4286 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/access_key_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7328 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/access_key_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14440 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/access_key_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4107 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/ace_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5730 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/ace_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6786 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/acl_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6589 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/acl_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3601 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/activity_graph_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7375 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/activity_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8578 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/add_on_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7271 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/add_on_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15975 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/add_on_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7513 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/add_on_preview_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6530 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/add_on_preview_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11088 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/add_on_tool_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17343 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/add_on_tool_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4143 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/administrator_contact_information_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4853 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/agent_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3128 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/agent_key_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7460 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/agent_orchestrator_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13856 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/agent_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8806 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/agent_status_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7833 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/agent_status_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4282 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/annotation_image_link_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11035 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/annotation_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4225 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/annotation_interest_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3750 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/annotation_interest_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7392 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/annotation_list_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    34976 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/annotation_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4433 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/archive_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4176 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/asset_batch_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4667 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/asset_error.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14717 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/asset_group_asset_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4038 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/asset_group_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3969 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/asset_group_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13792 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/asset_group_root_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6462 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/asset_group_tree_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11760 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/asset_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17564 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/asset_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8465 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/asset_selection_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13114 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/asset_selection_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7086 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/asset_tree_batch_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11209 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/asset_tree_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4432 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/asset_tree_single_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4890 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/assistant_status_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4866 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/attachment_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8190 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/audit_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9644 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/audit_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7075 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/auth_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3442 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/auth_providers_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4444 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/authoritative_region_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2455 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/boolean_configuration_field_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9542 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/cache_block.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4089 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/cache_info_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20746 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/calculated_item_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5332 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/capsule_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4348 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/capsule_property_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4161 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/capsule_property_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7480 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/capsule_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3259 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/capsules_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10294 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/capsules_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4020 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/capsules_overwrite_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7228 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/channel_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4181 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/column_definition_input_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8308 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/column_definition_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7370 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/column_definition_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4700 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/column_rule_ancestor_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4577 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/column_rule_concat_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3634 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/column_rule_event_property_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6087 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/column_rule_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4507 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/column_rule_item_property_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5485 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/column_rule_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5213 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/column_rule_path_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3409 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/condition_batch_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20503 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/condition_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9576 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/condition_monitor_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11131 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/condition_monitor_notification_configuration_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19957 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/condition_monitor_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9233 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/condition_notification_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6660 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/condition_notification_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    24429 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/condition_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23781 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/condition_update_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7750 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/configuration_field_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4064 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/configuration_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4276 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/configuration_option_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3748 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/configuration_option_output_simple_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12329 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/configuration_option_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8813 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/configuration_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4959 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/configured_directives_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8527 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/connection_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27327 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/connection_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18799 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/connection_status_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16922 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/connection_status_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3253 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/connections_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4941 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/connector_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14854 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/connector_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3273 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/connectors_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15681 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/content_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    22574 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/content_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5298 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/content_with_metadata_list_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28438 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/content_with_metadata_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4040 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/context_comment_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9457 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/context_comment_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4025 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/context_label_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11193 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/context_label_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4920 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/context_opaque_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10177 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/context_opaque_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3446 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/csv_datafile_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    50145 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/datafile_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    53738 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/datafile_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3115 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/datafiles_csv_body.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9607 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/datasource_clean_up_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4283 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/datasource_clean_up_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13246 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/datasource_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7504 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/datasource_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20066 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/datasource_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8806 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/datasource_preview_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15846 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/datasource_statistics_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8689 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/datasource_status_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9118 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/datasource_status_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28984 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/datasource_summary_status_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11225 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/datasources_status_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9723 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/date_range_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16890 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/date_range_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4111 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/debug_cache_block_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4868 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/detailed_meter_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5727 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/detailed_timer_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5047 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/directive_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5244 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/display_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7354 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/display_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14727 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/display_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9431 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/display_template_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7791 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/display_template_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15926 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/display_template_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4899 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/document_backup_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4138 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/double_configuration_field_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5405 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/email_notification_recipient_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6366 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/emailer_configuration_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5314 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/export_item_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21966 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/export_items_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18512 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/export_items_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7286 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/export_preview_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10723 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/export_preview_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6490 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/folded_stack_node_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7686 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/folder_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5698 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/folder_navigation_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15863 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/folder_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4035 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/formula_compile_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6875 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/formula_compile_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8113 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/formula_compiler_error_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4330 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/formula_dependency_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4006 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/formula_doc_example_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3464 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/formula_doc_example_list_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7389 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/formula_doc_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3415 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/formula_doc_keyword_list_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    21607 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/formula_doc_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3228 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/formula_doc_summaries_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8265 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/formula_doc_summary_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8265 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/formula_error_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3952 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/formula_example_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18896 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/formula_item_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20492 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/formula_item_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3933 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/formula_log_entry.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3718 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/formula_log_entry_details.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4453 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/formula_log_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6771 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/formula_package_import_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6060 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/formula_package_import_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9360 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/formula_package_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17867 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/formula_package_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6189 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/formula_parameter_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5572 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/formula_parameter_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12942 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/formula_run_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12280 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/formula_run_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4077 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/formula_token.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4064 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/formula_update_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4108 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/formula_upgrade_change_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4932 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/formula_upgrade_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13617 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/function_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4594 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/function_parameter_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6327 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/function_variant_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4834 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/gauge_datum_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4157 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/generic_table_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3286 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/get_add_on_tools_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7344 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/get_channels_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9186 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/get_condition_monitor_items_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7561 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/get_content_items_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7469 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/get_date_ranges_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7136 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/get_jobs_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7319 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/get_metrics_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7348 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/get_projects_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4191 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/get_request_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3122 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/get_requests_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6221 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/get_sample_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11225 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/get_samples_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7292 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/get_signals_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3806 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/graph_ql_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3765 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/graph_ql_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3087 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/id_images_body.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3541 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/identity_mapping_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6253 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/identity_mapping_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8348 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/identity_preview_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12927 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/identity_preview_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4212 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/indexing_parameters_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4947 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/installer_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4136 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/interval_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2997 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/invalid_swap_out_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5360 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/item_batch_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11549 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/item_dependency_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7047 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/item_finder_configuration_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8479 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/item_finder_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7639 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/item_finder_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15489 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/item_finder_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3168 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/item_id_list_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14649 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/item_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11275 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/item_parameter_of_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8178 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/item_preview_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6934 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/item_preview_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9485 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/item_preview_with_assets_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4196 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/item_search_preview_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8661 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/item_search_preview_paginated_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16178 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/item_search_preview_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4708 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/item_swap_result_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6537 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/item_update_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4220 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/item_user_attributes_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5888 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/item_user_attributes_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5144 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/item_with_swap_pairs_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4395 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/jira_attachment.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6025 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/jira_attachment_media_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6230 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/job_accepted_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14001 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/job_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4845 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/json_backup_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3798 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/label_category_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3222 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/label_category_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4490 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/label_category_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4621 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/label_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3062 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/label_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5063 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/label_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4381 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/license_importer_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13507 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/license_status_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6191 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/licensed_feature_status_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4668 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/log_message.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4136 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/long_configuration_field_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4693 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/meter_datum_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3177 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/migrate_editor_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4779 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/monitor_definition_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3420 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/monitor_definitions_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4520 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/monitor_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3189 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/monitor_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13074 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/monitor_values.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3164 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/monitors_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8926 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/notifiable_report_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8191 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/notifiable_report_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12017 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/notification_configuration_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6065 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/optional_report_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6206 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/parameter_doc_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4124 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/permissions_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8236 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/plugin_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16602 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/plugin_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3084 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/plugins_body.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6354 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/pre_provision_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3980 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/pre_provision_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4929 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/priority_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4011 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/progress_information_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10158 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/project_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20788 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/project_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4255 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/property_href_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4582 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/property_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6492 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/property_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5041 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/provision_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13320 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/put_asset_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19360 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/put_scalar_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7198 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/put_scalars_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3288 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/put_signals_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3413 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/put_user_groups_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3276 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/referenced_items_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11239 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/regression_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4575 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/remote_agent_directives_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16599 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/remote_agent_status_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16708 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/remote_agent_status_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5135 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/report_input_item_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4810 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/report_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8329 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/report_notification_configuration_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6225 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/report_template_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15217 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/report_template_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15198 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/request_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4385 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/sample_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4453 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/sample_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3237 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/samples_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3501 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/samples_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3994 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/samples_overwrite_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11225 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/scalar_evaluate_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17724 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/scalar_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5290 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/scalar_property_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4748 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/scalar_value_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4542 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/scale_across_tree_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8516 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/schedulable_admin_list_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16074 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/schedulable_admin_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4210 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/schedulable_summary_day_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3331 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/schedulable_summary_week_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4216 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/schedule_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4974 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/schedule_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9394 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/scheduled_notebook_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4611 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/scheduled_notebook_list_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20104 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/scheduled_notebook_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4186 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/scim_token_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4325 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/screenshot_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4142 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/secret_configuration_field_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5699 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/see_also_doc_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4926 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/send_email_attachment_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3804 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/send_email_contact_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7956 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/send_email_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5175 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/sent_email_attachment_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12471 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/sent_email_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3347 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/sent_emails_list_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3349 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/server_build_info_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4641 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/server_load_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6420 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/server_spec_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11947 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/server_status_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18077 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/signal_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    27753 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/signal_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    23062 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/signal_with_id_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3267 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/status_message.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3515 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/status_message_base.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3788 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/store_secret_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4142 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/string_configuration_field_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4368 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/subscription_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4908 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/subscription_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3389 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/subscription_update_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10912 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/support_request_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4180 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/support_request_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4302 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/supported_units_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4209 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/swap_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3559 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/swap_option_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5575 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/swap_option_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3784 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/swap_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11724 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/sync_progress.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18924 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/sync_progress_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3122 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/system_license_body.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4800 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/table_column_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10792 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/table_definition_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7909 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/table_definition_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16936 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/table_definition_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5426 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/table_definition_update_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19125 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/threshold_metric_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    28187 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/threshold_metric_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5042 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/threshold_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4793 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/timer_datum_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20067 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/tree_item_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7244 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/treemap_item_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10190 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/treemap_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3553 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/units_of_measure_batch_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4051 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/units_of_measure_item_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3472 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/units_of_measure_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11015 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/unsubscribe_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4193 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/usage_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10238 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/usage_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3055 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/usage_types_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9888 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/user_group_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    19622 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/user_group_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13170 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/user_group_with_id_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18031 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/user_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8124 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/user_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    29747 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/user_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4241 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/user_password_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5463 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/validate_cron_list_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3332 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/validate_cron_list_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7088 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/validate_cron_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9328 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/workbench_item_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20603 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/workbench_search_result_preview_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8268 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/workbook_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7400 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/workbook_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16804 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/workbook_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6769 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/worksheet_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7452 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/worksheet_output_list_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14268 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/worksheet_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3232 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/workstep_input_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13818 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/models/workstep_output_v1.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13450 2024-04-17 03:28:35.000000 seeq-64.2.1/seeq/sdk/rest.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-17 04:38:09.809467 seeq-64.2.1/seeq.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3869 2024-04-17 04:38:09.000000 seeq-64.2.1/seeq.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17759 2024-04-17 04:38:09.000000 seeq-64.2.1/seeq.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-17 04:38:09.000000 seeq-64.2.1/seeq.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-17 04:38:09.000000 seeq-64.2.1/seeq.egg-info/not-zip-safe
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       86 2024-04-17 04:38:09.000000 seeq-64.2.1/seeq.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        5 2024-04-17 04:38:09.000000 seeq-64.2.1/seeq.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-17 04:38:09.845468 seeq-64.2.1/setup.cfg
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1192 2024-04-17 03:27:15.000000 seeq-64.2.1/setup.py
```

### Comparing `seeq-64.2.0/LICENSE` & `seeq-64.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seeq-64.2.0/PKG-INFO` & `seeq-64.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeq
-Version: 64.2.0
+Version: 64.2.1
 Summary: The Seeq SDK for Python
 Home-page: https://www.seeq.com
 Author: Seeq Corporation
 Author-email: support@seeq.com
 Project-URL: Documentation, https://python-docs.seeq.com/
 Project-URL: Changelog, https://python-docs.seeq.com/changelog.html
 Classifier: Programming Language :: Python :: 2
```

### Comparing `seeq-64.2.0/README.md` & `seeq-64.2.1/README.md`

 * *Files identical despite different names*

### Comparing `seeq-64.2.0/seeq/sdk/__init__.py` & `seeq-64.2.1/seeq/sdk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
-__version__ = "64.2.0"
+__version__ = "64.2.1"
 
 # import apis into sdk package
 from .api.access_keys_api import AccessKeysApi
 from .api.add_ons_api import AddOnsApi
 from .api.agents_api import AgentsApi
 from .api.annotations_api import AnnotationsApi
 from .api.assets_api import AssetsApi
```

### Comparing `seeq-64.2.0/seeq/sdk/api/__init__.py` & `seeq-64.2.1/seeq/sdk/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
-__version__ = "64.2.0"
+__version__ = "64.2.1"
 
 # import apis into sdk package
 from .access_keys_api import AccessKeysApi
 from .add_ons_api import AddOnsApi
 from .agents_api import AgentsApi
 from .annotations_api import AnnotationsApi
 from .assets_api import AssetsApi
```

### Comparing `seeq-64.2.0/seeq/sdk/api/access_keys_api.py` & `seeq-64.2.1/seeq/sdk/api/access_keys_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/add_ons_api.py` & `seeq-64.2.1/seeq/sdk/api/add_ons_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/agents_api.py` & `seeq-64.2.1/seeq/sdk/api/agents_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/annotations_api.py` & `seeq-64.2.1/seeq/sdk/api/annotations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/assets_api.py` & `seeq-64.2.1/seeq/sdk/api/assets_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/assistants_api.py` & `seeq-64.2.1/seeq/sdk/api/assistants_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/audit_api.py` & `seeq-64.2.1/seeq/sdk/api/audit_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/auth_api.py` & `seeq-64.2.1/seeq/sdk/api/auth_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/condition_monitors_api.py` & `seeq-64.2.1/seeq/sdk/api/condition_monitors_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/conditions_api.py` & `seeq-64.2.1/seeq/sdk/api/conditions_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/content_api.py` & `seeq-64.2.1/seeq/sdk/api/content_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/context_api.py` & `seeq-64.2.1/seeq/sdk/api/context_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/datafiles_api.py` & `seeq-64.2.1/seeq/sdk/api/datafiles_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/datasources_api.py` & `seeq-64.2.1/seeq/sdk/api/datasources_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/display_templates_api.py` & `seeq-64.2.1/seeq/sdk/api/display_templates_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/displays_api.py` & `seeq-64.2.1/seeq/sdk/api/displays_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/export_api.py` & `seeq-64.2.1/seeq/sdk/api/export_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/folders_api.py` & `seeq-64.2.1/seeq/sdk/api/folders_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/formulas_api.py` & `seeq-64.2.1/seeq/sdk/api/formulas_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 00000050: 7920 5377 6167 6765 7220 436f 6465 6765  y Swagger Codege
 00000060: 6e20 6874 7470 733a 2f2f 6769 7468 7562  n https://github
 00000070: 2e63 6f6d 2f73 7761 6767 6572 2d61 7069  .com/swagger-api
 00000080: 2f73 7761 6767 6572 2d63 6f64 6567 656e  /swagger-codegen
 00000090: 2920 2023 206e 6f71 613a 2045 3530 310a  )  # noqa: E501.
 000000a0: 0a20 2020 204f 7065 6e41 5049 2073 7065  .    OpenAPI spe
 000000b0: 6320 7665 7273 696f 6e3a 2036 342e 322e  c version: 64.2.
-000000c0: 302d 7632 3032 3430 3430 3432 3032 320a  0-v202404042022.
+000000c0: 312d 7632 3032 3430 3431 3730 3332 370a  1-v202404170327.
 000000d0: 2020 2020 0a20 2020 2047 656e 6572 6174      .    Generat
 000000e0: 6564 2062 793a 2068 7474 7073 3a2f 2f67  ed by: https://g
 000000f0: 6974 6875 622e 636f 6d2f 7377 6167 6765  ithub.com/swagge
 00000100: 722d 6170 692f 7377 6167 6765 722d 636f  r-api/swagger-co
 00000110: 6465 6765 6e2e 6769 740a 2222 220a 0a66  degen.git."""..f
 00000120: 726f 6d20 5f5f 6675 7475 7265 5f5f 2069  rom __future__ i
 00000130: 6d70 6f72 7420 6162 736f 6c75 7465 5f69  mport absolute_i
```

### Comparing `seeq-64.2.0/seeq/sdk/api/graph_ql_api.py` & `seeq-64.2.1/seeq/sdk/api/graph_ql_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/items_api.py` & `seeq-64.2.1/seeq/sdk/api/items_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/jobs_api.py` & `seeq-64.2.1/seeq/sdk/api/jobs_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/logs_api.py` & `seeq-64.2.1/seeq/sdk/api/logs_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/metrics_api.py` & `seeq-64.2.1/seeq/sdk/api/metrics_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/monitors_api.py` & `seeq-64.2.1/seeq/sdk/api/monitors_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/networks_api.py` & `seeq-64.2.1/seeq/sdk/api/networks_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/notification_configurations_api.py` & `seeq-64.2.1/seeq/sdk/api/notification_configurations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/notifier_api.py` & `seeq-64.2.1/seeq/sdk/api/notifier_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/plugins_api.py` & `seeq-64.2.1/seeq/sdk/api/plugins_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/projects_api.py` & `seeq-64.2.1/seeq/sdk/api/projects_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/report_templates_api.py` & `seeq-64.2.1/seeq/sdk/api/report_templates_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/reports_api.py` & `seeq-64.2.1/seeq/sdk/api/reports_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/requests_api.py` & `seeq-64.2.1/seeq/sdk/api/requests_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/scalars_api.py` & `seeq-64.2.1/seeq/sdk/api/scalars_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/scim_api.py` & `seeq-64.2.1/seeq/sdk/api/scim_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/signals_api.py` & `seeq-64.2.1/seeq/sdk/api/signals_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/subscriptions_api.py` & `seeq-64.2.1/seeq/sdk/api/subscriptions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/system_api.py` & `seeq-64.2.1/seeq/sdk/api/system_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/table_definitions_api.py` & `seeq-64.2.1/seeq/sdk/api/table_definitions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/trees_api.py` & `seeq-64.2.1/seeq/sdk/api/trees_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/unstable_api.py` & `seeq-64.2.1/seeq/sdk/api/unstable_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/usage_api.py` & `seeq-64.2.1/seeq/sdk/api/usage_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/user_groups_api.py` & `seeq-64.2.1/seeq/sdk/api/user_groups_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/users_api.py` & `seeq-64.2.1/seeq/sdk/api/users_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api/workbooks_api.py` & `seeq-64.2.1/seeq/sdk/api/workbooks_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import sys
```

### Comparing `seeq-64.2.0/seeq/sdk/api_client.py` & `seeq-64.2.1/seeq/sdk/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 from __future__ import absolute_import
 
 import json
 import mimetypes
@@ -73,15 +73,15 @@
             self.default_headers[header_name] = header_value
         if host is None:
             self.host = self.configuration.host
         else:
             self.host = host
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/64.2.0/python'
+        self.user_agent = 'Swagger-Codegen/64.2.1/python'
         self.auth_token = None
         self.identity_path = None
         self.csrf_token = None
 
     @property
     def user_agent(self):
         """
```

### Comparing `seeq-64.2.0/seeq/sdk/configuration.py` & `seeq-64.2.1/seeq/sdk/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import urllib3
@@ -254,16 +254,16 @@
         Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 64.2.0-v202404042022\n"\
-               "SDK Package Version: 64.2.0".\
+               "Version of the API: 64.2.1-v202404170327\n"\
+               "SDK Package Version: 64.2.1".\
                format(env=sys.platform, pyversion=sys.version)
 
 
 default_configuration = ClientConfiguration()
 
 
 def Configuration():
```

### Comparing `seeq-64.2.0/seeq/sdk/models/__init__.py` & `seeq-64.2.1/seeq/sdk/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
-__version__ = "64.2.0"
+__version__ = "64.2.1"
 
 # import models into sdk package
 from .access_key_input_v1 import AccessKeyInputV1
 from .access_key_output_list_v1 import AccessKeyOutputListV1
 from .access_key_output_v1 import AccessKeyOutputV1
 from .ace_input_v1 import AceInputV1
 from .ace_output_v1 import AceOutputV1
```

### Comparing `seeq-64.2.0/seeq/sdk/models/access_key_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/access_key_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/access_key_output_list_v1.py` & `seeq-64.2.1/seeq/sdk/models/access_key_output_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/access_key_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/access_key_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/ace_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/ace_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/ace_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/ace_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/acl_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/acl_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/acl_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/acl_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/activity_graph_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/activity_graph_output_v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/activity_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/activity_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/add_on_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/add_on_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/add_on_output_list_v1.py` & `seeq-64.2.1/seeq/sdk/models/add_on_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/add_on_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/add_on_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/add_on_preview_output_list_v1.py` & `seeq-64.2.1/seeq/sdk/models/add_on_preview_output_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/add_on_preview_v1.py` & `seeq-64.2.1/seeq/sdk/models/add_on_preview_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/add_on_tool_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/add_on_tool_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/add_on_tool_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/add_on_tool_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/administrator_contact_information_v1.py` & `seeq-64.2.1/seeq/sdk/models/administrator_contact_information_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/agent_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/agent_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/agent_key_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/agent_key_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/agent_orchestrator_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/agent_orchestrator_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/agent_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/agent_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/agent_status_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/agent_status_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/agent_status_v1.py` & `seeq-64.2.1/seeq/sdk/models/agent_status_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/annotation_image_link_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/annotation_image_link_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/annotation_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/annotation_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/annotation_interest_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/annotation_interest_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/annotation_interest_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/annotation_interest_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/annotation_list_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/annotation_list_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/annotation_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/annotation_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/archive_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/archive_output_v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/asset_batch_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/asset_batch_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/asset_error.py` & `seeq-64.2.1/seeq/sdk/models/asset_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/asset_group_asset_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/asset_group_asset_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/asset_group_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/asset_group_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/asset_group_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/asset_group_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/asset_group_root_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/asset_group_root_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/asset_group_tree_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/asset_group_tree_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/asset_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/asset_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/asset_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/asset_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/asset_selection_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/asset_selection_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/asset_selection_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/asset_selection_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/asset_tree_batch_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/asset_tree_batch_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/asset_tree_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/asset_tree_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/asset_tree_single_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/asset_tree_single_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/assistant_status_v1.py` & `seeq-64.2.1/seeq/sdk/models/assistant_status_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/attachment_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/attachment_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/audit_output_list_v1.py` & `seeq-64.2.1/seeq/sdk/models/audit_output_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/audit_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/audit_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/auth_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/auth_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/auth_providers_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/auth_providers_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/authoritative_region_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/authoritative_region_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/boolean_configuration_field_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/boolean_configuration_field_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/cache_block.py` & `seeq-64.2.1/seeq/sdk/models/cache_block.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/cache_info_v1.py` & `seeq-64.2.1/seeq/sdk/models/cache_info_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/calculated_item_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/calculated_item_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/capsule_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/capsule_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/capsule_property_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/capsule_property_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/capsule_property_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/capsule_property_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/capsule_v1.py` & `seeq-64.2.1/seeq/sdk/models/capsule_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/capsules_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/capsules_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/capsules_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/capsules_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/capsules_overwrite_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/capsules_overwrite_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/channel_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/channel_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/column_definition_input_list_v1.py` & `seeq-64.2.1/seeq/sdk/models/column_definition_input_list_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/column_definition_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/column_definition_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/column_definition_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/column_definition_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/column_rule_ancestor_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/column_rule_ancestor_input_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/column_rule_concat_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/column_rule_concat_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/column_rule_event_property_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/column_rule_event_property_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/column_rule_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/column_rule_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/column_rule_item_property_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/column_rule_item_property_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/column_rule_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/column_rule_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/column_rule_path_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/column_rule_path_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/condition_batch_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/condition_batch_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/condition_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/condition_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/condition_monitor_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/condition_monitor_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/condition_monitor_notification_configuration_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/condition_monitor_notification_configuration_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/condition_monitor_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/condition_monitor_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/condition_notification_output_list_v1.py` & `seeq-64.2.1/seeq/sdk/models/condition_notification_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/condition_notification_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/condition_notification_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/condition_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/condition_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/condition_update_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/condition_update_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/configuration_field_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/configuration_field_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/configuration_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/configuration_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/configuration_option_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/configuration_option_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/configuration_option_output_simple_v1.py` & `seeq-64.2.1/seeq/sdk/models/configuration_option_output_simple_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/configuration_option_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/configuration_option_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/configuration_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/configuration_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/configured_directives_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/configured_directives_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/connection_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/connection_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/connection_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/connection_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/connection_status_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/connection_status_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/connection_status_v1.py` & `seeq-64.2.1/seeq/sdk/models/connection_status_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/connections_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/connections_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/connector_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/connector_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/connector_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/connector_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/connectors_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/connectors_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/content_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/content_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/content_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/content_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/content_with_metadata_list_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/content_with_metadata_list_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/content_with_metadata_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/content_with_metadata_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/context_comment_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/context_comment_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/context_comment_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/context_comment_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/context_label_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/context_label_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/context_label_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/context_label_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/context_opaque_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/context_opaque_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/context_opaque_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/context_opaque_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/csv_datafile_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/csv_datafile_output_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/datafile_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/datafile_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/datafile_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/datafile_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/datafiles_csv_body.py` & `seeq-64.2.1/seeq/sdk/models/datafiles_csv_body.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/datasource_clean_up_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/datasource_clean_up_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/datasource_clean_up_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/datasource_clean_up_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/datasource_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/datasource_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/datasource_output_list_v1.py` & `seeq-64.2.1/seeq/sdk/models/datasource_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/datasource_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/datasource_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/datasource_preview_v1.py` & `seeq-64.2.1/seeq/sdk/models/datasource_preview_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/datasource_statistics_v1.py` & `seeq-64.2.1/seeq/sdk/models/datasource_statistics_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/datasource_status_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/datasource_status_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/datasource_status_v1.py` & `seeq-64.2.1/seeq/sdk/models/datasource_status_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/datasource_summary_status_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/datasource_summary_status_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/datasources_status_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/datasources_status_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/date_range_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/date_range_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/date_range_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/date_range_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/debug_cache_block_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/debug_cache_block_output_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/detailed_meter_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/detailed_meter_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/detailed_timer_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/detailed_timer_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/directive_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/directive_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/display_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/display_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/display_output_list_v1.py` & `seeq-64.2.1/seeq/sdk/models/display_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/display_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/display_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/display_template_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/display_template_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/display_template_output_list_v1.py` & `seeq-64.2.1/seeq/sdk/models/display_template_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/display_template_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/display_template_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/document_backup_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/document_backup_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/double_configuration_field_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/double_configuration_field_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/email_notification_recipient_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/email_notification_recipient_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/emailer_configuration_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/emailer_configuration_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/export_item_v1.py` & `seeq-64.2.1/seeq/sdk/models/export_item_v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/export_items_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/export_items_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/export_items_v1.py` & `seeq-64.2.1/seeq/sdk/models/export_items_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/export_preview_list_v1.py` & `seeq-64.2.1/seeq/sdk/models/export_preview_list_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/export_preview_v1.py` & `seeq-64.2.1/seeq/sdk/models/export_preview_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/folded_stack_node_v1.py` & `seeq-64.2.1/seeq/sdk/models/folded_stack_node_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/folder_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/folder_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/folder_navigation_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/folder_navigation_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/folder_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/folder_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/formula_compile_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/formula_update_input_v1.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
 
 
-class FormulaCompileInputV1(object):
+class FormulaUpdateInputV1(object):
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     """
 
 
     """
@@ -37,64 +37,66 @@
     attribute_map = {
         'formula': 'formula',
         'parameters': 'parameters'
     }
 
     def __init__(self, formula=None, parameters=None):
         """
-        FormulaCompileInputV1 - a model defined in Swagger
+        FormulaUpdateInputV1 - a model defined in Swagger
         """
 
         self._formula = None
         self._parameters = None
 
         if formula is not None:
           self.formula = formula
         if parameters is not None:
           self.parameters = parameters
 
     @property
     def formula(self):
         """
-        Gets the formula of this FormulaCompileInputV1.
-        A formula to compile
+        Gets the formula of this FormulaUpdateInputV1.
+        The formula to be applied
 
-        :return: The formula of this FormulaCompileInputV1.
+        :return: The formula of this FormulaUpdateInputV1.
         :rtype: str
         """
         return self._formula
 
     @formula.setter
     def formula(self, formula):
         """
-        Sets the formula of this FormulaCompileInputV1.
-        A formula to compile
+        Sets the formula of this FormulaUpdateInputV1.
+        The formula to be applied
 
-        :param formula: The formula of this FormulaCompileInputV1.
+        :param formula: The formula of this FormulaUpdateInputV1.
         :type: str
         """
+        if formula is None:
+            raise ValueError("Invalid value for `formula`, must not be `None`")
 
         self._formula = formula
 
     @property
     def parameters(self):
         """
-        Gets the parameters of this FormulaCompileInputV1.
+        Gets the parameters of this FormulaUpdateInputV1.
 
-        :return: The parameters of this FormulaCompileInputV1.
+        :return: The parameters of this FormulaUpdateInputV1.
         :rtype: list[str]
         """
         return self._parameters
 
     @parameters.setter
     def parameters(self, parameters):
         """
-        Sets the parameters of this FormulaCompileInputV1.
+        Sets the parameters of this FormulaUpdateInputV1.
 
-        :param parameters: The parameters of this FormulaCompileInputV1.
+        :param parameters: The parameters of this FormulaUpdateInputV1.
         :type: list[str]
         """
         if parameters is None:
             raise ValueError("Invalid value for `parameters`, must not be `None`")
 
         self._parameters = parameters
 
@@ -136,15 +138,15 @@
         """
         return self.to_str()
 
     def __eq__(self, other):
         """
         Returns true if both objects are equal
         """
-        if not isinstance(other, FormulaCompileInputV1):
+        if not isinstance(other, FormulaUpdateInputV1):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """
         Returns true if both objects are not equal
```

### Comparing `seeq-64.2.0/seeq/sdk/models/formula_compile_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/formula_compile_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/formula_compiler_error_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/formula_compiler_error_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/formula_dependency_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/formula_dependency_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/formula_doc_example_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/formula_doc_example_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/formula_doc_example_list_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/formula_doc_example_list_input_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/formula_doc_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/formula_doc_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/formula_doc_keyword_list_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/formula_doc_keyword_list_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/formula_doc_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/formula_doc_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/formula_doc_summaries_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/formula_doc_summaries_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/formula_doc_summary_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/formula_doc_summary_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/formula_error_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/formula_error_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/formula_example_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/formula_example_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/formula_item_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/formula_item_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/formula_item_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/formula_item_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/formula_log_entry.py` & `seeq-64.2.1/seeq/sdk/models/formula_log_entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/formula_log_entry_details.py` & `seeq-64.2.1/seeq/sdk/models/formula_log_entry_details.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/formula_log_v1.py` & `seeq-64.2.1/seeq/sdk/models/formula_log_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/formula_package_import_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/formula_package_import_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/formula_package_import_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/formula_package_import_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/formula_package_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/formula_package_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/formula_package_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/formula_package_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/formula_parameter_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/formula_parameter_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/formula_parameter_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/formula_parameter_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/formula_run_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/formula_run_input_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
@@ -143,26 +143,26 @@
 
         self._end = end
 
     @property
     def formula(self):
         """
         Gets the formula of this FormulaRunInputV1.
-        The formula to be applied
+        The formula to be applied. Length must not exceed 1M characters.
 
         :return: The formula of this FormulaRunInputV1.
         :rtype: str
         """
         return self._formula
 
     @formula.setter
     def formula(self, formula):
         """
         Sets the formula of this FormulaRunInputV1.
-        The formula to be applied
+        The formula to be applied. Length must not exceed 1M characters.
 
         :param formula: The formula of this FormulaRunInputV1.
         :type: str
         """
         if formula is None:
             raise ValueError("Invalid value for `formula`, must not be `None`")
```

### Comparing `seeq-64.2.0/seeq/sdk/models/formula_run_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/formula_run_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/formula_token.py` & `seeq-64.2.1/seeq/sdk/models/formula_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/formula_update_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/formula_compile_input_v1.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
 
 
-class FormulaUpdateInputV1(object):
+class FormulaCompileInputV1(object):
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     """
 
 
     """
@@ -37,66 +37,64 @@
     attribute_map = {
         'formula': 'formula',
         'parameters': 'parameters'
     }
 
     def __init__(self, formula=None, parameters=None):
         """
-        FormulaUpdateInputV1 - a model defined in Swagger
+        FormulaCompileInputV1 - a model defined in Swagger
         """
 
         self._formula = None
         self._parameters = None
 
         if formula is not None:
           self.formula = formula
         if parameters is not None:
           self.parameters = parameters
 
     @property
     def formula(self):
         """
-        Gets the formula of this FormulaUpdateInputV1.
-        The formula to be applied
+        Gets the formula of this FormulaCompileInputV1.
+        A formula to compile. Length must not exceed 1M characters.
 
-        :return: The formula of this FormulaUpdateInputV1.
+        :return: The formula of this FormulaCompileInputV1.
         :rtype: str
         """
         return self._formula
 
     @formula.setter
     def formula(self, formula):
         """
-        Sets the formula of this FormulaUpdateInputV1.
-        The formula to be applied
+        Sets the formula of this FormulaCompileInputV1.
+        A formula to compile. Length must not exceed 1M characters.
 
-        :param formula: The formula of this FormulaUpdateInputV1.
+        :param formula: The formula of this FormulaCompileInputV1.
         :type: str
         """
-        if formula is None:
-            raise ValueError("Invalid value for `formula`, must not be `None`")
 
         self._formula = formula
 
     @property
     def parameters(self):
         """
-        Gets the parameters of this FormulaUpdateInputV1.
+        Gets the parameters of this FormulaCompileInputV1.
 
-        :return: The parameters of this FormulaUpdateInputV1.
+        :return: The parameters of this FormulaCompileInputV1.
         :rtype: list[str]
         """
         return self._parameters
 
     @parameters.setter
     def parameters(self, parameters):
         """
-        Sets the parameters of this FormulaUpdateInputV1.
+        Sets the parameters of this FormulaCompileInputV1.
 
-        :param parameters: The parameters of this FormulaUpdateInputV1.
+        :param parameters: The parameters of this FormulaCompileInputV1.
         :type: list[str]
         """
         if parameters is None:
             raise ValueError("Invalid value for `parameters`, must not be `None`")
 
         self._parameters = parameters
 
@@ -138,15 +136,15 @@
         """
         return self.to_str()
 
     def __eq__(self, other):
         """
         Returns true if both objects are equal
         """
-        if not isinstance(other, FormulaUpdateInputV1):
+        if not isinstance(other, FormulaCompileInputV1):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """
         Returns true if both objects are not equal
```

### Comparing `seeq-64.2.0/seeq/sdk/models/formula_upgrade_change_v1.py` & `seeq-64.2.1/seeq/sdk/models/formula_upgrade_change_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/formula_upgrade_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/formula_upgrade_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/function_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/function_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/function_parameter_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/function_parameter_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/function_variant_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/function_variant_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/gauge_datum_v1.py` & `seeq-64.2.1/seeq/sdk/models/gauge_datum_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/generic_table_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/generic_table_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/get_add_on_tools_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/get_add_on_tools_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/get_channels_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/get_channels_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/get_condition_monitor_items_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/get_condition_monitor_items_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/get_content_items_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/get_content_items_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/get_date_ranges_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/get_date_ranges_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/get_jobs_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/get_jobs_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/get_metrics_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/get_metrics_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/get_projects_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/get_projects_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/get_request_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/get_request_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/get_requests_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/get_requests_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/get_sample_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/get_sample_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/get_samples_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/get_samples_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/get_signals_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/get_signals_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/graph_ql_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/graph_ql_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/graph_ql_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/graph_ql_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/id_images_body.py` & `seeq-64.2.1/seeq/sdk/models/id_images_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/identity_mapping_list_v1.py` & `seeq-64.2.1/seeq/sdk/models/identity_mapping_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/identity_mapping_v1.py` & `seeq-64.2.1/seeq/sdk/models/identity_mapping_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/identity_preview_list_v1.py` & `seeq-64.2.1/seeq/sdk/models/identity_preview_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/identity_preview_v1.py` & `seeq-64.2.1/seeq/sdk/models/identity_preview_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/indexing_parameters_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/indexing_parameters_input_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/installer_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/installer_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/interval_v1.py` & `seeq-64.2.1/seeq/sdk/models/interval_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/invalid_swap_out_v1.py` & `seeq-64.2.1/seeq/sdk/models/invalid_swap_out_v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/item_batch_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/item_batch_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/item_dependency_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/item_dependency_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/item_finder_configuration_v1.py` & `seeq-64.2.1/seeq/sdk/models/item_finder_configuration_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/item_finder_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/item_finder_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/item_finder_output_list_v1.py` & `seeq-64.2.1/seeq/sdk/models/item_finder_output_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/item_finder_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/item_finder_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/item_id_list_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/item_id_list_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/item_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/item_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/item_parameter_of_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/item_parameter_of_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/item_preview_list_v1.py` & `seeq-64.2.1/seeq/sdk/models/item_preview_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/item_preview_v1.py` & `seeq-64.2.1/seeq/sdk/models/item_preview_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/item_preview_with_assets_v1.py` & `seeq-64.2.1/seeq/sdk/models/item_preview_with_assets_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/item_search_preview_list_v1.py` & `seeq-64.2.1/seeq/sdk/models/item_search_preview_list_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/item_search_preview_paginated_list_v1.py` & `seeq-64.2.1/seeq/sdk/models/item_search_preview_paginated_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/item_search_preview_v1.py` & `seeq-64.2.1/seeq/sdk/models/item_search_preview_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/item_swap_result_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/item_swap_result_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/item_update_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/item_update_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/item_user_attributes_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/item_user_attributes_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/item_user_attributes_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/item_user_attributes_output_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/item_with_swap_pairs_v1.py` & `seeq-64.2.1/seeq/sdk/models/item_with_swap_pairs_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/jira_attachment.py` & `seeq-64.2.1/seeq/sdk/models/jira_attachment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/jira_attachment_media_type.py` & `seeq-64.2.1/seeq/sdk/models/jira_attachment_media_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/job_accepted_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/job_accepted_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/job_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/job_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/json_backup_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/json_backup_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/label_category_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/label_category_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/label_category_output_list_v1.py` & `seeq-64.2.1/seeq/sdk/models/label_category_output_list_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/label_category_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/label_category_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/label_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/label_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/label_output_list_v1.py` & `seeq-64.2.1/seeq/sdk/models/label_output_list_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/label_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/label_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/license_importer_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/license_importer_output_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/license_status_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/license_status_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/licensed_feature_status_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/licensed_feature_status_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/log_message.py` & `seeq-64.2.1/seeq/sdk/models/log_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/long_configuration_field_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/long_configuration_field_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/meter_datum_v1.py` & `seeq-64.2.1/seeq/sdk/models/meter_datum_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/migrate_editor_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/migrate_editor_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/monitor_definition_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/monitor_definition_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/monitor_definitions_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/monitor_definitions_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/monitor_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/monitor_input_v1.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/monitor_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/monitor_output_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/monitor_values.py` & `seeq-64.2.1/seeq/sdk/models/monitor_values.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/monitors_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/monitors_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/notifiable_report_output_list_v1.py` & `seeq-64.2.1/seeq/sdk/models/notifiable_report_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/notifiable_report_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/notifiable_report_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/notification_configuration_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/notification_configuration_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/optional_report_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/optional_report_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/parameter_doc_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/parameter_doc_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/permissions_v1.py` & `seeq-64.2.1/seeq/sdk/models/permissions_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/plugin_output_list_v1.py` & `seeq-64.2.1/seeq/sdk/models/plugin_output_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/plugin_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/plugin_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/plugins_body.py` & `seeq-64.2.1/seeq/sdk/models/plugins_body.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/pre_provision_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/pre_provision_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/pre_provision_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/pre_provision_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/priority_v1.py` & `seeq-64.2.1/seeq/sdk/models/priority_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/progress_information_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/progress_information_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/project_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/project_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/project_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/project_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/property_href_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/property_href_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/property_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/property_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/property_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/property_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/provision_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/provision_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/put_asset_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/put_asset_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/put_scalar_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/put_scalar_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/put_scalars_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/put_scalars_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/put_signals_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/put_signals_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/put_user_groups_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/put_user_groups_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/referenced_items_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/referenced_items_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/regression_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/regression_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/remote_agent_directives_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/remote_agent_directives_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/remote_agent_status_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/remote_agent_status_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/remote_agent_status_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/remote_agent_status_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/report_input_item_v1.py` & `seeq-64.2.1/seeq/sdk/models/report_input_item_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/report_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/report_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/report_notification_configuration_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/report_notification_configuration_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/report_template_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/report_template_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/report_template_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/report_template_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/request_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/request_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/sample_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/sample_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/sample_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/sample_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/samples_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/samples_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/samples_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/samples_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/samples_overwrite_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/samples_overwrite_input_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/scalar_evaluate_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/scalar_evaluate_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/scalar_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/scalar_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/scalar_property_v1.py` & `seeq-64.2.1/seeq/sdk/models/scalar_property_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/scalar_value_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/scalar_value_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/scale_across_tree_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/scale_across_tree_output_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/schedulable_admin_list_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/schedulable_admin_list_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/schedulable_admin_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/schedulable_admin_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/schedulable_summary_day_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/schedulable_summary_day_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/schedulable_summary_week_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/schedulable_summary_week_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/schedule_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/schedule_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/schedule_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/schedule_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/scheduled_notebook_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/scheduled_notebook_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/scheduled_notebook_list_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/scheduled_notebook_list_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/scheduled_notebook_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/scheduled_notebook_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/scim_token_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/scim_token_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/screenshot_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/screenshot_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/secret_configuration_field_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/secret_configuration_field_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/see_also_doc_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/see_also_doc_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/send_email_attachment_v1.py` & `seeq-64.2.1/seeq/sdk/models/send_email_attachment_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/send_email_contact_v1.py` & `seeq-64.2.1/seeq/sdk/models/send_email_contact_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/send_email_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/send_email_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/sent_email_attachment_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/sent_email_attachment_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/sent_email_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/sent_email_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/sent_emails_list_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/sent_emails_list_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/server_build_info_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/server_build_info_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/server_load_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/server_load_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/server_spec_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/server_spec_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/server_status_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/server_status_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/signal_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/signal_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/signal_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/signal_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/signal_with_id_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/signal_with_id_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/status_message.py` & `seeq-64.2.1/seeq/sdk/models/status_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/status_message_base.py` & `seeq-64.2.1/seeq/sdk/models/status_message_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/store_secret_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/store_secret_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/string_configuration_field_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/string_configuration_field_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/subscription_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/subscription_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/subscription_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/subscription_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/subscription_update_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/subscription_update_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/support_request_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/support_request_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/support_request_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/support_request_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/supported_units_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/supported_units_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/swap_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/swap_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/swap_option_list_v1.py` & `seeq-64.2.1/seeq/sdk/models/swap_option_list_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/swap_option_v1.py` & `seeq-64.2.1/seeq/sdk/models/swap_option_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/swap_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/swap_output_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/sync_progress.py` & `seeq-64.2.1/seeq/sdk/models/sync_progress.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/sync_progress_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/sync_progress_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/system_license_body.py` & `seeq-64.2.1/seeq/sdk/models/system_license_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/table_column_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/table_column_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/table_definition_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/table_definition_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/table_definition_output_list_v1.py` & `seeq-64.2.1/seeq/sdk/models/table_definition_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/table_definition_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/table_definition_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/table_definition_update_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/table_definition_update_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/threshold_metric_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/threshold_metric_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/threshold_metric_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/threshold_metric_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/threshold_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/threshold_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/timer_datum_v1.py` & `seeq-64.2.1/seeq/sdk/models/timer_datum_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/tree_item_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/tree_item_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/treemap_item_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/treemap_item_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/treemap_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/treemap_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/units_of_measure_batch_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/units_of_measure_batch_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/units_of_measure_item_v1.py` & `seeq-64.2.1/seeq/sdk/models/units_of_measure_item_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/units_of_measure_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/units_of_measure_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/unsubscribe_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/unsubscribe_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/usage_output_list_v1.py` & `seeq-64.2.1/seeq/sdk/models/usage_output_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/usage_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/usage_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/usage_types_v1.py` & `seeq-64.2.1/seeq/sdk/models/usage_types_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/user_group_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/user_group_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/user_group_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/user_group_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/user_group_with_id_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/user_group_with_id_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/user_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/user_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/user_output_list_v1.py` & `seeq-64.2.1/seeq/sdk/models/user_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/user_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/user_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/user_password_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/user_password_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/validate_cron_list_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/validate_cron_list_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/validate_cron_list_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/validate_cron_list_output_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/validate_cron_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/validate_cron_output_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/workbench_item_output_list_v1.py` & `seeq-64.2.1/seeq/sdk/models/workbench_item_output_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/workbench_search_result_preview_v1.py` & `seeq-64.2.1/seeq/sdk/models/workbench_search_result_preview_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/workbook_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/workbook_input_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/workbook_output_list_v1.py` & `seeq-64.2.1/seeq/sdk/models/workbook_output_list_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/workbook_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/workbook_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/worksheet_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/worksheet_input_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/worksheet_output_list_v1.py` & `seeq-64.2.1/seeq/sdk/models/worksheet_output_list_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/worksheet_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/worksheet_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/workstep_input_v1.py` & `seeq-64.2.1/seeq/sdk/models/workstep_input_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/models/workstep_output_v1.py` & `seeq-64.2.1/seeq/sdk/models/workstep_output_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from pprint import pformat
 from six import iteritems
 import re
```

### Comparing `seeq-64.2.0/seeq/sdk/rest.py` & `seeq-64.2.1/seeq/sdk/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Seeq REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
-    OpenAPI spec version: 64.2.0-v202404042022
+    OpenAPI spec version: 64.2.1-v202404170327
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import io
```

### Comparing `seeq-64.2.0/seeq.egg-info/PKG-INFO` & `seeq-64.2.1/seeq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeq
-Version: 64.2.0
+Version: 64.2.1
 Summary: The Seeq SDK for Python
 Home-page: https://www.seeq.com
 Author: Seeq Corporation
 Author-email: support@seeq.com
 Project-URL: Documentation, https://python-docs.seeq.com/
 Project-URL: Changelog, https://python-docs.seeq.com/changelog.html
 Classifier: Programming Language :: Python :: 2
```

### Comparing `seeq-64.2.0/seeq.egg-info/SOURCES.txt` & `seeq-64.2.1/seeq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seeq-64.2.0/setup.py` & `seeq-64.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="seeq",
-    version="64.2.0",
+    version="64.2.1",
     author="Seeq Corporation",
     author_email="support@seeq.com",
     description="The Seeq SDK for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.seeq.com",
     project_urls={
```

