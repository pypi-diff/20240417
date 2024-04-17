# Comparing `tmp/dig_ass_ocr_protos-0.0.3.tar.gz` & `tmp/dig_ass_ocr_protos-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dig_ass_ocr_protos-0.0.3.tar", last modified: Fri Apr 12 21:08:56 2024, max compression
+gzip compressed data, was "dig_ass_ocr_protos-0.0.4.tar", last modified: Wed Apr 17 15:45:58 2024, max compression
```

## Comparing `dig_ass_ocr_protos-0.0.3.tar` & `dig_ass_ocr_protos-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 21:08:56.738471 dig_ass_ocr_protos-0.0.3/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_ocr_protos-0.0.3/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      333 2024-04-12 21:08:56.738471 dig_ass_ocr_protos-0.0.3/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:44.000000 dig_ass_ocr_protos-0.0.3/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 21:08:56.738471 dig_ass_ocr_protos-0.0.3/dig_ass_ocr_protos/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1689 2024-04-12 21:08:55.000000 dig_ass_ocr_protos-0.0.3/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      692 2024-04-12 21:08:55.000000 dig_ass_ocr_protos-0.0.3/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.pyi
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2917 2024-04-12 21:08:55.000000 dig_ass_ocr_protos-0.0.3/dig_ass_ocr_protos/DigitalAssistantOCR_pb2_grpc.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-12 21:07:05.000000 dig_ass_ocr_protos-0.0.3/dig_ass_ocr_protos/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      389 2024-04-12 20:28:21.000000 dig_ass_ocr_protos-0.0.3/dig_ass_ocr_protos/abstract_client.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      648 2024-04-12 21:06:32.000000 dig_ass_ocr_protos-0.0.3/dig_ass_ocr_protos/client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 21:08:56.738471 dig_ass_ocr_protos-0.0.3/dig_ass_ocr_protos.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      333 2024-04-12 21:08:56.000000 dig_ass_ocr_protos-0.0.3/dig_ass_ocr_protos.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      498 2024-04-12 21:08:56.000000 dig_ass_ocr_protos-0.0.3/dig_ass_ocr_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-12 21:08:56.000000 dig_ass_ocr_protos-0.0.3/dig_ass_ocr_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-12 21:08:56.000000 dig_ass_ocr_protos-0.0.3/dig_ass_ocr_protos.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       19 2024-04-12 21:08:56.000000 dig_ass_ocr_protos-0.0.3/dig_ass_ocr_protos.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_ocr_protos-0.0.3/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-12 21:08:56.738471 dig_ass_ocr_protos-0.0.3/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      800 2024-04-11 10:26:57.000000 dig_ass_ocr_protos-0.0.3/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-17 15:45:58.129968 dig_ass_ocr_protos-0.0.4/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_ocr_protos-0.0.4/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      333 2024-04-17 15:45:58.129968 dig_ass_ocr_protos-0.0.4/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:44.000000 dig_ass_ocr_protos-0.0.4/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-17 15:45:58.129968 dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1686 2024-04-17 15:45:56.000000 dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      692 2024-04-17 15:45:56.000000 dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.pyi
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2914 2024-04-17 15:45:56.000000 dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos/DigitalAssistantOCR_pb2_grpc.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-17 15:45:14.000000 dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      389 2024-04-12 20:28:21.000000 dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos/abstract_client.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      648 2024-04-12 21:06:32.000000 dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos/client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-17 15:45:58.129968 dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      333 2024-04-17 15:45:58.000000 dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      498 2024-04-17 15:45:58.000000 dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-17 15:45:58.000000 dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-17 15:45:58.000000 dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       19 2024-04-17 15:45:58.000000 dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_ocr_protos-0.0.4/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-17 15:45:58.129968 dig_ass_ocr_protos-0.0.4/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      800 2024-04-11 10:26:57.000000 dig_ass_ocr_protos-0.0.4/setup.py
```

### Comparing `dig_ass_ocr_protos-0.0.3/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.py` & `dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,dig_ass_ocr_protos/DigitalAssistantOCR.proto\x12\x0f\x64ig.ass.text.v1\"+\n\x1b\x44igitalAssistantOCRResponse\x12\x0c\n\x04Text\x18\x01 \x01(\t\"8\n\x1a\x44igitalAssistantOCRRequest\x12\r\n\x05Image\x18\x01 \x01(\x0c\x12\x0b\n\x03PDF\x18\x02 \x01(\x0c\x32\x83\x01\n\x13\x44igitalAssistantOCR\x12l\n\x0fGetTextResponse\x12+.dig.ass.text.v1.DigitalAssistantOCRRequest\x1a,.dig.ass.text.v1.DigitalAssistantOCRResponseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,dig_ass_ocr_protos/DigitalAssistantOCR.proto\x12\x0e\x64ig.ass.ocr.v1\"+\n\x1b\x44igitalAssistantOCRResponse\x12\x0c\n\x04Text\x18\x01 \x01(\t\"8\n\x1a\x44igitalAssistantOCRRequest\x12\r\n\x05Image\x18\x01 \x01(\x0c\x12\x0b\n\x03PDF\x18\x02 \x01(\x0c\x32\x81\x01\n\x13\x44igitalAssistantOCR\x12j\n\x0fGetTextResponse\x12*.dig.ass.ocr.v1.DigitalAssistantOCRRequest\x1a+.dig.ass.ocr.v1.DigitalAssistantOCRResponseb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'dig_ass_ocr_protos.DigitalAssistantOCR_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
-  _globals['_DIGITALASSISTANTOCRRESPONSE']._serialized_start=65
-  _globals['_DIGITALASSISTANTOCRRESPONSE']._serialized_end=108
-  _globals['_DIGITALASSISTANTOCRREQUEST']._serialized_start=110
-  _globals['_DIGITALASSISTANTOCRREQUEST']._serialized_end=166
-  _globals['_DIGITALASSISTANTOCR']._serialized_start=169
-  _globals['_DIGITALASSISTANTOCR']._serialized_end=300
+  _globals['_DIGITALASSISTANTOCRRESPONSE']._serialized_start=64
+  _globals['_DIGITALASSISTANTOCRRESPONSE']._serialized_end=107
+  _globals['_DIGITALASSISTANTOCRREQUEST']._serialized_start=109
+  _globals['_DIGITALASSISTANTOCRREQUEST']._serialized_end=165
+  _globals['_DIGITALASSISTANTOCR']._serialized_start=168
+  _globals['_DIGITALASSISTANTOCR']._serialized_end=297
 # @@protoc_insertion_point(module_scope)
