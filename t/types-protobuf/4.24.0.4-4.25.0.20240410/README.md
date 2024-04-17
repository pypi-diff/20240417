# Comparing `tmp/types-protobuf-4.24.0.4.tar.gz` & `tmp/types-protobuf-4.25.0.20240410.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-protobuf-4.24.0.4.tar", last modified: Sun Oct 29 02:16:23 2023, max compression
+gzip compressed data, was "types-protobuf-4.25.0.20240410.tar", last modified: Wed Apr 10 02:15:07 2024, max compression
```

## Comparing `types-protobuf-4.24.0.4.tar` & `types-protobuf-4.25.0.20240410.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 02:16:23.659463 types-protobuf-4.24.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     7971 2023-10-29 02:16:22.000000 types-protobuf-4.24.0.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-10-29 02:16:22.000000 types-protobuf-4.24.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2023-10-29 02:16:23.655463 types-protobuf-4.24.0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 02:16:23.651463 types-protobuf-4.24.0.4/google-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2023-10-29 02:16:22.000000 types-protobuf-4.24.0.4/google-stubs/METADATA.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 02:16:23.655463 types-protobuf-4.24.0.4/google-stubs/protobuf/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/any_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11425 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/api_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 02:16:23.655463 types-protobuf-4.24.0.4/google-stubs/protobuf/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/compiler/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12273 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/compiler/plugin_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8860 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/descriptor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    76466 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/descriptor_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/descriptor_pool.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/duration_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/empty_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8791 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/field_mask_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 02:16:23.655463 types-protobuf-4.24.0.4/google-stubs/protobuf/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/internal/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/internal/api_implementation.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      263 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/internal/builder.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/internal/containers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/internal/decoder.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/internal/encoder.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      809 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/internal/enum_type_wrapper.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/internal/extension_dict.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/internal/message_listener.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      145 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/internal/python_message.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      492 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/internal/type_checkers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/internal/well_known_types.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/internal/wire_format.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/json_format.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/message.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      841 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/message_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/reflection.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/source_context_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7821 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/struct_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      908 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/symbol_database.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7354 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/text_format.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6961 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/timestamp_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16113 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/type_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 02:16:23.655463 types-protobuf-4.24.0.4/google-stubs/protobuf/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/util/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2023-10-29 02:16:08.000000 types-protobuf-4.24.0.4/google-stubs/protobuf/wrappers_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-29 02:16:23.659463 types-protobuf-4.24.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2023-10-29 02:16:22.000000 types-protobuf-4.24.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 02:16:23.655463 types-protobuf-4.24.0.4/types_protobuf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2023-10-29 02:16:23.000000 types-protobuf-4.24.0.4/types_protobuf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2023-10-29 02:16:23.000000 types-protobuf-4.24.0.4/types_protobuf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-29 02:16:23.000000 types-protobuf-4.24.0.4/types_protobuf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-29 02:16:23.000000 types-protobuf-4.24.0.4/types_protobuf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:15:07.936002 types-protobuf-4.25.0.20240410/
+-rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-04-10 02:15:06.000000 types-protobuf-4.25.0.20240410/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-10 02:15:06.000000 types-protobuf-4.25.0.20240410/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-10 02:15:07.936002 types-protobuf-4.25.0.20240410/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:15:07.928002 types-protobuf-4.25.0.20240410/google-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-10 02:15:06.000000 types-protobuf-4.25.0.20240410/google-stubs/METADATA.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:15:07.932002 types-protobuf-4.25.0.20240410/google-stubs/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/any_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11250 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/api_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:15:07.932002 types-protobuf-4.25.0.20240410/google-stubs/protobuf/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/compiler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13116 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/compiler/plugin_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9034 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/descriptor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   105834 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/descriptor_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/descriptor_pool.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/duration_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/empty_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/field_mask_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:15:07.936002 types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/api_implementation.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/builder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/containers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/decoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/encoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/enum_type_wrapper.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/extension_dict.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/message_listener.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/python_message.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/type_checkers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/well_known_types.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/wire_format.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/json_format.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/message.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/message_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 02:15:06.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/reflection.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/source_context_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/struct_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/symbol_database.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/text_format.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/timestamp_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16542 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/type_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:15:07.936002 types-protobuf-4.25.0.20240410/google-stubs/protobuf/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/util/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-10 02:14:56.000000 types-protobuf-4.25.0.20240410/google-stubs/protobuf/wrappers_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 02:15:07.936002 types-protobuf-4.25.0.20240410/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-10 02:15:06.000000 types-protobuf-4.25.0.20240410/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 02:15:07.936002 types-protobuf-4.25.0.20240410/types_protobuf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-10 02:15:07.000000 types-protobuf-4.25.0.20240410/types_protobuf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-10 02:15:07.000000 types-protobuf-4.25.0.20240410/types_protobuf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 02:15:07.000000 types-protobuf-4.25.0.20240410/types_protobuf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-10 02:15:07.000000 types-protobuf-4.25.0.20240410/types_protobuf.egg-info/top_level.txt
```

### Comparing `types-protobuf-4.24.0.4/CHANGELOG.md` & `types-protobuf-4.25.0.20240410/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+## 4.25.0.20240410 (2024-04-10)
+
+Bump protobuf to v25.3 (#11694)
+
+## 4.24.0.20240408 (2024-04-08)
+
+Bump protobuf to v24.4 and update generator script (#11693)
+
+## 4.24.0.20240311 (2024-03-11)
+
+Use PEP 570 syntax in third party stubs (#11554)
+
+## 4.24.0.20240302 (2024-03-02)
+
+Add pyupgrade check outdated-version-block (UP036) (#11509)
+
+Co-authored-by: Alex Waygood <Alex.Waygood@Gmail.com>
+
+## 4.24.0.20240106 (2024-01-06)
+
+Bump various test dependencies (#11249)
+
+Update typing_extensions imports in third-party stubs (#11245)
+
 ## 4.24.0.4 (2023-10-29)
 
 Enable ruff's isort rules on files generated using mypy-protobuf (#10939)
 
 Co-authored-by: AlexWaygood <alex.waygood@gmail.com>
 
 ## 4.24.0.3 (2023-10-23)
```

### Comparing `types-protobuf-4.24.0.4/PKG-INFO` & `types-protobuf-4.25.0.20240410/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: types-protobuf
-Version: 4.24.0.4
+Version: 4.25.0.20240410
 Summary: Typing stubs for protobuf
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/protobuf.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ## Typing stubs for protobuf
 
 This is a [PEP 561](https://peps.python.org/pep-0561/)
 type stub package for the [`protobuf`](https://github.com/protocolbuffers/protobuf) package.
 It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `protobuf`.
 
 This version of `types-protobuf` aims to provide accurate annotations
-for `protobuf==4.24.*`.
+for `protobuf==4.25.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/protobuf. All fixes for
 types and metadata should be contributed there.
 
-Generated using [mypy-protobuf==3.5.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.5.0) on protobuf==4.21.8
+Generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) on [protobuf v25.3](https://github.com/protocolbuffers/protobuf/releases/tag/v25.3) (python protobuf==4.25.3)
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `9d345b4df42939b697a84ee461a8760eb674050e` and was tested
-with mypy 1.6.1, pyright 1.1.332, and
-pytype 2023.10.17.
+This package was generated from typeshed commit `1af2babc03ca0cbd248f5f2044e68311a671595f` and was tested
+with mypy 1.9.0, pyright 1.1.357, and
+pytype 2024.3.19.
```

### Comparing `types-protobuf-4.24.0.4/google-stubs/protobuf/any_pb2.pyi` & `types-protobuf-4.25.0.20240410/google-stubs/protobuf/any_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -27,29 +27,25 @@
 SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
 LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
+
 import builtins
-import sys
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.well_known_types
 import google.protobuf.message
 
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
-
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class Any(google.protobuf.message.Message, google.protobuf.internal.well_known_types.Any):
     """`Any` contains an arbitrary serialized protocol buffer message along with a
     URL that describes the type of the serialized message.
 
     Protobuf library provides support to pack/unpack Any values in the form
     of utility functions or additional generated methods of the Any type.
 
@@ -67,26 +63,30 @@
 
         Foo foo = ...;
         Any any = Any.pack(foo);
         ...
         if (any.is(Foo.class)) {
           foo = any.unpack(Foo.class);
         }
+        // or ...
+        if (any.isSameTypeAs(Foo.getDefaultInstance())) {
+          foo = any.unpack(Foo.getDefaultInstance());
+        }
 
-    Example 3: Pack and unpack a message in Python.
+     Example 3: Pack and unpack a message in Python.
 
         foo = Foo(...)
         any = Any()
         any.Pack(foo)
         ...
         if any.Is(Foo.DESCRIPTOR):
           any.Unpack(foo)
           ...
 
-    Example 4: Pack and unpack a message in Go
+     Example 4: Pack and unpack a message in Go
 
          foo := &pb.Foo{...}
          any, err := anypb.New(foo)
          if err != nil {
            ...
          }
          ...
@@ -97,17 +97,16 @@
 
     The pack methods provided by protobuf library will by default use
     'type.googleapis.com/full.type.name' as the type URL and the unpack
     methods only use the fully qualified type name after the last '/'
     in the type URL, for example "foo.bar.com/x/y.z" will yield type
     name "y.z".
 
-
     JSON
-
+    ====
     The JSON representation of an `Any` value uses the regular
     representation of the deserialized, embedded message, with an
     additional field `@type` which contains the type URL. Example:
 
         package google.profile;
         message Person {
           string first_name = 1;
@@ -155,23 +154,24 @@
       URL, or have them precompiled into a binary to avoid any
       lookup. Therefore, binary compatibility needs to be preserved
       on changes to types. (Use versioned type names to manage
       breaking changes.)
 
     Note: this functionality is not currently available in the official
     protobuf release, and it is not used for type URLs beginning with
-    type.googleapis.com.
+    type.googleapis.com. As of May 2023, there are no widely used type server
+    implementations and no plans to implement one.
 
     Schemes other than `http`, `https` (or the empty scheme) might be
     used with implementation specific semantics.
     """
     value: builtins.bytes
     """Must be a valid serialized protocol buffer of the above specified type."""
     def __init__(
         self,
         *,
         type_url: builtins.str | None = ...,
         value: builtins.bytes | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["type_url", b"type_url", "value", b"value"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["type_url", b"type_url", "value", b"value"]) -> None: ...
 
 global___Any = Any
```

### Comparing `types-protobuf-4.24.0.4/google-stubs/protobuf/api_pb2.pyi` & `types-protobuf-4.25.0.20240410/google-stubs/protobuf/api_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -27,32 +27,28 @@
 SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
 LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
+
 import builtins
 import collections.abc
-import sys
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import google.protobuf.source_context_pb2
 import google.protobuf.type_pb2
 
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
-
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class Api(google.protobuf.message.Message):
     """Api is a light-weight descriptor for an API Interface.
 
     Interfaces are also described as "protocol buffer services" in some contexts,
     such as by the "service" keyword in a .proto file, but they are different
     from API Services, which represent a concrete implementation of an interface
     as opposed to simply a description of methods and bindings. They are also
@@ -70,20 +66,14 @@
     SOURCE_CONTEXT_FIELD_NUMBER: builtins.int
     MIXINS_FIELD_NUMBER: builtins.int
     SYNTAX_FIELD_NUMBER: builtins.int
     name: builtins.str
     """The fully qualified name of this interface, including package name
     followed by the interface's simple name.
     """
-    @property
-    def methods(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Method]:
-        """The methods of this interface, in unspecified order."""
-    @property
-    def options(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[google.protobuf.type_pb2.Option]:
-        """Any metadata attached to the interface."""
     version: builtins.str
     """A version string for this interface. If specified, must have the form
     `major-version.minor-version`, as in `1.10`. If the minor version is
     omitted, it defaults to zero. If the entire version field is empty, the
     major version is derived from the package name, as outlined below. If the
     field is not empty, the version in the package name will be verified to be
     consistent with what is provided here.
@@ -97,41 +87,51 @@
 
     The major version is also reflected in the package name of the
     interface, which must end in `v<major-version>`, as in
     `google.feature.v1`. For major versions 0 and 1, the suffix can
     be omitted. Zero major versions must only be used for
     experimental, non-GA interfaces.
     """
+    syntax: google.protobuf.type_pb2.Syntax.ValueType
+    """The source syntax of the service."""
+    @property
+    def methods(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Method]:
+        """The methods of this interface, in unspecified order."""
+
+    @property
+    def options(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[google.protobuf.type_pb2.Option]:
+        """Any metadata attached to the interface."""
+
     @property
     def source_context(self) -> google.protobuf.source_context_pb2.SourceContext:
         """Source context for the protocol buffer service represented by this
         message.
         """
+
     @property
     def mixins(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Mixin]:
         """Included interfaces. See [Mixin][]."""
-    syntax: google.protobuf.type_pb2.Syntax.ValueType
-    """The source syntax of the service."""
+
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         methods: collections.abc.Iterable[global___Method] | None = ...,
         options: collections.abc.Iterable[google.protobuf.type_pb2.Option] | None = ...,
         version: builtins.str | None = ...,
         source_context: google.protobuf.source_context_pb2.SourceContext | None = ...,
         mixins: collections.abc.Iterable[global___Mixin] | None = ...,
         syntax: google.protobuf.type_pb2.Syntax.ValueType | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["source_context", b"source_context"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["methods", b"methods", "mixins", b"mixins", "name", b"name", "options", b"options", "source_context", b"source_context", "syntax", b"syntax", "version", b"version"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["source_context", b"source_context"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["methods", b"methods", "mixins", b"mixins", "name", b"name", "options", b"options", "source_context", b"source_context", "syntax", b"syntax", "version", b"version"]) -> None: ...
 
 global___Api = Api
 
-@typing_extensions.final
+@typing.final
 class Method(google.protobuf.message.Message):
     """Method represents a method of an API interface."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     REQUEST_TYPE_URL_FIELD_NUMBER: builtins.int
@@ -146,35 +146,36 @@
     """A URL of the input message type."""
     request_streaming: builtins.bool
     """If true, the request is streamed."""
     response_type_url: builtins.str
     """The URL of the output message type."""
     response_streaming: builtins.bool
     """If true, the response is streamed."""
+    syntax: google.protobuf.type_pb2.Syntax.ValueType
+    """The source syntax of this method."""
     @property
     def options(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[google.protobuf.type_pb2.Option]:
         """Any metadata attached to the method."""
-    syntax: google.protobuf.type_pb2.Syntax.ValueType
-    """The source syntax of this method."""
+
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         request_type_url: builtins.str | None = ...,
         request_streaming: builtins.bool | None = ...,
         response_type_url: builtins.str | None = ...,
         response_streaming: builtins.bool | None = ...,
         options: collections.abc.Iterable[google.protobuf.type_pb2.Option] | None = ...,
         syntax: google.protobuf.type_pb2.Syntax.ValueType | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "options", b"options", "request_streaming", b"request_streaming", "request_type_url", b"request_type_url", "response_streaming", b"response_streaming", "response_type_url", b"response_type_url", "syntax", b"syntax"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["name", b"name", "options", b"options", "request_streaming", b"request_streaming", "request_type_url", b"request_type_url", "response_streaming", b"response_streaming", "response_type_url", b"response_type_url", "syntax", b"syntax"]) -> None: ...
 
 global___Method = Method
 
-@typing_extensions.final
+@typing.final
 class Mixin(google.protobuf.message.Message):
     """Declares an API Interface to be included in this interface. The including
     interface must redeclare all the methods from the included interface, but
     documentation and options are inherited as follows:
 
     - If after comment and whitespace stripping, the documentation
       string of the redeclared method is empty, it will be inherited
@@ -215,15 +216,15 @@
         - name: google.storage.v2.Storage
           mixins:
           - name: google.acl.v1.AccessControl
 
     The mixin construct implies that all methods in `AccessControl` are
     also declared with same name and request/response types in
     `Storage`. A documentation generator or annotation processor will
-    see the effective `Storage.GetAcl` method after inheriting
+    see the effective `Storage.GetAcl` method after inherting
     documentation and annotations as follows:
 
         service Storage {
           // Get the underlying ACL object.
           rpc GetAcl(GetAclRequest) returns (Acl) {
             option (google.api.http).get = "/v2/{resource=**}:getAcl";
           }
@@ -264,10 +265,10 @@
     """
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         root: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "root", b"root"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["name", b"name", "root", b"root"]) -> None: ...
 
 global___Mixin = Mixin
```

### Comparing `types-protobuf-4.24.0.4/google-stubs/protobuf/compiler/plugin_pb2.pyi` & `types-protobuf-4.25.0.20240410/google-stubs/protobuf/compiler/plugin_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 Author: kenton@google.com (Kenton Varda)
 
-WARNING:  The plugin interface is currently EXPERIMENTAL and is subject to
-  change.
-
 protoc (aka the Protocol Compiler) can be extended via plugins.  A plugin is
 just a program that reads a CodeGeneratorRequest from stdin and writes a
 CodeGeneratorResponse to stdout.
 
 Plugins written using C++ can use google/protobuf/compiler/plugin.h instead
 of dealing with the raw protocol defined here.
 
 A plugin executable needs only to be placed somewhere in the path.  The
 plugin should be named "protoc-gen-$NAME", and will then be used when the
 flag "--${NAME}_out" is passed to protoc.
 """
+
 import builtins
 import collections.abc
 import sys
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.descriptor_pb2
@@ -31,15 +29,15 @@
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class Version(google.protobuf.message.Message):
     """The version number of protocol compiler."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MAJOR_FIELD_NUMBER: builtins.int
     MINOR_FIELD_NUMBER: builtins.int
@@ -56,92 +54,111 @@
         self,
         *,
         major: builtins.int | None = ...,
         minor: builtins.int | None = ...,
         patch: builtins.int | None = ...,
         suffix: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["major", b"major", "minor", b"minor", "patch", b"patch", "suffix", b"suffix"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["major", b"major", "minor", b"minor", "patch", b"patch", "suffix", b"suffix"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["major", b"major", "minor", b"minor", "patch", b"patch", "suffix", b"suffix"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["major", b"major", "minor", b"minor", "patch", b"patch", "suffix", b"suffix"]) -> None: ...
 
 global___Version = Version
 
-@typing_extensions.final
+@typing.final
 class CodeGeneratorRequest(google.protobuf.message.Message):
     """An encoded CodeGeneratorRequest is written to the plugin's stdin."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     FILE_TO_GENERATE_FIELD_NUMBER: builtins.int
     PARAMETER_FIELD_NUMBER: builtins.int
     PROTO_FILE_FIELD_NUMBER: builtins.int
+    SOURCE_FILE_DESCRIPTORS_FIELD_NUMBER: builtins.int
     COMPILER_VERSION_FIELD_NUMBER: builtins.int
+    parameter: builtins.str
+    """The generator parameter passed on the command-line."""
     @property
     def file_to_generate(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """The .proto files that were explicitly listed on the command-line.  The
         code generator should generate code only for these files.  Each file's
         descriptor will be included in proto_file, below.
         """
-    parameter: builtins.str
-    """The generator parameter passed on the command-line."""
+
     @property
     def proto_file(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[google.protobuf.descriptor_pb2.FileDescriptorProto]:
         """FileDescriptorProtos for all files in files_to_generate and everything
         they import.  The files will appear in topological order, so each file
         appears before any file that imports it.
 
+        Note: the files listed in files_to_generate will include runtime-retention
+        options only, but all other files will include source-retention options.
+        The source_file_descriptors field below is available in case you need
+        source-retention options for files_to_generate.
+
         protoc guarantees that all proto_files will be written after
         the fields above, even though this is not technically guaranteed by the
         protobuf wire format.  This theoretically could allow a plugin to stream
         in the FileDescriptorProtos and handle them one by one rather than read
         the entire set into memory at once.  However, as of this writing, this
         is not similarly optimized on protoc's end -- it will store all fields in
         memory at once before sending them to the plugin.
 
         Type names of fields and extensions in the FileDescriptorProto are always
         fully qualified.
         """
+
+    @property
+    def source_file_descriptors(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[google.protobuf.descriptor_pb2.FileDescriptorProto]:
+        """File descriptors with all options, including source-retention options.
+        These descriptors are only provided for the files listed in
+        files_to_generate.
+        """
+
     @property
     def compiler_version(self) -> global___Version:
         """The version number of protocol compiler."""
+
     def __init__(
         self,
         *,
         file_to_generate: collections.abc.Iterable[builtins.str] | None = ...,
         parameter: builtins.str | None = ...,
         proto_file: collections.abc.Iterable[google.protobuf.descriptor_pb2.FileDescriptorProto] | None = ...,
+        source_file_descriptors: collections.abc.Iterable[google.protobuf.descriptor_pb2.FileDescriptorProto] | None = ...,
         compiler_version: global___Version | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["compiler_version", b"compiler_version", "parameter", b"parameter"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["compiler_version", b"compiler_version", "file_to_generate", b"file_to_generate", "parameter", b"parameter", "proto_file", b"proto_file"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["compiler_version", b"compiler_version", "parameter", b"parameter"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["compiler_version", b"compiler_version", "file_to_generate", b"file_to_generate", "parameter", b"parameter", "proto_file", b"proto_file", "source_file_descriptors", b"source_file_descriptors"]) -> None: ...
 
 global___CodeGeneratorRequest = CodeGeneratorRequest
 
-@typing_extensions.final
+@typing.final
 class CodeGeneratorResponse(google.protobuf.message.Message):
     """The plugin writes an encoded CodeGeneratorResponse to stdout."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _Feature:
         ValueType = typing.NewType("ValueType", builtins.int)
         V: typing_extensions.TypeAlias = ValueType
 
     class _FeatureEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[CodeGeneratorResponse._Feature.ValueType], builtins.type):
         DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
         FEATURE_NONE: CodeGeneratorResponse._Feature.ValueType  # 0
         FEATURE_PROTO3_OPTIONAL: CodeGeneratorResponse._Feature.ValueType  # 1
+        FEATURE_SUPPORTS_EDITIONS: CodeGeneratorResponse._Feature.ValueType  # 2
 
     class Feature(_Feature, metaclass=_FeatureEnumTypeWrapper):
         """Sync with code_generator.h."""
 
     FEATURE_NONE: CodeGeneratorResponse.Feature.ValueType  # 0
     FEATURE_PROTO3_OPTIONAL: CodeGeneratorResponse.Feature.ValueType  # 1
+    FEATURE_SUPPORTS_EDITIONS: CodeGeneratorResponse.Feature.ValueType  # 2
 
-    @typing_extensions.final
+    @typing.final
     class File(google.protobuf.message.Message):
         """Represents a single generated file."""
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         NAME_FIELD_NUMBER: builtins.int
         INSERTION_POINT_FIELD_NUMBER: builtins.int
@@ -203,24 +220,25 @@
         """The file contents."""
         @property
         def generated_code_info(self) -> google.protobuf.descriptor_pb2.GeneratedCodeInfo:
             """Information describing the file content being inserted. If an insertion
             point is used, this information will be appropriately offset and inserted
             into the code generation metadata for the generated files.
             """
+
         def __init__(
             self,
             *,
             name: builtins.str | None = ...,
             insertion_point: builtins.str | None = ...,
             content: builtins.str | None = ...,
             generated_code_info: google.protobuf.descriptor_pb2.GeneratedCodeInfo | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["content", b"content", "generated_code_info", b"generated_code_info", "insertion_point", b"insertion_point", "name", b"name"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["content", b"content", "generated_code_info", b"generated_code_info", "insertion_point", b"insertion_point", "name", b"name"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["content", b"content", "generated_code_info", b"generated_code_info", "insertion_point", b"insertion_point", "name", b"name"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["content", b"content", "generated_code_info", b"generated_code_info", "insertion_point", b"insertion_point", "name", b"name"]) -> None: ...
 
     ERROR_FIELD_NUMBER: builtins.int
     SUPPORTED_FEATURES_FIELD_NUMBER: builtins.int
     FILE_FIELD_NUMBER: builtins.int
     error: builtins.str
     """Error message.  If non-empty, code generation failed.  The plugin process
     should exit with status code zero even if it reports an error in this way.
@@ -240,11 +258,11 @@
     def __init__(
         self,
         *,
         error: builtins.str | None = ...,
         supported_features: builtins.int | None = ...,
         file: collections.abc.Iterable[global___CodeGeneratorResponse.File] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["error", b"error", "supported_features", b"supported_features"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["error", b"error", "file", b"file", "supported_features", b"supported_features"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["error", b"error", "supported_features", b"supported_features"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["error", b"error", "file", b"file", "supported_features", b"supported_features"]) -> None: ...
 
 global___CodeGeneratorResponse = CodeGeneratorResponse
```

### Comparing `types-protobuf-4.24.0.4/google-stubs/protobuf/descriptor.pyi` & `types-protobuf-4.25.0.20240410/google-stubs/protobuf/descriptor.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     def __instancecheck__(self, obj: Any) -> bool: ...
 
 _internal_create_key: object
 _USE_C_DESCRIPTORS: bool
 
 class DescriptorBase(metaclass=DescriptorMetaclass):
     has_options: Any
-    def __init__(self, options, serialized_options, options_class_name) -> None: ...
+    def __init__(self, file, options, serialized_options, options_class_name) -> None: ...
     def GetOptions(self): ...
 
 class _NestedDescriptorBase(DescriptorBase):
     name: Any
     full_name: Any
     file: Any
     containing_type: Any
@@ -36,17 +36,17 @@
         self,
         options,
         options_class_name,
         name,
         full_name,
         file,
         containing_type,
-        serialized_start=...,
-        serialized_end=...,
-        serialized_options=...,
+        serialized_start=None,
+        serialized_end=None,
+        serialized_options=None,
     ) -> None: ...
     def CopyToProto(self, proto): ...
 
 class Descriptor(_NestedDescriptorBase):
     fields: Any
     fields_by_number: Any
     fields_by_name: Any
@@ -57,35 +57,37 @@
     enum_values_by_name: Any
     extensions: Any
     extensions_by_name: Any
     is_extendable: Any
     extension_ranges: Any
     oneofs: Any
     oneofs_by_name: Any
-    syntax: Any
+    @property
+    def syntax(self): ...
     def __init__(
         self,
         name: str,
         full_name: str,
         filename: Any,
         containing_type: Descriptor | None,
         fields: list[FieldDescriptor],
         nested_types: list[FieldDescriptor],
         enum_types: list[EnumDescriptor],
         extensions: list[FieldDescriptor],
-        options: Incomplete | None = ...,
-        serialized_options: Incomplete | None = ...,
-        is_extendable: bool | None = ...,
-        extension_ranges: Incomplete | None = ...,
-        oneofs: list[OneofDescriptor] | None = ...,
-        file: FileDescriptor | None = ...,
-        serialized_start: Incomplete | None = ...,
-        serialized_end: Incomplete | None = ...,
-        syntax: str | None = ...,
-        create_key: Incomplete | None = ...,
+        options: Incomplete | None = None,
+        serialized_options: Incomplete | None = None,
+        is_extendable: bool | None = True,
+        extension_ranges: Incomplete | None = None,
+        oneofs: list[OneofDescriptor] | None = None,
+        file: FileDescriptor | None = None,
+        serialized_start: Incomplete | None = None,
+        serialized_end: Incomplete | None = None,
+        syntax: str | None = None,
+        is_map_entry=False,
+        create_key: Incomplete | None = None,
     ): ...
     def EnumValueName(self, enum, value): ...
     def CopyToProto(self, proto): ...
     def GetOptions(self) -> MessageOptions: ...
 
 class FieldDescriptor(DescriptorBase):
     TYPE_DOUBLE: Any
@@ -136,21 +138,21 @@
         label,
         default_value,
         message_type,
         enum_type,
         containing_type,
         is_extension,
         extension_scope,
-        options=...,
-        serialized_options=...,
-        has_default_value=...,
-        containing_oneof=...,
-        json_name=...,
-        file=...,
-        create_key=...,
+        options=None,
+        serialized_options=None,
+        has_default_value=True,
+        containing_oneof=None,
+        json_name=None,
+        file=None,
+        create_key=None,
     ): ...
     name: Any
     full_name: Any
     index: Any
     number: Any
     type: Any
     cpp_type: Any
@@ -174,117 +176,117 @@
         label,
         default_value,
         message_type,
         enum_type,
         containing_type,
         is_extension,
         extension_scope,
-        options=...,
-        serialized_options=...,
-        has_default_value=...,
-        containing_oneof=...,
-        json_name=...,
-        file=...,
-        create_key=...,
+        options=None,
+        serialized_options=None,
+        has_default_value=True,
+        containing_oneof=None,
+        json_name=None,
+        file=None,
+        create_key=None,
     ) -> None: ...
     @staticmethod
     def ProtoTypeToCppProtoType(proto_type): ...
     def GetOptions(self) -> FieldOptions: ...
 
 class EnumDescriptor(_NestedDescriptorBase):
     def __new__(
         cls,
         name,
         full_name,
         filename,
         values,
-        containing_type=...,
-        options=...,
-        serialized_options=...,
-        file=...,
-        serialized_start=...,
-        serialized_end=...,
-        create_key=...,
+        containing_type=None,
+        options=None,
+        serialized_options=None,
+        file=None,
+        serialized_start=None,
+        serialized_end=None,
+        create_key=None,
     ): ...
     values: Any
     values_by_name: Any
     values_by_number: Any
     def __init__(
         self,
         name,
         full_name,
         filename,
         values,
-        containing_type=...,
-        options=...,
-        serialized_options=...,
-        file=...,
-        serialized_start=...,
-        serialized_end=...,
-        create_key=...,
+        containing_type=None,
+        options=None,
+        serialized_options=None,
+        file=None,
+        serialized_start=None,
+        serialized_end=None,
+        create_key=None,
     ) -> None: ...
     def CopyToProto(self, proto): ...
     def GetOptions(self) -> EnumOptions: ...
 
 class EnumValueDescriptor(DescriptorBase):
-    def __new__(cls, name, index, number, type=..., options=..., serialized_options=..., create_key=...): ...
+    def __new__(cls, name, index, number, type=None, options=None, serialized_options=None, create_key=None): ...
     name: Any
     index: Any
     number: Any
     type: Any
-    def __init__(self, name, index, number, type=..., options=..., serialized_options=..., create_key=...) -> None: ...
+    def __init__(self, name, index, number, type=None, options=None, serialized_options=None, create_key=None) -> None: ...
     def GetOptions(self) -> EnumValueOptions: ...
 
 class OneofDescriptor:
-    def __new__(cls, name, full_name, index, containing_type, fields, options=..., serialized_options=..., create_key=...): ...
+    def __new__(cls, name, full_name, index, containing_type, fields, options=None, serialized_options=None, create_key=None): ...
     name: Any
     full_name: Any
     index: Any
     containing_type: Any
     fields: Any
     def __init__(
-        self, name, full_name, index, containing_type, fields, options=..., serialized_options=..., create_key=...
+        self, name, full_name, index, containing_type, fields, options=None, serialized_options=None, create_key=None
     ) -> None: ...
     def GetOptions(self) -> OneofOptions: ...
 
 class ServiceDescriptor(_NestedDescriptorBase):
     index: Any
     methods: Any
     methods_by_name: Any
     def __init__(
         self,
         name: str,
         full_name: str,
         index: int,
         methods: list[MethodDescriptor],
-        options: ServiceOptions | None = ...,
-        serialized_options: Incomplete | None = ...,
-        file: FileDescriptor | None = ...,
-        serialized_start: Incomplete | None = ...,
-        serialized_end: Incomplete | None = ...,
-        create_key: Incomplete | None = ...,
+        options: ServiceOptions | None = None,
+        serialized_options: Incomplete | None = None,
+        file: FileDescriptor | None = None,
+        serialized_start: Incomplete | None = None,
+        serialized_end: Incomplete | None = None,
+        create_key: Incomplete | None = None,
     ): ...
     def FindMethodByName(self, name): ...
     def CopyToProto(self, proto): ...
     def GetOptions(self) -> ServiceOptions: ...
 
 class MethodDescriptor(DescriptorBase):
     def __new__(
         cls,
         name,
         full_name,
         index,
         containing_service,
         input_type,
         output_type,
-        client_streaming=...,
-        server_streaming=...,
-        options=...,
-        serialized_options=...,
-        create_key=...,
+        client_streaming=False,
+        server_streaming=False,
+        options=None,
+        serialized_options=None,
+        create_key=None,
     ): ...
     name: Any
     full_name: Any
     index: Any
     containing_service: Any
     input_type: Any
     output_type: Any
@@ -294,59 +296,60 @@
         self,
         name,
         full_name,
         index,
         containing_service,
         input_type,
         output_type,
-        client_streaming=...,
-        server_streaming=...,
-        options=...,
-        serialized_options=...,
-        create_key=...,
+        client_streaming=False,
+        server_streaming=False,
+        options=None,
+        serialized_options=None,
+        create_key=None,
     ) -> None: ...
     def GetOptions(self) -> MethodOptions: ...
 
 class FileDescriptor(DescriptorBase):
     def __new__(
         cls,
         name,
         package,
-        options=...,
-        serialized_options=...,
-        serialized_pb=...,
-        dependencies=...,
-        public_dependencies=...,
-        syntax=...,
-        pool=...,
-        create_key=...,
+        options=None,
+        serialized_options=None,
+        serialized_pb=None,
+        dependencies=None,
+        public_dependencies=None,
+        syntax=None,
+        pool=None,
+        create_key=None,
     ): ...
     _options: Any
     pool: Any
     message_types_by_name: Any
     name: Any
     package: Any
-    syntax: Any
+    @property
+    def syntax(self): ...
     serialized_pb: Any
     enum_types_by_name: Any
     extensions_by_name: Any
     services_by_name: Any
     dependencies: Any
     public_dependencies: Any
     def __init__(
         self,
         name,
         package,
-        options=...,
-        serialized_options=...,
-        serialized_pb=...,
-        dependencies=...,
-        public_dependencies=...,
-        syntax=...,
-        pool=...,
-        create_key=...,
+        options=None,
+        serialized_options=None,
+        serialized_pb=None,
+        dependencies=None,
+        public_dependencies=None,
+        syntax=None,
+        pool=None,
+        create_key=None,
     ) -> None: ...
     def CopyToProto(self, proto): ...
     def GetOptions(self) -> FileOptions: ...
 
-def MakeDescriptor(desc_proto, package=..., build_file_if_cpp=..., syntax=...): ...
+def MakeDescriptor(desc_proto, package="", build_file_if_cpp=True, syntax=None): ...
 def _ParseOptions(message: Message, string: bytes) -> Message: ...
```

### Comparing `types-protobuf-4.24.0.4/google-stubs/protobuf/descriptor_pb2.pyi` & `types-protobuf-4.25.0.20240410/google-stubs/protobuf/descriptor_pb2.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -5,14 +5,15 @@
  Based on original Protocol Buffers design by
  Sanjay Ghemawat, Jeff Dean, and others.
 
 The messages in this file describe the definitions found in .proto files.
 A valid .proto file can be translated directly to a FileDescriptorProto
 without any other information (e.g. without reading its imports).
 """
+
 import builtins
 import collections.abc
 import sys
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
@@ -22,15 +23,71 @@
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+class _Edition:
+    ValueType = typing.NewType("ValueType", builtins.int)
+    V: typing_extensions.TypeAlias = ValueType
+
+class _EditionEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_Edition.ValueType], builtins.type):
+    DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+    EDITION_UNKNOWN: _Edition.ValueType  # 0
+    """A placeholder for an unknown edition value."""
+    EDITION_PROTO2: _Edition.ValueType  # 998
+    """Legacy syntax "editions".  These pre-date editions, but behave much like
+    distinct editions.  These can't be used to specify the edition of proto
+    files, but feature definitions must supply proto2/proto3 defaults for
+    backwards compatibility.
+    """
+    EDITION_PROTO3: _Edition.ValueType  # 999
+    EDITION_2023: _Edition.ValueType  # 1000
+    """Editions that have been released.  The specific values are arbitrary and
+    should not be depended on, but they will always be time-ordered for easy
+    comparison.
+    """
+    EDITION_1_TEST_ONLY: _Edition.ValueType  # 1
+    """Placeholder editions for testing feature resolution.  These should not be
+    used or relyed on outside of tests.
+    """
+    EDITION_2_TEST_ONLY: _Edition.ValueType  # 2
+    EDITION_99997_TEST_ONLY: _Edition.ValueType  # 99997
+    EDITION_99998_TEST_ONLY: _Edition.ValueType  # 99998
+    EDITION_99999_TEST_ONLY: _Edition.ValueType  # 99999
+
+class Edition(_Edition, metaclass=_EditionEnumTypeWrapper):
+    """The full set of known editions."""
+
+EDITION_UNKNOWN: Edition.ValueType  # 0
+"""A placeholder for an unknown edition value."""
+EDITION_PROTO2: Edition.ValueType  # 998
+"""Legacy syntax "editions".  These pre-date editions, but behave much like
+distinct editions.  These can't be used to specify the edition of proto
+files, but feature definitions must supply proto2/proto3 defaults for
+backwards compatibility.
+"""
+EDITION_PROTO3: Edition.ValueType  # 999
+EDITION_2023: Edition.ValueType  # 1000
+"""Editions that have been released.  The specific values are arbitrary and
+should not be depended on, but they will always be time-ordered for easy
+comparison.
+"""
+EDITION_1_TEST_ONLY: Edition.ValueType  # 1
+"""Placeholder editions for testing feature resolution.  These should not be
+used or relyed on outside of tests.
+"""
+EDITION_2_TEST_ONLY: Edition.ValueType  # 2
+EDITION_99997_TEST_ONLY: Edition.ValueType  # 99997
+EDITION_99998_TEST_ONLY: Edition.ValueType  # 99998
+EDITION_99999_TEST_ONLY: Edition.ValueType  # 99999
+global___Edition = Edition
+
+@typing.final
 class FileDescriptorSet(google.protobuf.message.Message):
     """The protocol compiler can output a FileDescriptorSet containing the .proto
     files it parses.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -38,19 +95,19 @@
     @property
     def file(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___FileDescriptorProto]: ...
     def __init__(
         self,
         *,
         file: collections.abc.Iterable[global___FileDescriptorProto] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["file", b"file"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["file", b"file"]) -> None: ...
 
 global___FileDescriptorSet = FileDescriptorSet
 
-@typing_extensions.final
+@typing.final
 class FileDescriptorProto(google.protobuf.message.Message):
     """Describes a complete .proto file."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     PACKAGE_FIELD_NUMBER: builtins.int
@@ -60,32 +117,45 @@
     MESSAGE_TYPE_FIELD_NUMBER: builtins.int
     ENUM_TYPE_FIELD_NUMBER: builtins.int
     SERVICE_FIELD_NUMBER: builtins.int
     EXTENSION_FIELD_NUMBER: builtins.int
     OPTIONS_FIELD_NUMBER: builtins.int
     SOURCE_CODE_INFO_FIELD_NUMBER: builtins.int
     SYNTAX_FIELD_NUMBER: builtins.int
+    EDITION_FIELD_NUMBER: builtins.int
     name: builtins.str
     """file name, relative to root of source tree"""
     package: builtins.str
     """e.g. "foo", "foo.bar", etc."""
+    syntax: builtins.str
+    """The syntax of the proto file.
+    The supported values are "proto2", "proto3", and "editions".
+
+    If `edition` is present, this value must be "editions".
+    """
+    edition: global___Edition.ValueType
+    """The edition of the proto file."""
     @property
     def dependency(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """Names of files imported by this file."""
+
     @property
     def public_dependency(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """Indexes of the public imported files in the dependency list above."""
+
     @property
     def weak_dependency(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """Indexes of the weak imported files in the dependency list.
         For Google-internal migration only. Do not use.
         """
+
     @property
     def message_type(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___DescriptorProto]:
         """All top-level definitions in this file."""
+
     @property
     def enum_type(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___EnumDescriptorProto]: ...
     @property
     def service(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ServiceDescriptorProto]: ...
     @property
     def extension(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___FieldDescriptorProto]: ...
     @property
@@ -93,18 +163,15 @@
     @property
     def source_code_info(self) -> global___SourceCodeInfo:
         """This field contains optional information about the original source code.
         You may safely remove this entire field without harming runtime
         functionality of the descriptors -- the information is needed only by
         development tools.
         """
-    syntax: builtins.str
-    """The syntax of the proto file.
-    The supported values are "proto2" and "proto3".
-    """
+
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         package: builtins.str | None = ...,
         dependency: collections.abc.Iterable[builtins.str] | None = ...,
         public_dependency: collections.abc.Iterable[builtins.int] | None = ...,
@@ -112,27 +179,28 @@
         message_type: collections.abc.Iterable[global___DescriptorProto] | None = ...,
         enum_type: collections.abc.Iterable[global___EnumDescriptorProto] | None = ...,
         service: collections.abc.Iterable[global___ServiceDescriptorProto] | None = ...,
         extension: collections.abc.Iterable[global___FieldDescriptorProto] | None = ...,
         options: global___FileOptions | None = ...,
         source_code_info: global___SourceCodeInfo | None = ...,
         syntax: builtins.str | None = ...,
+        edition: global___Edition.ValueType | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["name", b"name", "options", b"options", "package", b"package", "source_code_info", b"source_code_info", "syntax", b"syntax"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["dependency", b"dependency", "enum_type", b"enum_type", "extension", b"extension", "message_type", b"message_type", "name", b"name", "options", b"options", "package", b"package", "public_dependency", b"public_dependency", "service", b"service", "source_code_info", b"source_code_info", "syntax", b"syntax", "weak_dependency", b"weak_dependency"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["edition", b"edition", "name", b"name", "options", b"options", "package", b"package", "source_code_info", b"source_code_info", "syntax", b"syntax"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["dependency", b"dependency", "edition", b"edition", "enum_type", b"enum_type", "extension", b"extension", "message_type", b"message_type", "name", b"name", "options", b"options", "package", b"package", "public_dependency", b"public_dependency", "service", b"service", "source_code_info", b"source_code_info", "syntax", b"syntax", "weak_dependency", b"weak_dependency"]) -> None: ...
 
 global___FileDescriptorProto = FileDescriptorProto
 
-@typing_extensions.final
+@typing.final
 class DescriptorProto(google.protobuf.message.Message):
     """Describes a message type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class ExtensionRange(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         START_FIELD_NUMBER: builtins.int
         END_FIELD_NUMBER: builtins.int
         OPTIONS_FIELD_NUMBER: builtins.int
         start: builtins.int
@@ -144,18 +212,18 @@
         def __init__(
             self,
             *,
             start: builtins.int | None = ...,
             end: builtins.int | None = ...,
             options: global___ExtensionRangeOptions | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["end", b"end", "options", b"options", "start", b"start"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["end", b"end", "options", b"options", "start", b"start"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["end", b"end", "options", b"options", "start", b"start"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["end", b"end", "options", b"options", "start", b"start"]) -> None: ...
 
-    @typing_extensions.final
+    @typing.final
     class ReservedRange(google.protobuf.message.Message):
         """Range of reserved tag numbers. Reserved tag numbers may not be used by
         fields or extension ranges in the same message. Reserved ranges may
         not overlap.
         """
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -168,16 +236,16 @@
         """Exclusive."""
         def __init__(
             self,
             *,
             start: builtins.int | None = ...,
             end: builtins.int | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["end", b"end", "start", b"start"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["end", b"end", "start", b"start"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["end", b"end", "start", b"start"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["end", b"end", "start", b"start"]) -> None: ...
 
     NAME_FIELD_NUMBER: builtins.int
     FIELD_FIELD_NUMBER: builtins.int
     EXTENSION_FIELD_NUMBER: builtins.int
     NESTED_TYPE_FIELD_NUMBER: builtins.int
     ENUM_TYPE_FIELD_NUMBER: builtins.int
     EXTENSION_RANGE_FIELD_NUMBER: builtins.int
@@ -203,51 +271,134 @@
     @property
     def reserved_range(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___DescriptorProto.ReservedRange]: ...
     @property
     def reserved_name(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """Reserved field names, which may not be used by fields in the same message.
         A given name may only be reserved once.
         """
+
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         field: collections.abc.Iterable[global___FieldDescriptorProto] | None = ...,
         extension: collections.abc.Iterable[global___FieldDescriptorProto] | None = ...,
         nested_type: collections.abc.Iterable[global___DescriptorProto] | None = ...,
         enum_type: collections.abc.Iterable[global___EnumDescriptorProto] | None = ...,
         extension_range: collections.abc.Iterable[global___DescriptorProto.ExtensionRange] | None = ...,
         oneof_decl: collections.abc.Iterable[global___OneofDescriptorProto] | None = ...,
         options: global___MessageOptions | None = ...,
         reserved_range: collections.abc.Iterable[global___DescriptorProto.ReservedRange] | None = ...,
         reserved_name: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["name", b"name", "options", b"options"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["enum_type", b"enum_type", "extension", b"extension", "extension_range", b"extension_range", "field", b"field", "name", b"name", "nested_type", b"nested_type", "oneof_decl", b"oneof_decl", "options", b"options", "reserved_name", b"reserved_name", "reserved_range", b"reserved_range"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["name", b"name", "options", b"options"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["enum_type", b"enum_type", "extension", b"extension", "extension_range", b"extension_range", "field", b"field", "name", b"name", "nested_type", b"nested_type", "oneof_decl", b"oneof_decl", "options", b"options", "reserved_name", b"reserved_name", "reserved_range", b"reserved_range"]) -> None: ...
 
 global___DescriptorProto = DescriptorProto
 
-@typing_extensions.final
+@typing.final
 class ExtensionRangeOptions(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    class _VerificationState:
+        ValueType = typing.NewType("ValueType", builtins.int)
+        V: typing_extensions.TypeAlias = ValueType
+
+    class _VerificationStateEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[ExtensionRangeOptions._VerificationState.ValueType], builtins.type):
+        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+        DECLARATION: ExtensionRangeOptions._VerificationState.ValueType  # 0
+        """All the extensions of the range must be declared."""
+        UNVERIFIED: ExtensionRangeOptions._VerificationState.ValueType  # 1
+
+    class VerificationState(_VerificationState, metaclass=_VerificationStateEnumTypeWrapper):
+        """The verification state of the extension range."""
+
+    DECLARATION: ExtensionRangeOptions.VerificationState.ValueType  # 0
+    """All the extensions of the range must be declared."""
+    UNVERIFIED: ExtensionRangeOptions.VerificationState.ValueType  # 1
+
+    @typing.final
+    class Declaration(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        NUMBER_FIELD_NUMBER: builtins.int
+        FULL_NAME_FIELD_NUMBER: builtins.int
+        TYPE_FIELD_NUMBER: builtins.int
+        RESERVED_FIELD_NUMBER: builtins.int
+        REPEATED_FIELD_NUMBER: builtins.int
+        number: builtins.int
+        """The extension number declared within the extension range."""
+        full_name: builtins.str
+        """The fully-qualified name of the extension field. There must be a leading
+        dot in front of the full name.
+        """
+        type: builtins.str
+        """The fully-qualified type name of the extension field. Unlike
+        Metadata.type, Declaration.type must have a leading dot for messages
+        and enums.
+        """
+        reserved: builtins.bool
+        """If true, indicates that the number is reserved in the extension range,
+        and any extension field with the number will fail to compile. Set this
+        when a declared extension field is deleted.
+        """
+        repeated: builtins.bool
+        """If true, indicates that the extension must be defined as repeated.
+        Otherwise the extension must be defined as optional.
+        """
+        def __init__(
+            self,
+            *,
+            number: builtins.int | None = ...,
+            full_name: builtins.str | None = ...,
+            type: builtins.str | None = ...,
+            reserved: builtins.bool | None = ...,
+            repeated: builtins.bool | None = ...,
+        ) -> None: ...
+        def HasField(self, field_name: typing.Literal["full_name", b"full_name", "number", b"number", "repeated", b"repeated", "reserved", b"reserved", "type", b"type"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["full_name", b"full_name", "number", b"number", "repeated", b"repeated", "reserved", b"reserved", "type", b"type"]) -> None: ...
+
     UNINTERPRETED_OPTION_FIELD_NUMBER: builtins.int
+    DECLARATION_FIELD_NUMBER: builtins.int
+    FEATURES_FIELD_NUMBER: builtins.int
+    VERIFICATION_FIELD_NUMBER: builtins.int
+    verification: global___ExtensionRangeOptions.VerificationState.ValueType
+    """The verification state of the range.
+    TODO: flip the default to DECLARATION once all empty ranges
+    are marked as UNVERIFIED.
+    """
     @property
     def uninterpreted_option(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___UninterpretedOption]:
         """The parser stores options it doesn't recognize here. See above."""
+
+    @property
+    def declaration(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ExtensionRangeOptions.Declaration]:
+        """For external users: DO NOT USE. We are in the process of open sourcing
+        extension declaration and executing internal cleanups before it can be
+        used externally.
+        """
+
+    @property
+    def features(self) -> global___FeatureSet:
+        """Any features defined in the specific edition."""
+
     def __init__(
         self,
         *,
         uninterpreted_option: collections.abc.Iterable[global___UninterpretedOption] | None = ...,
+        declaration: collections.abc.Iterable[global___ExtensionRangeOptions.Declaration] | None = ...,
+        features: global___FeatureSet | None = ...,
+        verification: global___ExtensionRangeOptions.VerificationState.ValueType | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["uninterpreted_option", b"uninterpreted_option"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["features", b"features", "verification", b"verification"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["declaration", b"declaration", "features", b"features", "uninterpreted_option", b"uninterpreted_option", "verification", b"verification"]) -> None: ...
 
 global___ExtensionRangeOptions = ExtensionRangeOptions
 
-@typing_extensions.final
+@typing.final
 class FieldDescriptorProto(google.protobuf.message.Message):
     """Describes a field within a message."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _Type:
         ValueType = typing.NewType("ValueType", builtins.int)
@@ -271,17 +422,18 @@
         """
         TYPE_FIXED64: FieldDescriptorProto._Type.ValueType  # 6
         TYPE_FIXED32: FieldDescriptorProto._Type.ValueType  # 7
         TYPE_BOOL: FieldDescriptorProto._Type.ValueType  # 8
         TYPE_STRING: FieldDescriptorProto._Type.ValueType  # 9
         TYPE_GROUP: FieldDescriptorProto._Type.ValueType  # 10
         """Tag-delimited aggregate.
-        Group type is deprecated and not supported in proto3. However, Proto3
+        Group type is deprecated and not supported after google.protobuf. However, Proto3
         implementations should still be able to parse the group wire format and
-        treat group fields as unknown fields.
+        treat group fields as unknown fields.  In Editions, the group wire format
+        can be enabled via the `message_encoding` feature.
         """
         TYPE_MESSAGE: FieldDescriptorProto._Type.ValueType  # 11
         """Length-delimited aggregate."""
         TYPE_BYTES: FieldDescriptorProto._Type.ValueType  # 12
         """New in version 2."""
         TYPE_UINT32: FieldDescriptorProto._Type.ValueType  # 13
         TYPE_ENUM: FieldDescriptorProto._Type.ValueType  # 14
@@ -309,17 +461,18 @@
     """
     TYPE_FIXED64: FieldDescriptorProto.Type.ValueType  # 6
     TYPE_FIXED32: FieldDescriptorProto.Type.ValueType  # 7
     TYPE_BOOL: FieldDescriptorProto.Type.ValueType  # 8
     TYPE_STRING: FieldDescriptorProto.Type.ValueType  # 9
     TYPE_GROUP: FieldDescriptorProto.Type.ValueType  # 10
     """Tag-delimited aggregate.
-    Group type is deprecated and not supported in proto3. However, Proto3
+    Group type is deprecated and not supported after google.protobuf. However, Proto3
     implementations should still be able to parse the group wire format and
-    treat group fields as unknown fields.
+    treat group fields as unknown fields.  In Editions, the group wire format
+    can be enabled via the `message_encoding` feature.
     """
     TYPE_MESSAGE: FieldDescriptorProto.Type.ValueType  # 11
     """Length-delimited aggregate."""
     TYPE_BYTES: FieldDescriptorProto.Type.ValueType  # 12
     """New in version 2."""
     TYPE_UINT32: FieldDescriptorProto.Type.ValueType  # 13
     TYPE_ENUM: FieldDescriptorProto.Type.ValueType  # 14
@@ -334,22 +487,30 @@
         ValueType = typing.NewType("ValueType", builtins.int)
         V: typing_extensions.TypeAlias = ValueType
 
     class _LabelEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[FieldDescriptorProto._Label.ValueType], builtins.type):
         DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
         LABEL_OPTIONAL: FieldDescriptorProto._Label.ValueType  # 1
         """0 is reserved for errors"""
-        LABEL_REQUIRED: FieldDescriptorProto._Label.ValueType  # 2
         LABEL_REPEATED: FieldDescriptorProto._Label.ValueType  # 3
+        LABEL_REQUIRED: FieldDescriptorProto._Label.ValueType  # 2
+        """The required label is only allowed in google.protobuf.  In proto3 and Editions
+        it's explicitly prohibited.  In Editions, the `field_presence` feature
+        can be used to get this behavior.
+        """
 
     class Label(_Label, metaclass=_LabelEnumTypeWrapper): ...
     LABEL_OPTIONAL: FieldDescriptorProto.Label.ValueType  # 1
     """0 is reserved for errors"""
-    LABEL_REQUIRED: FieldDescriptorProto.Label.ValueType  # 2
     LABEL_REPEATED: FieldDescriptorProto.Label.ValueType  # 3
+    LABEL_REQUIRED: FieldDescriptorProto.Label.ValueType  # 2
+    """The required label is only allowed in google.protobuf.  In proto3 and Editions
+    it's explicitly prohibited.  In Editions, the `field_presence` feature
+    can be used to get this behavior.
+    """
 
     NAME_FIELD_NUMBER: builtins.int
     NUMBER_FIELD_NUMBER: builtins.int
     LABEL_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     TYPE_NAME_FIELD_NUMBER: builtins.int
     EXTENDEE_FIELD_NUMBER: builtins.int
@@ -388,16 +549,14 @@
     """
     json_name: builtins.str
     """JSON name of this field. The value is set by protocol compiler. If the
     user has set a "json_name" option on this field, that option's value
     will be used. Otherwise, it's deduced from the field's name by converting
     it to camelCase.
     """
-    @property
-    def options(self) -> global___FieldOptions: ...
     proto3_optional: builtins.bool
     """If true, this is a proto3 "optional". When a proto3 field is optional, it
     tracks presence regardless of field type.
 
     When proto3_optional is true, this field must be belong to a oneof to
     signal to old proto3 clients that presence is tracked for this field. This
     oneof is known as a "synthetic" oneof, and this field must be its sole
@@ -413,14 +572,16 @@
     to track presence. This is especially important because the parser can't
     tell if a field is a message or an enum, so it must always create a
     synthetic oneof.
 
     Proto2 optional fields do not set this flag, because they already indicate
     optional with `LABEL_OPTIONAL`.
     """
+    @property
+    def options(self) -> global___FieldOptions: ...
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         number: builtins.int | None = ...,
         label: global___FieldDescriptorProto.Label.ValueType | None = ...,
         type: global___FieldDescriptorProto.Type.ValueType | None = ...,
@@ -428,20 +589,20 @@
         extendee: builtins.str | None = ...,
         default_value: builtins.str | None = ...,
         oneof_index: builtins.int | None = ...,
         json_name: builtins.str | None = ...,
         options: global___FieldOptions | None = ...,
         proto3_optional: builtins.bool | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["default_value", b"default_value", "extendee", b"extendee", "json_name", b"json_name", "label", b"label", "name", b"name", "number", b"number", "oneof_index", b"oneof_index", "options", b"options", "proto3_optional", b"proto3_optional", "type", b"type", "type_name", b"type_name"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["default_value", b"default_value", "extendee", b"extendee", "json_name", b"json_name", "label", b"label", "name", b"name", "number", b"number", "oneof_index", b"oneof_index", "options", b"options", "proto3_optional", b"proto3_optional", "type", b"type", "type_name", b"type_name"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["default_value", b"default_value", "extendee", b"extendee", "json_name", b"json_name", "label", b"label", "name", b"name", "number", b"number", "oneof_index", b"oneof_index", "options", b"options", "proto3_optional", b"proto3_optional", "type", b"type", "type_name", b"type_name"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["default_value", b"default_value", "extendee", b"extendee", "json_name", b"json_name", "label", b"label", "name", b"name", "number", b"number", "oneof_index", b"oneof_index", "options", b"options", "proto3_optional", b"proto3_optional", "type", b"type", "type_name", b"type_name"]) -> None: ...
 
 global___FieldDescriptorProto = FieldDescriptorProto
 
-@typing_extensions.final
+@typing.final
 class OneofDescriptorProto(google.protobuf.message.Message):
     """Describes a oneof."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     OPTIONS_FIELD_NUMBER: builtins.int
@@ -450,26 +611,26 @@
     def options(self) -> global___OneofOptions: ...
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         options: global___OneofOptions | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["name", b"name", "options", b"options"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "options", b"options"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["name", b"name", "options", b"options"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["name", b"name", "options", b"options"]) -> None: ...
 
 global___OneofDescriptorProto = OneofDescriptorProto
 
-@typing_extensions.final
+@typing.final
 class EnumDescriptorProto(google.protobuf.message.Message):
     """Describes an enum type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class EnumReservedRange(google.protobuf.message.Message):
         """Range of reserved numeric values. Reserved values may not be used by
         entries in the same enum. Reserved ranges may not overlap.
 
         Note that this is distinct from DescriptorProto.ReservedRange in that it
         is inclusive such that it can appropriately represent the entire int32
         domain.
@@ -485,16 +646,16 @@
         """Inclusive."""
         def __init__(
             self,
             *,
             start: builtins.int | None = ...,
             end: builtins.int | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["end", b"end", "start", b"start"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["end", b"end", "start", b"start"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["end", b"end", "start", b"start"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["end", b"end", "start", b"start"]) -> None: ...
 
     NAME_FIELD_NUMBER: builtins.int
     VALUE_FIELD_NUMBER: builtins.int
     OPTIONS_FIELD_NUMBER: builtins.int
     RESERVED_RANGE_FIELD_NUMBER: builtins.int
     RESERVED_NAME_FIELD_NUMBER: builtins.int
     name: builtins.str
@@ -504,34 +665,36 @@
     def options(self) -> global___EnumOptions: ...
     @property
     def reserved_range(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___EnumDescriptorProto.EnumReservedRange]:
         """Range of reserved numeric values. Reserved numeric values may not be used
         by enum values in the same enum declaration. Reserved ranges may not
         overlap.
         """
+
     @property
     def reserved_name(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """Reserved enum value names, which may not be reused. A given name may only
         be reserved once.
         """
+
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         value: collections.abc.Iterable[global___EnumValueDescriptorProto] | None = ...,
         options: global___EnumOptions | None = ...,
         reserved_range: collections.abc.Iterable[global___EnumDescriptorProto.EnumReservedRange] | None = ...,
         reserved_name: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["name", b"name", "options", b"options"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "options", b"options", "reserved_name", b"reserved_name", "reserved_range", b"reserved_range", "value", b"value"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["name", b"name", "options", b"options"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["name", b"name", "options", b"options", "reserved_name", b"reserved_name", "reserved_range", b"reserved_range", "value", b"value"]) -> None: ...
 
 global___EnumDescriptorProto = EnumDescriptorProto
 
-@typing_extensions.final
+@typing.final
 class EnumValueDescriptorProto(google.protobuf.message.Message):
     """Describes a value within an enum."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     NUMBER_FIELD_NUMBER: builtins.int
@@ -543,20 +706,20 @@
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         number: builtins.int | None = ...,
         options: global___EnumValueOptions | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["name", b"name", "number", b"number", "options", b"options"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "number", b"number", "options", b"options"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["name", b"name", "number", b"number", "options", b"options"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["name", b"name", "number", b"number", "options", b"options"]) -> None: ...
 
 global___EnumValueDescriptorProto = EnumValueDescriptorProto
 
-@typing_extensions.final
+@typing.final
 class ServiceDescriptorProto(google.protobuf.message.Message):
     """Describes a service."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     METHOD_FIELD_NUMBER: builtins.int
@@ -569,20 +732,20 @@
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         method: collections.abc.Iterable[global___MethodDescriptorProto] | None = ...,
         options: global___ServiceOptions | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["name", b"name", "options", b"options"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["method", b"method", "name", b"name", "options", b"options"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["name", b"name", "options", b"options"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["method", b"method", "name", b"name", "options", b"options"]) -> None: ...
 
 global___ServiceDescriptorProto = ServiceDescriptorProto
 
-@typing_extensions.final
+@typing.final
 class MethodDescriptorProto(google.protobuf.message.Message):
     """Describes a method of a service."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     INPUT_TYPE_FIELD_NUMBER: builtins.int
@@ -592,36 +755,36 @@
     SERVER_STREAMING_FIELD_NUMBER: builtins.int
     name: builtins.str
     input_type: builtins.str
     """Input and output type names.  These are resolved in the same way as
     FieldDescriptorProto.type_name, but must refer to a message type.
     """
     output_type: builtins.str
-    @property
-    def options(self) -> global___MethodOptions: ...
     client_streaming: builtins.bool
     """Identifies if client streams multiple client messages"""
     server_streaming: builtins.bool
     """Identifies if server streams multiple server messages"""
+    @property
+    def options(self) -> global___MethodOptions: ...
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         input_type: builtins.str | None = ...,
         output_type: builtins.str | None = ...,
         options: global___MethodOptions | None = ...,
         client_streaming: builtins.bool | None = ...,
         server_streaming: builtins.bool | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["client_streaming", b"client_streaming", "input_type", b"input_type", "name", b"name", "options", b"options", "output_type", b"output_type", "server_streaming", b"server_streaming"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["client_streaming", b"client_streaming", "input_type", b"input_type", "name", b"name", "options", b"options", "output_type", b"output_type", "server_streaming", b"server_streaming"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["client_streaming", b"client_streaming", "input_type", b"input_type", "name", b"name", "options", b"options", "output_type", b"output_type", "server_streaming", b"server_streaming"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["client_streaming", b"client_streaming", "input_type", b"input_type", "name", b"name", "options", b"options", "output_type", b"output_type", "server_streaming", b"server_streaming"]) -> None: ...
 
 global___MethodDescriptorProto = MethodDescriptorProto
 
-@typing_extensions.final
+@typing.final
 class FileOptions(google.protobuf.message.Message):
     """Each of the definitions above may have "options" attached.  These are
     just annotations which may cause code to be generated slightly differently
     or may contain hints for code that manipulates protocol messages.
 
     Clients may define custom options as extensions of the *Options messages.
     These extensions may not yet be known at parsing time, so the parser cannot
@@ -694,14 +857,15 @@
     OBJC_CLASS_PREFIX_FIELD_NUMBER: builtins.int
     CSHARP_NAMESPACE_FIELD_NUMBER: builtins.int
     SWIFT_PREFIX_FIELD_NUMBER: builtins.int
     PHP_CLASS_PREFIX_FIELD_NUMBER: builtins.int
     PHP_NAMESPACE_FIELD_NUMBER: builtins.int
     PHP_METADATA_NAMESPACE_FIELD_NUMBER: builtins.int
     RUBY_PACKAGE_FIELD_NUMBER: builtins.int
+    FEATURES_FIELD_NUMBER: builtins.int
     UNINTERPRETED_OPTION_FIELD_NUMBER: builtins.int
     java_package: builtins.str
     """Sets the Java package where classes generated from this .proto will be
     placed.  By default, the proto package is used, but this is often
     inappropriate because proto packages do not normally start with backwards
     domain names.
     """
@@ -791,18 +955,23 @@
     """
     ruby_package: builtins.str
     """Use this option to change the package of ruby generated classes. Default
     is empty. When this option is not set, the package name will be used for
     determining the ruby package.
     """
     @property
+    def features(self) -> global___FeatureSet:
+        """Any features defined in the specific edition."""
+
+    @property
     def uninterpreted_option(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___UninterpretedOption]:
         """The parser stores options it doesn't recognize here.
         See the documentation for the "Options" section above.
         """
+
     def __init__(
         self,
         *,
         java_package: builtins.str | None = ...,
         java_outer_classname: builtins.str | None = ...,
         java_multiple_files: builtins.bool | None = ...,
         java_generate_equals_and_hash: builtins.bool | None = ...,
@@ -818,29 +987,32 @@
         objc_class_prefix: builtins.str | None = ...,
         csharp_namespace: builtins.str | None = ...,
         swift_prefix: builtins.str | None = ...,
         php_class_prefix: builtins.str | None = ...,
         php_namespace: builtins.str | None = ...,
         php_metadata_namespace: builtins.str | None = ...,
         ruby_package: builtins.str | None = ...,
+        features: global___FeatureSet | None = ...,
         uninterpreted_option: collections.abc.Iterable[global___UninterpretedOption] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["cc_enable_arenas", b"cc_enable_arenas", "cc_generic_services", b"cc_generic_services", "csharp_namespace", b"csharp_namespace", "deprecated", b"deprecated", "go_package", b"go_package", "java_generate_equals_and_hash", b"java_generate_equals_and_hash", "java_generic_services", b"java_generic_services", "java_multiple_files", b"java_multiple_files", "java_outer_classname", b"java_outer_classname", "java_package", b"java_package", "java_string_check_utf8", b"java_string_check_utf8", "objc_class_prefix", b"objc_class_prefix", "optimize_for", b"optimize_for", "php_class_prefix", b"php_class_prefix", "php_generic_services", b"php_generic_services", "php_metadata_namespace", b"php_metadata_namespace", "php_namespace", b"php_namespace", "py_generic_services", b"py_generic_services", "ruby_package", b"ruby_package", "swift_prefix", b"swift_prefix"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cc_enable_arenas", b"cc_enable_arenas", "cc_generic_services", b"cc_generic_services", "csharp_namespace", b"csharp_namespace", "deprecated", b"deprecated", "go_package", b"go_package", "java_generate_equals_and_hash", b"java_generate_equals_and_hash", "java_generic_services", b"java_generic_services", "java_multiple_files", b"java_multiple_files", "java_outer_classname", b"java_outer_classname", "java_package", b"java_package", "java_string_check_utf8", b"java_string_check_utf8", "objc_class_prefix", b"objc_class_prefix", "optimize_for", b"optimize_for", "php_class_prefix", b"php_class_prefix", "php_generic_services", b"php_generic_services", "php_metadata_namespace", b"php_metadata_namespace", "php_namespace", b"php_namespace", "py_generic_services", b"py_generic_services", "ruby_package", b"ruby_package", "swift_prefix", b"swift_prefix", "uninterpreted_option", b"uninterpreted_option"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["cc_enable_arenas", b"cc_enable_arenas", "cc_generic_services", b"cc_generic_services", "csharp_namespace", b"csharp_namespace", "deprecated", b"deprecated", "features", b"features", "go_package", b"go_package", "java_generate_equals_and_hash", b"java_generate_equals_and_hash", "java_generic_services", b"java_generic_services", "java_multiple_files", b"java_multiple_files", "java_outer_classname", b"java_outer_classname", "java_package", b"java_package", "java_string_check_utf8", b"java_string_check_utf8", "objc_class_prefix", b"objc_class_prefix", "optimize_for", b"optimize_for", "php_class_prefix", b"php_class_prefix", "php_generic_services", b"php_generic_services", "php_metadata_namespace", b"php_metadata_namespace", "php_namespace", b"php_namespace", "py_generic_services", b"py_generic_services", "ruby_package", b"ruby_package", "swift_prefix", b"swift_prefix"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["cc_enable_arenas", b"cc_enable_arenas", "cc_generic_services", b"cc_generic_services", "csharp_namespace", b"csharp_namespace", "deprecated", b"deprecated", "features", b"features", "go_package", b"go_package", "java_generate_equals_and_hash", b"java_generate_equals_and_hash", "java_generic_services", b"java_generic_services", "java_multiple_files", b"java_multiple_files", "java_outer_classname", b"java_outer_classname", "java_package", b"java_package", "java_string_check_utf8", b"java_string_check_utf8", "objc_class_prefix", b"objc_class_prefix", "optimize_for", b"optimize_for", "php_class_prefix", b"php_class_prefix", "php_generic_services", b"php_generic_services", "php_metadata_namespace", b"php_metadata_namespace", "php_namespace", b"php_namespace", "py_generic_services", b"py_generic_services", "ruby_package", b"ruby_package", "swift_prefix", b"swift_prefix", "uninterpreted_option", b"uninterpreted_option"]) -> None: ...
 
 global___FileOptions = FileOptions
 
-@typing_extensions.final
+@typing.final
 class MessageOptions(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     MESSAGE_SET_WIRE_FORMAT_FIELD_NUMBER: builtins.int
     NO_STANDARD_DESCRIPTOR_ACCESSOR_FIELD_NUMBER: builtins.int
     DEPRECATED_FIELD_NUMBER: builtins.int
     MAP_ENTRY_FIELD_NUMBER: builtins.int
+    DEPRECATED_LEGACY_JSON_FIELD_CONFLICTS_FIELD_NUMBER: builtins.int
+    FEATURES_FIELD_NUMBER: builtins.int
     UNINTERPRETED_OPTION_FIELD_NUMBER: builtins.int
     message_set_wire_format: builtins.bool
     """Set true to use the old proto1 MessageSet wire format for extensions.
     This is provided for backwards-compatibility with the MessageSet wire
     format.  You should not use this for any other reason:  It's less
     efficient, has fewer features, and is more complicated.
 
@@ -866,15 +1038,19 @@
     deprecated: builtins.bool
     """Is this message deprecated?
     Depending on the target platform, this can emit Deprecated annotations
     for the message, or it will be completely ignored; in the very least,
     this is a formalization for deprecating messages.
     """
     map_entry: builtins.bool
-    """Whether the message is an automatically generated map entry type for the
+    """NOTE: Do not set the option in .proto files. Always use the maps syntax
+    instead. The option should only be implicitly set by the proto compiler
+    parser.
+
+    Whether the message is an automatically generated map entry type for the
     maps field.
 
     For maps fields:
         map<KeyType, ValueType> map_field = 1;
     The parsed descriptor looks like:
         message MapFieldEntry {
             option map_entry = true;
@@ -883,55 +1059,84 @@
         }
         repeated MapFieldEntry map_field = 1;
 
     Implementations may choose not to generate the map_entry=true message, but
     use a native map in the target language to hold the keys and values.
     The reflection APIs in such implementations still need to work as
     if the field is a repeated message field.
+    """
+    deprecated_legacy_json_field_conflicts: builtins.bool
+    """Enable the legacy handling of JSON field name conflicts.  This lowercases
+    and strips underscored from the fields before comparison in proto3 only.
+    The new behavior takes `json_name` into account and applies to proto2 as
+    well.
 
-    NOTE: Do not set the option in .proto files. Always use the maps syntax
-    instead. The option should only be implicitly set by the proto compiler
-    parser.
+    This should only be used as a temporary measure against broken builds due
+    to the change in behavior for JSON field name conflicts.
+
+    TODO This is legacy behavior we plan to remove once downstream
+    teams have had time to migrate.
     """
     @property
+    def features(self) -> global___FeatureSet:
+        """Any features defined in the specific edition."""
+
+    @property
     def uninterpreted_option(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___UninterpretedOption]:
         """The parser stores options it doesn't recognize here. See above."""
+
     def __init__(
         self,
         *,
         message_set_wire_format: builtins.bool | None = ...,
         no_standard_descriptor_accessor: builtins.bool | None = ...,
         deprecated: builtins.bool | None = ...,
         map_entry: builtins.bool | None = ...,
+        deprecated_legacy_json_field_conflicts: builtins.bool | None = ...,
+        features: global___FeatureSet | None = ...,
         uninterpreted_option: collections.abc.Iterable[global___UninterpretedOption] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["deprecated", b"deprecated", "map_entry", b"map_entry", "message_set_wire_format", b"message_set_wire_format", "no_standard_descriptor_accessor", b"no_standard_descriptor_accessor"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["deprecated", b"deprecated", "map_entry", b"map_entry", "message_set_wire_format", b"message_set_wire_format", "no_standard_descriptor_accessor", b"no_standard_descriptor_accessor", "uninterpreted_option", b"uninterpreted_option"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["deprecated", b"deprecated", "deprecated_legacy_json_field_conflicts", b"deprecated_legacy_json_field_conflicts", "features", b"features", "map_entry", b"map_entry", "message_set_wire_format", b"message_set_wire_format", "no_standard_descriptor_accessor", b"no_standard_descriptor_accessor"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["deprecated", b"deprecated", "deprecated_legacy_json_field_conflicts", b"deprecated_legacy_json_field_conflicts", "features", b"features", "map_entry", b"map_entry", "message_set_wire_format", b"message_set_wire_format", "no_standard_descriptor_accessor", b"no_standard_descriptor_accessor", "uninterpreted_option", b"uninterpreted_option"]) -> None: ...
 
 global___MessageOptions = MessageOptions
 
-@typing_extensions.final
+@typing.final
 class FieldOptions(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _CType:
         ValueType = typing.NewType("ValueType", builtins.int)
         V: typing_extensions.TypeAlias = ValueType
 
     class _CTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[FieldOptions._CType.ValueType], builtins.type):
         DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
         STRING: FieldOptions._CType.ValueType  # 0
         """Default mode."""
         CORD: FieldOptions._CType.ValueType  # 1
+        """The option [ctype=CORD] may be applied to a non-repeated field of type
+        "bytes". It indicates that in C++, the data should be stored in a Cord
+        instead of a string.  For very large strings, this may reduce memory
+        fragmentation. It may also allow better performance when parsing from a
+        Cord, or when parsing with aliasing enabled, as the parsed Cord may then
+        alias the original buffer.
+        """
         STRING_PIECE: FieldOptions._CType.ValueType  # 2
 
     class CType(_CType, metaclass=_CTypeEnumTypeWrapper): ...
     STRING: FieldOptions.CType.ValueType  # 0
     """Default mode."""
     CORD: FieldOptions.CType.ValueType  # 1
+    """The option [ctype=CORD] may be applied to a non-repeated field of type
+    "bytes". It indicates that in C++, the data should be stored in a Cord
+    instead of a string.  For very large strings, this may reduce memory
+    fragmentation. It may also allow better performance when parsing from a
+    Cord, or when parsing with aliasing enabled, as the parsed Cord may then
+    alias the original buffer.
+    """
     STRING_PIECE: FieldOptions.CType.ValueType  # 2
 
     class _JSType:
         ValueType = typing.NewType("ValueType", builtins.int)
         V: typing_extensions.TypeAlias = ValueType
 
     class _JSTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[FieldOptions._JSType.ValueType], builtins.type):
@@ -947,34 +1152,116 @@
     JS_NORMAL: FieldOptions.JSType.ValueType  # 0
     """Use the default type."""
     JS_STRING: FieldOptions.JSType.ValueType  # 1
     """Use JavaScript strings."""
     JS_NUMBER: FieldOptions.JSType.ValueType  # 2
     """Use JavaScript numbers."""
 
+    class _OptionRetention:
+        ValueType = typing.NewType("ValueType", builtins.int)
+        V: typing_extensions.TypeAlias = ValueType
+
+    class _OptionRetentionEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[FieldOptions._OptionRetention.ValueType], builtins.type):
+        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+        RETENTION_UNKNOWN: FieldOptions._OptionRetention.ValueType  # 0
+        RETENTION_RUNTIME: FieldOptions._OptionRetention.ValueType  # 1
+        RETENTION_SOURCE: FieldOptions._OptionRetention.ValueType  # 2
+
+    class OptionRetention(_OptionRetention, metaclass=_OptionRetentionEnumTypeWrapper):
+        """If set to RETENTION_SOURCE, the option will be omitted from the binary.
+        Note: as of January 2023, support for this is in progress and does not yet
+        have an effect (b/264593489).
+        """
+
+    RETENTION_UNKNOWN: FieldOptions.OptionRetention.ValueType  # 0
+    RETENTION_RUNTIME: FieldOptions.OptionRetention.ValueType  # 1
+    RETENTION_SOURCE: FieldOptions.OptionRetention.ValueType  # 2
+
+    class _OptionTargetType:
+        ValueType = typing.NewType("ValueType", builtins.int)
+        V: typing_extensions.TypeAlias = ValueType
+
+    class _OptionTargetTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[FieldOptions._OptionTargetType.ValueType], builtins.type):
+        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+        TARGET_TYPE_UNKNOWN: FieldOptions._OptionTargetType.ValueType  # 0
+        TARGET_TYPE_FILE: FieldOptions._OptionTargetType.ValueType  # 1
+        TARGET_TYPE_EXTENSION_RANGE: FieldOptions._OptionTargetType.ValueType  # 2
+        TARGET_TYPE_MESSAGE: FieldOptions._OptionTargetType.ValueType  # 3
+        TARGET_TYPE_FIELD: FieldOptions._OptionTargetType.ValueType  # 4
+        TARGET_TYPE_ONEOF: FieldOptions._OptionTargetType.ValueType  # 5
+        TARGET_TYPE_ENUM: FieldOptions._OptionTargetType.ValueType  # 6
+        TARGET_TYPE_ENUM_ENTRY: FieldOptions._OptionTargetType.ValueType  # 7
+        TARGET_TYPE_SERVICE: FieldOptions._OptionTargetType.ValueType  # 8
+        TARGET_TYPE_METHOD: FieldOptions._OptionTargetType.ValueType  # 9
+
+    class OptionTargetType(_OptionTargetType, metaclass=_OptionTargetTypeEnumTypeWrapper):
+        """This indicates the types of entities that the field may apply to when used
+        as an option. If it is unset, then the field may be freely used as an
+        option on any kind of entity. Note: as of January 2023, support for this is
+        in progress and does not yet have an effect (b/264593489).
+        """
+
+    TARGET_TYPE_UNKNOWN: FieldOptions.OptionTargetType.ValueType  # 0
+    TARGET_TYPE_FILE: FieldOptions.OptionTargetType.ValueType  # 1
+    TARGET_TYPE_EXTENSION_RANGE: FieldOptions.OptionTargetType.ValueType  # 2
+    TARGET_TYPE_MESSAGE: FieldOptions.OptionTargetType.ValueType  # 3
+    TARGET_TYPE_FIELD: FieldOptions.OptionTargetType.ValueType  # 4
+    TARGET_TYPE_ONEOF: FieldOptions.OptionTargetType.ValueType  # 5
+    TARGET_TYPE_ENUM: FieldOptions.OptionTargetType.ValueType  # 6
+    TARGET_TYPE_ENUM_ENTRY: FieldOptions.OptionTargetType.ValueType  # 7
+    TARGET_TYPE_SERVICE: FieldOptions.OptionTargetType.ValueType  # 8
+    TARGET_TYPE_METHOD: FieldOptions.OptionTargetType.ValueType  # 9
+
+    @typing.final
+    class EditionDefault(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        EDITION_FIELD_NUMBER: builtins.int
+        VALUE_FIELD_NUMBER: builtins.int
+        edition: global___Edition.ValueType
+        value: builtins.str
+        """Textproto value."""
+        def __init__(
+            self,
+            *,
+            edition: global___Edition.ValueType | None = ...,
+            value: builtins.str | None = ...,
+        ) -> None: ...
+        def HasField(self, field_name: typing.Literal["edition", b"edition", "value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["edition", b"edition", "value", b"value"]) -> None: ...
+
     CTYPE_FIELD_NUMBER: builtins.int
     PACKED_FIELD_NUMBER: builtins.int
     JSTYPE_FIELD_NUMBER: builtins.int
     LAZY_FIELD_NUMBER: builtins.int
     UNVERIFIED_LAZY_FIELD_NUMBER: builtins.int
     DEPRECATED_FIELD_NUMBER: builtins.int
     WEAK_FIELD_NUMBER: builtins.int
+    DEBUG_REDACT_FIELD_NUMBER: builtins.int
+    RETENTION_FIELD_NUMBER: builtins.int
+    TARGETS_FIELD_NUMBER: builtins.int
+    EDITION_DEFAULTS_FIELD_NUMBER: builtins.int
+    FEATURES_FIELD_NUMBER: builtins.int
     UNINTERPRETED_OPTION_FIELD_NUMBER: builtins.int
     ctype: global___FieldOptions.CType.ValueType
     """The ctype option instructs the C++ code generator to use a different
     representation of the field than it normally would.  See the specific
-    options below.  This option is not yet implemented in the open source
-    release -- sorry, we'll try to include it in a future version!
+    options below.  This option is only implemented to support use of
+    [ctype=CORD] and [ctype=STRING] (the default) on non-repeated fields of
+    type "bytes" in the open source release -- sorry, we'll try to include
+    other types in a future version!
     """
     packed: builtins.bool
     """The packed option can be enabled for repeated primitive fields to enable
     a more efficient representation on the wire. Rather than repeatedly
     writing the tag and type for each element, the entire array is encoded as
     a single length-delimited blob. In proto3, only explicit setting it to
-    false will avoid using packed encoding.
+    false will avoid using packed encoding.  This option is prohibited in
+    Editions, but the `repeated_field_encoding` feature can be used to control
+    the behavior.
     """
     jstype: global___FieldOptions.JSType.ValueType
     """The jstype option determines the JavaScript type used for values of the
     field.  The option is permitted only for 64 bit integral and fixed types
     (int64, uint64, sint64, fixed64, sfixed64).  A field with jstype JS_STRING
     is represented as JavaScript string, which avoids loss of precision that
     can happen when a large value is converted to a floating point JavaScript.
@@ -999,172 +1286,233 @@
 
     This option does not affect the public interface of any generated code;
     all method signatures remain the same.  Furthermore, thread-safety of the
     interface is not affected by this option; const methods remain safe to
     call from multiple threads concurrently, while non-const methods continue
     to require exclusive access.
 
-
     Note that implementations may choose not to check required fields within
     a lazy sub-message.  That is, calling IsInitialized() on the outer message
     may return true even if the inner message has missing required fields.
     This is necessary because otherwise the inner message would have to be
     parsed in order to perform the check, defeating the purpose of lazy
     parsing.  An implementation which chooses not to check required fields
     must be consistent about it.  That is, for any particular sub-message, the
     implementation must either *always* check its required fields, or *never*
     check its required fields, regardless of whether or not the message has
     been parsed.
 
-    As of 2021, lazy does no correctness checks on the byte stream during
-    parsing.  This may lead to crashes if and when an invalid byte stream is
-    finally parsed upon access.
-
-    TODO(b/211906113):  Enable validation on lazy fields.
+    As of May 2022, lazy verifies the contents of the byte stream during
+    parsing.  An invalid byte stream will cause the overall parsing to fail.
     """
     unverified_lazy: builtins.bool
     """unverified_lazy does no correctness checks on the byte stream. This should
     only be used where lazy with verification is prohibitive for performance
     reasons.
     """
     deprecated: builtins.bool
     """Is this field deprecated?
     Depending on the target platform, this can emit Deprecated annotations
     for accessors, or it will be completely ignored; in the very least, this
     is a formalization for deprecating fields.
     """
     weak: builtins.bool
     """For Google-internal migration only. Do not use."""
+    debug_redact: builtins.bool
+    """Indicate that the field value should not be printed out when using debug
+    formats, e.g. when the field contains sensitive credentials.
+    """
+    retention: global___FieldOptions.OptionRetention.ValueType
+    @property
+    def targets(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[global___FieldOptions.OptionTargetType.ValueType]: ...
+    @property
+    def edition_defaults(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___FieldOptions.EditionDefault]: ...
+    @property
+    def features(self) -> global___FeatureSet:
+        """Any features defined in the specific edition."""
+
     @property
     def uninterpreted_option(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___UninterpretedOption]:
         """The parser stores options it doesn't recognize here. See above."""
+
     def __init__(
         self,
         *,
         ctype: global___FieldOptions.CType.ValueType | None = ...,
         packed: builtins.bool | None = ...,
         jstype: global___FieldOptions.JSType.ValueType | None = ...,
         lazy: builtins.bool | None = ...,
         unverified_lazy: builtins.bool | None = ...,
         deprecated: builtins.bool | None = ...,
         weak: builtins.bool | None = ...,
+        debug_redact: builtins.bool | None = ...,
+        retention: global___FieldOptions.OptionRetention.ValueType | None = ...,
+        targets: collections.abc.Iterable[global___FieldOptions.OptionTargetType.ValueType] | None = ...,
+        edition_defaults: collections.abc.Iterable[global___FieldOptions.EditionDefault] | None = ...,
+        features: global___FeatureSet | None = ...,
         uninterpreted_option: collections.abc.Iterable[global___UninterpretedOption] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["ctype", b"ctype", "deprecated", b"deprecated", "jstype", b"jstype", "lazy", b"lazy", "packed", b"packed", "unverified_lazy", b"unverified_lazy", "weak", b"weak"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["ctype", b"ctype", "deprecated", b"deprecated", "jstype", b"jstype", "lazy", b"lazy", "packed", b"packed", "uninterpreted_option", b"uninterpreted_option", "unverified_lazy", b"unverified_lazy", "weak", b"weak"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["ctype", b"ctype", "debug_redact", b"debug_redact", "deprecated", b"deprecated", "features", b"features", "jstype", b"jstype", "lazy", b"lazy", "packed", b"packed", "retention", b"retention", "unverified_lazy", b"unverified_lazy", "weak", b"weak"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["ctype", b"ctype", "debug_redact", b"debug_redact", "deprecated", b"deprecated", "edition_defaults", b"edition_defaults", "features", b"features", "jstype", b"jstype", "lazy", b"lazy", "packed", b"packed", "retention", b"retention", "targets", b"targets", "uninterpreted_option", b"uninterpreted_option", "unverified_lazy", b"unverified_lazy", "weak", b"weak"]) -> None: ...
 
 global___FieldOptions = FieldOptions
 
-@typing_extensions.final
+@typing.final
 class OneofOptions(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    FEATURES_FIELD_NUMBER: builtins.int
     UNINTERPRETED_OPTION_FIELD_NUMBER: builtins.int
     @property
+    def features(self) -> global___FeatureSet:
+        """Any features defined in the specific edition."""
+
+    @property
     def uninterpreted_option(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___UninterpretedOption]:
         """The parser stores options it doesn't recognize here. See above."""
+
     def __init__(
         self,
         *,
+        features: global___FeatureSet | None = ...,
         uninterpreted_option: collections.abc.Iterable[global___UninterpretedOption] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["uninterpreted_option", b"uninterpreted_option"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["features", b"features"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["features", b"features", "uninterpreted_option", b"uninterpreted_option"]) -> None: ...
 
 global___OneofOptions = OneofOptions
 
-@typing_extensions.final
+@typing.final
 class EnumOptions(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ALLOW_ALIAS_FIELD_NUMBER: builtins.int
     DEPRECATED_FIELD_NUMBER: builtins.int
+    DEPRECATED_LEGACY_JSON_FIELD_CONFLICTS_FIELD_NUMBER: builtins.int
+    FEATURES_FIELD_NUMBER: builtins.int
     UNINTERPRETED_OPTION_FIELD_NUMBER: builtins.int
     allow_alias: builtins.bool
     """Set this option to true to allow mapping different tag names to the same
     value.
     """
     deprecated: builtins.bool
     """Is this enum deprecated?
     Depending on the target platform, this can emit Deprecated annotations
     for the enum, or it will be completely ignored; in the very least, this
     is a formalization for deprecating enums.
     """
+    deprecated_legacy_json_field_conflicts: builtins.bool
+    """Enable the legacy handling of JSON field name conflicts.  This lowercases
+    and strips underscored from the fields before comparison in proto3 only.
+    The new behavior takes `json_name` into account and applies to proto2 as
+    well.
+    TODO Remove this legacy behavior once downstream teams have
+    had time to migrate.
+    """
+    @property
+    def features(self) -> global___FeatureSet:
+        """Any features defined in the specific edition."""
+
     @property
     def uninterpreted_option(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___UninterpretedOption]:
         """The parser stores options it doesn't recognize here. See above."""
+
     def __init__(
         self,
         *,
         allow_alias: builtins.bool | None = ...,
         deprecated: builtins.bool | None = ...,
+        deprecated_legacy_json_field_conflicts: builtins.bool | None = ...,
+        features: global___FeatureSet | None = ...,
         uninterpreted_option: collections.abc.Iterable[global___UninterpretedOption] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["allow_alias", b"allow_alias", "deprecated", b"deprecated"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["allow_alias", b"allow_alias", "deprecated", b"deprecated", "uninterpreted_option", b"uninterpreted_option"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["allow_alias", b"allow_alias", "deprecated", b"deprecated", "deprecated_legacy_json_field_conflicts", b"deprecated_legacy_json_field_conflicts", "features", b"features"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["allow_alias", b"allow_alias", "deprecated", b"deprecated", "deprecated_legacy_json_field_conflicts", b"deprecated_legacy_json_field_conflicts", "features", b"features", "uninterpreted_option", b"uninterpreted_option"]) -> None: ...
 
 global___EnumOptions = EnumOptions
 
-@typing_extensions.final
+@typing.final
 class EnumValueOptions(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DEPRECATED_FIELD_NUMBER: builtins.int
+    FEATURES_FIELD_NUMBER: builtins.int
+    DEBUG_REDACT_FIELD_NUMBER: builtins.int
     UNINTERPRETED_OPTION_FIELD_NUMBER: builtins.int
     deprecated: builtins.bool
     """Is this enum value deprecated?
     Depending on the target platform, this can emit Deprecated annotations
     for the enum value, or it will be completely ignored; in the very least,
     this is a formalization for deprecating enum values.
     """
+    debug_redact: builtins.bool
+    """Indicate that fields annotated with this enum value should not be printed
+    out when using debug formats, e.g. when the field contains sensitive
+    credentials.
+    """
+    @property
+    def features(self) -> global___FeatureSet:
+        """Any features defined in the specific edition."""
+
     @property
     def uninterpreted_option(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___UninterpretedOption]:
         """The parser stores options it doesn't recognize here. See above."""
+
     def __init__(
         self,
         *,
         deprecated: builtins.bool | None = ...,
+        features: global___FeatureSet | None = ...,
+        debug_redact: builtins.bool | None = ...,
         uninterpreted_option: collections.abc.Iterable[global___UninterpretedOption] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["deprecated", b"deprecated"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["deprecated", b"deprecated", "uninterpreted_option", b"uninterpreted_option"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["debug_redact", b"debug_redact", "deprecated", b"deprecated", "features", b"features"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["debug_redact", b"debug_redact", "deprecated", b"deprecated", "features", b"features", "uninterpreted_option", b"uninterpreted_option"]) -> None: ...
 
 global___EnumValueOptions = EnumValueOptions
 
-@typing_extensions.final
+@typing.final
 class ServiceOptions(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    FEATURES_FIELD_NUMBER: builtins.int
     DEPRECATED_FIELD_NUMBER: builtins.int
     UNINTERPRETED_OPTION_FIELD_NUMBER: builtins.int
     deprecated: builtins.bool
     """Note:  Field numbers 1 through 32 are reserved for Google's internal RPC
       framework.  We apologize for hoarding these numbers to ourselves, but
       we were already using them long before we decided to release Protocol
       Buffers.
 
     Is this service deprecated?
     Depending on the target platform, this can emit Deprecated annotations
     for the service, or it will be completely ignored; in the very least,
     this is a formalization for deprecating services.
     """
     @property
+    def features(self) -> global___FeatureSet:
+        """Any features defined in the specific edition."""
+
+    @property
     def uninterpreted_option(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___UninterpretedOption]:
         """The parser stores options it doesn't recognize here. See above."""
+
     def __init__(
         self,
         *,
+        features: global___FeatureSet | None = ...,
         deprecated: builtins.bool | None = ...,
         uninterpreted_option: collections.abc.Iterable[global___UninterpretedOption] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["deprecated", b"deprecated"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["deprecated", b"deprecated", "uninterpreted_option", b"uninterpreted_option"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["deprecated", b"deprecated", "features", b"features"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["deprecated", b"deprecated", "features", b"features", "uninterpreted_option", b"uninterpreted_option"]) -> None: ...
 
 global___ServiceOptions = ServiceOptions
 
-@typing_extensions.final
+@typing.final
 class MethodOptions(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _IdempotencyLevel:
         ValueType = typing.NewType("ValueType", builtins.int)
         V: typing_extensions.TypeAlias = ValueType
 
@@ -1186,55 +1534,62 @@
     NO_SIDE_EFFECTS: MethodOptions.IdempotencyLevel.ValueType  # 1
     """implies idempotent"""
     IDEMPOTENT: MethodOptions.IdempotencyLevel.ValueType  # 2
     """idempotent, but may have side effects"""
 
     DEPRECATED_FIELD_NUMBER: builtins.int
     IDEMPOTENCY_LEVEL_FIELD_NUMBER: builtins.int
+    FEATURES_FIELD_NUMBER: builtins.int
     UNINTERPRETED_OPTION_FIELD_NUMBER: builtins.int
     deprecated: builtins.bool
     """Note:  Field numbers 1 through 32 are reserved for Google's internal RPC
       framework.  We apologize for hoarding these numbers to ourselves, but
       we were already using them long before we decided to release Protocol
       Buffers.
 
     Is this method deprecated?
     Depending on the target platform, this can emit Deprecated annotations
     for the method, or it will be completely ignored; in the very least,
     this is a formalization for deprecating methods.
     """
     idempotency_level: global___MethodOptions.IdempotencyLevel.ValueType
     @property
+    def features(self) -> global___FeatureSet:
+        """Any features defined in the specific edition."""
+
+    @property
     def uninterpreted_option(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___UninterpretedOption]:
         """The parser stores options it doesn't recognize here. See above."""
+
     def __init__(
         self,
         *,
         deprecated: builtins.bool | None = ...,
         idempotency_level: global___MethodOptions.IdempotencyLevel.ValueType | None = ...,
+        features: global___FeatureSet | None = ...,
         uninterpreted_option: collections.abc.Iterable[global___UninterpretedOption] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["deprecated", b"deprecated", "idempotency_level", b"idempotency_level"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["deprecated", b"deprecated", "idempotency_level", b"idempotency_level", "uninterpreted_option", b"uninterpreted_option"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["deprecated", b"deprecated", "features", b"features", "idempotency_level", b"idempotency_level"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["deprecated", b"deprecated", "features", b"features", "idempotency_level", b"idempotency_level", "uninterpreted_option", b"uninterpreted_option"]) -> None: ...
 
 global___MethodOptions = MethodOptions
 
-@typing_extensions.final
+@typing.final
 class UninterpretedOption(google.protobuf.message.Message):
     """A message representing a option the parser does not recognize. This only
     appears in options protos created by the compiler::Parser class.
     DescriptorPool resolves these when building Descriptor objects. Therefore,
     options protos in descriptor objects (e.g. returned by Descriptor::options(),
     or produced by Descriptor::CopyTo()) will never have UninterpretedOptions
     in them.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class NamePart(google.protobuf.message.Message):
         """The name of the uninterpreted option.  Each string represents a segment in
         a dot-separated name.  is_extension is true iff a segment represents an
         extension (denoted with parentheses in options specs in .proto files).
         E.g.,{ ["foo", false], ["bar.baz", true], ["moo", false] } represents
         "foo.(bar.baz).moo".
         """
@@ -1247,105 +1602,264 @@
         is_extension: builtins.bool
         def __init__(
             self,
             *,
             name_part: builtins.str | None = ...,
             is_extension: builtins.bool | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["is_extension", b"is_extension", "name_part", b"name_part"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["is_extension", b"is_extension", "name_part", b"name_part"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["is_extension", b"is_extension", "name_part", b"name_part"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["is_extension", b"is_extension", "name_part", b"name_part"]) -> None: ...
 
     NAME_FIELD_NUMBER: builtins.int
     IDENTIFIER_VALUE_FIELD_NUMBER: builtins.int
     POSITIVE_INT_VALUE_FIELD_NUMBER: builtins.int
     NEGATIVE_INT_VALUE_FIELD_NUMBER: builtins.int
     DOUBLE_VALUE_FIELD_NUMBER: builtins.int
     STRING_VALUE_FIELD_NUMBER: builtins.int
     AGGREGATE_VALUE_FIELD_NUMBER: builtins.int
-    @property
-    def name(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___UninterpretedOption.NamePart]: ...
     identifier_value: builtins.str
     """The value of the uninterpreted option, in whatever type the tokenizer
     identified it as during parsing. Exactly one of these should be set.
     """
     positive_int_value: builtins.int
     negative_int_value: builtins.int
     double_value: builtins.float
     string_value: builtins.bytes
     aggregate_value: builtins.str
+    @property
+    def name(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___UninterpretedOption.NamePart]: ...
     def __init__(
         self,
         *,
         name: collections.abc.Iterable[global___UninterpretedOption.NamePart] | None = ...,
         identifier_value: builtins.str | None = ...,
         positive_int_value: builtins.int | None = ...,
         negative_int_value: builtins.int | None = ...,
         double_value: builtins.float | None = ...,
         string_value: builtins.bytes | None = ...,
         aggregate_value: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["aggregate_value", b"aggregate_value", "double_value", b"double_value", "identifier_value", b"identifier_value", "negative_int_value", b"negative_int_value", "positive_int_value", b"positive_int_value", "string_value", b"string_value"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["aggregate_value", b"aggregate_value", "double_value", b"double_value", "identifier_value", b"identifier_value", "name", b"name", "negative_int_value", b"negative_int_value", "positive_int_value", b"positive_int_value", "string_value", b"string_value"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["aggregate_value", b"aggregate_value", "double_value", b"double_value", "identifier_value", b"identifier_value", "negative_int_value", b"negative_int_value", "positive_int_value", b"positive_int_value", "string_value", b"string_value"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["aggregate_value", b"aggregate_value", "double_value", b"double_value", "identifier_value", b"identifier_value", "name", b"name", "negative_int_value", b"negative_int_value", "positive_int_value", b"positive_int_value", "string_value", b"string_value"]) -> None: ...
 
 global___UninterpretedOption = UninterpretedOption
 
-@typing_extensions.final
+@typing.final
+class FeatureSet(google.protobuf.message.Message):
+    """===================================================================
+    Features
+
+    TODO Enums in C++ gencode (and potentially other languages) are
+    not well scoped.  This means that each of the feature enums below can clash
+    with each other.  The short names we've chosen maximize call-site
+    readability, but leave us very open to this scenario.  A future feature will
+    be designed and implemented to handle this, hopefully before we ever hit a
+    conflict here.
+    """
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    class _FieldPresence:
+        ValueType = typing.NewType("ValueType", builtins.int)
+        V: typing_extensions.TypeAlias = ValueType
+
+    class _FieldPresenceEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[FeatureSet._FieldPresence.ValueType], builtins.type):
+        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+        FIELD_PRESENCE_UNKNOWN: FeatureSet._FieldPresence.ValueType  # 0
+        EXPLICIT: FeatureSet._FieldPresence.ValueType  # 1
+        IMPLICIT: FeatureSet._FieldPresence.ValueType  # 2
+        LEGACY_REQUIRED: FeatureSet._FieldPresence.ValueType  # 3
+
+    class FieldPresence(_FieldPresence, metaclass=_FieldPresenceEnumTypeWrapper): ...
+    FIELD_PRESENCE_UNKNOWN: FeatureSet.FieldPresence.ValueType  # 0
+    EXPLICIT: FeatureSet.FieldPresence.ValueType  # 1
+    IMPLICIT: FeatureSet.FieldPresence.ValueType  # 2
+    LEGACY_REQUIRED: FeatureSet.FieldPresence.ValueType  # 3
+
+    class _EnumType:
+        ValueType = typing.NewType("ValueType", builtins.int)
+        V: typing_extensions.TypeAlias = ValueType
+
+    class _EnumTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[FeatureSet._EnumType.ValueType], builtins.type):
+        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+        ENUM_TYPE_UNKNOWN: FeatureSet._EnumType.ValueType  # 0
+        OPEN: FeatureSet._EnumType.ValueType  # 1
+        CLOSED: FeatureSet._EnumType.ValueType  # 2
+
+    class EnumType(_EnumType, metaclass=_EnumTypeEnumTypeWrapper): ...
+    ENUM_TYPE_UNKNOWN: FeatureSet.EnumType.ValueType  # 0
+    OPEN: FeatureSet.EnumType.ValueType  # 1
+    CLOSED: FeatureSet.EnumType.ValueType  # 2
+
+    class _RepeatedFieldEncoding:
+        ValueType = typing.NewType("ValueType", builtins.int)
+        V: typing_extensions.TypeAlias = ValueType
+
+    class _RepeatedFieldEncodingEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[FeatureSet._RepeatedFieldEncoding.ValueType], builtins.type):
+        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+        REPEATED_FIELD_ENCODING_UNKNOWN: FeatureSet._RepeatedFieldEncoding.ValueType  # 0
+        PACKED: FeatureSet._RepeatedFieldEncoding.ValueType  # 1
+        EXPANDED: FeatureSet._RepeatedFieldEncoding.ValueType  # 2
+
+    class RepeatedFieldEncoding(_RepeatedFieldEncoding, metaclass=_RepeatedFieldEncodingEnumTypeWrapper): ...
+    REPEATED_FIELD_ENCODING_UNKNOWN: FeatureSet.RepeatedFieldEncoding.ValueType  # 0
+    PACKED: FeatureSet.RepeatedFieldEncoding.ValueType  # 1
+    EXPANDED: FeatureSet.RepeatedFieldEncoding.ValueType  # 2
+
+    class _Utf8Validation:
+        ValueType = typing.NewType("ValueType", builtins.int)
+        V: typing_extensions.TypeAlias = ValueType
+
+    class _Utf8ValidationEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[FeatureSet._Utf8Validation.ValueType], builtins.type):
+        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+        UTF8_VALIDATION_UNKNOWN: FeatureSet._Utf8Validation.ValueType  # 0
+        NONE: FeatureSet._Utf8Validation.ValueType  # 1
+        VERIFY: FeatureSet._Utf8Validation.ValueType  # 2
+
+    class Utf8Validation(_Utf8Validation, metaclass=_Utf8ValidationEnumTypeWrapper): ...
+    UTF8_VALIDATION_UNKNOWN: FeatureSet.Utf8Validation.ValueType  # 0
+    NONE: FeatureSet.Utf8Validation.ValueType  # 1
+    VERIFY: FeatureSet.Utf8Validation.ValueType  # 2
+
+    class _MessageEncoding:
+        ValueType = typing.NewType("ValueType", builtins.int)
+        V: typing_extensions.TypeAlias = ValueType
+
+    class _MessageEncodingEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[FeatureSet._MessageEncoding.ValueType], builtins.type):
+        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+        MESSAGE_ENCODING_UNKNOWN: FeatureSet._MessageEncoding.ValueType  # 0
+        LENGTH_PREFIXED: FeatureSet._MessageEncoding.ValueType  # 1
+        DELIMITED: FeatureSet._MessageEncoding.ValueType  # 2
+
+    class MessageEncoding(_MessageEncoding, metaclass=_MessageEncodingEnumTypeWrapper): ...
+    MESSAGE_ENCODING_UNKNOWN: FeatureSet.MessageEncoding.ValueType  # 0
+    LENGTH_PREFIXED: FeatureSet.MessageEncoding.ValueType  # 1
+    DELIMITED: FeatureSet.MessageEncoding.ValueType  # 2
+
+    class _JsonFormat:
+        ValueType = typing.NewType("ValueType", builtins.int)
+        V: typing_extensions.TypeAlias = ValueType
+
+    class _JsonFormatEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[FeatureSet._JsonFormat.ValueType], builtins.type):
+        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+        JSON_FORMAT_UNKNOWN: FeatureSet._JsonFormat.ValueType  # 0
+        ALLOW: FeatureSet._JsonFormat.ValueType  # 1
+        LEGACY_BEST_EFFORT: FeatureSet._JsonFormat.ValueType  # 2
+
+    class JsonFormat(_JsonFormat, metaclass=_JsonFormatEnumTypeWrapper): ...
+    JSON_FORMAT_UNKNOWN: FeatureSet.JsonFormat.ValueType  # 0
+    ALLOW: FeatureSet.JsonFormat.ValueType  # 1
+    LEGACY_BEST_EFFORT: FeatureSet.JsonFormat.ValueType  # 2
+
+    FIELD_PRESENCE_FIELD_NUMBER: builtins.int
+    ENUM_TYPE_FIELD_NUMBER: builtins.int
+    REPEATED_FIELD_ENCODING_FIELD_NUMBER: builtins.int
+    UTF8_VALIDATION_FIELD_NUMBER: builtins.int
+    MESSAGE_ENCODING_FIELD_NUMBER: builtins.int
+    JSON_FORMAT_FIELD_NUMBER: builtins.int
+    field_presence: global___FeatureSet.FieldPresence.ValueType
+    enum_type: global___FeatureSet.EnumType.ValueType
+    repeated_field_encoding: global___FeatureSet.RepeatedFieldEncoding.ValueType
+    utf8_validation: global___FeatureSet.Utf8Validation.ValueType
+    message_encoding: global___FeatureSet.MessageEncoding.ValueType
+    json_format: global___FeatureSet.JsonFormat.ValueType
+    def __init__(
+        self,
+        *,
+        field_presence: global___FeatureSet.FieldPresence.ValueType | None = ...,
+        enum_type: global___FeatureSet.EnumType.ValueType | None = ...,
+        repeated_field_encoding: global___FeatureSet.RepeatedFieldEncoding.ValueType | None = ...,
+        utf8_validation: global___FeatureSet.Utf8Validation.ValueType | None = ...,
+        message_encoding: global___FeatureSet.MessageEncoding.ValueType | None = ...,
+        json_format: global___FeatureSet.JsonFormat.ValueType | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing.Literal["enum_type", b"enum_type", "field_presence", b"field_presence", "json_format", b"json_format", "message_encoding", b"message_encoding", "repeated_field_encoding", b"repeated_field_encoding", "utf8_validation", b"utf8_validation"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["enum_type", b"enum_type", "field_presence", b"field_presence", "json_format", b"json_format", "message_encoding", b"message_encoding", "repeated_field_encoding", b"repeated_field_encoding", "utf8_validation", b"utf8_validation"]) -> None: ...
+
+global___FeatureSet = FeatureSet
+
+@typing.final
+class FeatureSetDefaults(google.protobuf.message.Message):
+    """A compiled specification for the defaults of a set of features.  These
+    messages are generated from FeatureSet extensions and can be used to seed
+    feature resolution. The resolution with this object becomes a simple search
+    for the closest matching edition, followed by proto merges.
+    """
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    @typing.final
+    class FeatureSetEditionDefault(google.protobuf.message.Message):
+        """A map from every known edition with a unique set of defaults to its
+        defaults. Not all editions may be contained here.  For a given edition,
+        the defaults at the closest matching edition ordered at or before it should
+        be used.  This field must be in strict ascending order by edition.
+        """
+
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        EDITION_FIELD_NUMBER: builtins.int
+        FEATURES_FIELD_NUMBER: builtins.int
+        edition: global___Edition.ValueType
+        @property
+        def features(self) -> global___FeatureSet: ...
+        def __init__(
+            self,
+            *,
+            edition: global___Edition.ValueType | None = ...,
+            features: global___FeatureSet | None = ...,
+        ) -> None: ...
+        def HasField(self, field_name: typing.Literal["edition", b"edition", "features", b"features"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["edition", b"edition", "features", b"features"]) -> None: ...
+
+    DEFAULTS_FIELD_NUMBER: builtins.int
+    MINIMUM_EDITION_FIELD_NUMBER: builtins.int
+    MAXIMUM_EDITION_FIELD_NUMBER: builtins.int
+    minimum_edition: global___Edition.ValueType
+    """The minimum supported edition (inclusive) when this was constructed.
+    Editions before this will not have defaults.
+    """
+    maximum_edition: global___Edition.ValueType
+    """The maximum known edition (inclusive) when this was constructed. Editions
+    after this will not have reliable defaults.
+    """
+    @property
+    def defaults(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___FeatureSetDefaults.FeatureSetEditionDefault]: ...
+    def __init__(
+        self,
+        *,
+        defaults: collections.abc.Iterable[global___FeatureSetDefaults.FeatureSetEditionDefault] | None = ...,
+        minimum_edition: global___Edition.ValueType | None = ...,
+        maximum_edition: global___Edition.ValueType | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing.Literal["maximum_edition", b"maximum_edition", "minimum_edition", b"minimum_edition"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["defaults", b"defaults", "maximum_edition", b"maximum_edition", "minimum_edition", b"minimum_edition"]) -> None: ...
+
+global___FeatureSetDefaults = FeatureSetDefaults
+
+@typing.final
 class SourceCodeInfo(google.protobuf.message.Message):
     """===================================================================
     Optional source code info
 
     Encapsulates information about the original source file from which a
     FileDescriptorProto was generated.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class Location(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         PATH_FIELD_NUMBER: builtins.int
         SPAN_FIELD_NUMBER: builtins.int
         LEADING_COMMENTS_FIELD_NUMBER: builtins.int
         TRAILING_COMMENTS_FIELD_NUMBER: builtins.int
         LEADING_DETACHED_COMMENTS_FIELD_NUMBER: builtins.int
-        @property
-        def path(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
-            """Identifies which part of the FileDescriptorProto was defined at this
-            location.
-
-            Each element is a field number or an index.  They form a path from
-            the root FileDescriptorProto to the place where the definition occurs.
-            For example, this path:
-              [ 4, 3, 2, 7, 1 ]
-            refers to:
-              file.message_type(3)  // 4, 3
-                  .field(7)         // 2, 7
-                  .name()           // 1
-            This is because FileDescriptorProto.message_type has field number 4:
-              repeated DescriptorProto message_type = 4;
-            and DescriptorProto.field has field number 2:
-              repeated FieldDescriptorProto field = 2;
-            and FieldDescriptorProto.name has field number 1:
-              optional string name = 1;
-
-            Thus, the above path gives the location of a field name.  If we removed
-            the last element:
-              [ 4, 3, 2, 7 ]
-            this path refers to the whole field declaration (from the beginning
-            of the label to the terminating semicolon).
-            """
-        @property
-        def span(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
-            """Always has exactly three or four elements: start line, start column,
-            end line (optional, otherwise assumed same as start line), end column.
-            These are packed into a single field for efficiency.  Note that line
-            and column numbers are zero-based -- typically you will want to add
-            1 to each before displaying to a user.
-            """
         leading_comments: builtins.str
         """If this SourceCodeInfo represents a complete declaration, these are any
         comments appearing before and after the declaration which appear to be
         attached to the declaration.
 
         A series of line comments appearing on consecutive lines, with no other
         tokens appearing on those lines, will be treated as a single comment.
@@ -1389,26 +1903,62 @@
            * grault. */
           optional int32 grault = 6;
 
           // ignored detached comments.
         """
         trailing_comments: builtins.str
         @property
+        def path(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
+            """Identifies which part of the FileDescriptorProto was defined at this
+            location.
+
+            Each element is a field number or an index.  They form a path from
+            the root FileDescriptorProto to the place where the definition occurs.
+            For example, this path:
+              [ 4, 3, 2, 7, 1 ]
+            refers to:
+              file.message_type(3)  // 4, 3
+                  .field(7)         // 2, 7
+                  .name()           // 1
+            This is because FileDescriptorProto.message_type has field number 4:
+              repeated DescriptorProto message_type = 4;
+            and DescriptorProto.field has field number 2:
+              repeated FieldDescriptorProto field = 2;
+            and FieldDescriptorProto.name has field number 1:
+              optional string name = 1;
+
+            Thus, the above path gives the location of a field name.  If we removed
+            the last element:
+              [ 4, 3, 2, 7 ]
+            this path refers to the whole field declaration (from the beginning
+            of the label to the terminating semicolon).
+            """
+
+        @property
+        def span(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
+            """Always has exactly three or four elements: start line, start column,
+            end line (optional, otherwise assumed same as start line), end column.
+            These are packed into a single field for efficiency.  Note that line
+            and column numbers are zero-based -- typically you will want to add
+            1 to each before displaying to a user.
+            """
+
+        @property
         def leading_detached_comments(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
         def __init__(
             self,
             *,
             path: collections.abc.Iterable[builtins.int] | None = ...,
             span: collections.abc.Iterable[builtins.int] | None = ...,
             leading_comments: builtins.str | None = ...,
             trailing_comments: builtins.str | None = ...,
             leading_detached_comments: collections.abc.Iterable[builtins.str] | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["leading_comments", b"leading_comments", "trailing_comments", b"trailing_comments"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["leading_comments", b"leading_comments", "leading_detached_comments", b"leading_detached_comments", "path", b"path", "span", b"span", "trailing_comments", b"trailing_comments"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["leading_comments", b"leading_comments", "trailing_comments", b"trailing_comments"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["leading_comments", b"leading_comments", "leading_detached_comments", b"leading_detached_comments", "path", b"path", "span", b"span", "trailing_comments", b"trailing_comments"]) -> None: ...
 
     LOCATION_FIELD_NUMBER: builtins.int
     @property
     def location(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___SourceCodeInfo.Location]:
         """A Location identifies a piece of source code in a .proto file which
         corresponds to a particular definition.  This information is intended
         to be useful to IDEs, code indexers, documentation generators, and similar
@@ -1449,74 +1999,105 @@
           does not mean that it is a descendant.  For example, a "group" defines
           both a type and a field in a single declaration.  Thus, the locations
           corresponding to the type and field and their components will overlap.
         - Code which tries to interpret locations should probably be designed to
           ignore those that it doesn't understand, as more types of locations could
           be recorded in the future.
         """
+
     def __init__(
         self,
         *,
         location: collections.abc.Iterable[global___SourceCodeInfo.Location] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["location", b"location"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["location", b"location"]) -> None: ...
 
 global___SourceCodeInfo = SourceCodeInfo
 
-@typing_extensions.final
+@typing.final
 class GeneratedCodeInfo(google.protobuf.message.Message):
     """Describes the relationship between generated code and its original source
     file. A GeneratedCodeInfo message is associated with only one generated
     source file, but may contain references to different source .proto files.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class Annotation(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+        class _Semantic:
+            ValueType = typing.NewType("ValueType", builtins.int)
+            V: typing_extensions.TypeAlias = ValueType
+
+        class _SemanticEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[GeneratedCodeInfo.Annotation._Semantic.ValueType], builtins.type):
+            DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+            NONE: GeneratedCodeInfo.Annotation._Semantic.ValueType  # 0
+            """There is no effect or the effect is indescribable."""
+            SET: GeneratedCodeInfo.Annotation._Semantic.ValueType  # 1
+            """The element is set or otherwise mutated."""
+            ALIAS: GeneratedCodeInfo.Annotation._Semantic.ValueType  # 2
+            """An alias to the element is returned."""
+
+        class Semantic(_Semantic, metaclass=_SemanticEnumTypeWrapper):
+            """Represents the identified object's effect on the element in the original
+            .proto file.
+            """
+
+        NONE: GeneratedCodeInfo.Annotation.Semantic.ValueType  # 0
+        """There is no effect or the effect is indescribable."""
+        SET: GeneratedCodeInfo.Annotation.Semantic.ValueType  # 1
+        """The element is set or otherwise mutated."""
+        ALIAS: GeneratedCodeInfo.Annotation.Semantic.ValueType  # 2
+        """An alias to the element is returned."""
+
         PATH_FIELD_NUMBER: builtins.int
         SOURCE_FILE_FIELD_NUMBER: builtins.int
         BEGIN_FIELD_NUMBER: builtins.int
         END_FIELD_NUMBER: builtins.int
-        @property
-        def path(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
-            """Identifies the element in the original source .proto file. This field
-            is formatted the same as SourceCodeInfo.Location.path.
-            """
+        SEMANTIC_FIELD_NUMBER: builtins.int
         source_file: builtins.str
         """Identifies the filesystem path to the original source .proto."""
         begin: builtins.int
         """Identifies the starting offset in bytes in the generated code
         that relates to the identified object.
         """
         end: builtins.int
         """Identifies the ending offset in bytes in the generated code that
-        relates to the identified offset. The end offset should be one past
+        relates to the identified object. The end offset should be one past
         the last relevant byte (so the length of the text = end - begin).
         """
+        semantic: global___GeneratedCodeInfo.Annotation.Semantic.ValueType
+        @property
+        def path(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
+            """Identifies the element in the original source .proto file. This field
+            is formatted the same as SourceCodeInfo.Location.path.
+            """
+
         def __init__(
             self,
             *,
             path: collections.abc.Iterable[builtins.int] | None = ...,
             source_file: builtins.str | None = ...,
             begin: builtins.int | None = ...,
             end: builtins.int | None = ...,
+            semantic: global___GeneratedCodeInfo.Annotation.Semantic.ValueType | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["begin", b"begin", "end", b"end", "source_file", b"source_file"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["begin", b"begin", "end", b"end", "path", b"path", "source_file", b"source_file"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["begin", b"begin", "end", b"end", "semantic", b"semantic", "source_file", b"source_file"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["begin", b"begin", "end", b"end", "path", b"path", "semantic", b"semantic", "source_file", b"source_file"]) -> None: ...
 
     ANNOTATION_FIELD_NUMBER: builtins.int
     @property
     def annotation(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___GeneratedCodeInfo.Annotation]:
         """An Annotation connects some span of text in generated code to an element
         of its generating .proto file.
         """
+
     def __init__(
         self,
         *,
         annotation: collections.abc.Iterable[global___GeneratedCodeInfo.Annotation] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["annotation", b"annotation"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["annotation", b"annotation"]) -> None: ...
 
 global___GeneratedCodeInfo = GeneratedCodeInfo
```

### Comparing `types-protobuf-4.24.0.4/google-stubs/protobuf/descriptor_pool.pyi` & `types-protobuf-4.25.0.20240410/google-stubs/protobuf/descriptor_pool.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from _typeshed import Incomplete
 
 class DescriptorPool:
-    def __new__(cls, descriptor_db: Incomplete | None = ...): ...
+    def __new__(cls, descriptor_db: Incomplete | None = None): ...
     def __init__(  # pyright: ignore[reportInconsistentConstructor]
-        self, descriptor_db: Incomplete | None = ..., use_deprecated_legacy_json_field_conflicts: bool = ...
+        self, descriptor_db: Incomplete | None = None, use_deprecated_legacy_json_field_conflicts: bool = False
     ) -> None: ...
     def Add(self, file_desc_proto): ...
     def AddSerializedFile(self, serialized_file_desc_proto): ...
     def AddDescriptor(self, desc): ...
     def AddServiceDescriptor(self, service_desc): ...
     def AddExtensionDescriptor(self, extension): ...
     def AddFileDescriptor(self, file_desc): ...
```

### Comparing `types-protobuf-4.24.0.4/google-stubs/protobuf/duration_pb2.pyi` & `types-protobuf-4.25.0.20240410/google-stubs/protobuf/duration_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -27,29 +27,25 @@
 SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
 LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
+
 import builtins
-import sys
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.well_known_types
 import google.protobuf.message
 
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
-
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class Duration(google.protobuf.message.Message, google.protobuf.internal.well_known_types.Duration):
     """A Duration represents a signed, fixed-length span of time represented
     as a count of seconds and fractions of seconds at nanosecond
     resolution. It is independent of any calendar and concepts like "day"
     or "month". It is related to Timestamp in that the difference between
     two Timestamp values is a Duration and it can be added or subtracted
     from a Timestamp. Range is approximately +-10,000 years.
@@ -126,10 +122,10 @@
     """
     def __init__(
         self,
         *,
         seconds: builtins.int | None = ...,
         nanos: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["nanos", b"nanos", "seconds", b"seconds"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["nanos", b"nanos", "seconds", b"seconds"]) -> None: ...
 
 global___Duration = Duration
```

### Comparing `types-protobuf-4.24.0.4/google-stubs/protobuf/empty_pb2.pyi` & `types-protobuf-4.25.0.20240410/google-stubs/protobuf/empty_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -27,27 +27,23 @@
 SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
 LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
-import sys
+
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.message
 
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
-
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class Empty(google.protobuf.message.Message):
     """A generic empty message that you can re-use to avoid defining duplicated
     empty messages in your APIs. A typical example is to use it as the request
     or the response type of an API method. For instance:
 
         service Foo {
           rpc Bar(google.protobuf.Empty) returns (google.protobuf.Empty);
```

### Comparing `types-protobuf-4.24.0.4/google-stubs/protobuf/field_mask_pb2.pyi` & `types-protobuf-4.25.0.20240410/google-stubs/protobuf/field_mask_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -27,31 +27,27 @@
 SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
 LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
+
 import builtins
 import collections.abc
-import sys
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.internal.well_known_types
 import google.protobuf.message
 
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
-
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class FieldMask(google.protobuf.message.Message, google.protobuf.internal.well_known_types.FieldMask):
     """`FieldMask` represents a set of symbolic field paths, for example:
 
         paths: "f.a"
         paths: "f.b.d"
 
     Here `f` represents a field in some root message, `a` and `b`
@@ -252,15 +248,16 @@
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PATHS_FIELD_NUMBER: builtins.int
     @property
     def paths(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """The set of field mask paths."""
+
     def __init__(
         self,
         *,
         paths: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["paths", b"paths"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["paths", b"paths"]) -> None: ...
 
 global___FieldMask = FieldMask
```

### Comparing `types-protobuf-4.24.0.4/google-stubs/protobuf/internal/containers.pyi` & `types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/containers.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from collections.abc import Callable, Iterable, Iterator, MutableMapping, Sequence
-from typing import Any, TypeVar, overload
-from typing_extensions import SupportsIndex
+from typing import Any, Protocol, SupportsIndex, TypeVar, overload
 
 from google.protobuf.descriptor import Descriptor
 from google.protobuf.internal.message_listener import MessageListener
 from google.protobuf.internal.python_message import GeneratedProtocolMessageType
-from google.protobuf.internal.type_checkers import _ValueChecker
 from google.protobuf.message import Message
 
 _T = TypeVar("_T")
 _K = TypeVar("_K", bound=bool | int | str)
 _ScalarV = TypeVar("_ScalarV", bound=bool | int | float | str | bytes)
 _MessageV = TypeVar("_MessageV", bound=Message)
 _M = TypeVar("_M")
 
+class _ValueChecker(Protocol[_T]):
+    def CheckValue(self, proposed_value: _T) -> _T: ...
+    def DefaultValue(self) -> _T: ...
+
 class BaseContainer(Sequence[_T]):
     def __init__(self, message_listener: MessageListener) -> None: ...
     def __len__(self) -> int: ...
     def __ne__(self, other: object) -> bool: ...
     def __hash__(self) -> int: ...
     def sort(self, *, key: Callable[[_T], Any] | None = ..., reverse: bool = ...) -> None: ...
     @overload
@@ -28,15 +30,15 @@
 class RepeatedScalarFieldContainer(BaseContainer[_ScalarV]):
     def __init__(self, message_listener: MessageListener, type_checker: _ValueChecker[_ScalarV]) -> None: ...
     def append(self, value: _ScalarV) -> None: ...
     def insert(self, key: int, value: _ScalarV) -> None: ...
     def extend(self, elem_seq: Iterable[_ScalarV] | None) -> None: ...
     def MergeFrom(self: _M, other: _M) -> None: ...
     def remove(self, elem: _ScalarV) -> None: ...
-    def pop(self, key: int = ...) -> _ScalarV: ...
+    def pop(self, key: int = -1) -> _ScalarV: ...
     @overload
     def __setitem__(self, key: int, value: _ScalarV) -> None: ...
     @overload
     def __setitem__(self, key: slice, value: Iterable[_ScalarV]) -> None: ...
     def __delitem__(self, key: int | slice) -> None: ...
     def __eq__(self, other: object) -> bool: ...
 
@@ -44,15 +46,15 @@
     def __init__(self, message_listener: MessageListener, message_descriptor: Descriptor) -> None: ...
     def add(self, **kwargs: Any) -> _MessageV: ...
     def append(self, value: _MessageV) -> None: ...
     def insert(self, key: int, value: _MessageV) -> None: ...
     def extend(self, elem_seq: Iterable[_MessageV]) -> None: ...
     def MergeFrom(self: _M, other: _M) -> None: ...
     def remove(self, elem: _MessageV) -> None: ...
-    def pop(self, key: int = ...) -> _MessageV: ...
+    def pop(self, key: int = -1) -> _MessageV: ...
     def __delitem__(self, key: int | slice) -> None: ...
     def __eq__(self, other: object) -> bool: ...
 
 class ScalarMap(MutableMapping[_K, _ScalarV]):
     def __init__(
         self,
         message_listener: MessageListener,
@@ -63,15 +65,15 @@
     def __setitem__(self, k: _K, v: _ScalarV) -> None: ...
     def __delitem__(self, v: _K) -> None: ...
     def __getitem__(self, k: _K) -> _ScalarV: ...
     def __len__(self) -> int: ...
     def __iter__(self) -> Iterator[_K]: ...
     def __eq__(self, other: object) -> bool: ...
     @overload
-    def get(self, key: _K, default: None = ...) -> _ScalarV | None: ...
+    def get(self, key: _K, default: None = None) -> _ScalarV | None: ...
     @overload
     def get(self, key: _K, default: _ScalarV | _T) -> _ScalarV | _T: ...
     def MergeFrom(self: _M, other: _M): ...
     def InvalidateIterators(self) -> None: ...
     def GetEntryClass(self) -> GeneratedProtocolMessageType: ...
 
 class MessageMap(MutableMapping[_K, _MessageV]):
@@ -85,14 +87,14 @@
     def __setitem__(self, k: _K, v: _MessageV) -> None: ...
     def __delitem__(self, v: _K) -> None: ...
     def __getitem__(self, k: _K) -> _MessageV: ...
     def __len__(self) -> int: ...
     def __iter__(self) -> Iterator[_K]: ...
     def __eq__(self, other: object) -> bool: ...
     @overload
-    def get(self, key: _K, default: None = ...) -> _MessageV | None: ...
+    def get(self, key: _K, default: None = None) -> _MessageV | None: ...
     @overload
     def get(self, key: _K, default: _MessageV | _T) -> _MessageV | _T: ...
     def get_or_create(self, key: _K) -> _MessageV: ...
     def MergeFrom(self: _M, other: _M): ...
     def InvalidateIterators(self) -> None: ...
     def GetEntryClass(self) -> GeneratedProtocolMessageType: ...
```

### Comparing `types-protobuf-4.24.0.4/google-stubs/protobuf/internal/decoder.pyi` & `types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/decoder.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -26,31 +26,31 @@
 
 def EnumDecoder(
     field_number: int,
     is_repeated: bool,
     is_packed: bool,
     key: FieldDescriptor,
     new_default: _NewDefault,
-    clear_if_default: bool = ...,
+    clear_if_default: bool = False,
 ) -> _Decoder: ...
 def StringDecoder(
     field_number: int,
     is_repeated: bool,
     is_packed: bool,
     key: FieldDescriptor,
     new_default: _NewDefault,
-    clear_if_default: bool = ...,
+    clear_if_default: bool = False,
 ) -> _Decoder: ...
 def BytesDecoder(
     field_number: int,
     is_repeated: bool,
     is_packed: bool,
     key: FieldDescriptor,
     new_default: _NewDefault,
-    clear_if_default: bool = ...,
+    clear_if_default: bool = False,
 ) -> _Decoder: ...
 def GroupDecoder(
     field_number: int, is_repeated: bool, is_packed: bool, key: FieldDescriptor, new_default: _NewDefault
 ) -> _Decoder: ...
 def MessageDecoder(
     field_number: int, is_repeated: bool, is_packed: bool, key: FieldDescriptor, new_default: _NewDefault
 ) -> _Decoder: ...
```

### Comparing `types-protobuf-4.24.0.4/google-stubs/protobuf/internal/encoder.pyi` & `types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/encoder.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.24.0.4/google-stubs/protobuf/internal/enum_type_wrapper.pyi` & `types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/enum_type_wrapper.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.24.0.4/google-stubs/protobuf/internal/extension_dict.pyi` & `types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/extension_dict.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.24.0.4/google-stubs/protobuf/internal/well_known_types.pyi` & `types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/well_known_types.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     def ToMicroseconds(self) -> int: ...
     def ToMilliseconds(self) -> int: ...
     def ToSeconds(self) -> int: ...
     def FromNanoseconds(self, nanos: int) -> None: ...
     def FromMicroseconds(self, micros: int) -> None: ...
     def FromMilliseconds(self, millis: int) -> None: ...
     def FromSeconds(self, seconds: int) -> None: ...
-    def ToDatetime(self, tzinfo: tzinfo | None = ...) -> datetime: ...
+    def ToDatetime(self, tzinfo: tzinfo | None = None) -> datetime: ...
     def FromDatetime(self, dt: datetime) -> None: ...
 
 class Duration:
     def ToJsonString(self) -> str: ...
     seconds: int
     nanos: int
     def FromJsonString(self, value: tAny) -> None: ...
@@ -54,15 +54,15 @@
     def FromJsonString(self, value: tAny) -> None: ...
     def IsValidForDescriptor(self, message_descriptor: tAny): ...
     def AllFieldsFromDescriptor(self, message_descriptor: tAny) -> None: ...
     def CanonicalFormFromMask(self, mask: tAny) -> None: ...
     def Union(self, mask1: tAny, mask2: tAny) -> None: ...
     def Intersect(self, mask1: tAny, mask2: tAny) -> None: ...
     def MergeMessage(
-        self, source: tAny, destination: tAny, replace_message_field: bool = ..., replace_repeated_field: bool = ...
+        self, source: tAny, destination: tAny, replace_message_field: bool = False, replace_repeated_field: bool = False
     ) -> None: ...
 
 class _FieldMaskTree:
     def __init__(self, field_mask: Incomplete | None = ...) -> None: ...
     def MergeFromFieldMask(self, field_mask: tAny) -> None: ...
     def AddPath(self, path: tAny): ...
     def ToFieldMask(self, field_mask: tAny) -> None: ...
```

### Comparing `types-protobuf-4.24.0.4/google-stubs/protobuf/internal/wire_format.pyi` & `types-protobuf-4.25.0.20240410/google-stubs/protobuf/internal/wire_format.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.24.0.4/google-stubs/protobuf/json_format.pyi` & `types-protobuf-4.25.0.20240410/google-stubs/protobuf/json_format.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -7,38 +7,38 @@
 
 class Error(Exception): ...
 class ParseError(Error): ...
 class SerializeToJsonError(Error): ...
 
 def MessageToJson(
     message: Message,
-    including_default_value_fields: bool = ...,
-    preserving_proto_field_name: bool = ...,
-    indent: int | None = ...,
-    sort_keys: bool = ...,
-    use_integers_for_enums: bool = ...,
-    descriptor_pool: DescriptorPool | None = ...,
-    float_precision: int | None = ...,
-    ensure_ascii: bool = ...,
+    including_default_value_fields: bool = False,
+    preserving_proto_field_name: bool = False,
+    indent: int | None = 2,
+    sort_keys: bool = False,
+    use_integers_for_enums: bool = False,
+    descriptor_pool: DescriptorPool | None = None,
+    float_precision: int | None = None,
+    ensure_ascii: bool = True,
 ) -> str: ...
 def MessageToDict(
     message: Message,
-    including_default_value_fields: bool = ...,
-    preserving_proto_field_name: bool = ...,
-    use_integers_for_enums: bool = ...,
-    descriptor_pool: DescriptorPool | None = ...,
-    float_precision: int | None = ...,
+    including_default_value_fields: bool = False,
+    preserving_proto_field_name: bool = False,
+    use_integers_for_enums: bool = False,
+    descriptor_pool: DescriptorPool | None = None,
+    float_precision: int | None = None,
 ) -> dict[str, Any]: ...
 def Parse(
     text: bytes | str,
     message: _MessageT,
-    ignore_unknown_fields: bool = ...,
-    descriptor_pool: DescriptorPool | None = ...,
-    max_recursion_depth: int = ...,
+    ignore_unknown_fields: bool = False,
+    descriptor_pool: DescriptorPool | None = None,
+    max_recursion_depth: int = 100,
 ) -> _MessageT: ...
 def ParseDict(
     js_dict: Any,
     message: _MessageT,
-    ignore_unknown_fields: bool = ...,
-    descriptor_pool: DescriptorPool | None = ...,
-    max_recursion_depth: int = ...,
+    ignore_unknown_fields: bool = False,
+    descriptor_pool: DescriptorPool | None = None,
+    max_recursion_depth: int = 100,
 ) -> _MessageT: ...
```

### Comparing `types-protobuf-4.24.0.4/google-stubs/protobuf/message.pyi` & `types-protobuf-4.25.0.20240410/google-stubs/protobuf/message.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class DecodeError(Error): ...
 class EncodeError(Error): ...
 
 _M = TypeVar("_M", bound=Message)  # message type (of self)
 
 class Message:
     DESCRIPTOR: Descriptor
-    def __deepcopy__(self, memo: Any = ...) -> Self: ...
+    def __deepcopy__(self, memo: Any = None) -> Self: ...
     def __eq__(self, other_msg): ...
     def __ne__(self, other_msg): ...
     def MergeFrom(self, other_msg: Self) -> None: ...
     def CopyFrom(self, other_msg: Self) -> None: ...
     def Clear(self) -> None: ...
     def SetInParent(self) -> None: ...
     def IsInitialized(self) -> bool: ...
```

### Comparing `types-protobuf-4.24.0.4/google-stubs/protobuf/message_factory.pyi` & `types-protobuf-4.25.0.20240410/google-stubs/protobuf/message_factory.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 from google.protobuf.descriptor import Descriptor
 from google.protobuf.descriptor_pb2 import FileDescriptorProto
 from google.protobuf.descriptor_pool import DescriptorPool
 from google.protobuf.message import Message
 
 class MessageFactory:
     pool: Any
-    def __init__(self, pool: DescriptorPool | None = ...) -> None: ...
+    def __init__(self, pool: DescriptorPool | None = None) -> None: ...
     def GetPrototype(self, descriptor: Descriptor) -> type[Message]: ...
     def GetMessages(self, files: Iterable[str]) -> dict[str, type[Message]]: ...
 
 def GetMessageClass(descriptor: Descriptor) -> type[Message]: ...
 def GetMessageClassesForFiles(files: Iterable[str], pool: DescriptorPool) -> dict[str, type[Message]]: ...
-def GetMessages(file_protos: Iterable[FileDescriptorProto], pool: DescriptorPool | None = ...) -> dict[str, type[Message]]: ...
+def GetMessages(file_protos: Iterable[FileDescriptorProto], pool: DescriptorPool | None = None) -> dict[str, type[Message]]: ...
```

### Comparing `types-protobuf-4.24.0.4/google-stubs/protobuf/service.pyi` & `types-protobuf-4.25.0.20240410/google-stubs/protobuf/service.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.24.0.4/google-stubs/protobuf/source_context_pb2.pyi` & `types-protobuf-4.25.0.20240410/google-stubs/protobuf/source_context_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -27,28 +27,24 @@
 SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
 LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
+
 import builtins
-import sys
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.message
 
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
-
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class SourceContext(google.protobuf.message.Message):
     """`SourceContext` represents information about the source of a
     protobuf element, like the file in which it is defined.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -58,10 +54,10 @@
     protobuf element.  For example: `"google/protobuf/source_context.proto"`.
     """
     def __init__(
         self,
         *,
         file_name: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["file_name", b"file_name"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["file_name", b"file_name"]) -> None: ...
 
 global___SourceContext = SourceContext
```

### Comparing `types-protobuf-4.24.0.4/google-stubs/protobuf/struct_pb2.pyi` & `types-protobuf-4.25.0.20240410/google-stubs/protobuf/struct_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
 LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
+
 import builtins
 import collections.abc
 import sys
 import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
@@ -58,67 +59,68 @@
     NULL_VALUE: _NullValue.ValueType  # 0
     """Null value."""
 
 class NullValue(_NullValue, metaclass=_NullValueEnumTypeWrapper):
     """`NullValue` is a singleton enumeration to represent the null value for the
     `Value` type union.
 
-     The JSON representation for `NullValue` is JSON `null`.
+    The JSON representation for `NullValue` is JSON `null`.
     """
 
 NULL_VALUE: NullValue.ValueType  # 0
 """Null value."""
 global___NullValue = NullValue
 
-@typing_extensions.final
+@typing.final
 class Struct(google.protobuf.message.Message, google.protobuf.internal.well_known_types.Struct):
     """`Struct` represents a structured data value, consisting of fields
     which map to dynamically typed values. In some languages, `Struct`
     might be supported by a native representation. For example, in
     scripting languages like JS a struct is represented as an
     object. The details of that representation are described together
     with the proto support for the language.
 
     The JSON representation for `Struct` is JSON object.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
+    @typing.final
     class FieldsEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         @property
         def value(self) -> global___Value: ...
         def __init__(
             self,
             *,
             key: builtins.str | None = ...,
             value: global___Value | None = ...,
         ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+        def HasField(self, field_name: typing.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     FIELDS_FIELD_NUMBER: builtins.int
     @property
     def fields(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___Value]:
         """Unordered map of dynamically typed values."""
+
     def __init__(
         self,
         *,
         fields: collections.abc.Mapping[builtins.str, global___Value] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["fields", b"fields"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["fields", b"fields"]) -> None: ...
 
 global___Struct = Struct
 
-@typing_extensions.final
+@typing.final
 class Value(google.protobuf.message.Message):
     """`Value` represents a dynamically typed value which can be either
     null, a number, a string, a boolean, a recursive struct value, or a
     list of values. A producer of value is expected to set one of these
     variants. Absence of any variant indicates an error.
 
     The JSON representation for `Value` is JSON value.
@@ -139,47 +141,50 @@
     string_value: builtins.str
     """Represents a string value."""
     bool_value: builtins.bool
     """Represents a boolean value."""
     @property
     def struct_value(self) -> global___Struct:
         """Represents a structured value."""
+
     @property
     def list_value(self) -> global___ListValue:
         """Represents a repeated `Value`."""
+
     def __init__(
         self,
         *,
         null_value: global___NullValue.ValueType | None = ...,
         number_value: builtins.float | None = ...,
         string_value: builtins.str | None = ...,
         bool_value: builtins.bool | None = ...,
         struct_value: global___Struct | None = ...,
         list_value: global___ListValue | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["bool_value", b"bool_value", "kind", b"kind", "list_value", b"list_value", "null_value", b"null_value", "number_value", b"number_value", "string_value", b"string_value", "struct_value", b"struct_value"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["bool_value", b"bool_value", "kind", b"kind", "list_value", b"list_value", "null_value", b"null_value", "number_value", b"number_value", "string_value", b"string_value", "struct_value", b"struct_value"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["kind", b"kind"]) -> typing_extensions.Literal["null_value", "number_value", "string_value", "bool_value", "struct_value", "list_value"] | None: ...
+    def HasField(self, field_name: typing.Literal["bool_value", b"bool_value", "kind", b"kind", "list_value", b"list_value", "null_value", b"null_value", "number_value", b"number_value", "string_value", b"string_value", "struct_value", b"struct_value"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["bool_value", b"bool_value", "kind", b"kind", "list_value", b"list_value", "null_value", b"null_value", "number_value", b"number_value", "string_value", b"string_value", "struct_value", b"struct_value"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing.Literal["kind", b"kind"]) -> typing.Literal["null_value", "number_value", "string_value", "bool_value", "struct_value", "list_value"] | None: ...
 
 global___Value = Value
 
-@typing_extensions.final
+@typing.final
 class ListValue(google.protobuf.message.Message, google.protobuf.internal.well_known_types.ListValue):
     """`ListValue` is a wrapper around a repeated field of values.
 
     The JSON representation for `ListValue` is JSON array.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VALUES_FIELD_NUMBER: builtins.int
     @property
     def values(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Value]:
         """Repeated field of dynamically typed values."""
+
     def __init__(
         self,
         *,
         values: collections.abc.Iterable[global___Value] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["values", b"values"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["values", b"values"]) -> None: ...
 
 global___ListValue = ListValue
```

### Comparing `types-protobuf-4.24.0.4/google-stubs/protobuf/symbol_database.pyi` & `types-protobuf-4.25.0.20240410/google-stubs/protobuf/symbol_database.pyi`

 * *Files identical despite different names*

### Comparing `types-protobuf-4.24.0.4/google-stubs/protobuf/text_format.pyi` & `types-protobuf-4.25.0.20240410/google-stubs/protobuf/text_format.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -8,41 +8,41 @@
 from .message import Message
 
 _M = TypeVar("_M", bound=Message)  # message type (of self)
 
 class Error(Exception): ...
 
 class ParseError(Error):
-    def __init__(self, message: str | None = ..., line: int | None = ..., column: int | None = ...) -> None: ...
+    def __init__(self, message: str | None = None, line: int | None = None, column: int | None = None) -> None: ...
     def GetLine(self) -> int | None: ...
     def GetColumn(self) -> int | None: ...
 
 class TextWriter:
     def __init__(self, as_utf8: bool) -> None: ...
     def write(self, val: str) -> int: ...
     def getvalue(self) -> str: ...
     def close(self) -> None: ...
 
 _MessageFormatter: TypeAlias = Callable[[Message, int, bool], str | None]
 
 def MessageToString(
     message: Message,
-    as_utf8: bool = ...,
-    as_one_line: bool = ...,
-    use_short_repeated_primitives: bool = ...,
-    pointy_brackets: bool = ...,
-    use_index_order: bool = ...,
-    float_format: str | None = ...,
-    double_format: str | None = ...,
-    use_field_number: bool = ...,
-    descriptor_pool: DescriptorPool | None = ...,
-    indent: int = ...,
-    message_formatter: _MessageFormatter | None = ...,
-    print_unknown_fields: bool = ...,
-    force_colon: bool = ...,
+    as_utf8: bool = False,
+    as_one_line: bool = False,
+    use_short_repeated_primitives: bool = False,
+    pointy_brackets: bool = False,
+    use_index_order: bool = False,
+    float_format: str | None = None,
+    double_format: str | None = None,
+    use_field_number: bool = False,
+    descriptor_pool: DescriptorPool | None = None,
+    indent: int = 0,
+    message_formatter: _MessageFormatter | None = None,
+    print_unknown_fields: bool = False,
+    force_colon: bool = False,
 ) -> str: ...
 def MessageToBytes(
     message: Message,
     as_utf8: bool = ...,
     as_one_line: bool = ...,
     use_short_repeated_primitives: bool = ...,
     pointy_brackets: bool = ...,
@@ -55,59 +55,59 @@
     message_formatter: _MessageFormatter = ...,
     print_unknown_fields: bool = ...,
     force_colon: bool = ...,
 ) -> bytes: ...
 def PrintMessage(
     message: Message,
     out: SupportsWrite[str],
-    indent: int = ...,
-    as_utf8: bool = ...,
-    as_one_line: bool = ...,
-    use_short_repeated_primitives: bool = ...,
-    pointy_brackets: bool = ...,
-    use_index_order: bool = ...,
-    float_format: str | None = ...,
-    double_format: str | None = ...,
-    use_field_number: bool = ...,
-    descriptor_pool: DescriptorPool | None = ...,
-    message_formatter: _MessageFormatter | None = ...,
-    print_unknown_fields: bool = ...,
-    force_colon: bool = ...,
+    indent: int = 0,
+    as_utf8: bool = False,
+    as_one_line: bool = False,
+    use_short_repeated_primitives: bool = False,
+    pointy_brackets: bool = False,
+    use_index_order: bool = False,
+    float_format: str | None = None,
+    double_format: str | None = None,
+    use_field_number: bool = False,
+    descriptor_pool: DescriptorPool | None = None,
+    message_formatter: _MessageFormatter | None = None,
+    print_unknown_fields: bool = False,
+    force_colon: bool = False,
 ) -> None: ...
 def PrintField(
     field: FieldDescriptor,
     value: Any,
     out: SupportsWrite[str],
-    indent: int = ...,
-    as_utf8: bool = ...,
-    as_one_line: bool = ...,
-    use_short_repeated_primitives: bool = ...,
-    pointy_brackets: bool = ...,
-    use_index_order: bool = ...,
-    float_format: str | None = ...,
-    double_format: str | None = ...,
-    message_formatter: _MessageFormatter | None = ...,
-    print_unknown_fields: bool = ...,
-    force_colon: bool = ...,
+    indent: int = 0,
+    as_utf8: bool = False,
+    as_one_line: bool = False,
+    use_short_repeated_primitives: bool = False,
+    pointy_brackets: bool = False,
+    use_index_order: bool = False,
+    float_format: str | None = None,
+    double_format: str | None = None,
+    message_formatter: _MessageFormatter | None = None,
+    print_unknown_fields: bool = False,
+    force_colon: bool = False,
 ) -> None: ...
 def PrintFieldValue(
     field: FieldDescriptor,
     value: Any,
     out: SupportsWrite[str],
-    indent: int = ...,
-    as_utf8: bool = ...,
-    as_one_line: bool = ...,
-    use_short_repeated_primitives: bool = ...,
-    pointy_brackets: bool = ...,
-    use_index_order: bool = ...,
-    float_format: str | None = ...,
-    double_format: str | None = ...,
-    message_formatter: _MessageFormatter | None = ...,
-    print_unknown_fields: bool = ...,
-    force_colon: bool = ...,
+    indent: int = 0,
+    as_utf8: bool = False,
+    as_one_line: bool = False,
+    use_short_repeated_primitives: bool = False,
+    pointy_brackets: bool = False,
+    use_index_order: bool = False,
+    float_format: str | None = None,
+    double_format: str | None = None,
+    message_formatter: _MessageFormatter | None = None,
+    print_unknown_fields: bool = False,
+    force_colon: bool = False,
 ) -> None: ...
 
 class _Printer:
     out: SupportsWrite[str]
     indent: int
     as_utf8: bool
     as_one_line: bool
@@ -120,68 +120,68 @@
     descriptor_pool: DescriptorPool | None
     message_formatter: _MessageFormatter | None
     print_unknown_fields: bool
     force_colon: bool
     def __init__(
         self,
         out: SupportsWrite[str],
-        indent: int = ...,
-        as_utf8: bool = ...,
-        as_one_line: bool = ...,
-        use_short_repeated_primitives: bool = ...,
-        pointy_brackets: bool = ...,
-        use_index_order: bool = ...,
-        float_format: str | None = ...,
-        double_format: str | None = ...,
-        use_field_number: bool = ...,
-        descriptor_pool: DescriptorPool | None = ...,
-        message_formatter: _MessageFormatter | None = ...,
-        print_unknown_fields: bool = ...,
-        force_colon: bool = ...,
+        indent: int = 0,
+        as_utf8: bool = False,
+        as_one_line: bool = False,
+        use_short_repeated_primitives: bool = False,
+        pointy_brackets: bool = False,
+        use_index_order: bool = False,
+        float_format: str | None = None,
+        double_format: str | None = None,
+        use_field_number: bool = False,
+        descriptor_pool: DescriptorPool | None = None,
+        message_formatter: _MessageFormatter | None = None,
+        print_unknown_fields: bool = False,
+        force_colon: bool = False,
     ) -> None: ...
     def PrintMessage(self, message: Message) -> None: ...
     def PrintField(self, field: FieldDescriptor, value: Any) -> None: ...
     def PrintFieldValue(self, field: FieldDescriptor, value: Any) -> None: ...
 
 def Parse(
     text: str | bytes,
     message: _M,
-    allow_unknown_extension: bool = ...,
-    allow_field_number: bool = ...,
-    descriptor_pool: DescriptorPool | None = ...,
-    allow_unknown_field: bool = ...,
+    allow_unknown_extension: bool = False,
+    allow_field_number: bool = False,
+    descriptor_pool: DescriptorPool | None = None,
+    allow_unknown_field: bool = False,
 ) -> _M: ...
 def Merge(
     text: str | bytes,
     message: _M,
-    allow_unknown_extension: bool = ...,
-    allow_field_number: bool = ...,
-    descriptor_pool: DescriptorPool | None = ...,
-    allow_unknown_field: bool = ...,
+    allow_unknown_extension: bool = False,
+    allow_field_number: bool = False,
+    descriptor_pool: DescriptorPool | None = None,
+    allow_unknown_field: bool = False,
 ) -> _M: ...
 def MergeLines(
     lines: Iterable[str | bytes],
     message: _M,
-    allow_unknown_extension: bool = ...,
-    allow_field_number: bool = ...,
-    descriptor_pool: DescriptorPool | None = ...,
-    allow_unknown_field: bool = ...,
+    allow_unknown_extension: bool = False,
+    allow_field_number: bool = False,
+    descriptor_pool: DescriptorPool | None = None,
+    allow_unknown_field: bool = False,
 ) -> _M: ...
 
 class _Parser:
     allow_unknown_extension: bool
     allow_field_number: bool
     descriptor_pool: DescriptorPool | None
     allow_unknown_field: bool
     def __init__(
         self,
-        allow_unknown_extension: bool = ...,
-        allow_field_number: bool = ...,
-        descriptor_pool: DescriptorPool | None = ...,
-        allow_unknown_field: bool = ...,
+        allow_unknown_extension: bool = False,
+        allow_field_number: bool = False,
+        descriptor_pool: DescriptorPool | None = None,
+        allow_unknown_field: bool = False,
     ) -> None: ...
     def ParseLines(self, lines: Iterable[str | bytes], message: _M) -> _M: ...
     def MergeLines(self, lines: Iterable[str | bytes], message: _M) -> _M: ...
 
 _ParseError: TypeAlias = ParseError
 
 class Tokenizer:
@@ -206,11 +206,11 @@
     def ConsumeString(self) -> str: ...
     def ConsumeByteString(self) -> bytes: ...
     def ConsumeEnum(self, field: FieldDescriptor) -> int: ...
     def ParseErrorPreviousToken(self, message: Message) -> _ParseError: ...
     def ParseError(self, message: Message) -> _ParseError: ...
     def NextToken(self) -> None: ...
 
-def ParseInteger(text: str, is_signed: bool = ..., is_long: bool = ...) -> int: ...
+def ParseInteger(text: str, is_signed: bool = False, is_long: bool = False) -> int: ...
 def ParseFloat(text: str) -> float: ...
 def ParseBool(text: str) -> bool: ...
 def ParseEnum(field: FieldDescriptor, value: str) -> int: ...
```

### Comparing `types-protobuf-4.24.0.4/google-stubs/protobuf/timestamp_pb2.pyi` & `types-protobuf-4.25.0.20240410/google-stubs/protobuf/timestamp_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -27,29 +27,25 @@
 SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
 LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
+
 import builtins
-import sys
+import typing
 
 import google.protobuf.descriptor
 import google.protobuf.internal.well_known_types
 import google.protobuf.message
 
-if sys.version_info >= (3, 8):
-    import typing as typing_extensions
-else:
-    import typing_extensions
-
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
+@typing.final
 class Timestamp(google.protobuf.message.Message, google.protobuf.internal.well_known_types.Timestamp):
     """A Timestamp represents a point in time independent of any time zone or local
     calendar, encoded as a count of seconds and fractions of seconds at
     nanosecond resolution. The count is relative to an epoch at UTC midnight on
     January 1, 1970, in the proleptic Gregorian calendar which extends the
     Gregorian calendar backwards to year one.
 
@@ -93,24 +89,22 @@
     Example 4: Compute Timestamp from Java `System.currentTimeMillis()`.
 
         long millis = System.currentTimeMillis();
 
         Timestamp timestamp = Timestamp.newBuilder().setSeconds(millis / 1000)
             .setNanos((int) ((millis % 1000) * 1000000)).build();
 
-
     Example 5: Compute Timestamp from Java `Instant.now()`.
 
         Instant now = Instant.now();
 
         Timestamp timestamp =
             Timestamp.newBuilder().setSeconds(now.getEpochSecond())
                 .setNanos(now.getNano()).build();
 
-
     Example 6: Compute Timestamp from current time in Python.
 
         timestamp = Timestamp()
         timestamp.GetCurrentTime()
 
     # JSON Mapping
 
@@ -132,15 +126,15 @@
     standard
     [toISOString()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date/toISOString)
     method. In Python, a standard `datetime.datetime` object can be converted
     to this format using
     [`strftime`](https://docs.python.org/2/library/time.html#time.strftime) with
     the time format spec '%Y-%m-%dT%H:%M:%S.%fZ'. Likewise, in Java, one can use
     the Joda Time's [`ISODateTimeFormat.dateTime()`](
-    http://www.joda.org/joda-time/apidocs/org/joda/time/format/ISODateTimeFormat.html#dateTime%2D%2D
+    http://joda-time.sourceforge.net/apidocs/org/joda/time/format/ISODateTimeFormat.html#dateTime()
     ) to obtain a formatter capable of generating timestamps in this format.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SECONDS_FIELD_NUMBER: builtins.int
     NANOS_FIELD_NUMBER: builtins.int
@@ -157,10 +151,10 @@
     """
     def __init__(
         self,
         *,
         seconds: builtins.int | None = ...,
         nanos: builtins.int | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["nanos", b"nanos", "seconds", b"seconds"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["nanos", b"nanos", "seconds", b"seconds"]) -> None: ...
 
 global___Timestamp = Timestamp
```

### Comparing `types-protobuf-4.24.0.4/google-stubs/protobuf/type_pb2.pyi` & `types-protobuf-4.25.0.20240410/google-stubs/protobuf/type_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
 LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
+
 import builtins
 import collections.abc
 import sys
 import typing
 
 import google.protobuf.any_pb2
 import google.protobuf.descriptor
@@ -56,68 +57,80 @@
 
 class _SyntaxEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_Syntax.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     SYNTAX_PROTO2: _Syntax.ValueType  # 0
     """Syntax `proto2`."""
     SYNTAX_PROTO3: _Syntax.ValueType  # 1
     """Syntax `proto3`."""
+    SYNTAX_EDITIONS: _Syntax.ValueType  # 2
+    """Syntax `editions`."""
 
 class Syntax(_Syntax, metaclass=_SyntaxEnumTypeWrapper):
     """The syntax in which a protocol buffer element is defined."""
 
 SYNTAX_PROTO2: Syntax.ValueType  # 0
 """Syntax `proto2`."""
 SYNTAX_PROTO3: Syntax.ValueType  # 1
 """Syntax `proto3`."""
+SYNTAX_EDITIONS: Syntax.ValueType  # 2
+"""Syntax `editions`."""
 global___Syntax = Syntax
 
-@typing_extensions.final
+@typing.final
 class Type(google.protobuf.message.Message):
     """A protocol buffer message type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     FIELDS_FIELD_NUMBER: builtins.int
     ONEOFS_FIELD_NUMBER: builtins.int
     OPTIONS_FIELD_NUMBER: builtins.int
     SOURCE_CONTEXT_FIELD_NUMBER: builtins.int
     SYNTAX_FIELD_NUMBER: builtins.int
+    EDITION_FIELD_NUMBER: builtins.int
     name: builtins.str
     """The fully qualified message name."""
+    syntax: global___Syntax.ValueType
+    """The source syntax."""
+    edition: builtins.str
+    """The source edition string, only valid when syntax is SYNTAX_EDITIONS."""
     @property
     def fields(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Field]:
         """The list of fields."""
+
     @property
     def oneofs(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """The list of types appearing in `oneof` definitions in this type."""
+
     @property
     def options(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Option]:
         """The protocol buffer options."""
+
     @property
     def source_context(self) -> google.protobuf.source_context_pb2.SourceContext:
         """The source context."""
-    syntax: global___Syntax.ValueType
-    """The source syntax."""
+
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         fields: collections.abc.Iterable[global___Field] | None = ...,
         oneofs: collections.abc.Iterable[builtins.str] | None = ...,
         options: collections.abc.Iterable[global___Option] | None = ...,
         source_context: google.protobuf.source_context_pb2.SourceContext | None = ...,
         syntax: global___Syntax.ValueType | None = ...,
+        edition: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["source_context", b"source_context"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["fields", b"fields", "name", b"name", "oneofs", b"oneofs", "options", b"options", "source_context", b"source_context", "syntax", b"syntax"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["source_context", b"source_context"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["edition", b"edition", "fields", b"fields", "name", b"name", "oneofs", b"oneofs", "options", b"options", "source_context", b"source_context", "syntax", b"syntax"]) -> None: ...
 
 global___Type = Type
 
-@typing_extensions.final
+@typing.final
 class Field(google.protobuf.message.Message):
     """A single field of a message type."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _Kind:
         ValueType = typing.NewType("ValueType", builtins.int)
@@ -257,78 +270,86 @@
     """
     oneof_index: builtins.int
     """The index of the field type in `Type.oneofs`, for message or enumeration
     types. The first type has index 1; zero means the type is not in the list.
     """
     packed: builtins.bool
     """Whether to use alternative packed wire representation."""
-    @property
-    def options(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Option]:
-        """The protocol buffer options."""
     json_name: builtins.str
     """The field JSON name."""
     default_value: builtins.str
     """The string value of the default value of this field. Proto2 syntax only."""
+    @property
+    def options(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Option]:
+        """The protocol buffer options."""
+
     def __init__(
         self,
         *,
         kind: global___Field.Kind.ValueType | None = ...,
         cardinality: global___Field.Cardinality.ValueType | None = ...,
         number: builtins.int | None = ...,
         name: builtins.str | None = ...,
         type_url: builtins.str | None = ...,
         oneof_index: builtins.int | None = ...,
         packed: builtins.bool | None = ...,
         options: collections.abc.Iterable[global___Option] | None = ...,
         json_name: builtins.str | None = ...,
         default_value: builtins.str | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cardinality", b"cardinality", "default_value", b"default_value", "json_name", b"json_name", "kind", b"kind", "name", b"name", "number", b"number", "oneof_index", b"oneof_index", "options", b"options", "packed", b"packed", "type_url", b"type_url"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["cardinality", b"cardinality", "default_value", b"default_value", "json_name", b"json_name", "kind", b"kind", "name", b"name", "number", b"number", "oneof_index", b"oneof_index", "options", b"options", "packed", b"packed", "type_url", b"type_url"]) -> None: ...
 
 global___Field = Field
 
-@typing_extensions.final
+@typing.final
 class Enum(google.protobuf.message.Message):
     """Enum type definition."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     ENUMVALUE_FIELD_NUMBER: builtins.int
     OPTIONS_FIELD_NUMBER: builtins.int
     SOURCE_CONTEXT_FIELD_NUMBER: builtins.int
     SYNTAX_FIELD_NUMBER: builtins.int
+    EDITION_FIELD_NUMBER: builtins.int
     name: builtins.str
     """Enum type name."""
+    syntax: global___Syntax.ValueType
+    """The source syntax."""
+    edition: builtins.str
+    """The source edition string, only valid when syntax is SYNTAX_EDITIONS."""
     @property
     def enumvalue(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___EnumValue]:
         """Enum value definitions."""
+
     @property
     def options(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Option]:
         """Protocol buffer options."""
+
     @property
     def source_context(self) -> google.protobuf.source_context_pb2.SourceContext:
         """The source context."""
-    syntax: global___Syntax.ValueType
-    """The source syntax."""
+
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         enumvalue: collections.abc.Iterable[global___EnumValue] | None = ...,
         options: collections.abc.Iterable[global___Option] | None = ...,
         source_context: google.protobuf.source_context_pb2.SourceContext | None = ...,
         syntax: global___Syntax.ValueType | None = ...,
+        edition: builtins.str | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["source_context", b"source_context"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["enumvalue", b"enumvalue", "name", b"name", "options", b"options", "source_context", b"source_context", "syntax", b"syntax"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["source_context", b"source_context"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["edition", b"edition", "enumvalue", b"enumvalue", "name", b"name", "options", b"options", "source_context", b"source_context", "syntax", b"syntax"]) -> None: ...
 
 global___Enum = Enum
 
-@typing_extensions.final
+@typing.final
 class EnumValue(google.protobuf.message.Message):
     """Enum value definition."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     NUMBER_FIELD_NUMBER: builtins.int
@@ -336,26 +357,27 @@
     name: builtins.str
     """Enum value name."""
     number: builtins.int
     """Enum value number."""
     @property
     def options(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Option]:
         """Protocol buffer options."""
+
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         number: builtins.int | None = ...,
         options: collections.abc.Iterable[global___Option] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "number", b"number", "options", b"options"]) -> None: ...
+    def ClearField(self, field_name: typing.Literal["name", b"name", "number", b"number", "options", b"options"]) -> None: ...
 
 global___EnumValue = EnumValue
 
-@typing_extensions.final
+@typing.final
 class Option(google.protobuf.message.Message):
     """A protocol buffer option, which can be attached to a message, field,
     enumeration, etc.
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -370,17 +392,18 @@
     @property
     def value(self) -> google.protobuf.any_pb2.Any:
         """The option's value packed in an Any message. If the value is a primitive,
         the corresponding wrapper type defined in google/protobuf/wrappers.proto
         should be used. If the value is an enum, it should be stored as an int32
         value using the google.protobuf.Int32Value type.
         """
+
     def __init__(
         self,
         *,
         name: builtins.str | None = ...,
         value: google.protobuf.any_pb2.Any | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "value", b"value"]) -> None: ...
+    def HasField(self, field_name: typing.Literal["value", b"value"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing.Literal["name", b"name", "value", b"value"]) -> None: ...
 
 global___Option = Option
```

### Comparing `types-protobuf-4.24.0.4/setup.py` & `types-protobuf-4.25.0.20240410/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,47 +11,47 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `protobuf`.
 
 This version of `types-protobuf` aims to provide accurate annotations
-for `protobuf==4.24.*`.
+for `protobuf==4.25.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/protobuf. All fixes for
 types and metadata should be contributed there.
 
-Generated using [mypy-protobuf==3.5.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.5.0) on protobuf==4.21.8
+Generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) on [protobuf v25.3](https://github.com/protocolbuffers/protobuf/releases/tag/v25.3) (python protobuf==4.25.3)
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `9d345b4df42939b697a84ee461a8760eb674050e` and was tested
-with mypy 1.6.1, pyright 1.1.332, and
-pytype 2023.10.17.
+This package was generated from typeshed commit `1af2babc03ca0cbd248f5f2044e68311a671595f` and was tested
+with mypy 1.9.0, pyright 1.1.357, and
+pytype 2024.3.19.
 '''.lstrip()
 
 setup(name=name,
-      version="4.24.0.4",
+      version="4.25.0.20240410",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/protobuf.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['google-stubs'],
-      package_data={'google-stubs': ['protobuf/__init__.pyi', 'protobuf/any_pb2.pyi', 'protobuf/api_pb2.pyi', 'protobuf/compiler/__init__.pyi', 'protobuf/compiler/plugin_pb2.pyi', 'protobuf/descriptor.pyi', 'protobuf/descriptor_pb2.pyi', 'protobuf/descriptor_pool.pyi', 'protobuf/duration_pb2.pyi', 'protobuf/empty_pb2.pyi', 'protobuf/field_mask_pb2.pyi', 'protobuf/internal/__init__.pyi', 'protobuf/internal/api_implementation.pyi', 'protobuf/internal/builder.pyi', 'protobuf/internal/containers.pyi', 'protobuf/internal/decoder.pyi', 'protobuf/internal/encoder.pyi', 'protobuf/internal/enum_type_wrapper.pyi', 'protobuf/internal/extension_dict.pyi', 'protobuf/internal/message_listener.pyi', 'protobuf/internal/python_message.pyi', 'protobuf/internal/type_checkers.pyi', 'protobuf/internal/well_known_types.pyi', 'protobuf/internal/wire_format.pyi', 'protobuf/json_format.pyi', 'protobuf/message.pyi', 'protobuf/message_factory.pyi', 'protobuf/reflection.pyi', 'protobuf/service.pyi', 'protobuf/source_context_pb2.pyi', 'protobuf/struct_pb2.pyi', 'protobuf/symbol_database.pyi', 'protobuf/text_format.pyi', 'protobuf/timestamp_pb2.pyi', 'protobuf/type_pb2.pyi', 'protobuf/util/__init__.pyi', 'protobuf/wrappers_pb2.pyi', 'METADATA.toml', 'py.typed']},
+      package_data={'google-stubs': ['protobuf/__init__.pyi', 'protobuf/any_pb2.pyi', 'protobuf/api_pb2.pyi', 'protobuf/compiler/__init__.pyi', 'protobuf/compiler/plugin_pb2.pyi', 'protobuf/descriptor.pyi', 'protobuf/descriptor_pb2.pyi', 'protobuf/descriptor_pool.pyi', 'protobuf/duration_pb2.pyi', 'protobuf/empty_pb2.pyi', 'protobuf/field_mask_pb2.pyi', 'protobuf/internal/__init__.pyi', 'protobuf/internal/api_implementation.pyi', 'protobuf/internal/builder.pyi', 'protobuf/internal/containers.pyi', 'protobuf/internal/decoder.pyi', 'protobuf/internal/encoder.pyi', 'protobuf/internal/enum_type_wrapper.pyi', 'protobuf/internal/extension_dict.pyi', 'protobuf/internal/message_listener.pyi', 'protobuf/internal/python_message.pyi', 'protobuf/internal/type_checkers.pyi', 'protobuf/internal/well_known_types.pyi', 'protobuf/internal/wire_format.pyi', 'protobuf/json_format.pyi', 'protobuf/message.pyi', 'protobuf/message_factory.pyi', 'protobuf/reflection.pyi', 'protobuf/service.pyi', 'protobuf/source_context_pb2.pyi', 'protobuf/struct_pb2.pyi', 'protobuf/symbol_database.pyi', 'protobuf/text_format.pyi', 'protobuf/timestamp_pb2.pyi', 'protobuf/type_pb2.pyi', 'protobuf/util/__init__.pyi', 'protobuf/wrappers_pb2.pyi', 'METADATA.toml', 'protobuf/py.typed']},
       license="Apache-2.0 license",
-      python_requires=">=3.7",
+      python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-protobuf-4.24.0.4/types_protobuf.egg-info/PKG-INFO` & `types-protobuf-4.25.0.20240410/types_protobuf.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: types-protobuf
-Version: 4.24.0.4
+Version: 4.25.0.20240410
 Summary: Typing stubs for protobuf
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/protobuf.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ## Typing stubs for protobuf
 
 This is a [PEP 561](https://peps.python.org/pep-0561/)
 type stub package for the [`protobuf`](https://github.com/protocolbuffers/protobuf) package.
 It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `protobuf`.
 
 This version of `types-protobuf` aims to provide accurate annotations
-for `protobuf==4.24.*`.
+for `protobuf==4.25.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/protobuf. All fixes for
 types and metadata should be contributed there.
 
-Generated using [mypy-protobuf==3.5.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.5.0) on protobuf==4.21.8
+Generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) on [protobuf v25.3](https://github.com/protocolbuffers/protobuf/releases/tag/v25.3) (python protobuf==4.25.3)
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `9d345b4df42939b697a84ee461a8760eb674050e` and was tested
-with mypy 1.6.1, pyright 1.1.332, and
-pytype 2023.10.17.
+This package was generated from typeshed commit `1af2babc03ca0cbd248f5f2044e68311a671595f` and was tested
+with mypy 1.9.0, pyright 1.1.357, and
+pytype 2024.3.19.
```

### Comparing `types-protobuf-4.24.0.4/types_protobuf.egg-info/SOURCES.txt` & `types-protobuf-4.25.0.20240410/types_protobuf.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 google-stubs/protobuf/descriptor_pool.pyi
 google-stubs/protobuf/duration_pb2.pyi
 google-stubs/protobuf/empty_pb2.pyi
 google-stubs/protobuf/field_mask_pb2.pyi
 google-stubs/protobuf/json_format.pyi
 google-stubs/protobuf/message.pyi
 google-stubs/protobuf/message_factory.pyi
+google-stubs/protobuf/py.typed
 google-stubs/protobuf/reflection.pyi
 google-stubs/protobuf/service.pyi
 google-stubs/protobuf/source_context_pb2.pyi
 google-stubs/protobuf/struct_pb2.pyi
 google-stubs/protobuf/symbol_database.pyi
 google-stubs/protobuf/text_format.pyi
 google-stubs/protobuf/timestamp_pb2.pyi
```

