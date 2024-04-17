# Comparing `tmp/MOBiceps-0.1.1.tar.gz` & `tmp/MOBiceps-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MOBiceps-0.1.1.tar", last modified: Wed Apr 17 11:46:58 2024, max compression
+gzip compressed data, was "MOBiceps-0.1.2.tar", last modified: Wed Apr 17 12:18:25 2024, max compression
```

## Comparing `MOBiceps-0.1.1.tar` & `MOBiceps-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 dalco     (1001) dalco     (1001)        0 2024-04-17 11:46:58.724036 MOBiceps-0.1.1/
--rw-rw-r--   0 dalco     (1001) dalco     (1001)    11357 2024-02-26 10:27:50.000000 MOBiceps-0.1.1/LICENSE
--rw-rw-r--   0 dalco     (1001) dalco     (1001)       71 2023-11-06 11:19:17.000000 MOBiceps-0.1.1/MANIFEST.in
-drwxrwxr-x   0 dalco     (1001) dalco     (1001)        0 2024-04-17 11:46:58.724036 MOBiceps-0.1.1/MOBiceps/
--rw-rw-r--   0 dalco     (1001) dalco     (1001)      653 2024-02-26 10:22:38.000000 MOBiceps-0.1.1/MOBiceps/__init__.py
--rw-rw-r--   0 dalco     (1001) dalco     (1001)     4652 2024-02-26 10:12:52.000000 MOBiceps-0.1.1/MOBiceps/clean_expression_table.py
--rw-rw-r--   0 dalco     (1001) dalco     (1001)     9173 2024-02-26 10:14:12.000000 MOBiceps-0.1.1/MOBiceps/container2img.py
--rw-rw-r--   0 dalco     (1001) dalco     (1001)     6890 2024-02-26 10:14:41.000000 MOBiceps-0.1.1/MOBiceps/container_extraction.py
--rw-rw-r--   0 dalco     (1001) dalco     (1001)     6692 2024-02-26 10:16:21.000000 MOBiceps-0.1.1/MOBiceps/convertRawMP.py
--rw-rw-r--   0 dalco     (1001) dalco     (1001)     3068 2024-02-26 09:33:04.000000 MOBiceps-0.1.1/MOBiceps/convert_mzXML2img.py
--rw-rw-r--   0 dalco     (1001) dalco     (1001)    12758 2024-02-26 10:16:42.000000 MOBiceps-0.1.1/MOBiceps/create_expression_table.py
--rw-rw-r--   0 dalco     (1001) dalco     (1001)     3291 2023-11-06 11:19:17.000000 MOBiceps-0.1.1/MOBiceps/dataClasses.py
--rw-rw-r--   0 dalco     (1001) dalco     (1001)     4856 2024-02-26 10:17:12.000000 MOBiceps-0.1.1/MOBiceps/expression_table.py
--rw-rw-r--   0 dalco     (1001) dalco     (1001)    82051 2024-02-26 10:20:44.000000 MOBiceps-0.1.1/MOBiceps/featureSelector.py
--rw-rw-r--   0 dalco     (1001) dalco     (1001)     4827 2024-02-26 10:21:37.000000 MOBiceps-0.1.1/MOBiceps/foldsConstruction.py
--rw-rw-r--   0 dalco     (1001) dalco     (1001)    13535 2023-11-06 11:19:17.000000 MOBiceps-0.1.1/MOBiceps/modifiedYellowbrick.py
--rw-rw-r--   0 dalco     (1001) dalco     (1001)    30315 2024-02-26 10:23:32.000000 MOBiceps-0.1.1/MOBiceps/modifiedYellowbrick_ROCAUC.py
--rw-rw-r--   0 dalco     (1001) dalco     (1001)     8321 2024-02-26 09:56:28.000000 MOBiceps-0.1.1/MOBiceps/mzXML2npyContainer.py
--rw-rw-r--   0 dalco     (1001) dalco     (1001)     3379 2023-11-06 11:19:17.000000 MOBiceps-0.1.1/MOBiceps/npy2png.py
--rw-rw-r--   0 dalco     (1001) dalco     (1001)     8402 2024-02-26 10:24:26.000000 MOBiceps-0.1.1/MOBiceps/rfePlusPlusWF.py
-drwxrwxr-x   0 dalco     (1001) dalco     (1001)        0 2024-04-17 11:46:58.724036 MOBiceps-0.1.1/MOBiceps.egg-info/
--rw-rw-r--   0 dalco     (1001) dalco     (1001)     1224 2024-04-17 11:46:58.000000 MOBiceps-0.1.1/MOBiceps.egg-info/PKG-INFO
--rw-rw-r--   0 dalco     (1001) dalco     (1001)      662 2024-04-17 11:46:58.000000 MOBiceps-0.1.1/MOBiceps.egg-info/SOURCES.txt
--rw-rw-r--   0 dalco     (1001) dalco     (1001)        1 2024-04-17 11:46:58.000000 MOBiceps-0.1.1/MOBiceps.egg-info/dependency_links.txt
--rw-rw-r--   0 dalco     (1001) dalco     (1001)      291 2024-04-17 11:46:58.000000 MOBiceps-0.1.1/MOBiceps.egg-info/requires.txt
--rw-rw-r--   0 dalco     (1001) dalco     (1001)        9 2024-04-17 11:46:58.000000 MOBiceps-0.1.1/MOBiceps.egg-info/top_level.txt
--rw-rw-r--   0 dalco     (1001) dalco     (1001)     1224 2024-04-17 11:46:58.724036 MOBiceps-0.1.1/PKG-INFO
--rw-rw-r--   0 dalco     (1001) dalco     (1001)      811 2024-04-17 11:31:47.000000 MOBiceps-0.1.1/README.md
--rw-rw-r--   0 dalco     (1001) dalco     (1001)       38 2024-04-17 11:46:58.724036 MOBiceps-0.1.1/setup.cfg
--rw-rw-r--   0 dalco     (1001) dalco     (1001)      991 2024-02-26 13:51:51.000000 MOBiceps-0.1.1/setup.py
+drwxrwxr-x   0 dalco     (1001) dalco     (1001)        0 2024-04-17 12:18:25.753104 MOBiceps-0.1.2/
+-rw-rw-r--   0 dalco     (1001) dalco     (1001)    11357 2024-02-26 10:27:50.000000 MOBiceps-0.1.2/LICENSE
+-rw-rw-r--   0 dalco     (1001) dalco     (1001)       71 2023-11-06 11:19:17.000000 MOBiceps-0.1.2/MANIFEST.in
+drwxrwxr-x   0 dalco     (1001) dalco     (1001)        0 2024-04-17 12:18:25.749104 MOBiceps-0.1.2/MOBiceps/
+-rw-rw-r--   0 dalco     (1001) dalco     (1001)      653 2024-02-26 10:22:38.000000 MOBiceps-0.1.2/MOBiceps/__init__.py
+-rw-rw-r--   0 dalco     (1001) dalco     (1001)     4652 2024-02-26 10:12:52.000000 MOBiceps-0.1.2/MOBiceps/clean_expression_table.py
+-rw-rw-r--   0 dalco     (1001) dalco     (1001)     9173 2024-02-26 10:14:12.000000 MOBiceps-0.1.2/MOBiceps/container2img.py
+-rw-rw-r--   0 dalco     (1001) dalco     (1001)     6890 2024-02-26 10:14:41.000000 MOBiceps-0.1.2/MOBiceps/container_extraction.py
+-rw-rw-r--   0 dalco     (1001) dalco     (1001)     6692 2024-02-26 10:16:21.000000 MOBiceps-0.1.2/MOBiceps/convertRawMP.py
+-rw-rw-r--   0 dalco     (1001) dalco     (1001)     3068 2024-02-26 09:33:04.000000 MOBiceps-0.1.2/MOBiceps/convert_mzXML2img.py
+-rw-rw-r--   0 dalco     (1001) dalco     (1001)    12758 2024-02-26 10:16:42.000000 MOBiceps-0.1.2/MOBiceps/create_expression_table.py
+-rw-rw-r--   0 dalco     (1001) dalco     (1001)     3291 2023-11-06 11:19:17.000000 MOBiceps-0.1.2/MOBiceps/dataClasses.py
+-rw-rw-r--   0 dalco     (1001) dalco     (1001)     4856 2024-02-26 10:17:12.000000 MOBiceps-0.1.2/MOBiceps/expression_table.py
+-rw-rw-r--   0 dalco     (1001) dalco     (1001)    82051 2024-02-26 10:20:44.000000 MOBiceps-0.1.2/MOBiceps/featureSelector.py
+-rw-rw-r--   0 dalco     (1001) dalco     (1001)     4827 2024-02-26 10:21:37.000000 MOBiceps-0.1.2/MOBiceps/foldsConstruction.py
+-rw-rw-r--   0 dalco     (1001) dalco     (1001)    13535 2023-11-06 11:19:17.000000 MOBiceps-0.1.2/MOBiceps/modifiedYellowbrick.py
+-rw-rw-r--   0 dalco     (1001) dalco     (1001)    30315 2024-02-26 10:23:32.000000 MOBiceps-0.1.2/MOBiceps/modifiedYellowbrick_ROCAUC.py
+-rw-rw-r--   0 dalco     (1001) dalco     (1001)     8321 2024-02-26 09:56:28.000000 MOBiceps-0.1.2/MOBiceps/mzXML2npyContainer.py
+-rw-rw-r--   0 dalco     (1001) dalco     (1001)     3379 2023-11-06 11:19:17.000000 MOBiceps-0.1.2/MOBiceps/npy2png.py
+-rw-rw-r--   0 dalco     (1001) dalco     (1001)     8402 2024-02-26 10:24:26.000000 MOBiceps-0.1.2/MOBiceps/rfePlusPlusWF.py
+drwxrwxr-x   0 dalco     (1001) dalco     (1001)        0 2024-04-17 12:18:25.753104 MOBiceps-0.1.2/MOBiceps.egg-info/
+-rw-rw-r--   0 dalco     (1001) dalco     (1001)     1299 2024-04-17 12:18:25.000000 MOBiceps-0.1.2/MOBiceps.egg-info/PKG-INFO
+-rw-rw-r--   0 dalco     (1001) dalco     (1001)      662 2024-04-17 12:18:25.000000 MOBiceps-0.1.2/MOBiceps.egg-info/SOURCES.txt
+-rw-rw-r--   0 dalco     (1001) dalco     (1001)        1 2024-04-17 12:18:25.000000 MOBiceps-0.1.2/MOBiceps.egg-info/dependency_links.txt
+-rw-rw-r--   0 dalco     (1001) dalco     (1001)      291 2024-04-17 12:18:25.000000 MOBiceps-0.1.2/MOBiceps.egg-info/requires.txt
+-rw-rw-r--   0 dalco     (1001) dalco     (1001)        9 2024-04-17 12:18:25.000000 MOBiceps-0.1.2/MOBiceps.egg-info/top_level.txt
+-rw-rw-r--   0 dalco     (1001) dalco     (1001)     1299 2024-04-17 12:18:25.753104 MOBiceps-0.1.2/PKG-INFO
+-rw-rw-r--   0 dalco     (1001) dalco     (1001)      861 2024-04-17 12:07:29.000000 MOBiceps-0.1.2/README.md
+-rw-rw-r--   0 dalco     (1001) dalco     (1001)       38 2024-04-17 12:18:25.753104 MOBiceps-0.1.2/setup.cfg
+-rw-rw-r--   0 dalco     (1001) dalco     (1001)     1022 2024-04-17 12:16:51.000000 MOBiceps-0.1.2/setup.py
```

### Comparing `MOBiceps-0.1.1/LICENSE` & `MOBiceps-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `MOBiceps-0.1.1/MOBiceps/__init__.py` & `MOBiceps-0.1.2/MOBiceps/__init__.py`

 * *Files identical despite different names*

