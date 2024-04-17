# Comparing `tmp/maxwell_client-0.8.0.tar.gz` & `tmp/maxwell_client-0.9.0.tar.gz`

## Comparing `maxwell_client-0.8.0.tar` & `maxwell_client-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 maxwell_client-0.8.0/.git
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 maxwell_client-0.8.0/Makefile
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 maxwell_client-0.8.0/requirements.txt
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 maxwell_client-0.8.0/setup.py
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 maxwell_client-0.8.0/config/logging.json
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 maxwell_client-0.8.0/maxwell/__init__.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 maxwell_client-0.8.0/maxwell/client/__init__.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 maxwell_client-0.8.0/maxwell/client/client.py
--rw-r--r--   0        0        0     7461 2020-02-02 00:00:00.000000 maxwell_client-0.8.0/maxwell/client/frontend.py
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 maxwell_client-0.8.0/maxwell/client/master.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 maxwell_client-0.8.0/maxwell/client/msg_queue.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 maxwell_client-0.8.0/maxwell/client/msg_queue_mgr.py
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 maxwell_client-0.8.0/maxwell/client/subscription_mgr.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 maxwell_client-0.8.0/test/test_master.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 maxwell_client-0.8.0/test/test_request.py
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 maxwell_client-0.8.0/test/test_subscribe.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 maxwell_client-0.8.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 maxwell_client-0.8.0/LICENSE
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 maxwell_client-0.8.0/README.md
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 maxwell_client-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    13859 2020-02-02 00:00:00.000000 maxwell_client-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 maxwell_client-0.9.0/.git
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 maxwell_client-0.9.0/Makefile
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 maxwell_client-0.9.0/requirements.txt
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 maxwell_client-0.9.0/setup.py
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 maxwell_client-0.9.0/config/logging.json
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 maxwell_client-0.9.0/maxwell/__init__.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 maxwell_client-0.9.0/maxwell/client/__init__.py
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 maxwell_client-0.9.0/maxwell/client/client.py
+-rw-r--r--   0        0        0     8155 2020-02-02 00:00:00.000000 maxwell_client-0.9.0/maxwell/client/frontend.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 maxwell_client-0.9.0/maxwell/client/master.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 maxwell_client-0.9.0/maxwell/client/msg_queue.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 maxwell_client-0.9.0/maxwell/client/msg_queue_mgr.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 maxwell_client-0.9.0/maxwell/client/subscription_mgr.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 maxwell_client-0.9.0/test/test_master.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 maxwell_client-0.9.0/test/test_request.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 maxwell_client-0.9.0/test/test_subscribe.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 maxwell_client-0.9.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 maxwell_client-0.9.0/LICENSE
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 maxwell_client-0.9.0/README.md
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 maxwell_client-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    13859 2020-02-02 00:00:00.000000 maxwell_client-0.9.0/PKG-INFO
```

### Comparing `maxwell_client-0.8.0/Makefile` & `maxwell_client-0.9.0/Makefile`

 * *Files identical despite different names*

### Comparing `maxwell_client-0.8.0/requirements.txt` & `maxwell_client-0.9.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `maxwell_client-0.8.0/config/logging.json` & `maxwell_client-0.9.0/config/logging.json`

 * *Files identical despite different names*

### Comparing `maxwell_client-0.8.0/maxwell/client/client.py` & `maxwell_client-0.9.0/maxwell/client/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,24 +24,37 @@
 
     def unsubscribe(self, topic):
         self.__frontend.unsubscribe(topic)
 
     def receive(self, topic, limit):
         return self.__frontend.receive(topic, limit)
 
-    async def request(self, path, payload=None, header={}):
-        return await self.__frontend.request(path, payload, header)
+    async def request(
+        self,
+        path,
+        payload=None,
+        header={},
+        wait_open_timeout=None,
+        round_timeout=None,
+    ):
+        return await self.__frontend.request(
+            path, payload, header, wait_open_timeout, round_timeout
+        )
 
     # ===========================================
     #  internal functions
     # ===========================================
     def __build_options(self, options):
         options = options if options else {}
+        if options.get("wait_open_timeout") == None:
+            options["wait_open_timeout"] = 3
+        if options.get("round_timeout") == None:
+            options["round_timeout"] = 5
+        if options.get("wait_consuming_timeout") == None:
+            options["wait_consuming_timeout"] = 10
         if options.get("queue_capacity") == None:
             options["queue_capacity"] = 512
         if options.get("get_limit") == None:
             options["get_limit"] = 128
         if options.get("endpoint_cache_ttl") == None:
             options["endpoint_cache_ttl"] = 10
-        if options.get("wait_consuming_timeout") == None:
-            options["wait_consuming_timeout"] = 10
         return options
