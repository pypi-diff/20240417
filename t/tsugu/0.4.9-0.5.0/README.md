# Comparing `tmp/tsugu-0.4.9.tar.gz` & `tmp/tsugu-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-0.4.9.tar", last modified: Tue Apr 16 01:13:29 2024, max compression
+gzip compressed data, was "tsugu-0.5.0.tar", last modified: Wed Apr 17 06:31:17 2024, max compression
```

## Comparing `tsugu-0.4.9.tar` & `tsugu-0.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:13:29.890428 tsugu-0.4.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-16 01:13:20.000000 tsugu-0.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-16 01:13:29.890428 tsugu-0.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-16 01:13:20.000000 tsugu-0.4.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 01:13:29.890428 tsugu-0.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-16 01:13:20.000000 tsugu-0.4.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:13:29.890428 tsugu-0.4.9/test/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-16 01:13:20.000000 tsugu-0.4.9/test/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:13:29.890428 tsugu-0.4.9/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-16 01:13:20.000000 tsugu-0.4.9/tsugu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11131 2024-04-16 01:13:20.000000 tsugu-0.4.9/tsugu/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)    21286 2024-04-16 01:13:20.000000 tsugu-0.4.9/tsugu/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-04-16 01:13:20.000000 tsugu-0.4.9/tsugu/router.py
--rw-r--r--   0 runner    (1001) docker     (127)    21225 2024-04-16 01:13:20.000000 tsugu-0.4.9/tsugu/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:13:29.890428 tsugu-0.4.9/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-16 01:13:29.000000 tsugu-0.4.9/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-16 01:13:29.000000 tsugu-0.4.9/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 01:13:29.000000 tsugu-0.4.9/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 01:13:29.000000 tsugu-0.4.9/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 01:13:29.000000 tsugu-0.4.9/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:31:17.090951 tsugu-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-17 06:31:07.000000 tsugu-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-17 06:31:17.090951 tsugu-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-17 06:31:07.000000 tsugu-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 06:31:17.090951 tsugu-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-17 06:31:07.000000 tsugu-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:31:17.090951 tsugu-0.5.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-17 06:31:07.000000 tsugu-0.5.0/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:31:17.090951 tsugu-0.5.0/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-17 06:31:07.000000 tsugu-0.5.0/tsugu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21286 2024-04-17 06:31:07.000000 tsugu-0.5.0/tsugu/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12003 2024-04-17 06:31:07.000000 tsugu-0.5.0/tsugu/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-04-17 06:31:07.000000 tsugu-0.5.0/tsugu/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21534 2024-04-17 06:31:07.000000 tsugu-0.5.0/tsugu/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:31:17.090951 tsugu-0.5.0/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-17 06:31:16.000000 tsugu-0.5.0/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-17 06:31:17.000000 tsugu-0.5.0/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:31:16.000000 tsugu-0.5.0/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 06:31:16.000000 tsugu-0.5.0/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 06:31:16.000000 tsugu-0.5.0/tsugu.egg-info/top_level.txt
```

### Comparing `tsugu-0.4.9/LICENSE` & `tsugu-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.9/PKG-INFO` & `tsugu-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.4.9
+Version: 0.5.0
 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
         <h1 align="center"> Tsugu Python Frontend <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu Version: 0.4.9 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.5.0 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

### Comparing `tsugu-0.4.9/README.md` & `tsugu-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.9/setup.py` & `tsugu-0.5.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='0.4.9',
+    version='0.5.0',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py',
@@ -17,12 +17,13 @@
     classifiers=[
         'Programming Language :: Python :: 3.8',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent'
     ],
     install_requires=[
             "urllib3",
+            "loguru",
         ],
     python_requires='>=3.8',
     include_package_data=False,
 
 )
```

### Comparing `tsugu-0.4.9/test/test_main.py` & `tsugu-0.5.0/test/test_main.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.9/tsugu/bot.py` & `tsugu-0.5.0/tsugu/handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,22 @@
+import base64
+from typing import List, Union
+
 from .utils import *
 
 
 def bot(message, user_id, platform, channel_id):
+    '''
+    不再建议直接使用此函数，请使用 handler 函数
+    :param message:
+    :param user_id:
+    :param platform:
+    :param channel_id:
+    :return:
+    '''
     try:
         message = message.strip()
 
         # help
         if config.features.get('help', True):
             if message.startswith('帮助'):
                 return help_command()
