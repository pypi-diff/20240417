# Comparing `tmp/olspow-1.0.2.tar.gz` & `tmp/olspow-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olspow-1.0.2.tar", last modified: Wed Apr 17 06:13:41 2024, max compression
+gzip compressed data, was "olspow-1.0.3.tar", last modified: Wed Apr 17 16:27:41 2024, max compression
```

## Comparing `olspow-1.0.2.tar` & `olspow-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 benjaminknight   (502) staff       (20)        0 2024-04-17 06:13:41.787058 olspow-1.0.2/
--rw-r--r--   0 benjaminknight   (502) staff       (20)     1074 2024-01-30 22:10:55.000000 olspow-1.0.2/LICENSE
--rw-r--r--   0 benjaminknight   (502) staff       (20)     5513 2024-04-17 06:13:41.786636 olspow-1.0.2/PKG-INFO
--rw-r--r--   0 benjaminknight   (502) staff       (20)     4858 2024-04-16 03:57:58.000000 olspow-1.0.2/README.md
--rw-r--r--   0 benjaminknight   (502) staff       (20)      734 2024-04-16 04:05:15.000000 olspow-1.0.2/pyproject.toml
--rw-r--r--   0 benjaminknight   (502) staff       (20)       38 2024-04-17 06:13:41.787144 olspow-1.0.2/setup.cfg
-drwxr-xr-x   0 benjaminknight   (502) staff       (20)        0 2024-04-17 06:13:41.783994 olspow-1.0.2/src/
--rw-r--r--   0 benjaminknight   (502) staff       (20)       76 2024-04-16 04:05:09.000000 olspow-1.0.2/src/__init__.py
-drwxr-xr-x   0 benjaminknight   (502) staff       (20)        0 2024-04-17 06:13:41.786045 olspow-1.0.2/src/olspow.egg-info/
--rw-r--r--   0 benjaminknight   (502) staff       (20)     5513 2024-04-17 06:13:41.000000 olspow-1.0.2/src/olspow.egg-info/PKG-INFO
--rw-r--r--   0 benjaminknight   (502) staff       (20)      231 2024-04-17 06:13:41.000000 olspow-1.0.2/src/olspow.egg-info/SOURCES.txt
--rw-r--r--   0 benjaminknight   (502) staff       (20)        1 2024-04-17 06:13:41.000000 olspow-1.0.2/src/olspow.egg-info/dependency_links.txt
--rw-r--r--   0 benjaminknight   (502) staff       (20)       40 2024-04-17 06:13:41.000000 olspow-1.0.2/src/olspow.egg-info/requires.txt
--rw-r--r--   0 benjaminknight   (502) staff       (20)       16 2024-04-17 06:13:41.000000 olspow-1.0.2/src/olspow.egg-info/top_level.txt
--rw-r--r--   0 benjaminknight   (502) staff       (20)    32802 2024-04-17 05:35:09.000000 olspow-1.0.2/src/olspow.py
+drwxr-xr-x   0 benjaminknight   (502) staff       (20)        0 2024-04-17 16:27:41.318904 olspow-1.0.3/
+-rw-r--r--   0 benjaminknight   (502) staff       (20)     1074 2024-01-30 22:10:55.000000 olspow-1.0.3/LICENSE
+-rw-r--r--   0 benjaminknight   (502) staff       (20)     5513 2024-04-17 16:27:41.318536 olspow-1.0.3/PKG-INFO
+-rw-r--r--   0 benjaminknight   (502) staff       (20)     4858 2024-04-16 03:57:58.000000 olspow-1.0.3/README.md
+-rw-r--r--   0 benjaminknight   (502) staff       (20)      734 2024-04-17 16:26:27.000000 olspow-1.0.3/pyproject.toml
+-rw-r--r--   0 benjaminknight   (502) staff       (20)       38 2024-04-17 16:27:41.318981 olspow-1.0.3/setup.cfg
+drwxr-xr-x   0 benjaminknight   (502) staff       (20)        0 2024-04-17 16:27:41.315002 olspow-1.0.3/src/
+drwxr-xr-x   0 benjaminknight   (502) staff       (20)        0 2024-04-17 16:27:41.316254 olspow-1.0.3/src/olspow/
+-rw-r--r--   0 benjaminknight   (502) staff       (20)       76 2024-04-17 16:26:32.000000 olspow-1.0.3/src/olspow/__init__.py
+-rw-r--r--   0 benjaminknight   (502) staff       (20)    32802 2024-04-17 05:35:09.000000 olspow-1.0.3/src/olspow/olspow.py
+drwxr-xr-x   0 benjaminknight   (502) staff       (20)        0 2024-04-17 16:27:41.318050 olspow-1.0.3/src/olspow.egg-info/
+-rw-r--r--   0 benjaminknight   (502) staff       (20)     5513 2024-04-17 16:27:41.000000 olspow-1.0.3/src/olspow.egg-info/PKG-INFO
+-rw-r--r--   0 benjaminknight   (502) staff       (20)      245 2024-04-17 16:27:41.000000 olspow-1.0.3/src/olspow.egg-info/SOURCES.txt
+-rw-r--r--   0 benjaminknight   (502) staff       (20)        1 2024-04-17 16:27:41.000000 olspow-1.0.3/src/olspow.egg-info/dependency_links.txt
+-rw-r--r--   0 benjaminknight   (502) staff       (20)       40 2024-04-17 16:27:41.000000 olspow-1.0.3/src/olspow.egg-info/requires.txt
+-rw-r--r--   0 benjaminknight   (502) staff       (20)        7 2024-04-17 16:27:41.000000 olspow-1.0.3/src/olspow.egg-info/top_level.txt
```

### Comparing `olspow-1.0.2/LICENSE` & `olspow-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `olspow-1.0.2/PKG-INFO` & `olspow-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olspow
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python package for conducting power analysis given ratio metrics, clustered data, and covariate adjustment.
 Author-email: "Benjamin S. Knight" <knight.benjamin@gmail.com>
 Project-URL: Homepage, https://github.com/b-knight/olspow
 Project-URL: Issues, https://github.com/b-knight/olspow/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `olspow-1.0.2/README.md` & `olspow-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `olspow-1.0.2/pyproject.toml` & `olspow-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "olspow"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Benjamin S. Knight", email="knight.benjamin@gmail.com" },
 ]
 description = "Python package for conducting power analysis given ratio metrics, clustered data, and covariate adjustment."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `olspow-1.0.2/src/olspow.egg-info/PKG-INFO` & `olspow-1.0.3/src/olspow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olspow
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python package for conducting power analysis given ratio metrics, clustered data, and covariate adjustment.
 Author-email: "Benjamin S. Knight" <knight.benjamin@gmail.com>
 Project-URL: Homepage, https://github.com/b-knight/olspow
 Project-URL: Issues, https://github.com/b-knight/olspow/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `olspow-1.0.2/src/olspow.py` & `olspow-1.0.3/src/olspow/olspow.py`

 * *Files identical despite different names*

