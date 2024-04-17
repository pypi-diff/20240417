# Comparing `tmp/lennoxs30api-0.2.8.tar.gz` & `tmp/lennoxs30api-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lennoxs30api-0.2.8.tar", last modified: Thu Jun 22 20:08:24 2023, max compression
+gzip compressed data, was "lennoxs30api-0.2.9.tar", last modified: Fri Aug 18 13:07:02 2023, max compression
```

## Comparing `lennoxs30api-0.2.8.tar` & `lennoxs30api-0.2.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0 pete      (1000) pete      (1000)        0 2023-06-22 20:08:24.972399 lennoxs30api-0.2.8/
--rwxrwxrwx   0 pete      (1000) pete      (1000)     1092 2021-06-16 19:56:17.000000 lennoxs30api-0.2.8/LICENSE
--rwxrwxrwx   0 pete      (1000) pete      (1000)     2535 2023-06-22 20:08:24.969397 lennoxs30api-0.2.8/PKG-INFO
--rwxrwxrwx   0 pete      (1000) pete      (1000)     2140 2021-07-18 14:46:26.000000 lennoxs30api-0.2.8/README.md
-drwxrwxrwx   0 pete      (1000) pete      (1000)        0 2023-06-22 20:08:24.876053 lennoxs30api-0.2.8/lennoxs30api/
--rwxrwxrwx   0 pete      (1000) pete      (1000)      171 2023-06-22 20:07:02.000000 lennoxs30api-0.2.8/lennoxs30api/__init__.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     3188 2023-04-23 14:36:07.000000 lennoxs30api-0.2.8/lennoxs30api/lennox_ble.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     5357 2022-09-03 00:30:25.000000 lennoxs30api-0.2.8/lennoxs30api/lennox_equipment.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)    29143 2022-10-18 13:38:00.000000 lennoxs30api-0.2.8/lennoxs30api/lennox_errors.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)      627 2021-12-24 15:46:31.000000 lennoxs30api-0.2.8/lennoxs30api/lennox_home.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     1613 2021-06-25 11:10:06.000000 lennoxs30api-0.2.8/lennoxs30api/lennox_period.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     1118 2021-06-25 11:10:06.000000 lennoxs30api-0.2.8/lennoxs30api/lennox_schedule.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     2938 2022-05-22 21:24:48.000000 lennoxs30api-0.2.8/lennoxs30api/message_logger.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     3903 2023-04-23 14:36:07.000000 lennoxs30api-0.2.8/lennoxs30api/metrics.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)   131305 2023-06-22 20:07:02.000000 lennoxs30api-0.2.8/lennoxs30api/s30api_async.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     2964 2022-12-15 21:56:21.000000 lennoxs30api-0.2.8/lennoxs30api/s30exception.py
--rwxrwxrwx   0 pete      (1000) pete      (1000)     2414 2023-04-23 14:36:07.000000 lennoxs30api-0.2.8/lennoxs30api/subscriber_base.py
-drwxrwxrwx   0 pete      (1000) pete      (1000)        0 2023-06-22 20:08:24.949397 lennoxs30api-0.2.8/lennoxs30api.egg-info/
--rwxrwxrwx   0 pete      (1000) pete      (1000)     2535 2023-06-22 20:08:24.000000 lennoxs30api-0.2.8/lennoxs30api.egg-info/PKG-INFO
--rwxrwxrwx   0 pete      (1000) pete      (1000)      555 2023-06-22 20:08:24.000000 lennoxs30api-0.2.8/lennoxs30api.egg-info/SOURCES.txt
--rwxrwxrwx   0 pete      (1000) pete      (1000)        1 2023-06-22 20:08:24.000000 lennoxs30api-0.2.8/lennoxs30api.egg-info/dependency_links.txt
--rwxrwxrwx   0 pete      (1000) pete      (1000)        8 2023-06-22 20:08:24.000000 lennoxs30api-0.2.8/lennoxs30api.egg-info/requires.txt
--rwxrwxrwx   0 pete      (1000) pete      (1000)       13 2023-06-22 20:08:24.000000 lennoxs30api-0.2.8/lennoxs30api.egg-info/top_level.txt
--rwxrwxrwx   0 pete      (1000) pete      (1000)       38 2023-06-22 20:08:24.973398 lennoxs30api-0.2.8/setup.cfg
--rwxrwxrwx   0 pete      (1000) pete      (1000)      697 2023-06-22 20:07:02.000000 lennoxs30api-0.2.8/setup.py
+drwxrwxrwx   0 pete      (1000) pete      (1000)        0 2023-08-18 13:07:02.459020 lennoxs30api-0.2.9/
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     1092 2021-06-16 19:56:17.000000 lennoxs30api-0.2.9/LICENSE
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     2535 2023-08-18 13:07:02.457017 lennoxs30api-0.2.9/PKG-INFO
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     2140 2021-07-18 14:46:26.000000 lennoxs30api-0.2.9/README.md
+drwxrwxrwx   0 pete      (1000) pete      (1000)        0 2023-08-18 13:07:02.377015 lennoxs30api-0.2.9/lennoxs30api/
+-rwxrwxrwx   0 pete      (1000) pete      (1000)      171 2023-08-18 13:02:37.000000 lennoxs30api-0.2.9/lennoxs30api/__init__.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     3188 2023-04-23 14:36:07.000000 lennoxs30api-0.2.9/lennoxs30api/lennox_ble.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     5357 2022-09-03 00:30:25.000000 lennoxs30api-0.2.9/lennoxs30api/lennox_equipment.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)    29143 2022-10-18 13:38:00.000000 lennoxs30api-0.2.9/lennoxs30api/lennox_errors.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)      627 2021-12-24 15:46:31.000000 lennoxs30api-0.2.9/lennoxs30api/lennox_home.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     1613 2021-06-25 11:10:06.000000 lennoxs30api-0.2.9/lennoxs30api/lennox_period.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     1118 2021-06-25 11:10:06.000000 lennoxs30api-0.2.9/lennoxs30api/lennox_schedule.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     2938 2022-05-22 21:24:48.000000 lennoxs30api-0.2.9/lennoxs30api/message_logger.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     3903 2023-04-23 14:36:07.000000 lennoxs30api-0.2.9/lennoxs30api/metrics.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)   131304 2023-08-18 12:58:00.000000 lennoxs30api-0.2.9/lennoxs30api/s30api_async.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     2964 2022-12-15 21:56:21.000000 lennoxs30api-0.2.9/lennoxs30api/s30exception.py
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     2414 2023-04-23 14:36:07.000000 lennoxs30api-0.2.9/lennoxs30api/subscriber_base.py
+drwxrwxrwx   0 pete      (1000) pete      (1000)        0 2023-08-18 13:07:02.443016 lennoxs30api-0.2.9/lennoxs30api.egg-info/
+-rwxrwxrwx   0 pete      (1000) pete      (1000)     2535 2023-08-18 13:07:02.000000 lennoxs30api-0.2.9/lennoxs30api.egg-info/PKG-INFO
+-rwxrwxrwx   0 pete      (1000) pete      (1000)      555 2023-08-18 13:07:02.000000 lennoxs30api-0.2.9/lennoxs30api.egg-info/SOURCES.txt
+-rwxrwxrwx   0 pete      (1000) pete      (1000)        1 2023-08-18 13:07:02.000000 lennoxs30api-0.2.9/lennoxs30api.egg-info/dependency_links.txt
+-rwxrwxrwx   0 pete      (1000) pete      (1000)        8 2023-08-18 13:07:02.000000 lennoxs30api-0.2.9/lennoxs30api.egg-info/requires.txt
+-rwxrwxrwx   0 pete      (1000) pete      (1000)       13 2023-08-18 13:07:02.000000 lennoxs30api-0.2.9/lennoxs30api.egg-info/top_level.txt
+-rwxrwxrwx   0 pete      (1000) pete      (1000)       38 2023-08-18 13:07:02.461017 lennoxs30api-0.2.9/setup.cfg
+-rwxrwxrwx   0 pete      (1000) pete      (1000)      697 2023-08-18 13:02:39.000000 lennoxs30api-0.2.9/setup.py
```

### Comparing `lennoxs30api-0.2.8/LICENSE` & `lennoxs30api-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.8/PKG-INFO` & `lennoxs30api-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lennoxs30api
-Version: 0.2.8
+Version: 0.2.9
 Summary: API Wrapper for Lennox S30 Cloud and LAN API
 Home-page: https://github.com/PeteRager/lennoxs30api
 Author: Pete Rage
 Author-email: pete.rager@x.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lennoxs30api-0.2.8/README.md` & `lennoxs30api-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.8/lennoxs30api/lennox_ble.py` & `lennoxs30api-0.2.9/lennoxs30api/lennox_ble.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.8/lennoxs30api/lennox_equipment.py` & `lennoxs30api-0.2.9/lennoxs30api/lennox_equipment.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.8/lennoxs30api/lennox_errors.py` & `lennoxs30api-0.2.9/lennoxs30api/lennox_errors.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.8/lennoxs30api/lennox_home.py` & `lennoxs30api-0.2.9/lennoxs30api/lennox_home.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.8/lennoxs30api/lennox_period.py` & `lennoxs30api-0.2.9/lennoxs30api/lennox_period.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.8/lennoxs30api/lennox_schedule.py` & `lennoxs30api-0.2.9/lennoxs30api/lennox_schedule.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.8/lennoxs30api/message_logger.py` & `lennoxs30api-0.2.9/lennoxs30api/message_logger.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.8/lennoxs30api/metrics.py` & `lennoxs30api-0.2.9/lennoxs30api/metrics.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.8/lennoxs30api/s30api_async.py` & `lennoxs30api-0.2.9/lennoxs30api/s30api_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -677,15 +677,15 @@
             }
             params = {
                 "Direction": "Oldest-to-Newest",
                 "MessageCount": "10",
                 "StartTime": "1",
             }
             if self.isLANConnection:
