# Comparing `tmp/ecmv-0.2.8.tar.gz` & `tmp/ecmv-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecmv-0.2.8.tar", max compression
+gzip compressed data, was "ecmv-0.2.9.tar", max compression
```

## Comparing `ecmv-0.2.8.tar` & `ecmv-0.2.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    20177 2024-03-20 10:41:23.154167 ecmv-0.2.8/LICENSE
--rw-r--r--   0        0        0    12184 2024-03-21 17:26:51.401304 ecmv-0.2.8/README.md
--rw-r--r--   0        0        0      229 2024-03-11 13:00:30.214949 ecmv-0.2.8/ecmv/__init__.py
--rw-r--r--   0        0        0      420 2024-03-20 10:40:17.189357 ecmv-0.2.8/ecmv/constants.py
--rw-r--r--   0        0        0     1995 2024-03-11 13:02:10.317321 ecmv-0.2.8/ecmv/decorators.py
--rw-r--r--   0        0        0      210 2024-03-11 11:54:14.539786 ecmv-0.2.8/ecmv/errors.py
--rw-r--r--   0        0        0     2699 2024-03-11 16:46:48.944734 ecmv-0.2.8/ecmv/extract.py
--rw-r--r--   0        0        0      797 2024-03-07 08:54:11.834000 ecmv-0.2.8/ecmv/features.py
--rw-r--r--   0        0        0  4872198 2024-03-12 09:17:02.703962 ecmv-0.2.8/ecmv/store/extract.csv
--rw-r--r--   0        0        0     2441 2024-03-11 13:00:45.973433 ecmv-0.2.8/ecmv/store.py
--rw-r--r--   0        0        0      512 2024-03-21 17:27:21.207190 ecmv-0.2.8/pyproject.toml
--rw-r--r--   0        0        0    12840 1970-01-01 00:00:00.000000 ecmv-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    20177 2024-03-20 10:41:23.154167 ecmv-0.2.9/LICENSE
+-rw-r--r--   0        0        0    12307 2024-03-21 17:30:29.313595 ecmv-0.2.9/README.md
+-rw-r--r--   0        0        0      229 2024-03-11 13:00:30.214949 ecmv-0.2.9/ecmv/__init__.py
+-rw-r--r--   0        0        0      420 2024-03-20 10:40:17.189357 ecmv-0.2.9/ecmv/constants.py
+-rw-r--r--   0        0        0     1995 2024-03-11 13:02:10.317321 ecmv-0.2.9/ecmv/decorators.py
+-rw-r--r--   0        0        0      210 2024-03-11 11:54:14.539786 ecmv-0.2.9/ecmv/errors.py
+-rw-r--r--   0        0        0     2699 2024-03-11 16:46:48.944734 ecmv-0.2.9/ecmv/extract.py
+-rw-r--r--   0        0        0      797 2024-03-07 08:54:11.834000 ecmv-0.2.9/ecmv/features.py
+-rw-r--r--   0        0        0  4872198 2024-03-12 09:17:02.703962 ecmv-0.2.9/ecmv/store/extract.csv
+-rw-r--r--   0        0        0     2441 2024-03-11 13:00:45.973433 ecmv-0.2.9/ecmv/store.py
+-rw-r--r--   0        0        0      512 2024-03-21 17:30:39.880065 ecmv-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0    12963 1970-01-01 00:00:00.000000 ecmv-0.2.9/PKG-INFO
```

### Comparing `ecmv-0.2.8/LICENSE` & `ecmv-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ecmv-0.2.8/README.md` & `ecmv-0.2.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Exeter College Machine Vision 
 
 Code for the EXE3002 - Classifiers and Machine Vision written assignment
 
-<img src="https://github.com/JWSchaefer/EXE3001-RiceData/blob/main/rice.png?raw=true"  width="200"/>
+<img src="https://github.com/JWSchaefer/EXE30001-RiceData/blob/main/Jasmine/Jasmine%20(10070).jpg?raw=True"  width="200"/>
 
 ## Index
 
 - [Overview](#overview)
 - [Installation](#installation)
 - [Examples](#examples)
 - [Documentation](#documentation)
@@ -536,7 +536,8 @@
 data : pd.Dataframe
     A pandas dataframe where each row contains the features extracted from an image
 ```
 ## Support
 
 If you are struggling to use this code, please contact your supervisor.
 
+<img src="https://github.com/JWSchaefer/EXE3001-RiceData/blob/main/rice.png?raw=True"  width="200"/>
```

### Comparing `ecmv-0.2.8/ecmv/decorators.py` & `ecmv-0.2.9/ecmv/decorators.py`

 * *Files identical despite different names*

### Comparing `ecmv-0.2.8/ecmv/extract.py` & `ecmv-0.2.9/ecmv/extract.py`

 * *Files identical despite different names*

### Comparing `ecmv-0.2.8/ecmv/features.py` & `ecmv-0.2.9/ecmv/features.py`

 * *Files identical despite different names*

### Comparing `ecmv-0.2.8/ecmv/store/extract.csv` & `ecmv-0.2.9/ecmv/store/extract.csv`

 * *Files identical despite different names*

### Comparing `ecmv-0.2.8/ecmv/store.py` & `ecmv-0.2.9/ecmv/store.py`

 * *Files identical despite different names*

### Comparing `ecmv-0.2.8/pyproject.toml` & `ecmv-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ecmv"
-version = "0.2.8"
+version = "0.2.9"
 description = "Python package for the EXE3002 - Classifiers and Machine Vision written assignment"
 authors = ["JWSchaefer <joe.w.schaefer@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 pandas = "^2.2.1"
```

### Comparing `ecmv-0.2.8/PKG-INFO` & `ecmv-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecmv
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python package for the EXE3002 - Classifiers and Machine Vision written assignment
 Author: JWSchaefer
 Author-email: joe.w.schaefer@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
@@ -16,15 +16,15 @@
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Exeter College Machine Vision 
 
 Code for the EXE3002 - Classifiers and Machine Vision written assignment
 
-<img src="https://github.com/JWSchaefer/EXE3001-RiceData/blob/main/rice.png?raw=true"  width="200"/>
+<img src="https://github.com/JWSchaefer/EXE30001-RiceData/blob/main/Jasmine/Jasmine%20(10070).jpg?raw=True"  width="200"/>
 
 ## Index
 
 - [Overview](#overview)
 - [Installation](#installation)
 - [Examples](#examples)
 - [Documentation](#documentation)
@@ -554,8 +554,9 @@
 data : pd.Dataframe
     A pandas dataframe where each row contains the features extracted from an image
 ```
 ## Support
 
 If you are struggling to use this code, please contact your supervisor.
 
+<img src="https://github.com/JWSchaefer/EXE3001-RiceData/blob/main/rice.png?raw=True"  width="200"/>
```

