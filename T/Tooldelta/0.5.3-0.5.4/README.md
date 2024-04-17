# Comparing `tmp/tooldelta-0.5.3.tar.gz` & `tmp/tooldelta-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tooldelta-0.5.3.tar", max compression
+gzip compressed data, was "tooldelta-0.5.4.tar", max compression
```

## Comparing `tooldelta-0.5.3.tar` & `tooldelta-0.5.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rwxr-xr-x   0        0        0     1497 2024-04-14 08:09:42.324543 tooldelta-0.5.3/LICENSE
--rwxr-xr-x   0        0        0     2504 2024-04-14 08:09:42.324543 tooldelta-0.5.3/README.md
--rwxr-xr-x   0        0        0      929 2024-04-14 08:09:51.320553 tooldelta-0.5.3/pyproject.toml
--rwxr-xr-x   0        0        0      330 2024-04-14 08:09:42.328543 tooldelta-0.5.3/tooldelta/__init__.py
--rw-r--r--   0        0        0     5906 2024-04-14 08:09:42.328543 tooldelta-0.5.3/tooldelta/auths.py
--rwxr-xr-x   0        0        0      599 2024-04-14 08:09:42.328543 tooldelta-0.5.3/tooldelta/basic_mods.py
--rwxr-xr-x   0        0        0    16782 2024-04-14 08:09:42.328543 tooldelta-0.5.3/tooldelta/builtins.py
--rwxr-xr-x   0        0        0    10594 2024-04-14 08:09:42.328543 tooldelta-0.5.3/tooldelta/cfg.py
--rwxr-xr-x   0        0        0     7848 2024-04-14 08:09:42.328543 tooldelta-0.5.3/tooldelta/color_print.py
--rw-r--r--   0        0        0     2045 2024-04-14 08:09:42.328543 tooldelta-0.5.3/tooldelta/constants.py
--rw-r--r--   0        0        0     5870 2024-04-14 08:09:42.328543 tooldelta-0.5.3/tooldelta/fb_conn/fbconn.py
--rwxr-xr-x   0        0        0    34708 2024-04-14 08:09:42.328543 tooldelta-0.5.3/tooldelta/frame.py
--rwxr-xr-x   0        0        0     3772 2024-04-14 08:09:42.328543 tooldelta-0.5.3/tooldelta/game_texts.py
--rwxr-xr-x   0        0        0      338 2024-04-14 08:09:42.328543 tooldelta-0.5.3/tooldelta/get_tool_delta_version.py
--rwxr-xr-x   0        0        0    30695 2024-04-14 08:09:42.328543 tooldelta-0.5.3/tooldelta/launch_cli.py
--rwxr-xr-x   0        0        0     1080 2024-04-14 08:09:42.328543 tooldelta-0.5.3/tooldelta/launch_options.py
--rwxr-xr-x   0        0        0     2138 2024-04-14 08:09:42.328543 tooldelta-0.5.3/tooldelta/logger.py
--rwxr-xr-x   0        0        0    29503 2024-04-14 08:09:42.328543 tooldelta-0.5.3/tooldelta/neo_libs/neo_conn.py
--rwxr-xr-x   0        0        0     1143 2024-04-14 08:09:42.328543 tooldelta-0.5.3/tooldelta/packets.py
--rwxr-xr-x   0        0        0    11378 2024-04-14 08:09:42.328543 tooldelta-0.5.3/tooldelta/plugin_load/PluginGroup.py
--rwxr-xr-x   0        0        0     2273 2024-04-14 08:09:42.328543 tooldelta-0.5.3/tooldelta/plugin_load/__init__.py
--rwxr-xr-x   0        0        0     6200 2024-04-14 08:09:42.328543 tooldelta-0.5.3/tooldelta/plugin_load/classic_plugin/__init__.py
--rwxr-xr-x   0        0        0      345 2024-04-14 08:09:42.328543 tooldelta-0.5.3/tooldelta/plugin_load/funcs.py
--rwxr-xr-x   0        0        0     6780 2024-04-14 08:09:42.328543 tooldelta-0.5.3/tooldelta/plugin_load/injected_plugin/__init__.py
--rwxr-xr-x   0        0        0     9235 2024-04-14 08:09:42.328543 tooldelta-0.5.3/tooldelta/plugin_load/injected_plugin/movent.py
--rwxr-xr-x   0        0        0    13702 2024-04-14 08:09:42.328543 tooldelta-0.5.3/tooldelta/plugin_manager.py
--rwxr-xr-x   0        0        0    13369 2024-04-14 08:09:42.328543 tooldelta-0.5.3/tooldelta/plugin_market.py
--rw-r--r--   0        0        0     1864 2024-04-14 08:09:42.328543 tooldelta-0.5.3/tooldelta/starter.py
--rwxr-xr-x   0        0        0      638 2024-04-14 08:09:42.328543 tooldelta-0.5.3/tooldelta/sys_args.py
--rwxr-xr-x   0        0        0     7057 2024-04-14 08:09:42.328543 tooldelta-0.5.3/tooldelta/urlmethod.py
--rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 tooldelta-0.5.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1497 2024-04-17 13:22:32.158901 tooldelta-0.5.4/LICENSE
+-rwxr-xr-x   0        0        0     2504 2024-04-17 13:22:32.158901 tooldelta-0.5.4/README.md
+-rwxr-xr-x   0        0        0      973 2024-04-17 13:22:49.482918 tooldelta-0.5.4/pyproject.toml
+-rwxr-xr-x   0        0        0      330 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/__init__.py
+-rw-r--r--   0        0        0     4963 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/auths.py
+-rwxr-xr-x   0        0        0      599 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/basic_mods.py
+-rwxr-xr-x   0        0        0    16782 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/builtins.py
+-rwxr-xr-x   0        0        0    10594 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/cfg.py
+-rwxr-xr-x   0        0        0     7848 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/color_print.py
+-rw-r--r--   0        0        0     2045 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/constants.py
+-rw-r--r--   0        0        0     5870 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/fb_conn/fbconn.py
+-rwxr-xr-x   0        0        0    29713 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/frame.py
+-rwxr-xr-x   0        0        0     3772 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/game_texts.py
+-rwxr-xr-x   0        0        0      338 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/get_tool_delta_version.py
+-rwxr-xr-x   0        0        0    31347 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/launch_cli.py
+-rwxr-xr-x   0        0        0     1080 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/launch_options.py
+-rwxr-xr-x   0        0        0     2138 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/logger.py
+-rwxr-xr-x   0        0        0    29561 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/neo_libs/neo_conn.py
+-rwxr-xr-x   0        0        0     1143 2024-04-17 13:22:32.158901 tooldelta-0.5.4/tooldelta/packets.py
+-rwxr-xr-x   0        0        0    11378 2024-04-17 13:22:32.162901 tooldelta-0.5.4/tooldelta/plugin_load/PluginGroup.py
+-rwxr-xr-x   0        0        0     2318 2024-04-17 13:22:32.162901 tooldelta-0.5.4/tooldelta/plugin_load/__init__.py
+-rwxr-xr-x   0        0        0     6200 2024-04-17 13:22:32.162901 tooldelta-0.5.4/tooldelta/plugin_load/classic_plugin/__init__.py
+-rwxr-xr-x   0        0        0      345 2024-04-17 13:22:32.162901 tooldelta-0.5.4/tooldelta/plugin_load/funcs.py
+-rwxr-xr-x   0        0        0     6780 2024-04-17 13:22:32.162901 tooldelta-0.5.4/tooldelta/plugin_load/injected_plugin/__init__.py
+-rwxr-xr-x   0        0        0     9235 2024-04-17 13:22:32.162901 tooldelta-0.5.4/tooldelta/plugin_load/injected_plugin/movent.py
+-rwxr-xr-x   0        0        0    13702 2024-04-17 13:22:32.162901 tooldelta-0.5.4/tooldelta/plugin_manager.py
+-rwxr-xr-x   0        0        0    13481 2024-04-17 13:22:32.162901 tooldelta-0.5.4/tooldelta/plugin_market.py
+-rw-r--r--   0        0        0     1758 2024-04-17 13:22:32.162901 tooldelta-0.5.4/tooldelta/starter.py
+-rwxr-xr-x   0        0        0      638 2024-04-17 13:22:32.162901 tooldelta-0.5.4/tooldelta/sys_args.py
+-rwxr-xr-x   0        0        0     9071 2024-04-17 13:22:32.162901 tooldelta-0.5.4/tooldelta/urlmethod.py
+-rw-r--r--   0        0        0     3743 1970-01-01 00:00:00.000000 tooldelta-0.5.4/PKG-INFO
```

### Comparing `tooldelta-0.5.3/LICENSE` & `tooldelta-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.3/README.md` & `tooldelta-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.3/pyproject.toml` & `tooldelta-0.5.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Tooldelta"
-version = "0.5.3" # This field is automatically set to the value in the version file
+version = "0.5.4" # This field is automatically set to the value in the version file
 description = "Plugin Loader for NeteaseRentalServer on Panel"
 authors = ["SuperScript-PRC"]
 license = ""
 
 readme = "README.md"
 homepage = "https://github.com/SuperScript-PRC/ToolDelta"
 repository = "https://github.com/SuperScript-PRC/ToolDelta"
@@ -24,11 +24,13 @@
 pillow = "^10.2.0"
 shellescape = "^3.8.1"
 pyspeedtest = "1.2.7"
 tqdm = "4.66.2"
 aiohttp = "^3.9.3"
 python-socketio = "5.11.1"
 flask = "^3.0.2"
+mido = "^1.3.2"
+websocket-client = "^1.7.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tooldelta-0.5.3/tooldelta/auths.py` & `tooldelta-0.5.4/tooldelta/auths.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,156 +1,137 @@
-import requests, getpass, hashlib, json
+from typing import Any
+import requests
+import getpass
+import json
+import hashlib
 from tooldelta import constants
 from tooldelta.color_print import Print
 
