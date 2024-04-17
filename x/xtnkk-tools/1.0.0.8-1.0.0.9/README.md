# Comparing `tmp/xtnkk-tools-1.0.0.8.tar.gz` & `tmp/xtnkk-tools-1.0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xtnkk-tools-1.0.0.8.tar", last modified: Wed Apr 17 09:53:36 2024, max compression
+gzip compressed data, was "dist\xtnkk-tools-1.0.0.9.tar", last modified: Wed Apr 17 13:44:48 2024, max compression
```

## Comparing `xtnkk-tools-1.0.0.8.tar` & `xtnkk-tools-1.0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 09:53:36.000000 xtnkk-tools-1.0.0.8/
--rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtnkk-tools-1.0.0.8/LICENSE
--rw-rw-rw-   0        0        0      283 2024-04-17 09:53:36.000000 xtnkk-tools-1.0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtnkk-tools-1.0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-04-17 09:53:36.000000 xtnkk-tools-1.0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1167 2024-04-17 09:53:23.000000 xtnkk-tools-1.0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 09:53:36.000000 xtnkk-tools-1.0.0.8/xtnkk_tools/
--rw-rw-rw-   0        0        0     5484 2024-04-17 09:53:16.000000 xtnkk-tools-1.0.0.8/xtnkk_tools/MongoDB.py
--rw-rw-rw-   0        0        0      395 2024-04-17 03:29:31.000000 xtnkk-tools-1.0.0.8/xtnkk_tools/__init__.py
--rw-rw-rw-   0        0        0     4491 2024-04-17 08:40:50.000000 xtnkk-tools-1.0.0.8/xtnkk_tools/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-17 09:53:36.000000 xtnkk-tools-1.0.0.8/xtnkk_tools.egg-info/
--rw-rw-rw-   0        0        0      283 2024-04-17 09:53:36.000000 xtnkk-tools-1.0.0.8/xtnkk_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2024-04-17 09:53:36.000000 xtnkk-tools-1.0.0.8/xtnkk_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 09:53:36.000000 xtnkk-tools-1.0.0.8/xtnkk_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-17 09:53:36.000000 xtnkk-tools-1.0.0.8/xtnkk_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-17 09:53:36.000000 xtnkk-tools-1.0.0.8/xtnkk_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 13:44:48.000000 xtnkk-tools-1.0.0.9/
+-rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtnkk-tools-1.0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      283 2024-04-17 13:44:48.000000 xtnkk-tools-1.0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtnkk-tools-1.0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-17 13:44:48.000000 xtnkk-tools-1.0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1167 2024-04-17 13:44:33.000000 xtnkk-tools-1.0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 13:44:48.000000 xtnkk-tools-1.0.0.9/xtnkk_tools/
+-rw-rw-rw-   0        0        0     5484 2024-04-17 09:53:16.000000 xtnkk-tools-1.0.0.9/xtnkk_tools/MongoDB.py
+-rw-rw-rw-   0        0        0      395 2024-04-17 03:29:31.000000 xtnkk-tools-1.0.0.9/xtnkk_tools/__init__.py
+-rw-rw-rw-   0        0        0     5196 2024-04-17 13:44:24.000000 xtnkk-tools-1.0.0.9/xtnkk_tools/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-17 13:44:48.000000 xtnkk-tools-1.0.0.9/xtnkk_tools.egg-info/
+-rw-rw-rw-   0        0        0      283 2024-04-17 13:44:48.000000 xtnkk-tools-1.0.0.9/xtnkk_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2024-04-17 13:44:48.000000 xtnkk-tools-1.0.0.9/xtnkk_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 13:44:48.000000 xtnkk-tools-1.0.0.9/xtnkk_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-17 13:44:48.000000 xtnkk-tools-1.0.0.9/xtnkk_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-17 13:44:48.000000 xtnkk-tools-1.0.0.9/xtnkk_tools.egg-info/top_level.txt
```

### Comparing `xtnkk-tools-1.0.0.8/setup.py` & `xtnkk-tools-1.0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="xtnkk-tools",  # 模块名称
-    version="1.0.0.8",  # 版本
+    version="1.0.0.9",  # 版本
     author="xtn",  # 作者
     author_email="czw011122@163.com",  # 作者邮箱
     description="xtn 开发工具",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     long_description_content_type="text/markdown",  # 模块详细介绍格式
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
     # 模块相关的元数据(更多描述信息)
```

### Comparing `xtnkk-tools-1.0.0.8/xtnkk_tools/MongoDB.py` & `xtnkk-tools-1.0.0.9/xtnkk_tools/MongoDB.py`

 * *Files identical despite different names*

### Comparing `xtnkk-tools-1.0.0.8/xtnkk_tools/tools.py` & `xtnkk-tools-1.0.0.9/xtnkk_tools/tools.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 # 说明：
 #    tools
 # History:
 # Date          Author    Version       Modification
 # --------------------------------------------------------------------------------------------------
 # 2024/4/17    xiatn     V00.01.000    新建
 # --------------------------------------------------------------------------------------------------
-import hashlib, time, datetime
+import hashlib, time, datetime, json
+from urllib.parse import urlencode
 
 
 def get_md5_32(s, is_upper=False):
     """
         获取文本的md5值 32位
     :param s: 文本
     :param is_upper: 是否转大写 默认False
@@ -109,14 +110,41 @@
     # 转换为整数类型
     if is_time_13:
         return int(timestamp * 1000)
     else:
         return int(timestamp)
 
 
+def get_str_to_json(str_json):
+    """
+        字符串类型的json格式 转 json
+    :param str_json: 字符串json
+    :return:
+    """
+    try:
+        new_str_json = str_json.replace("'", '"'). \
+            replace("None", "null").replace("True", "true"). \
+            replace("False", "false")
+        return json.loads(new_str_json)
+    except Exception as e:
+        return {}
+
+
+def get_url_params(url, params):
+    """
+        传入url和params拼接完整的url
+    :param url:
+    :param params:
+    :return:
+    """
+    encoded_params = urlencode(params)
+    full_url = url + "?" + encoded_params
+    return full_url
+
+
 if __name__ == '__main__':
     pass
     # print(get_md5_16("1", True))  # 获取16位md5结果
     # print(get_md5_32("1", True))  # 获取32位md5结果
     # print(get_now_time_int())  # 获取当前时间戳
     # print(get_now_time_int(True, False))  # 获取当前10位时间戳
     # print(get_now_time_int(False, True))  # 获取当前13位时间戳
```

