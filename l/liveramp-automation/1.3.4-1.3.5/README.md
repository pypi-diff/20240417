# Comparing `tmp/liveramp_automation-1.3.4.tar.gz` & `tmp/liveramp_automation-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveramp_automation-1.3.4.tar", last modified: Wed Apr 17 08:14:07 2024, max compression
+gzip compressed data, was "liveramp_automation-1.3.5.tar", last modified: Wed Apr 17 08:17:05 2024, max compression
```

## Comparing `liveramp_automation-1.3.4.tar` & `liveramp_automation-1.3.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 08:14:07.591312 liveramp_automation-1.3.4/
--rw-r--r--   0 jasqia     (503) staff       (20)    11356 2023-08-02 06:57:58.000000 liveramp_automation-1.3.4/LICENSE
--rw-r--r--   0 jasqia     (503) staff       (20)     2976 2024-04-17 08:14:07.590990 liveramp_automation-1.3.4/PKG-INFO
--rwxrwxrwx   0 jasqia     (503) staff       (20)     1744 2024-03-18 02:41:18.000000 liveramp_automation-1.3.4/README.md
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 08:14:07.574777 liveramp_automation-1.3.4/liveramp_automation/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-09-13 07:36:00.000000 liveramp_automation-1.3.4/liveramp_automation/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)      479 2024-04-17 08:14:06.000000 liveramp_automation-1.3.4/liveramp_automation/__version__.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 08:14:07.578850 liveramp_automation-1.3.4/liveramp_automation/helpers/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.3.4/liveramp_automation/helpers/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4948 2023-09-06 05:34:31.000000 liveramp_automation-1.3.4/liveramp_automation/helpers/bigquery.py
--rw-r--r--   0 jasqia     (503) staff       (20)     8134 2024-04-16 03:01:46.000000 liveramp_automation-1.3.4/liveramp_automation/helpers/bucket.py
--rw-r--r--   0 jasqia     (503) staff       (20)     7898 2024-03-28 09:52:13.000000 liveramp_automation-1.3.4/liveramp_automation/helpers/file.py
--rw-r--r--   0 jasqia     (503) staff       (20)     7284 2024-03-14 07:40:53.000000 liveramp_automation-1.3.4/liveramp_automation/helpers/fixture.py
--rw-r--r--   0 jasqia     (503) staff       (20)     6180 2024-04-16 03:15:54.000000 liveramp_automation-1.3.4/liveramp_automation/helpers/login.py
--rw-r--r--   0 jasqia     (503) staff       (20)    10686 2024-04-17 08:09:25.000000 liveramp_automation-1.3.4/liveramp_automation/helpers/notification.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 08:14:07.583201 liveramp_automation-1.3.4/liveramp_automation/utils/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.3.4/liveramp_automation/utils/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1934 2024-04-01 03:10:38.000000 liveramp_automation-1.3.4/liveramp_automation/utils/allure.py
--rw-r--r--   0 jasqia     (503) staff       (20)     6445 2024-03-01 06:50:54.000000 liveramp_automation-1.3.4/liveramp_automation/utils/log.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4941 2024-04-17 08:04:49.000000 liveramp_automation-1.3.4/liveramp_automation/utils/pagerduty.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1728 2023-08-16 02:33:25.000000 liveramp_automation-1.3.4/liveramp_automation/utils/parsers.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4025 2023-09-13 03:08:07.000000 liveramp_automation-1.3.4/liveramp_automation/utils/playwright.py
--rw-r--r--   0 jasqia     (503) staff       (20)    10164 2023-12-01 07:13:44.000000 liveramp_automation-1.3.4/liveramp_automation/utils/request.py
--rw-r--r--   0 jasqia     (503) staff       (20)    49909 2023-12-11 09:06:44.000000 liveramp_automation-1.3.4/liveramp_automation/utils/selenium.py
--rw-r--r--   0 jasqia     (503) staff       (20)    10500 2024-03-05 09:08:06.000000 liveramp_automation-1.3.4/liveramp_automation/utils/slack.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1660 2023-12-11 09:11:45.000000 liveramp_automation-1.3.4/liveramp_automation/utils/time.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 08:14:07.590448 liveramp_automation-1.3.4/liveramp_automation.egg-info/
--rw-r--r--   0 jasqia     (503) staff       (20)     2976 2024-04-17 08:14:07.000000 liveramp_automation-1.3.4/liveramp_automation.egg-info/PKG-INFO
--rw-r--r--   0 jasqia     (503) staff       (20)     1501 2024-04-17 08:14:07.000000 liveramp_automation-1.3.4/liveramp_automation.egg-info/SOURCES.txt
--rw-r--r--   0 jasqia     (503) staff       (20)        1 2024-04-17 08:14:07.000000 liveramp_automation-1.3.4/liveramp_automation.egg-info/dependency_links.txt
--rw-r--r--   0 jasqia     (503) staff       (20)      450 2024-04-17 08:14:07.000000 liveramp_automation-1.3.4/liveramp_automation.egg-info/requires.txt
--rw-r--r--   0 jasqia     (503) staff       (20)       26 2024-04-17 08:14:07.000000 liveramp_automation-1.3.4/liveramp_automation.egg-info/top_level.txt
--rw-r--r--   0 jasqia     (503) staff       (20)       38 2024-04-17 08:14:07.591382 liveramp_automation-1.3.4/setup.cfg
--rw-r--r--   0 jasqia     (503) staff       (20)     1492 2024-04-17 08:10:51.000000 liveramp_automation-1.3.4/setup.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 08:14:07.583545 liveramp_automation-1.3.4/tests/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.3.4/tests/__init__.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 08:14:07.586052 liveramp_automation-1.3.4/tests/test_helpers/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:03.000000 liveramp_automation-1.3.4/tests/test_helpers/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)     2599 2024-04-01 03:10:38.000000 liveramp_automation-1.3.4/tests/test_helpers/test_bigquery.py
--rw-r--r--   0 jasqia     (503) staff       (20)     2345 2024-04-01 03:35:43.000000 liveramp_automation-1.3.4/tests/test_helpers/test_bucket.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4132 2024-04-01 03:42:11.000000 liveramp_automation-1.3.4/tests/test_helpers/test_file.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1247 2024-03-14 08:05:22.000000 liveramp_automation-1.3.4/tests/test_helpers/test_fixtures.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1676 2024-03-14 09:32:27.000000 liveramp_automation-1.3.4/tests/test_helpers/test_login.py
--rw-r--r--   0 jasqia     (503) staff       (20)     3508 2024-03-05 09:08:06.000000 liveramp_automation-1.3.4/tests/test_helpers/test_notification.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 08:14:07.589835 liveramp_automation-1.3.4/tests/test_utils/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.3.4/tests/test_utils/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1832 2024-03-28 09:52:13.000000 liveramp_automation-1.3.4/tests/test_utils/test_log.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4783 2024-03-28 09:52:13.000000 liveramp_automation-1.3.4/tests/test_utils/test_pagerduty.py
--rw-r--r--   0 jasqia     (503) staff       (20)     3337 2024-04-01 03:10:38.000000 liveramp_automation-1.3.4/tests/test_utils/test_parsers.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1014 2024-03-14 08:40:57.000000 liveramp_automation-1.3.4/tests/test_utils/test_playwright.py
--rw-r--r--   0 jasqia     (503) staff       (20)    13489 2024-04-01 03:10:38.000000 liveramp_automation-1.3.4/tests/test_utils/test_request.py
--rw-r--r--   0 jasqia     (503) staff       (20)    39767 2024-03-28 09:52:13.000000 liveramp_automation-1.3.4/tests/test_utils/test_selenium.py
--rw-r--r--   0 jasqia     (503) staff       (20)     6615 2024-03-28 09:52:13.000000 liveramp_automation-1.3.4/tests/test_utils/test_slack.py
--rw-r--r--   0 jasqia     (503) staff       (20)      742 2024-03-14 08:51:35.000000 liveramp_automation-1.3.4/tests/test_utils/test_version.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 08:17:05.464918 liveramp_automation-1.3.5/
+-rw-r--r--   0 jasqia     (503) staff       (20)    11356 2023-08-02 06:57:58.000000 liveramp_automation-1.3.5/LICENSE
+-rw-r--r--   0 jasqia     (503) staff       (20)     2983 2024-04-17 08:17:05.464497 liveramp_automation-1.3.5/PKG-INFO
+-rwxrwxrwx   0 jasqia     (503) staff       (20)     1744 2024-03-18 02:41:18.000000 liveramp_automation-1.3.5/README.md
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 08:17:05.444604 liveramp_automation-1.3.5/liveramp_automation/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-09-13 07:36:00.000000 liveramp_automation-1.3.5/liveramp_automation/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)      479 2024-04-17 08:16:51.000000 liveramp_automation-1.3.5/liveramp_automation/__version__.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 08:17:05.450136 liveramp_automation-1.3.5/liveramp_automation/helpers/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.3.5/liveramp_automation/helpers/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4948 2023-09-06 05:34:31.000000 liveramp_automation-1.3.5/liveramp_automation/helpers/bigquery.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     8134 2024-04-16 03:01:46.000000 liveramp_automation-1.3.5/liveramp_automation/helpers/bucket.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     7898 2024-03-28 09:52:13.000000 liveramp_automation-1.3.5/liveramp_automation/helpers/file.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     7284 2024-03-14 07:40:53.000000 liveramp_automation-1.3.5/liveramp_automation/helpers/fixture.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     6180 2024-04-16 03:15:54.000000 liveramp_automation-1.3.5/liveramp_automation/helpers/login.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    10686 2024-04-17 08:09:25.000000 liveramp_automation-1.3.5/liveramp_automation/helpers/notification.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 08:17:05.456013 liveramp_automation-1.3.5/liveramp_automation/utils/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.3.5/liveramp_automation/utils/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1934 2024-04-01 03:10:38.000000 liveramp_automation-1.3.5/liveramp_automation/utils/allure.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     6445 2024-03-01 06:50:54.000000 liveramp_automation-1.3.5/liveramp_automation/utils/log.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4941 2024-04-17 08:04:49.000000 liveramp_automation-1.3.5/liveramp_automation/utils/pagerduty.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1728 2023-08-16 02:33:25.000000 liveramp_automation-1.3.5/liveramp_automation/utils/parsers.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4025 2023-09-13 03:08:07.000000 liveramp_automation-1.3.5/liveramp_automation/utils/playwright.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    10164 2023-12-01 07:13:44.000000 liveramp_automation-1.3.5/liveramp_automation/utils/request.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    49909 2023-12-11 09:06:44.000000 liveramp_automation-1.3.5/liveramp_automation/utils/selenium.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    10500 2024-03-05 09:08:06.000000 liveramp_automation-1.3.5/liveramp_automation/utils/slack.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1660 2023-12-11 09:11:45.000000 liveramp_automation-1.3.5/liveramp_automation/utils/time.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 08:17:05.463882 liveramp_automation-1.3.5/liveramp_automation.egg-info/
+-rw-r--r--   0 jasqia     (503) staff       (20)     2983 2024-04-17 08:17:05.000000 liveramp_automation-1.3.5/liveramp_automation.egg-info/PKG-INFO
+-rw-r--r--   0 jasqia     (503) staff       (20)     1501 2024-04-17 08:17:05.000000 liveramp_automation-1.3.5/liveramp_automation.egg-info/SOURCES.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)        1 2024-04-17 08:17:05.000000 liveramp_automation-1.3.5/liveramp_automation.egg-info/dependency_links.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)      457 2024-04-17 08:17:05.000000 liveramp_automation-1.3.5/liveramp_automation.egg-info/requires.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)       26 2024-04-17 08:17:05.000000 liveramp_automation-1.3.5/liveramp_automation.egg-info/top_level.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)       38 2024-04-17 08:17:05.464989 liveramp_automation-1.3.5/setup.cfg
+-rw-r--r--   0 jasqia     (503) staff       (20)     1499 2024-04-17 08:16:46.000000 liveramp_automation-1.3.5/setup.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 08:17:05.456449 liveramp_automation-1.3.5/tests/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.3.5/tests/__init__.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 08:17:05.459161 liveramp_automation-1.3.5/tests/test_helpers/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:03.000000 liveramp_automation-1.3.5/tests/test_helpers/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     2599 2024-04-01 03:10:38.000000 liveramp_automation-1.3.5/tests/test_helpers/test_bigquery.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     2345 2024-04-01 03:35:43.000000 liveramp_automation-1.3.5/tests/test_helpers/test_bucket.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4132 2024-04-01 03:42:11.000000 liveramp_automation-1.3.5/tests/test_helpers/test_file.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1247 2024-03-14 08:05:22.000000 liveramp_automation-1.3.5/tests/test_helpers/test_fixtures.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1676 2024-03-14 09:32:27.000000 liveramp_automation-1.3.5/tests/test_helpers/test_login.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     3508 2024-03-05 09:08:06.000000 liveramp_automation-1.3.5/tests/test_helpers/test_notification.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 08:17:05.463158 liveramp_automation-1.3.5/tests/test_utils/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.3.5/tests/test_utils/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1832 2024-03-28 09:52:13.000000 liveramp_automation-1.3.5/tests/test_utils/test_log.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4783 2024-03-28 09:52:13.000000 liveramp_automation-1.3.5/tests/test_utils/test_pagerduty.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     3337 2024-04-01 03:10:38.000000 liveramp_automation-1.3.5/tests/test_utils/test_parsers.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1014 2024-03-14 08:40:57.000000 liveramp_automation-1.3.5/tests/test_utils/test_playwright.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    13489 2024-04-01 03:10:38.000000 liveramp_automation-1.3.5/tests/test_utils/test_request.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    39767 2024-03-28 09:52:13.000000 liveramp_automation-1.3.5/tests/test_utils/test_selenium.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     6615 2024-03-28 09:52:13.000000 liveramp_automation-1.3.5/tests/test_utils/test_slack.py
+-rw-r--r--   0 jasqia     (503) staff       (20)      742 2024-03-14 08:51:35.000000 liveramp_automation-1.3.5/tests/test_utils/test_version.py
```

### Comparing `liveramp_automation-1.3.4/LICENSE` & `liveramp_automation-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.4/PKG-INFO` & `liveramp_automation-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: liveramp_automation
-Version: 1.3.4
+Version: 1.3.5
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/liveramp-automation
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: allure-pytest-bdd
 Requires-Dist: allure-python-commons
 Requires-Dist: boto3
 Requires-Dist: certifi
 Requires-Dist: datadog
 Requires-Dist: db-dtypes
 Requires-Dist: dnspython
