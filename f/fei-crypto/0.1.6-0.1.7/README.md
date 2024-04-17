# Comparing `tmp/fei_crypto-0.1.6.tar.gz` & `tmp/fei_crypto-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fei_crypto-0.1.6.tar", max compression
+gzip compressed data, was "fei_crypto-0.1.7.tar", max compression
```

## Comparing `fei_crypto-0.1.6.tar` & `fei_crypto-0.1.7.tar`

### file list

```diff
@@ -1,51 +1,83 @@
--rw-r--r--   0        0        0      140 2023-12-20 05:11:49.661668 fei_crypto-0.1.6/fei_crypto/__init__.py
--rw-r--r--   0        0        0      887 2024-03-21 05:14:18.936639 fei_crypto-0.1.6/fei_crypto/captcha.py
--rw-r--r--   0        0        0      488 2023-11-29 13:54:30.172545 fei_crypto-0.1.6/fei_crypto/crypto.py
--rw-r--r--   0        0        0     1218 2024-03-29 08:54:22.246792 fei_crypto-0.1.6/fei_crypto/discordwebhook.py
--rw-r--r--   0        0        0       79 2024-03-21 04:40:21.216364 fei_crypto-0.1.6/fei_crypto/env.py
--rw-r--r--   0        0        0      137 2023-09-26 15:21:11.446999 fei_crypto-0.1.6/fei_crypto/md5.py
--rw-r--r--   0        0        0      319 2023-09-26 14:30:44.514337 fei_crypto-0.1.6/fei_crypto/os.py
--rw-r--r--   0        0        0     1338 2023-11-29 17:18:37.219370 fei_crypto-0.1.6/fei_crypto/rmw.py
--rw-r--r--   0        0        0     1138 2023-09-28 06:14:48.561059 fei_crypto-0.1.6/fei_crypto/rnd_emoj.py
--rw-r--r--   0        0        0     2166 2024-03-29 02:58:44.194898 fei_crypto-0.1.6/fei_crypto/t2m.py
--rw-r--r--   0        0        0      369 2023-09-26 14:38:05.472651 fei_crypto-0.1.6/fei_crypto/time.py
--rw-r--r--   0        0        0     1067 2023-09-18 06:59:02.002584 fei_crypto-0.1.6/LICENSE
--rw-r--r--   0        0        0       58 2023-09-26 14:44:19.909970 fei_crypto-0.1.6/main/__init__.py
--rw-r--r--   0        0        0      120 2023-12-20 05:11:23.650909 fei_crypto-0.1.6/main/btc_eth.py
--rw-r--r--   0        0        0      137 2024-03-29 08:38:57.954290 fei_crypto-0.1.6/main/captcha.py
--rw-r--r--   0        0        0      138 2024-03-29 08:38:24.168499 fei_crypto-0.1.6/main/dc_webhook_send.py
--rw-r--r--   0        0        0      124 2023-12-20 05:11:23.620986 fei_crypto-0.1.6/main/emoj.py
--rw-r--r--   0        0        0      266 2023-12-20 05:11:23.679147 fei_crypto-0.1.6/main/env.py
--rw-r--r--   0        0        0      159 2023-12-20 05:11:54.326071 fei_crypto-0.1.6/main/main.py
--rw-r--r--   0        0        0       98 2023-12-20 05:11:23.591706 fei_crypto-0.1.6/main/os.py
--rw-r--r--   0        0        0      125 2023-12-20 05:11:23.709307 fei_crypto-0.1.6/main/rmw.py
--rw-r--r--   0        0        0       60 2023-09-26 16:09:10.583645 fei_crypto-0.1.6/main/say.py
--rw-r--r--   0        0        0      125 2024-03-28 19:31:13.343469 fei_crypto-0.1.6/main/t2m.py
--rw-r--r--   0        0        0       81 2024-04-02 12:09:40.362527 fei_crypto-0.1.6/main/tg_forward.py
--rw-r--r--   0        0        0       75 2024-04-02 12:07:53.673901 fei_crypto-0.1.6/main/tg_login.py
--rw-r--r--   0        0        0      348 2023-12-20 05:11:23.737349 fei_crypto-0.1.6/main/ts.py
--rw-r--r--   0        0        0       97 2023-09-26 16:09:52.597612 fei_crypto-0.1.6/main/uu_id.py
--rw-r--r--   0        0        0     1453 2024-04-04 11:07:03.897698 fei_crypto-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3597 2024-04-04 09:38:32.012308 fei_crypto-0.1.6/README.md
--rw-r--r--   0        0        0       56 2024-04-02 12:07:46.806912 fei_crypto-0.1.6/tg/__init__.py
--rw-r--r--   0        0        0       33 2024-04-02 20:14:26.971417 fei_crypto-0.1.6/tg/bot/__init__.py
--rw-r--r--   0        0        0     4024 2024-04-03 08:01:55.185079 fei_crypto-0.1.6/tg/bot/live_bot.py
--rw-r--r--   0        0        0     1908 2024-04-02 17:24:42.314843 fei_crypto-0.1.6/tg/bot/utils.py
--rw-r--r--   0        0        0     3966 2024-04-03 08:28:04.109210 fei_crypto-0.1.6/tg/cli_forward.py
--rw-r--r--   0        0        0     1665 2024-04-03 03:07:19.467042 fei_crypto-0.1.6/tg/cli_login.py
--rw-r--r--   0        0        0     6472 2024-04-03 08:27:32.982473 fei_crypto-0.1.6/tg/config.py
--rw-r--r--   0        0        0      338 2024-04-03 08:04:18.836132 fei_crypto-0.1.6/tg/const.py
--rw-r--r--   0        0        0     3903 2024-04-03 08:01:55.176079 fei_crypto-0.1.6/tg/live.py
--rw-r--r--   0        0        0     2974 2024-04-03 03:07:42.633426 fei_crypto-0.1.6/tg/login.py
--rw-r--r--   0        0        0     2407 2024-04-03 09:46:41.767357 fei_crypto-0.1.6/tg/message.py
--rw-r--r--   0        0        0      356 2024-04-02 17:19:01.228599 fei_crypto-0.1.6/tg/parse.py
--rw-r--r--   0        0        0     3031 2024-04-03 08:31:15.484901 fei_crypto-0.1.6/tg/past.py
--rw-r--r--   0        0        0     1504 2024-04-03 03:07:53.634670 fei_crypto-0.1.6/tg/plugin_models.py
--rw-r--r--   0        0        0     2533 2024-04-03 08:01:56.261327 fei_crypto-0.1.6/tg/plugins/__init__.py
--rw-r--r--   0        0        0      438 2024-04-03 03:06:07.826906 fei_crypto-0.1.6/tg/plugins/caption.py
--rw-r--r--   0        0        0     2401 2024-04-03 07:12:39.950474 fei_crypto-0.1.6/tg/plugins/filter.py
--rw-r--r--   0        0        0      608 2024-04-03 03:06:20.136916 fei_crypto-0.1.6/tg/plugins/fmt.py
--rw-r--r--   0        0        0      573 2024-04-03 03:05:11.028077 fei_crypto-0.1.6/tg/plugins/replace.py
--rw-r--r--   0        0        0      905 2024-04-02 12:49:19.540873 fei_crypto-0.1.6/tg/storage.py
--rw-r--r--   0        0        0     1779 2024-04-02 18:16:11.762778 fei_crypto-0.1.6/tg/utils.py
--rw-r--r--   0        0        0     4586 1970-01-01 00:00:00.000000 fei_crypto-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       78 2024-04-16 13:51:49.192517 fei_crypto-0.1.7/fei_crypto/__init__.py
+-rw-r--r--   0        0        0      876 2024-04-16 13:53:17.866879 fei_crypto-0.1.7/fei_crypto/captcha.py
+-rw-r--r--   0        0        0      488 2023-11-29 13:54:30.172545 fei_crypto-0.1.7/fei_crypto/crypto.py
+-rw-r--r--   0        0        0     1218 2024-03-29 08:54:22.246792 fei_crypto-0.1.7/fei_crypto/discordwebhook.py
+-rw-r--r--   0        0        0       79 2024-03-21 04:40:21.216364 fei_crypto-0.1.7/fei_crypto/env.py
+-rw-r--r--   0        0        0      137 2023-09-26 15:21:11.446999 fei_crypto-0.1.7/fei_crypto/md5.py
+-rw-r--r--   0        0        0      319 2023-09-26 14:30:44.514337 fei_crypto-0.1.7/fei_crypto/os.py
+-rw-r--r--   0        0        0     1338 2023-11-29 17:18:37.219370 fei_crypto-0.1.7/fei_crypto/rmw.py
+-rw-r--r--   0        0        0     1138 2023-09-28 06:14:48.561059 fei_crypto-0.1.7/fei_crypto/rnd_emoj.py
+-rw-r--r--   0        0        0     2166 2024-03-29 02:58:44.194898 fei_crypto-0.1.7/fei_crypto/t2m.py
+-rw-r--r--   0        0        0      369 2023-09-26 14:38:05.472651 fei_crypto-0.1.7/fei_crypto/time.py
+-rw-r--r--   0        0        0     1067 2023-09-18 06:59:02.002584 fei_crypto-0.1.7/LICENSE
+-rw-r--r--   0        0        0       58 2023-09-26 14:44:19.909970 fei_crypto-0.1.7/main/__init__.py
+-rw-r--r--   0        0        0      120 2023-12-20 05:11:23.650909 fei_crypto-0.1.7/main/btc_eth.py
+-rw-r--r--   0        0        0      137 2024-03-29 08:38:57.954290 fei_crypto-0.1.7/main/captcha.py
+-rw-r--r--   0        0        0      138 2024-03-29 08:38:24.168499 fei_crypto-0.1.7/main/dc_webhook_send.py
+-rw-r--r--   0        0        0      124 2023-12-20 05:11:23.620986 fei_crypto-0.1.7/main/emoj.py
+-rw-r--r--   0        0        0      266 2023-12-20 05:11:23.679147 fei_crypto-0.1.7/main/env.py
+-rw-r--r--   0        0        0      159 2023-12-20 05:11:54.326071 fei_crypto-0.1.7/main/main.py
+-rw-r--r--   0        0        0       98 2023-12-20 05:11:23.591706 fei_crypto-0.1.7/main/os.py
+-rw-r--r--   0        0        0      125 2023-12-20 05:11:23.709307 fei_crypto-0.1.7/main/rmw.py
+-rw-r--r--   0        0        0       60 2023-09-26 16:09:10.583645 fei_crypto-0.1.7/main/say.py
+-rw-r--r--   0        0        0      125 2024-03-28 19:31:13.343469 fei_crypto-0.1.7/main/t2m.py
+-rw-r--r--   0        0        0       81 2024-04-02 12:09:40.362527 fei_crypto-0.1.7/main/tg_forward.py
+-rw-r--r--   0        0        0      156 2024-04-17 12:01:33.870269 fei_crypto-0.1.7/main/tg_koltime_menu.py
+-rw-r--r--   0        0        0       75 2024-04-02 12:07:53.673901 fei_crypto-0.1.7/main/tg_login.py
+-rw-r--r--   0        0        0      348 2023-12-20 05:11:23.737349 fei_crypto-0.1.7/main/ts.py
+-rw-r--r--   0        0        0       97 2023-09-26 16:09:52.597612 fei_crypto-0.1.7/main/uu_id.py
+-rw-r--r--   0        0        0     1614 2024-04-17 12:06:50.897188 fei_crypto-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3631 2024-04-16 05:01:03.117989 fei_crypto-0.1.7/README.md
+-rw-r--r--   0        0        0      389 2024-04-16 14:59:52.401824 fei_crypto-0.1.7/tests/__init__.py
+-rw-r--r--   0        0        0      196 2024-04-03 09:48:00.078906 fei_crypto-0.1.7/tests/calc.py
+-rw-r--r--   0        0        0      356 2024-04-02 16:40:47.033897 fei_crypto-0.1.7/tests/console.py
+-rw-r--r--   0        0        0      183 2024-04-03 03:01:53.459809 fei_crypto-0.1.7/tests/dict.py
+-rw-r--r--   0        0        0      463 2024-04-16 14:07:08.378494 fei_crypto-0.1.7/tests/enum_test.py
+-rw-r--r--   0        0        0       88 2024-04-17 10:03:49.057111 fei_crypto-0.1.7/tests/env_test.py
+-rw-r--r--   0        0        0      206 2024-04-02 15:53:35.170989 fei_crypto-0.1.7/tests/getattr.py
+-rw-r--r--   0        0        0       53 2024-03-21 03:22:41.838133 fei_crypto-0.1.7/tests/hello.py
+-rw-r--r--   0        0        0     1155 2024-03-21 04:51:46.085571 fei_crypto-0.1.7/tests/image_base64.py
+-rw-r--r--   0        0        0      349 2024-04-15 08:49:16.084219 fei_crypto-0.1.7/tests/logging_test.py
+-rw-r--r--   0        0        0     1665 2024-03-28 19:19:29.326677 fei_crypto-0.1.7/tests/manim.py
+-rw-r--r--   0        0        0      186 2024-04-03 08:27:11.338227 fei_crypto-0.1.7/tests/open.py
+-rw-r--r--   0        0        0      545 2024-03-29 07:27:10.711077 fei_crypto-0.1.7/tests/path.py
+-rw-r--r--   0        0        0     1312 2024-04-17 11:34:47.610297 fei_crypto-0.1.7/tests/redis_hash.py
+-rw-r--r--   0        0        0     2611 2024-04-17 11:57:24.452664 fei_crypto-0.1.7/tests/redis_koltime_channels.py
+-rw-r--r--   0        0        0     1036 2024-04-17 09:58:52.863717 fei_crypto-0.1.7/tests/redis_set_test.py
+-rw-r--r--   0        0        0      158 2024-04-17 10:41:30.695499 fei_crypto-0.1.7/tests/scope_test.py
+-rw-r--r--   0        0        0      495 2024-04-16 20:41:31.838245 fei_crypto-0.1.7/tests/str_test.py
+-rw-r--r--   0        0        0     4083 2024-04-16 15:12:18.915950 fei_crypto-0.1.7/tests/tg_arbitrarycallbackdatabot.py
+-rw-r--r--   0        0        0     3228 2024-04-16 14:04:46.204833 fei_crypto-0.1.7/tests/tg_inlinebot.py
+-rw-r--r--   0        0        0     2468 2024-04-16 14:04:52.248862 fei_crypto-0.1.7/tests/tg_inlinekeyboard.py
+-rw-r--r--   0        0        0     6858 2024-04-16 14:05:05.464671 fei_crypto-0.1.7/tests/tg_inlinekeyboard2.py
+-rw-r--r--   0        0        0    13620 2024-04-16 14:05:18.553946 fei_crypto-0.1.7/tests/tg_nestedconversationbot.py
+-rw-r--r--   0        0        0     6587 2024-04-16 13:40:50.781376 fei_crypto-0.1.7/tests/tg_pollbot.py
+-rw-r--r--   0        0        0     2382 2024-04-16 13:40:28.566730 fei_crypto-0.1.7/tests/tg_rawapibot.py
+-rw-r--r--   0        0        0     2707 2024-04-16 14:06:07.187762 fei_crypto-0.1.7/tests/tg_webappbot.py
+-rw-r--r--   0        0        0      140 2024-04-03 05:46:33.338377 fei_crypto-0.1.7/tests/time.py
+-rw-r--r--   0        0        0      924 2024-04-03 02:55:54.333858 fei_crypto-0.1.7/tests/tuple.py
+-rw-r--r--   0        0        0      143 2024-04-17 06:38:57.801384 fei_crypto-0.1.7/tests/tuple_list.py
+-rw-r--r--   0        0        0      455 2023-11-29 13:21:57.903302 fei_crypto-0.1.7/tests/typer.py
+-rw-r--r--   0        0        0       56 2024-04-02 12:07:46.806912 fei_crypto-0.1.7/tg/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-02 20:14:26.971417 fei_crypto-0.1.7/tg/bot/__init__.py
+-rw-r--r--   0        0        0     4040 2024-04-16 05:45:45.842618 fei_crypto-0.1.7/tg/bot/live_bot.py
+-rw-r--r--   0        0        0     1757 2024-04-16 05:44:27.008518 fei_crypto-0.1.7/tg/bot/utils.py
+-rw-r--r--   0        0        0     3966 2024-04-16 03:35:51.804389 fei_crypto-0.1.7/tg/cli_forward.py
+-rw-r--r--   0        0        0     1665 2024-04-03 03:07:19.467042 fei_crypto-0.1.7/tg/cli_login.py
+-rw-r--r--   0        0        0     6472 2024-04-15 12:37:24.327913 fei_crypto-0.1.7/tg/config.py
+-rw-r--r--   0        0        0      338 2024-04-03 08:04:18.836132 fei_crypto-0.1.7/tg/const.py
+-rw-r--r--   0        0        0     4833 2024-04-17 12:00:28.700820 fei_crypto-0.1.7/tg/koltime_menu_bot.py
+-rw-r--r--   0        0        0     3903 2024-04-15 12:46:20.229789 fei_crypto-0.1.7/tg/live.py
+-rw-r--r--   0        0        0     2974 2024-04-03 03:07:42.633426 fei_crypto-0.1.7/tg/login.py
+-rw-r--r--   0        0        0     2407 2024-04-03 09:46:41.767357 fei_crypto-0.1.7/tg/message.py
+-rw-r--r--   0        0        0      356 2024-04-02 17:19:01.228599 fei_crypto-0.1.7/tg/parse.py
+-rw-r--r--   0        0        0     3031 2024-04-03 08:31:15.484901 fei_crypto-0.1.7/tg/past.py
+-rw-r--r--   0        0        0     1504 2024-04-03 03:07:53.634670 fei_crypto-0.1.7/tg/plugin_models.py
+-rw-r--r--   0        0        0     2533 2024-04-03 08:01:56.261327 fei_crypto-0.1.7/tg/plugins/__init__.py
+-rw-r--r--   0        0        0      438 2024-04-03 03:06:07.826906 fei_crypto-0.1.7/tg/plugins/caption.py
+-rw-r--r--   0        0        0     2401 2024-04-03 07:12:39.950474 fei_crypto-0.1.7/tg/plugins/filter.py
+-rw-r--r--   0        0        0      608 2024-04-03 03:06:20.136916 fei_crypto-0.1.7/tg/plugins/fmt.py
+-rw-r--r--   0        0        0      573 2024-04-03 03:05:11.028077 fei_crypto-0.1.7/tg/plugins/replace.py
+-rw-r--r--   0        0        0      905 2024-04-02 12:49:19.540873 fei_crypto-0.1.7/tg/storage.py
+-rw-r--r--   0        0        0     1954 2024-04-16 05:44:49.091593 fei_crypto-0.1.7/tg/utils.py
+-rw-r--r--   0        0        0     4729 1970-01-01 00:00:00.000000 fei_crypto-0.1.7/PKG-INFO
```

### Comparing `fei_crypto-0.1.6/fei_crypto/captcha.py` & `fei_crypto-0.1.7/fei_crypto/captcha.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import base64
-import os
 
 import typer
 import requests
 
 
 def captcha(file_abs_path: str, aliyun_ocr_appcode: str, pri_id='dn') -> str:
     with open(file_abs_path, 'rb') as f:
```

### Comparing `fei_crypto-0.1.6/fei_crypto/discordwebhook.py` & `fei_crypto-0.1.7/fei_crypto/discordwebhook.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.6/fei_crypto/rmw.py` & `fei_crypto-0.1.7/fei_crypto/rmw.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.6/fei_crypto/rnd_emoj.py` & `fei_crypto-0.1.7/fei_crypto/rnd_emoj.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.6/fei_crypto/t2m.py` & `fei_crypto-0.1.7/fei_crypto/t2m.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.6/LICENSE` & `fei_crypto-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.6/pyproject.toml` & `fei_crypto-0.1.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,60 +3,64 @@
 description = "fei crypto command utils"
 license = "MIT"
 name = "fei-crypto"
 packages = [
     { include = "fei_crypto" },
     { include = "tg" },
     { include = "main" },
+    { include = "tests" },
 ]
 readme = "README.md"
-version = "0.1.6"
+version = "0.1.7"
 
 [tool.poetry.dependencies]
 cowsay = "^6.1"
 filestools = "^0.2.1"
 pillow = "^9.5.0"
 python = "<3.12,>=3.10"
-#python = "~3.11"
+discord-webhook = "^1.3.1"
+ipython = "^8.23.0"
+manim = "^0.18.0"
+pymongo = "^4.6.3"
 python-dotenv = "^1.0.0"
 python-socks = { extras = ["asyncio"], version = "^2.4.3" }
