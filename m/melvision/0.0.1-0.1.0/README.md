# Comparing `tmp/melvision-0.0.1.tar.gz` & `tmp/melvision-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melvision-0.0.1.tar", last modified: Wed Apr 17 13:56:37 2024, max compression
+gzip compressed data, was "melvision-0.1.0.tar", last modified: Wed Apr 17 14:37:34 2024, max compression
```

## Comparing `melvision-0.0.1.tar` & `melvision-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 13:56:37.431333 melvision-0.0.1/
--rw-rw-rw-   0        0        0      417 2024-04-17 13:56:37.431333 melvision-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-17 13:56:37.431333 melvision-0.0.1/melvision/
--rw-rw-rw-   0        0        0        0 2024-04-17 13:38:27.000000 melvision-0.0.1/melvision/__init__.py
--rw-rw-rw-   0        0        0     1926 2024-04-17 13:41:41.000000 melvision-0.0.1/melvision/alexnet.py
--rw-rw-rw-   0        0        0     6004 2024-04-17 13:41:41.000000 melvision-0.0.1/melvision/googlenet.py
--rw-rw-rw-   0        0        0     8762 2024-04-17 13:41:41.000000 melvision-0.0.1/melvision/resnet.py
--rw-rw-rw-   0        0        0     5443 2024-04-17 13:41:41.000000 melvision-0.0.1/melvision/vgg.py
-drwxrwxrwx   0        0        0        0 2024-04-17 13:56:37.431333 melvision-0.0.1/melvision.egg-info/
--rw-rw-rw-   0        0        0      417 2024-04-17 13:56:37.000000 melvision-0.0.1/melvision.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2024-04-17 13:56:37.000000 melvision-0.0.1/melvision.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 13:56:37.000000 melvision-0.0.1/melvision.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-17 13:56:37.000000 melvision-0.0.1/melvision.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 13:56:37.431333 melvision-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      546 2024-04-17 13:55:58.000000 melvision-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 14:37:34.213792 melvision-0.1.0/
+-rw-rw-rw-   0        0        0      426 2024-04-17 14:37:34.213792 melvision-0.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-17 14:37:34.213792 melvision-0.1.0/melvision/
+-rw-rw-rw-   0        0        0        0 2024-04-17 13:38:27.000000 melvision-0.1.0/melvision/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 14:37:34.213792 melvision-0.1.0/melvision/models/
+-rw-rw-rw-   0        0        0        0 2024-04-17 14:19:41.000000 melvision-0.1.0/melvision/models/__init__.py
+-rw-rw-rw-   0        0        0     1926 2024-04-17 13:41:41.000000 melvision-0.1.0/melvision/models/alexnet.py
+-rw-rw-rw-   0        0        0     6004 2024-04-17 13:41:41.000000 melvision-0.1.0/melvision/models/googlenet.py
+-rw-rw-rw-   0        0        0     8762 2024-04-17 13:41:41.000000 melvision-0.1.0/melvision/models/resnet.py
+-rw-rw-rw-   0        0        0     5443 2024-04-17 13:41:41.000000 melvision-0.1.0/melvision/models/vgg.py
+-rw-rw-rw-   0        0        0      522 2024-04-17 14:22:12.000000 melvision-0.1.0/melvision/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-17 14:37:34.213792 melvision-0.1.0/melvision.egg-info/
+-rw-rw-rw-   0        0        0      426 2024-04-17 14:37:34.000000 melvision-0.1.0/melvision.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2024-04-17 14:37:34.000000 melvision-0.1.0/melvision.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 14:37:34.000000 melvision-0.1.0/melvision.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-17 14:37:34.000000 melvision-0.1.0/melvision.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 14:37:34.213792 melvision-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      555 2024-04-17 14:30:08.000000 melvision-0.1.0/setup.py
```

### Comparing `melvision-0.0.1/melvision/alexnet.py` & `melvision-0.1.0/melvision/models/alexnet.py`

 * *Files identical despite different names*

### Comparing `melvision-0.0.1/melvision/googlenet.py` & `melvision-0.1.0/melvision/models/googlenet.py`

 * *Files identical despite different names*

### Comparing `melvision-0.0.1/melvision/resnet.py` & `melvision-0.1.0/melvision/models/resnet.py`

 * *Files identical despite different names*

### Comparing `melvision-0.0.1/melvision/vgg.py` & `melvision-0.1.0/melvision/models/vgg.py`

 * *Files identical despite different names*

### Comparing `melvision-0.0.1/setup.py` & `melvision-0.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 setuptools.setup(
     name="melvision",
-    version="0.0.1",
+    version="0.1.0",
     author="Melvin Hwang",
     author_email="huang667399@gmail.com",
-    description="A lightweight third-party deep learning library",
+    description="A convenient deep learning and image processing library.",
     long_description_content_type="text/markdown",
     url="https://github.com/Manuel667399/melvision",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

