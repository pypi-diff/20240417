# Comparing `tmp/protobuf_to_pydantic-0.2.6.1.tar.gz` & `tmp/protobuf_to_pydantic-0.2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protobuf_to_pydantic-0.2.6.1.tar", max compression
+gzip compressed data, was "protobuf_to_pydantic-0.2.6.2.tar", max compression
```

## Comparing `protobuf_to_pydantic-0.2.6.1.tar` & `protobuf_to_pydantic-0.2.6.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0    11357 2021-12-05 05:37:05.000000 protobuf_to_pydantic-0.2.6.1/LICENSE
--rw-r--r--   0        0        0    53105 2024-04-12 16:29:25.422060 protobuf_to_pydantic-0.2.6.1/README.md
--rw-r--r--   0        0        0      157 2023-07-25 07:16:59.663544 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/__init__.py
--rw-r--r--   0        0        0       25 2024-04-12 16:30:50.520666 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/__version__.py
--rw-r--r--   0        0        0     3600 2023-08-14 14:18:09.829408 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/_pydantic_adapter.py
--rw-r--r--   0        0        0     1915 2024-03-18 17:01:38.809044 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/constant.py
--rw-r--r--   0        0        0        0 2022-06-28 03:26:29.000000 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/contrib/__init__.py
--rw-r--r--   0        0        0    15428 2023-09-11 08:36:58.424118 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/contrib/proto_parser.py
--rw-r--r--   0        0        0      134 2023-08-14 14:18:09.829408 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/customer_con_type/__init__.py
--rw-r--r--   0        0        0     7954 2023-08-14 14:18:09.829408 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/customer_con_type/v1.py
--rw-r--r--   0        0        0    14102 2023-12-26 05:38:18.658043 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/customer_con_type/v2.py
--rw-r--r--   0        0        0      177 2023-08-14 14:18:09.829408 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/customer_validator/__init__.py
--rw-r--r--   0        0        0     9782 2024-02-28 17:06:54.586662 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/customer_validator/rule.py
--rw-r--r--   0        0        0     8204 2024-02-28 17:06:54.586662 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/customer_validator/v1.py
--rw-r--r--   0        0        0     9648 2024-02-28 17:06:54.586662 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/customer_validator/v2.py
--rw-r--r--   0        0        0     2579 2023-09-14 10:22:59.213024 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/desc_template/__init__.py
--rw-r--r--   0        0        0    35019 2024-03-29 06:52:18.350469 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/gen_code.py
--rw-r--r--   0        0        0    35234 2024-03-18 17:01:38.809044 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/gen_model.py
--rw-r--r--   0        0        0      169 2022-07-26 07:13:09.000000 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/get_desc/__init__.py
--rw-r--r--   0        0        0      134 2022-07-26 07:13:09.000000 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/get_desc/from_pb_option/__init__.py
--rw-r--r--   0        0        0    20179 2024-02-28 17:06:54.586662 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/get_desc/from_pb_option/base.py
--rw-r--r--   0        0        0      479 2023-02-21 11:07:15.262565 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/get_desc/from_pb_option/from_p2p.py
--rw-r--r--   0        0        0      356 2023-02-21 11:07:15.326564 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/get_desc/from_pb_option/from_pgv.py
--rw-r--r--   0        0        0     4349 2023-12-26 05:38:18.658043 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/get_desc/from_pb_option/types.py
--rw-r--r--   0        0        0     3663 2023-03-31 07:16:34.356473 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/get_desc/from_proto_file.py
--rw-r--r--   0        0        0     5626 2023-02-23 06:43:54.137679 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/get_desc/from_pyi_file.py
--rw-r--r--   0        0        0     7514 2024-03-18 17:01:38.809044 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/grpc_types.py
--rw-r--r--   0        0        0        0 2022-12-04 12:28:50.000000 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/plugin/__init__.py
--rw-r--r--   0        0        0       31 2022-12-28 10:00:32.000000 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/plugin/__main__.py
--rw-r--r--   0        0        0     2655 2023-11-07 15:24:27.394042 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/plugin/cli.py
--rw-r--r--   0        0        0     6402 2023-11-07 16:10:23.558322 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/plugin/code_gen.py
--rw-r--r--   0        0        0     2841 2023-11-07 15:24:27.394042 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/plugin/config.py
--rw-r--r--   0        0        0    29201 2024-03-29 07:16:25.193672 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/plugin/field_desc_proto_to_code.py
--rwxr-xr-x   0        0        0      413 2023-11-07 15:24:27.394042 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/plugin/main.py
--rw-r--r--   0        0        0      423 2024-03-18 17:01:38.809044 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/plugin/my_types.py
--rw-r--r--   0        0        0   414477 2024-04-12 08:25:47.566089 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.py
--rw-r--r--   0        0        0   198324 2024-04-12 08:25:47.566089 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.pyi
--rw-r--r--   0        0        0      158 2023-10-19 17:28:47.711467 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2_grpc.py
--rw-r--r--   0        0        0      169 2023-10-19 17:17:13.384141 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2_grpc.pyi
--rw-r--r--   0        0        0   121461 2024-04-12 08:25:47.566089 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/old/protos/validate_pb2.py
--rw-r--r--   0        0        0    64630 2024-04-12 08:25:47.566089 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/old/protos/validate_pb2.pyi
--rw-r--r--   0        0        0      158 2023-10-19 17:28:47.723467 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/old/protos/validate_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-10-19 17:17:13.384141 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/old/protos/validate_pb2_grpc.pyi
--rw-r--r--   0        0        0      270 2023-04-01 17:49:33.439309 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/p2p_validate_pb2.py
--rw-r--r--   0        0        0    36680 2024-04-12 16:29:25.426060 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.py
--rw-r--r--   0        0        0   198324 2024-04-12 08:25:53.378232 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.pyi
--rw-r--r--   0        0        0      158 2023-10-19 17:28:47.695466 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/protos/p2p_validate_pb2_grpc.py
--rw-r--r--   0        0        0      169 2023-10-19 17:17:44.003669 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/protos/p2p_validate_pb2_grpc.pyi
--rw-r--r--   0        0        0    13083 2024-04-12 16:29:25.426060 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/protos/validate_pb2.py
--rw-r--r--   0        0        0    64630 2024-04-12 08:25:53.378232 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/protos/validate_pb2.pyi
--rw-r--r--   0        0        0      158 2023-10-19 17:28:47.695466 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/protos/validate_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-10-19 17:17:44.003669 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/protos/validate_pb2_grpc.pyi
--rw-r--r--   0        0        0      262 2023-04-01 17:20:07.469049 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/validate_pb2.py
--rw-r--r--   0        0        0     2683 2023-12-26 05:38:18.658043 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/types.py
--rw-r--r--   0        0        0     7158 2024-03-18 17:01:38.809044 protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/util.py
--rw-r--r--   0        0        0     3631 2024-04-12 16:30:50.516667 protobuf_to_pydantic-0.2.6.1/pyproject.toml
--rw-r--r--   0        0        0    55696 1970-01-01 00:00:00.000000 protobuf_to_pydantic-0.2.6.1/setup.py
--rw-r--r--   0        0        0    54355 1970-01-01 00:00:00.000000 protobuf_to_pydantic-0.2.6.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2021-12-05 05:37:05.000000 protobuf_to_pydantic-0.2.6.2/LICENSE
+-rw-r--r--   0        0        0    53105 2024-04-12 16:29:25.422060 protobuf_to_pydantic-0.2.6.2/README.md
+-rw-r--r--   0        0        0      157 2023-07-25 07:16:59.663544 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/__init__.py
+-rw-r--r--   0        0        0       25 2024-04-17 16:04:24.778587 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/__version__.py
+-rw-r--r--   0        0        0     3600 2023-08-14 14:18:09.829408 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/_pydantic_adapter.py
+-rw-r--r--   0        0        0     1806 2024-04-17 16:03:57.030208 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/constant.py
+-rw-r--r--   0        0        0        0 2022-06-28 03:26:29.000000 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/contrib/__init__.py
+-rw-r--r--   0        0        0    15428 2023-09-11 08:36:58.424118 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/contrib/proto_parser.py
+-rw-r--r--   0        0        0      134 2023-08-14 14:18:09.829408 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/customer_con_type/__init__.py
+-rw-r--r--   0        0        0     7954 2023-08-14 14:18:09.829408 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/customer_con_type/v1.py
+-rw-r--r--   0        0        0    14102 2023-12-26 05:38:18.658043 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/customer_con_type/v2.py
+-rw-r--r--   0        0        0      177 2023-08-14 14:18:09.829408 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/customer_validator/__init__.py
+-rw-r--r--   0        0        0     9782 2024-02-28 17:06:54.586662 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/customer_validator/rule.py
+-rw-r--r--   0        0        0     8204 2024-02-28 17:06:54.586662 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/customer_validator/v1.py
+-rw-r--r--   0        0        0     9648 2024-02-28 17:06:54.586662 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/customer_validator/v2.py
+-rw-r--r--   0        0        0     2579 2023-09-14 10:22:59.213024 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/desc_template/__init__.py
+-rw-r--r--   0        0        0    35019 2024-03-29 06:52:18.350469 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/gen_code.py
+-rw-r--r--   0        0        0    35857 2024-04-17 16:03:57.030208 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/gen_model.py
+-rw-r--r--   0        0        0      169 2022-07-26 07:13:09.000000 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/get_desc/__init__.py
+-rw-r--r--   0        0        0      134 2022-07-26 07:13:09.000000 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/get_desc/from_pb_option/__init__.py
+-rw-r--r--   0        0        0    20179 2024-02-28 17:06:54.586662 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/get_desc/from_pb_option/base.py
+-rw-r--r--   0        0        0      479 2023-02-21 11:07:15.262565 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/get_desc/from_pb_option/from_p2p.py
+-rw-r--r--   0        0        0      356 2023-02-21 11:07:15.326564 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/get_desc/from_pb_option/from_pgv.py
+-rw-r--r--   0        0        0     4349 2023-12-26 05:38:18.658043 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/get_desc/from_pb_option/types.py
+-rw-r--r--   0        0        0     3663 2023-03-31 07:16:34.356473 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/get_desc/from_proto_file.py
+-rw-r--r--   0        0        0     5626 2023-02-23 06:43:54.137679 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/get_desc/from_pyi_file.py
+-rw-r--r--   0        0        0     7514 2024-03-18 17:01:38.809044 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/grpc_types.py
+-rw-r--r--   0        0        0        0 2022-12-04 12:28:50.000000 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/plugin/__init__.py
+-rw-r--r--   0        0        0       31 2022-12-28 10:00:32.000000 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/plugin/__main__.py
+-rw-r--r--   0        0        0     2655 2023-11-07 15:24:27.394042 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/plugin/cli.py
+-rw-r--r--   0        0        0     6402 2023-11-07 16:10:23.558322 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/plugin/code_gen.py
+-rw-r--r--   0        0        0     4223 2024-04-17 16:03:57.030208 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/plugin/config.py
+-rw-r--r--   0        0        0    30923 2024-04-17 16:03:57.030208 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/plugin/field_desc_proto_to_code.py
+-rwxr-xr-x   0        0        0      413 2023-11-07 15:24:27.394042 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/plugin/main.py
+-rw-r--r--   0        0        0      423 2024-03-18 17:01:38.809044 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/plugin/my_types.py
+-rw-r--r--   0        0        0   414477 2024-04-17 09:53:56.325615 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.py
+-rw-r--r--   0        0        0   198324 2024-04-17 09:53:56.325615 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-10-19 17:28:47.711467 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2_grpc.py
+-rw-r--r--   0        0        0      169 2023-10-19 17:17:13.384141 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2_grpc.pyi
+-rw-r--r--   0        0        0   121461 2024-04-17 09:53:56.325615 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/protos/old/protos/validate_pb2.py
+-rw-r--r--   0        0        0    64630 2024-04-17 09:53:56.325615 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/protos/old/protos/validate_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-10-19 17:28:47.723467 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/protos/old/protos/validate_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-10-19 17:17:13.384141 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/protos/old/protos/validate_pb2_grpc.pyi
+-rw-r--r--   0        0        0      270 2023-04-01 17:49:33.439309 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/protos/p2p_validate_pb2.py
+-rw-r--r--   0        0        0    36680 2024-04-17 09:54:01.297725 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.py
+-rw-r--r--   0        0        0   198324 2024-04-17 09:54:01.297725 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-10-19 17:28:47.695466 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/protos/protos/p2p_validate_pb2_grpc.py
+-rw-r--r--   0        0        0      169 2023-10-19 17:17:44.003669 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/protos/protos/p2p_validate_pb2_grpc.pyi
+-rw-r--r--   0        0        0    13083 2024-04-17 09:54:01.297725 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/protos/protos/validate_pb2.py
+-rw-r--r--   0        0        0    64630 2024-04-17 09:54:01.297725 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/protos/protos/validate_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-10-19 17:28:47.695466 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/protos/protos/validate_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-10-19 17:17:44.003669 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/protos/protos/validate_pb2_grpc.pyi
+-rw-r--r--   0        0        0      262 2023-04-01 17:20:07.469049 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/protos/validate_pb2.py
+-rw-r--r--   0        0        0     2683 2023-12-26 05:38:18.658043 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/types.py
+-rw-r--r--   0        0        0     7158 2024-03-18 17:01:38.809044 protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/util.py
+-rw-r--r--   0        0        0     3631 2024-04-17 16:04:24.774587 protobuf_to_pydantic-0.2.6.2/pyproject.toml
+-rw-r--r--   0        0        0    55696 1970-01-01 00:00:00.000000 protobuf_to_pydantic-0.2.6.2/setup.py
+-rw-r--r--   0        0        0    54355 1970-01-01 00:00:00.000000 protobuf_to_pydantic-0.2.6.2/PKG-INFO
```

### Comparing `protobuf_to_pydantic-0.2.6.1/LICENSE` & `protobuf_to_pydantic-0.2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6.1/README.md` & `protobuf_to_pydantic-0.2.6.2/README.md`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/_pydantic_adapter.py` & `protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/_pydantic_adapter.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/constant.py` & `protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/constant.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import datetime
 from typing import Any, Dict, Type
 
 from google.protobuf.any_pb2 import Any as AnyMessage
 from google.protobuf.descriptor import FieldDescriptor
-from google.protobuf.field_mask_pb2 import FieldMask
 
 from protobuf_to_pydantic import _pydantic_adapter
 from protobuf_to_pydantic.util import Timedelta
 
 message_name_default_factory_dict: Dict[str, Any] = {
     "Timestamp": datetime.datetime.now,
     "Struct": dict,
     "Duration": Timedelta,
     "Any": AnyMessage,
-    "FieldMask": FieldMask,
 }
 pydantic_field_v1_migration_v2_dict = {
     "min_items": "min_length",
     "max_items": "max_length",
     "allow_mutation": "frozen",
     "regex": "pattern",
     "const": None,
@@ -25,15 +23,14 @@
 }
 message_name_type_dict: Dict[str, Any] = {
     "Timestamp": datetime.datetime,
     "Struct": Dict[str, Any],
     "Empty": Any,
     "Duration": Timedelta,
     "Any": AnyMessage,
-    "FieldMask": FieldMask,
 }
 
 if not _pydantic_adapter.is_v1:
     from pydantic import BeforeValidator
     from typing_extensions import Annotated
 
     message_name_type_dict["Duration"] = Annotated[datetime.timedelta, BeforeValidator(Timedelta.validate)]
```