+pyyaml = "^6.0.1"
 requests = { extras = ["socks"], version = "^2.31.0" }
+rich = "^13.7.1"
 telethon = "^1.34.0"
 typer = { extras = ["all"], version = "^0.9.0" }
-manim = "^0.18.0"
-discord-webhook = "^1.3.1"
 verlat = "^0.1.0.post1"
-rich = "^13.7.1"
-ipython = "^8.23.0"
-pymongo = "^4.6.3"
-pyyaml = "^6.0.1"
+redis = "^5.0.3"
+python-telegram-bot = { extras = ["callback-data", "socks"], version = "^21.1" }
 
 [tool.poetry.scripts]
 btc-eth = 'main.btc_eth:run'
+captcha = 'main.captcha:run'
+dcw = 'main.dc_webhook_send:run'
 dt = 'main.ts:run'
 e = 'main.env:run'
 ms = 'main.ts:ms'
 nano = 'main.ts:nano'
 os = 'main.os:run'
 rmw = 'main.rmw:run'
 say = 'main.say:run'
-tgl = 'main.tg_login:run'
+t2m = 'main.t2m:run'
 tgf = 'main.tg_forward:run'
+tgl = 'main.tg_login:run'
+tgkm = 'main.tg_koltime_menu:run'
 ts = 'main.ts:sec'
 uuid = 'main.uu_id:run'
