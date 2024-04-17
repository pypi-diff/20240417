# Comparing `tmp/multivariate_cwru-1.2.tar.gz` & `tmp/multivariate_cwru-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multivariate_cwru-1.2.tar", last modified: Tue Feb 27 10:31:04 2024, max compression
+gzip compressed data, was "multivariate_cwru-1.3.tar", last modified: Wed Apr 17 13:18:53 2024, max compression
```

## Comparing `multivariate_cwru-1.2.tar` & `multivariate_cwru-1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jhoogen    (501) staff       (20)        0 2024-02-27 10:31:04.784965 multivariate_cwru-1.2/
--rw-r--r--   0 jhoogen    (501) staff       (20)       58 2020-12-02 05:22:24.000000 multivariate_cwru-1.2/MANIFEST.in
--rw-r--r--   0 jhoogen    (501) staff       (20)     3187 2024-02-27 10:31:04.784818 multivariate_cwru-1.2/PKG-INFO
--rw-r--r--   0 jhoogen    (501) staff       (20)     2717 2020-12-03 09:51:32.000000 multivariate_cwru-1.2/README.MD
-drwxr-xr-x   0 jhoogen    (501) staff       (20)        0 2024-02-27 10:31:04.781390 multivariate_cwru-1.2/multivariate_cwru/
--rw-r--r--   0 jhoogen    (501) staff       (20)     5982 2024-02-27 10:22:23.000000 multivariate_cwru-1.2/multivariate_cwru/__init__.py
--rw-r--r--   0 jhoogen    (501) staff       (20)    14165 2022-05-13 09:51:24.000000 multivariate_cwru-1.2/multivariate_cwru/datafiles.txt
-drwxr-xr-x   0 jhoogen    (501) staff       (20)        0 2024-02-27 10:31:04.784288 multivariate_cwru-1.2/multivariate_cwru.egg-info/
--rw-r--r--   0 jhoogen    (501) staff       (20)     3187 2024-02-27 10:31:04.000000 multivariate_cwru-1.2/multivariate_cwru.egg-info/PKG-INFO
--rw-r--r--   0 jhoogen    (501) staff       (20)      276 2024-02-27 10:31:04.000000 multivariate_cwru-1.2/multivariate_cwru.egg-info/SOURCES.txt
--rw-r--r--   0 jhoogen    (501) staff       (20)        1 2024-02-27 10:31:04.000000 multivariate_cwru-1.2/multivariate_cwru.egg-info/dependency_links.txt
--rw-r--r--   0 jhoogen    (501) staff       (20)       18 2024-02-27 10:31:04.000000 multivariate_cwru-1.2/multivariate_cwru.egg-info/top_level.txt
--rw-r--r--   0 jhoogen    (501) staff       (20)       38 2024-02-27 10:31:04.785475 multivariate_cwru-1.2/setup.cfg
--rw-r--r--   0 jhoogen    (501) staff       (20)      856 2024-02-27 10:22:42.000000 multivariate_cwru-1.2/setup.py
+drwxr-xr-x   0 jhoogen    (501) staff       (20)        0 2024-04-17 13:18:53.847119 multivariate_cwru-1.3/
+-rw-r--r--   0 jhoogen    (501) staff       (20)       58 2020-12-02 05:22:24.000000 multivariate_cwru-1.3/MANIFEST.in
+-rw-r--r--   0 jhoogen    (501) staff       (20)     3187 2024-04-17 13:18:53.846910 multivariate_cwru-1.3/PKG-INFO
+-rw-r--r--   0 jhoogen    (501) staff       (20)     2717 2020-12-03 09:51:32.000000 multivariate_cwru-1.3/README.MD
+drwxr-xr-x   0 jhoogen    (501) staff       (20)        0 2024-04-17 13:18:53.842215 multivariate_cwru-1.3/multivariate_cwru/
+-rw-r--r--   0 jhoogen    (501) staff       (20)     5982 2024-02-27 10:22:23.000000 multivariate_cwru-1.3/multivariate_cwru/__init__.py
+-rw-r--r--   0 jhoogen    (501) staff       (20)    15549 2024-04-17 13:15:05.000000 multivariate_cwru-1.3/multivariate_cwru/datafiles.txt
+drwxr-xr-x   0 jhoogen    (501) staff       (20)        0 2024-04-17 13:18:53.846096 multivariate_cwru-1.3/multivariate_cwru.egg-info/
+-rw-r--r--   0 jhoogen    (501) staff       (20)     3187 2024-04-17 13:18:53.000000 multivariate_cwru-1.3/multivariate_cwru.egg-info/PKG-INFO
+-rw-r--r--   0 jhoogen    (501) staff       (20)      276 2024-04-17 13:18:53.000000 multivariate_cwru-1.3/multivariate_cwru.egg-info/SOURCES.txt
+-rw-r--r--   0 jhoogen    (501) staff       (20)        1 2024-04-17 13:18:53.000000 multivariate_cwru-1.3/multivariate_cwru.egg-info/dependency_links.txt
+-rw-r--r--   0 jhoogen    (501) staff       (20)       18 2024-04-17 13:18:53.000000 multivariate_cwru-1.3/multivariate_cwru.egg-info/top_level.txt
+-rw-r--r--   0 jhoogen    (501) staff       (20)       38 2024-04-17 13:18:53.847772 multivariate_cwru-1.3/setup.cfg
+-rw-r--r--   0 jhoogen    (501) staff       (20)      856 2024-04-17 13:15:42.000000 multivariate_cwru-1.3/setup.py
```

### Comparing `multivariate_cwru-1.2/PKG-INFO` & `multivariate_cwru-1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multivariate_cwru
-Version: 1.2
+Version: 1.3
 Summary: Preprocessed CWRU Bearing Dataset for multivariate signals
 Home-page: https://github.com/JvdHoogen/multivariate_cwru
 Author: Jurgen van den Hoogen
 Author-email: jurgenvandenhoogen@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `multivariate_cwru-1.2/README.MD` & `multivariate_cwru-1.3/README.MD`

 * *Files identical despite different names*

### Comparing `multivariate_cwru-1.2/multivariate_cwru/__init__.py` & `multivariate_cwru-1.3/multivariate_cwru/__init__.py`

 * *Files identical despite different names*

### Comparing `multivariate_cwru-1.2/multivariate_cwru.egg-info/PKG-INFO` & `multivariate_cwru-1.3/multivariate_cwru.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multivariate_cwru
-Version: 1.2
+Version: 1.3
 Summary: Preprocessed CWRU Bearing Dataset for multivariate signals
 Home-page: https://github.com/JvdHoogen/multivariate_cwru
 Author: Jurgen van den Hoogen
 Author-email: jurgenvandenhoogen@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `multivariate_cwru-1.2/setup.py` & `multivariate_cwru-1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="multivariate_cwru",
-    version="1.2",
+    version="1.3",
     author="Jurgen van den Hoogen",
     author_email="jurgenvandenhoogen@hotmail.com",
     description="Preprocessed CWRU Bearing Dataset for multivariate signals",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/JvdHoogen/multivariate_cwru",
     packages=setuptools.find_packages(),
```

