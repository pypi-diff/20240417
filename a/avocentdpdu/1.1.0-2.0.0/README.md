# Comparing `tmp/avocentdpdu-1.1.0.tar.gz` & `tmp/avocentdpdu-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avocentdpdu-1.1.0.tar", last modified: Tue Apr 16 02:03:02 2024, max compression
+gzip compressed data, was "avocentdpdu-2.0.0.tar", last modified: Tue Apr 16 23:21:25 2024, max compression
```

## Comparing `avocentdpdu-1.1.0.tar` & `avocentdpdu-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 02:03:02.164528 avocentdpdu-1.1.0/
--rw-rw-rw-   0        0        0     1090 2024-04-13 23:19:37.000000 avocentdpdu-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     1615 2024-04-16 02:03:02.164528 avocentdpdu-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1071 2024-04-14 00:54:59.000000 avocentdpdu-1.1.0/README.md
--rw-rw-rw-   0        0        0      528 2024-04-16 02:02:45.000000 avocentdpdu-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-16 02:03:02.164528 avocentdpdu-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-16 02:03:02.136539 avocentdpdu-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-16 02:03:02.148528 avocentdpdu-1.1.0/src/avocentdpdu/
--rw-rw-rw-   0        0        0        0 2024-04-14 00:05:20.000000 avocentdpdu-1.1.0/src/avocentdpdu/__init__.py
--rw-rw-rw-   0        0        0     8370 2024-04-16 02:02:19.000000 avocentdpdu-1.1.0/src/avocentdpdu/avocentdpdu.py
-drwxrwxrwx   0        0        0        0 2024-04-16 02:03:02.160539 avocentdpdu-1.1.0/src/avocentdpdu.egg-info/
--rw-rw-rw-   0        0        0     1615 2024-04-16 02:03:02.000000 avocentdpdu-1.1.0/src/avocentdpdu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2024-04-16 02:03:02.000000 avocentdpdu-1.1.0/src/avocentdpdu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 02:03:02.000000 avocentdpdu-1.1.0/src/avocentdpdu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-16 02:03:02.000000 avocentdpdu-1.1.0/src/avocentdpdu.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 23:21:25.540381 avocentdpdu-2.0.0/
+-rw-rw-rw-   0        0        0     1090 2024-04-13 23:19:37.000000 avocentdpdu-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     1615 2024-04-16 23:21:25.538381 avocentdpdu-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1071 2024-04-14 00:54:59.000000 avocentdpdu-2.0.0/README.md
+-rw-rw-rw-   0        0        0      528 2024-04-16 23:20:52.000000 avocentdpdu-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-16 23:21:25.541382 avocentdpdu-2.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-16 23:21:25.503780 avocentdpdu-2.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-16 23:21:25.524772 avocentdpdu-2.0.0/src/avocentdpdu/
+-rw-rw-rw-   0        0        0        0 2024-04-14 00:05:20.000000 avocentdpdu-2.0.0/src/avocentdpdu/__init__.py
+-rw-rw-rw-   0        0        0     9322 2024-04-16 23:20:11.000000 avocentdpdu-2.0.0/src/avocentdpdu/avocentdpdu.py
+drwxrwxrwx   0        0        0        0 2024-04-16 23:21:25.535385 avocentdpdu-2.0.0/src/avocentdpdu.egg-info/
+-rw-rw-rw-   0        0        0     1615 2024-04-16 23:21:25.000000 avocentdpdu-2.0.0/src/avocentdpdu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2024-04-16 23:21:25.000000 avocentdpdu-2.0.0/src/avocentdpdu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 23:21:25.000000 avocentdpdu-2.0.0/src/avocentdpdu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-16 23:21:25.000000 avocentdpdu-2.0.0/src/avocentdpdu.egg-info/top_level.txt
```

### Comparing `avocentdpdu-1.1.0/LICENSE` & `avocentdpdu-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `avocentdpdu-1.1.0/PKG-INFO` & `avocentdpdu-2.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avocentdpdu
-Version: 1.1.0
+Version: 2.0.0
 Summary: Library to control Avocent DPDU10x PDUs
 Author-email: William Gibson <william.gibson.wg@gmail.com>
 Project-URL: Homepage, https://github.com/wgprojects/avocent_pdu
 Project-URL: Issues, https://github.com/wgprojects/avocent_pdu/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `avocentdpdu-1.1.0/README.md` & `avocentdpdu-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `avocentdpdu-1.1.0/pyproject.toml` & `avocentdpdu-2.0.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "avocentdpdu"
-version = "1.1.0"
+version = "2.0.0"
 authors = [
   { name="William Gibson", email="william.gibson.wg@gmail.com" },
 ]
 description = "Library to control Avocent DPDU10x PDUs"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `avocentdpdu-1.1.0/src/avocentdpdu/avocentdpdu.py` & `avocentdpdu-2.0.0/src/avocentdpdu/avocentdpdu.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         self.outlet_idx = outlet_idx
         self.outlet_id = outlet_idx + 1
         self.is_on_bool = False
         self.timeout = timeout
 
         # e.g. 0100000 to control OutletB 
         # or 11111111 to control all outlets on an 8 port unit
