# Comparing `tmp/nonebot_plugin_fhl-0.1.2.tar.gz` & `tmp/nonebot_plugin_fhl-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_fhl-0.1.2.tar", last modified: Wed Apr 17 10:04:09 2024, max compression
+gzip compressed data, was "nonebot_plugin_fhl-0.1.3.tar", last modified: Wed Apr 17 10:14:09 2024, max compression
```

## Comparing `nonebot_plugin_fhl-0.1.2.tar` & `nonebot_plugin_fhl-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2024-04-17 10:03:56.580718 nonebot_plugin_fhl-0.1.2/LICENSE
--rw-r--r--   0        0        0       21 2024-04-17 10:03:56.580718 nonebot_plugin_fhl-0.1.2/README.md
--rw-r--r--   0        0        0     1354 2024-04-17 10:04:09.824604 nonebot_plugin_fhl-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4851 2024-04-17 10:03:56.580718 nonebot_plugin_fhl-0.1.2/src/nonebot_plugin_fhl/__init__.py
--rw-r--r--   0        0        0     1069 2024-04-17 10:03:56.580718 nonebot_plugin_fhl-0.1.2/src/nonebot_plugin_fhl/api.py
--rw-r--r--   0        0        0      265 2024-04-17 10:03:56.580718 nonebot_plugin_fhl-0.1.2/src/nonebot_plugin_fhl/config.py
--rw-r--r--   0        0        0      743 2024-04-17 10:03:56.580718 nonebot_plugin_fhl-0.1.2/src/nonebot_plugin_fhl/logic.py
--rw-r--r--   0        0        0     1171 2024-04-17 10:03:56.580718 nonebot_plugin_fhl-0.1.2/src/nonebot_plugin_fhl/model.py
--rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 nonebot_plugin_fhl-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-17 10:13:54.329829 nonebot_plugin_fhl-0.1.3/LICENSE
+-rw-r--r--   0        0        0       21 2024-04-17 10:13:54.329829 nonebot_plugin_fhl-0.1.3/README.md
+-rw-r--r--   0        0        0     1354 2024-04-17 10:14:09.701938 nonebot_plugin_fhl-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4820 2024-04-17 10:13:54.329829 nonebot_plugin_fhl-0.1.3/src/nonebot_plugin_fhl/__init__.py
+-rw-r--r--   0        0        0     1069 2024-04-17 10:13:54.329829 nonebot_plugin_fhl-0.1.3/src/nonebot_plugin_fhl/api.py
+-rw-r--r--   0        0        0      265 2024-04-17 10:13:54.329829 nonebot_plugin_fhl-0.1.3/src/nonebot_plugin_fhl/config.py
+-rw-r--r--   0        0        0      808 2024-04-17 10:13:54.329829 nonebot_plugin_fhl-0.1.3/src/nonebot_plugin_fhl/logic.py
+-rw-r--r--   0        0        0     1195 2024-04-17 10:13:54.329829 nonebot_plugin_fhl-0.1.3/src/nonebot_plugin_fhl/model.py
+-rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 nonebot_plugin_fhl-0.1.3/PKG-INFO
```

### Comparing `nonebot_plugin_fhl-0.1.2/LICENSE` & `nonebot_plugin_fhl-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_fhl-0.1.2/pyproject.toml` & `nonebot_plugin_fhl-0.1.3/pyproject.toml`

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
-requires-python = ">=3.9"
+requires-python = ">=3.8"
 readme = "README.md"
 keywords = [
     "nonebot",
     "fei hua ling",
 ]
-version = "0.1.2"
+version = "0.1.3"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/baiqwerdvd/nonebot-plugin-fhl"
 repository = "https://github.com/baiqwerdvd/nonebot-plugin-fhl"
@@ -45,15 +45,15 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "ruff>=0.3.7",
 ]
 
 [tool.ruff]
 line-length = 88
-target-version = "py39"
+target-version = "py38"
 
 [tool.ruff.lint]
 select = [
     "E",
     "W",
     "F",
     "UP",
@@ -67,15 +67,15 @@
     "C901",
     "T201",
     "E731",
     "E402",
 ]
 
 [tool.pyright]
-pythonVersion = "3.9"
+pythonVersion = "3.8"
 pythonPlatform = "All"
 typeCheckingMode = "basic"
 reportShadowedImports = false
 disableBytesTypePromotions = true
 
 [tool.pyright.defineConstant]
 PYDANTIC_V2 = true
```

### Comparing `nonebot_plugin_fhl-0.1.2/src/nonebot_plugin_fhl/__init__.py` & `nonebot_plugin_fhl-0.1.3/src/nonebot_plugin_fhl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 import asyncio
-from typing import Annotated, Any, Optional
+from typing import Any, Dict, Optional, Type
 from asyncio import TimerHandle
