# Comparing `tmp/cloudcomponents.cdk-blue-green-container-deployment-2.2.0.tar.gz` & `tmp/cloudcomponents.cdk-blue-green-container-deployment-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudcomponents.cdk-blue-green-container-deployment-2.2.0.tar", last modified: Mon Mar 25 18:23:32 2024, max compression
+gzip compressed data, was "cloudcomponents.cdk-blue-green-container-deployment-2.3.0.tar", last modified: Wed Apr 17 18:35:46 2024, max compression
```

## Comparing `cloudcomponents.cdk-blue-green-container-deployment-2.2.0.tar` & `cloudcomponents.cdk-blue-green-container-deployment-2.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:23:32.265227 cloudcomponents.cdk-blue-green-container-deployment-2.2.0/
--rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-03-25 18:23:29.000000 cloudcomponents.cdk-blue-green-container-deployment-2.2.0/LICENSE
--rw-r--r--   0 hupe       (501) staff       (20)       23 2024-03-25 18:23:29.000000 cloudcomponents.cdk-blue-green-container-deployment-2.2.0/MANIFEST.in
--rw-r--r--   0 hupe       (501) staff       (20)     7023 2024-03-25 18:23:32.265041 cloudcomponents.cdk-blue-green-container-deployment-2.2.0/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)     6159 2024-03-25 18:23:29.000000 cloudcomponents.cdk-blue-green-container-deployment-2.2.0/README.md
--rw-r--r--   0 hupe       (501) staff       (20)      234 2024-03-25 18:23:29.000000 cloudcomponents.cdk-blue-green-container-deployment-2.2.0/pyproject.toml
--rw-r--r--   0 hupe       (501) staff       (20)       38 2024-03-25 18:23:32.265261 cloudcomponents.cdk-blue-green-container-deployment-2.2.0/setup.cfg
--rw-r--r--   0 hupe       (501) staff       (20)     1879 2024-03-25 18:23:29.000000 cloudcomponents.cdk-blue-green-container-deployment-2.2.0/setup.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:23:32.262600 cloudcomponents.cdk-blue-green-container-deployment-2.2.0/src/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:23:32.262653 cloudcomponents.cdk-blue-green-container-deployment-2.2.0/src/cloudcomponents/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:23:32.264231 cloudcomponents.cdk-blue-green-container-deployment-2.2.0/src/cloudcomponents/cdk_blue_green_container_deployment/
--rw-r--r--   0 hupe       (501) staff       (20)    80643 2024-03-25 18:23:29.000000 cloudcomponents.cdk-blue-green-container-deployment-2.2.0/src/cloudcomponents/cdk_blue_green_container_deployment/__init__.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:23:32.264489 cloudcomponents.cdk-blue-green-container-deployment-2.2.0/src/cloudcomponents/cdk_blue_green_container_deployment/_jsii/
--rw-r--r--   0 hupe       (501) staff       (20)      467 2024-03-25 18:23:29.000000 cloudcomponents.cdk-blue-green-container-deployment-2.2.0/src/cloudcomponents/cdk_blue_green_container_deployment/_jsii/__init__.py
--rw-r--r--   0 hupe       (501) staff       (20)   775898 2024-03-25 18:23:29.000000 cloudcomponents.cdk-blue-green-container-deployment-2.2.0/src/cloudcomponents/cdk_blue_green_container_deployment/_jsii/cdk-blue-green-container-deployment@2.2.0.jsii.tgz
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-03-25 18:23:29.000000 cloudcomponents.cdk-blue-green-container-deployment-2.2.0/src/cloudcomponents/cdk_blue_green_container_deployment/py.typed
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:23:32.263937 cloudcomponents.cdk-blue-green-container-deployment-2.2.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/
--rw-r--r--   0 hupe       (501) staff       (20)     7023 2024-03-25 18:23:32.000000 cloudcomponents.cdk-blue-green-container-deployment-2.2.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)      767 2024-03-25 18:23:32.000000 cloudcomponents.cdk-blue-green-container-deployment-2.2.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/SOURCES.txt
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-03-25 18:23:32.000000 cloudcomponents.cdk-blue-green-container-deployment-2.2.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/dependency_links.txt
--rw-r--r--   0 hupe       (501) staff       (20)      112 2024-03-25 18:23:32.000000 cloudcomponents.cdk-blue-green-container-deployment-2.2.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/requires.txt
--rw-r--r--   0 hupe       (501) staff       (20)       16 2024-03-25 18:23:32.000000 cloudcomponents.cdk-blue-green-container-deployment-2.2.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/top_level.txt
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.573362 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/
+-rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-04-17 18:35:42.000000 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/LICENSE
+-rw-r--r--   0 hupe       (501) staff       (20)       23 2024-04-17 18:35:42.000000 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/MANIFEST.in
+-rw-r--r--   0 hupe       (501) staff       (20)     7023 2024-04-17 18:35:46.573039 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)     6159 2024-04-17 18:35:42.000000 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/README.md
+-rw-r--r--   0 hupe       (501) staff       (20)      234 2024-04-17 18:35:42.000000 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/pyproject.toml
+-rw-r--r--   0 hupe       (501) staff       (20)       38 2024-04-17 18:35:46.573407 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/setup.cfg
+-rw-r--r--   0 hupe       (501) staff       (20)     1879 2024-04-17 18:35:42.000000 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/setup.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.567765 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.567833 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.570717 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents/cdk_blue_green_container_deployment/
+-rw-r--r--   0 hupe       (501) staff       (20)    80643 2024-04-17 18:35:42.000000 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents/cdk_blue_green_container_deployment/__init__.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.571021 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents/cdk_blue_green_container_deployment/_jsii/
+-rw-r--r--   0 hupe       (501) staff       (20)      467 2024-04-17 18:35:42.000000 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents/cdk_blue_green_container_deployment/_jsii/__init__.py
+-rw-r--r--   0 hupe       (501) staff       (20)  3178833 2024-04-17 18:35:42.000000 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents/cdk_blue_green_container_deployment/_jsii/cdk-blue-green-container-deployment@2.3.0.jsii.tgz
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:35:42.000000 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents/cdk_blue_green_container_deployment/py.typed
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.570354 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/
+-rw-r--r--   0 hupe       (501) staff       (20)     7023 2024-04-17 18:35:46.000000 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)      767 2024-04-17 18:35:46.000000 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/SOURCES.txt
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:35:46.000000 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/dependency_links.txt
+-rw-r--r--   0 hupe       (501) staff       (20)      112 2024-04-17 18:35:46.000000 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/requires.txt
+-rw-r--r--   0 hupe       (501) staff       (20)       16 2024-04-17 18:35:46.000000 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/top_level.txt
```

### Comparing `cloudcomponents.cdk-blue-green-container-deployment-2.2.0/LICENSE` & `cloudcomponents.cdk-blue-green-container-deployment-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-blue-green-container-deployment-2.2.0/PKG-INFO` & `cloudcomponents.cdk-blue-green-container-deployment-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-blue-green-container-deployment
-Version: 2.2.0
+Version: 2.3.0
 Summary: Blue green container deployment with CodeDeploy
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-blue-green-container-deployment-2.2.0/README.md` & `cloudcomponents.cdk-blue-green-container-deployment-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-blue-green-container-deployment-2.2.0/setup.py` & `cloudcomponents.cdk-blue-green-container-deployment-2.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudcomponents.cdk-blue-green-container-deployment",
-    "version": "2.2.0",
+    "version": "2.3.0",
     "description": "Blue green container deployment with CodeDeploy",
     "license": "MIT",
     "url": "https://github.com/cloudcomponents/cdk-constructs",
     "long_description_content_type": "text/markdown",
     "author": "hupe1980",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cloudcomponents.cdk_blue_green_container_deployment",
         "cloudcomponents.cdk_blue_green_container_deployment._jsii"
     ],
     "package_data": {
         "cloudcomponents.cdk_blue_green_container_deployment._jsii": [
-            "cdk-blue-green-container-deployment@2.2.0.jsii.tgz"
+            "cdk-blue-green-container-deployment@2.3.0.jsii.tgz"
         ],
         "cloudcomponents.cdk_blue_green_container_deployment": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cloudcomponents.cdk-blue-green-container-deployment-2.2.0/src/cloudcomponents/cdk_blue_green_container_deployment/__init__.py` & `cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents/cdk_blue_green_container_deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-blue-green-container-deployment-2.2.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/PKG-INFO` & `cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-blue-green-container-deployment
-Version: 2.2.0
+Version: 2.3.0
 Summary: Blue green container deployment with CodeDeploy
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-blue-green-container-deployment-2.2.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/SOURCES.txt` & `cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/SOURCES.txt
 src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/dependency_links.txt
 src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/requires.txt
 src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/top_level.txt
 src/cloudcomponents/cdk_blue_green_container_deployment/__init__.py
 src/cloudcomponents/cdk_blue_green_container_deployment/py.typed
 src/cloudcomponents/cdk_blue_green_container_deployment/_jsii/__init__.py
-src/cloudcomponents/cdk_blue_green_container_deployment/_jsii/cdk-blue-green-container-deployment@2.2.0.jsii.tgz
+src/cloudcomponents/cdk_blue_green_container_deployment/_jsii/cdk-blue-green-container-deployment@2.3.0.jsii.tgz
```

