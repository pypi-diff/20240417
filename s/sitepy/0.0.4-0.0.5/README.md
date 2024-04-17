# Comparing `tmp/sitepy-0.0.4.tar.gz` & `tmp/sitepy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitepy-0.0.4.tar", last modified: Wed Apr 17 17:59:34 2024, max compression
+gzip compressed data, was "sitepy-0.0.5.tar", last modified: Wed Apr 17 18:22:20 2024, max compression
```

## Comparing `sitepy-0.0.4.tar` & `sitepy-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-17 17:59:34.310418 sitepy-0.0.4/
--rw-r--r--   0 lewis-family   (501) staff       (20)     1700 2024-04-17 17:59:34.309721 sitepy-0.0.4/PKG-INFO
--rw-r--r--   0 lewis-family   (501) staff       (20)       38 2024-04-17 17:59:34.310654 sitepy-0.0.4/setup.cfg
--rw-r--r--   0 lewis-family   (501) staff       (20)     1028 2024-04-17 17:59:26.000000 sitepy-0.0.4/setup.py
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-17 17:59:34.306907 sitepy-0.0.4/sitepy/
--rw-r--r--   0 lewis-family   (501) staff       (20)       30 2024-04-17 17:59:20.000000 sitepy-0.0.4/sitepy/__init__.py
--rw-r--r--   0 lewis-family   (501) staff       (20)     2784 2024-04-17 17:53:10.000000 sitepy-0.0.4/sitepy/sitepy.py
-drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-17 17:59:34.309148 sitepy-0.0.4/sitepy.egg-info/
--rw-r--r--   0 lewis-family   (501) staff       (20)     1700 2024-04-17 17:59:34.000000 sitepy-0.0.4/sitepy.egg-info/PKG-INFO
--rw-r--r--   0 lewis-family   (501) staff       (20)      164 2024-04-17 17:59:34.000000 sitepy-0.0.4/sitepy.egg-info/SOURCES.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-04-17 17:59:34.000000 sitepy-0.0.4/sitepy.egg-info/dependency_links.txt
--rw-r--r--   0 lewis-family   (501) staff       (20)        7 2024-04-17 17:59:34.000000 sitepy-0.0.4/sitepy.egg-info/top_level.txt
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-17 18:22:20.483252 sitepy-0.0.5/
+-rw-r--r--   0 lewis-family   (501) staff       (20)     1700 2024-04-17 18:22:20.482175 sitepy-0.0.5/PKG-INFO
+-rw-r--r--   0 lewis-family   (501) staff       (20)       38 2024-04-17 18:22:20.483464 sitepy-0.0.5/setup.cfg
+-rw-r--r--   0 lewis-family   (501) staff       (20)     1028 2024-04-17 18:22:13.000000 sitepy-0.0.5/setup.py
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-17 18:22:20.476530 sitepy-0.0.5/sitepy/
+-rw-r--r--   0 lewis-family   (501) staff       (20)       20 2024-04-17 18:22:03.000000 sitepy-0.0.5/sitepy/__init__.py
+-rw-r--r--   0 lewis-family   (501) staff       (20)     2784 2024-04-17 17:53:10.000000 sitepy-0.0.5/sitepy/sitepy.py
+drwxr-xr-x   0 lewis-family   (501) staff       (20)        0 2024-04-17 18:22:20.481250 sitepy-0.0.5/sitepy.egg-info/
+-rw-r--r--   0 lewis-family   (501) staff       (20)     1700 2024-04-17 18:22:20.000000 sitepy-0.0.5/sitepy.egg-info/PKG-INFO
+-rw-r--r--   0 lewis-family   (501) staff       (20)      164 2024-04-17 18:22:20.000000 sitepy-0.0.5/sitepy.egg-info/SOURCES.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)        1 2024-04-17 18:22:20.000000 sitepy-0.0.5/sitepy.egg-info/dependency_links.txt
+-rw-r--r--   0 lewis-family   (501) staff       (20)        7 2024-04-17 18:22:20.000000 sitepy-0.0.5/sitepy.egg-info/top_level.txt
```

### Comparing `sitepy-0.0.4/PKG-INFO` & `sitepy-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitepy
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple web framework.
 Home-page: https://github.com/WolfTheDeveloper/sitepy
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `sitepy-0.0.4/setup.py` & `sitepy-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sitepy',
-    version='0.0.4',
+    version='0.0.5',
     description='A simple web framework.',
     author='WolfTheDev',
     author_email='wolfthedev@gmail.com',
     url='https://github.com/WolfTheDeveloper/sitepy',
     packages=find_packages(),
     long_description=open('sitepy/README.md').read(),
     long_description_content_type='text/markdown',  # Add this line
```

### Comparing `sitepy-0.0.4/sitepy/sitepy.py` & `sitepy-0.0.5/sitepy/sitepy.py`

 * *Files identical despite different names*

### Comparing `sitepy-0.0.4/sitepy.egg-info/PKG-INFO` & `sitepy-0.0.5/sitepy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitepy
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple web framework.
 Home-page: https://github.com/WolfTheDeveloper/sitepy
 Author: WolfTheDev
 Author-email: wolfthedev@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

