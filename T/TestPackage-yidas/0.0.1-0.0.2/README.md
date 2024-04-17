# Comparing `tmp/testpackage_yidas-0.0.1.tar.gz` & `tmp/testpackage_yidas-0.0.2.tar.gz`

## Comparing `testpackage_yidas-0.0.1.tar` & `testpackage_yidas-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 testpackage_yidas-0.0.1/setup.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 testpackage_yidas-0.0.1/src/TestPackage_yidas/TestClass.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 testpackage_yidas-0.0.1/src/TestPackage_yidas/__init__.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 testpackage_yidas-0.0.1/README.md
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 testpackage_yidas-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 testpackage_yidas-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 testpackage_yidas-0.0.2/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 testpackage_yidas-0.0.2/src/TestPackage_yidas/__init__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 testpackage_yidas-0.0.2/src/TestPackage_yidas/example.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 testpackage_yidas-0.0.2/README.md
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 testpackage_yidas-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 testpackage_yidas-0.0.2/PKG-INFO
```

### Comparing `testpackage_yidas-0.0.1/setup.py` & `testpackage_yidas-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `testpackage_yidas-0.0.1/pyproject.toml` & `testpackage_yidas-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "TestPackage_yidas"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `testpackage_yidas-0.0.1/PKG-INFO` & `testpackage_yidas-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: TestPackage_yidas
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Author-email: Example Author <author@example.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

