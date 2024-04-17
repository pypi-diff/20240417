# Comparing `tmp/dalsa-0.0.1.tar.gz` & `tmp/dalsa-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalsa-0.0.1.tar", last modified: Wed Apr 17 07:55:36 2024, max compression
+gzip compressed data, was "dalsa-0.0.2.tar", last modified: Wed Apr 17 08:01:38 2024, max compression
```

## Comparing `dalsa-0.0.1.tar` & `dalsa-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-04-17 07:55:36.200459 dalsa-0.0.1/
--rw-r--r--   0 dev       (1001) dev       (1001)      612 2024-04-17 07:55:36.200459 dalsa-0.0.1/PKG-INFO
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-04-17 07:39:32.000000 dalsa-0.0.1/README.md
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-04-17 07:55:36.200459 dalsa-0.0.1/dalsa/
--rw-rw-r--   0 dev       (1001) dev       (1001)     9459 2024-04-17 07:19:25.000000 dalsa-0.0.1/dalsa/ALSA.py
--rw-rw-r--   0 dev       (1001) dev       (1001)       22 2024-04-17 07:44:54.000000 dalsa-0.0.1/dalsa/__init__.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     1444 2024-04-17 07:19:25.000000 dalsa-0.0.1/dalsa/openfunctions_utils.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-04-17 07:55:36.200459 dalsa-0.0.1/dalsa.egg-info/
--rw-r--r--   0 dev       (1001) dev       (1001)      612 2024-04-17 07:55:36.000000 dalsa-0.0.1/dalsa.egg-info/PKG-INFO
--rw-rw-r--   0 dev       (1001) dev       (1001)      223 2024-04-17 07:55:36.000000 dalsa-0.0.1/dalsa.egg-info/SOURCES.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)        1 2024-04-17 07:55:36.000000 dalsa-0.0.1/dalsa.egg-info/dependency_links.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)       64 2024-04-17 07:55:36.000000 dalsa-0.0.1/dalsa.egg-info/requires.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)        6 2024-04-17 07:55:36.000000 dalsa-0.0.1/dalsa.egg-info/top_level.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)       38 2024-04-17 07:55:36.200459 dalsa-0.0.1/setup.cfg
--rw-rw-r--   0 dev       (1001) dev       (1001)     2688 2024-04-17 07:53:33.000000 dalsa-0.0.1/setup.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-04-17 08:01:38.888948 dalsa-0.0.2/
+-rw-r--r--   0 dev       (1001) dev       (1001)      612 2024-04-17 08:01:38.888948 dalsa-0.0.2/PKG-INFO
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-04-17 07:39:32.000000 dalsa-0.0.2/README.md
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-04-17 08:01:38.888948 dalsa-0.0.2/dalsa/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     9460 2024-04-17 07:59:50.000000 dalsa-0.0.2/dalsa/ALSA.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)       22 2024-04-17 07:44:54.000000 dalsa-0.0.2/dalsa/__init__.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)     1444 2024-04-17 07:19:25.000000 dalsa-0.0.2/dalsa/openfunctions_utils.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-04-17 08:01:38.888948 dalsa-0.0.2/dalsa.egg-info/
+-rw-r--r--   0 dev       (1001) dev       (1001)      612 2024-04-17 08:01:38.000000 dalsa-0.0.2/dalsa.egg-info/PKG-INFO
+-rw-rw-r--   0 dev       (1001) dev       (1001)      223 2024-04-17 08:01:38.000000 dalsa-0.0.2/dalsa.egg-info/SOURCES.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)        1 2024-04-17 08:01:38.000000 dalsa-0.0.2/dalsa.egg-info/dependency_links.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)       64 2024-04-17 08:01:38.000000 dalsa-0.0.2/dalsa.egg-info/requires.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)        6 2024-04-17 08:01:38.000000 dalsa-0.0.2/dalsa.egg-info/top_level.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)       38 2024-04-17 08:01:38.888948 dalsa-0.0.2/setup.cfg
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2688 2024-04-17 08:00:26.000000 dalsa-0.0.2/setup.py
```

### Comparing `dalsa-0.0.1/PKG-INFO` & `dalsa-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalsa
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package does Aspect Level Sentiment Analysis (ALSA) on user comments about a given product
 Author: Mostafa Amiri
 Author-email: <mostafa.amiri.62@gmail.com>
 Keywords: python,crawler,dall company
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dalsa-0.0.1/dalsa/ALSA.py` & `dalsa-0.0.2/dalsa/ALSA.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import torch
 from transformers import AutoTokenizer, AutoModelForCausalLM, pipeline
-from openfunctions_utils import strip_function_calls, parse_function_call
+from .openfunctions_utils import strip_function_calls, parse_function_call
 import pandas as pd
 from googletrans import Translator
 from tqdm import tqdm
 import re
```

### Comparing `dalsa-0.0.1/dalsa/openfunctions_utils.py` & `dalsa-0.0.2/dalsa/openfunctions_utils.py`

 * *Files identical despite different names*

### Comparing `dalsa-0.0.1/dalsa.egg-info/PKG-INFO` & `dalsa-0.0.2/dalsa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalsa
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package does Aspect Level Sentiment Analysis (ALSA) on user comments about a given product
 Author: Mostafa Amiri
 Author-email: <mostafa.amiri.62@gmail.com>
 Keywords: python,crawler,dall company
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dalsa-0.0.1/setup.py` & `dalsa-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 # Clone repositories
 clone_repositories()
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
     name="dalsa",
-    version='0.0.1',
+    version='0.0.2',
     author="Mostafa Amiri",
     author_email="<mostafa.amiri.62@gmail.com>",
     description="This package does Aspect Level Sentiment Analysis (ALSA) on user comments about a given product",
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=['regex', 'torch', 'transformers', 'pandas', 'googletrans==3.1.0a0', 'tqdm', 'regex'], # add any additional packages that
```

