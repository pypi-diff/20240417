# Comparing `tmp/iscp-0.9.1-py3-none-any.whl.zip` & `tmp/iscp-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,64 +1,60 @@
-Zip file size: 72115 bytes, number of entries: 62
+Zip file size: 75842 bytes, number of entries: 58
 -rw-r--r--  2.0 unx     3385 b- defN 80-Jan-01 00:00 iscp/__init__.py
--rw-r--r--  2.0 unx    32299 b- defN 80-Jan-01 00:00 iscp/_conn.py
--rw-r--r--  2.0 unx    15745 b- defN 80-Jan-01 00:00 iscp/_downstream.py
+-rw-r--r--  2.0 unx    32653 b- defN 80-Jan-01 00:00 iscp/_conn.py
+-rw-r--r--  2.0 unx    15759 b- defN 80-Jan-01 00:00 iscp/_downstream.py
 -rw-r--r--  2.0 unx      168 b- defN 80-Jan-01 00:00 iscp/_encoding/__init__.py
+-rw-r--r--  2.0 unx     3005 b- defN 80-Jan-01 00:00 iscp/_encoding/_codegen/iscp2/v1/common_pb2.py
+-rw-r--r--  2.0 unx     2901 b- defN 80-Jan-01 00:00 iscp/_encoding/_codegen/iscp2/v1/connection_pb2.py
+-rw-r--r--  2.0 unx    11050 b- defN 80-Jan-01 00:00 iscp/_encoding/_codegen/iscp2/v1/downstream_pb2.py
+-rw-r--r--  2.0 unx     3092 b- defN 80-Jan-01 00:00 iscp/_encoding/_codegen/iscp2/v1/e2e_call_pb2.py
+-rw-r--r--  2.0 unx     2307 b- defN 80-Jan-01 00:00 iscp/_encoding/_codegen/iscp2/v1/extensions/connection_pb2.py
+-rw-r--r--  2.0 unx     3671 b- defN 80-Jan-01 00:00 iscp/_encoding/_codegen/iscp2/v1/extensions/downstream_pb2.py
+-rw-r--r--  2.0 unx     1916 b- defN 80-Jan-01 00:00 iscp/_encoding/_codegen/iscp2/v1/extensions/e2e_call_pb2.py
+-rw-r--r--  2.0 unx     1671 b- defN 80-Jan-01 00:00 iscp/_encoding/_codegen/iscp2/v1/extensions/ping_pong_pb2.py
+-rw-r--r--  2.0 unx     3556 b- defN 80-Jan-01 00:00 iscp/_encoding/_codegen/iscp2/v1/extensions/upstream_pb2.py
+-rw-r--r--  2.0 unx     5167 b- defN 80-Jan-01 00:00 iscp/_encoding/_codegen/iscp2/v1/message_pb2.py
+-rw-r--r--  2.0 unx     4036 b- defN 80-Jan-01 00:00 iscp/_encoding/_codegen/iscp2/v1/metadata_pb2.py
+-rw-r--r--  2.0 unx     1870 b- defN 80-Jan-01 00:00 iscp/_encoding/_codegen/iscp2/v1/ping_pong_pb2.py
+-rw-r--r--  2.0 unx     2860 b- defN 80-Jan-01 00:00 iscp/_encoding/_codegen/iscp2/v1/result_code_pb2.py
+-rw-r--r--  2.0 unx     8376 b- defN 80-Jan-01 00:00 iscp/_encoding/_codegen/iscp2/v1/upstream_pb2.py
 -rw-r--r--  2.0 unx      540 b- defN 80-Jan-01 00:00 iscp/_encoding/_encoding.py
 -rw-r--r--  2.0 unx      168 b- defN 80-Jan-01 00:00 iscp/_encoding/_protobuf/__init__.py
--rw-r--r--  2.0 unx     1153 b- defN 80-Jan-01 00:00 iscp/_encoding/_protobuf/_protobuf.py
+-rw-r--r--  2.0 unx     1313 b- defN 80-Jan-01 00:00 iscp/_encoding/_protobuf/_protobuf.py
 -rw-r--r--  2.0 unx      101 b- defN 80-Jan-01 00:00 iscp/_encoding/_protobuf/converter/__init__.py
--rw-r--r--  2.0 unx     6248 b- defN 80-Jan-01 00:00 iscp/_encoding/_protobuf/converter/_common.py
--rw-r--r--  2.0 unx     6224 b- defN 80-Jan-01 00:00 iscp/_encoding/_protobuf/converter/_connection.py
--rw-r--r--  2.0 unx    10867 b- defN 80-Jan-01 00:00 iscp/_encoding/_protobuf/converter/_converter.py
--rw-r--r--  2.0 unx    26623 b- defN 80-Jan-01 00:00 iscp/_encoding/_protobuf/converter/_downstream.py
--rw-r--r--  2.0 unx     4672 b- defN 80-Jan-01 00:00 iscp/_encoding/_protobuf/converter/_e2e_call.py
--rw-r--r--  2.0 unx     6328 b- defN 80-Jan-01 00:00 iscp/_encoding/_protobuf/converter/_metadata.py
--rw-r--r--  2.0 unx     1964 b- defN 80-Jan-01 00:00 iscp/_encoding/_protobuf/converter/_ping_pong.py
--rw-r--r--  2.0 unx      496 b- defN 80-Jan-01 00:00 iscp/_encoding/_protobuf/converter/_result_code.py
--rw-r--r--  2.0 unx    20496 b- defN 80-Jan-01 00:00 iscp/_encoding/_protobuf/converter/_upstream.py
--rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 iscp/_encoding/codegen/__init__.py
--rw-r--r--  2.0 unx     1206 b- defN 80-Jan-01 00:00 iscp/_encoding/codegen/__init__.pyi
--rw-r--r--  2.0 unx     2236 b- defN 80-Jan-01 00:00 iscp/_encoding/codegen/common_pb2.py
--rw-r--r--  2.0 unx     2106 b- defN 80-Jan-01 00:00 iscp/_encoding/codegen/connection_pb2.py
--rw-r--r--  2.0 unx     8555 b- defN 80-Jan-01 00:00 iscp/_encoding/codegen/downstream_pb2.py
--rw-r--r--  2.0 unx     2247 b- defN 80-Jan-01 00:00 iscp/_encoding/codegen/e2e_call_pb2.py
--rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 iscp/_encoding/codegen/extensions/__init__.py
--rw-r--r--  2.0 unx      612 b- defN 80-Jan-01 00:00 iscp/_encoding/codegen/extensions/__init__.pyi
--rw-r--r--  2.0 unx     1608 b- defN 80-Jan-01 00:00 iscp/_encoding/codegen/extensions/connection_pb2.py
--rw-r--r--  2.0 unx     2850 b- defN 80-Jan-01 00:00 iscp/_encoding/codegen/extensions/downstream_pb2.py
--rw-r--r--  2.0 unx     1304 b- defN 80-Jan-01 00:00 iscp/_encoding/codegen/extensions/e2e_call_pb2.py
--rw-r--r--  2.0 unx     1101 b- defN 80-Jan-01 00:00 iscp/_encoding/codegen/extensions/ping_pong_pb2.py
--rw-r--r--  2.0 unx     2727 b- defN 80-Jan-01 00:00 iscp/_encoding/codegen/extensions/upstream_pb2.py
--rw-r--r--  2.0 unx     3908 b- defN 80-Jan-01 00:00 iscp/_encoding/codegen/message_pb2.py
--rw-r--r--  2.0 unx     3021 b- defN 80-Jan-01 00:00 iscp/_encoding/codegen/metadata_pb2.py
--rw-r--r--  2.0 unx     1327 b- defN 80-Jan-01 00:00 iscp/_encoding/codegen/ping_pong_pb2.py
--rw-r--r--  2.0 unx     2439 b- defN 80-Jan-01 00:00 iscp/_encoding/codegen/result_code_pb2.py
--rw-r--r--  2.0 unx     6424 b- defN 80-Jan-01 00:00 iscp/_encoding/codegen/upstream_pb2.py
+-rw-r--r--  2.0 unx     6318 b- defN 80-Jan-01 00:00 iscp/_encoding/_protobuf/converter/_common.py
+-rw-r--r--  2.0 unx     6294 b- defN 80-Jan-01 00:00 iscp/_encoding/_protobuf/converter/_connection.py
+-rw-r--r--  2.0 unx    10877 b- defN 80-Jan-01 00:00 iscp/_encoding/_protobuf/converter/_converter.py
+-rw-r--r--  2.0 unx    26976 b- defN 80-Jan-01 00:00 iscp/_encoding/_protobuf/converter/_downstream.py
+-rw-r--r--  2.0 unx     4732 b- defN 80-Jan-01 00:00 iscp/_encoding/_protobuf/converter/_e2e_call.py
+-rw-r--r--  2.0 unx     6418 b- defN 80-Jan-01 00:00 iscp/_encoding/_protobuf/converter/_metadata.py
+-rw-r--r--  2.0 unx     2004 b- defN 80-Jan-01 00:00 iscp/_encoding/_protobuf/converter/_ping_pong.py
+-rw-r--r--  2.0 unx      506 b- defN 80-Jan-01 00:00 iscp/_encoding/_protobuf/converter/_result_code.py
+-rw-r--r--  2.0 unx    20716 b- defN 80-Jan-01 00:00 iscp/_encoding/_protobuf/converter/_upstream.py
 -rw-r--r--  2.0 unx      103 b- defN 80-Jan-01 00:00 iscp/_exceptions/__init__.py
 -rw-r--r--  2.0 unx     1557 b- defN 80-Jan-01 00:00 iscp/_exceptions/_exceptions.py
 -rw-r--r--  2.0 unx     3416 b- defN 80-Jan-01 00:00 iscp/_flush_policy.py
 -rw-r--r--  2.0 unx      698 b- defN 80-Jan-01 00:00 iscp/_message/__init__.py
--rw-r--r--  2.0 unx     7192 b- defN 80-Jan-01 00:00 iscp/_message/_common.py
--rw-r--r--  2.0 unx     1852 b- defN 80-Jan-01 00:00 iscp/_message/_connection.py
--rw-r--r--  2.0 unx     4933 b- defN 80-Jan-01 00:00 iscp/_message/_downstream.py
+-rw-r--r--  2.0 unx     9119 b- defN 80-Jan-01 00:00 iscp/_message/_common.py
+-rw-r--r--  2.0 unx     1978 b- defN 80-Jan-01 00:00 iscp/_message/_connection.py
+-rw-r--r--  2.0 unx     4960 b- defN 80-Jan-01 00:00 iscp/_message/_downstream.py
 -rw-r--r--  2.0 unx     1077 b- defN 80-Jan-01 00:00 iscp/_message/_e2e.py
 -rw-r--r--  2.0 unx      314 b- defN 80-Jan-01 00:00 iscp/_message/_message.py
 -rw-r--r--  2.0 unx     3818 b- defN 80-Jan-01 00:00 iscp/_message/_metadata.py
 -rw-r--r--  2.0 unx      426 b- defN 80-Jan-01 00:00 iscp/_message/_ping_pong.py
 -rw-r--r--  2.0 unx     4434 b- defN 80-Jan-01 00:00 iscp/_message/_result_code.py
 -rw-r--r--  2.0 unx     5987 b- defN 80-Jan-01 00:00 iscp/_message/_upstream.py
 -rw-r--r--  2.0 unx     6078 b- defN 80-Jan-01 00:00 iscp/_model.py
--rw-r--r--  2.0 unx     1324 b- defN 80-Jan-01 00:00 iscp/_sequence.py
+-rw-r--r--  2.0 unx     1318 b- defN 80-Jan-01 00:00 iscp/_sequence.py
 -rw-r--r--  2.0 unx      937 b- defN 80-Jan-01 00:00 iscp/_ticker.py
 -rw-r--r--  2.0 unx      331 b- defN 80-Jan-01 00:00 iscp/_transport/__init__.py
 -rw-r--r--  2.0 unx     1751 b- defN 80-Jan-01 00:00 iscp/_transport/_negotiation_params.py
--rw-r--r--  2.0 unx     9195 b- defN 80-Jan-01 00:00 iscp/_transport/_quic.py
+-rw-r--r--  2.0 unx     9193 b- defN 80-Jan-01 00:00 iscp/_transport/_quic.py
 -rw-r--r--  2.0 unx     2903 b- defN 80-Jan-01 00:00 iscp/_transport/_transport.py
 -rw-r--r--  2.0 unx     3410 b- defN 80-Jan-01 00:00 iscp/_transport/_websocket.py
--rw-r--r--  2.0 unx    18854 b- defN 80-Jan-01 00:00 iscp/_upstream.py
--rw-r--r--  2.0 unx      206 b- defN 80-Jan-01 00:00 iscp/_utils.py
--rw-r--r--  2.0 unx    10619 b- defN 80-Jan-01 00:00 iscp-0.9.1.dist-info/LICENSE
-?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 iscp-0.9.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1280 b- defN 16-Jan-01 00:00 iscp-0.9.1.dist-info/METADATA
-?rw-r--r--  2.0 unx     5546 b- defN 16-Jan-01 00:00 iscp-0.9.1.dist-info/RECORD
-62 files, 279477 bytes uncompressed, 63221 bytes compressed:  77.4%
+-rw-r--r--  2.0 unx    19632 b- defN 80-Jan-01 00:00 iscp/_upstream.py
+-rw-r--r--  2.0 unx      570 b- defN 80-Jan-01 00:00 iscp/_utils.py
+-rw-r--r--  2.0 unx    10619 b- defN 80-Jan-01 00:00 iscp-1.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1381 b- defN 80-Jan-01 00:00 iscp-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 iscp-1.0.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     5306 b- defN 16-Jan-01 00:00 iscp-1.0.0.dist-info/RECORD
+58 files, 295810 bytes uncompressed, 67292 bytes compressed:  77.3%
```

## zipnote {}

```diff
@@ -6,105 +6,93 @@
 
 Filename: iscp/_downstream.py
 Comment: 
 
 Filename: iscp/_encoding/__init__.py
 Comment: 
 
-Filename: iscp/_encoding/_encoding.py
+Filename: iscp/_encoding/_codegen/iscp2/v1/common_pb2.py
 Comment: 
 
-Filename: iscp/_encoding/_protobuf/__init__.py
+Filename: iscp/_encoding/_codegen/iscp2/v1/connection_pb2.py
 Comment: 
 
-Filename: iscp/_encoding/_protobuf/_protobuf.py
+Filename: iscp/_encoding/_codegen/iscp2/v1/downstream_pb2.py
 Comment: 
 
-Filename: iscp/_encoding/_protobuf/converter/__init__.py
+Filename: iscp/_encoding/_codegen/iscp2/v1/e2e_call_pb2.py
 Comment: 
 
-Filename: iscp/_encoding/_protobuf/converter/_common.py
-Comment: 
-
-Filename: iscp/_encoding/_protobuf/converter/_connection.py
-Comment: 
-
-Filename: iscp/_encoding/_protobuf/converter/_converter.py
-Comment: 
-
-Filename: iscp/_encoding/_protobuf/converter/_downstream.py
-Comment: 
-
-Filename: iscp/_encoding/_protobuf/converter/_e2e_call.py
+Filename: iscp/_encoding/_codegen/iscp2/v1/extensions/connection_pb2.py
 Comment: 
 
-Filename: iscp/_encoding/_protobuf/converter/_metadata.py
+Filename: iscp/_encoding/_codegen/iscp2/v1/extensions/downstream_pb2.py
 Comment: 
 
-Filename: iscp/_encoding/_protobuf/converter/_ping_pong.py
+Filename: iscp/_encoding/_codegen/iscp2/v1/extensions/e2e_call_pb2.py
 Comment: 
 
-Filename: iscp/_encoding/_protobuf/converter/_result_code.py
+Filename: iscp/_encoding/_codegen/iscp2/v1/extensions/ping_pong_pb2.py
 Comment: 
 
-Filename: iscp/_encoding/_protobuf/converter/_upstream.py
+Filename: iscp/_encoding/_codegen/iscp2/v1/extensions/upstream_pb2.py
 Comment: 
 
-Filename: iscp/_encoding/codegen/__init__.py
+Filename: iscp/_encoding/_codegen/iscp2/v1/message_pb2.py
 Comment: 
 
