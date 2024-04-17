# Comparing `tmp/s3path-0.5.4.tar.gz` & `tmp/s3path-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3path-0.5.4.tar", last modified: Thu Apr 11 20:52:10 2024, max compression
+gzip compressed data, was "s3path-0.5.5.tar", last modified: Thu Apr 11 21:09:49 2024, max compression
```

## Comparing `s3path-0.5.4.tar` & `s3path-0.5.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:52:10.987448 s3path-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-11 20:52:05.000000 s3path-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 20:52:05.000000 s3path-0.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-11 20:52:10.987448 s3path-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-11 20:52:05.000000 s3path-0.5.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:52:10.987448 s3path-0.5.4/s3path/
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-11 20:52:05.000000 s3path-0.5.4/s3path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17211 2024-04-11 20:52:05.000000 s3path-0.5.4/s3path/accessor.py
--rw-r--r--   0 runner    (1001) docker     (127)    28111 2024-04-11 20:52:05.000000 s3path-0.5.4/s3path/current_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    50156 2024-04-11 20:52:05.000000 s3path-0.5.4/s3path/old_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:52:10.987448 s3path-0.5.4/s3path.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-11 20:52:10.000000 s3path-0.5.4/s3path.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-11 20:52:10.000000 s3path-0.5.4/s3path.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 20:52:10.000000 s3path-0.5.4/s3path.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-11 20:52:10.000000 s3path-0.5.4/s3path.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 20:52:10.000000 s3path-0.5.4/s3path.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-11 20:52:10.991448 s3path-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-11 20:52:05.000000 s3path-0.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 20:52:10.987448 s3path-0.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-11 20:52:05.000000 s3path-0.5.4/tests/test_not_supported.py
--rw-r--r--   0 runner    (1001) docker     (127)    32259 2024-04-11 20:52:05.000000 s3path-0.5.4/tests/test_path_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-04-11 20:52:05.000000 s3path-0.5.4/tests/test_pure_path_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5769 2024-04-11 20:52:05.000000 s3path-0.5.4/tests/test_s3path_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:09:49.297275 s3path-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-11 21:09:43.000000 s3path-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 21:09:43.000000 s3path-0.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-11 21:09:49.297275 s3path-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-04-11 21:09:43.000000 s3path-0.5.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:09:49.293275 s3path-0.5.5/s3path/
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-11 21:09:43.000000 s3path-0.5.5/s3path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17272 2024-04-11 21:09:43.000000 s3path-0.5.5/s3path/accessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28111 2024-04-11 21:09:43.000000 s3path-0.5.5/s3path/current_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50156 2024-04-11 21:09:43.000000 s3path-0.5.5/s3path/old_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:09:49.297275 s3path-0.5.5/s3path.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-11 21:09:49.000000 s3path-0.5.5/s3path.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-11 21:09:49.000000 s3path-0.5.5/s3path.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 21:09:49.000000 s3path-0.5.5/s3path.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-11 21:09:49.000000 s3path-0.5.5/s3path.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 21:09:49.000000 s3path-0.5.5/s3path.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-11 21:09:49.297275 s3path-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-11 21:09:43.000000 s3path-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:09:49.297275 s3path-0.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-11 21:09:43.000000 s3path-0.5.5/tests/test_not_supported.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32259 2024-04-11 21:09:43.000000 s3path-0.5.5/tests/test_path_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-04-11 21:09:43.000000 s3path-0.5.5/tests/test_pure_path_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5769 2024-04-11 21:09:43.000000 s3path-0.5.5/tests/test_s3path_configuration.py
```

### Comparing `s3path-0.5.4/LICENSE` & `s3path-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `s3path-0.5.4/PKG-INFO` & `s3path-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3path
-Version: 0.5.4
+Version: 0.5.5
 Home-page: https://github.com/liormizr/s3path
 Author: Lior Mizrahi
 Author-email: li.mizr@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: s3path Version: 0.5.4 Home-page: https://
+Metadata-Version: 2.1 Name: s3path Version: 0.5.5 Home-page: https://
 github.com/liormizr/s3path Author: Lior Mizrahi Author-email: li.mizr@gmail.com
 License: Apache 2.0 Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `s3path-0.5.4/README.rst` & `s3path-0.5.5/README.rst`

 * *Files identical despite different names*

### Comparing `s3path-0.5.4/s3path/__init__.py` & `s3path-0.5.5/s3path/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 s3path provides a Pythonic API to S3 by wrapping boto3 with pathlib interface
 """
 import sys
 
 from . import accessor
 
-__version__ = '0.5.4'
+__version__ = '0.5.5'
 __all__ = (
     'register_configuration_parameter',
     'StatResult',
     'PureS3Path',
     'S3Path',
     'VersionedS3Path',
     'PureVersionedS3Path',
```

### Comparing `s3path-0.5.4/s3path/accessor.py` & `s3path-0.5.5/s3path/accessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from functools import lru_cache
 from contextlib import suppress
 from collections import namedtuple
 from io import UnsupportedOperation
 
 
 def _lazy_import_resources(name):
+    if name in sys.modules:
+        return sys.modules[name]
     spec = importlib.util.find_spec(name)
     loader = importlib.util.LazyLoader(spec.loader)
     spec.loader = loader
     module = importlib.util.module_from_spec(spec)
     sys.modules[name] = module
     loader.exec_module(module)
     return module
```

### Comparing `s3path-0.5.4/s3path/current_version.py` & `s3path-0.5.5/s3path/current_version.py`

 * *Files identical despite different names*

### Comparing `s3path-0.5.4/s3path/old_versions.py` & `s3path-0.5.5/s3path/old_versions.py`

 * *Files identical despite different names*

### Comparing `s3path-0.5.4/s3path.egg-info/PKG-INFO` & `s3path-0.5.5/s3path.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3path
-Version: 0.5.4
+Version: 0.5.5
 Home-page: https://github.com/liormizr/s3path
 Author: Lior Mizrahi
 Author-email: li.mizr@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: s3path Version: 0.5.4 Home-page: https://
+Metadata-Version: 2.1 Name: s3path Version: 0.5.5 Home-page: https://
 github.com/liormizr/s3path Author: Lior Mizrahi Author-email: li.mizr@gmail.com
 License: Apache 2.0 Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `s3path-0.5.4/setup.py` & `s3path-0.5.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 setup(
     name='s3path',
-    version='0.5.4',
+    version='0.5.5',
     url='https://github.com/liormizr/s3path',
     author='Lior Mizrahi',
     author_email='li.mizr@gmail.com',
     packages=['s3path'],
     install_requires=[
         'boto3>=1.16.35',
         'smart-open>=5.1.0',
```

### Comparing `s3path-0.5.4/tests/test_not_supported.py` & `s3path-0.5.5/tests/test_not_supported.py`

 * *Files identical despite different names*

### Comparing `s3path-0.5.4/tests/test_path_operations.py` & `s3path-0.5.5/tests/test_path_operations.py`

 * *Files identical despite different names*

### Comparing `s3path-0.5.4/tests/test_pure_path_operations.py` & `s3path-0.5.5/tests/test_pure_path_operations.py`

 * *Files identical despite different names*

### Comparing `s3path-0.5.4/tests/test_s3path_configuration.py` & `s3path-0.5.5/tests/test_s3path_configuration.py`

 * *Files identical despite different names*

