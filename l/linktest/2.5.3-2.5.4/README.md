# Comparing `tmp/linktest-2.5.3.tar.gz` & `tmp/linktest-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.5.3.tar", last modified: Tue Apr 16 09:15:37 2024, max compression
+gzip compressed data, was "linktest-2.5.4.tar", last modified: Wed Apr 17 05:56:48 2024, max compression
```

## Comparing `linktest-2.5.3.tar` & `linktest-2.5.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-16 09:15:37.399645 linktest-2.5.3/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-16 09:15:37.399243 linktest-2.5.3/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-16 09:15:37.396526 linktest-2.5.3/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-16 09:11:18.000000 linktest-2.5.3/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10266 2024-04-16 08:28:08.000000 linktest-2.5.3/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/detect_delimiter.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16523 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10249 2024-04-16 08:58:04.000000 linktest-2.5.3/linktest/generate_html_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    34730 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   105820 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/re_func.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8022 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-16 09:11:23.000000 linktest-2.5.3/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    11186 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/webdriver_wrapper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-16 07:43:25.000000 linktest-2.5.3/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-16 09:15:37.398630 linktest-2.5.3/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-16 09:15:37.000000 linktest-2.5.3/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1271 2024-04-16 09:15:37.000000 linktest-2.5.3/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-16 09:15:37.000000 linktest-2.5.3/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-16 09:15:37.000000 linktest-2.5.3/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-16 09:15:37.000000 linktest-2.5.3/linktest.egg-info/top_level.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-16 09:15:37.399699 linktest-2.5.3/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-16 09:15:30.000000 linktest-2.5.3/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-17 05:56:48.568931 linktest-2.5.4/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-17 05:56:48.568054 linktest-2.5.4/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-17 05:56:48.565050 linktest-2.5.4/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-17 05:52:21.000000 linktest-2.5.4/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-04-17 05:53:16.000000 linktest-2.5.4/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/detect_delimiter.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16523 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    12705 2024-04-17 05:40:41.000000 linktest-2.5.4/linktest/generate_html_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    34732 2024-04-17 03:17:24.000000 linktest-2.5.4/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   105788 2024-04-17 05:38:51.000000 linktest-2.5.4/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/re_func.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8022 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-17 05:52:27.000000 linktest-2.5.4/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    11186 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/webdriver_wrapper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-16 09:16:20.000000 linktest-2.5.4/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-17 05:56:48.567658 linktest-2.5.4/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-17 05:56:48.000000 linktest-2.5.4/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1271 2024-04-17 05:56:48.000000 linktest-2.5.4/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-17 05:56:48.000000 linktest-2.5.4/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-17 05:56:48.000000 linktest-2.5.4/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-17 05:56:48.000000 linktest-2.5.4/linktest.egg-info/top_level.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-17 05:56:48.568992 linktest-2.5.4/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-17 05:56:42.000000 linktest-2.5.4/setup.py
```

### Comparing `linktest-2.5.3/linktest/appium_utils.py` & `linktest-2.5.4/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.3/linktest/auto_generate_testcase_list.py` & `linktest-2.5.4/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.3/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.5.4/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.3/linktest/base_testcase.py` & `linktest-2.5.4/linktest/base_testcase.py`

 * *Files 4% similar despite different names*

```diff
@@ -194,20 +194,16 @@
                 "name": "IKEA",
                 "No": 1
             }
         }
         """
 
         self.logger.info("========================= Compare JSON Objects =========================")
-        # self.logger.info("Expected JSON: "+ os.linesep + self.pformat(expected_json))
         self.logger.info("Expected JSON: "+ os.linesep + json.dumps(expected_json, ensure_ascii=False, indent=2))
-        # self.logger.info(self.pformat(expected_json))
-        # self.logger.info("Actual json: "+ os.linesep + self.pformat(actual_json))
         self.logger.info("Expected JSON: "+ os.linesep + json.dumps(actual_json, ensure_ascii=False, indent=2))
-        # self.logger.info(self.pformat(actual_json))
 
         if rules:
             self.logger.info("Compare Rules:")
             self.logger.info(rules)
 
         diff = Compare(rules=rules).check(expected_json, actual_json)
         self.logger.info("========================= JSON diff ========================= ")
```

### Comparing `linktest-2.5.3/linktest/clean_data.py` & `linktest-2.5.4/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.3/linktest/conver_xml_into_db.py` & `linktest-2.5.4/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.3/linktest/database_helper.py` & `linktest-2.5.4/linktest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.3/linktest/date_utilities.py` & `linktest-2.5.4/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.3/linktest/doctor.py` & `linktest-2.5.4/linktest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.3/linktest/framework_log.py` & `linktest-2.5.4/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.3/linktest/generate_html_log.py` & `linktest-2.5.4/linktest/generate_html_log.py`

 * *Files 22% similar despite different names*

```diff
@@ -36,14 +36,20 @@
         execution_log = logfile.readlines()
 
     parts = [part for part in executing_testcase.packages.split(',') if part]
     last_part = parts[-1] if parts else ''
 
     testcase_name_with_package = last_part + '.' + executing_testcase.logger.name
 
+    testcase_status_info = ""
+    if executing_testcase.ExecutionStatusSetByFramework == "failed":
+        testcase_status_info = '<h2><span style="color:red; padding: 8px;">Status: Failed</span><button style="color: red; font-size: large; height: auto; width: auto;" onclick="scrollToTraceback()">Scroll to Traceback</button></h2>'
+    else:
+        testcase_status_info = '<h2 style="color:green; padding: 8px;">Status: Passed</h2>'
+
     # 构建HTML页面
     html_content = """
     <!DOCTYPE html>
     <html lang="en">
     <head>
         <meta charset="UTF-8">
         <title>Execution Log for TestCase</title>
