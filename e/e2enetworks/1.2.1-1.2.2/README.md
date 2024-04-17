# Comparing `tmp/e2enetworks-1.2.1.tar.gz` & `tmp/e2enetworks-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2enetworks-1.2.1.tar", last modified: Mon Apr 15 09:56:06 2024, max compression
+gzip compressed data, was "e2enetworks-1.2.2.tar", last modified: Wed Apr 17 10:20:46 2024, max compression
```

## Comparing `e2enetworks-1.2.1.tar` & `e2enetworks-1.2.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-04-15 09:56:06.282729 e2enetworks-1.2.1/
--rw-r--r--   0 jagga      (501) staff       (20)    10786 2024-04-15 09:47:56.000000 e2enetworks-1.2.1/LICENSE.txt
--rw-r--r--   0 jagga      (501) staff       (20)     1207 2024-04-15 09:56:06.282625 e2enetworks-1.2.1/PKG-INFO
--rw-r--r--   0 jagga      (501) staff       (20)        0 2024-04-15 09:47:56.000000 e2enetworks-1.2.1/README.rst
-drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-04-15 09:56:06.278804 e2enetworks-1.2.1/e2enetworks/
--rw-r--r--   0 jagga      (501) staff       (20)        0 2024-04-15 09:47:56.000000 e2enetworks-1.2.1/e2enetworks/__init__.py
-drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-04-15 09:56:06.279585 e2enetworks-1.2.1/e2enetworks/cloud/
--rw-r--r--   0 jagga      (501) staff       (20)        0 2024-04-15 09:47:56.000000 e2enetworks-1.2.1/e2enetworks/cloud/__init__.py
--rw-r--r--   0 jagga      (501) staff       (20)      147 2024-04-15 09:47:56.000000 e2enetworks-1.2.1/e2enetworks/cloud/test.py
-drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-04-15 09:56:06.282465 e2enetworks-1.2.1/e2enetworks/cloud/tir/
--rw-r--r--   0 jagga      (501) staff       (20)     2290 2024-04-15 09:47:56.000000 e2enetworks-1.2.1/e2enetworks/cloud/tir/__init__.py
--rw-r--r--   0 jagga      (501) staff       (20)     9296 2024-04-15 09:47:56.000000 e2enetworks-1.2.1/e2enetworks/cloud/tir/api_client.py
--rw-r--r--   0 jagga      (501) staff       (20)     2794 2024-04-15 09:47:56.000000 e2enetworks-1.2.1/e2enetworks/cloud/tir/apitoken.py
--rw-r--r--   0 jagga      (501) staff       (20)     9405 2024-04-15 09:47:56.000000 e2enetworks-1.2.1/e2enetworks/cloud/tir/client.py
--rw-r--r--   0 jagga      (501) staff       (20)     7401 2024-04-15 09:47:56.000000 e2enetworks-1.2.1/e2enetworks/cloud/tir/constants.py
--rw-r--r--   0 jagga      (501) staff       (20)     5788 2024-04-15 09:47:56.000000 e2enetworks-1.2.1/e2enetworks/cloud/tir/datasets.py
--rw-r--r--   0 jagga      (501) staff       (20)    13823 2024-04-15 09:47:56.000000 e2enetworks-1.2.1/e2enetworks/cloud/tir/endpoints.py
--rw-r--r--   0 jagga      (501) staff       (20)     2573 2024-04-15 09:47:56.000000 e2enetworks-1.2.1/e2enetworks/cloud/tir/helpers.py
--rw-r--r--   0 jagga      (501) staff       (20)     1368 2024-04-15 09:47:56.000000 e2enetworks-1.2.1/e2enetworks/cloud/tir/images.py
--rw-r--r--   0 jagga      (501) staff       (20)     2105 2024-04-15 09:47:56.000000 e2enetworks-1.2.1/e2enetworks/cloud/tir/minio_service.py
--rw-r--r--   0 jagga      (501) staff       (20)     6455 2024-04-15 09:47:56.000000 e2enetworks-1.2.1/e2enetworks/cloud/tir/models.py
--rw-r--r--   0 jagga      (501) staff       (20)     6022 2024-04-15 09:47:56.000000 e2enetworks-1.2.1/e2enetworks/cloud/tir/notebook.py
--rw-r--r--   0 jagga      (501) staff       (20)     9999 2024-04-15 09:47:56.000000 e2enetworks-1.2.1/e2enetworks/cloud/tir/pipelines.py
--rw-r--r--   0 jagga      (501) staff       (20)     2849 2024-04-15 09:47:56.000000 e2enetworks-1.2.1/e2enetworks/cloud/tir/projects.py
--rw-r--r--   0 jagga      (501) staff       (20)     4268 2024-04-15 09:47:56.000000 e2enetworks-1.2.1/e2enetworks/cloud/tir/skus.py
--rw-r--r--   0 jagga      (501) staff       (20)     2391 2024-04-15 09:47:56.000000 e2enetworks-1.2.1/e2enetworks/cloud/tir/teams.py
--rw-r--r--   0 jagga      (501) staff       (20)     1159 2024-04-15 09:47:56.000000 e2enetworks-1.2.1/e2enetworks/cloud/tir/utils.py
--rw-r--r--   0 jagga      (501) staff       (20)       23 2024-04-15 09:47:56.000000 e2enetworks-1.2.1/e2enetworks/cloud/tir/version.py
--rw-r--r--   0 jagga      (501) staff       (20)     1517 2024-04-15 09:47:56.000000 e2enetworks-1.2.1/e2enetworks/constants.py
-drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-04-15 09:56:06.279362 e2enetworks-1.2.1/e2enetworks.egg-info/
--rw-r--r--   0 jagga      (501) staff       (20)     1207 2024-04-15 09:56:06.000000 e2enetworks-1.2.1/e2enetworks.egg-info/PKG-INFO
--rw-r--r--   0 jagga      (501) staff       (20)      914 2024-04-15 09:56:06.000000 e2enetworks-1.2.1/e2enetworks.egg-info/SOURCES.txt
--rw-r--r--   0 jagga      (501) staff       (20)        1 2024-04-15 09:56:06.000000 e2enetworks-1.2.1/e2enetworks.egg-info/dependency_links.txt
--rw-r--r--   0 jagga      (501) staff       (20)      138 2024-04-15 09:56:06.000000 e2enetworks-1.2.1/e2enetworks.egg-info/requires.txt
--rw-r--r--   0 jagga      (501) staff       (20)       12 2024-04-15 09:56:06.000000 e2enetworks-1.2.1/e2enetworks.egg-info/top_level.txt
--rw-r--r--   0 jagga      (501) staff       (20)       38 2024-04-15 09:56:06.282774 e2enetworks-1.2.1/setup.cfg
--rw-r--r--   0 jagga      (501) staff       (20)     1829 2024-04-15 09:55:55.000000 e2enetworks-1.2.1/setup.py
+drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-04-17 10:20:46.289658 e2enetworks-1.2.2/
+-rw-r--r--   0 jagga      (501) staff       (20)    10786 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/LICENSE.txt
+-rw-r--r--   0 jagga      (501) staff       (20)     1418 2024-04-17 10:20:46.289445 e2enetworks-1.2.2/PKG-INFO
+-rw-r--r--   0 jagga      (501) staff       (20)        0 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/README.rst
+drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-04-17 10:20:46.284177 e2enetworks-1.2.2/e2enetworks/
+-rw-r--r--   0 jagga      (501) staff       (20)        0 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/__init__.py
+drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-04-17 10:20:46.285296 e2enetworks-1.2.2/e2enetworks/cloud/
+-rw-r--r--   0 jagga      (501) staff       (20)        0 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/__init__.py
+-rw-r--r--   0 jagga      (501) staff       (20)      147 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/test.py
+drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-04-17 10:20:46.288985 e2enetworks-1.2.2/e2enetworks/cloud/tir/
+-rw-r--r--   0 jagga      (501) staff       (20)     2290 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/__init__.py
+-rw-r--r--   0 jagga      (501) staff       (20)     9305 2024-04-17 10:17:07.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/api_client.py
+-rw-r--r--   0 jagga      (501) staff       (20)     2794 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/apitoken.py
+-rw-r--r--   0 jagga      (501) staff       (20)     9405 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/client.py
+-rw-r--r--   0 jagga      (501) staff       (20)     7401 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/constants.py
+-rw-r--r--   0 jagga      (501) staff       (20)     5788 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/datasets.py
+-rw-r--r--   0 jagga      (501) staff       (20)    13823 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/endpoints.py
+-rw-r--r--   0 jagga      (501) staff       (20)     2619 2024-04-17 10:17:07.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/helpers.py
+-rw-r--r--   0 jagga      (501) staff       (20)     1368 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/images.py
+-rw-r--r--   0 jagga      (501) staff       (20)     2105 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/minio_service.py
+-rw-r--r--   0 jagga      (501) staff       (20)     6455 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/models.py
+-rw-r--r--   0 jagga      (501) staff       (20)     6022 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/notebook.py
+-rw-r--r--   0 jagga      (501) staff       (20)     9999 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/pipelines.py
+-rw-r--r--   0 jagga      (501) staff       (20)     2849 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/projects.py
+-rw-r--r--   0 jagga      (501) staff       (20)     4268 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/skus.py
+-rw-r--r--   0 jagga      (501) staff       (20)     2391 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/teams.py
+-rw-r--r--   0 jagga      (501) staff       (20)     1159 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/utils.py
+-rw-r--r--   0 jagga      (501) staff       (20)       23 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/cloud/tir/version.py
+-rw-r--r--   0 jagga      (501) staff       (20)     1517 2024-04-15 09:47:56.000000 e2enetworks-1.2.2/e2enetworks/constants.py
+drwxr-xr-x   0 jagga      (501) staff       (20)        0 2024-04-17 10:20:46.289195 e2enetworks-1.2.2/e2enetworks.egg-info/
+-rw-r--r--   0 jagga      (501) staff       (20)     1418 2024-04-17 10:20:46.000000 e2enetworks-1.2.2/e2enetworks.egg-info/PKG-INFO
+-rw-r--r--   0 jagga      (501) staff       (20)      914 2024-04-17 10:20:46.000000 e2enetworks-1.2.2/e2enetworks.egg-info/SOURCES.txt
+-rw-r--r--   0 jagga      (501) staff       (20)        1 2024-04-17 10:20:46.000000 e2enetworks-1.2.2/e2enetworks.egg-info/dependency_links.txt
+-rw-r--r--   0 jagga      (501) staff       (20)      138 2024-04-17 10:20:46.000000 e2enetworks-1.2.2/e2enetworks.egg-info/requires.txt
+-rw-r--r--   0 jagga      (501) staff       (20)       12 2024-04-17 10:20:46.000000 e2enetworks-1.2.2/e2enetworks.egg-info/top_level.txt
+-rw-r--r--   0 jagga      (501) staff       (20)       38 2024-04-17 10:20:46.289710 e2enetworks-1.2.2/setup.cfg
+-rw-r--r--   0 jagga      (501) staff       (20)     1829 2024-04-17 10:17:07.000000 e2enetworks-1.2.2/setup.py
```

### Comparing `e2enetworks-1.2.1/LICENSE.txt` & `e2enetworks-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.1/e2enetworks/cloud/tir/__init__.py` & `e2enetworks-1.2.2/e2enetworks/cloud/tir/__init__.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.1/e2enetworks/cloud/tir/api_client.py` & `e2enetworks-1.2.2/e2enetworks/cloud/tir/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,22 +36,22 @@
             return self.__whisper_infer(data)
         
         namespace = "p-" + str(client.Default.project())
         try:
             url_status, url = get_model_url(model_name, namespace)
             if not url_status:
                 raise Exception(f"Invalid input Error {url} model not present")