+from typing_extensions import Annotated
 
 from nonebot import on_regex, require
 from nonebot.matcher import Matcher
 from nonebot.params import RegexDict
 from nonebot.plugin import PluginMetadata, inherit_supported_adapters
 from nonebot.rule import to_me
 
 require("nonebot_plugin_alconna")
 require("nonebot_plugin_session")
 
 from nonebot_plugin_alconna import (
     Alconna,
-    AlconnaQuery,
-    Args,
-    Image,
-    Option,
-    Query,
-    Text,
     UniMessage,
     on_alconna,
 )
 
 from nonebot_plugin_session import SessionId, SessionIdType
 
 from .logic import FeiHuaLing
 from .config import Config
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 __plugin_meta__ = PluginMetadata(
     name="Fei Hua Ling",
     description="飞花令小游戏",
     usage="""
     /梦笔生花,
     [WIP] /走马观花[5-9] [WIP]
@@ -44,16 +39,16 @@
     config=Config,
     extra={"author": "baiqwerdvd", "example": "/梦笔生花"},
     supported_adapters=inherit_supported_adapters(
         "nonebot_plugin_alconna", "nonebot_plugin_session"
     ),
 )
 
-games: dict[str, FeiHuaLing] = {}
-timers: dict[str, TimerHandle] = {}
+games: Dict[str, FeiHuaLing] = {}
+timers: Dict[str, TimerHandle] = {}
 
 UserId = Annotated[str, SessionId(SessionIdType.GROUP)]
 
 
 def game_is_running(user_id: UserId) -> bool:
     return user_id in games
 
@@ -103,15 +98,15 @@
     "结束",
     aliases=("结束游戏", "结束飞花令"),
     rule=game_is_running,
     use_cmd_start=True,
     block=True,
     priority=13,
 )
-wordle_word: Optional[type[Matcher]] = None
+wordle_word: Optional[Type[Matcher]] = None
 
 
 def stop_game(user_id: str):
     if timer := timers.pop(user_id, None):
         timer.cancel()
     games.pop(user_id, None)
     if wordle_word:
@@ -158,15 +153,15 @@
     poery_word.append_handler(handle_poery)
 
     msg = f"题目：{game_instance.subject}"
     await UniMessage.text(msg).send()
 
 
 async def handle_poery(
-    matcher: Matcher, user_id: UserId, matched: dict[str, Any] = RegexDict()
+    matcher: Matcher, user_id: UserId, matched: Dict[str, Any] = RegexDict()
 ):
     game = games[user_id]
     set_timeout(matcher, user_id)
 
     poetry = str(matched["poetry"])
     result = await game.answer(poetry)
     code = result.code
```

### Comparing `nonebot_plugin_fhl-0.1.2/src/nonebot_plugin_fhl/api.py` & `nonebot_plugin_fhl-0.1.3/src/nonebot_plugin_fhl/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_fhl-0.1.2/src/nonebot_plugin_fhl/logic.py` & `nonebot_plugin_fhl-0.1.3/src/nonebot_plugin_fhl/logic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from typing import List
 from .config import config
 from .api import api
 
 
 class FeiHuaLing:
     subject: str
-    history: list[str]
+    history: List[str]
     turn_timer: int
 
     def __init__(self, user_id: str, game_mode: str, poetry_size: int) -> None:
         self.api = config.feihualing_api
         self.game_id = user_id
         self.game_mode = game_mode
         self.poetry_size = poetry_size
@@ -23,8 +24,9 @@
         return self.subject
 
     async def answer(self, answer: str):
         resp = await api.answer(
             self.game_id,
             answer,
         )
+        self.history = resp.data.history
         return resp
```

### Comparing `nonebot_plugin_fhl-0.1.2/src/nonebot_plugin_fhl/model.py` & `nonebot_plugin_fhl-0.1.3/src/nonebot_plugin_fhl/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import List
 from msgspec import Struct, field
 
 
 class GetTopicRequest(Struct):
     """获取飞花令题目请求"""
 
     modtype: str
@@ -54,15 +55,15 @@
 
     text: str
     """回答的语句"""
 
     update: str
     """特殊标识"""
 
-    history: list[str]
+    history: List[str]
     """历史正确回答"""
 
     user: int
     """用户"""
 
     reason: str
     """回答不合题意的原因"""
```

### Comparing `nonebot_plugin_fhl-0.1.2/PKG-INFO` & `nonebot_plugin_fhl-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-fhl
-Version: 0.1.2
+Version: 0.1.3
 Summary: Nonebot plugin for fhl
 Keywords: nonebot,fei hua ling
 Home-page: https://github.com/baiqwerdvd/nonebot-plugin-fhl
 Author-Email: baiqwerdvd <158065462+baiqwerdvd@users.noreply.github.com>
 License: MIT
 Project-URL: Homepage, https://github.com/baiqwerdvd/nonebot-plugin-fhl
 Project-URL: Repository, https://github.com/baiqwerdvd/nonebot-plugin-fhl
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Requires-Dist: nonebot2>=2.2.1
 Requires-Dist: nonebot-plugin-alconna>=0.42.4
 Requires-Dist: nonebot-plugin-session>=0.3.1
 Requires-Dist: httpx>=0.27.0
 Requires-Dist: msgspec>=0.18.6
 Description-Content-Type: text/markdown
```

