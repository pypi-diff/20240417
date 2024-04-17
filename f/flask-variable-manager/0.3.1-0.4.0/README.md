# Comparing `tmp/flask-variable-manager-0.3.1.tar.gz` & `tmp/flask_variable_manager-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-variable-manager-0.3.1.tar", last modified: Fri Apr 12 14:35:37 2024, max compression
+gzip compressed data, was "flask_variable_manager-0.4.0.tar", last modified: Wed Apr 17 08:00:36 2024, max compression
```

## Comparing `flask-variable-manager-0.3.1.tar` & `flask_variable_manager-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:35:37.170586 flask-variable-manager-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-12 14:35:30.000000 flask-variable-manager-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-12 14:35:37.170586 flask-variable-manager-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-12 14:35:30.000000 flask-variable-manager-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:35:37.170586 flask-variable-manager-0.3.1/flask_variable_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-12 14:35:30.000000 flask-variable-manager-0.3.1/flask_variable_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:35:37.170586 flask-variable-manager-0.3.1/flask_variable_manager/extension/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:35:30.000000 flask-variable-manager-0.3.1/flask_variable_manager/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-04-12 14:35:30.000000 flask-variable-manager-0.3.1/flask_variable_manager/extension/variable_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:35:37.170586 flask-variable-manager-0.3.1/flask_variable_manager/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:35:30.000000 flask-variable-manager-0.3.1/flask_variable_manager/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-12 14:35:30.000000 flask-variable-manager-0.3.1/flask_variable_manager/tests/test_vm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:35:37.170586 flask-variable-manager-0.3.1/flask_variable_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-12 14:35:37.000000 flask-variable-manager-0.3.1/flask_variable_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-12 14:35:37.000000 flask-variable-manager-0.3.1/flask_variable_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:35:37.000000 flask-variable-manager-0.3.1/flask_variable_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-12 14:35:37.000000 flask-variable-manager-0.3.1/flask_variable_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 14:35:37.000000 flask-variable-manager-0.3.1/flask_variable_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-12 14:35:30.000000 flask-variable-manager-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:35:37.170586 flask-variable-manager-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:00:36.842660 flask_variable_manager-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-17 08:00:32.000000 flask_variable_manager-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-17 08:00:36.842660 flask_variable_manager-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-17 08:00:32.000000 flask_variable_manager-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:00:36.838660 flask_variable_manager-0.4.0/flask_variable_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-17 08:00:32.000000 flask_variable_manager-0.4.0/flask_variable_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:00:36.842660 flask_variable_manager-0.4.0/flask_variable_manager/extension/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:00:32.000000 flask_variable_manager-0.4.0/flask_variable_manager/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-04-17 08:00:32.000000 flask_variable_manager-0.4.0/flask_variable_manager/extension/variable_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:00:36.842660 flask_variable_manager-0.4.0/flask_variable_manager/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:00:32.000000 flask_variable_manager-0.4.0/flask_variable_manager/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-17 08:00:32.000000 flask_variable_manager-0.4.0/flask_variable_manager/tests/test_vm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:00:36.842660 flask_variable_manager-0.4.0/flask_variable_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-17 08:00:36.000000 flask_variable_manager-0.4.0/flask_variable_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-17 08:00:36.000000 flask_variable_manager-0.4.0/flask_variable_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 08:00:36.000000 flask_variable_manager-0.4.0/flask_variable_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-17 08:00:36.000000 flask_variable_manager-0.4.0/flask_variable_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-17 08:00:36.000000 flask_variable_manager-0.4.0/flask_variable_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-17 08:00:32.000000 flask_variable_manager-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 08:00:36.842660 flask_variable_manager-0.4.0/setup.cfg
```

### Comparing `flask-variable-manager-0.3.1/LICENSE` & `flask_variable_manager-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-variable-manager-0.3.1/PKG-INFO` & `flask_variable_manager-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-variable-manager
-Version: 0.3.1
+Version: 0.4.0
 Summary: Create a variable manager in flask, enter values in python, and use values on the jinja template.
 Author-email: minwook-shin <minwook0106@gmail.com>
 Project-URL: Homepage, https://github.com/minwook-shin/flask-variable-manager
 Project-URL: Bug Tracker, https://github.com/minwook-shin/flask-variable-manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -100,14 +100,26 @@
 import platform
 from flask import g
 data = additionalProp + "-" + platform.platform()
 g.local['saved_user_variable'] = data
 return data
 ```
 
+### Check the list of packages
+
+This route allows you to check the list of python packages.
+
+It accepts a GET request at the `/py/packages` endpoint.
+
+### install and uninstall a package
+
+This route allows you to install and uninstall a python package.
+
+It accepts a POST request at the `/py/install`, `/py/uninstall` endpoint.
+
 ## License
 
 This project is licensed under the terms of the MIT license.
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit a Pull Request.
```

