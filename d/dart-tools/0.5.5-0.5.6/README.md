# Comparing `tmp/dart-tools-0.5.5.tar.gz` & `tmp/dart_tools-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dart-tools-0.5.5.tar", last modified: Fri Mar 15 07:28:51 2024, max compression
+gzip compressed data, was "dart_tools-0.5.6.tar", last modified: Tue Apr 16 22:06:41 2024, max compression
```

## Comparing `dart-tools-0.5.5.tar` & `dart_tools-0.5.6.tar`

### file list

```diff
@@ -1,193 +1,194 @@
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-03-15 07:28:51.994594 dart-tools-0.5.5/
--rw-r--r--   0 zack       (501) staff       (20)     1061 2023-02-28 02:56:19.000000 dart-tools-0.5.5/LICENSE
--rw-r--r--   0 zack       (501) staff       (20)     7166 2024-03-15 07:28:51.994345 dart-tools-0.5.5/PKG-INFO
--rw-r--r--   0 zack       (501) staff       (20)     4220 2024-03-15 07:27:40.000000 dart-tools-0.5.5/README.md
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-03-15 07:28:51.956783 dart-tools-0.5.5/dart/
--rw-r--r--   0 zack       (501) staff       (20)      229 2023-12-01 08:32:06.000000 dart-tools-0.5.5/dart/__init__.py
--rwxr-xr-x   0 zack       (501) staff       (20)    28447 2024-03-01 23:48:16.000000 dart-tools-0.5.5/dart/dart.py
--rw-r--r--   0 zack       (501) staff       (20)       85 2023-12-01 08:32:06.000000 dart-tools-0.5.5/dart/exception.py
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-03-15 07:28:51.958446 dart-tools-0.5.5/dart/generated/
--rw-r--r--   0 zack       (501) staff       (20)      152 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/__init__.py
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-03-15 07:28:51.958923 dart-tools-0.5.5/dart/generated/api/
--rw-r--r--   0 zack       (501) staff       (20)       47 2024-03-15 07:28:17.000000 dart-tools-0.5.5/dart/generated/api/__init__.py
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-03-15 07:28:51.959303 dart-tools-0.5.5/dart/generated/api/transactions/
--rw-r--r--   0 zack       (501) staff       (20)        0 2024-03-15 07:28:17.000000 dart-tools-0.5.5/dart/generated/api/transactions/__init__.py
--rw-r--r--   0 zack       (501) staff       (20)     4663 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/api/transactions/transactions_create.py
--rw-r--r--   0 zack       (501) staff       (20)    12131 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/client.py
--rw-r--r--   0 zack       (501) staff       (20)      470 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/errors.py
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-03-15 07:28:51.992508 dart-tools-0.5.5/dart/generated/models/
--rw-r--r--   0 zack       (501) staff       (20)    11026 2024-03-15 07:28:17.000000 dart-tools-0.5.5/dart/generated/models/__init__.py
--rw-r--r--   0 zack       (501) staff       (20)     3474 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/attachment.py
--rw-r--r--   0 zack       (501) staff       (20)     3945 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/attachment_create.py
--rw-r--r--   0 zack       (501) staff       (20)     4270 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/attachment_update.py
--rw-r--r--   0 zack       (501) staff       (20)      704 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/batch.py
--rw-r--r--   0 zack       (501) staff       (20)     3879 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/brainstorm.py
--rw-r--r--   0 zack       (501) staff       (20)     3889 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/brainstorm_create.py
--rw-r--r--   0 zack       (501) staff       (20)      190 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/brainstorm_state.py
--rw-r--r--   0 zack       (501) staff       (20)     4833 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/brainstorm_update.py
--rw-r--r--   0 zack       (501) staff       (20)      742 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/color_name.py
--rw-r--r--   0 zack       (501) staff       (20)     4984 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/comment.py
--rw-r--r--   0 zack       (501) staff       (20)     3538 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/comment_create.py
--rw-r--r--   0 zack       (501) staff       (20)     2103 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/comment_reaction.py
--rw-r--r--   0 zack       (501) staff       (20)     2052 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/comment_reaction_create.py
--rw-r--r--   0 zack       (501) staff       (20)     2352 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/comment_reaction_update.py
--rw-r--r--   0 zack       (501) staff       (20)     3712 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/comment_update.py
--rw-r--r--   0 zack       (501) staff       (20)     7027 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/dartboard.py
--rw-r--r--   0 zack       (501) staff       (20)     7410 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/dartboard_create.py
--rw-r--r--   0 zack       (501) staff       (20)      244 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/dartboard_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     7579 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/dartboard_update.py
--rw-r--r--   0 zack       (501) staff       (20)      249 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/dartboards_list_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     1724 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/discord_integration.py
--rw-r--r--   0 zack       (501) staff       (20)     6853 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/doc.py
--rw-r--r--   0 zack       (501) staff       (20)     9159 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/doc_create.py
--rw-r--r--   0 zack       (501) staff       (20)      306 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/doc_source_type.py
--rw-r--r--   0 zack       (501) staff       (20)     9329 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/doc_update.py
--rw-r--r--   0 zack       (501) staff       (20)      421 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/entity_name.py
--rw-r--r--   0 zack       (501) staff       (20)    10339 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/event.py
--rw-r--r--   0 zack       (501) staff       (20)      549 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/event_actor.py
--rw-r--r--   0 zack       (501) staff       (20)     5770 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/event_create.py
--rw-r--r--   0 zack       (501) staff       (20)     3192 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/event_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     1775 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/event_subscription.py
--rw-r--r--   0 zack       (501) staff       (20)     6402 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/event_subscription_update.py
--rw-r--r--   0 zack       (501) staff       (20)      521 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/filter_applicability.py
--rw-r--r--   0 zack       (501) staff       (20)     3149 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/filter_assignee.py
--rw-r--r--   0 zack       (501) staff       (20)      150 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/filter_connector.py
--rw-r--r--   0 zack       (501) staff       (20)     3511 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/filter_group.py
--rw-r--r--   0 zack       (501) staff       (20)     1915 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/filter_search.py
--rw-r--r--   0 zack       (501) staff       (20)     3124 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/filter_set.py
--rw-r--r--   0 zack       (501) staff       (20)     5265 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/folder.py
--rw-r--r--   0 zack       (501) staff       (20)     6484 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/folder_create.py
--rw-r--r--   0 zack       (501) staff       (20)      183 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/folder_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     6653 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/folder_update.py
--rw-r--r--   0 zack       (501) staff       (20)      188 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/folders_list_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     4426 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/form.py
--rw-r--r--   0 zack       (501) staff       (20)     5169 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/form_create.py
--rw-r--r--   0 zack       (501) staff       (20)     3283 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/form_field.py
--rw-r--r--   0 zack       (501) staff       (20)     3306 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/form_field_create.py
--rw-r--r--   0 zack       (501) staff       (20)     3564 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/form_field_update.py
--rw-r--r--   0 zack       (501) staff       (20)     5251 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/form_update.py
--rw-r--r--   0 zack       (501) staff       (20)     4228 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/github_integration.py
--rw-r--r--   0 zack       (501) staff       (20)      245 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/github_integration_tenant_extension_status.py
--rw-r--r--   0 zack       (501) staff       (20)     2114 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/google_data.py
--rw-r--r--   0 zack       (501) staff       (20)      169 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/icon_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     4937 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/layout.py
--rw-r--r--   0 zack       (501) staff       (20)     1768 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/layout_config.py
--rw-r--r--   0 zack       (501) staff       (20)     4247 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/layout_create.py
--rw-r--r--   0 zack       (501) staff       (20)      203 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/layout_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     1751 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/layout_kind_config_map.py
--rw-r--r--   0 zack       (501) staff       (20)     4247 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/layout_update.py
--rw-r--r--   0 zack       (501) staff       (20)    24662 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/models_response.py
--rw-r--r--   0 zack       (501) staff       (20)     2825 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/notification.py
--rw-r--r--   0 zack       (501) staff       (20)     2619 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/notification_update.py
--rw-r--r--   0 zack       (501) staff       (20)     2310 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/notion_integration.py
--rw-r--r--   0 zack       (501) staff       (20)      217 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/notion_integration_tenant_extension_status.py
--rw-r--r--   0 zack       (501) staff       (20)    32625 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/operation.py
--rw-r--r--   0 zack       (501) staff       (20)      270 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/operation_kind.py
--rw-r--r--   0 zack       (501) staff       (20)      861 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/operation_model_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     3367 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/option.py
--rw-r--r--   0 zack       (501) staff       (20)     3330 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/option_create.py
--rw-r--r--   0 zack       (501) staff       (20)     3502 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/option_update.py
--rw-r--r--   0 zack       (501) staff       (20)     3104 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/paginated_attachment_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3068 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/paginated_comment_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3169 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/paginated_comment_reaction_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3092 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/paginated_dartboard_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3020 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/paginated_doc_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3056 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/paginated_folder_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3097 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/paginated_form_field_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3032 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/paginated_form_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3056 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/paginated_layout_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3056 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/paginated_option_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3082 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/paginated_property_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3181 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/paginated_relationship_kind_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3128 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/paginated_relationship_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3044 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/paginated_space_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3056 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/paginated_status_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3222 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/paginated_task_doc_relationship_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3085 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/paginated_task_link_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3032 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/paginated_task_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3056 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/paginated_tenant_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3222 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/paginated_user_dartboard_layout_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3032 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/paginated_user_list.py
--rw-r--r--   0 zack       (501) staff       (20)     3032 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/paginated_view_list.py
--rw-r--r--   0 zack       (501) staff       (20)      195 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/priority.py
--rw-r--r--   0 zack       (501) staff       (20)      913 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/properties_list_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     3915 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/property_.py
--rw-r--r--   0 zack       (501) staff       (20)     3852 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/property_create.py
--rw-r--r--   0 zack       (501) staff       (20)      907 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/property_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     4247 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/property_update.py
--rw-r--r--   0 zack       (501) staff       (20)      177 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/recommendation_status.py
--rw-r--r--   0 zack       (501) staff       (20)     1839 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/relationship.py
--rw-r--r--   0 zack       (501) staff       (20)     2392 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/relationship_create.py
--rw-r--r--   0 zack       (501) staff       (20)     3014 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/relationship_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     3013 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/relationship_kind_create.py
--rw-r--r--   0 zack       (501) staff       (20)      257 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/relationship_kind_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     3187 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/relationship_kind_update.py
--rw-r--r--   0 zack       (501) staff       (20)      167 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/report_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     2093 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/request_body.py
--rw-r--r--   0 zack       (501) staff       (20)     1989 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/response_body.py
--rw-r--r--   0 zack       (501) staff       (20)     2300 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/slack_integration.py
--rw-r--r--   0 zack       (501) staff       (20)      216 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/slack_integration_tenant_extension_status.py
--rw-r--r--   0 zack       (501) staff       (20)     1611 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/sort.py
--rw-r--r--   0 zack       (501) staff       (20)     7814 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/space.py
--rw-r--r--   0 zack       (501) staff       (20)     9821 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/space_create.py
--rw-r--r--   0 zack       (501) staff       (20)      188 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/space_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     9903 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/space_update.py
--rw-r--r--   0 zack       (501) staff       (20)      151 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/sprint_mode.py
--rw-r--r--   0 zack       (501) staff       (20)     4280 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/status.py
--rw-r--r--   0 zack       (501) staff       (20)     4497 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/status_create.py
--rw-r--r--   0 zack       (501) staff       (20)      243 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/status_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     4980 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/status_update.py
--rw-r--r--   0 zack       (501) staff       (20)      249 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/statuses_list_kind.py
--rw-r--r--   0 zack       (501) staff       (20)      167 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/subscription.py
--rw-r--r--   0 zack       (501) staff       (20)      172 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/subtask_display_mode.py
--rw-r--r--   0 zack       (501) staff       (20)      403 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/summary_statistic_kind.py
--rw-r--r--   0 zack       (501) staff       (20)    11576 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/task.py
--rw-r--r--   0 zack       (501) staff       (20)    13810 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/task_create.py
--rw-r--r--   0 zack       (501) staff       (20)     2298 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/task_doc_relationship.py
--rw-r--r--   0 zack       (501) staff       (20)     1863 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/task_doc_relationship_create.py
--rw-r--r--   0 zack       (501) staff       (20)     3093 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/task_link.py
--rw-r--r--   0 zack       (501) staff       (20)     3668 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/task_link_create.py
--rw-r--r--   0 zack       (501) staff       (20)      661 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/task_link_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     3916 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/task_link_update.py
--rw-r--r--   0 zack       (501) staff       (20)     4890 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/task_notion_document.py
--rw-r--r--   0 zack       (501) staff       (20)     1337 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/task_notion_document_block_children_map.py
--rw-r--r--   0 zack       (501) staff       (20)     1294 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/task_notion_document_block_map.py
--rw-r--r--   0 zack       (501) staff       (20)     1289 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/task_notion_document_page_map.py
--rw-r--r--   0 zack       (501) staff       (20)     1225 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/task_properties.py
--rw-r--r--   0 zack       (501) staff       (20)      811 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/task_source_type.py
--rw-r--r--   0 zack       (501) staff       (20)    14071 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/task_update.py
--rw-r--r--   0 zack       (501) staff       (20)     8226 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/tenant.py
--rw-r--r--   0 zack       (501) staff       (20)     4446 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/tenant_update.py
--rw-r--r--   0 zack       (501) staff       (20)      186 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/theme.py
--rw-r--r--   0 zack       (501) staff       (20)     5226 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/transaction.py
--rw-r--r--   0 zack       (501) staff       (20)     2426 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/transaction_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     2470 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/transaction_response.py
--rw-r--r--   0 zack       (501) staff       (20)     5894 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/user.py
--rw-r--r--   0 zack       (501) staff       (20)     1718 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/user_dartboard_layout.py
--rw-r--r--   0 zack       (501) staff       (20)     1991 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/user_dartboard_layout_create.py
--rw-r--r--   0 zack       (501) staff       (20)      767 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/user_data_entity_retrieve_entity_kind.py
--rw-r--r--   0 zack       (501) staff       (20)      175 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/user_role.py
--rw-r--r--   0 zack       (501) staff       (20)      313 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/user_status.py
--rw-r--r--   0 zack       (501) staff       (20)     6910 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/user_update.py
--rw-r--r--   0 zack       (501) staff       (20)     1804 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/validation_error_response.py
--rw-r--r--   0 zack       (501) staff       (20)     1301 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/validation_error_response_items.py
--rw-r--r--   0 zack       (501) staff       (20)     5643 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/view.py
--rw-r--r--   0 zack       (501) staff       (20)     6457 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/view_create.py
--rw-r--r--   0 zack       (501) staff       (20)      203 2024-03-15 07:28:18.000000 dart-tools-0.5.5/dart/generated/models/view_kind.py
--rw-r--r--   0 zack       (501) staff       (20)     6627 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/view_update.py
--rw-r--r--   0 zack       (501) staff       (20)     3316 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/models/yc_integration.py
--rw-r--r--   0 zack       (501) staff       (20)       25 2024-03-15 07:28:17.000000 dart-tools-0.5.5/dart/generated/py.typed
--rw-r--r--   0 zack       (501) staff       (20)      968 2024-03-15 07:28:19.000000 dart-tools-0.5.5/dart/generated/types.py
--rw-r--r--   0 zack       (501) staff       (20)     1905 2023-12-06 01:16:03.000000 dart-tools-0.5.5/dart/order_manager.py
--rw-r--r--   0 zack       (501) staff       (20)      569 2023-12-01 08:32:06.000000 dart-tools-0.5.5/dart/webhook.py
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-03-15 07:28:51.993931 dart-tools-0.5.5/dart_tools.egg-info/
--rw-r--r--   0 zack       (501) staff       (20)     7166 2024-03-15 07:28:51.000000 dart-tools-0.5.5/dart_tools.egg-info/PKG-INFO
--rw-r--r--   0 zack       (501) staff       (20)     7373 2024-03-15 07:28:51.000000 dart-tools-0.5.5/dart_tools.egg-info/SOURCES.txt
--rw-r--r--   0 zack       (501) staff       (20)        1 2024-03-15 07:28:51.000000 dart-tools-0.5.5/dart_tools.egg-info/dependency_links.txt
-drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-03-15 07:28:51.993545 dart-tools-0.5.5/dart_tools.egg-info/dist/
--rw-r--r--   0 zack       (501) staff       (20)     8788 2023-06-03 08:11:34.000000 dart-tools-0.5.5/dart_tools.egg-info/dist/dart-tools-0.3.3.tar.gz
--rw-r--r--   0 zack       (501) staff       (20)       34 2024-03-15 07:28:51.000000 dart-tools-0.5.5/dart_tools.egg-info/entry_points.txt
--rw-r--r--   0 zack       (501) staff       (20)       38 2024-03-15 07:28:51.000000 dart-tools-0.5.5/dart_tools.egg-info/requires.txt
--rw-r--r--   0 zack       (501) staff       (20)        5 2024-03-15 07:28:51.000000 dart-tools-0.5.5/dart_tools.egg-info/top_level.txt
--rw-r--r--   0 zack       (501) staff       (20)     1891 2024-03-15 07:28:29.000000 dart-tools-0.5.5/pyproject.toml
--rw-r--r--   0 zack       (501) staff       (20)       38 2024-03-15 07:28:51.994642 dart-tools-0.5.5/setup.cfg
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-04-16 22:06:41.834949 dart_tools-0.5.6/
+-rw-r--r--   0 zack       (501) staff       (20)     1061 2023-02-28 02:56:19.000000 dart_tools-0.5.6/LICENSE
+-rw-r--r--   0 zack       (501) staff       (20)     7166 2024-04-16 22:06:41.834724 dart_tools-0.5.6/PKG-INFO
+-rw-r--r--   0 zack       (501) staff       (20)     4220 2024-03-15 07:27:40.000000 dart_tools-0.5.6/README.md
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-04-16 22:06:41.788462 dart_tools-0.5.6/dart/
+-rw-r--r--   0 zack       (501) staff       (20)      229 2023-12-01 08:32:06.000000 dart_tools-0.5.6/dart/__init__.py
+-rwxr-xr-x   0 zack       (501) staff       (20)    28838 2024-04-16 22:05:57.000000 dart_tools-0.5.6/dart/dart.py
+-rw-r--r--   0 zack       (501) staff       (20)       85 2023-12-01 08:32:06.000000 dart_tools-0.5.6/dart/exception.py
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-04-16 22:06:41.790170 dart_tools-0.5.6/dart/generated/
+-rw-r--r--   0 zack       (501) staff       (20)      152 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/__init__.py
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-04-16 22:06:41.790501 dart_tools-0.5.6/dart/generated/api/
+-rw-r--r--   0 zack       (501) staff       (20)       47 2024-04-16 22:06:24.000000 dart_tools-0.5.6/dart/generated/api/__init__.py
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-04-16 22:06:41.790959 dart_tools-0.5.6/dart/generated/api/transactions/
+-rw-r--r--   0 zack       (501) staff       (20)        0 2024-04-16 22:06:24.000000 dart_tools-0.5.6/dart/generated/api/transactions/__init__.py
+-rw-r--r--   0 zack       (501) staff       (20)     4663 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/api/transactions/transactions_create.py
+-rw-r--r--   0 zack       (501) staff       (20)    12131 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/client.py
+-rw-r--r--   0 zack       (501) staff       (20)      470 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/errors.py
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-04-16 22:06:41.832417 dart_tools-0.5.6/dart/generated/models/
+-rw-r--r--   0 zack       (501) staff       (20)    11101 2024-04-16 22:06:24.000000 dart_tools-0.5.6/dart/generated/models/__init__.py
+-rw-r--r--   0 zack       (501) staff       (20)     3474 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/attachment.py
+-rw-r--r--   0 zack       (501) staff       (20)     3945 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/attachment_create.py
+-rw-r--r--   0 zack       (501) staff       (20)     4270 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/attachment_update.py
+-rw-r--r--   0 zack       (501) staff       (20)      704 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/batch.py
+-rw-r--r--   0 zack       (501) staff       (20)     3879 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/brainstorm.py
+-rw-r--r--   0 zack       (501) staff       (20)     3889 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/brainstorm_create.py
+-rw-r--r--   0 zack       (501) staff       (20)      190 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/brainstorm_state.py
+-rw-r--r--   0 zack       (501) staff       (20)     4833 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/brainstorm_update.py
+-rw-r--r--   0 zack       (501) staff       (20)      742 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/color_name.py
+-rw-r--r--   0 zack       (501) staff       (20)     4984 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/comment.py
+-rw-r--r--   0 zack       (501) staff       (20)     3538 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/comment_create.py
+-rw-r--r--   0 zack       (501) staff       (20)     2103 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/comment_reaction.py
+-rw-r--r--   0 zack       (501) staff       (20)     2052 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/comment_reaction_create.py
+-rw-r--r--   0 zack       (501) staff       (20)     2352 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/comment_reaction_update.py
+-rw-r--r--   0 zack       (501) staff       (20)     3712 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/comment_update.py
+-rw-r--r--   0 zack       (501) staff       (20)     7835 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/dartboard.py
+-rw-r--r--   0 zack       (501) staff       (20)     8711 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/dartboard_create.py
+-rw-r--r--   0 zack       (501) staff       (20)      244 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/dartboard_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     8880 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/dartboard_update.py
+-rw-r--r--   0 zack       (501) staff       (20)      249 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/dartboards_list_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     1724 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/discord_integration.py
+-rw-r--r--   0 zack       (501) staff       (20)     6853 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/doc.py
+-rw-r--r--   0 zack       (501) staff       (20)     9649 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/doc_create.py
+-rw-r--r--   0 zack       (501) staff       (20)      306 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/doc_source_type.py
+-rw-r--r--   0 zack       (501) staff       (20)     9649 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/doc_update.py
+-rw-r--r--   0 zack       (501) staff       (20)      421 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/entity_name.py
+-rw-r--r--   0 zack       (501) staff       (20)    10339 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/event.py
+-rw-r--r--   0 zack       (501) staff       (20)      549 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/event_actor.py
+-rw-r--r--   0 zack       (501) staff       (20)     5770 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/event_create.py
+-rw-r--r--   0 zack       (501) staff       (20)     3192 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/event_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     1775 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/event_subscription.py
+-rw-r--r--   0 zack       (501) staff       (20)     6402 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/event_subscription_update.py
+-rw-r--r--   0 zack       (501) staff       (20)      521 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/filter_applicability.py
+-rw-r--r--   0 zack       (501) staff       (20)     3149 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/filter_assignee.py
+-rw-r--r--   0 zack       (501) staff       (20)      150 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/filter_connector.py
+-rw-r--r--   0 zack       (501) staff       (20)     3511 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/filter_group.py
+-rw-r--r--   0 zack       (501) staff       (20)     1915 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/filter_search.py
+-rw-r--r--   0 zack       (501) staff       (20)     3124 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/filter_set.py
+-rw-r--r--   0 zack       (501) staff       (20)     5265 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/folder.py
+-rw-r--r--   0 zack       (501) staff       (20)     6484 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/folder_create.py
+-rw-r--r--   0 zack       (501) staff       (20)      183 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/folder_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     6653 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/folder_update.py
+-rw-r--r--   0 zack       (501) staff       (20)      188 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/folders_list_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     4426 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/form.py
+-rw-r--r--   0 zack       (501) staff       (20)     5169 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/form_create.py
+-rw-r--r--   0 zack       (501) staff       (20)     3283 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/form_field.py
+-rw-r--r--   0 zack       (501) staff       (20)     3306 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/form_field_create.py
+-rw-r--r--   0 zack       (501) staff       (20)     3564 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/form_field_update.py
+-rw-r--r--   0 zack       (501) staff       (20)     5251 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/form_update.py
+-rw-r--r--   0 zack       (501) staff       (20)     4228 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/github_integration.py
+-rw-r--r--   0 zack       (501) staff       (20)      245 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/github_integration_tenant_extension_status.py
+-rw-r--r--   0 zack       (501) staff       (20)     2114 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/google_data.py
+-rw-r--r--   0 zack       (501) staff       (20)      169 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/icon_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     4937 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/layout.py
+-rw-r--r--   0 zack       (501) staff       (20)     1768 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/layout_config.py
+-rw-r--r--   0 zack       (501) staff       (20)     4247 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/layout_create.py
+-rw-r--r--   0 zack       (501) staff       (20)      203 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/layout_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     1751 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/layout_kind_config_map.py
+-rw-r--r--   0 zack       (501) staff       (20)     4247 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/layout_update.py
+-rw-r--r--   0 zack       (501) staff       (20)    24662 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/models_response.py
+-rw-r--r--   0 zack       (501) staff       (20)     2825 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/notification.py
+-rw-r--r--   0 zack       (501) staff       (20)     2619 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/notification_update.py
+-rw-r--r--   0 zack       (501) staff       (20)     2310 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/notion_integration.py
+-rw-r--r--   0 zack       (501) staff       (20)      217 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/notion_integration_tenant_extension_status.py
+-rw-r--r--   0 zack       (501) staff       (20)    32625 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/operation.py
+-rw-r--r--   0 zack       (501) staff       (20)      270 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/operation_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)      861 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/operation_model_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     3367 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/option.py
+-rw-r--r--   0 zack       (501) staff       (20)     3330 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/option_create.py
+-rw-r--r--   0 zack       (501) staff       (20)     3502 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/option_update.py
+-rw-r--r--   0 zack       (501) staff       (20)     3104 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_attachment_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     3068 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_comment_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     3169 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_comment_reaction_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     3092 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_dartboard_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     3020 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_doc_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     3056 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_folder_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     3097 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_form_field_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     3032 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_form_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     3056 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_layout_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     3056 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_option_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     3082 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_property_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     3181 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_relationship_kind_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     3128 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_relationship_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     3044 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_space_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     3056 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_status_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     3222 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_task_doc_relationship_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     3085 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_task_link_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     3032 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_task_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     3056 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_tenant_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     3222 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_user_dartboard_layout_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     3032 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_user_list.py
+-rw-r--r--   0 zack       (501) staff       (20)     3032 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/paginated_view_list.py
+-rw-r--r--   0 zack       (501) staff       (20)      195 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/priority.py
+-rw-r--r--   0 zack       (501) staff       (20)      913 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/properties_list_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     3915 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/property_.py
+-rw-r--r--   0 zack       (501) staff       (20)     3852 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/property_create.py
+-rw-r--r--   0 zack       (501) staff       (20)      907 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/property_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     4247 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/property_update.py
+-rw-r--r--   0 zack       (501) staff       (20)      177 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/recommendation_status.py
+-rw-r--r--   0 zack       (501) staff       (20)     1839 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/relationship.py
+-rw-r--r--   0 zack       (501) staff       (20)     2392 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/relationship_create.py
+-rw-r--r--   0 zack       (501) staff       (20)     3014 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/relationship_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     3013 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/relationship_kind_create.py
+-rw-r--r--   0 zack       (501) staff       (20)      257 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/relationship_kind_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     3187 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/relationship_kind_update.py
+-rw-r--r--   0 zack       (501) staff       (20)      167 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/report_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     2093 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/request_body.py
+-rw-r--r--   0 zack       (501) staff       (20)     1989 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/response_body.py
+-rw-r--r--   0 zack       (501) staff       (20)     2300 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/slack_integration.py
+-rw-r--r--   0 zack       (501) staff       (20)      216 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/slack_integration_tenant_extension_status.py
+-rw-r--r--   0 zack       (501) staff       (20)     1611 2024-04-16 22:06:26.000000 dart_tools-0.5.6/dart/generated/models/sort.py
+-rw-r--r--   0 zack       (501) staff       (20)     7814 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/space.py
+-rw-r--r--   0 zack       (501) staff       (20)     9821 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/space_create.py
+-rw-r--r--   0 zack       (501) staff       (20)      188 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/space_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     9903 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/space_update.py
+-rw-r--r--   0 zack       (501) staff       (20)      151 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/sprint_mode.py
+-rw-r--r--   0 zack       (501) staff       (20)     4280 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/status.py
+-rw-r--r--   0 zack       (501) staff       (20)     4497 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/status_create.py
+-rw-r--r--   0 zack       (501) staff       (20)      243 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/status_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     4980 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/status_update.py
+-rw-r--r--   0 zack       (501) staff       (20)      249 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/statuses_list_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)      167 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/subscription.py
+-rw-r--r--   0 zack       (501) staff       (20)      172 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/subtask_display_mode.py
+-rw-r--r--   0 zack       (501) staff       (20)      403 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/summary_statistic_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)    11576 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/task.py
+-rw-r--r--   0 zack       (501) staff       (20)    14468 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/task_create.py
+-rw-r--r--   0 zack       (501) staff       (20)     2298 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/task_doc_relationship.py
+-rw-r--r--   0 zack       (501) staff       (20)     1863 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/task_doc_relationship_create.py
+-rw-r--r--   0 zack       (501) staff       (20)     3093 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/task_link.py
+-rw-r--r--   0 zack       (501) staff       (20)     3668 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/task_link_create.py
+-rw-r--r--   0 zack       (501) staff       (20)      661 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/task_link_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     3916 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/task_link_update.py
+-rw-r--r--   0 zack       (501) staff       (20)     4890 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/task_notion_document.py
+-rw-r--r--   0 zack       (501) staff       (20)     1337 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/task_notion_document_block_children_map.py
+-rw-r--r--   0 zack       (501) staff       (20)     1294 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/task_notion_document_block_map.py
+-rw-r--r--   0 zack       (501) staff       (20)     1289 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/task_notion_document_page_map.py
+-rw-r--r--   0 zack       (501) staff       (20)     1225 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/task_properties.py
+-rw-r--r--   0 zack       (501) staff       (20)      811 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/task_source_type.py
+-rw-r--r--   0 zack       (501) staff       (20)    14468 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/task_update.py
+-rw-r--r--   0 zack       (501) staff       (20)     8963 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/tenant.py
+-rw-r--r--   0 zack       (501) staff       (20)     4446 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/tenant_update.py
+-rw-r--r--   0 zack       (501) staff       (20)      186 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/theme.py
+-rw-r--r--   0 zack       (501) staff       (20)     5226 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/transaction.py
+-rw-r--r--   0 zack       (501) staff       (20)     2426 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/transaction_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     2470 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/transaction_response.py
+-rw-r--r--   0 zack       (501) staff       (20)     5894 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/user.py
+-rw-r--r--   0 zack       (501) staff       (20)     1718 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/user_dartboard_layout.py
+-rw-r--r--   0 zack       (501) staff       (20)     1991 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/user_dartboard_layout_create.py
+-rw-r--r--   0 zack       (501) staff       (20)      767 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/user_data_entity_retrieve_entity_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)      175 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/user_role.py
+-rw-r--r--   0 zack       (501) staff       (20)      313 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/user_status.py
+-rw-r--r--   0 zack       (501) staff       (20)     6910 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/user_update.py
+-rw-r--r--   0 zack       (501) staff       (20)     1804 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/validation_error_response.py
+-rw-r--r--   0 zack       (501) staff       (20)     1301 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/validation_error_response_items.py
+-rw-r--r--   0 zack       (501) staff       (20)     6445 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/view.py
+-rw-r--r--   0 zack       (501) staff       (20)     7752 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/view_create.py
+-rw-r--r--   0 zack       (501) staff       (20)      203 2024-04-16 22:06:25.000000 dart_tools-0.5.6/dart/generated/models/view_kind.py
+-rw-r--r--   0 zack       (501) staff       (20)     7922 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/view_update.py
+-rw-r--r--   0 zack       (501) staff       (20)     3316 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/yc_integration.py
+-rw-r--r--   0 zack       (501) staff       (20)     1782 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/models/zapier_integration.py
+-rw-r--r--   0 zack       (501) staff       (20)       25 2024-04-16 22:06:24.000000 dart_tools-0.5.6/dart/generated/py.typed
+-rw-r--r--   0 zack       (501) staff       (20)      968 2024-04-16 22:06:27.000000 dart_tools-0.5.6/dart/generated/types.py
+-rw-r--r--   0 zack       (501) staff       (20)     1905 2023-12-06 01:16:03.000000 dart_tools-0.5.6/dart/order_manager.py
+-rw-r--r--   0 zack       (501) staff       (20)      569 2023-12-01 08:32:06.000000 dart_tools-0.5.6/dart/webhook.py
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-04-16 22:06:41.834422 dart_tools-0.5.6/dart_tools.egg-info/
+-rw-r--r--   0 zack       (501) staff       (20)     7166 2024-04-16 22:06:41.000000 dart_tools-0.5.6/dart_tools.egg-info/PKG-INFO
+-rw-r--r--   0 zack       (501) staff       (20)     7417 2024-04-16 22:06:41.000000 dart_tools-0.5.6/dart_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 zack       (501) staff       (20)        1 2024-04-16 22:06:41.000000 dart_tools-0.5.6/dart_tools.egg-info/dependency_links.txt
+drwxr-xr-x   0 zack       (501) staff       (20)        0 2024-04-16 22:06:41.833928 dart_tools-0.5.6/dart_tools.egg-info/dist/
+-rw-r--r--   0 zack       (501) staff       (20)     8788 2023-06-03 08:11:34.000000 dart_tools-0.5.6/dart_tools.egg-info/dist/dart-tools-0.3.3.tar.gz
+-rw-r--r--   0 zack       (501) staff       (20)       34 2024-04-16 22:06:41.000000 dart_tools-0.5.6/dart_tools.egg-info/entry_points.txt
+-rw-r--r--   0 zack       (501) staff       (20)       38 2024-04-16 22:06:41.000000 dart_tools-0.5.6/dart_tools.egg-info/requires.txt
+-rw-r--r--   0 zack       (501) staff       (20)        5 2024-04-16 22:06:41.000000 dart_tools-0.5.6/dart_tools.egg-info/top_level.txt
+-rw-r--r--   0 zack       (501) staff       (20)     1891 2024-04-16 22:06:10.000000 dart_tools-0.5.6/pyproject.toml
+-rw-r--r--   0 zack       (501) staff       (20)       38 2024-04-16 22:06:41.834998 dart_tools-0.5.6/setup.cfg
```

### Comparing `dart-tools-0.5.5/LICENSE` & `dart_tools-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/PKG-INFO` & `dart_tools-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dart-tools
-Version: 0.5.5
+Version: 0.5.6
 Summary: The Dart CLI and Python Library
 Author-email: Dart Software Team <software@itsdart.com>
 License: MIT License
         
         Copyright (c) 2023 Dart
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dart-tools Version: 0.5.5 Summary: The Dart CLI and
+Metadata-Version: 2.1 Name: dart-tools Version: 0.5.6 Summary: The Dart CLI and
 Python Library Author-email: Dart Software Team
 itsdart.com> License: MIT License Copyright (c) 2023 Dart Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `dart-tools-0.5.5/README.md` & `dart_tools-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/dart.py` & `dart_tools-0.5.6/dart/dart.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,16 @@
 _CLIENT_DUID_KEY = "clientDuid"
 _HOST_KEY = "host"
 _HOSTS_KEY = "hosts"
 _AUTH_TOKEN_KEY = "authToken"
 _CSRF_TOKEN_KEY = "csrfToken"
 
 _DUID_CHARS = string.ascii_lowercase + string.ascii_uppercase + string.digits
+_NON_ALPHANUM_RE = re.compile(r"[^a-zA-Z0-9-]+")
+_REPEATED_DASH_RE = re.compile(r"-{2,}")
 _PRIORITY_MAP = {
     0: Priority.CRITICAL,
     1: Priority.HIGH,
     2: Priority.MEDIUM,
     3: Priority.LOW,
 }
 _SIZES = {1, 2, 3, 5, 8}
@@ -95,14 +97,31 @@
 
 
 # TODO dedupe these functions with other usages elsewhere
 def _make_duid():
     return "".join(random.choices(_DUID_CHARS, k=12))
 
 
+def trim_slug_str(s: str, length: int, max_under: int | None = None):
+    max_under = max_under if max_under is not None else length // 6
+    if len(s) <= length:
+        return s
+    for i in range(1, max_under + 1):
+        if s[length - i] == "-":
+            return s[: length - i]
+    return s[:length]
+
+
+def slugify_str(s: str, lower=False, trim_kwargs=None):
+    lowered = s.lower() if lower else s
+    formatted = _NON_ALPHANUM_RE.sub("-", lowered.replace("'", ""))
+    formatted = _REPEATED_DASH_RE.sub("-", formatted).strip("-")
+    return trim_slug_str(formatted, **trim_kwargs) if trim_kwargs is not None else formatted
+
+
 def _run_cmd(cmd):
     return subprocess.check_output(cmd, shell=True).decode()
 
 
 def _get_space_url(host, duid):
     return f"{host}/s/{duid}"
 
@@ -334,30 +353,18 @@
         except subprocess.CalledProcessError as ex:
             if "128" in str(ex):
                 return False
             raise ex
         return True
 
     @staticmethod
-    def _format_for_branch(s):
-        return re.sub(
-            r"-{2,}", "-", re.sub(r"[^a-z0-9-]+", "-", s.lower().replace("'", ""))
-        ).strip("-")
-
-    @staticmethod
     def make_task_name(email, task):
-        username = _Git._format_for_branch(email.split("@")[0])
-        title = _Git._format_for_branch(task.title)
-        long = f"{username}/{task.duid}-{title}"
-        if len(long) <= 60:
-            return long
-        for i in range(1, 11):
-            if long[60 - i] == "-":
-                return long[: 60 - i]
-        return long[:60]
+        username = slugify_str(email.split("@")[0], lower=True)
+        title = slugify_str(task.title, lower=True)
+        return trim_slug_str(f"{username}/{task.duid}-{title}", length=60)
 
     @staticmethod
     def get_current_branch():
         return _run_cmd("git rev-parse --abbrev-ref HEAD").strip()
 
     @staticmethod
     def ensure_in_repo():
```

