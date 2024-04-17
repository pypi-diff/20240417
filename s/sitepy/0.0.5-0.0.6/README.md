# Comparing `tmp/sitepy-0.0.5.tar.gz` & `tmp/sitepy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitepy-0.0.5.tar", last modified: Wed Apr 17 18:22:20 2024, max compression
+gzip compressed data, was "sitepy-0.0.6.tar", last modified: Wed Apr 17 18:27:54 2024, max compression
```

## Comparing `sitepy-0.0.5.tar` & `sitepy-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-17 18:22:20.483252 sitepy-0.0.5/
--rw-r--r--   0 lewis-family   (501) staff       (20)     1700 2024-04-17 18:22:20.482175 sitepy-0.0.5/PKG-INFO
--rw-r--r--   0 lewis-family   (501) staff       (20)       38 2024-04-17 18:22:20.483464 sitepy-0.0.5/setup.cfg
--rw-r--r--   0 lewis-family   (501) staff       (20)     1028 2024-04-17 18:22:13.000000 sitepy-0.0.5/setup.py
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-17 18:22:20.476530 sitepy-0.0.5/sitepy/
--rw-r--r--   0 lewis-family   (501) staff       (20)       20 2024-04-17 18:22:03.000000 sitepy-0.0.5/sitepy/__init__.py
--rw-r--r--   0 lewis-family   (501) staff       (20)     2784 2024-04-17 17:53:10.000000 sitepy-0.0.5/sitepy/sitepy.py
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-17 18:22:20.481250 sitepy-0.0.5/sitepy.egg-info/
--rw-r--r--   0 lewis-family   (501) staff       (20)     1700 2024-04-17 18:22:20.000000 sitepy-0.0.5/sitepy.egg-info/PKG-INFO
--rw-r--r--   0 lewis-family   (501) staff       (20)      164 2024-04-17 18:22:20.000000 sitepy-0.0.5/sitepy.egg-info/SOURCES.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-04-17 18:22:20.000000 sitepy-0.0.5/sitepy.egg-info/dependency_links.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)        7 2024-04-17 18:22:20.000000 sitepy-0.0.5/sitepy.egg-info/top_level.txt
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-17 18:27:54.047955 sitepy-0.0.6/
+-rw-r--r--   0 lewis-family   (501) staff       (20)     1700 2024-04-17 18:27:54.046828 sitepy-0.0.6/PKG-INFO
+-rw-r--r--   0 lewis-family   (501) staff       (20)       38 2024-04-17 18:27:54.048133 sitepy-0.0.6/setup.cfg
+-rw-r--r--   0 lewis-family   (501) staff       (20)     1028 2024-04-17 18:27:47.000000 sitepy-0.0.6/setup.py
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-17 18:27:54.037191 sitepy-0.0.6/sitepy/
+-rw-r--r--   0 lewis-family   (501) staff       (20)       24 2024-04-17 18:27:23.000000 sitepy-0.0.6/sitepy/__init__.py
+-rw-r--r--   0 lewis-family   (501) staff       (20)     2784 2024-04-17 17:53:10.000000 sitepy-0.0.6/sitepy/core.py
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-17 18:27:54.045783 sitepy-0.0.6/sitepy.egg-info/
+-rw-r--r--   0 lewis-family   (501) staff       (20)     1700 2024-04-17 18:27:53.000000 sitepy-0.0.6/sitepy.egg-info/PKG-INFO
+-rw-r--r--   0 lewis-family   (501) staff       (20)      162 2024-04-17 18:27:53.000000 sitepy-0.0.6/sitepy.egg-info/SOURCES.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-04-17 18:27:53.000000 sitepy-0.0.6/sitepy.egg-info/dependency_links.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)        7 2024-04-17 18:27:53.000000 sitepy-0.0.6/sitepy.egg-info/top_level.txt
```

### Comparing `sitepy-0.0.5/PKG-INFO` & `sitepy-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitepy
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simple web framework.
 Home-page: https://github.com/WolfTheDeveloper/sitepy
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `sitepy-0.0.5/setup.py` & `sitepy-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sitepy',
-    version='0.0.5',
+    version='0.0.6',
     description='A simple web framework.',
     author='WolfTheDev',
     author_email='wolfthedev@gmail.com',
     url='https://github.com/WolfTheDeveloper/sitepy',
     packages=find_packages(),
     long_description=open('sitepy/README.md').read(),
     long_description_content_type='text/markdown',  # Add this line
```

### Comparing `sitepy-0.0.5/sitepy/sitepy.py` & `sitepy-0.0.6/sitepy/core.py`

 * *Files identical despite different names*

### Comparing `sitepy-0.0.5/sitepy.egg-info/PKG-INFO` & `sitepy-0.0.6/sitepy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitepy
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simple web framework.
 Home-page: https://github.com/WolfTheDeveloper/sitepy
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

