# Comparing `tmp/liveramp_automation-1.3.1.tar.gz` & `tmp/liveramp_automation-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveramp_automation-1.3.1.tar", last modified: Fri Apr 12 01:22:43 2024, max compression
+gzip compressed data, was "liveramp_automation-1.3.2.tar", last modified: Wed Apr 17 06:13:26 2024, max compression
```

## Comparing `liveramp_automation-1.3.1.tar` & `liveramp_automation-1.3.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-12 01:22:43.086596 liveramp_automation-1.3.1/
--rw-r--r--   0 jasqia     (503) staff       (20)    11356 2023-08-02 06:57:58.000000 liveramp_automation-1.3.1/LICENSE
--rw-r--r--   0 jasqia     (503) staff       (20)     2906 2024-04-12 01:22:43.086268 liveramp_automation-1.3.1/PKG-INFO
--rwxrwxrwx   0 jasqia     (503) staff       (20)     1744 2024-03-18 02:41:18.000000 liveramp_automation-1.3.1/README.md
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-12 01:22:43.068800 liveramp_automation-1.3.1/liveramp_automation/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-09-13 07:36:00.000000 liveramp_automation-1.3.1/liveramp_automation/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)      479 2024-04-12 01:22:24.000000 liveramp_automation-1.3.1/liveramp_automation/__version__.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-12 01:22:43.072868 liveramp_automation-1.3.1/liveramp_automation/helpers/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.3.1/liveramp_automation/helpers/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4948 2023-09-06 05:34:31.000000 liveramp_automation-1.3.1/liveramp_automation/helpers/bigquery.py
--rw-r--r--   0 jasqia     (503) staff       (20)     8133 2024-02-28 01:54:10.000000 liveramp_automation-1.3.1/liveramp_automation/helpers/bucket.py
--rw-r--r--   0 jasqia     (503) staff       (20)     7898 2024-03-28 09:52:13.000000 liveramp_automation-1.3.1/liveramp_automation/helpers/file.py
--rw-r--r--   0 jasqia     (503) staff       (20)     7284 2024-03-14 07:40:53.000000 liveramp_automation-1.3.1/liveramp_automation/helpers/fixture.py
--rw-r--r--   0 jasqia     (503) staff       (20)     6180 2024-04-03 03:14:23.000000 liveramp_automation-1.3.1/liveramp_automation/helpers/login.py
--rw-r--r--   0 jasqia     (503) staff       (20)     9622 2024-03-20 08:56:22.000000 liveramp_automation-1.3.1/liveramp_automation/helpers/notification.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-12 01:22:43.077639 liveramp_automation-1.3.1/liveramp_automation/utils/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.3.1/liveramp_automation/utils/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1934 2024-04-01 03:10:38.000000 liveramp_automation-1.3.1/liveramp_automation/utils/allure.py
--rw-r--r--   0 jasqia     (503) staff       (20)     6445 2024-03-01 06:50:54.000000 liveramp_automation-1.3.1/liveramp_automation/utils/log.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4960 2024-03-28 09:52:13.000000 liveramp_automation-1.3.1/liveramp_automation/utils/pagerduty.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1728 2023-08-16 02:33:25.000000 liveramp_automation-1.3.1/liveramp_automation/utils/parsers.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4025 2023-09-13 03:08:07.000000 liveramp_automation-1.3.1/liveramp_automation/utils/playwright.py
--rw-r--r--   0 jasqia     (503) staff       (20)    10164 2023-12-01 07:13:44.000000 liveramp_automation-1.3.1/liveramp_automation/utils/request.py
--rw-r--r--   0 jasqia     (503) staff       (20)    49909 2023-12-11 09:06:44.000000 liveramp_automation-1.3.1/liveramp_automation/utils/selenium.py
--rw-r--r--   0 jasqia     (503) staff       (20)    10500 2024-03-05 09:08:06.000000 liveramp_automation-1.3.1/liveramp_automation/utils/slack.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1660 2023-12-11 09:11:45.000000 liveramp_automation-1.3.1/liveramp_automation/utils/time.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-12 01:22:43.085735 liveramp_automation-1.3.1/liveramp_automation.egg-info/
--rw-r--r--   0 jasqia     (503) staff       (20)     2906 2024-04-12 01:22:43.000000 liveramp_automation-1.3.1/liveramp_automation.egg-info/PKG-INFO
--rw-r--r--   0 jasqia     (503) staff       (20)     1501 2024-04-12 01:22:43.000000 liveramp_automation-1.3.1/liveramp_automation.egg-info/SOURCES.txt
--rw-r--r--   0 jasqia     (503) staff       (20)        1 2024-04-12 01:22:43.000000 liveramp_automation-1.3.1/liveramp_automation.egg-info/dependency_links.txt
--rw-r--r--   0 jasqia     (503) staff       (20)      425 2024-04-12 01:22:43.000000 liveramp_automation-1.3.1/liveramp_automation.egg-info/requires.txt
--rw-r--r--   0 jasqia     (503) staff       (20)       26 2024-04-12 01:22:43.000000 liveramp_automation-1.3.1/liveramp_automation.egg-info/top_level.txt
--rw-r--r--   0 jasqia     (503) staff       (20)       38 2024-04-12 01:22:43.086662 liveramp_automation-1.3.1/setup.cfg
--rw-r--r--   0 jasqia     (503) staff       (20)     1434 2024-04-12 01:22:13.000000 liveramp_automation-1.3.1/setup.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-12 01:22:43.078025 liveramp_automation-1.3.1/tests/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.3.1/tests/__init__.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-12 01:22:43.080515 liveramp_automation-1.3.1/tests/test_helpers/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:03.000000 liveramp_automation-1.3.1/tests/test_helpers/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)     2599 2024-04-01 03:10:38.000000 liveramp_automation-1.3.1/tests/test_helpers/test_bigquery.py
--rw-r--r--   0 jasqia     (503) staff       (20)     2345 2024-04-01 03:35:43.000000 liveramp_automation-1.3.1/tests/test_helpers/test_bucket.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4132 2024-04-01 03:42:11.000000 liveramp_automation-1.3.1/tests/test_helpers/test_file.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1247 2024-03-14 08:05:22.000000 liveramp_automation-1.3.1/tests/test_helpers/test_fixtures.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1676 2024-03-14 09:32:27.000000 liveramp_automation-1.3.1/tests/test_helpers/test_login.py
--rw-r--r--   0 jasqia     (503) staff       (20)     3508 2024-03-05 09:08:06.000000 liveramp_automation-1.3.1/tests/test_helpers/test_notification.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-12 01:22:43.085087 liveramp_automation-1.3.1/tests/test_utils/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.3.1/tests/test_utils/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1832 2024-03-28 09:52:13.000000 liveramp_automation-1.3.1/tests/test_utils/test_log.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4783 2024-03-28 09:52:13.000000 liveramp_automation-1.3.1/tests/test_utils/test_pagerduty.py
--rw-r--r--   0 jasqia     (503) staff       (20)     3337 2024-04-01 03:10:38.000000 liveramp_automation-1.3.1/tests/test_utils/test_parsers.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1014 2024-03-14 08:40:57.000000 liveramp_automation-1.3.1/tests/test_utils/test_playwright.py
--rw-r--r--   0 jasqia     (503) staff       (20)    13489 2024-04-01 03:10:38.000000 liveramp_automation-1.3.1/tests/test_utils/test_request.py
--rw-r--r--   0 jasqia     (503) staff       (20)    39767 2024-03-28 09:52:13.000000 liveramp_automation-1.3.1/tests/test_utils/test_selenium.py
--rw-r--r--   0 jasqia     (503) staff       (20)     6615 2024-03-28 09:52:13.000000 liveramp_automation-1.3.1/tests/test_utils/test_slack.py
--rw-r--r--   0 jasqia     (503) staff       (20)      742 2024-03-14 08:51:35.000000 liveramp_automation-1.3.1/tests/test_utils/test_version.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 06:13:26.392931 liveramp_automation-1.3.2/
+-rw-r--r--   0 jasqia     (503) staff       (20)    11356 2023-08-02 06:57:58.000000 liveramp_automation-1.3.2/LICENSE
+-rw-r--r--   0 jasqia     (503) staff       (20)     2954 2024-04-17 06:13:26.392579 liveramp_automation-1.3.2/PKG-INFO
+-rwxrwxrwx   0 jasqia     (503) staff       (20)     1744 2024-03-18 02:41:18.000000 liveramp_automation-1.3.2/README.md
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 06:13:26.377081 liveramp_automation-1.3.2/liveramp_automation/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-09-13 07:36:00.000000 liveramp_automation-1.3.2/liveramp_automation/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)      479 2024-04-17 06:13:24.000000 liveramp_automation-1.3.2/liveramp_automation/__version__.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 06:13:26.380810 liveramp_automation-1.3.2/liveramp_automation/helpers/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.3.2/liveramp_automation/helpers/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4948 2023-09-06 05:34:31.000000 liveramp_automation-1.3.2/liveramp_automation/helpers/bigquery.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     8134 2024-04-16 03:01:46.000000 liveramp_automation-1.3.2/liveramp_automation/helpers/bucket.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     7898 2024-03-28 09:52:13.000000 liveramp_automation-1.3.2/liveramp_automation/helpers/file.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     7284 2024-03-14 07:40:53.000000 liveramp_automation-1.3.2/liveramp_automation/helpers/fixture.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     6180 2024-04-16 03:15:54.000000 liveramp_automation-1.3.2/liveramp_automation/helpers/login.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    10440 2024-04-16 03:23:44.000000 liveramp_automation-1.3.2/liveramp_automation/helpers/notification.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 06:13:26.385025 liveramp_automation-1.3.2/liveramp_automation/utils/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.3.2/liveramp_automation/utils/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1934 2024-04-01 03:10:38.000000 liveramp_automation-1.3.2/liveramp_automation/utils/allure.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     6445 2024-03-01 06:50:54.000000 liveramp_automation-1.3.2/liveramp_automation/utils/log.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4872 2024-04-16 03:16:13.000000 liveramp_automation-1.3.2/liveramp_automation/utils/pagerduty.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1728 2023-08-16 02:33:25.000000 liveramp_automation-1.3.2/liveramp_automation/utils/parsers.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4025 2023-09-13 03:08:07.000000 liveramp_automation-1.3.2/liveramp_automation/utils/playwright.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    10164 2023-12-01 07:13:44.000000 liveramp_automation-1.3.2/liveramp_automation/utils/request.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    49909 2023-12-11 09:06:44.000000 liveramp_automation-1.3.2/liveramp_automation/utils/selenium.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    10500 2024-03-05 09:08:06.000000 liveramp_automation-1.3.2/liveramp_automation/utils/slack.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1660 2023-12-11 09:11:45.000000 liveramp_automation-1.3.2/liveramp_automation/utils/time.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 06:13:26.392065 liveramp_automation-1.3.2/liveramp_automation.egg-info/
+-rw-r--r--   0 jasqia     (503) staff       (20)     2954 2024-04-17 06:13:26.000000 liveramp_automation-1.3.2/liveramp_automation.egg-info/PKG-INFO
+-rw-r--r--   0 jasqia     (503) staff       (20)     1501 2024-04-17 06:13:26.000000 liveramp_automation-1.3.2/liveramp_automation.egg-info/SOURCES.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)        1 2024-04-17 06:13:26.000000 liveramp_automation-1.3.2/liveramp_automation.egg-info/dependency_links.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)      443 2024-04-17 06:13:26.000000 liveramp_automation-1.3.2/liveramp_automation.egg-info/requires.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)       26 2024-04-17 06:13:26.000000 liveramp_automation-1.3.2/liveramp_automation.egg-info/top_level.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)       38 2024-04-17 06:13:26.392991 liveramp_automation-1.3.2/setup.cfg
+-rw-r--r--   0 jasqia     (503) staff       (20)     1474 2024-04-17 06:12:35.000000 liveramp_automation-1.3.2/setup.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 06:13:26.385435 liveramp_automation-1.3.2/tests/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.3.2/tests/__init__.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 06:13:26.387848 liveramp_automation-1.3.2/tests/test_helpers/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:03.000000 liveramp_automation-1.3.2/tests/test_helpers/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     2599 2024-04-01 03:10:38.000000 liveramp_automation-1.3.2/tests/test_helpers/test_bigquery.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     2345 2024-04-01 03:35:43.000000 liveramp_automation-1.3.2/tests/test_helpers/test_bucket.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4132 2024-04-01 03:42:11.000000 liveramp_automation-1.3.2/tests/test_helpers/test_file.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1247 2024-03-14 08:05:22.000000 liveramp_automation-1.3.2/tests/test_helpers/test_fixtures.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1676 2024-03-14 09:32:27.000000 liveramp_automation-1.3.2/tests/test_helpers/test_login.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     3508 2024-03-05 09:08:06.000000 liveramp_automation-1.3.2/tests/test_helpers/test_notification.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-04-17 06:13:26.391500 liveramp_automation-1.3.2/tests/test_utils/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.3.2/tests/test_utils/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1832 2024-03-28 09:52:13.000000 liveramp_automation-1.3.2/tests/test_utils/test_log.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4783 2024-03-28 09:52:13.000000 liveramp_automation-1.3.2/tests/test_utils/test_pagerduty.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     3337 2024-04-01 03:10:38.000000 liveramp_automation-1.3.2/tests/test_utils/test_parsers.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1014 2024-03-14 08:40:57.000000 liveramp_automation-1.3.2/tests/test_utils/test_playwright.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    13489 2024-04-01 03:10:38.000000 liveramp_automation-1.3.2/tests/test_utils/test_request.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    39767 2024-03-28 09:52:13.000000 liveramp_automation-1.3.2/tests/test_utils/test_selenium.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     6615 2024-03-28 09:52:13.000000 liveramp_automation-1.3.2/tests/test_utils/test_slack.py
+-rw-r--r--   0 jasqia     (503) staff       (20)      742 2024-03-14 08:51:35.000000 liveramp_automation-1.3.2/tests/test_utils/test_version.py
```

### Comparing `liveramp_automation-1.3.1/LICENSE` & `liveramp_automation-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.1/PKG-INFO` & `liveramp_automation-1.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: liveramp_automation
-Version: 1.3.1
+Version: 1.3.2
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/liveramp-automation
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: allure-pytest-bdd
 Requires-Dist: allure-python-commons
 Requires-Dist: boto3
