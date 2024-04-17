# Comparing `tmp/gpp_components-0.1.2.tar.gz` & `tmp/gpp_components-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpp_components-0.1.2.tar", last modified: Tue Apr 16 02:00:37 2024, max compression
+gzip compressed data, was "gpp_components-0.1.3.tar", last modified: Wed Apr 17 06:43:32 2024, max compression
```

## Comparing `gpp_components-0.1.2.tar` & `gpp_components-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 02:00:37.175449 gpp_components-0.1.2/
--rw-rw-rw-   0        0        0     1097 2023-11-13 03:12:05.000000 gpp_components-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      412 2024-04-16 02:00:37.168921 gpp_components-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       58 2023-11-13 03:12:05.000000 gpp_components-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 02:00:37.085574 gpp_components-0.1.2/gpp_components/
--rw-rw-rw-   0        0        0       19 2023-12-26 05:13:21.000000 gpp_components-0.1.2/gpp_components/__init__.py
--rw-rw-rw-   0        0        0     1076 2023-12-26 05:13:21.000000 gpp_components-0.1.2/gpp_components/aes.py
--rw-rw-rw-   0        0        0      239 2024-02-22 03:46:53.000000 gpp_components-0.1.2/gpp_components/constant.py
--rw-rw-rw-   0        0        0     4442 2023-12-26 05:13:21.000000 gpp_components-0.1.2/gpp_components/dbConfig.py
--rw-rw-rw-   0        0        0     2535 2024-04-16 01:08:29.000000 gpp_components-0.1.2/gpp_components/decorator.py
--rw-rw-rw-   0        0        0     9366 2024-04-16 02:00:09.000000 gpp_components-0.1.2/gpp_components/fileImporter.py
--rw-rw-rw-   0        0        0     7696 2024-04-16 01:08:29.000000 gpp_components-0.1.2/gpp_components/handleData.py
--rw-rw-rw-   0        0        0     1629 2023-12-26 05:13:21.000000 gpp_components-0.1.2/gpp_components/lazyImport.py
--rw-rw-rw-   0        0        0     1422 2024-03-20 05:27:27.000000 gpp_components-0.1.2/gpp_components/response.py
--rw-rw-rw-   0        0        0     5115 2024-04-16 01:33:35.000000 gpp_components-0.1.2/gpp_components/runOracle.py
--rw-rw-rw-   0        0        0     2880 2023-12-26 05:13:21.000000 gpp_components-0.1.2/gpp_components/sendMail.py
-drwxrwxrwx   0        0        0        0 2024-04-16 02:00:37.157002 gpp_components-0.1.2/gpp_components.egg-info/
--rw-rw-rw-   0        0        0      412 2024-04-16 02:00:35.000000 gpp_components-0.1.2/gpp_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      517 2024-04-16 02:00:35.000000 gpp_components-0.1.2/gpp_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 02:00:35.000000 gpp_components-0.1.2/gpp_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-16 02:00:35.000000 gpp_components-0.1.2/gpp_components.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-16 02:00:35.000000 gpp_components-0.1.2/gpp_components.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 02:00:37.178020 gpp_components-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      877 2024-04-16 02:00:19.000000 gpp_components-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:43:32.665585 gpp_components-0.1.3/
+-rw-rw-rw-   0        0        0     1097 2024-01-24 04:54:41.000000 gpp_components-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      412 2024-04-17 06:43:32.657586 gpp_components-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       58 2024-01-24 04:54:41.000000 gpp_components-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 06:43:32.470559 gpp_components-0.1.3/gpp_components/
+-rw-rw-rw-   0        0        0       19 2024-01-24 04:54:41.000000 gpp_components-0.1.3/gpp_components/__init__.py
+-rw-rw-rw-   0        0        0     1076 2024-01-24 04:54:41.000000 gpp_components-0.1.3/gpp_components/aes.py
+-rw-rw-rw-   0        0        0      239 2024-01-26 05:10:34.000000 gpp_components-0.1.3/gpp_components/constant.py
+-rw-rw-rw-   0        0        0     4442 2024-01-24 04:54:41.000000 gpp_components-0.1.3/gpp_components/dbConfig.py
+-rw-rw-rw-   0        0        0     2535 2024-04-02 12:30:35.000000 gpp_components-0.1.3/gpp_components/decorator.py
+-rw-rw-rw-   0        0        0     9366 2024-04-17 06:41:00.000000 gpp_components-0.1.3/gpp_components/fileImporter.py
+-rw-rw-rw-   0        0        0     7692 2024-04-17 06:42:48.000000 gpp_components-0.1.3/gpp_components/handleData.py
+-rw-rw-rw-   0        0        0     1629 2024-01-24 04:54:41.000000 gpp_components-0.1.3/gpp_components/lazyImport.py
+-rw-rw-rw-   0        0        0     1422 2024-03-04 01:22:22.000000 gpp_components-0.1.3/gpp_components/response.py
+-rw-rw-rw-   0        0        0     5115 2024-04-17 06:41:00.000000 gpp_components-0.1.3/gpp_components/runOracle.py
+-rw-rw-rw-   0        0        0     2880 2024-01-24 04:54:41.000000 gpp_components-0.1.3/gpp_components/sendMail.py
+drwxrwxrwx   0        0        0        0 2024-04-17 06:43:32.622683 gpp_components-0.1.3/gpp_components.egg-info/
+-rw-rw-rw-   0        0        0      412 2024-04-17 06:43:31.000000 gpp_components-0.1.3/gpp_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      517 2024-04-17 06:43:31.000000 gpp_components-0.1.3/gpp_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 06:43:31.000000 gpp_components-0.1.3/gpp_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-17 06:43:31.000000 gpp_components-0.1.3/gpp_components.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-17 06:43:31.000000 gpp_components-0.1.3/gpp_components.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 06:43:32.669591 gpp_components-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      876 2024-04-17 06:42:48.000000 gpp_components-0.1.3/setup.py
```

### Comparing `gpp_components-0.1.2/LICENSE` & `gpp_components-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.2/gpp_components/aes.py` & `gpp_components-0.1.3/gpp_components/aes.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.2/gpp_components/dbConfig.py` & `gpp_components-0.1.3/gpp_components/dbConfig.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.2/gpp_components/decorator.py` & `gpp_components-0.1.3/gpp_components/decorator.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.2/gpp_components/fileImporter.py` & `gpp_components-0.1.3/gpp_components/fileImporter.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.2/gpp_components/handleData.py` & `gpp_components-0.1.3/gpp_components/handleData.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from django.db.models import Q  # 不要拿掉
 from jsonpath import jsonpath
 from django.core.paginator import Paginator
 
 
 class HandleData(Constant):
     def get_(
-        self, table_name, conditions={}, page_size=None, current_page=None, sort=None
+        self, table_name, conditions={}, page_size=None, current_page=None, sort=[]
     ):
         # table_name = kwargs.get("table_name")
         # condition = {} if not kwargs.get("condition")
         name_type = "db_table" if not "." in table_name else "verbose_name"
 
         if len(list(conditions.keys())) == 0:
             conditions = {"data": [{}]}
