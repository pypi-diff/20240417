# Comparing `tmp/avocentdpdu-1.0.1.tar.gz` & `tmp/avocentdpdu-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avocentdpdu-1.0.1.tar", last modified: Tue Apr 16 01:26:57 2024, max compression
+gzip compressed data, was "avocentdpdu-1.1.0.tar", last modified: Tue Apr 16 02:03:02 2024, max compression
```

## Comparing `avocentdpdu-1.0.1.tar` & `avocentdpdu-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 01:26:57.006531 avocentdpdu-1.0.1/
--rw-rw-rw-   0        0        0     1090 2024-04-13 23:19:37.000000 avocentdpdu-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     1615 2024-04-16 01:26:57.003531 avocentdpdu-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1071 2024-04-14 00:54:59.000000 avocentdpdu-1.0.1/README.md
--rw-rw-rw-   0        0        0      528 2024-04-16 01:25:31.000000 avocentdpdu-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-16 01:26:57.006531 avocentdpdu-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-16 01:26:56.973532 avocentdpdu-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-16 01:26:56.989529 avocentdpdu-1.0.1/src/avocentdpdu/
--rw-rw-rw-   0        0        0        0 2024-04-14 00:05:20.000000 avocentdpdu-1.0.1/src/avocentdpdu/__init__.py
--rw-rw-rw-   0        0        0     7847 2024-04-16 01:19:39.000000 avocentdpdu-1.0.1/src/avocentdpdu/avocentdpdu.py
-drwxrwxrwx   0        0        0        0 2024-04-16 01:26:57.001533 avocentdpdu-1.0.1/src/avocentdpdu.egg-info/
--rw-rw-rw-   0        0        0     1615 2024-04-16 01:26:56.000000 avocentdpdu-1.0.1/src/avocentdpdu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2024-04-16 01:26:56.000000 avocentdpdu-1.0.1/src/avocentdpdu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 01:26:56.000000 avocentdpdu-1.0.1/src/avocentdpdu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-16 01:26:56.000000 avocentdpdu-1.0.1/src/avocentdpdu.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 02:03:02.164528 avocentdpdu-1.1.0/
+-rw-rw-rw-   0        0        0     1090 2024-04-13 23:19:37.000000 avocentdpdu-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1615 2024-04-16 02:03:02.164528 avocentdpdu-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1071 2024-04-14 00:54:59.000000 avocentdpdu-1.1.0/README.md
+-rw-rw-rw-   0        0        0      528 2024-04-16 02:02:45.000000 avocentdpdu-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-16 02:03:02.164528 avocentdpdu-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-16 02:03:02.136539 avocentdpdu-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-16 02:03:02.148528 avocentdpdu-1.1.0/src/avocentdpdu/
+-rw-rw-rw-   0        0        0        0 2024-04-14 00:05:20.000000 avocentdpdu-1.1.0/src/avocentdpdu/__init__.py
+-rw-rw-rw-   0        0        0     8370 2024-04-16 02:02:19.000000 avocentdpdu-1.1.0/src/avocentdpdu/avocentdpdu.py
+drwxrwxrwx   0        0        0        0 2024-04-16 02:03:02.160539 avocentdpdu-1.1.0/src/avocentdpdu.egg-info/
+-rw-rw-rw-   0        0        0     1615 2024-04-16 02:03:02.000000 avocentdpdu-1.1.0/src/avocentdpdu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2024-04-16 02:03:02.000000 avocentdpdu-1.1.0/src/avocentdpdu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 02:03:02.000000 avocentdpdu-1.1.0/src/avocentdpdu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-16 02:03:02.000000 avocentdpdu-1.1.0/src/avocentdpdu.egg-info/top_level.txt
```

### Comparing `avocentdpdu-1.0.1/LICENSE` & `avocentdpdu-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `avocentdpdu-1.0.1/PKG-INFO` & `avocentdpdu-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avocentdpdu
-Version: 1.0.1
+Version: 1.1.0
 Summary: Library to control Avocent DPDU10x PDUs
 Author-email: William Gibson <william.gibson.wg@gmail.com>
 Project-URL: Homepage, https://github.com/wgprojects/avocent_pdu
 Project-URL: Issues, https://github.com/wgprojects/avocent_pdu/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `avocentdpdu-1.0.1/README.md` & `avocentdpdu-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `avocentdpdu-1.0.1/pyproject.toml` & `avocentdpdu-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "avocentdpdu"
-version = "1.0.1"
+version = "1.1.0"
 authors = [
   { name="William Gibson", email="william.gibson.wg@gmail.com" },
 ]
 description = "Library to control Avocent DPDU10x PDUs"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `avocentdpdu-1.0.1/src/avocentdpdu/avocentdpdu.py` & `avocentdpdu-1.1.0/src/avocentdpdu/avocentdpdu.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,22 +92,36 @@
         self.switch_list = [Outlet(self, N, number_outlets, timeout) for N in range(self.number_outlets)]
         self.timeout = timeout
         self.pdu_status = "unknown"
         self.pdu_status_int = -1
         self.current_deciamps = 0
         self.password_status = "unknown"
         self.is_initialized = False
+        self.mac = ""
+
+    async def obtain_mac(self) -> str:
+        """Get PDU's MAC address from index page"""
+        async with aiohttp.ClientSession() as session:
+            url = f'http://{self.host}/mac.cgi'
+            async with session.get(url, timeout=self.timeout) as response:
+                return await response.text()
 
     async def initialize(self) -> None:
         """Call once after construction to test login, and obtain Outlet names"""
+        self.mac = await self.obtain_mac()  # Get MAC address identifier
+
+        # Pointless command used to test authentication
         await self.command_state(SwitchCommand.TURN_OFF, "0"*self.number_outlets)
+
+        # Request names for all outlets
         tasks = []
         for s in self.switch_list:
             tasks.append(s.obtain_name())
         await asyncio.gather(*tasks)
+
         self.is_initialized = True
 
     async def command_state(self, cmd_on: SwitchCommand, which_switches: str):
         """Command PDU to change one or more outlet states
         Note: The Avocent PDU commits the cardinal sin of using a GET request to change state
         """
```

### Comparing `avocentdpdu-1.0.1/src/avocentdpdu.egg-info/PKG-INFO` & `avocentdpdu-1.1.0/src/avocentdpdu.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avocentdpdu
-Version: 1.0.1
+Version: 1.1.0
 Summary: Library to control Avocent DPDU10x PDUs
 Author-email: William Gibson <william.gibson.wg@gmail.com>
 Project-URL: Homepage, https://github.com/wgprojects/avocent_pdu
 Project-URL: Issues, https://github.com/wgprojects/avocent_pdu/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

