# Comparing `tmp/lqbox-2.6.0.tar.gz` & `tmp/lqbox-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lqbox-2.6.0.tar", max compression
+gzip compressed data, was "lqbox-2.7.0.tar", max compression
```

## Comparing `lqbox-2.6.0.tar` & `lqbox-2.7.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1091 2024-03-20 09:46:12.799882 lqbox-2.6.0/LICENSE
--rw-r--r--   0        0        0      322 2024-04-11 07:23:14.076378 lqbox-2.6.0/pyproject.toml
--rw-r--r--   0        0        0       30 2024-03-20 09:46:12.799882 lqbox-2.6.0/README.md
--rw-r--r--   0        0        0      143 2024-03-20 09:46:12.801882 lqbox-2.6.0/src/lqbox/__init__.py
--rw-r--r--   0        0        0     2705 2024-04-09 01:53:28.324154 lqbox-2.6.0/src/lqbox/ali/__init__.py
--rw-r--r--   0        0        0     1289 2024-03-20 09:46:12.801882 lqbox-2.6.0/src/lqbox/base/__init__.py
--rw-r--r--   0        0        0     2970 2024-04-10 08:12:43.668992 lqbox-2.6.0/src/lqbox/bidp/__init__.py
--rw-r--r--   0        0        0     2975 2024-03-20 09:46:12.802882 lqbox-2.6.0/src/lqbox/elihu/__init__.py
--rw-r--r--   0        0        0     1834 2024-03-20 09:46:12.802882 lqbox-2.6.0/src/lqbox/mc/__init__.py
--rw-r--r--   0        0        0     2421 2024-04-11 07:20:15.936012 lqbox-2.6.0/src/lqbox/oc/__init__.py
--rw-r--r--   0        0        0     2324 2024-03-20 09:46:12.803882 lqbox-2.6.0/src/lqbox/open_bidp/__init__.py
--rw-r--r--   0        0        0     3803 2024-03-20 09:46:12.803882 lqbox-2.6.0/src/lqbox/open_elihu/__init__.py
--rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 lqbox-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-03-20 09:46:12.799882 lqbox-2.7.0/LICENSE
+-rw-r--r--   0        0        0      322 2024-04-17 09:22:35.882463 lqbox-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0       30 2024-03-20 09:46:12.799882 lqbox-2.7.0/README.md
+-rw-r--r--   0        0        0      143 2024-03-20 09:46:12.801882 lqbox-2.7.0/src/lqbox/__init__.py
+-rw-r--r--   0        0        0     2705 2024-04-09 01:53:28.324154 lqbox-2.7.0/src/lqbox/ali/__init__.py
+-rw-r--r--   0        0        0     1289 2024-03-20 09:46:12.801882 lqbox-2.7.0/src/lqbox/base/__init__.py
+-rw-r--r--   0        0        0     2970 2024-04-10 08:12:43.668992 lqbox-2.7.0/src/lqbox/bidp/__init__.py
+-rw-r--r--   0        0        0     2975 2024-03-20 09:46:12.802882 lqbox-2.7.0/src/lqbox/elihu/__init__.py
+-rw-r--r--   0        0        0     1834 2024-03-20 09:46:12.802882 lqbox-2.7.0/src/lqbox/mc/__init__.py
+-rw-r--r--   0        0        0     2421 2024-04-11 07:20:15.936012 lqbox-2.7.0/src/lqbox/oc/__init__.py
+-rw-r--r--   0        0        0     2324 2024-03-20 09:46:12.803882 lqbox-2.7.0/src/lqbox/open_bidp/__init__.py
+-rw-r--r--   0        0        0     4031 2024-04-17 09:22:35.887463 lqbox-2.7.0/src/lqbox/open_elihu/__init__.py
+-rw-r--r--   0        0        0      710 1970-01-01 00:00:00.000000 lqbox-2.7.0/PKG-INFO
```

### Comparing `lqbox-2.6.0/LICENSE` & `lqbox-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lqbox-2.6.0/src/lqbox/ali/__init__.py` & `lqbox-2.7.0/src/lqbox/ali/__init__.py`

 * *Files identical despite different names*

### Comparing `lqbox-2.6.0/src/lqbox/base/__init__.py` & `lqbox-2.7.0/src/lqbox/base/__init__.py`

 * *Files identical despite different names*

### Comparing `lqbox-2.6.0/src/lqbox/bidp/__init__.py` & `lqbox-2.7.0/src/lqbox/bidp/__init__.py`

 * *Files identical despite different names*

### Comparing `lqbox-2.6.0/src/lqbox/elihu/__init__.py` & `lqbox-2.7.0/src/lqbox/elihu/__init__.py`

 * *Files identical despite different names*

### Comparing `lqbox-2.6.0/src/lqbox/mc/__init__.py` & `lqbox-2.7.0/src/lqbox/mc/__init__.py`

 * *Files identical despite different names*

### Comparing `lqbox-2.6.0/src/lqbox/oc/__init__.py` & `lqbox-2.7.0/src/lqbox/oc/__init__.py`

 * *Files identical despite different names*

### Comparing `lqbox-2.6.0/src/lqbox/open_bidp/__init__.py` & `lqbox-2.7.0/src/lqbox/open_bidp/__init__.py`

 * *Files identical despite different names*

### Comparing `lqbox-2.6.0/src/lqbox/open_elihu/__init__.py` & `lqbox-2.7.0/src/lqbox/open_elihu/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,14 +71,18 @@
             {'account_id_list': account_id_list, 'platform_code': platform_code}
         )
 
     def call_get_count_of_special_cookie(self, name: str):
         """获取特殊cookie的数量"""
         return self.request_open_api('KaiwaOpenApiController/getCountOfSpecialCookie', {'name': name})
 
+    def call_get_count_of_unused_valid_special_cookie(self, name: str):
+        return self.request_open_api('KaiwaOpenApiController/getUnusedCountOfValidSpecialCookie',
+                                     {'name': name})
+
     def call_request_one_time_shovel_task(
             self,
             task_title: str,
             target_machine: str,
             shovel_project: str,
             shovel_class: str,
             shovel_extra: dict = None,
```

### Comparing `lqbox-2.6.0/PKG-INFO` & `lqbox-2.7.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lqbox
-Version: 2.6.0
+Version: 2.7.0
 Summary: lqbox
 License: MIT
 Author: luke9012
 Author-email: luke781520097@163.com
 Requires-Python: >=3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

