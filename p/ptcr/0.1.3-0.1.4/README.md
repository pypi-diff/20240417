# Comparing `tmp/ptcr-0.1.3.tar.gz` & `tmp/ptcr-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptcr-0.1.3.tar", last modified: Wed Apr 17 02:44:28 2024, max compression
+gzip compressed data, was "ptcr-0.1.4.tar", last modified: Wed Apr 17 02:47:52 2024, max compression
```

## Comparing `ptcr-0.1.3.tar` & `ptcr-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 02:44:28.082069 ptcr-0.1.3/
--rw-rw-rw-   0        0        0     1069 2024-04-16 23:53:12.000000 ptcr-0.1.3/LICENSE
--rw-rw-rw-   0        0        0    11205 2024-04-17 02:44:28.082069 ptcr-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0    10639 2024-04-17 02:44:06.000000 ptcr-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 02:44:28.081059 ptcr-0.1.3/ptcr.egg-info/
--rw-rw-rw-   0        0        0    11205 2024-04-17 02:44:28.000000 ptcr-0.1.3/ptcr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      138 2024-04-17 02:44:28.000000 ptcr-0.1.3/ptcr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 02:44:28.000000 ptcr-0.1.3/ptcr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 02:44:28.000000 ptcr-0.1.3/ptcr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 02:44:28.083063 ptcr-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      704 2024-04-17 02:44:24.000000 ptcr-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 02:47:52.356341 ptcr-0.1.4/
+-rw-rw-rw-   0        0        0     1069 2024-04-16 23:53:12.000000 ptcr-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0    11205 2024-04-17 02:47:52.355345 ptcr-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0    10639 2024-04-17 02:44:06.000000 ptcr-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 02:47:52.346224 ptcr-0.1.4/ptcr.egg-info/
+-rw-rw-rw-   0        0        0    11205 2024-04-17 02:47:52.000000 ptcr-0.1.4/ptcr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2024-04-17 02:47:52.000000 ptcr-0.1.4/ptcr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 02:47:52.000000 ptcr-0.1.4/ptcr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-17 02:47:52.000000 ptcr-0.1.4/ptcr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 02:47:52.354334 ptcr-0.1.4/ptcr2/
+-rw-rw-rw-   0        0        0        0 2024-02-23 22:22:15.000000 ptcr-0.1.4/ptcr2/__init__.py
+-rw-rw-rw-   0        0        0     7664 2024-03-06 16:01:26.000000 ptcr-0.1.4/ptcr2/automata_utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-16 13:50:12.000000 ptcr-0.1.4/ptcr2/base_model.py
+-rw-rw-rw-   0        0        0     3364 2024-04-07 16:47:54.000000 ptcr-0.1.4/ptcr2/belief_tree.py
+-rw-rw-rw-   0        0        0    27773 2024-04-16 23:22:39.000000 ptcr-0.1.4/ptcr2/event_predictor.py
+-rw-rw-rw-   0        0        0    10168 2024-04-07 21:33:36.000000 ptcr-0.1.4/ptcr2/fom.py
+-rw-rw-rw-   0        0        0     9897 2024-04-07 16:36:30.000000 ptcr-0.1.4/ptcr2/markov_chain.py
+-rw-rw-rw-   0        0        0    75894 2024-04-07 21:39:01.000000 ptcr-0.1.4/ptcr2/markov_decision_process.py
+-rw-rw-rw-   0        0        0       42 2024-04-17 02:47:52.356341 ptcr-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      704 2024-04-17 02:47:35.000000 ptcr-0.1.4/setup.py
```

### Comparing `ptcr-0.1.3/LICENSE` & `ptcr-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ptcr-0.1.3/PKG-INFO` & `ptcr-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptcr
-Version: 0.1.3
+Version: 0.1.4
 Summary: Constructs and simulates PTCR models.
 Home-page: https://github.com/T-Lind/ptcr
 Author: Tiernan Lindauer
 Author-email: tiernanlind@tamu.edu
 License: MIT
 Keywords: PTCR,FOM,simulation,optimization,decision making,models
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ptcr-0.1.3/README.md` & `ptcr-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ptcr-0.1.3/ptcr.egg-info/PKG-INFO` & `ptcr-0.1.4/ptcr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptcr
-Version: 0.1.3
+Version: 0.1.4
 Summary: Constructs and simulates PTCR models.
 Home-page: https://github.com/T-Lind/ptcr
 Author: Tiernan Lindauer
 Author-email: tiernanlind@tamu.edu
 License: MIT
 Keywords: PTCR,FOM,simulation,optimization,decision making,models
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ptcr-0.1.3/setup.py` & `ptcr-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ptcr',
-    version='0.1.3',
+    version='0.1.4',
     author='Tiernan Lindauer',
     author_email='tiernanlind@tamu.edu',
     description='Constructs and simulates PTCR models.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     classifiers=[
```