-Requires-Dist: dotenv
 Requires-Dist: google
 Requires-Dist: google-api-core
 Requires-Dist: google-auth
 Requires-Dist: google-cloud-bigquery
 Requires-Dist: google-cloud-core
 Requires-Dist: google-cloud-storage
 Requires-Dist: google-crc32c
@@ -30,14 +29,15 @@
 Requires-Dist: pysftp
 Requires-Dist: pytest==7.4.4
 Requires-Dist: pytest-bdd==7.0.1
 Requires-Dist: pytest-json
 Requires-Dist: pytest-json-report
 Requires-Dist: pytest-playwright==0.4.3
 Requires-Dist: pytest-xdist==3.5.0
+Requires-Dist: python-dotenv
 Requires-Dist: PyYAML
 Requires-Dist: requests
 Requires-Dist: retrying
 Requires-Dist: snowflake
 Requires-Dist: selenium==4.16.0
 
 # liveramp-automation
```

### Comparing `liveramp_automation-1.3.4/README.md` & `liveramp_automation-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.4/liveramp_automation/helpers/bigquery.py` & `liveramp_automation-1.3.5/liveramp_automation/helpers/bigquery.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.4/liveramp_automation/helpers/bucket.py` & `liveramp_automation-1.3.5/liveramp_automation/helpers/bucket.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.4/liveramp_automation/helpers/file.py` & `liveramp_automation-1.3.5/liveramp_automation/helpers/file.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.4/liveramp_automation/helpers/fixture.py` & `liveramp_automation-1.3.5/liveramp_automation/helpers/fixture.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.4/liveramp_automation/helpers/login.py` & `liveramp_automation-1.3.5/liveramp_automation/helpers/login.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.4/liveramp_automation/helpers/notification.py` & `liveramp_automation-1.3.5/liveramp_automation/helpers/notification.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.4/liveramp_automation/utils/allure.py` & `liveramp_automation-1.3.5/liveramp_automation/utils/allure.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.4/liveramp_automation/utils/log.py` & `liveramp_automation-1.3.5/liveramp_automation/utils/log.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.4/liveramp_automation/utils/pagerduty.py` & `liveramp_automation-1.3.5/liveramp_automation/utils/pagerduty.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.4/liveramp_automation/utils/parsers.py` & `liveramp_automation-1.3.5/liveramp_automation/utils/parsers.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.4/liveramp_automation/utils/playwright.py` & `liveramp_automation-1.3.5/liveramp_automation/utils/playwright.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.4/liveramp_automation/utils/request.py` & `liveramp_automation-1.3.5/liveramp_automation/utils/request.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.4/liveramp_automation/utils/selenium.py` & `liveramp_automation-1.3.5/liveramp_automation/utils/selenium.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.4/liveramp_automation/utils/slack.py` & `liveramp_automation-1.3.5/liveramp_automation/utils/slack.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.4/liveramp_automation/utils/time.py` & `liveramp_automation-1.3.5/liveramp_automation/utils/time.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.4/liveramp_automation.egg-info/PKG-INFO` & `liveramp_automation-1.3.5/liveramp_automation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: liveramp-automation
-Version: 1.3.4
+Version: 1.3.5
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/liveramp-automation
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: allure-pytest-bdd
 Requires-Dist: allure-python-commons
 Requires-Dist: boto3
 Requires-Dist: certifi
 Requires-Dist: datadog
 Requires-Dist: db-dtypes
 Requires-Dist: dnspython
