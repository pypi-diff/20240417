# Comparing `tmp/stackql_deploy-1.0.2.tar.gz` & `tmp/stackql_deploy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackql_deploy-1.0.2.tar", last modified: Tue Apr 16 21:35:30 2024, max compression
+gzip compressed data, was "stackql_deploy-1.0.3.tar", last modified: Tue Apr 16 22:25:13 2024, max compression
```

## Comparing `stackql_deploy-1.0.2.tar` & `stackql_deploy-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 21:35:30.176355 stackql_deploy-1.0.2/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 stackql_deploy-1.0.2/LICENSE
--rwxrwxrwx   0 javen     (1000) javen     (1000)    10291 2024-04-16 21:35:30.160123 stackql_deploy-1.0.2/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)     9668 2024-04-16 21:34:54.000000 stackql_deploy-1.0.2/README.rst
--rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-04-16 21:35:30.178878 stackql_deploy-1.0.2/setup.cfg
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1300 2024-04-16 21:35:05.000000 stackql_deploy-1.0.2/setup.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 21:35:29.908845 stackql_deploy-1.0.2/stackql_deploy/
--rwxrwxrwx   0 javen     (1000) javen     (1000)       23 2024-04-16 21:35:05.000000 stackql_deploy-1.0.2/stackql_deploy/__init__.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     3965 2024-04-16 05:13:28.000000 stackql_deploy-1.0.2/stackql_deploy/cli.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 21:35:30.140536 stackql_deploy-1.0.2/stackql_deploy.egg-info/
--rwxrwxrwx   0 javen     (1000) javen     (1000)    10291 2024-04-16 21:35:29.000000 stackql_deploy-1.0.2/stackql_deploy.egg-info/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)      306 2024-04-16 21:35:29.000000 stackql_deploy-1.0.2/stackql_deploy.egg-info/SOURCES.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-04-16 21:35:29.000000 stackql_deploy-1.0.2/stackql_deploy.egg-info/dependency_links.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       58 2024-04-16 21:35:29.000000 stackql_deploy-1.0.2/stackql_deploy.egg-info/entry_points.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       37 2024-04-16 21:35:29.000000 stackql_deploy-1.0.2/stackql_deploy.egg-info/requires.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       15 2024-04-16 21:35:29.000000 stackql_deploy-1.0.2/stackql_deploy.egg-info/top_level.txt
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 22:25:13.256174 stackql_deploy-1.0.3/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 stackql_deploy-1.0.3/LICENSE
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     8895 2024-04-16 22:25:13.239631 stackql_deploy-1.0.3/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     8217 2024-04-16 22:05:57.000000 stackql_deploy-1.0.3/README.rst
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-04-16 22:25:13.257178 stackql_deploy-1.0.3/setup.cfg
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1300 2024-04-16 21:39:17.000000 stackql_deploy-1.0.3/setup.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 22:25:12.957263 stackql_deploy-1.0.3/stackql_deploy/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       23 2024-04-16 21:39:17.000000 stackql_deploy-1.0.3/stackql_deploy/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     3965 2024-04-16 05:13:28.000000 stackql_deploy-1.0.3/stackql_deploy/cli.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 22:25:13.218315 stackql_deploy-1.0.3/stackql_deploy.egg-info/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     8895 2024-04-16 22:25:12.000000 stackql_deploy-1.0.3/stackql_deploy.egg-info/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      306 2024-04-16 22:25:12.000000 stackql_deploy-1.0.3/stackql_deploy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-04-16 22:25:12.000000 stackql_deploy-1.0.3/stackql_deploy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       58 2024-04-16 22:25:12.000000 stackql_deploy-1.0.3/stackql_deploy.egg-info/entry_points.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       37 2024-04-16 22:25:12.000000 stackql_deploy-1.0.3/stackql_deploy.egg-info/requires.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       15 2024-04-16 22:25:12.000000 stackql_deploy-1.0.3/stackql_deploy.egg-info/top_level.txt
```

### Comparing `stackql_deploy-1.0.2/LICENSE` & `stackql_deploy-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.2/PKG-INFO` & `stackql_deploy-1.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackql-deploy
-Version: 1.0.2
+Version: 1.0.3
 Summary: Model driven resource provisioning and deployment framework using StackQL.
 Home-page: https://github.com/stackql/stackql-deploy
 Author: Jeffrey Aven
 Author-email: javen@stackql.io
 License: MIT
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -209,65 +209,10 @@
     /*+ postdeploy, retries=5, retry_delay=5 */
     SELECT COUNT(*) as count FROM azure.resources.resource_groups
     WHERE subscriptionId = '{{ subscription_id }}'
     AND resourceGroupName = '{{ resource_group_name }}'
     AND location = '{{ location }}'
     AND JSON_EXTRACT(properties, '$.provisioningState') = 'Succeeded'
 
