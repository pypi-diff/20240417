# Comparing `tmp/nonebot-plugin-hx-yinying-0.0.3.tar.gz` & `tmp/nonebot-plugin-hx-yinying-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-hx-yinying-0.0.3.tar", last modified: Wed Apr 17 13:19:02 2024, max compression
+gzip compressed data, was "nonebot-plugin-hx-yinying-0.0.4.tar", last modified: Wed Apr 17 16:02:55 2024, max compression
```

## Comparing `nonebot-plugin-hx-yinying-0.0.3.tar` & `nonebot-plugin-hx-yinying-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 13:19:02.463190 nonebot-plugin-hx-yinying-0.0.3/
--rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     3179 2024-04-17 13:19:02.480025 nonebot-plugin-hx-yinying-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2731 2024-04-17 08:20:26.000000 nonebot-plugin-hx-yinying-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 13:19:02.396695 nonebot-plugin-hx-yinying-0.0.3/nonebot_plugin_hx_yinying/
--rw-rw-rw-   0        0        0     1330 2024-04-17 07:14:59.000000 nonebot-plugin-hx-yinying-0.0.3/nonebot_plugin_hx_yinying/__init__.py
--rw-rw-rw-   0        0        0     7601 2024-04-17 13:15:48.000000 nonebot-plugin-hx-yinying-0.0.3/nonebot_plugin_hx_yinying/chat.py
--rw-rw-rw-   0        0        0      544 2024-04-17 06:08:40.000000 nonebot-plugin-hx-yinying-0.0.3/nonebot_plugin_hx_yinying/config.py
-drwxrwxrwx   0        0        0        0 2024-04-17 13:19:02.463190 nonebot-plugin-hx-yinying-0.0.3/nonebot_plugin_hx_yinying.egg-info/
--rw-rw-rw-   0        0        0     3179 2024-04-17 13:19:01.000000 nonebot-plugin-hx-yinying-0.0.3/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2024-04-17 13:19:02.000000 nonebot-plugin-hx-yinying-0.0.3/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 13:19:01.000000 nonebot-plugin-hx-yinying-0.0.3/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      124 2024-04-17 13:19:01.000000 nonebot-plugin-hx-yinying-0.0.3/nonebot_plugin_hx_yinying.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-17 13:19:01.000000 nonebot-plugin-hx-yinying-0.0.3/nonebot_plugin_hx_yinying.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-04-17 13:19:02.480025 nonebot-plugin-hx-yinying-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      840 2024-04-17 13:18:43.000000 nonebot-plugin-hx-yinying-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 16:02:55.579310 nonebot-plugin-hx-yinying-0.0.4/
+-rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     3353 2024-04-17 16:02:55.580311 nonebot-plugin-hx-yinying-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2913 2024-04-17 15:39:35.000000 nonebot-plugin-hx-yinying-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 16:02:55.474057 nonebot-plugin-hx-yinying-0.0.4/nonebot_plugin_hx_yinying/
+-rw-rw-rw-   0        0        0     1330 2024-04-17 07:14:59.000000 nonebot-plugin-hx-yinying-0.0.4/nonebot_plugin_hx_yinying/__init__.py
+-rw-rw-rw-   0        0        0     7633 2024-04-17 15:38:59.000000 nonebot-plugin-hx-yinying-0.0.4/nonebot_plugin_hx_yinying/chat.py
+-rw-rw-rw-   0        0        0      597 2024-04-17 15:33:44.000000 nonebot-plugin-hx-yinying-0.0.4/nonebot_plugin_hx_yinying/config.py
+drwxrwxrwx   0        0        0        0 2024-04-17 16:02:55.571306 nonebot-plugin-hx-yinying-0.0.4/nonebot_plugin_hx_yinying.egg-info/
+-rw-rw-rw-   0        0        0     3353 2024-04-17 16:02:55.000000 nonebot-plugin-hx-yinying-0.0.4/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2024-04-17 16:02:55.000000 nonebot-plugin-hx-yinying-0.0.4/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 16:02:55.000000 nonebot-plugin-hx-yinying-0.0.4/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      124 2024-04-17 16:02:55.000000 nonebot-plugin-hx-yinying-0.0.4/nonebot_plugin_hx_yinying.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-17 16:02:55.000000 nonebot-plugin-hx-yinying-0.0.4/nonebot_plugin_hx_yinying.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-04-17 16:02:55.590216 nonebot-plugin-hx-yinying-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      840 2024-04-17 16:02:50.000000 nonebot-plugin-hx-yinying-0.0.4/setup.py
```

### Comparing `nonebot-plugin-hx-yinying-0.0.3/LICENSE` & `nonebot-plugin-hx-yinying-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-0.0.3/PKG-INFO` & `nonebot-plugin-hx-yinying-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 0.0.3
+Version: 0.0.4
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -86,18 +86,24 @@
 
 
 ## hx_path
 - 类型：`str`
 - 默认值：`None`
 - 说明：银影对话的用户数据存储路径(不写将使用默认配置)
 
