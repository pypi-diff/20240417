# Comparing `tmp/aligned-0.0.94.tar.gz` & `tmp/aligned-0.0.9a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aligned-0.0.94.tar", max compression
+gzip compressed data, was "aligned-0.0.9a0.tar", max compression
```

## Comparing `aligned-0.0.94.tar` & `aligned-0.0.9a0.tar`

### file list

```diff
@@ -1,110 +1,73 @@
--rw-r--r--   0        0        0    11358 2024-04-17 20:16:46.976541 aligned-0.0.94/LICENSE
--rw-r--r--   0        0        0     9669 2024-04-17 20:16:46.976541 aligned-0.0.94/README.md
--rw-r--r--   0        0        0     2161 2024-04-17 20:16:46.976541 aligned-0.0.94/aligned/__init__.py
--rw-r--r--   0        0        0     1174 2024-04-17 20:16:46.976541 aligned-0.0.94/aligned/active_learning/job.py
--rw-r--r--   0        0        0     1906 2024-04-17 20:16:46.976541 aligned-0.0.94/aligned/active_learning/selection.py
--rw-r--r--   0        0        0     2202 2024-04-17 20:16:46.976541 aligned-0.0.94/aligned/active_learning/write_policy.py
--rw-r--r--   0        0        0     8531 2024-04-17 20:16:46.976541 aligned-0.0.94/aligned/cli.py
--rw-r--r--   0        0        0    12133 2024-04-17 20:16:46.976541 aligned-0.0.94/aligned/compiler/aggregation_factory.py
--rw-r--r--   0        0        0    56720 2024-04-17 20:16:46.976541 aligned-0.0.94/aligned/compiler/feature_factory.py
--rw-r--r--   0        0        0    17497 2024-04-17 20:16:46.976541 aligned-0.0.94/aligned/compiler/model.py
--rw-r--r--   0        0        0     6557 2024-04-17 20:16:46.976541 aligned-0.0.94/aligned/compiler/repo_reader.py
--rw-r--r--   0        0        0      283 2024-04-17 20:16:46.976541 aligned-0.0.94/aligned/compiler/tests/features.py
--rw-r--r--   0        0        0      540 2024-04-17 20:16:46.976541 aligned-0.0.94/aligned/compiler/tests/test_repo_reader.py
--rw-r--r--   0        0        0    24833 2024-04-17 20:16:46.976541 aligned-0.0.94/aligned/compiler/transformation_factory.py
--rw-r--r--   0        0        0      829 2024-04-17 20:16:46.976541 aligned-0.0.94/aligned/compiler/vector_index_factory.py
--rw-r--r--   0        0        0     1224 2024-04-17 20:16:46.976541 aligned-0.0.94/aligned/data_file.py
--rw-r--r--   0        0        0        0 2024-04-17 20:16:46.976541 aligned-0.0.94/aligned/data_source/__init__.py
--rw-r--r--   0        0        0    39711 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/data_source/batch_data_source.py
--rw-r--r--   0        0        0     2836 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/data_source/stream_data_source.py
--rw-r--r--   0        0        0     1794 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/data_source/tests/test_batch_source.py
--rw-r--r--   0        0        0     6383 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/enricher.py
--rw-r--r--   0        0        0      669 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/exceptions.py
--rw-r--r--   0        0        0     9643 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/exposed_model/interface.py
--rw-r--r--   0        0        0     7472 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/exposed_model/mlflow.py
--rw-r--r--   0        0        0    12162 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/exposed_model/ollama.py
--rw-r--r--   0        0        0     1776 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/exposed_model/tests/test_mlflow.py
--rw-r--r--   0        0        0     5946 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/feature_source.py
--rw-r--r--   0        0        0    69495 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/feature_store.py
--rw-r--r--   0        0        0      235 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/feature_view/__init__.py
--rw-r--r--   0        0        0     5301 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/feature_view/combined_view.py
--rw-r--r--   0        0        0    27730 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/feature_view/feature_view.py
--rw-r--r--   0        0        0      846 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/feature_view/tests/test_brest_cancer.py
--rw-r--r--   0        0        0     2830 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/feature_view/tests/test_brest_cancer_event_timestamp.py
--rw-r--r--   0        0        0      969 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/feature_view/tests/test_check_schema.py
--rw-r--r--   0        0        0     3183 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/feature_view/tests/test_combined_view.py
--rw-r--r--   0        0        0      737 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/feature_view/tests/test_custom_source.py
--rw-r--r--   0        0        0     2242 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/feature_view/tests/test_hidden_variable.py
--rw-r--r--   0        0        0     3982 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/feature_view/tests/test_joined_source.py
--rw-r--r--   0        0        0     1079 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/jobs/tests/test_combined_job.py
--rw-r--r--   0        0        0     4942 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/jobs/tests/test_derived_job.py
--rw-r--r--   0        0        0        0 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/local/__init__.py
--rw-r--r--   0        0        0    20312 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/local/job.py
--rw-r--r--   0        0        0      817 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/local/tests/test_directory_interfaces.py
--rw-r--r--   0        0        0     1621 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/local/tests/test_jobs.py
--rw-r--r--   0        0        0        0 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/psql/__init__.py
--rw-r--r--   0        0        0    25143 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/psql/jobs.py
--rw-r--r--   0        0        0        0 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/redis/__init__.py
--rw-r--r--   0        0        0     4213 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/redis/job.py
--rw-r--r--   0        0        0     5232 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/redis/tests/test_redis_job.py
--rw-r--r--   0        0        0        0 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/redshift/__init__.py
--rw-r--r--   0        0        0    18626 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/redshift/jobs.py
--rw-r--r--   0        0        0     4749 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/redshift/sql_job.py
--rw-r--r--   0        0        0    18952 2024-04-17 20:16:46.980541 aligned-0.0.94/aligned/request/retrival_request.py
--rw-r--r--   0        0        0     1916 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/request/tests/test_feature_request_generation.py
--rw-r--r--   0        0        0    85465 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/retrival_job.py
--rw-r--r--   0        0        0        0 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/s3/__init__.py
--rw-r--r--   0        0        0     2018 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/s3/storage.py
--rw-r--r--   0        0        0      251 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/schemas/codable.py
--rw-r--r--   0        0        0      312 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/schemas/constraint_types.py
--rw-r--r--   0        0        0     3730 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/schemas/constraints.py
--rw-r--r--   0        0        0     3720 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/schemas/date_formatter.py
--rw-r--r--   0        0        0     3558 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/schemas/derivied_feature.py
--rw-r--r--   0        0        0     2745 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/schemas/event_trigger.py
--rw-r--r--   0        0        0    11597 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/schemas/feature.py
--rw-r--r--   0        0        0    16800 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/schemas/feature_view.py
--rw-r--r--   0        0        0     7537 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/schemas/folder.py
--rw-r--r--   0        0        0     3197 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/schemas/literal_value.py
--rw-r--r--   0        0        0     9244 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/schemas/model.py
--rw-r--r--   0        0        0     2207 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/schemas/record_coders.py
--rw-r--r--   0        0        0     7594 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/schemas/repo_definition.py
--rw-r--r--   0        0        0     1686 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/schemas/target.py
--rw-r--r--   0        0        0     8976 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/schemas/text_vectoriser.py
--rw-r--r--   0        0        0    70366 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/schemas/transformation.py
--rw-r--r--   0        0        0     2330 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/schemas/vector_storage.py
--rw-r--r--   0        0        0     9963 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/server.py
--rw-r--r--   0        0        0     1047 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/source_validation.py
--rw-r--r--   0        0        0        0 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/sources/__init__.py
--rw-r--r--   0        0        0    23798 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/sources/azure_blob_storage.py
--rw-r--r--   0        0        0     1125 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/sources/kafka.py
--rw-r--r--   0        0        0    26687 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/sources/local.py
--rw-r--r--   0        0        0     7407 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/sources/psql.py
--rw-r--r--   0        0        0    10507 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/sources/redis.py
--rw-r--r--   0        0        0     5021 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/sources/redshift.py
--rw-r--r--   0        0        0     8248 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/sources/s3.py
--rw-r--r--   0        0        0     7017 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/sources/tests/test_parquet.py
--rw-r--r--   0        0        0     4464 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/sources/tests/test_psql.py
--rw-r--r--   0        0        0     9894 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/split_strategy.py
--rw-r--r--   0        0        0      196 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/storage.py
--rw-r--r--   0        0        0        0 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/streams/__init__.py
--rw-r--r--   0        0        0     1037 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/streams/interface.py
--rw-r--r--   0        0        0      617 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/streams/kafka.py
--rw-r--r--   0        0        0     1641 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/streams/redis.py
--rw-r--r--   0        0        0      682 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/tests/test_cache_enricher.py
--rw-r--r--   0        0        0      623 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/tests/test_cached_parquet.py
--rw-r--r--   0        0        0     1628 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/tests/test_date_timezone_converter.py
--rw-r--r--   0        0        0     1767 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/tests/test_feature_view_wrapper.py
--rw-r--r--   0        0        0     2246 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/tests/test_filter_job_request.py
--rw-r--r--   0        0        0     6722 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/tests/test_model_target.py
--rw-r--r--   0        0        0     3355 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/tests/test_models_as_feature.py
--rw-r--r--   0        0        0     1506 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/tests/test_source_validation.py
--rw-r--r--   0        0        0     2057 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/tests/test_statistic_enricher.py
--rw-r--r--   0        0        0     3178 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/tests/test_timestamp_decoding.py
--rw-r--r--   0        0        0     4036 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/tests/test_train_test_validate_set.py
--rw-r--r--   0        0        0     5286 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/tests/test_transformations.py
--rw-r--r--   0        0        0      377 2024-04-17 20:16:46.984541 aligned-0.0.94/aligned/validation/interface.py
--rw-r--r--   0        0        0     2882 2024-04-17 20:16:46.988541 aligned-0.0.94/aligned/validation/pandera.py
--rw-r--r--   0        0        0     1464 2024-04-17 20:16:46.988541 aligned-0.0.94/aligned/validation/tests/test_pandera_validator.py
--rw-r--r--   0        0        0    12497 2024-04-17 20:16:46.988541 aligned-0.0.94/aligned/worker.py
--rw-r--r--   0        0        0     3158 2024-04-17 20:16:46.988541 aligned-0.0.94/pyproject.toml
--rw-r--r--   0        0        0    12642 1970-01-01 00:00:00.000000 aligned-0.0.94/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-01-03 20:34:00.544967 aligned-0.0.9a0/LICENSE
+-rw-r--r--   0        0        0     8521 2023-01-03 20:34:00.544967 aligned-0.0.9a0/README.md
+-rw-r--r--   0        0        0     1189 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/__init__.py
+-rw-r--r--   0        0        0    14066 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/cli.py
+-rw-r--r--   0        0        0      441 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/compiler/constraint_factory.py
+-rw-r--r--   0        0        0    19110 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/compiler/feature_factory.py
+-rw-r--r--   0        0        0     5784 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/compiler/repo_reader.py
+-rw-r--r--   0        0        0    18324 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/compiler/transformation_factory.py
+-rw-r--r--   0        0        0      822 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/data_file.py
+-rw-r--r--   0        0        0        0 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/data_source/__init__.py
+-rw-r--r--   0        0        0     3467 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/data_source/batch_data_source.py
+-rw-r--r--   0        0        0     1973 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/data_source/stream_data_source.py
+-rw-r--r--   0        0        0     8108 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/enricher.py
+-rw-r--r--   0        0        0      278 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/entity_data_source.py
+-rw-r--r--   0        0        0      341 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/exceptions.py
+-rw-r--r--   0        0        0     7657 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_source.py
+-rw-r--r--   0        0        0    17949 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_store.py
+-rw-r--r--   0        0        0      298 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_view/__init__.py
+-rw-r--r--   0        0        0     4969 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_view/combined_view.py
+-rw-r--r--   0        0        0    10029 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_view/feature_view.py
+-rw-r--r--   0        0        0      944 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_view/tests/test_brest_cancer.py
+-rw-r--r--   0        0        0     3135 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_view/tests/test_brest_cancer_event_timestamp.py
+-rw-r--r--   0        0        0     1239 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_view/tests/test_combined_view.py
+-rw-r--r--   0        0        0     1692 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/feature_view/tests/test_hidden_variable.py
+-rw-r--r--   0        0        0     1074 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/jobs/tests/test_combined_job.py
+-rw-r--r--   0        0        0     1981 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/jobs/tests/test_derived_job.py
+-rw-r--r--   0        0        0        0 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/local/__init__.py
+-rw-r--r--   0        0        0     6962 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/local/job.py
+-rw-r--r--   0        0        0     8899 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/local/source.py
+-rw-r--r--   0        0        0     1105 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/local/tests/test_jobs.py
+-rw-r--r--   0        0        0     3006 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/model.py
+-rw-r--r--   0        0        0     2967 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/online_source.py
+-rw-r--r--   0        0        0        0 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/psql/__init__.py
+-rw-r--r--   0        0        0     4431 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/psql/data_source.py
+-rw-r--r--   0        0        0    10601 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/psql/jobs.py
+-rw-r--r--   0        0        0        0 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redis/__init__.py
+-rw-r--r--   0        0        0     4348 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redis/config.py
+-rw-r--r--   0        0        0     3288 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redis/job.py
+-rw-r--r--   0        0        0     2275 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redis/stream.py
+-rw-r--r--   0        0        0     4402 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redis/tests/test_redis_job.py
+-rw-r--r--   0        0        0        0 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redshift/__init__.py
+-rw-r--r--   0        0        0     2660 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redshift/data_source.py
+-rw-r--r--   0        0        0     1172 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/redshift/factory.py
+-rw-r--r--   0        0        0     8250 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/request/retrival_request.py
+-rw-r--r--   0        0        0     1817 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/request/tests/test_feature_request_generation.py
+-rw-r--r--   0        0        0    15322 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/retrival_job.py
+-rw-r--r--   0        0        0        0 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/s3/__init__.py
+-rw-r--r--   0        0        0     5715 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/s3/config.py
+-rw-r--r--   0        0        0     1447 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/s3/factory.py
+-rw-r--r--   0        0        0     1846 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/s3/storage.py
+-rw-r--r--   0        0        0      251 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/codable.py
+-rw-r--r--   0        0        0     2356 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/constraints.py
+-rw-r--r--   0        0        0     1379 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/derivied_feature.py
+-rw-r--r--   0        0        0     3663 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/feature.py
+-rw-r--r--   0        0        0     8217 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/feature_view.py
+-rw-r--r--   0        0        0      409 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/model.py
+-rw-r--r--   0        0        0     4478 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/repo_definition.py
+-rw-r--r--   0        0        0    37245 2023-01-03 20:34:00.548967 aligned-0.0.9a0/aligned/schemas/transformation.py
+-rw-r--r--   0        0        0     8663 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/server.py
+-rw-r--r--   0        0        0     5086 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/split_strategy.py
+-rw-r--r--   0        0        0      196 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/storage.py
+-rw-r--r--   0        0        0      682 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/tests/test_cache_enricher.py
+-rw-r--r--   0        0        0      549 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/tests/test_cached_parquet.py
+-rw-r--r--   0        0        0     2056 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/tests/test_statistic_enricher.py
+-rw-r--r--   0        0        0     2371 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/tests/test_train_test_validate_set.py
+-rw-r--r--   0        0        0      905 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/tests/test_transformations.py
+-rw-r--r--   0        0        0      193 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/validation/interface.py
+-rw-r--r--   0        0        0     2392 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/validation/pandera.py
+-rw-r--r--   0        0        0      848 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/validation/tests/test_pandera_validator.py
+-rw-r--r--   0        0        0     3846 2023-01-03 20:34:00.552967 aligned-0.0.9a0/aligned/worker.py
+-rw-r--r--   0        0        0     2553 2023-01-03 20:34:00.552967 aligned-0.0.9a0/pyproject.toml
+-rw-r--r--   0        0        0    10667 1970-01-01 00:00:00.000000 aligned-0.0.9a0/setup.py
+-rw-r--r--   0        0        0    10982 1970-01-01 00:00:00.000000 aligned-0.0.9a0/PKG-INFO
```

### Comparing `aligned-0.0.94/LICENSE` & `aligned-0.0.9a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aligned-0.0.94/README.md` & `aligned-0.0.9a0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,309 +1,286 @@
 # Aligned
 
