# Comparing `tmp/pyrtma-2.2.2.tar.gz` & `tmp/pyrtma-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrtma-2.2.2.tar", last modified: Tue Mar 12 20:33:03 2024, max compression
+gzip compressed data, was "pyrtma-2.2.3.tar", last modified: Wed Apr 17 19:50:05 2024, max compression
```

## Comparing `pyrtma-2.2.2.tar` & `pyrtma-2.2.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:33:03.550613 pyrtma-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-12 20:32:59.000000 pyrtma-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-12 20:32:59.000000 pyrtma-2.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-03-12 20:33:03.550613 pyrtma-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-03-12 20:32:59.000000 pyrtma-2.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-03-12 20:32:59.000000 pyrtma-2.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 20:33:03.550613 pyrtma-2.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:33:03.542613 pyrtma-2.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:33:03.546613 pyrtma-2.2.2/src/pyrtma/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-12 20:32:59.000000 pyrtma-2.2.2/src/pyrtma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-12 20:32:59.000000 pyrtma-2.2.2/src/pyrtma/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28510 2024-03-12 20:32:59.000000 pyrtma-2.2.2/src/pyrtma/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-03-12 20:32:59.000000 pyrtma-2.2.2/src/pyrtma/compile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:33:03.546613 pyrtma-2.2.2/src/pyrtma/compilers/
--rw-r--r--   0 runner    (1001) docker     (127)    13544 2024-03-12 20:32:59.000000 pyrtma-2.2.2/src/pyrtma/compilers/c99.py
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-03-12 20:32:59.000000 pyrtma-2.2.2/src/pyrtma/compilers/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-03-12 20:32:59.000000 pyrtma-2.2.2/src/pyrtma/compilers/javascript.py
--rw-r--r--   0 runner    (1001) docker     (127)    11678 2024-03-12 20:32:59.000000 pyrtma-2.2.2/src/pyrtma/compilers/matlab.py
--rw-r--r--   0 runner    (1001) docker     (127)    11264 2024-03-12 20:32:59.000000 pyrtma-2.2.2/src/pyrtma/compilers/python.py
--rw-r--r--   0 runner    (1001) docker     (127)    10014 2024-03-12 20:32:59.000000 pyrtma-2.2.2/src/pyrtma/compilers/python_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-03-12 20:32:59.000000 pyrtma-2.2.2/src/pyrtma/compilers/yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-03-12 20:32:59.000000 pyrtma-2.2.2/src/pyrtma/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:33:03.546613 pyrtma-2.2.2/src/pyrtma/core_defs/
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-03-12 20:32:59.000000 pyrtma-2.2.2/src/pyrtma/core_defs/core_defs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13355 2024-03-12 20:32:59.000000 pyrtma-2.2.2/src/pyrtma/core_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-03-12 20:32:59.000000 pyrtma-2.2.2/src/pyrtma/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-03-12 20:32:59.000000 pyrtma-2.2.2/src/pyrtma/header.py
--rw-r--r--   0 runner    (1001) docker     (127)    24977 2024-03-12 20:32:59.000000 pyrtma-2.2.2/src/pyrtma/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-03-12 20:32:59.000000 pyrtma-2.2.2/src/pyrtma/message.py
--rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-03-12 20:32:59.000000 pyrtma-2.2.2/src/pyrtma/message_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-12 20:32:59.000000 pyrtma-2.2.2/src/pyrtma/message_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    47924 2024-03-12 20:32:59.000000 pyrtma-2.2.2/src/pyrtma/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 20:32:59.000000 pyrtma-2.2.2/src/pyrtma/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:33:03.550613 pyrtma-2.2.2/src/pyrtma/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-03-12 20:32:59.000000 pyrtma-2.2.2/src/pyrtma/utils/generate_test_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-03-12 20:32:59.000000 pyrtma-2.2.2/src/pyrtma/utils/print.py
--rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-03-12 20:32:59.000000 pyrtma-2.2.2/src/pyrtma/utils/quicklogger_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-03-12 20:32:59.000000 pyrtma-2.2.2/src/pyrtma/utils/random_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    32274 2024-03-12 20:32:59.000000 pyrtma-2.2.2/src/pyrtma/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)    13953 2024-03-12 20:32:59.000000 pyrtma-2.2.2/src/pyrtma/web_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:33:03.550613 pyrtma-2.2.2/src/pyrtma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-03-12 20:33:03.000000 pyrtma-2.2.2/src/pyrtma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-03-12 20:33:03.000000 pyrtma-2.2.2/src/pyrtma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 20:33:03.000000 pyrtma-2.2.2/src/pyrtma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-12 20:33:03.000000 pyrtma-2.2.2/src/pyrtma.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-12 20:33:03.000000 pyrtma-2.2.2/src/pyrtma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-12 20:33:03.000000 pyrtma-2.2.2/src/pyrtma.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:33:03.550613 pyrtma-2.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-03-12 20:32:59.000000 pyrtma-2.2.2/tests/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-03-12 20:32:59.000000 pyrtma-2.2.2/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    17821 2024-03-12 20:32:59.000000 pyrtma-2.2.2/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-03-12 20:32:59.000000 pyrtma-2.2.2/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)    22361 2024-03-12 20:32:59.000000 pyrtma-2.2.2/tests/test_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:50:05.270963 pyrtma-2.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-17 19:50:01.000000 pyrtma-2.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-17 19:50:01.000000 pyrtma-2.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-04-17 19:50:05.270963 pyrtma-2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-04-17 19:50:01.000000 pyrtma-2.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-17 19:50:01.000000 pyrtma-2.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 19:50:05.270963 pyrtma-2.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:50:05.262963 pyrtma-2.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:50:05.266963 pyrtma-2.2.3/src/pyrtma/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27808 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/compile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:50:05.266963 pyrtma-2.2.3/src/pyrtma/compilers/
+-rw-r--r--   0 runner    (1001) docker     (127)    13544 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/compilers/c99.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/compilers/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7539 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/compilers/javascript.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11678 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/compilers/matlab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11264 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/compilers/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10014 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/compilers/python_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/compilers/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:50:05.266963 pyrtma-2.2.3/src/pyrtma/core_defs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/core_defs/core_defs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13355 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/core_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24977 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11016 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/message_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/message_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47924 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:50:05.266963 pyrtma-2.2.3/src/pyrtma/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/utils/generate_test_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/utils/print.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/utils/quicklogger_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/utils/random_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32568 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14914 2024-04-17 19:50:01.000000 pyrtma-2.2.3/src/pyrtma/web_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:50:05.266963 pyrtma-2.2.3/src/pyrtma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5439 2024-04-17 19:50:05.000000 pyrtma-2.2.3/src/pyrtma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-17 19:50:05.000000 pyrtma-2.2.3/src/pyrtma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 19:50:05.000000 pyrtma-2.2.3/src/pyrtma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-17 19:50:05.000000 pyrtma-2.2.3/src/pyrtma.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-17 19:50:05.000000 pyrtma-2.2.3/src/pyrtma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 19:50:05.000000 pyrtma-2.2.3/src/pyrtma.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:50:05.266963 pyrtma-2.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-17 19:50:01.000000 pyrtma-2.2.3/tests/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-17 19:50:01.000000 pyrtma-2.2.3/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17821 2024-04-17 19:50:01.000000 pyrtma-2.2.3/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-17 19:50:01.000000 pyrtma-2.2.3/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22361 2024-04-17 19:50:01.000000 pyrtma-2.2.3/tests/test_validators.py
```

### Comparing `pyrtma-2.2.2/LICENSE` & `pyrtma-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.2/PKG-INFO` & `pyrtma-2.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrtma
-Version: 2.2.2
+Version: 2.2.3
 Summary: A Python client for RTMA/Dragonfly
 Author-email: David Weir <dmw109@pitt.edu>, Jeff Weiss <jmw182@pitt.edu>, Tyler Madonna <tjm159@pitt.edu>, Tyler Simpson <tws21@pitt.edu>
 Project-URL: Homepage, https://github.com/pitt-rnel/pyrtma
 Project-URL: Bug Tracker, https://github.com/pitt-rnel/pyrtma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrtma-2.2.2/README.md` & `pyrtma-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.2/pyproject.toml` & `pyrtma-2.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.2/src/pyrtma/__version__.py` & `pyrtma-2.2.3/src/pyrtma/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __title__ = "pyrtma"
 __description__ = "A Python compiler and client for RTMA/Dragonfly messaging system"
 __url__ = "https://github.com/pitt-rnel/pyrtma"
