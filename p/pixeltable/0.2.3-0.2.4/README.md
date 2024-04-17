# Comparing `tmp/pixeltable-0.2.3.tar.gz` & `tmp/pixeltable-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixeltable-0.2.3.tar", max compression
+gzip compressed data, was "pixeltable-0.2.4.tar", max compression
```

## Comparing `pixeltable-0.2.3.tar` & `pixeltable-0.2.4.tar`

### file list

```diff
@@ -1,126 +1,132 @@
--rw-r--r--   0        0        0      746 2024-03-22 03:20:30.854989 pixeltable-0.2.3/LICENSE
--rw-r--r--   0        0        0     4193 2024-04-06 17:38:28.064844 pixeltable-0.2.3/README.md
--rw-r--r--   0        0        0      959 2024-04-04 00:11:47.491970 pixeltable-0.2.3/pixeltable/__init__.py
--rw-r--r--   0        0        0      453 2024-03-22 03:20:30.929081 pixeltable-0.2.3/pixeltable/catalog/__init__.py
--rw-r--r--   0        0        0     7908 2024-04-04 00:11:47.492457 pixeltable-0.2.3/pixeltable/catalog/catalog.py
--rw-r--r--   0        0        0     8661 2024-04-04 00:11:47.492730 pixeltable-0.2.3/pixeltable/catalog/column.py
--rw-r--r--   0        0        0      919 2024-03-22 03:20:30.929659 pixeltable-0.2.3/pixeltable/catalog/dir.py
--rw-r--r--   0        0        0      943 2024-03-22 03:20:30.929786 pixeltable-0.2.3/pixeltable/catalog/globals.py
--rw-r--r--   0        0        0     8280 2024-04-04 00:11:47.492972 pixeltable-0.2.3/pixeltable/catalog/insertable_table.py
--rw-r--r--   0        0        0     1147 2024-03-22 03:20:30.930368 pixeltable-0.2.3/pixeltable/catalog/named_function.py
--rw-r--r--   0        0        0     1677 2024-04-04 00:11:47.493163 pixeltable-0.2.3/pixeltable/catalog/path.py
--rw-r--r--   0        0        0     5941 2024-04-04 00:11:47.493341 pixeltable-0.2.3/pixeltable/catalog/path_dict.py
--rw-r--r--   0        0        0     1059 2024-03-22 03:20:30.931044 pixeltable-0.2.3/pixeltable/catalog/schema_object.py
--rw-r--r--   0        0        0    25499 2024-04-04 00:11:47.493604 pixeltable-0.2.3/pixeltable/catalog/table.py
--rw-r--r--   0        0        0    35680 2024-04-04 00:11:47.493943 pixeltable-0.2.3/pixeltable/catalog/table_version.py
--rw-r--r--   0        0        0     5461 2024-04-04 00:11:47.494156 pixeltable-0.2.3/pixeltable/catalog/table_version_path.py
--rw-r--r--   0        0        0     9734 2024-04-04 00:11:47.494389 pixeltable-0.2.3/pixeltable/catalog/view.py
--rw-r--r--   0        0        0    20548 2024-04-04 00:11:47.494657 pixeltable-0.2.3/pixeltable/client.py
--rw-r--r--   0        0        0    28339 2024-04-06 17:38:28.087008 pixeltable-0.2.3/pixeltable/dataframe.py
--rw-r--r--   0        0        0    16398 2024-04-06 17:38:28.087581 pixeltable-0.2.3/pixeltable/env.py
--rw-r--r--   0        0        0      376 2024-03-22 03:20:30.937922 pixeltable-0.2.3/pixeltable/exceptions.py
--rw-r--r--   0        0        0      412 2024-03-22 03:20:30.938153 pixeltable-0.2.3/pixeltable/exec/__init__.py
--rw-r--r--   0        0        0     3321 2024-04-04 00:11:47.495476 pixeltable-0.2.3/pixeltable/exec/aggregation_node.py
--rw-r--r--   0        0        0     5212 2024-04-08 22:50:04.684752 pixeltable-0.2.3/pixeltable/exec/cache_prefetch_node.py
--rw-r--r--   0        0        0     4069 2024-03-22 03:20:30.939348 pixeltable-0.2.3/pixeltable/exec/component_iteration_node.py
--rw-r--r--   0        0        0     3505 2024-03-22 03:20:30.939513 pixeltable-0.2.3/pixeltable/exec/data_row_batch.py
--rw-r--r--   0        0        0      924 2024-03-22 03:20:30.939633 pixeltable-0.2.3/pixeltable/exec/exec_context.py
--rw-r--r--   0        0        0     2170 2024-03-22 03:20:30.939748 pixeltable-0.2.3/pixeltable/exec/exec_node.py
--rw-r--r--   0        0        0    10810 2024-04-04 00:11:47.495696 pixeltable-0.2.3/pixeltable/exec/expr_eval_node.py
--rw-r--r--   0        0        0     2949 2024-03-22 03:20:30.941553 pixeltable-0.2.3/pixeltable/exec/in_memory_data_node.py
--rw-r--r--   0        0        0     1514 2024-03-22 03:20:30.945244 pixeltable-0.2.3/pixeltable/exec/media_validation_node.py
--rw-r--r--   0        0        0    10318 2024-03-22 03:20:30.945695 pixeltable-0.2.3/pixeltable/exec/sql_scan_node.py
--rw-r--r--   0        0        0      935 2024-04-04 00:11:47.495925 pixeltable-0.2.3/pixeltable/exprs/__init__.py
--rw-r--r--   0        0        0     4386 2024-03-22 03:20:30.948503 pixeltable-0.2.3/pixeltable/exprs/arithmetic_expr.py
--rw-r--r--   0        0        0     2131 2024-03-22 03:20:30.948806 pixeltable-0.2.3/pixeltable/exprs/array_slice.py
--rw-r--r--   0        0        0     2706 2024-03-22 03:20:30.949036 pixeltable-0.2.3/pixeltable/exprs/column_property_ref.py
--rw-r--r--   0        0        0     4794 2024-03-22 03:20:30.949236 pixeltable-0.2.3/pixeltable/exprs/column_ref.py
--rw-r--r--   0        0        0     3000 2024-03-22 03:20:30.949375 pixeltable-0.2.3/pixeltable/exprs/comparison.py
--rw-r--r--   0        0        0     3830 2024-03-22 03:20:30.949509 pixeltable-0.2.3/pixeltable/exprs/compound_predicate.py
--rw-r--r--   0        0        0     8046 2024-04-08 22:50:04.685112 pixeltable-0.2.3/pixeltable/exprs/data_row.py
--rw-r--r--   0        0        0    23748 2024-04-04 00:11:47.496409 pixeltable-0.2.3/pixeltable/exprs/expr.py
--rw-r--r--   0        0        0     1222 2024-03-22 03:20:30.954653 pixeltable-0.2.3/pixeltable/exprs/expr_set.py
--rw-r--r--   0        0        0    16961 2024-04-04 00:11:47.496718 pixeltable-0.2.3/pixeltable/exprs/function_call.py
--rw-r--r--   0        0        0     1537 2024-03-22 03:20:30.958471 pixeltable-0.2.3/pixeltable/exprs/globals.py
--rw-r--r--   0        0        0     4663 2024-03-22 03:20:30.958665 pixeltable-0.2.3/pixeltable/exprs/image_member_access.py
--rw-r--r--   0        0        0     1906 2024-03-22 03:20:30.958803 pixeltable-0.2.3/pixeltable/exprs/image_similarity_predicate.py
--rw-r--r--   0        0        0     4312 2024-03-22 03:20:30.958978 pixeltable-0.2.3/pixeltable/exprs/inline_array.py
--rw-r--r--   0        0        0     3695 2024-03-22 03:20:30.959427 pixeltable-0.2.3/pixeltable/exprs/inline_dict.py
--rw-r--r--   0        0        0     1041 2024-03-22 03:20:30.959589 pixeltable-0.2.3/pixeltable/exprs/is_null.py
--rw-r--r--   0        0        0     4559 2024-03-22 03:20:30.959717 pixeltable-0.2.3/pixeltable/exprs/json_mapper.py
--rw-r--r--   0        0        0     6526 2024-03-22 03:20:30.959875 pixeltable-0.2.3/pixeltable/exprs/json_path.py
--rw-r--r--   0        0        0     1885 2024-03-22 03:20:30.960091 pixeltable-0.2.3/pixeltable/exprs/literal.py
--rw-r--r--   0        0        0     1250 2024-03-22 03:20:30.960205 pixeltable-0.2.3/pixeltable/exprs/object_ref.py
--rw-r--r--   0        0        0     1859 2024-03-22 03:20:30.960322 pixeltable-0.2.3/pixeltable/exprs/predicate.py
--rw-r--r--   0        0        0    16992 2024-04-04 00:11:47.497017 pixeltable-0.2.3/pixeltable/exprs/row_builder.py
--rw-r--r--   0        0        0     4268 2024-03-22 03:20:30.962221 pixeltable-0.2.3/pixeltable/exprs/rowid_ref.py
--rw-r--r--   0        0        0     1793 2024-03-22 03:20:30.962353 pixeltable-0.2.3/pixeltable/exprs/type_cast.py
--rw-r--r--   0        0        0     1361 2024-04-04 00:11:47.497543 pixeltable-0.2.3/pixeltable/exprs/variable.py
--rw-r--r--   0        0        0      457 2024-04-04 00:11:47.497746 pixeltable-0.2.3/pixeltable/func/__init__.py
--rw-r--r--   0        0        0     9177 2024-04-04 00:11:47.497895 pixeltable-0.2.3/pixeltable/func/aggregate_function.py
--rw-r--r--   0        0        0     2350 2024-04-04 00:11:47.498062 pixeltable-0.2.3/pixeltable/func/batched_function.py
--rw-r--r--   0        0        0     2357 2024-04-04 00:11:47.498480 pixeltable-0.2.3/pixeltable/func/callable_function.py
--rw-r--r--   0        0        0     3392 2024-04-04 00:11:47.498601 pixeltable-0.2.3/pixeltable/func/expr_template_function.py
--rw-r--r--   0        0        0     4023 2024-04-04 00:11:47.498783 pixeltable-0.2.3/pixeltable/func/function.py
--rw-r--r--   0        0        0    11456 2024-04-04 00:11:47.498985 pixeltable-0.2.3/pixeltable/func/function_registry.py
--rw-r--r--   0        0        0     1220 2024-04-04 00:11:47.499364 pixeltable-0.2.3/pixeltable/func/globals.py
--rw-r--r--   0        0        0     9650 2024-04-04 00:11:47.499601 pixeltable-0.2.3/pixeltable/func/nos_function.py
--rw-r--r--   0        0        0     7107 2024-04-04 00:11:47.499798 pixeltable-0.2.3/pixeltable/func/signature.py
--rw-r--r--   0        0        0     6457 2024-04-04 00:11:47.499973 pixeltable-0.2.3/pixeltable/func/udf.py
--rw-r--r--   0        0        0     3419 2024-04-04 00:11:47.500386 pixeltable-0.2.3/pixeltable/functions/__init__.py
--rw-r--r--   0        0        0     8453 2024-04-04 00:11:47.500621 pixeltable-0.2.3/pixeltable/functions/eval.py
--rw-r--r--   0        0        0     1596 2024-04-06 17:37:50.512896 pixeltable-0.2.3/pixeltable/functions/fireworks.py
--rw-r--r--   0        0        0     4804 2024-04-04 00:11:47.500918 pixeltable-0.2.3/pixeltable/functions/huggingface.py
--rw-r--r--   0        0        0      431 2024-04-04 00:11:47.501186 pixeltable-0.2.3/pixeltable/functions/image.py
--rw-r--r--   0        0        0     2863 2024-04-04 00:11:47.501300 pixeltable-0.2.3/pixeltable/functions/openai.py
--rw-r--r--   0        0        0     6217 2024-04-04 00:11:47.501525 pixeltable-0.2.3/pixeltable/functions/pil/image.py
--rw-r--r--   0        0        0      516 2024-04-04 00:11:47.501661 pixeltable-0.2.3/pixeltable/functions/string.py
--rw-r--r--   0        0        0      650 2024-04-04 00:11:47.501927 pixeltable-0.2.3/pixeltable/functions/together.py
--rw-r--r--   0        0        0     1596 2024-04-04 00:11:47.502099 pixeltable-0.2.3/pixeltable/functions/util.py
--rw-r--r--   0        0        0     2403 2024-04-04 00:11:47.502279 pixeltable-0.2.3/pixeltable/functions/video.py
--rw-r--r--   0        0        0       70 2024-03-22 03:20:30.970568 pixeltable-0.2.3/pixeltable/iterators/__init__.py
--rw-r--r--   0        0        0     1545 2024-03-22 03:20:30.970760 pixeltable-0.2.3/pixeltable/iterators/base.py
--rw-r--r--   0        0        0    13105 2024-04-08 22:50:04.685460 pixeltable-0.2.3/pixeltable/iterators/document.py
--rw-r--r--   0        0        0     3444 2024-03-22 03:20:30.991846 pixeltable-0.2.3/pixeltable/iterators/video.py
--rw-r--r--   0        0        0     2083 2024-04-04 00:11:47.502483 pixeltable-0.2.3/pixeltable/metadata/__init__.py
--rw-r--r--   0        0        0      733 2024-03-22 03:20:30.992614 pixeltable-0.2.3/pixeltable/metadata/converters/convert_10.py
--rw-r--r--   0        0        0     7761 2024-04-04 00:11:47.502834 pixeltable-0.2.3/pixeltable/metadata/schema.py
--rw-r--r--   0        0        0    34710 2024-04-04 00:11:47.503153 pixeltable-0.2.3/pixeltable/plan.py
--rw-r--r--   0        0        0    19511 2024-04-08 22:50:04.685849 pixeltable-0.2.3/pixeltable/store.py
--rw-r--r--   0        0        0     6677 2024-04-06 17:38:28.088257 pixeltable-0.2.3/pixeltable/tests/conftest.py
--rw-r--r--   0        0        0     3186 2024-04-04 00:11:47.504570 pixeltable-0.2.3/pixeltable/tests/test_audio.py
--rw-r--r--   0        0        0     1189 2024-03-22 03:20:31.514506 pixeltable-0.2.3/pixeltable/tests/test_catalog.py
--rw-r--r--   0        0        0      531 2024-04-04 00:11:47.504789 pixeltable-0.2.3/pixeltable/tests/test_client.py
--rw-r--r--   0        0        0    17732 2024-04-06 17:38:28.114456 pixeltable-0.2.3/pixeltable/tests/test_component_view.py
--rw-r--r--   0        0        0    18007 2024-04-08 22:50:04.686513 pixeltable-0.2.3/pixeltable/tests/test_dataframe.py
--rw-r--r--   0        0        0     3611 2024-04-04 00:11:47.505572 pixeltable-0.2.3/pixeltable/tests/test_dirs.py
--rw-r--r--   0        0        0     5810 2024-04-06 17:38:32.384273 pixeltable-0.2.3/pixeltable/tests/test_document.py
--rw-r--r--   0        0        0    32743 2024-04-08 22:50:04.687225 pixeltable-0.2.3/pixeltable/tests/test_exprs.py
--rw-r--r--   0        0        0    12817 2024-04-04 00:11:47.506385 pixeltable-0.2.3/pixeltable/tests/test_function.py
--rw-r--r--   0        0        0    14394 2024-04-06 17:38:28.115085 pixeltable-0.2.3/pixeltable/tests/test_functions.py
--rw-r--r--   0        0        0     1535 2024-04-04 00:11:47.506868 pixeltable-0.2.3/pixeltable/tests/test_migration.py
--rw-r--r--   0        0        0     2649 2024-04-04 00:11:47.507072 pixeltable-0.2.3/pixeltable/tests/test_nos.py
--rw-r--r--   0        0        0     9297 2024-04-04 00:11:47.507288 pixeltable-0.2.3/pixeltable/tests/test_snapshot.py
--rw-r--r--   0        0        0    48484 2024-04-06 17:38:32.384895 pixeltable-0.2.3/pixeltable/tests/test_table.py
--rw-r--r--   0        0        0     1308 2024-04-04 00:11:47.507879 pixeltable-0.2.3/pixeltable/tests/test_transactional_directory.py
--rw-r--r--   0        0        0      970 2024-04-04 00:11:47.508085 pixeltable-0.2.3/pixeltable/tests/test_types.py
--rw-r--r--   0        0        0     7782 2024-04-06 17:38:32.385556 pixeltable-0.2.3/pixeltable/tests/test_video.py
--rw-r--r--   0        0        0    21859 2024-04-04 00:11:47.508548 pixeltable-0.2.3/pixeltable/tests/test_view.py
--rw-r--r--   0        0        0    10378 2024-04-08 22:50:04.687903 pixeltable-0.2.3/pixeltable/tests/utils.py
--rw-r--r--   0        0        0     5148 2024-04-04 00:11:47.508980 pixeltable-0.2.3/pixeltable/tool/create_test_db_dump.py
--rw-r--r--   0        0        0     2899 2024-04-06 17:38:28.116159 pixeltable-0.2.3/pixeltable/tool/create_test_video.py
--rw-r--r--   0        0        0    31798 2024-04-08 22:50:04.688715 pixeltable-0.2.3/pixeltable/type_system.py
--rw-r--r--   0        0        0      439 2024-03-22 03:20:31.517814 pixeltable-0.2.3/pixeltable/utils/__init__.py
--rw-r--r--   0        0        0      720 2024-03-22 03:20:31.517938 pixeltable-0.2.3/pixeltable/utils/clip.py
--rw-r--r--   0        0        0     5604 2024-03-22 03:20:31.518069 pixeltable-0.2.3/pixeltable/utils/coco.py
--rw-r--r--   0        0        0     1094 2024-03-22 03:20:31.518173 pixeltable-0.2.3/pixeltable/utils/documents.py
--rw-r--r--   0        0        0     7839 2024-03-22 03:20:31.518306 pixeltable-0.2.3/pixeltable/utils/filecache.py
--rw-r--r--   0        0        0      252 2024-03-22 03:20:31.518421 pixeltable-0.2.3/pixeltable/utils/help.py
--rw-r--r--   0        0        0     3116 2024-03-22 03:20:31.518536 pixeltable-0.2.3/pixeltable/utils/media_store.py
--rw-r--r--   0        0        0     5775 2024-03-22 03:20:31.518658 pixeltable-0.2.3/pixeltable/utils/parquet.py
--rw-r--r--   0        0        0     6515 2024-04-04 00:11:47.509542 pixeltable-0.2.3/pixeltable/utils/pytorch.py
--rw-r--r--   0        0        0      432 2024-03-22 03:20:31.518890 pixeltable-0.2.3/pixeltable/utils/s3.py
--rw-r--r--   0        0        0      765 2024-03-22 03:20:31.519000 pixeltable-0.2.3/pixeltable/utils/sql.py
--rw-r--r--   0        0        0     1349 2024-04-04 00:11:47.509715 pixeltable-0.2.3/pixeltable/utils/transactional_directory.py
--rw-r--r--   0        0        0     3267 2024-04-08 22:50:04.692841 pixeltable-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     5473 1970-01-01 00:00:00.000000 pixeltable-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      746 2024-03-22 03:20:30.854989 pixeltable-0.2.4/LICENSE
+-rw-r--r--   0        0        0     4680 2024-04-17 01:12:13.386362 pixeltable-0.2.4/README.md
+-rw-r--r--   0        0        0      959 2024-04-04 00:11:47.491970 pixeltable-0.2.4/pixeltable/__init__.py
+-rw-r--r--   0        0        0      453 2024-03-22 03:20:30.929081 pixeltable-0.2.4/pixeltable/catalog/__init__.py
+-rw-r--r--   0        0        0     7908 2024-04-04 00:11:47.492457 pixeltable-0.2.4/pixeltable/catalog/catalog.py
+-rw-r--r--   0        0        0     8663 2024-04-17 01:12:13.387513 pixeltable-0.2.4/pixeltable/catalog/column.py
+-rw-r--r--   0        0        0      919 2024-03-22 03:20:30.929659 pixeltable-0.2.4/pixeltable/catalog/dir.py
+-rw-r--r--   0        0        0      943 2024-03-22 03:20:30.929786 pixeltable-0.2.4/pixeltable/catalog/globals.py
+-rw-r--r--   0        0        0     8280 2024-04-04 00:11:47.492972 pixeltable-0.2.4/pixeltable/catalog/insertable_table.py
+-rw-r--r--   0        0        0     1147 2024-03-22 03:20:30.930368 pixeltable-0.2.4/pixeltable/catalog/named_function.py
+-rw-r--r--   0        0        0     1677 2024-04-04 00:11:47.493163 pixeltable-0.2.4/pixeltable/catalog/path.py
+-rw-r--r--   0        0        0     5941 2024-04-04 00:11:47.493341 pixeltable-0.2.4/pixeltable/catalog/path_dict.py
+-rw-r--r--   0        0        0     1059 2024-03-22 03:20:30.931044 pixeltable-0.2.4/pixeltable/catalog/schema_object.py
+-rw-r--r--   0        0        0    25499 2024-04-04 00:11:47.493604 pixeltable-0.2.4/pixeltable/catalog/table.py
+-rw-r--r--   0        0        0    35680 2024-04-04 00:11:47.493943 pixeltable-0.2.4/pixeltable/catalog/table_version.py
+-rw-r--r--   0        0        0     5461 2024-04-04 00:11:47.494156 pixeltable-0.2.4/pixeltable/catalog/table_version_path.py
+-rw-r--r--   0        0        0     9734 2024-04-04 00:11:47.494389 pixeltable-0.2.4/pixeltable/catalog/view.py
+-rw-r--r--   0        0        0    23616 2024-04-17 01:12:13.388062 pixeltable-0.2.4/pixeltable/client.py
+-rw-r--r--   0        0        0    28339 2024-04-06 17:38:28.087008 pixeltable-0.2.4/pixeltable/dataframe.py
+-rw-r--r--   0        0        0    15744 2024-04-17 01:12:13.388412 pixeltable-0.2.4/pixeltable/env.py
+-rw-r--r--   0        0        0      376 2024-03-22 03:20:30.937922 pixeltable-0.2.4/pixeltable/exceptions.py
+-rw-r--r--   0        0        0      412 2024-03-22 03:20:30.938153 pixeltable-0.2.4/pixeltable/exec/__init__.py
+-rw-r--r--   0        0        0     3321 2024-04-04 00:11:47.495476 pixeltable-0.2.4/pixeltable/exec/aggregation_node.py
+-rw-r--r--   0        0        0     5212 2024-04-08 22:50:04.684752 pixeltable-0.2.4/pixeltable/exec/cache_prefetch_node.py
+-rw-r--r--   0        0        0     4069 2024-03-22 03:20:30.939348 pixeltable-0.2.4/pixeltable/exec/component_iteration_node.py
+-rw-r--r--   0        0        0     3505 2024-03-22 03:20:30.939513 pixeltable-0.2.4/pixeltable/exec/data_row_batch.py
+-rw-r--r--   0        0        0      924 2024-03-22 03:20:30.939633 pixeltable-0.2.4/pixeltable/exec/exec_context.py
+-rw-r--r--   0        0        0     2170 2024-03-22 03:20:30.939748 pixeltable-0.2.4/pixeltable/exec/exec_node.py
+-rw-r--r--   0        0        0    10810 2024-04-04 00:11:47.495696 pixeltable-0.2.4/pixeltable/exec/expr_eval_node.py
+-rw-r--r--   0        0        0     2949 2024-03-22 03:20:30.941553 pixeltable-0.2.4/pixeltable/exec/in_memory_data_node.py
+-rw-r--r--   0        0        0     1514 2024-03-22 03:20:30.945244 pixeltable-0.2.4/pixeltable/exec/media_validation_node.py
+-rw-r--r--   0        0        0    10318 2024-03-22 03:20:30.945695 pixeltable-0.2.4/pixeltable/exec/sql_scan_node.py
+-rw-r--r--   0        0        0      935 2024-04-04 00:11:47.495925 pixeltable-0.2.4/pixeltable/exprs/__init__.py
+-rw-r--r--   0        0        0     4386 2024-03-22 03:20:30.948503 pixeltable-0.2.4/pixeltable/exprs/arithmetic_expr.py
+-rw-r--r--   0        0        0     2131 2024-03-22 03:20:30.948806 pixeltable-0.2.4/pixeltable/exprs/array_slice.py
+-rw-r--r--   0        0        0     2706 2024-03-22 03:20:30.949036 pixeltable-0.2.4/pixeltable/exprs/column_property_ref.py
+-rw-r--r--   0        0        0     4794 2024-03-22 03:20:30.949236 pixeltable-0.2.4/pixeltable/exprs/column_ref.py
+-rw-r--r--   0        0        0     3000 2024-03-22 03:20:30.949375 pixeltable-0.2.4/pixeltable/exprs/comparison.py
+-rw-r--r--   0        0        0     3830 2024-03-22 03:20:30.949509 pixeltable-0.2.4/pixeltable/exprs/compound_predicate.py
+-rw-r--r--   0        0        0     8046 2024-04-08 22:50:04.685112 pixeltable-0.2.4/pixeltable/exprs/data_row.py
+-rw-r--r--   0        0        0    23748 2024-04-04 00:11:47.496409 pixeltable-0.2.4/pixeltable/exprs/expr.py
+-rw-r--r--   0        0        0     1222 2024-03-22 03:20:30.954653 pixeltable-0.2.4/pixeltable/exprs/expr_set.py
+-rw-r--r--   0        0        0    16961 2024-04-04 00:11:47.496718 pixeltable-0.2.4/pixeltable/exprs/function_call.py
+-rw-r--r--   0        0        0     1537 2024-03-22 03:20:30.958471 pixeltable-0.2.4/pixeltable/exprs/globals.py
+-rw-r--r--   0        0        0     4663 2024-03-22 03:20:30.958665 pixeltable-0.2.4/pixeltable/exprs/image_member_access.py
+-rw-r--r--   0        0        0     1906 2024-03-22 03:20:30.958803 pixeltable-0.2.4/pixeltable/exprs/image_similarity_predicate.py
+-rw-r--r--   0        0        0     4312 2024-03-22 03:20:30.958978 pixeltable-0.2.4/pixeltable/exprs/inline_array.py
+-rw-r--r--   0        0        0     3695 2024-03-22 03:20:30.959427 pixeltable-0.2.4/pixeltable/exprs/inline_dict.py
+-rw-r--r--   0        0        0     1041 2024-03-22 03:20:30.959589 pixeltable-0.2.4/pixeltable/exprs/is_null.py
+-rw-r--r--   0        0        0     4559 2024-03-22 03:20:30.959717 pixeltable-0.2.4/pixeltable/exprs/json_mapper.py
+-rw-r--r--   0        0        0     6526 2024-03-22 03:20:30.959875 pixeltable-0.2.4/pixeltable/exprs/json_path.py
+-rw-r--r--   0        0        0     1885 2024-03-22 03:20:30.960091 pixeltable-0.2.4/pixeltable/exprs/literal.py
+-rw-r--r--   0        0        0     1250 2024-03-22 03:20:30.960205 pixeltable-0.2.4/pixeltable/exprs/object_ref.py
+-rw-r--r--   0        0        0     1859 2024-03-22 03:20:30.960322 pixeltable-0.2.4/pixeltable/exprs/predicate.py
+-rw-r--r--   0        0        0    16992 2024-04-04 00:11:47.497017 pixeltable-0.2.4/pixeltable/exprs/row_builder.py
+-rw-r--r--   0        0        0     4268 2024-03-22 03:20:30.962221 pixeltable-0.2.4/pixeltable/exprs/rowid_ref.py
+-rw-r--r--   0        0        0     1793 2024-03-22 03:20:30.962353 pixeltable-0.2.4/pixeltable/exprs/type_cast.py
+-rw-r--r--   0        0        0     1361 2024-04-04 00:11:47.497543 pixeltable-0.2.4/pixeltable/exprs/variable.py
+-rw-r--r--   0        0        0      457 2024-04-04 00:11:47.497746 pixeltable-0.2.4/pixeltable/func/__init__.py
+-rw-r--r--   0        0        0     9177 2024-04-04 00:11:47.497895 pixeltable-0.2.4/pixeltable/func/aggregate_function.py
+-rw-r--r--   0        0        0     2350 2024-04-04 00:11:47.498062 pixeltable-0.2.4/pixeltable/func/batched_function.py
+-rw-r--r--   0        0        0     2357 2024-04-04 00:11:47.498480 pixeltable-0.2.4/pixeltable/func/callable_function.py
+-rw-r--r--   0        0        0     3392 2024-04-04 00:11:47.498601 pixeltable-0.2.4/pixeltable/func/expr_template_function.py
+-rw-r--r--   0        0        0     4023 2024-04-04 00:11:47.498783 pixeltable-0.2.4/pixeltable/func/function.py
+-rw-r--r--   0        0        0    11456 2024-04-04 00:11:47.498985 pixeltable-0.2.4/pixeltable/func/function_registry.py
+-rw-r--r--   0        0        0     1220 2024-04-04 00:11:47.499364 pixeltable-0.2.4/pixeltable/func/globals.py
+-rw-r--r--   0        0        0     9650 2024-04-04 00:11:47.499601 pixeltable-0.2.4/pixeltable/func/nos_function.py
+-rw-r--r--   0        0        0     7107 2024-04-04 00:11:47.499798 pixeltable-0.2.4/pixeltable/func/signature.py
+-rw-r--r--   0        0        0     6457 2024-04-04 00:11:47.499973 pixeltable-0.2.4/pixeltable/func/udf.py
+-rw-r--r--   0        0        0     3390 2024-04-17 01:12:13.388971 pixeltable-0.2.4/pixeltable/functions/__init__.py
+-rw-r--r--   0        0        0     8453 2024-04-04 00:11:47.500621 pixeltable-0.2.4/pixeltable/functions/eval.py
+-rw-r--r--   0        0        0      908 2024-04-17 01:12:13.389269 pixeltable-0.2.4/pixeltable/functions/fireworks.py
+-rw-r--r--   0        0        0     4804 2024-04-04 00:11:47.500918 pixeltable-0.2.4/pixeltable/functions/huggingface.py
+-rw-r--r--   0        0        0      431 2024-04-04 00:11:47.501186 pixeltable-0.2.4/pixeltable/functions/image.py
+-rw-r--r--   0        0        0     6861 2024-04-17 01:12:13.389598 pixeltable-0.2.4/pixeltable/functions/openai.py
+-rw-r--r--   0        0        0     6217 2024-04-04 00:11:47.501525 pixeltable-0.2.4/pixeltable/functions/pil/image.py
+-rw-r--r--   0        0        0      516 2024-04-04 00:11:47.501661 pixeltable-0.2.4/pixeltable/functions/string.py
+-rw-r--r--   0        0        0     3423 2024-04-17 01:12:13.390515 pixeltable-0.2.4/pixeltable/functions/together.py
+-rw-r--r--   0        0        0     1596 2024-04-04 00:11:47.502099 pixeltable-0.2.4/pixeltable/functions/util.py
+-rw-r--r--   0        0        0     2403 2024-04-04 00:11:47.502279 pixeltable-0.2.4/pixeltable/functions/video.py
+-rw-r--r--   0        0        0       70 2024-03-22 03:20:30.970568 pixeltable-0.2.4/pixeltable/iterators/__init__.py
+-rw-r--r--   0        0        0     1545 2024-03-22 03:20:30.970760 pixeltable-0.2.4/pixeltable/iterators/base.py
+-rw-r--r--   0        0        0    13105 2024-04-08 22:50:04.685460 pixeltable-0.2.4/pixeltable/iterators/document.py
+-rw-r--r--   0        0        0     3444 2024-03-22 03:20:30.991846 pixeltable-0.2.4/pixeltable/iterators/video.py
+-rw-r--r--   0        0        0     2083 2024-04-04 00:11:47.502483 pixeltable-0.2.4/pixeltable/metadata/__init__.py
+-rw-r--r--   0        0        0      733 2024-03-22 03:20:30.992614 pixeltable-0.2.4/pixeltable/metadata/converters/convert_10.py
+-rw-r--r--   0        0        0     7761 2024-04-04 00:11:47.502834 pixeltable-0.2.4/pixeltable/metadata/schema.py
+-rw-r--r--   0        0        0    34710 2024-04-04 00:11:47.503153 pixeltable-0.2.4/pixeltable/plan.py
+-rw-r--r--   0        0        0    19511 2024-04-08 22:50:04.685849 pixeltable-0.2.4/pixeltable/store.py
+-rw-r--r--   0        0        0     6684 2024-04-17 01:12:13.409679 pixeltable-0.2.4/pixeltable/tests/conftest.py
+-rw-r--r--   0        0        0     1666 2024-04-17 01:12:13.428542 pixeltable-0.2.4/pixeltable/tests/functions/test_fireworks.py
+-rw-r--r--   0        0        0     2884 2024-04-17 01:12:13.428969 pixeltable-0.2.4/pixeltable/tests/functions/test_functions.py
+-rw-r--r--   0        0        0     7739 2024-04-17 01:12:13.429213 pixeltable-0.2.4/pixeltable/tests/functions/test_huggingface.py
+-rw-r--r--   0        0        0     8172 2024-04-17 01:12:13.429479 pixeltable-0.2.4/pixeltable/tests/functions/test_openai.py
+-rw-r--r--   0        0        0     4788 2024-04-17 01:12:13.429686 pixeltable-0.2.4/pixeltable/tests/functions/test_together.py
+-rw-r--r--   0        0        0     3186 2024-04-04 00:11:47.504570 pixeltable-0.2.4/pixeltable/tests/test_audio.py
+-rw-r--r--   0        0        0     1189 2024-03-22 03:20:31.514506 pixeltable-0.2.4/pixeltable/tests/test_catalog.py
+-rw-r--r--   0        0        0      531 2024-04-04 00:11:47.504789 pixeltable-0.2.4/pixeltable/tests/test_client.py
+-rw-r--r--   0        0        0    17732 2024-04-06 17:38:28.114456 pixeltable-0.2.4/pixeltable/tests/test_component_view.py
+-rw-r--r--   0        0        0    17975 2024-04-17 01:12:13.430071 pixeltable-0.2.4/pixeltable/tests/test_dataframe.py
+-rw-r--r--   0        0        0     3611 2024-04-04 00:11:47.505572 pixeltable-0.2.4/pixeltable/tests/test_dirs.py
+-rw-r--r--   0        0        0     5810 2024-04-06 17:38:32.384273 pixeltable-0.2.4/pixeltable/tests/test_document.py
+-rw-r--r--   0        0        0    32743 2024-04-08 22:50:04.687225 pixeltable-0.2.4/pixeltable/tests/test_exprs.py
+-rw-r--r--   0        0        0    12817 2024-04-04 00:11:47.506385 pixeltable-0.2.4/pixeltable/tests/test_function.py
+-rw-r--r--   0        0        0     1535 2024-04-04 00:11:47.506868 pixeltable-0.2.4/pixeltable/tests/test_migration.py
+-rw-r--r--   0        0        0     2649 2024-04-04 00:11:47.507072 pixeltable-0.2.4/pixeltable/tests/test_nos.py
+-rw-r--r--   0        0        0     9297 2024-04-04 00:11:47.507288 pixeltable-0.2.4/pixeltable/tests/test_snapshot.py
+-rw-r--r--   0        0        0    53303 2024-04-17 01:12:13.430814 pixeltable-0.2.4/pixeltable/tests/test_table.py
+-rw-r--r--   0        0        0     1308 2024-04-04 00:11:47.507879 pixeltable-0.2.4/pixeltable/tests/test_transactional_directory.py
+-rw-r--r--   0        0        0      970 2024-04-04 00:11:47.508085 pixeltable-0.2.4/pixeltable/tests/test_types.py
+-rw-r--r--   0        0        0     7782 2024-04-06 17:38:32.385556 pixeltable-0.2.4/pixeltable/tests/test_video.py
+-rw-r--r--   0        0        0    21859 2024-04-04 00:11:47.508548 pixeltable-0.2.4/pixeltable/tests/test_view.py
+-rw-r--r--   0        0        0    14359 2024-04-17 01:12:13.431171 pixeltable-0.2.4/pixeltable/tests/utils.py
+-rw-r--r--   0        0        0     5148 2024-04-04 00:11:47.508980 pixeltable-0.2.4/pixeltable/tool/create_test_db_dump.py
+-rw-r--r--   0        0        0     2899 2024-04-06 17:38:28.116159 pixeltable-0.2.4/pixeltable/tool/create_test_video.py
+-rw-r--r--   0        0        0    30374 2024-04-17 01:12:13.431574 pixeltable-0.2.4/pixeltable/type_system.py
+-rw-r--r--   0        0        0      439 2024-03-22 03:20:31.517814 pixeltable-0.2.4/pixeltable/utils/__init__.py
+-rw-r--r--   0        0        0     3692 2024-04-17 01:12:13.431812 pixeltable-0.2.4/pixeltable/utils/arrow.py
+-rw-r--r--   0        0        0      720 2024-03-22 03:20:31.517938 pixeltable-0.2.4/pixeltable/utils/clip.py
+-rw-r--r--   0        0        0     5604 2024-03-22 03:20:31.518069 pixeltable-0.2.4/pixeltable/utils/coco.py
+-rw-r--r--   0        0        0     1094 2024-03-22 03:20:31.518173 pixeltable-0.2.4/pixeltable/utils/documents.py
+-rw-r--r--   0        0        0     7839 2024-03-22 03:20:31.518306 pixeltable-0.2.4/pixeltable/utils/filecache.py
+-rw-r--r--   0        0        0      252 2024-03-22 03:20:31.518421 pixeltable-0.2.4/pixeltable/utils/help.py
+-rw-r--r--   0        0        0     7005 2024-04-17 01:12:13.432021 pixeltable-0.2.4/pixeltable/utils/hf_datasets.py
+-rw-r--r--   0        0        0     3116 2024-03-22 03:20:31.518536 pixeltable-0.2.4/pixeltable/utils/media_store.py
+-rw-r--r--   0        0        0     7120 2024-04-17 01:12:13.432624 pixeltable-0.2.4/pixeltable/utils/parquet.py
+-rw-r--r--   0        0        0     3483 2024-04-17 01:12:13.433243 pixeltable-0.2.4/pixeltable/utils/pytorch.py
+-rw-r--r--   0        0        0      432 2024-03-22 03:20:31.518890 pixeltable-0.2.4/pixeltable/utils/s3.py
+-rw-r--r--   0        0        0      765 2024-03-22 03:20:31.519000 pixeltable-0.2.4/pixeltable/utils/sql.py
+-rw-r--r--   0        0        0     1349 2024-04-04 00:11:47.509715 pixeltable-0.2.4/pixeltable/utils/transactional_directory.py
+-rw-r--r--   0        0        0     3332 2024-04-17 01:12:13.436364 pixeltable-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     5983 1970-01-01 00:00:00.000000 pixeltable-0.2.4/PKG-INFO
```

### Comparing `pixeltable-0.2.3/LICENSE` & `pixeltable-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/README.md` & `pixeltable-0.2.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,39 @@
+<div align="center">
 <img src="docs/pixeltable-banner.png" width="45%"/>
 
