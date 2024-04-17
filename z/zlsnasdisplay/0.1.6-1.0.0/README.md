# Comparing `tmp/zlsnasdisplay-0.1.6.tar.gz` & `tmp/zlsnasdisplay-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zlsnasdisplay-0.1.6.tar", max compression
+gzip compressed data, was "zlsnasdisplay-1.0.0.tar", max compression
```

## Comparing `zlsnasdisplay-0.1.6.tar` & `zlsnasdisplay-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1071 2024-03-21 19:22:27.664880 zlsnasdisplay-0.1.6/LICENSE
--rw-r--r--   0        0        0     4775 2024-03-21 19:22:27.664880 zlsnasdisplay-0.1.6/README.md
--rw-r--r--   0        0        0     1365 2024-03-21 19:22:27.664880 zlsnasdisplay-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       66 2024-03-21 19:22:27.664880 zlsnasdisplay-0.1.6/zlsnasdisplay/__init__.py
--rwxr-xr-x   0        0        0      100 2024-03-21 19:22:27.664880 zlsnasdisplay-0.1.6/zlsnasdisplay/__main__.py
--rw-r--r--   0        0        0       18 2024-03-21 19:22:27.664880 zlsnasdisplay-0.1.6/zlsnasdisplay/_version.py
--rw-r--r--   0        0        0      561 2024-03-21 19:22:27.664880 zlsnasdisplay-0.1.6/zlsnasdisplay/display_controller.py
--rw-r--r--   0        0        0     9187 2024-03-21 19:22:27.664880 zlsnasdisplay-0.1.6/zlsnasdisplay/display_renderer.py
--rw-r--r--   0        0        0 11604276 2024-03-21 19:22:27.732876 zlsnasdisplay-0.1.6/zlsnasdisplay/fonts/MaterialSymbolsRounded.ttf
--rw-r--r--   0        0        0   362552 2024-03-21 19:22:27.732876 zlsnasdisplay-0.1.6/zlsnasdisplay/fonts/Ubuntu-Light.ttf
--rw-r--r--   0        0        0   299684 2024-03-21 19:22:27.736876 zlsnasdisplay-0.1.6/zlsnasdisplay/fonts/Ubuntu-Regular.ttf
--rwxr-xr-x   0        0        0     2602 2024-03-21 19:22:27.736876 zlsnasdisplay-0.1.6/zlsnasdisplay/main.py
--rw-r--r--   0        0        0     2972 2024-03-21 19:22:27.736876 zlsnasdisplay-0.1.6/zlsnasdisplay/network_operations.py
--rw-r--r--   0        0        0        0 2024-03-21 19:22:27.736876 zlsnasdisplay-0.1.6/zlsnasdisplay/py.typed
--rw-r--r--   0        0        0     2330 2024-03-21 19:22:27.736876 zlsnasdisplay-0.1.6/zlsnasdisplay/system_operations.py
--rw-r--r--   0        0        0        0 2024-03-21 19:22:27.736876 zlsnasdisplay-0.1.6/zlsnasdisplay/waveshare_epd/__init__.py
--rw-r--r--   0        0        0    23799 2024-03-21 19:22:27.736876 zlsnasdisplay-0.1.6/zlsnasdisplay/waveshare_epd/epd2in9_V2.py
--rw-r--r--   0        0        0     8468 2024-03-21 19:22:27.736876 zlsnasdisplay-0.1.6/zlsnasdisplay/waveshare_epd/epdconfig.py
--rw-r--r--   0        0        0     5508 1970-01-01 00:00:00.000000 zlsnasdisplay-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-17 21:13:00.183050 zlsnasdisplay-1.0.0/LICENSE
+-rw-r--r--   0        0        0     4775 2024-04-17 21:13:00.183050 zlsnasdisplay-1.0.0/README.md
+-rw-r--r--   0        0        0     1365 2024-04-17 21:13:00.183050 zlsnasdisplay-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       66 2024-04-17 21:13:00.183050 zlsnasdisplay-1.0.0/zlsnasdisplay/__init__.py
+-rwxr-xr-x   0        0        0      100 2024-04-17 21:13:00.187050 zlsnasdisplay-1.0.0/zlsnasdisplay/__main__.py
+-rw-r--r--   0        0        0       18 2024-04-17 21:13:00.187050 zlsnasdisplay-1.0.0/zlsnasdisplay/_version.py
+-rw-r--r--   0        0        0      561 2024-04-17 21:13:00.187050 zlsnasdisplay-1.0.0/zlsnasdisplay/display_controller.py
+-rw-r--r--   0        0        0     9187 2024-04-17 21:13:00.187050 zlsnasdisplay-1.0.0/zlsnasdisplay/display_renderer.py
+-rw-r--r--   0        0        0 11604276 2024-04-17 21:13:00.251050 zlsnasdisplay-1.0.0/zlsnasdisplay/fonts/MaterialSymbolsRounded.ttf
+-rw-r--r--   0        0        0   362552 2024-04-17 21:13:00.255050 zlsnasdisplay-1.0.0/zlsnasdisplay/fonts/Ubuntu-Light.ttf
+-rw-r--r--   0        0        0   299684 2024-04-17 21:13:00.255050 zlsnasdisplay-1.0.0/zlsnasdisplay/fonts/Ubuntu-Regular.ttf
+-rwxr-xr-x   0        0        0     2602 2024-04-17 21:13:00.255050 zlsnasdisplay-1.0.0/zlsnasdisplay/main.py
+-rw-r--r--   0        0        0     3047 2024-04-17 21:13:00.255050 zlsnasdisplay-1.0.0/zlsnasdisplay/network_operations.py
+-rw-r--r--   0        0        0        0 2024-04-17 21:13:00.255050 zlsnasdisplay-1.0.0/zlsnasdisplay/py.typed
+-rw-r--r--   0        0        0     2330 2024-04-17 21:13:00.255050 zlsnasdisplay-1.0.0/zlsnasdisplay/system_operations.py
+-rw-r--r--   0        0        0        0 2024-04-17 21:13:00.255050 zlsnasdisplay-1.0.0/zlsnasdisplay/waveshare_epd/__init__.py
+-rw-r--r--   0        0        0    23799 2024-04-17 21:13:00.255050 zlsnasdisplay-1.0.0/zlsnasdisplay/waveshare_epd/epd2in9_V2.py
+-rw-r--r--   0        0        0     8468 2024-04-17 21:13:00.255050 zlsnasdisplay-1.0.0/zlsnasdisplay/waveshare_epd/epdconfig.py
+-rw-r--r--   0        0        0     5508 1970-01-01 00:00:00.000000 zlsnasdisplay-1.0.0/PKG-INFO
```

### Comparing `zlsnasdisplay-0.1.6/LICENSE` & `zlsnasdisplay-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zlsnasdisplay-0.1.6/README.md` & `zlsnasdisplay-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `zlsnasdisplay-0.1.6/pyproject.toml` & `zlsnasdisplay-1.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zlsnasdisplay"
-version = "0.1.6"
+version = "1.0.0"
 description = "Eink display manager"
 authors = ["Ondrej Zalesky <o.zalesky@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -12,18 +12,18 @@
 gpiozero = "^2.0.1"
 schedule = "^1.2.1"
 psutil = "^5.9.8"
 requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "1.9.0"
-pre-commit = "3.6.2"
+pre-commit = "3.7.0"
 pytest = "8.1.1"
-pytest-cov = "4.1.0"
-ruff = "0.3.3"
+pytest-cov = "5.0.0"
+ruff = "0.3.7"
 tomli = {version = "2.0.1", python = "<3.9"}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
```

