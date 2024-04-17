# Comparing `tmp/aioipfs-0.6.8.tar.gz` & `tmp/aioipfs-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioipfs-0.6.8.tar", last modified: Tue Apr 16 21:29:11 2024, max compression
+gzip compressed data, was "aioipfs-0.6.9.tar", last modified: Wed Apr 17 09:41:14 2024, max compression
```

## Comparing `aioipfs-0.6.8.tar` & `aioipfs-0.6.9.tar`

### file list

```diff
@@ -1,32 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 21:29:11.621747 aioipfs-0.6.8/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2024-04-16 21:28:40.000000 aioipfs-0.6.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       54 2024-04-16 21:28:40.000000 aioipfs-0.6.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7627 2024-04-16 21:29:11.621747 aioipfs-0.6.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5502 2024-04-16 21:28:40.000000 aioipfs-0.6.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 21:29:11.616747 aioipfs-0.6.8/aioipfs/
--rw-rw-rw-   0 root         (0) root         (0)    10795 2024-04-16 21:28:40.000000 aioipfs-0.6.8/aioipfs/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    59423 2024-04-16 21:28:40.000000 aioipfs-0.6.8/aioipfs/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 21:29:11.619747 aioipfs-0.6.8/aioipfs/apis/
--rw-rw-rw-   0 root         (0) root         (0)     8143 2024-04-16 21:28:40.000000 aioipfs-0.6.8/aioipfs/apis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6802 2024-04-16 21:28:40.000000 aioipfs-0.6.8/aioipfs/apis/dag.py
--rw-rw-rw-   0 root         (0) root         (0)     2109 2024-04-16 21:28:40.000000 aioipfs-0.6.8/aioipfs/apis/multibase.py
--rw-rw-rw-   0 root         (0) root         (0)    12682 2024-04-16 21:28:40.000000 aioipfs-0.6.8/aioipfs/apis/p2p.py
--rw-rw-rw-   0 root         (0) root         (0)     7641 2024-04-16 21:28:40.000000 aioipfs-0.6.8/aioipfs/apis/pin.py
--rw-rw-rw-   0 root         (0) root         (0)     6161 2024-04-16 21:28:40.000000 aioipfs-0.6.8/aioipfs/apis/pubsub.py
--rw-rw-rw-   0 root         (0) root         (0)     4769 2024-04-16 21:28:40.000000 aioipfs-0.6.8/aioipfs/apis/swarm.py
--rw-rw-rw-   0 root         (0) root         (0)     2443 2024-04-16 21:28:40.000000 aioipfs-0.6.8/aioipfs/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     5484 2024-04-16 21:28:40.000000 aioipfs-0.6.8/aioipfs/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    10807 2024-04-16 21:28:40.000000 aioipfs-0.6.8/aioipfs/multi.py
--rw-rw-rw-   0 root         (0) root         (0)     2403 2024-04-16 21:28:40.000000 aioipfs-0.6.8/aioipfs/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 21:29:11.619747 aioipfs-0.6.8/aioipfs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7627 2024-04-16 21:29:11.000000 aioipfs-0.6.8/aioipfs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      541 2024-04-16 21:29:11.000000 aioipfs-0.6.8/aioipfs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 21:29:11.000000 aioipfs-0.6.8/aioipfs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2024-04-16 21:29:11.000000 aioipfs-0.6.8/aioipfs.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      398 2024-04-16 21:29:11.000000 aioipfs-0.6.8/aioipfs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-16 21:29:11.000000 aioipfs-0.6.8/aioipfs.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     2008 2024-04-16 21:28:40.000000 aioipfs-0.6.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 21:29:11.622747 aioipfs-0.6.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 21:29:11.619747 aioipfs-0.6.8/tests/
--rwxrwxrwx   0 root         (0) root         (0)    33305 2024-04-16 21:28:40.000000 aioipfs-0.6.8/tests/test_client.py
--rwxrwxrwx   0 root         (0) root         (0)     1193 2024-04-16 21:28:40.000000 aioipfs-0.6.8/tests/test_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:41:14.891605 aioipfs-0.6.9/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2024-04-17 09:40:45.000000 aioipfs-0.6.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       54 2024-04-17 09:40:45.000000 aioipfs-0.6.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7627 2024-04-17 09:41:14.890604 aioipfs-0.6.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5502 2024-04-17 09:40:45.000000 aioipfs-0.6.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:41:14.884604 aioipfs-0.6.9/aioipfs/
+-rw-rw-rw-   0 root         (0) root         (0)    10795 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    59427 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:41:14.887604 aioipfs-0.6.9/aioipfs/apis/
+-rw-rw-rw-   0 root         (0) root         (0)     8143 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/apis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6802 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/apis/dag.py
+-rw-rw-rw-   0 root         (0) root         (0)     2109 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/apis/multibase.py
+-rw-rw-rw-   0 root         (0) root         (0)    12682 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/apis/p2p.py
+-rw-rw-rw-   0 root         (0) root         (0)     7641 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/apis/pin.py
+-rw-rw-rw-   0 root         (0) root         (0)     6161 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/apis/pubsub.py
+-rw-rw-rw-   0 root         (0) root         (0)     4769 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/apis/swarm.py
+-rw-rw-rw-   0 root         (0) root         (0)     2443 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5484 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    10807 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/multi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:41:14.887604 aioipfs-0.6.9/aioipfs/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/scripts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:41:14.888604 aioipfs-0.6.9/aioipfs/scripts/bohort/
+-rw-rw-rw-   0 root         (0) root         (0)     7860 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/scripts/bohort/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1163 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/scripts/bohort/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2403 2024-04-17 09:40:45.000000 aioipfs-0.6.9/aioipfs/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:41:14.889604 aioipfs-0.6.9/aioipfs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7627 2024-04-17 09:41:14.000000 aioipfs-0.6.9/aioipfs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      634 2024-04-17 09:41:14.000000 aioipfs-0.6.9/aioipfs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 09:41:14.000000 aioipfs-0.6.9/aioipfs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2024-04-17 09:41:14.000000 aioipfs-0.6.9/aioipfs.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      398 2024-04-17 09:41:14.000000 aioipfs-0.6.9/aioipfs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-17 09:41:14.000000 aioipfs-0.6.9/aioipfs.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2008 2024-04-17 09:40:45.000000 aioipfs-0.6.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 09:41:14.891605 aioipfs-0.6.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 09:41:14.888604 aioipfs-0.6.9/tests/
+-rwxrwxrwx   0 root         (0) root         (0)    33595 2024-04-17 09:40:45.000000 aioipfs-0.6.9/tests/test_client.py
+-rwxrwxrwx   0 root         (0) root         (0)     1193 2024-04-17 09:40:45.000000 aioipfs-0.6.9/tests/test_helpers.py
```

### Comparing `aioipfs-0.6.8/LICENSE` & `aioipfs-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.8/PKG-INFO` & `aioipfs-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioipfs
-Version: 0.6.8
+Version: 0.6.9
 Summary: Asynchronous IPFS client library
 Author-email: cipres <alkaline@gmx.co.uk>
 License: LGPLv3
 Project-URL: Homepage, https://gitlab.com/cipres/aioipfs
 Keywords: asyncio,aiohttp,ipfs
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
@@ -59,15 +59,15 @@
 :info: Asynchronous IPFS_ client library
 
 **aioipfs** is a python3 library providing an asynchronous API for IPFS_.
 Supported python versions: *3.6*, *3.7*, *3.8*, *3.9*, *3.10*, *3.11*, *3.12*.
 
 This library supports the
 `RPC API specifications <https://docs.ipfs.tech/reference/kubo/rpc>`_
