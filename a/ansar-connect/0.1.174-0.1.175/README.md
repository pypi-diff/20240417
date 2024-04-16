# Comparing `tmp/ansar_connect-0.1.174.tar.gz` & `tmp/ansar_connect-0.1.175.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.174.tar", last modified: Tue Apr 16 16:29:53 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.175.tar", last modified: Tue Apr 16 16:45:06 2024, max compression
```

## Comparing `ansar_connect-0.1.174.tar` & `ansar_connect-0.1.175.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-16 16:29:53.913399 ansar_connect-0.1.174/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.174/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-16 16:29:53.913399 ansar_connect-0.1.174/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.174/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      723 2024-04-16 08:58:45.000000 ansar_connect-0.1.174/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-16 16:29:53.913399 ansar_connect-0.1.174/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2210 2024-04-16 08:58:37.000000 ansar_connect-0.1.174/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-16 16:29:53.909399 ansar_connect-0.1.174/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-16 16:29:53.909399 ansar_connect-0.1.174/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-16 16:29:53.909399 ansar_connect-0.1.174/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar_connect-0.1.174/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar_connect-0.1.174/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.174/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar_connect-0.1.174/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-16 16:29:53.909399 ansar_connect-0.1.174/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3055 2024-04-16 16:29:50.000000 ansar_connect-0.1.174/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14167 2024-04-15 03:23:57.000000 ansar_connect-0.1.174/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    78025 2024-04-13 03:14:49.000000 ansar_connect-0.1.174/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar_connect-0.1.174/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.174/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar_connect-0.1.174/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.174/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.174/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar_connect-0.1.174/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.174/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.174/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.174/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    33015 2024-04-13 00:35:04.000000 ansar_connect-0.1.174/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar_connect-0.1.174/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    43236 2024-04-16 16:25:57.000000 ansar_connect-0.1.174/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.174/src/ansar/connect/standard.py
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2205 2024-04-14 02:42:33.000000 ansar_connect-0.1.174/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar_connect-0.1.174/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-16 16:29:53.913399 ansar_connect-0.1.174/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     2674 2024-04-16 16:29:53.000000 ansar_connect-0.1.174/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-16 16:29:53.000000 ansar_connect-0.1.174/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-16 16:29:53.000000 ansar_connect-0.1.174/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-16 16:29:53.000000 ansar_connect-0.1.174/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       21 2024-04-16 16:29:53.000000 ansar_connect-0.1.174/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-16 16:29:53.000000 ansar_connect-0.1.174/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-16 16:45:06.321336 ansar_connect-0.1.175/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.175/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-16 16:45:06.321336 ansar_connect-0.1.175/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     1966 2023-06-28 15:55:38.000000 ansar_connect-0.1.175/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-04-16 16:44:47.000000 ansar_connect-0.1.175/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-04-16 16:45:06.321336 ansar_connect-0.1.175/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-04-16 16:44:25.000000 ansar_connect-0.1.175/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-16 16:45:06.317336 ansar_connect-0.1.175/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-16 16:45:06.317336 ansar_connect-0.1.175/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-16 16:45:06.317336 ansar_connect-0.1.175/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14522 2024-04-12 09:29:14.000000 ansar_connect-0.1.175/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3441 2024-04-12 14:58:30.000000 ansar_connect-0.1.175/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.175/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9054 2024-04-12 15:15:53.000000 ansar_connect-0.1.175/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-16 16:45:06.321336 ansar_connect-0.1.175/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3055 2024-04-16 16:45:03.000000 ansar_connect-0.1.175/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14167 2024-04-15 03:23:57.000000 ansar_connect-0.1.175/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    78025 2024-04-13 03:14:49.000000 ansar_connect-0.1.175/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     7752 2024-04-01 20:33:07.000000 ansar_connect-0.1.175/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9979 2024-04-02 12:37:04.000000 ansar_connect-0.1.175/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2168 2024-04-11 23:23:48.000000 ansar_connect-0.1.175/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14174 2024-03-01 03:02:47.000000 ansar_connect-0.1.175/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.175/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    21087 2024-04-06 01:12:06.000000 ansar_connect-0.1.175/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.175/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34999 2024-03-23 01:59:51.000000 ansar_connect-0.1.175/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.175/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    33015 2024-04-13 00:35:04.000000 ansar_connect-0.1.175/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2372 2024-04-12 15:15:53.000000 ansar_connect-0.1.175/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    43236 2024-04-16 16:25:57.000000 ansar_connect-0.1.175/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.175/src/ansar/connect/standard.py
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2205 2024-04-14 02:42:33.000000 ansar_connect-0.1.175/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6532 2024-04-13 00:17:21.000000 ansar_connect-0.1.175/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-04-16 16:45:06.321336 ansar_connect-0.1.175/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     2731 2024-04-16 16:45:06.000000 ansar_connect-0.1.175/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      984 2024-04-16 16:45:06.000000 ansar_connect-0.1.175/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-04-16 16:45:06.000000 ansar_connect-0.1.175/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-04-16 16:45:06.000000 ansar_connect-0.1.175/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-04-16 16:45:06.000000 ansar_connect-0.1.175/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-04-16 16:45:06.000000 ansar_connect-0.1.175/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.174/LICENSE` & `ansar_connect-0.1.175/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.174/PKG-INFO` & `ansar_connect-0.1.175/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.174
+Version: 0.1.175
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cffi>=1.16.0
+Requires-Dist: PyNaCl>=1.5.0
 Requires-Dist: ansar-create>=0.1.76
 
 # ansar-connect
 
 The **ansar-connect** library implements sophisticated asynchronous network messaging. It builds
 on the features of the `ansar-encode <https://pypi.org/project/ansar-encode>`_
 and `ansar-create <https://pypi.org/project/ansar-create>`_ libraries to integrate network
