# Comparing `tmp/azure_simple_email-0.0.9.tar.gz` & `tmp/azure_simple_email-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure_simple_email-0.0.9.tar", last modified: Thu Feb 15 15:03:44 2024, max compression
+gzip compressed data, was "azure_simple_email-0.1.0.tar", last modified: Wed Apr 17 06:21:33 2024, max compression
```

## Comparing `azure_simple_email-0.0.9.tar` & `azure_simple_email-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 15:03:44.135907 azure_simple_email-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-15 15:03:32.000000 azure_simple_email-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-02-15 15:03:44.135907 azure_simple_email-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-02-15 15:03:32.000000 azure_simple_email-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 15:03:44.135907 azure_simple_email-0.0.9/azure_simple_email/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 15:03:32.000000 azure_simple_email-0.0.9/azure_simple_email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-02-15 15:03:32.000000 azure_simple_email-0.0.9/azure_simple_email/azure_mail.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 15:03:44.135907 azure_simple_email-0.0.9/azure_simple_email.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-02-15 15:03:44.000000 azure_simple_email-0.0.9/azure_simple_email.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-02-15 15:03:44.000000 azure_simple_email-0.0.9/azure_simple_email.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 15:03:44.000000 azure_simple_email-0.0.9/azure_simple_email.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-15 15:03:44.000000 azure_simple_email-0.0.9/azure_simple_email.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-15 15:03:44.000000 azure_simple_email-0.0.9/azure_simple_email.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 15:03:44.135907 azure_simple_email-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-02-15 15:03:32.000000 azure_simple_email-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:21:33.459202 azure_simple_email-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-17 06:21:22.000000 azure_simple_email-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-17 06:21:33.459202 azure_simple_email-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-17 06:21:22.000000 azure_simple_email-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:21:33.459202 azure_simple_email-0.1.0/azure_simple_email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:21:22.000000 azure_simple_email-0.1.0/azure_simple_email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-17 06:21:22.000000 azure_simple_email-0.1.0/azure_simple_email/azure_mail.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:21:33.459202 azure_simple_email-0.1.0/azure_simple_email.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-17 06:21:33.000000 azure_simple_email-0.1.0/azure_simple_email.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-17 06:21:33.000000 azure_simple_email-0.1.0/azure_simple_email.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:21:33.000000 azure_simple_email-0.1.0/azure_simple_email.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-17 06:21:33.000000 azure_simple_email-0.1.0/azure_simple_email.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-17 06:21:33.000000 azure_simple_email-0.1.0/azure_simple_email.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 06:21:33.459202 azure_simple_email-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-17 06:21:22.000000 azure_simple_email-0.1.0/setup.py
```

### Comparing `azure_simple_email-0.0.9/LICENSE` & `azure_simple_email-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `azure_simple_email-0.0.9/PKG-INFO` & `azure_simple_email-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure_simple_email
-Version: 0.0.9
+Version: 0.1.0
 Summary: This is an esperimental library to send email using Microsoft Graph API
 Home-page: https://github.com/marcotn/azure_simple_email
 Author: Marco Pavanelli
 Author-email: marco.pavanelli@sasabz.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `azure_simple_email-0.0.9/README.md` & `azure_simple_email-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `azure_simple_email-0.0.9/azure_simple_email/azure_mail.py` & `azure_simple_email-0.1.0/azure_simple_email/azure_mail.py`

 * *Files identical despite different names*

### Comparing `azure_simple_email-0.0.9/azure_simple_email.egg-info/PKG-INFO` & `azure_simple_email-0.1.0/azure_simple_email.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure_simple_email
-Version: 0.0.9
+Version: 0.1.0
 Summary: This is an esperimental library to send email using Microsoft Graph API
 Home-page: https://github.com/marcotn/azure_simple_email
 Author: Marco Pavanelli
 Author-email: marco.pavanelli@sasabz.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `azure_simple_email-0.0.9/setup.py` & `azure_simple_email-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="azure_simple_email",
-    version="0.0.9",
+    version="0.1.0",
     author="Marco Pavanelli",
     author_email="marco.pavanelli@sasabz.it",
     description="This is an esperimental library to send email using Microsoft Graph API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/marcotn/azure_simple_email",
     packages=setuptools.find_packages(),
```

