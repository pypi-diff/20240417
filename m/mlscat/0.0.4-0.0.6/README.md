# Comparing `tmp/mlscat-0.0.4.tar.gz` & `tmp/mlscat-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlscat-0.0.4.tar", last modified: Wed Apr 10 06:56:34 2024, max compression
+gzip compressed data, was "mlscat-0.0.6.tar", last modified: Wed Apr 17 07:15:35 2024, max compression
```

## Comparing `mlscat-0.0.4.tar` & `mlscat-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 wink       (501) staff       (20)        0 2024-04-10 06:56:34.523596 mlscat-0.0.4/
--rw-r--r--   0 wink       (501) staff       (20)      756 2024-04-10 06:56:34.523291 mlscat-0.0.4/PKG-INFO
--rw-r--r--   0 wink       (501) staff       (20)      481 2024-04-09 04:32:51.000000 mlscat-0.0.4/README.md
-drwxr-xr-x   0 wink       (501) staff       (20)        0 2024-04-10 06:56:34.519654 mlscat-0.0.4/mlscat/
--rw-r--r--   0 wink       (501) staff       (20)      131 2024-04-10 06:56:27.000000 mlscat-0.0.4/mlscat/__init__.py
--rw-r--r--   0 wink       (501) staff       (20)      172 2024-04-08 14:31:16.000000 mlscat-0.0.4/mlscat/api.py
--rw-r--r--   0 wink       (501) staff       (20)     2110 2024-04-10 06:42:52.000000 mlscat-0.0.4/mlscat/attacks.py
--rw-r--r--   0 wink       (501) staff       (20)     1420 2024-04-09 07:28:32.000000 mlscat-0.0.4/mlscat/ranks.py
--rw-r--r--   0 wink       (501) staff       (20)     1700 2024-04-10 06:37:33.000000 mlscat-0.0.4/mlscat/utils.py
-drwxr-xr-x   0 wink       (501) staff       (20)        0 2024-04-10 06:56:34.522991 mlscat-0.0.4/mlscat.egg-info/
--rw-r--r--   0 wink       (501) staff       (20)      756 2024-04-10 06:56:34.000000 mlscat-0.0.4/mlscat.egg-info/PKG-INFO
--rw-r--r--   0 wink       (501) staff       (20)      250 2024-04-10 06:56:34.000000 mlscat-0.0.4/mlscat.egg-info/SOURCES.txt
--rw-r--r--   0 wink       (501) staff       (20)        1 2024-04-10 06:56:34.000000 mlscat-0.0.4/mlscat.egg-info/dependency_links.txt
--rw-r--r--   0 wink       (501) staff       (20)       13 2024-04-10 06:56:34.000000 mlscat-0.0.4/mlscat.egg-info/requires.txt
--rw-r--r--   0 wink       (501) staff       (20)        7 2024-04-10 06:56:34.000000 mlscat-0.0.4/mlscat.egg-info/top_level.txt
--rw-r--r--   0 wink       (501) staff       (20)       38 2024-04-10 06:56:34.523657 mlscat-0.0.4/setup.cfg
--rw-r--r--   0 wink       (501) staff       (20)      608 2024-04-08 13:19:29.000000 mlscat-0.0.4/setup.py
+drwxrwxr-x   0 M0nk3y    (1021) M0nk3y    (1021)        0 2024-04-17 07:15:35.942598 mlscat-0.0.6/
+-rw-r--r--   0 M0nk3y    (1021) M0nk3y    (1021)      776 2024-04-17 07:15:35.942598 mlscat-0.0.6/PKG-INFO
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      523 2024-04-17 06:13:37.000000 mlscat-0.0.6/README.md
+drwxrwxr-x   0 M0nk3y    (1021) M0nk3y    (1021)        0 2024-04-17 07:15:35.942598 mlscat-0.0.6/mlscat/
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      131 2024-04-17 07:15:25.000000 mlscat-0.0.6/mlscat/__init__.py
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      172 2024-04-17 06:13:37.000000 mlscat-0.0.6/mlscat/api.py
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)     2111 2024-04-17 06:24:18.000000 mlscat-0.0.6/mlscat/attacks.py
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)     1420 2024-04-17 06:13:37.000000 mlscat-0.0.6/mlscat/ranks.py
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)    25641 2024-04-17 07:03:35.000000 mlscat-0.0.6/mlscat/utils.py
+drwxrwxr-x   0 M0nk3y    (1021) M0nk3y    (1021)        0 2024-04-17 07:15:35.942598 mlscat-0.0.6/mlscat.egg-info/
+-rw-r--r--   0 M0nk3y    (1021) M0nk3y    (1021)      776 2024-04-17 07:15:35.000000 mlscat-0.0.6/mlscat.egg-info/PKG-INFO
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      250 2024-04-17 07:15:35.000000 mlscat-0.0.6/mlscat.egg-info/SOURCES.txt
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)        1 2024-04-17 07:15:35.000000 mlscat-0.0.6/mlscat.egg-info/dependency_links.txt
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)        6 2024-04-17 07:15:35.000000 mlscat-0.0.6/mlscat.egg-info/requires.txt
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)        7 2024-04-17 07:15:35.000000 mlscat-0.0.6/mlscat.egg-info/top_level.txt
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)       38 2024-04-17 07:15:35.942598 mlscat-0.0.6/setup.cfg
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      590 2024-04-17 07:12:12.000000 mlscat-0.0.6/setup.py
```

### Comparing `mlscat-0.0.4/PKG-INFO` & `mlscat-0.0.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: mlscat
-Version: 0.0.4
+Version: 0.0.6
 Summary: A small cat help you enjoy your side channel attack journal!
 Author: i4mhmh
 Author-email: i4mhmh@outlook.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
