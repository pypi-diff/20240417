# Comparing `tmp/zhanshop-0.0.2.tar.gz` & `tmp/zhanshop-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhanshop-0.0.2.tar", last modified: Tue Apr 16 09:15:48 2024, max compression
+gzip compressed data, was "zhanshop-0.0.3.tar", last modified: Wed Apr 17 08:47:28 2024, max compression
```

## Comparing `zhanshop-0.0.2.tar` & `zhanshop-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 zhangqiquan   (501) staff       (20)        0 2024-04-16 09:15:48.362721 zhanshop-0.0.2/
--rw-r--r--   0 zhangqiquan   (501) staff       (20)     1100 2024-04-16 02:30:09.000000 zhanshop-0.0.2/LICENSE
--rw-r--r--   0 zhangqiquan   (501) staff       (20)      124 2024-04-16 09:15:48.361842 zhanshop-0.0.2/PKG-INFO
--rw-r--r--   0 zhangqiquan   (501) staff       (20)      440 2024-04-16 02:37:57.000000 zhanshop-0.0.2/README.md
--rw-r--r--   0 zhangqiquan   (501) staff       (20)       46 2024-04-16 09:15:27.000000 zhanshop-0.0.2/pyproject.toml
--rw-r--r--   0 zhangqiquan   (501) staff       (20)       82 2024-04-16 09:15:48.365747 zhanshop-0.0.2/setup.cfg
--rw-r--r--   0 zhangqiquan   (501) staff       (20)      318 2024-04-16 09:15:21.000000 zhanshop-0.0.2/setup.py
-drwxr-xr-x   0 zhangqiquan   (501) staff       (20)        0 2024-04-16 09:15:48.340173 zhanshop-0.0.2/test/
--rw-r--r--   0 zhangqiquan   (501) staff       (20)      104 2024-04-16 02:30:09.000000 zhanshop-0.0.2/test/test_zhanshop.py
-drwxr-xr-x   0 zhangqiquan   (501) staff       (20)        0 2024-04-16 09:15:48.345425 zhanshop-0.0.2/zhanshop/
--rw-r--r--   0 zhangqiquan   (501) staff       (20)      170 2024-04-16 05:37:08.000000 zhanshop-0.0.2/zhanshop/app.py
-drwxr-xr-x   0 zhangqiquan   (501) staff       (20)        0 2024-04-16 09:15:48.354752 zhanshop-0.0.2/zhanshop/command/
--rw-r--r--   0 zhangqiquan   (501) staff       (20)       73 2024-04-16 05:08:48.000000 zhanshop-0.0.2/zhanshop/command/__init__.py
--rw-r--r--   0 zhangqiquan   (501) staff       (20)      130 2024-04-16 07:09:51.000000 zhanshop-0.0.2/zhanshop/command/helper.py
--rw-r--r--   0 zhangqiquan   (501) staff       (20)      658 2024-04-16 05:51:46.000000 zhanshop-0.0.2/zhanshop/command/server.py
--rw-r--r--   0 zhangqiquan   (501) staff       (20)      889 2024-04-16 07:09:08.000000 zhanshop-0.0.2/zhanshop/console.py
--rw-r--r--   0 zhangqiquan   (501) staff       (20)      397 2024-04-16 05:08:48.000000 zhanshop-0.0.2/zhanshop/container.py
--rw-r--r--   0 zhangqiquan   (501) staff       (20)      373 2024-04-16 08:43:54.000000 zhanshop-0.0.2/zhanshop/controller.py
--rw-r--r--   0 zhangqiquan   (501) staff       (20)      234 2024-04-16 05:08:48.000000 zhanshop-0.0.2/zhanshop/helper.py
--rw-r--r--   0 zhangqiquan   (501) staff       (20)      459 2024-04-16 05:08:48.000000 zhanshop-0.0.2/zhanshop/log.py
--rw-r--r--   0 zhangqiquan   (501) staff       (20)      455 2024-04-16 06:47:48.000000 zhanshop-0.0.2/zhanshop/webhandle.py
-drwxr-xr-x   0 zhangqiquan   (501) staff       (20)        0 2024-04-16 09:15:48.358830 zhanshop-0.0.2/zhanshop.egg-info/
--rw-r--r--   0 zhangqiquan   (501) staff       (20)      124 2024-04-16 09:15:48.000000 zhanshop-0.0.2/zhanshop.egg-info/PKG-INFO
--rw-r--r--   0 zhangqiquan   (501) staff       (20)      422 2024-04-16 09:15:48.000000 zhanshop-0.0.2/zhanshop.egg-info/SOURCES.txt
--rw-r--r--   0 zhangqiquan   (501) staff       (20)        1 2024-04-16 09:15:48.000000 zhanshop-0.0.2/zhanshop.egg-info/dependency_links.txt
--rw-r--r--   0 zhangqiquan   (501) staff       (20)        9 2024-04-16 09:15:48.000000 zhanshop-0.0.2/zhanshop.egg-info/top_level.txt
+drwxr-xr-x   0 zhangqiquan   (501) staff       (20)        0 2024-04-17 08:47:28.098935 zhanshop-0.0.3/
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)     1100 2024-04-16 02:30:09.000000 zhanshop-0.0.3/LICENSE
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)      124 2024-04-17 08:47:28.098541 zhanshop-0.0.3/PKG-INFO
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)      440 2024-04-16 02:37:57.000000 zhanshop-0.0.3/README.md
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)       46 2024-04-17 08:43:48.000000 zhanshop-0.0.3/pyproject.toml
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)       82 2024-04-17 08:47:28.100305 zhanshop-0.0.3/setup.cfg
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)      318 2024-04-17 08:47:11.000000 zhanshop-0.0.3/setup.py
+drwxr-xr-x   0 zhangqiquan   (501) staff       (20)        0 2024-04-17 08:47:28.043031 zhanshop-0.0.3/test/
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)      104 2024-04-16 02:30:09.000000 zhanshop-0.0.3/test/test_zhanshop.py
+drwxr-xr-x   0 zhangqiquan   (501) staff       (20)        0 2024-04-17 08:47:28.071738 zhanshop-0.0.3/zhanshop/
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)      170 2024-04-16 05:37:08.000000 zhanshop-0.0.3/zhanshop/app.py
+drwxr-xr-x   0 zhangqiquan   (501) staff       (20)        0 2024-04-17 08:47:28.095885 zhanshop-0.0.3/zhanshop/command/
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)       73 2024-04-16 05:08:48.000000 zhanshop-0.0.3/zhanshop/command/__init__.py
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)      130 2024-04-16 07:09:51.000000 zhanshop-0.0.3/zhanshop/command/helper.py
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)      658 2024-04-16 05:51:46.000000 zhanshop-0.0.3/zhanshop/command/server.py
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)      889 2024-04-16 07:09:08.000000 zhanshop-0.0.3/zhanshop/console.py
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)      397 2024-04-16 05:08:48.000000 zhanshop-0.0.3/zhanshop/container.py
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)      391 2024-04-17 08:46:58.000000 zhanshop-0.0.3/zhanshop/controller.py
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)      234 2024-04-16 05:08:48.000000 zhanshop-0.0.3/zhanshop/helper.py
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)      459 2024-04-16 05:08:48.000000 zhanshop-0.0.3/zhanshop/log.py
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)      311 2024-04-17 08:46:58.000000 zhanshop-0.0.3/zhanshop/webhandle.py
+drwxr-xr-x   0 zhangqiquan   (501) staff       (20)        0 2024-04-17 08:47:28.097617 zhanshop-0.0.3/zhanshop.egg-info/
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)      124 2024-04-17 08:47:27.000000 zhanshop-0.0.3/zhanshop.egg-info/PKG-INFO
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)      422 2024-04-17 08:47:27.000000 zhanshop-0.0.3/zhanshop.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)        1 2024-04-17 08:47:27.000000 zhanshop-0.0.3/zhanshop.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangqiquan   (501) staff       (20)        9 2024-04-17 08:47:27.000000 zhanshop-0.0.3/zhanshop.egg-info/top_level.txt
```

### Comparing `zhanshop-0.0.2/LICENSE` & `zhanshop-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zhanshop-0.0.2/zhanshop/command/server.py` & `zhanshop-0.0.3/zhanshop/command/server.py`

 * *Files identical despite different names*

### Comparing `zhanshop-0.0.2/zhanshop/console.py` & `zhanshop-0.0.3/zhanshop/console.py`

 * *Files identical despite different names*