-captcha = 'main.captcha:run'
-t2m = 'main.t2m:run'
-dcw = 'main.dc_webhook_send:run'
-
-[build-system]
-build-backend = "poetry.core.masonry.api"
-requires = ["poetry-core"]
 
 [[tool.poetry.source]]
 name = "aliyun"
 priority = "primary"
 url = "https://mirrors.aliyun.com/pypi/simple"
 
-[virtualenvs]
-create = true
-in-project = true
-cache-dir = "e:/cache/poetry"
+# ---
+# [virtualenvs]
+# cache-dir = "e:/cache/poetry"
+# create = true
+# in-project = true
+
+[build-system]
+build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core"]
```

### Comparing `fei_crypto-0.1.6/README.md` & `fei_crypto-0.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,17 +51,17 @@
     - webhook_url:webhook url
     - --text:发送的文本
     - --file-paths:发送的文件路径,多个路径用逗号分隔
     - --proxy:使用代理,例如`http://127.0.0.1:7890`
     - --help:帮助文档
 15. tgf # 转发telegram group或channel,支持用户转发和机器人转发,转发规则在配置文件`forwards`节点下
     - 用户转发需申请对应的api_id,api_hash,并使用以上`tgl`命令获取`sesssionString`,网址:`https://my.telegram.org/auth`
