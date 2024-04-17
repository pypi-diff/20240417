# Comparing `tmp/interopt-0.1.0.tar.gz` & `tmp/interopt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interopt-0.1.0.tar", last modified: Sat Mar  2 16:06:07 2024, max compression
+gzip compressed data, was "interopt-0.1.1.tar", last modified: Wed Apr 17 00:19:05 2024, max compression
```

## Comparing `interopt-0.1.0.tar` & `interopt-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 jacobot   (1000) jacobot   (1000)        0 2024-03-02 16:06:07.137494 interopt-0.1.0/
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)      386 2024-03-02 16:06:07.137494 interopt-0.1.0/PKG-INFO
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)        0 2024-02-24 20:08:52.000000 interopt-0.1.0/README.md
-drwxr-xr-x   0 jacobot   (1000) jacobot   (1000)        0 2024-03-02 16:06:07.134160 interopt-0.1.0/interopt/
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)       32 2024-02-27 12:30:04.000000 interopt-0.1.0/interopt/__init__.py
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)      854 2024-03-02 14:02:17.000000 interopt-0.1.0/interopt/__main__.py
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)      310 2024-02-26 09:45:20.000000 interopt-0.1.0/interopt/definition.py
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)     4254 2024-02-27 11:43:23.000000 interopt-0.1.0/interopt/parameter.py
-drwxr-xr-x   0 jacobot   (1000) jacobot   (1000)        0 2024-03-02 16:06:07.134160 interopt-0.1.0/interopt/runner/
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)        0 2024-02-24 20:52:11.000000 interopt-0.1.0/interopt/runner/__init__.py
-drwxr-xr-x   0 jacobot   (1000) jacobot   (1000)        0 2024-03-02 16:06:07.137494 interopt-0.1.0/interopt/runner/grpc_runner/
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)       29 2024-02-25 07:25:19.000000 interopt-0.1.0/interopt/runner/grpc_runner/__init__.py
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)     4616 2024-02-13 14:31:34.000000 interopt-0.1.0/interopt/runner/grpc_runner/config_service_pb2.py
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)     4270 2024-02-24 20:39:48.000000 interopt-0.1.0/interopt/runner/grpc_runner/config_service_pb2_grpc.py
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)     3007 2024-03-02 13:28:01.000000 interopt-0.1.0/interopt/runner/grpc_runner/main.py
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)     3564 2024-03-02 15:54:13.000000 interopt-0.1.0/interopt/runner/grpc_runner/server.py
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)     4004 2024-03-02 14:33:02.000000 interopt-0.1.0/interopt/runner/model.py
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)     1249 2024-02-28 10:57:13.000000 interopt-0.1.0/interopt/search_space.py
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)    11356 2024-03-02 14:33:13.000000 interopt-0.1.0/interopt/study.py
-drwxr-xr-x   0 jacobot   (1000) jacobot   (1000)        0 2024-03-02 16:06:07.137494 interopt-0.1.0/interopt.egg-info/
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)      386 2024-03-02 16:06:07.000000 interopt-0.1.0/interopt.egg-info/PKG-INFO
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)      579 2024-03-02 16:06:07.000000 interopt-0.1.0/interopt.egg-info/SOURCES.txt
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)        1 2024-03-02 16:06:07.000000 interopt-0.1.0/interopt.egg-info/dependency_links.txt
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)       58 2024-03-02 16:06:07.000000 interopt-0.1.0/interopt.egg-info/requires.txt
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)        9 2024-03-02 16:06:07.000000 interopt-0.1.0/interopt.egg-info/top_level.txt
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)       38 2024-03-02 16:06:07.137494 interopt-0.1.0/setup.cfg
--rw-r--r--   0 jacobot   (1000) jacobot   (1000)      581 2024-02-24 20:08:49.000000 interopt-0.1.0/setup.py
+drwxr-xr-x   0 jacobot   (1000) jacobot   (1000)        0 2024-04-17 00:19:05.528967 interopt-0.1.1/
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)      410 2024-04-17 00:19:05.528967 interopt-0.1.1/PKG-INFO
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)        0 2024-02-24 20:08:52.000000 interopt-0.1.1/README.md
+drwxr-xr-x   0 jacobot   (1000) jacobot   (1000)        0 2024-04-17 00:19:05.525633 interopt-0.1.1/interopt/
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)       32 2024-02-27 12:30:04.000000 interopt-0.1.1/interopt/__init__.py
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)      856 2024-03-27 12:26:56.000000 interopt-0.1.1/interopt/__main__.py
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)      310 2024-02-26 09:45:20.000000 interopt-0.1.1/interopt/definition.py
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)     4581 2024-03-29 18:29:35.000000 interopt-0.1.1/interopt/parameter.py
+drwxr-xr-x   0 jacobot   (1000) jacobot   (1000)        0 2024-04-17 00:19:05.528967 interopt-0.1.1/interopt/runner/
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)        0 2024-02-24 20:52:11.000000 interopt-0.1.1/interopt/runner/__init__.py
+drwxr-xr-x   0 jacobot   (1000) jacobot   (1000)        0 2024-04-17 00:19:05.528967 interopt-0.1.1/interopt/runner/grpc_runner/
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)       29 2024-02-25 07:25:19.000000 interopt-0.1.1/interopt/runner/grpc_runner/__init__.py
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)     4705 2024-03-13 12:40:56.000000 interopt-0.1.1/interopt/runner/grpc_runner/config_service_pb2.py
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)     5201 2024-03-13 12:40:56.000000 interopt-0.1.1/interopt/runner/grpc_runner/config_service_pb2.pyi
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)     4270 2024-03-13 12:41:56.000000 interopt-0.1.1/interopt/runner/grpc_runner/config_service_pb2_grpc.py
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)     2705 2024-03-27 13:19:28.000000 interopt-0.1.1/interopt/runner/grpc_runner/main.py
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)     3706 2024-03-13 11:15:32.000000 interopt-0.1.1/interopt/runner/grpc_runner/server.py
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)     4140 2024-04-05 20:08:17.000000 interopt-0.1.1/interopt/runner/model.py
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)     1462 2024-03-27 12:36:55.000000 interopt-0.1.1/interopt/search_space.py
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)    12472 2024-04-05 20:36:54.000000 interopt-0.1.1/interopt/study.py
+drwxr-xr-x   0 jacobot   (1000) jacobot   (1000)        0 2024-04-17 00:19:05.528967 interopt-0.1.1/interopt.egg-info/
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)      410 2024-04-17 00:19:05.000000 interopt-0.1.1/interopt.egg-info/PKG-INFO
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)      630 2024-04-17 00:19:05.000000 interopt-0.1.1/interopt.egg-info/SOURCES.txt
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)        1 2024-04-17 00:19:05.000000 interopt-0.1.1/interopt.egg-info/dependency_links.txt
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)       67 2024-04-17 00:19:05.000000 interopt-0.1.1/interopt.egg-info/requires.txt
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)        9 2024-04-17 00:19:05.000000 interopt-0.1.1/interopt.egg-info/top_level.txt
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)       38 2024-04-17 00:19:05.528967 interopt-0.1.1/setup.cfg
+-rw-r--r--   0 jacobot   (1000) jacobot   (1000)      601 2024-04-17 00:16:53.000000 interopt-0.1.1/setup.py
```

### Comparing `interopt-0.1.0/interopt/__main__.py` & `interopt-0.1.1/interopt/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def main():
     parser = argparse.ArgumentParser(description="Run a benchmark")
     parser.add_argument('--servers', type=str, help='Benchmark to use', default="spmm")
 
     args = parser.parse_args()
     study = Study(benchmark_name='spmm', definition=get_spmm_definition(),
                   enable_tabular=True, enable_model=True, dataset='10k',
-                  objectives=['compute_time'], server_address=args.servers)
+                  objectives=['compute_time'], server_addresses=args.servers)
     server = Server(study, port=50050)
     server.start()
     #print(study.query({
     #    'tuned_sp0': 4096,
     #    'tuned_gs0': 16,
     #    'tuned_stride': 2,
     #    'tuned_sp1': 1024,
