# Comparing `tmp/ansar_connect-0.1.180.tar.gz` & `tmp/ansar_connect-0.1.181.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.180.tar", last modified: Wed Apr 17 03:13:15 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.181.tar", last modified: Wed Apr 17 04:07:46 2024, max compression
```

## Comparing `ansar_connect-0.1.180.tar` & `ansar_connect-0.1.181.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 03:13:15.531877 ansar_connect-0.1.180/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.180/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-17 03:13:15.531877 ansar_connect-0.1.180/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.180/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.180/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-17 03:13:15.531877 ansar_connect-0.1.180/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.180/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 03:13:15.527877 ansar_connect-0.1.180/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 03:13:15.527877 ansar_connect-0.1.180/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 03:13:15.527877 ansar_connect-0.1.180/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar_connect-0.1.180/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar_connect-0.1.180/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.180/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar_connect-0.1.180/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 03:13:15.531877 ansar_connect-0.1.180/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3063 2024-04-17 03:13:12.000000 ansar_connect-0.1.180/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14167 2024-04-15 03:23:57.000000 ansar_connect-0.1.180/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    77934 2024-04-17 02:33:18.000000 ansar_connect-0.1.180/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar_connect-0.1.180/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.180/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar_connect-0.1.180/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.180/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.180/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar_connect-0.1.180/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.180/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.180/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.180/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    33015 2024-04-13 00:35:04.000000 ansar_connect-0.1.180/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar_connect-0.1.180/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    44462 2024-04-17 03:11:32.000000 ansar_connect-0.1.180/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.180/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2310 2024-04-16 22:48:33.000000 ansar_connect-0.1.180/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar_connect-0.1.180/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 03:13:15.531877 ansar_connect-0.1.180/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-17 03:13:15.000000 ansar_connect-0.1.180/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-17 03:13:15.000000 ansar_connect-0.1.180/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-17 03:13:15.000000 ansar_connect-0.1.180/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-17 03:13:15.000000 ansar_connect-0.1.180/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-04-17 03:13:15.000000 ansar_connect-0.1.180/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-17 03:13:15.000000 ansar_connect-0.1.180/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 04:07:46.694073 ansar_connect-0.1.181/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.181/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-17 04:07:46.694073 ansar_connect-0.1.181/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.181/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.181/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-17 04:07:46.694073 ansar_connect-0.1.181/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.181/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 04:07:46.694073 ansar_connect-0.1.181/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 04:07:46.694073 ansar_connect-0.1.181/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 04:07:46.694073 ansar_connect-0.1.181/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar_connect-0.1.181/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar_connect-0.1.181/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.181/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar_connect-0.1.181/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 04:07:46.694073 ansar_connect-0.1.181/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3063 2024-04-17 04:07:43.000000 ansar_connect-0.1.181/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14167 2024-04-15 03:23:57.000000 ansar_connect-0.1.181/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    77934 2024-04-17 02:33:18.000000 ansar_connect-0.1.181/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar_connect-0.1.181/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.181/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar_connect-0.1.181/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.181/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.181/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar_connect-0.1.181/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.181/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.181/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.181/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    33015 2024-04-13 00:35:04.000000 ansar_connect-0.1.181/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar_connect-0.1.181/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    44607 2024-04-17 04:05:42.000000 ansar_connect-0.1.181/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.181/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2171 2024-04-17 04:03:15.000000 ansar_connect-0.1.181/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.181/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar_connect-0.1.181/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 04:07:46.694073 ansar_connect-0.1.181/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-17 04:07:46.000000 ansar_connect-0.1.181/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-04-17 04:07:46.000000 ansar_connect-0.1.181/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-17 04:07:46.000000 ansar_connect-0.1.181/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-17 04:07:46.000000 ansar_connect-0.1.181/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-04-17 04:07:46.000000 ansar_connect-0.1.181/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-17 04:07:46.000000 ansar_connect-0.1.181/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.180/LICENSE` & `ansar_connect-0.1.181/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.180/PKG-INFO` & `ansar_connect-0.1.181/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.180
+Version: 0.1.181
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.180/README.md` & `ansar_connect-0.1.181/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.180/pyproject.toml` & `ansar_connect-0.1.181/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.180/setup.py` & `ansar_connect-0.1.181/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.180/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.181/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.180/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.181/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.180/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.181/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.180/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.181/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.180/src/ansar/connect/__init__.py` & `ansar_connect-0.1.181/src/ansar/connect/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: cb5e057ef1617f475aa9790c3404be19a4d6370a
-Version: 0.1.179 (2024-04-17@15:13:12+NZST)
+Commit: 3ad392c9dba4a1dc8263de105d613bd580925a49
+Version: 0.1.180 (2024-04-17@16:07:43+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.180/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.181/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.180/src/ansar/connect/directory.py` & `ansar_connect-0.1.181/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.180/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.181/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.180/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.181/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.180/src/ansar/connect/group_if.py` & `ansar_connect-0.1.181/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.180/src/ansar/connect/grouping.py` & `ansar_connect-0.1.181/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.180/src/ansar/connect/moving.py` & `ansar_connect-0.1.181/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.180/src/ansar/connect/networking.py` & `ansar_connect-0.1.181/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.180/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.181/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.180/src/ansar/connect/node.py` & `ansar_connect-0.1.181/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.180/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.181/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.180/src/ansar/connect/procedure.py` & `ansar_connect-0.1.181/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.180/src/ansar/connect/product.py` & `ansar_connect-0.1.181/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.180/src/ansar/connect/socketry.py` & `ansar_connect-0.1.181/src/ansar/connect/socketry.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 import socket
 import select
 import re
 import uuid
 import nacl.utils
 from nacl.public import PrivateKey, PublicKey, Box
 import ansar.create as ar
+from .transporting_if import ts
 
 from copy import copy
 
 __all__ = [
 	'HostPort',
 	'LocalPort',
 	'ScopeOfIP',
@@ -684,14 +685,15 @@
 	'public_key': ar.Any(),
 	'error_text': ar.Unicode(),
 }
 
 ar.bind(HandshakeCompleted, object_schema=HANDSHAKE_SCHEMA, copy_before_sending=False)
 
 
+
 # Signals from the network represented
 # as distinct classes - for dispatching.
 class ReceiveBlock: pass
 class ReadyToSend: pass
 class BrokenTransport: pass
 
 # CONTROL CHANNEL
@@ -1444,34 +1446,34 @@
 	# Respond with our own.
 	public_key = self.private_key.public_key
 	public_blob = Blob(public_key.encode())
 	self.reply(public_blob)
 
 	handshake = HandshakeCompleted(handshake_id=self.accepted_id,
 		private_key=self.private_key, public_key=PublicKey(message.block))
-	ar.wrench(self, handshake)
+	ts.channel.send(handshake, self.address)
 	self.complete()
 
 def ServerHandshake_PENDING_Unknown(self, message):
 	t = ar.tof(message)
 	handshake = HandshakeCompleted(handshake_id=self.accepted_id,
 		error_text=f'unexpected "{t}"')
-	ar.wrench(self, handshake)
+	ts.channel.send(handshake, self.address)
 	self.complete()
 
 def ServerHandshake_PENDING_T1(self, message):
 	handshake = HandshakeCompleted(handshake_id=self.accepted_id,
 		error_text=f'timed out')
-	ar.wrench(self, handshake)
+	ts.channel.send(handshake, self.address)
 	self.complete()
 
 def ServerHandshake_PENDING_Stop(self, message):
 	handshake = HandshakeCompleted(handshake_id=self.accepted_id,
 		error_text=f'aborted')
-	ar.wrench(self, handshake)
+	ts.channel.send(handshake, self.address)
 	self.complete()
 
 SERVER_HANDSHAKE_DISPATCH = {
 	INITIAL: (
 		(ar.Start,), ()
 	),
 	PENDING: (
@@ -1499,34 +1501,34 @@
 	return PENDING
 
 def ClientHandshake_PENDING_Blob(self, message):
 	# Sent our public key.
 	# Expecting one from remote.
 	handshake = HandshakeCompleted(handshake_id=self.connected_id,
 		private_key=self.private_key, public_key=PublicKey(message.block))
-	ar.wrench(self, handshake)
+	ts.channel.send(handshake, self.address)
 	self.complete()
 
 def ClientHandshake_PENDING_Unknown(self, message):
 	t = ar.tof(message)
 	handshake = HandshakeCompleted(handshake_id=self.connected_id,
 		error_text=f'unexpected "{t}"')
-	ar.wrench(self, handshake)
+	ts.channel.send(handshake, self.address)
 	self.complete()
 
 def ClientHandshake_PENDING_T1(self, message):
 	handshake = HandshakeCompleted(handshake_id=self.connected_id,
 		error_text=f'timed out')
-	ar.wrench(self, handshake)
+	ts.channel.send(handshake, self.address)
 	self.complete()
 
 def ClientHandshake_PENDING_Stop(self, message):
 	handshake = HandshakeCompleted(handshake_id=self.connected_id,
 		error_text=f'aborted')
-	ar.wrench(self, handshake)
+	ts.channel.send(handshake, self.address)
 	self.complete()
 
 CLIENT_HANDSHAKE_DISPATCH = {
 	INITIAL: (
 		(ar.Start,), ()
 	),
 	PENDING: (
```

### Comparing `ansar_connect-0.1.180/src/ansar/connect/standard.py` & `ansar_connect-0.1.181/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.180/src/ansar/connect/transporting.py` & `ansar_connect-0.1.181/src/ansar/connect/transporting.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,53 +20,44 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 __docformat__ = 'restructuredtext'
 
 import ansar.create as ar
 from .socketry import *
+from .transporting_if import ts
 
 __all__ = [
-	'wrench',
 	'connect',
 	'listen',
 	'stop_listen',
 ]
 
-sockets = None
-channel = None
-
 def create_sockets(root):
-	global sockets, channel
-	sockets = root.create(SocketSelect)
-	channel = root.select(SocketChannel)
+	ts.sockets = root.create(SocketSelect)
+	ts.channel = root.select(SocketChannel)
 
 def stop_sockets(root):
-	global sockets, channel
-	channel.send(ar.Stop(), root.address)
+	ts.channel.send(ar.Stop(), root.address)
 	root.select(ar.Completed)
 
 ar.AddOn(create_sockets, stop_sockets)
 
 #
 #
 def wrench(self, message):
-	global sockets, channel
-	channel.send(message, self.address)
+	ts.channel.send(message, self.address)
 
 #
 #
 def connect(self, requested_ipp, session=None, tag=None, encrypted=None):
-	global sockets, channel
-	channel.send(ConnectStream(requested_ipp=requested_ipp, create_session=session, tag=tag, encrypted=encrypted), self.address)
+	ts.channel.send(ConnectStream(requested_ipp=requested_ipp, create_session=session, tag=tag, encrypted=encrypted), self.address)
 
 #
 #
 def listen(self, requested_ipp, session=None, tag=None, encrypted=None):
-	global sockets, channel
-	channel.send(ListenForStream(requested_ipp=requested_ipp, create_session=session, tag=tag, encrypted=encrypted), self.address)
+	ts.channel.send(ListenForStream(requested_ipp=requested_ipp, create_session=session, tag=tag, encrypted=encrypted), self.address)
 
 #
 #
 def stop_listen(self, requested_ipp):
-	global sockets, channel
-	channel.send(StopListening(requested_ipp), self.address)
+	ts.channel.send(StopListening(requested_ipp), self.address)
```

### Comparing `ansar_connect-0.1.180/src/ansar/connect/wan.py` & `ansar_connect-0.1.181/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.180/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.181/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.180
+Version: 0.1.181
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.180/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.181/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 src/ansar/connect/node.py
 src/ansar/connect/plumbing.py
 src/ansar/connect/procedure.py
 src/ansar/connect/product.py
 src/ansar/connect/socketry.py
 src/ansar/connect/standard.py
 src/ansar/connect/transporting.py
+src/ansar/connect/transporting_if.py
 src/ansar/connect/wan.py
 src/ansar_connect.egg-info/PKG-INFO
 src/ansar_connect.egg-info/SOURCES.txt
 src/ansar_connect.egg-info/dependency_links.txt
 src/ansar_connect.egg-info/entry_points.txt
 src/ansar_connect.egg-info/requires.txt
 src/ansar_connect.egg-info/top_level.txt
```