### Comparing `dart-tools-0.5.5/dart/generated/api/transactions/transactions_create.py` & `dart_tools-0.5.6/dart/generated/api/transactions/transactions_create.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/client.py` & `dart_tools-0.5.6/dart/generated/client.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/__init__.py` & `dart_tools-0.5.6/dart/generated/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,14 +155,15 @@
 from .validation_error_response import ValidationErrorResponse
 from .validation_error_response_items import ValidationErrorResponseItems
 from .view import View
 from .view_create import ViewCreate
 from .view_kind import ViewKind
 from .view_update import ViewUpdate
 from .yc_integration import YcIntegration
+from .zapier_integration import ZapierIntegration
 
 __all__ = (
     "Attachment",
     "AttachmentCreate",
     "AttachmentUpdate",
     "Batch",
     "Brainstorm",
@@ -316,8 +317,9 @@
     "ValidationErrorResponse",
     "ValidationErrorResponseItems",
     "View",
     "ViewCreate",
     "ViewKind",
     "ViewUpdate",
     "YcIntegration",
+    "ZapierIntegration",
 )
```

### Comparing `dart-tools-0.5.5/dart/generated/models/attachment.py` & `dart_tools-0.5.6/dart/generated/models/attachment.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/attachment_create.py` & `dart_tools-0.5.6/dart/generated/models/attachment_create.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/attachment_update.py` & `dart_tools-0.5.6/dart/generated/models/attachment_update.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/batch.py` & `dart_tools-0.5.6/dart/generated/models/batch.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/brainstorm.py` & `dart_tools-0.5.6/dart/generated/models/brainstorm.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/brainstorm_create.py` & `dart_tools-0.5.6/dart/generated/models/brainstorm_create.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/brainstorm_update.py` & `dart_tools-0.5.6/dart/generated/models/brainstorm_update.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/color_name.py` & `dart_tools-0.5.6/dart/generated/models/color_name.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/comment.py` & `dart_tools-0.5.6/dart/generated/models/comment.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/comment_create.py` & `dart_tools-0.5.6/dart/generated/models/comment_create.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/comment_reaction.py` & `dart_tools-0.5.6/dart/generated/models/comment_reaction.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/comment_reaction_create.py` & `dart_tools-0.5.6/dart/generated/models/comment_reaction_create.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/comment_reaction_update.py` & `dart_tools-0.5.6/dart/generated/models/comment_reaction_update.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/comment_update.py` & `dart_tools-0.5.6/dart/generated/models/comment_update.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/dartboard.py` & `dart_tools-0.5.6/dart/generated/models/dartboard.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import datetime
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Type, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Type, TypeVar, Union, cast
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from dateutil.parser import isoparse
 
 from ..models.color_name import ColorName
 from ..models.dartboard_kind import DartboardKind