@@ -86,17 +92,19 @@
             .timestamp {
                 color: #666;
                 font-size: 14px;
             }
         </style>
     </head>
     <body>
+    
         <div class="container">
-            <h1>Execution Log for TestCase: %s</h1>
-    """ % testcase_name_with_package
+            <h1>Execution Log for TestCase: %s</h1> 
+            <b>%s</b>
+    """ % (testcase_name_with_package,  testcase_status_info)
 
     lines = ""
     single_line_flag = False
     traceback_flag = False
 
     # 将日志行转换为HTML元素
     for line in execution_log:
@@ -109,106 +117,132 @@
         elif "INFO" in line:
             class_name += " info"
             cls_name_only_time_Log_entry += " info"
 
         if "WebDriver Action:" in line:
             action_name = line.split("'")[1]
             line = line.replace("WebDriver Action:", "<span style='color:#0066CC'>WebDriver Action:</span>")
-            line = line.replace(f"'{action_name}'", f"<b style='color:#006600'>'{action_name}'</b>")
+            line = line.replace(f"'{action_name}'", f"<b style='color:#006600; font-size: 20px;'>'{action_name}'</b>")
             if "args" in line:
                 line = line.replace("args", "<b style='color:#333333'>args</b>")
 
         if "WebElement Action:" in line:
             action_name = line.split("'")[1]
             line = line.replace("WebElement Action:", "<span style='color:#0066CC'>WebElement Action:</span>")
-            line = line.replace(f"'{action_name}'", f"<b style='color:#006600'>'{action_name}'</b>")
+            line = line.replace(f"'{action_name}'", f"<b style='color:#006600; font-size: 20px;'>'{action_name}'</b>")
             if "args" in line:
                 line = line.replace("args", "<b style='color:#333333'>args</b>")
 
-        if "WebDriver Action:</span> <b style='color:#006600'>'save_screenshot'</b> with <b style='color:#333333'>args</b>:" in line:
-            line += "<img src='" + line.split("WebDriver Action:</span> <b style='color:#006600'>'save_screenshot'</b> with <b style='color:#333333'>args</b>:")[1].strip() + "' width='100%'>"
+        if "WebDriver Action:</span> <b style='color:#006600; font-size: 20px;'>'save_screenshot'</b> with <b style='color:#333333'>args</b>:" in line:
+            line += "<img src='" + line.split("WebDriver Action:</span> <b style='color:#006600; font-size: 20px;'>'save_screenshot'</b> with <b style='color:#333333'>args</b>:")[1].strip() + "' width='100%'>"
 
         # if "logged_requests.py" in line:
         #     line = line.replace("logged_requests.py", "<span style='color:#0066CC'>logged_requests.py</span>")
 
