# Comparing `tmp/dalsa-0.0.4.tar.gz` & `tmp/dalsa-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalsa-0.0.4.tar", last modified: Wed Apr 17 09:24:14 2024, max compression
+gzip compressed data, was "dalsa-0.0.5.tar", last modified: Wed Apr 17 09:27:36 2024, max compression
```

## Comparing `dalsa-0.0.4.tar` & `dalsa-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-04-17 09:24:14.421301 dalsa-0.0.4/
--rw-r--r--   0 dev       (1001) dev       (1001)      612 2024-04-17 09:24:14.421301 dalsa-0.0.4/PKG-INFO
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-04-17 07:39:32.000000 dalsa-0.0.4/README.md
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-04-17 09:24:14.421301 dalsa-0.0.4/dalsa/
--rw-rw-r--   0 dev       (1001) dev       (1001)     9465 2024-04-17 08:07:59.000000 dalsa-0.0.4/dalsa/ALSA.py
--rw-rw-r--   0 dev       (1001) dev       (1001)       22 2024-04-17 07:44:54.000000 dalsa-0.0.4/dalsa/__init__.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     1447 2024-04-17 08:23:25.000000 dalsa-0.0.4/dalsa/openfunctions_utils.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-04-17 09:24:14.421301 dalsa-0.0.4/dalsa.egg-info/
--rw-r--r--   0 dev       (1001) dev       (1001)      612 2024-04-17 09:24:14.000000 dalsa-0.0.4/dalsa.egg-info/PKG-INFO
--rw-rw-r--   0 dev       (1001) dev       (1001)      223 2024-04-17 09:24:14.000000 dalsa-0.0.4/dalsa.egg-info/SOURCES.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)        1 2024-04-17 09:24:14.000000 dalsa-0.0.4/dalsa.egg-info/dependency_links.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)       64 2024-04-17 09:24:14.000000 dalsa-0.0.4/dalsa.egg-info/requires.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)        6 2024-04-17 09:24:14.000000 dalsa-0.0.4/dalsa.egg-info/top_level.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)       38 2024-04-17 09:24:14.421301 dalsa-0.0.4/setup.cfg
--rw-rw-r--   0 dev       (1001) dev       (1001)     2688 2024-04-17 08:25:46.000000 dalsa-0.0.4/setup.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-04-17 09:27:36.511881 dalsa-0.0.5/
+-rw-r--r--   0 dev       (1001) dev       (1001)      612 2024-04-17 09:27:36.511881 dalsa-0.0.5/PKG-INFO
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-04-17 07:39:32.000000 dalsa-0.0.5/README.md
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-04-17 09:27:36.511881 dalsa-0.0.5/dalsa/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     9465 2024-04-17 08:07:59.000000 dalsa-0.0.5/dalsa/ALSA.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)       22 2024-04-17 07:44:54.000000 dalsa-0.0.5/dalsa/__init__.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1447 2024-04-17 09:26:53.000000 dalsa-0.0.5/dalsa/openfunctions_utils.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-04-17 09:27:36.511881 dalsa-0.0.5/dalsa.egg-info/
+-rw-r--r--   0 dev       (1001) dev       (1001)      612 2024-04-17 09:27:36.000000 dalsa-0.0.5/dalsa.egg-info/PKG-INFO
+-rw-rw-r--   0 dev       (1001) dev       (1001)      223 2024-04-17 09:27:36.000000 dalsa-0.0.5/dalsa.egg-info/SOURCES.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)        1 2024-04-17 09:27:36.000000 dalsa-0.0.5/dalsa.egg-info/dependency_links.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)       64 2024-04-17 09:27:36.000000 dalsa-0.0.5/dalsa.egg-info/requires.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)        6 2024-04-17 09:27:36.000000 dalsa-0.0.5/dalsa.egg-info/top_level.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)       38 2024-04-17 09:27:36.511881 dalsa-0.0.5/setup.cfg
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2688 2024-04-17 09:27:13.000000 dalsa-0.0.5/setup.py
```

### Comparing `dalsa-0.0.4/PKG-INFO` & `dalsa-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalsa
-Version: 0.0.4
+Version: 0.0.5
 Summary: This package does Aspect Level Sentiment Analysis (ALSA) on user comments about a given product
 Author: Mostafa Amiri
 Author-email: <mostafa.amiri.62@gmail.com>
 Keywords: python,crawler,dall company
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dalsa-0.0.4/dalsa/ALSA.py` & `dalsa-0.0.5/dalsa/ALSA.py`

 * *Files identical despite different names*

### Comparing `dalsa-0.0.4/dalsa/openfunctions_utils.py` & `dalsa-0.0.5/dalsa/openfunctions_utils.py`

 * *Files identical despite different names*

### Comparing `dalsa-0.0.4/dalsa.egg-info/PKG-INFO` & `dalsa-0.0.5/dalsa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalsa
-Version: 0.0.4
+Version: 0.0.5
 Summary: This package does Aspect Level Sentiment Analysis (ALSA) on user comments about a given product
 Author: Mostafa Amiri
 Author-email: <mostafa.amiri.62@gmail.com>
 Keywords: python,crawler,dall company
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dalsa-0.0.4/setup.py` & `dalsa-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 # Clone repositories
 clone_repositories()
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
     name="dalsa",
-    version='0.0.4',
+    version='0.0.5',
     author="Mostafa Amiri",
     author_email="<mostafa.amiri.62@gmail.com>",
     description="This package does Aspect Level Sentiment Analysis (ALSA) on user comments about a given product",
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=['regex', 'torch', 'transformers', 'pandas', 'googletrans==3.1.0a0', 'tqdm', 'regex'], # add any additional packages that
```