```

### Comparing `interopt-0.1.0/interopt/parameter.py` & `interopt-0.1.1/interopt/parameter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from enum import Enum
 from typing import Any, Union, Type, Callable
+import re
 
 class Configuration:
     def __init__(self, parameters: dict):
         self.parameters = parameters
 
     def to_dict(self):
         return self.parameters
@@ -87,30 +88,39 @@
 
 class Constraint:
     def __init__(self, constraint: Union[Callable[[Any], Any], str]):
         self.constraint = constraint
 
     @staticmethod
     def _as_dict_string(input_str: str, variable_names: list[str]) -> str:
-        for var_name in variable_names:
-            input_str = input_str.replace(var_name, f"x['{var_name}']")
+        for var_name in sorted(variable_names, key=len, reverse=True):
+            pattern = r'\b' + re.escape(var_name) + r'\b'
+            replacement = f"x['{var_name}']"
+            input_str = re.sub(pattern, replacement, input_str)
         return input_str
 
     @staticmethod
     def as_dict_lambda(input_str: str, variable_names: list[str]) -> Callable[[Any], Any]:
         return Constraint._string_as_lambda(Constraint._as_dict_string(input_str, variable_names))
 
     @staticmethod
     def _string_as_lambda(input_str: str) -> Callable[[Any], Any]:
         return eval(f"lambda x: ({input_str})")
 
     @classmethod
     def from_dict(cls, d: dict):
         return cls(**d)
 
+    def direct_eval(self, x: dict) -> bool:
+        return eval(self.constraint, {}, x)
+
+    # Implement callable
+    def __call__(self, x: dict) -> bool:
+        return self.direct_eval(x)
+
 
 def string_to_param_type(param_type_str: str) -> ParamType:
     return ParamType[param_type_str.upper()]
 
 def param_type_to_class(param_type: ParamType) -> Type[Param]:
     # Inspect all subclasses of Param to find the matching param_type_enum
     for cls in Param.__subclasses__():