-Building and Testing Locally
-----------------------------
-
-To get started with **stackql-deploy**, install it locally using pip:
-
-.. code-block:: none
-
-    pip install -e .
-
-Building and Deploying to PyPI
-------------------------------
-
-To distribute **stackql-deploy** on PyPI, you'll need to ensure that you have all required files set up correctly in your project directory. This typically includes your `setup.py`, `README.rst`, `LICENSE`, and any other necessary files.
-
-Building the Package
-^^^^^^^^^^^^^^^^^^^^
-
-First, ensure you have the latest versions of ``setuptools`` and ``wheel`` installed:
-
-.. code-block:: none
-
-    pip install --upgrade setuptools wheel
-
-Then, navigate to your project root directory and build the distribution files:
-
-.. code-block:: none
-
-    python3 setup.py sdist bdist_wheel
-
-This command generates distribution packages in the ``dist/`` directory.
-
-Uploading the Package to PyPI
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-To upload the package to PyPI, you'll need to use ``twine``, a utility for publishing Python packages. First, install ``twine``:
-
-.. code-block:: none
-
-    pip install twine
-
-Then, use `twine` to upload all of the archives under ``dist/``:
-
-.. code-block:: none
-
-    twine upload dist/*
-
-Building the Docs
-^^^^^^^^^^^^^^^^^
-Navigate to your ``docs`` directory and build the Sphinx documentation:
-
-.. code-block:: none
-
-    cd docs
-    make html
-
 **stackql-deploy** simplifies cloud resource management by treating infrastructure as flexible, dynamically assessed code.
 
 .. _stackql: https://github.com/stackql/stackql
```

### Comparing `stackql_deploy-1.0.2/README.rst` & `stackql_deploy-1.0.3/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -185,65 +185,10 @@
     /*+ postdeploy, retries=5, retry_delay=5 */
     SELECT COUNT(*) as count FROM azure.resources.resource_groups
     WHERE subscriptionId = '{{ subscription_id }}'
     AND resourceGroupName = '{{ resource_group_name }}'
     AND location = '{{ location }}'
     AND JSON_EXTRACT(properties, '$.provisioningState') = 'Succeeded'
 
