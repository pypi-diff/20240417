# Comparing `tmp/ansar_connect-0.1.186.tar.gz` & `tmp/ansar_connect-0.1.187.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.186.tar", last modified: Wed Apr 17 08:15:00 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.187.tar", last modified: Wed Apr 17 14:34:04 2024, max compression
```

## Comparing `ansar_connect-0.1.186.tar` & `ansar_connect-0.1.187.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 08:15:00.145707 ansar_connect-0.1.186/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.186/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-17 08:15:00.145707 ansar_connect-0.1.186/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.186/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.186/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-17 08:15:00.145707 ansar_connect-0.1.186/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.186/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 08:15:00.145707 ansar_connect-0.1.186/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 08:15:00.145707 ansar_connect-0.1.186/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 08:15:00.145707 ansar_connect-0.1.186/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar_connect-0.1.186/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar_connect-0.1.186/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.186/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar_connect-0.1.186/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 08:15:00.145707 ansar_connect-0.1.186/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3063 2024-04-17 08:14:56.000000 ansar_connect-0.1.186/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14167 2024-04-15 03:23:57.000000 ansar_connect-0.1.186/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    77934 2024-04-17 02:33:18.000000 ansar_connect-0.1.186/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar_connect-0.1.186/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.186/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar_connect-0.1.186/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.186/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.186/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar_connect-0.1.186/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.186/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.186/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.186/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    33015 2024-04-13 00:35:04.000000 ansar_connect-0.1.186/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar_connect-0.1.186/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    44807 2024-04-17 08:09:33.000000 ansar_connect-0.1.186/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.186/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2171 2024-04-17 04:03:15.000000 ansar_connect-0.1.186/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.186/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar_connect-0.1.186/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 08:15:00.145707 ansar_connect-0.1.186/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-17 08:15:00.000000 ansar_connect-0.1.186/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-04-17 08:15:00.000000 ansar_connect-0.1.186/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-17 08:15:00.000000 ansar_connect-0.1.186/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-17 08:15:00.000000 ansar_connect-0.1.186/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-04-17 08:15:00.000000 ansar_connect-0.1.186/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-17 08:15:00.000000 ansar_connect-0.1.186/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 14:34:04.304067 ansar_connect-0.1.187/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.187/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-17 14:34:04.304067 ansar_connect-0.1.187/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.187/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.187/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-17 14:34:04.304067 ansar_connect-0.1.187/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.187/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 14:34:04.300068 ansar_connect-0.1.187/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 14:34:04.300068 ansar_connect-0.1.187/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 14:34:04.304067 ansar_connect-0.1.187/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar_connect-0.1.187/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar_connect-0.1.187/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.187/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar_connect-0.1.187/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 14:34:04.304067 ansar_connect-0.1.187/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3063 2024-04-17 14:34:01.000000 ansar_connect-0.1.187/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14167 2024-04-15 03:23:57.000000 ansar_connect-0.1.187/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    77934 2024-04-17 02:33:18.000000 ansar_connect-0.1.187/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar_connect-0.1.187/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.187/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar_connect-0.1.187/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.187/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.187/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar_connect-0.1.187/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.187/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.187/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.187/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    33015 2024-04-13 00:35:04.000000 ansar_connect-0.1.187/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar_connect-0.1.187/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    40927 2024-04-17 14:33:18.000000 ansar_connect-0.1.187/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.187/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2171 2024-04-17 04:03:15.000000 ansar_connect-0.1.187/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.187/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar_connect-0.1.187/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 14:34:04.304067 ansar_connect-0.1.187/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-17 14:34:04.000000 ansar_connect-0.1.187/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-04-17 14:34:04.000000 ansar_connect-0.1.187/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-17 14:34:04.000000 ansar_connect-0.1.187/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-17 14:34:04.000000 ansar_connect-0.1.187/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-04-17 14:34:04.000000 ansar_connect-0.1.187/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-17 14:34:04.000000 ansar_connect-0.1.187/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.186/LICENSE` & `ansar_connect-0.1.187/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.186/PKG-INFO` & `ansar_connect-0.1.187/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.186
+Version: 0.1.187
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.186/README.md` & `ansar_connect-0.1.187/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.186/pyproject.toml` & `ansar_connect-0.1.187/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.186/setup.py` & `ansar_connect-0.1.187/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.186/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.187/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.186/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.187/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.186/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.187/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.186/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.187/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.186/src/ansar/connect/__init__.py` & `ansar_connect-0.1.187/src/ansar/connect/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: ccffe0b77c820aaafa527cb02b50872e754c4df8
-Version: 0.1.185 (2024-04-17@20:14:56+NZST)
+Commit: 22a3a704c5044589b0a193ed5547f6695656bbba
+Version: 0.1.186 (2024-04-18@02:34:01+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.186/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.187/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.186/src/ansar/connect/directory.py` & `ansar_connect-0.1.187/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.186/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.187/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.186/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.187/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.186/src/ansar/connect/group_if.py` & `ansar_connect-0.1.187/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.186/src/ansar/connect/grouping.py` & `ansar_connect-0.1.187/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.186/src/ansar/connect/moving.py` & `ansar_connect-0.1.187/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.186/src/ansar/connect/networking.py` & `ansar_connect-0.1.187/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.186/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.187/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.186/src/ansar/connect/node.py` & `ansar_connect-0.1.187/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.186/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.187/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.186/src/ansar/connect/procedure.py` & `ansar_connect-0.1.187/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.186/src/ansar/connect/product.py` & `ansar_connect-0.1.187/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.186/src/ansar/connect/socketry.py` & `ansar_connect-0.1.187/src/ansar/connect/socketry.py`

 * *Files 7% similar despite different names*

```diff
@@ -448,18 +448,18 @@
 				continue
 			if self.byte_part is self.byte_body:
 				self.analysis_state = 1
 				self.size_digits.clear()
 				self.jump_size = 0
 				self.byte_part = self.byte_space
 				continue
-			if self.encrypted:
-				h = self.encrypted.decrypt(self.byte_header)
-				b_ = self.encrypted.decrypt(self.byte_body)
-				s = self.encrypted.decrypt(self.byte_space)
+			if self.key_box:
+				h = self.key_box.decrypt(self.byte_header)
+				b_ = self.key_box.decrypt(self.byte_body)
+				s = self.key_box.decrypt(self.byte_space)
 				yield h, b_, s
 			else:
 				yield self.byte_header, self.byte_body, self.byte_space
 			self.analysis_state = 1
 			self.size_digits.clear()
 			self.jump_size = 0
 			# Ownership passed with yield. Make new
@@ -499,65 +499,78 @@
 		encrypted = self.encrypted
 		while len(encoded_bytes) < TCP_SEND:
 			if len(self.messages_to_encode) == 0:
 				added = self.drain(self.messages_to_encode)
 				if added == 0:
 					break
 			m, t, r = self.messages_to_encode.popleft()
-			f = isinstance(m, Blob)
+			f = False
+			if isinstance(m, Diffie):
+				self.private_key = PrivateKey.generate()
+				public_key = self.private_key.public_key.encode()
+				m.public_key = bytearray(public_key)
+			elif isinstance(m, Hellman):
+				self.private_key = PrivateKey.generate()
+				shared_key = m.public_key
+				self.key_box = Box(self.private_key, shared_key)
+				public_key = self.private_key.public_key.encode()
+				m.public_key = bytearray(public_key)
+			elif isinstance(m, Blob):
+				f = True
+			key_box = self.key_box
 			h = Header(t, r, f)
 			e = codec.encode(h, HEADING)
 			e = e.encode('utf-8')
-			if encrypted:
-				e = encrypted.encrypt(e)
+			if key_box:
+				e = key_box.encrypt(e)
 			n = len(e)
 			# Stream the header
 			encoded_bytes += str(n).encode('ascii')
 			encoded_bytes += b'\n'
 			encoded_bytes += e
 			encoded_bytes += b'\n'
 			# Then a tunnelled bock, relay or normal message.
 			if f:
 				e = m.block
-				if encrypted:
-					e = encrypted.encrypt(e)
+				if key_box:
+					e = key_box.encrypt(e)
 				n = len(e)
 				encoded_bytes += str(n).encode('ascii')
 				encoded_bytes += b'\n'
 				encoded_bytes += e
 				encoded_bytes += b'\n'
 				# Tunnel block contains no addresses
 				# Could just assign '[]' (an empty JSON list)
 				s = codec.encode([], SPACE)
 			elif isinstance(m, Relay):
 				e = m.block
-				if encrypted:
-					e = encrypted.encrypt(e)
+				if key_box:
+					e = key_box.encrypt(e)
 				n = len(e)
 				encoded_bytes += str(n).encode('ascii')
 				encoded_bytes += b'\n'
 				encoded_bytes += e
 				encoded_bytes += b'\n'
 				s = codec.encode(m.space, SPACE)
 			else:
 				space = []
 				e = codec.encode(m, ar.Any(), space=space)
 				e = e.encode('utf-8')
-				if encrypted:
-					e = encrypted.encrypt(e)
+				if key_box:
+					e = key_box.encrypt(e)
 				n = len(e)
 				encoded_bytes += str(n).encode('ascii')
 				encoded_bytes += b'\n'
 				encoded_bytes += e
 				encoded_bytes += b'\n'
 				s = codec.encode(space, SPACE)
 			# And lastly, the mutated section.
 			e = s.encode('utf-8')
-			if encrypted:
-				e = encrypted.encrypt(e)
+			if key_box:
+				e = key_box.encrypt(e)
 			n = len(e)
 			encoded_bytes += str(n).encode('ascii')
 			encoded_bytes += b'\n'
 			encoded_bytes += e
 			encoded_bytes += b'\n'
 		return len(encoded_bytes)
 
@@ -571,16 +584,17 @@
 		self.upgrade = upgrade
 		self.opened = opened
 		self.tag = tag
 		self.closing = False
 		self.value = None
 		self.codec = None
 		self.encoded_bytes = bytearray()
-		self.encrypted = None
-		self.handshaking = None
+		self.diffie_hellman = None
+		self.private_key = None
+		self.key_box = None
 
 	def routing(self, return_proxy, local_termination, remote_address):
 		# Define addresses for message forwarding.
 		# return_proxy ........ address that response should go back to.
 		# local_termination ... address of default target, actor or session.
 		# remote_address ...... source address of connection updates, session or proxy.
 		self.codec = ar.CodecJson(return_proxy=return_proxy, local_termination=local_termination)
@@ -591,31 +605,37 @@
 			s = h.decode('utf-8')
 			header, v = self.codec.decode(s, HEADING)
 			if v is not None:
 				raise ValueError(f'header with unexpected versioning "{v}"')
 			s = a.decode('utf-8')
 			space, v = self.codec.decode(s, SPACE)
 
-			to_address = self.handshaking or header.to_address
+			to_address = header.to_address
 
 			if header.tunnel:
 				sockets.forward(Blob(b_), to_address, header.return_address)
 				continue
 			elif len(header.to_address) > 1:
 				sockets.forward(Relay(b_, space), to_address, header.return_address)
 				continue
 
 			s = b_.decode('utf-8')
 			body, v = self.codec.decode(s, ar.Any(), space=space)
 			if v is not None:
 				if not self.upgrade:
 					raise ValueError(f'body version "{v}" and no upgrade')
 				body = self.upgrade(body, v)
-			
-			sockets.forward(body, to_address, header.return_address)
+
+			if isinstance(body, Diffie):
+				sockets.send(Hellman(body.public_key), self.remote_address)
+			elif isinstance(body, Hellman):
+				h = self.diffie_hellman[0]
+				sockets.forward(h[0], h[1], h[2])
+			else:
+				sockets.forward(body, to_address, header.return_address)
 
 	def send_a_block(self, s):
 		t = self.best_block(self.encoded_bytes, self.codec)
 		if t == 0:
 			return False
 		n = t if t <= TCP_SEND else TCP_SEND
 		chunk = self.encoded_bytes[:n]
@@ -668,29 +688,28 @@
 	),
 }
 
 ar.bind(SocketProxy, TCP_PROXY_DISPATCH)
 
 #
 #