-A data managment tool for ML applications.
+Aligned help defining a single source of truth for logic while keeping the technology stack flexible. Such innovation has been possible by removing the need to depend on a processing engine, leading to less- and more transparent- code. Furthermore, the declarative API has made it possible to comment, add data validation, and define feature transformation at the same location. Therefore, it leads to a precise definition of the intended result.
 
-Similar to how DBT is a data managment tool for business analytics, will Aligned manage ML projects.
+Read the post about [how the most elegant MLOps tool was created](https://matsmoll.github.io/2022/12/31/How-I-created-the-most-elegant-MLOps-tool.html)
 
-Aligned does this through two things.
-1. A light weight data managment system. Making it possible to query a data lake and databases.
-2. Tooling to define a `model_contract`. Clearing up common unanswerd questions through code.
+Also check out the the [example repo](https://github.com/otovo/aligned-example) to see how it can be used
 
+⚠️ Aligned is in alpha, so bugs will be likely. Even though Otovo use this for production.
 
-Furthermore, Aligned collect data lineage between models, basic feature transformations. While also making it easy to reduce data leakage with point-in-time valid data and fix other problems described in [Sculley et al. [2015]](https://papers.nips.cc/paper/2015/file/86df7dcfd896fcaf2674f757a2463eba-Paper.pdf).
-
-## Examples
-
-Bellow are some examples of how Aligned can be used.
-
-### Aligned UI
-
-Aligned provides an UI to view which data exists, the expectations we have and find faults.
-
-[View the example UI](https://aligned-catalog.azurewebsites.net/).
-However, this is still under development, so sign up for a [wait list](https://aligned-managed-web.vercel.app/) to get access.
-
-
-### Example Repo
+## Feature Views
 
-Want to look at examples of how to use `aligned`?
-View the [`MatsMoll/aligned-example` repo](https://github.com/MatsMoll/aligned-example).
+Write features as the should be, as data models.
+Then get code completion and typesafety by referencing them in other features.
 
-Or see how you could query a file in a data lake.
+This makes the features light weight, data source indipendent, and flexible.
 
 ```python
-store = await ContractStore.from_dir(".")
-df = await store.execute_sql("SELECT * FROM titanic LIMIT 10").to_polars()
-```
-
-## Docs
+class TitanicPassenger(FeatureView):
 
-Check out the [Aligned Docs](https://www.aligned.codes), but keep in mind that they are still work in progress.
-
----
-
-### Available Features
-
-Bellow are some of the features Aligned offers:
+    metadata = FeatureViewMetadata(
+        name="passenger",
+        description="Some features from the titanic dataset",
+        batch_source=FileSource.csv_at("titanic.csv"),
+        stream_source=HttpStreamSource(topic_name="titanic")
+    )
 
-- [Data Catalog](https://aligned-managed-web.vercel.app/)
-- [Data Lineage](https://aligned-managed-web.vercel.app/)
-- [Model Performance Monitoring](https://aligned-managed-web.vercel.app/)
-- [Data Freshness](#data-freshness)
-- [Data Quality Assurance](#data-quality)
-- [Feature Store](https://matsmoll.github.io/posts/understanding-the-chaotic-landscape-of-mlops#feature-store)
-- [Exposing Models](#exposed-models)
+    passenger_id = Entity(dtype=Int32())
 
+    # Input values
+    age = (
+        Float()
+            .description("A float as some have decimals")
+            .is_required()
+            .lower_bound(0)
+            .upper_bound(110)
+    )
 
-All from the simple API of defining
-- [Data Sources](#data-sources)
-- [Feature Views](#feature-views)
-- [Models](#describe-models)
+    name = String()
+    sex = String().accepted_values(["male", "female"])
+    survived = Bool().description("If the passenger survived")
+    sibsp = Int32().lower_bound(0, is_inclusive=True).description("Number of siblings on titanic")
+    cabin = String()
 
-As a result, loading model features is as easy as:
+    # Creates two one hot encoded values
+    is_male, is_female = sex.one_hot_encode(['male', 'female'])
 
-```python
-entities = {"passenger_id": [1, 2, 3, 4]}
-await store.model("titanic").features_for(entities).to_pandas()
+    # Standard scale the age.
+    # This will fit the scaler using a data slice from the batch source
+    # limited to maximum 100 rows. We can also uese a time constraint if wanted
+    scaled_age = age.standard_scaled(limit=100)
 ```
 
-Aligned is still in active development, so changes are likely.
+## Data sources
 
-## Model Contract
+Alinged makes handling data sources easy, as you do not have to think about how it is done.
+Only define where the data is, and we handle the dirty work.
 
-Aligned introduces a new concept called the "model contract", which tries to answer the following questions.
+```python
+my_db = PostgreSQLConfig(env_var="DATABASE_URL")
 
-- What is predicted?
-- What is assosiated with a prediction? - A user id?
-- Where do we store predictions?
-- Do a model depend on other models?
-- Is the model exposed through an API?
-- What needs to be sent in, to use the model?
-- Is it classification, regression, gen ai?
-- Where is the ground truth stored? - if any
-- Who owns the model?
-- Where do we store data sets?
+class TitanicPassenger(FeatureView):
 
-All this is described through a `model_contract`, as shown bellow.
+    metadata = FeatureViewMetadata(
+        name="passenger",
+        description="Some features from the titanic dataset",
+        batch_source=my_db.table(
+            "passenger",
+            mapping_keys={
+                "Passenger_Id": "passenger_id"
+            }
+        ),
+        stream_source=HttpStreamSource(topic_name="titanic")
+    )
 
-```python
-@model_contract(
-    name="eta_taxi",
-    input_features=[
-        trips.eucledian_distance,
-        trips.number_of_passengers,
-        traffic.expected_delay
-    ],
-    output_source=FileSource.delta_at("titanic_model/predictions")
-)
-class EtaTaxi:
-    trip_id = Int32().as_entity()
-    predicted_at = EventTimestamp()
-    predicted_duration = trips.duration.as_regression_target()
+    passenger_id = Entity(dtype=Int32())
 ```
 
-## Data Sources
+### Fast development
 
-Alinged makes handling data sources easy, as you do not have to think about how it is done.
-
-Furthermore, Aligned makes it easy to switch parts of the business logic to a local setup for debugging purposes.
+Making iterativ and fast exploration in ML is important. This is why Aligned also makes it super easy to combine, and test multiple sources.
 
 ```python
-from aligned import FileSource, AwsS3Config, AzureBlobConfig
-
-dir_type: Literal["local", "aws", "azure"] = ...
+my_db = PostgreSQLConfig.localhost()
 
-if dir_type == "aws":
-    aws_config = AwsS3Config(...)
-    root_directory = aws_config.directory("my-awesome-project")
+aws_bucket = AwsS3Config(...)
 
-elif dir_type == "azure":
-    azure_config = AzureBlobConfig(...)
-    root_directory = azure_config.directory("my-awesome-project")
-else:
-    root_directory = FileSource.directory("my-awesome-project")
+class SomeFeatures(FeatureView):
 
+    metadata = FeatureViewMetadata(
+        name="some_features",
+        description="...",
+        batch_source=my_db.table("local_features")
+    )
 
-taxi_project = root_directory.sub_directory("eta_taxi")
+    # Some features
+    ...
 
-csv_source = taxi_project.csv_at("predictions.csv")
-parquet_source = taxi_project.parquet_at("predictions.parquet")
-delta_source = taxi_project.delta_at("predictions")
-```
+class AwsFeatures(FeatureView):
 
-### Date Formatting
-Managing a data lake can be hard. However, a common problem when using file formats can be managing date formats. As a result do Aligned provide a way to standardise this, so you can focus on what matters.
+    metadata = FeatureViewMetadata(
+        name="aws",
+        description="...",
+        batch_source=aws_bucket.file_at("path/to/file.parquet")
+    )
 
-```python
-from aligned import FileSource
-from aligned.schemas.date_formatter import DateFormatter
+    # Some features
+    ...
+```
 
-iso_formatter = DateFormatter.iso_8601()
-unix_formatter = DateFormatter.unix_timestamp(time_unit="us", time_zone="UTC")
-custom_strtime_formatter = DateFormatter.string_format("%Y/%m/%d %H:%M:%S")
+## Model Service
 
-FileSource.csv_at("my/file.csv", date_formatter=unix_formatter)
+Usually will you need to combine multiple features for each model.
+This is where a `ModelService` comes in.
+Here can you define which features should be exposed.
+
+```python
+# Uses the variable name, as the model service name.
+# Can also define a custom name, if wanted.
+titanic_model = ModelService(
+    features=[
+        TitanicPassenger.select_all(),
+
+        # Select features with code completion
+        LocationFeatures.select(lambda view: [
+            view.distance_to_shore,
+            view.distance_to_closest_boat
+        ]),
+    ]
+)
 ```
 
-## Feature Views
-
-Aligned also makes it possible to define data and features through `feature_view`s.
-Then get code completion and typesafety by referencing them in other features.
 
-This makes the features light weight, data source independent, and flexible.
+## Data Enrichers
 
-```python
-@feature_view(
-    name="passenger",
-    description="Some features from the titanic dataset",
-    source=FileSource.csv_at("titanic.csv"),
-    materialized_source=FileSource.parquet_at("titanic.parquet"),
+In manny cases will extra data be needed in order to generate some features.
+We therefore need some way of enriching the data.
+This can easily be done with Alinged's `DataEnricher`s.
+
+```python
+my_db = PostgreSQLConfig.localhost()
+redis = RedisConfig.localhost()
+
+user_location = my_db.data_enricher( # Fetch all user locations
+    sql="SELECT * FROM user_location"
+).cache( # Cache them for one day
+    ttl=timedelta(days=1),
+    cache_key="user_location_cache"
+).lock( # Make sure only one processer fetches the data at a time
+    lock_name="user_location_lock",
+    redis_config=redis
 )
-class TitanicPassenger:
 
-    passenger_id = Int32().as_entity()
 
-    age = (
-        Float()
-            .description("A float as some have decimals")
-            .lower_bound(0)
-            .upper_bound(110)
-    )
+async def distance_to_users(df: DataFrame) -> Series:
+    user_location_df = await user_location.load()
+    ...
+    return distances
 
-    name = String()
-    sex = String().accepted_values(["male", "female"])
-    did_survive = Bool().description("If the passenger survived")
-    sibsp = Int32().lower_bound(0).description("Number of siblings on titanic")
-    cabin = String().is_optional()
+class SomeFeatures(FeatureView):
 
-    # Creates two one hot encoded values
-    is_male, is_female = sex.one_hot_encode(['male', 'female'])
+    metadata = FeatureViewMetadata(...)
+
+    latitude = Float()
+    longitude = Float()
+
+    distance_to_users = Float().transformed(distance_to_users, using_features=[latitude, longitude])
 ```
 
-### Exposed models
 
-Aligned mainly focuses on defining the expected input and output of different models. However, this in itself makes it hard to use the models. This is why Aligned makes it possible to define how our ML models are exposed by setting an `exposed_model` attribute.
+## Access Data
 
+You can easily create a feature store that contains all your feature definitions.
+This can then be used to genreate data sets, setup an instce to serve features, DAG's etc.
 
 ```python
-from aligned.exposed_model.mlflow import mlflow_server
+store = FeatureStore.from_dir(".")
 
-@model_contract(
-    name="eta_taxi",
-    exposed_model=mlflow_server(
-        host="http://localhost:8000",
-    ),
-    ...
-)
-class EtaTaxi:
-    trip_id = Int32().as_entity()
-    predicted_at = EventTimestamp()
-    predicted_duration = trips.duration.as_regression_target()
+# Select all features from a single feature view
+df = await store.all_for("passenger", limit=100).to_df()
 ```
 
-This also makes it possible to get predictions with the following command:
+### Centraliced Feature Store Definition
+You would often share the features with other coworkers, or split them into different stages, like `staging`, `shadow`, or `production`.
+One option is therefore to reference the storage you use, and load the `FeatureStore` from there.
 
 ```python
-await store.model("eta_taxi").predict_over({
-    "trip_id": [...]
-}).to_polars()
-```
-
-Or store them directly in the `output_source` with something like:
+aws_bucket = AwsS3Config(...)
+store = await aws_bucket.file_at("production.json").feature_store()
 
-```python
-await store.model("eta_taxi").predict_over({
-    "trip_id": [...]
-}).upsert_into_output_source()
+# This switches from the production online store to the offline store
+# Aka. the batch sources defined on the feature views
+experimental_store = store.offline_store()
 ```
+This json file can be generated by running `alinged apply`.
 
-Some of the existing implementations are:
-- MLFlow Server
-- Run MLFLow model in memory
-- Ollama completion endpoint
-- Ollama embedded endpoint
-- Send entities to generic endpoint
-
-## Data Freshness
-Making sure a source contains fresh data is a crucial part to create propper ML applications.
-Therefore, Aligned provides an easy way to check how fresh a source is.
+### Select multiple feature views
 
 ```python
-@feature_view(
-    name="departures",
-    description="Features related to the departure of a taxi ride",
-    source=taxi_db.table("departures"),
-)
-class TaxiDepartures:
+df = await store.features_for({
+    "passenger_id": [1, 50, 110]
+}, features=[
+    "passenger:scaled_age",
+    "passenger:is_male",
+    "passenger:sibsp"
 
-    trip_id = UUID().as_entity()
+    "other_features:distance_to_closest_boat",
+]).to_df()
+```
 
-    pickuped_at = EventTimestamp()
+### Model Service
 
-    number_of_passengers = Int32().is_optional()
+Selecting features for a model is super simple.
 
-    dropoff_latitude = Float()
-    dropoff_longitude = Float()
 
-    pickup_latitude = Float()
-    pickup_longitude = Float()
+```python
+df = await store.model("titanic_model").features_for({
+    "passenger_id": [1, 50, 110]
+}).to_df()
+```
 
+### Feature View
 
-freshness = await TaxiDepartures.freshness_in_batch_source()
+If you want to only select features for a specific feature view, then this is also possible.
 
-if freshness < datetime.now() - timedelta(days=2):
-    raise ValueError("To old data to create an ML model")
+```python
+prev_30_days = await store.feature_view("match").previous(days=30).to_df()
+sample_of_20 = await store.feature_view("match").all(limit=20).to_df()
 ```
 
 ## Data quality
 Alinged will make sure all the different features gets formatted as the correct datatype.
 In addition will aligned also make sure that the returend features aligne with defined constraints.
 
 ```python
-@feature_view(...)
-class TitanicPassenger:
+class TitanicPassenger(FeatureView):
+
     ...
+
     age = (
         Float()
+            .is_required()
             .lower_bound(0)
             .upper_bound(110)
     )
-    sibsp = Int32().lower_bound(0).is_optional()
+    sibsp = Int32().lower_bound(0, is_inclusive=True)
 ```
 
-Then since our feature view have a `is_optional` and a `lower_bound`, will the `.validate(...)` command filter out the entites that do not follow that behavior.
+Then since our feature view have a `is_required` and a `lower_bound`, will the `.validate(...)` command filter out the entites that do not follow that behavior.
 
 ```python
 from aligned.validation.pandera import PanderaValidator
 
 df = await store.model("titanic_model").features_for({
     "passenger_id": [1, 50, 110]
 }).validate(
     PanderaValidator()  # Validates all features
-).to_pandas()
+).to_df()
 ```
 
-## Contract Store
-
-Aligned collects all the feature views and model contracts in a contract store. You can generate this in a few different ways, and each method serves some different use-cases.
-
-For experimentational use-cases will the `await ContractStore.from_dir(".")` probably make the most sense. However, this will scan the full directory which can lead to slow startup times.
+## Feature Server
 
-Therefore, it is also possible to manually add the different feature views and contracts with the following.
+This expectes that you either run the command in your feature store repo, or have a file with a `RepoReference` instance.
+You can also setup an online source like Redis, for faster storage.
 
 ```python
-store = ContractStore.empty()
-store.add_feature_view(MyView)
-store.add_model(MyModel)
-```
-
-This makes it possible to define different contracts per project, or team. As a result, you can also combine differnet stores with.
+redis = RedisConfig.localhost()
 
-```python
-combined_store = recommendation_store.combined_with(forecasting_store)
-```
+aws_bucket = AwsS3Config(...)
 
-Lastly, we can also load the all features from a serializable format, such as a JSON file.
+repo_files = RepoReference(
+    env_var_name="ENVIRONMENT",
+    repo_paths={
+        "production": aws_bucket.file_at("feature-store/production.json"),
+        "shadow": aws_bucket.file_at("feature-store/shadow.json"),
+        "staging": aws_bucket.file_at("feature-store/staging.json")
+        # else generate the feature store from the current dir
+    }
+)
 
-```python
-await FileSource.json_at("contracts.json").as_contract_store()
+# Use redis as the online source, if not running localy
+if repo_files.selected != "local":
+    online_source = redis.online_source()
 ```
+
+Then run `aligned serve`, and a FastAPI server will start. Here can you push new features, which then transforms and stores the features, or just fetch them.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aligned-0.0.94/aligned/compiler/repo_reader.py` & `aligned-0.0.9a0/aligned/compiler/repo_reader.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 import logging
-from datetime import datetime
 from importlib import import_module
 from inspect import getmro, isclass
+from pathlib import Path
 from typing import Any
-from aligned.compiler.model import ModelContractWrapper
 
 from aligned.enricher import Enricher
-from aligned.feature_view.combined_view import CombinedFeatureViewWrapper
-from aligned.feature_view.feature_view import FeatureViewWrapper
-from aligned.schemas.repo_definition import EnricherReference, RepoDefinition, RepoMetadata, RepoReference
-from pathlib import Path
-
+from aligned.model import Model
+from aligned.online_source import BatchOnlineSource, OnlineSource
+from aligned.schemas.repo_definition import EnricherReference, RepoDefinition, RepoReference
 
 logger = logging.getLogger(__name__)
 
 
 def imports_for(file_path: Path) -> set[str]:
     try:
         with open(file_path) as file:
@@ -49,108 +46,98 @@
     # Remove the class name. Only store the superclasses
     # Otherwise it might init a abstract class and crash
     s = str(obj).replace("'", '').replace('>', '')
     super_class_names.remove(s.split('.')[-1])
     return super_class_names
 
 
-def find_files(repo_path: Path, ignore_path: Path | None = None, file_extension: str = 'py') -> list[Path]:
+def python_files(repo_path: Path, ignore_path: Path | None = None) -> list[Path]:
     files = {
         path.resolve()
-        for path in repo_path.resolve().glob(f'**/*.{file_extension}')
-        if path.is_file()
-        and '__init__.py' != path.name
-        and not any(part.startswith('.') for part in path.parts)
+        for path in repo_path.resolve().glob('**/*.py')
+        if path.is_file() and '__init__.py' != path.name
     }
     if ignore_path:
         ignore_files = {
             path.resolve()
-            for path in ignore_path.glob(f'**/*.{file_extension}')
-            if path.is_file()
-            and '__init__.py' != path.name
-            and not any(part.startswith('.') for part in path.parts)
+            for path in ignore_path.glob('**/*.py')
+            if path.is_file() and '__init__.py' != path.name
         }
         files -= ignore_files
     return sorted(files)
 
 
 def path_to_py_module(path: Path, repo_root: Path) -> str:
-    return str(path.relative_to(repo_root.resolve()))[: -len('.py')].replace('./', '').replace('/', '.')
+    return str(path.relative_to(repo_root))[: -len('.py')].replace('./', '').replace('/', '.')
 
 
 class RepoReader:
     """
     A class reading a repo, and generates a repo config
     """
 
     @staticmethod
-    async def definition_from_path(repo_path: Path, excludes: list[str] | None = None) -> RepoDefinition:
-
-        excluded_files: list[Path] = []
-        for exclude in excludes or []:
-            excluded_files.extend(repo_path.resolve().glob(exclude))
-
-        metadata = RepoMetadata(created_at=datetime.now(), name=repo_path.name, github_url=None)
+    async def definition_from_path(repo_path: Path) -> RepoDefinition:
         repo = RepoDefinition(
-            metadata=metadata,
             feature_views=set(),
             combined_feature_views=set(),
             models=set(),
+            online_source=BatchOnlineSource(),
             enrichers=[],
         )
 
         feature_view_names: dict[str, str] = {}
 
-        for py_file in find_files(repo_path):
-            if py_file in excluded_files:
-                continue
-
+        for py_file in python_files(repo_path):
             imports = imports_for(py_file)
 
             module_path = path_to_py_module(py_file, repo_path)
-
-            if module_path.startswith('aladdin') or module_path.startswith('.') or module_path.endswith('__'):
-                # Skip no feature defintion modules
+            if (
+                module_path.startswith('aladdin')
+                or module_path.startswith('.')
+                or module_path.startswith('heroku')
+                or module_path.endswith('__')
+            ):
+                # Skip aladdin modules
                 continue
 
             module = import_module(module_path)
 
             for attribute in dir(module):
                 if attribute in imports:
                     continue
 
                 obj = getattr(module, attribute)
 
-                if isinstance(obj, Enricher):
+                if isinstance(obj, Model):
+                    if not obj.name:
+                        obj.name = attribute
+                    repo.models.add(obj.schema())
+
+                elif isinstance(obj, Enricher):
                     repo.enrichers.append(
                         EnricherReference(module=module_path, attribute_name=attribute, enricher=obj)
                     )
-                elif isinstance(obj, FeatureViewWrapper):
-                    repo.feature_views.add(obj.compile())
-                elif isinstance(obj, CombinedFeatureViewWrapper):
-                    repo.combined_feature_views.add(obj.compile())
-                elif isinstance(obj, ModelContractWrapper):
-                    repo.models.add(obj.compile())
+                elif isinstance(obj, OnlineSource):
+                    repo.online_source = obj
                 else:
                     classes = super_classes_in(obj)
-                    if 'ModelContract' in classes:
-                        repo.models.add(obj.compile())
-                    elif 'FeatureView' in classes:
-                        fv = obj.compile()
+                    if 'FeatureView' in classes:
+                        fv = await obj.compile()
                         if fv.name in feature_view_names:
                             raise Exception(
                                 (
                                     f'Duplicate feature view names: {fv.name},',
                                     f' in {py_file}, and {feature_view_names[fv.name]}',
                                 )
                             )
                         feature_view_names[fv.name] = py_file.as_posix()
                         repo.feature_views.add(fv)
                     elif 'CombinedFeatureView' in classes:
-                        fv = obj.compile()
+                        fv = await obj.compile()
                         if fv.name in feature_view_names:
                             raise Exception(
                                 (
                                     f'Duplicate feature view names: {fv.name},',
                                     f' in {py_file}, and {feature_view_names[fv.name]}',
                                 )
                             )
```

### Comparing `aligned-0.0.94/aligned/data_source/stream_data_source.py` & `aligned-0.0.9a0/aligned/data_source/batch_data_source.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,95 +1,101 @@
-from __future__ import annotations
-
-from abc import ABC
-from dataclasses import dataclass, field
-from typing import TYPE_CHECKING
+from abc import ABC, abstractmethod
+from datetime import datetime
+from typing import Optional, TypeVar
 
 from mashumaro.types import SerializableType
 
+from aligned.request.retrival_request import RetrivalRequest
+from aligned.retrival_job import DateRangeJob, FullExtractJob, RetrivalJob
 from aligned.schemas.codable import Codable
-
-if TYPE_CHECKING:
-    from aligned.retrival_job import RetrivalJob
-    from aligned.streams.interface import ReadableStream
+from aligned.schemas.feature import Feature
 
 
-class StreamDataSourceFactory:
+class BatchDataSourceFactory:
 
-    supported_data_sources: dict[str, type[StreamDataSource]]
+    supported_data_sources: dict[str, type['BatchDataSource']]
 
-    _shared: StreamDataSourceFactory | None = None
+    _shared: Optional['BatchDataSourceFactory'] = None
 
     def __init__(self) -> None:
-        from aligned.sources.kafka import KafkaTopicConfig
-        from aligned.sources.redis import RedisStreamSource
+        from aligned.local.source import CsvFileSource
+        from aligned.psql.data_source import PostgreSQLDataSource
+        from aligned.redshift.data_source import RedshiftSQLDataSource
+        from aligned.s3.config import AwsS3CsvDataSource, AwsS3ParquetDataSource
 
         self.supported_data_sources = {
-            HttpStreamSource.name: HttpStreamSource,
-            RedisStreamSource.name: RedisStreamSource,
-            KafkaTopicConfig.name: KafkaTopicConfig,
+            PostgreSQLDataSource.type_name: PostgreSQLDataSource,
+            CsvFileSource.type_name: CsvFileSource,
+            AwsS3CsvDataSource.type_name: AwsS3CsvDataSource,
+            AwsS3ParquetDataSource.type_name: AwsS3ParquetDataSource,
+            RedshiftSQLDataSource.type_name: RedshiftSQLDataSource,
         }
 
     @classmethod
-    def shared(cls) -> StreamDataSourceFactory:
+    def shared(cls) -> 'BatchDataSourceFactory':
         if cls._shared:
             return cls._shared
-        cls._shared = StreamDataSourceFactory()
+        cls._shared = BatchDataSourceFactory()
         return cls._shared
 
 
-class StreamDataSource(ABC, Codable, SerializableType):
+T = TypeVar('T')
+
+
+class BatchDataSource(ABC, Codable, SerializableType):
     """
-    Used to determend if an API call should be created, or if we should listen to a stream.
+    A definition to where a specific pice of data can be found.
+    E.g: A database table, a file, a web service, etc.
+
+    Ths can thereafter be combined with other BatchDataSources in order to create a rich dataset.
     """
 
-    name: str
-    topic_name: str
+    type_name: str
+
+    @abstractmethod
+    def job_group_key(self) -> str:
+        pass
 
     def _serialize(self) -> dict:
-        assert self.name in StreamDataSourceFactory.shared().supported_data_sources
         return self.to_dict()
 
+    def __hash__(self) -> int:
+        return hash(self.job_group_key())
+
     @classmethod
-    def _deserialize(cls, value: dict) -> StreamDataSource:
-        name = value['name']
-        if name not in StreamDataSourceFactory.shared().supported_data_sources:
+    def _deserialize(cls, value: dict) -> 'BatchDataSource':
+        name_type = value['type_name']
+        if name_type not in BatchDataSourceFactory.shared().supported_data_sources:
             raise ValueError(
-                f"Unknown stream data source id: '{name}'.\nRemember to add the"
-                ' data source to the StreamDataSourceFactory.supported_data_sources if'
+                f"Unknown batch data source id: '{name_type}'.\nRemember to add the"
+                ' data source to the BatchDataSourceFactory.supported_data_sources if'
                 ' it is a custom type.'
             )
-        del value['name']
-        data_class = StreamDataSourceFactory.shared().supported_data_sources[name]
+        del value['type_name']
+        data_class = BatchDataSourceFactory.shared().supported_data_sources[name_type]
         return data_class.from_dict(value)
 
-    def consumer(self, from_timestamp: str | None = None) -> ReadableStream:
-        """Returns a consumer that actually can load data
-
-        E.g:
-        ```python
-        redis_config = RedisConfig(env_var="REDIS_URL")
-
-        consumer = redis_config.consumer()
-        ```
-
-        Returns:
-            ReadableStream: A stream you can read records from
-        """
+    def all_data(self, request: RetrivalRequest, limit: int | None) -> FullExtractJob:
         raise NotImplementedError()
 
+    def all_between_dates(
+        self,
+        request: RetrivalRequest,
+        start_date: datetime,
+        end_date: datetime,
+    ) -> DateRangeJob:
+        raise NotImplementedError()
 
-@dataclass
-class HttpStreamSource(StreamDataSource):
-
-    topic_name: str
-    mappings: dict[str, str] = field(default_factory=dict)
+    @classmethod
+    def feature_for(cls: type[T], facts: dict[str, list], requests: dict[T, RetrivalRequest]) -> RetrivalJob:
+        raise NotImplementedError()
 
-    name: str = 'http'
 
-    def map_values(self, mappings: dict[str, str]) -> HttpStreamSource:
-        return HttpStreamSource(topic_name=self.topic_name, mappings=self.mappings | mappings)
+class ColumnFeatureMappable:
+    mapping_keys: dict[str, str]
 
+    def columns_for(self, features: list[Feature]) -> list[str]:
+        return [self.mapping_keys.get(feature.name, feature.name) for feature in features]
 
-class SinkableDataSource:
-    async def write_to_stream(self, job: RetrivalJob) -> None:
-        pass
+    def feature_identifier_for(self, columns: list[str]) -> list[str]:
+        reverse_map = {v: k for k, v in self.mapping_keys.items()}
+        return [reverse_map.get(column, column) for column in columns]
```

### Comparing `aligned-0.0.94/aligned/enricher.py` & `aligned-0.0.9a0/aligned/enricher.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from __future__ import annotations
 
 import logging
 from abc import ABC, abstractmethod
+from contextlib import suppress
 from dataclasses import dataclass, field
 from datetime import datetime, timedelta
 from pathlib import Path
 
 import pandas as pd
 from mashumaro.types import SerializableType
 
+from aligned.redis.config import RedisConfig
 from aligned.schemas.codable import Codable
-from aligned.sources.redis import RedisConfig
+
+with suppress(ModuleNotFoundError):
+    import dask.dataframe as dd
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class TimespanSelector(Codable):
     timespand: timedelta
@@ -53,14 +57,18 @@
     def cache(self, ttl: timedelta, cache_key: str) -> Enricher:
         return FileCacheEnricher(ttl, cache_key, self)
 
     @abstractmethod
     async def as_df(self) -> pd.DataFrame:
         pass
 
+    @abstractmethod
+    async def as_dask(self) -> dd.DataFrame:
+        pass
+
 
 class SupportedEnrichers:
 
     types: dict[str, type[Enricher]]
 
     _shared: SupportedEnrichers | None = None
 
@@ -98,14 +106,19 @@
         self.timeout = timeout
 
     async def as_df(self) -> pd.DataFrame:
         redis = self.config.redis()
         async with redis.lock(self.lock_name, timeout=self.timeout) as _:
             return await self.enricher.as_df()
 
+    async def as_dask(self) -> dd.DataFrame:
+        redis = self.config.redis()
+        async with redis.lock(self.lock_name, timeout=self.timeout) as _:
+            return await self.enricher.as_dask()
+
 
 @dataclass
 class CsvFileSelectedEnricher(Enricher):
     file: str
     time: TimespanSelector | None = field(default=None)
     limit: int | None = field(default=None)
     name: str = 'selective_file'
@@ -128,14 +141,17 @@
         if not self.time:
             return file
 
         date = datetime.now() - self.time.timespand
         selector = file[self.time.time_column] >= date
         return file.loc[selector]
 
+    async def as_dask(self) -> dd.DataFrame:
+        return dd.read_csv(self.file)
+
 
 @dataclass
 class CsvFileEnricher(Enricher):
 
     file: str
     name: str = 'file'
 
@@ -143,14 +159,17 @@
         self, time: TimespanSelector | None = None, limit: int | None = None
     ) -> CsvFileSelectedEnricher:
         return CsvFileSelectedEnricher(self.file, time=time, limit=limit)
 
     async def as_df(self) -> pd.DataFrame:
         return pd.read_csv(self.file)
 
+    async def as_dask(self) -> dd.DataFrame:
+        return dd.read_csv(self.file)
+
 
 @dataclass
 class LoadedStatEnricher(Enricher):
 
     stat: str
     columns: list[str]
     enricher: Enricher
@@ -162,14 +181,24 @@
         if self.stat == 'mean':
             return renamed[self.columns].mean()
         elif self.stat == 'std':
             return renamed[self.columns].std()
         else:
             raise ValueError(f'Not supporting stat: {self.stat}')
 
+    async def as_dask(self) -> dd.DataFrame:
+        data = await self.enricher.as_dask()
+        renamed = data.rename(columns=self.mapping_keys)
+        if self.stat == 'mean':
+            return renamed[self.columns].mean()
+        elif self.stat == 'std':
+            return renamed[self.columns].std()
+        else:
+            raise ValueError(f'Not supporting stat: {self.stat}')
+
 
 @dataclass
 class FileCacheEnricher(Enricher):
 
     ttl: timedelta
     file_path: str
     enricher: Enricher
@@ -195,14 +224,28 @@
             logger.info(f'Storing cache at file {file_uri.as_uri()}')
             data.to_parquet(file_uri)
         else:
             logger.info('Loading cache')
             data = pd.read_parquet(file_uri)
         return data
 
+    async def as_dask(self) -> dd.DataFrame:
+        file_uri = Path(self.file_path).absolute()
+
+        if self.is_out_of_date_cache():
+            logger.info('Fetching from source')
+            data: dd.DataFrame = await self.enricher.as_dask()
+            file_uri.parent.mkdir(exist_ok=True, parents=True)
+            logger.info(f'Storing cache at file {file_uri.as_uri()}')
+            data.to_parquet(file_uri)
+        else:
+            logger.info('Loading cache')
+            data = dd.read_parquet(file_uri)
+        return data
+
 
 @dataclass
 class SqlDatabaseEnricher(Enricher):
 
     query: str
     values: dict | None
     url_env: str
@@ -212,16 +255,20 @@
         self.query = query
         self.values = values
         self.url_env = url_env
 
     async def as_df(self) -> pd.DataFrame:
         import os
 
-        import connectorx as cx
-
-        df = cx.read_sql(os.environ[self.url_env], self.query, return_type='pandas')
+        from databases import Database
 
+        async with Database(os.environ[self.url_env]) as db:
+            records = await db.fetch_all(self.query, values=self.values)
+        df = pd.DataFrame.from_records([dict(record) for record in records])
         for name, dtype in df.dtypes.iteritems():
             if dtype == 'object':  # Need to convert the databases UUID type
                 df[name] = df[name].astype('str')
-
         return df
+
+    async def as_dask(self) -> dd.DataFrame:
+        pdf = await self.as_df()
+        return dd.from_pandas(pdf)
```

### Comparing `aligned-0.0.94/aligned/feature_view/combined_view.py` & `aligned-0.0.9a0/aligned/feature_view/combined_view.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,159 +1,120 @@
 import logging
 from abc import ABC, abstractproperty
 from dataclasses import dataclass
-from typing import Generic, TypeVar, Any, Type, Callable, TYPE_CHECKING
+from typing import Callable
 
 from aligned.compiler.feature_factory import FeatureFactory
-from aligned.feature_view.feature_view import FeatureView
+from aligned.feature_view.feature_view import FeatureSelectable, FeatureView, FVType
 from aligned.request.retrival_request import RetrivalRequest
 from aligned.schemas.derivied_feature import DerivedFeature
-from aligned.schemas.feature import FeatureLocation
 from aligned.schemas.feature_view import CompiledCombinedFeatureView, CompiledFeatureView
 
-if TYPE_CHECKING:
-    from aligned.feature_store import FeatureViewStore
-
 logger = logging.getLogger(__name__)
 
-T = TypeVar('T')
-
 
 @dataclass
 class CombinedFeatureViewMetadata:
     name: str
     description: str | None = None
     tags: dict[str, str] | None = None
     owner: str | None = None
 
 
-@dataclass
-class CombinedFeatureViewWrapper(Generic[T]):
-
-    metadata: CombinedFeatureViewMetadata
-    view: Type[T]
-
-    def __call__(self) -> T:
-        # Needed to make sure that the `location` is set in the view's features
-        _ = self.compile()
-        return self.view()
-
-    def compile(self) -> CompiledCombinedFeatureView:
-        return CombinedFeatureView.compile_with_metadata(self.view(), self.metadata)
-
-    def query(self) -> 'FeatureViewStore':
-        """Makes it possible to query the feature view for features
-
-        ```python
-        @feature_view(...)
-        class SomeView:
-
-            id = Int32().as_entity()
-
-            a = Int32()
-            b = Int32()
-
-        data = await SomeView.query().features_for({
-            "id": [1, 2, 3],
-        }).to_pandas()
-        ```
-
-        Returns:
-            FeatureViewStore: Returns a queryable `FeatureViewStore` containing the feature view
-        """
-        from aligned import ContractStore
-
-        store = ContractStore.experimental()
-        store.add_combined_view(self.compile())
-        return store.feature_view(self.metadata.name)
-
-    async def process(self, data: dict[str, list[Any]]) -> list[dict]:
-        df = await self.query().process_input(data).to_lazy_polars()
-        return df.collect().to_dicts()
-
-
-def combined_feature_view(
-    name: str, description: str, tags: dict[str, str] | None = None, owner: str | None = None
-) -> Callable[[Type[T]], CombinedFeatureViewWrapper[T]]:
-    """
-    Wraps a view as a combined view
-
-    ```python
-    @combined_feature_view(
-        name="my_combined_view",
-        description="some description"
-    )
-    class MyView:
-
-        other = OtherView()
-        another = AnotherView()
-
-        y = other.x * another.y
-    ```
-    """
-
-    def decorator(cls: Type[T]) -> CombinedFeatureViewWrapper[T]:
-        return CombinedFeatureViewWrapper(
-            CombinedFeatureViewMetadata(name, description, tags=tags, owner=owner), cls
-        )
-
-    return decorator
-
-
-class CombinedFeatureView(ABC):
+class CombinedFeatureView(ABC, FeatureSelectable):
     @abstractproperty
     def metadata(self) -> CombinedFeatureViewMetadata:
-        raise NotImplementedError(f'Need to add a metadata field to in {self}')
+        pass
 
     @staticmethod
     def _needed_features(
-        depending_on: list[FeatureFactory], feature_views: dict[FeatureLocation, CompiledFeatureView]
+        depending_on: list[FeatureFactory], feature_views: dict[str, CompiledFeatureView]
     ) -> list[RetrivalRequest]:
 
         feature_refs: dict[CompiledFeatureView, set[str]] = {}
 
         for feature_dep in depending_on:
-            view = feature_views[feature_dep._location]
+            view = feature_views[feature_dep._feature_view]
             feature_refs.setdefault(view, set()).add(feature_dep.name)
 
         return [
             feature_view.request_for(features).needed_requests[0]
             for feature_view, features in feature_refs.items()
         ]
 
     @classmethod
-    def compile(cls) -> CompiledCombinedFeatureView:
-        instance = cls()
-        return CombinedFeatureView.compile_with_metadata(instance, instance.metadata)
+    async def compile(cls) -> CompiledCombinedFeatureView:
+        transformations: set[DerivedFeature] = set()
+        metadata = cls().metadata
+        var_names = [name for name in cls().__dir__() if not name.startswith('_')]
 
-    @staticmethod
-    def compile_with_metadata(
-        view: Any, metadata: CombinedFeatureViewMetadata
-    ) -> CompiledCombinedFeatureView:
+        requests: dict[str, list[RetrivalRequest]] = {}
+        feature_view_deps: dict[str, CompiledFeatureView] = {}
+
+        for var_name in var_names:
+            feature = getattr(cls, var_name)
+            if isinstance(feature, FeatureView):
+                # Needs to compile the view one more time. unfortunally..
+                # not optimal as the view will be duplicated in the definition file
+                feature_view_deps[feature.metadata.name] = await feature.compile()
+            if isinstance(feature, FeatureFactory):
+                feature._feature_view = metadata.name
+                feature._name = var_name  # Needed in some cases for later inferance and features
+                if not feature.transformation:
+                    logger.info('Feature had no transformation, which do not make sense in a CombinedView')
+                    continue
+                requests[var_name] = CombinedFeatureView._needed_features(
+                    feature.transformation.using_features, feature_view_deps
+                )
+
+                transformations.add(await feature.compile(list(feature_view_deps.values())))
+
+        return CompiledCombinedFeatureView(
+            name=metadata.name,
+            features=transformations,
+            feature_referances=requests,
+        )
+
+    @classmethod
+    def compile_only_graph(cls) -> CompiledCombinedFeatureView:
         transformations: set[DerivedFeature] = set()
-        var_names = [name for name in view.__dir__() if not name.startswith('_')]
+        metadata = cls().metadata
+        var_names = [name for name in cls().__dir__() if not name.startswith('_')]
 
         requests: dict[str, list[RetrivalRequest]] = {}
-        feature_view_deps: dict[FeatureLocation, CompiledFeatureView] = {}
+        feature_view_deps: dict[str, CompiledFeatureView] = {}
 
         for var_name in var_names:
-            feature = getattr(view, var_name)
+            feature = getattr(cls, var_name)
             if isinstance(feature, FeatureView):
                 # Needs to compile the view one more time. unfortunally..
                 # not optimal as the view will be duplicated in the definition file
-                feature_view_deps[FeatureLocation.feature_view(feature.metadata.name)] = feature.compile()
+                feature_view_deps[feature.metadata.name] = feature.compile_graph_only()
             if isinstance(feature, FeatureFactory):
-                feature._location = FeatureLocation.combined_view(var_name)
+                feature._feature_view = metadata.name
+                feature._name = var_name  # Needed in some cases for later inferance and features
                 if not feature.transformation:
                     logger.info('Feature had no transformation, which do not make sense in a CombinedView')
                     continue
                 requests[var_name] = CombinedFeatureView._needed_features(
                     feature.transformation.using_features, feature_view_deps
                 )
 
-                transformations.add(feature.compile())
+                transformations.add(feature.compile_graph_only())
 
         return CompiledCombinedFeatureView(
             name=metadata.name,
             features=transformations,
             feature_referances=requests,
         )
+
+    @classmethod
+    def select(
+        cls: type[FVType], features: Callable[[type[FVType]], list[FeatureFactory]]
+    ) -> RetrivalRequest:
+        view: CompiledCombinedFeatureView = cls.compile_only_graph()  # type: ignore[attr-defined]
+        names = features(cls)
+        return view.requests_for({feat.name for feat in names})
+
+    @classmethod
+    def select_all(cls: type[FVType]) -> RetrivalRequest:
+        return cls.compile_only_graph().request_all  # type: ignore[attr-defined]
```

### Comparing `aligned-0.0.94/aligned/feature_view/tests/test_brest_cancer.py` & `aligned-0.0.9a0/aligned/feature_view/tests/test_brest_cancer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import pytest
 
-from aligned import ContractStore
-from aligned.feature_view.feature_view import FeatureView
+from aligned import FeatureStore, FeatureView
 
 
 @pytest.mark.asyncio
 async def test_all_features(
-    breast_scan_without_timestamp_feature_store: ContractStore,
+    breast_scan_without_timestamp_feature_store: FeatureStore,
     breast_scan_feature_viewout_with_datetime: FeatureView,
 ) -> None:
     store = breast_scan_without_timestamp_feature_store
     feature_view = breast_scan_feature_viewout_with_datetime
 
     features = await store.feature_view(feature_view.metadata.name).all().to_pandas()
 
+    for feature in type(breast_scan_feature_viewout_with_datetime).select_all().features_to_include:
+        assert feature in features.columns
+
     assert 'is_malignant' in features.columns
     assert not features['is_malignant'].isna().any()
     assert 'diagnosis' in features.columns
     assert 'scan_id' in features.columns
 
     limit = 10
     limit_features = await store.feature_view(feature_view.metadata.name).all(limit=limit).to_pandas()
```

### Comparing `aligned-0.0.94/aligned/feature_view/tests/test_brest_cancer_event_timestamp.py` & `aligned-0.0.9a0/aligned/feature_view/tests/test_brest_cancer_event_timestamp.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,84 +1,93 @@
 from datetime import datetime
 
 import pytest
 
-from aligned import ContractStore
-from aligned.feature_view.feature_view import FeatureView
+from aligned import FeatureStore, FeatureView
 
 
 @pytest.mark.asyncio
 async def test_between_datetime_features(
     breast_scan_feature_view_with_datetime: FeatureView,
-    breast_scan_with_timestamp_feature_store: ContractStore,
+    breast_scan_with_timestamp_feature_store: FeatureStore,
 ) -> None:
     feature_view = breast_scan_feature_view_with_datetime
     store = breast_scan_with_timestamp_feature_store
     features = await store.feature_view(feature_view.metadata.name).all().to_pandas()
 
+    for feature in type(feature_view).select_all().features_to_include:
+        assert feature in features.columns
+
     assert 'created_at' in features.columns
     assert 'is_malignant' in features.columns
     assert 'diagnosis' in features.columns
     assert 'scan_id' in features.columns
 
     limit_features = (
         await store.feature_view(feature_view.metadata.name)
-        .between_dates(
+        .between(
             start_date=datetime(2020, 1, 5),
             end_date=datetime(2020, 1, 11),
         )
         .to_pandas()
     )
     assert limit_features.shape[0] == 6
 
 
 @pytest.mark.asyncio
 async def test_between_datetime_features_with_aggregation(
     breast_scan_feature_view_with_datetime_and_aggregation: FeatureView,
-    breast_scan_with_timestamp_and_aggregation_feature_store: ContractStore,
+    breast_scan_with_timestamp_and_aggregation_feature_store: FeatureStore,
 ) -> None:
     feature_view = breast_scan_feature_view_with_datetime_and_aggregation
     store = breast_scan_with_timestamp_and_aggregation_feature_store
     features = await store.feature_view(feature_view.metadata.name).all().to_pandas()
 
+    for feature in type(feature_view).select_all().features_to_include:
+        assert feature in features.columns
+
     assert 'created_at' in features.columns
     assert 'is_malignant' in features.columns
     assert 'diagnosis' in features.columns
     assert 'scan_id' in features.columns
 
     limit_features = (
         await store.feature_view(feature_view.metadata.name)
-        .between_dates(
+        .between(
             start_date=datetime(2020, 1, 5),
             end_date=datetime(2020, 1, 11),
         )
         .to_pandas()
     )
 
     assert limit_features.shape[0] == 6
+    assert features['mean_fd_worst_for_group'].isna().count() != 0
+
+
+@pytest.mark.asyncio
+async def test_between_datetime_features_polars(
+    breast_scan_feature_view_with_datetime: FeatureView,
+    breast_scan_with_timestamp_feature_store: FeatureStore,
+) -> None:
+    feature_view = breast_scan_feature_view_with_datetime
+    store = breast_scan_with_timestamp_feature_store
+    job = store.feature_view(feature_view.metadata.name).all()
+    features = (await job.to_polars()).collect()
+
+    for feature in type(feature_view).select_all().features_to_include:
+        assert feature in features.columns
 
+    assert 'created_at' in features.columns
+    assert 'is_malignant' in features.columns
+    assert 'diagnosis' in features.columns
+    assert 'scan_id' in features.columns
 
-# @pytest.mark.asyncio
-# async def test_between_datetime_features_polars(
-#     breast_scan_feature_view_with_datetime: FeatureView,
-#     breast_scan_with_timestamp_feature_store: FeatureStore,
-# ) -> None:
-#     feature_view = breast_scan_feature_view_with_datetime
-#     store = breast_scan_with_timestamp_feature_store
-#     job = store.feature_view(feature_view.metadata.name).all()
-#     features = (await job.to_polars()).collect()
-
-#     assert 'created_at' in features.columns
-#     assert 'is_malignant' in features.columns
-#     assert 'diagnosis' in features.columns
-#     assert 'scan_id' in features.columns
-
-#     limit_features = (
-#         await store.feature_view(feature_view.metadata.name)
-#         .between_dates(
-#             start_date=datetime(2020, 1, 5),
-#             end_date=datetime(2020, 1, 11),
-#         )
-#         .to_polars()
-#     ).collect()
+    limit_features = (
+        await store.feature_view(feature_view.metadata.name)
+        .between(
+            start_date=datetime(2020, 1, 5),
+            end_date=datetime(2020, 1, 11),
+        )
+        .to_polars()
+    ).collect()
 
-#     assert limit_features.shape[0] == 6
+    assert limit_features.shape[0] == 6
```

### Comparing `aligned-0.0.94/aligned/jobs/tests/test_combined_job.py` & `aligned-0.0.9a0/aligned/jobs/tests/test_combined_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,11 +23,11 @@
     retrival_job: RetrivalJob,
     retrival_job_with_timestamp: RetrivalJob,
     combined_retrival_request: RetrivalRequest,
 ) -> None:
     job = CombineFactualJob(
         jobs=[retrival_job, retrival_job_with_timestamp], combined_requests=[combined_retrival_request]
     )
-    data = (await job.to_lazy_polars()).collect()
+    data = (await job.to_polars()).collect()
 
     assert set(data.columns) == {'id', 'a', 'b', 'c', 'd', 'created_at', 'c+d', 'a+c+d'}
     assert data.shape[0] == 5
```

### Comparing `aligned-0.0.94/aligned/request/tests/test_feature_request_generation.py` & `aligned-0.0.9a0/aligned/request/tests/test_feature_request_generation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pytest
 
-from aligned.feature_view.feature_view import FeatureView
+from aligned import FeatureView
 
 
 @pytest.mark.asyncio
 async def test_fetch_all_request(titanic_feature_view: FeatureView) -> None:
 
-    compiled_view = type(titanic_feature_view).compile()
+    compiled_view = await type(titanic_feature_view).compile()
     request = compiled_view.request_all
 
     expected_features = {
         'age',
         'name',
         'sex',
         'survived',
@@ -33,23 +33,21 @@
     assert len(request.request_result.entities) == 1
     assert len(request.request_result.features) == len(expected_features)
 
 
 @pytest.mark.asyncio
 async def test_fetch_features_request(titanic_feature_view: FeatureView) -> None:
 
-    compiled_view = type(titanic_feature_view).compile()
+    compiled_view = await type(titanic_feature_view).compile()
     wanted_features = {'cabin', 'is_male'}
     request = compiled_view.request_for(wanted_features)
     expected_features = {'sex', 'cabin', 'is_male'}
     assert not request.needs_event_timestamp
     assert len(request.needed_requests) == 1
 
     retrival_request = request.needed_requests[0]
     missing_features = expected_features - retrival_request.all_feature_names
-    # All the features to retrive and computed
     assert retrival_request.all_feature_names == expected_features, f'Missing features {missing_features}'
     assert retrival_request.entity_names == {'passenger_id'}
 
-    # All the features that is returned
     assert len(request.request_result.entities) == 1
-    assert len(request.request_result.features) == len(wanted_features)
+    assert len(request.request_result.features) == len(expected_features)
```

### Comparing `aligned-0.0.94/aligned/schemas/constraints.py` & `aligned-0.0.9a0/aligned/schemas/constraints.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from dataclasses import dataclass
-from typing import Optional as OptionalType
+from typing import Optional
 
 from mashumaro.types import SerializableType
 
 from aligned.schemas.codable import Codable
 
 
 class Constraint(Codable, SerializableType):
     name: str
 
     def __hash__(self) -> int:
         return hash(self.name)
 
     def _serialize(self) -> dict:
-        assert self.name in SupportedConstraints.shared().types, f'Constraint {self.name} is not supported'
         return self.to_dict()
 
     @classmethod
     def _deserialize(cls, value: dict) -> 'Constraint':
         name_type = value['name']
         del value['name']
         data_class = SupportedConstraints.shared().types[name_type]
@@ -25,38 +24,26 @@
         return data_class.from_dict(value)
 
 
 class SupportedConstraints:
 
     types: dict[str, type[Constraint]]
 
-    _shared: OptionalType['SupportedConstraints'] = None
+    _shared: Optional['SupportedConstraints'] = None
 
     def __init__(self) -> None:
-        from aligned.schemas.constraint_types import (
-            ReferencingColumn,
-        )
-
         self.types = {}
 
         for tran_type in [
             LowerBound,
             LowerBoundInclusive,
             UpperBound,
             UpperBoundInclusive,
             Required,
-            Optional,
             InDomain,
-            MaxLength,
-            MinLength,
-            StartsWith,
-            EndsWith,
-            Unique,
-            Regex,
-            ReferencingColumn,
         ]:
             self.add(tran_type)
 
     def add(self, constraint: type[Constraint]) -> None:
         self.types[constraint.name] = constraint
 
     @classmethod
@@ -104,72 +91,14 @@
     name = 'upper_bound_inc'
 
     def __hash__(self) -> int:
         return hash(self.name)
 
 
 @dataclass
-class Unique(Constraint):
-    name = 'unique'
-
-    def __hash__(self) -> int:
-        return hash(self.name)
-
-
-@dataclass
-class MinLength(Constraint):
-    value: int
-
-    name = 'min_length'
-
-    def __hash__(self) -> int:
-        return hash(self.name)
-
-
-@dataclass
-class Regex(Constraint):
-    value: str
-
-    name = 'regex'
-
-    def __hash__(self) -> int:
-        return hash(self.name)
-
-
-@dataclass
-class EndsWith(Constraint):
-    value: str
-
-    name = 'ends_with'
-
-    def __hash__(self) -> int:
-        return hash(self.name)
-
-
-@dataclass
-class StartsWith(Constraint):
-    value: str
-
-    name = 'starts_with'
-
-    def __hash__(self) -> int:
-        return hash(self.name)
-
-
-@dataclass
-class MaxLength(Constraint):
-    value: int
-
-    name = 'max_length'
-
-    def __hash__(self) -> int:
-        return hash(self.name)
-
-
-@dataclass
 class And(Constraint):
 
     left: Constraint
     right: Constraint
     name = 'and'
 
     def __hash__(self) -> int:
@@ -182,23 +111,14 @@
     name = 'requierd'
 
     def __hash__(self) -> int:
         return hash(self.name)
 
 
 @dataclass
-class Optional(Constraint):
-
-    name = 'optional'
-
-    def __hash__(self) -> int:
-        return hash(self.name)
-
-
-@dataclass
 class InDomain(Constraint):
 
     values: list[str]
     name = 'in_domain'
 
     def __hash__(self) -> int:
         return hash(self.name)
```

### Comparing `aligned-0.0.94/aligned/server.py` & `aligned-0.0.9a0/aligned/server.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,22 @@
-from __future__ import annotations
-
 import asyncio
 import logging
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any
 
 from fastapi import FastAPI, HTTPException, Response
-from fastapi.responses import RedirectResponse
 from numpy import nan
 from pydantic import BaseModel
 
 from aligned.data_source.stream_data_source import HttpStreamSource
 from aligned.feature_source import WritableFeatureSource
-from aligned.feature_store import ContractStore
+from aligned.feature_store import FeatureStore
 from aligned.schemas.feature import Feature
 from aligned.schemas.feature_view import CompiledFeatureView
-from aligned.sources.local import StorageFileReference
 
 logger = logging.getLogger(__name__)
 
 
 class APIFeatureRequest(BaseModel):
     entities: dict[str, list]
     features: list[str]
@@ -31,15 +27,15 @@
     name: str
     views: list[CompiledFeatureView]
     mappings: dict[str, str]
 
 
 class FastAPIServer:
     @staticmethod
-    def write_to_topic_path(topic: TopicInfo, feature_store: ContractStore, app: FastAPI) -> None:
+    def write_to_topic_path(topic: TopicInfo, feature_store: FeatureStore, app: FastAPI) -> None:
 
         required_features: set[Feature] = set()
         for view in topic.views:
             required_features.update(view.entities.union(view.features))
 
         view_names = [view.name for view in topic.views]
         mappings: dict[str, list[str]] = {
@@ -91,28 +87,25 @@
                     feature_values[output_name] = [value if value != {} else None for value in values]
 
             await asyncio.gather(
                 *[feature_store.feature_view(view_name).write(feature_values) for view_name in view_names]
             )
 
     @staticmethod
-    def feature_view_path(name: str, feature_store: ContractStore, app: FastAPI) -> None:
+    def feature_view_path(name: str, feature_store: FeatureStore, app: FastAPI) -> None:
         @app.post(f'/feature-views/{name}/all')
         async def all(limit: int | None = None) -> dict:
             df = await feature_store.feature_view(name).all(limit=limit).to_pandas()
             df.replace(nan, value=None, inplace=True)
             return df.to_dict('list')
 
     @staticmethod
-    def model_path(name: str, feature_store: ContractStore, app: FastAPI) -> None:
-        from aligned.feature_store import RawStringFeatureRequest
-
-        model = feature_store.models[name]
-        features = {f'{feature.location.identifier}:{feature.name}' for feature in model.features}
-        feature_request = feature_store.requests_for(RawStringFeatureRequest(features))
+    def model_path(name: str, feature_store: FeatureStore, app: FastAPI) -> None:
+        model = feature_store.model_requests[name]
+        feature_request = feature_store.requests_for_model(model)
 
         entities: set[Feature] = set()
         for request in feature_request.needed_requests:
             entities.update(request.entities)
 
         required_features = entities.copy()
         for request in feature_request.needed_requests:
@@ -155,43 +148,28 @@
                 entity_values['event_timestamp'] = [
                     datetime.fromtimestamp(value)
                     if isinstance(value, (float, int))
                     else datetime.fromisoformat(value)
                     for value in entity_values['event_timestamp']
                 ]
 
-            df = await feature_store.model(name).features_for(entity_values).to_lazy_polars()
-            pandas_df = df.collect().to_pandas()
+            df = await feature_store.model(name).features_for(entity_values).to_pandas()
             orient = 'values'
-            body = ','.join(
-                [f'"{column}":{pandas_df[column].to_json(orient=orient)}' for column in pandas_df.columns]
-            )
+            body = ','.join([f'"{column}":{df[column].to_json(orient=orient)}' for column in df.columns])
             return Response(content=f'{{{body}}}', media_type='application/json')
 
     @staticmethod
-    def app(feature_store: ContractStore, auth_tokens: list[str] | None = None) -> FastAPI:
+    def app(feature_store: FeatureStore) -> FastAPI:
         from asgi_correlation_id import CorrelationIdMiddleware
         from fastapi import FastAPI
         from fastapi.middleware import Middleware
-        from prometheus_fastapi_instrumentator import Instrumentator
-        from starlette.status import HTTP_200_OK
 
         app = FastAPI(middleware=[Middleware(CorrelationIdMiddleware)])
         app.docs_url = '/docs'
 
-        prom_instrument = Instrumentator().instrument(app)
-
-        @app.on_event('startup')
-        async def startup():
-            prom_instrument.expose(app)
-
-        @app.get('health', status_code=HTTP_200_OK)
-        def health() -> None:
-            return
-
         for model in feature_store.all_models:
             FastAPIServer.model_path(model, feature_store, app)
 
         can_write_to_store = isinstance(feature_store.feature_source, WritableFeatureSource)
 
         topics: dict[str, TopicInfo] = {}
 
@@ -221,49 +199,31 @@
             logger.info(
                 (
                     'Warning! The server is not using a WritableFeatureSource, ',
                     'and can therefore not setup stream sources',
                 )
             )
 
-        @app.get('/')
-        async def root() -> RedirectResponse:
-            return RedirectResponse('/docs')
-
         @app.post('/features')
         async def features(payload: APIFeatureRequest) -> dict:
-            import json
-
             df = await feature_store.features_for(
-                payload.entities, features=payload.features
-            ).to_lazy_polars()
-            json_data = json.dumps(df.collect().to_dict(as_series=False))
-            return Response(content=json_data, media_type='application/json')
+                payload.entities,
+                features=payload.features,
+            ).to_pandas()
+            orient = 'values'
+            body = ','.join([f'"{column}":{df[column].to_json(orient=orient)}' for column in df.columns])
+            return Response(content=f'{{{body}}}', media_type='application/json')
 
         return app
 
     @staticmethod
     def run(
-        feature_store: ContractStore,
+        feature_store: FeatureStore,
         host: str | None = None,
         port: int | None = None,
         workers: int | None = None,
     ) -> None:
         import uvicorn
 
         app = FastAPIServer.app(feature_store)
 
         uvicorn.run(app, host=host or '127.0.0.1', port=port or 8000, workers=workers or workers)
-
-
-class FeatureServer:
-
-    definition_reference: StorageFileReference
-    auth_keys: list[str] | None = None
-
-    @staticmethod
-    def from_reference(source: StorageFileReference) -> FeatureServer:
-        return FeatureServer(source)
-
-    async def build_app(self) -> FastAPI:
-        definitions = await self.definition_reference.feature_store()
-        return FastAPIServer.app(definitions)
```

### Comparing `aligned-0.0.94/aligned/sources/s3.py` & `aligned-0.0.9a0/aligned/s3/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,21 @@
 from dataclasses import dataclass
 from datetime import datetime
 from io import BytesIO
 
 import pandas as pd
-import polars as pl
 from httpx import HTTPStatusError
 
 from aligned.data_source.batch_data_source import BatchDataSource, ColumnFeatureMappable
 from aligned.exceptions import UnableToFindFileException
 from aligned.local.job import FileDateJob, FileFullJob
-from aligned.retrival_job import RetrivalRequest, RetrivalJob
+from aligned.local.source import CsvConfig, DataFileReference, ParquetConfig, StorageFileReference
+from aligned.retrival_job import DateRangeJob, FullExtractJob, RetrivalRequest
 from aligned.s3.storage import AwsS3Storage
 from aligned.schemas.codable import Codable
-from aligned.sources.local import (
-    CsvConfig,
-    DataFileReference,
-    ParquetConfig,
-    StorageFileReference,
-    Directory,
-    DeltaFileConfig,
-)
 from aligned.storage import Storage
 
 try:
     from aioaws.s3 import S3Config
 except ModuleNotFoundError:
 
     class S3Config:  # type: ignore[no-redef]
@@ -53,15 +45,15 @@
     def url(self) -> str:
         import os
 
         region = os.environ[self.bucket_env]
         bucket = os.environ[self.bucket_env]
         return f'https://{region}.amazoneaws.com/{bucket}/'
 
-    def json_at(self, path: str, mapping_keys: dict[str, str] | None = None) -> 'AwsS3DataSource':
+    def file_at(self, path: str, mapping_keys: dict[str, str] | None = None) -> 'AwsS3DataSource':
         return AwsS3DataSource(config=self, path=path)
 
     def csv_at(
         self, path: str, mapping_keys: dict[str, str] | None = None, csv_config: CsvConfig | None = None
     ) -> 'AwsS3CsvDataSource':
         return AwsS3CsvDataSource(
             config=self, path=path, mapping_keys=mapping_keys or {}, csv_config=csv_config or CsvConfig()
@@ -70,67 +62,20 @@
     def parquet_at(
         self, path: str, mapping_keys: dict[str, str] | None = None, config: ParquetConfig | None = None
     ) -> 'AwsS3ParquetDataSource':
         return AwsS3ParquetDataSource(
             config=self, path=path, mapping_keys=mapping_keys or {}, parquet_config=config or ParquetConfig()
         )
 
-    def sub_directory(self, path: str) -> 'AwsS3Directory':
-        return AwsS3Directory(config=self, path=path)
-
-    def directory(self, path: str) -> 'AwsS3Directory':
-        return self.sub_directory(path)
-
     @property
     def storage(self) -> Storage:
         return AwsS3Storage(self)
 
 
 @dataclass
-class AwsS3Directory(Directory):
-
-    config: AwsS3Config
-    path: str
-
-    def json_at(self, path: str) -> 'AwsS3DataSource':
-        return AwsS3DataSource(config=self.config, path=f'{self.path}/{path}')
-
-    def csv_at(
-        self, path: str, mapping_keys: dict[str, str] | None = None, csv_config: CsvConfig | None = None
-    ) -> 'AwsS3CsvDataSource':
-        return AwsS3CsvDataSource(
-            config=self.config,
-            path=f'{self.path}/{path}',
-            mapping_keys=mapping_keys or {},
-            csv_config=csv_config or CsvConfig(),
-        )
-
-    def parquet_at(
-        self, path: str, mapping_keys: dict[str, str] | None = None, config: ParquetConfig | None = None
-    ) -> 'AwsS3ParquetDataSource':
-        return AwsS3ParquetDataSource(
-            config=self.config,
-            path=f'{self.path}/{path}',
-            mapping_keys=mapping_keys or {},
-            parquet_config=config or ParquetConfig(),
-        )
-
-    def delta_at(
-        self, path: str, mapping_keys: dict[str, str] | None = None, config: DeltaFileConfig | None = None
-    ) -> BatchDataSource:
-        raise NotImplementedError(type(self))
-
-    def sub_directory(self, path: str) -> 'AwsS3Directory':
-        return AwsS3Directory(config=self.config, path=f'{self.path}/{path}')
-
-    def directory(self, path: str) -> 'AwsS3Directory':
-        return self.sub_directory(path)
-
-
-@dataclass
 class AwsS3DataSource(StorageFileReference, ColumnFeatureMappable):
 
     config: AwsS3Config
     path: str
 
     type_name: str = 'aws_s3'
 
@@ -190,41 +135,32 @@
             sep=self.csv_config.seperator,
             index=self.csv_config.should_write_index,
             compression=self.csv_config.compression,
         )
         buffer.seek(0)
         await self.storage.write(self.path, buffer.read())
 
-    async def write_polars(self, df: pl.LazyFrame) -> None:
-        buffer = BytesIO()
-        df.collect().write_csv(
-            buffer,
-            sep=self.csv_config.seperator,
-        )
-        buffer.seek(0)
-        await self.storage.write(self.path, buffer.read())
-
-    def all_data(self, request: RetrivalRequest, limit: int | None) -> RetrivalJob:
+    def all_data(self, request: RetrivalRequest, limit: int | None) -> FullExtractJob:
         return FileFullJob(self, request=request, limit=limit)
 
     def all_between_dates(
         self, request: RetrivalRequest, start_date: datetime, end_date: datetime
-    ) -> RetrivalJob:
+    ) -> DateRangeJob:
         return FileDateJob(self, request, start_date, end_date)
 
 
 @dataclass
 class AwsS3ParquetDataSource(BatchDataSource, DataFileReference, ColumnFeatureMappable):
 
     config: AwsS3Config
     path: str
-    mapping_keys: dict[str, str]
+    mapping_keys: dict[str, str]  # = field(default_factory=dict)
 
-    parquet_config: ParquetConfig
-    type_name: str = 'aws_s3_parquet'
+    parquet_config: ParquetConfig  # = field(default_factory=ParquetConfig)
+    type_name: str = 'aws_s3_parquet'  # = field(default='aws_s3_parquet')
 
     def job_group_key(self) -> str:
         return f'{self.type_name}/{self.path}'
 
     @property
     def storage(self) -> Storage:
         return self.config.storage
@@ -239,28 +175,12 @@
             buffer = BytesIO(data)
             return pd.read_parquet(buffer)
         except FileNotFoundError:
             raise UnableToFindFileException()
         except HTTPStatusError:
             raise UnableToFindFileException()
 
-    async def to_lazy_polars(self) -> pl.LazyFrame:
-        try:
-            data = await self.storage.read(self.path)
-            buffer = BytesIO(data)
-            return pl.read_parquet(buffer).lazy()
-        except FileNotFoundError:
-            raise UnableToFindFileException()
-        except HTTPStatusError:
-            raise UnableToFindFileException()
-
     async def write_pandas(self, df: pd.DataFrame) -> None:
         buffer = BytesIO()
-        df.to_parquet(buffer, compression=self.parquet_config.compression, engine=self.parquet_config.engine)
-        buffer.seek(0)
-        await self.storage.write(self.path, buffer.read())
-
-    async def write_polars(self, df: pl.LazyFrame) -> None:
-        buffer = BytesIO()
-        df.collect().write_parquet(buffer, compression=self.parquet_config.compression)
+        df.to_parquet(buffer)
         buffer.seek(0)
         await self.storage.write(self.path, buffer.read())
```

### Comparing `aligned-0.0.94/aligned/tests/test_cache_enricher.py` & `aligned-0.0.9a0/aligned/tests/test_cache_enricher.py`

 * *Files identical despite different names*

### Comparing `aligned-0.0.94/aligned/tests/test_cached_parquet.py` & `aligned-0.0.9a0/aligned/tests/test_cached_parquet.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 import pytest
 
-from aligned import ContractStore, FileSource
+from aligned import FeatureStore, FileSource
 
 
 @pytest.mark.asyncio
-async def test_cached_at(titanic_feature_store: ContractStore) -> None:
-    """
-    Checks that we load all rows form the cached file.
-    """
+async def test_cached_at(titanic_feature_store: FeatureStore) -> None:
     file_source = FileSource.parquet_at('test_data/titanic.parquet')
-
-    cached = await file_source.read_pandas()
     data_set = (
         await titanic_feature_store.feature_view('titanic_parquet').all().cached_at(file_source).to_pandas()
     )
+    cached = await file_source.read_pandas()
 
     assert cached.shape[0] == data_set.shape[0]
     assert (set(cached.columns).intersection(set(data_set.columns)) - set(cached.columns)) == set()
```

### Comparing `aligned-0.0.94/aligned/tests/test_statistic_enricher.py` & `aligned-0.0.9a0/aligned/tests/test_statistic_enricher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import timedelta
 
 import pandas as pd
 import pytest
 from freezegun import freeze_time
 
 from aligned.enricher import TimespanSelector
-from aligned.sources.local import CsvFileSource
+from aligned.local.source import CsvFileSource
 
 
 @pytest.mark.asyncio
 async def test_statistic_enricher(scan_with_datetime: CsvFileSource) -> None:
     columns = {'fractal_dimension_worst', 'symmetry_worst'}
     file = await scan_with_datetime.mean(columns=columns).as_df()
     limit_file = await scan_with_datetime.mean(columns=columns, limit=3).as_df()
```

### Comparing `aligned-0.0.94/pyproject.toml` & `aligned-0.0.9a0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 [tool.poetry]
 name = "aligned"
-version = "0.0.94"
-description = "A data managment and lineage tool for ML applications."
+version = "0.0.9a"
+description = "A scalable feature store that makes it easy to align offline and online ML systems"
 authors = ["Mats E. Mollestad <mats@mollestad.no>"]
 license = "Apache-2.0"
 readme = "README.md"
-homepage = "https://github.com/MatsMoll/aligned"
-repository = "https://github.com/MatsMoll/aligned"
+homepage = "https://github.com/otovo/aladdin"
+repository = "https://github.com/otovo/aladdin"
 keywords = [
     'python',
     'typed',
     'ml',
     'prediction',
     'feature',
     'store',
     'feature-store',
-    'mlops',
     'feast',
     'tecton',
-    'dbt',
-    'data',
-    'lineage'
 ]
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Environment :: Web Environment',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
     'Operating System :: OS Independent',
@@ -40,63 +36,46 @@
 ]
 packages = [
     { include = "aligned" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-python-dotenv = "^0.21.0"
 click = "^8.1.3"
-pandas = "^2.0.0"
-fastapi = { version = "^0.100.0", optional = true }
+pandas = "^1.3.1"
+fastapi = { version = "^0.77.1", optional = true }
 uvicorn = { version = "^0.17.6", optional = true }
 redis = { version = "^4.3.1", optional = true }
 mashumaro = "^3.0.1"
 dill = "^0.3.4"
 aioaws = { version = "^0.12", optional = true }
+databases = { version = "^0.5.5", optional = true }
+asyncpg = { version = "^0.25.0", optional = true }
+pyarrow = "^8.0.0"
 Jinja2 = "^3.1.2"
 nest-asyncio = "^1.5.5"
-pydantic = "^2.0.0"
-prometheus_client = "^0.16.0"
 asgi-correlation-id = { version = "^3.0.0", optional = true }
-pandera = { version = "^0.17.0", optional = true}
-polars = { version = "^0.20.0", extras = ["pyarrow"] }
-pillow = { version = "^9.4.0", optional = true }
-prometheus-fastapi-instrumentator = { version="^5.9.1", optional = true }
-kafka-python = { version= "^2.0.2", optional = true }
-connectorx = { version = "^0.3.2", optional = true }
-asyncpg = { version = "^0.29.0", optional = true }
-sqlglot = { version = "^22.5.0", optional = true }
-ollama = { version = "^0.1.8", optional = true }
-httpx = "^0.27.0"
-mlflow = { version = "^2.11.3", optional = true }
+dask = {version = "^2022.7.0", extras = ["dataframe"], optional = true}
+pandera = {version = "^0.13.3", optional = true}
+httpx = "^0.23.0"
+polars = { version = "^0.15.6", extras = ["all"] }
 
 [tool.poetry.extras]
-aws = ["aioaws", "connectorx"]
-psql = ["connectorx", "asyncpg"]
+aws = ["aioaws", "databases"]
+psql = ["databases", "asyncpg"]
 redis = ["redis"]
-server = ["asgi-correlation-id", "fastapi", "uvicorn", "prometheus-fastapi-instrumentator"]
+server = ["asgi-correlation-id", "fastapi", "uvicorn"]
+dask = ["dask"]
 pandera = ["pandera"]
-image = ["pillow"]
-kafka = ["kafka-python"]
-ollama = ["ollama"]
-sql = ["sqlglot"]
-mlflow = ["mlflow"]
 
 [tool.poetry.group.dev.dependencies]
 types-redis = "^4.2.6"
 pytest-mock = "^3.8.1"
 freezegun = "^1.2.2"
 pytest-asyncio = "^0.20.1"
-fakeredis = "^2.10.0"
-sqlalchemy = "^2.0.19"
-printf-log-formatter = "^0.3.0"
-isort = "^5.12.0"
-black = "^23.7.0"
-psycopg2 = "^2.9.6"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 aligned = 'aligned.cli:cli'
```

### Comparing `aligned-0.0.94/PKG-INFO` & `aligned-0.0.9a0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,375 +1,341 @@
 Metadata-Version: 2.1
 Name: aligned
-Version: 0.0.94
-Summary: A data managment and lineage tool for ML applications.
-Home-page: https://github.com/MatsMoll/aligned
+Version: 0.0.9a0
+Summary: A scalable feature store that makes it easy to align offline and online ML systems
+Home-page: https://github.com/otovo/aladdin
 License: Apache-2.0
-Keywords: python,typed,ml,prediction,feature,store,feature-store,mlops,feast,tecton,dbt,data,lineage
+Keywords: python,typed,ml,prediction,feature,store,feature-store,feast,tecton
 Author: Mats E. Mollestad
 Author-email: mats@mollestad.no
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: aws
-Provides-Extra: image
-Provides-Extra: kafka
-Provides-Extra: mlflow
-Provides-Extra: ollama
+Provides-Extra: dask
 Provides-Extra: pandera
 Provides-Extra: psql
 Provides-Extra: redis
 Provides-Extra: server
-Provides-Extra: sql
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: aioaws (>=0.12,<0.13) ; extra == "aws"
 Requires-Dist: asgi-correlation-id (>=3.0.0,<4.0.0) ; extra == "server"
-Requires-Dist: asyncpg (>=0.29.0,<0.30.0) ; extra == "psql"
+Requires-Dist: asyncpg (>=0.25.0,<0.26.0) ; extra == "psql"
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: connectorx (>=0.3.2,<0.4.0) ; extra == "aws" or extra == "psql"
+Requires-Dist: dask[dataframe] (>=2022.7.0,<2023.0.0) ; extra == "dask"
+Requires-Dist: databases (>=0.5.5,<0.6.0) ; extra == "aws" or extra == "psql"
 Requires-Dist: dill (>=0.3.4,<0.4.0)
-Requires-Dist: fastapi (>=0.100.0,<0.101.0) ; extra == "server"
-Requires-Dist: httpx (>=0.27.0,<0.28.0)
-Requires-Dist: kafka-python (>=2.0.2,<3.0.0) ; extra == "kafka"
+Requires-Dist: fastapi (>=0.77.1,<0.78.0) ; extra == "server"
+Requires-Dist: httpx (>=0.23.0,<0.24.0)
 Requires-Dist: mashumaro (>=3.0.1,<4.0.0)
-Requires-Dist: mlflow (>=2.11.3,<3.0.0) ; extra == "mlflow"
 Requires-Dist: nest-asyncio (>=1.5.5,<2.0.0)
-Requires-Dist: ollama (>=0.1.8,<0.2.0) ; extra == "ollama"
-Requires-Dist: pandas (>=2.0.0,<3.0.0)
-Requires-Dist: pandera (>=0.17.0,<0.18.0) ; extra == "pandera"
-Requires-Dist: pillow (>=9.4.0,<10.0.0) ; extra == "image"
-Requires-Dist: polars[pyarrow] (>=0.20.0,<0.21.0)
-Requires-Dist: prometheus-fastapi-instrumentator (>=5.9.1,<6.0.0) ; extra == "server"
-Requires-Dist: prometheus_client (>=0.16.0,<0.17.0)
-Requires-Dist: pydantic (>=2.0.0,<3.0.0)
-Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
+Requires-Dist: pandas (>=1.3.1,<2.0.0)
+Requires-Dist: pandera (>=0.13.3,<0.14.0) ; extra == "pandera"
+Requires-Dist: polars[all] (>=0.15.6,<0.16.0)
+Requires-Dist: pyarrow (>=8.0.0,<9.0.0)
 Requires-Dist: redis (>=4.3.1,<5.0.0) ; extra == "redis"
-Requires-Dist: sqlglot (>=22.5.0,<23.0.0) ; extra == "sql"
 Requires-Dist: uvicorn (>=0.17.6,<0.18.0) ; extra == "server"
-Project-URL: Repository, https://github.com/MatsMoll/aligned
+Project-URL: Repository, https://github.com/otovo/aladdin
 Description-Content-Type: text/markdown
 
 # Aligned
 
-A data managment tool for ML applications.
-
-Similar to how DBT is a data managment tool for business analytics, will Aligned manage ML projects.
-
-Aligned does this through two things.
-1. A light weight data managment system. Making it possible to query a data lake and databases.
-2. Tooling to define a `model_contract`. Clearing up common unanswerd questions through code.
-
-
-Furthermore, Aligned collect data lineage between models, basic feature transformations. While also making it easy to reduce data leakage with point-in-time valid data and fix other problems described in [Sculley et al. [2015]](https://papers.nips.cc/paper/2015/file/86df7dcfd896fcaf2674f757a2463eba-Paper.pdf).
-
-## Examples
+Aligned help defining a single source of truth for logic while keeping the technology stack flexible. Such innovation has been possible by removing the need to depend on a processing engine, leading to less- and more transparent- code. Furthermore, the declarative API has made it possible to comment, add data validation, and define feature transformation at the same location. Therefore, it leads to a precise definition of the intended result.
 
-Bellow are some examples of how Aligned can be used.
+Read the post about [how the most elegant MLOps tool was created](https://matsmoll.github.io/2022/12/31/How-I-created-the-most-elegant-MLOps-tool.html)
 
-### Aligned UI
+Also check out the the [example repo](https://github.com/otovo/aligned-example) to see how it can be used
 
-Aligned provides an UI to view which data exists, the expectations we have and find faults.
+⚠️ Aligned is in alpha, so bugs will be likely. Even though Otovo use this for production.
 
-[View the example UI](https://aligned-catalog.azurewebsites.net/).
-However, this is still under development, so sign up for a [wait list](https://aligned-managed-web.vercel.app/) to get access.
-
-
-### Example Repo
+## Feature Views
 
-Want to look at examples of how to use `aligned`?
-View the [`MatsMoll/aligned-example` repo](https://github.com/MatsMoll/aligned-example).
+Write features as the should be, as data models.
+Then get code completion and typesafety by referencing them in other features.
 
-Or see how you could query a file in a data lake.
+This makes the features light weight, data source indipendent, and flexible.
 
 ```python
-store = await ContractStore.from_dir(".")
-df = await store.execute_sql("SELECT * FROM titanic LIMIT 10").to_polars()
-```
+class TitanicPassenger(FeatureView):
 
-## Docs
-
-Check out the [Aligned Docs](https://www.aligned.codes), but keep in mind that they are still work in progress.
-
----
-
-### Available Features
-
-Bellow are some of the features Aligned offers:
+    metadata = FeatureViewMetadata(
+        name="passenger",
+        description="Some features from the titanic dataset",
+        batch_source=FileSource.csv_at("titanic.csv"),
+        stream_source=HttpStreamSource(topic_name="titanic")
+    )
 
-- [Data Catalog](https://aligned-managed-web.vercel.app/)
-- [Data Lineage](https://aligned-managed-web.vercel.app/)
-- [Model Performance Monitoring](https://aligned-managed-web.vercel.app/)
-- [Data Freshness](#data-freshness)
-- [Data Quality Assurance](#data-quality)
-- [Feature Store](https://matsmoll.github.io/posts/understanding-the-chaotic-landscape-of-mlops#feature-store)
-- [Exposing Models](#exposed-models)
+    passenger_id = Entity(dtype=Int32())
 
+    # Input values
+    age = (
+        Float()
+            .description("A float as some have decimals")
+            .is_required()
+            .lower_bound(0)
+            .upper_bound(110)
+    )
 
-All from the simple API of defining
-- [Data Sources](#data-sources)
-- [Feature Views](#feature-views)
-- [Models](#describe-models)
+    name = String()
+    sex = String().accepted_values(["male", "female"])
+    survived = Bool().description("If the passenger survived")
+    sibsp = Int32().lower_bound(0, is_inclusive=True).description("Number of siblings on titanic")
+    cabin = String()
 
-As a result, loading model features is as easy as:
+    # Creates two one hot encoded values
+    is_male, is_female = sex.one_hot_encode(['male', 'female'])
 
-```python
-entities = {"passenger_id": [1, 2, 3, 4]}
-await store.model("titanic").features_for(entities).to_pandas()
+    # Standard scale the age.
+    # This will fit the scaler using a data slice from the batch source
+    # limited to maximum 100 rows. We can also uese a time constraint if wanted
+    scaled_age = age.standard_scaled(limit=100)
 ```
 
-Aligned is still in active development, so changes are likely.
+## Data sources
 
-## Model Contract
+Alinged makes handling data sources easy, as you do not have to think about how it is done.
+Only define where the data is, and we handle the dirty work.
 
-Aligned introduces a new concept called the "model contract", which tries to answer the following questions.
+```python
+my_db = PostgreSQLConfig(env_var="DATABASE_URL")
 
-- What is predicted?
-- What is assosiated with a prediction? - A user id?
-- Where do we store predictions?
-- Do a model depend on other models?
-- Is the model exposed through an API?
-- What needs to be sent in, to use the model?
-- Is it classification, regression, gen ai?
-- Where is the ground truth stored? - if any
-- Who owns the model?
-- Where do we store data sets?
+class TitanicPassenger(FeatureView):
 
-All this is described through a `model_contract`, as shown bellow.
+    metadata = FeatureViewMetadata(
+        name="passenger",
+        description="Some features from the titanic dataset",
+        batch_source=my_db.table(
+            "passenger",
+            mapping_keys={
+                "Passenger_Id": "passenger_id"
+            }
+        ),
+        stream_source=HttpStreamSource(topic_name="titanic")
+    )
 
-```python
-@model_contract(
-    name="eta_taxi",
-    input_features=[
-        trips.eucledian_distance,
-        trips.number_of_passengers,
-        traffic.expected_delay
-    ],
-    output_source=FileSource.delta_at("titanic_model/predictions")
-)
-class EtaTaxi:
-    trip_id = Int32().as_entity()
-    predicted_at = EventTimestamp()
-    predicted_duration = trips.duration.as_regression_target()
+    passenger_id = Entity(dtype=Int32())
 ```
 
-## Data Sources
+### Fast development
 
-Alinged makes handling data sources easy, as you do not have to think about how it is done.
-
-Furthermore, Aligned makes it easy to switch parts of the business logic to a local setup for debugging purposes.
+Making iterativ and fast exploration in ML is important. This is why Aligned also makes it super easy to combine, and test multiple sources.
 
 ```python
-from aligned import FileSource, AwsS3Config, AzureBlobConfig
-
-dir_type: Literal["local", "aws", "azure"] = ...
+my_db = PostgreSQLConfig.localhost()
 
-if dir_type == "aws":
-    aws_config = AwsS3Config(...)
-    root_directory = aws_config.directory("my-awesome-project")
+aws_bucket = AwsS3Config(...)
 
-elif dir_type == "azure":
-    azure_config = AzureBlobConfig(...)
-    root_directory = azure_config.directory("my-awesome-project")
-else:
-    root_directory = FileSource.directory("my-awesome-project")
+class SomeFeatures(FeatureView):
 
+    metadata = FeatureViewMetadata(
+        name="some_features",
+        description="...",
+        batch_source=my_db.table("local_features")
+    )
 
-taxi_project = root_directory.sub_directory("eta_taxi")
+    # Some features
+    ...
 
-csv_source = taxi_project.csv_at("predictions.csv")
-parquet_source = taxi_project.parquet_at("predictions.parquet")
-delta_source = taxi_project.delta_at("predictions")
-```
+class AwsFeatures(FeatureView):
 
-### Date Formatting
-Managing a data lake can be hard. However, a common problem when using file formats can be managing date formats. As a result do Aligned provide a way to standardise this, so you can focus on what matters.
+    metadata = FeatureViewMetadata(
+        name="aws",
+        description="...",
+        batch_source=aws_bucket.file_at("path/to/file.parquet")
+    )
 
-```python
-from aligned import FileSource
-from aligned.schemas.date_formatter import DateFormatter
+    # Some features
+    ...
+```
 
-iso_formatter = DateFormatter.iso_8601()
-unix_formatter = DateFormatter.unix_timestamp(time_unit="us", time_zone="UTC")
-custom_strtime_formatter = DateFormatter.string_format("%Y/%m/%d %H:%M:%S")
+## Model Service
 
-FileSource.csv_at("my/file.csv", date_formatter=unix_formatter)
+Usually will you need to combine multiple features for each model.
+This is where a `ModelService` comes in.
+Here can you define which features should be exposed.
+
+```python
+# Uses the variable name, as the model service name.
+# Can also define a custom name, if wanted.
+titanic_model = ModelService(
+    features=[
+        TitanicPassenger.select_all(),
+
+        # Select features with code completion
+        LocationFeatures.select(lambda view: [
+            view.distance_to_shore,
+            view.distance_to_closest_boat
+        ]),
+    ]
+)
 ```
 
-## Feature Views
-
-Aligned also makes it possible to define data and features through `feature_view`s.
-Then get code completion and typesafety by referencing them in other features.
 
-This makes the features light weight, data source independent, and flexible.
+## Data Enrichers
 
-```python
-@feature_view(
-    name="passenger",
-    description="Some features from the titanic dataset",
-    source=FileSource.csv_at("titanic.csv"),
-    materialized_source=FileSource.parquet_at("titanic.parquet"),
+In manny cases will extra data be needed in order to generate some features.
+We therefore need some way of enriching the data.
+This can easily be done with Alinged's `DataEnricher`s.
+
+```python
+my_db = PostgreSQLConfig.localhost()
+redis = RedisConfig.localhost()
+
+user_location = my_db.data_enricher( # Fetch all user locations
+    sql="SELECT * FROM user_location"
+).cache( # Cache them for one day
+    ttl=timedelta(days=1),
+    cache_key="user_location_cache"
+).lock( # Make sure only one processer fetches the data at a time
+    lock_name="user_location_lock",
+    redis_config=redis
 )
-class TitanicPassenger:
 
-    passenger_id = Int32().as_entity()
 
-    age = (
-        Float()
-            .description("A float as some have decimals")
-            .lower_bound(0)
-            .upper_bound(110)
-    )
+async def distance_to_users(df: DataFrame) -> Series:
+    user_location_df = await user_location.load()
+    ...
+    return distances
 
-    name = String()
-    sex = String().accepted_values(["male", "female"])
-    did_survive = Bool().description("If the passenger survived")
-    sibsp = Int32().lower_bound(0).description("Number of siblings on titanic")
-    cabin = String().is_optional()
+class SomeFeatures(FeatureView):
 
-    # Creates two one hot encoded values
-    is_male, is_female = sex.one_hot_encode(['male', 'female'])
+    metadata = FeatureViewMetadata(...)
+
+    latitude = Float()
+    longitude = Float()
+
+    distance_to_users = Float().transformed(distance_to_users, using_features=[latitude, longitude])
 ```
 
-### Exposed models
 
-Aligned mainly focuses on defining the expected input and output of different models. However, this in itself makes it hard to use the models. This is why Aligned makes it possible to define how our ML models are exposed by setting an `exposed_model` attribute.
+## Access Data
 
+You can easily create a feature store that contains all your feature definitions.
+This can then be used to genreate data sets, setup an instce to serve features, DAG's etc.
 
 ```python
-from aligned.exposed_model.mlflow import mlflow_server
+store = FeatureStore.from_dir(".")
 
-@model_contract(
-    name="eta_taxi",
-    exposed_model=mlflow_server(
-        host="http://localhost:8000",
-    ),
-    ...
-)
-class EtaTaxi:
-    trip_id = Int32().as_entity()
-    predicted_at = EventTimestamp()
-    predicted_duration = trips.duration.as_regression_target()
+# Select all features from a single feature view
+df = await store.all_for("passenger", limit=100).to_df()
 ```
 
-This also makes it possible to get predictions with the following command:
+### Centraliced Feature Store Definition
+You would often share the features with other coworkers, or split them into different stages, like `staging`, `shadow`, or `production`.
+One option is therefore to reference the storage you use, and load the `FeatureStore` from there.
 
 ```python
-await store.model("eta_taxi").predict_over({
-    "trip_id": [...]
-}).to_polars()
-```
-
-Or store them directly in the `output_source` with something like:
+aws_bucket = AwsS3Config(...)
+store = await aws_bucket.file_at("production.json").feature_store()
 
-```python
-await store.model("eta_taxi").predict_over({
-    "trip_id": [...]
-}).upsert_into_output_source()
+# This switches from the production online store to the offline store
+# Aka. the batch sources defined on the feature views
+experimental_store = store.offline_store()
 ```
+This json file can be generated by running `alinged apply`.
 
-Some of the existing implementations are:
-- MLFlow Server
-- Run MLFLow model in memory
-- Ollama completion endpoint
-- Ollama embedded endpoint
-- Send entities to generic endpoint
-
-## Data Freshness
-Making sure a source contains fresh data is a crucial part to create propper ML applications.
-Therefore, Aligned provides an easy way to check how fresh a source is.
+### Select multiple feature views
 
 ```python
-@feature_view(
-    name="departures",
-    description="Features related to the departure of a taxi ride",
-    source=taxi_db.table("departures"),
-)
-class TaxiDepartures:
+df = await store.features_for({
+    "passenger_id": [1, 50, 110]
+}, features=[
+    "passenger:scaled_age",
+    "passenger:is_male",
+    "passenger:sibsp"
 
-    trip_id = UUID().as_entity()
+    "other_features:distance_to_closest_boat",
+]).to_df()
+```
 
-    pickuped_at = EventTimestamp()
+### Model Service
 
-    number_of_passengers = Int32().is_optional()
+Selecting features for a model is super simple.
 
-    dropoff_latitude = Float()
-    dropoff_longitude = Float()
 
-    pickup_latitude = Float()
-    pickup_longitude = Float()
+```python
+df = await store.model("titanic_model").features_for({
+    "passenger_id": [1, 50, 110]
+}).to_df()
+```
 
+### Feature View
 
-freshness = await TaxiDepartures.freshness_in_batch_source()
+If you want to only select features for a specific feature view, then this is also possible.
 
-if freshness < datetime.now() - timedelta(days=2):
-    raise ValueError("To old data to create an ML model")
+```python
+prev_30_days = await store.feature_view("match").previous(days=30).to_df()
+sample_of_20 = await store.feature_view("match").all(limit=20).to_df()
 ```
 
 ## Data quality
 Alinged will make sure all the different features gets formatted as the correct datatype.
 In addition will aligned also make sure that the returend features aligne with defined constraints.
 
 ```python
-@feature_view(...)
-class TitanicPassenger:
+class TitanicPassenger(FeatureView):
+
     ...
+
     age = (
         Float()
+            .is_required()
             .lower_bound(0)
             .upper_bound(110)
     )
-    sibsp = Int32().lower_bound(0).is_optional()
+    sibsp = Int32().lower_bound(0, is_inclusive=True)
 ```
 
-Then since our feature view have a `is_optional` and a `lower_bound`, will the `.validate(...)` command filter out the entites that do not follow that behavior.
+Then since our feature view have a `is_required` and a `lower_bound`, will the `.validate(...)` command filter out the entites that do not follow that behavior.
 
 ```python
 from aligned.validation.pandera import PanderaValidator
 
 df = await store.model("titanic_model").features_for({
     "passenger_id": [1, 50, 110]
 }).validate(
     PanderaValidator()  # Validates all features
-).to_pandas()
+).to_df()
 ```
 
-## Contract Store
-
-Aligned collects all the feature views and model contracts in a contract store. You can generate this in a few different ways, and each method serves some different use-cases.
-
-For experimentational use-cases will the `await ContractStore.from_dir(".")` probably make the most sense. However, this will scan the full directory which can lead to slow startup times.
+## Feature Server
 
-Therefore, it is also possible to manually add the different feature views and contracts with the following.
+This expectes that you either run the command in your feature store repo, or have a file with a `RepoReference` instance.
+You can also setup an online source like Redis, for faster storage.
 
 ```python
-store = ContractStore.empty()
-store.add_feature_view(MyView)
-store.add_model(MyModel)
-```
-
-This makes it possible to define different contracts per project, or team. As a result, you can also combine differnet stores with.
+redis = RedisConfig.localhost()
 
-```python
-combined_store = recommendation_store.combined_with(forecasting_store)
-```
+aws_bucket = AwsS3Config(...)
 
-Lastly, we can also load the all features from a serializable format, such as a JSON file.
+repo_files = RepoReference(
+    env_var_name="ENVIRONMENT",
+    repo_paths={
+        "production": aws_bucket.file_at("feature-store/production.json"),
+        "shadow": aws_bucket.file_at("feature-store/shadow.json"),
+        "staging": aws_bucket.file_at("feature-store/staging.json")
+        # else generate the feature store from the current dir
+    }
+)
 
-```python
-await FileSource.json_at("contracts.json").as_contract_store()
+# Use redis as the online source, if not running localy
+if repo_files.selected != "local":
+    online_source = redis.online_source()
 ```
 
+Then run `aligned serve`, and a FastAPI server will start. Here can you push new features, which then transforms and stores the features, or just fetch them.
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```
