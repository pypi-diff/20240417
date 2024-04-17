# Comparing `tmp/databricks_labs_pylint-0.1.0.tar.gz` & `tmp/databricks_labs_pylint-0.1.1.tar.gz`

## Comparing `databricks_labs_pylint-0.1.0.tar` & `databricks_labs_pylint-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/databricks/__init__.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/databricks/labs/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/databricks/labs/pylint/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/databricks/labs/pylint/__init__.py
--rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/databricks/labs/pylint/airflow.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/databricks/labs/pylint/all.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/databricks/labs/pylint/cli.py
--rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/databricks/labs/pylint/dbutils.py
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/databricks/labs/pylint/legacy.py
--rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/databricks/labs/pylint/mocking.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/databricks/labs/pylint/notebooks.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/databricks/labs/pylint/spark.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/.gitignore
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/LICENSE
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/NOTICE
--rw-r--r--   0        0        0    15833 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/README.md
--rw-r--r--   0        0        0    26402 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    16845 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/databricks/__init__.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/databricks/labs/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/databricks/labs/pylint/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/databricks/labs/pylint/__init__.py
+-rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/databricks/labs/pylint/airflow.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/databricks/labs/pylint/all.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/databricks/labs/pylint/cli.py
+-rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/databricks/labs/pylint/dbutils.py
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/databricks/labs/pylint/legacy.py
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/databricks/labs/pylint/mocking.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/databricks/labs/pylint/notebooks.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/databricks/labs/pylint/spark.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/.gitignore
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/LICENSE
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/NOTICE
+-rw-r--r--   0        0        0    16007 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/README.md
+-rw-r--r--   0        0        0    26416 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    17033 2020-02-02 00:00:00.000000 databricks_labs_pylint-0.1.1/PKG-INFO
```

### Comparing `databricks_labs_pylint-0.1.0/databricks/labs/pylint/airflow.py` & `databricks_labs_pylint-0.1.1/databricks/labs/pylint/airflow.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.1.0/databricks/labs/pylint/all.py` & `databricks_labs_pylint-0.1.1/databricks/labs/pylint/all.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.1.0/databricks/labs/pylint/cli.py` & `databricks_labs_pylint-0.1.1/databricks/labs/pylint/cli.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.1.0/databricks/labs/pylint/dbutils.py` & `databricks_labs_pylint-0.1.1/databricks/labs/pylint/dbutils.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.1.0/databricks/labs/pylint/legacy.py` & `databricks_labs_pylint-0.1.1/databricks/labs/pylint/legacy.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.1.0/databricks/labs/pylint/mocking.py` & `databricks_labs_pylint-0.1.1/databricks/labs/pylint/mocking.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.1.0/databricks/labs/pylint/notebooks.py` & `databricks_labs_pylint-0.1.1/databricks/labs/pylint/notebooks.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.1.0/databricks/labs/pylint/spark.py` & `databricks_labs_pylint-0.1.1/databricks/labs/pylint/spark.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.1.0/.gitignore` & `databricks_labs_pylint-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.1.0/LICENSE` & `databricks_labs_pylint-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.1.0/NOTICE` & `databricks_labs_pylint-0.1.1/NOTICE`

 * *Files identical despite different names*

### Comparing `databricks_labs_pylint-0.1.0/README.md` & `databricks_labs_pylint-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -36,24 +36,27 @@
   * [`databricks-notebooks` checker](#databricks-notebooks-checker)
     * [`C8913`: `notebooks-too-many-cells`](#c8913-notebooks-too-many-cells)
     * [`R8914`: `notebooks-percent-run`](#r8914-notebooks-percent-run)
   * [`spark` checker](#spark-checker)
     * [`C8915`: `spark-outside-function`](#c8915-spark-outside-function)
     * [`C8917`: `use-display-instead-of-show`](#c8917-use-display-instead-of-show)
     * [`W8916`: `no-spark-argument-in-function`](#w8916-no-spark-argument-in-function)
+  * [`mocking` checker](#mocking-checker)
+    * [`R8918`: `explicit-dependency-required`](#r8918-explicit-dependency-required)
+    * [`R8919`: `obscure-mock`](#r8919-obscure-mock)
   * [Testing in isolation](#testing-in-isolation)
 * [Project Support](#project-support)
 <!-- TOC -->
 
 # Installation as PyLint plugin
 
 You can install this project via `pip`:
 
 ```bash
-pip install pylint-plugin-for-databricks
+pip install databricks-labs-pylint
 ```
 
 and then use it with `pylint`:
 
 ```bash
 pylint --load-plugins=databricks.labs.pylint.all <your-python-file>.py
 ```
```

### Comparing `databricks_labs_pylint-0.1.0/pyproject.toml` & `databricks_labs_pylint-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,16 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
 dependencies = ["pylint", "astroid", "databricks-sdk"]
 
 [project.urls]
-Issues = "https://github.com/databrickslabs/pylint/issues"
-Source = "https://github.com/databrickslabs/pylint"
+Issues = "https://github.com/databrickslabs/pylint-plugin/issues"
+Source = "https://github.com/databrickslabs/pylint-plugin"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build]
 sources = ["src"]
```

### Comparing `databricks_labs_pylint-0.1.0/PKG-INFO` & `databricks_labs_pylint-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.3
 Name: databricks-labs-pylint
-Version: 0.1.0
+Version: 0.1.1
 Summary: Plugin for PyLint to support Databricks specific code patterns and best practices.
-Project-URL: Issues, https://github.com/databrickslabs/pylint/issues
-Project-URL: Source, https://github.com/databrickslabs/pylint
+Project-URL: Issues, https://github.com/databrickslabs/pylint-plugin/issues
+Project-URL: Source, https://github.com/databrickslabs/pylint-plugin
 Author-email: Serge Smertin <serge.smertin@databricks.com>
 License-File: LICENSE
 License-File: NOTICE
 Keywords: Databricks
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
@@ -61,24 +61,27 @@
   * [`databricks-notebooks` checker](#databricks-notebooks-checker)
     * [`C8913`: `notebooks-too-many-cells`](#c8913-notebooks-too-many-cells)
     * [`R8914`: `notebooks-percent-run`](#r8914-notebooks-percent-run)
   * [`spark` checker](#spark-checker)
     * [`C8915`: `spark-outside-function`](#c8915-spark-outside-function)
     * [`C8917`: `use-display-instead-of-show`](#c8917-use-display-instead-of-show)
     * [`W8916`: `no-spark-argument-in-function`](#w8916-no-spark-argument-in-function)
+  * [`mocking` checker](#mocking-checker)
+    * [`R8918`: `explicit-dependency-required`](#r8918-explicit-dependency-required)
+    * [`R8919`: `obscure-mock`](#r8919-obscure-mock)
   * [Testing in isolation](#testing-in-isolation)
 * [Project Support](#project-support)
 <!-- TOC -->
 
 # Installation as PyLint plugin
 
 You can install this project via `pip`:
 
 ```bash
-pip install pylint-plugin-for-databricks
+pip install databricks-labs-pylint
 ```
 
 and then use it with `pylint`:
 
 ```bash
 pylint --load-plugins=databricks.labs.pylint.all <your-python-file>.py
 ```
```