+Requires-Dist: certifi
 Requires-Dist: datadog
 Requires-Dist: db-dtypes
+Requires-Dist: dnspython
 Requires-Dist: google
 Requires-Dist: google-api-core
 Requires-Dist: google-auth
 Requires-Dist: google-cloud-bigquery
 Requires-Dist: google-cloud-core
 Requires-Dist: google-cloud-storage
 Requires-Dist: google-crc32c
```

### Comparing `liveramp_automation-1.3.1/README.md` & `liveramp_automation-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.1/liveramp_automation/helpers/bigquery.py` & `liveramp_automation-1.3.2/liveramp_automation/helpers/bigquery.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.1/liveramp_automation/helpers/bucket.py` & `liveramp_automation-1.3.2/liveramp_automation/helpers/bucket.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
             if not os.path.exists(local_file_path):
                 Logger.error(f"Local file path does not exist: {local_file_path}")
 
             if os.path.isfile(local_file_path):
                 blob = self.bucket.blob(os.path.join(cloud_blob_path, os.path.basename(local_file_path)))
                 blob.upload_from_filename(local_file_path)
-                Logger.info(f"Item Uploded on Path = {local_file_path}")
+                Logger.info(f"Item Uploaded on Path = {local_file_path}")
 
             for item in glob.glob(os.path.join(local_file_path, '*')):
                 if os.path.isfile(item):
                     if item == ".keep":
                         continue
                     blob = self.bucket.blob(os.path.join(cloud_blob_path, os.path.basename(item)))
                     blob.upload_from_filename(item)
