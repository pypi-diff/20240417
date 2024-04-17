# Comparing `tmp/titanq-0.9.0.tar.gz` & `tmp/titanq-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titanq-0.9.0.tar", last modified: Wed Apr 10 17:54:39 2024, max compression
+gzip compressed data, was "titanq-0.9.1.tar", last modified: Wed Apr 17 16:04:04 2024, max compression
```

## Comparing `titanq-0.9.0.tar` & `titanq-0.9.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-10 17:54:39.256404 titanq-0.9.0/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      549 2024-04-01 13:41:38.000000 titanq-0.9.0/LICENSE.txt
--rw-r--r--   0 sabri     (1000) sabri     (1000)     6056 2024-04-10 17:54:39.256404 titanq-0.9.0/PKG-INFO
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     5011 2024-04-01 18:11:59.000000 titanq-0.9.0/README.md
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     1243 2024-04-09 20:13:03.000000 titanq-0.9.0/pyproject.toml
--rw-rw-r--   0 sabri     (1000) sabri     (1000)       61 2024-04-01 13:41:38.000000 titanq-0.9.0/requirements.txt
--rw-rw-r--   0 sabri     (1000) sabri     (1000)       38 2024-04-10 17:54:39.256404 titanq-0.9.0/setup.cfg
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-10 17:54:39.256404 titanq-0.9.0/tests/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     6756 2024-04-02 15:31:47.000000 titanq-0.9.0/tests/test_client.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)    22306 2024-04-09 20:13:03.000000 titanq-0.9.0/tests/test_model.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     2849 2024-04-02 15:31:47.000000 titanq-0.9.0/tests/test_numpy_util.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     1405 2024-04-05 13:48:53.000000 titanq-0.9.0/tests/test_optimize_response.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     1104 2024-04-09 20:13:03.000000 titanq-0.9.0/tests/test_variable.py
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-10 17:54:39.256404 titanq-0.9.0/titanq/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      757 2024-04-01 13:41:38.000000 titanq-0.9.0/titanq/__init__.py
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-10 17:54:39.256404 titanq-0.9.0/titanq/_client/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      127 2024-04-02 15:31:47.000000 titanq-0.9.0/titanq/_client/__init__.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     3771 2024-04-02 13:51:42.000000 titanq-0.9.0/titanq/_client/client.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     3844 2024-04-02 15:31:47.000000 titanq-0.9.0/titanq/_client/model.py
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-10 17:54:39.256404 titanq-0.9.0/titanq/_model/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      151 2024-04-01 18:11:59.000000 titanq-0.9.0/titanq/_model/__init__.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     3449 2024-04-09 20:13:03.000000 titanq-0.9.0/titanq/_model/constraints.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      984 2024-04-05 13:48:53.000000 titanq-0.9.0/titanq/_model/errors.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     1837 2024-04-02 15:31:47.000000 titanq-0.9.0/titanq/_model/manifest.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)    28992 2024-04-09 20:13:03.000000 titanq-0.9.0/titanq/_model/model.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     2752 2024-04-02 15:31:47.000000 titanq-0.9.0/titanq/_model/numpy_util.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     1986 2024-04-01 13:41:38.000000 titanq-0.9.0/titanq/_model/objective.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     4721 2024-04-05 13:48:53.000000 titanq-0.9.0/titanq/_model/optimize_response.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     3424 2024-04-09 20:13:03.000000 titanq-0.9.0/titanq/_model/variable.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     2685 2024-04-10 17:28:31.000000 titanq-0.9.0/titanq/_model/variable_list.py
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-10 17:54:39.256404 titanq-0.9.0/titanq/_storage/
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      119 2024-04-01 13:41:38.000000 titanq-0.9.0/titanq/_storage/__init__.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     4283 2024-04-05 13:48:53.000000 titanq-0.9.0/titanq/_storage/managed_storage.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     6173 2024-04-02 15:31:47.000000 titanq-0.9.0/titanq/_storage/s3_storage.py
--rw-rw-r--   0 sabri     (1000) sabri     (1000)     3919 2024-04-02 15:31:47.000000 titanq-0.9.0/titanq/_storage/storage_client.py
-drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-10 17:54:39.256404 titanq-0.9.0/titanq.egg-info/
--rw-r--r--   0 sabri     (1000) sabri     (1000)     6056 2024-04-10 17:54:39.000000 titanq-0.9.0/titanq.egg-info/PKG-INFO
--rw-rw-r--   0 sabri     (1000) sabri     (1000)      820 2024-04-10 17:54:39.000000 titanq-0.9.0/titanq.egg-info/SOURCES.txt
--rw-rw-r--   0 sabri     (1000) sabri     (1000)        1 2024-04-10 17:54:39.000000 titanq-0.9.0/titanq.egg-info/dependency_links.txt
--rw-rw-r--   0 sabri     (1000) sabri     (1000)       62 2024-04-10 17:54:39.000000 titanq-0.9.0/titanq.egg-info/requires.txt
--rw-rw-r--   0 sabri     (1000) sabri     (1000)        7 2024-04-10 17:54:39.000000 titanq-0.9.0/titanq.egg-info/top_level.txt
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-17 16:04:04.644055 titanq-0.9.1/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      549 2024-04-11 20:26:44.000000 titanq-0.9.1/LICENSE.txt
+-rw-r--r--   0 sabri     (1000) sabri     (1000)     6056 2024-04-17 16:04:04.644055 titanq-0.9.1/PKG-INFO
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     5011 2024-04-11 20:26:44.000000 titanq-0.9.1/README.md
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     1243 2024-04-17 14:24:22.000000 titanq-0.9.1/pyproject.toml
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)       61 2024-04-11 20:26:44.000000 titanq-0.9.1/requirements.txt
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)       38 2024-04-17 16:04:04.644055 titanq-0.9.1/setup.cfg
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-17 16:04:04.640055 titanq-0.9.1/tests/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     6756 2024-04-11 20:34:41.000000 titanq-0.9.1/tests/test_client.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)    22306 2024-04-11 20:34:41.000000 titanq-0.9.1/tests/test_model.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     2849 2024-04-11 20:34:41.000000 titanq-0.9.1/tests/test_numpy_util.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     1405 2024-04-11 20:34:41.000000 titanq-0.9.1/tests/test_optimize_response.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     1104 2024-04-11 20:34:41.000000 titanq-0.9.1/tests/test_variable.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-17 16:04:04.640055 titanq-0.9.1/titanq/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      757 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/__init__.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-17 16:04:04.644055 titanq-0.9.1/titanq/_client/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      127 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/_client/__init__.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3771 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/_client/client.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3844 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/_client/model.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-17 16:04:04.644055 titanq-0.9.1/titanq/_model/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      151 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/_model/__init__.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3449 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/_model/constraints.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      984 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/_model/errors.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     1837 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/_model/manifest.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)    29245 2024-04-17 14:41:47.000000 titanq-0.9.1/titanq/_model/model.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     2752 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/_model/numpy_util.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     1986 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/_model/objective.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     4721 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/_model/optimize_response.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3424 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/_model/variable.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     2685 2024-04-16 15:57:02.000000 titanq-0.9.1/titanq/_model/variable_list.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-17 16:04:04.644055 titanq-0.9.1/titanq/_storage/
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      119 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/_storage/__init__.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     4283 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/_storage/managed_storage.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     6173 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/_storage/s3_storage.py
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)     3919 2024-04-11 20:34:41.000000 titanq-0.9.1/titanq/_storage/storage_client.py
+drwxrwxr-x   0 sabri     (1000) sabri     (1000)        0 2024-04-17 16:04:04.644055 titanq-0.9.1/titanq.egg-info/
+-rw-r--r--   0 sabri     (1000) sabri     (1000)     6056 2024-04-17 16:04:04.000000 titanq-0.9.1/titanq.egg-info/PKG-INFO
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)      820 2024-04-17 16:04:04.000000 titanq-0.9.1/titanq.egg-info/SOURCES.txt
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)        1 2024-04-17 16:04:04.000000 titanq-0.9.1/titanq.egg-info/dependency_links.txt
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)       62 2024-04-17 16:04:04.000000 titanq-0.9.1/titanq.egg-info/requires.txt
+-rw-rw-r--   0 sabri     (1000) sabri     (1000)        7 2024-04-17 16:04:04.000000 titanq-0.9.1/titanq.egg-info/top_level.txt
```

### Comparing `titanq-0.9.0/LICENSE.txt` & `titanq-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `titanq-0.9.0/PKG-INFO` & `titanq-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titanq
-Version: 0.9.0
+Version: 0.9.1
 Summary: The TitanQ SDK for python
 Maintainer-email: InfinityQ <support@infinityq.tech>
 License: Apache 2.0
 Project-URL: Homepage, https://www.infinityq.tech
 Project-URL: Documentation, https://docs.titanq.infinityq.io/quickstart/category/python-sdk
 Project-URL: Examples, https://github.com/infinityq-tech/titanq-examples
 Keywords: titan,titanq,optimization,platform,infinity,infinityq
```

