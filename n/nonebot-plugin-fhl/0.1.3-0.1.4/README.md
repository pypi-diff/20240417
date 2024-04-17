# Comparing `tmp/nonebot_plugin_fhl-0.1.3.tar.gz` & `tmp/nonebot_plugin_fhl-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_fhl-0.1.3.tar", last modified: Wed Apr 17 10:14:09 2024, max compression
+gzip compressed data, was "nonebot_plugin_fhl-0.1.4.tar", last modified: Wed Apr 17 10:16:50 2024, max compression
```

## Comparing `nonebot_plugin_fhl-0.1.3.tar` & `nonebot_plugin_fhl-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2024-04-17 10:13:54.329829 nonebot_plugin_fhl-0.1.3/LICENSE
--rw-r--r--   0        0        0       21 2024-04-17 10:13:54.329829 nonebot_plugin_fhl-0.1.3/README.md
--rw-r--r--   0        0        0     1354 2024-04-17 10:14:09.701938 nonebot_plugin_fhl-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4820 2024-04-17 10:13:54.329829 nonebot_plugin_fhl-0.1.3/src/nonebot_plugin_fhl/__init__.py
--rw-r--r--   0        0        0     1069 2024-04-17 10:13:54.329829 nonebot_plugin_fhl-0.1.3/src/nonebot_plugin_fhl/api.py
--rw-r--r--   0        0        0      265 2024-04-17 10:13:54.329829 nonebot_plugin_fhl-0.1.3/src/nonebot_plugin_fhl/config.py
--rw-r--r--   0        0        0      808 2024-04-17 10:13:54.329829 nonebot_plugin_fhl-0.1.3/src/nonebot_plugin_fhl/logic.py
--rw-r--r--   0        0        0     1195 2024-04-17 10:13:54.329829 nonebot_plugin_fhl-0.1.3/src/nonebot_plugin_fhl/model.py
--rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 nonebot_plugin_fhl-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-17 10:16:30.891071 nonebot_plugin_fhl-0.1.4/LICENSE
+-rw-r--r--   0        0        0       21 2024-04-17 10:16:30.891071 nonebot_plugin_fhl-0.1.4/README.md
+-rw-r--r--   0        0        0     1360 2024-04-17 10:16:50.019054 nonebot_plugin_fhl-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4820 2024-04-17 10:16:30.895071 nonebot_plugin_fhl-0.1.4/src/nonebot_plugin_fhl/__init__.py
+-rw-r--r--   0        0        0     1069 2024-04-17 10:16:30.895071 nonebot_plugin_fhl-0.1.4/src/nonebot_plugin_fhl/api.py
+-rw-r--r--   0        0        0      266 2024-04-17 10:16:30.895071 nonebot_plugin_fhl-0.1.4/src/nonebot_plugin_fhl/config.py
+-rw-r--r--   0        0        0      808 2024-04-17 10:16:30.895071 nonebot_plugin_fhl-0.1.4/src/nonebot_plugin_fhl/logic.py
+-rw-r--r--   0        0        0     1195 2024-04-17 10:16:30.895071 nonebot_plugin_fhl-0.1.4/src/nonebot_plugin_fhl/model.py
+-rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 nonebot_plugin_fhl-0.1.4/PKG-INFO
```

### Comparing `nonebot_plugin_fhl-0.1.3/LICENSE` & `nonebot_plugin_fhl-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_fhl-0.1.3/pyproject.toml` & `nonebot_plugin_fhl-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 dependencies = [
     "nonebot2>=2.2.1",
     "nonebot-plugin-alconna>=0.42.4",
     "nonebot-plugin-session>=0.3.1",
     "httpx>=0.27.0",
     "msgspec>=0.18.6",
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.8, <4.0"
 readme = "README.md"
 keywords = [
     "nonebot",
     "fei hua ling",
 ]
-version = "0.1.3"
+version = "0.1.4"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/baiqwerdvd/nonebot-plugin-fhl"
 repository = "https://github.com/baiqwerdvd/nonebot-plugin-fhl"
```

### Comparing `nonebot_plugin_fhl-0.1.3/src/nonebot_plugin_fhl/__init__.py` & `nonebot_plugin_fhl-0.1.4/src/nonebot_plugin_fhl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 )
 
 from nonebot_plugin_session import SessionId, SessionIdType
 
 from .logic import FeiHuaLing
 from .config import Config
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 
 __plugin_meta__ = PluginMetadata(
     name="Fei Hua Ling",
     description="飞花令小游戏",
     usage="""
     /梦笔生花,
     [WIP] /走马观花[5-9] [WIP]
```

### Comparing `nonebot_plugin_fhl-0.1.3/src/nonebot_plugin_fhl/api.py` & `nonebot_plugin_fhl-0.1.4/src/nonebot_plugin_fhl/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_fhl-0.1.3/src/nonebot_plugin_fhl/logic.py` & `nonebot_plugin_fhl-0.1.4/src/nonebot_plugin_fhl/logic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_fhl-0.1.3/src/nonebot_plugin_fhl/model.py` & `nonebot_plugin_fhl-0.1.4/src/nonebot_plugin_fhl/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_fhl-0.1.3/PKG-INFO` & `nonebot_plugin_fhl-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-fhl
-Version: 0.1.3
+Version: 0.1.4
 Summary: Nonebot plugin for fhl
 Keywords: nonebot,fei hua ling
 Home-page: https://github.com/baiqwerdvd/nonebot-plugin-fhl
 Author-Email: baiqwerdvd <158065462+baiqwerdvd@users.noreply.github.com>
 License: MIT
 Project-URL: Homepage, https://github.com/baiqwerdvd/nonebot-plugin-fhl
 Project-URL: Repository, https://github.com/baiqwerdvd/nonebot-plugin-fhl
-Requires-Python: >=3.8
+Requires-Python: <4.0,>=3.8
 Requires-Dist: nonebot2>=2.2.1
 Requires-Dist: nonebot-plugin-alconna>=0.42.4
 Requires-Dist: nonebot-plugin-session>=0.3.1
 Requires-Dist: httpx>=0.27.0
 Requires-Dist: msgspec>=0.18.6
 Description-Content-Type: text/markdown
```

