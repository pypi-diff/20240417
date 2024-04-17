# Comparing `tmp/smtp_proxy-0.1.0.tar.gz` & `tmp/smtp_proxy-0.1.1.tar.gz`

## Comparing `smtp_proxy-0.1.0.tar` & `smtp_proxy-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 smtp_proxy-0.1.0/CHANGES.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smtp_proxy-0.1.0/src/smtp_proxy/__init__.py
--rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 smtp_proxy-0.1.0/src/smtp_proxy/smtp_proxy.py
--rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 smtp_proxy-0.1.0/tests/test_smtp_proxy.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 smtp_proxy-0.1.0/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 smtp_proxy-0.1.0/LICENSE
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 smtp_proxy-0.1.0/README.md
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 smtp_proxy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 smtp_proxy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 smtp_proxy-0.1.1/CHANGES.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smtp_proxy-0.1.1/src/smtp_proxy/__init__.py
+-rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 smtp_proxy-0.1.1/src/smtp_proxy/smtp_proxy.py
+-rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 smtp_proxy-0.1.1/tests/test_smtp_proxy.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 smtp_proxy-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 smtp_proxy-0.1.1/LICENSE
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 smtp_proxy-0.1.1/README.md
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 smtp_proxy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 smtp_proxy-0.1.1/PKG-INFO
```

### Comparing `smtp_proxy-0.1.0/src/smtp_proxy/smtp_proxy.py` & `smtp_proxy-0.1.1/src/smtp_proxy/smtp_proxy.py`

 * *Files identical despite different names*

### Comparing `smtp_proxy-0.1.0/tests/test_smtp_proxy.py` & `smtp_proxy-0.1.1/tests/test_smtp_proxy.py`

 * *Files identical despite different names*

### Comparing `smtp_proxy-0.1.0/LICENSE` & `smtp_proxy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smtp_proxy-0.1.0/pyproject.toml` & `smtp_proxy-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "smtp-proxy"
-version = "0.1.0"
+version = "0.1.1"
 description = "SMTP server meant to redirect SMTP requests to a third-party email provider"
 readme = "README.md"
 requires-python = ">=3"
 keywords = ["smtp", "email", "proxy"]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
```

### Comparing `smtp_proxy-0.1.0/PKG-INFO` & `smtp_proxy-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smtp-proxy
-Version: 0.1.0
+Version: 0.1.1
 Summary: SMTP server meant to redirect SMTP requests to a third-party email provider
 License-File: LICENSE
 Keywords: email,proxy,smtp
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

