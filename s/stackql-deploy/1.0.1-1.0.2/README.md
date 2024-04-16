# Comparing `tmp/stackql_deploy-1.0.1.tar.gz` & `tmp/stackql_deploy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackql_deploy-1.0.1.tar", last modified: Tue Apr 16 21:31:42 2024, max compression
+gzip compressed data, was "stackql_deploy-1.0.2.tar", last modified: Tue Apr 16 21:35:30 2024, max compression
```

## Comparing `stackql_deploy-1.0.1.tar` & `stackql_deploy-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 21:31:42.790046 stackql_deploy-1.0.1/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 stackql_deploy-1.0.1/LICENSE
--rwxrwxrwx   0 javen     (1000) javen     (1000)    10342 2024-04-16 21:31:42.774349 stackql_deploy-1.0.1/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)     9719 2024-04-16 21:29:08.000000 stackql_deploy-1.0.1/README.rst
--rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-04-16 21:31:42.791045 stackql_deploy-1.0.1/setup.cfg
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1300 2024-04-16 21:31:36.000000 stackql_deploy-1.0.1/setup.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 21:31:42.600012 stackql_deploy-1.0.1/stackql_deploy/
--rwxrwxrwx   0 javen     (1000) javen     (1000)       23 2024-04-16 21:31:36.000000 stackql_deploy-1.0.1/stackql_deploy/__init__.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     3965 2024-04-16 05:13:28.000000 stackql_deploy-1.0.1/stackql_deploy/cli.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 21:31:42.756295 stackql_deploy-1.0.1/stackql_deploy.egg-info/
--rwxrwxrwx   0 javen     (1000) javen     (1000)    10342 2024-04-16 21:31:42.000000 stackql_deploy-1.0.1/stackql_deploy.egg-info/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)      306 2024-04-16 21:31:42.000000 stackql_deploy-1.0.1/stackql_deploy.egg-info/SOURCES.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-04-16 21:31:42.000000 stackql_deploy-1.0.1/stackql_deploy.egg-info/dependency_links.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       58 2024-04-16 21:31:42.000000 stackql_deploy-1.0.1/stackql_deploy.egg-info/entry_points.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       37 2024-04-16 21:31:42.000000 stackql_deploy-1.0.1/stackql_deploy.egg-info/requires.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       15 2024-04-16 21:31:42.000000 stackql_deploy-1.0.1/stackql_deploy.egg-info/top_level.txt
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 21:35:30.176355 stackql_deploy-1.0.2/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 stackql_deploy-1.0.2/LICENSE
+-rwxrwxrwx   0 javen     (1000) javen     (1000)    10291 2024-04-16 21:35:30.160123 stackql_deploy-1.0.2/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     9668 2024-04-16 21:34:54.000000 stackql_deploy-1.0.2/README.rst
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-04-16 21:35:30.178878 stackql_deploy-1.0.2/setup.cfg
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1300 2024-04-16 21:35:05.000000 stackql_deploy-1.0.2/setup.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 21:35:29.908845 stackql_deploy-1.0.2/stackql_deploy/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       23 2024-04-16 21:35:05.000000 stackql_deploy-1.0.2/stackql_deploy/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     3965 2024-04-16 05:13:28.000000 stackql_deploy-1.0.2/stackql_deploy/cli.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 21:35:30.140536 stackql_deploy-1.0.2/stackql_deploy.egg-info/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)    10291 2024-04-16 21:35:29.000000 stackql_deploy-1.0.2/stackql_deploy.egg-info/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      306 2024-04-16 21:35:29.000000 stackql_deploy-1.0.2/stackql_deploy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-04-16 21:35:29.000000 stackql_deploy-1.0.2/stackql_deploy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       58 2024-04-16 21:35:29.000000 stackql_deploy-1.0.2/stackql_deploy.egg-info/entry_points.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       37 2024-04-16 21:35:29.000000 stackql_deploy-1.0.2/stackql_deploy.egg-info/requires.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       15 2024-04-16 21:35:29.000000 stackql_deploy-1.0.2/stackql_deploy.egg-info/top_level.txt
```

### Comparing `stackql_deploy-1.0.1/LICENSE` & `stackql_deploy-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.1/PKG-INFO` & `stackql_deploy-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackql-deploy
-Version: 1.0.1
+Version: 1.0.2
 Summary: Model driven resource provisioning and deployment framework using StackQL.
 Home-page: https://github.com/stackql/stackql-deploy
 Author: Jeffrey Aven
 Author-email: javen@stackql.io
 License: MIT
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -23,17 +23,17 @@
 Requires-Dist: pystackql
 
 .. image:: https://stackql.io/img/stackql-logo-bold.png
     :alt: "stackql logo"
     :target: https://github.com/stackql/stackql
     :align: center
 