### Comparing `zlsnasdisplay-0.1.6/zlsnasdisplay/display_controller.py` & `zlsnasdisplay-1.0.0/zlsnasdisplay/display_controller.py`

 * *Files identical despite different names*

### Comparing `zlsnasdisplay-0.1.6/zlsnasdisplay/display_renderer.py` & `zlsnasdisplay-1.0.0/zlsnasdisplay/display_renderer.py`

 * *Files identical despite different names*

### Comparing `zlsnasdisplay-0.1.6/zlsnasdisplay/fonts/MaterialSymbolsRounded.ttf` & `zlsnasdisplay-1.0.0/zlsnasdisplay/fonts/MaterialSymbolsRounded.ttf`

 * *Files identical despite different names*

### Comparing `zlsnasdisplay-0.1.6/zlsnasdisplay/fonts/Ubuntu-Light.ttf` & `zlsnasdisplay-1.0.0/zlsnasdisplay/fonts/Ubuntu-Light.ttf`

 * *Files identical despite different names*

### Comparing `zlsnasdisplay-0.1.6/zlsnasdisplay/fonts/Ubuntu-Regular.ttf` & `zlsnasdisplay-1.0.0/zlsnasdisplay/fonts/Ubuntu-Regular.ttf`

 * *Files identical despite different names*

### Comparing `zlsnasdisplay-0.1.6/zlsnasdisplay/main.py` & `zlsnasdisplay-1.0.0/zlsnasdisplay/main.py`

 * *Files identical despite different names*

### Comparing `zlsnasdisplay-0.1.6/zlsnasdisplay/network_operations.py` & `zlsnasdisplay-1.0.0/zlsnasdisplay/network_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #! /usr/bin/env python3
 import logging
+import socket
 import subprocess
 import time
 
 import psutil
 import requests as requests
 
 
@@ -46,15 +47,17 @@
         except subprocess.CalledProcessError as e:
             logging.debug(f"Error running iwconfig: {e.output}")
             return None
 
     @staticmethod
     def get_ip_address():
         """Get the IP address of the wireless network."""
-        return psutil.net_if_addrs()["wlan0"][0].address
+        hostname = socket.gethostname()
+        ip_address = socket.gethostbyname(hostname)
+        return ip_address
 
 
 class TrafficMonitor:
     def get_current_traffic(self):
         """Get the current network traffic."""
 
         interval = 1
```

### Comparing `zlsnasdisplay-0.1.6/zlsnasdisplay/system_operations.py` & `zlsnasdisplay-1.0.0/zlsnasdisplay/system_operations.py`

 * *Files identical despite different names*

### Comparing `zlsnasdisplay-0.1.6/zlsnasdisplay/waveshare_epd/epd2in9_V2.py` & `zlsnasdisplay-1.0.0/zlsnasdisplay/waveshare_epd/epd2in9_V2.py`

 * *Files identical despite different names*

### Comparing `zlsnasdisplay-0.1.6/zlsnasdisplay/waveshare_epd/epdconfig.py` & `zlsnasdisplay-1.0.0/zlsnasdisplay/waveshare_epd/epdconfig.py`

 * *Files identical despite different names*

### Comparing `zlsnasdisplay-0.1.6/PKG-INFO` & `zlsnasdisplay-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zlsnasdisplay
-Version: 0.1.6
+Version: 1.0.0
 Summary: Eink display manager
 License: MIT
 Author: Ondrej Zalesky
 Author-email: o.zalesky@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