@@ -57,14 +57,16 @@
             * `Light Orange` - LIGHT_ORANGE
             * `Light Pink` - LIGHT_PINK
             * `Tan` - TAN
             * `Dark Gray` - DARK_GRAY
             * `Light Brown` - LIGHT_BROWN
             * `Light Gray` - LIGHT_GRAY
         user_duids_to_layout_duids (List['UserDartboardLayout']):
+        always_shown_property_duids (List[str]):
+        always_hidden_property_duids (List[str]):
         updated_by_client_duid (Union[Unset, None, str]):
         index (Optional[int]):
         started_at (Optional[datetime.datetime]):
         finished_at (Optional[datetime.datetime]):
     """
 
     duid: str
@@ -73,14 +75,16 @@
     order: str
     title: str
     description: str
     icon_kind: IconKind
     icon_name_or_emoji: str
     color_name: ColorName
     user_duids_to_layout_duids: List["UserDartboardLayout"]
+    always_shown_property_duids: List[str]
+    always_hidden_property_duids: List[str]
     index: Optional[int]
     started_at: Optional[datetime.datetime]
     finished_at: Optional[datetime.datetime]
     updated_by_client_duid: Union[Unset, None, str] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
@@ -98,14 +102,18 @@
 
         user_duids_to_layout_duids = []
         for user_duids_to_layout_duids_item_data in self.user_duids_to_layout_duids:
             user_duids_to_layout_duids_item = user_duids_to_layout_duids_item_data.to_dict()
 
             user_duids_to_layout_duids.append(user_duids_to_layout_duids_item)
 
+        always_shown_property_duids = self.always_shown_property_duids
+
+        always_hidden_property_duids = self.always_hidden_property_duids
+
         updated_by_client_duid = self.updated_by_client_duid
         index = self.index
         started_at = self.started_at.isoformat() if self.started_at else None
 
         finished_at = self.finished_at.isoformat() if self.finished_at else None
 
         field_dict: Dict[str, Any] = {}
@@ -118,14 +126,16 @@
                 "order": order,
                 "title": title,
                 "description": description,
                 "iconKind": icon_kind,
                 "iconNameOrEmoji": icon_name_or_emoji,
                 "colorName": color_name,
                 "userDuidsToLayoutDuids": user_duids_to_layout_duids,
+                "alwaysShownPropertyDuids": always_shown_property_duids,
+                "alwaysHiddenPropertyDuids": always_hidden_property_duids,
                 "index": index,
                 "startedAt": started_at,
                 "finishedAt": finished_at,
             }
         )
         if updated_by_client_duid is not UNSET:
             field_dict["updatedByClientDuid"] = updated_by_client_duid
@@ -158,14 +168,18 @@
         user_duids_to_layout_duids = []
         _user_duids_to_layout_duids = d.pop("userDuidsToLayoutDuids")
         for user_duids_to_layout_duids_item_data in _user_duids_to_layout_duids:
             user_duids_to_layout_duids_item = UserDartboardLayout.from_dict(user_duids_to_layout_duids_item_data)
 
             user_duids_to_layout_duids.append(user_duids_to_layout_duids_item)
 
+        always_shown_property_duids = cast(List[str], d.pop("alwaysShownPropertyDuids"))
+
+        always_hidden_property_duids = cast(List[str], d.pop("alwaysHiddenPropertyDuids"))
+
         updated_by_client_duid = d.pop("updatedByClientDuid", UNSET)
 
         index = d.pop("index")
 
         _started_at = d.pop("startedAt")
         started_at: Optional[datetime.datetime]
         if _started_at is None:
@@ -187,14 +201,16 @@
             order=order,
             title=title,
             description=description,
             icon_kind=icon_kind,
             icon_name_or_emoji=icon_name_or_emoji,
             color_name=color_name,
             user_duids_to_layout_duids=user_duids_to_layout_duids,
+            always_shown_property_duids=always_shown_property_duids,
+            always_hidden_property_duids=always_hidden_property_duids,
             updated_by_client_duid=updated_by_client_duid,
             index=index,
             started_at=started_at,
             finished_at=finished_at,
         )
 
         dartboard.additional_properties = d
```

### Comparing `dart-tools-0.5.5/dart/generated/models/dartboard_create.py` & `dart_tools-0.5.6/dart/generated/models/folder_update.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,32 @@
-import datetime
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
-from dateutil.parser import isoparse
 
 from ..models.color_name import ColorName
-from ..models.dartboard_kind import DartboardKind
+from ..models.folder_kind import FolderKind
 from ..models.icon_kind import IconKind
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="DartboardCreate")
+T = TypeVar("T", bound="FolderUpdate")
 
 
 @_attrs_define
-class DartboardCreate:
+class FolderUpdate:
     """
     Attributes:
         duid (str):
-        space_duid (str):
-        order (str):
-        kind (Union[Unset, DartboardKind]): * `Active` - ACTIVE
-            * `Next` - NEXT
-            * `Backlog` - BACKLOG
-            * `YC` - YC
-            * `Finished` - FINISHED
-            * `Custom` - CUSTOM
+        space_duid (Union[Unset, str]):
+        kind (Union[Unset, FolderKind]): * `Other` - OTHER
+            * `Default` - DEFAULT
+            * `Reports` - REPORTS
+        accessible_by_team (Union[Unset, bool]):
+        accessible_by_user_duids (Union[Unset, List[str]]):
+        order (Union[Unset, str]):
         title (Union[Unset, str]):
         description (Union[Unset, str]):
         icon_kind (Union[Unset, IconKind]): * `None` - NONE
             * `Icon` - ICON
             * `Emoji` - EMOJI
         icon_name_or_emoji (Union[Unset, str]):
         color_name (Union[Unset, ColorName]): * `Red` - RED
@@ -52,106 +49,102 @@
             * `Light Purple` - LIGHT_PURPLE
             * `Light Orange` - LIGHT_ORANGE
             * `Light Pink` - LIGHT_PINK
             * `Tan` - TAN
             * `Dark Gray` - DARK_GRAY
             * `Light Brown` - LIGHT_BROWN
             * `Light Gray` - LIGHT_GRAY
