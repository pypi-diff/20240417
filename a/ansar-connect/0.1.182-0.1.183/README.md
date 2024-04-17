# Comparing `tmp/ansar_connect-0.1.182.tar.gz` & `tmp/ansar_connect-0.1.183.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.182.tar", last modified: Wed Apr 17 04:39:37 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.183.tar", last modified: Wed Apr 17 06:02:56 2024, max compression
```

## Comparing `ansar_connect-0.1.182.tar` & `ansar_connect-0.1.183.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 04:39:37.441123 ansar_connect-0.1.182/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.182/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-17 04:39:37.441123 ansar_connect-0.1.182/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.182/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.182/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-17 04:39:37.441123 ansar_connect-0.1.182/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.182/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 04:39:37.437123 ansar_connect-0.1.182/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 04:39:37.437123 ansar_connect-0.1.182/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 04:39:37.441123 ansar_connect-0.1.182/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar_connect-0.1.182/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar_connect-0.1.182/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.182/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar_connect-0.1.182/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 04:39:37.441123 ansar_connect-0.1.182/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3063 2024-04-17 04:39:34.000000 ansar_connect-0.1.182/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14167 2024-04-15 03:23:57.000000 ansar_connect-0.1.182/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    77934 2024-04-17 02:33:18.000000 ansar_connect-0.1.182/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar_connect-0.1.182/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.182/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar_connect-0.1.182/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.182/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.182/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar_connect-0.1.182/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.182/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.182/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.182/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    33015 2024-04-13 00:35:04.000000 ansar_connect-0.1.182/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar_connect-0.1.182/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    44744 2024-04-17 04:38:10.000000 ansar_connect-0.1.182/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.182/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2171 2024-04-17 04:03:15.000000 ansar_connect-0.1.182/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.182/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar_connect-0.1.182/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 04:39:37.441123 ansar_connect-0.1.182/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-17 04:39:37.000000 ansar_connect-0.1.182/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-04-17 04:39:37.000000 ansar_connect-0.1.182/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-17 04:39:37.000000 ansar_connect-0.1.182/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-17 04:39:37.000000 ansar_connect-0.1.182/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-04-17 04:39:37.000000 ansar_connect-0.1.182/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-17 04:39:37.000000 ansar_connect-0.1.182/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 06:02:56.623139 ansar_connect-0.1.183/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.183/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-17 06:02:56.623139 ansar_connect-0.1.183/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.183/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.183/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-17 06:02:56.623139 ansar_connect-0.1.183/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.183/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 06:02:56.619139 ansar_connect-0.1.183/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 06:02:56.619139 ansar_connect-0.1.183/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 06:02:56.619139 ansar_connect-0.1.183/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar_connect-0.1.183/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar_connect-0.1.183/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.183/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar_connect-0.1.183/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 06:02:56.623139 ansar_connect-0.1.183/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3063 2024-04-17 06:02:53.000000 ansar_connect-0.1.183/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14167 2024-04-15 03:23:57.000000 ansar_connect-0.1.183/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    77934 2024-04-17 02:33:18.000000 ansar_connect-0.1.183/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar_connect-0.1.183/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.183/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar_connect-0.1.183/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.183/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.183/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar_connect-0.1.183/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.183/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.183/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.183/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    33015 2024-04-13 00:35:04.000000 ansar_connect-0.1.183/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar_connect-0.1.183/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    44844 2024-04-17 06:01:48.000000 ansar_connect-0.1.183/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.183/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2171 2024-04-17 04:03:15.000000 ansar_connect-0.1.183/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.183/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar_connect-0.1.183/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-17 06:02:56.623139 ansar_connect-0.1.183/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-17 06:02:56.000000 ansar_connect-0.1.183/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-04-17 06:02:56.000000 ansar_connect-0.1.183/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-17 06:02:56.000000 ansar_connect-0.1.183/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-17 06:02:56.000000 ansar_connect-0.1.183/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-04-17 06:02:56.000000 ansar_connect-0.1.183/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-17 06:02:56.000000 ansar_connect-0.1.183/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.182/LICENSE` & `ansar_connect-0.1.183/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.182/PKG-INFO` & `ansar_connect-0.1.183/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.182
+Version: 0.1.183
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.182/README.md` & `ansar_connect-0.1.183/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.182/pyproject.toml` & `ansar_connect-0.1.183/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.182/setup.py` & `ansar_connect-0.1.183/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.182/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.183/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.182/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.183/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.182/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.183/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.182/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.183/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.182/src/ansar/connect/__init__.py` & `ansar_connect-0.1.183/src/ansar/connect/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 2125fe63281c2da8a848f4e9d521c5096cfeae59
-Version: 0.1.181 (2024-04-17@16:39:34+NZST)
+Commit: 710176a123de5b0021f71d4a0a3921859bc57873
+Version: 0.1.182 (2024-04-17@18:02:53+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.182/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.183/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.182/src/ansar/connect/directory.py` & `ansar_connect-0.1.183/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.182/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.183/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.182/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.183/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.182/src/ansar/connect/group_if.py` & `ansar_connect-0.1.183/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.182/src/ansar/connect/grouping.py` & `ansar_connect-0.1.183/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.182/src/ansar/connect/moving.py` & `ansar_connect-0.1.183/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.182/src/ansar/connect/networking.py` & `ansar_connect-0.1.183/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.182/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.183/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.182/src/ansar/connect/node.py` & `ansar_connect-0.1.183/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.182/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.183/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.182/src/ansar/connect/procedure.py` & `ansar_connect-0.1.183/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.182/src/ansar/connect/product.py` & `ansar_connect-0.1.183/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.182/src/ansar/connect/socketry.py` & `ansar_connect-0.1.183/src/ansar/connect/socketry.py`

 * *Files 1% similar despite different names*

```diff
@@ -988,17 +988,14 @@
 		accepted.setblocking(False)
 	except socket.error as e:
 		self.send(NotAccepted(listening.requested_ipp, e.errno, str(e), listening.tag), server.controller_address)
 		return
 
 	opened_at = ar.world_now()
 	stream, proxy_address = open_stream(self, server, accepted, None)
-	self.receiving.append(accepted)
-	self.sending.append(accepted)
-	self.faulting.append(accepted)
 
 	accepted_ipp = HostPort(hap[0], hap[1])
 
 	accepted = Accepted(listening_ipp=listening.listening_ipp,
 		accepted_ipp=accepted_ipp, remote_address=stream.remote_address,
 		opened_at=opened_at, tag=listening.tag)
 	stream.opened = accepted
@@ -1009,16 +1006,23 @@
 		not_accepted = NotAccepted(listening.requested_ipp, None, None, listening.tag)
 		self.handshake[handshake_id] = (
 			(accepted, server.controller_address, stream.remote_address),
 			(not_accepted, server.controller_address),
 			stream)
 		h = self.create(ServerHandshake, handshake_id, object_ending=no_ending)
 		stream.handshaking = h
+		self.receiving.append(accepted)
+		self.sending.append(accepted)
+		self.faulting.append(accepted)
 		return
 
+	self.receiving.append(accepted)
+	self.sending.append(accepted)
+	self.faulting.append(accepted)
+
 	self.trace(f'Accepted "{accepted_ipp}", listening at "{listening.listening_ipp}"')
 
 	self.forward(accepted, server.controller_address, stream.remote_address)
 
 def TcpServer_BrokenTransport(self, server, s):
 	listening = server.listening
 	self.send(NotListening(listening.listening_ipp, 0, "signaled by networking subsystem"), server.controller_address)
```

### Comparing `ansar_connect-0.1.182/src/ansar/connect/standard.py` & `ansar_connect-0.1.183/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.182/src/ansar/connect/transporting.py` & `ansar_connect-0.1.183/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.182/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.183/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.182/src/ansar/connect/wan.py` & `ansar_connect-0.1.183/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.182/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.183/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.182
+Version: 0.1.183
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.182/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.183/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

