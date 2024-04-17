# Comparing `tmp/replit_river-0.1.5.tar.gz` & `tmp/replit_river-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replit_river-0.1.5.tar", max compression
+gzip compressed data, was "replit_river-0.1.6.tar", max compression
```

## Comparing `replit_river-0.1.5.tar` & `replit_river-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1064 2024-04-02 22:20:09.999604 replit_river-0.1.5/LICENSE
--rw-r--r--   0        0        0     1628 2024-03-26 20:33:50.343232 replit_river-0.1.5/README.md
--rw-r--r--   0        0        0     1732 2024-04-11 23:45:50.609062 replit_river-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      487 2024-04-11 21:05:27.020432 replit_river-0.1.5/replit_river/__init__.py
--rw-r--r--   0        0        0    18569 2024-04-11 21:02:04.035350 replit_river-0.1.5/replit_river/client.py
--rw-r--r--   0        0        0        0 2024-04-11 18:24:00.533020 replit_river-0.1.5/replit_river/codegen/__init__.py
--rwxr-xr-x   0        0        0      153 2024-04-11 18:24:00.533220 replit_river-0.1.5/replit_river/codegen/__main__.py
--rw-r--r--   0        0        0    13363 2024-04-11 23:41:44.032313 replit_river-0.1.5/replit_river/codegen/client.py
--rw-r--r--   0        0        0     1903 2024-04-11 18:24:00.535693 replit_river-0.1.5/replit_river/codegen/run.py
--rw-r--r--   0        0        0     5354 2024-04-11 18:24:00.535865 replit_river-0.1.5/replit_river/codegen/schema.py
--rw-r--r--   0        0        0    12624 2024-04-11 23:41:43.436976 replit_river-0.1.5/replit_river/codegen/server.py
--rw-r--r--   0        0        0      478 2024-04-11 18:33:34.741591 replit_river-0.1.5/replit_river/error_schema.py
--rw-r--r--   0        0        0        0 2024-04-11 18:24:00.536395 replit_river-0.1.5/replit_river/py.typed
--rw-r--r--   0        0        0    11973 2024-04-11 18:34:41.139263 replit_river-0.1.5/replit_river/rpc.py
--rw-r--r--   0        0        0     2152 2024-04-11 21:05:41.429562 replit_river-0.1.5/replit_river/seq_manager.py
--rw-r--r--   0        0        0     1340 2024-04-11 21:05:27.021060 replit_river-0.1.5/replit_river/server.py
--rw-r--r--   0        0        0    15581 2024-04-11 21:05:49.017905 replit_river-0.1.5/replit_river/transport.py
--rw-r--r--   0        0        0     2450 1970-01-01 00:00:00.000000 replit_river-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-02 22:20:09.999604 replit_river-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1628 2024-03-26 20:33:50.343232 replit_river-0.1.6/README.md
+-rw-r--r--   0        0        0     1742 2024-04-17 19:11:30.870951 replit_river-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      487 2024-04-17 00:20:58.071349 replit_river-0.1.6/replit_river/__init__.py
+-rw-r--r--   0        0        0    19574 2024-04-17 18:56:54.976159 replit_river-0.1.6/replit_river/client.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:24:00.533020 replit_river-0.1.6/replit_river/codegen/__init__.py
+-rwxr-xr-x   0        0        0      153 2024-04-11 18:24:00.533220 replit_river-0.1.6/replit_river/codegen/__main__.py
+-rw-r--r--   0        0        0    13363 2024-04-17 00:20:58.072227 replit_river-0.1.6/replit_river/codegen/client.py
+-rw-r--r--   0        0        0     1903 2024-04-11 18:24:00.535693 replit_river-0.1.6/replit_river/codegen/run.py
+-rw-r--r--   0        0        0     5354 2024-04-11 18:24:00.535865 replit_river-0.1.6/replit_river/codegen/schema.py
+-rw-r--r--   0        0        0    12620 2024-04-17 19:05:12.058141 replit_river-0.1.6/replit_river/codegen/server.py
+-rw-r--r--   0        0        0      478 2024-04-17 00:20:58.073048 replit_river-0.1.6/replit_river/error_schema.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:24:00.536395 replit_river-0.1.6/replit_river/py.typed
+-rw-r--r--   0        0        0    11973 2024-04-17 19:05:34.905421 replit_river-0.1.6/replit_river/rpc.py
+-rw-r--r--   0        0        0     2152 2024-04-17 00:20:58.073573 replit_river-0.1.6/replit_river/seq_manager.py
+-rw-r--r--   0        0        0     1340 2024-04-17 00:20:58.073881 replit_river-0.1.6/replit_river/server.py
+-rw-r--r--   0        0        0     2336 2024-04-17 19:05:00.731417 replit_river-0.1.6/replit_river/task_manager.py
+-rw-r--r--   0        0        0    14852 2024-04-17 19:05:12.100062 replit_river-0.1.6/replit_river/transport.py
+-rw-r--r--   0        0        0     2446 1970-01-01 00:00:00.000000 replit_river-0.1.6/PKG-INFO
```

### Comparing `replit_river-0.1.5/LICENSE` & `replit_river-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.5/README.md` & `replit_river-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.5/pyproject.toml` & `replit_river-0.1.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name="replit-river"
-version="0.1.5"
+version="0.1.6"
 description="Replit river toolkit for Python"
 authors = ["Replit <eng@replit.com>"]
 license = "LICENSE"
 keywords = ["rpc", "websockets"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 river-codegen-py = "river.codegen:run"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 grpcio = "^1.59.3"
 grpcio-tools = "^1.59.3"
 protobuf = "^4.24.4"
-black = "^23.11.0"
+black = ">=23.11,<25.0"
 msgpack = "^1.0.7"
 aiochannel = "^1.2.1"
 nanoid = "^2.0.0"
 pydantic = "^2.5.2"
 websockets = "^12.0"
 pydantic-core = "^2.16.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 mypy = "^1.4.0"
-black = "^23.3.0"
+black = ">=23.3,<25.0"
 pytest-cov = "^4.1.0"
 ruff = "^0.0.278"
 pytest-mock = "^3.11.1"
 pytest-asyncio = "^0.21.1"
 types-protobuf = "^4.24.0.20240311"
 mypy-protobuf = "^3.5.0"
 deptry = "^0.14.0"
```

### Comparing `replit_river-0.1.5/replit_river/client.py` & `replit_river-0.1.6/replit_river/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 from collections.abc import AsyncIterable, AsyncIterator
 from typing import Any, Callable, Dict, Optional, Union
 
 import msgpack  # type: ignore
 import nanoid  # type: ignore
 from aiochannel import Channel
 from pydantic import ValidationError
-from websockets import Data
+from websockets import ConnectionClosedError, Data
 from websockets.client import WebSocketClientProtocol
 from websockets.exceptions import ConnectionClosed
 
 from replit_river.error_schema import ERROR_CODE_STREAM_CLOSED, RiverException
 from replit_river.seq_manager import (
     IgnoreTransportMessageException,
     InvalidTransportMessageException,
     SeqManager,
 )
+from replit_river.task_manager import BackgroundTaskManager
 from replit_river.transport import FailedSendingMessageException
 
 from .rpc import (
     ACK_BIT,
     STREAM_CLOSED_BIT,
     STREAM_OPEN_BIT,
     ControlMessageHandshakeRequest,
@@ -30,45 +31,38 @@
     RequestType,
     ResponseType,
     TransportMessage,
 )
 
 CROSIS_PREFIX_BYTES = b"\x00\x00"
 PID2_PREFIX_BYTES = b"\xff\xff"
+HEART_BEAT_INTERVAL_SECS = 2
 
 
 class Client:
     def __init__(
         self,
         websockets: WebSocketClientProtocol,
         use_prefix_bytes: bool = True,
         client_id: Optional[str] = None,
         server_id: Optional[str] = None,
     ) -> None:
         self.ws = websockets
-        self._tasks = set()
         self._from = nanoid.generate()
         self._streams: Dict[str, Channel[Dict[str, Any]]] = {}
         self._seq_manager = SeqManager()
         self._is_handshaked = False
         self._use_prefix_bytes = use_prefix_bytes
-        self._instance_id = client_id or "python-client-" + self.generate_nanoid()
+        self._client_id = client_id or "python-client-" + self.generate_nanoid()
         self._server_id = server_id or "SERVER"
+        self._background_task_manager = BackgroundTaskManager()
+        asyncio.create_task(self._start_handle_messages())
 
-        task = asyncio.create_task(self._handle_messages())
-        self._tasks.add(task)
-
-        def _handle_messages_callback(task: asyncio.Task) -> None:
-            self._tasks.remove(task)
-            if task.exception():
-                logging.error(
-                    f"Error in river.client._handle_messages: {task.exception()}"
-                )
-
-        task.add_done_callback(_handle_messages_callback)
+    async def _start_handle_messages(self) -> None:
+        await self._background_task_manager.create_task(self._handle_messages())
 
     async def send_close_stream(
         self, service_name: str, procedure_name: str, stream_id: str
     ) -> None:
         # close stream
         await self.send_transport_message(
             from_=self._from,
@@ -78,14 +72,37 @@
             streamId=stream_id,
             controlFlags=STREAM_CLOSED_BIT,
             payload={
                 "type": "CLOSE",
             },
         )
 
+    async def _heartbeat(
+        self,
+        msg: TransportMessage,
+    ) -> None:
+        logging.debug("Start heartbeat")
+        while True:
+            await asyncio.sleep(HEART_BEAT_INTERVAL_SECS)
+            try:
+                await self.send_transport_message(
+                    self._client_id,
+                    self._server_id,
+                    None,
+                    None,
+                    "heartbeat",
+                    ACK_BIT,
+                    {
+                        "ack": msg.id,
+                    },
+                )
+            except ConnectionClosedError:
+                logging.debug("heartbeat failed")
+                return
+
     def to_transport_message(self, message: Data) -> TransportMessage:
         unpacked = msgpack.unpackb(message, timestamp=3)
 
         return TransportMessage(**unpacked)
 
     async def send_transport_message(
         self,
@@ -144,15 +161,15 @@
             return data[2:]
         return data
 
     async def _handle_messages(self) -> None:
         handshake_request = ControlMessageHandshakeRequest(
             type="HANDSHAKE_REQ",
             protocolVersion="v1",
-            instanceId=self._instance_id,
+            instanceId=self._client_id,
         )
         try:
             await self.send_transport_message(
                 from_=self._from,
                 to=self._server_id,
                 serviceName=None,
                 procedureName=None,
@@ -176,62 +193,68 @@
             # TODO: close the connection here
             return
         if not handshake_response.status.ok:
             logging.error(f"Handshake failed: {handshake_response.status.reason}")
             # TODO: close the connection here
             return
         self._is_handshaked = True
+        await self._background_task_manager.create_task(self._heartbeat(first_message))
 
-        async for message in self.ws:
-            if isinstance(message, str):
-                # Not something we will try to handle.
-                logging.debug(
-                    "ignored a message beacuse it was a text frame: %r",
-                    message,
-                )
-                continue
-            if self._use_prefix_bytes:
-                if message[:2] == CROSIS_PREFIX_BYTES:
-                    logging.debug("ignored a crosis message")
+        try:
+            async for message in self.ws:
+                if isinstance(message, str):
+                    # Not something we will try to handle.
+                    logging.debug(
+                        "ignored a message beacuse it was a text frame: %r",
+                        message,
+                    )
                     continue
-                message = message[2:]
+                if self._use_prefix_bytes:
+                    if message[:2] == CROSIS_PREFIX_BYTES:
+                        logging.debug("ignored a crosis message")
+                        continue
+                    message = message[2:]
 
-            try:
-                unpacked = msgpack.unpackb(message, timestamp=3)
-                msg = TransportMessage(**unpacked)
                 try:
-                    await self._seq_manager.check_seq_and_update(msg)
-                except IgnoreTransportMessageException:
-                    continue
-                except InvalidTransportMessageException:
+                    unpacked = msgpack.unpackb(message, timestamp=3)
+                    msg = TransportMessage(**unpacked)
+                    try:
+                        await self._seq_manager.check_seq_and_update(msg)
+                    except IgnoreTransportMessageException:
+                        continue
+                    except InvalidTransportMessageException:
+                        return
+                    if msg.controlFlags == ACK_BIT:
+                        continue
+
+                except ConnectionClosed:
+                    logging.info("Connection closed")
+                    break
+
+                except (
+                    ValidationError,
+                    ValueError,
+                    msgpack.UnpackException,
+                    msgpack.exceptions.ExtraData,
+                ):
+                    logging.exception("failed to parse message")
                     return
-                if msg.controlFlags == ACK_BIT:
+                previous_output = self._streams.get(msg.streamId, None)
+                if not previous_output:
+                    logging.warning("no stream for %s", msg.streamId)
                     continue
-
-            except ConnectionClosed:
-                logging.info("Connection closed")
-                break
-
-            except (
-                ValidationError,
-                ValueError,
-                msgpack.UnpackException,
-                msgpack.exceptions.ExtraData,
-            ):
-                logging.exception("failed to parse message")
-                return
-            previous_output = self._streams.get(msg.streamId, None)
-            if not previous_output:
-                logging.warning("no stream for %s", msg.streamId)
-                continue
-            await previous_output.put(msg.payload)
-            if msg.controlFlags & STREAM_CLOSED_BIT != 0:
-                logging.info("Closing stream %s", msg.streamId)
-                previous_output.close()
-                del self._streams[msg.streamId]
+                await previous_output.put(msg.payload)
+                if msg.controlFlags & STREAM_CLOSED_BIT != 0:
+                    logging.info("Closing stream %s", msg.streamId)
+                    previous_output.close()
+                    del self._streams[msg.streamId]
+        except asyncio.CancelledError:
+            logging.debug("Client loop was successfully cancelled", exc_info=False)
+        finally:
+            await self._background_task_manager.cancel_all_tasks()
 
     async def send_rpc(
         self,
         service_name: str,
         procedure_name: str,
         request: RequestType,
         request_serializer: Callable[[RequestType], Any],
@@ -474,17 +497,15 @@
                     procedureName=procedure_name,
                     streamId=stream_id,
                     controlFlags=0,
                     payload=request_serializer(item),
                 )
             await self.send_close_stream(service_name, procedure_name, stream_id)
 
-        task = asyncio.create_task(_encode_stream())
-        self._tasks.add(task)
-        task.add_done_callback(lambda _: self._tasks.remove(task))
+        await self._background_task_manager.create_task(_encode_stream())
 
         # Handle potential errors during communication
         try:
             async for item in output:
                 if "type" in item and item["type"] == "CLOSE":
                     break
                 if not item.get("ok", False):
```

### Comparing `replit_river-0.1.5/replit_river/codegen/client.py` & `replit_river-0.1.6/replit_river/codegen/client.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.5/replit_river/codegen/run.py` & `replit_river-0.1.6/replit_river/codegen/run.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.5/replit_river/codegen/schema.py` & `replit_river-0.1.6/replit_river/codegen/schema.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.5/replit_river/codegen/server.py` & `replit_river-0.1.6/replit_river/codegen/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,17 +42,17 @@
         "  d: Mapping[str, Any],",
         f") -> {module_name}_pb2.{m.name}:",
         f"  m = {module_name}_pb2.{m.name}()",
         "  if d is None:",
         "    return m",
     ]
     # Non-oneof fields.
-    oneofs: DefaultDict[int, List[descriptor_pb2.FieldDescriptorProto]] = (
-        collections.defaultdict(list)
-    )
+    oneofs: DefaultDict[
+        int, List[descriptor_pb2.FieldDescriptorProto]
+    ] = collections.defaultdict(list)
     for field in m.field:
         if field.HasField("oneof_index"):
             oneofs[field.oneof_index].append(field)
             continue
         chunks.append(
             f"  if d.get('{to_camel_case(field.name)}') is not None:",
         )
@@ -153,17 +153,17 @@
     chunks = [
         f"def _{m.name}Encoder(",
         f"  e: {module_name}_pb2.{m.name}",
         ") -> Dict[str, Any]:",
         "  d: Dict[str, Any] = {}",
     ]
     # Non-oneof fields.
-    oneofs: DefaultDict[int, List[descriptor_pb2.FieldDescriptorProto]] = (
-        collections.defaultdict(list)
-    )
+    oneofs: DefaultDict[
+        int, List[descriptor_pb2.FieldDescriptorProto]
+    ] = collections.defaultdict(list)
     for field in m.field:
         if field.HasField("oneof_index"):
             oneofs[field.oneof_index].append(field)
             continue
         value: str
         if field.type_name == ".google.protobuf.Timestamp":
             value = f"_{field.name}.ToDatetime(tzinfo=datetime.timezone.utc)"
```

### Comparing `replit_river-0.1.5/replit_river/rpc.py` & `replit_river-0.1.6/replit_river/rpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
             "ok": True,
             "payload": response_serializer(response),
         }
 
 
 def rpc_method_handler(
     method: Callable[[RequestType, grpc.aio.ServicerContext], Awaitable[ResponseType]],
-    request_deserializer: Callable[[str], RequestType],
+    request_deserializer: Callable[[Any], RequestType],
     response_serializer: Callable[[ResponseType], Any],
 ) -> GenericRpcHandler:
     async def wrapped(
         peer: str,
         input: Channel[Any],
         output: Channel[Any],
     ) -> None:
```

### Comparing `replit_river-0.1.5/replit_river/seq_manager.py` & `replit_river-0.1.6/replit_river/seq_manager.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.5/replit_river/server.py` & `replit_river-0.1.6/replit_river/server.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.5/replit_river/transport.py` & `replit_river-0.1.6/replit_river/transport.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
 import logging
-from typing import Any, Dict, Optional, Set, Tuple
+from typing import Any, Dict, Optional, Tuple
 
 import msgpack  # type: ignore
 import nanoid  # type: ignore
 import websockets
 from aiochannel import Channel
 from pydantic import ValidationError
 from pydantic_core import ValidationError as PydanticCoreValidationError
@@ -12,14 +12,15 @@
 from websockets.server import WebSocketServerProtocol
 
 from replit_river.seq_manager import (
     IgnoreTransportMessageException,
     InvalidTransportMessageException,
     SeqManager,
 )
+from replit_river.task_manager import BackgroundTaskManager
 
 from .rpc import (
     ACK_BIT,
     STREAM_CLOSED_BIT,
     STREAM_OPEN_BIT,
     ControlMessageHandshakeRequest,
     ControlMessageHandshakeResponse,
@@ -76,18 +77,18 @@
         transports_manager: TransportManager,
     ) -> None:
         self._server_instance_id = server_instance_id
         self._client_instance_id: Optional[str] = None
         self._handlers = handlers
         self.websocket = websocket
         self.streams: Dict[str, Channel[Any]] = {}
-        self.background_tasks: Set[asyncio.Task] = set()
         self.is_handshake_success = False
         self._transports_manager = transports_manager
         self._seq_manager = SeqManager()
+        self._background_task_manager = BackgroundTaskManager()
 
     async def send_message(
         self,
         initial_message: TransportMessage,
         ws: WebSocketServerProtocol,
         control_flags: int,
         payload: Dict,
@@ -251,40 +252,14 @@
                         "ack": msg.id,
                     },
                 )
             except ConnectionClosedError:
                 logging.debug("heartbeat failed")
                 return
 