```

### Comparing `dig_ass_ocr_protos-0.0.3/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.pyi` & `dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dig_ass_ocr_protos-0.0.3/dig_ass_ocr_protos/DigitalAssistantOCR_pb2_grpc.py` & `dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos/DigitalAssistantOCR_pb2_grpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.GetTextResponse = channel.unary_unary(
-                '/dig.ass.text.v1.DigitalAssistantOCR/GetTextResponse',
+                '/dig.ass.ocr.v1.DigitalAssistantOCR/GetTextResponse',
                 request_serializer=dig__ass__ocr__protos_dot_DigitalAssistantOCR__pb2.DigitalAssistantOCRRequest.SerializeToString,
                 response_deserializer=dig__ass__ocr__protos_dot_DigitalAssistantOCR__pb2.DigitalAssistantOCRResponse.FromString,
                 )
 
 
 class DigitalAssistantOCRServicer(object):
     """Missing associated documentation comment in .proto file."""
@@ -36,15 +36,15 @@
             'GetTextResponse': grpc.unary_unary_rpc_method_handler(
                     servicer.GetTextResponse,
                     request_deserializer=dig__ass__ocr__protos_dot_DigitalAssistantOCR__pb2.DigitalAssistantOCRRequest.FromString,
                     response_serializer=dig__ass__ocr__protos_dot_DigitalAssistantOCR__pb2.DigitalAssistantOCRResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'dig.ass.text.v1.DigitalAssistantOCR', rpc_method_handlers)
+            'dig.ass.ocr.v1.DigitalAssistantOCR', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class DigitalAssistantOCR(object):
     """Missing associated documentation comment in .proto file."""
 
@@ -55,12 +55,12 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/dig.ass.text.v1.DigitalAssistantOCR/GetTextResponse',
+        return grpc.experimental.unary_unary(request, target, '/dig.ass.ocr.v1.DigitalAssistantOCR/GetTextResponse',
             dig__ass__ocr__protos_dot_DigitalAssistantOCR__pb2.DigitalAssistantOCRRequest.SerializeToString,
             dig__ass__ocr__protos_dot_DigitalAssistantOCR__pb2.DigitalAssistantOCRResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `dig_ass_ocr_protos-0.0.3/dig_ass_ocr_protos/client.py` & `dig_ass_ocr_protos-0.0.4/dig_ass_ocr_protos/client.py`

 * *Files identical despite different names*

### Comparing `dig_ass_ocr_protos-0.0.3/setup.py` & `dig_ass_ocr_protos-0.0.4/setup.py`

 * *Files identical despite different names*

