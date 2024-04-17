# Comparing `tmp/simplace-5.0.5.tar.gz` & `tmp/simplace-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplace-5.0.5.tar", last modified: Wed Jun 28 22:10:06 2023, max compression
+gzip compressed data, was "simplace-5.1.0.tar", last modified: Wed Apr 17 14:40:53 2024, max compression
```

## Comparing `simplace-5.0.5.tar` & `simplace-5.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 22:10:06.517146 simplace-5.0.5/
--rw-rw-rw-   0        0        0     3689 2023-06-28 22:09:37.000000 simplace-5.0.5/CHANGELOG.rst
--rw-rw-rw-   0        0        0    35141 2017-07-20 15:04:53.000000 simplace-5.0.5/LICENSE
--rw-rw-rw-   0        0        0       41 2016-11-17 17:32:58.000000 simplace-5.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1293 2023-06-28 22:10:06.516155 simplace-5.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      743 2022-04-19 11:42:59.000000 simplace-5.0.5/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-28 22:10:06.517146 simplace-5.0.5/setup.cfg
--rw-rw-rw-   0        0        0      995 2021-11-25 08:32:20.000000 simplace-5.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-28 22:10:06.491162 simplace-5.0.5/simplace/
--rw-rw-rw-   0        0        0     6267 2023-03-01 12:31:13.000000 simplace-5.0.5/simplace/SimplaceClasses.py
--rw-rw-rw-   0        0        0      125 2016-11-17 17:32:58.000000 simplace-5.0.5/simplace/__init__.py
--rw-rw-rw-   0        0        0       77 2023-06-28 22:08:41.000000 simplace-5.0.5/simplace/_version.py
--rw-rw-rw-   0        0        0    23951 2023-06-28 22:06:24.000000 simplace-5.0.5/simplace/simplace.py
-drwxrwxrwx   0        0        0        0 2023-06-28 22:10:06.511156 simplace-5.0.5/simplace.egg-info/
--rw-rw-rw-   0        0        0     1293 2023-06-28 22:10:06.000000 simplace-5.0.5/simplace.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      334 2023-06-28 22:10:06.000000 simplace-5.0.5/simplace.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 22:10:06.000000 simplace-5.0.5/simplace.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-11-24 10:54:28.000000 simplace-5.0.5/simplace.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-06-28 22:10:06.000000 simplace-5.0.5/simplace.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-28 22:10:06.000000 simplace-5.0.5/simplace.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 14:40:53.667788 simplace-5.1.0/
+-rw-rw-rw-   0        0        0     3836 2024-04-17 14:36:38.000000 simplace-5.1.0/CHANGELOG.rst
+-rw-rw-rw-   0        0        0    35141 2017-07-20 15:04:53.000000 simplace-5.1.0/LICENSE
+-rw-rw-rw-   0        0        0       41 2016-11-17 17:32:58.000000 simplace-5.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1315 2024-04-17 14:40:53.665793 simplace-5.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      743 2022-04-19 11:42:59.000000 simplace-5.1.0/README.rst
+-rw-rw-rw-   0        0        0       42 2024-04-17 14:40:53.667788 simplace-5.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      995 2021-11-25 08:32:20.000000 simplace-5.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 14:40:53.648067 simplace-5.1.0/simplace/
+-rw-rw-rw-   0        0        0     6269 2024-04-17 14:26:27.000000 simplace-5.1.0/simplace/SimplaceClasses.py
+-rw-rw-rw-   0        0        0      125 2016-11-17 17:32:58.000000 simplace-5.1.0/simplace/__init__.py
+-rw-rw-rw-   0        0        0       77 2024-04-17 14:34:35.000000 simplace-5.1.0/simplace/_version.py
+-rw-rw-rw-   0        0        0    23951 2023-06-28 22:06:24.000000 simplace-5.1.0/simplace/simplace.py
+drwxrwxrwx   0        0        0        0 2024-04-17 14:40:53.664786 simplace-5.1.0/simplace.egg-info/
+-rw-rw-rw-   0        0        0     1315 2024-04-17 14:40:53.000000 simplace-5.1.0/simplace.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      334 2024-04-17 14:40:53.000000 simplace-5.1.0/simplace.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 14:40:53.000000 simplace-5.1.0/simplace.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-11-24 10:54:28.000000 simplace-5.1.0/simplace.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2024-04-17 14:40:53.000000 simplace-5.1.0/simplace.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-17 14:40:53.000000 simplace-5.1.0/simplace.egg-info/top_level.txt
```

### Comparing `simplace-5.0.5/CHANGELOG.rst` & `simplace-5.1.0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+Version 5.1.0
+~~~~~~~~~~~~~
+* compatible with Simplace 5.1
+* fix initialisation of object oriented version when no java parmeters were given
+
 Version 5.0.5
 ~~~~~~~~~~~~~
 * additional java parameters as list or as string (one parameter)
 
 Version 5.0.4
 ~~~~~~~~~~~~~
 * Bugfix to allow more than one additional java parameter
