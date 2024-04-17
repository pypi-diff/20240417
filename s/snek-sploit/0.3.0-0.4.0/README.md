# Comparing `tmp/snek_sploit-0.3.0.tar.gz` & `tmp/snek_sploit-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snek_sploit-0.3.0.tar", max compression
+gzip compressed data, was "snek_sploit-0.4.0.tar", max compression
```

## Comparing `snek_sploit-0.3.0.tar` & `snek_sploit-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1069 2024-04-12 09:29:23.618328 snek_sploit-0.3.0/LICENSE
--rw-r--r--   0        0        0     1420 2024-04-12 09:29:23.618328 snek_sploit-0.3.0/README.md
--rw-r--r--   0        0        0      603 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1178 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/lib/__init__.py
--rw-r--r--   0        0        0     4600 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/lib/context.py
--rw-r--r--   0        0        0     3010 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/lib/metasploit.py
--rw-r--r--   0        0        0        0 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/lib/rpc/__init__.py
--rw-r--r--   0        0        0     3085 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/lib/rpc/auth.py
--rw-r--r--   0        0        0     9243 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/lib/rpc/consoles.py
--rw-r--r--   0        0        0     7887 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/lib/rpc/core.py
--rw-r--r--   0        0        0    12329 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/lib/rpc/db.py
--rw-r--r--   0        0        0      727 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/lib/rpc/health.py
--rw-r--r--   0        0        0     2641 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/lib/rpc/jobs.py
--rw-r--r--   0        0        0    19857 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/lib/rpc/modules.py
--rw-r--r--   0        0        0     1628 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/lib/rpc/plugins.py
--rw-r--r--   0        0        0    23772 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/lib/rpc/sessions.py
--rw-r--r--   0        0        0        0 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/util/__init__.py
--rw-r--r--   0        0        0     1887 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/util/constants.py
--rw-r--r--   0        0        0      446 2024-04-12 09:29:23.622328 snek_sploit-0.3.0/snek_sploit/util/enums.py
--rw-r--r--   0        0        0     2320 1970-01-01 00:00:00.000000 snek_sploit-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-17 11:49:05.731010 snek_sploit-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1420 2024-04-17 11:49:05.731010 snek_sploit-0.4.0/README.md
+-rw-r--r--   0        0        0      648 2024-04-17 11:49:05.731010 snek_sploit-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1331 2024-04-17 11:49:05.731010 snek_sploit-0.4.0/snek_sploit/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:49:05.731010 snek_sploit-0.4.0/snek_sploit/lib/__init__.py
+-rw-r--r--   0        0        0     4595 2024-04-17 11:49:05.731010 snek_sploit-0.4.0/snek_sploit/lib/context.py
+-rw-r--r--   0        0        0     3004 2024-04-17 11:49:05.731010 snek_sploit-0.4.0/snek_sploit/lib/metasploit.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:49:05.731010 snek_sploit-0.4.0/snek_sploit/lib/rpc/__init__.py
+-rw-r--r--   0        0        0     3086 2024-04-17 11:49:05.731010 snek_sploit-0.4.0/snek_sploit/lib/rpc/auth.py
+-rw-r--r--   0        0        0     9284 2024-04-17 11:49:05.731010 snek_sploit-0.4.0/snek_sploit/lib/rpc/consoles.py
+-rw-r--r--   0        0        0     7892 2024-04-17 11:49:05.731010 snek_sploit-0.4.0/snek_sploit/lib/rpc/core.py
+-rw-r--r--   0        0        0    12331 2024-04-17 11:49:05.731010 snek_sploit-0.4.0/snek_sploit/lib/rpc/db.py
+-rw-r--r--   0        0        0      728 2024-04-17 11:49:05.731010 snek_sploit-0.4.0/snek_sploit/lib/rpc/health.py
+-rw-r--r--   0        0        0     2676 2024-04-17 11:49:05.731010 snek_sploit-0.4.0/snek_sploit/lib/rpc/jobs.py
+-rw-r--r--   0        0        0    19865 2024-04-17 11:49:05.731010 snek_sploit-0.4.0/snek_sploit/lib/rpc/modules.py
+-rw-r--r--   0        0        0     1629 2024-04-17 11:49:05.735010 snek_sploit-0.4.0/snek_sploit/lib/rpc/plugins.py
+-rw-r--r--   0        0        0    24221 2024-04-17 11:49:05.735010 snek_sploit-0.4.0/snek_sploit/lib/rpc/sessions.py
+-rw-r--r--   0        0        0        0 2024-04-17 11:49:05.735010 snek_sploit-0.4.0/snek_sploit/util/__init__.py
+-rw-r--r--   0        0        0     1887 2024-04-17 11:49:05.735010 snek_sploit-0.4.0/snek_sploit/util/constants.py
+-rw-r--r--   0        0        0      448 2024-04-17 11:49:05.735010 snek_sploit-0.4.0/snek_sploit/util/enums.py
+-rw-r--r--   0        0        0      276 2024-04-17 11:49:05.735010 snek_sploit-0.4.0/snek_sploit/util/exceptions.py
+-rw-r--r--   0        0        0     2308 1970-01-01 00:00:00.000000 snek_sploit-0.4.0/PKG-INFO
```

### Comparing `snek_sploit-0.3.0/LICENSE` & `snek_sploit-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.3.0/README.md` & `snek_sploit-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.3.0/snek_sploit/__init__.py` & `snek_sploit-0.4.0/snek_sploit/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,24 +12,39 @@
     "ModuleShortInfo",
     "ModuleExecutionInfo",
     "ModuleRunningStatistics",
     "SessionInformation",
     "MeterpreterSessionTransportOptions",
     "SessionShell",
     "SessionMeterpreter",
