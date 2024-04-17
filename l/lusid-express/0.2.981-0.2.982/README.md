# Comparing `tmp/lusid_express-0.2.981.tar.gz` & `tmp/lusid_express-0.2.982.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_express-0.2.981.tar", last modified: Tue Apr 16 21:50:43 2024, max compression
+gzip compressed data, was "lusid_express-0.2.982.tar", last modified: Tue Apr 16 21:58:11 2024, max compression
```

## Comparing `lusid_express-0.2.981.tar` & `lusid_express-0.2.982.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 21:50:43.547955 lusid_express-0.2.981/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-16 21:50:40.000000 lusid_express-0.2.981/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       86 2024-04-16 21:50:40.000000 lusid_express-0.2.981/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6550 2024-04-16 21:50:43.547955 lusid_express-0.2.981/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5908 2024-04-16 21:50:40.000000 lusid_express-0.2.981/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 21:50:43.547955 lusid_express-0.2.981/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1538 2024-04-16 21:50:40.000000 lusid_express-0.2.981/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 21:50:43.543955 lusid_express-0.2.981/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 21:50:43.545956 lusid_express-0.2.981/src/lusid_express/
--rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-16 21:50:40.000000 lusid_express-0.2.981/src/lusid_express/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1918 2024-04-16 21:50:40.000000 lusid_express-0.2.981/src/lusid_express/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 21:50:43.546955 lusid_express-0.2.981/src/lusid_express/apis/
--rw-rw-rw-   0 root         (0) root         (0)     1414 2024-04-16 21:50:40.000000 lusid_express-0.2.981/src/lusid_express/apis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 21:50:43.546955 lusid_express-0.2.981/src/lusid_express/config/
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-16 21:50:40.000000 lusid_express-0.2.981/src/lusid_express/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1411 2024-04-16 21:50:40.000000 lusid_express-0.2.981/src/lusid_express/load.le
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 21:50:43.547955 lusid_express-0.2.981/src/lusid_express/markdown/
--rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-16 21:50:40.000000 lusid_express-0.2.981/src/lusid_express/markdown/PRELOADED_VARS.md
--rw-rw-rw-   0 root         (0) root         (0)      298 2024-04-16 21:50:40.000000 lusid_express-0.2.981/src/lusid_express/markdown/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 21:50:43.546955 lusid_express-0.2.981/src/lusid_express.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6550 2024-04-16 21:50:43.000000 lusid_express-0.2.981/src/lusid_express.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      484 2024-04-16 21:50:43.000000 lusid_express-0.2.981/src/lusid_express.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 21:50:43.000000 lusid_express-0.2.981/src/lusid_express.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      479 2024-04-16 21:50:43.000000 lusid_express-0.2.981/src/lusid_express.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-16 21:50:43.000000 lusid_express-0.2.981/src/lusid_express.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 21:58:11.111574 lusid_express-0.2.982/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-16 21:58:08.000000 lusid_express-0.2.982/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       86 2024-04-16 21:58:08.000000 lusid_express-0.2.982/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6550 2024-04-16 21:58:11.111574 lusid_express-0.2.982/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5908 2024-04-16 21:58:08.000000 lusid_express-0.2.982/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-16 21:58:11.111574 lusid_express-0.2.982/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1538 2024-04-16 21:58:08.000000 lusid_express-0.2.982/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 21:58:11.107574 lusid_express-0.2.982/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 21:58:11.109574 lusid_express-0.2.982/src/lusid_express/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-16 21:58:08.000000 lusid_express-0.2.982/src/lusid_express/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1918 2024-04-16 21:58:08.000000 lusid_express-0.2.982/src/lusid_express/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 21:58:11.110574 lusid_express-0.2.982/src/lusid_express/apis/
+-rw-rw-rw-   0 root         (0) root         (0)     1414 2024-04-16 21:58:08.000000 lusid_express-0.2.982/src/lusid_express/apis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 21:58:11.110574 lusid_express-0.2.982/src/lusid_express/config/
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-16 21:58:08.000000 lusid_express-0.2.982/src/lusid_express/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1407 2024-04-16 21:58:08.000000 lusid_express-0.2.982/src/lusid_express/load.le
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 21:58:11.111574 lusid_express-0.2.982/src/lusid_express/markdown/
+-rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-16 21:58:08.000000 lusid_express-0.2.982/src/lusid_express/markdown/PRELOADED_VARS.md
+-rw-rw-rw-   0 root         (0) root         (0)      298 2024-04-16 21:58:08.000000 lusid_express-0.2.982/src/lusid_express/markdown/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 21:58:11.110574 lusid_express-0.2.982/src/lusid_express.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6550 2024-04-16 21:58:11.000000 lusid_express-0.2.982/src/lusid_express.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      484 2024-04-16 21:58:11.000000 lusid_express-0.2.982/src/lusid_express.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 21:58:11.000000 lusid_express-0.2.982/src/lusid_express.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      479 2024-04-16 21:58:11.000000 lusid_express-0.2.982/src/lusid_express.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-16 21:58:11.000000 lusid_express-0.2.982/src/lusid_express.egg-info/top_level.txt
```

### Comparing `lusid_express-0.2.981/LICENSE` & `lusid_express-0.2.982/LICENSE`

 * *Files identical despite different names*

### Comparing `lusid_express-0.2.981/PKG-INFO` & `lusid_express-0.2.982/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid_express
-Version: 0.2.981
+Version: 0.2.982
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lusid_express-0.2.981/README.md` & `lusid_express-0.2.982/README.md`

 * *Files identical despite different names*

### Comparing `lusid_express-0.2.981/setup.py` & `lusid_express-0.2.982/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ]
 
 
 
 
 setup(
     name='lusid_express',
-    version='0.2.981',
+    version='0.2.982',
     package_dir={'': 'src'},  # tells setuptools that packages are under src
     packages=find_packages(where='src'),  # tells setuptools to look for packages in src
     install_requires=requirements,
     description='lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.',
     long_description=open('README.md').read(),
     include_package_data=True,  
     long_description_content_type='text/markdown',
```

### Comparing `lusid_express-0.2.981/src/lusid_express/__main__.py` & `lusid_express-0.2.982/src/lusid_express/__main__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-0.2.981/src/lusid_express/apis/__init__.py` & `lusid_express-0.2.982/src/lusid_express/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-0.2.981/src/lusid_express/load.le` & `lusid_express-0.2.982/src/lusid_express/load.le`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     if do_vars:
         from IPython import get_ipython
         ipython = get_ipython()
         
         # Perform imports and assign them to variables
         import lusid as lu
         import lusid.models as lm
-        import src.lusid_express.apis as apis
+        import lusid_express.apis as apis
 
         # Assign the modules to the IPython user namespace
         ipython.user_ns['lu'] = lu
         ipython.user_ns['lm'] = lm
         ipython.user_ns['apis'] = apis
     if do_magic:
         from IPython.core.magic import register_line_cell_magic
```

### Comparing `lusid_express-0.2.981/src/lusid_express/markdown/PRELOADED_VARS.md` & `lusid_express-0.2.982/src/lusid_express/markdown/PRELOADED_VARS.md`

 * *Files identical despite different names*

### Comparing `lusid_express-0.2.981/src/lusid_express.egg-info/PKG-INFO` & `lusid_express-0.2.982/src/lusid_express.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-express
-Version: 0.2.981
+Version: 0.2.982
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