```

### Comparing `liveramp_automation-1.3.1/liveramp_automation/helpers/file.py` & `liveramp_automation-1.3.2/liveramp_automation/helpers/file.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.1/liveramp_automation/helpers/fixture.py` & `liveramp_automation-1.3.2/liveramp_automation/helpers/fixture.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.1/liveramp_automation/helpers/login.py` & `liveramp_automation-1.3.2/liveramp_automation/helpers/login.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.1/liveramp_automation/helpers/notification.py` & `liveramp_automation-1.3.2/liveramp_automation/helpers/notification.py`

 * *Files 14% similar despite different names*

```diff
@@ -219,14 +219,29 @@
         pagerduty_client = PagerDutyClient(api_key)
         return pagerduty_client.list_open_incidents(service_id)
 
     def oc_notify(self):
         return
 
     @staticmethod
-    def deal_enqueue(api_key: str, service_id: str, event_action: str, summary: str, details: dict = None,
-                     dedup_key: str = None,
-                     escalation_policy_id: str = None, assignee: str = None) -> Tuple[Optional[str], Optional[str]]:
+    def deal_enqueue(api_key: str,
+                     service_id: str,
+                     event_action: str,
+                     summary: str,
+                     custom_details: dict = None,
+                     dedup_key: str = None):
+        """
+        Static method to send PagerDuty a trigger event to report a new problem,
+        or update an ongoing problem, depending on the event type.
+        https://developer.pagerduty.com/api-reference/368ae3d938c9e-send-an-event-to-pager-duty
+        Args:
+            api_key (str): The PagerDuty API key.
+                           The GUID of one of your Events API V2 integrations.
+                           This is the "Integration Key" listed on the Events API V2 integration's detail page.
+            service_id (str): The ID of the PagerDuty service to trigger the incident on.
+            event_action (str): The type of event. Can be trigger, acknowledge or resolve.
+            summary (str): Summary or title of the incident.
+            custom_details (dict, optional): Additional details about the event and affected system. Defaults to None.
+            dedup_key (str, optional): The unique value to differ events.
+        """
         pagerduty_client = PagerDutyClient(api_key)