```

### Comparing `maxwell_client-0.8.0/maxwell/client/frontend.py` & `maxwell_client-0.9.0/maxwell/client/frontend.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     def __init__(self, master, options, loop):
         super().__init__()
 
         self.__master = master
         self.__options = options
         self.__loop = loop
 
+        self.__should_run = True
+
         self.__subscription_mgr = SubscriptionMgr()
         self.__subscribe_callbacks = {}
         self.__msg_queue_mgr = MsgQueueMgr(self.__options.get("queue_capacity"))
         self.__not_full_events = {}  # {topic0: event0, ...}
         self.__pull_tasks = {}
 
         self.__connection = MultiAltEndpointsConnection(
@@ -40,14 +42,15 @@
             options=self.__options,
             event_handler=self,
             loop=self.__loop,
         )
         self.__failed_to_connect = False
 
     async def close(self):
+        self.__should_run = False
         self.__delete_all_pull_tasks()
         self.__subscription_mgr.clear()
         self.__subscribe_callbacks.clear()
         self.__msg_queue_mgr.clear()
         self.__not_full_events.clear()
         await self.__connection.close()
 
@@ -79,16 +82,27 @@
             msg_queue.delete_to(msgs[-1].offset)
             event.set()  # trigger not_full_event
             return msgs
         else:
             event.set()  # trigger not_full_event
             return []
 
-    async def request(self, path, payload=None, header=None):
-        result = await self.__request(self.__build_req_req(path, payload, header))
+    async def request(
+        self,
+        path,
+        payload=None,
+        header={},
+        wait_open_timeout=None,
+        round_timeout=None,
+    ):
+        result = await self.__request(
+            self.__build_req_req(path, payload, header),
+            wait_open_timeout,
+            round_timeout,
+        )
         return json.loads(result.payload)
 
     # ===========================================
     # EventHandler implementation
     # ===========================================
     def on_connecting(self, connection: MultiAltEndpointsConnection, _):
         self.notify(Event.ON_CONNECTING, connection)
@@ -133,21 +147,21 @@
     def __delete_pull_task(self, topic):
         task = self.__pull_tasks.get(topic)
         if task != None:
             task.cancel()
         self.__pull_tasks.pop(topic, None)
 
     async def __repeat_pull(self, topic):
-        while True:
+        while self.__should_run:
             try:
                 await self.__pull(topic)
             except asyncio.TimeoutError:
                 logger.debug("Timeout triggered, pull again...")
-            except Exception:
-                logger.warning("Error occured: %s", traceback.format_exc())
+            except Exception as e:
+                logger.warning("Error occured: %s", e)
                 await asyncio.sleep(1)
 
     async def __pull(self, topic):
         if not self.__subscription_mgr.has_subscribed(topic):
             logger.warning(f"Already unsubscribed: topic: {topic}")
             return
 
@@ -174,17 +188,30 @@
                 "topic: %s, last offset: %s",
                 topic,
                 msg_queue.last_offset(),
             )
             event.clear()
             await event.wait(self.__options["wait_consuming_timeout"])
 
-    async def __request(self, msg):
-        await self.__connection.wait_open()
-        return await self.__connection.request(msg)
+    async def __request(
+        self,
+        msg,
+        wait_open_timeout=None,
+        round_timeout=None,
+    ):
+        if wait_open_timeout == None:
+            wait_open_timeout = self.__options["wait_open_timeout"]
+        if round_timeout == None:
+            round_timeout = self.__options["round_timeout"]
+
+        async with asyncio.timeout(wait_open_timeout) as cm:
+            await self.__connection.wait_open()
+            next_delay = self.__loop.time() + round_timeout
+            cm.reschedule(next_delay)
+            return await self.__connection.request(msg)
 
     # ===========================================
     # req builders
     # ===========================================
     def __build_auth_req(self):
         auth_req = protocol_types.auth_req_t()
         auth_req.token = "ignore"
```

### Comparing `maxwell_client-0.8.0/maxwell/client/master.py` & `maxwell_client-0.9.0/maxwell/client/master.py`

 * *Files identical despite different names*

### Comparing `maxwell_client-0.8.0/maxwell/client/msg_queue.py` & `maxwell_client-0.9.0/maxwell/client/msg_queue.py`

 * *Files identical despite different names*

### Comparing `maxwell_client-0.8.0/maxwell/client/msg_queue_mgr.py` & `maxwell_client-0.9.0/maxwell/client/msg_queue_mgr.py`

 * *Files identical despite different names*

### Comparing `maxwell_client-0.8.0/maxwell/client/subscription_mgr.py` & `maxwell_client-0.9.0/maxwell/client/subscription_mgr.py`

 * *Files identical despite different names*

### Comparing `maxwell_client-0.8.0/test/test_master.py` & `maxwell_client-0.9.0/test/test_master.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,22 +4,26 @@
 from maxwell.client.master import Master
 
 logger = get_logger(__name__)
 
 
 def build_options(options=None):
     options = options if options else {}
