# Comparing `tmp/ansar_connect-0.1.181.tar.gz` & `tmp/ansar_connect-0.1.182.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.181.tar", last modified: Wed Apr 17 04:07:46 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.182.tar", last modified: Wed Apr 17 04:39:37 2024, max compression
```

## Comparing `ansar_connect-0.1.181.tar` & `ansar_connect-0.1.182.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 04:07:46.694073 ansar_connect-0.1.181/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.181/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-17 04:07:46.694073 ansar_connect-0.1.181/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.181/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.181/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-17 04:07:46.694073 ansar_connect-0.1.181/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.181/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 04:07:46.694073 ansar_connect-0.1.181/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 04:07:46.694073 ansar_connect-0.1.181/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 04:07:46.694073 ansar_connect-0.1.181/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar_connect-0.1.181/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar_connect-0.1.181/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.181/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar_connect-0.1.181/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 04:07:46.694073 ansar_connect-0.1.181/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3063 2024-04-17 04:07:43.000000 ansar_connect-0.1.181/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14167 2024-04-15 03:23:57.000000 ansar_connect-0.1.181/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    77934 2024-04-17 02:33:18.000000 ansar_connect-0.1.181/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar_connect-0.1.181/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.181/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar_connect-0.1.181/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.181/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.181/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar_connect-0.1.181/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.181/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.181/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.181/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    33015 2024-04-13 00:35:04.000000 ansar_connect-0.1.181/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar_connect-0.1.181/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    44607 2024-04-17 04:05:42.000000 ansar_connect-0.1.181/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.181/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2171 2024-04-17 04:03:15.000000 ansar_connect-0.1.181/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.181/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar_connect-0.1.181/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 04:07:46.694073 ansar_connect-0.1.181/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-17 04:07:46.000000 ansar_connect-0.1.181/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-04-17 04:07:46.000000 ansar_connect-0.1.181/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-17 04:07:46.000000 ansar_connect-0.1.181/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-17 04:07:46.000000 ansar_connect-0.1.181/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-04-17 04:07:46.000000 ansar_connect-0.1.181/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-17 04:07:46.000000 ansar_connect-0.1.181/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 04:39:37.441123 ansar_connect-0.1.182/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.182/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-17 04:39:37.441123 ansar_connect-0.1.182/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.182/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.182/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-17 04:39:37.441123 ansar_connect-0.1.182/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.182/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 04:39:37.437123 ansar_connect-0.1.182/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 04:39:37.437123 ansar_connect-0.1.182/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 04:39:37.441123 ansar_connect-0.1.182/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar_connect-0.1.182/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar_connect-0.1.182/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.182/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar_connect-0.1.182/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 04:39:37.441123 ansar_connect-0.1.182/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3063 2024-04-17 04:39:34.000000 ansar_connect-0.1.182/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14167 2024-04-15 03:23:57.000000 ansar_connect-0.1.182/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    77934 2024-04-17 02:33:18.000000 ansar_connect-0.1.182/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar_connect-0.1.182/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.182/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar_connect-0.1.182/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.182/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.182/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar_connect-0.1.182/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.182/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.182/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.182/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    33015 2024-04-13 00:35:04.000000 ansar_connect-0.1.182/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar_connect-0.1.182/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    44744 2024-04-17 04:38:10.000000 ansar_connect-0.1.182/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.182/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2171 2024-04-17 04:03:15.000000 ansar_connect-0.1.182/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.182/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar_connect-0.1.182/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 04:39:37.441123 ansar_connect-0.1.182/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-17 04:39:37.000000 ansar_connect-0.1.182/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-04-17 04:39:37.000000 ansar_connect-0.1.182/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-17 04:39:37.000000 ansar_connect-0.1.182/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-17 04:39:37.000000 ansar_connect-0.1.182/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-04-17 04:39:37.000000 ansar_connect-0.1.182/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-17 04:39:37.000000 ansar_connect-0.1.182/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.181/LICENSE` & `ansar_connect-0.1.182/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.181/PKG-INFO` & `ansar_connect-0.1.182/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.181
+Version: 0.1.182
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.181/README.md` & `ansar_connect-0.1.182/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.181/pyproject.toml` & `ansar_connect-0.1.182/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.181/setup.py` & `ansar_connect-0.1.182/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.181/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.182/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.181/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.182/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.181/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.182/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.181/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.182/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.181/src/ansar/connect/__init__.py` & `ansar_connect-0.1.182/src/ansar/connect/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 3ad392c9dba4a1dc8263de105d613bd580925a49
-Version: 0.1.180 (2024-04-17@16:07:43+NZST)
+Commit: 2125fe63281c2da8a848f4e9d521c5096cfeae59
+Version: 0.1.181 (2024-04-17@16:39:34+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.181/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.182/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.181/src/ansar/connect/directory.py` & `ansar_connect-0.1.182/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.181/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.182/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.181/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.182/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.181/src/ansar/connect/group_if.py` & `ansar_connect-0.1.182/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.181/src/ansar/connect/grouping.py` & `ansar_connect-0.1.182/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.181/src/ansar/connect/moving.py` & `ansar_connect-0.1.182/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.181/src/ansar/connect/networking.py` & `ansar_connect-0.1.182/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.181/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.182/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.181/src/ansar/connect/node.py` & `ansar_connect-0.1.182/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.181/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.182/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.181/src/ansar/connect/procedure.py` & `ansar_connect-0.1.182/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.181/src/ansar/connect/product.py` & `ansar_connect-0.1.182/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.181/src/ansar/connect/socketry.py` & `ansar_connect-0.1.182/src/ansar/connect/socketry.py`

 * *Files 2% similar despite different names*

```diff
@@ -905,24 +905,31 @@
 		text = 'stopped "%s"(%d)' % (listening_ipp.host, listening_ipp.port)
 	else:
 		text = 'not listening to "%s"(%d)' % (listening_ipp.host, listening_ipp.port)
 	self.send(NotListening(listening_ipp, 0, text), r)
 
 def ControlChannel_HandshakeCompleted(self, control, mr):
 	m, r = mr
+	self.trace('Handshake completed')
 	h = self.handshake.pop(m.handshake_id, None)
-	if h:
-		c, n, stream = h
-		stream.handshaking = None
-		if m.private_key and m.private_key:
-			stream.encrypted = Box(m.private_key, m.public_key)
-			self.forward(c[0], c[1], c[2])
-		else:
-			n[0].error_text = m.error_text
-			self.send(n[0], n[1])
+	if h is None:
+		self.trace('Handshake unknown')
+		return
+
+	c, n, stream = h
+	stream.handshaking = None
+	if m.private_key and m.private_key:
+		self.trace('Stream encrypted')
+		stream.encrypted = Box(m.private_key, m.public_key)
+		self.forward(c[0], c[1], c[2])
+	else:
+		self.trace('Handshake failed')
+		n[0].error_text = m.error_text
+		self.send(n[0], n[1])
+
 
 def ControlChannel_Stop(self, control, mr):
 	m, r = mr
 	def soc(p): # Server or client.
 		return isinstance(p, (TcpServer, TcpClient))
 
 	# Clear any servers and clients. Not
@@ -1060,15 +1067,15 @@
 			self.trace(f'Connected (encrypted) "{connected_ipp}", requested "{request.requested_ipp}"')
 			handshake_id = uuid.uuid4()
 			not_connected = NotConnected(request.requested_ipp, None, None, request.tag)
 			self.handshake[handshake_id] = (
 				(connected, stream.controller_address, stream.remote_address),
 				(not_connected, selector.controller_address),
 				stream)
-			h = self.create(ClientHandshake, handshake_id, stream.remote_address, object_ending=no_ending)
+			h = self.create(ClientHandshake, handshake_id, proxy_address, object_ending=no_ending)
 			stream.handshaking = h
 		else:
 			self.forward(connected, stream.controller_address, stream.remote_address)
 
 		if not scrap:
 			# Immediate shutdown. Need to
 			# generate the full set of messages.
@@ -1116,15 +1123,15 @@
 		self.trace(f'Connected (encrypted) "{connected_ipp}", requested "{request.requested_ipp}"')
 		handshake_id = uuid.uuid4()
 		not_connected = NotConnected(request.requested_ipp, None, None, request.tag)
 		self.handshake[handshake_id] = (
 			(connected, stream.controller_address, stream.remote_address),
 			(not_connected, selector.controller_address),
 			stream)
-		h = self.create(ClientHandshake, handshake_id, stream.remote_address, object_ending=no_ending)
+		h = self.create(ClientHandshake, handshake_id, proxy_address, object_ending=no_ending)
 		stream.handshaking = h
 		return
 
 	self.forward(connected, stream.controller_address, stream.remote_address)
 
 def TcpClient_BrokenTransport(self, selector, s):
 	text = 'fault on pending connect, unreachable, no service at that address or blocked'
@@ -1426,52 +1433,52 @@
 	self.complete()
 
 ar.bind(SocketSelect, (ar.Start,))
 
 #
 #
 class ServerHandshake(ar.Point, ar.StateMachine):
-	def __init__(self, accepted_id):
+	def __init__(self, handshake_id):
 		ar.Point.__init__(self)
 		ar.StateMachine.__init__(self, INITIAL)
-		self.accepted_id = accepted_id
+		self.handshake_id = handshake_id
 		self.private_key = None
 
 def ServerHandshake_INITIAL_Start(self, message):
 	self.private_key = PrivateKey.generate()
 	self.start(ar.T1, seconds=4.0)
 	return PENDING
 
 def ServerHandshake_PENDING_Blob(self, message):
 	# Got the clients public key.
 	# Respond with our own.
 	public_key = self.private_key.public_key
 	public_blob = Blob(public_key.encode())
 	self.reply(public_blob)
 
-	handshake = HandshakeCompleted(handshake_id=self.accepted_id,
+	handshake = HandshakeCompleted(handshake_id=self.handshake_id,
 		private_key=self.private_key, public_key=PublicKey(message.block))
 	ts.channel.send(handshake, self.address)
 	self.complete()
 
 def ServerHandshake_PENDING_Unknown(self, message):
 	t = ar.tof(message)
-	handshake = HandshakeCompleted(handshake_id=self.accepted_id,
+	handshake = HandshakeCompleted(handshake_id=self.handshake_id,
 		error_text=f'unexpected "{t}"')
 	ts.channel.send(handshake, self.address)
 	self.complete()
 
 def ServerHandshake_PENDING_T1(self, message):
-	handshake = HandshakeCompleted(handshake_id=self.accepted_id,
+	handshake = HandshakeCompleted(handshake_id=self.handshake_id,
 		error_text=f'timed out')
 	ts.channel.send(handshake, self.address)
 	self.complete()
 
 def ServerHandshake_PENDING_Stop(self, message):
-	handshake = HandshakeCompleted(handshake_id=self.accepted_id,
+	handshake = HandshakeCompleted(handshake_id=self.handshake_id,
 		error_text=f'aborted')
 	ts.channel.send(handshake, self.address)
 	self.complete()
 
 SERVER_HANDSHAKE_DISPATCH = {
 	INITIAL: (
 		(ar.Start,), ()
@@ -1481,52 +1488,52 @@
 	),
 }
 
 ar.bind(ServerHandshake, SERVER_HANDSHAKE_DISPATCH)
 
 
 class ClientHandshake(ar.Point, ar.StateMachine):
-	def __init__(self, connected_id, remote_address):
+	def __init__(self, handshake_id, remote_address):
 		ar.Point.__init__(self)
 		ar.StateMachine.__init__(self, INITIAL)
-		self.connected_id = connected_id
+		self.handshake_id = handshake_id
 		self.remote_address = remote_address
 		self.private_key = None
 
 def ClientHandshake_INITIAL_Start(self, message):
 	self.private_key = PrivateKey.generate()
 	public_key = self.private_key.public_key
 	public_blob = Blob(public_key.encode())
 	self.send(public_blob, self.remote_address)
 	self.start(ar.T1, seconds=4.0)
 	return PENDING
 
 def ClientHandshake_PENDING_Blob(self, message):
 	# Sent our public key.
 	# Expecting one from remote.
-	handshake = HandshakeCompleted(handshake_id=self.connected_id,
+	handshake = HandshakeCompleted(handshake_id=self.handshake_id,
 		private_key=self.private_key, public_key=PublicKey(message.block))
 	ts.channel.send(handshake, self.address)
 	self.complete()
 
 def ClientHandshake_PENDING_Unknown(self, message):
 	t = ar.tof(message)
-	handshake = HandshakeCompleted(handshake_id=self.connected_id,
+	handshake = HandshakeCompleted(handshake_id=self.handshake_id,
 		error_text=f'unexpected "{t}"')
 	ts.channel.send(handshake, self.address)
 	self.complete()
 
 def ClientHandshake_PENDING_T1(self, message):
-	handshake = HandshakeCompleted(handshake_id=self.connected_id,
+	handshake = HandshakeCompleted(handshake_id=self.handshake_id,
 		error_text=f'timed out')
 	ts.channel.send(handshake, self.address)
 	self.complete()
 
 def ClientHandshake_PENDING_Stop(self, message):
-	handshake = HandshakeCompleted(handshake_id=self.connected_id,
+	handshake = HandshakeCompleted(handshake_id=self.handshake_id,
 		error_text=f'aborted')
 	ts.channel.send(handshake, self.address)
 	self.complete()
 
 CLIENT_HANDSHAKE_DISPATCH = {
 	INITIAL: (
 		(ar.Start,), ()
```

### Comparing `ansar_connect-0.1.181/src/ansar/connect/standard.py` & `ansar_connect-0.1.182/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.181/src/ansar/connect/transporting.py` & `ansar_connect-0.1.182/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.181/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.182/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.181/src/ansar/connect/wan.py` & `ansar_connect-0.1.182/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.181/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.182/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.181
+Version: 0.1.182
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.181/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.182/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

