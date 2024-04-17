# Comparing `tmp/pyhomelink-0.1.8.tar.gz` & `tmp/pyhomelink-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhomelink-0.1.8.tar", last modified: Mon Dec 11 11:37:22 2023, max compression
+gzip compressed data, was "pyhomelink-0.1.9.tar", last modified: Wed Jan 24 18:10:05 2024, max compression
```

## Comparing `pyhomelink-0.1.8.tar` & `pyhomelink-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 roger     (1000) roger     (1000)        0 2023-12-11 11:37:22.000000 pyhomelink-0.1.8/
--rw-r--r--   0 roger     (1000) roger     (1000)     1068 2023-09-14 13:55:28.000000 pyhomelink-0.1.8/LICENSE
--rw-r--r--   0 roger     (1000) roger     (1000)     2700 2023-12-11 11:37:22.000000 pyhomelink-0.1.8/PKG-INFO
--rw-r--r--   0 roger     (1000) roger     (1000)     1824 2023-12-11 09:18:34.000000 pyhomelink-0.1.8/README.md
-drwxr-xr-x   0 roger     (1000) roger     (1000)        0 2023-12-11 11:37:22.000000 pyhomelink-0.1.8/pyhomelink/
--rw-r--r--   0 roger     (1000) roger     (1000)      127 2023-12-11 11:37:04.000000 pyhomelink-0.1.8/pyhomelink/__init__.py
--rw-r--r--   0 roger     (1000) roger     (1000)     3201 2023-12-11 11:37:04.000000 pyhomelink-0.1.8/pyhomelink/alert.py
--rw-r--r--   0 roger     (1000) roger     (1000)     7078 2023-12-11 11:37:04.000000 pyhomelink-0.1.8/pyhomelink/api.py
--rw-r--r--   0 roger     (1000) roger     (1000)     1840 2023-12-11 11:37:04.000000 pyhomelink-0.1.8/pyhomelink/auth.py
--rw-r--r--   0 roger     (1000) roger     (1000)     1271 2023-12-11 11:37:04.000000 pyhomelink-0.1.8/pyhomelink/const.py
--rw-r--r--   0 roger     (1000) roger     (1000)     7261 2023-12-11 11:37:04.000000 pyhomelink-0.1.8/pyhomelink/device.py
--rw-r--r--   0 roger     (1000) roger     (1000)      298 2023-12-11 11:37:04.000000 pyhomelink-0.1.8/pyhomelink/exceptions.py
--rw-r--r--   0 roger     (1000) roger     (1000)     1839 2023-12-11 11:37:04.000000 pyhomelink-0.1.8/pyhomelink/insight.py
--rw-r--r--   0 roger     (1000) roger     (1000)     1290 2023-12-11 11:37:04.000000 pyhomelink-0.1.8/pyhomelink/lookup.py
--rw-r--r--   0 roger     (1000) roger     (1000)     4753 2023-12-11 11:37:04.000000 pyhomelink-0.1.8/pyhomelink/property.py
--rw-r--r--   0 roger     (1000) roger     (1000)     3659 2023-12-11 11:37:04.000000 pyhomelink-0.1.8/pyhomelink/reading.py
--rw-r--r--   0 roger     (1000) roger     (1000)      482 2023-12-11 11:37:04.000000 pyhomelink-0.1.8/pyhomelink/utils.py
--rw-r--r--   0 roger     (1000) roger     (1000)       50 2023-12-11 11:37:04.000000 pyhomelink-0.1.8/pyhomelink/version.py
-drwxr-xr-x   0 roger     (1000) roger     (1000)        0 2023-12-11 11:37:22.000000 pyhomelink-0.1.8/pyhomelink.egg-info/
--rw-r--r--   0 roger     (1000) roger     (1000)     2700 2023-12-11 11:37:21.000000 pyhomelink-0.1.8/pyhomelink.egg-info/PKG-INFO
--rw-r--r--   0 roger     (1000) roger     (1000)      504 2023-12-11 11:37:21.000000 pyhomelink-0.1.8/pyhomelink.egg-info/SOURCES.txt
--rw-r--r--   0 roger     (1000) roger     (1000)        1 2023-12-11 11:37:21.000000 pyhomelink-0.1.8/pyhomelink.egg-info/dependency_links.txt
--rw-r--r--   0 roger     (1000) roger     (1000)        1 2023-09-14 14:18:39.000000 pyhomelink-0.1.8/pyhomelink.egg-info/not-zip-safe
--rw-r--r--   0 roger     (1000) roger     (1000)       15 2023-12-11 11:37:21.000000 pyhomelink-0.1.8/pyhomelink.egg-info/requires.txt
--rw-r--r--   0 roger     (1000) roger     (1000)       16 2023-12-11 11:37:21.000000 pyhomelink-0.1.8/pyhomelink.egg-info/top_level.txt
--rw-r--r--   0 roger     (1000) roger     (1000)       38 2023-12-11 11:37:22.000000 pyhomelink-0.1.8/setup.cfg
--rw-r--r--   0 roger     (1000) roger     (1000)     1464 2023-10-07 17:06:22.000000 pyhomelink-0.1.8/setup.py
+drwxr-xr-x   0 roger     (1000) roger     (1000)        0 2024-01-24 18:10:05.000000 pyhomelink-0.1.9/
+-rw-r--r--   0 roger     (1000) roger     (1000)     1068 2023-09-14 13:55:28.000000 pyhomelink-0.1.9/LICENSE
+-rw-r--r--   0 roger     (1000) roger     (1000)     2700 2024-01-24 18:10:05.000000 pyhomelink-0.1.9/PKG-INFO
+-rw-r--r--   0 roger     (1000) roger     (1000)     1824 2024-01-08 09:24:13.000000 pyhomelink-0.1.9/README.md
+drwxr-xr-x   0 roger     (1000) roger     (1000)        0 2024-01-24 18:10:05.000000 pyhomelink-0.1.9/pyhomelink/
+-rw-r--r--   0 roger     (1000) roger     (1000)      127 2024-01-24 18:09:32.000000 pyhomelink-0.1.9/pyhomelink/__init__.py
+-rw-r--r--   0 roger     (1000) roger     (1000)     3201 2024-01-24 18:09:32.000000 pyhomelink-0.1.9/pyhomelink/alert.py
+-rw-r--r--   0 roger     (1000) roger     (1000)     7076 2024-01-24 18:09:32.000000 pyhomelink-0.1.9/pyhomelink/api.py
+-rw-r--r--   0 roger     (1000) roger     (1000)     2901 2024-01-24 18:09:32.000000 pyhomelink-0.1.9/pyhomelink/auth.py
+-rw-r--r--   0 roger     (1000) roger     (1000)     1271 2024-01-24 18:09:32.000000 pyhomelink-0.1.9/pyhomelink/const.py
+-rw-r--r--   0 roger     (1000) roger     (1000)     7257 2024-01-24 18:09:32.000000 pyhomelink-0.1.9/pyhomelink/device.py
+-rw-r--r--   0 roger     (1000) roger     (1000)      298 2024-01-24 18:09:32.000000 pyhomelink-0.1.9/pyhomelink/exceptions.py
+-rw-r--r--   0 roger     (1000) roger     (1000)     2006 2024-01-24 18:09:32.000000 pyhomelink-0.1.9/pyhomelink/insight.py
+-rw-r--r--   0 roger     (1000) roger     (1000)     1290 2024-01-24 18:09:32.000000 pyhomelink-0.1.9/pyhomelink/lookup.py
+-rw-r--r--   0 roger     (1000) roger     (1000)     4753 2024-01-24 18:09:32.000000 pyhomelink-0.1.9/pyhomelink/property.py
+-rw-r--r--   0 roger     (1000) roger     (1000)     3659 2024-01-24 18:09:32.000000 pyhomelink-0.1.9/pyhomelink/reading.py
+-rw-r--r--   0 roger     (1000) roger     (1000)      482 2024-01-24 18:09:32.000000 pyhomelink-0.1.9/pyhomelink/utils.py
+-rw-r--r--   0 roger     (1000) roger     (1000)       50 2024-01-24 18:09:32.000000 pyhomelink-0.1.9/pyhomelink/version.py
+drwxr-xr-x   0 roger     (1000) roger     (1000)        0 2024-01-24 18:10:05.000000 pyhomelink-0.1.9/pyhomelink.egg-info/
+-rw-r--r--   0 roger     (1000) roger     (1000)     2700 2024-01-24 18:10:05.000000 pyhomelink-0.1.9/pyhomelink.egg-info/PKG-INFO
+-rw-r--r--   0 roger     (1000) roger     (1000)      504 2024-01-24 18:10:05.000000 pyhomelink-0.1.9/pyhomelink.egg-info/SOURCES.txt
+-rw-r--r--   0 roger     (1000) roger     (1000)        1 2024-01-24 18:10:05.000000 pyhomelink-0.1.9/pyhomelink.egg-info/dependency_links.txt
+-rw-r--r--   0 roger     (1000) roger     (1000)        1 2023-09-14 14:18:39.000000 pyhomelink-0.1.9/pyhomelink.egg-info/not-zip-safe
+-rw-r--r--   0 roger     (1000) roger     (1000)       15 2024-01-24 18:10:05.000000 pyhomelink-0.1.9/pyhomelink.egg-info/requires.txt
+-rw-r--r--   0 roger     (1000) roger     (1000)       16 2024-01-24 18:10:05.000000 pyhomelink-0.1.9/pyhomelink.egg-info/top_level.txt
+-rw-r--r--   0 roger     (1000) roger     (1000)       38 2024-01-24 18:10:05.000000 pyhomelink-0.1.9/setup.cfg
+-rw-r--r--   0 roger     (1000) roger     (1000)     1464 2023-10-07 17:06:22.000000 pyhomelink-0.1.9/setup.py
```

### Comparing `pyhomelink-0.1.8/LICENSE` & `pyhomelink-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhomelink-0.1.8/PKG-INFO` & `pyhomelink-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhomelink
-Version: 0.1.8
+Version: 0.1.9
 Summary: Library for AICO HomeLINK
 Home-page: https://github.com/RogerSelwyn/python_homelink
 Author: Roger Selwyn
 Author-email: roger.selwyn@users.noreply.github.com
 Maintainer: RogerSelwyn
 Maintainer-email: roger.selwyn@users.noreply.github.com
 License: MIT
