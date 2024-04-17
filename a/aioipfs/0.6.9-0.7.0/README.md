# Comparing `tmp/aioipfs-0.6.9.tar.gz` & `tmp/aioipfs-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioipfs-0.6.9.tar", last modified: Wed Apr 17 09:41:14 2024, max compression
+gzip compressed data, was "aioipfs-0.7.0.tar", last modified: Wed Apr 17 18:00:57 2024, max compression
```

## Comparing `aioipfs-0.6.9.tar` & `aioipfs-0.7.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:41:14.891605 aioipfs-0.6.9/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2024-04-17 09:40:45.000000 aioipfs-0.6.9/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       54 2024-04-17 09:40:45.000000 aioipfs-0.6.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7627 2024-04-17 09:41:14.890604 aioipfs-0.6.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5502 2024-04-17 09:40:45.000000 aioipfs-0.6.9/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:41:14.884604 aioipfs-0.6.9/aioipfs/
--rw-rw-rw-   0 root         (0) root         (0)    10795 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    59427 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:41:14.887604 aioipfs-0.6.9/aioipfs/apis/
--rw-rw-rw-   0 root         (0) root         (0)     8143 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/apis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6802 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/apis/dag.py
--rw-rw-rw-   0 root         (0) root         (0)     2109 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/apis/multibase.py
--rw-rw-rw-   0 root         (0) root         (0)    12682 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/apis/p2p.py
--rw-rw-rw-   0 root         (0) root         (0)     7641 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/apis/pin.py
--rw-rw-rw-   0 root         (0) root         (0)     6161 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/apis/pubsub.py
--rw-rw-rw-   0 root         (0) root         (0)     4769 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/apis/swarm.py
--rw-rw-rw-   0 root         (0) root         (0)     2443 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     5484 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    10807 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/multi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:41:14.887604 aioipfs-0.6.9/aioipfs/scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/scripts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:41:14.888604 aioipfs-0.6.9/aioipfs/scripts/bohort/
--rw-rw-rw-   0 root         (0) root         (0)     7860 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/scripts/bohort/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1163 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/scripts/bohort/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2403 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:41:14.889604 aioipfs-0.6.9/aioipfs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7627 2024-04-17 09:41:14.000000 aioipfs-0.6.9/aioipfs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      634 2024-04-17 09:41:14.000000 aioipfs-0.6.9/aioipfs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 09:41:14.000000 aioipfs-0.6.9/aioipfs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2024-04-17 09:41:14.000000 aioipfs-0.6.9/aioipfs.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      398 2024-04-17 09:41:14.000000 aioipfs-0.6.9/aioipfs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-17 09:41:14.000000 aioipfs-0.6.9/aioipfs.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     2008 2024-04-17 09:40:45.000000 aioipfs-0.6.9/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 09:41:14.891605 aioipfs-0.6.9/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:41:14.888604 aioipfs-0.6.9/tests/
--rwxrwxrwx   0 root         (0) root         (0)    33595 2024-04-17 09:40:45.000000 aioipfs-0.6.9/tests/test_client.py
--rwxrwxrwx   0 root         (0) root         (0)     1193 2024-04-17 09:40:45.000000 aioipfs-0.6.9/tests/test_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 18:00:57.984653 aioipfs-0.7.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2024-04-17 18:00:25.000000 aioipfs-0.7.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       54 2024-04-17 18:00:25.000000 aioipfs-0.7.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7663 2024-04-17 18:00:57.984653 aioipfs-0.7.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5502 2024-04-17 18:00:25.000000 aioipfs-0.7.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 18:00:57.978653 aioipfs-0.7.0/aioipfs/
+-rw-rw-rw-   0 root         (0) root         (0)    11032 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    59427 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 18:00:57.981653 aioipfs-0.7.0/aioipfs/apis/
+-rw-rw-rw-   0 root         (0) root         (0)     8143 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/apis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6802 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/apis/dag.py
+-rw-rw-rw-   0 root         (0) root         (0)     2109 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/apis/multibase.py
+-rw-rw-rw-   0 root         (0) root         (0)    12682 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/apis/p2p.py
+-rw-rw-rw-   0 root         (0) root         (0)     7641 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/apis/pin.py
+-rw-rw-rw-   0 root         (0) root         (0)     6161 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/apis/pubsub.py
+-rw-rw-rw-   0 root         (0) root         (0)     4769 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/apis/swarm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2443 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5464 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    10807 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/multi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 18:00:57.981653 aioipfs-0.7.0/aioipfs/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/scripts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 18:00:57.981653 aioipfs-0.7.0/aioipfs/scripts/bohort/
+-rw-rw-rw-   0 root         (0) root         (0)     7860 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/scripts/bohort/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1163 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/scripts/bohort/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2403 2024-04-17 18:00:25.000000 aioipfs-0.7.0/aioipfs/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 18:00:57.982653 aioipfs-0.7.0/aioipfs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7663 2024-04-17 18:00:57.000000 aioipfs-0.7.0/aioipfs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      634 2024-04-17 18:00:57.000000 aioipfs-0.7.0/aioipfs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 18:00:57.000000 aioipfs-0.7.0/aioipfs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2024-04-17 18:00:57.000000 aioipfs-0.7.0/aioipfs.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      419 2024-04-17 18:00:57.000000 aioipfs-0.7.0/aioipfs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-17 18:00:57.000000 aioipfs-0.7.0/aioipfs.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2036 2024-04-17 18:00:25.000000 aioipfs-0.7.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 18:00:57.984653 aioipfs-0.7.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 18:00:57.982653 aioipfs-0.7.0/tests/
+-rwxrwxrwx   0 root         (0) root         (0)    33964 2024-04-17 18:00:25.000000 aioipfs-0.7.0/tests/test_client.py
+-rwxrwxrwx   0 root         (0) root         (0)     1193 2024-04-17 18:00:25.000000 aioipfs-0.7.0/tests/test_helpers.py
```

### Comparing `aioipfs-0.6.9/LICENSE` & `aioipfs-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.9/PKG-INFO` & `aioipfs-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioipfs
-Version: 0.6.9
+Version: 0.7.0
 Summary: Asynchronous IPFS client library
 Author-email: cipres <alkaline@gmx.co.uk>
 License: LGPLv3
 Project-URL: Homepage, https://gitlab.com/cipres/aioipfs
 Keywords: asyncio,aiohttp,ipfs
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
@@ -21,14 +21,15 @@
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: Communications :: File Sharing
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.7.4
 Requires-Dist: aiofiles>=0.7.0