@@ -24,16 +24,16 @@
         condition = strConditions(formatConditions(conditions))
 
         for model in apps.get_models():
             if model._meta.app_label == self.app_name:
                 if model._meta.__getattribute__(name_type) == table_name:
                     models = model.objects.filter(eval(condition))
                     qs = models.all().values()
-                    if not sort == None:
-                        qs = qs.order_by(sort)
+                    if len(sort) > 0:
+                        qs = qs.order_by(*sort)
                     if page_size == None:
                         return Response(data=list(qs))
                     else:
                         # 创建Paginator对象并指定每页显示的记录数量
                         paginator = Paginator(list(qs), per_page=page_size)
                         page = paginator.get_page(current_page)
```

### Comparing `gpp_components-0.1.2/gpp_components/lazyImport.py` & `gpp_components-0.1.3/gpp_components/lazyImport.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.2/gpp_components/response.py` & `gpp_components-0.1.3/gpp_components/response.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.2/gpp_components/runOracle.py` & `gpp_components-0.1.3/gpp_components/runOracle.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.2/gpp_components/sendMail.py` & `gpp_components-0.1.3/gpp_components/sendMail.py`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.2/gpp_components.egg-info/SOURCES.txt` & `gpp_components-0.1.3/gpp_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpp_components-0.1.2/setup.py` & `gpp_components-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import os, shutil
 
-os.chdir(r"D:\Coding\GPP-Vue\gpp-py-components")
-# os.chdir(r"D:\gitLab\gpp-py-components")
+#os.chdir(r"D:\Coding\GPP-Vue\gpp-py-components")
+os.chdir(r"D:\gitLab\gpp-py-components")
 dir_list = ["./build", "./dist", "./gpp_components.egg-info"]
 for i in dir_list:
     if os.path.exists(i):
         shutil.rmtree(i)
 
 
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="gpp_components",
-    version = '0.1.2',
+    version = '0.1.3',
     # version="0.0.36", # last version for Py310
     #
     author="L",
     description="for internal use",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT Licence",
```