-Requires-Dist: pandas
 
 # MLSCAT
 
 A small cat that helps you enjoy your side channel attack journey!
 
 ## Features
 
 - Read Datasets: We provide a simple method to read some exist datasets(it would be better if there have the same structure!
 - Cal Rank: try to give the key and result nparray
+- Simple Attack: CPA, Correlation.
 
 example:
 
 ```python
 import mlscat as cat
 
 print(cat.__version__)
@@ -33,8 +33,8 @@
 To install mlscat, just follow one steps:
 
 `pip install mlscat`
 
 ## Benefits
 
 - Reduce Workload.
-- Reduce Errors.
+- Increase hair volume.
```

### Comparing `mlscat-0.0.4/mlscat/attacks.py` & `mlscat-0.0.6/mlscat/attacks.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -53,8 +53,8 @@
 
 def pearson(x:np.array, y:np.array):
     x = (x-np.mean(x,axis=0))/np.std(x,axis=0)
     x = x/np.linalg.norm(x,axis=0)
     y = (y-np.mean(y,axis=0))/np.std(y,axis=0)
     y = y/np.linalg.norm(y,axis=0)
     m = np.dot(x.T,y)
-    return abs(m)
+    return abs(m)
```

### Comparing `mlscat-0.0.4/mlscat/ranks.py` & `mlscat-0.0.6/mlscat/ranks.py`

 * *Files identical despite different names*

### Comparing `mlscat-0.0.4/mlscat.egg-info/PKG-INFO` & `mlscat-0.0.6/mlscat.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: mlscat
-Version: 0.0.4
+Version: 0.0.6
 Summary: A small cat help you enjoy your side channel attack journal!
 Author: i4mhmh
 Author-email: i4mhmh@outlook.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
-Requires-Dist: pandas
 
 # MLSCAT
 
 A small cat that helps you enjoy your side channel attack journey!
 
 ## Features
 
 - Read Datasets: We provide a simple method to read some exist datasets(it would be better if there have the same structure!
 - Cal Rank: try to give the key and result nparray
+- Simple Attack: CPA, Correlation.
 
 example:
 
 ```python
 import mlscat as cat
 
 print(cat.__version__)
@@ -33,8 +33,8 @@
 To install mlscat, just follow one steps:
 
 `pip install mlscat`
 
 ## Benefits
 
 - Reduce Workload.
-- Reduce Errors.
+- Increase hair volume.
```

### Comparing `mlscat-0.0.4/setup.py` & `mlscat-0.0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 setup(
     name=NAME,
     version=VERSION,
     packages=find_packages(),
     install_requires=[
         'numpy',
-        'pandas',
     ],
     author="i4mhmh",
     author_email='i4mhmh@outlook.com',
     description='A small cat help you enjoy your side channel attack journal!',
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires = ">=3.8"
```

