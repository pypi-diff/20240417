# Comparing `tmp/nonebot_plugin_fhl-0.1.4.tar.gz` & `tmp/nonebot_plugin_fhl-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_fhl-0.1.4.tar", last modified: Wed Apr 17 10:16:50 2024, max compression
+gzip compressed data, was "nonebot_plugin_fhl-0.1.5.tar", last modified: Wed Apr 17 10:37:23 2024, max compression
```

## Comparing `nonebot_plugin_fhl-0.1.4.tar` & `nonebot_plugin_fhl-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2024-04-17 10:16:30.891071 nonebot_plugin_fhl-0.1.4/LICENSE
--rw-r--r--   0        0        0       21 2024-04-17 10:16:30.891071 nonebot_plugin_fhl-0.1.4/README.md
--rw-r--r--   0        0        0     1360 2024-04-17 10:16:50.019054 nonebot_plugin_fhl-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4820 2024-04-17 10:16:30.895071 nonebot_plugin_fhl-0.1.4/src/nonebot_plugin_fhl/__init__.py
--rw-r--r--   0        0        0     1069 2024-04-17 10:16:30.895071 nonebot_plugin_fhl-0.1.4/src/nonebot_plugin_fhl/api.py
--rw-r--r--   0        0        0      266 2024-04-17 10:16:30.895071 nonebot_plugin_fhl-0.1.4/src/nonebot_plugin_fhl/config.py
--rw-r--r--   0        0        0      808 2024-04-17 10:16:30.895071 nonebot_plugin_fhl-0.1.4/src/nonebot_plugin_fhl/logic.py
--rw-r--r--   0        0        0     1195 2024-04-17 10:16:30.895071 nonebot_plugin_fhl-0.1.4/src/nonebot_plugin_fhl/model.py
--rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 nonebot_plugin_fhl-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-17 10:37:10.791437 nonebot_plugin_fhl-0.1.5/LICENSE
+-rw-r--r--   0        0        0       21 2024-04-17 10:37:10.791437 nonebot_plugin_fhl-0.1.5/README.md
+-rw-r--r--   0        0        0     1360 2024-04-17 10:37:23.483554 nonebot_plugin_fhl-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4820 2024-04-17 10:37:10.791437 nonebot_plugin_fhl-0.1.5/src/nonebot_plugin_fhl/__init__.py
+-rw-r--r--   0        0        0     1101 2024-04-17 10:37:10.791437 nonebot_plugin_fhl-0.1.5/src/nonebot_plugin_fhl/api.py
+-rw-r--r--   0        0        0      266 2024-04-17 10:37:10.791437 nonebot_plugin_fhl-0.1.5/src/nonebot_plugin_fhl/config.py
+-rw-r--r--   0        0        0      808 2024-04-17 10:37:10.791437 nonebot_plugin_fhl-0.1.5/src/nonebot_plugin_fhl/logic.py
+-rw-r--r--   0        0        0     1195 2024-04-17 10:37:10.791437 nonebot_plugin_fhl-0.1.5/src/nonebot_plugin_fhl/model.py
+-rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 nonebot_plugin_fhl-0.1.5/PKG-INFO
```

### Comparing `nonebot_plugin_fhl-0.1.4/LICENSE` & `nonebot_plugin_fhl-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_fhl-0.1.4/pyproject.toml` & `nonebot_plugin_fhl-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ]
 requires-python = ">=3.8, <4.0"
 readme = "README.md"
 keywords = [
     "nonebot",
     "fei hua ling",
 ]
-version = "0.1.4"
+version = "0.1.5"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/baiqwerdvd/nonebot-plugin-fhl"
 repository = "https://github.com/baiqwerdvd/nonebot-plugin-fhl"
```

### Comparing `nonebot_plugin_fhl-0.1.4/src/nonebot_plugin_fhl/__init__.py` & `nonebot_plugin_fhl-0.1.5/src/nonebot_plugin_fhl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 )
 
 from nonebot_plugin_session import SessionId, SessionIdType
 
 from .logic import FeiHuaLing
 from .config import Config
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
 
 __plugin_meta__ = PluginMetadata(
     name="Fei Hua Ling",
     description="飞花令小游戏",
     usage="""
     /梦笔生花,
     [WIP] /走马观花[5-9] [WIP]
```

### Comparing `nonebot_plugin_fhl-0.1.4/src/nonebot_plugin_fhl/api.py` & `nonebot_plugin_fhl-0.1.5/src/nonebot_plugin_fhl/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import httpx
-from msgspec import convert
+from msgspec import convert, json
 
 from .config import config
 from .model import (
     GetTopicRequest,
     GetTopicResponse,
     AnswerRequest,
     AnswerResponse,
@@ -23,28 +23,28 @@
         data = GetTopicRequest(
             modtype=game_mode,
             size=poetry_size,
             id_=game_id,
         )
         response = await self.client.post(
             "/gettopic",
-            json=data,
+            json=json.encode(data),
         )
         return convert(response.json(), GetTopicResponse)
 
     async def answer(
         self,
         game_id: str,
         answer: str,
     ):
         data = AnswerRequest(
             id_=game_id,
             text=answer,
         )
         response = await self.client.post(
             "/answer",
-            json=data,
+            json=json.encode(data),
         )
         return convert(response.json(), AnswerResponse)
 
 
 api = FHLApi()
```

### Comparing `nonebot_plugin_fhl-0.1.4/src/nonebot_plugin_fhl/logic.py` & `nonebot_plugin_fhl-0.1.5/src/nonebot_plugin_fhl/logic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_fhl-0.1.4/src/nonebot_plugin_fhl/model.py` & `nonebot_plugin_fhl-0.1.5/src/nonebot_plugin_fhl/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_fhl-0.1.4/PKG-INFO` & `nonebot_plugin_fhl-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-fhl
-Version: 0.1.4
+Version: 0.1.5
 Summary: Nonebot plugin for fhl
 Keywords: nonebot,fei hua ling
 Home-page: https://github.com/baiqwerdvd/nonebot-plugin-fhl
 Author-Email: baiqwerdvd <158065462+baiqwerdvd@users.noreply.github.com>
 License: MIT
 Project-URL: Homepage, https://github.com/baiqwerdvd/nonebot-plugin-fhl
 Project-URL: Repository, https://github.com/baiqwerdvd/nonebot-plugin-fhl
```