+Requires-Dist: async-timeout>=4.0.3
 Requires-Dist: base58>=1.0.2
 Requires-Dist: gitignore-parser==0.1.9
 Requires-Dist: multiaddr>=0.0.9
 Requires-Dist: py-multibase>=1.0.3
 Requires-Dist: py-multiformats-cid>=0.4.3
 Requires-Dist: setuptools>=67.7.0
 Provides-Extra: orjson
```

### Comparing `aioipfs-0.6.9/README.rst` & `aioipfs-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.9/aioipfs/__init__.py` & `aioipfs-0.7.0/aioipfs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-__version__ = '0.6.9'
+__version__ = '0.7.0'
 
 from yarl import URL
 from distutils.version import StrictVersion  # type: ignore
 from typing import Union
 
+import async_timeout
 import asyncio
 import aiohttp
 import ipaddress
 import re
 import socket
 
 from aiohttp import BasicAuth
@@ -348,12 +349,18 @@
         try:
             ip = ipaddress.ip_address(self.host)
             return Multiaddr(f'/ip{ip.version}/{self.host}/tcp/{port}')
         except Exception:
             # Shouldn't assume dns4 here
             return Multiaddr(f'/dns4/{self.host}/tcp/{port}')
 
+    def timeout(self, time: float) -> async_timeout.Timeout:
+        return async_timeout.timeout(time)
+
+    def timeout_at(self, time: float) -> async_timeout.Timeout:
+        return async_timeout.timeout_at(time)
+
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, *args):
         await self.close()
```

### Comparing `aioipfs-0.6.9/aioipfs/api.py` & `aioipfs-0.7.0/aioipfs/api.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.9/aioipfs/apis/__init__.py` & `aioipfs-0.7.0/aioipfs/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.9/aioipfs/apis/dag.py` & `aioipfs-0.7.0/aioipfs/apis/dag.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.9/aioipfs/apis/multibase.py` & `aioipfs-0.7.0/aioipfs/apis/multibase.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.9/aioipfs/apis/p2p.py` & `aioipfs-0.7.0/aioipfs/apis/p2p.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.9/aioipfs/apis/pin.py` & `aioipfs-0.7.0/aioipfs/apis/pin.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.9/aioipfs/apis/pubsub.py` & `aioipfs-0.7.0/aioipfs/apis/pubsub.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.9/aioipfs/apis/swarm.py` & `aioipfs-0.7.0/aioipfs/apis/swarm.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.9/aioipfs/exceptions.py` & `aioipfs-0.7.0/aioipfs/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.9/aioipfs/helpers.py` & `aioipfs-0.7.0/aioipfs/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 
 from multiaddr import Multiaddr  # type: ignore
 from distutils.version import StrictVersion  # type: ignore
 from contextlib import closing
 from typing import Union
 import socket
-import os.path
+import posixpath
 
 from urllib.parse import quote
 
 from multiformats_cid import make_cid
 from multiformats_cid import CIDv1
 from multiformats_cid import CIDv0
 