-__version__ = "2.2.2"
+__version__ = "2.2.3"
 __author__ = "RNEL"
 __author_email__ = ""
 __license__ = "MIT"
 __copyright__ = "University of Pittsburgh Rehab Neural Engineering Labs, 2024"
 
 
 def check_compiled_version(compiled_version: str):
```

### Comparing `pyrtma-2.2.2/src/pyrtma/client.py` & `pyrtma-2.2.3/src/pyrtma/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,26 @@
 import os
 import ctypes
 from contextlib import contextmanager
 
 from .message import Message, get_msg_cls
 from .message_data import MessageData
 from .header import MessageHeader, get_header_cls
-from .exceptions import InvalidMessageDefinition, UnknownMessageType
+from .exceptions import (
+    InvalidMessageDefinition,
+    UnknownMessageType,
+    ClientError,
+    SocketOptionError,
+    MessageManagerNotFound,
+    NotConnectedError,
+    ConnectionLost,
+    AcknowledgementTimeout,
+    InvalidDestinationModule,
+    InvalidDestinationHost,
+)
 from . import core_defs as cd
 
 from functools import wraps
 from typing import (
     Optional,
     Tuple,
     Type,
@@ -40,62 +51,14 @@
     "InvalidDestinationModule",
     "InvalidDestinationHost",
     "Client",
     "client_context",
 ]
 
 
