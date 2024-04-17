# Comparing `tmp/linktest-2.5.4.tar.gz` & `tmp/linktest-2.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.5.4.tar", last modified: Wed Apr 17 05:56:48 2024, max compression
+gzip compressed data, was "linktest-2.5.5.tar", last modified: Wed Apr 17 06:42:40 2024, max compression
```

## Comparing `linktest-2.5.4.tar` & `linktest-2.5.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-17 05:56:48.568931 linktest-2.5.4/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-17 05:56:48.568054 linktest-2.5.4/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-17 05:56:48.565050 linktest-2.5.4/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-17 05:52:21.000000 linktest-2.5.4/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-04-17 05:53:16.000000 linktest-2.5.4/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/detect_delimiter.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16523 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    12705 2024-04-17 05:40:41.000000 linktest-2.5.4/linktest/generate_html_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    34732 2024-04-17 03:17:24.000000 linktest-2.5.4/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   105788 2024-04-17 05:38:51.000000 linktest-2.5.4/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/re_func.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8022 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-17 05:52:27.000000 linktest-2.5.4/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    11186 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/webdriver_wrapper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-17 05:56:48.567658 linktest-2.5.4/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-17 05:56:48.000000 linktest-2.5.4/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1271 2024-04-17 05:56:48.000000 linktest-2.5.4/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-17 05:56:48.000000 linktest-2.5.4/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-17 05:56:48.000000 linktest-2.5.4/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-17 05:56:48.000000 linktest-2.5.4/linktest.egg-info/top_level.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-17 05:56:48.568992 linktest-2.5.4/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-17 05:56:42.000000 linktest-2.5.4/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-17 06:42:40.080793 linktest-2.5.5/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-17 06:42:40.080451 linktest-2.5.5/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-17 06:42:40.077258 linktest-2.5.5/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-17 06:37:53.000000 linktest-2.5.5/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/detect_delimiter.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16523 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    15476 2024-04-17 06:39:53.000000 linktest-2.5.5/linktest/generate_html_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    34732 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   105788 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/re_func.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8022 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-17 06:38:00.000000 linktest-2.5.5/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    11186 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/webdriver_wrapper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-17 06:06:05.000000 linktest-2.5.5/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-17 06:42:40.079980 linktest-2.5.5/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-17 06:42:39.000000 linktest-2.5.5/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1271 2024-04-17 06:42:39.000000 linktest-2.5.5/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-17 06:42:39.000000 linktest-2.5.5/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-17 06:42:39.000000 linktest-2.5.5/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-17 06:42:39.000000 linktest-2.5.5/linktest.egg-info/top_level.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-17 06:42:40.080850 linktest-2.5.5/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-17 06:42:33.000000 linktest-2.5.5/setup.py
```

### Comparing `linktest-2.5.4/linktest/appium_utils.py` & `linktest-2.5.5/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.4/linktest/auto_generate_testcase_list.py` & `linktest-2.5.5/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.4/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.5.5/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.4/linktest/base_testcase.py` & `linktest-2.5.5/linktest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.4/linktest/clean_data.py` & `linktest-2.5.5/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.4/linktest/conver_xml_into_db.py` & `linktest-2.5.5/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.4/linktest/database_helper.py` & `linktest-2.5.5/linktest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.4/linktest/date_utilities.py` & `linktest-2.5.5/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.4/linktest/doctor.py` & `linktest-2.5.5/linktest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.4/linktest/framework_log.py` & `linktest-2.5.5/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.4/linktest/generate_html_log.py` & `linktest-2.5.5/linktest/generate_html_log.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,47 @@
+# -*- coding: utf-8 -*-
+"""
+File: generate_html_log.py
+Author: Wang Lin
+Date: 2023-06-05
+Description:
+    该文件包含了将测试用例执行日志转换为HTML格式的函数。
+    主要功能包括:
+    1. 读取测试用例的日志文件。
+    2. 解析日志内容,提取关键信息如时间戳、日志级别等。
+    3. 将日志内容转换为HTML格式,并应用样式和颜色以增强可读性。
+    4. 处理特定的日志模式,如WebDriver操作、请求响应等,并对其进行高亮显示。
+    5. 将转换后的HTML内容写入文件,生成测试用例执行日志的HTML报告。
+
+Functions:
+    - starts_with_date(input_string: str) -> bool
+        判断字符串是否以YYYY-MM-DD格式的日期开头。
+
+    - is_logged_requests_line(line: str) -> bool
+        判断日志行是否为特定的logged_requests.py格式。
+
+    - format_json(json_string: str) -> str
+        格式化JSON字符串,使其在HTML中显示时更易读。
+
+    - generate_html_log(executing_testcase: object) -> None
+        生成测试用例执行日志的HTML报告。
+        接收一个表示正在执行的测试用例的对象作为参数。
+        读取测试用例的日志文件,将日志内容转换为HTML格式,并写入HTML文件。
+
+Dependencies:
+    - os: 用于文件和目录操作。
+    - re: 用于正则表达式匹配。
+    - json: 用于处理JSON数据。
+
+Notes:
+    - 该文件依赖于特定的测试框架和日志格式。
+    - HTML样式和布局可以根据需要进行自定义和调整。
+    - 生成的HTML报告文件名与原始日志文件名相同,扩展名为.html。
+"""
+
 import os
 import re
 import json
 
 def starts_with_date(input_string):
     # 正则表达式匹配 YYYY-MM-DD 格式的日期
     pattern = r'^\d{4}-\d{2}-\d{2}'