-Filename: iscp/_encoding/codegen/__init__.pyi
+Filename: iscp/_encoding/_codegen/iscp2/v1/metadata_pb2.py
 Comment: 
 
-Filename: iscp/_encoding/codegen/common_pb2.py
+Filename: iscp/_encoding/_codegen/iscp2/v1/ping_pong_pb2.py
 Comment: 
 
-Filename: iscp/_encoding/codegen/connection_pb2.py
+Filename: iscp/_encoding/_codegen/iscp2/v1/result_code_pb2.py
 Comment: 
 
-Filename: iscp/_encoding/codegen/downstream_pb2.py
+Filename: iscp/_encoding/_codegen/iscp2/v1/upstream_pb2.py
 Comment: 
 
-Filename: iscp/_encoding/codegen/e2e_call_pb2.py
+Filename: iscp/_encoding/_encoding.py
 Comment: 
 
-Filename: iscp/_encoding/codegen/extensions/__init__.py
+Filename: iscp/_encoding/_protobuf/__init__.py
 Comment: 
 
-Filename: iscp/_encoding/codegen/extensions/__init__.pyi
+Filename: iscp/_encoding/_protobuf/_protobuf.py
 Comment: 
 
-Filename: iscp/_encoding/codegen/extensions/connection_pb2.py
+Filename: iscp/_encoding/_protobuf/converter/__init__.py
 Comment: 
 
-Filename: iscp/_encoding/codegen/extensions/downstream_pb2.py
+Filename: iscp/_encoding/_protobuf/converter/_common.py
 Comment: 
 
-Filename: iscp/_encoding/codegen/extensions/e2e_call_pb2.py
+Filename: iscp/_encoding/_protobuf/converter/_connection.py
 Comment: 
 
-Filename: iscp/_encoding/codegen/extensions/ping_pong_pb2.py
+Filename: iscp/_encoding/_protobuf/converter/_converter.py
 Comment: 
 
-Filename: iscp/_encoding/codegen/extensions/upstream_pb2.py
+Filename: iscp/_encoding/_protobuf/converter/_downstream.py
 Comment: 
 
-Filename: iscp/_encoding/codegen/message_pb2.py
+Filename: iscp/_encoding/_protobuf/converter/_e2e_call.py
 Comment: 
 
-Filename: iscp/_encoding/codegen/metadata_pb2.py
+Filename: iscp/_encoding/_protobuf/converter/_metadata.py
 Comment: 
 
-Filename: iscp/_encoding/codegen/ping_pong_pb2.py
+Filename: iscp/_encoding/_protobuf/converter/_ping_pong.py
 Comment: 
 
-Filename: iscp/_encoding/codegen/result_code_pb2.py
+Filename: iscp/_encoding/_protobuf/converter/_result_code.py
 Comment: 
 
-Filename: iscp/_encoding/codegen/upstream_pb2.py
+Filename: iscp/_encoding/_protobuf/converter/_upstream.py
 Comment: 
 
 Filename: iscp/_exceptions/__init__.py
 Comment: 
 
 Filename: iscp/_exceptions/_exceptions.py
 Comment: 
@@ -168,20 +156,20 @@
 
 Filename: iscp/_upstream.py
 Comment: 
 
 Filename: iscp/_utils.py
 Comment: 
 
-Filename: iscp-0.9.1.dist-info/LICENSE
+Filename: iscp-1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: iscp-0.9.1.dist-info/WHEEL
+Filename: iscp-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: iscp-0.9.1.dist-info/METADATA
+Filename: iscp-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: iscp-0.9.1.dist-info/RECORD
+Filename: iscp-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## iscp/__init__.py

```diff
@@ -72,15 +72,15 @@
     AfterReceiveAckCallback,
     BeforeSendDataPointsCallback,
     Upstream,
     UpstreamClosedEvent,
     UpstreamClosedEventHandler,
 )
 
-__version__ = "0.9.1"  # embed by poetry-dynamic-versioning
+__version__ = "1.0.0"  # embed by poetry-dynamic-versioning
 
 __all__ = [
     # conn
     "Conn",
     "TokenSource",
     "DisconnectedEventHandler",
     "DisconnectedEvent",
```

## iscp/_conn.py

```diff
@@ -164,16 +164,16 @@
         self._token_source = token_source
 
         # Event
         self._called_close_event = asyncio.Event()
         self._closed = asyncio.Event()
 
         # Read queue
-        self._downstream_call_queue: asyncio.Queue[Optional[DownstreamCall]] = asyncio.Queue(maxsize=8)
-        self._downstream_reply_queue: asyncio.Queue[Optional[DownstreamCall]] = asyncio.Queue(maxsize=8)
+        self._downstream_call_queue: asyncio.Queue[Optional[DownstreamCall]] = asyncio.Queue(256)
+        self._downstream_reply_queue: asyncio.Queue[Optional[DownstreamCall]] = asyncio.Queue(256)
 
         # Request callback queues
         self._request_callback_queues: Dict[int, asyncio.Queue[message.RequestMessage]] = {}
         self._upstream_call_callback_queues: Dict[str, asyncio.Queue[message.UpstreamCallAck]] = {}
         self._downstream_reply_callback_queues: Dict[str, asyncio.Queue[_model.DownstreamReplyCall]] = {}
 
         # StreamHolder
@@ -304,14 +304,15 @@
 
             # dispatch
             if isinstance(msg, DownstreamChunk):
                 await self._downstreams[msg.stream_id_alias]._handle_chunk(msg)
 
     async def _read_loop(self):
         while not self._called_close_event.is_set():
+            await asyncio.sleep(0)
             msg = await self._read()
 
             # dispatch
             if isinstance(msg, message.Ping):
                 await self._write(
                     message.Pong(
                         request_id=msg.request_id,
@@ -320,17 +321,19 @@
                 )
             elif isinstance(msg, DownstreamChunk):
                 await self._downstreams[msg.stream_id_alias]._handle_chunk(msg)
             elif isinstance(msg, DownstreamMetadata):
                 if msg.stream_id_alias in self._metadata_downstreams[msg.source_node_id]:
                     await self._metadata_downstreams[msg.source_node_id][msg.stream_id_alias]._handle_metadata(msg)
             elif isinstance(msg, message.DownstreamChunkAckComplete):
-                await self._downstreams[msg.stream_id_alias]._handle_chunk_ack_complete(
-                    msg
-                ) if msg.stream_id_alias in self._downstreams else None
+                (
+                    await self._downstreams[msg.stream_id_alias]._handle_chunk_ack_complete(msg)
+                    if msg.stream_id_alias in self._downstreams
+                    else None
+                )
             elif isinstance(msg, message.UpstreamChunkAck):
                 await self._upstreams[msg.stream_id_alias]._handle_ack(msg) if msg.stream_id_alias in self._upstreams else None
             elif isinstance(msg, DownstreamCall):
                 if msg.request_call_id == "":
                     await self._downstream_call_queue.put(msg)
                 elif msg.request_call_id in self._downstream_reply_callback_queues:
                     await self._downstream_reply_queue.put(msg)
@@ -421,15 +424,14 @@
         except Exception as e:
             logger.error(e)
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.close()
 
     async def _wait_for_connected(self) -> message.ConnectResponse:
-
         req = message.ConnectRequest(
             request_id=self._req_sequence(),
             node_id=self._node_id if self._node_id else "",
             protocol_version=self._protocol_version,
             ping_interval=self._ping_interval,
             ping_timeout=self._ping_timeout,
             extension_fields=message.ConnectRequestExtensionFields(
@@ -512,17 +514,19 @@
 
             up = Upstream(
                 id=resp.assigned_stream_id,
                 id_alias=resp.assigned_stream_id_alias,
                 data_id_aliases=resp.data_id_aliases,
                 server_time=resp.server_time,
                 requester=self._send_request,
-                sender=self._send_upstream_chunk_unreliable
-                if qos is message.QoS.UNRELIABLE and self._unreliable_writer
-                else self._send_upstream_chunk,
+                sender=(
+                    self._send_upstream_chunk_unreliable
+                    if qos is message.QoS.UNRELIABLE and self._unreliable_writer
+                    else self._send_upstream_chunk
+                ),
                 receive_ack_callback=receive_ack_callback,
                 send_data_point_callback=send_data_points_callback,
                 close_timeout=close_timeout,
                 session_id=session_id or "",
                 ack_interval=ack_interval,
                 expiry_interval=expiry_interval,
                 flush_policy=flush_policy,
@@ -535,38 +539,40 @@
             self._upstreams[up._id_alias] = up
             self._all_tasks.append(asyncio.create_task(self._remove_upstream_when_closed(up)))
             return up
 
         raise ISCPFailedMessageError(received_message=resp)
 
     async def _remove_upstream_when_closed(self, up: Upstream):
-        await up._is_closed.wait()
+        await up._closed.wait()
         del self._upstreams[up._id_alias]
 
     async def open_downstream(
         self,
         filters: List[message.DownstreamFilter],
         *,
         data_ids: Optional[List[message.DataID]] = None,
         qos: message.QoS | str = message.QoS.UNRELIABLE,
         expiry_interval: float = 1,
         ack_interval: float = 1,
         closed_event_handler: Optional[DownstreamClosedEventHandler] = None,
+        omit_empty_chunk=False,
     ) -> Downstream:
         """
 
         ダウンストリームを開きます。
 
         Args:
             filters (List[iscp.DownstreamFilter]): ダウンストリームフィルタのリスト
             data_ids (Optional[List[iscp.DataID]]): データIDのリスト
             qos (iscp.QoS|str): QoS
             expiry_interval (float): 有効期限（秒）
             ack_interval (float): Ack返却間隔（秒）
             closed_event_handler (Optional[iscp.DownstreamClosedEventHandler]): ダウンストリームクローズイベントのハンドラ
+            omit_empty_chunk (bool): 空チャンク省略フラグ。Trueにすると空のDataPointGroupのチャンクはサーバーから配信されません。
         Returns:
             iscp.Downstream: ダウンストリーム
         """
 
         stream_id_alias = self._stream_sequence()
         data_id_alias_sequence = Sequence.for_data_id_alias()
         if isinstance(qos, str):
@@ -575,14 +581,15 @@
             request_id=0,
             desired_stream_id_alias=stream_id_alias,
             downstream_filters=filters,
             expiry_interval=expiry_interval,
             data_id_aliases={} if data_ids is None else {data_id_alias_sequence(): v for v in data_ids},
             qos=qos,
             extension_fields=message.DownstreamOpenRequestExtensionFields(),
+            omit_empty_chunk=omit_empty_chunk,
         )
         resp = await self._send_request(req)
 
         if isinstance(resp, message.DownstreamOpenResponse):
             if resp.result_code is not message.ResultCode.SUCCEEDED:
                 raise ISCPFailedMessageError(
                     received_message=resp, message=f"code=[{resp.result_code}] msg=[{resp.result_string}]"
@@ -790,15 +797,14 @@
     def _unsubscribe_reply_call(
         self,
         request_call_id: str,
     ):
         del self._downstream_reply_callback_queues[request_call_id]
 
     async def send_call_and_wait_reply_call(self, upstream_call: _model.UpstreamCall) -> _model.DownstreamReplyCall:
-
         """
         E2Eコールを送信し、リプライコールを受信するまで待ちます。
 
         Args:
             upstream_call(iscp.UpstreamCall): アップストリームコール
 
         Returns:
```

## iscp/_downstream.py

```diff
@@ -7,15 +7,15 @@
 
 from . import _exceptions as exceptions
 from . import _message as message
 from . import _model
 from ._message import DateTime, DownstreamChunk, DownstreamMetadata
 from ._sequence import Sequence
 from ._ticker import Ticker
-from ._utils import drain
+from ._utils import drain, enqueue
 
 __all__ = [
     "Downstream",
     "_DownstreamChunkIterator",
     "DownstreamMetadata",
     "_DownstreamMetadataIterator",
     "DownstreamClosedEventHandler",
@@ -117,18 +117,18 @@
 
         self._requester = requester
 
         self._stream_message_sender = stream_message_sender
         self._request_message_sender = request_message_sender
 
         # Queue
-        self._queue: asyncio.Queue[Optional[DownstreamChunk]] = asyncio.Queue(maxsize=8)
+        self._queue: asyncio.Queue[Optional[DownstreamChunk]] = asyncio.Queue(maxsize=262144)
         self._generator_call_once = asyncio.Event()
 
-        self._metadata_queue: asyncio.Queue[Optional[DownstreamMetadata]] = asyncio.Queue(maxsize=8)
+        self._metadata_queue: asyncio.Queue[Optional[DownstreamMetadata]] = asyncio.Queue(maxsize=256)
         self._metadata_generator_call_once = asyncio.Event()
 
         # Buffer
         self._ack_chunk_result_buffer: List[message.DownstreamChunkResult] = []
         self._ack_data_id_aliases_buffer: Dict[int, message.DataID] = {}
         self._ack_upstream_info_buffer: Dict[int, message.UpstreamInfo] = {}
 
@@ -239,18 +239,18 @@
 
     async def _handle_chunk_ack_complete(self, msg: message.DownstreamChunkAckComplete):
         if msg.result_code == message.ResultCode.SUCCEEDED:
             return
         logger.warn(f"code[{msg.result_code!r}],message,[{msg.result_string!r}]")
 
     async def _handle_chunk(self, msg: DownstreamChunk):
-        await self._queue.put(msg)
+        enqueue(self._queue, msg)
 
     async def _handle_metadata(self, msg: DownstreamMetadata):
-        await self._metadata_queue.put(msg)
+        enqueue(self._metadata_queue, msg)
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.close()
```

## iscp/_encoding/_protobuf/_protobuf.py

```diff
@@ -1,8 +1,10 @@
-from ..._encoding.codegen.message_pb2 import Message as MessagePB
+# from ....iscp-proto.gen.pytnon.iscp2.v1.message_pbs import Message as MessagePB
+# from ..._encoding.codegen.message_pb2 import Message as MessagePB
+from ..._encoding._codegen.iscp2.v1.message_pb2 import Message as MessagePB
 from ..._message import Message
 from ..._transport._transport import Writer, Reader
 
 from .._encoding import Encoding, EncodingName
 from .converter import ProtoToWire, WireToProto
 from ..._exceptions import ISCPMalformedMessageError
```

## iscp/_encoding/_protobuf/converter/_common.py

```diff
@@ -1,16 +1,16 @@
 from typing import Dict, List
 
-from iscp._encoding.codegen.common_pb2 import DataFilter as DataFilterPB
-from iscp._encoding.codegen.common_pb2 import DataID as DataIDPB
-from iscp._encoding.codegen.common_pb2 import DataPoint as DataPointPB
-from iscp._encoding.codegen.common_pb2 import DataPointGroup as DataPointGroupPB
-from iscp._encoding.codegen.common_pb2 import DownstreamFilter as DownstreamFilterPB
-from iscp._encoding.codegen.common_pb2 import QoS as QoSPB
-from iscp._encoding.codegen.common_pb2 import StreamChunk as StreamChunkPB
+from iscp._encoding._codegen.iscp2.v1.common_pb2 import DataFilter as DataFilterPB
+from iscp._encoding._codegen.iscp2.v1.common_pb2 import DataID as DataIDPB
+from iscp._encoding._codegen.iscp2.v1.common_pb2 import DataPoint as DataPointPB
+from iscp._encoding._codegen.iscp2.v1.common_pb2 import DataPointGroup as DataPointGroupPB
+from iscp._encoding._codegen.iscp2.v1.common_pb2 import DownstreamFilter as DownstreamFilterPB
+from iscp._encoding._codegen.iscp2.v1.common_pb2 import QoS as QoSPB
+from iscp._encoding._codegen.iscp2.v1.common_pb2 import StreamChunk as StreamChunkPB
 from iscp._exceptions import ISCPMalformedMessageError
 from iscp._message import (
     DataFilter,
     DataID,
     DataPoint,
     DataPointGroup,
     DownstreamFilter,
```

## iscp/_encoding/_protobuf/converter/_connection.py

