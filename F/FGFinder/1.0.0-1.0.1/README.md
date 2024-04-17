# Comparing `tmp/fgfinder-1.tar.gz` & `tmp/fgfinder-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgfinder-1.tar", last modified: Fri Apr 12 19:05:22 2024, max compression
+gzip compressed data, was "fgfinder-1.0.1.tar", last modified: Wed Apr 17 17:02:28 2024, max compression
```

## Comparing `fgfinder-1.tar` & `fgfinder-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2024-04-12 19:05:22.958083 fgfinder-1/
-drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2024-04-12 19:05:22.958083 fgfinder-1/FGFinder/
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     2104 2024-04-12 19:02:02.000000 fgfinder-1/FGFinder/FGFinder.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       30 2024-04-12 18:17:16.000000 fgfinder-1/FGFinder/__init__.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        0 2024-04-12 18:17:16.000000 fgfinder-1/FGFinder/__main__.py
-drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2024-04-12 19:05:22.958083 fgfinder-1/FGFinder/data/
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     8014 2024-04-12 18:17:16.000000 fgfinder-1/FGFinder/data/fgsmarts.pkl
-drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2024-04-12 19:05:22.958083 fgfinder-1/FGFinder.egg-info/
--rw-r--r--   0 jefferson  (1000) jefferson  (1000)     1313 2024-04-12 19:05:22.000000 fgfinder-1/FGFinder.egg-info/PKG-INFO
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      297 2024-04-12 19:05:22.000000 fgfinder-1/FGFinder.egg-info/SOURCES.txt
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        1 2024-04-12 19:05:22.000000 fgfinder-1/FGFinder.egg-info/dependency_links.txt
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       34 2024-04-12 19:05:22.000000 fgfinder-1/FGFinder.egg-info/requires.txt
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        9 2024-04-12 19:05:22.000000 fgfinder-1/FGFinder.egg-info/top_level.txt
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1063 2024-04-12 17:59:22.000000 fgfinder-1/LICENSE
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       24 2024-04-12 19:02:02.000000 fgfinder-1/MANIFEST.in
--rw-r--r--   0 jefferson  (1000) jefferson  (1000)     1313 2024-04-12 19:05:22.958083 fgfinder-1/PKG-INFO
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      235 2024-04-12 18:21:15.000000 fgfinder-1/README.md
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       79 2024-04-12 19:05:22.958083 fgfinder-1/setup.cfg
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1213 2024-04-12 19:02:02.000000 fgfinder-1/setup.py
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2024-04-17 17:02:28.194971 fgfinder-1.0.1/
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2024-04-17 17:02:28.190971 fgfinder-1.0.1/FGFinder/
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     2153 2024-04-17 16:58:08.000000 fgfinder-1.0.1/FGFinder/FGFinder.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       30 2024-04-17 16:58:08.000000 fgfinder-1.0.1/FGFinder/__init__.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        0 2024-04-17 16:58:08.000000 fgfinder-1.0.1/FGFinder/__main__.py
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2024-04-17 17:02:28.194971 fgfinder-1.0.1/FGFinder/data/
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     8014 2024-04-17 16:58:08.000000 fgfinder-1.0.1/FGFinder/data/fgsmarts.pkl
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2024-04-17 17:02:28.194971 fgfinder-1.0.1/FGFinder.egg-info/
+-rw-r--r--   0 jefferson  (1000) jefferson  (1000)     1410 2024-04-17 17:02:28.000000 fgfinder-1.0.1/FGFinder.egg-info/PKG-INFO
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      297 2024-04-17 17:02:28.000000 fgfinder-1.0.1/FGFinder.egg-info/SOURCES.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        1 2024-04-17 17:02:28.000000 fgfinder-1.0.1/FGFinder.egg-info/dependency_links.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       34 2024-04-17 17:02:28.000000 fgfinder-1.0.1/FGFinder.egg-info/requires.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        9 2024-04-17 17:02:28.000000 fgfinder-1.0.1/FGFinder.egg-info/top_level.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1063 2024-04-12 17:59:22.000000 fgfinder-1.0.1/LICENSE
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       24 2024-04-17 16:58:08.000000 fgfinder-1.0.1/MANIFEST.in
+-rw-r--r--   0 jefferson  (1000) jefferson  (1000)     1410 2024-04-17 17:02:28.194971 fgfinder-1.0.1/PKG-INFO
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      332 2024-04-17 16:58:08.000000 fgfinder-1.0.1/README.md
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       79 2024-04-17 17:02:28.194971 fgfinder-1.0.1/setup.cfg
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1213 2024-04-17 17:01:09.000000 fgfinder-1.0.1/setup.py
```

### Comparing `fgfinder-1/FGFinder/FGFinder.py` & `fgfinder-1.0.1/FGFinder/FGFinder.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,14 +35,15 @@
             return freq
         except:
             return 0
 
     def __GetFreqs(self,smile):
         df_copy = self.df_fg[['Name']].copy()
         df_copy['Frequency'] = self.df_fg['SMARTS'].apply(lambda x: self.__testMatch(smile, x))
