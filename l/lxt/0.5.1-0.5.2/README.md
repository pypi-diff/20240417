# Comparing `tmp/lxt-0.5.1.tar.gz` & `tmp/lxt-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lxt-0.5.1.tar", last modified: Thu Apr 11 16:18:35 2024, max compression
+gzip compressed data, was "lxt-0.5.2.tar", last modified: Wed Apr 17 14:00:51 2024, max compression
```

## Comparing `lxt-0.5.1.tar` & `lxt-0.5.2.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxr-xr-x   0 achtibat (1342060776) domain users (1342000513)        0 2024-04-11 16:18:35.473678 lxt-0.5.1/
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     2156 2024-04-05 14:07:44.000000 lxt-0.5.1/LICENSE
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     5812 2024-04-11 16:18:35.473678 lxt-0.5.1/PKG-INFO
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     5560 2024-04-11 13:37:53.000000 lxt-0.5.1/README.md
-drwxr-xr-x   0 achtibat (1342060776) domain users (1342000513)        0 2024-04-11 16:18:35.473678 lxt-0.5.1/lxt/
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)        0 2024-04-05 14:07:44.000000 lxt-0.5.1/lxt/__init__.py
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)      785 2024-04-05 14:18:02.000000 lxt-0.5.1/lxt/check.py
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)    15189 2024-04-05 14:07:45.000000 lxt-0.5.1/lxt/core.py
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)    20440 2024-04-11 16:00:37.000000 lxt-0.5.1/lxt/functional.py
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     3081 2024-04-11 16:15:12.000000 lxt-0.5.1/lxt/modules.py
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)    13091 2024-04-05 14:28:12.000000 lxt-0.5.1/lxt/rules.py
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     3435 2024-04-05 14:44:58.000000 lxt-0.5.1/lxt/utils.py
-drwxr-xr-x   0 achtibat (1342060776) domain users (1342000513)        0 2024-04-11 16:18:35.473678 lxt-0.5.1/lxt.egg-info/
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     5812 2024-04-11 16:18:35.000000 lxt-0.5.1/lxt.egg-info/PKG-INFO
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)      327 2024-04-11 16:18:35.000000 lxt-0.5.1/lxt.egg-info/SOURCES.txt
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)        1 2024-04-11 16:18:35.000000 lxt-0.5.1/lxt.egg-info/dependency_links.txt
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)       63 2024-04-11 16:18:35.000000 lxt-0.5.1/lxt.egg-info/requires.txt
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)        4 2024-04-11 16:18:35.000000 lxt-0.5.1/lxt.egg-info/top_level.txt
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)       38 2024-04-11 16:18:35.473678 lxt-0.5.1/setup.cfg
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)      600 2024-04-11 16:07:52.000000 lxt-0.5.1/setup.py
-drwxr-xr-x   0 achtibat (1342060776) domain users (1342000513)        0 2024-04-11 16:18:35.473678 lxt-0.5.1/tests/
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     5262 2024-04-11 16:03:47.000000 lxt-0.5.1/tests/test_functional.py
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)      943 2024-04-11 16:16:01.000000 lxt-0.5.1/tests/test_modules.py
--rw-r--r--   0 achtibat (1342060776) domain users (1342000513)      758 2024-04-11 15:35:57.000000 lxt-0.5.1/tests/test_rules.py
+drwxr-xr-x   0 achtibat (1342060776) domain users (1342000513)        0 2024-04-17 14:00:51.352733 lxt-0.5.2/
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     2156 2024-04-05 14:07:44.000000 lxt-0.5.2/LICENSE
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     5812 2024-04-17 14:00:51.348733 lxt-0.5.2/PKG-INFO
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     5560 2024-04-11 13:37:53.000000 lxt-0.5.2/README.md
+drwxr-xr-x   0 achtibat (1342060776) domain users (1342000513)        0 2024-04-17 14:00:51.348733 lxt-0.5.2/lxt/
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)        0 2024-04-05 14:07:44.000000 lxt-0.5.2/lxt/__init__.py
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)      785 2024-04-05 14:18:02.000000 lxt-0.5.2/lxt/check.py
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)    15189 2024-04-05 14:07:45.000000 lxt-0.5.2/lxt/core.py
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)    20440 2024-04-11 16:00:37.000000 lxt-0.5.2/lxt/functional.py
+drwxr-xr-x   0 achtibat (1342060776) domain users (1342000513)        0 2024-04-17 14:00:51.348733 lxt-0.5.2/lxt/models/
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)        0 2024-04-17 13:59:18.000000 lxt-0.5.2/lxt/models/__init__.py
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)    46773 2024-04-05 14:35:59.000000 lxt-0.5.2/lxt/models/llama.py
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)    55330 2024-04-05 15:06:50.000000 lxt-0.5.2/lxt/models/mixtral.py
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     3081 2024-04-11 16:15:12.000000 lxt-0.5.2/lxt/modules.py
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)    13091 2024-04-05 14:28:12.000000 lxt-0.5.2/lxt/rules.py
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     3435 2024-04-05 14:44:58.000000 lxt-0.5.2/lxt/utils.py
+drwxr-xr-x   0 achtibat (1342060776) domain users (1342000513)        0 2024-04-17 14:00:51.348733 lxt-0.5.2/lxt.egg-info/
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     5812 2024-04-17 14:00:51.000000 lxt-0.5.2/lxt.egg-info/PKG-INFO
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)      392 2024-04-17 14:00:51.000000 lxt-0.5.2/lxt.egg-info/SOURCES.txt
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)        1 2024-04-17 14:00:51.000000 lxt-0.5.2/lxt.egg-info/dependency_links.txt
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)       63 2024-04-17 14:00:51.000000 lxt-0.5.2/lxt.egg-info/requires.txt
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)        4 2024-04-17 14:00:51.000000 lxt-0.5.2/lxt.egg-info/top_level.txt
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)       38 2024-04-17 14:00:51.352733 lxt-0.5.2/setup.cfg
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)      600 2024-04-17 13:59:49.000000 lxt-0.5.2/setup.py
+drwxr-xr-x   0 achtibat (1342060776) domain users (1342000513)        0 2024-04-17 14:00:51.348733 lxt-0.5.2/tests/
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)     5262 2024-04-11 16:03:47.000000 lxt-0.5.2/tests/test_functional.py
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)      943 2024-04-11 16:16:01.000000 lxt-0.5.2/tests/test_modules.py
+-rw-r--r--   0 achtibat (1342060776) domain users (1342000513)      758 2024-04-11 15:35:57.000000 lxt-0.5.2/tests/test_rules.py
```

### Comparing `lxt-0.5.1/LICENSE` & `lxt-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lxt-0.5.1/PKG-INFO` & `lxt-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lxt
-Version: 0.5.1
+Version: 0.5.2
 Summary: LRP explains Transformers
 Home-page: https://github.com/rachtibat/LRP-for-Transformers
 Author: Reduan Achtibat
 License: BSD 3-clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `lxt-0.5.1/README.md` & `lxt-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `lxt-0.5.1/lxt/check.py` & `lxt-0.5.2/lxt/check.py`

 * *Files identical despite different names*

### Comparing `lxt-0.5.1/lxt/core.py` & `lxt-0.5.2/lxt/core.py`

 * *Files identical despite different names*

### Comparing `lxt-0.5.1/lxt/functional.py` & `lxt-0.5.2/lxt/functional.py`

 * *Files identical despite different names*

### Comparing `lxt-0.5.1/lxt/modules.py` & `lxt-0.5.2/lxt/modules.py`

 * *Files identical despite different names*

### Comparing `lxt-0.5.1/lxt/rules.py` & `lxt-0.5.2/lxt/rules.py`

 * *Files identical despite different names*

### Comparing `lxt-0.5.1/lxt/utils.py` & `lxt-0.5.2/lxt/utils.py`

 * *Files identical despite different names*

### Comparing `lxt-0.5.1/lxt.egg-info/PKG-INFO` & `lxt-0.5.2/lxt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lxt
-Version: 0.5.1
+Version: 0.5.2
 Summary: LRP explains Transformers
 Home-page: https://github.com/rachtibat/LRP-for-Transformers
 Author: Reduan Achtibat
 License: BSD 3-clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `lxt-0.5.1/setup.py` & `lxt-0.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name='lxt',  
-    version='0.5.1',
+    version='0.5.2',
     install_requires=[
         'torch',
         'transformers',
         'accelerate',
         'tabulate',
         'matplotlib',
         'bitsandbytes'
```

### Comparing `lxt-0.5.1/tests/test_functional.py` & `lxt-0.5.2/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `lxt-0.5.1/tests/test_modules.py` & `lxt-0.5.2/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `lxt-0.5.1/tests/test_rules.py` & `lxt-0.5.2/tests/test_rules.py`

 * *Files identical despite different names*

