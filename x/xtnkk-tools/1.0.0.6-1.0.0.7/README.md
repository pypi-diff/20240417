# Comparing `tmp/xtnkk-tools-1.0.0.6.tar.gz` & `tmp/xtnkk-tools-1.0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xtnkk-tools-1.0.0.6.tar", last modified: Wed Apr 17 08:17:00 2024, max compression
+gzip compressed data, was "dist\xtnkk-tools-1.0.0.7.tar", last modified: Wed Apr 17 08:41:12 2024, max compression
```

## Comparing `xtnkk-tools-1.0.0.6.tar` & `xtnkk-tools-1.0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 08:17:00.000000 xtnkk-tools-1.0.0.6/
--rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtnkk-tools-1.0.0.6/LICENSE
--rw-rw-rw-   0        0        0      283 2024-04-17 08:17:00.000000 xtnkk-tools-1.0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtnkk-tools-1.0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-17 08:17:00.000000 xtnkk-tools-1.0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1167 2024-04-17 08:16:49.000000 xtnkk-tools-1.0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 08:17:00.000000 xtnkk-tools-1.0.0.6/xtnkk_tools/
--rw-rw-rw-   0        0        0     4920 2024-04-17 08:16:03.000000 xtnkk-tools-1.0.0.6/xtnkk_tools/MongoDB.py
--rw-rw-rw-   0        0        0      395 2024-04-17 03:29:31.000000 xtnkk-tools-1.0.0.6/xtnkk_tools/__init__.py
--rw-rw-rw-   0        0        0     1792 2024-04-17 08:09:37.000000 xtnkk-tools-1.0.0.6/xtnkk_tools/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-17 08:17:00.000000 xtnkk-tools-1.0.0.6/xtnkk_tools.egg-info/
--rw-rw-rw-   0        0        0      283 2024-04-17 08:17:00.000000 xtnkk-tools-1.0.0.6/xtnkk_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2024-04-17 08:17:00.000000 xtnkk-tools-1.0.0.6/xtnkk_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 08:17:00.000000 xtnkk-tools-1.0.0.6/xtnkk_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-17 08:17:00.000000 xtnkk-tools-1.0.0.6/xtnkk_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-17 08:17:00.000000 xtnkk-tools-1.0.0.6/xtnkk_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 08:41:12.000000 xtnkk-tools-1.0.0.7/
+-rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtnkk-tools-1.0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      283 2024-04-17 08:41:12.000000 xtnkk-tools-1.0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtnkk-tools-1.0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-17 08:41:12.000000 xtnkk-tools-1.0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1167 2024-04-17 08:41:04.000000 xtnkk-tools-1.0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:41:12.000000 xtnkk-tools-1.0.0.7/xtnkk_tools/
+-rw-rw-rw-   0        0        0     4932 2024-04-17 08:22:51.000000 xtnkk-tools-1.0.0.7/xtnkk_tools/MongoDB.py
+-rw-rw-rw-   0        0        0      395 2024-04-17 03:29:31.000000 xtnkk-tools-1.0.0.7/xtnkk_tools/__init__.py
+-rw-rw-rw-   0        0        0     4491 2024-04-17 08:40:50.000000 xtnkk-tools-1.0.0.7/xtnkk_tools/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-17 08:41:12.000000 xtnkk-tools-1.0.0.7/xtnkk_tools.egg-info/
+-rw-rw-rw-   0        0        0      283 2024-04-17 08:41:12.000000 xtnkk-tools-1.0.0.7/xtnkk_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2024-04-17 08:41:12.000000 xtnkk-tools-1.0.0.7/xtnkk_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 08:41:12.000000 xtnkk-tools-1.0.0.7/xtnkk_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-17 08:41:12.000000 xtnkk-tools-1.0.0.7/xtnkk_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-17 08:41:12.000000 xtnkk-tools-1.0.0.7/xtnkk_tools.egg-info/top_level.txt
```

### Comparing `xtnkk-tools-1.0.0.6/setup.py` & `xtnkk-tools-1.0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="xtnkk-tools",  # 模块名称
-    version="1.0.0.6",  # 版本
+    version="1.0.0.7",  # 版本
     author="xtn",  # 作者
     author_email="czw011122@163.com",  # 作者邮箱
     description="xtn 开发工具",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     long_description_content_type="text/markdown",  # 模块详细介绍格式
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
     # 模块相关的元数据(更多描述信息)
```

### Comparing `xtnkk-tools-1.0.0.6/xtnkk_tools/MongoDB.py` & `xtnkk-tools-1.0.0.7/xtnkk_tools/MongoDB.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # 说明：
 #    MongoDBPro
 # History:
 # Date          Author    Version       Modification
 # --------------------------------------------------------------------------------------------------
 # 2024/4/17    xiatn     V00.01.000    新建
 # --------------------------------------------------------------------------------------------------
-from tools import *
+from xtnkk_tools.tools import *
 from urllib import parse
 from typing import List, Dict, Optional
 from pymongo import MongoClient
 from pymongo.database import Database
 from pymongo.collection import Collection
 from pymongo.errors import DuplicateKeyError, BulkWriteError
```