### Comparing `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/contrib/proto_parser.py` & `protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/contrib/proto_parser.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/customer_con_type/v1.py` & `protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/customer_con_type/v1.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/customer_con_type/v2.py` & `protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/customer_con_type/v2.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/customer_validator/rule.py` & `protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/customer_validator/rule.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/customer_validator/v1.py` & `protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/customer_validator/v1.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/customer_validator/v2.py` & `protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/customer_validator/v2.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/desc_template/__init__.py` & `protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/desc_template/__init__.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/gen_code.py` & `protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/gen_code.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/gen_model.py` & `protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/gen_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import dataclasses
 import datetime
+import importlib
 import inspect
 import warnings
 from dataclasses import MISSING
 from enum import IntEnum
 from pathlib import Path
 from types import ModuleType
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Set, Tuple, Type, Union
@@ -330,15 +331,19 @@
     def model(self) -> Type[BaseModel]:
         return self._gen_model
 
     ###############
     # util method #
     ###############
     def _get_field_info_dict_by_full_name(self, full_name: str) -> Optional["FieldInfoTypedDict"]:
-        message_name, *key_list = full_name.split(".")[1:]  # ignore package name
+        split_full_name = full_name.split(".")
+        if len(split_full_name) == 2:
+            message_name, *key_list = split_full_name
+        else:
+            message_name, *key_list = split_full_name[1:]  # ignore package name
         if message_name not in self._field_doc_dict:
             return None
         desc_dict: "DescFromOptionTypedDict" = self._field_doc_dict[message_name]
 
         for key in key_list:
             if key in desc_dict["message"]:
                 return desc_dict["message"][key]
@@ -449,14 +454,20 @@
                     k_v_type = self._message_type_dict_by_type_name[k_v_field.message_type.name]
                 else:
                     k_v_type = self._parse_msg_to_pydantic_model(descriptor=k_v_field.message_type)
                 dict_type_param_list.append(k_v_type)
 
             field_dataclass.field_type = Dict[tuple(dict_type_param_list)]  # type: ignore
             field_dataclass.field_default_factory = dict
+        elif protobuf_field.message_type.file.name.startswith("google/protobuf/"):
+            module_name = protobuf_field.message_type.file.name.split(".")[0].replace("/", ".") + "_pb2"
+            message_name = protobuf_field.message_type.name
+            type_factory = getattr(importlib.import_module(module_name), message_name)
+            field_dataclass.field_type = type_factory
+            field_dataclass.field_default_factory = type_factory
         else:
             # support google.protobuf.Message
             if protobuf_field.message_type.full_name in field_dataclass.nested_message_dict:
                 field_dataclass.field_type = field_dataclass.nested_message_dict[protobuf_field.message_type.full_name]
             else:
                 # Python Protobuf does not solve the namespace problem of modules,
                 # so there is no uniform cross-module reference