```

### Comparing `interopt-0.1.0/interopt/runner/grpc_runner/config_service_pb2.py` & `interopt-0.1.1/interopt/runner/grpc_runner/config_service_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: config_service.proto
+# Protobuf Python Version: 4.25.0
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14\x63onfig_service.proto\"#\n\x0fShutdownRequest\x12\x10\n\x08shutdown\x18\x01 \x01(\x08\"#\n\x10ShutdownResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"X\n\x14\x43onfigurationRequest\x12&\n\x0e\x63onfigurations\x18\x01 \x01(\x0b\x32\x0e.Configuration\x12\x18\n\x10output_data_file\x18\x02 \x01(\t\"\x82\x01\n\rConfiguration\x12\x32\n\nparameters\x18\x01 \x03(\x0b\x32\x1e.Configuration.ParametersEntry\x1a=\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x19\n\x05value\x18\x02 \x01(\x0b\x32\n.Parameter:\x02\x38\x01\"\x91\x02\n\tParameter\x12&\n\rinteger_param\x18\x01 \x01(\x0b\x32\r.IntegerParamH\x00\x12 \n\nreal_param\x18\x02 \x01(\x0b\x32\n.RealParamH\x00\x12.\n\x11\x63\x61tegorical_param\x18\x03 \x01(\x0b\x32\x11.CategoricalParamH\x00\x12&\n\rordinal_param\x18\x04 \x01(\x0b\x32\r.OrdinalParamH\x00\x12$\n\x0cstring_param\x18\x05 \x01(\x0b\x32\x0c.StringParamH\x00\x12.\n\x11permutation_param\x18\x06 \x01(\x0b\x32\x11.PermutationParamH\x00\x42\x0c\n\nparam_type\"\x1d\n\x0cIntegerParam\x12\r\n\x05value\x18\x01 \x01(\x05\"\x1a\n\tRealParam\x12\r\n\x05value\x18\x01 \x01(\x02\"!\n\x10\x43\x61tegoricalParam\x12\r\n\x05value\x18\x01 \x01(\x05\"\x1d\n\x0cOrdinalParam\x12\r\n\x05value\x18\x01 \x01(\x05\"\x1c\n\x0bStringParam\x12\r\n\x05value\x18\x01 \x01(\t\"\"\n\x10PermutationParam\x12\x0e\n\x06values\x18\x01 \x03(\x05\"n\n\x15\x43onfigurationResponse\x12\x18\n\x07metrics\x18\x01 \x03(\x0b\x32\x07.Metric\x12\x1e\n\ntimestamps\x18\x02 \x01(\x0b\x32\n.Timestamp\x12\x1b\n\x08\x66\x65\x61sible\x18\x03 \x01(\x0b\x32\t.Feasible\"\x18\n\x06Metric\x12\x0e\n\x06values\x18\x01 \x03(\x01\"\x1e\n\tTimestamp\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\"\x19\n\x08\x46\x65\x61sible\x12\r\n\x05value\x18\x01 \x01(\x08\x32\x97\x01\n\x14\x43onfigurationService\x12N\n\x1dRunConfigurationsClientServer\x12\x15.ConfigurationRequest\x1a\x16.ConfigurationResponse\x12/\n\x08Shutdown\x12\x10.ShutdownRequest\x1a\x11.ShutdownResponseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14\x63onfig_service.proto\"#\n\x0fShutdownRequest\x12\x10\n\x08shutdown\x18\x01 \x01(\x08\"#\n\x10ShutdownResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"X\n\x14\x43onfigurationRequest\x12&\n\x0e\x63onfigurations\x18\x01 \x01(\x0b\x32\x0e.Configuration\x12\x18\n\x10output_data_file\x18\x02 \x01(\t\"\x82\x01\n\rConfiguration\x12\x32\n\nparameters\x18\x01 \x03(\x0b\x32\x1e.Configuration.ParametersEntry\x1a=\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x19\n\x05value\x18\x02 \x01(\x0b\x32\n.Parameter:\x02\x38\x01\"\x91\x02\n\tParameter\x12&\n\rinteger_param\x18\x01 \x01(\x0b\x32\r.IntegerParamH\x00\x12 \n\nreal_param\x18\x02 \x01(\x0b\x32\n.RealParamH\x00\x12.\n\x11\x63\x61tegorical_param\x18\x03 \x01(\x0b\x32\x11.CategoricalParamH\x00\x12&\n\rordinal_param\x18\x04 \x01(\x0b\x32\r.OrdinalParamH\x00\x12$\n\x0cstring_param\x18\x05 \x01(\x0b\x32\x0c.StringParamH\x00\x12.\n\x11permutation_param\x18\x06 \x01(\x0b\x32\x11.PermutationParamH\x00\x42\x0c\n\nparam_type\"\x1d\n\x0cIntegerParam\x12\r\n\x05value\x18\x01 \x01(\x05\"\x1a\n\tRealParam\x12\r\n\x05value\x18\x01 \x01(\x02\"!\n\x10\x43\x61tegoricalParam\x12\r\n\x05value\x18\x01 \x01(\x05\"\x1d\n\x0cOrdinalParam\x12\r\n\x05value\x18\x01 \x01(\x05\"\x1c\n\x0bStringParam\x12\r\n\x05value\x18\x01 \x01(\t\"\"\n\x10PermutationParam\x12\x0e\n\x06values\x18\x01 \x03(\x05\"n\n\x15\x43onfigurationResponse\x12\x18\n\x07metrics\x18\x01 \x03(\x0b\x32\x07.Metric\x12\x1e\n\ntimestamps\x18\x02 \x01(\x0b\x32\n.Timestamp\x12\x1b\n\x08\x66\x65\x61sible\x18\x03 \x01(\x0b\x32\t.Feasible\"&\n\x06Metric\x12\x0e\n\x06values\x18\x01 \x03(\x01\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x1e\n\tTimestamp\x12\x11\n\ttimestamp\x18\x01 \x01(\x03\"\x19\n\x08\x46\x65\x61sible\x12\r\n\x05value\x18\x01 \x01(\x08\x32\x97\x01\n\x14\x43onfigurationService\x12N\n\x1dRunConfigurationsClientServer\x12\x15.ConfigurationRequest\x1a\x16.ConfigurationResponse\x12/\n\x08Shutdown\x12\x10.ShutdownRequest\x1a\x11.ShutdownResponseb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'config_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
   DESCRIPTOR._options = None
-  _CONFIGURATION_PARAMETERSENTRY._options = None
-  _CONFIGURATION_PARAMETERSENTRY._serialized_options = b'8\001'
+  _globals['_CONFIGURATION_PARAMETERSENTRY']._options = None
+  _globals['_CONFIGURATION_PARAMETERSENTRY']._serialized_options = b'8\001'
   _globals['_SHUTDOWNREQUEST']._serialized_start=24
   _globals['_SHUTDOWNREQUEST']._serialized_end=59
   _globals['_SHUTDOWNRESPONSE']._serialized_start=61
   _globals['_SHUTDOWNRESPONSE']._serialized_end=96
   _globals['_CONFIGURATIONREQUEST']._serialized_start=98
   _globals['_CONFIGURATIONREQUEST']._serialized_end=186
   _globals['_CONFIGURATION']._serialized_start=189
@@ -46,15 +46,15 @@
   _globals['_STRINGPARAM']._serialized_start=722
   _globals['_STRINGPARAM']._serialized_end=750
   _globals['_PERMUTATIONPARAM']._serialized_start=752
   _globals['_PERMUTATIONPARAM']._serialized_end=786
   _globals['_CONFIGURATIONRESPONSE']._serialized_start=788
   _globals['_CONFIGURATIONRESPONSE']._serialized_end=898
   _globals['_METRIC']._serialized_start=900
-  _globals['_METRIC']._serialized_end=924
-  _globals['_TIMESTAMP']._serialized_start=926
-  _globals['_TIMESTAMP']._serialized_end=956
-  _globals['_FEASIBLE']._serialized_start=958
-  _globals['_FEASIBLE']._serialized_end=983
-  _globals['_CONFIGURATIONSERVICE']._serialized_start=986
-  _globals['_CONFIGURATIONSERVICE']._serialized_end=1137
+  _globals['_METRIC']._serialized_end=938
+  _globals['_TIMESTAMP']._serialized_start=940
+  _globals['_TIMESTAMP']._serialized_end=970
+  _globals['_FEASIBLE']._serialized_start=972
+  _globals['_FEASIBLE']._serialized_end=997
+  _globals['_CONFIGURATIONSERVICE']._serialized_start=1000
+  _globals['_CONFIGURATIONSERVICE']._serialized_end=1151
 # @@protoc_insertion_point(module_scope)
```

### Comparing `interopt-0.1.0/interopt/runner/grpc_runner/config_service_pb2_grpc.py` & `interopt-0.1.1/interopt/runner/grpc_runner/config_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `interopt-0.1.0/interopt/runner/grpc_runner/main.py` & `interopt-0.1.1/interopt/runner/grpc_runner/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -34,38 +34,33 @@
     parameter_names = [param.name for param in parameters]
     parameter_types = [param.param_type_enum for param in parameters]
     query_dict_list = []
     for name, value in query_dict.items():
         if name not in parameter_names:
             raise ValueError(f"Unknown parameter: {name}")
         query_dict_list.append([name, value, parameter_types[parameter_names.index(name)]])
-    #print(f"Parameter names: {parameter_names}")
-    #print(f"Query_dict: {query_dict}")
-    #print(f"Query_dict_list: {query_dict_list}")
     query_dict_grpc = {
         name: value_to_param(value, param_type)
-        for name, value, param_type in query_dict_list #zip(parameter_names, query_dict.values(), parameter_types)
+        for name, value, param_type in query_dict_list
     }
-    #print(f"Query_dict_grpc: {query_dict_grpc}")
     config = cs.Configuration(parameters=query_dict_grpc)
-    result = []
+    result = {}
 
     async with grpc.aio.insecure_channel(grpc_url) as channel:
         stub = cs_grpc.ConfigurationServiceStub(channel)
         request = cs.ConfigurationRequest(
             configurations=config,
             output_data_file="test"
         )
         try:
-            #print(f"Sending request: {request}")
-            #print(f"Sending request: {request}")
             response = await stub.RunConfigurationsClientServer(request)
             #print(f"Received response: {response}")
-            #print(response)
-            result = [metric.values for metric in response.metrics]
+            for metric in response.metrics:
+                result[metric.name] = metric.values
+            #print(f"Received result: {result}")
         except grpc.aio.AioRpcError as e:
             print(e.with_traceback(None))
             # Extracting the status code
             status_code = e.code()
             print(f"Status code: {status_code}")
 
             # Extracting the details
```

### Comparing `interopt-0.1.0/interopt/runner/grpc_runner/server.py` & `interopt-0.1.1/interopt/runner/grpc_runner/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,18 @@
     async def convert_response(self, result):
         #print(f"Metrics: {result}")
         #print(f"Metrics: {cs.Metric(values=[result['compute_time']])}")
         #metrics = [
         #    cs.Metric(values=metric)
         #    for metric in result
         #]
-        metrics = [cs.Metric(values=[result['compute_time']])]
+        metrics = []
+        for obj in self.study.enabled_objectives:
+            metrics.append(cs.Metric(name=obj, values=[result[obj]]))
+        #metrics = [cs.Metric(values=[result['compute_time']])]
         #print(f"Metrics: {metrics}")
         return cs.ConfigurationResponse(
             metrics=metrics,
             timestamps=cs.Timestamp(timestamp=int()),
             feasible=cs.Feasible(value=True)
         )
```

### Comparing `interopt-0.1.0/interopt/runner/model.py` & `interopt-0.1.1/interopt/runner/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import ast
 import os
 
+import numpy as np
+
 from sklearn.model_selection import train_test_split
 from sklearn.metrics import mean_squared_error, mean_absolute_error, r2_score
 
-from autogluon.tabular import TabularDataset, TabularPredictor
+#from autogluon.tabular import TabularDataset, TabularPredictor
 from catboost import CatBoostRegressor
 
 def load_catboost_models(tab, benchmark_name, dataset, objectives, features):
     models = {}
     for objective in objectives:
         model_root = 'models'
         os.mkdir(model_root) if not os.path.exists(model_root) else None
@@ -52,39 +54,42 @@
         models = load_catboost_models(tab, benchmark_name, dataset, objectives, features)
     else:
         models = load_autogluon_models(tab, benchmark_name, dataset, objectives, features)
     return models
 
 def train_model(input_tab, objective, benchmark_name, in_features):
     features = in_features.copy()
-    features.remove('permutation')
     tab = input_tab.copy()
     tab.reset_index(inplace=True)
-    tab['tuple_str'] = tab['permutation'].apply(ast.literal_eval)
-    for i in range(5):
-        tab[f'tuple_permutation_{i}'] = tab['tuple_str'].apply(lambda x: x[i])
-    features.extend([f'tuple_permutation_{i}' for i in range(5)])
+    if "permutation" in features:
+        features.remove('permutation')
+        tab['tuple_str'] = tab['permutation'].apply(ast.literal_eval)
+        for i in range(5):
+            tab[f'tuple_permutation_{i}'] = tab['tuple_str'].apply(lambda x: x[i])
+        features.extend([f'tuple_permutation_{i}' for i in range(5)])
 
     # Assume 'df' is your DataFrame
     X = tab[features]
 
     y = tab[objective]
+    # Convert the y vector into a log scale
+    y = np.log(y)
 
     # Splitting the dataset
     X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)
 
     # Initialize CatBoostRegressor
     if catboost:
         catboost_model = CatBoostRegressor(silent=True)
 
         # Fit model
         catboost_model.fit(X_train, y_train)
         y_pred = catboost_model.predict(X_test)
     else:
-        # Autogluon expects the complete dataframe as input, e.g. both X and Y in one dataframe 
+        # Autogluon expects the complete dataframe as input, e.g. both X and Y in one dataframe
         df_train = X_train.copy()
         df_train[objective] = y_train
         print(df_train.head(), df_train.shape, df_train.columns)
         autogluon_model = TabularPredictor(label=objective, path='models').fit(
             train_data=TabularDataset(df_train), presets='high_quality', time_limit=180)
         y_pred = autogluon_model.predict(X_test)
         df_test = X_test.copy()
```

### Comparing `interopt-0.1.0/interopt/search_space.py` & `interopt-0.1.1/interopt/search_space.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from typing import Union
 from interopt.parameter import Param, Constraint, string_to_param_type, param_type_to_class
 
-class Objective:
-    def __init__(self, name: str, minimize: bool):
+class Metric:
+    def __init__(self, name: str, index: int, singular: bool):
         self.name = name
-        self.minimize = minimize
+        self.index = index
+        self.singular = singular
 
     @staticmethod
     def from_dict(d: dict):
-        return Objective(d['name'], d['minimize'])
+        return Metric(d['name'], d['index'], d['singular'])
 
-class Metric:
-    def __init__(self, name: str):
+class Objective:
+    def __init__(self, name: str, metric: Metric, minimize: bool):
         self.name = name
+        assert self.name == metric.name
+        self.metric = metric
+        self.minimize = minimize
 
     @staticmethod
     def from_dict(d: dict):
-        return Metric(d['name'])
+        return Objective(d['name'], d['metric'], d['minimize'])
 
 class SearchSpace():
     def __init__(self, params: Union[list[Param], list[dict]],
                  metrics: list[Metric], objectives: list[Objective],
                  constraints: list[Constraint] = []):
         if isinstance(params[0], dict):
             self.params = [self.dict_to_param(p) for p in params]
```

### Comparing `interopt-0.1.0/interopt/study.py` & `interopt-0.1.1/interopt/study.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,34 +3,41 @@
 import requests
 import asyncio
 
 from typing import Optional
 from enum import Enum, auto
 
 import pandas as pd
+import numpy as np
 
 from interopt.runner.grpc_runner import run_config
 from interopt.runner.model import load_models
 from interopt.definition import ProblemDefinition
 
 class TabularDataset:
-    def __init__(self, benchmark_name, dataset, parameter_names, objectives):
+    def __init__(self, benchmark_name, dataset, parameter_names, objectives, enable_download):
         self.objectives = objectives
-        success = self.ensure_dataset_downloaded(benchmark_name, dataset)
-        if success:
-            file_path = f'datasets/{benchmark_name}_{dataset}.csv'
-            self.tab = pd.read_csv(file_path).dropna()
-            print(self.tab)
+        self.tab = None
+        self.parameter_names = parameter_names
+        self.tab_path = f'datasets/{benchmark_name}_{dataset}.csv'
+        if os.path.exists(self.tab_path):
+            self.tab = pd.read_csv(self.tab_path).dropna()
+        elif enable_download:
+            success = self.ensure_dataset_downloaded(benchmark_name, dataset)
+            if success:
+                self.tab = pd.read_csv(self.tab_path).dropna()
+                print(self.tab)
+        if self.tab is None:
+            multi_index = pd.MultiIndex.from_tuples([], names=self.parameter_names)
+            self.tab = pd.DataFrame(columns=parameter_names + objectives, index=multi_index)
         else:
-            self.tab = pd.DataFrame(columns=parameter_names + objectives)
+            self.tab.set_index(parameter_names, inplace=True)
+            self.tab.sort_index(inplace=True)
         #self.load_and_prepare_dataset(parameter_names)
         self.query_tab = self.tab.copy()
-        #print(self.query_tab)
-        self.query_tab.set_index(parameter_names, inplace=True)
-        self.query_tab.sort_index(inplace=True)
 
     #def load_and_prepare_dataset(self, parameter_names):
         #self.tab['energy_consumptions'] = self.tab['energy_consumptions'].apply(
         #    ast.literal_eval)
         #self.tab['energy'] = self.tab['energy_consumptions'].apply(
         #    lambda x: sum(x)/len(x) if len(x) > 0 else 0)
         # Set the index for the query_tab, modify as needed for each benchmark
@@ -58,34 +65,51 @@
             print(f"Downloaded {local_file_path}")
             return True
         except requests.exceptions.HTTPError as e:
             print(f"Failed to download {url}: {e}")
             return False
 
     def query(self, query_dict) -> Optional[pd.Series]:
-        #print(f"Query: {query_dict}")
-        #print(f"Index: {self.query_tab.index.names}")
         query_tuple = tuple(query_dict[col] for col in self.query_tab.index.names)
         if query_tuple in self.query_tab.index:
             print("Using tabular data")
             query_result: pd.Series = self.query_tab.loc[query_tuple][self.objectives]
             return query_result
         #print("Query not found in tabular data")
         return None
 
+    def write(self, result):
+        # Check if the CSV file exists
+        file_exists = os.path.isfile(self.tab_path)
+
+        # If file exists, append without header; otherwise, write with header
+        write_result = result.reset_index()
+        if file_exists:
+            write_result.to_csv(self.tab_path, mode='a', sep=",",
+                          index=False, header=False)
+        else:
+            write_result.to_csv(self.tab_path, mode='w', sep=",",
+                          index=False, header=True)
+
+    def add(self, result):
+        self.write(result)
+        self.query_tab = pd.concat([self.query_tab, result])
+
+
+
 
 class SoftwareQuery:
-    def __init__(self, benchmark_name, dataset, parameter_names, objectives,
-                 enable_tabular, enable_model):
+    def __init__(self, benchmark_name, dataset, parameter_names, enabled_objectives,
+                 enable_tabular, enable_model, enable_download):
         self.tabular_dataset = TabularDataset(
-            benchmark_name, dataset, parameter_names, objectives)
+            benchmark_name, dataset, parameter_names, enabled_objectives, enable_download)
         if enable_model:
             self.models = load_models(
                 self.tabular_dataset.query_tab, benchmark_name, dataset,
-                objectives, parameter_names)
+                enabled_objectives, parameter_names)
         self.query_tab = self.tabular_dataset.query_tab
         self.enable_tabular = enable_tabular
         self.enable_model = enable_model
         #print(f"Enable tabular: {enable_tabular}")
         #print(f"Enable model: {enable_model}")
 
     def get_objectives(self):
@@ -100,25 +124,32 @@
             #print(f"Query result: {query_result}")
         if query_result is None and self.enable_model:
             # Use surrogate model, query is not available in the table
             query_result: pd.Series = self.query_model(query_dict)
             #print(f"Query result: {query_result}")
 
         if query_result is not None:
-            return query_result.to_frame().T
+            #return query_result.to_frame().T
+            return query_result
 
         return None
 
     def query_model(self, query_dict) -> pd.Series:
-        model_query_dict = self.convert_permutation_to_tuple(query_dict, 'permutation')
+        if "permutation" in query_dict.keys():
+            model_query_dict = self.convert_permutation_to_tuple(query_dict, 'permutation')
+        else:
+            model_query_dict = query_dict
 
         print("Using surrogate model")
         results = [self.models[objective].predict(pd.DataFrame([model_query_dict]))[0]
                    for objective in self.get_objectives()]
 
+        # Convert from log scale back to normal
+        results = [np.exp(result) for result in results]
+
         return pd.DataFrame([results], columns=self.get_objectives(),
                           index=[tuple(query_dict.values())]).iloc[0]
 
     def convert_permutation_to_tuple(self, query_dict: dict, param: str) -> list[int]:
         new_dict = query_dict.copy()
         tuple_str = ast.literal_eval(new_dict[param])
         for i, value in enumerate(tuple_str):
@@ -137,34 +168,35 @@
         self.queue = asyncio.Queue()
         self.server_availability = {url: True for url in self.grpc_urls}
         self.available_server_event = asyncio.Event()
         self.available_server_event.set()
         self.lock = asyncio.Lock()
 
     async def get_available_server_url(self):
-        await self.available_server_event.wait()  # Wait until a server is available
-        async with self.lock:
-            for url, is_available in self.server_availability.items():
-                if is_available:
-                    self.server_availability[url] = False  # Mark the server as busy
-                    if not any(self.server_availability.values()):  # Check if all servers are now busy
-                        self.available_server_event.clear()  # Clear the event to wait again
-                    return url
-
+        while True:
+            async with self.lock:
+                for url, is_available in self.server_availability.items():
+                    if is_available:
+                        self.server_availability[url] = False  # Mark the server as busy
+                        if not any(self.server_availability.values()): # Check if all servers are now busy
+                            self.available_server_event.clear()  # Clear the event to wait again
+                        return url # If no available servers found, wait for one to become available
+            await self.available_server_event.wait()
 
     async def mark_server_as_available(self, url):
         async with self.lock:
             self.server_availability[url] = True
             self.available_server_event.set()  # Signal that at least one server is available
 
 class GRPCQuery:
     def __init__(self, grpc_urls, parameters,
-                 objectives):
+                 enabled_objectives, definition: ProblemDefinition):
         self.parameters = parameters