-    "SessionRing"
+    "SessionRing",
+    "Error",
+    "InputError",
+    "RPCError",
 ]
 
 from snek_sploit.lib.metasploit import MetasploitClient
+
 # from snek_sploit.lib.rpc.auth import
 from snek_sploit.lib.rpc.consoles import ConsoleInfo, ConsoleData, ConsoleOptions
 from snek_sploit.lib.rpc.core import ModuleStatistics, VersionInformation, FrameworkThread
+
 # from snek_sploit.lib.rpc.db import
 # from snek_sploit.lib.rpc.health import
 from snek_sploit.lib.rpc.jobs import JobInformation
 from snek_sploit.lib.rpc.modules import (
-    ModuleType, EncodingOptions, ModuleShortInfo, ModuleExecutionInfo, ModuleRunningStatistics
+    ModuleType,
+    EncodingOptions,
+    ModuleShortInfo,
+    ModuleExecutionInfo,
+    ModuleRunningStatistics,
 )
+
 # from snek_sploit.lib.rpc.plugins import
 from snek_sploit.lib.rpc.sessions import (
-    SessionInformation, MeterpreterSessionTransportOptions, SessionShell, SessionMeterpreter, SessionRing
+    SessionInformation,
+    MeterpreterSessionTransportOptions,
+    SessionShell,
+    SessionMeterpreter,
+    SessionRing,
 )
+from snek_sploit.util.exceptions import Error, InputError, RPCError
```

### Comparing `snek_sploit-0.3.0/snek_sploit/lib/context.py` & `snek_sploit-0.4.0/snek_sploit/lib/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 import requests
 import msgpack
 from abc import ABC
 from typing import Union, List, Dict
 
-from snek_sploit.util import constants
+from snek_sploit.util import constants, exceptions
 
 
 ResponseDict = Dict[Union[int, str, bytes], Union[int, str, bytes, list, dict, bool]]
 ResponseList = List[Union[str, bytes, dict]]
 RPCResponse = Union[ResponseDict, str, ResponseList]
 
 
 class Context:
-    def __init__(self, username: str, password: str, host: str = "127.0.0.1", port: int = 55553, uri: str = "/api/",
-                 ssl: bool = True, certificate: str = "", token: str = "", timeout: Union[float, tuple] = None,
-                 verbose: bool = False):
+    def __init__(
+        self,
+        username: str,
+        password: str,
+        host: str = "127.0.0.1",
+        port: int = 55553,
+        uri: str = "/api/",
+        ssl: bool = True,
+        certificate: str = "",
+        token: str = "",
+        timeout: Union[float, tuple] = None,
+        verbose: bool = False,
+    ):
         """
         Context holds information used for authentication and communication with MSF RPC.
         :param username: Username used for authentication
         :param password: Password used for authentication
         :param host: MSF RPC Host
         :param port: MSF RPC Port
         :param uri: API uri
@@ -49,24 +59,25 @@
         arguments = [self.token] if use_token else []
 
         if call_arguments is not None:
             arguments += call_arguments
 
         return arguments
 
-    def call(self, endpoint: str, arguments: list = None, use_token: bool = True,
-             timeout: Union[float, tuple] = None) -> RPCResponse:
+    def call(
+        self, endpoint: str, arguments: list = None, use_token: bool = True, timeout: Union[float, tuple] = None
+    ) -> RPCResponse:
         """
         Create a call to an endpoint.
         :param endpoint: Endpoint name
         :param arguments: Arguments that will be processed and passed to the endpoint
         :param use_token: Whether to use the context token or not
         :param timeout: Timeout for the call
         :return: Unprocessed endpoint response
-        :raise Exception: In case the response contains errors, raise an Exception
+        :raise RPCError: In case the response contains errors
         :full error example:
             {'error': True, 'error_class': 'Msf::RPC::Exception', 'error_string': 'Msf::RPC::Exception',
              'error_backtrace': ["lib/msf/core/rpc/v10/rpc_base.rb:26:in `error'", ...],
              'error_message': b'Results not found for module instance asd', 'error_code': 404}
         """
         if timeout is None:
             timeout = self.timeout
@@ -74,17 +85,16 @@
         data = msgpack.dumps([endpoint, *self._create_arguments(arguments, use_token)])
         request = requests.post(self._url, data, headers=self._headers, verify=self._certificate, timeout=timeout)
         response = msgpack.loads(request.content, strict_map_key=False)
 
         if self.verbose:
             print(response)
 
-        # TODO: add custom error classes and raise different errors
         if isinstance(response, dict) and response.get(constants.ERROR) is not None:
-            raise Exception(response)
+            raise exceptions.RPCError(response)
 
         return response
 
 
 class ContextBase(ABC):
     def __init__(self, context: Context):
         self._context = context
```

### Comparing `snek_sploit-0.3.0/snek_sploit/lib/metasploit.py` & `snek_sploit-0.4.0/snek_sploit/lib/metasploit.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,17 +10,29 @@
 from snek_sploit.lib.rpc.jobs import Jobs
 from snek_sploit.lib.rpc.modules import Modules
 from snek_sploit.lib.rpc.plugins import Plugins
 from snek_sploit.lib.rpc.sessions import Sessions
 
 
 class MetasploitClient:
-    def __init__(self, username: str, password: str, host: str = "127.0.0.1", port: int = 55553, uri: str = "/api/",
-                 ssl: bool = True, certificate: str = "", log_in: bool = True, token: str = "",
-                 disable_https_warnings: bool = False, timeout: Union[float, tuple] = None, verbose: bool = False):
+    def __init__(
+        self,
+        username: str,
+        password: str,
+        host: str = "127.0.0.1",
+        port: int = 55553,
+        uri: str = "/api/",
+        ssl: bool = True,
+        certificate: str = "",
+        log_in: bool = True,
+        token: str = "",
+        disable_https_warnings: bool = False,
+        timeout: Union[float, tuple] = None,
+        verbose: bool = False,
+    ):
         """
         Client used for communication with MSF RPC.
         :param username: Username used for authentication
         :param password: Password used for authentication
         :param host: MSF RPC Host
         :param port: MSF RPC Port
         :param uri: API uri
