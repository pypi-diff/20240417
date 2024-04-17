# Comparing `tmp/tsugu-0.5.3.tar.gz` & `tmp/tsugu-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-0.5.3.tar", last modified: Wed Apr 17 07:35:05 2024, max compression
+gzip compressed data, was "tsugu-0.5.4.tar", last modified: Wed Apr 17 07:43:22 2024, max compression
```

## Comparing `tsugu-0.5.3.tar` & `tsugu-0.5.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:35:05.472995 tsugu-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-17 07:34:56.000000 tsugu-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-17 07:35:05.472995 tsugu-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-17 07:34:56.000000 tsugu-0.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 07:35:05.472995 tsugu-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-17 07:34:56.000000 tsugu-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:35:05.468995 tsugu-0.5.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-17 07:34:56.000000 tsugu-0.5.3/test/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:35:05.468995 tsugu-0.5.3/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-17 07:34:56.000000 tsugu-0.5.3/tsugu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21286 2024-04-17 07:34:56.000000 tsugu-0.5.3/tsugu/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12008 2024-04-17 07:34:56.000000 tsugu-0.5.3/tsugu/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-04-17 07:34:56.000000 tsugu-0.5.3/tsugu/router.py
--rw-r--r--   0 runner    (1001) docker     (127)    21585 2024-04-17 07:34:56.000000 tsugu-0.5.3/tsugu/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:35:05.468995 tsugu-0.5.3/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-17 07:35:05.000000 tsugu-0.5.3/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-17 07:35:05.000000 tsugu-0.5.3/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 07:35:05.000000 tsugu-0.5.3/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 07:35:05.000000 tsugu-0.5.3/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 07:35:05.000000 tsugu-0.5.3/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:43:22.974630 tsugu-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-17 07:43:12.000000 tsugu-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-17 07:43:22.974630 tsugu-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-17 07:43:12.000000 tsugu-0.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 07:43:22.974630 tsugu-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-17 07:43:12.000000 tsugu-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:43:22.974630 tsugu-0.5.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-17 07:43:12.000000 tsugu-0.5.4/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:43:22.974630 tsugu-0.5.4/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-17 07:43:12.000000 tsugu-0.5.4/tsugu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21286 2024-04-17 07:43:12.000000 tsugu-0.5.4/tsugu/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-04-17 07:43:12.000000 tsugu-0.5.4/tsugu/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-04-17 07:43:12.000000 tsugu-0.5.4/tsugu/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21682 2024-04-17 07:43:12.000000 tsugu-0.5.4/tsugu/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:43:22.974630 tsugu-0.5.4/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-17 07:43:22.000000 tsugu-0.5.4/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-17 07:43:22.000000 tsugu-0.5.4/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 07:43:22.000000 tsugu-0.5.4/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 07:43:22.000000 tsugu-0.5.4/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 07:43:22.000000 tsugu-0.5.4/tsugu.egg-info/top_level.txt
```

### Comparing `tsugu-0.5.3/LICENSE` & `tsugu-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-0.5.3/PKG-INFO` & `tsugu-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.5.3
+Version: 0.5.4
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
-Metadata-Version: 2.1 Name: tsugu Version: 0.5.3 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.5.4 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

### Comparing `tsugu-0.5.3/README.md` & `tsugu-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-0.5.3/setup.py` & `tsugu-0.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='0.5.3',
+    version='0.5.4',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py',
```

### Comparing `tsugu-0.5.3/test/test_main.py` & `tsugu-0.5.4/test/test_main.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.5.3/tsugu/config.py` & `tsugu-0.5.4/tsugu/config.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.5.3/tsugu/handler.py` & `tsugu-0.5.4/tsugu/handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,14 +154,15 @@
         if message.startswith('绑定玩家'):
             # 如果匹配 绑定玩家 则绑定默认服务器的玩家 如果用户输入了服务器名 则绑定对应服务器的玩家，如果服务器名无效则 赋值为 None
             server = Remote.get_user_data(platform, user_id)['data']['server_mode'] if message[4:].strip() == '' else (r_ if server_exists(r_ := query_server_info(message[4:])) else None)
             if not server_exists(server):
                 return text_response(f'未找到名为 {(message[4:]).strip()} 的服务器信息，请确保输入的是服务器名而不是玩家ID，通常情况发送"绑定玩家"即可')
 
             res = Remote.bind_player_request(platform, user_id, server, True)
+
             if res.get('status') != 'success':
                 # {'status': 'success', 'data': {'verifyCode': 12492}}
                 return text_response(res.get('data'))
             # if not res.get('status') == 'failed':
             #     return text_response('未知错误喵')
             return text_response(f'''正在绑定账号，请将 评论(个性签名) 或者 当前使用的 乐队编队名称改为\n{res.get('data')['verifyCode']}\n稍等片刻等待同步后，发送\n验证 + 空格 + 玩家ID 来完成本次身份验证\n验证 10000xxxx 国服''')
```

### Comparing `tsugu-0.5.3/tsugu/router.py` & `tsugu-0.5.4/tsugu/router.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.5.3/tsugu/utils.py` & `tsugu-0.5.4/tsugu/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,18 +93,19 @@
 def requests_post_for_user(url, data):
     if config.user_data_backend_use_proxy:
         http = urllib3.ProxyManager(config.proxy_url, cert_reqs='CERT_NONE')
     else:
         http = urllib3.PoolManager(cert_reqs='CERT_NONE')
     try:
         response = http.request('POST', url, headers={'Content-Type': 'application/json'}, body=json.dumps(data))
-
         # 检查响应的状态码是否为 200
         if response.status == 200:
             return json.loads(response.data.decode('utf-8'))
+        elif response.status == 400:
+            return json.loads(response.data.decode('utf-8'))
         else:
             # 处理其他状态码
             return {"status": "error", "message": "服务器出现了问题，请稍后再试。"}
 
     except HTTPError as http_err:
         logger.error(f'HTTP 错误：{http_err}')
         return {"status": "error", "message": "服务器出现了问题，请稍后再试。"}
```

### Comparing `tsugu-0.5.3/tsugu.egg-info/PKG-INFO` & `tsugu-0.5.4/tsugu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.5.3
+Version: 0.5.4
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
-Metadata-Version: 2.1 Name: tsugu Version: 0.5.3 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.5.4 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