-    - 用户转发需在配置文件中填写`API_ID`,`API_HASH`,`SESSION_STRING`
+    - 用户转发需在配置文件中填写`API_ID`,`API_HASH`,`SESSION_STRING`,`"user_type": 1`
     - 机器人转发直接到telegram`@BotFather` 里按流程申请Token
-    - 机器人转发需在配置文件中填写`BOT_TOKEN`
+    - 机器人转发需在配置文件中填写`BOT_TOKEN`,`"user_type": 0`
     - 代理配置,在配置文件login下配置`"PROXY": "socks5://127.0.0.1:7890"`
     - 示例:`tgf live -c "d:/tg.config.json"` 默认值:当前目录下的`tg.config.json`
     - mode:`live`或者`past` live:实时转发 past:每分钟读取历史记录转发,第一次默认读取一个小时内的记录
     - --config-path,-c: 可传入任意配置文件路径,不传会在当前目录下创建`tg.config.json`,在json文件中填写配置重新运行即可
     - --version,-v: 查看版本信息
     - --help:帮助文档
```

### Comparing `fei_crypto-0.1.6/tg/bot/live_bot.py` & `fei_crypto-0.1.7/tg/bot/live_bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 from telethon import events
 
 from tg import config, const, plugins
 from tg.bot.utils import (
     admin_protect,
     display_forwards,
     get_args,
-    get_command_prefix,
     remove_source,
 )
 from tg.config import CONFIG, write_config
 from tg.plugin_models import Style
