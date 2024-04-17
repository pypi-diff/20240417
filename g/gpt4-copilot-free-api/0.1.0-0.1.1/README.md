# Comparing `tmp/gpt4_copilot_free_api-0.1.0.tar.gz` & `tmp/gpt4_copilot_free_api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt4_copilot_free_api-0.1.0.tar", last modified: Wed Apr 17 19:22:34 2024, max compression
+gzip compressed data, was "gpt4_copilot_free_api-0.1.1.tar", last modified: Wed Apr 17 19:30:59 2024, max compression
```

## Comparing `gpt4_copilot_free_api-0.1.0.tar` & `gpt4_copilot_free_api-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,8 @@
-drwxr-xr-x   0 olek      (1000) olek      (1000)        0 2024-04-17 19:22:34.234396 gpt4_copilot_free_api-0.1.0/
--rw-r--r--   0 olek      (1000) olek      (1000)       93 2024-04-17 19:18:23.000000 gpt4_copilot_free_api-0.1.0/MANIFEST.in
--rw-r--r--   0 olek      (1000) olek      (1000)      386 2024-04-17 19:22:34.234396 gpt4_copilot_free_api-0.1.0/PKG-INFO
--rw-r--r--   0 olek      (1000) olek      (1000)       24 2024-04-17 14:05:34.000000 gpt4_copilot_free_api-0.1.0/README.md
-drwxr-xr-x   0 olek      (1000) olek      (1000)        0 2024-04-17 19:22:34.234396 gpt4_copilot_free_api-0.1.0/gpt4_copilot_free_api/
--rw-r--r--   0 olek      (1000) olek      (1000)        0 2024-04-17 14:05:34.000000 gpt4_copilot_free_api-0.1.0/gpt4_copilot_free_api/__init__.py
--rw-r--r--   0 olek      (1000) olek      (1000)     5203 2024-04-17 11:27:52.000000 gpt4_copilot_free_api-0.1.0/gpt4_copilot_free_api/api.py
--rw-r--r--   0 olek      (1000) olek      (1000)     4272 2024-04-17 11:39:08.000000 gpt4_copilot_free_api-0.1.0/gpt4_copilot_free_api/free-gpt4.py
--rw-r--r--   0 olek      (1000) olek      (1000)     5611 2024-04-17 17:15:23.000000 gpt4_copilot_free_api-0.1.0/gpt4_copilot_free_api/server.py
-drwxr-xr-x   0 olek      (1000) olek      (1000)        0 2024-04-17 19:22:34.234396 gpt4_copilot_free_api-0.1.0/gpt4_copilot_free_api.egg-info/
--rw-r--r--   0 olek      (1000) olek      (1000)      386 2024-04-17 19:22:34.000000 gpt4_copilot_free_api-0.1.0/gpt4_copilot_free_api.egg-info/PKG-INFO
--rw-r--r--   0 olek      (1000) olek      (1000)      417 2024-04-17 19:22:34.000000 gpt4_copilot_free_api-0.1.0/gpt4_copilot_free_api.egg-info/SOURCES.txt
--rw-r--r--   0 olek      (1000) olek      (1000)        1 2024-04-17 19:22:34.000000 gpt4_copilot_free_api-0.1.0/gpt4_copilot_free_api.egg-info/dependency_links.txt
--rw-r--r--   0 olek      (1000) olek      (1000)       30 2024-04-17 19:22:34.000000 gpt4_copilot_free_api-0.1.0/gpt4_copilot_free_api.egg-info/requires.txt
--rw-r--r--   0 olek      (1000) olek      (1000)       28 2024-04-17 19:22:34.000000 gpt4_copilot_free_api-0.1.0/gpt4_copilot_free_api.egg-info/top_level.txt
--rw-r--r--   0 olek      (1000) olek      (1000)      542 2024-04-17 19:07:57.000000 gpt4_copilot_free_api-0.1.0/pyproject.toml
--rw-r--r--   0 olek      (1000) olek      (1000)       38 2024-04-17 19:22:34.234396 gpt4_copilot_free_api-0.1.0/setup.cfg
--rw-r--r--   0 olek      (1000) olek      (1000)      926 2024-04-17 19:20:45.000000 gpt4_copilot_free_api-0.1.0/setup.py
-drwxr-xr-x   0 olek      (1000) olek      (1000)        0 2024-04-17 19:22:34.234396 gpt4_copilot_free_api-0.1.0/tests/
--rw-r--r--   0 olek      (1000) olek      (1000)        0 2024-04-17 14:05:34.000000 gpt4_copilot_free_api-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-17 14:05:34.655247 gpt4_copilot_free_api-0.1.1/README.md
+-rw-r--r--   0        0        0      522 2024-04-17 19:30:59.499020 gpt4_copilot_free_api-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-17 19:30:11.327289 gpt4_copilot_free_api-0.1.1/src/gpt4_copilot_free_api/__init__.py
+-rw-r--r--   0        0        0     5203 2024-04-17 19:30:11.327289 gpt4_copilot_free_api-0.1.1/src/gpt4_copilot_free_api/api.py
+-rw-r--r--   0        0        0     4272 2024-04-17 19:30:11.327289 gpt4_copilot_free_api-0.1.1/src/gpt4_copilot_free_api/free-gpt4.py
+-rw-r--r--   0        0        0     5611 2024-04-17 19:30:11.327289 gpt4_copilot_free_api-0.1.1/src/gpt4_copilot_free_api/server.py
+-rw-r--r--   0        0        0        0 2024-04-17 14:05:34.655247 gpt4_copilot_free_api-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      314 1970-01-01 00:00:00.000000 gpt4_copilot_free_api-0.1.1/PKG-INFO
```

### Comparing `gpt4_copilot_free_api-0.1.0/gpt4_copilot_free_api/api.py` & `gpt4_copilot_free_api-0.1.1/src/gpt4_copilot_free_api/api.py`

 * *Files identical despite different names*

### Comparing `gpt4_copilot_free_api-0.1.0/gpt4_copilot_free_api/free-gpt4.py` & `gpt4_copilot_free_api-0.1.1/src/gpt4_copilot_free_api/free-gpt4.py`

 * *Files identical despite different names*

### Comparing `gpt4_copilot_free_api-0.1.0/gpt4_copilot_free_api/server.py` & `gpt4_copilot_free_api-0.1.1/src/gpt4_copilot_free_api/server.py`

 * *Files identical despite different names*