-def login_liliya():
-    while 1:
-        hash_obj: hashlib._Hash = hashlib.sha256()
-        username: str = input(Print.fmt_info("请输入账号:", "§6 账号 "))
-        hash_obj.update(
-            getpass.getpass(Print.fmt_info("请输入密码(已隐藏):", "§6 密码 ")).encode()
-        )
-        __password: str = hash_obj.hexdigest()
-        Authorization: str = requests.get(url=constants.GUGU_APIS[1], timeout=5).text
-        repo: requests.Response = requests.post(
-            url=constants.GUGU_APIS[0],
-            data=json.dumps(
-                {
-                    "client_public_key": "",
-                    "server_code": "::DRY::",
-                    "server_passcode": "::DRY::",
-                    "username": username,
-                    "password": __password,
-                },
-                ensure_ascii=False,
-            ),
-            headers={
-                "Content-Type": "application/json",
-                "Authorization": f"Bearer {Authorization}",
-            }, timeout=5
-        )
-        repo_text: dict = json.loads(repo.text)
-        repo_message: str = repo_text["message"]
-        repo_success: bool = repo_text["success"]
-        if repo.status_code != 200:
-            Print.print_war(
-                f"请求Api接口失败，将自动使用Token登陆!状态码:{repo.status_code}，返回值:{repo.text}"
-            )
-            return
-        if not repo_success:
-            if "无效的用户中心用户名或密码" in repo_message:
-                Print.print_war("登录失败, 无效的用户名、密码或MFA代码!")
-            else:
-                Print.print_war("登录失败, 原因: " + repo_message + ", 请重试!")
-        else:
-            break
-    token = repo_text["token"]
-    with open("fbtoken", "w", encoding="utf-8") as f:
-        f.write(token)
 
