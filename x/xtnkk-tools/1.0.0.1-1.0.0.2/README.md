# Comparing `tmp/xtnkk-tools-1.0.0.1.tar.gz` & `tmp/xtnkk-tools-1.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xtnkk-tools-1.0.0.1.tar", last modified: Wed Apr 17 04:56:00 2024, max compression
+gzip compressed data, was "dist\xtnkk-tools-1.0.0.2.tar", last modified: Wed Apr 17 05:02:58 2024, max compression
```

## Comparing `xtnkk-tools-1.0.0.1.tar` & `xtnkk-tools-1.0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 04:56:00.000000 xtnkk-tools-1.0.0.1/
--rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtnkk-tools-1.0.0.1/LICENSE
--rw-rw-rw-   0        0        0      283 2024-04-17 04:56:00.000000 xtnkk-tools-1.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtnkk-tools-1.0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-17 04:56:00.000000 xtnkk-tools-1.0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1167 2024-04-17 04:53:21.000000 xtnkk-tools-1.0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 04:56:00.000000 xtnkk-tools-1.0.0.1/xtnkk_tools/
--rw-rw-rw-   0        0        0      395 2024-04-17 03:29:31.000000 xtnkk-tools-1.0.0.1/xtnkk_tools/__init__.py
--rw-rw-rw-   0        0        0     1111 2024-04-17 04:52:07.000000 xtnkk-tools-1.0.0.1/xtnkk_tools/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-17 04:56:00.000000 xtnkk-tools-1.0.0.1/xtnkk_tools.egg-info/
--rw-rw-rw-   0        0        0      283 2024-04-17 04:56:00.000000 xtnkk-tools-1.0.0.1/xtnkk_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2024-04-17 04:56:00.000000 xtnkk-tools-1.0.0.1/xtnkk_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 04:56:00.000000 xtnkk-tools-1.0.0.1/xtnkk_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-17 04:56:00.000000 xtnkk-tools-1.0.0.1/xtnkk_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-17 04:56:00.000000 xtnkk-tools-1.0.0.1/xtnkk_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 05:02:58.000000 xtnkk-tools-1.0.0.2/
+-rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtnkk-tools-1.0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      283 2024-04-17 05:02:58.000000 xtnkk-tools-1.0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtnkk-tools-1.0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-17 05:02:58.000000 xtnkk-tools-1.0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1167 2024-04-17 05:02:46.000000 xtnkk-tools-1.0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 05:02:58.000000 xtnkk-tools-1.0.0.2/xtnkk_tools/
+-rw-rw-rw-   0        0        0      395 2024-04-17 03:29:31.000000 xtnkk-tools-1.0.0.2/xtnkk_tools/__init__.py
+-rw-rw-rw-   0        0        0     1117 2024-04-17 05:02:40.000000 xtnkk-tools-1.0.0.2/xtnkk_tools/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-17 05:02:58.000000 xtnkk-tools-1.0.0.2/xtnkk_tools.egg-info/
+-rw-rw-rw-   0        0        0      283 2024-04-17 05:02:58.000000 xtnkk-tools-1.0.0.2/xtnkk_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2024-04-17 05:02:58.000000 xtnkk-tools-1.0.0.2/xtnkk_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 05:02:58.000000 xtnkk-tools-1.0.0.2/xtnkk_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-17 05:02:58.000000 xtnkk-tools-1.0.0.2/xtnkk_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-17 05:02:58.000000 xtnkk-tools-1.0.0.2/xtnkk_tools.egg-info/top_level.txt
```

### Comparing `xtnkk-tools-1.0.0.1/setup.py` & `xtnkk-tools-1.0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="xtnkk-tools",  # 模块名称
-    version="1.0.0.1",  # 版本
+    version="1.0.0.2",  # 版本
     author="xtn",  # 作者
     author_email="czw011122@163.com",  # 作者邮箱
     description="xtn 开发工具",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     long_description_content_type="text/markdown",  # 模块详细介绍格式
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
     # 模块相关的元数据(更多描述信息)
```

### Comparing `xtnkk-tools-1.0.0.1/xtnkk_tools/tools.py` & `xtnkk-tools-1.0.0.2/xtnkk_tools/tools.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,10 +32,10 @@
     :param is_upper: 是否转大写 默认False
     :return:
     """
     result = get_md5_32(s, is_upper)
     return result[8:24]
 
 
-if __name__ == '__main__':
-    print(get_md5_16("1", True))
-    print(get_md5_32("1", True))
+# if __name__ == '__main__':
+#     print(get_md5_16("1", True))
+#     print(get_md5_32("1", True))
```

