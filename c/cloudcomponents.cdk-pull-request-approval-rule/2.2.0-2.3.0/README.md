# Comparing `tmp/cloudcomponents.cdk-pull-request-approval-rule-2.2.0.tar.gz` & `tmp/cloudcomponents.cdk-pull-request-approval-rule-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudcomponents.cdk-pull-request-approval-rule-2.2.0.tar", last modified: Mon Mar 25 18:25:55 2024, max compression
+gzip compressed data, was "cloudcomponents.cdk-pull-request-approval-rule-2.3.0.tar", last modified: Wed Apr 17 18:35:56 2024, max compression
```

## Comparing `cloudcomponents.cdk-pull-request-approval-rule-2.2.0.tar` & `cloudcomponents.cdk-pull-request-approval-rule-2.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:55.138749 cloudcomponents.cdk-pull-request-approval-rule-2.2.0/
--rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-03-25 18:25:51.000000 cloudcomponents.cdk-pull-request-approval-rule-2.2.0/LICENSE
--rw-r--r--   0 hupe       (501) staff       (20)       23 2024-03-25 18:25:51.000000 cloudcomponents.cdk-pull-request-approval-rule-2.2.0/MANIFEST.in
--rw-r--r--   0 hupe       (501) staff       (20)     5252 2024-03-25 18:25:55.138520 cloudcomponents.cdk-pull-request-approval-rule-2.2.0/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)     4362 2024-03-25 18:25:51.000000 cloudcomponents.cdk-pull-request-approval-rule-2.2.0/README.md
--rw-r--r--   0 hupe       (501) staff       (20)      234 2024-03-25 18:25:51.000000 cloudcomponents.cdk-pull-request-approval-rule-2.2.0/pyproject.toml
--rw-r--r--   0 hupe       (501) staff       (20)       38 2024-03-25 18:25:55.138795 cloudcomponents.cdk-pull-request-approval-rule-2.2.0/setup.cfg
--rw-r--r--   0 hupe       (501) staff       (20)     1880 2024-03-25 18:25:51.000000 cloudcomponents.cdk-pull-request-approval-rule-2.2.0/setup.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:55.135813 cloudcomponents.cdk-pull-request-approval-rule-2.2.0/src/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:55.135890 cloudcomponents.cdk-pull-request-approval-rule-2.2.0/src/cloudcomponents/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:55.137930 cloudcomponents.cdk-pull-request-approval-rule-2.2.0/src/cloudcomponents/cdk_pull_request_approval_rule/
--rw-r--r--   0 hupe       (501) staff       (20)    22845 2024-03-25 18:25:51.000000 cloudcomponents.cdk-pull-request-approval-rule-2.2.0/src/cloudcomponents/cdk_pull_request_approval_rule/__init__.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:55.138215 cloudcomponents.cdk-pull-request-approval-rule-2.2.0/src/cloudcomponents/cdk_pull_request_approval_rule/_jsii/
--rw-r--r--   0 hupe       (501) staff       (20)      457 2024-03-25 18:25:51.000000 cloudcomponents.cdk-pull-request-approval-rule-2.2.0/src/cloudcomponents/cdk_pull_request_approval_rule/_jsii/__init__.py
--rw-r--r--   0 hupe       (501) staff       (20)   130891 2024-03-25 18:25:51.000000 cloudcomponents.cdk-pull-request-approval-rule-2.2.0/src/cloudcomponents/cdk_pull_request_approval_rule/_jsii/cdk-pull-request-approval-rule@2.2.0.jsii.tgz
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-03-25 18:25:51.000000 cloudcomponents.cdk-pull-request-approval-rule-2.2.0/src/cloudcomponents/cdk_pull_request_approval_rule/py.typed
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:55.137602 cloudcomponents.cdk-pull-request-approval-rule-2.2.0/src/cloudcomponents.cdk_pull_request_approval_rule.egg-info/
--rw-r--r--   0 hupe       (501) staff       (20)     5252 2024-03-25 18:25:55.000000 cloudcomponents.cdk-pull-request-approval-rule-2.2.0/src/cloudcomponents.cdk_pull_request_approval_rule.egg-info/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)      717 2024-03-25 18:25:55.000000 cloudcomponents.cdk-pull-request-approval-rule-2.2.0/src/cloudcomponents.cdk_pull_request_approval_rule.egg-info/SOURCES.txt
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-03-25 18:25:55.000000 cloudcomponents.cdk-pull-request-approval-rule-2.2.0/src/cloudcomponents.cdk_pull_request_approval_rule.egg-info/dependency_links.txt
--rw-r--r--   0 hupe       (501) staff       (20)      112 2024-03-25 18:25:55.000000 cloudcomponents.cdk-pull-request-approval-rule-2.2.0/src/cloudcomponents.cdk_pull_request_approval_rule.egg-info/requires.txt
--rw-r--r--   0 hupe       (501) staff       (20)       16 2024-03-25 18:25:55.000000 cloudcomponents.cdk-pull-request-approval-rule-2.2.0/src/cloudcomponents.cdk_pull_request_approval_rule.egg-info/top_level.txt
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:56.376803 cloudcomponents.cdk-pull-request-approval-rule-2.3.0/
+-rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-04-17 18:35:53.000000 cloudcomponents.cdk-pull-request-approval-rule-2.3.0/LICENSE
+-rw-r--r--   0 hupe       (501) staff       (20)       23 2024-04-17 18:35:53.000000 cloudcomponents.cdk-pull-request-approval-rule-2.3.0/MANIFEST.in
+-rw-r--r--   0 hupe       (501) staff       (20)     5252 2024-04-17 18:35:56.376511 cloudcomponents.cdk-pull-request-approval-rule-2.3.0/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)     4362 2024-04-17 18:35:53.000000 cloudcomponents.cdk-pull-request-approval-rule-2.3.0/README.md
+-rw-r--r--   0 hupe       (501) staff       (20)      234 2024-04-17 18:35:53.000000 cloudcomponents.cdk-pull-request-approval-rule-2.3.0/pyproject.toml
+-rw-r--r--   0 hupe       (501) staff       (20)       38 2024-04-17 18:35:56.376851 cloudcomponents.cdk-pull-request-approval-rule-2.3.0/setup.cfg
+-rw-r--r--   0 hupe       (501) staff       (20)     1880 2024-04-17 18:35:53.000000 cloudcomponents.cdk-pull-request-approval-rule-2.3.0/setup.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:56.372544 cloudcomponents.cdk-pull-request-approval-rule-2.3.0/src/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:56.372604 cloudcomponents.cdk-pull-request-approval-rule-2.3.0/src/cloudcomponents/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:56.374368 cloudcomponents.cdk-pull-request-approval-rule-2.3.0/src/cloudcomponents/cdk_pull_request_approval_rule/
+-rw-r--r--   0 hupe       (501) staff       (20)    22845 2024-04-17 18:35:53.000000 cloudcomponents.cdk-pull-request-approval-rule-2.3.0/src/cloudcomponents/cdk_pull_request_approval_rule/__init__.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:56.374638 cloudcomponents.cdk-pull-request-approval-rule-2.3.0/src/cloudcomponents/cdk_pull_request_approval_rule/_jsii/
+-rw-r--r--   0 hupe       (501) staff       (20)      457 2024-04-17 18:35:53.000000 cloudcomponents.cdk-pull-request-approval-rule-2.3.0/src/cloudcomponents/cdk_pull_request_approval_rule/_jsii/__init__.py
+-rw-r--r--   0 hupe       (501) staff       (20)  2532026 2024-04-17 18:35:53.000000 cloudcomponents.cdk-pull-request-approval-rule-2.3.0/src/cloudcomponents/cdk_pull_request_approval_rule/_jsii/cdk-pull-request-approval-rule@2.3.0.jsii.tgz
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:35:53.000000 cloudcomponents.cdk-pull-request-approval-rule-2.3.0/src/cloudcomponents/cdk_pull_request_approval_rule/py.typed
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:56.374079 cloudcomponents.cdk-pull-request-approval-rule-2.3.0/src/cloudcomponents.cdk_pull_request_approval_rule.egg-info/
+-rw-r--r--   0 hupe       (501) staff       (20)     5252 2024-04-17 18:35:56.000000 cloudcomponents.cdk-pull-request-approval-rule-2.3.0/src/cloudcomponents.cdk_pull_request_approval_rule.egg-info/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)      717 2024-04-17 18:35:56.000000 cloudcomponents.cdk-pull-request-approval-rule-2.3.0/src/cloudcomponents.cdk_pull_request_approval_rule.egg-info/SOURCES.txt
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:35:56.000000 cloudcomponents.cdk-pull-request-approval-rule-2.3.0/src/cloudcomponents.cdk_pull_request_approval_rule.egg-info/dependency_links.txt
+-rw-r--r--   0 hupe       (501) staff       (20)      112 2024-04-17 18:35:56.000000 cloudcomponents.cdk-pull-request-approval-rule-2.3.0/src/cloudcomponents.cdk_pull_request_approval_rule.egg-info/requires.txt
+-rw-r--r--   0 hupe       (501) staff       (20)       16 2024-04-17 18:35:56.000000 cloudcomponents.cdk-pull-request-approval-rule-2.3.0/src/cloudcomponents.cdk_pull_request_approval_rule.egg-info/top_level.txt
```

### Comparing `cloudcomponents.cdk-pull-request-approval-rule-2.2.0/LICENSE` & `cloudcomponents.cdk-pull-request-approval-rule-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-pull-request-approval-rule-2.2.0/PKG-INFO` & `cloudcomponents.cdk-pull-request-approval-rule-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-pull-request-approval-rule
-Version: 2.2.0
+Version: 2.3.0
 Summary: CodeCommit pull request approval rules to enforcing your pull request workflow
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-pull-request-approval-rule-2.2.0/README.md` & `cloudcomponents.cdk-pull-request-approval-rule-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-pull-request-approval-rule-2.2.0/setup.py` & `cloudcomponents.cdk-pull-request-approval-rule-2.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudcomponents.cdk-pull-request-approval-rule",
-    "version": "2.2.0",
+    "version": "2.3.0",
     "description": "CodeCommit pull request approval rules to enforcing your pull request workflow",
     "license": "MIT",
     "url": "https://github.com/cloudcomponents/cdk-constructs",
     "long_description_content_type": "text/markdown",
     "author": "hupe1980",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cloudcomponents.cdk_pull_request_approval_rule",
         "cloudcomponents.cdk_pull_request_approval_rule._jsii"
     ],
     "package_data": {
         "cloudcomponents.cdk_pull_request_approval_rule._jsii": [
-            "cdk-pull-request-approval-rule@2.2.0.jsii.tgz"
+            "cdk-pull-request-approval-rule@2.3.0.jsii.tgz"
         ],
         "cloudcomponents.cdk_pull_request_approval_rule": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cloudcomponents.cdk-pull-request-approval-rule-2.2.0/src/cloudcomponents/cdk_pull_request_approval_rule/__init__.py` & `cloudcomponents.cdk-pull-request-approval-rule-2.3.0/src/cloudcomponents/cdk_pull_request_approval_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-pull-request-approval-rule-2.2.0/src/cloudcomponents.cdk_pull_request_approval_rule.egg-info/PKG-INFO` & `cloudcomponents.cdk-pull-request-approval-rule-2.3.0/src/cloudcomponents.cdk_pull_request_approval_rule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-pull-request-approval-rule
-Version: 2.2.0
+Version: 2.3.0
 Summary: CodeCommit pull request approval rules to enforcing your pull request workflow
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-pull-request-approval-rule-2.2.0/src/cloudcomponents.cdk_pull_request_approval_rule.egg-info/SOURCES.txt` & `cloudcomponents.cdk-pull-request-approval-rule-2.3.0/src/cloudcomponents.cdk_pull_request_approval_rule.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cloudcomponents.cdk_pull_request_approval_rule.egg-info/SOURCES.txt
 src/cloudcomponents.cdk_pull_request_approval_rule.egg-info/dependency_links.txt
 src/cloudcomponents.cdk_pull_request_approval_rule.egg-info/requires.txt
 src/cloudcomponents.cdk_pull_request_approval_rule.egg-info/top_level.txt
 src/cloudcomponents/cdk_pull_request_approval_rule/__init__.py
 src/cloudcomponents/cdk_pull_request_approval_rule/py.typed
 src/cloudcomponents/cdk_pull_request_approval_rule/_jsii/__init__.py
-src/cloudcomponents/cdk_pull_request_approval_rule/_jsii/cdk-pull-request-approval-rule@2.2.0.jsii.tgz
+src/cloudcomponents/cdk_pull_request_approval_rule/_jsii/cdk-pull-request-approval-rule@2.3.0.jsii.tgz
```