@@ -38,36 +78,49 @@
     parts = [part for part in executing_testcase.packages.split(',') if part]
     last_part = parts[-1] if parts else ''
 
     testcase_name_with_package = last_part + '.' + executing_testcase.logger.name
 
     testcase_status_info = ""
     if executing_testcase.ExecutionStatusSetByFramework == "failed":
-        testcase_status_info = '<h2><span style="color:red; padding: 8px;">Status: Failed</span><button style="color: red; font-size: large; height: auto; width: auto;" onclick="scrollToTraceback()">Scroll to Traceback</button></h2>'
+        testcase_status_info = '<span style="color:red; padding: 8px;">Status: Failed</span><button style="color: red; font-size: large; height: auto; width: auto;" onclick="scrollToTraceback()">Scroll to Traceback</button>'
     else:
-        testcase_status_info = '<h2 style="color:green; padding: 8px;">Status: Passed</h2>'
+        testcase_status_info = '<span style="color:green; padding: 8px;">Status: Passed</span>'
 
     # 构建HTML页面
     html_content = """
     <!DOCTYPE html>
     <html lang="en">
     <head>
         <meta charset="UTF-8">
         <title>Execution Log for TestCase</title>
         <style>
             body {
                 font-family: Arial, sans-serif;
                 background-color: #f4f4f4;
-                margin: 20px;
+                margin: 0;
                 padding: 0;
             }
+            .header {
+                position: fixed;
+                top: 0;
+                left: 0;
+                width: 100%%;
+                background-color: white;
+                padding: 0px;
+                box-shadow: 0 2px 4px rgba(0,0,0,0.1);
+                z-index: 1;
+            }
             .container {
+                margin-top: 120px;
+                margin-left: 20px;
+                margin-right: 20px;
+                padding: 20px;
                 background-color: white;
                 border: 1px solid #ddd;
-                padding: 20px;
                 border-radius: 8px;
                 box-shadow: 0 2px 4px rgba(0,0,0,0.1);
             }
             .log-entry {
                 margin-bottom: 10px;
                 padding: 10px;
                 background-color: #f9f9f9;
@@ -92,19 +145,20 @@
             .timestamp {
                 color: #666;
                 font-size: 14px;
             }
         </style>
     </head>
     <body>
-    
+        <div class="header">
+            <h1 style='padding-left: 25px;'>Execution Log for TestCase: %s</h1> 
+            <h2 style='padding-left: 22px;'>%s</h2>
+        </div>
         <div class="container">
-            <h1>Execution Log for TestCase: %s</h1> 
-            <b>%s</b>
-    """ % (testcase_name_with_package,  testcase_status_info)
+    """ % (testcase_name_with_package, testcase_status_info)
 
     lines = ""
     single_line_flag = False
     traceback_flag = False
 
     # 将日志行转换为HTML元素
     for line in execution_log:
@@ -135,15 +189,16 @@
         if "WebDriver Action:</span> <b style='color:#006600; font-size: 20px;'>'save_screenshot'</b> with <b style='color:#333333'>args</b>:" in line:
             line += "<img src='" + line.split("WebDriver Action:</span> <b style='color:#006600; font-size: 20px;'>'save_screenshot'</b> with <b style='color:#333333'>args</b>:")[1].strip() + "' width='100%'>"
 
         # if "logged_requests.py" in line:
         #     line = line.replace("logged_requests.py", "<span style='color:#0066CC'>logged_requests.py</span>")
 
         if "run_test() start" in line:
-            line = line.replace("run_test() start", "<strong style='color:#0066CC; font-size: 20px;'>run_test() start</strong>")
+            line = line.replace("run_test() start",
+                                "<strong style='color:#0066CC; font-size: 20px;'>run_test() start</strong>")
 
         if "setup() start" in line:
             line = line.replace("setup() start",
                                 "<strong style='color:#0066CC; font-size: 20px;'>setup() start</strong>")
 
         if "setup() end" in line:
             line = line.replace("setup() end",
@@ -161,71 +216,89 @@
             line = line.replace("cURL Start",
                                 "<strong style='color:#0066CC; font-size: 20px;'>cURL Start</strong>")
 
         if "cURL End" in line:
             line = line.replace("cURL End",
                                 "<strong style='color:#0066CC; font-size: 20px;'>cURL End</strong>")
 
-
         if " POST Request Started" in line:
-            line = line.replace(" POST Request Started", "<strong style='color:#0066CC; font-size: 20px;'> POST Request Started</strong>")
+            line = line.replace(" POST Request Started",
+                                "<strong style='color:#0066CC; font-size: 20px;'> POST Request Started</strong>")
 
         if " POST Response:" in line:
-            line = line.replace(" POST Response:", "<strong style='color:#0066CC; font-size: 20px;'> POST Response:</strong>")
+            line = line.replace(" POST Response:",
+                                "<strong style='color:#0066CC; font-size: 20px;'> POST Response:</strong>")
 
         if "POST Request Completed" in line:
-            line = line.replace("POST Request Completed", "<strong style='color:#0066CC; font-size: 20px;'>POST Request Completed</strong>")
+            line = line.replace("POST Request Completed",
+                                "<strong style='color:#0066CC; font-size: 20px;'>POST Request Completed</strong>")
 
         if "GET Request Started" in line:
-            line = line.replace("GET Request Started", "<strong style='color:#0066CC; font-size: 20px;'>GET Request Started</strong>")
+            line = line.replace("GET Request Started",
+                                "<strong style='color:#0066CC; font-size: 20px;'>GET Request Started</strong>")
 
         if "GET Response" in line:
-            line = line.replace("GET Response", "<strong style='color:#0066CC; font-size: 20px;'>GET Response</strong>")
+            line = line.replace("GET Response",
+                                "<strong style='color:#0066CC; font-size: 20px;'>GET Response</strong>")
 
         if "GET Request Completed" in line:
-            line = line.replace("GET Request Completed", "<strong style='color:#0066CC; font-size: 20px;'>GET Request Completed</strong>")
+            line = line.replace("GET Request Completed",
+                                "<strong style='color:#0066CC; font-size: 20px;'>GET Request Completed</strong>")
 
         if "Test Execution Environment:" in line:
-            line = line.replace("Test Execution Environment:", "<strong style='color:#0066CC; font-size: 20px;'>Test Execution Environment:</strong>")
+            line = line.replace("Test Execution Environment:",
+                                "<strong style='color:#0066CC; font-size: 20px;'>Test Execution Environment:</strong>")
 
         if "Response [200]" in line:
-            line = line.replace("Response [200]", "<strong style='color:green; font-size: 20px;'>Response [200]</strong>")
+            line = line.replace("Response [200]",
+                                "<strong style='color:green; font-size: 20px;'>Response [200]</strong>")
 
         if "Response [201]" in line:
-            line = line.replace("Response [201]", "<strong style='color:green; font-size: 20px;'>Response [201]</strong>")
+            line = line.replace("Response [201]",
+                                "<strong style='color:green; font-size: 20px;'>Response [201]</strong>")
 
         if "Response [400]" in line:
-            line = line.replace("Response [400]", "<strong style='color:red; font-size: 20px;'>Response [400]</strong>")
+            line = line.replace("Response [400]",
+                                "<strong style='color:red; font-size: 20px;'>Response [400]</strong>")
 
         if "Response [401]" in line:
-            line = line.replace("Response [401]", "<strong style='color:red; font-size: 20px;'>Response [401]</strong>")
+            line = line.replace("Response [401]",
+                                "<strong style='color:red; font-size: 20px;'>Response [401]</strong>")
 
         if "Response [403]" in line:
-            line = line.replace("Response [403]", "<strong style='color:red; font-size: 20px;'>Response [403]</strong>")
+            line = line.replace("Response [403]",
+                                "<strong style='color:red; font-size: 20px;'>Response [403]</strong>")
 
         if "Response [404]" in line:
-            line = line.replace("Response [404]", "<strong style='color:red; font-size: 20px;'>Response [404]</strong>")
+            line = line.replace("Response [404]",
+                                "<strong style='color:red; font-size: 20px;'>Response [404]</strong>")
 
         if "Response [500]" in line:
-            line = line.replace("Response [500]", "<strong style='color:red; font-size: 20px;'>Response [500]</strong>")
+            line = line.replace("Response [500]",
+                                "<strong style='color:red; font-size: 20px;'>Response [500]</strong>")
 
         if "Response [502]" in line:
-            line = line.replace("Response [502]", "<strong style='color:red; font-size: 20px;'>Response [502]</strong>")
+            line = line.replace("Response [502]",
+                                "<strong style='color:red; font-size: 20px;'>Response [502]</strong>")
 
         if "Response [503]" in line:
-            line = line.replace("Response [503]", "<strong style='color:red; font-size: 20px;'>Response [503]</strong>")
+            line = line.replace("Response [503]",
+                                "<strong style='color:red; font-size: 20px;'>Response [503]</strong>")
 
         if "Response [504]" in line:
-            line = line.replace("Response [504]", "<strong style='color:red; font-size: 20px;'>Response [504]</strong>")
+            line = line.replace("Response [504]",
+                                "<strong style='color:red; font-size: 20px;'>Response [504]</strong>")
 
         if "Assertion Passed:" in line:
-            line = line.replace("Assertion Passed:", "<strong style='color:green; font-size: 20px;'>Assertion Passed:</strong>")
+            line = line.replace("Assertion Passed:",
+                                "<strong style='color:green; font-size: 20px;'>Assertion Passed:</strong>")
 
         if "Assertion Failed:" in line:
-            line = line.replace("Assertion Failed:", "<strong style='color:red; font-size: 20px;'>Assertion Failed:</strong>")
+            line = line.replace("Assertion Failed:",
+                                "<strong style='color:red; font-size: 20px;'>Assertion Failed:</strong>")
 
         if "logged_requests.py" in line:
             if "URL:" in line and "logged_requests.py" in line.split("URL:")[0]:
                 line = line.replace("URL:", f"<strong style='color:#0066CC; font-size: 20px;'>URL:</strong>")
             if "JSON:" in line and "logged_requests.py" in line.split("JSON:")[0]:
                 line = line.replace("JSON:",f"<strong style='color:#0066CC; font-size: 20px;'>JSON:</strong>")
             if "kwargs:" in line and "logged_requests.py" in line.split("kwargs:")[0]:
```

### Comparing `linktest-2.5.4/linktest/get_adb_devices.py` & `linktest-2.5.5/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.4/linktest/get_ios_devices_list.py` & `linktest-2.5.5/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.4/linktest/get_platform_info.py` & `linktest-2.5.5/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.4/linktest/get_project_info.py` & `linktest-2.5.5/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.4/linktest/html_report.py` & `linktest-2.5.5/linktest/html_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.4/linktest/logged_requests.py` & `linktest-2.5.5/linktest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.4/linktest/main.py` & `linktest-2.5.5/linktest/main.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.4/linktest/memory_usage.py` & `linktest-2.5.5/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.4/linktest/re_func.py` & `linktest-2.5.5/linktest/re_func.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.4/linktest/run.py` & `linktest-2.5.5/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.4/linktest/run_testcase_thread.py` & `linktest-2.5.5/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.4/linktest/scp_report_to_specified_path.py` & `linktest-2.5.5/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.4/linktest/selenium_helper.py` & `linktest-2.5.5/linktest/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.4/linktest/timeout_thread.py` & `linktest-2.5.5/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.4/linktest/ui_testcase.py` & `linktest-2.5.5/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.4/linktest/update_config.py` & `linktest-2.5.5/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.4/linktest/webdriver_wrapper.py` & `linktest-2.5.5/linktest/webdriver_wrapper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.4/linktest/xml_report.py` & `linktest-2.5.5/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.4/linktest.egg-info/SOURCES.txt` & `linktest-2.5.5/linktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