-===========================================================================================
-stackql-deploy - Model driven resource provisioning and deployment framework using StackQL.
-===========================================================================================
+==========================================================================
+Model driven resource provisioning and deployment framework using StackQL.
+==========================================================================
 
 .. .. image:: https://readthedocs.org/projects/pystackql/badge/?version=latest
 ..    :target: https://pystackql.readthedocs.io/en/latest/
 ..    :alt: Documentation Status
 
 .. image:: https://img.shields.io/pypi/v/stackql-deploy
    :target: https://pypi.org/project/stackql-deploy/
```

### Comparing `stackql_deploy-1.0.1/README.rst` & `stackql_deploy-1.0.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. image:: https://stackql.io/img/stackql-logo-bold.png
     :alt: "stackql logo"
     :target: https://github.com/stackql/stackql
     :align: center
 
-===========================================================================================
-stackql-deploy - Model driven resource provisioning and deployment framework using StackQL.
-===========================================================================================
+==========================================================================
+Model driven resource provisioning and deployment framework using StackQL.
+==========================================================================
 
 .. .. image:: https://readthedocs.org/projects/pystackql/badge/?version=latest
 ..    :target: https://pystackql.readthedocs.io/en/latest/
 ..    :alt: Documentation Status
 
 .. image:: https://img.shields.io/pypi/v/stackql-deploy
    :target: https://pypi.org/project/stackql-deploy/
```

### Comparing `stackql_deploy-1.0.1/setup.py` & `stackql_deploy-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.rst', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='stackql-deploy',
-    version='1.0.1',
+    version='1.0.2',
     description='Model driven resource provisioning and deployment framework using StackQL.',
     long_description=readme,
     author='Jeffrey Aven',
     author_email='javen@stackql.io',
     url='https://github.com/stackql/stackql-deploy',
     license='MIT',
     packages=find_packages(),
```

### Comparing `stackql_deploy-1.0.1/stackql_deploy/cli.py` & `stackql_deploy-1.0.2/stackql_deploy/cli.py`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.1/stackql_deploy.egg-info/PKG-INFO` & `stackql_deploy-1.0.2/stackql_deploy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackql-deploy
-Version: 1.0.1
+Version: 1.0.2
 Summary: Model driven resource provisioning and deployment framework using StackQL.
 Home-page: https://github.com/stackql/stackql-deploy
 Author: Jeffrey Aven
 Author-email: javen@stackql.io
 License: MIT
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -23,17 +23,17 @@
 Requires-Dist: pystackql
 
 .. image:: https://stackql.io/img/stackql-logo-bold.png
     :alt: "stackql logo"
     :target: https://github.com/stackql/stackql
     :align: center
 
-===========================================================================================
-stackql-deploy - Model driven resource provisioning and deployment framework using StackQL.
-===========================================================================================
+==========================================================================
+Model driven resource provisioning and deployment framework using StackQL.
+==========================================================================
 
 .. .. image:: https://readthedocs.org/projects/pystackql/badge/?version=latest
 ..    :target: https://pystackql.readthedocs.io/en/latest/
 ..    :alt: Documentation Status
 
 .. image:: https://img.shields.io/pypi/v/stackql-deploy
    :target: https://pypi.org/project/stackql-deploy/
```

