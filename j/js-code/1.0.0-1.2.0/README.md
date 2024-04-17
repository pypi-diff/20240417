# Comparing `tmp/js-code-1.0.0.tar.gz` & `tmp/js_code-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "js-code-1.0.0.tar", last modified: Sat May 20 03:10:12 2023, max compression
+gzip compressed data, was "js_code-1.2.0.tar", last modified: Wed Apr 17 00:25:20 2024, max compression
```

## Comparing `js-code-1.0.0.tar` & `js_code-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 03:10:12.430037 js-code-1.0.0/
--rw-rw-rw-   0        0        0     1094 2023-04-12 08:29:30.000000 js-code-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      330 2023-05-20 03:10:12.429041 js-code-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-20 03:10:12.412085 js-code-1.0.0/js_code/
--rw-rw-rw-   0        0        0        0 2023-04-12 06:50:12.000000 js-code-1.0.0/js_code/__init__.py
--rw-rw-rw-   0        0        0     1130 2023-05-19 00:11:10.000000 js-code-1.0.0/js_code/js_open.py
-drwxrwxrwx   0        0        0        0 2023-05-20 03:10:12.428046 js-code-1.0.0/js_code.egg-info/
--rw-rw-rw-   0        0        0      330 2023-05-20 03:10:12.000000 js-code-1.0.0/js_code.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-05-20 03:10:12.000000 js-code-1.0.0/js_code.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 03:10:12.000000 js-code-1.0.0/js_code.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-20 03:10:12.000000 js-code-1.0.0/js_code.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-20 03:10:12.000000 js-code-1.0.0/js_code.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 03:10:12.430037 js-code-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      490 2023-05-20 03:09:23.000000 js-code-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 00:25:20.123046 js_code-1.2.0/
+-rw-rw-rw-   0        0        0     1094 2023-04-12 08:29:30.000000 js_code-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0      333 2024-04-17 00:25:20.122049 js_code-1.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-17 00:25:20.113074 js_code-1.2.0/js_code/
+-rw-rw-rw-   0        0        0        0 2023-04-12 06:50:12.000000 js_code-1.2.0/js_code/__init__.py
+-rw-rw-rw-   0        0        0     1294 2024-04-17 00:12:11.000000 js_code-1.2.0/js_code/js_open.py
+drwxrwxrwx   0        0        0        0 2024-04-17 00:25:20.121051 js_code-1.2.0/js_code.egg-info/
+-rw-rw-rw-   0        0        0      333 2024-04-17 00:25:20.000000 js_code-1.2.0/js_code.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2024-04-17 00:25:20.000000 js_code-1.2.0/js_code.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 00:25:20.000000 js_code-1.2.0/js_code.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-17 00:25:20.000000 js_code-1.2.0/js_code.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-17 00:25:20.000000 js_code-1.2.0/js_code.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 00:25:20.123046 js_code-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      494 2024-04-17 00:21:15.000000 js_code-1.2.0/setup.py
```

### Comparing `js-code-1.0.0/LICENSE` & `js_code-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `js-code-1.0.0/js_code/js_open.py` & `js_code-1.2.0/js_code/js_open.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,23 @@
 import subprocess
 
 # 防止乱码
 subprocess.Popen = partial(subprocess.Popen, encoding="utf-8")
 import execjs
 
 
-def js_lead_into(file=None, code=None, encoding="utf-8"):
+from functools import partial  # 锁定参数
+import subprocess
+
+# 防止乱码
+subprocess.Popen = partial(subprocess.Popen, encoding="utf-8")
+import execjs
+
+
+def js_read(file=None, code=None, encoding="utf-8"):
     """
     :param code:需要添加在文件开头  javascript 代码  示例 code = "var a = 10;\n"
     :param file: 需要手动添加文件路径，或者javascript的代码格式(function fn(){return xxx;};
     有条件判断增加相应的条件判断，或者循环)
     :param mode: 只读模式
     :param encoding: 默认utf-8
     """
@@ -29,7 +37,8 @@
             js = execjs.compile(f"{code}{file}")
         else:
             js = execjs.compile(file)
     return js
 
 
 
+
```