+## hx_reply
+- 类型：`bool`
+- 默认值：`False`
+- 说明：bot发送chat消息时是否回复
+- 注意：该项启用时hx_reply_at将被忽略
+
 ## hx_reply_at
 - 类型：`bool`
 - 默认值：`False`
-- 说明：bot回复消息是否艾特
+- 说明：bot发送chat消息时不回复时是否艾特
 
 ## yinying_limit
 - 类型：`int`
 - 默认值：`12`
 - 说明：对于银影对话限制的次数
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 0.0.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 0.0.4 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-0-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin * @Date : 2024-4-17 00:04:25 *
@@ -19,13 +19,16 @@
 å¨å±éç½®æä»¶ä¸­æ·»å ä»¥ä¸éç½®é¡¹å³å¯ã ### yinying_model -
 ç±»åï¼`str` - é»è®¤å¼ï¼`None` - è¯´æï¼éæ©ä½¿ç¨é¶å½±çæ¨¡å ###
 yinying_token - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼è¿éåä½ æ¾ç§©ä¹±è·åå°çapi_key ### hx_api_yinying -
 ç±»åï¼`str` - é»è®¤å¼ï¼`None` - è¯´æï¼yinyingçapiå°å ## hx_path -
 ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼é¶å½±å¯¹è¯çç¨æ·æ°æ®å­å¨è·¯å¾(ä¸åå°ä½¿ç¨é»è®¤éç½®)
-## hx_reply_at - ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
-è¯´æï¼botåå¤æ¶æ¯æ¯å¦è¾ç¹ ## yinying_limit - ç±»åï¼`int` -
-é»è®¤å¼ï¼`12` - è¯´æï¼å¯¹äºé¶å½±å¯¹è¯éå¶çæ¬¡æ°
+## hx_reply - ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
+è¯´æï¼botåéchatæ¶æ¯æ¶æ¯å¦åå¤ -
+æ³¨æï¼è¯¥é¡¹å¯ç¨æ¶hx_reply_atå°è¢«å¿½ç¥ ## hx_reply_at -
+ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
+è¯´æï¼botåéchatæ¶æ¯æ¶ä¸åå¤æ¶æ¯å¦è¾ç¹ ## yinying_limit -
+ç±»åï¼`int` - é»è®¤å¼ï¼`12` - è¯´æï¼å¯¹äºé¶å½±å¯¹è¯éå¶çæ¬¡æ°
 éç½®æä»¶ç¤ºä¾ï¼é»è®¤æ¨¡æ¿ï¼ ```dotenv hx_api_yinying=https://å°å
 yinying_model=æ¨¡å yinying_token=ä½ çtoken(ä¸å¸¦bearer) hx_reply_at=False
 yinying_limit=12 ``` ## Contributors â¨