@@ -51,17 +63,15 @@
             self.login()
 
     def login(self) -> None:
         """
         Login.
         :return: None
         """
-        token = self.auth.login()
-        self._context.token = token
-        self.auth.rpc.token_add(token)
+        self.auth.login()
 
     def logout(self) -> None:
         """
         Logout.
         :return: None
         """
         self.auth.rpc.logout(self._context.token)
```

### Comparing `snek_sploit-0.3.0/snek_sploit/lib/rpc/auth.py` & `snek_sploit-0.4.0/snek_sploit/lib/rpc/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from snek_sploit.util import constants
 
 
 class RPCAuth(ContextBase):
     """
     https://docs.metasploit.com/api/Msf/RPC/RPC_Auth.html
     """
+
     LOGIN = "auth.login"
     LOGOUT = "auth.logout"
     TOKEN_ADD = "auth.token_add"
     TOKEN_REMOVE = "auth.token_remove"
     TOKEN_LIST = "auth.token_list"
     TOKEN_GENERATE = "auth.token_generate"
```

### Comparing `snek_sploit-0.3.0/snek_sploit/lib/rpc/consoles.py` & `snek_sploit-0.4.0/snek_sploit/lib/rpc/consoles.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 from dataclasses import dataclass, asdict
 from typing import List
 import time
 
 from snek_sploit.lib.context import ContextBase, Context
-from snek_sploit.util import constants
+from snek_sploit.util import constants, exceptions
 
 
 @dataclass
 class ConsoleInfo:
     """
     Information about the console.
     """
+
     id: int
     prompt: str
     busy: bool
 
 
 @dataclass
 class ConsoleData:
     """
     Information about the console, including returned data.
     """
+
     prompt: str
     busy: bool
     data: str
 
 
 @dataclass
 class ConsoleOptions:
     """
     Options used to initialize the console.
     Only the relevant options are mentioned here, since some are always modified by the MSF.
     Sources:
     https://github.com/rapid7/metasploit-framework/blob/master/lib/msf/ui/web/web_console.rb#L46C10-L46C10
     https://github.com/rapid7/metasploit-framework/blob/master/lib/msf/ui/console/driver.rb
     """
+
     workspace: str = None  # Use a workspace
     Readline: bool = None  # Whether to use the readline or not
     RealReadline: bool = None  # Whether to use the system's readline library instead of RBReadline
     HistFile: str = None  # Path to a file where we can store command history
     Config: str = None  # Path to the config file
     ConfirmExit: bool = None  # Whether to confirm before exiting
     XCommands: List[str] = None  # Additional startup commands
@@ -46,14 +49,15 @@
     Plugins: List[str] = None  # Plugins to load
 
 
 class RPCConsoles(ContextBase):
     """
     https://docs.metasploit.com/api/Msf/RPC/RPC_Console.html
     """
+
     CREATE = "console.create"
     DESTROY = "console.destroy"
     LIST = "console.list"
     READ = "console.read"
     WRITE = "console.write"
     TABS = "console.tabs"
     SESSION_KILL = "console.session_kill"
@@ -63,30 +67,26 @@
     def _parse_console_info(response: dict) -> ConsoleInfo:
         """
         Get console information from the response.
         :param response: API response containing the necessary data
         :return: Information about the console
         """
         return ConsoleInfo(
-            int(response[constants.B_ID]),
-            response[constants.B_PROMPT].decode(),
-            response[constants.B_BUSY]
+            int(response[constants.B_ID]), response[constants.B_PROMPT].decode(), response[constants.B_BUSY]
         )
 
     @staticmethod
     def _parse_console_data(response: dict) -> ConsoleData:
         """
         Get console data from the response.
         :param response: API response containing the necessary data
         :return: Information about the console and its data
         """
         return ConsoleData(
-            response[constants.B_PROMPT].decode(),
-            response[constants.B_BUSY],
-            response[constants.B_DATA].decode()
+            response[constants.B_PROMPT].decode(), response[constants.B_BUSY], response[constants.B_DATA].decode()
         )
 
     def create(self, options: ConsoleOptions = None) -> ConsoleInfo:
         """
         Create a new framework console instance.
         :param options: Options used for creating the console
         :return: Information about the console
@@ -104,15 +104,15 @@
         :param console_id: ID of the console
         :return: True in case of success
         :full response example: {b'result': b'success'}
         """
         response = self._context.call(self.DESTROY, [console_id])
 
         if response[constants.B_RESULT] == constants.B_FAILURE:
