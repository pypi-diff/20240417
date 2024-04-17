# Comparing `tmp/internet_domain_local-0.0.4.tar.gz` & `tmp/internet_domain_local-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "internet_domain_local-0.0.4.tar", last modified: Sat Apr 13 19:11:14 2024, max compression
+gzip compressed data, was "internet_domain_local-0.0.5.tar", last modified: Wed Apr 17 10:07:00 2024, max compression
```

## Comparing `internet_domain_local-0.0.4.tar` & `internet_domain_local-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:11:14.191152 internet_domain_local-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-13 19:11:14.191152 internet_domain_local-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-13 19:10:43.000000 internet_domain_local-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:11:14.187152 internet_domain_local-0.0.4/internet_domain_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:11:14.191152 internet_domain_local-0.0.4/internet_domain_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 19:10:43.000000 internet_domain_local-0.0.4/internet_domain_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8543 2024-04-13 19:10:43.000000 internet_domain_local-0.0.4/internet_domain_local/src/internet_domain_local.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-13 19:10:43.000000 internet_domain_local-0.0.4/internet_domain_local/src/internet_domain_local_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:11:14.191152 internet_domain_local-0.0.4/internet_domain_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-13 19:11:14.000000 internet_domain_local-0.0.4/internet_domain_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-13 19:11:14.000000 internet_domain_local-0.0.4/internet_domain_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 19:11:14.000000 internet_domain_local-0.0.4/internet_domain_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-13 19:11:14.000000 internet_domain_local-0.0.4/internet_domain_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-13 19:11:14.000000 internet_domain_local-0.0.4/internet_domain_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-13 19:10:43.000000 internet_domain_local-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 19:11:14.191152 internet_domain_local-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-13 19:10:43.000000 internet_domain_local-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:07:00.775770 internet_domain_local-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-17 10:07:00.775770 internet_domain_local-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 10:06:33.000000 internet_domain_local-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:07:00.771770 internet_domain_local-0.0.5/internet_domain_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:07:00.775770 internet_domain_local-0.0.5/internet_domain_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 10:06:33.000000 internet_domain_local-0.0.5/internet_domain_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8682 2024-04-17 10:06:33.000000 internet_domain_local-0.0.5/internet_domain_local/src/internet_domain_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-17 10:06:33.000000 internet_domain_local-0.0.5/internet_domain_local/src/internet_domain_local_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 10:07:00.775770 internet_domain_local-0.0.5/internet_domain_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-17 10:07:00.000000 internet_domain_local-0.0.5/internet_domain_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-17 10:07:00.000000 internet_domain_local-0.0.5/internet_domain_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 10:07:00.000000 internet_domain_local-0.0.5/internet_domain_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-17 10:07:00.000000 internet_domain_local-0.0.5/internet_domain_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-17 10:07:00.000000 internet_domain_local-0.0.5/internet_domain_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-17 10:06:33.000000 internet_domain_local-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 10:07:00.775770 internet_domain_local-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-17 10:06:33.000000 internet_domain_local-0.0.5/setup.py
```

### Comparing `internet_domain_local-0.0.4/PKG-INFO` & `internet_domain_local-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internet-domain-local
-Version: 0.0.4
+Version: 0.0.5
 Summary: PyPI Package for Circles internet-domain-local Python
 Home-page: https://github.com/circles-zone/internet-domain-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `internet_domain_local-0.0.4/internet_domain_local/src/internet_domain_local.py` & `internet_domain_local-0.0.5/internet_domain_local/src/internet_domain_local.py`

 * *Files 3% similar despite different names*

```diff
@@ -151,19 +151,22 @@
             if contact_internet_domain_id is None:
                 contact_internet_domain_id = self.insert_mapping(
                     entity_id1=contact_id, entity_id2=internet_domain_id,
                     ignore_duplicate=True
                 )
             # Add url to url_table
             # TODO: add url type
+            parsed_url = urlparse(url)
+            normalized_url = parsed_url.netloc + parsed_url.path.rstrip('/')
+
             data_json = {
-                'url': url
+                'url': normalized_url
             }
             data_json_compare = {
-                'url': url
+                'url': normalized_url
             }
             url_id = self.upsert(
                 schema_name='url',
                 table_name='url_table',
                 view_table_name='url_view',
                 data_json=data_json,
                 data_json_compare=data_json_compare
```

### Comparing `internet_domain_local-0.0.4/internet_domain_local/src/internet_domain_local_constants.py` & `internet_domain_local-0.0.5/internet_domain_local/src/internet_domain_local_constants.py`

 * *Files identical despite different names*

### Comparing `internet_domain_local-0.0.4/internet_domain_local.egg-info/PKG-INFO` & `internet_domain_local-0.0.5/internet_domain_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internet-domain-local
-Version: 0.0.4
+Version: 0.0.5
 Summary: PyPI Package for Circles internet-domain-local Python
 Home-page: https://github.com/circles-zone/internet-domain-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `internet_domain_local-0.0.4/setup.py` & `internet_domain_local-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PACKAGE_NAME = "internet-domain-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.4',  # update only the minor version each time # https://pypi.org/project/internet-domain-local/
+    version='0.0.5',  # update only the minor version each time # https://pypi.org/project/internet-domain-local/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles internet-domain-local Python",
     long_description="PyPI Package for Circles internet-domain-local Python",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/internet-domain-local-python-package",
     packages=[package_dir],
```

