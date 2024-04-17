# Comparing `tmp/nonebot_plugin_fhl-0.1.8.tar.gz` & `tmp/nonebot_plugin_fhl-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_fhl-0.1.8.tar", last modified: Wed Apr 17 11:21:29 2024, max compression
+gzip compressed data, was "nonebot_plugin_fhl-0.1.9.tar", last modified: Wed Apr 17 11:25:00 2024, max compression
```

## Comparing `nonebot_plugin_fhl-0.1.8.tar` & `nonebot_plugin_fhl-0.1.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2024-04-17 11:21:14.888038 nonebot_plugin_fhl-0.1.8/LICENSE
--rw-r--r--   0        0        0       21 2024-04-17 11:21:14.888038 nonebot_plugin_fhl-0.1.8/README.md
--rw-r--r--   0        0        0     1360 2024-04-17 11:21:29.976065 nonebot_plugin_fhl-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     5191 2024-04-17 11:21:14.888038 nonebot_plugin_fhl-0.1.8/src/nonebot_plugin_fhl/__init__.py
--rw-r--r--   0        0        0     1101 2024-04-17 11:21:14.888038 nonebot_plugin_fhl-0.1.8/src/nonebot_plugin_fhl/api.py
--rw-r--r--   0        0        0      273 2024-04-17 11:21:14.888038 nonebot_plugin_fhl-0.1.8/src/nonebot_plugin_fhl/config.py
--rw-r--r--   0        0        0      808 2024-04-17 11:21:14.888038 nonebot_plugin_fhl-0.1.8/src/nonebot_plugin_fhl/logic.py
--rw-r--r--   0        0        0     1195 2024-04-17 11:21:14.888038 nonebot_plugin_fhl-0.1.8/src/nonebot_plugin_fhl/model.py
--rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 nonebot_plugin_fhl-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-17 11:24:42.028443 nonebot_plugin_fhl-0.1.9/LICENSE
+-rw-r--r--   0        0        0       21 2024-04-17 11:24:42.028443 nonebot_plugin_fhl-0.1.9/README.md
+-rw-r--r--   0        0        0     1360 2024-04-17 11:25:00.620509 nonebot_plugin_fhl-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     5191 2024-04-17 11:24:42.032443 nonebot_plugin_fhl-0.1.9/src/nonebot_plugin_fhl/__init__.py
+-rw-r--r--   0        0        0     1101 2024-04-17 11:24:42.032443 nonebot_plugin_fhl-0.1.9/src/nonebot_plugin_fhl/api.py
+-rw-r--r--   0        0        0      273 2024-04-17 11:24:42.032443 nonebot_plugin_fhl-0.1.9/src/nonebot_plugin_fhl/config.py
+-rw-r--r--   0        0        0      834 2024-04-17 11:24:42.032443 nonebot_plugin_fhl-0.1.9/src/nonebot_plugin_fhl/logic.py
+-rw-r--r--   0        0        0     1195 2024-04-17 11:24:42.032443 nonebot_plugin_fhl-0.1.9/src/nonebot_plugin_fhl/model.py
+-rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 nonebot_plugin_fhl-0.1.9/PKG-INFO
```

### Comparing `nonebot_plugin_fhl-0.1.8/LICENSE` & `nonebot_plugin_fhl-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_fhl-0.1.8/pyproject.toml` & `nonebot_plugin_fhl-0.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ]
 requires-python = ">=3.8, <4.0"
 readme = "README.md"
 keywords = [
     "nonebot",
     "fei hua ling",
 ]
-version = "0.1.8"
+version = "0.1.9"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/baiqwerdvd/nonebot-plugin-fhl"
 repository = "https://github.com/baiqwerdvd/nonebot-plugin-fhl"
```

### Comparing `nonebot_plugin_fhl-0.1.8/src/nonebot_plugin_fhl/__init__.py` & `nonebot_plugin_fhl-0.1.9/src/nonebot_plugin_fhl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 )
 
 from nonebot_plugin_session import SessionId, SessionIdType
 
 from .logic import FeiHuaLing
 from .config import Config
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 
 __plugin_meta__ = PluginMetadata(
     name="Fei Hua Ling",
     description="飞花令小游戏",
     usage="""
     /梦笔生花,
     [WIP] /走马观花[5-9] [WIP]
```

### Comparing `nonebot_plugin_fhl-0.1.8/src/nonebot_plugin_fhl/api.py` & `nonebot_plugin_fhl-0.1.9/src/nonebot_plugin_fhl/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_fhl-0.1.8/src/nonebot_plugin_fhl/logic.py` & `nonebot_plugin_fhl-0.1.9/src/nonebot_plugin_fhl/logic.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 class FeiHuaLing:
     subject: str
     history: List[str]
     turn_timer: int
 
     def __init__(self, user_id: str, game_mode: str, poetry_size: int) -> None:
         self.api = config.feihualing_api
+        self.history = []
         self.game_id = user_id
         self.game_mode = game_mode
         self.poetry_size = poetry_size
 
     async def init_game(self):
         resp = await api.get_topic(
             self.game_mode,
```

### Comparing `nonebot_plugin_fhl-0.1.8/src/nonebot_plugin_fhl/model.py` & `nonebot_plugin_fhl-0.1.9/src/nonebot_plugin_fhl/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_fhl-0.1.8/PKG-INFO` & `nonebot_plugin_fhl-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-fhl
-Version: 0.1.8
+Version: 0.1.9
 Summary: Nonebot plugin for fhl
 Keywords: nonebot,fei hua ling
 Home-page: https://github.com/baiqwerdvd/nonebot-plugin-fhl
 Author-Email: baiqwerdvd <158065462+baiqwerdvd@users.noreply.github.com>
 License: MIT
 Project-URL: Homepage, https://github.com/baiqwerdvd/nonebot-plugin-fhl
 Project-URL: Repository, https://github.com/baiqwerdvd/nonebot-plugin-fhl
```

