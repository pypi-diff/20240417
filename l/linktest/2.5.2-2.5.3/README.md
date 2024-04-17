# Comparing `tmp/linktest-2.5.2.tar.gz` & `tmp/linktest-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.5.2.tar", last modified: Tue Apr 16 07:43:02 2024, max compression
+gzip compressed data, was "linktest-2.5.3.tar", last modified: Tue Apr 16 09:15:37 2024, max compression
```

## Comparing `linktest-2.5.2.tar` & `linktest-2.5.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-16 07:43:02.179054 linktest-2.5.2/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-16 07:43:02.178594 linktest-2.5.2/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-16 07:43:02.175162 linktest-2.5.2/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-16 07:40:15.000000 linktest-2.5.2/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9940 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/detect_delimiter.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16523 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8530 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/generate_html_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    34730 2024-04-16 07:20:03.000000 linktest-2.5.2/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   105820 2024-04-16 07:35:33.000000 linktest-2.5.2/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/re_func.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8022 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-16 07:40:20.000000 linktest-2.5.2/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    11186 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/webdriver_wrapper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-16 07:15:29.000000 linktest-2.5.2/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-16 07:43:02.178166 linktest-2.5.2/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-16 07:43:01.000000 linktest-2.5.2/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1271 2024-04-16 07:43:02.000000 linktest-2.5.2/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-16 07:43:01.000000 linktest-2.5.2/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-16 07:43:01.000000 linktest-2.5.2/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-16 07:43:01.000000 linktest-2.5.2/linktest.egg-info/top_level.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-16 07:43:02.179106 linktest-2.5.2/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-16 07:42:56.000000 linktest-2.5.2/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-16 09:15:37.399645 linktest-2.5.3/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-16 09:15:37.399243 linktest-2.5.3/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-16 09:15:37.396526 linktest-2.5.3/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-16 09:11:18.000000 linktest-2.5.3/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10266 2024-04-16 08:28:08.000000 linktest-2.5.3/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/detect_delimiter.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16523 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10249 2024-04-16 08:58:04.000000 linktest-2.5.3/linktest/generate_html_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    34730 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   105820 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/re_func.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8022 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-16 09:11:23.000000 linktest-2.5.3/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    11186 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/webdriver_wrapper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-16 09:15:37.398630 linktest-2.5.3/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-16 09:15:37.000000 linktest-2.5.3/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1271 2024-04-16 09:15:37.000000 linktest-2.5.3/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-16 09:15:37.000000 linktest-2.5.3/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-16 09:15:37.000000 linktest-2.5.3/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-16 09:15:37.000000 linktest-2.5.3/linktest.egg-info/top_level.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-16 09:15:37.399699 linktest-2.5.3/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-16 09:15:30.000000 linktest-2.5.3/setup.py
```

### Comparing `linktest-2.5.2/linktest/appium_utils.py` & `linktest-2.5.3/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.2/linktest/auto_generate_testcase_list.py` & `linktest-2.5.3/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.2/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.5.3/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.2/linktest/base_testcase.py` & `linktest-2.5.3/linktest/base_testcase.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import logging
 import time
 import traceback
 import json
 
 # import threading
 # from .logged_requests import LoggedRequests
@@ -193,18 +194,20 @@
                 "name": "IKEA",
                 "No": 1
             }
         }
         """
 
         self.logger.info("========================= Compare JSON Objects =========================")
-        self.logger.info("Expected JSON: ")
-        self.logger.info(self.pformat(expected_json))
-        self.logger.info("Actual json: ")
-        self.logger.info(self.pformat(actual_json))
+        # self.logger.info("Expected JSON: "+ os.linesep + self.pformat(expected_json))
+        self.logger.info("Expected JSON: "+ os.linesep + json.dumps(expected_json, ensure_ascii=False, indent=2))
+        # self.logger.info(self.pformat(expected_json))
+        # self.logger.info("Actual json: "+ os.linesep + self.pformat(actual_json))
+        self.logger.info("Expected JSON: "+ os.linesep + json.dumps(actual_json, ensure_ascii=False, indent=2))
+        # self.logger.info(self.pformat(actual_json))
 
         if rules:
             self.logger.info("Compare Rules:")
             self.logger.info(rules)
 
         diff = Compare(rules=rules).check(expected_json, actual_json)
         self.logger.info("========================= JSON diff ========================= ")
```

### Comparing `linktest-2.5.2/linktest/clean_data.py` & `linktest-2.5.3/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.2/linktest/conver_xml_into_db.py` & `linktest-2.5.3/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.2/linktest/database_helper.py` & `linktest-2.5.3/linktest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.2/linktest/date_utilities.py` & `linktest-2.5.3/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.2/linktest/doctor.py` & `linktest-2.5.3/linktest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.2/linktest/framework_log.py` & `linktest-2.5.3/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.2/linktest/get_adb_devices.py` & `linktest-2.5.3/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.2/linktest/get_ios_devices_list.py` & `linktest-2.5.3/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.2/linktest/get_platform_info.py` & `linktest-2.5.3/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.2/linktest/get_project_info.py` & `linktest-2.5.3/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.2/linktest/html_report.py` & `linktest-2.5.3/linktest/html_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.2/linktest/logged_requests.py` & `linktest-2.5.3/linktest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.2/linktest/main.py` & `linktest-2.5.3/linktest/main.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.2/linktest/memory_usage.py` & `linktest-2.5.3/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.2/linktest/re_func.py` & `linktest-2.5.3/linktest/re_func.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.2/linktest/run.py` & `linktest-2.5.3/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.2/linktest/run_testcase_thread.py` & `linktest-2.5.3/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.2/linktest/scp_report_to_specified_path.py` & `linktest-2.5.3/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.2/linktest/selenium_helper.py` & `linktest-2.5.3/linktest/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.2/linktest/timeout_thread.py` & `linktest-2.5.3/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.2/linktest/ui_testcase.py` & `linktest-2.5.3/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.2/linktest/update_config.py` & `linktest-2.5.3/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.2/linktest/webdriver_wrapper.py` & `linktest-2.5.3/linktest/webdriver_wrapper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.2/linktest/xml_report.py` & `linktest-2.5.3/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.2/linktest.egg-info/SOURCES.txt` & `linktest-2.5.3/linktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

