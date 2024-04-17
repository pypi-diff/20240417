# Comparing `tmp/nonebot_plugin_fhl-0.2.1.tar.gz` & `tmp/nonebot_plugin_fhl-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_fhl-0.2.1.tar", last modified: Wed Apr 17 12:05:44 2024, max compression
+gzip compressed data, was "nonebot_plugin_fhl-1.0.0.tar", last modified: Wed Apr 17 12:36:14 2024, max compression
```

## Comparing `nonebot_plugin_fhl-0.2.1.tar` & `nonebot_plugin_fhl-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2024-04-17 12:05:28.104971 nonebot_plugin_fhl-0.2.1/LICENSE
--rw-r--r--   0        0        0       21 2024-04-17 12:05:28.104971 nonebot_plugin_fhl-0.2.1/README.md
--rw-r--r--   0        0        0     1360 2024-04-17 12:05:44.408952 nonebot_plugin_fhl-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     5414 2024-04-17 12:05:28.104971 nonebot_plugin_fhl-0.2.1/src/nonebot_plugin_fhl/__init__.py
--rw-r--r--   0        0        0     1101 2024-04-17 12:05:28.104971 nonebot_plugin_fhl-0.2.1/src/nonebot_plugin_fhl/api.py
--rw-r--r--   0        0        0      273 2024-04-17 12:05:28.104971 nonebot_plugin_fhl-0.2.1/src/nonebot_plugin_fhl/config.py
--rw-r--r--   0        0        0      834 2024-04-17 12:05:28.104971 nonebot_plugin_fhl-0.2.1/src/nonebot_plugin_fhl/logic.py
--rw-r--r--   0        0        0     1195 2024-04-17 12:05:28.104971 nonebot_plugin_fhl-0.2.1/src/nonebot_plugin_fhl/model.py
--rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 nonebot_plugin_fhl-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-17 12:36:01.582847 nonebot_plugin_fhl-1.0.0/LICENSE
+-rw-r--r--   0        0        0      703 2024-04-17 12:36:01.582847 nonebot_plugin_fhl-1.0.0/README.md
+-rw-r--r--   0        0        0     1360 2024-04-17 12:36:14.562793 nonebot_plugin_fhl-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5414 2024-04-17 12:36:01.582847 nonebot_plugin_fhl-1.0.0/src/nonebot_plugin_fhl/__init__.py
+-rw-r--r--   0        0        0     1101 2024-04-17 12:36:01.582847 nonebot_plugin_fhl-1.0.0/src/nonebot_plugin_fhl/api.py
+-rw-r--r--   0        0        0      273 2024-04-17 12:36:01.582847 nonebot_plugin_fhl-1.0.0/src/nonebot_plugin_fhl/config.py
+-rw-r--r--   0        0        0      834 2024-04-17 12:36:01.582847 nonebot_plugin_fhl-1.0.0/src/nonebot_plugin_fhl/logic.py
+-rw-r--r--   0        0        0     1195 2024-04-17 12:36:01.582847 nonebot_plugin_fhl-1.0.0/src/nonebot_plugin_fhl/model.py
+-rw-r--r--   0        0        0     1371 1970-01-01 00:00:00.000000 nonebot_plugin_fhl-1.0.0/PKG-INFO
```

### Comparing `nonebot_plugin_fhl-0.2.1/LICENSE` & `nonebot_plugin_fhl-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_fhl-0.2.1/pyproject.toml` & `nonebot_plugin_fhl-1.0.0/pyproject.toml`

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
-version = "0.2.1"
+version = "1.0.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/baiqwerdvd/nonebot-plugin-fhl"
 repository = "https://github.com/baiqwerdvd/nonebot-plugin-fhl"
```

### Comparing `nonebot_plugin_fhl-0.2.1/src/nonebot_plugin_fhl/__init__.py` & `nonebot_plugin_fhl-1.0.0/src/nonebot_plugin_fhl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 )
 
 from nonebot_plugin_session import SessionId, SessionIdType
 
 from .logic import FeiHuaLing
 from .config import Config
 
-__version__ = "0.2.1"
+__version__ = "1.0.0"
 
 __plugin_meta__ = PluginMetadata(
     name="Fei Hua Ling",
     description="飞花令小游戏",
     usage="""
     /梦笔生花,
     [WIP] /走马观花[5-9] [WIP]
```

### Comparing `nonebot_plugin_fhl-0.2.1/src/nonebot_plugin_fhl/api.py` & `nonebot_plugin_fhl-1.0.0/src/nonebot_plugin_fhl/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_fhl-0.2.1/src/nonebot_plugin_fhl/logic.py` & `nonebot_plugin_fhl-1.0.0/src/nonebot_plugin_fhl/logic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_fhl-0.2.1/src/nonebot_plugin_fhl/model.py` & `nonebot_plugin_fhl-1.0.0/src/nonebot_plugin_fhl/model.py`

 * *Files identical despite different names*