-        self.objectives = objectives
+        self.enabled_objectives = enabled_objectives
+        self.definition = definition
         self.queue_handler = QueueHandler(grpc_urls)
 
     async def send_queries_to_servers(self, query: dict) -> dict:
         return await self.send_query(query)
 
     async def send_query(self, query: dict) -> dict:
         url = await self.queue_handler.get_available_server_url()
@@ -178,101 +210,92 @@
     async def query_hardware(self, query: dict) -> pd.DataFrame:
         # Implement or override as needed
         result = await self.send_queries_to_servers(query)
         result = await self.process_grpc_results(result, query)
         return result
 
     async def process_grpc_results(self, result: dict, query: dict) -> pd.DataFrame:
-        df_results = pd.DataFrame()
-        #print(f"Results 3: {result}")
-        j = 0
-        r_dict = {}
+        # Create a MultiIndex with names
+        index_tuples = [tuple(query.values())]  # This will be a list of tuples
+
         if len(result) == 0:
-            df = pd.DataFrame([r_dict], columns=self.objectives, index=[tuple(query.values())])
-            return df
-        r_dict['compute_time'] = result[0][j]
-        #r_dict['energy'] = result[2][j]
-        values = [r_dict['compute_time']]
-        columns = [self.objectives[0]]
-        indices = [tuple(query.values())]
-        #print(f"R_dict: {r_dict}")
-        #print(f"Values: {values}")
-        #print(f"Objectives: {self.objectives}")
-        #print(f"Index: {indices}")
-
-        df_temp = pd.DataFrame(values,
-                           columns=columns,
-                           index=indices)
-        #print(f"Results 4: {df_temp}")
-        df_results = pd.concat([df_results, df_temp])
-        #print(f"Results 5: {df_results}")
-        return df_results
+            # Creating a MultiIndex without rows initially
+            multi_index = pd.MultiIndex.from_tuples([], names=list(query.keys()))
+
+            # Creating an empty DataFrame with a MultiIndex and specific columns
+            return pd.DataFrame(columns=self.enabled_objectives, index=multi_index)
+
+        values = [result[e][0] for e in self.enabled_objectives]
+        multi_index = pd.MultiIndex.from_tuples(index_tuples, names=list(query.keys()))
+        return pd.DataFrame([values], columns=self.enabled_objectives, index=multi_index)
 
 class Study():
     tab = None
     query_tab = None
     models = None
 
     def __init__(self, benchmark_name: str, definition: ProblemDefinition,
-                 enable_tabular: bool, dataset, objectives, server_address="localhost",
-                 port=50051, url="", enable_model: bool = True):
+                 enable_tabular: bool, dataset, enabled_objectives: list[str],
+                 server_addresses: list[str] = ["localhost"], port=50051, url="",
+                 enable_model: bool = True, enable_download: bool = True):
         self.benchmark_name = benchmark_name
