# Comparing `tmp/coolML-0.0.2.tar.gz` & `tmp/coolML-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolML-0.0.2.tar", last modified: Tue Apr 16 12:13:38 2024, max compression
+gzip compressed data, was "coolML-0.0.3.tar", last modified: Wed Apr 17 08:51:44 2024, max compression
```

## Comparing `coolML-0.0.2.tar` & `coolML-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 12:13:38.487306 coolML-0.0.2/
--rw-r--r--   0 root         (0) root         (0)     3622 2024-04-16 12:13:38.487306 coolML-0.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2913 2024-04-16 12:13:22.000000 coolML-0.0.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 12:13:38.487306 coolML-0.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1427 2024-04-16 12:13:22.000000 coolML-0.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 12:13:38.483306 coolML-0.0.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 12:13:38.487306 coolML-0.0.2/src/coolML.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3622 2024-04-16 12:13:38.000000 coolML-0.0.2/src/coolML.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      187 2024-04-16 12:13:38.000000 coolML-0.0.2/src/coolML.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 12:13:38.000000 coolML-0.0.2/src/coolML.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-04-16 12:13:38.000000 coolML-0.0.2/src/coolML.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 12:13:38.000000 coolML-0.0.2/src/coolML.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 08:51:44.038751 coolML-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)     3619 2024-04-17 08:51:44.038751 coolML-0.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2913 2024-04-17 08:51:32.000000 coolML-0.0.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 08:51:44.038751 coolML-0.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1405 2024-04-17 08:51:32.000000 coolML-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 08:51:44.034751 coolML-0.0.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 08:51:44.038751 coolML-0.0.3/src/coolML/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2024-04-17 08:51:32.000000 coolML-0.0.3/src/coolML/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23002 2024-04-17 08:51:32.000000 coolML-0.0.3/src/coolML/data_processing.py
+-rw-rw-rw-   0 root         (0) root         (0)     7840 2024-04-17 08:51:32.000000 coolML-0.0.3/src/coolML/model_fitting.py
+-rw-rw-rw-   0 root         (0) root         (0)     8424 2024-04-17 08:51:32.000000 coolML-0.0.3/src/coolML/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 08:51:44.038751 coolML-0.0.3/src/coolML.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3619 2024-04-17 08:51:43.000000 coolML-0.0.3/src/coolML.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      289 2024-04-17 08:51:43.000000 coolML-0.0.3/src/coolML.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 08:51:43.000000 coolML-0.0.3/src/coolML.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-17 08:51:43.000000 coolML-0.0.3/src/coolML.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-17 08:51:43.000000 coolML-0.0.3/src/coolML.egg-info/top_level.txt
```

### Comparing `coolML-0.0.2/PKG-INFO` & `coolML-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: coolML
-Version: 0.0.2
+Version: 0.0.3
 Summary: Cool ML is a machine learning workflow developed to optimize thermionic double-assymmetric barrier heterostructures based on semiconductors
 Home-page: https://gitlab.citius.usc.es/julian.garcia.fernandez/coolML
-Author: Julián García Fernández 
+Author: Julian Garcia Fernandez 
 Author-email: julian.garcia.fernandez2@usc.es
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
```

### Comparing `coolML-0.0.2/README.md` & `coolML-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `coolML-0.0.2/setup.py` & `coolML-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,22 +5,22 @@
     long_description=''
     with open(Path(Path(__file__).parent,'README.md'), 'r') as fh:
         long_description=fh.read()
     return long_description
 
 setuptools.setup(
     name='coolML',
-    version='0.0.2',
+    version='0.0.3',
     description='Cool ML is a machine learning workflow developed to optimize thermionic double-assymmetric barrier heterostructures based on semiconductors',
     long_description=get_long_description(),
     long_description_content_type='text/markdown',
-    author='Julián García Fernández ',
+    author='Julian Garcia Fernandez ',
     author_email='julian.garcia.fernandez2@usc.es',
     url='https://gitlab.citius.usc.es/julian.garcia.fernandez/coolML',
-    setup_requires=['setuptools','numpy','pathlib '],
+    setup_requires=['setuptools'],
     install_requires=['torch','pytorch_lightning','wandb','numpy','pandas','scikit-learn','pathlib'],
     package_dir={"":"src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
     classifiers=[
         'Topic :: Utilities',
         'Intended Audience :: Developers',
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `coolML-0.0.2/src/coolML.egg-info/PKG-INFO` & `coolML-0.0.3/src/coolML.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: coolML
-Version: 0.0.2
+Version: 0.0.3
 Summary: Cool ML is a machine learning workflow developed to optimize thermionic double-assymmetric barrier heterostructures based on semiconductors
 Home-page: https://gitlab.citius.usc.es/julian.garcia.fernandez/coolML
-Author: Julián García Fernández 
+Author: Julian Garcia Fernandez 
 Author-email: julian.garcia.fernandez2@usc.es
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
```