-for kubo_ version *0.27.0*. Unit tests are run against
+for kubo_ version *0.28.0*. Unit tests are run against
 most major go-ipfs releases and all kubo_
 releases, see the *CI* section below.
 
 See the documentation `here <https://aioipfs.readthedocs.io/en/latest>`_.
 
 .. image:: https://gitlab.com/cipres/aioipfs/badges/master/coverage.svg
 
@@ -219,15 +219,15 @@
 ==
 
 The Gitlab CI workflow runs unit tests against the following
 go-ipfs/kubo releases (`go here <https://gitlab.com/cipres/aioipfs/-/jobs>`_
 for the CI jobs overview).
 
 - go-ipfs >=0.11.0,<=0.13.0
-- kubo >=0.14.0,<=0.27.0
+- kubo >=0.14.0,<=0.28.0
 
 .. image:: https://github.com/pinnaculum/aioipfs/workflows/aioipfs-build/badge.svg
     :target: https://github.com/pinnaculum/aioipfs/actions
 
 .. image:: https://gitlab.com/cipres/aioipfs/badges/master/pipeline.svg
     :target: https://gitlab.com/cipres/aioipfs/-/jobs
```

### Comparing `aioipfs-0.6.8/README.rst` & `aioipfs-0.6.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 :info: Asynchronous IPFS_ client library
 
 **aioipfs** is a python3 library providing an asynchronous API for IPFS_.
 Supported python versions: *3.6*, *3.7*, *3.8*, *3.9*, *3.10*, *3.11*, *3.12*.
 
 This library supports the
 `RPC API specifications <https://docs.ipfs.tech/reference/kubo/rpc>`_
