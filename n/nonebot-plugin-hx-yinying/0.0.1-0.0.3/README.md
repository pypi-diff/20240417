# Comparing `tmp/nonebot-plugin-hx-yinying-0.0.1.tar.gz` & `tmp/nonebot-plugin-hx-yinying-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-hx-yinying-0.0.1.tar", last modified: Wed Apr 17 07:19:12 2024, max compression
+gzip compressed data, was "nonebot-plugin-hx-yinying-0.0.3.tar", last modified: Wed Apr 17 13:19:02 2024, max compression
```

## Comparing `nonebot-plugin-hx-yinying-0.0.1.tar` & `nonebot-plugin-hx-yinying-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 07:19:12.296160 nonebot-plugin-hx-yinying-0.0.1/
--rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2679 2024-04-17 07:19:12.301491 nonebot-plugin-hx-yinying-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2239 2024-04-17 00:42:32.000000 nonebot-plugin-hx-yinying-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 07:19:12.176689 nonebot-plugin-hx-yinying-0.0.1/nonebot_plugin_hx_yinying/
--rw-rw-rw-   0        0        0     1330 2024-04-17 07:14:59.000000 nonebot-plugin-hx-yinying-0.0.1/nonebot_plugin_hx_yinying/__init__.py
--rw-rw-rw-   0        0        0     7562 2024-04-17 07:11:52.000000 nonebot-plugin-hx-yinying-0.0.1/nonebot_plugin_hx_yinying/chat.py
--rw-rw-rw-   0        0        0      544 2024-04-17 06:08:40.000000 nonebot-plugin-hx-yinying-0.0.1/nonebot_plugin_hx_yinying/config.py
-drwxrwxrwx   0        0        0        0 2024-04-17 07:19:12.281165 nonebot-plugin-hx-yinying-0.0.1/nonebot_plugin_hx_yinying.egg-info/
--rw-rw-rw-   0        0        0     2679 2024-04-17 07:19:11.000000 nonebot-plugin-hx-yinying-0.0.1/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2024-04-17 07:19:11.000000 nonebot-plugin-hx-yinying-0.0.1/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 07:19:11.000000 nonebot-plugin-hx-yinying-0.0.1/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      124 2024-04-17 07:19:11.000000 nonebot-plugin-hx-yinying-0.0.1/nonebot_plugin_hx_yinying.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-17 07:19:11.000000 nonebot-plugin-hx-yinying-0.0.1/nonebot_plugin_hx_yinying.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-04-17 07:19:12.405710 nonebot-plugin-hx-yinying-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      840 2024-04-17 07:18:35.000000 nonebot-plugin-hx-yinying-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 13:19:02.463190 nonebot-plugin-hx-yinying-0.0.3/
+-rw-rw-rw-   0        0        0     1098 2024-04-16 15:27:11.000000 nonebot-plugin-hx-yinying-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3179 2024-04-17 13:19:02.480025 nonebot-plugin-hx-yinying-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2731 2024-04-17 08:20:26.000000 nonebot-plugin-hx-yinying-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 13:19:02.396695 nonebot-plugin-hx-yinying-0.0.3/nonebot_plugin_hx_yinying/
+-rw-rw-rw-   0        0        0     1330 2024-04-17 07:14:59.000000 nonebot-plugin-hx-yinying-0.0.3/nonebot_plugin_hx_yinying/__init__.py
+-rw-rw-rw-   0        0        0     7601 2024-04-17 13:15:48.000000 nonebot-plugin-hx-yinying-0.0.3/nonebot_plugin_hx_yinying/chat.py
+-rw-rw-rw-   0        0        0      544 2024-04-17 06:08:40.000000 nonebot-plugin-hx-yinying-0.0.3/nonebot_plugin_hx_yinying/config.py
+drwxrwxrwx   0        0        0        0 2024-04-17 13:19:02.463190 nonebot-plugin-hx-yinying-0.0.3/nonebot_plugin_hx_yinying.egg-info/
+-rw-rw-rw-   0        0        0     3179 2024-04-17 13:19:01.000000 nonebot-plugin-hx-yinying-0.0.3/nonebot_plugin_hx_yinying.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2024-04-17 13:19:02.000000 nonebot-plugin-hx-yinying-0.0.3/nonebot_plugin_hx_yinying.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 13:19:01.000000 nonebot-plugin-hx-yinying-0.0.3/nonebot_plugin_hx_yinying.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      124 2024-04-17 13:19:01.000000 nonebot-plugin-hx-yinying-0.0.3/nonebot_plugin_hx_yinying.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-17 13:19:01.000000 nonebot-plugin-hx-yinying-0.0.3/nonebot_plugin_hx_yinying.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-04-17 13:19:02.480025 nonebot-plugin-hx-yinying-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      840 2024-04-17 13:18:43.000000 nonebot-plugin-hx-yinying-0.0.3/setup.py
```

### Comparing `nonebot-plugin-hx-yinying-0.0.1/LICENSE` & `nonebot-plugin-hx-yinying-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-0.0.1/PKG-INFO` & `nonebot-plugin-hx-yinying-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 0.0.1
+Version: 0.0.3
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!--
+<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
+[![All Contributors](https://img.shields.io/badge/all_contributors-0-orange.svg?style=flat-square)](#contributors-)
+<!-- ALL-CONTRIBUTORS-BADGE:END -->
  * @Author         : huanxin
  * @Date           : 2024-4-17 00:04:25
- * @LastEditors    : yanyongyu
+ * @LastEditors    : huanxin
  * @LastEditTime   : 2024-4-17 00:04:25
  * @Description    : None
  * @GitHub         : https://github.com/huanxin
 -->
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
@@ -103,7 +106,20 @@
 ```dotenv
 hx_api_yinying=https://地址
 yinying_model=模型
 yinying_token=你的token(不带bearer)
 hx_reply_at=False
 yinying_limit=12
 ```
+
+
+## Contributors ✨
+
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+
```

#### html2text {}

```diff
@@ -1,13 +1,17 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 0.0.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 0.0.3 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
-Type: text/markdown License-File: LICENSE
+Type: text/markdown License-File: LICENSE [![All Contributors](https://
+img.shields.io/badge/all_contributors-0-orange.svg?style=flat-square)]
+(#contributors-) * @Author : huanxin * @Date : 2024-4-17 00:04:25 *
+@LastEditors : huanxin * @LastEditTime : 2024-4-17 00:04:25 * @Description :
+None * @GitHub : https://github.com/huanxin -->
                                    _[_n_o_n_e_b_o_t_]
                 # nonebot_plugin_hx-yinying _â¨ Hx vs YinYing
                   (å¨çº¿ä¸é¶å½±è¿è¡å¯¹è¯çæä»¶) â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## ä½¿ç¨æ¹å¼ éç¨: - @Bot æèåå¤å³å¯ OneBot: - @Bot - åå¤Bot ##
 éç½®é¡¹ > [!WARNING] > GitHub ä»åºä¸­çææ¡£ä¸ºææ° DEV
 çæ¬ï¼éç½®æ¹å¼è¯·åè [PyPI](https://pypi.org/project/nonebot-plugin-
@@ -20,8 +24,8 @@
 ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼é¶å½±å¯¹è¯çç¨æ·æ°æ®å­å¨è·¯å¾(ä¸åå°ä½¿ç¨é»è®¤éç½®)
 ## hx_reply_at - ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
 è¯´æï¼botåå¤æ¶æ¯æ¯å¦è¾ç¹ ## yinying_limit - ç±»åï¼`int` -
 é»è®¤å¼ï¼`12` - è¯´æï¼å¯¹äºé¶å½±å¯¹è¯éå¶çæ¬¡æ°
 éç½®æä»¶ç¤ºä¾ï¼é»è®¤æ¨¡æ¿ï¼ ```dotenv hx_api_yinying=https://å°å
 yinying_model=æ¨¡å yinying_token=ä½ çtoken(ä¸å¸¦bearer) hx_reply_at=False
-yinying_limit=12 ```
+yinying_limit=12 ``` ## Contributors â¨
```

### Comparing `nonebot-plugin-hx-yinying-0.0.1/nonebot_plugin_hx_yinying/__init__.py` & `nonebot-plugin-hx-yinying-0.0.3/nonebot_plugin_hx_yinying/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-0.0.1/nonebot_plugin_hx_yinying/chat.py` & `nonebot-plugin-hx-yinying-0.0.3/nonebot_plugin_hx_yinying/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
                 with open(f'{log_dir}/{id}/times.json','r',encoding='utf-8') as file:
                     data = json.load(file)
                     data["times"] = data["times"] + 1
                     data.update(file)
                 with open(f'{log_dir}/{id}/times.json','w',encoding='utf-8') as file:
                     json.dump(data, file)
     else:
+        create_dir_usr(f"{log_dir}\{id}")
         with open(f'{log_dir}/{id}/times.json','w',encoding='utf-8') as file:
                 with open(f'{log_dir}/{id}/times.json','w',encoding='utf-8') as file:
                     old_data = {}
                     dt = time.time()
                     t = int(dt)
                     data = {"times":0,"time":t,"character":"是一只猫猫龙哦"}
                     old_data.update(data)
@@ -192,9 +193,7 @@
     try:
         back_msg = str(await yinying(text,id,nick))
         msg = back_msg.replace("\n","\\n")
         await send_with_at(matcher,msg)
     except httpx.HTTPError as e:
         back_msg = f"请求接口报错！\t返回结果：{e}"
         await finish_with_at(matcher, back_msg)
-
-
```

### Comparing `nonebot-plugin-hx-yinying-0.0.1/nonebot_plugin_hx_yinying/config.py` & `nonebot-plugin-hx-yinying-0.0.3/nonebot_plugin_hx_yinying/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-hx-yinying-0.0.1/nonebot_plugin_hx_yinying.egg-info/PKG-INFO` & `nonebot-plugin-hx-yinying-0.0.3/nonebot_plugin_hx_yinying.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-hx-yinying
-Version: 0.0.1
+Version: 0.0.3
 Summary: chat with yinying
 Home-page: https://github.com/huanxin996/nonebot_plugin_hx-yinying
 Author: Huan Xin
 Author-email: mc.xiaolang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <!--
+<!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
+[![All Contributors](https://img.shields.io/badge/all_contributors-0-orange.svg?style=flat-square)](#contributors-)
+<!-- ALL-CONTRIBUTORS-BADGE:END -->
  * @Author         : huanxin
  * @Date           : 2024-4-17 00:04:25
- * @LastEditors    : yanyongyu
+ * @LastEditors    : huanxin
  * @LastEditTime   : 2024-4-17 00:04:25
  * @Description    : None
  * @GitHub         : https://github.com/huanxin
 -->
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
@@ -103,7 +106,20 @@
 ```dotenv
 hx_api_yinying=https://地址
 yinying_model=模型
 yinying_token=你的token(不带bearer)
 hx_reply_at=False
 yinying_limit=12
 ```
+
+
+## Contributors ✨
+
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+
```

#### html2text {}

```diff
@@ -1,13 +1,17 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 0.0.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-hx-yinying Version: 0.0.3 Summary:
 chat with yinying Home-page: https://github.com/huanxin996/nonebot_plugin_hx-
 yinying Author: Huan Xin Author-email: mc.xiaolang@foxmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
-Type: text/markdown License-File: LICENSE
+Type: text/markdown License-File: LICENSE [![All Contributors](https://
+img.shields.io/badge/all_contributors-0-orange.svg?style=flat-square)]
+(#contributors-) * @Author : huanxin * @Date : 2024-4-17 00:04:25 *
+@LastEditors : huanxin * @LastEditTime : 2024-4-17 00:04:25 * @Description :
+None * @GitHub : https://github.com/huanxin -->
                                    _[_n_o_n_e_b_o_t_]
                 # nonebot_plugin_hx-yinying _â¨ Hx vs YinYing
                   (å¨çº¿ä¸é¶å½±è¿è¡å¯¹è¯çæä»¶) â¨_
                             _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
 ## ä½¿ç¨æ¹å¼ éç¨: - @Bot æèåå¤å³å¯ OneBot: - @Bot - åå¤Bot ##
 éç½®é¡¹ > [!WARNING] > GitHub ä»åºä¸­çææ¡£ä¸ºææ° DEV
 çæ¬ï¼éç½®æ¹å¼è¯·åè [PyPI](https://pypi.org/project/nonebot-plugin-
@@ -20,8 +24,8 @@
 ç±»åï¼`str` - é»è®¤å¼ï¼`None` -
 è¯´æï¼é¶å½±å¯¹è¯çç¨æ·æ°æ®å­å¨è·¯å¾(ä¸åå°ä½¿ç¨é»è®¤éç½®)
 ## hx_reply_at - ç±»åï¼`bool` - é»è®¤å¼ï¼`False` -
 è¯´æï¼botåå¤æ¶æ¯æ¯å¦è¾ç¹ ## yinying_limit - ç±»åï¼`int` -
 é»è®¤å¼ï¼`12` - è¯´æï¼å¯¹äºé¶å½±å¯¹è¯éå¶çæ¬¡æ°
 éç½®æä»¶ç¤ºä¾ï¼é»è®¤æ¨¡æ¿ï¼ ```dotenv hx_api_yinying=https://å°å
 yinying_model=æ¨¡å yinying_token=ä½ çtoken(ä¸å¸¦bearer) hx_reply_at=False
-yinying_limit=12 ```
+yinying_limit=12 ``` ## Contributors â¨
```

### Comparing `nonebot-plugin-hx-yinying-0.0.1/setup.py` & `nonebot-plugin-hx-yinying-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot-plugin-hx-yinying",
-    version="0.0.1",
+    version="0.0.3",
     author="Huan Xin",
     author_email="mc.xiaolang@foxmail.com",
     description="chat with yinying",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/huanxin996/nonebot_plugin_hx-yinying",
     packages=setuptools.find_packages(),
```