```diff
@@ -1,23 +1,23 @@
 from typing import Optional
 from uuid import UUID
 
-from iscp._encoding.codegen.connection_pb2 import ConnectRequest as ConnectRequestPB
-from iscp._encoding.codegen.connection_pb2 import ConnectResponse as ConnectResponsePB
-from iscp._encoding.codegen.connection_pb2 import Disconnect as DisconnectPB
-from iscp._encoding.codegen.extensions.connection_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.connection_pb2 import ConnectRequest as ConnectRequestPB
+from iscp._encoding._codegen.iscp2.v1.connection_pb2 import ConnectResponse as ConnectResponsePB
+from iscp._encoding._codegen.iscp2.v1.connection_pb2 import Disconnect as DisconnectPB
+from iscp._encoding._codegen.iscp2.v1.extensions.connection_pb2 import (
     ConnectRequestExtensionFields as ConnectRequestExtensionFieldsPB,
 )
-from iscp._encoding.codegen.extensions.connection_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.extensions.connection_pb2 import (
     ConnectResponseExtensionFields as ConnectResponseExtensionFieldsPB,
 )
-from iscp._encoding.codegen.extensions.connection_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.extensions.connection_pb2 import (
     DisconnectExtensionFields as DisconnectExtensionFieldsPB,
 )
-from iscp._encoding.codegen.extensions.connection_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.extensions.connection_pb2 import (
     IntdashExtensionFields as IntdashExtensionFieldsPB,
 )
 from iscp._message import (
     ConnectRequest,
     ConnectRequestExtensionFields,
     ConnectResponse,
     ConnectResponseExtensionFields,
```

## iscp/_encoding/_protobuf/converter/_converter.py

```diff
@@ -1,8 +1,8 @@
-from ...._encoding.codegen.message_pb2 import Message as MessagePB
+from ...._encoding._codegen.iscp2.v1.message_pb2 import Message as MessagePB
 from ...._exceptions import ISCPMalformedMessageError
 from ...._message import (
     ConnectRequest,
     ConnectResponse,
     Disconnect,
     DownstreamChunkAck,
     DownstreamChunkAckComplete,
```

## iscp/_encoding/_protobuf/converter/_downstream.py

```diff
@@ -1,81 +1,81 @@
 __all__ = ["WireToProto", "ProtoToWire"]
 
 from typing import Dict, List
 from uuid import UUID
 
-from iscp._encoding.codegen.downstream_pb2 import DownstreamChunk as DownstreamChunkPB
-from iscp._encoding.codegen.downstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.downstream_pb2 import DownstreamChunk as DownstreamChunkPB
+from iscp._encoding._codegen.iscp2.v1.downstream_pb2 import (
     DownstreamChunkAck as DownstreamChunkAckPB,
 )
-from iscp._encoding.codegen.downstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.downstream_pb2 import (
     DownstreamChunkAckComplete as DownstreamChunkAckCompletePB,
 )
-from iscp._encoding.codegen.downstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.downstream_pb2 import (
     DownstreamChunkResult as DownstreamChunkResultPB,
 )
-from iscp._encoding.codegen.downstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.downstream_pb2 import (
     DownstreamCloseRequest as DownstreamCloseRequestPB,
 )
-from iscp._encoding.codegen.downstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.downstream_pb2 import (
     DownstreamCloseResponse as DownstreamCloseResponsePB,
 )
-from iscp._encoding.codegen.downstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.downstream_pb2 import (
     DownstreamMetadata as DownstreamMetadataPB,
 )
-from iscp._encoding.codegen.downstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.downstream_pb2 import (
     DownstreamMetadataAck as DownstreamMetadataAckPB,
 )
-from iscp._encoding.codegen.downstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.downstream_pb2 import (
     DownstreamOpenRequest as DownstreamOpenRequestPB,
 )
-from iscp._encoding.codegen.downstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.downstream_pb2 import (
     DownstreamOpenResponse as DownstreamOpenResponsePB,
 )
-from iscp._encoding.codegen.downstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.downstream_pb2 import (
     DownstreamResumeRequest as DownstreamResumeRequestPB,
 )
-from iscp._encoding.codegen.downstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.downstream_pb2 import (
     DownstreamResumeResponse as DownstreamResumeResponsePB,
 )
-from iscp._encoding.codegen.downstream_pb2 import UpstreamInfo as UpstreamInfoPB
-from iscp._encoding.codegen.extensions.downstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.downstream_pb2 import UpstreamInfo as UpstreamInfoPB
+from iscp._encoding._codegen.iscp2.v1.extensions.downstream_pb2 import (
     DownstreamChunkAckCompleteExtensionFields as DownstreamChunkAckCompleteExtensionFieldsPB,
 )
-from iscp._encoding.codegen.extensions.downstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.extensions.downstream_pb2 import (
     DownstreamChunkAckExtensionFields as DownstreamChunkAckExtensionFieldsPB,
 )
-from iscp._encoding.codegen.extensions.downstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.extensions.downstream_pb2 import (
     DownstreamChunkExtensionFields as DownstreamChunkExtensionFieldsPB,
 )
-from iscp._encoding.codegen.extensions.downstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.extensions.downstream_pb2 import (
     DownstreamChunkResultExtensionFields as DownstreamChunkResultExtensionFieldsPB,
 )
-from iscp._encoding.codegen.extensions.downstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.extensions.downstream_pb2 import (
     DownstreamCloseRequestExtensionFields as DownstreamCloseRequestExtensionFieldsPB,
 )
-from iscp._encoding.codegen.extensions.downstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.extensions.downstream_pb2 import (
     DownstreamCloseResponseExtensionFields as DownstreamCloseResponseExtensionFieldsPB,
 )
-from iscp._encoding.codegen.extensions.downstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.extensions.downstream_pb2 import (
     DownstreamMetadataAckExtensionFields as DownstreamMetadataAckExtensionFieldsPB,
 )
-from iscp._encoding.codegen.extensions.downstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.extensions.downstream_pb2 import (
     DownstreamMetadataExtensionFields as DownstreamMetadataExtensionFieldsPB,
 )
-from iscp._encoding.codegen.extensions.downstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.extensions.downstream_pb2 import (
     DownstreamOpenRequestExtensionFields as DownstreamOpenRequestExtensionFieldsPB,
 )
-from iscp._encoding.codegen.extensions.downstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.extensions.downstream_pb2 import (
     DownstreamOpenResponseExtensionFields as DownstreamOpenResponseExtensionFieldsPB,
 )
-from iscp._encoding.codegen.extensions.downstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.extensions.downstream_pb2 import (
     DownstreamResumeRequestExtensionFields as DownstreamResumeRequestExtensionFieldsPB,
 )
-from iscp._encoding.codegen.extensions.downstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.extensions.downstream_pb2 import (
     DownstreamResumeResponseExtensionFields as DownstreamResumeResponseExtensionFieldsPB,
 )
 from iscp._exceptions import ISCPMalformedMessageError
 from iscp._message import (
     BaseTime,
     DownstreamAbnormalClose,
     DownstreamChunkAck,
@@ -193,14 +193,15 @@
         res.request_id = arg.request_id
         res.desired_stream_id_alias = arg.desired_stream_id_alias
         res.downstream_filters.extend(_common.WireToProto.downstream_filters(arg.downstream_filters))
         res.expiry_interval = arg.expiry_interval
         _common.WireToProto.data_id_aliases(res.data_id_aliases, arg.data_id_aliases)
         res.qos = _common.WireToProto.qos(arg.qos)
         res.extension_fields.CopyFrom(cls.downstream_open_request_extension_fields(arg.extension_fields))
+        res.omit_empty_chunk = arg.omit_empty_chunk
         return res
 
     @classmethod
     def downstream_open_response(cls, arg: DownstreamOpenResponse) -> DownstreamOpenResponsePB:
         res = DownstreamOpenResponsePB()
         res.request_id = arg.request_id
         res.assigned_stream_id = arg.assigned_stream_id.bytes
@@ -448,14 +449,15 @@
             request_id=arg.request_id,
             desired_stream_id_alias=arg.desired_stream_id_alias,
             downstream_filters=_common.ProtoToWire.downstream_filters(arg.downstream_filters),
             expiry_interval=arg.expiry_interval,
             data_id_aliases=_common.ProtoToWire.data_id_aliases(arg.data_id_aliases),
             qos=_common.ProtoToWire.qos(arg.qos),
             extension_fields=cls.downstream_open_request_extension_fields(arg.extension_fields),
+            omit_empty_chunk=arg.omit_empty_chunk,
         )
 
     @classmethod
     def downstream_open_response(cls, arg: DownstreamOpenResponsePB) -> DownstreamOpenResponse:
         return DownstreamOpenResponse(
             request_id=arg.request_id,
             assigned_stream_id=UUID(bytes=arg.assigned_stream_id),
```

## iscp/_encoding/_protobuf/converter/_e2e_call.py

```diff
@@ -1,19 +1,19 @@
 __all__ = ["WireToProto", "ProtoToWire"]
 
-from iscp._encoding.codegen.e2e_call_pb2 import DownstreamCall as DownstreamCallPB
-from iscp._encoding.codegen.e2e_call_pb2 import UpstreamCall as UpstreamCallPB
-from iscp._encoding.codegen.e2e_call_pb2 import UpstreamCallAck as UpstreamCallAckPB
-from iscp._encoding.codegen.extensions.e2e_call_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.e2e_call_pb2 import DownstreamCall as DownstreamCallPB
+from iscp._encoding._codegen.iscp2.v1.e2e_call_pb2 import UpstreamCall as UpstreamCallPB
+from iscp._encoding._codegen.iscp2.v1.e2e_call_pb2 import UpstreamCallAck as UpstreamCallAckPB
+from iscp._encoding._codegen.iscp2.v1.extensions.e2e_call_pb2 import (
     DownstreamCallExtensionFields as DownstreamCallExtensionFieldsPB,
 )
-from iscp._encoding.codegen.extensions.e2e_call_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.extensions.e2e_call_pb2 import (
     UpstreamCallAckExtensionFields as UpstreamCallAckExtensionFieldsPB,
 )
-from iscp._encoding.codegen.extensions.e2e_call_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.extensions.e2e_call_pb2 import (
     UpstreamCallExtensionFields as UpstreamCallExtensionFieldsPB,
 )
 from iscp._message import (
     DownstreamCallExtensionFields,
     UpstreamCall,
     UpstreamCallAck,
     UpstreamCallAckExtensionFields,
```

## iscp/_encoding/_protobuf/converter/_metadata.py

```diff
@@ -1,26 +1,26 @@
 from uuid import UUID
 
-from iscp._encoding.codegen.metadata_pb2 import BaseTime as BaseTimePB
-from iscp._encoding.codegen.metadata_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.metadata_pb2 import BaseTime as BaseTimePB
+from iscp._encoding._codegen.iscp2.v1.metadata_pb2 import (
     DownstreamAbnormalClose as DownstreamAbnormalClosePB,
 )
-from iscp._encoding.codegen.metadata_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.metadata_pb2 import (
     DownstreamNormalClose as DownstreamNormalClosePB,
 )
-from iscp._encoding.codegen.metadata_pb2 import DownstreamOpen as DownstreamOpenPB
-from iscp._encoding.codegen.metadata_pb2 import DownstreamResume as DownstreamResumePB
-from iscp._encoding.codegen.metadata_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.metadata_pb2 import DownstreamOpen as DownstreamOpenPB
+from iscp._encoding._codegen.iscp2.v1.metadata_pb2 import DownstreamResume as DownstreamResumePB
+from iscp._encoding._codegen.iscp2.v1.metadata_pb2 import (
     UpstreamAbnormalClose as UpstreamAbnormalClosePB,
 )
-from iscp._encoding.codegen.metadata_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.metadata_pb2 import (
     UpstreamNormalClose as UpstreamNormalClosePB,
 )
-from iscp._encoding.codegen.metadata_pb2 import UpstreamOpen as UpstreamOpenPB
-from iscp._encoding.codegen.metadata_pb2 import UpstreamResume as UpstreamResumePB
+from iscp._encoding._codegen.iscp2.v1.metadata_pb2 import UpstreamOpen as UpstreamOpenPB
+from iscp._encoding._codegen.iscp2.v1.metadata_pb2 import UpstreamResume as UpstreamResumePB
 from iscp._message import (
     BaseTime,
     DownstreamAbnormalClose,
     DownstreamNormalClose,
     DownstreamOpen,
     DownstreamResume,
     UpstreamAbnormalClose,
```

## iscp/_encoding/_protobuf/converter/_ping_pong.py

```diff
@@ -1,18 +1,18 @@
 __all__ = ["WireToProto", "ProtoToWire"]
 
 
-from iscp._encoding.codegen.extensions.ping_pong_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.extensions.ping_pong_pb2 import (
     PingExtensionFields as PingExtensionFieldsPB,
 )
-from iscp._encoding.codegen.extensions.ping_pong_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.extensions.ping_pong_pb2 import (
     PongExtensionFields as PongExtensionFieldsPB,
 )
-from iscp._encoding.codegen.ping_pong_pb2 import Ping as PingPB
-from iscp._encoding.codegen.ping_pong_pb2 import Pong as PongPB
+from iscp._encoding._codegen.iscp2.v1.ping_pong_pb2 import Ping as PingPB
+from iscp._encoding._codegen.iscp2.v1.ping_pong_pb2 import Pong as PongPB
 from iscp._message import Ping, PingExtensionFields, Pong, PongExtensionFields
 
 
 class WireToProto(object):
     @classmethod
     def ping_extension_fields(cls, _: PingExtensionFields) -> PingExtensionFieldsPB:
         return PingExtensionFieldsPB()
```

## iscp/_encoding/_protobuf/converter/_result_code.py

```diff
@@ -1,8 +1,8 @@
-from iscp._encoding.codegen.result_code_pb2 import ResultCode as ResultCodePB
+from iscp._encoding._codegen.iscp2.v1.result_code_pb2 import ResultCode as ResultCodePB
 from iscp._message import ResultCode
 
 __all__ = ["WireToProto", "ProtoToWire"]
 
 
 class WireToProto(object):
     @classmethod
```

## iscp/_encoding/_protobuf/converter/_upstream.py

```diff
@@ -1,71 +1,71 @@
 __all__ = ["WireToProto", "ProtoToWire"]
 
 
 from typing import List
 from uuid import UUID
 
-from iscp._encoding.codegen.extensions.upstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.extensions.upstream_pb2 import (
     UpstreamChunkAckExtensionFields as UpstreamChunkAckExtensionFieldsPB,
 )
-from iscp._encoding.codegen.extensions.upstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.extensions.upstream_pb2 import (
     UpstreamChunkExtensionFields as UpstreamChunkExtensionFieldsPB,
 )
-from iscp._encoding.codegen.extensions.upstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.extensions.upstream_pb2 import (
     UpstreamChunkResultExtensionFields as UpstreamChunkResultExtensionFieldsPB,
 )
-from iscp._encoding.codegen.extensions.upstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.extensions.upstream_pb2 import (
     UpstreamCloseRequestExtensionFields as UpstreamCloseRequestExtensionFieldsPB,
 )
-from iscp._encoding.codegen.extensions.upstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.extensions.upstream_pb2 import (
     UpstreamCloseResponseExtensionFields as UpstreamCloseResponseExtensionFieldsPB,
 )
-from iscp._encoding.codegen.extensions.upstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.extensions.upstream_pb2 import (
     UpstreamMetadataAckExtensionFields as UpstreamMetadataAckExtensionFieldsPB,
 )
-from iscp._encoding.codegen.extensions.upstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.extensions.upstream_pb2 import (
     UpstreamMetadataExtensionFields as UpstreamMetadataExtensionFieldsPB,
 )
-from iscp._encoding.codegen.extensions.upstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.extensions.upstream_pb2 import (
     UpstreamOpenRequestExtensionFields as UpstreamOpenRequestExtensionFieldsPB,
 )
-from iscp._encoding.codegen.extensions.upstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.extensions.upstream_pb2 import (
     UpstreamOpenResponseExtensionFields as UpstreamOpenResponseExtensionFieldsPB,
 )
-from iscp._encoding.codegen.extensions.upstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.extensions.upstream_pb2 import (
     UpstreamResumeRequestExtensionFields as UpstreamResumeRequestExtensionFieldsPB,
 )
-from iscp._encoding.codegen.extensions.upstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.extensions.upstream_pb2 import (
     UpstreamResumeResponseExtensionFields as UpstreamResumeResponseExtensionFieldsPB,
 )
-from iscp._encoding.codegen.upstream_pb2 import UpstreamChunk as UpstreamChunkPB
-from iscp._encoding.codegen.upstream_pb2 import UpstreamChunkAck as UpstreamChunkAckPB
-from iscp._encoding.codegen.upstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.upstream_pb2 import UpstreamChunk as UpstreamChunkPB
+from iscp._encoding._codegen.iscp2.v1.upstream_pb2 import UpstreamChunkAck as UpstreamChunkAckPB
+from iscp._encoding._codegen.iscp2.v1.upstream_pb2 import (
     UpstreamChunkResult as UpstreamChunkResultPB,
 )
-from iscp._encoding.codegen.upstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.upstream_pb2 import (
     UpstreamCloseRequest as UpstreamCloseRequestPB,
 )
-from iscp._encoding.codegen.upstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.upstream_pb2 import (
     UpstreamCloseResponse as UpstreamCloseResponsePB,
 )
-from iscp._encoding.codegen.upstream_pb2 import UpstreamMetadata as UpstreamMetadataPB
-from iscp._encoding.codegen.upstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.upstream_pb2 import UpstreamMetadata as UpstreamMetadataPB
+from iscp._encoding._codegen.iscp2.v1.upstream_pb2 import (
     UpstreamMetadataAck as UpstreamMetadataAckPB,
 )
-from iscp._encoding.codegen.upstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.upstream_pb2 import (
     UpstreamOpenRequest as UpstreamOpenRequestPB,
 )
-from iscp._encoding.codegen.upstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.upstream_pb2 import (
     UpstreamOpenResponse as UpstreamOpenResponsePB,
 )
-from iscp._encoding.codegen.upstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.upstream_pb2 import (
     UpstreamResumeRequest as UpstreamResumeRequestPB,
 )
-from iscp._encoding.codegen.upstream_pb2 import (
+from iscp._encoding._codegen.iscp2.v1.upstream_pb2 import (
     UpstreamResumeResponse as UpstreamResumeResponsePB,
 )
 from iscp._exceptions import ISCPMalformedMessageError
 from iscp._message import (
     BaseTime,
     Metadata,
     UpstreamChunk,
```

