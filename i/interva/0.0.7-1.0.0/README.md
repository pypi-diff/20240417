# Comparing `tmp/interva-0.0.7.tar.gz` & `tmp/interva-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interva-0.0.7.tar", last modified: Wed Apr  3 20:19:45 2024, max compression
+gzip compressed data, was "interva-1.0.0.tar", last modified: Wed Apr 17 17:20:38 2024, max compression
```

## Comparing `interva-0.0.7.tar` & `interva-1.0.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-03 20:19:45.162723 interva-0.0.7/
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    35149 2022-07-29 15:44:16.000000 interva-0.0.7/LICENSE
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)      126 2024-04-03 19:06:42.000000 interva-0.0.7/MANIFEST.in
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     4514 2024-04-03 20:19:45.161797 interva-0.0.7/PKG-INFO
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     3462 2023-03-13 22:54:59.000000 interva-0.0.7/README.md
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     1376 2024-04-03 19:07:52.000000 interva-0.0.7/pyproject.toml
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)       38 2024-04-03 20:19:45.163200 interva-0.0.7/setup.cfg
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)       38 2024-04-03 19:09:08.000000 interva-0.0.7/setup.py
-drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-03 20:19:45.139001 interva-0.0.7/src/
-drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-03 20:19:45.146562 interva-0.0.7/src/interva/
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)      150 2023-02-09 17:14:38.000000 interva-0.0.7/src/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)      290 2023-08-09 13:57:17.000000 interva-0.0.7/src/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-03 20:19:45.155549 interva-0.0.7/src/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     5724 2023-05-12 20:38:51.000000 interva-0.0.7/src/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)   459264 2023-03-22 19:50:10.000000 interva-0.0.7/src/interva/data/probbase.xls
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)   164661 2022-07-29 16:52:08.000000 interva-0.0.7/src/interva/data/probbaseV5_19.csv
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)   286521 2022-11-03 17:23:26.000000 interva-0.0.7/src/interva/data/randomva5.csv
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)      518 2023-05-11 15:53:16.000000 interva-0.0.7/src/interva/exceptions.py
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    42335 2024-04-03 19:51:03.000000 interva-0.0.7/src/interva/interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    19211 2024-04-03 19:24:32.000000 interva-0.0.7/src/interva/utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-03 20:19:45.159959 interva-0.0.7/src/interva.egg-info/
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     4514 2024-04-03 20:19:45.000000 interva-0.0.7/src/interva.egg-info/PKG-INFO
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)      542 2024-04-03 20:19:45.000000 interva-0.0.7/src/interva.egg-info/SOURCES.txt
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        1 2024-04-03 20:19:45.000000 interva-0.0.7/src/interva.egg-info/dependency_links.txt
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)       26 2024-04-03 20:19:45.000000 interva-0.0.7/src/interva.egg-info/requires.txt
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        8 2024-04-03 20:19:45.000000 interva-0.0.7/src/interva.egg-info/top_level.txt
-drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-03 20:19:45.158764 interva-0.0.7/tests/
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     3833 2024-04-03 19:46:40.000000 interva-0.0.7/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    10772 2023-05-12 16:39:17.000000 interva-0.0.7/tests/test_interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     4733 2024-04-03 20:08:46.000000 interva-0.0.7/tests/test_utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-17 17:20:38.435361 interva-1.0.0/
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    35149 2022-07-29 15:44:16.000000 interva-1.0.0/LICENSE
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)      126 2024-04-03 19:06:42.000000 interva-1.0.0/MANIFEST.in
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     4632 2024-04-17 17:20:38.434804 interva-1.0.0/PKG-INFO
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     3579 2024-04-17 17:16:59.000000 interva-1.0.0/README.md
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     1377 2024-04-17 17:16:59.000000 interva-1.0.0/pyproject.toml
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)       38 2024-04-17 17:20:38.435483 interva-1.0.0/setup.cfg
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)       38 2024-04-03 19:09:08.000000 interva-1.0.0/setup.py
+drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-17 17:20:38.418571 interva-1.0.0/src/
+drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-17 17:20:38.424739 interva-1.0.0/src/interva/
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)      150 2023-02-09 17:14:38.000000 interva-1.0.0/src/interva/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)      290 2023-08-09 13:57:17.000000 interva-1.0.0/src/interva/__version__.py
+drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-17 17:20:38.430876 interva-1.0.0/src/interva/data/
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     5724 2023-05-12 20:38:51.000000 interva-1.0.0/src/interva/data/causetext.py
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)   459264 2023-03-22 19:50:10.000000 interva-1.0.0/src/interva/data/probbase.xls
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)   164661 2022-07-29 16:52:08.000000 interva-1.0.0/src/interva/data/probbaseV5_19.csv
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)   286521 2022-11-03 17:23:26.000000 interva-1.0.0/src/interva/data/randomva5.csv
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)      518 2023-05-11 15:53:16.000000 interva-1.0.0/src/interva/exceptions.py
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    42286 2024-04-17 17:11:53.000000 interva-1.0.0/src/interva/interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    19211 2024-04-03 19:24:32.000000 interva-1.0.0/src/interva/utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-17 17:20:38.433966 interva-1.0.0/src/interva.egg-info/
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     4632 2024-04-17 17:20:38.000000 interva-1.0.0/src/interva.egg-info/PKG-INFO
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)      542 2024-04-17 17:20:38.000000 interva-1.0.0/src/interva.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        1 2024-04-17 17:20:38.000000 interva-1.0.0/src/interva.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)       33 2024-04-17 17:20:38.000000 interva-1.0.0/src/interva.egg-info/requires.txt
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        8 2024-04-17 17:20:38.000000 interva-1.0.0/src/interva.egg-info/top_level.txt
+drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-17 17:20:38.433121 interva-1.0.0/tests/
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     3833 2024-04-03 19:46:40.000000 interva-1.0.0/tests/test_compare_r.py
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    10772 2023-05-12 16:39:17.000000 interva-1.0.0/tests/test_interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     4733 2024-04-03 20:08:46.000000 interva-1.0.0/tests/test_utils.py
```

### Comparing `interva-0.0.7/LICENSE` & `interva-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `interva-0.0.7/PKG-INFO` & `interva-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: interva
-Version: 0.0.7
+Version: 1.0.0
 Summary: Python implementation of the InterVA Algorithm.
 Author-email: Sherry Zhao <zhao.3248@buckeyemail.osu.edu>, Jason Thomas <jarathomas@gmail.com>
-Maintainer-email: Jason Thomas <jarathomas@gmail.com>
+Maintainer-email: openVA Team <help@openva.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/verbal-autopsy-software/interva
 Project-URL: Bug Tracker, https://github.com/verbal-autopsy-software/interva/issues
 Keywords: verbal autopsy
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -17,23 +17,24 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: numpy
-Requires-Dist: vacheck
+Requires-Dist: vacheck>=0.0.3
 Requires-Dist: xlrd
 
 # interva
 
 [![image](https://img.shields.io/pypi/pyversions/interva)](https://pypi.org/project/interva/)
 [![pytest](https://github.com/verbal-autopsy-software/interva/actions/workflows/python-package.yml/badge.svg)](https://github.com/verbal-autopsy-software/interva/actions)
 
-Python implementation of the InterVA algorithm for assigning causes of death to verbal autopsy data
+Python implementation of the InterVA (version 5) algorithm for assigning causes of death to verbal autopsy data.  This package replicates the R
+version [InterVA5](https://github.com/verbal-autopsy-software/InterVA5).
 
 
 ## Importing package and installing dependencies
 
 To install all package dependencies, run:  
 
 ```python