```

### Comparing `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/get_desc/from_pb_option/base.py` & `protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/get_desc/from_pb_option/base.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/get_desc/from_pb_option/types.py` & `protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/get_desc/from_pb_option/types.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/get_desc/from_proto_file.py` & `protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/get_desc/from_proto_file.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/get_desc/from_pyi_file.py` & `protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/get_desc/from_pyi_file.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/grpc_types.py` & `protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/grpc_types.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/plugin/cli.py` & `protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/plugin/cli.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/plugin/code_gen.py` & `protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/plugin/code_gen.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/plugin/config.py` & `protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/plugin/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 from collections import deque
-from typing import Any, Deque, List, Set, Type, TypeVar
+from typing import Any, Deque, Dict, List, Set, Type, TypeVar
 
 from pydantic import BaseModel, Field
 
 from protobuf_to_pydantic import _pydantic_adapter
 from protobuf_to_pydantic.desc_template import DescTemplate
 from protobuf_to_pydantic.plugin.field_desc_proto_to_code import FileDescriptorProtoToCode
 
 ConfigT = TypeVar("ConfigT", bound="ConfigModel")
 
 
+class ProtobufTypeConfigModel(BaseModel):
+    module_name: str = Field(description="Python module name")
+    message_name: str = Field(description="Python message name")
+    is_custom: bool = Field(
+        default=False,
+        description="Whether it is a custom message, if true, model config arbitrary_types_allowed = True",
+    )
+
+
 class ConfigModel(BaseModel):
     local_dict: dict = Field(default_factory=dict, description="Dict for local variables")
     desc_template: Type[DescTemplate] = Field(
         default=DescTemplate, description="Support more templates by customizing 'Desc Template'"
     )
     comment_prefix: str = Field(default="p2p", description="Comment prefix")
     customer_import_set: Set[str] = Field(default_factory=set, description="customer import code set")
@@ -32,15 +41,44 @@
         default="_p2p",
         description=(
             "The file name suffix, but not the file type. "
             "For example, if the name of the proto file is `book`, the generated file name is `book_p2p.py`"
         ),
     )
     file_descriptor_proto_to_code: Type[FileDescriptorProtoToCode] = Field(default=FileDescriptorProtoToCode)
-
+    protobuf_type_config: Dict[str, ProtobufTypeConfigModel] = Field(
+        default_factory=dict,
+        description="""
+        Fixed the issue that some protobuf message names are inconsistent with Python module names
+
+        use template: {"{protobuf message name}": ("{python module name}", "{python message name}")}
+
+        The configuration of the protobuf type, for example protobuf:
+        ```protobuf
+        syntax = "proto3";
+
+        import "google/protobuf/wrappers.proto";
+
+        message CalculatedValue {
+            google.protobuf.DoubleValue myValue = 1;
+        }
+        ```
+        In order for `protobuf_to_pydantic` to find google.protobuf.DoubleValue module - google/protobuf/wrappers.proto,
+        need to enter the configuration information:
+        ```Python
+        {
+            "google.protobuf.DoubleValue": ProtobufTypeConfigModel(
+                module_name="builtins",
+                message_name="float",
+                is_custom=False
+            ),
+        }
+        ```
+        """,
+    )
     desc_template_instance: DescTemplate = Field(
         default_factory=lambda: DescTemplate({}, ""),
         description="This variable does not support configuration and will be overwritten even if configured",
     )
 
     class Config:
         arbitrary_types_allowed = True
```

### Comparing `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/plugin/field_desc_proto_to_code.py` & `protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/plugin/field_desc_proto_to_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -552,27 +552,48 @@
         )
         if not any([class_head_content, class_field_content]):
             content += " " * (indent + self.code_indent) + "pass\n"
         self._parse_desc_name_dict[class_name] = content
         return content
 
     def _get_protobuf_type_model(self, field: FieldDescriptorProto) -> ProtobufTypeModel:
+        def _get_type_factory(module_name: str, message_name: str) -> Any:
+            try:
+                return getattr(importlib.import_module(module_name), message_name)
+            except ModuleNotFoundError:
+                details = {"field name": field.name, "field type name": field.type_name[1:], "field type": field.type}
+                raise ModuleNotFoundError(
+                    "Can't find protobuf type module, "
+                    "please check that config.protobuf_type_config is configured correctly!"
+                    f"  details info: {details}"
+                )
+
         type_factory: Optional[Any] = None
         use_custom_type = False
         # TODO use gen_model.py _message_default_factory_dict_by_type_name
         if field.type in protobuf_desc_python_type_dict:
             type_factory = protobuf_desc_python_type_dict[field.type]
             return ProtobufTypeModel(
                 type_factory=type_factory,
                 py_type_str=self._get_value_code(type_factory),
                 rule_type_str=protobuf_common_type_dict.get(field.type, ""),
             )
         elif field.type_name.startswith(".google.protobuf"):
             _type_str = field.type_name.split(".")[-1]
-            if _type_str == "Empty":
+            protobuf_type_config_key = field.type_name[1:]
+            if protobuf_type_config_key in self.config.protobuf_type_config:
+                # Through configuration, users can define the type of Protobuf they want
+                rule_type_str = "any"
+                use_custom_type = self.config.protobuf_type_config[protobuf_type_config_key].is_custom
+                type_module_name = self.config.protobuf_type_config[protobuf_type_config_key].module_name
+                _type_str = self.config.protobuf_type_config[protobuf_type_config_key].message_name
+                py_type_str = _type_str  # rewrite py_type_str
+                type_factory = _get_type_factory(type_module_name, _type_str)
+                self._add_import_code(type_module_name, _type_str)
+            elif _type_str == "Empty":
                 py_type_str = "None"
                 rule_type_str = ""
             elif _type_str == "Timestamp":
                 py_type_str = "datetime"
                 rule_type_str = "timestamp"
                 type_factory = datetime.now
                 self._add_import_code("datetime", "datetime")
@@ -603,16 +624,22 @@
                 rule_type_str = "struct"
                 type_factory = dict
             elif field.type_name.startswith(".google.protobuf"):
                 py_type_str = _type_str
                 rule_type_str = "any"
                 use_custom_type = True
 
-                type_module_name = "google.protobuf." + camel_to_snake(_type_str) + "_pb2"
-                type_factory = getattr(importlib.import_module(type_module_name), _type_str)
+                if field.type_name in self._descriptors.message_to_fd:
+                    message_fd = self._descriptors.message_to_fd[field.type_name]
+                    # google/protobuf/wrappers.proto -> google.protobuf.wrappers_pb2
+                    type_module_name = message_fd.name.split(".")[0].replace("/", ".") + "_pb2"
+                else:
+                    type_module_name = "google.protobuf." + camel_to_snake(_type_str) + "_pb2"
+
+                type_factory = _get_type_factory(type_module_name, _type_str)
                 self._add_import_code(type_module_name, _type_str)
             else:
                 logger.error(f"Not support type {field.type_name}")
                 py_type_str = "Any"
                 rule_type_str = "any"
                 use_custom_type = True
                 type_factory = AnyMessage