+from tg.utils import get_command_prefix
 
 
 @admin_protect
 async def forward_command_handler(event):
     """Handle the `/forward` command."""
     notes = """The `/forward` command allows you to add a new forward.
     Example: suppose you want to forward from a to (b and c)
```

### Comparing `fei_crypto-0.1.6/tg/bot/utils.py` & `fei_crypto-0.1.7/tg/bot/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,11 +56,8 @@
     for i, forward in enumerate(forwards):
         if forward.source == source:
             del forwards[i]
             return forwards
     raise ValueError("The source does not exist")
 
 
-def get_command_prefix():
-    if config.is_bot is None:
-        raise ValueError("config.is_bot is not set!")
-    return "/" if config.is_bot else "\."
+
```

### Comparing `fei_crypto-0.1.6/tg/cli_forward.py` & `fei_crypto-0.1.7/tg/cli_forward.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.6/tg/cli_login.py` & `fei_crypto-0.1.7/tg/cli_login.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.6/tg/config.py` & `fei_crypto-0.1.7/tg/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         return val
 
 
 class LoginConfig(BaseModel):
     API_ID: int = 0
     API_HASH: str = ""
     user_type: int = 0  # 0:bot, 1:user
-    phone_no: int = 91
+    phone_no: int = 86
     USERNAME: str = ""
     SESSION_STRING: str = ""
     BOT_TOKEN: str = ""
     PROXY: str = ""
 
 
 class BotMessages(BaseModel):
```

### Comparing `fei_crypto-0.1.6/tg/live.py` & `fei_crypto-0.1.7/tg/live.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.6/tg/login.py` & `fei_crypto-0.1.7/tg/login.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.6/tg/message.py` & `fei_crypto-0.1.7/tg/message.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.6/tg/past.py` & `fei_crypto-0.1.7/tg/past.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.6/tg/plugin_models.py` & `fei_crypto-0.1.7/tg/plugin_models.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.6/tg/plugins/__init__.py` & `fei_crypto-0.1.7/tg/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.6/tg/plugins/filter.py` & `fei_crypto-0.1.7/tg/plugins/filter.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.6/tg/plugins/fmt.py` & `fei_crypto-0.1.7/tg/plugins/fmt.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.6/tg/plugins/replace.py` & `fei_crypto-0.1.7/tg/plugins/replace.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.6/tg/storage.py` & `fei_crypto-0.1.7/tg/storage.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.6/tg/utils.py` & `fei_crypto-0.1.7/tg/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Utility functions to smoothen your life."""
 
 import logging
 import os
 import re
 from datetime import datetime
