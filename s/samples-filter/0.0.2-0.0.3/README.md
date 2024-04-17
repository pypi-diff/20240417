# Comparing `tmp/samples-filter-0.0.2.tar.gz` & `tmp/samples-filter-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samples-filter-0.0.2.tar", last modified: Wed Apr 17 14:47:16 2024, max compression
+gzip compressed data, was "samples-filter-0.0.3.tar", last modified: Wed Apr 17 15:05:09 2024, max compression
```

## Comparing `samples-filter-0.0.2.tar` & `samples-filter-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 r         (1000) r         (1001)        0 2024-04-17 14:47:16.054175 samples-filter-0.0.2/
--rw-r--r--   0 r         (1000) r         (1001)     1087 2024-04-17 14:47:01.000000 samples-filter-0.0.2/LICENSE.txt
--rw-rw-r--   0 r         (1000) r         (1001)     4339 2024-04-17 14:47:16.054175 samples-filter-0.0.2/PKG-INFO
--rw-r--r--   0 r         (1000) r         (1001)     3636 2024-04-17 14:47:01.000000 samples-filter-0.0.2/README.md
-drwxrwxr-x   0 r         (1000) r         (1001)        0 2024-04-17 14:47:16.050175 samples-filter-0.0.2/objects/
--rw-r--r--   0 r         (1000) r         (1001)     1261 2024-04-17 14:47:01.000000 samples-filter-0.0.2/objects/__init__.py
--rw-r--r--   0 r         (1000) r         (1001)     1434 2024-04-17 14:47:01.000000 samples-filter-0.0.2/objects/__main__.py
--rw-r--r--   0 r         (1000) r         (1001)     2423 2024-04-17 14:47:01.000000 samples-filter-0.0.2/objects/cli.py
-drwxrwxr-x   0 r         (1000) r         (1001)        0 2024-04-17 14:47:16.054175 samples-filter-0.0.2/samples_filter.egg-info/
--rw-rw-r--   0 r         (1000) r         (1001)     4339 2024-04-17 14:47:15.000000 samples-filter-0.0.2/samples_filter.egg-info/PKG-INFO
--rw-rw-r--   0 r         (1000) r         (1001)      315 2024-04-17 14:47:16.000000 samples-filter-0.0.2/samples_filter.egg-info/SOURCES.txt
--rw-rw-r--   0 r         (1000) r         (1001)        1 2024-04-17 14:47:15.000000 samples-filter-0.0.2/samples_filter.egg-info/dependency_links.txt
--rw-rw-r--   0 r         (1000) r         (1001)       61 2024-04-17 14:47:15.000000 samples-filter-0.0.2/samples_filter.egg-info/entry_points.txt
--rw-rw-r--   0 r         (1000) r         (1001)        6 2024-04-17 14:47:15.000000 samples-filter-0.0.2/samples_filter.egg-info/requires.txt
--rw-rw-r--   0 r         (1000) r         (1001)        8 2024-04-17 14:47:15.000000 samples-filter-0.0.2/samples_filter.egg-info/top_level.txt
--rw-rw-r--   0 r         (1000) r         (1001)       38 2024-04-17 14:47:16.054175 samples-filter-0.0.2/setup.cfg
--rw-r--r--   0 r         (1000) r         (1001)     2524 2024-04-17 14:47:01.000000 samples-filter-0.0.2/setup.py
+drwxrwxr-x   0 r         (1000) r         (1001)        0 2024-04-17 15:05:09.125554 samples-filter-0.0.3/
+-rw-r--r--   0 r         (1000) r         (1001)     1087 2024-04-17 15:04:54.000000 samples-filter-0.0.3/LICENSE.txt
+-rw-rw-r--   0 r         (1000) r         (1001)     4339 2024-04-17 15:05:09.125554 samples-filter-0.0.3/PKG-INFO
+-rw-r--r--   0 r         (1000) r         (1001)     3636 2024-04-17 15:04:54.000000 samples-filter-0.0.3/README.md
+drwxrwxr-x   0 r         (1000) r         (1001)        0 2024-04-17 15:05:09.121554 samples-filter-0.0.3/objects/
+-rw-r--r--   0 r         (1000) r         (1001)     1261 2024-04-17 15:04:54.000000 samples-filter-0.0.3/objects/__init__.py
+-rw-r--r--   0 r         (1000) r         (1001)     1434 2024-04-17 15:04:54.000000 samples-filter-0.0.3/objects/__main__.py
+-rw-r--r--   0 r         (1000) r         (1001)     2423 2024-04-17 15:04:54.000000 samples-filter-0.0.3/objects/cli.py
+drwxrwxr-x   0 r         (1000) r         (1001)        0 2024-04-17 15:05:09.125554 samples-filter-0.0.3/samples_filter.egg-info/
+-rw-rw-r--   0 r         (1000) r         (1001)     4339 2024-04-17 15:05:09.000000 samples-filter-0.0.3/samples_filter.egg-info/PKG-INFO
+-rw-rw-r--   0 r         (1000) r         (1001)      315 2024-04-17 15:05:09.000000 samples-filter-0.0.3/samples_filter.egg-info/SOURCES.txt
+-rw-rw-r--   0 r         (1000) r         (1001)        1 2024-04-17 15:05:09.000000 samples-filter-0.0.3/samples_filter.egg-info/dependency_links.txt
+-rw-rw-r--   0 r         (1000) r         (1001)       58 2024-04-17 15:05:09.000000 samples-filter-0.0.3/samples_filter.egg-info/entry_points.txt
+-rw-rw-r--   0 r         (1000) r         (1001)        6 2024-04-17 15:05:09.000000 samples-filter-0.0.3/samples_filter.egg-info/requires.txt
+-rw-rw-r--   0 r         (1000) r         (1001)        8 2024-04-17 15:05:09.000000 samples-filter-0.0.3/samples_filter.egg-info/top_level.txt
+-rw-rw-r--   0 r         (1000) r         (1001)       38 2024-04-17 15:05:09.125554 samples-filter-0.0.3/setup.cfg
+-rw-r--r--   0 r         (1000) r         (1001)     2521 2024-04-17 15:04:54.000000 samples-filter-0.0.3/setup.py
```

### Comparing `samples-filter-0.0.2/LICENSE.txt` & `samples-filter-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `samples-filter-0.0.2/PKG-INFO` & `samples-filter-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samples-filter
-Version: 0.0.2
+Version: 0.0.3
 Summary: Command-line filter for GitHub repositories that contain "samples", instead of real project or framework or library
 Home-page: https://github.com/h1alexbel/samples-filter
 Author: Aliaksei Bialiauski
 Author-email: aliaksei.bialiauski@hey.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `samples-filter-0.0.2/README.md` & `samples-filter-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `samples-filter-0.0.2/objects/__init__.py` & `samples-filter-0.0.3/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `samples-filter-0.0.2/objects/__main__.py` & `samples-filter-0.0.3/objects/__main__.py`

 * *Files identical despite different names*

### Comparing `samples-filter-0.0.2/objects/cli.py` & `samples-filter-0.0.3/objects/cli.py`

 * *Files identical despite different names*

### Comparing `samples-filter-0.0.2/samples_filter.egg-info/PKG-INFO` & `samples-filter-0.0.3/samples_filter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samples-filter
-Version: 0.0.2
+Version: 0.0.3
 Summary: Command-line filter for GitHub repositories that contain "samples", instead of real project or framework or library
 Home-page: https://github.com/h1alexbel/samples-filter
 Author: Aliaksei Bialiauski
 Author-email: aliaksei.bialiauski@hey.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `samples-filter-0.0.2/setup.py` & `samples-filter-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     version=actual,
     packages=find_packages(),
     install_requires=[
         'typer'
     ],
     entry_points={
         'console_scripts': [
-            'samples-filter=objects.__main__.py:main',
+            'samples-filter=objects.__main__:main',
         ],
     },
     author='Aliaksei Bialiauski',
     author_email='aliaksei.bialiauski@hey.com',
     description=
     'Command-line filter for GitHub repositories that contain "samples",'
     ' instead of real project or framework or library',
```

