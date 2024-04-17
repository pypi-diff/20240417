# Comparing `tmp/ng_data_pipelines_sdk-0.1.2.tar.gz` & `tmp/ng_data_pipelines_sdk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ng_data_pipelines_sdk-0.1.2.tar", max compression
+gzip compressed data, was "ng_data_pipelines_sdk-0.1.3.tar", max compression
```

## Comparing `ng_data_pipelines_sdk-0.1.2.tar` & `ng_data_pipelines_sdk-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      106 2024-04-16 22:58:49.033258 ng_data_pipelines_sdk-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-04-16 22:58:49.057258 ng_data_pipelines_sdk-0.1.2/ng_data_pipelines_sdk/__init__.py
--rw-r--r--   0        0        0     4434 2024-04-16 22:58:49.034258 ng_data_pipelines_sdk-0.1.2/ng_data_pipelines_sdk/aws_interface.py
--rw-r--r--   0        0        0      231 2024-04-16 22:58:49.034258 ng_data_pipelines_sdk-0.1.2/ng_data_pipelines_sdk/custom_logger.py
--rw-r--r--   0        0        0    24305 2024-04-16 22:58:49.035258 ng_data_pipelines_sdk-0.1.2/ng_data_pipelines_sdk/dataframe_manager.py
--rw-r--r--   0        0        0     8365 2024-04-16 22:58:49.035258 ng_data_pipelines_sdk-0.1.2/ng_data_pipelines_sdk/interfaces.py
--rw-r--r--   0        0        0     2969 2024-04-16 22:58:49.035258 ng_data_pipelines_sdk-0.1.2/ng_data_pipelines_sdk/spark_manager.py
--rw-r--r--   0        0        0     3498 2024-04-16 22:58:49.035258 ng_data_pipelines_sdk-0.1.2/ng_data_pipelines_sdk/utils.py
--rw-r--r--   0        0        0      619 2024-04-16 22:58:49.035258 ng_data_pipelines_sdk-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      573 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      106 2024-04-17 03:16:33.688690 ng_data_pipelines_sdk-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 03:16:33.714690 ng_data_pipelines_sdk-0.1.3/ng_data_pipelines_sdk/__init__.py
+-rw-r--r--   0        0        0     4434 2024-04-17 03:16:33.688690 ng_data_pipelines_sdk-0.1.3/ng_data_pipelines_sdk/aws_interface.py
+-rw-r--r--   0        0        0      231 2024-04-17 03:16:33.688690 ng_data_pipelines_sdk-0.1.3/ng_data_pipelines_sdk/custom_logger.py
+-rw-r--r--   0        0        0    24305 2024-04-17 03:16:33.688690 ng_data_pipelines_sdk-0.1.3/ng_data_pipelines_sdk/dataframe_manager.py
+-rw-r--r--   0        0        0     8365 2024-04-17 03:16:33.688690 ng_data_pipelines_sdk-0.1.3/ng_data_pipelines_sdk/interfaces.py
+-rw-r--r--   0        0        0     2969 2024-04-17 03:16:33.688690 ng_data_pipelines_sdk-0.1.3/ng_data_pipelines_sdk/spark_manager.py
+-rw-r--r--   0        0        0     3498 2024-04-17 03:16:33.688690 ng_data_pipelines_sdk-0.1.3/ng_data_pipelines_sdk/utils.py
+-rw-r--r--   0        0        0      618 2024-04-17 03:16:33.689690 ng_data_pipelines_sdk-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-0.1.3/PKG-INFO
```

### Comparing `ng_data_pipelines_sdk-0.1.2/ng_data_pipelines_sdk/aws_interface.py` & `ng_data_pipelines_sdk-0.1.3/ng_data_pipelines_sdk/aws_interface.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.1.2/ng_data_pipelines_sdk/dataframe_manager.py` & `ng_data_pipelines_sdk-0.1.3/ng_data_pipelines_sdk/dataframe_manager.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.1.2/ng_data_pipelines_sdk/interfaces.py` & `ng_data_pipelines_sdk-0.1.3/ng_data_pipelines_sdk/interfaces.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.1.2/ng_data_pipelines_sdk/spark_manager.py` & `ng_data_pipelines_sdk-0.1.3/ng_data_pipelines_sdk/spark_manager.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.1.2/ng_data_pipelines_sdk/utils.py` & `ng_data_pipelines_sdk-0.1.3/ng_data_pipelines_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.1.2/pyproject.toml` & `ng_data_pipelines_sdk-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "ng-data-pipelines-sdk"
-version = "0.1.2"
+version = "0.1.3"
 description = "A library for facilitating the development of data engineering pipelines using pyspark"
 authors = ["ng.cash"]
 readme = "README.md"
 exclude = [".git/", ".gitignore", "tests/", "docs/", "*.yml", "__pycache__/", "*.pyc", "*.ipynb", "playground/", "poetry.lock", "dist/", "build/"]
 
 [tool.poetry.dependencies]
 python = "~3.9"
-pyspark = "~3.5.0"
+pyspark = "3.2.0"
 pydantic = "^2.7.0"
 boto3 = "^1.34.84"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.29.4"
 ruff = "^0.3.7"
```

### Comparing `ng_data_pipelines_sdk-0.1.2/PKG-INFO` & `ng_data_pipelines_sdk-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ng-data-pipelines-sdk
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library for facilitating the development of data engineering pipelines using pyspark
 Author: ng.cash
 Requires-Python: >=3.9,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: boto3 (>=1.34.84,<2.0.0)
 Requires-Dist: pydantic (>=2.7.0,<3.0.0)
-Requires-Dist: pyspark (>=3.5.0,<3.6.0)
+Requires-Dist: pyspark (==3.2.0)
 Description-Content-Type: text/markdown
 
 docker run --rm -it -d -e PYTHONPATH="/ng-data-pipelines-sdk" -v $pwd:/ng-data-pipelines-sdk pyspark-local
```

