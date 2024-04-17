# Comparing `tmp/ptcr-0.1.1.tar.gz` & `tmp/ptcr-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptcr-0.1.1.tar", last modified: Wed Apr 17 02:34:04 2024, max compression
+gzip compressed data, was "ptcr-0.1.2.tar", last modified: Wed Apr 17 02:39:01 2024, max compression
```

## Comparing `ptcr-0.1.1.tar` & `ptcr-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 02:34:04.650390 ptcr-0.1.1/
--rw-rw-rw-   0        0        0     1069 2024-04-16 23:53:12.000000 ptcr-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     5724 2024-04-17 02:34:04.650390 ptcr-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5323 2024-04-16 23:55:11.000000 ptcr-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 02:34:04.649391 ptcr-0.1.1/ptcr.egg-info/
--rw-rw-rw-   0        0        0     5724 2024-04-17 02:34:04.000000 ptcr-0.1.1/ptcr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      138 2024-04-17 02:34:04.000000 ptcr-0.1.1/ptcr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 02:34:04.000000 ptcr-0.1.1/ptcr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 02:34:04.000000 ptcr-0.1.1/ptcr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 02:34:04.650390 ptcr-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      512 2024-04-17 02:34:00.000000 ptcr-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 02:39:01.566275 ptcr-0.1.2/
+-rw-rw-rw-   0        0        0     1069 2024-04-16 23:53:12.000000 ptcr-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     5889 2024-04-17 02:39:01.566275 ptcr-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5323 2024-04-16 23:55:11.000000 ptcr-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 02:39:01.565099 ptcr-0.1.2/ptcr.egg-info/
+-rw-rw-rw-   0        0        0     5889 2024-04-17 02:39:01.000000 ptcr-0.1.2/ptcr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      138 2024-04-17 02:39:01.000000 ptcr-0.1.2/ptcr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 02:39:01.000000 ptcr-0.1.2/ptcr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 02:39:01.000000 ptcr-0.1.2/ptcr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 02:39:01.567281 ptcr-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      704 2024-04-17 02:38:59.000000 ptcr-0.1.2/setup.py
```

### Comparing `ptcr-0.1.1/LICENSE` & `ptcr-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ptcr-0.1.1/PKG-INFO` & `ptcr-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: ptcr
-Version: 0.1.1
+Version: 0.1.2
 Summary: Constructs and simulates PTCR models.
+Home-page: https://github.com/T-Lind/ptcr
 Author: Tiernan Lindauer
 Author-email: tiernanlind@tamu.edu
+License: MIT
+Keywords: PTCR,FOM,simulation,optimization,decision making,models
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: ==3.9
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Exploring Alternative Cost Mechanisms for Probabilistic Planning
 
 ### Author: T-Lind
 
 ## Overview
```

### Comparing `ptcr-0.1.1/README.md` & `ptcr-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ptcr-0.1.1/ptcr.egg-info/PKG-INFO` & `ptcr-0.1.2/ptcr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: ptcr
-Version: 0.1.1
+Version: 0.1.2
 Summary: Constructs and simulates PTCR models.
+Home-page: https://github.com/T-Lind/ptcr
 Author: Tiernan Lindauer
 Author-email: tiernanlind@tamu.edu
+License: MIT
+Keywords: PTCR,FOM,simulation,optimization,decision making,models
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: ==3.9
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Exploring Alternative Cost Mechanisms for Probabilistic Planning
 
 ### Author: T-Lind
 
 ## Overview
```

### Comparing `ptcr-0.1.1/setup.py` & `ptcr-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ptcr',
-    version='0.1.1',
+    version='0.1.2',
     author='Tiernan Lindauer',
     author_email='tiernanlind@tamu.edu',
     description='Constructs and simulates PTCR models.',
     long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='==3.9',
+    url='https://github.com/T-Lind/ptcr',
+    license='MIT',
+    keywords='PTCR, FOM, simulation, optimization, decision making, models'
 )
```