-            raise Exception("Invalid console ID")
+            raise exceptions.InputError("Invalid console ID")
 
         return response[constants.B_RESULT] == constants.B_SUCCESS
 
     def list_consoles(self) -> List[ConsoleInfo]:
         """
         List framework consoles.
         :return: List of framework consoles
@@ -132,15 +132,15 @@
         :param console_id: ID of the console
         :return: Output from the console
         :full response example: {b'data': b"... https://docs.metasploit.com/\n\n", b'prompt': b'msf6 > ', b'busy': True}
         """
         response = self._context.call(self.READ, [console_id])
 
         if response.get(constants.B_RESULT) == constants.B_FAILURE:
-            raise Exception("Invalid console ID")
+            raise exceptions.InputError("Invalid console ID")
 
         return self._parse_console_data(response)
 
     def write(self, console_id: int, data: str, add_new_line: bool = True) -> int:
         """
         Send an input (such as a command) to the framework console.
         :param console_id: ID of the console
@@ -151,59 +151,59 @@
         """
         if add_new_line:
             data += "\r\n"
 
         response = self._context.call(self.WRITE, [console_id, data])
 
         if response.get(constants.B_RESULT) == constants.B_FAILURE:
-            raise Exception("Invalid console ID")
+            raise exceptions.InputError("Invalid console ID")
 
         return response[constants.B_WROTE]
 
     def tabs(self, console_id: int, line: str) -> List[str]:
         """
         Get tab-completed version of your input (such as a module path).
         :param console_id: ID of the console
         :param line: Line you want to complete
         :return: Possible tab-completions for your input
         :full response example: {b'tabs': [b'use exploit/windows/smb/ms08_067_netapi']}
         """
         response = self._context.call(self.TABS, [console_id, line])
 
         if response.get(constants.B_RESULT) == constants.B_FAILURE:
-            raise Exception("Invalid console ID")
+            raise exceptions.InputError("Invalid console ID")
 
         return [tab.decode() for tab in response[constants.B_TABS]]
 
     def session_kill(self, console_id: int) -> bool:
         """
         Kill a framework session. This serves the same purpose as CTRL+C to abort an interactive session.
         Consider using the session API calls instead.
         :param console_id: ID of the console
         :return: True in case of success
         :full response example: {b'result': b'success'}
         """
         response = self._context.call(self.SESSION_KILL, [console_id])
 
         if response[constants.B_RESULT] == constants.B_FAILURE:
-            raise Exception("Invalid console ID")
+            raise exceptions.InputError("Invalid console ID")
 
         return response[constants.B_RESULT] == constants.B_SUCCESS
 
     def session_detach(self, console_id: int) -> bool:
         """
         Detache a framework session. This serves the same purpose as CTRL+Z to background an interactive session.
         :param console_id: ID of the console
         :return: True in case of success
         :full response example: {b'result': b'success'}
         """
         response = self._context.call(self.SESSION_DETACH, [console_id])
 
         if response[constants.B_RESULT] == constants.B_FAILURE:
-            raise Exception("Invalid console ID")
+            raise exceptions.InputError("Invalid console ID")
 
         return response[constants.B_RESULT] == constants.B_SUCCESS
 
 
 class Console:
     def __init__(self, rpc: RPCConsoles, console_id: int):
         self._rpc = rpc
@@ -262,8 +262,8 @@
         self.rpc = RPCConsoles(context)
 
     def create(self, options: ConsoleOptions = None):
         console_info = self.rpc.create(options)
         return Console(self.rpc, console_info.id)
 
     def all(self):
-        return self.rpc.list_consoles()
+        return self.rpc.list_consoles()
```

### Comparing `snek_sploit-0.3.0/snek_sploit/lib/rpc/core.py` & `snek_sploit-0.4.0/snek_sploit/lib/rpc/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,54 +1,58 @@
 from requests import ReadTimeout
 from dataclasses import dataclass
 from typing import Union, Dict
 
 from snek_sploit.lib.context import ContextBase, Context
-from snek_sploit.util import constants
+from snek_sploit.util import constants, exceptions
 
 
 @dataclass
 class ModuleStatistics:
     """
     Number of installed modules.
     """
+
     exploits: int
     auxiliary: int
     post: int
     encoders: int
     nops: int
     payloads: int
     evasions: int
 
 
 @dataclass
 class VersionInformation:
     """
     Information about framework versions.
     """
+
     version: str
     ruby: str
     api: str
 
 
 @dataclass
 class FrameworkThread:
     """
     Information about framework thread.
     """
+
     status: str
     critical: bool
     name: str
     started: str
 
 
 class RPCCore(ContextBase):
     """
     https://docs.metasploit.com/api/Msf/RPC/RPC_Core.html
     """
+
     VERSION = "core.version"
     STOP = "core.stop"
     GETG = "core.getg"
     SETG = "core.setg"
     UNSETG = "core.unsetg"
     SAVE = "core.save"
     MODULE_STATS = "core.module_stats"
