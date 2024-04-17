# Comparing `tmp/tej_tool_api-1.1.2.tar.gz` & `tmp/tej_tool_api-1.1.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tej_tool_api-1.1.2.tar", last modified: Wed Apr 17 02:17:15 2024, max compression
+gzip compressed data, was "tej_tool_api-1.1.2rc0.tar", last modified: Tue Apr 16 09:41:55 2024, max compression
```

## Comparing `tej_tool_api-1.1.2.tar` & `tej_tool_api-1.1.2rc0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:15.607099 tej_tool_api-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-04-17 02:17:10.000000 tej_tool_api-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-17 02:17:10.000000 tej_tool_api-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-04-17 02:17:15.607099 tej_tool_api-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-17 02:17:10.000000 tej_tool_api-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:15.607099 tej_tool_api-1.1.2/TejToolAPI/
--rw-r--r--   0 runner    (1001) docker     (127)    29372 2024-04-17 02:17:10.000000 tej_tool_api-1.1.2/TejToolAPI/Map_Dask_API.py
--rw-r--r--   0 runner    (1001) docker     (127)    13543 2024-04-17 02:17:10.000000 tej_tool_api-1.1.2/TejToolAPI/TejToolAPI.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-17 02:17:10.000000 tej_tool_api-1.1.2/TejToolAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-17 02:17:15.000000 tej_tool_api-1.1.2/TejToolAPI/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-04-17 02:17:10.000000 tej_tool_api-1.1.2/TejToolAPI/exchange_calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-17 02:17:10.000000 tej_tool_api-1.1.2/TejToolAPI/meta_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-17 02:17:10.000000 tej_tool_api-1.1.2/TejToolAPI/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:15.607099 tej_tool_api-1.1.2/TejToolAPI/tables/
--rw-r--r--   0 runner    (1001) docker     (127)    24887 2024-04-17 02:17:10.000000 tej_tool_api-1.1.2/TejToolAPI/tables/all_meta.json
--rw-r--r--   0 runner    (1001) docker     (127)    62159 2024-04-17 02:17:10.000000 tej_tool_api-1.1.2/TejToolAPI/tables/columns_group.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-17 02:17:10.000000 tej_tool_api-1.1.2/TejToolAPI/tables/~$columns_group.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-17 02:17:10.000000 tej_tool_api-1.1.2/TejToolAPI/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-17 02:17:10.000000 tej_tool_api-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 02:17:15.607099 tej_tool_api-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-17 02:17:10.000000 tej_tool_api-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:17:15.607099 tej_tool_api-1.1.2/tej_tool_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-17 02:17:15.000000 tej_tool_api-1.1.2/tej_tool_api.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:41:55.945784 tej_tool_api-1.1.2rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-04-16 09:41:48.000000 tej_tool_api-1.1.2rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-16 09:41:48.000000 tej_tool_api-1.1.2rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-04-16 09:41:55.945784 tej_tool_api-1.1.2rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-16 09:41:48.000000 tej_tool_api-1.1.2rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:41:55.945784 tej_tool_api-1.1.2rc0/TejToolAPI/
+-rw-r--r--   0 runner    (1001) docker     (127)    29372 2024-04-16 09:41:48.000000 tej_tool_api-1.1.2rc0/TejToolAPI/Map_Dask_API.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13543 2024-04-16 09:41:48.000000 tej_tool_api-1.1.2rc0/TejToolAPI/TejToolAPI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-16 09:41:48.000000 tej_tool_api-1.1.2rc0/TejToolAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-16 09:41:55.000000 tej_tool_api-1.1.2rc0/TejToolAPI/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-04-16 09:41:48.000000 tej_tool_api-1.1.2rc0/TejToolAPI/exchange_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-16 09:41:48.000000 tej_tool_api-1.1.2rc0/TejToolAPI/meta_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-16 09:41:48.000000 tej_tool_api-1.1.2rc0/TejToolAPI/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:41:55.945784 tej_tool_api-1.1.2rc0/TejToolAPI/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)    24887 2024-04-16 09:41:48.000000 tej_tool_api-1.1.2rc0/TejToolAPI/tables/all_meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)    62159 2024-04-16 09:41:48.000000 tej_tool_api-1.1.2rc0/TejToolAPI/tables/columns_group.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-16 09:41:48.000000 tej_tool_api-1.1.2rc0/TejToolAPI/tables/~$columns_group.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-16 09:41:48.000000 tej_tool_api-1.1.2rc0/TejToolAPI/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-16 09:41:48.000000 tej_tool_api-1.1.2rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 09:41:55.945784 tej_tool_api-1.1.2rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-16 09:41:48.000000 tej_tool_api-1.1.2rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 09:41:55.945784 tej_tool_api-1.1.2rc0/tej_tool_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-16 09:41:55.000000 tej_tool_api-1.1.2rc0/tej_tool_api.egg-info/SOURCES.txt
```

### Comparing `tej_tool_api-1.1.2/LICENSE` & `tej_tool_api-1.1.2rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `tej_tool_api-1.1.2/PKG-INFO` & `tej_tool_api-1.1.2rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tej-tool-api
-Version: 1.1.2
+Version: 1.1.2rc0
 Summary: Package to fetch a large quantity of data from tejapi.
 Author: tej
 Author-email: tej@tej.com.tw
 Maintainer: tej api Development Team
 Maintainer-email: tej@tej.com.tw
 License: Apache-2.0
 Project-URL: homepage, https://api.tej.com.tw
```