```

### Comparing `nonebot-plugin-hx-yinying-0.0.3/README.md` & `nonebot-plugin-hx-yinying-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <!--
-<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-0-orange.svg?style=flat-square)](#contributors-)
+<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
+[![All Contributors](https://img.shields.io/badge/all_contributors-0-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
  * @Author         : huanxin
  * @Date           : 2024-4-17 00:04:25
  * @LastEditors    : huanxin
  * @LastEditTime   : 2024-4-17 00:04:25
  * @Description    : None
  * @GitHub         : https://github.com/huanxin
@@ -73,18 +73,24 @@
 
 
 ## hx_path
 - 类型：`str`
 - 默认值：`None`
 - 说明：银影对话的用户数据存储路径(不写将使用默认配置)
 
+## hx_reply
+- 类型：`bool`
+- 默认值：`False`
+- 说明：bot发送chat消息时是否回复
+- 注意：该项启用时hx_reply_at将被忽略
+
 ## hx_reply_at
 - 类型：`bool`
 - 默认值：`False`
-- 说明：bot回复消息是否艾特
+- 说明：bot发送chat消息时不回复时是否艾特
 
 ## yinying_limit
 - 类型：`int`
 - 默认值：`12`
 - 说明：对于银影对话限制的次数
 
 
@@ -98,15 +104,15 @@
 yinying_limit=12
 ```
 
 
 ## Contributors ✨
 
 
-<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
-<!-- prettier-ignore-start -->
-<!-- markdownlint-disable -->
-<!-- markdownlint-restore -->
-<!-- prettier-ignore-end -->
-
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

#### html2text {}

```diff
@@ -13,13 +13,16 @@
 å¨å±éç½®æä»¶ä¸­æ·»å ä»¥ä¸éç½®é¡¹å³å¯ã ### yinying_model -
 ç±»åï¼`str` - é»è®¤å¼ï¼`None` - è¯´æï¼éæ©ä½¿ç¨é¶å½±çæ¨¡å ###
 yinying_token - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼è¿éåä½ æ¾ç§©ä¹±è·åå°çapi_key ### hx_api_yinying -
 ç±»åï¼`str` - é»è®¤å¼ï¼`None` - è¯´æï¼yinyingçapiå°å ## hx_path -
 ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼é¶å½±å¯¹è¯çç¨æ·æ°æ®å­å¨è·¯å¾(ä¸åå°ä½¿ç¨é»è®¤éç½®)
-## hx_reply_at - ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
-è¯´æï¼botåå¤æ¶æ¯æ¯å¦è¾ç¹ ## yinying_limit - ç±»åï¼`int` -
-é»è®¤å¼ï¼`12` - è¯´æï¼å¯¹äºé¶å½±å¯¹è¯éå¶çæ¬¡æ°
+## hx_reply - ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
+è¯´æï¼botåéchatæ¶æ¯æ¶æ¯å¦åå¤ -
+æ³¨æï¼è¯¥é¡¹å¯ç¨æ¶hx_reply_atå°è¢«å¿½ç¥ ## hx_reply_at -
+ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
+è¯´æï¼botåéchatæ¶æ¯æ¶ä¸åå¤æ¶æ¯å¦è¾ç¹ ## yinying_limit -
+ç±»åï¼`int` - é»è®¤å¼ï¼`12` - è¯´æï¼å¯¹äºé¶å½±å¯¹è¯éå¶çæ¬¡æ°
 éç½®æä»¶ç¤ºä¾ï¼é»è®¤æ¨¡æ¿ï¼ ```dotenv hx_api_yinying=https://å°å
 yinying_model=æ¨¡å yinying_token=ä½ çtoken(ä¸å¸¦bearer) hx_reply_at=False
 yinying_limit=12 ``` ## Contributors â¨
```

### Comparing `nonebot-plugin-hx-yinying-0.0.3/nonebot_plugin_hx_yinying/__init__.py` & `nonebot-plugin-hx-yinying-0.0.4/nonebot_plugin_hx_yinying/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-0.0.3/nonebot_plugin_hx_yinying/chat.py` & `nonebot-plugin-hx-yinying-0.0.4/nonebot_plugin_hx_yinying/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -- coding: utf-8 --**
-from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent, MessageEvent
+from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent, MessageEvent ,MessageSegment
 from nonebot.adapters.onebot.v11 import MessageSegment as MS
 from nonebot.matcher import Matcher
 from html import unescape
 import os,httpx, json, datetime, time
 from .config import Config
 from nonebot import get_plugin_config, logger, require
 from datetime import datetime
@@ -131,21 +131,20 @@
     nick = info["nickname"]
     if nick is None:
         nick = None
     else:
         nick = nick
     return nick
 
-async def send_with_at(matcher: Matcher, content):
-    await matcher.send(content, at_sender=hx_config.hx_reply_at)
-
-
-async def finish_with_at(matcher: Matcher, content):
-    await matcher.finish(content, at_sender=hx_config.hx_reply_at)
 
+async def send_msg(matcher: Matcher, event: MessageEvent, content):
+    if hx_config.hx_reply == True:
+        await matcher.send(MessageSegment.reply(event.message_id) + content)
+    else:
+        await matcher.send(content, at_sender=hx_config.hx_reply_at)
 
 async def yinying(text,id,nick):
     chat_times(id)
     with open(f'{log_dir}/{id}/times.json','r',encoding='utf-8') as file:
         data = json.load(file)
         times_yinying = data["times"]
         character = data["character"]
@@ -189,11 +188,11 @@
 async def get_answer(matcher: Matcher, event: MessageEvent, bot: Bot):
     text = unescape(await gen_chat_text(event, bot))
     id = get_id(event)
     nick = await get_nick(bot,event)
     try:
         back_msg = str(await yinying(text,id,nick))
         msg = back_msg.replace("\n","\\n")
-        await send_with_at(matcher,msg)
+        await send_msg(matcher,event,msg)
     except httpx.HTTPError as e:
         back_msg = f"请求接口报错！\t返回结果：{e}"
-        await finish_with_at(matcher, back_msg)
+        await send_msg(matcher, back_msg)
```

### Comparing `nonebot-plugin-hx-yinying-0.0.3/nonebot_plugin_hx_yinying/config.py` & `nonebot-plugin-hx-yinying-0.0.4/nonebot_plugin_hx_yinying/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,11 +15,13 @@
     yinying_token: Optional[str] = None
 
     # api地址
     hx_api_yinying: Optional[str] = None
     hx_path: Optional[str] = None
     # bot回复消息时是否艾特
     hx_reply_at: bool = False
+    #是否回复消息
+    hx_reply: bool = False
 
     yinying_limit: int = 12
 
 global_config = nonebot.get_driver().config
```

### Comparing `nonebot-plugin-hx-yinying-0.0.3/nonebot_plugin_hx_yinying.egg-info/PKG-INFO` & `nonebot-plugin-hx-yinying-0.0.4/nonebot_plugin_hx_yinying.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 0.0.3
+Version: 0.0.4
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -86,18 +86,24 @@
 
 
 ## hx_path
 - 类型：`str`
 - 默认值：`None`
 - 说明：银影对话的用户数据存储路径(不写将使用默认配置)
 
+## hx_reply
+- 类型：`bool`
+- 默认值：`False`
+- 说明：bot发送chat消息时是否回复
+- 注意：该项启用时hx_reply_at将被忽略
+
 ## hx_reply_at
 - 类型：`bool`
 - 默认值：`False`
-- 说明：bot回复消息是否艾特
+- 说明：bot发送chat消息时不回复时是否艾特
 
 ## yinying_limit
 - 类型：`int`
 - 默认值：`12`
 - 说明：对于银影对话限制的次数
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 0.0.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 0.0.4 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown License-File: LICENSE [![All Contributors](https://
 img.shields.io/badge/all_contributors-0-orange.svg?style=flat-square)]
 (#contributors-) * @Author : huanxin * @Date : 2024-4-17 00:04:25 *
@@ -19,13 +19,16 @@
 å¨å±éç½®æä»¶ä¸­æ·»å ä»¥ä¸éç½®é¡¹å³å¯ã ### yinying_model -
 ç±»åï¼`str` - é»è®¤å¼ï¼`None` - è¯´æï¼éæ©ä½¿ç¨é¶å½±çæ¨¡å ###
 yinying_token - ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼è¿éåä½ æ¾ç§©ä¹±è·åå°çapi_key ### hx_api_yinying -
 ç±»åï¼`str` - é»è®¤å¼ï¼`None` - è¯´æï¼yinyingçapiå°å ## hx_path -
 ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼é¶å½±å¯¹è¯çç¨æ·æ°æ®å­å¨è·¯å¾(ä¸åå°ä½¿ç¨é»è®¤éç½®)
-## hx_reply_at - ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
-è¯´æï¼botåå¤æ¶æ¯æ¯å¦è¾ç¹ ## yinying_limit - ç±»åï¼`int` -
-é»è®¤å¼ï¼`12` - è¯´æï¼å¯¹äºé¶å½±å¯¹è¯éå¶çæ¬¡æ°
+## hx_reply - ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
+è¯´æï¼botåéchatæ¶æ¯æ¶æ¯å¦åå¤ -
+æ³¨æï¼è¯¥é¡¹å¯ç¨æ¶hx_reply_atå°è¢«å¿½ç¥ ## hx_reply_at -
+ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
+è¯´æï¼botåéchatæ¶æ¯æ¶ä¸åå¤æ¶æ¯å¦è¾ç¹ ## yinying_limit -
+ç±»åï¼`int` - é»è®¤å¼ï¼`12` - è¯´æï¼å¯¹äºé¶å½±å¯¹è¯éå¶çæ¬¡æ°
 éç½®æä»¶ç¤ºä¾ï¼é»è®¤æ¨¡æ¿ï¼ ```dotenv hx_api_yinying=https://å°å
 yinying_model=æ¨¡å yinying_token=ä½ çtoken(ä¸å¸¦bearer) hx_reply_at=False
 yinying_limit=12 ``` ## Contributors â¨
```

### Comparing `nonebot-plugin-hx-yinying-0.0.3/setup.py` & `nonebot-plugin-hx-yinying-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot-plugin-hx-yinying",
-    version="0.0.3",
+    version="0.0.4",
     author="Huan Xin",
     author_email="mc.xiaolang@foxmail.com",
     description="chat with yinying",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/huanxin996/nonebot_plugin_hx-yinying",
     packages=setuptools.find_packages(),
```