+from tg import config
 from tg.plugin_models import STYLE_CODES
 
 
 def cleanup(*files: str) -> None:
     """Delete the file names passed as args."""
     for file in files:
         try:
@@ -56,7 +57,13 @@
         return string.replace(pattern, new)
 
 
 def clean_session_files():
     for item in os.listdir():
         if item.endswith(".session") or item.endswith(".session-journal"):
             os.remove(item)
+
+
+def get_command_prefix():
+    if config.is_bot is None:
+        raise ValueError("config.is_bot is not set!")
+    return "/" if config.is_bot else "\."
```

### Comparing `fei_crypto-0.1.6/PKG-INFO` & `fei_crypto-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fei-crypto
-Version: 0.1.6
+Version: 0.1.7
 Summary: fei crypto command utils
 License: MIT
 Author: feicrypto
 Author-email: feicrypto@proton.me
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,17 @@
 Requires-Dist: filestools (>=0.2.1,<0.3.0)
 Requires-Dist: ipython (>=8.23.0,<9.0.0)
 Requires-Dist: manim (>=0.18.0,<0.19.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: pymongo (>=4.6.3,<5.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: python-socks[asyncio] (>=2.4.3,<3.0.0)
+Requires-Dist: python-telegram-bot[callback-data,socks] (>=21.1,<22.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Requires-Dist: redis (>=5.0.3,<6.0.0)
 Requires-Dist: requests[socks] (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: telethon (>=1.34.0,<2.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Requires-Dist: verlat (>=0.1.0.post1,<0.2.0)
 Description-Content-Type: text/markdown
 
@@ -80,17 +82,17 @@
     - webhook_url:webhook url
     - --text:发送的文本
     - --file-paths:发送的文件路径,多个路径用逗号分隔
     - --proxy:使用代理,例如`http://127.0.0.1:7890`
     - --help:帮助文档
 15. tgf # 转发telegram group或channel,支持用户转发和机器人转发,转发规则在配置文件`forwards`节点下
     - 用户转发需申请对应的api_id,api_hash,并使用以上`tgl`命令获取`sesssionString`,网址:`https://my.telegram.org/auth`
-    - 用户转发需在配置文件中填写`API_ID`,`API_HASH`,`SESSION_STRING`
+    - 用户转发需在配置文件中填写`API_ID`,`API_HASH`,`SESSION_STRING`,`"user_type": 1`
     - 机器人转发直接到telegram`@BotFather` 里按流程申请Token
-    - 机器人转发需在配置文件中填写`BOT_TOKEN`
+    - 机器人转发需在配置文件中填写`BOT_TOKEN`,`"user_type": 0`
     - 代理配置,在配置文件login下配置`"PROXY": "socks5://127.0.0.1:7890"`
     - 示例:`tgf live -c "d:/tg.config.json"` 默认值:当前目录下的`tg.config.json`
     - mode:`live`或者`past` live:实时转发 past:每分钟读取历史记录转发,第一次默认读取一个小时内的记录
     - --config-path,-c: 可传入任意配置文件路径,不传会在当前目录下创建`tg.config.json`,在json文件中填写配置重新运行即可
     - --version,-v: 查看版本信息
     - --help:帮助文档
```