+        df_copy['SMARTS'] = self.df_fg['SMARTS']
         df_copy.rename(columns={'Name':'Functional Groups'}, inplace=True)
 
         return df_copy
 
     def findFunctionalGroups(self, smile):
         '''
         Pesquisa de grupos funcionais para um único smile
```

### Comparing `fgfinder-1/FGFinder/data/fgsmarts.pkl` & `fgfinder-1.0.1/FGFinder/data/fgsmarts.pkl`

 * *Files identical despite different names*

### Comparing `fgfinder-1/FGFinder.egg-info/PKG-INFO` & `fgfinder-1.0.1/FGFinder.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FGFinder
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package to identify functional groups in molecules.
 Home-page: https://github.com/Borest5543/Fg_Finder
 Author: Túlio Augusto and Jefferson Richard
 Author-email: borest5543@gmail.com
 License: MIT License
 Keywords: Cheminformatics RDKit Chemistry
 Classifier: Intended Audience :: Developers
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas<=2.2.2
 Requires-Dist: rdkit
 Requires-Dist: numpy<=1.26.4
 
+[![DOI](https://zenodo.org/badge/783865416.svg)](https://zenodo.org/doi/10.5281/zenodo.10966985)
 # FG Finder
 A python package to identfy functional groups in molecules.
 
 # How to install
 ### Pip
 ```
 pip install FGFinder
```

### Comparing `fgfinder-1/LICENSE` & `fgfinder-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fgfinder-1/PKG-INFO` & `fgfinder-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FGFinder
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package to identify functional groups in molecules.
 Home-page: https://github.com/Borest5543/Fg_Finder
 Author: Túlio Augusto and Jefferson Richard
 Author-email: borest5543@gmail.com
 License: MIT License
 Keywords: Cheminformatics RDKit Chemistry
 Classifier: Intended Audience :: Developers
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas<=2.2.2
 Requires-Dist: rdkit
 Requires-Dist: numpy<=1.26.4
 
+[![DOI](https://zenodo.org/badge/783865416.svg)](https://zenodo.org/doi/10.5281/zenodo.10966985)
 # FG Finder
 A python package to identfy functional groups in molecules.
 
 # How to install
 ### Pip
 ```
 pip install FGFinder
```

### Comparing `fgfinder-1/setup.py` & `fgfinder-1.0.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", 'r') as fr:
 	description = fr.read()
 
 setup(
     name='FGFinder',
-    version='1.0.0',
+    version='1.0.1',
     url='https://github.com/Borest5543/Fg_Finder',
     license='MIT License',
     author='Túlio Augusto and Jefferson Richard',
     author_email='borest5543@gmail.com',
     keywords='Cheminformatics RDKit Chemistry',
     description='A package to identify functional groups in molecules.',
     long_description = description,
```