@@ -26,19 +37,38 @@
         command_matched, api = match_command(message, load_commands_from_config(config.commands))
         if command_matched:
             return v2_api_command(message, command_matched, api, platform, user_id, channel_id)
         if config.user_database_path:
             return bot_extra_local_database(message, user_id, platform)
         return bot_extra_remote_server(message, user_id, platform)
     except Exception as e:
-        print(e)
-        raise e
+        logger.error(f'Error: {e}')
+        # raise e
         return []
 
 
+def handler(message: str, user_id: str, platform: str, channel_id: str) -> List[Union[bytes, str]]:
+    '''
+    :param message: 用户消息
+    :param user_id: 用户ID
+    :param platform: 平台名称 默认 red
+    :param channel_id: 频道ID / 群号
+    :return: List[Union[bytes, str]] bytes 为图片 str 为文字
+    '''
+    data = bot(message, user_id, platform, channel_id)
+    response = []
+    for item in data:
+        if item['type'] == 'string':
+            response.append(item['string'].encode('utf-8'))
+        elif item['type'] == 'base64':
+            bytes_data = base64.b64decode(item['string'].encode('utf-8'))
+            response.append(bytes_data)
+    return response
+
+
 def bot_extra_local_database(message, user_id, platform):
     # 玩家状态
     if config.features.get('player_status', True):
         if message.endswith('服玩家状态'):
             return player_status(user_id, platform, message[:-4]) if server_exists(r_ := query_server_info(message[:-4])) else text_response('未找到被指定的服务器') if len(message) <= 7 else None
 
         if message.startswith('玩家状态'):
@@ -64,15 +94,14 @@
             arg = message.replace('验证', '').strip()
             # 正则出数字
             player_ids = re.findall(r'\d+', arg)
             if not player_ids or len(player_ids) > 1:
                 return text_response('请确保输入正确(例如: 验证 10000xxxxx cn)')
             player_id = player_ids[0]
             server = query_server_info(arg.replace(player_id, ''))  # 后续自动处理 None
-            # print(server, type(server))
             return bind_player_verification(platform, user_id, server, player_id, True)
 
         if message.startswith('解除绑定'):
             if message[4:].strip() == '':
                 return unbind_player_request(platform, user_id)
             msg_list = message.split(' ')
             if len(msg_list) < 2:
@@ -125,15 +154,14 @@
             # 如果匹配 绑定玩家 则绑定默认服务器的玩家 如果用户输入了服务器名 则绑定对应服务器的玩家，如果服务器名无效则 赋值为 None
             server = Remote.get_user_data(platform, user_id)['data']['server_mode'] if message[4:].strip() == '' else (r_ if server_exists(r_ := query_server_info(message[4:])) else None)
             if not server_exists(server):
                 return text_response(f'未找到名为 {(message[4:]).strip()} 的服务器信息，请确保输入的是服务器名而不是玩家ID，通常情况发送"绑定玩家"即可')
 
             res = Remote.bind_player_request(platform, user_id, server, True)
             if res.get('status') != 'success':
-                # print(res)
                 # {'status': 'success', 'data': {'verifyCode': 12492}}
                 return text_response(res.get('data'))
             # if not res.get('status') == 'failed':
             #     return text_response('未知错误喵')
             return text_response(f'''正在绑定账号，请将 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{res.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证 + 空格 + 玩家ID 来完成本次身份验证\n验证 10000xxxx 国服''')
 
         if message.startswith('解除绑定'):
```

### Comparing `tsugu-0.4.9/tsugu/config.py` & `tsugu-0.5.0/tsugu/config.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.9/tsugu/router.py` & `tsugu-0.5.0/tsugu/router.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,23 +63,23 @@
         return v2api_from_backend('ycm', text, default_servers, server)
 
     @staticmethod
     def card_illustration(text: str, default_servers: List[int], server: int):
         return v2api_from_backend('cardIllustration', text, default_servers, server)
 
     @staticmethod
-    def bind_player_request(platform: str, user_id: str, server: int, status: bool):
-        return bind_player_request(platform, user_id, server, status)
+    def bind_player_request(platform: str, user_id: str):
+        return bind_player_request(platform, user_id)
 
     @staticmethod
     def bind_player_verification(platform: str, user_id: str, server: int, player_id: str, status: bool):
         return bind_player_verification(platform, user_id, server, player_id, status)
 
     @staticmethod
-    def set_car_forward(platform: str, user_id: str, status: str):
+    def set_car_forward(platform: str, user_id: str, status: bool):
         return set_car_forward(platform, user_id, status)
 
     @staticmethod
     def set_default_server(platform: str, user_id: str, text: str):
         return set_default_server(platform, user_id, text)
 
     @staticmethod
