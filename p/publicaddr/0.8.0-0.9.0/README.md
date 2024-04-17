# Comparing `tmp/publicaddr-0.8.0.tar.gz` & `tmp/publicaddr-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "publicaddr-0.8.0.tar", last modified: Wed Sep 14 18:42:07 2022, max compression
+gzip compressed data, was "publicaddr-0.9.0.tar", last modified: Wed Sep 14 18:46:06 2022, max compression
```

## Comparing `publicaddr-0.8.0.tar` & `publicaddr-0.9.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 18:42:07.451199 publicaddr-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-14 18:41:55.000000 publicaddr-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3441 2022-09-14 18:42:07.451199 publicaddr-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2892 2022-09-14 18:41:55.000000 publicaddr-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 18:42:07.447199 publicaddr-0.8.0/publicaddr/
--rw-r--r--   0 runner    (1001) docker     (121)     7173 2022-09-14 18:41:55.000000 publicaddr-0.8.0/publicaddr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-09-14 18:41:55.000000 publicaddr-0.8.0/publicaddr/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     3951 2022-09-14 18:41:55.000000 publicaddr-0.8.0/publicaddr/handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1279 2022-09-14 18:41:55.000000 publicaddr-0.8.0/publicaddr/randprov.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 18:42:07.447199 publicaddr-0.8.0/publicaddr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3441 2022-09-14 18:42:07.000000 publicaddr-0.8.0/publicaddr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-09-14 18:42:07.000000 publicaddr-0.8.0/publicaddr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-14 18:42:07.000000 publicaddr-0.8.0/publicaddr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-09-14 18:42:07.000000 publicaddr-0.8.0/publicaddr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-09-14 18:42:07.000000 publicaddr-0.8.0/publicaddr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-14 18:42:07.451199 publicaddr-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-09-14 18:42:07.000000 publicaddr-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 18:42:07.447199 publicaddr-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-14 18:41:55.000000 publicaddr-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      844 2022-09-14 18:41:55.000000 publicaddr-0.8.0/tests/test_akamai.py
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-09-14 18:41:55.000000 publicaddr-0.8.0/tests/test_cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (121)      804 2022-09-14 18:41:55.000000 publicaddr-0.8.0/tests/test_google.py
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-09-14 18:41:55.000000 publicaddr-0.8.0/tests/test_icanhazip.py
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-09-14 18:41:55.000000 publicaddr-0.8.0/tests/test_ipify.py
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-09-14 18:41:55.000000 publicaddr-0.8.0/tests/test_lookup.py
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-09-14 18:41:55.000000 publicaddr-0.8.0/tests/test_opendns.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 18:46:06.213508 publicaddr-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-09-14 18:45:55.000000 publicaddr-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-09-14 18:45:55.000000 publicaddr-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3441 2022-09-14 18:46:06.213508 publicaddr-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2892 2022-09-14 18:45:55.000000 publicaddr-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 18:46:06.213508 publicaddr-0.9.0/publicaddr/
+-rw-r--r--   0 runner    (1001) docker     (121)     7173 2022-09-14 18:45:55.000000 publicaddr-0.9.0/publicaddr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      140 2022-09-14 18:45:55.000000 publicaddr-0.9.0/publicaddr/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3951 2022-09-14 18:45:55.000000 publicaddr-0.9.0/publicaddr/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1148 2022-09-14 18:45:55.000000 publicaddr-0.9.0/publicaddr/publicaddr.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1279 2022-09-14 18:45:55.000000 publicaddr-0.9.0/publicaddr/randprov.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 18:46:06.213508 publicaddr-0.9.0/publicaddr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3441 2022-09-14 18:46:06.000000 publicaddr-0.9.0/publicaddr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      498 2022-09-14 18:46:06.000000 publicaddr-0.9.0/publicaddr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-14 18:46:06.000000 publicaddr-0.9.0/publicaddr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2022-09-14 18:46:06.000000 publicaddr-0.9.0/publicaddr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-09-14 18:46:06.000000 publicaddr-0.9.0/publicaddr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-14 18:46:06.213508 publicaddr-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      910 2022-09-14 18:46:05.000000 publicaddr-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 18:46:06.213508 publicaddr-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-14 18:45:55.000000 publicaddr-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      844 2022-09-14 18:45:55.000000 publicaddr-0.9.0/tests/test_akamai.py
+-rw-r--r--   0 runner    (1001) docker     (121)      414 2022-09-14 18:45:55.000000 publicaddr-0.9.0/tests/test_cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (121)      804 2022-09-14 18:45:55.000000 publicaddr-0.9.0/tests/test_google.py
+-rw-r--r--   0 runner    (1001) docker     (121)      470 2022-09-14 18:45:55.000000 publicaddr-0.9.0/tests/test_icanhazip.py
+-rw-r--r--   0 runner    (1001) docker     (121)      460 2022-09-14 18:45:55.000000 publicaddr-0.9.0/tests/test_ipify.py
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2022-09-14 18:45:55.000000 publicaddr-0.9.0/tests/test_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (121)      406 2022-09-14 18:45:55.000000 publicaddr-0.9.0/tests/test_opendns.py
```

### Comparing `publicaddr-0.8.0/LICENSE` & `publicaddr-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `publicaddr-0.8.0/PKG-INFO` & `publicaddr-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: publicaddr
-Version: 0.8.0
+Version: 0.9.0
 Summary: Getting your public IP v4 and v6
 Home-page: https://github.com/dmachard/python-publicaddr
 Author: Denis MACHARD
 Author-email: d.machard@gmail.com
 Keywords: public ip dns http google akamai opendns cloudflare
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `publicaddr-0.8.0/README.md` & `publicaddr-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `publicaddr-0.8.0/publicaddr/__init__.py` & `publicaddr-0.9.0/publicaddr/__init__.py`

 * *Files identical despite different names*

### Comparing `publicaddr-0.8.0/publicaddr/handlers.py` & `publicaddr-0.9.0/publicaddr/handlers.py`

 * *Files identical despite different names*

### Comparing `publicaddr-0.8.0/publicaddr/randprov.py` & `publicaddr-0.9.0/publicaddr/randprov.py`

 * *Files identical despite different names*

### Comparing `publicaddr-0.8.0/publicaddr.egg-info/PKG-INFO` & `publicaddr-0.9.0/publicaddr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: publicaddr
-Version: 0.8.0
+Version: 0.9.0
 Summary: Getting your public IP v4 and v6
 Home-page: https://github.com/dmachard/python-publicaddr
 Author: Denis MACHARD
 Author-email: d.machard@gmail.com
 Keywords: public ip dns http google akamai opendns cloudflare
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `publicaddr-0.8.0/setup.py` & `publicaddr-0.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open("README.md", "r") as fh:
     LONG_DESCRIPTION = fh.read()
 
 KEYWORDS = ('public ip dns http google akamai opendns cloudflare')
 
 setuptools.setup(
     name="publicaddr",
-    version="0.8.0",
+    version="0.9.0",
     author="Denis MACHARD",
     author_email="d.machard@gmail.com",
     description="Getting your public IP v4 and v6",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/dmachard/python-publicaddr",
     packages=['publicaddr', 'tests'],
```

### Comparing `publicaddr-0.8.0/tests/test_akamai.py` & `publicaddr-0.9.0/tests/test_akamai.py`

 * *Files identical despite different names*

### Comparing `publicaddr-0.8.0/tests/test_google.py` & `publicaddr-0.9.0/tests/test_google.py`

 * *Files identical despite different names*