-        index (Union[Unset, None, int]):
-        started_at (Union[Unset, None, datetime.datetime]):
-        finished_at (Union[Unset, None, datetime.datetime]):
     """
 
     duid: str
-    space_duid: str
-    order: str
-    kind: Union[Unset, DartboardKind] = UNSET
+    space_duid: Union[Unset, str] = UNSET
+    kind: Union[Unset, FolderKind] = UNSET
+    accessible_by_team: Union[Unset, bool] = UNSET
+    accessible_by_user_duids: Union[Unset, List[str]] = UNSET
+    order: Union[Unset, str] = UNSET
     title: Union[Unset, str] = UNSET
     description: Union[Unset, str] = UNSET
     icon_kind: Union[Unset, IconKind] = UNSET
     icon_name_or_emoji: Union[Unset, str] = UNSET
     color_name: Union[Unset, ColorName] = UNSET
-    index: Union[Unset, None, int] = UNSET
-    started_at: Union[Unset, None, datetime.datetime] = UNSET
-    finished_at: Union[Unset, None, datetime.datetime] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         duid = self.duid
         space_duid = self.space_duid
-        order = self.order
         kind: Union[Unset, str] = UNSET
         if not isinstance(self.kind, Unset):
             kind = self.kind.value
 
+        accessible_by_team = self.accessible_by_team
+        accessible_by_user_duids: Union[Unset, List[str]] = UNSET
+        if not isinstance(self.accessible_by_user_duids, Unset):
+            accessible_by_user_duids = self.accessible_by_user_duids
+
+        order = self.order
         title = self.title
         description = self.description
         icon_kind: Union[Unset, str] = UNSET
         if not isinstance(self.icon_kind, Unset):
             icon_kind = self.icon_kind.value
 
         icon_name_or_emoji = self.icon_name_or_emoji
         color_name: Union[Unset, str] = UNSET
         if not isinstance(self.color_name, Unset):
             color_name = self.color_name.value
 
-        index = self.index
-        started_at: Union[Unset, None, str] = UNSET
-        if not isinstance(self.started_at, Unset):
-            started_at = self.started_at.isoformat() if self.started_at else None
-
-        finished_at: Union[Unset, None, str] = UNSET
-        if not isinstance(self.finished_at, Unset):
-            finished_at = self.finished_at.isoformat() if self.finished_at else None
-
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "duid": duid,
-                "spaceDuid": space_duid,
-                "order": order,
             }
         )
+        if space_duid is not UNSET:
+            field_dict["spaceDuid"] = space_duid
         if kind is not UNSET:
             field_dict["kind"] = kind
+        if accessible_by_team is not UNSET:
+            field_dict["accessibleByTeam"] = accessible_by_team
+        if accessible_by_user_duids is not UNSET:
+            field_dict["accessibleByUserDuids"] = accessible_by_user_duids
+        if order is not UNSET:
+            field_dict["order"] = order
         if title is not UNSET:
             field_dict["title"] = title
         if description is not UNSET:
             field_dict["description"] = description
         if icon_kind is not UNSET:
             field_dict["iconKind"] = icon_kind
         if icon_name_or_emoji is not UNSET:
             field_dict["iconNameOrEmoji"] = icon_name_or_emoji
         if color_name is not UNSET:
             field_dict["colorName"] = color_name
-        if index is not UNSET:
-            field_dict["index"] = index
-        if started_at is not UNSET:
-            field_dict["startedAt"] = started_at
-        if finished_at is not UNSET:
-            field_dict["finishedAt"] = finished_at
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         duid = d.pop("duid")
 
-        space_duid = d.pop("spaceDuid")
-
-        order = d.pop("order")
+        space_duid = d.pop("spaceDuid", UNSET)
 
         _kind = d.pop("kind", UNSET)
-        kind: Union[Unset, DartboardKind]
+        kind: Union[Unset, FolderKind]
         if isinstance(_kind, Unset):
             kind = UNSET
         else:
-            kind = DartboardKind(_kind)
+            kind = FolderKind(_kind)
+
+        accessible_by_team = d.pop("accessibleByTeam", UNSET)
+
+        accessible_by_user_duids = cast(List[str], d.pop("accessibleByUserDuids", UNSET))
+
+        order = d.pop("order", UNSET)
 
         title = d.pop("title", UNSET)
 
         description = d.pop("description", UNSET)
 
         _icon_kind = d.pop("iconKind", UNSET)
         icon_kind: Union[Unset, IconKind]
@@ -165,51 +158,30 @@
         _color_name = d.pop("colorName", UNSET)
         color_name: Union[Unset, ColorName]
         if isinstance(_color_name, Unset):
             color_name = UNSET
         else:
             color_name = ColorName(_color_name)
 
-        index = d.pop("index", UNSET)
-
-        _started_at = d.pop("startedAt", UNSET)
-        started_at: Union[Unset, None, datetime.datetime]
-        if _started_at is None:
-            started_at = None
-        elif isinstance(_started_at, Unset):
-            started_at = UNSET
-        else:
-            started_at = isoparse(_started_at)
-
-        _finished_at = d.pop("finishedAt", UNSET)
-        finished_at: Union[Unset, None, datetime.datetime]
-        if _finished_at is None:
-            finished_at = None
-        elif isinstance(_finished_at, Unset):
-            finished_at = UNSET
-        else:
-            finished_at = isoparse(_finished_at)
-
-        dartboard_create = cls(
+        folder_update = cls(
             duid=duid,
             space_duid=space_duid,
-            order=order,
             kind=kind,
+            accessible_by_team=accessible_by_team,
+            accessible_by_user_duids=accessible_by_user_duids,
+            order=order,
             title=title,
             description=description,
             icon_kind=icon_kind,
             icon_name_or_emoji=icon_name_or_emoji,
             color_name=color_name,
-            index=index,
-            started_at=started_at,
-            finished_at=finished_at,
         )
 
-        dartboard_create.additional_properties = d
-        return dartboard_create
+        folder_update.additional_properties = d
+        return folder_update
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart-tools-0.5.5/dart/generated/models/dartboard_update.py` & `dart_tools-0.5.6/dart/generated/models/user_update.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,32 @@
-import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
-from dateutil.parser import isoparse
 
 from ..models.color_name import ColorName
-from ..models.dartboard_kind import DartboardKind
-from ..models.icon_kind import IconKind
+from ..models.theme import Theme
+from ..models.user_role import UserRole
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="DartboardUpdate")
+T = TypeVar("T", bound="UserUpdate")
 
 
 @_attrs_define
-class DartboardUpdate:
+class UserUpdate:
     """
     Attributes:
         duid (str):
-        space_duid (Union[Unset, str]):
-        kind (Union[Unset, DartboardKind]): * `Active` - ACTIVE
-            * `Next` - NEXT
-            * `Backlog` - BACKLOG
-            * `YC` - YC
-            * `Finished` - FINISHED
-            * `Custom` - CUSTOM
-        order (Union[Unset, str]):
-        title (Union[Unset, str]):
-        description (Union[Unset, str]):
-        icon_kind (Union[Unset, IconKind]): * `None` - NONE
-            * `Icon` - ICON
-            * `Emoji` - EMOJI
-        icon_name_or_emoji (Union[Unset, str]):
+        role (Union[Unset, UserRole]): * `Admin` - ADMIN
+            * `Member` - MEMBER
+            * `Guest` - GUEST
+        name (Union[Unset, str]):
+        theme (Union[Unset, Theme]): * `System Default` - SYSTEM_DEFAULT
+            * `Light` - LIGHT
+            * `Dark` - DARK
         color_name (Union[Unset, ColorName]): * `Red` - RED
             * `Dark Blue` - DARK_BLUE
             * `Dark Orange` - DARK_ORANGE
             * `Dark Green` - DARK_GREEN
             * `Purple` - PURPLE
             * `Dark Teal` - DARK_TEAL
             * `Pink` - PINK
@@ -52,166 +43,151 @@
             * `Light Purple` - LIGHT_PURPLE
             * `Light Orange` - LIGHT_ORANGE
             * `Light Pink` - LIGHT_PINK
             * `Tan` - TAN
             * `Dark Gray` - DARK_GRAY
             * `Light Brown` - LIGHT_BROWN
             * `Light Gray` - LIGHT_GRAY
-        index (Union[Unset, None, int]):
-        started_at (Union[Unset, None, datetime.datetime]):
-        finished_at (Union[Unset, None, datetime.datetime]):
+        open_in_native_app (Union[Unset, bool]):
+        first_day_of_week (Union[Unset, int]):
+        sections (Union[Unset, Any]):
+        notification_default (Union[Unset, bool]):
+        notification_in_app (Union[Unset, bool]):
+        notification_email (Union[Unset, bool]):
+        notification_slack (Union[Unset, bool]):
     """
 
     duid: str
-    space_duid: Union[Unset, str] = UNSET
-    kind: Union[Unset, DartboardKind] = UNSET
-    order: Union[Unset, str] = UNSET
-    title: Union[Unset, str] = UNSET
-    description: Union[Unset, str] = UNSET
-    icon_kind: Union[Unset, IconKind] = UNSET
-    icon_name_or_emoji: Union[Unset, str] = UNSET
+    role: Union[Unset, UserRole] = UNSET
+    name: Union[Unset, str] = UNSET
+    theme: Union[Unset, Theme] = UNSET
     color_name: Union[Unset, ColorName] = UNSET
-    index: Union[Unset, None, int] = UNSET
-    started_at: Union[Unset, None, datetime.datetime] = UNSET
-    finished_at: Union[Unset, None, datetime.datetime] = UNSET
+    open_in_native_app: Union[Unset, bool] = UNSET
+    first_day_of_week: Union[Unset, int] = UNSET
+    sections: Union[Unset, Any] = UNSET
+    notification_default: Union[Unset, bool] = UNSET
+    notification_in_app: Union[Unset, bool] = UNSET
+    notification_email: Union[Unset, bool] = UNSET
+    notification_slack: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         duid = self.duid
-        space_duid = self.space_duid
-        kind: Union[Unset, str] = UNSET
-        if not isinstance(self.kind, Unset):
-            kind = self.kind.value
-
-        order = self.order
-        title = self.title
-        description = self.description
-        icon_kind: Union[Unset, str] = UNSET
-        if not isinstance(self.icon_kind, Unset):
-            icon_kind = self.icon_kind.value
+        role: Union[Unset, str] = UNSET
+        if not isinstance(self.role, Unset):
+            role = self.role.value
+
+        name = self.name
+        theme: Union[Unset, str] = UNSET
+        if not isinstance(self.theme, Unset):
+            theme = self.theme.value
 
-        icon_name_or_emoji = self.icon_name_or_emoji
         color_name: Union[Unset, str] = UNSET
         if not isinstance(self.color_name, Unset):
             color_name = self.color_name.value
 
-        index = self.index
-        started_at: Union[Unset, None, str] = UNSET
-        if not isinstance(self.started_at, Unset):
-            started_at = self.started_at.isoformat() if self.started_at else None
-
-        finished_at: Union[Unset, None, str] = UNSET
-        if not isinstance(self.finished_at, Unset):
-            finished_at = self.finished_at.isoformat() if self.finished_at else None
+        open_in_native_app = self.open_in_native_app
+        first_day_of_week = self.first_day_of_week
+        sections = self.sections
+        notification_default = self.notification_default
+        notification_in_app = self.notification_in_app
+        notification_email = self.notification_email
+        notification_slack = self.notification_slack
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "duid": duid,
             }
         )
-        if space_duid is not UNSET:
-            field_dict["spaceDuid"] = space_duid
-        if kind is not UNSET:
-            field_dict["kind"] = kind
-        if order is not UNSET:
-            field_dict["order"] = order
-        if title is not UNSET:
-            field_dict["title"] = title
-        if description is not UNSET:
-            field_dict["description"] = description
-        if icon_kind is not UNSET:
-            field_dict["iconKind"] = icon_kind
-        if icon_name_or_emoji is not UNSET:
-            field_dict["iconNameOrEmoji"] = icon_name_or_emoji
+        if role is not UNSET:
+            field_dict["role"] = role
+        if name is not UNSET:
+            field_dict["name"] = name
+        if theme is not UNSET:
+            field_dict["theme"] = theme
         if color_name is not UNSET:
             field_dict["colorName"] = color_name
-        if index is not UNSET:
-            field_dict["index"] = index
-        if started_at is not UNSET:
-            field_dict["startedAt"] = started_at
-        if finished_at is not UNSET:
-            field_dict["finishedAt"] = finished_at
+        if open_in_native_app is not UNSET:
+            field_dict["openInNativeApp"] = open_in_native_app
+        if first_day_of_week is not UNSET:
+            field_dict["firstDayOfWeek"] = first_day_of_week
+        if sections is not UNSET:
+            field_dict["sections"] = sections
+        if notification_default is not UNSET:
+            field_dict["notificationDefault"] = notification_default
+        if notification_in_app is not UNSET:
+            field_dict["notificationInApp"] = notification_in_app
+        if notification_email is not UNSET:
+            field_dict["notificationEmail"] = notification_email
+        if notification_slack is not UNSET:
+            field_dict["notificationSlack"] = notification_slack
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         duid = d.pop("duid")
 
-        space_duid = d.pop("spaceDuid", UNSET)
-
-        _kind = d.pop("kind", UNSET)
-        kind: Union[Unset, DartboardKind]
-        if isinstance(_kind, Unset):
-            kind = UNSET
+        _role = d.pop("role", UNSET)
+        role: Union[Unset, UserRole]
+        if isinstance(_role, Unset):
+            role = UNSET
         else:
-            kind = DartboardKind(_kind)
-
-        order = d.pop("order", UNSET)
-
-        title = d.pop("title", UNSET)
+            role = UserRole(_role)
 
-        description = d.pop("description", UNSET)
+        name = d.pop("name", UNSET)
 
-        _icon_kind = d.pop("iconKind", UNSET)
-        icon_kind: Union[Unset, IconKind]
-        if isinstance(_icon_kind, Unset):
-            icon_kind = UNSET
+        _theme = d.pop("theme", UNSET)
+        theme: Union[Unset, Theme]
+        if isinstance(_theme, Unset):
+            theme = UNSET
         else:
-            icon_kind = IconKind(_icon_kind)
-
-        icon_name_or_emoji = d.pop("iconNameOrEmoji", UNSET)
+            theme = Theme(_theme)
 
         _color_name = d.pop("colorName", UNSET)
         color_name: Union[Unset, ColorName]
         if isinstance(_color_name, Unset):
             color_name = UNSET
         else:
             color_name = ColorName(_color_name)
 
-        index = d.pop("index", UNSET)
+        open_in_native_app = d.pop("openInNativeApp", UNSET)
 
-        _started_at = d.pop("startedAt", UNSET)
-        started_at: Union[Unset, None, datetime.datetime]
-        if _started_at is None:
-            started_at = None
-        elif isinstance(_started_at, Unset):
-            started_at = UNSET
-        else:
-            started_at = isoparse(_started_at)
+        first_day_of_week = d.pop("firstDayOfWeek", UNSET)
 
-        _finished_at = d.pop("finishedAt", UNSET)
-        finished_at: Union[Unset, None, datetime.datetime]
-        if _finished_at is None:
-            finished_at = None
-        elif isinstance(_finished_at, Unset):
-            finished_at = UNSET
-        else:
-            finished_at = isoparse(_finished_at)
+        sections = d.pop("sections", UNSET)
+
+        notification_default = d.pop("notificationDefault", UNSET)
+
+        notification_in_app = d.pop("notificationInApp", UNSET)
+
+        notification_email = d.pop("notificationEmail", UNSET)
+
+        notification_slack = d.pop("notificationSlack", UNSET)
 
-        dartboard_update = cls(
+        user_update = cls(
             duid=duid,
-            space_duid=space_duid,
-            kind=kind,
-            order=order,
-            title=title,
-            description=description,
-            icon_kind=icon_kind,
-            icon_name_or_emoji=icon_name_or_emoji,
+            role=role,
+            name=name,
+            theme=theme,
             color_name=color_name,
-            index=index,
-            started_at=started_at,
-            finished_at=finished_at,
+            open_in_native_app=open_in_native_app,
+            first_day_of_week=first_day_of_week,
+            sections=sections,
+            notification_default=notification_default,
+            notification_in_app=notification_in_app,
+            notification_email=notification_email,
+            notification_slack=notification_slack,
         )
 
-        dartboard_update.additional_properties = d
-        return dartboard_update
+        user_update.additional_properties = d
+        return user_update
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart-tools-0.5.5/dart/generated/models/discord_integration.py` & `dart_tools-0.5.6/dart/generated/models/discord_integration.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/doc.py` & `dart_tools-0.5.6/dart/generated/models/doc.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/doc_create.py` & `dart_tools-0.5.6/dart/generated/models/doc_update.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,37 +5,38 @@
 
 from ..models.color_name import ColorName
 from ..models.doc_source_type import DocSourceType
 from ..models.icon_kind import IconKind
 from ..models.report_kind import ReportKind
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="DocCreate")
+T = TypeVar("T", bound="DocUpdate")
 
 
 @_attrs_define
-class DocCreate:
+class DocUpdate:
     """
     Attributes:
         duid (str):
-        folder_duid (str):
-        order (str):
         source_user (Union[Unset, None, str]):
         source_type (Union[Unset, DocSourceType]): * `Unknown` - UNKNOWN
             * `Onboarding` - ONBOARDING
             * `Recommendation` - RECOMMENDATION
             * `GeneratedReport` - GENERATED_REPORT
             * `ChatGPT` - CHAT_GPT
             * `Application` - APPLICATION Default: DocSourceType.UNKNOWN.
         drafter_duid (Union[Unset, None, str]):
         in_trash (Union[Unset, bool]):
+        folder_duid (Union[Unset, str]):
         report_kind (Union[Unset, None, ReportKind]): * `Standup` - STANDUP
             * `Changelog` - CHANGELOG
+        order (Union[Unset, str]):
         title (Union[Unset, str]):
         text (Union[Unset, Any]):
+        text_markdown (Union[Unset, str]):
         edited_by_ai (Union[Unset, bool]):
         recommendation_duid (Union[Unset, None, str]):
         editor_duids (Union[Unset, List[str]]):
         subscriber_duids (Union[Unset, List[str]]):
         icon_kind (Union[Unset, IconKind]): * `None` - NONE
             * `Icon` - ICON
             * `Emoji` - EMOJI
