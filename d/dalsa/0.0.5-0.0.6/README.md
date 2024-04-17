# Comparing `tmp/dalsa-0.0.5.tar.gz` & `tmp/dalsa-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalsa-0.0.5.tar", last modified: Wed Apr 17 09:27:36 2024, max compression
+gzip compressed data, was "dalsa-0.0.6.tar", last modified: Wed Apr 17 09:49:36 2024, max compression
```

## Comparing `dalsa-0.0.5.tar` & `dalsa-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-04-17 09:27:36.511881 dalsa-0.0.5/
--rw-r--r--   0 dev       (1001) dev       (1001)      612 2024-04-17 09:27:36.511881 dalsa-0.0.5/PKG-INFO
--rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-04-17 07:39:32.000000 dalsa-0.0.5/README.md
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-04-17 09:27:36.511881 dalsa-0.0.5/dalsa/
--rw-rw-r--   0 dev       (1001) dev       (1001)     9465 2024-04-17 08:07:59.000000 dalsa-0.0.5/dalsa/ALSA.py
--rw-rw-r--   0 dev       (1001) dev       (1001)       22 2024-04-17 07:44:54.000000 dalsa-0.0.5/dalsa/__init__.py
--rw-rw-r--   0 dev       (1001) dev       (1001)     1447 2024-04-17 09:26:53.000000 dalsa-0.0.5/dalsa/openfunctions_utils.py
-drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-04-17 09:27:36.511881 dalsa-0.0.5/dalsa.egg-info/
--rw-r--r--   0 dev       (1001) dev       (1001)      612 2024-04-17 09:27:36.000000 dalsa-0.0.5/dalsa.egg-info/PKG-INFO
--rw-rw-r--   0 dev       (1001) dev       (1001)      223 2024-04-17 09:27:36.000000 dalsa-0.0.5/dalsa.egg-info/SOURCES.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)        1 2024-04-17 09:27:36.000000 dalsa-0.0.5/dalsa.egg-info/dependency_links.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)       64 2024-04-17 09:27:36.000000 dalsa-0.0.5/dalsa.egg-info/requires.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)        6 2024-04-17 09:27:36.000000 dalsa-0.0.5/dalsa.egg-info/top_level.txt
--rw-rw-r--   0 dev       (1001) dev       (1001)       38 2024-04-17 09:27:36.511881 dalsa-0.0.5/setup.cfg
--rw-rw-r--   0 dev       (1001) dev       (1001)     2688 2024-04-17 09:27:13.000000 dalsa-0.0.5/setup.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-04-17 09:49:36.615417 dalsa-0.0.6/
+-rw-r--r--   0 dev       (1001) dev       (1001)      612 2024-04-17 09:49:36.615417 dalsa-0.0.6/PKG-INFO
+-rw-rw-r--   0 dev       (1001) dev       (1001)        0 2024-04-17 07:39:32.000000 dalsa-0.0.6/README.md
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-04-17 09:49:36.615417 dalsa-0.0.6/dalsa/
+-rw-rw-r--   0 dev       (1001) dev       (1001)     9470 2024-04-17 09:45:39.000000 dalsa-0.0.6/dalsa/ALSA.py
+-rw-rw-r--   0 dev       (1001) dev       (1001)       22 2024-04-17 07:44:54.000000 dalsa-0.0.6/dalsa/__init__.py
+drwxrwxr-x   0 dev       (1001) dev       (1001)        0 2024-04-17 09:49:36.615417 dalsa-0.0.6/dalsa.egg-info/
+-rw-r--r--   0 dev       (1001) dev       (1001)      612 2024-04-17 09:49:36.000000 dalsa-0.0.6/dalsa.egg-info/PKG-INFO
+-rw-rw-r--   0 dev       (1001) dev       (1001)      194 2024-04-17 09:49:36.000000 dalsa-0.0.6/dalsa.egg-info/SOURCES.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)        1 2024-04-17 09:49:36.000000 dalsa-0.0.6/dalsa.egg-info/dependency_links.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)       64 2024-04-17 09:49:36.000000 dalsa-0.0.6/dalsa.egg-info/requires.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)        6 2024-04-17 09:49:36.000000 dalsa-0.0.6/dalsa.egg-info/top_level.txt
+-rw-rw-r--   0 dev       (1001) dev       (1001)       38 2024-04-17 09:49:36.615417 dalsa-0.0.6/setup.cfg
+-rw-rw-r--   0 dev       (1001) dev       (1001)     2326 2024-04-17 09:49:19.000000 dalsa-0.0.6/setup.py
```

### Comparing `dalsa-0.0.5/PKG-INFO` & `dalsa-0.0.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalsa
-Version: 0.0.5
+Version: 0.0.6
 Summary: This package does Aspect Level Sentiment Analysis (ALSA) on user comments about a given product
 Author: Mostafa Amiri
 Author-email: <mostafa.amiri.62@gmail.com>
 Keywords: python,crawler,dall company
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dalsa-0.0.5/dalsa/ALSA.py` & `dalsa-0.0.6/dalsa/ALSA.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import torch
 from transformers import AutoTokenizer, AutoModelForCausalLM, pipeline
