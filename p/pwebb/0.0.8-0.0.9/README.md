# Comparing `tmp/pwebb-0.0.8.tar.gz` & `tmp/pwebb-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwebb-0.0.8.tar", last modified: Mon Nov 20 01:25:33 2023, max compression
+gzip compressed data, was "pwebb-0.0.9.tar", last modified: Wed Dec 13 13:22:07 2023, max compression
```

## Comparing `pwebb-0.0.8.tar` & `pwebb-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-11-20 01:25:33.816628 pwebb-0.0.8/
--rw-rw-rw-   0        0        0    11549 2023-10-23 17:44:04.000000 pwebb-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     3116 2023-11-20 01:25:33.815631 pwebb-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2386 2023-10-23 17:44:04.000000 pwebb-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-11-20 01:25:33.755183 pwebb-0.0.8/pweb/
--rw-rw-rw-   0        0        0     1013 2023-11-05 16:11:02.000000 pwebb-0.0.8/pweb/__init__.py
--rw-rw-rw-   0        0        0     1458 2023-10-23 17:36:55.000000 pwebb-0.0.8/pweb/pweb_engine.py
-drwxrwxrwx   0        0        0        0 2023-11-20 01:25:33.797768 pwebb-0.0.8/pweb/system12/
--rw-rw-rw-   0        0        0        0 2023-10-23 17:36:55.000000 pwebb-0.0.8/pweb/system12/__init__.py
--rw-rw-rw-   0        0        0     1749 2023-11-05 16:11:02.000000 pwebb-0.0.8/pweb/system12/pweb_app_config.py
--rw-rw-rw-   0        0        0       63 2023-10-23 17:36:55.000000 pwebb-0.0.8/pweb/system12/pweb_base.py
--rw-rw-rw-   0        0        0     5769 2023-11-05 16:11:02.000000 pwebb-0.0.8/pweb/system12/pweb_bismillah.py
--rw-rw-rw-   0        0        0     1267 2023-10-23 17:36:55.000000 pwebb-0.0.8/pweb/system12/pweb_cache.py
--rw-rw-rw-   0        0        0      858 2023-10-23 17:36:55.000000 pwebb-0.0.8/pweb/system12/pweb_interfaces.py
--rw-rw-rw-   0        0        0      694 2023-10-23 17:36:55.000000 pwebb-0.0.8/pweb/system12/pweb_module_cli.py
--rw-rw-rw-   0        0        0     3659 2023-11-17 03:57:21.000000 pwebb-0.0.8/pweb/system12/pweb_module_manager.py
--rw-rw-rw-   0        0        0      269 2023-10-23 17:36:55.000000 pwebb-0.0.8/pweb/system12/pweb_registry.py
-drwxrwxrwx   0        0        0        0 2023-11-20 01:25:33.814633 pwebb-0.0.8/pwebb.egg-info/
--rw-rw-rw-   0        0        0     3116 2023-11-20 01:25:33.000000 pwebb-0.0.8/pwebb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      547 2023-11-20 01:25:33.000000 pwebb-0.0.8/pwebb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-20 01:25:33.000000 pwebb-0.0.8/pwebb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-11-20 01:25:33.000000 pwebb-0.0.8/pwebb.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-10-23 17:36:57.000000 pwebb-0.0.8/pwebb.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       87 2023-11-20 01:25:33.000000 pwebb-0.0.8/pwebb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-11-20 01:25:33.000000 pwebb-0.0.8/pwebb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-20 01:25:33.816628 pwebb-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1244 2023-11-20 01:24:04.000000 pwebb-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-12-13 13:22:07.455299 pwebb-0.0.9/
+-rw-rw-rw-   0        0        0    11549 2023-11-24 04:41:27.000000 pwebb-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3116 2023-12-13 13:22:07.452309 pwebb-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2386 2023-11-24 04:41:27.000000 pwebb-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-12-13 13:22:07.347133 pwebb-0.0.9/pweb/
+-rw-rw-rw-   0        0        0     1013 2023-11-24 04:41:27.000000 pwebb-0.0.9/pweb/__init__.py
+-rw-rw-rw-   0        0        0     1458 2023-11-24 04:41:27.000000 pwebb-0.0.9/pweb/pweb_engine.py
+drwxrwxrwx   0        0        0        0 2023-12-13 13:22:07.419978 pwebb-0.0.9/pweb/system12/
+-rw-rw-rw-   0        0        0        0 2023-11-24 04:41:27.000000 pwebb-0.0.9/pweb/system12/__init__.py
+-rw-rw-rw-   0        0        0     1749 2023-11-24 04:41:27.000000 pwebb-0.0.9/pweb/system12/pweb_app_config.py
+-rw-rw-rw-   0        0        0       63 2023-11-24 04:41:27.000000 pwebb-0.0.9/pweb/system12/pweb_base.py
+-rw-rw-rw-   0        0        0     5769 2023-11-24 04:41:27.000000 pwebb-0.0.9/pweb/system12/pweb_bismillah.py
+-rw-rw-rw-   0        0        0     1267 2023-11-24 04:41:27.000000 pwebb-0.0.9/pweb/system12/pweb_cache.py
+-rw-rw-rw-   0        0        0      858 2023-11-24 04:41:27.000000 pwebb-0.0.9/pweb/system12/pweb_interfaces.py
+-rw-rw-rw-   0        0        0      694 2023-11-24 04:41:27.000000 pwebb-0.0.9/pweb/system12/pweb_module_cli.py
+-rw-rw-rw-   0        0        0     3659 2023-11-24 04:41:27.000000 pwebb-0.0.9/pweb/system12/pweb_module_manager.py
+-rw-rw-rw-   0        0        0      269 2023-11-24 04:41:27.000000 pwebb-0.0.9/pweb/system12/pweb_registry.py
+drwxrwxrwx   0        0        0        0 2023-12-13 13:22:07.451310 pwebb-0.0.9/pwebb.egg-info/
+-rw-rw-rw-   0        0        0     3116 2023-12-13 13:22:07.000000 pwebb-0.0.9/pwebb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2023-12-13 13:22:07.000000 pwebb-0.0.9/pwebb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-12-13 13:22:07.000000 pwebb-0.0.9/pwebb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-12-13 13:22:07.000000 pwebb-0.0.9/pwebb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-11-24 04:41:32.000000 pwebb-0.0.9/pwebb.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       87 2023-12-13 13:22:07.000000 pwebb-0.0.9/pwebb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-12-13 13:22:07.000000 pwebb-0.0.9/pwebb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-12-13 13:22:07.455299 pwebb-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1244 2023-12-13 13:05:35.000000 pwebb-0.0.9/setup.py
```

### Comparing `pwebb-0.0.8/LICENSE` & `pwebb-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pwebb-0.0.8/PKG-INFO` & `pwebb-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwebb
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python Web Boot (PWebB). PWebB is a DRY full-stack framework based on Flask micro web framework.
 Home-page: https://github.com/banglafighter/pweb
 Author: Bangla Fighter
 Author-email: banglafighter.com@gmail.com
 License: Apache 2.0
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `pwebb-0.0.8/README.md` & `pwebb-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pwebb-0.0.8/pweb/__init__.py` & `pwebb-0.0.9/pweb/__init__.py`

 * *Files identical despite different names*