-        return pagerduty_client.deal_enqueue(service_id, event_action, summary, details, dedup_key,
-                                             escalation_policy_id,
-                                             assignee)
+        return pagerduty_client.deal_enqueue(service_id, event_action, summary, custom_details, dedup_key)
```

### Comparing `liveramp_automation-1.3.1/liveramp_automation/utils/allure.py` & `liveramp_automation-1.3.2/liveramp_automation/utils/allure.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.1/liveramp_automation/utils/log.py` & `liveramp_automation-1.3.2/liveramp_automation/utils/log.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.1/liveramp_automation/utils/pagerduty.py` & `liveramp_automation-1.3.2/liveramp_automation/utils/pagerduty.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,27 +92,26 @@
         response.raise_for_status()
         Logger.debug(f"Received the response: {response.json()}")
         incidents = response.json().get('incidents', [])
         incident_list = [{'id': incident['id'], 'url': incident['html_url']} for incident in incidents]
         return incident_list
 
     def deal_enqueue(self, service_id: str, event_action: str, dedup_key: str, summary: str,
-                     details: Optional[Dict[str, Any]] = None,
-                     escalation_policy_id: Optional[str] = None,
-                     assignee: Optional[str] = None):
+                     custom_details: Optional[Dict[str, Any]] = None):
         endpoint = f'{self.event_url}/v2/enqueue'
         json_data = {
             "dedup_key": dedup_key,
             "event_action": event_action,
             "payload": {
                 "severity": "critical",
             },
             "routing_key": service_id
         }
         if summary:
             json_data["payload"]['summary'] = summary
 
