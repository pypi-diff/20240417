# Comparing `tmp/testpackage_yidas-0.0.2.tar.gz` & `tmp/testpackage_yidas-0.0.3.tar.gz`

## Comparing `testpackage_yidas-0.0.2.tar` & `testpackage_yidas-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 testpackage_yidas-0.0.2/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 testpackage_yidas-0.0.2/src/TestPackage_yidas/__init__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 testpackage_yidas-0.0.2/src/TestPackage_yidas/example.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 testpackage_yidas-0.0.2/README.md
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 testpackage_yidas-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 testpackage_yidas-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 testpackage_yidas-0.0.3/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 testpackage_yidas-0.0.3/src/TestPackage_yidas/__init__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 testpackage_yidas-0.0.3/src/TestPackage_yidas/example.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 testpackage_yidas-0.0.3/README.md
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 testpackage_yidas-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 testpackage_yidas-0.0.3/PKG-INFO
```

### Comparing `testpackage_yidas-0.0.2/setup.py` & `testpackage_yidas-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `testpackage_yidas-0.0.2/pyproject.toml` & `testpackage_yidas-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "TestPackage_yidas"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

