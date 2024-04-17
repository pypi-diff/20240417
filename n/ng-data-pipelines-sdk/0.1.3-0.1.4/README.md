# Comparing `tmp/ng_data_pipelines_sdk-0.1.3.tar.gz` & `tmp/ng_data_pipelines_sdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ng_data_pipelines_sdk-0.1.3.tar", max compression
+gzip compressed data, was "ng_data_pipelines_sdk-0.1.4.tar", max compression
```

## Comparing `ng_data_pipelines_sdk-0.1.3.tar` & `ng_data_pipelines_sdk-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      106 2024-04-17 03:16:33.688690 ng_data_pipelines_sdk-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-04-17 03:16:33.714690 ng_data_pipelines_sdk-0.1.3/ng_data_pipelines_sdk/__init__.py
--rw-r--r--   0        0        0     4434 2024-04-17 03:16:33.688690 ng_data_pipelines_sdk-0.1.3/ng_data_pipelines_sdk/aws_interface.py
--rw-r--r--   0        0        0      231 2024-04-17 03:16:33.688690 ng_data_pipelines_sdk-0.1.3/ng_data_pipelines_sdk/custom_logger.py
--rw-r--r--   0        0        0    24305 2024-04-17 03:16:33.688690 ng_data_pipelines_sdk-0.1.3/ng_data_pipelines_sdk/dataframe_manager.py
--rw-r--r--   0        0        0     8365 2024-04-17 03:16:33.688690 ng_data_pipelines_sdk-0.1.3/ng_data_pipelines_sdk/interfaces.py
--rw-r--r--   0        0        0     2969 2024-04-17 03:16:33.688690 ng_data_pipelines_sdk-0.1.3/ng_data_pipelines_sdk/spark_manager.py
--rw-r--r--   0        0        0     3498 2024-04-17 03:16:33.688690 ng_data_pipelines_sdk-0.1.3/ng_data_pipelines_sdk/utils.py
--rw-r--r--   0        0        0      618 2024-04-17 03:16:33.689690 ng_data_pipelines_sdk-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      106 2024-04-17 04:56:49.565763 ng_data_pipelines_sdk-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 04:56:49.590762 ng_data_pipelines_sdk-0.1.4/ng_data_pipelines_sdk/__init__.py
+-rw-r--r--   0        0        0     4434 2024-04-17 04:56:49.565763 ng_data_pipelines_sdk-0.1.4/ng_data_pipelines_sdk/aws_interface.py
+-rw-r--r--   0        0        0      231 2024-04-17 04:56:49.565763 ng_data_pipelines_sdk-0.1.4/ng_data_pipelines_sdk/custom_logger.py
+-rw-r--r--   0        0        0    24231 2024-04-17 04:56:49.566763 ng_data_pipelines_sdk-0.1.4/ng_data_pipelines_sdk/dataframe_manager.py
+-rw-r--r--   0        0        0     8365 2024-04-17 04:56:49.566763 ng_data_pipelines_sdk-0.1.4/ng_data_pipelines_sdk/interfaces.py
+-rw-r--r--   0        0        0     2969 2024-04-17 04:56:49.566763 ng_data_pipelines_sdk-0.1.4/ng_data_pipelines_sdk/spark_manager.py
+-rw-r--r--   0        0        0     3498 2024-04-17 04:56:49.566763 ng_data_pipelines_sdk-0.1.4/ng_data_pipelines_sdk/utils.py
+-rw-r--r--   0        0        0      618 2024-04-17 04:56:49.567763 ng_data_pipelines_sdk-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-0.1.4/PKG-INFO
```

### Comparing `ng_data_pipelines_sdk-0.1.3/ng_data_pipelines_sdk/aws_interface.py` & `ng_data_pipelines_sdk-0.1.4/ng_data_pipelines_sdk/aws_interface.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.1.3/ng_data_pipelines_sdk/dataframe_manager.py` & `ng_data_pipelines_sdk-0.1.4/ng_data_pipelines_sdk/dataframe_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-import os
 from datetime import datetime, timedelta
 from typing import Any, Dict, List, Optional, Union
 
 from pyspark.sql import DataFrame
 from pyspark.sql.functions import lit
 from pyspark.sql.types import StructType
 
@@ -28,17 +27,15 @@
 )
 from ng_data_pipelines_sdk.custom_logger import logger
 from ng_data_pipelines_sdk.spark_manager import SparkManager
 from ng_data_pipelines_sdk.utils import (
     handle_pyspark_timestamp_in_schema,
 )
 
-logger.setLevel("DEBUG")
-
-CURRENT_FILE_DIR = os.path.dirname(os.path.abspath(__file__))
+logger.setLevel("INFO")
 
 
 class DataFrameManager:
     def __init__(
         self,
         file_system: str,
         aws_interface: AWSInterface,
```

### Comparing `ng_data_pipelines_sdk-0.1.3/ng_data_pipelines_sdk/interfaces.py` & `ng_data_pipelines_sdk-0.1.4/ng_data_pipelines_sdk/interfaces.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.1.3/ng_data_pipelines_sdk/spark_manager.py` & `ng_data_pipelines_sdk-0.1.4/ng_data_pipelines_sdk/spark_manager.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.1.3/ng_data_pipelines_sdk/utils.py` & `ng_data_pipelines_sdk-0.1.4/ng_data_pipelines_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.1.3/pyproject.toml` & `ng_data_pipelines_sdk-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ng-data-pipelines-sdk"
-version = "0.1.3"
+version = "0.1.4"
 description = "A library for facilitating the development of data engineering pipelines using pyspark"
 authors = ["ng.cash"]
 readme = "README.md"
 exclude = [".git/", ".gitignore", "tests/", "docs/", "*.yml", "__pycache__/", "*.pyc", "*.ipynb", "playground/", "poetry.lock", "dist/", "build/"]
 
 [tool.poetry.dependencies]
 python = "~3.9"
```

### Comparing `ng_data_pipelines_sdk-0.1.3/PKG-INFO` & `ng_data_pipelines_sdk-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ng-data-pipelines-sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: A library for facilitating the development of data engineering pipelines using pyspark
 Author: ng.cash
 Requires-Python: >=3.9,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: boto3 (>=1.34.84,<2.0.0)
 Requires-Dist: pydantic (>=2.7.0,<3.0.0)
```