@@ -126,15 +126,15 @@
     (peer_id, proto_full, proto_version)
 
     proto_full can be passed to 'ipfs p2p dial'
     """
 
     peer_id_re = re.compile(r'([\w]){46,59}$')
 
-    parts = addr.lstrip(os.path.sep).split(os.path.sep)
+    parts = addr.lstrip('/').split('/')
     try:
         assert parts.pop(0) == 'p2p'
         peer_id = parts.pop(0)
         prefix = parts.pop(0)
         assert peer_id_re.match(peer_id)
         assert prefix in ['x', 'y', 'z']
 
@@ -158,15 +158,15 @@
                 pass
             else:
                 # Found a version, should be last element
                 p_version = v
                 assert len(parts) == 0
                 break
 
-        return peer_id, os.path.sep + os.path.join(*proto_a), p_version
+        return peer_id, '/' + posixpath.join(*proto_a), p_version
     except Exception as err:
         raise ValueError(f'Invalid p2p endpoint addr: {err}')
 
 
 def peerid_reencode(peer_id: str,
                     base: str = 'base36',
                     multicodec: str = 'libp2p-key') -> Union[str, None]:
```

### Comparing `aioipfs-0.6.9/aioipfs/multi.py` & `aioipfs-0.7.0/aioipfs/multi.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.9/aioipfs/scripts/bohort/__init__.py` & `aioipfs-0.7.0/aioipfs/scripts/bohort/__init__.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.9/aioipfs/scripts/bohort/cli.py` & `aioipfs-0.7.0/aioipfs/scripts/bohort/cli.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.9/aioipfs/util.py` & `aioipfs-0.7.0/aioipfs/util.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.9/aioipfs.egg-info/PKG-INFO` & `aioipfs-0.7.0/aioipfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioipfs
-Version: 0.6.9
+Version: 0.7.0
 Summary: Asynchronous IPFS client library
 Author-email: cipres <alkaline@gmx.co.uk>
 License: LGPLv3
 Project-URL: Homepage, https://gitlab.com/cipres/aioipfs
 Keywords: asyncio,aiohttp,ipfs
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
@@ -21,14 +21,15 @@
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: Communications :: File Sharing
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.7.4
 Requires-Dist: aiofiles>=0.7.0
+Requires-Dist: async-timeout>=4.0.3
 Requires-Dist: base58>=1.0.2
 Requires-Dist: gitignore-parser==0.1.9
 Requires-Dist: multiaddr>=0.0.9
 Requires-Dist: py-multibase>=1.0.3
 Requires-Dist: py-multiformats-cid>=0.4.3
 Requires-Dist: setuptools>=67.7.0
 Provides-Extra: orjson
```

### Comparing `aioipfs-0.6.9/aioipfs.egg-info/SOURCES.txt` & `aioipfs-0.7.0/aioipfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.9/pyproject.toml` & `aioipfs-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     "Topic :: System :: Filesystems",
     "Topic :: Communications :: File Sharing",
 ]
 urls = {Homepage = "https://gitlab.com/cipres/aioipfs"}
 dependencies = [
     "aiohttp>=3.7.4",
     "aiofiles>=0.7.0",
+    "async-timeout>=4.0.3",
     "base58>=1.0.2",
     "gitignore-parser==0.1.9",
     "multiaddr>=0.0.9",
     "py-multibase>=1.0.3",
     "py-multiformats-cid>=0.4.3",
     "setuptools>=67.7.0",
 ]
```

### Comparing `aioipfs-0.6.9/tests/test_client.py` & `aioipfs-0.7.0/tests/test_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,14 +143,24 @@
     @pytest.mark.asyncio
     async def test_basic(self, event_loop, ipfsdaemon, iclient):
         await iclient.id()
         await iclient.core.version()
         await iclient.commands()
 
     @pytest.mark.asyncio
+    async def test_timeout(self, event_loop, iclient):
+        with pytest.raises(asyncio.TimeoutError):
+            async with iclient.timeout(1):
+                await asyncio.sleep(3)
+
+        with pytest.raises(asyncio.TimeoutError):
+            async with iclient.timeout_at(event_loop.time() + 2):
+                await asyncio.sleep(4)
+
+    @pytest.mark.asyncio
     async def test_bootstrap(self, event_loop, ipfsdaemon, iclient):
         await iclient.bootstrap.list()
 
     @pytest.mark.asyncio
     async def test_swarm(self, event_loop, ipfsdaemon, iclient):
         await iclient.swarm.peers()
         await iclient.swarm.addrs()
```

### Comparing `aioipfs-0.6.9/tests/test_helpers.py` & `aioipfs-0.7.0/tests/test_helpers.py`

 * *Files identical despite different names*