```

### Comparing `tsugu-0.4.9/tsugu/utils.py` & `tsugu-0.5.0/tsugu/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,32 +3,30 @@
 import json
 import sqlite3
 import os
 import sys
 import random
 import urllib3
 from urllib3.exceptions import HTTPError
+from loguru import logger
 
 from .config import config
 
 
-urllib3.disable_warnings()
-
-
 class DatabaseManager:
     def __init__(self, path):
         self.path = path
         self.conn = None
         self.cursor = None
         self.init_db(self.path)
 
     def init_db(self, path):
         if path:
             self.conn = sqlite3.connect(path, check_same_thread=False)
-            print('数据库连接成功，路径:', path)
+            logger.success(f'数据库连接成功，路径: {path}')
             self.cursor = self.conn.cursor()
             self.cursor.execute('''
                 CREATE TABLE IF NOT EXISTS users (
                     id INTEGER PRIMARY KEY AUTOINCREMENT,
                     user_id TEXT UNIQUE,
                     platform TEXT,
                     server_mode INTEGER,
@@ -38,15 +36,15 @@
                     verify_code TEXT
                 )
             ''')
             self.conn.commit()
         else:
             # 如果不使用数据库，设置连接为 None
             self.conn = None
-            # print('不使用数据库')
+            # logger.info('不使用数据库')
 
     def close_db(self):
         if self.conn:
             self.conn.close()
 
     def execute_query(self, query):
         if self.cursor:
@@ -90,72 +88,71 @@
     if server or server == 0:
         return True
     return False
 
 
 def requests_post_for_user(url, data):
     if config.user_data_backend_use_proxy:
-        http = urllib3.ProxyManager(config.proxy_url)
+        http = urllib3.ProxyManager(config.proxy_url, cert_reqs='CERT_NONE')
     else:
-        http = urllib3.PoolManager()
+        http = urllib3.PoolManager(cert_reqs='CERT_NONE')
     try:
         response = http.request('POST', url, headers={'Content-Type': 'application/json'}, body=json.dumps(data))
 
         # 检查响应的状态码是否为 200
         if response.status == 200:
             return json.loads(response.data.decode('utf-8'))
         else:
             # 处理其他状态码
             return text_response("服务器出现了问题，请稍后再试。")
 
     except HTTPError as http_err:
-        print(f'HTTP 错误：{http_err}')
+        logger.error(f'HTTP 错误：{http_err}')
         return text_response("服务器出现了问题，请稍后再试。")
 
     except Exception as e:
-        print(f'发生异常：{e}')
+        logger.error(f'发生异常：{e}')
         return text_response("发生了未知错误。")
 
 
 def requests_post_for_backend(url, data):
     if config.backend_use_proxy:
-        http = urllib3.ProxyManager(config.proxy_url)
+        http = urllib3.ProxyManager(config.proxy_url, cert_reqs='CERT_NONE')
     else:
-        http = urllib3.PoolManager()
+        http = urllib3.PoolManager(cert_reqs='CERT_NONE')
     try:
         response = http.request('POST', url, headers={'Content-Type': 'application/json'}, body=json.dumps(data))
 
         # 检查响应的状态码是否为 200
         if response.status == 200:
             return json.loads(response.data.decode('utf-8'))
         else:
             # 处理其他状态码
             return text_response("服务器出现了问题，请稍后再试。")
 
     except HTTPError as http_err:
-        print(f'HTTP 错误：{http_err}')
+        logger.error(f'HTTP 错误：{http_err}')
         return text_response("服务器出现了问题，请稍后再试。")
 
     except Exception as e:
-        print(f'发生异常：{e}')
+        logger.error(f'发生异常：{e}')
         return text_response("发生了未知错误。")
 
 
 def v2api_from_backend(api, text, default_servers: List[int] = None, server=3):
     if default_servers is None:
         default_servers = [3, 0]
     path = f"/v2/{api}"
     data = {
         "default_servers": default_servers,
         "server": server,
         "text": text,
         "useEasyBG": config.use_easy_bg,
         "compress": config.compress
     }
-    # print(data)
     res = requests_post_for_backend(f"{config.backend}{path}", data)
     return res
 
 
 def v2_api_command(message, command_matched, api, platform, user_id, channel_id):
     text = message[len(command_matched):].strip()
 
@@ -163,22 +160,23 @@
         return v2api_from_backend(api, text)
 
     if api == 'gachaSimulate':
         if channel_id in config.ban_gacha_simulate_group_data:
             return text_response('此群禁止使用模拟抽卡功能')
 
     # 获取用户数据