```

### Comparing `simplace-5.0.5/LICENSE` & `simplace-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simplace-5.0.5/PKG-INFO` & `simplace-5.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: simplace
-Version: 5.0.5
+Version: 5.1.0
 Summary: Interact with the simulation framework Simplace
 Home-page: https://www.simplace.net/
 Author: Gunther Krauss
 Author-email: guntherkrauss@uni-bonn.de
 License: GPL3
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Java
 License-File: LICENSE
+Requires-Dist: Jpype1
+Requires-Dist: numpy
 
 See the documentation at https://simplace.readthedocs.io/
 
 Run and control simulations in the simulation framework Simplace.
 
 You need to install the Simplace simulation
 framework https://www.simplace.net/
@@ -31,9 +32,7 @@
     >>> simplace.runSimulations(sh)
     >>> result = simplace.resultToList(simplace.getResult(sh,'YearOut',simid))
     >>> simplace.closeProject(sh)
     >>> print(result['BiomassModule.Yield'])
     805.45
 
 The module requires Java >= 11.0 and python packages numpy and JPype1.
-
-
```

### Comparing `simplace-5.0.5/README.rst` & `simplace-5.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `simplace-5.0.5/setup.py` & `simplace-5.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `simplace-5.0.5/simplace/SimplaceClasses.py` & `simplace-5.1.0/simplace/SimplaceClasses.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 import simplace
 
 class SimplaceInstance:
     """Class to access and control the simulation Framework Simplace"""
 
     def __init__(self, installDir = None, workDir = None, outputDir = None,
                 projectsDir=None, dataDir=None,
-                 additionalClasspathList =[], javaParameters = ''):
+                 additionalClasspathList =[], javaParameters = None):
         self._sh = simplace.initSimplace(installDir, workDir, outputDir,
                                  projectsDir, dataDir,
                                  additionalClasspathList, javaParameters)
 
     def shutDown(self):
         """Terminates the java virtual machine"""
         simplace.shutDown(self._sh)
```

### Comparing `simplace-5.0.5/simplace/simplace.py` & `simplace-5.1.0/simplace/simplace.py`

 * *Files identical despite different names*

### Comparing `simplace-5.0.5/simplace.egg-info/PKG-INFO` & `simplace-5.1.0/simplace.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: simplace
-Version: 5.0.5
+Version: 5.1.0
 Summary: Interact with the simulation framework Simplace
 Home-page: https://www.simplace.net/
 Author: Gunther Krauss
 Author-email: guntherkrauss@uni-bonn.de
 License: GPL3
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Java
 License-File: LICENSE
+Requires-Dist: Jpype1
+Requires-Dist: numpy
 
 See the documentation at https://simplace.readthedocs.io/
 
 Run and control simulations in the simulation framework Simplace.
 
 You need to install the Simplace simulation
 framework https://www.simplace.net/
@@ -31,9 +32,7 @@
     >>> simplace.runSimulations(sh)
     >>> result = simplace.resultToList(simplace.getResult(sh,'YearOut',simid))
     >>> simplace.closeProject(sh)
     >>> print(result['BiomassModule.Yield'])
     805.45
 
 The module requires Java >= 11.0 and python packages numpy and JPype1.
-
-
```