-class HandshakeCompleted(object):
-	def __init__(self, handshake_id=None, private_key=None, public_key=None, error_text=None):
-		self.handshake_id = handshake_id
-		self.private_key = private_key
+class Diffie(object):
+	def __init__(self, public_key=None):
 		self.public_key = public_key
-		self.error_text = error_text
 
-HANDSHAKE_SCHEMA = {
-	'handshake_id': ar.UUID(),
-	'private_key': ar.Any(),
-	'public_key': ar.Any(),
-	'error_text': ar.Unicode(),
+class Hellman(object):
+	def __init__(self, public_key=None):
+		self.public_key = public_key
+
+DH_SCHEMA = {
+	'public_key': ar.Block(),
 }
 
-ar.bind(HandshakeCompleted, object_schema=HANDSHAKE_SCHEMA, copy_before_sending=False)
+ar.bind(Diffie, object_schema=DH_SCHEMA, copy_before_sending=False)
+ar.bind(Hellman, object_schema=DH_SCHEMA, copy_before_sending=False)
 
 
 
 # Signals from the network represented
 # as distinct classes - for dispatching.
 class ReceiveBlock: pass
 class ReadyToSend: pass
@@ -751,15 +770,15 @@
 		server.close()
 		self.send(NotListening(requested_ipp, 0, str(e), m.tag), r)
 		return
 
 	hap = server.getsockname()
 
 	if isinstance(m.encrypted, TlsServer):
-		self.trace(f'Encrypting listen as TLS server "{m.encrypted.certificate_file}"')
+		self.trace(f'Listening (encrypted) as TLS server "{m.encrypted.certificate_file}"')
 
 	self.trace('Listening on "%s"(%d), requested "%s"(%d)' %
 		(hap[0], hap[1],
 		requested_ipp.host, requested_ipp.port))
 	listening = Listening(requested_ipp=requested_ipp, listening_ipp=HostPort(hap[0], hap[1]), tag=m.tag, context=m.encrypted)
 
 	self.networking[server] = TcpServer(server, m, listening, r, m.upgrade)
@@ -871,22 +890,19 @@
 	self.networking[client] = stream
 	self.receiving.append(client)
 	self.sending.append(client)
 	self.faulting.append(client)
 
 	if m.encrypted:
 		self.trace(f'Connected (encrypted) "{connected_ipp}", requested "{m.requested_ipp}"')
-		handshake_id = uuid.uuid4()
 		not_connected = NotConnected(requested_ipp, None, None, m.tag)
-		self.handshake[handshake_id] = (
+		stream.diffie_hellman = (
 			(connected, r, stream.remote_address),
-			(not_connected, r),
-			stream)
-		h = self.create(ClientHandshake, handshake_id, proxy_address, object_ending=no_ending)
-		stream.handshaking = h
+			(not_connected, r))
+		self.send(Diffie(), proxy_address)
 		return
 
 	self.forward(connected, r, stream.remote_address)
 
 def ControlChannel_StopListening(self, control, mr):
 	m, r = mr
 	listening_ipp = m.listening_ipp
@@ -903,34 +919,14 @@
 	if len(sockets) == 1:
 		self.clear(sockets[0], TcpServer)
 		text = 'stopped "%s"(%d)' % (listening_ipp.host, listening_ipp.port)
 	else:
 		text = 'not listening to "%s"(%d)' % (listening_ipp.host, listening_ipp.port)
 	self.send(NotListening(listening_ipp, 0, text), r)
 
-def ControlChannel_HandshakeCompleted(self, control, mr):
-	m, r = mr
-	self.trace('Handshake completed')
-	h = self.handshake.pop(m.handshake_id, None)
-	if h is None:
-		self.trace('Handshake unknown')
-		return
-
-	c, n, stream = h
-	stream.handshaking = None
-	if m.private_key and m.private_key:
-		self.trace('Stream encrypted')
-		stream.encrypted = Box(m.private_key, m.public_key)
-		self.forward(c[0], c[1], c[2])
-	else:
-		self.trace('Handshake failed')
-		n[0].error_text = m.error_text
-		self.send(n[0], n[1])
-
-
 def ControlChannel_Stop(self, control, mr):
 	m, r = mr
 	def soc(p): # Server or client.
 		return isinstance(p, (TcpServer, TcpClient))
 
 	# Clear any servers and clients. Not
 	# accepting or connecting any more.
@@ -1000,23 +996,19 @@
 
 	accepted = Accepted(listening_ipp=listening.listening_ipp,
 		accepted_ipp=accepted_ipp, remote_address=stream.remote_address,
 		opened_at=opened_at, tag=listening.tag)
 	stream.opened = accepted
 
 	if listening.context:
-		self.trace(f'Accepted (encrypted) "{accepted_ipp}", listening at "{listening.listening_ipp}"')
-		handshake_id = uuid.uuid4()
+		self.trace(f'Accepted (encrypted) "{accepted_ipp}", requested "{listening.listening_ipp}"')
 		not_accepted = NotAccepted(listening.requested_ipp, None, None, listening.tag)
-		self.handshake[handshake_id] = (
-			(accepted, server.controller_address, stream.remote_address),
-			(not_accepted, server.controller_address),
-			stream)
-		h = self.create(ServerHandshake, handshake_id, object_ending=no_ending)
-		stream.handshaking = h
+		stream.diffie_hellman = (
+			(accepted, stream.controller_address, stream.remote_address),
+			(not_accepted, server.controller_address))
 		return
 
 	self.trace(f'Accepted "{accepted_ipp}", listening at "{listening.listening_ipp}"')
 
 	self.forward(accepted, server.controller_address, stream.remote_address)
 
 def TcpServer_BrokenTransport(self, server, s):
@@ -1061,24 +1053,21 @@
 
 		self.trace( 'Connected to "%s"(%d), at local address "%s"(%d)' %
 					   (request.requested_ipp.host, request.requested_ipp.port,
 					   hap[0], hap[1]))
 
 		if selector.encrypted:
 			self.trace(f'Connected (encrypted) "{connected_ipp}", requested "{request.requested_ipp}"')
-			handshake_id = uuid.uuid4()
 			not_connected = NotConnected(request.requested_ipp, None, None, request.tag)
-			self.handshake[handshake_id] = (
+			stream.diffie_hellman = (
 				(connected, stream.controller_address, stream.remote_address),
-				(not_connected, selector.controller_address),
-				stream)
-			h = self.create(ClientHandshake, handshake_id, proxy_address, object_ending=no_ending)
-			stream.handshaking = h
-		else:
-			self.forward(connected, stream.controller_address, stream.remote_address)
+				(not_connected, selector.controller_address))
+			self.send(Diffie(), proxy_address)
+			return
+		self.forward(connected, stream.controller_address, stream.remote_address)
 
 		if not scrap:
 			# Immediate shutdown. Need to
 			# generate the full set of messages.
 			#self.clear(s, TcpStream)
 			return
 
@@ -1117,22 +1106,19 @@
 	stream, proxy_address = open_stream(self, selector, client, connected)
 	connected.remote_address = proxy_address
 	#receiving.append( client)
 	#self.faulting.append( client)
 
 	if selector.encrypted:
 		self.trace(f'Connected (encrypted) "{connected_ipp}", requested "{request.requested_ipp}"')
-		handshake_id = uuid.uuid4()
 		not_connected = NotConnected(request.requested_ipp, None, None, request.tag)
-		self.handshake[handshake_id] = (
+		stream.diffie_hellman = (
 			(connected, stream.controller_address, stream.remote_address),
-			(not_connected, selector.controller_address),
-			stream)
-		h = self.create(ClientHandshake, handshake_id, proxy_address, object_ending=no_ending)
-		stream.handshaking = h
+			(not_connected, selector.controller_address))
+		self.send(Diffie(), proxy_address)
 		return
 
 	self.forward(connected, stream.controller_address, stream.remote_address)
 
 def TcpClient_BrokenTransport(self, selector, s):
 	text = 'fault on pending connect, unreachable, no service at that address or blocked'
 	self.send(NotConnected(selector.requested_ipp, 0, text, selector.tag), selector.controller_address)
@@ -1279,15 +1265,14 @@
 	(ControlChannel, ReceiveBlock):	 ControlChannel_ReceiveBlock,		# Signals down the control channel.
 	(ControlChannel, BrokenTransport):  ControlChannel_BrokenTransport,
 
 	# Made to look as if the select thread can actually receive
 	# sockets signals and application messages. Called from above.
 	(ControlChannel, ListenForStream):  ControlChannel_ListenForStream,		# Process signals to sockets.
 	(ControlChannel, ConnectStream):	ControlChannel_ConnectStream,
-	(ControlChannel, HandshakeCompleted):	ControlChannel_HandshakeCompleted,
 	(ControlChannel, Shutdown):		 ControlChannel_Shutdown,
 	(ControlChannel, Bump):			 ControlChannel_Bump,
 	(ControlChannel, StopListening):	ControlChannel_StopListening,
 	(ControlChannel, ar.Stop):		  ControlChannel_Stop,
 
 	# Operational sockets
 	(TcpServer,	ReceiveBlock):	   TcpServer_ReceiveBlock,			# Accept inbound connections.
@@ -1323,17 +1308,14 @@
 		self.receiving = [self.accepted]
 		self.sending = []
 		self.faulting = self.receiving + self.sending
 
 		# Live.
 		self.running = True
 
-		# Encryption.
-		self.handshake = {}
-
 	def clear(self, s, expected=None):
 		# Remove the specified socket from operations.
 		try:
 			t = self.networking[s]
 		except KeyError:
 			self.warning('Attempt to remove unknown socket')
 			return None
@@ -1429,123 +1411,7 @@
 				continue
 			j(self, a, f)
 
 	control_close(self.lac)
 	self.complete()
 
 ar.bind(SocketSelect, (ar.Start,))
-
-#
-#
-class ServerHandshake(ar.Point, ar.StateMachine):
-	def __init__(self, handshake_id):
-		ar.Point.__init__(self)
-		ar.StateMachine.__init__(self, INITIAL)
-		self.handshake_id = handshake_id
-		self.private_key = None
-
-def ServerHandshake_INITIAL_Start(self, message):
-	self.private_key = PrivateKey.generate()
-	self.start(ar.T1, seconds=4.0)
-	return PENDING
-
-def ServerHandshake_PENDING_Blob(self, message):
-	# Got the clients public key.
-	# Respond with our own.
-	public_key = self.private_key.public_key
-	public_blob = Blob(public_key.encode())
-	self.reply(public_blob)
-
-	b = bytes(message.block)
-	public_key=PublicKey(b)
-
-	handshake = HandshakeCompleted(handshake_id=self.handshake_id,
-		private_key=self.private_key, public_key=public_key)
-	ts.channel.send(handshake, self.address)
-	self.complete()
-
-def ServerHandshake_PENDING_Unknown(self, message):
-	t = ar.tof(message)
-	handshake = HandshakeCompleted(handshake_id=self.handshake_id,
-		error_text=f'unexpected "{t}"')
-	ts.channel.send(handshake, self.address)
-	self.complete()
-
-def ServerHandshake_PENDING_T1(self, message):
-	handshake = HandshakeCompleted(handshake_id=self.handshake_id,
-		error_text=f'timed out')
-	ts.channel.send(handshake, self.address)
-	self.complete()
-
-def ServerHandshake_PENDING_Stop(self, message):
-	handshake = HandshakeCompleted(handshake_id=self.handshake_id,
-		error_text=f'aborted')
-	ts.channel.send(handshake, self.address)
-	self.complete()
-
-SERVER_HANDSHAKE_DISPATCH = {
-	INITIAL: (
-		(ar.Start,), ()
-	),
-	PENDING: (
-		(Blob, ar.Unknown, ar.T1, ar.Stop), ()
-	),
-}
-
-ar.bind(ServerHandshake, SERVER_HANDSHAKE_DISPATCH)
-
-
-class ClientHandshake(ar.Point, ar.StateMachine):
-	def __init__(self, handshake_id, remote_address):
-		ar.Point.__init__(self)
-		ar.StateMachine.__init__(self, INITIAL)
-		self.handshake_id = handshake_id
-		self.remote_address = remote_address
-		self.private_key = None
-
-def ClientHandshake_INITIAL_Start(self, message):
-	self.private_key = PrivateKey.generate()
-	public_key = self.private_key.public_key
-	public_blob = Blob(public_key.encode())
-	self.send(public_blob, self.remote_address)
-	self.start(ar.T1, seconds=4.0)
-	return PENDING
-
-def ClientHandshake_PENDING_Blob(self, message):
-	# Sent our public key.
-	# Expecting one from remote.
-	b = bytes(message.block)
-	public_key = PublicKey(b)
-	handshake = HandshakeCompleted(handshake_id=self.handshake_id,
-		private_key=self.private_key, public_key=public_key)
-	ts.channel.send(handshake, self.address)
-	self.complete()
-
-def ClientHandshake_PENDING_Unknown(self, message):
-	t = ar.tof(message)
-	handshake = HandshakeCompleted(handshake_id=self.handshake_id,
-		error_text=f'unexpected "{t}"')
-	ts.channel.send(handshake, self.address)
-	self.complete()
-
-def ClientHandshake_PENDING_T1(self, message):
-	handshake = HandshakeCompleted(handshake_id=self.handshake_id,
-		error_text=f'timed out')
-	ts.channel.send(handshake, self.address)
-	self.complete()
-
-def ClientHandshake_PENDING_Stop(self, message):
-	handshake = HandshakeCompleted(handshake_id=self.handshake_id,
-		error_text=f'aborted')
-	ts.channel.send(handshake, self.address)
-	self.complete()
-
-CLIENT_HANDSHAKE_DISPATCH = {
-	INITIAL: (
-		(ar.Start,), ()
-	),
-	PENDING: (
-		(Blob, ar.Unknown, ar.T1, ar.Stop), ()
-	),
-}
-
-ar.bind(ClientHandshake, CLIENT_HANDSHAKE_DISPATCH)
```

### Comparing `ansar_connect-0.1.186/src/ansar/connect/standard.py` & `ansar_connect-0.1.187/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.186/src/ansar/connect/transporting.py` & `ansar_connect-0.1.187/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.186/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.187/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.186/src/ansar/connect/wan.py` & `ansar_connect-0.1.187/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.186/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.187/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.186
+Version: 0.1.187
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.186/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.187/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