-Requires-Dist: dotenv
 Requires-Dist: google
 Requires-Dist: google-api-core
 Requires-Dist: google-auth
 Requires-Dist: google-cloud-bigquery
 Requires-Dist: google-cloud-core
 Requires-Dist: google-cloud-storage
 Requires-Dist: google-crc32c
@@ -30,14 +29,15 @@
 Requires-Dist: pysftp
 Requires-Dist: pytest==7.4.4
 Requires-Dist: pytest-bdd==7.0.1
 Requires-Dist: pytest-json
 Requires-Dist: pytest-json-report
 Requires-Dist: pytest-playwright==0.4.3
 Requires-Dist: pytest-xdist==3.5.0
+Requires-Dist: python-dotenv
 Requires-Dist: PyYAML
 Requires-Dist: requests
 Requires-Dist: retrying
 Requires-Dist: snowflake
 Requires-Dist: selenium==4.16.0
 
 # liveramp-automation
```

### Comparing `liveramp_automation-1.3.4/liveramp_automation.egg-info/SOURCES.txt` & `liveramp_automation-1.3.5/liveramp_automation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.4/setup.py` & `liveramp_automation-1.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
         'allure-pytest-bdd',
         'allure-python-commons',
         'boto3',
         'certifi',
         'datadog',
         'db-dtypes',
         'dnspython',
