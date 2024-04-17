# Comparing `tmp/sophia_opt-0.2.0.tar.gz` & `tmp/sophia_opt-0.2.1.tar.gz`

## Comparing `sophia_opt-0.2.0.tar` & `sophia_opt-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 sophia_opt-0.2.0/configurator.py
--rw-r--r--   0        0        0    86679 2020-02-02 00:00:00.000000 sophia_opt-0.2.0/assets/1.5B_200k_new.png
--rw-r--r--   0        0        0    93283 2020-02-02 00:00:00.000000 sophia_opt-0.2.0/assets/medium_100k_plus.png
--rw-r--r--   0        0        0    87763 2020-02-02 00:00:00.000000 sophia_opt-0.2.0/assets/small_100k_plus.png
--rw-r--r--   0        0        0    97326 2020-02-02 00:00:00.000000 sophia_opt-0.2.0/assets/t5_winrate.png
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 sophia_opt-0.2.0/config/train_gpt2_large_adam.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 sophia_opt-0.2.0/config/train_gpt2_large_sophiag.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 sophia_opt-0.2.0/config/train_gpt2_medium_adam.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 sophia_opt-0.2.0/config/train_gpt2_medium_sophiag.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 sophia_opt-0.2.0/config/train_gpt2_small_adam.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 sophia_opt-0.2.0/config/train_gpt2_small_sophiag.py
--rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 sophia_opt-0.2.0/data/openwebtext/prepare.py
--rw-r--r--   0        0        0    18489 2020-02-02 00:00:00.000000 sophia_opt-0.2.0/examples/model.py
--rw-r--r--   0        0        0    14774 2020-02-02 00:00:00.000000 sophia_opt-0.2.0/examples/train_adam.py
--rw-r--r--   0        0        0    20308 2020-02-02 00:00:00.000000 sophia_opt-0.2.0/examples/train_sophiag.py
--rw-r--r--   0        0        0     7381 2020-02-02 00:00:00.000000 sophia_opt-0.2.0/src/sophia_opt/__init__.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 sophia_opt-0.2.0/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 sophia_opt-0.2.0/LICENSE
--rw-r--r--   0        0        0     8921 2020-02-02 00:00:00.000000 sophia_opt-0.2.0/README.md
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 sophia_opt-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     9184 2020-02-02 00:00:00.000000 sophia_opt-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 sophia_opt-0.2.1/configurator.py
+-rw-r--r--   0        0        0    86679 2020-02-02 00:00:00.000000 sophia_opt-0.2.1/assets/1.5B_200k_new.png
+-rw-r--r--   0        0        0    93283 2020-02-02 00:00:00.000000 sophia_opt-0.2.1/assets/medium_100k_plus.png
+-rw-r--r--   0        0        0    87763 2020-02-02 00:00:00.000000 sophia_opt-0.2.1/assets/small_100k_plus.png
+-rw-r--r--   0        0        0    97326 2020-02-02 00:00:00.000000 sophia_opt-0.2.1/assets/t5_winrate.png
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 sophia_opt-0.2.1/config/train_gpt2_large_adam.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 sophia_opt-0.2.1/config/train_gpt2_large_sophiag.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 sophia_opt-0.2.1/config/train_gpt2_medium_adam.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 sophia_opt-0.2.1/config/train_gpt2_medium_sophiag.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 sophia_opt-0.2.1/config/train_gpt2_small_adam.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 sophia_opt-0.2.1/config/train_gpt2_small_sophiag.py
+-rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 sophia_opt-0.2.1/data/openwebtext/prepare.py
+-rw-r--r--   0        0        0    18489 2020-02-02 00:00:00.000000 sophia_opt-0.2.1/examples/model.py
+-rw-r--r--   0        0        0    14774 2020-02-02 00:00:00.000000 sophia_opt-0.2.1/examples/train_adam.py
+-rw-r--r--   0        0        0    20308 2020-02-02 00:00:00.000000 sophia_opt-0.2.1/examples/train_sophiag.py
+-rw-r--r--   0        0        0     7381 2020-02-02 00:00:00.000000 sophia_opt-0.2.1/src/sophia_opt/__init__.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 sophia_opt-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 sophia_opt-0.2.1/LICENSE
+-rw-r--r--   0        0        0     8968 2020-02-02 00:00:00.000000 sophia_opt-0.2.1/README.md
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 sophia_opt-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     9374 2020-02-02 00:00:00.000000 sophia_opt-0.2.1/PKG-INFO
```

### Comparing `sophia_opt-0.2.0/configurator.py` & `sophia_opt-0.2.1/configurator.py`

 * *Files identical despite different names*

### Comparing `sophia_opt-0.2.0/assets/1.5B_200k_new.png` & `sophia_opt-0.2.1/assets/1.5B_200k_new.png`

 * *Files identical despite different names*

### Comparing `sophia_opt-0.2.0/assets/medium_100k_plus.png` & `sophia_opt-0.2.1/assets/medium_100k_plus.png`

 * *Files identical despite different names*

### Comparing `sophia_opt-0.2.0/assets/small_100k_plus.png` & `sophia_opt-0.2.1/assets/small_100k_plus.png`

 * *Files identical despite different names*

### Comparing `sophia_opt-0.2.0/assets/t5_winrate.png` & `sophia_opt-0.2.1/assets/t5_winrate.png`

 * *Files identical despite different names*

### Comparing `sophia_opt-0.2.0/config/train_gpt2_large_adam.py` & `sophia_opt-0.2.1/config/train_gpt2_large_adam.py`

 * *Files identical despite different names*

### Comparing `sophia_opt-0.2.0/config/train_gpt2_large_sophiag.py` & `sophia_opt-0.2.1/config/train_gpt2_large_sophiag.py`

 * *Files identical despite different names*

### Comparing `sophia_opt-0.2.0/config/train_gpt2_medium_adam.py` & `sophia_opt-0.2.1/config/train_gpt2_medium_adam.py`

 * *Files identical despite different names*

### Comparing `sophia_opt-0.2.0/config/train_gpt2_medium_sophiag.py` & `sophia_opt-0.2.1/config/train_gpt2_medium_sophiag.py`

 * *Files identical despite different names*

### Comparing `sophia_opt-0.2.0/config/train_gpt2_small_adam.py` & `sophia_opt-0.2.1/config/train_gpt2_small_adam.py`

 * *Files identical despite different names*

### Comparing `sophia_opt-0.2.0/config/train_gpt2_small_sophiag.py` & `sophia_opt-0.2.1/config/train_gpt2_small_sophiag.py`

 * *Files identical despite different names*

### Comparing `sophia_opt-0.2.0/data/openwebtext/prepare.py` & `sophia_opt-0.2.1/data/openwebtext/prepare.py`

 * *Files identical despite different names*

### Comparing `sophia_opt-0.2.0/examples/model.py` & `sophia_opt-0.2.1/examples/model.py`

 * *Files identical despite different names*

### Comparing `sophia_opt-0.2.0/examples/train_adam.py` & `sophia_opt-0.2.1/examples/train_adam.py`

 * *Files identical despite different names*

### Comparing `sophia_opt-0.2.0/examples/train_sophiag.py` & `sophia_opt-0.2.1/examples/train_sophiag.py`

 * *Files identical despite different names*

### Comparing `sophia_opt-0.2.0/src/sophia_opt/__init__.py` & `sophia_opt-0.2.1/src/sophia_opt/__init__.py`

 * *Files identical despite different names*

### Comparing `sophia_opt-0.2.0/LICENSE` & `sophia_opt-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sophia_opt-0.2.0/README.md` & `sophia_opt-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 
 # sophia-opt