-        if "run_test() Start" in line:
-            line = line.replace("run_test() Start", "<strong style='color:#0066CC'>run_test() Start</strong>")
+        if "run_test() start" in line:
+            line = line.replace("run_test() start", "<strong style='color:#0066CC; font-size: 20px;'>run_test() start</strong>")
+
+        if "setup() start" in line:
+            line = line.replace("setup() start",
+                                "<strong style='color:#0066CC; font-size: 20px;'>setup() start</strong>")
+
+        if "setup() end" in line:
+            line = line.replace("setup() end",
+                                "<strong style='color:#0066CC; font-size: 20px;'>setup() end</strong>")
+
+        if "teardown() start" in line:
+            line = line.replace("teardown() start",
+                                "<strong style='color:#0066CC; font-size: 20px;'>teardown() start</strong>")
+
+        if "teardown() end" in line:
+            line = line.replace("teardown() end",
+                                "<strong style='color:#0066CC; font-size: 20px;'>teardown() end</strong>")
+
+        if "cURL Start" in line:
+            line = line.replace("cURL Start",
+                                "<strong style='color:#0066CC; font-size: 20px;'>cURL Start</strong>")
+
+        if "cURL End" in line:
+            line = line.replace("cURL End",
+                                "<strong style='color:#0066CC; font-size: 20px;'>cURL End</strong>")
+
 
         if " POST Request Started" in line:
-            line = line.replace(" POST Request Started", "<strong style='color:#0066CC'> POST Request Started</strong>")
+            line = line.replace(" POST Request Started", "<strong style='color:#0066CC; font-size: 20px;'> POST Request Started</strong>")
 
         if " POST Response:" in line:
-            line = line.replace(" POST Response:", "<strong style='color:#0066CC'> POST Response:</strong>")
+            line = line.replace(" POST Response:", "<strong style='color:#0066CC; font-size: 20px;'> POST Response:</strong>")
 
         if "POST Request Completed" in line:
-            line = line.replace("POST Request Completed", "<strong style='color:#0066CC'>POST Request Completed</strong>")
+            line = line.replace("POST Request Completed", "<strong style='color:#0066CC; font-size: 20px;'>POST Request Completed</strong>")
 
         if "GET Request Started" in line:
-            line = line.replace("GET Request Started", "<strong style='color:#0066CC'>GET Request Started</strong>")
+            line = line.replace("GET Request Started", "<strong style='color:#0066CC; font-size: 20px;'>GET Request Started</strong>")
 
         if "GET Response" in line:
-            line = line.replace("GET Response", "<strong style='color:#0066CC'>GET Response</strong>")
+            line = line.replace("GET Response", "<strong style='color:#0066CC; font-size: 20px;'>GET Response</strong>")
 
         if "GET Request Completed" in line:
-            line = line.replace("GET Request Completed", "<strong style='color:#0066CC'>GET Request Completed</strong>")
+            line = line.replace("GET Request Completed", "<strong style='color:#0066CC; font-size: 20px;'>GET Request Completed</strong>")
 
         if "Test Execution Environment:" in line:
-            line = line.replace("Test Execution Environment:", "<strong style='color:#0066CC'>Test Execution Environment:</strong>")
+            line = line.replace("Test Execution Environment:", "<strong style='color:#0066CC; font-size: 20px;'>Test Execution Environment:</strong>")
 
         if "Response [200]" in line:
-            line = line.replace("Response [200]", "<strong style='color:green'>Response [200]</strong>")
+            line = line.replace("Response [200]", "<strong style='color:green; font-size: 20px;'>Response [200]</strong>")
 
         if "Response [201]" in line:
-            line = line.replace("Response [201]", "<strong style='color:green'>Response [201]</strong>")
+            line = line.replace("Response [201]", "<strong style='color:green; font-size: 20px;'>Response [201]</strong>")
 
         if "Response [400]" in line:
-            line = line.replace("Response [400]", "<strong style='color:red'>Response [400]</strong>")
+            line = line.replace("Response [400]", "<strong style='color:red; font-size: 20px;'>Response [400]</strong>")
 
         if "Response [401]" in line:
-            line = line.replace("Response [401]", "<strong style='color:red'>Response [401]</strong>")
+            line = line.replace("Response [401]", "<strong style='color:red; font-size: 20px;'>Response [401]</strong>")
 
         if "Response [403]" in line:
-            line = line.replace("Response [403]", "<strong style='color:red'>Response [403]</strong>")
+            line = line.replace("Response [403]", "<strong style='color:red; font-size: 20px;'>Response [403]</strong>")
 
         if "Response [404]" in line:
