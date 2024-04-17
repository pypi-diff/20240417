# Comparing `tmp/cesm-0.0.1.tar.gz` & `tmp/cesm-0.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cesm-0.0.1.tar", last modified: Tue Apr 16 15:05:38 2024, max compression
+gzip compressed data, was "cesm-0.0.1a0.tar", last modified: Wed Apr 17 13:21:10 2024, max compression
```

## Comparing `cesm-0.0.1.tar` & `cesm-0.0.1a0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 15:05:38.521126 cesm-0.0.1/
-drwxrwxrwx   0        0        0        0 2024-04-16 15:05:38.402431 cesm-0.0.1/Core/
--rw-rw-rw-   0        0        0        0 2023-10-24 14:59:49.000000 cesm-0.0.1/Core/__init__.py
--rw-rw-rw-   0        0        0    12046 2024-04-16 15:04:30.000000 cesm-0.0.1/Core/data_access.py
--rw-rw-rw-   0        0        0    12680 2024-04-16 15:05:25.000000 cesm-0.0.1/Core/input_parser.py
--rw-rw-rw-   0        0        0    19682 2024-04-16 13:57:56.000000 cesm-0.0.1/Core/model.py
--rw-rw-rw-   0        0        0     2035 2024-04-16 09:39:04.000000 cesm-0.0.1/Core/params.py
--rw-rw-rw-   0        0        0    12206 2024-04-11 15:21:04.000000 cesm-0.0.1/Core/plotter.py
--rw-rw-rw-   0        0        0     1118 2024-04-11 15:21:05.000000 cesm-0.0.1/LICENSE.md
--rw-rw-rw-   0        0        0      504 2024-04-16 15:05:38.513132 cesm-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3779 2024-04-16 09:41:51.000000 cesm-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 15:05:38.507129 cesm-0.0.1/cesm.egg-info/
--rw-rw-rw-   0        0        0      504 2024-04-16 15:05:37.000000 cesm-0.0.1/cesm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2024-04-16 15:05:38.000000 cesm-0.0.1/cesm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 15:05:37.000000 cesm-0.0.1/cesm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-04-16 15:05:37.000000 cesm-0.0.1/cesm.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       77 2024-04-16 15:05:37.000000 cesm-0.0.1/cesm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-16 15:05:37.000000 cesm-0.0.1/cesm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7557 2024-04-11 15:21:05.000000 cesm-0.0.1/cesm.py
--rw-rw-rw-   0        0        0       42 2024-04-16 15:05:38.522131 cesm-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      877 2024-04-16 14:50:09.000000 cesm-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 13:21:10.795258 cesm-0.0.1a0/
+drwxrwxrwx   0        0        0        0 2024-04-17 13:21:10.737266 cesm-0.0.1a0/Core/
+-rw-rw-rw-   0        0        0        0 2023-10-24 14:59:49.000000 cesm-0.0.1a0/Core/__init__.py
+-rw-rw-rw-   0        0        0    12046 2024-04-16 15:04:30.000000 cesm-0.0.1a0/Core/data_access.py
+-rw-rw-rw-   0        0        0    12672 2024-04-17 12:35:29.000000 cesm-0.0.1a0/Core/input_parser.py
+-rw-rw-rw-   0        0        0    19682 2024-04-16 13:57:56.000000 cesm-0.0.1a0/Core/model.py
+-rw-rw-rw-   0        0        0     2035 2024-04-16 09:39:04.000000 cesm-0.0.1a0/Core/params.py
+-rw-rw-rw-   0        0        0    12206 2024-04-11 15:21:04.000000 cesm-0.0.1a0/Core/plotter.py
+-rw-rw-rw-   0        0        0     1118 2024-04-11 15:21:05.000000 cesm-0.0.1a0/LICENSE.md
+-rw-rw-rw-   0        0        0      533 2024-04-17 13:21:10.791258 cesm-0.0.1a0/PKG-INFO
+-rw-rw-rw-   0        0        0     3779 2024-04-16 09:41:51.000000 cesm-0.0.1a0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 13:21:10.787088 cesm-0.0.1a0/cesm.egg-info/
+-rw-rw-rw-   0        0        0      533 2024-04-17 13:21:09.000000 cesm-0.0.1a0/cesm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2024-04-17 13:21:10.000000 cesm-0.0.1a0/cesm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 13:21:10.000000 cesm-0.0.1a0/cesm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-04-17 13:21:10.000000 cesm-0.0.1a0/cesm.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       88 2024-04-17 13:21:10.000000 cesm-0.0.1a0/cesm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-17 13:21:10.000000 cesm-0.0.1a0/cesm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7557 2024-04-11 15:21:05.000000 cesm-0.0.1a0/cesm.py
+-rw-rw-rw-   0        0        0       42 2024-04-17 13:21:10.797258 cesm-0.0.1a0/setup.cfg
+-rw-rw-rw-   0        0        0      908 2024-04-17 13:19:15.000000 cesm-0.0.1a0/setup.py
```

### Comparing `cesm-0.0.1/Core/data_access.py` & `cesm-0.0.1a0/Core/data_access.py`

 * *Files identical despite different names*

### Comparing `cesm-0.0.1/Core/input_parser.py` & `cesm-0.0.1a0/Core/input_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         self.scenario = scenario
 
         self.conn = db_conn
         self.cursor = self.conn.cursor()
 
         self.param_index_dict = Param_Index_Dict
 
-        file_path = pkg_resources.resource_filename('package_name', 'Core/init_queries.sql')
+        file_path = pkg_resources.resource_filename('cesm', 'Core/init_queries.sql')
         # Read queries from the .sql file
         with open(file_path, 'r') as file:
             queries = file.read()
 
         # Execute the queries
         self.cursor.executescript(queries)
```

### Comparing `cesm-0.0.1/Core/model.py` & `cesm-0.0.1a0/Core/model.py`

 * *Files identical despite different names*

### Comparing `cesm-0.0.1/Core/params.py` & `cesm-0.0.1a0/Core/params.py`

 * *Files identical despite different names*

### Comparing `cesm-0.0.1/Core/plotter.py` & `cesm-0.0.1a0/Core/plotter.py`

 * *Files identical despite different names*

### Comparing `cesm-0.0.1/LICENSE.md` & `cesm-0.0.1a0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cesm-0.0.1/README.md` & `cesm-0.0.1a0/README.md`

 * *Files identical despite different names*

### Comparing `cesm-0.0.1/cesm.py` & `cesm-0.0.1a0/cesm.py`

 * *Files identical despite different names*

### Comparing `cesm-0.0.1/setup.py` & `cesm-0.0.1a0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cesm',
-    version='0.0.1',
+    version='v0.0.1alpha.0',
     packages=find_packages(),
     package_data={
         'cesm': ['Data/*'],
     },
     py_modules=['cesm'],  # Assuming cesm.py is in the root of your package directory
     entry_points={
         'console_scripts': [
             'cesm = cesm:app',  # Assuming your main function is named main
         ],
     },
     install_requires=[
+        "setuptools",
         "openpyxl",
         "numpy",
         "scipy",
         "pandas",
         "gurobipy",
         "plotly",
         "kaleido",
```

