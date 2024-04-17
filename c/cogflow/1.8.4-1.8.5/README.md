# Comparing `tmp/cogflow-1.8.4.tar.gz` & `tmp/cogflow-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cogflow-1.8.4.tar", last modified: Wed Apr 17 15:12:09 2024, max compression
+gzip compressed data, was "cogflow-1.8.5.tar", last modified: Wed Apr 17 15:29:14 2024, max compression
```

## Comparing `cogflow-1.8.4.tar` & `cogflow-1.8.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 15:12:09.902510 cogflow-1.8.4/
--rw-rw-rw-   0        0        0      401 2024-04-17 15:12:09.895599 cogflow-1.8.4/PKG-INFO
--rw-rw-rw-   0        0        0     4024 2024-04-15 10:04:49.000000 cogflow-1.8.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 15:12:09.857969 cogflow-1.8.4/cogflow/
--rw-rw-rw-   0        0        0      725 2024-04-17 14:53:14.000000 cogflow-1.8.4/cogflow/__init__.py
--rw-rw-rw-   0        0        0     5088 2024-04-16 13:26:15.000000 cogflow-1.8.4/cogflow/dataset_plugin.py
--rw-rw-rw-   0        0        0     8946 2024-04-17 14:52:41.000000 cogflow-1.8.4/cogflow/kubeflowplugin.py
--rw-rw-rw-   0        0        0    11094 2024-04-17 14:52:41.000000 cogflow-1.8.4/cogflow/mlflowplugin.py
--rw-rw-rw-   0        0        0      714 2024-04-17 14:53:54.000000 cogflow-1.8.4/cogflow/plugin_config.py
--rw-rw-rw-   0        0        0      620 2024-04-15 10:04:49.000000 cogflow-1.8.4/cogflow/plugin_status.py
--rw-rw-rw-   0        0        0      174 2024-04-15 10:04:49.000000 cogflow-1.8.4/cogflow/pluginerrors.py
--rw-rw-rw-   0        0        0     5447 2024-04-17 14:53:54.000000 cogflow-1.8.4/cogflow/pluginmanager.py
-drwxrwxrwx   0        0        0        0 2024-04-17 15:12:09.890900 cogflow-1.8.4/cogflow.egg-info/
--rw-rw-rw-   0        0        0      401 2024-04-17 15:12:09.000000 cogflow-1.8.4/cogflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2024-04-17 15:12:09.000000 cogflow-1.8.4/cogflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 15:12:09.000000 cogflow-1.8.4/cogflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      214 2024-04-17 15:12:09.000000 cogflow-1.8.4/cogflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-17 15:12:09.000000 cogflow-1.8.4/cogflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 15:12:09.902564 cogflow-1.8.4/setup.cfg
--rw-rw-rw-   0        0        0     1594 2024-04-17 15:12:04.000000 cogflow-1.8.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 15:29:14.235496 cogflow-1.8.5/
+-rw-rw-rw-   0        0        0      401 2024-04-17 15:29:14.231198 cogflow-1.8.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4024 2024-04-15 10:04:49.000000 cogflow-1.8.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 15:29:14.205387 cogflow-1.8.5/cogflow/
+-rw-rw-rw-   0        0        0      757 2024-04-17 15:25:52.000000 cogflow-1.8.5/cogflow/__init__.py
+-rw-rw-rw-   0        0        0     5088 2024-04-16 13:26:15.000000 cogflow-1.8.5/cogflow/dataset_plugin.py
+-rw-rw-rw-   0        0        0     8959 2024-04-17 15:27:00.000000 cogflow-1.8.5/cogflow/kubeflowplugin.py
+-rw-rw-rw-   0        0        0    11107 2024-04-17 15:27:24.000000 cogflow-1.8.5/cogflow/mlflowplugin.py
+-rw-rw-rw-   0        0        0      714 2024-04-17 14:53:54.000000 cogflow-1.8.5/cogflow/plugin_config.py
+-rw-rw-rw-   0        0        0      620 2024-04-15 10:04:49.000000 cogflow-1.8.5/cogflow/plugin_status.py
+-rw-rw-rw-   0        0        0      174 2024-04-15 10:04:49.000000 cogflow-1.8.5/cogflow/pluginerrors.py
+-rw-rw-rw-   0        0        0     5494 2024-04-17 15:28:19.000000 cogflow-1.8.5/cogflow/pluginmanager.py
+drwxrwxrwx   0        0        0        0 2024-04-17 15:29:14.228969 cogflow-1.8.5/cogflow.egg-info/
+-rw-rw-rw-   0        0        0      401 2024-04-17 15:29:13.000000 cogflow-1.8.5/cogflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2024-04-17 15:29:14.000000 cogflow-1.8.5/cogflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 15:29:13.000000 cogflow-1.8.5/cogflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      214 2024-04-17 15:29:13.000000 cogflow-1.8.5/cogflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-17 15:29:13.000000 cogflow-1.8.5/cogflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 15:29:14.235496 cogflow-1.8.5/setup.cfg
+-rw-rw-rw-   0        0        0     1594 2024-04-17 15:28:58.000000 cogflow-1.8.5/setup.py
```

### Comparing `cogflow-1.8.4/README.md` & `cogflow-1.8.5/README.md`

 * *Files identical despite different names*

### Comparing `cogflow-1.8.4/cogflow/__init__.py` & `cogflow-1.8.5/cogflow/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,18 +6,18 @@
     TIMER_IN_SEC (int): Timer interval in seconds.
     ML_TOOL (str): Machine learning tool being used.
     ACCESS_KEY_ID (str): Access key ID for authentication.
     SECRET_ACCESS_KEY (str): Secret access key for authentication.
     S3_ENDPOINT_URL (str): Endpoint URL for Amazon S3.
 """
 
-from plugin_config import (
+from cogflow.plugin_config import (
     TRACKING_URI,
     TIMER_IN_SEC,
     ML_TOOL,
     ACCESS_KEY_ID,
     SECRET_ACCESS_KEY,
     S3_ENDPOINT_URL,
 )
-from plugin_status import plugin_statuses
-from pluginerrors import PluginErrors
-from pluginmanager import PluginManager
+from cogflow.plugin_status import plugin_statuses
+from cogflow.pluginerrors import PluginErrors
+from cogflow.pluginmanager import PluginManager
```

### Comparing `cogflow-1.8.4/cogflow/dataset_plugin.py` & `cogflow-1.8.5/cogflow/dataset_plugin.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.8.4/cogflow/kubeflowplugin.py` & `cogflow-1.8.5/cogflow/kubeflowplugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     V1beta1SKLearnSpec,
     constants,
     utils,
 )
 from kubernetes import client
 from kubernetes.client import V1ObjectMeta
 from kubernetes.client.models import V1EnvVar
-import plugin_config
+from cogflow import plugin_config
 
 
 class CogContainer(kfp.dsl._container_op.Container):
     """
     Subclass of Container to add model access environment variables.
     """
```

### Comparing `cogflow-1.8.4/cogflow/mlflowplugin.py` & `cogflow-1.8.5/cogflow/mlflowplugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import numpy as np
 import pandas as pd
 import requests
 from mlflow.models.signature import ModelSignature
 from mlflow.tracking import MlflowClient
 from scipy.sparse import csr_matrix, csc_matrix
 
-import plugin_config
+from cogflow import plugin_config
 
 
 class CogModel(ml.pyfunc.PythonModel):
     """
     A custom Mlflow PythonModel implementation for demonstration purposes.
     """
```

### Comparing `cogflow-1.8.4/cogflow/plugin_config.py` & `cogflow-1.8.5/cogflow/plugin_config.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.8.4/cogflow/plugin_status.py` & `cogflow-1.8.5/cogflow/plugin_status.py`

 * *Files identical despite different names*

### Comparing `cogflow-1.8.4/cogflow/pluginmanager.py` & `cogflow-1.8.5/cogflow/pluginmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 Attributes:
     mlplugin (class): The Mlflow plugin class.
     kfplugin (class): The Kubeflow plugin class.
     dsplugin (class): The Dataset plugin class.
 """
 
 import importlib
-from kubeflowplugin import KubeflowPlugin
-from mlflowplugin import MlflowPlugin
-from dataset_plugin import DatasetPlugin
-import plugin_status
-from plugin_status import plugin_statuses
+from cogflow.kubeflowplugin import KubeflowPlugin
+from cogflow.mlflowplugin import MlflowPlugin
+from cogflow.dataset_plugin import DatasetPlugin
+from cogflow import plugin_status
+from cogflow.plugin_status import plugin_statuses
+
 
 
 class PluginManager:
     """
     Class responsible for managing plugins.
 
     Attributes:
```

### Comparing `cogflow-1.8.4/setup.py` & `cogflow-1.8.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 """
 
 from setuptools import setup, find_packages
 
 setup(
     name="cogflow",
-    version="1.8.4",
+    version="1.8.5",
     author="Sai_kireeti",
     author_email="sai.kireeti@hiro-microdatacenters.nl",
     description="cog modules",
     packages=find_packages(),
     install_requires=[
         "mlflow==2.10.2",
         "kfp==1.8.22",
```