-for kubo_ version *0.27.0*. Unit tests are run against
+for kubo_ version *0.28.0*. Unit tests are run against
 most major go-ipfs releases and all kubo_
 releases, see the *CI* section below.
 
 See the documentation `here <https://aioipfs.readthedocs.io/en/latest>`_.
 
 .. image:: https://gitlab.com/cipres/aioipfs/badges/master/coverage.svg
 
@@ -165,15 +165,15 @@
 ==
 
 The Gitlab CI workflow runs unit tests against the following
 go-ipfs/kubo releases (`go here <https://gitlab.com/cipres/aioipfs/-/jobs>`_
 for the CI jobs overview).
 
 - go-ipfs >=0.11.0,<=0.13.0
-- kubo >=0.14.0,<=0.27.0
+- kubo >=0.14.0,<=0.28.0
 
 .. image:: https://github.com/pinnaculum/aioipfs/workflows/aioipfs-build/badge.svg
     :target: https://github.com/pinnaculum/aioipfs/actions
 
 .. image:: https://gitlab.com/cipres/aioipfs/badges/master/pipeline.svg
     :target: https://gitlab.com/cipres/aioipfs/-/jobs
```

### Comparing `aioipfs-0.6.8/aioipfs/__init__.py` & `aioipfs-0.6.9/aioipfs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.6.8'
+__version__ = '0.6.9'
 
 from yarl import URL
 from distutils.version import StrictVersion  # type: ignore
 from typing import Union
 
 import asyncio
 import aiohttp
```

### Comparing `aioipfs-0.6.8/aioipfs/api.py` & `aioipfs-0.6.9/aioipfs/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -666,15 +666,15 @@
 
         if isinstance(ipns_base, str):
             params['ipns-base'] = ipns_base
 
         return await self.fetch_json(self.url('key/list'),
                                      params=params)
 