@@ -63,49 +64,51 @@
             * `Tan` - TAN
             * `Dark Gray` - DARK_GRAY
             * `Light Brown` - LIGHT_BROWN
             * `Light Gray` - LIGHT_GRAY
     """
 
     duid: str
-    folder_duid: str
-    order: str
     source_user: Union[Unset, None, str] = UNSET
     source_type: Union[Unset, DocSourceType] = DocSourceType.UNKNOWN
     drafter_duid: Union[Unset, None, str] = UNSET
     in_trash: Union[Unset, bool] = UNSET
+    folder_duid: Union[Unset, str] = UNSET
     report_kind: Union[Unset, None, ReportKind] = UNSET
+    order: Union[Unset, str] = UNSET
     title: Union[Unset, str] = UNSET
     text: Union[Unset, Any] = UNSET
+    text_markdown: Union[Unset, str] = UNSET
     edited_by_ai: Union[Unset, bool] = UNSET
     recommendation_duid: Union[Unset, None, str] = UNSET
     editor_duids: Union[Unset, List[str]] = UNSET
     subscriber_duids: Union[Unset, List[str]] = UNSET
     icon_kind: Union[Unset, IconKind] = UNSET
     icon_name_or_emoji: Union[Unset, str] = UNSET
     color_name: Union[Unset, ColorName] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         duid = self.duid
-        folder_duid = self.folder_duid
-        order = self.order
         source_user = self.source_user
         source_type: Union[Unset, str] = UNSET
         if not isinstance(self.source_type, Unset):
             source_type = self.source_type.value
 
         drafter_duid = self.drafter_duid
         in_trash = self.in_trash
+        folder_duid = self.folder_duid
         report_kind: Union[Unset, None, str] = UNSET
         if not isinstance(self.report_kind, Unset):
             report_kind = self.report_kind.value if self.report_kind else None
 
+        order = self.order
         title = self.title
         text = self.text
+        text_markdown = self.text_markdown
         edited_by_ai = self.edited_by_ai
         recommendation_duid = self.recommendation_duid
         editor_duids: Union[Unset, List[str]] = UNSET
         if not isinstance(self.editor_duids, Unset):
             editor_duids = self.editor_duids
 
         subscriber_duids: Union[Unset, List[str]] = UNSET
@@ -122,32 +125,36 @@
             color_name = self.color_name.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "duid": duid,
-                "folderDuid": folder_duid,
-                "order": order,
             }
         )
         if source_user is not UNSET:
             field_dict["sourceUser"] = source_user
         if source_type is not UNSET:
             field_dict["sourceType"] = source_type
         if drafter_duid is not UNSET:
             field_dict["drafterDuid"] = drafter_duid
         if in_trash is not UNSET:
             field_dict["inTrash"] = in_trash
+        if folder_duid is not UNSET:
+            field_dict["folderDuid"] = folder_duid
         if report_kind is not UNSET:
             field_dict["reportKind"] = report_kind
+        if order is not UNSET:
+            field_dict["order"] = order
         if title is not UNSET:
             field_dict["title"] = title
         if text is not UNSET:
             field_dict["text"] = text
+        if text_markdown is not UNSET:
+            field_dict["textMarkdown"] = text_markdown
         if edited_by_ai is not UNSET:
             field_dict["editedByAi"] = edited_by_ai
         if recommendation_duid is not UNSET:
             field_dict["recommendationDuid"] = recommendation_duid
         if editor_duids is not UNSET:
             field_dict["editorDuids"] = editor_duids
         if subscriber_duids is not UNSET:
@@ -162,44 +169,46 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         duid = d.pop("duid")
 
-        folder_duid = d.pop("folderDuid")
-
-        order = d.pop("order")
-
         source_user = d.pop("sourceUser", UNSET)
 
         _source_type = d.pop("sourceType", UNSET)
         source_type: Union[Unset, DocSourceType]
         if isinstance(_source_type, Unset):
             source_type = UNSET
         else:
             source_type = DocSourceType(_source_type)
 
         drafter_duid = d.pop("drafterDuid", UNSET)
 
         in_trash = d.pop("inTrash", UNSET)
 
+        folder_duid = d.pop("folderDuid", UNSET)
+
         _report_kind = d.pop("reportKind", UNSET)
         report_kind: Union[Unset, None, ReportKind]
         if _report_kind is None:
             report_kind = None
         elif isinstance(_report_kind, Unset):
             report_kind = UNSET
         else:
             report_kind = ReportKind(_report_kind)
 
+        order = d.pop("order", UNSET)
+
         title = d.pop("title", UNSET)
 
         text = d.pop("text", UNSET)
 
+        text_markdown = d.pop("textMarkdown", UNSET)
+
         edited_by_ai = d.pop("editedByAi", UNSET)
 
         recommendation_duid = d.pop("recommendationDuid", UNSET)
 
         editor_duids = cast(List[str], d.pop("editorDuids", UNSET))
 
         subscriber_duids = cast(List[str], d.pop("subscriberDuids", UNSET))
@@ -216,36 +225,37 @@
         _color_name = d.pop("colorName", UNSET)
         color_name: Union[Unset, ColorName]
         if isinstance(_color_name, Unset):
             color_name = UNSET
         else:
             color_name = ColorName(_color_name)
 
-        doc_create = cls(
+        doc_update = cls(
             duid=duid,
-            folder_duid=folder_duid,
-            order=order,
             source_user=source_user,
             source_type=source_type,
             drafter_duid=drafter_duid,
             in_trash=in_trash,
+            folder_duid=folder_duid,
             report_kind=report_kind,
+            order=order,
             title=title,
             text=text,
+            text_markdown=text_markdown,
             edited_by_ai=edited_by_ai,
             recommendation_duid=recommendation_duid,
             editor_duids=editor_duids,
             subscriber_duids=subscriber_duids,
             icon_kind=icon_kind,
             icon_name_or_emoji=icon_name_or_emoji,
             color_name=color_name,
         )
 
-        doc_create.additional_properties = d
-        return doc_create
+        doc_update.additional_properties = d
+        return doc_update
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart-tools-0.5.5/dart/generated/models/doc_update.py` & `dart_tools-0.5.6/dart/generated/models/doc_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 
 from ..models.color_name import ColorName
 from ..models.doc_source_type import DocSourceType
 from ..models.icon_kind import IconKind
 from ..models.report_kind import ReportKind
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="DocUpdate")
+T = TypeVar("T", bound="DocCreate")
 
 
 @_attrs_define
-class DocUpdate:
+class DocCreate:
     """
     Attributes:
         duid (str):
         source_user (Union[Unset, None, str]):
         source_type (Union[Unset, DocSourceType]): * `Unknown` - UNKNOWN
             * `Onboarding` - ONBOARDING
             * `Recommendation` - RECOMMENDATION
@@ -28,14 +28,15 @@
         in_trash (Union[Unset, bool]):
         folder_duid (Union[Unset, str]):
         report_kind (Union[Unset, None, ReportKind]): * `Standup` - STANDUP
             * `Changelog` - CHANGELOG
         order (Union[Unset, str]):
         title (Union[Unset, str]):
         text (Union[Unset, Any]):
+        text_markdown (Union[Unset, str]):
         edited_by_ai (Union[Unset, bool]):
         recommendation_duid (Union[Unset, None, str]):
         editor_duids (Union[Unset, List[str]]):
         subscriber_duids (Union[Unset, List[str]]):
         icon_kind (Union[Unset, IconKind]): * `None` - NONE
             * `Icon` - ICON
             * `Emoji` - EMOJI
@@ -72,14 +73,15 @@
     drafter_duid: Union[Unset, None, str] = UNSET
     in_trash: Union[Unset, bool] = UNSET
     folder_duid: Union[Unset, str] = UNSET
     report_kind: Union[Unset, None, ReportKind] = UNSET
     order: Union[Unset, str] = UNSET
     title: Union[Unset, str] = UNSET
     text: Union[Unset, Any] = UNSET
+    text_markdown: Union[Unset, str] = UNSET
     edited_by_ai: Union[Unset, bool] = UNSET
     recommendation_duid: Union[Unset, None, str] = UNSET
     editor_duids: Union[Unset, List[str]] = UNSET
     subscriber_duids: Union[Unset, List[str]] = UNSET
     icon_kind: Union[Unset, IconKind] = UNSET
     icon_name_or_emoji: Union[Unset, str] = UNSET
     color_name: Union[Unset, ColorName] = UNSET
@@ -98,14 +100,15 @@
         report_kind: Union[Unset, None, str] = UNSET
         if not isinstance(self.report_kind, Unset):
             report_kind = self.report_kind.value if self.report_kind else None
 
         order = self.order
         title = self.title
         text = self.text
+        text_markdown = self.text_markdown
         edited_by_ai = self.edited_by_ai
         recommendation_duid = self.recommendation_duid
         editor_duids: Union[Unset, List[str]] = UNSET
         if not isinstance(self.editor_duids, Unset):
             editor_duids = self.editor_duids
 
         subscriber_duids: Union[Unset, List[str]] = UNSET
@@ -142,14 +145,16 @@
             field_dict["reportKind"] = report_kind
         if order is not UNSET:
             field_dict["order"] = order
         if title is not UNSET:
             field_dict["title"] = title
         if text is not UNSET:
             field_dict["text"] = text
+        if text_markdown is not UNSET:
+            field_dict["textMarkdown"] = text_markdown
         if edited_by_ai is not UNSET:
             field_dict["editedByAi"] = edited_by_ai
         if recommendation_duid is not UNSET:
             field_dict["recommendationDuid"] = recommendation_duid
         if editor_duids is not UNSET:
             field_dict["editorDuids"] = editor_duids
         if subscriber_duids is not UNSET:
@@ -194,14 +199,16 @@
 
         order = d.pop("order", UNSET)
 
         title = d.pop("title", UNSET)
 
         text = d.pop("text", UNSET)
 
+        text_markdown = d.pop("textMarkdown", UNSET)
+
         edited_by_ai = d.pop("editedByAi", UNSET)
 
         recommendation_duid = d.pop("recommendationDuid", UNSET)
 
         editor_duids = cast(List[str], d.pop("editorDuids", UNSET))
 
         subscriber_duids = cast(List[str], d.pop("subscriberDuids", UNSET))
@@ -218,36 +225,37 @@
         _color_name = d.pop("colorName", UNSET)
         color_name: Union[Unset, ColorName]
         if isinstance(_color_name, Unset):
             color_name = UNSET
         else:
             color_name = ColorName(_color_name)
 
-        doc_update = cls(
+        doc_create = cls(
             duid=duid,
             source_user=source_user,
             source_type=source_type,
             drafter_duid=drafter_duid,
             in_trash=in_trash,
             folder_duid=folder_duid,
             report_kind=report_kind,
             order=order,
             title=title,
             text=text,
+            text_markdown=text_markdown,
             edited_by_ai=edited_by_ai,
             recommendation_duid=recommendation_duid,
             editor_duids=editor_duids,
             subscriber_duids=subscriber_duids,
             icon_kind=icon_kind,
             icon_name_or_emoji=icon_name_or_emoji,
             color_name=color_name,
         )
 
-        doc_update.additional_properties = d
-        return doc_update
+        doc_create.additional_properties = d
+        return doc_create
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart-tools-0.5.5/dart/generated/models/event.py` & `dart_tools-0.5.6/dart/generated/models/event.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/event_actor.py` & `dart_tools-0.5.6/dart/generated/models/event_actor.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/event_create.py` & `dart_tools-0.5.6/dart/generated/models/event_create.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/event_kind.py` & `dart_tools-0.5.6/dart/generated/models/event_kind.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/event_subscription.py` & `dart_tools-0.5.6/dart/generated/models/event_subscription.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/event_subscription_update.py` & `dart_tools-0.5.6/dart/generated/models/event_subscription_update.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/filter_applicability.py` & `dart_tools-0.5.6/dart/generated/models/filter_applicability.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/filter_assignee.py` & `dart_tools-0.5.6/dart/generated/models/filter_assignee.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/filter_group.py` & `dart_tools-0.5.6/dart/generated/models/filter_group.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/filter_search.py` & `dart_tools-0.5.6/dart/generated/models/filter_search.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/filter_set.py` & `dart_tools-0.5.6/dart/generated/models/filter_set.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/folder.py` & `dart_tools-0.5.6/dart/generated/models/folder.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/folder_create.py` & `dart_tools-0.5.6/dart/generated/models/folder_create.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/folder_update.py` & `dart_tools-0.5.6/dart/generated/models/form_create.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,27 @@
-from typing import Any, Dict, List, Type, TypeVar, Union, cast
+from typing import Any, Dict, List, Type, TypeVar, Union
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..models.color_name import ColorName
-from ..models.folder_kind import FolderKind
 from ..models.icon_kind import IconKind
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="FolderUpdate")
+T = TypeVar("T", bound="FormCreate")
 
 
 @_attrs_define
-class FolderUpdate:
+class FormCreate:
     """
     Attributes:
         duid (str):
-        space_duid (Union[Unset, str]):
-        kind (Union[Unset, FolderKind]): * `Other` - OTHER
-            * `Default` - DEFAULT
-            * `Reports` - REPORTS
-        accessible_by_team (Union[Unset, bool]):
-        accessible_by_user_duids (Union[Unset, List[str]]):
-        order (Union[Unset, str]):
+        order (str):
+        hidden (Union[Unset, bool]):
+        public (Union[Unset, bool]):
         title (Union[Unset, str]):
         description (Union[Unset, str]):
         icon_kind (Union[Unset, IconKind]): * `None` - NONE
             * `Icon` - ICON
             * `Emoji` - EMOJI
         icon_name_or_emoji (Union[Unset, str]):
         color_name (Union[Unset, ColorName]): * `Red` - RED
@@ -52,39 +47,29 @@
             * `Tan` - TAN
             * `Dark Gray` - DARK_GRAY
             * `Light Brown` - LIGHT_BROWN
             * `Light Gray` - LIGHT_GRAY
     """
 
     duid: str
-    space_duid: Union[Unset, str] = UNSET
-    kind: Union[Unset, FolderKind] = UNSET
-    accessible_by_team: Union[Unset, bool] = UNSET
-    accessible_by_user_duids: Union[Unset, List[str]] = UNSET
-    order: Union[Unset, str] = UNSET
+    order: str
+    hidden: Union[Unset, bool] = UNSET
+    public: Union[Unset, bool] = UNSET
     title: Union[Unset, str] = UNSET
     description: Union[Unset, str] = UNSET
     icon_kind: Union[Unset, IconKind] = UNSET
     icon_name_or_emoji: Union[Unset, str] = UNSET
     color_name: Union[Unset, ColorName] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         duid = self.duid
-        space_duid = self.space_duid
-        kind: Union[Unset, str] = UNSET
-        if not isinstance(self.kind, Unset):
-            kind = self.kind.value
-
-        accessible_by_team = self.accessible_by_team
-        accessible_by_user_duids: Union[Unset, List[str]] = UNSET
-        if not isinstance(self.accessible_by_user_duids, Unset):
-            accessible_by_user_duids = self.accessible_by_user_duids
-
         order = self.order
+        hidden = self.hidden
+        public = self.public
         title = self.title
         description = self.description
         icon_kind: Union[Unset, str] = UNSET
         if not isinstance(self.icon_kind, Unset):
             icon_kind = self.icon_kind.value
 
         icon_name_or_emoji = self.icon_name_or_emoji
@@ -93,26 +78,21 @@
             color_name = self.color_name.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "duid": duid,
+                "order": order,
             }
         )
-        if space_duid is not UNSET:
-            field_dict["spaceDuid"] = space_duid
-        if kind is not UNSET:
-            field_dict["kind"] = kind
-        if accessible_by_team is not UNSET:
-            field_dict["accessibleByTeam"] = accessible_by_team
-        if accessible_by_user_duids is not UNSET:
-            field_dict["accessibleByUserDuids"] = accessible_by_user_duids
-        if order is not UNSET:
-            field_dict["order"] = order
+        if hidden is not UNSET:
+            field_dict["hidden"] = hidden
+        if public is not UNSET:
+            field_dict["public"] = public
         if title is not UNSET:
             field_dict["title"] = title
         if description is not UNSET:
             field_dict["description"] = description
         if icon_kind is not UNSET:
             field_dict["iconKind"] = icon_kind
         if icon_name_or_emoji is not UNSET:
@@ -123,28 +103,19 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         duid = d.pop("duid")
 
-        space_duid = d.pop("spaceDuid", UNSET)
-
-        _kind = d.pop("kind", UNSET)
-        kind: Union[Unset, FolderKind]
-        if isinstance(_kind, Unset):
-            kind = UNSET
-        else:
-            kind = FolderKind(_kind)
-
-        accessible_by_team = d.pop("accessibleByTeam", UNSET)
+        order = d.pop("order")
 
-        accessible_by_user_duids = cast(List[str], d.pop("accessibleByUserDuids", UNSET))
+        hidden = d.pop("hidden", UNSET)
 
-        order = d.pop("order", UNSET)
+        public = d.pop("public", UNSET)
 
         title = d.pop("title", UNSET)
 
         description = d.pop("description", UNSET)
 
         _icon_kind = d.pop("iconKind", UNSET)
         icon_kind: Union[Unset, IconKind]
@@ -158,30 +129,28 @@
         _color_name = d.pop("colorName", UNSET)
         color_name: Union[Unset, ColorName]
         if isinstance(_color_name, Unset):
             color_name = UNSET
         else:
             color_name = ColorName(_color_name)
 
