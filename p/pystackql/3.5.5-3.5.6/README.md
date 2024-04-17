# Comparing `tmp/pystackql-3.5.5.tar.gz` & `tmp/pystackql-3.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystackql-3.5.5.tar", last modified: Wed Apr 17 03:51:23 2024, max compression
+gzip compressed data, was "pystackql-3.5.6.tar", last modified: Wed Apr 17 04:49:32 2024, max compression
```

## Comparing `pystackql-3.5.5.tar` & `pystackql-3.5.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 03:51:23.008951 pystackql-3.5.5/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 pystackql-3.5.5/LICENSE
--rwxrwxrwx   0 javen     (1000) javen     (1000)     6997 2024-04-17 03:51:22.982606 pystackql-3.5.5/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)     5176 2024-04-17 03:50:46.000000 pystackql-3.5.5/README.rst
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 03:51:22.455032 pystackql-3.5.5/pystackql/
--rwxrwxrwx   0 javen     (1000) javen     (1000)      101 2024-04-12 21:02:08.000000 pystackql-3.5.5/pystackql/__init__.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     5209 2024-03-15 01:52:38.000000 pystackql-3.5.5/pystackql/_util.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1751 2024-03-15 01:52:38.000000 pystackql-3.5.5/pystackql/base_stackql_magic.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1740 2024-03-15 01:52:38.000000 pystackql-3.5.5/pystackql/magic.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1743 2024-03-15 01:52:38.000000 pystackql-3.5.5/pystackql/magics.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)    26007 2024-04-17 03:50:46.000000 pystackql-3.5.5/pystackql/stackql.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 03:51:22.955498 pystackql-3.5.5/pystackql.egg-info/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     6997 2024-04-17 03:51:21.000000 pystackql-3.5.5/pystackql.egg-info/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)      345 2024-04-17 03:51:21.000000 pystackql-3.5.5/pystackql.egg-info/SOURCES.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-04-17 03:51:21.000000 pystackql-3.5.5/pystackql.egg-info/dependency_links.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       24 2024-04-17 03:51:21.000000 pystackql-3.5.5/pystackql.egg-info/requires.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       10 2024-04-17 03:51:21.000000 pystackql-3.5.5/pystackql.egg-info/top_level.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-04-17 03:51:23.013531 pystackql-3.5.5/setup.cfg
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1254 2024-04-17 03:50:46.000000 pystackql-3.5.5/setup.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 03:51:22.872036 pystackql-3.5.5/tests/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     2348 2024-04-07 22:41:05.000000 pystackql-3.5.5/tests/test_params.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 04:49:32.325905 pystackql-3.5.6/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 pystackql-3.5.6/LICENSE
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     7019 2024-04-17 04:49:32.267235 pystackql-3.5.6/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     5198 2024-04-17 04:48:58.000000 pystackql-3.5.6/README.rst
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 04:49:30.737245 pystackql-3.5.6/pystackql/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      101 2024-04-12 21:02:08.000000 pystackql-3.5.6/pystackql/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     5209 2024-03-15 01:52:38.000000 pystackql-3.5.6/pystackql/_util.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1751 2024-03-15 01:52:38.000000 pystackql-3.5.6/pystackql/base_stackql_magic.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1740 2024-03-15 01:52:38.000000 pystackql-3.5.6/pystackql/magic.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1743 2024-03-15 01:52:38.000000 pystackql-3.5.6/pystackql/magics.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)    26027 2024-04-17 04:47:42.000000 pystackql-3.5.6/pystackql/stackql.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 04:49:32.171670 pystackql-3.5.6/pystackql.egg-info/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     7019 2024-04-17 04:49:27.000000 pystackql-3.5.6/pystackql.egg-info/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      345 2024-04-17 04:49:29.000000 pystackql-3.5.6/pystackql.egg-info/SOURCES.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-04-17 04:49:27.000000 pystackql-3.5.6/pystackql.egg-info/dependency_links.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       24 2024-04-17 04:49:28.000000 pystackql-3.5.6/pystackql.egg-info/requires.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       10 2024-04-17 04:49:28.000000 pystackql-3.5.6/pystackql.egg-info/top_level.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-04-17 04:49:32.337828 pystackql-3.5.6/setup.cfg
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1254 2024-04-17 04:48:58.000000 pystackql-3.5.6/setup.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 04:49:31.934096 pystackql-3.5.6/tests/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     2348 2024-04-07 22:41:05.000000 pystackql-3.5.6/tests/test_params.py
```

### Comparing `pystackql-3.5.5/LICENSE` & `pystackql-3.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pystackql-3.5.5/PKG-INFO` & `pystackql-3.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystackql
-Version: 3.5.5
+Version: 3.5.6
 Summary: A Python interface for StackQL
 Home-page: https://github.com/stackql/pystackql
 Author: Jeffrey Aven
 Author-email: javen@stackql.io
 License: MIT License
         
         Copyright (c) 2022 StackQL Studios
