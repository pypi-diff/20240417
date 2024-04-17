# Comparing `tmp/skipy-0.1.2.tar.gz` & `tmp/skipy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skipy-0.1.2.tar", max compression
+gzip compressed data, was "skipy-0.1.3.tar", max compression
```

## Comparing `skipy-0.1.2.tar` & `skipy-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      119 2024-01-29 07:59:49.313144 skipy-0.1.2/README.md
--rw-r--r--   0        0        0     1152 2024-01-29 07:59:49.313144 skipy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       64 2024-01-29 07:59:49.313144 skipy-0.1.2/skipy/AWS/__init__.py
--rw-r--r--   0        0        0      599 2024-01-29 07:59:49.313144 skipy-0.1.2/skipy/AWS/utils.py
--rw-r--r--   0        0        0       56 2024-01-29 07:59:49.313144 skipy-0.1.2/skipy/Chatwork/__init__.py
--rw-r--r--   0        0        0     5722 2024-01-29 07:59:49.313144 skipy-0.1.2/skipy/Chatwork/__wrapper.py
--rw-r--r--   0        0        0      108 2024-01-29 07:59:49.313144 skipy-0.1.2/skipy/GCP/__init__.py
--rw-r--r--   0        0        0     5944 2024-01-29 07:59:49.313144 skipy-0.1.2/skipy/GCP/drive.py
--rw-r--r--   0        0        0     3633 2024-01-29 07:59:49.313144 skipy-0.1.2/skipy/GCP/sheet.py
--rw-r--r--   0        0        0       64 2024-01-29 07:59:49.313144 skipy-0.1.2/skipy/Selenium/__init__.py
--rw-r--r--   0        0        0      857 2024-01-29 07:59:49.313144 skipy-0.1.2/skipy/Selenium/__wrapper.py
--rw-r--r--   0        0        0       50 2024-01-29 07:59:49.313144 skipy-0.1.2/skipy/Slack/__init__.py
--rw-r--r--   0        0        0      483 2024-01-29 07:59:49.313144 skipy-0.1.2/skipy/Slack/__wrapper.py
--rw-r--r--   0        0        0       50 2024-01-29 07:59:49.313144 skipy-0.1.2/skipy/__init__.py
--rw-r--r--   0        0        0      872 1970-01-01 00:00:00.000000 skipy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      119 2024-04-17 04:56:02.098215 skipy-0.1.3/README.md
+-rw-r--r--   0        0        0     1152 2024-04-17 04:56:02.098215 skipy-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       64 2024-04-17 04:56:02.098215 skipy-0.1.3/skipy/AWS/__init__.py
+-rw-r--r--   0        0        0      599 2024-04-17 04:56:02.098215 skipy-0.1.3/skipy/AWS/utils.py
+-rw-r--r--   0        0        0       56 2024-04-17 04:56:02.098215 skipy-0.1.3/skipy/Chatwork/__init__.py
+-rw-r--r--   0        0        0     5722 2024-04-17 04:56:02.098215 skipy-0.1.3/skipy/Chatwork/__wrapper.py
+-rw-r--r--   0        0        0      108 2024-04-17 04:56:02.098215 skipy-0.1.3/skipy/GCP/__init__.py
+-rw-r--r--   0        0        0     5944 2024-04-17 04:56:02.098215 skipy-0.1.3/skipy/GCP/drive.py
+-rw-r--r--   0        0        0     3633 2024-04-17 04:56:02.098215 skipy-0.1.3/skipy/GCP/sheet.py
+-rw-r--r--   0        0        0       64 2024-04-17 04:56:02.098215 skipy-0.1.3/skipy/Selenium/__init__.py
+-rw-r--r--   0        0        0      898 2024-04-17 04:56:02.098215 skipy-0.1.3/skipy/Selenium/__wrapper.py
+-rw-r--r--   0        0        0       50 2024-04-17 04:56:02.098215 skipy-0.1.3/skipy/Slack/__init__.py
+-rw-r--r--   0        0        0      483 2024-04-17 04:56:02.098215 skipy-0.1.3/skipy/Slack/__wrapper.py
+-rw-r--r--   0        0        0       50 2024-04-17 04:56:02.098215 skipy-0.1.3/skipy/__init__.py
+-rw-r--r--   0        0        0      872 1970-01-01 00:00:00.000000 skipy-0.1.3/PKG-INFO
```

### Comparing `skipy-0.1.2/pyproject.toml` & `skipy-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skipy-0.1.2/skipy/AWS/utils.py` & `skipy-0.1.3/skipy/AWS/utils.py`

 * *Files identical despite different names*

### Comparing `skipy-0.1.2/skipy/Chatwork/__wrapper.py` & `skipy-0.1.3/skipy/Chatwork/__wrapper.py`

 * *Files identical despite different names*

### Comparing `skipy-0.1.2/skipy/GCP/drive.py` & `skipy-0.1.3/skipy/GCP/drive.py`

 * *Files identical despite different names*

### Comparing `skipy-0.1.2/skipy/GCP/sheet.py` & `skipy-0.1.3/skipy/GCP/sheet.py`

 * *Files identical despite different names*

### Comparing `skipy-0.1.2/skipy/Selenium/__wrapper.py` & `skipy-0.1.3/skipy/Selenium/__wrapper.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 
 from selenium import webdriver
 
 
-def setup_driver(is_lambda=False):
+def setup_driver(is_lambda=True, is_headless=True):
     options = webdriver.ChromeOptions()
-    options.add_argument("--headless")
+    if is_headless:
+        options.add_argument("--headless")
     options.add_argument("--no-sandbox")
     options.add_argument("--disable-gpu")
     options.add_argument("--window-size=1920x1080")
     options.add_argument("--single-process")
     options.add_argument("--disable-dev-shm-usage")
     options.add_argument("--disable-dev-tools")
     options.add_argument("--no-zygote")
```

### Comparing `skipy-0.1.2/PKG-INFO` & `skipy-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skipy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Skip-tac python modules
 License: MIT
 Author: syamaguc
 Author-email: programmer2844@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

