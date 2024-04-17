# Comparing `tmp/nonebot_plugin_fhl-0.1.0.tar.gz` & `tmp/nonebot_plugin_fhl-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_fhl-0.1.0.tar", last modified: Wed Apr 17 09:49:41 2024, max compression
+gzip compressed data, was "nonebot_plugin_fhl-0.1.1.tar", last modified: Wed Apr 17 10:01:37 2024, max compression
```

## Comparing `nonebot_plugin_fhl-0.1.0.tar` & `nonebot_plugin_fhl-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2024-04-17 09:49:28.396411 nonebot_plugin_fhl-0.1.0/LICENSE
--rw-r--r--   0        0        0       21 2024-04-17 09:49:28.396411 nonebot_plugin_fhl-0.1.0/README.md
--rw-r--r--   0        0        0     1354 2024-04-17 09:49:41.468414 nonebot_plugin_fhl-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4797 2024-04-17 09:49:28.400411 nonebot_plugin_fhl-0.1.0/src/nonebot_plugin_fhl/__init__.py
--rw-r--r--   0        0        0     1069 2024-04-17 09:49:28.400411 nonebot_plugin_fhl-0.1.0/src/nonebot_plugin_fhl/api.py
--rw-r--r--   0        0        0      191 2024-04-17 09:49:28.400411 nonebot_plugin_fhl-0.1.0/src/nonebot_plugin_fhl/config.py
--rw-r--r--   0        0        0      743 2024-04-17 09:49:28.400411 nonebot_plugin_fhl-0.1.0/src/nonebot_plugin_fhl/logic.py
--rw-r--r--   0        0        0     1171 2024-04-17 09:49:28.400411 nonebot_plugin_fhl-0.1.0/src/nonebot_plugin_fhl/model.py
--rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 nonebot_plugin_fhl-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-17 10:01:25.906135 nonebot_plugin_fhl-0.1.1/LICENSE
+-rw-r--r--   0        0        0       21 2024-04-17 10:01:25.906135 nonebot_plugin_fhl-0.1.1/README.md
+-rw-r--r--   0        0        0     1354 2024-04-17 10:01:37.862276 nonebot_plugin_fhl-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4817 2024-04-17 10:01:25.910135 nonebot_plugin_fhl-0.1.1/src/nonebot_plugin_fhl/__init__.py
+-rw-r--r--   0        0        0     1069 2024-04-17 10:01:25.910135 nonebot_plugin_fhl-0.1.1/src/nonebot_plugin_fhl/api.py
+-rw-r--r--   0        0        0      265 2024-04-17 10:01:25.910135 nonebot_plugin_fhl-0.1.1/src/nonebot_plugin_fhl/config.py
+-rw-r--r--   0        0        0      743 2024-04-17 10:01:25.910135 nonebot_plugin_fhl-0.1.1/src/nonebot_plugin_fhl/logic.py
+-rw-r--r--   0        0        0     1171 2024-04-17 10:01:25.910135 nonebot_plugin_fhl-0.1.1/src/nonebot_plugin_fhl/model.py
+-rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 nonebot_plugin_fhl-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_fhl-0.1.0/LICENSE` & `nonebot_plugin_fhl-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_fhl-0.1.0/pyproject.toml` & `nonebot_plugin_fhl-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ]
 requires-python = ">=3.9"
 readme = "README.md"
 keywords = [
     "nonebot",
     "fei hua ling",
 ]
-version = "0.1.0"
+version = "0.1.1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/baiqwerdvd/nonebot-plugin-fhl"
 repository = "https://github.com/baiqwerdvd/nonebot-plugin-fhl"
```

### Comparing `nonebot_plugin_fhl-0.1.0/src/nonebot_plugin_fhl/__init__.py` & `nonebot_plugin_fhl-0.1.1/src/nonebot_plugin_fhl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 )
 
 from nonebot_plugin_session import SessionId, SessionIdType
 
 from .logic import FeiHuaLing
 from .config import Config
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 __plugin_meta__ = PluginMetadata(
     name="Fei Hua Ling",
     description="飞花令小游戏",
     usage="""
     /梦笔生花,
     [WIP] /走马观花[5-9] [WIP]
@@ -64,24 +64,24 @@
 fhl_mode_1 = on_alconna(
     Alconna("梦笔生花"),
     rule=to_me() & game_not_running,
     use_cmd_start=True,
     block=True,
     priority=13,
 )
-fhl_mode_2 = on_alconna(
-    Alconna(
-        "走马观花",
-        Option("-l|--length", Args["length", int], help_text="诗句长度"),
-    ),
-    rule=to_me() & game_not_running,
-    use_cmd_start=True,
-    block=True,
-    priority=13,
-)
+# fhl_mode_2 = on_alconna(
+#     Alconna(
+#         "走马观花",
+#         Option("-l|--length", Args["length", int], help_text="诗句长度"),
+#     ),
+#     rule=to_me() & game_not_running,
+#     use_cmd_start=True,
+#     block=True,
+#     priority=13,
+# )
 # fhl_mode_3 = on_alconna(
 #     Alconna(
 #         "天女散花",
 #         Option("-l|--length", Args["length", int], help_text="诗句长度"),
 #     ),
 #     rule=to_me() & game_not_running,
 #     use_cmd_start=True,
```

### Comparing `nonebot_plugin_fhl-0.1.0/src/nonebot_plugin_fhl/api.py` & `nonebot_plugin_fhl-0.1.1/src/nonebot_plugin_fhl/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import httpx
 from msgspec import convert
 
-from .config import Config
+from .config import config
 from .model import (
     GetTopicRequest,
     GetTopicResponse,
     AnswerRequest,
     AnswerResponse,
 )
 
 
 class FHLApi:
     def __init__(self) -> None:
-        self.client = httpx.AsyncClient(base_url=Config.feihualing_api)
+        self.client = httpx.AsyncClient(base_url=config.feihualing_api)
 
     async def get_topic(
         self,
         game_mode: str,
         poetry_size: int,
         game_id: str,
     ) -> GetTopicResponse:
```

### Comparing `nonebot_plugin_fhl-0.1.0/src/nonebot_plugin_fhl/logic.py` & `nonebot_plugin_fhl-0.1.1/src/nonebot_plugin_fhl/logic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from .config import Config
+from .config import config
 from .api import api
 
 
 class FeiHuaLing:
     subject: str
     history: list[str]
     turn_timer: int
 
     def __init__(self, user_id: str, game_mode: str, poetry_size: int) -> None:
-        self.api = Config.feihualing_api
+        self.api = config.feihualing_api
         self.game_id = user_id
         self.game_mode = game_mode
         self.poetry_size = poetry_size
 
     async def init_game(self):
         resp = await api.get_topic(
             self.game_mode,
```

### Comparing `nonebot_plugin_fhl-0.1.0/src/nonebot_plugin_fhl/model.py` & `nonebot_plugin_fhl-0.1.1/src/nonebot_plugin_fhl/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_fhl-0.1.0/PKG-INFO` & `nonebot_plugin_fhl-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-fhl
-Version: 0.1.0
+Version: 0.1.1
 Summary: Nonebot plugin for fhl
 Keywords: nonebot,fei hua ling
 Home-page: https://github.com/baiqwerdvd/nonebot-plugin-fhl
 Author-Email: baiqwerdvd <158065462+baiqwerdvd@users.noreply.github.com>
 License: MIT
 Project-URL: Homepage, https://github.com/baiqwerdvd/nonebot-plugin-fhl
 Project-URL: Repository, https://github.com/baiqwerdvd/nonebot-plugin-fhl
```