### Comparing `MOBiceps-0.1.1/MOBiceps/clean_expression_table.py` & `MOBiceps-0.1.2/MOBiceps/clean_expression_table.py`

 * *Files identical despite different names*

### Comparing `MOBiceps-0.1.1/MOBiceps/container2img.py` & `MOBiceps-0.1.2/MOBiceps/container2img.py`

 * *Files identical despite different names*

### Comparing `MOBiceps-0.1.1/MOBiceps/container_extraction.py` & `MOBiceps-0.1.2/MOBiceps/container_extraction.py`

 * *Files identical despite different names*

### Comparing `MOBiceps-0.1.1/MOBiceps/convertRawMP.py` & `MOBiceps-0.1.2/MOBiceps/convertRawMP.py`

 * *Files identical despite different names*

### Comparing `MOBiceps-0.1.1/MOBiceps/convert_mzXML2img.py` & `MOBiceps-0.1.2/MOBiceps/convert_mzXML2img.py`

 * *Files identical despite different names*

### Comparing `MOBiceps-0.1.1/MOBiceps/create_expression_table.py` & `MOBiceps-0.1.2/MOBiceps/create_expression_table.py`

 * *Files identical despite different names*

### Comparing `MOBiceps-0.1.1/MOBiceps/dataClasses.py` & `MOBiceps-0.1.2/MOBiceps/dataClasses.py`

 * *Files identical despite different names*