-    def remove_task(
-        self,
-        task_to_remove: asyncio.Task[Any],
-        background_tasks: Set[asyncio.Task],
-    ) -> None:
-        if task_to_remove in background_tasks:
-            background_tasks.remove(task_to_remove)
-        try:
-            exception = task_to_remove.exception()
-        except asyncio.CancelledError:
-            logging.debug("Task was cancelled", exc_info=False)
-            return
-        except Exception:
-            logging.error("Error retrieving task exception", exc_info=True)
-            return
-        if exception:
-            logging.error(
-                "Task resulted in an exception",
-                exc_info=exception,
-            )
-
-    def _create_task(self, fn: Any, tg: asyncio.TaskGroup) -> None:
-        task = tg.create_task(fn)
-        self.background_tasks.add(task)
-        task.add_done_callback(lambda x: self.remove_task(x, self.background_tasks))
-
     async def handle_messages_from_ws(
         self, websocket: WebSocketServerProtocol, tg: asyncio.TaskGroup
     ) -> None:
         async for message in websocket:
             try:
                 msg = self._parse_transport_msg(message)
             except IgnoreTransportMessageException:
@@ -295,15 +270,17 @@
 
             logging.debug("got a message %r", msg)
 
             if not self.is_handshake_success:
                 try:
                     await self._establish_handshake(msg, websocket)
                     self.is_handshake_success = True
