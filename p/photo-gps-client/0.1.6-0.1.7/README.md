# Comparing `tmp/photo_gps_client-0.1.6.tar.gz` & `tmp/photo_gps_client-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "photo_gps_client-0.1.6.tar", max compression
+gzip compressed data, was "photo_gps_client-0.1.7.tar", max compression
```

## Comparing `photo_gps_client-0.1.6.tar` & `photo_gps_client-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       86 2024-04-17 18:35:03.061611 photo_gps_client-0.1.6/README.md
--rw-r--r--   0        0        0      532 2024-04-17 16:36:49.817402 photo_gps_client-0.1.6/photo_gps/DSCF0311.xmp
--rw-r--r--   0        0        0      534 2024-04-15 20:17:07.000000 photo_gps_client-0.1.6/photo_gps/DSCF0312.xmp
--rw-r--r--   0        0        0      534 2024-04-15 20:17:07.000000 photo_gps_client-0.1.6/photo_gps/DSCF0313.xmp
--rw-r--r--   0        0        0        0 2024-04-13 11:43:05.727802 photo_gps_client-0.1.6/photo_gps/__init__.py
--rw-r--r--   0        0        0     2711 2024-04-17 17:05:22.779144 photo_gps_client-0.1.6/photo_gps/commands.py
--rw-r--r--   0        0        0     1272 2024-04-17 17:00:45.203444 photo_gps_client-0.1.6/photo_gps/config.py
--rw-r--r--   0        0        0      551 2024-04-17 18:26:05.323417 photo_gps_client-0.1.6/photo_gps/jinja/xmp.jinja
--rw-r--r--   0        0        0      327 2024-04-17 16:51:39.780517 photo_gps_client-0.1.6/photo_gps/photogps.example.yaml
--rw-r--r--   0        0        0     1112 2024-04-17 17:01:24.642844 photo_gps_client-0.1.6/photo_gps/photogps.py
--rw-r--r--   0        0        0     2881 2024-04-17 18:26:05.326871 photo_gps_client-0.1.6/photo_gps/tools.py
--rw-r--r--   0        0        0      686 2024-04-17 18:31:44.388155 photo_gps_client-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      660 1970-01-01 00:00:00.000000 photo_gps_client-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       86 2024-04-17 18:35:03.061611 photo_gps_client-0.1.7/README.md
+-rw-r--r--   0        0        0      532 2024-04-17 16:36:49.817402 photo_gps_client-0.1.7/photo_gps/DSCF0311.xmp
+-rw-r--r--   0        0        0      534 2024-04-15 20:17:07.000000 photo_gps_client-0.1.7/photo_gps/DSCF0312.xmp
+-rw-r--r--   0        0        0      534 2024-04-15 20:17:07.000000 photo_gps_client-0.1.7/photo_gps/DSCF0313.xmp
+-rw-r--r--   0        0        0        0 2024-04-13 11:43:05.727802 photo_gps_client-0.1.7/photo_gps/__init__.py
+-rw-r--r--   0        0        0     2711 2024-04-17 17:05:22.779144 photo_gps_client-0.1.7/photo_gps/commands.py
+-rw-r--r--   0        0        0     1272 2024-04-17 17:00:45.203444 photo_gps_client-0.1.7/photo_gps/config.py
+-rw-r--r--   0        0        0      551 2024-04-17 18:51:53.580694 photo_gps_client-0.1.7/photo_gps/jinja/xmp.jinja
+-rw-r--r--   0        0        0      327 2024-04-17 16:51:39.780517 photo_gps_client-0.1.7/photo_gps/photogps.example.yaml
+-rw-r--r--   0        0        0     1112 2024-04-17 17:01:24.642844 photo_gps_client-0.1.7/photo_gps/photogps.py
+-rw-r--r--   0        0        0     2881 2024-04-17 18:26:05.326871 photo_gps_client-0.1.7/photo_gps/tools.py
+-rw-r--r--   0        0        0      686 2024-04-17 18:53:29.866329 photo_gps_client-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      660 1970-01-01 00:00:00.000000 photo_gps_client-0.1.7/PKG-INFO
```

### Comparing `photo_gps_client-0.1.6/photo_gps/DSCF0311.xmp` & `photo_gps_client-0.1.7/photo_gps/DSCF0311.xmp`

 * *Files identical despite different names*

### Comparing `photo_gps_client-0.1.6/photo_gps/DSCF0312.xmp` & `photo_gps_client-0.1.7/photo_gps/DSCF0312.xmp`

 * *Files identical despite different names*

### Comparing `photo_gps_client-0.1.6/photo_gps/DSCF0313.xmp` & `photo_gps_client-0.1.7/photo_gps/DSCF0313.xmp`

 * *Files identical despite different names*

### Comparing `photo_gps_client-0.1.6/photo_gps/commands.py` & `photo_gps_client-0.1.7/photo_gps/commands.py`

 * *Files identical despite different names*

### Comparing `photo_gps_client-0.1.6/photo_gps/config.py` & `photo_gps_client-0.1.7/photo_gps/config.py`

 * *Files identical despite different names*

### Comparing `photo_gps_client-0.1.6/photo_gps/jinja/xmp.jinja` & `photo_gps_client-0.1.7/photo_gps/jinja/xmp.jinja`

 * *Files identical despite different names*

### Comparing `photo_gps_client-0.1.6/photo_gps/photogps.py` & `photo_gps_client-0.1.7/photo_gps/photogps.py`

 * *Files identical despite different names*

### Comparing `photo_gps_client-0.1.6/photo_gps/tools.py` & `photo_gps_client-0.1.7/photo_gps/tools.py`

 * *Files identical despite different names*

### Comparing `photo_gps_client-0.1.6/pyproject.toml` & `photo_gps_client-0.1.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "photo-gps-client"
-version = "0.1.6"  # set by antonio-py-dynamic-version
+version = "0.1.7"  # set by antonio-py-dynamic-version
 description = ""
 authors = ["antonio <mr.antonsilin@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "photo_gps"},
 ]
```

### Comparing `photo_gps_client-0.1.6/PKG-INFO` & `photo_gps_client-0.1.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photo-gps-client
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: antonio
 Author-email: mr.antonsilin@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arrow (>=1.3.0,<2.0.0)
```
