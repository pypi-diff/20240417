# Comparing `tmp/zq-tools-1.0.2.tar.gz` & `tmp/zq-tools-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zq-tools-1.0.2.tar", last modified: Wed Aug  2 03:39:00 2023, max compression
+gzip compressed data, was "zq-tools-1.0.3.tar", last modified: Tue Apr 16 07:46:46 2024, max compression
```

## Comparing `zq-tools-1.0.2.tar` & `zq-tools-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 togo      (1000) togo      (1000)        0 2023-08-02 03:39:00.108540 zq-tools-1.0.2/
--rw-r--r--   0 togo      (1000) togo      (1000)     3040 2023-08-02 03:39:00.108540 zq-tools-1.0.2/PKG-INFO
--rw-r--r--   0 togo      (1000) togo      (1000)     2707 2023-08-02 03:37:45.000000 zq-tools-1.0.2/README.md
--rw-r--r--   0 togo      (1000) togo      (1000)       38 2023-08-02 03:39:00.108540 zq-tools-1.0.2/setup.cfg
--rw-r--r--   0 togo      (1000) togo      (1000)      622 2023-08-02 03:38:09.000000 zq-tools-1.0.2/setup.py
-drwxr-xr-x   0 togo      (1000) togo      (1000)        0 2023-08-02 03:39:00.108540 zq-tools-1.0.2/test/
--rw-r--r--   0 togo      (1000) togo      (1000)       91 2023-08-02 02:47:40.000000 zq-tools-1.0.2/test/test_zq_logger.py
--rw-r--r--   0 togo      (1000) togo      (1000)     1051 2023-08-02 02:47:40.000000 zq-tools-1.0.2/test/test_zq_tracing.py
-drwxr-xr-x   0 togo      (1000) togo      (1000)        0 2023-08-02 03:39:00.108540 zq-tools-1.0.2/zq_tools/
--rw-r--r--   0 togo      (1000) togo      (1000)      187 2023-08-02 02:47:40.000000 zq-tools-1.0.2/zq_tools/__init__.py
--rw-r--r--   0 togo      (1000) togo      (1000)      830 2023-08-02 02:47:40.000000 zq-tools-1.0.2/zq_tools/zq_cycle.py
--rw-r--r--   0 togo      (1000) togo      (1000)     4596 2023-08-02 02:47:40.000000 zq-tools-1.0.2/zq_tools/zq_decorator.py
--rw-r--r--   0 togo      (1000) togo      (1000)      520 2023-08-02 02:47:40.000000 zq-tools-1.0.2/zq_tools/zq_files.py
--rw-r--r--   0 togo      (1000) togo      (1000)     9290 2023-08-02 03:35:41.000000 zq-tools-1.0.2/zq_tools/zq_logger.py
--rw-r--r--   0 togo      (1000) togo      (1000)     5227 2023-08-02 02:47:40.000000 zq-tools-1.0.2/zq_tools/zq_tracing.py
-drwxr-xr-x   0 togo      (1000) togo      (1000)        0 2023-08-02 03:39:00.108540 zq-tools-1.0.2/zq_tools.egg-info/
--rw-r--r--   0 togo      (1000) togo      (1000)     3040 2023-08-02 03:39:00.000000 zq-tools-1.0.2/zq_tools.egg-info/PKG-INFO
--rw-r--r--   0 togo      (1000) togo      (1000)      357 2023-08-02 03:39:00.000000 zq-tools-1.0.2/zq_tools.egg-info/SOURCES.txt
--rw-r--r--   0 togo      (1000) togo      (1000)        1 2023-08-02 03:39:00.000000 zq-tools-1.0.2/zq_tools.egg-info/dependency_links.txt
--rw-r--r--   0 togo      (1000) togo      (1000)       23 2023-08-02 03:39:00.000000 zq-tools-1.0.2/zq_tools.egg-info/requires.txt
--rw-r--r--   0 togo      (1000) togo      (1000)        9 2023-08-02 03:39:00.000000 zq-tools-1.0.2/zq_tools.egg-info/top_level.txt
+drwxrwxr-x   0 qzhou     (1003) qzhou     (1003)        0 2024-04-16 07:46:46.847846 zq-tools-1.0.3/
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)     3095 2024-04-16 07:46:46.847846 zq-tools-1.0.3/PKG-INFO
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)     2762 2024-04-16 07:44:13.000000 zq-tools-1.0.3/README.md
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)       38 2024-04-16 07:46:46.847846 zq-tools-1.0.3/setup.cfg
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)      622 2024-04-16 07:43:43.000000 zq-tools-1.0.3/setup.py
+drwxrwxr-x   0 qzhou     (1003) qzhou     (1003)        0 2024-04-16 07:46:46.847846 zq-tools-1.0.3/test/
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)       91 2022-11-19 05:19:08.000000 zq-tools-1.0.3/test/test_zq_logger.py
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)     1051 2022-09-25 08:06:36.000000 zq-tools-1.0.3/test/test_zq_tracing.py
+drwxrwxr-x   0 qzhou     (1003) qzhou     (1003)        0 2024-04-16 07:46:46.847846 zq-tools-1.0.3/zq_tools/
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)      187 2022-11-19 05:17:23.000000 zq-tools-1.0.3/zq_tools/__init__.py
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)      830 2022-12-21 11:09:55.000000 zq-tools-1.0.3/zq_tools/zq_cycle.py
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)     4596 2022-10-25 03:53:08.000000 zq-tools-1.0.3/zq_tools/zq_decorator.py
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)      520 2022-09-25 08:26:17.000000 zq-tools-1.0.3/zq_tools/zq_files.py
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)     9429 2024-04-16 07:43:35.000000 zq-tools-1.0.3/zq_tools/zq_logger.py
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)     5227 2022-10-20 06:14:14.000000 zq-tools-1.0.3/zq_tools/zq_tracing.py
+drwxrwxr-x   0 qzhou     (1003) qzhou     (1003)        0 2024-04-16 07:46:46.847846 zq-tools-1.0.3/zq_tools.egg-info/
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)     3095 2024-04-16 07:46:46.000000 zq-tools-1.0.3/zq_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)      357 2024-04-16 07:46:46.000000 zq-tools-1.0.3/zq_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)        1 2024-04-16 07:46:46.000000 zq-tools-1.0.3/zq_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)       23 2024-04-16 07:46:46.000000 zq-tools-1.0.3/zq_tools.egg-info/requires.txt
+-rw-rw-r--   0 qzhou     (1003) qzhou     (1003)        9 2024-04-16 07:46:46.000000 zq-tools-1.0.3/zq_tools.egg-info/top_level.txt
```

### Comparing `zq-tools-1.0.2/PKG-INFO` & `zq-tools-1.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zq-tools
-Version: 1.0.2
+Version: 1.0.3
 Summary: A collection of tools for zzqq2199
 Author: zzqq2199
 Author-email: zhouquanjs@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -19,15 +19,16 @@
 # zq_tracing
 help generate json file used in `chrome://tracing`
 
 ![](https://raw.githubusercontent.com/zzqq2199/pic_for_public/master/img/20220608134508.png)
 
 
 # Release Notes
-- 1.0.2: Fine grained control of different handlers
+- 1.0.3: make logger.debug to print without any color.
+- 1.0.2: fine grained control of different handlers
 - 0.9.9: add `__repr__` for zq_cycle
 - 0.9.8: support `from zq_tools import logger` as well as `from zq_tools.zq_logger import default_logger as logger` for shorter code
 - 0.9.7: fix `setLevel` bug in zq_logger; use env value to initilize ZQ_Logger's controlling level
 - 0.9.6: increase version due to keep failing on uploading
 - 0.9.4: fix bug: `zq_decorator.time_it(sync)`
 - 0.9.3: update `zq_decorator:: do_nothing, pass_it, time_it(support sync and self-defined print)`
 - 0.9.2: fix bug: `.zq_logger` to `zq_tools.zq_logger`
```

### Comparing `zq-tools-1.0.2/README.md` & `zq-tools-1.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 # zq_tracing
 help generate json file used in `chrome://tracing`
 
 ![](https://raw.githubusercontent.com/zzqq2199/pic_for_public/master/img/20220608134508.png)
 
 
 # Release Notes
-- 1.0.2: Fine grained control of different handlers
+- 1.0.3: make logger.debug to print without any color.
+- 1.0.2: fine grained control of different handlers
 - 0.9.9: add `__repr__` for zq_cycle
 - 0.9.8: support `from zq_tools import logger` as well as `from zq_tools.zq_logger import default_logger as logger` for shorter code
 - 0.9.7: fix `setLevel` bug in zq_logger; use env value to initilize ZQ_Logger's controlling level
 - 0.9.6: increase version due to keep failing on uploading
 - 0.9.4: fix bug: `zq_decorator.time_it(sync)`
 - 0.9.3: update `zq_decorator:: do_nothing, pass_it, time_it(support sync and self-defined print)`
 - 0.9.2: fix bug: `.zq_logger` to `zq_tools.zq_logger`
```

### Comparing `zq-tools-1.0.2/setup.py` & `zq-tools-1.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="zq-tools",
-    version="1.0.2",
+    version="1.0.3",
     author="zzqq2199",
     author_email="zhouquanjs@qq.com",
     description="A collection of tools for zzqq2199",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["zq_tools"],
     classifiers=[
```

### Comparing `zq-tools-1.0.2/test/test_zq_tracing.py` & `zq-tools-1.0.3/test/test_zq_tracing.py`

 * *Files identical despite different names*

### Comparing `zq-tools-1.0.2/zq_tools/zq_cycle.py` & `zq-tools-1.0.3/zq_tools/zq_cycle.py`

 * *Files identical despite different names*

### Comparing `zq-tools-1.0.2/zq_tools/zq_decorator.py` & `zq-tools-1.0.3/zq_tools/zq_decorator.py`

 * *Files identical despite different names*

### Comparing `zq-tools-1.0.2/zq_tools/zq_files.py` & `zq-tools-1.0.3/zq_tools/zq_files.py`

 * *Files identical despite different names*

### Comparing `zq-tools-1.0.2/zq_tools/zq_logger.py` & `zq-tools-1.0.3/zq_tools/zq_logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,19 +92,21 @@
         return self
     
     def prank(self, msg:str, color:str='',*args, **kwargs):
         '''print with rank. If color is not specified, use the color format corresponding to the rank'''
         if not self.isEnabledFor(self.PRANK): return
         color = getattr(cf, color) if color else self.default_color
         self._log(self.PRANK, color(msg), args, **kwargs)
-    def debug(self, msg:str, color:str='',*args, **kwargs):
-        '''print with rank. If color is not specified, use the color format corresponding to the rank'''
-        if not self.isEnabledFor(self.DEBUG): return
-        color = getattr(cf, color) if color else self.default_color
-        self._log(self.DEBUG, color(msg), args, **kwargs)
+    # def debug(self, msg:str, color:str='',*args, **kwargs):
+    #     '''print with rank. If color is not specified, use the color format corresponding to the rank'''
+    #     if not self.isEnabledFor(self.DEBUG): return
+    #     color = getattr(cf, color) if color else self.default_color
+    #     self._log(self.DEBUG, color(msg), args, **kwargs)
+    def debug(self, msg:str, *args, **kwargs):
+        if self.isEnabledFor(logging.INFO): self._log(logging.INFO, args, kwargs)
     def info(self, msg:str, *args, **kwargs):
         if self.isEnabledFor(logging.INFO): self._log(logging.INFO, cf.green(msg), args, kwargs)
     def warn(self, msg:str, *args, **kwargs):
         if self.isEnabledFor(logging.WARN): self._log(logging.WARN, cf.yellow(msg), args, kwargs)
     def error(self, msg:str, *args, **kwargs):
         if self.isEnabledFor(logging.ERROR): self._log(logging.ERROR, cf.red(msg), args, kwargs)
     def fatal(self, msg:str, *args, **kwargs):
```

### Comparing `zq-tools-1.0.2/zq_tools/zq_tracing.py` & `zq-tools-1.0.3/zq_tools/zq_tracing.py`

 * *Files identical despite different names*

### Comparing `zq-tools-1.0.2/zq_tools.egg-info/PKG-INFO` & `zq-tools-1.0.3/zq_tools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zq-tools
-Version: 1.0.2
+Version: 1.0.3
 Summary: A collection of tools for zzqq2199
 Author: zzqq2199
 Author-email: zhouquanjs@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -19,15 +19,16 @@
 # zq_tracing
 help generate json file used in `chrome://tracing`
 
 ![](https://raw.githubusercontent.com/zzqq2199/pic_for_public/master/img/20220608134508.png)
 
 
 # Release Notes
-- 1.0.2: Fine grained control of different handlers
+- 1.0.3: make logger.debug to print without any color.
+- 1.0.2: fine grained control of different handlers
 - 0.9.9: add `__repr__` for zq_cycle
 - 0.9.8: support `from zq_tools import logger` as well as `from zq_tools.zq_logger import default_logger as logger` for shorter code
 - 0.9.7: fix `setLevel` bug in zq_logger; use env value to initilize ZQ_Logger's controlling level
 - 0.9.6: increase version due to keep failing on uploading
 - 0.9.4: fix bug: `zq_decorator.time_it(sync)`
 - 0.9.3: update `zq_decorator:: do_nothing, pass_it, time_it(support sync and self-defined print)`
 - 0.9.2: fix bug: `.zq_logger` to `zq_tools.zq_logger`
```

