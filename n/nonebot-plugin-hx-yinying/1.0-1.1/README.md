# Comparing `tmp/nonebot_plugin_hx-yinying-1.0.tar.gz` & `tmp/nonebot_plugin_hx-yinying-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_hx-yinying-1.0.tar", last modified: Tue Apr 16 18:02:25 2024, max compression
+gzip compressed data, was "nonebot_plugin_hx-yinying-1.1.tar", last modified: Tue Apr 16 20:23:33 2024, max compression
```

## Comparing `nonebot_plugin_hx-yinying-1.0.tar` & `nonebot_plugin_hx-yinying-1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 18:02:25.562609 nonebot_plugin_hx-yinying-1.0/
--rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot_plugin_hx-yinying-1.0/LICENSE
--rw-rw-rw-   0        0        0     2925 2024-04-16 18:02:25.563645 nonebot_plugin_hx-yinying-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2487 2024-04-16 17:05:31.000000 nonebot_plugin_hx-yinying-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 18:02:25.458307 nonebot_plugin_hx-yinying-1.0/nonebot_plugin_hx-yinying/
--rw-rw-rw-   0        0        0     1268 2024-04-16 16:52:55.000000 nonebot_plugin_hx-yinying-1.0/nonebot_plugin_hx-yinying/__init__.py
--rw-rw-rw-   0        0        0     5467 2024-04-16 15:59:07.000000 nonebot_plugin_hx-yinying-1.0/nonebot_plugin_hx-yinying/chat.py
--rw-rw-rw-   0        0        0      627 2024-04-16 18:01:40.000000 nonebot_plugin_hx-yinying-1.0/nonebot_plugin_hx-yinying/config.py
-drwxrwxrwx   0        0        0        0 2024-04-16 18:02:25.540230 nonebot_plugin_hx-yinying-1.0/nonebot_plugin_hx_yinying.egg-info/
--rw-rw-rw-   0        0        0     2925 2024-04-16 18:02:25.000000 nonebot_plugin_hx-yinying-1.0/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2024-04-16 18:02:25.000000 nonebot_plugin_hx-yinying-1.0/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 18:02:25.000000 nonebot_plugin_hx-yinying-1.0/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2024-04-16 18:02:25.000000 nonebot_plugin_hx-yinying-1.0/nonebot_plugin_hx_yinying.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-16 18:02:25.000000 nonebot_plugin_hx-yinying-1.0/nonebot_plugin_hx_yinying.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-04-16 18:02:25.573597 nonebot_plugin_hx-yinying-1.0/setup.cfg
--rw-rw-rw-   0        0        0      836 2024-04-16 18:01:56.000000 nonebot_plugin_hx-yinying-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 20:23:33.334412 nonebot_plugin_hx-yinying-1.1/
+-rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot_plugin_hx-yinying-1.1/LICENSE
+-rw-rw-rw-   0        0        0     2925 2024-04-16 20:23:33.334412 nonebot_plugin_hx-yinying-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2487 2024-04-16 17:05:31.000000 nonebot_plugin_hx-yinying-1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 20:23:33.234456 nonebot_plugin_hx-yinying-1.1/nonebot_plugin_hx-yinying/
+-rw-rw-rw-   0        0        0     1268 2024-04-16 16:52:55.000000 nonebot_plugin_hx-yinying-1.1/nonebot_plugin_hx-yinying/__init__.py
+-rw-rw-rw-   0        0        0     7721 2024-04-16 20:22:46.000000 nonebot_plugin_hx-yinying-1.1/nonebot_plugin_hx-yinying/chat.py
+-rw-rw-rw-   0        0        0      627 2024-04-16 18:01:40.000000 nonebot_plugin_hx-yinying-1.1/nonebot_plugin_hx-yinying/config.py
+drwxrwxrwx   0        0        0        0 2024-04-16 20:23:33.334412 nonebot_plugin_hx-yinying-1.1/nonebot_plugin_hx_yinying.egg-info/
+-rw-rw-rw-   0        0        0     2925 2024-04-16 20:23:32.000000 nonebot_plugin_hx-yinying-1.1/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2024-04-16 20:23:32.000000 nonebot_plugin_hx-yinying-1.1/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 20:23:32.000000 nonebot_plugin_hx-yinying-1.1/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2024-04-16 20:23:32.000000 nonebot_plugin_hx-yinying-1.1/nonebot_plugin_hx_yinying.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-16 20:23:32.000000 nonebot_plugin_hx-yinying-1.1/nonebot_plugin_hx_yinying.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-04-16 20:23:33.351196 nonebot_plugin_hx-yinying-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      836 2024-04-16 20:23:29.000000 nonebot_plugin_hx-yinying-1.1/setup.py
```

### Comparing `nonebot_plugin_hx-yinying-1.0/LICENSE` & `nonebot_plugin_hx-yinying-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_hx-yinying-1.0/PKG-INFO` & `nonebot_plugin_hx-yinying-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_hx-yinying
-Version: 1.0
+Version: 1.1
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx_yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_hx-yinying Version: 1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_hx-yinying Version: 1.1 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/
 nonebot_plugin_hx_yinying Author: Huan Xin Author-email:
 mc.xiaolang@foxmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Description-Content-Type: text/markdown License-File: LICENSE
                                    _[_n_o_n_e_b_o_t_]
                 # nonebot_plugin_hx-yinying _â¨ Hx vs YinYing