@@ -22,15 +22,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![CodeFactor](https://www.codefactor.io/repository/github/rogerselwyn/python_homelink/badge)](https://www.codefactor.io/repository/github/rogerselwyn/python_homelink)
 [![CodeQL](https://github.com/RogerSelwyn/python_homelink/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/RogerSelwyn/python_homelink/actions/workflows/github-code-scanning/codeql)
 [![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/pyhomelink)](https://libraries.io/pypi/pyhomelink)
 
-![GitHub release](https://img.shields.io/github/v/release/RogerSelwyn/python_homelink) [![maintained](https://img.shields.io/maintenance/yes/2023.svg)](#)
+![GitHub release](https://img.shields.io/github/v/release/RogerSelwyn/python_homelink) [![maintained](https://img.shields.io/maintenance/yes/2024.svg)](#)
 [![maintainer](https://img.shields.io/badge/maintainer-%20%40RogerSelwyn-blue.svg)](https://github.com/RogerSelwyn)
 ![PyPI - Status](https://img.shields.io/pypi/status/pyhomelink)
 [![PyPI](https://img.shields.io/pypi/v/pyhomelink)](https://pypi.org/project/pyhomelink/)
 [![GitHub](https://img.shields.io/github/license/rogerselwyn/python_homelink)](https://github.com/RogerSewlwyn/python_homelink/blob/main/LICENSE)
 
 
 # python_homelink
```

### Comparing `pyhomelink-0.1.8/README.md` & `pyhomelink-0.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [![CodeFactor](https://www.codefactor.io/repository/github/rogerselwyn/python_homelink/badge)](https://www.codefactor.io/repository/github/rogerselwyn/python_homelink)
 [![CodeQL](https://github.com/RogerSelwyn/python_homelink/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/RogerSelwyn/python_homelink/actions/workflows/github-code-scanning/codeql)
 [![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/pyhomelink)](https://libraries.io/pypi/pyhomelink)
 
-![GitHub release](https://img.shields.io/github/v/release/RogerSelwyn/python_homelink) [![maintained](https://img.shields.io/maintenance/yes/2023.svg)](#)
+![GitHub release](https://img.shields.io/github/v/release/RogerSelwyn/python_homelink) [![maintained](https://img.shields.io/maintenance/yes/2024.svg)](#)
 [![maintainer](https://img.shields.io/badge/maintainer-%20%40RogerSelwyn-blue.svg)](https://github.com/RogerSelwyn)
 ![PyPI - Status](https://img.shields.io/pypi/status/pyhomelink)
 [![PyPI](https://img.shields.io/pypi/v/pyhomelink)](https://pypi.org/project/pyhomelink/)
 [![GitHub](https://img.shields.io/github/license/rogerselwyn/python_homelink)](https://github.com/RogerSewlwyn/python_homelink/blob/main/LICENSE)
 
 
 # python_homelink
```

### Comparing `pyhomelink-0.1.8/pyhomelink/alert.py` & `pyhomelink-0.1.9/pyhomelink/alert.py`

 * *Files identical despite different names*

### Comparing `pyhomelink-0.1.8/pyhomelink/api.py` & `pyhomelink-0.1.9/pyhomelink/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,21 +139,21 @@
     ) -> DeviceReading:
         """Return the Device Alerts."""
         url = HomeLINKEndpoint.DEVICE_READINGS.format(
             serialnumber=serialnumber,
             readingtype=readingtype,
         )
         if start or end:
-            url = url + "?"
+            url = f"{url}?"
         if start:
-            url = url + f"start={start}"
+            url = f"{url}start={start}"
         if start and end:
-            url = url + "&"
+            url = f"{url}&"
         if end:
-            url = url + f"end={end}"
+            url = f"{url}end={end}"
         resp = await self.auth.request(
             "get",
             url,
         )
         check_status(resp)
         return DeviceReading(await resp.json())
```

### Comparing `pyhomelink-0.1.8/pyhomelink/const.py` & `pyhomelink-0.1.9/pyhomelink/const.py`

 * *Files identical despite different names*

### Comparing `pyhomelink-0.1.8/pyhomelink/device.py` & `pyhomelink-0.1.9/pyhomelink/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,18 +210,18 @@
             url = self.rel.readings.co2readings
         elif readingtype == HomeLINKReadingType.HUMIDITY:
             url = self.rel.readings.humidityreadings
         elif readingtype == HomeLINKReadingType.TEMPERATURE:
             url = self.rel.readings.temperaturereadings
 
         if start or end:
-            url = url + "?"
+            url = f"{url}?"
         if start:
-            url = url + f"start={start}"
-        if start and end:
-            url = url + "&"
+            url = f"{url}start={start}"
+            if end:
+                url = f"{url}&"
         if end:
-            url = url + f"end={end}"
+            url = f"{url}end={end}"
         resp = await self._auth.request("get", url)
 
         check_status(resp)
         return DeviceReading(await resp.json())
```

### Comparing `pyhomelink-0.1.8/pyhomelink/insight.py` & `pyhomelink-0.1.9/pyhomelink/insight.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,19 @@
 
     @property
     def location(self) -> str:
         """Return the location of the Insight"""
         return self._raw_data.get("location", None)
 
     @property
+    def calculatedat(self) -> str:
+        """Return the datetime of the Insight calculation"""
+        return self._raw_data.get("calculatedAt", None)
+
+    @property
     def rel(self) -> any:
         """Return the tags of the Insight"""
         return self.Rel(self._raw_data["_rel"])
 
     class Rel:
         """Relative URLs for property."""
```

### Comparing `pyhomelink-0.1.8/pyhomelink/lookup.py` & `pyhomelink-0.1.9/pyhomelink/lookup.py`

 * *Files identical despite different names*

### Comparing `pyhomelink-0.1.8/pyhomelink/property.py` & `pyhomelink-0.1.9/pyhomelink/property.py`

 * *Files identical despite different names*

### Comparing `pyhomelink-0.1.8/pyhomelink/reading.py` & `pyhomelink-0.1.9/pyhomelink/reading.py`

 * *Files identical despite different names*

### Comparing `pyhomelink-0.1.8/pyhomelink.egg-info/PKG-INFO` & `pyhomelink-0.1.9/pyhomelink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhomelink
-Version: 0.1.8
+Version: 0.1.9
 Summary: Library for AICO HomeLINK
 Home-page: https://github.com/RogerSelwyn/python_homelink
 Author: Roger Selwyn
 Author-email: roger.selwyn@users.noreply.github.com
 Maintainer: RogerSelwyn
 Maintainer-email: roger.selwyn@users.noreply.github.com
 License: MIT
@@ -22,15 +22,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![CodeFactor](https://www.codefactor.io/repository/github/rogerselwyn/python_homelink/badge)](https://www.codefactor.io/repository/github/rogerselwyn/python_homelink)
 [![CodeQL](https://github.com/RogerSelwyn/python_homelink/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/RogerSelwyn/python_homelink/actions/workflows/github-code-scanning/codeql)
 [![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/pyhomelink)](https://libraries.io/pypi/pyhomelink)
 
-![GitHub release](https://img.shields.io/github/v/release/RogerSelwyn/python_homelink) [![maintained](https://img.shields.io/maintenance/yes/2023.svg)](#)
+![GitHub release](https://img.shields.io/github/v/release/RogerSelwyn/python_homelink) [![maintained](https://img.shields.io/maintenance/yes/2024.svg)](#)
 [![maintainer](https://img.shields.io/badge/maintainer-%20%40RogerSelwyn-blue.svg)](https://github.com/RogerSelwyn)
 ![PyPI - Status](https://img.shields.io/pypi/status/pyhomelink)
 [![PyPI](https://img.shields.io/pypi/v/pyhomelink)](https://pypi.org/project/pyhomelink/)
 [![GitHub](https://img.shields.io/github/license/rogerselwyn/python_homelink)](https://github.com/RogerSewlwyn/python_homelink/blob/main/LICENSE)
 
 
 # python_homelink
```

### Comparing `pyhomelink-0.1.8/setup.py` & `pyhomelink-0.1.9/setup.py`

 * *Files identical despite different names*