-        folder_update = cls(
+        form_create = cls(
             duid=duid,
-            space_duid=space_duid,
-            kind=kind,
-            accessible_by_team=accessible_by_team,
-            accessible_by_user_duids=accessible_by_user_duids,
             order=order,
+            hidden=hidden,
+            public=public,
             title=title,
             description=description,
             icon_kind=icon_kind,
             icon_name_or_emoji=icon_name_or_emoji,
             color_name=color_name,
         )
 
-        folder_update.additional_properties = d
-        return folder_update
+        form_create.additional_properties = d
+        return form_create
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart-tools-0.5.5/dart/generated/models/form.py` & `dart_tools-0.5.6/dart/generated/models/form.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/form_create.py` & `dart_tools-0.5.6/dart/generated/models/form_update.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..models.color_name import ColorName
 from ..models.icon_kind import IconKind
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="FormCreate")
+T = TypeVar("T", bound="FormUpdate")
 
 
 @_attrs_define
-class FormCreate:
+class FormUpdate:
     """
     Attributes:
         duid (str):
-        order (str):
         hidden (Union[Unset, bool]):
         public (Union[Unset, bool]):
+        order (Union[Unset, str]):
         title (Union[Unset, str]):
         description (Union[Unset, str]):
         icon_kind (Union[Unset, IconKind]): * `None` - NONE
             * `Icon` - ICON
             * `Emoji` - EMOJI
         icon_name_or_emoji (Union[Unset, str]):
         color_name (Union[Unset, ColorName]): * `Red` - RED
@@ -47,29 +47,29 @@
             * `Tan` - TAN
             * `Dark Gray` - DARK_GRAY
             * `Light Brown` - LIGHT_BROWN
             * `Light Gray` - LIGHT_GRAY
     """
 
     duid: str
-    order: str
     hidden: Union[Unset, bool] = UNSET
     public: Union[Unset, bool] = UNSET
+    order: Union[Unset, str] = UNSET
     title: Union[Unset, str] = UNSET
     description: Union[Unset, str] = UNSET
     icon_kind: Union[Unset, IconKind] = UNSET
     icon_name_or_emoji: Union[Unset, str] = UNSET
     color_name: Union[Unset, ColorName] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         duid = self.duid
-        order = self.order
         hidden = self.hidden
         public = self.public
+        order = self.order
         title = self.title
         description = self.description
         icon_kind: Union[Unset, str] = UNSET
         if not isinstance(self.icon_kind, Unset):
             icon_kind = self.icon_kind.value
 
         icon_name_or_emoji = self.icon_name_or_emoji
@@ -78,21 +78,22 @@
             color_name = self.color_name.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "duid": duid,
-                "order": order,
             }
         )
         if hidden is not UNSET:
             field_dict["hidden"] = hidden
         if public is not UNSET:
             field_dict["public"] = public
+        if order is not UNSET:
+            field_dict["order"] = order
         if title is not UNSET:
             field_dict["title"] = title
         if description is not UNSET:
             field_dict["description"] = description
         if icon_kind is not UNSET:
             field_dict["iconKind"] = icon_kind
         if icon_name_or_emoji is not UNSET:
@@ -103,20 +104,20 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         duid = d.pop("duid")
 
-        order = d.pop("order")
-
         hidden = d.pop("hidden", UNSET)
 
         public = d.pop("public", UNSET)
 
+        order = d.pop("order", UNSET)
+
         title = d.pop("title", UNSET)
 
         description = d.pop("description", UNSET)
 
         _icon_kind = d.pop("iconKind", UNSET)
         icon_kind: Union[Unset, IconKind]
         if isinstance(_icon_kind, Unset):
@@ -129,28 +130,28 @@
         _color_name = d.pop("colorName", UNSET)
         color_name: Union[Unset, ColorName]
         if isinstance(_color_name, Unset):
             color_name = UNSET
         else:
             color_name = ColorName(_color_name)
 
-        form_create = cls(
+        form_update = cls(
             duid=duid,
-            order=order,
             hidden=hidden,
             public=public,
+            order=order,
             title=title,
             description=description,
             icon_kind=icon_kind,
             icon_name_or_emoji=icon_name_or_emoji,
             color_name=color_name,
         )
 
-        form_create.additional_properties = d
-        return form_create
+        form_update.additional_properties = d
+        return form_update
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart-tools-0.5.5/dart/generated/models/form_field.py` & `dart_tools-0.5.6/dart/generated/models/form_field.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/form_field_create.py` & `dart_tools-0.5.6/dart/generated/models/form_field_create.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/form_field_update.py` & `dart_tools-0.5.6/dart/generated/models/form_field_update.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/form_update.py` & `dart_tools-0.5.6/dart/generated/models/status_update.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..models.color_name import ColorName
-from ..models.icon_kind import IconKind
+from ..models.status_kind import StatusKind
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="FormUpdate")
+T = TypeVar("T", bound="StatusUpdate")
 
 
 @_attrs_define
-class FormUpdate:
+class StatusUpdate:
     """
     Attributes:
         duid (str):
-        hidden (Union[Unset, bool]):
-        public (Union[Unset, bool]):
+        property_duid (Union[Unset, str]):
+        kind (Union[Unset, StatusKind]): * `Unstarted` - UNSTARTED
+            * `Started` - STARTED
+            * `Blocked` - BLOCKED
+            * `Finished` - FINISHED
+            * `Canceled` - CANCELED
+        locked (Union[Unset, bool]):
         order (Union[Unset, str]):
         title (Union[Unset, str]):
-        description (Union[Unset, str]):
-        icon_kind (Union[Unset, IconKind]): * `None` - NONE
-            * `Icon` - ICON
-            * `Emoji` - EMOJI
-        icon_name_or_emoji (Union[Unset, str]):
         color_name (Union[Unset, ColorName]): * `Red` - RED
             * `Dark Blue` - DARK_BLUE
             * `Dark Orange` - DARK_ORANGE
             * `Dark Green` - DARK_GREEN
             * `Purple` - PURPLE
             * `Dark Teal` - DARK_TEAL
             * `Pink` - PINK
@@ -44,114 +44,109 @@
             * `Light Purple` - LIGHT_PURPLE
             * `Light Orange` - LIGHT_ORANGE
             * `Light Pink` - LIGHT_PINK
             * `Tan` - TAN
             * `Dark Gray` - DARK_GRAY
             * `Light Brown` - LIGHT_BROWN
             * `Light Gray` - LIGHT_GRAY
+        description (Union[Unset, str]):
     """
 
     duid: str
-    hidden: Union[Unset, bool] = UNSET
-    public: Union[Unset, bool] = UNSET
+    property_duid: Union[Unset, str] = UNSET
+    kind: Union[Unset, StatusKind] = UNSET
+    locked: Union[Unset, bool] = UNSET
     order: Union[Unset, str] = UNSET
     title: Union[Unset, str] = UNSET
-    description: Union[Unset, str] = UNSET
-    icon_kind: Union[Unset, IconKind] = UNSET
-    icon_name_or_emoji: Union[Unset, str] = UNSET
     color_name: Union[Unset, ColorName] = UNSET
+    description: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         duid = self.duid
-        hidden = self.hidden
-        public = self.public
+        property_duid = self.property_duid
+        kind: Union[Unset, str] = UNSET
+        if not isinstance(self.kind, Unset):
+            kind = self.kind.value
+
+        locked = self.locked
         order = self.order
         title = self.title
-        description = self.description
-        icon_kind: Union[Unset, str] = UNSET
-        if not isinstance(self.icon_kind, Unset):
-            icon_kind = self.icon_kind.value
-
-        icon_name_or_emoji = self.icon_name_or_emoji
         color_name: Union[Unset, str] = UNSET
         if not isinstance(self.color_name, Unset):
             color_name = self.color_name.value
 
+        description = self.description
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "duid": duid,
             }
         )
-        if hidden is not UNSET:
-            field_dict["hidden"] = hidden
-        if public is not UNSET:
-            field_dict["public"] = public
+        if property_duid is not UNSET:
+            field_dict["propertyDuid"] = property_duid
+        if kind is not UNSET:
+            field_dict["kind"] = kind
+        if locked is not UNSET:
+            field_dict["locked"] = locked
         if order is not UNSET:
             field_dict["order"] = order
         if title is not UNSET:
             field_dict["title"] = title
-        if description is not UNSET:
-            field_dict["description"] = description
-        if icon_kind is not UNSET:
-            field_dict["iconKind"] = icon_kind
-        if icon_name_or_emoji is not UNSET:
-            field_dict["iconNameOrEmoji"] = icon_name_or_emoji
         if color_name is not UNSET:
             field_dict["colorName"] = color_name
+        if description is not UNSET:
+            field_dict["description"] = description
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         duid = d.pop("duid")
 
-        hidden = d.pop("hidden", UNSET)
+        property_duid = d.pop("propertyDuid", UNSET)
+
+        _kind = d.pop("kind", UNSET)
+        kind: Union[Unset, StatusKind]
+        if isinstance(_kind, Unset):
+            kind = UNSET
+        else:
+            kind = StatusKind(_kind)
 
-        public = d.pop("public", UNSET)
+        locked = d.pop("locked", UNSET)
 
         order = d.pop("order", UNSET)
 
         title = d.pop("title", UNSET)
 
-        description = d.pop("description", UNSET)
-
-        _icon_kind = d.pop("iconKind", UNSET)
-        icon_kind: Union[Unset, IconKind]
-        if isinstance(_icon_kind, Unset):
-            icon_kind = UNSET
-        else:
-            icon_kind = IconKind(_icon_kind)
-
-        icon_name_or_emoji = d.pop("iconNameOrEmoji", UNSET)
-
         _color_name = d.pop("colorName", UNSET)
         color_name: Union[Unset, ColorName]
         if isinstance(_color_name, Unset):
             color_name = UNSET
         else:
             color_name = ColorName(_color_name)
 
-        form_update = cls(
+        description = d.pop("description", UNSET)
+
+        status_update = cls(
             duid=duid,
-            hidden=hidden,
-            public=public,
+            property_duid=property_duid,
+            kind=kind,
+            locked=locked,
             order=order,
             title=title,
-            description=description,
-            icon_kind=icon_kind,
-            icon_name_or_emoji=icon_name_or_emoji,
             color_name=color_name,
+            description=description,
         )
 
-        form_update.additional_properties = d
-        return form_update
+        status_update.additional_properties = d
+        return status_update
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart-tools-0.5.5/dart/generated/models/github_integration.py` & `dart_tools-0.5.6/dart/generated/models/github_integration.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/google_data.py` & `dart_tools-0.5.6/dart/generated/models/google_data.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/layout.py` & `dart_tools-0.5.6/dart/generated/models/layout.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/layout_config.py` & `dart_tools-0.5.6/dart/generated/models/layout_config.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/layout_create.py` & `dart_tools-0.5.6/dart/generated/models/layout_create.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/layout_kind_config_map.py` & `dart_tools-0.5.6/dart/generated/models/layout_kind_config_map.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/layout_update.py` & `dart_tools-0.5.6/dart/generated/models/layout_update.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/models_response.py` & `dart_tools-0.5.6/dart/generated/models/models_response.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/notification.py` & `dart_tools-0.5.6/dart/generated/models/notification.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/notification_update.py` & `dart_tools-0.5.6/dart/generated/models/notification_update.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/notion_integration.py` & `dart_tools-0.5.6/dart/generated/models/notion_integration.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/operation.py` & `dart_tools-0.5.6/dart/generated/models/operation.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/operation_model_kind.py` & `dart_tools-0.5.6/dart/generated/models/operation_model_kind.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/option.py` & `dart_tools-0.5.6/dart/generated/models/option.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/option_create.py` & `dart_tools-0.5.6/dart/generated/models/option_create.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/option_update.py` & `dart_tools-0.5.6/dart/generated/models/option_update.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/paginated_attachment_list.py` & `dart_tools-0.5.6/dart/generated/models/paginated_attachment_list.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/paginated_comment_list.py` & `dart_tools-0.5.6/dart/generated/models/paginated_comment_list.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/paginated_comment_reaction_list.py` & `dart_tools-0.5.6/dart/generated/models/paginated_comment_reaction_list.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/paginated_dartboard_list.py` & `dart_tools-0.5.6/dart/generated/models/paginated_dartboard_list.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/paginated_doc_list.py` & `dart_tools-0.5.6/dart/generated/models/paginated_doc_list.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/paginated_folder_list.py` & `dart_tools-0.5.6/dart/generated/models/paginated_folder_list.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/paginated_form_field_list.py` & `dart_tools-0.5.6/dart/generated/models/paginated_form_field_list.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/paginated_form_list.py` & `dart_tools-0.5.6/dart/generated/models/paginated_form_list.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/paginated_layout_list.py` & `dart_tools-0.5.6/dart/generated/models/paginated_layout_list.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/paginated_option_list.py` & `dart_tools-0.5.6/dart/generated/models/paginated_option_list.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/paginated_property_list.py` & `dart_tools-0.5.6/dart/generated/models/paginated_property_list.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/paginated_relationship_kind_list.py` & `dart_tools-0.5.6/dart/generated/models/paginated_relationship_kind_list.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/paginated_relationship_list.py` & `dart_tools-0.5.6/dart/generated/models/paginated_relationship_list.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/paginated_space_list.py` & `dart_tools-0.5.6/dart/generated/models/paginated_space_list.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/paginated_status_list.py` & `dart_tools-0.5.6/dart/generated/models/paginated_status_list.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/paginated_task_doc_relationship_list.py` & `dart_tools-0.5.6/dart/generated/models/paginated_task_doc_relationship_list.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/paginated_task_link_list.py` & `dart_tools-0.5.6/dart/generated/models/paginated_task_link_list.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/paginated_task_list.py` & `dart_tools-0.5.6/dart/generated/models/paginated_task_list.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/paginated_tenant_list.py` & `dart_tools-0.5.6/dart/generated/models/paginated_tenant_list.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/paginated_user_dartboard_layout_list.py` & `dart_tools-0.5.6/dart/generated/models/paginated_user_dartboard_layout_list.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/paginated_user_list.py` & `dart_tools-0.5.6/dart/generated/models/paginated_user_list.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/paginated_view_list.py` & `dart_tools-0.5.6/dart/generated/models/paginated_view_list.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/properties_list_kind.py` & `dart_tools-0.5.6/dart/generated/models/properties_list_kind.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/property_.py` & `dart_tools-0.5.6/dart/generated/models/property_.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/property_create.py` & `dart_tools-0.5.6/dart/generated/models/property_create.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/property_kind.py` & `dart_tools-0.5.6/dart/generated/models/property_kind.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/property_update.py` & `dart_tools-0.5.6/dart/generated/models/property_update.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/relationship.py` & `dart_tools-0.5.6/dart/generated/models/relationship.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/relationship_create.py` & `dart_tools-0.5.6/dart/generated/models/relationship_create.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/relationship_kind.py` & `dart_tools-0.5.6/dart/generated/models/relationship_kind.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/relationship_kind_create.py` & `dart_tools-0.5.6/dart/generated/models/relationship_kind_create.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/relationship_kind_update.py` & `dart_tools-0.5.6/dart/generated/models/relationship_kind_update.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/request_body.py` & `dart_tools-0.5.6/dart/generated/models/request_body.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/response_body.py` & `dart_tools-0.5.6/dart/generated/models/response_body.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/slack_integration.py` & `dart_tools-0.5.6/dart/generated/models/slack_integration.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/sort.py` & `dart_tools-0.5.6/dart/generated/models/sort.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/space.py` & `dart_tools-0.5.6/dart/generated/models/space.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/space_create.py` & `dart_tools-0.5.6/dart/generated/models/space_create.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/space_update.py` & `dart_tools-0.5.6/dart/generated/models/space_update.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/status.py` & `dart_tools-0.5.6/dart/generated/models/status.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/status_create.py` & `dart_tools-0.5.6/dart/generated/models/status_create.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/status_update.py` & `dart_tools-0.5.6/dart/generated/models/task_link_update.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,152 +1,119 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
-from ..models.color_name import ColorName
-from ..models.status_kind import StatusKind
+from ..models.task_link_kind import TaskLinkKind
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="StatusUpdate")
+T = TypeVar("T", bound="TaskLinkUpdate")
 
 
 @_attrs_define
