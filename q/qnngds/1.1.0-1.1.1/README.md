# Comparing `tmp/qnngds-1.1.0.tar.gz` & `tmp/qnngds-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qnngds-1.1.0.tar", last modified: Tue Apr  9 18:48:14 2024, max compression
+gzip compressed data, was "qnngds-1.1.1.tar", last modified: Wed Apr 17 18:51:59 2024, max compression
```

## Comparing `qnngds-1.1.0.tar` & `qnngds-1.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1081 2024-04-09 18:48:09.367252 qnngds-1.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1129 2024-04-09 18:48:09.367252 qnngds-1.1.0/README.md
--rw-r--r--   0        0        0     1161 2024-04-09 18:48:14.255247 qnngds-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      112 2024-04-09 18:48:09.371252 qnngds-1.1.0/src/qnngds/__init__.py
--rw-r--r--   0        0        0    10600 2024-04-09 18:48:09.371252 qnngds-1.1.0/src/qnngds/circuits.py
--rw-r--r--   0        0        0    51283 2024-04-09 18:48:09.371252 qnngds-1.1.0/src/qnngds/design.py
--rw-r--r--   0        0        0    13740 2024-04-09 18:48:09.371252 qnngds-1.1.0/src/qnngds/devices.py
--rw-r--r--   0        0        0     8244 2024-04-09 18:48:09.375252 qnngds-1.1.0/src/qnngds/geometries.py
--rw-r--r--   0        0        0    21375 2024-04-09 18:48:09.375252 qnngds-1.1.0/src/qnngds/utilities.py
--rw-r--r--   0        0        0     3301 1970-01-01 00:00:00.000000 qnngds-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-17 18:51:55.915072 qnngds-1.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     1129 2024-04-17 18:51:55.915072 qnngds-1.1.1/README.md
+-rw-r--r--   0        0        0     1161 2024-04-17 18:51:59.127080 qnngds-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      112 2024-04-17 18:51:55.919072 qnngds-1.1.1/src/qnngds/__init__.py
+-rw-r--r--   0        0        0    10600 2024-04-17 18:51:55.919072 qnngds-1.1.1/src/qnngds/circuits.py
+-rw-r--r--   0        0        0    51283 2024-04-17 18:51:55.919072 qnngds-1.1.1/src/qnngds/design.py
+-rw-r--r--   0        0        0    13740 2024-04-17 18:51:55.919072 qnngds-1.1.1/src/qnngds/devices.py
+-rw-r--r--   0        0        0     8244 2024-04-17 18:51:55.919072 qnngds-1.1.1/src/qnngds/geometries.py
+-rw-r--r--   0        0        0    21375 2024-04-17 18:51:55.919072 qnngds-1.1.1/src/qnngds/utilities.py
+-rw-r--r--   0        0        0     3309 1970-01-01 00:00:00.000000 qnngds-1.1.1/PKG-INFO
```

### Comparing `qnngds-1.1.0/LICENSE.txt` & `qnngds-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qnngds-1.1.0/README.md` & `qnngds-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `qnngds-1.1.0/pyproject.toml` & `qnngds-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "qnngds"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
     { name = "A. Jacquillat", email = "audrey01@mit.edu" },
     { name = "A. Jacquillat", email = "audrey.jacquillat@gmail.com" },
     { name = "R. Foster", email = "reedf@mit.edu" },
 ]
 maintainers = [
     { name = "A. Jacquillat", email = "audrey01@mit.edu" },
```

### Comparing `qnngds-1.1.0/src/qnngds/circuits.py` & `qnngds-1.1.1/src/qnngds/circuits.py`

 * *Files identical despite different names*

### Comparing `qnngds-1.1.0/src/qnngds/design.py` & `qnngds-1.1.1/src/qnngds/design.py`

 * *Files identical despite different names*

### Comparing `qnngds-1.1.0/src/qnngds/devices.py` & `qnngds-1.1.1/src/qnngds/devices.py`

 * *Files identical despite different names*

### Comparing `qnngds-1.1.0/src/qnngds/geometries.py` & `qnngds-1.1.1/src/qnngds/geometries.py`

 * *Files identical despite different names*

### Comparing `qnngds-1.1.0/src/qnngds/utilities.py` & `qnngds-1.1.1/src/qnngds/utilities.py`

 * *Files identical despite different names*

### Comparing `qnngds-1.1.0/PKG-INFO` & `qnngds-1.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: qnngds
-Version: 1.1.0
+Version: 1.1.1
 Summary: The QNN library for creating gds files
-Keywords: phidl nanowire_electronics nanofabrication gds
-Author-Email: A. Jacquillat <audrey01@mit.edu>, A. Jacquillat <audrey.jacquillat@gmail.com>, R. Foster <reedf@mit.edu>
-Maintainer-Email: A. Jacquillat <audrey01@mit.edu>
+Keywords: phidl,nanowire_electronics,nanofabrication,gds
+Author-Email: "A. Jacquillat" <audrey01@mit.edu>, "A. Jacquillat" <audrey.jacquillat@gmail.com>, "R. Foster" <reedf@mit.edu>
+Maintainer-Email: "A. Jacquillat" <audrey01@mit.edu>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
         use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
         of the Software, and to permit persons to whom the Software is furnished to do
```