@@ -61,17 +65,15 @@
     def _parse_version(response: Dict[bytes, Union[bytes, str]]) -> VersionInformation:
         """
         Get versions from the response.
         :param response: API response containing the necessary data
         :return: Parsed version information
         """
         return VersionInformation(
-            response[constants.B_VERSION],
-            response[constants.B_RUBY].decode(),
-            response[constants.B_API].decode()
+            response[constants.B_VERSION], response[constants.B_RUBY].decode(), response[constants.B_API].decode()
         )
 
     @staticmethod
     def _parse_module_statistics(response: Dict[bytes, int]) -> ModuleStatistics:
         """
         Get module statistics from the response.
         :param response: API response containing the necessary data
@@ -94,15 +96,15 @@
         :param response: API response containing the necessary data
         :return: Parsed framework thread information
         """
         return FrameworkThread(
             response[constants.STATUS].decode(),
             response[constants.CRITICAL],
             response[constants.NAME],
-            response[constants.STARTED]
+            response[constants.STARTED],
         )
 
     def version(self) -> VersionInformation:
         """
         Get the RPC service versions.
         :return: RPC service versions
         :full response example:
@@ -136,15 +138,15 @@
         """
         variable = variable.upper()
 
         response = self._context.call(self.GETG, [variable])
 
         value = response[variable.encode()]
         if value == "":
-            raise Exception("Undefined variable")
+            raise exceptions.InputError("Undefined variable")
 
         return value.decode()
 
     def global_set(self, variable: str, value: str) -> bool:
         """
         Set a global datastore option (variable).
         :param variable: Name of the variable
```

### Comparing `snek_sploit-0.3.0/snek_sploit/lib/rpc/db.py` & `snek_sploit-0.4.0/snek_sploit/lib/rpc/db.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
 
 @dataclass
 class AnalyzeHostOptions:
     """
     Options used to get module suggestions.
     """
+
     workspace: str  # Name of the workspace
     addr: str  # Host address
     address: str  # Same as addr
     host: str  # Same as addr
     analyze_options: Dict[str, object]  # All returned modules will support these options # TODO: no clue; what is obj?
 
 
@@ -44,14 +45,15 @@
 
 
 # TODO unfinished, untested
 class RPCDB(ContextBase):
     """
     https://docs.metasploit.com/api/Msf/RPC/RPC_Db.html
     """
+
     CREATE_CRACKED_CREDENTIAL = "db.create_cracked_credential"
     CREATE_CREDENTIAL = "db.create_credential"
     INVALIDATE_LOGIN = "db.invalidate_login"
     CREDS = "db.creds"
     DEL_CREDS = "db.del_creds"
     HOSTS = "db.hosts"
     SERVICES = "db.services"
```

### Comparing `snek_sploit-0.3.0/snek_sploit/lib/rpc/health.py` & `snek_sploit-0.4.0/snek_sploit/lib/rpc/health.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from snek_sploit.util import constants
 
 
 class RPCHealth(ContextBase):
     """
     https://docs.metasploit.com/api/Msf/RPC/RPC_Health.html
     """
+
     CHECK = "health.check"
 
     def check(self) -> bool:
         """
         Check if the service is currently healthy and ready to accept requests.
         :return: True in case of success
         :full response example: {'status': b'UP'}
```

### Comparing `snek_sploit-0.3.0/snek_sploit/lib/rpc/jobs.py` & `snek_sploit-0.4.0/snek_sploit/lib/rpc/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,29 @@
     datastore: Dict[str, Any]
 
 
 class RPCJobs(ContextBase):
     """
     https://docs.metasploit.com/api/Msf/RPC/RPC_Job.html
     """
+
     INFO = "job.info"
     LIST = "job.list"
     STOP = "job.stop"
 
     @staticmethod
     def _parse_job_information(response: Dict[str, Any]) -> JobInformation:
         return JobInformation(
             response[constants.JID],
             response[constants.NAME].decode(),
             response[constants.START_TIME],
-            {key.decode() if isinstance(key, bytes) else key: value
-             for key, value in response[constants.DATASTORE].items()}
+            {
+                key.decode() if isinstance(key, bytes) else key: value
+                for key, value in response[constants.DATASTORE].items()
+            },
         )
 
     def info(self, job_id: int) -> JobInformation:
         """
         Get information about a job.
         :param job_id: ID of the job
         :return: Information about the job
```

### Comparing `snek_sploit-0.3.0/snek_sploit/lib/rpc/modules.py` & `snek_sploit-0.4.0/snek_sploit/lib/rpc/modules.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,39 +7,43 @@
 
 
 @dataclass
 class ModuleShortInfo:
     """
     Short module information.
     """
+
     type: str
     name: str
     fullname: str
     rank: str
     disclosure_date: str
 
 
 @dataclass
 class ModuleRunningStatistics:
     """
     Jobs' statistics. Matched using job's UUID.
     """
+
     waiting: List[str]
     running: List[str]
     results: List[str]
 
 
 @dataclass
 class ModuleExecutionInfo:
     """
     Execution information.
     """
+
     job_id: int
     uuid: str
 
+
 # @dataclass
 # class DatastoreOption:  # TODO: some are probably missing, needs more research and testing
 #     type: str
 #     required: bool
 #     advanced: bool
 #     evasion: bool
 #     desc: str
@@ -58,14 +62,15 @@
         arch: Architecture
         ecount: Number of times to encode
         inject: Enable injection
         template: Template file (an executable)
         template_path: Template path
         addshellcode: Custom shellcode
     """
