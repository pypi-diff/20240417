# Comparing `tmp/cloudcomponents.cdk-codepipeline-merge-action-2.2.0.tar.gz` & `tmp/cloudcomponents.cdk-codepipeline-merge-action-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudcomponents.cdk-codepipeline-merge-action-2.2.0.tar", last modified: Mon Mar 25 18:25:28 2024, max compression
+gzip compressed data, was "cloudcomponents.cdk-codepipeline-merge-action-2.3.0.tar", last modified: Wed Apr 17 18:35:46 2024, max compression
```

## Comparing `cloudcomponents.cdk-codepipeline-merge-action-2.2.0.tar` & `cloudcomponents.cdk-codepipeline-merge-action-2.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.267467 cloudcomponents.cdk-codepipeline-merge-action-2.2.0/
--rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-merge-action-2.2.0/LICENSE
--rw-r--r--   0 hupe       (501) staff       (20)       23 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-merge-action-2.2.0/MANIFEST.in
--rw-r--r--   0 hupe       (501) staff       (20)     3670 2024-03-25 18:25:28.267159 cloudcomponents.cdk-codepipeline-merge-action-2.2.0/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)     2795 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-merge-action-2.2.0/README.md
--rw-r--r--   0 hupe       (501) staff       (20)      234 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-merge-action-2.2.0/pyproject.toml
--rw-r--r--   0 hupe       (501) staff       (20)       38 2024-03-25 18:25:28.267525 cloudcomponents.cdk-codepipeline-merge-action-2.2.0/setup.cfg
--rw-r--r--   0 hupe       (501) staff       (20)     1860 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-merge-action-2.2.0/setup.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.263345 cloudcomponents.cdk-codepipeline-merge-action-2.2.0/src/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.263423 cloudcomponents.cdk-codepipeline-merge-action-2.2.0/src/cloudcomponents/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.265698 cloudcomponents.cdk-codepipeline-merge-action-2.2.0/src/cloudcomponents/cdk_codepipeline_merge_action/
--rw-r--r--   0 hupe       (501) staff       (20)    20936 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-merge-action-2.2.0/src/cloudcomponents/cdk_codepipeline_merge_action/__init__.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.266737 cloudcomponents.cdk-codepipeline-merge-action-2.2.0/src/cloudcomponents/cdk_codepipeline_merge_action/_jsii/
--rw-r--r--   0 hupe       (501) staff       (20)      455 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-merge-action-2.2.0/src/cloudcomponents/cdk_codepipeline_merge_action/_jsii/__init__.py
--rw-r--r--   0 hupe       (501) staff       (20)   133738 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-merge-action-2.2.0/src/cloudcomponents/cdk_codepipeline_merge_action/_jsii/cdk-codepipeline-merge-action@2.2.0.jsii.tgz
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-merge-action-2.2.0/src/cloudcomponents/cdk_codepipeline_merge_action/py.typed
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.265134 cloudcomponents.cdk-codepipeline-merge-action-2.2.0/src/cloudcomponents.cdk_codepipeline_merge_action.egg-info/
--rw-r--r--   0 hupe       (501) staff       (20)     3670 2024-03-25 18:25:28.000000 cloudcomponents.cdk-codepipeline-merge-action-2.2.0/src/cloudcomponents.cdk_codepipeline_merge_action.egg-info/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)      707 2024-03-25 18:25:28.000000 cloudcomponents.cdk-codepipeline-merge-action-2.2.0/src/cloudcomponents.cdk_codepipeline_merge_action.egg-info/SOURCES.txt
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-03-25 18:25:28.000000 cloudcomponents.cdk-codepipeline-merge-action-2.2.0/src/cloudcomponents.cdk_codepipeline_merge_action.egg-info/dependency_links.txt
--rw-r--r--   0 hupe       (501) staff       (20)      112 2024-03-25 18:25:28.000000 cloudcomponents.cdk-codepipeline-merge-action-2.2.0/src/cloudcomponents.cdk_codepipeline_merge_action.egg-info/requires.txt
--rw-r--r--   0 hupe       (501) staff       (20)       16 2024-03-25 18:25:28.000000 cloudcomponents.cdk-codepipeline-merge-action-2.2.0/src/cloudcomponents.cdk_codepipeline_merge_action.egg-info/top_level.txt
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.190838 cloudcomponents.cdk-codepipeline-merge-action-2.3.0/
+-rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-04-17 18:35:41.000000 cloudcomponents.cdk-codepipeline-merge-action-2.3.0/LICENSE
+-rw-r--r--   0 hupe       (501) staff       (20)       23 2024-04-17 18:35:41.000000 cloudcomponents.cdk-codepipeline-merge-action-2.3.0/MANIFEST.in
+-rw-r--r--   0 hupe       (501) staff       (20)     3670 2024-04-17 18:35:46.190462 cloudcomponents.cdk-codepipeline-merge-action-2.3.0/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)     2795 2024-04-17 18:35:41.000000 cloudcomponents.cdk-codepipeline-merge-action-2.3.0/README.md
+-rw-r--r--   0 hupe       (501) staff       (20)      234 2024-04-17 18:35:41.000000 cloudcomponents.cdk-codepipeline-merge-action-2.3.0/pyproject.toml
+-rw-r--r--   0 hupe       (501) staff       (20)       38 2024-04-17 18:35:46.192494 cloudcomponents.cdk-codepipeline-merge-action-2.3.0/setup.cfg
+-rw-r--r--   0 hupe       (501) staff       (20)     1860 2024-04-17 18:35:41.000000 cloudcomponents.cdk-codepipeline-merge-action-2.3.0/setup.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.186281 cloudcomponents.cdk-codepipeline-merge-action-2.3.0/src/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.186447 cloudcomponents.cdk-codepipeline-merge-action-2.3.0/src/cloudcomponents/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.188785 cloudcomponents.cdk-codepipeline-merge-action-2.3.0/src/cloudcomponents/cdk_codepipeline_merge_action/
+-rw-r--r--   0 hupe       (501) staff       (20)    20936 2024-04-17 18:35:41.000000 cloudcomponents.cdk-codepipeline-merge-action-2.3.0/src/cloudcomponents/cdk_codepipeline_merge_action/__init__.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.189175 cloudcomponents.cdk-codepipeline-merge-action-2.3.0/src/cloudcomponents/cdk_codepipeline_merge_action/_jsii/
+-rw-r--r--   0 hupe       (501) staff       (20)      455 2024-04-17 18:35:41.000000 cloudcomponents.cdk-codepipeline-merge-action-2.3.0/src/cloudcomponents/cdk_codepipeline_merge_action/_jsii/__init__.py
+-rw-r--r--   0 hupe       (501) staff       (20)  1339291 2024-04-17 18:35:41.000000 cloudcomponents.cdk-codepipeline-merge-action-2.3.0/src/cloudcomponents/cdk_codepipeline_merge_action/_jsii/cdk-codepipeline-merge-action@2.3.0.jsii.tgz
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:35:41.000000 cloudcomponents.cdk-codepipeline-merge-action-2.3.0/src/cloudcomponents/cdk_codepipeline_merge_action/py.typed
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.188349 cloudcomponents.cdk-codepipeline-merge-action-2.3.0/src/cloudcomponents.cdk_codepipeline_merge_action.egg-info/
+-rw-r--r--   0 hupe       (501) staff       (20)     3670 2024-04-17 18:35:46.000000 cloudcomponents.cdk-codepipeline-merge-action-2.3.0/src/cloudcomponents.cdk_codepipeline_merge_action.egg-info/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)      707 2024-04-17 18:35:46.000000 cloudcomponents.cdk-codepipeline-merge-action-2.3.0/src/cloudcomponents.cdk_codepipeline_merge_action.egg-info/SOURCES.txt
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:35:46.000000 cloudcomponents.cdk-codepipeline-merge-action-2.3.0/src/cloudcomponents.cdk_codepipeline_merge_action.egg-info/dependency_links.txt
+-rw-r--r--   0 hupe       (501) staff       (20)      112 2024-04-17 18:35:46.000000 cloudcomponents.cdk-codepipeline-merge-action-2.3.0/src/cloudcomponents.cdk_codepipeline_merge_action.egg-info/requires.txt
+-rw-r--r--   0 hupe       (501) staff       (20)       16 2024-04-17 18:35:46.000000 cloudcomponents.cdk-codepipeline-merge-action-2.3.0/src/cloudcomponents.cdk_codepipeline_merge_action.egg-info/top_level.txt
```

### Comparing `cloudcomponents.cdk-codepipeline-merge-action-2.2.0/LICENSE` & `cloudcomponents.cdk-codepipeline-merge-action-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-codepipeline-merge-action-2.2.0/PKG-INFO` & `cloudcomponents.cdk-codepipeline-merge-action-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-codepipeline-merge-action
-Version: 2.2.0
+Version: 2.3.0
 Summary: Cdk component that automatically merge branches in codepipelines
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-codepipeline-merge-action-2.2.0/README.md` & `cloudcomponents.cdk-codepipeline-merge-action-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-codepipeline-merge-action-2.2.0/setup.py` & `cloudcomponents.cdk-codepipeline-merge-action-2.3.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudcomponents.cdk-codepipeline-merge-action",
-    "version": "2.2.0",
+    "version": "2.3.0",
     "description": "Cdk component that automatically merge branches in codepipelines",
     "license": "MIT",
     "url": "https://github.com/cloudcomponents/cdk-constructs",
     "long_description_content_type": "text/markdown",
     "author": "hupe1980",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cloudcomponents.cdk_codepipeline_merge_action",
         "cloudcomponents.cdk_codepipeline_merge_action._jsii"
     ],
     "package_data": {
         "cloudcomponents.cdk_codepipeline_merge_action._jsii": [
-            "cdk-codepipeline-merge-action@2.2.0.jsii.tgz"
+            "cdk-codepipeline-merge-action@2.3.0.jsii.tgz"
         ],
         "cloudcomponents.cdk_codepipeline_merge_action": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cloudcomponents.cdk-codepipeline-merge-action-2.2.0/src/cloudcomponents/cdk_codepipeline_merge_action/__init__.py` & `cloudcomponents.cdk-codepipeline-merge-action-2.3.0/src/cloudcomponents/cdk_codepipeline_merge_action/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-codepipeline-merge-action-2.2.0/src/cloudcomponents.cdk_codepipeline_merge_action.egg-info/PKG-INFO` & `cloudcomponents.cdk-codepipeline-merge-action-2.3.0/src/cloudcomponents.cdk_codepipeline_merge_action.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-codepipeline-merge-action
-Version: 2.2.0
+Version: 2.3.0
 Summary: Cdk component that automatically merge branches in codepipelines
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-codepipeline-merge-action-2.2.0/src/cloudcomponents.cdk_codepipeline_merge_action.egg-info/SOURCES.txt` & `cloudcomponents.cdk-codepipeline-merge-action-2.3.0/src/cloudcomponents.cdk_codepipeline_merge_action.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cloudcomponents.cdk_codepipeline_merge_action.egg-info/SOURCES.txt
 src/cloudcomponents.cdk_codepipeline_merge_action.egg-info/dependency_links.txt
 src/cloudcomponents.cdk_codepipeline_merge_action.egg-info/requires.txt
 src/cloudcomponents.cdk_codepipeline_merge_action.egg-info/top_level.txt
 src/cloudcomponents/cdk_codepipeline_merge_action/__init__.py
 src/cloudcomponents/cdk_codepipeline_merge_action/py.typed
 src/cloudcomponents/cdk_codepipeline_merge_action/_jsii/__init__.py
-src/cloudcomponents/cdk_codepipeline_merge_action/_jsii/cdk-codepipeline-merge-action@2.2.0.jsii.tgz
+src/cloudcomponents/cdk_codepipeline_merge_action/_jsii/cdk-codepipeline-merge-action@2.3.0.jsii.tgz
```

