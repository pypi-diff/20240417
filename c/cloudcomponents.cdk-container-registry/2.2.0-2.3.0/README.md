# Comparing `tmp/cloudcomponents.cdk-container-registry-2.2.0.tar.gz` & `tmp/cloudcomponents.cdk-container-registry-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudcomponents.cdk-container-registry-2.2.0.tar", last modified: Mon Mar 25 18:25:38 2024, max compression
+gzip compressed data, was "cloudcomponents.cdk-container-registry-2.3.0.tar", last modified: Wed Apr 17 18:35:56 2024, max compression
```

## Comparing `cloudcomponents.cdk-container-registry-2.2.0.tar` & `cloudcomponents.cdk-container-registry-2.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:38.068248 cloudcomponents.cdk-container-registry-2.2.0/
--rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-03-25 18:25:35.000000 cloudcomponents.cdk-container-registry-2.2.0/LICENSE
--rw-r--r--   0 hupe       (501) staff       (20)       23 2024-03-25 18:25:35.000000 cloudcomponents.cdk-container-registry-2.2.0/MANIFEST.in
--rw-r--r--   0 hupe       (501) staff       (20)     3059 2024-03-25 18:25:38.068064 cloudcomponents.cdk-container-registry-2.2.0/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)     2226 2024-03-25 18:25:35.000000 cloudcomponents.cdk-container-registry-2.2.0/README.md
--rw-r--r--   0 hupe       (501) staff       (20)      234 2024-03-25 18:25:35.000000 cloudcomponents.cdk-container-registry-2.2.0/pyproject.toml
--rw-r--r--   0 hupe       (501) staff       (20)       38 2024-03-25 18:25:38.068284 cloudcomponents.cdk-container-registry-2.2.0/setup.cfg
--rw-r--r--   0 hupe       (501) staff       (20)     1783 2024-03-25 18:25:35.000000 cloudcomponents.cdk-container-registry-2.2.0/setup.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:38.065828 cloudcomponents.cdk-container-registry-2.2.0/src/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:38.065885 cloudcomponents.cdk-container-registry-2.2.0/src/cloudcomponents/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:38.067541 cloudcomponents.cdk-container-registry-2.2.0/src/cloudcomponents/cdk_container_registry/
--rw-r--r--   0 hupe       (501) staff       (20)    26928 2024-03-25 18:25:35.000000 cloudcomponents.cdk-container-registry-2.2.0/src/cloudcomponents/cdk_container_registry/__init__.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:38.067805 cloudcomponents.cdk-container-registry-2.2.0/src/cloudcomponents/cdk_container_registry/_jsii/
--rw-r--r--   0 hupe       (501) staff       (20)      441 2024-03-25 18:25:35.000000 cloudcomponents.cdk-container-registry-2.2.0/src/cloudcomponents/cdk_container_registry/_jsii/__init__.py
--rw-r--r--   0 hupe       (501) staff       (20)   128198 2024-03-25 18:25:35.000000 cloudcomponents.cdk-container-registry-2.2.0/src/cloudcomponents/cdk_container_registry/_jsii/cdk-container-registry@2.2.0.jsii.tgz
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-03-25 18:25:35.000000 cloudcomponents.cdk-container-registry-2.2.0/src/cloudcomponents/cdk_container_registry/py.typed
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:38.067270 cloudcomponents.cdk-container-registry-2.2.0/src/cloudcomponents.cdk_container_registry.egg-info/
--rw-r--r--   0 hupe       (501) staff       (20)     3059 2024-03-25 18:25:38.000000 cloudcomponents.cdk-container-registry-2.2.0/src/cloudcomponents.cdk_container_registry.egg-info/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)      637 2024-03-25 18:25:38.000000 cloudcomponents.cdk-container-registry-2.2.0/src/cloudcomponents.cdk_container_registry.egg-info/SOURCES.txt
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-03-25 18:25:38.000000 cloudcomponents.cdk-container-registry-2.2.0/src/cloudcomponents.cdk_container_registry.egg-info/dependency_links.txt
--rw-r--r--   0 hupe       (501) staff       (20)      112 2024-03-25 18:25:38.000000 cloudcomponents.cdk-container-registry-2.2.0/src/cloudcomponents.cdk_container_registry.egg-info/requires.txt
--rw-r--r--   0 hupe       (501) staff       (20)       16 2024-03-25 18:25:38.000000 cloudcomponents.cdk-container-registry-2.2.0/src/cloudcomponents.cdk_container_registry.egg-info/top_level.txt
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:56.094441 cloudcomponents.cdk-container-registry-2.3.0/
+-rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-04-17 18:35:52.000000 cloudcomponents.cdk-container-registry-2.3.0/LICENSE
+-rw-r--r--   0 hupe       (501) staff       (20)       23 2024-04-17 18:35:52.000000 cloudcomponents.cdk-container-registry-2.3.0/MANIFEST.in
+-rw-r--r--   0 hupe       (501) staff       (20)     3059 2024-04-17 18:35:56.094222 cloudcomponents.cdk-container-registry-2.3.0/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)     2226 2024-04-17 18:35:52.000000 cloudcomponents.cdk-container-registry-2.3.0/README.md
+-rw-r--r--   0 hupe       (501) staff       (20)      234 2024-04-17 18:35:52.000000 cloudcomponents.cdk-container-registry-2.3.0/pyproject.toml
+-rw-r--r--   0 hupe       (501) staff       (20)       38 2024-04-17 18:35:56.094481 cloudcomponents.cdk-container-registry-2.3.0/setup.cfg
+-rw-r--r--   0 hupe       (501) staff       (20)     1783 2024-04-17 18:35:52.000000 cloudcomponents.cdk-container-registry-2.3.0/setup.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:56.091061 cloudcomponents.cdk-container-registry-2.3.0/src/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:56.091121 cloudcomponents.cdk-container-registry-2.3.0/src/cloudcomponents/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:56.092882 cloudcomponents.cdk-container-registry-2.3.0/src/cloudcomponents/cdk_container_registry/
+-rw-r--r--   0 hupe       (501) staff       (20)    26928 2024-04-17 18:35:52.000000 cloudcomponents.cdk-container-registry-2.3.0/src/cloudcomponents/cdk_container_registry/__init__.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:56.093194 cloudcomponents.cdk-container-registry-2.3.0/src/cloudcomponents/cdk_container_registry/_jsii/
+-rw-r--r--   0 hupe       (501) staff       (20)      441 2024-04-17 18:35:52.000000 cloudcomponents.cdk-container-registry-2.3.0/src/cloudcomponents/cdk_container_registry/_jsii/__init__.py
+-rw-r--r--   0 hupe       (501) staff       (20)  1330183 2024-04-17 18:35:52.000000 cloudcomponents.cdk-container-registry-2.3.0/src/cloudcomponents/cdk_container_registry/_jsii/cdk-container-registry@2.3.0.jsii.tgz
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:35:52.000000 cloudcomponents.cdk-container-registry-2.3.0/src/cloudcomponents/cdk_container_registry/py.typed
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:56.092577 cloudcomponents.cdk-container-registry-2.3.0/src/cloudcomponents.cdk_container_registry.egg-info/
+-rw-r--r--   0 hupe       (501) staff       (20)     3059 2024-04-17 18:35:56.000000 cloudcomponents.cdk-container-registry-2.3.0/src/cloudcomponents.cdk_container_registry.egg-info/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)      637 2024-04-17 18:35:56.000000 cloudcomponents.cdk-container-registry-2.3.0/src/cloudcomponents.cdk_container_registry.egg-info/SOURCES.txt
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:35:56.000000 cloudcomponents.cdk-container-registry-2.3.0/src/cloudcomponents.cdk_container_registry.egg-info/dependency_links.txt
+-rw-r--r--   0 hupe       (501) staff       (20)      112 2024-04-17 18:35:56.000000 cloudcomponents.cdk-container-registry-2.3.0/src/cloudcomponents.cdk_container_registry.egg-info/requires.txt
+-rw-r--r--   0 hupe       (501) staff       (20)       16 2024-04-17 18:35:56.000000 cloudcomponents.cdk-container-registry-2.3.0/src/cloudcomponents.cdk_container_registry.egg-info/top_level.txt
```

### Comparing `cloudcomponents.cdk-container-registry-2.2.0/LICENSE` & `cloudcomponents.cdk-container-registry-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-container-registry-2.2.0/PKG-INFO` & `cloudcomponents.cdk-container-registry-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-container-registry
-Version: 2.2.0
+Version: 2.3.0
 Summary: Registry for container images
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-container-registry-2.2.0/README.md` & `cloudcomponents.cdk-container-registry-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-container-registry-2.2.0/setup.py` & `cloudcomponents.cdk-container-registry-2.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudcomponents.cdk-container-registry",
-    "version": "2.2.0",
+    "version": "2.3.0",
     "description": "Registry for container images",
     "license": "MIT",
     "url": "https://github.com/cloudcomponents/cdk-constructs",
     "long_description_content_type": "text/markdown",
     "author": "hupe1980",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cloudcomponents.cdk_container_registry",
         "cloudcomponents.cdk_container_registry._jsii"
     ],
     "package_data": {
         "cloudcomponents.cdk_container_registry._jsii": [
-            "cdk-container-registry@2.2.0.jsii.tgz"
+            "cdk-container-registry@2.3.0.jsii.tgz"
         ],
         "cloudcomponents.cdk_container_registry": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cloudcomponents.cdk-container-registry-2.2.0/src/cloudcomponents/cdk_container_registry/__init__.py` & `cloudcomponents.cdk-container-registry-2.3.0/src/cloudcomponents/cdk_container_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-container-registry-2.2.0/src/cloudcomponents.cdk_container_registry.egg-info/PKG-INFO` & `cloudcomponents.cdk-container-registry-2.3.0/src/cloudcomponents.cdk_container_registry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-container-registry
-Version: 2.2.0
+Version: 2.3.0
 Summary: Registry for container images
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-container-registry-2.2.0/src/cloudcomponents.cdk_container_registry.egg-info/SOURCES.txt` & `cloudcomponents.cdk-container-registry-2.3.0/src/cloudcomponents.cdk_container_registry.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cloudcomponents.cdk_container_registry.egg-info/SOURCES.txt
 src/cloudcomponents.cdk_container_registry.egg-info/dependency_links.txt
 src/cloudcomponents.cdk_container_registry.egg-info/requires.txt
 src/cloudcomponents.cdk_container_registry.egg-info/top_level.txt
 src/cloudcomponents/cdk_container_registry/__init__.py
 src/cloudcomponents/cdk_container_registry/py.typed
 src/cloudcomponents/cdk_container_registry/_jsii/__init__.py
-src/cloudcomponents/cdk_container_registry/_jsii/cdk-container-registry@2.2.0.jsii.tgz
+src/cloudcomponents/cdk_container_registry/_jsii/cdk-container-registry@2.3.0.jsii.tgz
```