+
     format: str = None
     badchars: str = None
     platform: str = None
     arch: str = None
     ecount: int = None
     inject: bool = None
     template: str = None
@@ -73,14 +78,15 @@
     addshellcode: str = None
 
 
 class RPCModules(ContextBase):
     """
     https://docs.metasploit.com/api/Msf/RPC/RPC_Module.html
     """
+
     EXPLOITS = "module.exploits"
     EVASION = "module.evasion"
     AUXILIARY = "module.auxiliary"
     PAYLOADS = "module.payloads"
     ENCODERS = "module.encoders"
     NOPS = "module.nops"
     POST = "module.post"
@@ -113,15 +119,15 @@
         :return: Parsed module's short information
         """
         return ModuleShortInfo(
             response[constants.B_TYPE],
             response[constants.B_NAME],
             response[constants.B_FULLNAME],
             response[constants.B_RANK].decode(),
-            response[constants.B_DISCLOSURE_DATE].decode()
+            response[constants.B_DISCLOSURE_DATE].decode(),
         )
 
     # TODO: once the DatastoreOption dataclass is implemented
     # def _parse_datastore_option(self, response: Dict[bytes, Union[bytes, bool, int]]):
     #     # Using auto-decode, since in some cases the enums parameter can contain multiple types (others probably too)
     #     decoded = self.decode(response)
     #
@@ -161,16 +167,17 @@
         :return: List of auxiliary names.
         :full response example: {b'modules': ['admin/2wire/xslt_password_reset']}
         """
         response = self._context.call(self.AUXILIARY)
 
         return response[constants.B_MODULES]
 
-    def list_payload_modules(self, fields: List[str] = None, architectures: List[str] = None) \
-            -> Union[List[str], Dict[str, Dict[str, str]]]:
+    def list_payload_modules(
+        self, fields: List[str] = None, architectures: List[str] = None
+    ) -> Union[List[str], Dict[str, Dict[str, str]]]:
         # TODO: split into 2 methods?
         # TODO: can the dict in dict (fields) have a different value?
         """
         Get a list of payload module names.
         In case you define a field/architecture, you get a dictionary with more information.
         :param fields: Module information fields to display
         :param architectures: Module supported architectures
@@ -184,16 +191,17 @@
         if architectures is not None:
             architectures = ",".join(architectures)
 
         response = self._context.call(self.PAYLOADS, [fields, architectures])
 
         return response[constants.B_MODULES]
 
-    def list_encoder_modules(self, fields: List[str] = None, architectures: List[str] = None) \
-            -> Union[List[str], Dict[str, Dict[str, str]]]:
+    def list_encoder_modules(
+        self, fields: List[str] = None, architectures: List[str] = None
+    ) -> Union[List[str], Dict[str, Dict[str, str]]]:
         # TODO: split into 2 methods?
         # TODO: can the dict in dict (fields) have a different value?
         """
         Get a list of encoder module names.
         In case you define a field/architecture, you get a dictionary with more information.
         :param fields: Module information fields to display
         :param architectures: Module supported architectures
@@ -207,16 +215,17 @@
         if architectures is not None:
             architectures = ",".join(architectures)
 
         response = self._context.call(self.ENCODERS, [fields, architectures])
 
         return response[constants.B_MODULES]
 
-    def list_nop_modules(self, fields: List[str] = None, architectures: List[str] = None) \
-            -> Union[List[str], Dict[str, Dict[str, str]]]:
+    def list_nop_modules(
+        self, fields: List[str] = None, architectures: List[str] = None
+    ) -> Union[List[str], Dict[str, Dict[str, str]]]:
         # TODO: split into 2 methods?
         # TODO: can the dict in dict (fields) have a different value?
         """
         Get a list of NOP module names.
         In case you define a field/architecture, you get a dictionary with more information.
         :param fields: Module information fields to display
         :param architectures: Module supported architectures
@@ -357,19 +366,20 @@
         :full response example: {b'waiting': [], b'running': [b'RNEN1jKepDfcWLpvuPlmhktc'], b'results': []}
         """
         response = self._context.call(self.RUNNING_STATS)
 
         return ModuleRunningStatistics(
             [each.decode() for each in response[constants.B_WAITING]],
             [each.decode() for each in response[constants.B_RUNNING]],
-            response[constants.B_RESULTS]
+            response[constants.B_RESULTS],
         )
 
-    def list_module_options(self, module_type: ModuleType, module_name: str) \
-            -> Dict[str, Dict[str, Union[dict, list, str, bool, int]]]:
+    def list_module_options(
+        self, module_type: ModuleType, module_name: str
+    ) -> Dict[str, Dict[str, Union[dict, list, str, bool, int]]]:
         """
         Get module's datastore options.
         :param module_type: Module type
         :param module_name: Module name
         :return: Module's datastore options (variables)
         :full response example:
             {b'WORKSPACE': {b'type': b'string', b'required': False, b'advanced': True, b'evasion': False,
```

### Comparing `snek_sploit-0.3.0/snek_sploit/lib/rpc/plugins.py` & `snek_sploit-0.4.0/snek_sploit/lib/rpc/plugins.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from snek_sploit.util import constants
 
 
 class RPCPlugins(ContextBase):
     """
     https://docs.metasploit.com/api/Msf/RPC/RPC_Plugin.html
     """
+
     LOAD = "plugin.load"
     UNLOAD = "plugin.unload"
     LOADED = "plugin.loaded"
 
     def load(self, name: str, options: dict = None) -> bool:
         """
         Load a plugin.
