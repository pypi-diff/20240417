# Comparing `tmp/ng_data_pipelines_sdk-0.1.5.tar.gz` & `tmp/ng_data_pipelines_sdk-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ng_data_pipelines_sdk-0.1.5.tar", max compression
+gzip compressed data, was "ng_data_pipelines_sdk-0.1.6.tar", max compression
```

## Comparing `ng_data_pipelines_sdk-0.1.5.tar` & `ng_data_pipelines_sdk-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      106 2024-04-17 15:37:58.380710 ng_data_pipelines_sdk-0.1.5/README.md
--rw-r--r--   0        0        0        0 2024-04-17 15:37:58.406710 ng_data_pipelines_sdk-0.1.5/ng_data_pipelines_sdk/__init__.py
--rw-r--r--   0        0        0     4434 2024-04-17 15:37:58.380710 ng_data_pipelines_sdk-0.1.5/ng_data_pipelines_sdk/aws_interface.py
--rw-r--r--   0        0        0      231 2024-04-17 15:37:58.380710 ng_data_pipelines_sdk-0.1.5/ng_data_pipelines_sdk/custom_logger.py
--rw-r--r--   0        0        0    24231 2024-04-17 15:37:58.380710 ng_data_pipelines_sdk-0.1.5/ng_data_pipelines_sdk/dataframe_manager.py
--rw-r--r--   0        0        0     8365 2024-04-17 15:37:58.380710 ng_data_pipelines_sdk-0.1.5/ng_data_pipelines_sdk/interfaces.py
--rw-r--r--   0        0        0     2969 2024-04-17 15:37:58.380710 ng_data_pipelines_sdk-0.1.5/ng_data_pipelines_sdk/spark_manager.py
--rw-r--r--   0        0        0     3498 2024-04-17 15:37:58.380710 ng_data_pipelines_sdk-0.1.5/ng_data_pipelines_sdk/utils.py
--rw-r--r--   0        0        0      626 2024-04-17 15:37:58.382711 ng_data_pipelines_sdk-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      668 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      106 2024-04-17 15:54:49.104810 ng_data_pipelines_sdk-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 15:54:49.129810 ng_data_pipelines_sdk-0.1.6/ng_data_pipelines_sdk/__init__.py
+-rw-r--r--   0        0        0     4434 2024-04-17 15:54:49.104810 ng_data_pipelines_sdk-0.1.6/ng_data_pipelines_sdk/aws_interface.py
+-rw-r--r--   0        0        0      231 2024-04-17 15:54:49.104810 ng_data_pipelines_sdk-0.1.6/ng_data_pipelines_sdk/custom_logger.py
+-rw-r--r--   0        0        0    24231 2024-04-17 15:54:49.104810 ng_data_pipelines_sdk-0.1.6/ng_data_pipelines_sdk/dataframe_manager.py
+-rw-r--r--   0        0        0     8365 2024-04-17 15:54:49.105810 ng_data_pipelines_sdk-0.1.6/ng_data_pipelines_sdk/interfaces.py
+-rw-r--r--   0        0        0     2969 2024-04-17 15:54:49.105810 ng_data_pipelines_sdk-0.1.6/ng_data_pipelines_sdk/spark_manager.py
+-rw-r--r--   0        0        0     3498 2024-04-17 15:54:49.105810 ng_data_pipelines_sdk-0.1.6/ng_data_pipelines_sdk/utils.py
+-rw-r--r--   0        0        0      626 2024-04-17 15:54:49.106810 ng_data_pipelines_sdk-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      668 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-0.1.6/PKG-INFO
```

### Comparing `ng_data_pipelines_sdk-0.1.5/ng_data_pipelines_sdk/aws_interface.py` & `ng_data_pipelines_sdk-0.1.6/ng_data_pipelines_sdk/aws_interface.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.1.5/ng_data_pipelines_sdk/dataframe_manager.py` & `ng_data_pipelines_sdk-0.1.6/ng_data_pipelines_sdk/dataframe_manager.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.1.5/ng_data_pipelines_sdk/interfaces.py` & `ng_data_pipelines_sdk-0.1.6/ng_data_pipelines_sdk/interfaces.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.1.5/ng_data_pipelines_sdk/spark_manager.py` & `ng_data_pipelines_sdk-0.1.6/ng_data_pipelines_sdk/spark_manager.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.1.5/ng_data_pipelines_sdk/utils.py` & `ng_data_pipelines_sdk-0.1.6/ng_data_pipelines_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.1.5/pyproject.toml` & `ng_data_pipelines_sdk-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "ng-data-pipelines-sdk"
-version = "0.1.5"
+version = "0.1.6"
 description = "A library for facilitating the development of data engineering pipelines using pyspark"
 authors = ["ng.cash"]
 readme = "README.md"
 exclude = [".git/", ".gitignore", "tests/", "docs/", "*.yml", "__pycache__/", "*.pyc", "*.ipynb", "playground/", "poetry.lock", "dist/", "build/"]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
 pyspark = "3.2.0"
 pydantic = "^2.7.0"
-boto3 = "^1.34.84"
+boto3 = "^1.33.13"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.29.4"
 ruff = "^0.3.7"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `ng_data_pipelines_sdk-0.1.5/PKG-INFO` & `ng_data_pipelines_sdk-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ng-data-pipelines-sdk
-Version: 0.1.5
+Version: 0.1.6
 Summary: A library for facilitating the development of data engineering pipelines using pyspark
 Author: ng.cash
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: boto3 (>=1.34.84,<2.0.0)
+Requires-Dist: boto3 (>=1.33.13,<2.0.0)
 Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Requires-Dist: pyspark (==3.2.0)
 Description-Content-Type: text/markdown
 
 docker run --rm -it -d -e PYTHONPATH="/ng-data-pipelines-sdk" -v $pwd:/ng-data-pipelines-sdk pyspark-local
```

