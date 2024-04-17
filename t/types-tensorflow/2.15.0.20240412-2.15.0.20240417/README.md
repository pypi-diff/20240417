# Comparing `tmp/types-tensorflow-2.15.0.20240412.tar.gz` & `tmp/types-tensorflow-2.15.0.20240417.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-tensorflow-2.15.0.20240412.tar", last modified: Fri Apr 12 02:19:11 2024, max compression
+gzip compressed data, was "types-tensorflow-2.15.0.20240417.tar", last modified: Wed Apr 17 02:17:36 2024, max compression
```

## Comparing `types-tensorflow-2.15.0.20240412.tar` & `types-tensorflow-2.15.0.20240417.tar`

### file list

```diff
@@ -1,204 +1,204 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.776861 types-tensorflow-2.15.0.20240412/
--rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-04-12 02:19:11.000000 types-tensorflow-2.15.0.20240412/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-12 02:19:11.000000 types-tensorflow-2.15.0.20240412/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-12 02:19:11.776861 types-tensorflow-2.15.0.20240412/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 02:19:11.776861 types-tensorflow-2.15.0.20240412/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-12 02:19:11.000000 types-tensorflow-2.15.0.20240412/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.756861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-12 02:19:11.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)    16625 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/_aliases.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/audio.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/autodiff.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.756861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/autograph/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/autograph/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/autograph/experimental.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/bitwise.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.752861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/compiler/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.756861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/compiler/xla/
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/compiler/xla/autotune_results_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.760861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/compiler/xla/service/
--rw-r--r--   0 runner    (1001) docker     (127)    79109 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/compiler/xla/service/metrics_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    81470 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.760861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/config/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/config/experimental.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.752861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.760861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/example/
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12177 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/example/example_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/example/feature_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.764861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/allocation_description_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12387 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/api_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8125 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/attr_value_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8984 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/cost_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    22002 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/dataset_options_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/dataset_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/device_attributes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    24101 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/full_type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12916 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/function_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10526 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/kernel_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/log_memory_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12531 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7696 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/node_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15145 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/op_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/optimized_function_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/reader_base_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/resource_handle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/step_stats_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12870 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/summary_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/tensor_description_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/tensor_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/types_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/variable_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/versions_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.768861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/bfc_memory_map_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/cluster_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    74211 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8509 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/data_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    26003 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/debug_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    28263 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    27444 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/rpc_options_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    26715 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/saver_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8661 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/service_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    19383 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/struct_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.768861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/tpu/
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    50609 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.768861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/util/
--rw-r--r--   0 runner    (1001) docker     (127)    14861 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/util/event_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/util/test_log_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.768861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/data/
--rw-r--r--   0 runner    (1001) docker     (127)    11419 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/data/experimental.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.768861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/distribute/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/distribute/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.768861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/distribute/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/distribute/experimental/coordinator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/dtypes.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.768861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/experimental/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/experimental/dtensor.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.768861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/feature_column/
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/feature_column/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/initializers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.768861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/io/
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/io/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/io/gfile.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.772861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/activations.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/callbacks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/constraints.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/initializers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.772861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/layers/
--rw-r--r--   0 runner    (1001) docker     (127)    12597 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/layers/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.772861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/layers/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/layers/experimental/preprocessing.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.772861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/layers/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/layers/preprocessing/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/layers/preprocessing/index_lookup.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6289 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/losses.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/metrics.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10576 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/models.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.772861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/optimizers/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.772861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/optimizers/legacy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/optimizers/schedules.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/regularizers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/linalg.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12515 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/math.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/nn.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-12 02:19:11.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.772861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/python/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/python/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.772861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/python/distribute/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/python/distribute/distribute_lib.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.772861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/python/feature_column/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/python/feature_column/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8752 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/python/feature_column/feature_column_v2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.772861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/python/framework/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/python/framework/dtypes.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.772861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/python/keras/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/python/keras/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.772861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/python/keras/protobuf/
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.772861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/python/trackable/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/python/trackable/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/python/trackable/autotrackable.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/python/trackable/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/python/trackable/resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/python/trackable/ressource.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.756861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/python/training/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.772861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/python/training/tracking/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/python/training/tracking/autotrackable.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/random.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/raw_ops.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.772861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/saved_model/
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/saved_model/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/saved_model/experimental.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/sparse.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/strings.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/summary.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.776861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/train/
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/train/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/train/experimental.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.756861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/tsl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.776861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/tsl/protobuf/
--rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/tsl/protobuf/autotuning_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/tsl/protobuf/bfc_memory_map_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/tsl/protobuf/coordination_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    25411 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/tsl/protobuf/coordination_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/tsl/protobuf/distributed_runtime_payloads_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    19832 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/tsl/protobuf/dnn_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12745 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/tsl/protobuf/rpc_options_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    24216 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/tsl/protobuf/test_log_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.776861 types-tensorflow-2.15.0.20240412/tensorflow-stubs/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-12 02:18:54.000000 types-tensorflow-2.15.0.20240412/tensorflow-stubs/types/experimental.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 02:19:11.776861 types-tensorflow-2.15.0.20240412/types_tensorflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-12 02:19:11.000000 types-tensorflow-2.15.0.20240412/types_tensorflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-04-12 02:19:11.000000 types-tensorflow-2.15.0.20240412/types_tensorflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 02:19:11.000000 types-tensorflow-2.15.0.20240412/types_tensorflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-12 02:19:11.000000 types-tensorflow-2.15.0.20240412/types_tensorflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-12 02:19:11.000000 types-tensorflow-2.15.0.20240412/types_tensorflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.405538 types-tensorflow-2.15.0.20240417/
+-rw-r--r--   0 runner    (1001) docker     (127)     8141 2024-04-17 02:17:35.000000 types-tensorflow-2.15.0.20240417/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-17 02:17:35.000000 types-tensorflow-2.15.0.20240417/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-17 02:17:36.405538 types-tensorflow-2.15.0.20240417/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 02:17:36.405538 types-tensorflow-2.15.0.20240417/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-17 02:17:35.000000 types-tensorflow-2.15.0.20240417/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.385538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-17 02:17:35.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    16608 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/_aliases.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/audio.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/autodiff.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.385538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/autograph/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/autograph/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/autograph/experimental.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/bitwise.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.381538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/compiler/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.385538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/compiler/xla/
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/compiler/xla/autotune_results_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.385538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/compiler/xla/service/
+-rw-r--r--   0 runner    (1001) docker     (127)    79109 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/compiler/xla/service/metrics_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    81470 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.385538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/config/experimental.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.381538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.389538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/example/
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12177 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/example/example_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/example/feature_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.393538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/allocation_description_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12387 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/api_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8125 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/attr_value_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8984 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/cost_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    22002 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/dataset_options_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/dataset_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/device_attributes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    24101 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/full_type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12916 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/function_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10526 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/kernel_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/log_memory_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12531 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7696 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/node_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15145 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/op_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/optimized_function_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/reader_base_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/resource_handle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/step_stats_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12870 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/summary_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/tensor_description_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/tensor_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/types_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/variable_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/versions_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.397538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/bfc_memory_map_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/cluster_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    74211 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8509 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/data_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    26003 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7063 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/debug_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    28263 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    27444 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/rpc_options_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    26715 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/saver_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8661 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/service_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    19383 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/struct_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.397538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/tpu/
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    50609 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.397538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/util/
+-rw-r--r--   0 runner    (1001) docker     (127)    14861 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/util/event_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/util/test_log_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.397538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    11419 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/data/experimental.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.397538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/distribute/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/distribute/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.397538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/distribute/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/distribute/experimental/coordinator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/dtypes.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.397538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/experimental/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/experimental/dtensor.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.397538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/feature_column/
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/feature_column/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/initializers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.401538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/io/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/io/gfile.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.401538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/activations.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7526 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/callbacks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/constraints.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/initializers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.401538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)    12597 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/layers/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.401538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/layers/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/layers/experimental/preprocessing.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.401538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/layers/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/layers/preprocessing/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/layers/preprocessing/index_lookup.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6289 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/losses.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/metrics.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10496 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/models.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.401538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/optimizers/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.401538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/optimizers/legacy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/optimizers/schedules.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/regularizers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/linalg.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12515 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/math.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/nn.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 02:17:35.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.401538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.401538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/distribute/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/distribute/distribute_lib.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.401538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/feature_column/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/feature_column/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8752 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/feature_column/feature_column_v2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.401538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/framework/dtypes.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.401538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/keras/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.401538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/keras/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.405538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/trackable/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/trackable/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/trackable/autotrackable.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/trackable/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/trackable/resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/trackable/ressource.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.381538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/training/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.405538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/training/tracking/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/training/tracking/autotrackable.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/random.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/raw_ops.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.405538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/saved_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/saved_model/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/saved_model/experimental.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/sparse.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/strings.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/summary.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.405538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/train/
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/train/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/train/experimental.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.381538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.405538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/autotuning_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/bfc_memory_map_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/coordination_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    25411 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/coordination_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/distributed_runtime_payloads_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    19832 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/dnn_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12745 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/rpc_options_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    24216 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/test_log_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.405538 types-tensorflow-2.15.0.20240417/tensorflow-stubs/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-17 02:16:41.000000 types-tensorflow-2.15.0.20240417/tensorflow-stubs/types/experimental.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:36.405538 types-tensorflow-2.15.0.20240417/types_tensorflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-17 02:17:36.000000 types-tensorflow-2.15.0.20240417/types_tensorflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-04-17 02:17:36.000000 types-tensorflow-2.15.0.20240417/types_tensorflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 02:17:36.000000 types-tensorflow-2.15.0.20240417/types_tensorflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-17 02:17:36.000000 types-tensorflow-2.15.0.20240417/types_tensorflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-17 02:17:36.000000 types-tensorflow-2.15.0.20240417/types_tensorflow.egg-info/top_level.txt
```

### Comparing `types-tensorflow-2.15.0.20240412/CHANGELOG.md` & `types-tensorflow-2.15.0.20240417/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 2.15.0.20240417 (2024-04-17)
+
+Remove remaining bare `Incomplete`s (#11768)
+
+Enable Y065
+
 ## 2.15.0.20240412 (2024-04-12)
 
 Bump flake8-pyi to 24.4.0 (#11745)
 
 ## 2.15.0.20240411 (2024-04-11)
 
 Bump mypy-protobuf in sync_tensorflow script and improve generation scripts (#11740)
```

### Comparing `types-tensorflow-2.15.0.20240412/PKG-INFO` & `types-tensorflow-2.15.0.20240417/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tensorflow
-Version: 2.15.0.20240412
+Version: 2.15.0.20240417
 Summary: Typing stubs for tensorflow
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tensorflow.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -34,10 +34,10 @@
 Partially generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) on tensorflow==2.12.1
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6883b80f5286c7c8d540fa56b4fbf49364719e18` and was tested
+This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
 with mypy 1.9.0, pyright 1.1.358, and
-pytype 2024.3.19.
+pytype 2024.4.11.
```

### Comparing `types-tensorflow-2.15.0.20240412/setup.py` & `types-tensorflow-2.15.0.20240417/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 Partially generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) on tensorflow==2.12.1
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6883b80f5286c7c8d540fa56b4fbf49364719e18` and was tested
+This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
 with mypy 1.9.0, pyright 1.1.358, and
-pytype 2024.3.19.
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="2.15.0.20240412",
+      version="2.15.0.20240417",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tensorflow.md",
```

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/__init__.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -178,23 +178,23 @@
     def __truediv__(self, other: RaggedTensor | float, name: str | None = None) -> RaggedTensor: ...
     def __getitem__(self, slice_spec: Slice | tuple[Slice, ...]) -> RaggedTensor: ...
     def __getattr__(self, name: str) -> Incomplete: ...
 
 class Operation:
     def __init__(
         self,
-        node_def: Incomplete,
+        node_def,
         g: Graph,
         # isinstance is used so can not be Sequence/Iterable.
         inputs: list[Tensor] | None = None,
         output_types: Unused = None,
         control_inputs: Iterable[Tensor | Operation] | None = None,
         input_types: Iterable[DType] | None = None,
         original_op: Operation | None = None,
-        op_def: Incomplete = None,
+        op_def: Incomplete | None = None,
     ) -> None: ...
     @property
     def inputs(self) -> list[Tensor]: ...
     @property
     def outputs(self) -> list[Tensor]: ...
     @property
     def device(self) -> str: ...
@@ -297,15 +297,15 @@
     def experimental_as_proto(self) -> _SpecProto: ...
     @classmethod
     def experimental_from_proto(cls, proto: _SpecProto) -> Self: ...
     @classmethod
     def experimental_type_proto(cls) -> type[_SpecProto]: ...
     def is_compatible_with(self, spec_or_value: Self | TensorCompatible | SparseTensor | RaggedTensor) -> _bool: ...
     # Incomplete as tf.types is not yet covered.
-    def is_subtype_of(self, other: Incomplete) -> _bool: ...
+    def is_subtype_of(self, other) -> _bool: ...
     def most_specific_common_supertype(self, others: Sequence[Incomplete]) -> Self | None: ...
     def most_specific_compatible_type(self, other: Self) -> Self: ...
 
 class TensorSpec(TypeSpec[struct_pb2.TensorSpecProto]):
     def __init__(self, shape: ShapeLike, dtype: DTypeLike = ..., name: str | None = None) -> None: ...
     @property
     def value_type(self) -> Tensor: ...
```

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/_aliases.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/_aliases.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/autodiff.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/autodiff.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/autograph/__init__.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/autograph/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/autograph/experimental.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/autograph/experimental.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/bitwise.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/bitwise.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/compiler/xla/autotune_results_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/compiler/xla/autotune_results_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/compiler/xla/service/metrics_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/compiler/xla/service/metrics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/config/__init__.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/config/experimental.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/config/experimental.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/example/example_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/example/example_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/example/feature_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/example/feature_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/allocation_description_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/allocation_description_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/api_def_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/api_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/attr_value_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/attr_value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/cost_graph_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/cost_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/dataset_options_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/dataset_options_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/dataset_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/dataset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/device_attributes_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/device_attributes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/full_type_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/full_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/function_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/graph_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/kernel_def_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/kernel_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/log_memory_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/log_memory_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/model_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/node_def_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/node_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/op_def_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/op_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/optimized_function_graph_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/optimized_function_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/reader_base_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/reader_base_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/resource_handle_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/resource_handle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/step_stats_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/step_stats_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/summary_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/summary_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/tensor_description_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/tensor_description_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/tensor_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/tensor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/types_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/variable_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/variable_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/framework/versions_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/framework/versions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/cluster_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/cluster_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/config_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/data_service_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/data_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/debug_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/debug_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/saver_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/saver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/service_config_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/service_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/struct_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/struct_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/util/event_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/util/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/core/util/test_log_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/core/util/test_log_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/data/__init__.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/data/experimental.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/data/experimental.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/dtypes.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/dtypes.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/experimental/dtensor.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/experimental/dtensor.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/feature_column/__init__.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/feature_column/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/io/__init__.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/io/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/io/gfile.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/io/gfile.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/activations.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/activations.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/callbacks.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/callbacks.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from _typeshed import Incomplete
 from collections.abc import Callable, Iterable, Mapping, Sequence
 from typing import Any, Literal
 from typing_extensions import TypeAlias
 
 import tensorflow as tf
 from requests.api import _HeadersMapping
 from tensorflow.keras import Model
@@ -144,15 +143,15 @@
         factor: float = 0.1,
         patience: int = 10,
         verbose: Literal[0, 1] = 0,
         mode: Literal["auto", "min", "max"] = "auto",
         min_delta: float = 1e-4,
         cooldown: int = 0,
         min_lr: float = 0,
-        **kwargs: Incomplete,
+        **kwargs,
     ) -> None: ...
     def in_cooldown(self) -> bool: ...
 
 class RemoteMonitor(Callback):
     def __init__(
         self,
         root: str = "http://localhost:9000",
```

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/constraints.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/constraints.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/initializers.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/initializers.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/layers/__init__.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/layers/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/layers/experimental/preprocessing.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/layers/experimental/preprocessing.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/layers/preprocessing/__init__.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/layers/preprocessing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/losses.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/losses.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/metrics.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/metrics.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/models.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/models.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -22,16 +22,16 @@
     optimizer: Optimizer | None
     loss: tf.keras.losses.Loss | dict[str, tf.keras.losses.Loss]
     stop_training: bool
 
     def __new__(cls, *args: Any, **kwargs: Any) -> Model[_InputT, _OutputT]: ...
     def __init__(self, *args: Any, **kwargs: Any) -> None: ...
     def __setattr__(self, name: str, value: Any) -> None: ...
-    def __reduce__(self) -> Incomplete: ...
-    def __deepcopy__(self, memo: Incomplete) -> Incomplete: ...
+    def __reduce__(self): ...
+    def __deepcopy__(self, memo): ...
     def build(self, input_shape: ShapeLike) -> None: ...
     def __call__(self, inputs: _InputT, *, training: bool = False, mask: TensorCompatible | None = None) -> _OutputT: ...
     def call(self, inputs: _InputT, training: bool | None = None, mask: TensorCompatible | None = None) -> _OutputT: ...
     # Ideally loss/metrics/output would share the same structure but higher kinded types are not supported.
     def compile(
         self,
         optimizer: Optimizer | str = "rmsprop",
@@ -57,24 +57,24 @@
     def autotune_steps_per_execution(self) -> bool: ...
     @property
     def steps_per_execution(self) -> int | None: ...  # Returns None for a non-compiled model.
     @property
     def jit_compile(self) -> bool: ...
     @property
     def distribute_reduction_method(self) -> Incomplete | Literal["auto"]: ...
-    def train_step(self, data: TensorCompatible) -> Incomplete: ...
+    def train_step(self, data: TensorCompatible): ...
     def compute_loss(
         self,
         x: TensorCompatible | None = None,
         y: TensorCompatible | None = None,
         y_pred: TensorCompatible | None = None,
         sample_weight: Incomplete | None = None,
     ) -> tf.Tensor | None: ...
     def compute_metrics(
-        self, x: TensorCompatible, y: TensorCompatible, y_pred: TensorCompatible, sample_weight: Incomplete
+        self, x: TensorCompatible, y: TensorCompatible, y_pred: TensorCompatible, sample_weight
     ) -> dict[str, float]: ...
     def get_metrics_result(self) -> dict[str, float]: ...
     def make_train_function(self, force: bool = False) -> Callable[[tf.data.Iterator[Incomplete]], dict[str, float]]: ...
     def fit(
         self,
         x: TensorCompatible | dict[str, TensorCompatible] | tf.data.Dataset[Incomplete] | None = None,
         y: TensorCompatible | dict[str, TensorCompatible] | tf.data.Dataset[Incomplete] | None = None,
@@ -182,15 +182,15 @@
         use_multiprocessing: bool = False,
         verbose: Literal["auto", 0, 1, 2] = 0,
     ) -> _OutputT: ...
     @property
     def trainable_weights(self) -> list[Variable]: ...
     @property
     def non_trainable_weights(self) -> list[Variable]: ...
-    def get_weights(self) -> Incomplete: ...
+    def get_weights(self): ...
     def save(
         self, filepath: str | Path, overwrite: bool = True, save_format: Literal["keras", "tf", "h5"] | None = None, **kwargs: Any
     ) -> None: ...
     def save_weights(
         self,
         filepath: str | Path,
         overwrite: bool = True,
```

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/optimizers/legacy/__init__.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/optimizers/legacy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/optimizers/schedules.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/optimizers/schedules.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/keras/regularizers.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/keras/regularizers.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/linalg.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/linalg.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/math.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/math.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/nn.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/nn.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/python/feature_column/feature_column_v2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/feature_column/feature_column_v2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/random.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/random.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/raw_ops.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/raw_ops.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/saved_model/__init__.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/saved_model/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/saved_model/experimental.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/saved_model/experimental.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from _typeshed import Incomplete
 from enum import Enum
 from typing_extensions import Self
 
 import tensorflow as tf
 from tensorflow._aliases import Integer, TensorValue
 from tensorflow.python.trackable.resource import CapturableResource
 
@@ -20,15 +19,15 @@
         graph_def_program_hash: Integer | None = None,
         signature_def_hash: Integer | None = None,
         saved_object_graph_hash: Integer | None = None,
         checkpoint_hash: Integer | None = None,
         version: Integer | None = None,
     ) -> None: ...
     @classmethod
-    def from_proto(cls, proto: Incomplete) -> Self: ...
+    def from_proto(cls, proto) -> Self: ...
     def singleprint(self) -> str: ...
 
 class TrackableResource(CapturableResource):
     @property
     def resource_handle(self) -> tf.Tensor: ...
     def __init__(self, device: str = "") -> None: ...
```

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/sparse.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/sparse.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/strings.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/strings.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/summary.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/summary.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/train/__init__.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/train/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/tsl/protobuf/autotuning_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/autotuning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/tsl/protobuf/bfc_memory_map_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/bfc_memory_map_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/tsl/protobuf/coordination_config_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/coordination_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/tsl/protobuf/coordination_service_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/coordination_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/tsl/protobuf/distributed_runtime_payloads_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/distributed_runtime_payloads_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/tsl/protobuf/dnn_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/dnn_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/tsl/protobuf/rpc_options_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/rpc_options_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/tsl/protobuf/test_log_pb2.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/tsl/protobuf/test_log_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.15.0.20240412/tensorflow-stubs/types/experimental.pyi` & `types-tensorflow-2.15.0.20240417/tensorflow-stubs/types/experimental.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -20,10 +20,10 @@
     @abc.abstractmethod
     def get_concrete_function(self, *args: _P.args, **kwargs: _P.kwargs) -> ConcreteFunction[_P, _R]: ...
     @overload
     @abc.abstractmethod
     def get_concrete_function(
         self, *args: ContainerGeneric[tf.TypeSpec[Any]], **kwargs: ContainerGeneric[tf.TypeSpec[Any]]
     ) -> ConcreteFunction[_P, _R]: ...
-    def experimental_get_compiler_ir(self, *args: Incomplete, **kwargs: Incomplete) -> Incomplete: ...
+    def experimental_get_compiler_ir(self, *args, **kwargs): ...
 
 def __getattr__(name: str) -> Incomplete: ...
```

### Comparing `types-tensorflow-2.15.0.20240412/types_tensorflow.egg-info/PKG-INFO` & `types-tensorflow-2.15.0.20240417/types_tensorflow.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tensorflow
-Version: 2.15.0.20240412
+Version: 2.15.0.20240417
 Summary: Typing stubs for tensorflow
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tensorflow.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -34,10 +34,10 @@
 Partially generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) on tensorflow==2.12.1
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6883b80f5286c7c8d540fa56b4fbf49364719e18` and was tested
+This package was generated from typeshed commit `7d56cd9a6cf6e0a4ea89c68d0397e197aff32cbe` and was tested
 with mypy 1.9.0, pyright 1.1.358, and
-pytype 2024.3.19.
+pytype 2024.4.11.
```

### Comparing `types-tensorflow-2.15.0.20240412/types_tensorflow.egg-info/SOURCES.txt` & `types-tensorflow-2.15.0.20240417/types_tensorflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

