# Comparing `tmp/ansar_connect-0.1.187.tar.gz` & `tmp/ansar_connect-0.1.189.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.187.tar", last modified: Wed Apr 17 14:34:04 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.189.tar", last modified: Wed Apr 17 14:42:23 2024, max compression
```

## Comparing `ansar_connect-0.1.187.tar` & `ansar_connect-0.1.189.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 14:34:04.304067 ansar_connect-0.1.187/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.187/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-17 14:34:04.304067 ansar_connect-0.1.187/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.187/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.187/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-17 14:34:04.304067 ansar_connect-0.1.187/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.187/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 14:34:04.300068 ansar_connect-0.1.187/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 14:34:04.300068 ansar_connect-0.1.187/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 14:34:04.304067 ansar_connect-0.1.187/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar_connect-0.1.187/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar_connect-0.1.187/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.187/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar_connect-0.1.187/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 14:34:04.304067 ansar_connect-0.1.187/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3063 2024-04-17 14:34:01.000000 ansar_connect-0.1.187/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14167 2024-04-15 03:23:57.000000 ansar_connect-0.1.187/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    77934 2024-04-17 02:33:18.000000 ansar_connect-0.1.187/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar_connect-0.1.187/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.187/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar_connect-0.1.187/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.187/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.187/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar_connect-0.1.187/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.187/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.187/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.187/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    33015 2024-04-13 00:35:04.000000 ansar_connect-0.1.187/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar_connect-0.1.187/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    40927 2024-04-17 14:33:18.000000 ansar_connect-0.1.187/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.187/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2171 2024-04-17 04:03:15.000000 ansar_connect-0.1.187/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.187/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar_connect-0.1.187/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 14:34:04.304067 ansar_connect-0.1.187/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-17 14:34:04.000000 ansar_connect-0.1.187/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-04-17 14:34:04.000000 ansar_connect-0.1.187/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-17 14:34:04.000000 ansar_connect-0.1.187/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-17 14:34:04.000000 ansar_connect-0.1.187/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-04-17 14:34:04.000000 ansar_connect-0.1.187/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-17 14:34:04.000000 ansar_connect-0.1.187/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 14:42:23.744345 ansar_connect-0.1.189/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.189/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-17 14:42:23.744345 ansar_connect-0.1.189/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.189/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.189/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-17 14:42:23.744345 ansar_connect-0.1.189/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.189/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 14:42:23.740345 ansar_connect-0.1.189/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 14:42:23.740345 ansar_connect-0.1.189/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 14:42:23.740345 ansar_connect-0.1.189/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar_connect-0.1.189/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar_connect-0.1.189/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.189/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar_connect-0.1.189/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 14:42:23.744345 ansar_connect-0.1.189/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3063 2024-04-17 14:42:20.000000 ansar_connect-0.1.189/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14167 2024-04-15 03:23:57.000000 ansar_connect-0.1.189/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    77934 2024-04-17 02:33:18.000000 ansar_connect-0.1.189/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar_connect-0.1.189/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.189/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar_connect-0.1.189/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.189/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.189/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar_connect-0.1.189/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.189/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.189/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.189/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    33015 2024-04-13 00:35:04.000000 ansar_connect-0.1.189/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar_connect-0.1.189/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    41017 2024-04-17 14:41:24.000000 ansar_connect-0.1.189/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.189/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2171 2024-04-17 04:03:15.000000 ansar_connect-0.1.189/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.189/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar_connect-0.1.189/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 14:42:23.744345 ansar_connect-0.1.189/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-17 14:42:23.000000 ansar_connect-0.1.189/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-04-17 14:42:23.000000 ansar_connect-0.1.189/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-17 14:42:23.000000 ansar_connect-0.1.189/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-17 14:42:23.000000 ansar_connect-0.1.189/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-04-17 14:42:23.000000 ansar_connect-0.1.189/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-17 14:42:23.000000 ansar_connect-0.1.189/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.187/LICENSE` & `ansar_connect-0.1.189/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.187/PKG-INFO` & `ansar_connect-0.1.189/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.187
+Version: 0.1.189
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.187/README.md` & `ansar_connect-0.1.189/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.187/pyproject.toml` & `ansar_connect-0.1.189/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.187/setup.py` & `ansar_connect-0.1.189/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.187/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.189/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.187/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.189/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.187/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.189/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.187/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.189/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.187/src/ansar/connect/__init__.py` & `ansar_connect-0.1.189/src/ansar/connect/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 22a3a704c5044589b0a193ed5547f6695656bbba
-Version: 0.1.186 (2024-04-18@02:34:01+NZST)
+Commit: e654784dbf24a807627603fc55d1e33f4df3d25f
+Version: 0.1.188 (2024-04-18@02:42:20+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.187/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.189/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.187/src/ansar/connect/directory.py` & `ansar_connect-0.1.189/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.187/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.189/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.187/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.189/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.187/src/ansar/connect/group_if.py` & `ansar_connect-0.1.189/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.187/src/ansar/connect/grouping.py` & `ansar_connect-0.1.189/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.187/src/ansar/connect/moving.py` & `ansar_connect-0.1.189/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.187/src/ansar/connect/networking.py` & `ansar_connect-0.1.189/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.187/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.189/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.187/src/ansar/connect/node.py` & `ansar_connect-0.1.189/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.187/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.189/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.187/src/ansar/connect/procedure.py` & `ansar_connect-0.1.189/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.187/src/ansar/connect/product.py` & `ansar_connect-0.1.189/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.187/src/ansar/connect/socketry.py` & `ansar_connect-0.1.189/src/ansar/connect/socketry.py`

 * *Files 0% similar despite different names*

```diff
@@ -492,15 +492,15 @@
 			a.extend(self.pending)
 			self.pending = []
 		finally:
 			self.lock.release()
 		return count
 
 	def best_block(self, encoded_bytes, codec):
-		encrypted = self.encrypted
+		key_box = self.key_box
 		while len(encoded_bytes) < TCP_SEND:
 			if len(self.messages_to_encode) == 0:
 				added = self.drain(self.messages_to_encode)
 				if added == 0:
 					break
 			m, t, r = self.messages_to_encode.popleft()
 			f = False
@@ -508,19 +508,19 @@
 				self.private_key = PrivateKey.generate()
 				public_key = self.private_key.public_key.encode()
 				m.public_key = bytearray(public_key)
 			elif isinstance(m, Hellman):
 				self.private_key = PrivateKey.generate()
 				shared_key = m.public_key
 				self.key_box = Box(self.private_key, shared_key)
+				key_box = self.key_box
 				public_key = self.private_key.public_key.encode()
 				m.public_key = bytearray(public_key)
 			elif isinstance(m, Blob):
 				f = True
-			key_box = self.key_box
 			h = Header(t, r, f)
 			e = codec.encode(h, HEADING)
 			e = e.encode('utf-8')
 			if key_box:
 				e = key_box.encrypt(e)
 			n = len(e)
 			# Stream the header
@@ -624,14 +624,16 @@
 				if not self.upgrade:
 					raise ValueError(f'body version "{v}" and no upgrade')
 				body = self.upgrade(body, v)
 
 			if isinstance(body, Diffie):
 				sockets.send(Hellman(body.public_key), self.remote_address)
 			elif isinstance(body, Hellman):
+				shared_key = bytes(body.public_key)
+				self.key_box = Box(self.private_key, shared_key)
 				h = self.diffie_hellman[0]
 				sockets.forward(h[0], h[1], h[2])
 			else:
 				sockets.forward(body, to_address, header.return_address)
 
 	def send_a_block(self, s):
 		t = self.best_block(self.encoded_bytes, self.codec)
```

### Comparing `ansar_connect-0.1.187/src/ansar/connect/standard.py` & `ansar_connect-0.1.189/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.187/src/ansar/connect/transporting.py` & `ansar_connect-0.1.189/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.187/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.189/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.187/src/ansar/connect/wan.py` & `ansar_connect-0.1.189/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.187/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.189/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.187
+Version: 0.1.189
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.187/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.189/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

