# Comparing `tmp/nonebot-plugin-hx-yinying-0.3.tar.gz` & `tmp/nonebot-plugin-hx-yinying-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-hx-yinying-0.3.tar", last modified: Wed Apr 17 01:18:15 2024, max compression
+gzip compressed data, was "nonebot-plugin-hx-yinying-0.4.tar", last modified: Wed Apr 17 01:27:45 2024, max compression
```

## Comparing `nonebot-plugin-hx-yinying-0.3.tar` & `nonebot-plugin-hx-yinying-0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 01:18:14.999583 nonebot-plugin-hx-yinying-0.3/
--rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-0.3/LICENSE
--rw-rw-rw-   0        0        0     2677 2024-04-17 01:18:14.999583 nonebot-plugin-hx-yinying-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2239 2024-04-17 00:42:32.000000 nonebot-plugin-hx-yinying-0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 01:18:14.911351 nonebot-plugin-hx-yinying-0.3/nonebot_plugin_hx_yinying/
--rw-rw-rw-   0        0        0     1260 2024-04-17 01:00:56.000000 nonebot-plugin-hx-yinying-0.3/nonebot_plugin_hx_yinying/__init__.py
--rw-rw-rw-   0        0        0     7723 2024-04-16 20:22:00.000000 nonebot-plugin-hx-yinying-0.3/nonebot_plugin_hx_yinying/chat.py
--rw-rw-rw-   0        0        0      625 2024-04-16 08:05:07.000000 nonebot-plugin-hx-yinying-0.3/nonebot_plugin_hx_yinying/config.py
-drwxrwxrwx   0        0        0        0 2024-04-17 01:18:14.999583 nonebot-plugin-hx-yinying-0.3/nonebot_plugin_hx_yinying.egg-info/
--rw-rw-rw-   0        0        0     2677 2024-04-17 01:18:14.000000 nonebot-plugin-hx-yinying-0.3/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2024-04-17 01:18:14.000000 nonebot-plugin-hx-yinying-0.3/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 01:18:14.000000 nonebot-plugin-hx-yinying-0.3/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2024-04-17 01:18:14.000000 nonebot-plugin-hx-yinying-0.3/nonebot_plugin_hx_yinying.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-17 01:18:14.000000 nonebot-plugin-hx-yinying-0.3/nonebot_plugin_hx_yinying.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      144 2024-04-17 01:18:15.021502 nonebot-plugin-hx-yinying-0.3/setup.cfg
--rw-rw-rw-   0        0        0      836 2024-04-17 01:18:06.000000 nonebot-plugin-hx-yinying-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 01:27:45.352338 nonebot-plugin-hx-yinying-0.4/
+-rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-0.4/LICENSE
+-rw-rw-rw-   0        0        0     2677 2024-04-17 01:27:45.352338 nonebot-plugin-hx-yinying-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2239 2024-04-17 00:42:32.000000 nonebot-plugin-hx-yinying-0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 01:27:45.273482 nonebot-plugin-hx-yinying-0.4/nonebot_plugin_hx_yinying/
+-rw-rw-rw-   0        0        0     1260 2024-04-17 01:00:56.000000 nonebot-plugin-hx-yinying-0.4/nonebot_plugin_hx_yinying/__init__.py
+-rw-rw-rw-   0        0        0     7770 2024-04-17 01:27:29.000000 nonebot-plugin-hx-yinying-0.4/nonebot_plugin_hx_yinying/chat.py
+-rw-rw-rw-   0        0        0      625 2024-04-16 08:05:07.000000 nonebot-plugin-hx-yinying-0.4/nonebot_plugin_hx_yinying/config.py
+drwxrwxrwx   0        0        0        0 2024-04-17 01:27:45.344007 nonebot-plugin-hx-yinying-0.4/nonebot_plugin_hx_yinying.egg-info/
+-rw-rw-rw-   0        0        0     2677 2024-04-17 01:27:44.000000 nonebot-plugin-hx-yinying-0.4/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2024-04-17 01:27:45.000000 nonebot-plugin-hx-yinying-0.4/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 01:27:44.000000 nonebot-plugin-hx-yinying-0.4/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2024-04-17 01:27:44.000000 nonebot-plugin-hx-yinying-0.4/nonebot_plugin_hx_yinying.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-17 01:27:44.000000 nonebot-plugin-hx-yinying-0.4/nonebot_plugin_hx_yinying.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      144 2024-04-17 01:27:45.366793 nonebot-plugin-hx-yinying-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      836 2024-04-17 01:26:38.000000 nonebot-plugin-hx-yinying-0.4/setup.py
```

### Comparing `nonebot-plugin-hx-yinying-0.3/LICENSE` & `nonebot-plugin-hx-yinying-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-0.3/PKG-INFO` & `nonebot-plugin-hx-yinying-0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 0.3
+Version: 0.4
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 0.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 0.4 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE
                                    _[_n_o_n_e_b_o_t_]
                 # nonebot_plugin_hx-yinying _â¨ Hx vs YinYing
```

### Comparing `nonebot-plugin-hx-yinying-0.3/README.md` & `nonebot-plugin-hx-yinying-0.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-0.3/nonebot_plugin_hx_yinying/__init__.py` & `nonebot-plugin-hx-yinying-0.4/nonebot_plugin_hx_yinying/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-0.3/nonebot_plugin_hx_yinying/chat.py` & `nonebot-plugin-hx-yinying-0.4/nonebot_plugin_hx_yinying/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # -- coding: utf-8 --**
 from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent, MessageEvent
 from nonebot.adapters.onebot.v11 import MessageSegment as MS
 from nonebot.matcher import Matcher
 from html import unescape
 import os,httpx, json, datetime, time
 from .config import Config
-from nonebot import get_plugin_config, logger
+from nonebot import get_plugin_config, logger, require
 from datetime import datetime
 hx_config = get_plugin_config(Config)
 from pathlib import Path
+require("nonebot_plugin_localstore")
 import nonebot_plugin_localstore as store
 
 if hx_config.hx_path == None:
     logger.warning("找不到配置里的路径，将使用默认配置")
     history_dir = store.get_data_dir("Hx_YingYing")
     log_dir = Path(f"{history_dir}\yinying_chat\chat").absolute()
     log_dir.mkdir(parents=True, exist_ok=True)
```

### Comparing `nonebot-plugin-hx-yinying-0.3/nonebot_plugin_hx_yinying/config.py` & `nonebot-plugin-hx-yinying-0.4/nonebot_plugin_hx_yinying/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-0.3/nonebot_plugin_hx_yinying.egg-info/PKG-INFO` & `nonebot-plugin-hx-yinying-0.4/nonebot_plugin_hx_yinying.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 0.3
+Version: 0.4
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 0.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 0.4 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE
                                    _[_n_o_n_e_b_o_t_]
                 # nonebot_plugin_hx-yinying _â¨ Hx vs YinYing
```

### Comparing `nonebot-plugin-hx-yinying-0.3/setup.py` & `nonebot-plugin-hx-yinying-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot-plugin-hx-yinying",
-    version="0.3",
+    version="0.4",
     author="Huan Xin",
     author_email="mc.xiaolang@foxmail.com",
     description="chat with yinying",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/huanxin996/nonebot_plugin_hx-yinying",
     packages=setuptools.find_packages(),
```