### Comparing `MOBiceps-0.1.1/MOBiceps/expression_table.py` & `MOBiceps-0.1.2/MOBiceps/expression_table.py`

 * *Files identical despite different names*

### Comparing `MOBiceps-0.1.1/MOBiceps/featureSelector.py` & `MOBiceps-0.1.2/MOBiceps/featureSelector.py`

 * *Files identical despite different names*

### Comparing `MOBiceps-0.1.1/MOBiceps/foldsConstruction.py` & `MOBiceps-0.1.2/MOBiceps/foldsConstruction.py`

 * *Files identical despite different names*

### Comparing `MOBiceps-0.1.1/MOBiceps/modifiedYellowbrick.py` & `MOBiceps-0.1.2/MOBiceps/modifiedYellowbrick.py`

 * *Files identical despite different names*

### Comparing `MOBiceps-0.1.1/MOBiceps/modifiedYellowbrick_ROCAUC.py` & `MOBiceps-0.1.2/MOBiceps/modifiedYellowbrick_ROCAUC.py`

 * *Files identical despite different names*

### Comparing `MOBiceps-0.1.1/MOBiceps/mzXML2npyContainer.py` & `MOBiceps-0.1.2/MOBiceps/mzXML2npyContainer.py`

 * *Files identical despite different names*