### Comparing `pwebb-0.0.8/pweb/pweb_engine.py` & `pwebb-0.0.9/pweb/pweb_engine.py`

 * *Files identical despite different names*

### Comparing `pwebb-0.0.8/pweb/system12/pweb_app_config.py` & `pwebb-0.0.9/pweb/system12/pweb_app_config.py`

 * *Files identical despite different names*

### Comparing `pwebb-0.0.8/pweb/system12/pweb_bismillah.py` & `pwebb-0.0.9/pweb/system12/pweb_bismillah.py`

 * *Files identical despite different names*

### Comparing `pwebb-0.0.8/pweb/system12/pweb_cache.py` & `pwebb-0.0.9/pweb/system12/pweb_cache.py`

 * *Files identical despite different names*

### Comparing `pwebb-0.0.8/pweb/system12/pweb_interfaces.py` & `pwebb-0.0.9/pweb/system12/pweb_interfaces.py`

 * *Files identical despite different names*

### Comparing `pwebb-0.0.8/pweb/system12/pweb_module_cli.py` & `pwebb-0.0.9/pweb/system12/pweb_module_cli.py`

 * *Files identical despite different names*

### Comparing `pwebb-0.0.8/pweb/system12/pweb_module_manager.py` & `pwebb-0.0.9/pweb/system12/pweb_module_manager.py`

 * *Files identical despite different names*

### Comparing `pwebb-0.0.8/pwebb.egg-info/PKG-INFO` & `pwebb-0.0.9/pwebb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwebb
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python Web Boot (PWebB). PWebB is a DRY full-stack framework based on Flask micro web framework.
 Home-page: https://github.com/banglafighter/pweb
 Author: Bangla Fighter
 Author-email: banglafighter.com@gmail.com
 License: Apache 2.0
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `pwebb-0.0.8/pwebb.egg-info/SOURCES.txt` & `pwebb-0.0.9/pwebb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pwebb-0.0.8/setup.py` & `pwebb-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         return dependency
 
     return dependency + ["ppy-common", "pweb-orm", "pweb-form-rest", "pweb-cli", "ppy-jsonyml"]
 
 
 setup(
     name='pwebb',
-    version='0.0.8',
+    version='0.0.9',
     url='https://github.com/banglafighter/pweb',
     license='Apache 2.0',
     author='Bangla Fighter',
     author_email='banglafighter.com@gmail.com',
     description='Python Web Boot (PWebB). PWebB is a DRY full-stack framework based on Flask micro web framework.',
     long_description=README,
     long_description_content_type='text/markdown',
```

