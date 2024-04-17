# Comparing `tmp/mcitemlib-0.2.1.tar.gz` & `tmp/mcitemlib-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcitemlib-0.2.1.tar", max compression
+gzip compressed data, was "mcitemlib-0.2.2.tar", max compression
```

## Comparing `mcitemlib-0.2.1.tar` & `mcitemlib-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1060 2024-03-20 01:07:11.643195 mcitemlib-0.2.1/LICENSE
--rw-r--r--   0        0        0      599 2024-03-22 02:04:24.820036 mcitemlib-0.2.1/README.md
--rw-r--r--   0        0        0        0 2024-03-20 01:07:11.643195 mcitemlib-0.2.1/mcitemlib/__init__.py
--rw-r--r--   0        0        0    17709 2024-04-16 14:37:33.570484 mcitemlib-0.2.1/mcitemlib/itemlib.py
--rw-r--r--   0        0        0     8073 2024-04-16 14:37:33.570484 mcitemlib-0.2.1/mcitemlib/style.py
--rw-r--r--   0        0        0      432 2024-04-16 14:36:47.450324 mcitemlib-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1353 1970-01-01 00:00:00.000000 mcitemlib-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-03-20 01:07:11.643195 mcitemlib-0.2.2/LICENSE
+-rw-r--r--   0        0        0      599 2024-03-22 02:04:24.820036 mcitemlib-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2024-03-20 01:07:11.643195 mcitemlib-0.2.2/mcitemlib/__init__.py
+-rw-r--r--   0        0        0    17639 2024-04-17 02:17:42.400125 mcitemlib-0.2.2/mcitemlib/itemlib.py
+-rw-r--r--   0        0        0     8073 2024-04-16 14:37:33.570484 mcitemlib-0.2.2/mcitemlib/style.py
+-rw-r--r--   0        0        0      432 2024-04-17 02:21:34.773809 mcitemlib-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1353 1970-01-01 00:00:00.000000 mcitemlib-0.2.2/PKG-INFO
```

### Comparing `mcitemlib-0.2.1/LICENSE` & `mcitemlib-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mcitemlib-0.2.1/README.md` & `mcitemlib-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `mcitemlib-0.2.1/mcitemlib/itemlib.py` & `mcitemlib-0.2.2/mcitemlib/itemlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -485,51 +485,51 @@
         """
         if method == 'recode':
             return send_recode(self)
         if method == 'codeclient':
             return send_codeclient(self)
         return -1
 
-# TODO: change "template sent successfully" message into a more generic item sent message
-def send_recode(item: Item) -> int:
+
+def send_recode(item: Item, source: str='mcitemlib') -> int:
     """
     Sends a template to DiamondFire via recode item api.
 
     :param str templateCode: The code for the template as a base64 string.
     :param str name: The name of the template.
     :param str author: The author of the template.
 
     :return: status code
         - `0` = Success
         - `1` = Connection refused
         - `2` = Other socket error
     """
     
-    data = {'type': 'nbt', 'source': f'mcitemlib - {item.get_name().to_string()}', 'data': item.get_nbt()}
+    data = {'type': 'nbt', 'source': f'{source} - {item.get_name().to_string()}', 'data': item.get_nbt()}
     s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     try:
         s.connect(('localhost', RECODE_PORT))
     except ConnectionRefusedError:
         print(f"""{COL_ERROR}Could not connect to recode item API. Possible problems:
     - Minecraft is not open
     - Recode is not installed (get it here: https://modrinth.com/mod/recode or join the discord here: https://discord.gg/GWxWtcwA2C){COL_RESET}""")
         s.close()
         return 1
     
-    s.send((str(data) + '\n').encode('utf-8'))
+    s.send((json.dumps(data) + '\n').encode('utf-8'))
     received = json.loads(s.recv(1024).decode())
     status = received['status']
     s.close()
     time.sleep(0.5)
 
     if status == 'success':
-        print(f'{COL_SUCCESS}Template sent to client successfully.{COL_RESET}')
+        print(f'{COL_SUCCESS}Item sent to client successfully.{COL_RESET}')
         return 0
     error = received['error']
-    print(f'{COL_ERROR}Error sending template: {error}{COL_RESET}')
+    print(f'{COL_ERROR}Error sending item: {error}{COL_RESET}')
     return 2
 
 
 def send_codeclient(item: Item) -> int:
     try:
         ws = websocket.WebSocket()
         ws.connect(CODECLIENT_URL)
@@ -537,15 +537,15 @@
         
         ws.recv()  # auth response
 
         command = f'give {item.get_nbt()}'
         ws.send(command)
         ws.close()
 
-        print(f'{COL_SUCCESS}Template sent to client successfully.{COL_RESET}')
+        print(f'{COL_SUCCESS}Item sent to client successfully.{COL_RESET}')
         return 0
         
     except Exception as e:
         if isinstance(e, ConnectionRefusedError):
             print(f'{COL_ERROR}Could not connect to CodeClient API. Possible problems:')
             print(f'    - Minecraft is not open')
             print(f'    - CodeClient is not installed (get it here: https://modrinth.com/mod/codeclient)')
```

### Comparing `mcitemlib-0.2.1/mcitemlib/style.py` & `mcitemlib-0.2.2/mcitemlib/style.py`

 * *Files identical despite different names*

### Comparing `mcitemlib-0.2.1/PKG-INFO` & `mcitemlib-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcitemlib
-Version: 0.2.1
+Version: 0.2.2
 Summary: A library for creating and editing Minecraft items using python.
 Home-page: https://github.com/Amp63/mcitemlib
 License: MIT
 Keywords: minecraft,item,block,nbt
 Author: Amp
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

