# Comparing `tmp/asksageclient-1.2.0.tar.gz` & `tmp/asksageclient-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asksageclient-1.2.0.tar", last modified: Sun Jan 21 21:44:13 2024, max compression
+gzip compressed data, was "asksageclient-1.2.1.tar", last modified: Wed Apr 17 20:23:55 2024, max compression
```

## Comparing `asksageclient-1.2.0.tar` & `asksageclient-1.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-01-21 21:44:13.611130 asksageclient-1.2.0/
--rw-rw-rw-   0        0        0     1128 2023-09-28 23:51:19.000000 asksageclient-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     2451 2024-01-21 21:44:13.611130 asksageclient-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1920 2024-01-21 21:42:41.000000 asksageclient-1.2.0/README.md
--rw-rw-rw-   0        0        0      609 2024-01-21 21:25:38.000000 asksageclient-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-21 21:44:13.611130 asksageclient-1.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-01-21 21:44:13.598296 asksageclient-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-01-21 21:44:13.605119 asksageclient-1.2.0/src/asksageclient/
--rw-rw-rw-   0        0        0       33 2023-09-28 23:47:35.000000 asksageclient-1.2.0/src/asksageclient/__init__.py
--rw-rw-rw-   0        0        0    16154 2024-01-21 21:41:55.000000 asksageclient-1.2.0/src/asksageclient/client.py
-drwxrwxrwx   0        0        0        0 2024-01-21 21:44:13.610128 asksageclient-1.2.0/src/asksageclient.egg-info/
--rw-rw-rw-   0        0        0     2451 2024-01-21 21:44:13.000000 asksageclient-1.2.0/src/asksageclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-01-21 21:44:13.000000 asksageclient-1.2.0/src/asksageclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-21 21:44:13.000000 asksageclient-1.2.0/src/asksageclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-01-21 21:44:13.000000 asksageclient-1.2.0/src/asksageclient.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 20:23:55.206426 asksageclient-1.2.1/
+-rw-rw-rw-   0        0        0     1128 2023-09-28 23:51:19.000000 asksageclient-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     2451 2024-04-17 20:23:55.199658 asksageclient-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1920 2024-01-21 21:42:41.000000 asksageclient-1.2.1/README.md
+-rw-rw-rw-   0        0        0      609 2024-04-17 20:19:34.000000 asksageclient-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-17 20:23:55.206426 asksageclient-1.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 20:23:55.179496 asksageclient-1.2.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-17 20:23:55.187643 asksageclient-1.2.1/src/asksageclient/
+-rw-rw-rw-   0        0        0       33 2023-09-28 23:47:35.000000 asksageclient-1.2.1/src/asksageclient/__init__.py
+-rw-rw-rw-   0        0        0    16304 2024-04-17 19:16:37.000000 asksageclient-1.2.1/src/asksageclient/client.py
+drwxrwxrwx   0        0        0        0 2024-04-17 20:23:55.199658 asksageclient-1.2.1/src/asksageclient.egg-info/
+-rw-rw-rw-   0        0        0     2451 2024-04-17 20:23:55.000000 asksageclient-1.2.1/src/asksageclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-04-17 20:23:55.000000 asksageclient-1.2.1/src/asksageclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 20:23:55.000000 asksageclient-1.2.1/src/asksageclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-17 20:23:55.000000 asksageclient-1.2.1/src/asksageclient.egg-info/top_level.txt
```

### Comparing `asksageclient-1.2.0/LICENSE` & `asksageclient-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asksageclient-1.2.0/PKG-INFO` & `asksageclient-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asksageclient
-Version: 1.2.0
+Version: 1.2.1
 Summary: Ask Sage Python Client API
 Author-email: "Ask Sage, Inc." <support@asksage.ai>
 Project-URL: Homepage, https://github.com/Ask-Sage/asksage-client
 Project-URL: Bug Tracker, https://github.com/Ask-Sage/asksage-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `asksageclient-1.2.0/README.md` & `asksageclient-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `asksageclient-1.2.0/pyproject.toml` & `asksageclient-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "asksageclient"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="Ask Sage, Inc.", email="support@asksage.ai" },
 ]
 description = "Ask Sage Python Client API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `asksageclient-1.2.0/src/asksageclient/client.py` & `asksageclient-1.2.1/src/asksageclient/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -313,30 +313,32 @@
     Get the count of monthly training tokens spent for this user from the Ask Sage service.
 
     Returns:
     dict: The response from the service with the count.
         """
         return self._request('POST', 'count-monthly-teach-tokens')
 
-    def train(self, content, force_dataset=None, context=''):
+    def train(self, content, force_dataset=None, context='', skip_vectordb=False):
         """
     Train the model based on the provided content.
 
     Parameters:
     content (str): The message to be processed by the service. Ensure it is under 500 tokens.
     force_dataset (str, optional): The dataset to be used. Enter your custom dataset, must follow the following format: user_content_USERID_DATASET-NAME_content. Replace USERID by user ID and DATASET-NAME by the name of your dataset.
     context (str): Short context about the content (metadata). Under 20 tokens.
+    skip_vectordb (bool): Whether to skip the VectorDB training. Default is False.
     
     Returns:
     dict: The response from the service.
         """
         return self._request('POST', 'train', json= {
             'content': content,
             'force_dataset': force_dataset,
-            'context': context
+            'context': context,
+            'skip_vectordb': skip_vectordb
         })
 
     def train_with_file(self, file_path, dataset):
         """
     Train the dataset based on the provided file.
 
     Parameters:
```

### Comparing `asksageclient-1.2.0/src/asksageclient.egg-info/PKG-INFO` & `asksageclient-1.2.1/src/asksageclient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asksageclient
-Version: 1.2.0
+Version: 1.2.1
 Summary: Ask Sage Python Client API
 Author-email: "Ask Sage, Inc." <support@asksage.ai>
 Project-URL: Homepage, https://github.com/Ask-Sage/asksage-client
 Project-URL: Bug Tracker, https://github.com/Ask-Sage/asksage-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