```

### Comparing `ansar_connect-0.1.174/README.md` & `ansar_connect-0.1.175/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.174/pyproject.toml` & `ansar_connect-0.1.175/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -18,12 +18,14 @@
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
 	"Operating System :: OS Independent",
 	"Topic :: Software Development :: Libraries"
 ]
 dynamic = ["description", "version", "scripts"]
 dependencies = [
+    "cffi>=1.16.0",
+    "PyNaCl>=1.5.0",
     "ansar-create>=0.1.76"
 ]
 
 [project.urls]
 Documentation = "https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html"
```

### Comparing `ansar_connect-0.1.174/setup.py` & `ansar_connect-0.1.175/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,14 +35,16 @@
     long_description = f.read()
 
 with open("DOC_LATEST_LINK", "r", encoding="utf-8") as f:
     d = f.read()
 DOC_LINK = d[:-1]
 
 REQUIRES = [
+    "cffi>=1.16.0",
+    "PyNaCl>=1.5.0",
     "ansar-create>=0.1.76",
 ]
 
 setuptools.setup(
     name=PACKAGE,
     version=VERSION,
     author="Scott Woods",
```

### Comparing `ansar_connect-0.1.174/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.175/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.174/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.175/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.174/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.175/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.174/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.175/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.174/src/ansar/connect/__init__.py` & `ansar_connect-0.1.175/src/ansar/connect/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 71acdc9df29564d2947a91a7c438821d70422466
-Version: 0.1.173 (2024-04-17@04:29:50+NZST)
+Commit: 9949292802730e967e78ae52b5ef59c48b5c7bd5
+Version: 0.1.174 (2024-04-17@04:45:03+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.174/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.175/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.174/src/ansar/connect/directory.py` & `ansar_connect-0.1.175/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.174/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.175/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.174/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.175/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.174/src/ansar/connect/group_if.py` & `ansar_connect-0.1.175/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.174/src/ansar/connect/grouping.py` & `ansar_connect-0.1.175/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.174/src/ansar/connect/moving.py` & `ansar_connect-0.1.175/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.174/src/ansar/connect/networking.py` & `ansar_connect-0.1.175/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.174/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.175/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.174/src/ansar/connect/node.py` & `ansar_connect-0.1.175/src/ansar/connect/node.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.174/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.175/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.174/src/ansar/connect/procedure.py` & `ansar_connect-0.1.175/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.174/src/ansar/connect/product.py` & `ansar_connect-0.1.175/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.174/src/ansar/connect/socketry.py` & `ansar_connect-0.1.175/src/ansar/connect/socketry.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.174/src/ansar/connect/standard.py` & `ansar_connect-0.1.175/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.174/src/ansar/connect/transporting.py` & `ansar_connect-0.1.175/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.174/src/ansar/connect/wan.py` & `ansar_connect-0.1.175/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.174/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.175/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.174
+Version: 0.1.175
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cffi>=1.16.0
+Requires-Dist: PyNaCl>=1.5.0
 Requires-Dist: ansar-create>=0.1.76
 
 # ansar-connect
 
 The **ansar-connect** library implements sophisticated asynchronous network messaging. It builds
 on the features of the `ansar-encode <https://pypi.org/project/ansar-encode>`_
 and `ansar-create <https://pypi.org/project/ansar-create>`_ libraries to integrate network
```

### Comparing `ansar_connect-0.1.174/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.175/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