## iscp/_message/_common.py

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass
-from datetime import datetime
+from datetime import datetime, timedelta
 from enum import Enum
 from time import time_ns
 from typing import List, Union
 
 __all__ = [
     "QoS",
     "DataPoint",
@@ -246,7 +246,73 @@
         """
         UNIX時刻（ナノ秒単位）を返却します。
 
         Returns:
             int: UNIX時刻（ナノ秒単位）
         """
         return int(self.datetime.timestamp() * 1_000_000) * 1000 + self.nano_secs
+
+    def isoformat(self, sep="T", timespec="auto") -> str:
+        """
+        UNIX時刻（ナノ秒単位）を返却します。
+
+        Args:
+            sep(str): セパレータ。デフォルトは"T"
+            timespec(str): 仕様。デフォルトは "auto"
+        Returns:
+            str: ISO文字列
+        """
+
+        s = "%04d-%02d-%02d%c" % (self.datetime.year, self.datetime.month, self.datetime.day, sep) + _format_time(
+            self.datetime.hour, self.datetime.minute, self.datetime.second, self.nano_secs, timespec
+        )
+
+        off = self.datetime.utcoffset()
+        tz = _format_offset(off)
+        if tz:
+            s += tz
+
+        return s
+
+
+def _format_time(hh, mm, ss, ns, timespec="auto"):
+    specs = {
+        "hours": "{:02d}",
+        "minutes": "{:02d}:{:02d}",
+        "seconds": "{:02d}:{:02d}:{:02d}",
+        "milliseconds": "{:02d}:{:02d}:{:02d}.{:03d}",
+        "microseconds": "{:02d}:{:02d}:{:02d}.{:06d}",
+        "nanoseconds": "{:02d}:{:02d}:{:02d}.{:09d}",
+    }
+
+    if timespec == "auto":
+        # Skip trailing microseconds when us==0.
+        timespec = "nanoseconds" if ns else "seconds"
+    elif timespec == "milliseconds":
+        ns //= 1000000
+    elif timespec == "microseconds":
+        ns //= 1000
+    try:
+        fmt = specs[timespec]
+    except KeyError:
+        raise ValueError("Unknown timespec value")
+    else:
+        return fmt.format(hh, mm, ss, ns)
+
+
+def _format_offset(off):
+    s = ""
+    if off is not None:
+        if off.days < 0:
+            sign = "-"
+            off = -off
+        else:
+            sign = "+"
+        hh, mm = divmod(off, timedelta(hours=1))
+        mm, ss = divmod(mm, timedelta(minutes=1))
+        s += "%s%02d:%02d" % (sign, hh, mm)
+        if ss or ss.microseconds:
+            s += ":%02d" % ss.seconds
+
+            if ss.microseconds:
+                s += ".%06d" % ss.microseconds
+    return s
```

## iscp/_message/_connection.py

```diff
@@ -1,8 +1,8 @@
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import Optional
 from uuid import UUID
 
 from ._message import Message, RequestMessage
 from ._result_code import ResultCode
 
 __all__ = [
@@ -35,32 +35,34 @@
 @dataclass
 class ConnectRequest(Message):
     request_id: int  # リクエストID
     node_id: str  # ノードID
     protocol_version: str  # プロトコルバージョン
     ping_interval: float  # Ping間隔秒数
     ping_timeout: float  # Pingタイムアウト秒数
-    extension_fields: ConnectRequestExtensionFields = ConnectRequestExtensionFields(
-        access_token="",
-        intdash=IntdashExtensionFields(project_uuid=UUID("00000000-0000-0000-0000-000000000000")),
+    extension_fields: ConnectRequestExtensionFields = field(
+        default_factory=lambda: ConnectRequestExtensionFields(
+            access_token="",
+            intdash=IntdashExtensionFields(project_uuid=UUID("00000000-0000-0000-0000-000000000000")),
+        )
     )  # 拡張フィールド
 
 
 @dataclass
 class ConnectResponse(RequestMessage):
     request_id: int  # リクエストID
     protocol_version: str  # プロトコルバージョン
     result_code: ResultCode  # 結果コード
     result_string: str  # 結果文字列
-    extension_fields: ConnectResponseExtensionFields = ConnectResponseExtensionFields()  # 拡張フィールド
+    extension_fields: ConnectResponseExtensionFields = field(default_factory=lambda: ConnectResponseExtensionFields())  # 拡張フィールド
 
 
 @dataclass
 class DisconnectExtensionFields(Message):
     pass
 
 
 @dataclass
 class Disconnect(Message):
     result_code: ResultCode  # 結果コード
     result_string: str  # 結果文字列
-    extension_fields: DisconnectExtensionFields = DisconnectExtensionFields()  # 拡張フィールド
+    extension_fields: DisconnectExtensionFields = field(default_factory=lambda: DisconnectExtensionFields())  # 拡張フィールド
```

## iscp/_message/_downstream.py

```diff
@@ -125,14 +125,15 @@
 class DownstreamOpenRequest(RequestMessage):
     desired_stream_id_alias: int
     downstream_filters: List[DownstreamFilter]
     expiry_interval: float
     data_id_aliases: Dict[int, DataID]
     qos: QoS
     extension_fields: DownstreamOpenRequestExtensionFields
+    omit_empty_chunk: bool
 
 
 @dataclass
 class DownstreamOpenResponse(RequestMessage):
     assigned_stream_id: UUID
     server_time: DateTime
     result_code: ResultCode
```

## iscp/_sequence.py

```diff
@@ -2,35 +2,35 @@
 
 from . import _exceptions
 
 
 class Sequence(object):
     @classmethod
     def for_request_id(cls):
-        return cls(initial=0, max_value=2 ^ 32, delta=2)
+        return cls(initial=0, max_value=2**32, delta=2)
 
     @classmethod
     def for_stream_id(cls):
-        return cls(initial=1, max_value=2 ^ 32, delta=1)
+        return cls(initial=1, max_value=2**32, delta=1)
 
     @classmethod
     def for_sequence_number(cls):
-        return cls(initial=1, max_value=2 ^ 32, delta=1, is_cyclic=False)
+        return cls(initial=1, max_value=2**32, delta=1, is_cyclic=False)
 
     @classmethod
     def for_ack_id(cls):
-        return cls(initial=1, max_value=2 ^ 32, delta=1)
+        return cls(initial=1, max_value=2**32, delta=1)
 
     @classmethod
     def for_data_id_alias(cls):
-        return cls(initial=1, max_value=2 ^ 32, delta=1)
+        return cls(initial=1, max_value=2**32, delta=1)
 
     @classmethod
     def for_upstream_info_alias(cls):
-        return cls(initial=1, max_value=2 ^ 32, delta=1)
+        return cls(initial=1, max_value=2**32, delta=1)
 
     def __init__(self, initial: int, max_value: int, delta: int, is_cyclic=True):
         self._next = initial
         self._current: Optional[int] = None
         self._max_value = max_value
         self._delta = delta
         self._is_cyclic = is_cyclic
```

## iscp/_transport/_quic.py

```diff
@@ -16,15 +16,15 @@
 from .. import _exceptions as exceptions
 from .._sequence import Sequence
 from ._negotiation_params import NegotiationParams
 from ._transport import Connector, Reader, Transport, TransportName, Unreliable, Writer
 
 __all__ = ["Quic", "QuicConnector", "_MAX_PAYLOAD_SIZE", "_MAX_PAYLOAD_SIZE"]
 
-_MAX_DATAGRAM_FRAME_SIZE = 1200
+_MAX_DATAGRAM_FRAME_SIZE = 1170
 _MAX_PAYLOAD_SIZE = _MAX_DATAGRAM_FRAME_SIZE - 8
 _READ_BUFFER_EXPIRY = 1.0
 
 _ReadWriteMessage = collections.namedtuple("ReceivedMessage", ["seq_num", "seg_idx", "max_idx", "payload"])
 
 
 @dataclass
@@ -130,15 +130,14 @@
             seq_num=int.from_bytes(rd.read(4), "big", signed=False),
             max_idx=int.from_bytes(rd.read(2), "big", signed=False),
             seg_idx=int.from_bytes(rd.read(2), "big", signed=False),
             payload=rd.read(),
         )
 
     async def _negotiate(self, negotiation_params: NegotiationParams):
-
         negotiation_stream_id = self._quic.get_next_available_stream_id(is_unidirectional=True)
         self._quic.send_stream_data(negotiation_stream_id, negotiation_params.encode_to_binary(), end_stream=True)
 
         self._send_stream_id = self._quic.get_next_available_stream_id(is_unidirectional=True)
 
     def quic_event_received(self, event: QuicEvent):
         if isinstance(event, events.ConnectionTerminated):
@@ -155,15 +154,14 @@
 
     def __init__(
         self,
         address: str,
         negotiation_params=NegotiationParams(),
         insecure: bool = False,
     ):
-
         self._address = address
         self._negotiation_params = negotiation_params
         self._insecure = insecure
 
         # Event
         self._connected = asyncio.Event()
         self._called_close_event = asyncio.Event()
```

## iscp/_upstream.py

```diff
@@ -93,15 +93,14 @@
         flush_policy: FlushPolicy,
         persist: bool,
         receive_ack_callback: Optional[AfterReceiveAckCallback] = None,
         send_data_point_callback: Optional[BeforeSendDataPointsCallback] = None,
         closed_event_handler: Optional[UpstreamClosedEventHandler] = None,
         close_session: bool = False,
     ):
-
         self._flush_policy = flush_policy
         self._close_timeout = close_timeout
         self._persist = persist
         self._close_session = close_session
 
         # From Upstream Open Request
         self._session_id = session_id
@@ -127,17 +126,19 @@
         self._sequence_number_sequence = Sequence.for_sequence_number()
 
         # Callback
         self._send_data_point_callback = send_data_point_callback if send_data_point_callback is not None else lambda a, b: None
         self._receive_ack_callback = receive_ack_callback if receive_ack_callback is not None else lambda a, b: None
 
         # Internal Event
-        self._is_draining = asyncio.Event()
+        self._started_draining = asyncio.Event()
         self._received_all_ack = asyncio.Event()
-        self._is_closed = asyncio.Event()
+        self._closed = asyncio.Event()
+        self._finished_flush_buffer_size_loop = asyncio.Event()
+        self._finished_flush_interval_loop = asyncio.Event()
         self._closed_event_handler = closed_event_handler
 
         # Internal Queue
         self._ack_queue: asyncio.Queue[message.UpstreamChunkAck] = asyncio.Queue()
         self._receive_ack_callback_queue: asyncio.Queue[_model.UpstreamChunkAck] = asyncio.Queue()
         self._send_data_point_callback_queue: asyncio.Queue[_model.UpstreamChunk] = asyncio.Queue()
 
@@ -275,15 +276,15 @@
         self._all_loops.append(asyncio.create_task(self._flush_buffer_size_loop()))
         self._all_loops.append(asyncio.create_task(self._receive_ack_hook_loop()))
         self._all_loops.append(asyncio.create_task(self._send_data_point_hook_loop()))
         asyncio.create_task(self._wait_closed_for_event_handler())
         return self
 
     async def _wait_closed_for_event_handler(self):
-        await self._is_closed.wait()
+        await self._closed.wait()
         if self._closed_event_handler:
             self._closed_event_handler(
                 UpstreamClosedEvent(
                     state=self.state,
                     error=self._internal_error,
                 )
             )
@@ -293,23 +294,23 @@
         while True:
             msg = await self._receive_ack_callback_queue.get()
             self._receive_ack_callback(self._id, msg)
             self._receive_ack_callback_queue.task_done()
 
     async def _send_data_point_hook_loop(self):
         logger.debug("start send_data_point_hook_loop")
-        while not self._is_draining.is_set():
+        while not self._started_draining.is_set():
             msg = await self._send_data_point_callback_queue.get()
             self._send_data_point_callback(self._id, msg)
             self._send_data_point_callback_queue.task_done()
 
     async def _ack_loop(self):
         try:
             while True:
-                async with _event_or_coro(self._ack_queue.get(), self._is_draining, self._is_closed) as (done, pending):
+                async with _event_or_coro(self._ack_queue.get(), self._closed) as (done, pending):
                     for result in done:
                         ack = await result
                         if isinstance(ack, message.UpstreamChunkAck):
                             self._data_id_aliases.update(ack.data_id_aliases)
                             await self._receive_ack_callback_queue.put(
                                 _model.UpstreamChunkAck(
                                     results=[
@@ -322,52 +323,59 @@
                                     ]
                                 )
                             )
                             self._update_data_id_alias(ack.data_id_aliases)
                             for n in [n.sequence_number for n in ack.results]:
                                 self._waiting_sequence_numbers.remove(n)
                             self._ack_queue.task_done()
+                            if self._finished_flush_buffer_size_loop.is_set() and self._finished_flush_interval_loop.is_set():
+                                if len(self._waiting_sequence_numbers) == 0:
+                                    self._received_all_ack.set()
+                                    return
                         else:
-                            # called_close_event
-                            if len(self._waiting_sequence_numbers) == 0:
-                                self._received_all_ack.set()
-                                return
+                            return
 
         except Exception as e:
             logger.error(e)
 
     def _update_data_id_alias(self, arg: Dict[int, message.DataID]):
         self._data_id_aliases.update(arg)
         self._rev_data_id_aliases = {v: k for k, v in self._data_id_aliases.items()}
 
     async def _flush_buffer_size_loop(self):
-        while True:
-            async with self._send_buffer_condition:
-                if self._is_closed.is_set():
-                    return
-                if self._is_draining.is_set() or self._flush_policy.IsFlush(self._send_buffer_size):
-                    await self._flush()
-                if self._is_draining.is_set():
-                    return
-                await self._send_buffer_condition.wait()
+        try:
+            while True:
+                async with self._send_buffer_condition:
+                    if self._closed.is_set():
+                        return
+                    if self._started_draining.is_set() or self._flush_policy.IsFlush(self._send_buffer_size):
+                        await self._flush()
+                    if self._started_draining.is_set():
+                        return
+                    await self._send_buffer_condition.wait()
+        finally:
+            self._finished_flush_buffer_size_loop.set()
 
     async def _flush_interval_loop(self):
-        tick = self._flush_policy.Ticker()
-        if not tick:
-            return
         try:
-
+            tick = self._flush_policy.Ticker()
+            if not tick:
+                return
             async for _ in tick():
                 async with self._send_buffer_condition:
-                    if self._is_draining.is_set() and not self._send_buffer:
+                    if self._started_draining.is_set() and not self._send_buffer:
                         return
                     await self._flush()
+                    if self._started_draining.is_set():
+                        return
                     await self._send_buffer_condition.wait()
         finally:
-            tick.stop()
+            if tick:
+                tick.stop()
+            self._finished_flush_interval_loop.set()
 
     async def flush(self):
         """
         データポイントの内部バッファをUpstreamChunkとしてサーバーへ送信します。
         """
         await self._flush()
 
@@ -410,15 +418,15 @@
                 )
             )
             await self._sender(chunk)
             self._send_buffer = defaultdict(lambda: [])
             self._send_buffer_size = 0
         except exceptions.ISCPException as e:
             self._internal_error = e
