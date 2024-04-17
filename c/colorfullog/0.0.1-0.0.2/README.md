# Comparing `tmp/colorfullog-0.0.1.tar.gz` & `tmp/colorfullog-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorfullog-0.0.1.tar", last modified: Wed Apr 17 06:48:32 2024, max compression
+gzip compressed data, was "colorfullog-0.0.2.tar", last modified: Wed Apr 17 07:14:11 2024, max compression
```

## Comparing `colorfullog-0.0.1.tar` & `colorfullog-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxrwxr-x   0 ares      (1000) ares      (1000)        0 2024-04-17 06:48:32.009066 colorfullog-0.0.1/
--rw-rw-r--   0 ares      (1000) ares      (1000)      444 2024-04-17 06:48:32.009066 colorfullog-0.0.1/PKG-INFO
--rw-r--r--   0 ares      (1000) ares      (1000)      518 2024-04-17 06:47:59.000000 colorfullog-0.0.1/README.md
-drwxrwxr-x   0 ares      (1000) ares      (1000)        0 2024-04-17 06:48:32.009066 colorfullog-0.0.1/colorfullog/
--rw-r--r--   0 ares      (1000) ares      (1000)       70 2024-04-17 06:48:19.000000 colorfullog-0.0.1/colorfullog/__init__.py
--rw-r--r--   0 ares      (1000) ares      (1000)     3245 2018-06-21 03:15:57.000000 colorfullog-0.0.1/colorfullog/colorfullog.py
-drwxrwxr-x   0 ares      (1000) ares      (1000)        0 2024-04-17 06:48:32.009066 colorfullog-0.0.1/colorfullog.egg-info/
--rw-rw-r--   0 ares      (1000) ares      (1000)      444 2024-04-17 06:48:31.000000 colorfullog-0.0.1/colorfullog.egg-info/PKG-INFO
--rw-rw-r--   0 ares      (1000) ares      (1000)      219 2024-04-17 06:48:31.000000 colorfullog-0.0.1/colorfullog.egg-info/SOURCES.txt
--rw-rw-r--   0 ares      (1000) ares      (1000)        1 2024-04-17 06:48:31.000000 colorfullog-0.0.1/colorfullog.egg-info/dependency_links.txt
--rw-rw-r--   0 ares      (1000) ares      (1000)       12 2024-04-17 06:48:31.000000 colorfullog-0.0.1/colorfullog.egg-info/top_level.txt
--rw-r--r--   0 ares      (1000) ares      (1000)       38 2024-04-17 06:48:32.009066 colorfullog-0.0.1/setup.cfg
--rw-r--r--   0 ares      (1000) ares      (1000)     1315 2024-04-17 06:47:50.000000 colorfullog-0.0.1/setup.py
+drwxrwxr-x   0 ares      (1000) ares      (1000)        0 2024-04-17 07:14:11.125286 colorfullog-0.0.2/
+-rw-rw-r--   0 ares      (1000) ares      (1000)      444 2024-04-17 07:14:11.125286 colorfullog-0.0.2/PKG-INFO
+-rw-r--r--   0 ares      (1000) ares      (1000)      518 2024-04-17 06:47:59.000000 colorfullog-0.0.2/README.md
+drwxrwxr-x   0 ares      (1000) ares      (1000)        0 2024-04-17 07:14:11.125286 colorfullog-0.0.2/colorfullog/
+-rw-r--r--   0 ares      (1000) ares      (1000)       90 2024-04-17 07:14:01.000000 colorfullog-0.0.2/colorfullog/__init__.py
+-rw-r--r--   0 ares      (1000) ares      (1000)     3245 2018-06-21 03:15:57.000000 colorfullog-0.0.2/colorfullog/colorfullog.py
+drwxrwxr-x   0 ares      (1000) ares      (1000)        0 2024-04-17 07:14:11.125286 colorfullog-0.0.2/colorfullog/libs/
+-rw-rw-r--   0 ares      (1000) ares      (1000)        0 2024-04-17 07:03:38.000000 colorfullog-0.0.2/colorfullog/libs/__init__.py
+-rw-------   0 ares      (1000) ares      (1000)    96311 2022-07-15 03:49:46.000000 colorfullog-0.0.2/colorfullog/libs/argparse.py
+-rw-------   0 ares      (1000) ares      (1000)    41477 2024-04-17 07:01:46.000000 colorfullog-0.0.2/colorfullog/libs/os.py
+drwxrwxr-x   0 ares      (1000) ares      (1000)        0 2024-04-17 07:14:11.125286 colorfullog-0.0.2/colorfullog.egg-info/
+-rw-rw-r--   0 ares      (1000) ares      (1000)      444 2024-04-17 07:14:11.000000 colorfullog-0.0.2/colorfullog.egg-info/PKG-INFO
+-rw-rw-r--   0 ares      (1000) ares      (1000)      300 2024-04-17 07:14:11.000000 colorfullog-0.0.2/colorfullog.egg-info/SOURCES.txt
+-rw-rw-r--   0 ares      (1000) ares      (1000)        1 2024-04-17 07:14:11.000000 colorfullog-0.0.2/colorfullog.egg-info/dependency_links.txt
+-rw-rw-r--   0 ares      (1000) ares      (1000)       12 2024-04-17 07:14:11.000000 colorfullog-0.0.2/colorfullog.egg-info/top_level.txt
+-rw-r--r--   0 ares      (1000) ares      (1000)       38 2024-04-17 07:14:11.125286 colorfullog-0.0.2/setup.cfg
+-rw-r--r--   0 ares      (1000) ares      (1000)     1315 2024-04-17 06:52:56.000000 colorfullog-0.0.2/setup.py
```

### Comparing `colorfullog-0.0.1/README.md` & `colorfullog-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `colorfullog-0.0.1/colorfullog/colorfullog.py` & `colorfullog-0.0.2/colorfullog/colorfullog.py`

 * *Files identical despite different names*

### Comparing `colorfullog-0.0.1/setup.py` & `colorfullog-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 long_description = 'set console color of font'
 if os.path.exists('README.rst'):
     long_description = open('README.rst').read()
 
 setuptools.setup(
     name="colorfullog",
-    version="0.0.1",
+    version="0.0.2",
     author="Peng Shiyu",
     license = 'MIT License',
     author_email="pengshiyuyx@gmail.com",
     description="set console color of font",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/mouday/colorfullog",
```

