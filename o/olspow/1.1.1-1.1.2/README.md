# Comparing `tmp/olspow-1.1.1.tar.gz` & `tmp/olspow-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olspow-1.1.1.tar", last modified: Wed Apr 17 17:26:40 2024, max compression
+gzip compressed data, was "olspow-1.1.2.tar", last modified: Wed Apr 17 17:28:32 2024, max compression
```

## Comparing `olspow-1.1.1.tar` & `olspow-1.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 benjaminknight   (502) staff       (20)        0 2024-04-17 17:26:40.957516 olspow-1.1.1/
--rw-r--r--   0 benjaminknight   (502) staff       (20)     1074 2024-01-30 22:10:55.000000 olspow-1.1.1/LICENSE
--rw-r--r--   0 benjaminknight   (502) staff       (20)     5513 2024-04-17 17:26:40.957147 olspow-1.1.1/PKG-INFO
--rw-r--r--   0 benjaminknight   (502) staff       (20)     4858 2024-04-16 03:57:58.000000 olspow-1.1.1/README.md
--rw-r--r--   0 benjaminknight   (502) staff       (20)      734 2024-04-17 17:26:12.000000 olspow-1.1.1/pyproject.toml
--rw-r--r--   0 benjaminknight   (502) staff       (20)       38 2024-04-17 17:26:40.957605 olspow-1.1.1/setup.cfg
-drwxr-xr-x   0 benjaminknight   (502) staff       (20)        0 2024-04-17 17:26:40.953353 olspow-1.1.1/src/
-drwxr-xr-x   0 benjaminknight   (502) staff       (20)        0 2024-04-17 17:26:40.954753 olspow-1.1.1/src/olspow/
--rw-r--r--   0 benjaminknight   (502) staff       (20)       92 2024-04-17 17:26:03.000000 olspow-1.1.1/src/olspow/__init__.py
--rw-r--r--   0 benjaminknight   (502) staff       (20)    32802 2024-04-17 05:35:09.000000 olspow-1.1.1/src/olspow/olspow.py
-drwxr-xr-x   0 benjaminknight   (502) staff       (20)        0 2024-04-17 17:26:40.956629 olspow-1.1.1/src/olspow.egg-info/
--rw-r--r--   0 benjaminknight   (502) staff       (20)     5513 2024-04-17 17:26:40.000000 olspow-1.1.1/src/olspow.egg-info/PKG-INFO
--rw-r--r--   0 benjaminknight   (502) staff       (20)      245 2024-04-17 17:26:40.000000 olspow-1.1.1/src/olspow.egg-info/SOURCES.txt
--rw-r--r--   0 benjaminknight   (502) staff       (20)        1 2024-04-17 17:26:40.000000 olspow-1.1.1/src/olspow.egg-info/dependency_links.txt
--rw-r--r--   0 benjaminknight   (502) staff       (20)       40 2024-04-17 17:26:40.000000 olspow-1.1.1/src/olspow.egg-info/requires.txt
--rw-r--r--   0 benjaminknight   (502) staff       (20)        7 2024-04-17 17:26:40.000000 olspow-1.1.1/src/olspow.egg-info/top_level.txt
+drwxr-xr-x   0 benjaminknight   (502) staff       (20)        0 2024-04-17 17:28:32.835608 olspow-1.1.2/
+-rw-r--r--   0 benjaminknight   (502) staff       (20)     1074 2024-01-30 22:10:55.000000 olspow-1.1.2/LICENSE
+-rw-r--r--   0 benjaminknight   (502) staff       (20)     5513 2024-04-17 17:28:32.835204 olspow-1.1.2/PKG-INFO
+-rw-r--r--   0 benjaminknight   (502) staff       (20)     4858 2024-04-16 03:57:58.000000 olspow-1.1.2/README.md
+-rw-r--r--   0 benjaminknight   (502) staff       (20)      734 2024-04-17 17:27:52.000000 olspow-1.1.2/pyproject.toml
+-rw-r--r--   0 benjaminknight   (502) staff       (20)       38 2024-04-17 17:28:32.835704 olspow-1.1.2/setup.cfg
+drwxr-xr-x   0 benjaminknight   (502) staff       (20)        0 2024-04-17 17:28:32.831516 olspow-1.1.2/src/
+drwxr-xr-x   0 benjaminknight   (502) staff       (20)        0 2024-04-17 17:28:32.832870 olspow-1.1.2/src/olspow/
+-rw-r--r--   0 benjaminknight   (502) staff       (20)       92 2024-04-17 17:27:58.000000 olspow-1.1.2/src/olspow/__init__.py
+-rw-r--r--   0 benjaminknight   (502) staff       (20)    32802 2024-04-17 05:35:09.000000 olspow-1.1.2/src/olspow/olspow.py
+drwxr-xr-x   0 benjaminknight   (502) staff       (20)        0 2024-04-17 17:28:32.834585 olspow-1.1.2/src/olspow.egg-info/
+-rw-r--r--   0 benjaminknight   (502) staff       (20)     5513 2024-04-17 17:28:32.000000 olspow-1.1.2/src/olspow.egg-info/PKG-INFO
+-rw-r--r--   0 benjaminknight   (502) staff       (20)      245 2024-04-17 17:28:32.000000 olspow-1.1.2/src/olspow.egg-info/SOURCES.txt
+-rw-r--r--   0 benjaminknight   (502) staff       (20)        1 2024-04-17 17:28:32.000000 olspow-1.1.2/src/olspow.egg-info/dependency_links.txt
+-rw-r--r--   0 benjaminknight   (502) staff       (20)       40 2024-04-17 17:28:32.000000 olspow-1.1.2/src/olspow.egg-info/requires.txt
+-rw-r--r--   0 benjaminknight   (502) staff       (20)        7 2024-04-17 17:28:32.000000 olspow-1.1.2/src/olspow.egg-info/top_level.txt
```

### Comparing `olspow-1.1.1/LICENSE` & `olspow-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `olspow-1.1.1/PKG-INFO` & `olspow-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olspow
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python package for conducting power analysis given ratio metrics, clustered data, and covariate adjustment.
 Author-email: "Benjamin S. Knight" <knight.benjamin@gmail.com>
 Project-URL: Homepage, https://github.com/b-knight/olspow
 Project-URL: Issues, https://github.com/b-knight/olspow/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `olspow-1.1.1/README.md` & `olspow-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `olspow-1.1.1/pyproject.toml` & `olspow-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "olspow"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="Benjamin S. Knight", email="knight.benjamin@gmail.com" },
 ]
 description = "Python package for conducting power analysis given ratio metrics, clustered data, and covariate adjustment."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `olspow-1.1.1/src/olspow/olspow.py` & `olspow-1.1.2/src/olspow/olspow.py`

 * *Files identical despite different names*

### Comparing `olspow-1.1.1/src/olspow.egg-info/PKG-INFO` & `olspow-1.1.2/src/olspow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olspow
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python package for conducting power analysis given ratio metrics, clustered data, and covariate adjustment.
 Author-email: "Benjamin S. Knight" <knight.benjamin@gmail.com>
 Project-URL: Homepage, https://github.com/b-knight/olspow
 Project-URL: Issues, https://github.com/b-knight/olspow/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