```

### Comparing `interva-0.0.7/README.md` & `interva-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # interva
 
 [![image](https://img.shields.io/pypi/pyversions/interva)](https://pypi.org/project/interva/)
 [![pytest](https://github.com/verbal-autopsy-software/interva/actions/workflows/python-package.yml/badge.svg)](https://github.com/verbal-autopsy-software/interva/actions)
 
-Python implementation of the InterVA algorithm for assigning causes of death to verbal autopsy data
+Python implementation of the InterVA (version 5) algorithm for assigning causes of death to verbal autopsy data.  This package replicates the R
+version [InterVA5](https://github.com/verbal-autopsy-software/InterVA5).
 
 
 ## Importing package and installing dependencies
 
 To install all package dependencies, run:  
 
 ```python
```

### Comparing `interva-0.0.7/pyproject.toml` & `interva-1.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "interva"
-version = "0.0.7"
+version = "1.0.0"
 authors = [
     {name = "Sherry Zhao", email = "zhao.3248@buckeyemail.osu.edu"},
     {name = "Jason Thomas", email = "jarathomas@gmail.com"},
 ]
 maintainers = [
-    {name = "Jason Thomas", email = "jarathomas@gmail.com"},
+    {name = "openVA Team", email = "help@openva.net"},
 ]
 description = "Python implementation of the InterVA Algorithm."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["verbal autopsy",]
 license = {text = "GPLv3"}
 classifiers=[
@@ -26,15 +26,15 @@
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
 ]
 dependencies = [
         "pandas",
         "numpy",
-	"vacheck",
+	"vacheck>=0.0.3",
 	"xlrd",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/verbal-autopsy-software/interva"
 "Bug Tracker" = "https://github.com/verbal-autopsy-software/interva/issues"
```

### Comparing `interva-0.0.7/src/interva/data/causetext.py` & `interva-1.0.0/src/interva/data/causetext.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.7/src/interva/data/probbase.xls` & `interva-1.0.0/src/interva/data/probbase.xls`

 * *Files identical despite different names*

### Comparing `interva-0.0.7/src/interva/data/probbaseV5_19.csv` & `interva-1.0.0/src/interva/data/probbaseV5_19.csv`

 * *Files identical despite different names*

### Comparing `interva-0.0.7/src/interva/data/randomva5.csv` & `interva-1.0.0/src/interva/data/randomva5.csv`

 * *Files identical despite different names*

### Comparing `interva-0.0.7/src/interva/exceptions.py` & `interva-1.0.0/src/interva/exceptions.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.7/src/interva/interva5.py` & `interva-1.0.0/src/interva/interva5.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,16 +280,15 @@
             file_handler = FileHandler("errorlogV5.txt", mode="w")
             logger.addHandler(file_handler)
             now = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
             logger.info(f"Error & warning log built for InterVA5 {now}\n")
         if isinstance(self.va_input, str) and self.va_input[-4:] == ".csv":
             self.va_input = read_csv(self.va_input)
         if "i183o" in self.va_input.columns:
-            self.va_input.rename(columns={"i183o": "i183a"}, axis="columns",
-                                 inplace=True)
+            self.va_input.rename(columns={"i183o": "i183a"}, inplace=True)
             print(
                 "Due to the inconsistent names in the early version of "
                 "InterVA5, the indicator 'i183o' has been renamed as 'i183a'.")
 
         va_data = self.va_input.copy()
         va_input_names = va_data.columns
         id_inputs = va_data.iloc[:, 0]
```

### Comparing `interva-0.0.7/src/interva/utils.py` & `interva-1.0.0/src/interva/utils.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.7/src/interva.egg-info/PKG-INFO` & `interva-1.0.0/src/interva.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: interva
-Version: 0.0.7
+Version: 1.0.0
 Summary: Python implementation of the InterVA Algorithm.
 Author-email: Sherry Zhao <zhao.3248@buckeyemail.osu.edu>, Jason Thomas <jarathomas@gmail.com>
-Maintainer-email: Jason Thomas <jarathomas@gmail.com>
+Maintainer-email: openVA Team <help@openva.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/verbal-autopsy-software/interva
 Project-URL: Bug Tracker, https://github.com/verbal-autopsy-software/interva/issues
 Keywords: verbal autopsy
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -17,23 +17,24 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: numpy
-Requires-Dist: vacheck
+Requires-Dist: vacheck>=0.0.3
 Requires-Dist: xlrd
 
 # interva
 
 [![image](https://img.shields.io/pypi/pyversions/interva)](https://pypi.org/project/interva/)
 [![pytest](https://github.com/verbal-autopsy-software/interva/actions/workflows/python-package.yml/badge.svg)](https://github.com/verbal-autopsy-software/interva/actions)
 
-Python implementation of the InterVA algorithm for assigning causes of death to verbal autopsy data
+Python implementation of the InterVA (version 5) algorithm for assigning causes of death to verbal autopsy data.  This package replicates the R
+version [InterVA5](https://github.com/verbal-autopsy-software/InterVA5).
 
 
 ## Importing package and installing dependencies
 
 To install all package dependencies, run:  
 
 ```python
```

### Comparing `interva-0.0.7/src/interva.egg-info/SOURCES.txt` & `interva-1.0.0/src/interva.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `interva-0.0.7/tests/test_compare_r.py` & `interva-1.0.0/tests/test_compare_r.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.7/tests/test_interva5.py` & `interva-1.0.0/tests/test_interva5.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.7/tests/test_utils.py` & `interva-1.0.0/tests/test_utils.py`

 * *Files identical despite different names*