-            data_status, data = get_formated_data_for_model(model_name, data)
+            data_status, payload = get_formated_data_for_model(model_name, data)
             if not data_status:
-                raise Exception(f"Invalid data key Error {str(data)}")
+                raise Exception(f"Invalid data key Error {str(payload)}")
 
         except Exception as e:
             raise Exception(f"Input Error {e}")
         headers["Authorization"] = f"Bearer {client.Default.access_token()}"
-        response = requests.post(url=url, headers=headers, data=json.dumps(data))
+        response = requests.post(url=url, headers=headers, data=json.dumps(payload))
         response = prepare_object(response)
         return response
     
     def __whisper_infer(self, data : dict):
         namespace = "p-" + str(client.Default.project())
         try:
             is_valid_input, error = self.__validate_whisper_data(data)
```

### Comparing `e2enetworks-1.2.1/e2enetworks/cloud/tir/apitoken.py` & `e2enetworks-1.2.2/e2enetworks/cloud/tir/apitoken.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.1/e2enetworks/cloud/tir/client.py` & `e2enetworks-1.2.2/e2enetworks/cloud/tir/client.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.1/e2enetworks/cloud/tir/constants.py` & `e2enetworks-1.2.2/e2enetworks/cloud/tir/constants.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.1/e2enetworks/cloud/tir/datasets.py` & `e2enetworks-1.2.2/e2enetworks/cloud/tir/datasets.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.1/e2enetworks/cloud/tir/endpoints.py` & `e2enetworks-1.2.2/e2enetworks/cloud/tir/endpoints.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.1/e2enetworks/cloud/tir/helpers.py` & `e2enetworks-1.2.2/e2enetworks/cloud/tir/helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from copy import deepcopy
 import string
 import random
 from e2enetworks.constants import BASE_URL_MODEL_API_CLIENT
 from e2enetworks.cloud.tir.constants import MODEL_NAME_TO_URL_PATH_MAPPING, MODEL_API_DEFAULT_DATA, MODELS_API_DATA_FORMATS
 
 
 def get_random_string(N):
