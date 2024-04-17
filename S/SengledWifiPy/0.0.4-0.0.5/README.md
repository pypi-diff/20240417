# Comparing `tmp/sengledwifipy-0.0.4.tar.gz` & `tmp/sengledwifipy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sengledwifipy-0.0.4.tar", max compression
+gzip compressed data, was "sengledwifipy-0.0.5.tar", max compression
```

## Comparing `sengledwifipy-0.0.4.tar` & `sengledwifipy-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2024-04-17 17:19:31.613185 sengledwifipy-0.0.4/LICENSE
--rw-r--r--   0        0        0     2434 2024-04-17 17:19:31.613185 sengledwifipy-0.0.4/README.md
--rw-r--r--   0        0        0     3052 2024-04-17 17:19:49.517426 sengledwifipy-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1448 2024-04-17 17:19:31.617185 sengledwifipy-0.0.4/sengledwifipy/__init__.py
--rw-r--r--   0        0        0      716 2024-04-17 17:19:31.617185 sengledwifipy-0.0.4/sengledwifipy/const.py
--rw-r--r--   0        0        0      773 2024-04-17 17:19:31.617185 sengledwifipy-0.0.4/sengledwifipy/errors.py
--rw-r--r--   0        0        0     6973 2024-04-17 17:19:31.617185 sengledwifipy-0.0.4/sengledwifipy/helpers.py
--rw-r--r--   0        0        0     6954 2024-04-17 17:19:31.617185 sengledwifipy-0.0.4/sengledwifipy/sengledwifiapi.py
--rw-r--r--   0        0        0    11984 2024-04-17 17:19:31.617185 sengledwifipy-0.0.4/sengledwifipy/sengledwifilogin.py
--rw-r--r--   0        0        0    11983 2024-04-17 17:19:31.617185 sengledwifipy-0.0.4/sengledwifipy/sengledwifimqtt.py
--rw-r--r--   0        0        0     3330 1970-01-01 00:00:00.000000 sengledwifipy-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-17 17:26:56.647762 sengledwifipy-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2434 2024-04-17 17:26:56.647762 sengledwifipy-0.0.5/README.md
+-rw-r--r--   0        0        0     3052 2024-04-17 17:27:11.051976 sengledwifipy-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1448 2024-04-17 17:26:56.647762 sengledwifipy-0.0.5/sengledwifipy/__init__.py
+-rw-r--r--   0        0        0      716 2024-04-17 17:26:56.647762 sengledwifipy-0.0.5/sengledwifipy/const.py
+-rw-r--r--   0        0        0      773 2024-04-17 17:26:56.647762 sengledwifipy-0.0.5/sengledwifipy/errors.py
+-rw-r--r--   0        0        0     6973 2024-04-17 17:26:56.647762 sengledwifipy-0.0.5/sengledwifipy/helpers.py
+-rw-r--r--   0        0        0     6954 2024-04-17 17:26:56.647762 sengledwifipy-0.0.5/sengledwifipy/sengledwifiapi.py
+-rw-r--r--   0        0        0    11984 2024-04-17 17:26:56.647762 sengledwifipy-0.0.5/sengledwifipy/sengledwifilogin.py
+-rw-r--r--   0        0        0    11983 2024-04-17 17:26:56.647762 sengledwifipy-0.0.5/sengledwifipy/sengledwifimqtt.py
+-rw-r--r--   0        0        0     3330 1970-01-01 00:00:00.000000 sengledwifipy-0.0.5/PKG-INFO
```

### Comparing `sengledwifipy-0.0.4/LICENSE` & `sengledwifipy-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sengledwifipy-0.0.4/README.md` & `sengledwifipy-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sengledwifipy-0.0.4/pyproject.toml` & `sengledwifipy-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  SPDX-License-Identifier: Apache-2.0
 
 [tool.poetry]
 name = "SengledWifiPy"
-version = "0.0.4"
+version = "0.0.5"
 description = "Python API to control Sengled Wifi Devices Programmatically."
 authors = [
   "Cesar <gv4plolxe@mozmail.com>"
 ]
 license = "Apache-2.0"
 readme = 'README.md'
 repository = "https://github.com/cpadil/sengledwifipy"
```

### Comparing `sengledwifipy-0.0.4/sengledwifipy/__init__.py` & `sengledwifipy-0.0.5/sengledwifipy/__init__.py`

 * *Files identical despite different names*

### Comparing `sengledwifipy-0.0.4/sengledwifipy/const.py` & `sengledwifipy-0.0.5/sengledwifipy/const.py`

 * *Files identical despite different names*

### Comparing `sengledwifipy-0.0.4/sengledwifipy/errors.py` & `sengledwifipy-0.0.5/sengledwifipy/errors.py`

 * *Files identical despite different names*

### Comparing `sengledwifipy-0.0.4/sengledwifipy/helpers.py` & `sengledwifipy-0.0.5/sengledwifipy/helpers.py`

 * *Files identical despite different names*

### Comparing `sengledwifipy-0.0.4/sengledwifipy/sengledwifiapi.py` & `sengledwifipy-0.0.5/sengledwifipy/sengledwifiapi.py`

 * *Files identical despite different names*

### Comparing `sengledwifipy-0.0.4/sengledwifipy/sengledwifilogin.py` & `sengledwifipy-0.0.5/sengledwifipy/sengledwifilogin.py`

 * *Files identical despite different names*

### Comparing `sengledwifipy-0.0.4/sengledwifipy/sengledwifimqtt.py` & `sengledwifipy-0.0.5/sengledwifipy/sengledwifimqtt.py`

 * *Files identical despite different names*

### Comparing `sengledwifipy-0.0.4/PKG-INFO` & `sengledwifipy-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SengledWifiPy
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python API to control Sengled Wifi Devices Programmatically.
 Home-page: https://github.com/cpadil/sengledwifipy
 License: Apache-2.0
 Keywords: Sengled,Wifi,homeassistant
 Author: Cesar
 Author-email: gv4plolxe@mozmail.com
 Requires-Python: >=3.11,<4
```