```

### Comparing `nonebot_plugin_hx-yinying-1.0/README.md` & `nonebot_plugin_hx-yinying-1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_hx-yinying-1.0/nonebot_plugin_hx-yinying/__init__.py` & `nonebot_plugin_hx-yinying-1.1/nonebot_plugin_hx-yinying/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_hx-yinying-1.0/nonebot_plugin_hx-yinying/chat.py` & `nonebot_plugin_hx-yinying-1.1/nonebot_plugin_hx-yinying/chat.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -- coding: utf-8 --**
-__author__ = "HuanXin"
 from nonebot.adapters.onebot.v11 import Bot, GroupMessageEvent, MessageEvent
 from nonebot.adapters.onebot.v11 import MessageSegment as MS
 from nonebot.matcher import Matcher
 from html import unescape
-import os,httpx, json, datetime
+import os,httpx, json, datetime, time
 from .config import Config
 from nonebot import get_plugin_config, logger
 from datetime import datetime
 hx_config = get_plugin_config(Config)
 from pathlib import Path
 import nonebot_plugin_localstore as store
 
@@ -19,14 +18,15 @@
     log_dir.mkdir(parents=True, exist_ok=True)
 else:
     logger.success("找到配置里的路径，载入成功")
     history_dir = store.get_data_dir(f"{hx_config.hx_path}")
     log_dir = Path(f"{history_dir}\yinying_chat\chat").absolute()
     log_dir.mkdir(parents=True, exist_ok=True)
 
+
 #创建用户文件夹
 def create_dir_usr(path):
     if not os.path.exists(path):
         os.mkdir(path)
 
 #用户输入
 def user_in(id, text):
@@ -44,14 +44,52 @@
         with open(f'{log_dir}\{id}\content.json','a',encoding='utf-8') as file:
             file.write(',\n{"role": "assistant", "content": "' + text + '"}')
     else:
         create_dir_usr(f"{log_dir}\{id}")
         with open(f'{log_dir}\{id}\content.json','w',encoding='utf-8') as file:
             file.write('{"role": "assistant", "content": "' + text + '"}')
 
+#存储对话次数
+def chat_times(id):
+    if os.path.exists(f'{log_dir}/{id}/times.json'):
+        with open(f"{log_dir}/{id}/times.json",'a',encoding='utf-8') as file:
+                with open(f'{log_dir}/{id}/times.json','r',encoding='utf-8') as file:
+                    data = json.load(file)
+                    data["times"] = data["times"] + 1
+                    data.update(file)
+                with open(f'{log_dir}/{id}/times.json','w',encoding='utf-8') as file:
+                    json.dump(data, file)
+    else:
+        with open(f'{log_dir}/{id}/times.json','w',encoding='utf-8') as file:
+                with open(f'{log_dir}/{id}/times.json','w',encoding='utf-8') as file:
+                    old_data = {}
+                    dt = time.time()
+                    t = int(dt)
+                    data = {"times":0,"time":t}
+                    old_data.update(data)
+                with open(f'{log_dir}/{id}/times.json','w',encoding='utf-8') as file:
+                    json.dump(data, file)
+                    return 0
+
+
+
+#存储对话次数
+def chat_clear(id):
+    with open(f"{log_dir}/{id}/times.json",'a',encoding='utf-8') as file:
+        with open(f'{log_dir}/{id}/times.json','r',encoding='utf-8') as file:
+            data = json.load(file)
+            dt = time.time()
+            t = int(dt)
+            data["times"] = 0
+            data["time"] = t
+            data.update(file)
+        with open(f'{log_dir}/{id}/times.json','w',encoding='utf-8') as file:
+            json.dump(data, file)
+            return True
+     
 
 
 async def gen_chat_text(event: MessageEvent, bot: Bot) -> str:
     msg = ""
     for seg in event.message:
         if seg.is_text():
             msg += seg.data.get("text", "")