+    import logging
+    logging.debug(config.user_database_path)
     user_data = get_user_data(platform, user_id) if config.user_database_path else Remote.get_user_data(platform, user_id)
-    # print(user_data)
     try:
         if user_data['status'] != 'success':
-            return text_response('获取用户数据失败')
+            return text_response('获取用户数据失败：内部错误')
         return v2api_from_backend(api, text, user_data['data']['default_server'], user_data['data']['server_mode'])
     except Exception as e:
-        return text_response('前端错误: ' + str(e))
+        return text_response('获取用户数据失败：网络 / 前端错误')
 
 
 def submit_car_number_msg(message, user_id, platform=None):
     # 检查car_config['car']中的关键字
     for keyword in config.car_config["car"]:
         if str(keyword) in message:
             break
@@ -195,43 +193,43 @@
     # 获取用户数据
     try:
         if platform:
             user_data = get_user_data(platform, user_id) if config.user_database_path else Remote.get_user_data(platform, user_id)
             if not user_data['data']['car']:
                 return True
     except Exception as e:
-        print('unknown user')
+        logger.error('unknown user')
         # 默认不开启关闭车牌，继续提交
         pass
 
     try:
         car_id = message[:6]
         if not car_id.isdigit() and car_id[:5].isdigit():
             car_id = car_id[:5]
 
         # 构建 URL
         url = f"https://api.bandoristation.com/index.php?function=submit_room_number&number={car_id}&user_id={user_id}&raw_message={message}&source={config.token_name}&token={config.bandori_station_token}"
 
         if config.submit_car_number_use_proxy:
-            http = urllib3.ProxyManager(config.proxy_url)
+            http = urllib3.ProxyManager(config.proxy_url, cert_reqs='CERT_NONE')
         else:
-            http = urllib3.PoolManager()
+            http = urllib3.PoolManager(cert_reqs='CERT_NONE')
 
         # 发送请求
         response = http.request('GET', url)
 
         # 检查响应的状态码是否为 200
         if response.status == 200:
             return True
         else:
-            print(f"[Tsugu] 提交车牌失败，HTTP响应码: {response.status}")
+            logger.error(f"[Tsugu] 提交车牌失败，HTTP响应码: {response.status}")
             return True  # 虽然提交失败，但是确定了是车牌消息
 
     except Exception as e:
-        print(f"[Tsugu] 发生异常: {e}")
+        logger.error(f"[Tsugu] 发生异常: {e}")
         return True  # 虽然提交失败，但是确定了是车牌消息
 
 
 def match_command(message, cmd_dict):
     for command, api_value in cmd_dict.items():
         if message.startswith(command):
             return command, api_value
@@ -427,25 +425,25 @@
         if i.get("game_id") == player_id and i.get("server") == server:
             return text_response('请勿重复绑定')
     server_s_name = config.server_index_to_s_name[str(server)]
 
     # 构建 URL
     url = f'https://bestdori.com/api/player/{server_s_name}/{player_id}?mode=2'
     if config.verify_player_bind_use_proxy:
-        http = urllib3.ProxyManager(config.proxy_url)
+        http = urllib3.ProxyManager(config.proxy_url, cert_reqs='CERT_NONE')
     else:
-        http = urllib3.PoolManager()
+        http = urllib3.PoolManager(cert_reqs='CERT_NONE')
     # 发送请求
     response = http.request('GET', url)
     # 检查响应的状态码是否为 200
     if response.status == 200:
         # 解析 JSON 响应数据
         data = json.loads(response.data.decode('utf-8'))
     else:
-        print(f"获取玩家数据失败，HTTP响应码: {response.status}")
+        logger.error(f"获取玩家数据失败，HTTP响应码: {response.status}")
         return None
 
     if data.get("data").get("profile") is None or data.get("profile") == {}:
         return text_response('玩家ID不存在，请检查输入，或服务器是否对应')
     introduction = data.get("data", {}).get("profile", {}).get("introduction")
     deck_name = data.get("data", {}).get("profile", {}).get("mainUserDeck", {}).get("deckName")
     if verify_code != introduction and verify_code != deck_name:
```

### Comparing `tsugu-0.4.9/tsugu.egg-info/PKG-INFO` & `tsugu-0.5.0/tsugu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.4.9
+Version: 0.5.0
 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
         <h1 align="center"> Tsugu Python Frontend <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu Version: 0.4.9 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.5.0 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

