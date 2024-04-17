# Comparing `tmp/nonebot_plugin_fhl-0.1.5.tar.gz` & `tmp/nonebot_plugin_fhl-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_fhl-0.1.5.tar", last modified: Wed Apr 17 10:37:23 2024, max compression
+gzip compressed data, was "nonebot_plugin_fhl-0.1.6.tar", last modified: Wed Apr 17 10:44:46 2024, max compression
```

## Comparing `nonebot_plugin_fhl-0.1.5.tar` & `nonebot_plugin_fhl-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2024-04-17 10:37:10.791437 nonebot_plugin_fhl-0.1.5/LICENSE
--rw-r--r--   0        0        0       21 2024-04-17 10:37:10.791437 nonebot_plugin_fhl-0.1.5/README.md
--rw-r--r--   0        0        0     1360 2024-04-17 10:37:23.483554 nonebot_plugin_fhl-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     4820 2024-04-17 10:37:10.791437 nonebot_plugin_fhl-0.1.5/src/nonebot_plugin_fhl/__init__.py
--rw-r--r--   0        0        0     1101 2024-04-17 10:37:10.791437 nonebot_plugin_fhl-0.1.5/src/nonebot_plugin_fhl/api.py
--rw-r--r--   0        0        0      266 2024-04-17 10:37:10.791437 nonebot_plugin_fhl-0.1.5/src/nonebot_plugin_fhl/config.py
--rw-r--r--   0        0        0      808 2024-04-17 10:37:10.791437 nonebot_plugin_fhl-0.1.5/src/nonebot_plugin_fhl/logic.py
--rw-r--r--   0        0        0     1195 2024-04-17 10:37:10.791437 nonebot_plugin_fhl-0.1.5/src/nonebot_plugin_fhl/model.py
--rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 nonebot_plugin_fhl-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-17 10:44:28.911381 nonebot_plugin_fhl-0.1.6/LICENSE
+-rw-r--r--   0        0        0       21 2024-04-17 10:44:28.911381 nonebot_plugin_fhl-0.1.6/README.md
+-rw-r--r--   0        0        0     1360 2024-04-17 10:44:46.711299 nonebot_plugin_fhl-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     4837 2024-04-17 10:44:28.911381 nonebot_plugin_fhl-0.1.6/src/nonebot_plugin_fhl/__init__.py
+-rw-r--r--   0        0        0     1127 2024-04-17 10:44:28.911381 nonebot_plugin_fhl-0.1.6/src/nonebot_plugin_fhl/api.py
+-rw-r--r--   0        0        0      273 2024-04-17 10:44:28.915381 nonebot_plugin_fhl-0.1.6/src/nonebot_plugin_fhl/config.py
+-rw-r--r--   0        0        0      808 2024-04-17 10:44:28.915381 nonebot_plugin_fhl-0.1.6/src/nonebot_plugin_fhl/logic.py
+-rw-r--r--   0        0        0     1195 2024-04-17 10:44:28.915381 nonebot_plugin_fhl-0.1.6/src/nonebot_plugin_fhl/model.py
+-rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 nonebot_plugin_fhl-0.1.6/PKG-INFO
```

### Comparing `nonebot_plugin_fhl-0.1.5/LICENSE` & `nonebot_plugin_fhl-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_fhl-0.1.5/pyproject.toml` & `nonebot_plugin_fhl-0.1.6/pyproject.toml`

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
-version = "0.1.5"
+version = "0.1.6"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/baiqwerdvd/nonebot-plugin-fhl"
 repository = "https://github.com/baiqwerdvd/nonebot-plugin-fhl"
```

### Comparing `nonebot_plugin_fhl-0.1.5/src/nonebot_plugin_fhl/__init__.py` & `nonebot_plugin_fhl-0.1.6/src/nonebot_plugin_fhl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 )
 
 from nonebot_plugin_session import SessionId, SessionIdType
 
 from .logic import FeiHuaLing
 from .config import Config
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 
 __plugin_meta__ = PluginMetadata(
     name="Fei Hua Ling",
     description="飞花令小游戏",
     usage="""
     /梦笔生花,
     [WIP] /走马观花[5-9] [WIP]
@@ -163,14 +163,15 @@
     set_timeout(matcher, user_id)
 
     poetry = str(matched["poetry"])
     result = await game.answer(poetry)
     code = result.code
 
     if code == 200:
+        tup = ""
         if result.data.reason != "":
             tup = f"\nUpdate: {result.data.update}"
         msg = f"题目: {result.data.subjectstring}\n历史: {result.data.history}\n{tup}"
         await UniMessage.text(msg).send()
     elif code == 201:
         # 不切题
         msg = f"不切题: {result.data.reason}"
```

### Comparing `nonebot_plugin_fhl-0.1.5/src/nonebot_plugin_fhl/api.py` & `nonebot_plugin_fhl-0.1.6/src/nonebot_plugin_fhl/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,28 +23,28 @@
         data = GetTopicRequest(
             modtype=game_mode,
             size=poetry_size,
             id_=game_id,
         )
         response = await self.client.post(
             "/gettopic",
-            json=json.encode(data),
+            data=json.decode(json.encode(data)),
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
-            json=json.encode(data),
+            data=json.decode(json.encode(data)),
         )
         return convert(response.json(), AnswerResponse)
 
 
 api = FHLApi()
```

### Comparing `nonebot_plugin_fhl-0.1.5/src/nonebot_plugin_fhl/logic.py` & `nonebot_plugin_fhl-0.1.6/src/nonebot_plugin_fhl/logic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_fhl-0.1.5/src/nonebot_plugin_fhl/model.py` & `nonebot_plugin_fhl-0.1.6/src/nonebot_plugin_fhl/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_fhl-0.1.5/PKG-INFO` & `nonebot_plugin_fhl-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-fhl
-Version: 0.1.5
+Version: 0.1.6
 Summary: Nonebot plugin for fhl
 Keywords: nonebot,fei hua ling
 Home-page: https://github.com/baiqwerdvd/nonebot-plugin-fhl
 Author-Email: baiqwerdvd <158065462+baiqwerdvd@users.noreply.github.com>
 License: MIT
 Project-URL: Homepage, https://github.com/baiqwerdvd/nonebot-plugin-fhl
 Project-URL: Repository, https://github.com/baiqwerdvd/nonebot-plugin-fhl
```