-Building and Testing Locally
-----------------------------
-
-To get started with **stackql-deploy**, install it locally using pip:
-
-.. code-block:: none
-
-    pip install -e .
-
-Building and Deploying to PyPI
-------------------------------
-
-To distribute **stackql-deploy** on PyPI, you'll need to ensure that you have all required files set up correctly in your project directory. This typically includes your `setup.py`, `README.rst`, `LICENSE`, and any other necessary files.
-
-Building the Package
-^^^^^^^^^^^^^^^^^^^^
-
-First, ensure you have the latest versions of ``setuptools`` and ``wheel`` installed:
-
-.. code-block:: none
-
-    pip install --upgrade setuptools wheel
-
-Then, navigate to your project root directory and build the distribution files:
-
-.. code-block:: none
-
-    python3 setup.py sdist bdist_wheel
-
-This command generates distribution packages in the ``dist/`` directory.
-
-Uploading the Package to PyPI
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-To upload the package to PyPI, you'll need to use ``twine``, a utility for publishing Python packages. First, install ``twine``:
-
-.. code-block:: none
-
-    pip install twine
-
-Then, use `twine` to upload all of the archives under ``dist/``:
-
-.. code-block:: none
-
-    twine upload dist/*
-
-Building the Docs
-^^^^^^^^^^^^^^^^^
-Navigate to your ``docs`` directory and build the Sphinx documentation:
-
-.. code-block:: none
-
-    cd docs
-    make html
-
 **stackql-deploy** simplifies cloud resource management by treating infrastructure as flexible, dynamically assessed code.
 
 .. _stackql: https://github.com/stackql/stackql
```

### Comparing `stackql_deploy-1.0.2/setup.py` & `stackql_deploy-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.rst', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='stackql-deploy',
-    version='1.0.2',
+    version='1.0.3',
     description='Model driven resource provisioning and deployment framework using StackQL.',
     long_description=readme,
     author='Jeffrey Aven',
     author_email='javen@stackql.io',
     url='https://github.com/stackql/stackql-deploy',
     license='MIT',
     packages=find_packages(),
```

### Comparing `stackql_deploy-1.0.2/stackql_deploy/cli.py` & `stackql_deploy-1.0.3/stackql_deploy/cli.py`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.2/stackql_deploy.egg-info/PKG-INFO` & `stackql_deploy-1.0.3/stackql_deploy.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackql-deploy
-Version: 1.0.2
+Version: 1.0.3
 Summary: Model driven resource provisioning and deployment framework using StackQL.
 Home-page: https://github.com/stackql/stackql-deploy
 Author: Jeffrey Aven
 Author-email: javen@stackql.io
 License: MIT
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -209,65 +209,10 @@
     /*+ postdeploy, retries=5, retry_delay=5 */
     SELECT COUNT(*) as count FROM azure.resources.resource_groups
     WHERE subscriptionId = '{{ subscription_id }}'
     AND resourceGroupName = '{{ resource_group_name }}'
     AND location = '{{ location }}'
     AND JSON_EXTRACT(properties, '$.provisioningState') = 'Succeeded'
 
-Building and Testing Locally
-----------------------------
-
-To get started with **stackql-deploy**, install it locally using pip:
-
-.. code-block:: none
-
-    pip install -e .
-
-Building and Deploying to PyPI
-------------------------------
-
-To distribute **stackql-deploy** on PyPI, you'll need to ensure that you have all required files set up correctly in your project directory. This typically includes your `setup.py`, `README.rst`, `LICENSE`, and any other necessary files.
-
-Building the Package
-^^^^^^^^^^^^^^^^^^^^
-
-First, ensure you have the latest versions of ``setuptools`` and ``wheel`` installed:
-
-.. code-block:: none
-
-    pip install --upgrade setuptools wheel
-
-Then, navigate to your project root directory and build the distribution files:
-
-.. code-block:: none
-
-    python3 setup.py sdist bdist_wheel
-
-This command generates distribution packages in the ``dist/`` directory.
-
-Uploading the Package to PyPI
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-To upload the package to PyPI, you'll need to use ``twine``, a utility for publishing Python packages. First, install ``twine``:
-
-.. code-block:: none
-
-    pip install twine
-
-Then, use `twine` to upload all of the archives under ``dist/``:
-
-.. code-block:: none
-
-    twine upload dist/*
-
-Building the Docs
-^^^^^^^^^^^^^^^^^
-Navigate to your ``docs`` directory and build the Sphinx documentation:
-
-.. code-block:: none
-
-    cd docs
-    make html
-
 **stackql-deploy** simplifies cloud resource management by treating infrastructure as flexible, dynamically assessed code.
 
 .. _stackql: https://github.com/stackql/stackql
```