### Comparing `flask-variable-manager-0.3.1/README.md` & `flask_variable_manager-0.4.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -79,14 +79,26 @@
 import platform
 from flask import g
 data = additionalProp + "-" + platform.platform()
 g.local['saved_user_variable'] = data
 return data
 ```
 
+### Check the list of packages
+
+This route allows you to check the list of python packages.
+
+It accepts a GET request at the `/py/packages` endpoint.
+
+### install and uninstall a package
+
+This route allows you to install and uninstall a python package.
+
+It accepts a POST request at the `/py/install`, `/py/uninstall` endpoint.
+
 ## License
 
 This project is licensed under the terms of the MIT license.
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit a Pull Request.
```

### Comparing `flask-variable-manager-0.3.1/flask_variable_manager/extension/variable_manager.py` & `flask_variable_manager-0.4.0/flask_variable_manager/extension/variable_manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -177,14 +177,87 @@
         del local_vars["_wrapped"]
         del local_vars["result"]
         unwanted_keys = [key for key in local_vars if key.startswith('__') and key.endswith('__')]
         for key in unwanted_keys:
             del local_vars[key]
         return jsonify({'result': str(result)})
 
+    @app.route('/py/install', methods=['POST'])
+    def install_python_package():
+        """
+        ---
+        tags:
+          - Python
+        summary: Install a Python package
+        description: This endpoint allows you to install a Python package.
+        parameters:
+          - in: formData
+            name: package_name
+            type: string
+            required: true
+            description: The name of the package to install.
+        responses:
+          200:
+            description: The package has been installed successfully.
+        """
+        package_name = request.form.get('package_name')
+        import subprocess
+        for package_name in package_name.split('\n'):
+            subprocess.run(['pip', 'install', package_name])
+        return jsonify({'message': 'The package has been installed successfully.'})
+
+    @app.route('/py/uninstall', methods=['POST'])
+    def uninstall_python_package():
+        """
+        ---
+        tags:
+          - Python
+        summary: Uninstall a Python package
+        description: This endpoint allows you to uninstall a Python package.
+        parameters:
+          - in: formData
+            name: package_name
+            type: string
+            required: true
+            description: The name of the package to uninstall.
+        responses:
+          200:
+            description: The package has been uninstalled successfully.
+        """
+        package_name = request.form.get('package_name')
+        import subprocess
+        for package_name in package_name.split('\n'):
+            subprocess.run(['pip', 'uninstall', '-y', package_name])
+        return jsonify({'message': 'The package has been uninstalled successfully.'})
+
+    @app.route('/py/packages', methods=['GET'])
+    def get_python_packages():
+        """
+        ---
+        tags:
+          - Python
+        summary: Get all installed Python packages
+        description: This endpoint allows you to get all installed Python packages.
+        responses:
+          200:
+            description: The installed packages have been retrieved successfully.
+            schema:
+              type: object
+              properties:
+                packages:
+                  type: array
+                  items:
+                    type: string
+                  description: The installed packages.
+        """
+        import subprocess
+        result = subprocess.run(['pip', 'freeze'], stdout=subprocess.PIPE)
+        packages = result.stdout.decode('utf-8').split('\n')
+        return jsonify({'packages': packages})
+
 
 class VariableManagerExtension:
     def __init__(self, app=None):
         self._local = Local()
         if app is not None:
             self.init_app(app)
```

### Comparing `flask-variable-manager-0.3.1/flask_variable_manager/tests/test_vm.py` & `flask_variable_manager-0.4.0/flask_variable_manager/tests/test_vm.py`

 * *Files identical despite different names*

### Comparing `flask-variable-manager-0.3.1/flask_variable_manager.egg-info/PKG-INFO` & `flask_variable_manager-0.4.0/flask_variable_manager.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-variable-manager
-Version: 0.3.1
+Version: 0.4.0
 Summary: Create a variable manager in flask, enter values in python, and use values on the jinja template.
 Author-email: minwook-shin <minwook0106@gmail.com>
 Project-URL: Homepage, https://github.com/minwook-shin/flask-variable-manager
 Project-URL: Bug Tracker, https://github.com/minwook-shin/flask-variable-manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -100,14 +100,26 @@
 import platform
 from flask import g
 data = additionalProp + "-" + platform.platform()
 g.local['saved_user_variable'] = data
 return data
 ```
 
+### Check the list of packages
+
+This route allows you to check the list of python packages.
+
+It accepts a GET request at the `/py/packages` endpoint.
+
+### install and uninstall a package
+
+This route allows you to install and uninstall a python package.
+
+It accepts a POST request at the `/py/install`, `/py/uninstall` endpoint.
+
 ## License
 
 This project is licensed under the terms of the MIT license.
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit a Pull Request.
```

### Comparing `flask-variable-manager-0.3.1/pyproject.toml` & `flask_variable_manager-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 include-package-data = false
 
 [tool.setuptools.packages.find]
 include = ['flask_variable_manager*']
 
 [project]
 name = "flask-variable-manager"
-version = "0.3.1"
+version = "0.4.0"
 description = "Create a variable manager in flask, enter values in python, and use values on the jinja template."
 authors = [
     { name = "minwook-shin", email = "minwook0106@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