-        if details:
-            json_data["payload"]['source'] = details
+        if custom_details:
+            json_data["payload"]['custom_details'] = custom_details
+
         Logger.debug(f"Sending a request - url: {endpoint}, payload: {json_data}, headers: {self.headers}")
         response = requests.post(endpoint, json=json_data, headers=self.headers)
         return response
```

### Comparing `liveramp_automation-1.3.1/liveramp_automation/utils/parsers.py` & `liveramp_automation-1.3.2/liveramp_automation/utils/parsers.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.1/liveramp_automation/utils/playwright.py` & `liveramp_automation-1.3.2/liveramp_automation/utils/playwright.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.1/liveramp_automation/utils/request.py` & `liveramp_automation-1.3.2/liveramp_automation/utils/request.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.1/liveramp_automation/utils/selenium.py` & `liveramp_automation-1.3.2/liveramp_automation/utils/selenium.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.1/liveramp_automation/utils/slack.py` & `liveramp_automation-1.3.2/liveramp_automation/utils/slack.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.1/liveramp_automation/utils/time.py` & `liveramp_automation-1.3.2/liveramp_automation/utils/time.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.1/liveramp_automation.egg-info/PKG-INFO` & `liveramp_automation-1.3.2/liveramp_automation.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: liveramp-automation
-Version: 1.3.1
+Version: 1.3.2
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/liveramp-automation
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: allure-pytest-bdd
 Requires-Dist: allure-python-commons
 Requires-Dist: boto3
