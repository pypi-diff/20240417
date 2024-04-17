# Comparing `tmp/apmtools-0.0.5.tar.gz` & `tmp/apmtools-0.0.6.tar.gz`

## Comparing `apmtools-0.0.5.tar` & `apmtools-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apmtools-0.0.5/src/apmtools/__init__.py
--rw-r--r--   0        0        0     9091 2020-02-02 00:00:00.000000 apmtools-0.0.5/src/apmtools/classes.py
--rw-r--r--   0        0        0    17745 2020-02-02 00:00:00.000000 apmtools-0.0.5/src/apmtools/data_processing.py
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 apmtools-0.0.5/src/apmtools/functions.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 apmtools-0.0.5/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 apmtools-0.0.5/LICENSE
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 apmtools-0.0.5/README.md
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 apmtools-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 apmtools-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apmtools-0.0.6/src/apmtools/__init__.py
+-rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 apmtools-0.0.6/src/apmtools/classes.py
+-rw-r--r--   0        0        0    17745 2020-02-02 00:00:00.000000 apmtools-0.0.6/src/apmtools/data_processing.py
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 apmtools-0.0.6/src/apmtools/functions.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 apmtools-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 apmtools-0.0.6/LICENSE
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 apmtools-0.0.6/README.md
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 apmtools-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 apmtools-0.0.6/PKG-INFO
```

### Comparing `apmtools-0.0.5/src/apmtools/classes.py` & `apmtools-0.0.6/src/apmtools/classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
                 else:
                     try:
                         if value.__getattr__(i) in j:
                             a[key] = value
                     except:
                         pass
 
-        return DictionaryPlus(return_dict)
+        return DictionaryPlus(a)
 
     def set_attrib(self, attribute):
         """
         returns the set of attribute values for dictionary
         """
         return_set = set()
         for i in self.values():
```

### Comparing `apmtools-0.0.5/src/apmtools/data_processing.py` & `apmtools-0.0.6/src/apmtools/data_processing.py`

 * *Files identical despite different names*

### Comparing `apmtools-0.0.5/src/apmtools/functions.py` & `apmtools-0.0.6/src/apmtools/functions.py`

 * *Files identical despite different names*

### Comparing `apmtools-0.0.5/LICENSE` & `apmtools-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `apmtools-0.0.5/pyproject.toml` & `apmtools-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "apmtools"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Federico Lorenzetti", email="lorenzetti.federico@gmail.com" },
 ]
 description = "A collection of tools for processing air pollution monitoring data"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `apmtools-0.0.5/PKG-INFO` & `apmtools-0.0.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: apmtools
-Version: 0.0.5
+Version: 0.0.6
 Summary: A collection of tools for processing air pollution monitoring data
 Project-URL: Homepage, https://github.com/federlorenz/apmtools
 Author-email: Federico Lorenzetti <lorenzetti.federico@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

