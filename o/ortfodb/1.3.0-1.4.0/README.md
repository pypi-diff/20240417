# Comparing `tmp/ortfodb-1.3.0.tar.gz` & `tmp/ortfodb-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ortfodb-1.3.0.tar", max compression
+gzip compressed data, was "ortfodb-1.4.0.tar", max compression
```

## Comparing `ortfodb-1.3.0.tar` & `ortfodb-1.4.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      209 2024-04-12 21:43:37.285597 ortfodb-1.3.0/README.md
--rw-r--r--   0        0        0      434 2024-04-12 21:42:27.066289 ortfodb-1.3.0/ortfodb/__init__.py
--rw-r--r--   0        0        0     8179 2024-04-16 10:41:08.684908 ortfodb-1.3.0/ortfodb/configuration.py
--rw-r--r--   0        0        0    15476 2024-04-16 10:41:09.568276 ortfodb-1.3.0/ortfodb/database.py
--rw-r--r--   0        0        0     5270 2024-04-16 10:41:10.408308 ortfodb-1.3.0/ortfodb/exporter.py
--rw-r--r--   0        0        0     2791 2024-04-16 10:41:11.231673 ortfodb-1.3.0/ortfodb/tags.py
--rw-r--r--   0        0        0     2750 2024-04-16 10:41:12.031704 ortfodb-1.3.0/ortfodb/technologies.py
--rw-r--r--   0        0        0      301 2024-04-16 10:41:13.608431 ortfodb-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 ortfodb-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      209 2024-04-12 21:43:37.285597 ortfodb-1.4.0/README.md
+-rw-r--r--   0        0        0      434 2024-04-12 21:42:27.066289 ortfodb-1.4.0/ortfodb/__init__.py
+-rw-r--r--   0        0        0     8179 2024-04-16 19:28:14.546364 ortfodb-1.4.0/ortfodb/configuration.py
+-rw-r--r--   0        0        0    15476 2024-04-16 19:28:15.419730 ortfodb-1.4.0/ortfodb/database.py
+-rw-r--r--   0        0        0     5270 2024-04-16 19:28:16.253094 ortfodb-1.4.0/ortfodb/exporter.py
+-rw-r--r--   0        0        0     2791 2024-04-16 19:28:17.069790 ortfodb-1.4.0/ortfodb/tags.py
+-rw-r--r--   0        0        0     2750 2024-04-16 19:28:17.869820 ortfodb-1.4.0/ortfodb/technologies.py
+-rw-r--r--   0        0        0      301 2024-04-16 19:28:19.246537 ortfodb-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 ortfodb-1.4.0/PKG-INFO
```

### Comparing `ortfodb-1.3.0/ortfodb/configuration.py` & `ortfodb-1.4.0/ortfodb/configuration.py`

 * *Files identical despite different names*

### Comparing `ortfodb-1.3.0/ortfodb/database.py` & `ortfodb-1.4.0/ortfodb/database.py`

 * *Files identical despite different names*

### Comparing `ortfodb-1.3.0/ortfodb/exporter.py` & `ortfodb-1.4.0/ortfodb/exporter.py`

 * *Files identical despite different names*

### Comparing `ortfodb-1.3.0/ortfodb/tags.py` & `ortfodb-1.4.0/ortfodb/tags.py`

 * *Files identical despite different names*

### Comparing `ortfodb-1.3.0/ortfodb/technologies.py` & `ortfodb-1.4.0/ortfodb/technologies.py`

 * *Files identical despite different names*

### Comparing `ortfodb-1.3.0/PKG-INFO` & `ortfodb-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ortfodb
-Version: 1.3.0
+Version: 1.4.0
 Summary: ortfodb client library
 License: MIT
 Author: Ewen Le Bihan
 Author-email: hey@ewen.works
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