### Comparing `MOBiceps-0.1.1/MOBiceps/npy2png.py` & `MOBiceps-0.1.2/MOBiceps/npy2png.py`

 * *Files identical despite different names*

### Comparing `MOBiceps-0.1.1/MOBiceps/rfePlusPlusWF.py` & `MOBiceps-0.1.2/MOBiceps/rfePlusPlusWF.py`

 * *Files identical despite different names*

### Comparing `MOBiceps-0.1.1/MOBiceps.egg-info/PKG-INFO` & `MOBiceps-0.1.2/MOBiceps.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: MOBiceps
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python tools for Mass Spectrometry and Omics data.
 Home-page: https://github.com/JensSettelmeier/MOBiceps
 Author: Jens Settelmeier
 Author-email: jenssettelmeier@googlemail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
+Requires-Python: ==3.8.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MOBiceps
 ![MOBicpes logo](./images/MOBiceps.png)
 MOBiceps is a collection of python functions for omics and mass spectrometry data. It is the working arm of [MOAgent](https://github.com/wollscheidlab/MOAgent). An early version of its core function featureSelector.py was first time applied in the work [Nature Communications, 2023](https://www.nature.com/articles/s41467-023-42101-z) to identify phenotype-specific proteins in myeloproliferative neoplasms (blood cancer).
 If you have any questions please do not hesitate to contact jsettelmeier@ethz.ch
@@ -23,7 +24,10 @@
 $ git clone https://github.com/wollscheidlab/MOBiceps.git
 ```
 or using the python package distribution system pip via
 
 ```bash
 $ pip install MOBiceps
 ```
+
+## Notes
+Developed and tested under python 3.8.
```

### Comparing `MOBiceps-0.1.1/MOBiceps.egg-info/SOURCES.txt` & `MOBiceps-0.1.2/MOBiceps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MOBiceps-0.1.1/PKG-INFO` & `MOBiceps-0.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: MOBiceps
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python tools for Mass Spectrometry and Omics data.
 Home-page: https://github.com/JensSettelmeier/MOBiceps
 Author: Jens Settelmeier
 Author-email: jenssettelmeier@googlemail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
+Requires-Python: ==3.8.*
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MOBiceps
 ![MOBicpes logo](./images/MOBiceps.png)
 MOBiceps is a collection of python functions for omics and mass spectrometry data. It is the working arm of [MOAgent](https://github.com/wollscheidlab/MOAgent). An early version of its core function featureSelector.py was first time applied in the work [Nature Communications, 2023](https://www.nature.com/articles/s41467-023-42101-z) to identify phenotype-specific proteins in myeloproliferative neoplasms (blood cancer).
 If you have any questions please do not hesitate to contact jsettelmeier@ethz.ch
@@ -23,7 +24,10 @@
 $ git clone https://github.com/wollscheidlab/MOBiceps.git
 ```
 or using the python package distribution system pip via
 
 ```bash
 $ pip install MOBiceps
 ```
+
+## Notes
+Developed and tested under python 3.8.
```

### Comparing `MOBiceps-0.1.1/README.md` & `MOBiceps-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -11,7 +11,10 @@
 $ git clone https://github.com/wollscheidlab/MOBiceps.git
 ```
 or using the python package distribution system pip via
 
 ```bash
 $ pip install MOBiceps
 ```
+
+## Notes
+Developed and tested under python 3.8.
```

### Comparing `MOBiceps-0.1.1/setup.py` & `MOBiceps-0.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ﻿from setuptools import setup, find_packages
 
 setup(
     name="MOBiceps",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'joblib==1.2.0',
 	'numpy==1.21.6',
 	'pandas==1.4.1',
 	'seaborn==0.11.2',
@@ -20,14 +20,15 @@
 	'tqdm==4.63.0',
 	'pyopenms==2.7.0',
 	'numba==0.55.1',
 	'torch==1.13.1',
 	'torchvision==0.14.1',
 	'torchaudio==0.13.1',
 	'statsmodels==0.13.2'],
+    python_requires='==3.8.*',
     author='Jens Settelmeier',
     author_email='jenssettelmeier@googlemail.com',
     description='Python tools for Mass Spectrometry and Omics data.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown', 
     url='https://github.com/JensSettelmeier/MOBiceps',  
     classifiers=[
```

