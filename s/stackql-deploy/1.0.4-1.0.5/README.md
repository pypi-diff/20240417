# Comparing `tmp/stackql_deploy-1.0.4.tar.gz` & `tmp/stackql_deploy-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackql_deploy-1.0.4.tar", last modified: Tue Apr 16 23:23:16 2024, max compression
+gzip compressed data, was "stackql_deploy-1.0.5.tar", last modified: Tue Apr 16 23:32:13 2024, max compression
```

## Comparing `stackql_deploy-1.0.4.tar` & `stackql_deploy-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,22 @@
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:23:16.971059 stackql_deploy-1.0.4/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 stackql_deploy-1.0.4/LICENSE
--rwxrwxrwx   0 javen     (1000) javen     (1000)     8892 2024-04-16 23:23:16.957812 stackql_deploy-1.0.4/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)     8214 2024-04-16 23:03:24.000000 stackql_deploy-1.0.4/README.rst
--rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-04-16 23:23:16.972767 stackql_deploy-1.0.4/setup.cfg
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1300 2024-04-16 22:58:08.000000 stackql_deploy-1.0.4/setup.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:23:16.728353 stackql_deploy-1.0.4/stackql_deploy/
--rwxrwxrwx   0 javen     (1000) javen     (1000)       23 2024-04-16 22:58:08.000000 stackql_deploy-1.0.4/stackql_deploy/__init__.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     3687 2024-04-16 23:18:07.000000 stackql_deploy-1.0.4/stackql_deploy/cli.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:23:16.942042 stackql_deploy-1.0.4/stackql_deploy.egg-info/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     8892 2024-04-16 23:23:16.000000 stackql_deploy-1.0.4/stackql_deploy.egg-info/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)      306 2024-04-16 23:23:16.000000 stackql_deploy-1.0.4/stackql_deploy.egg-info/SOURCES.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-04-16 23:23:16.000000 stackql_deploy-1.0.4/stackql_deploy.egg-info/dependency_links.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       58 2024-04-16 23:23:16.000000 stackql_deploy-1.0.4/stackql_deploy.egg-info/entry_points.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       37 2024-04-16 23:23:16.000000 stackql_deploy-1.0.4/stackql_deploy.egg-info/requires.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       15 2024-04-16 23:23:16.000000 stackql_deploy-1.0.4/stackql_deploy.egg-info/top_level.txt
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:32:13.209099 stackql_deploy-1.0.5/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 stackql_deploy-1.0.5/LICENSE
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     8892 2024-04-16 23:32:13.194885 stackql_deploy-1.0.5/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     8214 2024-04-16 23:03:24.000000 stackql_deploy-1.0.5/README.rst
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-04-16 23:32:13.210617 stackql_deploy-1.0.5/setup.cfg
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1300 2024-04-16 23:31:56.000000 stackql_deploy-1.0.5/setup.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:32:12.750799 stackql_deploy-1.0.5/stackql_deploy/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       23 2024-04-16 23:31:56.000000 stackql_deploy-1.0.5/stackql_deploy/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     3687 2024-04-16 23:18:07.000000 stackql_deploy-1.0.5/stackql_deploy/cli.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:32:13.129269 stackql_deploy-1.0.5/stackql_deploy/lib/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:31:31.000000 stackql_deploy-1.0.5/stackql_deploy/lib/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      333 2024-04-12 03:18:07.000000 stackql_deploy-1.0.5/stackql_deploy/lib/bootstrap.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     3647 2024-04-16 02:40:32.000000 stackql_deploy-1.0.5/stackql_deploy/lib/config.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     2782 2024-04-16 03:47:18.000000 stackql_deploy-1.0.5/stackql_deploy/lib/templating.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     5279 2024-04-16 03:46:51.000000 stackql_deploy-1.0.5/stackql_deploy/lib/utils.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:32:13.176156 stackql_deploy-1.0.5/stackql_deploy.egg-info/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     8892 2024-04-16 23:32:12.000000 stackql_deploy-1.0.5/stackql_deploy.egg-info/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      459 2024-04-16 23:32:12.000000 stackql_deploy-1.0.5/stackql_deploy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-04-16 23:32:12.000000 stackql_deploy-1.0.5/stackql_deploy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       58 2024-04-16 23:32:12.000000 stackql_deploy-1.0.5/stackql_deploy.egg-info/entry_points.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       37 2024-04-16 23:32:12.000000 stackql_deploy-1.0.5/stackql_deploy.egg-info/requires.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       15 2024-04-16 23:32:12.000000 stackql_deploy-1.0.5/stackql_deploy.egg-info/top_level.txt
```

### Comparing `stackql_deploy-1.0.4/LICENSE` & `stackql_deploy-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.4/PKG-INFO` & `stackql_deploy-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackql-deploy
-Version: 1.0.4
+Version: 1.0.5
 Summary: Model driven resource provisioning and deployment framework using StackQL.
 Home-page: https://github.com/stackql/stackql-deploy
 Author: Jeffrey Aven
 Author-email: javen@stackql.io
 License: MIT
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
```

### Comparing `stackql_deploy-1.0.4/README.rst` & `stackql_deploy-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.4/setup.py` & `stackql_deploy-1.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.rst', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='stackql-deploy',
-    version='1.0.4',
+    version='1.0.5',
     description='Model driven resource provisioning and deployment framework using StackQL.',
     long_description=readme,
     author='Jeffrey Aven',
     author_email='javen@stackql.io',
     url='https://github.com/stackql/stackql-deploy',
     license='MIT',
     packages=find_packages(),
```

### Comparing `stackql_deploy-1.0.4/stackql_deploy/cli.py` & `stackql_deploy-1.0.5/stackql_deploy/cli.py`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.4/stackql_deploy.egg-info/PKG-INFO` & `stackql_deploy-1.0.5/stackql_deploy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackql-deploy
-Version: 1.0.4
+Version: 1.0.5
 Summary: Model driven resource provisioning and deployment framework using StackQL.
 Home-page: https://github.com/stackql/stackql-deploy
 Author: Jeffrey Aven
 Author-email: javen@stackql.io
 License: MIT
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
```