+    if options.get("wait_open_timeout") == None:
+        options["wait_open_timeout"] = 3
+    if options.get("round_timeout") == None:
+        options["round_timeout"] = 5
+    if options.get("wait_consuming_timeout") == None:
+        options["wait_consuming_timeout"] = 10
     if options.get("queue_capacity") == None:
         options["queue_capacity"] = 512
     if options.get("get_limit") == None:
         options["get_limit"] = 128
     if options.get("endpoint_cache_ttl") == None:
         options["endpoint_cache_ttl"] = 10
-    if options.get("wait_consuming_timeout") == None:
-        options["wait_consuming_timeout"] = 10
     return options
 
 
 class TestMaster:
     @pytest.mark.asyncio
     async def test_normal(self):
         master = Master(["localhost:8081"], build_options())
```

### Comparing `maxwell_client-0.8.0/test/test_request.py` & `maxwell_client-0.9.0/test/test_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,34 +4,38 @@
 from maxwell.client.client import Client
 
 logger = get_logger(__name__)
 
 
 def build_options(options=None):
     options = options if options else {}
+    if options.get("wait_open_timeout") == None:
+        options["wait_open_timeout"] = 3
+    if options.get("round_timeout") == None:
+        options["round_timeout"] = 5
+    if options.get("wait_consuming_timeout") == None:
+        options["wait_consuming_timeout"] = 10
     if options.get("queue_capacity") == None:
         options["queue_capacity"] = 512
     if options.get("get_limit") == None:
         options["get_limit"] = 128
     if options.get("endpoint_cache_ttl") == None:
         options["endpoint_cache_ttl"] = 10
-    if options.get("wait_consuming_timeout") == None:
-        options["wait_consuming_timeout"] = 10
     return options
 
 
 class TestRequest:
     @pytest.mark.asyncio
     async def test_normal(self):
         client = Client(["localhost:8081"], build_options())
         result = await client.request(
             "/hello",
             {},
         )
-        assert result == "world"
+        assert result == "python"
         await client.close()
 
     @pytest.mark.asyncio
     async def test_nonexist_path(self):
         client = Client(["localhost:8081"], build_options())
         try:
             await client.request(
```

### Comparing `maxwell_client-0.8.0/test/test_subscribe.py` & `maxwell_client-0.9.0/test/test_subscribe.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,22 +4,26 @@
 from maxwell.client.client import Client
 
 logger = get_logger(__name__)
 
 
 def build_options(options=None):
     options = options if options else {}
+    if options.get("wait_open_timeout") == None:
+        options["wait_open_timeout"] = 3
+    if options.get("round_timeout") == None:
+        options["round_timeout"] = 5
+    if options.get("wait_consuming_timeout") == None:
+        options["wait_consuming_timeout"] = 10
     if options.get("queue_capacity") == None:
         options["queue_capacity"] = 512
     if options.get("get_limit") == None:
         options["get_limit"] = 128
     if options.get("endpoint_cache_ttl") == None:
         options["endpoint_cache_ttl"] = 10
-    if options.get("wait_consuming_timeout") == None:
-        options["wait_consuming_timeout"] = 10
     return options
 
 
 class TestSubscribe:
     @pytest.mark.asyncio
     async def test_normal(self):
         client = Client(["localhost:8081"], build_options())
```

### Comparing `maxwell_client-0.8.0/.gitignore` & `maxwell_client-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `maxwell_client-0.8.0/LICENSE` & `maxwell_client-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `maxwell_client-0.8.0/pyproject.toml` & `maxwell_client-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
   "maxwell-utils == 0.6.2",
 ]
 description = "The maxwell client implementation for python."
 license = {file = "LICENSE"}
 name = "maxwell-client"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "0.8.0"
+version = "0.9.0"
 
 [tool.pytest.ini_options]
 log_cli = true
 log_cli_date_format = "%Y-%m-%d %H:%M:%S"
 log_cli_format = "[%(levelname)8s] %(asctime)s (%(filename)s:%(lineno)s) %(message)s"
 log_cli_level = "DEBUG"
```

### Comparing `maxwell_client-0.8.0/PKG-INFO` & `maxwell_client-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maxwell-client
-Version: 0.8.0
+Version: 0.9.0
 Summary: The maxwell client implementation for python.
 Project-URL: changelog, https://github.com/maxwell-dev/maxwell-client-python/CHANGELOG.md
 Project-URL: repository, https://github.com/maxwell-dev/maxwell-client-python
 Author-email: Xu Chaoqian <chaoranxu@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

