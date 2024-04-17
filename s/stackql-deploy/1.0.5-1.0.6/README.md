# Comparing `tmp/stackql_deploy-1.0.5.tar.gz` & `tmp/stackql_deploy-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackql_deploy-1.0.5.tar", last modified: Tue Apr 16 23:32:13 2024, max compression
+gzip compressed data, was "stackql_deploy-1.0.6.tar", last modified: Tue Apr 16 23:36:38 2024, max compression
```

## Comparing `stackql_deploy-1.0.5.tar` & `stackql_deploy-1.0.6.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:32:13.209099 stackql_deploy-1.0.5/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 stackql_deploy-1.0.5/LICENSE
--rwxrwxrwx   0 javen     (1000) javen     (1000)     8892 2024-04-16 23:32:13.194885 stackql_deploy-1.0.5/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)     8214 2024-04-16 23:03:24.000000 stackql_deploy-1.0.5/README.rst
--rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-04-16 23:32:13.210617 stackql_deploy-1.0.5/setup.cfg
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1300 2024-04-16 23:31:56.000000 stackql_deploy-1.0.5/setup.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:32:12.750799 stackql_deploy-1.0.5/stackql_deploy/
--rwxrwxrwx   0 javen     (1000) javen     (1000)       23 2024-04-16 23:31:56.000000 stackql_deploy-1.0.5/stackql_deploy/__init__.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     3687 2024-04-16 23:18:07.000000 stackql_deploy-1.0.5/stackql_deploy/cli.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:32:13.129269 stackql_deploy-1.0.5/stackql_deploy/lib/
--rwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:31:31.000000 stackql_deploy-1.0.5/stackql_deploy/lib/__init__.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)      333 2024-04-12 03:18:07.000000 stackql_deploy-1.0.5/stackql_deploy/lib/bootstrap.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     3647 2024-04-16 02:40:32.000000 stackql_deploy-1.0.5/stackql_deploy/lib/config.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     2782 2024-04-16 03:47:18.000000 stackql_deploy-1.0.5/stackql_deploy/lib/templating.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     5279 2024-04-16 03:46:51.000000 stackql_deploy-1.0.5/stackql_deploy/lib/utils.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:32:13.176156 stackql_deploy-1.0.5/stackql_deploy.egg-info/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     8892 2024-04-16 23:32:12.000000 stackql_deploy-1.0.5/stackql_deploy.egg-info/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)      459 2024-04-16 23:32:12.000000 stackql_deploy-1.0.5/stackql_deploy.egg-info/SOURCES.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-04-16 23:32:12.000000 stackql_deploy-1.0.5/stackql_deploy.egg-info/dependency_links.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       58 2024-04-16 23:32:12.000000 stackql_deploy-1.0.5/stackql_deploy.egg-info/entry_points.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       37 2024-04-16 23:32:12.000000 stackql_deploy-1.0.5/stackql_deploy.egg-info/requires.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       15 2024-04-16 23:32:12.000000 stackql_deploy-1.0.5/stackql_deploy.egg-info/top_level.txt
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:36:38.461588 stackql_deploy-1.0.6/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 stackql_deploy-1.0.6/LICENSE
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     8892 2024-04-16 23:36:38.448344 stackql_deploy-1.0.6/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     8214 2024-04-16 23:03:24.000000 stackql_deploy-1.0.6/README.rst
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-04-16 23:36:38.463303 stackql_deploy-1.0.6/setup.cfg
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1300 2024-04-16 23:36:28.000000 stackql_deploy-1.0.6/setup.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:36:37.827758 stackql_deploy-1.0.6/stackql_deploy/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       23 2024-04-16 23:36:28.000000 stackql_deploy-1.0.6/stackql_deploy/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     3687 2024-04-16 23:18:07.000000 stackql_deploy-1.0.6/stackql_deploy/cli.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:36:38.192966 stackql_deploy-1.0.6/stackql_deploy/cmd/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:31:31.000000 stackql_deploy-1.0.6/stackql_deploy/cmd/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     6291 2024-04-16 23:16:19.000000 stackql_deploy-1.0.6/stackql_deploy/cmd/build.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     3433 2024-04-16 23:17:44.000000 stackql_deploy-1.0.6/stackql_deploy/cmd/teardown.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     2542 2024-04-16 23:17:44.000000 stackql_deploy-1.0.6/stackql_deploy/cmd/test.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:36:38.382306 stackql_deploy-1.0.6/stackql_deploy/lib/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:31:31.000000 stackql_deploy-1.0.6/stackql_deploy/lib/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      333 2024-04-12 03:18:07.000000 stackql_deploy-1.0.6/stackql_deploy/lib/bootstrap.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     3647 2024-04-16 02:40:32.000000 stackql_deploy-1.0.6/stackql_deploy/lib/config.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     2782 2024-04-16 03:47:18.000000 stackql_deploy-1.0.6/stackql_deploy/lib/templating.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     5279 2024-04-16 03:46:51.000000 stackql_deploy-1.0.6/stackql_deploy/lib/utils.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:36:38.432724 stackql_deploy-1.0.6/stackql_deploy.egg-info/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     8892 2024-04-16 23:36:37.000000 stackql_deploy-1.0.6/stackql_deploy.egg-info/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      576 2024-04-16 23:36:37.000000 stackql_deploy-1.0.6/stackql_deploy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-04-16 23:36:37.000000 stackql_deploy-1.0.6/stackql_deploy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       58 2024-04-16 23:36:37.000000 stackql_deploy-1.0.6/stackql_deploy.egg-info/entry_points.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       37 2024-04-16 23:36:37.000000 stackql_deploy-1.0.6/stackql_deploy.egg-info/requires.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       15 2024-04-16 23:36:37.000000 stackql_deploy-1.0.6/stackql_deploy.egg-info/top_level.txt
```

### Comparing `stackql_deploy-1.0.5/LICENSE` & `stackql_deploy-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.5/PKG-INFO` & `stackql_deploy-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackql-deploy
-Version: 1.0.5
+Version: 1.0.6
 Summary: Model driven resource provisioning and deployment framework using StackQL.
 Home-page: https://github.com/stackql/stackql-deploy
 Author: Jeffrey Aven
 Author-email: javen@stackql.io
 License: MIT
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
```

### Comparing `stackql_deploy-1.0.5/README.rst` & `stackql_deploy-1.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.5/setup.py` & `stackql_deploy-1.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.rst', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='stackql-deploy',
-    version='1.0.5',
+    version='1.0.6',
     description='Model driven resource provisioning and deployment framework using StackQL.',
     long_description=readme,
     author='Jeffrey Aven',
     author_email='javen@stackql.io',
     url='https://github.com/stackql/stackql-deploy',
     license='MIT',
     packages=find_packages(),
```

### Comparing `stackql_deploy-1.0.5/stackql_deploy/cli.py` & `stackql_deploy-1.0.6/stackql_deploy/cli.py`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.5/stackql_deploy/lib/config.py` & `stackql_deploy-1.0.6/stackql_deploy/lib/config.py`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.5/stackql_deploy/lib/templating.py` & `stackql_deploy-1.0.6/stackql_deploy/lib/templating.py`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.5/stackql_deploy/lib/utils.py` & `stackql_deploy-1.0.6/stackql_deploy/lib/utils.py`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.5/stackql_deploy.egg-info/PKG-INFO` & `stackql_deploy-1.0.6/stackql_deploy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackql-deploy
-Version: 1.0.5
+Version: 1.0.6
 Summary: Model driven resource provisioning and deployment framework using StackQL.
 Home-page: https://github.com/stackql/stackql-deploy
 Author: Jeffrey Aven
 Author-email: javen@stackql.io
 License: MIT
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
```