-        self.grpc_urls = [f"{server_address}:{port}" if url == "" else url]
-        self.objectives = objectives
+        #self.grpc_urls = [f"{server_address}:{port}" if url == "" else url]
+        self.grpc_urls = [f"{server_address}:{port}" for server_address in server_addresses]
+        self.enabled_objectives = enabled_objectives
         self.enable_tabular = enable_tabular
         self.enable_model = enable_model
         self.dataset = dataset
         self.definition = definition
         self.parameters = definition.search_space.params
         self.port = port
 
         if self.enable_tabular or self.enable_model:
             self.software_query = SoftwareQuery(
-                benchmark_name, dataset, self.get_parameter_names(), self.objectives,
-                enable_tabular=self.enable_tabular, enable_model=self.enable_model)
+                benchmark_name, dataset, self.get_parameter_names(),
+                enabled_objectives=self.enabled_objectives,
+                enable_tabular=self.enable_tabular, enable_model=self.enable_model,
+                enable_download=enable_download)
         else:
             self.software_query = None
-        self.grpc_query = GRPCQuery(self.grpc_urls, self.parameters, self.objectives)
+        self.grpc_query = GRPCQuery(self.grpc_urls, self.parameters,
+                                    self.enabled_objectives, self.definition)
 
     def set_tabular(self, enable_tabular: bool):
         self.enable_tabular = enable_tabular
 
