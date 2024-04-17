# Comparing `tmp/openobd-protocol-0.0.36.tar.gz` & `tmp/openobd_protocol-0.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openobd-protocol-0.0.36.tar", last modified: Wed Apr 10 14:28:04 2024, max compression
+gzip compressed data, was "openobd_protocol-0.0.37.tar", last modified: Wed Apr 17 12:31:28 2024, max compression
```

## Comparing `openobd-protocol-0.0.36.tar` & `openobd_protocol-0.0.37.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 14:28:04.054864 openobd-protocol-0.0.36/
--rw-r--r--   0 root         (0) root         (0)     1066 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2457 2024-04-10 14:28:04.054864 openobd-protocol-0.0.36/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      241 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/README.md
--rw-r--r--   0 root         (0) root         (0)     1895 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 14:28:04.054864 openobd-protocol-0.0.36/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 14:28:04.034864 openobd-protocol-0.0.36/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 14:28:04.041864 openobd-protocol-0.0.36/src/openobd_protocol/
--rw-r--r--   0 root         (0) root         (0)     1745 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/Authentication_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/Authentication_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1234 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/BasicResponse_pb2.py
--rw-r--r--   0 root         (0) root         (0)      504 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/BasicResponse_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     5065 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/BusConfiguration_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6043 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/BusConfiguration_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 14:28:04.046864 openobd-protocol-0.0.36/src/openobd_protocol/CAN/
--rw-r--r--   0 root         (0) root         (0)     2103 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/CAN/CanServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      462 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/CAN/CanServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     4415 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/CAN/CanServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2636 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/CAN/Isotp_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2500 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/CAN/Isotp_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2349 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/RemoteDiagnosticServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      405 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/RemoteDiagnosticServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     8395 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 14:28:04.048864 openobd-protocol-0.0.36/src/openobd_protocol/SessionController/
--rw-r--r--   0 root         (0) root         (0)     1940 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/SessionController/SessionServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      190 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/SessionController/SessionServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     9440 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     1712 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/Status_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1203 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/Status_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 14:28:04.051864 openobd-protocol-0.0.36/src/openobd_protocol/UserInterface/
--rw-r--r--   0 root         (0) root         (0)     1748 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      273 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2973 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3920 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/UserInterface/UserInterface_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4208 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-10 14:27:59.000000 openobd-protocol-0.0.36/src/openobd_protocol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 14:28:04.052864 openobd-protocol-0.0.36/src/openobd_protocol.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2457 2024-04-10 14:28:04.000000 openobd-protocol-0.0.36/src/openobd_protocol.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1501 2024-04-10 14:28:04.000000 openobd-protocol-0.0.36/src/openobd_protocol.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 14:28:04.000000 openobd-protocol-0.0.36/src/openobd_protocol.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2024-04-10 14:28:04.000000 openobd-protocol-0.0.36/src/openobd_protocol.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-10 14:28:04.000000 openobd-protocol-0.0.36/src/openobd_protocol.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:31:28.087921 openobd_protocol-0.0.37/
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-04-17 12:31:23.000000 openobd_protocol-0.0.37/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-17 12:31:28.087921 openobd_protocol-0.0.37/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      241 2024-04-17 12:31:23.000000 openobd_protocol-0.0.37/README.md
+-rw-r--r--   0 root         (0) root         (0)     1895 2024-04-17 12:31:23.000000 openobd_protocol-0.0.37/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 12:31:28.087921 openobd_protocol-0.0.37/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:31:28.071920 openobd_protocol-0.0.37/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:31:28.077921 openobd_protocol-0.0.37/src/openobd_protocol/
+-rw-r--r--   0 root         (0) root         (0)     1745 2024-04-17 12:31:23.000000 openobd_protocol-0.0.37/src/openobd_protocol/Authentication_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-04-17 12:31:23.000000 openobd_protocol-0.0.37/src/openobd_protocol/Authentication_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1234 2024-04-17 12:31:23.000000 openobd_protocol-0.0.37/src/openobd_protocol/BasicResponse_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      504 2024-04-17 12:31:23.000000 openobd_protocol-0.0.37/src/openobd_protocol/BasicResponse_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     5065 2024-04-17 12:31:23.000000 openobd_protocol-0.0.37/src/openobd_protocol/BusConfiguration_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6043 2024-04-17 12:31:23.000000 openobd_protocol-0.0.37/src/openobd_protocol/BusConfiguration_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:31:28.080921 openobd_protocol-0.0.37/src/openobd_protocol/CAN/
+-rw-r--r--   0 root         (0) root         (0)     2103 2024-04-17 12:31:23.000000 openobd_protocol-0.0.37/src/openobd_protocol/CAN/CanServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      462 2024-04-17 12:31:23.000000 openobd_protocol-0.0.37/src/openobd_protocol/CAN/CanServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     4415 2024-04-17 12:31:23.000000 openobd_protocol-0.0.37/src/openobd_protocol/CAN/CanServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2636 2024-04-17 12:31:23.000000 openobd_protocol-0.0.37/src/openobd_protocol/CAN/Isotp_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2500 2024-04-17 12:31:23.000000 openobd_protocol-0.0.37/src/openobd_protocol/CAN/Isotp_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2349 2024-04-17 12:31:23.000000 openobd_protocol-0.0.37/src/openobd_protocol/RemoteDiagnosticServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      405 2024-04-17 12:31:23.000000 openobd_protocol-0.0.37/src/openobd_protocol/RemoteDiagnosticServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     8395 2024-04-17 12:31:23.000000 openobd_protocol-0.0.37/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:31:28.083921 openobd_protocol-0.0.37/src/openobd_protocol/SessionController/
+-rw-r--r--   0 root         (0) root         (0)     1940 2024-04-17 12:31:23.000000 openobd_protocol-0.0.37/src/openobd_protocol/SessionController/SessionServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      190 2024-04-17 12:31:23.000000 openobd_protocol-0.0.37/src/openobd_protocol/SessionController/SessionServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     9440 2024-04-17 12:31:23.000000 openobd_protocol-0.0.37/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     1712 2024-04-17 12:31:23.000000 openobd_protocol-0.0.37/src/openobd_protocol/Status_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2024-04-17 12:31:23.000000 openobd_protocol-0.0.37/src/openobd_protocol/Status_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:31:28.086921 openobd_protocol-0.0.37/src/openobd_protocol/UserInterface/
+-rw-r--r--   0 root         (0) root         (0)     1748 2024-04-17 12:31:23.000000 openobd_protocol-0.0.37/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      273 2024-04-17 12:31:23.000000 openobd_protocol-0.0.37/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2973 2024-04-17 12:31:23.000000 openobd_protocol-0.0.37/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3920 2024-04-17 12:31:23.000000 openobd_protocol-0.0.37/src/openobd_protocol/UserInterface/UserInterface_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4208 2024-04-17 12:31:23.000000 openobd_protocol-0.0.37/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-17 12:31:23.000000 openobd_protocol-0.0.37/src/openobd_protocol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:31:28.086921 openobd_protocol-0.0.37/src/openobd_protocol.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-17 12:31:28.000000 openobd_protocol-0.0.37/src/openobd_protocol.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1501 2024-04-17 12:31:28.000000 openobd_protocol-0.0.37/src/openobd_protocol.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 12:31:28.000000 openobd_protocol-0.0.37/src/openobd_protocol.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2024-04-17 12:31:28.000000 openobd_protocol-0.0.37/src/openobd_protocol.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-17 12:31:28.000000 openobd_protocol-0.0.37/src/openobd_protocol.egg-info/top_level.txt
```

### Comparing `openobd-protocol-0.0.36/LICENSE` & `openobd_protocol-0.0.37/LICENSE`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.36/PKG-INFO` & `openobd_protocol-0.0.37/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openobd-protocol
-Version: 0.0.36
+Version: 0.0.37
 Summary: Jifeline Networks OpenOBD Protocol Buffers gRPC
 Author-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 Maintainer-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 License: Copyright (c) 2024 Jifeline Networks B.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `openobd-protocol-0.0.36/pyproject.toml` & `openobd_protocol-0.0.37/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.36/src/openobd_protocol/Authentication_pb2.py` & `openobd_protocol-0.0.37/src/openobd_protocol/Authentication_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.36/src/openobd_protocol/Authentication_pb2.pyi` & `openobd_protocol-0.0.37/src/openobd_protocol/Authentication_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.36/src/openobd_protocol/BasicResponse_pb2.py` & `openobd_protocol-0.0.37/src/openobd_protocol/BasicResponse_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.36/src/openobd_protocol/BusConfiguration_pb2.py` & `openobd_protocol-0.0.37/src/openobd_protocol/BusConfiguration_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.36/src/openobd_protocol/BusConfiguration_pb2.pyi` & `openobd_protocol-0.0.37/src/openobd_protocol/BusConfiguration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.36/src/openobd_protocol/CAN/CanServices_pb2.py` & `openobd_protocol-0.0.37/src/openobd_protocol/CAN/CanServices_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.36/src/openobd_protocol/CAN/CanServices_pb2_grpc.py` & `openobd_protocol-0.0.37/src/openobd_protocol/CAN/CanServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.36/src/openobd_protocol/CAN/Isotp_pb2.py` & `openobd_protocol-0.0.37/src/openobd_protocol/CAN/Isotp_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.36/src/openobd_protocol/CAN/Isotp_pb2.pyi` & `openobd_protocol-0.0.37/src/openobd_protocol/CAN/Isotp_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.36/src/openobd_protocol/RemoteDiagnosticServices_pb2.py` & `openobd_protocol-0.0.37/src/openobd_protocol/RemoteDiagnosticServices_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.36/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py` & `openobd_protocol-0.0.37/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.36/src/openobd_protocol/SessionController/SessionServices_pb2.py` & `openobd_protocol-0.0.37/src/openobd_protocol/SessionController/SessionServices_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.36/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py` & `openobd_protocol-0.0.37/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.36/src/openobd_protocol/Status_pb2.py` & `openobd_protocol-0.0.37/src/openobd_protocol/Status_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.36/src/openobd_protocol/Status_pb2.pyi` & `openobd_protocol-0.0.37/src/openobd_protocol/Status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.36/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py` & `openobd_protocol-0.0.37/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.36/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py` & `openobd_protocol-0.0.37/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.36/src/openobd_protocol/UserInterface/UserInterface_pb2.py` & `openobd_protocol-0.0.37/src/openobd_protocol/UserInterface/UserInterface_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.36/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi` & `openobd_protocol-0.0.37/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd-protocol-0.0.36/src/openobd_protocol.egg-info/PKG-INFO` & `openobd_protocol-0.0.37/src/openobd_protocol.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openobd-protocol
-Version: 0.0.36
+Version: 0.0.37
 Summary: Jifeline Networks OpenOBD Protocol Buffers gRPC
 Author-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 Maintainer-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 License: Copyright (c) 2024 Jifeline Networks B.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `openobd-protocol-0.0.36/src/openobd_protocol.egg-info/SOURCES.txt` & `openobd_protocol-0.0.37/src/openobd_protocol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

