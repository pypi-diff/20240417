# Comparing `tmp/crm1-0.1.0.tar.gz` & `tmp/crm1-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crm1-0.1.0.tar", max compression
+gzip compressed data, was "crm1-0.1.1.tar", max compression
```

## Comparing `crm1-0.1.0.tar` & `crm1-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1064 2024-04-12 20:13:20.045375 crm1-0.1.0/LICENSE
--rw-r--r--   0        0        0     4110 2024-04-12 20:13:20.045375 crm1-0.1.0/README.md
--rw-r--r--   0        0        0      139 2024-04-12 20:13:20.045375 crm1-0.1.0/crm1/__init__.py
--rw-r--r--   0        0        0      534 2024-04-12 20:13:20.045375 crm1-0.1.0/crm1/autorepotools.py
--rw-r--r--   0        0        0        0 2024-04-12 20:13:20.045375 crm1-0.1.0/crm1/helpers/__init__.py
--rw-r--r--   0        0        0     7075 2024-04-12 20:13:20.045375 crm1-0.1.0/crm1/helpers/versions.py
--rw-r--r--   0        0        0      677 2024-04-12 20:13:20.045375 crm1-0.1.0/crm1/spec/__init__.py
--rw-r--r--   0        0        0      176 2024-04-12 20:13:20.045375 crm1-0.1.0/crm1/spec/v1/__init__.py
--rw-r--r--   0        0        0     1972 2024-04-12 20:13:20.045375 crm1-0.1.0/crm1/spec/v1/common_modext.py
--rw-r--r--   0        0        0      436 2024-04-12 20:13:20.045375 crm1-0.1.0/crm1/spec/v1/dependency.py
--rw-r--r--   0        0        0      907 2024-04-12 20:13:20.045375 crm1-0.1.0/crm1/spec/v1/mod.py
--rw-r--r--   0        0        0      557 2024-04-12 20:13:20.045375 crm1-0.1.0/crm1/spec/v1/repository.py
--rw-r--r--   0        0        0      176 2024-04-12 20:13:20.045375 crm1-0.1.0/crm1/spec/v2/__init__.py
--rw-r--r--   0        0        0     1973 2024-04-12 20:13:20.045375 crm1-0.1.0/crm1/spec/v2/common_modext.py
--rw-r--r--   0        0        0      436 2024-04-12 20:13:20.045375 crm1-0.1.0/crm1/spec/v2/dependency.py
--rw-r--r--   0        0        0      907 2024-04-12 20:13:20.045375 crm1-0.1.0/crm1/spec/v2/mod.py
--rw-r--r--   0        0        0      680 2024-04-12 20:13:20.045375 crm1-0.1.0/crm1/spec/v2/repository.py
--rw-r--r--   0        0        0      142 2024-04-12 20:13:20.049375 crm1-0.1.0/crm1/types/__init__.py
--rw-r--r--   0        0        0     2156 2024-04-12 20:13:20.049375 crm1-0.1.0/crm1/types/dependency.py
--rw-r--r--   0        0        0     1093 2024-04-12 20:13:20.049375 crm1-0.1.0/crm1/types/mod.py
--rw-r--r--   0        0        0     3750 2024-04-12 20:13:20.049375 crm1-0.1.0/crm1/types/repository.py
--rw-r--r--   0        0        0     3125 2024-04-12 20:13:20.049375 crm1-0.1.0/crm1/types/repository_pool.py
--rw-r--r--   0        0        0      824 2024-04-12 20:13:20.049375 crm1-0.1.0/crm1/utils.py
--rw-r--r--   0        0        0      631 2024-04-12 20:13:20.049375 crm1-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4871 1970-01-01 00:00:00.000000 crm1-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-17 18:32:38.106831 crm1-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4110 2024-04-17 18:32:38.106831 crm1-0.1.1/README.md
+-rw-r--r--   0        0        0      139 2024-04-17 18:32:38.106831 crm1-0.1.1/crm1/__init__.py
+-rw-r--r--   0        0        0      534 2024-04-17 18:32:38.106831 crm1-0.1.1/crm1/autorepotools.py
+-rw-r--r--   0        0        0        0 2024-04-17 18:32:38.106831 crm1-0.1.1/crm1/helpers/__init__.py
+-rw-r--r--   0        0        0     8486 2024-04-17 18:32:38.106831 crm1-0.1.1/crm1/helpers/versions.py
+-rw-r--r--   0        0        0      677 2024-04-17 18:32:38.106831 crm1-0.1.1/crm1/spec/__init__.py
+-rw-r--r--   0        0        0      176 2024-04-17 18:32:38.106831 crm1-0.1.1/crm1/spec/v1/__init__.py
+-rw-r--r--   0        0        0     1972 2024-04-17 18:32:38.110831 crm1-0.1.1/crm1/spec/v1/common_modext.py
+-rw-r--r--   0        0        0      436 2024-04-17 18:32:38.110831 crm1-0.1.1/crm1/spec/v1/dependency.py
+-rw-r--r--   0        0        0      907 2024-04-17 18:32:38.110831 crm1-0.1.1/crm1/spec/v1/mod.py
+-rw-r--r--   0        0        0      557 2024-04-17 18:32:38.110831 crm1-0.1.1/crm1/spec/v1/repository.py
+-rw-r--r--   0        0        0      176 2024-04-17 18:32:38.110831 crm1-0.1.1/crm1/spec/v2/__init__.py
+-rw-r--r--   0        0        0     1973 2024-04-17 18:32:38.110831 crm1-0.1.1/crm1/spec/v2/common_modext.py
+-rw-r--r--   0        0        0      436 2024-04-17 18:32:38.110831 crm1-0.1.1/crm1/spec/v2/dependency.py
+-rw-r--r--   0        0        0      907 2024-04-17 18:32:38.110831 crm1-0.1.1/crm1/spec/v2/mod.py
+-rw-r--r--   0        0        0      680 2024-04-17 18:32:38.110831 crm1-0.1.1/crm1/spec/v2/repository.py
+-rw-r--r--   0        0        0      142 2024-04-17 18:32:38.110831 crm1-0.1.1/crm1/types/__init__.py
+-rw-r--r--   0        0        0     2156 2024-04-17 18:32:38.110831 crm1-0.1.1/crm1/types/dependency.py
+-rw-r--r--   0        0        0     1093 2024-04-17 18:32:38.110831 crm1-0.1.1/crm1/types/mod.py
+-rw-r--r--   0        0        0     3750 2024-04-17 18:32:38.110831 crm1-0.1.1/crm1/types/repository.py
+-rw-r--r--   0        0        0     3125 2024-04-17 18:32:38.110831 crm1-0.1.1/crm1/types/repository_pool.py
+-rw-r--r--   0        0        0      824 2024-04-17 18:32:38.110831 crm1-0.1.1/crm1/utils.py
+-rw-r--r--   0        0        0      631 2024-04-17 18:32:38.110831 crm1-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4871 1970-01-01 00:00:00.000000 crm1-0.1.1/PKG-INFO
```

### Comparing `crm1-0.1.0/LICENSE` & `crm1-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `crm1-0.1.0/README.md` & `crm1-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `crm1-0.1.0/crm1/autorepotools.py` & `crm1-0.1.1/crm1/autorepotools.py`

 * *Files identical despite different names*

### Comparing `crm1-0.1.0/crm1/spec/__init__.py` & `crm1-0.1.1/crm1/spec/__init__.py`

 * *Files identical despite different names*

### Comparing `crm1-0.1.0/crm1/spec/v1/common_modext.py` & `crm1-0.1.1/crm1/spec/v1/common_modext.py`

 * *Files identical despite different names*

### Comparing `crm1-0.1.0/crm1/spec/v1/mod.py` & `crm1-0.1.1/crm1/spec/v1/mod.py`

 * *Files identical despite different names*

### Comparing `crm1-0.1.0/crm1/spec/v1/repository.py` & `crm1-0.1.1/crm1/spec/v1/repository.py`

 * *Files identical despite different names*

### Comparing `crm1-0.1.0/crm1/spec/v2/common_modext.py` & `crm1-0.1.1/crm1/spec/v2/common_modext.py`

 * *Files identical despite different names*

### Comparing `crm1-0.1.0/crm1/spec/v2/mod.py` & `crm1-0.1.1/crm1/spec/v2/mod.py`

 * *Files identical despite different names*

### Comparing `crm1-0.1.0/crm1/spec/v2/repository.py` & `crm1-0.1.1/crm1/spec/v2/repository.py`

 * *Files identical despite different names*

### Comparing `crm1-0.1.0/crm1/types/dependency.py` & `crm1-0.1.1/crm1/types/dependency.py`

 * *Files identical despite different names*

### Comparing `crm1-0.1.0/crm1/types/mod.py` & `crm1-0.1.1/crm1/types/mod.py`

 * *Files identical despite different names*

### Comparing `crm1-0.1.0/crm1/types/repository.py` & `crm1-0.1.1/crm1/types/repository.py`

 * *Files identical despite different names*

### Comparing `crm1-0.1.0/crm1/types/repository_pool.py` & `crm1-0.1.1/crm1/types/repository_pool.py`

 * *Files identical despite different names*

### Comparing `crm1-0.1.0/crm1/utils.py` & `crm1-0.1.1/crm1/utils.py`

 * *Files identical despite different names*

### Comparing `crm1-0.1.0/pyproject.toml` & `crm1-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crm1"
-version = "0.1.0"
+version = "0.1.1"
 description = "A CRM-1 repository exploration package"
 authors = ["JoJoJux <johannes@jojojux.de>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/J0J0HA/py-crm1"
 homepage = "https://github.com/J0J0HA/py-crm1"
 keywords = ["crm1", "repository", "exploration", "python"]
```

### Comparing `crm1-0.1.0/PKG-INFO` & `crm1-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crm1
-Version: 0.1.0
+Version: 0.1.1
 Summary: A CRM-1 repository exploration package
 Home-page: https://github.com/J0J0HA/py-crm1
 License: MIT
 Keywords: crm1,repository,exploration,python
 Author: JoJoJux
 Author-email: johannes@jojojux.de
 Requires-Python: >=3.10,<4.0
```

