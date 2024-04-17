# Comparing `tmp/pycis_cli-0.1.0.tar.gz` & `tmp/pycis_cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycis_cli-0.1.0.tar", max compression
+gzip compressed data, was "pycis_cli-0.1.1.tar", max compression
```

## Comparing `pycis_cli-0.1.0.tar` & `pycis_cli-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1083 2023-07-12 18:00:09.011444 pycis_cli-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0      394 2023-07-15 21:22:15.146910 pycis_cli-0.1.0/README.rst
--rw-r--r--   0        0        0     1024 2024-01-22 00:00:20.253428 pycis_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-13 03:17:30.118993 pycis_cli-0.1.0/source/packages/pycis/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 04:12:29.753800 pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/__init__.py
--rw-r--r--   0        0        0      768 2023-07-15 21:02:15.428500 pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/datastore/__init__.py
--rw-r--r--   0        0        0       43 2023-07-15 21:15:03.524375 pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/datastore/constants.py
--rw-r--r--   0        0        0      802 2023-07-15 21:02:15.432500 pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/datastore/couchdb/__init__.py
--rw-r--r--   0        0        0     2948 2023-07-19 22:27:05.917177 pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/datastore/couchdb/initialize.py
--rw-r--r--   0        0        0     3291 2023-10-24 03:40:54.475785 pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/datastore/couchdb/publish.py
--rw-r--r--   0        0        0      602 2023-07-15 21:02:15.432500 pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/datastore/mongodb/__init__.py
--rw-r--r--   0        0        0     2835 2023-10-23 20:37:15.702849 pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/datastore/mongodb/publish.py
--rw-r--r--   0        0        0      882 2023-09-05 02:09:16.097152 pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/document/__init__.py
--rw-r--r--   0        0        0     1367 2023-07-15 21:14:22.747367 pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/document/build/__init__.py
--rw-r--r--   0        0        0     2611 2023-07-15 21:16:57.763186 pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/document/build/addbyproduct.py
--rw-r--r--   0        0        0     2189 2023-07-15 21:16:57.759186 pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/document/build/addchange.py
--rw-r--r--   0        0        0     2748 2023-07-19 22:35:48.004906 pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/document/build/initialize.py
--rw-r--r--   0        0        0     2487 2023-07-15 21:16:57.759186 pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/document/build/setjobdetail.py
--rw-r--r--   0        0        0     2703 2023-07-15 21:16:57.755186 pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/document/build/update.py
--rw-r--r--   0        0        0      859 2023-09-05 02:08:20.859891 pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/document/configuration/__init__.py
--rw-r--r--   0        0        0     2168 2023-09-05 02:46:00.650817 pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/document/configuration/decrypt.py
--rw-r--r--   0        0        0     1846 2023-09-05 02:38:58.785434 pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/document/configuration/encrypt.py
--rw-r--r--   0        0        0      612 2023-07-15 21:02:15.432500 pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/document/testrun/__init__.py
--rw-r--r--   0        0        0     1708 2023-07-27 15:21:47.069389 pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/document/testrun/create.py
--rw-r--r--   0        0        0     1273 2023-07-15 21:02:15.428500 pycis_cli-0.1.0/source/packages/pycis/cli/pycis_command.py
--rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 pycis_cli-0.1.0/setup.py
--rw-r--r--   0        0        0     1353 1970-01-01 00:00:00.000000 pycis_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-01-26 02:55:36.937365 pycis_cli-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0      394 2024-01-26 02:55:36.937511 pycis_cli-0.1.1/README.rst
+-rw-r--r--   0        0        0     1024 2024-04-17 20:07:57.988900 pycis_cli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-26 02:55:36.939407 pycis_cli-0.1.1/source/packages/pycis/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:55:36.939494 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/__init__.py
+-rw-r--r--   0        0        0      768 2024-01-26 02:55:36.939649 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/datastore/__init__.py
+-rw-r--r--   0        0        0       43 2024-01-26 02:55:36.939728 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/datastore/constants.py
+-rw-r--r--   0        0        0      802 2024-01-26 02:55:36.939873 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/datastore/couchdb/__init__.py
+-rw-r--r--   0        0        0     2948 2024-01-26 02:55:36.940023 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/datastore/couchdb/initialize.py
+-rw-r--r--   0        0        0     3290 2024-04-17 20:07:28.153563 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/datastore/couchdb/publish.py
+-rw-r--r--   0        0        0      602 2024-01-26 02:55:36.940225 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/datastore/mongodb/__init__.py
+-rw-r--r--   0        0        0     2835 2024-01-26 02:55:36.940304 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/datastore/mongodb/publish.py
+-rw-r--r--   0        0        0      882 2024-01-26 02:55:36.940432 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/__init__.py
+-rw-r--r--   0        0        0     1367 2024-01-26 02:55:36.940557 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/build/__init__.py
+-rw-r--r--   0        0        0     2611 2024-01-26 02:55:36.940655 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/build/addbyproduct.py
+-rw-r--r--   0        0        0     2189 2024-01-26 02:55:36.940760 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/build/addchange.py
+-rw-r--r--   0        0        0     2748 2024-01-26 02:55:36.940851 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/build/initialize.py
+-rw-r--r--   0        0        0     2487 2024-01-26 02:55:36.940942 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/build/setjobdetail.py
+-rw-r--r--   0        0        0     2703 2024-01-26 02:55:36.941058 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/build/update.py
+-rw-r--r--   0        0        0      859 2024-01-26 02:55:36.941225 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/configuration/__init__.py
+-rw-r--r--   0        0        0     2168 2024-01-26 02:55:36.941347 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/configuration/decrypt.py
+-rw-r--r--   0        0        0     1846 2024-01-26 02:55:36.941437 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/configuration/encrypt.py
+-rw-r--r--   0        0        0      612 2024-01-26 02:55:36.941583 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/testrun/__init__.py
+-rw-r--r--   0        0        0     1708 2024-01-26 02:55:36.941711 pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/testrun/create.py
+-rw-r--r--   0        0        0     1273 2024-01-26 02:55:36.941794 pycis_cli-0.1.1/source/packages/pycis/cli/pycis_command.py
+-rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 pycis_cli-0.1.1/setup.py
+-rw-r--r--   0        0        0     1353 1970-01-01 00:00:00.000000 pycis_cli-0.1.1/PKG-INFO
```

### Comparing `pycis_cli-0.1.0/LICENSE.txt` & `pycis_cli-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.0/pyproject.toml` & `pycis_cli-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pycis-cli"
 description = "Python Continuous Integration System (PyCIS) - CLI Tools"