-            line = line.replace("Response [404]", "<strong style='color:red'>Response [404]</strong>")
+            line = line.replace("Response [404]", "<strong style='color:red; font-size: 20px;'>Response [404]</strong>")
 
         if "Response [500]" in line:
-            line = line.replace("Response [500]", "<strong style='color:red'>Response [500]</strong>")
+            line = line.replace("Response [500]", "<strong style='color:red; font-size: 20px;'>Response [500]</strong>")
 
         if "Response [502]" in line:
-            line = line.replace("Response [502]", "<strong style='color:red'>Response [502]</strong>")
+            line = line.replace("Response [502]", "<strong style='color:red; font-size: 20px;'>Response [502]</strong>")
 
         if "Response [503]" in line:
-            line = line.replace("Response [503]", "<strong style='color:red'>Response [503]</strong>")
+            line = line.replace("Response [503]", "<strong style='color:red; font-size: 20px;'>Response [503]</strong>")
 
         if "Response [504]" in line:
-            line = line.replace("Response [504]", "<strong style='color:red'>Response [504]</strong>")
+            line = line.replace("Response [504]", "<strong style='color:red; font-size: 20px;'>Response [504]</strong>")
 
         if "Assertion Passed:" in line:
-            line = line.replace("Assertion Passed:", "<strong style='color:green'>Assertion Passed:</strong>")
+            line = line.replace("Assertion Passed:", "<strong style='color:green; font-size: 20px;'>Assertion Passed:</strong>")
 
         if "Assertion Failed:" in line:
-            line = line.replace("Assertion Failed:", "<strong style='color:red'>Assertion Failed:</strong>")
+            line = line.replace("Assertion Failed:", "<strong style='color:red; font-size: 20px;'>Assertion Failed:</strong>")
 
         if "logged_requests.py" in line:
             if "URL:" in line and "logged_requests.py" in line.split("URL:")[0]:
-                line = line.replace("URL:", f"<strong style='color:#0066CC'>URL:</strong>")
+                line = line.replace("URL:", f"<strong style='color:#0066CC; font-size: 20px;'>URL:</strong>")
             if "JSON:" in line and "logged_requests.py" in line.split("JSON:")[0]:
-                line = line.replace("JSON:",f"<strong style='color:#0066CC'>JSON:</strong>")
+                line = line.replace("JSON:",f"<strong style='color:#0066CC; font-size: 20px;'>JSON:</strong>")
             if "kwargs:" in line and "logged_requests.py" in line.split("kwargs:")[0]:
-                line = line.replace("kwargs:",f"<strong style='color:#0066CC'>kwargs:</strong>")
+                line = line.replace("kwargs:",f"<strong style='color:#0066CC; font-size: 20px;'>kwargs:</strong>")
             if "params:" in line and "logged_requests.py" in line.split("params:")[0]:
-                line = line.replace("params:", f"<strong style='color:#0066CC'>params:</strong>")
+                line = line.replace("params:", f"<strong style='color:#0066CC; font-size: 20px;'>params:</strong>")
 
         if line == "\n":
             continue
 
         if starts_with_date(line):
             if line.strip().endswith("Traceback (most recent call last):"):
+                line = '<div id="linktest-traceback-section">' + line.strip() + '</div>'
                 traceback_flag = True
 
             if single_line_flag:
                 if lines.startswith("{"):
                     html_content += f'<div class="{class_name}"><pre>{format_json(lines)}</pre></div>'
                 else:
                     if lines.startswith("curl "):
@@ -232,14 +266,20 @@
             lines += line.replace("\n", "<br>")
             single_line_flag = True
             continue
 
     html_content += """
         </div>
     </body>
+        <script>
+            function scrollToTraceback() {
+                var element = document.getElementById("linktest-traceback-section");
+                element.scrollIntoView({behavior: "smooth"});
+            }
+        </script>
     </html>
     """
 
     # 写入HTML文件
     with open(os.path.join(executing_testcase.full_tc_folder,
                            executing_testcase.logfile_full_name.split(os.sep)[-1]).replace("log", "html"), "w") as f:
         f.write(html_content)
