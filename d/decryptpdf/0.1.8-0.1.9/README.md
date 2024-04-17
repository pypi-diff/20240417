# Comparing `tmp/decryptpdf-0.1.8.tar.gz` & `tmp/decryptpdf-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decryptpdf-0.1.8.tar", max compression
+gzip compressed data, was "decryptpdf-0.1.9.tar", max compression
```

## Comparing `decryptpdf-0.1.8.tar` & `decryptpdf-0.1.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     7049 2023-12-17 00:57:03.591776 decryptpdf-0.1.8/LICENSE
--rw-r--r--   0        0        0     3698 2023-12-17 00:57:03.591776 decryptpdf-0.1.8/README.md
--rw-r--r--   0        0        0     2533 2023-12-17 00:57:04.675777 decryptpdf-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       80 2023-12-17 00:57:03.591776 decryptpdf-0.1.8/src/decryptpdf/__init__.py
--rw-r--r--   0        0        0       59 2023-12-17 00:57:03.591776 decryptpdf-0.1.8/src/decryptpdf/__main__.py
--rw-r--r--   0        0        0      373 2023-12-17 00:57:03.591776 decryptpdf-0.1.8/src/decryptpdf/_main.py
--rw-r--r--   0        0        0     1537 2023-12-17 00:57:03.591776 decryptpdf-0.1.8/src/decryptpdf/cli.py
--rw-r--r--   0        0        0        0 2023-12-17 00:57:03.591776 decryptpdf-0.1.8/src/decryptpdf/py.typed
--rw-r--r--   0        0        0     4966 1970-01-01 00:00:00.000000 decryptpdf-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     7049 2023-12-17 12:24:01.551354 decryptpdf-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3698 2023-12-17 12:24:01.551354 decryptpdf-0.1.9/README.md
+-rw-r--r--   0        0        0     2533 2023-12-17 12:24:03.263348 decryptpdf-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-12-17 12:24:01.551354 decryptpdf-0.1.9/src/decryptpdf/__init__.py
+-rw-r--r--   0        0        0       59 2023-12-17 12:24:01.551354 decryptpdf-0.1.9/src/decryptpdf/__main__.py
+-rw-r--r--   0        0        0      373 2023-12-17 12:24:01.551354 decryptpdf-0.1.9/src/decryptpdf/_main.py
+-rw-r--r--   0        0        0     1537 2023-12-17 12:24:01.551354 decryptpdf-0.1.9/src/decryptpdf/cli.py
+-rw-r--r--   0        0        0        0 2023-12-17 12:24:01.551354 decryptpdf-0.1.9/src/decryptpdf/py.typed
+-rw-r--r--   0        0        0     4966 1970-01-01 00:00:00.000000 decryptpdf-0.1.9/PKG-INFO
```

### Comparing `decryptpdf-0.1.8/LICENSE` & `decryptpdf-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `decryptpdf-0.1.8/README.md` & `decryptpdf-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `decryptpdf-0.1.8/pyproject.toml` & `decryptpdf-0.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "decryptpdf"
-version = "0.1.8"
+version = "0.1.9"
 description = "Simple CLI tool for decrypting PDF files."
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "CC0 1.0 Universal"
 readme = "README.md"
 repository = "https://github.com/34j/decryptpdf"
 documentation = "https://decryptpdf.readthedocs.io"
 classifiers = [
```

### Comparing `decryptpdf-0.1.8/src/decryptpdf/cli.py` & `decryptpdf-0.1.9/src/decryptpdf/cli.py`

 * *Files identical despite different names*

### Comparing `decryptpdf-0.1.8/PKG-INFO` & `decryptpdf-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decryptpdf
-Version: 0.1.8
+Version: 0.1.9
 Summary: Simple CLI tool for decrypting PDF files.
 Home-page: https://github.com/34j/decryptpdf
 License: CC0 1.0 Universal
 Author: 34j
 Author-email: 34j.95a2p@simplelogin.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: decryptpdf Version: 0.1.8 Summary: Simple CLI tool
+Metadata-Version: 2.1 Name: decryptpdf Version: 0.1.9 Summary: Simple CLI tool
 for decrypting PDF files. Home-page: https://github.com/34j/decryptpdf License:
 CC0 1.0 Universal Author: 34j Author-email: 34j.95a2p@simplelogin.com Requires-
 Python: >=3.8,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: Other/Proprietary
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