-version = "0.1.0"
+version = "0.1.1"
 authors = []
 readme = "README.rst"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX"
```

### Comparing `pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/datastore/__init__.py` & `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/datastore/couchdb/__init__.py` & `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/datastore/couchdb/__init__.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/datastore/couchdb/initialize.py` & `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/datastore/couchdb/initialize.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/datastore/couchdb/publish.py` & `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/datastore/couchdb/publish.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     docobj = None
     with open(filename, 'r') as sf:
         docobj = json.load(sf)
 
     if category != None:
         if "_id" in docobj:
             docid = docobj["_id"]
-            if docid.find(category) < -1:
+            if docid.find(category) < 0:
                 docid = f"{category}-{docid}"
                 docobj["_id"] = docid
         else:
             errmsg = "When specifying a 'category' the document must have an '_id' field."
             raise click.BadOptionUsage('category', errmsg)
 
     docobj["expiry_date"] = expiry_date.isoformat()
```

### Comparing `pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/datastore/mongodb/__init__.py` & `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/datastore/mongodb/__init__.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/datastore/mongodb/publish.py` & `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/datastore/mongodb/publish.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/document/__init__.py` & `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/__init__.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/document/build/__init__.py` & `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/build/__init__.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/document/build/addbyproduct.py` & `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/build/addbyproduct.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/document/build/addchange.py` & `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/build/addchange.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/document/build/initialize.py` & `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/build/initialize.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/document/build/setjobdetail.py` & `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/build/setjobdetail.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/document/build/update.py` & `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/build/update.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/document/configuration/__init__.py` & `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/document/configuration/decrypt.py` & `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/configuration/decrypt.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/document/configuration/encrypt.py` & `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/configuration/encrypt.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/document/testrun/__init__.py` & `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/testrun/__init__.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.0/source/packages/pycis/cli/cmdtree/document/testrun/create.py` & `pycis_cli-0.1.1/source/packages/pycis/cli/cmdtree/document/testrun/create.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.0/source/packages/pycis/cli/pycis_command.py` & `pycis_cli-0.1.1/source/packages/pycis/cli/pycis_command.py`

 * *Files identical despite different names*

### Comparing `pycis_cli-0.1.0/setup.py` & `pycis_cli-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 {'couchdb': ['couchdb>=1.2,<2.0'], 'mongodb': ['pymongo[srv]>=4.0.0,<5.0.0']}
 
 entry_points = \
 {'console_scripts': ['pycis = pycis.cli.pycis_command:pycis_root_command']}
 
 setup_kwargs = {
     'name': 'pycis-cli',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Python Continuous Integration System (PyCIS) - CLI Tools',
     'long_description': '========================================================\nPython Continuous Integration System (PyCIS) - CLI Tools\n========================================================\n\nProvides a set of CLI tools for working with the PyCIS continuous integration system.\n\n==========\nReferences\n==========\n\n- `User Guide <userguide/userguide.rst>`\n- `Coding Standards <userguide/10-00-coding-standards.rst>`\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pycis_cli-0.1.0/PKG-INFO` & `pycis_cli-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycis-cli
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python Continuous Integration System (PyCIS) - CLI Tools
 License: LICENSE.txt
 Keywords: python
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX
```