```

### Comparing `snek_sploit-0.3.0/snek_sploit/lib/rpc/sessions.py` & `snek_sploit-0.4.0/snek_sploit/lib/rpc/sessions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABC, abstractmethod
 from typing import List, Dict, Union
 from dataclasses import dataclass, asdict
 import time
 
 from snek_sploit.lib.context import ContextBase, Context
-from snek_sploit.util import constants
+from snek_sploit.util import constants, exceptions
 from snek_sploit.util.enums import SessionType
 
 
 @dataclass
 class SessionInformation:
     """
     Information about a session.
@@ -28,14 +28,15 @@
         username: Username
         uuid: UUID
         exploit_uuid: Exploit's UUID
         routes: Routes
         arch: Architecture
         platform: Platform (Only if the session type is `meterpreter`)
     """
+
     type: str = None
     tunnel_local: str = None
     tunnel_peer: str = None
     via_exploit: str = None
     via_payload: str = None
     desc: str = None
     info: str = None
@@ -54,16 +55,19 @@
         # TODO: allow dict
         if not isinstance(other, SessionInformation):
             return False
 
         this = asdict(self)
         for key, o_value in asdict(other).items():
             t_value = this[key]
-            if o_value is not None and t_value is not None \
-                    and ((strict and o_value != t_value) or (not strict and o_value not in t_value)):
+            if (
+                o_value is not None
+                and t_value is not None
+                and ((strict and o_value != t_value) or (not strict and o_value not in t_value))
+            ):
                 return False
 
         return True
 
 
 # TODO: allow usage of a dict instead of a dataclass (everywhere)
 @dataclass
@@ -83,14 +87,15 @@
         proxy_pass: The password to authenticate to the proxy with
         comm_timeout: Connection timeout in seconds
         session_exp: Session Expiration Timeout
         retry_total: Total number of times to retry establishing the transport
         retry_wait: The number of seconds to wait between retries
         cert: Path to the SSL Cert to use for HTTPS
     """
+
     transport: str
     lhost: str
     lport: str
     ua: str
     proxy_host: str
     proxy_port: str
     proxy_type: str
@@ -103,14 +108,15 @@
     cert: str
 
 
 class RPCSessions(ContextBase):
     """
     https://docs.metasploit.com/api/Msf/RPC/RPC_Session.html
     """
+
     LIST = "session.list"
     STOP = "session.stop"
     SHELL_READ = "session.shell_read"
     SHELL_WRITE = "session.shell_write"
     SHELL_UPGRADE = "session.shell_upgrade"
     METERPRETER_READ = "session.meterpreter_read"
     METERPRETER_WRITE = "session.meterpreter_write"
@@ -148,15 +154,15 @@
             parsed_response[constants.SESSION_PORT],
             parsed_response[constants.TARGET_HOST],
             parsed_response[constants.USERNAME],
             parsed_response[constants.UUID],
             parsed_response[constants.EXPLOIT_UUID],
             parsed_response[constants.ROUTES],
             parsed_response[constants.ARCH],
-            parsed_response.get(constants.PLATFORM, "")
+            parsed_response.get(constants.PLATFORM, ""),
         )
 
     def list_sessions(self) -> Dict[int, SessionInformation]:
         """
         Get a list of sessions that belong to the framework instance used by the RPC service.
         :return: Existing sessions
         :full response example:
@@ -407,15 +413,17 @@
 class Session(ABC):
     def __init__(self, rpc: RPCSessions, session_id: int, info: SessionInformation = None):
         self._rpc = rpc
         self.id = session_id
         try:
             self.info = info if info is not None else self.fetch_information()
         except Exception:
-            raise Exception(f"Unable to fetch information about the session with id {self.id}. Make sure it exists.")
+            raise exceptions.InputError(
+                f"Unable to fetch information about the session with id {self.id}. Make sure it exists."
+            )
 
     def fetch_information(self) -> SessionInformation:
         return self._rpc.list_sessions()[self.id]
 
     def kill(self) -> bool:
         return self._rpc.stop(self.id)
 
@@ -427,20 +435,31 @@
         pass
 
     @abstractmethod
     def read(self) -> str:
         pass
 
     @abstractmethod
-    def execute(self, command: str, minimal_execution_time: float, timeout: float, success_flags: List[str],
-                reading_delay: float) -> str:
+    def execute(
+        self,
+        command: str,
+        minimal_execution_time: float,
+        timeout: float,
+        success_flags: List[str],
+        reading_delay: float,
+    ) -> str:
         pass
 