-class ClientError(Exception):
-    """Base exception for all Client Errors."""
-
-    pass
-
-
-class MessageManagerNotFound(ClientError):
-    """Raised when unable to connect to message manager."""
-
-    pass
-
-
-class SocketOptionError(ClientError):
-    """Raised when unable to set socket options."""
-
-    pass
-
-
-class NotConnectedError(ClientError):
-    """Raised when the client tries to read/write while not connected."""
-
-    pass
-
-
-class ConnectionLost(ClientError):
-    """Raised when there is a connection error with the server."""
-
-    pass
-
-
-class AcknowledgementTimeout(ClientError):
-    """Raised when client does not receive ack from message manager."""
-
-    pass
-
-
-class InvalidDestinationModule(ClientError):
-    """Raised when client tries to send to an invalid module."""
-
-    pass
-
-
-class InvalidDestinationHost(ClientError):
-    """Raised when client tries to send to an invalid host."""
-
-    pass
-
-
 F = TypeVar("F", bound=Callable[..., Any])
 
 
 def requires_connection(func: F) -> F:
     """Decorator wrapper for Client methods that require a connection"""
 
     @wraps(func)
```

### Comparing `pyrtma-2.2.2/src/pyrtma/compile.py` & `pyrtma-2.2.3/src/pyrtma/compile.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.2/src/pyrtma/compilers/c99.py` & `pyrtma-2.2.3/src/pyrtma/compilers/c99.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.2/src/pyrtma/compilers/info.py` & `pyrtma-2.2.3/src/pyrtma/compilers/info.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.2/src/pyrtma/compilers/javascript.py` & `pyrtma-2.2.3/src/pyrtma/compilers/javascript.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.2/src/pyrtma/compilers/matlab.py` & `pyrtma-2.2.3/src/pyrtma/compilers/matlab.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.2/src/pyrtma/compilers/python.py` & `pyrtma-2.2.3/src/pyrtma/compilers/python.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.2/src/pyrtma/compilers/python_v1.py` & `pyrtma-2.2.3/src/pyrtma/compilers/python_v1.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.2/src/pyrtma/compilers/yaml.py` & `pyrtma-2.2.3/src/pyrtma/compilers/yaml.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.2/src/pyrtma/constants.py` & `pyrtma-2.2.3/src/pyrtma/constants.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.2/src/pyrtma/core_defs/core_defs.yaml` & `pyrtma-2.2.3/src/pyrtma/core_defs/core_defs.yaml`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.2/src/pyrtma/core_defs.py` & `pyrtma-2.2.3/src/pyrtma/core_defs.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.2/src/pyrtma/header.py` & `pyrtma-2.2.3/src/pyrtma/header.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.2/src/pyrtma/manager.py` & `pyrtma-2.2.3/src/pyrtma/manager.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.2/src/pyrtma/message.py` & `pyrtma-2.2.3/src/pyrtma/message.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.2/src/pyrtma/message_base.py` & `pyrtma-2.2.3/src/pyrtma/message_base.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.2/src/pyrtma/parser.py` & `pyrtma-2.2.3/src/pyrtma/parser.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.2/src/pyrtma/utils/generate_test_defs.py` & `pyrtma-2.2.3/src/pyrtma/utils/generate_test_defs.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.2/src/pyrtma/utils/print.py` & `pyrtma-2.2.3/src/pyrtma/utils/print.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.2/src/pyrtma/utils/quicklogger_reader.py` & `pyrtma-2.2.3/src/pyrtma/utils/quicklogger_reader.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.2/src/pyrtma/utils/random_fields.py` & `pyrtma-2.2.3/src/pyrtma/utils/random_fields.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.2/src/pyrtma/validators.py` & `pyrtma-2.2.3/src/pyrtma/validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,22 +48,33 @@
     "disable_message_validation",
 ]
 
 _VALIDATION_ENABLED: ContextVar[bool] = ContextVar("_VALIDATION_ENABLED", default=True)
 
 
 @contextmanager
-def disable_message_validation():
+def disable_message_validation(ignore=False):
     """Context manager function to temporarily disable message field validation
     Use with `with` keyword:
     `with disable_message_validation():`
+
+    Optionally pass in ignore=True to do nothing, e.g. for debugging:
+
+    ```
+    DEBUG = True
+    with disable_message_validation(ignore=DEBUG):
+        ... # disable validation unless DEBUG is True
+    ```
     """
-    token = _VALIDATION_ENABLED.set(False)
-    yield
-    _VALIDATION_ENABLED.reset(token)
+    if not ignore:
+        token = _VALIDATION_ENABLED.set(False)
+        yield
+        _VALIDATION_ENABLED.reset(token)
+    else:
+        yield  # dummy context
 
 
 _P = TypeVar("_P")  # Parent
 _V = TypeVar("_V")  # Value
 
 
 class FieldValidator(Generic[_P, _V], metaclass=ABCMeta):
```