-        'dotenv',
         'google',
         'google-api-core',
         'google-auth',
         'google-cloud-bigquery',
         'google-cloud-core',
         'google-cloud-storage',
         'google-crc32c',
@@ -44,14 +43,15 @@
         'pysftp',
         'pytest==7.4.4',
         'pytest-bdd==7.0.1',
         'pytest-json',
         'pytest-json-report',
         'pytest-playwright==0.4.3',
         'pytest-xdist==3.5.0',
+        'python-dotenv',
         'PyYAML',
         'requests',
         'retrying',
         'snowflake',
         'selenium==4.16.0',
     ],
 )
```

### Comparing `liveramp_automation-1.3.4/tests/test_helpers/test_bigquery.py` & `liveramp_automation-1.3.5/tests/test_helpers/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.4/tests/test_helpers/test_bucket.py` & `liveramp_automation-1.3.5/tests/test_helpers/test_bucket.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.4/tests/test_helpers/test_file.py` & `liveramp_automation-1.3.5/tests/test_helpers/test_file.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.4/tests/test_helpers/test_fixtures.py` & `liveramp_automation-1.3.5/tests/test_helpers/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.4/tests/test_helpers/test_login.py` & `liveramp_automation-1.3.5/tests/test_helpers/test_login.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.4/tests/test_helpers/test_notification.py` & `liveramp_automation-1.3.5/tests/test_helpers/test_notification.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.4/tests/test_utils/test_log.py` & `liveramp_automation-1.3.5/tests/test_utils/test_log.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.4/tests/test_utils/test_pagerduty.py` & `liveramp_automation-1.3.5/tests/test_utils/test_pagerduty.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.4/tests/test_utils/test_parsers.py` & `liveramp_automation-1.3.5/tests/test_utils/test_parsers.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.4/tests/test_utils/test_playwright.py` & `liveramp_automation-1.3.5/tests/test_utils/test_playwright.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.4/tests/test_utils/test_request.py` & `liveramp_automation-1.3.5/tests/test_utils/test_request.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.4/tests/test_utils/test_selenium.py` & `liveramp_automation-1.3.5/tests/test_utils/test_selenium.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.4/tests/test_utils/test_slack.py` & `liveramp_automation-1.3.5/tests/test_utils/test_slack.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.4/tests/test_utils/test_version.py` & `liveramp_automation-1.3.5/tests/test_utils/test_version.py`

 * *Files identical despite different names*