-            self._is_closed.set()
+            self._closed.set()
             for t in self._all_loops:
                 t.cancel()
 
             await asyncio.wait(self._all_loops)
 
             resp = await self._requester(
                 message.UpstreamCloseRequest(
@@ -445,55 +453,60 @@
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         with contextlib.suppress(exceptions.ISCPException):
             await self.close()
 
-    async def write_data_point(self, data_id: message.DataID, *data_points: message.DataPoint):
+    async def write_data_points(self, data_id: message.DataID, *data_points: message.DataPoint):
         """
         データポイントを送信します。
 
         Args:
             data_id(iscp.DataID): データID
             *data_points(iscp.DataPoint): データポイント
         """
 
-        if self._is_draining.is_set():
+        if self._started_draining.is_set():
             raise exceptions.ISCPTransportClosedError()
 
         async with self._send_buffer_condition:
-
             self._send_buffer[data_id].extend(data_points)
             self._send_buffer_size += sum([len(v.payload) for v in data_points])
             self._send_buffer_condition.notify_all()
 
     async def _handle_ack(self, msg: message.UpstreamChunkAck):
         await self._ack_queue.put(msg)
 
     async def close(self, overwrite_close_session: Optional[bool] = None):
         """
         アップストリームを閉じます。
 
         Args:
             overwrite_close_session(Optional[bool]): アップストリームに設定されている `close_session` を上書きします。
         """
-        if self._is_closed.is_set():
+        if self._closed.is_set():
             return
-        if self._is_draining.is_set():
+        if self._started_draining.is_set():
             raise exceptions.ISCPException("already draining")
 
-        self._is_draining.set()
+        self._started_draining.set()
 
         try:
-            while self._send_buffer:
+            while (
+                self._send_buffer
+                or not self._finished_flush_buffer_size_loop.is_set()
+                or not self._finished_flush_interval_loop.is_set()
+            ):
                 async with self._send_buffer_condition:
                     self._send_buffer_condition.notify_all()
                     await asyncio.sleep(0)
-            await asyncio.wait_for(self._received_all_ack.wait(), timeout=self._close_timeout)
+
+            if len(self._waiting_sequence_numbers) != 0:
+                await asyncio.wait_for(self._received_all_ack.wait(), timeout=self._close_timeout)
         except asyncio.TimeoutError as e:
             logger.warning(e)
 
         try:
             for t in self._all_loops:
                 t.cancel()
 
@@ -516,15 +529,15 @@
                 logger.error(
                     f"failed to close a upstream. stream_id \
                             [{self._id}] code=[{resp.result_code}] msg=[{resp.result_string}]",
                 )
                 return
             raise exceptions.ISCPFailedMessageError(received_message=resp)
         finally:
-            self._is_closed.set()
+            self._closed.set()
 
 
 @contextlib.asynccontextmanager
 async def _event_or_coro(aw: Coroutine, *evs: asyncio.Event):
     ts = [asyncio.create_task(ev.wait()) for ev in evs]
     ts.append(asyncio.create_task(aw))
     try:
```

## iscp/_utils.py

```diff
@@ -1,10 +1,25 @@
 import asyncio
+import logging
 from contextlib import suppress
 
+logger = logging.getLogger(__name__)
+
 
 def drain(q: asyncio.Queue):
     with suppress(asyncio.QueueEmpty):
         # drain
         while True:
             q.get_nowait()
             q.task_done()
+
+
+def enqueue(queue: asyncio.Queue, msg):
+    while True:
+        try:
+            queue.put_nowait(msg)
+            return
+        except asyncio.QueueFull:
+            # discard
+            logger.warning(f"discard msg:{msg}")
+            with suppress(asyncio.QueueEmpty):
+                queue.get_nowait()
```

## Comparing `iscp/_encoding/codegen/connection_pb2.py` & `iscp/_encoding/_codegen/iscp2/v1/e2e_call_pb2.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: connection.proto
+# source: iscp2/v1/e2e_call.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from . import result_code_pb2 as result__code__pb2
-from .extensions import connection_pb2 as extensions_dot_connection__pb2
+from .extensions import e2e_call_pb2 as iscp2_dot_v1_dot_extensions_dot_e2e__call__pb2
+from . import result_code_pb2 as iscp2_dot_v1_dot_result__code__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x63onnection.proto\x12\x05iscp2\x1a\x11result_code.proto\x1a\x1b\x65xtensions/connection.proto\"\xbc\x01\n\x0e\x43onnectRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\r\x12\x18\n\x10protocol_version\x18\x02 \x01(\t\x12\x0f\n\x07node_id\x18\x03 \x01(\t\x12\x15\n\rping_interval\x18\x04 \x01(\r\x12\x14\n\x0cping_timeout\x18\x05 \x01(\r\x12>\n\x10\x65xtension_fields\x18\x06 \x01(\x0b\x32$.iscp2.ConnectRequestExtensionFields\"\xbf\x01\n\x0f\x43onnectResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\r\x12\x18\n\x10protocol_version\x18\x02 \x01(\t\x12&\n\x0bresult_code\x18\x03 \x01(\x0e\x32\x11.iscp2.ResultCode\x12\x15\n\rresult_string\x18\x04 \x01(\t\x12?\n\x10\x65xtension_fields\x18\x05 \x01(\x0b\x32%.iscp2.ConnectResponseExtensionFields\"\x87\x01\n\nDisconnect\x12&\n\x0bresult_code\x18\x01 \x01(\x0e\x32\x11.iscp2.ResultCode\x12\x15\n\rresult_string\x18\x02 \x01(\t\x12:\n\x10\x65xtension_fields\x18\x03 \x01(\x0b\x32 .iscp2.DisconnectExtensionFieldsb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17iscp2/v1/e2e_call.proto\x12\x08iscp2.v1\x1a\"iscp2/v1/extensions/e2e_call.proto\x1a\x1aiscp2/v1/result_code.proto\"\x9e\x02\n\x0cUpstreamCall\x12\x17\n\x07\x63\x61ll_id\x18\x01 \x01(\tR\x06\x63\x61llId\x12&\n\x0frequest_call_id\x18\x02 \x01(\tR\rrequestCallId\x12.\n\x13\x64\x65stination_node_id\x18\x03 \x01(\tR\x11\x64\x65stinationNodeId\x12\x12\n\x04name\x18\x04 \x01(\tR\x04name\x12\x12\n\x04type\x18\x05 \x01(\tR\x04type\x12\x18\n\x07payload\x18\x06 \x01(\x0cR\x07payload\x12[\n\x10\x65xtension_fields\x18\x07 \x01(\x0b\x32\x30.iscp2.v1.extensions.UpstreamCallExtensionFieldsR\x0f\x65xtensionFields\"\xe6\x01\n\x0fUpstreamCallAck\x12\x17\n\x07\x63\x61ll_id\x18\x01 \x01(\tR\x06\x63\x61llId\x12\x35\n\x0bresult_code\x18\x02 \x01(\x0e\x32\x14.iscp2.v1.ResultCodeR\nresultCode\x12#\n\rresult_string\x18\x03 \x01(\tR\x0cresultString\x12^\n\x10\x65xtension_fields\x18\x04 \x01(\x0b\x32\x33.iscp2.v1.extensions.UpstreamCallAckExtensionFieldsR\x0f\x65xtensionFields\"\x98\x02\n\x0e\x44ownstreamCall\x12\x17\n\x07\x63\x61ll_id\x18\x01 \x01(\tR\x06\x63\x61llId\x12&\n\x0frequest_call_id\x18\x02 \x01(\tR\rrequestCallId\x12$\n\x0esource_node_id\x18\x03 \x01(\tR\x0csourceNodeId\x12\x12\n\x04name\x18\x04 \x01(\tR\x04name\x12\x12\n\x04type\x18\x05 \x01(\tR\x04type\x12\x18\n\x07payload\x18\x06 \x01(\x0cR\x07payload\x12]\n\x10\x65xtension_fields\x18\x07 \x01(\x0b\x32\x32.iscp2.v1.extensions.DownstreamCallExtensionFieldsR\x0f\x65xtensionFieldsB]\n\x0c\x63om.iscp2.v1B\x0c\x45\x32\x65\x43\x61llProtoP\x01\xa2\x02\x03IXX\xaa\x02\x08Iscp2.V1\xca\x02\x08Iscp2\\V1\xe2\x02\x14Iscp2\\V1\\GPBMetadata\xea\x02\tIscp2::V1b\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'connection_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'iscp2.v1.e2e_call_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _CONNECTREQUEST._serialized_start=76
-  _CONNECTREQUEST._serialized_end=264
-  _CONNECTRESPONSE._serialized_start=267
-  _CONNECTRESPONSE._serialized_end=458
-  _DISCONNECT._serialized_start=461
-  _DISCONNECT._serialized_end=596
+  DESCRIPTOR._serialized_options = b'\n\014com.iscp2.v1B\014E2eCallProtoP\001\242\002\003IXX\252\002\010Iscp2.V1\312\002\010Iscp2\\V1\342\002\024Iscp2\\V1\\GPBMetadata\352\002\tIscp2::V1'
+  _globals['_UPSTREAMCALL']._serialized_start=102
+  _globals['_UPSTREAMCALL']._serialized_end=388
+  _globals['_UPSTREAMCALLACK']._serialized_start=391
+  _globals['_UPSTREAMCALLACK']._serialized_end=621
+  _globals['_DOWNSTREAMCALL']._serialized_start=624
+  _globals['_DOWNSTREAMCALL']._serialized_end=904
 # @@protoc_insertion_point(module_scope)
```

## Comparing `iscp/_encoding/codegen/downstream_pb2.py` & `iscp/_encoding/_codegen/iscp2/v1/upstream_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,59 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: downstream.proto
+# source: iscp2/v1/upstream.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from . import common_pb2 as common__pb2
-from . import metadata_pb2 as metadata__pb2
-from . import result_code_pb2 as result__code__pb2
-from .extensions import downstream_pb2 as extensions_dot_downstream__pb2
+from . import common_pb2 as iscp2_dot_v1_dot_common__pb2
+from .extensions import upstream_pb2 as iscp2_dot_v1_dot_extensions_dot_upstream__pb2
+from . import metadata_pb2 as iscp2_dot_v1_dot_metadata__pb2
+from . import result_code_pb2 as iscp2_dot_v1_dot_result__code__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x64ownstream.proto\x12\x05iscp2\x1a\x0c\x63ommon.proto\x1a\x0emetadata.proto\x1a\x11result_code.proto\x1a\x1b\x65xtensions/downstream.proto\"\x89\x03\n\x15\x44ownstreamOpenRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\r\x12\x1f\n\x17\x64\x65sired_stream_id_alias\x18\x02 \x01(\r\x12\x33\n\x12\x64ownstream_filters\x18\x03 \x03(\x0b\x32\x17.iscp2.DownstreamFilter\x12\x17\n\x0f\x65xpiry_interval\x18\x04 \x01(\r\x12H\n\x0f\x64\x61ta_id_aliases\x18\x05 \x03(\x0b\x32/.iscp2.DownstreamOpenRequest.DataIdAliasesEntry\x12\x17\n\x03qos\x18\x06 \x01(\x0e\x32\n.iscp2.QoS\x12\x45\n\x10\x65xtension_fields\x18\x07 \x01(\x0b\x32+.iscp2.DownstreamOpenRequestExtensionFields\x1a\x43\n\x12\x44\x61taIdAliasesEntry\x12\x0b\n\x03key\x18\x01 \x01(\r\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.iscp2.DataID:\x02\x38\x01\"\xe4\x01\n\x16\x44ownstreamOpenResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\r\x12\x1a\n\x12\x61ssigned_stream_id\x18\x02 \x01(\x0c\x12\x13\n\x0bserver_time\x18\x03 \x01(\x12\x12&\n\x0bresult_code\x18\x04 \x01(\x0e\x32\x11.iscp2.ResultCode\x12\x15\n\rresult_string\x18\x05 \x01(\t\x12\x46\n\x10\x65xtension_fields\x18\x06 \x01(\x0b\x32,.iscp2.DownstreamOpenResponseExtensionFields\"\xaa\x01\n\x17\x44ownstreamResumeRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\r\x12\x11\n\tstream_id\x18\x02 \x01(\x0c\x12\x1f\n\x17\x64\x65sired_stream_id_alias\x18\x03 \x01(\r\x12G\n\x10\x65xtension_fields\x18\x04 \x01(\x0b\x32-.iscp2.DownstreamResumeRequestExtensionFields\"\xb7\x01\n\x18\x44ownstreamResumeResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\r\x12&\n\x0bresult_code\x18\x02 \x01(\x0e\x32\x11.iscp2.ResultCode\x12\x15\n\rresult_string\x18\x03 \x01(\t\x12H\n\x10\x65xtension_fields\x18\x04 \x01(\x0b\x32..iscp2.DownstreamResumeResponseExtensionFields\"\x87\x01\n\x16\x44ownstreamCloseRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\r\x12\x11\n\tstream_id\x18\x02 \x01(\x0c\x12\x46\n\x10\x65xtension_fields\x18\x03 \x01(\x0b\x32,.iscp2.DownstreamCloseRequestExtensionFields\"\xb5\x01\n\x17\x44ownstreamCloseResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\r\x12&\n\x0bresult_code\x18\x02 \x01(\x0e\x32\x11.iscp2.ResultCode\x12\x15\n\rresult_string\x18\x03 \x01(\t\x12G\n\x10\x65xtension_fields\x18\x04 \x01(\x0b\x32-.iscp2.DownstreamCloseResponseExtensionFields\"\xf2\x01\n\x0f\x44ownstreamChunk\x12\x17\n\x0fstream_id_alias\x18\x01 \x01(\r\x12,\n\rupstream_info\x18\x02 \x01(\x0b\x32\x13.iscp2.UpstreamInfoH\x00\x12\x18\n\x0eupstream_alias\x18\x03 \x01(\rH\x00\x12(\n\x0cstream_chunk\x18\x04 \x01(\x0b\x32\x12.iscp2.StreamChunk\x12?\n\x10\x65xtension_fields\x18\x05 \x01(\x0b\x32%.iscp2.DownstreamChunkExtensionFieldsB\x13\n\x11upstream_or_alias\"\xd3\x03\n\x12\x44ownstreamChunkAck\x12\x17\n\x0fstream_id_alias\x18\x01 \x01(\r\x12\x0e\n\x06\x61\x63k_id\x18\x02 \x01(\r\x12-\n\x07results\x18\x03 \x03(\x0b\x32\x1c.iscp2.DownstreamChunkResult\x12H\n\x10upstream_aliases\x18\x04 \x03(\x0b\x32..iscp2.DownstreamChunkAck.UpstreamAliasesEntry\x12\x45\n\x0f\x64\x61ta_id_aliases\x18\x05 \x03(\x0b\x32,.iscp2.DownstreamChunkAck.DataIdAliasesEntry\x12\x42\n\x10\x65xtension_fields\x18\x06 \x01(\x0b\x32(.iscp2.DownstreamChunkAckExtensionFields\x1aK\n\x14UpstreamAliasesEntry\x12\x0b\n\x03key\x18\x01 \x01(\r\x12\"\n\x05value\x18\x02 \x01(\x0b\x32\x13.iscp2.UpstreamInfo:\x02\x38\x01\x1a\x43\n\x12\x44\x61taIdAliasesEntry\x12\x0b\n\x03key\x18\x01 \x01(\r\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.iscp2.DataID:\x02\x38\x01\"\xd0\x01\n\x1a\x44ownstreamChunkAckComplete\x12\x17\n\x0fstream_id_alias\x18\x01 \x01(\r\x12\x0e\n\x06\x61\x63k_id\x18\x02 \x01(\r\x12&\n\x0bresult_code\x18\x03 \x01(\x0e\x32\x11.iscp2.ResultCode\x12\x15\n\rresult_string\x18\x04 \x01(\t\x12J\n\x10\x65xtension_fields\x18\x05 \x01(\x0b\x32\x30.iscp2.DownstreamChunkAckCompleteExtensionFields\"\x9b\x05\n\x12\x44ownstreamMetadata\x12\x12\n\nrequest_id\x18\x01 \x01(\r\x12\x17\n\x0fstream_id_alias\x18\r \x01(\r\x12$\n\tbase_time\x18\x02 \x01(\x0b\x32\x0f.iscp2.BaseTimeH\x00\x12,\n\rupstream_open\x18\x03 \x01(\x0b\x32\x13.iscp2.UpstreamOpenH\x00\x12?\n\x17upstream_abnormal_close\x18\x04 \x01(\x0b\x32\x1c.iscp2.UpstreamAbnormalCloseH\x00\x12\x30\n\x0fupstream_resume\x18\x05 \x01(\x0b\x32\x15.iscp2.UpstreamResumeH\x00\x12;\n\x15upstream_normal_close\x18\x06 \x01(\x0b\x32\x1a.iscp2.UpstreamNormalCloseH\x00\x12\x30\n\x0f\x64ownstream_open\x18\x07 \x01(\x0b\x32\x15.iscp2.DownstreamOpenH\x00\x12\x43\n\x19\x64ownstream_abnormal_close\x18\x08 \x01(\x0b\x32\x1e.iscp2.DownstreamAbnormalCloseH\x00\x12\x34\n\x11\x64ownstream_resume\x18\t \x01(\x0b\x32\x17.iscp2.DownstreamResumeH\x00\x12?\n\x17\x64ownstream_normal_close\x18\n \x01(\x0b\x32\x1c.iscp2.DownstreamNormalCloseH\x00\x12\x16\n\x0esource_node_id\x18\x0b \x01(\t\x12\x42\n\x10\x65xtension_fields\x18\x0c \x01(\x0b\x32(.iscp2.DownstreamMetadataExtensionFieldsB\n\n\x08metadata\"\xb1\x01\n\x15\x44ownstreamMetadataAck\x12\x12\n\nrequest_id\x18\x01 \x01(\r\x12&\n\x0bresult_code\x18\x02 \x01(\x0e\x32\x11.iscp2.ResultCode\x12\x15\n\rresult_string\x18\x03 \x01(\t\x12\x45\n\x10\x65xtension_fields\x18\x04 \x01(\x0b\x32+.iscp2.DownstreamMetadataAckExtensionFields\"M\n\x0cUpstreamInfo\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x11\n\tstream_id\x18\x02 \x01(\x0c\x12\x16\n\x0esource_node_id\x18\x03 \x01(\t\"\xe1\x01\n\x15\x44ownstreamChunkResult\x12\x1d\n\x15stream_id_of_upstream\x18\x01 \x01(\x0c\x12#\n\x1bsequence_number_in_upstream\x18\x02 \x01(\r\x12&\n\x0bresult_code\x18\x03 \x01(\x0e\x32\x11.iscp2.ResultCode\x12\x15\n\rresult_string\x18\x04 \x01(\t\x12\x45\n\x10\x65xtension_fields\x18\x05 \x01(\x0b\x32+.iscp2.DownstreamChunkResultExtensionFieldsb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17iscp2/v1/upstream.proto\x12\x08iscp2.v1\x1a\x15iscp2/v1/common.proto\x1a\"iscp2/v1/extensions/upstream.proto\x1a\x17iscp2/v1/metadata.proto\x1a\x1aiscp2/v1/result_code.proto\"\xd1\x02\n\x13UpstreamOpenRequest\x12\x1d\n\nrequest_id\x18\x01 \x01(\rR\trequestId\x12\x1d\n\nsession_id\x18\x02 \x01(\tR\tsessionId\x12!\n\x0c\x61\x63k_interval\x18\x03 \x01(\rR\x0b\x61\x63kInterval\x12\'\n\x0f\x65xpiry_interval\x18\x05 \x01(\rR\x0e\x65xpiryInterval\x12+\n\x08\x64\x61ta_ids\x18\x06 \x03(\x0b\x32\x10.iscp2.v1.DataIDR\x07\x64\x61taIds\x12\x1f\n\x03qos\x18\x07 \x01(\x0e\x32\r.iscp2.v1.QoSR\x03qos\x12\x62\n\x10\x65xtension_fields\x18\x08 \x01(\x0b\x32\x37.iscp2.v1.extensions.UpstreamOpenRequestExtensionFieldsR\x0f\x65xtensionFields\"\xad\x04\n\x14UpstreamOpenResponse\x12\x1d\n\nrequest_id\x18\x01 \x01(\rR\trequestId\x12,\n\x12\x61ssigned_stream_id\x18\x02 \x01(\x0cR\x10\x61ssignedStreamId\x12\x37\n\x18\x61ssigned_stream_id_alias\x18\x03 \x01(\rR\x15\x61ssignedStreamIdAlias\x12Y\n\x0f\x64\x61ta_id_aliases\x18\x04 \x03(\x0b\x32\x31.iscp2.v1.UpstreamOpenResponse.DataIdAliasesEntryR\rdataIdAliases\x12\x1f\n\x0bserver_time\x18\x05 \x01(\x12R\nserverTime\x12\x35\n\x0bresult_code\x18\x06 \x01(\x0e\x32\x14.iscp2.v1.ResultCodeR\nresultCode\x12#\n\rresult_string\x18\x07 \x01(\tR\x0cresultString\x12\x63\n\x10\x65xtension_fields\x18\x08 \x01(\x0b\x32\x38.iscp2.v1.extensions.UpstreamOpenResponseExtensionFieldsR\x0f\x65xtensionFields\x1aR\n\x12\x44\x61taIdAliasesEntry\x12\x10\n\x03key\x18\x01 \x01(\rR\x03key\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x10.iscp2.v1.DataIDR\x05value:\x02\x38\x01\"\xb9\x01\n\x15UpstreamResumeRequest\x12\x1d\n\nrequest_id\x18\x01 \x01(\rR\trequestId\x12\x1b\n\tstream_id\x18\x02 \x01(\x0cR\x08streamId\x12\x64\n\x10\x65xtension_fields\x18\x03 \x01(\x0b\x32\x39.iscp2.v1.extensions.UpstreamResumeRequestExtensionFieldsR\x0f\x65xtensionFields\"\xb3\x02\n\x16UpstreamResumeResponse\x12\x1d\n\nrequest_id\x18\x01 \x01(\rR\trequestId\x12\x37\n\x18\x61ssigned_stream_id_alias\x18\x02 \x01(\rR\x15\x61ssignedStreamIdAlias\x12\x35\n\x0bresult_code\x18\x03 \x01(\x0e\x32\x14.iscp2.v1.ResultCodeR\nresultCode\x12#\n\rresult_string\x18\x04 \x01(\tR\x0cresultString\x12\x65\n\x10\x65xtension_fields\x18\x05 \x01(\x0b\x32:.iscp2.v1.extensions.UpstreamResumeResponseExtensionFieldsR\x0f\x65xtensionFields\"\x97\x02\n\x14UpstreamCloseRequest\x12\x1d\n\nrequest_id\x18\x01 \x01(\rR\trequestId\x12\x1b\n\tstream_id\x18\x02 \x01(\x0cR\x08streamId\x12*\n\x11total_data_points\x18\x03 \x01(\x04R\x0ftotalDataPoints\x12\x32\n\x15\x66inal_sequence_number\x18\x04 \x01(\rR\x13\x66inalSequenceNumber\x12\x63\n\x10\x65xtension_fields\x18\x05 \x01(\x0b\x32\x38.iscp2.v1.extensions.UpstreamCloseRequestExtensionFieldsR\x0f\x65xtensionFields\"\xf8\x01\n\x15UpstreamCloseResponse\x12\x1d\n\nrequest_id\x18\x01 \x01(\rR\trequestId\x12\x35\n\x0bresult_code\x18\x02 \x01(\x0e\x32\x14.iscp2.v1.ResultCodeR\nresultCode\x12#\n\rresult_string\x18\x03 \x01(\tR\x0cresultString\x12\x64\n\x10\x65xtension_fields\x18\x04 \x01(\x0b\x32\x39.iscp2.v1.extensions.UpstreamCloseResponseExtensionFieldsR\x0f\x65xtensionFields\"\xfc\x01\n\rUpstreamChunk\x12&\n\x0fstream_id_alias\x18\x01 \x01(\rR\rstreamIdAlias\x12\x38\n\x0cstream_chunk\x18\x02 \x01(\x0b\x32\x15.iscp2.v1.StreamChunkR\x0bstreamChunk\x12+\n\x08\x64\x61ta_ids\x18\x03 \x03(\x0b\x32\x10.iscp2.v1.DataIDR\x07\x64\x61taIds\x12\\\n\x10\x65xtension_fields\x18\x04 \x01(\x0b\x32\x31.iscp2.v1.extensions.UpstreamChunkExtensionFieldsR\x0f\x65xtensionFields\"\xff\x02\n\x10UpstreamChunkAck\x12&\n\x0fstream_id_alias\x18\x01 \x01(\rR\rstreamIdAlias\x12\x37\n\x07results\x18\x02 \x03(\x0b\x32\x1d.iscp2.v1.UpstreamChunkResultR\x07results\x12U\n\x0f\x64\x61ta_id_aliases\x18\x03 \x03(\x0b\x32-.iscp2.v1.UpstreamChunkAck.DataIdAliasesEntryR\rdataIdAliases\x12_\n\x10\x65xtension_fields\x18\x04 \x01(\x0b\x32\x34.iscp2.v1.extensions.UpstreamChunkAckExtensionFieldsR\x0f\x65xtensionFields\x1aR\n\x12\x44\x61taIdAliasesEntry\x12\x10\n\x03key\x18\x01 \x01(\rR\x03key\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x10.iscp2.v1.DataIDR\x05value:\x02\x38\x01\"\xd1\x01\n\x10UpstreamMetadata\x12\x1d\n\nrequest_id\x18\x01 \x01(\rR\trequestId\x12\x31\n\tbase_time\x18\x02 \x01(\x0b\x32\x12.iscp2.v1.BaseTimeH\x00R\x08\x62\x61seTime\x12_\n\x10\x65xtension_fields\x18\x04 \x01(\x0b\x32\x34.iscp2.v1.extensions.UpstreamMetadataExtensionFieldsR\x0f\x65xtensionFieldsB\n\n\x08metadata\"\xf4\x01\n\x13UpstreamMetadataAck\x12\x1d\n\nrequest_id\x18\x01 \x01(\rR\trequestId\x12\x35\n\x0bresult_code\x18\x02 \x01(\x0e\x32\x14.iscp2.v1.ResultCodeR\nresultCode\x12#\n\rresult_string\x18\x03 \x01(\tR\x0cresultString\x12\x62\n\x10\x65xtension_fields\x18\x04 \x01(\x0b\x32\x37.iscp2.v1.extensions.UpstreamMetadataAckExtensionFieldsR\x0f\x65xtensionFields\"\xfe\x01\n\x13UpstreamChunkResult\x12\'\n\x0fsequence_number\x18\x01 \x01(\rR\x0esequenceNumber\x12\x35\n\x0bresult_code\x18\x02 \x01(\x0e\x32\x14.iscp2.v1.ResultCodeR\nresultCode\x12#\n\rresult_string\x18\x03 \x01(\tR\x0cresultString\x12\x62\n\x10\x65xtension_fields\x18\x04 \x01(\x0b\x32\x37.iscp2.v1.extensions.UpstreamChunkResultExtensionFieldsR\x0f\x65xtensionFieldsB^\n\x0c\x63om.iscp2.v1B\rUpstreamProtoP\x01\xa2\x02\x03IXX\xaa\x02\x08Iscp2.V1\xca\x02\x08Iscp2\\V1\xe2\x02\x14Iscp2\\V1\\GPBMetadata\xea\x02\tIscp2::V1b\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'downstream_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'iscp2.v1.upstream_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _DOWNSTREAMOPENREQUEST_DATAIDALIASESENTRY._options = None
-  _DOWNSTREAMOPENREQUEST_DATAIDALIASESENTRY._serialized_options = b'8\001'
-  _DOWNSTREAMCHUNKACK_UPSTREAMALIASESENTRY._options = None
-  _DOWNSTREAMCHUNKACK_UPSTREAMALIASESENTRY._serialized_options = b'8\001'
-  _DOWNSTREAMCHUNKACK_DATAIDALIASESENTRY._options = None
-  _DOWNSTREAMCHUNKACK_DATAIDALIASESENTRY._serialized_options = b'8\001'
-  _DOWNSTREAMOPENREQUEST._serialized_start=106
-  _DOWNSTREAMOPENREQUEST._serialized_end=499
-  _DOWNSTREAMOPENREQUEST_DATAIDALIASESENTRY._serialized_start=432
-  _DOWNSTREAMOPENREQUEST_DATAIDALIASESENTRY._serialized_end=499
-  _DOWNSTREAMOPENRESPONSE._serialized_start=502
-  _DOWNSTREAMOPENRESPONSE._serialized_end=730
-  _DOWNSTREAMRESUMEREQUEST._serialized_start=733
-  _DOWNSTREAMRESUMEREQUEST._serialized_end=903
-  _DOWNSTREAMRESUMERESPONSE._serialized_start=906
-  _DOWNSTREAMRESUMERESPONSE._serialized_end=1089
-  _DOWNSTREAMCLOSEREQUEST._serialized_start=1092
-  _DOWNSTREAMCLOSEREQUEST._serialized_end=1227
-  _DOWNSTREAMCLOSERESPONSE._serialized_start=1230
-  _DOWNSTREAMCLOSERESPONSE._serialized_end=1411
-  _DOWNSTREAMCHUNK._serialized_start=1414
-  _DOWNSTREAMCHUNK._serialized_end=1656
-  _DOWNSTREAMCHUNKACK._serialized_start=1659
-  _DOWNSTREAMCHUNKACK._serialized_end=2126
-  _DOWNSTREAMCHUNKACK_UPSTREAMALIASESENTRY._serialized_start=1982
-  _DOWNSTREAMCHUNKACK_UPSTREAMALIASESENTRY._serialized_end=2057
-  _DOWNSTREAMCHUNKACK_DATAIDALIASESENTRY._serialized_start=432
-  _DOWNSTREAMCHUNKACK_DATAIDALIASESENTRY._serialized_end=499
-  _DOWNSTREAMCHUNKACKCOMPLETE._serialized_start=2129
-  _DOWNSTREAMCHUNKACKCOMPLETE._serialized_end=2337
-  _DOWNSTREAMMETADATA._serialized_start=2340
-  _DOWNSTREAMMETADATA._serialized_end=3007
-  _DOWNSTREAMMETADATAACK._serialized_start=3010
-  _DOWNSTREAMMETADATAACK._serialized_end=3187
-  _UPSTREAMINFO._serialized_start=3189
-  _UPSTREAMINFO._serialized_end=3266
-  _DOWNSTREAMCHUNKRESULT._serialized_start=3269
-  _DOWNSTREAMCHUNKRESULT._serialized_end=3494
+  DESCRIPTOR._serialized_options = b'\n\014com.iscp2.v1B\rUpstreamProtoP\001\242\002\003IXX\252\002\010Iscp2.V1\312\002\010Iscp2\\V1\342\002\024Iscp2\\V1\\GPBMetadata\352\002\tIscp2::V1'
+  _UPSTREAMOPENRESPONSE_DATAIDALIASESENTRY._options = None
+  _UPSTREAMOPENRESPONSE_DATAIDALIASESENTRY._serialized_options = b'8\001'
+  _UPSTREAMCHUNKACK_DATAIDALIASESENTRY._options = None
+  _UPSTREAMCHUNKACK_DATAIDALIASESENTRY._serialized_options = b'8\001'
+  _globals['_UPSTREAMOPENREQUEST']._serialized_start=150
+  _globals['_UPSTREAMOPENREQUEST']._serialized_end=487
+  _globals['_UPSTREAMOPENRESPONSE']._serialized_start=490
+  _globals['_UPSTREAMOPENRESPONSE']._serialized_end=1047
+  _globals['_UPSTREAMOPENRESPONSE_DATAIDALIASESENTRY']._serialized_start=965
+  _globals['_UPSTREAMOPENRESPONSE_DATAIDALIASESENTRY']._serialized_end=1047
+  _globals['_UPSTREAMRESUMEREQUEST']._serialized_start=1050
+  _globals['_UPSTREAMRESUMEREQUEST']._serialized_end=1235
+  _globals['_UPSTREAMRESUMERESPONSE']._serialized_start=1238
+  _globals['_UPSTREAMRESUMERESPONSE']._serialized_end=1545
+  _globals['_UPSTREAMCLOSEREQUEST']._serialized_start=1548
+  _globals['_UPSTREAMCLOSEREQUEST']._serialized_end=1827
+  _globals['_UPSTREAMCLOSERESPONSE']._serialized_start=1830
+  _globals['_UPSTREAMCLOSERESPONSE']._serialized_end=2078
+  _globals['_UPSTREAMCHUNK']._serialized_start=2081
+  _globals['_UPSTREAMCHUNK']._serialized_end=2333
+  _globals['_UPSTREAMCHUNKACK']._serialized_start=2336
+  _globals['_UPSTREAMCHUNKACK']._serialized_end=2719
+  _globals['_UPSTREAMCHUNKACK_DATAIDALIASESENTRY']._serialized_start=965
+  _globals['_UPSTREAMCHUNKACK_DATAIDALIASESENTRY']._serialized_end=1047
+  _globals['_UPSTREAMMETADATA']._serialized_start=2722
+  _globals['_UPSTREAMMETADATA']._serialized_end=2931
+  _globals['_UPSTREAMMETADATAACK']._serialized_start=2934
+  _globals['_UPSTREAMMETADATAACK']._serialized_end=3178
+  _globals['_UPSTREAMCHUNKRESULT']._serialized_start=3181
+  _globals['_UPSTREAMCHUNKRESULT']._serialized_end=3435
 # @@protoc_insertion_point(module_scope)
```

## Comparing `iscp/_encoding/codegen/extensions/connection_pb2.py` & `iscp/_encoding/_codegen/iscp2/v1/extensions/ping_pong_pb2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: extensions/connection.proto
+# source: iscp2/v1/extensions/ping_pong.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x65xtensions/connection.proto\x12\x05iscp2\"f\n\x1d\x43onnectRequestExtensionFields\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x01 \x01(\t\x12/\n\x07intdash\x18\x80\x08 \x01(\x0b\x32\x1d.iscp2.IntdashExtensionFields\".\n\x16IntdashExtensionFields\x12\x14\n\x0cproject_uuid\x18\x01 \x01(\t\" \n\x1e\x43onnectResponseExtensionFields\"\x1b\n\x19\x44isconnectExtensionFieldsb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#iscp2/v1/extensions/ping_pong.proto\x12\x13iscp2.v1.extensions\"\x15\n\x13PingExtensionFields\"\x15\n\x13PongExtensionFieldsB\x96\x01\n\x17\x63om.iscp2.v1.extensionsB\rPingPongProtoP\x01\xa2\x02\x03IVE\xaa\x02\x13Iscp2.V1.Extensions\xca\x02\x13Iscp2\\V1\\Extensions\xe2\x02\x1fIscp2\\V1\\Extensions\\GPBMetadata\xea\x02\x15Iscp2::V1::Extensionsb\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'extensions.connection_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'iscp2.v1.extensions.ping_pong_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _CONNECTREQUESTEXTENSIONFIELDS._serialized_start=38
-  _CONNECTREQUESTEXTENSIONFIELDS._serialized_end=140
-  _INTDASHEXTENSIONFIELDS._serialized_start=142
-  _INTDASHEXTENSIONFIELDS._serialized_end=188
-  _CONNECTRESPONSEEXTENSIONFIELDS._serialized_start=190
-  _CONNECTRESPONSEEXTENSIONFIELDS._serialized_end=222
-  _DISCONNECTEXTENSIONFIELDS._serialized_start=224
-  _DISCONNECTEXTENSIONFIELDS._serialized_end=251
+  DESCRIPTOR._serialized_options = b'\n\027com.iscp2.v1.extensionsB\rPingPongProtoP\001\242\002\003IVE\252\002\023Iscp2.V1.Extensions\312\002\023Iscp2\\V1\\Extensions\342\002\037Iscp2\\V1\\Extensions\\GPBMetadata\352\002\025Iscp2::V1::Extensions'
+  _globals['_PINGEXTENSIONFIELDS']._serialized_start=60
+  _globals['_PINGEXTENSIONFIELDS']._serialized_end=81
+  _globals['_PONGEXTENSIONFIELDS']._serialized_start=83
+  _globals['_PONGEXTENSIONFIELDS']._serialized_end=104
 # @@protoc_insertion_point(module_scope)
```

## Comparing `iscp/_encoding/codegen/extensions/e2e_call_pb2.py` & `iscp/_encoding/_codegen/iscp2/v1/ping_pong_pb2.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: extensions/e2e_call.proto
+# source: iscp2/v1/ping_pong.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from .extensions import ping_pong_pb2 as iscp2_dot_v1_dot_extensions_dot_ping__pong__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19\x65xtensions/e2e_call.proto\x12\x05iscp2\"\x1d\n\x1bUpstreamCallExtensionFields\" \n\x1eUpstreamCallAckExtensionFields\"\x1f\n\x1d\x44ownstreamCallExtensionFieldsb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18iscp2/v1/ping_pong.proto\x12\x08iscp2.v1\x1a#iscp2/v1/extensions/ping_pong.proto\"z\n\x04Ping\x12\x1d\n\nrequest_id\x18\x01 \x01(\rR\trequestId\x12S\n\x10\x65xtension_fields\x18\x02 \x01(\x0b\x32(.iscp2.v1.extensions.PingExtensionFieldsR\x0f\x65xtensionFields\"z\n\x04Pong\x12\x1d\n\nrequest_id\x18\x01 \x01(\rR\trequestId\x12S\n\x10\x65xtension_fields\x18\x02 \x01(\x0b\x32(.iscp2.v1.extensions.PongExtensionFieldsR\x0f\x65xtensionFieldsB^\n\x0c\x63om.iscp2.v1B\rPingPongProtoP\x01\xa2\x02\x03IXX\xaa\x02\x08Iscp2.V1\xca\x02\x08Iscp2\\V1\xe2\x02\x14Iscp2\\V1\\GPBMetadata\xea\x02\tIscp2::V1b\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'extensions.e2e_call_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'iscp2.v1.ping_pong_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _UPSTREAMCALLEXTENSIONFIELDS._serialized_start=36
-  _UPSTREAMCALLEXTENSIONFIELDS._serialized_end=65
-  _UPSTREAMCALLACKEXTENSIONFIELDS._serialized_start=67
-  _UPSTREAMCALLACKEXTENSIONFIELDS._serialized_end=99
-  _DOWNSTREAMCALLEXTENSIONFIELDS._serialized_start=101
-  _DOWNSTREAMCALLEXTENSIONFIELDS._serialized_end=132
+  DESCRIPTOR._serialized_options = b'\n\014com.iscp2.v1B\rPingPongProtoP\001\242\002\003IXX\252\002\010Iscp2.V1\312\002\010Iscp2\\V1\342\002\024Iscp2\\V1\\GPBMetadata\352\002\tIscp2::V1'
+  _globals['_PING']._serialized_start=75
+  _globals['_PING']._serialized_end=197
+  _globals['_PONG']._serialized_start=199
+  _globals['_PONG']._serialized_end=321
 # @@protoc_insertion_point(module_scope)
```

## Comparing `iscp/_encoding/codegen/result_code_pb2.py` & `iscp/_encoding/_codegen/iscp2/v1/result_code_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: result_code.proto
+# source: iscp2/v1/result_code.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11result_code.proto\x12\x05iscp2*\xfc\x06\n\nResultCode\x12\r\n\tSUCCEEDED\x10\x00\x12\x12\n\x0eNORMAL_CLOSURE\x10\x00\x12\x18\n\x14INCOMPATIBLE_VERSION\x10\x01\x12\x19\n\x15MAXIMUM_DATA_ID_ALIAS\x10\x02\x12\x1a\n\x16MAXIMUM_UPSTREAM_ALIAS\x10\x03\x12\x15\n\x11UNSPECIFIED_ERROR\x10@\x12\x0e\n\nNO_NODE_ID\x10\x41\x12\x0f\n\x0b\x41UTH_FAILED\x10\x42\x12\x13\n\x0f\x43ONNECT_TIMEOUT\x10\x43\x12\x15\n\x11MALFORMED_MESSAGE\x10\x44\x12\x12\n\x0ePROTOCOL_ERROR\x10\x45\x12\x0f\n\x0b\x41\x43K_TIMEOUT\x10\x46\x12\x13\n\x0fINVALID_PAYLOAD\x10G\x12\x13\n\x0fINVALID_DATA_ID\x10H\x12\x19\n\x15INVALID_DATA_ID_ALIAS\x10I\x12\x17\n\x13INVALID_DATA_FILTER\x10J\x12\x14\n\x10STREAM_NOT_FOUND\x10K\x12\x1b\n\x17RESUME_REQUEST_CONFLICT\x10L\x12\x12\n\x0ePROCESS_FAILED\x10M\x12\x1d\n\x19\x44\x45SIRED_QOS_NOT_SUPPORTED\x10N\x12\x10\n\x0cPING_TIMEOUT\x10O\x12\x1a\n\x16TOO_LARGE_MESSAGE_SIZE\x10P\x12\x1c\n\x18TOO_MANY_DATA_ID_ALIASES\x10Q\x12\x14\n\x10TOO_MANY_STREAMS\x10R\x12\x19\n\x15TOO_LONG_ACK_INTERVAL\x10S\x12\x1f\n\x1bTOO_MANY_DOWNSTREAM_FILTERS\x10T\x12\x19\n\x15TOO_MANY_DATA_FILTERS\x10U\x12\x1c\n\x18TOO_LONG_EXPIRY_INTERVAL\x10V\x12\x19\n\x15TOO_LONG_PING_TIMEOUT\x10W\x12\x1b\n\x17TOO_SHORT_PING_INTERVAL\x10X\x12\x1a\n\x16TOO_SHORT_PING_TIMEOUT\x10Y\x12\x16\n\x12RATE_LIMIT_REACHED\x10Z\x12\x15\n\x10NODE_ID_MISMATCH\x10\x80\x01\x12\x16\n\x11SESSION_NOT_FOUND\x10\x81\x01\x12\x1b\n\x16SESSION_ALREADY_CLOSED\x10\x82\x01\x12\x1a\n\x15SESSION_CANNOT_CLOSED\x10\x83\x01\x1a\x02\x10\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1aiscp2/v1/result_code.proto\x12\x08iscp2.v1*\xfc\x06\n\nResultCode\x12\r\n\tSUCCEEDED\x10\x00\x12\x12\n\x0eNORMAL_CLOSURE\x10\x00\x12\x18\n\x14INCOMPATIBLE_VERSION\x10\x01\x12\x19\n\x15MAXIMUM_DATA_ID_ALIAS\x10\x02\x12\x1a\n\x16MAXIMUM_UPSTREAM_ALIAS\x10\x03\x12\x15\n\x11UNSPECIFIED_ERROR\x10@\x12\x0e\n\nNO_NODE_ID\x10\x41\x12\x0f\n\x0b\x41UTH_FAILED\x10\x42\x12\x13\n\x0f\x43ONNECT_TIMEOUT\x10\x43\x12\x15\n\x11MALFORMED_MESSAGE\x10\x44\x12\x12\n\x0ePROTOCOL_ERROR\x10\x45\x12\x0f\n\x0b\x41\x43K_TIMEOUT\x10\x46\x12\x13\n\x0fINVALID_PAYLOAD\x10G\x12\x13\n\x0fINVALID_DATA_ID\x10H\x12\x19\n\x15INVALID_DATA_ID_ALIAS\x10I\x12\x17\n\x13INVALID_DATA_FILTER\x10J\x12\x14\n\x10STREAM_NOT_FOUND\x10K\x12\x1b\n\x17RESUME_REQUEST_CONFLICT\x10L\x12\x12\n\x0ePROCESS_FAILED\x10M\x12\x1d\n\x19\x44\x45SIRED_QOS_NOT_SUPPORTED\x10N\x12\x10\n\x0cPING_TIMEOUT\x10O\x12\x1a\n\x16TOO_LARGE_MESSAGE_SIZE\x10P\x12\x1c\n\x18TOO_MANY_DATA_ID_ALIASES\x10Q\x12\x14\n\x10TOO_MANY_STREAMS\x10R\x12\x19\n\x15TOO_LONG_ACK_INTERVAL\x10S\x12\x1f\n\x1bTOO_MANY_DOWNSTREAM_FILTERS\x10T\x12\x19\n\x15TOO_MANY_DATA_FILTERS\x10U\x12\x1c\n\x18TOO_LONG_EXPIRY_INTERVAL\x10V\x12\x19\n\x15TOO_LONG_PING_TIMEOUT\x10W\x12\x1b\n\x17TOO_SHORT_PING_INTERVAL\x10X\x12\x1a\n\x16TOO_SHORT_PING_TIMEOUT\x10Y\x12\x16\n\x12RATE_LIMIT_REACHED\x10Z\x12\x15\n\x10NODE_ID_MISMATCH\x10\x80\x01\x12\x16\n\x11SESSION_NOT_FOUND\x10\x81\x01\x12\x1b\n\x16SESSION_ALREADY_CLOSED\x10\x82\x01\x12\x1a\n\x15SESSION_CANNOT_CLOSED\x10\x83\x01\x1a\x02\x10\x01\x42`\n\x0c\x63om.iscp2.v1B\x0fResultCodeProtoP\x01\xa2\x02\x03IXX\xaa\x02\x08Iscp2.V1\xca\x02\x08Iscp2\\V1\xe2\x02\x14Iscp2\\V1\\GPBMetadata\xea\x02\tIscp2::V1b\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'result_code_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'iscp2.v1.result_code_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
+  DESCRIPTOR._serialized_options = b'\n\014com.iscp2.v1B\017ResultCodeProtoP\001\242\002\003IXX\252\002\010Iscp2.V1\312\002\010Iscp2\\V1\342\002\024Iscp2\\V1\\GPBMetadata\352\002\tIscp2::V1'
   _RESULTCODE._options = None
   _RESULTCODE._serialized_options = b'\020\001'
-  _RESULTCODE._serialized_start=29
-  _RESULTCODE._serialized_end=921
+  _globals['_RESULTCODE']._serialized_start=41
+  _globals['_RESULTCODE']._serialized_end=933
 # @@protoc_insertion_point(module_scope)
```

## Comparing `iscp-0.9.1.dist-info/LICENSE` & `iscp-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `iscp-0.9.1.dist-info/METADATA` & `iscp-1.0.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: iscp
-Version: 0.9.1
+Version: 1.0.0
 Summary: iSCP client for python
 License: Apache-2.0
 Keywords: intdash,iscp,intdash sdk,iscp sdk
 Author: aptpod,Inc
 Author-email: sdk-support@aptpod.co.jp
 Maintainer: aptpod,Inc
 Maintainer-email: sdk-support@aptpod.co.jp
-Requires-Python: >=3.10,<3.11
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aioquic (>=0.9.20,<0.10.0)
 Requires-Dist: protobuf (>4.0.0)
 Requires-Dist: websockets (>=10.2,<11.0)
 Description-Content-Type: text/markdown
 
 # iscp-py
```

## Comparing `iscp-0.9.1.dist-info/RECORD` & `iscp-1.0.0.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,58 @@
-iscp/__init__.py,sha256=0NGrF9JhA0tsMBHzTLOFExVr0zJ4hzRAJaxpopLg-bM,3385
-iscp/_conn.py,sha256=c0ndyYa55X8D3ihIvTjzkdV1-Hm4zNfCZq2ws5Hu824,32299
-iscp/_downstream.py,sha256=8tSImgitXz9H9xk1SuC6f7YYsyPSl79gfY7HczgvCk8,15745
+iscp/__init__.py,sha256=p6AOEv-CrMBVvmxIcgLDSL9_7y3oNKhKABkV-d0R9k4,3385
+iscp/_conn.py,sha256=qv-iZts8EPcTJq9zNMzTUmow2d8H134730PBz7VBOn8,32653
+iscp/_downstream.py,sha256=Wp8ucoCU--G5GZxmUPyh08uDTbs2mJBWk4FFVzzm3fw,15759
 iscp/_encoding/__init__.py,sha256=27OAXmMjjXWboCT8jjDEKadRdRMxqki_CGQb6YJLOKU,168
+iscp/_encoding/_codegen/iscp2/v1/common_pb2.py,sha256=o0M7Bhahs2bxP1pk5wDbhXva7WENj8RY-QNxQgfBGMA,3005
+iscp/_encoding/_codegen/iscp2/v1/connection_pb2.py,sha256=6CxSu5YH5rGkZp5TfC-t63JgoHbziOguV4bW6YWpRlg,2901
+iscp/_encoding/_codegen/iscp2/v1/downstream_pb2.py,sha256=lsIMGoBC_Sv3Izs7DpaFuFNJiAHVRHtGhmwO4Sle_yU,11050
+iscp/_encoding/_codegen/iscp2/v1/e2e_call_pb2.py,sha256=xxo-Op1thSsxhtBtRKrg3Ap0-Ra1S5DoaL3tSPqRoUE,3092
+iscp/_encoding/_codegen/iscp2/v1/extensions/connection_pb2.py,sha256=kpH8QeFqrOoMqLq2AfQY6A7Ds5y6b9tLyrPZ9OeOXIY,2307
+iscp/_encoding/_codegen/iscp2/v1/extensions/downstream_pb2.py,sha256=aGbtUN6EttraAYiZ8VSTRiRNfBt16n75cjCsJiT4kHI,3671
+iscp/_encoding/_codegen/iscp2/v1/extensions/e2e_call_pb2.py,sha256=IeA6y2Sh_4DbCFC46xbz4foMixHwwXNAElrg1a75MPc,1916
+iscp/_encoding/_codegen/iscp2/v1/extensions/ping_pong_pb2.py,sha256=stBHgMwKvFIJtrWTRnr10ECSakF6XnT1H4CeyzX4xVw,1671
+iscp/_encoding/_codegen/iscp2/v1/extensions/upstream_pb2.py,sha256=qQ07b1A8hEfms5ABAWdaYl6n4U-OWG62JTuqmkZRzrQ,3556
+iscp/_encoding/_codegen/iscp2/v1/message_pb2.py,sha256=QB7c2TZnah0PB5dE7yakG4JjLj_-IK-oUdi_K67ECl8,5167
+iscp/_encoding/_codegen/iscp2/v1/metadata_pb2.py,sha256=fXnuPSJHZViu_IGxs6Tt4oGAnU-b0jWoZA7JWJNWSAk,4036
+iscp/_encoding/_codegen/iscp2/v1/ping_pong_pb2.py,sha256=0rcM_skI4B3RYcQ3CYygX25YiAPFK_-SH5RJ_dou9hM,1870
+iscp/_encoding/_codegen/iscp2/v1/result_code_pb2.py,sha256=8LQctACMlSqTgJend1o5O2PoI57hJkhmiBeNZPqUObg,2860
+iscp/_encoding/_codegen/iscp2/v1/upstream_pb2.py,sha256=tiUFN5-PLPkZ4K2U2MU-ocrFOje7HE8L6jsN8KVoqb8,8376
 iscp/_encoding/_encoding.py,sha256=Z_f5315iLwKkepaawEurkZTtkvjrmWly37yMUEHnQM8,540
 iscp/_encoding/_protobuf/__init__.py,sha256=vz1kuNcMuLJ-Ercgxc4Yq8BZITcx0b2huGifN_QdpRY,168
-iscp/_encoding/_protobuf/_protobuf.py,sha256=MPNW6vWY1X0zWB96Do8SGTuRFjjbeED6ZLL4DqXSHwU,1153
+iscp/_encoding/_protobuf/_protobuf.py,sha256=37GpXN7PH9q-P99-AZT42Xp4h6_sz30a_ZdkfAz8pfw,1313
 iscp/_encoding/_protobuf/converter/__init__.py,sha256=TBtCrdKRgRr90RuMa-bxgZj4iNo8faWYhD0M1xsExYo,101
-iscp/_encoding/_protobuf/converter/_common.py,sha256=DtVkq8PIfOs9nABWDtW4mIO9YgeJlT7c7eoGmTnsvQc,6248
-iscp/_encoding/_protobuf/converter/_connection.py,sha256=xs8xbIpBx-FjvelLLOJf3u8cTfYqPddc-vowUjp0Uic,6224
-iscp/_encoding/_protobuf/converter/_converter.py,sha256=eLCQ_z7KoOMfbmZ-q9iywKMblKn6yLgSt_m7bSQti5M,10867
-iscp/_encoding/_protobuf/converter/_downstream.py,sha256=NH6YYN0tYjRPsrHf_7h9xXEBd3y2bFfdkzzM1wS6K0U,26623
-iscp/_encoding/_protobuf/converter/_e2e_call.py,sha256=LaNU-A_tWHladUCtLGJvUU-EHyRws5CfmwlSowuLRTc,4672
-iscp/_encoding/_protobuf/converter/_metadata.py,sha256=eiwFWhXZfSNE6bX4euoZlg3Q0KomiHskJLefoh8blwA,6328
-iscp/_encoding/_protobuf/converter/_ping_pong.py,sha256=Val3bRikAzmqaR7yG1CwTwhDq6hVbm7x2zChdTEA9TE,1964
-iscp/_encoding/_protobuf/converter/_result_code.py,sha256=Gs1HflhdXt3BTs98inr3Z1aa4WJMp_GvDR5_zcieGhk,496
-iscp/_encoding/_protobuf/converter/_upstream.py,sha256=qPHn70VxD5irm6VlU38tVpinz1ADTB-Io4FstKQXSr4,20496
-iscp/_encoding/codegen/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-iscp/_encoding/codegen/__init__.pyi,sha256=OQhbll7kIDZxQYQyzh5K9Cr-qjLCGIhPGCjyM4Nak5Y,1206
-iscp/_encoding/codegen/common_pb2.py,sha256=pNc7EHAZCbggasfC8bRRAHhtuDvYZ2Ntcufr6IqU_qo,2236
-iscp/_encoding/codegen/connection_pb2.py,sha256=gXDdVi8jZpkF_xBM7sCgxVpia3Lgh33toX94u0Bd7-Q,2106
-iscp/_encoding/codegen/downstream_pb2.py,sha256=LB8WAEiKaLTTqx2zhC3c-U3_bHPwgM0tzNW7NEktb7U,8555
-iscp/_encoding/codegen/e2e_call_pb2.py,sha256=udjDVubE28Ip5_FgwBABscjJOpIsFEuqxTNjNUG1F0A,2247
-iscp/_encoding/codegen/extensions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-iscp/_encoding/codegen/extensions/__init__.pyi,sha256=bof8UAG8sWYUOjDDPLV8RFGgFCyx3pyc57c5vxmOsRk,612
-iscp/_encoding/codegen/extensions/connection_pb2.py,sha256=8N2N_JEth012D2D5Xy1-bCWNiygLqi4BGr4RSUE6HEE,1608
-iscp/_encoding/codegen/extensions/downstream_pb2.py,sha256=PsUQVeOxRCJULp4-bpqIYljeIpg2e5OVG2Q_tkb88DU,2850
-iscp/_encoding/codegen/extensions/e2e_call_pb2.py,sha256=moRaHQGl-igMb5ZgiT-CqkbIOkTtr4vbUK3SSsiuKYA,1304
-iscp/_encoding/codegen/extensions/ping_pong_pb2.py,sha256=a2wsR_aMWsxLbJunIAZRWB2Ezzja4C8x3MMyEMEkrOE,1101
-iscp/_encoding/codegen/extensions/upstream_pb2.py,sha256=oAlfM84FWLHTKgxLOu5GqLI86krXT5CKdlnpmWYVeiU,2727
-iscp/_encoding/codegen/message_pb2.py,sha256=riCYfb8z5ZZlGJ6p-3o2TuwBLXQl4sXz9I2bmgWuBi8,3908
-iscp/_encoding/codegen/metadata_pb2.py,sha256=zRt4s12B6SR05gFu6RijyIsbVHGXt9A3A784ZBXdpcw,3021
-iscp/_encoding/codegen/ping_pong_pb2.py,sha256=nAImTyT7gEDAT2Q-U7raV_sVvL8jjlfbdEGOErmwQxE,1327
-iscp/_encoding/codegen/result_code_pb2.py,sha256=6w3ca9sEHGeVJh7gDI3gUxiRdDJOH3PubpSc-DjllB8,2439
-iscp/_encoding/codegen/upstream_pb2.py,sha256=vvQyWLCP-rV1AOY0yNsx1bphG4mihT20UPld7iHzeOc,6424
+iscp/_encoding/_protobuf/converter/_common.py,sha256=cL7KKkzzW1sbgjDdXAWaghcoxaIM9a7ledaW-u9yZ-U,6318
+iscp/_encoding/_protobuf/converter/_connection.py,sha256=43gnNHcmwWAO01dtlKCLbZHTeT9noQHuAjlMKuCpLcc,6294
+iscp/_encoding/_protobuf/converter/_converter.py,sha256=3MQ0-7CMYXNne5GzdQWbcGLPaqoMPBVfTq01IqUtEKg,10877
+iscp/_encoding/_protobuf/converter/_downstream.py,sha256=omwEWh1G0dReCrNsC0XXnBKxNCUCDdyvefY4keDyI7k,26976
+iscp/_encoding/_protobuf/converter/_e2e_call.py,sha256=PAQ5VTcxwqSHsn6P1A823Q3LMuJwgRQzLlE0A79NBys,4732
+iscp/_encoding/_protobuf/converter/_metadata.py,sha256=ueB4-p80ez1YrpbkFDsUvQLAqyO6pG1OVFWqq9e8nVM,6418
+iscp/_encoding/_protobuf/converter/_ping_pong.py,sha256=lrqH4-3iYMDS3YtQXiVsQu2u8vylqPywX6cm0re3_lE,2004
+iscp/_encoding/_protobuf/converter/_result_code.py,sha256=voz0uh_hRIDc3YGrzyWztBqVYrMFXbuf7G873gSsLpU,506
+iscp/_encoding/_protobuf/converter/_upstream.py,sha256=q4uVPAEygmHVeCC9uYedDSHhKb6DlCmNuwGF9KRf9VM,20716
 iscp/_exceptions/__init__.py,sha256=0AXLPW91bclurmk86RW53cSBjk35g86Bowy3fjDymAA,103
 iscp/_exceptions/_exceptions.py,sha256=_LLQPaGdqeEizCp0MVATUJaPkSWB614vL3Q_ofNxUto,1557
 iscp/_flush_policy.py,sha256=7mfUmbGx8D0YC24_6twtOgNttDFZY0rihZjvP67Ni7E,3416
 iscp/_message/__init__.py,sha256=q2W4wMZPA42cynZOx-GfOoBHd0in44_syaDPetJk2BY,698
-iscp/_message/_common.py,sha256=HD89qmV26B3fETwDyfRWBi-546dWNIZyobH1VqOfh5A,7192
-iscp/_message/_connection.py,sha256=5pmyqGzsy8p8OhVWmwfZ7rLb9rH_0JikWxOptGzEFHw,1852
-iscp/_message/_downstream.py,sha256=RWue__thpZ0amvH2FTf7bqi7JfSNy8KESX83GwWYGfY,4933
+iscp/_message/_common.py,sha256=s1HM0Gdz92YIk6nfN7hCohbDALP3rLeEGRQbGs91jHw,9119
+iscp/_message/_connection.py,sha256=v0W51419BosamOb8pB-6MR-6bHFz1JomFobPlfyCmCI,1978
+iscp/_message/_downstream.py,sha256=HHk54xarpjgNfLM4vIrs-5kF7dFH5-fqtIu7ONP-YSA,4960
 iscp/_message/_e2e.py,sha256=QI6FA9Qeck1qdBLiW2OA-K3682lNeJBLC_k-3Ky0MaQ,1077
 iscp/_message/_message.py,sha256=ltzpJEgvXD5PMNyYaEvhLwBXtbFs68OEwSdaA4N23xE,314
 iscp/_message/_metadata.py,sha256=8DpgjN_KXdt7ioSG1Os3qpc0wQKAyLRdzf-9QZ9OBhk,3818
 iscp/_message/_ping_pong.py,sha256=b1IZzzmk4egbJJZyu_0qQAUsE2UE5wwoxNuHatFqkyM,426
 iscp/_message/_result_code.py,sha256=NDHBUuk5okmramQ8NV80AAUS6v8fDx8v-zN9-t9OaQ0,4434
 iscp/_message/_upstream.py,sha256=VR20rjn1NSetCK4l-M9ngsNCVp1x0gub8lS_y6nFDFE,5987
 iscp/_model.py,sha256=iHVepUJdbW559bi17M9_1E7Q6L21bozyR4z6Ii0SGDs,6078
-iscp/_sequence.py,sha256=LUcaEVX0T-dRhElwKyoLZfiw_-zPNNusSx8c-eUHde8,1324
+iscp/_sequence.py,sha256=kcgCJ_nnL1Qa2ykEIXuQoC0ePw5hdERcGkIGnUjAZMQ,1318
 iscp/_ticker.py,sha256=HOcs5dgHuMBP0_wUC9XndSeDRe334Tchcf8fjnzBoPI,937
 iscp/_transport/__init__.py,sha256=wqUAizhgLzf-7p6Q3L0gjIJq8sVXWk7VcXcrFlXhR0A,331
 iscp/_transport/_negotiation_params.py,sha256=y8K0P1sUvxUqdwK8f5biZXMvFDBsFK5ezgZWt0aB9oM,1751
-iscp/_transport/_quic.py,sha256=pXVBjsIG8KYXqbLgVS2-fYzvDLRwT2fpJRn2RjvYWBg,9195
+iscp/_transport/_quic.py,sha256=cGuTTd-mfjWsUT0hjNC66TnNcoWXBPPNT2xOlu3j0VY,9193
 iscp/_transport/_transport.py,sha256=wddNI6zOqDLrMXQ2B8ZTwppONd56fM4F2G-_OiHdHbc,2903
 iscp/_transport/_websocket.py,sha256=XRyzpnRGDFJqhzedbSfrrmUXDekdSFXyR-wHab4Xq5I,3410
-iscp/_upstream.py,sha256=fZXlzSdMkP5jaqlT4wBOJtYA9nw_mL__obgOoYaywvg,18854
-iscp/_utils.py,sha256=4Lpsy2upD750YwcdPJKqCbBt7DE74rekwSxCOJvppac,206
-iscp-0.9.1.dist-info/LICENSE,sha256=zM40BteXbVVne2uqncO4pi_zK8IbfXs1NBPjmAEHAAs,10619
-iscp-0.9.1.dist-info/WHEEL,sha256=vxFmldFsRN_Hx10GDvsdv1wroKq8r5Lzvjp6GZ4OO8c,88
-iscp-0.9.1.dist-info/METADATA,sha256=GaIKN4OqyXkZO8CDwkQ_Rzjdapr5ECKRxAGye9P3LAM,1280
-iscp-0.9.1.dist-info/RECORD,,
+iscp/_upstream.py,sha256=3zzWFbmyrr_3UXqvutNPA6YP2Dm9NQYZ3ZxR9GUDR2w,19632
+iscp/_utils.py,sha256=k3Jn-5QL1kCSOHDt2D4wXksnVyDrXNaS_HdchnmTBcY,570
+iscp-1.0.0.dist-info/LICENSE,sha256=zM40BteXbVVne2uqncO4pi_zK8IbfXs1NBPjmAEHAAs,10619
+iscp-1.0.0.dist-info/METADATA,sha256=2kXR4pIiLQ6U9SGdKGfe0VsYCI-SckkkyE9oqdXfQBM,1381
+iscp-1.0.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+iscp-1.0.0.dist-info/RECORD,,
```