-class StatusUpdate:
+class TaskLinkUpdate:
     """
     Attributes:
         duid (str):
-        property_duid (Union[Unset, str]):
-        kind (Union[Unset, StatusKind]): * `Unstarted` - UNSTARTED
-            * `Started` - STARTED
-            * `Blocked` - BLOCKED
-            * `Finished` - FINISHED
-            * `Canceled` - CANCELED
-        locked (Union[Unset, bool]):
+        task_duid (Union[Unset, str]):
         order (Union[Unset, str]):
-        title (Union[Unset, str]):
-        color_name (Union[Unset, ColorName]): * `Red` - RED
-            * `Dark Blue` - DARK_BLUE
-            * `Dark Orange` - DARK_ORANGE
-            * `Dark Green` - DARK_GREEN
-            * `Purple` - PURPLE
-            * `Dark Teal` - DARK_TEAL
-            * `Pink` - PINK
-            * `Orange` - ORANGE
-            * `Green` - GREEN
-            * `Yellow` - YELLOW
-            * `Brown` - BROWN
-            * `Dark Red` - DARK_RED
-            * `Flat Green` - FLAT_GREEN
-            * `Red Orange` - RED_ORANGE
-            * `Teal` - TEAL
-            * `Light Green` - LIGHT_GREEN
-            * `Light Blue` - LIGHT_BLUE
-            * `Light Purple` - LIGHT_PURPLE
-            * `Light Orange` - LIGHT_ORANGE
-            * `Light Pink` - LIGHT_PINK
-            * `Tan` - TAN
-            * `Dark Gray` - DARK_GRAY
-            * `Light Brown` - LIGHT_BROWN
-            * `Light Gray` - LIGHT_GRAY
-        description (Union[Unset, str]):
+        kind (Union[Unset, TaskLinkKind]): * `Standard` - STANDARD
+            * `Source From Template` - SOURCE_FROM_TEMPLATE
+            * `Source From Third Party` - SOURCE_FROM_THIRD_PARTY
+            * `GitHub Branch` - GITHUB_BRANCH
+            * `GitHub Pull Request` - GITHUB_PULL_REQUEST
+            * `GitHub Expansion` - GITHUB_EXPANSION
+            * `Notion Link` - NOTION_LINK
+            * `Notion Document` - NOTION_DOCUMENT
+            * `Notion Document Doesnt Exist` - NOTION_DOCUMENT_DOESNT_EXIST
+            * `Notion Document Parse Failed` - NOTION_DOCUMENT_PARSE_FAILED
+            * `Notion Expansion` - NOTION_EXPANSION
+            * `Slack Expansion` - SLACK_EXPANSION
+        url (Union[Unset, str]):
+        title (Union[Unset, None, str]):
+        icon_url (Union[Unset, None, str]):
     """
 
     duid: str
-    property_duid: Union[Unset, str] = UNSET
-    kind: Union[Unset, StatusKind] = UNSET
-    locked: Union[Unset, bool] = UNSET
+    task_duid: Union[Unset, str] = UNSET
     order: Union[Unset, str] = UNSET
-    title: Union[Unset, str] = UNSET
-    color_name: Union[Unset, ColorName] = UNSET
-    description: Union[Unset, str] = UNSET
+    kind: Union[Unset, TaskLinkKind] = UNSET
+    url: Union[Unset, str] = UNSET
+    title: Union[Unset, None, str] = UNSET
+    icon_url: Union[Unset, None, str] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         duid = self.duid
-        property_duid = self.property_duid
+        task_duid = self.task_duid
+        order = self.order
         kind: Union[Unset, str] = UNSET
         if not isinstance(self.kind, Unset):
             kind = self.kind.value
 
-        locked = self.locked
-        order = self.order
+        url = self.url
         title = self.title
-        color_name: Union[Unset, str] = UNSET
-        if not isinstance(self.color_name, Unset):
-            color_name = self.color_name.value
-
-        description = self.description
+        icon_url = self.icon_url
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "duid": duid,
             }
         )
-        if property_duid is not UNSET:
-            field_dict["propertyDuid"] = property_duid
-        if kind is not UNSET:
-            field_dict["kind"] = kind
-        if locked is not UNSET:
-            field_dict["locked"] = locked
+        if task_duid is not UNSET:
+            field_dict["taskDuid"] = task_duid
         if order is not UNSET:
             field_dict["order"] = order
+        if kind is not UNSET:
+            field_dict["kind"] = kind
+        if url is not UNSET:
+            field_dict["url"] = url
         if title is not UNSET:
             field_dict["title"] = title
-        if color_name is not UNSET:
-            field_dict["colorName"] = color_name
-        if description is not UNSET:
-            field_dict["description"] = description
+        if icon_url is not UNSET:
+            field_dict["iconUrl"] = icon_url
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         duid = d.pop("duid")
 
-        property_duid = d.pop("propertyDuid", UNSET)
+        task_duid = d.pop("taskDuid", UNSET)
+
+        order = d.pop("order", UNSET)
 
         _kind = d.pop("kind", UNSET)
-        kind: Union[Unset, StatusKind]
+        kind: Union[Unset, TaskLinkKind]
         if isinstance(_kind, Unset):
             kind = UNSET
         else:
-            kind = StatusKind(_kind)
-
-        locked = d.pop("locked", UNSET)
+            kind = TaskLinkKind(_kind)
 
-        order = d.pop("order", UNSET)
+        url = d.pop("url", UNSET)
 
         title = d.pop("title", UNSET)
 
-        _color_name = d.pop("colorName", UNSET)
-        color_name: Union[Unset, ColorName]
-        if isinstance(_color_name, Unset):
-            color_name = UNSET
-        else:
-            color_name = ColorName(_color_name)
+        icon_url = d.pop("iconUrl", UNSET)
 
-        description = d.pop("description", UNSET)
-
-        status_update = cls(
+        task_link_update = cls(
             duid=duid,
-            property_duid=property_duid,
-            kind=kind,
-            locked=locked,
+            task_duid=task_duid,
             order=order,
+            kind=kind,
+            url=url,
             title=title,
-            color_name=color_name,
-            description=description,
+            icon_url=icon_url,
         )
 
-        status_update.additional_properties = d
-        return status_update
+        task_link_update.additional_properties = d
+        return task_link_update
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart-tools-0.5.5/dart/generated/models/task.py` & `dart_tools-0.5.6/dart/generated/models/task.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/task_create.py` & `dart_tools-0.5.6/dart/generated/models/task_update.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,25 +6,22 @@
 from dateutil.parser import isoparse
 
 from ..models.priority import Priority
 from ..models.recommendation_status import RecommendationStatus
 from ..models.task_source_type import TaskSourceType
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="TaskCreate")
+T = TypeVar("T", bound="TaskUpdate")
 
 
 @_attrs_define
-class TaskCreate:
+class TaskUpdate:
     """
     Attributes:
         duid (str):
-        dartboard_duid (str):
-        order (str):
-        status_duid (str):
         source_type (Union[Unset, TaskSourceType]): * `Unknown` - UNKNOWN
             * `Import` - IMPORT
             * `Onboarding` - ONBOARDING
             * `Recommendation` - RECOMMENDATION
             * `Recurrence` - RECURRENCE
             * `Template` - TEMPLATE
             * `ChatGPT` - CHAT_GPT
@@ -48,16 +45,20 @@
         source_form_duid (Union[Unset, None, str]):
         created_by_duid (Union[Unset, None, str]):
         updated_by_duid (Union[Unset, None, str]):
         drafter_duid (Union[Unset, None, str]):
         in_trash (Union[Unset, bool]):
         recommendation_status (Union[Unset, None, RecommendationStatus]): * `Accepted` - ACCEPTED
             * `Declined` - DECLINED
+        dartboard_duid (Union[Unset, str]):
+        order (Union[Unset, str]):
         title (Union[Unset, str]):
         description (Union[Unset, Any]):
+        description_markdown (Union[Unset, str]):
+        status_duid (Union[Unset, str]):
         assigned_to_ai (Union[Unset, bool]):
         assignee_duids (Union[Unset, List[str]]):
         subscriber_duids (Union[Unset, List[str]]):
         tag_duids (Union[Unset, List[str]]):
         attachment_duids (Union[Unset, List[str]]):
         priority (Union[Unset, None, Priority]): * `Critical` - CRITICAL
             * `High` - HIGH
@@ -69,26 +70,27 @@
         remind_at (Union[Unset, None, datetime.datetime]):
         recurrence (Union[Unset, Any]):
         recurrs_next_at (Union[Unset, None, datetime.datetime]):
         properties (Union[Unset, Any]):
     """
 
     duid: str
-    dartboard_duid: str
-    order: str
-    status_duid: str
     source_type: Union[Unset, TaskSourceType] = TaskSourceType.UNKNOWN
     source_form_duid: Union[Unset, None, str] = UNSET
     created_by_duid: Union[Unset, None, str] = UNSET
     updated_by_duid: Union[Unset, None, str] = UNSET
     drafter_duid: Union[Unset, None, str] = UNSET
     in_trash: Union[Unset, bool] = UNSET
     recommendation_status: Union[Unset, None, RecommendationStatus] = UNSET
+    dartboard_duid: Union[Unset, str] = UNSET
+    order: Union[Unset, str] = UNSET
     title: Union[Unset, str] = UNSET
     description: Union[Unset, Any] = UNSET
+    description_markdown: Union[Unset, str] = UNSET
+    status_duid: Union[Unset, str] = UNSET
     assigned_to_ai: Union[Unset, bool] = UNSET
     assignee_duids: Union[Unset, List[str]] = UNSET
     subscriber_duids: Union[Unset, List[str]] = UNSET
     tag_duids: Union[Unset, List[str]] = UNSET
     attachment_duids: Union[Unset, List[str]] = UNSET
     priority: Union[Unset, None, Priority] = UNSET
     size: Union[Unset, None, int] = UNSET
@@ -98,32 +100,33 @@
     recurrence: Union[Unset, Any] = UNSET
     recurrs_next_at: Union[Unset, None, datetime.datetime] = UNSET
     properties: Union[Unset, Any] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         duid = self.duid
-        dartboard_duid = self.dartboard_duid
-        order = self.order
-        status_duid = self.status_duid
         source_type: Union[Unset, str] = UNSET
         if not isinstance(self.source_type, Unset):
             source_type = self.source_type.value
 
         source_form_duid = self.source_form_duid
         created_by_duid = self.created_by_duid
         updated_by_duid = self.updated_by_duid
         drafter_duid = self.drafter_duid
         in_trash = self.in_trash
         recommendation_status: Union[Unset, None, str] = UNSET
         if not isinstance(self.recommendation_status, Unset):
             recommendation_status = self.recommendation_status.value if self.recommendation_status else None
 
+        dartboard_duid = self.dartboard_duid
+        order = self.order
         title = self.title
         description = self.description
+        description_markdown = self.description_markdown
+        status_duid = self.status_duid
         assigned_to_ai = self.assigned_to_ai
         assignee_duids: Union[Unset, List[str]] = UNSET
         if not isinstance(self.assignee_duids, Unset):
             assignee_duids = self.assignee_duids
 
         subscriber_duids: Union[Unset, List[str]] = UNSET
         if not isinstance(self.subscriber_duids, Unset):
@@ -162,17 +165,14 @@
         properties = self.properties
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "duid": duid,
-                "dartboardDuid": dartboard_duid,
-                "order": order,
-                "statusDuid": status_duid,
             }
         )
         if source_type is not UNSET:
             field_dict["sourceType"] = source_type
         if source_form_duid is not UNSET:
             field_dict["sourceFormDuid"] = source_form_duid
         if created_by_duid is not UNSET:
@@ -181,18 +181,26 @@
             field_dict["updatedByDuid"] = updated_by_duid
         if drafter_duid is not UNSET:
             field_dict["drafterDuid"] = drafter_duid
         if in_trash is not UNSET:
             field_dict["inTrash"] = in_trash
         if recommendation_status is not UNSET:
             field_dict["recommendationStatus"] = recommendation_status
+        if dartboard_duid is not UNSET:
+            field_dict["dartboardDuid"] = dartboard_duid
+        if order is not UNSET:
+            field_dict["order"] = order
         if title is not UNSET:
             field_dict["title"] = title
         if description is not UNSET:
             field_dict["description"] = description
+        if description_markdown is not UNSET:
+            field_dict["descriptionMarkdown"] = description_markdown
+        if status_duid is not UNSET:
+            field_dict["statusDuid"] = status_duid
         if assigned_to_ai is not UNSET:
             field_dict["assignedToAi"] = assigned_to_ai
         if assignee_duids is not UNSET:
             field_dict["assigneeDuids"] = assignee_duids
         if subscriber_duids is not UNSET:
             field_dict["subscriberDuids"] = subscriber_duids
         if tag_duids is not UNSET:
@@ -219,20 +227,14 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         duid = d.pop("duid")
 
-        dartboard_duid = d.pop("dartboardDuid")
-
-        order = d.pop("order")
-
-        status_duid = d.pop("statusDuid")
-
         _source_type = d.pop("sourceType", UNSET)
         source_type: Union[Unset, TaskSourceType]
         if isinstance(_source_type, Unset):
             source_type = UNSET
         else:
             source_type = TaskSourceType(_source_type)
 
@@ -251,18 +253,26 @@
         if _recommendation_status is None:
             recommendation_status = None
         elif isinstance(_recommendation_status, Unset):
             recommendation_status = UNSET
         else:
             recommendation_status = RecommendationStatus(_recommendation_status)
 
+        dartboard_duid = d.pop("dartboardDuid", UNSET)
+
+        order = d.pop("order", UNSET)
+
         title = d.pop("title", UNSET)
 
         description = d.pop("description", UNSET)
 
+        description_markdown = d.pop("descriptionMarkdown", UNSET)
+
+        status_duid = d.pop("statusDuid", UNSET)
+
         assigned_to_ai = d.pop("assignedToAi", UNSET)
 
         assignee_duids = cast(List[str], d.pop("assigneeDuids", UNSET))
 
         subscriber_duids = cast(List[str], d.pop("subscriberDuids", UNSET))
 
         tag_duids = cast(List[str], d.pop("tagDuids", UNSET))
@@ -316,28 +326,29 @@
         elif isinstance(_recurrs_next_at, Unset):
             recurrs_next_at = UNSET
         else:
             recurrs_next_at = isoparse(_recurrs_next_at)
 
         properties = d.pop("properties", UNSET)
 
-        task_create = cls(
+        task_update = cls(
             duid=duid,
-            dartboard_duid=dartboard_duid,
-            order=order,
-            status_duid=status_duid,
             source_type=source_type,
             source_form_duid=source_form_duid,
             created_by_duid=created_by_duid,
             updated_by_duid=updated_by_duid,
             drafter_duid=drafter_duid,
             in_trash=in_trash,
             recommendation_status=recommendation_status,
+            dartboard_duid=dartboard_duid,
+            order=order,
             title=title,
             description=description,
+            description_markdown=description_markdown,
+            status_duid=status_duid,
             assigned_to_ai=assigned_to_ai,
             assignee_duids=assignee_duids,
             subscriber_duids=subscriber_duids,
             tag_duids=tag_duids,
             attachment_duids=attachment_duids,
             priority=priority,
             size=size,
@@ -345,16 +356,16 @@
             due_at=due_at,
             remind_at=remind_at,
             recurrence=recurrence,
             recurrs_next_at=recurrs_next_at,
             properties=properties,
         )
 
-        task_create.additional_properties = d
-        return task_create
+        task_update.additional_properties = d
+        return task_update
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart-tools-0.5.5/dart/generated/models/task_doc_relationship.py` & `dart_tools-0.5.6/dart/generated/models/task_doc_relationship.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/task_doc_relationship_create.py` & `dart_tools-0.5.6/dart/generated/models/task_doc_relationship_create.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/task_link.py` & `dart_tools-0.5.6/dart/generated/models/task_link.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/task_link_create.py` & `dart_tools-0.5.6/dart/generated/models/task_link_create.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/task_link_kind.py` & `dart_tools-0.5.6/dart/generated/models/task_link_kind.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/task_notion_document.py` & `dart_tools-0.5.6/dart/generated/models/task_notion_document.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/task_notion_document_block_children_map.py` & `dart_tools-0.5.6/dart/generated/models/task_notion_document_block_children_map.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/task_notion_document_block_map.py` & `dart_tools-0.5.6/dart/generated/models/task_notion_document_block_map.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/task_notion_document_page_map.py` & `dart_tools-0.5.6/dart/generated/models/task_notion_document_page_map.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/task_properties.py` & `dart_tools-0.5.6/dart/generated/models/task_properties.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/task_source_type.py` & `dart_tools-0.5.6/dart/generated/models/task_source_type.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/task_update.py` & `dart_tools-0.5.6/dart/generated/models/task_create.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 from dateutil.parser import isoparse
 
 from ..models.priority import Priority
 from ..models.recommendation_status import RecommendationStatus
 from ..models.task_source_type import TaskSourceType
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="TaskUpdate")
+T = TypeVar("T", bound="TaskCreate")
 
 
 @_attrs_define