-from dalsa.openfunctions_utils import strip_function_calls, parse_function_call
+# from dalsa.openfunctions_utils import strip_function_calls, parse_function_call
 import pandas as pd
 from googletrans import Translator
 from tqdm import tqdm
 import re
 
 
 
@@ -18,15 +18,15 @@
         self.torch_dtype = torch.float16 if torch.cuda.is_available() else torch.float32
         self.model_id = model_path#"/run/user/1001/gvfs/smb-share:server=192.168.10.5,share=devel/S.Eghdami/gorilla"
         self.tokenizer = AutoTokenizer.from_pretrained(self.model_id)
         self.model = AutoModelForCausalLM.from_pretrained(self.model_id, torch_dtype=self.torch_dtype, low_cpu_mem_usage=True).to(self.device)
         self.pipe = pipeline(
         "text-generation",
         model=self.model,
-        tokenizer=self.tokenizer,
+        tokenizer=self.tokenizer,   
         max_new_tokens=64,
         batch_size=16,
         torch_dtype=self.torch_dtype,
         device=self.device,)
     def __getprompt__(self,comment,product):
```

### Comparing `dalsa-0.0.5/dalsa.egg-info/PKG-INFO` & `dalsa-0.0.6/dalsa.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalsa
-Version: 0.0.5
+Version: 0.0.6
 Summary: This package does Aspect Level Sentiment Analysis (ALSA) on user comments about a given product
 Author: Mostafa Amiri
 Author-email: <mostafa.amiri.62@gmail.com>
 Keywords: python,crawler,dall company
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dalsa-0.0.5/setup.py` & `dalsa-0.0.6/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -30,34 +30,29 @@
 #                 "Operating System :: OS Independent",
 #         ]
 # )
 import subprocess
 from setuptools import setup, find_packages
 from pathlib import Path
 
-# Function to clone repositories
-def clone_repositories():
-    subprocess.run(['pip3', 'install', 'tree_sitter'])
-    subprocess.run(['git', 'clone', 'https://github.com/tree-sitter/tree-sitter-java.git', '/alsa'])
-    subprocess.run(['git', 'clone', 'https://github.com/tree-sitter/tree-sitter-javascript.git', '/alsa'])
+
 
 # Get the current directory
 this_directory = Path(__file__).parent
 
 # Read README.md for long description
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
-# Clone repositories
-clone_repositories()
+
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
     name="dalsa",
-    version='0.0.5',
+    version='0.0.6',
     author="Mostafa Amiri",
     author_email="<mostafa.amiri.62@gmail.com>",
     description="This package does Aspect Level Sentiment Analysis (ALSA) on user comments about a given product",
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=['regex', 'torch', 'transformers', 'pandas', 'googletrans==3.1.0a0', 'tqdm', 'regex'], # add any additional packages that
```

