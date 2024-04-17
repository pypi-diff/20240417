# Comparing `tmp/nonebot_plugin_fhl-0.1.6.tar.gz` & `tmp/nonebot_plugin_fhl-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_fhl-0.1.6.tar", last modified: Wed Apr 17 10:44:46 2024, max compression
+gzip compressed data, was "nonebot_plugin_fhl-0.1.8.tar", last modified: Wed Apr 17 11:21:29 2024, max compression
```

## Comparing `nonebot_plugin_fhl-0.1.6.tar` & `nonebot_plugin_fhl-0.1.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2024-04-17 10:44:28.911381 nonebot_plugin_fhl-0.1.6/LICENSE
--rw-r--r--   0        0        0       21 2024-04-17 10:44:28.911381 nonebot_plugin_fhl-0.1.6/README.md
--rw-r--r--   0        0        0     1360 2024-04-17 10:44:46.711299 nonebot_plugin_fhl-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     4837 2024-04-17 10:44:28.911381 nonebot_plugin_fhl-0.1.6/src/nonebot_plugin_fhl/__init__.py
--rw-r--r--   0        0        0     1127 2024-04-17 10:44:28.911381 nonebot_plugin_fhl-0.1.6/src/nonebot_plugin_fhl/api.py
--rw-r--r--   0        0        0      273 2024-04-17 10:44:28.915381 nonebot_plugin_fhl-0.1.6/src/nonebot_plugin_fhl/config.py
--rw-r--r--   0        0        0      808 2024-04-17 10:44:28.915381 nonebot_plugin_fhl-0.1.6/src/nonebot_plugin_fhl/logic.py
--rw-r--r--   0        0        0     1195 2024-04-17 10:44:28.915381 nonebot_plugin_fhl-0.1.6/src/nonebot_plugin_fhl/model.py
--rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 nonebot_plugin_fhl-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-17 11:21:14.888038 nonebot_plugin_fhl-0.1.8/LICENSE
+-rw-r--r--   0        0        0       21 2024-04-17 11:21:14.888038 nonebot_plugin_fhl-0.1.8/README.md
+-rw-r--r--   0        0        0     1360 2024-04-17 11:21:29.976065 nonebot_plugin_fhl-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     5191 2024-04-17 11:21:14.888038 nonebot_plugin_fhl-0.1.8/src/nonebot_plugin_fhl/__init__.py
+-rw-r--r--   0        0        0     1101 2024-04-17 11:21:14.888038 nonebot_plugin_fhl-0.1.8/src/nonebot_plugin_fhl/api.py
+-rw-r--r--   0        0        0      273 2024-04-17 11:21:14.888038 nonebot_plugin_fhl-0.1.8/src/nonebot_plugin_fhl/config.py
+-rw-r--r--   0        0        0      808 2024-04-17 11:21:14.888038 nonebot_plugin_fhl-0.1.8/src/nonebot_plugin_fhl/logic.py
+-rw-r--r--   0        0        0     1195 2024-04-17 11:21:14.888038 nonebot_plugin_fhl-0.1.8/src/nonebot_plugin_fhl/model.py
+-rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 nonebot_plugin_fhl-0.1.8/PKG-INFO
```

### Comparing `nonebot_plugin_fhl-0.1.6/LICENSE` & `nonebot_plugin_fhl-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_fhl-0.1.6/pyproject.toml` & `nonebot_plugin_fhl-0.1.8/pyproject.toml`

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
-version = "0.1.6"
+version = "0.1.8"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/baiqwerdvd/nonebot-plugin-fhl"
 repository = "https://github.com/baiqwerdvd/nonebot-plugin-fhl"
```

### Comparing `nonebot_plugin_fhl-0.1.6/src/nonebot_plugin_fhl/__init__.py` & `nonebot_plugin_fhl-0.1.8/src/nonebot_plugin_fhl/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 )
 
 from nonebot_plugin_session import SessionId, SessionIdType
 
 from .logic import FeiHuaLing
 from .config import Config
 
-__version__ = "0.1.6"
+__version__ = "0.1.8"
 
 __plugin_meta__ = PluginMetadata(
     name="Fei Hua Ling",
     description="飞花令小游戏",
     usage="""
     /梦笔生花,
     [WIP] /走马观花[5-9] [WIP]
@@ -142,39 +142,54 @@
     await game_instance.init_game()
 
     games[user_id] = game_instance
     set_timeout(matcher, user_id)
     global poery_word
     poery_word = on_regex(
         r"(?P<poetry>[\u4e00-\u9fa5]+)",
-        rule=game_is_running,
+        rule=to_me() & game_is_running,
         block=True,
         priority=14,
     )
     poery_word.append_handler(handle_poery)
 
     msg = f"题目：{game_instance.subject}"
     await UniMessage.text(msg).send()
 
 
+@fhl_stop.handle()
+async def _(matcher: Matcher, user_id: UserId):
+    game = games[user_id]
+    stop_game(user_id)
+
+    msg = "游戏已结束"
+    if len(game.history) >= 1:
+        for i in game.history:
+            msg += i + "\n"
+    await matcher.finish(msg)
+
+
 async def handle_poery(
     matcher: Matcher, user_id: UserId, matched: Dict[str, Any] = RegexDict()
 ):
     game = games[user_id]
     set_timeout(matcher, user_id)
 
     poetry = str(matched["poetry"])
     result = await game.answer(poetry)
     code = result.code
 
     if code == 200:
         tup = ""
         if result.data.reason != "":
             tup = f"\nUpdate: {result.data.update}"
-        msg = f"题目: {result.data.subjectstring}\n历史: {result.data.history}\n{tup}"
+        history = ""
+        for i in result.data.history:
+            history += i + "\n"
+        msg = f"题目: {result.data.subjectstring}\n历史: {history}{tup}"
         await UniMessage.text(msg).send()
     elif code == 201:
         # 不切题
         msg = f"不切题: {result.data.reason}"
         await UniMessage.text(msg).send()
     elif code == 202:
         # game finish
```

### Comparing `nonebot_plugin_fhl-0.1.6/src/nonebot_plugin_fhl/api.py` & `nonebot_plugin_fhl-0.1.8/src/nonebot_plugin_fhl/api.py`

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
-            data=json.decode(json.encode(data)),
+            data=json.encode(data),
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
-            data=json.decode(json.encode(data)),
+            data=json.encode(data),
         )
         return convert(response.json(), AnswerResponse)
 
 
 api = FHLApi()
```

### Comparing `nonebot_plugin_fhl-0.1.6/src/nonebot_plugin_fhl/logic.py` & `nonebot_plugin_fhl-0.1.8/src/nonebot_plugin_fhl/logic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_fhl-0.1.6/src/nonebot_plugin_fhl/model.py` & `nonebot_plugin_fhl-0.1.8/src/nonebot_plugin_fhl/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_fhl-0.1.6/PKG-INFO` & `nonebot_plugin_fhl-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-fhl
-Version: 0.1.6
+Version: 0.1.8
 Summary: Nonebot plugin for fhl
 Keywords: nonebot,fei hua ling
 Home-page: https://github.com/baiqwerdvd/nonebot-plugin-fhl
 Author-Email: baiqwerdvd <158065462+baiqwerdvd@users.noreply.github.com>
 License: MIT
 Project-URL: Homepage, https://github.com/baiqwerdvd/nonebot-plugin-fhl
 Project-URL: Repository, https://github.com/baiqwerdvd/nonebot-plugin-fhl
```