+Requires-Dist: certifi
 Requires-Dist: datadog
 Requires-Dist: db-dtypes
+Requires-Dist: dnspython
 Requires-Dist: google
 Requires-Dist: google-api-core
 Requires-Dist: google-auth
 Requires-Dist: google-cloud-bigquery
 Requires-Dist: google-cloud-core
 Requires-Dist: google-cloud-storage
 Requires-Dist: google-crc32c
```

### Comparing `liveramp_automation-1.3.1/liveramp_automation.egg-info/SOURCES.txt` & `liveramp_automation-1.3.2/liveramp_automation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.1/setup.py` & `liveramp_automation-1.3.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,16 +20,18 @@
     long_description_content_type="text/markdown",
     url="https://github.com/LiveRamp/liveramp-automation",
     packages=find_packages(),
     install_requires=[
         'allure-pytest-bdd',
         'allure-python-commons',
         'boto3',
+        'certifi',
         'datadog',
         'db-dtypes',
+        'dnspython',
         'google',
         'google-api-core',
         'google-auth',
         'google-cloud-bigquery',
         'google-cloud-core',
         'google-cloud-storage',
         'google-crc32c',
```

### Comparing `liveramp_automation-1.3.1/tests/test_helpers/test_bigquery.py` & `liveramp_automation-1.3.2/tests/test_helpers/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.1/tests/test_helpers/test_bucket.py` & `liveramp_automation-1.3.2/tests/test_helpers/test_bucket.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.1/tests/test_helpers/test_file.py` & `liveramp_automation-1.3.2/tests/test_helpers/test_file.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.1/tests/test_helpers/test_fixtures.py` & `liveramp_automation-1.3.2/tests/test_helpers/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.1/tests/test_helpers/test_login.py` & `liveramp_automation-1.3.2/tests/test_helpers/test_login.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.1/tests/test_helpers/test_notification.py` & `liveramp_automation-1.3.2/tests/test_helpers/test_notification.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.1/tests/test_utils/test_log.py` & `liveramp_automation-1.3.2/tests/test_utils/test_log.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.1/tests/test_utils/test_pagerduty.py` & `liveramp_automation-1.3.2/tests/test_utils/test_pagerduty.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.1/tests/test_utils/test_parsers.py` & `liveramp_automation-1.3.2/tests/test_utils/test_parsers.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.1/tests/test_utils/test_playwright.py` & `liveramp_automation-1.3.2/tests/test_utils/test_playwright.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.1/tests/test_utils/test_request.py` & `liveramp_automation-1.3.2/tests/test_utils/test_request.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.1/tests/test_utils/test_selenium.py` & `liveramp_automation-1.3.2/tests/test_utils/test_selenium.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.1/tests/test_utils/test_slack.py` & `liveramp_automation-1.3.2/tests/test_utils/test_slack.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.3.1/tests/test_utils/test_version.py` & `liveramp_automation-1.3.2/tests/test_utils/test_version.py`

 * *Files identical despite different names*