@@ -49,16 +50,16 @@
     if model_name not in MODEL_NAME_TO_URL_PATH_MAPPING:
         return False, model_name
     url = BASE_URL_MODEL_API_CLIENT + MODEL_NAME_TO_URL_PATH_MAPPING[model_name].format(namespace=namespace)
     return True, url
 
 def get_formated_data_for_model(model_name, parameters):
     extra_keys = []
-    fromatted_data = MODEL_API_DEFAULT_DATA
-    model_formatted_data = MODELS_API_DATA_FORMATS.get(model_name)
+    fromatted_data = deepcopy(MODEL_API_DEFAULT_DATA)
+    model_formatted_data = deepcopy(MODELS_API_DATA_FORMATS).get(model_name)
     for input_key in parameters:
         if input_key in model_formatted_data:
             key_data = model_formatted_data.get(input_key)
             key_data["data"].append(parameters.get(input_key))
             fromatted_data["inputs"].append(key_data)
         else:
             extra_keys.append(input_key)
```

### Comparing `e2enetworks-1.2.1/e2enetworks/cloud/tir/images.py` & `e2enetworks-1.2.2/e2enetworks/cloud/tir/images.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.1/e2enetworks/cloud/tir/minio_service.py` & `e2enetworks-1.2.2/e2enetworks/cloud/tir/minio_service.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.1/e2enetworks/cloud/tir/models.py` & `e2enetworks-1.2.2/e2enetworks/cloud/tir/models.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.1/e2enetworks/cloud/tir/notebook.py` & `e2enetworks-1.2.2/e2enetworks/cloud/tir/notebook.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.1/e2enetworks/cloud/tir/pipelines.py` & `e2enetworks-1.2.2/e2enetworks/cloud/tir/pipelines.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.1/e2enetworks/cloud/tir/projects.py` & `e2enetworks-1.2.2/e2enetworks/cloud/tir/projects.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.1/e2enetworks/cloud/tir/skus.py` & `e2enetworks-1.2.2/e2enetworks/cloud/tir/skus.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.1/e2enetworks/cloud/tir/teams.py` & `e2enetworks-1.2.2/e2enetworks/cloud/tir/teams.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.1/e2enetworks/cloud/tir/utils.py` & `e2enetworks-1.2.2/e2enetworks/cloud/tir/utils.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.1/e2enetworks/constants.py` & `e2enetworks-1.2.2/e2enetworks/constants.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.1/e2enetworks.egg-info/SOURCES.txt` & `e2enetworks-1.2.2/e2enetworks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `e2enetworks-1.2.1/setup.py` & `e2enetworks-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 from setuptools import find_packages
 from os import path
 
-version = "1.2.1"
+version = "1.2.2"
 install_requires = [
     "requests~=2.30.0",
     "urllib3==1.26.6",
     "kfp==1.8.22",
     "kfp-pipeline-spec==0.1.16",
     "kfp-server-api==1.8.5",
     "minio==7.1.3",
```

