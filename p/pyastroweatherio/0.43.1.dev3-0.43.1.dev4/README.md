# Comparing `tmp/pyastroweatherio-0.43.1.dev3.tar.gz` & `tmp/pyastroweatherio-0.43.1.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyastroweatherio-0.43.1.dev3.tar", last modified: Sun Apr 14 12:31:44 2024, max compression
+gzip compressed data, was "pyastroweatherio-0.43.1.dev4.tar", last modified: Wed Apr 17 12:35:14 2024, max compression
```

## Comparing `pyastroweatherio-0.43.1.dev3.tar` & `pyastroweatherio-0.43.1.dev4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-14 12:31:44.365509 pyastroweatherio-0.43.1.dev3/
--rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.43.1.dev3/LICENSE
--rw-r--r--   0 markus    (1000) markus    (1000)     1042 2024-04-14 12:31:44.365509 pyastroweatherio-0.43.1.dev3/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)     1576 2023-10-06 18:49:53.000000 pyastroweatherio-0.43.1.dev3/README.md
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-14 12:31:44.361509 pyastroweatherio-0.43.1.dev3/pyastroweatherio/
--rw-rw-r--   0 markus    (1000) markus    (1000)      285 2023-04-10 18:40:11.000000 pyastroweatherio-0.43.1.dev3/pyastroweatherio/__init__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    32176 2024-04-14 12:31:08.000000 pyastroweatherio-0.43.1.dev3/pyastroweatherio/client.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     3638 2024-04-14 12:30:04.000000 pyastroweatherio-0.43.1.dev3/pyastroweatherio/const.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    20074 2024-04-14 12:24:57.000000 pyastroweatherio-0.43.1.dev3/pyastroweatherio/dataclasses.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      337 2023-11-05 13:15:24.000000 pyastroweatherio-0.43.1.dev3/pyastroweatherio/errors.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    32312 2023-11-12 10:53:43.000000 pyastroweatherio-0.43.1.dev3/pyastroweatherio/helper_functions.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-14 12:31:44.365509 pyastroweatherio-0.43.1.dev3/pyastroweatherio.egg-info/
--rw-r--r--   0 markus    (1000) markus    (1000)     1042 2024-04-14 12:31:44.000000 pyastroweatherio-0.43.1.dev3/pyastroweatherio.egg-info/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)      413 2024-04-14 12:31:44.000000 pyastroweatherio-0.43.1.dev3/pyastroweatherio.egg-info/SOURCES.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-04-14 12:31:44.000000 pyastroweatherio-0.43.1.dev3/pyastroweatherio.egg-info/dependency_links.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       16 2024-04-14 12:31:44.000000 pyastroweatherio-0.43.1.dev3/pyastroweatherio.egg-info/requires.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       17 2024-04-14 12:31:44.000000 pyastroweatherio-0.43.1.dev3/pyastroweatherio.egg-info/top_level.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       79 2024-04-14 12:31:44.365509 pyastroweatherio-0.43.1.dev3/setup.cfg
--rw-rw-r--   0 markus    (1000) markus    (1000)     1340 2024-04-14 12:31:40.000000 pyastroweatherio-0.43.1.dev3/setup.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-17 12:35:14.156187 pyastroweatherio-0.43.1.dev4/
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.43.1.dev4/LICENSE
+-rw-r--r--   0 markus    (1000) markus    (1000)     1042 2024-04-17 12:35:14.156187 pyastroweatherio-0.43.1.dev4/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1576 2023-10-06 18:49:53.000000 pyastroweatherio-0.43.1.dev4/README.md
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-17 12:35:14.156187 pyastroweatherio-0.43.1.dev4/pyastroweatherio/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      285 2023-04-10 18:40:11.000000 pyastroweatherio-0.43.1.dev4/pyastroweatherio/__init__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    32193 2024-04-17 12:34:37.000000 pyastroweatherio-0.43.1.dev4/pyastroweatherio/client.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     3638 2024-04-14 12:30:04.000000 pyastroweatherio-0.43.1.dev4/pyastroweatherio/const.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    20074 2024-04-14 12:24:57.000000 pyastroweatherio-0.43.1.dev4/pyastroweatherio/dataclasses.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      337 2023-11-05 13:15:24.000000 pyastroweatherio-0.43.1.dev4/pyastroweatherio/errors.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    32312 2023-11-12 10:53:43.000000 pyastroweatherio-0.43.1.dev4/pyastroweatherio/helper_functions.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-17 12:35:14.156187 pyastroweatherio-0.43.1.dev4/pyastroweatherio.egg-info/
+-rw-r--r--   0 markus    (1000) markus    (1000)     1042 2024-04-17 12:35:14.000000 pyastroweatherio-0.43.1.dev4/pyastroweatherio.egg-info/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)      413 2024-04-17 12:35:14.000000 pyastroweatherio-0.43.1.dev4/pyastroweatherio.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-04-17 12:35:14.000000 pyastroweatherio-0.43.1.dev4/pyastroweatherio.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       16 2024-04-17 12:35:14.000000 pyastroweatherio-0.43.1.dev4/pyastroweatherio.egg-info/requires.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       17 2024-04-17 12:35:14.000000 pyastroweatherio-0.43.1.dev4/pyastroweatherio.egg-info/top_level.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       79 2024-04-17 12:35:14.156187 pyastroweatherio-0.43.1.dev4/setup.cfg
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1340 2024-04-17 12:35:06.000000 pyastroweatherio-0.43.1.dev4/setup.py
```

### Comparing `pyastroweatherio-0.43.1.dev3/LICENSE` & `pyastroweatherio-0.43.1.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.43.1.dev3/PKG-INFO` & `pyastroweatherio-0.43.1.dev4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.43.1.dev3
+Version: 0.43.1.dev4
 Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Met.no,Python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyastroweatherio-0.43.1.dev3/README.md` & `pyastroweatherio-0.43.1.dev4/README.md`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.43.1.dev3/pyastroweatherio/client.py` & `pyastroweatherio-0.43.1.dev4/pyastroweatherio/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,15 +432,15 @@
         for idx, row in enumerate(self._forecast_data):
             if row.forecast_time.hour % 24 == sun_next_rising.hour and len(start_indexes) == 0:
                 start_indexes.append(0)
             if row.forecast_time.hour % 24 == sun_next_setting.hour:
                 start_indexes.append(idx)
 
         forecast_data_len = len(self._forecast_data)
-        for day in range(0, 2):
+        for day in range(0, len(start_indexes)):
             start_forecast_hour = 0
             start_weather = ""
             interval_points = []
             start_index = start_indexes[day]
             for idx in range(
                 start_index,
                 start_index + int(math.floor(night_duration_astronomical / 3600) + 2),
```

### Comparing `pyastroweatherio-0.43.1.dev3/pyastroweatherio/const.py` & `pyastroweatherio-0.43.1.dev4/pyastroweatherio/const.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.43.1.dev3/pyastroweatherio/dataclasses.py` & `pyastroweatherio-0.43.1.dev4/pyastroweatherio/dataclasses.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.43.1.dev3/pyastroweatherio/helper_functions.py` & `pyastroweatherio-0.43.1.dev4/pyastroweatherio/helper_functions.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.43.1.dev3/pyastroweatherio.egg-info/PKG-INFO` & `pyastroweatherio-0.43.1.dev4/pyastroweatherio.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.43.1.dev3
+Version: 0.43.1.dev4
 Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Met.no,Python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyastroweatherio-0.43.1.dev3/setup.py` & `pyastroweatherio-0.43.1.dev4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name="pyastroweatherio",
     packages=["pyastroweatherio"],
-    version="0.43.1.dev3",
+    version="0.43.1.dev4",
     license="MIT",
     description="Python Wrapper for 7Timer and Met.no REST API",
     long_description=" ".join(
         [
             "Lightweight Python 3 module to receive data via",
             "REST API from 7Timer and Met.no.",
         ],
```