-    async def gen(self, name, type='rsa', size: int = 2048,
+    async def gen(self, name, type='ed25519', size: int = 2048,
                   ipns_base: Optional[str] = None):
         params = {ARG_PARAM: name, 'type': type, 'size': str(size)}
 
         if isinstance(ipns_base, str):
             params['ipns-base'] = ipns_base
 
         return await self.fetch_json(self.url('key/gen'),
```

### Comparing `aioipfs-0.6.8/aioipfs/apis/__init__.py` & `aioipfs-0.6.9/aioipfs/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.8/aioipfs/apis/dag.py` & `aioipfs-0.6.9/aioipfs/apis/dag.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.8/aioipfs/apis/multibase.py` & `aioipfs-0.6.9/aioipfs/apis/multibase.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.8/aioipfs/apis/p2p.py` & `aioipfs-0.6.9/aioipfs/apis/p2p.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.8/aioipfs/apis/pin.py` & `aioipfs-0.6.9/aioipfs/apis/pin.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.8/aioipfs/apis/pubsub.py` & `aioipfs-0.6.9/aioipfs/apis/pubsub.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.8/aioipfs/apis/swarm.py` & `aioipfs-0.6.9/aioipfs/apis/swarm.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.8/aioipfs/exceptions.py` & `aioipfs-0.6.9/aioipfs/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.8/aioipfs/helpers.py` & `aioipfs-0.6.9/aioipfs/helpers.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.8/aioipfs/multi.py` & `aioipfs-0.6.9/aioipfs/multi.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.8/aioipfs/util.py` & `aioipfs-0.6.9/aioipfs/util.py`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.8/aioipfs.egg-info/PKG-INFO` & `aioipfs-0.6.9/aioipfs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioipfs
-Version: 0.6.8
+Version: 0.6.9
 Summary: Asynchronous IPFS client library
 Author-email: cipres <alkaline@gmx.co.uk>
 License: LGPLv3
 Project-URL: Homepage, https://gitlab.com/cipres/aioipfs
 Keywords: asyncio,aiohttp,ipfs
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
@@ -59,15 +59,15 @@
 :info: Asynchronous IPFS_ client library
 
 **aioipfs** is a python3 library providing an asynchronous API for IPFS_.
 Supported python versions: *3.6*, *3.7*, *3.8*, *3.9*, *3.10*, *3.11*, *3.12*.
 
 This library supports the
 `RPC API specifications <https://docs.ipfs.tech/reference/kubo/rpc>`_
-for kubo_ version *0.27.0*. Unit tests are run against
+for kubo_ version *0.28.0*. Unit tests are run against
 most major go-ipfs releases and all kubo_
 releases, see the *CI* section below.
 
 See the documentation `here <https://aioipfs.readthedocs.io/en/latest>`_.
 
 .. image:: https://gitlab.com/cipres/aioipfs/badges/master/coverage.svg
 
@@ -219,15 +219,15 @@
 ==
 
 The Gitlab CI workflow runs unit tests against the following
 go-ipfs/kubo releases (`go here <https://gitlab.com/cipres/aioipfs/-/jobs>`_
 for the CI jobs overview).
 
 - go-ipfs >=0.11.0,<=0.13.0
-- kubo >=0.14.0,<=0.27.0
+- kubo >=0.14.0,<=0.28.0
 
 .. image:: https://github.com/pinnaculum/aioipfs/workflows/aioipfs-build/badge.svg
     :target: https://github.com/pinnaculum/aioipfs/actions
 
 .. image:: https://gitlab.com/cipres/aioipfs/badges/master/pipeline.svg
     :target: https://gitlab.com/cipres/aioipfs/-/jobs
```

### Comparing `aioipfs-0.6.8/aioipfs.egg-info/SOURCES.txt` & `aioipfs-0.6.9/aioipfs.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -17,9 +17,12 @@
 aioipfs/apis/__init__.py
 aioipfs/apis/dag.py
 aioipfs/apis/multibase.py
 aioipfs/apis/p2p.py
 aioipfs/apis/pin.py
 aioipfs/apis/pubsub.py
 aioipfs/apis/swarm.py
+aioipfs/scripts/__init__.py
+aioipfs/scripts/bohort/__init__.py
+aioipfs/scripts/bohort/cli.py
 tests/test_client.py
 tests/test_helpers.py
```

### Comparing `aioipfs-0.6.8/pyproject.toml` & `aioipfs-0.6.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aioipfs-0.6.8/tests/test_client.py` & `aioipfs-0.6.9/tests/test_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -707,14 +707,21 @@
 
     @pytest.mark.asyncio
     @pytest.mark.parametrize('obj1', [b'0123456789'])
     @pytest.mark.parametrize('obj2', [b'0a1b2c3d4e5'])
     async def test_object(self, event_loop, ipfsdaemon, iclient, obj1, obj2,
                           testfile2):
         """ Unsure if this is correct """
+
+        if await iclient.agent_version_get() >= \
+                aioipfs.IpfsDaemonVersion('0.28.0'):
+            # Many of the 'object' RPC API methods are being deprecated
+            # starting with kubo v0.28.0
+            pytest.skip('This API is deprecated for this kubo version')
+
         obj1Ent = await iclient.add_bytes(obj1)
         obj2Ent = await iclient.add_bytes(obj2)
         obj = await iclient.object.new()
         r1 = await iclient.object.patch.add_link(obj['Hash'], 'obj1',
                                                  obj1Ent['Hash'])
         r2 = await iclient.object.patch.add_link(r1['Hash'], 'obj2',
                                                  obj2Ent['Hash'])
```

### Comparing `aioipfs-0.6.8/tests/test_helpers.py` & `aioipfs-0.6.9/tests/test_helpers.py`

 * *Files identical despite different names*

