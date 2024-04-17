# Comparing `tmp/liveramp_automation-1.3.2.tar.gz` & `tmp/liveramp_automation-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveramp_automation-1.3.2.tar", last modified: Wed Apr 17 06:13:26 2024, max compression
+gzip compressed data, was "liveramp_automation-1.3.3.tar", last modified: Wed Apr 17 08:09:29 2024, max compression
```

## Comparing `liveramp_automation-1.3.2.tar` & `liveramp_automation-1.3.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 06:13:26.392931 liveramp_automation-1.3.2/
--rw-r--r--   0 jasqia     (503) staff       (20)    11356 2023-08-02 06:57:58.000000 liveramp_automation-1.3.2/LICENSE
--rw-r--r--   0 jasqia     (503) staff       (20)     2954 2024-04-17 06:13:26.392579 liveramp_automation-1.3.2/PKG-INFO
--rwxrwxrwx   0 jasqia     (503) staff       (20)     1744 2024-03-18 02:41:18.000000 liveramp_automation-1.3.2/README.md
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 06:13:26.377081 liveramp_automation-1.3.2/liveramp_automation/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-09-13 07:36:00.000000 liveramp_automation-1.3.2/liveramp_automation/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)      479 2024-04-17 06:13:24.000000 liveramp_automation-1.3.2/liveramp_automation/__version__.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 06:13:26.380810 liveramp_automation-1.3.2/liveramp_automation/helpers/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.3.2/liveramp_automation/helpers/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4948 2023-09-06 05:34:31.000000 liveramp_automation-1.3.2/liveramp_automation/helpers/bigquery.py
--rw-r--r--   0 jasqia     (503) staff       (20)     8134 2024-04-16 03:01:46.000000 liveramp_automation-1.3.2/liveramp_automation/helpers/bucket.py
--rw-r--r--   0 jasqia     (503) staff       (20)     7898 2024-03-28 09:52:13.000000 liveramp_automation-1.3.2/liveramp_automation/helpers/file.py
--rw-r--r--   0 jasqia     (503) staff       (20)     7284 2024-03-14 07:40:53.000000 liveramp_automation-1.3.2/liveramp_automation/helpers/fixture.py
--rw-r--r--   0 jasqia     (503) staff       (20)     6180 2024-04-16 03:15:54.000000 liveramp_automation-1.3.2/liveramp_automation/helpers/login.py
--rw-r--r--   0 jasqia     (503) staff       (20)    10440 2024-04-16 03:23:44.000000 liveramp_automation-1.3.2/liveramp_automation/helpers/notification.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 06:13:26.385025 liveramp_automation-1.3.2/liveramp_automation/utils/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.3.2/liveramp_automation/utils/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1934 2024-04-01 03:10:38.000000 liveramp_automation-1.3.2/liveramp_automation/utils/allure.py
--rw-r--r--   0 jasqia     (503) staff       (20)     6445 2024-03-01 06:50:54.000000 liveramp_automation-1.3.2/liveramp_automation/utils/log.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4872 2024-04-16 03:16:13.000000 liveramp_automation-1.3.2/liveramp_automation/utils/pagerduty.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1728 2023-08-16 02:33:25.000000 liveramp_automation-1.3.2/liveramp_automation/utils/parsers.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4025 2023-09-13 03:08:07.000000 liveramp_automation-1.3.2/liveramp_automation/utils/playwright.py
--rw-r--r--   0 jasqia     (503) staff       (20)    10164 2023-12-01 07:13:44.000000 liveramp_automation-1.3.2/liveramp_automation/utils/request.py
--rw-r--r--   0 jasqia     (503) staff       (20)    49909 2023-12-11 09:06:44.000000 liveramp_automation-1.3.2/liveramp_automation/utils/selenium.py
--rw-r--r--   0 jasqia     (503) staff       (20)    10500 2024-03-05 09:08:06.000000 liveramp_automation-1.3.2/liveramp_automation/utils/slack.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1660 2023-12-11 09:11:45.000000 liveramp_automation-1.3.2/liveramp_automation/utils/time.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 06:13:26.392065 liveramp_automation-1.3.2/liveramp_automation.egg-info/
--rw-r--r--   0 jasqia     (503) staff       (20)     2954 2024-04-17 06:13:26.000000 liveramp_automation-1.3.2/liveramp_automation.egg-info/PKG-INFO
--rw-r--r--   0 jasqia     (503) staff       (20)     1501 2024-04-17 06:13:26.000000 liveramp_automation-1.3.2/liveramp_automation.egg-info/SOURCES.txt
--rw-r--r--   0 jasqia     (503) staff       (20)        1 2024-04-17 06:13:26.000000 liveramp_automation-1.3.2/liveramp_automation.egg-info/dependency_links.txt
--rw-r--r--   0 jasqia     (503) staff       (20)      443 2024-04-17 06:13:26.000000 liveramp_automation-1.3.2/liveramp_automation.egg-info/requires.txt
--rw-r--r--   0 jasqia     (503) staff       (20)       26 2024-04-17 06:13:26.000000 liveramp_automation-1.3.2/liveramp_automation.egg-info/top_level.txt
--rw-r--r--   0 jasqia     (503) staff       (20)       38 2024-04-17 06:13:26.392991 liveramp_automation-1.3.2/setup.cfg
--rw-r--r--   0 jasqia     (503) staff       (20)     1474 2024-04-17 06:12:35.000000 liveramp_automation-1.3.2/setup.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 06:13:26.385435 liveramp_automation-1.3.2/tests/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.3.2/tests/__init__.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 06:13:26.387848 liveramp_automation-1.3.2/tests/test_helpers/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:03.000000 liveramp_automation-1.3.2/tests/test_helpers/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)     2599 2024-04-01 03:10:38.000000 liveramp_automation-1.3.2/tests/test_helpers/test_bigquery.py
--rw-r--r--   0 jasqia     (503) staff       (20)     2345 2024-04-01 03:35:43.000000 liveramp_automation-1.3.2/tests/test_helpers/test_bucket.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4132 2024-04-01 03:42:11.000000 liveramp_automation-1.3.2/tests/test_helpers/test_file.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1247 2024-03-14 08:05:22.000000 liveramp_automation-1.3.2/tests/test_helpers/test_fixtures.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1676 2024-03-14 09:32:27.000000 liveramp_automation-1.3.2/tests/test_helpers/test_login.py
--rw-r--r--   0 jasqia     (503) staff       (20)     3508 2024-03-05 09:08:06.000000 liveramp_automation-1.3.2/tests/test_helpers/test_notification.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 06:13:26.391500 liveramp_automation-1.3.2/tests/test_utils/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.3.2/tests/test_utils/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1832 2024-03-28 09:52:13.000000 liveramp_automation-1.3.2/tests/test_utils/test_log.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4783 2024-03-28 09:52:13.000000 liveramp_automation-1.3.2/tests/test_utils/test_pagerduty.py
--rw-r--r--   0 jasqia     (503) staff       (20)     3337 2024-04-01 03:10:38.000000 liveramp_automation-1.3.2/tests/test_utils/test_parsers.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1014 2024-03-14 08:40:57.000000 liveramp_automation-1.3.2/tests/test_utils/test_playwright.py
--rw-r--r--   0 jasqia     (503) staff       (20)    13489 2024-04-01 03:10:38.000000 liveramp_automation-1.3.2/tests/test_utils/test_request.py
--rw-r--r--   0 jasqia     (503) staff       (20)    39767 2024-03-28 09:52:13.000000 liveramp_automation-1.3.2/tests/test_utils/test_selenium.py
--rw-r--r--   0 jasqia     (503) staff       (20)     6615 2024-03-28 09:52:13.000000 liveramp_automation-1.3.2/tests/test_utils/test_slack.py
--rw-r--r--   0 jasqia     (503) staff       (20)      742 2024-03-14 08:51:35.000000 liveramp_automation-1.3.2/tests/test_utils/test_version.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 08:09:29.977399 liveramp_automation-1.3.3/
+-rw-r--r--   0 jasqia     (503) staff       (20)    11356 2023-08-02 06:57:58.000000 liveramp_automation-1.3.3/LICENSE
+-rw-r--r--   0 jasqia     (503) staff       (20)     2954 2024-04-17 08:09:29.977066 liveramp_automation-1.3.3/PKG-INFO
+-rwxrwxrwx   0 jasqia     (503) staff       (20)     1744 2024-03-18 02:41:18.000000 liveramp_automation-1.3.3/README.md
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 08:09:29.960279 liveramp_automation-1.3.3/liveramp_automation/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-09-13 07:36:00.000000 liveramp_automation-1.3.3/liveramp_automation/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)      479 2024-04-17 08:09:25.000000 liveramp_automation-1.3.3/liveramp_automation/__version__.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 08:09:29.964316 liveramp_automation-1.3.3/liveramp_automation/helpers/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.3.3/liveramp_automation/helpers/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4948 2023-09-06 05:34:31.000000 liveramp_automation-1.3.3/liveramp_automation/helpers/bigquery.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     8134 2024-04-16 03:01:46.000000 liveramp_automation-1.3.3/liveramp_automation/helpers/bucket.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     7898 2024-03-28 09:52:13.000000 liveramp_automation-1.3.3/liveramp_automation/helpers/file.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     7284 2024-03-14 07:40:53.000000 liveramp_automation-1.3.3/liveramp_automation/helpers/fixture.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     6180 2024-04-16 03:15:54.000000 liveramp_automation-1.3.3/liveramp_automation/helpers/login.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    10686 2024-04-17 08:09:25.000000 liveramp_automation-1.3.3/liveramp_automation/helpers/notification.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 08:09:29.968380 liveramp_automation-1.3.3/liveramp_automation/utils/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.3.3/liveramp_automation/utils/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1934 2024-04-01 03:10:38.000000 liveramp_automation-1.3.3/liveramp_automation/utils/allure.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     6445 2024-03-01 06:50:54.000000 liveramp_automation-1.3.3/liveramp_automation/utils/log.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4941 2024-04-17 08:04:49.000000 liveramp_automation-1.3.3/liveramp_automation/utils/pagerduty.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1728 2023-08-16 02:33:25.000000 liveramp_automation-1.3.3/liveramp_automation/utils/parsers.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4025 2023-09-13 03:08:07.000000 liveramp_automation-1.3.3/liveramp_automation/utils/playwright.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    10164 2023-12-01 07:13:44.000000 liveramp_automation-1.3.3/liveramp_automation/utils/request.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    49909 2023-12-11 09:06:44.000000 liveramp_automation-1.3.3/liveramp_automation/utils/selenium.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    10500 2024-03-05 09:08:06.000000 liveramp_automation-1.3.3/liveramp_automation/utils/slack.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1660 2023-12-11 09:11:45.000000 liveramp_automation-1.3.3/liveramp_automation/utils/time.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 08:09:29.976556 liveramp_automation-1.3.3/liveramp_automation.egg-info/
+-rw-r--r--   0 jasqia     (503) staff       (20)     2954 2024-04-17 08:09:29.000000 liveramp_automation-1.3.3/liveramp_automation.egg-info/PKG-INFO
+-rw-r--r--   0 jasqia     (503) staff       (20)     1501 2024-04-17 08:09:29.000000 liveramp_automation-1.3.3/liveramp_automation.egg-info/SOURCES.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)        1 2024-04-17 08:09:29.000000 liveramp_automation-1.3.3/liveramp_automation.egg-info/dependency_links.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)      443 2024-04-17 08:09:29.000000 liveramp_automation-1.3.3/liveramp_automation.egg-info/requires.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)       26 2024-04-17 08:09:29.000000 liveramp_automation-1.3.3/liveramp_automation.egg-info/top_level.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)       38 2024-04-17 08:09:29.977449 liveramp_automation-1.3.3/setup.cfg
+-rw-r--r--   0 jasqia     (503) staff       (20)     1474 2024-04-17 06:12:35.000000 liveramp_automation-1.3.3/setup.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 08:09:29.968774 liveramp_automation-1.3.3/tests/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.3.3/tests/__init__.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 08:09:29.971190 liveramp_automation-1.3.3/tests/test_helpers/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:03.000000 liveramp_automation-1.3.3/tests/test_helpers/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     2599 2024-04-01 03:10:38.000000 liveramp_automation-1.3.3/tests/test_helpers/test_bigquery.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     2345 2024-04-01 03:35:43.000000 liveramp_automation-1.3.3/tests/test_helpers/test_bucket.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4132 2024-04-01 03:42:11.000000 liveramp_automation-1.3.3/tests/test_helpers/test_file.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1247 2024-03-14 08:05:22.000000 liveramp_automation-1.3.3/tests/test_helpers/test_fixtures.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1676 2024-03-14 09:32:27.000000 liveramp_automation-1.3.3/tests/test_helpers/test_login.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     3508 2024-03-05 09:08:06.000000 liveramp_automation-1.3.3/tests/test_helpers/test_notification.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 08:09:29.975895 liveramp_automation-1.3.3/tests/test_utils/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.3.3/tests/test_utils/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1832 2024-03-28 09:52:13.000000 liveramp_automation-1.3.3/tests/test_utils/test_log.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4783 2024-03-28 09:52:13.000000 liveramp_automation-1.3.3/tests/test_utils/test_pagerduty.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     3337 2024-04-01 03:10:38.000000 liveramp_automation-1.3.3/tests/test_utils/test_parsers.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1014 2024-03-14 08:40:57.000000 liveramp_automation-1.3.3/tests/test_utils/test_playwright.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    13489 2024-04-01 03:10:38.000000 liveramp_automation-1.3.3/tests/test_utils/test_request.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    39767 2024-03-28 09:52:13.000000 liveramp_automation-1.3.3/tests/test_utils/test_selenium.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     6615 2024-03-28 09:52:13.000000 liveramp_automation-1.3.3/tests/test_utils/test_slack.py
+-rw-r--r--   0 jasqia     (503) staff       (20)      742 2024-03-14 08:51:35.000000 liveramp_automation-1.3.3/tests/test_utils/test_version.py
```

### Comparing `liveramp_automation-1.3.2/LICENSE` & `liveramp_automation-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.2/PKG-INFO` & `liveramp_automation-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp_automation
-Version: 1.3.2
+Version: 1.3.3
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/liveramp-automation
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: allure-pytest-bdd
```

### Comparing `liveramp_automation-1.3.2/README.md` & `liveramp_automation-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.2/liveramp_automation/helpers/bigquery.py` & `liveramp_automation-1.3.3/liveramp_automation/helpers/bigquery.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.2/liveramp_automation/helpers/bucket.py` & `liveramp_automation-1.3.3/liveramp_automation/helpers/bucket.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.2/liveramp_automation/helpers/file.py` & `liveramp_automation-1.3.3/liveramp_automation/helpers/file.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.2/liveramp_automation/helpers/fixture.py` & `liveramp_automation-1.3.3/liveramp_automation/helpers/fixture.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.2/liveramp_automation/helpers/login.py` & `liveramp_automation-1.3.3/liveramp_automation/helpers/login.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.2/liveramp_automation/helpers/notification.py` & `liveramp_automation-1.3.3/liveramp_automation/helpers/notification.py`

 * *Files 3% similar despite different names*

```diff
@@ -223,25 +223,29 @@
         return
 
     @staticmethod
     def deal_enqueue(api_key: str,
                      service_id: str,
                      event_action: str,
                      summary: str,
+                     source: str,
+                     dedup_key: str = None,
                      custom_details: dict = None,
-                     dedup_key: str = None):
+                     critical: str = "critical"
+                     ):
         """
         Static method to send PagerDuty a trigger event to report a new problem,
         or update an ongoing problem, depending on the event type.
         https://developer.pagerduty.com/api-reference/368ae3d938c9e-send-an-event-to-pager-duty
         Args:
-            api_key (str): The PagerDuty API key.
-                           The GUID of one of your Events API V2 integrations.
-                           This is the "Integration Key" listed on the Events API V2 integration's detail page.
+            api_key (str): This is the "Integration Key" listed on the Events API V2 integration's detail page.
             service_id (str): The ID of the PagerDuty service to trigger the incident on.
             event_action (str): The type of event. Can be trigger, acknowledge or resolve.
             summary (str): Summary or title of the incident.
+            source (str): The unique location of the affected system, preferably a hostname or FQDN
             custom_details (dict, optional): Additional details about the event and affected system. Defaults to None.
             dedup_key (str, optional): The unique value to differ events.
+            critical (str, optional): Allowed values: critical,warning,error,info. Defaults to "critical".
         """
         pagerduty_client = PagerDutyClient(api_key)