-        self.switch_flag = '0'*(outlet_idx) + '1' + '0'*(number_outlets-outlet_idx)
+        self.switch_flag = '0'*(outlet_idx) + '1' + '0'*(number_outlets-outlet_idx-1)
 
     async def obtain_name(self):
         """Call after initialization to obtain outlet name from PDU"""
         async with aiohttp.ClientSession() as session:
             async with session.get(f'http://{self.pdu.host}/switch{self.outlet_id}.cgi', timeout=self.timeout) as response:
                 html = await response.text()
                 if response.status == 200:
@@ -77,23 +77,23 @@
 
 
 # Default Username 'snmp'
 # Default Password '1234'
 class AvocentDPDU():
     """Main class representing an Avocent PDU"""
 
-    def __init__(self, host, username, password, number_outlets, timeout):
-        _LOGGER.info('Avocent PDU init')
+    def __init__(self, host, username, password, timeout):
+        _LOGGER.debug('Avocent PDU init')
         self.host = host
         self.username = username
         self.password = password
-        self.number_outlets = number_outlets
+        self.number_outlets = -1
         self.password_status = "Not attempted"
         self.password_ok = False
-        self.switch_list = [Outlet(self, N, number_outlets, timeout) for N in range(self.number_outlets)]
+        self.switch_list = []
         self.timeout = timeout
         self.pdu_status = "unknown"
         self.pdu_status_int = -1
         self.current_deciamps = 0
         self.password_status = "unknown"
         self.is_initialized = False
         self.mac = ""
@@ -105,17 +105,25 @@
             async with session.get(url, timeout=self.timeout) as response:
                 return await response.text()
 
     async def initialize(self) -> None:
         """Call once after construction to test login, and obtain Outlet names"""
         self.mac = await self.obtain_mac()  # Get MAC address identifier
 
+        self.number_outlets = await self.query_num_outlets()
+        assert self.number_outlets > 0
+
+        _LOGGER.debug("PDU has %s outlets.", self.number_outlets)
+        self.switch_list = [Outlet(self, N, self.number_outlets, self.timeout) for N in range(self.number_outlets)]
+
         # Pointless command used to test authentication
         await self.command_state(SwitchCommand.TURN_OFF, "0"*self.number_outlets)
 
+        _LOGGER.debug("PDU Authenticated: %s", self.is_valid_login())
+
         # Request names for all outlets
         tasks = []
         for s in self.switch_list:
             tasks.append(s.obtain_name())
         await asyncio.gather(*tasks)
 
         self.is_initialized = True
@@ -129,14 +137,29 @@
 
         async with aiohttp.ClientSession() as session:
             url = f'http://{self.host}/{endpoint}?3={self.username},{self.password},{which_switches},'
             async with session.get(url, timeout=self.timeout) as response:
                 await response.text()
                 # Response is always 404 with no body, even on success. Do nothing.
 
+    async def query_num_outlets(self) -> int:
+        """Check status and count number of reported outlet flags"""
+        async with aiohttp.ClientSession() as session:
+            url = f'http://{self.host}/control.cgi'
+            async with session.get(url, timeout=self.timeout) as response:
+                document = await response.text()
+                if response.status == 200:
+                    # Basic HTML parsing
+                    if "Z1" in document:
+                        name = document.split('name=')[1]
+                        data2 = name.split(',')
+                        statuses = data2[0]
+                        return len(statuses)
+        return -1
+
     async def update(self) -> None:
         """Get the status of the PDU"""
 
         if not self.is_initialized:
             await self.initialize()
 
         async with aiohttp.ClientSession() as session:
@@ -196,27 +219,26 @@
         return f"<AvocentPDU host:{self.host}; status:{self.pdu_status};\
         current:{self.current_deciamps/10.0}A;\
         login:{self.password_status}\n {switch_vals} >"
 
 
 async def main():
     _LOGGER.basicConfig(level=_LOGGER.INFO)
-    A = AvocentDPDU('192.168.1.131', 'snmp', '1234', 8, 10)
+    A = AvocentDPDU('192.168.1.131', 'snmp', '1234', 10)
     await A.update()
     print(A)
 
-    switches = A.switches()
+    # switches = A.switches()
 
-    switch = switches[2]
-    if switch.is_on():
-        await switch.turn_off()
-    else:
-        await switch.turn_on()
+    # switch = switches[2]
+    # if switch.is_on():
+    #     await switch.turn_off()
+    # else:
+    #     await switch.turn_on()
 
-    await A.update()
-    print(switch)
+    # await A.update()
+    # print(switch)
 
 if __name__ == "__main__":
-    print("laksjdla")
     loop = asyncio.get_event_loop()
     loop.run_until_complete(main())
     loop.close()
```

### Comparing `avocentdpdu-1.1.0/src/avocentdpdu.egg-info/PKG-INFO` & `avocentdpdu-2.0.0/src/avocentdpdu.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avocentdpdu
-Version: 1.1.0
+Version: 2.0.0
 Summary: Library to control Avocent DPDU10x PDUs
 Author-email: William Gibson <william.gibson.wg@gmail.com>
 Project-URL: Homepage, https://github.com/wgprojects/avocent_pdu
 Project-URL: Issues, https://github.com/wgprojects/avocent_pdu/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