### Comparing `titanq-0.9.0/README.md` & `titanq-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `titanq-0.9.0/pyproject.toml` & `titanq-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "titanq"
 description = "The TitanQ SDK for python"
 dynamic = ["dependencies"]
 readme = { file = "README.md", content-type = "text/markdown" }
-version = "0.9.0"
+version = "0.9.1"
 license = { text = "Apache 2.0" }
 keywords = ["titan", "titanq", "optimization", "platform", "infinity", "infinityq"]
 requires-python = ">= 3.9"
 maintainers = [
     { name = "InfinityQ", email = "support@infinityq.tech" }
 ]
 classifiers = [
```

### Comparing `titanq-0.9.0/tests/test_client.py` & `titanq-0.9.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.0/tests/test_model.py` & `titanq-0.9.1/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.0/tests/test_numpy_util.py` & `titanq-0.9.1/tests/test_numpy_util.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.0/tests/test_optimize_response.py` & `titanq-0.9.1/tests/test_optimize_response.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.0/tests/test_variable.py` & `titanq-0.9.1/tests/test_variable.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.0/titanq/__init__.py` & `titanq-0.9.1/titanq/__init__.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.0/titanq/_client/client.py` & `titanq-0.9.1/titanq/_client/client.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.0/titanq/_client/model.py` & `titanq-0.9.1/titanq/_client/model.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.0/titanq/_model/constraints.py` & `titanq-0.9.1/titanq/_model/constraints.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.0/titanq/_model/errors.py` & `titanq-0.9.1/titanq/_model/errors.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.0/titanq/_model/manifest.py` & `titanq-0.9.1/titanq/_model/manifest.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.0/titanq/_model/model.py` & `titanq-0.9.1/titanq/_model/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import io
 import json
 import logging
 import numpy as np
 import zipfile
-from typing import Any, Dict, List, Tuple
+from typing import Any, Dict, List, Tuple, Union
 
 from .constraints import Constraints
 from .errors import (
     ConstraintAlreadySetError,
     MissingVariableError,
     MissingObjectiveError,
     ObjectiveAlreadySetError,
@@ -85,42 +85,40 @@
         # the user chose a managed storage or left it as default
         if storage_client is None:
             storage_client = ManagedStorage(self._titanq_client)
 
         self._storage_client = storage_client
 
 
-    def add_variable_vector(self, name='', size=1, vtype=Vtype.BINARY, variable_bounds: List[Tuple[int, int]]=[]):
+    def add_variable_vector(self, name='', size=1, vtype=Vtype.BINARY, variable_bounds: Union[List[Tuple[int, int]], List[Tuple[float, float]]]=[]):
         """
-        Add a vector of variable to the model. Only a single vector of variables can be set.
-        Calling this method again will override the current vector of variables
+        Add a vector of variable to the model. Multiple variable vectors can be set but with different names.
+
+        If Vtype is set to ``Vtype.INTEGER`` or ``Vtype.CONTINUOUS``, variable_bounds need to be set.
 
         :param name: The name given to this variable vector.
         :param size: The size of the vector.
         :param vtype: Type of the variables inside the vector.
         :param variable_bounds: Lower and upper bounds for the variable vector.
 
-        :raise MaximumVariableLimitError: If a variable is already defined.
-        :raise ValueError: If the size of the vector is < 1.
+        :raises MaximumVariableLimitError: If a variable is already defined.
+        :raises ValueError: If the size of the vector is < 1.
 
         Example
         ~~~~~~~
         ..  highlight:: python
         ..  code-block:: python
-        import numpy as np
         from titanq import Model, Vtype
 
         # set up model
         ...
 
-        # set up variable vectors
-        bounds = [[2.3, 4.6], [3.1, 5.3], [1.1, 4]]
-
-        model.add_variable_vector('x', 10, Vtype.BINARY)
-        model.add_variable_vector('y', 3, Vtype.CONTINUOUS, bounds)
+        model.add_variable_vector('x', 3, Vtype.BINARY)
+        model.add_variable_vector('y', 3, Vtype.INTEGER, [[0, 5], [1, 6]])
+        model.add_variable_vector('z', 3, Vtype.CONTINUOUS, [[2.3, 4.6], [3.1, 5.3], [1.1, 4]])
         """
         # validation
         if not self._constraints.is_empty():
             raise ConstraintAlreadySetError("Cannot add additional variable once constraints have been defined")
 
         if self._objective is not None:
             raise ObjectiveAlreadySetError("Cannot add additional variable once objective have been defined")
@@ -161,18 +159,18 @@
 
         :param bias: The linear constraint vector
         :type bias:  a NumPy 1-D ndarray
 
         :param target: The target of this objective matrix.
         :type target: Target Enum
 
-        :raise MissingVariableError: If no variable have been added to the model.
-        :raise ObjectiveAlreadySetError: If an objective has already been setted in this model.
-        :raise ValueError: If the weights shape or the bias shape does not fit the variable in the model.
-        :raise ValueError: If the weights or bias data type is not f32.
+        :raises MissingVariableError: If no variable have been added to the model.
+        :raises ObjectiveAlreadySetError: If an objective has already been setted in this model.
+        :raises ValueError: If the weights shape or the bias shape does not fit the variable in the model.
+        :raises ValueError: If the weights or bias data type is not f32.
 
         Example
         ~~~~~~~
         ..  highlight:: python
         ..  code-block:: python
         from titanq import Model, Target
 
@@ -184,17 +182,14 @@
         for root, connections in edges.items():
             for c in connections:
                 weights[root][c] = 1
 
         # construct the bias vector (Uniform weighting across all nodes)
         bias = np.asarray([0]*size, dtype=np.float32)
 
-        # set up model
-        ...
-
         model.set_objective_matrices(weights, bias, Target.MINIMIZE)
         """
 
         if self._variables.n_variables() == 0:
             raise MissingVariableError("Cannot set objective before adding a variable to the model.")
 
         if self._objective is not None:
@@ -208,39 +203,38 @@
     def add_set_partitioning_constraints_matrix(self, constraint_mask: np.ndarray):
         """
         Adds set partitioning constraints in matrix format to the model.
 
         :param constraint_mask: The constraint_mask matrix of shape (M, N) where M the number of constraints and N is the number of variables.
         :type constraint_mask: A NumPy 2-D dense ndarray (must be binary)
 
-        :raise MissingVariableError: If no variable have been added to the model.
-        :raise MaximumConstraintLimitError: The number of constraint exeed the limit.
-        :raise ConstraintSizeError: If the constraint_mask shape does not fit the expected shape of this model.
-        :raise ValueError: If the constraint_mask data type is not binary.
+        :raises MissingVariableError: If no variable have been added to the model.
+        :raises MaximumConstraintLimitError: The number of constraint exeed the limit.
+        :raises ConstraintSizeError: If the constraint_mask shape does not fit the expected shape of this model.
+        :raises ValueError: If the constraint_mask data type is not binary.
 
         Example
         ~~~~~~~
         ..  highlight:: python
         ..  code-block:: python
-
         from titanq import Model
 
         # set up model
         ...
 
         constraint_mask = np.array([[1, 1, 1, 0, 1], [1, 1, 1, 1, 0]])
         model.add_set_partitioning_constraints_matrix(constraint_mask)
         """
         if self._variables.n_variables() == 0:
             raise MissingVariableError("Cannot set constraints before adding a variable to the model.")
 
         if constraint_mask.ndim == 1:
             raise ValueError(
                 "Cannot use add_set_partitioning_constraints_matrix() function with a vector, " \
-                "please use add_set_partitioning_constraint() insead")
+                "please use add_set_partitioning_constraint() instead")
 
         if not is_ndarray_binary(constraint_mask):
             raise ValueError(f"Cannot add a constraint if the values are not in binary.")
 
         self._constraints.add_constraint(
             constraint_weights=constraint_mask,
             constraint_bounds=np.ones((constraint_mask.shape[0],2))
@@ -250,60 +244,58 @@
     def add_set_partitioning_constraint(self, constraint_mask: np.ndarray):
         """
         Adds set partitioning constraint vector to the model.
 
         :param constraint_mask: The constraint_mask vector of shape (N,) where N is the number of variables.
         :type constraint_mask: A NumPy 1-D dense ndarray (must be binary)
 
-        :raise MissingVariableError: If no variable have been added to the model.
+        :raises MissingVariableError: If no variable have been added to the model.
         :raises MaximumConstraintLimitError: The number of constraint exeed the limit.
-        :raise ConstraintSizeError: If the constraint_mask shape does not fit the expected shape of this model.
-        :raise ValueError: If the constraint_mask data type is not binary.
+        :raises ConstraintSizeError: If the constraint_mask shape does not fit the expected shape of this model.
+        :raises ValueError: If the constraint_mask data type is not binary.
 
         Example
         ~~~~~~~
         ..  highlight:: python
         ..  code-block:: python
-
         from titanq import Model
 
         # set up model
         ...
 
         constraint_mask = np.array([1, 1, 1, 0, 1])
         model.add_set_partitioning_constraint(constraint_mask)
         """
         if constraint_mask.ndim > 1:
             raise ValueError(
                 "Cannot use this add_set_partitioning_constraint() function with a matrix, " \
-                "please use add_set_partitioning_constraints_matrix() insead")
+                "please use add_set_partitioning_constraints_matrix() instead")
 
         self.add_set_partitioning_constraints_matrix(reshape_to_2d(constraint_mask))
 
 
     def add_cardinality_constraints_matrix(self, constraint_mask: np.ndarray, cardinalities: np.ndarray):
         """
         Adds cardinality constraints in matrix format to the model.
 
         :param constraint_mask: The constraint_mask matrix of shape (M, N) where M the number of constraints and N is the number of variables.
         :type constraint_mask: a NumPy 2-D dense ndarray (must be binary)
 
         :param cardinalities: The constraint_rhs vector of shape (M,) where M is the number of constraints
         :type cardinalities:  a NumPy 1-D ndarray (must be non-zero unsigned integer)
 
-        :raise MissingVariableError: If no variable have been added to the model.
+        :raises MissingVariableError: If no variable have been added to the model.
         :raises MaximumConstraintLimitError: The number of constraint exeed the limit.
-        :raise ConstraintSizeError: If the constraint_mask shape or the constraint_rhs shape does not fit the expected shape of this model.
-        :raise ValueError: If the constraint_mask is not binary or cardinalities data type is not unsigned integer.
+        :raises ConstraintSizeError: If the constraint_mask shape or the constraint_rhs shape does not fit the expected shape of this model.
+        :raises ValueError: If the constraint_mask is not binary or cardinalities data type is not unsigned integer.
 
         Example
         ~~~~~~~
         ..  highlight:: python
         ..  code-block:: python
-
         from titanq import Model
 
         # set up model
         ...
 
         constraint_mask = np.array([[1, 1, 1, 0, 1], [1, 1, 1, 1, 0]])
         cardinalities = np.array([3, 2])
@@ -311,15 +303,15 @@
         """
         if self._variables.n_variables() == 0:
             raise MissingVariableError("Cannot set constraints before adding a variable to the model.")
 
         if constraint_mask.ndim == 1:
             raise ValueError(
                 "Cannot use add_cardinality_constraints_matrix() function with a vector, " \
-                "please use add_cardinality_constraint() insead")
+                "please use add_cardinality_constraint() instead")
 
         if cardinalities.ndim != 1:
             raise ValueError(f"Cannot set constraints if cardinalities is not a NumPy 1-D dense ndarray")
 
         if not np.issubdtype(cardinalities.dtype, np.integer):
             raise ValueError("Found cardinalities data types not integer")
 
@@ -349,60 +341,58 @@
 
         :param constraint_mask: The constraint_mask vector of shape (N,) where N is the number of variables.
         :type constraint_mask: a NumPy 1-D dense ndarray (must be binary)
 
         :param cardinality: The constraint_rhs vector of shape (M,) where M is the number of constraints
         :type cardinality:  a non-zero unsigned integer
 
-        :raise MissingVariableError: If no variable have been added to the model.
+        :raises MissingVariableError: If no variable have been added to the model.
         :raises MaximumConstraintLimitError: The number of constraint exeed the limit.
-        :raise ConstraintSizeError: If the constraint_mask shape or the constraint_rhs shape does not fit the expected shape of this model.
-        :raise ValueError: If the constraint_mask is not binary or constraint_rhs data type is not unsigned integer.
+        :raises ConstraintSizeError: If the constraint_mask shape or the constraint_rhs shape does not fit the expected shape of this model.
+        :raises ValueError: If the constraint_mask is not binary or constraint_rhs data type is not unsigned integer.
 
         Example
         ~~~~~~~
         ..  highlight:: python
         ..  code-block:: python
-
         from titanq import Model
 
         # set up model
         ...
 
         constraint_mask = np.array([1, 1, 1, 0, 1])
-        cardinalities = 3
+        cardinality = 3
         model.add_cardinality_constraint(constraint_mask, cardinality)
         """
         if constraint_mask.ndim > 1:
             raise ValueError(
                 "Cannot use add_cardinality_constraint() function with a matrix, " \
-                "please use add_cardinality_constraints_matrix() insead")
+                "please use add_cardinality_constraints_matrix() instead")
 
         self.add_cardinality_constraints_matrix(reshape_to_2d(constraint_mask), np.full((1,), cardinality))
 
 
     def add_equality_constraints_matrix(self, constraint_mask: np.ndarray, limit: np.ndarray) -> None:
         """
         Adds an equality constraint matrix to the model.
 
         :param constraint_mask: The constraint_mask vector of shape (M, N) where M the number of constraints and N is the number of variables.
         :type constraint_mask: A NumPy 2-D dense ndarray (float32)
         :param limit: The limit vector of shape (M,) where M is the number of constraints
         :type limit: A NumPy 1-D array (float32)
 
-        :raise MissingVariableError: If no variable have been added to the model.
+        :raises MissingVariableError: If no variable have been added to the model.
         :raises MaximumConstraintLimitError: The number of constraint exceed the limit.
-        :raise ValueError: If the constraint_mask shape does not fit the expected shape of this model.
-        :raise ValueError: If the constraint_mask or limit contains irregular format ('NaN' or 'inf')
+        :raises ValueError: If the constraint_mask shape does not fit the expected shape of this model.
+        :raises ValueError: If the constraint_mask or limit contains irregular format ('NaN' or 'inf')
 
         Example
         ~~~~~~~
         ..  highlight:: python
         ..  code-block:: python
-
         from titanq import Model
 
         # set up model
         ...
 
         constraint_mask = np.array([[-3.51, 0, 0, 0], [10, 0, 0, 0]], dtype=np.float32)
         limit = np.array([2, 10], dtype=np.float32)
@@ -414,15 +404,15 @@
 
         if constraint_mask.dtype != np.float32 or limit.dtype != np.float32:
             raise ValueError(f"Input parameters must be float32, got Constraint mask: {constraint_mask.dtype}, Limit: {limit.dtype}")
 
         if constraint_mask.ndim == 1:
             raise ValueError(
                 "Cannot use add_equality_constraint_matrix() function with a vector, " \
-                "please use add_equality_constraint() insead")
+                "please use add_equality_constraint() instead")
 
         if ndarray_contains_nan_inf(constraint_mask):
             raise ValueError("Constraint mask contains NaN  or inf values")
 
         if limit.ndim != 1:
             raise ValueError("Limit must be a NumPy 1-D array")
 
@@ -443,62 +433,60 @@
         Adds an equality constraint vector to the model.
 
         :param constraint_mask: The constraint_mask vector of shape (N,) where N is the number of variables.
         :type constraint_mask: a NumPy 1-D dense ndarray (float32)
         :param limit: Limit value to the constraint mask
         :type limit: np.float32
 
-        :raise MissingVariableError: If no variable have been added to the model.
+        :raises MissingVariableError: If no variable have been added to the model.
         :raises MaximumConstraintLimitError: The number of constraint exeed the limit.
-        :raise ValueError: If the constraint_mask shape does not fit the expected shape of this model.
-        :raise ValueError: If the constraint_mask or limit contains irregular format ('NaN' or 'inf')
+        :raises ValueError: If the constraint_mask shape does not fit the expected shape of this model.
+        :raises ValueError: If the constraint_mask or limit contains irregular format ('NaN' or 'inf')
 
         Example
         ~~~~~~~
         ..  highlight:: python
         ..  code-block:: python
-
         from titanq import Model
 
         # set up model
         ...
 
         constraint_mask = np.array([1.05, -1.1], dtype=np.float32)
         limit = -3.45
 
         model.add_equality_constraint(constraint_mask, limit)
         """
         if constraint_mask.ndim > 1:
             raise ValueError(
                 "Cannot use add_equality_constraint() function with a matrix, " \
-                "please use add_equality_constraint_matrix() insead")
+                "please use add_equality_constraint_matrix() instead")
 
         self.add_equality_constraints_matrix(reshape_to_2d(constraint_mask), np.full((1,), limit, dtype=np.float32))
 
 
     def add_inequality_constraints_matrix(self, constraint_mask: np.ndarray, constraint_bounds: np.ndarray):
         """
         Adds inequality constraint matrix to the model.
 
         :param constraint_mask: The constraint_mask vector of shape (M, N) where N is the number of variables.
         :type constraint_mask: A NumPy 2-D dense ndarray (float32)
         :param constraints_bounds: Vector of shape (M, 2) where M is the number of constraints
         :type constraint_bounds: A NumPy 2-D ndarray (float32)
 
-        :raise MissingVariableError: If no variable have been added to the model.
+        :raises MissingVariableError: If no variable have been added to the model.
         :raises MaximumConstraintLimitError: The number of constraint exeed the limit.
-        :raise ValueError: If the constraint_mask shape does not fit the expected shape of this model.
-        :raise ValueError: A lowerbound is equal or higher than its given upperbound
-        :raise ValueError: If the constraint_mask contains irregular format ('NaN' or 'inf')
+        :raises ValueError: If the constraint_mask shape does not fit the expected shape of this model.
+        :raises ValueError: A lowerbound is equal or higher than its given upperbound
+        :raises ValueError: If the constraint_mask contains irregular format ('NaN' or 'inf')
 
         Example
         ~~~~~~~
         ..  highlight:: python
         ..  code-block:: python
-
         from titanq import Model
 
         # set up model
         ...
 
         constraint_mask = np.array([[-3.51, 0], [10, 0]], dtype=np.float32)
         constraint_bounds = np.array([[8, 9], [np.nan, 100_000]], dtype=np.float32)
@@ -510,15 +498,15 @@
 
         if constraint_mask.dtype != np.float32 or constraint_bounds.dtype != np.float32:
             raise ValueError(f"Input parameters must be float32, got Constraint mask: {constraint_mask.dtype}, Limit: {constraint_bounds.dtype}")
 
         if constraint_mask.ndim == 1:
             raise ValueError(
                 "Cannot use add_inequality_constraint_matrix() function with a vector, " \
-                "please use add_inequality_constraint() insead")
+                "please use add_inequality_constraint() instead")
 
         if ndarray_contains_nan_inf(constraint_mask):
             raise ValueError("Constraint mask contains NaN  or inf values.")
 
         if is_upperbound_bigger_equal_lowerbound(constraint_bounds):
             raise ValueError("Constraint bounds contains lowerbounds equal or higher than their upperbound.")
 
@@ -534,65 +522,68 @@
         Adds inequality constraint vector to the model. At least one bound must be set.
 
         :param constraint_mask: The constraint_mask vector of shape (N,) where N is the number of variables.
         :type constraint_mask: A NumPy 1-D dense ndarray (float32)
         :param constraints_bounds: Vector of shape (2,)
         :type constraint_bounds: A NumPy 1-D ndarray (float32)
 
-        :raise MissingVariableError: If no variable have been added to the model.
+        :raises MissingVariableError: If no variable have been added to the model.
         :raises MaximumConstraintLimitError: The number of constraint exeed the limit.
-        :raise ValueError: If the constraint_mask shape does not fit the expected shape of this model.
-        :raise ValueError: If the constraint_mask contains irregular format ('NaN' or 'inf')
-        :raise ValueError: Lowerbound is equal or higher than the upperbound
+        :raises ValueError: If the constraint_mask shape does not fit the expected shape of this model.
+        :raises ValueError: If the constraint_mask contains irregular format ('NaN' or 'inf')
+        :raises ValueError: Lowerbound is equal or higher than the upperbound
 
         Example
         ~~~~~~~
         ..  highlight:: python
         ..  code-block:: python
-
         from titanq import Model
 
         # set up model
         ...
 
         constraint_mask = np.array([1.05, -1.1], dtype=np.float32)
         constraint_bounds = np.array([1.0, np.nan], dtype=np.float32)
 
         model.add_inequality_constraint(constraint_mask, constraint_bounds)
         """
         if constraint_mask.ndim > 1:
             raise ValueError(
                 "Cannot use add_inequality_constraint() function with a matrix, " \
-                "please use add_inequality_constraint_matrix() insead")
+                "please use add_inequality_constraint_matrix() instead")
 
         self.add_inequality_constraints_matrix(reshape_to_2d(constraint_mask), reshape_to_2d(constraint_bounds))
 
 
     def optimize(self, *, beta=[0.1], coupling_mult=0.5, timeout_in_secs=10.0, num_chains=8, num_engines=1, normalized=False):
         """
         Optimize this model.
 
         Note: All of the files used during the computation will be cleaned at the end.
 
-        :param beta: beta hyper parameter used by the backend solver.
-        :param coupling_mult: coupling_mult hyper parameter used by the backend solver.
-        :param timeout_in_secs: Maximum time (in seconds) the backend solver can take to resolve this problem.
-        :param num_chains: num_chains hyper parameter used by the backend solver.
-        :param num_engines: num_engines parameter used by the backend solver.
-        :param normalized: normalized paramater used by backend solver.
+        :param beta: ``beta`` hyper parameter used by the solver.
+        :param coupling_mult: ``coupling_mult`` hyper parameter used by the solver.
+        :param timeout_in_secs: Maximum time (in seconds) the solver can take to resolve this problem.
+        :param num_chains: ``num_chains`` hyper parameter used by the solver.
+        :param num_engines: ``num_engines`` parameter used by the solver.
+
+        :param normalized: DEPRECATED ``normalized`` parameter used by the solver, this will be removed.
+        Note: ``normalized`` should only be used when the model is only using binary or bipolar variables and does not contain any constraints
 
         For more information on how to tunes those parameters, visit the API doc at `https://docs.titanq.infinityq.io/`
 
-        :raise MissingVariableError: If no variable have been added to the model.
-        :raise MissingObjectiveError: If no variable have been added to the model.
+        :raises MissingVariableError: If no variable have been added to the model.
+        :raises MissingObjectiveError: If no variable have been added to the model.
 
         Example
         ~~~~~~~
         ..  highlight:: python
         ..  code-block:: python
+        from titanq import Model
+
         # set up model, objective and variable
         ...
 
         # basic solve
         response = model.optimize(timeout_in_secs=60)
 
         # multiple engine
```

### Comparing `titanq-0.9.0/titanq/_model/numpy_util.py` & `titanq-0.9.1/titanq/_model/numpy_util.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.0/titanq/_model/objective.py` & `titanq-0.9.1/titanq/_model/objective.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.0/titanq/_model/optimize_response.py` & `titanq-0.9.1/titanq/_model/optimize_response.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.0/titanq/_model/variable.py` & `titanq-0.9.1/titanq/_model/variable.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.0/titanq/_model/variable_list.py` & `titanq-0.9.1/titanq/_model/variable_list.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.0/titanq/_storage/managed_storage.py` & `titanq-0.9.1/titanq/_storage/managed_storage.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.0/titanq/_storage/s3_storage.py` & `titanq-0.9.1/titanq/_storage/s3_storage.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.0/titanq/_storage/storage_client.py` & `titanq-0.9.1/titanq/_storage/storage_client.py`

 * *Files identical despite different names*

### Comparing `titanq-0.9.0/titanq.egg-info/PKG-INFO` & `titanq-0.9.1/titanq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titanq
-Version: 0.9.0
+Version: 0.9.1
 Summary: The TitanQ SDK for python
 Maintainer-email: InfinityQ <support@infinityq.tech>
 License: Apache 2.0
 Project-URL: Homepage, https://www.infinityq.tech
 Project-URL: Documentation, https://docs.titanq.infinityq.io/quickstart/category/python-sdk
 Project-URL: Examples, https://github.com/infinityq-tech/titanq-examples
 Keywords: titan,titanq,optimization,platform,infinity,infinityq
```

### Comparing `titanq-0.9.0/titanq.egg-info/SOURCES.txt` & `titanq-0.9.1/titanq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