```

### Comparing `linktest-2.5.3/linktest/get_adb_devices.py` & `linktest-2.5.4/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.3/linktest/get_ios_devices_list.py` & `linktest-2.5.4/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.3/linktest/get_platform_info.py` & `linktest-2.5.4/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.3/linktest/get_project_info.py` & `linktest-2.5.4/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.3/linktest/html_report.py` & `linktest-2.5.4/linktest/html_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -356,15 +356,15 @@
             if len(failed_cases) > 0:
                 str_failed_testcase_names = ""
 
                 for failed_testcase in failed_cases:
                     str_failed_testcase_names += failed_testcase.__class__.__name__ + " "
 
                 str_failed_testcases = """
-                <button style='background-color: #DC3912; border: none; border-radius: 6px; margin-top: 1px; margin-left: 10%%; width: 125px; height: 38px;' 
+                <button style='background-color: #DC3912; border: none; border-radius: 6px; margin-top: -10px; margin-left: 10%%; width: 125px; height: 39px;' 
                 id="failed_testcase_names" class='failed_testcase_names'
                  data-clipboard-text="%s" onclick="copyFailedTestCase()">
                     <font color='white'>Copy Names of Failed Cases</font>
                 </button>
                 <script>
                     new Clipboard('.failed_testcase_names');
                 </script>
```

### Comparing `linktest-2.5.3/linktest/logged_requests.py` & `linktest-2.5.4/linktest/logged_requests.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.3/linktest/main.py` & `linktest-2.5.4/linktest/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -926,19 +926,19 @@
                     # 执行 setup() 之前 先 log TestEngineCaseInput(如果是 test-engine 发起的)
                     if BaseTestCase.TestEngineCaseInput:
                         executing_testcase.logger.info("- TestEngineCaseInput:")
                         executing_testcase.logger.info(executing_testcase.TestEngineCaseInput)
 
                     # 先执行 setup()， 再执行 run_test()
                     if hasattr(executing_testcase, "setup"):
-                        executing_testcase.logger.info("- execute setup() Start")
+                        executing_testcase.logger.info("- setup() start")
                         executing_testcase.setup()
-                        executing_testcase.logger.info("- execute setup() End")
+                        executing_testcase.logger.info("- setup() end")
 
-                    executing_testcase.logger.info("- run_test() Start")
+                    executing_testcase.logger.info("- run_test() start")
 
                     # For DEBUG_RUN mode,will not set timeout for each testcase
                     executing_testcase.run_test()
 
             except BaseException:
                 executing_testcase.ExecutionStatusSetByFramework = "failed"
                 traceback.print_exc()
@@ -1092,17 +1092,17 @@
                     pass
             finally:
                 # 如果case中 有调用： self.GlobalDataList.append("XXX") 则推荐 settings中设置 ReRun_flag = False
                 executing_testcase.GlobalExecutedCaseList.append(executing_testcase)
 
                 try:
                     if hasattr(executing_testcase, "teardown"):
-                        executing_testcase.logger.info("- execute teardown() Start")
+                        executing_testcase.logger.info("- teardown() start")
                         executing_testcase.teardown()
-                        executing_testcase.logger.info("- execute teardown() End")
+                        executing_testcase.logger.info("- teardown() end")
                 except BaseException as e:
                     executing_testcase.logger.error(e)
 
                 try:
                     if hasattr(executing_testcase, "testcase_id"):
                         testcase.testcase_id = executing_testcase.testcase_id
                     elif hasattr(executing_testcase, "test_case_id"):
```

### Comparing `linktest-2.5.3/linktest/memory_usage.py` & `linktest-2.5.4/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.3/linktest/re_func.py` & `linktest-2.5.4/linktest/re_func.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.3/linktest/run.py` & `linktest-2.5.4/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.3/linktest/run_testcase_thread.py` & `linktest-2.5.4/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.3/linktest/scp_report_to_specified_path.py` & `linktest-2.5.4/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.3/linktest/selenium_helper.py` & `linktest-2.5.4/linktest/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.3/linktest/timeout_thread.py` & `linktest-2.5.4/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.3/linktest/ui_testcase.py` & `linktest-2.5.4/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.3/linktest/update_config.py` & `linktest-2.5.4/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.3/linktest/webdriver_wrapper.py` & `linktest-2.5.4/linktest/webdriver_wrapper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.3/linktest/xml_report.py` & `linktest-2.5.4/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.5.3/linktest.egg-info/SOURCES.txt` & `linktest-2.5.4/linktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

