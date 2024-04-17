# Comparing `tmp/ptcr-0.1.5.tar.gz` & `tmp/ptcr-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptcr-0.1.5.tar", last modified: Wed Apr 17 02:51:25 2024, max compression
+gzip compressed data, was "ptcr-0.1.6.tar", last modified: Wed Apr 17 02:53:18 2024, max compression
```

## Comparing `ptcr-0.1.5.tar` & `ptcr-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 02:51:25.654745 ptcr-0.1.5/
--rw-rw-rw-   0        0        0     1069 2024-04-16 23:53:12.000000 ptcr-0.1.5/LICENSE
--rw-rw-rw-   0        0        0    11205 2024-04-17 02:51:25.654745 ptcr-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0    10639 2024-04-17 02:44:06.000000 ptcr-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 02:51:25.645162 ptcr-0.1.5/ptcr.egg-info/
--rw-rw-rw-   0        0        0    11205 2024-04-17 02:51:25.000000 ptcr-0.1.5/ptcr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2024-04-17 02:51:25.000000 ptcr-0.1.5/ptcr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 02:51:25.000000 ptcr-0.1.5/ptcr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      167 2024-04-17 02:51:25.000000 ptcr-0.1.5/ptcr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-17 02:51:25.000000 ptcr-0.1.5/ptcr.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-17 02:51:25.652725 ptcr-0.1.5/ptcr2/
--rw-rw-rw-   0        0        0        0 2024-02-23 22:22:15.000000 ptcr-0.1.5/ptcr2/__init__.py
--rw-rw-rw-   0        0        0     7664 2024-03-06 16:01:26.000000 ptcr-0.1.5/ptcr2/automata_utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-16 13:50:12.000000 ptcr-0.1.5/ptcr2/base_model.py
--rw-rw-rw-   0        0        0     3364 2024-04-07 16:47:54.000000 ptcr-0.1.5/ptcr2/belief_tree.py
--rw-rw-rw-   0        0        0    27773 2024-04-16 23:22:39.000000 ptcr-0.1.5/ptcr2/event_predictor.py
--rw-rw-rw-   0        0        0    10168 2024-04-07 21:33:36.000000 ptcr-0.1.5/ptcr2/fom.py
--rw-rw-rw-   0        0        0     9897 2024-04-07 16:36:30.000000 ptcr-0.1.5/ptcr2/markov_chain.py
--rw-rw-rw-   0        0        0    75894 2024-04-07 21:39:01.000000 ptcr-0.1.5/ptcr2/markov_decision_process.py
--rw-rw-rw-   0        0        0       42 2024-04-17 02:51:25.654745 ptcr-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1022 2024-04-17 02:51:24.000000 ptcr-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 02:53:18.835877 ptcr-0.1.6/
+-rw-rw-rw-   0        0        0     1069 2024-04-16 23:53:12.000000 ptcr-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0    11205 2024-04-17 02:53:18.834371 ptcr-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0    10639 2024-04-17 02:44:06.000000 ptcr-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 02:53:18.825841 ptcr-0.1.6/ptcr.egg-info/
+-rw-rw-rw-   0        0        0    11205 2024-04-17 02:53:18.000000 ptcr-0.1.6/ptcr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2024-04-17 02:53:18.000000 ptcr-0.1.6/ptcr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 02:53:18.000000 ptcr-0.1.6/ptcr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      167 2024-04-17 02:53:18.000000 ptcr-0.1.6/ptcr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-17 02:53:18.000000 ptcr-0.1.6/ptcr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 02:53:18.833360 ptcr-0.1.6/ptcr2/
+-rw-rw-rw-   0        0        0        0 2024-02-23 22:22:15.000000 ptcr-0.1.6/ptcr2/__init__.py
+-rw-rw-rw-   0        0        0     7664 2024-03-06 16:01:26.000000 ptcr-0.1.6/ptcr2/automata_utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-16 13:50:12.000000 ptcr-0.1.6/ptcr2/base_model.py
+-rw-rw-rw-   0        0        0     3364 2024-04-07 16:47:54.000000 ptcr-0.1.6/ptcr2/belief_tree.py
+-rw-rw-rw-   0        0        0    27773 2024-04-16 23:22:39.000000 ptcr-0.1.6/ptcr2/event_predictor.py
+-rw-rw-rw-   0        0        0    10168 2024-04-07 21:33:36.000000 ptcr-0.1.6/ptcr2/fom.py
+-rw-rw-rw-   0        0        0     9897 2024-04-07 16:36:30.000000 ptcr-0.1.6/ptcr2/markov_chain.py
+-rw-rw-rw-   0        0        0    75894 2024-04-07 21:39:01.000000 ptcr-0.1.6/ptcr2/markov_decision_process.py
+-rw-rw-rw-   0        0        0       42 2024-04-17 02:53:18.835877 ptcr-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1022 2024-04-17 02:53:17.000000 ptcr-0.1.6/setup.py
```

### Comparing `ptcr-0.1.5/LICENSE` & `ptcr-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ptcr-0.1.5/PKG-INFO` & `ptcr-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptcr
-Version: 0.1.5
+Version: 0.1.6
 Summary: Constructs and simulates PTCR models.
 Home-page: https://github.com/T-Lind/ptcr
 Author: Tiernan Lindauer
 Author-email: tiernanlind@tamu.edu
 License: MIT
 Keywords: PTCR,FOM,simulation,optimization,decision making,models
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ptcr-0.1.5/README.md` & `ptcr-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ptcr-0.1.5/ptcr.egg-info/PKG-INFO` & `ptcr-0.1.6/ptcr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptcr
-Version: 0.1.5
+Version: 0.1.6
 Summary: Constructs and simulates PTCR models.
 Home-page: https://github.com/T-Lind/ptcr
 Author: Tiernan Lindauer
 Author-email: tiernanlind@tamu.edu
 License: MIT
 Keywords: PTCR,FOM,simulation,optimization,decision making,models
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ptcr-0.1.5/ptcr2/automata_utility.py` & `ptcr-0.1.6/ptcr2/automata_utility.py`

 * *Files identical despite different names*

### Comparing `ptcr-0.1.5/ptcr2/base_model.py` & `ptcr-0.1.6/ptcr2/base_model.py`

 * *Files identical despite different names*

### Comparing `ptcr-0.1.5/ptcr2/belief_tree.py` & `ptcr-0.1.6/ptcr2/belief_tree.py`

 * *Files identical despite different names*

### Comparing `ptcr-0.1.5/ptcr2/event_predictor.py` & `ptcr-0.1.6/ptcr2/event_predictor.py`

 * *Files identical despite different names*

### Comparing `ptcr-0.1.5/ptcr2/fom.py` & `ptcr-0.1.6/ptcr2/fom.py`

 * *Files identical despite different names*

### Comparing `ptcr-0.1.5/ptcr2/markov_chain.py` & `ptcr-0.1.6/ptcr2/markov_chain.py`

 * *Files identical despite different names*

### Comparing `ptcr-0.1.5/ptcr2/markov_decision_process.py` & `ptcr-0.1.6/ptcr2/markov_decision_process.py`

 * *Files identical despite different names*

### Comparing `ptcr-0.1.5/setup.py` & `ptcr-0.1.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ptcr',
-    version='0.1.5',
+    version='0.1.6',
     author='Tiernan Lindauer',
     author_email='tiernanlind@tamu.edu',
     description='Constructs and simulates PTCR models.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     install_requires=[
         'automata-lib==4.0.0',
         'cached-method==0.1.0',
-        'frozendict==2.0.0',
-        'mpmath==1.0.0',
-        'networkx==2.6.1',
+        'frozendict==2.4.0',
+        'mpmath==1.3.0',
+        'networkx==3.2.1',
         'numpy==1.26.4',
         'sympy==1.12',
         'scipy==1.13.0',
-        'typing-extensions==4.0.0',
+        'typing-extensions==4.9.0',
         'tqdm==4.66.2'
     ],
     python_requires='==3.9',
     url='https://github.com/T-Lind/ptcr',
     license='MIT',
     keywords='PTCR, FOM, simulation, optimization, decision making, models'
 )
```