-        return pagerduty_client.deal_enqueue(service_id, event_action, summary, custom_details, dedup_key)
+        return pagerduty_client.deal_enqueue(service_id, event_action, dedup_key, summary,
+                                             source, custom_details, critical)
```

### Comparing `liveramp_automation-1.3.2/liveramp_automation/utils/allure.py` & `liveramp_automation-1.3.3/liveramp_automation/utils/allure.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.2/liveramp_automation/utils/log.py` & `liveramp_automation-1.3.3/liveramp_automation/utils/log.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.2/liveramp_automation/utils/pagerduty.py` & `liveramp_automation-1.3.3/liveramp_automation/utils/pagerduty.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,27 +91,29 @@
         response = requests.get(endpoint, params=payload, headers=self.headers)
         response.raise_for_status()
         Logger.debug(f"Received the response: {response.json()}")
         incidents = response.json().get('incidents', [])
         incident_list = [{'id': incident['id'], 'url': incident['html_url']} for incident in incidents]
         return incident_list
 
-    def deal_enqueue(self, service_id: str, event_action: str, dedup_key: str, summary: str,
-                     custom_details: Optional[Dict[str, Any]] = None):
+    def deal_enqueue(self, service_id: str, event_action: str, dedup_key: str,
+                     summary: str, source: str,
+                     custom_details: Optional[Dict[str, Any]] = None,
+                     severity="critical"):
         endpoint = f'{self.event_url}/v2/enqueue'
         json_data = {
             "dedup_key": dedup_key,
             "event_action": event_action,
             "payload": {
-                "severity": "critical",
+                "severity": severity,
+                "summary": summary,
+                "source": source
             },
             "routing_key": service_id
         }