-def login_fbuc():
-    while 1:
-        hash_obj: hashlib._Hash = hashlib.sha256()
-        username: str = input(Print.fmt_info("请输入账号:", "§6 账号 "))
-        hash_obj.update(
-            getpass.getpass(
-                Print.fmt_info("请输入密码(已隐藏):", "§6 密码 ")
-            ).encode()
-        )
-        __password: str = hash_obj.hexdigest()
-        __mfa_code: str = getpass.getpass(
-            Print.fmt_info(
-                "请输入双重验证码(已隐藏)(如未设置请直接回车):", "§6 MFA  "
-            )
-        )
-        Authorization: str = requests.get(url=constants.FB_APIS[1], timeout=5).text
-        repo: requests.Response = requests.post(
-            url=constants.FB_APIS[3],
-            data=json.dumps(
-                {
-                    "username": username,
-                    "password": __password,
-                    "mfa_code": __mfa_code,
-                },
-                ensure_ascii=False,
-            ),
-            headers={
-                "Content-Type": "application/json",
-                "authorization": f"Bearer {Authorization}",
+def liliya_login() -> str:
+    """登录咕咕账号
+
+    Raises:
+        requests.exceptions.RequestException: 登录失败
+    """
+    hash_obj = hashlib.sha256()
+    username = input(Print.fmt_info("请输入账号:", "§6 账号 "))
+    hash_obj.update(
+        getpass.getpass(Print.fmt_info("请输入密码(已隐藏):", "§6 密码 ")).encode()
+    )
+    password = hash_obj.hexdigest()
+    auth_key = requests.get(url=constants.GUGU_APIS[1], timeout=5).text
+    repo = requests.post(
+        url=constants.GUGU_APIS[0],
+        data=json.dumps(
+            {
+                "client_public_key": "",
+                "server_code": "::DRY::",
+                "server_passcode": "::DRY::",
+                "username": username,
+                "password": password,
             },
+            ensure_ascii=False,
+        ),
+        headers={
+            "Content-Type": "application/json",
+            "Authorization": f"Bearer {auth_key}",
+        }, timeout=5
+    )
+    repo_text: dict[str, Any] = json.loads(repo.text)
+    repo_message: str = repo_text["message"]
+    repo_success: bool = repo_text["success"]
+    if repo.status_code != 200:
+        Print.print_war(
+            f"请求Api接口失败，将自动使用Token登陆! 状态码:{repo.status_code}，返回值:{repo.text}"
         )
-        repo_text: dict = json.loads(repo.text)
-        repo_message: str = repo_text["message"]
-        repo_success: bool = repo_text["success"]
-        if repo.status_code != 200:
-            Print.print_war(
-                f"请求Api接口失败，将自动使用Token登陆! 状态码:{repo.status_code}，返回值:{repo.text}"
-            )
-            return
-        if not repo_success:
-            if "Invalid username, password, or MFA code." in repo_message:
-                Print.print_war("登陆失败; 无效的用户名、密码或MFA代码!")
-            else:
-                Print.print_war("登录失败, 原因: " + repo_message + ", 请重试!")
-        else:
-            break
-    with_perfix: dict = json.loads(
-        requests.get(
-            url=constants.FB_APIS[2],
-            data=json.dumps({"with_prefix": constants.FB_APIS[4]}),
-            timeout=5,
-            headers={
-                "Content-Type": "application/json",
-                "authorization": f"Bearer {Authorization}",
-            },
-        ).text
+        raise requests.exceptions.RequestException("请求Api接口失败", repo)
+    if not repo_success:
+        if "无效的用户中心用户名或密码" in repo_message:
+            Print.print_war("登录失败, 无效的用户名或密码!")
+            raise requests.exceptions.RequestException("无效的用户名或密码")
+        Print.print_war(f"登录失败, 原因: {repo_message}")
+        raise requests.exceptions.RequestException("登录无效", repo)
+    token = repo_text["token"]
+    return token
+
+
+def fbuc_login() -> str:
+    """登录FastBuilder账号
+
+    Raises:
+        requests.exceptions.RequestException: 登录失败
+    """
+    hash_obj = hashlib.sha256()
+    username = input(Print.fmt_info("请输入账号:", "§6 账号 "))
+    hash_obj.update(
+        getpass.getpass(
+            Print.fmt_info("请输入密码(已隐藏):", "§6 密码 ")
+        ).encode()
     )
-    fetch_announcements: dict = json.loads(
-        requests.get(
-            url=constants.FB_APIS[4] + with_perfix["fetch_announcements"],
-            timeout=5,
-            headers={
-                "Content-Type": "application/json",
-                "authorization": f"Bearer {Authorization}",
-            },
-        ).text
+    password = hash_obj.hexdigest()
+    mfa_code = getpass.getpass(
+        Print.fmt_info(
+            "请输入双重验证码(已隐藏)(如未设置请直接回车):", "§6 MFA  "
+        )
     )
-    fetch_profile: dict = json.loads(
-        requests.get(
-            url=constants.FB_APIS[4] + with_perfix["fetch_profile"],
-            timeout=5,
-            headers={
-                "Content-Type": "application/json",
-                "authorization": f"Bearer {Authorization}",
+    auth_key = requests.get(url=constants.FB_APIS[1], timeout=5).text
+    repo = requests.post(
+        url=constants.FB_APIS[3],
+        data=json.dumps(
+            {
+                "username": username,
+                "password": password,
+                "mfa_code": mfa_code,
             },
-        ).text
+            ensure_ascii=False,
+        ),
+        headers={
+            "Content-Type": "application/json",
+            "authorization": f"Bearer {auth_key}",
+        },
+        timeout=5
     )
-    get_helper_status: dict = json.loads(
-        requests.get(
-            url=constants.FB_APIS[4] + with_perfix["get_helper_status"],
-            timeout=5,
-            headers={
-                "Content-Type": "application/json",
-                "authorization": f"Bearer {Authorization}",
-            },
-        ).text
+    repo_text: dict[str, Any] = json.loads(repo.text)
+    repo_message: str = repo_text["message"]
+    repo_success: bool = repo_text["success"]
+    if repo.status_code != 200:
+        Print.print_war(
+            f"请求Api接口失败，将自动使用Token登陆! 状态码:{repo.status_code}，返回值:{repo.text}"
+        )
+        raise requests.exceptions.RequestException("请求Api接口失败", repo)
+
+    if not repo_success:
+        if "Invalid username, password, or MFA code." in repo_message:
+            raise requests.exceptions.RequestException("无效的用户名、密码或MFA代码")
+        raise requests.exceptions.RequestException("登录无效", repo)
+    # 获取token前缀
+    repo = requests.get(
+        url=constants.FB_APIS[2],
+        data=json.dumps({"with_prefix": constants.FB_APIS[4]}),
+        timeout=5,
+        headers={
+            "Content-Type": "application/json",
+            "authorization": f"Bearer {auth_key}",
+        },
     )
-    UserInfo: dict = {
-        "isadmin": repo_text["isadmin"],
-        "blc": fetch_profile["blc"],
-            "cn_username": fetch_profile["cn_username"],
-            "phoenix_otp": fetch_profile["phoenix_otp"],
-            "points": fetch_profile["points"],
-            "slots": fetch_profile["slots"],
-            "get_helper_status": get_helper_status,
-        }
-    token = requests.get(
+    if repo.status_code != 200:
+        Print.print_war(
+            f"无法获取tokenx信息! 状态码:{repo.status_code}，返回值:{repo.text}"
+        )
+        raise requests.exceptions.RequestException("请求Api接口失败", repo)
+    with_perfix: dict[str, Any] = json.loads(repo.text)
+    token_request = requests.get(
         url=constants.FB_APIS[4] + with_perfix["get_phoenix_token"],
-        data=json.dumps({"secret": f"{Authorization}"}),
+        data=json.dumps({"secret": f"{auth_key}"}),
         timeout=5,
         headers={
             "Content-Type": "application/json",
-            "authorization": f"Bearer {Authorization}",
+            "authorization": f"Bearer {auth_key}",
         },
-    ).text
-    with open("fbtoken", "w", encoding="utf-8") as f:
-        f.write(token)
+    )
+    if token_request.status_code != 200:
+        Print.print_war(
+            f"无法获取tokenx信息! 状态码:{token_request.status_code}，返回值:{token_request.text}"
+        )
+        raise requests.exceptions.RequestException("请求Api接口失败", token_request)
+    return token_request.text
```

### Comparing `tooldelta-0.5.3/tooldelta/basic_mods.py` & `tooldelta-0.5.4/tooldelta/basic_mods.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.3/tooldelta/builtins.py` & `tooldelta-0.5.4/tooldelta/builtins.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.3/tooldelta/cfg.py` & `tooldelta-0.5.4/tooldelta/cfg.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.3/tooldelta/color_print.py` & `tooldelta-0.5.4/tooldelta/color_print.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.3/tooldelta/constants.py` & `tooldelta-0.5.4/tooldelta/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List
 from tooldelta.launch_cli import FrameFBConn, FrameNeOmg, FrameNeOmgRemote
 from tooldelta.cfg import Cfg
 
 PRG_NAME = "ToolDelta"
 
-PLUGIN_MARKET_SOURCE_OFFICIAL = "https://gh.api.99988866.xyz/https://raw.githubusercontent.com/ToolDelta/ToolDelta-PluginMarket/main"
+PLUGIN_MARKET_SOURCE_OFFICIAL = "https://tdload.tblstudio.cn/https://raw.githubusercontent.com/ToolDelta/ToolDelta-PluginMarket/main"
 
 LAUNCHERS: List[
     tuple[str, type[FrameFBConn | FrameNeOmg | FrameNeOmgRemote]]
 ] = [
     (
         "FastBuilder External 模式 (经典模式) §c(已停止维护, 无法适应新版本租赁服!)",
         FrameFBConn,
```

### Comparing `tooldelta-0.5.3/tooldelta/fb_conn/fbconn.py` & `tooldelta-0.5.4/tooldelta/fb_conn/fbconn.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.3/tooldelta/frame.py` & `tooldelta-0.5.4/tooldelta/frame.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,41 @@
+"""
+整个系统由三个部分组成
+    Frame: 负责整个 ToolDelta 的基本框架运行
+    GameCtrl: 负责对接游戏
+        - Launchers: 负责将不同启动器的游戏接口统一成固定的接口, 供插件在多平台游戏接口运行(FastBuilder External, NeOmega, (TLSP, etc.))
+"""
 
+
+from typing import TYPE_CHECKING
 import tooldelta
 from tooldelta import (
     auths,
     constants,
-    builtins,
     plugin_market,
-    sys_args,
 )
-
-from tooldelta.get_tool_delta_version import get_tool_delta_version
-from tooldelta.color_print import Print
-from tooldelta.basic_mods import (
+from .constants import PRG_NAME
+from .builtins import Builtins, safe_close
+from .get_tool_delta_version import get_tool_delta_version
+from .color_print import Print
+from .basic_mods import (
     Callable,
     os,
     sys,
     time,
     traceback,
     requests,
-    platform,
-    subprocess,
-    threading,
     getpass
 )
-
-from tooldelta.cfg import Cfg
-from tooldelta.logger import publicLogger
-from tooldelta.plugin_load.PluginGroup import PluginGroup
-from tooldelta.game_texts import GameTextsLoader
-from tooldelta.urlmethod import download_file_multithreading, test_site_latency
-from tooldelta.sys_args import sys_args_to_dict
-from tooldelta.launch_cli import (
+from .cfg import Cfg
+from .logger import publicLogger
+from .game_texts import GameTextsLoader
+from .urlmethod import if_token, fbtokenFix
+from .sys_args import sys_args_to_dict
+from .launch_cli import (
     FrameFBConn,
     FrameNeOmg,
     FrameNeOmgRemote,
     SysStatus,
 )
 
 from .basic_mods import asyncio, json
@@ -46,233 +48,81 @@
     execute_player_left,
     execute_player_message,
     execute_repeat,
     safe_jump,
 )
 
 sys_args_dict = sys_args_to_dict(sys.argv)
-createThread = builtins.Builtins.createThread
 VERSION = get_tool_delta_version()
-Builtins = builtins.Builtins
 Config = Cfg()
-
-# 整个系统由三个部分组成
-#  Frame: 负责整个 ToolDelta 的基本框架运行
-#  GameCtrl: 负责对接游戏
-#    - Launchers: 负责将不同启动器的游戏接口统一成固定的接口, 供插件在多平台游戏接口运行(FastBuilder External, NeOmega, (TLSP, etc.))
-#  PluginGroup: 负责管理和运行插件
+if TYPE_CHECKING:
+    from .plugin_load.PluginGroup import PluginGroup
 
 
 class Frame:
-    # 系统框架
-    class SystemVersionException(OSError):
-        ...
+    """系统框架"""
 
     class FrameBasic:
+        """系统基本信息"""
         system_version = VERSION
         max_connect_fb_time = 60
         connect_fb_start_time = time.time()
         data_path = "插件数据文件/"
 
-    createThread = ClassicThread = Builtins.createThread
-    PRG_NAME = constants.PRG_NAME
-    sys_data = FrameBasic()
-    serverNumber: str = ""
-    serverPasswd: str
-    launchMode: int = 0
-    consoleMenu = []
-    link_game_ctrl = None
-    link_plugin_group = None
-    on_plugin_err = staticmethod(
-        lambda name, _, err: Print.print_err(f"插件 <{name}> 出现问题: \n{err}")
-    )
-    is_mir: bool
-    plugin_market_url: str
-
-    @staticmethod
-    def check_use_token(tok_name="", check_md=""):
-        res = sys_args.sys_args_to_dict()
-        res = res.get(tok_name, 1)
-        if (res == 1 and check_md) or res != check_md:
-            Print.print_err("启动参数错误")
-            raise SystemExit
-
-    @staticmethod
-    def if_token():
-        if not os.path.isfile("fbtoken"):
-            Print.print_err(
-                "请到对应的验证服务器官网下载FBToken, 并放在本目录中, 或者在下面输入fbtoken"
-            )
-            fbtoken = input(Print.fmt_info("请输入fbtoken: ", "§b 输入 "))
-            if fbtoken:
-                with open("fbtoken", "w", encoding="utf-8") as f:
-                    f.write(fbtoken)
-            else:
-                Print.print_err("未输入fbtoken, 无法继续")
-                raise SystemExit
-
-    class ToolDeltaUpdater:
-        def __init__(self, launcher):
-            self.launcher = launcher
-            self.auto_update(self.launcher)
-            self.start_auto_update_thread()
-
-        def start_auto_update_thread(self):
-            # 每24小时检查一次更新
-            threading.Timer(24 * 60 * 60, self.auto_update,
-                            args=(self.launcher)).start()
-
-        @staticmethod
-        def auto_update(launcher):
-            try:
-                try:
-                    num: int = 0  # 初始化计次器数据
-                    while True:
-                        if launcher.TDC.SocketIO.connected:
-                            latest_version = launcher.TDC.get_version_updates()
-                            break
-                        else:
-                            time.sleep(0.1)
-                            num = num + 1
-                        if num >= 50:
-                            latest_version = requests.get(
-                                "https://api.github.com/repos/ToolDelta/ToolDelta/releases/latest").json()["tag_name"]
-                            break
-                except:
-                    latest_version = requests.get(
-                        "https://api.github.com/repos/ToolDelta/ToolDelta/releases/latest").json()["tag_name"]
-                current_version = ".".join(
-                    map(str, get_tool_delta_version()[:3]))
-
-                if latest_version.replace(".", "") <= current_version.replace(".", ""):
-                    # Print.print_suc(f"检测成功,当前为最新版本 -> {current_version.replace('.', '')}，无需更新")
-                    return
-                if ".py" in os.path.basename(
-                    __file__
-                ) and ".pyc" not in os.path.basename(__file__):
-                    Print.print_load(
-                        f"检测到最新版本 -> {latest_version}，请及时拉取最新版本代码!"
-                    )
-                else:
-                    tooldelta_url = f"github.com/ToolDelta/ToolDelta/releases/download/{latest_version}"
-                    url = (
-                        f"https://gh.con.sh/{tooldelta_url}/ToolDelta-linux"
-                        if platform.system() == "Linux"
-                        else f"https://gh.con.sh/{tooldelta_url}/ToolDelta-windows.exe"
-                    )
-                    mirror_urls = (
-                        [
-                            f"https://gh.api.99988866.xyz/{tooldelta_url}/ToolDelta-linux",
-                            f"https://hub.gitmirror.com/{tooldelta_url}/ToolDelta-linux",
-                        ]
-                        if platform.system() == "Linux"
-                        else [
-                            f"https://gh.api.99988866.xyz/{tooldelta_url}/ToolDelta-windows.exe",
-                            f"https://hub.gitmirror.com/{tooldelta_url}/ToolDelta-windows.exe",
-                        ]
-                    )
-                    file_path = (
-                        os.path.join(os.getcwd(), "ToolDelta-linux_new")
-                        if platform.system() == "Linux"
-                        else os.path.join(os.getcwd(), "ToolDelta-windows_new.exe")
-                    )
-                    fastest_url = next(
-                        iter(test_site_latency(
-                            {"url": url, "mirror_url": mirror_urls}))
-                    )
-
-                    if not fastest_url:
-                        Print.print_war(
-                            "在检测源速度时出现异常，所有镜像源以及官方源均无法访问，请检查网络是否正常!"
-                        )
-                        return
-
-                    with Print.lock:
-                        Print.print_load(
-                            f"检测到最新版本 -> {latest_version}，正在下载最新版本的ToolDelta"
-                        )
-                    download_file_multithreading(fastest_url[0], file_path)
-
-                    if os.path.exists(file_path):
-                        if platform.system() == "Windows":
-                            win_old_tool_delta_path = next(
-                                os.path.join(filewalks[0], files)
-                                for filewalks, _, files in os.walk(os.getcwd())
-                                if any(
-                                    ".exe" in file
-                                    and "new" not in file
-                                    and ("ToolDelta" in file or "tooldelta" in file)
-                                    for file in files
-                                )
-                            )
-
-                        upgrade_script_path = (
-                            "upgrade.sh"
-                            if platform.system() == "Linux"
-                            else "upgrade.bat"
-                        )
-                        with open(
-                            upgrade_script_path, "w", encoding="utf-8"
-                        ) as upgrade_script:
-                            temp_shell = (
-                                f'#!/bin/bash\nif [ -f "{file_path}" ];then\n  sleep 3\n  rm -f {os.getcwd()}/{os.path.basename(__file__)}\n  mv {os.getcwd()}/ToolDelta-linux_new {os.getcwd()}/{os.path.basename(__file__)}\n  /usr/bin/chmod 777 {os.path.basename(__file__)}\n  ./{os.path.basename(__file__)} -l 1\nelse\n  exit\nfi'
-                                if platform.system() == "Linux"
-                                else f"@echo off\ncd {os.getcwd()}\nif not exist {win_old_tool_delta_path} exit\ntimeout /T 3 /NOBREAK\ndel {win_old_tool_delta_path}\nren ToolDelta-windows_new.exe {os.path.basename(win_old_tool_delta_path)}\nstart {os.path.basename(win_old_tool_delta_path)}"
-                            )
-                            upgrade_script.write(temp_shell)
-                        threading.Thread(
-                            target=tooldelta.safe_jump, kwargs={
-                                "exit_directly": True}
-                        ).start()
-                        upgrade_process = subprocess.Popen(
-                            (
-                                f"sh {upgrade_script_path}"
-                                if platform.system() == "Linux"
-                                else f"{upgrade_script_path}"
-                            ),
-                            cwd=os.getcwd(),
-                        )
-                        upgrade_process.communicate()
-
-            except Exception as err:
-                Print.print_war(
-                    f"在检测最新版本或更新ToolDelta至最新版本时出现异常，ToolDelta将会在下次启动时重新更新: {err}"
-                )
+    class SystemVersionException(ImportError):
+        """系统版本异常"""
+        msg: str
+
+    def __init__(self) -> None:
+        """初始化"""
+        self.ClassicThread = self.createThread = Builtins.createThread
+        self.sys_data = self.FrameBasic()
+        self.serverNumber: int = 0
+        self.serverPasswd: str = ""
+        self.launchMode: int = 0
+        self.consoleMenu = []
+        self.on_plugin_err = staticmethod(
+            lambda name, _, err: Print.print_err(f"插件 <{name}> 出现问题: \n{err}")
+        )
+        self.launcher: FrameFBConn | FrameNeOmg | FrameNeOmgRemote
+        self.is_mir: bool
+        self.plugin_market_url: str
+        self.link_game_ctrl: "GameCtrl"
+        self.link_plugin_group: "PluginGroup"
 
-    def read_cfg(self):
+    def loadConfiguration(self) -> None:
+        """加载配置文件"""
         Config.default_cfg("ToolDelta基本配置.json", constants.LAUNCH_CFG)
         try:
+            # 读取配置文件
             cfgs = Config.get_cfg("ToolDelta基本配置.json",
                                   constants.LAUNCH_CFG_STD)
-            self.serverNumber = str(cfgs["服务器号"])
+            self.serverNumber = cfgs["服务器号"]
             self.serverPasswd = cfgs["密码"]
             self.launchMode = cfgs["启动器启动模式(请不要手动更改此项, 改为0可重置)"]
             self.is_mir = cfgs["是否使用github镜像"]
             self.plugin_market_url = cfgs["插件市场源"]
             auth_server = cfgs["验证服务器地址(更换时记得更改fbtoken)"]
             publicLogger.switch_logger(cfgs["是否记录日志"])
-            if self.launchMode != 0 and self.launchMode not in range(
-                1, len(constants.LAUNCHERS) + 1
-            ):
-                raise Config.ConfigError(
-                    "你不该随意修改启动器模式, 现在赶紧把它改回0吧"
-                )
+            if self.launchMode != 0 and self.launchMode not in range(1, len(constants.LAUNCHERS) + 1):
+                raise Config.ConfigError("你不该随意修改启动器模式, 现在赶紧把它改回0吧")
         except Config.ConfigError as err:
+            # 配置文件有误
             r = self.upgrade_cfg()
             if r:
                 Print.print_war("配置文件未升级, 已自动升级, 请重启 ToolDelta")
             else:
                 Print.print_err(f"ToolDelta基本配置有误, 需要更正: {err}")
-            raise SystemExit
+            raise SystemExit from err
         if self.serverNumber == "0":
             while 1:
                 try:
-                    self.serverNumber = input(
+                    self.serverNumber = int(input(
                         Print.fmt_info("请输入租赁服号: ", "§b 输入 ")
-                    )
+                    ))
                     self.serverPasswd = (
                         getpass.getpass(
                             Print.fmt_info(
                                 "请输入租赁服密码(不会回显, 没有请直接回车): ", "§b 输入 "
                             )
                         )
                         or "0"
@@ -280,15 +130,15 @@
                     std = constants.LAUNCH_CFG.copy()
                     std["服务器号"] = int(self.serverNumber)
                     std["密码"] = int(self.serverPasswd)
                     Config.default_cfg("ToolDelta基本配置.json", std, True)
                     Print.print_suc("登录配置设置成功")
                     cfgs = std
                     break
-                except:
+                except Exception:
                     Print.print_err("输入有误， 租赁服号和密码应当是纯数字")
 
         auth_servers = constants.AUTH_SERVERS
         if auth_server == "":
             Print.print_inf("选择 ToolDelta机器人账号 使用的验证服务器:")
             for i, (auth_server_name, _) in enumerate(auth_servers):
                 Print.print_inf(f" {i + 1} - {auth_server_name}")
@@ -321,26 +171,28 @@
                 elif int(Login_method) > 2 or int(Login_method) < 1:
                     Login_method = input(
                         Print.fmt_info("输入有误, 请输入正确的序号: ", "§6 警告 ")
                     )
                 else:
                     break
             if Login_method == "1":
-                match cfgs["验证服务器地址(更换时记得更改fbtoken)"]:
-                    case "https://liliya233.uk":
-                        auths.login_liliya()
-                    case "https://api.fastbuilder.pro":
-                        auths.login_fbuc()
-                    case _:
-                        Print.print_err("暂无法登录该验证服务器")
-                        raise SystemExit
-            elif Login_method == "2":
-                self.if_token()
-            else:
-                self.if_token()
+                try:
+                    match cfgs["验证服务器地址(更换时记得更改fbtoken)"]:
+                        case "https://liliya233.uk":
+                            token = auths.liliya_login()
+                        case "https://api.fastbuilder.pro":
+                            token = auths.fbuc_login()
+                        case _:
+                            Print.print_err("暂无法登录该验证服务器")
+                            raise SystemExit
+                    with open("fbtoken", "w", encoding="utf-8") as f:
+                        f.write(token)
+                except requests.exceptions.RequestException as e:
+                    Print.print_err(f"登录失败，原因：{e}\n正在切换至Token登录")
+            if_token()
         launchers = constants.LAUNCHERS
         if self.launchMode == 0:
             Print.print_inf("请选择启动器启动模式(之后可在ToolDelta启动配置更改):")
             for i, (launcher_name, _) in enumerate(launchers):
                 Print.print_inf(f" {i + 1} - {launcher_name}")
             while 1:
                 try:
@@ -348,67 +200,75 @@
                     if ch not in range(1, len(launchers) + 1):
                         raise ValueError
                     cfgs["启动器启动模式(请不要手动更改此项, 改为0可重置)"] = ch
                     break
                 except ValueError:
                     Print.print_err("输入不合法, 或者是不在范围内, 请重新输入")
             Config.default_cfg("ToolDelta基本配置.json", cfgs, True)
-        launcher: Callable = launchers[
-            cfgs["启动器启动模式(请不要手动更改此项, 改为0可重置)"] - 1
-        ][1]
-        self.fbtokenFix()
+        # 修复fbtoken
+        fbtokenFix()
         with open("fbtoken", "r", encoding="utf-8") as f:
             fbtoken = f.read()
-        self.launcher: FrameFBConn | FrameNeOmg | FrameNeOmgRemote = launcher(
+        self.launcher = launchers[
+            cfgs["启动器启动模式(请不要手动更改此项, 改为0可重置)"] - 1
+        ][1](
             self.serverNumber,
             self.serverPasswd,
             fbtoken,
             auth_server,
         )
 
     @staticmethod
-    def upgrade_cfg():
-        # 升级本地的配置文件
+    def upgrade_cfg() -> bool:
+        """升级配置文件
+
+        Returns:
+            bool: 是否升级了配置文件
+        """
         old_cfg = Config.get_cfg("ToolDelta基本配置.json", {})
         old_cfg_keys = old_cfg.keys()
         need_upgrade_cfg = False
         for k, v in constants.LAUNCH_CFG.items():
             if k not in old_cfg_keys:
                 old_cfg[k] = v
                 need_upgrade_cfg = True
         if need_upgrade_cfg:
             Config.default_cfg("ToolDelta基本配置.json", old_cfg, True)
         return need_upgrade_cfg
 
-    def welcome(self):
-        # 欢迎提示
+    def welcome(self) -> None:
+        """欢迎提示"""
         Print.print_with_info(
-            f"§d{self.PRG_NAME} Panel Embed By SuperScript", Print.INFO_LOAD
+            f"§d{PRG_NAME} Panel Embed By SuperScript", Print.INFO_LOAD
         )
         Print.print_with_info(
-            f"§d{self.PRG_NAME} Wiki: https://tooldelta-wiki.tblstudio.cn/", Print.INFO_LOAD
+            f"§d{PRG_NAME} Wiki: https://tooldelta-wiki.tblstudio.cn/", Print.INFO_LOAD
         )
         Print.print_with_info(
-            f"§d{self.PRG_NAME} 项目地址: https://github.com/ToolDelta", Print.INFO_LOAD
+            f"§d{PRG_NAME} 项目地址: https://github.com/ToolDelta", Print.INFO_LOAD
         )
         Print.print_with_info(
-            f"§d{self.PRG_NAME} v {'.'.join([str(i) for i in VERSION])}", Print.INFO_LOAD
+            f"§d{PRG_NAME} v {'.'.join([str(i) for i in VERSION])}", Print.INFO_LOAD
         )
-        Print.print_with_info(f"§d{self.PRG_NAME} Panel 已启动", Print.INFO_LOAD)
+        Print.print_with_info(f"§d{PRG_NAME} Panel 已启动", Print.INFO_LOAD)
 
     @staticmethod
-    def plugin_load_finished(plugins: PluginGroup):
-        # 插件成功载入提示
+    def plugin_load_finished(plugins: "PluginGroup"):
+        """插件加载完成时的回调函数
+
+        Args:
+            plugins (PluginGroup): 插件组对象，包含已加载的插件信息
+        """
         Print.print_suc(
             f"成功载入 §f{plugins.normal_plugin_loaded_num}§a 个组合式插件, §f{plugins.injected_plugin_loaded_num}§a 个注入式插件"
         )
 
     @staticmethod
     def basic_operation():
-        # 初始化文件夹
+        """初始化文件夹"""
         if os.path.isdir("插件文件/ToolDelta组合式插件"):
             os.rename(
                 "插件文件/ToolDelta组合式插件",
                 f"插件文件/{constants.TOOLDELTA_CLASSIC_PLUGIN}",
             )
         os.makedirs(
             f"插件文件/{constants.TOOLDELTA_CLASSIC_PLUGIN}", exist_ok=True)
@@ -417,108 +277,112 @@
         os.makedirs("插件配置文件", exist_ok=True)
         os.makedirs("tooldelta/fb_conn", exist_ok=True)
         os.makedirs("tooldelta/neo_libs", exist_ok=True)
         os.makedirs("插件数据文件/status", exist_ok=True)
         os.makedirs("插件数据文件/players", exist_ok=True)
         os.makedirs("插件数据文件/game_texts", exist_ok=True)
 
-    @staticmethod
-    def fbtokenFix():
-        # 对异常FbToken的自动修复
-        with open("fbtoken", "r", encoding="utf-8") as f:
-            token = f.read()
-            if "\n" in token:
-                Print.print_war("fbtoken里有换行符， 会造成fb登陆失败， 已自动修复")
-                with open("fbtoken", "w", encoding="utf-8") as f:
-                    f.write(token.replace("\n", ""))
-
     def add_console_cmd_trigger(
         self,
         triggers: list[str],
         arg_hint: str | None,
         usage: str,
         func: Callable[[list[str]], None],
-    ):
-        """
-        注册ToolDelta控制台的菜单项
+    ) -> None:
+        """注册ToolDelta控制台的菜单项
 
-        参数:
-            triggers: 触发词列表
-            arg_hint: 菜单命令参数提示句
-            usage: 命令说明
-            func: 菜单回调方法 (list[str])
+        Args:
+            triggers (list[str]): 触发词列表
+            arg_hint (str | None): 菜单命令参数提示句
+            usage (str): 命令说明
+            func (Callable[[list[str]], None]): 菜单回调方法
         """
         try:
             if self.consoleMenu.index(triggers) != -1:
                 Print.print_war(f"§6后台指令关键词冲突: {func}, 不予添加至指令菜单")
-        except:
+        except Exception:
             self.consoleMenu.append([usage, arg_hint, func, triggers])
 
-    def init_basic_help_menu(self, _):
+    def init_basic_help_menu(self, _) -> None:
+        """初始化基本的帮助菜单"""
         menu = self.get_console_menus()
         Print.print_inf("§a以下是可选的菜单指令项: ")
         for usage, arg_hint, _, triggers in menu:
             if arg_hint:
                 Print.print_inf(
                     f" §e{' 或 '.join(triggers)} §b{arg_hint} §f->  {usage}")
             else:
                 Print.print_inf(f" §e{' 或 '.join(triggers)}  §f->  {usage}")
 
-    def comsole_cmd_start(self):
+    def comsole_cmd_start(self) -> None:
+        """启动控制台命令"""
         def _try_execute_console_cmd(func, rsp, mode, arg1):
             try:
                 if mode == 0:
                     rsp_arg = rsp.split()[1:]
                 elif mode == 1:
                     rsp_arg = rsp[len(arg1):].split()
             except IndexError:
                 Print.print_err("[控制台执行命令] 指令缺少参数")
                 return
             try:
                 return func(rsp_arg) or 0
-            except:
+            except Exception:
                 Print.print_err(f"控制台指令出错： {traceback.format_exc()}")
                 return 0
 
         @Builtins.thread_func
-        def _execute_mc_command_and_get_callback(cmd: str):
+        def _execute_mc_command_and_get_callback(cmd: str) -> None:
+            """执行Minecraft指令并获取回调结果。
+
+            Args:
+                cmd (str): 要执行的Minecraft指令。
+
+            Raises:
+                ValueError: 当指令执行失败时抛出。
+            """
             cmd = " ".join(cmd)
             try:
                 result = self.link_game_ctrl.sendcmd(cmd, True, 10)
+                if isinstance(result, type(None)):
+                    raise ValueError("指令执行失败")
                 if (result.OutputMessages[0].Message == "commands.generic.syntax") | (
                     result.OutputMessages[0].Message == "commands.generic.unknown"
                 ):
                     Print.print_err(f'未知的MC指令， 可能是指令格式有误： "{cmd}"')
                 else:
                     jso = json.dumps(
                         result.as_dict["OutputMessages"], indent=2, ensure_ascii=False
                     )
                     if not result.SuccessCount:
                         Print.print_war(f"指令执行失败: \n{jso}")
                     else:
                         Print.print_suc(f"指令执行成功: \n{jso}")
-            except IndexError:
+            except IndexError as exec_err:
+                if isinstance(result, type(None)):
+                    raise ValueError("指令执行失败") from exec_err
                 if result.SuccessCount:
                     Print.print_suc(
                         f"指令执行成功: \n{json.dumps(result.as_dict['OutputMessages'], indent=2, ensure_ascii=False)}"
                     )
             except TimeoutError:
                 Print.print_err("[超时] 指令获取结果返回超时")
 
-        def _console_cmd_thread():
+        def _console_cmd_thread() -> None:
+            """控制台线程"""
             self.add_console_cmd_trigger(
                 ["?", "help", "帮助"],
                 None,
                 "查询可用菜单指令",
                 self.init_basic_help_menu,
             )
             self.add_console_cmd_trigger(
                 ["exit"],
                 None,
-                f"退出并关闭{self.PRG_NAME}",
+                f"退出并关闭{PRG_NAME}",
                 lambda _: tooldelta.safe_jump(out_task=True),
             )
             self.add_console_cmd_trigger(
                 ["插件市场"],
                 None,
                 "进入插件市场",
                 lambda _: plugin_market.market.enter_plugin_market(
@@ -543,15 +407,16 @@
                 rsp = ""
                 while True:
                     res = sys.stdin.read(1)
                     if res == "\n":  # 如果是换行符，则输出当前输入并清空输入
                         break
                     if res in ("", "^C", "^D"):
                         Print.print_inf("按退出键退出中...")
-                        self.launcher.status = SysStatus.NORMAL_EXIT
+                        if isinstance(self.launcher, (FrameNeOmgRemote, FrameNeOmg, FrameFBConn)):
+                            self.launcher.status = SysStatus.NORMAL_EXIT
                         self.system_exit()
                         return
                     rsp += res
                 for _, _, func, triggers in self.consoleMenu:
                     if not rsp:
                         continue
                     if rsp.split()[0] in triggers:
@@ -564,103 +429,147 @@
                                 res = _try_execute_console_cmd(
                                     func, rsp, 1, tri)
                                 if res == -1:
                                     return
 
         self.createThread(_console_cmd_thread, usage="控制台指令")
 
-    def system_exit(self):
+    def system_exit(self) -> None:
+        """系统退出"""
         asyncio.run(safe_jump())
         exit_status_code = getattr(self.launcher, "secret_exit_key", "null")
         if self.link_game_ctrl.allplayers and not isinstance(
             self.launcher, (FrameNeOmgRemote,)
         ):
             try:
                 self.link_game_ctrl.sendwscmd(
                     f"/kick {self.link_game_ctrl.bot_name} ToolDelta 退出中(看到这条消息请重新加入游戏)\nSTATUS CODE: {exit_status_code}"
                 )
-            except:
+            except Exception:
                 pass
         time.sleep(0.5)
-        self.launcher.exit_event.set()
+        if isinstance(self.launcher, (FrameNeOmgRemote, FrameNeOmg, FrameFBConn)):
+            self.launcher.exit_event.set()
+
+    def get_console_menus(self) -> list:
+        """获取控制台命令列表
 
-    def get_console_menus(self):
-        # 获取所有控制台命令菜单
+        Returns:
+            list: 命令列表
+        """
         return self.consoleMenu
 
-    def set_game_control(self, game_ctrl):
-        "使用外源GameControl..."
-        self.link_game_ctrl: GameCtrl = game_ctrl
-
-    def set_plugin_group(self, plug_grp):
-        "使用外源PluginGroup..."
-        self.link_plugin_group: PluginGroup = plug_grp
+    def set_game_control(self, game_ctrl) -> None:
+        """使用外源GameControl
+
+        Args:
+            game_ctrl (_type_): GameControl对象
+        """
+        self.link_game_ctrl: "GameCtrl" = game_ctrl
+
+    def set_plugin_group(self, plug_grp) -> None:
+        """使用外源PluginGroup
+
+        Args:
+            plug_grp (_type_): PluginGroup对象
+        """
+        self.link_plugin_group: "PluginGroup" = plug_grp
+
+    def get_game_control(self) -> "GameCtrl":
+        """获取GameControl对象
 
-    def get_game_control(self):
-        gcl: GameCtrl = self.link_game_ctrl
+        Returns:
+            GameCtrl: GameControl对象
+        """
+        gcl: "GameCtrl" = self.link_game_ctrl
         return gcl
 
     @staticmethod
-    def safe_close():
-        builtins.safe_close()
+    def safelyExit() -> None:
+        """安全退出"""
+        safe_close()
         publicLogger.exit()
         Print.print_inf("已保存数据与日志等信息.")
 
 
 class GameCtrl:
-    # 游戏连接和交互部分
-    def __init__(self, frame: Frame):
+    """游戏连接和交互部分"""
+
+    def __init__(self, frame: "Frame"):
+        """初始化
+
+        Args:
+            frame (Frame): 继承Frame的对象
+        """
         frame.basic_operation()
         self.Game_Data = GameTextsLoader().game_texts_data
         self.linked_frame = frame
         self.players_uuid = {}
         self.allplayers = []
         self.bot_name = ""
         self.linked_frame: Frame
         self.pkt_unique_id: int = 0
         self.pkt_cache: list = []
         self.require_listen_packets = {9, 79, 63}
         self.store_uuid_pkt: dict[str, str] | None = None
-
-    def init_funcs(self):
         self.launcher = self.linked_frame.launcher
-        self.launcher.packet_handler = lambda pckType, pck: createThread(
-            self.packet_handler, (pckType, pck)
-        )
+        if isinstance(self.launcher, (FrameNeOmgRemote, FrameNeOmg, FrameFBConn)):
+            self.launcher.packet_handler = lambda pckType, pck: Builtins.createThread(
+                self.packet_handler, (pckType, pck), usage="数据包处理")
         self.sendcmd = self.launcher.sendcmd
         self.sendwscmd = self.launcher.sendwscmd
         self.sendwocmd = self.launcher.sendwocmd
         self.sendPacket = self.launcher.sendPacket
         self.sendfbcmd = self.launcher.sendfbcmd
         if isinstance(self.linked_frame.launcher, FrameNeOmg):
             self.requireUUIDPacket = False
         else:
             self.requireUUIDPacket = True
 
-    def set_listen_packets(self):
-        # 向启动器初始化监听的游戏数据包
-        # 不应该再次调用此方法
+    def set_listen_packets(self) -> None:
+        """
+        向启动器初始化监听的游戏数据包
+
+        不应该再次调用此方法
+        """
         for pktID in self.require_listen_packets:
             self.launcher.add_listen_packets(pktID)
 
-    def add_listen_pkt(self, pkt: int):
+    def add_listen_pkt(self, pkt: int) -> None:
+        """添加监听的数据包
+
+        Args:
+            pkt (int): 数据包ID
+        """
         self.require_listen_packets.add(pkt)
 
     @Builtins.run_as_new_thread
-    def packet_handler(self, pkt_type: int, pkt: dict):
+    def packet_handler(self, pkt_type: int, pkt: dict) -> None:
+        """数据包处理分发任务函数
+
+        Args:
+            pkt_type (int): 数据包类型
+            pkt (dict): 数据包内容
+        """
         is_skiped = self.linked_frame.link_plugin_group.processPacketFunc(
             pkt_type, pkt)
         if is_skiped:
             return
         if pkt_type == PacketIDS.PlayerList:
             self.process_player_list(pkt, self.linked_frame.link_plugin_group)
         elif pkt_type == PacketIDS.Text:
             self.process_text_packet(pkt, self.linked_frame.link_plugin_group)
 
-    def process_player_list(self, pkt, plugin_group: PluginGroup):
+    def process_player_list(self, pkt, plugin_group: "PluginGroup") -> None:
+        """处理玩家列表等数据包
+
+        Args:
+            pkt (_type_): 数据包内容
+            plugin_group (PluginGroup): 插件组对象
+        """
         # 处理玩家进出事件
         res = self.launcher.get_players_and_uuids()
         if res:
             self.allplayers = list(res.keys())
             self.players_uuid.update(res)
         for player in pkt["Entries"]:
             isJoining = bool(player["Skin"]["SkinData"])
@@ -687,16 +596,21 @@
                     self.allplayers.remove(playername)
                 Print.print_inf(f"§e{playername} 退出了游戏")
                 plugin_group.execute_player_leave(
                     playername, self.linked_frame.on_plugin_err
                 )
                 asyncio.run(execute_player_left(playername))
 
-    def process_text_packet(self, pkt: dict, plugin_grp: PluginGroup):
-        # 处理9号数据包的消息, 因特殊原因将一些插件事件放到此处理
+    def process_text_packet(self, pkt: dict, plugin_grp: "PluginGroup") -> None:
+        """处理9号数据包的消息
+
+        Args:
+            pkt (dict): 数据包内容
+            plugin_grp (PluginGroup): 插件组对象
+        """
         match pkt["TextType"]:
             case 2:
                 if pkt["Message"] == "§e%multiplayer.player.joined":
                     player = pkt["Parameters"][0]
                     plugin_grp.execute_player_prejoin(
                         player, self.linked_frame.on_plugin_err
                     )
@@ -744,33 +658,35 @@
                 asyncio.run(execute_player_message(player, msg))
             case 9:
                 msg = pkt["Message"]
                 try:
                     msg_text = json.loads(msg)["rawtext"]
                     msg_text = "".join([i["text"] for i in msg_text])
                     Print.print_inf(msg_text)
-                except:
+                except Exception:
                     pass
 
-    def Inject(self):
-        # 载入游戏时的初始化
+    def Inject(self) -> None:
+        """载入游戏时的初始化"""
         res = self.launcher.get_players_and_uuids()
         if res:
             self.allplayers = list(res.keys())
             self.players_uuid.update(res)
         else:
             while 1:
                 try:
-                    self.allplayers = (
-                        self.sendwscmd("/list", True)
-                        .OutputMessages[1]
-                        .Parameters[0]
-                        .split(", ")
-                    )
-                    break
+                    cmd_result = self.sendwscmd("/list", True)
+                    if cmd_result:
+                        self.allplayers = (
+                            cmd_result
+                            .OutputMessages[1]
+                            .Parameters[0]
+                            .split(", ")
+                        )
+                        break
                 except TimeoutError:
                     Print.print_war("获取全局玩家失败..重试")
         self.bot_name = self.launcher.get_bot_name()
         if self.bot_name is None:
             self.bot_name = self.allplayers[0]
         self.linked_frame.comsole_cmd_start()
         self.linked_frame.link_plugin_group.execute_init(
@@ -778,66 +694,66 @@
         )
         Builtins.createThread(asyncio.run, (execute_repeat(),))
         Print.print_inf("正在执行初始化注入式函数init任务")
         asyncio.run(execute_init())
         Print.print_suc("初始化注入式函数init任务执行完毕")
         self.inject_welcome()
 
-    def inject_welcome(self):
-        # 载入游戏后的欢迎提示语
-        Print.print_suc(
-            "初始化完成, 在线玩家: "
-            + ", ".join(self.allplayers)
-            + ", 机器人ID: "
-            + self.bot_name
-        )
+    def inject_welcome(self) -> None:
+        """初始化欢迎信息"""
+
+        if isinstance(self.bot_name, str):
+            Print.print_suc(
+                "初始化完成, 在线玩家: "
+                + ", ".join(self.allplayers)
+                + ", 机器人ID: "+self.bot_name
+            )
+        else:
+            Print.print_suc("初始化完成, 在线玩家: " + ", ".join(self.allplayers))
+            Print.print_war("未能获取机器人ID")
         self.sendcmd("/tag @s add robot")
         Print.print_suc("§f在控制台输入 §ahelp / ?§f可查看控制台命令")
 
-    def say_to(self, target: str, msg: str):
-        """
-        向玩家发送聊天栏信息
+    def say_to(self, target: str, msg: str) -> None:
+        """向玩家发送消息
 
-        参数:
-            target: 玩家名/目标选择器
-            msg: 信息
+        Args:
+            target (str): 玩家名/目标选择器
+            msg (str): 消息
         """
         self.sendwocmd("tellraw " + target +
                        ' {"rawtext":[{"text":"' + msg + '"}]}')
 
-    def player_title(self, target: str, text: str):
-        """
-        向玩家展示大标题文本
+    def player_title(self, target: str, text: str) -> None:
+        """向玩家展示标题文本
 
-        参数:
-            target: 玩家名/目标选择器
-            text: 文本
+        Args:
+            target (str): 玩家名/目标选择器
+            text (str): 文本
         """
         self.sendwocmd(f"title {target} title {text}")
 
-    def player_subtitle(self, target: str, text: str):
-        """
-        向玩家展示小标题文本
+    def player_subtitle(self, target: str, text: str) -> None:
+        """向玩家展示副标题文本
 
-        参数:
-            target: 玩家名/目标选择器
-            text: 文本
+        Args:
+            target (str): 玩家名/目标选择器
+            text (str): 文本
         """
         self.sendwocmd(f"title {target} subtitle {text}")
 
-    def player_actionbar(self, target: str, text: str):
-        """
-        向玩家展示行动栏文本
+    def player_actionbar(self, target: str, text: str) ->None:
+        """向玩家展示动作栏文本
 
-        参数:
-            target: 玩家名/目标选择器
-            text: 文本
+        Args:
+            target (str): 玩家名/目标选择器
+            text (str): 文本
         """
         self.sendwocmd(f"title {target} actionbar {text}")
 
-    def get_game_data(self):
-        """
-        获取minecraft信息数据
+    def get_game_data(self) -> dict:
+        """获取游戏数据
 
-        返回类型: dict
+        Returns:
+            dict: 游戏数据
         """
         return self.Game_Data
```

### Comparing `tooldelta-0.5.3/tooldelta/game_texts.py` & `tooldelta-0.5.4/tooldelta/game_texts.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.3/tooldelta/launch_cli.py` & `tooldelta-0.5.4/tooldelta/launch_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,80 +1,85 @@
-from hmac import new
-import platform
+"""客户端启动器框架"""
+
 import os
-from poplib import CR
+import threading
 import shlex
-import subprocess
 import uuid
 import time
 import json
-import ssl
+import random
+import subprocess
+import platform
+from typing import Callable, Optional
 import requests
 import ujson
-import random
 
-from tooldelta import (
-    constants,
-)
-from typing import Callable, Optional
-from .color_print import Print
-from .urlmethod import download_file_singlethreaded, get_free_port
+import tooldelta
+from tooldelta import constants
+from .cfg import Cfg
+from .fb_conn import fbconn
 from .builtins import Builtins
+from .color_print import Print
 from .basic_mods import socketio
-from .packets import Packet_CommandOutput, PacketIDS
 from .sys_args import sys_args_to_dict
-from tooldelta.cfg import Cfg
-from .fb_conn import fbconn
-import threading
-import tooldelta
+from .packets import Packet_CommandOutput, PacketIDS
+from .urlmethod import download_file_singlethreaded, get_free_port
+
 Config = Cfg()
 
 
 class SysStatus:
+    """系统状态码
+
+    LOADING: 启动器正在加载
+    LAUNCHING: 启动器正在启动
+    RUNNING: 启动器正在运行
+    NORMAL_EXIT: 正常退出
+    FB_LAUNCH_EXC: FastBuilder 启动异常
+    CRASHED_EXIT: 启动器崩溃退出
+    NEED_RESTART: 需要重启
+    """
     LOADING = 100
     LAUNCHING = 101
     RUNNING = 102
     NORMAL_EXIT = 103
     FB_LAUNCH_EXC = 104
     CRASHED_EXIT = 105
     NEED_RESTART = 106
     launch_type = "None"
 
 
 class StandardFrame:
-    # 提供了标准的启动器框架, 作为 ToolDelta 和游戏交互的接口
+    """提供了标准的启动器框架, 作为 ToolDelta 和游戏交互的接口"""
     launch_type = "Original"
 
     def __init__(self, serverNumber, password, fbToken, auth_server_url):
         self.serverNumber = serverNumber
         self.serverPassword = password
         self.fbToken = fbToken
         self.auth_server = auth_server_url
-        self.status = SysStatus.LOADING
         self.system_type = platform.uname().system
         self.inject_events = []
         self.packet_handler: Callable | None = lambda pckType, pck: None
         self.need_listen_packets = {9, 63, 79}
         self._launcher_listener = None
         self.exit_event = threading.Event()
+        self.status = SysStatus.LOADING
 
     def add_listen_packets(self, *pcks: int):
         for i in pcks:
             self.need_listen_packets.add(i)
 
     @staticmethod
     def launch():
         raise Exception("Cannot launch this launcher")
 
     def listen_launched(self, cb):
         self._launcher_listener = cb
 
-    def close_fb(self):
-        raise NotImplementedError()
-
     @staticmethod
     def get_players_and_uuids():
         return None
 
     @staticmethod
     def get_bot_name():
         return None
@@ -85,21 +90,42 @@
             tooldelta.safe_jump(out_task=True)
             self.exit_event.set()  # 设置事件，触发等待结束
         if new_status == SysStatus.CRASHED_EXIT:
             tooldelta.safe_jump(out_task=False)
             self.exit_event.set()
 
     get_all_players = None
-    sendcmd: Callable[[str, bool, int | float], None | Packet_CommandOutput]
-    sendwscmd: Callable[[str, bool, int | float], Packet_CommandOutput]
-    sendwocmd: Callable[[str], None]
-    sendfbcmd: Callable[[str], None | AttributeError]
-    sendPacket: Callable[[int, str], None]
-    sendPacketJson: Callable[[int, str], None]
-    is_op: Callable[[str], None | bool] | None
+
+    @staticmethod
+    def sendcmd(cmd: str, waitForResp: bool = False, timeout: int | float = 30) -> Optional[Packet_CommandOutput]:
+        ...
+
+    @staticmethod
+    def sendwscmd(cmd: str, waitForResp: bool = False, timeout: int | float = 30) -> Optional[Packet_CommandOutput]:
+        ...
+
+    @staticmethod
+    def sendwocmd(cmd: str) -> None:
+        ...
+
+    @staticmethod
+    def sendfbcmd(cmd: str) -> None:
+        ...
+
+    @staticmethod
+    def sendPacket(pckID: int, pck: str) -> None:
+        ...
+
+    @staticmethod
+    def sendPacketJson(pckID: int, pck: str) -> None:
+        ...
+
+    @staticmethod
+    def is_op(player: str) -> bool:
+        ...
 
 
 class FrameFBConn(StandardFrame):
     # 使用原生 FastBuilder External 连接
     cmds_reqs = []
     cmds_resp = {}
 
@@ -250,15 +276,15 @@
         except StopIteration:
             pass
         self.update_status(SysStatus.CRASHED_EXIT)
 
     def downloadMissingFiles(self):
         "获取缺失文件"
         Print.print_with_info("§d将自动检测缺失文件并补全", "§d 加载 ")
-        mirror_src = "https://gh.api.99988866.xyz/"
+        mirror_src = "https://tdload.tblstudio.cn/"
         file_get_src = (
             mirror_src
             + "https://raw.githubusercontent.com/ToolDelta/ToolDelta/main/require_files.json"
         )
         try:
             files_to_get = json.loads(
                 requests.get(file_get_src, timeout=30).text)
@@ -358,14 +384,15 @@
     def __init__(self, serverNumber, password, fbToken, auth_server):
         super().__init__(serverNumber, password, fbToken, auth_server)
         self.status = None
         self.launch_event = threading.Event()
         self.injected = False
         self.omega = None
         self.TDC = None
+        self.neomg_proc = None
         self.set_tooldelta_cli()
         self.download_libs()
         self.init_all_functions()
         self.status = SysStatus.LOADING
         self.secret_exit_key = ""
 
     def set_omega(self, openat_port):
@@ -414,15 +441,15 @@
             os.system("chmod +x " + shlex.quote(py_file_path))
         # 只需要+x即可
         Print.print_inf(f"DEBUG: 将使用端口 {free_port}")
         self.neomg_proc = subprocess.Popen(
             [
                 py_file_path,
                 "-server",
-                self.serverNumber,
+                str(self.serverNumber),
                 "-T",
                 self.fbToken,
                 "-access-point-addr",
                 f"tcp://localhost:{free_port}",
                 "-server-password",
                 str(self.serverPassword),
                 "-auth-server",
@@ -482,17 +509,17 @@
         return SystemError("未知的退出状态")
 
     def download_libs(self):
         """根据系统架构和平台下载所需的库。"""
         cfgs = Config.get_cfg("ToolDelta基本配置.json", constants.LAUNCH_CFG_STD)
         is_mir: bool = cfgs["是否使用github镜像"]
         if is_mir:
-            mirror_src = "https://gh.api.99988866.xyz/" + \
+            mirror_src = "https://tdload.tblstudio.cn/" + \
                 "https://raw.githubusercontent.com/ToolDelta/ToolDelta/main/"
-            depen_url = "https://gh.api.99988866.xyz/" + \
+            depen_url = "https://tdload.tblstudio.cn/" + \
                 "https://raw.githubusercontent.com/ToolDelta/DependencyLibrary/main/"
         else:
             mirror_src = "https://raw.githubusercontent.com/ToolDelta/ToolDelta/main/"
             depen_url = "https://raw.githubusercontent.com/ToolDelta/DependencyLibrary/main/"
         try:
             require_depen = json.loads(
                 requests.get(
@@ -595,14 +622,17 @@
         self.sendwocmd = sendwocmd
         self.sendPacket = self.sendPacketJson = sendPacket
         self.sendfbcmd = sendfbcmd
         self.is_op = is_op
 
 
 class FrameNeOmgRemote(FrameNeOmg):
+    def __init__(self, serverNumber, password, fbToken, auth_server):
+        super().__init__(serverNumber, password, fbToken, auth_server)
+
     def launch(self):
         try:
             openat_port = int(sys_args_to_dict().get(
                 "access-point-port", "24020"))
             if openat_port not in range(65536):
                 raise AssertionError
         except (ValueError, AssertionError):
```

### Comparing `tooldelta-0.5.3/tooldelta/launch_options.py` & `tooldelta-0.5.4/tooldelta/launch_options.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.3/tooldelta/logger.py` & `tooldelta-0.5.4/tooldelta/logger.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.3/tooldelta/neo_libs/neo_conn.py` & `tooldelta-0.5.4/tooldelta/neo_libs/neo_conn.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import traceback
 import threading
 import enum
 from typing import Iterable, Tuple, Optional, Union, Any, Callable, List, Dict
 from threading import Thread
 from dataclasses import dataclass
 from tooldelta.color_print import Print
+from tooldelta.packets import Packet_CommandOutput
 
 CInt = ctypes.c_longlong
 CString = ctypes.c_char_p
 CBytes = ctypes.POINTER(ctypes.c_char)
 
 
 class byteCSlice(ctypes.Structure):
@@ -757,15 +758,15 @@
         SendWebSocketCommandNeedResponse(cmd, retriever_id)
         res = getter(timeout=timeout)
         del self._omega_cmd_callback_events[retriever_id]
         return res
 
     def send_player_command_need_response(
         self, cmd: str, timeout: int = -1
-    ) -> Optional[CommandOutput]:
+    ) -> Optional[Packet_CommandOutput]:
         setter, getter = self._create_lock_and_result_setter()
         try:
             retriever_id = next(self._cmd_callback_retriever_counter)
         except StopIteration:
             raise ValueError("retriever counter overflow")
         self._omega_cmd_callback_events[retriever_id] = setter
         SendPlayerCommandNeedResponse(cmd, retriever_id)
```

### Comparing `tooldelta-0.5.3/tooldelta/packets.py` & `tooldelta-0.5.4/tooldelta/packets.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.3/tooldelta/plugin_load/PluginGroup.py` & `tooldelta-0.5.4/tooldelta/plugin_load/PluginGroup.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.3/tooldelta/plugin_load/__init__.py` & `tooldelta-0.5.4/tooldelta/plugin_load/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         self.name: str = name
         if isinstance(plugin_data.get("version"), str):
             self.version: tuple = tuple(
                 int(i) for i in plugin_data.get("version", "0.0.0").split(".")
             )
         else:
             self.version = plugin_data.get("version", (0, 0, 0))
+        #  以下的方法或许存在危险
         self.author: str = plugin_data.get("author", "unknown")
         self.plugin_type: str = plugin_data.get("plugin-type", "unknown")
         self.description: str = plugin_data.get("description", "")
         self.pre_plugins: dict[str, str] = plugin_data.get("pre-plugins", [])
         self.plugin_id = plugin_data.get("plugin-id", "???")
         self.is_registered = is_registered
         if plugin_data.get("enabled") is not None:
```

### Comparing `tooldelta-0.5.3/tooldelta/plugin_load/classic_plugin/__init__.py` & `tooldelta-0.5.4/tooldelta/plugin_load/classic_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.3/tooldelta/plugin_load/injected_plugin/__init__.py` & `tooldelta-0.5.4/tooldelta/plugin_load/injected_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.3/tooldelta/plugin_load/injected_plugin/movent.py` & `tooldelta-0.5.4/tooldelta/plugin_load/injected_plugin/movent.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.3/tooldelta/plugin_manager.py` & `tooldelta-0.5.4/tooldelta/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.3/tooldelta/plugin_market.py` & `tooldelta-0.5.4/tooldelta/plugin_market.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,14 +206,16 @@
         self.plugin_id_name_map = res1
         return res1
 
     def download_plugin(
         self,
         plugin_data: PluginRegData
     ):
+        if self.plugin_id_name_map is None:
+            self.plugin_id_name_map = self.get_plugin_id_name_map()
         pres = [plugin_data]
         download_paths = self.find_dirs(plugin_data)
         for plugin_id in plugin_data.pre_plugins:
             plugin_name = self.plugin_id_name_map[plugin_id]
             Print.clean_print(f"正在下载 {plugin_data.name} 的前置插件 {plugin_name}")
             plugin_datas = self.get_plugin_data_from_market(plugin_id)
             pres += self.download_plugin(plugin_datas)
```

### Comparing `tooldelta-0.5.3/tooldelta/starter.py` & `tooldelta-0.5.4/tooldelta/starter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,52 @@
 import signal
 import time
-from tooldelta import builtins
+from tooldelta import builtins, urlmethod
 from tooldelta.frame import Frame
 from tooldelta.frame import GameCtrl
-from tooldelta.basic_mods import os, traceback, threading
+from tooldelta.basic_mods import os, traceback
 from tooldelta.color_print import Print
 from tooldelta.plugin_load.PluginGroup import plugin_group
 from tooldelta.plugin_load.injected_plugin import movent
 
 frame = Frame()
-game_control = GameCtrl(frame)
 def signal_handler(*arg):
     # 排除信号中断
     pass
 signal.signal(signal.SIGINT, signal_handler)
 
 def start_tool_delta():
     # 初始化系统
     plugin_group.set_frame(frame)
     try:
         frame.welcome()
+        urlmethod.check_update()
         frame.basic_operation()
+        frame.loadConfiguration()
+        game_control = GameCtrl(frame)
         frame.set_game_control(game_control)
         frame.set_plugin_group(plugin_group)
         movent.set_frame(frame)
-        frame.read_cfg()
-        game_control.init_funcs()
         plugin_group.read_all_plugins()
         frame.plugin_load_finished(plugin_group)
         builtins.tmpjson_save_thread()
         frame.launcher.listen_launched(game_control.Inject)
         game_control.set_listen_packets()
         # TODO: 自动更新需要时间间隔
-        builtins.Builtins.createThread(frame.ToolDeltaUpdater, usage="自动更新 ToolDelta", launcher = frame.launcher)
         raise frame.launcher.launch()
     except (KeyboardInterrupt, SystemExit):
         pass
     except:
         Print.print_err("ToolDelta 运行过程中出现问题: " + traceback.format_exc())
 
 
 def safe_jump(*, out_task=True, exit_directly=True):
     if out_task:
         frame.system_exit()
-    frame.safe_close()
+    frame.safelyExit()
     if exit_directly:
         for _ in range(2, 0, -1):
             Print.print_war(f"{_}秒后强制退出...", end="\r")
             time.sleep(1)
         Print.print_war("0秒后强制退出...", end="\r")
         Print.print_suc("ToolDelta 已退出.")
         os._exit(0)
```

### Comparing `tooldelta-0.5.3/tooldelta/sys_args.py` & `tooldelta-0.5.4/tooldelta/sys_args.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.3/PKG-INFO` & `tooldelta-0.5.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: Tooldelta
-Version: 0.5.3
+Version: 0.5.4
 Summary: Plugin Loader for NeteaseRentalServer on Panel
 Home-page: https://github.com/SuperScript-PRC/ToolDelta
 Author: SuperScript-PRC
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: flask (>=3.0.2,<4.0.0)
+Requires-Dist: mido (>=1.3.2,<2.0.0)
 Requires-Dist: nbt (==1.5.1)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Requires-Dist: psutil (==5.9.8)
 Requires-Dist: pymysql (==1.1.0)
 Requires-Dist: pyspeedtest (==1.2.7)
 Requires-Dist: python-socketio (==5.11.1)
 Requires-Dist: qrcode (==7.4.2)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: rich (==13.7.0)
 Requires-Dist: shellescape (>=3.8.1,<4.0.0)
 Requires-Dist: tqdm (==4.66.2)
 Requires-Dist: ujson (==5.9.0)
+Requires-Dist: websocket-client (>=1.7.0,<2.0.0)
 Requires-Dist: websockets (==12.0)
 Project-URL: Repository, https://github.com/SuperScript-PRC/ToolDelta
 Description-Content-Type: text/markdown
 
 <h1 align="center">ToolDelta - Multi Platform Edition</h1>
 <p align="center">
   <a href="https://github.com/ToolDelta/ToolDelta/releases"><img src="https://img.shields.io/github/v/release/ToolDelta/ToolDelta?display_name=tag&sort=semver" alt="Releases"></a>
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: Tooldelta Version: 0.5.3 Summary: Plugin Loader for
+Metadata-Version: 2.1 Name: Tooldelta Version: 0.5.4 Summary: Plugin Loader for
 NeteaseRentalServer on Panel Home-page: https://github.com/SuperScript-PRC/
 ToolDelta Author: SuperScript-PRC Requires-Python: >=3.9,<3.13 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: aiohttp (>=3.9.3,<4.0.0) Requires-Dist: colorama
-(>=0.4.6,<0.5.0) Requires-Dist: flask (>=3.0.2,<4.0.0) Requires-Dist: nbt
-(==1.5.1) Requires-Dist: pillow (>=10.2.0,<11.0.0) Requires-Dist: psutil
-(==5.9.8) Requires-Dist: pymysql (==1.1.0) Requires-Dist: pyspeedtest (==1.2.7)
-Requires-Dist: python-socketio (==5.11.1) Requires-Dist: qrcode (==7.4.2)
-Requires-Dist: requests (==2.31.0) Requires-Dist: rich (==13.7.0) Requires-
-Dist: shellescape (>=3.8.1,<4.0.0) Requires-Dist: tqdm (==4.66.2) Requires-
-Dist: ujson (==5.9.0) Requires-Dist: websockets (==12.0) Project-URL:
-Repository, https://github.com/SuperScript-PRC/ToolDelta Description-Content-
-Type: text/markdown
+(>=0.4.6,<0.5.0) Requires-Dist: flask (>=3.0.2,<4.0.0) Requires-Dist: mido
+(>=1.3.2,<2.0.0) Requires-Dist: nbt (==1.5.1) Requires-Dist: pillow
+(>=10.2.0,<11.0.0) Requires-Dist: psutil (==5.9.8) Requires-Dist: pymysql
+(==1.1.0) Requires-Dist: pyspeedtest (==1.2.7) Requires-Dist: python-socketio
+(==5.11.1) Requires-Dist: qrcode (==7.4.2) Requires-Dist: requests (==2.31.0)
+Requires-Dist: rich (==13.7.0) Requires-Dist: shellescape (>=3.8.1,<4.0.0)
+Requires-Dist: tqdm (==4.66.2) Requires-Dist: ujson (==5.9.0) Requires-Dist:
+websocket-client (>=1.7.0,<2.0.0) Requires-Dist: websockets (==12.0) Project-
+URL: Repository, https://github.com/SuperScript-PRC/ToolDelta Description-
+Content-Type: text/markdown
                ************ TToooollDDeellttaa -- MMuullttii PPllaattffoorrmm EEddiittiioonn ************
                                _[_R_e_l_e_a_s_e_s_][Stars]
                        _[_o_p_i_s_s_u_e_s_]_[_c_l_i_s_s_u_e_s_]_[_o_p_p_r_]_[_c_l_p_r_]
                TToooollDDeellttaa æ¯ä¾èµäº PPhhooeenniixxBBuuiillddeerr || NNeeoo OOmmeeggaa
     çå¤åè½æ©å±ç»ä»¶ï¼å¯ä»¥å è½½åç§åæ ·æè¶£çæä»¶ã
   TToooollDDeellttaa å¯ä»¥ä½¿å¾ä½ ç ?ä?¸?­?å??½?ç???ã???æ???ç???ä?¸??ç???ã???å??º?å?²?©?ç???ç?§??è?µ??æ??
                      çç©æ³ååè½æ´å å¤æ ·åã
```