-    def get_objectives(self):
-        return self.objectives
+    def get_enabled_objectives(self):
+        return self.enabled_objectives
 
     def query(self, query: dict) -> dict:
-        return asyncio.run(self.query_async(query))
+        res = asyncio.run(self.query_async(query))
+        ret = {}
+        for k in self.enabled_objectives:
+            ret[k] = res[k]
+        return ret
 
     async def query_async(self, query: dict) -> list[dict]:
-        #print(f"Queries: {query}")
         return await self.query_choice(query)
 
     async def query_choice(self, query: dict) -> dict:
-        # Directly call and await the appropriate method based on the condition
         result = None
         if self.enable_tabular:
             result = await self.software_query.query_software(query.copy())
-            #print(f"Tab software result: {result}")
-        #print(f"Result: {result}")
+            if isinstance(result, pd.Series):
+                result = result.to_frame().T
         if result is None:
             result = await self.grpc_query.query_hardware(query.copy())
-            #print(f"Tab result add: {result}")
-            df: pd.DataFrame = self.software_query.tabular_dataset.query_tab
-            df = pd.concat([df, result])
-            #print(f"DF: {df}")
-            df.index.names = self.get_parameter_names()
-            #print(f"DF: {df}")
-            self.software_query.tabular_dataset.query_tab = df
-            #print(f"Added to tabular data: {result}")
 