-class TaskUpdate:
+class TaskCreate:
     """
     Attributes:
         duid (str):
         source_type (Union[Unset, TaskSourceType]): * `Unknown` - UNKNOWN
             * `Import` - IMPORT
             * `Onboarding` - ONBOARDING
             * `Recommendation` - RECOMMENDATION
@@ -49,14 +49,15 @@
         in_trash (Union[Unset, bool]):
         recommendation_status (Union[Unset, None, RecommendationStatus]): * `Accepted` - ACCEPTED
             * `Declined` - DECLINED
         dartboard_duid (Union[Unset, str]):
         order (Union[Unset, str]):
         title (Union[Unset, str]):
         description (Union[Unset, Any]):
+        description_markdown (Union[Unset, str]):
         status_duid (Union[Unset, str]):
         assigned_to_ai (Union[Unset, bool]):
         assignee_duids (Union[Unset, List[str]]):
         subscriber_duids (Union[Unset, List[str]]):
         tag_duids (Union[Unset, List[str]]):
         attachment_duids (Union[Unset, List[str]]):
         priority (Union[Unset, None, Priority]): * `Critical` - CRITICAL
@@ -80,14 +81,15 @@
     drafter_duid: Union[Unset, None, str] = UNSET
     in_trash: Union[Unset, bool] = UNSET
     recommendation_status: Union[Unset, None, RecommendationStatus] = UNSET
     dartboard_duid: Union[Unset, str] = UNSET
     order: Union[Unset, str] = UNSET
     title: Union[Unset, str] = UNSET
     description: Union[Unset, Any] = UNSET
+    description_markdown: Union[Unset, str] = UNSET
     status_duid: Union[Unset, str] = UNSET
     assigned_to_ai: Union[Unset, bool] = UNSET
     assignee_duids: Union[Unset, List[str]] = UNSET
     subscriber_duids: Union[Unset, List[str]] = UNSET
     tag_duids: Union[Unset, List[str]] = UNSET
     attachment_duids: Union[Unset, List[str]] = UNSET
     priority: Union[Unset, None, Priority] = UNSET
@@ -115,14 +117,15 @@
         if not isinstance(self.recommendation_status, Unset):
             recommendation_status = self.recommendation_status.value if self.recommendation_status else None
 
         dartboard_duid = self.dartboard_duid
         order = self.order
         title = self.title
         description = self.description
+        description_markdown = self.description_markdown
         status_duid = self.status_duid
         assigned_to_ai = self.assigned_to_ai
         assignee_duids: Union[Unset, List[str]] = UNSET
         if not isinstance(self.assignee_duids, Unset):
             assignee_duids = self.assignee_duids
 
         subscriber_duids: Union[Unset, List[str]] = UNSET
@@ -186,14 +189,16 @@
             field_dict["dartboardDuid"] = dartboard_duid
         if order is not UNSET:
             field_dict["order"] = order
         if title is not UNSET:
             field_dict["title"] = title
         if description is not UNSET:
             field_dict["description"] = description
+        if description_markdown is not UNSET:
+            field_dict["descriptionMarkdown"] = description_markdown
         if status_duid is not UNSET:
             field_dict["statusDuid"] = status_duid
         if assigned_to_ai is not UNSET:
             field_dict["assignedToAi"] = assigned_to_ai
         if assignee_duids is not UNSET:
             field_dict["assigneeDuids"] = assignee_duids
         if subscriber_duids is not UNSET:
@@ -256,14 +261,16 @@
 
         order = d.pop("order", UNSET)
 
         title = d.pop("title", UNSET)
 
         description = d.pop("description", UNSET)
 
+        description_markdown = d.pop("descriptionMarkdown", UNSET)
+
         status_duid = d.pop("statusDuid", UNSET)
 
         assigned_to_ai = d.pop("assignedToAi", UNSET)
 
         assignee_duids = cast(List[str], d.pop("assigneeDuids", UNSET))
 
         subscriber_duids = cast(List[str], d.pop("subscriberDuids", UNSET))
@@ -319,27 +326,28 @@
         elif isinstance(_recurrs_next_at, Unset):
             recurrs_next_at = UNSET
         else:
             recurrs_next_at = isoparse(_recurrs_next_at)
 
         properties = d.pop("properties", UNSET)
 
-        task_update = cls(
+        task_create = cls(
             duid=duid,
             source_type=source_type,
             source_form_duid=source_form_duid,
             created_by_duid=created_by_duid,
             updated_by_duid=updated_by_duid,
             drafter_duid=drafter_duid,
             in_trash=in_trash,
             recommendation_status=recommendation_status,
             dartboard_duid=dartboard_duid,
             order=order,
             title=title,
             description=description,
+            description_markdown=description_markdown,
             status_duid=status_duid,
             assigned_to_ai=assigned_to_ai,
             assignee_duids=assignee_duids,
             subscriber_duids=subscriber_duids,
             tag_duids=tag_duids,
             attachment_duids=attachment_duids,
             priority=priority,
@@ -348,16 +356,16 @@
             due_at=due_at,
             remind_at=remind_at,
             recurrence=recurrence,
             recurrs_next_at=recurrs_next_at,
             properties=properties,
         )
 
-        task_update.additional_properties = d
-        return task_update
+        task_create.additional_properties = d
+        return task_create
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `dart-tools-0.5.5/dart/generated/models/tenant.py` & `dart_tools-0.5.6/dart/generated/models/tenant.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 if TYPE_CHECKING:
     from ..models.discord_integration import DiscordIntegration
     from ..models.github_integration import GithubIntegration
     from ..models.notion_integration import NotionIntegration
     from ..models.slack_integration import SlackIntegration
     from ..models.yc_integration import YcIntegration
+    from ..models.zapier_integration import ZapierIntegration
 
 
 T = TypeVar("T", bound="Tenant")
 
 
 @_attrs_define
 class Tenant:
@@ -36,14 +37,15 @@
         image_url (Optional[str]):
         webhook_url (Optional[str]):
         yc (Optional[YcIntegration]):
         notion_integration (Optional[NotionIntegration]):
         slack_integration (Optional[SlackIntegration]):
         discord_integration (Optional[DiscordIntegration]):
         github_integration (Optional[GithubIntegration]):
+        zapier_integration (Optional[ZapierIntegration]):
     """
 
     duid: str
     is_dart: bool
     name: str
     timezone: str
     subscription: Subscription
@@ -57,14 +59,15 @@
     image_url: Optional[str]
     webhook_url: Optional[str]
     yc: Optional["YcIntegration"]
     notion_integration: Optional["NotionIntegration"]
     slack_integration: Optional["SlackIntegration"]
     discord_integration: Optional["DiscordIntegration"]
     github_integration: Optional["GithubIntegration"]
+    zapier_integration: Optional["ZapierIntegration"]
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         duid = self.duid
         is_dart = self.is_dart
         name = self.name
         timezone = self.timezone
@@ -85,14 +88,16 @@
 
         slack_integration = self.slack_integration.to_dict() if self.slack_integration else None
 
         discord_integration = self.discord_integration.to_dict() if self.discord_integration else None
 
         github_integration = self.github_integration.to_dict() if self.github_integration else None
 
+        zapier_integration = self.zapier_integration.to_dict() if self.zapier_integration else None
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "duid": duid,
                 "isDart": is_dart,
                 "name": name,
@@ -108,26 +113,28 @@
                 "imageUrl": image_url,
                 "webhookUrl": webhook_url,
                 "yc": yc,
                 "notionIntegration": notion_integration,
                 "slackIntegration": slack_integration,
                 "discordIntegration": discord_integration,
                 "githubIntegration": github_integration,
+                "zapierIntegration": zapier_integration,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.discord_integration import DiscordIntegration
         from ..models.github_integration import GithubIntegration
         from ..models.notion_integration import NotionIntegration
         from ..models.slack_integration import SlackIntegration
         from ..models.yc_integration import YcIntegration
+        from ..models.zapier_integration import ZapierIntegration
 
         d = src_dict.copy()
         duid = d.pop("duid")
 
         is_dart = d.pop("isDart")
 
         name = d.pop("name")
@@ -185,14 +192,21 @@
         _github_integration = d.pop("githubIntegration")
         github_integration: Optional[GithubIntegration]
         if _github_integration is None:
             github_integration = None
         else:
             github_integration = GithubIntegration.from_dict(_github_integration)
 
+        _zapier_integration = d.pop("zapierIntegration")
+        zapier_integration: Optional[ZapierIntegration]
+        if _zapier_integration is None:
+            zapier_integration = None
+        else:
+            zapier_integration = ZapierIntegration.from_dict(_zapier_integration)
+
         tenant = cls(
             duid=duid,
             is_dart=is_dart,
             name=name,
             timezone=timezone,
             subscription=subscription,
             entitlement_overrides=entitlement_overrides,
@@ -205,14 +219,15 @@
             image_url=image_url,
             webhook_url=webhook_url,
             yc=yc,
             notion_integration=notion_integration,
             slack_integration=slack_integration,
             discord_integration=discord_integration,
             github_integration=github_integration,
+            zapier_integration=zapier_integration,
         )
 
         tenant.additional_properties = d
         return tenant
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `dart-tools-0.5.5/dart/generated/models/tenant_update.py` & `dart_tools-0.5.6/dart/generated/models/tenant_update.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/transaction.py` & `dart_tools-0.5.6/dart/generated/models/transaction.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/transaction_kind.py` & `dart_tools-0.5.6/dart/generated/models/transaction_kind.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/transaction_response.py` & `dart_tools-0.5.6/dart/generated/models/transaction_response.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/user.py` & `dart_tools-0.5.6/dart/generated/models/user.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/user_dartboard_layout.py` & `dart_tools-0.5.6/dart/generated/models/user_dartboard_layout.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/user_dartboard_layout_create.py` & `dart_tools-0.5.6/dart/generated/models/user_dartboard_layout_create.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/user_data_entity_retrieve_entity_kind.py` & `dart_tools-0.5.6/dart/generated/models/user_data_entity_retrieve_entity_kind.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/validation_error_response.py` & `dart_tools-0.5.6/dart/generated/models/validation_error_response.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/validation_error_response_items.py` & `dart_tools-0.5.6/dart/generated/models/validation_error_response_items.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/models/view.py` & `dart_tools-0.5.6/dart/generated/models/view.py`

 * *Files 15% similar despite different names*

```diff
@@ -51,14 +51,16 @@
             * `Light Pink` - LIGHT_PINK
             * `Tan` - TAN
             * `Dark Gray` - DARK_GRAY
             * `Light Brown` - LIGHT_BROWN
             * `Light Gray` - LIGHT_GRAY
         layout_duid (str):
         favorited_by_user_duids (List[str]):
+        always_shown_property_duids (List[str]):
+        always_hidden_property_duids (List[str]):
         updated_by_client_duid (Union[Unset, None, str]):
     """
 
     duid: str
     kind: ViewKind
     accessible_by_team: bool
     accessible_by_user_duids: List[str]
@@ -66,14 +68,16 @@
     title: str
     description: str
     icon_kind: IconKind
     icon_name_or_emoji: str
     color_name: ColorName
     layout_duid: str
     favorited_by_user_duids: List[str]
+    always_shown_property_duids: List[str]
+    always_hidden_property_duids: List[str]
     updated_by_client_duid: Union[Unset, None, str] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         duid = self.duid
         kind = self.kind.value
 
@@ -87,14 +91,18 @@
 
         icon_name_or_emoji = self.icon_name_or_emoji
         color_name = self.color_name.value
 
         layout_duid = self.layout_duid
         favorited_by_user_duids = self.favorited_by_user_duids
 
+        always_shown_property_duids = self.always_shown_property_duids
+
+        always_hidden_property_duids = self.always_hidden_property_duids
+
         updated_by_client_duid = self.updated_by_client_duid
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "duid": duid,
@@ -105,14 +113,16 @@
                 "title": title,
                 "description": description,
                 "iconKind": icon_kind,
                 "iconNameOrEmoji": icon_name_or_emoji,
                 "colorName": color_name,
                 "layoutDuid": layout_duid,
                 "favoritedByUserDuids": favorited_by_user_duids,
+                "alwaysShownPropertyDuids": always_shown_property_duids,
+                "alwaysHiddenPropertyDuids": always_hidden_property_duids,
             }
         )
         if updated_by_client_duid is not UNSET:
             field_dict["updatedByClientDuid"] = updated_by_client_duid
 
         return field_dict
 
@@ -139,14 +149,18 @@
 
         color_name = ColorName(d.pop("colorName"))
 
         layout_duid = d.pop("layoutDuid")
 
         favorited_by_user_duids = cast(List[str], d.pop("favoritedByUserDuids"))
 
+        always_shown_property_duids = cast(List[str], d.pop("alwaysShownPropertyDuids"))
+
+        always_hidden_property_duids = cast(List[str], d.pop("alwaysHiddenPropertyDuids"))
+
         updated_by_client_duid = d.pop("updatedByClientDuid", UNSET)
 
         view = cls(
             duid=duid,
             kind=kind,
             accessible_by_team=accessible_by_team,
             accessible_by_user_duids=accessible_by_user_duids,
@@ -154,14 +168,16 @@
             title=title,
             description=description,
             icon_kind=icon_kind,
             icon_name_or_emoji=icon_name_or_emoji,
             color_name=color_name,
             layout_duid=layout_duid,
             favorited_by_user_duids=favorited_by_user_duids,
+            always_shown_property_duids=always_shown_property_duids,
+            always_hidden_property_duids=always_hidden_property_duids,
             updated_by_client_duid=updated_by_client_duid,
         )
 
         view.additional_properties = d
         return view
 
     @property
```

### Comparing `dart-tools-0.5.5/dart/generated/models/yc_integration.py` & `dart_tools-0.5.6/dart/generated/models/yc_integration.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/generated/types.py` & `dart_tools-0.5.6/dart/generated/types.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/order_manager.py` & `dart_tools-0.5.6/dart/order_manager.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart/webhook.py` & `dart_tools-0.5.6/dart/webhook.py`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/dart_tools.egg-info/PKG-INFO` & `dart_tools-0.5.6/dart_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dart-tools
-Version: 0.5.5
+Version: 0.5.6
 Summary: The Dart CLI and Python Library
 Author-email: Dart Software Team <software@itsdart.com>
 License: MIT License
         
         Copyright (c) 2023 Dart
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dart-tools Version: 0.5.5 Summary: The Dart CLI and
+Metadata-Version: 2.1 Name: dart-tools Version: 0.5.6 Summary: The Dart CLI and
 Python Library Author-email: Dart Software Team
 itsdart.com> License: MIT License Copyright (c) 2023 Dart Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `dart-tools-0.5.5/dart_tools.egg-info/SOURCES.txt` & `dart_tools-0.5.6/dart_tools.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -170,14 +170,15 @@
 dart/generated/models/validation_error_response.py
 dart/generated/models/validation_error_response_items.py
 dart/generated/models/view.py
 dart/generated/models/view_create.py
 dart/generated/models/view_kind.py
 dart/generated/models/view_update.py
 dart/generated/models/yc_integration.py
+dart/generated/models/zapier_integration.py
 dart_tools.egg-info/PKG-INFO
 dart_tools.egg-info/SOURCES.txt
 dart_tools.egg-info/dependency_links.txt
 dart_tools.egg-info/entry_points.txt
 dart_tools.egg-info/requires.txt
 dart_tools.egg-info/top_level.txt
 dart_tools.egg-info/dist/dart-tools-0.3.3.tar.gz
```

### Comparing `dart-tools-0.5.5/dart_tools.egg-info/dist/dart-tools-0.3.3.tar.gz` & `dart_tools-0.5.6/dart_tools.egg-info/dist/dart-tools-0.3.3.tar.gz`

 * *Files identical despite different names*

### Comparing `dart-tools-0.5.5/pyproject.toml` & `dart_tools-0.5.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dart-tools"
-version = "0.5.5"
+version = "0.5.6"
 description = "The Dart CLI and Python Library"
 readme = "README.md"
 requires-python = ">=3.8"
 
 license = {file = "LICENSE"}
 keywords = ["dart", "cli", "projectmanagement", "taskmanagement"]
 authors = [
```

