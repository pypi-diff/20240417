# Comparing `tmp/nonebot_plugin_fhl-0.1.9.tar.gz` & `tmp/nonebot_plugin_fhl-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_fhl-0.1.9.tar", last modified: Wed Apr 17 11:25:00 2024, max compression
+gzip compressed data, was "nonebot_plugin_fhl-0.2.1.tar", last modified: Wed Apr 17 12:05:44 2024, max compression
```

## Comparing `nonebot_plugin_fhl-0.1.9.tar` & `nonebot_plugin_fhl-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2024-04-17 11:24:42.028443 nonebot_plugin_fhl-0.1.9/LICENSE
--rw-r--r--   0        0        0       21 2024-04-17 11:24:42.028443 nonebot_plugin_fhl-0.1.9/README.md
--rw-r--r--   0        0        0     1360 2024-04-17 11:25:00.620509 nonebot_plugin_fhl-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     5191 2024-04-17 11:24:42.032443 nonebot_plugin_fhl-0.1.9/src/nonebot_plugin_fhl/__init__.py
--rw-r--r--   0        0        0     1101 2024-04-17 11:24:42.032443 nonebot_plugin_fhl-0.1.9/src/nonebot_plugin_fhl/api.py
--rw-r--r--   0        0        0      273 2024-04-17 11:24:42.032443 nonebot_plugin_fhl-0.1.9/src/nonebot_plugin_fhl/config.py
--rw-r--r--   0        0        0      834 2024-04-17 11:24:42.032443 nonebot_plugin_fhl-0.1.9/src/nonebot_plugin_fhl/logic.py
--rw-r--r--   0        0        0     1195 2024-04-17 11:24:42.032443 nonebot_plugin_fhl-0.1.9/src/nonebot_plugin_fhl/model.py
--rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 nonebot_plugin_fhl-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-17 12:05:28.104971 nonebot_plugin_fhl-0.2.1/LICENSE
+-rw-r--r--   0        0        0       21 2024-04-17 12:05:28.104971 nonebot_plugin_fhl-0.2.1/README.md
+-rw-r--r--   0        0        0     1360 2024-04-17 12:05:44.408952 nonebot_plugin_fhl-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5414 2024-04-17 12:05:28.104971 nonebot_plugin_fhl-0.2.1/src/nonebot_plugin_fhl/__init__.py
+-rw-r--r--   0        0        0     1101 2024-04-17 12:05:28.104971 nonebot_plugin_fhl-0.2.1/src/nonebot_plugin_fhl/api.py
+-rw-r--r--   0        0        0      273 2024-04-17 12:05:28.104971 nonebot_plugin_fhl-0.2.1/src/nonebot_plugin_fhl/config.py
+-rw-r--r--   0        0        0      834 2024-04-17 12:05:28.104971 nonebot_plugin_fhl-0.2.1/src/nonebot_plugin_fhl/logic.py
+-rw-r--r--   0        0        0     1195 2024-04-17 12:05:28.104971 nonebot_plugin_fhl-0.2.1/src/nonebot_plugin_fhl/model.py
+-rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 nonebot_plugin_fhl-0.2.1/PKG-INFO
```

### Comparing `nonebot_plugin_fhl-0.1.9/LICENSE` & `nonebot_plugin_fhl-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_fhl-0.1.9/pyproject.toml` & `nonebot_plugin_fhl-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ]
 requires-python = ">=3.8, <4.0"
 readme = "README.md"
 keywords = [
     "nonebot",
     "fei hua ling",
 ]
-version = "0.1.9"
+version = "0.2.1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/baiqwerdvd/nonebot-plugin-fhl"
 repository = "https://github.com/baiqwerdvd/nonebot-plugin-fhl"
```

### Comparing `nonebot_plugin_fhl-0.1.9/src/nonebot_plugin_fhl/__init__.py` & `nonebot_plugin_fhl-0.2.1/src/nonebot_plugin_fhl/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 )
 
 from nonebot_plugin_session import SessionId, SessionIdType
 
 from .logic import FeiHuaLing
 from .config import Config
 