+            self.software_query.tabular_dataset.add(result)
+        print(result, type(result))
+        if len(result.index) == 0:
+            return { "compute_time": 0.0 }
 
-        # Process and return results
-        # return [results.iloc[0].to_dict() if len(queries) == 1 else results.T.to_dict()[tuple(query.values())] for query in queries]
         return result.iloc[0].to_dict()
 
+
     def get_parameter_names(self):
         return [param.name for param in self.parameters]
 
     def get_parameter_types(self):
         return [param.param_type_enum for param in self.parameters]
 
     def get_default_config(self):
```

### Comparing `interopt-0.1.0/interopt.egg-info/SOURCES.txt` & `interopt-0.1.1/interopt.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,10 +11,11 @@
 interopt.egg-info/dependency_links.txt
 interopt.egg-info/requires.txt
 interopt.egg-info/top_level.txt
 interopt/runner/__init__.py
 interopt/runner/model.py
 interopt/runner/grpc_runner/__init__.py
 interopt/runner/grpc_runner/config_service_pb2.py
+interopt/runner/grpc_runner/config_service_pb2.pyi
 interopt/runner/grpc_runner/config_service_pb2_grpc.py
 interopt/runner/grpc_runner/main.py
 interopt/runner/grpc_runner/server.py
```

### Comparing `interopt-0.1.0/setup.py` & `interopt-0.1.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # setup.py
 from setuptools import setup, find_packages
 
 setup(
     name='interopt',
-    version='0.1.0',
+    version='0.1.1',
     author='Jacob Odgård Tørring',
     author_email='jacob.torring@ntnu.no',
     packages=find_packages(),
     license='LICENSE',
     description='An interoperability layer for black-box optimization',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     install_requires=[
+        'requests',
         'pandas',
         'catboost',
         'grpcio',
         'grpcio-tools',
         'protobuf',
         'scikit-learn',
     ],
```

