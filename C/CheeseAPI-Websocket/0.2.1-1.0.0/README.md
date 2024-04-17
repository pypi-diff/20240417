# Comparing `tmp/cheeseapi_websocket-0.2.1.tar.gz` & `tmp/cheeseapi_websocket-1.0.0.tar.gz`

## Comparing `cheeseapi_websocket-0.2.1.tar` & `cheeseapi_websocket-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 cheeseapi_websocket-0.2.1/CheeseAPI_Websocket/__init__.py
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 cheeseapi_websocket-0.2.1/CheeseAPI_Websocket/handle.py
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 cheeseapi_websocket-0.2.1/CheeseAPI_Websocket/websocket.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cheeseapi_websocket-0.2.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi_websocket-0.2.1/LICENSE
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 cheeseapi_websocket-0.2.1/README.md
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 cheeseapi_websocket-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 cheeseapi_websocket-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.0/CheeseAPI_Websocket/__init__.py
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.0/CheeseAPI_Websocket/handle.py
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.0/CheeseAPI_Websocket/websocket.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.0/README.md
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.0/PKG-INFO
```

### Comparing `cheeseapi_websocket-0.2.1/CheeseAPI_Websocket/handle.py` & `cheeseapi_websocket-1.0.0/CheeseAPI_Websocket/handle.py`

 * *Files identical despite different names*

### Comparing `cheeseapi_websocket-0.2.1/CheeseAPI_Websocket/websocket.py` & `cheeseapi_websocket-1.0.0/CheeseAPI_Websocket/websocket.py`

 * *Files identical despite different names*

### Comparing `cheeseapi_websocket-0.2.1/LICENSE` & `cheeseapi_websocket-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cheeseapi_websocket-0.2.1/README.md` & `cheeseapi_websocket-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cheeseapi_websocket-0.2.1/pyproject.toml` & `cheeseapi_websocket-1.0.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = [ "hatchling" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "CheeseAPI_Websocket"
-version = "0.2.1"
+version = "1.0.0"
 description = "一款基于CheeseAPI的升级款Websocket插件。"
 readme = "README.md"
 license-files = { paths = [ "LICENSE" ] }
 authors = [
     { name = "Cheese Unknown", email = "cheese@cheese.ren" }
 ]
 keywords = [ 'websocket' ]
 
 dependencies = [
-    "CheeseAPI",
+    "CheeseAPI==1.0.*",
     "redis"
 ]
 
 [project.urls]
 Source = "https://github.com/CheeseUnknown/CheeseAPI_Websocket"
 
 [tool.hatch.build.targets.sdist]
```

### Comparing `cheeseapi_websocket-0.2.1/PKG-INFO` & `cheeseapi_websocket-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.3
 Name: CheeseAPI_Websocket
-Version: 0.2.1
+Version: 1.0.0
 Summary: 一款基于CheeseAPI的升级款Websocket插件。
 Project-URL: Source, https://github.com/CheeseUnknown/CheeseAPI_Websocket
 Author-email: Cheese Unknown <cheese@cheese.ren>
 License-File: LICENSE
 Keywords: websocket
-Requires-Dist: cheeseapi
+Requires-Dist: cheeseapi==1.0.*
 Requires-Dist: redis
 Description-Content-Type: text/markdown
 
 # **CheeseAPI_Websocket**
 
 ## **介绍**
```