### Comparing `pyrtma-2.2.2/src/pyrtma/web_manager.py` & `pyrtma-2.2.3/src/pyrtma/web_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 import importlib
 import pathlib
 import sys
 import json
 import time
 from rich.logging import RichHandler
 
-from pyrtma import Client, Message, MessageHeader, get_msg_cls
+from pyrtma import Client, Message, MessageHeader, get_msg_cls, ClientError
 from pyrtma.exceptions import RTMAMessageError
 import pyrtma.core_defs as cd
 
 from socket import error as SocketError
+import socket
 from socketserver import TCPServer
 from websocket_server import (  # type: ignore
     WebsocketServer,
     WebSocketHandler,
     logger,
     OPCODE,
     MASKED,
@@ -56,14 +57,22 @@
         """
         # Initialize RTMA Proxy connection
         self.mm_ip = server.mm_ip
         self.proxy = Client()
 
         WebSocketHandler.__init__(self, socket, addr, server)
 
+    @property
+    def ws_ready_to_send(self):
+        if self.keep_alive:
+            _, wd, _ = select.select([], [self.wfile], [], 0)
+            return self.wfile in wd
+        else:
+            return False
+
     def handle(self):
         """Handle RTMA proxy connection"""
         if not self.handshake_done:
             self.handshake()
 
         if not self.valid_client:
             logger.error("Websocket handshake failed.")
@@ -89,28 +98,29 @@
             if self.proxy.sock in rd and self.proxy.connected:
                 try:
                     msg = self.proxy.read_message(timeout=None, ack=True)
                 except RTMAMessageError as e:
                     error_json = json.dumps(
                         {"rtma_msg_error": str(e)}, separators=(",", ":")
                     )
-                    self.send_message(error_json)
+                    if self.ws_ready_to_send:
+                        self.send_message(error_json)
                     logger.error(e, stack_info=False)
                     continue
 
-                if msg is not None:
+                if msg is not None and self.keep_alive:
                     # Pass message thru websocket as json
-                    _, wd, _ = select.select([], [self.wfile], [], 0)
-                    if self.wfile in wd:
+                    if self.ws_ready_to_send:
                         logger.debug(
                             f"Forwarding message type {get_msg_cls(msg.header.msg_type).type_name} to ws"
                         )
                         self.send_message(msg.to_json(minify=True))
                     else:
-                        self.send_failed_message(msg.header, time.perf_counter())
+                        if self.proxy.connected:
+                            self.send_failed_message(msg.header, time.perf_counter())
                         logger.warning(
                             f"Failed to foward message type {get_msg_cls(msg.header.msg_type).type_name} to ws. Mod ID = {self.proxy.module_id}"
                         )
 
     def pong_received(self, msg: str):
         """Log that pong was received
 
@@ -126,16 +136,15 @@
         # self.proxy._host_id = msg.header.src_host_id
         msg.data = cast(cd.MDF_CONNECT, msg.data)
         ack_msg = self.proxy._connect_helper(
             bool(msg.data.logger_status), bool(msg.data.daemon_status)
         )
         # forward ack
         # Pass message thru websocket as json
-        _, wd, _ = select.select([], [self.wfile], [], 0)
-        if self.wfile in wd:
+        if self.ws_ready_to_send:
             logger.debug(
                 f"Forwarding ACK from connect to ws. Mod ID = {self.proxy.module_id}"
             )
             self.send_message(ack_msg.to_json(minify=True))
         else:
             self.send_failed_message(ack_msg.header, time.perf_counter())
             logger.warning(
@@ -146,15 +155,15 @@
         """Process incoming json message
 
         Called when a client receives a message over websocket
 
         Args:
             message (str): JSON message string
         """
-        if message == "PING":
+        if message == "PING" and self.ws_ready_to_send:
             self.send_message("PONG")
             return
 
         try:
             msg = Message.from_json(message)
 
             if msg.header.msg_type == cd.MT_DISCONNECT:
@@ -190,17 +199,20 @@
                     f"Proxy CONNECTED, assigned module ID {self.proxy.module_id}"
                 )
             else:
                 self.proxy.forward_message(msg.header, msg.data or None)
                 logger.debug(
                     f"Forwarded message type {get_msg_cls(msg.header.msg_type).type_name} from ws"
                 )
-        except RTMAMessageError as e:
-            error_json = json.dumps({"rtma_msg_error": str(e)}, separators=(",", ":"))
-            self.send_message(error_json)
+        except (RTMAMessageError, ClientError) as e:
+            if self.ws_ready_to_send:
+                error_json = json.dumps(
+                    {"rtma_msg_error": str(e)}, separators=(",", ":")
+                )
+                self.send_message(error_json)
             logger.error(e, stack_info=False)
             return
 
     def read_ws_message(self) -> Optional[str]:
         """Read websocket message
 
         Returns:
@@ -272,16 +284,16 @@
         for fname, ftype in data.msg_header._fields_:
             setattr(data.msg_header, fname, getattr(header, fname))
 
         if (
             data.msg_header.msg_type == cd.MT_FAILED_MESSAGE
         ):  # avoid unlikely infinite recursion
             return
-
-        self.proxy.send_message(data)
+        if self.proxy.connected:
+            self.proxy.send_message(data)
 
     def finish(self):
         """Close RTMA connection"""
         # Disconnect on behalf of the web client if still connected here
         if self.proxy.connected:
             self.proxy.disconnect()
             logger.debug("Disconnected proxy from MM.")
@@ -313,14 +325,25 @@
         """
 
         logger.setLevel(loglevel)
         TCPServer.__init__(self, (host, port), RTMAWebSocketHandler)
         self.host = host
         self.port = self.socket.getsockname()[1]
 
+        if self.host not in ("", "0.0.0.0"):
+            logger.info(f"WebMessageManager listening on {self.host}:{self.port}")
+        else:
+            hosts = socket.gethostbyname_ex(socket.gethostname())[-1]
+            if "127.0.0.1" not in hosts:
+                hosts.append("127.0.0.1")
+            logger.info(
+                f"WebMessageManager listening on all interfaces, port {self.port}"
+            )
+            logger.info(f"IP addresses: {hosts}")
+
         self.key = key
         self.cert = cert
 
         self.clients: List[dict] = []
         self.id_counter = 0
         self.thread = None
 
@@ -336,26 +359,32 @@
     """Websocket client connect
 
         Called for every client connecting (after handshake)
     Args:
         client (Dict[str, Any]): Client dictionary
         server: WebMessageManager Server object
     """
-    logger.info(f"Client connected -> id: {client['id']}")
+    try:
+        logger.info(f"Client connected -> id: {client['id']}")
+    except:
+        pass
 
 
 def ws_client_disconnect(client: Dict[str, Any], server: WebMessageManager):
     """Websocket client disconnect
 
         Called for every client disconnecting
     Args:
         client (Dict[str, Any]): Client dictionary
         server: WebMessageManager Server object
     """
-    logger.info(f"Client disconnected -> id: {client['id']}\n")
+    try:
+        logger.info(f"Client disconnected -> id: {client['id']}")
+    except:
+        pass
 
 
 def main():
     """Main function for starting web_manager"""
 
     parser = argparse.ArgumentParser(description="Websocket Message Manager")
 
@@ -365,14 +394,15 @@
         default="127.0.0.1:7111",
         dest="mm_ip",
         type=str,
         help="IP address of Message Manager. Defaults to 127.0.0.1:7111.",
     )
 
     parser.add_argument(
+        "-a",
         "--host",
         default="",
         dest="host",
         type=str,
         help='Host IP address, defaults to "" (any local IP).',
     )
```

### Comparing `pyrtma-2.2.2/src/pyrtma.egg-info/PKG-INFO` & `pyrtma-2.2.3/src/pyrtma.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrtma
-Version: 2.2.2
+Version: 2.2.3
 Summary: A Python client for RTMA/Dragonfly
 Author-email: David Weir <dmw109@pitt.edu>, Jeff Weiss <jmw182@pitt.edu>, Tyler Madonna <tjm159@pitt.edu>, Tyler Simpson <tws21@pitt.edu>
 Project-URL: Homepage, https://github.com/pitt-rnel/pyrtma
 Project-URL: Bug Tracker, https://github.com/pitt-rnel/pyrtma/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyrtma-2.2.2/src/pyrtma.egg-info/SOURCES.txt` & `pyrtma-2.2.3/src/pyrtma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.2/tests/test_encoding.py` & `pyrtma-2.2.3/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.2/tests/test_json.py` & `pyrtma-2.2.3/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.2/tests/test_parser.py` & `pyrtma-2.2.3/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.2/tests/test_sync.py` & `pyrtma-2.2.3/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `pyrtma-2.2.2/tests/test_validators.py` & `pyrtma-2.2.3/tests/test_validators.py`

 * *Files identical despite different names*