-                params["LongPollingTimeout"] = "15"
+                params["LongPollingTimeout"] = "5"
             else:
                 params["LongPollingTimeout"] = "0"
 
             resp = await self.get(url, headers=headers, params=params)
             self.metrics.inc_receive_bytes(resp.content_length)
             if resp.status == 200:
                 resp_txt = await resp.text()
```

### Comparing `lennoxs30api-0.2.8/lennoxs30api/s30exception.py` & `lennoxs30api-0.2.9/lennoxs30api/s30exception.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.8/lennoxs30api/subscriber_base.py` & `lennoxs30api-0.2.9/lennoxs30api/subscriber_base.py`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.8/lennoxs30api.egg-info/PKG-INFO` & `lennoxs30api-0.2.9/lennoxs30api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lennoxs30api
-Version: 0.2.8
+Version: 0.2.9
 Summary: API Wrapper for Lennox S30 Cloud and LAN API
 Home-page: https://github.com/PeteRager/lennoxs30api
 Author: Pete Rage
 Author-email: pete.rager@x.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lennoxs30api-0.2.8/lennoxs30api.egg-info/SOURCES.txt` & `lennoxs30api-0.2.9/lennoxs30api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lennoxs30api-0.2.8/setup.py` & `lennoxs30api-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lennoxs30api",
-    version="0.2.8",
+    version="0.2.9",
     description="API Wrapper for Lennox S30 Cloud and LAN API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/PeteRager/lennoxs30api",
     author="Pete Rage",
     author_email="pete.rager@x.com",
     license="MIT",
```