```

### Comparing `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.py` & `protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.pyi` & `protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/protos/old/protos/p2p_validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/old/protos/validate_pb2.py` & `protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/protos/old/protos/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/old/protos/validate_pb2.pyi` & `protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/protos/old/protos/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.py` & `protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.pyi` & `protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/protos/protos/p2p_validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/protos/validate_pb2.py` & `protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/protos/protos/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/protos/protos/validate_pb2.pyi` & `protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/protos/protos/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/types.py` & `protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/types.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6.1/protobuf_to_pydantic/util.py` & `protobuf_to_pydantic-0.2.6.2/protobuf_to_pydantic/util.py`

 * *Files identical despite different names*

### Comparing `protobuf_to_pydantic-0.2.6.1/pyproject.toml` & `protobuf_to_pydantic-0.2.6.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "protobuf_to_pydantic"
-version = "v0.2.6.1"
+version = "v0.2.6.2"
 description = "Generate the `pydantic.BaseModel` class (and the corresponding source code) with parameter verification function through the Protobuf file"
 authors = ["So1n <so1n897046026@gmail.com>"]
 license = "Apache Software License"
 readme = "./README.md"
 repository = "https://github.com/so1n/protobuf_to_pydantic"
 homepage = "https://github.com/so1n/protobuf_to_pydantic"
 packages = [
```

### Comparing `protobuf_to_pydantic-0.2.6.1/setup.py` & `protobuf_to_pydantic-0.2.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 entry_points = \
 {'console_scripts': ['protoc-gen-protobuf-to-pydantic = '
                      'protobuf_to_pydantic.plugin.main:main']}
 
 setup_kwargs = {
     'name': 'protobuf-to-pydantic',
-    'version': '0.2.6.1',
+    'version': '0.2.6.2',
     'description': 'Generate the `pydantic.BaseModel` class (and the corresponding source code) with parameter verification function through the Protobuf file',
     'long_description': '# protobuf_to_pydantic\nGenerate Pydantic Model or source code with parameter verification function based on Protobuf file (Proto3).\n\n\n[中文文档](https://github.com/so1n/protobuf_to_pydantic/blob/master/README_ZH.md)\n\n# Feature\n\nFeature：\n- [x] Generate source code through `Protobuf` plugin。\n- [x] Generate `Pydantic Model` or source code by parsing `Protobuf Message` in `Python` runtime.\n- [x] Compatible with `V1` and `V2` versions of `Pydantic`。\n- [x] Supports multiple verification rules and is compatible with `proto-gen-validate` (subsequent versions will support the rules of `proto-gen-validate` 1.0)。\n- [x] Support custom functionality through templates。\n- [ ] Supports `protovalidate` verification rules（`proto-gen-validate` version >= 1.0）\n\nThe following is a functional overview diagram of `protobuf-to-pydantic`.\nIn the picture `P2P` represents `protobuf-to-pydantic`, `Protoc` represents the command for `Protobuf` to generate code, and `plugin` represents ` Plugin for Protoc`:\n![protobuf-to-pydantic](https://github.com/so1n/protobuf_to_pydantic/blob/master/images/protobuf-to-pydantic_index.png?raw=true)\n\n# Installation\nBy default, `protobuf-to-pydantic` can be installed directly via the following command:\n```bash\npip install protobuf_to_pydantic\n```\nIf want to use the full functionality of `protobuf-to-pydantic`, can install `protobuf-to-pydantic` with the following command:.\n```bash\npip install protobuf_to_pydantic[all]\n```\n# Usage\n## 1.code generation\n`protobuf-to-pydantic` currently has two methods to generate `Pydantic Model` objects based on Protobuf files.：\n- 1: Use the `Protoc` plug-in to generate the corresponding `Python` code file through the Protobuf file。\n- 2: Generate the corresponding `Pydantic Model` object through the `Message` object in `Python` runtime。\n\n### 1.1.Directly generate `Pydantic Model` code files through plug-ins\n#### 1.1.0.Install dependencies\nThe `protobuf-to-pydantic` plug-in depends on `mypy-protobuf`, need to install `mypy-protobuf` through the following command first:\n```bash\npython -m pip install protobuf-to-pydantic[mypy-protobuf]\n```\nor\n```bash\npoetry add protobuf-to-pydantic -E mypy-protobuf\n```\n#### 1.1.1.Use plugins\nPlug-in is the `Pydantic Model` source code generation method recommended by `protobuf-to-pydantic`.\nIt supports the most complete functions and is also very simple to use.\n\nAssume that it is usually generated through the following command Code corresponding to Protobuf file:\n```bash\npython -m grpc_tools.protoc -I. example.proto\n# or\nprotoc -I. --python_out=. example.proto\n```\nAfter installing `protobuf-to-pydantic`,can use the `protobuf-to-pydantic` plugin with the `--protobuf-to-pydantic_out` option with the following command:\n```bash\npython -m grpc_tools.protoc -I. --protobuf-to-pydantic_out=. example.proto\n# or\nprotoc -I. --protobuf-to-pydantic_out=. example.proto\n```\n\nIn this command, `--protobuf-to-pydantic_out=.` means using the `prorobuf-to-pydantic` plug-in,\nAnd it is declared that the output location of the `protobuf-to-pydantic` plug-in is `.`\n\n> `.` indicates the output path used by `grpc_tools.proto`.\n\nAfter running the command, the `protobuf-to-pydantic` plugin writes the generated source code to a file with the filename suffix `p2p.py`, e.g., `example.proto` generates a file with the name `example_p2p.py`.\n\n\n#### 1.1.2.Plug-in configuration\nThe `protobuf-to-pydantic` plugin supports loading configuration by reading a `Python` file。\n\n> In order to ensure that the variables of the configuration file can be introduced normally, the configuration file must be stored in the current path of the running command.。\n\nAn example configuration that can be read by `protobuf-to-pydantic` is as follows:\n```Python\nimport logging\nfrom typing import List, Type\n\nfrom google.protobuf.any_pb2 import Any  # type: ignore\nfrom pydantic import confloat, conint\nfrom pydantic.fields import FieldInfo\n\nfrom protobuf_to_pydantic.desc_template import DescTemplate\n\n# Configure the log output format and log level of the plugin, which is very useful when debugging\nlogging.basicConfig(format="[%(asctime)s %(levelname)s] %(message)s", datefmt="%y-%m-%d %H:%M:%S", level=logging.DEBUG)\n\n\nclass CustomerField(FieldInfo):\n    pass\n\n\ndef customer_any() -> Any:\n    return Any  # type: ignore\n\n\n# For the configuration of the local template, see the use of the local template for details\nlocal_dict = {\n    "CustomerField": CustomerField,\n    "confloat": confloat,\n    "conint": conint,\n    "customer_any": customer_any,\n}\n# Specifies the start of key comments\ncomment_prefix = "p2p"\n# Specify the class of the template, can extend the template by inheriting this class, see the chapter on custom templates for details\ndesc_template: Type[DescTemplate] = DescTemplate\n# Specify the protobuf files of which packages to ignore, and the messages of the ignored packages will not be parsed\nignore_pkg_list: List[str] = ["validate", "p2p_validate"]\n# Specifies the generated file name suffix (without .py)\nfile_name_suffix = "_p2p"\n```\nNext, in order to be able to read this file, need to change the `--protobuf-to-pydantic_out=. ` to ` --protobuf-to-pydantic_out=config_path=plugin_config.py:. `.\nwhere the left side of `:` indicates that the configuration file path to be read is `plugin_config.py`, and the right side of `:` declares that the output location of the `protobuf-to-pydantic` plugin is `. `\nThe final complete command is as follows：\n```bash\npython -m grpc_tools.protoc -I. --protobuf-to-pydantic_out=config_path=plugin_config.py:. example.proto\n# or\nprotoc -I. --protobuf-to-pydantic_out=config_path=plugin_config.py:. example.proto\n```\nThrough this command, can load the corresponding configuration and run the `protobuf-to-pydantic` plug-in。\n\nIn addition to the configuration options in the example configuration file,\nthe `protobuf-to-pydantic` plug-in also supports other configuration options.\nThe specific configuration instructions are as follows：\n\n| Configuration name            | Functional module                      | Type                                            | Hidden meaning                                                                                                                                      |\n|-------------------------------|----------------------------------------|-------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------|\n| local_dict                    | Template                               | dict                                            | Holds variables for the `local` template                                                                                                            |\n| desc_template                 | Template                               | protobuf_to_pydantic.desc_template.DescTemplate | Implementation of the template class                                                                                                                |\n| comment_prefix                | Template                               | str                                             | Comment prefix.Only strings with a fixed prefix will be used by the template                                                                        |\n| customer_import_set           | Code generation                        | `Set[str]`                                      | A collection of custom import statements, such as `from typing import Set`or `import typing`, that will write data in order to the source code file |\n| customer_deque                | Code generation                        | `deque[str]`                                    | Custom source file content, used to add custom content                                                                                              |\n| module_path                   | str                                    | str                                             | Used to define the root path of the project or module, which helps `protobuf-to-pydantic`to better automatically generate module import statements   |\n| pyproject_file_path           | Code generation                        | str                                             | Define the pyproject file path, which defaults to the current project path                                                                          |\n| code_indent                   | Code generation                        | int                                             | Defines the number of indentation Spaces in the code; the default is 4                                                                              |\n| ignore_pkg_list               | Code generation(Limit plug-ins only)   | `list[str]`                                     | Definition ignores parsing of the specified package file                                                                                            |\n| base_model_class              | Model Code generation, Code generation | `Type[BaseModel]`                               | Define the parent class of the generated Model                                                                                                      |\n| file_name_suffix              | Code generation                        | str                                             | Define the generated file suffix, default `_p2p.py`                                                                                                 |\n| file_descriptor_proto_to_code | Code generation(Limit plug-ins only)   | `Type[FileDescriptorProtoToCode]`               | Define the `FileDescriptorProtoToCode` to use                                                                                                       |\n\n\n#### 1.1.3.buf-cli\nIf you are using `buf-cli` to manage Protobuf files,\nthen you can also use `protobuf-to-pydantic` in `buf-cli`, See [How to use `protobuf-to-pydantic` in `buf-cli`](https://github.com/so1n/protobuf_to_pydantic/blob/master/buf-plugin/README.md)\n\n### 1.2.Generate a `Pydantic Model` object in Python runtime\n`protobuf_to_pydantic` can generate the corresponding `PydanticModel` object based on the `Message` object at runtime。\n\nFor example, the `UserMessage` in the following Protobuf file named `demo.proto`:\n```protobuf\n// path: ./demo.proto\nsyntax = "proto3";\npackage user;\n\nenum SexType {\n  man = 0;\n  women = 1;\n}\n\nmessage UserMessage {\n  string uid=1;\n  int32 age=2;\n  float height=3;\n  SexType sex=4;\n  bool is_adult=5;\n  string user_name=6;\n}\n```\n`protoc` can be used to generate the Python code file corresponding to the `Protobuf` file (the file name is `demo_pb2.py`), and the code related to the `UserMessage` is stored in the code file.\n\nAt `Python` runtime, The func `msg_to_pydantic_model` can be called to read the `UserMessage` object from the `demo_pb2` module and generate the corresponding `Pydantic Model` object as follows:\n```Python\nfrom typing import Type\nfrom protobuf_to_pydantic import msg_to_pydantic_model\nfrom pydantic import BaseModel\n\n# import protobuf gen python obj\nfrom . import demo_pb2\n\nUserModel: Type[BaseModel] = msg_to_pydantic_model(demo_pb2.UserMessage)\nprint(\n    {\n        k: v.field_info\n        for k, v in UserModel.__fields__.items()\n    }\n)\n\n# output\n# {\n#   `uid`: FieldInfo(default=``, extra={}),\n#   `age`: FieldInfo(default=0, extra={}),\n#   `height`: FieldInfo(default=0.0, extra={}),\n#   `sex`: FieldInfo(default=0, extra={}),\n#   `is_adult`: FieldInfo(default=False, extra={}),\n#   `user_name`: FieldInfo(default=``, extra={})\n#  }\n```\nThrough the output results, it can be found that the generated `pydantic.BaseModel` object also contains `uid`, `age`, `height`, `sex`, `is adult` and `user name` fields,\nand the `default` property matches the zero value of the Protobuf type。\n\nThe `msg_to_pydantic_model` func is customizable just like plugins, with the following extension parameters:\n\n| Fields                                    | Meaning                                                   |\n|-------------------------------------------|-----------------------------------------------------------|\n| default_field                             | Generate a `Field` for each field in the `Pydantic Model` |\n| comment_prefix                            | The prefix of a comment that can be parsed                |\n| parse_msg_desc_method                     | Parsing rules to use                                      |\n| local_dict                                | Variables used by the `local` template                    |\n| pydantic_base                             | Generates the parent class of the `Pydantic Model` object |\n| pydantic_module                           | Generate the `Module` of the `Pydantic Model` object      |\n| desc_template                             | Template class to use                                     |\n| message_type_dict_by_type_name            | Protobuf type mapping to `Python` type                    |\n| message_default_factory_dict_by_type_name | Protobuf type mapping to the Python type factory          |\n\n\nIn addition to generating the corresponding `Pydantic Model` object at runtime,\n`protobuf-to-pydantic` also supports converting `Pydantic Model` objects to Python code text at runtime (only compatible with `Pydantic Model` objects generated by `protobuf-to-pydantic`).\nThe `pydantic_model_to_py_code` func is used to generate the source code, and the `pydantic_model_to_py_file` func is used to generate the code file. The example code of the `pydantic_model_to_py_file` func is as follows:\n\n```Python\nfrom protobuf_to_pydantic import msg_to_pydantic_model, pydantic_model_to_py_file\n\n# import protobuf gen python obj\nfrom example.example_proto_python_code.example_proto.demo import demo_pb2\n\npydantic_model_to_py_file(\n    "./demo_gen_code.py",\n    msg_to_pydantic_model(demo_pb2.NestedMessage),\n)\n```\nWhen the code runs, it converts`demo_pb2.NestedMessage`to a Pydantic Model object and passes it to the  `pydantic_model_to_py_file`. `pydantic_model_to_py_file` generates the source code and writes it to a `demo_gen_code.py` file.\n\n\n## 2.Parameter validation\nIn the previous section, the `Pydantic Model` object generated by the Protobuf file is very simple because the Protobuf file does not have enough parameters to verify the relevant information.\nIn order for each field in the generated `Pydantic Model` object to have parameter validation capabilities, the corresponding parameter checking rules for the field need to be refined in the Protobuf file.\n\nCurrently, `protobuf-to-pydantic` supports three validation rules：\n- 1.Text annotations\n- 2.PGV(protoc-geb-validate)\n- 3.P2P\n\nWith these rules, the `Pydantic Model` object generated by `protobuf-to-pydantic` will have parameter validation feature.\nAmong them, text annotations and P2P rules are consistent, they both support most of the parameters in `Pydantic Field`, some of the variations and new parameters are seen\n[2.4.`P2P` and text annotation rule other parameter support](#24p2p-and-text-comment-rule-other-parameter-support)\n\n> NOTE:\n>  - 1.Text annotation rules are not the focus of subsequent functional iterative development, and it is recommended to use P2P verification rules.\n>  - 2.`Protoc Plug-in` only support `PGV` and `P2P` rule.\n\n\n### 2.1.Text annotations\nIn the Protobuf file, can write annotations for each field that meet the requirements of `protobuf-to-pydantic`,\nso that `protobuf-to-pydantic` can obtain the validation information of the parameters when parsing the Protobuf file, such as the following example\n```protobuf\nsyntax = "proto3";\npackage user;\n\nenum SexType {\n  man = 0;\n  women = 1;\n}\n\n// user info\nmessage UserMessage {\n  // p2p: {"required": true, "example": "10086"}\n  // p2p: {"title": "UID"}\n  string uid=1; // p2p: {"description": "user union id"}\n  // p2p: {"example": 18, "title": "use age", "ge": 0}\n  int32 age=2;\n  // p2p: {"ge": 0, "le": 2.5}\n  float height=3;\n  SexType sex=4;\n  bool is_adult=5;\n  // p2p: {"description": "user name"}\n  // p2p: {"default": "", "min_length": 1, "max_length": "10", "example": "so1n"}\n  string user_name=6;\n}\n```\n\nIn this example, each annotation that can be used by `protobuf_to_pydantic` starts with `p2p:` (supports customization) and is followed by a complete Json string. If are familiar with the usage of `pydantic`, can find This Json string contains the verification information corresponding to `pydantic.Field`. For example, the `uid` field in `UserMessage` contains a total of 4 pieces of information as follows：\n\n| Column      | Meaning                                                                               |\n|-------------|---------------------------------------------------------------------------------------|\n| required    | Indicates that the generated field does not have a default value                      |\n| example     | An example value representing the generated field is 10086                            |\n| title       | Indicates that the schema name of the field is UID                                    |\n | description | The schema documentation for the representation field is described as `user_union_id` |\n\n> Note:\n>   - 1.Currently only single-line comments are supported and comments must be a complete Json data (no line breaks).\n>   - 2.multi line comments are not supported。\n\nWhen these annotations are written, `protobuf_to_pydantic` will bring the corresponding information for each field when converting the Message into the corresponding `Pydantic.BaseModel` object, as follows:\n\n```python\n# pydantic version V1\nfrom typing import Type\nfrom protobuf_to_pydantic import msg_to_pydantic_model\nfrom pydantic import BaseModel\n\n# import protobuf gen python obj\nfrom example.example_proto_python_code.example_proto.demo import demo_pb2\n\nUserModel: Type[BaseModel] = msg_to_pydantic_model(demo_pb2.UserMessage, parse_msg_desc_method=demo_pb2)\nprint(\n    {\n        k: v.field_info\n        for k, v in UserModel.__fields__.items()\n    }\n)\n# output\n# {\n#   `uid`: FieldInfo(default=PydanticUndefined, title=`UID`, description=`user union id`, extra={`example`: `10086`}),\n#   `age`: FieldInfo(default=0, title=`use age`, ge=0, extra={`example`: 18}),\n#   `height`: FieldInfo(default=0.0, ge=0, le=2, extra={}),\n#   `sex`: FieldInfo(default=0, extra={}),\n#   `is_adult`: FieldInfo(default=False, extra={}),\n#   `user_name`: FieldInfo(default=``, description=`user name`, min_length=1, max_length=10, extra={`example`: `so1n`})\n# }\n```\nIt can be seen that the output fields carry the corresponding information, which is consistent with the comments of the Protobuf file.\n\nIn addition, this code differs from the previous section in that the `msg_to_pydantic_model` function has a keyword argument named `parse_msg_desc_method` and its value is the \'demo_pb2\' module.\nThis parameter enables `protobuf-to-pydantic` to obtain additional information about each field in the Message object through comments in the `.pyi` file of the `demo_pb2` module.\n\n> Note: This function needs to use the [mypy-protobuf](https://github.com/nipunn1313/mypy-protobuf) plugin when generating the corresponding `Python code through the Protobuf file, and the specified pyi file output path is the same as the generated `Python` code path to take effect.\n> And need to install `protobuf-to-pydantic` via the `python -m pip install protobuf-to-pydantic[mypy-protobuf]` command\n\nIn addition to getting comments from the `.pyi` file, `protobuf-to-pydantic` also supports getting comment information for each field through comments on the Protobuf file to which the Message object belongs.\nUsing this feature is as simple as setting the value of `parse_msg_desc_method` to the root directory path specified when the Message object was generated.\n\n> When using this method, make sure to install `protobuf-to-pydantic` via `python -m pip install protobuf-to-pydantic[lark]`, and also make sure that the Protobuf file exists in the project.\n\nFor example, the project structure of the `protobuf-to-pydantic` sample code is as follows:\n```bash\n./protobuf_to_pydantic/\n├── example/\n│ ├── python_example_proto_code/\n│ └── example_proto/\n├── protobuf_to_pydantic/\n└── /\n```\n\nThe Protobuf file is stored in the `example/example_proto` folder, and then run the following command in the `example` directory to generate the `Python` code file corresponding to Protobuf:\n```bash\ncd example\n\npython -m grpc_tools.protoc\n  --python_out=./python_example_proto_code \\\n  --grpc_python_out=./python_example_proto_code \\\n  -I. \\\n# or\nprotoc\n  --python_out=./python_example_proto_code \\\n  --grpc_python_out=./python_example_proto_code \\\n  -I. \\\n```\nThen the path that needs to be filled in for `parse_msg_desc_method` at this time is `./protobuf_to_pydantic/example`.\nThe following sample code:\n```python\n# pydantic Version v1\nfrom typing import Type\nfrom protobuf_to_pydantic import msg_to_pydantic_model\nfrom pydantic import BaseModel\n\n# import protobuf gen python obj\nfrom example.proto_3_20_pydanticv1.example.example_proto.demo import demo_pb2\n\nUserModel: Type[BaseModel] = msg_to_pydantic_model(\n    demo_pb2.UserMessage, parse_msg_desc_method="./protobuf_to_pydantic/example"\n)\nprint(\n    {\n        k: v.field_info\n        for k, v in UserModel.__fields__.items()\n    }\n)\n# output\n# {\n#   `uid`: FieldInfo(default=PydanticUndefined, title=`UID`, description=`user union id`, extra={`example`: `10086`}),\n#   `age`: FieldInfo(default=0, title=`use age`, ge=0, extra={`example`: 18}),\n#   `height`: FieldInfo(default=0.0, ge=0, le=2, extra={}),\n#   `sex`: FieldInfo(default=0, extra={}),\n#   `is_adult`: FieldInfo(default=False, extra={}),\n#   `user_name`: FieldInfo(default=``, description=`user name`, min_length=1, max_length=10, extra={`example`: `so1n`})\n# }\n```\nAs you can see, the only difference in this code is the value of the `parse_msg_desc_method`, but through the output result, you can see that the field carries the same information as the result obtained through the module.\n\n### 2.2.PGV(protoc-gen-validate)\nAt present, the commonly used parameter verification project in the Protobuf ecosystem is [protoc-gen-validate](https://github.com/envoyproxy/protoc-gen-validate)，\nIt has become a common standard in Protobuf because it supports multiple languages and requires only one writing of `PGV` rules to make the generated `Message` object support the corresponding validation rules.\n\n> Currently `protobuf-to-pydantic` only supports rules that [protoc-gen-validate](https://github.com/envoyproxy/protoc-gen-validate) is less than version 1.0.0\n\n`protobuf-to-pydantic` supports parsing of `PGV` validation rules and generates `Pydantic Model` objects with validation logic functions.\nUsing `PGV` checksum rules in `protobuf-to-pydantic` is very simple, just write the corresponding `PGV` rules in the Protobuf file first,\nand then specify the value of `parse_msg_desc_method` to be `PGV` when calling `msg_to_pydantic_model` as the code below:\n```Python\n# pydantic version V1\nfrom typing import Type\nfrom protobuf_to_pydantic import msg_to_pydantic_model\nfrom pydantic import BaseModel\n\n# import protobuf gen python obj\nfrom example.proto_3_20_pydanticv1.example.example_proto.validate import demo_pb2\n\nUserModel: Type[BaseModel] = msg_to_pydantic_model(\n    demo_pb2.FloatTest, parse_msg_desc_method="PGV"\n)\nprint(\n    {\n        k: v.field_info\n        for k, v in UserModel.__fields__.items()\n    }\n)\n# output\n# {\n#   `const_test`: FieldInfo(default=1.0, const=True, extra={}),\n#   `range_e_test`: FieldInfo(default=0.0, ge=1, le=10, extra={}),\n#   `range_test`: FieldInfo(default=0.0, gt=1, lt=10, extra={}),\n#   `in_test`: FieldInfo(default=0.0, extra={`in`: [1.0, 2.0, 3.0]}),\n#   `not_in_test`: FieldInfo(default=0.0, extra={`not_in`: [1.0, 2.0, 3.0]}),\n#   `ignore_test`: FieldInfo(default=0.0, extra={})\n# }\n```\n\n> Note:\n>  - 1.For the usage of `PGV`, see: [protoc-gen-validate doc](https://github.com/bufbuild/protoc-gen-validate/blob/v0.10.2-SNAPSHOT.17/README.md)\n>  - 2.Need to install `PGV` through `pip install protoc_gen_validate` or download [validate.proto](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/example_proto/common/validate.proto) to the protobuf directory in the project to write pgv rules in the Protobuf file.\n\n\n### 2.3.P2P\nThe `PGV` verification rules are written in the Option attribute of each field of `Message` and have a better code specification,\nso Protobuf that use `PGV` checksum rules will be more readable than Protobuf that use annotation .\n\nAt the same time, when writing `PGV` rules, can also experience the convenience of the IDE\'s auto-completion and the security of checksumming when generating the corresponding language objects from Protobuf files, but it only supports checksumming-related logic, which is not as rich as the file annotation mode.\n\n\nThe `P2P` verification rule that comes with `protobuf-to-pydantic` expands on the `PGV` verification rule by incorporating some of the functionality of the text annotation verification rule, which satisfies most of the customization of the properties of each `Field` in the `Pydantic Model`, such as the following Protobuf file.\n```protobuf\nsyntax = "proto3";\npackage p2p_validate_test;\n\nimport "example_proto/common/p2p_validate.proto";\n\n\nmessage FloatTest {\n  float const_test = 1 [(p2p_validate.rules).float.const = 1];\n  float range_e_test = 2 [(p2p_validate.rules).float = {ge: 1, le: 10}];\n  float range_test = 3[(p2p_validate.rules).float = {gt: 1, lt: 10}];\n  float in_test = 4[(p2p_validate.rules).float = {in: [1,2,3]}];\n  float not_in_test = 5[(p2p_validate.rules).float = {not_in: [1,2,3]}];\n  float default_test = 6[(p2p_validate.rules).float.default = 1.0];\n  float not_enable_test = 7[(p2p_validate.rules).float.enable = false];\n  float default_factory_test = 8[(p2p_validate.rules).float.default_factory = "p2p@builtin|float"];\n  float miss_default_test = 9[(p2p_validate.rules).float.miss_default = true];\n  float alias_test = 10 [(p2p_validate.rules).float.alias = "alias"];\n  float desc_test = 11 [(p2p_validate.rules).float.description = "test desc"];\n  float multiple_of_test = 12 [(p2p_validate.rules).float.multiple_of = 3.0];\n  float example_test = 13 [(p2p_validate.rules).float.example = 1.0];\n  float example_factory = 14 [(p2p_validate.rules).float.example_factory = "p2p@builtin|float"];\n  float field_test = 15[(p2p_validate.rules).float.field = "p2p@local|CustomerField"];\n  float type_test = 16[(p2p_validate.rules).float.type = "p2p@local|confloat"];\n  float title_test = 17 [(p2p_validate.rules).float.title = "title_test"];\n}\n```\n`protobuf-to-pydantic` can read the generated Message object at runtime and generate a `Pydantic Model` object with the corresponding information:\n\n```python\n# pydantic version V1\nfrom typing import Type\nfrom protobuf_to_pydantic import msg_to_pydantic_model\nfrom pydantic import BaseModel, confloat\nfrom pydantic.fields import FieldInfo\n\n# import protobuf gen python obj\nfrom example.proto_3_20_pydanticv1.example.example_proto.p2p_validate import demo_pb2\n\n\nclass CustomerField(FieldInfo):\n    pass\n\n\nDemoModel: Type[BaseModel] = msg_to_pydantic_model(\n    demo_pb2.FloatTest,\n    local_dict={"CustomerField": CustomerField, "confloat": confloat},\n)\nprint(\n    {\n        k: v.field_info\n        for k, v in DemoModel.__fields__.items()\n    }\n)\n# output:\n# {\n#   \'const_test\': FieldInfo(default=1.0, const=True, extra={}),\n#   \'range_e_test\': FieldInfo(default=0.0, ge=1, le=10, extra={}),\n#   \'range_test\': FieldInfo(default=0.0, gt=1, lt=10, extra={}),\n#   \'in_test\': FieldInfo(default=0.0, extra={\'in\': [1.0, 2.0, 3.0]}),\n#   \'not_in_test\': FieldInfo(default=0.0, extra={\'not_in\': [1.0, 2.0, 3.0]}),\n#   \'default_test\': FieldInfo(default=1.0, extra={}),\n#   \'default_factory_test\': FieldInfo(default=PydanticUndefined, default_factory=<class \'float\'>, extra={}),\n#   \'miss_default_test\': FieldInfo(extra={}),\n#   \'alias_test\': FieldInfo(default=0.0, alias=\'alias\', alias_priority=2, extra={}),\n#   \'desc_test\': FieldInfo(default=0.0, description=\'test desc\', extra={}),\n#   \'multiple_of_test\': FieldInfo(default=0.0, multiple_of=3, extra={}),\n#   \'example_test\': FieldInfo(default=0.0, extra={\'example\': 1.0}),\n#   \'example_factory\': FieldInfo(default=0.0, extra={\'example\': <class \'float\'>}),\n#   \'field_test\': CustomerField(default=0.0, extra={}),\n#   \'type_test\': FieldInfo(default=0.0, extra={}),\n#   \'title_test\': FieldInfo(default=0.0, title=\'title_test\', extra={})\n#   }\n```\n\n> Note:\n>  - 1.See the [2.5.template](#25Template) for the usage of `local_dict`\n>  - 2.If the reference to the Proto file fails, need to download [p2p_validate.proto](https://github.com/so1n/protobuf_to_pydantic/blob/master/protos/protobuf_to_pydantic/protos/p2p_validate.proto) in the project and use it in the Protobuf file。\n\n\n\n### 2.4.`P2P` and text annotation rule other parameter support\nThe `protobuf-to-pydantic` text annotation rules and the `P2P` rules support most of the parameters in `FieldInfo`, as described in the [Pydantic Field doc](https://docs.pydantic.dev/latest/usage/fields/)。\n\n> The new parameters added to `Pydantic V2` will be supported in version 2.1, for now `P2P` rule naming is still written on the basis of `Pydantic V1`, but automatic mapping to `Pydantic V2` naming is supported.\n\nOther partial changes in meaning and new parameters are described as follows:\n\n| Parameter        | Default value | Illustrate                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |\n|------------------|---------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|\n| required         | False         | By default, the default value of each field in the generated `Pydantic Model` object is the same as the zero value of its corresponding type. When `required` is `True`, no more default values are generated for the fields.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |\n| enable           | True          | By default, `protobuf-to-pydantic` generates all fields for `Message`, if don\'t want the generated `Message` to have this field, can set `enable` to `False`.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |\n| const            | None          | Used to specify a constant value for a field, though different `Pydantic` versions behave differently<br/>  For `Pydantic V1`, the value of `default` in `Field` is set to the value specified by `const`, and `const` in `Field` is set to True.Note: `Pydantic Model`\'s const only supports bool variables, when `const` is `True`, the accepted value can only be the value set by `default`, and the default value carried by the message generated by protobuf is the zero value of the corresponding type does not match with `Pydantic Model`, so ` protobuf-to-pydantic` makes some changes to the input of this value.<br/> For `Pydantic V2`, the value of `default` in `Field` remains the same, but the type annotation changes to `typing_extensions.Literal[xxx]` |\n| type             | None          | By default, the default type of a field is the same as Protobuf\'s, but use the [2.5.template](#25Template) function to modify the type of a field.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |\n| extra            | None          | The `extra` parameter accepted by `Pydantic` is of type `Python Dict`, which is not supported by Protobuf, and requires the use of either [2.5.Templates](#25Templates) or the corresponding Json structure `protobuf-to-pydantic` in the Protobuf file to parse it properly.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |\n| field            | None          | By default, the `Field` of the parameter is `Pydantic FieldInfo`, although it can be customized using the [2.5.Templates](#25Templates) function                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |\n| default_template | None          | Similar to `default`, default values can be customized in fields that are not of string type using the [2.5.Templates](#25Templates) feature.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |\n\nIn addition to the above parameters, also support for fast import of `Pydantic type` for string types. For example, if want to add a check for card numbers via the `pydantic.types.PaymentCardNumber` type, can specify the type of the `pydantic_type` parameter field to be `PaymentCardNumber`, which is similar to the use of template imports in the `type` rule, as follows:\n- Text annotation rules：\n  ```protobuf\n  syntax = "proto3";\n  package common_validate_test;\n\n  // common example\n  message UserPayMessage {\n    string bank_number=1; // p2p: {"pydantic_type": "PaymentCardNumber"}\n    string other_bank_number=2; // p2p: {"type": "p2p@import|pydantic.types|PaymentCardNumber"}\n  }\n  ```\n- P2P rules：\n  ```protobuf\n  syntax = "proto3";\n  package p2p_validate_test;\n\n  import "example_proto/common/p2p_validate.proto";\n  // p2p example\n  message UserPayMessage {\n    string bank_number=1[(p2p_validate.rules).string.pydantic_type = "PaymentCardNumber"];\n    string other_bank_number=2[(p2p_validate.rules).string.type = "p2p@import|pydantic.types|PaymentCardNumber"];\n  }\n  ```\n\n> See [Extra Types Overview](https://docs.pydantic.dev/latest/usage/types/extra_types/extra_types/) for supported `Pydantic Types\'.\n### 2.5.Template\nWhen working with definition fields, will find that some fields are filled with values that are methods or functions of one of the libraries in `Python` (e.g., the values of the `type` parameter and the `default_factory` parameter), which can\'t be accomplished with the Json syntax.\nAt this point, templates can be used to solve the corresponding problem, and currently `protobuf-to-pydantic` supports a variety of template functi\n\n> Note: The `p2p` string at the beginning of a template can be defined via the comment_prefix variable\n\n#### 2.5.1.`p2p@import`Template\nThe `p2p@import` template is used to represent variables in other modules that need to be introduced before they can be used, as follows.\n- Examples of text annotation rules：\n  ```protobuf\n  syntax = "proto3";\n  package comment_validate_test;\n\n  // comment example\n  message UserPayMessage {\n    string bank_number=1; // p2p: {"type": "p2p@import|pydantic.types|PaymentCardNumber"}\n  }\n  ```\n\n- Examples of P2P rules (1)：\n  ```protobuf\n  syntax = "proto3";\n  package p2p_validate_test;\n  import "example_proto/common/p2p_validate.proto";\n\n  message UserPayMessage {\n    string bank_number=1[(p2p_validate.rules).string.type = "p2p@import|pydantic.types|PaymentCardNumber"];\n  }\n  ```\n\n- Examples of P2P rules (2)：\n  ```protobuf\n  syntax = "proto3";\n  package p2p_other_validate_test;\n  import "example_proto/common/p2p_validate.proto";\n  // p2p other example\n  message UserPayMessage {\n    string bank_number=1[(p2p_validate.rules).string.pydantic_type = "PaymentCardNumber"];\n  }\n  ```\n\nThe example Protobuf file uses a syntax in the format `p2p@{methods of the template}|{modules to be imported:A}|{variables in modules:B}`, indicating that a `B` object needs to be imported by `from A import B` and used by the corresponding rule.\nWith the definition of the template, `protobuf-to-pydantic` converts the corresponding Message into a `Pydantic Model`, as follows:\n```python\nfrom pydantic import BaseModel\nfrom pydantic.fields import FieldInfo\n# p2p@import|pydantic.types|PaymentCardNumber\nfrom pydantic.types import PaymentCardNumber\n\nclass UserPayMessage(BaseModel):\n    bank_number: PaymentCardNumber = FieldInfo(default="", extra={})\n```\n\n#### 2.5.2.`p2p@import_instance` Template\nThe `p2p@import_instance` template introduces the class of a library and then instantiates it in combination with the specified parameters before it is used by the corresponding rule, which is used as follows:\n```protobuf\nsyntax = "proto3";\npackage p2p_validate_test;\nimport "google/protobuf/any.proto";\nimport "example_proto/common/p2p_validate.proto";\n// p2p example\nmessage AnyTest {\n  google.protobuf.Any default_test = 23 [\n    (p2p_validate.rules).any.default = \'p2p@import_instance|google.protobuf.any_pb2|Any|{"type_url": "type.googleapis.com/google.protobuf.Duration"}\'\n  ];\n}\n```\nThe syntax used here is `p2p@{methods of the template}|{modules to be introduced}|{classes to be introduced}|{initialization parameters}`, and the definition of `protobuf-to-pydantic` through the template will turn the corresponding Message into the following `Pydantic Model` object:\n```python\nfrom google.protobuf.any_pb2 import Any as AnyMessage\nfrom pydantic import BaseModel\nfrom pydantic.fields import FieldInfo\n\n\nclass AnyTest(BaseModel):\n    default_test: AnyMessage = FieldInfo(\n        default=AnyMessage(type_url="type.googleapis.com/google.protobuf.Duration")\n    )\n```\n\n#### 2.5.3.`p2p@local` Template\nThis template is used to introduce user-defined variables, using a syntax in the format `{method of the template}|{local variable to be used}`, as follows:\n\n- Example of text annotation:\n  ```protobuf\n  syntax = "proto3";\n  package comment_validate_test;\n  import "google/protobuf/timestamp.proto";\n  import "example_proto/common/p2p_validate.proto";\n  // comment example\n  message UserPayMessage {\n    google.protobuf.Timestamp exp=1; // p2p: {"default_factory": "p2p@local|exp_time"}\n  }\n  ```\n- Examples of P2P rules：\n  ```protobuf\n  syntax = "proto3";\n  package p2p_validate_test;\n  import "google/protobuf/timestamp.proto";\n  import "example_proto/common/p2p_validate.proto";\n  // p2p example\n  message UserPayMessage {\n    google.protobuf.Timestamp exp=1[(p2p_validate.rules).timestamp.default_factory= "p2p@local|exp_time"];\n  }\n  ```\nHowever, the `msg_to_pydantic_model` func needs to be called with the parameter `local_dict` to register the corresponding value, the pseudo-code is as follows:\n```Python\n# a.py\nimport time\n\nfrom example.proto_3_20_pydanticv1.example.example_proto.p2p_validate import demo_pb2\nfrom protobuf_to_pydantic import msg_to_pydantic_model\n\n\ndef exp_time() -> float:\n  return time.time()\n\nmsg_to_pydantic_model(\n    demo_pb2.NestedMessage,\n    local_dict={"exp_time": exp_time},  # <----  use local_dict\n)\n```\nIn this way, `protobuf-to-pydantic` generates a conforming `Pydantic Model` object:\n```python\n# b.py\nfrom datetime import datetime\nfrom pydantic import BaseModel\nfrom pydantic.fields import FieldInfo\n\nfrom a import exp_time  # <-- exp_time in a.py\n\nclass UserPayMessage(BaseModel):\n    exp: datetime = FieldInfo(default_factory=exp_time, extra={})\n```\n\n\n#### 2.5.4.`p2p@builtin` Template\nThis template (which can be thought of as a simplified version of the `p2p@local` template) can be used directly when the variables to be used come from `Python` built-in functions,the syntax is used as follows:\n- Examples of text annotation rules:\n  ```protobuf\n  syntax = "proto3";\n  package comment_validate_test;\n  import "google/protobuf/timestamp.proto";\n  import "example_proto/common/p2p_validate.proto";\n  // comment example\n  message UserPayMessage {\n    google.protobuf.Timestamp exp=1; // p2p: {"type": "p2p@builtin|float"}\n  }\n  ```\n- Examples of P2P rules：\n  ```protobuf\n  syntax = "proto3";\n  package p2p_validate_test;\n  import "google/protobuf/timestamp.proto";\n  import "example_proto/common/p2p_validate.proto";\n  // p2p example\n  message UserPayMessage {\n    google.protobuf.Timestamp exp=1[(p2p_validate.rules).timestamp.type= "p2p@builtin|float"];\n  }\n  ```\nThen can directly generate a conforming `Pydantic Model` object by calling the `msg_to_pydantic_model` function, as follows:\n```python\nfrom pydantic import BaseModel\nfrom pydantic.fields import FieldInfo\n\n\nclass UserPayMessage(BaseModel):\n    exp: float = FieldInfo()\n```\n#### 2.5.5.Customized templates\nCurrently `protobuf-to-pydantic` only supports a few simple templates, if have more template needs, can extend the templates by inheriting the `DescTemplate` class.\n\nFor example, there is an odd feature that requires the default value of a field to be the timestamp of the time when the `Pydantic Model` object was generated, but the timestamps used are available in lengths of 10 and 13, so the following Protobuf file needs to be written to support defining the length of the timestamps:\n```protobuf\nsyntax = "proto3";\npackage p2p_validate_test;\nimport "google/protobuf/timestamp.proto";\nimport "example_proto/common/p2p_validate.proto";\n\nmessage TimestampTest{\n  int32 timestamp_10 = 1[(p2p_validate.rules).int32.default_template = "p2p@timestamp|10"];\n  int32 timestamp_13 = 2[(p2p_validate.rules).int32.default_template = "p2p@timestamp|13"];\n}\n```\nAs you can see, the Protobuf file customizes the syntax of `p2p@timestamp|{x}`, where `x` has only two values, 10 and 13. The next step is to write code based on this template behavior, which looks like this.\n```python\nimport time\nfrom protobuf_to_pydantic.gen_model import DescTemplate\n\nclass CustomDescTemplate(DescTemplate):\n    def template_timestamp(self, length_str: str) -> int:\n        timestamp: float = time.time()\n        if length_str == "10":\n            return int(timestamp)\n        elif length_str == "13":\n            return int(timestamp * 100)\n        else:\n            raise KeyError(f"timestamp template not support value:{length_str}")\n\n\nfrom .demo_pb2 import TimestampTest # fake code\nfrom protobuf_to_pydantic import msg_to_pydantic_model\n\nmsg_to_pydantic_model(\n    TimestampTest,\n    desc_template=CustomDescTemplate   # <-- Use a custom template class\n)\n```\nThis code first creates a class `CustomDescTemplate` that inherits from `DescTemplate`.\n`DescTemplate` will forwards to the corresponding `template_{template name}` method based on the naming of the template, so this class needs to define the `template_timestamp` method to implement the `p2p@timestamp` template functionality.\nIn addition, the `length_str` variable received in this method is either 10 in `p2p@timestamp|10` or 13 in `p2p@timestamp|13`.\n\nThen load the `CustomDescTemplate` through the `msg_to_pydantic_model` function, then the following code will be generated (assuming that the code is generated at a timestamp of 1600000000):\n```python\nfrom pydantic import BaseModel\nfrom pydantic.fields import FieldInfo\n\nclass TimestampTest(BaseModel):\n    timestamp_10: int = FieldInfo(default=1600000000)\n    timestamp_13: int = FieldInfo(default=1600000000000)\n```\n## 3.Code format\nThe code generated directly through `protobuf-to-pydantic` is not perfect, but it is possible to indirectly generate code that conforms to the `Python` specification through different formatting tools.\nCurrently, `protobuf-to-pydantic` supports formatting tools such as `autoflake`, `black` and `isort`. If the corresponding formatting tool is installed in the current `Python` environment, then `protobuf-to-pydantic` will call the tool to format the generated code before outputting it to a file.\n\nIn addition, the decision to enable or disable a formatting tool can be made through the `pyproject.toml` configuration file, the `pyproject.toml` example of which reads as follows:\n```toml\n# Controls which formatting tools protobuf-to-pydantic uses,\n# if false then no formatting tools are used (default is true)\n[tool.protobuf-to-pydantic.format]\nblack = true\nisort = true\nautoflake = true\n\n# black docc:https://black.readthedocs.io/en/stable/usage_and_configuration/the_basics.html#configuration-format\n[tool.black]\nline-length = 120\ntarget-version = [\'py37\']\n\n# isort doc:https://pycqa.github.io/isort/docs/configuration/config_files.html#pyprojecttoml-preferred-format\n[tool.isort]\nprofile = "black"\nmulti_line_output = 3\ninclude_trailing_comma = true\nforce_grid_wrap = 0\nuse_parentheses = true\nensure_newline_before_comments = true\nline_length = 120\n\n# autoflake doc:https://github.com/PyCQA/autoflake#configuration\n[tool.autoflake]\nin-place = true\nremove-all-unused-imports = true\nremove-unused-variables = true\n```\n\n## 4.example\n`protobuf-to-pydantic` provides some simple example code for reference only.\n\n### 4.1.Generate code directly\nProtobuf file: [demo/demo.proto](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/example_proto/demo/demo.proto)\n\nGenerate `Pydantic Model`(Pydantic V1): [proto_pydanticv1/demo_gen_code.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv1/demo_gen_code.py)\n\nGenerate `Pydantic Model`(Pydantic V2): [proto_pydanticv2/demo_gen_code.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv2/demo_gen_code.py)\n### 4.2.Text annotation\nProtobuf File: [demo/demo.proto](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/example_proto/demo/demo.proto)\n\n`Pydantic Model` generated based on `pyi` file(Pydantic V1): [proto_pydanticv1/demo_gen_code_by_text_comment_pyi.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv1/demo_gen_code_by_text_comment_pyi.py)\n\n`Pydantic Model` generated based on `pyi` file(Pydantic V2): [proto_pydanticv2/demo_gen_code_by_text_comment_pyi.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv2/demo_gen_code_by_text_comment_pyi.py)\n\n`Pydantic Model` generated based on protobuf file(Pydantic V1): [proto_pydanticv1/demo_gen_code_by_text_comment_protobuf_field.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv1/demo_gen_code_by_text_comment_protobuf_field.py)\n`Pydantic Model` generated based on protobuf file(Pydantic V2): [proto_pydanticv2/demo_gen_code_by_text_comment_protobuf_field.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv2/demo_gen_code_by_text_comment_protobuf_field.py)\nvalidate/demo.proto](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/example_proto/validate/demo.proto)\n\nGenerate `Pydantic Model`(Pydantic V1): [proto_pydanticv1/demo_gen_code_by_pgv.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv1/demo_gen_code_by_pgv.py)\n\nGenerate `Pydantic Model`(Pydantic V2): [proto_pydanticv2/demo_gen_code_by_pgv.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv2/demo_gen_code_by_pgv.py)\n### 4.4.P2P rule\nProtobuf file: [p2p_validate/demo.proto](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/example_proto/p2p_validate/demo.proto)\n\nGenerate `Pydantic Model`(Pydantic V1): [proto_pydanticv1/demo_gen_code_by_p2p.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv1/demo_gen_code_by_p2p.py)\n\nGenerate `Pydantic Model`(Pydantic V2): [proto_pydanticv2/demo_gen_code_by_p2p.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv2/demo_gen_code_by_p2p.py)\n### 4.5.Protoc Plugin-in\nProtobuf field: [demo/demo.proto](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/example_proto/demo/demo.proto)，[validate/demo.proto](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/example_proto/validate/demo.proto)，[p2p_validate/demo.proto](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/example_proto/p2p_validate/demo.proto)\n\n> Note: The Protoc plugin only supports P2P and PGV rules\n\n`Pydantic Model` generated via `demo/demo.proto`(Pydantic V1):[example_proto/demo/demo_p2p.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv1/example/example_proto/demo/demo_p2p.py)\n\n`Pydantic Model` generated via `demo/demo.proto`(Pydantic V2):[example_proto/demo/demo_p2p.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv2/example/example_proto/demo/demo_p2p.py)\n\n`Pydantic Model` generated via `validate/demo.proto`(Pydantic V1):[example_proto/validate/demo_p2p.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv1/example/example_proto/validate/demo_p2p.py)\n\n`Pydantic Model` generated via `validate/demo.proto`(Pydantic V1):[example_proto/validate/demo_p2p.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv2/example/example_proto/validate/demo_p2p.py)\n\n`Pydantic Model` generated via `p2p_validate/demo.proto`(Pydantic V1):[example_proto/p2p_validate/demo_p2p.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv1/example/example_proto/p2p_validate/demo_p2p.py)\n\n`Pydantic Model` generated via `p2p_validate/demo.proto`(Pydantic V1):[example_proto/p2p_validate/demo_p2p.py](https://github.com/so1n/protobuf_to_pydantic/blob/master/example/proto_pydanticv2/example/example_proto/p2p_validate/demo_p2p.py)\n',
     'author': 'So1n',
     'author_email': 'so1n897046026@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/so1n/protobuf_to_pydantic',
```

### Comparing `protobuf_to_pydantic-0.2.6.1/PKG-INFO` & `protobuf_to_pydantic-0.2.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protobuf-to-pydantic
-Version: 0.2.6.1
+Version: 0.2.6.2
 Summary: Generate the `pydantic.BaseModel` class (and the corresponding source code) with parameter verification function through the Protobuf file
 Home-page: https://github.com/so1n/protobuf_to_pydantic
 License: Apache Software License
 Author: So1n
 Author-email: so1n897046026@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
```