-        if summary:
-            json_data["payload"]['summary'] = summary
 
         if custom_details:
             json_data["payload"]['custom_details'] = custom_details
 
         Logger.debug(f"Sending a request - url: {endpoint}, payload: {json_data}, headers: {self.headers}")
         response = requests.post(endpoint, json=json_data, headers=self.headers)
         return response
```

### Comparing `liveramp_automation-1.3.2/liveramp_automation/utils/parsers.py` & `liveramp_automation-1.3.3/liveramp_automation/utils/parsers.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.2/liveramp_automation/utils/playwright.py` & `liveramp_automation-1.3.3/liveramp_automation/utils/playwright.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.2/liveramp_automation/utils/request.py` & `liveramp_automation-1.3.3/liveramp_automation/utils/request.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.2/liveramp_automation/utils/selenium.py` & `liveramp_automation-1.3.3/liveramp_automation/utils/selenium.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.2/liveramp_automation/utils/slack.py` & `liveramp_automation-1.3.3/liveramp_automation/utils/slack.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.2/liveramp_automation/utils/time.py` & `liveramp_automation-1.3.3/liveramp_automation/utils/time.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.2/liveramp_automation.egg-info/PKG-INFO` & `liveramp_automation-1.3.3/liveramp_automation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp-automation
-Version: 1.3.2
+Version: 1.3.3
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/liveramp-automation
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: allure-pytest-bdd
```

### Comparing `liveramp_automation-1.3.2/liveramp_automation.egg-info/SOURCES.txt` & `liveramp_automation-1.3.3/liveramp_automation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.2/setup.py` & `liveramp_automation-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.2/tests/test_helpers/test_bigquery.py` & `liveramp_automation-1.3.3/tests/test_helpers/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.2/tests/test_helpers/test_bucket.py` & `liveramp_automation-1.3.3/tests/test_helpers/test_bucket.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.2/tests/test_helpers/test_file.py` & `liveramp_automation-1.3.3/tests/test_helpers/test_file.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.2/tests/test_helpers/test_fixtures.py` & `liveramp_automation-1.3.3/tests/test_helpers/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.2/tests/test_helpers/test_login.py` & `liveramp_automation-1.3.3/tests/test_helpers/test_login.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.2/tests/test_helpers/test_notification.py` & `liveramp_automation-1.3.3/tests/test_helpers/test_notification.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.2/tests/test_utils/test_log.py` & `liveramp_automation-1.3.3/tests/test_utils/test_log.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.2/tests/test_utils/test_pagerduty.py` & `liveramp_automation-1.3.3/tests/test_utils/test_pagerduty.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.2/tests/test_utils/test_parsers.py` & `liveramp_automation-1.3.3/tests/test_utils/test_parsers.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.2/tests/test_utils/test_playwright.py` & `liveramp_automation-1.3.3/tests/test_utils/test_playwright.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.2/tests/test_utils/test_request.py` & `liveramp_automation-1.3.3/tests/test_utils/test_request.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.2/tests/test_utils/test_selenium.py` & `liveramp_automation-1.3.3/tests/test_utils/test_selenium.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.2/tests/test_utils/test_slack.py` & `liveramp_automation-1.3.3/tests/test_utils/test_slack.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.2/tests/test_utils/test_version.py` & `liveramp_automation-1.3.3/tests/test_utils/test_version.py`

 * *Files identical despite different names*

