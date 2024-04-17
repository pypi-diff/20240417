# Comparing `tmp/tsugu-0.5.1.tar.gz` & `tmp/tsugu-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-0.5.1.tar", last modified: Wed Apr 17 06:58:37 2024, max compression
+gzip compressed data, was "tsugu-0.5.2.tar", last modified: Wed Apr 17 07:02:50 2024, max compression
```

## Comparing `tsugu-0.5.1.tar` & `tsugu-0.5.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:37.284395 tsugu-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-17 06:58:26.000000 tsugu-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-17 06:58:37.284395 tsugu-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-17 06:58:26.000000 tsugu-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 06:58:37.284395 tsugu-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-17 06:58:26.000000 tsugu-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:37.280395 tsugu-0.5.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-17 06:58:26.000000 tsugu-0.5.1/test/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:37.284395 tsugu-0.5.1/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-17 06:58:26.000000 tsugu-0.5.1/tsugu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21286 2024-04-17 06:58:26.000000 tsugu-0.5.1/tsugu/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11967 2024-04-17 06:58:26.000000 tsugu-0.5.1/tsugu/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-04-17 06:58:26.000000 tsugu-0.5.1/tsugu/router.py
--rw-r--r--   0 runner    (1001) docker     (127)    21534 2024-04-17 06:58:26.000000 tsugu-0.5.1/tsugu/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:58:37.284395 tsugu-0.5.1/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-17 06:58:36.000000 tsugu-0.5.1/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-17 06:58:37.000000 tsugu-0.5.1/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:58:36.000000 tsugu-0.5.1/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 06:58:36.000000 tsugu-0.5.1/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 06:58:36.000000 tsugu-0.5.1/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:02:50.850352 tsugu-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-17 07:02:42.000000 tsugu-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-17 07:02:50.850352 tsugu-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-17 07:02:42.000000 tsugu-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 07:02:50.850352 tsugu-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-17 07:02:42.000000 tsugu-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:02:50.850352 tsugu-0.5.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-17 07:02:42.000000 tsugu-0.5.2/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:02:50.850352 tsugu-0.5.2/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-17 07:02:42.000000 tsugu-0.5.2/tsugu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21286 2024-04-17 07:02:42.000000 tsugu-0.5.2/tsugu/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12008 2024-04-17 07:02:42.000000 tsugu-0.5.2/tsugu/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-04-17 07:02:42.000000 tsugu-0.5.2/tsugu/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21534 2024-04-17 07:02:42.000000 tsugu-0.5.2/tsugu/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 07:02:50.850352 tsugu-0.5.2/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-17 07:02:50.000000 tsugu-0.5.2/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-17 07:02:50.000000 tsugu-0.5.2/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 07:02:50.000000 tsugu-0.5.2/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 07:02:50.000000 tsugu-0.5.2/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 07:02:50.000000 tsugu-0.5.2/tsugu.egg-info/top_level.txt
```

### Comparing `tsugu-0.5.1/LICENSE` & `tsugu-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-0.5.1/PKG-INFO` & `tsugu-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.5.1
+Version: 0.5.2
 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
         <h1 align="center"> Tsugu Python Frontend <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu Version: 0.5.1 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.5.2 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

### Comparing `tsugu-0.5.1/README.md` & `tsugu-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-0.5.1/setup.py` & `tsugu-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='0.5.1',
+    version='0.5.2',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py',
```

### Comparing `tsugu-0.5.1/test/test_main.py` & `tsugu-0.5.2/test/test_main.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.5.1/tsugu/config.py` & `tsugu-0.5.2/tsugu/config.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.5.1/tsugu/handler.py` & `tsugu-0.5.2/tsugu/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,16 @@
     :param user_id: 用户ID
     :param platform: 平台名称 默认 red
     :param channel_id: 频道ID / 群号
     :return: List[Union[bytes, str]] bytes 为图片 str 为文字
     '''
     data = bot(message, user_id, platform, channel_id)
     response = []
+    if not data:
+        return response
     for item in data:
         if item['type'] == 'string':
             response.append(item['string'])
         elif item['type'] == 'base64':
             bytes_data = base64.b64decode(item['string'].encode('utf-8'))
             response.append(bytes_data)
     return response
```

### Comparing `tsugu-0.5.1/tsugu/router.py` & `tsugu-0.5.2/tsugu/router.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.5.1/tsugu/utils.py` & `tsugu-0.5.2/tsugu/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.5.1/tsugu.egg-info/PKG-INFO` & `tsugu-0.5.2/tsugu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.5.1
+Version: 0.5.2
 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
         <h1 align="center"> Tsugu Python Frontend <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu Version: 0.5.1 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.5.2 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

