# Comparing `tmp/kingdon-1.0.0.tar.gz` & `tmp/kingdon-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kingdon-1.0.0.tar", last modified: Wed Apr 17 10:51:41 2024, max compression
+gzip compressed data, was "kingdon-1.0.1.tar", last modified: Wed Apr 17 13:21:38 2024, max compression
```

## Comparing `kingdon-1.0.0.tar` & `kingdon-1.0.1.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:51:41.596796 kingdon-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-17 10:51:31.000000 kingdon-1.0.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-17 10:51:31.000000 kingdon-1.0.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-17 10:51:31.000000 kingdon-1.0.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-17 10:51:31.000000 kingdon-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-17 10:51:31.000000 kingdon-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8680 2024-04-17 10:51:41.596796 kingdon-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-04-17 10:51:31.000000 kingdon-1.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:51:41.592796 kingdon-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-17 10:51:31.000000 kingdon-1.0.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:51:41.592796 kingdon-1.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    94383 2024-04-17 10:51:31.000000 kingdon-1.0.0/docs/_static/graph_triangle.png
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 10:51:31.000000 kingdon-1.0.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-04-17 10:51:31.000000 kingdon-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-17 10:51:31.000000 kingdon-1.0.0/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:51:41.592796 kingdon-1.0.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-17 10:51:31.000000 kingdon-1.0.0/docs/examples/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 10:51:31.000000 kingdon-1.0.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-17 10:51:31.000000 kingdon-1.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-17 10:51:31.000000 kingdon-1.0.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-17 10:51:31.000000 kingdon-1.0.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-17 10:51:31.000000 kingdon-1.0.0/docs/module_docs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-04-17 10:51:31.000000 kingdon-1.0.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-04-17 10:51:31.000000 kingdon-1.0.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-17 10:51:31.000000 kingdon-1.0.0/docs/workings.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:51:41.592796 kingdon-1.0.0/kingdon/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-17 10:51:31.000000 kingdon-1.0.0/kingdon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21930 2024-04-17 10:51:31.000000 kingdon-1.0.0/kingdon/algebra.py
--rw-r--r--   0 runner    (1001) docker     (127)    30710 2024-04-17 10:51:31.000000 kingdon-1.0.0/kingdon/codegen.py
--rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-04-17 10:51:31.000000 kingdon-1.0.0/kingdon/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-04-17 10:51:31.000000 kingdon-1.0.0/kingdon/matrixreps.py
--rw-r--r--   0 runner    (1001) docker     (127)    19332 2024-04-17 10:51:31.000000 kingdon-1.0.0/kingdon/multivector.py
--rw-r--r--   0 runner    (1001) docker     (127)     8017 2024-04-17 10:51:31.000000 kingdon-1.0.0/kingdon/operator_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-04-17 10:51:31.000000 kingdon-1.0.0/kingdon/polynomial.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-17 10:51:31.000000 kingdon-1.0.0/kingdon/taperecorder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:51:41.592796 kingdon-1.0.0/kingdon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8680 2024-04-17 10:51:41.000000 kingdon-1.0.0/kingdon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-17 10:51:41.000000 kingdon-1.0.0/kingdon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 10:51:41.000000 kingdon-1.0.0/kingdon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 10:51:41.000000 kingdon-1.0.0/kingdon.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-17 10:51:41.000000 kingdon-1.0.0/kingdon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 10:51:41.000000 kingdon-1.0.0/kingdon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-17 10:51:41.596796 kingdon-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-17 10:51:31.000000 kingdon-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:51:41.596796 kingdon-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-17 10:51:31.000000 kingdon-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-17 10:51:31.000000 kingdon-1.0.0/tests/performance_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-17 10:51:31.000000 kingdon-1.0.0/tests/test_expr_as_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)    26180 2024-04-17 10:51:31.000000 kingdon-1.0.0/tests/test_kingdon.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-17 10:51:31.000000 kingdon-1.0.0/tests/test_operator_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-04-17 10:51:31.000000 kingdon-1.0.0/tests/test_polynomial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:21:38.960552 kingdon-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-17 13:21:32.000000 kingdon-1.0.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-17 13:21:32.000000 kingdon-1.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-17 13:21:32.000000 kingdon-1.0.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-17 13:21:32.000000 kingdon-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-17 13:21:32.000000 kingdon-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8680 2024-04-17 13:21:38.960552 kingdon-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-04-17 13:21:32.000000 kingdon-1.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:21:38.956552 kingdon-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-17 13:21:32.000000 kingdon-1.0.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:21:38.960552 kingdon-1.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    94383 2024-04-17 13:21:32.000000 kingdon-1.0.1/docs/_static/graph_triangle.png
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 13:21:32.000000 kingdon-1.0.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-04-17 13:21:32.000000 kingdon-1.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-17 13:21:32.000000 kingdon-1.0.1/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:21:38.960552 kingdon-1.0.1/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-17 13:21:32.000000 kingdon-1.0.1/docs/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 13:21:32.000000 kingdon-1.0.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-17 13:21:32.000000 kingdon-1.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-17 13:21:32.000000 kingdon-1.0.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-17 13:21:32.000000 kingdon-1.0.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-17 13:21:32.000000 kingdon-1.0.1/docs/module_docs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6307 2024-04-17 13:21:32.000000 kingdon-1.0.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-04-17 13:21:32.000000 kingdon-1.0.1/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-17 13:21:32.000000 kingdon-1.0.1/docs/workings.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:21:38.960552 kingdon-1.0.1/kingdon/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-17 13:21:32.000000 kingdon-1.0.1/kingdon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21930 2024-04-17 13:21:32.000000 kingdon-1.0.1/kingdon/algebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30710 2024-04-17 13:21:32.000000 kingdon-1.0.1/kingdon/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-17 13:21:32.000000 kingdon-1.0.1/kingdon/graph.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-04-17 13:21:32.000000 kingdon-1.0.1/kingdon/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-04-17 13:21:32.000000 kingdon-1.0.1/kingdon/matrixreps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19332 2024-04-17 13:21:32.000000 kingdon-1.0.1/kingdon/multivector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8017 2024-04-17 13:21:32.000000 kingdon-1.0.1/kingdon/operator_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-04-17 13:21:32.000000 kingdon-1.0.1/kingdon/polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-17 13:21:32.000000 kingdon-1.0.1/kingdon/taperecorder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:21:38.960552 kingdon-1.0.1/kingdon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8680 2024-04-17 13:21:38.000000 kingdon-1.0.1/kingdon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-17 13:21:38.000000 kingdon-1.0.1/kingdon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 13:21:38.000000 kingdon-1.0.1/kingdon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 13:21:38.000000 kingdon-1.0.1/kingdon.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-17 13:21:38.000000 kingdon-1.0.1/kingdon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 13:21:38.000000 kingdon-1.0.1/kingdon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-17 13:21:38.964552 kingdon-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-17 13:21:32.000000 kingdon-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:21:38.960552 kingdon-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-17 13:21:32.000000 kingdon-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-17 13:21:32.000000 kingdon-1.0.1/tests/performance_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-17 13:21:32.000000 kingdon-1.0.1/tests/test_expr_as_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26180 2024-04-17 13:21:32.000000 kingdon-1.0.1/tests/test_kingdon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-17 13:21:32.000000 kingdon-1.0.1/tests/test_operator_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-04-17 13:21:32.000000 kingdon-1.0.1/tests/test_polynomial.py
```

### Comparing `kingdon-1.0.0/CONTRIBUTING.rst` & `kingdon-1.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.0/HISTORY.rst` & `kingdon-1.0.1/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.0/LICENSE` & `kingdon-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.0/PKG-INFO` & `kingdon-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingdon
-Version: 1.0.0
+Version: 1.0.1
 Summary: Pythonic Geometric Algebra Package
 Home-page: https://github.com/tbuli/kingdon
 Author: Martin Roelfs
 Author-email: martinroelfs@yahoo.com
 License: MIT license
 Keywords: kingdon
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `kingdon-1.0.0/README.rst` & `kingdon-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.0/docs/Makefile` & `kingdon-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.0/docs/_static/graph_triangle.png` & `kingdon-1.0.1/docs/_static/graph_triangle.png`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.0/docs/conf.py` & `kingdon-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.0/docs/examples/index.rst` & `kingdon-1.0.1/docs/examples/index.rst`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.0/docs/installation.rst` & `kingdon-1.0.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.0/docs/make.bat` & `kingdon-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.0/docs/module_docs.rst` & `kingdon-1.0.1/docs/module_docs.rst`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.0/docs/readme.rst` & `kingdon-1.0.1/docs/readme.rst`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.0/docs/usage.rst` & `kingdon-1.0.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.0/kingdon/algebra.py` & `kingdon-1.0.1/kingdon/algebra.py`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.0/kingdon/codegen.py` & `kingdon-1.0.1/kingdon/codegen.py`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.0/kingdon/graph.py` & `kingdon-1.0.1/kingdon/graph.py`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.0/kingdon/matrixreps.py` & `kingdon-1.0.1/kingdon/matrixreps.py`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.0/kingdon/multivector.py` & `kingdon-1.0.1/kingdon/multivector.py`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.0/kingdon/operator_dict.py` & `kingdon-1.0.1/kingdon/operator_dict.py`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.0/kingdon/polynomial.py` & `kingdon-1.0.1/kingdon/polynomial.py`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.0/kingdon/taperecorder.py` & `kingdon-1.0.1/kingdon/taperecorder.py`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.0/kingdon.egg-info/PKG-INFO` & `kingdon-1.0.1/kingdon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingdon
-Version: 1.0.0
+Version: 1.0.1
 Summary: Pythonic Geometric Algebra Package
 Home-page: https://github.com/tbuli/kingdon
 Author: Martin Roelfs
 Author-email: martinroelfs@yahoo.com
 License: MIT license
 Keywords: kingdon
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `kingdon-1.0.0/kingdon.egg-info/SOURCES.txt` & `kingdon-1.0.1/kingdon.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 docs/usage.rst
 docs/workings.rst
 docs/_static/graph_triangle.png
 docs/examples/index.rst
 kingdon/__init__.py
 kingdon/algebra.py
 kingdon/codegen.py
