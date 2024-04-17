# Comparing `tmp/dalsa-0.0.6.tar.gz` & `tmp/dalsa-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalsa-0.0.6.tar", last modified: Wed Apr 17 09:49:36 2024, max compression
+gzip compressed data, was "dalsa-0.0.7.tar", last modified: Wed Apr 17 10:04:05 2024, max compression
```

## Comparing `dalsa-0.0.6.tar` & `dalsa-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-04-17 09:49:36.615417 dalsa-0.0.6/
--rw-r--r--   0 dev       (1001) dev       (1001)      612 2024-04-17 09:49:36.615417 dalsa-0.0.6/PKG-INFO
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-04-17 07:39:32.000000 dalsa-0.0.6/README.md
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-04-17 09:49:36.615417 dalsa-0.0.6/dalsa/
--rw-rw-r--   0 dev       (1001) dev       (1001)     9470 2024-04-17 09:45:39.000000 dalsa-0.0.6/dalsa/ALSA.py
--rw-rw-r--   0 dev       (1001) dev       (1001)       22 2024-04-17 07:44:54.000000 dalsa-0.0.6/dalsa/__init__.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-04-17 09:49:36.615417 dalsa-0.0.6/dalsa.egg-info/
--rw-r--r--   0 dev       (1001) dev       (1001)      612 2024-04-17 09:49:36.000000 dalsa-0.0.6/dalsa.egg-info/PKG-INFO
--rw-rw-r--   0 dev       (1001) dev       (1001)      194 2024-04-17 09:49:36.000000 dalsa-0.0.6/dalsa.egg-info/SOURCES.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)        1 2024-04-17 09:49:36.000000 dalsa-0.0.6/dalsa.egg-info/dependency_links.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)       64 2024-04-17 09:49:36.000000 dalsa-0.0.6/dalsa.egg-info/requires.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)        6 2024-04-17 09:49:36.000000 dalsa-0.0.6/dalsa.egg-info/top_level.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)       38 2024-04-17 09:49:36.615417 dalsa-0.0.6/setup.cfg
--rw-rw-r--   0 dev       (1001) dev       (1001)     2326 2024-04-17 09:49:19.000000 dalsa-0.0.6/setup.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-04-17 10:04:05.403769 dalsa-0.0.7/
+-rw-r--r--   0 dev       (1001) dev       (1001)      612 2024-04-17 10:04:05.403769 dalsa-0.0.7/PKG-INFO
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-04-17 07:39:32.000000 dalsa-0.0.7/README.md
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-04-17 10:04:05.403769 dalsa-0.0.7/dalsa/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     9470 2024-04-17 09:57:12.000000 dalsa-0.0.7/dalsa/ALSA.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)       22 2024-04-17 07:44:54.000000 dalsa-0.0.7/dalsa/__init__.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-04-17 10:04:05.403769 dalsa-0.0.7/dalsa.egg-info/
+-rw-r--r--   0 dev       (1001) dev       (1001)      612 2024-04-17 10:04:05.000000 dalsa-0.0.7/dalsa.egg-info/PKG-INFO
+-rw-rw-r--   0 dev       (1001) dev       (1001)      194 2024-04-17 10:04:05.000000 dalsa-0.0.7/dalsa.egg-info/SOURCES.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)        1 2024-04-17 10:04:05.000000 dalsa-0.0.7/dalsa.egg-info/dependency_links.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)       64 2024-04-17 10:04:05.000000 dalsa-0.0.7/dalsa.egg-info/requires.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)        6 2024-04-17 10:04:05.000000 dalsa-0.0.7/dalsa.egg-info/top_level.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)       38 2024-04-17 10:04:05.403769 dalsa-0.0.7/setup.cfg
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2326 2024-04-17 10:04:00.000000 dalsa-0.0.7/setup.py
```

### Comparing `dalsa-0.0.6/PKG-INFO` & `dalsa-0.0.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalsa
-Version: 0.0.6
+Version: 0.0.7
 Summary: This package does Aspect Level Sentiment Analysis (ALSA) on user comments about a given product
 Author: Mostafa Amiri
 Author-email: <mostafa.amiri.62@gmail.com>
 Keywords: python,crawler,dall company
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dalsa-0.0.6/dalsa/ALSA.py` & `dalsa-0.0.7/dalsa/ALSA.py`

 * *Files identical despite different names*

### Comparing `dalsa-0.0.6/dalsa.egg-info/PKG-INFO` & `dalsa-0.0.7/dalsa.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalsa
-Version: 0.0.6
+Version: 0.0.7
 Summary: This package does Aspect Level Sentiment Analysis (ALSA) on user comments about a given product
 Author: Mostafa Amiri
 Author-email: <mostafa.amiri.62@gmail.com>
 Keywords: python,crawler,dall company
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dalsa-0.0.6/setup.py` & `dalsa-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
     name="dalsa",
-    version='0.0.6',
+    version='0.0.7',
     author="Mostafa Amiri",
     author_email="<mostafa.amiri.62@gmail.com>",
     description="This package does Aspect Level Sentiment Analysis (ALSA) on user comments about a given product",
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=['regex', 'torch', 'transformers', 'pandas', 'googletrans==3.1.0a0', 'tqdm', 'regex'], # add any additional packages that
```

