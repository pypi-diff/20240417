# Comparing `tmp/django_cacheable_model-1.2.0.tar.gz` & `tmp/django_cacheable_model-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_cacheable_model-1.2.0.tar", last modified: Fri Mar 29 12:03:14 2024, max compression
+gzip compressed data, was "django_cacheable_model-1.2.1.tar", last modified: Wed Apr 17 00:19:45 2024, max compression
```

## Comparing `django_cacheable_model-1.2.0.tar` & `django_cacheable_model-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 12:03:14.820362 django_cacheable_model-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)      568 2023-06-18 02:52:28.000000 django_cacheable_model-1.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2912 2024-03-29 12:03:14.820362 django_cacheable_model-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2363 2023-09-09 06:47:49.000000 django_cacheable_model-1.2.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      746 2024-03-29 11:58:37.000000 django_cacheable_model-1.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-29 12:03:14.820362 django_cacheable_model-1.2.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 12:03:14.816362 django_cacheable_model-1.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 12:03:14.820362 django_cacheable_model-1.2.0/src/django_cacheable_model/
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-03-29 11:58:37.000000 django_cacheable_model-1.2.0/src/django_cacheable_model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2498 2023-09-09 06:47:49.000000 django_cacheable_model-1.2.0/src/django_cacheable_model/models.py
--rw-rw-rw-   0 root         (0) root         (0)     4691 2023-06-29 02:21:26.000000 django_cacheable_model-1.2.0/src/django_cacheable_model/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 12:03:14.820362 django_cacheable_model-1.2.0/src/django_cacheable_model.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2912 2024-03-29 12:03:14.000000 django_cacheable_model-1.2.0/src/django_cacheable_model.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      393 2024-03-29 12:03:14.000000 django_cacheable_model-1.2.0/src/django_cacheable_model.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-29 12:03:14.000000 django_cacheable_model-1.2.0/src/django_cacheable_model.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-03-29 12:03:14.000000 django_cacheable_model-1.2.0/src/django_cacheable_model.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-03-29 12:03:14.000000 django_cacheable_model-1.2.0/src/django_cacheable_model.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 00:19:45.923744 django_cacheable_model-1.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)      568 2023-06-18 02:52:28.000000 django_cacheable_model-1.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2912 2024-04-17 00:19:45.919744 django_cacheable_model-1.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2363 2023-09-09 06:47:49.000000 django_cacheable_model-1.2.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      746 2024-04-17 00:13:21.000000 django_cacheable_model-1.2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 00:19:45.923744 django_cacheable_model-1.2.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 00:19:45.919744 django_cacheable_model-1.2.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 00:19:45.919744 django_cacheable_model-1.2.1/src/django_cacheable_model/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-04-17 00:13:21.000000 django_cacheable_model-1.2.1/src/django_cacheable_model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2498 2023-09-09 06:47:49.000000 django_cacheable_model-1.2.1/src/django_cacheable_model/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     4691 2023-06-29 02:21:26.000000 django_cacheable_model-1.2.1/src/django_cacheable_model/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 00:19:45.919744 django_cacheable_model-1.2.1/src/django_cacheable_model.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2912 2024-04-17 00:19:45.000000 django_cacheable_model-1.2.1/src/django_cacheable_model.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      393 2024-04-17 00:19:45.000000 django_cacheable_model-1.2.1/src/django_cacheable_model.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 00:19:45.000000 django_cacheable_model-1.2.1/src/django_cacheable_model.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-17 00:19:45.000000 django_cacheable_model-1.2.1/src/django_cacheable_model.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-17 00:19:45.000000 django_cacheable_model-1.2.1/src/django_cacheable_model.egg-info/top_level.txt
```

### Comparing `django_cacheable_model-1.2.0/LICENSE` & `django_cacheable_model-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_cacheable_model-1.2.0/PKG-INFO` & `django_cacheable_model-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_cacheable_model
-Version: 1.2.0
+Version: 1.2.1
 Summary: A cacheable Django model
 Author-email: "Harisankar Krishna Swamy @ Vevde" <harisankar.krishna@outlook.com>
 Project-URL: Homepage, https://github.com/harisankar-krishna-swamy/django_cacheable_model.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7.4
```

### Comparing `django_cacheable_model-1.2.0/README.md` & `django_cacheable_model-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `django_cacheable_model-1.2.0/pyproject.toml` & `django_cacheable_model-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["django_cacheable_model*"]
 namespaces = false
 
 [project]
 name = "django_cacheable_model"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="Harisankar Krishna Swamy @ Vevde", email="harisankar.krishna@outlook.com" },
 ]
 description = "A cacheable Django model"
 readme = "README.md"
 requires-python = ">=3.7.4"
 dependencies = [
```

### Comparing `django_cacheable_model-1.2.0/src/django_cacheable_model/models.py` & `django_cacheable_model-1.2.1/src/django_cacheable_model/models.py`

 * *Files identical despite different names*

### Comparing `django_cacheable_model-1.2.0/src/django_cacheable_model/utils.py` & `django_cacheable_model-1.2.1/src/django_cacheable_model/utils.py`

 * *Files identical despite different names*

### Comparing `django_cacheable_model-1.2.0/src/django_cacheable_model.egg-info/PKG-INFO` & `django_cacheable_model-1.2.1/src/django_cacheable_model.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_cacheable_model
-Version: 1.2.0
+Version: 1.2.1
 Summary: A cacheable Django model
 Author-email: "Harisankar Krishna Swamy @ Vevde" <harisankar.krishna@outlook.com>
 Project-URL: Homepage, https://github.com/harisankar-krishna-swamy/django_cacheable_model.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7.4
```