+kingdon/graph.js
 kingdon/graph.py
 kingdon/matrixreps.py
 kingdon/multivector.py
 kingdon/operator_dict.py
 kingdon/polynomial.py
 kingdon/taperecorder.py
 kingdon.egg-info/PKG-INFO
```

### Comparing `kingdon-1.0.0/setup.py` & `kingdon-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,10 +37,10 @@
     include_package_data=True,
     keywords='kingdon',
     name='kingdon',
     packages=find_packages(include=['kingdon', 'kingdon.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/tbuli/kingdon',
-    version='1.0.0',
+    version='1.0.1',
     zip_safe=False,
 )
```

### Comparing `kingdon-1.0.0/tests/performance_check.py` & `kingdon-1.0.1/tests/performance_check.py`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.0/tests/test_expr_as_matrix.py` & `kingdon-1.0.1/tests/test_expr_as_matrix.py`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.0/tests/test_kingdon.py` & `kingdon-1.0.1/tests/test_kingdon.py`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.0/tests/test_operator_dict.py` & `kingdon-1.0.1/tests/test_operator_dict.py`

 * *Files identical despite different names*

### Comparing `kingdon-1.0.0/tests/test_polynomial.py` & `kingdon-1.0.1/tests/test_polynomial.py`

 * *Files identical despite different names*

