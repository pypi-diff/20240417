# Comparing `tmp/ptcr-0.1.2.tar.gz` & `tmp/ptcr-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptcr-0.1.2.tar", last modified: Wed Apr 17 02:39:01 2024, max compression
+gzip compressed data, was "ptcr-0.1.3.tar", last modified: Wed Apr 17 02:44:28 2024, max compression
```

## Comparing `ptcr-0.1.2.tar` & `ptcr-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 02:39:01.566275 ptcr-0.1.2/
--rw-rw-rw-   0        0        0     1069 2024-04-16 23:53:12.000000 ptcr-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     5889 2024-04-17 02:39:01.566275 ptcr-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     5323 2024-04-16 23:55:11.000000 ptcr-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 02:39:01.565099 ptcr-0.1.2/ptcr.egg-info/
--rw-rw-rw-   0        0        0     5889 2024-04-17 02:39:01.000000 ptcr-0.1.2/ptcr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      138 2024-04-17 02:39:01.000000 ptcr-0.1.2/ptcr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 02:39:01.000000 ptcr-0.1.2/ptcr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 02:39:01.000000 ptcr-0.1.2/ptcr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 02:39:01.567281 ptcr-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      704 2024-04-17 02:38:59.000000 ptcr-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 02:44:28.082069 ptcr-0.1.3/
+-rw-rw-rw-   0        0        0     1069 2024-04-16 23:53:12.000000 ptcr-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0    11205 2024-04-17 02:44:28.082069 ptcr-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    10639 2024-04-17 02:44:06.000000 ptcr-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 02:44:28.081059 ptcr-0.1.3/ptcr.egg-info/
+-rw-rw-rw-   0        0        0    11205 2024-04-17 02:44:28.000000 ptcr-0.1.3/ptcr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      138 2024-04-17 02:44:28.000000 ptcr-0.1.3/ptcr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 02:44:28.000000 ptcr-0.1.3/ptcr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 02:44:28.000000 ptcr-0.1.3/ptcr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 02:44:28.083063 ptcr-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      704 2024-04-17 02:44:24.000000 ptcr-0.1.3/setup.py
```

### Comparing `ptcr-0.1.2/LICENSE` & `ptcr-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ptcr-0.1.2/setup.py` & `ptcr-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ptcr',
-    version='0.1.2',
+    version='0.1.3',
     author='Tiernan Lindauer',
     author_email='tiernanlind@tamu.edu',
     description='Constructs and simulates PTCR models.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     classifiers=[
```

