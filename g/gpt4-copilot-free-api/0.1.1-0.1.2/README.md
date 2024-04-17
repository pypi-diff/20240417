# Comparing `tmp/gpt4_copilot_free_api-0.1.1.tar.gz` & `tmp/gpt4_copilot_free_api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt4_copilot_free_api-0.1.1.tar", last modified: Wed Apr 17 19:30:59 2024, max compression
+gzip compressed data, was "gpt4_copilot_free_api-0.1.2.tar", last modified: Wed Apr 17 19:35:24 2024, max compression
```

## Comparing `gpt4_copilot_free_api-0.1.1.tar` & `gpt4_copilot_free_api-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,12 @@
--rw-r--r--   0        0        0       24 2024-04-17 14:05:34.655247 gpt4_copilot_free_api-0.1.1/README.md
--rw-r--r--   0        0        0      522 2024-04-17 19:30:59.499020 gpt4_copilot_free_api-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-17 19:30:11.327289 gpt4_copilot_free_api-0.1.1/src/gpt4_copilot_free_api/__init__.py
--rw-r--r--   0        0        0     5203 2024-04-17 19:30:11.327289 gpt4_copilot_free_api-0.1.1/src/gpt4_copilot_free_api/api.py
--rw-r--r--   0        0        0     4272 2024-04-17 19:30:11.327289 gpt4_copilot_free_api-0.1.1/src/gpt4_copilot_free_api/free-gpt4.py
--rw-r--r--   0        0        0     5611 2024-04-17 19:30:11.327289 gpt4_copilot_free_api-0.1.1/src/gpt4_copilot_free_api/server.py
--rw-r--r--   0        0        0        0 2024-04-17 14:05:34.655247 gpt4_copilot_free_api-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0      314 1970-01-01 00:00:00.000000 gpt4_copilot_free_api-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       24 2024-04-17 14:05:34.655247 gpt4_copilot_free_api-0.1.2/README.md
+-rw-r--r--   0        0        0      522 2024-04-17 19:35:24.336291 gpt4_copilot_free_api-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-17 19:30:11.327289 gpt4_copilot_free_api-0.1.2/src/gpt4_copilot_free_api/__init__.py
+-rw-r--r--   0        0        0     5203 2024-04-17 19:30:11.327289 gpt4_copilot_free_api-0.1.2/src/gpt4_copilot_free_api/api.py
+-rw-r--r--   0        0        0      489 2024-04-17 19:34:26.594550 gpt4_copilot_free_api-0.1.2/src/gpt4_copilot_free_api/dist/index.html
+-rw-r--r--   0        0        0    17721 2024-04-17 19:34:26.604550 gpt4_copilot_free_api-0.1.2/src/gpt4_copilot_free_api/dist/static/index-G2uJJii4.css
+-rw-r--r--   0        0        0  1302707 2024-04-17 19:34:26.604550 gpt4_copilot_free_api-0.1.2/src/gpt4_copilot_free_api/dist/static/index-a3eJDKBc.js
+-rw-r--r--   0        0        0     1497 2024-04-17 19:34:26.604550 gpt4_copilot_free_api-0.1.2/src/gpt4_copilot_free_api/dist/vite.svg
+-rw-r--r--   0        0        0     4272 2024-04-17 19:30:11.327289 gpt4_copilot_free_api-0.1.2/src/gpt4_copilot_free_api/free-gpt4.py
+-rw-r--r--   0        0        0     5579 2024-04-17 19:34:41.815430 gpt4_copilot_free_api-0.1.2/src/gpt4_copilot_free_api/server.py
+-rw-r--r--   0        0        0        0 2024-04-17 14:05:34.655247 gpt4_copilot_free_api-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      314 1970-01-01 00:00:00.000000 gpt4_copilot_free_api-0.1.2/PKG-INFO
```

### Comparing `gpt4_copilot_free_api-0.1.1/pyproject.toml` & `gpt4_copilot_free_api-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gpt4-copilot-free-api"
-version = "0.1.1"
+version = "0.1.2"
 description = "Default template for PDM package"
 authors = [
     { name = "xDepcio", email = "olek.drwal@gmail.com" },
 ]
 dependencies = [
     "flask>=3.0.3",
     "requests>=2.31.0",
```

### Comparing `gpt4_copilot_free_api-0.1.1/src/gpt4_copilot_free_api/api.py` & `gpt4_copilot_free_api-0.1.2/src/gpt4_copilot_free_api/api.py`

 * *Files identical despite different names*

### Comparing `gpt4_copilot_free_api-0.1.1/src/gpt4_copilot_free_api/free-gpt4.py` & `gpt4_copilot_free_api-0.1.2/src/gpt4_copilot_free_api/free-gpt4.py`

 * *Files identical despite different names*

### Comparing `gpt4_copilot_free_api-0.1.1/src/gpt4_copilot_free_api/server.py` & `gpt4_copilot_free_api-0.1.2/src/gpt4_copilot_free_api/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import time
 from flask import Flask, render_template, request, send_from_directory
 import requests
 
 app = Flask(
     __name__,
-    static_folder="../../../frontend/dist/static",
-    template_folder="../../../frontend/dist",
+    static_folder="./dist/static",
+    template_folder="./dist",
 )
 
 MODEL = "gpt-4-1106-preview"
 token = None
 
 
 def get_token():
```