### Comparing `tej_tool_api-1.1.2/README.md` & `tej_tool_api-1.1.2rc0/README.md`

 * *Files identical despite different names*

### Comparing `tej_tool_api-1.1.2/TejToolAPI/Map_Dask_API.py` & `tej_tool_api-1.1.2rc0/TejToolAPI/Map_Dask_API.py`

 * *Files identical despite different names*

### Comparing `tej_tool_api-1.1.2/TejToolAPI/TejToolAPI.py` & `tej_tool_api-1.1.2rc0/TejToolAPI/TejToolAPI.py`

 * *Files identical despite different names*

### Comparing `tej_tool_api-1.1.2/TejToolAPI/__init__.py` & `tej_tool_api-1.1.2rc0/TejToolAPI/__init__.py`

 * *Files identical despite different names*

### Comparing `tej_tool_api-1.1.2/TejToolAPI/exchange_calendar.py` & `tej_tool_api-1.1.2rc0/TejToolAPI/exchange_calendar.py`

 * *Files identical despite different names*

### Comparing `tej_tool_api-1.1.2/TejToolAPI/meta_types.py` & `tej_tool_api-1.1.2rc0/TejToolAPI/meta_types.py`

 * *Files identical despite different names*

### Comparing `tej_tool_api-1.1.2/TejToolAPI/parameters.py` & `tej_tool_api-1.1.2rc0/TejToolAPI/parameters.py`

 * *Files identical despite different names*

### Comparing `tej_tool_api-1.1.2/TejToolAPI/tables/all_meta.json` & `tej_tool_api-1.1.2rc0/TejToolAPI/tables/all_meta.json`

 * *Files identical despite different names*

### Comparing `tej_tool_api-1.1.2/TejToolAPI/tables/columns_group.xlsx` & `tej_tool_api-1.1.2rc0/TejToolAPI/tables/columns_group.xlsx`

 * *Files identical despite different names*

### Comparing `tej_tool_api-1.1.2/TejToolAPI/utils.py` & `tej_tool_api-1.1.2rc0/TejToolAPI/utils.py`

 * *Files identical despite different names*

### Comparing `tej_tool_api-1.1.2/pyproject.toml` & `tej_tool_api-1.1.2rc0/pyproject.toml`

 * *Files identical despite different names*

