# Comparing `tmp/xtnkk-tools-1.0.0.3.tar.gz` & `tmp/xtnkk-tools-1.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xtnkk-tools-1.0.0.3.tar", last modified: Wed Apr 17 05:04:31 2024, max compression
+gzip compressed data, was "dist\xtnkk-tools-1.0.0.4.tar", last modified: Wed Apr 17 05:16:25 2024, max compression
```

## Comparing `xtnkk-tools-1.0.0.3.tar` & `xtnkk-tools-1.0.0.4.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 05:04:31.000000 xtnkk-tools-1.0.0.3/
--rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtnkk-tools-1.0.0.3/LICENSE
--rw-rw-rw-   0        0        0      283 2024-04-17 05:04:31.000000 xtnkk-tools-1.0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtnkk-tools-1.0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-17 05:04:31.000000 xtnkk-tools-1.0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1150 2024-04-17 05:04:25.000000 xtnkk-tools-1.0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 05:04:31.000000 xtnkk-tools-1.0.0.3/xtnkk_tools/
--rw-rw-rw-   0        0        0      395 2024-04-17 03:29:31.000000 xtnkk-tools-1.0.0.3/xtnkk_tools/__init__.py
--rw-rw-rw-   0        0        0     1117 2024-04-17 05:02:40.000000 xtnkk-tools-1.0.0.3/xtnkk_tools/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-17 05:04:31.000000 xtnkk-tools-1.0.0.3/xtnkk_tools.egg-info/
--rw-rw-rw-   0        0        0      283 2024-04-17 05:04:31.000000 xtnkk-tools-1.0.0.3/xtnkk_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2024-04-17 05:04:31.000000 xtnkk-tools-1.0.0.3/xtnkk_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 05:04:31.000000 xtnkk-tools-1.0.0.3/xtnkk_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-17 05:04:31.000000 xtnkk-tools-1.0.0.3/xtnkk_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 05:16:25.000000 xtnkk-tools-1.0.0.4/
+-rw-rw-rw-   0        0        0        0 2024-04-17 03:27:01.000000 xtnkk-tools-1.0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      283 2024-04-17 05:16:25.000000 xtnkk-tools-1.0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2024-04-17 03:28:15.000000 xtnkk-tools-1.0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-17 05:16:25.000000 xtnkk-tools-1.0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1167 2024-04-17 05:16:12.000000 xtnkk-tools-1.0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 05:16:25.000000 xtnkk-tools-1.0.0.4/xtnkk_tools/
+-rw-rw-rw-   0        0        0     4448 2024-04-17 05:15:54.000000 xtnkk-tools-1.0.0.4/xtnkk_tools/MongoDB.py
+-rw-rw-rw-   0        0        0      395 2024-04-17 03:29:31.000000 xtnkk-tools-1.0.0.4/xtnkk_tools/__init__.py
+-rw-rw-rw-   0        0        0     1111 2024-04-17 05:13:16.000000 xtnkk-tools-1.0.0.4/xtnkk_tools/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-17 05:16:25.000000 xtnkk-tools-1.0.0.4/xtnkk_tools.egg-info/
+-rw-rw-rw-   0        0        0      283 2024-04-17 05:16:25.000000 xtnkk-tools-1.0.0.4/xtnkk_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2024-04-17 05:16:25.000000 xtnkk-tools-1.0.0.4/xtnkk_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 05:16:25.000000 xtnkk-tools-1.0.0.4/xtnkk_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-17 05:16:25.000000 xtnkk-tools-1.0.0.4/xtnkk_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-17 05:16:25.000000 xtnkk-tools-1.0.0.4/xtnkk_tools.egg-info/top_level.txt
```

### Comparing `xtnkk-tools-1.0.0.3/setup.py` & `xtnkk-tools-1.0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="xtnkk-tools",  # 模块名称
-    version="1.0.0.3",  # 版本
+    version="1.0.0.4",  # 版本
     author="xtn",  # 作者
     author_email="czw011122@163.com",  # 作者邮箱
     description="xtn 开发工具",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     long_description_content_type="text/markdown",  # 模块详细介绍格式
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
     # 模块相关的元数据(更多描述信息)
     classifiers=[
         "Programming Language :: Python :: 3",
     ],
     # 依赖模块
     install_requires=[
-
+        "pymongo"
     ],
     python_requires='>=3',
 )
```

### Comparing `xtnkk-tools-1.0.0.3/xtnkk_tools/tools.py` & `xtnkk-tools-1.0.0.4/xtnkk_tools/tools.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,10 +32,10 @@
     :param is_upper: 是否转大写 默认False
     :return:
     """
     result = get_md5_32(s, is_upper)
     return result[8:24]
 
 
-# if __name__ == '__main__':
-#     print(get_md5_16("1", True))
-#     print(get_md5_32("1", True))
+if __name__ == '__main__':
+    print(get_md5_16("1", True))
+    print(get_md5_32("1", True))
```

