# Comparing `tmp/python_urbandict-0.3.4.tar.gz` & `tmp/python_urbandict-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_urbandict-0.3.4.tar", max compression
+gzip compressed data, was "python_urbandict-0.3.5.tar", max compression
```

## Comparing `python_urbandict-0.3.4.tar` & `python_urbandict-0.3.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1066 2024-04-03 00:18:50.181598 python_urbandict-0.3.4/LICENSE
--rw-r--r--   0        0        0     2325 2024-04-03 00:18:50.181598 python_urbandict-0.3.4/README.md
--rw-r--r--   0        0        0      954 2024-04-03 00:18:50.181598 python_urbandict-0.3.4/pyproject.toml
--rw-r--r--   0        0        0       77 2024-04-03 00:18:50.181598 python_urbandict-0.3.4/pyurbandict/__init__.py
--rw-r--r--   0        0        0     1211 2024-04-03 00:18:50.181598 python_urbandict-0.3.4/pyurbandict/parse.py
--rw-r--r--   0        0        0     3272 1970-01-01 00:00:00.000000 python_urbandict-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-17 19:02:38.144085 python_urbandict-0.3.5/LICENSE
+-rw-r--r--   0        0        0     2325 2024-04-17 19:02:38.144085 python_urbandict-0.3.5/README.md
+-rw-r--r--   0        0        0      954 2024-04-17 19:02:38.144085 python_urbandict-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0       77 2024-04-17 19:02:38.144085 python_urbandict-0.3.5/pyurbandict/__init__.py
+-rw-r--r--   0        0        0     1211 2024-04-17 19:02:38.144085 python_urbandict-0.3.5/pyurbandict/parse.py
+-rw-r--r--   0        0        0     3272 1970-01-01 00:00:00.000000 python_urbandict-0.3.5/PKG-INFO
```

### Comparing `python_urbandict-0.3.4/LICENSE` & `python_urbandict-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python_urbandict-0.3.4/README.md` & `python_urbandict-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `python_urbandict-0.3.4/pyproject.toml` & `python_urbandict-0.3.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.flake8]
 max-line-length = 88
 
 [tool.poetry]
 name = "python-urbandict"
-version = "0.3.4"
+version = "0.3.5"
 description = "Python wrapper for the Urban Dictionary API."
 authors = ["atbuy <contact.atbuy@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/atbuy/pyurbandict"
 repository = "https://github.com/atbuy/pyurbandict"
 keywords = ["urban", "dictionary", "api", "wrapper", "python"]
 include = ["README.md"]
```

### Comparing `python_urbandict-0.3.4/pyurbandict/parse.py` & `python_urbandict-0.3.5/pyurbandict/parse.py`

 * *Files identical despite different names*

### Comparing `python_urbandict-0.3.4/PKG-INFO` & `python_urbandict-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-urbandict
-Version: 0.3.4
+Version: 0.3.5
 Summary: Python wrapper for the Urban Dictionary API.
 Home-page: https://github.com/atbuy/pyurbandict
 License: MIT
 Keywords: urban,dictionary,api,wrapper,python
 Author: atbuy
 Author-email: contact.atbuy@gmail.com
 Requires-Python: >=3.9,<4.0
```

