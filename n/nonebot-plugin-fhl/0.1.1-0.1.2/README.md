# Comparing `tmp/nonebot_plugin_fhl-0.1.1.tar.gz` & `tmp/nonebot_plugin_fhl-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_fhl-0.1.1.tar", last modified: Wed Apr 17 10:01:37 2024, max compression
+gzip compressed data, was "nonebot_plugin_fhl-0.1.2.tar", last modified: Wed Apr 17 10:04:09 2024, max compression
```

## Comparing `nonebot_plugin_fhl-0.1.1.tar` & `nonebot_plugin_fhl-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2024-04-17 10:01:25.906135 nonebot_plugin_fhl-0.1.1/LICENSE
--rw-r--r--   0        0        0       21 2024-04-17 10:01:25.906135 nonebot_plugin_fhl-0.1.1/README.md
--rw-r--r--   0        0        0     1354 2024-04-17 10:01:37.862276 nonebot_plugin_fhl-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4817 2024-04-17 10:01:25.910135 nonebot_plugin_fhl-0.1.1/src/nonebot_plugin_fhl/__init__.py
--rw-r--r--   0        0        0     1069 2024-04-17 10:01:25.910135 nonebot_plugin_fhl-0.1.1/src/nonebot_plugin_fhl/api.py
--rw-r--r--   0        0        0      265 2024-04-17 10:01:25.910135 nonebot_plugin_fhl-0.1.1/src/nonebot_plugin_fhl/config.py
--rw-r--r--   0        0        0      743 2024-04-17 10:01:25.910135 nonebot_plugin_fhl-0.1.1/src/nonebot_plugin_fhl/logic.py
--rw-r--r--   0        0        0     1171 2024-04-17 10:01:25.910135 nonebot_plugin_fhl-0.1.1/src/nonebot_plugin_fhl/model.py
--rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 nonebot_plugin_fhl-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-17 10:03:56.580718 nonebot_plugin_fhl-0.1.2/LICENSE
+-rw-r--r--   0        0        0       21 2024-04-17 10:03:56.580718 nonebot_plugin_fhl-0.1.2/README.md
+-rw-r--r--   0        0        0     1354 2024-04-17 10:04:09.824604 nonebot_plugin_fhl-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4851 2024-04-17 10:03:56.580718 nonebot_plugin_fhl-0.1.2/src/nonebot_plugin_fhl/__init__.py
+-rw-r--r--   0        0        0     1069 2024-04-17 10:03:56.580718 nonebot_plugin_fhl-0.1.2/src/nonebot_plugin_fhl/api.py
+-rw-r--r--   0        0        0      265 2024-04-17 10:03:56.580718 nonebot_plugin_fhl-0.1.2/src/nonebot_plugin_fhl/config.py
+-rw-r--r--   0        0        0      743 2024-04-17 10:03:56.580718 nonebot_plugin_fhl-0.1.2/src/nonebot_plugin_fhl/logic.py
+-rw-r--r--   0        0        0     1171 2024-04-17 10:03:56.580718 nonebot_plugin_fhl-0.1.2/src/nonebot_plugin_fhl/model.py
+-rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 nonebot_plugin_fhl-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_fhl-0.1.1/LICENSE` & `nonebot_plugin_fhl-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_fhl-0.1.1/pyproject.toml` & `nonebot_plugin_fhl-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ]
 requires-python = ">=3.9"
 readme = "README.md"
 keywords = [
     "nonebot",
     "fei hua ling",
 ]
-version = "0.1.1"
+version = "0.1.2"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/baiqwerdvd/nonebot-plugin-fhl"
 repository = "https://github.com/baiqwerdvd/nonebot-plugin-fhl"
```

### Comparing `nonebot_plugin_fhl-0.1.1/src/nonebot_plugin_fhl/__init__.py` & `nonebot_plugin_fhl-0.1.2/src/nonebot_plugin_fhl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from nonebot import on_regex, require
 from nonebot.matcher import Matcher
 from nonebot.params import RegexDict
 from nonebot.plugin import PluginMetadata, inherit_supported_adapters
 from nonebot.rule import to_me
 
 require("nonebot_plugin_alconna")
+require("nonebot_plugin_session")
 
 from nonebot_plugin_alconna import (
     Alconna,
     AlconnaQuery,
     Args,
     Image,
     Option,
@@ -23,15 +24,15 @@
 )
 
 from nonebot_plugin_session import SessionId, SessionIdType
 
 from .logic import FeiHuaLing
 from .config import Config
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 __plugin_meta__ = PluginMetadata(
     name="Fei Hua Ling",
     description="飞花令小游戏",
     usage="""
     /梦笔生花,
     [WIP] /走马观花[5-9] [WIP]
```

### Comparing `nonebot_plugin_fhl-0.1.1/src/nonebot_plugin_fhl/api.py` & `nonebot_plugin_fhl-0.1.2/src/nonebot_plugin_fhl/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_fhl-0.1.1/src/nonebot_plugin_fhl/logic.py` & `nonebot_plugin_fhl-0.1.2/src/nonebot_plugin_fhl/logic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_fhl-0.1.1/src/nonebot_plugin_fhl/model.py` & `nonebot_plugin_fhl-0.1.2/src/nonebot_plugin_fhl/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_fhl-0.1.1/PKG-INFO` & `nonebot_plugin_fhl-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-fhl
-Version: 0.1.1
+Version: 0.1.2
 Summary: Nonebot plugin for fhl
 Keywords: nonebot,fei hua ling
 Home-page: https://github.com/baiqwerdvd/nonebot-plugin-fhl
 Author-Email: baiqwerdvd <158065462+baiqwerdvd@users.noreply.github.com>
 License: MIT
 Project-URL: Homepage, https://github.com/baiqwerdvd/nonebot-plugin-fhl
 Project-URL: Repository, https://github.com/baiqwerdvd/nonebot-plugin-fhl
```