-__version__ = "0.1.9"
+__version__ = "0.2.1"
 
 __plugin_meta__ = PluginMetadata(
     name="Fei Hua Ling",
     description="飞花令小游戏",
     usage="""
     /梦笔生花,
     [WIP] /走马观花[5-9] [WIP]
@@ -91,30 +91,29 @@
 #     ),
 #     rule=to_me() & game_not_running,
 #     use_cmd_start=True,
 #     block=True,
 #     priority=13,
 # )
 fhl_stop = on_alconna(
-    "结束",
-    aliases=("结束游戏", "结束飞花令"),
+    "结束飞花令",
     rule=game_is_running,
     use_cmd_start=True,
     block=True,
     priority=13,
 )
-wordle_word: Optional[Type[Matcher]] = None
+poery_word: Optional[Type[Matcher]] = None
 
 
 def stop_game(user_id: str):
     if timer := timers.pop(user_id, None):
         timer.cancel()
     games.pop(user_id, None)
-    if wordle_word:
-        wordle_word.destroy()
+    if poery_word:
+        poery_word.destroy()
 
 
 async def stop_game_timeout(matcher: Matcher, user_id: str):
     game = games.get(user_id, None)
     stop_game(user_id)
     if game:
         msg = "猜单词超时，游戏结束"
@@ -157,39 +156,47 @@
 
 
 @fhl_stop.handle()
 async def _(matcher: Matcher, user_id: UserId):
     game = games[user_id]
     stop_game(user_id)
 
-    msg = "游戏已结束"
+    msg = "游戏已结束" + "\n"
     if len(game.history) >= 1:
         for i in game.history:
-            msg += i + "\n"
+            msg += "\n" + i
     await matcher.finish(msg)
 
 
 async def handle_poery(
     matcher: Matcher, user_id: UserId, matched: Dict[str, Any] = RegexDict()
 ):
     game = games[user_id]
     set_timeout(matcher, user_id)
 
     poetry = str(matched["poetry"])
     result = await game.answer(poetry)
     code = result.code
 
+    if len(result.data.history) > 10:
+        stop_game(user_id)
+        msg = "已经答出10句, 本局游戏结束\n"
+        if len(game.history) >= 1:
+            for i in game.history:
+                msg += "\n" + i
+        await matcher.finish(msg)
+
     if code == 200:
         tup = ""
         if result.data.reason != "":
             tup = f"\nUpdate: {result.data.update}"
         history = ""
         for i in result.data.history:
             history += i + "\n"
-        msg = f"题目: {result.data.subjectstring}\n历史: {history}{tup}"
+        msg = f"题目: {result.data.subjectstring}\n历史:\n{history}{tup}"
         await UniMessage.text(msg).send()
     elif code == 201:
         # 不切题
         msg = f"不切题: {result.data.reason}"
         await UniMessage.text(msg).send()
     elif code == 202:
         # game finish
```

### Comparing `nonebot_plugin_fhl-0.1.9/src/nonebot_plugin_fhl/api.py` & `nonebot_plugin_fhl-0.2.1/src/nonebot_plugin_fhl/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_fhl-0.1.9/src/nonebot_plugin_fhl/logic.py` & `nonebot_plugin_fhl-0.2.1/src/nonebot_plugin_fhl/logic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_fhl-0.1.9/src/nonebot_plugin_fhl/model.py` & `nonebot_plugin_fhl-0.2.1/src/nonebot_plugin_fhl/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_fhl-0.1.9/PKG-INFO` & `nonebot_plugin_fhl-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-fhl
-Version: 0.1.9
+Version: 0.2.1
 Summary: Nonebot plugin for fhl
 Keywords: nonebot,fei hua ling
 Home-page: https://github.com/baiqwerdvd/nonebot-plugin-fhl
 Author-Email: baiqwerdvd <158065462+baiqwerdvd@users.noreply.github.com>
 License: MIT
 Project-URL: Homepage, https://github.com/baiqwerdvd/nonebot-plugin-fhl
 Project-URL: Repository, https://github.com/baiqwerdvd/nonebot-plugin-fhl
```

