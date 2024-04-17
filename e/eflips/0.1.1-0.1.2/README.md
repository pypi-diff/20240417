# Comparing `tmp/eflips-0.1.1.tar.gz` & `tmp/eflips-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eflips-0.1.1.tar", max compression
+gzip compressed data, was "eflips-0.1.2.tar", max compression
```

## Comparing `eflips-0.1.1.tar` & `eflips-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2024-02-13 15:16:25.056236 eflips-0.1.1/README.md
--rw-r--r--   0        0        0      775 2024-02-13 15:16:52.177209 eflips-0.1.1/eflips/__init__.py
--rw-r--r--   0        0        0    67577 2024-02-13 15:16:52.177528 eflips-0.1.1/eflips/evaluation.py
--rw-r--r--   0        0        0    16924 2024-02-13 15:16:52.177715 eflips-0.1.1/eflips/helperFunctions.py
--rw-r--r--   0        0        0     7088 2024-02-13 15:16:52.177910 eflips-0.1.1/eflips/misc.py
--rw-r--r--   0        0        0     9313 2024-02-13 15:16:52.178074 eflips-0.1.1/eflips/settings.py
--rw-r--r--   0        0        0     2739 2024-02-13 15:16:52.178204 eflips-0.1.1/eflips/settings_files/default.json
--rw-r--r--   0        0        0      350 2024-02-13 15:16:52.178295 eflips-0.1.1/eflips/settings_files/exampledata.json
--rw-r--r--   0        0        0    42517 2024-02-13 15:16:52.178435 eflips-0.1.1/eflips/simpy_ext.py
--rw-r--r--   0        0        0      492 2024-02-13 15:17:23.995410 eflips-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 eflips-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-17 13:43:12.896849 eflips-0.1.2/README.md
+-rw-r--r--   0        0        0      775 2024-04-17 13:48:34.128607 eflips-0.1.2/eflips/__init__.py
+-rw-r--r--   0        0        0    67577 2024-04-17 13:48:34.128992 eflips-0.1.2/eflips/evaluation.py
+-rw-r--r--   0        0        0    16923 2024-04-17 13:49:25.547009 eflips-0.1.2/eflips/helperFunctions.py
+-rw-r--r--   0        0        0     7088 2024-04-17 13:48:34.129444 eflips-0.1.2/eflips/misc.py
+-rw-r--r--   0        0        0     9313 2024-04-17 13:48:34.129673 eflips-0.1.2/eflips/settings.py
+-rw-r--r--   0        0        0     2739 2024-04-17 13:48:34.130035 eflips-0.1.2/eflips/settings_files/default.json
+-rw-r--r--   0        0        0      350 2024-04-17 13:48:34.130141 eflips-0.1.2/eflips/settings_files/exampledata.json
+-rw-r--r--   0        0        0    42517 2024-04-17 13:48:34.130333 eflips-0.1.2/eflips/simpy_ext.py
+-rw-r--r--   0        0        0      492 2024-04-17 13:49:24.469405 eflips-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 eflips-0.1.2/PKG-INFO
```

### Comparing `eflips-0.1.1/eflips/__init__.py` & `eflips-0.1.2/eflips/__init__.py`

 * *Files identical despite different names*

### Comparing `eflips-0.1.1/eflips/evaluation.py` & `eflips-0.1.2/eflips/evaluation.py`

 * *Files identical despite different names*

### Comparing `eflips-0.1.1/eflips/helperFunctions.py` & `eflips-0.1.2/eflips/helperFunctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
 
 def add_class_attribute(obj, old_attribute_name, new_attribute_name):
     """Adds '_' in front of an object attribute.
     Internal function to change attribute name when using getter and setter
 
     Pavel Boev
     """
-    if old_attribute_name[0] is not '_' and\
+    if old_attribute_name[0] is != '_' and\
             hasattr(obj, '_' + old_attribute_name) is False:
         setattr(obj.__class__, new_attribute_name,
                 getattr(obj, old_attribute_name))
         # del obj.old_attribute_name
 
 
 def complex_setter(self, logObjClass, attr, new_attr_name, value):
```

### Comparing `eflips-0.1.1/eflips/misc.py` & `eflips-0.1.2/eflips/misc.py`

 * *Files identical despite different names*

### Comparing `eflips-0.1.1/eflips/settings.py` & `eflips-0.1.2/eflips/settings.py`

 * *Files identical despite different names*

### Comparing `eflips-0.1.1/eflips/settings_files/default.json` & `eflips-0.1.2/eflips/settings_files/default.json`

 * *Files identical despite different names*

### Comparing `eflips-0.1.1/eflips/simpy_ext.py` & `eflips-0.1.2/eflips/simpy_ext.py`

 * *Files identical despite different names*

### Comparing `eflips-0.1.1/PKG-INFO` & `eflips-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eflips
-Version: 0.1.1
+Version: 0.1.2
 Summary: eFLIPS: Electric Fleet and Infrastructure Planning/Simulation
 License: AGPLv3
 Author: D. Jefferies
 Author-email: dominic.jefferies@tu-berlin.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

