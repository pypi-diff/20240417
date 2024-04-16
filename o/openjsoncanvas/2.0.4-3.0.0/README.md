# Comparing `tmp/openjsoncanvas-2.0.4.tar.gz` & `tmp/openjsoncanvas-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openjsoncanvas-2.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "openjsoncanvas-3.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `openjsoncanvas-2.0.4.tar` & `openjsoncanvas-3.0.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1102 2024-04-12 12:47:53.175260 openjsoncanvas-2.0.4/LICENSE
--rw-r--r--   0        0        0     1772 2024-04-12 23:27:55.463768 openjsoncanvas-2.0.4/README.md
--rw-r--r--   0        0        0     4966 2024-04-13 00:54:23.552138 openjsoncanvas-2.0.4/openjsoncanvas.py
--rw-r--r--   0        0        0      471 2024-04-12 23:28:41.108195 openjsoncanvas-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     2120 1970-01-01 00:00:00.000000 openjsoncanvas-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-04-12 12:47:53.175260 openjsoncanvas-3.0.0/LICENSE
+-rw-r--r--   0        0        0     1772 2024-04-12 23:27:55.463768 openjsoncanvas-3.0.0/README.md
+-rw-r--r--   0        0        0     7732 2024-04-16 23:04:48.751395 openjsoncanvas-3.0.0/openjsoncanvas.py
+-rw-r--r--   0        0        0      471 2024-04-12 23:28:41.108195 openjsoncanvas-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2120 1970-01-01 00:00:00.000000 openjsoncanvas-3.0.0/PKG-INFO
```

### Comparing `openjsoncanvas-2.0.4/LICENSE` & `openjsoncanvas-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openjsoncanvas-2.0.4/README.md` & `openjsoncanvas-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `openjsoncanvas-2.0.4/PKG-INFO` & `openjsoncanvas-3.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openjsoncanvas
-Version: 2.0.4
+Version: 3.0.0
 Summary: A python implementation of the JsonCanvas format: https://github.com/obsidianmd/jsoncanvas/blob/main/spec/1.0.md
 Author: Alyce Osbourne
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pydantic
 Project-URL: Home, https://github.com/AlyceOsbourne/openjsoncanvas
```

