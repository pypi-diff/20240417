# Comparing `tmp/xtnkk-tools-1.0.0.4.tar.gz` & `tmp/xtnkk-tools-1.0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xtnkk-tools-1.0.0.4.tar", last modified: Wed Apr 17 05:16:25 2024, max compression
+gzip compressed data, was "dist\xtnkk-tools-1.0.0.5.tar", last modified: Wed Apr 17 08:09:55 2024, max compression
```

## Comparing `xtnkk-tools-1.0.0.4.tar` & `xtnkk-tools-1.0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 05:16:25.000000 xtnkk-tools-1.0.0.4/
--rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtnkk-tools-1.0.0.4/LICENSE
--rw-rw-rw-   0        0        0      283 2024-04-17 05:16:25.000000 xtnkk-tools-1.0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtnkk-tools-1.0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-17 05:16:25.000000 xtnkk-tools-1.0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1167 2024-04-17 05:16:12.000000 xtnkk-tools-1.0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 05:16:25.000000 xtnkk-tools-1.0.0.4/xtnkk_tools/
--rw-rw-rw-   0        0        0     4448 2024-04-17 05:15:54.000000 xtnkk-tools-1.0.0.4/xtnkk_tools/MongoDB.py
--rw-rw-rw-   0        0        0      395 2024-04-17 03:29:31.000000 xtnkk-tools-1.0.0.4/xtnkk_tools/__init__.py
--rw-rw-rw-   0        0        0     1111 2024-04-17 05:13:16.000000 xtnkk-tools-1.0.0.4/xtnkk_tools/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-17 05:16:25.000000 xtnkk-tools-1.0.0.4/xtnkk_tools.egg-info/
--rw-rw-rw-   0        0        0      283 2024-04-17 05:16:25.000000 xtnkk-tools-1.0.0.4/xtnkk_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2024-04-17 05:16:25.000000 xtnkk-tools-1.0.0.4/xtnkk_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 05:16:25.000000 xtnkk-tools-1.0.0.4/xtnkk_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-17 05:16:25.000000 xtnkk-tools-1.0.0.4/xtnkk_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-17 05:16:25.000000 xtnkk-tools-1.0.0.4/xtnkk_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 08:09:55.000000 xtnkk-tools-1.0.0.5/
+-rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtnkk-tools-1.0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      283 2024-04-17 08:09:55.000000 xtnkk-tools-1.0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtnkk-tools-1.0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-17 08:09:55.000000 xtnkk-tools-1.0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1167 2024-04-17 08:09:53.000000 xtnkk-tools-1.0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:09:55.000000 xtnkk-tools-1.0.0.5/xtnkk_tools/
+-rw-rw-rw-   0        0        0     4448 2024-04-17 05:15:54.000000 xtnkk-tools-1.0.0.5/xtnkk_tools/MongoDB.py
+-rw-rw-rw-   0        0        0      395 2024-04-17 03:29:31.000000 xtnkk-tools-1.0.0.5/xtnkk_tools/__init__.py
+-rw-rw-rw-   0        0        0     1792 2024-04-17 08:09:37.000000 xtnkk-tools-1.0.0.5/xtnkk_tools/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:09:55.000000 xtnkk-tools-1.0.0.5/xtnkk_tools.egg-info/
+-rw-rw-rw-   0        0        0      283 2024-04-17 08:09:55.000000 xtnkk-tools-1.0.0.5/xtnkk_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2024-04-17 08:09:55.000000 xtnkk-tools-1.0.0.5/xtnkk_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 08:09:55.000000 xtnkk-tools-1.0.0.5/xtnkk_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-17 08:09:55.000000 xtnkk-tools-1.0.0.5/xtnkk_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-17 08:09:55.000000 xtnkk-tools-1.0.0.5/xtnkk_tools.egg-info/top_level.txt
```

### Comparing `xtnkk-tools-1.0.0.4/setup.py` & `xtnkk-tools-1.0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="xtnkk-tools",  # 模块名称
-    version="1.0.0.4",  # 版本
+    version="1.0.0.5",  # 版本
     author="xtn",  # 作者
     author_email="czw011122@163.com",  # 作者邮箱
     description="xtn 开发工具",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     long_description_content_type="text/markdown",  # 模块详细介绍格式
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
     # 模块相关的元数据(更多描述信息)
```

### Comparing `xtnkk-tools-1.0.0.4/xtnkk_tools/MongoDB.py` & `xtnkk-tools-1.0.0.5/xtnkk_tools/MongoDB.py`

 * *Files identical despite different names*