-                    self._create_task(self._heartbeat(msg, websocket), tg)
+                    await self._background_task_manager.create_task(
+                        self._heartbeat(msg, websocket), tg
+                    )
                     logging.debug(
                         "handshake success for client_instance_id :"
                         f" {self._client_instance_id}"
                     )
 
                     continue
                 except InvalidTransportMessageException:
@@ -348,18 +325,18 @@
                     1024 if is_streaming_output else 1
                 )
                 await input_stream.put(msg.payload)
                 if not stream:
                     # We'll need to save it for later.
                     self.streams[msg.streamId] = input_stream
                 # Start the handler.
-                self._create_task(
+                await self._background_task_manager.create_task(
                     handler_func(msg.from_, input_stream, output_stream), tg
                 )
-                self._create_task(
+                await self._background_task_manager.create_task(
                     self.send_responses(
                         msg, websocket, output_stream, is_streaming_output
                     ),
                     tg,
                 )
 
             else:
@@ -403,11 +380,10 @@
                     "Unhandled exceptions on River server", unhandled.exceptions
                 )
 
     async def close(self) -> None:
         for previous_input in self.streams.values():
             previous_input.close()
         self.streams.clear()
-        for task in self.background_tasks:
-            task.cancel()
+        await self._background_task_manager.cancel_all_tasks()
         if self.websocket:
             await self.websocket.close()
```

### Comparing `replit_river-0.1.5/PKG-INFO` & `replit_river-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: replit-river
-Version: 0.1.5
+Version: 0.1.6
 Summary: Replit river toolkit for Python
 License: LICENSE
 Keywords: rpc,websockets
 Author: Replit
 Author-email: eng@replit.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiochannel (>=1.2.1,<2.0.0)
-Requires-Dist: black (>=23.11.0,<24.0.0)
+Requires-Dist: black (>=23.11,<25.0)
 Requires-Dist: grpcio (>=1.59.3,<2.0.0)
 Requires-Dist: grpcio-tools (>=1.59.3,<2.0.0)
 Requires-Dist: msgpack (>=1.0.7,<2.0.0)
 Requires-Dist: nanoid (>=2.0.0,<3.0.0)
 Requires-Dist: protobuf (>=4.24.4,<5.0.0)
 Requires-Dist: pydantic (>=2.5.2,<3.0.0)
 Requires-Dist: pydantic-core (>=2.16.3,<3.0.0)
```