@@ -104,50 +142,62 @@
         res_raw = res['choices'][0]['message']['content']
     except Exception as e:
         res_raw = res
     return res_raw
 
 
 async def yinying(text,id):
-    user_in(id,text)
-    headers = {
+    chat_times(id)
+    with open(f'{log_dir}/{id}/times.json','r',encoding='utf-8') as file:
+        data = json.load(file)
+        times_yinying = data["times"]
+        time = data["time"]
+        headers = {
         'Content-type': 'application/json',
         'Authorization': f'Bearer {hx_config.yinying_token}'
     }
-    data = {
+        data = {
                 'appId':'huanxinbot',
-                'chatId':'huanxinbot-3485462167-ces',
+                'chatId':f'huanxinbot-{id}-{time}',
                 'model':f'{hx_config.yinying_model}',
                 'variables':{'nickName': '幻歆','furryCharacter': '一只猫猫龙'},
                 'message':f'{text}'
                 }
-    async with httpx.AsyncClient(timeout=httpx.Timeout(connect=10, read=60, write=20, pool=30)) as client:
-            back = await client.post(hx_config.hx_api_yinying, headers=headers, json=data)
-    try:
-            back = back.json()
-    except json.decoder.JSONDecodeError as e:
-            back_msg = f"请求接口报错！\n返回结果：{e}"
-            return back_msg
-    try:
-        back_msg = back['choices'][0]['message']['content']
-    except Exception as e:
-        back_msg = back
-    return back_msg
+        async with httpx.AsyncClient(timeout=httpx.Timeout(connect=10, read=60, write=20, pool=30)) as client:
+                back = await client.post(hx_config.hx_api_yinying, headers=headers, json=data)
+        try:
+                back = back.json()
+        except json.decoder.JSONDecodeError as e:
+                back_msg = f"请求接口报错！\t返回结果：{e}"
+                return back_msg
+        try:
+            if times_yinying>=hx_config.yinying_limit:
+                msg = back['choices'][0]['message']['content']
+                back_msg = f"[对话次数达到上限，即将清空缓存.]\t{msg}"
+                user_in(id,text)
+                ai_out(id,msg)
+                chat_clear(id)
+            else:
+                msg = back['choices'][0]['message']['content']
+                back_msg = f"[{times_yinying}|{hx_config.yinying_limit}]{msg}"
+                user_in(id,text)
+                ai_out(id,msg)
+        except Exception as e:
+                back_msg = back
+        return back_msg
     
 
 
 async def get_answer(matcher: Matcher, event: MessageEvent, bot: Bot):
     text = unescape(await gen_chat_text(event, bot))
     id = get_id(event)
     try:
         back_msg = str(await yinying(text,id))
         msg = back_msg.replace("\n","\\n")
-        ai_out(id,msg)
         await send_with_at(matcher,msg)
     except httpx.HTTPError as e:
-        back_msg = f"请求接口报错！\n返回结果：{e}"
+        back_msg = f"请求接口报错！\t返回结果：{e}"
         await finish_with_at(matcher, back_msg)
 
 
 
 
-
```

### Comparing `nonebot_plugin_hx-yinying-1.0/nonebot_plugin_hx-yinying/config.py` & `nonebot_plugin_hx-yinying-1.1/nonebot_plugin_hx-yinying/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_hx-yinying-1.0/nonebot_plugin_hx_yinying.egg-info/PKG-INFO` & `nonebot_plugin_hx-yinying-1.1/nonebot_plugin_hx_yinying.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 1.0
+Version: 1.1
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx_yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 1.1 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/
 nonebot_plugin_hx_yinying Author: Huan Xin Author-email:
 mc.xiaolang@foxmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Description-Content-Type: text/markdown License-File: LICENSE
                                    _[_n_o_n_e_b_o_t_]
                 # nonebot_plugin_hx-yinying _â¨ Hx vs YinYing
```

### Comparing `nonebot_plugin_hx-yinying-1.0/setup.py` & `nonebot_plugin_hx-yinying-1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot_plugin_hx-yinying",
-    version="1.0",
+    version="1.1",
     author="Huan Xin",
     author_email="mc.xiaolang@foxmail.com",
     description="chat with yinying",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/huanxin996/nonebot_plugin_hx_yinying",
     packages=setuptools.find_packages(),
```