+
+[PyPI](https://pypi.org/project/sophia-opt/)
+
 This package is a fork of the official implementation(
 [https://github.com/Liuhong99/Sophia](https://github.com/Liuhong99/Sophia)
 ) and is simply packaged to improve ease of installation.
 
 
 ### Installation
 ```sh
```

### Comparing `sophia_opt-0.2.0/pyproject.toml` & `sophia_opt-0.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 [project]
 name = "sophia-opt"
-version = "0.2.0"
-description = "Add your description here"
+version = "0.2.1"
+description = "A community package of the official implementation of “Sophia: A Scalable Stochastic Second-order Optimizer for Language Model Pre-training”"
 authors = [
     { name = "Liuhong99" },
     { name = "fuyutarow", email = "fuyutarow@gmail.com" }
 ]
 dependencies = [
     "torch>=2",
 ]
 readme = "README.md"
 requires-python = ">= 3.8"
+homepage = "https://github.com/fuyutarow/sophia-opt"
+repository = "https://github.com/fuyutarow/sophia-opt"
+license = "MIT"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 managed = true
@@ -22,7 +25,8 @@
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/sophia_opt"]
 
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sophia_opt-0.2.0/PKG-INFO` & `sophia_opt-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.3
 Name: sophia-opt
-Version: 0.2.0
-Summary: Add your description here
+Version: 0.2.1
+Summary: A community package of the official implementation of “Sophia: A Scalable Stochastic Second-order Optimizer for Language Model Pre-training”
 Author: Liuhong99
 Author-email: fuyutarow <fuyutarow@gmail.com>
+License-Expression: MIT
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: torch>=2
 Description-Content-Type: text/markdown
 
 
 # sophia-opt
+
+[PyPI](https://pypi.org/project/sophia-opt/)
+
 This package is a fork of the official implementation(
 [https://github.com/Liuhong99/Sophia](https://github.com/Liuhong99/Sophia)
 ) and is simply packaged to improve ease of installation.
 
 
 ### Installation
 ```sh
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

