# Comparing `tmp/ray_utils-0.0.3.tar.gz` & `tmp/ray_utils-0.0.4.tar.gz`

## Comparing `ray_utils-0.0.3.tar` & `ray_utils-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 ray_utils-0.0.3/src/ray_utils/__init__.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 ray_utils-0.0.3/src/ray_utils/_apply_parallel.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 ray_utils-0.0.3/src/ray_utils/_init_in_context.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 ray_utils-0.0.3/tests/_apply_parallel.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ray_utils-0.0.3/tests/_init_in_context.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 ray_utils-0.0.3/LICENSE
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 ray_utils-0.0.3/README.md
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 ray_utils-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 ray_utils-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 ray_utils-0.0.4/src/ray_utils/__init__.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 ray_utils-0.0.4/src/ray_utils/_apply_parallel.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 ray_utils-0.0.4/src/ray_utils/_init_in_context.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 ray_utils-0.0.4/tests/_apply_parallel.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ray_utils-0.0.4/tests/_init_in_context.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 ray_utils-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 ray_utils-0.0.4/README.md
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 ray_utils-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 ray_utils-0.0.4/PKG-INFO
```

### Comparing `ray_utils-0.0.3/src/ray_utils/_apply_parallel.py` & `ray_utils-0.0.4/src/ray_utils/_apply_parallel.py`

 * *Files identical despite different names*

### Comparing `ray_utils-0.0.3/src/ray_utils/_init_in_context.py` & `ray_utils-0.0.4/src/ray_utils/_init_in_context.py`

 * *Files identical despite different names*

### Comparing `ray_utils-0.0.3/LICENSE` & `ray_utils-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ray_utils-0.0.3/README.md` & `ray_utils-0.0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # ray-utils
 
+[![PyPI version](https://badge.fury.io/py/ray-utils.svg)](https://badge.fury.io/py/ray-utils)
+
 utility functions for https://github.com/ray-project/ray/
     
 ## Usage
 
 Installation
 
 ```
-pip install -i https://test.pypi.org/simple/ ray-utils
+pip install ray-utils
 ```
 
 ## Documentation
 
 ### `apply_parallel`
 
 Apply a function in parallel on elements of an iterable.
@@ -41,8 +43,17 @@
 
 ## Dev notes
 
 Edit project in `github.dev` at:
 - https://github.dev/shadiakiki1986/ray-utils
 
 Push python package updates to pypi at:
-- https://www.kaggle.com/code/shadiakiki1/ray-utils--publish-to-pypi/notebook
+- https://www.kaggle.com/code/shadiakiki1/ray-utils--publish-to-pypi/notebook
+
+Python package development tutorial:
+- https://packaging.python.org/en/latest/tutorials/packaging-projects/
+
+pypi page:
+- https://pypi.org/project/ray-utils/
+
+pypi badge in this readme:
+- https://badge.fury.io/for/py/ray-utils
```

### Comparing `ray_utils-0.0.3/pyproject.toml` & `ray_utils-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ray_utils"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Shadi Akiki", email="shadi@akiki.us" },
 ]
 description = "utility functions for https://github.com/ray-project/ray/"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `ray_utils-0.0.3/PKG-INFO` & `ray_utils-0.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 Metadata-Version: 2.3
 Name: ray_utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: utility functions for https://github.com/ray-project/ray/
 Project-URL: Homepage, https://github.com/shadiakiki1986/ray_utils
 Project-URL: Issues, https://github.com/shadiakiki1986/ray_utils/issues
 Author-email: Shadi Akiki <shadi@akiki.us>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # ray-utils
 
+[![PyPI version](https://badge.fury.io/py/ray-utils.svg)](https://badge.fury.io/py/ray-utils)
+
 utility functions for https://github.com/ray-project/ray/
     
 ## Usage
 
 Installation
 
 ```
-pip install -i https://test.pypi.org/simple/ ray-utils
+pip install ray-utils
 ```
 
 ## Documentation
 
 ### `apply_parallel`
 
 Apply a function in parallel on elements of an iterable.
@@ -55,8 +57,17 @@
 
 ## Dev notes
 
 Edit project in `github.dev` at:
 - https://github.dev/shadiakiki1986/ray-utils
 
 Push python package updates to pypi at:
-- https://www.kaggle.com/code/shadiakiki1/ray-utils--publish-to-pypi/notebook
+- https://www.kaggle.com/code/shadiakiki1/ray-utils--publish-to-pypi/notebook
+
+Python package development tutorial:
+- https://packaging.python.org/en/latest/tutorials/packaging-projects/
+
+pypi page:
+- https://pypi.org/project/ray-utils/
+
+pypi badge in this readme:
+- https://badge.fury.io/for/py/ray-utils
```

