# Comparing `tmp/soma_integ-0.0.1.tar.gz` & `tmp/soma_integ-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soma_integ-0.0.1.tar", last modified: Mon Apr 15 11:41:07 2024, max compression
+gzip compressed data, was "soma_integ-0.0.2.tar", last modified: Wed Apr 17 06:41:05 2024, max compression
```

## Comparing `soma_integ-0.0.1.tar` & `soma_integ-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-15 11:41:07.106881 soma_integ-0.0.1/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1073 2024-04-15 11:21:18.000000 soma_integ-0.0.1/LICENSE
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      711 2024-04-15 11:41:07.106533 soma_integ-0.0.1/PKG-INFO
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-15 11:15:15.000000 soma_integ-0.0.1/README.md
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      813 2024-04-15 11:36:14.000000 soma_integ-0.0.1/pyproject.toml
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       38 2024-04-15 11:41:07.106930 soma_integ-0.0.1/setup.cfg
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-15 11:41:07.102150 soma_integ-0.0.1/src/
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-15 11:41:07.104855 soma_integ-0.0.1/src/soma_integ/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      469 2024-03-09 18:26:42.000000 soma_integ-0.0.1/src/soma_integ/__init__.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      681 2024-03-04 18:10:58.000000 soma_integ-0.0.1/src/soma_integ/basemodel.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1841 2024-03-04 18:10:58.000000 soma_integ-0.0.1/src/soma_integ/config.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     2298 2024-03-09 19:19:18.000000 soma_integ-0.0.1/src/soma_integ/data.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     2038 2024-03-04 18:10:58.000000 soma_integ-0.0.1/src/soma_integ/evaluation.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      272 2024-03-04 18:10:58.000000 soma_integ-0.0.1/src/soma_integ/methods.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     4851 2024-03-09 18:31:58.000000 soma_integ-0.0.1/src/soma_integ/optimization.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      197 2024-03-04 18:10:58.000000 soma_integ-0.0.1/src/soma_integ/utils.py
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-15 11:41:07.106150 soma_integ-0.0.1/src/soma_integ.egg-info/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      711 2024-04-15 11:41:07.000000 soma_integ-0.0.1/src/soma_integ.egg-info/PKG-INFO
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      448 2024-04-15 11:41:07.000000 soma_integ-0.0.1/src/soma_integ.egg-info/SOURCES.txt
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        1 2024-04-15 11:41:07.000000 soma_integ-0.0.1/src/soma_integ.egg-info/dependency_links.txt
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       20 2024-04-15 11:41:07.000000 soma_integ-0.0.1/src/soma_integ.egg-info/requires.txt
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       11 2024-04-15 11:41:07.000000 soma_integ-0.0.1/src/soma_integ.egg-info/top_level.txt
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-15 11:41:07.105952 soma_integ-0.0.1/tests/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-15 11:14:17.000000 soma_integ-0.0.1/tests/test.py
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-17 06:41:05.626341 soma_integ-0.0.2/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1073 2024-04-15 11:21:18.000000 soma_integ-0.0.2/LICENSE
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      745 2024-04-17 06:41:05.626119 soma_integ-0.0.2/PKG-INFO
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-15 11:15:15.000000 soma_integ-0.0.2/README.md
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      833 2024-04-17 06:35:12.000000 soma_integ-0.0.2/pyproject.toml
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       38 2024-04-17 06:41:05.626376 soma_integ-0.0.2/setup.cfg
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-17 06:41:05.621747 soma_integ-0.0.2/src/
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-17 06:41:05.624640 soma_integ-0.0.2/src/soma_integ/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      469 2024-03-09 18:26:42.000000 soma_integ-0.0.2/src/soma_integ/__init__.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      681 2024-03-04 18:10:58.000000 soma_integ-0.0.2/src/soma_integ/basemodel.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1841 2024-03-04 18:10:58.000000 soma_integ-0.0.2/src/soma_integ/config.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     2298 2024-03-09 19:19:18.000000 soma_integ-0.0.2/src/soma_integ/data.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     2038 2024-03-04 18:10:58.000000 soma_integ-0.0.2/src/soma_integ/evaluation.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      272 2024-03-04 18:10:58.000000 soma_integ-0.0.2/src/soma_integ/methods.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     4851 2024-03-09 18:31:58.000000 soma_integ-0.0.2/src/soma_integ/optimization.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      197 2024-03-04 18:10:58.000000 soma_integ-0.0.2/src/soma_integ/utils.py
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-17 06:41:05.625832 soma_integ-0.0.2/src/soma_integ.egg-info/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      745 2024-04-17 06:41:05.000000 soma_integ-0.0.2/src/soma_integ.egg-info/PKG-INFO
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      448 2024-04-17 06:41:05.000000 soma_integ-0.0.2/src/soma_integ.egg-info/SOURCES.txt
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        1 2024-04-17 06:41:05.000000 soma_integ-0.0.2/src/soma_integ.egg-info/dependency_links.txt
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       26 2024-04-17 06:41:05.000000 soma_integ-0.0.2/src/soma_integ.egg-info/requires.txt
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       11 2024-04-17 06:41:05.000000 soma_integ-0.0.2/src/soma_integ.egg-info/top_level.txt
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-17 06:41:05.625632 soma_integ-0.0.2/tests/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-15 11:14:17.000000 soma_integ-0.0.2/tests/test.py
```

### Comparing `soma_integ-0.0.1/LICENSE` & `soma_integ-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `soma_integ-0.0.1/pyproject.toml` & `soma_integ-0.0.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "soma_integ"
-version = "0.0.1"
-dependencies = ["numpy", "sklearn", "torch"]
+version = "0.0.2"
+dependencies = ["numpy", "sklearn"]
 authors = [
     { name = "Sobhan Ahmadian Moghadam", email = "sobhan.ahmadian.moghadam@gmail.com" },
     { name = "Arman Rezaei", email = "arman.x.rezaei@gmail.com" },
 ]
 description = "A package for integrating implementation and evaluation of machine learning platforms"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
+[project.optional-dependencies]
+ML = ["torch"]
+
 [project.urls]
-Homepage = "https://github.com/sobhanAhmadian/soma_integrate"      # TODO
-Issues = "https://github.com/sobhanAhmadian/soma_integrate/issues" # TODO
+Homepage = "https://github.com/sobhanAhmadian/soma_integrate"
+Issues = "https://github.com/sobhanAhmadian/soma_integrate/issues"
```

### Comparing `soma_integ-0.0.1/src/soma_integ/basemodel.py` & `soma_integ-0.0.2/src/soma_integ/basemodel.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.0.1/src/soma_integ/config.py` & `soma_integ-0.0.2/src/soma_integ/config.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.0.1/src/soma_integ/data.py` & `soma_integ-0.0.2/src/soma_integ/data.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.0.1/src/soma_integ/evaluation.py` & `soma_integ-0.0.2/src/soma_integ/evaluation.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.0.1/src/soma_integ/optimization.py` & `soma_integ-0.0.2/src/soma_integ/optimization.py`

 * *Files identical despite different names*

