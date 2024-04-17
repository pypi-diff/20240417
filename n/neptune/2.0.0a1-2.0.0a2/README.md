# Comparing `tmp/neptune-2.0.0a1.tar.gz` & `tmp/neptune-2.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neptune-2.0.0a1.tar", max compression
+gzip compressed data, was "neptune-2.0.0a2.tar", max compression
```

## Comparing `neptune-2.0.0a1.tar` & `neptune-2.0.0a2.tar`

### file list

```diff
@@ -1,280 +1,283 @@
--rw-r--r--   0        0        0    44436 2024-04-11 15:36:18.970295 neptune-2.0.0a1/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2024-04-11 15:36:18.970295 neptune-2.0.0a1/LICENSE
--rw-r--r--   0        0        0    12786 2024-04-11 15:36:18.970295 neptune-2.0.0a1/README.md
--rw-r--r--   0        0        0    10951 2024-04-11 15:36:28.874262 neptune-2.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     3596 2024-04-11 15:36:18.970295 neptune-2.0.0a1/src/neptune/__init__.py
--rw-r--r--   0        0        0      596 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/api/__init__.py
--rw-r--r--   0        0        0     2768 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/api/field_visitor.py
--rw-r--r--   0        0        0    19028 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/api/models.py
--rw-r--r--   0        0        0      596 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/api/proto/__init__.py
--rw-r--r--   0        0        0      596 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/api/proto/neptune_pb/__init__.py
--rw-r--r--   0        0        0      596 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/api/proto/neptune_pb/api/__init__.py
--rw-r--r--   0        0        0      596 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/api/proto/neptune_pb/api/model/__init__.py
--rw-r--r--   0        0        0     1590 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/api/proto/neptune_pb/api/model/attributes_pb2.py
--rw-r--r--   0        0        0     1642 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/api/proto/neptune_pb/api/model/attributes_pb2.pyi
--rw-r--r--   0        0        0     6126 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/api/proto/neptune_pb/api/model/leaderboard_entries_pb2.py
--rw-r--r--   0        0        0    17492 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/api/proto/neptune_pb/api/model/leaderboard_entries_pb2.pyi
--rw-r--r--   0        0        0      990 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/api/requests_utils.py
--rw-r--r--   0        0        0     7771 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/api/searching_entries.py
--rw-r--r--   0        0        0     1218 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/__init__.py
--rw-r--r--   0        0        0     1011 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/atoms/__init__.py
--rw-r--r--   0        0        0     3146 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/atoms/artifact.py
--rw-r--r--   0        0        0      701 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/atoms/atom.py
--rw-r--r--   0        0        0     1709 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/atoms/boolean.py
--rw-r--r--   0        0        0     2105 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/atoms/copiable_atom.py
--rw-r--r--   0        0        0     2075 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/atoms/datetime.py
--rw-r--r--   0        0        0     1923 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/atoms/file.py
--rw-r--r--   0        0        0     2446 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/atoms/float.py
--rw-r--r--   0        0        0      696 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/atoms/git_ref.py
--rw-r--r--   0        0        0     2397 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/atoms/integer.py
--rw-r--r--   0        0        0      707 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/atoms/notebook_ref.py
--rw-r--r--   0        0        0      700 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/atoms/run_state.py
--rw-r--r--   0        0        0     2665 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/atoms/string.py
--rw-r--r--   0        0        0     2139 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/attribute.py
--rw-r--r--   0        0        0     2723 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/constants.py
--rw-r--r--   0        0        0     3023 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/file_set.py
--rw-r--r--   0        0        0     4585 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/namespace.py
--rw-r--r--   0        0        0      782 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/series/__init__.py
--rw-r--r--   0        0        0     2594 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/series/fetchable_series.py
--rw-r--r--   0        0        0     4432 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/series/file_series.py
--rw-r--r--   0        0        0     2656 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/series/float_series.py
--rw-r--r--   0        0        0     6193 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/series/series.py
--rw-r--r--   0        0        0     3505 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/series/string_series.py
--rw-r--r--   0        0        0      662 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/sets/__init__.py
--rw-r--r--   0        0        0      699 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/sets/set.py
--rw-r--r--   0        0        0     2627 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/sets/string_set.py
--rw-r--r--   0        0        0     2057 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/attributes/utils.py
--rw-r--r--   0        0        0      686 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/cli/__init__.py
--rw-r--r--   0        0        0     1348 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/cli/__main__.py
--rw-r--r--   0        0        0     3184 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/cli/clear.py
--rw-r--r--   0        0        0     5391 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/cli/collect.py
--rw-r--r--   0        0        0     5220 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/cli/commands.py
--rw-r--r--   0        0        0    10813 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/cli/containers.py
--rw-r--r--   0        0        0     1511 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/cli/path_option.py
--rw-r--r--   0        0        0     3854 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/cli/status.py
--rw-r--r--   0        0        0     5537 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/cli/sync.py
--rw-r--r--   0        0        0     5167 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/cli/utils.py
--rw-r--r--   0        0        0     1087 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/constants.py
--rw-r--r--   0        0        0      596 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/core/__init__.py
--rw-r--r--   0        0        0      596 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/core/components/__init__.py
--rw-r--r--   0        0        0     1821 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/core/components/abstract.py
--rw-r--r--   0        0        0     2172 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/core/components/metadata_file.py
--rw-r--r--   0        0        0     1237 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/core/components/operation_storage.py
--rw-r--r--   0        0        0      596 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/core/components/queue/__init__.py
--rw-r--r--   0        0        0     8848 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/core/components/queue/disk_queue.py
--rw-r--r--   0        0        0     3610 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/core/components/queue/json_file_splitter.py
--rw-r--r--   0        0        0     2229 2024-04-11 15:36:18.974295 neptune-2.0.0a1/src/neptune/core/components/queue/log_file.py
--rw-r--r--   0        0        0     1766 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/core/components/queue/sync_offset_file.py
--rw-r--r--   0        0        0     2573 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/envs.py
--rw-r--r--   0        0        0    42022 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/exceptions.py
--rw-r--r--   0        0        0    32876 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/handler.py
--rw-r--r--   0        0        0      596 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/__init__.py
--rw-r--r--   0        0        0      775 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/aws/__init__.py
--rw-r--r--   0        0        0      796 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/detectron2/__init__.py
--rw-r--r--   0        0        0      784 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/fastai/__init__.py
--rw-r--r--   0        0        0      781 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/kedro/__init__.py
--rw-r--r--   0        0        0      790 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/lightgbm/__init__.py
--rw-r--r--   0        0        0      795 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/mosaicml/__init__.py
--rw-r--r--   0        0        0      784 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/optuna/__init__.py
--rw-r--r--   0        0        0     3633 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/pandas/__init__.py
--rw-r--r--   0        0        0      787 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/prophet/__init__.py
--rw-r--r--   0        0        0     3026 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/python_logger.py
--rw-r--r--   0        0        0      787 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/pytorch/__init__.py
--rw-r--r--   0        0        0      814 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/pytorch_lightning/__init__.py
--rw-r--r--   0        0        0      784 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/sacred/__init__.py
--rw-r--r--   0        0        0      787 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/sklearn/__init__.py
--rw-r--r--   0        0        0      799 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/tensorboard/__init__.py
--rw-r--r--   0        0        0      814 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/tensorflow_keras/__init__.py
--rw-r--r--   0        0        0      812 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/transformers/__init__.py
--rw-r--r--   0        0        0      864 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/utils.py
--rw-r--r--   0        0        0      787 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/integrations/xgboost/__init__.py
--rw-r--r--   0        0        0      596 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/__init__.py
--rw-r--r--   0        0        0      760 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/artifacts/__init__.py
--rw-r--r--   0        0        0      791 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/artifacts/drivers/__init__.py
--rw-r--r--   0        0        0     4240 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/artifacts/drivers/local.py
--rw-r--r--   0        0        0     4810 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/artifacts/drivers/s3.py
--rw-r--r--   0        0        0     5141 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/artifacts/file_hasher.py
--rw-r--r--   0        0        0     2377 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/artifacts/local_file_hash_storage.py
--rw-r--r--   0        0        0     3578 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/artifacts/types.py
--rw-r--r--   0        0        0      999 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/artifacts/utils.py
--rw-r--r--   0        0        0      596 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/__init__.py
--rw-r--r--   0        0        0     6311 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/api_model.py
--rw-r--r--   0        0        0     1703 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/factory.py
--rw-r--r--   0        0        0     9567 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/hosted_artifact_operations.py
--rw-r--r--   0        0        0     6714 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/hosted_client.py
--rw-r--r--   0        0        0    18056 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/hosted_file_operations.py
--rw-r--r--   0        0        0    46218 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/hosted_neptune_backend.py
--rw-r--r--   0        0        0     9535 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/neptune_backend.py
--rw-r--r--   0        0        0    32992 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/neptune_backend_mock.py
--rw-r--r--   0        0        0     2894 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/nql.py
--rw-r--r--   0        0        0     5864 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/offline_neptune_backend.py
--rw-r--r--   0        0        0     3948 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/operation_api_name_visitor.py
--rw-r--r--   0        0        0     5005 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/operation_api_object_converter.py
--rw-r--r--   0        0        0    13843 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/operations_preprocessor.py
--rw-r--r--   0        0        0     1642 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/project_name_lookup.py
--rw-r--r--   0        0        0     5658 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/swagger_client_wrapper.py
--rw-r--r--   0        0        0    15994 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backends/utils.py
--rw-r--r--   0        0        0     1517 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/backgroud_job_list.py
--rw-r--r--   0        0        0     1134 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/background_job.py
--rw-r--r--   0        0        0      947 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/constants.py
--rw-r--r--   0        0        0     4486 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/container_structure.py
--rw-r--r--   0        0        0     1302 2024-04-11 15:36:18.978295 neptune-2.0.0a1/src/neptune/internal/container_type.py
--rw-r--r--   0        0        0     2349 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/credentials.py
--rw-r--r--   0        0        0      859 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/envs.py
--rw-r--r--   0        0        0    15028 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/exceptions.py
--rw-r--r--   0        0        0     1725 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/extensions.py
--rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/__init__.py
--rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/cgroup/__init__.py
--rw-r--r--   0        0        0     2638 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/cgroup/cgroup_filesystem_reader.py
--rw-r--r--   0        0        0     3216 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/cgroup/cgroup_monitor.py
--rw-r--r--   0        0        0      694 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/constants.py
--rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/gauges/__init__.py
--rw-r--r--   0        0        0     1560 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/gauges/cpu.py
--rw-r--r--   0        0        0      979 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/gauges/gauge.py
--rw-r--r--   0        0        0     2031 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/gauges/gauge_factory.py
--rw-r--r--   0        0        0      667 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/gauges/gauge_mode.py
--rw-r--r--   0        0        0     1772 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/gauges/gpu.py
--rw-r--r--   0        0        0     1756 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/gauges/memory.py
--rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/gpu/__init__.py
--rw-r--r--   0        0        0     2488 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/gpu/gpu_monitor.py
--rw-r--r--   0        0        0     5122 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/hardware_metric_reporting_job.py
--rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/metrics/__init__.py
--rw-r--r--   0        0        0     2432 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/metrics/metric.py
--rw-r--r--   0        0        0     1216 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/metrics/metrics_container.py
--rw-r--r--   0        0        0     3496 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/metrics/metrics_factory.py
--rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/metrics/reports/__init__.py
--rw-r--r--   0        0        0      792 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/metrics/reports/metric_report.py
--rw-r--r--   0        0        0     1681 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/metrics/reports/metric_reporter.py
--rw-r--r--   0        0        0      949 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/metrics/reports/metric_reporter_factory.py
--rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/metrics/service/__init__.py
--rw-r--r--   0        0        0     1106 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/metrics/service/metric_service.py
--rw-r--r--   0        0        0     2323 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/metrics/service/metric_service_factory.py
--rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/resources/__init__.py
--rw-r--r--   0        0        0     1821 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/resources/gpu_card_indices_provider.py
--rw-r--r--   0        0        0     1574 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/resources/system_resource_info.py
--rw-r--r--   0        0        0     2512 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/resources/system_resource_info_factory.py
--rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/system/__init__.py
--rw-r--r--   0        0        0      964 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/hardware/system/system_monitor.py
--rw-r--r--   0        0        0      933 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/id_formats.py
--rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/init/__init__.py
--rw-r--r--   0        0        0     1137 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/init/parameters.py
--rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/notebooks/__init__.py
--rw-r--r--   0        0        0     1595 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/notebooks/comm.py
--rw-r--r--   0        0        0     1854 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/notebooks/notebooks.py
--rw-r--r--   0        0        0     4784 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/oauth.py
--rw-r--r--   0        0        0    17298 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/operation.py
--rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/operation_processors/__init__.py
--rw-r--r--   0        0        0    13129 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/operation_processors/async_operation_processor.py
--rw-r--r--   0        0        0     3073 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/operation_processors/factory.py
--rw-r--r--   0        0        0     3936 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/operation_processors/lazy_operation_processor_wrapper.py
--rw-r--r--   0        0        0     3070 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/operation_processors/offline_operation_processor.py
--rw-r--r--   0        0        0     6886 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/operation_processors/operation_logger.py
--rw-r--r--   0        0        0     1422 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/operation_processors/operation_processor.py
--rw-r--r--   0        0        0     1146 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/operation_processors/read_only_operation_processor.py
--rw-r--r--   0        0        0     3361 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/operation_processors/sync_operation_processor.py
--rw-r--r--   0        0        0     2443 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/operation_processors/utils.py
--rw-r--r--   0        0        0     3724 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/operation_visitor.py
--rw-r--r--   0        0        0      886 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/patches/__init__.py
--rw-r--r--   0        0        0     2731 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/patches/bravado.py
--rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/signals_processing/__init__.py
--rw-r--r--   0        0        0     2883 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/signals_processing/background_job.py
--rw-r--r--   0        0        0     1663 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/signals_processing/signals.py
--rw-r--r--   0        0        0     4899 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/signals_processing/signals_processor.py
--rw-r--r--   0        0        0     1789 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/signals_processing/utils.py
--rw-r--r--   0        0        0      776 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/state.py
--rw-r--r--   0        0        0     1130 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/storage/__init__.py
--rw-r--r--   0        0        0     3227 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/storage/datastream.py
--rw-r--r--   0        0        0     7330 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/storage/storage_utils.py
--rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/streams/__init__.py
--rw-r--r--   0        0        0     1999 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/streams/std_capture_background_job.py
--rw-r--r--   0        0        0     3066 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/streams/std_stream_capture_logger.py
--rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/threading/__init__.py
--rw-r--r--   0        0        0     5581 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/threading/daemon.py
--rw-r--r--   0        0        0      596 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/types/__init__.py
--rw-r--r--   0        0        0     4586 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/types/file_types.py
--rw-r--r--   0        0        0     2484 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/types/stringify_value.py
--rw-r--r--   0        0        0      799 2024-04-11 15:36:18.982295 neptune-2.0.0a1/src/neptune/internal/types/utils.py
--rw-r--r--   0        0        0     5311 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/__init__.py
--rw-r--r--   0        0        0     2409 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/dependency_tracking.py
--rw-r--r--   0        0        0     2116 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/deprecation.py
--rw-r--r--   0        0        0     5746 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/disk_utilization.py
--rw-r--r--   0        0        0     2300 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/generic_attribute_mapper.py
--rw-r--r--   0        0        0     6158 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/git.py
--rw-r--r--   0        0        0     2490 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/git_info.py
--rw-r--r--   0        0        0      849 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/hashing.py
--rw-r--r--   0        0        0    10577 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/images.py
--rw-r--r--   0        0        0     1152 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/iso_dates.py
--rw-r--r--   0        0        0     1288 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/iteration.py
--rw-r--r--   0        0        0     1657 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/limits.py
--rw-r--r--   0        0        0     2972 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/logger.py
--rw-r--r--   0        0        0     1065 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/paths.py
--rw-r--r--   0        0        0      726 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/patterns.py
--rw-r--r--   0        0        0     2187 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/ping_background_job.py
--rw-r--r--   0        0        0     1809 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/process_killer.py
--rw-r--r--   0        0        0     1168 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/requirement_check.py
--rw-r--r--   0        0        0     1566 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/run_state.py
--rw-r--r--   0        0        0     1143 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/runningmode.py
--rw-r--r--   0        0        0     1340 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/s3.py
--rw-r--r--   0        0        0     2266 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/source_code.py
--rw-r--r--   0        0        0     2001 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/traceback_job.py
--rw-r--r--   0        0        0     2450 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/uncaught_exception_handler.py
--rw-r--r--   0        0        0     7575 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/utils/utils.py
--rw-r--r--   0        0        0     4442 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/value_to_attribute_visitor.py
--rw-r--r--   0        0        0     3284 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/warnings.py
--rw-r--r--   0        0        0      596 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/websockets/__init__.py
--rw-r--r--   0        0        0     3591 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/websockets/reconnecting_websocket.py
--rw-r--r--   0        0        0     2638 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/websockets/websocket_client_adapter.py
--rw-r--r--   0        0        0     5210 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/websockets/websocket_signals_background_job.py
--rw-r--r--   0        0        0     1231 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/internal/websockets/websockets_factory.py
--rw-r--r--   0        0        0     4795 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/management/__init__.py
--rw-r--r--   0        0        0     6943 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/management/exceptions.py
--rw-r--r--   0        0        0      596 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/management/internal/__init__.py
--rw-r--r--   0        0        0    44742 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/management/internal/api.py
--rw-r--r--   0        0        0     2853 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/management/internal/dto.py
--rw-r--r--   0        0        0     1069 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/management/internal/types.py
--rw-r--r--   0        0        0     2021 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/management/internal/utils.py
--rw-r--r--   0        0        0      923 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/objects/__init__.py
--rw-r--r--   0        0        0     2031 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/objects/abstract.py
--rw-r--r--   0        0        0    15915 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/objects/model.py
--rw-r--r--   0        0        0    13820 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/objects/model_version.py
--rw-r--r--   0        0        0    26780 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/objects/neptune_object.py
--rw-r--r--   0        0        0    19245 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/objects/project.py
--rw-r--r--   0        0        0    26549 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/objects/run.py
--rw-r--r--   0        0        0     1576 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/objects/structure_version.py
--rw-r--r--   0        0        0     4043 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/objects/utils.py
--rw-r--r--   0        0        0     5783 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/table.py
--rw-r--r--   0        0        0     1071 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/types/__init__.py
--rw-r--r--   0        0        0      914 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/types/atoms/__init__.py
--rw-r--r--   0        0        0     1626 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/types/atoms/artifact.py
--rw-r--r--   0        0        0      936 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/types/atoms/atom.py
--rw-r--r--   0        0        0     1302 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/types/atoms/boolean.py
--rw-r--r--   0        0        0     1435 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/types/atoms/datetime.py
--rw-r--r--   0        0        0    12157 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/types/atoms/file.py
--rw-r--r--   0        0        0     1297 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/types/atoms/float.py
--rw-r--r--   0        0        0     1902 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/types/atoms/git_ref.py
--rw-r--r--   0        0        0     1299 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/types/atoms/integer.py
--rw-r--r--   0        0        0     1473 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/types/atoms/string.py
--rw-r--r--   0        0        0     1485 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/types/file_set.py
--rw-r--r--   0        0        0      831 2024-04-11 15:36:18.986295 neptune-2.0.0a1/src/neptune/types/mode.py
--rw-r--r--   0        0        0      777 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/types/model_version_stage.py
--rw-r--r--   0        0        0     1753 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/types/namespace.py
--rw-r--r--   0        0        0      783 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/types/series/__init__.py
--rw-r--r--   0        0        0     2473 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/types/series/file_series.py
--rw-r--r--   0        0        0     3854 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/types/series/float_series.py
--rw-r--r--   0        0        0     1221 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/types/series/series.py
--rw-r--r--   0        0        0     1353 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/types/series/series_value.py
--rw-r--r--   0        0        0     2601 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/types/series/string_series.py
--rw-r--r--   0        0        0      655 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/types/sets/__init__.py
--rw-r--r--   0        0        0      934 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/types/sets/set.py
--rw-r--r--   0        0        0     1119 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/types/sets/string_set.py
--rw-r--r--   0        0        0     3551 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/types/type_casting.py
--rw-r--r--   0        0        0      892 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/types/value.py
--rw-r--r--   0        0        0     1634 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/types/value_copy.py
--rw-r--r--   0        0        0     2596 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/types/value_visitor.py
--rw-r--r--   0        0        0     3089 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/typing.py
--rw-r--r--   0        0        0     4310 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/utils.py
--rw-r--r--   0        0        0        0 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/vendor/__init__.py
--rw-r--r--   0        0        0     6306 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/vendor/lib_programname.py
--rw-r--r--   0        0        0    68552 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/vendor/pynvml.py
--rw-r--r--   0        0        0     1431 2024-04-11 15:36:18.990295 neptune-2.0.0a1/src/neptune/version.py
--rw-r--r--   0        0        0    16631 1970-01-01 00:00:00.000000 neptune-2.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0    45352 2024-04-17 12:47:35.378597 neptune-2.0.0a2/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2024-04-17 12:47:35.378597 neptune-2.0.0a2/LICENSE
+-rw-r--r--   0        0        0    12786 2024-04-17 12:47:35.378597 neptune-2.0.0a2/README.md
+-rw-r--r--   0        0        0    10932 2024-04-17 12:47:47.738600 neptune-2.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0     3596 2024-04-17 12:47:35.378597 neptune-2.0.0a2/src/neptune/__init__.py
+-rw-r--r--   0        0        0      596 2024-04-17 12:47:35.378597 neptune-2.0.0a2/src/neptune/api/__init__.py
+-rw-r--r--   0        0        0     1936 2024-04-17 12:47:35.378597 neptune-2.0.0a2/src/neptune/api/fetching_series_values.py
+-rw-r--r--   0        0        0     2768 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/api/field_visitor.py
+-rw-r--r--   0        0        0    22709 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/api/models.py
+-rw-r--r--   0        0        0      596 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/api/proto/__init__.py
+-rw-r--r--   0        0        0      596 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/__init__.py
+-rw-r--r--   0        0        0      596 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/api/__init__.py
+-rw-r--r--   0        0        0      596 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/api/model/__init__.py
+-rw-r--r--   0        0        0     1590 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/api/model/attributes_pb2.py
+-rw-r--r--   0        0        0     1642 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/api/model/attributes_pb2.pyi
+-rw-r--r--   0        0        0     6126 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/api/model/leaderboard_entries_pb2.py
+-rw-r--r--   0        0        0    17492 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/api/model/leaderboard_entries_pb2.pyi
+-rw-r--r--   0        0        0     1669 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/api/model/series_values_pb2.py
+-rw-r--r--   0        0        0     1955 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/api/model/series_values_pb2.pyi
+-rw-r--r--   0        0        0      990 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/api/requests_utils.py
+-rw-r--r--   0        0        0     7771 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/api/searching_entries.py
+-rw-r--r--   0        0        0     1218 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/__init__.py
+-rw-r--r--   0        0        0     1011 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/atoms/__init__.py
+-rw-r--r--   0        0        0     3146 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/atoms/artifact.py
+-rw-r--r--   0        0        0      701 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/atoms/atom.py
+-rw-r--r--   0        0        0     1709 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/atoms/boolean.py
+-rw-r--r--   0        0        0     2105 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/atoms/copiable_atom.py
+-rw-r--r--   0        0        0     2075 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/atoms/datetime.py
+-rw-r--r--   0        0        0     2215 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/atoms/file.py
+-rw-r--r--   0        0        0     2446 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/atoms/float.py
+-rw-r--r--   0        0        0      696 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/atoms/git_ref.py
+-rw-r--r--   0        0        0     2397 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/atoms/integer.py
+-rw-r--r--   0        0        0      707 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/atoms/notebook_ref.py
+-rw-r--r--   0        0        0      700 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/atoms/run_state.py
+-rw-r--r--   0        0        0     2665 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/atoms/string.py
+-rw-r--r--   0        0        0     2139 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/attribute.py
+-rw-r--r--   0        0        0     2723 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/constants.py
+-rw-r--r--   0        0        0     3425 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/file_set.py
+-rw-r--r--   0        0        0     4585 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/namespace.py
+-rw-r--r--   0        0        0      782 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/series/__init__.py
+-rw-r--r--   0        0        0     2094 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/series/fetchable_series.py
+-rw-r--r--   0        0        0     4515 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/series/file_series.py
+-rw-r--r--   0        0        0     2899 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/series/float_series.py
+-rw-r--r--   0        0        0     6193 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/series/series.py
+-rw-r--r--   0        0        0     3762 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/series/string_series.py
+-rw-r--r--   0        0        0      662 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/sets/__init__.py
+-rw-r--r--   0        0        0      699 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/sets/set.py
+-rw-r--r--   0        0        0     2809 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/sets/string_set.py
+-rw-r--r--   0        0        0     2057 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/attributes/utils.py
+-rw-r--r--   0        0        0      686 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/cli/__init__.py
+-rw-r--r--   0        0        0     1348 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/cli/__main__.py
+-rw-r--r--   0        0        0     3184 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/cli/clear.py
+-rw-r--r--   0        0        0     5391 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/cli/collect.py
+-rw-r--r--   0        0        0     5220 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/cli/commands.py
+-rw-r--r--   0        0        0    10813 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/cli/containers.py
+-rw-r--r--   0        0        0     1511 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/cli/path_option.py
+-rw-r--r--   0        0        0     3854 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/cli/status.py
+-rw-r--r--   0        0        0     5537 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/cli/sync.py
+-rw-r--r--   0        0        0     5167 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/cli/utils.py
+-rw-r--r--   0        0        0     1087 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/constants.py
+-rw-r--r--   0        0        0      596 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/core/__init__.py
+-rw-r--r--   0        0        0      596 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/core/components/__init__.py
+-rw-r--r--   0        0        0     1821 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/core/components/abstract.py
+-rw-r--r--   0        0        0     2172 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/core/components/metadata_file.py
+-rw-r--r--   0        0        0     1237 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/core/components/operation_storage.py
+-rw-r--r--   0        0        0      596 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/core/components/queue/__init__.py
+-rw-r--r--   0        0        0     8848 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/core/components/queue/disk_queue.py
+-rw-r--r--   0        0        0     3610 2024-04-17 12:47:35.382597 neptune-2.0.0a2/src/neptune/core/components/queue/json_file_splitter.py
+-rw-r--r--   0        0        0     2229 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/core/components/queue/log_file.py
+-rw-r--r--   0        0        0     1766 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/core/components/queue/sync_offset_file.py
+-rw-r--r--   0        0        0     2596 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/envs.py
+-rw-r--r--   0        0        0    42022 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/exceptions.py
+-rw-r--r--   0        0        0    33497 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/handler.py
+-rw-r--r--   0        0        0      596 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/__init__.py
+-rw-r--r--   0        0        0      775 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/aws/__init__.py
+-rw-r--r--   0        0        0      796 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/detectron2/__init__.py
+-rw-r--r--   0        0        0      784 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/fastai/__init__.py
+-rw-r--r--   0        0        0      781 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/kedro/__init__.py
+-rw-r--r--   0        0        0      790 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/lightgbm/__init__.py
+-rw-r--r--   0        0        0      795 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/mosaicml/__init__.py
+-rw-r--r--   0        0        0      784 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/optuna/__init__.py
+-rw-r--r--   0        0        0     3633 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/pandas/__init__.py
+-rw-r--r--   0        0        0      787 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/prophet/__init__.py
+-rw-r--r--   0        0        0     3026 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/python_logger.py
+-rw-r--r--   0        0        0      787 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/pytorch/__init__.py
+-rw-r--r--   0        0        0      814 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/pytorch_lightning/__init__.py
+-rw-r--r--   0        0        0      784 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/sacred/__init__.py
+-rw-r--r--   0        0        0      787 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/sklearn/__init__.py
+-rw-r--r--   0        0        0      799 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/tensorboard/__init__.py
+-rw-r--r--   0        0        0      814 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/tensorflow_keras/__init__.py
+-rw-r--r--   0        0        0      812 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/transformers/__init__.py
+-rw-r--r--   0        0        0      864 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/utils.py
+-rw-r--r--   0        0        0      787 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/integrations/xgboost/__init__.py
+-rw-r--r--   0        0        0      596 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/__init__.py
+-rw-r--r--   0        0        0      760 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/artifacts/__init__.py
+-rw-r--r--   0        0        0      791 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/artifacts/drivers/__init__.py
+-rw-r--r--   0        0        0     4240 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/artifacts/drivers/local.py
+-rw-r--r--   0        0        0     4879 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/artifacts/drivers/s3.py
+-rw-r--r--   0        0        0     5141 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/artifacts/file_hasher.py
+-rw-r--r--   0        0        0     2377 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/artifacts/local_file_hash_storage.py
+-rw-r--r--   0        0        0     3578 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/artifacts/types.py
+-rw-r--r--   0        0        0      999 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/artifacts/utils.py
+-rw-r--r--   0        0        0      596 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/__init__.py
+-rw-r--r--   0        0        0     5735 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/api_model.py
+-rw-r--r--   0        0        0     1703 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/factory.py
+-rw-r--r--   0        0        0     9567 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/hosted_artifact_operations.py
+-rw-r--r--   0        0        0     6714 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/hosted_client.py
+-rw-r--r--   0        0        0    18056 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/hosted_file_operations.py
+-rw-r--r--   0        0        0    46935 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/hosted_neptune_backend.py
+-rw-r--r--   0        0        0     9603 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/neptune_backend.py
+-rw-r--r--   0        0        0    33084 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/neptune_backend_mock.py
+-rw-r--r--   0        0        0     2894 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/nql.py
+-rw-r--r--   0        0        0     5898 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/offline_neptune_backend.py
+-rw-r--r--   0        0        0     3948 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/operation_api_name_visitor.py
+-rw-r--r--   0        0        0     5005 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/operation_api_object_converter.py
+-rw-r--r--   0        0        0    13843 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/operations_preprocessor.py
+-rw-r--r--   0        0        0     1642 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/project_name_lookup.py
+-rw-r--r--   0        0        0     5658 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/swagger_client_wrapper.py
+-rw-r--r--   0        0        0    15994 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backends/utils.py
+-rw-r--r--   0        0        0     1517 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/backgroud_job_list.py
+-rw-r--r--   0        0        0     1134 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/background_job.py
+-rw-r--r--   0        0        0      947 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/constants.py
+-rw-r--r--   0        0        0     4486 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/container_structure.py
+-rw-r--r--   0        0        0     1302 2024-04-17 12:47:35.386597 neptune-2.0.0a2/src/neptune/internal/container_type.py
+-rw-r--r--   0        0        0     2349 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/credentials.py
+-rw-r--r--   0        0        0      859 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/envs.py
+-rw-r--r--   0        0        0    15028 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/exceptions.py
+-rw-r--r--   0        0        0     1725 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/extensions.py
+-rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/__init__.py
+-rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/cgroup/__init__.py
+-rw-r--r--   0        0        0     2638 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/cgroup/cgroup_filesystem_reader.py
+-rw-r--r--   0        0        0     3216 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/cgroup/cgroup_monitor.py
+-rw-r--r--   0        0        0      694 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/constants.py
+-rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/gauges/__init__.py
+-rw-r--r--   0        0        0     1560 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/gauges/cpu.py
+-rw-r--r--   0        0        0      979 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/gauges/gauge.py
+-rw-r--r--   0        0        0     2031 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/gauges/gauge_factory.py
+-rw-r--r--   0        0        0      667 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/gauges/gauge_mode.py
+-rw-r--r--   0        0        0     1772 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/gauges/gpu.py
+-rw-r--r--   0        0        0     1756 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/gauges/memory.py
+-rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/gpu/__init__.py
+-rw-r--r--   0        0        0     2488 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/gpu/gpu_monitor.py
+-rw-r--r--   0        0        0     5122 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/hardware_metric_reporting_job.py
+-rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/metrics/__init__.py
+-rw-r--r--   0        0        0     2432 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/metrics/metric.py
+-rw-r--r--   0        0        0     1216 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/metrics/metrics_container.py
+-rw-r--r--   0        0        0     3496 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/metrics/metrics_factory.py
+-rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/metrics/reports/__init__.py
+-rw-r--r--   0        0        0      792 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/metrics/reports/metric_report.py
+-rw-r--r--   0        0        0     1681 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/metrics/reports/metric_reporter.py
+-rw-r--r--   0        0        0      949 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/metrics/reports/metric_reporter_factory.py
+-rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/metrics/service/__init__.py
+-rw-r--r--   0        0        0     1106 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/metrics/service/metric_service.py
+-rw-r--r--   0        0        0     2323 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/metrics/service/metric_service_factory.py
+-rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/resources/__init__.py
+-rw-r--r--   0        0        0     1821 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/resources/gpu_card_indices_provider.py
+-rw-r--r--   0        0        0     1574 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/resources/system_resource_info.py
+-rw-r--r--   0        0        0     2512 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/resources/system_resource_info_factory.py
+-rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/system/__init__.py
+-rw-r--r--   0        0        0      964 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/hardware/system/system_monitor.py
+-rw-r--r--   0        0        0      933 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/id_formats.py
+-rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/init/__init__.py
+-rw-r--r--   0        0        0     1137 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/init/parameters.py
+-rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/notebooks/__init__.py
+-rw-r--r--   0        0        0     1595 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/notebooks/comm.py
+-rw-r--r--   0        0        0     1854 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/notebooks/notebooks.py
+-rw-r--r--   0        0        0     4784 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/oauth.py
+-rw-r--r--   0        0        0    17298 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/operation.py
+-rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/operation_processors/__init__.py
+-rw-r--r--   0        0        0    13129 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/operation_processors/async_operation_processor.py
+-rw-r--r--   0        0        0     3073 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/operation_processors/factory.py
+-rw-r--r--   0        0        0     3936 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/operation_processors/lazy_operation_processor_wrapper.py
+-rw-r--r--   0        0        0     3070 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/operation_processors/offline_operation_processor.py
+-rw-r--r--   0        0        0     6886 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/operation_processors/operation_logger.py
+-rw-r--r--   0        0        0     1422 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/operation_processors/operation_processor.py
+-rw-r--r--   0        0        0     1146 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/operation_processors/read_only_operation_processor.py
+-rw-r--r--   0        0        0     3361 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/operation_processors/sync_operation_processor.py
+-rw-r--r--   0        0        0     2443 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/operation_processors/utils.py
+-rw-r--r--   0        0        0     3724 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/operation_visitor.py
+-rw-r--r--   0        0        0      886 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/patches/__init__.py
+-rw-r--r--   0        0        0     2731 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/patches/bravado.py
+-rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/signals_processing/__init__.py
+-rw-r--r--   0        0        0     2883 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/signals_processing/background_job.py
+-rw-r--r--   0        0        0     1663 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/signals_processing/signals.py
+-rw-r--r--   0        0        0     4899 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/signals_processing/signals_processor.py
+-rw-r--r--   0        0        0     1789 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/signals_processing/utils.py
+-rw-r--r--   0        0        0      776 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/state.py
+-rw-r--r--   0        0        0     1130 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/storage/__init__.py
+-rw-r--r--   0        0        0     3227 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/storage/datastream.py
+-rw-r--r--   0        0        0     7330 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/storage/storage_utils.py
+-rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/streams/__init__.py
+-rw-r--r--   0        0        0     1999 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/streams/std_capture_background_job.py
+-rw-r--r--   0        0        0     3066 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/streams/std_stream_capture_logger.py
+-rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/threading/__init__.py
+-rw-r--r--   0        0        0     5581 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/threading/daemon.py
+-rw-r--r--   0        0        0      596 2024-04-17 12:47:35.390597 neptune-2.0.0a2/src/neptune/internal/types/__init__.py
+-rw-r--r--   0        0        0     4586 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/types/file_types.py
+-rw-r--r--   0        0        0     2484 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/types/stringify_value.py
+-rw-r--r--   0        0        0      799 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/types/utils.py
+-rw-r--r--   0        0        0     5311 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/__init__.py
+-rw-r--r--   0        0        0     2409 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/dependency_tracking.py
+-rw-r--r--   0        0        0     2116 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/deprecation.py
+-rw-r--r--   0        0        0     5746 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/disk_utilization.py
+-rw-r--r--   0        0        0     2300 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/generic_attribute_mapper.py
+-rw-r--r--   0        0        0     6158 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/git.py
+-rw-r--r--   0        0        0     2490 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/git_info.py
+-rw-r--r--   0        0        0      849 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/hashing.py
+-rw-r--r--   0        0        0    10577 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/images.py
+-rw-r--r--   0        0        0     1152 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/iso_dates.py
+-rw-r--r--   0        0        0     1288 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/iteration.py
+-rw-r--r--   0        0        0     1657 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/limits.py
+-rw-r--r--   0        0        0     2972 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/logger.py
+-rw-r--r--   0        0        0     1065 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/paths.py
+-rw-r--r--   0        0        0      726 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/patterns.py
+-rw-r--r--   0        0        0     2187 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/ping_background_job.py
+-rw-r--r--   0        0        0     1809 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/process_killer.py
+-rw-r--r--   0        0        0     1168 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/requirement_check.py
+-rw-r--r--   0        0        0     1566 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/run_state.py
+-rw-r--r--   0        0        0     1143 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/runningmode.py
+-rw-r--r--   0        0        0     1345 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/s3.py
+-rw-r--r--   0        0        0     2266 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/source_code.py
+-rw-r--r--   0        0        0     2001 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/traceback_job.py
+-rw-r--r--   0        0        0     2450 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/uncaught_exception_handler.py
+-rw-r--r--   0        0        0     7575 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/utils/utils.py
+-rw-r--r--   0        0        0     4442 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/value_to_attribute_visitor.py
+-rw-r--r--   0        0        0     3284 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/warnings.py
+-rw-r--r--   0        0        0      596 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/websockets/__init__.py
+-rw-r--r--   0        0        0     3591 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/websockets/reconnecting_websocket.py
+-rw-r--r--   0        0        0     2638 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/websockets/websocket_client_adapter.py
+-rw-r--r--   0        0        0     5210 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/websockets/websocket_signals_background_job.py
+-rw-r--r--   0        0        0     1231 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/internal/websockets/websockets_factory.py
+-rw-r--r--   0        0        0     4795 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/management/__init__.py
+-rw-r--r--   0        0        0     6943 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/management/exceptions.py
+-rw-r--r--   0        0        0      596 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/management/internal/__init__.py
+-rw-r--r--   0        0        0    44742 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/management/internal/api.py
+-rw-r--r--   0        0        0     2853 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/management/internal/dto.py
+-rw-r--r--   0        0        0     1069 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/management/internal/types.py
+-rw-r--r--   0        0        0     2021 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/management/internal/utils.py
+-rw-r--r--   0        0        0      923 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/objects/__init__.py
+-rw-r--r--   0        0        0     2031 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/objects/abstract.py
+-rw-r--r--   0        0        0    15915 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/objects/model.py
+-rw-r--r--   0        0        0    13820 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/objects/model_version.py
+-rw-r--r--   0        0        0    26780 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/objects/neptune_object.py
+-rw-r--r--   0        0        0    19245 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/objects/project.py
+-rw-r--r--   0        0        0    26549 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/objects/run.py
+-rw-r--r--   0        0        0     1576 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/objects/structure_version.py
+-rw-r--r--   0        0        0     4043 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/objects/utils.py
+-rw-r--r--   0        0        0     5783 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/table.py
+-rw-r--r--   0        0        0     1071 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/types/__init__.py
+-rw-r--r--   0        0        0      914 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/types/atoms/__init__.py
+-rw-r--r--   0        0        0     1626 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/types/atoms/artifact.py
+-rw-r--r--   0        0        0      936 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/types/atoms/atom.py
+-rw-r--r--   0        0        0     1302 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/types/atoms/boolean.py
+-rw-r--r--   0        0        0     1435 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/types/atoms/datetime.py
+-rw-r--r--   0        0        0    12157 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/types/atoms/file.py
+-rw-r--r--   0        0        0     1297 2024-04-17 12:47:35.394597 neptune-2.0.0a2/src/neptune/types/atoms/float.py
+-rw-r--r--   0        0        0     1902 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/atoms/git_ref.py
+-rw-r--r--   0        0        0     1299 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/atoms/integer.py
+-rw-r--r--   0        0        0     1473 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/atoms/string.py
+-rw-r--r--   0        0        0     1485 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/file_set.py
+-rw-r--r--   0        0        0      831 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/mode.py
+-rw-r--r--   0        0        0      777 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/model_version_stage.py
+-rw-r--r--   0        0        0     1753 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/namespace.py
+-rw-r--r--   0        0        0      783 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/series/__init__.py
+-rw-r--r--   0        0        0     2473 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/series/file_series.py
+-rw-r--r--   0        0        0     3854 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/series/float_series.py
+-rw-r--r--   0        0        0     1221 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/series/series.py
+-rw-r--r--   0        0        0     1353 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/series/series_value.py
+-rw-r--r--   0        0        0     2601 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/series/string_series.py
+-rw-r--r--   0        0        0      655 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/sets/__init__.py
+-rw-r--r--   0        0        0      934 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/sets/set.py
+-rw-r--r--   0        0        0     1119 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/sets/string_set.py
+-rw-r--r--   0        0        0     3551 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/type_casting.py
+-rw-r--r--   0        0        0      892 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/value.py
+-rw-r--r--   0        0        0     1634 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/value_copy.py
+-rw-r--r--   0        0        0     2596 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/types/value_visitor.py
+-rw-r--r--   0        0        0     3089 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/typing.py
+-rw-r--r--   0        0        0     4310 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/utils.py
+-rw-r--r--   0        0        0        0 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/vendor/__init__.py
+-rw-r--r--   0        0        0     6306 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/vendor/lib_programname.py
+-rw-r--r--   0        0        0    68552 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/vendor/pynvml.py
+-rw-r--r--   0        0        0     1431 2024-04-17 12:47:35.398597 neptune-2.0.0a2/src/neptune/version.py
+-rw-r--r--   0        0        0    16599 1970-01-01 00:00:00.000000 neptune-2.0.0a2/PKG-INFO
```

### Comparing `neptune-2.0.0a1/CHANGELOG.md` & `neptune-2.0.0a2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,29 +10,34 @@
 - Deleted `neptune.logging` package ([#1698](https://github.com/neptune-ai/neptune-client/pull/1698))
 - Disabled `Model` ([#1701](https://github.com/neptune-ai/neptune-client/pull/1701))
 - Disabled `ModelVersion` ([#1701](https://github.com/neptune-ai/neptune-client/pull/1708))
 - Disabled `Project` ([#1709](https://github.com/neptune-ai/neptune-client/pull/1709))
 - Disabled `neptune command-line tool` ([#1718](https://github.com/neptune-ai/neptune-client/pull/1718))
 - Disabled deleting fields in `Handler` ([#1729](https://github.com/neptune-ai/neptune-client/pull/1729))
 - Removed `AbstractNeptuneObject` ([#1725](https://github.com/neptune-ai/neptune-client/pull/1725))
+- Disabled artifact-related methods in `Handler` ([#1734](https://github.com/neptune-ai/neptune-client/pull/1734))
+- Removed `boto3` from requirements ([#1743](https://github.com/neptune-ai/neptune-client/pull/1743))
+- Disabled `StringSet` `remove` and `clear` methods ([#1732](https://github.com/neptune-ai/neptune-client/pull/1732))
+- Disable `fetch_last` and `download_last` ([#1731](https://github.com/neptune-ai/neptune-client/pull/1731))
+- Disabled file related functionality ([#1726](https://github.com/neptune-ai/neptune-client/pull/1726))
 
 ### Changes
 - Stop sending `X-Neptune-LegacyClient` header ([#1715](https://github.com/neptune-ai/neptune-client/pull/1715))
 - Use `tqdm.auto` ([#1717](https://github.com/neptune-ai/neptune-client/pull/1717))
 - Fields DTO conversion reworked ([#1722](https://github.com/neptune-ai/neptune-client/pull/1722))
 - Added support for Protocol Buffers ([#1728](https://github.com/neptune-ai/neptune-client/pull/1728))
-
-### Features
-- ?
+- Series values DTO conversion reworked with protocol buffer support ([#1738](https://github.com/neptune-ai/neptune-client/pull/1738))
+- Series values fetching reworked with protocol buffer support ([#1744](https://github.com/neptune-ai/neptune-client/pull/1744))
 
 ### Fixes
 - Fixed `tqdm.notebook` import only in Notebook environment ([#1716](https://github.com/neptune-ai/neptune-client/pull/1716))
 - Added `setuptools` to dependencies for `python >= 3.12` ([#1721](https://github.com/neptune-ai/neptune-client/pull/1721))
 - Fixed compatibility checks with pre-release versions ([#1730](https://github.com/neptune-ai/neptune-client/pull/1730))
 - Added `Accept` and `Accept-Encoding` headers to protocol buffer requests ([#1736](https://github.com/neptune-ai/neptune-client/pull/1736))
+- Fixed default params for getAttributesWithPathsFilter ([#1740](https://github.com/neptune-ai/neptune-client/pull/1740))
 
 
 ## neptune 1.10.0
 
 ### Features
 - Added `get_workspace_status()` method to management API ([#1662](https://github.com/neptune-ai/neptune-client/pull/1662))
 - Added auto-scaling pixel values for image logging ([#1664](https://github.com/neptune-ai/neptune-client/pull/1664))
```

### Comparing `neptune-2.0.0a1/LICENSE` & `neptune-2.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/README.md` & `neptune-2.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/pyproject.toml` & `neptune-2.0.0a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 requests-oauthlib = ">=1.0.0"
 websocket-client = ">=0.35.0, !=1.0.0"
 urllib3 = "*"
 swagger-spec-validator = ">=2.7.4"
 protobuf = "^4.0.0"
 
 # Built-in integrations
-boto3 = ">=1.28.0"
 Pillow = ">=1.1.6"
 GitPython = ">=2.0.8"
 psutil = "*"
 pandas = "*"
 
 # Additional integrations
 kedro-neptune = { version = "*", optional = true, python = ">=3.9,<3.12" }
@@ -87,15 +86,15 @@
 repository = "https://github.com/neptune-ai/neptune-client"
 homepage = "https://neptune.ai/"
 documentation = "https://docs.neptune.ai/"
 include = ["CHANGELOG.md"]
 license = "Apache License 2.0"
 name = "neptune"
 readme = "README.md"
-version = "2.0.0-alpha.1"
+version = "2.0.0-alpha.2"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
```

### Comparing `neptune-2.0.0a1/src/neptune/__init__.py` & `neptune-2.0.0a2/src/neptune/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/api/__init__.py` & `neptune-2.0.0a2/src/neptune/api/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/api/field_visitor.py` & `neptune-2.0.0a2/src/neptune/api/field_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/api/models.py` & `neptune-2.0.0a2/src/neptune/api/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,14 +35,19 @@
     "ImageSeriesField",
     "StringSetField",
     "GitRefField",
     "ObjectStateField",
     "NotebookRefField",
     "ArtifactField",
     "FieldDefinition",
+    "FloatSeriesValues",
+    "FloatPointValue",
+    "StringSeriesValues",
+    "StringPointValue",
+    "ImageSeriesValues",
 )
 
 import abc
 import re
 from dataclasses import dataclass
 from dataclasses import field as dataclass_field
 from datetime import (
@@ -608,7 +613,128 @@
     @staticmethod
     def from_model(model: Any) -> FieldDefinition:
         return FieldDefinition(path=model.name, type=FieldType(model.type))
 
     @staticmethod
     def from_proto(data: ProtoAttributeDefinitionDTO) -> FieldDefinition:
         return FieldDefinition(path=data.name, type=FieldType(data.type))
+
+
+@dataclass
+class FloatSeriesValues:
+    total: int
+    values: List[FloatPointValue]
+
+    @staticmethod
+    def from_dict(data: Dict[str, Any]) -> FloatSeriesValues:
+        return FloatSeriesValues(
+            total=data["totalItemCount"], values=[FloatPointValue.from_dict(value) for value in data["values"]]
+        )
+
+    @staticmethod
+    def from_model(model: Any) -> FloatSeriesValues:
+        return FloatSeriesValues(
+            total=model.totalItemCount, values=[FloatPointValue.from_model(value) for value in model.values]
+        )
+
+    @staticmethod
+    def from_proto(data: Any) -> FloatSeriesValues:
+        return FloatSeriesValues(
+            total=data.total_item_count, values=[FloatPointValue.from_proto(value) for value in data.values]
+        )
+
+
+@dataclass
+class FloatPointValue:
+    timestamp: datetime
+    value: float
+    step: float
+
+    @staticmethod
+    def from_dict(data: Dict[str, Any]) -> FloatPointValue:
+        return FloatPointValue(
+            timestamp=datetime.fromtimestamp(data["timestampMillis"] / 1000.0, tz=timezone.utc),
+            value=float(data["value"]),
+            step=float(data["step"]),
+        )
+
+    @staticmethod
+    def from_model(model: Any) -> FloatPointValue:
+        return FloatPointValue(
+            timestamp=datetime.fromtimestamp(model.timestampMillis / 1000.0, tz=timezone.utc),
+            value=model.value,
+            step=model.step,
+        )
+
+    @staticmethod
+    def from_proto(data: Any) -> FloatPointValue:
+        return FloatPointValue(
+            timestamp=datetime.fromtimestamp(data.timestamp_millis / 1000.0, tz=timezone.utc),
+            value=data.value,
+            step=data.step,
+        )
+
+
+@dataclass
+class StringSeriesValues:
+    total: int
+    values: List[StringPointValue]
+
+    @staticmethod
+    def from_dict(data: Dict[str, Any]) -> StringSeriesValues:
+        return StringSeriesValues(
+            total=data["totalItemCount"], values=[StringPointValue.from_dict(value) for value in data["values"]]
+        )
+
+    @staticmethod
+    def from_model(model: Any) -> StringSeriesValues:
+        return StringSeriesValues(
+            total=model.totalItemCount, values=[StringPointValue.from_model(value) for value in model.values]
+        )
+
+    @staticmethod
+    def from_proto(data: Any) -> StringSeriesValues:
+        raise NotImplementedError()
+
+
+@dataclass
+class StringPointValue:
+    timestamp: datetime
+    step: float
+    value: str
+
+    @staticmethod
+    def from_dict(data: Dict[str, Any]) -> StringPointValue:
+        return StringPointValue(
+            timestamp=datetime.fromtimestamp(data["timestampMillis"] / 1000.0, tz=timezone.utc),
+            value=str(data["value"]),
+            step=float(data["step"]),
+        )
+
+    @staticmethod
+    def from_model(model: Any) -> StringPointValue:
+        return StringPointValue(
+            timestamp=datetime.fromtimestamp(model.timestampMillis / 1000.0, tz=timezone.utc),
+            value=model.value,
+            step=model.step,
+        )
+
+    @staticmethod
+    def from_proto(data: Any) -> StringPointValue:
+        raise NotImplementedError()
+
+
+@dataclass
+class ImageSeriesValues:
+    total: int
+
+    @staticmethod
+    def from_dict(data: Dict[str, Any]) -> ImageSeriesValues:
+        return ImageSeriesValues(total=data["totalItemCount"])
+
+    @staticmethod
+    def from_model(model: Any) -> ImageSeriesValues:
+        return ImageSeriesValues(total=model.totalItemCount)
+
+    @staticmethod
+    def from_proto(data: Any) -> ImageSeriesValues:
+        raise NotImplementedError()
```

### Comparing `neptune-2.0.0a1/src/neptune/api/proto/__init__.py` & `neptune-2.0.0a2/src/neptune/api/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/api/proto/neptune_pb/__init__.py` & `neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/api/proto/neptune_pb/api/__init__.py` & `neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/api/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/api/proto/neptune_pb/api/model/__init__.py` & `neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/api/proto/neptune_pb/api/model/attributes_pb2.py` & `neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/api/model/attributes_pb2.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/api/proto/neptune_pb/api/model/attributes_pb2.pyi` & `neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/api/model/attributes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/api/proto/neptune_pb/api/model/leaderboard_entries_pb2.py` & `neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/api/model/leaderboard_entries_pb2.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/api/proto/neptune_pb/api/model/leaderboard_entries_pb2.pyi` & `neptune-2.0.0a2/src/neptune/api/proto/neptune_pb/api/model/leaderboard_entries_pb2.pyi`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/api/requests_utils.py` & `neptune-2.0.0a2/src/neptune/api/requests_utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/api/searching_entries.py` & `neptune-2.0.0a2/src/neptune/api/searching_entries.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/attributes/__init__.py` & `neptune-2.0.0a2/src/neptune/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/attributes/atoms/__init__.py` & `neptune-2.0.0a2/src/neptune/attributes/atoms/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/attributes/atoms/artifact.py` & `neptune-2.0.0a2/src/neptune/attributes/atoms/artifact.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/attributes/atoms/atom.py` & `neptune-2.0.0a2/src/neptune/attributes/atoms/atom.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/attributes/atoms/boolean.py` & `neptune-2.0.0a2/src/neptune/attributes/atoms/boolean.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/attributes/atoms/copiable_atom.py` & `neptune-2.0.0a2/src/neptune/attributes/atoms/copiable_atom.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/attributes/atoms/datetime.py` & `neptune-2.0.0a2/src/neptune/attributes/atoms/datetime.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/attributes/atoms/file.py` & `neptune-2.0.0a2/src/neptune/attributes/atoms/file.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,40 +14,45 @@
 # limitations under the License.
 #
 __all__ = ["File"]
 
 from typing import Optional
 
 from neptune.attributes.atoms.atom import Atom
+from neptune.exceptions import NeptuneUnsupportedFunctionalityException
 from neptune.internal.operation import UploadFile
 from neptune.internal.utils import verify_type
 from neptune.types.atoms.file import File as FileVal
 from neptune.typing import ProgressBarType
 
 
 class File(Atom):
     def assign(self, value: FileVal, *, wait: bool = False) -> None:
+        raise NeptuneUnsupportedFunctionalityException
         verify_type("value", value, FileVal)
 
         operation = UploadFile.of_file(
             value=value,
             attribute_path=self._path,
             operation_storage=self._container._op_processor.operation_storage,
         )
 
         with self._container.lock():
             self._enqueue_operation(operation, wait=wait)
 
     def upload(self, value, *, wait: bool = False) -> None:
+        raise NeptuneUnsupportedFunctionalityException
         self.assign(FileVal.create_from(value), wait=wait)
 
     def download(
         self,
         destination: Optional[str] = None,
         progress_bar: Optional[ProgressBarType] = None,
     ) -> None:
+        raise NeptuneUnsupportedFunctionalityException
         verify_type("destination", destination, (str, type(None)))
         self._backend.download_file(self._container_id, self._container_type, self._path, destination, progress_bar)
 
     def fetch_extension(self) -> str:
+        raise NeptuneUnsupportedFunctionalityException
         val = self._backend.get_file_attribute(self._container_id, self._container_type, self._path)
         return val.ext
```

### Comparing `neptune-2.0.0a1/src/neptune/attributes/atoms/float.py` & `neptune-2.0.0a2/src/neptune/attributes/atoms/float.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/attributes/atoms/git_ref.py` & `neptune-2.0.0a2/src/neptune/attributes/atoms/git_ref.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/attributes/atoms/integer.py` & `neptune-2.0.0a2/src/neptune/attributes/atoms/integer.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/attributes/atoms/notebook_ref.py` & `neptune-2.0.0a2/src/neptune/attributes/atoms/notebook_ref.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/attributes/atoms/run_state.py` & `neptune-2.0.0a2/src/neptune/attributes/atoms/run_state.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/attributes/atoms/string.py` & `neptune-2.0.0a2/src/neptune/attributes/atoms/string.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/attributes/attribute.py` & `neptune-2.0.0a2/src/neptune/attributes/attribute.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/attributes/constants.py` & `neptune-2.0.0a2/src/neptune/attributes/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/attributes/file_set.py` & `neptune-2.0.0a2/src/neptune/attributes/series/fetchable_series.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,73 +9,60 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__all__ = ["FileSet"]
+__all__ = ["FetchableSeries"]
 
-import os
+import abc
+from datetime import datetime
 from typing import (
-    Iterable,
-    List,
+    Dict,
+    Generic,
     Optional,
+    TypeVar,
     Union,
 )
 
-from neptune.api.models import FileEntry
-from neptune.attributes.attribute import Attribute
-from neptune.internal.operation import (
-    DeleteFiles,
-    UploadFileSet,
+from neptune.api.fetching_series_values import fetch_series_values
+from neptune.api.models import (
+    FloatPointValue,
+    StringPointValue,
 )
-from neptune.internal.utils import (
-    verify_collection_type,
-    verify_type,
-)
-from neptune.types.file_set import FileSet as FileSetVal
+from neptune.internal.utils.paths import path_to_str
 from neptune.typing import ProgressBarType
 
+Row = TypeVar("Row", StringPointValue, FloatPointValue)
+
+
+def make_row(entry: Row, include_timestamp: bool = True) -> Dict[str, Union[str, float, datetime]]:
+    row: Dict[str, Union[str, float, datetime]] = {
+        "step": entry.step,
+        "value": entry.value,
+    }
+
+    if include_timestamp:
+        row["timestamp"] = entry.timestamp
+
+    return row
+
+
+class FetchableSeries(Generic[Row]):
+    @abc.abstractmethod
+    def _fetch_values_from_backend(self, limit: int, from_step: Optional[float] = None) -> Row: ...
+
+    def fetch_values(self, *, include_timestamp: bool = True, progress_bar: Optional[ProgressBarType] = None):
+        import pandas as pd
+
+        path = path_to_str(self._path) if hasattr(self, "_path") else ""
+        data = fetch_series_values(
+            getter=self._fetch_values_from_backend,
+            path=path,
+            progress_bar=progress_bar,
+        )
+
+        rows = dict((n, make_row(entry=entry, include_timestamp=include_timestamp)) for (n, entry) in enumerate(data))
 
-class FileSet(Attribute):
-    def assign(self, value: Union[FileSetVal, str, Iterable[str]], *, wait: bool = False) -> None:
-        verify_type("value", value, (FileSetVal, str, Iterable))
-        if isinstance(value, FileSetVal):
-            value = value.file_globs
-        elif isinstance(value, str):
-            value = [value]
-        else:
-            verify_collection_type("value", value, str)
-        self._enqueue_upload_operation(value, reset=True, wait=wait)
-
-    def upload_files(self, globs: Union[str, Iterable[str]], *, wait: bool = False) -> None:
-        if isinstance(globs, str):
-            globs = [globs]
-        else:
-            verify_collection_type("globs", globs, str)
-        self._enqueue_upload_operation(globs, reset=False, wait=wait)
-
-    def delete_files(self, paths: Union[str, Iterable[str]], *, wait: bool = False) -> None:
-        if isinstance(paths, str):
-            paths = [paths]
-        else:
-            verify_collection_type("paths", paths, str)
-        with self._container.lock():
-            self._enqueue_operation(DeleteFiles(self._path, set(paths)), wait=wait)
-
-    def _enqueue_upload_operation(self, globs: Iterable[str], *, reset: bool, wait: bool):
-        with self._container.lock():
-            abs_file_globs = list(os.path.abspath(file_glob) for file_glob in globs)
-            self._enqueue_operation(UploadFileSet(self._path, abs_file_globs, reset=reset), wait=wait)
-
-    def download(
-        self,
-        destination: Optional[str] = None,
-        progress_bar: Optional[ProgressBarType] = None,
-    ) -> None:
-        verify_type("destination", destination, (str, type(None)))
-        self._backend.download_file_set(self._container_id, self._container_type, self._path, destination, progress_bar)
-
-    def list_fileset_files(self, path: Optional[str] = None) -> List[FileEntry]:
-        path = path or ""
-        return self._backend.list_fileset_files(self._path, self._container_id, path)
+        df = pd.DataFrame.from_dict(data=rows, orient="index")
+        return df
```

### Comparing `neptune-2.0.0a1/src/neptune/attributes/namespace.py` & `neptune-2.0.0a2/src/neptune/attributes/namespace.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/attributes/series/__init__.py` & `neptune-2.0.0a2/src/neptune/attributes/series/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/attributes/series/file_series.py` & `neptune-2.0.0a2/src/neptune/attributes/series/file_series.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     Image,
     UnidentifiedImageError,
 )
 
 from neptune.attributes.series.series import Series
 from neptune.exceptions import (
     FileNotFound,
+    NeptuneUnsupportedFunctionalityException,
     OperationNotSupported,
 )
 from neptune.internal.operation import (
     ClearImageLog,
     ImageValue,
     LogImages,
     Operation,
@@ -96,25 +97,26 @@
 
         return base64_encode(file_content)
 
     def download(self, destination: Optional[str], progress_bar: Optional[ProgressBarType] = None):
         target_dir = self._get_destination(destination)
         item_count = self._backend.get_image_series_values(
             self._container_id, self._container_type, self._path, 0, 1
-        ).totalItemCount
+        ).total
         for i in range(0, item_count):
             self._backend.download_file_series_by_index(
                 self._container_id, self._container_type, self._path, i, target_dir, progress_bar
             )
 
     def download_last(self, destination: Optional[str]):
+        raise NeptuneUnsupportedFunctionalityException
         target_dir = self._get_destination(destination)
         item_count = self._backend.get_image_series_values(
             self._container_id, self._container_type, self._path, 0, 1
-        ).totalItemCount
+        ).total
         if item_count > 0:
             self._backend.download_file_series_by_index(
                 self._container_id,
                 self._container_type,
                 self._path,
                 item_count - 1,
                 target_dir,
```

### Comparing `neptune-2.0.0a1/src/neptune/attributes/series/float_series.py` & `neptune-2.0.0a2/src/neptune/attributes/series/float_series.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 
 from typing import (
     Iterable,
     Optional,
     Union,
 )
 
+from neptune.api.models import FloatSeriesValues
 from neptune.attributes.series.fetchable_series import FetchableSeries
 from neptune.attributes.series.series import Series
-from neptune.internal.backends.api_model import FloatSeriesValues
+from neptune.exceptions import NeptuneUnsupportedFunctionalityException
 from neptune.internal.operation import (
     ClearFloatLog,
     ConfigFloatSeries,
     LogFloats,
     Operation,
 )
 from neptune.internal.utils import verify_type
@@ -63,14 +64,19 @@
     def _data_to_value(self, values: Iterable, **kwargs) -> Val:
         return FloatSeriesVal(values, **kwargs)
 
     def _is_value_type(self, value) -> bool:
         return isinstance(value, FloatSeriesVal)
 
     def fetch_last(self) -> float:
+        raise NeptuneUnsupportedFunctionalityException
         val = self._backend.get_float_series_attribute(self._container_id, self._container_type, self._path)
         return val.last
 
-    def _fetch_values_from_backend(self, offset, limit) -> FloatSeriesValues:
+    def _fetch_values_from_backend(self, limit: int, from_step: Optional[float] = None) -> FloatSeriesValues:
         return self._backend.get_float_series_values(
-            self._container_id, self._container_type, self._path, offset, limit
+            container_id=self._container_id,
+            container_type=self._container_type,
+            path=self._path,
+            from_step=from_step,
+            limit=limit,
         )
```

### Comparing `neptune-2.0.0a1/src/neptune/attributes/series/series.py` & `neptune-2.0.0a2/src/neptune/attributes/series/series.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/attributes/series/string_series.py` & `neptune-2.0.0a2/src/neptune/attributes/series/string_series.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,20 +15,22 @@
 #
 __all__ = ["StringSeries"]
 
 from typing import (
     TYPE_CHECKING,
     Iterable,
     List,
+    Optional,
     Union,
 )
 
+from neptune.api.models import StringSeriesValues
 from neptune.attributes.series.fetchable_series import FetchableSeries
 from neptune.attributes.series.series import Series
-from neptune.internal.backends.api_model import StringSeriesValues
+from neptune.exceptions import NeptuneUnsupportedFunctionalityException
 from neptune.internal.operation import (
     ClearStringLog,
     LogStrings,
     Operation,
 )
 from neptune.internal.utils import is_collection
 from neptune.internal.utils.logger import get_logger
@@ -87,14 +89,19 @@
 
     def _handle_stringified_value(self, value) -> Union[List[str], str]:
         if is_collection(value.value):
             return list(map(str, value.value))
         return str(value.value)
 
     def fetch_last(self) -> str:
+        raise NeptuneUnsupportedFunctionalityException
         val = self._backend.get_string_series_attribute(self._container_id, self._container_type, self._path)
         return val.last
 
-    def _fetch_values_from_backend(self, offset, limit) -> StringSeriesValues:
+    def _fetch_values_from_backend(self, limit: int, from_step: Optional[float] = None) -> StringSeriesValues:
         return self._backend.get_string_series_values(
-            self._container_id, self._container_type, self._path, offset, limit
+            container_id=self._container_id,
+            container_type=self._container_type,
+            path=self._path,
+            from_step=from_step,
+            limit=limit,
         )
```

### Comparing `neptune-2.0.0a1/src/neptune/attributes/sets/__init__.py` & `neptune-2.0.0a2/src/neptune/attributes/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/attributes/sets/set.py` & `neptune-2.0.0a2/src/neptune/attributes/sets/set.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/attributes/sets/string_set.py` & `neptune-2.0.0a2/src/neptune/attributes/sets/string_set.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import typing
 from typing import (
     Iterable,
     Union,
 )
 
 from neptune.attributes.sets.set import Set
+from neptune.exceptions import NeptuneUnsupportedFunctionalityException
 from neptune.internal.operation import (
     AddStrings,
     ClearStringSet,
     RemoveStrings,
 )
 from neptune.internal.utils import (
     is_collection,
@@ -47,19 +48,21 @@
 
     def add(self, values: Union[str, Iterable[str]], *, wait: bool = False):
         values = self._to_proper_value_type(values)
         with self._container.lock():
             self._enqueue_operation(AddStrings(self._path, set(values)), wait=wait)
 
     def remove(self, values: Union[str, Iterable[str]], *, wait: bool = False):
+        raise NeptuneUnsupportedFunctionalityException
         values = self._to_proper_value_type(values)
         with self._container.lock():
             self._enqueue_operation(RemoveStrings(self._path, set(values)), wait=wait)
 
     def clear(self, *, wait: bool = False):
+        raise NeptuneUnsupportedFunctionalityException
         with self._container.lock():
             self._enqueue_operation(ClearStringSet(self._path), wait=wait)
 
     def fetch(self) -> typing.Set[str]:
         val = self._backend.get_string_set_attribute(self._container_id, self._container_type, self._path)
         return val.values
```

### Comparing `neptune-2.0.0a1/src/neptune/attributes/utils.py` & `neptune-2.0.0a2/src/neptune/attributes/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/cli/__init__.py` & `neptune-2.0.0a2/src/neptune/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/cli/__main__.py` & `neptune-2.0.0a2/src/neptune/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/cli/clear.py` & `neptune-2.0.0a2/src/neptune/cli/clear.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/cli/collect.py` & `neptune-2.0.0a2/src/neptune/cli/collect.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/cli/commands.py` & `neptune-2.0.0a2/src/neptune/cli/commands.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/cli/containers.py` & `neptune-2.0.0a2/src/neptune/cli/containers.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/cli/path_option.py` & `neptune-2.0.0a2/src/neptune/cli/path_option.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/cli/status.py` & `neptune-2.0.0a2/src/neptune/cli/status.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/cli/sync.py` & `neptune-2.0.0a2/src/neptune/cli/sync.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/cli/utils.py` & `neptune-2.0.0a2/src/neptune/cli/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/constants.py` & `neptune-2.0.0a2/src/neptune/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/core/__init__.py` & `neptune-2.0.0a2/src/neptune/core/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/core/components/__init__.py` & `neptune-2.0.0a2/src/neptune/core/components/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/core/components/abstract.py` & `neptune-2.0.0a2/src/neptune/core/components/abstract.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/core/components/metadata_file.py` & `neptune-2.0.0a2/src/neptune/core/components/metadata_file.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/core/components/operation_storage.py` & `neptune-2.0.0a2/src/neptune/core/components/operation_storage.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/core/components/queue/__init__.py` & `neptune-2.0.0a2/src/neptune/core/components/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/core/components/queue/disk_queue.py` & `neptune-2.0.0a2/src/neptune/core/components/queue/disk_queue.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/core/components/queue/json_file_splitter.py` & `neptune-2.0.0a2/src/neptune/core/components/queue/json_file_splitter.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/core/components/queue/log_file.py` & `neptune-2.0.0a2/src/neptune/core/components/queue/log_file.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/core/components/queue/sync_offset_file.py` & `neptune-2.0.0a2/src/neptune/core/components/queue/sync_offset_file.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/envs.py` & `neptune-2.0.0a2/src/neptune/envs.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     "NEPTUNE_REQUEST_TIMEOUT",
     "NEPTUNE_MAX_DISK_USAGE",
     "NEPTUNE_RAISE_ERROR_ON_DISK_USAGE_EXCEEDED",
     "NEPTUNE_ENABLE_DEFAULT_ASYNC_LAG_CALLBACK",
     "NEPTUNE_ENABLE_DEFAULT_ASYNC_NO_PROGRESS_CALLBACK",
     "NEPTUNE_USE_PROTOCOL_BUFFERS",
     "NEPTUNE_ASYNC_BATCH_SIZE",
+    "S3_ENDPOINT_URL",
 ]
 
 from neptune.internal.envs import (
     API_TOKEN_ENV_NAME,
     NEPTUNE_RETRIES_TIMEOUT_ENV,
 )
```

### Comparing `neptune-2.0.0a1/src/neptune/exceptions.py` & `neptune-2.0.0a2/src/neptune/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/handler.py` & `neptune-2.0.0a2/src/neptune/handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 #
 __all__ = ["Handler"]
 
 from functools import wraps
 from typing import (
     TYPE_CHECKING,
     Any,
+    Callable,
     Collection,
     Dict,
     Iterable,
     Iterator,
     List,
     Optional,
     Union,
@@ -69,14 +70,21 @@
 from neptune.typing import ProgressBarType
 from neptune.utils import stringify_unsupported
 
 if TYPE_CHECKING:
     from neptune.objects import NeptuneObject
 
 
+def feature_temporarily_unavailable(_: Callable[..., Any]) -> Callable[..., Any]:
+    def wrapper(*_, **__):
+        raise NeptuneUnsupportedFunctionalityException()
+
+    return wrapper
+
+
 def validate_path_not_protected(target_path: str, handler: "Handler"):
     path_protection_exception = handler._PROTECTED_PATHS.get(target_path)
     if path_protection_exception:
         raise path_protection_exception(target_path)
 
 
 def check_protected_paths(fun):
@@ -240,25 +248,27 @@
             >>> from neptune.types import File
             >>> run["dataset/data_sample"].upload(File("sample_data.csv"))
 
         For more information, see the docs:
            https://docs.neptune.ai/api/field_types#upload
 
         """
+        raise NeptuneUnsupportedFunctionalityException
         value = FileVal.create_from(value)
 
         with self._container.lock():
             attr = self._container.get_attribute(self._path)
             if attr is None:
                 attr = File(self._container, parse_path(self._path))
                 self._container.set_attribute(self._path, attr)
             attr.upload(value, wait=wait)
 
     @check_protected_paths
     def upload_files(self, value: Union[str, Iterable[str]], *, wait: bool = False) -> None:
+        raise NeptuneUnsupportedFunctionalityException
         if is_collection(value):
             verify_collection_type("value", value, str)
         else:
             verify_type("value", value, str)
 
         with self._container.lock():
             attr = self._container.get_attribute(self._path)
@@ -464,33 +474,14 @@
         with self._container.lock():
             attr = self._container.get_attribute(self._path)
             if attr is None:
                 attr = StringSet(self._container, parse_path(self._path))
                 self._container.set_attribute(self._path, attr)
             attr.add(values, wait=wait)
 
-    def _delete_item(self, path: str = None, *, wait: bool = False) -> None:
-        with self._container.lock():
-            handler = self
-            if path:
-                verify_type("path", path, str)
-                handler = self[path]
-                path = join_paths(self._path, path)
-                # extra check: check_protected_paths decorator does not catch flow with non-null path
-                validate_path_not_protected(path, self)
-            else:
-                path = self._path
-
-            attribute = self._container.get_attribute(path)
-            if isinstance(attribute, Namespace):
-                for child_path in list(attribute):
-                    handler.pop(child_path, wait=wait)
-            else:
-                self._container._pop_impl(parse_path(path), wait=wait)
-
     @check_protected_paths
     def remove(self, values: Union[str, Iterable[str]], *, wait: bool = False) -> None:
         """Removes the provided tags from the set.
 
         Args:
             values (str or collection of str): Tags to be removed.
             wait (bool, optional): If `True`, the client will wait to send all tracked metadata to the server first.
@@ -595,14 +586,15 @@
             wait (bool, optional): If `True`, the client will wait to send all tracked metadata to the server.
                 This makes the call synchronous.
                 Defaults to `None`.
 
         For more information, see the docs:
             https://docs.neptune.ai/api/field_types#delete_files
         """
+        raise NeptuneUnsupportedFunctionalityException
         return self._pass_call_to_attr(function_name="delete_files", paths=paths, wait=wait)
 
     @check_protected_paths
     def download(
         self,
         destination: Optional[str] = None,
         progress_bar: Optional[ProgressBarType] = None,
@@ -628,14 +620,15 @@
                 If `False` no progress bar will be used.
                 If a type of progress bar is passed, it will be used instead of the default one.
                 Defaults to `None`.
 
         For more information, see the docs:
            https://docs.neptune.ai/api-reference/field-types
         """
+        raise NeptuneUnsupportedFunctionalityException
         return self._pass_call_to_attr(function_name="download", destination=destination, progress_bar=progress_bar)
 
     def download_last(self, destination: str = None) -> None:
         """Downloads the stored files to the working directory or to the specified destination.
 
         Args:
             destination (str, optional): Path to where the file(s) should be downloaded.
@@ -646,36 +639,40 @@
                 Defaults to `None`.
 
         For more information, see the docs:
            https://docs.neptune.ai/api/field_types#download_last
         """
         return self._pass_call_to_attr(function_name="download_last", destination=destination)
 
+    @feature_temporarily_unavailable
     def fetch_hash(self) -> str:
         """Fetches the hash of an artifact.
 
         You may also want to check the docs:
            https://docs.neptune.ai/api/field_types#fetch_hash
         """
         return self._pass_call_to_attr(function_name="fetch_hash")
 
     def fetch_extension(self) -> str:
         """Fetches the extension of a file.
 
         You may also want to check the docs:
            https://docs.neptune.ai/api/field_types#fetch_extension
         """
+        raise NeptuneUnsupportedFunctionalityException
         return self._pass_call_to_attr(function_name="fetch_extension")
 
+    @feature_temporarily_unavailable
     def fetch_files_list(self) -> List[ArtifactFileData]:
         """Fetches the list of files in an artifact and their metadata.
 
         You may also want to check the docs:
            https://docs.neptune.ai/api/field_types#fetch_files_list
         """
+        raise NeptuneUnsupportedFunctionalityException
         return self._pass_call_to_attr(function_name="fetch_files_list")
 
     def list_fileset_files(self, path: Optional[str] = None) -> List[FileEntry]:
         """Fetches metadata of the file set.
 
         If the top-level artifact of the field is a directory, only the metadata of this directory is returned.
         You can use the `path` argument to list metadata of the files contained inside the directory or subdirectories.
@@ -705,40 +702,60 @@
             [FileEntry(name='sample_v2.csv', size=215, mtime=datetime.datetime(2023, 8, 17, 10, 31, 26, 491000,
             tzinfo=tzutc()), file_type='file'), FileEntry(name='sample_v3.csv', size=215, mtime=datetime.datetime(2023,
             8, 17, 10, 31, 26, 338000, tzinfo=tzutc()), file_type='file'), ...]
 
         For more information, see the API reference:
            https://docs.neptune.ai/api/field_types#list_fileset_files
         """
+        raise NeptuneUnsupportedFunctionalityException
         return self._pass_call_to_attr(function_name="list_fileset_files", path=path)
 
     def _pass_call_to_attr(self, function_name, **kwargs):
         return getattr(self._get_attribute(), function_name)(**kwargs)
 
+    @feature_temporarily_unavailable
     @check_protected_paths
     def track_files(self, path: str, *, destination: str = None, wait: bool = False) -> None:
         """Creates an artifact tracking some files.
 
         You may also want to check the docs:
            https://docs.neptune.ai/api/field_types#track_files
         """
+        raise NeptuneUnsupportedFunctionalityException
         with self._container.lock():
             attr = self._container.get_attribute(self._path)
             if attr is None:
                 attr = Artifact(self._container, parse_path(self._path))
                 self._container.set_attribute(self._path, attr)
 
             attr.track_files(path=path, destination=destination, wait=wait)
 
     def __delitem__(self, path) -> None:
-        raise NeptuneUnsupportedFunctionalityException()
+        self.pop(path)
 
+    @feature_temporarily_unavailable
     @check_protected_paths
     def pop(self, path: str = None, *, wait: bool = False) -> None:
-        raise NeptuneUnsupportedFunctionalityException()
+        with self._container.lock():
+            handler = self
+            if path:
+                verify_type("path", path, str)
+                handler = self[path]
+                path = join_paths(self._path, path)
+                # extra check: check_protected_paths decorator does not catch flow with non-null path
+                validate_path_not_protected(path, self)
+            else:
+                path = self._path
+
+            attribute = self._container.get_attribute(path)
+            if isinstance(attribute, Namespace):
+                for child_path in list(attribute):
+                    handler.pop(child_path, wait=wait)
+            else:
+                self._container._pop_impl(parse_path(path), wait=wait)
 
 
 class ExtendUtils:
     @staticmethod
     def transform_to_extend_format(value):
         """Preserves the nested structure created by `Namespaces` and `dict_like` objects,
         but replaces all other values with single-element lists,
```

### Comparing `neptune-2.0.0a1/src/neptune/integrations/__init__.py` & `neptune-2.0.0a2/src/neptune/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/integrations/aws/__init__.py` & `neptune-2.0.0a2/src/neptune/integrations/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/integrations/detectron2/__init__.py` & `neptune-2.0.0a2/src/neptune/integrations/detectron2/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/integrations/fastai/__init__.py` & `neptune-2.0.0a2/src/neptune/integrations/fastai/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/integrations/kedro/__init__.py` & `neptune-2.0.0a2/src/neptune/integrations/kedro/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/integrations/lightgbm/__init__.py` & `neptune-2.0.0a2/src/neptune/integrations/lightgbm/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/integrations/mosaicml/__init__.py` & `neptune-2.0.0a2/src/neptune/integrations/mosaicml/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/integrations/optuna/__init__.py` & `neptune-2.0.0a2/src/neptune/integrations/optuna/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/integrations/pandas/__init__.py` & `neptune-2.0.0a2/src/neptune/integrations/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/integrations/prophet/__init__.py` & `neptune-2.0.0a2/src/neptune/integrations/prophet/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/integrations/python_logger.py` & `neptune-2.0.0a2/src/neptune/integrations/python_logger.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/integrations/pytorch/__init__.py` & `neptune-2.0.0a2/src/neptune/integrations/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/integrations/pytorch_lightning/__init__.py` & `neptune-2.0.0a2/src/neptune/integrations/pytorch_lightning/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/integrations/sacred/__init__.py` & `neptune-2.0.0a2/src/neptune/integrations/sacred/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/integrations/sklearn/__init__.py` & `neptune-2.0.0a2/src/neptune/integrations/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/integrations/tensorboard/__init__.py` & `neptune-2.0.0a2/src/neptune/integrations/tensorboard/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/integrations/tensorflow_keras/__init__.py` & `neptune-2.0.0a2/src/neptune/integrations/tensorflow_keras/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/integrations/transformers/__init__.py` & `neptune-2.0.0a2/src/neptune/integrations/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/integrations/utils.py` & `neptune-2.0.0a2/src/neptune/integrations/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/integrations/xgboost/__init__.py` & `neptune-2.0.0a2/src/neptune/integrations/xgboost/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/__init__.py` & `neptune-2.0.0a2/src/neptune/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/artifacts/__init__.py` & `neptune-2.0.0a2/src/neptune/internal/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/artifacts/drivers/__init__.py` & `neptune-2.0.0a2/src/neptune/internal/artifacts/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/artifacts/drivers/local.py` & `neptune-2.0.0a2/src/neptune/internal/artifacts/drivers/local.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/artifacts/drivers/s3.py` & `neptune-2.0.0a2/src/neptune/internal/artifacts/drivers/s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 __all__ = ["S3ArtifactDriver"]
 
 import pathlib
 import typing
 from datetime import datetime
 from urllib.parse import urlparse
 
-from botocore.exceptions import NoCredentialsError
-
 from neptune.exceptions import (
     NeptuneRemoteStorageAccessException,
     NeptuneRemoteStorageCredentialsException,
     NeptuneUnsupportedArtifactFunctionalityException,
 )
 from neptune.internal.artifacts.types import (
     ArtifactDriver,
@@ -70,14 +68,16 @@
                 f"Wildcard characters (*,?) in location URI ({path}) are not supported."
             )
 
         remote_storage = get_boto_s3_client().Bucket(bucket_name)
 
         stored_files: typing.List[ArtifactFileData] = list()
 
+        from botocore.exceptions import NoCredentialsError
+
         try:
             for remote_object in remote_storage.objects.filter(Prefix=prefix):
                 # If prefix is path to file get only directories
                 if prefix == remote_object.key:
                     prefix = str(pathlib.PurePosixPath(prefix).parent)
 
                 remote_key = remote_object.key
@@ -113,14 +113,17 @@
     @classmethod
     def download_file(cls, destination: pathlib.Path, file_definition: ArtifactFileData):
         location = file_definition.metadata.get("location")
         url = urlparse(location)
         bucket_name, path = url.netloc, url.path.lstrip("/")
 
         remote_storage = get_boto_s3_client()
+
+        from botocore.exceptions import NoCredentialsError
+
         try:
             bucket = remote_storage.Bucket(bucket_name)
             bucket.download_file(path, str(destination))
         except NoCredentialsError:
             raise NeptuneRemoteStorageCredentialsException()
         except (
             remote_storage.meta.client.exceptions.NoSuchBucket,
```

### Comparing `neptune-2.0.0a1/src/neptune/internal/artifacts/file_hasher.py` & `neptune-2.0.0a2/src/neptune/internal/artifacts/file_hasher.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/artifacts/local_file_hash_storage.py` & `neptune-2.0.0a2/src/neptune/internal/artifacts/local_file_hash_storage.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/artifacts/types.py` & `neptune-2.0.0a2/src/neptune/internal/artifacts/types.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/artifacts/utils.py` & `neptune-2.0.0a2/src/neptune/internal/artifacts/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/backends/__init__.py` & `neptune-2.0.0a2/src/neptune/internal/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/backends/api_model.py` & `neptune-2.0.0a2/src/neptune/internal/backends/api_model.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,27 +16,21 @@
 __all__ = [
     "Project",
     "Workspace",
     "ApiExperiment",
     "OptionalFeatures",
     "VersionInfo",
     "ClientConfig",
-    "StringPointValue",
-    "ImageSeriesValues",
-    "StringSeriesValues",
-    "FloatPointValue",
-    "FloatSeriesValues",
     "ArtifactModel",
     "MultipartConfig",
 ]
 
 from dataclasses import dataclass
 from typing import (
     FrozenSet,
-    List,
     Optional,
 )
 
 from packaging import version
 
 from neptune.internal.container_type import ContainerType
 from neptune.internal.id_formats import (
@@ -178,42 +172,11 @@
             _missing_features=frozenset(missing_features),
             version_info=VersionInfo.build(min_recommended, min_compatible, max_compatible),
             multipart_config=multipart_upload_config,
         )
 
 
 @dataclass
-class StringPointValue:
-    timestampMillis: int
-    step: float
-    value: str
-
-
-@dataclass
-class ImageSeriesValues:
-    totalItemCount: int
-
-
-@dataclass
-class StringSeriesValues:
-    totalItemCount: int
-    values: List[StringPointValue]
-
-
-@dataclass
-class FloatPointValue:
-    timestampMillis: int
-    step: float
-    value: float
-
-
-@dataclass
-class FloatSeriesValues:
-    totalItemCount: int
-    values: List[FloatPointValue]
-
-
-@dataclass
 class ArtifactModel:
     received_metadata: bool
     hash: str
     size: int
```

### Comparing `neptune-2.0.0a1/src/neptune/internal/backends/factory.py` & `neptune-2.0.0a2/src/neptune/internal/backends/factory.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/backends/hosted_artifact_operations.py` & `neptune-2.0.0a2/src/neptune/internal/backends/hosted_artifact_operations.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/backends/hosted_client.py` & `neptune-2.0.0a2/src/neptune/internal/backends/hosted_client.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/backends/hosted_file_operations.py` & `neptune-2.0.0a2/src/neptune/internal/backends/hosted_file_operations.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/backends/hosted_neptune_backend.py` & `neptune-2.0.0a2/src/neptune/internal/backends/hosted_neptune_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,22 +45,26 @@
     Field,
     FieldDefinition,
     FieldType,
     FileEntry,
     FileField,
     FloatField,
     FloatSeriesField,
+    FloatSeriesValues,
+    ImageSeriesValues,
     IntField,
     LeaderboardEntry,
     StringField,
     StringSeriesField,
+    StringSeriesValues,
     StringSetField,
 )
 from neptune.api.proto.neptune_pb.api.model.attributes_pb2 import ProtoAttributesSearchResultDTO
 from neptune.api.proto.neptune_pb.api.model.leaderboard_entries_pb2 import ProtoAttributesDTO
+from neptune.api.proto.neptune_pb.api.model.series_values_pb2 import ProtoFloatSeriesValuesDTO
 from neptune.api.searching_entries import iter_over_pages
 from neptune.core.components.operation_storage import OperationStorage
 from neptune.envs import (
     NEPTUNE_FETCH_TABLE_STEP_SIZE,
     NEPTUNE_USE_PROTOCOL_BUFFERS,
 )
 from neptune.exceptions import (
@@ -75,21 +79,16 @@
     NeptuneObjectCreationConflict,
     ProjectNotFound,
     ProjectNotFoundWithSuggestions,
 )
 from neptune.internal.artifacts.types import ArtifactFileData
 from neptune.internal.backends.api_model import (
     ApiExperiment,
-    FloatPointValue,
-    FloatSeriesValues,
-    ImageSeriesValues,
     OptionalFeatures,
     Project,
-    StringPointValue,
-    StringSeriesValues,
     Workspace,
 )
 from neptune.internal.backends.hosted_artifact_operations import (
     get_artifact_attribute,
     list_artifact_files,
     track_to_existing_artifact,
     track_to_new_artifact,
@@ -953,65 +952,80 @@
             "attribute": path_to_str(path),
             "limit": limit,
             "offset": offset,
             **DEFAULT_REQUEST_KWARGS,
         }
         try:
             result = self.leaderboard_client.api.getImageSeriesValues(**params).response().result
-            return ImageSeriesValues(result.totalItemCount)
+            return ImageSeriesValues.from_model(result)
         except HTTPNotFound:
             raise FetchAttributeNotFoundException(path_to_str(path))
 
     @with_api_exceptions_handler
     def get_string_series_values(
         self,
         container_id: str,
         container_type: ContainerType,
         path: List[str],
-        offset: int,
         limit: int,
+        from_step: Optional[float] = None,
     ) -> StringSeriesValues:
         params = {
             "experimentId": container_id,
             "attribute": path_to_str(path),
             "limit": limit,
-            "offset": offset,
+            "skipToStep": from_step,
             **DEFAULT_REQUEST_KWARGS,
         }
         try:
             result = self.leaderboard_client.api.getStringSeriesValues(**params).response().result
-            return StringSeriesValues(
-                result.totalItemCount,
-                [StringPointValue(v.timestampMillis, v.step, v.value) for v in result.values],
-            )
+            return StringSeriesValues.from_model(result)
         except HTTPNotFound:
             raise FetchAttributeNotFoundException(path_to_str(path))
 
     @with_api_exceptions_handler
     def get_float_series_values(
         self,
         container_id: str,
         container_type: ContainerType,
         path: List[str],
-        offset: int,
         limit: int,
+        from_step: Optional[float] = None,
+        use_proto: Optional[bool] = None,
     ) -> FloatSeriesValues:
+        use_proto = use_proto if use_proto is not None else self.use_proto
+
         params = {
             "experimentId": container_id,
             "attribute": path_to_str(path),
             "limit": limit,
-            "offset": offset,
-            **DEFAULT_REQUEST_KWARGS,
+            "skipToStep": from_step,
         }
         try:
-            result = self.leaderboard_client.api.getFloatSeriesValues(**params).response().result
-            return FloatSeriesValues(
-                result.totalItemCount,
-                [FloatPointValue(v.timestampMillis, v.step, v.value) for v in result.values],
-            )
+            if use_proto:
+                result = (
+                    self.leaderboard_client.api.getFloatSeriesValuesProto(
+                        **params,
+                        **DEFAULT_PROTO_REQUEST_KWARGS,
+                    )
+                    .response()
+                    .result
+                )
+                data = ProtoFloatSeriesValuesDTO.FromString(result)
+                return FloatSeriesValues.from_proto(data)
+            else:
+                result = (
+                    self.leaderboard_client.api.getFloatSeriesValues(
+                        **params,
+                        **DEFAULT_REQUEST_KWARGS,
+                    )
+                    .response()
+                    .result
+                )
+                return FloatSeriesValues.from_model(result)
         except HTTPNotFound:
             raise FetchAttributeNotFoundException(path_to_str(path))
 
     @with_api_exceptions_handler
     def fetch_atom_attribute_values(
         self, container_id: str, container_type: ContainerType, path: List[str]
     ) -> List[Tuple[str, FieldType, Any]]:
@@ -1176,15 +1190,14 @@
 
         params = {
             "holderIdentifier": container_id,
             "holderType": "experiment",
             "attributeQuery": {
                 "attributePathsFilter": paths,
             },
-            **DEFAULT_REQUEST_KWARGS,
         }
 
         try:
             if use_proto:
                 result = (
                     self.leaderboard_client.api.getAttributesWithPathsFilterProto(
                         **params,
@@ -1192,15 +1205,22 @@
                     )
                     .response()
                     .result
                 )
                 data = ProtoAttributesDTO.FromString(result)
                 return [Field.from_proto(field) for field in data.attributes]
             else:
-                data = self.leaderboard_client.api.getAttributesWithPathsFilter(**params).response().result
+                data = (
+                    self.leaderboard_client.api.getAttributesWithPathsFilter(
+                        **params,
+                        **DEFAULT_REQUEST_KWARGS,
+                    )
+                    .response()
+                    .result
+                )
                 return [Field.from_model(field) for field in data.attributes]
         except HTTPNotFound as e:
             raise ContainerUUIDNotFound(
                 container_id=container_id,
                 container_type=container_type,
             ) from e
```

### Comparing `neptune-2.0.0a1/src/neptune/internal/backends/neptune_backend.py` & `neptune-2.0.0a2/src/neptune/internal/backends/neptune_backend.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,28 +32,28 @@
     Field,
     FieldDefinition,
     FieldType,
     FileEntry,
     FileField,
     FloatField,
     FloatSeriesField,
+    FloatSeriesValues,
+    ImageSeriesValues,
     IntField,
     LeaderboardEntry,
     StringField,
     StringSeriesField,
+    StringSeriesValues,
     StringSetField,
 )
 from neptune.core.components.operation_storage import OperationStorage
 from neptune.internal.artifacts.types import ArtifactFileData
 from neptune.internal.backends.api_model import (
     ApiExperiment,
-    FloatSeriesValues,
-    ImageSeriesValues,
     Project,
-    StringSeriesValues,
     Workspace,
 )
 from neptune.internal.backends.nql import NQLQuery
 from neptune.internal.container_type import ContainerType
 from neptune.internal.exceptions import NeptuneException
 from neptune.internal.id_formats import (
     QualifiedName,
@@ -253,29 +253,28 @@
 
     @abc.abstractmethod
     def get_string_series_values(
         self,
         container_id: str,
         container_type: ContainerType,
         path: List[str],
-        offset: int,
         limit: int,
-    ) -> StringSeriesValues:
-        pass
+        from_step: Optional[float] = None,
+    ) -> StringSeriesValues: ...
 
     @abc.abstractmethod
     def get_float_series_values(
         self,
         container_id: str,
         container_type: ContainerType,
         path: List[str],
-        offset: int,
         limit: int,
-    ) -> FloatSeriesValues:
-        pass
+        from_step: Optional[float] = None,
+        use_proto: Optional[bool] = None,
+    ) -> FloatSeriesValues: ...
 
     @abc.abstractmethod
     def get_run_url(self, run_id: str, workspace: str, project_name: str, sys_id: str) -> str:
         pass
 
     @abc.abstractmethod
     def get_project_url(self, project_id: str, workspace: str, project_name: str) -> str:
```

### Comparing `neptune-2.0.0a1/src/neptune/internal/backends/neptune_backend_mock.py` & `neptune-2.0.0a2/src/neptune/internal/backends/neptune_backend_mock.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,38 +40,38 @@
     DateTimeField,
     Field,
     FieldDefinition,
     FieldType,
     FileEntry,
     FileField,
     FloatField,
+    FloatPointValue,
     FloatSeriesField,
+    FloatSeriesValues,
+    ImageSeriesValues,
     IntField,
     LeaderboardEntry,
     StringField,
+    StringPointValue,
     StringSeriesField,
+    StringSeriesValues,
     StringSetField,
 )
 from neptune.core.components.operation_storage import OperationStorage
 from neptune.exceptions import (
     ContainerUUIDNotFound,
     MetadataInconsistency,
     ModelVersionNotFound,
     ProjectNotFound,
     RunNotFound,
 )
 from neptune.internal.artifacts.types import ArtifactFileData
 from neptune.internal.backends.api_model import (
     ApiExperiment,
-    FloatPointValue,
-    FloatSeriesValues,
-    ImageSeriesValues,
     Project,
-    StringPointValue,
-    StringSeriesValues,
     Workspace,
 )
 from neptune.internal.backends.hosted_file_operations import get_unique_upload_entries
 from neptune.internal.backends.neptune_backend import NeptuneBackend
 from neptune.internal.backends.nql import NQLQuery
 from neptune.internal.container_structure import ContainerStructure
 from neptune.internal.container_type import ContainerType
@@ -448,35 +448,36 @@
         raise MetadataInconsistency("Attribute {} is not {}".format(str_path, type.__name__))
 
     def get_string_series_values(
         self,
         container_id: str,
         container_type: ContainerType,
         path: List[str],
-        offset: int,
         limit: int,
+        from_step: Optional[float] = None,
     ) -> StringSeriesValues:
         val = self._get_attribute(container_id, container_type, path, StringSeries)
         return StringSeriesValues(
             len(val.values),
-            [StringPointValue(timestampMillis=42342, step=idx, value=v) for idx, v in enumerate(val.values)],
+            [StringPointValue(timestamp=datetime.now(), step=idx, value=v) for idx, v in enumerate(val.values)],
         )
 
     def get_float_series_values(
         self,
         container_id: str,
         container_type: ContainerType,
         path: List[str],
-        offset: int,
         limit: int,
+        from_step: Optional[float] = None,
+        use_proto: Optional[bool] = None,
     ) -> FloatSeriesValues:
         val = self._get_attribute(container_id, container_type, path, FloatSeries)
         return FloatSeriesValues(
             len(val.values),
-            [FloatPointValue(timestampMillis=42342, step=idx, value=v) for idx, v in enumerate(val.values)],
+            [FloatPointValue(timestamp=datetime.now(), step=idx, value=v) for idx, v in enumerate(val.values)],
         )
 
     def get_image_series_values(
         self,
         container_id: str,
         container_type: ContainerType,
         path: List[str],
```

### Comparing `neptune-2.0.0a1/src/neptune/internal/backends/nql.py` & `neptune-2.0.0a2/src/neptune/internal/backends/nql.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/backends/offline_neptune_backend.py` & `neptune-2.0.0a2/src/neptune/internal/backends/offline_neptune_backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,27 +28,25 @@
     DateTimeField,
     Field,
     FieldDefinition,
     FileEntry,
     FileField,
     FloatField,
     FloatSeriesField,
+    FloatSeriesValues,
+    ImageSeriesValues,
     IntField,
     LeaderboardEntry,
     StringField,
     StringSeriesField,
+    StringSeriesValues,
     StringSetField,
 )
 from neptune.exceptions import NeptuneOfflineModeFetchException
 from neptune.internal.artifacts.types import ArtifactFileData
-from neptune.internal.backends.api_model import (
-    FloatSeriesValues,
-    ImageSeriesValues,
-    StringSeriesValues,
-)
 from neptune.internal.backends.neptune_backend_mock import NeptuneBackendMock
 from neptune.internal.backends.nql import NQLQuery
 from neptune.internal.container_type import ContainerType
 from neptune.internal.id_formats import UniqueId
 from neptune.typing import ProgressBarType
 
 
@@ -102,26 +100,27 @@
         raise NeptuneOfflineModeFetchException
 
     def get_string_series_values(
         self,
         container_id: str,
         container_type: ContainerType,
         path: List[str],
-        offset: int,
         limit: int,
+        from_step: Optional[float] = None,
     ) -> StringSeriesValues:
         raise NeptuneOfflineModeFetchException
 
     def get_float_series_values(
         self,
         container_id: str,
         container_type: ContainerType,
         path: List[str],
-        offset: int,
         limit: int,
+        from_step: Optional[float] = None,
+        use_proto: Optional[bool] = None,
     ) -> FloatSeriesValues:
         raise NeptuneOfflineModeFetchException
 
     def get_image_series_values(
         self,
         container_id: str,
         container_type: ContainerType,
```

### Comparing `neptune-2.0.0a1/src/neptune/internal/backends/operation_api_name_visitor.py` & `neptune-2.0.0a2/src/neptune/internal/backends/operation_api_name_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/backends/operation_api_object_converter.py` & `neptune-2.0.0a2/src/neptune/internal/backends/operation_api_object_converter.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/backends/operations_preprocessor.py` & `neptune-2.0.0a2/src/neptune/internal/backends/operations_preprocessor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/backends/project_name_lookup.py` & `neptune-2.0.0a2/src/neptune/internal/backends/project_name_lookup.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/backends/swagger_client_wrapper.py` & `neptune-2.0.0a2/src/neptune/internal/backends/swagger_client_wrapper.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/backends/utils.py` & `neptune-2.0.0a2/src/neptune/internal/backends/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/backgroud_job_list.py` & `neptune-2.0.0a2/src/neptune/internal/backgroud_job_list.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/background_job.py` & `neptune-2.0.0a2/src/neptune/internal/background_job.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/constants.py` & `neptune-2.0.0a2/src/neptune/internal/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/container_structure.py` & `neptune-2.0.0a2/src/neptune/internal/container_structure.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/container_type.py` & `neptune-2.0.0a2/src/neptune/internal/container_type.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/credentials.py` & `neptune-2.0.0a2/src/neptune/internal/credentials.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/envs.py` & `neptune-2.0.0a2/src/neptune/internal/envs.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/exceptions.py` & `neptune-2.0.0a2/src/neptune/internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/extensions.py` & `neptune-2.0.0a2/src/neptune/internal/extensions.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/__init__.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/cgroup/__init__.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/cgroup/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/cgroup/cgroup_filesystem_reader.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/cgroup/cgroup_filesystem_reader.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/cgroup/cgroup_monitor.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/cgroup/cgroup_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/constants.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/constants.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/gauges/__init__.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/gauges/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/gauges/cpu.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/gauges/cpu.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/gauges/gauge.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/gauges/gauge.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/gauges/gauge_factory.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/gauges/gauge_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/gauges/gauge_mode.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/gauges/gauge_mode.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/gauges/gpu.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/gauges/gpu.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/gauges/memory.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/gauges/memory.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/gpu/__init__.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/gpu/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/gpu/gpu_monitor.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/gpu/gpu_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/hardware_metric_reporting_job.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/hardware_metric_reporting_job.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/metrics/__init__.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/metrics/metric.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/metrics/metrics_container.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/metrics/metrics_container.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/metrics/metrics_factory.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/metrics/metrics_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/metrics/reports/__init__.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/metrics/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/metrics/reports/metric_report.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/metrics/reports/metric_report.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/metrics/reports/metric_reporter.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/metrics/reports/metric_reporter.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/metrics/reports/metric_reporter_factory.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/metrics/reports/metric_reporter_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/metrics/service/__init__.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/metrics/service/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/metrics/service/metric_service.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/metrics/service/metric_service.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/metrics/service/metric_service_factory.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/metrics/service/metric_service_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/resources/__init__.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/resources/gpu_card_indices_provider.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/resources/gpu_card_indices_provider.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/resources/system_resource_info.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/resources/system_resource_info.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/resources/system_resource_info_factory.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/resources/system_resource_info_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/system/__init__.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/system/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/hardware/system/system_monitor.py` & `neptune-2.0.0a2/src/neptune/internal/hardware/system/system_monitor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/id_formats.py` & `neptune-2.0.0a2/src/neptune/internal/id_formats.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/init/__init__.py` & `neptune-2.0.0a2/src/neptune/internal/init/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/init/parameters.py` & `neptune-2.0.0a2/src/neptune/internal/init/parameters.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/notebooks/__init__.py` & `neptune-2.0.0a2/src/neptune/internal/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/notebooks/comm.py` & `neptune-2.0.0a2/src/neptune/internal/notebooks/comm.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/notebooks/notebooks.py` & `neptune-2.0.0a2/src/neptune/internal/notebooks/notebooks.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/oauth.py` & `neptune-2.0.0a2/src/neptune/internal/oauth.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/operation.py` & `neptune-2.0.0a2/src/neptune/internal/operation.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/operation_processors/__init__.py` & `neptune-2.0.0a2/src/neptune/internal/operation_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/operation_processors/async_operation_processor.py` & `neptune-2.0.0a2/src/neptune/internal/operation_processors/async_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/operation_processors/factory.py` & `neptune-2.0.0a2/src/neptune/internal/operation_processors/factory.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/operation_processors/lazy_operation_processor_wrapper.py` & `neptune-2.0.0a2/src/neptune/internal/operation_processors/lazy_operation_processor_wrapper.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/operation_processors/offline_operation_processor.py` & `neptune-2.0.0a2/src/neptune/internal/operation_processors/offline_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/operation_processors/operation_logger.py` & `neptune-2.0.0a2/src/neptune/internal/operation_processors/operation_logger.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/operation_processors/operation_processor.py` & `neptune-2.0.0a2/src/neptune/internal/operation_processors/operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/operation_processors/read_only_operation_processor.py` & `neptune-2.0.0a2/src/neptune/internal/operation_processors/read_only_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/operation_processors/sync_operation_processor.py` & `neptune-2.0.0a2/src/neptune/internal/operation_processors/sync_operation_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/operation_processors/utils.py` & `neptune-2.0.0a2/src/neptune/internal/operation_processors/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/operation_visitor.py` & `neptune-2.0.0a2/src/neptune/internal/operation_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/patches/__init__.py` & `neptune-2.0.0a2/src/neptune/internal/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/patches/bravado.py` & `neptune-2.0.0a2/src/neptune/internal/patches/bravado.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/signals_processing/__init__.py` & `neptune-2.0.0a2/src/neptune/internal/signals_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/signals_processing/background_job.py` & `neptune-2.0.0a2/src/neptune/internal/signals_processing/background_job.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/signals_processing/signals.py` & `neptune-2.0.0a2/src/neptune/internal/signals_processing/signals.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/signals_processing/signals_processor.py` & `neptune-2.0.0a2/src/neptune/internal/signals_processing/signals_processor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/signals_processing/utils.py` & `neptune-2.0.0a2/src/neptune/internal/signals_processing/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/state.py` & `neptune-2.0.0a2/src/neptune/internal/state.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/storage/__init__.py` & `neptune-2.0.0a2/src/neptune/internal/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/storage/datastream.py` & `neptune-2.0.0a2/src/neptune/internal/storage/datastream.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/storage/storage_utils.py` & `neptune-2.0.0a2/src/neptune/internal/storage/storage_utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/streams/__init__.py` & `neptune-2.0.0a2/src/neptune/internal/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/streams/std_capture_background_job.py` & `neptune-2.0.0a2/src/neptune/internal/streams/std_capture_background_job.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/streams/std_stream_capture_logger.py` & `neptune-2.0.0a2/src/neptune/internal/streams/std_stream_capture_logger.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/threading/__init__.py` & `neptune-2.0.0a2/src/neptune/internal/threading/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/threading/daemon.py` & `neptune-2.0.0a2/src/neptune/internal/threading/daemon.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/types/__init__.py` & `neptune-2.0.0a2/src/neptune/internal/types/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/types/file_types.py` & `neptune-2.0.0a2/src/neptune/internal/types/file_types.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/types/stringify_value.py` & `neptune-2.0.0a2/src/neptune/internal/types/stringify_value.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/types/utils.py` & `neptune-2.0.0a2/src/neptune/internal/types/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/utils/__init__.py` & `neptune-2.0.0a2/src/neptune/internal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/utils/dependency_tracking.py` & `neptune-2.0.0a2/src/neptune/internal/utils/dependency_tracking.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/utils/deprecation.py` & `neptune-2.0.0a2/src/neptune/internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/utils/disk_utilization.py` & `neptune-2.0.0a2/src/neptune/internal/utils/disk_utilization.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/utils/generic_attribute_mapper.py` & `neptune-2.0.0a2/src/neptune/internal/utils/generic_attribute_mapper.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/utils/git.py` & `neptune-2.0.0a2/src/neptune/internal/utils/git.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/utils/git_info.py` & `neptune-2.0.0a2/src/neptune/internal/utils/git_info.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/utils/hashing.py` & `neptune-2.0.0a2/src/neptune/internal/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/utils/images.py` & `neptune-2.0.0a2/src/neptune/internal/utils/images.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/utils/iso_dates.py` & `neptune-2.0.0a2/src/neptune/internal/utils/iso_dates.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/utils/iteration.py` & `neptune-2.0.0a2/src/neptune/internal/utils/iteration.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/utils/limits.py` & `neptune-2.0.0a2/src/neptune/internal/utils/limits.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/utils/logger.py` & `neptune-2.0.0a2/src/neptune/internal/utils/logger.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/utils/paths.py` & `neptune-2.0.0a2/src/neptune/internal/utils/paths.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/utils/patterns.py` & `neptune-2.0.0a2/src/neptune/internal/utils/patterns.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/utils/ping_background_job.py` & `neptune-2.0.0a2/src/neptune/internal/utils/ping_background_job.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/utils/process_killer.py` & `neptune-2.0.0a2/src/neptune/internal/utils/process_killer.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/utils/requirement_check.py` & `neptune-2.0.0a2/src/neptune/internal/utils/requirement_check.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/utils/run_state.py` & `neptune-2.0.0a2/src/neptune/internal/utils/run_state.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/utils/runningmode.py` & `neptune-2.0.0a2/src/neptune/internal/utils/runningmode.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/utils/s3.py` & `neptune-2.0.0a2/src/neptune/internal/utils/s3.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,26 +13,27 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 __all__ = ["get_boto_s3_client"]
 
 import os
 
-import boto3
-
 from neptune.envs import S3_ENDPOINT_URL
 
 
 def get_boto_s3_client():
     """
     User might want to use other than `AWS` `S3` providers, so we should be able to override `endpoint_url`.
     Unfortunately `boto3` doesn't support this parameter in configuration, so we'll have to create our env variable.
     boto3 supported config envs:
      * https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html#using-environment-variables
     boto3 `endpoint_url` support PR:
      * https://github.com/boto/boto3/pull/2746
     """
     endpoint_url = os.getenv(S3_ENDPOINT_URL)
+
+    import boto3
+
     return boto3.resource(
         service_name="s3",
         endpoint_url=endpoint_url,
     )
```

### Comparing `neptune-2.0.0a1/src/neptune/internal/utils/source_code.py` & `neptune-2.0.0a2/src/neptune/internal/utils/source_code.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/utils/traceback_job.py` & `neptune-2.0.0a2/src/neptune/internal/utils/traceback_job.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/utils/uncaught_exception_handler.py` & `neptune-2.0.0a2/src/neptune/internal/utils/uncaught_exception_handler.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/utils/utils.py` & `neptune-2.0.0a2/src/neptune/internal/utils/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/value_to_attribute_visitor.py` & `neptune-2.0.0a2/src/neptune/internal/value_to_attribute_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/warnings.py` & `neptune-2.0.0a2/src/neptune/internal/warnings.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/websockets/__init__.py` & `neptune-2.0.0a2/src/neptune/internal/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/websockets/reconnecting_websocket.py` & `neptune-2.0.0a2/src/neptune/internal/websockets/reconnecting_websocket.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/websockets/websocket_client_adapter.py` & `neptune-2.0.0a2/src/neptune/internal/websockets/websocket_client_adapter.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/websockets/websocket_signals_background_job.py` & `neptune-2.0.0a2/src/neptune/internal/websockets/websocket_signals_background_job.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/internal/websockets/websockets_factory.py` & `neptune-2.0.0a2/src/neptune/internal/websockets/websockets_factory.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/management/__init__.py` & `neptune-2.0.0a2/src/neptune/management/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/management/exceptions.py` & `neptune-2.0.0a2/src/neptune/management/exceptions.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/management/internal/__init__.py` & `neptune-2.0.0a2/src/neptune/management/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/management/internal/api.py` & `neptune-2.0.0a2/src/neptune/management/internal/api.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/management/internal/dto.py` & `neptune-2.0.0a2/src/neptune/management/internal/dto.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/management/internal/types.py` & `neptune-2.0.0a2/src/neptune/management/internal/types.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/management/internal/utils.py` & `neptune-2.0.0a2/src/neptune/management/internal/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/objects/__init__.py` & `neptune-2.0.0a2/src/neptune/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/objects/abstract.py` & `neptune-2.0.0a2/src/neptune/objects/abstract.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/objects/model.py` & `neptune-2.0.0a2/src/neptune/objects/model.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/objects/model_version.py` & `neptune-2.0.0a2/src/neptune/objects/model_version.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/objects/neptune_object.py` & `neptune-2.0.0a2/src/neptune/objects/neptune_object.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/objects/project.py` & `neptune-2.0.0a2/src/neptune/objects/project.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/objects/run.py` & `neptune-2.0.0a2/src/neptune/objects/run.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/objects/structure_version.py` & `neptune-2.0.0a2/src/neptune/objects/structure_version.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/objects/utils.py` & `neptune-2.0.0a2/src/neptune/objects/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/table.py` & `neptune-2.0.0a2/src/neptune/table.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/types/__init__.py` & `neptune-2.0.0a2/src/neptune/types/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/types/atoms/__init__.py` & `neptune-2.0.0a2/src/neptune/types/atoms/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/types/atoms/artifact.py` & `neptune-2.0.0a2/src/neptune/types/atoms/artifact.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/types/atoms/atom.py` & `neptune-2.0.0a2/src/neptune/types/atoms/atom.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/types/atoms/boolean.py` & `neptune-2.0.0a2/src/neptune/types/atoms/boolean.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/types/atoms/datetime.py` & `neptune-2.0.0a2/src/neptune/types/atoms/datetime.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/types/atoms/file.py` & `neptune-2.0.0a2/src/neptune/types/atoms/file.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/types/atoms/float.py` & `neptune-2.0.0a2/src/neptune/types/atoms/float.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/types/atoms/git_ref.py` & `neptune-2.0.0a2/src/neptune/types/atoms/git_ref.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/types/atoms/integer.py` & `neptune-2.0.0a2/src/neptune/types/atoms/integer.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/types/atoms/string.py` & `neptune-2.0.0a2/src/neptune/types/atoms/string.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/types/file_set.py` & `neptune-2.0.0a2/src/neptune/types/file_set.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/types/mode.py` & `neptune-2.0.0a2/src/neptune/types/mode.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/types/model_version_stage.py` & `neptune-2.0.0a2/src/neptune/types/model_version_stage.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/types/namespace.py` & `neptune-2.0.0a2/src/neptune/types/namespace.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/types/series/__init__.py` & `neptune-2.0.0a2/src/neptune/types/series/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/types/series/file_series.py` & `neptune-2.0.0a2/src/neptune/types/series/file_series.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/types/series/float_series.py` & `neptune-2.0.0a2/src/neptune/types/series/float_series.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/types/series/series.py` & `neptune-2.0.0a2/src/neptune/types/series/series.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/types/series/series_value.py` & `neptune-2.0.0a2/src/neptune/types/series/series_value.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/types/series/string_series.py` & `neptune-2.0.0a2/src/neptune/types/series/string_series.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/types/sets/__init__.py` & `neptune-2.0.0a2/src/neptune/types/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/types/sets/set.py` & `neptune-2.0.0a2/src/neptune/types/sets/set.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/types/sets/string_set.py` & `neptune-2.0.0a2/src/neptune/types/sets/string_set.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/types/type_casting.py` & `neptune-2.0.0a2/src/neptune/types/type_casting.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/types/value.py` & `neptune-2.0.0a2/src/neptune/types/value.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/types/value_copy.py` & `neptune-2.0.0a2/src/neptune/types/value_copy.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/types/value_visitor.py` & `neptune-2.0.0a2/src/neptune/types/value_visitor.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/typing.py` & `neptune-2.0.0a2/src/neptune/typing.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/utils.py` & `neptune-2.0.0a2/src/neptune/utils.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/vendor/lib_programname.py` & `neptune-2.0.0a2/src/neptune/vendor/lib_programname.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/vendor/pynvml.py` & `neptune-2.0.0a2/src/neptune/vendor/pynvml.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/src/neptune/version.py` & `neptune-2.0.0a2/src/neptune/version.py`

 * *Files identical despite different names*

### Comparing `neptune-2.0.0a1/PKG-INFO` & `neptune-2.0.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neptune
-Version: 2.0.0a1
+Version: 2.0.0a2
 Summary: Neptune Client
 Home-page: https://neptune.ai/
 License: Apache-2.0
 Keywords: MLOps,ML Experiment Tracking,ML Model Registry,ML Model Store,ML Metadata Store
 Author: neptune.ai
 Author-email: contact@neptune.ai
 Requires-Python: >=3.7,<4.0
@@ -47,15 +47,14 @@
 Provides-Extra: tensorflow-keras
 Provides-Extra: transformers
 Provides-Extra: xgboost
 Provides-Extra: zenml
 Requires-Dist: GitPython (>=2.0.8)
 Requires-Dist: Pillow (>=1.1.6)
 Requires-Dist: PyJWT
-Requires-Dist: boto3 (>=1.28.0)
 Requires-Dist: bravado (>=11.0.0,<12.0.0)
 Requires-Dist: click (>=7.0)
 Requires-Dist: importlib-metadata ; python_version < "3.8"
 Requires-Dist: kedro-neptune ; (python_version >= "3.9" and python_version < "3.12") and (extra == "kedro")
 Requires-Dist: mosaicml ; extra == "mosaicml"
 Requires-Dist: neptune-airflow ; extra == "airflow"
 Requires-Dist: neptune-aws ; extra == "aws"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: neptune Version: 2.0.0a1 Summary: Neptune Client
+Metadata-Version: 2.1 Name: neptune Version: 2.0.0a2 Summary: Neptune Client
 Home-page: https://neptune.ai/ License: Apache-2.0 Keywords: MLOps,ML
 Experiment Tracking,ML Model Registry,ML Model Store,ML Metadata Store Author:
 neptune.ai Author-email: contact@neptune.ai Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Natural Language :: English Classifier: Operating
@@ -19,29 +19,28 @@
 Extra: aws Provides-Extra: detectron2 Provides-Extra: experimental Provides-
 Extra: fastai Provides-Extra: kedro Provides-Extra: lightgbm Provides-Extra:
 mlflow Provides-Extra: mosaicml Provides-Extra: optuna Provides-Extra: prophet
 Provides-Extra: pytorch Provides-Extra: pytorch-lightning Provides-Extra:
 sacred Provides-Extra: sklearn Provides-Extra: tensorboard Provides-Extra:
 tensorflow-keras Provides-Extra: transformers Provides-Extra: xgboost Provides-
 Extra: zenml Requires-Dist: GitPython (>=2.0.8) Requires-Dist: Pillow (>=1.1.6)
-Requires-Dist: PyJWT Requires-Dist: boto3 (>=1.28.0) Requires-Dist: bravado
-(>=11.0.0,<12.0.0) Requires-Dist: click (>=7.0) Requires-Dist: importlib-
-metadata ; python_version < "3.8" Requires-Dist: kedro-neptune ;
-(python_version >= "3.9" and python_version < "3.12") and (extra == "kedro")
-Requires-Dist: mosaicml ; extra == "mosaicml" Requires-Dist: neptune-airflow ;
-extra == "airflow" Requires-Dist: neptune-aws ; extra == "aws" Requires-Dist:
-neptune-detectron2 ; (python_version >= "3.7") and (extra == "detectron2")
-Requires-Dist: neptune-fastai ; extra == "fastai" Requires-Dist: neptune-
-lightgbm ; extra == "lightgbm" Requires-Dist: neptune-mlflow ; extra ==
-"mlflow" Requires-Dist: neptune-optuna ; extra == "optuna" Requires-Dist:
-neptune-prophet ; extra == "prophet" Requires-Dist: neptune-pytorch ; extra ==
-"pytorch" Requires-Dist: neptune-sacred ; extra == "sacred" Requires-Dist:
-neptune-sklearn ; extra == "sklearn" Requires-Dist: neptune-tensorboard ; extra
-== "tensorboard" Requires-Dist: neptune-tensorflow-keras ; extra ==
-"tensorflow-keras" Requires-Dist: neptune-xgboost ; extra == "xgboost"
+Requires-Dist: PyJWT Requires-Dist: bravado (>=11.0.0,<12.0.0) Requires-Dist:
+click (>=7.0) Requires-Dist: importlib-metadata ; python_version < "3.8"
+Requires-Dist: kedro-neptune ; (python_version >= "3.9" and python_version <
+"3.12") and (extra == "kedro") Requires-Dist: mosaicml ; extra == "mosaicml"
+Requires-Dist: neptune-airflow ; extra == "airflow" Requires-Dist: neptune-aws
+; extra == "aws" Requires-Dist: neptune-detectron2 ; (python_version >= "3.7")
+and (extra == "detectron2") Requires-Dist: neptune-fastai ; extra == "fastai"
+Requires-Dist: neptune-lightgbm ; extra == "lightgbm" Requires-Dist: neptune-
+mlflow ; extra == "mlflow" Requires-Dist: neptune-optuna ; extra == "optuna"
+Requires-Dist: neptune-prophet ; extra == "prophet" Requires-Dist: neptune-
+pytorch ; extra == "pytorch" Requires-Dist: neptune-sacred ; extra == "sacred"
+Requires-Dist: neptune-sklearn ; extra == "sklearn" Requires-Dist: neptune-
+tensorboard ; extra == "tensorboard" Requires-Dist: neptune-tensorflow-keras ;
+extra == "tensorflow-keras" Requires-Dist: neptune-xgboost ; extra == "xgboost"
 Requires-Dist: oauthlib (>=2.1.0) Requires-Dist: packaging Requires-Dist:
 pandas Requires-Dist: protobuf (>=4.0.0,<5.0.0) Requires-Dist: psutil Requires-
 Dist: pytorch-lightning ; extra == "pytorch-lightning" Requires-Dist: requests
 (>=2.20.0) Requires-Dist: requests-oauthlib (>=1.0.0) Requires-Dist: setuptools
 ; python_version >= "3.12" Requires-Dist: swagger-spec-validator (>=2.7.4)
 Requires-Dist: transformers ; extra == "transformers" Requires-Dist: typing-
 extensions (>=3.10.0) Requires-Dist: urllib3 Requires-Dist: websocket-client
```

