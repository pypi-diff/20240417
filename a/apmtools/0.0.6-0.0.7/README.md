# Comparing `tmp/apmtools-0.0.6.tar.gz` & `tmp/apmtools-0.0.7.tar.gz`

## Comparing `apmtools-0.0.6.tar` & `apmtools-0.0.7.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apmtools-0.0.6/src/apmtools/__init__.py
--rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 apmtools-0.0.6/src/apmtools/classes.py
--rw-r--r--   0        0        0    17745 2020-02-02 00:00:00.000000 apmtools-0.0.6/src/apmtools/data_processing.py
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 apmtools-0.0.6/src/apmtools/functions.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 apmtools-0.0.6/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 apmtools-0.0.6/LICENSE
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 apmtools-0.0.6/README.md
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 apmtools-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 apmtools-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0  4949333 2020-02-02 00:00:00.000000 apmtools-0.0.7/test.zip
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apmtools-0.0.7/src/apmtools/__init__.py
+-rw-r--r--   0        0        0    10412 2020-02-02 00:00:00.000000 apmtools-0.0.7/src/apmtools/classes.py
+-rw-r--r--   0        0        0    17745 2020-02-02 00:00:00.000000 apmtools-0.0.7/src/apmtools/data_processing.py
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 apmtools-0.0.7/src/apmtools/functions.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 apmtools-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 apmtools-0.0.7/LICENSE
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 apmtools-0.0.7/README.md
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 apmtools-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 apmtools-0.0.7/PKG-INFO
```

### Comparing `apmtools-0.0.6/src/apmtools/classes.py` & `apmtools-0.0.7/src/apmtools/classes.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,43 +16,69 @@
         If number is not specified, returns the values associated with the first key
         """
         try:
             return (self[list(self.keys())[number]])
         except:
             print("something's wrong")
 
-    def subset(self, filter_dict):
+    def subset(self, filter_dict, filter_style='all'):
         """
         Return a subset of a dictionary, specified in filter_dict (itself a dictionary)
         filter_dict is {attrib:["attrib_value_x","attrib_value_y",..]}, where 
             attrib is an attribute of the elements of dictionary, and attrib_value is a list
             of the values of such attrib that the elements of returned dictionary can have    
+        
+        specify filter_style='all' if all conditions should be met to be included in the return dictionary, specify filter_style='any' for including when any condition is met. Default is 'all'.
         """
         if type(filter_dict) != type(dict()):
             print("subset function error: type filter_dict should be dict")
             return
         return_dict = self
-        for i, j in filter_dict.items():
+        if filter_style=='any':
             a = {}
-            for key, value in return_dict.items():
-                if hasattr(value, 'meta') & (type(value.meta) == type({})) & (i in value.meta.keys()):
-                    try:
-                        if value.__getattr__('meta')[i] in j:
-                            a[key] = value
-                    except:
-                        pass
-                else:
-                    try:
-                        if value.__getattr__(i) in j:
-                            a[key] = value
-                    except:
-                        pass
+            for key, value in return_dict.items():            
+                for i, j in filter_dict.items():
+                    if hasattr(value, 'meta') & (type(value.meta) == type({})) & (i in value.meta.keys()):
+                        try:
+                            if value.__getattr__('meta')[i] in j:
+                                a[key] = value
+                        except:
+                            pass
+                    else:
+                        try:
+                            if value.__getattr__(i) in j:
+                                a[key] = value
+                        except:
+                            pass
+        if filter_style == 'all':
+            a = {}            
+            for key, value in return_dict.items():           
+                for i, j in filter_dict.items():
+                    if hasattr(value, 'meta') & (type(value.meta) == type({})) & (i in value.meta.keys()):
+                        try:
+                            if value.__getattr__('meta')[i] in j:
+                                a[key] = value
+                            else:
+                                if key in a.keys():
+                                    del a[key]
+                        except:
+                            pass
+                    else:
+                        try:
+                            if value.__getattr__(i) in j:
+                                a[key] = value
+                            else:
+                                if key in a.keys():
+                                    del a[key]
+                        except:
+                            pass
 
         return DictionaryPlus(a)
 
+
     def set_attrib(self, attribute):
         """
         returns the set of attribute values for dictionary
         """
         return_set = set()
         for i in self.values():
             if hasattr(i, 'meta') & (type(i.meta) == type({})) & (attribute in i.meta.keys()):
```

### Comparing `apmtools-0.0.6/src/apmtools/data_processing.py` & `apmtools-0.0.7/src/apmtools/data_processing.py`

 * *Files identical despite different names*

### Comparing `apmtools-0.0.6/src/apmtools/functions.py` & `apmtools-0.0.7/src/apmtools/functions.py`

 * *Files identical despite different names*

### Comparing `apmtools-0.0.6/LICENSE` & `apmtools-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `apmtools-0.0.6/pyproject.toml` & `apmtools-0.0.7/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "apmtools"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Federico Lorenzetti", email="lorenzetti.federico@gmail.com" },
 ]
 description = "A collection of tools for processing air pollution monitoring data"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `apmtools-0.0.6/PKG-INFO` & `apmtools-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: apmtools
-Version: 0.0.6
+Version: 0.0.7
 Summary: A collection of tools for processing air pollution monitoring data
 Project-URL: Homepage, https://github.com/federlorenz/apmtools
 Author-email: Federico Lorenzetti <lorenzetti.federico@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