-# Pixeltable: The Multimodal AI Data Plane
+# Unifying Data, Models, and Orchestration for AI Products
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 &nbsp;&nbsp;
 ![pytest status](https://github.com/pixeltable/pixeltable/actions/workflows/pytest.yml/badge.svg)
 
-Pixeltable is a Python library that lets AI engineers and data scientists focus on
-exploration, modeling, and app development without having to deal with the customary
-data plumbing.
+[Installation](https://pixeltable.github.io/pixeltable/getting-started/) | [Documentation](https://pixeltable.github.io/pixeltable/)
+</div>
 
-**Pixeltable redefines data infrastructure and workflow orchestration for AI development.**
-It brings together data storage, versioning, and indexing with orchestration and model
-versioning under a declarative table interface, with transformations, model inference,
-and custom logic represented as computed columns.
+Pixeltable is a Python library that lets AI engineers and data scientists focus on exploration, modeling, and app development without dealing with the customary data plumbing.
 
-## Quick Start
+## What problems does Pixeltable solve?
+
+Today’s solutions for AI app development require extensive custom coding and infrastructure
+plumbing. Tracking lineage and versions between and across data transformations, models, and
+deployment is cumbersome. Pixeltable is a replacement for traditional data plumbing, providing
+a unified plane for data, models, and orchestration. It removes the data plumbing overhead in
+building and productionizing AI applications.
+
+## ⚡Quick Start
+Learn the basics of Pixeltable through interactive examples. View the notebooks on Google Colab or Kaggle, for free.
 
-If you just want to play around with Pixeltable to see what it's capable of, the easiest way is to run
-the Pixeltable Basics tutorial in colab:
+### Pixeltable Basics
+In this tutorial, we'll survey how to create tables, populate them with data, and enhance them with built-in and user-defined transformations and AI operations.
 
-<a target="_blank" href="https://colab.research.google.com/github/pixeltable/pixeltable/blob/master/docs/tutorials/pixeltable-basics.ipynb">
-  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
-</a>
+[![Open in Kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/code/brunep/pixeltable-basics) <a target="_blank" href="https://colab.research.google.com/github/pixeltable/pixeltable/blob/master/docs/tutorials/pixeltable-basics.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a>
 
-## Installation
 
+## 💾 Installation
 Pixeltable works with Python 3.9, 3.10, or 3.11 running on Linux or MacOS.
 
 ```
 pip install pixeltable
 ```
 
 To verify that it's working:
@@ -41,22 +45,14 @@
 
 For more detailed installation instructions, see the
 [Getting Started with Pixeltable](https://pixeltable.github.io/pixeltable/getting-started/)
 guide. Then, check out the
 [Pixeltable Basics](https://pixeltable.github.io/pixeltable/tutorials/pixeltable-basics/)
 tutorial for a tour of its most important features.
 
-## What problems does Pixeltable solve?
-
-Today’s solutions for AI app development require extensive custom coding and infrastructure
-plumbing. Tracking lineage and versions between and across data transformations, models, and
-deployment is cumbersome. Pixeltable is a replacement for traditional data plumbing, providing
-a unified plane for data, models, and orchestration. It removes the data plumbing overhead in
-building and productionizing AI applications.
-
 ## Why should you use Pixeltable?
 
 - It gives you transparency and reproducibility
     - All generated data is automatically recorded and versioned
     - You will never need to re-run a workload because you lost track of the input data
 - It saves you money
     - All data changes are automatically incremental
@@ -81,7 +77,16 @@
 * Perform keyword and image similarity search at the video frame level without having to worry about frame
 storage.
 * Access all Pixeltable-resident data directly as a PyTorch dataset in your training scripts.
 * Understand the compute and storage costs of your data at the granularity of individual augmentations and
 get cost projections before adding new data and new augmentations.
 * Rely on Pixeltable's automatic versioning and snapshot functionality to protect against regressions
 and to ensure reproducibility.
+
+## Contributions & Feedback
+
+Are you experiencing issues or bugs with Pixeltable? File an [Issue](https://github.com/pixeltable/pixeltable/issues).
+</br>Do you want to contribute? Feel free to open a [PR](https://github.com/pixeltable/pixeltable/pulls).
+
+## :classical_building: License
+
+This library is licensed under the Apache 2.0 License.
```

### Comparing `pixeltable-0.2.3/pixeltable/__init__.py` & `pixeltable-0.2.4/pixeltable/__init__.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/catalog/catalog.py` & `pixeltable-0.2.4/pixeltable/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/catalog/column.py` & `pixeltable-0.2.4/pixeltable/catalog/column.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
         indexed: only valid for image columns; if true, maintains an NN index for this column
         """
         if not is_valid_identifier(name):
             raise excs.Error(f"Invalid column name: '{name}'")
         self.name = name
         if col_type is None and computed_with is None:
-            raise excs.Error(f'Column {name}: col_type is required if computed_with is not specified')
+            raise excs.Error(f'Column `{name}`: col_type is required if computed_with is not specified')
 
         self.value_expr: Optional['Expr'] = None
         self.compute_func: Optional[Callable] = None
         from pixeltable import exprs
         if computed_with is not None:
             value_expr = exprs.Expr.from_object(computed_with)
             if value_expr is None:
```

### Comparing `pixeltable-0.2.3/pixeltable/catalog/dir.py` & `pixeltable-0.2.4/pixeltable/catalog/dir.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/catalog/globals.py` & `pixeltable-0.2.4/pixeltable/catalog/globals.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/catalog/insertable_table.py` & `pixeltable-0.2.4/pixeltable/catalog/insertable_table.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/catalog/named_function.py` & `pixeltable-0.2.4/pixeltable/catalog/named_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/catalog/path.py` & `pixeltable-0.2.4/pixeltable/catalog/path.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/catalog/path_dict.py` & `pixeltable-0.2.4/pixeltable/catalog/path_dict.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/catalog/schema_object.py` & `pixeltable-0.2.4/pixeltable/catalog/schema_object.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/catalog/table.py` & `pixeltable-0.2.4/pixeltable/catalog/table.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/catalog/table_version.py` & `pixeltable-0.2.4/pixeltable/catalog/table_version.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/catalog/table_version_path.py` & `pixeltable-0.2.4/pixeltable/catalog/table_version_path.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/catalog/view.py` & `pixeltable-0.2.4/pixeltable/catalog/view.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/client.py` & `pixeltable-0.2.4/pixeltable/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from typing import List, Optional, Dict, Type, Any, Union
 import pandas as pd
 import logging
 import dataclasses
-from uuid import UUID
-from collections import defaultdict
 
 import sqlalchemy as sql
 import sqlalchemy.orm as orm
 
+import pixeltable
 from pixeltable.metadata import schema
 from pixeltable.env import Env
 import pixeltable.func as func
 import pixeltable.catalog as catalog
 from pixeltable import exceptions as excs
 from pixeltable.exprs import Predicate
 from pixeltable.iterators import ComponentIterator
 
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    import datasets
+
 __all__ = [
     'Client',
 ]
 
 
 _logger = logging.getLogger('pixeltable')
 
@@ -151,14 +154,81 @@
 
         tbl = catalog.InsertableTable.create(
             dir._id, path.name, schema, primary_key=primary_key, num_retained_versions=num_retained_versions, comment=comment)
         self.catalog.paths[path] = tbl
         _logger.info(f'Created table `{path_str}`.')
         return tbl
 
+    def import_parquet(
+        self,
+        table_path: str,
+        *,
+        parquet_path: str,
+        schema_override: Optional[Dict[str, Any]] = None,
+        **kwargs,
+    ) -> catalog.InsertableTable:
+        """Create a new `InsertableTable` from a Parquet file or set of files. Requires pyarrow to be installed.
+        Args:
+            path_str: Path to the table within pixeltable.
+            parquet_path: Path to an individual Parquet file or directory of Parquet files.
+            schema_override: Optional dictionary mapping column names to column type to override the default
+                            schema inferred from the Parquet file. The column type should be a pixeltable ColumnType.
+                            For example, {'col_vid': VideoType()}, rather than {'col_vid': StringType()}.
+                            Any fields not provided explicitly will map to types with `pixeltable.utils.parquet.parquet_schema_to_pixeltable_schema`
+            kwargs: Additional arguments to pass to `Client.create_table`.
+
+        Returns:
+            The newly created table. The table will have loaded the data from the Parquet file(s).
+        """
+        from pixeltable.utils import parquet
+
+        return parquet.import_parquet(
+            self,
+            table_path=table_path,
+            parquet_path=parquet_path,
+            schema_override=schema_override,
+            **kwargs,
+        )
+
+    def import_huggingface_dataset(
+        self,
+        table_path: str,
+        dataset: Union['datasets.Dataset', 'datasets.DatasetDict'],
+        *,
+        column_name_for_split: Optional[str] = 'split',
+        schema_override: Optional[Dict[str, Any]] = None,
+        **kwargs
+    ) -> catalog.InsertableTable:
+        """Create a new `InsertableTable` from a Huggingface dataset, or dataset dict with multiple splits.
+            Requires datasets library to be installed.
+
+        Args:
+            path_str: Path to the table.
+            dataset: Huggingface datasts.Dataset or datasts.DatasetDict to insert into the table.
+            column_name_for_split: column name to use for split information. If None, no split information will be stored.
+            schema_override: Optional dictionary mapping column names to column type to override the corresponding defaults from
+            `pixeltable.utils.hf_datasets.huggingface_schema_to_pixeltable_schema`. The column type should be a pixeltable ColumnType.
+            For example, {'col_vid': VideoType()}, rather than {'col_vid': StringType()}.
+
+            kwargs: Additional arguments to pass to `create_table`.
+
+        Returns:
+            The newly created table. The table will have loaded the data from the dataset.
+        """
+        from pixeltable.utils import hf_datasets
+
+        return hf_datasets.import_huggingface_dataset(
+            self,
+            table_path,
+            dataset,
+            column_name_for_split=column_name_for_split,
+            schema_override=schema_override,
+            **kwargs,
+        )
+
     def create_view(
             self, path_str: str, base: catalog.Table, *, schema: Optional[Dict[str, Any]] = None,
             filter: Optional[Predicate] = None,
             is_snapshot: bool = False, iterator_class: Optional[Type[ComponentIterator]] = None,
             iterator_args: Optional[Dict[str, Any]] = None, num_retained_versions: int = 10, comment: str = '',
             ignore_errors: bool = False) -> catalog.View:
         """Create a new `View`.
```

### Comparing `pixeltable-0.2.3/pixeltable/dataframe.py` & `pixeltable-0.2.4/pixeltable/dataframe.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/env.py` & `pixeltable-0.2.4/pixeltable/env.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,32 @@
 from __future__ import annotations
+
 import datetime
-import os
-from typing import Optional, Dict, Any, List
-from pathlib import Path
-import sqlalchemy as sql
-import uuid
+import glob
+import http.server
 import importlib
 import importlib.util
-
-import http.server
+import logging
+import os
 import socketserver
+import sys
 import threading
 import typing
 import uuid
 from pathlib import Path
-from typing import Optional, Dict, Any, List
+from typing import Callable, Optional, Dict, Any, List
 
+import pgserver
+import sqlalchemy as sql
 import yaml
 from sqlalchemy_utils.functions import database_exists, create_database, drop_database
-import pgserver
-import logging
-import sys
-import glob
 
-from pixeltable import metadata
 import pixeltable.exceptions as excs
+from pixeltable import metadata
 
-if typing.TYPE_CHECKING:
-    import openai
 
 class Env:
     """
     Store for runtime globals.
     """
     _instance: Optional[Env] = None
     _log_fmt_str = '%(asctime)s %(levelname)s %(name)s %(filename)s:%(lineno)d: %(message)s'
@@ -55,20 +50,20 @@
         self._db_server: Optional[pgserver.PostgresServer] = None
         self._db_url: Optional[str] = None
 
         # info about installed packages that are utilized by some parts of the code;
         # package name -> version; version == []: package is installed, but we haven't determined the version yet
         self._installed_packages: Dict[str, Optional[List[int]]] = {}
         self._nos_client: Optional[Any] = None
-        self._openai_client: Optional['openai.OpenAI'] = None
-        self._has_together_client: bool = False
         self._spacy_nlp: Optional[Any] = None  # spacy.Language
         self._httpd: Optional[socketserver.TCPServer] = None
         self._http_address: Optional[str] = None
 
+        self._registered_clients: dict[str, Any] = {}
+
         # logging-related state
         self._logger = logging.getLogger('pixeltable')
         self._logger.setLevel(logging.DEBUG)  # allow everything to pass, we filter in _log_filter()
         self._logger.propagate = False
         self._logger.addFilter(self._log_filter)
         self._default_log_level = logging.INFO
         self._logfilename: Optional[str] = None
@@ -252,39 +247,40 @@
             # it's already been created
             return
         except ImportError:
             pass
         from pixeltable.functions.util import create_nos_modules
         _ = create_nos_modules()
 
-    def _create_openai_client(self) -> None:
-        if not self.is_installed_package('openai'):
-            raise excs.Error('OpenAI client not initialized (cannot find package `openai`: `pip install openai`?)')
-        import openai
-        if 'openai' in self._config and 'api_key' in self._config['openai']:
-            api_key = self._config['openai']['api_key']
-        else:
-            api_key = os.environ.get('OPENAI_API_KEY')
-        if api_key is None or api_key == '':
-            raise excs.Error('OpenAI client not initialized (no API key configured).')
-        self._openai_client = openai.OpenAI(api_key=api_key)
-        self._logger.info('Initialized OpenAI client.')
-
-    def _create_together_client(self) -> None:
-        if 'together' in self._config and 'api_key' in self._config['together']:
-            api_key = self._config['together']['api_key']
+    def get_client(self, name: str, init: Callable, environ: Optional[str] = None) -> Any:
+        """
+        Gets the client with the specified name, using `init` to construct one if necessary.
+
+        - name: The name of the client
+        - init: A `Callable` with signature `fn(api_key: str) -> Any` that constructs a client object
+        - environ: The name of the environment variable to use for the API key, if no API key is found in config
+            (defaults to f'{name.upper()}_API_KEY')
+        """
+        if name in self._registered_clients:
+            return self._registered_clients[name]
+
+        if environ is None:
+            environ = f'{name.upper()}_API_KEY'
+
+        if name in self._config and 'api_key' in self._config[name]:
+            api_key = self._config[name]['api_key']
         else:
-            api_key = os.environ.get('TOGETHER_API_KEY')
+            api_key = os.environ.get(environ)
         if api_key is None or api_key == '':
-            self._logger.info('Together client not initialized (no API key configured).')
-            return
-        import together
-        self._logger.info('Initializing Together client.')
-        together.api_key = api_key
-        self._has_together_client = True
+            raise excs.Error(f'`{name}` client not initialized (no API key configured).')
+
+        client = init(api_key)
+        self._registered_clients[name] = client
+        self._logger.info(f'Initialized `{name}` client.')
+        return client
 
     def _start_web_server(self) -> None:
         """
         The http server root is the file system root.
         eg: /home/media/foo.mp4 is located at http://127.0.0.1:{port}/home/media/foo.mp4
         This arrangement enables serving media hosted within _home,
         as well as external media inserted into pixeltable or produced by pixeltable.
@@ -315,29 +311,28 @@
     def _check_installed_packages(self) -> None:
         def check(package: str) -> None:
             if importlib.util.find_spec(package) is not None:
                 self._installed_packages[package] = []
             else:
                 self._installed_packages[package] = None
 
+        check('datasets')
         check('torch')
         check('torchvision')
         check('transformers')
         check('sentence_transformers')
         check('boto3')
         check('pyarrow')
         check('spacy')  # TODO: deal with en-core-web-sm
         if self.is_installed_package('spacy'):
             import spacy
             self._spacy_nlp = spacy.load('en_core_web_sm')
         check('tiktoken')
         check('openai')
         check('together')
-        if self.is_installed_package('together'):
-            self._create_together_client()
         check('fireworks')
         check('nos')
         if self.is_installed_package('nos'):
             self._create_nos_client()
 
     def require_package(self, package: str, min_version: Optional[List[int]] = None) -> None:
         assert package in self._installed_packages
@@ -396,21 +391,10 @@
         return self._sa_engine
 
     @property
     def nos_client(self) -> Any:
         return self._nos_client
 
     @property
-    def openai_client(self) -> 'openai.OpenAI':
-        if self._openai_client is None:
-            self._create_openai_client()
-        assert self._openai_client is not None
-        return self._openai_client
-
-    @property
-    def has_together_client(self) -> bool:
-        return self._has_together_client
-
-    @property
     def spacy_nlp(self) -> Any:
         assert self._spacy_nlp is not None
         return self._spacy_nlp
```

### Comparing `pixeltable-0.2.3/pixeltable/exec/aggregation_node.py` & `pixeltable-0.2.4/pixeltable/exec/aggregation_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exec/cache_prefetch_node.py` & `pixeltable-0.2.4/pixeltable/exec/cache_prefetch_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exec/component_iteration_node.py` & `pixeltable-0.2.4/pixeltable/exec/component_iteration_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exec/data_row_batch.py` & `pixeltable-0.2.4/pixeltable/exec/data_row_batch.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exec/exec_context.py` & `pixeltable-0.2.4/pixeltable/exec/exec_context.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exec/exec_node.py` & `pixeltable-0.2.4/pixeltable/exec/exec_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exec/expr_eval_node.py` & `pixeltable-0.2.4/pixeltable/exec/expr_eval_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exec/in_memory_data_node.py` & `pixeltable-0.2.4/pixeltable/exec/in_memory_data_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exec/media_validation_node.py` & `pixeltable-0.2.4/pixeltable/exec/media_validation_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exec/sql_scan_node.py` & `pixeltable-0.2.4/pixeltable/exec/sql_scan_node.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exprs/__init__.py` & `pixeltable-0.2.4/pixeltable/exprs/__init__.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exprs/arithmetic_expr.py` & `pixeltable-0.2.4/pixeltable/exprs/arithmetic_expr.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exprs/array_slice.py` & `pixeltable-0.2.4/pixeltable/exprs/array_slice.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exprs/column_property_ref.py` & `pixeltable-0.2.4/pixeltable/exprs/column_property_ref.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exprs/column_ref.py` & `pixeltable-0.2.4/pixeltable/exprs/column_ref.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exprs/comparison.py` & `pixeltable-0.2.4/pixeltable/exprs/comparison.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exprs/compound_predicate.py` & `pixeltable-0.2.4/pixeltable/exprs/compound_predicate.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exprs/data_row.py` & `pixeltable-0.2.4/pixeltable/exprs/data_row.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exprs/expr.py` & `pixeltable-0.2.4/pixeltable/exprs/expr.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exprs/expr_set.py` & `pixeltable-0.2.4/pixeltable/exprs/expr_set.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exprs/function_call.py` & `pixeltable-0.2.4/pixeltable/exprs/function_call.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exprs/globals.py` & `pixeltable-0.2.4/pixeltable/exprs/globals.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exprs/image_member_access.py` & `pixeltable-0.2.4/pixeltable/exprs/image_member_access.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exprs/image_similarity_predicate.py` & `pixeltable-0.2.4/pixeltable/exprs/image_similarity_predicate.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exprs/inline_array.py` & `pixeltable-0.2.4/pixeltable/exprs/inline_array.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exprs/inline_dict.py` & `pixeltable-0.2.4/pixeltable/exprs/inline_dict.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exprs/is_null.py` & `pixeltable-0.2.4/pixeltable/exprs/is_null.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exprs/json_mapper.py` & `pixeltable-0.2.4/pixeltable/exprs/json_mapper.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exprs/json_path.py` & `pixeltable-0.2.4/pixeltable/exprs/json_path.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exprs/literal.py` & `pixeltable-0.2.4/pixeltable/exprs/literal.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exprs/object_ref.py` & `pixeltable-0.2.4/pixeltable/exprs/object_ref.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exprs/predicate.py` & `pixeltable-0.2.4/pixeltable/exprs/predicate.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exprs/row_builder.py` & `pixeltable-0.2.4/pixeltable/exprs/row_builder.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exprs/rowid_ref.py` & `pixeltable-0.2.4/pixeltable/exprs/rowid_ref.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exprs/type_cast.py` & `pixeltable-0.2.4/pixeltable/exprs/type_cast.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/exprs/variable.py` & `pixeltable-0.2.4/pixeltable/exprs/variable.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/func/aggregate_function.py` & `pixeltable-0.2.4/pixeltable/func/aggregate_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/func/batched_function.py` & `pixeltable-0.2.4/pixeltable/func/batched_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/func/callable_function.py` & `pixeltable-0.2.4/pixeltable/func/callable_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/func/expr_template_function.py` & `pixeltable-0.2.4/pixeltable/func/expr_template_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/func/function.py` & `pixeltable-0.2.4/pixeltable/func/function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/func/function_registry.py` & `pixeltable-0.2.4/pixeltable/func/function_registry.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/func/globals.py` & `pixeltable-0.2.4/pixeltable/func/globals.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/func/nos_function.py` & `pixeltable-0.2.4/pixeltable/func/nos_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/func/signature.py` & `pixeltable-0.2.4/pixeltable/func/signature.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/func/udf.py` & `pixeltable-0.2.4/pixeltable/func/udf.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/functions/__init__.py` & `pixeltable-0.2.4/pixeltable/functions/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import pixeltable.env as env
 import pixeltable.func as func
 # import all standard function modules here so they get registered with the FunctionRegistry
 import pixeltable.functions.pil.image
 from pixeltable import exprs
 from pixeltable.type_system import IntType, ColumnType, FloatType, ImageType, VideoType
 # automatically import all submodules so that the udfs get registered
-from . import image, string, video, openai, together, fireworks, huggingface
+from . import image, string, video, huggingface
 
 # TODO: remove and replace calls with astype()
 def cast(expr: exprs.Expr, target_type: ColumnType) -> exprs.Expr:
     expr.col_type = target_type
     return expr
 
 @func.uda(
```

### Comparing `pixeltable-0.2.3/pixeltable/functions/eval.py` & `pixeltable-0.2.4/pixeltable/functions/eval.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/functions/huggingface.py` & `pixeltable-0.2.4/pixeltable/functions/huggingface.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/functions/pil/image.py` & `pixeltable-0.2.4/pixeltable/functions/pil/image.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/functions/string.py` & `pixeltable-0.2.4/pixeltable/functions/string.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/functions/util.py` & `pixeltable-0.2.4/pixeltable/functions/util.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/functions/video.py` & `pixeltable-0.2.4/pixeltable/functions/video.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/iterators/base.py` & `pixeltable-0.2.4/pixeltable/iterators/base.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/iterators/document.py` & `pixeltable-0.2.4/pixeltable/iterators/document.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/iterators/video.py` & `pixeltable-0.2.4/pixeltable/iterators/video.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/metadata/__init__.py` & `pixeltable-0.2.4/pixeltable/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/metadata/converters/convert_10.py` & `pixeltable-0.2.4/pixeltable/metadata/converters/convert_10.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/metadata/schema.py` & `pixeltable-0.2.4/pixeltable/metadata/schema.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/plan.py` & `pixeltable-0.2.4/pixeltable/plan.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/store.py` & `pixeltable-0.2.4/pixeltable/store.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/tests/conftest.py` & `pixeltable-0.2.4/pixeltable/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,24 +76,24 @@
 
 
 @pytest.fixture(scope='function')
 def test_tbl(test_client: pxt.Client) -> catalog.Table:
     return create_test_tbl(test_client)
 
 # @pytest.fixture(scope='function')
-# def test_stored_fn(test_client: pt.Client) -> pt.Function:
-#     @pt.udf(return_type=pt.IntType(), param_types=[pt.IntType()])
+# def test_stored_fn(test_client: pxt.Client) -> pxt.Function:
+#     @pxt.udf(return_type=pxt.IntType(), param_types=[pxt.IntType()])
 #     def test_fn(x):
 #         return x + 1
 #     test_client.create_function('test_fn', test_fn)
 #     return test_fn
 
 @pytest.fixture(scope='function')
 def test_tbl_exprs(test_tbl: catalog.Table) -> List[exprs.Expr]:
-#def test_tbl_exprs(test_tbl: catalog.Table, test_stored_fn: pt.Function) -> List[exprs.Expr]:
+#def test_tbl_exprs(test_tbl: catalog.Table, test_stored_fn: pxt.Function) -> List[exprs.Expr]:
 
     t = test_tbl
     return [
         t.c1,
         t.c7['*'].f1,
         exprs.Literal('test'),
         exprs.InlineDict({
@@ -152,15 +152,15 @@
         img_t.img.fileurl,
         img_t.img.localpath,
     ]
 
 # TODO: why does this not work with a session scope? (some user tables don't get created with create_all())
 #@pytest.fixture(scope='session')
 #def indexed_img_tbl(init_env: None) -> catalog.Table:
-#    cl = pt.Client()
+#    cl = pxt.Client()
 #    db = cl.create_db('test_indexed')
 @pytest.fixture(scope='function')
 def indexed_img_tbl(test_client: pxt.Client) -> catalog.Table:
     skip_test_if_not_installed('nos')
     cl = test_client
     schema = {
         'img': { 'type': ImageType(nullable=False), 'indexed': True },
```

### Comparing `pixeltable-0.2.3/pixeltable/tests/test_audio.py` & `pixeltable-0.2.4/pixeltable/tests/test_audio.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/tests/test_catalog.py` & `pixeltable-0.2.4/pixeltable/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/tests/test_client.py` & `pixeltable-0.2.4/pixeltable/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/tests/test_component_view.py` & `pixeltable-0.2.4/pixeltable/tests/test_component_view.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/tests/test_dataframe.py` & `pixeltable-0.2.4/pixeltable/tests/test_dataframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         res3 = t.where(t.c2 < 10).select(c1=t.c1, c2=t.c2, c3=t.c3).show(0)
         assert res1 == res3
 
         res4 = t.where(t.c2 < 10).select(t.c1, c2=t.c2, c3=t.c3).show(0)
         assert res1 == res4
 
         _ = t.where(t.c2 < 10).select(t.c2, t.c2).show(0) # repeated name no error
-        
+
         # duplicate select list
         with pytest.raises(excs.Error) as exc_info:
             _ = t.select(t.c1).select(t.c2).show(0)
         assert 'already specified' in str(exc_info.value)
 
         # invalid expr in select list: Callable is not a valid literal
         with pytest.raises(TypeError) as exc_info:
@@ -216,15 +216,15 @@
         df = t.where(t.row_id < 1)
         assert df.count() > 0
         ds = df.to_pytorch_dataset()
         type_dict = dict(zip(df.get_column_names(),df.get_column_types()))
         for tup in ds:
             for col in df.get_column_names():
                 assert col in tup
-        
+
             arrval = tup['c_array']
             assert isinstance(arrval, np.ndarray)
             col_type = type_dict['c_array']
             assert arrval.dtype == col_type.numpy_dtype()
             assert arrval.shape == col_type.shape
             assert arrval.dtype == np.float32
             assert arrval.flags["WRITEABLE"], 'required by pytorch collate function'
@@ -300,15 +300,15 @@
         """
         skip_test_if_not_installed('torch')
         import torch.utils.data
         @pxt.udf(param_types=[pxt.JsonType()], return_type=pxt.JsonType())
         def restrict_json_for_default_collate(obj):
             keys = ['id', 'label', 'iscrowd', 'bounding_box']
             return {k: obj[k] for k in keys}
-        
+
         t = all_datatypes_tbl
         df = t.select(
             t.row_id,
             t.c_int,
             t.c_float,
             t.c_bool,
             t.c_timestamp,
@@ -366,15 +366,15 @@
 
         def _get_mtimes(dir: Path):
             return {p.name: p.stat().st_mtime for p in dir.iterdir()}
 
         #  check result cached
         ds1 = t.to_pytorch_dataset(image_format='pt')
         ds1_mtimes = _get_mtimes(ds1.path)
-        
+
         ds2 = t.to_pytorch_dataset(image_format='pt')
         ds2_mtimes = _get_mtimes(ds2.path)
         assert ds2.path == ds1.path, 'result should be cached'
         assert ds2_mtimes == ds1_mtimes, 'no extra file system work should have occurred'
 
         # check invalidation on insert
         t_size = t.count()
```

### Comparing `pixeltable-0.2.3/pixeltable/tests/test_dirs.py` & `pixeltable-0.2.4/pixeltable/tests/test_dirs.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/tests/test_document.py` & `pixeltable-0.2.4/pixeltable/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/tests/test_exprs.py` & `pixeltable-0.2.4/pixeltable/tests/test_exprs.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/tests/test_function.py` & `pixeltable-0.2.4/pixeltable/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/tests/test_migration.py` & `pixeltable-0.2.4/pixeltable/tests/test_migration.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/tests/test_nos.py` & `pixeltable-0.2.4/pixeltable/tests/test_nos.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/tests/test_snapshot.py` & `pixeltable-0.2.4/pixeltable/tests/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/tests/test_table.py` & `pixeltable-0.2.4/pixeltable/tests/test_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 import random
 from typing import List, Tuple
 
 import PIL
 import cv2
 import numpy as np
 import pandas as pd
+import pathlib
 import pytest
 
 import pixeltable as pxt
 import pixeltable.functions as ptf
 from pixeltable import catalog
 from pixeltable import exceptions as excs
 from pixeltable.iterators import FrameIterator
 from pixeltable.tests.utils import \
     make_tbl, create_table_data, read_data_file, get_video_files, get_audio_files, get_image_files, get_documents, \
-    assert_resultset_eq
+    assert_resultset_eq, assert_hf_dataset_equal, make_test_arrow_table
 from pixeltable.tests.utils import skip_test_if_not_installed
 from pixeltable.type_system import \
     StringType, IntType, FloatType, TimestampType, ImageType, VideoType, JsonType, BoolType, ArrayType, AudioType, \
     DocumentType
 from pixeltable.utils.filecache import FileCache
 from pixeltable.utils.media_store import MediaStore
 
-
 class TestTable:
     # exc for a % 10 == 0
     @pxt.udf(return_type=FloatType(), param_types=[IntType()])
     def f1(a: int) -> float:
         return a / (a % 10)
 
     # exception for a == None; this should not get triggered
@@ -112,14 +112,108 @@
         tbl.comment = new_comment
         assert tbl.comment == new_comment
         tbl.revert()
         assert tbl.comment == comment
         tbl.revert()
         assert tbl.num_retained_versions == num_retained_versions
 
+    def test_import_parquet(self, test_client: pxt.Client, tmp_path: pathlib.Path) -> None:
+        skip_test_if_not_installed('pyarrow')
+        import pyarrow as pa
+        from pixeltable.utils.arrow import iter_tuples
+
+        parquet_dir = tmp_path / 'test_data'
+        parquet_dir.mkdir()
+        make_test_arrow_table(parquet_dir)
+
+        tab = test_client.import_parquet('test_parquet', parquet_path=str(parquet_dir))
+        assert 'test_parquet' in test_client.list_tables()
+        assert tab is not None
+        num_elts = tab.count()
+        arrow_tab: pa.Table = pa.parquet.read_table(str(parquet_dir))
+        assert num_elts == arrow_tab.num_rows
+        assert set(tab.column_names()) == set(arrow_tab.column_names)
+
+        result_set = tab.order_by(tab.c_id).collect()
+        column_types = tab.column_types()
+
+        for tup, arrow_tup in zip(result_set, iter_tuples(arrow_tab)):
+            assert tup['c_id'] == arrow_tup['c_id']
+            for col, val in tup.items():
+                if val is None:
+                    assert arrow_tup[col] is None
+                    continue
+
+                if column_types[col].is_array_type():
+                    assert (val == arrow_tup[col]).all()
+                else:
+                    assert val == arrow_tup[col]
+
+    def test_import_huggingface_dataset(self, test_client: pxt.Client, tmp_path: pathlib.Path) -> None:
+        skip_test_if_not_installed('datasets')
+        import datasets
+
+        test_cases = [
+            # { # includes a timestamp. 20MB for specific slice
+            # Disbled this test case because download is failing, and its not critical.
+            #     'dataset_name': 'c4',
+            #     # see https://huggingface.co/datasets/allenai/c4/blob/main/realnewslike/c4-train.00000-of-00512.json.gz
+            #     'dataset': datasets.load_dataset(
+            #         "allenai/c4",
+            #         data_dir="realnewslike",
+            #         data_files="c4-train.00000-of-00512.json.gz",
+            #         split='train[:1000]',
+            #         cache_dir=tmp_path
+            #     ),
+            # },
+            {  # includes an embedding (array type), common in a few RAG datasets.
+                'dataset_name': 'cohere_wikipedia',
+                'dataset': datasets.load_dataset("Cohere/wikipedia-2023-11-embed-multilingual-v3",
+                                                 data_dir='cr').select_columns(['url', 'title', 'text', 'emb']),
+                # column with name `_id`` is not currently allowed by pixeltable rules,
+                # so filter out that column.
+                # cr subdir has a small number of rows, avoid running out of space in CI runner
+                # see https://huggingface.co/datasets/Cohere/wikipedia-2023-11-embed-multilingual-v3/tree/main/cr
+                'schema_override': {'emb': ArrayType((1024,), dtype=FloatType(), nullable=False)}
+            },
+            # example of dataset dictionary with multiple splits
+            {
+                'dataset_name': 'rotten_tomatoes',
+                'dataset': datasets.load_dataset("rotten_tomatoes"),
+            },
+        ]
+
+        # test a column name for splits other than the default of 'split'
+        split_column_name = 'my_split_col'
+        for rec in test_cases:
+            dataset_name = rec['dataset_name']
+            hf_dataset = rec['dataset']
+
+            tab = test_client.import_huggingface_dataset(
+                dataset_name,
+                hf_dataset,
+                column_name_for_split=split_column_name,
+                schema_override=rec.get('schema_override', None),
+            )
+            if isinstance(hf_dataset, datasets.Dataset):
+                assert_hf_dataset_equal(hf_dataset, tab.df(), split_column_name)
+            elif isinstance(hf_dataset, datasets.DatasetDict):
+                assert tab.count() == sum(hf_dataset.num_rows.values())
+                assert split_column_name in tab.column_names()
+
+                for dataset_name in hf_dataset:
+                    df = tab.where(tab.my_split_col == dataset_name)
+                    assert_hf_dataset_equal(hf_dataset[dataset_name], df, split_column_name)
+            else:
+                assert False
+
+        with pytest.raises(excs.Error) as exc_info:
+            test_client.import_huggingface_dataset('test', {})
+        assert 'type(dataset)' in str(exc_info.value)
+
     def test_image_table(self, test_client: pxt.Client) -> None:
         n_sample_rows = 20
         cl = test_client
         schema = {
             'img': ImageType(nullable=False),
             'category': StringType(nullable=False),
             'split': StringType(nullable=False),
@@ -529,14 +623,23 @@
         # bad array literal
         cl.drop_table('test1', ignore_errors=True)
         t = cl.create_table('test1', {'c5': ArrayType((2, 3), dtype=IntType(), nullable=False)})
         with pytest.raises(excs.Error) as exc_info:
             t.insert(c5=np.ndarray((3, 2)))
         assert 'expected ndarray((2, 3)' in str(exc_info.value)
 
+    def test_insert_string_with_null(self, test_client: pxt.Client) -> None:
+        cl = test_client
+        t = cl.create_table('test', {'c1': StringType()})
+
+        t.insert([{'c1': 'this is a python\x00string'}])
+        assert t.count() == 1
+        for tup in t.df().collect():
+            assert tup['c1'] == 'this is a python string'
+
     def test_query(self, test_client: pxt.Client) -> None:
         skip_test_if_not_installed('boto3')
         cl = test_client
         col_names = ['c1', 'c2', 'c3', 'c4', 'c5']
         t = make_tbl(cl, 'test', col_names)
         rows = create_table_data(t)
         t.insert(rows)
```

### Comparing `pixeltable-0.2.3/pixeltable/tests/test_transactional_directory.py` & `pixeltable-0.2.4/pixeltable/tests/test_transactional_directory.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/tests/test_types.py` & `pixeltable-0.2.4/pixeltable/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/tests/test_video.py` & `pixeltable-0.2.4/pixeltable/tests/test_video.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/tests/test_view.py` & `pixeltable-0.2.4/pixeltable/tests/test_view.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/tests/utils.py` & `pixeltable-0.2.4/pixeltable/tests/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 import datetime
 import glob
 import json
 import os
+from collections import namedtuple
 from pathlib import Path
-from typing import Dict, Any, List, Optional
+from typing import Any, Dict, List, Optional, Set
 
 import numpy as np
 import pandas as pd
 import pytest
 
 import pixeltable as pxt
 import pixeltable.type_system as ts
 from pixeltable import catalog
+from pixeltable.catalog.globals import UpdateStatus
 from pixeltable.dataframe import DataFrameResultSet
 from pixeltable.env import Env
-from pixeltable.type_system import \
-    ColumnType, StringType, IntType, FloatType, ArrayType, BoolType, TimestampType, JsonType, ImageType, VideoType
-
-
+from pixeltable.type_system import (
+    ArrayType,
+    BoolType,
+    ColumnType,
+    FloatType,
+    ImageType,
+    IntType,
+    JsonType,
+    StringType,
+    TimestampType,
+    VideoType,
+)
 
 
 def make_default_type(t: ColumnType.Type) -> ColumnType:
     if t == ColumnType.Type.STRING:
         return StringType()
     if t == ColumnType.Type.INT:
         return IntType()
@@ -262,24 +272,137 @@
     tests_dir = os.path.dirname(__file__)
     path = glob.glob(f'{tests_dir}/**/jeopardy.json', recursive=True)[0]
     with open(path, 'r', encoding='utf8') as f:
         questions_list = json.load(f)
     # this dataset contains \' around the questions
     return [q['question'].replace("'", '') for q in questions_list[:n]]
 
+
 def assert_resultset_eq(r1: DataFrameResultSet, r2: DataFrameResultSet) -> None:
     assert len(r1) == len(r2)
     assert len(r1.column_names()) == len(r2.column_names())  # we don't care about the actual column names
     r1_pd = r1.to_pandas()
     r2_pd = r2.to_pandas()
     for i in range(len(r1.column_names())):
         # only compare column values
         s1 = r1_pd.iloc[:, i]
         s2 = r2_pd.iloc[:, i]
         if s1.dtype == np.float64:
             assert np.allclose(s1, s2)
         else:
             assert s1.equals(s2)
 
+
 def skip_test_if_not_installed(package) -> None:
     if not Env.get().is_installed_package(package):
         pytest.skip(f'Package `{package}` is not installed.')
+
+
+def validate_update_status(status: UpdateStatus, expected_rows: Optional[int] = None) -> None:
+    assert status.num_excs == 0
+    if expected_rows is not None:
+        assert status.num_rows == expected_rows
+
+
+def make_test_arrow_table(output_path: Path) -> None:
+    import pyarrow as pa
+
+    value_dict = {
+        'c_id': [1, 2, 3, 4, 5],
+        'c_int64': [-10, -20, -30, -40, None],
+        'c_int32': [-1, -2, -3, -4, None],
+        'c_float32': [1.1, 2.2, 3.3, 4.4, None],
+        'c_string': ['aaa', 'bbb', 'ccc', 'ddd', None],
+        'c_boolean': [True, False, True, False, None],
+        'c_timestamp': [
+            datetime.datetime(2012, 1, 1, 12, 0, 0, 25),
+            datetime.datetime(2012, 1, 2, 12, 0, 0, 25),
+            datetime.datetime(2012, 1, 3, 12, 0, 0, 25),
+            datetime.datetime(2012, 1, 4, 12, 0, 0, 25),
+            None,
+        ],
+        # The pyarrow fixed_shape_tensor type does not support NULLs (currently can write them but not read them)
+        # So, no nulls in this column
+        'c_array_float32': [
+            [
+                1.0,
+                2.0,
+            ],
+            [
+                10.0,
+                20.0,
+            ],
+            [
+                100.0,
+                200.0,
+            ],
+            [
+                1000.0,
+                2000.0,
+            ],
+            [10000.0, 20000.0],
+        ],
+    }
+
+    arr_size = len(value_dict['c_array_float32'][0])
+    tensor_type = pa.fixed_shape_tensor(pa.float32(), (arr_size,))
+
+    schema = pa.schema(
+        [
+            ('c_id', pa.int32()),
+            ('c_int64', pa.int64()),
+            ('c_int32', pa.int32()),
+            ('c_float32', pa.float32()),
+            ('c_string', pa.string()),
+            ('c_boolean', pa.bool_()),
+            ('c_timestamp', pa.timestamp('us')),
+            ('c_array_float32', tensor_type),
+        ]
+    )
+
+    test_table = pa.Table.from_pydict(value_dict, schema=schema)
+    pa.parquet.write_table(test_table, str(output_path / 'test.parquet'))
+
+
+def assert_hf_dataset_equal(hf_dataset: 'datasets.Dataset', df: pxt.DataFrame, split_column_name: str) -> None:
+    import datasets
+    assert df.count() == hf_dataset.num_rows
+    assert set(df.get_column_names()) == (set(hf_dataset.features.keys()) | {split_column_name})
+
+    # immutable so we can use it as in a set
+    DatasetTuple = namedtuple('DatasetTuple', ' '.join(hf_dataset.features.keys()))
+    acc_dataset: Set[DatasetTuple] = set()
+    for tup in hf_dataset:
+        immutable_tup = {}
+        for k in tup:
+            if isinstance(tup[k], list):
+                immutable_tup[k] = tuple(tup[k])
+            else:
+                immutable_tup[k] = tup[k]
+
+        acc_dataset.add(DatasetTuple(**immutable_tup))
+
+    for tup in df.collect():
+        assert tup[split_column_name] in hf_dataset.split._name
+
+        encoded_tup = {}
+        for column_name, value in tup.items():
+            if column_name == split_column_name:
+                continue
+            feature_type = hf_dataset.features[column_name]
+            if isinstance(feature_type, datasets.ClassLabel):
+                assert value in feature_type.names
+                # must use the index of the class label as the value to
+                # compare with dataset iteration output.
+                value = feature_type.encode_example(value)
+            elif isinstance(feature_type, datasets.Sequence):
+                assert feature_type.feature.dtype == 'float32', 'may need to add more types'
+                value = tuple([float(x) for x in value])
+
+            encoded_tup[column_name] = value
+
+        check_tup = DatasetTuple(**encoded_tup)
+        assert check_tup in acc_dataset
+
+
+SAMPLE_IMAGE_URL = \
+    'https://raw.githubusercontent.com/pixeltable/pixeltable/master/docs/source/data/images/000000000009.jpg'
```

### Comparing `pixeltable-0.2.3/pixeltable/tool/create_test_db_dump.py` & `pixeltable-0.2.4/pixeltable/tool/create_test_db_dump.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/tool/create_test_video.py` & `pixeltable-0.2.4/pixeltable/tool/create_test_video.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/type_system.py` & `pixeltable-0.2.4/pixeltable/type_system.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 
 import abc
 import datetime
 import enum
 import json
 import typing
 import urllib.parse
-from copy import copy
 from pathlib import Path
-from typing import Any, Optional, Tuple, Dict, Callable, List, Union
+from typing import Any, Optional, Tuple, Dict, Callable, List, Union, Sequence, Mapping
 
 import PIL.Image
 import av
 import numpy as np
 import sqlalchemy as sql
 
 from pixeltable import exceptions as excs
@@ -236,27 +235,46 @@
             except TypeError:
                 return None
         return None
 
 
     @classmethod
     def from_python_type(cls, t: type) -> Optional[ColumnType]:
-        if t in _python_type_to_column_type:
-            return _python_type_to_column_type[t]
-        elif isinstance(t, typing._UnionGenericAlias) and t.__args__[1] is type(None):
-            # `t` is a type of the form Optional[T] (equivalently, Union[T, None]).
-            # We treat it as the underlying type but with nullable=True.
-            if t.__args__[0] in _python_type_to_column_type:
-                underlying = copy(_python_type_to_column_type[t.__args__[0]])
-                underlying.nullable = True
-                return underlying
-
+        if typing.get_origin(t) is typing.Union:
+            union_args = typing.get_args(t)
+            if union_args[1] is type(None):
+                # `t` is a type of the form Optional[T] (equivalently, Union[T, None]).
+                # We treat it as the underlying type but with nullable=True.
+                underlying = cls.from_python_type(union_args[0])
+                if underlying is not None:
+                    underlying.nullable = True
+                    return underlying
+        else:
+            # Discard type parameters to ensure that parameterized types such as `list[T]`
+            # are correctly mapped to Pixeltable types.
+            base = typing.get_origin(t)
+            if base is None:
+                # No type parameters; the base type is just `t` itself
+                base = t
+            if base is str:
+                return StringType()
+            if base is int:
+                return IntType()
+            if base is float:
+                return FloatType()
+            if base is bool:
+                return BoolType()
+            if base is datetime.date or base is datetime.datetime:
+                return TimestampType()
+            if issubclass(base, Sequence) or issubclass(base, Mapping):
+                return JsonType()
+            if issubclass(base, PIL.Image.Image):
+                return ImageType()
         return None
 
-
     def validate_literal(self, val: Any) -> None:
         """Raise TypeError if val is not a valid literal for this type"""
         if val is None:
             if not self.nullable:
                 raise TypeError('Expected non-None value')
             else:
                 return
@@ -379,18 +397,14 @@
             return sql.String
         if self._type == self.Type.JSON:
             return sql.dialects.postgresql.JSONB
         if self._type == self.Type.ARRAY:
             return sql.VARBINARY
         assert False
 
-    @abc.abstractmethod
-    def to_arrow_type(self) -> 'pyarrow.DataType':
-        assert False, f'Have not implemented {self.__class__.__name__} to Arrow'
- 
     @staticmethod
     def no_conversion(v: Any) -> Any:
         """
         Special return value of conversion_fn() that indicates that no conversion is necessary.
         Should not be called
         """
         assert False
@@ -409,17 +423,14 @@
 
     def to_sql(self) -> str:
         assert False
 
     def to_sa_type(self) -> Any:
         assert False
 
-    def to_arrow_type(self) -> 'pyarrow.DataType':
-        assert False
-
     def print_value(self, val: Any) -> str:
         assert False
 
     def _validate_literal(self, val: Any) -> None:
         assert False
 
 class StringType(ColumnType):
@@ -438,40 +449,39 @@
         return convert
 
     def to_sql(self) -> str:
         return 'VARCHAR'
 
     def to_sa_type(self) -> str:
         return sql.String
-    
-    def to_arrow_type(self) -> 'pyarrow.DataType':
-        import pyarrow as pa # pylint: disable=import-outside-toplevel
-        return pa.string()
 
     def print_value(self, val: Any) -> str:
         return f"'{val}'"
 
     def _validate_literal(self, val: Any) -> None:
         if not isinstance(val, str):
             raise TypeError(f'Expected string, got {val.__class__.__name__}')
 
+    def _create_literal(self, val: Any) -> Any:
+        # Replace null byte within python string with space to avoid issues with Postgres.
+        # Use a space to avoid merging words.
+        # TODO(orm): this will also be an issue with JSON inputs, would space still be a good replacement?
+        if isinstance(val, str) and '\x00' in val:
+            return val.replace('\x00', ' ')
+        return val
 
 class IntType(ColumnType):
     def __init__(self, nullable: bool = False):
         super().__init__(self.Type.INT, nullable=nullable)
 
     def to_sql(self) -> str:
         return 'BIGINT'
 
     def to_sa_type(self) -> str:
         return sql.BigInteger
-    
-    def to_arrow_type(self) -> 'pyarrow.DataType':
-        import pyarrow as pa # pylint: disable=import-outside-toplevel
-        return pa.int64() # to be consistent with bigint above
 
     def _validate_literal(self, val: Any) -> None:
         if not isinstance(val, int):
             raise TypeError(f'Expected int, got {val.__class__.__name__}')
 
 
 class FloatType(ColumnType):
@@ -479,18 +489,14 @@
         super().__init__(self.Type.FLOAT, nullable=nullable)
 
     def to_sql(self) -> str:
         return 'FLOAT'
 
     def to_sa_type(self) -> str:
         return sql.Float
-    
-    def to_arrow_type(self) -> 'pyarrow.DataType':
-        import pyarrow as pa
-        return pa.float32()
 
     def _validate_literal(self, val: Any) -> None:
         if not isinstance(val, float):
             raise TypeError(f'Expected float, got {val.__class__.__name__}')
 
     def _create_literal(self, val: Any) -> Any:
         if isinstance(val, int):
@@ -502,18 +508,14 @@
         super().__init__(self.Type.BOOL, nullable=nullable)
 
     def to_sql(self) -> str:
         return 'BOOLEAN'
 
     def to_sa_type(self) -> str:
         return sql.Boolean
-    
-    def to_arrow_type(self) -> 'pyarrow.DataType':
-        import pyarrow as pa # pylint: disable=import-outside-toplevel
-        return pa.bool_()
 
     def _validate_literal(self, val: Any) -> None:
         if not isinstance(val, bool):
             raise TypeError(f'Expected bool, got {val.__class__.__name__}')
 
     def _create_literal(self, val: Any) -> Any:
         if isinstance(val, int):
@@ -525,18 +527,14 @@
         super().__init__(self.Type.TIMESTAMP, nullable=nullable)
 
     def to_sql(self) -> str:
         return 'INTEGER'
 
     def to_sa_type(self) -> str:
         return sql.TIMESTAMP
-    
-    def to_arrow_type(self) -> 'pyarrow.DataType':
-        import pyarrow as pa # pylint: disable=import-outside-toplevel
-        return pa.timestamp('us') # postgres timestamp is microseconds
 
     def _validate_literal(self, val: Any) -> None:
         if not isinstance(val, datetime.datetime) and not isinstance(val, datetime.date):
             raise TypeError(f'Expected datetime.datetime or datetime.date, got {val.__class__.__name__}')
 
     def _create_literal(self, val: Any) -> Any:
         if isinstance(val, str):
@@ -566,18 +564,14 @@
         return cls(type_spec, nullable=d['nullable'])
 
     def to_sql(self) -> str:
         return 'JSONB'
 
     def to_sa_type(self) -> str:
         return sql.dialects.postgresql.JSONB
-    
-    def to_arrow_type(self) -> 'pyarrow.DataType':
-        import pyarrow as pa # pylint: disable=import-outside-toplevel
-        return pa.string() # TODO: weight advantage of pa.struct type.
 
     def print_value(self, val: Any) -> str:
         val_type = self.infer_literal_type(val)
         if val_type == self:
             return str(val)
         return val_type.print_value(val)
 
@@ -665,28 +659,24 @@
         if not self.is_valid_literal(val):
             raise TypeError((
                 f'Expected ndarray({self.shape}, dtype={self.numpy_dtype()}), '
                 f'got ndarray({val.shape}, dtype={val.dtype})'))
 
     def _create_literal(self, val: Any) -> Any:
         if isinstance(val, (list,tuple)):
-            return np.array(val)
+            # map python float to whichever numpy float is
+            # declared for this type, rather than assume float64
+            return np.array(val, dtype=self.numpy_dtype())
         return val
 
     def to_sql(self) -> str:
         return 'BYTEA'
 
     def to_sa_type(self) -> str:
         return sql.LargeBinary
-    
-    def to_arrow_type(self) -> 'pyarrow.DataType':
-        import pyarrow as pa # pylint: disable=import-outside-toplevel
-        if any([n is None for n in self.shape]):
-            raise TypeError(f'Cannot convert array with unknown shape to Arrow')        
-        return pa.fixed_shape_tensor(pa.from_numpy_dtype(self.numpy_dtype()), self.shape)
 
     def numpy_dtype(self) -> np.dtype:
         if self.dtype == self.Type.INT:
             return np.dtype(np.int64)
         if self.dtype == self.Type.FLOAT:
             return np.dtype(np.float32)
         if self.dtype == self.Type.BOOL:
@@ -784,18 +774,14 @@
         return convert
 
     def to_sql(self) -> str:
         return 'VARCHAR'
 
     def to_sa_type(self) -> str:
         return sql.String
-    
-    def to_arrow_type(self) -> 'pyarrow.DataType':
-        import pyarrow as pa # pylint: disable=import-outside-toplevel
-        return pa.binary()
 
     def _validate_literal(self, val: Any) -> None:
         if isinstance(val, PIL.Image.Image):
             return
         self._validate_file_path(val)
 
     def validate_media(self, val: Any) -> None:
@@ -811,18 +797,14 @@
 
     def to_sql(self) -> str:
         # stored as a file path
         return 'VARCHAR'
 
     def to_sa_type(self) -> str:
         return sql.String
-    
-    def to_arrow_type(self) -> 'pyarrow.DataType':
-        import pyarrow as pa # pylint: disable=import-outside-toplevel
-        return pa.string()
 
     def _validate_literal(self, val: Any) -> None:
         self._validate_file_path(val)
 
     def validate_media(self, val: Any) -> None:
         assert isinstance(val, str)
         try:
@@ -850,18 +832,14 @@
     def to_sql(self) -> str:
         # stored as a file path
         return 'VARCHAR'
 
     def to_sa_type(self) -> str:
         return sql.String
 
-    def to_arrow_type(self) -> 'pyarrow.DataType':
-        import pyarrow as pa  # pylint: disable=import-outside-toplevel
-        return pa.string()
-
     def _validate_literal(self, val: Any) -> None:
         self._validate_file_path(val)
 
     def validate_media(self, val: Any) -> None:
         try:
             with av.open(val) as container:
                 if len(container.streams.audio) == 0:
@@ -897,42 +875,21 @@
     def to_sql(self) -> str:
         # stored as a file path
         return 'VARCHAR'
 
     def to_sa_type(self) -> str:
         return sql.String
 
-    def to_arrow_type(self) -> 'pyarrow.DataType':
-        import pyarrow as pa  # pylint: disable=import-outside-toplevel
-        return pa.string()
-
     def _validate_literal(self, val: Any) -> None:
         self._validate_file_path(val)
 
     def validate_media(self, val: Any) -> None:
         assert isinstance(val, str)
         from pixeltable.utils.documents import get_document_handle
         with open(val, 'r', encoding='utf8') as fh:
             try:
                 s = fh.read()
                 dh = get_document_handle(s)
                 if dh is None:
                     raise excs.Error(f'Not a recognized document format: {val}')
             except Exception as e:
                 raise excs.Error(f'Not a recognized document format: {val}') from None
-
-
-# A dictionary mapping various Python types to their respective ColumnTypes.
-# This can be used to infer Pixeltable ColumnTypes from type hints on Python
-# functions. (Since Python functions do not necessarily have type hints, this
-# should always be an optional/convenience inference.)
-_python_type_to_column_type: dict[type, ColumnType] = {
-    str: StringType(),
-    int: IntType(),
-    float: FloatType(),
-    bool: BoolType(),
-    datetime.datetime: TimestampType(),
-    datetime.date: TimestampType(),
-    list: JsonType(),
-    dict: JsonType(),
-    PIL.Image.Image: ImageType()
-}
```

### Comparing `pixeltable-0.2.3/pixeltable/utils/clip.py` & `pixeltable-0.2.4/pixeltable/utils/clip.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/utils/coco.py` & `pixeltable-0.2.4/pixeltable/utils/coco.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/utils/documents.py` & `pixeltable-0.2.4/pixeltable/utils/documents.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/utils/filecache.py` & `pixeltable-0.2.4/pixeltable/utils/filecache.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/utils/media_store.py` & `pixeltable-0.2.4/pixeltable/utils/media_store.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/utils/sql.py` & `pixeltable-0.2.4/pixeltable/utils/sql.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pixeltable/utils/transactional_directory.py` & `pixeltable-0.2.4/pixeltable/utils/transactional_directory.py`

 * *Files identical despite different names*

### Comparing `pixeltable-0.2.3/pyproject.toml` & `pixeltable-0.2.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pixeltable"
-version = "0.2.3"
+version = "0.2.4"
 description = "Pixeltable: The Multimodal AI Data Plane"
 authors = ["Marcel Kornacker <marcelk@gmail.com>"]
 readme = "README.md"
 exclude = [
     ".pytype",
     ".pytest_cache",
     "pixeltable/.pytest_cache",
     "pixeltable/tests/data"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
-numpy = "^1.26"
+numpy = ">=1.26"
 pandas = ">=2.0,<3.0"
-pillow = "^9.4.0"
+pillow = ">=10.0"
 opencv-python-headless = "^4.7.0.68"
 tqdm = "^4.64.1"
 jmespath = "^1.0.1"
 regex = "^2022.10.31"
 cloudpickle = "^2.2.1"
 psycopg2-binary = "^2.9.5"
 psutil = "^5.9.5"
@@ -31,28 +31,30 @@
 sqlalchemy-utils = "^0.41.1"
 pgvector = "^0.2.1"
 av = ">=10.0.0"
 beautifulsoup4 = "^4.0.0"
 requests = "^2.31.0"
 pyyaml = "^6.0.1"
 jinja2 = "^3.1.3"
-pgserver = "0.0.9"
+tenacity = "^8.2"
+pgserver = "0.1.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 # pytest-related
 pytest = "^7.2.1"
 pytest-xdist = {extras = ["psutil"], version = "^3.3.1"}
 coverage = "^7.4"
 # mypy-related
 mypy = "^1.8.0"
-types-pillow = "^10.1.0.2"
+types-pillow = ">=10.0"
 types-pyyaml = "^6.0.1"
+pyarrow-stubs = "^10.0.1.7"
 # linting
 pylint = "^3.1.0"
 ruff = "^0.3.1"
 # jupyter
 notebook = "^7.1.0"
 # mkdocs-related
 mkdocs = "^1.5.3"
@@ -64,22 +66,23 @@
 ipykernel = "^6.27.1"
 nbmake = "^1.4.6"
 # packages required by various optional pieces of the codebase
 torch = "^2.2"
 torchvision = "^0.17"
 pyarrow = ">=13.0.0"
 openai = "^1.0.0"
-together = "^0.2.11"
+together = "^1.0.1"
 fireworks-ai = "^0.13.0"
 boto3 = "^1.17"
 spacy = "^3.0"
 en-core-web-sm = {url = "https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-3.7.1/en_core_web_sm-3.7.1-py3-none-any.whl"}
 tiktoken = ">=0.3"
 sentence-transformers = "^2.0.0"
 transformers = "^4.20"
+datasets = ">=2.15.0"
 
 [tool.mypy]
 plugins = "sqlalchemy.ext.mypy.plugin"
 disallow_untyped_defs = true
 disallow_any_unimported = true
 no_implicit_optional = true
 check_untyped_defs = true
```

### Comparing `pixeltable-0.2.3/PKG-INFO` & `pixeltable-0.2.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,73 @@
 Metadata-Version: 2.1
 Name: pixeltable
-Version: 0.2.3
+Version: 0.2.4
 Summary: Pixeltable: The Multimodal AI Data Plane
 Author: Marcel Kornacker
 Author-email: marcelk@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: av (>=10.0.0)
 Requires-Dist: beautifulsoup4 (>=4.0.0,<5.0.0)
 Requires-Dist: cloudpickle (>=2.2.1,<3.0.0)
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: jmespath (>=1.0.1,<2.0.0)
-Requires-Dist: numpy (>=1.26,<2.0)
+Requires-Dist: numpy (>=1.26)
 Requires-Dist: opencv-python-headless (>=4.7.0.68,<5.0.0.0)
 Requires-Dist: pandas (>=2.0,<3.0)
-Requires-Dist: pgserver (==0.0.9)
+Requires-Dist: pgserver (==0.1.0)
 Requires-Dist: pgvector (>=0.2.1,<0.3.0)
-Requires-Dist: pillow (>=9.4.0,<10.0.0)
+Requires-Dist: pillow (>=10.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: regex (>=2022.10.31,<2023.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: sqlalchemy-utils (>=0.41.1,<0.42.0)
 Requires-Dist: sqlalchemy[mypy] (>=2.0.23,<3.0.0)
+Requires-Dist: tenacity (>=8.2,<9.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Description-Content-Type: text/markdown
 
+<div align="center">
 <img src="docs/pixeltable-banner.png" width="45%"/>
 
-# Pixeltable: The Multimodal AI Data Plane
+# Unifying Data, Models, and Orchestration for AI Products
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 &nbsp;&nbsp;
 ![pytest status](https://github.com/pixeltable/pixeltable/actions/workflows/pytest.yml/badge.svg)
 
-Pixeltable is a Python library that lets AI engineers and data scientists focus on
-exploration, modeling, and app development without having to deal with the customary
-data plumbing.
+[Installation](https://pixeltable.github.io/pixeltable/getting-started/) | [Documentation](https://pixeltable.github.io/pixeltable/)
+</div>
 
-**Pixeltable redefines data infrastructure and workflow orchestration for AI development.**
-It brings together data storage, versioning, and indexing with orchestration and model
-versioning under a declarative table interface, with transformations, model inference,
-and custom logic represented as computed columns.
+Pixeltable is a Python library that lets AI engineers and data scientists focus on exploration, modeling, and app development without dealing with the customary data plumbing.
 
-## Quick Start
+## What problems does Pixeltable solve?
+
+Today’s solutions for AI app development require extensive custom coding and infrastructure
+plumbing. Tracking lineage and versions between and across data transformations, models, and
+deployment is cumbersome. Pixeltable is a replacement for traditional data plumbing, providing
+a unified plane for data, models, and orchestration. It removes the data plumbing overhead in
+building and productionizing AI applications.
+
+## ⚡Quick Start
+Learn the basics of Pixeltable through interactive examples. View the notebooks on Google Colab or Kaggle, for free.
 
-If you just want to play around with Pixeltable to see what it's capable of, the easiest way is to run
-the Pixeltable Basics tutorial in colab:
+### Pixeltable Basics
+In this tutorial, we'll survey how to create tables, populate them with data, and enhance them with built-in and user-defined transformations and AI operations.
 
-<a target="_blank" href="https://colab.research.google.com/github/pixeltable/pixeltable/blob/master/docs/tutorials/pixeltable-basics.ipynb">
-  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
-</a>
+[![Open in Kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/code/brunep/pixeltable-basics) <a target="_blank" href="https://colab.research.google.com/github/pixeltable/pixeltable/blob/master/docs/tutorials/pixeltable-basics.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a>
 
-## Installation
 
+## 💾 Installation
 Pixeltable works with Python 3.9, 3.10, or 3.11 running on Linux or MacOS.
 
 ```
 pip install pixeltable
 ```
 
 To verify that it's working:
@@ -74,22 +79,14 @@
 
 For more detailed installation instructions, see the
 [Getting Started with Pixeltable](https://pixeltable.github.io/pixeltable/getting-started/)
 guide. Then, check out the
 [Pixeltable Basics](https://pixeltable.github.io/pixeltable/tutorials/pixeltable-basics/)
 tutorial for a tour of its most important features.
 
-## What problems does Pixeltable solve?
-
-Today’s solutions for AI app development require extensive custom coding and infrastructure
-plumbing. Tracking lineage and versions between and across data transformations, models, and
-deployment is cumbersome. Pixeltable is a replacement for traditional data plumbing, providing
-a unified plane for data, models, and orchestration. It removes the data plumbing overhead in
-building and productionizing AI applications.
-
 ## Why should you use Pixeltable?
 
 - It gives you transparency and reproducibility
     - All generated data is automatically recorded and versioned
     - You will never need to re-run a workload because you lost track of the input data
 - It saves you money
     - All data changes are automatically incremental
@@ -115,7 +112,16 @@
 storage.
 * Access all Pixeltable-resident data directly as a PyTorch dataset in your training scripts.
 * Understand the compute and storage costs of your data at the granularity of individual augmentations and
 get cost projections before adding new data and new augmentations.
 * Rely on Pixeltable's automatic versioning and snapshot functionality to protect against regressions
 and to ensure reproducibility.
 
+## Contributions & Feedback
+
+Are you experiencing issues or bugs with Pixeltable? File an [Issue](https://github.com/pixeltable/pixeltable/issues).
+</br>Do you want to contribute? Feel free to open a [PR](https://github.com/pixeltable/pixeltable/pulls).
+
+## :classical_building: License
+
+This library is licensed under the Apache 2.0 License.
+
```