-    def gather_output(self, minimal_execution_time: float = 3, timeout: float = None, success_flags: List[str] = None,
-                      reading_delay: float = 1) -> str:
+    def gather_output(
+        self,
+        minimal_execution_time: float = 3,
+        timeout: float = None,
+        success_flags: List[str] = None,
+        reading_delay: float = 1,
+    ) -> str:
         """
         Gather output from the session.
         :param minimal_execution_time: The minimum amount of seconds to wait before exiting in case no output is read
         :param timeout: The maximum time to wait for the output
         :param success_flags: Flags to indicate the gathered output is enough (one flag == stop gathering)
         :param reading_delay: Delay between the readings
         :return: Gathered output
@@ -491,16 +510,22 @@
         if payload is None:
             return self._rpc.shell_upgrade(self.id, local_host, local_port)
 
         # TODO: set PAYLOAD_OVERRIDE: linux/x64/meterpreter/reverse_tcp,
         #  module: post/multi/manage/shell_to_meterpreter
         return False
 
-    def execute(self, command: str, minimal_execution_time: float = 3, timeout: float = None,
-                success_flags: List[str] = None, reading_delay: float = 1) -> str:
+    def execute(
+        self,
+        command: str,
+        minimal_execution_time: float = 3,
+        timeout: float = None,
+        success_flags: List[str] = None,
+        reading_delay: float = 1,
+    ) -> str:
         self.clear_buffer()
         self.write(command)
 
         return self.gather_output(minimal_execution_time, timeout, success_flags, reading_delay)
 
 
 class SessionMeterpreter(Session):
@@ -529,23 +554,36 @@
 
     def detach(self) -> bool:
         return self._rpc.meterpreter_session_detach(self.id)
 
     def change_transport(self, options: MeterpreterSessionTransportOptions) -> bool:
         return self._rpc.meterpreter_transport_change(self.id, options)
 
-    def execute(self, command: str, minimal_execution_time: float = 3, timeout: float = None,
-                success_flags: List[str] = None, reading_delay: float = 1) -> str:
+    def execute(
+        self,
+        command: str,
+        minimal_execution_time: float = 3,
+        timeout: float = None,
+        success_flags: List[str] = None,
+        reading_delay: float = 1,
+    ) -> str:
         self.clear_buffer()
         self.write(command)
 
         return self.gather_output(minimal_execution_time, timeout, success_flags, reading_delay)
 
-    def execute_in_shell(self, command: str, arguments: List[str], minimal_execution_time: float = 3,
-                         timeout: float = None, success_flags: List[str] = None, reading_delay: float = 1) -> str:
+    def execute_in_shell(
+        self,
+        command: str,
+        arguments: List[str],
+        minimal_execution_time: float = 3,
+        timeout: float = None,
+        success_flags: List[str] = None,
+        reading_delay: float = 1,
+    ) -> str:
         self.clear_buffer()
 
         # TODO: test with custom x64 payload
         self.run_single(f"execute -f {command} -c -i -a {' '.join(arguments)}")
 
         return self.gather_output(minimal_execution_time, timeout, success_flags, reading_delay)
 
@@ -554,29 +592,38 @@
     def write(self, data: str) -> bool:
         self._rpc.ring_put(self.id, data)
         return True
 
     def read(self) -> str:
         return self._rpc.ring_read(self.id)
 
-    def execute(self, command: str, minimal_execution_time: float = 3, timeout: float = None,
-                success_flags: List[str] = None, reading_delay: float = 1) -> str:
+    def execute(
+        self,
+        command: str,
+        minimal_execution_time: float = 3,
+        timeout: float = None,
+        success_flags: List[str] = None,
+        reading_delay: float = 1,
+    ) -> str:
         self.clear_buffer()
         self.write(command)
 
         return self.gather_output(minimal_execution_time, timeout, success_flags, reading_delay)
 
 
 class Sessions(ContextBase):
     def __init__(self, context: Context):
         super().__init__(context)
         self.rpc = RPCSessions(context)
 
     def get(self, session_id: int) -> Union[SessionShell, SessionMeterpreter, SessionRing]:
-        session_info = self.rpc.list_sessions()[session_id]
+        try:
+            session_info = self.rpc.list_sessions()[session_id]
+        except KeyError:
+            raise exceptions.InputError(f"Session with ID {session_id} doesn't exist.")
         session_type = session_info.type
         if session_type == SessionType.SHELL:
             return SessionShell(self.rpc, session_id, session_info)
         elif session_type == SessionType.METERPRETER:
             return SessionMeterpreter(self.rpc, session_id, session_info)
         else:
             return SessionRing(self.rpc, session_id, session_info)
```

### Comparing `snek_sploit-0.3.0/snek_sploit/util/constants.py` & `snek_sploit-0.4.0/snek_sploit/util/constants.py`

 * *Files identical despite different names*

### Comparing `snek_sploit-0.3.0/PKG-INFO` & `snek_sploit-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snek-sploit
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python RPC client for Metasploit Framework
 Home-page: https://github.com/SadParad1se/snek-sploit
 License: MIT
 Keywords: metasploit,msf,rpc,client
 Author: Jiří Rája
 Author-email: jiri.raja@gmail.com
 Maintainer: Jiří Rája
@@ -13,16 +13,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: msgpack (>=1.0.8,<2.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: msgpack (>=1,<2)
+Requires-Dist: requests (>=2.31,<3.0)
 Project-URL: Repository, https://github.com/SadParad1se/snek-sploit
 Description-Content-Type: text/markdown
 
 # snek-sploit
 Python typed RPC client for Metasploit Framework.
 
 ![](logo.png)
```