@@ -233,8 +233,8 @@
 Publishing the package
 ~~~~~~~~~~~~~~~~~~~~~~
 
 To publish the package to PyPI, run the following command:
 
 ::
 
-    twine upload dist/pystackql-3.5.5.tar.gz
+    twine upload --config-file .pypirc dist/pystackql-3.5.6.tar.gz
```

### Comparing `pystackql-3.5.5/README.rst` & `pystackql-3.5.6/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -190,8 +190,8 @@
 Publishing the package
 ~~~~~~~~~~~~~~~~~~~~~~
 
 To publish the package to PyPI, run the following command:
 
 ::
 
-    twine upload dist/pystackql-3.5.5.tar.gz
+    twine upload --config-file .pypirc dist/pystackql-3.5.6.tar.gz
```

### Comparing `pystackql-3.5.5/pystackql/_util.py` & `pystackql-3.5.6/pystackql/_util.py`

 * *Files identical despite different names*

### Comparing `pystackql-3.5.5/pystackql/base_stackql_magic.py` & `pystackql-3.5.6/pystackql/base_stackql_magic.py`

 * *Files identical despite different names*

### Comparing `pystackql-3.5.5/pystackql/magic.py` & `pystackql-3.5.6/pystackql/magic.py`

 * *Files identical despite different names*

### Comparing `pystackql-3.5.5/pystackql/magics.py` & `pystackql-3.5.6/pystackql/magics.py`

 * *Files identical despite different names*

### Comparing `pystackql-3.5.5/pystackql/stackql.py` & `pystackql-3.5.6/pystackql/stackql.py`

 * *Files 0% similar despite different names*

```diff
@@ -559,15 +559,15 @@
 						return pd.read_json(StringIO(output["data"]))
 					except ValueError:
 						return pd.DataFrame([{"error": "Invalid JSON output"}])
 				else:  # Assume 'dict' output
 					try:
 						return json.loads(output["data"])
 					except ValueError:
-						return {"error": "Invalid JSON output"}            
+						return {"error": f"Invalid JSON output : {output["data"]}"}            
 			else:
 				if "error" in output:
 					if suppress_errors:
 						return []
 					else:
 						return {"error": output["error"]}
```

### Comparing `pystackql-3.5.5/pystackql.egg-info/PKG-INFO` & `pystackql-3.5.6/pystackql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystackql
-Version: 3.5.5
+Version: 3.5.6
 Summary: A Python interface for StackQL
 Home-page: https://github.com/stackql/pystackql
 Author: Jeffrey Aven
 Author-email: javen@stackql.io
 License: MIT License
         
         Copyright (c) 2022 StackQL Studios
@@ -233,8 +233,8 @@
 Publishing the package
 ~~~~~~~~~~~~~~~~~~~~~~
 
 To publish the package to PyPI, run the following command:
 
 ::
 
-    twine upload dist/pystackql-3.5.5.tar.gz
+    twine upload --config-file .pypirc dist/pystackql-3.5.6.tar.gz
```

### Comparing `pystackql-3.5.5/setup.py` & `pystackql-3.5.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     readme = f.read()
 
 with open('LICENSE') as f:
     license = f.read()
 
 setup(
     name='pystackql',
-    version='3.5.5',
+    version='3.5.6',
     description='A Python interface for StackQL',
     long_description=readme,
     author='Jeffrey Aven',
     author_email='javen@stackql.io',
     url='https://github.com/stackql/pystackql',
     license=license,
     packages=['pystackql'],
```

### Comparing `pystackql-3.5.5/tests/test_params.py` & `pystackql-3.5.6/tests/test_params.py`

 * *Files identical despite different names*
